# Comparing `tmp/prodigy-teams-recipes-sdk-0.1.2.tar.gz` & `tmp/prodigy-teams-recipes-sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodigy-teams-recipes-sdk-0.1.2.tar", last modified: Wed May 17 11:39:57 2023, max compression
+gzip compressed data, was "prodigy-teams-recipes-sdk-0.1.3.tar", last modified: Fri Jun 16 13:46:14 2023, max compression
```

## Comparing `prodigy-teams-recipes-sdk-0.1.2.tar` & `prodigy-teams-recipes-sdk-0.1.3.tar`

### file list

```diff
@@ -1,75 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:39:57.417834 prodigy-teams-recipes-sdk-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 11:39:57.417834 prodigy-teams-recipes-sdk-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19623 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:39:57.405833 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:39:57.409834 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/preview.html
--rw-r--r--   0 runner    (1001) docker     (123)   134493 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/preview.js
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/recipe_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/recipe_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/teams_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:39:57.409834 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:39:57.413833 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/for_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/full_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/org.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/person.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipeplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    52947 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/ty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:39:57.413833 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:39:57.417834 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/version/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/version/0.1.0_2023-05-12-12-39-11_patch_699f4418-3c53-4c0f-8a27-f838383451b1
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/version/0.1.1_2023-05-17-11-05-43_patch_8e2fe949-3833-4639-84bf-bf1f5bcbe993
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/version/read_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:39:57.405833 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 11:39:57.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-17 11:39:57.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:39:57.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-17 11:39:57.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:39:57.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-17 11:39:57.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 11:39:57.000000 prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:39:57.417834 prodigy-teams-recipes-sdk-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-17 11:39:47.000000 prodigy-teams-recipes-sdk-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.821915 prodigy-teams-recipes-sdk-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-16 13:46:14.821915 prodigy-teams-recipes-sdk-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19623 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.801914 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/about.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.809914 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/preview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.809914 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/public/200.html
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/public/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.809914 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/public/_nuxt/
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.4c35cb5b.css
+-rw-r--r--   0 runner    (1001) docker     (123)   200330 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.d4386e81.js
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/recipe_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/recipe_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/teams_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.813914 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.817914 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/for_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/full_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipeplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59374 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/ty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.821915 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.821915 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/version/0.1.0_2023-05-12-12-39-11_patch_699f4418-3c53-4c0f-8a27-f838383451b1
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/version/0.1.1_2023-05-17-11-05-43_patch_8e2fe949-3833-4639-84bf-bf1f5bcbe993
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/version/0.1.2_2023-06-16-09-48-01_patch_7cae2ccc-2549-44a9-bbcf-3f56fa93b58e
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/version/read_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:46:14.805914 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-16 13:46:14.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-16 13:46:14.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:46:14.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 13:46:14.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:46:14.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-16 13:46:14.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 13:46:14.000000 prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:46:14.821915 prodigy-teams-recipes-sdk-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-16 13:45:58.000000 prodigy-teams-recipes-sdk-0.1.3/setup.py
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/README.md` & `prodigy-teams-recipes-sdk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/__init__.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/about.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/about.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/cli.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/cli.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/preview.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/preview.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,38 +3,41 @@
 from pathlib import Path
 from typing import Any, Dict, Optional, TypedDict, cast
 
 import srsly
 import uvicorn
 from fastapi import FastAPI
 from fastapi.middleware.cors import CORSMiddleware
-from starlette.responses import HTMLResponse, Response
+from fastapi.staticfiles import StaticFiles
 
 from ..about import __version__
 from . import registry
 from .recipe import Recipe
 
 
 class PreviewData(TypedDict):
     name: str
     path: Optional[str]
 
 
-BUNDLE_FILE = "preview.js"
-INDEX_PATH = Path(__file__).parent / "preview.html"
-BUNDLE_PATH = Path(__file__).parent / BUNDLE_FILE
+HTML_PATH = Path(__file__).parent / "public"
 RECIPE_PATH = Path(__file__).parent / "recipe.json"
 
-with INDEX_PATH.open("r", encoding="utf8") as file_:
-    INDEX_HTML = file_.read()
-with BUNDLE_PATH.open("r", encoding="utf8") as file_:
-    JAVASCRIPT = file_.read()
+app = FastAPI(title="Prodigy Teams Recipe Preview", version=__version__)
 
 
-app = FastAPI(title="Prodigy Teams Recipe Preview", version=__version__)
+@app.get("/schema")
+def schema() -> Dict[str, Any]:
+    """Request the JSON form schema for the currently served recipe."""
+    data = get_recipe().to_json()
+    return data["form_schema"]
+
+
+# Serve static nuxt forms app
+app.mount("/", StaticFiles(html=True, directory=HTML_PATH), name="index")
 
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
@@ -86,24 +89,7 @@
 
 def get_recipe() -> Recipe:
     assert RECIPE_PATH.exists(), "no recipe set"
     data = cast(PreviewData, srsly.read_json(RECIPE_PATH))
     if data["path"] is not None:
         import_recipe(Path(data["path"]))
     return registry.need(data["name"])
-
-
-@app.get("/")
-def static_root() -> HTMLResponse:
-    return HTMLResponse(INDEX_HTML)
-
-
-@app.get(f"/{BUNDLE_FILE}")
-def static_bundle() -> Response:
-    return Response(JAVASCRIPT, media_type="application/javascript")
-
-
-@app.get("/schema")
-def schema() -> Dict[str, Any]:
-    """Request the JSON form schema for the currently served recipe."""
-    data = get_recipe().to_json()
-    return data["form_schema"]
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/recipe.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/recipe.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/recipe_schema.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/recipe_schema.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/registry.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """
 
     def __init__(self) -> None:
         self._loader = RecipeLoader()
         self._registry: Dict[str, Dict[str, Recipe]] = defaultdict(dict)
         self._default_load_path: LoadPath = [
             PackageSource.ENTRYPOINTS,
-            PackageSource.BUILTIN,
+            # PackageSource.BUILTIN,
             PackageSource.IMPLICIT,
         ]
 
     @cached_property
     def entrypoint_packages(self) -> List[str]:
         return self._loader.discover_packages_from_entrypoints()
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/teams_type.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/teams_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,11 +147,12 @@
         exclude=set(exclude),
     )
     if len(data.type.__mro__) >= 2:
         parent = data.type.__mro__[1]
         if type_registry.has(parent):
             data = data.merge(type_registry.get_by_type(parent))
     if type_registry.has(data.type_name):
+        existing_name = type_registry.get(data.type_name).type
         raise RecipeProcessingError(
-            f"There is an existing type with name '{data.type_name}'. Please choose another type name for the class '{cls.__name__}'."
+            f"There is an existing type with name '{data.type_name}' ({existing_name}). Please choose another type name for the class '{cls.__name__}'."
         )
     type_registry.set(data.type_name, data)
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/engine/util.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/engine/util.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/asset.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/asset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from ..models import (
     AssetCreating,
     AssetDeleting,
     AssetDetail,
     AssetListingLatest,
     AssetReading,
     AssetReadingLatest,
-    AssetReturning,
+    AssetSummary,
     AssetUpdating,
 )
 from .base import VersionedModelClient
 
 
 class Asset(
     VersionedModelClient[
         AssetCreating,
         AssetReading,
         AssetUpdating,
         AssetDeleting,
-        AssetReturning,
+        AssetSummary,
         AssetDetail,
         AssetReadingLatest,
         AssetListingLatest,
     ]
 ):
     Creating = AssetCreating
     Reading = AssetReading
     Updating = AssetUpdating
     Deleting = AssetDeleting
-    Returning = AssetReturning
+    Summary = AssetSummary
     Detail = AssetDetail
     ReadingLatest = AssetReadingLatest
     ListingLatest = AssetListingLatest
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/base.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -170,124 +170,122 @@
         return return_model.parse_obj(data)
 
 
 _Creating = ty.TypeVar("_Creating", bound=BaseModel)
 _Reading = ty.TypeVar("_Reading", bound=BaseModel)
 _Updating = ty.TypeVar("_Updating", bound=BaseModel)
 _Deleting = ty.TypeVar("_Deleting", bound=BaseModel)
-_Returning = ty.TypeVar("_Returning", bound=BaseModel)
+_Summary = ty.TypeVar("_Summary", bound=BaseModel)
 _Detail = ty.TypeVar("_Detail", bound=BaseModel)
 
 
 class ModelClient(
     BaseClient,
-    ty.Generic[_Creating, _Reading, _Updating, _Deleting, _Returning, _Detail],
+    ty.Generic[_Creating, _Reading, _Updating, _Deleting, _Summary, _Detail],
 ):
     Creating: ty.Type[_Creating]
     Reading: ty.Type[_Reading]
     Updating: ty.Type[_Updating]
     Deleting: ty.Type[_Deleting]
-    Returning: ty.Type[_Returning]
+    Summary: ty.Type[_Summary]
     Detail: ty.Type[_Detail]
 
     def __init__(
         self, sync_client: httpx.Client, async_client: httpx.AsyncClient, path: str
     ) -> None:
         super().__init__(sync_client, async_client, path)
         self.plural_path = f"{self.path}s"
 
     # TODO: Eventually the `create`, `read`, `update` routes should all
-    # have _Detail models and they won't return Union[_Returning, _Detail] but
+    # have _Detail models and they won't return Union[_Summary], _Detail] but
     # explicitly return `_Detail`. This is temporary until the PAM API is finalized
     def create(
         self, data: ty.Optional[_Creating] = None, **kwargs: ty.Any
-    ) -> ty.Union[_Returning, _Detail]:
+    ) -> ty.Union[_Summary, _Detail]:
         data = data if data else self.Creating(**kwargs)
         has_detail, return_model = self._has_detail()
         # Using a type ignore here because the 'detail' stuff is messy and needs to be
         # refactored anyway
         res = self.request(
             "POST", endpoint="create", data=data, return_model=return_model  # type: ignore
         )
-        return ty.cast(_Detail, res) if has_detail else ty.cast(_Returning, res)
+        return ty.cast(_Detail, res) if has_detail else ty.cast(_Summary, res)
 
     async def create_async(
         self, data: ty.Optional[_Creating] = None, **kwargs: ty.Any
-    ) -> ty.Union[_Returning, _Detail]:
+    ) -> ty.Union[_Summary, _Detail]:
         data = data if data else self.Creating(**kwargs)
         has_detail, return_model = self._has_detail()
         res = await self.request_async(
             "POST", endpoint="create", data=data, return_model=return_model  # type: ignore
         )
-        return ty.cast(_Detail, res) if has_detail else ty.cast(_Returning, res)
+        return ty.cast(_Detail, res) if has_detail else ty.cast(_Summary, res)
 
     def read(
         self, query: ty.Optional[_Reading] = None, **kwargs: ty.Any
-    ) -> ty.Union[_Returning, _Detail]:
+    ) -> ty.Union[_Summary, _Detail]:
         params = query if query else self.Reading(**kwargs)
         has_detail, return_model = self._has_detail()
         res = self.request("GET", params=params, return_model=return_model)  # type: ignore
-        return ty.cast(_Detail, res) if has_detail else ty.cast(_Returning, res)
+        return ty.cast(_Detail, res) if has_detail else ty.cast(_Summary, res)
 
     async def read_async(
         self, query: ty.Optional[_Reading] = None, **kwargs: ty.Any
-    ) -> ty.Union[_Returning, _Detail]:
+    ) -> ty.Union[_Summary, _Detail]:
         params = query if query else self.Reading(**kwargs)
         has_detail, return_model = self._has_detail()
         res = await self.request_async("GET", params=params, return_model=return_model)  # type: ignore
-        return ty.cast(_Detail, res) if has_detail else ty.cast(_Returning, res)
+        return ty.cast(_Detail, res) if has_detail else ty.cast(_Summary, res)
 
     def exists(
         self, query: ty.Optional[_Reading] = None, **kwargs: ty.Any
-    ) -> ty.Optional[ty.Union[_Returning, _Detail]]:
+    ) -> ty.Optional[ty.Union[_Summary, _Detail]]:
         params = query if query else self.Reading(**kwargs)
         has_detail, return_model = self._has_detail()
         try:
             res = self.request("GET", params=params, return_model=return_model)  # type: ignore
         except errors.NotFound:
             res = None
         return (
             ty.cast(ty.Optional[_Detail], res)
             if has_detail
-            else ty.cast(ty.Optional[_Returning], res)
+            else ty.cast(ty.Optional[_Summary], res)
         )
 
     async def exists_async(
         self, query: ty.Optional[_Reading] = None, **kwargs: ty.Any
-    ) -> ty.Optional[ty.Union[_Returning, _Detail]]:
+    ) -> ty.Optional[ty.Union[_Summary, _Detail]]:
         params = query if query else self.Reading(**kwargs)
         has_detail, return_model = self._has_detail()
         try:
             res = await self.request_async(
                 "GET", params=params, return_model=return_model  # type: ignore
             )
         except errors.NotFound:
             res = None
         return (
             ty.cast(ty.Optional[_Detail], res)
             if has_detail
-            else ty.cast(ty.Optional[_Returning], res)
+            else ty.cast(ty.Optional[_Summary], res)
         )
 
-    def update(
-        self, data: ty.Optional[_Updating] = None, **kwargs: ty.Any
-    ) -> _Returning:
+    def update(self, data: ty.Optional[_Updating] = None, **kwargs: ty.Any) -> _Summary:
         data = data if data else self.Updating(**kwargs)
         has_detail, return_model = self._has_detail()
         res = self.request(
             "POST",
             endpoint="update",
             data=data,
             return_model=return_model,  # type: ignore
         )
         return res  # type: ignore
 
     async def update_async(
         self, data: ty.Optional[_Updating] = None, **kwargs: ty.Any
-    ) -> _Returning:
+    ) -> _Summary:
         data = data if data else self.Updating(**kwargs)
         has_detail, return_model = self._has_detail()
         res = await self.request_async(
             "POST",
             endpoint="update",
             data=data,
             return_model=return_model,  # type: ignore
@@ -305,72 +303,72 @@
     def all(
         self,
         query: ty.Optional[_Reading] = None,
         *,
         page: ty.Optional[int] = None,
         size: ty.Optional[int] = None,
         **kwargs: ty.Any,
-    ) -> ty.Page[_Returning]:
+    ) -> ty.Page[_Summary]:
         params = query if query else self.Reading(**kwargs)
         res = self.request(
             "GET",
             endpoint=self.plural_path,
             params=params,
             page=page,
             size=size,
-            return_model=ty.Page[self.Returning],  # type: ignore
+            return_model=ty.Page[self.Summary],  # type: ignore
         )
-        return ty.cast(ty.Page[_Returning], res)
+        return ty.cast(ty.Page[_Summary], res)
 
     async def all_async(
         self,
         query: ty.Optional[_Reading] = None,
         *,
         page: ty.Optional[int] = None,
         size: ty.Optional[int] = None,
         **kwargs: ty.Any,
-    ) -> ty.Page[_Returning]:
+    ) -> ty.Page[_Summary]:
         params = query if query else self.Reading(**kwargs)
         res = await self.request_async(
             "GET",
             endpoint=self.plural_path,
             params=params,
             page=page,
             size=size,
-            return_model=ty.Page[self.Returning],  # type: ignore
+            return_model=ty.Page[self.Summary],  # type: ignore
         )
-        return ty.cast(ty.Page[_Returning], res)
+        return ty.cast(ty.Page[_Summary], res)
 
     def all_readable(
         self,
         query: ty.Optional[_Reading] = None,
         **kwargs: ty.Any,
-    ) -> ty.Page[_Returning]:
+    ) -> ty.Page[_Summary]:
         params = query if query else self.Reading(**kwargs)
         res = self.request(
             "GET",
             endpoint=self.plural_path,
             params=params,
-            return_model=ty.Page[self.Returning],  # type: ignore
+            return_model=ty.Page[self.Summary],  # type: ignore
         )
-        return ty.cast(ty.Page[_Returning], res)
+        return ty.cast(ty.Page[_Summary], res)
 
     async def all_readable_async(
         self,
         query: ty.Optional[_Reading] = None,
         **kwargs: ty.Any,
-    ) -> ty.Page[_Returning]:
+    ) -> ty.Page[_Summary]:
         params = query if query else self.Reading(**kwargs)
         res = await self.request_async(
             "GET",
             endpoint=self.plural_path,
             params=params,
-            return_model=ty.Page[self.Returning],  # type: ignore
+            return_model=ty.Page[self.Summary],  # type: ignore
         )
-        return ty.cast(ty.Page[_Returning], res)
+        return ty.cast(ty.Page[_Summary], res)
 
     def _raise_and_handle_errors(self, response: httpx.Response) -> None:
         """Translate errors by status. This allows SDK consumers to get the original
         error from Prodigy Teams, not just the status.
         Does nothing if the reponse was successful
         """
         prefix = self.__class__.__name__
@@ -396,75 +394,82 @@
             elif status == 403:
                 raise getattr(errors, f"{prefix}Forbidden", errors.Forbidden)
             elif status == 404:
                 raise getattr(errors, f"{prefix}NotFound", errors.NotFound)
             else:
                 raise e
 
-    def _has_detail(self) -> ty.Tuple[bool, ty.Union[_Returning, _Detail]]:
+    def _has_detail(self) -> ty.Tuple[bool, ty.Union[_Summary, _Detail]]:
         if hasattr(self, "Detail"):
             return True, ty.cast(_Detail, self.Detail)
         else:
-            return False, ty.cast(_Detail, self.Returning)
+            return False, ty.cast(_Detail, self.Summary)
 
 
 _ReadingLatest = ty.TypeVar("_ReadingLatest", bound=BaseModel)
 _ListingLatest = ty.TypeVar("_ListingLatest", bound=BaseModel)
 
 
 class VersionedModelClient(
-    ModelClient,
     ty.Generic[
         _Creating,
         _Reading,
         _Updating,
         _Deleting,
-        _Returning,
+        _Summary,
         _Detail,
         _ReadingLatest,
         _ListingLatest,
     ],
+    ModelClient[
+        _Creating,
+        _Reading,
+        _Updating,
+        _Deleting,
+        _Summary,
+        _Detail,
+    ],
 ):
     Creating: ty.Type[_Creating]
     Reading: ty.Type[_Reading]
     Updating: ty.Type[_Updating]
     Deleting: ty.Type[_Deleting]
-    Returning: ty.Type[_Returning]
+    Summary: ty.Type[_Summary]
     Detail: ty.Type[_Detail]
     ReadingLatest: ty.Type[_ReadingLatest]
     ListingLatest: ty.Type[_ListingLatest]
 
-    def all_latest(self, *, body: _ListingLatest) -> ty.Page[_Returning]:
+    def all_latest(self, *, body: _ListingLatest) -> ty.Page[_Summary]:
         res = self.request(
             "POST",
             endpoint="all-latest",
             data=body,
-            return_model=ty.Page[self.Returning],  # type: ignore
+            return_model=ty.Page[self.Summary],  # type: ignore
         )
-        return ty.cast(ty.Page[_Returning], res)
+        return ty.cast(ty.Page[_Summary], res)
 
-    async def all_latest_async(self, *, body: _ListingLatest) -> ty.Page[_Returning]:
+    async def all_latest_async(self, *, body: _ListingLatest) -> ty.Page[_Summary]:
         res = await self.request_async(
             "POST",
             endpoint="all-latest",
             data=body,
-            return_model=ty.Page[self.Returning],  # type: ignore
+            return_model=ty.Page[self.Summary],  # type: ignore
         )
-        return ty.cast(ty.Page[_Returning], res)  # type: ignore
+        return ty.cast(ty.Page[_Summary], res)  # type: ignore
 
-    def latest(self, *, body: _ReadingLatest) -> _Returning:
+    def latest(self, *, body: _ReadingLatest) -> _Summary:
         res = self.request(
             "POST",
             endpoint="latest",
             data=body,
             return_model=self.Detail,
         )
-        return ty.cast(_Returning, res)
+        return ty.cast(_Summary, res)
 
-    async def latest_async(self, *, body: _ReadingLatest) -> _Returning:
+    async def latest_async(self, *, body: _ReadingLatest) -> _Summary:
         res = await self.request_async(
             "POST",
             endpoint="latest",
             data=body,
             return_model=self.Detail,
         )
-        return ty.cast(_Returning, res)
+        return ty.cast(_Summary, res)
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,81 @@
 from .. import ty
 from ..models import (
     BrokerDeleting,
+    BrokerDetail,
     BrokerReading,
     BrokerRegistering,
     BrokerRegistrationCreating,
-    BrokerRegistrationReturning,
-    BrokerReturning,
+    BrokerRegistrationSummary,
+    BrokerSummary,
     BrokerUpdating,
 )
 from .base import ModelClient
 
 
 class Broker(
     ModelClient[
         BrokerRegistering,
         BrokerReading,
         BrokerUpdating,
         BrokerDeleting,
-        BrokerReturning,
-        BrokerReturning,
+        BrokerSummary,
+        BrokerDetail,
     ]
 ):
     Creating = BrokerRegistering
     Reading = BrokerReading
     Updating = BrokerUpdating
     Deleting = BrokerDeleting
-    Returning = BrokerReturning
+    Summary = BrokerSummary
+    Detail = BrokerDetail
 
     class Token(ty.BaseModel):
         token: str
 
     def create(
         self, data: ty.Optional[BrokerRegistrationCreating] = None, **kwargs: ty.Any
-    ) -> BrokerRegistrationReturning:
+    ) -> BrokerRegistrationSummary:
         data = data if data else BrokerRegistrationCreating(**kwargs)
         res = self.request(
             "POST",
             endpoint="create",
             data=data,
-            return_model=BrokerRegistrationReturning,
+            return_model=BrokerRegistrationSummary,
         )
-        return ty.cast(BrokerRegistrationReturning, res)
+        return ty.cast(BrokerRegistrationSummary, res)
 
     async def create_async(
         self, data: ty.Optional[BrokerRegistrationCreating] = None, **kwargs: ty.Any
-    ) -> BrokerRegistrationReturning:
+    ) -> BrokerRegistrationSummary:
         data = data if data else BrokerRegistrationCreating(**kwargs)
         res = await self.request_async(
             "POST",
             endpoint="create",
             data=data,
-            return_model=BrokerRegistrationReturning,
+            return_model=BrokerRegistrationSummary,
         )
-        return ty.cast(BrokerRegistrationReturning, res)
+        return ty.cast(BrokerRegistrationSummary, res)
 
     def register(
         self, data: ty.Optional[BrokerRegistering] = None, **kwargs: ty.Any
-    ) -> BrokerReturning:
+    ) -> BrokerDetail:
         data = data if data else BrokerRegistering(**kwargs)
         res = self.request(
             "POST",
             endpoint="register",
             data=data,
-            return_model=BrokerReturning,
+            return_model=BrokerDetail,
         )
-        return ty.cast(BrokerReturning, res)
+        return ty.cast(BrokerDetail, res)
 
     async def register_async(
         self, data: ty.Optional[BrokerRegistering] = None, **kwargs: ty.Any
-    ) -> BrokerReturning:
+    ) -> BrokerDetail:
         data = data if data else BrokerRegistering(**kwargs)
         res = await self.request_async(
             "POST",
             endpoint="register",
             data=data,
-            return_model=BrokerReturning,
+            return_model=BrokerDetail,
         )
-        return ty.cast(BrokerReturning, res)
+        return ty.cast(BrokerDetail, res)
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker_path.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/broker_path.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from ..models import (
     BrokerPathCreating,
     BrokerPathDeleting,
+    BrokerPathDetail,
     BrokerPathReading,
-    BrokerPathReturning,
+    BrokerPathSummary,
     BrokerPathUpdating,
 )
 from .base import ModelClient
 
 
 class BrokerPath(
     ModelClient[
         BrokerPathCreating,
         BrokerPathReading,
         BrokerPathUpdating,
         BrokerPathDeleting,
-        BrokerPathReturning,
-        BrokerPathReturning,
+        BrokerPathSummary,
+        BrokerPathDetail,
     ]
 ):
     Creating = BrokerPathCreating
     Reading = BrokerPathReading
     Updating = BrokerPathUpdating
     Deleting = BrokerPathDeleting
-    Returning = BrokerPathReturning
+    Summary = BrokerPathSummary
+    Detail = BrokerPathDetail
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/dataset.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ..models import (
     DatasetCreating,
     DatasetDeleting,
     DatasetDetail,
     DatasetReading,
-    DatasetReturning,
+    DatasetSummary,
     DatasetUpdating,
 )
 from .base import ModelClient
 
 
 class Dataset(
     ModelClient[
         DatasetCreating,
         DatasetReading,
         DatasetUpdating,
         DatasetDeleting,
-        DatasetReturning,
+        DatasetSummary,
         DatasetDetail,
     ]
 ):
     Creating = DatasetCreating
     Reading = DatasetReading
     Updating = DatasetUpdating
     Deleting = DatasetDeleting
-    Returning = DatasetReturning
+    Summary = DatasetSummary
     Detail = DatasetDetail
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/for_cluster.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/for_cluster.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 from .. import ty
 from ..models import (
-    ActionReturning,
+    ActionDetail,
     ClusterJobReading,
     EmptyResponse,
     NomadAttemptUpdating,
     NomadEventBatchCreating,
     NomadEventGetIndex,
     NomadEventIndex,
     NomadJobs,
     ReportNomadJobResponse,
-    TaskReturning,
+    TaskDetail,
 )
 from .base import BaseClient
 
 
 class ForCluster(BaseClient):
     class Token(ty.BaseModel):
         token: str
 
-    def read_task(self, data: ClusterJobReading, **kwargs: ty.Any) -> TaskReturning:
+    def read_task(self, data: ClusterJobReading, **kwargs: ty.Any) -> TaskDetail:
         res = self.request(
             "POST",
             endpoint="read-task",
             data=data,
-            return_model=TaskReturning,
+            return_model=TaskDetail,
         )
-        return ty.cast(TaskReturning, res)
+        return ty.cast(TaskDetail, res)
 
     async def read_task_async(
         self, data: ClusterJobReading, **kwargs: ty.Any
-    ) -> TaskReturning:
+    ) -> TaskDetail:
         res = await self.request_async(
             "POST",
             endpoint="read-task",
             data=data,
-            return_model=TaskReturning,
+            return_model=TaskDetail,
         )
-        return ty.cast(TaskReturning, res)
+        return ty.cast(TaskDetail, res)
 
-    def read_action(self, data: ClusterJobReading, **kwargs: ty.Any) -> ActionReturning:
+    def read_action(self, data: ClusterJobReading, **kwargs: ty.Any) -> ActionDetail:
         res = self.request(
             "POST",
             endpoint="read-action",
             data=data,
-            return_model=ActionReturning,
+            return_model=ActionDetail,
         )
-        return ty.cast(ActionReturning, res)
+        return ty.cast(ActionDetail, res)
 
     async def read_action_async(
         self, data: ClusterJobReading, **kwargs: ty.Any
-    ) -> ActionReturning:
+    ) -> ActionDetail:
         res = await self.request_async(
             "POST",
             endpoint="read-action",
             data=data,
-            return_model=TaskReturning,
+            return_model=ActionDetail,
         )
-        return ty.cast(ActionReturning, res)
+        return ty.cast(ActionDetail, res)
 
     def report_nomad_event(
         self, data: NomadEventBatchCreating, **kwargs: ty.Any
     ) -> None:
         self.request(
             "POST",
             endpoint="report-nomad-event",
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/full_client.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/full_client.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/group.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/group.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from ..models import (
     GroupAuthorizing,
     GroupCreating,
     GroupDeleting,
+    GroupDetail,
     GroupPopulating,
     GroupReading,
-    GroupReturning,
+    GroupSummary,
     GroupUpdating,
 )
 from .base import ModelClient
 
 
 class Group(
     ModelClient[
         GroupCreating,
         GroupReading,
         GroupUpdating,
         GroupDeleting,
-        GroupReturning,
-        GroupReturning,
+        GroupSummary,
+        GroupDetail,
     ]
 ):
     Creating = GroupCreating
     Reading = GroupReading
     Updating = GroupUpdating
     Deleting = GroupDeleting
-    Returning = GroupReturning
+    Summary = GroupSummary
+    Detail = GroupDetail
     Populating = GroupPopulating
     Authorizing = GroupAuthorizing
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/invitation.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/invitation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from ..models import (
     InvitationCreating,
     InvitationDeleting,
+    InvitationDetail,
     InvitationReading,
-    InvitationReturning,
+    InvitationSummary,
     InvitationUpdating,
 )
 from .base import ModelClient
 
 
 class Invitation(
     ModelClient[
         InvitationCreating,
         InvitationReading,
         InvitationUpdating,
         InvitationDeleting,
-        InvitationReturning,
-        InvitationReturning,
+        InvitationSummary,
+        InvitationDetail,
     ]
 ):
     Creating = InvitationCreating
     Reading = InvitationReading
     Updating = InvitationUpdating
     Deleting = InvitationDeleting
-    Returning = InvitationReturning
+    Summary = InvitationSummary
+    Detail = InvitationDetail
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/notification.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/notification.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from ..models import (
     NotificationCreating,
     NotificationDeleting,
+    NotificationDetail,
     NotificationReading,
-    NotificationReturning,
+    NotificationSummary,
     NotificationUpdating,
 )
 from .base import ModelClient
 
 
 class Notification(
     ModelClient[
         NotificationCreating,
         NotificationReading,
         NotificationUpdating,
         NotificationDeleting,
-        NotificationReturning,
-        NotificationReturning,
+        NotificationSummary,
+        NotificationDetail,
     ]
 ):
     Creating = NotificationCreating
     Reading = NotificationReading
     Updating = NotificationUpdating
     Deleting = NotificationDeleting
-    Returning = NotificationReturning
+    Summary = NotificationSummary
+    Detail = NotificationDetail
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/package.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/package.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from ..models import (
     PackageCreating,
     PackageDeleting,
+    PackageDetail,
     PackageListingLatest,
     PackageReading,
     PackageReadingLatest,
-    PackageReturning,
+    PackageSummary,
     PackageUpdating,
 )
 from .base import VersionedModelClient
 
 
 class Package(
     VersionedModelClient[
         PackageCreating,
         PackageReading,
         PackageUpdating,
         PackageDeleting,
-        PackageReturning,
-        PackageReturning,
+        PackageSummary,
+        PackageDetail,
         PackageReadingLatest,
         PackageListingLatest,
     ]
 ):
     Creating = PackageCreating
     Reading = PackageReading
     Updating = PackageUpdating
     Deleting = PackageDeleting
-    Returning = PackageReturning
-    Detail = PackageReturning
+    Summary = PackageSummary
+    Detail = PackageDetail
     ReadingLatest = PackageReadingLatest
     ListingLatest = PackageListingLatest
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/person.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/person.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from .. import ty
 from ..models import (
     PersonCreating,
     PersonDeleting,
+    PersonDetail,
     PersonReading,
-    PersonReturning,
+    PersonSummary,
     PersonUpdating,
 )
 from .base import ModelClient
 
 
 class Person(
     ModelClient[
         PersonCreating,
         PersonReading,
         PersonUpdating,
         PersonDeleting,
-        PersonReturning,
-        PersonReturning,
+        PersonSummary,
+        PersonDetail,
     ]
 ):
     Creating = PersonCreating
     Reading = PersonReading
     Updating = PersonUpdating
     Deleting = PersonDeleting
-    Returning = PersonReturning
+    Summary = PersonSummary
+    Detail = PersonDetail
 
     class Authenticating(ty.BaseModel):
         """
         Data describing a Person derived from an identity token provided
         by an authentication provider such as Auth0. Used during signup and login.
         """
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipe.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from ..models import (
     RecipeCreating,
     RecipeDeleting,
     RecipeDetail,
     RecipeListingLatest,
     RecipeReading,
     RecipeReadingLatest,
-    RecipeReturning,
+    RecipeSummary,
     RecipeUpdating,
 )
 from .base import VersionedModelClient
 
 
 class Recipe(
     VersionedModelClient[
         RecipeCreating,
         RecipeReading,
         RecipeUpdating,
         RecipeDeleting,
-        RecipeReturning,
+        RecipeSummary,
         RecipeDetail,
         RecipeReadingLatest,
         RecipeListingLatest,
     ]
 ):
     Creating = RecipeCreating
     Reading = RecipeReading
     Updating = RecipeUpdating
     Deleting = RecipeDeleting
-    Returning = RecipeReturning
+    Summary = RecipeSummary
     Detail = RecipeDetail
     ReadingLatest = RecipeReadingLatest
     ListingLatest = RecipeListingLatest
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipeplan.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/recipeplan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from ..models import (
     ObjectValidation,
     RecipePlanCreating,
     RecipePlanDeleting,
+    RecipePlanDetail,
     RecipePlanReading,
-    RecipePlanReturning,
+    RecipePlanSummary,
     RecipePlanUpdating,
 )
 from .base import ModelClient
 
 
 class RecipePlan(
     ModelClient[
         RecipePlanCreating,
         RecipePlanReading,
         RecipePlanUpdating,
         RecipePlanDeleting,
-        RecipePlanReturning,
-        RecipePlanReturning,
+        RecipePlanSummary,
+        RecipePlanDetail,
     ]
 ):
     Creating = RecipePlanCreating
     Reading = RecipePlanReading
     Updating = RecipePlanUpdating
     Deleting = RecipePlanDeleting
-    Returning = RecipePlanReturning
+    Summary = RecipePlanSummary
+    Detail = RecipePlanDetail
 
     def validate_objects(self, data: RecipePlanCreating) -> ObjectValidation:
         res = self.request(
             "POST",
             endpoint="validate-objects",
             data=data,
             return_model=ObjectValidation,
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/secret.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/secret.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from ..models import (
     SecretCreating,
     SecretDeleting,
     SecretDetail,
     SecretReading,
-    SecretReturning,
+    SecretSummary,
     SecretUpdating,
 )
 from .base import ModelClient
 
 
 class Secret(
     ModelClient[
         SecretCreating,
         SecretReading,
         SecretUpdating,
         SecretDeleting,
-        SecretReturning,
+        SecretSummary,
         SecretDetail,
     ]
 ):
     Creating = SecretCreating
     Reading = SecretReading
     Updating = SecretUpdating
     Deleting = SecretDeleting
-    Returning = SecretReturning
+    Summary = SecretSummary
     Detail = SecretDetail
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/errors.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/models.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -103,18 +103,18 @@
 
 
 class AssetReadingLatest(BaseModel):
     name: str = Field(..., title="Name")
     broker_id: UUID = Field(..., title="Broker Id")
 
 
-class AssetReturning(BaseModel):
+class AssetSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     broker_id: UUID = Field(..., title="Broker Id")
     name: str = Field(..., title="Name")
     version: str = Field(..., title="Version")
     kind: str = Field(..., title="Kind")
     path: str = Field(..., title="Path")
     meta: Dict[str, Any] = Field(..., title="Meta")
     num_used_by: int = Field(..., title="Num Used By")
@@ -151,35 +151,59 @@
     token_type: Optional[str] = Field("bearer", title="Token Type")
 
 
 class BrokerDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
+class BrokerDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    org_id: UUID = Field(..., title="Org Id")
+    name: str = Field(..., title="Name")
+    address: str = Field(..., title="Address")
+    state: str = Field(..., title="State")
+    cloud_provider: str = Field(..., title="Cloud Provider")
+    cloud_account: Optional[str] = Field(None, title="Cloud Account")
+    cloud_region: Optional[str] = Field(None, title="Cloud Region")
+    client_id: UUID = Field(..., title="Client Id")
+    client_secret: str = Field(..., title="Client Secret")
+
+
 class BrokerPathCreating(BaseModel):
     broker_id: UUID = Field(..., title="Broker Id")
     name: str = Field(..., title="Name")
     path: str = Field(..., title="Path")
 
 
 class BrokerPathDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
+class BrokerPathDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    broker_id: UUID = Field(..., title="Broker Id")
+    name: str = Field(..., title="Name")
+    path: str = Field(..., title="Path")
+
+
 class BrokerPathReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     broker_id: Optional[UUID] = Field(None, title="Broker Id")
     name: Optional[str] = Field(None, title="Name")
     path: Optional[str] = Field(None, title="Path")
 
 
-class BrokerPathReturning(BaseModel):
+class BrokerPathSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     broker_id: UUID = Field(..., title="Broker Id")
     name: str = Field(..., title="Name")
     path: str = Field(..., title="Path")
 
 
 class BrokerPathUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
@@ -207,28 +231,29 @@
 class BrokerRegistrationCreating(BaseModel):
     name: str = Field(..., title="Name")
     cloud_provider: str = Field(..., title="Cloud Provider")
     cloud_account: Optional[str] = Field(None, title="Cloud Account")
     cloud_region: Optional[str] = Field(None, title="Cloud Region")
 
 
-class BrokerRegistrationReturning(BaseModel):
+class BrokerRegistrationSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
     org_id: UUID = Field(..., title="Org Id")
     name: str = Field(..., title="Name")
     registration_token: UUID = Field(..., title="Registration Token")
     claimed: bool = Field(..., title="Claimed")
     expiration: datetime = Field(..., title="Expiration")
 
 
-class BrokerReturning(BaseModel):
+class BrokerSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     org_id: UUID = Field(..., title="Org Id")
     name: str = Field(..., title="Name")
     address: str = Field(..., title="Address")
     state: str = Field(..., title="State")
     cloud_provider: str = Field(..., title="Cloud Provider")
     cloud_account: Optional[str] = Field(None, title="Cloud Account")
     cloud_region: Optional[str] = Field(None, title="Cloud Region")
@@ -269,18 +294,18 @@
 class DatasetReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     name: Optional[str] = Field(None, title="Name")
     kind: Optional[str] = Field(None, title="Kind")
     broker_id: Optional[UUID] = Field(None, title="Broker Id")
 
 
-class DatasetReturning(BaseModel):
+class DatasetSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     name: str = Field(..., title="Name")
     broker_id: UUID = Field(..., title="Broker Id")
     kind: str = Field(..., title="Kind")
     num_used_by: int = Field(..., title="Num Used By")
 
 
 class DatasetUpdating(BaseModel):
@@ -320,14 +345,22 @@
 
 class GroupReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     name: Optional[str] = Field(None, title="Name")
     org_id: Optional[UUID] = Field(None, title="Org Id")
 
 
+class GroupSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    name: str = Field(..., title="Name")
+    org_id: UUID = Field(..., title="Org Id")
+
+
 class GroupUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
     name: Optional[str] = Field(None, title="Name")
 
 
 class InvitationCreating(BaseModel):
     org_id: UUID = Field(..., title="Org Id")
@@ -337,26 +370,36 @@
     vars: Optional[Dict[str, Any]] = Field({}, title="Vars")
 
 
 class InvitationDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
+class InvitationDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    org_id: UUID = Field(..., title="Org Id")
+    email: str = Field(..., title="Email")
+    hash: str = Field(..., title="Hash")
+    claimed: bool = Field(..., title="Claimed")
+
+
 class InvitationReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     org_id: Optional[UUID] = Field(None, title="Org Id")
     email: Optional[str] = Field(None, title="Email")
     hash: Optional[str] = Field(None, title="Hash")
     claimed: Optional[bool] = Field(None, title="Claimed")
 
 
-class InvitationReturning(BaseModel):
+class InvitationSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     org_id: UUID = Field(..., title="Org Id")
     email: str = Field(..., title="Email")
     hash: str = Field(..., title="Hash")
     claimed: bool = Field(..., title="Claimed")
 
 
 class InvitationUpdating(BaseModel):
@@ -403,17 +446,17 @@
     key: str = Field(..., title="Key")
     payload: Dict[str, Any] = Field(..., title="Payload")
     filter_keys: Optional[List[str]] = Field([], title="Filter Keys")
     namespace: Optional[str] = Field("", title="Namespace")
 
 
 class NomadEventDetail(BaseModel):
-    created: Optional[datetime] = Field(None, title="Created")
-    updated: Optional[datetime] = Field(None, title="Updated")
     id: Optional[UUID] = Field(None, title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
     broker_id: Optional[UUID] = Field(None, title="Broker Id")
     action_id: Optional[UUID] = Field(None, title="Action Id")
     task_id: Optional[UUID] = Field(None, title="Task Id")
     index: Optional[int] = Field(None, title="Index")
     topic: Optional[str] = Field(None, title="Topic")
     type: Optional[str] = Field(None, title="Type")
     key: Optional[str] = Field(None, title="Key")
@@ -472,24 +515,35 @@
     details: Dict[str, Union[str, int, float]] = Field(..., title="Details")
 
 
 class NotificationDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
+class NotificationDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    user_id: UUID = Field(..., title="User Id")
+    type: str = Field(..., title="Type")
+    message: str = Field(..., title="Message")
+    is_read: bool = Field(..., title="Is Read")
+    details: Dict[str, Any] = Field(..., title="Details")
+
+
 class NotificationReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     user_id: Optional[UUID] = Field(None, title="User Id")
     is_read: Optional[bool] = Field(None, title="Is Read")
 
 
-class NotificationReturning(BaseModel):
+class NotificationSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     user_id: UUID = Field(..., title="User Id")
     type: str = Field(..., title="Type")
     message: str = Field(..., title="Message")
     is_read: bool = Field(..., title="Is Read")
     details: Dict[str, Any] = Field(..., title="Details")
 
 
@@ -510,23 +564,30 @@
     name: str = Field(..., title="Name")
 
 
 class OrgDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
+class OrgDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    name: str = Field(..., title="Name")
+
+
 class OrgReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     name: Optional[str] = Field(None, title="Name")
 
 
-class OrgReturning(BaseModel):
+class OrgSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     name: str = Field(..., title="Name")
 
 
 class OrgUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
     name: Optional[str] = Field(None, title="Name")
 
@@ -541,14 +602,28 @@
 
 
 class PackageDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
     force: Optional[bool] = Field(False, title="Force")
 
 
+class PackageDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    name: str = Field(..., title="Name")
+    version: str = Field(..., title="Version")
+    environment: str = Field(..., title="Environment")
+    tasks_using: Optional[int] = Field(None, title="Tasks Using")
+    actions_using: Optional[int] = Field(None, title="Actions Using")
+    org_id: UUID = Field(..., title="Org Id")
+    filename: str = Field(..., title="Filename")
+    meta: Dict[str, Any] = Field(..., title="Meta")
+
+
 class PackageListingLatest(BaseModel):
     org_id: Optional[UUID] = Field(None, title="Org Id")
     broker_id: Optional[UUID] = Field(None, title="Broker Id")
 
 
 class PackageReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
@@ -560,90 +635,88 @@
 
 
 class PackageReadingLatest(BaseModel):
     name: str = Field(..., title="Name")
     broker_id: UUID = Field(..., title="Broker Id")
 
 
-class PackageReturning(BaseModel):
+class PackageSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
-    org_id: UUID = Field(..., title="Org Id")
-    filename: str = Field(..., title="Filename")
     name: str = Field(..., title="Name")
     version: str = Field(..., title="Version")
-    meta: Dict[str, Any] = Field(..., title="Meta")
     environment: str = Field(..., title="Environment")
     tasks_using: Optional[int] = Field(None, title="Tasks Using")
     actions_using: Optional[int] = Field(None, title="Actions Using")
 
 
-class PackageSummary(BaseModel):
-    id: UUID = Field(..., title="Id")
-    name: str = Field(..., title="Name")
-    version: str = Field(..., title="Version")
-
-
 class PackageUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
     meta: Optional[Dict[str, Any]] = Field(None, title="Meta")
 
 
-class PageAssetReturning(BaseModel):
-    items: List[AssetReturning] = Field(..., title="Items")
+class PageAssetSummary(BaseModel):
+    items: List[AssetSummary] = Field(..., title="Items")
+    total: int = Field(..., ge=0, title="Total")
+    page: int = Field(..., ge=1, title="Page")
+    size: int = Field(..., ge=1, title="Size")
+
+
+class PageBrokerPathSummary(BaseModel):
+    items: List[BrokerPathSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageBrokerPathReturning(BaseModel):
-    items: List[BrokerPathReturning] = Field(..., title="Items")
+class PageBrokerSummary(BaseModel):
+    items: List[BrokerSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageBrokerReturning(BaseModel):
-    items: List[BrokerReturning] = Field(..., title="Items")
+class PageDatasetSummary(BaseModel):
+    items: List[DatasetSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageDatasetReturning(BaseModel):
-    items: List[DatasetReturning] = Field(..., title="Items")
+class PageGroupSummary(BaseModel):
+    items: List[GroupSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageInvitationReturning(BaseModel):
-    items: List[InvitationReturning] = Field(..., title="Items")
+class PageInvitationSummary(BaseModel):
+    items: List[InvitationSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageNotificationReturning(BaseModel):
-    items: List[NotificationReturning] = Field(..., title="Items")
+class PageNotificationSummary(BaseModel):
+    items: List[NotificationSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageOrgReturning(BaseModel):
-    items: List[OrgReturning] = Field(..., title="Items")
+class PageOrgSummary(BaseModel):
+    items: List[OrgSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PagePackageReturning(BaseModel):
-    items: List[PackageReturning] = Field(..., title="Items")
+class PagePackageSummary(BaseModel):
+    items: List[PackageSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
 class PersonCreating(BaseModel):
     name: str = Field(..., title="Name")
@@ -656,26 +729,40 @@
 
 
 class PersonDeleting(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     email: Optional[str] = Field(None, title="Email")
 
 
+class PersonDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    name: str = Field(..., title="Name")
+    source: str = Field(..., title="Source")
+    email: str = Field(..., title="Email")
+    picture: str = Field(..., title="Picture")
+    avatar_url: str = Field(..., title="Avatar Url")
+    locale: str = Field(..., title="Locale")
+    verified: bool = Field(..., title="Verified")
+    preferences: Dict[str, Any] = Field(..., title="Preferences")
+
+
 class PersonReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     name: Optional[str] = Field(None, title="Name")
     source: Optional[str] = Field(None, title="Source")
     email: Optional[str] = Field(None, title="Email")
     verified: Optional[bool] = Field(None, title="Verified")
 
 
-class PersonReturning(BaseModel):
+class PersonSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     name: str = Field(..., title="Name")
     source: str = Field(..., title="Source")
     email: str = Field(..., title="Email")
     picture: str = Field(..., title="Picture")
     avatar_url: str = Field(..., title="Avatar Url")
     locale: str = Field(..., title="Locale")
     verified: bool = Field(..., title="Verified")
@@ -700,37 +787,46 @@
     description: str = Field(..., title="Description")
 
 
 class ProjectDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
-class ProjectReading(BaseModel):
-    id: Optional[UUID] = Field(None, title="Id")
-    name: Optional[str] = Field(None, title="Name")
-    org_id: Optional[UUID] = Field(None, title="Org Id")
-
-
-class ProjectReturning(BaseModel):
+class ProjectDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     org_id: UUID = Field(..., title="Org Id")
     name: str = Field(..., title="Name")
     description: str = Field(..., title="Description")
 
 
+class ProjectReading(BaseModel):
+    id: Optional[UUID] = Field(None, title="Id")
+    name: Optional[str] = Field(None, title="Name")
+    org_id: Optional[UUID] = Field(None, title="Org Id")
+
+
 class ProjectStats(BaseModel):
     annotations: int = Field(..., title="Annotations")
     annotators: int = Field(..., title="Annotators")
     live_sessions: int = Field(..., title="Live Sessions")
     tasks_count: int = Field(..., title="Tasks Count")
     actions_count: int = Field(..., title="Actions Count")
 
 
+class ProjectSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    org_id: UUID = Field(..., title="Org Id")
+    name: str = Field(..., title="Name")
+    description: str = Field(..., title="Description")
+
+
 class ProjectUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
     name: Optional[str] = Field(None, title="Name")
     description: Optional[str] = Field(None, title="Description")
 
 
 class RecipeDeleting(BaseModel):
@@ -748,31 +844,51 @@
     args: Dict[str, Any] = Field(..., title="Args")
 
 
 class RecipePlanDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
+class RecipePlanDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    project_id: UUID = Field(..., title="Project Id")
+    project_name: str = Field(..., title="Project Name")
+    recipe_id: UUID = Field(..., title="Recipe Id")
+    recipe_name: str = Field(..., title="Recipe Name")
+    recipe_title: Optional[str] = Field(None, title="Recipe Title")
+    package_id: UUID = Field(..., title="Package Id")
+    package_name: str = Field(..., title="Package Name")
+    package_version: str = Field(..., title="Package Version")
+    environment: str = Field(..., title="Environment")
+    args: Dict[str, Any] = Field(..., title="Args")
+    command: List[str] = Field(..., title="Command")
+    objects: Dict[str, Dict[str, Dict[str, Any]]] = Field(..., title="Objects")
+
+
 class RecipePlanReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     recipe_id: Optional[UUID] = Field(None, title="Recipe Id")
     project_id: Optional[UUID] = Field(None, title="Project Id")
 
 
-class RecipePlanReturning(BaseModel):
+class RecipePlanSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
-    recipe_id: UUID = Field(..., title="Recipe Id")
     project_id: UUID = Field(..., title="Project Id")
-    environment: str = Field(..., title="Environment")
+    project_name: str = Field(..., title="Project Name")
+    recipe_id: UUID = Field(..., title="Recipe Id")
     recipe_name: str = Field(..., title="Recipe Name")
-    args: Dict[str, Any] = Field(..., title="Args")
-    command: List[str] = Field(..., title="Command")
-    objects: Dict[str, Dict[str, Dict[str, Any]]] = Field(..., title="Objects")
+    recipe_title: Optional[str] = Field(None, title="Recipe Title")
+    package_id: UUID = Field(..., title="Package Id")
+    package_name: str = Field(..., title="Package Name")
+    package_version: str = Field(..., title="Package Version")
+    environment: str = Field(..., title="Environment")
 
 
 class RecipePlanUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
 class RecipeReading(BaseModel):
@@ -783,26 +899,25 @@
 
 
 class RecipeReadingLatest(BaseModel):
     name: str = Field(..., title="Name")
     broker_id: UUID = Field(..., title="Broker Id")
 
 
-class RecipeReturning(BaseModel):
+class RecipeSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     org_id: UUID = Field(..., title="Org Id")
     package_id: UUID = Field(..., title="Package Id")
     name: str = Field(..., title="Name")
-    title: str = Field(..., title="Title")
-    description: str = Field(..., title="Description")
+    title: Optional[str] = Field(None, title="Title")
+    description: Optional[str] = Field(None, title="Description")
     is_action: bool = Field(..., title="Is Action")
-    entry_point: str = Field(..., title="Entry Point")
-    meta: Dict[str, Any] = Field(..., title="Meta")
+    entry_point: Optional[str] = Field(None, title="Entry Point")
     num_used_by: int = Field(..., title="Num Used By")
 
 
 class RecipeUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
     title: str = Field(..., title="Title")
 
@@ -818,32 +933,32 @@
 
 
 class SecretDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
 class SecretDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     name: str = Field(..., title="Name")
     path: str = Field(..., title="Path")
     broker_id: UUID = Field(..., title="Broker Id")
 
 
 class SecretReading(BaseModel):
     name: Optional[str] = Field(None, title="Name")
     path: Optional[str] = Field(None, title="Path")
     broker_id: Optional[UUID] = Field(None, title="Broker Id")
 
 
-class SecretReturning(BaseModel):
+class SecretSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     name: str = Field(..., title="Name")
     path: str = Field(..., title="Path")
     broker_id: UUID = Field(..., title="Broker Id")
 
 
 class SecretUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
@@ -856,60 +971,72 @@
     task_id: UUID = Field(..., title="Task Id")
 
 
 class SessionDeleting(BaseModel):
     id: UUID = Field(..., title="Id")
 
 
+class SessionDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    user_id: UUID = Field(..., title="User Id")
+    user_name: str = Field(..., title="User Name")
+    user_avatar_url: str = Field(..., title="User Avatar Url")
+    task_id: UUID = Field(..., title="Task Id")
+    count: int = Field(..., title="Count")
+    time_spent: int = Field(..., title="Time Spent")
+
+
 class SessionReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     user_id: Optional[UUID] = Field(None, title="User Id")
     task_id: Optional[UUID] = Field(None, title="Task Id")
     count: Optional[int] = Field(None, title="Count")
     time_spent: Optional[int] = Field(None, title="Time Spent")
 
 
-class SessionReturning(BaseModel):
+class SessionSaving(BaseModel):
+    id: UUID = Field(..., title="Id")
+    count: Optional[int] = Field(None, title="Count")
+    time_spent: Optional[int] = Field(None, title="Time Spent")
+
+
+class SessionSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     user_id: UUID = Field(..., title="User Id")
     user_name: str = Field(..., title="User Name")
     user_avatar_url: str = Field(..., title="User Avatar Url")
     task_id: UUID = Field(..., title="Task Id")
     count: int = Field(..., title="Count")
     time_spent: int = Field(..., title="Time Spent")
 
 
-class SessionSaving(BaseModel):
-    id: UUID = Field(..., title="Id")
-    count: Optional[int] = Field(None, title="Count")
-    time_spent: Optional[int] = Field(None, title="Time Spent")
-
-
 class SessionUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
     count: Optional[int] = Field(None, title="Count")
 
 
 class TaskAnnotator(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
+    name: str = Field(..., title="Name")
     org_id: UUID = Field(..., title="Org Id")
     org_name: str = Field(..., title="Org Name")
     person_id: UUID = Field(..., title="Person Id")
-    name: str = Field(..., title="Name")
     email: str = Field(..., title="Email")
     avatar_url: str = Field(..., title="Avatar Url")
     locale: str = Field(..., title="Locale")
-    groups: List[str] = Field(..., title="Groups")
-    tags: List[str] = Field(..., title="Tags")
     is_org_admin: bool = Field(..., title="Is Org Admin")
     is_org_developer: bool = Field(..., title="Is Org Developer")
+    groups: List[str] = Field(..., title="Groups")
+    tags: List[str] = Field(..., title="Tags")
     live_sessions: int = Field(..., title="Live Sessions")
     annotations: int = Field(..., title="Annotations")
     hours: str = Field(..., title="Hours")
 
 
 class TaskCreating(BaseModel):
     name: str = Field(..., title="Name")
@@ -1010,18 +1137,29 @@
     annotations: int = Field(..., title="Annotations")
     annotators: int = Field(..., title="Annotators")
     live_sessions: int = Field(..., title="Live Sessions")
 
 
 class TaskSummary(BaseModel):
     id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
     project_id: UUID = Field(..., title="Project Id")
+    broker_id: UUID = Field(..., title="Broker Id")
     name: str = Field(..., title="Name")
-    job_type: JobType
+    recipe_name: str = Field(..., title="Recipe Name")
+    recipe_title: str = Field(..., title="Recipe Title")
     state: TaskState
+    project_name: str = Field(..., title="Project Name")
+    is_running: bool = Field(..., title="Is Running")
+    is_startable: bool = Field(..., title="Is Startable")
+    is_stoppable: bool = Field(..., title="Is Stoppable")
+    error: Optional[str] = Field(None, title="Error")
+    plan: RecipePlanSummary
+    job_type: JobType
 
 
 class TaskUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
     name: Optional[str] = Field(None, title="Name")
 
 
@@ -1047,35 +1185,50 @@
 
 class UserDeleting(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     org_id: Optional[UUID] = Field(None, title="Org Id")
     person_id: Optional[UUID] = Field(None, title="Person Id")
 
 
+class UserDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    name: str = Field(..., title="Name")
+    org_id: UUID = Field(..., title="Org Id")
+    org_name: str = Field(..., title="Org Name")
+    person_id: UUID = Field(..., title="Person Id")
+    email: str = Field(..., title="Email")
+    avatar_url: str = Field(..., title="Avatar Url")
+    locale: str = Field(..., title="Locale")
+    is_org_admin: bool = Field(..., title="Is Org Admin")
+    is_org_developer: bool = Field(..., title="Is Org Developer")
+    groups: List[str] = Field(..., title="Groups")
+    tags: List[str] = Field(..., title="Tags")
+
+
 class UserReading(BaseModel):
     id: Optional[UUID] = Field(None, title="Id")
     org_id: Optional[UUID] = Field(None, title="Org Id")
     person_id: Optional[UUID] = Field(None, title="Person Id")
     is_org_admin: Optional[bool] = Field(None, title="Is Org Admin")
     is_org_developer: Optional[bool] = Field(None, title="Is Org Developer")
 
 
-class UserReturning(BaseModel):
+class UserSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
+    name: str = Field(..., title="Name")
     org_id: UUID = Field(..., title="Org Id")
     org_name: str = Field(..., title="Org Name")
     person_id: UUID = Field(..., title="Person Id")
-    name: str = Field(..., title="Name")
     email: str = Field(..., title="Email")
     avatar_url: str = Field(..., title="Avatar Url")
     locale: str = Field(..., title="Locale")
-    groups: List[str] = Field(..., title="Groups")
-    tags: List[str] = Field(..., title="Tags")
     is_org_admin: bool = Field(..., title="Is Org Admin")
     is_org_developer: bool = Field(..., title="Is Org Developer")
 
 
 class UserUpdating(BaseModel):
     id: UUID = Field(..., title="Id")
     name: Optional[str] = Field(None, title="Name")
@@ -1134,53 +1287,33 @@
     id: Optional[UUID] = Field(None, title="Id")
     name: Optional[str] = Field(None, title="Name")
     state: Optional[ActionState] = None
     project_id: Optional[UUID] = Field(None, title="Project Id")
     broker_id: Optional[UUID] = Field(None, title="Broker Id")
 
 
-class ActionReturning(BaseModel):
+class ActionSummary(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
-    project_id: UUID = Field(..., title="Project Id")
-    broker_id: UUID = Field(..., title="Broker Id")
-    name: str = Field(..., title="Name")
-    recipe_name: str = Field(..., title="Recipe Name")
-    recipe_title: str = Field(..., title="Recipe Title")
-    state: ActionState
-    evaluation: str = Field(..., title="Evaluation")
-    project_name: str = Field(..., title="Project Name")
     is_running: bool = Field(..., title="Is Running")
     is_startable: bool = Field(..., title="Is Startable")
     is_stoppable: bool = Field(..., title="Is Stoppable")
-    error: Optional[str] = Field(None, title="Error")
-    plan: RecipePlanReturning
-    executions: List[ActionExecution] = Field(..., title="Executions")
-    last_execution_id: Optional[UUID] = Field(None, title="Last Execution Id")
-    nomad_index: int = Field(..., title="Nomad Index")
-    stats: ActionStats
-    cli_command: str = Field(..., title="Cli Command")
-    url_logs: str = Field(..., title="Url Logs")
-    url: str = Field(..., title="Url")
-    related_tasks: List[UUID] = Field(..., title="Related Tasks")
-
-
-class ActionSummary(BaseModel):
-    id: UUID = Field(..., title="Id")
-    project_id: UUID = Field(..., title="Project Id")
+    broker_id: UUID = Field(..., title="Broker Id")
     name: str = Field(..., title="Name")
+    project_id: UUID = Field(..., title="Project Id")
     job_type: JobType
     state: ActionState
+    plan: RecipePlanSummary
 
 
 class AssetDetail(BaseModel):
-    created: Optional[datetime] = Field(None, title="Created")
-    updated: Optional[datetime] = Field(None, title="Updated")
     id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
     broker_id: UUID = Field(..., title="Broker Id")
     name: str = Field(..., title="Name")
     kind: str = Field(..., title="Kind")
     path: str = Field(..., title="Path")
     meta: Dict[str, Any] = Field(..., title="Meta")
     tasks: List[TaskSummary] = Field(..., title="Tasks")
     actions: List[ActionSummary] = Field(..., title="Actions")
@@ -1194,35 +1327,35 @@
 
 class ClusterJobReturning(BaseModel):
     job_id: UUID = Field(..., title="Job Id")
     execution_id: Optional[UUID] = Field(None, title="Execution Id")
     attempt_id: UUID = Field(..., title="Attempt Id")
     job_type: JobType
     name: str = Field(..., title="Name")
-    plan: RecipePlanReturning
+    plan: RecipePlanDetail
 
 
 class DatasetDetail(BaseModel):
-    created: Optional[datetime] = Field(None, title="Created")
-    updated: Optional[datetime] = Field(None, title="Updated")
     id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
     broker_id: UUID = Field(..., title="Broker Id")
     name: str = Field(..., title="Name")
     kind: str = Field(..., title="Kind")
     tasks: List[TaskSummary] = Field(..., title="Tasks")
     actions: List[ActionSummary] = Field(..., title="Actions")
 
 
-class GroupReturning(BaseModel):
+class GroupDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     name: str = Field(..., title="Name")
     org_id: UUID = Field(..., title="Org Id")
-    users: List[UserReturning] = Field(..., title="Users")
+    users: List[UserDetail] = Field(..., title="Users")
 
 
 class HTTPValidationError(BaseModel):
     detail: Optional[List[ValidationError]] = Field(None, title="Detail")
 
 
 class NomadEventBatchCreating(BaseModel):
@@ -1264,79 +1397,79 @@
     Restarts: int = Field(..., title="Restarts")
     LastRestart: Optional[int] = Field(None, title="Lastrestart")
     StartedAt: Optional[datetime] = Field(None, title="Startedat")
     FinishedAt: Optional[datetime] = Field(None, title="Finishedat")
     Events: List[NomadTaskEvent] = Field(..., title="Events")
 
 
-class PageActionReturning(BaseModel):
-    items: List[ActionReturning] = Field(..., title="Items")
+class PageActionSummary(BaseModel):
+    items: List[ActionSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageGroupReturning(BaseModel):
-    items: List[GroupReturning] = Field(..., title="Items")
+class PagePersonSummary(BaseModel):
+    items: List[PersonSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PagePersonReturning(BaseModel):
-    items: List[PersonReturning] = Field(..., title="Items")
+class PageProjectSummary(BaseModel):
+    items: List[ProjectSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageProjectReturning(BaseModel):
-    items: List[ProjectReturning] = Field(..., title="Items")
+class PageRecipePlanSummary(BaseModel):
+    items: List[RecipePlanSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageRecipePlanReturning(BaseModel):
-    items: List[RecipePlanReturning] = Field(..., title="Items")
+class PageRecipeSummary(BaseModel):
+    items: List[RecipeSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageRecipeReturning(BaseModel):
-    items: List[RecipeReturning] = Field(..., title="Items")
+class PageSecretSummary(BaseModel):
+    items: List[SecretSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageSecretReturning(BaseModel):
-    items: List[SecretReturning] = Field(..., title="Items")
+class PageSessionSummary(BaseModel):
+    items: List[SessionSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageSessionReturning(BaseModel):
-    items: List[SessionReturning] = Field(..., title="Items")
+class PageTaskAnnotator(BaseModel):
+    items: List[TaskAnnotator] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageTaskAnnotator(BaseModel):
-    items: List[TaskAnnotator] = Field(..., title="Items")
+class PageTaskSummary(BaseModel):
+    items: List[TaskSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
-class PageUserReturning(BaseModel):
-    items: List[UserReturning] = Field(..., title="Items")
+class PageUserSummary(BaseModel):
+    items: List[UserSummary] = Field(..., title="Items")
     total: int = Field(..., ge=0, title="Total")
     page: int = Field(..., ge=1, title="Page")
     size: int = Field(..., ge=1, title="Size")
 
 
 class Props(BaseModel):
     name: Optional[str] = Field(None, title="Name")
@@ -1353,43 +1486,74 @@
     choice: Optional[Dict[str, Props]] = Field(None, title="Choice")
     min: Optional[float] = Field(None, title="Min")
     max: Optional[float] = Field(None, title="Max")
     step: Optional[float] = Field(None, title="Step")
     optional_title: Optional[str] = Field(None, title="Optional Title")
 
 
-class TaskReading(BaseModel):
-    id: Optional[UUID] = Field(None, title="Id")
-    name: Optional[str] = Field(None, title="Name")
-    state: Optional[TaskState] = None
-    project_id: Optional[UUID] = Field(None, title="Project Id")
-
-
-class TaskReturning(BaseModel):
+class TaskDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     project_id: UUID = Field(..., title="Project Id")
     broker_id: UUID = Field(..., title="Broker Id")
     name: str = Field(..., title="Name")
     recipe_name: str = Field(..., title="Recipe Name")
     recipe_title: str = Field(..., title="Recipe Title")
     state: TaskState
     project_name: str = Field(..., title="Project Name")
     is_running: bool = Field(..., title="Is Running")
     is_startable: bool = Field(..., title="Is Startable")
     is_stoppable: bool = Field(..., title="Is Stoppable")
     error: Optional[str] = Field(None, title="Error")
-    plan: RecipePlanReturning
+    plan: RecipePlanDetail
+    job_type: JobType
     nomad_index: int = Field(..., title="Nomad Index")
     last_execution_id: Optional[UUID] = Field(None, title="Last Execution Id")
     related_actions: List[UUID] = Field(..., title="Related Actions")
     cli_command: str = Field(..., title="Cli Command")
     url_logs: str = Field(..., title="Url Logs")
     url: str = Field(..., title="Url")
+    created_by_user: Optional[UserSummary] = None
+
+
+class TaskReading(BaseModel):
+    id: Optional[UUID] = Field(None, title="Id")
+    name: Optional[str] = Field(None, title="Name")
+    state: Optional[TaskState] = None
+    project_id: Optional[UUID] = Field(None, title="Project Id")
+
+
+class ActionDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
+    created: datetime = Field(..., title="Created")
+    updated: datetime = Field(..., title="Updated")
+    is_running: bool = Field(..., title="Is Running")
+    is_startable: bool = Field(..., title="Is Startable")
+    is_stoppable: bool = Field(..., title="Is Stoppable")
+    broker_id: UUID = Field(..., title="Broker Id")
+    name: str = Field(..., title="Name")
+    project_id: UUID = Field(..., title="Project Id")
+    job_type: JobType
+    state: ActionState
+    plan: RecipePlanDetail
+    recipe_name: str = Field(..., title="Recipe Name")
+    recipe_title: str = Field(..., title="Recipe Title")
+    evaluation: str = Field(..., title="Evaluation")
+    project_name: str = Field(..., title="Project Name")
+    error: Optional[str] = Field(None, title="Error")
+    executions: List[ActionExecution] = Field(..., title="Executions")
+    last_execution_id: Optional[UUID] = Field(None, title="Last Execution Id")
+    nomad_index: int = Field(..., title="Nomad Index")
+    stats: ActionStats
+    cli_command: str = Field(..., title="Cli Command")
+    url_logs: str = Field(..., title="Url Logs")
+    url: str = Field(..., title="Url")
+    related_tasks: List[UUID] = Field(..., title="Related Tasks")
+    created_by_user: Optional[UserSummary] = None
 
 
 class FieldSchema(BaseModel):
     name: str = Field(..., title="Name")
     type: TypeSchema
     props: Props
     fields: Optional[List[FieldSchema]] = Field([], title="Fields")
@@ -1419,21 +1583,14 @@
     PreemptedByAllocation: Optional[UUID] = Field(None, title="Preemptedbyallocation")
     CreateIndex: int = Field(..., title="Createindex")
     ModifyIndex: int = Field(..., title="Modifyindex")
     CreateTime: int = Field(..., title="Createtime")
     ModifyTime: int = Field(..., title="Modifytime")
 
 
-class PageTaskReturning(BaseModel):
-    items: List[TaskReturning] = Field(..., title="Items")
-    total: int = Field(..., ge=0, title="Total")
-    page: int = Field(..., ge=1, title="Page")
-    size: int = Field(..., ge=1, title="Size")
-
-
 class RecipeSchema(BaseModel):
     name: str = Field(..., title="Name")
     fields: List[FieldSchema] = Field(..., title="Fields")
     title: Optional[str] = Field(None, title="Title")
     description: Optional[str] = Field(None, title="Description")
     view_id: Optional[str] = Field(None, title="View Id")
     cli_names: Optional[Dict[str, str]] = Field(None, title="Cli Names")
@@ -1453,30 +1610,30 @@
     form_schema: RecipeSchema
     cli_schema: Dict[str, Any] = Field(..., title="Cli Schema")
     meta: Dict[str, Any] = Field(..., title="Meta")
     package_id: UUID = Field(..., title="Package Id")
 
 
 class RecipeDetail(BaseModel):
+    id: UUID = Field(..., title="Id")
     created: datetime = Field(..., title="Created")
     updated: datetime = Field(..., title="Updated")
-    id: UUID = Field(..., title="Id")
     org_id: UUID = Field(..., title="Org Id")
     package_id: UUID = Field(..., title="Package Id")
     name: str = Field(..., title="Name")
-    title: str = Field(..., title="Title")
-    description: str = Field(..., title="Description")
+    title: Optional[str] = Field(None, title="Title")
+    description: Optional[str] = Field(None, title="Description")
     is_action: bool = Field(..., title="Is Action")
-    entry_point: str = Field(..., title="Entry Point")
+    entry_point: Optional[str] = Field(None, title="Entry Point")
+    num_used_by: int = Field(..., title="Num Used By")
     form_schema: RecipeSchema
     cli_schema: Dict[str, Any] = Field(..., title="Cli Schema")
     meta: Dict[str, Any] = Field(..., title="Meta")
     tasks: List[TaskSummary] = Field(..., title="Tasks")
     actions: List[ActionSummary] = Field(..., title="Actions")
-    package: Optional[PackageSummary] = None
-    num_used_by: int = Field(..., title="Num Used By")
+    package: PackageSummary
 
 
 CackQuerying.update_forward_refs()
 TypeSchema.update_forward_refs()
 Props.update_forward_refs()
 FieldSchema.update_forward_refs()
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_utils.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_utils.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/ty.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/ty.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/assets.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/assets.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/dataset.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/decorator.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/decorator.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/props.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/props.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/types.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/types.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/sdk/util.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/sdk/util.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/types.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/types.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk/version/read_version.py` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk/version/read_version.py`

 * *Files identical despite different names*

### Comparing `prodigy-teams-recipes-sdk-0.1.2/prodigy_teams_recipes_sdk.egg-info/SOURCES.txt` & `prodigy-teams-recipes-sdk-0.1.3/prodigy_teams_recipes_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,33 +4,37 @@
 pyproject.toml
 setup.cfg
 setup.py
 prodigy_teams_recipes_sdk/__init__.py
 prodigy_teams_recipes_sdk/__main__.py
 prodigy_teams_recipes_sdk/about.json
 prodigy_teams_recipes_sdk/about.py
+prodigy_teams_recipes_sdk/testing.py
 prodigy_teams_recipes_sdk/types.py
 prodigy_teams_recipes_sdk.egg-info/PKG-INFO
 prodigy_teams_recipes_sdk.egg-info/SOURCES.txt
 prodigy_teams_recipes_sdk.egg-info/dependency_links.txt
 prodigy_teams_recipes_sdk.egg-info/entry_points.txt
 prodigy_teams_recipes_sdk.egg-info/not-zip-safe
 prodigy_teams_recipes_sdk.egg-info/requires.txt
 prodigy_teams_recipes_sdk.egg-info/top_level.txt
 prodigy_teams_recipes_sdk/engine/__init__.py
 prodigy_teams_recipes_sdk/engine/cli.py
-prodigy_teams_recipes_sdk/engine/preview.html
-prodigy_teams_recipes_sdk/engine/preview.js
 prodigy_teams_recipes_sdk/engine/preview.py
 prodigy_teams_recipes_sdk/engine/recipe.py
 prodigy_teams_recipes_sdk/engine/recipe_loader.py
 prodigy_teams_recipes_sdk/engine/recipe_schema.py
 prodigy_teams_recipes_sdk/engine/registry.py
 prodigy_teams_recipes_sdk/engine/teams_type.py
 prodigy_teams_recipes_sdk/engine/util.py
+prodigy_teams_recipes_sdk/engine/public/200.html
+prodigy_teams_recipes_sdk/engine/public/404.html
+prodigy_teams_recipes_sdk/engine/public/index.html
+prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.4c35cb5b.css
+prodigy_teams_recipes_sdk/engine/public/_nuxt/entry.d4386e81.js
 prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/__init__.py
 prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/errors.py
 prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/models.py
 prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/recipe_utils.py
 prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/ty.py
 prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/__init__.py
 prodigy_teams_recipes_sdk/prodigy_teams_pam_sdk/client/action.py
@@ -59,8 +63,10 @@
 prodigy_teams_recipes_sdk/sdk/dataset.py
 prodigy_teams_recipes_sdk/sdk/decorator.py
 prodigy_teams_recipes_sdk/sdk/props.py
 prodigy_teams_recipes_sdk/sdk/types.py
 prodigy_teams_recipes_sdk/sdk/util.py
 prodigy_teams_recipes_sdk/version/0.1.0_2023-05-12-12-39-11_patch_699f4418-3c53-4c0f-8a27-f838383451b1
 prodigy_teams_recipes_sdk/version/0.1.1_2023-05-17-11-05-43_patch_8e2fe949-3833-4639-84bf-bf1f5bcbe993
+prodigy_teams_recipes_sdk/version/0.1.2_2023-06-16-09-48-01_patch_7cae2ccc-2549-44a9-bbcf-3f56fa93b58e
+prodigy_teams_recipes_sdk/version/__init__.py
 prodigy_teams_recipes_sdk/version/read_version.py
```

### Comparing `prodigy-teams-recipes-sdk-0.1.2/setup.py` & `prodigy-teams-recipes-sdk-0.1.3/setup.py`

 * *Files identical despite different names*

