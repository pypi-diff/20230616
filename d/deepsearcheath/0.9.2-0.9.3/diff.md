# Comparing `tmp/deepsearcheath-0.9.2-py3-none-any.whl.zip` & `tmp/deepsearcheath-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 13691 bytes, number of entries: 7
+Zip file size: 13787 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       18 b- defN 22-Jan-23 07:47 deepsearcheath/__init__.py
--rw-r--r--  2.0 unx    52180 b- defN 23-Feb-22 07:14 deepsearcheath/deepsearch.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Feb-27 06:30 deepsearcheath-0.9.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      742 b- defN 23-Feb-27 06:30 deepsearcheath-0.9.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-27 06:30 deepsearcheath-0.9.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Feb-27 06:30 deepsearcheath-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      588 b- defN 23-Feb-27 06:30 deepsearcheath-0.9.2.dist-info/RECORD
-7 files, 64992 bytes uncompressed, 12641 bytes compressed:  80.5%
+-rw-r--r--  2.0 unx    49557 b- defN 23-Jun-16 09:32 deepsearcheath/deepsearch.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-16 09:36 deepsearcheath-0.9.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      742 b- defN 23-Jun-16 09:36 deepsearcheath-0.9.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 09:36 deepsearcheath-0.9.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-16 09:36 deepsearcheath-0.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      588 b- defN 23-Jun-16 09:36 deepsearcheath-0.9.3.dist-info/RECORD
+7 files, 62369 bytes uncompressed, 12737 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: deepsearcheath/__init__.py
 Comment: 
 
 Filename: deepsearcheath/deepsearch.py
 Comment: 
 
-Filename: deepsearcheath-0.9.2.dist-info/LICENSE
+Filename: deepsearcheath-0.9.3.dist-info/LICENSE
 Comment: 
 
-Filename: deepsearcheath-0.9.2.dist-info/METADATA
+Filename: deepsearcheath-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: deepsearcheath-0.9.2.dist-info/WHEEL
+Filename: deepsearcheath-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: deepsearcheath-0.9.2.dist-info/top_level.txt
+Filename: deepsearcheath-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: deepsearcheath-0.9.2.dist-info/RECORD
+Filename: deepsearcheath-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deepsearcheath/deepsearch.py

```diff
@@ -26,69 +26,176 @@
     
     @classmethod
     async def compute(cls, query, locale='ko_KR'):
         params = {
             'input': query,
             'locale': locale
         } 
+        _count = 0
+        while True:
+            try:
+                async with aiohttp.ClientSession() as sess:
 
-        async with aiohttp.ClientSession() as sess:
-            async with sess.post( url=cls._COMPUTE_API, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), data=params, timeout=120 ) as co_resp:
-                response_json = await co_resp.json()
-                if (co_resp.status != 200) or (not response_json['success']):
-                    try:
-                        print("Response code, Success status:", co_resp.status, response_json['success'])
-                    except:
-                        print(response_json)
-                    print("Exception query log:", query)
-                    print(response_json)
-                    return None
-
-                pods = response_json['data']['pods']  # pods[0]: input
-
-                if pods[1]['class'] == 'Result:DataFrame':
-                    data    =    pods[1]['content']['data']
-                    index   =   pods[1]['content']['index']
-                    dtypes  =  pods[1]['content']['dtypes']
-                    columns = pods[1]['content']['columns']
-
-                    results = []
-
-                    no_obs = len(data[columns[0]])
-                    for i in range(no_obs):
-                        item = dict()
-                        for col in columns:
-                            item[col] = data[col][i]
-                        results.append(item)
+                    async with sess.post( url=cls._COMPUTE_API, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), data=params, timeout=120 ) as co_resp:
+                        response_json = await co_resp.json()
+                        if (co_resp.status != 200) or (not response_json['success']):
+                            try:
+                                print("Response code, Success status:", co_resp.status, response_json['success'])
+                            except:
+                                print(response_json)
+                            print("Exception query log:", query)
+                            print(response_json)
+                            return None
+
+                        pods = response_json['data']['pods']  # pods[0]: input
+
+                        if pods[1]['class'] == 'Result:DataFrame':
+                            data    =    pods[1]['content']['data']
+                            index   =   pods[1]['content']['index']
+                            dtypes  =  pods[1]['content']['dtypes']
+                            columns = pods[1]['content']['columns']
+
+                            results = []
+
+                            no_obs = len(data[columns[0]])
+                            for i in range(no_obs):
+                                item = dict()
+                                for col in columns:
+                                    item[col] = data[col][i]
+                                results.append(item)
+
+                            df_results = pd.DataFrame(results)
+
+                            if df_results.empty:
+                                return None
+
+                            for col in dtypes.keys():  # pyarrow converting
+                                df_results[col] = df_results[col].astype(dtypes[col])
+
+                            df_results = df_results.set_index(index)  # 'symbol'
+                            df_results = df_results.sort_index()
+
+                            return df_results
+
+                        elif pods[1]['class'] == 'Result:DocumentTrendsResult':
+                            data    =    pods[1]['content']['data']
+                            trends  =   pods[1]['content']['data']['trends']
+                            total_matches = trends[0]['total_matches']
+                            buckets = trends[0]['buckets']
+
+                            df_results = pd.DataFrame(buckets)
+                            
+                            return df_results
 
-                    df_results = pd.DataFrame(results)
+                        else:
+                            return pods[1]['content']
+            
+            except Exception as e:
+                print("Exception query log:", query)
+                print(e)
+                _count += 1
+                if _count > 5:
+                    return [None]
+                time.sleep(5)
+                continue
 
-                    if df_results.empty:
-                        return None
 
-                    for col in dtypes.keys():  # pyarrow converting
-                        df_results[col] = df_results[col].astype(dtypes[col])
 
-                    df_results = df_results.set_index(index)  # 'symbol'
-                    df_results = df_results.sort_index()
+class asyncDeepSearchAPI_mk2(object):
+    _COMPUTE_API = "{}/v1/compute".format('https://api.deepsearch.com')
+    _AUTH_ID = os.getenv('_AUTH_ID')
+    _AUTH_PW = os.getenv('_AUTH_PW')
+    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
+    
+    @classmethod
+    async def compute(cls, query, locale='ko_KR', timeout=120, max_count=5, sentiment=False):
+        params = {
+            'input': query,
+            'locale': locale
+        } 
+        _count = 0
+        retry = False
+        while True:
+            try:
+                async with aiohttp.ClientSession() as sess:
 
-                    return df_results
+                    async with sess.post( url=cls._COMPUTE_API, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), data=params, timeout=timeout ) as co_resp:
+                        response_json = await co_resp.json()
+                        if (co_resp.status != 200) or (not response_json['success']):
+                            print("Response code, Success status:", co_resp.status, response_json['success'])
+                            if sentiment:
+                                raise Exception("Response code, Success status:", co_resp.status, response_json['success'])
+                            return None, query
+                            return None
+
+                        pods = response_json['data']['pods']  # pods[0]: input
+
+                        if pods[1]['class'] == 'Result:DataFrame':
+                            data    =    pods[1]['content']['data']
+                            index   =   pods[1]['content']['index']
+                            dtypes  =  pods[1]['content']['dtypes']
+                            columns = pods[1]['content']['columns']
+
+                            results = []
+
+                            no_obs = len(data[columns[0]])
+                            for i in range(no_obs):
+                                item = dict()
+                                for col in columns:
+                                    item[col] = data[col][i]
+                                results.append(item)
+
+                            df_results = pd.DataFrame(results)
+
+                            if df_results.empty:
+                                print("Empty DataFrame:", query)
+                                return None, query
+                                return None
+
+                            for col in dtypes.keys():  # pyarrow converting
+                                df_results[col] = df_results[col].astype(dtypes[col])
+
+                            df_results = df_results.set_index(index)  # 'symbol'
+                            df_results = df_results.sort_index()
+
+                            if retry: print("retry success")
+                            return df_results, query
+                            return df_results
+
+                        elif pods[1]['class'] == 'Result:DocumentTrendsResult':
+                            data    =    pods[1]['content']['data']
+                            trends  =   pods[1]['content']['data']['trends']
+                            total_matches = trends[0]['total_matches']
+                            buckets = trends[0]['buckets']
+
+                            df_results = pd.DataFrame(buckets)
+                            
+                            if retry: print("retry success")
+                            return df_results, query
+                            return df_results
 
-                elif pods[1]['class'] == 'Result:DocumentTrendsResult':
-                    data    =    pods[1]['content']['data']
-                    trends  =   pods[1]['content']['data']['trends']
-                    total_matches = trends[0]['total_matches']
-                    buckets = trends[0]['buckets']
+                        else:
+                            if retry: print("retry success")
+                            return pods[1]['content'], query
+                            return pods[1]['content']
+            
+            except Exception as e:
+                retry = True
+                print("Exception query log:", query)
+                print(e)
+                _count += 1
+                print(_count)
+                if _count > max_count:
+                    print('max count exceeded')
+                    return [None], query
+                    return [None]
+                time.sleep(5)
+                continue
 
-                    df_results = pd.DataFrame(buckets)
-                    
-                    return df_results
 
-                else:
-                    return pods[1]['content']
 
 
 class DeepSearchAPI(object):
     _COMPUTE_API = "{}/v1/compute".format('https://api.deepsearch.com')
     _AUTH_ID = os.getenv('_AUTH_ID')
     _AUTH_PW = os.getenv('_AUTH_PW')
     _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
@@ -305,37 +412,37 @@
     async_deepsearch = asyncDeepSearchAPI()
     wavelet = WaveletAPI()
     
     loop = asyncio.get_event_loop()
     fdr_krx = fdr.StockListing('KRX')
     fdr_krx_delisted = fdr.StockListing('KRX-DELISTING')
 
-    def _split_phases(cls, deepsearch_df):
+    def _split_phases(cls, deepsearch_df:pd.DataFrame) -> dict:
         return_dict = dict()
         phases = deepsearch_df.index.unique()
         for p in phases:
             pdf = deepsearch_df.loc[p]
             return_dict[p] = pdf
         return return_dict
 
-    def _is_business_day(date):
+    def _is_business_day(date) -> bool:
         return bool(len(pd.bdate_range(date, date)))
 
-    def _datetime_reformer(date):
+    def _datetime_reformer(date:str) -> datetime:
         formats = [
             "%Y-%m-%d", 
             "%m/%d/%Y",
         ]
         for i in formats:
             try: _datetime = datetime.strptime(date, i)
             except: continue
         return _datetime  #! formats 에 없는 형식일 경우 에러
 
     @classmethod
-    async def _async_main(cls, symbol_list, date_from, date_to, krx=True):
+    async def _async_main(cls, symbol_list, date_from, date_to, krx=True) -> list or None:
         start = "'"
         separator = "', '"
         query = f"GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=['change_rate'], date_from={date_from}, date_to={date_to})"
         task = [cls.async_deepsearch.compute(query)]
         result = await asyncio.gather(*task)
         return result
         """
@@ -356,37 +463,37 @@
             separator = "', '"
             query = f'Global.GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=["close"], date_from={date_from}, date_to={date_to})'
         task = [cls.async_deepsearch.compute(query)]
         result = await asyncio.gather(*task)
         return result
         """
 
-    def _async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to, krx=True):
+    def _async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to, krx=True) -> list[pd.DataFrame] or list[None]:
         async_data_krx = cls.loop.run_until_complete( cls._async_main( [i for i in chunk_krx], _date_from, _date_to ) )
         if len(chunk_krx_not) > 0:
             async_data_krx_not = cls.loop.run_until_complete( cls._async_main( [i for i in chunk_krx_not], _date_from, _date_to, krx=False) )
             async_data_krx_not = [ cls._nonkrx_handler(async_data_krx_not[0], _date_from, _date_to) ]
             async_data = [ pd.concat([async_data_krx[0], async_data_krx_not[0]]) ]
         else:
             async_data = async_data_krx
         return async_data
 
 
     @classmethod
-    def _nonkrx_handler(cls, async_data_krx_not_df, _date_from, _date_to):
+    def _nonkrx_handler(cls, async_data_krx_not_df, _date_from, _date_to) -> pd.DataFrame:
         won_dollar = cls.deepsearch.compute('QueryBankOfKoreaSeriesData("BOK:731Y001.0000001")')
         async_data_krx_not = async_data_krx_not_df.rename({'close':f'주가 {_date_from}-{_date_to}'}, axis=1)
         wd_stockprice = pd.merge(async_data_krx_not.reset_index(), won_dollar.reset_index()).set_index(['date', 'symbol'])
         wd_stockprice[f'주가 {_date_from}-{_date_to}'] = wd_stockprice.loc[:, f'주가 {_date_from}-{_date_to}'] * wd_stockprice.loc[:, 'QueryBankOfKoreaSeriesData(BOK:731Y001.0000001)']
         async_data_krx_not[f'주가 {_date_from}-{_date_to}'] = wd_stockprice[f'주가 {_date_from}-{_date_to}']
         return async_data_krx_not
 
 
     @classmethod
-    def _fdr_handler(cls, symbol, _date_from, _date_to):
+    def _fdr_handler(cls, symbol, _date_from, _date_to) -> pd.DataFrame:
         if "KRX:" in symbol: symbol = symbol.split(":")[-1]
         if "NICE:" in symbol: symbol = symbol.split(":")[-1]
         _resp = fdr.DataReader(symbol,_date_from,_date_to)
         if symbol in list(cls.fdr_krx["Symbol"]): 
             _entity_name = cls.fdr_krx[cls.fdr_krx["Symbol"] == symbol]["Name"].values[0]
         else: 
             _entity_name = cls.fdr_krx_delisted[cls.fdr_krx_delisted["Symbol"] == symbol]["Name"].values[0]
@@ -411,15 +518,15 @@
         _resp.columns = ["date", "symbol", "entity_name", f"주가 {_date_from}-{_date_to}"]
         _resp = _resp.set_index(["date", "symbol"])
         return _resp
         """
 
 
     @classmethod
-    def _pdr_naver_handler(cls, chunk_krx, ticker_name_df, _date_from, _date_to):
+    def _pdr_naver_handler(cls, chunk_krx, ticker_name_df, _date_from, _date_to) -> list[pd.DataFrame]:
         """
         _date_from 은 change_rate 과 호환되어야 한다. 
         """
         # 220630 맘스터치 상폐 / 007460 무증
         resp_basket = pd.DataFrame()
         for idx, ticker in enumerate(chunk_krx):
             _ticker = ticker.replace("KRX:", "")
@@ -430,16 +537,16 @@
             _resp['date'] = _resp['Date']
             _resp["change_rate"] = _resp["close"].astype(float).pct_change()
             _resp = _resp[["date", "symbol", "entity_name", "change_rate"]]
 
             date_for_change_rate = ((_resp["date"] < pd.to_datetime(_date_from))).replace(False, np.nan).dropna()
             if len(date_for_change_rate) == 0: pass  # _start 이전 데이터가 없는 경우
             else:
-                resp = _resp.iloc[date_for_change_rate.index[-1] +1:]
-            resp_basket = pd.concat([resp_basket, resp], axis=0)
+                _resp = _resp.iloc[date_for_change_rate.index[-1] +1:]
+            resp_basket = pd.concat([resp_basket, _resp], axis=0)
         async_data = [resp_basket.sort_values(["date", "symbol"]).set_index(["date", "symbol"])]
         return async_data
 
 
     @classmethod
     def compute(cls, deepsearch_df, df_to_upload_bool=False, debug=False, fdr=False, naver=False):
         
@@ -453,14 +560,17 @@
         df = cls._split_phases(cls, deepsearch_df)
         rebalancing_dates = list(df.keys())
         for idx, date in enumerate(rebalancing_dates):
             if datetime.today() < cls._datetime_reformer(date):
                 print(rebalancing_dates, rebalancing_dates[:idx])
                 rebalancing_dates = rebalancing_dates[:idx]
                 break
+        """ 종가매수 """
+        if (rebalancing_dates[-1] == datetime.today().strftime("%m/%d/%Y")): 
+            rebalancing_dates = rebalancing_dates[:-1]
 
 
         _async_batch_size = 10
 
         cls._aum = 100_000_000_000.0  #! 변수 초기화
 
         total_return = pd.DataFrame()
@@ -583,14 +693,18 @@
                 for i in range(len(pdf)//_async_batch_size +1):
                     chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
                     
                     chunk = pdf[chunk_start:chunk_end]
                     chunk_krx = [i for i in chunk if (i.startswith('KRX:') | i.startswith('NICE:'))]
                     chunk_krx_not = set(chunk) - set(chunk_krx)
 
+                    if len(chunk) != len(chunk_krx):
+                        print(chunk)
+                        print(chunk_krx)
+
                     if len(chunk) == 0: break
                     if naver:
                         async_data = []
                         try: _async_data = cls._pdr_naver_handler(cls, chunk_krx, ticker_name_df, _date_from, _date_to)
                         except: _async_data = cls._pdr_naver_handler(chunk_krx, ticker_name_df, _date_from, _date_to)
                         async_data = async_data +_async_data
                     else:   
@@ -598,69 +712,15 @@
                         except: async_data = cls._async_main_wrapper( chunk_krx, chunk_krx_not, _date_from, _date_to)
 
 
                     for data in async_data:
                         # data.columns = ['entity_name', 'close']
                         data.columns = ['entity_name', 'change_rate']  #! 데이터가 안받아져 왔을 시 죽는다
                         async_result = pd.concat([async_result, data], axis=0)
-                '''
-                _date_from = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")
-                _date_to = datetime.strftime(datetime.today().date(), "%Y-%m-%d")
-
-                for i in range(len(pdf)//_async_batch_size +1):
-                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
-                    
-                    chunk = pdf[chunk_start:chunk_end]
-                    chunk_krx = [i for i in chunk if (i.startswith('KRX:') | i.startswith('NICE:'))]
-                    chunk_krx_not = list(set(chunk) - set(chunk_krx))
-
-                    # chunk_krx = chunk_krx[chunk_start:chunk_end]
-                    # chunk_krx_not = chunk_krx_not[chunk_start:chunk_end]
-
-
-                    if len(chunk) == 0: break
-                    #! 왜 다른가?
-                    """try: 
-                        async_data_krx = loop.run_until_complete( cls._async_main( cls, [i for i in chunk_krx], _date_from, _date_to) )  # datetime.strftime(datetime.today(), "%Y-%m-%d")
-                        if len(chunk_krx_not) > 0:
-                            async_data_krx_not = loop.run_until_complete( cls._async_main( cls, [i for i in chunk_krx_not], _date_from, _date_to, krx=False) )
-                            async_data_krx_not = [ cls._nonkrx_handler(async_data_krx_not[0], _date_from, _date_to) ]
-                            async_data = [ pd.concat([async_data_krx[0], async_data_krx_not[0]]) ]
-                        else:
-                            async_data = async_data_krx
-                    except: 
-                        async_data_krx = loop.run_until_complete( cls._async_main( [i for i in chunk_krx], _date_from, _date_to) )  # datetime.strftime(datetime.today(), "%Y-%m-%d")
-                        if len(chunk_krx_not) > 0:
-                            async_data_krx_not = loop.run_until_complete( cls._async_main( [i for i in chunk_krx_not], _date_from, _date_to, krx=False) )
-                            async_data_krx_not = [ cls._nonkrx_handler(async_data_krx_not[0], _date_from, _date_to) ]
-                            async_data = [ pd.concat([async_data_krx[0], async_data_krx_not[0]]) ]
-                        else:
-                            async_data = async_data_krx"""
-                    # if (datetime.strptime(_date_from, "%Y-%m-%d") < datetime(2022, 9, 28)) & (datetime(2022, 9, 28) < datetime.strptime(_date_to, "%Y-%m-%d")):
-                    #     _async_data_fdr = pd.DataFrame()
-                    #     for symbol in chunk_krx:
-                    #         if "NICE:" in symbol:
-                    #             symbol = _df[_df["symbol"]==symbol].iloc[0]["symbol_listed"]
-                    #         try:  # TypeError: _fdr_handler() takes 4 positional arguments but 5 were given
-                    #             _async_resp = cls._fdr_handler( symbol, _date_from, _date_to)
-                    #         except:
-                    #             _async_resp = cls._fdr_handler(cls, symbol, _date_from, _date_to)
-                    #         _async_data_fdr = pd.concat([_async_data_fdr, _async_resp]).sort_index()
-                    #     async_data = [_async_data_fdr]
-                    # else:
-                    try: 
-                        async_data = cls._async_main_wrapper( chunk_krx, chunk_krx_not, _date_from, _date_to)
-                    except:
-                        async_data = cls._async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to)
-
-
-                    for data in async_data:
-                        data.columns = ['entity_name', 'close']
-                        async_result = pd.concat([async_result, data], axis=0)'''
-            
+                
             async_result_reset = async_result.reset_index()
 
             
             #####################################################################################################################
             #* close
             # pdf_returns_ds = async_result_reset.drop_duplicates(subset=['date', 'symbol'], keep='first').pivot(index='date', columns='symbol', values='close').ffill()
             # pdf_returns_async = (pdf_returns_ds.pct_change().fillna(0) +1).cumprod()  #! NICE가 없다
@@ -691,78 +751,14 @@
 
         if debug == True:
             import pdb
             pdb.set_trace()
 
         total_return = total_return.groupby(total_return.index).first()
 
-        # cls._aum = 100_000_000_000.0  #! 변수 초기화
-
-        '''
-        if df_to_upload_bool:
-            total_return = total_return.groupby(total_return.index).first()
-            base_point = 1000
-            daily_aum = total_return.sum(axis=1)
-            daily_aum.index = pd.to_datetime(daily_aum.index)
-            try:
-                daily_idx = daily_aum / daily_aum[datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), "%Y-%m-%d")] *base_point
-            except:
-                print(f'error check [{rebalancing_dates[0]}] - date index not exists, call the most recent previous date')
-                daily_idx = daily_aum / daily_aum[:datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), "%Y-%m-%d")].iloc[-1] *base_point
-            daily_idx = daily_idx[datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), "%Y-%m-%d"):]
-
-
-            kospi = cls.deepsearch.compute(f"코스피 지수 {datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d')}-{datetime.strftime(datetime.today().date(), '%Y-%m-%d')}").reset_index().set_index('date')
-            # from pandas_datareader import data 
-            # df_krx = fdr.StockListing('KRX')
-            # resp = fdr.DataReader("069500", start=datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d'), end=datetime.strftime(datetime.today().date(), '%Y-%m-%d'))
-            # resp = data.DataReader("KOSPI", "naver", start=datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d'), end=datetime.strftime(datetime.today().date(), '%Y-%m-%d'))[["Open", "High", "Low", "Close", "Volume"]]
-            # resp = resp.astype(float)
-
-            # resp["symbol"] = "KRX:KOSPI"
-            # resp["entity_name"] = "코스피"
-            # resp = resp.reset_index()[["Date", "symbol", "entity_name", "Close"]].sort_values(by=["Date"])
-            # resp.columns = ["date", "symbol", "entity_name", f"주가 {datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d')}-{datetime.strftime(datetime.today().date(), '%Y-%m-%d')}"]
-            # resp = resp.set_index(["date", "symbol"])
-            # kospi = resp.reset_index().set_index('date')
-
-            kospi.columns = ['symbol', 'entity_name', 'close']
-            kospi.index = pd.to_datetime(kospi.index).date
-
-
-            # if fdr == False:
-            #     kospi = cls.deepsearch.compute(f"코스피 지수 {datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d')}-{datetime.strftime(datetime.today().date(), '%Y-%m-%d')}").reset_index().set_index('date')
-            # kospi.columns = ['symbol', 'entity_name', 'close']
-            # kospi.index = pd.to_datetime(kospi.index).date
-
-            #! 한국주식과 미국주식을 섞으면 공휴일이 다르다 
-            daily_idx_date_reviewed = daily_idx.loc[kospi.index]
-            # kospi_ret = kospi['close'].loc[daily_idx.index].pct_change()  # 당일의 종가수익률이 아니라 판다스에서 추가적으로 계산된 값이므로 첫날의 수익률은 누락 #! 그런데 첫날이 월요일이면 -1day때문에 길이가 안맞는다
-            kospi_ret = kospi['close'].pct_change()
-
-            daily_kospi = (kospi_ret+1).cumprod().fillna(1) *base_point
-            # daily_kospi.index = daily_kospi.index.date
-            #업로드용 파일 가공
-            _excel_date_format = "%Y-%m-%d"
-            # df_to_upload = pd.concat([daily_idx, daily_kospi], axis=1)
-            df_to_upload = pd.concat([daily_idx_date_reviewed, daily_kospi], axis=1)
-            df_to_upload.columns = ['index', 'KOSPI']
-            df_to_upload.index = pd.to_datetime(df_to_upload.index, format="%Y-%m-%d")
-            df_to_upload.index = df_to_upload.index.strftime(_excel_date_format)
-            df_to_upload = df_to_upload.reset_index()
-            df_to_upload.columns = ['date', 'index', 'KOSPI']
-
-            
-            df_to_upload['date'] = df_to_upload['date'].astype(str)
-
-            return df_to_upload
-        return total_return
-        '''
-
-
         if df_to_upload_bool:
             total_return = total_return.groupby(total_return.index).first()
             base_point = 1000
             daily_aum = total_return.sum(axis=1)
             daily_aum.index = pd.to_datetime(daily_aum.index)
             index_calc_start_date = cls._datetime_reformer(rebalancing_dates[0])
```

## Comparing `deepsearcheath-0.9.2.dist-info/LICENSE` & `deepsearcheath-0.9.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `deepsearcheath-0.9.2.dist-info/METADATA` & `deepsearcheath-0.9.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsearcheath
-Version: 0.9.2
+Version: 0.9.3
 Summary: Heath taylored DeepSearch api.
 Home-page: https://github.com/htaehpeed/deepsearcheath
 Author: Heath
 Author-email: heath@deepsearch.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

