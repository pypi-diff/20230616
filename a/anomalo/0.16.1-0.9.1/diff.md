# Comparing `tmp/anomalo-0.16.1.tar.gz` & `tmp/anomalo-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomalo-0.16.1.tar", max compression
+gzip compressed data, was "dist/anomalo-0.9.1.tar", last modified: Wed Sep  7 16:54:04 2022, max compression
```

## Comparing `anomalo-0.16.1.tar` & `anomalo-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11344 2023-06-15 16:25:30.607711 anomalo-0.16.1/LICENSE
--rw-r--r--   0        0        0      104 2023-06-15 16:25:30.607711 anomalo-0.16.1/README.public.md
--rw-r--r--   0        0        0      140 2023-06-15 16:25:30.607711 anomalo-0.16.1/anomalo/__init__.py
--rw-r--r--   0        0        0       35 2023-06-15 16:25:30.607711 anomalo-0.16.1/anomalo/__main__.py
--rw-r--r--   0        0        0       23 2023-06-15 23:55:41.451711 anomalo-0.16.1/anomalo/__version__.py
--rwxr-xr-x   0        0        0      250 2023-06-15 16:25:30.607711 anomalo-0.16.1/anomalo/anomalo.py
--rw-r--r--   0        0        0        0 2023-06-15 16:25:30.607711 anomalo-0.16.1/anomalo/cli/__init__.py
--rw-r--r--   0        0        0     1537 2023-06-15 16:25:30.607711 anomalo-0.16.1/anomalo/cli/cli.py
--rw-r--r--   0        0        0        0 2023-06-15 16:25:30.607711 anomalo-0.16.1/anomalo/cli/save_load/__init__.py
--rw-r--r--   0        0        0     6132 2023-06-15 16:25:30.607711 anomalo-0.16.1/anomalo/cli/save_load/commands.py
--rw-r--r--   0        0        0     7879 2023-06-15 16:25:30.611711 anomalo-0.16.1/anomalo/cli/save_load/models.py
--rw-r--r--   0        0        0        0 2023-06-15 16:25:30.611711 anomalo-0.16.1/anomalo/cli/state/__init__.py
--rw-r--r--   0        0        0     5849 2023-06-15 23:55:05.883711 anomalo-0.16.1/anomalo/cli/state/api.py
--rw-r--r--   0        0        0     1343 2023-06-15 16:25:30.611711 anomalo-0.16.1/anomalo/cli/state/errors.py
--rw-r--r--   0        0        0     1476 2023-06-15 16:25:30.611711 anomalo-0.16.1/anomalo/cli/state/file.py
--rw-r--r--   0        0        0     4765 2023-06-15 16:25:30.611711 anomalo-0.16.1/anomalo/cli/state/machine.py
--rw-r--r--   0        0        0     3897 2023-06-15 16:25:30.611711 anomalo-0.16.1/anomalo/cli/state/models.py
--rw-r--r--   0        0        0    11138 2023-06-15 16:25:30.611711 anomalo-0.16.1/anomalo/client.py
--rw-r--r--   0        0        0     3636 2023-06-15 16:25:30.611711 anomalo-0.16.1/anomalo/encoder.py
--rw-r--r--   0        0        0     1969 2023-06-15 16:25:30.611711 anomalo-0.16.1/anomalo/result.py
--rw-r--r--   0        0        0      895 2023-06-15 23:55:41.447711 anomalo-0.16.1/pyproject.toml
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 anomalo-0.16.1/PKG-INFO
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/
+-rw-r--r--   0 johnjoo    (501) staff       (20)       33 2022-09-06 04:48:18.000000 anomalo-0.9.1/.gitignore
+-rw-r--r--   0 johnjoo    (501) staff       (20)    11344 2022-09-06 04:48:18.000000 anomalo-0.9.1/LICENSE.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)      308 2022-09-07 16:54:04.000000 anomalo-0.9.1/PKG-INFO
+-rw-r--r--   0 johnjoo    (501) staff       (20)      211 2022-09-06 04:48:18.000000 anomalo-0.9.1/README.txt
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo/
+-rw-r--r--   0 johnjoo    (501) staff       (20)       57 2022-09-06 04:48:18.000000 anomalo-0.9.1/anomalo/__init__.py
+-rw-r--r--   0 johnjoo    (501) staff       (20)       22 2022-09-07 16:54:02.000000 anomalo-0.9.1/anomalo/_version.py
+-rwxr-xr-x   0 johnjoo    (501) staff       (20)     7444 2022-09-06 04:48:18.000000 anomalo-0.9.1/anomalo/anomalo.py
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/
+-rw-r--r--   0 johnjoo    (501) staff       (20)      308 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/PKG-INFO
+-rw-r--r--   0 johnjoo    (501) staff       (20)      348 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/SOURCES.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)        1 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/dependency_links.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)       41 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/entry_points.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)       14 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/requires.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)        8 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/top_level.txt
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/examples/
+-rw-r--r--   0 johnjoo    (501) staff       (20)     3701 2022-09-06 04:48:18.000000 anomalo-0.9.1/examples/bulk_rerun.py
+-rw-r--r--   0 johnjoo    (501) staff       (20)     1284 2022-09-06 04:48:18.000000 anomalo-0.9.1/examples/sample.py
+-rw-r--r--   0 johnjoo    (501) staff       (20)       29 2022-08-01 21:30:00.000000 anomalo-0.9.1/requirements.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)       38 2022-09-07 16:54:04.000000 anomalo-0.9.1/setup.cfg
+-rw-r--r--   0 johnjoo    (501) staff       (20)      899 2022-09-07 16:46:35.000000 anomalo-0.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `anomalo-0.16.1/LICENSE` & `anomalo-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anomalo-0.16.1/anomalo/client.py` & `anomalo-0.9.1/anomalo/anomalo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,20 @@
-from __future__ import annotations
+#!/usr/bin/env python
 
 import os
-from typing import Any
 from urllib.parse import urlparse
 
 import requests
 
-from .result import Result
-
 
 class Client:
+
     output_style = "json"
 
-    def __init__(
-        self,
-        api_token=None,
-        host=None,
-        proto=None,
-        ssl_cert_verify=None,
-        output_style=None,
-        legacy_auth: bool = True,
-    ):
-        if output_style:
-            self.output_style = output_style
+    def __init__(self, api_token=None, host=None, proto=None, ssl_cert_verify=None):
         self.host = host if host else os.environ.get("ANOMALO_INSTANCE_HOST")
         self.api_token = (
             api_token if api_token else os.environ.get("ANOMALO_API_SECRET_TOKEN")
         )
 
         if not self.host:
             raise RuntimeError(
@@ -41,91 +29,55 @@
         host_scheme = parsed_host_url.scheme
         if host_scheme:
             self.proto = host_scheme
             self.host = parsed_host_url.netloc
         else:
             self.proto = proto if proto else "https"
 
-        self.request_headers = (
-            {"X-Anomalo-Token": self.api_token}
-            if legacy_auth
-            else {"Authorization": f"Bearer {self.api_token}"}
-        )
+        self.request_headers = {"X-Anomalo-Token": self.api_token}
 
         self.verify = ssl_cert_verify
 
-    def _api_call(self, endpoint, method="GET", empty_response=False, **kwargs) -> Any:
+    def _api_call(self, endpoint, method="GET", **kwargs):
 
         endpoint_url = "{proto}://{host}/api/public/v1/{endpoint}".format(
             proto=self.proto, host=self.host, endpoint=endpoint
         )
 
-        if method in ["PUT", "POST", "PATCH", "DELETE"]:
+        if method in ["PUT", "POST"]:
             request_args = dict(json=kwargs)
         else:
             request_args = dict(params=kwargs)
-
         r = requests.request(
             method,
             endpoint_url,
             headers=self.request_headers,
             verify=self.verify,
             allow_redirects=False,
             **request_args,
         )
 
         if not r.ok:
             raise RuntimeError(r.text)
-        if empty_response:
-            return r
-        return Result.from_raw(r, self.output_style)
+        return r.json() if self.output_style == "json" else r.text
 
     def ping(self):
         return self._api_call("ping")
 
     def get_active_organization_id(self):
         return self._api_call("organization").get("id")
 
     def set_active_organization_id(self, organization_id):
         return self._api_call("organization", method="PUT", id=organization_id).get(
             "id"
         )
 
-    def get_all_organizations(self):
-        return self._api_call("organizations")
-
     def list_warehouses(self):
         return self._api_call("list_warehouses")
 
-    def get_warehouse(self, warehouse_id: int):
-        return self._api_call(f"warehouse/{warehouse_id}")
-
-    def create_warehouse(
-        self, name: str, warehouse_type: str, connection: dict[str, Any]
-    ):
-        return self._api_call(
-            "warehouse",
-            name=name,
-            warehouse_type=warehouse_type,
-            connection=connection,
-            method="POST",
-        )
-
-    def update_warehouse(
-        self, warehouse_id: int, name: str, connection: dict[str, Any]
-    ):
-        return self._api_call(
-            f"warehouse/{warehouse_id}", name=name, connection=connection, method="PUT"
-        )
-
-    def delete_warehouse(self, warehouse_id: int):
-        self._api_call(
-            f"warehouse/{warehouse_id}", method="DELETE", empty_response=True
-        )
-
     def refresh_warehouse(self, warehouse_id):
         return self._api_call(f"warehouse/{warehouse_id}/refresh", method="PUT")
 
     def refresh_warehouse_tables(self, warehouse_id, table_full_names):
         if not table_full_names:
             raise RuntimeError("Must specify a list of full table names to sync")
         return self._api_call(
@@ -136,63 +88,34 @@
 
     def refresh_warehouse_new_tables(self, warehouse_id):
         return self._api_call(f"warehouse/{warehouse_id}/refresh/new", method="PUT")
 
     def list_notification_channels(self):
         return self._api_call("list_notification_channels")
 
-    def configured_tables(
-        self,
-        check_cadence_type: str | None = None,
-        warehouse_id: int | None = None,
-        details: bool = True,
-        limit: int = 0,
-        offset: int = 0,
-    ):
+    def configured_tables(self, check_cadence_type=None, warehouse_id=None):
         return self._api_call(
             "configured_tables",
             check_cadence_type=check_cadence_type,
             warehouse_id=warehouse_id,
-            details=True,
-            limit=limit,
-            offset=offset,
         )
 
-    def tables(self, limit: int = 0, offset: int = 0):
-        return self._api_call("tables", limit=limit, offset=offset)
-
-    def filter_tables_by_label(self, label_id):
-        return self._api_call(f"tables?label_id={label_id}")
-
     def get_table_information(self, warehouse_id=None, table_id=None, table_name=None):
         if (not table_id or not warehouse_id) and not table_name:
             raise RuntimeError(
                 "Must specify either warehouse_id & table_id or table_name for get_table_information"
             )
         else:
             return self._api_call(
                 "get_table_information",
                 warehouse_id=warehouse_id,
                 table_id=table_id,
                 table_name=table_name,
             )
 
-    def get_table_profile(self, warehouse_id=None, table_id=None, table_name=None):
-        if (not table_id or not warehouse_id) and not table_name:
-            raise RuntimeError(
-                "Must specify either warehouse_id & table_id or table_name for get_table_profile"
-            )
-        else:
-            return self._api_call(
-                "get_table_profile",
-                warehouse_id=warehouse_id,
-                table_id=table_id,
-                table_name=table_name,
-            )
-
     def get_check_intervals(self, table_id=None, start=None, end=None):
         if not table_id:
             raise RuntimeError("Must specify a table_id for get_check_intervals")
         else:
             results = []
             page = 0
             paged_results = None
@@ -262,88 +185,48 @@
             new_table_id=new_table_id,
             method="POST",
         )
 
     def configure_table(
         self,
         table_id,
-        *,
         check_cadence_type=None,
         definition=None,
         time_column_type=None,
         notify_after=None,
         time_columns=None,
         fresh_after=None,
         interval_skip_expr=None,
         notification_channel_id=None,
         slack_users=None,
         check_cadence_run_at_duration=None,
-        always_alert_on_errors=False,
     ):
         time_columns = [] if time_columns is None else time_columns
         slack_users = {} if slack_users is None else slack_users
 
         return self._api_call(
             "configure_table",
             table_id=table_id,
             method="POST",
             check_cadence_type=check_cadence_type,
             definition=definition,
             time_column_type=time_column_type,
             notify_after=notify_after,
-            notification_channel_id=notification_channel_id,
+            selected_channel=notification_channel_id,
             time_columns=time_columns,
             fresh_after=fresh_after,
             interval_skip_expr=interval_skip_expr,
             slack_users=slack_users,
             check_cadence_run_at_duration=check_cadence_run_at_duration,
-            always_alert_on_errors=always_alert_on_errors,
         )
 
-    def create_table_label_for_organization(self, name):
-        return self._api_call(
-            "table-labels",
-            method="POST",
-            name=name,
-        )
 
-    def list_table_labels_for_organization(self):
-        return self._api_call("table-labels")
+def main():
+    import fire
 
-    def update_table_label_name_for_organization(self, label_id, new_name):
-        return self._api_call(
-            f"table-labels/{label_id}",
-            method="PUT",
-            name=new_name,
-        )
-
-    def delete_table_label_for_organization(self, label_id):
-        self._api_call(
-            f"table-labels/{label_id}",
-            method="DELETE",
-            empty_response=True,
-        )
+    Client.output_style = "text"
 
-    def merge_table_labels_for_organization(
-        self, source_label_id, destination_label_id
-    ):
-        return self._api_call(
-            f"table-labels/{destination_label_id}/merge",
-            method="POST",
-            source_label_id=source_label_id,
-        )
+    fire.Fire(Client)
 
-    def replace_labels_for_table(self, table_id, labels):
-        return self._api_call(
-            f"tables/{table_id}/labels",
-            method="PUT",
-            empty_response=True,
-            labels=labels,
-        )
 
-    def add_new_labels_to_table(self, table_id, labels):
-        return self._api_call(
-            f"tables/{table_id}/labels",
-            method="PATCH",
-            empty_response=True,
-            labels=labels,
-        )
+if __name__ == "__main__":
+    main()
```

