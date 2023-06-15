# Comparing `tmp/groundlight-0.8.0.tar.gz` & `tmp/groundlight-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundlight-0.8.0.tar", max compression
+gzip compressed data, was "groundlight-0.9.0.tar", max compression
```

## Comparing `groundlight-0.8.0.tar` & `groundlight-0.9.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1071 2023-05-08 18:55:30.181203 groundlight-0.8.0/LICENSE
--rw-r--r--   0        0        0     1868 2023-05-08 18:55:30.181203 groundlight-0.8.0/README.md
--rw-r--r--   0        0        0     3597 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/model.py
--rw-r--r--   0        0        0      721 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/__init__.py
--rw-r--r--   0        0        0      220 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    14018 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/api/detectors_api.py
--rw-r--r--   0        0        0    14322 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/api/image_queries_api.py
--rw-r--r--   0        0        0    35591 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/api_client.py
--rw-r--r--   0        0        0      537 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/apis/__init__.py
--rw-r--r--   0        0        0    17643 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/configuration.py
--rw-r--r--   0        0        0     4979 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/exceptions.py
--rw-r--r--   0        0        0      348 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/__init__.py
--rw-r--r--   0        0        0    11870 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/classification_result.py
--rw-r--r--   0        0        0    13623 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/detector.py
--rw-r--r--   0        0        0    13486 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/detector_creation_input.py
--rw-r--r--   0        0        0    11288 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/detector_type_enum.py
--rw-r--r--   0        0        0    13847 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/image_query.py
--rw-r--r--   0        0        0    11330 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/image_query_type_enum.py
--rw-r--r--   0        0        0    12129 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/paginated_detector_list.py
--rw-r--r--   0        0        0    12150 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/paginated_image_query_list.py
--rw-r--r--   0        0        0    11438 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model/result_type_enum.py
--rw-r--r--   0        0        0    79719 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/model_utils.py
--rw-r--r--   0        0        0     1007 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/models/__init__.py
--rw-r--r--   0        0        0    14005 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/openapi_client/rest.py
--rw-r--r--   0        0        0      955 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/setup.py
--rw-r--r--   0        0        0        0 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/__init__.py
--rw-r--r--   0        0        0      779 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_classification_result.py
--rw-r--r--   0        0        0      813 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_detector.py
--rw-r--r--   0        0        0      787 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_detector_creation_input.py
--rw-r--r--   0        0        0      752 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_detector_type_enum.py
--rw-r--r--   0        0        0      828 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_detectors_api.py
--rw-r--r--   0        0        0      864 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_image_queries_api.py
--rw-r--r--   0        0        0     1080 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_image_query.py
--rw-r--r--   0        0        0      767 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_image_query_type_enum.py
--rw-r--r--   0        0        0      872 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_paginated_detector_list.py
--rw-r--r--   0        0        0      896 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_paginated_image_query_list.py
--rw-r--r--   0        0        0      738 2023-05-08 18:55:30.189203 groundlight-0.8.0/generated/test/test_result_type_enum.py
--rw-r--r--   0        0        0     1804 2023-05-08 18:55:30.193203 groundlight-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      568 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/__init__.py
--rw-r--r--   0        0        0     2692 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/binary_labels.py
--rw-r--r--   0        0        0    11267 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/client.py
--rw-r--r--   0        0        0      271 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/config.py
--rw-r--r--   0        0        0     2135 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/images.py
--rw-r--r--   0        0        0     5759 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/internalapi.py
--rw-r--r--   0        0        0     1778 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/optional_imports.py
--rw-r--r--   0        0        0      308 2023-05-08 18:55:30.193203 groundlight-0.8.0/src/groundlight/status_codes.py
--rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 groundlight-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-15 23:03:07.003347 groundlight-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1868 2023-06-15 23:03:07.003347 groundlight-0.9.0/README.md
+-rw-r--r--   0        0        0     3557 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/model.py
+-rw-r--r--   0        0        0      752 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    14047 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/api/detectors_api.py
+-rw-r--r--   0        0        0    14351 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/api/image_queries_api.py
+-rw-r--r--   0        0        0    35605 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/api_client.py
+-rw-r--r--   0        0        0      539 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/apis/__init__.py
+-rw-r--r--   0        0        0    17676 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/configuration.py
+-rw-r--r--   0        0        0     5005 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/exceptions.py
+-rw-r--r--   0        0        0      348 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/__init__.py
+-rw-r--r--   0        0        0    11898 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/classification_result.py
+-rw-r--r--   0        0        0    13651 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/detector.py
+-rw-r--r--   0        0        0    13389 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/detector_creation_input.py
+-rw-r--r--   0        0        0    11317 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/detector_type_enum.py
+-rw-r--r--   0        0        0    13875 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/image_query.py
+-rw-r--r--   0        0        0    11359 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/image_query_type_enum.py
+-rw-r--r--   0        0        0    12157 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/paginated_detector_list.py
+-rw-r--r--   0        0        0    12178 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/paginated_image_query_list.py
+-rw-r--r--   0        0        0    11467 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model/result_type_enum.py
+-rw-r--r--   0        0        0    79730 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/model_utils.py
+-rw-r--r--   0        0        0     1009 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0    14036 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/openapi_client/rest.py
+-rw-r--r--   0        0        0     1013 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/setup.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_classification_result.py
+-rw-r--r--   0        0        0      813 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_detector.py
+-rw-r--r--   0        0        0      787 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_detector_creation_input.py
+-rw-r--r--   0        0        0      752 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_detector_type_enum.py
+-rw-r--r--   0        0        0      828 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_detectors_api.py
+-rw-r--r--   0        0        0      864 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_image_queries_api.py
+-rw-r--r--   0        0        0     1080 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_image_query.py
+-rw-r--r--   0        0        0      767 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_image_query_type_enum.py
+-rw-r--r--   0        0        0      872 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_paginated_detector_list.py
+-rw-r--r--   0        0        0      896 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_paginated_image_query_list.py
+-rw-r--r--   0        0        0      738 2023-06-15 23:03:07.015347 groundlight-0.9.0/generated/test/test_result_type_enum.py
+-rw-r--r--   0        0        0     1804 2023-06-15 23:03:07.019347 groundlight-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      568 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/__init__.py
+-rw-r--r--   0        0        0     2692 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/binary_labels.py
+-rw-r--r--   0        0        0    11410 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/client.py
+-rw-r--r--   0        0        0      271 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/config.py
+-rw-r--r--   0        0        0     2135 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/images.py
+-rw-r--r--   0        0        0     6001 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/internalapi.py
+-rw-r--r--   0        0        0     1778 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/optional_imports.py
+-rw-r--r--   0        0        0      308 2023-06-15 23:03:07.019347 groundlight-0.9.0/src/groundlight/status_codes.py
+-rw-r--r--   0        0        0     2849 1970-01-01 00:00:00.000000 groundlight-0.9.0/PKG-INFO
```

### Comparing `groundlight-0.8.0/LICENSE` & `groundlight-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/README.md` & `groundlight-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/model.py` & `groundlight-0.9.0/generated/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # generated by datamodel-codegen:
 #   filename:  public-api.yaml
-#   timestamp: 2022-07-30T20:30:21+00:00
+#   timestamp: 2023-05-26T20:07:17+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional
 
 from pydantic import AnyUrl, BaseModel, Field, confloat, constr
 
 
 class ClassificationResult(BaseModel):
     confidence: Optional[confloat(ge=0.0, le=1.0)] = Field(
-        None,
-        description="On a scale of 0 to 1, how confident are we in the predicted label?",
+        None, description="On a scale of 0 to 1, how confident are we in the predicted label?"
     )
     label: str = Field(..., description="What is the predicted label?")
 
 
 class DetectorCreationInput(BaseModel):
     name: constr(max_length=200) = Field(..., description="A short, descriptive name for the detector.")
     query: constr(max_length=300) = Field(..., description="A question about the image.")
     group_name: Optional[constr(max_length=100)] = Field(
         None, description="Which group should this detector be part of?"
     )
     confidence_threshold: Optional[confloat(ge=0.0, le=1.0)] = Field(
         0.9,
-        description="If the detector's prediction is below this confidence threshold, send the image query for human review.",
+        description=(
+            "If the detector's prediction is below this confidence threshold, send the image query for human review."
+        ),
     )
-    config_name: Optional[constr(max_length=100)] = Field(
-        None,
-        description="(Advanced usage) If your account has multiple named ML configuration options enabled, you can use this field to specify which one you would like to use.",
+    pipeline_config: Optional[constr(max_length=8192)] = Field(
+        None, description="(Advanced usage) Configuration to instantiate a specific prediction pipeline."
     )
 
 
 class DetectorTypeEnum(Enum):
     detector = "detector"
 
 
@@ -52,15 +52,17 @@
     type: DetectorTypeEnum = Field(..., description="The type of this object.")
     created_at: datetime = Field(..., description="When this detector was created.")
     name: constr(max_length=200) = Field(..., description="A short, descriptive name for the detector.")
     query: str = Field(..., description="A question about the image.")
     group_name: str = Field(..., description="Which group should this detector be part of?")
     confidence_threshold: Optional[confloat(ge=0.0, le=1.0)] = Field(
         0.9,
-        description="If the detector's prediction is below this confidence threshold, send the image query for human review.",
+        description=(
+            "If the detector's prediction is below this confidence threshold, send the image query for human review."
+        ),
     )
 
 
 class ImageQuery(BaseModel):
     id: str = Field(..., description="A unique ID for this object.")
     type: ImageQueryTypeEnum = Field(..., description="The type of this object.")
     created_at: datetime = Field(..., description="When was this detector created?")
```

### Comparing `groundlight-0.8.0/generated/openapi_client/__init__.py` & `groundlight-0.9.0/generated/openapi_client/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# ruff: noqa
+# flake8: noqa
 
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
```

### Comparing `groundlight-0.8.0/generated/openapi_client/api/detectors_api.py` & `groundlight-0.9.0/generated/openapi_client/api/detectors_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `groundlight-0.8.0/generated/openapi_client/api/image_queries_api.py` & `groundlight-0.9.0/generated/openapi_client/api/image_queries_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `groundlight-0.8.0/generated/openapi_client/api_client.py` & `groundlight-0.9.0/generated/openapi_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -503,15 +503,15 @@
                 query_params=query_params,
                 headers=headers,
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout,
                 body=body,
             )
         else:
-            raise ApiValueError("http method must be `GET`, `HEAD`, `OPTIONS`," " `POST`, `PATCH`, `PUT` or `DELETE`.")
+            raise ApiValueError("http method must be `GET`, `HEAD`, `OPTIONS`, `POST`, `PATCH`, `PUT` or `DELETE`.")
 
     def parameters_to_tuples(self, params, collection_formats):
         """Get parameters as list of tuples, formatting collections.
 
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: Parameters as list of tuples, collections formatted
@@ -561,15 +561,15 @@
                 continue
             for file_instance in file_instances:
                 if file_instance is None:
                     # if the file field is nullable, skip None values
                     continue
                 if file_instance.closed is True:
                     raise ApiValueError(
-                        "Cannot read a closed file. The passed in file_type " "for %s must be open." % param_name
+                        "Cannot read a closed file. The passed in file_type for %s must be open." % param_name
                     )
                 filename = os.path.basename(file_instance.name)
                 filedata = self.get_file_data_and_close_file(file_instance)
                 mimetype = mimetypes.guess_type(filename)[0] or "application/octet-stream"
                 params.append(tuple([param_name, tuple([filename, filedata, mimetype])]))
 
         return params
@@ -797,29 +797,29 @@
             if self.settings["servers"]:
                 raise ApiValueError("Invalid host index. Must be 0 <= index < %s" % len(self.settings["servers"]))
             _host = None
 
         for key, value in kwargs.items():
             if key not in self.params_map["all"]:
                 raise ApiTypeError(
-                    "Got an unexpected parameter '%s'" " to method `%s`" % (key, self.settings["operation_id"])
+                    "Got an unexpected parameter '%s' to method `%s`" % (key, self.settings["operation_id"])
                 )
             # only throw this nullable ApiValueError if _check_input_type
             # is False, if _check_input_type==True we catch this case
             # in self.__validate_inputs
             if key not in self.params_map["nullable"] and value is None and kwargs["_check_input_type"] is False:
                 raise ApiValueError(
-                    "Value may not be None for non-nullable parameter `%s`"
-                    " when calling `%s`" % (key, self.settings["operation_id"])
+                    "Value may not be None for non-nullable parameter `%s` when calling `%s`"
+                    % (key, self.settings["operation_id"])
                 )
 
         for key in self.params_map["required"]:
             if key not in kwargs.keys():
                 raise ApiValueError(
-                    "Missing the required parameter `%s` when calling " "`%s`" % (key, self.settings["operation_id"])
+                    "Missing the required parameter `%s` when calling `%s`" % (key, self.settings["operation_id"])
                 )
 
         self.__validate_inputs(kwargs)
 
         params = self.__gather_params(kwargs)
 
         accept_headers_list = self.headers_map["accept"]
```

### Comparing `groundlight-0.8.0/generated/openapi_client/apis/__init__.py` & `groundlight-0.9.0/generated/openapi_client/apis/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ruff: noqa
+# flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
 #   from .api.detectors_api import DetectorsApi
```

### Comparing `groundlight-0.8.0/generated/openapi_client/configuration.py` & `groundlight-0.9.0/generated/openapi_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -416,15 +416,15 @@
 
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
-            "Version of the API: 0.1.0\n"
+            "Version of the API: 0.6.0\n"
             "SDK Package Version: 1.0.0".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
@@ -461,28 +461,28 @@
         variables = {} if variables is None else variables
         servers = self.get_host_settings() if servers is None else servers
 
         try:
             server = servers[index]
         except IndexError:
             raise ValueError(
-                "Invalid index {0} when selecting the host settings. "
-                "Must be less than {1}".format(index, len(servers))
+                "Invalid index {0} when selecting the host settings. Must be less than {1}".format(index, len(servers))
             )
 
         url = server["url"]
 
         # go through variables and replace placeholders
         for variable_name, variable in server.get("variables", {}).items():
             used_value = variables.get(variable_name, variable["default_value"])
 
             if "enum_values" in variable and used_value not in variable["enum_values"]:
                 raise ValueError(
-                    "The variable `{0}` in the host URL has invalid value "
-                    "{1}. Must be {2}.".format(variable_name, variables[variable_name], variable["enum_values"])
+                    "The variable `{0}` in the host URL has invalid value {1}. Must be {2}.".format(
+                        variable_name, variables[variable_name], variable["enum_values"]
+                    )
                 )
 
             url = url.replace("{" + variable_name + "}", used_value)
 
         return url
 
     @property
```

### Comparing `groundlight-0.8.0/generated/openapi_client/exceptions.py` & `groundlight-0.9.0/generated/openapi_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
@@ -106,15 +106,15 @@
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
 
     def __str__(self):
         """Custom error messages for exception"""
-        error_message = "({0})\n" "Reason: {1}\n".format(self.status, self.reason)
+        error_message = "({0})\nReason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(self.headers)
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model/classification_result.py` & `groundlight-0.9.0/generated/openapi_client/model/classification_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -281,9 +281,9 @@
             ):
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(
                     f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                    f"class with read only attributes."
+                    "class with read only attributes."
                 )
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model/detector.py` & `groundlight-0.9.0/generated/openapi_client/model/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -323,9 +323,9 @@
             ):
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(
                     f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                    f"class with read only attributes."
+                    "class with read only attributes."
                 )
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model/detector_creation_input.py` & `groundlight-0.9.0/generated/openapi_client/model/detector_creation_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -66,16 +66,16 @@
         ("group_name",): {
             "max_length": 100,
         },
         ("confidence_threshold",): {
             "inclusive_maximum": 1.0,
             "inclusive_minimum": 0.0,
         },
-        ("config_name",): {
-            "max_length": 100,
+        ("pipeline_config",): {
+            "max_length": 8192,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
@@ -106,30 +106,30 @@
                 and the value is attribute type.
         """
         return {
             "name": (str,),  # noqa: E501
             "query": (str,),  # noqa: E501
             "group_name": (str,),  # noqa: E501
             "confidence_threshold": (float,),  # noqa: E501
-            "config_name": (
+            "pipeline_config": (
                 str,
                 none_type,
             ),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
     attribute_map = {
         "name": "name",  # noqa: E501
         "query": "query",  # noqa: E501
         "group_name": "group_name",  # noqa: E501
         "confidence_threshold": "confidence_threshold",  # noqa: E501
-        "config_name": "config_name",  # noqa: E501
+        "pipeline_config": "pipeline_config",  # noqa: E501
     }
 
     read_only_vars = {}
 
     _composed_schemas = {}
 
     @classmethod
@@ -170,15 +170,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             group_name (str): Which group should this detector be part of?. [optional]  # noqa: E501
             confidence_threshold (float): If the detector's prediction is below this confidence threshold, send the image query for human review.. [optional] if omitted the server will use the default value of 0.9  # noqa: E501
-            config_name (str, none_type): (Advanced usage) If your account has multiple named ML configuration options enabled, you can use this field to specify which one you would like to use.. [optional]  # noqa: E501
+            pipeline_config (str, none_type): (Advanced usage) Configuration to instantiate a specific prediction pipeline.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", False)
         _path_to_item = kwargs.pop("_path_to_item", ())
         _configuration = kwargs.pop("_configuration", None)
         _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
@@ -265,15 +265,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             group_name (str): Which group should this detector be part of?. [optional]  # noqa: E501
             confidence_threshold (float): If the detector's prediction is below this confidence threshold, send the image query for human review.. [optional] if omitted the server will use the default value of 0.9  # noqa: E501
-            config_name (str, none_type): (Advanced usage) If your account has multiple named ML configuration options enabled, you can use this field to specify which one you would like to use.. [optional]  # noqa: E501
+            pipeline_config (str, none_type): (Advanced usage) Configuration to instantiate a specific prediction pipeline.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop("_check_type", True)
         _spec_property_naming = kwargs.pop("_spec_property_naming", False)
         _path_to_item = kwargs.pop("_path_to_item", ())
         _configuration = kwargs.pop("_configuration", None)
         _visited_composed_classes = kwargs.pop("_visited_composed_classes", ())
@@ -307,9 +307,9 @@
             ):
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(
                     f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                    f"class with read only attributes."
+                    "class with read only attributes."
                 )
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model/detector_type_enum.py` & `groundlight-0.9.0/generated/openapi_client/model/detector_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model/image_query.py` & `groundlight-0.9.0/generated/openapi_client/model/image_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -341,9 +341,9 @@
             ):
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(
                     f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                    f"class with read only attributes."
+                    "class with read only attributes."
                 )
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model/image_query_type_enum.py` & `groundlight-0.9.0/generated/openapi_client/model/image_query_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model/paginated_detector_list.py` & `groundlight-0.9.0/generated/openapi_client/model/paginated_detector_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -289,9 +289,9 @@
             ):
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(
                     f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                    f"class with read only attributes."
+                    "class with read only attributes."
                 )
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model/paginated_image_query_list.py` & `groundlight-0.9.0/generated/openapi_client/model/paginated_image_query_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -289,9 +289,9 @@
             ):
                 # discard variable.
                 continue
             setattr(self, var_name, var_value)
             if var_name in self.read_only_vars:
                 raise ApiAttributeError(
                     f"`{var_name}` is a read-only attribute. Use `from_openapi_data` to instantiate "
-                    f"class with read only attributes."
+                    "class with read only attributes."
                 )
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model/result_type_enum.py` & `groundlight-0.9.0/generated/openapi_client/model/result_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `groundlight-0.8.0/generated/openapi_client/model_utils.py` & `groundlight-0.9.0/generated/openapi_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
@@ -850,56 +850,56 @@
         is_json_validation_enabled("multipleOf", configuration)
         and "multiple_of" in current_validations
         and isinstance(input_values, (int, float))
         and not (float(input_values) / current_validations["multiple_of"]).is_integer()
     ):
         # Note 'multipleOf' will be as good as the floating point arithmetic.
         raise ApiValueError(
-            "Invalid value for `%s`, value must be a multiple of "
-            "`%s`" % (input_variable_path[0], current_validations["multiple_of"])
+            "Invalid value for `%s`, value must be a multiple of `%s`"
+            % (input_variable_path[0], current_validations["multiple_of"])
         )
 
     if (
         is_json_validation_enabled("maxLength", configuration)
         and "max_length" in current_validations
         and len(input_values) > current_validations["max_length"]
     ):
         raise ApiValueError(
-            "Invalid value for `%s`, length must be less than or equal to "
-            "`%s`" % (input_variable_path[0], current_validations["max_length"])
+            "Invalid value for `%s`, length must be less than or equal to `%s`"
+            % (input_variable_path[0], current_validations["max_length"])
         )
 
     if (
         is_json_validation_enabled("minLength", configuration)
         and "min_length" in current_validations
         and len(input_values) < current_validations["min_length"]
     ):
         raise ApiValueError(
-            "Invalid value for `%s`, length must be greater than or equal to "
-            "`%s`" % (input_variable_path[0], current_validations["min_length"])
+            "Invalid value for `%s`, length must be greater than or equal to `%s`"
+            % (input_variable_path[0], current_validations["min_length"])
         )
 
     if (
         is_json_validation_enabled("maxItems", configuration)
         and "max_items" in current_validations
         and len(input_values) > current_validations["max_items"]
     ):
         raise ApiValueError(
-            "Invalid value for `%s`, number of items must be less than or "
-            "equal to `%s`" % (input_variable_path[0], current_validations["max_items"])
+            "Invalid value for `%s`, number of items must be less than or equal to `%s`"
+            % (input_variable_path[0], current_validations["max_items"])
         )
 
     if (
         is_json_validation_enabled("minItems", configuration)
         and "min_items" in current_validations
         and len(input_values) < current_validations["min_items"]
     ):
         raise ValueError(
-            "Invalid value for `%s`, number of items must be greater than or "
-            "equal to `%s`" % (input_variable_path[0], current_validations["min_items"])
+            "Invalid value for `%s`, number of items must be greater than or equal to `%s`"
+            % (input_variable_path[0], current_validations["min_items"])
         )
 
     items = ("exclusive_maximum", "inclusive_maximum", "exclusive_minimum", "inclusive_minimum")
     if any(item in current_validations for item in items):
         if isinstance(input_values, list):
             max_val = max(input_values)
             min_val = min(input_values)
@@ -922,16 +922,16 @@
 
     if (
         is_json_validation_enabled("maximum", configuration)
         and "inclusive_maximum" in current_validations
         and max_val > current_validations["inclusive_maximum"]
     ):
         raise ApiValueError(
-            "Invalid value for `%s`, must be a value less than or equal to "
-            "`%s`" % (input_variable_path[0], current_validations["inclusive_maximum"])
+            "Invalid value for `%s`, must be a value less than or equal to `%s`"
+            % (input_variable_path[0], current_validations["inclusive_maximum"])
         )
 
     if (
         is_json_validation_enabled("exclusiveMinimum", configuration)
         and "exclusive_minimum" in current_validations
         and min_val <= current_validations["exclusive_minimum"]
     ):
@@ -942,16 +942,16 @@
 
     if (
         is_json_validation_enabled("minimum", configuration)
         and "inclusive_minimum" in current_validations
         and min_val < current_validations["inclusive_minimum"]
     ):
         raise ApiValueError(
-            "Invalid value for `%s`, must be a value greater than or equal "
-            "to `%s`" % (input_variable_path[0], current_validations["inclusive_minimum"])
+            "Invalid value for `%s`, must be a value greater than or equal to `%s`"
+            % (input_variable_path[0], current_validations["inclusive_minimum"])
         )
     flags = current_validations.get("regex", {}).get("flags", 0)
     if (
         is_json_validation_enabled("pattern", configuration)
         and "regex" in current_validations
         and not re.search(current_validations["regex"]["pattern"], input_values, flags=flags)
     ):
@@ -1570,16 +1570,16 @@
             will be converted to a dict.
 
     Keyword Args:
         serialize (bool): if True, the keys in the dict will be values from
             attribute_map
     """
     result = {}
-    extract_item = (
-        lambda item: (item[0], model_to_dict(item[1], serialize=serialize)) if hasattr(item[1], "_data_store") else item
+    extract_item = lambda item: (
+        (item[0], model_to_dict(item[1], serialize=serialize)) if hasattr(item[1], "_data_store") else item
     )
 
     model_instances = [model_instance]
     if model_instance._composed_schemas:
         model_instances.extend(model_instance._composed_instances)
     seen_json_attribute_names = set()
     used_fallback_python_attribute_names = set()
@@ -1644,15 +1644,15 @@
                          True if it is a key in a dict
                          False if our item is an item in a list
     """
     key_or_value = "value"
     if key_type:
         key_or_value = "key"
     valid_classes_phrase = get_valid_classes_phrase(valid_classes)
-    msg = "Invalid type for variable '{0}'. Required {1} type {2} and " "passed type was {3}".format(
+    msg = "Invalid type for variable '{0}'. Required {1} type {2} and passed type was {3}".format(
         var_name,
         key_or_value,
         valid_classes_phrase,
         type(var_value).__name__,
     )
     return msg
 
@@ -1767,21 +1767,22 @@
                         configuration=constant_kwargs["_configuration"],
                     )
             oneof_instances.append(oneof_instance)
         except Exception:
             pass
     if len(oneof_instances) == 0:
         raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None "
-            "of the oneOf schemas matched the input data." % cls.__name__
+            "Invalid inputs given to generate an instance of %s. None of the oneOf schemas matched the input data."
+            % cls.__name__
         )
     elif len(oneof_instances) > 1:
         raise ApiValueError(
             "Invalid inputs given to generate an instance of %s. Multiple "
-            "oneOf schemas matched the inputs, but a max of one is allowed." % cls.__name__
+            "oneOf schemas matched the inputs, but a max of one is allowed."
+            % cls.__name__
         )
     return oneof_instances[0]
 
 
 def get_anyof_instances(self, model_args, constant_args):
     """
     Args:
@@ -1814,16 +1815,16 @@
             else:
                 anyof_instance = anyof_class(**model_args, **constant_args)
             anyof_instances.append(anyof_instance)
         except Exception:
             pass
     if len(anyof_instances) == 0:
         raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None of the "
-            "anyOf schemas matched the inputs." % self.__class__.__name__
+            "Invalid inputs given to generate an instance of %s. None of the anyOf schemas matched the inputs."
+            % self.__class__.__name__
         )
     return anyof_instances
 
 
 def get_discarded_args(self, composed_instances, model_args):
     """
     Gathers the args that were discarded by configuration.discard_unknown_keys
```

### Comparing `groundlight-0.8.0/generated/openapi_client/models/__init__.py` & `groundlight-0.9.0/generated/openapi_client/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ruff: noqa
+# flake8: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from from openapi_client.model.pet import Pet
 # or import this package, but before doing it, use:
```

### Comparing `groundlight-0.8.0/generated/openapi_client/rest.py` & `groundlight-0.9.0/generated/openapi_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
@@ -86,25 +86,25 @@
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
                 proxy_url=configuration.proxy,
                 proxy_headers=configuration.proxy_headers,
-                **addition_pool_args
+                **addition_pool_args,
             )
         else:
             self.pool_manager = urllib3.PoolManager(
                 num_pools=pools_size,
                 maxsize=maxsize,
                 cert_reqs=cert_reqs,
                 ca_certs=configuration.ssl_ca_cert,
                 cert_file=configuration.cert_file,
                 key_file=configuration.key_file,
-                **addition_pool_args
+                **addition_pool_args,
             )
 
     def request(
         self,
         method,
         url,
         query_params=None,
```

### Comparing `groundlight-0.8.0/generated/setup.py` & `groundlight-0.9.0/generated/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Groundlight API
 
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
+    The version of the OpenAPI document: 0.6.0
     Contact: support@groundlight.ai
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
@@ -34,10 +34,10 @@
     url="",
     keywords=["OpenAPI", "OpenAPI-Generator", "Groundlight API"],
     python_requires=">=3.6",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     long_description="""\
-    Ask visual queries.  # noqa: E501
+    Easy Computer Vision powered by Natural Language  # noqa: E501
     """,
 )
```

### Comparing `groundlight-0.8.0/generated/test/test_classification_result.py` & `groundlight-0.9.0/generated/test/test_classification_result.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_detector.py` & `groundlight-0.9.0/generated/test/test_detector.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_detector_creation_input.py` & `groundlight-0.9.0/generated/test/test_detector_creation_input.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_detector_type_enum.py` & `groundlight-0.9.0/generated/test/test_detector_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_detectors_api.py` & `groundlight-0.9.0/generated/test/test_detectors_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_image_queries_api.py` & `groundlight-0.9.0/generated/test/test_image_queries_api.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_image_query.py` & `groundlight-0.9.0/generated/test/test_image_query.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_image_query_type_enum.py` & `groundlight-0.9.0/generated/test/test_image_query_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_paginated_detector_list.py` & `groundlight-0.9.0/generated/test/test_paginated_detector_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_paginated_image_query_list.py` & `groundlight-0.9.0/generated/test/test_paginated_image_query_list.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/generated/test/test_result_type_enum.py` & `groundlight-0.9.0/generated/test/test_result_type_enum.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/pyproject.toml` & `groundlight-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 license = "MIT"
 name = "groundlight"
 packages = [
     {include = "**/*.py", from = "generated"},
     {include = "**/*.py", from = "src"},
 ]
 readme = "README.md"
-version = "0.8.0"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
 certifi = "^2021.10.8"
 frozendict = "^2.3.2"
 pillow = "^9.0.0" # TODO: We may want to mark pillow (and numpy) as extra (https://python-poetry.org/docs/master/pyproject#extras)
 pydantic = "^1.7.4"
 python = ">=3.7.0,<4.0"
```

### Comparing `groundlight-0.8.0/src/groundlight/__init__.py` & `groundlight-0.9.0/src/groundlight/__init__.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/src/groundlight/binary_labels.py` & `groundlight-0.9.0/src/groundlight/binary_labels.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/src/groundlight/client.py` & `groundlight-0.9.0/src/groundlight/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from openapi_client.api.detectors_api import DetectorsApi
 from openapi_client.api.image_queries_api import ImageQueriesApi
 from openapi_client.model.detector_creation_input import DetectorCreationInput
 
 from groundlight.binary_labels import Label, convert_display_label_to_internal, convert_internal_label_to_display
 from groundlight.config import API_TOKEN_VARIABLE_NAME, API_TOKEN_WEB_URL
 from groundlight.images import parse_supported_image_types
-from groundlight.internalapi import GroundlightApiClient, NotFoundError, sanitize_endpoint_url
+from groundlight.internalapi import GroundlightApiClient, NotFoundError, iq_is_confident, sanitize_endpoint_url
 from groundlight.optional_imports import Image, np
 
 logger = logging.getLogger("groundlight.sdk")
 
 
 class ApiTokenError(Exception):
     pass
@@ -67,20 +67,17 @@
 
         configuration.api_key["ApiToken"] = api_token
 
         self.api_client = GroundlightApiClient(configuration)
         self.detectors_api = DetectorsApi(self.api_client)
         self.image_queries_api = ImageQueriesApi(self.api_client)
 
-    @classmethod
-    def _post_process_image_query(cls, iq: ImageQuery) -> ImageQuery:
-        """Post-process the image query so we don't use confusing internal labels.
-
-        TODO: Get rid of this once we clean up the mapping logic server-side.
-        """
+    def _fixup_image_query(self, iq: ImageQuery) -> ImageQuery:  # pylint: disable=no-self-use
+        """Process the wire-format image query to make it more usable."""
+        # Note: This might go away once we clean up the mapping logic server-side.
         iq.result.label = convert_internal_label_to_display(iq, iq.result.label)
         return iq
 
     def get_detector(self, id: Union[str, Detector]) -> Detector:  # pylint: disable=redefined-builtin
         if isinstance(id, Detector):
             # Short-circuit
             return id
@@ -96,45 +93,45 @@
 
     def create_detector(
         self,
         name: str,
         query: str,
         *,
         confidence_threshold: Optional[float] = None,
-        config_name: Optional[str] = None,
+        pipeline_config: Optional[str] = None,
     ) -> Detector:
         detector_creation_input = DetectorCreationInput(name=name, query=query)
         if confidence_threshold is not None:
             detector_creation_input.confidence_threshold = confidence_threshold
-        if config_name is not None:
-            detector_creation_input.config_name = config_name
+        if pipeline_config is not None:
+            detector_creation_input.pipeline_config = pipeline_config
         obj = self.detectors_api.create_detector(detector_creation_input)
         return Detector.parse_obj(obj.to_dict())
 
     def get_or_create_detector(
         self,
         name: str,
         query: str,
         *,
         confidence_threshold: Optional[float] = None,
-        config_name: Optional[str] = None,
+        pipeline_config: Optional[str] = None,
     ) -> Detector:
         """Tries to look up the detector by name.  If a detector with that name, query, and
         confidence exists, return it. Otherwise, create a detector with the specified query and
         config.
         """
         try:
             existing_detector = self.get_detector_by_name(name)
         except NotFoundError:
             logger.debug(f"We could not find a detector with name='{name}'. So we will create a new detector ...")
             return self.create_detector(
                 name=name,
                 query=query,
                 confidence_threshold=confidence_threshold,
-                config_name=config_name,
+                pipeline_config=pipeline_config,
             )
 
         # TODO: We may soon allow users to update the retrieved detector's fields.
         if existing_detector.query != query:
             raise ValueError(
                 (
                     f"Found existing detector with name={name} (id={existing_detector.id}) but the queries don't match."
@@ -150,21 +147,21 @@
                 ),
             )
         return existing_detector
 
     def get_image_query(self, id: str) -> ImageQuery:  # pylint: disable=redefined-builtin
         obj = self.image_queries_api.get_image_query(id=id)
         iq = ImageQuery.parse_obj(obj.to_dict())
-        return self._post_process_image_query(iq)
+        return self._fixup_image_query(iq)
 
     def list_image_queries(self, page: int = 1, page_size: int = 10) -> PaginatedImageQueryList:
         obj = self.image_queries_api.list_image_queries(page=page, page_size=page_size)
         image_queries = PaginatedImageQueryList.parse_obj(obj.to_dict())
         if image_queries.results is not None:
-            image_queries.results = [self._post_process_image_query(iq) for iq in image_queries.results]
+            image_queries.results = [self._fixup_image_query(iq) for iq in image_queries.results]
         return image_queries
 
     def submit_image_query(
         self,
         detector: Union[Detector, str],
         image: Union[str, bytes, Image.Image, BytesIO, BufferedReader, np.ndarray],
         wait: Optional[float] = None,
@@ -187,49 +184,51 @@
         image_bytesio: Union[BytesIO, BufferedReader] = parse_supported_image_types(image)
 
         raw_image_query = self.image_queries_api.submit_image_query(detector_id=detector_id, body=image_bytesio)
         image_query = ImageQuery.parse_obj(raw_image_query.to_dict())
         if wait:
             threshold = self.get_detector(detector).confidence_threshold
             image_query = self.wait_for_confident_result(image_query, confidence_threshold=threshold, timeout_sec=wait)
-        return self._post_process_image_query(image_query)
+        return self._fixup_image_query(image_query)
 
     def wait_for_confident_result(
         self,
         image_query: ImageQuery,
         confidence_threshold: float,
         timeout_sec: float = 30.0,
     ) -> ImageQuery:
         """Waits for an image query result's confidence level to reach the specified value.
         Currently this is done by polling with an exponential back-off.
         :param image_query: An ImageQuery object to poll
         :param confidence_threshold: The minimum confidence level required to return before the timeout.
         :param timeout_sec: The maximum number of seconds to wait.
         """
         # TODO: Add support for ImageQuery id instead of object.
-        timeout_time = time.time() + timeout_sec
-        delay = self.POLLING_INITIAL_DELAY
-        while time.time() < timeout_time:
-            current_confidence = image_query.result.confidence
-            if current_confidence is None:
-                logging.debug("Image query with None confidence implies human label (for now)")
+        start_time = time.time()
+        next_delay = self.POLLING_INITIAL_DELAY
+        target_delay = 0.0
+        image_query = self._fixup_image_query(image_query)
+        while True:
+            patience_so_far = time.time() - start_time
+            if iq_is_confident(image_query, confidence_threshold):
+                logger.debug(f"Confident answer for {image_query} after {patience_so_far:.1f}s")
                 break
-            if current_confidence >= confidence_threshold:
-                logging.debug(f"Image query confidence {current_confidence:.3f} above {confidence_threshold:.3f}")
+            if patience_so_far >= timeout_sec:
+                logger.debug(f"Timeout after {timeout_sec:.0f}s waiting for {image_query}")
                 break
+            target_delay = min(patience_so_far + next_delay, timeout_sec)
+            sleep_time = max(target_delay - patience_so_far, 0)
             logger.debug(
-                (
-                    f"Polling for updated image_query because confidence {current_confidence:.3f} <"
-                    f" {confidence_threshold:.3f}"
-                ),
+                f"Polling ({target_delay:.1f}/{timeout_sec:.0f}s) {image_query} until"
+                f" confidence>={confidence_threshold:.3f}"
             )
-            time_left = max(0, time.time() - timeout_time)
-            time.sleep(min(delay, time_left))
-            delay *= self.POLLING_EXPONENTIAL_BACKOFF
+            time.sleep(sleep_time)
+            next_delay *= self.POLLING_EXPONENTIAL_BACKOFF
             image_query = self.get_image_query(image_query.id)
+            image_query = self._fixup_image_query(image_query)
         return image_query
 
     def add_label(self, image_query: Union[ImageQuery, str], label: Union[Label, str]):
         """A new label to an image query.  This answers the detector's question.
         :param image_query: Either an ImageQuery object (returned from `submit_image_query`) or
         an image_query id as a string.
         :param label: The string "YES" or the string "NO" in answer to the query.
```

### Comparing `groundlight-0.8.0/src/groundlight/images.py` & `groundlight-0.9.0/src/groundlight/images.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/src/groundlight/internalapi.py` & `groundlight-0.9.0/src/groundlight/internalapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import time
 import uuid
 from typing import Optional
 from urllib.parse import urlsplit, urlunsplit
 
 import requests
-from model import Detector
+from model import Detector, ImageQuery
 from openapi_client.api_client import ApiClient
 
 from groundlight.status_codes import is_ok
 
 logger = logging.getLogger("groundlight.sdk")
 
 
@@ -49,19 +49,28 @@
         logger.warning(f"Configured endpoint {endpoint} does not look right - path '{parts.path}' seems wrong.")
     out = urlunsplit(parts)
     out = out[:-1]  # remove trailing slash
     return out
 
 
 def _generate_request_id():
-    # TODO: use a ksuid instead of a uuid.  Most of our API uses ksuids for lots of reasons.
-    # But we don't want to just import ksuid because we want to avoid dependency bloat
     return "req_uu" + uuid.uuid4().hex
 
 
+def iq_is_confident(iq: ImageQuery, confidence_threshold: float) -> bool:
+    """Returns True if the image query's confidence is above threshold.
+    The only subtletie here is that currently confidence of None means
+    human label, which is treated as confident.
+    """
+    if iq.result.confidence is None:
+        # Human label
+        return True
+    return iq.result.confidence >= confidence_threshold
+
+
 class InternalApiError(RuntimeError):
     # TODO: We need a better exception hierarchy
     pass
 
 
 class GroundlightApiClient(ApiClient):
     """Subclassing the OpenAPI-generated ApiClient to add a bit of custom functionality.
```

### Comparing `groundlight-0.8.0/src/groundlight/optional_imports.py` & `groundlight-0.9.0/src/groundlight/optional_imports.py`

 * *Files identical despite different names*

### Comparing `groundlight-0.8.0/PKG-INFO` & `groundlight-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groundlight
-Version: 0.8.0
+Version: 0.9.0
 Summary: Build computer vision systems from natural language with Groundlight
 Home-page: https://code.groundlight.ai/python-sdk
 License: MIT
 Author: Groundlight AI
 Author-email: support@groundlight.ai
 Requires-Python: >=3.7.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

