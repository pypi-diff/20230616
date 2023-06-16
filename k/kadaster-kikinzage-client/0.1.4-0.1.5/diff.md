# Comparing `tmp/kadaster_kikinzage_client-0.1.4.tar.gz` & `tmp/kadaster_kikinzage_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kadaster_kikinzage_client-0.1.4.tar", max compression
+gzip compressed data, was "kadaster_kikinzage_client-0.1.5.tar", max compression
```

## Comparing `kadaster_kikinzage_client-0.1.4.tar` & `kadaster_kikinzage_client-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1071 2023-06-16 09:09:20.954109 kadaster_kikinzage_client-0.1.4/LICENSE
--rw-r--r--   0        0        0     4027 2023-06-16 09:09:20.954109 kadaster_kikinzage_client-0.1.4/README.md
--rw-r--r--   0        0        0     2113 2023-06-16 09:09:35.326634 kadaster_kikinzage_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       45 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/__init__.py
--rw-r--r--   0        0        0     2274 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/__main__.py
--rw-r--r--   0        0        0      302 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/__init__.py
--rw-r--r--   0        0        0     2379 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/asyncio.py
--rw-r--r--   0        0        0     9405 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/base.py
--rw-r--r--   0        0        0     5365 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/default.py
--rw-r--r--   0        0        0      610 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/errors.py
--rw-r--r--   0        0        0      182 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/utils.py
--rw-r--r--   0        0        0      372 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/__init__.py
--rw-r--r--   0        0        0     2975 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/adres.py
--rw-r--r--   0        0        0    11899 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/collectie.py
--rw-r--r--   0        0        0     5786 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/eigendomsinformatie.py
--rw-r--r--   0        0        0     1445 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/enum.py
--rw-r--r--   0        0        0     8739 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/generated.py
--rw-r--r--   0        0        0      629 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/misc.py
--rw-r--r--   0        0        0     3500 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/persoon.py
--rw-r--r--   0        0        0     4158 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/product.py
--rw-r--r--   0        0        0     2361 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/stukken.py
--rw-r--r--   0        0        0     1243 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/zekerheid.py
--rw-r--r--   0        0        0        0 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/py.typed
--rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 12:34:44.020569 kadaster_kikinzage_client-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4027 2023-06-16 12:34:44.020569 kadaster_kikinzage_client-0.1.5/README.md
+-rw-r--r--   0        0        0     2113 2023-06-16 12:35:02.385155 kadaster_kikinzage_client-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/__init__.py
+-rw-r--r--   0        0        0     2274 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/__main__.py
+-rw-r--r--   0        0        0      302 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/__init__.py
+-rw-r--r--   0        0        0     2379 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/asyncio.py
+-rw-r--r--   0        0        0     9405 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/base.py
+-rw-r--r--   0        0        0     5365 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/default.py
+-rw-r--r--   0        0        0      610 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/errors.py
+-rw-r--r--   0        0        0      182 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/client/utils.py
+-rw-r--r--   0        0        0      401 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/__init__.py
+-rw-r--r--   0        0        0     2927 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/adres.py
+-rw-r--r--   0        0        0    11899 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/collectie.py
+-rw-r--r--   0        0        0     5786 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/eigendomsinformatie.py
+-rw-r--r--   0        0        0     1445 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/enum.py
+-rw-r--r--   0        0        0     8739 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/generated.py
+-rw-r--r--   0        0        0      613 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/misc.py
+-rw-r--r--   0        0        0     3452 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/persoon.py
+-rw-r--r--   0        0        0     4030 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/product.py
+-rw-r--r--   0        0        0     2361 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/stukken.py
+-rw-r--r--   0        0        0     1195 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/models/zekerheid.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:34:44.024570 kadaster_kikinzage_client-0.1.5/src/kikinzage/py.typed
+-rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.5/PKG-INFO
```

### Comparing `kadaster_kikinzage_client-0.1.4/LICENSE` & `kadaster_kikinzage_client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/README.md` & `kadaster_kikinzage_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/pyproject.toml` & `kadaster_kikinzage_client-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kadaster-kikinzage-client"
-version = "0.1.4"
+version = "0.1.5"
 description = " Kadaster - KIK Inzage API Python client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 repository = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 documentation = "https://kadaster-kik-inzage-api-python-client.readthedocs.io"
```

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/__main__.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/__main__.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/client/asyncio.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/client/asyncio.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/client/base.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/client/base.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/client/default.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/client/default.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/client/errors.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/client/errors.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/adres.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/adres.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import RootModel
 from typing_extensions import Annotated
 
-from kikinzage.models.enum import AdresLocatieTypeEnum
-from kikinzage.models.misc import NEN3610ID
-from kikinzage.models.misc import Waardelijst
+from .enum import AdresLocatieTypeEnum
+from .misc import NEN3610ID
+from .misc import Waardelijst
 
 
 class Adresnummer(RootModel[str]):
     root: str = Field(..., title="Adresnummer")
 
 
 class OpenbareRuimte(BaseModel):
```

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/collectie.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/collectie.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/eigendomsinformatie.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/eigendomsinformatie.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/enum.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/enum.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/generated.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/generated.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/misc.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/misc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 
-from kikinzage.models.enum import Type
+from .enum import Type
 
 
 class NEN3610ID(BaseModel):
     lokaal_id: str = Field(..., alias="lokaalID")
     namespace: str
```

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/persoon.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/persoon.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from typing import Optional
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Field
 from typing_extensions import Annotated
 
-from kikinzage.models.enum import PersoonTypeEnum
-from kikinzage.models.misc import NEN3610ID
-from kikinzage.models.misc import Waardelijst
+from .enum import PersoonTypeEnum
+from .misc import NEN3610ID
+from .misc import Waardelijst
 
 
 class TypeOnvolledigeDatum(BaseModel):
     dag: Optional[int] = Field(None, ge=1, le=31)
     datum: Optional[date] = None
     jaar: Optional[int] = Field(None, le=9999)
     maand: Optional[int] = Field(None, ge=1, le=12)
```

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/product.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/product.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from datetime import datetime
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 
-from kikinzage.models.collectie import ATCollectie
-from kikinzage.models.collectie import EDICollectie
-from kikinzage.models.collectie import EGICollectie
-from kikinzage.models.collectie import HPICollectie
-from kikinzage.models.collectie import OICollectie
-from kikinzage.models.collectie import OLPCollectie
-from kikinzage.models.collectie import PTCollectie
-from kikinzage.models.misc import NEN3610ID
+from .collectie import ATCollectie
+from .collectie import EDICollectie
+from .collectie import EGICollectie
+from .collectie import HPICollectie
+from .collectie import OICollectie
+from .collectie import OLPCollectie
+from .collectie import PTCollectie
+from .misc import NEN3610ID
 
 
 class Product(BaseModel):
     actualiteitstijdstip_hypothecair: Optional[datetime] = Field(
         None, alias="actualiteitstijdstipHypothecair"
     )
     actualiteitstijdstip_kadastraal: Optional[datetime] = Field(
```

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/stukken.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/stukken.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/zekerheid.py` & `kadaster_kikinzage_client-0.1.5/src/kikinzage/models/zekerheid.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 
-from kikinzage.models.enum import ZekerheidsstellingTypeEnum
-from kikinzage.models.misc import NEN3610ID
-from kikinzage.models.misc import Waardelijst
+from .enum import ZekerheidsstellingTypeEnum
+from .misc import NEN3610ID
+from .misc import Waardelijst
 
 
 class FieldZekerheidsstelling(BaseModel):
     identificatie: Optional[NEN3610ID] = None
     type: Optional[ZekerheidsstellingTypeEnum] = None
     omschrijving_betrokken_recht: Optional[Waardelijst] = Field(
         None, alias="omschrijvingBetrokkenRecht"
```

### Comparing `kadaster_kikinzage_client-0.1.4/PKG-INFO` & `kadaster_kikinzage_client-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kadaster-kikinzage-client
-Version: 0.1.4
+Version: 0.1.5
 Summary:  Kadaster - KIK Inzage API Python client
 Home-page: https://github.com/foarsitter/kadaster-kik-inzage-api-python-client
 License: MIT
 Author: Jelmer Draaijer
 Author-email: info@jelmert.nl
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
```

