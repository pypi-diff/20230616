# Comparing `tmp/pywerview-0.5.0.tar.gz` & `tmp/pywerview-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywerview-0.5.0.tar", last modified: Tue May 30 16:01:23 2023, max compression
+gzip compressed data, was "pywerview-0.5.1.tar", last modified: Fri Jun 16 11:32:15 2023, max compression
```

## Comparing `pywerview-0.5.0.tar` & `pywerview-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/
--rw-rw-r--   0 szi       (1000) szi       (1000)    35147 2021-03-17 13:39:19.000000 pywerview-0.5.0/LICENSE
--rw-rw-r--   0 szi       (1000) szi       (1000)       26 2021-03-17 13:39:19.000000 pywerview-0.5.0/MANIFEST.in
--rw-rw-r--   0 szi       (1000) szi       (1000)    18122 2023-05-30 16:01:23.569161 pywerview-0.5.0/PKG-INFO
--rw-rw-r--   0 szi       (1000) szi       (1000)    17551 2023-05-30 15:59:15.000000 pywerview-0.5.0/README.md
-drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.561161 pywerview-0.5.0/pywerview/
--rw-rw-r--   0 szi       (1000) szi       (1000)       50 2022-04-13 08:50:48.000000 pywerview-0.5.0/pywerview/__init__.py
-drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview/cli/
--rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.0/pywerview/cli/__init__.py
--rw-rw-r--   0 szi       (1000) szi       (1000)    26577 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/cli/helpers.py
--rw-rw-r--   0 szi       (1000) szi       (1000)    39496 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/cli/main.py
--rw-rw-r--   0 szi       (1000) szi       (1000)     7101 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/formatters.py
-drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview/functions/
--rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.0/pywerview/functions/__init__.py
--rw-rw-r--   0 szi       (1000) szi       (1000)    25619 2023-01-26 10:46:48.000000 pywerview-0.5.0/pywerview/functions/gpo.py
--rw-rw-r--   0 szi       (1000) szi       (1000)    14138 2023-01-26 10:46:48.000000 pywerview-0.5.0/pywerview/functions/hunting.py
--rw-rw-r--   0 szi       (1000) szi       (1000)     3387 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/functions/misc.py
--rw-rw-r--   0 szi       (1000) szi       (1000)    46585 2023-05-30 15:59:39.000000 pywerview-0.5.0/pywerview/functions/net.py
-drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview/objects/
--rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.0/pywerview/objects/__init__.py
--rw-rw-r--   0 szi       (1000) szi       (1000)     7519 2023-05-24 15:55:25.000000 pywerview-0.5.0/pywerview/objects/adobjects.py
--rw-rw-r--   0 szi       (1000) szi       (1000)     3087 2023-01-26 10:46:48.000000 pywerview-0.5.0/pywerview/objects/rpcobjects.py
--rw-rw-r--   0 szi       (1000) szi       (1000)    25526 2023-05-30 15:59:15.000000 pywerview-0.5.0/pywerview/requester.py
-drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview/worker/
--rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.0/pywerview/worker/__init__.py
--rw-rw-r--   0 szi       (1000) szi       (1000)     6947 2023-01-26 10:46:48.000000 pywerview-0.5.0/pywerview/worker/hunting.py
-drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-05-30 16:01:23.565161 pywerview-0.5.0/pywerview.egg-info/
--rw-rw-r--   0 szi       (1000) szi       (1000)    18122 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/PKG-INFO
--rw-rw-r--   0 szi       (1000) szi       (1000)      717 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/SOURCES.txt
--rw-rw-r--   0 szi       (1000) szi       (1000)       78 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/dependency_links.txt
--rw-rw-r--   0 szi       (1000) szi       (1000)       54 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/entry_points.txt
--rw-rw-r--   0 szi       (1000) szi       (1000)        1 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/not-zip-safe
--rw-rw-r--   0 szi       (1000) szi       (1000)       77 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/requires.txt
--rw-rw-r--   0 szi       (1000) szi       (1000)       10 2023-05-30 16:01:23.000000 pywerview-0.5.0/pywerview.egg-info/top_level.txt
--rw-rw-r--   0 szi       (1000) szi       (1000)       79 2023-05-30 16:01:23.569161 pywerview-0.5.0/setup.cfg
--rw-rw-r--   0 szi       (1000) szi       (1000)     1245 2023-05-24 15:55:25.000000 pywerview-0.5.0/setup.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-06-16 11:32:15.818888 pywerview-0.5.1/
+-rw-rw-r--   0 szi       (1000) szi       (1000)    35147 2021-03-17 13:39:19.000000 pywerview-0.5.1/LICENSE
+-rw-rw-r--   0 szi       (1000) szi       (1000)       26 2021-03-17 13:39:19.000000 pywerview-0.5.1/MANIFEST.in
+-rw-rw-r--   0 szi       (1000) szi       (1000)    18905 2023-06-16 11:32:15.818888 pywerview-0.5.1/PKG-INFO
+-rw-rw-r--   0 szi       (1000) szi       (1000)    18334 2023-06-16 11:07:15.000000 pywerview-0.5.1/README.md
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-06-16 11:32:15.814888 pywerview-0.5.1/pywerview/
+-rw-rw-r--   0 szi       (1000) szi       (1000)       50 2022-04-13 08:50:48.000000 pywerview-0.5.1/pywerview/__init__.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-06-16 11:32:15.814888 pywerview-0.5.1/pywerview/cli/
+-rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.1/pywerview/cli/__init__.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    27335 2023-06-16 11:07:15.000000 pywerview-0.5.1/pywerview/cli/helpers.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    40322 2023-06-16 11:07:15.000000 pywerview-0.5.1/pywerview/cli/main.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     7101 2023-05-24 15:55:25.000000 pywerview-0.5.1/pywerview/formatters.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-06-16 11:32:15.814888 pywerview-0.5.1/pywerview/functions/
+-rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.1/pywerview/functions/__init__.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    25619 2023-01-26 10:46:48.000000 pywerview-0.5.1/pywerview/functions/gpo.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    14138 2023-01-26 10:46:48.000000 pywerview-0.5.1/pywerview/functions/hunting.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     3387 2023-05-24 15:55:25.000000 pywerview-0.5.1/pywerview/functions/misc.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    47815 2023-06-16 11:07:15.000000 pywerview-0.5.1/pywerview/functions/net.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-06-16 11:32:15.818888 pywerview-0.5.1/pywerview/objects/
+-rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.1/pywerview/objects/__init__.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     7557 2023-06-16 11:07:15.000000 pywerview-0.5.1/pywerview/objects/adobjects.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     3087 2023-01-26 10:46:48.000000 pywerview-0.5.1/pywerview/objects/rpcobjects.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)    28708 2023-06-16 11:07:15.000000 pywerview-0.5.1/pywerview/requester.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-06-16 11:32:15.818888 pywerview-0.5.1/pywerview/worker/
+-rw-rw-r--   0 szi       (1000) szi       (1000)        0 2021-03-17 13:39:19.000000 pywerview-0.5.1/pywerview/worker/__init__.py
+-rw-rw-r--   0 szi       (1000) szi       (1000)     6947 2023-01-26 10:46:48.000000 pywerview-0.5.1/pywerview/worker/hunting.py
+drwxrwxr-x   0 szi       (1000) szi       (1000)        0 2023-06-16 11:32:15.814888 pywerview-0.5.1/pywerview.egg-info/
+-rw-rw-r--   0 szi       (1000) szi       (1000)    18905 2023-06-16 11:32:15.000000 pywerview-0.5.1/pywerview.egg-info/PKG-INFO
+-rw-rw-r--   0 szi       (1000) szi       (1000)      717 2023-06-16 11:32:15.000000 pywerview-0.5.1/pywerview.egg-info/SOURCES.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)       78 2023-06-16 11:32:15.000000 pywerview-0.5.1/pywerview.egg-info/dependency_links.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)       54 2023-06-16 11:32:15.000000 pywerview-0.5.1/pywerview.egg-info/entry_points.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)        1 2023-05-30 16:01:23.000000 pywerview-0.5.1/pywerview.egg-info/not-zip-safe
+-rw-rw-r--   0 szi       (1000) szi       (1000)       77 2023-06-16 11:32:15.000000 pywerview-0.5.1/pywerview.egg-info/requires.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)       10 2023-06-16 11:32:15.000000 pywerview-0.5.1/pywerview.egg-info/top_level.txt
+-rw-rw-r--   0 szi       (1000) szi       (1000)       79 2023-06-16 11:32:15.818888 pywerview-0.5.1/setup.cfg
+-rw-rw-r--   0 szi       (1000) szi       (1000)     1245 2023-06-16 11:18:37.000000 pywerview-0.5.1/setup.py
```

### Comparing `pywerview-0.5.0/LICENSE` & `pywerview-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywerview-0.5.0/PKG-INFO` & `pywerview-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywerview
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python port of PowerSploit's PowerView
 Home-page: https://github.com/the-useless-one/pywerview
 Author: Yannick Méheut
 Author-email: yannick@meheut.org
 License: GNU GPLv3
 Keywords: python powersploit pentesting recon active directory windows
 Classifier: Environment :: Console
@@ -316,14 +316,26 @@
 enabled:                 True
 ```
 
 ### JSON output
 
 Pywerview can print results in json format by using the `--json` switch.
 
+### The case of LDAP Signing and LDAP Channel Binding
+
+If you want to use pywerview against DCs that implment LDAP Signing and/or LDAP Channel Binding,
+you need to install a forked version of the `ldap3` library. You can find this special version 
+[here](https://github.com/ThePirateWhoSmellsOfSunflowers/ldap3/tree/tls_cb_and_seal_for_ntlm). 
+This version adds [this PR](https://github.com/cannatag/ldap3/pull/1087) by 
+[@ThePirateWhoSmellsOfSunflowers](https://github.com/ThePirateWhoSmellsOfSunflowers) 
+and [this one](https://github.com/cannatag/ldap3/pull/1042) by [@CravateRouge](https://github.com/CravateRouge).
+
+`pip install` this branch within your pywerview virtual env. You can check if your pywerview 
+installation uses the fork by enabling debug logging (`-l DEBUG`).
+
 ## TODO
 
 * Many, many more PowerView functionalities to implement. I'll now focus on
   forest functions, then inter-forest trust functions
 * Lots of rewrite due to the last version of PowerView
 * Gracefully fail against Unix machines running Samba
 * Perform range cycling in `get-netgroupmember`
```

### Comparing `pywerview-0.5.0/README.md` & `pywerview-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -300,14 +300,26 @@
 enabled:                 True
 ```
 
 ### JSON output
 
 Pywerview can print results in json format by using the `--json` switch.
 
+### The case of LDAP Signing and LDAP Channel Binding
+
+If you want to use pywerview against DCs that implment LDAP Signing and/or LDAP Channel Binding,
+you need to install a forked version of the `ldap3` library. You can find this special version 
+[here](https://github.com/ThePirateWhoSmellsOfSunflowers/ldap3/tree/tls_cb_and_seal_for_ntlm). 
+This version adds [this PR](https://github.com/cannatag/ldap3/pull/1087) by 
+[@ThePirateWhoSmellsOfSunflowers](https://github.com/ThePirateWhoSmellsOfSunflowers) 
+and [this one](https://github.com/cannatag/ldap3/pull/1042) by [@CravateRouge](https://github.com/CravateRouge).
+
+`pip install` this branch within your pywerview virtual env. You can check if your pywerview 
+installation uses the fork by enabling debug logging (`-l DEBUG`).
+
 ## TODO
 
 * Many, many more PowerView functionalities to implement. I'll now focus on
   forest functions, then inter-forest trust functions
 * Lots of rewrite due to the last version of PowerView
 * Gracefully fail against Unix machines running Samba
 * Perform range cycling in `get-netgroupmember`
```

### Comparing `pywerview-0.5.0/pywerview/cli/helpers.py` & `pywerview-0.5.1/pywerview/cli/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,27 +32,40 @@
                                  lmhash, nthash, do_kerberos, do_tls,
                                  user_cert, user_key)
     return requester.get_adobject(queried_domain=queried_domain,
                     queried_sid=queried_sid, queried_name=queried_name,
                     queried_sam_account_name=queried_sam_account_name,
                     ads_path=ads_path, attributes=attributes, custom_filter=custom_filter)
 
-def get_adserviceaccount(domain_controller, domain, user, password=str(),
+def get_netgmsa(domain_controller, domain, user, password=str(),
                 lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
                 user_cert=str(), user_key=str(),
                 queried_domain=str(), queried_sid=str(), queried_name=str(),
                 queried_sam_account_name=str(), ads_path=str(), resolve_sids=False):
     requester = NetRequester(domain_controller, domain, user, password,
                                  lmhash, nthash, do_kerberos, do_tls,
                                  user_cert, user_key)
-    return requester.get_adserviceaccount(queried_domain=queried_domain,
+    return requester.get_netgmsa(queried_domain=queried_domain,
                     queried_sid=queried_sid, queried_name=queried_name,
                     queried_sam_account_name=queried_sam_account_name,
                     ads_path=ads_path, resolve_sids=resolve_sids)
 
+def get_netsmsa(domain_controller, domain, user, password=str(),
+                lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
+                user_cert=str(), user_key=str(),
+                queried_domain=str(), queried_sid=str(), queried_name=str(),
+                queried_sam_account_name=str(), ads_path=str()):
+    requester = NetRequester(domain_controller, domain, user, password,
+                                 lmhash, nthash, do_kerberos, do_tls,
+                                 user_cert, user_key)
+    return requester.get_netsmsa(queried_domain=queried_domain,
+                    queried_sid=queried_sid, queried_name=queried_name,
+                    queried_sam_account_name=queried_sam_account_name,
+                    ads_path=ads_path)
+
 def get_objectacl(domain_controller, domain, user, password=str(),
                 lmhash=str(), nthash=str(), do_kerberos=False, do_tls=False,
                 queried_domain=str(), queried_sid=str(), queried_name=str(),
                 user_cert=str(), user_key=str(),
                 queried_sam_account_name=str(), ads_path=str(), sacl=False,
                 rights_filter=str(), resolve_sids=False, resolve_guids=False,
                 custom_filter=str()):
```

### Comparing `pywerview-0.5.0/pywerview/cli/main.py` & `pywerview-0.5.1/pywerview/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,32 +125,48 @@
             help='Additional ADS path')
     get_adobject_parser.add_argument('--custom-filter', dest='custom_filter',
             default=str(), help='Custom filter')
     get_adobject_parser.add_argument('--attributes', nargs='+', dest='attributes',
             default=[], help='Object attributes to return')
     get_adobject_parser.set_defaults(func=get_adobject)
 
-    # Parser for the get-adserviceaccount command
-    get_adserviceaccount_parser = subparsers.add_parser('get-adserviceaccount', help='Returns a list of all the '\
+    # Parser for the get-netgmsa command
+    get_netgmsa_parser = subparsers.add_parser('get-netgmsa', help='Returns a list of all the '\
         'gMSA of the specified domain. To retrieve passwords, you need a privileged account and '\
         'a TLS connection to the LDAP server (use the --tls switch).',
         parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
-    get_adserviceaccount_parser.add_argument('--sid', dest='queried_sid',
+    get_netgmsa_parser.add_argument('--sid', dest='queried_sid',
             help='SID to query (wildcards accepted)')
-    get_adserviceaccount_parser.add_argument('--sam-account-name', dest='queried_sam_account_name',
+    get_netgmsa_parser.add_argument('--sam-account-name', dest='queried_sam_account_name',
             help='samAccountName to query (wildcards accepted)')
-    get_adserviceaccount_parser.add_argument('--name', dest='queried_name',
+    get_netgmsa_parser.add_argument('--name', dest='queried_name',
             help='Name to query (wildcards accepted)')
-    get_adserviceaccount_parser.add_argument('-d', '--domain', dest='queried_domain',
+    get_netgmsa_parser.add_argument('-d', '--domain', dest='queried_domain',
             help='Domain to query')
-    get_adserviceaccount_parser.add_argument('-a', '--ads-path',
+    get_netgmsa_parser.add_argument('-a', '--ads-path',
             help='Additional ADS path')
-    get_adserviceaccount_parser.add_argument('--resolve-sids', dest='resolve_sids',
+    get_netgmsa_parser.add_argument('--resolve-sids', dest='resolve_sids',
             action='store_true', help='Resolve SIDs when querying PrincipalsAllowedToRetrieveManagedPassword')
-    get_adserviceaccount_parser.set_defaults(func=get_adserviceaccount)
+    get_netgmsa_parser.set_defaults(func=get_netgmsa)
+
+    # Parser for the get-netsmsa command
+    get_netsmsa_parser = subparsers.add_parser('get-netsmsa', help='Returns a list of all the '\
+        'sMSA of the specified domain.',
+        parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
+    get_netsmsa_parser.add_argument('--sid', dest='queried_sid',
+            help='SID to query (wildcards accepted)')
+    get_netsmsa_parser.add_argument('--sam-account-name', dest='queried_sam_account_name',
+            help='samAccountName to query (wildcards accepted)')
+    get_netsmsa_parser.add_argument('--name', dest='queried_name',
+            help='Name to query (wildcards accepted)')
+    get_netsmsa_parser.add_argument('-d', '--domain', dest='queried_domain',
+            help='Domain to query')
+    get_netsmsa_parser.add_argument('-a', '--ads-path',
+            help='Additional ADS path')
+    get_netsmsa_parser.set_defaults(func=get_netsmsa)
     
     # Parser for the get-objectacl command
     get_objectacl_parser = subparsers.add_parser('get-objectacl', help='Takes a domain SID, '\
         'samAccountName or name, and return the ACL of the associated object',
         parents=[ad_parser, logging_parser, json_output_parser, certificate_parser])
     get_objectacl_parser.add_argument('--sid', dest='queried_sid',
             help='SID to query (wildcards accepted)')
```

### Comparing `pywerview-0.5.0/pywerview/formatters.py` & `pywerview-0.5.1/pywerview/formatters.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.5.0/pywerview/functions/gpo.py` & `pywerview-0.5.1/pywerview/functions/gpo.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.5.0/pywerview/functions/hunting.py` & `pywerview-0.5.1/pywerview/functions/hunting.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.5.0/pywerview/functions/misc.py` & `pywerview-0.5.1/pywerview/functions/misc.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.5.0/pywerview/functions/net.py` & `pywerview-0.5.1/pywerview/functions/net.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 break
         else:
             object_filter = '(&(name=*){})'.format(custom_filter)
 
         return self._ldap_search(object_filter, adobj.ADObject, attributes=attributes)
 
     @LDAPRPCRequester._ldap_connection_init
-    def get_adserviceaccount(self, queried_domain=str(), queried_sid=str(),
+    def get_netgmsa(self, queried_domain=str(), queried_sid=str(),
                      queried_name=str(), queried_sam_account_name=str(),
                      ads_path=str(), resolve_sids=False):
         filter_objectclass = '(ObjectClass=msDS-GroupManagedServiceAccount)'
         attributes = ['samaccountname', 'distinguishedname', 'objectsid', 'description',
                       'msds-managedpassword', 'msds-groupmsamembership', 'useraccountcontrol']
 
         if not self._ldap_connection.server.ssl:
@@ -65,32 +65,58 @@
                                       ('samAccountName', escape_filter_chars(queried_sam_account_name))):
             if attr_value:
                 object_filter = '(&({}={}){})'.format(attr_desc, attr_value, filter_objectclass)
                 break
         else:
             object_filter = '(&(name=*){})'.format(filter_objectclass)
 
-        adserviceaccounts = self._ldap_search(object_filter, adobj.GMSAAccount, attributes=attributes)
+        gmsa = self._ldap_search(object_filter, adobj.GMSAAccount, attributes=attributes)
 
         # In this loop, we resolve SID (if true) and we populate 'enabled' attribute
-        for i, adserviceaccount in enumerate(adserviceaccounts):
+        for i, adserviceaccount in enumerate(gmsa):
             if resolve_sids:
                 results = list()
                 for sid in getattr(adserviceaccount, 'msds-groupmsamembership'):
                     try:
                         resolved_sid = self.get_adobject(queried_sid=sid, queried_domain=self._queried_domain, 
                                                                   attributes=['distinguishedname'])[0].distinguishedname
                     except IndexError:
                         self._logger.warning('We did not manage to resolve this SID ({}) against the DC'.format(sid))
                         resolved_sid = sid
                     results.append(resolved_sid)
-                adserviceaccounts[i].add_attributes({'msds-groupmsamembership': results})
-            adserviceaccounts[i].add_attributes({'Enabled': 'ACCOUNTDISABLE' not in adserviceaccount.useraccountcontrol})
-            adserviceaccounts[i]._attributes_dict.pop('useraccountcontrol')
-        return adserviceaccounts
+                gmsa[i].add_attributes({'msds-groupmsamembership': results})
+            gmsa[i].add_attributes({'Enabled': 'ACCOUNTDISABLE' not in adserviceaccount.useraccountcontrol})
+            gmsa[i]._attributes_dict.pop('useraccountcontrol')
+
+        return gmsa
+
+    @LDAPRPCRequester._ldap_connection_init
+    def get_netsmsa(self, queried_domain=str(), queried_sid=str(),
+                     queried_name=str(), queried_sam_account_name=str(),
+                     ads_path=str()):
+
+        filter_objectclass = '(ObjectClass=msDS-ManagedServiceAccount)'
+        attributes = ['samaccountname', 'distinguishedname', 'objectsid', 'description',
+                      'msds-hostserviceaccountbl', 'useraccountcontrol']
+        for attr_desc, attr_value in (('objectSid', queried_sid), ('name', escape_filter_chars(queried_name)),
+                                      ('samAccountName', escape_filter_chars(queried_sam_account_name))):
+            if attr_value:
+                object_filter = '(&({}={}){})'.format(attr_desc, attr_value, filter_objectclass)
+                break
+        else:
+            object_filter = '(&(name=*){})'.format(filter_objectclass)
+
+        smsas = self._ldap_search(object_filter, adobj.SMSAAccount, attributes=attributes)
+
+        # In this loop, we populate 'enabled' attribute
+        for i, adserviceaccount in enumerate(smsas):
+            smsas[i].add_attributes({'Enabled': 'ACCOUNTDISABLE' not in adserviceaccount.useraccountcontrol})
+            smsas[i]._attributes_dict.pop('useraccountcontrol')
+
+        return smsas
 
     @LDAPRPCRequester._ldap_connection_init
     def get_objectacl(self, queried_domain=str(), queried_sid=str(),
                      queried_name=str(), queried_sam_account_name=str(),
                      ads_path=str(), sacl=False, rights_filter=str(),
                      resolve_sids=False, resolve_guids=False, custom_filter=str()):
         for attr_desc, attr_value in (('objectSid', queried_sid), ('name', escape_filter_chars(queried_name)),
@@ -105,15 +131,15 @@
         # This works on a mono-domain forest, must be tested on a more complex one
         if resolve_guids:
             # Dirty fix to get base DN even if custom ADS path was given
             base_dn = ','.join(self._base_dn.split(',')[-2:])
             guid_map = {'{00000000-0000-0000-0000-000000000000}': 'All'}
             for o in self.get_adobject(ads_path='CN=Schema,CN=Configuration,{}'.format(base_dn),
                     attributes=['name', 'schemaIDGUID'], custom_filter='(schemaIDGUID=*)'):
-                        guid_map['{{{}}}'.format(o.schemaidguid)] = o.name
+                        guid_map['{}'.format(format_uuid_le(o.schemaidguid))] = o.name
 
             for o in self.get_adobject(ads_path='CN=Extended-Rights,CN=Configuration,{}'.format(base_dn),
                     attributes=['name', 'rightsGuid'], custom_filter='(objectClass=controlAccessRight)'):
                         guid_map['{{{}}}'.format(o.rightsguid.lower())] = o.name
             self._base_dn = base_dn
 
         attributes = ['distinguishedname', 'objectsid', 'ntsecuritydescriptor']
```

### Comparing `pywerview-0.5.0/pywerview/objects/adobjects.py` & `pywerview-0.5.1/pywerview/objects/adobjects.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,7 +181,9 @@
 
 class GPOLocation(ADObject):
     pass
 
 class GMSAAccount(ADObject):
     pass
 
+class SMSAAccount(ADObject):
+    pass
```

### Comparing `pywerview-0.5.0/pywerview/objects/rpcobjects.py` & `pywerview-0.5.1/pywerview/objects/rpcobjects.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.5.0/pywerview/requester.py` & `pywerview-0.5.1/pywerview/requester.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,22 +60,227 @@
         self._ads_prefix = None
         self._ldap_connection = None
         self._base_dn = None
 
         logger = logging.getLogger('pywerview_main_logger.LDAPRequester')
         self._logger = logger
 
+        # We check here if the ldap3 install supports NTLM and Kerberos encryption
+        # along with TLS channel binding
+        # https://github.com/cannatag/ldap3/pull/1087
+        # https://github.com/cannatag/ldap3/pull/1042
+        try:
+            if ldap3.SIGN and ldap3.ENCRYPT:
+                self._sign_and_seal_supported = True
+                self._logger.debug('LDAP sign and seal are supported')
+        except AttributeError:
+            self._sign_and_seal_supported = False
+            self._logger.debug('LDAP sign and seal are not supported')
+
+        try:
+            if ldap3.TLS_CHANNEL_BINDING:
+                self._tls_channel_binding_supported = True
+                self._logger.debug('TLS channel binding is supported')
+        except AttributeError:
+            self._tls_channel_binding_supported = False
+            self._logger.debug('TLS channel binding is not supported')
+
+    def _do_ntlm_auth(self, ldap_scheme, formatter, seal_and_sign=False, tls_channel_binding=False):
+        self._logger.debug('LDAP authentication with NTLM: ldap_scheme = {0} / seal_and_sign = {1} / tls_channel_binding = {2}'.format(
+                            ldap_scheme, seal_and_sign, tls_channel_binding))
+        ldap_server = ldap3.Server('{}://{}'.format(ldap_scheme, self._domain_controller), formatter=formatter)
+        user = '{}\\{}'.format(self._domain, self._user)
+        ldap_connection_kwargs = {'user': user, 'raise_exceptions': True, 'authentication': ldap3.NTLM}
+
+        if self._lmhash and self._nthash:
+            ldap_connection_kwargs['password'] = '{}:{}'.format(self._lmhash, self._nthash)
+            self._logger.debug('LDAP binding parameters: server = {0} / user = {1} '
+               '/ hash = {2}'.format(self._domain_controller, user, ldap_connection_kwargs['password']))
+        else:
+            ldap_connection_kwargs['password'] = self._password
+            self._logger.debug('LDAP binding parameters: server = {0} / user = {1} '
+               '/ password = {2}'.format(self._domain_controller, user, ldap_connection_kwargs['password']))
+
+        if seal_and_sign:
+            ldap_connection_kwargs['session_security'] = ldap3.ENCRYPT
+        elif tls_channel_binding:
+            ldap_connection_kwargs['channel_binding'] = ldap3.TLS_CHANNEL_BINDING
+
+        try:
+            ldap_connection = ldap3.Connection(ldap_server, **ldap_connection_kwargs)
+            ldap_connection.bind()
+        except ldap3.core.exceptions.LDAPSocketOpenError as e:
+                self._logger.critical(e)
+                if self._do_tls:
+                    self._logger.critical('TLS negociation failed, this error is mostly due to your host '
+                                          'not supporting SHA1 as signing algorithm for certificates')
+                sys.exit(-1)
+        except ldap3.core.exceptions.LDAPInvalidCredentialsResult:
+                self._logger.warning('Server returns LDAPInvalidCredentialsResult')
+                # https://github.com/zyn3rgy/LdapRelayScan#ldaps-channel-binding-token-requirements
+                if 'AcceptSecurityContext error, data 80090346' in ldap_connection.result['message'] and not self._tls_channel_binding_supported:
+                    self._logger.critical('Server requires Channel Binding Token and your ldap3 install does not support it. '
+                                          'Please install https://github.com/cannatag/ldap3/pull/1087 or try another authentication method')
+                    sys.exit(-1)
+                elif self._tls_channel_binding_supported == True:
+                    self._logger.warning('Falling back to TLS with channel binding')
+                    self._do_ntlm_auth(ldap_scheme, formatter, tls_channel_binding=True)
+                    return
+                else:
+                    self._logger.critical('Invalid Credentials')
+                    sys.exit(-1)
+
+        except ldap3.core.exceptions.LDAPStrongerAuthRequiredResult:
+            self._logger.warning('Server returns LDAPStrongerAuthRequiredResult')
+            if not self._sign_and_seal_supported:
+                self._logger.warning('Sealing not available, falling back to LDAPS')
+                self._do_ntlm_auth('ldaps', formatter)
+                return
+            else:
+                self._logger.warning('Falling back to NTLM sealing')
+                self._do_ntlm_auth(ldap_scheme, formatter, seal_and_sign=True)
+                return
+
+        who_am_i = ldap_connection.extend.standard.who_am_i()
+        self._logger.debug('Successfully connected to the LDAP as {}'.format(who_am_i))
+        self._ldap_connection = ldap_connection
+
+    def _do_kerberos_auth(self, ldap_scheme, formatter, seal_and_sign=False):
+        self._logger.debug('LDAP authentication with Kerberos: ldap_scheme = {0} / seal_and_sign = {1}'.format(
+                            ldap_scheme, seal_and_sign))
+        ldap_server = ldap3.Server('{}://{}'.format(ldap_scheme, self._domain_controller), formatter=formatter)
+        user = '{}@{}'.format(self._user, self._domain.upper())
+        ldap_connection_kwargs = {'user': user, 'raise_exceptions': True, 
+                                  'authentication': ldap3.SASL,
+                                  'sasl_mechanism': ldap3.KERBEROS}
+
+        if seal_and_sign:
+            ldap_connection_kwargs['session_security'] = ldap3.ENCRYPT
+
+        # Verifying if we have the correct TGS/TGT to interrogate the LDAP server
+        ccache = CCache.loadFile(os.getenv('KRB5CCNAME'))
+        principal = 'ldap/{}@{}'.format(self._domain_controller.lower(), self._queried_domain.upper())
+
+        # We look for the TGS with the right SPN
+        creds = ccache.getCredential(principal, anySPN=False)
+        if creds:
+            self._logger.debug('TGS found in KRB5CCNAME file')
+            if creds['server'].prettyPrint().lower() != creds['server'].prettyPrint():
+                self._logger.debug('SPN not in lowercase, patching SPN')
+                new_creds = self._patch_spn(creds, principal)
+                # We build a new CCache with the new ticket
+                ccache.credentials.append(new_creds)
+                temp_ccache = tempfile.NamedTemporaryFile()
+                ccache.saveFile(temp_ccache.name)
+                cred_store = {'ccache': 'FILE:{}'.format(temp_ccache.name)}
+            else:
+                cred_store = dict()
+        else:
+            self._logger.debug('TGS not found in KRB5CCNAME, looking for '
+                    'TGS with alternative SPN')
+            # If we don't find it, we search for any SPN
+            creds = ccache.getCredential(principal, anySPN=True)
+            if creds:
+                # If we find one, we build a custom TGS
+                self._logger.debug('Alternative TGS found, patching SPN')
+                new_creds = self._patch_spn(creds, principal)
+                # We build a new CCache with the new ticket
+                ccache.credentials.append(new_creds)
+                temp_ccache = tempfile.NamedTemporaryFile()
+                ccache.saveFile(temp_ccache.name)
+                cred_store = {'ccache': 'FILE:{}'.format(temp_ccache.name)}
+            else:
+                # If we don't find any, we hope for the best (TGT in cache)
+                self._logger.debug('Alternative TGS not found, using KRB5CCNAME as is '
+                        'while hoping it contains a TGT')
+                cred_store = dict()
+        ldap_connection_kwargs['cred_store'] = cred_store
+        self._logger.debug('LDAP binding parameters: server = {0} / user = {1} '
+               '/ Kerberos auth'.format(self._domain_controller, user))
+
+        try:
+            ldap_connection = ldap3.Connection(ldap_server, **ldap_connection_kwargs)
+            ldap_connection.bind()
+        except ldap3.core.exceptions.LDAPSocketOpenError as e:
+                self._logger.critical(e)
+                if self._do_tls:
+                    self._logger.critical('TLS negociation failed, this error is mostly due to your host '
+                                          'not supporting SHA1 as signing algorithm for certificates')
+                sys.exit(-1)
+
+        except ldap3.core.exceptions.LDAPStrongerAuthRequiredResult:
+            self._logger.warning('Server returns LDAPStrongerAuthRequiredResult')
+            if not self._sign_and_seal_supported:
+                self._logger.warning('Sealing not available, falling back to LDAPS')
+                self._do_kerberos_auth('ldaps', formatter)
+                return
+            else:
+                self._logger.warning('Falling back to Kerberos sealing')
+                self._do_kerberos_auth(ldap_scheme, formatter, seal_and_sign=True)
+                return
+
+        who_am_i = ldap_connection.extend.standard.who_am_i()
+        self._logger.debug('Successfully connected to the LDAP as {}'.format(who_am_i))
+        self._ldap_connection = ldap_connection
+
+    def _do_schannel_auth(self, ldap_scheme, formatter):
+        self._logger.debug('LDAP authentication with SChannel: ldap_scheme = {0}'.format(ldap_scheme))
+        ldap_server = ldap3.Server('{}://{}'.format(ldap_scheme, self._domain_controller), formatter=formatter)
+        user = None
+        tls_mode = 'Implicit'
+        tls = ldap3.Tls(local_private_key_file=self._user_key, local_certificate_file=self._user_cert, validate=ssl.CERT_NONE)
+        ldap_server.tls = tls
+        ldap_connection_kwargs = {'user': user, 'raise_exceptions': True}
+
+        # Explicit TLS, setting up StartTLS
+        if not self._do_tls:
+            tls_mode = 'Explicit'
+            self._logger.warning('Using certificate authentication but --tls not provided, setting up TLS with StartTLS')
+            ldap_connection_kwargs['authentication'] = ldap3.SASL
+            ldap_connection_kwargs['sasl_mechanism'] = ldap3.EXTERNAL
+
+        self._logger.debug('LDAP binding parameters: server = {0} / cert = {1} '
+            '/ key = {2} / {3} TLS / SChannel auth'.format(self._domain_controller, self._user_cert, self._user_key, tls_mode))
+
+        try:
+            ldap_connection = ldap3.Connection(ldap_server, **ldap_connection_kwargs)
+            ldap_connection.open()
+            ldap_connection.raise_exceptions = False
+            if not self._do_tls:
+                self._logger.debug('Sending StartTLS command')
+                if ldap_connection.start_tls():
+                    self._logger.debug('StartTLS succeeded')
+                    ldap_connection.raise_exceptions = True
+                    ldap_connection.bind()
+                else:
+                    self._logger.critical('StartTLS failed, exiting')
+                    sys.exit(-1)
+        except Exception as e:
+            # I don't really understand exception when using SChannel authentication, but if you see this message
+            # your cert and key are probably not valid
+            self._logger.critical('Exception during SChannel authentication: {}'.format(e))
+            sys.exit(-1)
+
+        who_am_i = ldap_connection.extend.standard.who_am_i()
+
+        if not who_am_i:
+            self._logger.critical('Certificate authentication failed')
+            sys.exit(-1)
+
+        self._logger.debug('Successfully connected to the LDAP as {}'.format(who_am_i))
+        self._ldap_connection = ldap_connection
+
     def _get_netfqdn(self):
         try:
             smb = SMBConnection(self._domain_controller, self._domain_controller)
         except socket.error:
             self._logger.warning('Socket error when opening the SMB connection')
             return str()
 
-        self._logger.debug('SMB loging parameters : user = {0}  / password = {1} / domain = {2} '
+        self._logger.debug('SMB loging parameters: user = {0}  / password = {1} / domain = {2} '
                            '/ LM hash = {3} / NT hash = {4}'.format(self._user, self._password,
                                                                     self._domain, self._lmhash,
                                                                     self._nthash))
 
         smb.login(self._user, self._password, domain=self._domain,
                 lmhash=self._lmhash, nthash=self._nthash)
         fqdn = smb.getServerDNSDomainName()
@@ -145,15 +350,14 @@
         self._queried_domain = queried_domain
 
         base_dn = str()
 
         if ads_prefix:
             self._ads_prefix = ads_prefix
             base_dn = '{},'.format(self._ads_prefix)
-
         if ads_path:
             # TODO: manage ADS path starting with 'GC://'
             if ads_path.upper().startswith('LDAP://'):
                 ads_path = ads_path[7:]
             self._ads_path = ads_path
             base_dn += self._ads_path
         else:
@@ -187,157 +391,21 @@
                 'ms-Mcs-AdmPwdExpirationTime': format_ad_timestamp}
 
         if self._do_tls:
             ldap_scheme = 'ldaps'
             self._logger.debug('LDAPS connection forced')
         else:
             ldap_scheme = 'ldap'
-        ldap_server = ldap3.Server('{}://{}'.format(ldap_scheme, self._domain_controller), formatter=formatter)
-        ldap_connection_kwargs = {'user': user, 'raise_exceptions': True}
 
-        # We build the authentication arguments depending on auth mode
         if self._do_kerberos:
-            self._logger.debug('LDAP authentication with Keberos')
-            ldap_connection_kwargs['authentication'] = ldap3.SASL
-            ldap_connection_kwargs['sasl_mechanism'] = ldap3.KERBEROS
-
-            # Verifying if we have the correct TGS/TGT to interrogate the LDAP server
-            ccache = CCache.loadFile(os.getenv('KRB5CCNAME'))
-            principal = 'ldap/{}@{}'.format(self._domain_controller.lower(), self._queried_domain.upper())
-
-            # We look for the TGS with the right SPN
-            creds = ccache.getCredential(principal, anySPN=False)
-            if creds:
-                self._logger.debug('TGS found in KRB5CCNAME file')
-                if creds['server'].prettyPrint().lower() != creds['server'].prettyPrint():
-                    self._logger.debug('SPN not in lowercase, patching SPN')
-                    new_creds = self._patch_spn(creds, principal)
-                    # We build a new CCache with the new ticket
-                    ccache.credentials.append(new_creds)
-                    temp_ccache = tempfile.NamedTemporaryFile()
-                    ccache.saveFile(temp_ccache.name)
-                    cred_store = {'ccache': 'FILE:{}'.format(temp_ccache.name)}
-                else:
-                    cred_store = dict()
-            else:
-                self._logger.debug('TGS not found in KRB5CCNAME, looking for '
-                        'TGS with alternative SPN')
-                # If we don't find it, we search for any SPN
-                creds = ccache.getCredential(principal, anySPN=True)
-                if creds:
-                    # If we find one, we build a custom TGS
-                    self._logger.debug('Alternative TGS found, patching SPN')
-                    new_creds = self._patch_spn(creds, principal)
-                    # We build a new CCache with the new ticket
-                    ccache.credentials.append(new_creds)
-                    temp_ccache = tempfile.NamedTemporaryFile()
-                    ccache.saveFile(temp_ccache.name)
-                    cred_store = {'ccache': 'FILE:{}'.format(temp_ccache.name)}
-                else:
-                    # If we don't find any, we hope for the best (TGT in cache)
-                    self._logger.debug('Alternative TGS not found, using KRB5CCNAME as is '
-                            'while hoping it contains a TGT')
-                    cred_store = dict()
-            ldap_connection_kwargs['cred_store'] = cred_store
-            self._logger.debug('LDAP binding parameters: server = {0} / user = {1} '
-                   '/ Kerberos auth'.format(self._domain_controller, user))
-
+            self._do_kerberos_auth(ldap_scheme, formatter)
         elif self._do_certificate:
-            tls_mode = 'Implicit'
-            self._logger.debug('LDAPS authentication with certificate')
-            tls = ldap3.Tls(local_private_key_file=self._user_key, local_certificate_file=self._user_cert, validate=ssl.CERT_NONE)
-            ldap_server.tls = tls
-            # Explicit TLS, setting up StartTLS
-            if not self._do_tls:
-                tls_mode = 'Explicit'
-                self._logger.warning('Using certificate authentication but --tls not provided, setting up TLS with StartTLS')
-                ldap_connection_kwargs['authentication'] = ldap3.SASL
-                ldap_connection_kwargs['sasl_mechanism'] = ldap3.EXTERNAL
-            self._logger.debug('LDAP binding parameters: server = {0} / cert = {1} '
-                '/ key = {2} / {3} TLS / Certificate auth'.format(self._domain_controller, self._user_cert, self._user_key, tls_mode))
-
+            self._do_schannel_auth(ldap_scheme, formatter)
         else:
-            self._logger.debug('LDAP authentication with NTLM')
-            ldap_connection_kwargs['authentication'] = ldap3.NTLM
-            if self._lmhash and self._nthash:
-                ldap_connection_kwargs['password'] = '{}:{}'.format(self._lmhash, self._nthash)
-                self._logger.debug('LDAP binding parameters: server = {0} / user = {1} '
-                   '/ hash = {2}'.format(self._domain_controller, user, ldap_connection_kwargs['password']))
-            else:
-                ldap_connection_kwargs['password'] = self._password
-                self._logger.debug('LDAP binding parameters: server = {0} / user = {1} '
-                   '/ password = {2}'.format(self._domain_controller, user, ldap_connection_kwargs['password']))
-
-        try:
-            ldap_connection = ldap3.Connection(ldap_server, **ldap_connection_kwargs)
-            try:
-                if self._do_certificate:
-                    ldap_connection.open()
-                    if not self._do_tls:
-                        # raise_exceptions = True raises an exception (oh!) during StartTLS and
-                        # I don't know why, so we disable it for a moment
-                        ldap_connection.raise_exceptions = False
-                        self._logger.debug('Sending StartTLS command')
-                        if ldap_connection.start_tls():
-                            self._logger.debug('StartTLS succeeded')
-                            # Ok, back to normal
-                            ldap_connection.raise_exceptions = True
-                            ldap_connection.bind()
-                        else:
-                            self._logger.critical('StartTLS failed, exiting')
-                            sys.exit(-1)
-                else:
-                    ldap_connection.bind()
-            except ldap3.core.exceptions.LDAPSocketOpenError as e:
-                self._logger.critical(e)
-                if self._do_tls:
-                    self._logger.critical('TLS negociation failed, this error is mostly due to your host '
-                                          'not supporting SHA1 as signing algorithm for certificates')
-                sys.exit(-1)
-            except ldap3.core.exceptions.LDAPInvalidCredentialsResult:
-                # https://github.com/zyn3rgy/LdapRelayScan#ldaps-channel-binding-token-requirements
-                if 'AcceptSecurityContext error, data 80090346' in ldap_connection.result['message']:
-                    self._logger.critical('Server requires Channel Binding Token, try again without --tls flag '
-                                           'or use certificate authentication')
-                    sys.exit(-1)
-                else:
-                    self._logger.critical('Invalid Credentials')
-                    sys.exit(-1)
-
-        except ldap3.core.exceptions.LDAPStrongerAuthRequiredResult:
-            # We need to try TLS
-            self._logger.warning('Server returns LDAPStrongerAuthRequiredResult, falling back to LDAPS')
-            ldap_server = ldap3.Server('ldaps://{}'.format(self._domain_controller), formatter=formatter)
-            ldap_connection = ldap3.Connection(ldap_server, **ldap_connection_kwargs)
-            try:
-                ldap_connection.bind()
-            except ldap3.core.exceptions.LDAPSocketOpenError as e:
-                self._logger.critical(e)
-                self._logger.critical('TLS negociation failed, this error is mostly due to your host '
-                                      'not supporting SHA1 as signing algorithm for certificates')
-                sys.exit(-1)
-
-            except ldap3.core.exceptions.LDAPInvalidCredentialsResult:
-                # https://github.com/zyn3rgy/LdapRelayScan#ldaps-channel-binding-token-requirements
-                if 'AcceptSecurityContext error, data 80090346' in ldap_connection.result['message']:
-                    self._logger.critical('Server requires Channel Binding Token and LDAP Signing, pywerview will not work')
-                    sys.exit(-1)
-                else:
-                    self._logger.critical('Invalid Credentials')
-                    sys.exit(-1)
-
-        who_am_i = ldap_connection.extend.standard.who_am_i()
-
-        # Only failed here when using certificate authentication
-        if not who_am_i:
-            self._logger.critical('Certificate authentication failed')
-            sys.exit(-1)
-
-        self._logger.debug('Successfully connected to the LDAP as {}'.format(who_am_i))
-        self._ldap_connection = ldap_connection
+            self._do_ntlm_auth(ldap_scheme, formatter)
 
     def _ldap_search(self, search_filter, class_result, attributes=list(), controls=list()):
         results = list()
 
         # if no attribute name specified, we return all attributes
         if not attributes:
             attributes =  ldap3.ALL_ATTRIBUTES
```

### Comparing `pywerview-0.5.0/pywerview/worker/hunting.py` & `pywerview-0.5.1/pywerview/worker/hunting.py`

 * *Files identical despite different names*

### Comparing `pywerview-0.5.0/pywerview.egg-info/PKG-INFO` & `pywerview-0.5.1/pywerview.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywerview
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python port of PowerSploit's PowerView
 Home-page: https://github.com/the-useless-one/pywerview
 Author: Yannick Méheut
 Author-email: yannick@meheut.org
 License: GNU GPLv3
 Keywords: python powersploit pentesting recon active directory windows
 Classifier: Environment :: Console
@@ -316,14 +316,26 @@
 enabled:                 True
 ```
 
 ### JSON output
 
 Pywerview can print results in json format by using the `--json` switch.
 
+### The case of LDAP Signing and LDAP Channel Binding
+
+If you want to use pywerview against DCs that implment LDAP Signing and/or LDAP Channel Binding,
+you need to install a forked version of the `ldap3` library. You can find this special version 
+[here](https://github.com/ThePirateWhoSmellsOfSunflowers/ldap3/tree/tls_cb_and_seal_for_ntlm). 
+This version adds [this PR](https://github.com/cannatag/ldap3/pull/1087) by 
+[@ThePirateWhoSmellsOfSunflowers](https://github.com/ThePirateWhoSmellsOfSunflowers) 
+and [this one](https://github.com/cannatag/ldap3/pull/1042) by [@CravateRouge](https://github.com/CravateRouge).
+
+`pip install` this branch within your pywerview virtual env. You can check if your pywerview 
+installation uses the fork by enabling debug logging (`-l DEBUG`).
+
 ## TODO
 
 * Many, many more PowerView functionalities to implement. I'll now focus on
   forest functions, then inter-forest trust functions
 * Lots of rewrite due to the last version of PowerView
 * Gracefully fail against Unix machines running Samba
 * Perform range cycling in `get-netgroupmember`
```

### Comparing `pywerview-0.5.0/pywerview.egg-info/SOURCES.txt` & `pywerview-0.5.1/pywerview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywerview-0.5.0/setup.py` & `pywerview-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 long_description = open('README.md').read()
 
 setup(name='pywerview',
-    version='0.5.0',
+    version='0.5.1',
     description='A Python port of PowerSploit\'s PowerView',
     long_description=long_description,
     long_description_content_type='text/markdown',
     dependency_links = ['https://github.com/SecureAuthCorp/impacket/tarball/master#egg=impacket-0.9.22'],
     classifiers=[
         'Environment :: Console',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
```

