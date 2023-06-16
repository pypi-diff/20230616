# Comparing `tmp/gimera-0.6.90.tar.gz` & `tmp/gimera-0.6.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimera-0.6.90.tar", last modified: Mon Jun 12 21:34:53 2023, max compression
+gzip compressed data, was "gimera-0.6.91.tar", last modified: Fri Jun 16 16:03:30 2023, max compression
```

## Comparing `gimera-0.6.90.tar` & `gimera-0.6.91.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:34:53.944324 gimera-0.6.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 21:34:13.000000 gimera-0.6.90/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-12 21:34:53.948324 gimera-0.6.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-12 21:34:13.000000 gimera-0.6.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:34:53.944324 gimera-0.6.90/gimera/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-12 21:34:13.000000 gimera-0.6.90/gimera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-12 21:34:13.000000 gimera-0.6.90/gimera/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-12 21:34:13.000000 gimera-0.6.90/gimera/consts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38307 2023-06-12 21:34:13.000000 gimera-0.6.90/gimera/gimera.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-12 21:34:13.000000 gimera-0.6.90/gimera/gitcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-12 21:34:13.000000 gimera-0.6.90/gimera/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-12 21:34:13.000000 gimera-0.6.90/gimera/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:34:53.944324 gimera-0.6.90/gimera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-12 21:34:53.000000 gimera-0.6.90/gimera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-12 21:34:53.000000 gimera-0.6.90/gimera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:34:53.000000 gimera-0.6.90/gimera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-12 21:34:53.000000 gimera-0.6.90/gimera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 21:34:53.000000 gimera-0.6.90/gimera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 21:34:53.000000 gimera-0.6.90/gimera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-12 21:34:53.948324 gimera-0.6.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-12 21:34:13.000000 gimera-0.6.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.429068 gimera-0.6.91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 16:02:51.000000 gimera-0.6.91/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-16 16:03:30.429068 gimera-0.6.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-16 16:02:51.000000 gimera-0.6.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.429068 gimera-0.6.91/gimera/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/consts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37466 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/gimera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/gitcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-16 16:02:51.000000 gimera-0.6.91/gimera/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:03:30.429068 gimera-0.6.91/gimera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 16:03:30.000000 gimera-0.6.91/gimera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-16 16:03:30.429068 gimera-0.6.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-16 16:02:51.000000 gimera-0.6.91/setup.py
```

### Comparing `gimera-0.6.90/LICENSE.txt` & `gimera-0.6.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gimera-0.6.90/PKG-INFO` & `gimera-0.6.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.6.90
+Version: 0.6.91
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.6.90/README.md` & `gimera-0.6.91/README.md`

 * *Files identical despite different names*

### Comparing `gimera-0.6.90/gimera/config.py` & `gimera-0.6.91/gimera/config.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.90/gimera/gimera.py` & `gimera-0.6.91/gimera/gimera.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,14 @@
     all_submodule,
     parallel_safe,
     strict,
     recursive,
     no_patches,
     missing,
     remove_invalid_branches,
-    make_missing_patch_directories,
 ):
     if all_integrated and all_submodule:
         _raise_error("Please set either -I or -S")
     ttype = None
     ttype = REPO_TYPE_INT if all_integrated else ttype
     ttype = REPO_TYPE_SUB if all_submodule else ttype
 
@@ -213,28 +212,26 @@
         update,
         force_type=ttype,
         parallel_safe=parallel_safe,
         strict=strict,
         recursive=recursive,
         no_patches=no_patches,
         remove_invalid_branches=remove_invalid_branches,
-        make_missing_patch_directories=make_missing_patch_directories,
     )
 
 
 def _apply(
     repos,
     update,
     force_type=False,
     parallel_safe=False,
     strict=False,
     recursive=False,
     no_patches=False,
     remove_invalid_branches=False,
-    make_missing_patch_directories=False,
 ):
     """
     :param repos: user input parameter from commandline
     :param update: bool - flag from command line
     """
     config = Config(force_type=force_type, recursive=recursive)
 
@@ -250,15 +247,14 @@
         update,
         force_type,
         parallel_safe=parallel_safe,
         strict=strict,
         recursive=recursive,
         no_patches=no_patches,
         remove_invalid_branches=remove_invalid_branches,
-        make_missing_patch_directories=make_missing_patch_directories,
     )
 
 
 def _internal_apply(
     repos,
     update,
     force_type,
@@ -694,16 +690,14 @@
             main_repo.commit_dir_if_dirty(repo_yml.path, "\n".join(msg))
 
         del repo
 
         # apply patches:
         _apply_patches(
             repo_yml,
-            make_missing_patch_directories=options.get("make_missing_patch_directories")
-            or os.getenv("GIMERA_NON_INTERACTIVE") == "1",
         )
         main_repo.commit_dir_if_dirty(
             repo_yml.path, f"updated {REPO_TYPE_INT} submodule: {repo_yml.path}"
         )
         repo_yml.sha = new_sha
 
         if repo_yml.edit_patchfile:
@@ -812,28 +806,19 @@
         ):
             if not error_ok:
                 _raise_error(f"Error applying patch: {file}")
     except Exception as ex:  # pylint: disable=broad-except
         _raise_error(str(ex))
 
 
-def _apply_patches(repo_yml, make_missing_patch_directories=False):
+def _apply_patches(repo_yml):
     for patchdir in repo_yml.all_patch_dirs(rel_or_abs="absolute") or []:
         # with patchdir.path as dir:
         if not patchdir._path.exists():
-            if make_missing_patch_directories:
-                patchdir._path.mkdir(parents=True)
-            else:
-                if os.getenv("GIMERA_NON_INTERACTIVE") == "1":
-                    _raise_error(f"Directory does not exist: {patchdir._path}")
-                else:
-                    if confirm(
-                        f"Directory does not exist: {patchdir._path}\n" "Create it?\n"
-                    ):
-                        patchdir._path.mkdir(parents=True)
+            patchdir._path.mkdir(parents=True)
         for file in sorted(patchdir._path.rglob("*.patch")):
             if repo_yml.ignore_patchfile(file):
                 continue
             click.secho((f"Applying patch {file}"), fg="blue")
             # Git apply fails silently if applied within local repos
             _apply_patchfile(file, patchdir.apply_from_here_dir, error_ok=False)
```

### Comparing `gimera-0.6.90/gimera/gitcommands.py` & `gimera-0.6.91/gimera/gitcommands.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.90/gimera/repo.py` & `gimera-0.6.91/gimera/repo.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.90/gimera/tools.py` & `gimera-0.6.91/gimera/tools.py`

 * *Files identical despite different names*

### Comparing `gimera-0.6.90/gimera.egg-info/PKG-INFO` & `gimera-0.6.91/gimera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimera
-Version: 0.6.90
+Version: 0.6.91
 Summary: Handling git submodules and patches per yml
 Home-page: https://github.com/marcwimmer/gimera
 Author: Marc-Christian Wimmer
 Author-email: marc@itewimmer.de
 License: MIT
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `gimera-0.6.90/setup.py` & `gimera-0.6.91/setup.py`

 * *Files identical despite different names*

