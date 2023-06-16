# Comparing `tmp/plone.app.content-4.0.1.tar.gz` & `tmp/plone.app.content-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.content-4.0.1.tar", last modified: Fri Nov 18 11:07:46 2022, max compression
+gzip compressed data, was "plone.app.content-4.0.2.tar", last modified: Fri Jun 16 16:57:42 2023, max compression
```

## Comparing `plone.app.content-4.0.1.tar` & `plone.app.content-4.0.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.501066 plone.app.content-4.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    36771 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    38154 2022-11-18 11:07:46.501195 plone.app.content-4.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      461 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.480943 plone.app.content-4.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      679 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.481173 plone.app.content-4.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.483276 plone.app.content-4.0.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.485150 plone.app.content-4.0.1/plone/app/content/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.490445 plone.app.content-4.0.1/plone/app/content/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    11649 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      724 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/adding.py
--rw-r--r--   0 maurits    (501) staff       (20)     5361 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2575 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/constraintypes.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6317 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/constraintypes.py
--rw-r--r--   0 maurits    (501) staff       (20)     5402 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/content_status_history.py
--rw-r--r--   0 maurits    (501) staff       (20)     6511 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/content_status_modify.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.493487 plone.app.content-4.0.1/plone/app/content/browser/contents/
--rw-r--r--   0 maurits    (501) staff       (20)    13481 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3772 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1694 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/copy.py
--rw-r--r--   0 maurits    (501) staff       (20)     1969 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/cut.py
--rw-r--r--   0 maurits    (501) staff       (20)      712 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/defaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)     3185 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     2169 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/paste.py
--rw-r--r--   0 maurits    (501) staff       (20)     4999 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/properties.py
--rw-r--r--   0 maurits    (501) staff       (20)     3143 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/rearrange.py
--rw-r--r--   0 maurits    (501) staff       (20)     4230 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/rename.py
--rw-r--r--   0 maurits    (501) staff       (20)     1883 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/tags.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.494887 plone.app.content-4.0.1/plone/app/content/browser/contents/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      202 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/templates/delete.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1065 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/templates/folder_contents.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2738 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/templates/properties.pt
--rw-r--r--   0 maurits    (501) staff       (20)      799 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/templates/rename.pt
--rw-r--r--   0 maurits    (501) staff       (20)      809 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/templates/tags.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1229 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/templates/workflow.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3880 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/contents/workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     6662 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/file.py
--rw-r--r--   0 maurits    (501) staff       (20)     3916 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/folder_publish.py
--rw-r--r--   0 maurits    (501) staff       (20)     3111 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/folderfactories.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5327 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/folderfactories.py
--rw-r--r--   0 maurits    (501) staff       (20)     1103 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/full_review_list.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1490 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/i18n.py
--rw-r--r--   0 maurits    (501) staff       (20)      362 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      523 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/query.py
--rw-r--r--   0 maurits    (501) staff       (20)     6481 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/reviewlist.py
--rw-r--r--   0 maurits    (501) staff       (20)     4896 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/selection.py
--rw-r--r--   0 maurits    (501) staff       (20)    10061 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/table.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4806 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/table.txt
--rw-r--r--   0 maurits    (501) staff       (20)     5661 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/tableview.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.496190 plone.app.content-4.0.1/plone/app/content/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)    21104 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/templates/content_status_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2326 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/templates/delete_confirmation.pt
--rw-r--r--   0 maurits    (501) staff       (20)      849 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/templates/object_rename.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4245 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/templates/select_default_page.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4372 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/templates/select_default_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)    13662 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/browser/vocabulary.py
--rw-r--r--   0 maurits    (501) staff       (20)      220 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)      744 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      969 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3453 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/namechooser.py
--rw-r--r--   0 maurits    (501) staff       (20)     4860 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/namechooser.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4665 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.500068 plone.app.content-4.0.1/plone/app/content/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/image.png
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.500447 plone.app.content-4.0.1/plone/app/content/tests/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.500662 plone.app.content-4.0.1/plone/app/content/tests/profiles/non-ascii-workflow-profile/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.478656 plone.app.content-4.0.1/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.500880 plone.app.content-4.0.1/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/
--rw-r--r--   0 maurits    (501) staff       (20)     1944 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/definition.xml
--rw-r--r--   0 maurits    (501) staff       (20)      160 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows.xml
--rw-r--r--   0 maurits    (501) staff       (20)      450 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/profiles/non-ascii-workflow.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    17169 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      786 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_adding.py
--rw-r--r--   0 maurits    (501) staff       (20)     7025 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_content_status_modify.py
--rw-r--r--   0 maurits    (501) staff       (20)    26699 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_contents.py
--rw-r--r--   0 maurits    (501) staff       (20)    18594 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_folder.py
--rw-r--r--   0 maurits    (501) staff       (20)     5289 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_folder_publish.py
--rw-r--r--   0 maurits    (501) staff       (20)      457 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_namechooser.py
--rw-r--r--   0 maurits    (501) staff       (20)     1796 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_namechooser_unit.py
--rw-r--r--   0 maurits    (501) staff       (20)     2122 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_non_ascii_characters_in_workflow_state.py
--rw-r--r--   0 maurits    (501) staff       (20)     2911 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_reviewlist.py
--rw-r--r--   0 maurits    (501) staff       (20)     4862 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_selectdefaultpage.py
--rw-r--r--   0 maurits    (501) staff       (20)      386 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_table.py
--rw-r--r--   0 maurits    (501) staff       (20)    25303 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/tests/test_widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)     1049 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/plone/app/content/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2022-11-18 11:07:46.483048 plone.app.content-4.0.1/plone.app.content.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    38154 2022-11-18 11:07:46.000000 plone.app.content-4.0.1/plone.app.content.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     3683 2022-11-18 11:07:46.000000 plone.app.content-4.0.1/plone.app.content.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-11-18 11:07:46.000000 plone.app.content-4.0.1/plone.app.content.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2022-11-18 11:07:46.000000 plone.app.content-4.0.1/plone.app.content.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2022-11-18 11:07:46.000000 plone.app.content-4.0.1/plone.app.content.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      228 2022-11-18 11:07:46.000000 plone.app.content-4.0.1/plone.app.content.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2022-11-18 11:07:46.000000 plone.app.content-4.0.1/plone.app.content.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      172 2022-11-18 11:07:46.501598 plone.app.content-4.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1795 2022-11-18 11:07:45.000000 plone.app.content-4.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.667191 plone.app.content-4.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    36967 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    38350 2023-06-16 16:57:42.667331 plone.app.content-4.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      461 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.642376 plone.app.content-4.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.642631 plone.app.content-4.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.644923 plone.app.content-4.0.2/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.647665 plone.app.content-4.0.2/plone/app/content/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.654408 plone.app.content-4.0.2/plone/app/content/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11649 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      724 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/adding.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5361 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2575 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/constraintypes.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6317 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/constraintypes.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5402 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/content_status_history.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6511 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/content_status_modify.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.657952 plone.app.content-4.0.2/plone/app/content/browser/contents/
+-rw-r--r--   0 maurits    (501) staff       (20)    13481 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3772 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1694 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/copy.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1969 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/cut.py
+-rw-r--r--   0 maurits    (501) staff       (20)      712 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/defaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3185 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/delete.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2169 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/paste.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4999 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/properties.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3143 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/rearrange.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4230 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/rename.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1883 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/tags.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.659626 plone.app.content-4.0.2/plone/app/content/browser/contents/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)      202 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/templates/delete.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1065 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/templates/folder_contents.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2738 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/templates/properties.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      799 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/templates/rename.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      809 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/templates/tags.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1229 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/templates/workflow.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3880 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/contents/workflow.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6662 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/file.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3916 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/folder_publish.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3111 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/folderfactories.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5327 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/folderfactories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1103 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/full_review_list.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1490 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/i18n.py
+-rw-r--r--   0 maurits    (501) staff       (20)      362 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      523 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/query.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6481 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/reviewlist.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4896 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/selection.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10061 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/table.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4806 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/table.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     5661 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/tableview.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.661073 plone.app.content-4.0.2/plone/app/content/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)    21104 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/templates/content_status_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2326 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/templates/delete_confirmation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      849 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/templates/object_rename.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4245 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/templates/select_default_page.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4372 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/templates/select_default_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    13662 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/browser/vocabulary.py
+-rw-r--r--   0 maurits    (501) staff       (20)      220 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      744 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      969 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3453 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/namechooser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4860 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/namechooser.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4665 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.665879 plone.app.content-4.0.2/plone/app/content/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/image.png
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.666233 plone.app.content-4.0.2/plone/app/content/tests/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.666540 plone.app.content-4.0.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.639802 plone.app.content-4.0.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.666971 plone.app.content-4.0.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/
+-rw-r--r--   0 maurits    (501) staff       (20)     1944 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/definition.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      160 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      449 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/profiles/non-ascii-workflow.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    17317 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      786 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_adding.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7025 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_content_status_modify.py
+-rw-r--r--   0 maurits    (501) staff       (20)    26699 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_contents.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18594 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_folder.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5289 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_folder_publish.py
+-rw-r--r--   0 maurits    (501) staff       (20)      457 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_namechooser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1796 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_namechooser_unit.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2122 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_non_ascii_characters_in_workflow_state.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2911 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_reviewlist.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4862 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_selectdefaultpage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      386 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_table.py
+-rw-r--r--   0 maurits    (501) staff       (20)    25303 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/tests/test_widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1049 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/plone/app/content/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:57:42.644673 plone.app.content-4.0.2/plone.app.content.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    38350 2023-06-16 16:57:42.000000 plone.app.content-4.0.2/plone.app.content.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     3683 2023-06-16 16:57:42.000000 plone.app.content-4.0.2/plone.app.content.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:57:42.000000 plone.app.content-4.0.2/plone.app.content.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-06-16 16:57:42.000000 plone.app.content-4.0.2/plone.app.content.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:57:42.000000 plone.app.content-4.0.2/plone.app.content.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      228 2023-06-16 16:57:42.000000 plone.app.content-4.0.2/plone.app.content.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-16 16:57:42.000000 plone.app.content-4.0.2/plone.app.content.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      172 2023-06-16 16:57:42.667761 plone.app.content-4.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1795 2023-06-16 16:57:41.000000 plone.app.content-4.0.2/setup.py
```

### Comparing `plone.app.content-4.0.1/CHANGES.rst` & `plone.app.content-4.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Fixup test_delete_wrong_object_by_acquisition_with_action. We don't publish acquired content items anymore.  [jaroel] (explicitacquisition)
+
+
 4.0.1 (2022-11-18)
 ------------------
 
 Bug fixes:
 
 
 - Redirect to ``/view`` after publishing File or Image when they have a workflow.  [maurits] (#3676)
```

### Comparing `plone.app.content-4.0.1/PKG-INFO` & `plone.app.content-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.content
-Version: 4.0.1
+Version: 4.0.2
 Summary: Content Views for Plone
 Home-page: https://pypi.org/project/plone.app.content
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone content views viewlet
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Fixup test_delete_wrong_object_by_acquisition_with_action. We don't publish acquired content items anymore.  [jaroel] (explicitacquisition)
+
+
 4.0.1 (2022-11-18)
 ------------------
 
 Bug fixes:
 
 
 - Redirect to ``/view`` after publishing File or Image when they have a workflow.  [maurits] (#3676)
```

### Comparing `plone.app.content-4.0.1/docs/LICENSE.GPL` & `plone.app.content-4.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/docs/LICENSE.txt` & `plone.app.content-4.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/actions.py` & `plone.app.content-4.0.2/plone/app/content/browser/actions.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/adding.py` & `plone.app.content-4.0.2/plone/app/content/browser/adding.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/configure.zcml` & `plone.app.content-4.0.2/plone/app/content/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/constraintypes.pt` & `plone.app.content-4.0.2/plone/app/content/browser/constraintypes.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/constraintypes.py` & `plone.app.content-4.0.2/plone/app/content/browser/constraintypes.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/content_status_history.py` & `plone.app.content-4.0.2/plone/app/content/browser/content_status_history.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/content_status_modify.py` & `plone.app.content-4.0.2/plone/app/content/browser/content_status_modify.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/__init__.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/configure.zcml` & `plone.app.content-4.0.2/plone/app/content/browser/contents/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/copy.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/copy.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/cut.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/cut.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/defaultpage.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/defaultpage.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/delete.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/delete.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/paste.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/paste.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/properties.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/properties.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/rearrange.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/rearrange.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/rename.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/rename.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/tags.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/tags.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/templates/folder_contents.pt` & `plone.app.content-4.0.2/plone/app/content/browser/contents/templates/folder_contents.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/templates/properties.pt` & `plone.app.content-4.0.2/plone/app/content/browser/contents/templates/properties.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/templates/rename.pt` & `plone.app.content-4.0.2/plone/app/content/browser/contents/templates/rename.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/templates/tags.pt` & `plone.app.content-4.0.2/plone/app/content/browser/contents/templates/tags.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/templates/workflow.pt` & `plone.app.content-4.0.2/plone/app/content/browser/contents/templates/workflow.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/contents/workflow.py` & `plone.app.content-4.0.2/plone/app/content/browser/contents/workflow.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/file.py` & `plone.app.content-4.0.2/plone/app/content/browser/file.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/folder_publish.py` & `plone.app.content-4.0.2/plone/app/content/browser/folder_publish.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/folderfactories.pt` & `plone.app.content-4.0.2/plone/app/content/browser/folderfactories.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/folderfactories.py` & `plone.app.content-4.0.2/plone/app/content/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/full_review_list.pt` & `plone.app.content-4.0.2/plone/app/content/browser/full_review_list.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/i18n.py` & `plone.app.content-4.0.2/plone/app/content/browser/i18n.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/query.py` & `plone.app.content-4.0.2/plone/app/content/browser/query.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/reviewlist.py` & `plone.app.content-4.0.2/plone/app/content/browser/reviewlist.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/selection.py` & `plone.app.content-4.0.2/plone/app/content/browser/selection.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/table.pt` & `plone.app.content-4.0.2/plone/app/content/browser/table.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/table.txt` & `plone.app.content-4.0.2/plone/app/content/browser/table.txt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/tableview.py` & `plone.app.content-4.0.2/plone/app/content/browser/tableview.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/templates/content_status_history.pt` & `plone.app.content-4.0.2/plone/app/content/browser/templates/content_status_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/templates/delete_confirmation.pt` & `plone.app.content-4.0.2/plone/app/content/browser/templates/delete_confirmation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/templates/object_rename.pt` & `plone.app.content-4.0.2/plone/app/content/browser/templates/object_rename.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/templates/select_default_page.pt` & `plone.app.content-4.0.2/plone/app/content/browser/templates/select_default_page.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/templates/select_default_view.pt` & `plone.app.content-4.0.2/plone/app/content/browser/templates/select_default_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/browser/vocabulary.py` & `plone.app.content-4.0.2/plone/app/content/browser/vocabulary.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/configure.zcml` & `plone.app.content-4.0.2/plone/app/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/interfaces.py` & `plone.app.content-4.0.2/plone/app/content/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/namechooser.py` & `plone.app.content-4.0.2/plone/app/content/namechooser.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/namechooser.txt` & `plone.app.content-4.0.2/plone/app/content/namechooser.txt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/testing.py` & `plone.app.content-4.0.2/plone/app/content/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/image.png` & `plone.app.content-4.0.2/plone/app/content/tests/image.png`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/definition.xml` & `plone.app.content-4.0.2/plone/app/content/tests/profiles/non-ascii-workflow-profile/workflows/non-ascii-workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_actions.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.app.testing import TEST_USER_NAME
 from plone.app.testing import TEST_USER_PASSWORD
 from plone.locking.interfaces import ILockable
 from plone.testing.zope import Browser
 from z3c.form.interfaces import IFormLayer
-from zExceptions import Unauthorized
+from zExceptions import Unauthorized, NotFound
 from zope.component import getMultiAdapter
 from zope.interface import alsoProvides
 
 import transaction
 import unittest
 
 
 class ActionsDXTestCase(unittest.TestCase):
-
     layer = PLONE_APP_CONTENT_DX_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
 
-        self.portal.acl_users.userFolderAddUser("editor", TEST_USER_PASSWORD, ["Editor"], [])
+        self.portal.acl_users.userFolderAddUser(
+            "editor", TEST_USER_PASSWORD, ["Editor"], []
+        )
 
         # For z3c.forms request must provide IFormLayer
         alsoProvides(self.request, IFormLayer)
 
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         self.portal.invokeFactory(type_name="Folder", id="f1", title="A Tést Folder")
 
@@ -138,16 +139,21 @@
         p1_id, page_2, browser_2 = self.prepare_for_acquisition_tests()
 
         # open two different browsers to the 'delete confirmation' view
         delete_url = page_2.absolute_url() + "/delete_confirmation"
         self.browser.open(delete_url)
         browser_2.open(delete_url)
         self.assertTrue(p1_id in self.portal)
-        for browser in [self.browser, browser_2]:
-            browser.getControl(name="form.buttons.Delete").click()
+
+        # Try to delete in both browsers
+        self.browser.getControl(name="form.buttons.Delete").click()
+        try:
+            browser_2.getControl(name="form.buttons.Delete").click()
+        except NotFound:
+            pass
 
         # the nested folder should be gone, but the one at the root should
         # remain.
         self.assertFalse(page_2.id in self.portal["f1"])
         self.assertTrue(p1_id in self.portal)
 
     def test_rename_form(self):
```

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_adding.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_adding.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_content_status_modify.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_content_status_modify.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_contents.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_folder.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_folder_publish.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_folder_publish.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_namechooser_unit.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_namechooser_unit.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_non_ascii_characters_in_workflow_state.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_non_ascii_characters_in_workflow_state.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_reviewlist.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_reviewlist.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_selectdefaultpage.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_selectdefaultpage.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/tests/test_widgets.py` & `plone.app.content-4.0.2/plone/app/content/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone/app/content/utils.py` & `plone.app.content-4.0.2/plone/app/content/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/plone.app.content.egg-info/PKG-INFO` & `plone.app.content-4.0.2/plone.app.content.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.content
-Version: 4.0.1
+Version: 4.0.2
 Summary: Content Views for Plone
 Home-page: https://pypi.org/project/plone.app.content
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone content views viewlet
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,14 +45,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.2 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Fixup test_delete_wrong_object_by_acquisition_with_action. We don't publish acquired content items anymore.  [jaroel] (explicitacquisition)
+
+
 4.0.1 (2022-11-18)
 ------------------
 
 Bug fixes:
 
 
 - Redirect to ``/view`` after publishing File or Image when they have a workflow.  [maurits] (#3676)
```

### Comparing `plone.app.content-4.0.1/plone.app.content.egg-info/SOURCES.txt` & `plone.app.content-4.0.2/plone.app.content.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.content-4.0.1/setup.py` & `plone.app.content-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.1"
+version = "4.0.2"
 
 setup(
     name="plone.app.content",
     version=version,
     description="Content Views for Plone",
     long_description="\n\n".join(
         [
```

