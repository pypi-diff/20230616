# Comparing `tmp/pulumi_ns1-3.1.0a1686906576.tar.gz` & `tmp/pulumi_ns1-3.1.0a1686930571.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ns1-3.1.0a1686906576.tar", last modified: Fri Jun 16 09:13:56 2023, max compression
+gzip compressed data, was "pulumi_ns1-3.1.0a1686930571.tar", last modified: Fri Jun 16 15:53:51 2023, max compression
```

## Comparing `pulumi_ns1-3.1.0a1686906576.tar` & `pulumi_ns1-3.1.0a1686930571.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:13:56.494993 pulumi_ns1-3.1.0a1686906576/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-16 09:13:56.494993 pulumi_ns1-3.1.0a1686906576/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:13:56.494993 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30487 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    83734 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:13:56.494993 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/data_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/dnsview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/get_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/get_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/get_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/monitoring_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/notify_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    38381 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/pulsar_job.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33237 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/record.py
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    81290 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/tsigkey.py
--rw-r--r--   0 runner    (1001) docker     (123)    85038 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:13:56.494993 pulumi_ns1-3.1.0a1686906576/pulumi_ns1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/pulumi_ns1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 09:13:56.494993 pulumi_ns1-3.1.0a1686906576/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-16 09:13:56.000000 pulumi_ns1-3.1.0a1686906576/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:53:51.238876 pulumi_ns1-3.1.0a1686930571/
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-16 15:53:51.238876 pulumi_ns1-3.1.0a1686930571/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:53:51.234876 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31243 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86906 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:53:51.238876 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/dnsview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/get_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/get_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/get_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/monitoring_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/notify_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39137 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/pulsar_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33237 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81290 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/tsigkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88846 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:53:51.234876 pulumi_ns1-3.1.0a1686930571/pulumi_ns1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-16 15:53:51.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-16 15:53:51.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:53:51.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:53:51.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 15:53:51.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 15:53:51.000000 pulumi_ns1-3.1.0a1686930571/pulumi_ns1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:53:51.238876 pulumi_ns1-3.1.0a1686930571/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-16 15:53:50.000000 pulumi_ns1-3.1.0a1686930571/setup.py
```

### Comparing `pulumi_ns1-3.1.0a1686906576/PKG-INFO` & `pulumi_ns1-3.1.0a1686930571/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.1.0a1686906576
+Version: 3.1.0a1686930571
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi ns1
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-ns1/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-ns1/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fns1.svg)](https://www.npmjs.com/package/@pulumi/ns1)
 [![Python version](https://badge.fury.io/py/pulumi-ns1.svg)](https://pypi.org/project/pulumi-ns1)
 [![NuGet version](https://badge.fury.io/nu/pulumi.ns1.svg)](https://badge.fury.io/nu/pulumi.ns1)
```

### Comparing `pulumi_ns1-3.1.0a1686906576/README.md` & `pulumi_ns1-3.1.0a1686930571/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/__init__.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/_inputs.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,14 +477,34 @@
 class RecordAnswerArgs:
     def __init__(__self__, *,
                  answer: Optional[pulumi.Input[str]] = None,
                  meta: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  region: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] answer: Space delimited string of RDATA fields dependent on the record type.
+               
+               A:
+               
+               answer = "1.2.3.4"
+               
+               CNAME:
+               
+               answer = "www.example.com"
+               
+               MX:
+               
+               answer = "5 mail.example.com"
+               
+               SRV:
+               
+               answer = "10 0 2380 node-1.example.com"
+               
+               SPF:
+               
+               answer = "v=DKIM1; k=rsa; p=XXXXXXXX"
         :param pulumi.Input[str] region: The region (Answer Group really) that this answer
                belongs to. This should be one of the names specified in `regions`. Only a
                single `region` per answer is currently supported. If you want an answer in
                multiple regions, duplicating the answer (including metadata) is the correct
                approach.
                * ` meta` - (Optional) meta is supported at the `answer` level. Meta
                is documented below.
@@ -497,14 +517,34 @@
             pulumi.set(__self__, "region", region)
 
     @property
     @pulumi.getter
     def answer(self) -> Optional[pulumi.Input[str]]:
         """
         Space delimited string of RDATA fields dependent on the record type.
+
+        A:
+
+        answer = "1.2.3.4"
+
+        CNAME:
+
+        answer = "www.example.com"
+
+        MX:
+
+        answer = "5 mail.example.com"
+
+        SRV:
+
+        answer = "10 0 2380 node-1.example.com"
+
+        SPF:
+
+        answer = "v=DKIM1; k=rsa; p=XXXXXXXX"
         """
         return pulumi.get(self, "answer")
 
     @answer.setter
     def answer(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "answer", value)
```

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/_utilities.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/api_key.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/api_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1130,14 +1130,49 @@
                  monitoring_view_jobs: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  security_manage_active_directory: Optional[pulumi.Input[bool]] = None,
                  security_manage_global2fa: Optional[pulumi.Input[bool]] = None,
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
+        Provides a NS1 Api Key resource. This can be used to create, modify, and delete api keys.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_ns1 as ns1
+
+        example_team = ns1.Team("exampleTeam")
+        example_api_key = ns1.APIKey("exampleAPIKey",
+            teams=[example_team.id],
+            ip_whitelists=[
+                "1.1.1.1",
+                "2.2.2.2",
+            ],
+            dns_view_zones=False,
+            account_manage_users=False)
+        ```
+        ## Permissions
+
+        An API key will inherit permissions from the teams it is assigned to.
+        If a key is assigned to a team and also has individual permissions set on the key, the individual permissions
+        will be overridden by the inherited team permissions.
+        In a future release, setting permissions on a key that is part of a team will be explicitly disabled.
+
+        When a key is removed from all teams completely, it will inherit whatever permissions it had previously.
+        If a key is removed from all it's teams, it will probably be necessary to run `pulumi up` a second time
+        to update the keys permissions from it's old team permissions to new key-specific permissions.
+
+        See [the NS1 API docs](https://ns1.com/api#getget-all-account-users) for an overview of permission semantics or for [more details](https://help.ns1.com/hc/en-us/articles/360024409034-Managing-user-permissions) about the individual permission flags.
+
+        ## NS1 Documentation
+
+        [ApiKeys Api Doc](https://ns1.com/api#api-key)
+
         ## Import
 
         ```sh
          $ pulumi import ns1:index/aPIKey:APIKey `ns1_apikey`
         ```
 
          So for the example above
@@ -1189,14 +1224,49 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[APIKeyArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Provides a NS1 Api Key resource. This can be used to create, modify, and delete api keys.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_ns1 as ns1
+
+        example_team = ns1.Team("exampleTeam")
+        example_api_key = ns1.APIKey("exampleAPIKey",
+            teams=[example_team.id],
+            ip_whitelists=[
+                "1.1.1.1",
+                "2.2.2.2",
+            ],
+            dns_view_zones=False,
+            account_manage_users=False)
+        ```
+        ## Permissions
+
+        An API key will inherit permissions from the teams it is assigned to.
+        If a key is assigned to a team and also has individual permissions set on the key, the individual permissions
+        will be overridden by the inherited team permissions.
+        In a future release, setting permissions on a key that is part of a team will be explicitly disabled.
+
+        When a key is removed from all teams completely, it will inherit whatever permissions it had previously.
+        If a key is removed from all it's teams, it will probably be necessary to run `pulumi up` a second time
+        to update the keys permissions from it's old team permissions to new key-specific permissions.
+
+        See [the NS1 API docs](https://ns1.com/api#getget-all-account-users) for an overview of permission semantics or for [more details](https://help.ns1.com/hc/en-us/articles/360024409034-Managing-user-permissions) about the individual permission flags.
+
+        ## NS1 Documentation
+
+        [ApiKeys Api Doc](https://ns1.com/api#api-key)
+
         ## Import
 
         ```sh
          $ pulumi import ns1:index/aPIKey:APIKey `ns1_apikey`
         ```
 
          So for the example above
```

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/application.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/config/vars.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/data_feed.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/data_feed.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/data_source.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/data_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/dnsview.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/dnsview.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/get_dns_sec.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/get_dns_sec.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/get_networks.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/get_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/get_record.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/get_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/get_zone.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/get_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/monitoring_job.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/monitoring_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/notify_list.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/notify_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/outputs.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,34 @@
 class RecordAnswer(dict):
     def __init__(__self__, *,
                  answer: Optional[str] = None,
                  meta: Optional[Mapping[str, Any]] = None,
                  region: Optional[str] = None):
         """
         :param str answer: Space delimited string of RDATA fields dependent on the record type.
+               
+               A:
+               
+               answer = "1.2.3.4"
+               
+               CNAME:
+               
+               answer = "www.example.com"
+               
+               MX:
+               
+               answer = "5 mail.example.com"
+               
+               SRV:
+               
+               answer = "10 0 2380 node-1.example.com"
+               
+               SPF:
+               
+               answer = "v=DKIM1; k=rsa; p=XXXXXXXX"
         :param str region: The region (Answer Group really) that this answer
                belongs to. This should be one of the names specified in `regions`. Only a
                single `region` per answer is currently supported. If you want an answer in
                multiple regions, duplicating the answer (including metadata) is the correct
                approach.
                * ` meta` - (Optional) meta is supported at the `answer` level. Meta
                is documented below.
@@ -479,14 +499,34 @@
             pulumi.set(__self__, "region", region)
 
     @property
     @pulumi.getter
     def answer(self) -> Optional[str]:
         """
         Space delimited string of RDATA fields dependent on the record type.
+
+        A:
+
+        answer = "1.2.3.4"
+
+        CNAME:
+
+        answer = "www.example.com"
+
+        MX:
+
+        answer = "5 mail.example.com"
+
+        SRV:
+
+        answer = "10 0 2380 node-1.example.com"
+
+        SPF:
+
+        answer = "v=DKIM1; k=rsa; p=XXXXXXXX"
         """
         return pulumi.get(self, "answer")
 
     @property
     @pulumi.getter
     def meta(self) -> Optional[Mapping[str, Any]]:
         return pulumi.get(self, "meta")
```

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/provider.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/pulsar_job.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/pulsar_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/record.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/record.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/subnet.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/team.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/tsigkey.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/tsigkey.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/user.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1183,14 +1183,58 @@
                  notify: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  security_manage_active_directory: Optional[pulumi.Input[bool]] = None,
                  security_manage_global2fa: Optional[pulumi.Input[bool]] = None,
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Provides a NS1 User resource. Creating a user sends an invitation email to the
+        user's email address. This can be used to create, modify, and delete users.
+        The credentials used must have the `manage_users` permission set.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_ns1 as ns1
+
+        example_team = ns1.Team("exampleTeam",
+            ip_whitelists=[
+                "1.1.1.1",
+                "2.2.2.2",
+            ],
+            dns_view_zones=False,
+            account_manage_users=False)
+        example_user = ns1.User("exampleUser",
+            username="example_user",
+            email="user@example.com",
+            teams=[example_team.id],
+            notify={
+                "billing": False,
+            })
+        ```
+        ## Permissions
+
+        A user will inherit permissions from the teams they are assigned to.
+        If a user is assigned to a team and also has individual permissions set on the user, the individual permissions
+        will be overridden by the inherited team permissions.
+        In a future release, setting permissions on a user that is part of a team will be explicitly disabled.
+
+        When a user is removed from all teams completely, they will inherit whatever permissions they had previously.
+        If a user is removed from all their teams, it will probably be necessary to run `pulumi up` a second time
+        to update the users permissions from their old team permissions to new user-specific permissions.
+
+        See [this NS1 Help Center article](https://help.ns1.com/hc/en-us/articles/360024409034-Managing-user-permissions) for an overview of user permission settings.
+
+        ## NS1 Documentation
+
+        [User Api Docs](https://ns1.com/api#user)
+
+        [Managing user permissions](https://help.ns1.com/hc/en-us/articles/360024409034-Managing-user-permissions)
+
         ## Import
 
         ```sh
          $ pulumi import ns1:index/user:User <name> <username>`
         ```
 
         :param str resource_name: The name of the resource.
@@ -1235,14 +1279,58 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Provides a NS1 User resource. Creating a user sends an invitation email to the
+        user's email address. This can be used to create, modify, and delete users.
+        The credentials used must have the `manage_users` permission set.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_ns1 as ns1
+
+        example_team = ns1.Team("exampleTeam",
+            ip_whitelists=[
+                "1.1.1.1",
+                "2.2.2.2",
+            ],
+            dns_view_zones=False,
+            account_manage_users=False)
+        example_user = ns1.User("exampleUser",
+            username="example_user",
+            email="user@example.com",
+            teams=[example_team.id],
+            notify={
+                "billing": False,
+            })
+        ```
+        ## Permissions
+
+        A user will inherit permissions from the teams they are assigned to.
+        If a user is assigned to a team and also has individual permissions set on the user, the individual permissions
+        will be overridden by the inherited team permissions.
+        In a future release, setting permissions on a user that is part of a team will be explicitly disabled.
+
+        When a user is removed from all teams completely, they will inherit whatever permissions they had previously.
+        If a user is removed from all their teams, it will probably be necessary to run `pulumi up` a second time
+        to update the users permissions from their old team permissions to new user-specific permissions.
+
+        See [this NS1 Help Center article](https://help.ns1.com/hc/en-us/articles/360024409034-Managing-user-permissions) for an overview of user permission settings.
+
+        ## NS1 Documentation
+
+        [User Api Docs](https://ns1.com/api#user)
+
+        [Managing user permissions](https://help.ns1.com/hc/en-us/articles/360024409034-Managing-user-permissions)
+
         ## Import
 
         ```sh
          $ pulumi import ns1:index/user:User <name> <username>`
         ```
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1/zone.py` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1.egg-info/PKG-INFO` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-ns1
-Version: 3.1.0a1686906576
+Version: 3.1.0a1686930571
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi ns1
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-ns1/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-ns1/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fns1.svg)](https://www.npmjs.com/package/@pulumi/ns1)
 [![Python version](https://badge.fury.io/py/pulumi-ns1.svg)](https://pypi.org/project/pulumi-ns1)
 [![NuGet version](https://badge.fury.io/nu/pulumi.ns1.svg)](https://badge.fury.io/nu/pulumi.ns1)
```

### Comparing `pulumi_ns1-3.1.0a1686906576/pulumi_ns1.egg-info/SOURCES.txt` & `pulumi_ns1-3.1.0a1686930571/pulumi_ns1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.1.0a1686906576/setup.py` & `pulumi_ns1-3.1.0a1686930571/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.1.0a1686906576"
-PLUGIN_VERSION = "3.1.0-alpha.1686906576+9dd82675"
+VERSION = "3.1.0a1686930571"
+PLUGIN_VERSION = "3.1.0-alpha.1686930571+ed0439c2"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'ns1', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "ns1 Pulumi Package - Development Version"
 
 
 setup(name='pulumi_ns1',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing ns1 cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

