# Comparing `tmp/kadaster_kikinzage_client-0.1.3.tar.gz` & `tmp/kadaster_kikinzage_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kadaster_kikinzage_client-0.1.3.tar", max compression
+gzip compressed data, was "kadaster_kikinzage_client-0.1.4.tar", max compression
```

## Comparing `kadaster_kikinzage_client-0.1.3.tar` & `kadaster_kikinzage_client-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1071 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/LICENSE
--rw-r--r--   0        0        0     4027 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/README.md
--rw-r--r--   0        0        0     2113 2023-06-15 15:43:00.989328 kadaster_kikinzage_client-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       45 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/__init__.py
--rw-r--r--   0        0        0     2274 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/__main__.py
--rw-r--r--   0        0        0      302 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/__init__.py
--rw-r--r--   0        0        0     2379 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/asyncio.py
--rw-r--r--   0        0        0     9405 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/base.py
--rw-r--r--   0        0        0     5365 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/default.py
--rw-r--r--   0        0        0      610 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/errors.py
--rw-r--r--   0        0        0      182 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/client/utils.py
--rw-r--r--   0        0        0      372 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/__init__.py
--rw-r--r--   0        0        0    10276 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/collectie.py
--rw-r--r--   0        0        0     5786 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/eigendomsinformatie.py
--rw-r--r--   0        0        0     1400 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/enum.py
--rw-r--r--   0        0        0    16298 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/generated.py
--rw-r--r--   0        0        0      629 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/misc.py
--rw-r--r--   0        0        0     3500 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/persoon.py
--rw-r--r--   0        0        0     1129 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/product.py
--rw-r--r--   0        0        0     1941 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/stukken.py
--rw-r--r--   0        0        0     1243 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/models/zekerheid.py
--rw-r--r--   0        0        0        0 2023-06-15 15:42:46.941416 kadaster_kikinzage_client-0.1.3/src/kikinzage/py.typed
--rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-16 09:09:20.954109 kadaster_kikinzage_client-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4027 2023-06-16 09:09:20.954109 kadaster_kikinzage_client-0.1.4/README.md
+-rw-r--r--   0        0        0     2113 2023-06-16 09:09:35.326634 kadaster_kikinzage_client-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/__init__.py
+-rw-r--r--   0        0        0     2274 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/__main__.py
+-rw-r--r--   0        0        0      302 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/__init__.py
+-rw-r--r--   0        0        0     2379 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/asyncio.py
+-rw-r--r--   0        0        0     9405 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/base.py
+-rw-r--r--   0        0        0     5365 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/default.py
+-rw-r--r--   0        0        0      610 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/errors.py
+-rw-r--r--   0        0        0      182 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/client/utils.py
+-rw-r--r--   0        0        0      372 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/__init__.py
+-rw-r--r--   0        0        0     2975 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/adres.py
+-rw-r--r--   0        0        0    11899 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/collectie.py
+-rw-r--r--   0        0        0     5786 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/eigendomsinformatie.py
+-rw-r--r--   0        0        0     1445 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/enum.py
+-rw-r--r--   0        0        0     8739 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/generated.py
+-rw-r--r--   0        0        0      629 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/misc.py
+-rw-r--r--   0        0        0     3500 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/persoon.py
+-rw-r--r--   0        0        0     4158 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/product.py
+-rw-r--r--   0        0        0     2361 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/stukken.py
+-rw-r--r--   0        0        0     1243 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/models/zekerheid.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:09:20.958109 kadaster_kikinzage_client-0.1.4/src/kikinzage/py.typed
+-rw-r--r--   0        0        0     5083 1970-01-01 00:00:00.000000 kadaster_kikinzage_client-0.1.4/PKG-INFO
```

### Comparing `kadaster_kikinzage_client-0.1.3/LICENSE` & `kadaster_kikinzage_client-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.3/README.md` & `kadaster_kikinzage_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.3/pyproject.toml` & `kadaster_kikinzage_client-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kadaster-kikinzage-client"
-version = "0.1.3"
+version = "0.1.4"
 description = " Kadaster - KIK Inzage API Python client"
 authors = ["Jelmer Draaijer <info@jelmert.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 repository = "https://github.com/foarsitter/kadaster-kik-inzage-api-python-client"
 documentation = "https://kadaster-kik-inzage-api-python-client.readthedocs.io"
```

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/__main__.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
     ctx.obj["filename"] = filename
 
 
 @eigendomsinformatie.command()
 @click.pass_context
 @click.argument("postcode", type=str)
-@click.argument("huisnummer", type=str)
-def postcode(ctx: Context, postcode: str, huisnummer: str) -> None:
+@click.argument("huisnummer", type=int)
+def postcode(ctx: Context, postcode: str, huisnummer: int) -> None:
     """Eigendomsinformatie - Postcode."""
 
     log_response = ResponseStorage()
     response_path = Path(ctx.obj["filename"])
 
     kik = DefaultClient(
         username=os.getenv("KIK_USERNAME", default="EMPTY"),
```

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/client/asyncio.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/client/asyncio.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/client/base.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/client/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         )
 
         return request
 
     def request_eigendomsinformatie_postcode(
         self,
         postcode: str,
-        huisnummer: str,
+        huisnummer: int,
         huisletter: Optional[str] = None,
         huisnummertoevoeging: Optional[str] = None,
         *,
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
```

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/client/default.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/client/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         )
 
         return self.send(request, models.Eigendomsinformatie)
 
     def eigendomsinformatie_postcode(
         self,
         postcode: str,
-        huisnummer: str,
+        huisnummer: int,
         huisletter: Optional[str] = None,
         huisnummertoevoeging: Optional[str] = None,
         *,
         formaat: Union[Formaat, UseClientDefault] = USE_CLIENT_DEFAULT,
         klantreferentie: Union[str, UseClientDefault] = USE_CLIENT_DEFAULT,
         gebruikeridentificatie: Optional[str] = None,
         hyperlinkopproduct: Optional[bool] = None,
```

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/client/errors.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/client/errors.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/models/collectie.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/collectie.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from datetime import datetime
 from typing import List
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 
-from kikinzage.models.eigendomsinformatie import AppartementsrechtSplitsing
-from kikinzage.models.eigendomsinformatie import Beperkingsgebied
-from kikinzage.models.eigendomsinformatie import Erfpachtcanon
-from kikinzage.models.eigendomsinformatie import GezamenlijkAandeel
-from kikinzage.models.eigendomsinformatie import Herverkavelingsgebied
-from kikinzage.models.eigendomsinformatie import Mandeligheid
-from kikinzage.models.eigendomsinformatie import PubliekrechtelijkeBeperking
-from kikinzage.models.eigendomsinformatie import Tenaamstelling
-from kikinzage.models.eigendomsinformatie import VerkavelObject
-from kikinzage.models.eigendomsinformatie import ZakelijkRecht
-
-from .enum import AdresLocatieTypeEnum
+from .adres import AdresType
+from .adres import FieldAdresLocatie
+from .eigendomsinformatie import AppartementsrechtSplitsing
+from .eigendomsinformatie import Beperkingsgebied
+from .eigendomsinformatie import Erfpachtcanon
+from .eigendomsinformatie import GezamenlijkAandeel
+from .eigendomsinformatie import Herverkavelingsgebied
+from .eigendomsinformatie import Mandeligheid
+from .eigendomsinformatie import PubliekrechtelijkeBeperking
+from .eigendomsinformatie import Tenaamstelling
+from .eigendomsinformatie import VerkavelObject
+from .eigendomsinformatie import ZakelijkRecht
 from .enum import OnroerendeZaakTypeEnum
 from .misc import NEN3610ID
 from .misc import Bedrag
 from .misc import Waardelijst
 from .persoon import PersoonType
-from .product import Product
-from .stukken import FieldStuk
+from .stukken import FieldType
 from .zekerheid import FieldZekerheidsstelling
 
 
 class Aantekening(BaseModel):
     identificatie: Optional[NEN3610ID] = None
     aard: Optional[Waardelijst] = None
     betreft_gedeelte_van_perceel: Optional[bool] = Field(
@@ -61,19 +60,14 @@
     betreft_oz: Optional[NEN3610ID] = Field(None, alias="betreftOZ")
 
 
 class VoorwaartseOnroerendeZaakFiliatie(BaseModel):
     betreft_oz: Optional[NEN3610ID] = Field(None, alias="betreftOZ")
 
 
-class FieldAdresLocatie(BaseModel):
-    identificatie: Optional[NEN3610ID] = None
-    type: Optional[AdresLocatieTypeEnum] = None
-
-
 class FieldKadastraalObject(BaseModel):
     identificatie: Optional[NEN3610ID] = None
 
 
 class AanvullendeGegevens(BaseModel):
     bij_identificatie: Optional[NEN3610ID] = Field(None, alias="bijIdentificatie")
     soort: Optional[str] = None
@@ -227,25 +221,23 @@
     locatie_kadastraal_objecten: Optional[List[LocatieKadastraalObject]] = Field(
         None, alias="locatieKadastraalObjecten"
     )
     onroerende_zaken: Optional[List[FieldOnroerendeZaak]] = Field(
         None, alias="onroerendeZaken"
     )
     personen: Optional[List[PersoonType]] = None
-    adres_locaties: Optional[List[FieldAdresLocatie]] = Field(
-        None, alias="adresLocaties"
-    )
+    adres_locaties: Optional[List[AdresType]] = Field(None, alias="adresLocaties")
     attendering_kadastraal_objecten: Optional[
         List[AttenderingKadastraalObject]
     ] = Field(None, alias="attenderingKadastraalObjecten")
     signalering_kadastraal_objecten: Optional[
         List[SignaleringKadastraalObject]
     ] = Field(None, alias="signaleringKadastraalObjecten")
     stukdelen: Optional[List[Stukdeel]] = None
-    stukken: Optional[List[FieldStuk]] = None
+    stukken: Optional[List[FieldType]] = None
     verblijfsobjecten: Optional[List[Verblijfsobject]] = None
     aanvullende_gegevens: Optional[List[AanvullendeGegevens]] = Field(
         None, alias="aanvullendeGegevens"
     )
 
 
 class EDICollectie(Collectie):
@@ -274,9 +266,59 @@
 class HPICollectie(Collectie):
     zekerheidsstellingen: Optional[List[FieldZekerheidsstelling]] = None
     overig_betrokken_kadastraal_objecten: Optional[
         List[OverigBetrokkenKadastraalObject]
     ] = Field(None, alias="overigBetrokkenKadastraalObjecten")
 
 
-class EigendomsinformatieProduct(Product):
-    met: Optional[EDICollectie] = None
+class ATCollectie(BaseModel):
+    adres_locaties: Optional[List[FieldAdresLocatie]] = Field(
+        None, alias="adresLocaties"
+    )
+    gevraagd_gebied: Optional[GevraagdGebied] = Field(None, alias="gevraagdGebied")
+    locatie_kadastraal_objecten: Optional[List[LocatieKadastraalObject]] = Field(
+        None, alias="locatieKadastraalObjecten"
+    )
+    onroerende_zaken: Optional[List[FieldOnroerendeZaak]] = Field(
+        None, alias="onroerendeZaken"
+    )
+
+
+class SignaleringPersoon(BaseModel):
+    ten_behoeve_van: Optional[List[NEN3610ID]] = Field(None, alias="tenBehoeveVan")
+    van: Optional[NEN3610ID] = None
+
+
+class AttenderingPersoon(BaseModel):
+    van: Optional[NEN3610ID] = None
+    ten_behoeve_van: Optional[List[NEN3610ID]] = Field(
+        None, alias="tenBehoeveVan", title="tenBehoeveVan"
+    )
+
+
+class EGICollectie(Collectie):
+    erfpachtcanons: Optional[List[Erfpachtcanon]] = None
+    gezamenlijk_aandelen: Optional[List[GezamenlijkAandeel]] = Field(
+        None, alias="gezamenlijkAandelen"
+    )
+    mandeligheden: Optional[List[Mandeligheid]] = None
+    tenaamstellingen: Optional[List[Tenaamstelling]] = None
+    appartementsrecht_splitsingen: Optional[List[AppartementsrechtSplitsing]] = Field(
+        None, alias="appartementsrechtSplitsingen"
+    )
+    publiekrechtelijke_beperkingen: Optional[List[PubliekrechtelijkeBeperking]] = Field(
+        None, alias="publiekrechtelijkeBeperkingen"
+    )
+    beperkingsgebieden: Optional[List[Beperkingsgebied]] = None
+    zakelijk_rechten: Optional[List[ZakelijkRecht]] = Field(
+        None, alias="zakelijkRechten"
+    )
+    attendering_personen: Optional[List[AttenderingPersoon]] = Field(
+        None, alias="attenderingPersonen"
+    )
+    signalering_personen: Optional[List[SignaleringPersoon]] = Field(
+        None, alias="signaleringPersonen"
+    )
+    verkavel_objecten: Optional[List[VerkavelObject]] = Field(
+        None, alias="verkavelObjecten"
+    )
+    herverkavelingsgebieden: Optional[List[Herverkavelingsgebied]] = None
```

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/models/eigendomsinformatie.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/eigendomsinformatie.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/models/enum.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,57 +2,57 @@
 
 
 class PersoonTypeEnum(str, Enum):
     NATUURLIJK_PERSOON = "NatuurlijkPersoon"
     NIET_NATUURLIJK_PERSOON = "NietNatuurlijkPersoon"
 
 
-class AdresLocatieTypeEnum(Enum):
+class AdresLocatieTypeEnum(str, Enum):
     OBJECTLOCATIE_BINNENLAND = "ObjectlocatieBinnenland"
     OBJECTLOCATIE_BUITENLAND = "ObjectlocatieBuitenland"
     POSTBUS_LOCATIE = "PostbusLocatie"
 
 
-class AppartementsrechtSplitsingTypeEnum(Enum):
+class AppartementsrechtSplitsingTypeEnum(str, Enum):
     HOOFSPLITSING = "Hoofsplitsing"
     ONDERSPLITSING = "Ondersplitsing"
     SPIEGELSPLITSING_ONDERSPLITSING = "SpiegelsplitsingOndersplitsing"
     SPIEGELSPLITSING_AFKOOP_ERFPACHT = "SpiegelsplitsingAfkoopErfpacht"
 
 
-class Formaat(Enum):
+class Formaat(str, Enum):
     JSON = "json"
     PDF = "pdf"
     JSON_PDF = "json,pdf"
     PDF_JSON = "pdf,json"
 
 
-class SeverityCode(Enum):
+class SeverityCode(str, Enum):
     INFO = "INFO"
     WARNING = "WARNING"
     ERROR = "ERROR"
     FATAL = "FATAL"
 
 
-class ObjectReferentieType(Enum):
+class ObjectReferentieType(str, Enum):
     BAG = "BAG"
     BGT = "BGT"
 
 
-class OnroerendeZaakTypeEnum(Enum):
+class OnroerendeZaakTypeEnum(str, Enum):
     PERCEEL = "Perceel"
     APPARTEMENTSRECHT = "Appartementsrecht"
     LEIDINGNETWERK = "Leidingnetwerk"
 
 
-class StukTypeEnum(Enum):
+class StukTypeEnum(str, Enum):
     TER_INSCHRIJVING_AANGEBODEN_STUK = "TerInschrijvingAangebodenStuk"
     KADASTERSTUK = "Kadasterstuk"
 
 
-class ZekerheidsstellingTypeEnum(Enum):
+class ZekerheidsstellingTypeEnum(str, Enum):
     ZEKERHEIDSSTELLING_HYPOTHECAIR = "ZekerheidsstellingHypothecair"
     ZEKERHEIDSSTELLING_INZAKE_BESLAG = "ZekerheidsstellingInzakeBeslag"
 
 
-class Type(Enum):
+class Type(str, Enum):
     POINT = "Point"
```

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/models/misc.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/misc.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/models/persoon.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/persoon.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/models/stukken.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/stukken.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,67 @@
 from datetime import date
 from datetime import datetime
 from typing import List
+from typing import Literal
 from typing import Optional
+from typing import Union
 
 from pydantic import BaseModel
 from pydantic import Field
+from typing_extensions import Annotated
 
 from .enum import StukTypeEnum
 from .misc import NEN3610ID
 from .misc import Waardelijst
 
 
-class FieldStuk(BaseModel):
-    identificatie: Optional[NEN3610ID] = None
-    type: Optional[StukTypeEnum] = None
-    toelichting_bewaarder: Optional[str] = Field(None, alias="toelichtingBewaarder")
-    omvat: Optional[List[NEN3610ID]] = None
-
-
 class PortefeuilleId(BaseModel):
     akr_registercode: Optional[Waardelijst] = Field(None, alias="akrRegistercode")
     akr_stukdeel1: Optional[str] = Field(None, alias="akrStukdeel1")
     akr_stukdeel2: Optional[str] = Field(None, alias="akrStukdeel2")
     akr_stukdeel3: Optional[str] = Field(None, alias="akrStukdeel3")
     volgnummer_staat75: Optional[int] = Field(None, alias="volgnummerStaat75")
 
 
-class Kadasterstuk(FieldStuk):
-    portefeuillenummer: Optional[PortefeuilleId] = None
-
-
 class TypeDeelEnNummer(BaseModel):
     deel: Optional[str] = None
     nummer: Optional[str] = None
     reeks: Optional[Waardelijst] = None
     registercode: Optional[Waardelijst] = None
     soort_register: Optional[Waardelijst] = Field(None, alias="soortRegister")
 
 
 class Tijdstip(BaseModel):
     datum: date
-    tijd: datetime
+    tijd: Optional[datetime] = None
+
+
+class FieldStuk(BaseModel):
+    identificatie: Optional[NEN3610ID] = None
+    type: Optional[StukTypeEnum] = None
+    toelichting_bewaarder: Optional[str] = Field(None, alias="toelichtingBewaarder")
+    omvat: Optional[List[NEN3610ID]] = None
+
+
+class Kadasterstuk(FieldStuk):
+    type: Literal[StukTypeEnum.KADASTERSTUK] = StukTypeEnum.KADASTERSTUK
+    portefeuillenummer: Optional[PortefeuilleId] = None
 
 
 class TerInschrijvingAangebodenStuk(FieldStuk):
+    type: Literal[
+        StukTypeEnum.TER_INSCHRIJVING_AANGEBODEN_STUK
+    ] = StukTypeEnum.TER_INSCHRIJVING_AANGEBODEN_STUK
     aard: Optional[Waardelijst] = None
     deel_en_nummer: Optional[TypeDeelEnNummer] = Field(None, alias="deelEnNummer")
     heeft_kadaster_verzoek: Optional[bool] = Field(None, alias="heeftKadasterVerzoek")
     status_stuk_or: Optional[Waardelijst] = Field(None, alias="statusStukOR")
     tekening_ingeschreven: Optional[bool] = Field(None, alias="tekeningIngeschreven")
     tijdstip_aanbieding: Optional[Tijdstip] = Field(None, alias="tijdstipAanbieding")
     tijdstip_ondertekening: Optional[Tijdstip] = Field(
         None, alias="tijdstipOndertekening"
     )
+
+
+FieldType = Annotated[
+    Union[Kadasterstuk, TerInschrijvingAangebodenStuk], Field(discriminator="type")
+]
```

### Comparing `kadaster_kikinzage_client-0.1.3/src/kikinzage/models/zekerheid.py` & `kadaster_kikinzage_client-0.1.4/src/kikinzage/models/zekerheid.py`

 * *Files identical despite different names*

### Comparing `kadaster_kikinzage_client-0.1.3/PKG-INFO` & `kadaster_kikinzage_client-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kadaster-kikinzage-client
-Version: 0.1.3
+Version: 0.1.4
 Summary:  Kadaster - KIK Inzage API Python client
 Home-page: https://github.com/foarsitter/kadaster-kik-inzage-api-python-client
 License: MIT
 Author: Jelmer Draaijer
 Author-email: info@jelmert.nl
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
```

