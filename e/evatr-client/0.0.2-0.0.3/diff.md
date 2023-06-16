# Comparing `tmp/evatr-client-0.0.2.tar.gz` & `tmp/evatr-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evatr-client-0.0.2.tar", last modified: Thu Jun 15 17:02:03 2023, max compression
+gzip compressed data, was "evatr-client-0.0.3.tar", last modified: Fri Jun 16 08:44:43 2023, max compression
```

## Comparing `evatr-client-0.0.2.tar` & `evatr-client-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 17:02:03.300916 evatr-client-0.0.2/
--rw-rw-rw-   0        0        0     1084 2023-06-15 16:27:48.000000 evatr-client-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      825 2023-06-15 17:02:03.300916 evatr-client-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1751 2023-06-15 16:53:34.000000 evatr-client-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 17:02:03.291906 evatr-client-0.0.2/evatr_client/
--rw-rw-rw-   0        0        0      119 2023-06-15 16:57:51.000000 evatr-client-0.0.2/evatr_client/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-06-15 16:20:36.000000 evatr-client-0.0.2/evatr_client/evatr_client.py
--rw-rw-rw-   0        0        0     4612 2023-06-15 15:56:16.000000 evatr-client-0.0.2/evatr_client/status_codes.py
--rw-rw-rw-   0        0        0     2113 2023-06-15 15:57:13.000000 evatr-client-0.0.2/evatr_client/util.py
-drwxrwxrwx   0        0        0        0 2023-06-15 17:02:03.299905 evatr-client-0.0.2/evatr_client.egg-info/
--rw-rw-rw-   0        0        0      825 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 17:02:03.000000 evatr-client-0.0.2/evatr_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-15 17:02:03.301904 evatr-client-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1185 2023-06-15 17:00:13.000000 evatr-client-0.0.2/setup.py
+drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-16 08:44:43.886913 evatr-client-0.0.3/
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      810 2023-06-16 08:44:43.887082 evatr-client-0.0.3/PKG-INFO
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1696 2023-06-16 08:34:10.000000 evatr-client-0.0.3/README.md
+drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-16 08:44:43.884405 evatr-client-0.0.3/evatr_client/
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      138 2023-06-16 08:35:04.000000 evatr-client-0.0.3/evatr_client/__init__.py
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     3578 2023-06-16 08:34:10.000000 evatr-client-0.0.3/evatr_client/client.py
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     4532 2023-06-16 08:34:10.000000 evatr-client-0.0.3/evatr_client/status_codes.py
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     2015 2023-06-16 08:37:53.000000 evatr-client-0.0.3/evatr_client/util.py
+drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-16 08:44:43.886613 evatr-client-0.0.3/evatr_client.egg-info/
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      810 2023-06-16 08:44:43.000000 evatr-client-0.0.3/evatr_client.egg-info/PKG-INFO
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      305 2023-06-16 08:44:43.000000 evatr-client-0.0.3/evatr_client.egg-info/SOURCES.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)        1 2023-06-16 08:44:43.000000 evatr-client-0.0.3/evatr_client.egg-info/dependency_links.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)       32 2023-06-16 08:44:43.000000 evatr-client-0.0.3/evatr_client.egg-info/requires.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)       13 2023-06-16 08:44:43.000000 evatr-client-0.0.3/evatr_client.egg-info/top_level.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)       79 2023-06-16 08:44:43.887656 evatr-client-0.0.3/setup.cfg
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1152 2023-06-16 08:41:35.000000 evatr-client-0.0.3/setup.py
```

### Comparing `evatr-client-0.0.2/PKG-INFO` & `evatr-client-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1
-Name: evatr-client
-Version: 0.0.2
-Summary: A client for: https://evatr.bff-online.de/eVatR/
-Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.2.tar.gz
-Author: CeeDiii
-License: MIT
-Keywords: python,uid,vat,uid prüfung,vat validation,evatr
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/
+Metadata-Version: 2.1
+Name: evatr-client
+Version: 0.0.3
+Summary: A client for: https://evatr.bff-online.de/eVatR/
+Home-page: https://github.com/CeeDiii/evatr-client
+Author: CeeDiii
+License: MIT
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.3.tar.gz
+Description: A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/
+Keywords: python,uid,vat,uid prüfung,vat validation,evatr
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
```

### Comparing `evatr-client-0.0.2/README.md` & `evatr-client-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# Python eVatR Client
-A Python client for simple and qualified VAT-number validations. 
-
-This is a Python port of the Typescript client that can be found here: https://github.com/qqilihq/evatr/tree/master
-
-The API is provided by the German “Bundeszentralamt für Steuern”.
-
-To use this tool, you need to be in possession of a valid German VAT number.
-
-## Usage
-```python
-client = EvatrClient()
-
-simpleParams: ISimpleParams = ISimpleParams(include_raw_xml=False,
-                                                own_vat_number='<your own VAT number>', 
-                                                validate_vat_number='<the VAT number to validate>')
-
-client.check_simple(simpleParams)
-
-qualifiedParams: IQualifiedParams = IQualifiedParams(include_raw_xml=False,
-                                                own_vat_number='<your own VAT number>', 
-                                                validate_vat_number='<the VAT number to validate>', 
-                                                company_name='<SomeCompany Srl>', 
-                                                city='Milano', 
-                                                zip='20123', 
-                                                street='Via Italia 22')
-
-client.check_qualified(qualifiedParams)
-
-```
-
-## Installation
-The source code is currently hosted on GitHub at: https://github.com/CeeDiii/evatr-client
-
-The Python package is available at Python Package Index (PyPI)
-
-```
-pip install evatr-client
-```
-## Development
-
-Install dependecies from the `requirements.txt` file:
-
-```shell
-pip install -r requirements.txt
-```
-
-## Contributing 
-Feel free to open issues and pull requests in this repo.
-
-## License
-
-
-
-
+# Python eVatR Client
+A Python client for simple and qualified VAT-number validations. 
+
+This is a Python port of the Typescript client that can be found here: https://github.com/qqilihq/evatr/tree/master
+
+The API is provided by the German “Bundeszentralamt für Steuern”.
+
+To use this tool, you need to be in possession of a valid German VAT number.
+
+## Usage
+```python
+client = EvatrClient()
+
+simpleParams: ISimpleParams = ISimpleParams(include_raw_xml=False,
+                                                own_vat_number='<your own VAT number>', 
+                                                validate_vat_number='<the VAT number to validate>')
+
+client.check_simple(simpleParams)
+
+qualifiedParams: IQualifiedParams = IQualifiedParams(include_raw_xml=False,
+                                                own_vat_number='<your own VAT number>', 
+                                                validate_vat_number='<the VAT number to validate>', 
+                                                company_name='<SomeCompany Srl>', 
+                                                city='Milano', 
+                                                zip='20123', 
+                                                street='Via Italia 22')
+
+client.check_qualified(qualifiedParams)
+
+```
+
+## Installation
+The source code is currently hosted on GitHub at: https://github.com/CeeDiii/evatr-client
+
+The Python package is available at Python Package Index (PyPI)
+
+```
+pip install evatr-client
+```
+## Development
+
+Install dependecies from the `requirements.txt` file:
+
+```shell
+pip install -r requirements.txt
+```
+
+## Contributing 
+Feel free to open issues and pull requests in this repo.
+
+## License
+
+
+
+
```

### Comparing `evatr-client-0.0.2/evatr_client/evatr_client.py` & `evatr-client-0.0.3/evatr_client/client.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import requests
-
-from dataclasses import asdict
-from urllib.parse import urlencode
-from xml.etree.ElementTree import fromstring
-
-from util import ISimpleParams, IQualifiedParams, ISimpleResult, IQualifiedResult, get_error_description, get_result_description
-
-class EvatrClient:
-    def retrieve_xml(self, params: ISimpleParams | IQualifiedParams, qualified: bool = False) -> str:
-        if params is None:
-            raise AttributeError()
-
-        query = {
-            'UstId_1': params.own_vat_number,
-            'UstId_2': params.validate_vat_number
-        }
-
-        if qualified:
-            query['Firmenname'] = params.company_name
-            query['Ort'] = params.city
-            query['PLZ'] = params.zip
-            query['Strasse'] = params.street
-
-        requestUrl = f'https://evatr.bff-online.de/evatrRPC?{urlencode(query)}'
-        res = requests.get(requestUrl)
-
-        if res.ok:
-            return res.text
-        else:
-            raise Exception()
-        
-    def map_xml_response_data(self, raw_xml: str):
-        root = fromstring(raw_xml)
-        params = root.findall('.//param')
-        label = []
-        values = []
-        for param in params:
-            val_tag = param.findall('.//string')
-            if len(val_tag) >= 2:
-                label.append(val_tag[0].text)
-                values.append(val_tag[1].text)
-        response = dict(zip(label, values))
-        return response
-
-    def parse_xml_response(self, raw_xml: str, qualified: bool = False, include_raw_xml: bool = False) -> ISimpleResult | IQualifiedResult:   
-        response = self.map_xml_response_data(raw_xml)
-
-        error_code = int(response['ErrorCode'])
-        result_name = response['Erg_Name']
-        result_city = response['Erg_Ort']
-        result_zip = response['Erg_PLZ']
-        result_street = response['Erg_Str']
-
-        result = ISimpleResult(
-            valid=error_code == 200,
-            date=response['Datum'],
-            time=response['Uhrzeit'],
-            error_code=response['ErrorCode'],
-            error_description=get_error_description(error_code),
-            own_vat_number=response['UstId_1'],
-            validated_vat_number=response['UstId_2'],
-            valid_from=response['Gueltig_ab'],
-            valid_until=response['Gueltig_bis'],
-            raw_xml=raw_xml if include_raw_xml else None
-        )
-
-        if qualified:
-            result = IQualifiedResult(
-                *asdict(result).values(),
-                company_name=response['Firmenname'],
-                city=response['Ort'],
-                zip=response['PLZ'],
-                street=response['Strasse'],
-                result_name=result_name,
-                result_city=result_city,
-                result_zip=result_zip,
-                result_street=result_street,
-                result_name_description=get_result_description(result_name),
-                result_city_description=get_result_description(result_city),
-                result_zip_description=get_result_description(result_zip),
-                result_street_description=get_result_description(result_street)
-            )
-
-        return result
-
-
-    def check_simple(self, params: ISimpleParams):
-        xml = self.retrieve_xml(params, qualified=False)
-        return self.parse_xml_response(xml, qualified=False, include_raw_xml=params.include_raw_xml)
-
-
-    def check_qualified(self, params: IQualifiedParams):
-        xml = self.retrieve_xml(params, qualified=True)
+import requests
+
+from dataclasses import asdict
+from urllib.parse import urlencode
+from xml.etree.ElementTree import fromstring
+
+from util import ISimpleParams, IQualifiedParams, ISimpleResult, IQualifiedResult, get_error_description, get_result_description
+
+class EvatrClient:
+    def retrieve_xml(self, params: ISimpleParams | IQualifiedParams, qualified: bool = False) -> str:
+        if params is None:
+            raise AttributeError()
+
+        query = {
+            'UstId_1': params.own_vat_number,
+            'UstId_2': params.validate_vat_number
+        }
+
+        if qualified:
+            query['Firmenname'] = params.company_name
+            query['Ort'] = params.city
+            query['PLZ'] = params.zip
+            query['Strasse'] = params.street
+
+        requestUrl = f'https://evatr.bff-online.de/evatrRPC?{urlencode(query)}'
+        res = requests.get(requestUrl)
+
+        if res.ok:
+            return res.text
+        else:
+            raise Exception()
+        
+    def map_xml_response_data(self, raw_xml: str):
+        root = fromstring(raw_xml)
+        params = root.findall('.//param')
+        label = []
+        values = []
+        for param in params:
+            val_tag = param.findall('.//string')
+            if len(val_tag) >= 2:
+                label.append(val_tag[0].text)
+                values.append(val_tag[1].text)
+        response = dict(zip(label, values))
+        return response
+
+    def parse_xml_response(self, raw_xml: str, qualified: bool = False, include_raw_xml: bool = False) -> ISimpleResult | IQualifiedResult:   
+        response = self.map_xml_response_data(raw_xml)
+
+        error_code = int(response['ErrorCode'])
+        result_name = response['Erg_Name']
+        result_city = response['Erg_Ort']
+        result_zip = response['Erg_PLZ']
+        result_street = response['Erg_Str']
+
+        result = ISimpleResult(
+            valid=error_code == 200,
+            date=response['Datum'],
+            time=response['Uhrzeit'],
+            error_code=response['ErrorCode'],
+            error_description=get_error_description(error_code),
+            own_vat_number=response['UstId_1'],
+            validated_vat_number=response['UstId_2'],
+            valid_from=response['Gueltig_ab'],
+            valid_until=response['Gueltig_bis'],
+            raw_xml=raw_xml if include_raw_xml else None
+        )
+
+        if qualified:
+            result = IQualifiedResult(
+                *asdict(result).values(),
+                company_name=response['Firmenname'],
+                city=response['Ort'],
+                zip=response['PLZ'],
+                street=response['Strasse'],
+                result_name=result_name,
+                result_city=result_city,
+                result_zip=result_zip,
+                result_street=result_street,
+                result_name_description=get_result_description(result_name),
+                result_city_description=get_result_description(result_city),
+                result_zip_description=get_result_description(result_zip),
+                result_street_description=get_result_description(result_street)
+            )
+
+        return result
+
+
+    def check_simple(self, params: ISimpleParams):
+        xml = self.retrieve_xml(params, qualified=False)
+        return self.parse_xml_response(xml, qualified=False, include_raw_xml=params.include_raw_xml)
+
+
+    def check_qualified(self, params: IQualifiedParams):
+        xml = self.retrieve_xml(params, qualified=True)
         return self.parse_xml_response(xml, qualified=True, include_raw_xml=params.include_raw_xml)
```

### Comparing `evatr-client-0.0.2/evatr_client/util.py` & `evatr-client-0.0.3/evatr_client/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,72 @@
-import json
-import os
-
-from dataclasses import dataclass
-from enum import Enum
-from typing import Optional
-
-from status_codes import status_codes
-
-class ResultType(Enum):
-    MATCH = 'A',
-    NO_MATCH = 'B',
-    NOT_QUERIED = 'C',
-    NOT_RETURNED = 'D',
-
-@dataclass
-class ISimpleParams:
-    include_raw_xml: bool
-    own_vat_number: str
-    validate_vat_number: str
-
-
-@dataclass
-class IQualifiedParams(ISimpleParams):
-    company_name: str
-    city: str
-    zip: Optional[str] = None
-    street: Optional[str] = None
-
-
-@dataclass
-class ISimpleResult:
-    valid: bool
-    date: str
-    time: str
-    error_code: int
-    error_description: str
-    own_vat_number: str
-    validated_vat_number: str
-    valid_from: Optional[str] = None
-    valid_until: Optional[str] = None
-    raw_xml: Optional[str] = None
-
-
-@dataclass
-class IQualifiedResult(ISimpleResult):
-    company_name: Optional[str] = None
-    city: Optional[str] = None
-    zip: Optional[str] = None
-    street: Optional[str] = None
-    result_name: Optional[ResultType] = ResultType.NOT_QUERIED
-    result_city: Optional[ResultType] = ResultType.NOT_QUERIED
-    result_zip: Optional[ResultType] = ResultType.NOT_QUERIED
-    result_street: Optional[ResultType] = ResultType.NOT_QUERIED
-    result_name_description: Optional[str] = None
-    result_city_description: Optional[str] = None
-    result_zip_description: Optional[str] = None
-    result_street_description: Optional[str] = None
-
-def get_result_description(result_type):
-    if result_type == ResultType.MATCH:
-        return 'stimmt überein'
-    elif result_type == ResultType.NO_MATCH:
-        return 'stimmt nicht überein'
-    elif result_type == ResultType.NOT_QUERIED:
-        return 'nicht angefragt'
-    elif result_type == ResultType.NOT_RETURNED:
-        return 'vom EU-Mitgliedsstaat nicht mitgeteilt'
-    else:
-        return None
-    
-def get_error_description(error_code: int):
-    if error_code in status_codes:
-       return status_codes[error_code]
-    return 'Description not found for the given code.'
+from dataclasses import dataclass
+from enum import Enum
+from typing import Optional
+
+from status_codes import status_codes
+
+class ResultType(Enum):
+    MATCH = 'A',
+    NO_MATCH = 'B',
+    NOT_QUERIED = 'C',
+    NOT_RETURNED = 'D',
+
+@dataclass
+class ISimpleParams:
+    include_raw_xml: bool
+    own_vat_number: str
+    validate_vat_number: str
+
+
+@dataclass
+class IQualifiedParams(ISimpleParams):
+    company_name: str
+    city: str
+    zip: Optional[str] = None
+    street: Optional[str] = None
+
+
+@dataclass
+class ISimpleResult:
+    valid: bool
+    date: str
+    time: str
+    error_code: int
+    error_description: str
+    own_vat_number: str
+    validated_vat_number: str
+    valid_from: Optional[str] = None
+    valid_until: Optional[str] = None
+    raw_xml: Optional[str] = None
+
+
+@dataclass
+class IQualifiedResult(ISimpleResult):
+    company_name: Optional[str] = None
+    city: Optional[str] = None
+    zip: Optional[str] = None
+    street: Optional[str] = None
+    result_name: Optional[ResultType] = ResultType.NOT_QUERIED
+    result_city: Optional[ResultType] = ResultType.NOT_QUERIED
+    result_zip: Optional[ResultType] = ResultType.NOT_QUERIED
+    result_street: Optional[ResultType] = ResultType.NOT_QUERIED
+    result_name_description: Optional[str] = None
+    result_city_description: Optional[str] = None
+    result_zip_description: Optional[str] = None
+    result_street_description: Optional[str] = None
+
+def get_result_description(result_type):
+    if result_type == ResultType.MATCH:
+        return 'stimmt überein'
+    elif result_type == ResultType.NO_MATCH:
+        return 'stimmt nicht überein'
+    elif result_type == ResultType.NOT_QUERIED:
+        return 'nicht angefragt'
+    elif result_type == ResultType.NOT_RETURNED:
+        return 'vom EU-Mitgliedsstaat nicht mitgeteilt'
+    else:
+        return None
+    
+def get_error_description(error_code: int):
+    if error_code in status_codes:
+       return status_codes[error_code]
+    return 'Description not found for the given code.'
```

### Comparing `evatr-client-0.0.2/evatr_client.egg-info/PKG-INFO` & `evatr-client-0.0.3/evatr_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1
-Name: evatr-client
-Version: 0.0.2
-Summary: A client for: https://evatr.bff-online.de/eVatR/
-Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.2.tar.gz
-Author: CeeDiii
-License: MIT
-Keywords: python,uid,vat,uid prüfung,vat validation,evatr
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/
+Metadata-Version: 2.1
+Name: evatr-client
+Version: 0.0.3
+Summary: A client for: https://evatr.bff-online.de/eVatR/
+Home-page: https://github.com/CeeDiii/evatr-client
+Author: CeeDiii
+License: MIT
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.3.tar.gz
+Description: A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/
+Keywords: python,uid,vat,uid prüfung,vat validation,evatr
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
```

### Comparing `evatr-client-0.0.2/setup.py` & `evatr-client-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from setuptools import setup, find_packages
-
-VERSION = '0.0.2'
-DESCRIPTION = 'A client for: https://evatr.bff-online.de/eVatR/'
-LONG_DESCRIPTION = 'A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/'
-
-# Setting up
-setup(
-    name="evatr-client",
-    version=VERSION,
-    author="CeeDiii",
-    description=DESCRIPTION,
-    license='MIT',
-    url='https://github.com/CeeDiii/evatr-client',
-    download_url='https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.2.tar.gz',
-    long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
-    keywords=['python', 'uid', 'vat', 'uid prüfung', 'vat validation', 'evatr'],
-    install_requires=[
-          'requests',
-          'urllib3',
-          'beautifulsoup4',
-    ],
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ]
-)
+from setuptools import setup, find_packages
+
+VERSION = '0.0.3'
+DESCRIPTION = 'A client for: https://evatr.bff-online.de/eVatR/'
+LONG_DESCRIPTION = 'A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/'
+
+# Setting up
+setup(
+    name="evatr-client",
+    version=VERSION,
+    author="CeeDiii",
+    description=DESCRIPTION,
+    license='MIT',
+    url='https://github.com/CeeDiii/evatr-client',
+    download_url='https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.3.tar.gz',
+    long_description_content_type="text/markdown",
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    keywords=['python', 'uid', 'vat', 'uid prüfung', 'vat validation', 'evatr'],
+    install_requires=[
+          'requests',
+          'urllib3',
+          'beautifulsoup4',
+    ],
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```

