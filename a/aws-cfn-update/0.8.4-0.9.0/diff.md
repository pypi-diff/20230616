# Comparing `tmp/aws-cfn-update-0.8.4.tar.gz` & `tmp/aws-cfn-update-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cfn-update-0.8.4.tar", last modified: Wed May 17 12:01:09 2023, max compression
+gzip compressed data, was "aws-cfn-update-0.9.0.tar", last modified: Fri Jun 16 14:27:35 2023, max compression
```

## Comparing `aws-cfn-update-0.8.4.tar` & `aws-cfn-update-0.9.0.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.195872 aws-cfn-update-0.8.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.github/workflows/release-image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/aws-cfn-update.iml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/cfnlintPlugin.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.make-release-support
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.release
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Makefile.mk
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    75718 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.195872 aws-cfn-update-0.8.4/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/samples/add-new-resources/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/storage-server-new.json
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/storage-server-new.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/storage-server.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/storage-server.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/samples/config-rule-inline-code/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/config-rule-inline-code/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/config-rule-inline-code/dynamodb-pitr-enabled.guard
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/config-rule-inline-code/template.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/config-rule-inline-code/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/samples/container-image/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/container-image/paas-monitor.json
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/container-image/paas-monitor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/samples/cron-schedule-expression/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/cron-schedule-expression/cron.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/lambda-inline-code/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/lambda-inline-code/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn-listener-rule-provider.json
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn-listener-rule-provider.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn_listener_rule_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/latest-ami-update/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/latest-ami-update/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/latest-ami-update/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/oidc-provider/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/oidc-provider/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/oidc-provider/oidc-provider.json
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/oidc-provider/oidc-provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/packer-latest-ami/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/packer-latest-ami/packer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/remove-resource/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/remove-resource/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/remove-resource/storage-server.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/remove-resource/storage-server.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/rest-api-body/
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/rest-api-body/api-specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/rest-api-body/aws-extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/rest-api-body/rest-api.json
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/rest-api-body/rest-api.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/state-machine-definition/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/state-machine-definition/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/state-machine-definition/definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/state-machine-definition/definition.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/state-machine-definition/helloworld.json
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-17 12:01:09.211872 aws-cfn-update-0.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.195872 aws-cfn-update-0.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/src/aws_cfn_update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/add_missing_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/add_new_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/cfn_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/config_rule_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/container_image_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/cron_schedule_expression_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/lambda_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/latest_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/oidc_provider_thumbprints_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/packer_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/remove_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/replace_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/rest_api_body_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/statemachine_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:00:23.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/api-specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/aws-extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   204302 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/dummy_responses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_add_new_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_config_rule_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_cron_schedule_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_lambda_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_latest_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_oidc_provider_thumbprint_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_packer_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_remove_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_replace_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_rest_api_body_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_statemachine_definition_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/tests/update_packer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/update_packer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/update_packer/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/tests/update_packer/call_00001_describe_images/
--rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/update_packer/call_00001_describe_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/update_packer/test_update_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.041580 aws-cfn-update-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.021579 aws-cfn-update-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.025579 aws-cfn-update-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.github/workflows/release-image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.029579 aws-cfn-update-0.9.0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.idea/aws-cfn-update.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.idea/cfnlintPlugin.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.029579 aws-cfn-update-0.9.0/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.029579 aws-cfn-update-0.9.0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.make-release-support
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/.release
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/Makefile.mk
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-16 14:27:35.041580 aws-cfn-update-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    76080 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.025579 aws-cfn-update-0.9.0/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.029579 aws-cfn-update-0.9.0/samples/add-new-resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/add-new-resources/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/add-new-resources/storage-server-new.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/add-new-resources/storage-server-new.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/add-new-resources/storage-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/add-new-resources/storage-server.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.029579 aws-cfn-update-0.9.0/samples/config-rule-inline-code/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/config-rule-inline-code/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/config-rule-inline-code/dynamodb-pitr-enabled.guard
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/config-rule-inline-code/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/config-rule-inline-code/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.029579 aws-cfn-update-0.9.0/samples/container-image/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/container-image/paas-monitor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/container-image/paas-monitor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.029579 aws-cfn-update-0.9.0/samples/cron-schedule-expression/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/cron-schedule-expression/cron.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.029579 aws-cfn-update-0.9.0/samples/lambda-inline-code/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/lambda-inline-code/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/lambda-inline-code/cfn-listener-rule-provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/lambda-inline-code/cfn-listener-rule-provider.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/lambda-inline-code/cfn_listener_rule_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.029579 aws-cfn-update-0.9.0/samples/latest-ami-update/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/latest-ami-update/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/latest-ami-update/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.033580 aws-cfn-update-0.9.0/samples/oidc-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/oidc-provider/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/oidc-provider/oidc-provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/oidc-provider/oidc-provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.033580 aws-cfn-update-0.9.0/samples/packer-latest-ami/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/packer-latest-ami/packer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.033580 aws-cfn-update-0.9.0/samples/remove-resource/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/remove-resource/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/remove-resource/storage-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/remove-resource/storage-server.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.033580 aws-cfn-update-0.9.0/samples/rest-api-body/
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/rest-api-body/api-specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/rest-api-body/aws-extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/rest-api-body/rest-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/rest-api-body/rest-api.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.033580 aws-cfn-update-0.9.0/samples/state-machine-definition/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/state-machine-definition/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/state-machine-definition/definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/state-machine-definition/definition.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/samples/state-machine-definition/helloworld.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-16 14:27:35.041580 aws-cfn-update-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.025579 aws-cfn-update-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.037580 aws-cfn-update-0.9.0/src/aws_cfn_update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/add_missing_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/add_new_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/cfn_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/config_rule_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/container_image_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/cron_schedule_expression_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/lambda_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/latest_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/oidc_provider_thumbprints_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/packer_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/remove_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/replace_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/rest_api_body_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/src/aws_cfn_update/statemachine_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.037580 aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-16 14:27:34.000000 aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-16 14:27:34.000000 aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:27:34.000000 aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-16 14:27:34.000000 aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 14:27:34.000000 aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 14:27:34.000000 aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:26:45.000000 aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.037580 aws-cfn-update-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/api-specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/aws-extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   204302 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/dummy_responses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_add_new_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_config_rule_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_cron_schedule_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_lambda_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_latest_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_oidc_provider_thumbprint_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_packer_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_preserve_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_remove_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_replace_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_rest_api_body_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/test_statemachine_definition_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.037580 aws-cfn-update-0.9.0/tests/update_packer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/update_packer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/update_packer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:27:35.041580 aws-cfn-update-0.9.0/tests/update_packer/call_00001_describe_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/update_packer/call_00001_describe_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tests/update_packer/test_update_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 14:26:18.000000 aws-cfn-update-0.9.0/tox.ini
```

### Comparing `aws-cfn-update-0.8.4/.github/workflows/release-image.yaml` & `aws-cfn-update-0.9.0/.github/workflows/release-image.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/.github/workflows/release.yml` & `aws-cfn-update-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/.idea/aws-cfn-update.iml` & `aws-cfn-update-0.9.0/.idea/aws-cfn-update.iml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/.idea/codeStyles/Project.xml` & `aws-cfn-update-0.9.0/.idea/codeStyles/Project.xml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/.idea/inspectionProfiles/Project_Default.xml` & `aws-cfn-update-0.9.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/.make-release-support` & `aws-cfn-update-0.9.0/.make-release-support`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/LICENSE` & `aws-cfn-update-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/Makefile.mk` & `aws-cfn-update-0.9.0/Makefile.mk`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/PKG-INFO` & `aws-cfn-update-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cfn-update
-Version: 0.8.4
+Version: 0.9.0
 Summary: Programmatically update CloudFormation templates
 Home-page: https://github.com/binxio/aws-cfn-update
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-cfn-update-0.8.4/Pipfile.lock` & `aws-cfn-update-0.9.0/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9842159410872862%*

 * *Differences: {"'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:cf1067d101be538f399b685bbe6beb4bfed01095da8497d0c7fa8b8788a65c6b', "*

 * *              "'sha256:ee2b3733f40f935da78bf76bc8e82af6e90841406e04605e3b2d765b50cad05e'], "*

 * *              "'version': '==1.26.154'}, 'botocore': {'hashes': "*

 * *              "['sha256:a9c7da497ac5f7d4f3e932b4442e7c32cc2936f3a4658165f1528336fc429c3d', "*

 * *              "'sha256:b9853f72a3c93f1aa8c9a1636911cdbec3662bca2e04e4ee00437c4f8c9fa2d4'], "*

 * *              "'version': '==1.29.15 […]*

```diff
@@ -26,27 +26,27 @@
         },
         "aws-cfn-update": {
             "editable": true,
             "path": "."
         },
         "boto3": {
             "hashes": [
-                "sha256:23523d5d6aa51bba2461d67f6eb458d83b6a52d18e3d953b1ce71209b66462ec",
-                "sha256:ba7ca9215a1026620741273da10d0d3cceb9f7649f7c101e616a287071826f9d"
+                "sha256:cf1067d101be538f399b685bbe6beb4bfed01095da8497d0c7fa8b8788a65c6b",
+                "sha256:ee2b3733f40f935da78bf76bc8e82af6e90841406e04605e3b2d765b50cad05e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.135"
+            "version": "==1.26.154"
         },
         "botocore": {
             "hashes": [
-                "sha256:06502a4473924ef60ac0de908385a5afab9caee6c5b49cf6a330fab0d76ddf5f",
-                "sha256:0c61d4e5e04fe5329fa65da6b31492ef9d0d5174d72fc2af69de2ed0f87804ca"
+                "sha256:a9c7da497ac5f7d4f3e932b4442e7c32cc2936f3a4658165f1528336fc429c3d",
+                "sha256:b9853f72a3c93f1aa8c9a1636911cdbec3662bca2e04e4ee00437c4f8c9fa2d4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.135"
+            "version": "==1.29.154"
         },
         "certifi": {
             "hashes": [
                 "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
                 "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
@@ -215,44 +215,44 @@
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.1.3"
         },
         "croniter": {
             "hashes": [
-                "sha256:d067b1f95b553c6e82d95a983c465695913dcd12f47a8b9aa938a0450d94dd5e",
-                "sha256:da1a1a7ca977b38e952ab0a119576e002bc4c05d058d644e81fc06ef7e995bb0"
+                "sha256:1a6df60eacec3b7a0aa52a8f2ef251ae3dd2a7c7c8b9874e73e791636d55a361",
+                "sha256:9595da48af37ea06ec3a9f899738f1b2c1c13da3c38cea606ef7cd03ea421128"
             ],
             "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.3.14"
+            "version": "==1.4.1"
         },
         "cryptography": {
             "hashes": [
-                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
-                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
-                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
-                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
-                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
-                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
-                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
-                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
-                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
-                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
-                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
-                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
-                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
-                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
-                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
-                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
-                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
-                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
-                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==40.0.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.1"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -379,33 +379,34 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "requests": {
             "hashes": [
-                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
-                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.30.0"
+            "version": "==2.31.0"
         },
         "ruamel.yaml": {
             "hashes": [
-                "sha256:25d0ee82a0a9a6f44683dcf8c282340def4074a4562f3a24f55695bb254c1693",
-                "sha256:baa2d0a5aad2034826c439ce61c142c07082b76f4791d54145e131206e998059"
+                "sha256:098ed1eb6d338a684891a72380277c1e6fc4d4ae0e120de9a447275056dda335",
+                "sha256:3cf153f0047ced526e723097ac615d3009371779432e304dbd5596b6f3a4c777"
             ],
             "markers": "python_version >= '3'",
-            "version": "==0.17.26"
+            "version": "==0.17.31"
         },
         "ruamel.yaml.clib": {
             "hashes": [
                 "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
                 "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
                 "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
+                "sha256:1a6391a7cabb7641c32517539ca42cf84b87b667bad38b78d4d42dd23e957c81",
                 "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
                 "sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f",
                 "sha256:3110a99e0f94a4a3470ff67fc20d3f96c25b13d24c6980ff841e82bafe827cac",
                 "sha256:3243f48ecd450eddadc2d11b5feb08aca941b5cd98c9b1db14b2fd128be8c697",
                 "sha256:370445fd795706fd291ab00c9df38a0caed0f17a6fb46b0f607668ecb16ce763",
                 "sha256:40d030e2329ce5286d6b231b8726959ebbe0404c92f0a578c0e2482182e38282",
                 "sha256:41d0f1fa4c6830176eef5b276af04c89320ea616655d01327d5ce65e50575c94",
@@ -415,14 +416,15 @@
                 "sha256:721bc4ba4525f53f6a611ec0967bdcee61b31df5a56801281027a3a6d1c2daf5",
                 "sha256:763d65baa3b952479c4e972669f679fe490eee058d5aa85da483ebae2009d231",
                 "sha256:7bdb4c06b063f6fd55e472e201317a3bb6cdeeee5d5a38512ea5c01e1acbdd93",
                 "sha256:8831a2cedcd0f0927f788c5bdf6567d9dc9cc235646a434986a852af1cb54b4b",
                 "sha256:91a789b4aa0097b78c93e3dc4b40040ba55bef518f84a40d4442f713b4094acb",
                 "sha256:92460ce908546ab69770b2e576e4f99fbb4ce6ab4b245345a3869a0a0410488f",
                 "sha256:99e77daab5d13a48a4054803d052ff40780278240a902b880dd37a51ba01a307",
+                "sha256:9c7617df90c1365638916b98cdd9be833d31d337dbcd722485597b43c4a215bf",
                 "sha256:a234a20ae07e8469da311e182e70ef6b199d0fbeb6c6cc2901204dd87fb867e8",
                 "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
                 "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
                 "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
                 "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
                 "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
                 "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
@@ -461,19 +463,19 @@
                 "sha256:f3596e180296aaf2dbd97d124fe76ae3a0e3d32b258447de7b939b3fd4be992f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.0.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:8d36afa7616d8ab714608411b4a3b13e58f463aee519024578e062e141dce20f",
+                "sha256:8f135f6502756bde6b2a9b28989df5fbe87c9970cecaa69041edcce7f0589b14"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "version": "==1.26.16"
         }
     },
     "develop": {
         "attrs": {
             "hashes": [
                 "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04",
                 "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"
@@ -491,43 +493,43 @@
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:23523d5d6aa51bba2461d67f6eb458d83b6a52d18e3d953b1ce71209b66462ec",
-                "sha256:ba7ca9215a1026620741273da10d0d3cceb9f7649f7c101e616a287071826f9d"
+                "sha256:cf1067d101be538f399b685bbe6beb4bfed01095da8497d0c7fa8b8788a65c6b",
+                "sha256:ee2b3733f40f935da78bf76bc8e82af6e90841406e04605e3b2d765b50cad05e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.135"
+            "version": "==1.26.154"
         },
         "botocore": {
             "hashes": [
-                "sha256:06502a4473924ef60ac0de908385a5afab9caee6c5b49cf6a330fab0d76ddf5f",
-                "sha256:0c61d4e5e04fe5329fa65da6b31492ef9d0d5174d72fc2af69de2ed0f87804ca"
+                "sha256:a9c7da497ac5f7d4f3e932b4442e7c32cc2936f3a4658165f1528336fc429c3d",
+                "sha256:b9853f72a3c93f1aa8c9a1636911cdbec3662bca2e04e4ee00437c4f8c9fa2d4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.135"
+            "version": "==1.29.154"
         },
         "build": {
             "hashes": [
                 "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171",
                 "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"
             ],
             "index": "pypi",
             "version": "==0.10.0"
         },
         "cachetools": {
             "hashes": [
-                "sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14",
-                "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
+                "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590",
+                "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
             ],
-            "markers": "python_version ~= '3.7'",
-            "version": "==5.3.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
                 "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
                 "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
@@ -712,44 +714,44 @@
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==0.4.6"
         },
         "croniter": {
             "hashes": [
-                "sha256:d067b1f95b553c6e82d95a983c465695913dcd12f47a8b9aa938a0450d94dd5e",
-                "sha256:da1a1a7ca977b38e952ab0a119576e002bc4c05d058d644e81fc06ef7e995bb0"
+                "sha256:1a6df60eacec3b7a0aa52a8f2ef251ae3dd2a7c7c8b9874e73e791636d55a361",
+                "sha256:9595da48af37ea06ec3a9f899738f1b2c1c13da3c38cea606ef7cd03ea421128"
             ],
             "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.3.14"
+            "version": "==1.4.1"
         },
         "cryptography": {
             "hashes": [
-                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
-                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
-                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
-                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
-                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
-                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
-                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
-                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
-                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
-                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
-                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
-                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
-                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
-                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
-                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
-                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
-                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
-                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
-                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==40.0.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.1"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -768,19 +770,19 @@
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
-                "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.12.0"
+            "version": "==3.12.2"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -838,19 +840,19 @@
                 "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.13.1"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
-                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
@@ -878,19 +880,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
-                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
+                "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed",
+                "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.1"
+            "version": "==3.5.3"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -909,19 +911,19 @@
                 "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.15.1"
         },
         "pyproject-api": {
             "hashes": [
-                "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
-                "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
+                "sha256:999f58fa3c92b23ebd31a6bad5d1f87d456744d75e05391be7f5c729015d3d91",
+                "sha256:9cffcbfb64190f207444d7579d315f3278f2c04ba46d685fad93197b5326d348"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.5.1"
+            "version": "==1.5.2"
         },
         "pyproject-hooks": {
             "hashes": [
                 "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8",
                 "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
             ],
             "markers": "python_version >= '3.7'",
@@ -958,19 +960,19 @@
                 "sha256:f0e7c4b2f77593871e918be000b96c8107da48444d57005b6a6bc61fb4331b2c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.19.3"
         },
         "pytest": {
             "hashes": [
-                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
-                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
+                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
+                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
             ],
             "index": "pypi",
-            "version": "==7.3.1"
+            "version": "==7.3.2"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1035,19 +1037,19 @@
                 "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==37.3"
         },
         "requests": {
             "hashes": [
-                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
-                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.30.0"
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
                 "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
                 "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1059,33 +1061,34 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
-                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.5"
+            "version": "==13.4.2"
         },
         "ruamel.yaml": {
             "hashes": [
-                "sha256:25d0ee82a0a9a6f44683dcf8c282340def4074a4562f3a24f55695bb254c1693",
-                "sha256:baa2d0a5aad2034826c439ce61c142c07082b76f4791d54145e131206e998059"
+                "sha256:098ed1eb6d338a684891a72380277c1e6fc4d4ae0e120de9a447275056dda335",
+                "sha256:3cf153f0047ced526e723097ac615d3009371779432e304dbd5596b6f3a4c777"
             ],
             "markers": "python_version >= '3'",
-            "version": "==0.17.26"
+            "version": "==0.17.31"
         },
         "ruamel.yaml.clib": {
             "hashes": [
                 "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
                 "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
                 "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
+                "sha256:1a6391a7cabb7641c32517539ca42cf84b87b667bad38b78d4d42dd23e957c81",
                 "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
                 "sha256:2aa261c29a5545adfef9296b7e33941f46aa5bbd21164228e833412af4c9c75f",
                 "sha256:3110a99e0f94a4a3470ff67fc20d3f96c25b13d24c6980ff841e82bafe827cac",
                 "sha256:3243f48ecd450eddadc2d11b5feb08aca941b5cd98c9b1db14b2fd128be8c697",
                 "sha256:370445fd795706fd291ab00c9df38a0caed0f17a6fb46b0f607668ecb16ce763",
                 "sha256:40d030e2329ce5286d6b231b8726959ebbe0404c92f0a578c0e2482182e38282",
                 "sha256:41d0f1fa4c6830176eef5b276af04c89320ea616655d01327d5ce65e50575c94",
@@ -1095,14 +1098,15 @@
                 "sha256:721bc4ba4525f53f6a611ec0967bdcee61b31df5a56801281027a3a6d1c2daf5",
                 "sha256:763d65baa3b952479c4e972669f679fe490eee058d5aa85da483ebae2009d231",
                 "sha256:7bdb4c06b063f6fd55e472e201317a3bb6cdeeee5d5a38512ea5c01e1acbdd93",
                 "sha256:8831a2cedcd0f0927f788c5bdf6567d9dc9cc235646a434986a852af1cb54b4b",
                 "sha256:91a789b4aa0097b78c93e3dc4b40040ba55bef518f84a40d4442f713b4094acb",
                 "sha256:92460ce908546ab69770b2e576e4f99fbb4ce6ab4b245345a3869a0a0410488f",
                 "sha256:99e77daab5d13a48a4054803d052ff40780278240a902b880dd37a51ba01a307",
+                "sha256:9c7617df90c1365638916b98cdd9be833d31d337dbcd722485597b43c4a215bf",
                 "sha256:a234a20ae07e8469da311e182e70ef6b199d0fbeb6c6cc2901204dd87fb867e8",
                 "sha256:a7b301ff08055d73223058b5c46c55638917f04d21577c95e00e0c4d79201a6b",
                 "sha256:be2a7ad8fd8f7442b24323d24ba0b56c51219513cfa45b9ada3b87b76c374d4b",
                 "sha256:bf9a6bc4a0221538b1a7de3ed7bca4c93c02346853f44e1cd764be0023cd3640",
                 "sha256:c3ca1fbba4ae962521e5eb66d72998b51f0f4d0f608d3c0347a48e1af262efa7",
                 "sha256:d000f258cf42fec2b1bbf2863c61d7b8918d31ffee905da62dede869254d3b8a",
                 "sha256:d5859983f26d8cd7bb5c287ef452e8aacc86501487634573d260968f753e1d71",
@@ -1125,19 +1129,19 @@
                 "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
-                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
+                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
+                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.7.2"
+            "version": "==67.8.0"
         },
         "setuptools-scm": {
             "hashes": [
                 "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
                 "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"
             ],
             "index": "pypi",
@@ -1157,51 +1161,51 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tox": {
             "hashes": [
-                "sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56",
-                "sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046"
+                "sha256:b45c4927bd1b3d91d532fbae9d7ffb676ff2b4d2ae26ef93b41b3189d1eff860",
+                "sha256:bf71ff8ee08499d4a3db6b73e35ef8d0e4346a3bea84517245b1e4a09b9f0774"
             ],
             "index": "pypi",
-            "version": "==4.5.1"
+            "version": "==4.6.1"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
-                "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.5.0"
+            "version": "==4.6.3"
         },
         "tzlocal": {
             "hashes": [
                 "sha256:46eb99ad4bdb71f3f72b7d24f4267753e240944ecfc16f25d2719ba89827a803",
                 "sha256:f3596e180296aaf2dbd97d124fe76ae3a0e3d32b258447de7b939b3fd4be992f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.0.1"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:8d36afa7616d8ab714608411b4a3b13e58f463aee519024578e062e141dce20f",
+                "sha256:8f135f6502756bde6b2a9b28989df5fbe87c9970cecaa69041edcce7f0589b14"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "version": "==1.26.16"
         },
         "virtualenv": {
             "hashes": [
                 "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
                 "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `aws-cfn-update-0.8.4/README.md` & `aws-cfn-update-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/add-new-resources/storage-server-new.json` & `aws-cfn-update-0.9.0/samples/add-new-resources/storage-server-new.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/add-new-resources/storage-server-new.yaml` & `aws-cfn-update-0.9.0/samples/add-new-resources/storage-server-new.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/add-new-resources/storage-server.json` & `aws-cfn-update-0.9.0/samples/add-new-resources/storage-server.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/add-new-resources/storage-server.yaml` & `aws-cfn-update-0.9.0/samples/add-new-resources/storage-server.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/container-image/paas-monitor.json` & `aws-cfn-update-0.9.0/samples/container-image/paas-monitor.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn-listener-rule-provider.json` & `aws-cfn-update-0.9.0/samples/lambda-inline-code/cfn-listener-rule-provider.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn-listener-rule-provider.yaml` & `aws-cfn-update-0.9.0/samples/lambda-inline-code/cfn-listener-rule-provider.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn_listener_rule_provider.py` & `aws-cfn-update-0.9.0/samples/lambda-inline-code/cfn_listener_rule_provider.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/latest-ami-update/template.yaml` & `aws-cfn-update-0.9.0/samples/latest-ami-update/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/packer-latest-ami/packer.json` & `aws-cfn-update-0.9.0/samples/packer-latest-ami/packer.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/remove-resource/storage-server.json` & `aws-cfn-update-0.9.0/samples/remove-resource/storage-server.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/remove-resource/storage-server.yaml` & `aws-cfn-update-0.9.0/samples/remove-resource/storage-server.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/rest-api-body/api-specification.yaml` & `aws-cfn-update-0.9.0/samples/rest-api-body/api-specification.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/rest-api-body/aws-extensions.yaml` & `aws-cfn-update-0.9.0/samples/rest-api-body/aws-extensions.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/rest-api-body/rest-api.json` & `aws-cfn-update-0.9.0/samples/rest-api-body/rest-api.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/state-machine-definition/definition.json` & `aws-cfn-update-0.9.0/samples/state-machine-definition/definition.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/samples/state-machine-definition/definition.yaml` & `aws-cfn-update-0.9.0/samples/state-machine-definition/definition.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/setup.cfg` & `aws-cfn-update-0.9.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aws-cfn-update
-version = 0.8.4
+version = 0.9.0
 author = Mark van Holsteijn
 url = https://github.com/binxio/aws-cfn-update
 author_email = mark.vanholsteijn@xebia.com
 description = Programmatically update CloudFormation templates
 long_description = file: README.md
 long_description_content_type = text/markdown
 test_suite = tests
@@ -29,15 +29,15 @@
 install_requires = 
 	click
 	boto3
 	cfn-flip
 	pytz
 	croniter
 	tzlocal
-	ruamel.yaml
+	ruamel.yaml>=0.17.0
 	requests
 	jsonmerge
 	cryptography
 use_scm_version = True
 
 [options.entry_points]
 console_scripts =
```

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/add_new_resources.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/add_new_resources.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/cfn_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/cfn_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/cli.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/cli.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/config_rule_inline_code_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/config_rule_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/container_image_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/container_image_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/cron_schedule_expression_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/cron_schedule_expression_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/lambda_inline_code_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/lambda_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/latest_ami_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/latest_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/oidc_provider_thumbprints_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/oidc_provider_thumbprints_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/packer_ami_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/packer_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/remove_resource.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/remove_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,22 +43,22 @@
             map(lambda n: n.split(".")[0], re.findall(r"\${([^!][^}]*)}", sub)),
         )
     )
 
 
 def is_tag_reference(obj, name):
     if isinstance(obj, TaggedScalar):
-        if obj.tag.value == "!Ref":
+        if obj.tag.suffix == "Ref":
             return str(obj.value) == name
-        elif obj.tag.value == "!Sub":
+        elif obj.tag.suffix == "Sub":
             return references_in_sub(obj.value, name)
-        elif obj.tag.value == "!GetAtt":
+        elif obj.tag.suffix == "GetAtt":
             return str(obj.value).split(".")[0] == name
     elif isinstance(obj, CommentedSeq):
-        if obj.tag.value == "!GetAtt":
+        if obj.tag.suffix == "GetAtt":
             return len(obj) > 1 and obj[0] == name
     return False
 
 
 def remove_resource_from_template(template: dict, name: str):
     resources: dict = template.get("Resources")
     if resources and name in resources:
```

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/replace_references.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/replace_references.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         for name, value in template.items():
             if name == "Ref" and value == old_reference:
                 template["Ref"] = new_reference
                 result = True
             elif (
                 isinstance(value, TaggedScalar)
                 and value.tag
-                and value.tag.value == "!Ref"
+                and value.tag.suffix == "Ref"
                 and value.value == old_reference
             ):
                 value.value = new_reference
                 result = True
             else:
                 result = (
                     replace_references(template[name], old_reference, new_reference)
```

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/rest_api_body_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/rest_api_body_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update/statemachine_updater.py` & `aws-cfn-update-0.9.0/src/aws_cfn_update/statemachine_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/PKG-INFO` & `aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cfn-update
-Version: 0.8.4
+Version: 0.9.0
 Summary: Programmatically update CloudFormation templates
 Home-page: https://github.com/binxio/aws-cfn-update
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/SOURCES.txt` & `aws-cfn-update-0.9.0/src/aws_cfn_update.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 tests/test_add_new_resources.py
 tests/test_config_rule_inline_code_updater.py
 tests/test_cron_schedule_expression.py
 tests/test_lambda_inline_code_updater.py
 tests/test_latest_ami_updater.py
 tests/test_oidc_provider_thumbprint_updater.py
 tests/test_packer_ami_updater.py
+tests/test_preserve_spaces.py
 tests/test_remove_resources.py
 tests/test_replace_references.py
 tests/test_rest_api_body_updater.py
 tests/test_statemachine_definition_updater.py
 tests/update_packer/__init__.py
 tests/update_packer/base.py
 tests/update_packer/test_update_packer.py
```

### Comparing `aws-cfn-update-0.8.4/tests/api-specification.yaml` & `aws-cfn-update-0.9.0/tests/api-specification.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/aws-extensions.yaml` & `aws-cfn-update-0.9.0/tests/aws-extensions.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/dummy_responses.json` & `aws-cfn-update-0.9.0/tests/dummy_responses.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_add_new_resources.py` & `aws-cfn-update-0.9.0/tests/test_add_new_resources.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_config_rule_inline_code_updater.py` & `aws-cfn-update-0.9.0/tests/test_config_rule_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_cron_schedule_expression.py` & `aws-cfn-update-0.9.0/tests/test_cron_schedule_expression.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_lambda_inline_code_updater.py` & `aws-cfn-update-0.9.0/tests/test_lambda_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_latest_ami_updater.py` & `aws-cfn-update-0.9.0/tests/test_latest_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_oidc_provider_thumbprint_updater.py` & `aws-cfn-update-0.9.0/tests/test_oidc_provider_thumbprint_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_packer_ami_updater.py` & `aws-cfn-update-0.9.0/tests/test_packer_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_remove_resources.py` & `aws-cfn-update-0.9.0/tests/test_remove_resources.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_replace_references.py` & `aws-cfn-update-0.9.0/tests/test_replace_references.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_rest_api_body_updater.py` & `aws-cfn-update-0.9.0/tests/test_rest_api_body_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/test_statemachine_definition_updater.py` & `aws-cfn-update-0.9.0/tests/test_statemachine_definition_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/update_packer/base.py` & `aws-cfn-update-0.9.0/tests/update_packer/base.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/update_packer/call_00001_describe_images/__init__.py` & `aws-cfn-update-0.9.0/tests/update_packer/call_00001_describe_images/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.4/tests/update_packer/test_update_packer.py` & `aws-cfn-update-0.9.0/tests/update_packer/test_update_packer.py`

 * *Files identical despite different names*

