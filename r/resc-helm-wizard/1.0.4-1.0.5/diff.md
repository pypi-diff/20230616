# Comparing `tmp/resc_helm_wizard-1.0.4.tar.gz` & `tmp/resc_helm_wizard-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resc_helm_wizard-1.0.4.tar", last modified: Wed Jun 14 14:13:24 2023, max compression
+gzip compressed data, was "resc_helm_wizard-1.0.5.tar", last modified: Fri Jun 16 07:51:12 2023, max compression
```

## Comparing `resc_helm_wizard-1.0.4.tar` & `resc_helm_wizard-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.695875 resc_helm_wizard-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/src/resc_helm_wizard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14145 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/src/resc_helm_wizard/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/config/example-values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/helm_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/helm_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/kubernetes_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/questions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/run_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-14 14:13:19.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard/vcs_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:13:24.699875 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-14 14:13:24.000000 resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.438409 resc_helm_wizard-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.438409 resc_helm_wizard-1.0.5/src/resc_helm_wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/src/resc_helm_wizard/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/config/example-values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/helm_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/helm_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/kubernetes_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/questions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/run_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-16 07:51:07.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard/vcs_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:51:12.442409 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-16 07:51:12.000000 resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/top_level.txt
```

### Comparing `resc_helm_wizard-1.0.4/PKG-INFO` & `resc_helm_wizard-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc_helm_wizard
-Version: 1.0.4
+Version: 1.0.5
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_helm_wizard-1.0.4/setup.cfg` & `resc_helm_wizard-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = resc_helm_wizard
 description = Repository Scanner - Helm Wizard
-version = 1.0.4
+version = 1.0.5
 author = ABN AMRO
 author_email = resc@nl.abnamro.com
 url = https://github.com/ABNAMRO/repository-scanner
 download_url = 
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard/common.py` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Standard Library
 import logging
 import os
-import subprocess
 import sys
 from typing import List
 from urllib.parse import urlparse
 
 # Third Party
 import pkg_resources
 import requests
 import yaml
 
 # First Party
 from resc_helm_wizard import constants, questions
 from resc_helm_wizard.helm_utilities import (
     add_helm_repository,
+    check_helm_release_exists,
     install_or_upgrade_helm_release,
-    is_chart_already_installed,
     update_helm_repository,
     validate_helm_deployment_status
 )
 from resc_helm_wizard.helm_value import HelmValue
 from resc_helm_wizard.kubernetes_utilities import create_namespace_if_not_exists
 from resc_helm_wizard.vcs_instance import VcsInstance
 
@@ -290,15 +289,16 @@
         url of the file to download
     :param file:
         path of the downloaded file
     :return: bool
         Returns true if rule downloaded successfully else returns false
     """
     downloaded = False
-    response = requests.get(url, timeout=100, verify=True)
+    verify_ssl = questions.ask_ssl_verification(msg="Do you want to verify SSL certificates for HTTPS requests?")
+    response = requests.get(url, timeout=100, verify=verify_ssl)
     with open(file, "wb") as output:
         output.write(response.content)
     if os.path.exists(file) and os.path.getsize(file) > 0:
         downloaded = True
         logging.debug(f"{file} successfully downloaded")
     else:
         logging.error("Unable to download the rule file")
@@ -330,19 +330,17 @@
     add_helm_repository()
     update_helm_repository()
 
     if rule_file_downloaded:
         namespace_created = create_namespace_if_not_exists(namespace_name=constants.NAMESPACE)
 
     if namespace_created:
-        # Check if release is already installed
-        output = subprocess.run(["helm", "list", "-n", constants.NAMESPACE], capture_output=True, text=True, check=True)
-        # Check if deployment is already running
-        chart_installed = is_chart_already_installed()
-        if constants.RELEASE_NAME in output.stdout and chart_installed:
+        # Check if release already exists
+        helm_release_exists = check_helm_release_exists()
+        if helm_release_exists:
             run_upgrade_confirm_msg = f"Release {constants.RELEASE_NAME} is already installed in " \
                                       f"{constants.NAMESPACE} namespace. Do you want to upgrade the release?"
             run_upgrade_confirm = questions.ask_user_confirmation(msg=run_upgrade_confirm_msg)
             if run_upgrade_confirm is True:
                 deployment_status = install_or_upgrade_helm_release(action="upgrade")
                 validate_helm_deployment_status()
             else:
```

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard/config/example-values.yaml` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard/config/example-values.yaml`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard/helm_utilities.py` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard/helm_utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,48 +15,35 @@
         Install or upgrade a helm release
     :param action:
         action to perform like install or upgrade
     :return: bool
         Returns true if install or upgrade succeeded else returns false
     """
     logging.info(f"Running {action}. Please wait for a moment...")
-    helm_command = ["helm", action, "-n", constants.NAMESPACE, constants.RELEASE_NAME, constants.CHART_NAME, "-f",
-                    constants.VALUES_FILE, "--set-file", "global.secretScanRulePackConfig=" + constants.RULE_FILE,
-                    "--repo", constants.RESC_HELM_REPO_URL]
+    helm_command = ["helm", action, "--timeout", constants.HELM_DEPLOY_TIMEOUT, "-n",
+                    constants.NAMESPACE, constants.RELEASE_NAME, constants.CHART_NAME, "-f",
+                    constants.VALUES_FILE, "--set-file", "global.secretScanRulePackConfig=" + constants.RULE_FILE]
     try:
         output = subprocess.check_output(helm_command)
         logging.info(output.decode("utf-8"))
         return True
     except subprocess.CalledProcessError:
         logging.error(f"An error occurred during {constants.CHART_NAME} deployment")
         return False
 
 
-def get_deployment_status_from_installed_chart() -> str:
+def check_helm_release_exists() -> bool:
     """
-        Get status of the installed chart
-    :return: str
-        Returns status of the installed chart
-    """
-    cmd = f"helm list -f {constants.CHART_NAME} -n {constants.NAMESPACE} -o json"
-    output = subprocess.check_output(cmd, shell=True)
-    chart_info = json.loads(output.decode("utf-8"))
-    if chart_info and "status" in chart_info[0]:
-        return chart_info[0]["status"]
-    return None
-
-
-def is_chart_already_installed() -> bool:
-    """
-        Checks if chart installed or not
+        Checks if helm release exists or not
     :return: bool
-        Returns true if chart already installed else returns false
+        Returns true if helm release exists else returns false
     """
-    status = get_deployment_status_from_installed_chart()
-    return bool(status == "deployed")
+    output = subprocess.run(["helm", "list", "-f", constants.RELEASE_NAME, "-n", constants.NAMESPACE],
+                            capture_output=True, text=True, check=True)
+    return bool(constants.RELEASE_NAME in output.stdout.strip())
 
 
 def get_version_from_downloaded_chart() -> str:
     """
         Get version of the downloaded chart
     :return: str
         Returns version of the downloaded chart
@@ -100,10 +87,14 @@
     """
     try:
         result = subprocess.run(['helm', 'status', constants.RELEASE_NAME, "-n", constants.NAMESPACE],
                                 capture_output=True, check=True, text=True)
         output = result.stdout.strip()
         if "STATUS: deployed" in output:
             logging.info("The deployment was successful. Visit http://127.0.0.1:30000 to get started with RESC!")
+            logging.info("Refer this link for more information on how to trigger the scan: "
+                         "https://github.com/abnamro/repository-scanner/tree/main/"
+                         "deployment/kubernetes#trigger-scanning")
     except subprocess.CalledProcessError:
-        logging.error("An error occurred during deployment.")
+        logging.error("An error occurred during deployment. Please run this command to debug any issue: "
+                      "kubectl get pods -n resc")
         sys.exit(1)
```

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard/helm_value.py` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard/helm_value.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard/kubernetes_utilities.py` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard/kubernetes_utilities.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard/questions.py` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard/questions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # Standard Library
 import os
 
 # Third Party
 import questionary
 
 # First Party
+from resc_helm_wizard import constants
 from resc_helm_wizard.validator import (
     azure_devops_token_validator,
     bitbucket_token_validator,
     github_account_name_validator,
     github_token_validator,
-    password_validator
+    github_username_validator,
+    password_validator,
+    vcs_url_validator
 )
 
 
 def ask_operating_system() -> str:
     """
         Asks user to select operating system
     :return: str
@@ -82,27 +85,35 @@
     """
         Asks user to provide vcs instances details
     :return: dict
         Returns vcs instance info
     """
     username = "NA"
     organization = ""
-    url = questionary.text(f"Please enter {vcs_type} url").unsafe_ask()
 
     if vcs_type == "GitHub":
-        username = questionary.text(f"What's your {vcs_type} username").unsafe_ask()
+        url = questionary.text(f"Please enter {vcs_type} url",
+                               default=constants.DEFAULT_GITHUB_URL,
+                               validate=vcs_url_validator).unsafe_ask()
+        username = questionary.text(f"What's your {vcs_type} username",
+                                    validate=github_username_validator).unsafe_ask()
         token = questionary.password(f"Please enter your {vcs_type} personal access token",
                                      validate=github_token_validator).unsafe_ask()
 
     if vcs_type == "Bitbucket":
+        url = questionary.text(f"Please enter {vcs_type} url",
+                               validate=vcs_url_validator).unsafe_ask()
         username = questionary.text(f"What's your {vcs_type} username").unsafe_ask()
         token = questionary.password(f"Please enter your {vcs_type} personal access token",
                                      validate=bitbucket_token_validator).unsafe_ask()
 
     if vcs_type == "Azure Devops":
+        url = questionary.text(f"Please enter {vcs_type} url",
+                               default=constants.DEFAULT_AZURE_DEVOPS_URL,
+                               validate=vcs_url_validator).unsafe_ask()
         organization = questionary.text(f"What's your organization name in {vcs_type}").unsafe_ask()
         token = questionary.password(f"Please enter your {vcs_type} personal access token",
                                      validate=azure_devops_token_validator).unsafe_ask()
     vcs_instance_info = {"url": url, "organization": organization, "username": username, "token": token}
     return vcs_instance_info
 
 
@@ -112,7 +123,19 @@
     :return: [str]
         Returns array of GitHub account names
     """
     github_accounts = questionary.text("Enter a comma separated list of GitHub accounts you want to scan",
                                        default=default_github_accounts,
                                        validate=github_account_name_validator).unsafe_ask()
     return github_accounts
+
+
+def ask_ssl_verification(msg: str) -> bool:
+    """
+        Asks for ssl verification
+    :param msg:
+        confirmation message
+    :return: bool
+        Returns True or False based on user's confirmation
+    """
+    answer = questionary.confirm(msg, default=True).unsafe_ask()
+    return answer
```

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard/run_wizard.py` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard/run_wizard.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard/validator.py` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard/validator.py`

 * *Files 26% similar despite different names*

```diff
@@ -78,12 +78,55 @@
         Otherwise, the output will return true if validation was successful
     """
     input_list = [elem.strip() for elem in github_accounts.split(",")]
     regex = re.compile(r"^[a-zA-Z\d](?:[a-zA-Z\d]|-(?=[a-zA-Z\d])){0,38}$")
     for account in input_list:
         if not re.fullmatch(regex, account):
             if account:
-                msg = f"{account} is not a valid GitHub account"
+                msg = f"{account} is not a valid GitHub account. " \
+                      f"GitHub account must contain alphanumeric characters or single hyphens, " \
+                      f"can't begin or end with a hyphen and maximum 39 characters allowed."
             else:
                 msg = "Please enter a valid comma separated list of GitHub accounts you want to scan"
             return msg
     return True
+
+
+def github_username_validator(username):
+    """
+        GitHub username validator
+    :param username:
+        username of GitHub account
+    :return: str or bool.
+        If validation fails, the output will contain a validation error message.
+        Otherwise, the output will return true if validation was successful
+    """
+    regex = re.compile(r"^[a-zA-Z\d](?:[a-zA-Z\d]|-(?=[a-zA-Z\d])){0,38}$")
+
+    if not re.fullmatch(regex, username):
+        msg = f"{username} is not a valid GitHub username. " \
+              f"GitHub username must contain alphanumeric characters or single hyphens, " \
+              f"can't begin or end with a hyphen and maximum 39 characters allowed."
+        return msg
+    return True
+
+
+def vcs_url_validator(url):
+    """
+        VCS provider url validator
+    :param url:
+        url which needs to be validated
+    :return: str or bool.
+        If validation fails, the output will contain a validation error message.
+        Otherwise, the output will return true if validation was successful
+    """
+    regex = re.compile(
+        r'^(?:http)s?://'  # Scheme
+        r'(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|'  # Domain
+        r'localhost|'  # Localhost
+        r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'  # IP address
+        r'(?::\d+)?'  # Port (optional)
+        r'(?:/?|[/?]\S+)$', re.IGNORECASE)  # Path and query (optional)
+
+    if not re.fullmatch(regex, url):
+        return "Please provide a valid URL"
+    return True
```

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard/vcs_instance.py` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard/vcs_instance.py`

 * *Files identical despite different names*

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/PKG-INFO` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resc-helm-wizard
-Version: 1.0.4
+Version: 1.0.5
 Summary: Repository Scanner - Helm Wizard
 Home-page: https://github.com/ABNAMRO/repository-scanner
 Author: ABN AMRO
 Author-email: resc@nl.abnamro.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `resc_helm_wizard-1.0.4/src/resc_helm_wizard.egg-info/SOURCES.txt` & `resc_helm_wizard-1.0.5/src/resc_helm_wizard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

