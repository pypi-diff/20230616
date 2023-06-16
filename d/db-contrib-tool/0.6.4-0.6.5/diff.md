# Comparing `tmp/db_contrib_tool-0.6.4.tar.gz` & `tmp/db_contrib_tool-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_contrib_tool-0.6.4.tar", max compression
+gzip compressed data, was "db_contrib_tool-0.6.5.tar", max compression
```

## Comparing `db_contrib_tool-0.6.4.tar` & `db_contrib_tool-0.6.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     5222 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/README.md
--rw-r--r--   0        0        0     2139 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/pyproject.toml
--rw-r--r--   0        0        0       13 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/__init__.py
--rw-r--r--   0        0        0      883 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/cli.py
--rw-r--r--   0        0        0        0 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/clients/__init__.py
--rw-r--r--   0        0        0     7147 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/clients/download_client.py
--rw-r--r--   0        0        0     1329 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/clients/file_service.py
--rw-r--r--   0        0        0     2636 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/clients/git_client.py
--rw-r--r--   0        0        0      305 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/clients/io_client.py
--rw-r--r--   0        0        0      984 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/clients/platform_details.py
--rw-r--r--   0        0        0     2524 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/clients/resmoke_proxy.py
--rw-r--r--   0        0        0     9291 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/config/setup_repro_env_config.yml
--rw-r--r--   0        0        0     5999 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/config.py
--rw-r--r--   0        0        0     8844 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/evg_aware_bisect/__init__.py
--rw-r--r--   0        0        0     4639 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/evg_aware_bisect/cli.py
--rw-r--r--   0        0        0      110 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
--rw-r--r--   0        0        0      418 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
--rw-r--r--   0        0        0       52 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
--rw-r--r--   0        0        0        0 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/services/__init__.py
--rw-r--r--   0        0        0     9131 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/services/evergreen_service.py
--rw-r--r--   0        0        0     2404 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/services/git_service.py
--rw-r--r--   0        0        0     2029 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/services/platform_service.py
--rw-r--r--   0        0        0    13919 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/README.md
--rw-r--r--   0        0        0       13 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/__init__.py
--rw-r--r--   0        0        0    17392 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
--rw-r--r--   0        0        0     9368 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/cli.py
--rw-r--r--   0        0        0     8290 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/download_service.py
--rw-r--r--   0        0        0     4513 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
--rw-r--r--   0        0        0     5586 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/release_models.py
--rw-r--r--   0        0        0     3155 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/request_models.py
--rw-r--r--   0        0        0    11018 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
--rw-r--r--   0        0        0      614 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/symbolizer/README.md
--rw-r--r--   0        0        0        0 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/symbolizer/__init__.py
--rw-r--r--   0        0        0     4190 2023-05-16 07:29:22.438911 db_contrib_tool-0.6.4/src/db_contrib_tool/symbolizer/cli.py
--rw-r--r--   0        0        0     4798 2023-05-16 07:29:22.442911 db_contrib_tool-0.6.4/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
--rw-r--r--   0        0        0    24229 2023-05-16 07:29:22.442911 db_contrib_tool-0.6.4/src/db_contrib_tool/symbolizer/mongosymb.py
--rw-r--r--   0        0        0     2269 2023-05-16 07:29:22.442911 db_contrib_tool-0.6.4/src/db_contrib_tool/usage_analytics.py
--rw-r--r--   0        0        0      235 2023-05-16 07:29:22.442911 db_contrib_tool-0.6.4/src/db_contrib_tool/utils/__init__.py
--rw-r--r--   0        0        0     1855 2023-05-16 07:29:22.442911 db_contrib_tool-0.6.4/src/db_contrib_tool/utils/build_system_options.py
--rw-r--r--   0        0        0     2160 2023-05-16 07:29:22.442911 db_contrib_tool-0.6.4/src/db_contrib_tool/utils/evergreen_conn.py
--rw-r--r--   0        0        0     1085 2023-05-16 07:29:22.442911 db_contrib_tool-0.6.4/src/db_contrib_tool/utils/filesystem.py
--rw-r--r--   0        0        0    10608 2023-05-16 07:29:22.442911 db_contrib_tool-0.6.4/src/db_contrib_tool/utils/oauth.py
--rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.4/setup.py
--rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     5222 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/README.md
+-rw-r--r--   0        0        0     2139 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/__init__.py
+-rw-r--r--   0        0        0      883 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/cli.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/clients/__init__.py
+-rw-r--r--   0        0        0     7147 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/clients/download_client.py
+-rw-r--r--   0        0        0     1329 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/clients/file_service.py
+-rw-r--r--   0        0        0     2636 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/clients/git_client.py
+-rw-r--r--   0        0        0      305 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/clients/io_client.py
+-rw-r--r--   0        0        0      984 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/clients/platform_details.py
+-rw-r--r--   0        0        0     2524 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/clients/resmoke_proxy.py
+-rw-r--r--   0        0        0     9291 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/config/setup_repro_env_config.yml
+-rw-r--r--   0        0        0     5999 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/config.py
+-rw-r--r--   0        0        0     8844 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/evg_aware_bisect/__init__.py
+-rw-r--r--   0        0        0     4639 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/evg_aware_bisect/cli.py
+-rw-r--r--   0        0        0      110 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
+-rw-r--r--   0        0        0      418 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
+-rw-r--r--   0        0        0       52 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
+-rw-r--r--   0        0        0        0 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/services/__init__.py
+-rw-r--r--   0        0        0     9131 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/services/evergreen_service.py
+-rw-r--r--   0        0        0     2404 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/services/git_service.py
+-rw-r--r--   0        0        0     2029 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/services/platform_service.py
+-rw-r--r--   0        0        0    13919 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/README.md
+-rw-r--r--   0        0        0       13 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/__init__.py
+-rw-r--r--   0        0        0    17392 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
+-rw-r--r--   0        0        0     9874 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/cli.py
+-rw-r--r--   0        0        0     9928 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/download_service.py
+-rw-r--r--   0        0        0     4513 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
+-rw-r--r--   0        0        0     5586 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/release_models.py
+-rw-r--r--   0        0        0     3155 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/request_models.py
+-rw-r--r--   0        0        0    11018 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
+-rw-r--r--   0        0        0      614 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/symbolizer/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/symbolizer/__init__.py
+-rw-r--r--   0        0        0     4190 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/symbolizer/cli.py
+-rw-r--r--   0        0        0     4798 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
+-rw-r--r--   0        0        0    24229 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/symbolizer/mongosymb.py
+-rw-r--r--   0        0        0     2269 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/usage_analytics.py
+-rw-r--r--   0        0        0      235 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/utils/__init__.py
+-rw-r--r--   0        0        0     1855 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/utils/build_system_options.py
+-rw-r--r--   0        0        0     2160 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/utils/evergreen_conn.py
+-rw-r--r--   0        0        0     1085 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/utils/filesystem.py
+-rw-r--r--   0        0        0    10608 2023-06-16 19:15:06.283436 db_contrib_tool-0.6.5/src/db_contrib_tool/utils/oauth.py
+-rw-r--r--   0        0        0     6795 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.5/setup.py
+-rw-r--r--   0        0        0     6436 1970-01-01 00:00:00.000000 db_contrib_tool-0.6.5/PKG-INFO
```

### Comparing `db_contrib_tool-0.6.4/README.md` & `db_contrib_tool-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/pyproject.toml` & `db_contrib_tool-0.6.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "db-contrib-tool"
-version = "0.6.4"
+version = "0.6.5"
 description = "The `db-contrib-tool` - MongoDB's tool for contributors."
 authors = ["DAG team <dev-prod-dag@mongodb.com>"]
 readme = "README.md"
 repository = "https://github.com/10gen/db-contrib-tool"
 include = [
     "src/db_contrib_tool/bisect/*.sh",
     "src/db_contrib_tool/config/*.yml",
```

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/cli.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/clients/download_client.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/clients/download_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/clients/file_service.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/clients/file_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/clients/git_client.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/clients/platform_details.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/clients/platform_details.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/clients/resmoke_proxy.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/clients/resmoke_proxy.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/config/setup_repro_env_config.yml` & `db_contrib_tool-0.6.5/src/db_contrib_tool/config/setup_repro_env_config.yml`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/config.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/config.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/evg_aware_bisect/__init__.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/evg_aware_bisect/__init__.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/evg_aware_bisect/cli.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/evg_aware_bisect/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/services/evergreen_service.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/services/evergreen_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/services/git_service.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/services/git_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/services/platform_service.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/services/platform_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/README.md` & `db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/cli.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,14 +189,33 @@
     "--fallbackToMaster",
     "fallback_to_master",
     is_flag=True,
     help="Fallback to downloading the latest binaries from master if the requested"
     " version is not found (Only application for mongo versions).",
 )
 @click.option("--evgVersionsFile", "evg_versions_file", type=click.Path(), hidden=True)
+@click.option(
+    "-ed",
+    "--extractDownloads",
+    "extract_downloads",
+    default=True,
+    hidden=True,
+)
+@click.option(
+    "-bn",
+    "--binariesName",
+    "binaries_name",
+    hidden=True,
+)
+@click.option(
+    "-dn",
+    "--debugsymbolsName",
+    "debugsymbols_name",
+    hidden=True,
+)
 def setup_repro_env(
     ctx: click.Context,
     install_dir: str,
     link_dir: str,
     edition: str,
     _platform: Optional[str],
     architecture: str,
@@ -210,14 +229,17 @@
     download_python_venv: bool,
     evergreen_config: Optional[str],
     debug: bool,
     require_push: bool,
     resmoke_cmd: str,
     fallback_to_master: bool,
     evg_versions_file: str,
+    extract_downloads: bool,
+    binaries_name: str,
+    debugsymbols_name: str,
 ) -> None:
     """
     Set up MongoDB repro environment.
 
     Downloads and installs particular MongoDB versions into install directory
     and symlinks the binaries to another directory. Each symlink name will
     include the binary release version, e.g. mongod-6.1. This script supports
@@ -250,14 +272,17 @@
     download_options = DownloadOptions(
         download_binaries=(not skip_binaries),
         download_symbols=download_symbols,
         download_artifacts=download_artifacts,
         download_python_venv=download_python_venv,
         install_dir=os.path.abspath(install_dir),
         link_dir=os.path.abspath(link_dir),
+        extract_downloads=extract_downloads,
+        binaries_name=binaries_name,
+        debugsymbols_name=debugsymbols_name,
     )
     setup_repro_params = SetupReproParameters(
         edition=edition.lower(),
         platform=_platform.lower() if _platform else None,
         architecture=architecture.lower(),
         variant=variant.lower() if variant else None,
         versions=massage_versions(install_last_continuous, install_last_lts, versions),
```

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/download_service.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/download_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,35 +25,44 @@
 
     * download_binaries: Should the binaries be downloaded.
     * download_symbols: Should the debug symbols be downloaded.
     * download_artifacts: Should the build artifacts be downloaded.
     * download_python_venv: Should the python virtualenv be downloaded.
     * install_dir: Directory to install downloaded artifacts.
     * link_dir: Directory to link downloaded files to.
+    * extract_downloads: Should the downloaded evergreen files be extracted.
+    * binaries_name: The name of the unextracted binaries archive.
+    * debugsymbols_name: The name of the unextracted debugsymbols archive.
     """
 
     download_binaries: bool
     download_symbols: bool
     download_artifacts: bool
     download_python_venv: bool
 
     install_dir: str
     link_dir: str
 
+    extract_downloads: bool = True
+    binaries_name: Optional[str] = None
+    debugsymbols_name: Optional[str] = None
+
 
 class DownloadUrl(NamedTuple):
     """
     Wrapper for download URL and its fallback.
 
     * primary: Primary URL.
     * fallback: Fallback URL.
+    * download_name: The name of the downloaded file if not extracted.
     """
 
     primary: str
     fallback: Optional[str] = None
+    download_name: Optional[str] = None
 
 
 class ArtifactDownloadService:
     """A service for downloading artifacts."""
 
     @inject.autoparams()
     def __init__(self, download_client: DownloadClient, file_service: FileService) -> None:
@@ -88,14 +97,15 @@
         )
         linked_dir = self.setup_mongodb(
             url_list,
             download_options.download_binaries,
             install_dir,
             download_options.link_dir,
             download_request.bin_suffix,
+            extract_downloads=download_options.extract_downloads,
         )
         return linked_dir
 
     @staticmethod
     def find_urls_to_download(
         urls: Dict[str, str],
         fallback_urls: Optional[ReleaseUrls],
@@ -113,14 +123,15 @@
         if download_options.download_binaries:
             binaries_url = urls.get("Binaries")
             if binaries_url is not None:
                 download_list.append(
                     DownloadUrl(
                         primary=binaries_url,
                         fallback=fallback_urls.binary if fallback_urls is not None else None,
+                        download_name=download_options.binaries_name,
                     )
                 )
             else:
                 raise DownloadError("Binaries download requested but not URL available")
 
         if download_options.download_artifacts:
             artifacts_url = urls.get("Artifacts")
@@ -137,14 +148,15 @@
                 or urls.get("mongo-debugsymbols.zip")
             )
             if symbols_url is not None:
                 download_list.append(
                     DownloadUrl(
                         primary=symbols_url,
                         fallback=fallback_urls.debug_symbols if fallback_urls is not None else None,
+                        download_name=download_options.debugsymbols_name,
                     )
                 )
             else:
                 raise DownloadError("Symbols download requested but not URL available")
 
         if download_options.download_python_venv:
             python_venv_url = urls.get("Python venv (see included README.txt)") or urls.get(
@@ -160,65 +172,89 @@
     def setup_mongodb(
         self,
         urls: List[DownloadUrl],
         create_symlinks: bool,
         install_dir: str,
         link_dir: str,
         bin_suffix: str,
+        extract_downloads: bool = True,
     ) -> Optional[str]:
         """
         Download artifacts from the given URLs, extract them, and create symlinks.
 
         :param urls: List of artifact URLs to download.
         :param create_symlinks: Should symlinks be created to downloaded artifacts.
         :param install_dir: Directory to extract artifacts to.
         :param link_dir: Directory to create symlinks in.
         :param bin_suffix: Suffix to append to symlink name.
+        :param extract_downloads: Whether to extract downloaded files or not.
         :return: Directory symlinks were created in.
         """
         for url in urls:
-            self.download_with_retries(url, install_dir)
+            self.download_with_retries(url, install_dir, extract_downloads)
 
-        if create_symlinks:
+        if create_symlinks and extract_downloads:
             if self.is_windows:
                 LOGGER.info(
                     "Linking to install_dir on Windows; executable have to live in different "
                     "working directories to avoid DLLs for different versions clobbering each other"
                 )
                 link_dir = self.download_client.symlink_version(bin_suffix, install_dir, None)
             else:
                 link_dir = self.download_client.symlink_version(bin_suffix, install_dir, link_dir)
             return link_dir
         return None
 
-    def download_with_retries(self, url: DownloadUrl, install_dir: str) -> None:
+    def download_with_retries(
+        self, url: DownloadUrl, install_dir: str, extract_downloads: bool
+    ) -> None:
         """
         Download and extract with retries.
 
         :param url: Primary URL to download with fallback URL.
         :param install_dir: Location to extract the contents of the downloaded URL.
+        :param extract_downloads: Whether to extract downloaded files or not.
         """
         retrying = Retrying(
             stop=stop_after_attempt(MAX_RETRIES),
             wait=wait_fixed(self.retry_time_secs),
             reraise=True,
         )
 
         try:
-            retrying(self.try_download, url.primary, install_dir)
+            retrying(
+                self.try_download, url.primary, install_dir, extract_downloads, url.download_name
+            )
         except Exception as err:
             if url.fallback is None:
                 LOGGER.error("Failed to setup from primary source...", error=err)
                 raise err
             LOGGER.warning("Failed to setup from primary source, using fallback...", error=err)
-            retrying(self.try_download, url.fallback, install_dir)
+            retrying(
+                self.try_download, url.fallback, install_dir, extract_downloads, url.download_name
+            )
 
-    def try_download(self, target_url: str, install_dir: str) -> None:
+    def try_download(
+        self,
+        target_url: str,
+        install_dir: str,
+        extract_download: bool = True,
+        download_name: Optional[str] = None,
+    ) -> None:
         """
         Attempt to download the given URL.
 
         :param target_url: URL to download.
         :param install_dir: Location to extract the contents of the downloaded URL.
+        :param extract_download: Whether to extract downloaded files or not.
+        :param download_name: The name of the downloaded file if not extracted.
         """
         tarball = self.download_client.download_from_url(target_url)
-        self.download_client.extract_archive(tarball, install_dir)
-        self.file_service.delete_file(tarball)
+        if extract_download:
+            self.download_client.extract_archive(tarball, install_dir)
+            self.file_service.delete_file(tarball)
+        else:
+            _, file_name = os.path.split(tarball)
+            if download_name:
+                file_name = download_name
+            os.makedirs(install_dir, exist_ok=True)
+            os.rename(tarball, os.path.join(install_dir, file_name))
```

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/release_discovery_service.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/release_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/release_models.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/release_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/request_models.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/request_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/setup_repro_env/setup_repro_env.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/setup_repro_env/setup_repro_env.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/symbolizer/README.md` & `db_contrib_tool-0.6.5/src/db_contrib_tool/symbolizer/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/symbolizer/cli.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/symbolizer/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/symbolizer/mongosymb.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/symbolizer/mongosymb.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/usage_analytics.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/usage_analytics.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/utils/build_system_options.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/utils/build_system_options.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/utils/evergreen_conn.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/utils/evergreen_conn.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/utils/filesystem.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/src/db_contrib_tool/utils/oauth.py` & `db_contrib_tool-0.6.5/src/db_contrib_tool/utils/oauth.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.6.4/setup.py` & `db_contrib_tool-0.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'tenacity>=8.0.1,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['db-contrib-tool = db_contrib_tool.cli:cli']}
 
 setup_kwargs = {
     'name': 'db-contrib-tool',
-    'version': '0.6.4',
+    'version': '0.6.5',
     'description': "The `db-contrib-tool` - MongoDB's tool for contributors.",
     'long_description': '# db-contrib-tool\n\nThe `db-contrib-tool` - MongoDB\'s tools for contributors.\n\n## Table of contents\n\n- [db-contrib-tool](#db-contrib-tool)\n  - [Table of contents](#table-of-contents)\n  - [Description](#description)\n  - [Dependencies](#dependencies)\n  - [Installation](#installation)\n  - [Usage](#usage)\n  - [Contributor\'s Guide (local development)](#contributors-guide-local-development)\n    - [Install project dependencies](#install-project-dependencies)\n    - [Run command line tool (local development)](#run-command-line-tool-local-development)\n    - [Run linters](#run-linters)\n    - [Run tests](#run-tests)\n    - [Pre-commit](#pre-commit)\n    - [Testing changes in mongo](#testing-changes-in-mongo)\n    - [Test pipx package](#test-pipx-package)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThe command line tool with various subcommands:\n- `bisect` - performs an evergreen-aware git-bisect to find the \'last passing version\' and \'first failing version\' of mongo\n- `setup-repro-env`\n  - [README.md](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/setup_repro_env/README.md)\n  - downloads and installs:\n    - particular MongoDB versions\n    - debug symbols\n    - artifacts (including resmoke, python scripts etc)\n    - python venv for resmoke, python scripts etc\n- `symbolize`\n  - [README.md](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/symbolizer/README.md)\n  - Symbolizes stacktraces from recent `mongod` and `mongos` binaries compiled in Evergreen, including patch builds, mainline builds, and release/production builds.\n  - Requires authenticating to an internal MongoDB symbol mapping service.\n\n## Dependencies\n\n- Python 3.9 or later (python3 from the [MongoDB Toolchain](https://github.com/10gen/toolchain-builder/blob/master/INSTALL.md) is highly recommended)\n\n## Installation\n\nMake sure [dependencies](#dependencies) are installed.\nUse [pipx](https://pypa.github.io/pipx/) to install db-contrib-tool that will be available globally on your machine:\n```bash\n$ python3 -m pip install pipx\n$ python3 -m pipx ensurepath\n```\n\nInstalling db-contrib-tool:\n```bash\n$ python3 -m pipx install db-contrib-tool\n```\n\nUpgrading db-contrib-tool:\n```bash\n$ python3 -m pipx upgrade db-contrib-tool\n```\n\n## Usage\n\nPrint out help message:\n```bash\n$ db-contrib-tool -h\n```\nMore information on the usage of `setup-repro-env` can be found [here](https://github.com/10gen/db-contrib-tool/blob/main/src/db_contrib_tool/setup_repro_env/README.md).\n\n## Contributor\'s Guide (local development)\n\n### Install project dependencies\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management.\n```bash\n$ poetry install\n```\n\n### Run command line tool (local development)\n\n```bash\n$ ENV=DEV poetry run db-contrib-tool -h\n```\n\n### Run linters\n\n```bash\n$ poetry run isort src tests\n$ poetry run black src tests\n```\n\n### Run tests\n\n```bash\n$ poetry run pytest\n```\n\n### Pre-commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time.<br>\nTo enable pre-commit on your local repository run:\n```bash\n$ poetry run pre-commit install\n```\n\nTo run pre-commit manually:\n```bash\n$ poetry run pre-commit run\n```\n\n### Testing changes in mongo\n\nThis tool is used to help run tests in the mongodb/mongo repository. On occasion, it may be\ndesirable to run a mongodb-mongo-* patch build with in-flight changes to this repository. The\nfollowing steps can be take to accomplish that.\n\n- Create a branch with the changes you wish to test.\n- Push the branch to the origin repository: `git push -u origin <branch_name>`.\n- In the "mongo" repository, edit the [evergreen/prelude_db_contrib_tool.sh](https://github.com/10gen/mongo/blob/b1a3a357af735a53981737d91fd49e5e3ae67b95/evergreen/prelude_db_contrib_tool.sh#L10)\n  to install from the git repository instead of from pypi:\n\n  ```bash\n  pipx install "git+ssh://git@github.com/<user_name>/db-contrib-tool.git@<branch_name>" || exit 1\n  ```\n\n- Create a patch build.\n\nThe patch build should now pull down the changes from your branch instead of using the published\ndb-contrib-tool.\n\n**Note**: Since the db-contrib-tool is pulled from your branch, if you need to make additional\nchanges to the tool, you can just push to the branch and then restart the desired tasks. There is\nno need to create an additional patch build unless you also need to make updates to the mongo\nrepository.\n\n### Test pipx package\n\nPipx installation recommendations can be found in [installation](#installation) section.<br>\nThe tool can be installed via pipx from your local repo:\n```bash\n$ python3 -m pipx install /path/to/db-contrib-tool\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a Github Pull Request for code review.\nThis project uses the [Evergreen Commit Queue](https://github.com/evergreen-ci/evergreen/wiki/Commit-Queue#pr).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to pypi is automatically triggered on merges to main.\n',
     'author': 'DAG team',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/10gen/db-contrib-tool',
```

### Comparing `db_contrib_tool-0.6.4/PKG-INFO` & `db_contrib_tool-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-contrib-tool
-Version: 0.6.4
+Version: 0.6.5
 Summary: The `db-contrib-tool` - MongoDB's tool for contributors.
 Home-page: https://github.com/10gen/db-contrib-tool
 Author: DAG team
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

