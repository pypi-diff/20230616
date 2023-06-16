# Comparing `tmp/fsrs4anki_optimizer-3.24.1.tar.gz` & `tmp/fsrs4anki_optimizer-3.24.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.24.1.tar", last modified: Tue Jun 13 02:50:55 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.24.2.tar", last modified: Fri Jun 16 06:20:41 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.24.1.tar` & `fsrs4anki_optimizer-3.24.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:50:55.052592 fsrs4anki_optimizer-3.24.1/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-13 02:50:55.052592 fsrs4anki_optimizer-3.24.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:50:55.048592 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43250 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:50:55.052592 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 02:50:55.000000 fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:50:55.052592 fsrs4anki_optimizer-3.24.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 02:50:41.000000 fsrs4anki_optimizer-3.24.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43171 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 06:20:41.000000 fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:20:41.575673 fsrs4anki_optimizer-3.24.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 06:20:28.000000 fsrs4anki_optimizer-3.24.2/setup.py
```

### Comparing `fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.24.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.24.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,14 @@
 
     def forward(self, inputs, state=None):
         '''
         :param inputs: shape[seq_len, batch_size, 2]
         '''
         if state is None:
             state = torch.zeros((inputs.shape[1], 2))
-        else:
-            state, = state
         outputs = []
         for X in inputs:
             state = self.step(X, state)
             outputs.append(state)
         return torch.stack(outputs), state
 
     def mean_reversion(self, init, current):
@@ -105,14 +103,16 @@
     for li, response in enumerate(response):
         tensor[li][0] = int(ivl[li])
         tensor[li][1] = int(response)
     return tensor
 
 class RevlogDataset(Dataset):
     def __init__(self, dataframe):
+        if len(dataframe) == 0:
+            raise ValueError('Training data is inadequate.')
         padded = pad_sequence(dataframe['tensor'].to_list(), batch_first=True, padding_value=0)
         self.x_train = padded.int()
         self.t_train = torch.tensor(dataframe['delta_t'].values, dtype=torch.int)
         self.y_train = torch.tensor(dataframe['y'].values, dtype=torch.float)
         self.seq_len = torch.tensor(dataframe['tensor'].map(len).values, dtype=torch.long)
 
     def __getitem__(self, idx):
@@ -336,57 +336,52 @@
         elif os.path.isfile("collection.anki2"):
             con = sqlite3.connect("collection.anki2")
         else:
             raise Exception("Collection not exist!")
         cur = con.cursor()
         res = cur.execute("SELECT * FROM revlog")
         revlog = res.fetchall()
-
+        if len(revlog) == 0:
+            raise Exception("No review log found!")
         df = pd.DataFrame(revlog)
-        df.columns = ['id', 'cid', 'usn', 'r', 'ivl',
-                    'last_lvl', 'factor', 'time', 'type']
+        df.columns = ['id', 'cid', 'usn', 'r', 'ivl', 'last_lvl', 'factor', 'time', 'type']
         df = df[(df['cid'] <= time.time() * 1000) &
                 (df['id'] <= time.time() * 1000) &
                 (df['r'] > 0)].copy()
         df['create_date'] = pd.to_datetime(df['cid'] // 1000, unit='s')
-        df['create_date'] = df['create_date'].dt.tz_localize(
-            'UTC').dt.tz_convert(timezone)
+        df['create_date'] = df['create_date'].dt.tz_localize('UTC').dt.tz_convert(timezone)
         df['review_date'] = pd.to_datetime(df['id'] // 1000, unit='s')
-        df['review_date'] = df['review_date'].dt.tz_localize(
-            'UTC').dt.tz_convert(timezone)
+        df['review_date'] = df['review_date'].dt.tz_localize('UTC').dt.tz_convert(timezone)
         df.drop(df[df['review_date'].dt.year < 2006].index, inplace=True)
         df.sort_values(by=['cid', 'id'], inplace=True, ignore_index=True)
         self.type_sequence = np.array(df['type'])
         self.time_sequence = np.array(df['time'])
         df.to_csv("revlog.csv", index=False)
         print("revlog.csv saved.")
 
         df = df[df['type'] != 3].copy()
         df['real_days'] = df['review_date'] - timedelta(hours=int(next_day_starts_at))
         df['real_days'] = pd.DatetimeIndex(df['real_days'].dt.floor('D', ambiguous='infer', nonexistent='shift_forward')).to_julian_date()
         df.drop_duplicates(['cid', 'real_days'], keep='first', inplace=True)
         df['delta_t'] = df.real_days.diff()
         df.dropna(inplace=True)
-        df['delta_t'] = df['delta_t'].astype(dtype=int)
         df['i'] = df.groupby('cid').cumcount() + 1
         df.loc[df['i'] == 1, 'delta_t'] = 0
         df = df.groupby('cid').filter(lambda group: group['type'].iloc[0] == 0)
-        df = df.groupby('cid').filter(lambda group: group['type'].iloc[0] == 0)
         df['prev_type'] = df.groupby('cid')['type'].shift(1).fillna(0).astype(int)
-        df['helper'] = (df['type'] == 0) & ((df['prev_type'] == 1) | (df['prev_type'] == 2)) & (df['i'] > 1)
-        df['helper'] = df['helper'].astype(int)
+        df['helper'] = ((df['type'] == 0) & ((df['prev_type'] == 1) | (df['prev_type'] == 2)) & (df['i'] > 1)).astype(int)
         df['helper'] = df.groupby('cid')['helper'].cumsum()
         df = df[df['helper'] == 0]
         del df['prev_type']
         del df['helper']
 
         def cum_concat(x):
             return list(accumulate(x))
 
-        t_history = df.groupby('cid', group_keys=False)['delta_t'].apply(lambda x: cum_concat([[i] for i in x]))
+        t_history = df.groupby('cid', group_keys=False)['delta_t'].apply(lambda x: cum_concat([[int(i)] for i in x]))
         df['t_history']=[','.join(map(str, item[:-1])) for sublist in t_history for item in sublist]
         r_history = df.groupby('cid', group_keys=False)['r'].apply(lambda x: cum_concat([[i] for i in x]))
         df['r_history']=[','.join(map(str, item[:-1])) for sublist in r_history for item in sublist]
         df = df[df['id'] >= time.mktime(datetime.strptime(revlog_start_date, "%Y-%m-%d").timetuple()) * 1000]
         df['y'] = df['r'].map(lambda x: {1: 0, 2: 1, 3: 1, 4: 1}[x])
         df.to_csv('revlog_history.tsv', sep="\t", index=False)
         print("Trainset saved.")
```

