# Comparing `tmp/xython-1.2.0.tar.gz` & `tmp/xython-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xython-1.2.0.tar", last modified: Wed Jun 14 13:35:12 2023, max compression
+gzip compressed data, was "xython-1.3.0.tar", last modified: Fri Jun 16 11:47:26 2023, max compression
```

## Comparing `xython-1.2.0.tar` & `xython-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:35:12.245499 xython-1.2.0/
--rw-rw-rw-   0        0        0      388 2023-06-05 14:30:55.000000 xython-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9251 2023-06-14 13:35:12.245499 xython-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     8722 2023-06-05 14:30:55.000000 xython-1.2.0/README.md
--rw-rw-rw-   0        0        0        0 2021-06-11 06:00:16.000000 xython-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-06-14 13:35:12.247299 xython-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-06-14 13:33:39.000000 xython-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:35:12.177517 xython-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 13:35:12.223301 xython-1.2.0/src/xython/
--rw-rw-rw-   0        0        0      467 2023-06-14 13:32:51.000000 xython-1.2.0/src/xython/__init__.py
--rw-rw-rw-   0        0        0    23159 2023-05-14 09:19:38.000000 xython-1.2.0/src/xython/anydb.py
--rw-rw-rw-   0        0        0    80419 2023-06-03 06:07:50.000000 xython-1.2.0/src/xython/basic_data.py
--rw-rw-rw-   0        0        0    24552 2023-05-23 21:32:30.000000 xython-1.2.0/src/xython/ganada.py
--rw-rw-rw-   0        0        0    19604 2023-05-22 13:41:17.000000 xython-1.2.0/src/xython/jfinder.py
--rw-rw-rw-   0        0        0    24532 2023-05-23 21:32:30.000000 xython-1.2.0/src/xython/mailmail.py
--rw-rw-rw-   0        0        0   141238 2023-06-04 07:04:32.000000 xython-1.2.0/src/xython/pcell.py
--rw-rw-rw-   0        0        0     5736 2023-04-08 04:25:55.000000 xython-1.2.0/src/xython/pcell_event.py
--rw-rw-rw-   0        0        0    11415 2023-05-22 13:34:23.000000 xython-1.2.0/src/xython/pyclick.py
--rw-rw-rw-   0        0        0    36331 2023-05-23 20:51:47.000000 xython-1.2.0/src/xython/pynal.py
--rw-rw-rw-   0        0        0    34869 2023-05-29 02:11:51.000000 xython-1.2.0/src/xython/scolor.py
--rw-rw-rw-   0        0        0    52683 2023-06-04 07:06:03.000000 xython-1.2.0/src/xython/youtil.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:35:12.243302 xython-1.2.0/src/xython.egg-info/
--rw-rw-rw-   0        0        0     9251 2023-06-14 13:35:11.000000 xython-1.2.0/src/xython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-06-14 13:35:12.000000 xython-1.2.0/src/xython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:35:12.000000 xython-1.2.0/src/xython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 14:32:10.000000 xython-1.2.0/src/xython.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-14 13:35:12.000000 xython-1.2.0/src/xython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 11:47:25.999299 xython-1.3.0/
+-rw-rw-rw-   0        0        0      388 2023-06-05 14:30:55.000000 xython-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9250 2023-06-16 11:47:26.000298 xython-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8722 2023-06-05 14:30:55.000000 xython-1.3.0/README.md
+-rw-rw-rw-   0        0        0        0 2021-06-11 06:00:16.000000 xython-1.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-06-16 11:47:26.002302 xython-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-16 11:44:48.000000 xython-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:47:25.926703 xython-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 11:47:25.976299 xython-1.3.0/src/xython/
+-rw-rw-rw-   0        0        0      467 2023-06-16 11:39:36.000000 xython-1.3.0/src/xython/__init__.py
+-rw-rw-rw-   0        0        0    23237 2023-06-11 00:05:23.000000 xython-1.3.0/src/xython/anydb.py
+-rw-rw-rw-   0        0        0    86340 2023-06-13 13:09:23.000000 xython-1.3.0/src/xython/basic_data.py
+-rw-rw-rw-   0        0        0    24552 2023-05-23 21:32:30.000000 xython-1.3.0/src/xython/ganada.py
+-rw-rw-rw-   0        0        0    32173 2023-04-30 08:12:33.000000 xython-1.3.0/src/xython/gfinder.py
+-rw-rw-rw-   0        0        0    19604 2023-05-22 13:41:17.000000 xython-1.3.0/src/xython/jfinder.py
+-rw-rw-rw-   0        0        0    24532 2023-05-23 21:32:30.000000 xython-1.3.0/src/xython/mailmail.py
+-rw-rw-rw-   0        0        0   144097 2023-06-16 10:51:24.000000 xython-1.3.0/src/xython/pcell.py
+-rw-rw-rw-   0        0        0     5736 2023-04-08 04:25:55.000000 xython-1.3.0/src/xython/pcell_event.py
+-rw-rw-rw-   0        0        0    11415 2023-05-22 13:34:23.000000 xython-1.3.0/src/xython/pyclick.py
+-rw-rw-rw-   0        0        0    36331 2023-05-23 20:51:47.000000 xython-1.3.0/src/xython/pynal.py
+-rw-rw-rw-   0        0        0    35958 2023-06-16 10:41:29.000000 xython-1.3.0/src/xython/scolor.py
+-rw-rw-rw-   0        0        0    53568 2023-06-16 11:26:16.000000 xython-1.3.0/src/xython/youtil.py
+drwxrwxrwx   0        0        0        0 2023-06-16 11:47:25.997298 xython-1.3.0/src/xython.egg-info/
+-rw-rw-rw-   0        0        0     9250 2023-06-16 11:47:25.000000 xython-1.3.0/src/xython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-06-16 11:47:25.000000 xython-1.3.0/src/xython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 11:47:25.000000 xython-1.3.0/src/xython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-05 14:32:10.000000 xython-1.3.0/src/xython.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-16 11:47:25.000000 xython-1.3.0/src/xython.egg-info/top_level.txt
```

### Comparing `xython-1.2.0/PKG-INFO` & `xython-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: xython
-Version: 1.2.0
+Version: 1.3.0
 Summary: Easy Read / Write for Excel, Word, Color, Etc using Python
 Home-page: https://github.com/sjpark/xython
-Download-URL: https://github.com/sjpark/xython/archive/v1.2.0.tar.gz
+Download-URL: https://github.com/sjpark/xython/archive/v1.3.0.tar.gz
 Author: sjpark
 Author-email: sjpkorea@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ## xython 모듈에 대하여
 ### 개괄적인 설명
 이모듈은 업무용으로 많이 사용하는 엑셀 , 색, 정규표현식, 등에 대하여 Python과 win32com을 기본으로 사용하여 각기 새롭게 모듈을 만들어서 좀더 쉽고 편하게 사용하고 만들자는 것입니다
 자동화는 각자의 사용에 대한
```

### Comparing `xython-1.2.0/README.md` & `xython-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xython-1.2.0/setup.py` & `xython-1.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 #with open("README.md", "rt", encoding='UTF8') as fh:
 #    long_description = fh.read()
 setup(
     name='xython',
-    version='1.2.0',
+    version='1.3.0',
     url='https://github.com/sjpark/xython',
-    download_url='https://github.com/sjpark/xython/archive/v1.2.0.tar.gz',
+    download_url='https://github.com/sjpark/xython/archive/v1.3.0.tar.gz',
     author='sjpark',
     author_email='sjpkorea@yahoo.com',
     description='Easy Read / Write for Excel, Word, Color, Etc using Python',
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,
     package_data={
         "xython": ["*.*"],
         },
     long_description_content_type="text/markdown",
     long_description=open('README.md', "r", encoding='UTF8').read(),
     install_requires=[''],
-    python_requires='>=3.10',
+    python_requires='>=3.9',
     zip_safe=False,
     classifiers=['License :: OSI Approved :: MIT License'],
     )
```

### Comparing `xython-1.2.0/src/xython/anydb.py` & `xython-1.3.0/src/xython/anydb.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 		df자료를 커럼과 값을 기준으로 나누어서 결과를 리스트로 돌려주는 것이다
 		"""
 		col_list = df_obj.columns.values.tolist()
 		value_list = df_obj.values.tolist()
 		col_list.extend(value_list)
 		return col_list
 
-	def change_dic_to_sql_data(self, dic_data):
+	def change_dic_to_list_as_col_value_style(self, dic_data):
 		"""
 		사전의 자료를 sql에 입력이 가능한 형식으로 만드는 것
 		결과 : [[컬럼리스트], [자료1], [자료2]....]
 		"""
 		col_list = list(dic_data[0].keys())
 		value_list =[]
 		for one_col in col_list:
@@ -72,38 +72,33 @@
 	def change_list2d_to_df(self, col_list="", list2d=""):
 		"""
 		리스트 자료를 dataframe로 만드는것
 		입력형태 : 제목리스트, 2차원 값리스트형
 		출력형태 : dataframe로 바꾼것
 		"""
 		checked_list2d = self.yt.change_list1d_to_list2d(list2d)
-		checked_col_list = []
 		# 컬럼의 이름이 없거나하면 기본적인 이름을 만드는 것이다
-		if col_list == "" or col_list == []:
-			for num in range(len(checked_list2d)):
-				checked_col_list.append("col" + str(num))
-		else:
-			checked_col_list = col_list
-		input_df = pd.DataFrame(data=checked_list2d, columns=col_list)
+		checked_col_list = self.check_input_data(col_list, list2d)
+		input_df = pd.DataFrame(data=checked_list2d, columns=checked_col_list)
 		return input_df
 
-	def change_sqlite_table_to_df(self, table_name, db_name=""):
+	def change_sqlite_to_df(self, table_name, db_name=""):
 		"""
 		sqlite의 테이블을 df로 변경
 		"""
 		self.check_cursor(db_name)
 		sql = "SELECT * From {}".format(table_name)
 		sql_result = self.cursor.execute(sql)
 		cols = []
 		for column in sql_result.description:
 			cols.append(column[0])
 		input_df = pd.DataFrame.from_records(data=sql_result.fetchall(), columns=cols)
 		return input_df
 
-	def change_sqlite_table_to_list(self, table_name, db_name=""):
+	def change_sqlite_to_list(self, table_name, db_name=""):
 		"""
 		sqlite의 테이블 자료를 리스트로 변경
 		출력형태 :[2차원리스트(제목), 2차원리스트(값들)]
 		"""
 		self.check_cursor(db_name)
 		sql_result = self.cursor.execute("SELECT * From {}".format(table_name))
 		cols = []
@@ -127,21 +122,21 @@
 		"""
 		컬럼의 이름으로 쓰이는 것에 이상한 글자들이 들어가지 않도록 확인하는 것이다
 		"""
 		for data1, data2 in [["'", ""], ["/", ""], ["\\", ""], [".", ""],[" ", "_"] ]:
 			col_name = col_name.replace(data1, data2)
 		return col_name
 
-	def check_col_name_all_in_sqlite_table(self, table_name, db_name =""):
+	def check_col_name_all_in_sqlite(self, table_name, db_name =""):
 		"""
 		현재 있는 테이블의 이름에 특수문자들을 지우는 것이다
 		공백을 _로 변경하는것, Column의 이름을 변경한다
 		"""
 		self.check_cursor(db_name)
-		all_col_names = self.read_col_name_all_in_sqlite_table(db_name, table_name)
+		all_col_names = self.read_col_name_all_in_sqlite(db_name, table_name)
 		for col_name in all_col_names:
 			col_name_new = self.check_col_name(col_name)
 			if not col_name_new == col_name:
 				self.cursor.execute("alter table {} RENAME COLUMN {} to {}".format(table_name, col_name, col_name_new))
 
 	def check_cursor(self, db_name=""):
 		if db_name =="":
@@ -158,14 +153,24 @@
 		db_name_all = self.yt.read_all_filename_in_folder(path)
 		if db_name in db_name_all:
 			result = db_name
 		else:
 			result = ""
 		return result
 
+	def check_input_data(self, col_list, data_list):
+		result = []
+		# 컬럼의 이름이 없거나하면 기본적인 이름을 만드는 것이다
+		if col_list == "" or col_list == []:
+			for num in range(len(data_list)):
+				result.append("col" + str(num))
+		else:
+			result = col_list
+		return result
+
 	def check_df_range(self, input_df):
 		"""
 		개인적으로 만든 이용형태를 것으로,
 		check로 시작하는 메소드는 자료형태의 변경이나 맞는지를 확인하는 것이다
 		dataframe의 영역을 나타내는 방법을 dataframe에 맞도록 변경하는 것이다
 		x=["1:2", "1~2"] ===> 1, 2열
 		x=["1,2,3,4"] ===> 1,2,3,4열
@@ -185,15 +190,15 @@
 				temp_1 = []
 				for item in changed_one:
 					temp_1.append(int(item))
 				one = temp_1
 			temp.append(one)
 		return temp
 
-	def delete_column_in_sqlite_table(self, table_name, col_name_list, db_name=""):
+	def delete_column_in_sqlite(self, table_name, col_name_list, db_name=""):
 		"""
 		컬럼 삭제
 		입력형태 : ["col_1","col_2","col_3"]
 		"""
 		self.check_cursor(db_name)
 		if col_name_list:
 			for col_name in col_name_list:
@@ -207,37 +212,37 @@
 		"""
 		nan_value = float("NaN")
 		input_df.replace(0, nan_value, inplace=True)
 		input_df.replace("", nan_value, inplace=True)
 		input_df.dropna(how="all", axis=1, inplace=True)
 		return input_df
 
-	def delete_empty_column_in_sqlite_table(self, table_name, db_name=""):
+	def delete_empty_column_in_sqlite(self, table_name, db_name=""):
 		"""
 		테이블의 컬럼중에서 아무런 값도 없는 컬럼을 삭제한다
 		"""
 		self.check_cursor(db_name)
-		col_name_all = self.read_col_name_all_in_sqlite_table(db_name, table_name)
+		col_name_all = self.read_col_name_all_in_sqlite(db_name, table_name)
 
 		for col_name in col_name_all:
 			sql = ("select COUNT(*) from %s where %s is not null" % (table_name, col_name))
 			self.cursor.execute(sql)
 			if self.cursor.fetchall()[0][0] == 0:
 				#입력값이 없으면 0개이고, 그러면 삭제를 하는 것이다
 				sql = ("ALTER TABLE %s DROP COLUMN %s " % (table_name, col_name))
 				self.cursor.execute(sql)
 
-	def delete_sqlite_table(self, table_name, db_name=""):
+	def delete_sqlite(self, table_name, db_name=""):
 		"""
 		입력형태 : 테이블이름
 		"""
 		self.check_cursor(db_name)
 		self.cursor.execute("DROP TABLE " + table_name)
 
-	def insert_cols_in_sqlite_table(self, table_name, col_data_list_s, db_name=""):
+	def insert_cols_in_sqlite(self, table_name, col_data_list_s, db_name=""):
 		"""
 		새로운 컬럼을 만든다
 		col_data_list_s : [["이름1","int"],["이름2","text"]]
 		["이름2",""] => ["이름2","text"]
 		"""
 		self.check_cursor(db_name)
 		for one_list in col_data_list_s:
@@ -293,15 +298,15 @@
 	def make_new_sqlite_db(self, db_name=""):
 		"""
 		새로운 데이터베이스를 만든다
 		입력형태 : 이름
 		"""
 		self.make_connection_with_sqlite_db(db_name)
 
-	def make_new_sqlite_table_with_column(self, table_name, column_data_list, db_name=""):
+	def make_new_sqlite_with_column(self, table_name, column_data_list, db_name=""):
 		"""
 		어떤 형태의 자료가 입력이 되어도 테이블을 만드는 sql을 만드는 것이다
 		입력형태 1 : 테이블이름, [['번호1',"text"], ['번호2',"text"],['번호3',"text"],['번호4',"text"]]
 		입력형태 2 : 테이블이름, ['번호1','번호2','번호3','번호4']
 		입력형태 3 : 테이블이름, [['번호1',"text"], '번호2','번호3','번호4']
 		"""
 		self.check_cursor(db_name)
@@ -367,41 +372,41 @@
 		df.iloc[where_i, whe	re_j] Select both rows and columns by integer position
 		df.at[label_i, label	_j] Select a single scalar value by row and column label
 		df.iat[i, j]	Select a single scalar value by row and column position (integers)
 		get_value(), set_val	ue() Select single value by row and column label
 		"""
 		return result
 
-	def read_col_name_all_in_sqlite_table(self, table_name, db_name=""):
+	def read_col_name_all_in_sqlite(self, table_name, db_name=""):
 		"""
 		해당하는 테이의 컬럼구조를 갖고온다
 		입력형태 : 테이블이름
 		출력형태 : 컬럼이름들
 		"""
 		self.check_cursor(db_name)
 		self.cursor.execute("PRAGMA table_info('%s')" % table_name)
 		sql_result =self.cursor.fetchall()
 		result = []
 		for one_list in sql_result:
 			result.append(one_list[1])
 		return result
 
-	def read_col_property_all_in_sqlite_table(self, table_name, db_name=""):
+	def read_col_property_all_in_sqlite(self, table_name, db_name=""):
 		"""
 		해당하는 테이블의 컬럼의 모든 구조를 갖고온다
 		"""
 
 		self.check_cursor(db_name)
 		self.cursor.execute("PRAGMA table_info('%s')" % table_name)
 		result = []
 		for temp_2 in self.cursor.fetchall():
 			result.append(temp_2)
 		return result
 
-	def read_columns_data_from_no1_to_no2_in_sqlite_table(self, table_name, offset=0, row_count=100, db_name=""):
+	def read_columns_data_from_no1_to_no2_in_sqlite(self, table_name, offset=0, row_count=100, db_name=""):
 		"""
 		테이블의 자료중 원하는 갯수만 읽어오는 것
 		"""
 		self.check_cursor(db_name)
 		self.cursor.execute(("select * from %s LIMIT %s, %s;") % (table_name, str(offset), str(row_count)))
 		result = self.cursor.fetchall()
 		return result
@@ -463,14 +468,22 @@
 		"""
 		위치를 기준으로 값을 읽어오는 것이다
 		숫자를 넣으면 된다
 		"""
 		result = df_obj.iat[int(xy[0]), int(xy[1])]
 		return result
 
+	def read_pickle_file(self, path_n_name=""):
+		"""
+		pickle로 자료를 만든것을 읽어오는 것이다
+		"""
+		with open(path_n_name, "rb") as fr:
+			result = pickle.load(fr)
+		return result
+
 	def read_table_data_by_col_names_at_sqlite(self, col_name_s="", condition="all", db_name=""):
 		"""
 		문자는 컬럼이름으로, 숫자는 몇번째인것으로...
 		"""
 		self.check_cursor(db_name)
 		if col_name_s == "":
 			sql_columns = "*"
@@ -483,15 +496,15 @@
 			lim_no = condition
 		limit_text = "limit {}".format(lim_no)
 		sql = "SELECT {} FROM {} ORDER BY auto_no {}".format(sql_columns, self.table_name, limit_text)
 		self.cursor.execute(sql)
 		result = self.cursor.fetchall()
 		return result
 
-	def read_table_data_for_sqlite_table(self, table_name, db_name=""):
+	def read_table_data_for_sqlite(self, table_name, db_name=""):
 		"""
 		테이블의 모든 자료를 읽어온다
 		입력형태 : 테이블 이름
 		"""
 		self.check_cursor(db_name)
 		self.cursor.execute(("select * from {}").format(table_name))
 		result = self.cursor.fetchall()
@@ -519,14 +532,23 @@
 		"""
 		self.check_cursor(db_name)
 		self.cursor.execute(sql)
 		result = self.cursor.fetchall()
 		self.con.commit()
 		return result
 
+	def save_input_data_to_pickle_file(self, source_data = "", file_name = "", path = "D:\\"):
+		"""
+		자료를 pickle 로 저장하는것
+		"""
+		if not "." in file_name:
+			file_name = file_name +".pickle"
+		with open(path+file_name, "wb") as fr:
+			pickle.dump(source_data, fr)
+
 	def save_sqlite_memorydb_to_diskdb(self, db_name=""):
 		"""
 		memory에 저장된것을 화일로 저장하는것
 		python 3.7부터는 backup이 가능
 		"""
 		db_disk = sqlite3.connect(db_name)
 		self.con.backup(db_disk)
@@ -556,15 +578,15 @@
 		result = """
 		df : dataframe
 		con : Connection, 외부환경과 Database를 연결하는 것. 즉 db가 위치한 곳들을 연결하는 것이지요
 		cursor : DB에 어떤 일을 시키면, Db에서 Item이라는 객체가 만들어진다. 그 만들어진곳을 가리키는 객체
 		"""
 		return result
 
-	def write_data_in_sqlite_table(self, table_name, col_name_s, col_value_s, db_name=""):
+	def write_data_to_sqlite(self, table_name, col_name_s, col_value_s, db_name=""):
 		"""
 		"""
 		self.check_cursor(db_name)
 		sql_columns = ""
 		sql_values = ""
 		for column_data in col_name_s:
 			sql_columns = sql_columns + column_data + ", "
@@ -582,80 +604,63 @@
 		"""
 		col_list = input_df.columns.values.tolist()
 		value_list = input_df.values.tolist()
 		excel = pcell.pcell()
 		excel.write_list1d_in_yline("", xy, col_list)
 		excel.write_value_in_range_as_speedy("", [xy[0] + 1, xy[1]], value_list)
 
-	def write_df_to_sqlite_table(self, table_name, df_data, db_name=""):
+	def write_df_to_sqlite(self, table_name, df_data, db_name=""):
 		"""
 		df자료를 sqlite에 새로운 테이블로 만들어서 넣는 것
 		"""
 		self.check_cursor(db_name)
 		df_data.to_sql(table_name, self.con)
 
-	def write_dic_in_sqlite_table(self, table_name, dic_data, db_name=""):
+	def write_dic_to_sqlite(self, table_name, dic_data, db_name=""):
 		"""
 		사전의 키를 y이름으로 해서 값을 입력한다
 		"""
 		self.check_cursor(db_name)
 
 		for one_col in list(dic_data[0].keys()):
-			if not one_col in self.read_col_name_all_in_sqlite_table(table_name):
-				self.insert_cols_in_sqlite_table(table_name, [one_col])
+			if not one_col in self.read_col_name_all_in_sqlite(table_name):
+				self.insert_cols_in_sqlite(table_name, [one_col])
 
 		sql = self.make_insert_sql_by_col_names(table_name, list(dic_data[0].keys()))
 		value_list = []
 		for one_dic in dic_data:
 			value_list.append(list(one_dic.values()))
 		self.cursor.executemany(sql, value_list)
 
-	def write_list_to_sqlite_table(self, table_name, col_name_s, list_values, db_name=""):
+	def write_list_to_sqlite(self, table_name, col_name_s, list_values, db_name=""):
 		"""
 		리스트의 형태로 넘어오는것중에 y이름과 값을 분리해서 얻는 것이다
 		"""
 		self.check_cursor(db_name)
 		sql = self.make_insert_sql_by_col_names(table_name, col_name_s)
 		self.cursor.executemany(sql, list_values)
 
-	def write_sqlite_table_data_all_to_df(self, table_name, db_name=""):
+	def write_sqlite_data_all_to_df(self, table_name, db_name=""):
 		"""
 		sqlite를 df로 만드는것
 		"""
 		self.check_cursor(db_name)
 		sql = "SELECT * From %s" % (table_name)
 		query = self.cursor.execute(sql)
 		cols = [column[0] for column in query.description]
 		input_df = pd.DataFrame.from_records(data=query.fetchall(), columns=cols)
 		return input_df
 
-	def write_value_in_df_by_xy(self, df, xy, value):
+	def write_value_to_df_by_xy(self, df, xy, value):
 		"""
 		dataframe에 좌표로 값을 저장
 		"""
 		x_max = df.index.size
 		y_max = df.columns.size
 		if xy[1] > y_max:
 			for no in range(y_max, xy[1]):
 				df[len(df.columns)] = np.NaN
 		if xy[0] > x_max:
 			data_set = [(lambda x: np.NaN)(a) for a in range(len(df.columns))]
 			for no in range(xy[0] - x_max):
 				df.loc[len(df.index)] = data_set
-		df.iat[int(xy[0]), int(xy[1])] = value
-
-	def read_pickle_file(self, path_n_name=""):
-		"""
-		pickle로 자료를 만든것을 읽어오는 것이다
-		"""
-		with open(path_n_name, "rb") as fr:
-			result = pickle.load(fr)
-		return result
-
-	def save_input_data_to_pickle_file(self, source_data = "", file_name = "", path = "D:\\"):
-		"""
-		자료를 pickle 로 저장하는것
-		"""
-		if not "." in file_name:
-			file_name = file_name +".pickle"
-		with open(path+file_name, "wb") as fr:
-			pickle.dump(source_data, fr)
+		df.iat[int(xy[0]), int(xy[1])] = value
```

### Comparing `xython-1.2.0/src/xython/basic_data.py` & `xython-1.3.0/src/xython/basic_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -817,14 +817,244 @@
 		              "지역 전화번호 찾기": [4, "0(2|31|32|33|41|42|43|44|51|52|53|54|55|61|62|63|64)\-{0,1}\d{3,4}\-{0,1}\d{4}",
 		                             "type_z0"],
 		              "주민등록번호": [4, "[0-9]{2}0[1-9]|1[0-2]0[1-9]|[1,2][0-9]|3[0,1]-[1-4][0-9]{6}", "type_z0"],
 		              "금액": [4, "[숫자,][1~][원:0~1]", "type_z0"],
 		              "중복된 단어 찾기": [4, "\\b(\\w+)\\s+\\1\\b", "type_z0"],
 		              }
 
+		self.vars["shape_enum"] ={
+			'mixed': -2,
+			'rectangle': 1,
+			'직사각형': 1,
+			'parallelogram': 2,
+			'평행사변형': 2,
+			'trapezoid': 3,
+			'사다리꼴': 3,
+			'diamond': 4,
+			'다이아몬드': 4,
+			'roundedrectangle': 5,
+			'둥근모서리사각형': 5,
+			'Octagon': 6,
+			'팔각형': 6,
+			'isoscelestriangle': 7,
+			'이등변삼각형': 7,
+			'RightTriangle': 8,
+			'직각삼각형': 8,
+			'Oval': 9,
+			'타원': 9,
+			'Hexagon': 10,
+			'육각형': 10,
+			'Cross': 11,
+			'십자형': 11,
+			'RegularPentagon': 12,
+			'오각형': 12,
+			'Can': 13,
+			'원통형': 13,
+			'Cube': 14,
+			'정육면체': 14,
+			'Bevel': 15,
+			'빗면사각형': 15,
+			'FoldedCorner': 16,
+			'모서리접힌사각형': 16,
+			'SmileyFace': 17,
+			'웃는얼굴': 17,
+			'Donut': 18,
+			'원형': 18,
+			'NoSymbol': 19,
+			'BlockArc': 20,
+			'막힌원호': 20,
+			'Heart': 21,
+			'하트': 21,
+			'LightningBolt': 22,
+			'번개': 22,
+			'Sun': 23,
+			'해': 23,
+			'Moon': 24,
+			'달': 24,
+			'Arc': 25,
+			'원호': 25,
+			'DoubleBracket': 26,
+			'양쪽대괄호': 26,
+			'DoubleBrace': 27,
+			'양쪽중괄호': 27,
+			'Plaque': 28,
+			'배지': 28,
+			'LeftBracket': 29,
+			'왼쪽대괄호': 29,
+			'RightBracket': 30,
+			'오른쪽대괄호': 30,
+			'LeftBrace': 31,
+			'왼쪽중괄호': 31,
+			'RightBrace': 32,
+			'오른쪽중괄호': 32,
+			'RightArrow': 33,
+			'오른쪽화살표': 33,
+			'LeftArrow': 34,
+			'왼쪽화살표': 34,
+			'UpArrow': 35,
+			'위쪽화살표': 35,
+			'DownArrow': 36,
+			'아래쪽화살표': 36,
+			'LeftRightArrow': 37,
+			'왼쪽오른쪽화살표': 37,
+			'UpDownArrow': 38,
+			'위쪽아래쪽화살표': 38,
+			'QuadArrow': 39,
+			'상하좌우화살표': 39,
+			'LeftRightUpArrow': 40,
+			'상좌우화살표': 40,
+			'BentArrow': 41,
+			'굽음화살표': 41,
+			'UTurnArrow': 42,
+			'U턴화살표': 42,
+			'LeftUpArrow': 43,
+			'좌상화살표': 43,
+			'BentUpArrow': 44,
+			'위로굽음화살표': 44,
+			'CurvedRightArrow': 45,
+			'CurvedLeftArrow': 46,
+			'CurvedUpArrow': 47,
+			'CurvedDownArrow': 48,
+			'StripedRightArrow': 49,
+			'NotchedRightArrow': 50,
+			'Pentagon': 51,
+			'Chevron': 52,
+			'RightArrowCallout': 53,
+			'LeftArrowCallout': 54,
+			'UpArrowCallout': 55,
+			'DownArrowCallout': 56,
+			'LeftRightArrowCallout': 57,
+			'UpDownArrowCallout': 58,
+			'QuadArrowCallout': 59,
+			'CircularArrow': 60,
+			'FlowchartProcess': 61,
+			'FlowchartAlternateProcess': 62,
+			'FlowchartDecision': 63,
+			'FlowchartData': 64,
+			'FlowchartPredefinedProcess': 65,
+			'FlowchartInternalStorage': 66,
+			'FlowchartDocument': 67,
+			'FlowchartMultidocument': 68,
+			'FlowchartTerminator': 69,
+			'FlowchartPreparation': 70,
+			'FlowchartManualInput': 71,
+			'FlowchartManualOperation': 72,
+			'FlowchartConnector': 73,
+			'FlowchartOffpageConnector': 74,
+			'FlowchartCard': 75,
+			'FlowchartPunchedTape': 76,
+			'FlowchartSummingJunction': 77,
+			'FlowchartOr': 78,
+			'FlowchartCollate': 79,
+			'FlowchartSort': 80,
+			'FlowchartExtract': 81,
+			'FlowchartMerge': 82,
+			'FlowchartStoredData': 83,
+			'FlowchartDelay': 84,
+			'FlowchartSequentialAccessStorage': 85,
+			'FlowchartMagneticDisk': 86,
+			'FlowchartDirectAccessStorage': 87,
+			'FlowchartDisplay': 88,
+			'Explosion1': 89,
+			'Explosion2': 90,
+			'4pointStar': 91,
+			'5pointStar': 92,
+			'8pointStar': 93,
+			'16pointStar': 94,
+			'24pointStar': 95,
+			'32pointStar': 96,
+			'UpRibbon': 97,
+			'DownRibbon': 98,
+			'CurvedUpRibbon': 99,
+			'CurvedDownRibbon': 100,
+			'VerticalScroll': 101,
+			'HorizontalScroll': 102,
+			'Wave': 103,
+			'DoubleWave': 104,
+			'RectangularCallout': 105,
+			'RoundedRectangularCallout': 106,
+			'OvalCallout': 107,
+			'CloudCallout': 108,
+			'LineCallout1': 109,
+			'LineCallout2': 110,
+			'LineCallout3': 111,
+			'LineCallout4': 112,
+			'LineCallout1AccentBar': 113,
+			'LineCallout2AccentBar': 114,
+			'LineCallout3AccentBar': 115,
+			'LineCallout4AccentBar': 116,
+			'LineCallout1NoBorder': 117,
+			'LineCallout2NoBorder': 118,
+			'LineCallout3NoBorder': 119,
+			'LineCallout4NoBorder': 120,
+			'LineCallout1BorderandAccentBar': 121,
+			'LineCallout2BorderandAccentBar': 122,
+			'LineCallout3BorderandAccentBar': 123,
+			'LineCallout4BorderandAccentBar': 124,
+			'ActionButtonCustom': 125,
+			'ActionButtonHome': 126,
+			'ActionButtonHelp': 127,
+			'ActionButtonInformation': 128,
+			'ActionButtonBackorPrevious': 129,
+			'ActionButtonForwardorNext': 130,
+			'ActionButtonBeginning': 131,
+			'ActionButtonEnd': 132,
+			'ActionButtonReturn': 133,
+			'ActionButtonDocument': 134,
+			'ActionButtonSound': 135,
+			'ActionButtonMovie': 136,
+			'Balloon': 137,
+			'NotPrimitive': 138,
+			'FlowchartOfflineStorage': 139,
+			'LeftRightRibbon': 140,
+			'DiagonalStripe': 141,
+			'Pie': 142,
+			'NonIsoscelesTrapezoid': 143,
+			'Decagon': 144,
+			'Heptagon': 145,
+			'Dodecagon': 146,
+			'6pointStar': 147,
+			'7pointStar': 148,
+			'10pointStar': 149,
+			'12pointStar': 150,
+			'Round1Rectangle': 151,
+			'Round2SameRectangle': 152,
+			'SnipRoundRectangle': 154,
+			'Snip1Rectangle': 155,
+			'Snip2SameRectangle': 156,
+			'Round2DiagRectangle': 157,
+			'Snip2DiagRectangle': 157,
+			'Frame': 158,
+			'HalfFrame': 159,
+			'Tear': 160,
+			'Chord': 161,
+			'Corner': 162,
+			'MathPlus': 163,
+			'MathMinus': 164,
+			'MathMultiply': 165,
+			'MathDivide': 166,
+			'MathEqual': 167,
+			'MathNotEqual': 168,
+			'CornerTabs': 169,
+			'SquareTabs': 170,
+			'PlaqueTabs': 171,
+			'Gear6': 172,
+			'Gear9': 173,
+			'Funnel': 174,
+			'PieWedge': 175,
+			'LeftCircularArrow': 176,
+			'LeftRightCircularArrow': 177,
+			'SwooshArrow': 178,
+			'Cloud': 179,
+			'ChartX': 180,
+			'ChartStar': 181,
+			'ChartPlus': 182,
+			'LineInverse': 183,}
+
+
 class basic_cell_class():
 	# 각 셀에대해서 어떤 자료들을 넣을수있을지 설정하도록 만든 것이다
 	# 다음에 추가적인것들도 가능하도록 클래스로 만든 것이다
 	def __init__(self):
 		self.values = {
 			"font_dic": {"font_color": None, "font_size": None, "background": None, "bold": None, "color": None, "colorindex": None, "creator": None, "style": None, "italic": None,
 				"name": None, "size": None, "strikethrough": None, "subscript": None, "superscript": None, "themecolor": None, "themefont": None, "tintandshade": None, "underline": None},
```

### Comparing `xython-1.2.0/src/xython/ganada.py` & `xython-1.3.0/src/xython/ganada.py`

 * *Files identical despite different names*

### Comparing `xython-1.2.0/src/xython/jfinder.py` & `xython-1.3.0/src/xython/jfinder.py`

 * *Files identical despite different names*

### Comparing `xython-1.2.0/src/xython/mailmail.py` & `xython-1.3.0/src/xython/mailmail.py`

 * *Files identical despite different names*

### Comparing `xython-1.2.0/src/xython/pcell.py` & `xython-1.3.0/src/xython/pcell.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,17 +284,17 @@
 
 	def change_rgbint_to_colorname(self, rgbint ):
 		"""
 		rgb의 정수값을 color이름으로 변경
 		"""
 		try :
 			rgblist = self.change_rgbint_to_rgb(rgbint)
-			print("rgblist", rgblist)
+			#print("rgblist", rgblist)
 			color_index = self.data_dic_colorindex_to_rgblist(rgblist)
-			print("color_index", color_index)
+			#print("color_index", color_index)
 			colorname = self.data_dic_colorname_to_colorindex(color_index)
 		except:
 			colorname = None
 		return colorname
 
 	def change_rgbint_to_rgb(self, input_int):
 		"""
@@ -363,19 +363,19 @@
 		선택영역안의 모든글자를 소문자로 만들어 주는것
 		screen update를 off로 사용
 		값 읽어오는것을 range형태로 변경
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		list_2d = self.read_value_in_range(sheet_name, xyxy)
-		print(list_2d[0:3])
+		#print(list_2d[0:3])
 		self.screen_update_off()
 		for x in range(x1, x2 + 1):
 			for y in range(y1, y2 + 1):
-				print(x, y)
+				#print(x, y)
 				try:
 					sheet_object.Cells(x, y).Value = (list_2d[x - x1][y - y1]).lower()
 				except:
 					pass
 		self.screen_update_on()
 
 	def change_value_in_range_to_capital(self, sheet_name, xyxy):
@@ -803,15 +803,15 @@
 			for one in "!@#$%^*M-":
 				check_char.extend(one)
 		zz = combinations_with_replacement(check_char, len_num)
 		for aa in zz:
 			try:
 				pswd = "".join(aa)
 				self.unlock_sheet("", pswd)
-				print("발견", pswd)
+				#print("발견", pswd)
 				break
 			except:
 				pass
 
 	def check_string_address(self, input_text="입력필요"):
 		"""
 		Input Style :	"$1:$8", "1", "a","a1", "a1b1", "2:3", "b:b"
@@ -1219,15 +1219,15 @@
 		"""
 		모든 rangename을 삭제하는 것
 		"""
 		aaa = self.xlapp.Names
 		for one in aaa:
 			ddd = str(one.Name)
 			if ddd.find("!") < 0:
-				print(one.Name)
+				#print(one.Name)
 				self.xlapp.Names(aaa).Delete()
 
 	def delete_rangename_by_name(self, sheet_name, range_name):
 		"""
 		입력한 이름을 삭제한다
 		name은 workbook으로 되지만 동일하게 하기위하여 sheet_name을 넣은 것이다
 		"""
@@ -1326,15 +1326,15 @@
 		# 찾은값을 넣을 y열을 추가한다
 		new_x = int(x2) + 1
 		self.insert_yline(sheet_name, new_x)
 		for y in range(y1, y2 + 1):
 			temp = ""
 			for x in range(x1, x2 + 1):
 				cell_value = sheet_object.Cells(x, y).Value
-				print("셀 값", cell_value, re_basic)
+				#print("셀 값", cell_value, re_basic)
 				result_list = re.findall(re_basic, str(cell_value))
 
 				if result_list == None or result_list == []:
 					pass
 				else:
 					temp = temp + str(result_list)
 					self.paint_cell_by_scolor("", [x, y], "yel++")
@@ -1342,15 +1342,15 @@
 
 	def delete_value_in_range_by_continious_samevalue(self, sheet_name="", xyxy=""):
 		"""
 		영역안에서 연속된 같은 값을 삭제 한다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
-		print(x1, y1, x2, y2)
+		#print(x1, y1, x2, y2)
 		for y in range(y1, y2 +1):
 			for x in range(x2, x1 - 1, -1):
 				up_value = sheet_object.Cells(x-1, y).Value
 				down_value = sheet_object.Cells(x, y).Value
 				if down_value == up_value:
 					sheet_object.Cells(x, y).Value = ""
 
@@ -1560,15 +1560,15 @@
 		선택영역에서 선을 긋는것
 		pixel을 기준으로 선긋기
 		선을 그을때는 위치와 넓이 높이로 긋는데, change_xyxy_to_pxyxy을 사용하면 셀위치를 그렇게 바꾸게 만든다
 		"""
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(line_xyxy)
 		pxyxy = self.change_xyxy_to_pxyxy([x1, y1, x2, y2])
-		print(pxyxy)
+		#print(pxyxy)
 		sheet_object.Shapes.AddLine(pxyxy[0], pxyxy[1], pxyxy[2], pxyxy[3]).Select()
 		self.xlapp.Selection.ShapeRange.Line.ForeColor.RGB = self.color.change_rgb_to_rgbint(rgb_list)
 		self.xlapp.Selection.ShapeRange.Line.Weight = 5
 
 	def draw_line_in_range(self, sheet_name="", xyxy="", position="", scolor="", line_style="", thickness=""):
 		"""
 		입력예 : [선의위치, 색깔, 라인스타일, 굵기] ==> [7,1,2,1], "", "",""
@@ -1582,15 +1582,15 @@
 		line_style_dic = self.data_set_basic.vars["excel_line_style_dic"]
 
 
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
-		print(scolor)
+		#print(scolor)
 		rgb_list = self.color.change_scolor_to_rgb(scolor)
 		colorint = self.color.change_rgb_to_rgbint(rgb_list)
 		aa = []
 		if type(position) == type([]):
 			for one in position:
 				aa.extend(line_position[one])
 		else:
@@ -1777,15 +1777,15 @@
 		total_len = len(all_datas)
 		same_nos = []
 		for no in range(total_len):
 			if no in same_nos:
 				pass
 			else:
 				one_list = all_datas[no]
-				print(one_list)
+				#print(one_list)
 				for num in range(no+1, total_len):
 					if num in same_nos:
 						pass
 					else:
 						if one_list == all_datas[num]:
 							same_nos.append(num)
 		return same_nos
@@ -1930,17 +1930,17 @@
 		sheet_object = self.check_sheet_name(sheet_name)
 		x1, y1, x2, y2 = self.check_address_value(xyxy)
 		my_range = sheet_object.Range(sheet_object.Cells(x1, y1), sheet_object.Cells(x2, y2))
 
 		for x in range(0, x2 - x1 + 1):
 			mok, namuji = divmod(x, int(step_no))
 			if namuji == step_no - 1:
-				print("===>", x + x1)
+				#print("===>", x + x1)
 				x_no = self.change_char_to_num(x + x1)
-				print("===>", x_no)
+				#print("===>", x_no)
 				sheet_object.Range(str(x_no) + ':' + str(x_no)).Insert(-4121)
 
 	def insert_excel_function_in_cell(self, sheet_name, xy, input_fucntion, input_xyxy):
 		result = ""
 		sheet_object = self.check_sheet_name(sheet_name)
 		range = self.change_xyxy_to_r1r1(input_xyxy)
 		x1, y1, x2, y2 = self.check_address_value(xy)
@@ -3811,15 +3811,15 @@
 		zz = combinations_with_replacement(check_char, len_num)
 		for aa in zz:
 			try:
 				pswd = "".join(aa)
 				#print(pswd)
 				self.unlock_sheet("", pswd)
 				break
-				print("발견", pswd)
+				#print("발견", pswd)
 			except:
 				pass
 
 
 	def check_same_data(self, input_list, check_line = 10):
 		"""
 		엑셀의 선택한 자료에서 여러줄을 기준으로 같은 자료만 갖고오기
@@ -3866,36 +3866,119 @@
 		x_len = len(input_list2d)
 		y_len = len(input_list2d[0])
 		for y in range(y_len):
 			temp = ""
 			for x in range(x_len):
 				self.write_value_in_cell("", [x + xy[0], y + xy[1]], "")
 				if input_list2d[x][y]:
-					print(input_list2d[x][y])
+					#print(input_list2d[x][y])
 					temp = temp + " " + input_list2d[x][y]
-			print(temp)
+			#print(temp)
 			self.write_value_in_cell("", [xy[0], y + xy[1]], str(temp).strip())
 
 	def write_serial_no_by_step(self, xyxy, start_no, step = 1):
 		"""
 		선택한 영역에 시작번호, 간격으로 이루어진 연속된 숫자를 쓰는것
 		"""
 		new_no = start_no
 		for no in range(0, xyxy[2]-xyxy[0]+1):
 			self.write_value_in_cell("", [xyxy[0]+no, xyxy[1]], new_no)
 			new_no = new_no + step
-			print([xyxy[0]+no, xyxy[1]], new_no)
+			#print([xyxy[0]+no, xyxy[1]], new_no)
 
 	def split_partial_value_in_range_by_step_from_start(self, sheet_name, xyxy, n_char):
 		"""
 		어떤 자료중에 앞에서 몇번째것들만 갖고오고 싶을때
 		예:시군구 자료에서 앞의 2글자만 분리해서 얻어오는 코드
 		"""
 		list_2d = self.read_value_in_range(sheet_name, xyxy)
 		result = set()
 		for list_1d in list_2d:
 			for one in list_1d:
 				try:
 					result.add(one[0:n_char])
 				except:
 					pass
-		return list(result)
+		return list(result)
+
+	def rotate_shape(self, sheet_name, shape_obj, degree):
+		# 도형을 회전시키는 것
+		# shape _ obi :이동시킬 도형 이름
+		sheet_object = self.check_sheet_name(sheet_name)
+		oShape = sheet_object.Shapes(shape_obj)
+		oShape.IncrementRotation(degree)
+
+	def read_all_shape_names(self, sheet_name=""):
+		sheet_object = self.check_sheet_name(sheet_name)
+		drawings_nos = sheet_object.Shapes.count
+		result = []
+		if drawings_nos > 0:
+			for num in range(sheet_object.Shapes.count, 0, -1):
+				# Range를 앞에서부터하니 삭제하자마자 번호가 다시 매겨져서, 뒤에서부터 삭제하니 잘된다
+				result.append(sheet_object.Shapes(num).Name)
+		return result
+
+	def move_shape(self, sheet_name, shape_obj, top, left):
+		# shape_0b] : 이동시림 도형 이름
+		sheet_object = self.check_sheet_name(sheet_name)
+		oShape = sheet_object.Shapes(shape_obj)
+		oShape.Top = oShape.Top + top
+		oShape.Left = oShape.left + left
+
+	def add_shape(self, sheet_name, shape_no=35, xywh=""):
+		# shape_no : 엑셀에서 정의한 도형의 번호
+		# xywh : 왼쪽윗부분의 위치에서 너비와 높이
+		sheet_object = self.check_sheet_name(sheet_name)
+
+		#도형이 숫자이면 그대로, 문자이면 기본자료에서 찾도록 한다
+		if type(shape_no) == type(123):
+			pass
+		elif shape_no in list(self.data_set_basic.vars["shape_enum"].keys()):
+			shape_no = self.data_set_basic.vars["shape_enum"][shape_no]
+
+		sheet_object.Shapes.Addshape(shape_no, xywh[0], xywh[1], xywh[2], xywh[3])
+
+	def get_xy_list_for_circle(self, r, precious=10, xy=[0, 0]):
+		# 엑셀을 기준으로, 반지름이 글자를 원으로 계속 이동시키는 것
+		# r;반지름
+		# precious : 얼마나 정밀하게 할것인지, 1도를 몇번으로 나누어서 계산할것인지
+		result = []
+		temp = []
+		for do_1 in range(1, 5):
+			for do_step in range(90 * precious + 1):
+				degree = (do_1 * do_step) / precious
+				# r을 더하는 이유는 마이너스는 않되므로 x, y측을 이동시키는것
+				x = math.cos(degree) * r
+				y = math.sin(degree) * r
+				new_xy = [int(round(x)), int(round(y))]
+
+				if not new_xy in temp:
+					temp.append(new_xy)
+		area_1 = []
+		area_2 = []
+		area_3 = []
+		area_4 = []
+
+		for x, y in temp:
+			new_x = x + r + 1 + xy[0]
+			new_y = y + r + 1 + xy[1]
+
+			if x >= 0 and y >= 0:
+				area_1.append([new_x, new_y])
+			elif x >= 0 and y < 0:
+				area_2.append([new_x, new_y])
+			elif x < 0 and y < 0:
+				area_3.append([new_x, new_y])
+			elif x < 0 and y >= 0:
+				area_4.append([new_x, new_y])
+		area_1.sort()
+		area_1.reverse()
+		area_2.sort()
+		area_3.sort()
+		area_4.sort()
+		area_4.reverse()
+
+		result.extend(area_2)
+		result.extend(area_1)
+		result.extend(area_4)
+		result.extend(area_3)
+		return result
```

### Comparing `xython-1.2.0/src/xython/pcell_event.py` & `xython-1.3.0/src/xython/pcell_event.py`

 * *Files identical despite different names*

### Comparing `xython-1.2.0/src/xython/pyclick.py` & `xython-1.3.0/src/xython/pyclick.py`

 * *Files identical despite different names*

### Comparing `xython-1.2.0/src/xython/pynal.py` & `xython-1.3.0/src/xython/pynal.py`

 * *Files identical despite different names*

### Comparing `xython-1.2.0/src/xython/scolor.py` & `xython-1.3.0/src/xython/scolor.py`

 * *Files 2% similar despite different names*

```diff
@@ -565,23 +565,34 @@
 					#print(self.basic_12hsl_set)
 					h_code = self.color_vars["color_name_eng_vs_hsl_no"][color_name][0]
 					s_code = 100
 					l_code = int(color_step)
 
 				if int(l_code) > 100 : l_code = 100
 				if int(l_code) < 0 : l_code = 0
-			print("[h_code, s_code, l_code] ==> ", h_code, s_code, l_code)
+			#print("[h_code, s_code, l_code] ==> ", h_code, s_code, l_code)
 			result = [h_code, s_code, l_code]
 		return result
 
 	def change_scolor_to_rgb (self, input_scolor):
 		hsl_list = self.change_scolor_to_hsl(input_scolor)
 		result = self.change_hsl_to_rgb(hsl_list)
 		return result
 
+	def change_scolor_to_n_color_set(self, input_scolor, step_no = 10):
+		#하나의 색을 옅은것부터 진한것까지 N개의 rgb값으로 변경하는것
+		hsl_list = self.change_scolor_to_hsl(input_scolor)
+
+		result = []
+		for l in range(0, 110, 10):
+			temp = self.change_hsl_to_rgb([hsl_list[0], 100, l])
+			result.append(temp)
+		return result
+
+
 	def check_change_mode(self, change_mode):
 
 		if type(change_mode) == type([]):
 			result = change_mode
 		elif "+" == str(change_mode)[0]:
 			#현재의 값에서 10만큼 밝아지도록 한다
 			l_value = 10 * len(change_mode)
@@ -660,15 +671,15 @@
 
 		re_com4 = re.compile("[-]+")
 		color_minus = re_com4.findall(input_scolor)
 		if color_minus != []:
 			color_no = 50 - 5 * len(color_minus[0])
 
 		result = [number_only, color_name, color_no]
-		print(result)
+		#print(result)
 		return result
 
 	def check_input_type(self, input_value):
 		hsl = self.check_input_type(input_value)
 		return hsl
 
 	def control_hsl_by_scolor_style(self, input_hsl, s_step="++", l_step="++"):
@@ -1118,8 +1129,25 @@
 
 		changed_s = s + delta_s
 		changed_l = l + delta_l
 		return [h, changed_s, changed_l]
 	def terms(self):
 		result = 	"""
 			"""
+		return result
+
+	def mix_two_scolors_with_step(self, scolor_1, scolor_2, step=10):
+		# 두가지색을 기준으로 몇단계로 색을 만들어주는 기능
+		# 예를들어, 발강 ~파랑사이의 색을 10단계로 만들어 주는 기능
+		rgb_1 = self.change_scolor_to_rgb(scolor_1)
+		rgb_2 = self.change_scolor_to_rgb(scolor_2)
+		r_step = int((rgb_2[0] - rgb_1[0]) / step)
+		g_step = int((rgb_2[1] - rgb_1[1]) / step)
+		b_step = int((rgb_2[2] - rgb_1[2]) / step)
+		result = [rgb_1, ]
+		for no in range(1, step - 1):
+			new_r = int(rgb_1[0] + r_step * no)
+			new_g = int(rgb_1[1] + g_step * no)
+			new_b = int(rgb_1[2] + b_step * no)
+			result.append([new_r, new_g, new_b])
+			result.append(rgb_2)
 		return result
```

### Comparing `xython-1.2.0/src/xython/youtil.py` & `xython-1.3.0/src/xython/youtil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1661,8 +1661,39 @@
 
 	def split_value_to_str_num(self, input_text):
 		"""
 		문자와 숫자를 분리하는 것
 		"""
 		re_com_num = re.compile("[a-zA-Z]+|\d+")
 		result = re_com_num.findall(input_text)
+		return result
+
+	def float_range(self, start, end, step):
+		# 실수형으로 가능한 range 형태
+		value = start
+		while value <= end:
+			yield value
+			value = step + value
+
+	def sample_make_name(self, input_no=5):
+		# 입력한 갯수만큼 이름의 갯수를 만들어 주는것
+		sung = "김이박최정강조윤장"
+		name = "가나다라마바사아자차카"
+		last = "진원일이삼사오구원송국한"
+		if input_no > len(sung) * len(name) * len(last) / 2:
+			result = []
+			pass
+		else:
+			total_name = set()
+			num = 0
+			while True:
+				one_sung = random.choice(sung)
+				one_name = random.choice(name)
+				one_last = random.choice(last)
+				new_name = one_sung + one_name + one_last
+				total_name.add(new_name)
+				num = num + 1
+				if len(total_name) == input_no:
+					print(input_no, num)
+					break
+			result = list(total_name)
 		return result
```

### Comparing `xython-1.2.0/src/xython.egg-info/PKG-INFO` & `xython-1.3.0/src/xython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: xython
-Version: 1.2.0
+Version: 1.3.0
 Summary: Easy Read / Write for Excel, Word, Color, Etc using Python
 Home-page: https://github.com/sjpark/xython
-Download-URL: https://github.com/sjpark/xython/archive/v1.2.0.tar.gz
+Download-URL: https://github.com/sjpark/xython/archive/v1.3.0.tar.gz
 Author: sjpark
 Author-email: sjpkorea@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ## xython 모듈에 대하여
 ### 개괄적인 설명
 이모듈은 업무용으로 많이 사용하는 엑셀 , 색, 정규표현식, 등에 대하여 Python과 win32com을 기본으로 사용하여 각기 새롭게 모듈을 만들어서 좀더 쉽고 편하게 사용하고 만들자는 것입니다
 자동화는 각자의 사용에 대한
```

