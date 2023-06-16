# Comparing `tmp/natural-keys-2.0.0.tar.gz` & `tmp/natural-keys-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/natural-keys-2.0.0.tar", last modified: Tue Aug 24 12:23:01 2021, max compression
+gzip compressed data, was "natural-keys-2.1.0.tar", last modified: Fri Jun 16 14:22:24 2023, max compression
```

## Comparing `natural-keys-2.0.0.tar` & `natural-keys-2.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:23:01.000000 natural-keys-2.0.0/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       40 2021-08-24 12:22:31.000000 natural-keys-2.0.0/.gitignore
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:23:01.000000 natural-keys-2.0.0/tests/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8637 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/test_rest.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      107 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/urls.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3749 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/test_naturalkey.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      262 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/settings.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      315 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/__init__.py
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:23:01.000000 natural-keys-2.0.0/tests/test_app/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1351 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/test_app/models.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      637 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/test_app/urls.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1470 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/test_app/views.py
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:23:01.000000 natural-keys-2.0.0/tests/test_app/migrations/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     3057 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/test_app/migrations/0001_initial.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/test_app/migrations/__init__.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:22:31.000000 natural-keys-2.0.0/tests/test_app/__init__.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1106 2021-08-24 12:22:31.000000 natural-keys-2.0.0/LICENSE
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)    11495 2021-08-24 12:22:31.000000 natural-keys-2.0.0/README.md
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:23:01.000000 natural-keys-2.0.0/natural_keys/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8555 2021-08-24 12:22:31.000000 natural-keys-2.0.0/natural_keys/models.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     7589 2021-08-24 12:22:31.000000 natural-keys-2.0.0/natural_keys/serializers.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      394 2021-08-24 12:22:31.000000 natural-keys-2.0.0/natural_keys/__init__.py
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:23:01.000000 natural-keys-2.0.0/.github/
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:23:01.000000 natural-keys-2.0.0/.github/workflows/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1816 2021-08-24 12:22:31.000000 natural-keys-2.0.0/.github/workflows/test.yml
-drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2021-08-24 12:23:01.000000 natural-keys-2.0.0/natural_keys.egg-info/
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       13 2021-08-24 12:23:01.000000 natural-keys-2.0.0/natural_keys.egg-info/top_level.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)        1 2021-08-24 12:23:01.000000 natural-keys-2.0.0/natural_keys.egg-info/dependency_links.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)      592 2021-08-24 12:23:01.000000 natural-keys-2.0.0/natural_keys.egg-info/SOURCES.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       23 2021-08-24 12:23:01.000000 natural-keys-2.0.0/natural_keys.egg-info/requires.txt
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)    14550 2021-08-24 12:23:01.000000 natural-keys-2.0.0/natural_keys.egg-info/PKG-INFO
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)       38 2021-08-24 12:23:01.000000 natural-keys-2.0.0/setup.cfg
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1417 2021-08-24 12:22:31.000000 natural-keys-2.0.0/setup.py
--rw-r--r--   0 sheppard  (1000) sheppard  (1000)    14550 2021-08-24 12:23:01.000000 natural-keys-2.0.0/PKG-INFO
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:22:24.590177 natural-keys-2.1.0/
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:22:24.386578 natural-keys-2.1.0/.github/
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:22:24.437580 natural-keys-2.1.0/.github/workflows/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     2005 2023-06-16 14:21:06.000000 natural-keys-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       40 2023-06-16 14:21:06.000000 natural-keys-2.1.0/.gitignore
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1106 2023-06-16 14:21:06.000000 natural-keys-2.1.0/LICENSE
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)    12894 2023-06-16 14:22:24.586949 natural-keys-2.1.0/PKG-INFO
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)    11495 2023-06-16 14:21:06.000000 natural-keys-2.1.0/README.md
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:22:24.462586 natural-keys-2.1.0/natural_keys/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      408 2023-06-16 14:21:06.000000 natural-keys-2.1.0/natural_keys/__init__.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8902 2023-06-16 14:21:06.000000 natural-keys-2.1.0/natural_keys/models.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     7693 2023-06-16 14:21:06.000000 natural-keys-2.1.0/natural_keys/serializers.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:22:24.496580 natural-keys-2.1.0/natural_keys.egg-info/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)    12894 2023-06-16 14:22:24.000000 natural-keys-2.1.0/natural_keys.egg-info/PKG-INFO
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      598 2023-06-16 14:22:24.000000 natural-keys-2.1.0/natural_keys.egg-info/SOURCES.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)        1 2023-06-16 14:22:24.000000 natural-keys-2.1.0/natural_keys.egg-info/dependency_links.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       23 2023-06-16 14:22:24.000000 natural-keys-2.1.0/natural_keys.egg-info/requires.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       13 2023-06-16 14:22:24.000000 natural-keys-2.1.0/natural_keys.egg-info/top_level.txt
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1428 2023-06-16 14:21:06.000000 natural-keys-2.1.0/pyproject.toml
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)       38 2023-06-16 14:22:24.592177 natural-keys-2.1.0/setup.cfg
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:22:24.530561 natural-keys-2.1.0/tests/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      315 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/__init__.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      262 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/settings.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:22:24.561646 natural-keys-2.1.0/tests/test_app/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/test_app/__init__.py
+drwxr-xr-x   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:22:24.579165 natural-keys-2.1.0/tests/test_app/migrations/
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4481 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/test_app/migrations/0001_initial.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)        0 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/test_app/migrations/__init__.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1413 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/test_app/models.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      639 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/test_app/urls.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     1449 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/test_app/views.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     4091 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/test_naturalkey.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)     8585 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/test_rest.py
+-rw-r--r--   0 sheppard  (1000) sheppard  (1000)      104 2023-06-16 14:21:06.000000 natural-keys-2.1.0/tests/urls.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `natural-keys-2.0.0/tests/test_rest.py` & `natural-keys-2.1.0/tests/test_rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 try:
     from rest_framework.test import APITestCase
 except ImportError:
     raise unittest.SkipTest("Skipping DRF tests as DRF is not installed.")
 
 from rest_framework import status
 from tests.test_app.models import (
-    NaturalKeyChild, ModelWithNaturalKey, ModelWithSingleUniqueField,
+    NaturalKeyChild,
+    ModelWithNaturalKey,
+    ModelWithSingleUniqueField,
 )
 from natural_keys import NaturalKeySerializer
 
 # Tests for natural key DRF integration
 
 
 class NaturalKeyRestTestCase(APITestCase):
@@ -21,221 +23,216 @@
         expect = """
              Serializer():
                  parent = Serializer():
                      code = CharField(max_length=10)
                      group = CharField(max_length=10)
                  mode = CharField(max_length=10)
                  class Meta:
-                     validators = [<NaturalKeyValidator(queryset=NaturalKeyChild.objects.all(), fields=('parent', 'mode'))>]""".replace("             ", "")[1:]  # noqa
+                     validators = [<NaturalKeyValidator(queryset=NaturalKeyChild.objects.all(), fields=('parent', 'mode'))>]""".replace(
+            "             ", ""
+        )[
+            1:
+        ]  # noqa
         self.assertEqual(expect, str(serializer))
 
         fields = serializer.get_fields()
-        self.assertTrue(fields['parent'].required)
-        self.assertTrue(fields['mode'].required)
-        self.assertTrue(fields['parent'].get_fields()['code'].required)
+        self.assertTrue(fields["parent"].required)
+        self.assertTrue(fields["mode"].required)
+        self.assertTrue(fields["parent"].get_fields()["code"].required)
 
     def test_naturalkey_rest_singleunique(self):
         # Serializer should only have single top-level validator
         serializer = NaturalKeySerializer.for_model(
             ModelWithSingleUniqueField
         )()
         expect = """
              Serializer():
                  code = CharField(max_length=10, validators=[])
                  class Meta:
-                     validators = [<NaturalKeyValidator(queryset=ModelWithSingleUniqueField.objects.all(), fields=('code',))>]""".replace("             ", "")[1:]  # noqa
+                     validators = [<NaturalKeyValidator(queryset=ModelWithSingleUniqueField.objects.all(), fields=('code',))>]""".replace(
+            "             ", ""
+        )[
+            1:
+        ]  # noqa
         self.assertEqual(expect, str(serializer))
 
         fields = serializer.get_fields()
-        self.assertTrue(fields['code'].required)
+        self.assertTrue(fields["code"].required)
 
     def test_naturalkey_rest_post(self):
         # Posting a compound natural key should work
         form = {
-            'mode': 'mode3a',
-            'parent[code]': "code3",
-            'parent[group]': "group3",
+            "mode": "mode3a",
+            "parent[code]": "code3",
+            "parent[group]": "group3",
         }
-        response = self.client.post('/naturalkeychilds.json', form)
+        response = self.client.post("/naturalkeychilds.json", form)
         self.assertEqual(
             response.status_code, status.HTTP_201_CREATED, response.data
         )
-        self.assertEqual(response.data['mode'], "mode3a")
-        self.assertEqual(response.data['parent']['code'], "code3")
-        self.assertEqual(response.data['parent']['group'], "group3")
+        self.assertEqual(response.data["mode"], "mode3a")
+        self.assertEqual(response.data["parent"]["code"], "code3")
+        self.assertEqual(response.data["parent"]["group"], "group3")
 
         # Posting a simple natural key should work
         form = {
-            'code': 'code9',
+            "code": "code9",
         }
-        response = self.client.post('/modelwithsingleuniquefield.json', form)
+        response = self.client.post("/modelwithsingleuniquefield.json", form)
         self.assertEqual(
             response.status_code, status.HTTP_201_CREATED, response.data
         )
-        self.assertEqual(response.data['code'], "code9")
+        self.assertEqual(response.data["code"], "code9")
 
         # Posting same nested natural key should reuse nested object
         form = {
-            'mode': 'mode3b',
-            'parent[code]': "code3",
-            'parent[group]': "group3",
+            "mode": "mode3b",
+            "parent[code]": "code3",
+            "parent[group]": "group3",
         }
-        response = self.client.post('/naturalkeychilds.json', form)
+        response = self.client.post("/naturalkeychilds.json", form)
         self.assertEqual(
             response.status_code, status.HTTP_201_CREATED, response.data
         )
         self.assertEqual(
-            NaturalKeyChild.objects.get(mode='mode3a').parent.pk,
-            NaturalKeyChild.objects.get(mode='mode3b').parent.pk,
+            NaturalKeyChild.objects.get(mode="mode3a").parent.pk,
+            NaturalKeyChild.objects.get(mode="mode3b").parent.pk,
         )
 
     def test_naturalkey_rest_duplicate(self):
         # Posting identical compound natural key should fail
         form = {
-            'mode': 'mode3c',
-            'parent[code]': "code3",
-            'parent[group]': "group3",
+            "mode": "mode3c",
+            "parent[code]": "code3",
+            "parent[group]": "group3",
         }
-        response = self.client.post('/naturalkeychilds.json', form)
+        response = self.client.post("/naturalkeychilds.json", form)
         self.assertEqual(
             response.status_code, status.HTTP_201_CREATED, response.data
         )
         form = {
-            'mode': 'mode3c',
-            'parent[code]': "code3",
-            'parent[group]': "group3",
+            "mode": "mode3c",
+            "parent[code]": "code3",
+            "parent[group]": "group3",
         }
-        response = self.client.post('/naturalkeychilds.json', form)
+        response = self.client.post("/naturalkeychilds.json", form)
         self.assertEqual(
             response.status_code, status.HTTP_400_BAD_REQUEST, response.data
         )
         self.assertEqual(
-            response.data, {
-                'non_field_errors': [
-                    'The fields parent, mode must make a unique set.'
+            response.data,
+            {
+                "non_field_errors": [
+                    "The fields parent, mode must make a unique set."
                 ]
-            }
+            },
         )
 
         # Posting identical simple natural key should fail
         form = {
-            'code': 'code8',
+            "code": "code8",
         }
-        response = self.client.post('/modelwithsingleuniquefield.json', form)
+        response = self.client.post("/modelwithsingleuniquefield.json", form)
         self.assertEqual(
             response.status_code, status.HTTP_201_CREATED, response.data
         )
         form = {
-            'code': 'code8',
+            "code": "code8",
         }
-        response = self.client.post('/modelwithsingleuniquefield.json', form)
+        response = self.client.post("/modelwithsingleuniquefield.json", form)
         self.assertEqual(
             response.status_code, status.HTTP_400_BAD_REQUEST, response.data
         )
         self.assertEqual(
-            response.data, {
-                'code': [
-                    'model with single unique field '
-                    'with this code already exists.'
+            response.data,
+            {
+                "code": [
+                    "model with single unique field "
+                    "with this code already exists."
                 ]
-            }
+            },
         )
 
     def test_naturalkey_rest_nested_post(self):
         # Posting a regular model with a ref to natural key
         form = {
-            'key[mode]': 'mode4',
-            'key[parent][code]': "code4",
-            'key[parent][group]': "group4",
-            'value': 5,
+            "key[mode]": "mode4",
+            "key[parent][code]": "code4",
+            "key[parent][group]": "group4",
+            "value": 5,
         }
-        response = self.client.post('/modelwithnaturalkeys.json', form)
+        response = self.client.post("/modelwithnaturalkeys.json", form)
         self.assertEqual(
             response.status_code, status.HTTP_201_CREATED, response.data
         )
-        self.assertEqual(response.data['key']['mode'], "mode4")
-        self.assertEqual(response.data['key']['parent']['code'], "code4")
-        self.assertEqual(response.data['key']['parent']['group'], "group4")
+        self.assertEqual(response.data["key"]["mode"], "mode4")
+        self.assertEqual(response.data["key"]["parent"]["code"], "code4")
+        self.assertEqual(response.data["key"]["parent"]["group"], "group4")
 
     def test_naturalkey_rest_nested_put(self):
         # Updating a regular model with a ref to natural key
         instance = ModelWithNaturalKey.objects.create(
-            key=NaturalKeyChild.objects.find(
-                'code5', 'group5', 'mode5'
-            ),
+            key=NaturalKeyChild.objects.find("code5", "group5", "mode5"),
             value=7,
         )
-        self.assertEqual(instance.key.parent.code, 'code5')
+        self.assertEqual(instance.key.parent.code, "code5")
 
         # Updating with same natural key should reuse it
         form = {
-            'key[mode]': 'mode5',
-            'key[parent][code]': "code5",
-            'key[parent][group]': "group5",
-            'value': 8,
+            "key[mode]": "mode5",
+            "key[parent][code]": "code5",
+            "key[parent][group]": "group5",
+            "value": 8,
         }
-        self.assertEqual(
-            NaturalKeyChild.objects.count(),
-            1
-        )
+        self.assertEqual(NaturalKeyChild.objects.count(), 1)
 
         # Updating with new natural key should create it
         response = self.client.put(
-            '/modelwithnaturalkeys/%s.json' % instance.pk, form
+            "/modelwithnaturalkeys/%s.json" % instance.pk, form
         )
         form = {
-            'key[mode]': 'mode6',
-            'key[parent][code]': "code6",
-            'key[parent][group]': "group6",
-            'value': 9,
+            "key[mode]": "mode6",
+            "key[parent][code]": "code6",
+            "key[parent][group]": "group6",
+            "value": 9,
         }
         response = self.client.put(
-            '/modelwithnaturalkeys/%s.json' % instance.pk, form
+            "/modelwithnaturalkeys/%s.json" % instance.pk, form
         )
         self.assertEqual(
             response.status_code, status.HTTP_200_OK, response.data
         )
-        self.assertEqual(response.data['key']['mode'], "mode6")
-        self.assertEqual(response.data['key']['parent']['code'], "code6")
-        self.assertEqual(response.data['key']['parent']['group'], "group6")
-        self.assertEqual(
-            NaturalKeyChild.objects.count(),
-            2
-        )
+        self.assertEqual(response.data["key"]["mode"], "mode6")
+        self.assertEqual(response.data["key"]["parent"]["code"], "code6")
+        self.assertEqual(response.data["key"]["parent"]["group"], "group6")
+        self.assertEqual(NaturalKeyChild.objects.count(), 2)
 
     def test_naturalkey_lookup(self):
         # Support natural_key_slug as lookup_field setting
-        NaturalKeyChild.objects.find(
-            'code7', 'group7', 'mode7'
-        )
+        NaturalKeyChild.objects.find("code7", "group7", "mode7")
         response = self.client.get(
-            '/naturalkeylookup/code7-group7-mode7.json',
+            "/naturalkeylookup/code7-group7-mode7.json",
         )
         self.assertEqual(
             response.status_code, status.HTTP_200_OK, response.data
         )
-        self.assertEqual(
-            response.data['id'], 'code7-group7-mode7'
-        )
+        self.assertEqual(response.data["id"], "code7-group7-mode7")
 
     def test_naturalkey_lookup_slug(self):
         # Support separator in slug (but only for last part of key)
-        NaturalKeyChild.objects.find(
-            'code7', 'group7', 'mode7-alt'
-        )
+        NaturalKeyChild.objects.find("code7", "group7", "mode7-alt")
         response = self.client.get(
-            '/naturalkeylookup/code7-group7-mode7-alt.json',
+            "/naturalkeylookup/code7-group7-mode7-alt.json",
         )
         self.assertEqual(
             response.status_code, status.HTTP_200_OK, response.data
         )
-        self.assertEqual(
-            response.data['id'], 'code7-group7-mode7-alt'
-        )
+        self.assertEqual(response.data["id"], "code7-group7-mode7-alt")
 
     def test_invalid_slug_404(self):
         response = self.client.get(
-            '/naturalkeylookup/not-valid.json',
+            "/naturalkeylookup/not-valid.json",
         )
         self.assertEqual(
-            status.HTTP_404_NOT_FOUND, response.status_code,
+            status.HTTP_404_NOT_FOUND,
+            response.status_code,
         )
```

### Comparing `natural-keys-2.0.0/tests/test_naturalkey.py` & `natural-keys-2.1.0/tests/test_naturalkey.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 from django.test import TestCase
 from tests.test_app.models import (
-    NaturalKeyParent, NaturalKeyChild,
-    ModelWithSingleUniqueField, ModelWithExtraField, ModelWithConstraint
+    NaturalKeyParent,
+    NaturalKeyChild,
+    ModelWithSingleUniqueField,
+    ModelWithExtraField,
+    ModelWithConstraint,
 )
 from django.db.utils import IntegrityError
 
 # Tests for natural key models
 
 
 class NaturalKeyTestCase(TestCase):
     def test_naturalkey_fields(self):
         # Model APIs
         self.assertEqual(
             NaturalKeyParent.get_natural_key_fields(),
-            ['code', 'group']
+            ("code", "group"),
         )
         self.assertEqual(
-            NaturalKeyParent(code='code0', group='group0').natural_key(),
-            ['code0', 'group0'],
+            NaturalKeyParent(code="code0", group="group0").natural_key(),
+            ("code0", "group0"),
         )
         self.assertEqual(
             NaturalKeyChild.get_natural_key_fields(),
-            ['parent__code', 'parent__group', 'mode']
+            ("parent__code", "parent__group", "mode"),
         )
         self.assertEqual(
             ModelWithSingleUniqueField.get_natural_key_fields(),
-            ['code']
+            ("code",),
         )
 
     def test_naturalkey_create(self):
         # Manager create
-        p1 = NaturalKeyParent.objects.create_by_natural_key(
-            "code1", "group1"
-        )
+        p1 = NaturalKeyParent.objects.create_by_natural_key("code1", "group1")
         self.assertEqual(p1.code, "code1")
         self.assertEqual(p1.group, "group1")
 
         # get_or_create with same key retrieve existing item
         p2, is_new = NaturalKeyParent.objects.get_or_create_by_natural_key(
             "code1", "group1"
         )
         self.assertFalse(is_new)
         self.assertEqual(p1.pk, p2.pk)
 
         # Shortcut version
         p3 = NaturalKeyParent.objects.find("code1", "group1")
         self.assertEqual(p1.pk, p3.pk)
 
-        p4 = ModelWithSingleUniqueField.objects.create_by_natural_key(
-            "code4"
-        )
+        p4 = ModelWithSingleUniqueField.objects.create_by_natural_key("code4")
         self.assertEqual(p4.code, "code4")
 
     def test_naturalkey_nested_create(self):
         # Manager create, with nested natural key
         c1 = NaturalKeyChild.objects.create_by_natural_key(
             "code2", "group2", "mode1"
         )
@@ -66,55 +65,64 @@
             "code2", "group2", "mode2"
         )
         self.assertEqual(c1.parent.pk, c2.parent.pk)
         self.assertEqual(c2.mode, "mode2")
 
     def test_naturalkey_duplicate(self):
         # Manager create, with duplicate
-        NaturalKeyParent.objects.create_by_natural_key(
-            "code1", "group1"
-        )
+        NaturalKeyParent.objects.create_by_natural_key("code1", "group1")
         # create with same key should fail
         with self.assertRaises(IntegrityError):
-            NaturalKeyParent.objects.create_by_natural_key(
-                "code1", "group1"
-            )
+            NaturalKeyParent.objects.create_by_natural_key("code1", "group1")
 
     def test_filter_with_Q(self):
         from django.db.models import Q
+
         query = Q(code="bizarre")
         self.assertEqual(
-            ModelWithSingleUniqueField.objects.filter(query).count(),
-            0
+            ModelWithSingleUniqueField.objects.filter(query).count(), 0
         )
 
     def test_find_with_defaults(self):
         obj = ModelWithExtraField.objects.find(
-            'extra1',
-            '2019-07-26',
-            defaults={'extra': 'Test 123'},
-        )
-        self.assertEqual(
-            obj.extra,
-            'Test 123'
+            "extra1",
+            "2019-07-26",
+            defaults={"extra": "Test 123"},
         )
+        self.assertEqual(obj.extra, "Test 123")
 
     def test_find_with_kwargs(self):
         with self.assertRaises(TypeError) as e:
             ModelWithExtraField.objects.find(
-                'extra1',
-                date='2019-07-26',
+                "extra1",
+                date="2019-07-26",
             )
+        msg = str(e.exception).replace("NaturalKeyModelManager.", "")
         self.assertEqual(
-            str(e.exception),
-            "find() got an unexpected keyword argument 'date'"
+            msg, "find() got an unexpected keyword argument 'date'"
         )
 
     def test_find_with_constraint(self):
         obj = ModelWithConstraint.objects.find(
-            'constraint1',
-            '2021-08-23',
+            "constraint1",
+            "2021-08-23",
         )
+        self.assertEqual(str(obj), "constraint1 2021-08-23")
+
+    def test_null_foreign_key(self):
+        obj = NaturalKeyChild.objects.create(mode="mode0")
         self.assertEqual(
-            str(obj),
-            'constraint1 2021-08-23'
+            obj.natural_key(),
+            (
+                None,
+                None,
+                "mode0",
+            ),
+        )
+        self.assertEqual(
+            NaturalKeyChild.objects.get_by_natural_key(
+                None,
+                None,
+                "mode0",
+            ),
+            obj,
         )
```

### Comparing `natural-keys-2.0.0/tests/test_app/models.py` & `natural-keys-2.1.0/tests/test_app/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 
 
 class NaturalKeyParent(NaturalKeyModel):
     code = models.CharField(max_length=10)
     group = models.CharField(max_length=10)
 
     class Meta:
-        unique_together = ['code', 'group']
+        unique_together = ["code", "group"]
 
 
 class NaturalKeyChild(NaturalKeyModel):
-    parent = models.ForeignKey(NaturalKeyParent, on_delete=models.CASCADE)
+    parent = models.ForeignKey(
+        NaturalKeyParent,
+        on_delete=models.CASCADE,
+        null=True,
+        blank=True,
+    )
     mode = models.CharField(max_length=10)
 
     class Meta:
-        unique_together = ['parent', 'mode']
+        unique_together = ["parent", "mode"]
 
 
 class ModelWithNaturalKey(models.Model):
     key = models.ForeignKey(NaturalKeyChild, on_delete=models.CASCADE)
     value = models.CharField(max_length=10)
 
 
@@ -29,24 +34,24 @@
 
 class ModelWithExtraField(NaturalKeyModel):
     code = models.CharField(max_length=10)
     date = models.DateField(max_length=10)
     extra = models.TextField()
 
     class Meta:
-        unique_together = ['code', 'date']
+        unique_together = ["code", "date"]
 
 
 class ModelWithConstraint(NaturalKeyModel):
     code = models.CharField(max_length=10)
     date = models.DateField(max_length=10)
 
     def __str__(self):
-        return f'{self.code} {self.date}'
+        return f"{self.code} {self.date}"
 
     class Meta:
         constraints = [
             models.UniqueConstraint(
-                name='natural key',
-                fields=['code', 'date'],
+                name="natural key",
+                fields=["code", "date"],
             ),
         ]
```

### Comparing `natural-keys-2.0.0/tests/test_app/urls.py` & `natural-keys-2.1.0/tests/test_app/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 try:
     from rest_framework import routers
 except ImportError:
     urlpatterns = []
 else:
     from .views import (
-        NaturalKeyChildViewSet, ModelWithNaturalKeyViewSet,
+        NaturalKeyChildViewSet,
+        ModelWithNaturalKeyViewSet,
         ModelWithSingleUniqueFieldViewSet,
         NaturalKeyLookupViewSet,
     )
 
     router = routers.DefaultRouter()
-    router.register(r'naturalkeychilds', NaturalKeyChildViewSet)
-    router.register(r'modelwithnaturalkeys', ModelWithNaturalKeyViewSet)
-    router.register(r'modelwithsingleuniquefield',
-                    ModelWithSingleUniqueFieldViewSet)
-    router.register(r'naturalkeylookup', NaturalKeyLookupViewSet)
+    router.register(r"naturalkeychilds", NaturalKeyChildViewSet)
+    router.register(r"modelwithnaturalkeys", ModelWithNaturalKeyViewSet)
+    router.register(
+        r"modelwithsingleuniquefield", ModelWithSingleUniqueFieldViewSet
+    )
+    router.register(r"naturalkeylookup", NaturalKeyLookupViewSet)
 
     urlpatterns = router.urls
```

### Comparing `natural-keys-2.0.0/tests/test_app/views.py` & `natural-keys-2.1.0/tests/test_app/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 try:
     from rest_framework import viewsets
     from rest_framework import serializers
 except ImportError:
     pass
 else:
     from .models import (
-        NaturalKeyChild, ModelWithNaturalKey, ModelWithSingleUniqueField
-    )
-    from natural_keys import (
-        NaturalKeySerializer, NaturalKeyModelSerializer
+        NaturalKeyChild,
+        ModelWithNaturalKey,
+        ModelWithSingleUniqueField,
     )
+    from natural_keys import NaturalKeySerializer, NaturalKeyModelSerializer
 
     class NaturalKeyChildViewSet(viewsets.ModelViewSet):
         queryset = NaturalKeyChild.objects.all()
-        serializer_class = NaturalKeySerializer.for_model(
-            NaturalKeyChild
-        )
+        serializer_class = NaturalKeySerializer.for_model(NaturalKeyChild)
 
     class ModelWithNaturalKeyViewSet(viewsets.ModelViewSet):
         queryset = ModelWithNaturalKey.objects.all()
         serializer_class = NaturalKeyModelSerializer.for_model(
             ModelWithNaturalKey,
             include_fields="__all__",
         )
@@ -37,8 +35,8 @@
         class Meta:
             model = NaturalKeyChild
             fields = "__all__"
 
     class NaturalKeyLookupViewSet(viewsets.ModelViewSet):
         queryset = NaturalKeyChild.objects.all()
         serializer_class = LookupSerializer
-        lookup_field = 'natural_key_slug'
+        lookup_field = "natural_key_slug"
```

### Comparing `natural-keys-2.0.0/LICENSE` & `natural-keys-2.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2016-2021 S. Andrew Sheppard, https://wq.io/
+Copyright (c) 2016-2023 S. Andrew Sheppard, https://wq.io/
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `natural-keys-2.0.0/README.md` & `natural-keys-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -240,18 +240,18 @@
     fields='__all__',
     lookup='natural_key_slug',
 )
 ```
 
 Note that the `natural_key_slug` may not behave as expected if any of the component values contain the delimiter character (`-` by default).  To mitigate this, you can set `natural_key_separator` on the model class to another character.
 
-[natural keys]: https://docs.djangoproject.com/en/3.2/topics/serialization/#natural-keys
-[UniqueConstraint]: https://docs.djangoproject.com/en/3.2/ref/models/constraints/#uniqueconstraint
-[unique_together]: https://docs.djangoproject.com/en/3.2/ref/models/options/#unique-together
-[unique]: https://docs.djangoproject.com/en/3.2/ref/models/fields/#unique
+[natural keys]: https://docs.djangoproject.com/en/4.2/topics/serialization/#natural-keys
+[UniqueConstraint]: https://docs.djangoproject.com/en/4.2/ref/models/constraints/#uniqueconstraint
+[unique_together]: https://docs.djangoproject.com/en/4.2/ref/models/options/#unique-together
+[unique]: https://docs.djangoproject.com/en/4.2/ref/models/fields/#unique
 
 [wq.db]: https://wq.io/wq.db/
 [Django REST Framework]: http://www.django-rest-framework.org/
 [vera.Report]:https://github.com/powered-by-wq/vera#report
 [vera.Event]: https://github.com/powered-by-wq/vera#event
 [ModelSerializer]: https://www.django-rest-framework.org/api-guide/serializers/#modelserializer
 [RelatedField]: https://www.django-rest-framework.org/api-guide/relations/
```

### Comparing `natural-keys-2.0.0/natural_keys/models.py` & `natural-keys-2.1.0/natural_keys/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from django.db import models
 from functools import reduce
 
 
 class NaturalKeyQuerySet(models.QuerySet):
     def filter(self, *args, **kwargs):
-        natural_key_slug = kwargs.pop('natural_key_slug', None)
+        natural_key_slug = kwargs.pop("natural_key_slug", None)
         if natural_key_slug and type(natural_key_slug) is str:
-            slugs = natural_key_slug.split(
-                self.model.natural_key_separator
-            )
+            slugs = natural_key_slug.split(self.model.natural_key_separator)
             fields = self.model.get_natural_key_fields()
             if len(slugs) > len(fields):
-                slugs[len(fields) - 1:] = [
+                slugs[len(fields) - 1 :] = [
                     self.model.natural_key_separator.join(
-                        slugs[len(fields) - 1:]
+                        slugs[len(fields) - 1 :]
                     )
                 ]
             elif len(slugs) < len(fields):
                 return self.none()
             kwargs.update(self.natural_key_kwargs(*slugs))
 
         return super(NaturalKeyQuerySet, self).filter(*args, **kwargs)
 
     def natural_key_kwargs(self, *args):
         natural_key = self.model.get_natural_key_fields()
         if len(args) != len(natural_key):
-            raise TypeError("Wrong number of values, expected %s"
-                            % len(natural_key))
+            raise TypeError(
+                "Wrong number of values, expected %s" % len(natural_key)
+            )
         return dict(zip(natural_key, args))
 
 
 class NaturalKeyModelManager(models.Manager):
     """
     Manager for use with subclasses of NaturalKeyModel.
     """
+
     def get_queryset(self):
         return NaturalKeyQuerySet(self.model, using=self._db)
 
     def get_by_natural_key(self, *args):
         """
         Return the object corresponding to the provided natural key.
 
@@ -81,44 +81,54 @@
         kwargs = self.natural_key_kwargs(*args)
         for name, rel_to in self.model.get_natural_key_info():
             if not rel_to:
                 continue
             nested_key = extract_nested_key(kwargs, rel_to, name)
             # Automatically create any related objects as needed
             if nested_key:
-                kwargs[name], is_new = (
-                    rel_to.objects.get_or_create_by_natural_key(*nested_key)
-                )
+                (
+                    kwargs[name],
+                    is_new,
+                ) = rel_to.objects.get_or_create_by_natural_key(*nested_key)
             else:
                 kwargs[name] = None
         if defaults:
             attrs = defaults
             attrs.update(kwargs)
         else:
             attrs = kwargs
         return self.create(**attrs)
 
     def get_or_create_by_natural_key(self, *args, defaults=None):
         """
         get_or_create + get_by_natural_key
         """
         try:
-            return self.get_by_natural_key(*args), False
+            return (
+                self.get_by_natural_key(*args),
+                False,
+            )
         except self.model.DoesNotExist:
-            return self.create_by_natural_key(*args, defaults=defaults), True
+            return (
+                self.create_by_natural_key(
+                    *args,
+                    defaults=defaults,
+                ),
+                True,
+            )
 
     # Shortcut for common use case
     def find(self, *args, defaults=None):
         """
         Shortcut for get_or_create_by_natural_key that discards the "created"
         boolean.
         """
         obj, is_new = self.get_or_create_by_natural_key(
             *args,
-            defaults=defaults
+            defaults=defaults,
         )
         return obj
 
     def natural_key_kwargs(self, *args):
         """
         Convert args into kwargs by merging with model's natural key fieldnames
         """
@@ -157,44 +167,44 @@
         fields are related objects vs. regular fields.
         """
         fields = cls.get_natural_key_def()
         info = []
         for name in fields:
             field = cls._meta.get_field(name)
             rel_to = None
-            if hasattr(field, 'rel'):
+            if hasattr(field, "rel"):
                 rel_to = field.rel.to if field.rel else None
-            elif hasattr(field, 'remote_field'):
+            elif hasattr(field, "remote_field"):
                 if field.remote_field:
                     rel_to = field.remote_field.model
                 else:
                     rel_to = None
             info.append((name, rel_to))
         return info
 
     @classmethod
     def get_natural_key_def(cls):
-        if hasattr(cls, '_natural_key'):
+        if hasattr(cls, "_natural_key"):
             return cls._natural_key
 
         for constraint in cls._meta.constraints:
             if isinstance(constraint, models.UniqueConstraint):
                 return constraint.fields
 
         if cls._meta.unique_together:
             return cls._meta.unique_together[0]
 
         unique = [
-            f for f in cls._meta.fields
-            if f.unique and f.__class__.__name__ not in [
-                'AutoField', 'BigAutoField'
-            ]
+            f
+            for f in cls._meta.fields
+            if f.unique
+            and f.__class__.__name__ not in ["AutoField", "BigAutoField"]
         ]
         if unique:
-            return (unique[0].name, )
+            return (unique[0].name,)
 
         raise Exception("Add a UniqueConstraint to use natural-keys")
 
     @classmethod
     def get_natural_key_fields(cls):
         """
         Determine actual natural key field list, incorporating the natural keys
@@ -202,58 +212,66 @@
         """
         natural_key = []
         for name, rel_to in cls.get_natural_key_info():
             if not rel_to:
                 natural_key.append(name)
             else:
                 nested_key = rel_to.get_natural_key_fields()
-                natural_key.extend([
-                    name + '__' + nname
-                    for nname in nested_key
-                ])
-        return natural_key
+                natural_key.extend(
+                    [name + "__" + nname for nname in nested_key]
+                )
+        return tuple(natural_key)
 
     def natural_key(self):
         """
         Return the natural key for this object.
 
         (This is a generic implementation of the standard Django function)
         """
+        return tuple(
+            self.get_natural_key_value(field)
+            for field in self.get_natural_key_fields()
+        )
+
+    def get_natural_key_value(self, field):
         # Recursively extract properties from related objects if needed
-        vals = [reduce(getattr, name.split('__'), self)
-                for name in self.get_natural_key_fields()]
-        return vals
+        obj = self
+        for part in field.split("__"):
+            obj = getattr(obj, part)
+            if obj is None:
+                return None
+        return obj
 
-    natural_key_separator = '-'
+    natural_key_separator = "-"
 
     @property
     def natural_key_slug(self):
         return self.natural_key_separator.join(
             str(slug) for slug in self.natural_key()
         )
 
     class Meta:
         abstract = True
 
 
-def extract_nested_key(key, cls, prefix=''):
+def extract_nested_key(key, cls, prefix=""):
     nested_key = cls.get_natural_key_fields()
     local_fields = {field.name: field for field in cls._meta.local_fields}
     values = []
     has_val = False
     if prefix:
-        prefix += '__'
+        prefix += "__"
     for nname in nested_key:
         val = key.pop(prefix + nname, None)
         if val is None and nname in local_fields:
-            if type(local_fields[nname]).__name__ == 'DateTimeField':
-                date = key.pop(nname + '_date', None)
-                time = key.pop(nname + '_time', None)
+            if type(local_fields[nname]).__name__ == "DateTimeField":
+                date = key.pop(nname + "_date", None)
+                time = key.pop(nname + "_time", None)
                 if date and time:
-                    val = '%s %s' % (date, time)
+                    val = "%s %s" % (date, time)
 
         if val is not None:
             has_val = True
         values.append(val)
     if has_val:
         return values
     else:
```

### Comparing `natural-keys-2.0.0/natural_keys/serializers.py` & `natural-keys-2.1.0/natural_keys/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from html_json_forms.serializers import JSONFormModelSerializer
 from .models import NaturalKeyModel
 from collections import OrderedDict
 
 
 class NaturalKeyValidator(serializers.UniqueTogetherValidator):
     def set_context(self, serializer):
-        if getattr(self, 'requires_context', None):
+        if getattr(self, "requires_context", None):
             # DRF 3.11+
             pass
         else:
             # DRF 3.10 and older
             self.serializer = serializer
             super(NaturalKeyValidator, self).set_context(serializer)
 
@@ -26,27 +26,25 @@
             for name in self.fields
             if isinstance(serializer.fields[name], NaturalKeySerializer)
         }
 
         attrs = attrs.copy()
         for field in attrs:
             if field in nested_fields:
-                assert(isinstance(attrs[field], dict))
+                assert isinstance(attrs[field], dict)
                 cls = nested_fields[field].Meta.model
-                result = cls._default_manager.filter(
-                    **attrs[field]
-                )
+                result = cls._default_manager.filter(**attrs[field])
                 if result.count() == 0:
                     # No existing nested object for these values
                     return queryset.none()
                 else:
                     # Existing nested object, use it to validate
                     attrs[field] = result[0].pk
 
-        if getattr(self, 'requires_context', None):
+        if getattr(self, "requires_context", None):
             # DRF 3.11+
             return super(NaturalKeyValidator, self).filter_queryset(
                 attrs, queryset, serializer
             )
         else:
             # DRF 3.10 and older
             return super(NaturalKeyValidator, self).filter_queryset(
@@ -54,23 +52,24 @@
             )
 
 
 class NaturalKeySerializer(JSONFormModelSerializer):
     """
     Self-nesting Serializer for NaturalKeyModels
     """
+
     def build_standard_field(self, field_name, model_field):
         field_class, field_kwargs = super(
             NaturalKeySerializer, self
         ).build_standard_field(field_name, model_field)
 
-        if 'validators' in field_kwargs:
-            field_kwargs['validators'] = [
+        if "validators" in field_kwargs:
+            field_kwargs["validators"] = [
                 validator
-                for validator in field_kwargs.get('validators', [])
+                for validator in field_kwargs.get("validators", [])
                 if not isinstance(validator, UniqueValidator)
             ]
         return field_class, field_kwargs
 
     def build_nested_field(self, field_name, relation_info, nested_depth):
         field_class = NaturalKeySerializer.for_model(
             relation_info.related_model,
@@ -81,15 +80,15 @@
 
     def create(self, validated_data):
         model_class = self.Meta.model
         natural_key_fields = model_class.get_natural_key_fields()
         natural_key = []
         for field in natural_key_fields:
             val = validated_data
-            for key in field.split('__'):
+            for key in field.split("__"):
                 val = val[key]
             natural_key.append(val)
         return model_class.objects.find(*natural_key)
 
     def update(self, instance, validated_data):
         raise NotImplementedError(
             "Updating an existing natural key is not supported."
@@ -98,16 +97,19 @@
     @classmethod
     def for_model(cls, model_class, validate_key=True, include_fields=None):
         unique_together = model_class.get_natural_key_def()
         if include_fields and list(include_fields) != list(unique_together):
             raise NotImplementedError(
                 "NaturalKeySerializer for '%s' has unique_together = [%s], "
                 "but provided include_fields = [%s]"
-                % (model_class._meta.model_name, ', '.join(unique_together),
-                   ', '.join(include_fields))
+                % (
+                    model_class._meta.model_name,
+                    ", ".join(unique_together),
+                    ", ".join(include_fields),
+                )
             )
 
         class Serializer(cls):
             class Meta(cls.Meta):
                 model = model_class
                 fields = unique_together
                 if validate_key:
@@ -115,83 +117,82 @@
                         NaturalKeyValidator(
                             queryset=model_class._default_manager,
                             fields=unique_together,
                         )
                     ]
                 else:
                     validators = []
+
         return Serializer
 
     @classmethod
     def for_depth(cls, model_class):
         return cls
 
     class Meta:
         depth = 1
 
 
 class NaturalKeyModelSerializer(JSONFormModelSerializer):
     """
     Serializer for models with one or more foreign keys to a NaturalKeyModel
     """
+
+    def is_natural_key_model(self, related_model):
+        return issubclass(related_model, NaturalKeyModel)
+
     def build_nested_field(self, field_name, relation_info, nested_depth):
-        if issubclass(relation_info.related_model, NaturalKeyModel):
+        if self.is_natural_key_model(relation_info.related_model):
             field_class = NaturalKeySerializer.for_model(
                 relation_info.related_model,
                 validate_key=False,
             )
             field_kwargs = {}
             if relation_info.model_field.null:
-                field_kwargs['required'] = False
+                field_kwargs["required"] = False
             return field_class, field_kwargs
 
         return super(NaturalKeyModelSerializer, self).build_nested_field(
             field_name, relation_info, nested_depth
         )
 
     def build_relational_field(self, field_name, relation_info):
         field_class, field_kwargs = super(
             NaturalKeyModelSerializer, self
-        ).build_relational_field(
-            field_name, relation_info
-        )
-        if issubclass(relation_info.related_model, NaturalKeyModel):
-            field_kwargs.pop('queryset')
-            field_kwargs['read_only'] = True
+        ).build_relational_field(field_name, relation_info)
+        if self.is_natural_key_model(relation_info.related_model):
+            field_kwargs.pop("queryset")
+            field_kwargs["read_only"] = True
         return field_class, field_kwargs
 
     def get_fields(self):
         fields = super(NaturalKeyModelSerializer, self).get_fields()
         fields.update(self.build_natural_key_fields())
         return fields
 
     def build_natural_key_fields(self):
         info = model_meta.get_field_info(self.Meta.model)
         fields = OrderedDict()
         for field, relation_info in info.relations.items():
-            if not issubclass(relation_info.related_model, NaturalKeyModel):
+            if relation_info.reverse:
+                continue
+            if not self.is_natural_key_model(relation_info.related_model):
                 continue
             field_class, field_kwargs = self.build_nested_field(
                 field, relation_info, 1
             )
             fields[field] = field_class(**field_kwargs)
         return fields
 
     def create(self, validated_data):
-        self.convert_natural_keys(
-            validated_data
-        )
-        return super(NaturalKeyModelSerializer, self).create(
-            validated_data
-        )
+        self.convert_natural_keys(validated_data)
+        return super(NaturalKeyModelSerializer, self).create(validated_data)
 
     def update(self, instance, validated_data):
-        self.convert_natural_keys(
-            validated_data
-        )
+        self.convert_natural_keys(validated_data)
         return super(NaturalKeyModelSerializer, self).update(
             instance, validated_data
         )
 
     def convert_natural_keys(self, validated_data):
         fields = self.get_fields()
         for name, field in fields.items():
@@ -206,11 +207,12 @@
     def for_model(cls, model_class, include_fields=None):
         # c.f. wq.db.rest.serializers.ModelSerializer
         class Serializer(cls):
             class Meta(cls.Meta):
                 model = model_class
                 if include_fields:
                     fields = include_fields
+
         return Serializer
 
     class Meta:
         pass
```

### Comparing `natural-keys-2.0.0/.github/workflows/test.yml` & `natural-keys-2.1.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 name: Tests
 
 on: [push, pull_request]
 
 jobs:
   build:
     name: py=${{ matrix.python-version }} dj=${{ matrix.django-version }} drf=${{ matrix.drf-version }}
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     strategy:
       matrix:
-        python-version: [3.9]
-        django-version: [2.2.24, 3.1.13, 3.2.6]
-        drf-version: [3.12.4]
+        python-version: ["3.11"]
+        django-version: [3.2.19, 4.1.9, 4.2.2]
+        drf-version: [3.14.0]
         include:
-        - python-version: 3.9
-          django-version: 3.2.6
+        - python-version: "3.11"
+          django-version: "4.2.2"
           drf-version: none
+        - python-version: "3.10"
+          django-version: 4.2.2
+          drf-version: 3.14.0
+        - python-version: 3.9
+          django-version: 4.2.2
+          drf-version: 3.14.0
         - python-version: 3.8
-          django-version: 3.2.6
-          drf-version: 3.12.4
+          django-version: 4.2.2
+          drf-version: 3.14.0
         - python-version: 3.7
-          django-version: 3.2.6
-          drf-version: 3.12.4
-        - python-version: 3.6
-          django-version: 3.2.6
-          drf-version: 3.12.4
+          django-version: 3.2.19
+          drf-version: 3.14.0
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
+        python -m pip install build
         python -m pip install flake8 pytest wheel
         python -m pip install html-json-forms
         python -m pip install django==${{ matrix.django-version }}
     - name: Install Django REST Framework
       if: ${{ matrix.drf-version != 'none' }}
       run: |
         python -m pip install djangorestframework==${{ matrix.drf-version }}
@@ -44,7 +48,9 @@
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 natural_keys --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 natural_keys --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
     - name: Test with unittest
       run: python -m unittest discover -s tests -t . -v
+    - name: Test build
+      run: python -m build
```

### Comparing `natural-keys-2.0.0/natural_keys.egg-info/PKG-INFO` & `natural-keys-2.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,285 +1,291 @@
 Metadata-Version: 2.1
 Name: natural-keys
-Version: 2.0.0
-Summary: Enhanced support for natural keys in Django and Django REST Framework
-Home-page: https://github.com/wq/django-natural-keys
-Author: S. Andrew Sheppard
-Author-email: andrew@wq.io
+Version: 2.1.0
+Summary: Enhanced support for natural keys in Django and Django REST Framework.
+Author-email: "S. Andrew Sheppard" <andrew@wq.io>
 License: MIT
-Description: # Django Natural Keys
-        
-        Enhanced support for [natural keys] in Django and [Django REST Framework].  Extracted from [wq.db] for general use.
-        
-        *Django Natural Keys* provides a number of useful model methods (e.g. `get_or_create_by_natural_key()`) that speed up working with natural keys in Django.  The module also provides a couple of serializer classes that streamline creating REST API support for models with natural keys.
-        
-        [![Latest PyPI Release](https://img.shields.io/pypi/v/natural-keys.svg)](https://pypi.org/project/natural-keys/)
-        [![Release Notes](https://img.shields.io/github/release/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/releases)
-        [![License](https://img.shields.io/pypi/l/natural-keys.svg)](https://github.com/wq/django-natural-keys/blob/main/LICENSE)
-        [![GitHub Stars](https://img.shields.io/github/stars/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/stargazers)
-        [![GitHub Forks](https://img.shields.io/github/forks/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/network)
-        [![GitHub Issues](https://img.shields.io/github/issues/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/issues)
-        
-        [![Tests](https://github.com/wq/django-natural-keys/actions/workflows/test.yml/badge.svg)](https://github.com/wq/django-natural-keys/actions/workflows/test.yml)
-        [![Python Support](https://img.shields.io/pypi/pyversions/natural-keys.svg)](https://pypi.org/project/natural-keys/)
-        [![Django Support](https://img.shields.io/pypi/djversions/natural-keys.svg)](https://pypi.org/project/natural-keys/)
-        
-        
-        ## Usage
-        
-        *Django Natural Keys* is available via PyPI:
-        
-        ```bash
-        # Recommended: create virtual environment
-        # python3 -m venv venv
-        # . venv/bin/activate
-        pip install natural-keys
-        ```
-        
-        ### Model API
-        
-        To use [natural keys] in vanilla Django, you need to define a `natural_key()` method on your Model class and a `get_natural_key()` method on the Manager class.  With *Django Natural Keys*, you can instead extend `NaturalKeyModel` and define one of the following:
-        
-         * A [`UniqueConstraint`][UniqueConstraint] in `Meta.constraints` (recommended),
-         * A tuple in [`Meta.unique_together`][unique_together], or
-         * A [model field][unique] (other than `AutoField`) with `unique=True`
-        
-        The first unique constraint found will be treated as the natural key for the model, and all of the necessary functions for working with natural keys will automatically work.
-        
-        ```python
-        from natural_keys import NaturalKeyModel
-        
-        class Event(NaturalKeyModel):
-            name = models.CharField(max_length=255)
-            date = models.DateField()
-            class Meta:
-                constraints = [
-                    models.UniqueConstraint(
-                        fields=('name', 'date'),
-                        name='event_natural_key',
-                    )
-                ]
-                
-        class Note(models.Model):
-            event = models.ForeignKey(Event)
-            note = models.TextField()
-        ```
-        or
-        ```python
-        from natural_keys import NaturalKeyModel
-        
-        class Event(NaturalKeyModel):
-            name = models.CharField(unique=True)
-        ```
-        
-        The following methods will then be available on your Model and its Manager:
-        
-        ```python
-        # Default Django methods
-        instance = Event.objects.get_by_natural_key('ABC123', date(2016, 1, 1))
-        instance.natural_key == ('ABC123', date(2016, 1, 1))
-        
-        # get_or_create + natural keys
-        instance, is_new = Event.objects.get_or_create_by_natural_key('ABC123', date(2016, 1, 1))
-        
-        # Like get_or_create_by_natural_key, but discards is_new
-        # Useful for quick lookup/creation when you don't care whether the object exists already
-        instance = Event.objects.find('ABC123', date(2016, 1, 1))
-        note = Note.objects.create(
-             event=Event.objects.find('ABC123', date(2016, 1, 1)),
-             note="This is a note"
-        )
-        instance == note.event
-        
-        # Inspect natural key fields on a model without instantiating it
-        Event.get_natural_key_fields() == ('name', 'date')
-        ```
-        
-        #### Nested Natural Keys
-        One key feature of *Django Natural Keys* is that it will automatically traverse `ForeignKey`s to related models (which should also be `NaturalKeyModel` classes).  This makes it possible to define complex, arbitrarily nested natural keys with minimal effort.
-        
-        ```python
-        class Place(NaturalKeyModel):
-            name = models.CharField(max_length=255, unique=True)
-        
-        class Event(NaturalKeyModel):
-            place = models.ForeignKey(Place)
-            date = models.DateField()
-            class Meta:
-                constraints = [
-                    models.UniqueConstraint(
-                        fields=('place', 'date'),
-                        name='event_natural_key',
-                    )
-                ]
-        ```
-        
-        ```python
-        Event.get_natural_key_fields() == ('place__name', 'date')
-        instance = Event.find('ABC123', date(2016, 1, 1))
-        instance.place.name == 'ABC123'
-        ```
-        
-        ### REST Framework Support
-        *Django Natural Keys* provides several integrations with [Django REST Framework], primarily through custom Serializer classes.  In most cases, you will want to use either:
-         * `NaturalKeyModelSerializer`, or
-         * The `natural_key_slug` pseudo-field (see below)
-        
-        If you have only a single model with a single char field for its natural key, you probably do not need to use either of these integrations.  In your view, you can just use Django REST Framework's built in `lookup_field` to point directly to your natural key.
-        
-        #### `NaturalKeyModelSerializer`
-        `NaturalKeyModelSerializer` facilitates handling complex natural keys in your rest API.  It can be used with a `NaturalKeyModel`, or (more commonly) a model that has a foreign key to a `NaturalKeyModel` but is not a `NaturalKeyModel` itself.  (One concrete example of this is the [vera.Report] model, which has a ForeignKey to [vera.Event], which is a `NaturalKeyModel`).
-        
-        `NaturalKeyModelSerializer` extends DRF's [ModelSerializer], but uses `NaturalKeySerializer` for each foreign key that points to a `NaturalKeyModel`.  When `update()` or `create()`ing the primary model, the nested `NaturalKeySerializer`s will automatically create instances of referenced models if they do not exist already (via the `find()` method described above).  Note that `NaturalKeyModelSerializer` does not override DRF's default behavior for other fields, whether or not they form part of the primary model's natural key.
-        
-        `NaturalKeySerializer` can technically be used as a top level serializer, though this is not recommended.  `NaturalKeySerializer` is designed for dealing with nested natural keys and does not support updates or non-natural key fields.  Even when used together with `NaturalKeyModelSerializer`, `NaturalKeySerializer` never updates an existing related model instance.  Instead, it will repoint the foreign key to another (potentially new) instance of the related model.  It may help to think of `NaturalKeySerializer` as a special [RelatedField] class rather than as a `Serializer` per se.
-        
-        
-        You can use `NaturalKeyModelSerializer` with [Django REST Framework] and/or [wq.db] just like any other serializer:
-        ```python
-        # Django REST Framework usage example
-        from rest_framework import viewsets
-        from rest_framework import routers
-        from natural_keys import NaturalKeyModelSerializer
-        from .models import Event, Note
-        
-        class EventSerializer(NaturalKeyModelSerializer):
-            class Meta:
-                model = Event
-                
-        class NoteSerializer(NaturalKeyModelSerializer):
-            class Meta:
-                model = Note
-        
-        class EventViewSet(viewsets.ModelViewSet):
-            queryset = Event.objects.all()
-            serializer_class = EventSerializer
-        
-        class NoteViewSet(viewsets.ModelViewSet):
-            queryset = Note.objects.all()
-            serializer_class = NoteSerializer
-        
-        router = routers.DefaultRouter()
-        router.register(r'events', EventViewSet)
-        router.register(r'notes', NoteViewSet)
-        
-        # wq.db usage example
-        from wq.db import rest
-        from natural_keys import NaturalKeyModelSerializer
-        from .models import Event, Note
-        
-        rest.router.register_model(Note, serializer=NaturalKeyModelSerializer)
-        rest.router.register_model(Event, serializer=NaturalKeyModelSerializer)
-        ```
-        
-        Once this is set up, you can use your REST API to create and view your `NaturalKeyModel` instances and related data.  To facilitate integration with regular HTML Forms, *Django Natural Keys* is integrated with the [HTML JSON Forms] package, which supports nested keys via an array naming convention, as the examples below demonstrate.
-        
-        ```html
-        <form action="/events/" method="post">
-          <input name="place[name]">
-          <input type="date" name="date">
-        </form>
-        ```
-        ```js
-        // /events.json
-        [
-            {
-                "id": 123,
-                "place": {"name": "ABC123"},
-                "date": "2016-01-01"
-            }
-        ]
-        ```
-        ```html
-        <form action="/notes/" method="post">
-          <input name="event[place][name]">
-          <input type="date" name="event[date]">
-          <textarea name="note"></textarea>
-        </form>
-        ```
-        ```js
-        // /notes.json
-        [
-            {
-                "id": 12345,
-                "event": {
-                    "place": {"name": "ABC123"},
-                    "date": "2016-01-01"
-                },
-                "note": "This is a note"
-            }
-        ]
-        ```
-        
-        ### Natural Key Slugs
-        As an alternative to using `NaturalKeyModelSerializer` / `NaturalKeySerializer`, you can also use a single slug-like field for lookup and serialization.  `NaturalKeyModel` (and its associated queryset) defines a pseudo-field, `natural_key_slug`, for this purpose.
-        
-        ```python
-        class Place(NaturalKeyModel):
-            name = models.CharField(max_length=255, unique=True)
-            
-        class Room(NaturalKeyModel)
-            place = models.ForeignKey(Place, models.ON_DELETE)
-            name = models.CharField(max_length=255)
-            
-            class Meta:
-                unique_together = (('place', 'name'),)
-        ```
-        ```python
-        room = Room.objects.find("ABC123", "MainHall")
-        assert(room.natural_key_slug == "ABC123-MainHall")
-        assert(room == Room.objects.get(natural_key_slug="ABC123-MainHall"))
-        ```
-        
-        You can expose this functionality in your REST API to expose natural keys instead of database-generated ids.  To do this, you will likely want to do the following:
-        
-         1. Create a regular serializer with `id = serializers.ReadOnlyField(source='natural_key_slug')`
-         2. Set `lookup_field = 'natural_key_slug'` on your `ModelViewSet` (or similar generic class) and update the URL registration accordingly
-         3. Ensure foreign keys on any related models are serialized with `serializers.SlugRelatedField(slug_field='natural_key_slug')`
-        
-        In [wq.db], all three of the above can be achieved by setting the `"lookup"` attribute when registering with the [router]:
-        
-        ```python
-        # myapp/rest.py
-        from wq.db import rest
-        from .models import Room
-        
-        rest.router.register_model(
-            Room,
-            fields='__all__',
-            lookup='natural_key_slug',
-        )
-        ```
-        
-        Note that the `natural_key_slug` may not behave as expected if any of the component values contain the delimiter character (`-` by default).  To mitigate this, you can set `natural_key_separator` on the model class to another character.
-        
-        [natural keys]: https://docs.djangoproject.com/en/3.2/topics/serialization/#natural-keys
-        [UniqueConstraint]: https://docs.djangoproject.com/en/3.2/ref/models/constraints/#uniqueconstraint
-        [unique_together]: https://docs.djangoproject.com/en/3.2/ref/models/options/#unique-together
-        [unique]: https://docs.djangoproject.com/en/3.2/ref/models/fields/#unique
-        
-        [wq.db]: https://wq.io/wq.db/
-        [Django REST Framework]: http://www.django-rest-framework.org/
-        [vera.Report]:https://github.com/powered-by-wq/vera#report
-        [vera.Event]: https://github.com/powered-by-wq/vera#event
-        [ModelSerializer]: https://www.django-rest-framework.org/api-guide/serializers/#modelserializer
-        [RelatedField]: https://www.django-rest-framework.org/api-guide/relations/
-        [HTML JSON Forms]: https://github.com/wq/html-json-forms
-        [router]: https://wq.io/wq.db/router
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/wq/django-natural-keys
+Project-URL: Documentation, https://wq.io/
+Project-URL: Source, https://github.com/wq/django-natural-keys
+Project-URL: Release Notes, https://github.com/wq/django-natural-keys/releases
+Project-URL: Issues, https://github.com/wq/django-natural-keys/issues
+Project-URL: CI, https://github.com/wq/django-natural-keys/actions/workflows/test.yml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Database
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django Natural Keys
+
+Enhanced support for [natural keys] in Django and [Django REST Framework].  Extracted from [wq.db] for general use.
+
+*Django Natural Keys* provides a number of useful model methods (e.g. `get_or_create_by_natural_key()`) that speed up working with natural keys in Django.  The module also provides a couple of serializer classes that streamline creating REST API support for models with natural keys.
+
+[![Latest PyPI Release](https://img.shields.io/pypi/v/natural-keys.svg)](https://pypi.org/project/natural-keys/)
+[![Release Notes](https://img.shields.io/github/release/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/releases)
+[![License](https://img.shields.io/pypi/l/natural-keys.svg)](https://github.com/wq/django-natural-keys/blob/main/LICENSE)
+[![GitHub Stars](https://img.shields.io/github/stars/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/stargazers)
+[![GitHub Forks](https://img.shields.io/github/forks/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/network)
+[![GitHub Issues](https://img.shields.io/github/issues/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/issues)
+
+[![Tests](https://github.com/wq/django-natural-keys/actions/workflows/test.yml/badge.svg)](https://github.com/wq/django-natural-keys/actions/workflows/test.yml)
+[![Python Support](https://img.shields.io/pypi/pyversions/natural-keys.svg)](https://pypi.org/project/natural-keys/)
+[![Django Support](https://img.shields.io/pypi/djversions/natural-keys.svg)](https://pypi.org/project/natural-keys/)
+
+
+## Usage
+
+*Django Natural Keys* is available via PyPI:
+
+```bash
+# Recommended: create virtual environment
+# python3 -m venv venv
+# . venv/bin/activate
+pip install natural-keys
+```
+
+### Model API
+
+To use [natural keys] in vanilla Django, you need to define a `natural_key()` method on your Model class and a `get_natural_key()` method on the Manager class.  With *Django Natural Keys*, you can instead extend `NaturalKeyModel` and define one of the following:
+
+ * A [`UniqueConstraint`][UniqueConstraint] in `Meta.constraints` (recommended),
+ * A tuple in [`Meta.unique_together`][unique_together], or
+ * A [model field][unique] (other than `AutoField`) with `unique=True`
+
+The first unique constraint found will be treated as the natural key for the model, and all of the necessary functions for working with natural keys will automatically work.
+
+```python
+from natural_keys import NaturalKeyModel
+
+class Event(NaturalKeyModel):
+    name = models.CharField(max_length=255)
+    date = models.DateField()
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(
+                fields=('name', 'date'),
+                name='event_natural_key',
+            )
+        ]
+        
+class Note(models.Model):
+    event = models.ForeignKey(Event)
+    note = models.TextField()
+```
+or
+```python
+from natural_keys import NaturalKeyModel
+
+class Event(NaturalKeyModel):
+    name = models.CharField(unique=True)
+```
+
+The following methods will then be available on your Model and its Manager:
+
+```python
+# Default Django methods
+instance = Event.objects.get_by_natural_key('ABC123', date(2016, 1, 1))
+instance.natural_key == ('ABC123', date(2016, 1, 1))
+
+# get_or_create + natural keys
+instance, is_new = Event.objects.get_or_create_by_natural_key('ABC123', date(2016, 1, 1))
+
+# Like get_or_create_by_natural_key, but discards is_new
+# Useful for quick lookup/creation when you don't care whether the object exists already
+instance = Event.objects.find('ABC123', date(2016, 1, 1))
+note = Note.objects.create(
+     event=Event.objects.find('ABC123', date(2016, 1, 1)),
+     note="This is a note"
+)
+instance == note.event
+
+# Inspect natural key fields on a model without instantiating it
+Event.get_natural_key_fields() == ('name', 'date')
+```
+
+#### Nested Natural Keys
+One key feature of *Django Natural Keys* is that it will automatically traverse `ForeignKey`s to related models (which should also be `NaturalKeyModel` classes).  This makes it possible to define complex, arbitrarily nested natural keys with minimal effort.
+
+```python
+class Place(NaturalKeyModel):
+    name = models.CharField(max_length=255, unique=True)
+
+class Event(NaturalKeyModel):
+    place = models.ForeignKey(Place)
+    date = models.DateField()
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(
+                fields=('place', 'date'),
+                name='event_natural_key',
+            )
+        ]
+```
+
+```python
+Event.get_natural_key_fields() == ('place__name', 'date')
+instance = Event.find('ABC123', date(2016, 1, 1))
+instance.place.name == 'ABC123'
+```
+
+### REST Framework Support
+*Django Natural Keys* provides several integrations with [Django REST Framework], primarily through custom Serializer classes.  In most cases, you will want to use either:
+ * `NaturalKeyModelSerializer`, or
+ * The `natural_key_slug` pseudo-field (see below)
+
+If you have only a single model with a single char field for its natural key, you probably do not need to use either of these integrations.  In your view, you can just use Django REST Framework's built in `lookup_field` to point directly to your natural key.
+
+#### `NaturalKeyModelSerializer`
+`NaturalKeyModelSerializer` facilitates handling complex natural keys in your rest API.  It can be used with a `NaturalKeyModel`, or (more commonly) a model that has a foreign key to a `NaturalKeyModel` but is not a `NaturalKeyModel` itself.  (One concrete example of this is the [vera.Report] model, which has a ForeignKey to [vera.Event], which is a `NaturalKeyModel`).
+
+`NaturalKeyModelSerializer` extends DRF's [ModelSerializer], but uses `NaturalKeySerializer` for each foreign key that points to a `NaturalKeyModel`.  When `update()` or `create()`ing the primary model, the nested `NaturalKeySerializer`s will automatically create instances of referenced models if they do not exist already (via the `find()` method described above).  Note that `NaturalKeyModelSerializer` does not override DRF's default behavior for other fields, whether or not they form part of the primary model's natural key.
+
+`NaturalKeySerializer` can technically be used as a top level serializer, though this is not recommended.  `NaturalKeySerializer` is designed for dealing with nested natural keys and does not support updates or non-natural key fields.  Even when used together with `NaturalKeyModelSerializer`, `NaturalKeySerializer` never updates an existing related model instance.  Instead, it will repoint the foreign key to another (potentially new) instance of the related model.  It may help to think of `NaturalKeySerializer` as a special [RelatedField] class rather than as a `Serializer` per se.
+
+
+You can use `NaturalKeyModelSerializer` with [Django REST Framework] and/or [wq.db] just like any other serializer:
+```python
+# Django REST Framework usage example
+from rest_framework import viewsets
+from rest_framework import routers
+from natural_keys import NaturalKeyModelSerializer
+from .models import Event, Note
+
+class EventSerializer(NaturalKeyModelSerializer):
+    class Meta:
+        model = Event
+        
+class NoteSerializer(NaturalKeyModelSerializer):
+    class Meta:
+        model = Note
+
+class EventViewSet(viewsets.ModelViewSet):
+    queryset = Event.objects.all()
+    serializer_class = EventSerializer
+
+class NoteViewSet(viewsets.ModelViewSet):
+    queryset = Note.objects.all()
+    serializer_class = NoteSerializer
+
+router = routers.DefaultRouter()
+router.register(r'events', EventViewSet)
+router.register(r'notes', NoteViewSet)
+
+# wq.db usage example
+from wq.db import rest
+from natural_keys import NaturalKeyModelSerializer
+from .models import Event, Note
+
+rest.router.register_model(Note, serializer=NaturalKeyModelSerializer)
+rest.router.register_model(Event, serializer=NaturalKeyModelSerializer)
+```
+
+Once this is set up, you can use your REST API to create and view your `NaturalKeyModel` instances and related data.  To facilitate integration with regular HTML Forms, *Django Natural Keys* is integrated with the [HTML JSON Forms] package, which supports nested keys via an array naming convention, as the examples below demonstrate.
+
+```html
+<form action="/events/" method="post">
+  <input name="place[name]">
+  <input type="date" name="date">
+</form>
+```
+```js
+// /events.json
+[
+    {
+        "id": 123,
+        "place": {"name": "ABC123"},
+        "date": "2016-01-01"
+    }
+]
+```
+```html
+<form action="/notes/" method="post">
+  <input name="event[place][name]">
+  <input type="date" name="event[date]">
+  <textarea name="note"></textarea>
+</form>
+```
+```js
+// /notes.json
+[
+    {
+        "id": 12345,
+        "event": {
+            "place": {"name": "ABC123"},
+            "date": "2016-01-01"
+        },
+        "note": "This is a note"
+    }
+]
+```
+
+### Natural Key Slugs
+As an alternative to using `NaturalKeyModelSerializer` / `NaturalKeySerializer`, you can also use a single slug-like field for lookup and serialization.  `NaturalKeyModel` (and its associated queryset) defines a pseudo-field, `natural_key_slug`, for this purpose.
+
+```python
+class Place(NaturalKeyModel):
+    name = models.CharField(max_length=255, unique=True)
+    
+class Room(NaturalKeyModel)
+    place = models.ForeignKey(Place, models.ON_DELETE)
+    name = models.CharField(max_length=255)
+    
+    class Meta:
+        unique_together = (('place', 'name'),)
+```
+```python
+room = Room.objects.find("ABC123", "MainHall")
+assert(room.natural_key_slug == "ABC123-MainHall")
+assert(room == Room.objects.get(natural_key_slug="ABC123-MainHall"))
+```
+
+You can expose this functionality in your REST API to expose natural keys instead of database-generated ids.  To do this, you will likely want to do the following:
+
+ 1. Create a regular serializer with `id = serializers.ReadOnlyField(source='natural_key_slug')`
+ 2. Set `lookup_field = 'natural_key_slug'` on your `ModelViewSet` (or similar generic class) and update the URL registration accordingly
+ 3. Ensure foreign keys on any related models are serialized with `serializers.SlugRelatedField(slug_field='natural_key_slug')`
+
+In [wq.db], all three of the above can be achieved by setting the `"lookup"` attribute when registering with the [router]:
+
+```python
+# myapp/rest.py
+from wq.db import rest
+from .models import Room
+
+rest.router.register_model(
+    Room,
+    fields='__all__',
+    lookup='natural_key_slug',
+)
+```
+
+Note that the `natural_key_slug` may not behave as expected if any of the component values contain the delimiter character (`-` by default).  To mitigate this, you can set `natural_key_separator` on the model class to another character.
+
+[natural keys]: https://docs.djangoproject.com/en/4.2/topics/serialization/#natural-keys
+[UniqueConstraint]: https://docs.djangoproject.com/en/4.2/ref/models/constraints/#uniqueconstraint
+[unique_together]: https://docs.djangoproject.com/en/4.2/ref/models/options/#unique-together
+[unique]: https://docs.djangoproject.com/en/4.2/ref/models/fields/#unique
+
+[wq.db]: https://wq.io/wq.db/
+[Django REST Framework]: http://www.django-rest-framework.org/
+[vera.Report]:https://github.com/powered-by-wq/vera#report
+[vera.Event]: https://github.com/powered-by-wq/vera#event
+[ModelSerializer]: https://www.django-rest-framework.org/api-guide/serializers/#modelserializer
+[RelatedField]: https://www.django-rest-framework.org/api-guide/relations/
+[HTML JSON Forms]: https://github.com/wq/html-json-forms
+[router]: https://wq.io/wq.db/router
```

### Comparing `natural-keys-2.0.0/PKG-INFO` & `natural-keys-2.1.0/natural_keys.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,285 +1,291 @@
 Metadata-Version: 2.1
 Name: natural-keys
-Version: 2.0.0
-Summary: Enhanced support for natural keys in Django and Django REST Framework
-Home-page: https://github.com/wq/django-natural-keys
-Author: S. Andrew Sheppard
-Author-email: andrew@wq.io
+Version: 2.1.0
+Summary: Enhanced support for natural keys in Django and Django REST Framework.
+Author-email: "S. Andrew Sheppard" <andrew@wq.io>
 License: MIT
-Description: # Django Natural Keys
-        
-        Enhanced support for [natural keys] in Django and [Django REST Framework].  Extracted from [wq.db] for general use.
-        
-        *Django Natural Keys* provides a number of useful model methods (e.g. `get_or_create_by_natural_key()`) that speed up working with natural keys in Django.  The module also provides a couple of serializer classes that streamline creating REST API support for models with natural keys.
-        
-        [![Latest PyPI Release](https://img.shields.io/pypi/v/natural-keys.svg)](https://pypi.org/project/natural-keys/)
-        [![Release Notes](https://img.shields.io/github/release/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/releases)
-        [![License](https://img.shields.io/pypi/l/natural-keys.svg)](https://github.com/wq/django-natural-keys/blob/main/LICENSE)
-        [![GitHub Stars](https://img.shields.io/github/stars/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/stargazers)
-        [![GitHub Forks](https://img.shields.io/github/forks/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/network)
-        [![GitHub Issues](https://img.shields.io/github/issues/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/issues)
-        
-        [![Tests](https://github.com/wq/django-natural-keys/actions/workflows/test.yml/badge.svg)](https://github.com/wq/django-natural-keys/actions/workflows/test.yml)
-        [![Python Support](https://img.shields.io/pypi/pyversions/natural-keys.svg)](https://pypi.org/project/natural-keys/)
-        [![Django Support](https://img.shields.io/pypi/djversions/natural-keys.svg)](https://pypi.org/project/natural-keys/)
-        
-        
-        ## Usage
-        
-        *Django Natural Keys* is available via PyPI:
-        
-        ```bash
-        # Recommended: create virtual environment
-        # python3 -m venv venv
-        # . venv/bin/activate
-        pip install natural-keys
-        ```
-        
-        ### Model API
-        
-        To use [natural keys] in vanilla Django, you need to define a `natural_key()` method on your Model class and a `get_natural_key()` method on the Manager class.  With *Django Natural Keys*, you can instead extend `NaturalKeyModel` and define one of the following:
-        
-         * A [`UniqueConstraint`][UniqueConstraint] in `Meta.constraints` (recommended),
-         * A tuple in [`Meta.unique_together`][unique_together], or
-         * A [model field][unique] (other than `AutoField`) with `unique=True`
-        
-        The first unique constraint found will be treated as the natural key for the model, and all of the necessary functions for working with natural keys will automatically work.
-        
-        ```python
-        from natural_keys import NaturalKeyModel
-        
-        class Event(NaturalKeyModel):
-            name = models.CharField(max_length=255)
-            date = models.DateField()
-            class Meta:
-                constraints = [
-                    models.UniqueConstraint(
-                        fields=('name', 'date'),
-                        name='event_natural_key',
-                    )
-                ]
-                
-        class Note(models.Model):
-            event = models.ForeignKey(Event)
-            note = models.TextField()
-        ```
-        or
-        ```python
-        from natural_keys import NaturalKeyModel
-        
-        class Event(NaturalKeyModel):
-            name = models.CharField(unique=True)
-        ```
-        
-        The following methods will then be available on your Model and its Manager:
-        
-        ```python
-        # Default Django methods
-        instance = Event.objects.get_by_natural_key('ABC123', date(2016, 1, 1))
-        instance.natural_key == ('ABC123', date(2016, 1, 1))
-        
-        # get_or_create + natural keys
-        instance, is_new = Event.objects.get_or_create_by_natural_key('ABC123', date(2016, 1, 1))
-        
-        # Like get_or_create_by_natural_key, but discards is_new
-        # Useful for quick lookup/creation when you don't care whether the object exists already
-        instance = Event.objects.find('ABC123', date(2016, 1, 1))
-        note = Note.objects.create(
-             event=Event.objects.find('ABC123', date(2016, 1, 1)),
-             note="This is a note"
-        )
-        instance == note.event
-        
-        # Inspect natural key fields on a model without instantiating it
-        Event.get_natural_key_fields() == ('name', 'date')
-        ```
-        
-        #### Nested Natural Keys
-        One key feature of *Django Natural Keys* is that it will automatically traverse `ForeignKey`s to related models (which should also be `NaturalKeyModel` classes).  This makes it possible to define complex, arbitrarily nested natural keys with minimal effort.
-        
-        ```python
-        class Place(NaturalKeyModel):
-            name = models.CharField(max_length=255, unique=True)
-        
-        class Event(NaturalKeyModel):
-            place = models.ForeignKey(Place)
-            date = models.DateField()
-            class Meta:
-                constraints = [
-                    models.UniqueConstraint(
-                        fields=('place', 'date'),
-                        name='event_natural_key',
-                    )
-                ]
-        ```
-        
-        ```python
-        Event.get_natural_key_fields() == ('place__name', 'date')
-        instance = Event.find('ABC123', date(2016, 1, 1))
-        instance.place.name == 'ABC123'
-        ```
-        
-        ### REST Framework Support
-        *Django Natural Keys* provides several integrations with [Django REST Framework], primarily through custom Serializer classes.  In most cases, you will want to use either:
-         * `NaturalKeyModelSerializer`, or
-         * The `natural_key_slug` pseudo-field (see below)
-        
-        If you have only a single model with a single char field for its natural key, you probably do not need to use either of these integrations.  In your view, you can just use Django REST Framework's built in `lookup_field` to point directly to your natural key.
-        
-        #### `NaturalKeyModelSerializer`
-        `NaturalKeyModelSerializer` facilitates handling complex natural keys in your rest API.  It can be used with a `NaturalKeyModel`, or (more commonly) a model that has a foreign key to a `NaturalKeyModel` but is not a `NaturalKeyModel` itself.  (One concrete example of this is the [vera.Report] model, which has a ForeignKey to [vera.Event], which is a `NaturalKeyModel`).
-        
-        `NaturalKeyModelSerializer` extends DRF's [ModelSerializer], but uses `NaturalKeySerializer` for each foreign key that points to a `NaturalKeyModel`.  When `update()` or `create()`ing the primary model, the nested `NaturalKeySerializer`s will automatically create instances of referenced models if they do not exist already (via the `find()` method described above).  Note that `NaturalKeyModelSerializer` does not override DRF's default behavior for other fields, whether or not they form part of the primary model's natural key.
-        
-        `NaturalKeySerializer` can technically be used as a top level serializer, though this is not recommended.  `NaturalKeySerializer` is designed for dealing with nested natural keys and does not support updates or non-natural key fields.  Even when used together with `NaturalKeyModelSerializer`, `NaturalKeySerializer` never updates an existing related model instance.  Instead, it will repoint the foreign key to another (potentially new) instance of the related model.  It may help to think of `NaturalKeySerializer` as a special [RelatedField] class rather than as a `Serializer` per se.
-        
-        
-        You can use `NaturalKeyModelSerializer` with [Django REST Framework] and/or [wq.db] just like any other serializer:
-        ```python
-        # Django REST Framework usage example
-        from rest_framework import viewsets
-        from rest_framework import routers
-        from natural_keys import NaturalKeyModelSerializer
-        from .models import Event, Note
-        
-        class EventSerializer(NaturalKeyModelSerializer):
-            class Meta:
-                model = Event
-                
-        class NoteSerializer(NaturalKeyModelSerializer):
-            class Meta:
-                model = Note
-        
-        class EventViewSet(viewsets.ModelViewSet):
-            queryset = Event.objects.all()
-            serializer_class = EventSerializer
-        
-        class NoteViewSet(viewsets.ModelViewSet):
-            queryset = Note.objects.all()
-            serializer_class = NoteSerializer
-        
-        router = routers.DefaultRouter()
-        router.register(r'events', EventViewSet)
-        router.register(r'notes', NoteViewSet)
-        
-        # wq.db usage example
-        from wq.db import rest
-        from natural_keys import NaturalKeyModelSerializer
-        from .models import Event, Note
-        
-        rest.router.register_model(Note, serializer=NaturalKeyModelSerializer)
-        rest.router.register_model(Event, serializer=NaturalKeyModelSerializer)
-        ```
-        
-        Once this is set up, you can use your REST API to create and view your `NaturalKeyModel` instances and related data.  To facilitate integration with regular HTML Forms, *Django Natural Keys* is integrated with the [HTML JSON Forms] package, which supports nested keys via an array naming convention, as the examples below demonstrate.
-        
-        ```html
-        <form action="/events/" method="post">
-          <input name="place[name]">
-          <input type="date" name="date">
-        </form>
-        ```
-        ```js
-        // /events.json
-        [
-            {
-                "id": 123,
-                "place": {"name": "ABC123"},
-                "date": "2016-01-01"
-            }
-        ]
-        ```
-        ```html
-        <form action="/notes/" method="post">
-          <input name="event[place][name]">
-          <input type="date" name="event[date]">
-          <textarea name="note"></textarea>
-        </form>
-        ```
-        ```js
-        // /notes.json
-        [
-            {
-                "id": 12345,
-                "event": {
-                    "place": {"name": "ABC123"},
-                    "date": "2016-01-01"
-                },
-                "note": "This is a note"
-            }
-        ]
-        ```
-        
-        ### Natural Key Slugs
-        As an alternative to using `NaturalKeyModelSerializer` / `NaturalKeySerializer`, you can also use a single slug-like field for lookup and serialization.  `NaturalKeyModel` (and its associated queryset) defines a pseudo-field, `natural_key_slug`, for this purpose.
-        
-        ```python
-        class Place(NaturalKeyModel):
-            name = models.CharField(max_length=255, unique=True)
-            
-        class Room(NaturalKeyModel)
-            place = models.ForeignKey(Place, models.ON_DELETE)
-            name = models.CharField(max_length=255)
-            
-            class Meta:
-                unique_together = (('place', 'name'),)
-        ```
-        ```python
-        room = Room.objects.find("ABC123", "MainHall")
-        assert(room.natural_key_slug == "ABC123-MainHall")
-        assert(room == Room.objects.get(natural_key_slug="ABC123-MainHall"))
-        ```
-        
-        You can expose this functionality in your REST API to expose natural keys instead of database-generated ids.  To do this, you will likely want to do the following:
-        
-         1. Create a regular serializer with `id = serializers.ReadOnlyField(source='natural_key_slug')`
-         2. Set `lookup_field = 'natural_key_slug'` on your `ModelViewSet` (or similar generic class) and update the URL registration accordingly
-         3. Ensure foreign keys on any related models are serialized with `serializers.SlugRelatedField(slug_field='natural_key_slug')`
-        
-        In [wq.db], all three of the above can be achieved by setting the `"lookup"` attribute when registering with the [router]:
-        
-        ```python
-        # myapp/rest.py
-        from wq.db import rest
-        from .models import Room
-        
-        rest.router.register_model(
-            Room,
-            fields='__all__',
-            lookup='natural_key_slug',
-        )
-        ```
-        
-        Note that the `natural_key_slug` may not behave as expected if any of the component values contain the delimiter character (`-` by default).  To mitigate this, you can set `natural_key_separator` on the model class to another character.
-        
-        [natural keys]: https://docs.djangoproject.com/en/3.2/topics/serialization/#natural-keys
-        [UniqueConstraint]: https://docs.djangoproject.com/en/3.2/ref/models/constraints/#uniqueconstraint
-        [unique_together]: https://docs.djangoproject.com/en/3.2/ref/models/options/#unique-together
-        [unique]: https://docs.djangoproject.com/en/3.2/ref/models/fields/#unique
-        
-        [wq.db]: https://wq.io/wq.db/
-        [Django REST Framework]: http://www.django-rest-framework.org/
-        [vera.Report]:https://github.com/powered-by-wq/vera#report
-        [vera.Event]: https://github.com/powered-by-wq/vera#event
-        [ModelSerializer]: https://www.django-rest-framework.org/api-guide/serializers/#modelserializer
-        [RelatedField]: https://www.django-rest-framework.org/api-guide/relations/
-        [HTML JSON Forms]: https://github.com/wq/html-json-forms
-        [router]: https://wq.io/wq.db/router
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/wq/django-natural-keys
+Project-URL: Documentation, https://wq.io/
+Project-URL: Source, https://github.com/wq/django-natural-keys
+Project-URL: Release Notes, https://github.com/wq/django-natural-keys/releases
+Project-URL: Issues, https://github.com/wq/django-natural-keys/issues
+Project-URL: CI, https://github.com/wq/django-natural-keys/actions/workflows/test.yml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Database
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Django Natural Keys
+
+Enhanced support for [natural keys] in Django and [Django REST Framework].  Extracted from [wq.db] for general use.
+
+*Django Natural Keys* provides a number of useful model methods (e.g. `get_or_create_by_natural_key()`) that speed up working with natural keys in Django.  The module also provides a couple of serializer classes that streamline creating REST API support for models with natural keys.
+
+[![Latest PyPI Release](https://img.shields.io/pypi/v/natural-keys.svg)](https://pypi.org/project/natural-keys/)
+[![Release Notes](https://img.shields.io/github/release/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/releases)
+[![License](https://img.shields.io/pypi/l/natural-keys.svg)](https://github.com/wq/django-natural-keys/blob/main/LICENSE)
+[![GitHub Stars](https://img.shields.io/github/stars/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/stargazers)
+[![GitHub Forks](https://img.shields.io/github/forks/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/network)
+[![GitHub Issues](https://img.shields.io/github/issues/wq/django-natural-keys.svg)](https://github.com/wq/django-natural-keys/issues)
+
+[![Tests](https://github.com/wq/django-natural-keys/actions/workflows/test.yml/badge.svg)](https://github.com/wq/django-natural-keys/actions/workflows/test.yml)
+[![Python Support](https://img.shields.io/pypi/pyversions/natural-keys.svg)](https://pypi.org/project/natural-keys/)
+[![Django Support](https://img.shields.io/pypi/djversions/natural-keys.svg)](https://pypi.org/project/natural-keys/)
+
+
+## Usage
+
+*Django Natural Keys* is available via PyPI:
+
+```bash
+# Recommended: create virtual environment
+# python3 -m venv venv
+# . venv/bin/activate
+pip install natural-keys
+```
+
+### Model API
+
+To use [natural keys] in vanilla Django, you need to define a `natural_key()` method on your Model class and a `get_natural_key()` method on the Manager class.  With *Django Natural Keys*, you can instead extend `NaturalKeyModel` and define one of the following:
+
+ * A [`UniqueConstraint`][UniqueConstraint] in `Meta.constraints` (recommended),
+ * A tuple in [`Meta.unique_together`][unique_together], or
+ * A [model field][unique] (other than `AutoField`) with `unique=True`
+
+The first unique constraint found will be treated as the natural key for the model, and all of the necessary functions for working with natural keys will automatically work.
+
+```python
+from natural_keys import NaturalKeyModel
+
+class Event(NaturalKeyModel):
+    name = models.CharField(max_length=255)
+    date = models.DateField()
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(
+                fields=('name', 'date'),
+                name='event_natural_key',
+            )
+        ]
+        
+class Note(models.Model):
+    event = models.ForeignKey(Event)
+    note = models.TextField()
+```
+or
+```python
+from natural_keys import NaturalKeyModel
+
+class Event(NaturalKeyModel):
+    name = models.CharField(unique=True)
+```
+
+The following methods will then be available on your Model and its Manager:
+
+```python
+# Default Django methods
+instance = Event.objects.get_by_natural_key('ABC123', date(2016, 1, 1))
+instance.natural_key == ('ABC123', date(2016, 1, 1))
+
+# get_or_create + natural keys
+instance, is_new = Event.objects.get_or_create_by_natural_key('ABC123', date(2016, 1, 1))
+
+# Like get_or_create_by_natural_key, but discards is_new
+# Useful for quick lookup/creation when you don't care whether the object exists already
+instance = Event.objects.find('ABC123', date(2016, 1, 1))
+note = Note.objects.create(
+     event=Event.objects.find('ABC123', date(2016, 1, 1)),
+     note="This is a note"
+)
+instance == note.event
+
+# Inspect natural key fields on a model without instantiating it
+Event.get_natural_key_fields() == ('name', 'date')
+```
+
+#### Nested Natural Keys
+One key feature of *Django Natural Keys* is that it will automatically traverse `ForeignKey`s to related models (which should also be `NaturalKeyModel` classes).  This makes it possible to define complex, arbitrarily nested natural keys with minimal effort.
+
+```python
+class Place(NaturalKeyModel):
+    name = models.CharField(max_length=255, unique=True)
+
+class Event(NaturalKeyModel):
+    place = models.ForeignKey(Place)
+    date = models.DateField()
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(
+                fields=('place', 'date'),
+                name='event_natural_key',
+            )
+        ]
+```
+
+```python
+Event.get_natural_key_fields() == ('place__name', 'date')
+instance = Event.find('ABC123', date(2016, 1, 1))
+instance.place.name == 'ABC123'
+```
+
+### REST Framework Support
+*Django Natural Keys* provides several integrations with [Django REST Framework], primarily through custom Serializer classes.  In most cases, you will want to use either:
+ * `NaturalKeyModelSerializer`, or
+ * The `natural_key_slug` pseudo-field (see below)
+
+If you have only a single model with a single char field for its natural key, you probably do not need to use either of these integrations.  In your view, you can just use Django REST Framework's built in `lookup_field` to point directly to your natural key.
+
+#### `NaturalKeyModelSerializer`
+`NaturalKeyModelSerializer` facilitates handling complex natural keys in your rest API.  It can be used with a `NaturalKeyModel`, or (more commonly) a model that has a foreign key to a `NaturalKeyModel` but is not a `NaturalKeyModel` itself.  (One concrete example of this is the [vera.Report] model, which has a ForeignKey to [vera.Event], which is a `NaturalKeyModel`).
+
+`NaturalKeyModelSerializer` extends DRF's [ModelSerializer], but uses `NaturalKeySerializer` for each foreign key that points to a `NaturalKeyModel`.  When `update()` or `create()`ing the primary model, the nested `NaturalKeySerializer`s will automatically create instances of referenced models if they do not exist already (via the `find()` method described above).  Note that `NaturalKeyModelSerializer` does not override DRF's default behavior for other fields, whether or not they form part of the primary model's natural key.
+
+`NaturalKeySerializer` can technically be used as a top level serializer, though this is not recommended.  `NaturalKeySerializer` is designed for dealing with nested natural keys and does not support updates or non-natural key fields.  Even when used together with `NaturalKeyModelSerializer`, `NaturalKeySerializer` never updates an existing related model instance.  Instead, it will repoint the foreign key to another (potentially new) instance of the related model.  It may help to think of `NaturalKeySerializer` as a special [RelatedField] class rather than as a `Serializer` per se.
+
+
+You can use `NaturalKeyModelSerializer` with [Django REST Framework] and/or [wq.db] just like any other serializer:
+```python
+# Django REST Framework usage example
+from rest_framework import viewsets
+from rest_framework import routers
+from natural_keys import NaturalKeyModelSerializer
+from .models import Event, Note
+
+class EventSerializer(NaturalKeyModelSerializer):
+    class Meta:
+        model = Event
+        
+class NoteSerializer(NaturalKeyModelSerializer):
+    class Meta:
+        model = Note
+
+class EventViewSet(viewsets.ModelViewSet):
+    queryset = Event.objects.all()
+    serializer_class = EventSerializer
+
+class NoteViewSet(viewsets.ModelViewSet):
+    queryset = Note.objects.all()
+    serializer_class = NoteSerializer
+
+router = routers.DefaultRouter()
+router.register(r'events', EventViewSet)
+router.register(r'notes', NoteViewSet)
+
+# wq.db usage example
+from wq.db import rest
+from natural_keys import NaturalKeyModelSerializer
+from .models import Event, Note
+
+rest.router.register_model(Note, serializer=NaturalKeyModelSerializer)
+rest.router.register_model(Event, serializer=NaturalKeyModelSerializer)
+```
+
+Once this is set up, you can use your REST API to create and view your `NaturalKeyModel` instances and related data.  To facilitate integration with regular HTML Forms, *Django Natural Keys* is integrated with the [HTML JSON Forms] package, which supports nested keys via an array naming convention, as the examples below demonstrate.
+
+```html
+<form action="/events/" method="post">
+  <input name="place[name]">
+  <input type="date" name="date">
+</form>
+```
+```js
+// /events.json
+[
+    {
+        "id": 123,
+        "place": {"name": "ABC123"},
+        "date": "2016-01-01"
+    }
+]
+```
+```html
+<form action="/notes/" method="post">
+  <input name="event[place][name]">
+  <input type="date" name="event[date]">
+  <textarea name="note"></textarea>
+</form>
+```
+```js
+// /notes.json
+[
+    {
+        "id": 12345,
+        "event": {
+            "place": {"name": "ABC123"},
+            "date": "2016-01-01"
+        },
+        "note": "This is a note"
+    }
+]
+```
+
+### Natural Key Slugs
+As an alternative to using `NaturalKeyModelSerializer` / `NaturalKeySerializer`, you can also use a single slug-like field for lookup and serialization.  `NaturalKeyModel` (and its associated queryset) defines a pseudo-field, `natural_key_slug`, for this purpose.
+
+```python
+class Place(NaturalKeyModel):
+    name = models.CharField(max_length=255, unique=True)
+    
+class Room(NaturalKeyModel)
+    place = models.ForeignKey(Place, models.ON_DELETE)
+    name = models.CharField(max_length=255)
+    
+    class Meta:
+        unique_together = (('place', 'name'),)
+```
+```python
+room = Room.objects.find("ABC123", "MainHall")
+assert(room.natural_key_slug == "ABC123-MainHall")
+assert(room == Room.objects.get(natural_key_slug="ABC123-MainHall"))
+```
+
+You can expose this functionality in your REST API to expose natural keys instead of database-generated ids.  To do this, you will likely want to do the following:
+
+ 1. Create a regular serializer with `id = serializers.ReadOnlyField(source='natural_key_slug')`
+ 2. Set `lookup_field = 'natural_key_slug'` on your `ModelViewSet` (or similar generic class) and update the URL registration accordingly
+ 3. Ensure foreign keys on any related models are serialized with `serializers.SlugRelatedField(slug_field='natural_key_slug')`
+
+In [wq.db], all three of the above can be achieved by setting the `"lookup"` attribute when registering with the [router]:
+
+```python
+# myapp/rest.py
+from wq.db import rest
+from .models import Room
+
+rest.router.register_model(
+    Room,
+    fields='__all__',
+    lookup='natural_key_slug',
+)
+```
+
+Note that the `natural_key_slug` may not behave as expected if any of the component values contain the delimiter character (`-` by default).  To mitigate this, you can set `natural_key_separator` on the model class to another character.
+
+[natural keys]: https://docs.djangoproject.com/en/4.2/topics/serialization/#natural-keys
+[UniqueConstraint]: https://docs.djangoproject.com/en/4.2/ref/models/constraints/#uniqueconstraint
+[unique_together]: https://docs.djangoproject.com/en/4.2/ref/models/options/#unique-together
+[unique]: https://docs.djangoproject.com/en/4.2/ref/models/fields/#unique
+
+[wq.db]: https://wq.io/wq.db/
+[Django REST Framework]: http://www.django-rest-framework.org/
+[vera.Report]:https://github.com/powered-by-wq/vera#report
+[vera.Event]: https://github.com/powered-by-wq/vera#event
+[ModelSerializer]: https://www.django-rest-framework.org/api-guide/serializers/#modelserializer
+[RelatedField]: https://www.django-rest-framework.org/api-guide/relations/
+[HTML JSON Forms]: https://github.com/wq/html-json-forms
+[router]: https://wq.io/wq.db/router
```

