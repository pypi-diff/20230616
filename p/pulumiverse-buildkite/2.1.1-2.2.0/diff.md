# Comparing `tmp/pulumiverse_buildkite-2.1.1.tar.gz` & `tmp/pulumiverse_buildkite-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_buildkite-2.1.1.tar", last modified: Thu Jun  8 09:03:33 2023, max compression
+gzip compressed data, was "pulumiverse_buildkite-2.2.0.tar", last modified: Fri Jun 16 16:45:31 2023, max compression
```

## Comparing `pulumiverse_buildkite-2.1.1.tar` & `pulumiverse_buildkite-2.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:33.149163 pulumiverse_buildkite-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-08 09:03:33.149163 pulumiverse_buildkite-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:33.145163 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:33.149163 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/agent/agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:33.149163 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/get_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:33.149163 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/organization/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/organization/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:33.149163 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/get_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59566 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:33.149163 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/team/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/team/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/team/member.py
--rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/team/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:33.145163 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-08 09:03:33.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-08 09:03:33.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:03:33.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:03:33.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 09:03:33.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 09:03:33.000000 pulumiverse_buildkite-2.1.1/pulumiverse_buildkite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:03:33.149163 pulumiverse_buildkite-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-08 09:03:32.000000 pulumiverse_buildkite-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.258150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/agent/agent_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/get_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/get_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17692 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59466 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 16:45:31.000000 pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:45:31.262150 pulumiverse_buildkite-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-16 16:45:30.000000 pulumiverse_buildkite-2.2.0/setup.py
```

### Comparing `pulumiverse_buildkite-2.1.1/PKG-INFO` & `pulumiverse_buildkite-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_buildkite
-Version: 2.1.1
+Version: 2.2.0
 Summary: A Pulumi package for creating and managing Buildkite resources.
 Home-page: https://github.com/pulumiverse/pulumi-buildkite
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-buildkite
 Keywords: pulumi buildkite
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_buildkite-2.1.1/README.md` & `pulumiverse_buildkite-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/__init__.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/_utilities.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/agent/agent_token.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/agent/agent_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -118,22 +118,14 @@
         ```python
         import pulumi
         import pulumiverse_buildkite as buildkite
 
         fleet = buildkite.agent.AgentToken("fleet", description="token used by build fleet")
         ```
 
-        ## Import
-
-        Tokens can be imported using the `GraphQL ID` (not UUID), e.g.
-
-        ```sh
-         $ pulumi import buildkite:Agent/agentToken:AgentToken fleet QWdlbnRUb2tlbi0tLTQzNWNhZDU4LWU4MWQtNDVhZi04NjM3LWIxY2Y4MDcwMjM4ZA==
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: This is the description of the agent token.
                
                > Changing `description` will cause the resource to be destroyed and re-created.
         """
         ...
@@ -154,22 +146,14 @@
         ```python
         import pulumi
         import pulumiverse_buildkite as buildkite
 
         fleet = buildkite.agent.AgentToken("fleet", description="token used by build fleet")
         ```
 
-        ## Import
-
-        Tokens can be imported using the `GraphQL ID` (not UUID), e.g.
-
-        ```sh
-         $ pulumi import buildkite:Agent/agentToken:AgentToken fleet QWdlbnRUb2tlbi0tLTQzNWNhZDU4LWU4MWQtNDVhZi04NjM3LWIxY2Y4MDcwMjM4ZA==
-        ```
-
         :param str resource_name: The name of the resource.
         :param AgentTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(AgentTokenArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/config/vars.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/get_meta.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/get_meta.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/organization/settings.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/organization/settings.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/_inputs.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/_inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                  prefix_pull_request_fork_branch_names: Optional[pulumi.Input[bool]] = None,
                  publish_blocked_as_pending: Optional[pulumi.Input[bool]] = None,
                  publish_commit_status: Optional[pulumi.Input[bool]] = None,
                  publish_commit_status_per_step: Optional[pulumi.Input[bool]] = None,
                  pull_request_branch_filter_configuration: Optional[pulumi.Input[str]] = None,
                  pull_request_branch_filter_enabled: Optional[pulumi.Input[bool]] = None,
                  separate_pull_request_statuses: Optional[pulumi.Input[bool]] = None,
+                 skip_builds_for_existing_commits: Optional[pulumi.Input[bool]] = None,
                  skip_pull_request_builds_for_existing_commits: Optional[pulumi.Input[bool]] = None,
                  trigger_mode: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] build_branches: Whether to create builds when branches are pushed.
         :param pulumi.Input[bool] build_pull_request_forks: Whether to create builds for pull requests from third-party forks.
         :param pulumi.Input[bool] build_pull_request_labels_changed: Whether to create builds for pull requests when labels are added or removed.
         :param pulumi.Input[bool] build_pull_requests: Whether to create builds for commits that are part of a Pull Request.
@@ -51,14 +52,15 @@
         :param pulumi.Input[bool] prefix_pull_request_fork_branch_names: Prefix branch names for third-party fork builds to ensure they don't trigger branch conditions. For example, the `master` branch from `some-user` will become `some-user:master`.
         :param pulumi.Input[bool] publish_blocked_as_pending: The status to use for blocked builds. Pending can be used with [required status checks](https://help.github.com/en/articles/enabling-required-status-checks) to prevent merging pull requests with blocked builds.
         :param pulumi.Input[bool] publish_commit_status: Whether to update the status of commits in Bitbucket or GitHub.
         :param pulumi.Input[bool] publish_commit_status_per_step: Whether to create a separate status for each job in a build, allowing you to see the status of each job directly in Bitbucket or GitHub.
         :param pulumi.Input[str] pull_request_branch_filter_configuration: The branch filtering pattern. Only pull requests on branches matching this pattern will cause builds to be created.
         :param pulumi.Input[bool] pull_request_branch_filter_enabled: Whether to limit the creation of builds to specific branches or patterns.
         :param pulumi.Input[bool] separate_pull_request_statuses: Whether to create a separate status for pull request builds, allowing you to require a passing pull request build in your [required status checks](https://help.github.com/en/articles/enabling-required-status-checks) in GitHub.
+        :param pulumi.Input[bool] skip_builds_for_existing_commits: Whether to skip creating a new build if an existing build for the commit and branch already exists.
         :param pulumi.Input[bool] skip_pull_request_builds_for_existing_commits: Whether to skip creating a new build for a pull request if an existing build for the commit and branch already exists.
         :param pulumi.Input[str] trigger_mode: What type of event to trigger builds on. Must be one of:
         """
         if build_branches is not None:
             pulumi.set(__self__, "build_branches", build_branches)
         if build_pull_request_forks is not None:
             pulumi.set(__self__, "build_pull_request_forks", build_pull_request_forks)
@@ -86,14 +88,16 @@
             pulumi.set(__self__, "publish_commit_status_per_step", publish_commit_status_per_step)
         if pull_request_branch_filter_configuration is not None:
             pulumi.set(__self__, "pull_request_branch_filter_configuration", pull_request_branch_filter_configuration)
         if pull_request_branch_filter_enabled is not None:
             pulumi.set(__self__, "pull_request_branch_filter_enabled", pull_request_branch_filter_enabled)
         if separate_pull_request_statuses is not None:
             pulumi.set(__self__, "separate_pull_request_statuses", separate_pull_request_statuses)
+        if skip_builds_for_existing_commits is not None:
+            pulumi.set(__self__, "skip_builds_for_existing_commits", skip_builds_for_existing_commits)
         if skip_pull_request_builds_for_existing_commits is not None:
             pulumi.set(__self__, "skip_pull_request_builds_for_existing_commits", skip_pull_request_builds_for_existing_commits)
         if trigger_mode is not None:
             pulumi.set(__self__, "trigger_mode", trigger_mode)
 
     @property
     @pulumi.getter(name="buildBranches")
@@ -285,14 +289,26 @@
         return pulumi.get(self, "separate_pull_request_statuses")
 
     @separate_pull_request_statuses.setter
     def separate_pull_request_statuses(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "separate_pull_request_statuses", value)
 
     @property
+    @pulumi.getter(name="skipBuildsForExistingCommits")
+    def skip_builds_for_existing_commits(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether to skip creating a new build if an existing build for the commit and branch already exists.
+        """
+        return pulumi.get(self, "skip_builds_for_existing_commits")
+
+    @skip_builds_for_existing_commits.setter
+    def skip_builds_for_existing_commits(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "skip_builds_for_existing_commits", value)
+
+    @property
     @pulumi.getter(name="skipPullRequestBuildsForExistingCommits")
     def skip_pull_request_builds_for_existing_commits(self) -> Optional[pulumi.Input[bool]]:
         """
         Whether to skip creating a new build for a pull request if an existing build for the commit and branch already exists.
         """
         return pulumi.get(self, "skip_pull_request_builds_for_existing_commits")
```

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/get_pipeline.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/get_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/outputs.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
             suggest = "publish_commit_status_per_step"
         elif key == "pullRequestBranchFilterConfiguration":
             suggest = "pull_request_branch_filter_configuration"
         elif key == "pullRequestBranchFilterEnabled":
             suggest = "pull_request_branch_filter_enabled"
         elif key == "separatePullRequestStatuses":
             suggest = "separate_pull_request_statuses"
+        elif key == "skipBuildsForExistingCommits":
+            suggest = "skip_builds_for_existing_commits"
         elif key == "skipPullRequestBuildsForExistingCommits":
             suggest = "skip_pull_request_builds_for_existing_commits"
         elif key == "triggerMode":
             suggest = "trigger_mode"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in PipelineProviderSettings. Access the value via the '{suggest}' property getter instead.")
@@ -80,14 +82,15 @@
                  prefix_pull_request_fork_branch_names: Optional[bool] = None,
                  publish_blocked_as_pending: Optional[bool] = None,
                  publish_commit_status: Optional[bool] = None,
                  publish_commit_status_per_step: Optional[bool] = None,
                  pull_request_branch_filter_configuration: Optional[str] = None,
                  pull_request_branch_filter_enabled: Optional[bool] = None,
                  separate_pull_request_statuses: Optional[bool] = None,
+                 skip_builds_for_existing_commits: Optional[bool] = None,
                  skip_pull_request_builds_for_existing_commits: Optional[bool] = None,
                  trigger_mode: Optional[str] = None):
         """
         :param bool build_branches: Whether to create builds when branches are pushed.
         :param bool build_pull_request_forks: Whether to create builds for pull requests from third-party forks.
         :param bool build_pull_request_labels_changed: Whether to create builds for pull requests when labels are added or removed.
         :param bool build_pull_requests: Whether to create builds for commits that are part of a Pull Request.
@@ -102,14 +105,15 @@
         :param bool prefix_pull_request_fork_branch_names: Prefix branch names for third-party fork builds to ensure they don't trigger branch conditions. For example, the `master` branch from `some-user` will become `some-user:master`.
         :param bool publish_blocked_as_pending: The status to use for blocked builds. Pending can be used with [required status checks](https://help.github.com/en/articles/enabling-required-status-checks) to prevent merging pull requests with blocked builds.
         :param bool publish_commit_status: Whether to update the status of commits in Bitbucket or GitHub.
         :param bool publish_commit_status_per_step: Whether to create a separate status for each job in a build, allowing you to see the status of each job directly in Bitbucket or GitHub.
         :param str pull_request_branch_filter_configuration: The branch filtering pattern. Only pull requests on branches matching this pattern will cause builds to be created.
         :param bool pull_request_branch_filter_enabled: Whether to limit the creation of builds to specific branches or patterns.
         :param bool separate_pull_request_statuses: Whether to create a separate status for pull request builds, allowing you to require a passing pull request build in your [required status checks](https://help.github.com/en/articles/enabling-required-status-checks) in GitHub.
+        :param bool skip_builds_for_existing_commits: Whether to skip creating a new build if an existing build for the commit and branch already exists.
         :param bool skip_pull_request_builds_for_existing_commits: Whether to skip creating a new build for a pull request if an existing build for the commit and branch already exists.
         :param str trigger_mode: What type of event to trigger builds on. Must be one of:
         """
         if build_branches is not None:
             pulumi.set(__self__, "build_branches", build_branches)
         if build_pull_request_forks is not None:
             pulumi.set(__self__, "build_pull_request_forks", build_pull_request_forks)
@@ -137,14 +141,16 @@
             pulumi.set(__self__, "publish_commit_status_per_step", publish_commit_status_per_step)
         if pull_request_branch_filter_configuration is not None:
             pulumi.set(__self__, "pull_request_branch_filter_configuration", pull_request_branch_filter_configuration)
         if pull_request_branch_filter_enabled is not None:
             pulumi.set(__self__, "pull_request_branch_filter_enabled", pull_request_branch_filter_enabled)
         if separate_pull_request_statuses is not None:
             pulumi.set(__self__, "separate_pull_request_statuses", separate_pull_request_statuses)
+        if skip_builds_for_existing_commits is not None:
+            pulumi.set(__self__, "skip_builds_for_existing_commits", skip_builds_for_existing_commits)
         if skip_pull_request_builds_for_existing_commits is not None:
             pulumi.set(__self__, "skip_pull_request_builds_for_existing_commits", skip_pull_request_builds_for_existing_commits)
         if trigger_mode is not None:
             pulumi.set(__self__, "trigger_mode", trigger_mode)
 
     @property
     @pulumi.getter(name="buildBranches")
@@ -272,14 +278,22 @@
     def separate_pull_request_statuses(self) -> Optional[bool]:
         """
         Whether to create a separate status for pull request builds, allowing you to require a passing pull request build in your [required status checks](https://help.github.com/en/articles/enabling-required-status-checks) in GitHub.
         """
         return pulumi.get(self, "separate_pull_request_statuses")
 
     @property
+    @pulumi.getter(name="skipBuildsForExistingCommits")
+    def skip_builds_for_existing_commits(self) -> Optional[bool]:
+        """
+        Whether to skip creating a new build if an existing build for the commit and branch already exists.
+        """
+        return pulumi.get(self, "skip_builds_for_existing_commits")
+
+    @property
     @pulumi.getter(name="skipPullRequestBuildsForExistingCommits")
     def skip_pull_request_builds_for_existing_commits(self) -> Optional[bool]:
         """
         Whether to skip creating a new build for a pull request if an existing build for the commit and branch already exists.
         """
         return pulumi.get(self, "skip_pull_request_builds_for_existing_commits")
```

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/pipeline.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1013,15 +1013,15 @@
         __props__.__dict__["tags"] = tags
         __props__.__dict__["teams"] = teams
         __props__.__dict__["webhook_url"] = webhook_url
         return Pipeline(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="allowRebuilds")
-    def allow_rebuilds(self) -> pulumi.Output[Optional[bool]]:
+    def allow_rebuilds(self) -> pulumi.Output[bool]:
         """
         A boolean on whether or not to allow rebuilds for the pipeline.
         """
         return pulumi.get(self, "allow_rebuilds")
 
     @property
     @pulumi.getter(name="badgeUrl")
@@ -1029,31 +1029,31 @@
         """
         The pipeline's last build status so you can display build status badge.
         """
         return pulumi.get(self, "badge_url")
 
     @property
     @pulumi.getter(name="branchConfiguration")
-    def branch_configuration(self) -> pulumi.Output[Optional[str]]:
+    def branch_configuration(self) -> pulumi.Output[str]:
         """
         Limit which branches and tags cause new builds to be created, either via a code push or via the Builds REST API.
         """
         return pulumi.get(self, "branch_configuration")
 
     @property
     @pulumi.getter(name="cancelIntermediateBuilds")
-    def cancel_intermediate_builds(self) -> pulumi.Output[Optional[bool]]:
+    def cancel_intermediate_builds(self) -> pulumi.Output[bool]:
         """
         A boolean to enable automatically cancelling any running builds on the same branch when a new build is created.
         """
         return pulumi.get(self, "cancel_intermediate_builds")
 
     @property
     @pulumi.getter(name="cancelIntermediateBuildsBranchFilter")
-    def cancel_intermediate_builds_branch_filter(self) -> pulumi.Output[Optional[str]]:
+    def cancel_intermediate_builds_branch_filter(self) -> pulumi.Output[str]:
         """
         Limit which branches build cancelling applies to, for example !master will ensure that the master branch won't have its builds automatically cancelled.
         """
         return pulumi.get(self, "cancel_intermediate_builds_branch_filter")
 
     @property
     @pulumi.getter(name="clusterId")
@@ -1061,23 +1061,23 @@
         """
         The GraphQL ID of the cluster you want to use for the pipeline.
         """
         return pulumi.get(self, "cluster_id")
 
     @property
     @pulumi.getter(name="defaultBranch")
-    def default_branch(self) -> pulumi.Output[Optional[str]]:
+    def default_branch(self) -> pulumi.Output[str]:
         """
         The default branch to prefill when new builds are created or triggered, usually main or master but can be anything.
         """
         return pulumi.get(self, "default_branch")
 
     @property
     @pulumi.getter(name="defaultTimeoutInMinutes")
-    def default_timeout_in_minutes(self) -> pulumi.Output[Optional[int]]:
+    def default_timeout_in_minutes(self) -> pulumi.Output[int]:
         """
         The default timeout for commands in this pipeline, in minutes.
         """
         return pulumi.get(self, "default_timeout_in_minutes")
 
     @property
     @pulumi.getter(name="deletionProtection")
@@ -1085,23 +1085,23 @@
         """
         Set to either `true` or `false`. When set to `true`, `destroy` actions on a pipeline will be blocked and fail with a message "Deletion protection is enabled for pipeline: <pipeline name>"
         """
         return pulumi.get(self, "deletion_protection")
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    def description(self) -> pulumi.Output[str]:
         """
         A description of the pipeline.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="maximumTimeoutInMinutes")
-    def maximum_timeout_in_minutes(self) -> pulumi.Output[Optional[int]]:
+    def maximum_timeout_in_minutes(self) -> pulumi.Output[int]:
         """
         The maximum timeout for commands in this pipeline, in minutes.
         """
         return pulumi.get(self, "maximum_timeout_in_minutes")
 
     @property
     @pulumi.getter
@@ -1125,23 +1125,23 @@
         """
         The git URL of the repository.
         """
         return pulumi.get(self, "repository")
 
     @property
     @pulumi.getter(name="skipIntermediateBuilds")
-    def skip_intermediate_builds(self) -> pulumi.Output[Optional[bool]]:
+    def skip_intermediate_builds(self) -> pulumi.Output[bool]:
         """
         A boolean to enable automatically skipping any unstarted builds on the same branch when a new build is created.
         """
         return pulumi.get(self, "skip_intermediate_builds")
 
     @property
     @pulumi.getter(name="skipIntermediateBuildsBranchFilter")
-    def skip_intermediate_builds_branch_filter(self) -> pulumi.Output[Optional[str]]:
+    def skip_intermediate_builds_branch_filter(self) -> pulumi.Output[str]:
         """
         Limit which branches build skipping applies to, for example `!master` will ensure that the master branch won't have its builds automatically skipped.
         """
         return pulumi.get(self, "skip_intermediate_builds_branch_filter")
 
     @property
     @pulumi.getter
```

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/pipeline/schedule.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/pipeline/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/provider.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/team/get_team.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/team/member.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite/team/team.py` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite/team/team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite.egg-info/PKG-INFO` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-buildkite
-Version: 2.1.1
+Version: 2.2.0
 Summary: A Pulumi package for creating and managing Buildkite resources.
 Home-page: https://github.com/pulumiverse/pulumi-buildkite
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-buildkite
 Keywords: pulumi buildkite
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_buildkite-2.1.1/pulumiverse_buildkite.egg-info/SOURCES.txt` & `pulumiverse_buildkite-2.2.0/pulumiverse_buildkite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-2.1.1/setup.py` & `pulumiverse_buildkite-2.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.1.1"
-PLUGIN_VERSION = "2.1.1"
+VERSION = "2.2.0"
+PLUGIN_VERSION = "2.2.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'buildkite', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-buildkite'])
         except OSError as error:
```

