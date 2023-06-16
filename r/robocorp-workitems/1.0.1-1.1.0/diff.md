# Comparing `tmp/robocorp_workitems-1.0.1.tar.gz` & `tmp/robocorp_workitems-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_workitems-1.0.1.tar", max compression
+gzip compressed data, was "robocorp_workitems-1.1.0.tar", max compression
```

## Comparing `robocorp_workitems-1.0.1.tar` & `robocorp_workitems-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5629 2023-06-13 15:07:46.458620 robocorp_workitems-1.0.1/README.md
--rw-r--r--   0        0        0      817 2023-06-13 15:07:46.458620 robocorp_workitems-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4980 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/__init__.py
--rw-r--r--   0        0        0    17330 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_adapters.py
--rw-r--r--   0        0        0     2380 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_context.py
--rw-r--r--   0        0        0      958 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_exceptions.py
--rw-r--r--   0        0        0     6520 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_requests.py
--rw-r--r--   0        0        0     1558 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_types.py
--rw-r--r--   0        0        0     2331 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_utils.py
--rw-r--r--   0        0        0     8652 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_workitem.py
--rw-r--r--   0        0        0        0 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/py.typed
--rw-r--r--   0        0        0     6265 1970-01-01 00:00:00.000000 robocorp_workitems-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5629 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/README.md
+-rw-r--r--   0        0        0      817 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4980 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/__init__.py
+-rw-r--r--   0        0        0    17330 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_adapters.py
+-rw-r--r--   0        0        0     2380 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_context.py
+-rw-r--r--   0        0        0      958 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_exceptions.py
+-rw-r--r--   0        0        0     6520 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_requests.py
+-rw-r--r--   0        0        0     1657 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_types.py
+-rw-r--r--   0        0        0     2331 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_utils.py
+-rw-r--r--   0        0        0     8789 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/_workitem.py
+-rw-r--r--   0        0        0        0 2023-06-16 11:14:21.074686 robocorp_workitems-1.1.0/src/robocorp/workitems/py.typed
+-rw-r--r--   0        0        0     6265 1970-01-01 00:00:00.000000 robocorp_workitems-1.1.0/PKG-INFO
```

### Comparing `robocorp_workitems-1.0.1/README.md` & `robocorp_workitems-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.1/pyproject.toml` & `robocorp_workitems-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-workitems"
-version = "1.0.1"
+version = "1.1.0"
 description = "Robocorp Work Items library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
     "Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
```

### Comparing `robocorp_workitems-1.0.1/src/robocorp/workitems/__init__.py` & `robocorp_workitems-1.1.0/src/robocorp/workitems/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     BusinessException,
     EmptyQueue,
     to_exception_type,
 )
 from ._types import ExceptionType, JSONType, State
 from ._workitem import Input, Output
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 LOGGER = logging.getLogger(__name__)
 
 
 @task_cache
 def __ctx():
```

### Comparing `robocorp_workitems-1.0.1/src/robocorp/workitems/_adapters.py` & `robocorp_workitems-1.1.0/src/robocorp/workitems/_adapters.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.1/src/robocorp/workitems/_context.py` & `robocorp_workitems-1.1.0/src/robocorp/workitems/_context.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.1/src/robocorp/workitems/_exceptions.py` & `robocorp_workitems-1.1.0/src/robocorp/workitems/_exceptions.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.1/src/robocorp/workitems/_requests.py` & `robocorp_workitems-1.1.0/src/robocorp/workitems/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.1/src/robocorp/workitems/_types.py` & `robocorp_workitems-1.1.0/src/robocorp/workitems/_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,24 +39,26 @@
     """Container for Email attached to work item."""
 
     # Unable to use "from" as attribute as it is a reserved word
     from_: Address = field(metadata=config(field_name="from"))
     to: list[Address]
     cc: list[Address]
     bcc: list[Address]
-    reply_to: Address
 
     subject: str
     date: datetime = field(
         metadata={
             "dataclasses_json": {
                 "encoder": datetime.isoformat,
                 "decoder": isoparse,
                 "mm_field": fields.DateTime(format="iso"),
             }
         }
     )
 
+    # NB (2023-06-16): Documented as non-optional, but seems to be missing in CR
+    reply_to: Optional[Address] = None
+
     text: Optional[str] = None
     html: Optional[str] = None
 
     errors: list[str] = field(default_factory=list)
```

### Comparing `robocorp_workitems-1.0.1/src/robocorp/workitems/_utils.py` & `robocorp_workitems-1.1.0/src/robocorp/workitems/_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.1/src/robocorp/workitems/_workitem.py` & `robocorp_workitems-1.1.0/src/robocorp/workitems/_workitem.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,50 +81,53 @@
     def email(
         self,
         html=True,
         encoding="utf-8",
         ignore_errors=False,
     ) -> Optional[Email]:
         email = self._parse_email()
-        if email is None:
-            raise ValueError("No email in work item")
 
         if email.errors and not ignore_errors:
             raise ValueError("\n".join(email.errors))
 
         if html and "__mail.html" in self._files:
             content = self._adapter.get_file(self.id, "__mail.html")
             email.html = content.decode(encoding)
 
         return email
 
-    def _parse_email(self) -> Optional[Email]:
+    def _parse_email(self) -> Email:
         if not isinstance(self._payload, dict):
-            return None
+            typename = type(self._payload).__name__
+            raise ValueError(f"Expected 'dict' payload, was '{typename}'")
 
-        # Email was successfully parsed by Control Room
-        if "email" in self._payload:
+        def _try_parse(fields):
             try:
-                fields = self._payload["email"]
                 email = Email.from_dict(fields)  # type: ignore
                 return email
-            except Exception as exc:
-                LOGGER.warning("Malformed 'email' field: %s", exc)
+            except KeyError as err:
+                raise ValueError(f"Missing key in 'email' field: {err}") from err
+            except Exception as err:
+                raise ValueError(f"Malformed 'email' field: {err}") from err
+
+        # Email was successfully parsed by Control Room
+        if "email" in self._payload:
+            fields = self._payload["email"]
+            email = _try_parse(fields)
+            return email
 
         # Email parsing by Control Room failed (payload or attachments too big)
         if "failedEmail" in self._payload:
-            try:
-                fields = self._payload["failedEmail"]
-                email = Email.from_dict(fields)  # type: ignore
-                email.errors = self._parse_email_errors(self._payload)
-                return email
-            except Exception as exc:
-                LOGGER.warning("Malformed 'failedEmail' field: %s", exc)
+            fields = self._payload["failedEmail"]
+            email = _try_parse(fields)
+            email.errors = self._parse_email_errors(self._payload)
+            return email
 
-        return None
+        # No email fields in payload
+        raise ValueError("No email in work item")
 
     def _parse_email_errors(self, payload: dict[str, Any]) -> list[str]:
         errors = payload.get("errors", [])
         if not isinstance(errors, list):
             LOGGER.warning("Expected 'errors' as 'list', was '%s'", type(errors))
             return []
```

### Comparing `robocorp_workitems-1.0.1/PKG-INFO` & `robocorp_workitems-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-workitems
-Version: 1.0.1
+Version: 1.1.0
 Summary: Robocorp Work Items library
 Author: Ossi R.
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

