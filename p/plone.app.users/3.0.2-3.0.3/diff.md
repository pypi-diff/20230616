# Comparing `tmp/plone.app.users-3.0.2.tar.gz` & `tmp/plone.app.users-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.users-3.0.2.tar", last modified: Sat Apr 15 07:49:38 2023, max compression
+gzip compressed data, was "plone.app.users-3.0.3.tar", last modified: Fri Jun 16 16:41:29 2023, max compression
```

## Comparing `plone.app.users-3.0.2.tar` & `plone.app.users-3.0.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.166893 plone.app.users-3.0.2/
--rw-r--r--   0 gil       (1000) gil       (1000)    20577 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/CHANGES.rst
--rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/CONTRIBUTING.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      149 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/MANIFEST.in
--rw-r--r--   0 gil       (1000) gil       (1000)    24124 2023-04-15 07:49:38.166893 plone.app.users-3.0.2/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     2560 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/README.rst
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.159893 plone.app.users-3.0.2/docs/
--rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/docs/LICENSE.GPL
--rw-r--r--   0 gil       (1000) gil       (1000)      677 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.159893 plone.app.users-3.0.2/plone/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.160893 plone.app.users-3.0.2/plone/app/
--rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.161893 plone.app.users-3.0.2/plone/app/users/
--rw-r--r--   0 gil       (1000) gil       (1000)      637 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/TODO.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/__init__.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.163893 plone.app.users-3.0.2/plone/app/users/browser/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2053 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/account-configlet.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1367 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/account-panel.pt
--rw-r--r--   0 gil       (1000) gil       (1000)    13362 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/account.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3463 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     2534 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/interfaces.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1732 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/memberregistration.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     3587 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/membersearch.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4405 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/membersearch_form.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     1031 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/newuser_form.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     5006 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/passwordpanel.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3390 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/personalpreferences.py
--rw-r--r--   0 gil       (1000) gil       (1000)    29389 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/register.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1973 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/register_form.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     5235 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/registered.pt
--rw-r--r--   0 gil       (1000) gil       (1000)      573 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/registered.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2807 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/registersettingspanel.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1892 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/schema_layout.pt
--rw-r--r--   0 gil       (1000) gil       (1000)     9906 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/schemaeditor.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3820 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/browser/userdatapanel.py
--rw-r--r--   0 gil       (1000) gil       (1000)     3050 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/configure.zcml
--rw-r--r--   0 gil       (1000) gil       (1000)     2114 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/field_extender.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.158893 plone.app.users-3.0.2/plone/app/users/profiles/
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.163893 plone.app.users-3.0.2/plone/app/users/profiles/default/
--rw-r--r--   0 gil       (1000) gil       (1000)       85 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/profiles/default/metadata.xml
--rw-r--r--   0 gil       (1000) gil       (1000)     2085 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/profiles/default/userschema.xml
--rw-r--r--   0 gil       (1000) gil       (1000)     5682 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/schema.py
--rw-r--r--   0 gil       (1000) gil       (1000)      652 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/setuphandlers.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1415 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/testing.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.166893 plone.app.users-3.0.2/plone/app/users/tests/
--rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/__init__.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5022 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/base.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1997 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/duplicate_email.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     4463 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/email_login.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     7625 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/flexible_user_registration.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     2712 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/forms_navigationroot.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     3275 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/member_search.rst
--rw-r--r--   0 gil       (1000) gil       (1000)      306 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/onepixel.jpg
--rw-r--r--   0 gil       (1000) gil       (1000)     5282 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/password.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     4060 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/personal_preferences.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     3645 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/personal_preferences_prefs_user_details.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     4246 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/plugins.rst
--rw-r--r--   0 gil       (1000) gil       (1000)    15438 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/registration_forms.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     1618 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_account.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1136 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_doctests.py
--rw-r--r--   0 gil       (1000) gil       (1000)     8201 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_exportimport.py
--rw-r--r--   0 gil       (1000) gil       (1000)     2372 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_loginname_generator.py
--rw-r--r--   0 gil       (1000) gil       (1000)      530 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_member_search.py
--rw-r--r--   0 gil       (1000) gil       (1000)     8501 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_new_user.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1642 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_pam.py
--rw-r--r--   0 gil       (1000) gil       (1000)    12465 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_schema_types.py
--rw-r--r--   0 gil       (1000) gil       (1000)     1031 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_user_data_panel.py
--rw-r--r--   0 gil       (1000) gil       (1000)     5015 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/test_userid_generator.py
--rw-r--r--   0 gil       (1000) gil       (1000)     6049 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/userdata.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     2730 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/tests/userdata_prefs_user_details.rst
--rw-r--r--   0 gil       (1000) gil       (1000)     3672 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/upgrades.py
--rw-r--r--   0 gil       (1000) gil       (1000)      648 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/utils.py
--rw-r--r--   0 gil       (1000) gil       (1000)     4459 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/plone/app/users/vocabularies.py
-drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 07:49:38.160893 plone.app.users-3.0.2/plone.app.users.egg-info/
--rw-r--r--   0 gil       (1000) gil       (1000)    24124 2023-04-15 07:49:38.000000 plone.app.users-3.0.2/plone.app.users.egg-info/PKG-INFO
--rw-r--r--   0 gil       (1000) gil       (1000)     2739 2023-04-15 07:49:38.000000 plone.app.users-3.0.2/plone.app.users.egg-info/SOURCES.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:49:38.000000 plone.app.users-3.0.2/plone.app.users.egg-info/dependency_links.txt
--rw-r--r--   0 gil       (1000) gil       (1000)       40 2023-04-15 07:49:38.000000 plone.app.users-3.0.2/plone.app.users.egg-info/entry_points.txt
--rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 07:49:38.000000 plone.app.users-3.0.2/plone.app.users.egg-info/namespace_packages.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 07:49:38.000000 plone.app.users-3.0.2/plone.app.users.egg-info/not-zip-safe
--rw-r--r--   0 gil       (1000) gil       (1000)      624 2023-04-15 07:49:38.000000 plone.app.users-3.0.2/plone.app.users.egg-info/requires.txt
--rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 07:49:38.000000 plone.app.users-3.0.2/plone.app.users.egg-info/top_level.txt
--rw-r--r--   0 gil       (1000) gil       (1000)     1739 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/pyproject.toml
--rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 07:49:38.166893 plone.app.users-3.0.2/setup.cfg
--rw-r--r--   0 gil       (1000) gil       (1000)     2566 2023-04-15 07:49:37.000000 plone.app.users-3.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.971855 plone.app.users-3.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)    20887 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    24434 2023-06-16 16:41:29.971572 plone.app.users-3.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2560 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.951749 plone.app.users-3.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.952025 plone.app.users-3.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.955202 plone.app.users-3.0.3/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.958230 plone.app.users-3.0.3/plone/app/users/
+-rw-r--r--   0 maurits    (501) staff       (20)      637 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.963972 plone.app.users-3.0.3/plone/app/users/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2053 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/account-configlet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1367 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/account-panel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    13362 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/account.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3463 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1732 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/memberregistration.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3587 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/membersearch.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4405 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/membersearch_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/newuser_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5006 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/passwordpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3390 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/personalpreferences.py
+-rw-r--r--   0 maurits    (501) staff       (20)    29389 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/register.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1973 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/register_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5235 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/registered.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      573 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/registered.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2807 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/registersettingspanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1892 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/schema_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9906 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3820 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/browser/userdatapanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3050 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2282 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/field_extender.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.949117 plone.app.users-3.0.3/plone/app/users/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.964488 plone.app.users-3.0.3/plone/app/users/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2085 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/profiles/default/userschema.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5682 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/schema.py
+-rw-r--r--   0 maurits    (501) staff       (20)      652 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1415 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.971222 plone.app.users-3.0.3/plone/app/users/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5022 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1997 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/duplicate_email.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4463 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/email_login.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7625 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/flexible_user_registration.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2712 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/forms_navigationroot.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3275 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/member_search.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      306 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/onepixel.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     5282 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/password.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4060 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/personal_preferences.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3645 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/personal_preferences_prefs_user_details.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4246 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/plugins.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    15438 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/registration_forms.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1618 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_account.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1136 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8201 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2372 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_loginname_generator.py
+-rw-r--r--   0 maurits    (501) staff       (20)      530 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_member_search.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8501 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_new_user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1642 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_pam.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12465 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_schema_types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_user_data_panel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5015 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/test_userid_generator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6049 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/userdata.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2730 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/tests/userdata_prefs_user_details.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3672 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)      648 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4459 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone/app/users/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-16 16:41:29.954950 plone.app.users-3.0.3/plone.app.users.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    24434 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone.app.users.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2729 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone.app.users.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone.app.users.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone.app.users.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone.app.users.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone.app.users.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      624 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone.app.users.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/plone.app.users.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3858 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-06-16 16:41:29.971924 plone.app.users-3.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2566 2023-06-16 16:41:29.000000 plone.app.users-3.0.3/setup.py
```

### Comparing `plone.app.users-3.0.2/CHANGES.rst` & `plone.app.users-3.0.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Improve help text for member fields option where fields are shown.
+  For Managers the restriction to not show a field on the user profile does not apply.
+  [maurits] (#3794)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (53dc5b4c, e08b1234)
+
+
 3.0.2 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.users-3.0.2/PKG-INFO` & `plone.app.users-3.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.users
-Version: 3.0.2
+Version: 3.0.3
 Summary: A package for all things users and groups related (specific to plone)
 Home-page: https://pypi.org/project/plone.app.users
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Zope CMF Plone Users Groups
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,14 +93,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Improve help text for member fields option where fields are shown.
+  For Managers the restriction to not show a field on the user profile does not apply.
+  [maurits] (#3794)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (53dc5b4c, e08b1234)
+
+
 3.0.2 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plone.app.users Version: 3.0.2 Summary: A package
+Metadata-Version: 2.1 Name: plone.app.users Version: 3.0.3 Summary: A package
 for all things users and groups related (specific to plone) Home-page: https://
 pypi.org/project/plone.app.users Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: Zope CMF
 Plone Users Groups Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5 Classifier: License :: OSI Approved :: GNU
@@ -32,21 +32,24 @@
 ``portal_setup``. Note: the ``userschema.xml`` importation will automatically
 refresh the memberdata attributes, so the ``memberdata_properties.xml`` file is
 not needed. .. _plone.schemaeditor: https://github.com/plone/plone.schemaeditor
 .. _plone.supermodel: https://github.com/plone/plone.supermodel Changelog
 ========= .. You should *NOT* be adding new change log entries to this file.
 You should create a file in the news directory instead. For helpful
 instructions, please see: https://github.com/plone/plone.releaser/blob/master/
-ADD-A-NEWS-ITEM.rst .. towncrier release notes start 3.0.2 (2023-04-15) -------
------------ Internal: - Update configuration files. [plone devs] (434550cc)
-3.0.1 (2023-03-14) ------------------ Bug fixes: - Import more from plone.base.
-[maurits] (#1) 3.0.0 (2022-11-11) ------------------ Bug fixes: - For user
-schemas use a volatile cache on the request instead of on the portal. This
-prevents seeing an empty user profile when you have custom user schemas. This
-fixes `issue 76
+ADD-A-NEWS-ITEM.rst .. towncrier release notes start 3.0.3 (2023-06-16) -------
+----------- Bug fixes: - Improve help text for member fields option where
+fields are shown. For Managers the restriction to not show a field on the user
+profile does not apply. [maurits] (#3794) Internal: - Update configuration
+files. [plone devs] (53dc5b4c, e08b1234) 3.0.2 (2023-04-15) -----------------
+- Internal: - Update configuration files. [plone devs] (434550cc) 3.0.1 (2023-
+03-14) ------------------ Bug fixes: - Import more from plone.base. [maurits]
+(#1) 3.0.0 (2022-11-11) ------------------ Bug fixes: - For user schemas use a
+volatile cache on the request instead of on the portal. This prevents seeing an
+empty user profile when you have custom user schemas. This fixes `issue 76
 github.com/plone/plone.app.users/issues/76>`_. [maurits] (#76) 3.0.0b4 (2022-
 10-11) -------------------- Bug fixes: - Fix admin password in tests.
 [davisagli] (#113) 3.0.0b3 (2022-10-02) -------------------- Bug fixes: - Use
 longer passwords in tests. [davisagli] (#112) 3.0.0b2 (2022-09-01) ------------
 -------- Bug fixes: - Ensure that, when no timezone is selected, the value of
 the stored timezone is an empty string (#109) 3.0.0b1 (2022-07-19) ------------
 -------- Bug fixes: - Change default msgids for translations [erral] (#108)
```

### Comparing `plone.app.users-3.0.2/README.rst` & `plone.app.users-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/docs/LICENSE.GPL` & `plone.app.users-3.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/docs/LICENSE.txt` & `plone.app.users-3.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/TODO.txt` & `plone.app.users-3.0.3/plone/app/users/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/account-configlet.pt` & `plone.app.users-3.0.3/plone/app/users/browser/account-configlet.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/account-panel.pt` & `plone.app.users-3.0.3/plone/app/users/browser/account-panel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/account.py` & `plone.app.users-3.0.3/plone/app/users/browser/account.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/configure.zcml` & `plone.app.users-3.0.3/plone/app/users/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/interfaces.py` & `plone.app.users-3.0.3/plone/app/users/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/memberregistration.pt` & `plone.app.users-3.0.3/plone/app/users/browser/memberregistration.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/membersearch.py` & `plone.app.users-3.0.3/plone/app/users/browser/membersearch.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/membersearch_form.pt` & `plone.app.users-3.0.3/plone/app/users/browser/membersearch_form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/newuser_form.pt` & `plone.app.users-3.0.3/plone/app/users/browser/newuser_form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/passwordpanel.py` & `plone.app.users-3.0.3/plone/app/users/browser/passwordpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/personalpreferences.py` & `plone.app.users-3.0.3/plone/app/users/browser/personalpreferences.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/register.py` & `plone.app.users-3.0.3/plone/app/users/browser/register.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/register_form.pt` & `plone.app.users-3.0.3/plone/app/users/browser/register_form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/registered.pt` & `plone.app.users-3.0.3/plone/app/users/browser/registered.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/registered.py` & `plone.app.users-3.0.3/plone/app/users/browser/registered.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/registersettingspanel.py` & `plone.app.users-3.0.3/plone/app/users/browser/registersettingspanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/schema_layout.pt` & `plone.app.users-3.0.3/plone/app/users/browser/schema_layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/schemaeditor.py` & `plone.app.users-3.0.3/plone/app/users/browser/schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/browser/userdatapanel.py` & `plone.app.users-3.0.3/plone/app/users/browser/userdatapanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/configure.zcml` & `plone.app.users-3.0.3/plone/app/users/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/field_extender.py` & `plone.app.users-3.0.3/plone/app/users/field_extender.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from plone.app.users.browser.schemaeditor import USERS_NAMESPACE
 from plone.app.users.browser.schemaeditor import USERS_PREFIX
 from plone.autoform import directives as form
+from plone.base import PloneMessageFactory as _
 from plone.supermodel.interfaces import IFieldMetadataHandler
 from plone.supermodel.utils import ns
 from z3c.form.browser.checkbox import CheckBoxFieldWidget
 from zope.component import adapts
 from zope.interface import implementer
 from zope.interface import Interface
 from zope.schema.interfaces import IField
@@ -12,25 +13,28 @@
 from zope.schema.vocabulary import SimpleVocabulary
 
 import zope.schema
 
 
 form_vocab = SimpleVocabulary(
     [
-        SimpleTerm(value="On Registration", title="On Registration"),
-        SimpleTerm(value="In User Profile", title="In User Profile"),
+        SimpleTerm(value="On Registration", title=_("On Registration")),
+        SimpleTerm(value="In User Profile", title=_("In User Profile")),
     ]
 )
 
 
 class IUserFormSelection(Interface):
     form.widget(forms=CheckBoxFieldWidget)
     forms = zope.schema.List(
-        title="Where should this field be shown",
-        description="Does not apply to username or to email fields",
+        title=_("Where should this field be shown?"),
+        description=_(
+            "Does not apply to username or to email fields. "
+            "With the Manager role you always see all fields in the user profile."
+        ),
         required=True,
         value_type=zope.schema.Choice(vocabulary=form_vocab),
     )
 
 
 def get_user_form_selection(schema_context, field):
     return IUserFormSelection
```

### Comparing `plone.app.users-3.0.2/plone/app/users/profiles/default/userschema.xml` & `plone.app.users-3.0.3/plone/app/users/profiles/default/userschema.xml`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/schema.py` & `plone.app.users-3.0.3/plone/app/users/schema.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/setuphandlers.py` & `plone.app.users-3.0.3/plone/app/users/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/testing.py` & `plone.app.users-3.0.3/plone/app/users/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/base.py` & `plone.app.users-3.0.3/plone/app/users/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/duplicate_email.rst` & `plone.app.users-3.0.3/plone/app/users/tests/duplicate_email.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/email_login.rst` & `plone.app.users-3.0.3/plone/app/users/tests/email_login.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/flexible_user_registration.rst` & `plone.app.users-3.0.3/plone/app/users/tests/flexible_user_registration.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/forms_navigationroot.rst` & `plone.app.users-3.0.3/plone/app/users/tests/forms_navigationroot.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/member_search.rst` & `plone.app.users-3.0.3/plone/app/users/tests/member_search.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/password.rst` & `plone.app.users-3.0.3/plone/app/users/tests/password.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/personal_preferences.rst` & `plone.app.users-3.0.3/plone/app/users/tests/personal_preferences.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/personal_preferences_prefs_user_details.rst` & `plone.app.users-3.0.3/plone/app/users/tests/personal_preferences_prefs_user_details.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/plugins.rst` & `plone.app.users-3.0.3/plone/app/users/tests/plugins.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/registration_forms.rst` & `plone.app.users-3.0.3/plone/app/users/tests/registration_forms.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_account.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_doctests.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_exportimport.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_exportimport.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_loginname_generator.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_loginname_generator.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_member_search.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_member_search.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_new_user.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_new_user.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_pam.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_pam.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_schema_types.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_schema_types.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_user_data_panel.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_user_data_panel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/test_userid_generator.py` & `plone.app.users-3.0.3/plone/app/users/tests/test_userid_generator.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/userdata.rst` & `plone.app.users-3.0.3/plone/app/users/tests/userdata.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/tests/userdata_prefs_user_details.rst` & `plone.app.users-3.0.3/plone/app/users/tests/userdata_prefs_user_details.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/upgrades.py` & `plone.app.users-3.0.3/plone/app/users/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/utils.py` & `plone.app.users-3.0.3/plone/app/users/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone/app/users/vocabularies.py` & `plone.app.users-3.0.3/plone/app/users/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/plone.app.users.egg-info/PKG-INFO` & `plone.app.users-3.0.3/plone.app.users.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.users
-Version: 3.0.2
+Version: 3.0.3
 Summary: A package for all things users and groups related (specific to plone)
 Home-page: https://pypi.org/project/plone.app.users
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Zope CMF Plone Users Groups
 Classifier: Development Status :: 5 - Production/Stable
@@ -93,14 +93,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.3 (2023-06-16)
+------------------
+
+Bug fixes:
+
+
+- Improve help text for member fields option where fields are shown.
+  For Managers the restriction to not show a field on the user profile does not apply.
+  [maurits] (#3794)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (53dc5b4c, e08b1234)
+
+
 3.0.2 (2023-04-15)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plone.app.users Version: 3.0.2 Summary: A package
+Metadata-Version: 2.1 Name: plone.app.users Version: 3.0.3 Summary: A package
 for all things users and groups related (specific to plone) Home-page: https://
 pypi.org/project/plone.app.users Author: Plone Foundation Author-email: plone-
 developers@lists.sourceforge.net License: GPL version 2 Keywords: Zope CMF
 Plone Users Groups Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0 Classifier: Framework :: Plone :: Core
 Classifier: Framework :: Zope :: 5 Classifier: License :: OSI Approved :: GNU
@@ -32,21 +32,24 @@
 ``portal_setup``. Note: the ``userschema.xml`` importation will automatically
 refresh the memberdata attributes, so the ``memberdata_properties.xml`` file is
 not needed. .. _plone.schemaeditor: https://github.com/plone/plone.schemaeditor
 .. _plone.supermodel: https://github.com/plone/plone.supermodel Changelog
 ========= .. You should *NOT* be adding new change log entries to this file.
 You should create a file in the news directory instead. For helpful
 instructions, please see: https://github.com/plone/plone.releaser/blob/master/
-ADD-A-NEWS-ITEM.rst .. towncrier release notes start 3.0.2 (2023-04-15) -------
------------ Internal: - Update configuration files. [plone devs] (434550cc)
-3.0.1 (2023-03-14) ------------------ Bug fixes: - Import more from plone.base.
-[maurits] (#1) 3.0.0 (2022-11-11) ------------------ Bug fixes: - For user
-schemas use a volatile cache on the request instead of on the portal. This
-prevents seeing an empty user profile when you have custom user schemas. This
-fixes `issue 76
+ADD-A-NEWS-ITEM.rst .. towncrier release notes start 3.0.3 (2023-06-16) -------
+----------- Bug fixes: - Improve help text for member fields option where
+fields are shown. For Managers the restriction to not show a field on the user
+profile does not apply. [maurits] (#3794) Internal: - Update configuration
+files. [plone devs] (53dc5b4c, e08b1234) 3.0.2 (2023-04-15) -----------------
+- Internal: - Update configuration files. [plone devs] (434550cc) 3.0.1 (2023-
+03-14) ------------------ Bug fixes: - Import more from plone.base. [maurits]
+(#1) 3.0.0 (2022-11-11) ------------------ Bug fixes: - For user schemas use a
+volatile cache on the request instead of on the portal. This prevents seeing an
+empty user profile when you have custom user schemas. This fixes `issue 76
 github.com/plone/plone.app.users/issues/76>`_. [maurits] (#76) 3.0.0b4 (2022-
 10-11) -------------------- Bug fixes: - Fix admin password in tests.
 [davisagli] (#113) 3.0.0b3 (2022-10-02) -------------------- Bug fixes: - Use
 longer passwords in tests. [davisagli] (#112) 3.0.0b2 (2022-09-01) ------------
 -------- Bug fixes: - Ensure that, when no timezone is selected, the value of
 the stored timezone is an empty string (#109) 3.0.0b1 (2022-07-19) ------------
 -------- Bug fixes: - Change default msgids for translations [erral] (#108)
```

### Comparing `plone.app.users-3.0.2/plone.app.users.egg-info/SOURCES.txt` & `plone.app.users-3.0.3/plone.app.users.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.app.users.egg-info/PKG-INFO
 plone.app.users.egg-info/SOURCES.txt
 plone.app.users.egg-info/dependency_links.txt
```

### Comparing `plone.app.users-3.0.2/plone.app.users.egg-info/requires.txt` & `plone.app.users-3.0.3/plone.app.users.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.2/setup.py` & `plone.app.users-3.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.2"
+version = "3.0.3"
 
 long_description = "{}\n\n{}".format(
     open("README.rst").read(), open("CHANGES.rst").read()
 )
 
 extras_require = {
     "test": [
```

