# Comparing `tmp/iambic_core-0.9.1.tar.gz` & `tmp/iambic_core-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.9.1.tar", max compression
+gzip compressed data, was "iambic_core-0.9.6.tar", max compression
```

## Comparing `iambic_core-0.9.1.tar` & `iambic_core-0.9.6.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0    11356 2023-06-13 13:55:31.171837 iambic_core-0.9.1/LICENSE.md
--rw-r--r--   0        0        0    15630 2023-06-13 13:55:31.171837 iambic_core-0.9.1/README.md
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/config/__init__.py
--rw-r--r--   0        0        0    19724 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0     3312 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/config/utils.py
--rw-r--r--   0        0        0    79176 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/context.py
--rw-r--r--   0        0        0      609 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15943 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4845 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1844 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/logger.py
--rw-r--r--   0        0        0    25633 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/noq_json.py
--rw-r--r--   0        0        0     5515 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/parser.py
--rw-r--r--   0        0        0    48281 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/template_generation.py
--rw-r--r--   0        0        0    33010 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.203837 iambic_core-0.9.1/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/lambda/app.py
--rw-r--r--   0        0        0    14434 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/main.py
--rw-r--r--   0        0        0      664 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/__init__.py
--rw-r--r--   0        0        0     2799 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1753 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     2728 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     2268 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
--rw-r--r--   0        0        0     2712 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     2102 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    17407 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0     1721 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    39712 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10334 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    18144 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13681 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15896 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    18077 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10706 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16135 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21757 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    24602 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14064 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    21076 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22644 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     5842 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    31619 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20296 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35636 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    30301 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/__init__.py
--rw-r--r--   0        0        0      101 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/exceptions.py
--rw-r--r--   0        0        0    18860 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/models.py
--rw-r--r--   0        0        0    11040 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py
--rw-r--r--   0        0        0    19286 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py
--rw-r--r--   0        0        0     1291 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0     3009 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/template_generation.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-06-13 13:55:31.207837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    10209 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    14003 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3820 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2283 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     2033 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8515 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8798 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3783 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0     1128 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     3366 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      284 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    34737 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    12212 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     2015 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5383 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14801 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5437 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1359 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7860 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3029 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3177 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9327 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3176 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11442 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3606 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    20065 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2502 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2890 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1290 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9587 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3495 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13610 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0     1002 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4293 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      994 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      173 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12636 2023-06-13 13:55:31.211837 iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     2263 2023-06-13 13:55:31.215837 iambic_core-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    17598 1970-01-01 00:00:00.000000 iambic_core-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-15 22:09:36.885295 iambic_core-0.9.6/LICENSE.md
+-rw-r--r--   0        0        0    15653 2023-06-15 22:09:36.885295 iambic_core-0.9.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.921296 iambic_core-0.9.6/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/config/__init__.py
+-rw-r--r--   0        0        0    19724 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0     3312 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/config/utils.py
+-rw-r--r--   0        0        0    78470 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15943 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4845 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1946 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/logger.py
+-rw-r--r--   0        0        0    25633 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5515 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/parser.py
+-rw-r--r--   0        0        0    48281 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    33010 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/lambda/app.py
+-rw-r--r--   0        0        0    14703 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2799 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1753 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     2728 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     2268 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     2712 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     2102 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    18133 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0     1721 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    39712 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.925296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    18144 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13681 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    16084 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    18077 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10706 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    22080 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24602 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    21076 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22644 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     5842 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31619 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35636 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    30478 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/__init__.py
+-rw-r--r--   0        0        0      101 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/exceptions.py
+-rw-r--r--   0        0        0    18860 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/models.py
+-rw-r--r--   0        0        0    11040 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py
+-rw-r--r--   0        0        0    19286 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py
+-rw-r--r--   0        0        0     1291 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     3009 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10209 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    14003 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3820 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2283 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     2033 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8515 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8798 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3783 2023-06-15 22:09:36.929296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0     1128 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    34737 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    12212 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     2015 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5383 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14801 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5437 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1359 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7860 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3029 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3177 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9327 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3176 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11442 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3606 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2502 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2890 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1290 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9587 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3495 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13610 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0     1002 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4293 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      994 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      173 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-06-15 22:09:36.933296 iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     2263 2023-06-15 22:09:36.937296 iambic_core-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0    17621 1970-01-01 00:00:00.000000 iambic_core-0.9.6/PKG-INFO
```

### Comparing `iambic_core-0.9.1/LICENSE.md` & `iambic_core-0.9.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/README.md` & `iambic_core-0.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 - **[Dynamic AWS Permissions](https://docs.iambic.org/getting_started/aws#31---create-dynamic-iam-role-policies-that-vary-per-account)**: Simplify multi-account AWS management with flexible templates, allowing multi-account roles to have different permissions and access rules on different accounts.
 - **[Drift Prevention](https://docs.iambic.org/how_to_guides/prevent-drift)**: Protect the IAM resources you want to be exclusively managed via IAMbic. What is in Git becomes the absolute source of truth.
 - **[GitOps-driven Cloud IAM (IAMOps)](https://docs.iambic.org/reference/iamops_philosophy)**: Leverage GitOps-driven Cloud IAM with human-readable formats and your favorite tools.
 - **Centralized Management**: IAMbic keeps Git updated with the latest, complete state of your cloud environment, maintaining a single source of truth for auditing and compliance across multiple cloud providers in Git.
 - **Extendable**: Integrate with various clouds and applications through a powerful plugin architecture.
 - **Auditable**: Track changes to IAM policies, permissions, and rules with Git history. For AWS, IAmbic annotates out-of-band commits with details from CloudTrail.
 
-Check out [IAMbic IAMOps Philosophy](/reference/iamops_philosophy) and an [example IAMbic templates repository](https://github.com/noqdev/iambic-templates-examples) to see a real-life example of IAMbic.
+Check out [IAMbic IAMOps Philosophy](https://docs.iambic.org/reference/iamops_philosophy) and an [example IAMbic templates repository](https://github.com/noqdev/iambic-templates-examples) to see a real-life example of IAMbic.
 
 ## 📣 Let's chat
 
 Do you want to connect with our contributors?
 
 Just click the button below and follow the instructions.
```

### Comparing `iambic_core-0.9.1/iambic/config/dynamic_config.py` & `iambic_core-0.9.6/iambic/config/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/config/utils.py` & `iambic_core-0.9.6/iambic/config/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/config/wizard.py` & `iambic_core-0.9.6/iambic/config/wizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,22 +358,41 @@
         check_and_update_resource_limit(self.config)
         log.debug("Starting configuration wizard", config_path=self.config_path)
 
     @property
     def has_cf_permissions(self):
         if self._has_cf_permissions is None:
             try:
+                with contextlib.suppress(
+                    ClientError, NoCredentialsError, FileNotFoundError
+                ):
+                    org_client = self.boto3_session.client("organizations")
+                    self.autodetected_org_settings = org_client.describe_organization()[
+                        "Organization"
+                    ]
+                    self._has_cf_permissions = "member.org.stacksets.cloudformation.amazonaws.com" in [
+                        p["ServicePrincipal"]
+                        for p in org_client.list_aws_service_access_for_organization()[
+                            "EnabledServicePrincipals"
+                        ]
+                    ]
+                    if self._has_cf_permissions:
+                        return self._has_cf_permissions
+
                 click.echo(
                     f"\nThis requires that you have the ability to "
                     f"create CloudFormation stacks, stack sets, and stack set instances.\n"
                     f"If you are using an AWS Organization, be sure that trusted access is enabled.\n"
                     f"You can check this using the AWS Console:\n  "
                     f"https://{self.aws_default_region}.console.aws.amazon.com/organizations/v2/home/services/CloudFormation%20StackSets"
                 )
-                self._has_cf_permissions = questionary.confirm("Proceed?").unsafe_ask()
+                if self._has_cf_permissions is None:
+                    self._has_cf_permissions = questionary.confirm(
+                        "Proceed?"
+                    ).unsafe_ask()
             except KeyboardInterrupt:
                 log.info("Exiting...")
                 sys.exit(0)
 
         return self._has_cf_permissions
 
     @property
@@ -557,15 +576,14 @@
         except KeyboardInterrupt:
             log.info("Exiting...")
             sys.exit(0)
 
         return profile_name if profile_name != "None" else None
 
     def set_boto3_session(self, allow_none=False):
-        self._has_cf_permissions = True
         while True:
             try:
                 profile_name = self.set_aws_profile_name(allow_none=allow_none)
                 self.boto3_session = boto3.Session(
                     profile_name=profile_name, region_name=self.aws_default_region
                 )
                 self.caller_identity = self.boto3_session.client(
@@ -609,33 +627,14 @@
                     "\n - Ensure that the credentials have the correct permissions"
                     "\n - Ensure that the credentials are not expired"
                     "\n - Ensure that the credentials are not for a federated user"
                 )
                 continue
 
             self.profile_name = profile_name
-            with contextlib.suppress(
-                ClientError, NoCredentialsError, FileNotFoundError
-            ):
-                org_client = self.boto3_session.client(
-                    "organizations", region_name=self.aws_default_region
-                )
-                self.autodetected_org_settings = org_client.describe_organization()[
-                    "Organization"
-                ]
-                self._has_cf_permissions = (
-                    "member.org.stacksets.cloudformation.amazonaws.com"
-                    in [
-                        p["ServicePrincipal"]
-                        for p in org_client.list_aws_service_access_for_organization()[
-                            "EnabledServicePrincipals"
-                        ]
-                    ]
-                )
-
             break
 
     def get_boto3_session_for_account(self, account_id: str, region_name: str = None):
         # This need to follow standard credentials provider chain
         if not region_name:
             region_name = self.aws_default_region
 
@@ -1086,52 +1085,38 @@
             identity_arn = get_identity_arn(default_caller_identity)
             click.echo(
                 f"\nIAMbic detected you are using {identity_arn} for AWS access.\n"
                 f"This identity will require the ability to create"
                 f"CloudFormation stacks, stack sets, and stack set instances."
             )
             if questionary.confirm("Would you like to use this identity?").ask():
-                self.caller_identity = default_caller_identity
                 # If we are going to use the default_caller_identity,
                 # we need to set teh autodetected_org_settings to
-                with contextlib.suppress(
-                    ClientError, NoCredentialsError, FileNotFoundError
-                ):
-                    org_client = self.boto3_session.client("organizations")
-                    self.autodetected_org_settings = org_client.describe_organization()[
-                        "Organization"
-                    ]
-                    self._has_cf_permissions = "member.org.stacksets.cloudformation.amazonaws.com" in [
-                        p["ServicePrincipal"]
-                        for p in org_client.list_aws_service_access_for_organization()[
-                            "EnabledServicePrincipals"
-                        ]
-                    ]
+                self.caller_identity = default_caller_identity
             else:
                 self.set_boto3_session()
         else:
             self.set_boto3_session()
 
         asyncio.run(self.sync_config_aws_org())
 
     def configuration_wizard_aws_accounts(self):
-        while True:
-            if self.config.aws and self.config.aws.accounts:
-                action = questionary.select(
-                    "What would you like to do?",
-                    choices=["Go back", "Add AWS Account", "Edit AWS Account"],
-                ).unsafe_ask()
-                if action == "Go back":
-                    return
-                elif action == "Add AWS Account":
-                    self.configuration_wizard_aws_account_add()
-                elif action == "Edit AWS Account":
-                    self.configuration_wizard_aws_account_edit()
-            else:
+        if self.config.aws and self.config.aws.accounts:
+            action = questionary.select(
+                "What would you like to do?",
+                choices=["Go back", "Add AWS Account", "Edit AWS Account"],
+            ).unsafe_ask()
+            if action == "Go back":
+                return
+            elif action == "Add AWS Account":
                 self.configuration_wizard_aws_account_add()
+            elif action == "Edit AWS Account":
+                self.configuration_wizard_aws_account_edit()
+        else:
+            self.configuration_wizard_aws_account_add()
 
     def configuration_wizard_aws_organizations_edit(self):
         org_ids = [org.org_id for org in self.config.aws.organizations]
         org_id_to_config_elem_map = {
             org.org_id: elem for elem, org in enumerate(self.config.aws.organizations)
         }
         if len(org_ids) > 1:
```

### Comparing `iambic_core-0.9.1/iambic/core/aio_utils/__init__.py` & `iambic_core-0.9.6/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/core/exceptions.py` & `iambic_core-0.9.6/iambic/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/core/git.py` & `iambic_core-0.9.6/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/core/iambic_enum.py` & `iambic_core-0.9.6/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/core/iambic_plugin.py` & `iambic_core-0.9.6/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/core/logger.py` & `iambic_core-0.9.6/iambic/core/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,30 +24,31 @@
 
         return_dict[key] = value
 
     return return_dict
 
 
 def configure_logger(logger_name, log_level):
-    structlog.configure(
-        processors=[
-            pretty_log,
-            structlog.processors.add_log_level,
-            structlog.processors.StackInfoRenderer(),
-            structlog.dev.set_exc_info,
-            structlog.processors.TimeStamper("%Y/%m/%d %H:%M:%S", utc=False),
-            structlog.dev.ConsoleRenderer(),
-        ],
-        wrapper_class=structlog.make_filtering_bound_logger(
-            logging.getLevelName(log_level)
-        ),
-        context_class=dict,
-        logger_factory=structlog.PrintLoggerFactory(),
-        cache_logger_on_first_use=False,
-    )
+    if not structlog.is_configured():
+        structlog.configure(
+            processors=[
+                pretty_log,
+                structlog.processors.add_log_level,
+                structlog.processors.StackInfoRenderer(),
+                structlog.dev.set_exc_info,
+                structlog.processors.TimeStamper("%Y/%m/%d %H:%M:%S", utc=False),
+                structlog.dev.ConsoleRenderer(),
+            ],
+            wrapper_class=structlog.make_filtering_bound_logger(
+                logging.getLevelName(log_level)
+            ),
+            context_class=dict,
+            logger_factory=structlog.PrintLoggerFactory(),
+            cache_logger_on_first_use=False,
+        )
     log = structlog.get_logger(logger_name)
 
     if log_level == "DEBUG":
         boto3.set_stream_logger("", "DEBUG")
     else:
         default_logging_levels = {
             "boto3": "CRITICAL",
```

### Comparing `iambic_core-0.9.1/iambic/core/models.py` & `iambic_core-0.9.6/iambic/core/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/core/noq_json.py` & `iambic_core-0.9.6/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/core/parser.py` & `iambic_core-0.9.6/iambic/core/parser.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/core/template_generation.py` & `iambic_core-0.9.6/iambic/core/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/core/utils.py` & `iambic_core-0.9.6/iambic/core/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.9.6/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.9.6/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.9.6/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/github/templates/iambic-import.yml` & `iambic_core-0.9.6/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/github/utils.py` & `iambic_core-0.9.6/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/lambda/app.py` & `iambic_core-0.9.6/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/main.py` & `iambic_core-0.9.6/iambic/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,20 +91,20 @@
 def expire(templates: list[str], repo_dir: str):
     run_expire(templates, repo_dir=repo_dir)
 
 
 def run_expire(templates: list[str], repo_dir: str = str(pathlib.Path.cwd())):
     config_path = asyncio.run(resolve_config_template_path(repo_dir))
     # load_config is required to populate known templates
-    asyncio.run(load_config(config_path))
+    config = asyncio.run(load_config(config_path))
 
     if not templates:
         templates = asyncio.run(gather_templates(repo_dir))
 
-    asyncio.run(flag_expired_resources(templates))
+    asyncio.run(flag_expired_resources(templates, config.template_map))
 
 
 @cli.command()
 @click.option(
     "--repo-dir",
     "-d",
     "repo_dir",
@@ -359,15 +359,24 @@
         templates = asyncio.run(gather_templates(repo_dir))
 
     config_path = asyncio.run(resolve_config_template_path(repo_dir))
     config = asyncio.run(load_config(config_path))
     exe_message = ExecutionMessage(
         execution_id=str(uuid.uuid4()), command=Command.APPLY
     )
-    asyncio.run(flag_expired_resources(templates))
+
+    try:
+        asyncio.run(flag_expired_resources(templates, config.template_map))
+    except IsADirectoryError:
+        log.error(
+            f"Invalid template path: {templates}. Templates must be files."
+            f"A directory cannot be passed in."
+        )
+        sys.exit(1)
+
     ctx.eval_only = True
     template_changes = asyncio.run(
         config.run_apply(exe_message, load_templates(templates, config.template_map))
     )
     output_proposed_changes(template_changes)
     screen_render_resource_changes(template_changes)
```

### Comparing `iambic_core-0.9.1/iambic/output/__init__.py` & `iambic_core-0.9.6/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/output/filters.py` & `iambic_core-0.9.6/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/output/models.py` & `iambic_core-0.9.6/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.9.6/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.9.6/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.9.6/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/output/text.py` & `iambic_core-0.9.6/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/README.md` & `iambic_core-0.9.6/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import asyncio
 import os
 from datetime import datetime, timedelta
 from typing import Any, Optional, Union
 
+from aws_error_utils.aws_error_utils import ClientError, get_aws_error_info
+
 from iambic.core.logger import log
 from iambic.plugins.v0_1_0.aws.models import (
     IAMBIC_CHANGE_DETECTION_SUFFIX,
     IAMBIC_HUB_ROLE_NAME,
     IAMBIC_SPOKE_ROLE_NAME,
     get_hub_role_arn,
 )
@@ -145,24 +147,36 @@
             stack_set_name=stack_set_name,
             stack_set_url=f"https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacksets\n",
         )
         return True
     except client.exceptions.StackSetNotFoundException:
         pass
 
-    await boto_crud_call(
-        client.create_stack_set,
-        StackSetName=stack_set_name,
-        TemplateBody=template_body,
-        Parameters=parameters,
-        PermissionModel="SERVICE_MANAGED",
-        AutoDeployment={"Enabled": True, "RetainStacksOnAccountRemoval": True},
-        ManagedExecution={"Active": True},
-        **kwargs,
-    )
+    try:
+        await boto_crud_call(
+            client.create_stack_set,
+            StackSetName=stack_set_name,
+            TemplateBody=template_body,
+            Parameters=parameters,
+            PermissionModel="SERVICE_MANAGED",
+            AutoDeployment={"Enabled": True, "RetainStacksOnAccountRemoval": True},
+            ManagedExecution={"Active": True},
+            **kwargs,
+        )
+    except ClientError as err:
+        err_info = get_aws_error_info(err)
+        expected_message = "You must enable organizations access to operate a service managed stack set"
+
+        if err_info.message and expected_message in err_info.message:
+            log.error(
+                f"{expected_message}.\n"
+                + "Please refer to this site https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/stacksets-orgs-activate-trusted-access.html and "
+                + "follow the instructions to activate trusted access with AWS Organizations."
+            )
+        raise err
 
     await boto_crud_call(
         client.create_stack_instances,
         StackSetName=stack_set_name,
         DeploymentTargets=deployment_targets,
         Regions=deployment_regions,
         OperationPreferences=operation_preferences,
@@ -469,14 +483,15 @@
                 "ParameterValue": spoke_role_name,
             },
             {"ParameterKey": "AssumeAsArn", "ParameterValue": assume_as_arn},
         ],
         Capabilities=["CAPABILITY_NAMED_IAM"],
         **additional_kwargs,
     )
+
     if stack_created:
         return await create_spoke_role_stack(
             cf_client,
             hub_account_id,
             role_arn,
             read_only=read_only,
             stack_name=spoke_role_name,
```

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,18 @@
         description="The name of the policy.",
     )
     version: Optional[str]
     statement: Optional[Union[List[PolicyStatement], PolicyStatement]] = Field(
         None,
         description="List of policy statements",
     )
+    id: Optional[str] = Field(
+        None,
+        description="The Id element specifies an optional identifier for the policy. The ID is used differently in different services.",
+    )
 
     @property
     def resource_type(self):
         return "aws:policy_document"
 
     @property
     def resource_id(self):
```

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,23 +422,34 @@
 
     file_path = get_templated_role_file_path(
         role_dir,
         role_name,
         role_template_params.get("included_accounts"),
         role_path=path,
     )
-    return create_or_update_template(
-        file_path,
-        existing_template_map,
-        role_name,
-        AwsIamRoleTemplate,
-        role_template_params,
-        RoleProperties(**role_template_properties),
-        list(aws_account_map.values()),
-    )
+    try:
+        return create_or_update_template(
+            file_path,
+            existing_template_map,
+            role_name,
+            AwsIamRoleTemplate,
+            role_template_params,
+            RoleProperties(**role_template_properties),
+            list(aws_account_map.values()),
+        )
+    except Exception as e:
+        log_params = {
+            "role_name": role_name,
+            "role_template_params": role_template_params,
+        }
+        log.error(
+            "Not able to create_or_update_template",
+            **log_params,
+        )
+        raise e
 
 
 async def collect_aws_roles(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     iam_template_map: dict,
     detect_messages: list[RoleMessageDetails] = None,
```

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,14 +400,18 @@
             self.identity_center_details.identity_store_id = identity_center_instances[
                 "Instances"
             ][0]["IdentityStoreId"]
 
             if not set_identity_center_map:
                 return
 
+            self.identity_center_details.permission_set_map = {}
+            self.identity_center_details.user_map = {}
+            self.identity_center_details.group_map = {}
+
             permission_set_arns = await legacy_paginated_search(
                 identity_center_client.list_permission_sets,
                 response_key="PermissionSets",
                 InstanceArn=self.identity_center_details.instance_arn,
             )
             if permission_set_arns:
                 # WARNING
```

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/organizations/scp/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.9.6/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/request_handler/expire_resources.py` & `iambic_core-0.9.6/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/request_handler/git_apply.py` & `iambic_core-0.9.6/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/request_handler/git_plan.py` & `iambic_core-0.9.6/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.9.6/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.9.1/pyproject.toml` & `iambic_core-0.9.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.9.1"
+version = "0.9.6"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
```

### Comparing `iambic_core-0.9.1/PKG-INFO` & `iambic_core-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.9.1
+Version: 0.9.6
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -69,15 +69,15 @@
 - **[Dynamic AWS Permissions](https://docs.iambic.org/getting_started/aws#31---create-dynamic-iam-role-policies-that-vary-per-account)**: Simplify multi-account AWS management with flexible templates, allowing multi-account roles to have different permissions and access rules on different accounts.
 - **[Drift Prevention](https://docs.iambic.org/how_to_guides/prevent-drift)**: Protect the IAM resources you want to be exclusively managed via IAMbic. What is in Git becomes the absolute source of truth.
 - **[GitOps-driven Cloud IAM (IAMOps)](https://docs.iambic.org/reference/iamops_philosophy)**: Leverage GitOps-driven Cloud IAM with human-readable formats and your favorite tools.
 - **Centralized Management**: IAMbic keeps Git updated with the latest, complete state of your cloud environment, maintaining a single source of truth for auditing and compliance across multiple cloud providers in Git.
 - **Extendable**: Integrate with various clouds and applications through a powerful plugin architecture.
 - **Auditable**: Track changes to IAM policies, permissions, and rules with Git history. For AWS, IAmbic annotates out-of-band commits with details from CloudTrail.
 
-Check out [IAMbic IAMOps Philosophy](/reference/iamops_philosophy) and an [example IAMbic templates repository](https://github.com/noqdev/iambic-templates-examples) to see a real-life example of IAMbic.
+Check out [IAMbic IAMOps Philosophy](https://docs.iambic.org/reference/iamops_philosophy) and an [example IAMbic templates repository](https://github.com/noqdev/iambic-templates-examples) to see a real-life example of IAMbic.
 
 ## 📣 Let's chat
 
 Do you want to connect with our contributors?
 
 Just click the button below and follow the instructions.
```

