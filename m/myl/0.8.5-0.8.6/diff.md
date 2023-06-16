# Comparing `tmp/myl-0.8.5.tar.gz` & `tmp/myl-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.8.5.tar", last modified: Thu Jun 15 06:15:18 2023, max compression
+gzip compressed data, was "myl-0.8.6.tar", last modified: Fri Jun 16 06:46:50 2023, max compression
```

## Comparing `myl-0.8.5.tar` & `myl-0.8.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:15:18.023738 myl-0.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:15:18.019739 myl-0.8.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-15 06:15:06.000000 myl-0.8.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:15:18.019739 myl-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 06:15:06.000000 myl-0.8.5/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 06:15:06.000000 myl-0.8.5/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 06:15:06.000000 myl-0.8.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 06:15:06.000000 myl-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 06:15:06.000000 myl-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42933 2023-06-15 06:15:18.019739 myl-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-15 06:15:06.000000 myl-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:15:18.019739 myl-0.8.5/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42933 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-15 06:15:18.000000 myl-0.8.5/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 06:15:17.000000 myl-0.8.5/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-15 06:15:06.000000 myl-0.8.5/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-15 06:15:06.000000 myl-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:15:18.023738 myl-0.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:50.411144 myl-0.8.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:50.407144 myl-0.8.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-16 06:46:40.000000 myl-0.8.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:50.407144 myl-0.8.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-16 06:46:40.000000 myl-0.8.6/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 06:46:40.000000 myl-0.8.6/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-16 06:46:40.000000 myl-0.8.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 06:46:40.000000 myl-0.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 06:46:40.000000 myl-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42933 2023-06-16 06:46:50.411144 myl-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-16 06:46:40.000000 myl-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:46:50.411144 myl-0.8.6/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42933 2023-06-16 06:46:50.000000 myl-0.8.6/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-16 06:46:50.000000 myl-0.8.6/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:46:50.000000 myl-0.8.6/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 06:46:50.000000 myl-0.8.6/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 06:46:50.000000 myl-0.8.6/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 06:46:50.000000 myl-0.8.6/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-06-16 06:46:40.000000 myl-0.8.6/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-16 06:46:40.000000 myl-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 06:46:50.411144 myl-0.8.6/setup.cfg
```

### Comparing `myl-0.8.5/.github/workflows/pypi.yaml` & `myl-0.8.6/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.8.5/.github/workflows/release.yaml` & `myl-0.8.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.8.5/LICENSE` & `myl-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.8.5/PKG-INFO` & `myl-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.5
+Version: 0.8.6
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.8.5/README.md` & `myl-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `myl-0.8.5/myl.egg-info/PKG-INFO` & `myl-0.8.6/myl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.5
+Version: 0.8.6
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.8.5/myl.py` & `myl-0.8.6/myl.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,24 +108,27 @@
         if args.sent or args.folder == "Sent":
             args.folder = GMAIL_SENT_FOLDER
         # elif args.folder == "INBOX":
         #     args.folder = GMAIL_ALL_FOLDER
     else:
         if args.auto:
             try:
-                settings = autodiscover(args.username, password=args.password).get("imap")
+                settings = autodiscover(
+                    args.username, password=args.password
+                ).get("imap")
             except Exception:
                 error_msg("Failed to autodiscover IMAP settings")
                 if args.debug:
                     console.print_exception(show_locals=True)
                 return 1
             LOGGER.debug(f"Discovered settings: {settings})")
             args.server = settings.get("server")
             args.port = settings.get("port", IMAP_PORT)
             args.starttls = settings.get("starttls")
+
         if args.sent:
             args.folder = "Sent"
 
     if not args.server:
         error_msg(
             "No server specified\n"
             "You need to either:\n"
@@ -184,18 +187,18 @@
                 criteria=args.search,
                 reverse=True,
                 bulk=True,
                 limit=args.count,
                 mark_seen=args.mark_seen,
                 headers_only=False,  # required for attachments
             ):
-                subj_suffix = "📎 " if len(msg.attachments) > 0 else ""
+                subj_prefix = "📎 " if len(msg.attachments) > 0 else ""
                 table.add_row(
                     msg.uid if msg.uid else "???",
-                    subj_suffix
+                    subj_prefix
                     + (msg.subject if msg.subject else "<no-subject>"),
                     msg.from_,
                     msg.date.strftime("%H:%M %d/%m/%Y") if msg.date else "???",
                 )
                 if len(table.rows) >= args.count:
                     break
```

### Comparing `myl-0.8.5/pyproject.toml` & `myl-0.8.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 keywords = ["imap", "email"]
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "imap-tools == 1.0.0",
-  "myl-discovery == 0.5.2",
+  "myl-discovery == 0.5.6",
   "rich == 13.4.2",
 ]
-version = "0.8.5"
+version = "0.8.6"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

