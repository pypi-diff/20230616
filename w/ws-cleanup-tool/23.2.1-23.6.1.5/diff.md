# Comparing `tmp/ws_cleanup_tool-23.2.1-py3-none-any.whl.zip` & `tmp/ws_cleanup_tool-23.6.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,11 @@
-Zip file size: 15810 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-28 15:36 ws_cleanup_tool/__init__.py
--rw-r--r--  2.0 unx       90 b- defN 23-Feb-28 15:36 ws_cleanup_tool/_version.py
--rw-r--r--  2.0 unx    24480 b- defN 23-Feb-28 15:36 ws_cleanup_tool/cleanup_tool.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-28 15:36 ws_cleanup_tool/test/__init__.py
--rw-r--r--  2.0 unx     2233 b- defN 23-Feb-28 15:36 ws_cleanup_tool/test/test_projects-cleanup.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Feb-28 15:36 ws_cleanup_tool-23.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7750 b- defN 23-Feb-28 15:36 ws_cleanup_tool-23.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-28 15:36 ws_cleanup_tool-23.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-Feb-28 15:36 ws_cleanup_tool-23.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Feb-28 15:36 ws_cleanup_tool-23.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      976 b- defN 23-Feb-28 15:36 ws_cleanup_tool-23.2.1.dist-info/RECORD
-11 files, 47065 bytes uncompressed, 14122 bytes compressed:  70.0%
+Zip file size: 14662 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-16 17:53 mend_sca_cleanup_tool/__init__.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-16 17:53 mend_sca_cleanup_tool/_version.py
+-rw-r--r--  2.0 unx    21762 b- defN 23-Jun-16 17:53 mend_sca_cleanup_tool/sca_cleanup_tool.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9170 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/RECORD
+9 files, 43409 bytes uncompressed, 13212 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -1,34 +1,28 @@
-Filename: ws_cleanup_tool/__init__.py
+Filename: mend_sca_cleanup_tool/__init__.py
 Comment: 
 
-Filename: ws_cleanup_tool/_version.py
+Filename: mend_sca_cleanup_tool/_version.py
 Comment: 
 
-Filename: ws_cleanup_tool/cleanup_tool.py
+Filename: mend_sca_cleanup_tool/sca_cleanup_tool.py
 Comment: 
 
-Filename: ws_cleanup_tool/test/__init__.py
+Filename: ws_cleanup_tool-23.6.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: ws_cleanup_tool/test/test_projects-cleanup.py
+Filename: ws_cleanup_tool-23.6.1.5.dist-info/METADATA
 Comment: 
 
-Filename: ws_cleanup_tool-23.2.1.dist-info/LICENSE
+Filename: ws_cleanup_tool-23.6.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: ws_cleanup_tool-23.2.1.dist-info/METADATA
+Filename: ws_cleanup_tool-23.6.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ws_cleanup_tool-23.2.1.dist-info/WHEEL
+Filename: ws_cleanup_tool-23.6.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ws_cleanup_tool-23.2.1.dist-info/entry_points.txt
-Comment: 
-
-Filename: ws_cleanup_tool-23.2.1.dist-info/top_level.txt
-Comment: 
-
-Filename: ws_cleanup_tool-23.2.1.dist-info/RECORD
+Filename: ws_cleanup_tool-23.6.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ws_cleanup_tool/cleanup_tool.py` & `mend_sca_cleanup_tool/sca_cleanup_tool.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,462 +1,418 @@
-import argparse
+import http.client
 import json
-import logging
-import os
 import sys
-from abc import ABC, abstractmethod
-from configparser import ConfigParser
-from dataclasses import dataclass
+import argparse
+import re
+import os
+import uuid
 from datetime import timedelta, datetime
 from distutils.util import strtobool
-from multiprocessing import Manager
-from multiprocessing.pool import ThreadPool
-
-from ws_sdk import ws_errors, WS, ws_constants
-
-from ws_cleanup_tool._version import __description__, __tool_name__, __version__
-
-# skip_report_generation = bool(os.environ.get("SKIP_REPORT_GENERATION", 0))
-# skip_project_deletion = bool(os.environ.get("SKIP_PROJECT_DELETION", 0))
-
-logging.basicConfig(level=logging.DEBUG if bool(os.environ.get("DEBUG", "false")) is True else logging.INFO,
-                    handlers=[logging.StreamHandler(stream=sys.stdout)],
-                    format='%(levelname)s %(asctime)s %(thread)d %(name)s: %(message)s',
-                    datefmt='%y-%m-%d %H:%M:%S')
-logger = logging.getLogger(__tool_name__)
-logging.getLogger('urllib3').setLevel(logging.WARNING)
-
-conf = None
-
-
-class FilterStrategy:
-    def __init__(self, filter_projects) -> None:
-        self._filter_projects = filter_projects
-
-    def execute(self):
-        def replace_invalid_chars(directory: str) -> str:
-            for char in ws_constants.INVALID_FS_CHARS:
-                directory = directory.replace(char, "_")
-
-            return directory
-
-        projects = self._filter_projects.get_projects_to_archive()
+from configparser import ConfigParser
+from mend_sca_cleanup_tool._version import __description__, __tool_name__, __version__
 
-        for project in projects:
-            product_name = replace_invalid_chars(project['product_name'])
-            project_name = replace_invalid_chars(project['name'])
-            project_output_dir = os.path.join(os.path.join(conf.output_dir, product_name), project_name)
-            project_output_dir_180_char = (project_output_dir[:180] + '..') if len(project_output_dir) > 180 else project_output_dir
-            project['project_output_dir'] = project_output_dir_180_char
 
-        return projects
+ATTRIBUTION = "attribution"
+FILTER_PROJECTS_BY_UPDATE_TIME = "FilterProjectsByUpdateTime"
+FILTER_PROJECTS_BY_LAST_CREATED_COPIES = "FilterProjectsByLastCreatedCopies"
+HEADERS = {
+    'Content-Type': 'application/json',
+    'agent': f"ps-{__tool_name__}".replace('_', '-'),
+    'agentVersion': __version__,
+    'ctxId': uuid.uuid1().__str__()
+}
+IGNORED_ALERTS = "ignored_alerts"
+RESOLVED_ALERTS = "resolved_alerts"
+REJECTED_BY_POLICY = "alerts_rejected_by_policy"
+REPORTS = {
+           "bugs": "getProjectBugsReport",
+           IGNORED_ALERTS: "getProjectSecurityAlertsByVulnerabilityReport",
+           REJECTED_BY_POLICY: "getProjectAlertsByType",
+           "in_house_libraries": "getProjectInHouseReport",
+           "license_compatibility": "getProjectLicenseCompatibilityReport",
+           RESOLVED_ALERTS: "getProjectSecurityAlertsByVulnerabilityReport",
+           "source_files": "getProjectSourceFileInventoryReport", 
+           "alerts": "getProjectSecurityAlertsByVulnerabilityReport",
+           ATTRIBUTION: "getProjectAttributionReport",
+           "due_diligence": "getProjectDueDiligenceReport",
+           "inventory": "getProjectInventoryReport",
+           "request_history": "getProjectRequestHistoryReport",
+           "source_file_inventory": "getProjectSourceFileInventoryReport",
+           "vulnerability": "getProjectVulnerabilityReport"
+           }
 
+def main():
+    global CONFIG
+    global MAIN_API_CONNECTION
+    if len(sys.argv) == 1:
+        CONFIG = parse_config_file("params.config")
+    elif not sys.argv[1].startswith('-'):
+        CONFIG = parse_config_file(sys.argv[1])
+    else:
+        CONFIG = parse_args()
+    
+    setup_config()
 
-class FilterProjectsInt(ABC):
-    def __init__(self, products_to_clean, config):
-        self.products_to_clean = products_to_clean
-        self.conf = config
-        self.should_filter_by_tag = True if self.conf.analyzed_project_tag or self.conf.analyzed_project_tag_regex_in_value else False
+    MAIN_API_CONNECTION = http.client.HTTPSConnection(CONFIG.mend_url)
 
-    @abstractmethod
-    def get_projects_to_archive(self):
-        ...
+    if CONFIG.dry_run:
+        print("Dry Run enabled - no reports or deletions will occur")
 
-    def is_valid_project(self, project):
-        def is_tag_exist(p):
-            # tag:value set in the Unified Agent scanCommnet parameter
-            project_metadata_d = p.get('project_metadata_d', {})
-            if self.conf.analyzed_project_tag_t[0] in project_metadata_d.keys() \
-                    and project_metadata_d[self.conf.analyzed_project_tag_t[0]] == self.conf.analyzed_project_tag_t[1]:
-                return True
-            # Add support for tag value defined in the UI
-            elif self.conf.analyzed_project_tag_t[1] in p.get('tags')[0].get('tags').get(self.conf.analyzed_project_tag_t[0], ''):
-                return True
-            else:
-                return False
+    product_project_dict = get_projects_to_remove()
 
-        def is_tag_value_contained(p):
-            # tag:value set in the Unified Agent scanCommnet parameter
-            project_metadata_d = p.get('project_metadata_d', {})
-            if self.conf.analyzed_project_tag_t[0] in project_metadata_d.keys() \
-                    and self.conf.analyzed_project_tag_t[1] in project_metadata_d[self.conf.analyzed_project_tag_t[0]]:
-                return True
-            # Add support for tag value defined in the UI
-            elif self.conf.analyzed_project_tag_t[0]:
-                for k, v in p.get('tags')[0].get('tags').items():
-                    if self.conf.analyzed_project_tag_t[0] in k and self.conf.analyzed_project_tag_t[1] in v:
-                        return True
-            else:
-                return False
 
-        ret = True
-        if not self.should_filter_by_tag:
-            logger.debug(f"Project {project['name']} is valid")
-        elif self.should_filter_by_tag and is_tag_exist(project):
-            logger.debug(f"Project {project['name']} contains appropriate key:value pair: {self.conf.analyzed_project_tag_t}")
-        elif self.should_filter_by_tag and is_tag_value_contained(project):
-            logger.debug(f"Project {project['name']} contains appropriate key:value pair: {self.conf.analyzed_project_tag_t}")
+    total_projects_to_delete = (sum([len(product_project_dict[x]) for x in product_project_dict]))
+    if not CONFIG.dry_run:
+        if total_projects_to_delete == 0:
+            print("No projects to clean up were found")
+            exit()
         else:
-            logger.debug(f"Project {project['name']} does not contain appropriate key:value pair: {self.conf.analyzed_project_tag_t}")
-            ret = False
-
-        return ret
-
+            print(f"Found {total_projects_to_delete} project(s) to delete, generating reports and removing project(s)...")
+        for product_token in product_project_dict:
+            for project in product_project_dict[product_token]:
+                if not CONFIG.skip_report_generation:
+                    generate_reports(project)
+                else:
+                    print("skipReportGeneration flag found, skipping report generation")
+                if not CONFIG.skip_project_deletion:
+                    delete_scan(product_token, project)
+                else:
+                    print("skipProjectDeletion flag found, skipping project deletion")
+    else:
+        print(f"Dry Run found {total_projects_to_delete} project(s) to delete: {[project['name'] for projects in product_project_dict.values() for project in projects]}")
 
-class FilterProjectsByUpdateTime(FilterProjectsInt):
-    def get_projects_to_archive(self) -> list:
-        days_to_keep = timedelta(days=self.conf.days_to_keep)
-        archive_date = datetime.utcnow() - days_to_keep
-        logger.info(f"Keeping {days_to_keep.days} days. Looking for the projects older than {archive_date}")
-
-        manager = Manager()
-        projects_to_archive_q = manager.Queue()
-        with ThreadPool(processes=self.conf.project_parallelism_level) as pool:
-            pool.starmap(self.get_projects_to_archive_w,
-                         [(archive_date, prod, self.conf.ws_conn, projects_to_archive_q) for prod in self.products_to_clean])
-        return extract_from_q(projects_to_archive_q)
-
-    def get_projects_to_archive_w(self, archive_date, prod, ws_conn, projects_to_archive_q):
-        curr_prod_projects = ws_conn.get_projects(product_token=prod['token'], include_prod_proj_names=True)
-        logger.info(f"Handling product: {prod['name']} number of projects: {len(curr_prod_projects)}")
-
-        for project in curr_prod_projects:
-            project_time = datetime.strptime(project['lastUpdatedDate'], "%Y-%m-%d %H:%M:%S +%f")
-            project['tags'] = ws_conn.get_tags(token=project.get('token'))
-            if project_time < archive_date and self.is_valid_project(project):
-                logger.debug(f"Project {project['name']} Token: {project['token']} Last update: {project['lastUpdatedDate']} will be cleaned up")
-                projects_to_archive_q.put(project)
-
-
-class FilterProjectsByLastCreatedCopies(FilterProjectsInt):
-    def get_projects_to_archive(self) -> list:
-        logger.info(f"Keeping last recent {self.conf.days_to_keep} projects. Cleaning up the rest")
-        manager = Manager()
-        projects_to_archive_q = manager.Queue()
-        with ThreadPool(processes=self.conf.project_parallelism_level) as pool:
-            pool.starmap(self.get_projects_to_archive_w,
-                         [(prod['token'], self.conf.ws_conn, projects_to_archive_q) for prod in self.products_to_clean])
-        projects_to_archive = extract_from_q(projects_to_archive_q)
-
-        if not projects_to_archive:
-            logger.info("No projects to clean up were found")
-
-        return projects_to_archive
-
-    def get_projects_to_archive_w(self, product_token: str, ws_conn: WS, projects_to_archive_q):
-        projects = ws_conn.get_projects(product_token=product_token, sort_by=ws_constants.ScopeSorts.UPDATE_TIME)
-
-        for project in projects:
-            project['tags'] = ws_conn.get_tags(token=project.get('token'))
-
-        filtered_projects = [project for project in projects if self.is_valid_project(project)]
-        if len(filtered_projects) > self.conf.days_to_keep:
-            index = len(filtered_projects) - self.conf.days_to_keep
-            last_projects = filtered_projects[:index]
-            logger.debug(f"Total {len(filtered_projects)}. Archiving first {index}")
-            projects_to_archive_q.put(last_projects)
+def check_response_error(obj_response):
+    if isinstance(obj_response, dict):
+        if "errorMessage" in obj_response:
+            print(f"There was an issue with the request: {obj_response['errorMessage']}")
+            return True
         else:
-            logger.debug(f"Total {len(filtered_projects)}. Nothing to cleanup")
-
-
-def extract_from_q(projects_to_archive_q):
-    projects_to_archive = []
-    while not projects_to_archive_q.empty():
-        item = projects_to_archive_q.get(block=True, timeout=0.05)
-        projects_to_archive.append(item) if isinstance(item, dict) else projects_to_archive.extend(item)
-
-    return projects_to_archive
-
-
-def get_reports_to_archive(projects_to_archive: list) -> list:
-    project_reports_desc_list = []
-
-    for project in projects_to_archive:  # Creating list of report to-be-produced meta data
-        if not os.path.exists(project['project_output_dir']):
-            os.makedirs(project['project_output_dir'])
-
-        for report in conf.report_types:
-            curr_project_report = project.copy()
-            curr_project_report['report'] = report
-
-            project_reports_desc_list.append(curr_project_report)
-
-    logger.info(f"Found total {len(projects_to_archive)} projects to clean up ({len(project_reports_desc_list)} reports will be produced)")
-
-    return project_reports_desc_list
+            return False
 
+def create_output_directory(product_name, project_name):
+    product_name = remove_invalid_chars(product_name)
+    project_name = remove_invalid_chars(project_name)
+    if not CONFIG.output_dir.endswith("\\"):
+        CONFIG.output_dir = CONFIG.output_dir + "\\"
+    output_dir = CONFIG.output_dir + product_name + "\\" + project_name + "\\"
+    if len(output_dir) > 180:
+        output_dir = (output_dir[:180] + "..")
+    if not os.path.exists(output_dir):
+        print(f"Making directory {output_dir}")
+        os.makedirs(output_dir)
+    return output_dir
+
+def delete_scan(product_token, project):
+    print(f"Deleting project: {project['name']}")
+    request = json.dumps({
+                "requestType": "deleteProject",
+                "userKey": CONFIG.mend_user_key,
+                "productToken": product_token,
+                "projectToken": project['token']
+            })
+    response_obj = json.loads(post_api_request(request).decode("utf-8"))
+    if check_response_error(response_obj):
+        return
+
+def filter_projects_by_config(projects):
+    projects_to_return = [project for project in projects if project['token'] not in CONFIG.excluded_project_tokens]
+    if len(projects_to_return) == 0:
+        return []
+
+    if CONFIG.excluded_project_name_patterns:
+        print(f"Filtering projects with name containing values {CONFIG.project_name_exclude_list}")
+        for patt in CONFIG.project_name_exclude_list:
+            projects_to_return = [project for project in projects_to_return for k, v in project.items() if k == "name" and patt not in v]
+
+    if CONFIG.operation_mode == FILTER_PROJECTS_BY_UPDATE_TIME:
+        archive_date = (datetime.utcnow() - timedelta(days=CONFIG.days_to_keep))
+        print(f"Filtering projects older than: {archive_date}")
+        projects_to_return = [project for project in projects_to_return if archive_date.timestamp() > datetime.strptime(project['lastUpdatedDate'],'%Y-%m-%d %H:%M:%S %z').timestamp()]
+
+    if CONFIG.analyzed_project_tag:
+        print(f"Filtering projects based on project tag: {CONFIG.analyzed_project_tag}")
+        projects_to_return = filter_projects_by_tag_with_exact_match(projects_to_return) 
+
+    if CONFIG.analyzed_project_tag_regex_in_value:
+        print(f"Filtering projects based on project contain tag value: {CONFIG.analyzed_project_tag_regex_in_value}")
+        projects_to_return = filter_projects_by_tag_with_contains_match(projects_to_return)
+
+    if CONFIG.operation_mode == FILTER_PROJECTS_BY_LAST_CREATED_COPIES:
+        print(f"Filtering projects besides most recent: {CONFIG.days_to_keep}")
+        if len(projects_to_return) > CONFIG.days_to_keep:
+            index = len(projects_to_return) - CONFIG.days_to_keep
+            print(f"Total: {len(projects_to_return)}. Removing oldest {index}")
+            projects_to_return = sorted(projects_to_return, key=lambda d: d['lastUpdatedDate'])
+            projects_to_return = projects_to_return[:index]
+        else:
+            print(f"Total: {len(projects_to_return)}. Nothing to filter")
+    print(f"{len(projects_to_return)} project(s) to remove after filtering")
+    return projects_to_return
+
+def filter_projects_by_tag_with_exact_match(projects):
+    projects_to_return = []
+    for project in projects:
+        project_tags = get_project_tags(project)
+        if CONFIG.tag_pair[1] in project_tags.get(CONFIG.tag_pair[0], ''):
+            print(f"{project['name']} has matching tag")
+            projects_to_return.append(project)
+    return projects_to_return
+
+def filter_projects_by_tag_with_contains_match(projects):
+    projects_to_return = []
+    for project in projects:
+        project_tags = get_project_tags(project)
+        for k, v in project_tags.items():
+            if CONFIG.tag_pair[0] in k and any(CONFIG.tag_pair[1] in item for item in v):
+                print(f"{project['name']} contains tag value")
+                projects_to_return.append(project)
+    return projects_to_return
+
+def generate_reports(project):
+    print(f"Generating reports for project: {project['name']}")
+    project_token = project['token']
+    reports_to_generate = get_reports_to_generate()
+    if len(reports_to_generate) > 0:
+        output_dir = create_output_directory(project['productName'], project['name'])
+        for report in reports_to_generate.keys():
+            print(f"Generating {report} report for project {project['name']}")
+            reportFormat = 'xlsx'
+            if report.lower() == ATTRIBUTION:
+                data = get_attribution_report(project_token)
+                reportFormat = 'html'
+            elif report.lower() == RESOLVED_ALERTS:
+                data = get_alerts_report(reports_to_generate[report], project_token, "resolved")
+            elif report.lower() == IGNORED_ALERTS:
+                data = get_alerts_report(reports_to_generate[report], project_token, "ignored")
+            elif report.lower() == REJECTED_BY_POLICY:
+                data = get_alerts_by_type(reports_to_generate[report], project_token, "REJECTED_BY_POLICY_RESOURCE")
+                reportFormat = "json"
+            else:
+                data = get_excel_report(reports_to_generate[report], project_token)
 
-def get_products_to_archive(included_product_tokens: list, excluded_product_tokens: list) -> list:
-    if included_product_tokens:
-        logger.debug(f"Product tokens to check for cleanup: {included_product_tokens}")
-        prods = [conf.ws_conn.get_scopes(scope_type=ws_constants.ScopeTypes.PRODUCT, token=prod_t).pop() for prod_t in included_product_tokens]
+            check_response_error(data)
+            report = open(output_dir + report + '.' + reportFormat, "wb")
+            report.write(data)
+            report.close()
     else:
-        logger.debug("Getting all products")
-        prods = conf.ws_conn.get_products()
+        print("No reports to generate")
 
-    all_prods_n = len(prods)
-    if excluded_product_tokens:
-        logger.debug(f"Product tokens configured to be excluded from cleanup: {excluded_product_tokens}")
-        prods = [prod for prod in prods if prod['token'] not in excluded_product_tokens]
 
-    logger.info(f"Product names for cleanup check: {[prod['name'] for prod in prods]}")
-    logger.info(f"{all_prods_n} Products to handle out of {len(prods)}")
-
-    return prods
-
-
-def exclude_projects(projects_to_archive: list, excluded_project_tokens: list, excluded_project_name_patterns: list) -> list:
-    if excluded_project_tokens:
-        logger.debug(f"Exclude project tokens: {excluded_project_tokens}")
-
-    projects = [proj for proj in projects_to_archive if proj['token'] not in excluded_project_tokens] if excluded_project_tokens else projects_to_archive
-
-    if excluded_project_name_patterns:
-        for patt in excluded_project_name_patterns:
-            logger.debug(f"Exclude projects with name pattern: {patt}")
-            projects = [proj for proj in projects for k, v in proj.items() if k == "name" and patt not in v]
-
-    logger.info(f"Project names for cleanup check: {[proj['name'] for proj in projects]}")
-
-    return projects
-
-
-def generate_reports_m(reports_desc_list: list) -> list:
-    manager = Manager()
-    failed_proj_tokens_q = manager.Queue()
-    with ThreadPool(processes=conf.project_parallelism_level) as pool:
-        pool.starmap(generate_report_w,
-                     [(report_desc, conf.ws_conn, failed_proj_tokens_q) for report_desc in reports_desc_list])
-
-    failed_projects = []
-    while not failed_proj_tokens_q.empty():
-        failed_projects.append(failed_proj_tokens_q.get(block=True, timeout=0.05))
-
-    if failed_projects:
-        logger.warning(f"{len(failed_projects)} projects were failed to clean up")
-
-    return failed_projects
-
-
-def generate_report_w(report_desc: dict, connector: WS, w_f_proj_tokens_q) -> None:
-    def get_suffix(entity):  # Handling case where more than 1 suffix
-        return entity if isinstance(entity, str) else entity[0]
-
-    if report_desc['report'].bin_sfx:
-        report_name = f"{report_desc['report'].name}.{get_suffix(report_desc['report'].bin_sfx)}"
-        report_full_path = os.path.join(report_desc['project_output_dir'], report_name)
-        if conf.dry_run:
-            logger.info(f"[DRY_RUN] Report: '{report_name}' has to be created on the project: '{report_desc['name']}'")
-        else:
-            logger.debug(f"Generating report: '{report_full_path}' on the project: '{report_desc['name']}'")
-            try:
-                report = report_desc['report'].func(connector, token=report_desc['token'], report=True)
-                f = open(report_full_path, 'bw')
-                if not report:
-                    report = bytes()
-                f.write(report)
-            except ws_errors.WsSdkServerError or OSError:
-                logger.exception(f"Error producing report: '{report_desc['report_type']}' on project {report_desc['name']}. Project will not be deleted.")
-                w_f_proj_tokens_q.put(report_desc['token'])
-            try:
-                alerts_report = connector.get_alerts(token=report_desc['token'], alert_type="REJECTED_BY_POLICY_RESOURCE")
-                with open(f"{os.path.join(report_desc['project_output_dir'])}/alerts_rejected_by_policy.json", 'w', encoding='utf-8') as f:
-                    json.dump(alerts_report, f, ensure_ascii=False, indent=4)
-            except:
-                logger.exception(f"Error producing report: alerts for REJECTED_BY_POLICY_RESOURCE on project {report_desc['name']}. Project will not be deleted.")
-                w_f_proj_tokens_q.put(report_desc['token'])
+def get_alerts_report(request_type, project_token, alertType):
+    request = json.dumps({
+        "requestType": request_type,
+        "userKey": CONFIG.mend_user_key,
+        "projectToken": project_token,
+        "status": alertType,
+        "format": "xlsx"
+    })
+    return post_api_request(request)
+
+def get_alerts_by_type(request_type, project_token, alertType):
+    request = json.dumps({
+        "requestType": request_type,
+        "userKey": CONFIG.mend_user_key,
+        "projectToken": project_token,
+        "alertType": alertType
+    })
+    return post_api_request(request)
+
+def get_attribution_report(project_token):
+    request = json.dumps({
+        "requestType": REPORTS[ATTRIBUTION],
+        "userKey": CONFIG.mend_user_key,
+        "projectToken": project_token,
+        "reportingAggregationMode": "BY_PROJECT",
+        "exportFormat": "html"
+    })
+    return post_api_request(request)
+
+def get_config_file_value(config_val, default):
+        if isinstance(config_val, int):
+            return config_val if config_val is not None else default
+        return config_val if config_val else default
+
+def get_excel_report(request_type, project_token):
+    request = json.dumps({
+        "requestType": request_type,
+        "userKey": CONFIG.mend_user_key,
+        "projectToken": project_token,
+        "format": "xlsx"
+    })
+    return post_api_request(request)
+
+def get_reports_to_generate():
+    if len(CONFIG.report_types) == 0:
+        return REPORTS
     else:
-        logger.debug(f"Skipping report: {report_desc['report'].name} is invalid")
-
-
-def delete_projects(projects_to_archive: list, failed_project_tokens: list) -> None:
-    w_dry_run = conf.dry_run
-    projects_to_delete = projects_to_archive.copy()
-    for project in projects_to_archive:
-        if project['token'] in failed_project_tokens:
-            projects_to_delete.remove(project)
-    logger.info(f"Total found {len(projects_to_archive)} projects to delete. {len(projects_to_delete)} projects have valid tokens and should be deleted")
-
-    if projects_to_delete:
-        with ThreadPool(processes=1) as thread_pool:
-            thread_pool.starmap(worker_delete_project, [(conf.ws_conn, project, w_dry_run) for project in projects_to_delete])
-        if w_dry_run:
-            logger.info(f"Total found {len(projects_to_delete)} projects that have to be deleted")
-        else:
-            logger.info(f"{len(projects_to_delete)} projects have been deleted")
-
-
-def worker_delete_project(conn, project, w_dry_run):
-    if w_dry_run:
-        logger.info(f"[DRY_RUN] project: {project['name']}. Last update date is: {project['lastUpdatedDate']}. Token: {project['token']} ")
+        reportKeys = CONFIG.report_types.replace(" ", "").split(',')
+        report_dictionary = dict((k, REPORTS[k]) for k in reportKeys if k in REPORTS)
+        if len(report_dictionary) != len(reportKeys):
+            unmatched_keys = [k for k in reportKeys if k not in report_dictionary.keys()]
+            for unmatched_key in unmatched_keys:
+                print(f"Could not generate report for {unmatched_key}. Unsupported report, please reference the README for supported reports")
+        return report_dictionary
+
+
+def get_products():
+    request = json.dumps({
+        "requestType": "getAllProducts",
+        "userKey": CONFIG.mend_user_key,
+        "orgToken": CONFIG.mend_api_token,
+    })
+    response_obj = json.loads(post_api_request(request).decode("utf-8"))
+    if check_response_error(response_obj):
+        exit()
+    if len(CONFIG.included_product_tokens) == 0:
+        return [product for product in response_obj['products'] if product['productToken'] not in CONFIG.excluded_product_tokens]
     else:
-        logger.info(f"Deleting project: {project['name']}. Last update date is: {project['lastUpdatedDate']}. Token: {project['token']} ")
-        conn.delete_scope(token=project['token'], project=project)
+        return [product for product in response_obj['products'] if product['productToken'] in CONFIG.included_product_tokens and product['productToken'] not in CONFIG.excluded_product_tokens]
 
+def get_projects(product_token):
+    request = json.dumps({
+        "requestType": "getProductProjectVitals",
+        "userKey": CONFIG.mend_user_key,
+        "productToken": product_token,
+    })
+    response_obj = json.loads(post_api_request(request).decode("utf-8"))
+    if check_response_error(response_obj):
+        exit()
+    else:
+        return [vital_Response for vital_Response in response_obj['projectVitals']]
 
-def parse_config():
-    @dataclass
-    class Config:
-        ws_user_key: str
-        ws_org_token: str
-        ws_url: str
-        report_types: str
-        operation_mode: str
-        output_dir: str
-        excluded_product_tokens: list
-        included_product_tokens: list
-        excluded_project_tokens: list
-        excluded_project_name_patterns: list
-        analyzed_project_tag: dict
-        analyzed_project_tag_regex_in_value: dict
-        days_to_keep: int
-        project_parallelism_level: int
-        dry_run: bool
-        skip_report_generation: bool
-        skip_project_deletion: bool
-
-        ws_conn: WS
-
-    def get_conf_value(c_p_val, alt_val):
-        return c_p_val if c_p_val else alt_val
-
-    def generate_analyzed_project_tag(analyzed_project_tag):
-        conf.analyzed_project_tag_t = tuple(analyzed_project_tag.replace(" ", "").split(":"))
-        if len(conf.analyzed_project_tag_t) != 2:
-            logger.error(f"Unable to parse Project tag: {conf.analyzed_project_tag}")
-            conf.analyzed_project_tag_t = None
+def get_project_tags(project):
+    print(f"Getting tags for project {project['name']}")
+    request = json.dumps({
+            "requestType": "getProjectTags",
+            "userKey": CONFIG.mend_user_key,
+            "projectToken": project['token'],
+        })
+    response_obj = json.loads(post_api_request(request).decode("utf-8"))
+    if check_response_error(response_obj):
+        exit()
+    return [project_tags['tags'] for project_tags in response_obj['projectTags']][0]
+
+def get_projects_to_remove():
+    projects_to_remove = {}
+    products = get_products()
+    for product in products:
+        print(f"Getting projects to remove for product: {product['productName']}")
+        projects = get_projects(product['productToken'])
+        projects_length = len(projects)
+        if projects_length:
+            print(f"Product has {projects_length} project(s)")
+            filtered_projects = filter_projects_by_config(projects)
+            filted_projects_total = len(filtered_projects)
+            if filted_projects_total > 0:
+                projects_to_remove[product['productToken']] = filtered_projects
         else:
-            logger.info(f"Project tag is set. The tool will only analyze projects with tag: '{conf.analyzed_project_tag}'")
+            print(f"No projects found for product: {product['productName']}")
+    return projects_to_remove
 
-    global conf
-
-    if len(sys.argv) < 3:
-        maybe_config_file = True
-    if len(sys.argv) == 1:
-        conf_file = "../params.config"
-    elif not sys.argv[1].startswith('-'):
-        conf_file = sys.argv[1]
+def parse_args():
+    parser = argparse.ArgumentParser(description="Mend SCA Clean up tool")
+    parser.add_argument('-a', '--mendURL', '--wsURL', help="Mend URL", dest='mend_url', default="saas.whitesourcesoftware.com")
+    parser.add_argument('-e', '--excludedProductTokens', help="Excluded Product Tokens (comma seperated list)", dest='excluded_product_tokens')
+    parser.add_argument('-g', '--analyzedProjectTag', help="Analyze only the projects whose contain the specific Mend tag (key:value). Case sensitive.", dest='analyzed_project_tag')
+    parser.add_argument('-i', '--includedProductTokens', help="Included Product Tokens (comma seperated list)", dest='included_product_tokens')
+    parser.add_argument('-j', '--skipProjectDeletion', help="Skip Project Deletion", dest='skip_project_deletion', type=strtobool, default=False)
+    parser.add_argument('-k', '--apiToken', '--orgToken', help="Mend API token", dest='mend_api_token', required=True)
+    parser.add_argument('-m', '--operationMode', help="Clean up operation method", dest='operation_mode', default=FILTER_PROJECTS_BY_UPDATE_TIME,
+                                choices=[s for s in [FILTER_PROJECTS_BY_UPDATE_TIME, FILTER_PROJECTS_BY_LAST_CREATED_COPIES]])
+    parser.add_argument('-n', '--excludedProjectNamePatterns', help="List of excluded project name patterns (comma seperated list). Case sensitive.", dest='excluded_project_name_patterns')
+    parser.add_argument('-o', '--outputDir', help="Output directory", dest='output_dir', default=os.getcwd() + "\\Mend\\Reports\\")
+    parser.add_argument('-p', '--projectParallelismLevel', help="Project parallelism level directory Note: This is currently not used in this version of the mend-sca-cleanup-tool", dest='project_parallelism_level')
+    parser.add_argument('-r', '--daysToKeep', help="Number of days to keep (overridden by --dateToKeep)", dest='days_to_keep', type=int, default=50000)
+    parser.add_argument('-s', '--skipReportGeneration', help="Skip Report Generation", dest='skip_report_generation', type=strtobool, default=False)
+    parser.add_argument('-t', '--reportTypes', help="Report Types to generate (comma seperated list)", dest='report_types')
+    parser.add_argument('-u', '--userKey', help="Mend UserKey", dest='mend_user_key', required=True)
+    parser.add_argument('-v', '--analyzedProjectTagRegexInValue', help="Analyze only the projects whose match their tag key and the tag value contains the specified regex (key:value). Case sensitive. Note: This was originally broken in the original ws-cleanup-tool. The functionality was adjusted to work as originally written. The naming convention is a misnomer but was kept to avoid breaking existing integrations.", dest='analyzed_project_tag_regex_in_value')
+    parser.add_argument('-x', '--excludedProjectTokens', help="Excluded Project Tokens (comma seperated list)", dest='excluded_project_tokens')
+    parser.add_argument('-y', '--dryRun', help="Whether to run the tool without performing anything", dest='dry_run', type=strtobool, default=False)
+    return parser.parse_args()
+
+def parse_config_file(filepath):
+    if os.path.exists(filepath):
+        config = ConfigParser()
+        config.optionxform = str
+        config.read(filepath)
+        return argparse.Namespace(
+                    mend_user_key=get_config_file_value(config['DEFAULT'].get("MendUserKey", config['DEFAULT'].get("WsUserKey")), os.environ.get("WS_USER_KEY")),
+                    mend_api_token=get_config_file_value(config['DEFAULT'].get("MendApiToken", config['DEFAULT'].get("WsOrgToken")), os.environ.get("WS_ORG_TOKEN")),
+                    mend_url=get_config_file_value(config['DEFAULT'].get("MendUrl", config['DEFAULT'].get("WsUrl")), os.environ.get("WS_URL")),
+                    report_types=get_config_file_value(config['DEFAULT'].get('ReportTypes'), os.environ.get("REPORT_TYPES")),
+                    operation_mode=get_config_file_value(config['DEFAULT'].get("OperationMode"), FILTER_PROJECTS_BY_UPDATE_TIME),
+                    output_dir=get_config_file_value(config['DEFAULT'].get('OutputDir'), os.getcwd() + "\\Mend\\Reports\\"),
+                    excluded_product_tokens=get_config_file_value(config['DEFAULT'].get("ExcludedProductTokens", []), os.environ.get("EXCLUDED_PRODUCT_TOKENS")),
+                    included_product_tokens=get_config_file_value(config['DEFAULT'].get("IncludedProductTokens", []), os.environ.get("INCLUDED_PRODUCT_TOKENS")),
+                    excluded_project_tokens=get_config_file_value(config['DEFAULT'].get("ExcludedProjectTokens", []), os.environ.get("EXCLUDED_PROJECT_TOKENS")),
+                    excluded_project_name_patterns=get_config_file_value(config['DEFAULT'].get("ExcludedProjectNamePatterns", None), os.environ.get("EXCLUDED_PROJECT_NAME_PATTERNS")),
+                    analyzed_project_tag=get_config_file_value(config['DEFAULT'].get("AnalyzedProjectTag", None), os.environ.get("ANALYZED_PROJECT_TAG")),
+                    analyzed_project_tag_regex_in_value=get_config_file_value(config['DEFAULT'].get("AnalyzedProjectTagRegexInValue", None), os.environ.get("ANALYZED_PROJECT_TAG_REGEX_IN_VALUE")),
+                    days_to_keep=get_config_file_value(config['DEFAULT'].getint("DaysToKeep", 50000), os.environ.get("DAYS_TO_KEEP")),
+                    project_parallelism_level=config['DEFAULT'].get('ProjectParallelismLevel', 5),
+                    dry_run=config['DEFAULT'].getboolean("DryRun", False),
+                    skip_report_generation=config['DEFAULT'].getboolean("SkipReportGeneration", False),
+                    skip_project_deletion=config['DEFAULT'].getboolean("SkipProjectDeletion", False)
+                )
     else:
-        maybe_config_file = False
-
-    if maybe_config_file:  # Covers no conf file or only conf file
-        if os.path.exists(conf_file):
-            logger.info(f"loading configuration from file: {conf_file}")
-            config = ConfigParser()
-            config.optionxform = str
-            # if os.path.exists(conf_file):
-            #     logger.info(f"loading configuration from file: {conf_file}")
-            config.read(conf_file)
-            operation_mode = get_conf_value(config['DEFAULT'].get("OperationMode"), FilterProjectsByUpdateTime.__name__)
-
-            conf = Config(
-                ws_user_key=get_conf_value(config['DEFAULT'].get("WsUserKey"), os.environ.get("WS_USER_KEY")),
-                ws_org_token=get_conf_value(config['DEFAULT'].get("WsOrgToken"), os.environ.get("WS_ORG_TOKEN")),
-                ws_url=get_conf_value(config['DEFAULT'].get("WsUrl"), os.environ.get("WS_URL")),
-                report_types=get_conf_value(config['DEFAULT'].get('ReportTypes'), os.environ.get("REPORT_TYPES")),
-                operation_mode=operation_mode,
-                output_dir=get_conf_value(config['DEFAULT'].get('ReportsDir'), os.getcwd()),
-                excluded_product_tokens=get_conf_value(config['DEFAULT'].get("ExcludedProductTokens", None), os.environ.get("EXCLUDED_PRODUCT_TOKENS")),
-                included_product_tokens=get_conf_value(config['DEFAULT'].get("IncludedProductTokens", None), os.environ.get("INCLUDED_PRODUCT_TOKENS")),
-                excluded_project_tokens=get_conf_value(config['DEFAULT'].get("ExcludedProjectTokens", None), os.environ.get("EXCLUDED_PROJECT_TOKENS")),
-                excluded_project_name_patterns=get_conf_value(config['DEFAULT'].get("ExcludedProjectNamePatterns", None), os.environ.get("EXCLUDED_PROJECT_NAME_PATTERNS")),
-                analyzed_project_tag=get_conf_value(config['DEFAULT'].get("AnalyzedProjectTag", None), os.environ.get("ANALYZED_PROJECT_TAG")),
-                analyzed_project_tag_regex_in_value=get_conf_value(config['DEFAULT'].get("AnalyzedProjectTagRegexInValue", None), os.environ.get("ANALYZED_PROJECT_TAG_REGEX_IN_VALUE")),
-                days_to_keep=get_conf_value(config['DEFAULT'].getint("DaysToKeep", 50000), os.environ.get("DAYS_TO_KEEP")),
-                project_parallelism_level=config['DEFAULT'].getint('ProjectParallelismLevel', 5),
-                dry_run=config['DEFAULT'].getboolean("DryRun", False),
-                skip_report_generation=config['DEFAULT'].getboolean("SkipReportGeneration", True),
-                skip_project_deletion=config['DEFAULT'].getboolean("SkipProjectDeletion", False),
-                ws_conn=None
-            )
-
+        print(f"No configuration file found at: {filepath}")
+        exit()
 
+def post_api_request(request):
+    try:
+        MAIN_API_CONNECTION.request("POST", '/api/v1.4', request, HEADERS)
+        return MAIN_API_CONNECTION.getresponse().read()
+    except:
+        sys.exit(f"There was an issue calling the Mend API with URL: {CONFIG.mend_url}")
+
+def remove_invalid_chars(string_to_clean):
+    return re.sub('[:*<>/"?|.]', '-', string_to_clean).replace("\\", "-")
+
+def setup_config():
+    if not CONFIG.mend_user_key:
+        sys.exit(f"A Mend user key was not provided")
+    if not CONFIG.mend_api_token:
+        sys.exit(f"A Mend Api key was not provided")
+
+    if CONFIG.mend_url:
+        CONFIG.mend_url = re.sub("(https?)://", "", CONFIG.mend_url.lower())
+        if '/' in CONFIG.mend_url:
+            apiIndex = CONFIG.mend_url.find('/')
         else:
-            logger.error(f"No configuration file found at: {conf_file}")
-            raise FileNotFoundError
+            apiIndex = len(CONFIG.mend_url)
+        CONFIG.mend_url = CONFIG.mend_url[:apiIndex]
     else:
-        parser = argparse.ArgumentParser(description=__description__)
-        parser.add_argument('-u', '--userKey', help="WS User Key", dest='ws_user_key', default=os.environ.get("WS_USER_KEY"))
-        parser.add_argument('-k', '--orgToken', help="WS Organization Key", dest='ws_org_token', default=os.environ.get("WS_ORG_TOKEN"))
-        parser.add_argument('-a', '--wsUrl', help="WS URL", dest='ws_url', default=os.environ.get("WS_URL"))
-        parser.add_argument('-t', '--reportTypes', help="Report Types to generate (comma seperated list)", dest='report_types', default=os.environ.get("REPORT_TYPES"))
-        parser.add_argument('-m', '--operationMode', help="Clean up operation method", dest='operation_mode', default="FilterProjectsByUpdateTime",
-                            choices=[s.__name__ for s in FilterProjectsInt.__subclasses__()])
-        parser.add_argument('-o', '--outputDir', help="Output directory", dest='output_dir', default=os.getcwd())
-        parser.add_argument('-e', '--excludedProductTokens', help="Excluded Product Tokens list", dest='excluded_product_tokens', default=os.environ.get("EXCLUDED_PRODUCT_TOKENS"))
-        parser.add_argument('-i', '--includedProductTokens', help="Included Product Tokens list", dest='included_product_tokens', default=os.environ.get("INCLUDED_PRODUCT_TOKENS"))
-        parser.add_argument('-x', '--excludedProjectTokens', help="Excluded Project Tokens list", dest='excluded_project_tokens', default=os.environ.get("EXCLUDED_PROJECT_TOKENS"))
-        parser.add_argument('-n', '--excludedProjectNamePatterns', help="ExcludedProjectNamePatterns", dest='excluded_project_name_patterns', default=os.environ.get("EXCLUDED_PROJECT_NAME_PATTERNS"))
-        parser.add_argument('-g', '--analyzedProjectTag', help="Analyze only the projects whose contain the specific Mend tag", dest='analyzed_project_tag', default=os.environ.get("ANALYZED_PROJECT_TAG"))
-        parser.add_argument('-v', '--analyzedProjectTagRegexInValue', help="Analyze only the projects whose match their tag key and the tag value contains the specified regex", dest='analyzed_project_tag_regex_in_value', default=os.environ.get("ANALYZED_PROJECT_TAG_REGEX_IN_VALUE"))
-        parser.add_argument('-r', '--daysToKeep', help="Number of days to keep in FilterProjectsByUpdateTime or number of copies in FilterProjectsByLastCreatedCopies", dest='days_to_keep', type=int, default=50000)
-        parser.add_argument('-p', '--projectParallelismLevel', help="Project parallelism level", dest='project_parallelism_level', type=int, default=5)
-        parser.add_argument('-y', '--dryRun', help="Whether to run the tool without performing anything", dest='dry_run', type=strtobool, default=False)
-        parser.add_argument('-s', '--skipReportGeneration', help="Skip Report Generation", dest='skip_report_generation', type=strtobool, default=True)
-        parser.add_argument('-j', '--skipProjectDeletion', help="Skip Project Deletion", dest='skip_project_deletion', type=strtobool, default=False)
-        conf = parser.parse_args()
-
-    if conf.analyzed_project_tag:
-        generate_analyzed_project_tag(conf.analyzed_project_tag)
-    elif conf.analyzed_project_tag_regex_in_value:
-        generate_analyzed_project_tag(conf.analyzed_project_tag_regex_in_value)
-
-    conf.included_product_tokens = conf.included_product_tokens.replace(" ", "").split(",") if conf.included_product_tokens else []
-    conf.excluded_product_tokens = conf.excluded_product_tokens.replace(" ", "").split(",") if conf.excluded_product_tokens else []
-    conf.excluded_project_tokens = conf.excluded_project_tokens.replace(" ", "").split(",") if conf.excluded_project_tokens else []
-    conf.excluded_project_name_patterns = conf.excluded_project_name_patterns.split(",") if conf.excluded_project_name_patterns else []
-    conf.report_types = get_reports(conf.report_types)
-    conf.ws_conn = WS(url=conf.ws_url,
-                      user_key=conf.ws_user_key,
-                      token=conf.ws_org_token,
-                      skip_ua_download=True,
-                      tool_details=(f"ps-{__tool_name__.replace('_', '-')}", __version__))
-    return conf
-
-
-def get_reports(report_types: str) -> list:
-    reports_d = {}
-    all_reports = WS.get_reports_meta_data(scope=ws_constants.ScopeTypes.PROJECT)
-
-    if report_types:
-        report_types_l = report_types.replace(' ', '').split(",")
-        reports_to_gen_l = []
-        for r in all_reports:  # Converting list of report meta data tuples to dict
-            reports_d[r.name] = r
-
-        for r_t in report_types_l:
-            if r_t in reports_d.keys():
-                reports_to_gen_l.append(reports_d[r_t])
+        sys.exit(f"A Mend URL was not provided") 
 
-    return reports_to_gen_l if report_types else all_reports
-
-
-def main():
-    global conf
-    start_time = datetime.now()
-    try:
-        conf = parse_config()
-    except FileNotFoundError:
-        exit(-1)
-
-    logger.info(f"Starting project cleanup in '{conf.operation_mode}' mode. Generating {len(conf.report_types)} report types with {conf.project_parallelism_level} threads")
-    products_to_clean = get_products_to_archive(conf.included_product_tokens, conf.excluded_product_tokens)
-    filter_class = FilterStrategy(globals()[conf.operation_mode](products_to_clean, conf))
-    projects_to_archive = filter_class.execute()
-    filtered_projects_to_archive = exclude_projects(projects_to_archive, conf.excluded_project_tokens, conf.excluded_project_name_patterns)
-    reports_to_archive = get_reports_to_archive(filtered_projects_to_archive)
-    failed_project_tokens = []
-
-    if conf.skip_report_generation:
-        logger.info("Skipping Report Generation")
-    else:
-        failed_project_tokens = generate_reports_m(reports_to_archive)
-    if conf.skip_project_deletion:
-        logger.info("Skipping Project Deletion")
-    else:
-        delete_projects(filtered_projects_to_archive, failed_project_tokens)
+    if CONFIG.analyzed_project_tag:
+        tag_pair = tuple(CONFIG.analyzed_project_tag.replace(" ", "").split(":"))
+        if len(tag_pair) != 2:
+            print(f"Unable to parse project tag: {CONFIG.analyzed_project_tag}")
+            sys.exit("Expected format of project tags: <name:value>")
+        else:
+            CONFIG.tag_pair = tag_pair
 
-    logger.info(f"Project Cleanup has been finished. Run time: {datetime.now() - start_time}")
+    if CONFIG.analyzed_project_tag_regex_in_value:
+        tag_pair = tuple(CONFIG.analyzed_project_tag_regex_in_value.replace(" ", "").split(":"))
+        if len(tag_pair) != 2:
+            print(f"Unable to parse project tag: {CONFIG.analyzed_project_tag_regex_in_value}")
+            sys.exit("Expected format of project tags: <name:value>")
+        else:
+            CONFIG.tag_pair = tag_pair
 
+    if CONFIG.days_to_keep is None:
+        print("Days to keep was not provided, defaulting to 21")
+        CONFIG.days_to_keep = 21
+    
+    CONFIG.included_product_tokens = CONFIG.included_product_tokens.replace(" ", "").split(",") if CONFIG.included_product_tokens else []
+    CONFIG.excluded_product_tokens = CONFIG.excluded_product_tokens.replace(" ", "").split(",") if CONFIG.excluded_product_tokens else []
+    CONFIG.excluded_project_tokens = CONFIG.excluded_project_tokens.replace(" ", "").split(",") if CONFIG.excluded_project_tokens else []
+    CONFIG.excluded_project_name_patterns = CONFIG.excluded_project_name_patterns.split(",") if CONFIG.excluded_project_name_patterns else []
+    CONFIG.report_types = CONFIG.report_types if CONFIG.report_types else []
+
+    if CONFIG.excluded_project_name_patterns:
+        CONFIG.project_name_exclude_list = CONFIG.excluded_project_name_patterns
+   
 
-if __name__ == '__main__':
-    main()
+if __name__ == "__main__":
+    main()
```

## Comparing `ws_cleanup_tool-23.2.1.dist-info/LICENSE` & `ws_cleanup_tool-23.6.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ws_cleanup_tool-23.2.1.dist-info/METADATA` & `ws_cleanup_tool-23.6.1.5.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,149 +1,174 @@
 Metadata-Version: 2.1
 Name: ws-cleanup-tool
-Version: 23.2.1
-Summary: WS Cleanup Tool
-Home-page: https://github.com/whitesource-ps/ws-cleanup-tool
-Author: WhiteSource Professional Services
+Version: 23.6.1.5
+Summary: Mend SCA Cleanup Tool
+Home-page: https://github.com/whitesource-ps/mend-sca-cleanup-tool
+Author: Mend Professional Services
 Author-email: ps@whitesourcesoftware.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: configparser (==5.3.0)
 Requires-Dist: DateTime (~=4.3)
-Requires-Dist: ws-sdk (==22.8.4.2)
 
 [![Logo](https://resources.mend.io/mend-sig/logo/mend-dark-logo-horizontal.png)](https://www.mend.io/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
-[![WS projects cleanup](https://github.com/whitesource-ps/ws-cleanup-tool/actions/workflows/ci.yml/badge.svg)](https://github.com/whitesource-ps/ws-cleanup-tool/actions/workflows/ci.yml)
+[![Mend projects cleanup](https://github.com/whitesource-ps/ws-cleanup-tool/actions/workflows/ci.yml/badge.svg)](https://github.com/whitesource-ps/ws-cleanup-tool/actions/workflows/ci.yml)
 [![Python 3.6](https://upload.wikimedia.org/wikipedia/commons/thumb/8/8c/Blue_Python_3.6%2B_Shield_Badge.svg/86px-Blue_Python_3.6%2B_Shield_Badge.svg.png)](https://www.python.org/downloads/release/python-360/)
 [![PyPI](https://img.shields.io/pypi/v/ws-cleanup-tool?style=plastic)](https://pypi.org/project/ws-cleanup-tool/)
 
 # Mend Projects Cleanup CLI Tool
 * The self-hosted CLI tool features cleaning up projects and generating reports before deletion in 2 modes:
   * By stating _OperationMode=FilterProjectsByUpdateTime_ and how many days to keep (-r/ DaysToKeep=)
   * By stating _OperationMode=FilterProjectsByLastCreatedCopies_ and how many copies to keep (-r/ DaysToKeep=)
-* The reports are saved in the designated location as follows: _[ReportsDir]/[PRODUCT NAME]/[PROJECT NAME]/[REPORT NAME]_  
+* The reports are saved in the designated location as follows: _[Output_DIR]/[PRODUCT NAME]/[PROJECT NAME]/[REPORT NAME]_  
+  * The default location is the _[WORKING DIRECTORY]/Mend/Reports/[PRODUCT NAME]/[PROJECT NAME]/[REPORT NAME]_
 * To review the outcome before actual deletion use _-y true_ / _DryRun=True_ flag. It will _NOT_ delete any project nor create reports 
 * By default, the tool generates all possible project-level reports. By specifying ((_-t_ / _Reports=_/) it is possible to select specific reports
+  * The full list of available reports is below
 * The full parameters list is available below
 * There are two ways to configure the tool:
   * By configuring _params.config_ on the executed dir or passing a path to the file in the same format
   * By setting command line parameters as specified in the usage below
   
 ## Supported Operating Systems
 - **Linux (Bash):**	CentOS, Debian, Ubuntu, RedHat
 - **Windows (PowerShell):**	10, 2012, 2016
 
-## Pre-requisites
+## Pre-requisites 
 * Python 3.8+
 
 ## Permissions
 * The user used to execute the tool has to have "Organization Administrator" or "Product Administrator" on all the maintained products and "Organization Auditor" permissions. 
 * It is recommended to use a service user.
 
 ## Installation and Execution from PyPi (recommended):
-1. Install by executing: `pip install ws-cleanup-tool`
+1. Install by executing: `pip install mend-sca-cleanup-tool`
 2. Configure the appropriate parameters either by using the command line or in `params.config`.
-3. Execute the tool (`ws_cleanup_tool ...`). 
+3. Execute the tool (`mend_sca_cleanup_tool ...`). 
 
 ## Installation and Execution from GitHub:
-1. Download and unzip **ws-cleanup-tool.zip** 
+1. Download and unzip **mend-sca-cleanup-tool.zip** from the most recent tagged release.
 2. Install requirements: `pip install -r requirements.txt`
 3. Configure the appropriate parameters either by using the command line or `params.config`.
-4. Execute: `python cleanup_tool.py <CONFIG_FILE>` 
+4. Execute: `python sca_cleanup_tool.py <CONFIG_FILE>` 
 
 ## Examples:
 Perform dry run check-in to get to know which projects would have been deleted:  
-`ws_cleanup_tool -r 30 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -y true`
+`mend_sca_cleanup_tool -r 30 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -y true`
 
 ---
 
 Keep the last 60 days on each product, omitting a product token <PRODUCT_1> from analyzing:  
-`ws_cleanup_tool -r 60 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -e <PRODUCT_TOKEN_1>`
+`mend_sca_cleanup_tool -r 60 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -e <PRODUCT_TOKEN_1>`
 
 ---
 
 Keep only two of the newest projects in each product token PRODUCT_1 and PRODUCT_2:  
-`ws_cleanup_tool -r 2 -m FilterProjectsByLastCreatedCopies -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2>`
+`mend_sca_cleanup_tool -r 2 -m FilterProjectsByLastCreatedCopies -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2>`
 
 ---
 
 Analyze only the projects that have the specified Mend tag and keep the newest project in each product:  
-`ws_cleanup_tool -r 1 -m FilterProjectsByLastCreatedCopies -u <USER_KEY> -k <ORG_TOKEN> -g <KEY>:<VALUE>`
+`mend_sca_cleanup_tool -r 1 -m FilterProjectsByLastCreatedCopies -u <USER_KEY> -k <ORG_TOKEN> -g <KEY>:<VALUE>`
 
 ---
 
-Keep the last 2 weeks and analyze only the projects whose match their tag key and the tag value contains the specified regex:  
-`ws_cleanup_tool -r 14 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -g <KEY>:<REGEX_VALUE>`
+Keep the last 2 weeks and analyze only the projects whose match their tag key and the tag value contains the specified value:  
+`mend_sca_cleanup_tool -r 14 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -v <KEY>:<VALUE>`
 
 ---
 
 Keep the last 100 days for both PRODUCT_1 and PRODUCT_2, but do not delete the project PROJECT_1 (which is a project in one of the included products):  
-`ws_cleanup_tool -r 100 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2> -x <PROJECT_TOKEN_1>`
+`mend_sca_cleanup_tool -r 100 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2> -x <PROJECT_TOKEN_1>`
 
 ---
 
 Keep the last month for both PRODUCT_1 and PRODUCT_2, but do not delete projects that contain provided strings in their names:  
-`ws_cleanup_tool -r 31 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2> -n CI_,-test`
+`mend_sca_cleanup_tool -r 31 -m FilterProjectsByUpdateTime -u <USER_KEY> -k <ORG_TOKEN> -i <PRODUCT_TOKEN_1>,<PRODUCT_TOKEN_2> -n CI_,-test`
 
 ---
 
 
 ## Full Usage flags:
 ```shell
-usage: ws_cleanup_tool [-h] -u WS_USER_KEY -k WS_TOKEN [-a WS_URL] [-t REPORT_TYPES] [-m {FilterProjectsByUpdateTime,FilterProjectsByLastCreatedCopies}] [-o OUTPUT_DIR] [-e EXCLUDED_PRODUCT_TOKENS] [-i INCLUDED_PRODUCT_TOKENS]
+usage: ws_cleanup_tool [-h] -u MEND_USER_KEY -k MEND_TOKEN [-a MEND_URL] [-t REPORT_TYPES] [-m {FilterProjectsByUpdateTime,FilterProjectsByLastCreatedCopies}] [-o OUTPUT_DIR] [-e EXCLUDED_PRODUCT_TOKENS] [-i INCLUDED_PRODUCT_TOKENS]
                     [-g ANALYZED_PROJECT_TAG] [-r DAYS_TO_KEEP] [-p PROJECT_PARALLELISM_LEVEL] [-y DRY_RUN]
 
-WS Cleanup Tool
+Mend Cleanup Tool
 
 optional arguments:
   -h, --help            show this help message and exit
-  -u WS_USER_KEY, --userKey 
-                    WS User Key
-  -k WS_ORG_TOKEN, --orgToken
-                    WS Organization Key (API Key)
-  -a WS_URL, --wsUrl
-                    WS URL
+  -u MEND_USER_KEY, --userKey 
+                    Mend User Key
+  -k MEND_API_TOKEN, --apiToken, --orgToken
+                    Mend Organization Key (API Key)
+  -a MEND_URL, --mendUrl, --wsURL
+                    Mend URL. This value defaults to saas.whitesourcesoftware.com.
   -t REPORT_TYPES, --reportTypes
                     Report Types to generate (comma seperated list)
   -m OPERATION_MODE, --operationMode {FilterProjectsByUpdateTime,FilterProjectsByLastCreatedCopies}
                     Cleanup operation mode
   -o OUTPUT_DIR, --outputDir
                     Output directory
   -e EXCLUDED_PRODUCT_TOKENS, --excludedProductTokens
                     List of excluded products
   -i INCLUDED_PRODUCT_TOKENS, --includedProductTokens
                     List of included products
   -g ANALYZED_PROJECT_TAG, --AnalyzedProjectTag
-                    Analyze only the projects whose contain the specific Mend tag (key:value)
+                    Analyze only the projects whose contain the specific Mend tag (key:value). Case sensitive.
   -v ANALYZED_PROJECT_TAG_REGEX_IN_VALUE, --AnalyzedProjectTagRegexInValue
-                    Analyze only the projects whose match their tag key and the tag value contains the specified regex (key:regexValue)
+                    Analyze only the projects whose match their tag key and the tag value contains the specified value (key:value). Case sensitive.
+                    Note: This was originally broken in the original ws-cleanup-tool. The functionality was adjusted to work as originally written. The naming convention is a misnomer but was kept to avoid breaking existing integrations.
   -r DAYS_TO_KEEP, --DaysToKeep
                     Number of days to keep in FilterProjectsByUpdateTime or number of copies in FilterProjectsByLastCreatedCopies
   -p PROJECT_PARALLELISM_LEVEL, --ProjectParallelismLevel
                     Project parallelism level
+                    Note: This is currently not used in this version of the mend-sca-cleanup-tool. Was kept to prevent breaking existing integrations.
   -y DRY_RUN, --DryRun
                     Logging the projects that are supposed to be deleted without deleting and creating reports
                     default False
   -s SKIP_REPORT_GENERATION, --SkipReportGeneration
                     Skip report generation step
-                    default True
+                    default False
   -j SKIP_PROJECT_DELETION, --SkipProjectDeletion
                     Skip project deletion step
                     default False                                        
   -x EXCLUDED_PROJECT_TOKENS, --excludedProjectTokens
                     List of excluded projects
   -n EXCLUDED_PROJECT_NAME_PATTERNS, --excludedProjectNamePatterns
-                    List of excluded project name patterns                 
+                    List of excluded project name patterns (comma seperated list). Case sensitive.            
 ```
 
+## Available reports
+The following Mend project reports are available through the clean-up tool. These values can be specified with the -t flag to generate specific reports.
+* alerts
+* alerts_rejected_by_policy
+* attribution
+* bugs
+* due_diligence
+* ignored_alerts
+* in_house_libraries
+* inventory
+* license_compatibility
+* resolved_alerts
+* request_history
+* source_files
+* source_file_inventory
+* vulnerability
+
+## SAST Clean up
+If you need to run a clean up script for your SAST environment, please refer to the Mend SAST clean up kit in the [Mend Toolkit](https://github.com/mend-toolkit/mend-examples/tree/main/Scripts/Mend%20SAST) 
+
 **note:** The optimal cleanup scope is derived from the size of the environment, Mend scope size (memory and CPU) allocated for the server, and runtime time constraints.    
 
 
+
+
```

