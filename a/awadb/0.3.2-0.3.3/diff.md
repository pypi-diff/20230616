# Comparing `tmp/awadb-0.3.2-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/awadb-0.3.3-cp311-cp311-macosx_10_13_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2449392 bytes, number of entries: 8
--rwxr-xr-x  2.0 unx  7073416 b- defN 23-Jun-05 14:15 awa.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx    26165 b- defN 23-Jun-05 14:01 awadb/__init__.py
--rw-r--r--  2.0 unx      816 b- defN 23-May-07 14:27 awadb/llm_embedding/__init__.py
--rw-r--r--  2.0 unx    15759 b- defN 23-Jun-05 14:15 awadb-0.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      415 b- defN 23-Jun-05 14:15 awadb-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-Jun-05 14:15 awadb-0.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-05 14:15 awadb-0.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      633 b- defN 23-Jun-05 14:15 awadb-0.3.2.dist-info/RECORD
-8 files, 7117322 bytes uncompressed, 2448300 bytes compressed:  65.6%
+Zip file size: 3207263 bytes, number of entries: 8
+-rwxr-xr-x  2.0 unx  9370840 b- defN 23-Jun-16 06:38 awa.cpython-311-darwin.so
+-rw-r--r--  2.0 unx    30442 b- defN 23-Jun-16 06:32 awadb/__init__.py
+-rw-r--r--  2.0 unx     1116 b- defN 23-Jun-16 06:33 awadb/llm_embedding/__init__.py
+-rw-r--r--  2.0 unx    15759 b- defN 23-Jun-16 06:38 awadb-0.3.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Jun-16 06:38 awadb-0.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-16 06:38 awadb-0.3.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-16 06:38 awadb-0.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      625 b- defN 23-Jun-16 06:38 awadb-0.3.3.dist-info/RECORD
+8 files, 9419288 bytes uncompressed, 3206189 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: awa.cpython-39-x86_64-linux-gnu.so
+Filename: awa.cpython-311-darwin.so
 Comment: 
 
 Filename: awadb/__init__.py
 Comment: 
 
 Filename: awadb/llm_embedding/__init__.py
 Comment: 
 
-Filename: awadb-0.3.2.dist-info/LICENSE
+Filename: awadb-0.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: awadb-0.3.2.dist-info/METADATA
+Filename: awadb-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: awadb-0.3.2.dist-info/WHEEL
+Filename: awadb-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: awadb-0.3.2.dist-info/top_level.txt
+Filename: awadb-0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: awadb-0.3.2.dist-info/RECORD
+Filename: awadb-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awadb/__init__.py

```diff
@@ -2,18 +2,20 @@
 #!/usr/bin/python3
 
 import os
 import numpy as np
 import struct
 import json
 import io
+import hashlib
 
 from enum import Enum
 
-from typing import Optional
+from typing import Optional, List, Any, Iterable
+import time
 import awa
 
 
 class FieldDataType(Enum):
     INT = 1
     FLOAT = 2 
     STRING = 3 
@@ -37,14 +39,18 @@
         if is_vector:
             v_type = FieldDataType.VECTOR
     elif type(variate).__name__ == 'ndarray':
         v_type = FieldDataType.VECTOR
 
     return v_type
 
+def md5str(str):
+    m = hashlib.md5(str.encode(encoding="utf-8"))
+    return m.hexdigest()
+
 
 class Client:
     def __init__(self, root_dir="."):
         self.root_dir = root_dir 
         log_dir = root_dir + '/log'
         data_dir = root_dir + '/data'
         if not os.path.isdir(log_dir):
@@ -70,14 +76,15 @@
 
 
         existed_meta_file = data_dir + '/tables.meta'
         if os.path.isfile(existed_meta_file):
             self.Read()
 
         self.llm = None
+        self.is_duplicate_texts = True
         
 
     def Write(self):
         tables_meta = {}
         tables_meta['fields_check'] = self.tables_fields_check
         tables_types = {} 
         for table_name in self.tables_fields_type:
@@ -276,23 +283,21 @@
             print('Table %s not exist! Please create first!' % table_name)
             return False
         self.using_table_name = table_name 
         self.using_table_engine = self.tables[table_name]
 
 
     def __FieldCheck(self, field_idx, field_name, field_data, fields_type):
+        f_type = typeof(field_data)
         if not self.tables_fields_check[self.using_table_name]:
-            f_type = typeof(field_data)
             if f_type == FieldDataType.ERROR:
                 error_msg = Exception("Field data type error! Please input right data type : int|float|string|vector!")
                 raise error_msg
             fields_type[field_idx] = f_type
         else:
-            f_type = typeof(field_data)
-             
             if self.tables_fields_type[self.using_table_name][field_idx] != f_type: 
                 error_msg = Exception("No. %d field data type not %d, should %d!" % (field_idx, f_type, self.tables_fields_type[self.using_table_name][field_idx]))
                 raise error_msg
             elif field_name != self.key_confirmed_name and (not (field_name in self.tables_fields_names[self.using_table_name])):
                 error_msg = Exception("Field name \'%s\' not exist!" % field_name)
                 raise error_msg
 
@@ -345,15 +350,14 @@
             awadb_field.value = struct.pack('<f', field_value)
             awadb_field.datatype = awa.DataType.FLOAT
             self.AddField(field_name, awadb_field.datatype, is_index)
         elif field_type == FieldDataType.STRING:
             awadb_field.value = field_value
             awadb_field.datatype = awa.DataType.STRING
             self.AddField(field_name, awadb_field.datatype, is_index)
- 
         
         elif field_type == FieldDataType.VECTOR:
             if (type(field_value).__name__ == 'ndarray'):
                 awadb_field.value = field_value.tobytes()
             else:
                 vec_value = np.array(field_value, dtype = np.dtype('float32'))
                 awadb_field.value = vec_value.tobytes()
@@ -438,14 +442,109 @@
                             field_value = field['embedding_text']
                         else:
                             continue
                     doc.append(self.llm.Embedding(field_value))
                     
             field_no = field_no + 1
 
+    def AddTexts(
+        self,
+        text_field_name: str,
+        embedding_field_name: str,
+        texts: Iterable[str],
+        embeddings: Optional[List[List[float]]] = None,
+        metadatas: Optional[List[dict]] = None,
+        is_duplicate_texts: Optional[bool] = None,
+        **args: Any,
+    ) -> List[str]:
+        added_ids: List[str] = []
+        if not self.tables_fields_check[self.using_table_name]:
+            if (self.using_table_name == ''):
+                print("Please specify your table name!")
+                return added_ids
+
+            self.tables_attr[self.using_table_name] = awa.TableInfo()
+            self.tables_attr[self.using_table_name].SetName(self.using_table_name)
+
+        if is_duplicate_texts is not None:
+            self.is_duplicate_texts = is_duplicate_texts
+
+        if embeddings is None:
+            if self.llm is None:
+                from awadb import llm_embedding
+                self.llm = llm_embedding.LLMEmbedding()
+
+            embeddings = self.llm.EmbeddingBatch(texts)
+
+        awa_docs = awa.DocsVec()
+
+        adding_docs_no = 0
+        for text in texts:
+            fields_type = {}
+            fields_names = {}
+            doc = awa.Doc()
+            key_field = awa.Field()
+            key_field_name = '_id'
+            key_field_value = ''
+            # add unique primary id for each unique document
+            if self.is_duplicate_texts:
+                key_field_value = md5str(text)
+            # auto increasing id
+            else:
+                key_field_value = str(self.tables_doc_count[self.using_table_name])
+            self.tables_primary_key_fid_no[self.using_table_name] = 0
+            self.CheckAddField(key_field, fields_type, 0, key_field_name, key_field_value, True)
+            if (not self.tables_fields_check[self.using_table_name]):
+                fields_names[key_field_name] = 0
+            doc.AddField(key_field)
+            added_ids.append(key_field.value)
+            doc.SetKey(key_field.value)
+            text_field = awa.Field()
+            self.CheckAddField(text_field, fields_type, 1, text_field_name, text, True)
+            if (not self.tables_fields_check[self.using_table_name]):
+                fields_names[text_field_name] = 1
+            embedding_field = awa.Field()
+            self.CheckAddField(embedding_field, fields_type, 2, embedding_field_name, embeddings[adding_docs_no], True)
+            if (not self.tables_fields_check[self.using_table_name]):
+                fields_names[embedding_field_name] = 2
+
+            doc.AddField(text_field)
+            doc.AddField(embedding_field)
+            fid_no = 3
+            if metadatas is not None:
+                for field in metadatas[adding_docs_no]:
+                    meta_field = awa.Field()
+                    self.CheckAddField(meta_field, fields_type, fid_no, field, metadatas[adding_docs_no][field], True)
+                    if (not self.tables_fields_check[self.using_table_name]):
+                        fields_names[field] = fid_no
+
+                    fid_no = fid_no + 1
+                    doc.AddField(meta_field)
+
+            awa_docs.append(doc)
+            self.tables_doc_count[self.using_table_name] += 1
+            adding_docs_no = adding_docs_no + 1
+            if (not self.tables_fields_check[self.using_table_name]):
+                self.tables_attr[self.using_table_name].SetIndexingSize(10000)
+                self.tables_attr[self.using_table_name].SetRetrievalType('IVFPQ')
+                self.tables_attr[self.using_table_name].SetRetrievalParam('{"ncentroids" : 256, "nsubvector" : 16}')
+                self.tables_fields_type[self.using_table_name] = fields_type
+                self.tables_fields_names[self.using_table_name] = fields_names
+
+                if not awa.Create(self.using_table_engine, self.tables_attr[self.using_table_name]):
+                    error_msg = Exception("Create table error!!!")
+                    raise error_msg
+
+                self.tables_fields_check[self.using_table_name] = True
+                self.Write()
+
+        awa.AddTexts(self.using_table_engine, awa_docs)
+
+        return added_ids
+
     '''
     primary_key : format @name
     is_index :  format !province
     '''
     def Add(self, doc):
         if not isinstance(doc, list):
             error_msg = Exception("Incorrect argument, list type is needed for Add!!!")
```

## awadb/llm_embedding/__init__.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 #!/usr/bin/python3
 
 from sentence_transformers import SentenceTransformer
 from transformers import AutoModel
 from transformers import AutoTokenizer
-
+from typing import Iterable, Any, List
 
 class LLMEmbedding:
     def __init__(self):
         self.model = SentenceTransformer('all-MiniLM-L6-v2')
         self.tokenizer = None 
 
 
@@ -16,14 +16,24 @@
         tokens = []
         if self.tokenizer != None:
             tokens = self.tokenizer.tokenize(sentence)
         else:
             tokens.append(sentence)
         return self.model.encode(tokens[0])
 
+    def EmbeddingBatch(
+        self,
+        texts: Iterable[str],
+        **kwargs: Any,
+    ) -> List[List[float]]:
+        results: List[List[float]] = []
+        for text in texts:
+            results.append(self.model.encode(text))
+        return results
+
     #set your own llm
     def SetModel(self, model_name):
         self.model = AutoModel.from_pretrained(model_name)
 
     #set your own tokenizer
     def SetTokenizer(self, tokenizer_name):
         self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
```

## Comparing `awadb-0.3.2.dist-info/LICENSE` & `awadb-0.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

