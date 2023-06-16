# Comparing `tmp/breeze_strategies-4.0.tar.gz` & `tmp/breeze_strategies-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breeze_strategies-4.0.tar", last modified: Thu Jun 15 09:19:01 2023, max compression
+gzip compressed data, was "breeze_strategies-5.0.tar", last modified: Fri Jun 16 04:33:26 2023, max compression
```

## Comparing `breeze_strategies-4.0.tar` & `breeze_strategies-5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 09:19:01.261194 breeze_strategies-4.0/
--rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-4.0/LICENSE
--rw-rw-rw-   0        0        0     1544 2023-06-15 09:19:01.258161 breeze_strategies-4.0/PKG-INFO
--rw-rw-rw-   0        0        0      995 2023-06-15 09:18:49.000000 breeze_strategies-4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 09:19:01.221019 breeze_strategies-4.0/breeze_strategies/
--rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-4.0/breeze_strategies/__init__.py
--rw-rw-rw-   0        0        0    19225 2023-06-15 09:18:21.000000 breeze_strategies-4.0/breeze_strategies/breeze_strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-15 09:19:01.254194 breeze_strategies-4.0/breeze_strategies.egg-info/
--rw-rw-rw-   0        0        0     1544 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-15 09:19:01.000000 breeze_strategies-4.0/breeze_strategies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 09:19:01.261194 breeze_strategies-4.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-06-15 09:18:57.000000 breeze_strategies-4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:33:26.810087 breeze_strategies-5.0/
+-rw-rw-rw-   0        0        0     1113 2023-06-15 05:40:22.000000 breeze_strategies-5.0/LICENSE
+-rw-rw-rw-   0        0        0     1470 2023-06-16 04:33:26.809075 breeze_strategies-5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2023-06-16 04:33:18.000000 breeze_strategies-5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 04:33:26.730691 breeze_strategies-5.0/breeze_strategies/
+-rw-rw-rw-   0        0        0       58 2023-06-15 05:52:47.000000 breeze_strategies-5.0/breeze_strategies/__init__.py
+-rw-rw-rw-   0        0        0    15612 2023-06-16 04:33:00.000000 breeze_strategies-5.0/breeze_strategies/breeze_strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-16 04:33:26.806516 breeze_strategies-5.0/breeze_strategies.egg-info/
+-rw-rw-rw-   0        0        0     1470 2023-06-16 04:33:26.000000 breeze_strategies-5.0/breeze_strategies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-16 04:33:26.000000 breeze_strategies-5.0/breeze_strategies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 04:33:26.000000 breeze_strategies-5.0/breeze_strategies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-16 04:33:26.000000 breeze_strategies-5.0/breeze_strategies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-16 04:33:26.000000 breeze_strategies-5.0/breeze_strategies.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 04:33:26.811088 breeze_strategies-5.0/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-06-16 04:33:09.000000 breeze_strategies-5.0/setup.py
```

### Comparing `breeze_strategies-4.0/LICENSE` & `breeze_strategies-5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `breeze_strategies-4.0/PKG-INFO` & `breeze_strategies-5.0/breeze_strategies.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: breeze_strategies
-Version: 4.0
+Name: breeze-strategies
+Version: 5.0
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,32 +17,31 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==4.0
+pip install breeze_strategies==5.0
 
 ```
 
 
 ## code usage
 
 ```python
 
 from breeze_strategies import Strategies
 
-async def main():
-    obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
-    await obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
-    obj.stop()
-    obj.get_pnl()
-    obj.squareoff(rightval = "enter right value ",exchange_code = "exchange_code", stock_code = "stock_code", product_type = "product_type", expiry_date = "expiry_date", strike_price = "strike_price", action = "buy", order_type = "market" , validity = "validity", stoploss, quantity = "quantity" , price = "executed price",validity_date = "validity_date", trade_password = "", disclosed_quantity = "0")
+
+obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
+obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+obj.stop()
+obj.get_pnl()
+obj.squareoff(exchange_code = "exchange_code", stock_code = "stock_code", product_type = "product_type", expiry_date = "expiry_date", strike_price = "strike_price", action = "buy", order_type = "market" , validity = "validity", stoploss, quantity = "quantity" , price = "executed price",validity_date = "validity_date", trade_password = "", disclosed_quantity = "0",right = "Call")
 
 
-await main()
 
 ```
```

### Comparing `breeze_strategies-4.0/breeze_strategies/breeze_strategies.py` & `breeze_strategies-5.0/breeze_strategies/breeze_strategies.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,52 +4,49 @@
 #import datetime
 import sys
 import asyncio
 import nest_asyncio
 from breeze_connect import BreezeConnect
 from datetime import datetime
 
-nest_asyncio.apply()
+#nest_asyncio.apply()
 
 class Strategies:
     
     #initialize strategy object
     def __init__(self,app_key,secret_key,api_session,max_profit,max_loss):
         
-        
         self.maxloss = int(max_loss)
         self.maxprofit = int(max_profit)
-        self.calllock = threading.Lock()
-        self.putlock = threading.Lock()
         self.currentcall = 0
         self.currentput = 0
         self.flag = False
         self.client = BreezeConnect(app_key)
         self.client.generate_session(secret_key,api_session)
         self.client.ws_connect()
         self.quantity = 0
     
-    def squareoff(self,rightval,exchange_code, stock_code, product_type, expiry_date, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity,right = None):
+    def squareoff(self,exchange_code, stock_code, product_type, expiry_date, strike_price, action, order_type, validity, stoploss, quantity, price,validity_date, trade_password, disclosed_quantity,right):
         data = self.client.square_off(exchange_code=exchange_code,
                             product="options",
                             stock_code=stock_code,
                             expiry_date=expiry_date,
-                            right=rightval,
+                            right=right,
                             strike_price=strike_price,
                             action=action,
                             order_type=order_type,
                             validity=validity,
                             stoploss="0",
                             quantity=quantity,
                             price=price,
                             validity_date=validity_date,
                             trade_password="",
                             disclosed_quantity="0")
         
-        print(f"square off status of {rightval} is",data)
+        print(f"square off status of {right} is",data)
         
     def get_date_format(self,expiry_date):
         month_names = {
                             '01': 'Jan',
                             '02': 'Feb',
                             '03': 'Mar',
                             '04': 'Apr',
@@ -64,108 +61,73 @@
                       }
         year = expiry_date[:4]
         month = expiry_date[5:7]
         day = expiry_date[8:10]
         formatted_date = f"{day}-{month_names[month]}-{year}"
         return(formatted_date)
         
-    def trigger(self,product_type, rightval, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, executed_price,flag):
-        #print(f"current call is {self.currentcall} Rs and current put is {self.currentput} Rs")
+    def trigger(self,product_type, rightval, stock_code, strike_price, quantity, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution,put_execution):
         net_gain_loss = (self.currentcall + self.currentput)*int(quantity)
-        print(f"net gain/loss received : {net_gain_loss} Rs \n call gain per quantity :{self.currentcall} Rs \n put gain per quantity: {self.currentput} Rs")
-        
+        print(f"net gain/loss received : {net_gain_loss}/- Rs")
         formatted_date = self.get_date_format(expiry_date)
-        
+
         if(net_gain_loss > 0 and net_gain_loss >= self.maxprofit):
             print("maxprofit has reached...")
             print("SquareOff operation on both contracts call and put begins....")
             
-            self.squareoff(rightval,exchange_code, stock_code, product_type, expiry_date, "Call", strike_price, "buy", order_type, validity, stoploss, quantity, call_price, validity_date, "", disclosed_quantity="0")
-            self.squareoff(rightval,exchange_code, stock_code, product_type, expiry_date, "Put", strike_price, "buy", order_type, validity, stoploss, quantity, put_price, validity_date, "", disclosed_quantity="0")
+            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, "buy", order_type, validity, stoploss, quantity, call_price, validity_date, "", disclosed_quantity="0","Call")
+            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, "buy", order_type, validity, stoploss, quantity, put_price, validity_date, "", disclosed_quantity="0","Put")
             
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
             print("-------------END--------------")
             self.flag = True
+            return
         if(net_gain_loss < 0 and net_gain_loss <= self.maxloss):
             print("maxloss has reached...")
             print("SquareOff operation on both contracts call and put begins....")
-            self.squareoff(rightval,exchange_code, stock_code, product_type, expiry_date, "Call", strike_price, "buy", order_type, validity, stoploss, quantity, call_price, validity_date, "", disclosed_quantity="0")
-            self.squareoff(rightval,exchange_code, stock_code, product_type, expiry_date, "Put", strike_price, "buy", order_type, validity, stoploss, quantity, put_price, validity_date, "", disclosed_quantity="0")
+            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, "buy", order_type, validity, stoploss, quantity, call_price, validity_date, "", disclosed_quantity="0","Call")
+            self.squareoff(exchange_code, stock_code, product_type, expiry_date, strike_price, "buy", order_type, validity, stoploss, quantity, put_price, validity_date, "", disclosed_quantity="0","Put")
+
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Call", get_exchange_quotes=True, get_market_depth=False)
             self.client.unsubscribe_feeds(exchange_code=exchange_code, stock_code=stock_code, product_type="options", expiry_date= formatted_date, strike_price=strike_price, right="Put", get_exchange_quotes=True, get_market_depth=False)
             print("---------------END-----------------")
             self.flag = True
-            
-    async def calculate_current_call(self,product_type,rightval,stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag):
-        print(f"inside current call() method:{rightval}")
-        resultcall = []
-        formatted_date = self.get_date_format(expiry_date)
+            return
+
+    def calculate_current(self,product_type,stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution,flag):
         
-        def on_ticks2(data):
-            resultcall.append(data)
-            with self.calllock:
-                #while(result!=[]):
-                value = resultcall.pop(0)
-                print(f"{rightval} : current market value of call order is {value['last']}/- Rs and executed price : {executed_price}/- Rs")
-                self.currentcall = round(float(value['last']) - float(executed_price),2)
-                #print(f"current market value of call order is {value} Rs, The difference between current put price and executed price is {self.currentcall}")
-                if(self.flag == False):
-                    self.trigger(product_type, rightval, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag)
-                time.sleep(2)
-                
-        self.client.on_ticks2 = on_ticks2
-        self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = rightval, get_exchange_quotes=True, get_market_depth=False)
-         
-    async def calculate_current_put(self,product_type,rightval,stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag):
-        print(f"inside current put method():{rightval}")
-        result = []
+        resultcall = []
         formatted_date = self.get_date_format(expiry_date)
         
         def on_ticks(data):
-            result.append(data)
-            with self.putlock:
-                
-                value = result.pop(0)
-                print(f"Put : current market value of put order is {value['last']} Rs and executed price : {executed_price}")
-                self.currentput = round(float(value['last']) - float(executed_price),2)
-                #print(f"current market value of put order is {value} Rs , The difference between current put price and executed price is {self.currentput}")
+            
+            value = data
+            
+            if(value['right'] == "Call"):
+                self.currentcall = round(float(value['last']) - float(call_execution), 2)
+                print(f"current Call gain  : {self.currentcall}/- Rs")
                 if(self.flag == False):
-                    self.trigger(product_type, rightval, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,executed_price,flag)
-                time.sleep(2)
-        
+                    self.trigger(product_type, "Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
+            
+            if(value['right'] == "Put"):
+                self.currentput = round(float(value['last']) - float(put_execution), 2)
+                print(f"current Put gain :  {self.currentput}/- Rs")
+                if(self.flag == False):
+                    self.trigger(product_type, "Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,put_execution)
+            
         self.client.on_ticks = on_ticks
-        self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = rightval, get_exchange_quotes=True, get_market_depth=False)
-        
-    def profit_and_loss2(self,product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution):
-        #self.calculate_current_call(product_type,"Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,flag = False)
-        #self.calculate_current_put(product_type,"Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,put_execution,flag = False)
-        p1  =  mp.Process(target = self.calculate_current_call, args = (product_type,"Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution, False))
-        p2  =  mp.Process(target = self.calculate_current_put, args = (product_type,"Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, put_execution, False))
-        
-        p1.start()
-        p2.start()
-        
-        p1.join()
-        p2.join()
-        
-    async def profit_and_loss(self,product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution):
-        #self.calculate_current_call(product_type,"Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,call_execution,flag = False)
-        #self.calculate_current_put(product_type,"Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price,put_price,put_execution,flag = False)
-        p1  =  asyncio.create_task(self.calculate_current_call(product_type,"Call", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution, False))
-        p2  =  asyncio.create_task(self.calculate_current_put(product_type,"Put", stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, put_execution, False))
-        
-        #task1 = asyncio.create_task(perform_operation1())
-        #task2 = asyncio.create_task(perform_operation2())
+        self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Call", get_exchange_quotes=True, get_market_depth=False)
+        self.client.subscribe_feeds(exchange_code = exchange_code, stock_code = stock_code, product_type = product_type, expiry_date= formatted_date, strike_price=strike_price, right = "Put", get_exchange_quotes=True, get_market_depth=False) 
 
-        # Wait for all tasks to complete
-        await asyncio.gather(p1, p2)
         
-        
-    async def long_straddle(self, stock_code, strike_price, qty, expiry_date, stoploss = "", put_price = "0", call_price = "0",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO"):
+    def profit_and_loss(self,product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution):
+        self.calculate_current(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, call_execution, put_execution,False)
+            
+    def long_straddle(self, stock_code, strike_price, qty, expiry_date, stoploss = "", put_price = "0", call_price = "0",product_type = "options", order_type = "market", validity = "day", validity_date = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%S.%fZ'), exchange_code = "NFO"):
         self.quantity = qty
         def place_order_method(stock_code,exchange_code,product,action,order_type,stoploss,quantity,price,validity,validity_date,expiry_date,right,strike_price,res_queue):
          
             data =  self.client.place_order(stock_code=stock_code,
                     exchange_code=exchange_code,
                     product="options",
                     action = "buy",
@@ -301,18 +263,18 @@
                     #call cancel order api
                     print("put order could not execute due to some reason so cancelling order")
                     status = self.client.cancel_order(exchange_code=exchange_code,
                     order_id = orderids[1])
                     
             else:
                 print("Call order got executed at price :{0} Rs and Put Order got executed at price : {1} Rs".format(call_execution,put_execution))
-                await self.profit_and_loss(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
+                self.profit_and_loss(product_type, stock_code, strike_price, qty, expiry_date, order_type, validity, validity_date, exchange_code, stoploss, call_price, put_price, orderids,call_execution,put_execution)
             
     def stop(self):
         self.client.ws_disconnect()
 
     def get_pnl(self):
         print("- Negative indicates loss")
-        print(f"current call gain/loss per qty {self.currentcall} Rs")
-        print(f"current put gain/loss per qty {self.currentput} Rs")
+        print(f"current call gain/loss per qty {self.currentcall}/- Rs")
+        print(f"current put gain/loss per qty {self.currentput}/- Rs")
         outcome = (self.currentcall + self.currentput)*int(self.quantity)
-        print(f"Total Profit/Loss for {self.quantity} is {outcome} Rs")
+        print(f"Total Profit/Loss for {self.quantity} is {outcome}/- Rs")
```

### Comparing `breeze_strategies-4.0/breeze_strategies.egg-info/PKG-INFO` & `breeze_strategies-5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: breeze-strategies
-Version: 4.0
+Name: breeze_strategies
+Version: 5.0
 Summary: ICICIDIRECT's breezeconnect strategies in python
 Home-page: https://github.com/Idirect-Tech/python_strategies/tree/master
 Author: ICICI Direct Breeze
 Author-email: breezeapi@icicisecurities.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,32 +17,31 @@
 # LIVE  python_strategies
 
 ## Steps to install Strategy Library for LIVE
 
 
 ```python
 
-pip install breeze_strategies==4.0
+pip install breeze_strategies==5.0
 
 ```
 
 
 ## code usage
 
 ```python
 
 from breeze_strategies import Strategies
 
-async def main():
-    obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
-    await obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
-    obj.stop()
-    obj.get_pnl()
-    obj.squareoff(rightval = "enter right value ",exchange_code = "exchange_code", stock_code = "stock_code", product_type = "product_type", expiry_date = "expiry_date", strike_price = "strike_price", action = "buy", order_type = "market" , validity = "validity", stoploss, quantity = "quantity" , price = "executed price",validity_date = "validity_date", trade_password = "", disclosed_quantity = "0")
+
+obj = Strategies(app_key = "your app key",secret_key = "your secret key",api_session = "your api session",max_profit = "your max profit",max_loss = "your max loss")
+obj.long_straddle(stock_code = "NIFTY",strike_price = "18700",qty = "50",expiry_date = "2023-06-15T06:00:00.000Z")
+obj.stop()
+obj.get_pnl()
+obj.squareoff(exchange_code = "exchange_code", stock_code = "stock_code", product_type = "product_type", expiry_date = "expiry_date", strike_price = "strike_price", action = "buy", order_type = "market" , validity = "validity", stoploss, quantity = "quantity" , price = "executed price",validity_date = "validity_date", trade_password = "", disclosed_quantity = "0",right = "Call")
 
 
-await main()
 
 ```
```

### Comparing `breeze_strategies-4.0/setup.py` & `breeze_strategies-5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="breeze_strategies",
-    version="4.0",
+    version="5.0",
     author="ICICI Direct Breeze",
     author_email="breezeapi@icicisecurities.com",
     description="ICICIDIRECT's breezeconnect strategies in python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=['breeze_connect==1.0.37','nest_asyncio'],
     url="https://github.com/Idirect-Tech/python_strategies/tree/master",
```

