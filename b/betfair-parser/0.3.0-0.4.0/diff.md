# Comparing `tmp/betfair_parser-0.3.0.tar.gz` & `tmp/betfair_parser-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.3.0.tar", max compression
+gzip compressed data, was "betfair_parser-0.4.0.tar", max compression
```

## Comparing `betfair_parser-0.3.0.tar` & `betfair_parser-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0     1286 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      614 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/__init__.py
--rw-r--r--   0        0        0     2038 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/client.py
--rw-r--r--   0        0        0     2417 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/endpoints.py
--rw-r--r--   0        0        0      741 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0       85 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3177 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    11161 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0       84 2023-06-01 21:25:17.604660 betfair_parser-0.3.0/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    21951 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9634 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8860 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    32756 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0      238 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/__init__.py
--rw-r--r--   0        0        0     9826 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/enums.py
--rw-r--r--   0        0        0     6202 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/messages.py
--rw-r--r--   0        0        0     1526 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/type_definitions.py
--rw-r--r--   0        0        0      279 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/common/types.py
--rw-r--r--   0        0        0     2773 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     8653 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/identity.py
--rw-r--r--   0        0        0     3662 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     3172 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      399 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     5989 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2247 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2507 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2319 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/strenums.py
--rw-r--r--   0        0        0      902 2023-06-01 21:25:17.608660 betfair_parser-0.3.0/betfair_parser/util.py
--rw-r--r--   0        0        0     1731 2023-06-01 21:25:32.448697 betfair_parser-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 betfair_parser-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1286 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3277 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/__init__.py
+-rw-r--r--   0        0        0     2038 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/client.py
+-rw-r--r--   0        0        0     2417 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/endpoints.py
+-rw-r--r--   0        0        0      741 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3177 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11161 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0       84 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    21951 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9634 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8860 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    32688 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0      238 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/common/__init__.py
+-rw-r--r--   0        0        0     9771 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/common/enums.py
+-rw-r--r--   0        0        0     4716 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/common/messages.py
+-rw-r--r--   0        0        0     1493 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/common/type_definitions.py
+-rw-r--r--   0        0        0     2773 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     8653 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/identity.py
+-rw-r--r--   0        0        0     3645 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     3172 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      399 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     5989 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2247 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2507 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2319 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      902 2023-06-16 04:54:09.546226 betfair_parser-0.4.0/betfair_parser/util.py
+-rw-r--r--   0        0        0     1731 2023-06-16 04:54:28.902370 betfair_parser-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 betfair_parser-0.4.0/PKG-INFO
```

### Comparing `betfair_parser-0.3.0/LICENSE.txt` & `betfair_parser-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/client.py` & `betfair_parser-0.4.0/betfair_parser/client.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/endpoints.py` & `betfair_parser-0.4.0/betfair_parser/endpoints.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/exceptions.py` & `betfair_parser-0.4.0/betfair_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.4.0/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.4.0/betfair_parser/spec/accounts/operations.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.4.0/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.4.0/betfair_parser/spec/betting/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.4.0/betfair_parser/spec/betting/listings.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.4.0/betfair_parser/spec/betting/orders.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.4.0/betfair_parser/spec/betting/type_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     CustomerOrderRef,
     CustomerRef,
     CustomerStrategyRef,
     Date,
     EventId,
     EventTypeId,
     ExchangeId,
-    FloatStr,
     Handicap,
-    IntStr,
     MarketId,
     MatchId,
     OrderStatus,
     OrderType,
     Price,
     SelectionId,
     Size,
@@ -245,44 +243,44 @@
     # Yes, this is the only type definition, that has (mostly) uppered key names
     """
     Runner metadata as defined in the API as additional information.
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Additional+Information
     """
 
     weight_units: Optional[str] = None  # The unit of weight used.
-    adjusted_rating: Optional[IntStr] = None  # Race-specific ratings that reflect weights allocated in the race
-    dam_year_born: Optional[IntStr] = None  # The year the horse’s mother's birth
-    days_since_last_run: Optional[IntStr] = None  # The number of days since the horse last ran
+    adjusted_rating: Optional[int] = None  # Race-specific ratings that reflect weights allocated in the race
+    dam_year_born: Optional[int] = None  # The year the horse’s mother's birth
+    days_since_last_run: Optional[int] = None  # The number of days since the horse last ran
     wearing: Optional[str] = None  # Any extra equipment the horse is wearing
-    damsire_year_born: Optional[IntStr] = None  # Year in which the horse's grandfather was born on its mother's side
+    damsire_year_born: Optional[int] = None  # Year in which the horse's grandfather was born on its mother's side
     sire_bred: Optional[_MetaCountryCode] = None  # The country where the horse's father was bred
     trainer_name: Optional[str] = None  # The name of the horse's trainer
-    stall_draw: Optional[IntStr] = None  # The stall number the horse is starting from
+    stall_draw: Optional[int] = None  # The stall number the horse is starting from
     sex_type: Optional[str] = None  # The sex of the horse
     owner_name: Optional[str] = None  # The owner of the horse
     sire_name: Optional[str] = None  # The name of the horse's father
-    forecastprice_numerator: Optional[IntStr] = None  # The forecast price numerator
-    forecastprice_denominator: Optional[IntStr] = None  # The forecast price denominator
-    jockey_claim: Optional[IntStr] = None  # Reduction in the weight that the horse carries for a particular jockey
-    weight_value: Optional[FloatStr] = None  # The weight of the horse
+    forecastprice_numerator: Optional[int] = None  # The forecast price numerator
+    forecastprice_denominator: Optional[int] = None  # The forecast price denominator
+    jockey_claim: Optional[int] = None  # Reduction in the weight that the horse carries for a particular jockey
+    weight_value: Optional[float] = None  # The weight of the horse
     dam_name: Optional[str] = None  # The name of the horse's mother
-    age: Optional[IntStr] = None  # The age of the horse
+    age: Optional[int] = None  # The age of the horse
     colour_type: Optional[str] = None  # The colour of the horse
     damsire_bred: Optional[_MetaCountryCode] = None  # The country where the horse's grandfather was born
     damsire_name: Optional[str] = None  # The name of the horse's grandfather
-    sire_year_born: Optional[IntStr] = None  # The year the horse's father was born
-    official_rating: Optional[IntStr] = None  # The horses official rating
+    sire_year_born: Optional[int] = None  # The year the horse's father was born
+    official_rating: Optional[int] = None  # The horses official rating
     form: Optional[str] = None  # The horses recent form
     bred: Optional[_MetaCountryCode] = None  # The country in which the horse was born
-    runner_id: Optional[IntStr] = msgspec.field(name="runnerId", default=None)  # The runnerId for the horse
+    runner_id: Optional[int] = msgspec.field(name="runnerId", default=None)  # The runnerId for the horse
     jockey_name: Optional[str] = None  # Name of the jockey. This field will contain 'Reserve' if its a reserve runner
     dam_bred: Optional[_MetaCountryCode] = None  # The country where the horse's mother was born
     colours_description: Optional[str] = None  # The textual description of the jockey silk
     colours_filename: Optional[str] = None  # Image representing the jockey silk
-    cloth_number: Optional[IntStr] = None  # The number on the saddle-cloth
+    cloth_number: Optional[int] = None  # The number on the saddle-cloth
     cloth_number_alpha: Optional[str] = None  # The number on the saddle cloth for US paired runners, e.g. "1A"
 
     @property
     def colours_url(self):
         if self.colours_filename:
             return SILKS + self.colours_filename
```

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/common/enums.py` & `betfair_parser-0.4.0/betfair_parser/spec/common/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from enum import Enum
 
-from betfair_parser.spec.common.types import IntStr
 from betfair_parser.strenums import DocumentedEnum, LowerStrEnum, StrEnum, auto, doc
 
 
 class EndpointType(LowerStrEnum):
     IDENTITY = auto()
     IDENTITY_CERT = auto()
     NAVIGATION = auto()
@@ -129,15 +128,15 @@
     INVALID_GRANT_TYPE = doc(
         "The vendor making the request has not provided a valid grant_type, or the grant_type they have "
         "passed does not match the parameters (authCode/refreshToken)."
     )
     CUSTOMER_ACCOUNT_CLOSED = doc("A token could not be created because the customer's account is CLOSED.")
 
 
-class EventTypeIdCode(IntStr, Enum):
+class EventTypeIdCode(int, Enum):
     """Unique identifier for event types
 
     This is not a complete list and only serves for ease of use. For a full list, use the ListEventTypes API call.
 
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Additional+Information?preview=/43090178/43090179/EventTypIds.xlsx
     """
```

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/common/messages.py` & `betfair_parser-0.4.0/betfair_parser/spec/common/messages.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,30 @@
-from typing import Generic, Literal, Optional, TypeVar
+from typing import Any, Generic, Literal, Optional, TypeVar
 
 import msgspec
 
 from betfair_parser.exceptions import APINGException, JSONError
 from betfair_parser.spec.common.enums import (
     AccountAPINGExceptionCode,
     APINGExceptionCode,
     EndpointType,
     JSONExceptionCode,
 )
-from betfair_parser.spec.common.types import FloatStr, IntStr
 
 
-def encode_quoted(obj):
-    """Encode int and float subtypes as ordinary ints and floats."""
-    if isinstance(obj, int):
-        return int(obj)
-    if isinstance(obj, float):
-        return float(obj)
-    raise TypeError(f"Unencodable type: {type(obj).__name__}: {obj}")
-
-
-def decode_quoted(type_, obj):
-    """
-    Betfair uses JSON formatting inconsistently. For requests to their API they
-    format int and float values in all of their examples as '"123"' and '"5.5"',
-    even if those quotation marks aren't necessary and violate JSON
-    specification. It also occasionally returns "'null'" instead of a null value.
-
-    This decoding hook gets rid of any quotation marks and restores the original
-    data type. Unfortunately we can't use plain int and float, but need to define
-    a subclass of them, so that the dec_hook can do its job.
-    """
-    if type_ is IntStr:
-        if isinstance(obj, int):
-            return IntStr(obj)
-        if obj == "null":
-            return IntStr(0)
-        return IntStr(obj.strip("'\" "))
-    if type_ is FloatStr:
-        if isinstance(obj, (float, int)):
-            return FloatStr(obj)
-        if obj == "null":
-            return FloatStr("nan")
-        return FloatStr(obj.strip("'\" "))
-    raise TypeError(f"Undecodable type: {type(obj).__name__}: {obj}. Expected type: {type_.__name__}")
-
-
-def decode(raw, type=None):
+def decode(raw: bytes, type: Any = Any) -> Any:
     try:
-        if type is None:
-            return msgspec.json.decode(raw, dec_hook=decode_quoted)
-        return msgspec.json.decode(raw, type=type, dec_hook=decode_quoted)
+        return msgspec.json.decode(raw, strict=False, type=type)  # type: ignore
     except msgspec.DecodeError as e:
         raise JSONError(str(e)) from e
 
 
-def encode(data):
+def encode(data: Any) -> bytes:
     try:
-        return msgspec.json.encode(data, enc_hook=encode_quoted)
+        return msgspec.json.encode(data)
     except msgspec.EncodeError as e:
         raise JSONError(str(e)) from e
 
 
 class BaseMessage(msgspec.Struct, kw_only=True, forbid_unknown_fields=True, frozen=True, rename="camel"):
     @classmethod
     def parse(cls, raw):
```

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/common/type_definitions.py` & `betfair_parser-0.4.0/betfair_parser/spec/common/type_definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import datetime
 from typing import Annotated, Optional, Union
 
 import msgspec
 
-from betfair_parser.spec.common.messages import BaseMessage, FloatStr, IntStr
+from betfair_parser.spec.common.messages import BaseMessage
 
 
 # Type aliases with minimalistic validation. More would be great.
 
 Date = Annotated[datetime.datetime, msgspec.Meta(title="Date", tz=True)]
-SelectionId = Annotated[IntStr, msgspec.Meta(title="SelectionId")]
+SelectionId = Annotated[int, msgspec.Meta(title="SelectionId")]
 Venue = Annotated[str, msgspec.Meta(title="Venue")]
 MarketId = Annotated[str, msgspec.Meta(title="MarketId")]
-Handicap = Annotated[FloatStr, msgspec.Meta(title="Handicap")]
+Handicap = Annotated[float, msgspec.Meta(title="Handicap")]
 EventId = Annotated[str, msgspec.Meta(title="EventId")]
-EventTypeId = Annotated[IntStr, msgspec.Meta(title="EventTypeId")]
+EventTypeId = Annotated[int, msgspec.Meta(title="EventTypeId")]
 CountryCode = Annotated[str, msgspec.Meta(title="CountryCode", min_length=2, max_length=3)]
 ExchangeId = Annotated[str, msgspec.Meta(title="ExchangeId")]
 CompetitionId = Annotated[str, msgspec.Meta(title="CompetitionId")]
-Price = Annotated[FloatStr, msgspec.Meta(title="Price")]
-Size = Annotated[FloatStr, msgspec.Meta(title="Size")]
+Price = Annotated[float, msgspec.Meta(title="Price")]
+Size = Annotated[float, msgspec.Meta(title="Size")]
 BetId = Annotated[Union[str, int], msgspec.Meta(title="BetId")]
 MatchId = Annotated[Union[str, int], msgspec.Meta(title="MatchId")]
 CustomerRef = Annotated[Union[str, int], msgspec.Meta(title="CustomerRef")]
 CustomerOrderRef = Annotated[Union[str, int], msgspec.Meta(title="CustomerOrderRef")]
 CustomerStrategyRef = Annotated[Union[str, int], msgspec.Meta(title="CustomerStrategyRef")]
```

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.4.0/betfair_parser/spec/heartbeat.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/identity.py` & `betfair_parser-0.4.0/betfair_parser/spec/identity.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/navigation.py` & `betfair_parser-0.4.0/betfair_parser/spec/navigation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import Literal, Optional, Union
 
-from betfair_parser.spec.common import BaseMessage, BaseResponse, Date, EndpointType, IntStr, Request
+from betfair_parser.spec.common import BaseMessage, BaseResponse, Date, EndpointType, Request
 
 
 def tag_func(s: str):
     """
     >>> tag_func("EventType")
     'EVENT_TYPE'
 
@@ -22,15 +22,15 @@
     market_type: str
     market_start_time: Date
     number_of_winners: Union[int, str]
 
 
 class Event(BaseMessage, tag=tag_func, frozen=True):
     name: str
-    id: IntStr
+    id: int
     country_code: str
     children: list[Union["Group", "Event", Market]]
 
 
 class Race(BaseMessage, tag=tag_func, frozen=True):
     name: str
     id: str
@@ -45,15 +45,15 @@
     name: str
     id: str
     children: list[Union["Group", Event]]
 
 
 class EventType(BaseMessage, tag=tag_func, frozen=True):
     name: str
-    id: IntStr
+    id: int
     children: list[Union[Group, Event, Race]]
 
 
 class Navigation(BaseResponse, frozen=True):
     """Navigation root"""
 
     type: Literal["GROUP"]
@@ -77,15 +77,15 @@
     method = ""
     id: int = 0
     return_type = Navigation  # type: ignore
 
 
 class FlattenedMarket(BaseMessage, kw_only=True, frozen=True, rename=None):
     event_type_name: str
-    event_type_id: IntStr
+    event_type_id: int
     event_name: Optional[str] = None
     event_id: Optional[str] = None
     event_country_code: Optional[str] = None
     market_name: str
     market_id: str
     market_exchange_id: str
     market_market_type: str
```

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/race_status.py` & `betfair_parser-0.4.0/betfair_parser/spec/race_status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.4.0/betfair_parser/spec/streaming/mcm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.4.0/betfair_parser/spec/streaming/ocm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.4.0/betfair_parser/spec/streaming/status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/strenums.py` & `betfair_parser-0.4.0/betfair_parser/strenums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/betfair_parser/util.py` & `betfair_parser-0.4.0/betfair_parser/util.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.3.0/pyproject.toml` & `betfair_parser-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
     "Topic :: File Formats :: JSON",
     "Development Status :: 4 - Beta",
 ]
 keywords = ["parser", "betfair", "api", "json", "streaming"]
 dependencies = [
-    "msgspec>=0.15.1",
+    "msgspec>=0.16.0",
     "fsspec>=2022",
 ]
 
 [project.urls]
 Homepage = "https://github.com/limx0/betfair_parser"
 Documentation = "https://limx0.github.io/betfair_parser/"
 "Bug Tracker" = "https://github.com/limx0/betfair_parser/issues"
@@ -37,22 +37,22 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "betfair_parser"
-version = "0.3.0"
+version = "0.4.0"
 description = "A betfair parser"
 readme = "README.md"
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-msgspec = "^0.15.1"
+msgspec = "^0.16.0"
 fsspec = ">=2022"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 pytest-benchmark = "^4.0"
 requests = "^2.20"
```

