# Comparing `tmp/gundi_core-1.0.0.tar.gz` & `tmp/gundi_core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_core-1.0.0.tar", max compression
+gzip compressed data, was "gundi_core-1.0.1.tar", max compression
```

## Comparing `gundi_core-1.0.0.tar` & `gundi_core-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       40 2023-06-14 17:07:47.722189 gundi_core-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-06-14 20:35:09.913772 gundi_core-1.0.0/gundi_core/__init__.py
--rw-r--r--   0        0        0      114 2023-06-14 18:33:55.875739 gundi_core-1.0.0/gundi_core/schemas/__init__.py
--rw-r--r--   0        0        0    13847 2023-06-14 19:41:05.310697 gundi_core-1.0.0/gundi_core/schemas/v1.py
--rw-r--r--   0        0        0     3718 2023-06-15 15:37:41.088621 gundi_core-1.0.0/gundi_core/schemas/v2.py
--rw-r--r--   0        0        0      329 2023-06-14 18:54:36.408865 gundi_core-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       40 2023-06-14 17:07:47.722189 gundi_core-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 20:35:09.913772 gundi_core-1.0.1/gundi_core/__init__.py
+-rw-r--r--   0        0        0      114 2023-06-14 18:33:55.875739 gundi_core-1.0.1/gundi_core/schemas/__init__.py
+-rw-r--r--   0        0        0    13847 2023-06-14 19:41:05.310697 gundi_core-1.0.1/gundi_core/schemas/v1.py
+-rw-r--r--   0        0        0     6070 2023-06-16 15:18:43.492464 gundi_core-1.0.1/gundi_core/schemas/v2.py
+-rw-r--r--   0        0        0      329 2023-06-16 15:27:43.940970 gundi_core-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.0.1/PKG-INFO
```

### Comparing `gundi_core-1.0.0/gundi_core/schemas/v1.py` & `gundi_core-1.0.1/gundi_core/schemas/v1.py`

 * *Files identical despite different names*

### Comparing `gundi_core-1.0.0/gundi_core/schemas/v2.py` & `gundi_core-1.0.1/gundi_core/schemas/v2.py`

 * *Files 23% similar despite different names*

```diff
@@ -107,11 +107,88 @@
     annotations: Optional[Dict[str, Any]] = Field(
         None,
         title="Annotations",
         description="A dictionary of extra data that will be passed to destination systems.",
     )
 
 
+class ConnectionOrganization(BaseModel):
+    id: Union[UUID, str] = Field(
+        None,
+        title="Organization ID",
+        description="Id of the organization owning the connection",
+    )
+    name: Optional[str] = Field(
+        "",
+        example="Wild Conservation Organization X",
+        description="Name of the organization owning this connection",
+    )
+    description: Optional[str] = Field(
+        "",
+        example="An organization in X dedicated to protect YZ..",
+        description="Description of the organization owning this connection",
+    )
+
+
+class ConnectionIntegration(BaseModel):
+    id: Union[UUID, str] = Field(
+        None,
+        title="Integration ID",
+        description="Id of an integration associated to the connection",
+    )
+    name: Optional[str] = Field(
+        "",
+        example="X Data Provider for Y Reserve",
+        description="Route name",
+    )
+    type: Optional[str] = Field(
+        "",
+        example="earth_ranger",
+        description="natural key of an integration type",
+    )
+    base_url: Optional[str] = Field(
+        "",
+        example="https://easterisland.pamdas.org/",
+        description="Base URL of the third party system associated with this integration.",
+    )
+    status: Optional[str] = Field(
+        "unknown",
+        example="healthy",
+        description="Computed status representing if the integration is working properly or not",
+    )
+
+
+class ConnectionRoute(BaseModel):
+    id: Union[UUID, str] = Field(
+        None,
+        title="Route ID",
+        description="Id of a route associated to the connection",
+    )
+    name: Optional[str] = Field(
+        "",
+        example="X Animal collars to Y",
+        description="Route name",
+    )
+
+
+class Connection(BaseModel):
+    id: Union[UUID, str] = Field(
+        None,
+        title="Connection ID",
+        description="Id of the data provider integration in the connection",
+    )
+    provider: ConnectionIntegration
+    destinations: Optional[List[ConnectionIntegration]]
+    routing_rules: Optional[List[ConnectionRoute]]
+    default_route: Optional[ConnectionRoute]
+    owner: Optional[ConnectionOrganization]
+    status: Optional[str] = Field(
+        "unknown",
+        example="healthy",
+        description="Aggregate status representing if the connection is working properly or not",
+    )
+
+
 models_by_stream_type = {
     StreamPrefixEnum.event: Event,
     StreamPrefixEnum.attachment: Attachment,
 }
```

### Comparing `gundi_core-1.0.0/PKG-INFO` & `gundi_core-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gundi-core
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: Mariano M
 Author-email: marianom@earthranger.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

