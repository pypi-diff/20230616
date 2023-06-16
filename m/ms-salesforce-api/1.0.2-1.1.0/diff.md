# Comparing `tmp/ms_salesforce_api-1.0.2.tar.gz` & `tmp/ms_salesforce_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-1.0.2.tar", max compression
+gzip compressed data, was "ms_salesforce_api-1.1.0.tar", max compression
```

## Comparing `ms_salesforce_api-1.0.2.tar` & `ms_salesforce_api-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-06-16 10:22:23.980318 ms_salesforce_api-1.0.2/LICENSE
--rw-r--r--   0        0        0     8325 2023-06-16 10:22:23.980318 ms_salesforce_api-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0     1244 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2926 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2205 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0     3541 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/__tests__/__init__.py
--rw-r--r--   0        0        0    15342 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
--rw-r--r--   0        0        0     7675 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/constants.py
--rw-r--r--   0        0        0     3804 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    20445 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2166 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/dto/__init__.py
--rw-r--r--   0        0        0    23968 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
--rw-r--r--   0        0        0     9228 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    17755 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
--rw-r--r--   0        0        0    13717 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/helpers.py
--rw-r--r--   0        0        0     1055 2023-06-16 10:22:23.984319 ms_salesforce_api-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8325 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0      982 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2713 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0     3338 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    15342 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0     7675 2023-06-15 10:34:08.642830 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/constants.py
+-rw-r--r--   0        0        0     3804 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    20445 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2166 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/__init__.py
+-rw-r--r--   0        0        0    23105 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0     9263 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    17755 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py
+-rw-r--r--   0        0        0    13717 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/helpers.py
+-rw-r--r--   0        0        0     1055 2023-06-15 10:34:08.646831 ms_salesforce_api-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9101 1970-01-01 00:00:00.000000 ms_salesforce_api-1.1.0/PKG-INFO
```

### Comparing `ms_salesforce_api-1.0.2/LICENSE` & `ms_salesforce_api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/README.md` & `ms_salesforce_api-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-import logging
 import time
 from datetime import timedelta
 
 import jwt
 
-logging.basicConfig(
-    level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
-)
-
 
 class JWTGenerator:
     def __init__(
         self,
         client_id,
         private_key,
         username,
@@ -37,13 +32,10 @@
             "aud": self.audience,
             "exp": expiration_time,
         }
 
         try:
             token = jwt.encode(payload, self.private_key, algorithm="RS256")
         except ValueError:
-            logging.error(
-                "[ERROR: generate_token]: Cannot generate the JWT token for authentication."  # noqa: E501
-            )
             token = ""
 
         return token
```

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,17 +34,15 @@
             f"{domain}/{SALESFORCE_QUERY_ENDPOINT.format(api_version)}"
         )
         self.domain = domain
         self.access_token = self.authenticate()
 
     def fetch_data(self, query: str):
         if not self.access_token:
-            logging.error(
-                "[ERROR - fetch_data]: Authentication failed, cannot fetch data"  # noqa: E501
-            )
+            logging.error("Authentication failed, cannot fetch data")
             return None
 
         headers = {"Authorization": f"Bearer {self.access_token}"}
 
         all_records = []
         next_url = f"{self.endpoint}?q={query}"
 
@@ -71,23 +69,21 @@
             return response
         except (
             requests.exceptions.Timeout,
             requests.exceptions.TooManyRedirects,
         ) as e:
             if retry_count >= MAX_RETRIES:
                 logging.error(
-                    f"[ERROR - _make_request]: Request failed after {MAX_RETRIES} attempts due to: {e}"  # noqa: E501
+                    f"Request failed after {MAX_RETRIES} attempts due to: {e}"
                 )
 
                 return None
             logging.warning(
-                "[ERROR - _make_request]: Request timeout or too many redirects, retrying in 2 seconds"  # noqa: E501
+                "Request timeout or too many redirects, retrying in 2 seconds"
             )
             time.sleep(BACKOFF_FACTOR**retry_count)
 
             return self._make_request(url, headers, retry_count + 1)
         except requests.exceptions.RequestException as e:
-            logging.error(
-                f"[ERROR - _make_request]: Request failed due to an unexpected error: {e}"  # noqa: E501
-            )
+            logging.error(f"Request failed due to an unexpected error: {e}")
 
             return None
```

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/__init__.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,14 @@
     ):
         try:
             if last_executed_at:
                 query = query + f"WHERE CreatedDate > {last_executed_at}"
 
             data = self.fetch_data(query)
             if data is None:
-                logging.error(
-                    "[ERROR - SalesforceAPI]: No projects data return from Salesforce API"  # noqa: E501
-                )
                 return []
 
             opportunities = {
                 record["Id"]: OpportunityDTO.from_salesforce_record(record)
                 for record in data
             }
 
@@ -91,11 +88,9 @@
             if format == "json":
                 opportunities_list = [
                     opportunity.to_dict() for opportunity in opportunities_list
                 ]
 
             return opportunities_list
         except Exception as e:
-            logging.error(
-                f"[ERROR - get_all]: Failed to get opportunities: {e}"
-            )
+            logging.error(f"Failed to get opportunities: {e}")
             return []
```

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/__tests__/test_Project.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/__tests__/test_Project.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/constants.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/OpportunityDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/Bigquery.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/Bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-import logging
 from itertools import islice
 from urllib.parse import quote
 
 from gc_google_services_api.bigquery import BigQueryManager
 
-logging.basicConfig(
-    level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
-)
-
 
 class BigQueryExporter:
     """
     Initializes the Bigquery exporter with the given project ID and dataset ID.
 
     Args:
         project_id (str): The ID of the Google Cloud project.
@@ -23,122 +18,106 @@
         self.dataset_id = dataset_id
         self.client = BigQueryManager(
             project_id=project_id, dataset_id=dataset_id
         )
         self.batch_size = 200
         self.schemas = {
             "opportunities": {
-                "amount": "FLOAT",
-                "controller_email": "STRING",
-                "controller_sub_email": "STRING",
-                "cost_center": "STRING",
-                "created_at": "TIMESTAMP",
                 "currency": "STRING",
+                "amount": "FLOAT",
                 "invoicing_country_code": "STRING",
-                "jira_task_url": "STRING",
-                "last_updated_at": "TIMESTAMP",
-                "lead_source": "STRING",
                 "operation_coordinator_email": "STRING",
                 "operation_coordinator_sub_email": "STRING",
+                "created_at": "TIMESTAMP",
+                "last_updated_at": "TIMESTAMP",
                 "opportunity_name": "STRING",
-                "opportunity_percentage": "STRING",
-                "profit_center": "STRING",
+                "stage": "STRING",
+                "lead_source": "STRING",
                 "project_code": "STRING",
                 "project_id": "STRING",
                 "project_name": "STRING",
                 "project_start_date": "DATE",
+                "controller_email": "STRING",
+                "controller_sub_email": "STRING",
+                "profit_center": "STRING",
+                "cost_center": "STRING",
                 "project_tier": "STRING",
-                "stage": "STRING",
+                "jira_task_url": "STRING",
+                "opportunity_percentage": "STRING",
             },
             "billing_lines": {
+                "id": "STRING",
+                "project_id": "STRING",
+                "name": "STRING",
+                "currency": "STRING",
+                "created_date": "TIMESTAMP",
+                "last_modified_date": "TIMESTAMP",
                 "billing_amount": "FLOAT",
                 "billing_date": "DATE",
                 "billing_period_ending_date": "DATE",
                 "billing_period_starting_date": "DATE",
+                "hourly_price": "FLOAT",
+                "revenue_dedication": "FLOAT",
                 "billing_plan_amount": "STRING",
                 "billing_plan_billing_date": "DATE",
                 "billing_plan_item": "STRING",
                 "billing_plan_service_end_date": "DATE",
                 "billing_plan_service_start_date": "DATE",
-                "created_date": "TIMESTAMP",
-                "currency": "STRING",
-                "hourly_price": "FLOAT",
-                "id": "STRING",
-                "last_modified_date": "TIMESTAMP",
-                "name": "STRING",
-                "project_id": "STRING",
-                "revenue_dedication": "FLOAT",
             },
             "project_line_items": {
                 "country": "STRING",
+                "project_id": "STRING",
                 "created_date": "TIMESTAMP",
                 "effort": "STRING",
                 "ending_date": "DATE",
                 "id": "STRING",
                 "last_modified_date": "TIMESTAMP",
                 "ms_pli_name": "STRING",
                 "product_name": "STRING",
-                "project_id": "STRING",
                 "quantity": "FLOAT",
                 "starting_date": "DATE",
                 "total_price": "STRING",
                 "unit_price": "STRING",
             },
             "accounts": {
+                "id": "STRING",
+                "project_id": "STRING",
+                "name": "STRING",
                 "assigment_group": "STRING",
+                "tax_category": "STRING",
+                "tax_classification": "STRING",
+                "sap_id": "STRING",
+                "business_function": "STRING",
+                "tax_id_type": "STRING",
+                "currency_code": "STRING",
+                "created_date": "STRING",
+                "tier": "STRING",
+                "pec_email": "STRING",
+                "phone": "STRING",
+                "fax": "STRING",
+                "website": "STRING",
+                "cif": "STRING",
+                "billing_country": "STRING",
+                "business_name": "STRING",
                 "billing_address": "STRING",
                 "billing_city": "STRING",
-                "billing_country": "STRING",
                 "billing_postal_code": "STRING",
-                "billing_state_code": "STRING",
                 "billing_street": "STRING",
-                "business_function": "STRING",
-                "business_name": "STRING",
-                "cif": "STRING",
                 "company_invoicing": "STRING",
-                "created_date": "STRING",
-                "currency_code": "STRING",
-                "fax": "STRING",
-                "id": "STRING",
-                "invoicing_email": "STRING",
-                "mail_invoicing": "STRING",
-                "name": "STRING",
                 "office": "STRING",
                 "payment_terms": "STRING",
-                "pec_email": "STRING",
-                "phone": "STRING",
-                "project_id": "STRING",
-                "sap_id": "STRING",
-                "tax_category": "STRING",
-                "tax_classification": "STRING",
-                "tax_id_type": "STRING",
-                "tier": "STRING",
-                "website": "STRING",
+                "billing_state_code": "STRING",
+                "mail_invoicing": "STRING",
+                "invoicing_email": "STRING",
             },
         }
 
         for table_name, table_schema in self.schemas.items():
             self.client.create_table_if_not_exists(table_name, table_schema)
 
-    def _execute_query(self, query, log_id, default_error_value=None):
-        custom_error_value = f"{log_id}_custom_error"
-
-        result = self.client.execute_query(
-            query,
-            custom_error_value,
-        )
-
-        if result == custom_error_value:
-            logging.error(
-                "[ERROR - _execute_query]: Error executing query for {log_id} in BigQuery."
-            )
-            result = default_error_value
-
-        return result
-
     def _export_opportunities(self, opportunities):
         opportunities_values = []
         for opp in opportunities:
             project_start_date = (
                 f'DATE "{opp["project_start_date"]}"'
                 if opp["project_start_date"]
                 else "NULL"
@@ -206,17 +185,15 @@
 
             insert_opportunities_query = (
                 insert_opportunities_query.replace("\n", "")
                 .replace("    ", "")
                 .replace("  ", "")
             )
 
-            self._execute_query(
-                query=insert_opportunities_query, log_id="INSERT_opportunities"
-            )
+            self.client.execute_query(insert_opportunities_query, None)
 
     def _export_billing_lines(self, opportunities):
         total_billing_lines = sum(
             len(opp["billing_lines"]) for opp in opportunities
         )
 
         for i in range(0, total_billing_lines, self.batch_size):
@@ -321,17 +298,15 @@
             """
             insert_billing_lines_query = (
                 insert_billing_lines_query.replace("\n", "")
                 .replace("    ", "")
                 .replace("  ", "")
             )
 
-            self._execute_query(
-                query=insert_billing_lines_query, log_id="INSERT_billing_lines"
-            )
+            self.client.execute_query(insert_billing_lines_query, None)
 
     def _export_PLIs(self, opportunities):
         total_plis = sum(
             len(opp["project_line_items"]) for opp in opportunities
         )
 
         for i in range(0, total_plis, self.batch_size):
@@ -420,17 +395,15 @@
 
             insert_plis_query = (
                 insert_plis_query.replace("\n", "")
                 .replace("    ", "")
                 .replace("  ", "")
             )
 
-            self._execute_query(
-                query=insert_plis_query, log_id="INSERT_project_line_items"
-            )
+            self.client.execute_query(insert_plis_query, None)
 
     def _export_accounts(self, opportunities):
         account_values = []
         for opp in opportunities:
             account_name = (
                 f'"{opp["account_name"]}"' if opp["account_name"] else "NULL"
             )
@@ -587,17 +560,16 @@
                     {account_payment_terms},
                     {account_billing_state_code},
                     {account_mail_invoicing},
                     {account_invoicing_email}
                 )
                 """
             )
-
         if account_values:
-            insert_accounts_query = f"""
+            insert_opportunities_query = f"""
                 INSERT INTO `{self.project_id}.{self.dataset_id}.accounts` (
                     project_id,
                     name,
                     assigment_group,
                     tax_category,
                     tax_classification,
                     sap_id,
@@ -621,23 +593,21 @@
                     office,
                     payment_terms,
                     billing_state_code,
                     mail_invoicing,
                     invoicing_email
                 ) VALUES {', '.join(account_values)};
             """
-            insert_accounts_query = (
-                insert_accounts_query.replace("\n", "")
+            insert_opportunities_query = (
+                insert_opportunities_query.replace("\n", "")
                 .replace("    ", "")
                 .replace("  ", "")
             )
 
-            self._execute_query(
-                query=insert_accounts_query, log_id="INSERT_accounts"
-            )
+            self.client.execute_query(insert_opportunities_query, None)
 
     def export_data(self, opportunities):
         opportunities_batches = [
             opportunities[i : i + self.batch_size]  # noqa: E203
             for i in range(0, len(opportunities), self.batch_size)
         ]
         for batch in opportunities_batches:
@@ -649,11 +619,9 @@
 
             self._export_accounts(batch)
 
     def delete_all_rows(self):
         table_names = self.schemas.keys()
         for table_name in table_names:
             delete_query_table = f"DELETE FROM `{self.project_id}.{self.dataset_id}.{table_name}` WHERE true"
-            self._execute_query(
-                query=delete_query_table,
-                log_id=f"delete_table_{table_name}",
-            )
+
+            self.client.execute_query(delete_query_table, None)
```

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/CloudSQL.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,17 @@
 
             if self.debug_mode:
                 insert_query_string = cursor.mogrify(
                     insert_query.as_string(cursor.connection),
                     opportunity_fixed,
                 ).decode("utf-8")
                 logging.info(insert_query_string)
-            logging.error(f"[ERROR - _insert_accounts_batch (cloudsql)] - {e}")
+            logging.error(
+                f"[ERROR - _insert_opportunities_batch (cloudsql)] - {e}"
+            )
 
             raise (e)
 
     def _insert_billing_lines_batch(self, cursor, billing_lines):
         insert_query = sql.SQL(
             """
             INSERT INTO BillingLines ({})
```

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_Bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-1.1.0/ms_salesforce_api/salesforce/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-1.0.2/pyproject.toml` & `ms_salesforce_api-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "1.0.2"
+version = "1.1.0"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-1.0.2/PKG-INFO` & `ms_salesforce_api-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 1.0.2
+Version: 1.1.0
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

