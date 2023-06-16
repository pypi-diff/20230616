# Comparing `tmp/gitlabracadabra-1.9.0.tar.gz` & `tmp/gitlabracadabra-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabracadabra-1.9.0.tar", last modified: Wed Aug 31 09:08:00 2022, max compression
+gzip compressed data, was "gitlabracadabra-1.9.1.tar", last modified: Tue Sep 20 11:45:01 2022, max compression
```

## Comparing `gitlabracadabra-1.9.0.tar` & `gitlabracadabra-1.9.1.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.409669 gitlabracadabra-1.9.0/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7651 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/LICENSE
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       93 2021-02-09 21:28:09.000000 gitlabracadabra-1.9.0/MANIFEST.in
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6660 2022-08-31 09:08:00.409669 gitlabracadabra-1.9.0/PKG-INFO
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5640 2022-08-31 09:07:02.000000 gitlabracadabra-1.9.0/README.md
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.273661 gitlabracadabra-1.9.0/gitlabracadabra/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      965 2022-08-31 09:07:02.000000 gitlabracadabra-1.9.0/gitlabracadabra/__init__.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1300 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/auth_info.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5006 2021-05-21 14:14:32.000000 gitlabracadabra-1.9.0/gitlabracadabra/cli.py
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.281661 gitlabracadabra-1.9.0/gitlabracadabra/containers/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       26 2021-03-03 09:51:20.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/__init__.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8939 2022-08-31 09:04:14.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/authenticated_session.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1267 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/blob.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2138 2021-04-14 19:20:15.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/const.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4253 2021-09-17 09:22:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/manifest.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3147 2021-06-16 08:47:56.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/manifest_base.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5414 2021-06-16 08:47:56.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/registries.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1660 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/registry.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    15572 2022-06-28 18:44:02.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/registry_importer.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4146 2022-06-28 20:14:11.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/registry_session.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      881 2021-04-11 06:42:40.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/scope.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2774 2021-09-17 09:26:04.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/with_blobs.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9528 2022-01-05 09:54:46.000000 gitlabracadabra-1.9.0/gitlabracadabra/containers/with_digest.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1589 2021-03-13 09:14:56.000000 gitlabracadabra-1.9.0/gitlabracadabra/dictutils.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1544 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.0/gitlabracadabra/disk_cache.py
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.285662 gitlabracadabra-1.9.0/gitlabracadabra/gitlab/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-03-13 15:15:54.000000 gitlabracadabra-1.9.0/gitlabracadabra/gitlab/__init__.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1278 2021-03-13 09:30:28.000000 gitlabracadabra-1.9.0/gitlabracadabra/gitlab/access_levels.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      963 2021-03-17 09:43:20.000000 gitlabracadabra-1.9.0/gitlabracadabra/gitlab/connection.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2396 2021-03-17 09:29:14.000000 gitlabracadabra-1.9.0/gitlabracadabra/gitlab/connections.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3247 2021-06-16 08:54:25.000000 gitlabracadabra-1.9.0/gitlabracadabra/gitlab/group_cache.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1630 2021-03-17 10:07:14.000000 gitlabracadabra-1.9.0/gitlabracadabra/gitlab/pygit2.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3478 2021-06-16 08:34:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/gitlab/pygitlab.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3070 2021-06-16 08:54:25.000000 gitlabracadabra-1.9.0/gitlabracadabra/gitlab/user_cache.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6193 2022-05-06 12:39:26.000000 gitlabracadabra-1.9.0/gitlabracadabra/matchers.py
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.293662 gitlabracadabra-1.9.0/gitlabracadabra/mixins/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/__init__.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12115 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/boards.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4951 2021-05-07 08:28:38.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/groups.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8102 2022-01-05 09:54:46.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/image_mirrors.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5120 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/labels.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4495 2021-03-17 13:11:56.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/members.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5510 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/milestones.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11883 2021-05-19 16:44:36.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/mirrors.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2672 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/package_mirrors.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11136 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/pipeline_schedules.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2386 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/rename_branches.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4600 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/variables.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4135 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/mixins/webhooks.py
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.297662 gitlabracadabra-1.9.0/gitlabracadabra/objects/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/objects/__init__.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    39605 2022-06-29 08:32:53.000000 gitlabracadabra-1.9.0/gitlabracadabra/objects/application_settings.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19563 2021-05-07 08:28:38.000000 gitlabracadabra-1.9.0/gitlabracadabra/objects/group.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    13792 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.0/gitlabracadabra/objects/object.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    74405 2022-06-29 08:34:04.000000 gitlabracadabra-1.9.0/gitlabracadabra/objects/project.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9754 2022-07-21 09:12:59.000000 gitlabracadabra-1.9.0/gitlabracadabra/objects/user.py
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.305663 gitlabracadabra-1.9.0/gitlabracadabra/packages/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       24 2021-05-12 19:41:20.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/__init__.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10036 2022-02-23 15:01:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/destination.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7274 2021-06-16 08:54:25.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/github.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5919 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/gitlab.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4947 2022-07-06 14:52:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/helm.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3210 2021-06-16 08:47:56.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/package_file.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3009 2021-09-17 08:34:24.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/pip.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8489 2022-02-23 15:01:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/pypi.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4106 2021-06-16 08:47:56.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/raw.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1138 2021-05-28 13:56:30.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/source.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2859 2021-09-17 08:34:24.000000 gitlabracadabra-1.9.0/gitlabracadabra/packages/stream.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6019 2022-06-17 08:58:04.000000 gitlabracadabra-1.9.0/gitlabracadabra/parser.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1486 2021-03-13 07:24:36.000000 gitlabracadabra-1.9.0/gitlabracadabra/singleton.py
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.309663 gitlabracadabra-1.9.0/gitlabracadabra/tests/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      907 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/__init__.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3433 2022-04-13 07:37:15.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/case.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1389 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/patchfuncs.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      121 2022-08-31 08:56:18.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/python-gitlab.cfg
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.325664 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/__init__.py
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.393668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)   958338 2022-08-31 09:05:54.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ApplicationSettings_settings.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11767 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Blob_open.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    18948 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/GroupBoards_boards.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1288 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/GroupCache_get_full_path_from_id.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1307 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/GroupCache_get_id_from_full_path.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3550 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_create.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2452 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_delete.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1405 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_exists.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5448 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_groups.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4627 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_groups_change_access_level.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2697 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_groups_delete_unknown.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2673 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_groups_not_found.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8526 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_labels.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6554 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_members.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4435 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_members_change_access_level.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4002 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_members_delete_unknown.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4729 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_members_not_found.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12419 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_milestones.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1721 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_missing_parent.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      959 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_no_create.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9096 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_simple_parameters.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10810 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_variables.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9958 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Manifest_blobs.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12755 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Manifest_blobs_manifest_v1.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    17350 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Manifest_not_found.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    26748 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Manifest_tag_list.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    33160 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectBoards_boards.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    44108 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_digest.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    79419 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_manifest_v1.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    14062 2021-04-10 10:57:53.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_manifest_v1_exists.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    63467 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_no_digest_header.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    54863 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_auth.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)   198179 2021-04-12 19:29:56.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_mocked.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)   134882 2021-05-03 10:51:08.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_mounted.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    64184 2022-08-31 07:10:29.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_redirect.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5981 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectMirror_mirrors_pull.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5981 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectMirror_mirrors_pull_mappings.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    27844 2021-06-09 09:25:44.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_github.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    15828 2021-05-20 15:45:02.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_github_tarball.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10946 2021-07-07 19:25:03.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_helm.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8550 2021-05-26 14:41:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_helm_exists.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    30278 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_pypi.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19973 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_pypi_exists.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    18102 2021-05-20 13:00:18.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_raw.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19344 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectRenameBranches_rename_branches.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6807 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_archived.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9529 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_branches.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    20940 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_container_expiration_policy.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5021 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_create.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5923 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_default_branch_exists.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3959 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_default_branch_not_exists.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4437 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_delete.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2891 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_exists.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5165 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_groups.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4876 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_groups_change_access_level.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3777 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_groups_delete_unknown.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3796 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_groups_not_found.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10714 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_labels.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8121 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_members.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6002 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_members_change_access_level.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5569 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_members_delete_unknown.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6033 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_members_not_found.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    14402 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_milestones.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      964 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_no_create.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11686 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_pipeline_schedule_variables.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    13106 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_pipeline_schedules.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5640 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_branches_delete.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6054 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_branches_wildcard.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8288 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_change.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7059 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_delete.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7238 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_wildcard.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    57990 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_simple_parameters.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    51267 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_simple_parameters2.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6839 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_unarchived.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12558 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_variables.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    26005 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_webhooks.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10240 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_blob.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    29819 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11475 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_already_exists.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    35068 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    51629 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list_all.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    17094 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list_dry_run.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8553 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_not_found.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9463 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_manifest.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    14488 2022-06-28 16:00:40.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_manifest_list.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2394 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/UserCache_id_from_username.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1783 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/UserCache_username_from_id.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3580 2021-11-10 21:14:09.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_activate.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3572 2021-11-10 21:10:23.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_block.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3313 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_create.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3577 2021-11-10 21:13:39.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_deactivate.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3442 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_delete.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2247 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_exists.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1515 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_no_create.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    43388 2021-03-03 15:29:20.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_simple_parameters.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3575 2021-11-10 21:11:51.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_unblock.yaml
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.393668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       23 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/HEAD
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       66 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/config
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.265660 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.393668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/40/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       51 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/40/dbdf55dfd4065422462cc74a949254aefa972e
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.397668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/54/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       51 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/54/3b9bebdc6bd5c4b22136034a95dd097a57d3dd
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.397668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/5e/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      134 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/5e/8dfc288cf87620e22e67b6db671dc8a596e2f9
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.397668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/80/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       28 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/80/2992c4220de19a90767f3000a79a31b98d0df7
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.397668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/8d/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      166 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/8d/1fd4e584faf465d96e2f9b3cbd5000721469b3
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.397668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/e6/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       15 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.265660 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.397668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/heads/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       41 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/heads/hello
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       41 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/heads/master
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.397668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/tags/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       41 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/tags/tag1
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       41 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/tags/tag2
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.405668 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-05-12 19:41:20.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/__init__.py
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.409669 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)   313875 2021-05-19 16:54:27.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Github_package_files_assets.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5887 2021-05-19 16:54:27.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Github_package_files_latest_balls.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    13950 2021-05-15 20:58:39.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Gitlab_import_source.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2624 2021-05-26 14:11:09.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1150 2021-05-26 14:11:09.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files_index_not_found.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)   257614 2021-05-27 10:31:08.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files_relative.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7034 2021-07-07 19:51:10.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)   106867 2022-01-05 11:24:01.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files_yanked_equal.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)   106867 2022-01-05 11:24:01.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files_yanked_le.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2831 2021-05-21 13:09:26.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Stream_e2e.yaml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11008 2022-01-05 09:54:46.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_destination.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5767 2021-06-09 09:25:44.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_github.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3244 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_gitlab.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4104 2022-07-06 14:57:09.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_helm.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3556 2021-05-12 19:41:20.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_package_file.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6466 2022-01-05 11:24:32.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_pypi.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5861 2021-05-28 14:01:40.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_raw.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1111 2021-05-28 13:55:24.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_source.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3381 2021-05-21 13:49:21.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_stream.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19650 2022-08-31 09:05:54.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_application_settings.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2253 2022-04-13 07:15:01.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_blob.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3464 2021-03-13 09:07:42.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_dictutils.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3774 2022-04-26 19:21:22.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_gitlab_connections.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9512 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_group.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2214 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_group_boards.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1722 2021-03-17 10:45:20.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_group_cache.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4110 2021-06-16 08:50:47.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_manifest.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5445 2021-06-16 12:37:47.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_matchers.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11447 2022-06-29 08:42:54.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_parser.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    20661 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2890 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_boards.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19783 2022-08-31 07:06:44.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_image_mirrors.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8214 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_mirror.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    14832 2022-01-05 10:05:58.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_package_mirrors.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2240 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_rename_branches.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5036 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_registries.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10531 2022-06-28 20:14:11.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_registry.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2406 2022-06-28 20:14:11.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_token.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4197 2021-11-10 21:14:06.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_user.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1692 2021-03-17 13:53:18.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_user_cache.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2865 2022-08-31 08:56:15.000000 gitlabracadabra-1.9.0/gitlabracadabra/tests/vcrfuncs.py
-drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-08-31 09:08:00.273661 gitlabracadabra-1.9.0/gitlabracadabra.egg-info/
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6660 2022-08-31 09:07:59.000000 gitlabracadabra-1.9.0/gitlabracadabra.egg-info/PKG-INFO
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12420 2022-08-31 09:08:00.000000 gitlabracadabra-1.9.0/gitlabracadabra.egg-info/SOURCES.txt
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)        1 2022-08-31 09:07:59.000000 gitlabracadabra-1.9.0/gitlabracadabra.egg-info/dependency_links.txt
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       61 2022-08-31 09:07:59.000000 gitlabracadabra-1.9.0/gitlabracadabra.egg-info/entry_points.txt
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       98 2022-08-31 09:07:59.000000 gitlabracadabra-1.9.0/gitlabracadabra.egg-info/requires.txt
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       16 2022-08-31 09:07:59.000000 gitlabracadabra-1.9.0/gitlabracadabra.egg-info/top_level.txt
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4060 2022-06-29 08:55:19.000000 gitlabracadabra-1.9.0/gitlabracadabra.yml
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)      235 2022-08-31 09:05:54.000000 gitlabracadabra-1.9.0/requirements.txt
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       38 2022-08-31 09:08:00.409669 gitlabracadabra-1.9.0/setup.cfg
--rwxr-xr-x   0 mathieu   (1000) mathieu   (1000)     2096 2021-10-29 10:20:33.000000 gitlabracadabra-1.9.0/setup.py
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)       29 2022-08-31 07:29:13.000000 gitlabracadabra-1.9.0/test-requirements.txt
--rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5338 2022-08-31 09:04:14.000000 gitlabracadabra-1.9.0/tox.ini
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.859077 gitlabracadabra-1.9.1/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7651 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/LICENSE
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       93 2021-02-09 21:28:09.000000 gitlabracadabra-1.9.1/MANIFEST.in
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6660 2022-09-20 11:45:01.859077 gitlabracadabra-1.9.1/PKG-INFO
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5640 2022-09-20 11:44:22.000000 gitlabracadabra-1.9.1/README.md
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.795076 gitlabracadabra-1.9.1/gitlabracadabra/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      965 2022-09-20 11:44:22.000000 gitlabracadabra-1.9.1/gitlabracadabra/__init__.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1300 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/auth_info.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5006 2021-05-21 14:14:32.000000 gitlabracadabra-1.9.1/gitlabracadabra/cli.py
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.799076 gitlabracadabra-1.9.1/gitlabracadabra/containers/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       26 2021-03-03 09:51:20.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/__init__.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8939 2022-08-31 09:04:14.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/authenticated_session.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1267 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/blob.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2138 2021-04-14 19:20:15.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/const.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4253 2021-09-17 09:22:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/manifest.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3147 2021-06-16 08:47:56.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/manifest_base.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5414 2021-06-16 08:47:56.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/registries.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1660 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/registry.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    15572 2022-06-28 18:44:02.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/registry_importer.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4146 2022-06-28 20:14:11.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/registry_session.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      881 2021-04-11 06:42:40.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/scope.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2774 2021-09-17 09:26:04.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/with_blobs.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9528 2022-01-05 09:54:46.000000 gitlabracadabra-1.9.1/gitlabracadabra/containers/with_digest.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1589 2021-03-13 09:14:56.000000 gitlabracadabra-1.9.1/gitlabracadabra/dictutils.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1544 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.1/gitlabracadabra/disk_cache.py
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.803076 gitlabracadabra-1.9.1/gitlabracadabra/gitlab/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-03-13 15:15:54.000000 gitlabracadabra-1.9.1/gitlabracadabra/gitlab/__init__.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1278 2021-03-13 09:30:28.000000 gitlabracadabra-1.9.1/gitlabracadabra/gitlab/access_levels.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      963 2021-03-17 09:43:20.000000 gitlabracadabra-1.9.1/gitlabracadabra/gitlab/connection.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2396 2021-03-17 09:29:14.000000 gitlabracadabra-1.9.1/gitlabracadabra/gitlab/connections.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3247 2021-06-16 08:54:25.000000 gitlabracadabra-1.9.1/gitlabracadabra/gitlab/group_cache.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1630 2021-03-17 10:07:14.000000 gitlabracadabra-1.9.1/gitlabracadabra/gitlab/pygit2.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3478 2021-06-16 08:34:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/gitlab/pygitlab.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3070 2021-06-16 08:54:25.000000 gitlabracadabra-1.9.1/gitlabracadabra/gitlab/user_cache.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6193 2022-05-06 12:39:26.000000 gitlabracadabra-1.9.1/gitlabracadabra/matchers.py
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.803076 gitlabracadabra-1.9.1/gitlabracadabra/mixins/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/__init__.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12115 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/boards.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4951 2021-05-07 08:28:38.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/groups.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8102 2022-01-05 09:54:46.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/image_mirrors.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5120 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/labels.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4495 2021-03-17 13:11:56.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/members.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5510 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/milestones.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11883 2021-05-19 16:44:36.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/mirrors.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2672 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/package_mirrors.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11136 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/pipeline_schedules.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2386 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/rename_branches.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4600 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/variables.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4135 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/mixins/webhooks.py
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.807076 gitlabracadabra-1.9.1/gitlabracadabra/objects/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/objects/__init__.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    39605 2022-06-29 08:32:53.000000 gitlabracadabra-1.9.1/gitlabracadabra/objects/application_settings.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19563 2021-05-07 08:28:38.000000 gitlabracadabra-1.9.1/gitlabracadabra/objects/group.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    13792 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.1/gitlabracadabra/objects/object.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    74405 2022-06-29 08:34:04.000000 gitlabracadabra-1.9.1/gitlabracadabra/objects/project.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9754 2022-07-21 09:12:59.000000 gitlabracadabra-1.9.1/gitlabracadabra/objects/user.py
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.807076 gitlabracadabra-1.9.1/gitlabracadabra/packages/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       24 2021-05-12 19:41:20.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/__init__.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10036 2022-02-23 15:01:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/destination.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7274 2021-06-16 08:54:25.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/github.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5919 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/gitlab.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4947 2022-07-06 14:52:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/helm.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3210 2021-06-16 08:47:56.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/package_file.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3009 2021-09-17 08:34:24.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/pip.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8489 2022-02-23 15:01:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/pypi.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4106 2021-06-16 08:47:56.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/raw.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1138 2021-05-28 13:56:30.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/source.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2859 2021-09-17 08:34:24.000000 gitlabracadabra-1.9.1/gitlabracadabra/packages/stream.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6019 2022-06-17 08:58:04.000000 gitlabracadabra-1.9.1/gitlabracadabra/parser.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1486 2021-03-13 07:24:36.000000 gitlabracadabra-1.9.1/gitlabracadabra/singleton.py
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.811076 gitlabracadabra-1.9.1/gitlabracadabra/tests/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      907 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/__init__.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3433 2022-04-13 07:37:15.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/case.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1389 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/patchfuncs.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      121 2022-08-31 08:56:18.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/python-gitlab.cfg
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.815076 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/__init__.py
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.847077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)   958338 2022-08-31 09:05:54.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ApplicationSettings_settings.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11767 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Blob_open.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    18948 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/GroupBoards_boards.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1288 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/GroupCache_get_full_path_from_id.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1307 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/GroupCache_get_id_from_full_path.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3550 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_create.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2452 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_delete.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1405 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_exists.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5448 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_groups.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4627 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_groups_change_access_level.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2697 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_groups_delete_unknown.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2673 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_groups_not_found.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8526 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_labels.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6554 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_members.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4435 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_members_change_access_level.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4002 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_members_delete_unknown.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4729 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_members_not_found.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12419 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_milestones.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1721 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_missing_parent.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      959 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_no_create.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9096 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_simple_parameters.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10810 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_variables.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9958 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Manifest_blobs.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12755 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Manifest_blobs_manifest_v1.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    17350 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Manifest_not_found.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    26748 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Manifest_tag_list.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    33160 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectBoards_boards.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    44108 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_digest.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    79419 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_manifest_v1.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    14062 2021-04-10 10:57:53.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_manifest_v1_exists.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    63467 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_no_digest_header.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    54863 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_auth.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)   198179 2021-04-12 19:29:56.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_mocked.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)   134882 2021-05-03 10:51:08.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_mounted.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    64184 2022-08-31 07:10:29.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_redirect.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5981 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectMirror_mirrors_pull.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5981 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectMirror_mirrors_pull_mappings.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    27844 2021-06-09 09:25:44.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_github.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    15828 2021-05-20 15:45:02.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_github_tarball.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10946 2021-07-07 19:25:03.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_helm.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8550 2021-05-26 14:41:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_helm_exists.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    30278 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_pypi.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19973 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_pypi_exists.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    18102 2021-05-20 13:00:18.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_raw.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19344 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectRenameBranches_rename_branches.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6807 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_archived.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9529 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_branches.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    20940 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_container_expiration_policy.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5021 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_create.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5923 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_default_branch_exists.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3959 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_default_branch_not_exists.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4437 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_delete.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2891 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_exists.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5165 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_groups.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4876 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_groups_change_access_level.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3777 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_groups_delete_unknown.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3796 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_groups_not_found.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10714 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_labels.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8121 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_members.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6002 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_members_change_access_level.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5569 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_members_delete_unknown.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6033 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_members_not_found.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    14402 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_milestones.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      964 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_no_create.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11686 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_pipeline_schedule_variables.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    13106 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_pipeline_schedules.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5640 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_branches_delete.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6054 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_branches_wildcard.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8288 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_change.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7059 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_delete.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7238 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_wildcard.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    57990 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_simple_parameters.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    51267 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_simple_parameters2.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6839 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_unarchived.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12558 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_variables.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    26005 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_webhooks.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10240 2021-02-27 22:06:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_blob.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    29819 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11475 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_already_exists.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    35068 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    51629 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list_all.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    17094 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list_dry_run.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8553 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_not_found.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9463 2021-04-11 06:58:07.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_manifest.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    14488 2022-06-28 16:00:40.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_manifest_list.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2394 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/UserCache_id_from_username.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1783 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/UserCache_username_from_id.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3580 2021-11-10 21:14:09.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_activate.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3572 2021-11-10 21:10:23.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_block.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3313 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_create.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3577 2021-11-10 21:13:39.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_deactivate.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3442 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_delete.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2247 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_exists.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1515 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_no_create.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    43388 2021-03-03 15:29:20.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_simple_parameters.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3575 2021-11-10 21:11:51.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_unblock.yaml
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.847077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       23 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/HEAD
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       66 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/config
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.791076 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.847077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/40/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       51 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/40/dbdf55dfd4065422462cc74a949254aefa972e
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.847077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/54/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       51 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/54/3b9bebdc6bd5c4b22136034a95dd097a57d3dd
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.847077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/5e/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      134 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/5e/8dfc288cf87620e22e67b6db671dc8a596e2f9
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.847077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/80/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       28 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/80/2992c4220de19a90767f3000a79a31b98d0df7
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.847077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/8d/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      166 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/8d/1fd4e584faf465d96e2f9b3cbd5000721469b3
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.851077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/e6/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       15 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.791076 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.851077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/heads/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       41 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/heads/hello
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       41 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/heads/master
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.851077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/tags/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       41 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/tags/tag1
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       41 2021-01-15 10:32:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/testrepo.git/refs/tags/tag2
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.851077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)        0 2021-05-12 19:41:20.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/__init__.py
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.859077 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)   313875 2021-05-19 16:54:27.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Github_package_files_assets.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5887 2021-05-19 16:54:27.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Github_package_files_latest_balls.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    13950 2021-05-15 20:58:39.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Gitlab_import_source.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2624 2021-05-26 14:11:09.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1150 2021-05-26 14:11:09.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files_index_not_found.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)   257614 2021-05-27 10:31:08.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files_relative.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     7034 2021-07-07 19:51:10.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)   106867 2022-01-05 11:24:01.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files_yanked_equal.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)   106867 2022-01-05 11:24:01.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files_yanked_le.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2831 2021-05-21 13:09:26.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Stream_e2e.yaml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11008 2022-01-05 09:54:46.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_destination.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5767 2021-06-09 09:25:44.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_github.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3244 2021-07-07 20:48:17.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_gitlab.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4104 2022-07-06 14:57:09.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_helm.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3556 2021-05-12 19:41:20.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_package_file.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6466 2022-01-05 11:24:32.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_pypi.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5861 2021-05-28 14:01:40.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_raw.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1111 2021-05-28 13:55:24.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_source.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3381 2021-05-21 13:49:21.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_stream.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19897 2022-09-20 11:31:36.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_application_settings.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2253 2022-04-13 07:15:01.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_blob.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3464 2021-03-13 09:07:42.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_dictutils.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     3774 2022-04-26 19:21:22.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_gitlab_connections.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     9512 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_group.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2214 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_group_boards.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1722 2021-03-17 10:45:20.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_group_cache.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4110 2021-06-16 08:50:47.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_manifest.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5445 2021-06-16 12:37:47.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_matchers.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    11447 2022-06-29 08:42:54.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_parser.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    20661 2022-04-13 14:04:27.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2890 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_boards.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    19783 2022-08-31 07:06:44.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_image_mirrors.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     8214 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_mirror.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    14832 2022-01-05 10:05:58.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_package_mirrors.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2240 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_rename_branches.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5036 2021-03-03 21:27:33.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_registries.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    10531 2022-06-28 20:14:11.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_registry.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2406 2022-06-28 20:14:11.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_token.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4197 2021-11-10 21:14:06.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_user.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     1692 2021-03-17 13:53:18.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_user_cache.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     2865 2022-08-31 08:56:15.000000 gitlabracadabra-1.9.1/gitlabracadabra/tests/vcrfuncs.py
+drwxr-xr-x   0 mathieu   (1000) mathieu   (1000)        0 2022-09-20 11:45:01.799076 gitlabracadabra-1.9.1/gitlabracadabra.egg-info/
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     6660 2022-09-20 11:45:01.000000 gitlabracadabra-1.9.1/gitlabracadabra.egg-info/PKG-INFO
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)    12420 2022-09-20 11:45:01.000000 gitlabracadabra-1.9.1/gitlabracadabra.egg-info/SOURCES.txt
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)        1 2022-09-20 11:45:01.000000 gitlabracadabra-1.9.1/gitlabracadabra.egg-info/dependency_links.txt
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       61 2022-09-20 11:45:01.000000 gitlabracadabra-1.9.1/gitlabracadabra.egg-info/entry_points.txt
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       98 2022-09-20 11:45:01.000000 gitlabracadabra-1.9.1/gitlabracadabra.egg-info/requires.txt
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       16 2022-09-20 11:45:01.000000 gitlabracadabra-1.9.1/gitlabracadabra.egg-info/top_level.txt
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     4060 2022-06-29 08:55:19.000000 gitlabracadabra-1.9.1/gitlabracadabra.yml
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)      235 2022-09-20 11:16:13.000000 gitlabracadabra-1.9.1/requirements.txt
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       38 2022-09-20 11:45:01.859077 gitlabracadabra-1.9.1/setup.cfg
+-rwxr-xr-x   0 mathieu   (1000) mathieu   (1000)     2096 2021-10-29 10:20:33.000000 gitlabracadabra-1.9.1/setup.py
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)       29 2022-09-20 11:16:13.000000 gitlabracadabra-1.9.1/test-requirements.txt
+-rw-r--r--   0 mathieu   (1000) mathieu   (1000)     5338 2022-08-31 09:04:14.000000 gitlabracadabra-1.9.1/tox.ini
```

### Comparing `gitlabracadabra-1.9.0/LICENSE` & `gitlabracadabra-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/PKG-INFO` & `gitlabracadabra-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabracadabra
-Version: 1.9.0
+Version: 1.9.1
 Summary: Adds some magic to GitLab
 Home-page: https://gitlab.com/gitlabracadabra/gitlabracadabra
 Author: Mathieu Parent
 Author-email: math.parent@gmail.com
 License: LGPL3
 Keywords: gitlab api yaml
 Classifier: Development Status :: 5 - Production/Stable
@@ -82,15 +82,15 @@
 
 Example usage:
 
 ```shell
 sudo docker run -ti \
   -v "$HOME/.python-gitlab.cfg:/home/gitlabracadabra/.python-gitlab.cfg:ro" \
   -v "$PWD/gitlabracadabra.yml:/app/gitlabracadabra.yml:ro" \
-  'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.0' \
+  'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.1' \
   --verbose --dry-run
 ```
 
 Other images are available. Examples:
 
 - `registry.gitlab.com/gitlabracadabra/gitlabracadabra/main`: Current `main`
 - `registry.gitlab.com/gitlabracadabra/gitlabracadabra/main:b1cd3482bf9583c5db863c359e12cafcdb7119bf`: A specific commit of `main`
@@ -152,15 +152,15 @@
 - [Define](https://docs.gitlab.com/ee/ci/variables/README.html#create-a-custom-variable-in-the-ui) the
 `GITLAB_PRIVATE_TOKEN` **protected** variable
 - Use it in your jobs to configure `python-gitlab`. Example `.gitlab-ci.yml`:
 
 ```yaml
 default:
   image:
-    name: 'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.0'
+    name: 'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.1'
     entrypoint: [""]
   before_script:
     - |
         cat << EOF > ~/.python-gitlab.cfg
         [global]
         default = gitlab
         [gitlab]
```

### Comparing `gitlabracadabra-1.9.0/README.md` & `gitlabracadabra-1.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 Example usage:
 
 ```shell
 sudo docker run -ti \
   -v "$HOME/.python-gitlab.cfg:/home/gitlabracadabra/.python-gitlab.cfg:ro" \
   -v "$PWD/gitlabracadabra.yml:/app/gitlabracadabra.yml:ro" \
-  'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.0' \
+  'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.1' \
   --verbose --dry-run
 ```
 
 Other images are available. Examples:
 
 - `registry.gitlab.com/gitlabracadabra/gitlabracadabra/main`: Current `main`
 - `registry.gitlab.com/gitlabracadabra/gitlabracadabra/main:b1cd3482bf9583c5db863c359e12cafcdb7119bf`: A specific commit of `main`
@@ -126,15 +126,15 @@
 - [Define](https://docs.gitlab.com/ee/ci/variables/README.html#create-a-custom-variable-in-the-ui) the
 `GITLAB_PRIVATE_TOKEN` **protected** variable
 - Use it in your jobs to configure `python-gitlab`. Example `.gitlab-ci.yml`:
 
 ```yaml
 default:
   image:
-    name: 'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.0'
+    name: 'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.1'
     entrypoint: [""]
   before_script:
     - |
         cat << EOF > ~/.python-gitlab.cfg
         [global]
         default = gitlab
         [gitlab]
```

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/__init__.py` & `gitlabracadabra-1.9.1/gitlabracadabra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """GitLabracadabra."""
 
 __title__ = 'gitlabracadabra'
-__version__ = '1.9.0'
+__version__ = '1.9.1'
 __author__ = 'Mathieu Parent'
 __email__ = 'math.parent@gmail.com'
 __license__ = 'LGPL3'
 __copyright__ = 'Copyright 2019-2020 Mathieu Parent'
```

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/auth_info.py` & `gitlabracadabra-1.9.1/gitlabracadabra/auth_info.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/cli.py` & `gitlabracadabra-1.9.1/gitlabracadabra/cli.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/authenticated_session.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/authenticated_session.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/blob.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/blob.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/const.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/const.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/manifest.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/manifest.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/manifest_base.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/manifest_base.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/registries.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/registries.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/registry.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/registry.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/registry_importer.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/registry_importer.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/registry_session.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/registry_session.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/scope.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/scope.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/with_blobs.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/with_blobs.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/containers/with_digest.py` & `gitlabracadabra-1.9.1/gitlabracadabra/containers/with_digest.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/dictutils.py` & `gitlabracadabra-1.9.1/gitlabracadabra/dictutils.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/disk_cache.py` & `gitlabracadabra-1.9.1/gitlabracadabra/disk_cache.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/gitlab/access_levels.py` & `gitlabracadabra-1.9.1/gitlabracadabra/gitlab/access_levels.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/gitlab/connection.py` & `gitlabracadabra-1.9.1/gitlabracadabra/gitlab/connection.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/gitlab/connections.py` & `gitlabracadabra-1.9.1/gitlabracadabra/gitlab/connections.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/gitlab/group_cache.py` & `gitlabracadabra-1.9.1/gitlabracadabra/gitlab/group_cache.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/gitlab/pygit2.py` & `gitlabracadabra-1.9.1/gitlabracadabra/gitlab/pygit2.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/gitlab/pygitlab.py` & `gitlabracadabra-1.9.1/gitlabracadabra/gitlab/pygitlab.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/gitlab/user_cache.py` & `gitlabracadabra-1.9.1/gitlabracadabra/gitlab/user_cache.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/matchers.py` & `gitlabracadabra-1.9.1/gitlabracadabra/matchers.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/boards.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/boards.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/groups.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/image_mirrors.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/image_mirrors.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/labels.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/labels.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/members.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/members.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/milestones.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/milestones.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/mirrors.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/mirrors.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/package_mirrors.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/package_mirrors.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/pipeline_schedules.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/pipeline_schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/rename_branches.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/rename_branches.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/variables.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/variables.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/mixins/webhooks.py` & `gitlabracadabra-1.9.1/gitlabracadabra/mixins/webhooks.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/objects/application_settings.py` & `gitlabracadabra-1.9.1/gitlabracadabra/objects/application_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/objects/group.py` & `gitlabracadabra-1.9.1/gitlabracadabra/objects/group.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/objects/object.py` & `gitlabracadabra-1.9.1/gitlabracadabra/objects/object.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/objects/project.py` & `gitlabracadabra-1.9.1/gitlabracadabra/objects/project.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/objects/user.py` & `gitlabracadabra-1.9.1/gitlabracadabra/objects/user.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/destination.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/destination.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/github.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/github.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/gitlab.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/helm.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/helm.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/package_file.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/package_file.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/pip.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/pip.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/pypi.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/pypi.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/raw.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/raw.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/source.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/source.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/packages/stream.py` & `gitlabracadabra-1.9.1/gitlabracadabra/packages/stream.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/parser.py` & `gitlabracadabra-1.9.1/gitlabracadabra/parser.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/singleton.py` & `gitlabracadabra-1.9.1/gitlabracadabra/singleton.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/__init__.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/case.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/case.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/patchfuncs.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/patchfuncs.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ApplicationSettings_settings.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ApplicationSettings_settings.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Blob_open.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Blob_open.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/GroupBoards_boards.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/GroupBoards_boards.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/GroupCache_get_full_path_from_id.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/GroupCache_get_full_path_from_id.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/GroupCache_get_id_from_full_path.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/GroupCache_get_id_from_full_path.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_create.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_create.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_delete.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_delete.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_exists.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_exists.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_groups.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_groups.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_groups_change_access_level.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_groups_change_access_level.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_groups_delete_unknown.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_groups_delete_unknown.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_groups_not_found.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_groups_not_found.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_labels.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_labels.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_members.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_members.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_members_change_access_level.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_members_change_access_level.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_members_delete_unknown.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_members_delete_unknown.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_members_not_found.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_members_not_found.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_milestones.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_milestones.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_missing_parent.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_missing_parent.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_no_create.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_no_create.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_simple_parameters.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_simple_parameters.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Group_variables.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Group_variables.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Manifest_blobs.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Manifest_blobs.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Manifest_blobs_manifest_v1.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Manifest_blobs_manifest_v1.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Manifest_not_found.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Manifest_not_found.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Manifest_tag_list.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Manifest_tag_list.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectBoards_boards.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectBoards_boards.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_digest.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_digest.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_manifest_v1.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_manifest_v1.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_manifest_v1_exists.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_manifest_v1_exists.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_no_digest_header.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirror_no_digest_header.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_auth.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_auth.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_mocked.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_mocked.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_mounted.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_mounted.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_redirect.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectImageMirrors_image_mirrors_redirect.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectMirror_mirrors_pull.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectMirror_mirrors_pull.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectMirror_mirrors_pull_mappings.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectMirror_mirrors_pull_mappings.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_github.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_github.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_github_tarball.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_github_tarball.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_helm.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_helm.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_helm_exists.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_helm_exists.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_pypi.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_pypi.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_pypi_exists.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_pypi_exists.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_raw.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectPackageMirrors_package_mirrors_raw.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/ProjectRenameBranches_rename_branches.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/ProjectRenameBranches_rename_branches.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_archived.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_archived.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_branches.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_branches.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_container_expiration_policy.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_container_expiration_policy.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_create.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_create.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_default_branch_exists.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_default_branch_exists.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_default_branch_not_exists.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_default_branch_not_exists.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_delete.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_delete.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_exists.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_exists.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_groups.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_groups.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_groups_change_access_level.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_groups_change_access_level.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_groups_delete_unknown.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_groups_delete_unknown.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_groups_not_found.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_groups_not_found.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_labels.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_labels.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_members.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_members.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_members_change_access_level.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_members_change_access_level.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_members_delete_unknown.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_members_delete_unknown.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_members_not_found.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_members_not_found.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_milestones.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_milestones.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_no_create.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_no_create.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_pipeline_schedule_variables.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_pipeline_schedule_variables.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_pipeline_schedules.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_pipeline_schedules.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_branches_delete.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_branches_delete.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_branches_wildcard.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_branches_wildcard.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_change.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_change.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_delete.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_delete.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_wildcard.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_protected_tags_wildcard.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_simple_parameters.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_simple_parameters.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_simple_parameters2.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_simple_parameters2.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_unarchived.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_unarchived.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_variables.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_variables.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Project_webhooks.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Project_webhooks.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_blob.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_blob.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_already_exists.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_already_exists.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list_all.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list_all.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list_dry_run.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_list_dry_run.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_not_found.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_import_manifest_not_found.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_manifest.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_manifest.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/Registry_manifest_list.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/Registry_manifest_list.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/UserCache_id_from_username.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/UserCache_id_from_username.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/UserCache_username_from_id.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/UserCache_username_from_id.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_activate.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_activate.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_block.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_block.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_create.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_create.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_deactivate.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_deactivate.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_delete.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_delete.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_exists.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_exists.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_no_create.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_no_create.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_simple_parameters.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_simple_parameters.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/fixtures/User_unblock.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/fixtures/User_unblock.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Github_package_files_assets.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Github_package_files_assets.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Github_package_files_latest_balls.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Github_package_files_latest_balls.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Gitlab_import_source.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Gitlab_import_source.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files_index_not_found.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files_index_not_found.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files_relative.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Helm_package_files_relative.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files_yanked_equal.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files_yanked_equal.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files_yanked_le.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/PyPI_package_files_yanked_le.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/fixtures/Stream_e2e.yaml` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/fixtures/Stream_e2e.yaml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_destination.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_destination.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_github.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_github.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_gitlab.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_helm.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_helm.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_package_file.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_package_file.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_pypi.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_pypi.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_raw.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_raw.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_source.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_source.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/packages/test_stream.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/packages/test_stream.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_application_settings.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_application_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,27 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from unittest import skipIf
+
+from gitlab import __version__ as gitlab_version
+
+from packaging.version import parse as version_parse
+
 from gitlabracadabra.objects.application_settings import GitLabracadabraApplicationSettings
 from gitlabracadabra.tests import my_vcr
 from gitlabracadabra.tests.case import TestCaseWithManager
 
 
 class TestApplicationSettings(TestCaseWithManager):
+    @skipIf(version_parse(gitlab_version) < version_parse('3.7.0'), 'python-gitlab without proper array support')
     @my_vcr.use_cassette
     def test_settings(self, cass):
         # On the GitLab rails console, before recording:
         # ApplicationSetting.first.delete
         obj = GitLabracadabraApplicationSettings('memory', 'application_settings', {
             # 'abuse_notification_email': 'some string',
             # 'admin_mode': True,
```

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_blob.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_blob.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_dictutils.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_dictutils.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_gitlab_connections.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_gitlab_connections.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_group.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_group.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_group_boards.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_group_boards.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_group_cache.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_group_cache.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_manifest.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_manifest.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_matchers.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_matchers.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_parser.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_parser.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_boards.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_boards.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_image_mirrors.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_image_mirrors.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_mirror.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_mirror.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_package_mirrors.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_package_mirrors.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_project_rename_branches.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_project_rename_branches.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_registries.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_registries.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_registry.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_registry.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_token.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_token.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_user.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_user.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/unit/test_user_cache.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/unit/test_user_cache.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra/tests/vcrfuncs.py` & `gitlabracadabra-1.9.1/gitlabracadabra/tests/vcrfuncs.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra.egg-info/PKG-INFO` & `gitlabracadabra-1.9.1/gitlabracadabra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabracadabra
-Version: 1.9.0
+Version: 1.9.1
 Summary: Adds some magic to GitLab
 Home-page: https://gitlab.com/gitlabracadabra/gitlabracadabra
 Author: Mathieu Parent
 Author-email: math.parent@gmail.com
 License: LGPL3
 Keywords: gitlab api yaml
 Classifier: Development Status :: 5 - Production/Stable
@@ -82,15 +82,15 @@
 
 Example usage:
 
 ```shell
 sudo docker run -ti \
   -v "$HOME/.python-gitlab.cfg:/home/gitlabracadabra/.python-gitlab.cfg:ro" \
   -v "$PWD/gitlabracadabra.yml:/app/gitlabracadabra.yml:ro" \
-  'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.0' \
+  'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.1' \
   --verbose --dry-run
 ```
 
 Other images are available. Examples:
 
 - `registry.gitlab.com/gitlabracadabra/gitlabracadabra/main`: Current `main`
 - `registry.gitlab.com/gitlabracadabra/gitlabracadabra/main:b1cd3482bf9583c5db863c359e12cafcdb7119bf`: A specific commit of `main`
@@ -152,15 +152,15 @@
 - [Define](https://docs.gitlab.com/ee/ci/variables/README.html#create-a-custom-variable-in-the-ui) the
 `GITLAB_PRIVATE_TOKEN` **protected** variable
 - Use it in your jobs to configure `python-gitlab`. Example `.gitlab-ci.yml`:
 
 ```yaml
 default:
   image:
-    name: 'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.0'
+    name: 'registry.gitlab.com/gitlabracadabra/gitlabracadabra:v1.9.1'
     entrypoint: [""]
   before_script:
     - |
         cat << EOF > ~/.python-gitlab.cfg
         [global]
         default = gitlab
         [gitlab]
```

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra.egg-info/SOURCES.txt` & `gitlabracadabra-1.9.1/gitlabracadabra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/gitlabracadabra.yml` & `gitlabracadabra-1.9.1/gitlabracadabra.yml`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/setup.py` & `gitlabracadabra-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `gitlabracadabra-1.9.0/tox.ini` & `gitlabracadabra-1.9.1/tox.ini`

 * *Files identical despite different names*

