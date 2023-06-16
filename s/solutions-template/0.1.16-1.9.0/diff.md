# Comparing `tmp/solutions_template-0.1.16.tar.gz` & `tmp/solutions_template-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solutions_template-0.1.16.tar", max compression
+gzip compressed data, was "solutions_template-1.9.0.tar", max compression
```

## Comparing `solutions_template-0.1.16.tar` & `solutions_template-1.9.0.tar`

### file list

```diff
@@ -1,145 +1,146 @@
--rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_template-0.1.16/LICENSE
--rw-r--r--   0        0        0     4962 2023-06-07 19:17:21.305770 solutions_template-0.1.16/README.md
--rw-r--r--   0        0        0     1106 2023-06-14 05:05:11.332654 solutions_template-0.1.16/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 06:03:26.151656 solutions_template-0.1.16/solutions_template/__init__.py
--rw-r--r--   0        0        0     5169 2023-06-12 21:16:11.127992 solutions_template-0.1.16/solutions_template/cli/cli.py
--rw-r--r--   0        0        0     4199 2023-06-12 05:31:02.386771 solutions_template-0.1.16/solutions_template/cli/cli_utils.py
--rw-r--r--   0        0        0     5625 2023-06-12 19:16:45.957991 solutions_template-0.1.16/solutions_template/cli/component.py
--rw-r--r--   0        0        0     5883 2023-06-13 00:44:03.256194 solutions_template-0.1.16/solutions_template/cli/infra.py
--rw-r--r--   0        0        0     1072 2023-05-31 02:43:23.246104 solutions_template-0.1.16/solutions_template/cli/tool.py
--rw-r--r--   0        0        0        0 2023-05-30 05:26:14.220349 solutions_template-0.1.16/solutions_template/copier_extensions/__init__.py
--rw-r--r--   0        0        0     3561 2023-06-13 00:43:13.430765 solutions_template-0.1.16/solutions_template/copier_extensions/st_helpers.py
--rw-r--r--   0        0        0       80 2023-06-12 14:27:39.500453 solutions_template-0.1.16/solutions_template/modules/restful_service/.st/module_answers/{{component_name}}.yaml
--rw-r--r--   0        0        0      545 2023-05-25 05:42:40.959522 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/Dockerfile
--rw-r--r--   0        0        0     1258 2023-05-30 02:23:58.120959 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/README.md
--rw-r--r--   0        0        0      215 2023-05-28 08:06:57.402697 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
--rw-r--r--   0        0        0       77 2023-05-21 21:45:15.984417 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/requirements-test.txt
--rw-r--r--   0        0        0      109 2023-05-22 02:59:24.183865 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/requirements.txt
--rw-r--r--   0        0        0     3154 2023-05-25 06:15:31.353814 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/skaffold.yaml
--rw-r--r--   0        0        0      863 2023-05-30 02:57:45.839642 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/config.py
--rw-r--r--   0        0        0     1871 2023-05-30 02:57:45.896289 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/main.py
--rw-r--r--   0        0        0     1504 2023-05-30 02:57:45.872700 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
--rw-r--r--   0        0        0        0 2023-05-21 21:45:15.986832 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
--rw-r--r--   0        0        0     3780 2023-06-12 20:02:08.800090 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
--rw-r--r--   0        0        0        0 2023-05-21 21:45:15.989918 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
--rw-r--r--   0        0        0       81 2023-05-24 17:31:37.550531 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/st_module.yaml
--rw-r--r--   0        0        0     1191 2023-05-25 06:14:24.382461 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
--rw-r--r--   0        0        0      197 2023-05-25 05:22:13.230283 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
--rw-r--r--   0        0        0       60 2023-05-25 05:23:40.037322 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
--rw-r--r--   0        0        0      229 2023-05-25 05:56:07.486203 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
--rw-r--r--   0        0        0      421 2023-05-25 05:22:10.057932 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
--rw-r--r--   0        0        0      103 2023-05-21 21:45:15.984125 solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
--rw-r--r--   0        0        0     2255 2023-06-12 17:38:25.956053 solutions_template-0.1.16/solutions_template/modules/restful_service/copier.yaml
--rw-r--r--   0        0        0       92 2023-05-23 03:08:54.329834 solutions_template-0.1.16/solutions_template/modules/restful_service/skaffold.yaml.patch
--rw-r--r--   0        0        0      263 2023-05-28 06:13:12.606449 solutions_template-0.1.16/solutions_template/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
--rw-r--r--   0        0        0     3461 2023-06-12 21:02:10.127155 solutions_template-0.1.16/solutions_template/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
--rw-r--r--   0        0        0     3269 2023-06-01 22:02:03.561803 solutions_template-0.1.16/solutions_template/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
--rw-r--r--   0        0        0      792 2023-05-25 04:45:34.188865 solutions_template-0.1.16/solutions_template/modules/terraform_gke/README.md
--rw-r--r--   0        0        0     1032 2023-06-12 17:37:53.053362 solutions_template-0.1.16/solutions_template/modules/terraform_gke/copier.yaml
--rw-r--r--   0        0        0      166 2023-05-29 05:54:17.246779 solutions_template-0.1.16/solutions_template/modules/terraform_gke/ingress/skaffold.yaml
--rw-r--r--   0        0        0      701 2023-05-25 05:06:12.024615 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/backend.tf
--rw-r--r--   0        0        0     1568 2023-05-25 03:02:53.830787 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/iam.tf
--rw-r--r--   0        0        0     2466 2023-05-25 05:02:51.705138 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/main.tf
--rw-r--r--   0        0        0     1783 2023-05-25 03:02:53.831430 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/providers.tf
--rw-r--r--   0        0        0      167 2023-05-25 05:06:56.865134 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
--rw-r--r--   0        0        0     1656 2023-05-25 05:02:58.250892 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/variables.tf
--rw-r--r--   0        0        0      709 2023-05-25 05:06:22.144012 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/backend.tf
--rw-r--r--   0        0        0     1568 2023-05-25 04:45:57.272841 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/iam.tf
--rw-r--r--   0        0        0     1765 2023-05-28 01:43:52.014934 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/main.tf
--rw-r--r--   0        0        0     1838 2023-05-26 06:25:11.934680 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/providers.tf
--rw-r--r--   0        0        0      327 2023-05-25 04:45:57.274732 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/terraform.tfvars
--rw-r--r--   0        0        0     1538 2023-05-25 04:45:57.275123 solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/variables.tf
--rw-r--r--   0        0        0     1038 2023-06-12 17:38:09.167120 solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/copier.yaml
--rw-r--r--   0        0        0      834 2023-05-28 03:28:10.934376 solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
--rw-r--r--   0        0        0     2760 2023-06-01 16:37:41.517011 solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
--rw-r--r--   0        0        0      671 2023-05-29 03:50:54.696615 solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
--rw-r--r--   0        0        0     1298 2023-06-01 06:45:19.546991 solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
--rw-r--r--   0        0        0       81 2023-05-28 06:36:18.400305 solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
--rw-r--r--   0        0        0      196 2023-06-01 07:43:52.668115 solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
--rw-r--r--   0        0        0     1967 2023-06-01 07:44:04.537279 solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
--rw-r--r--   0        0        0       74 2023-05-30 14:59:07.908351 solutions_template-0.1.16/solutions_template/requirements.txt
--rw-r--r--   0        0        0    68957 2022-10-04 18:33:22.391632 solutions_template-0.1.16/solutions_template/template_root/.github/assets/setup_local.png
--rw-r--r--   0        0        0   239307 2022-10-04 18:33:22.393205 solutions_template-0.1.16/solutions_template/template_root/.github/assets/skaffold_dev_terminal.png
--rw-r--r--   0        0        0     2639 2023-06-01 21:59:25.166269 solutions_template-0.1.16/solutions_template/template_root/.github/workflows/deployment_cloudrun_dev.yaml
--rw-r--r--   0        0        0     2690 2023-06-01 21:59:25.176262 solutions_template-0.1.16/solutions_template/template_root/.github/workflows/deployment_gke_dev.yaml
--rw-r--r--   0        0        0     5786 2023-06-01 21:59:25.166741 solutions_template-0.1.16/solutions_template/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
--rw-r--r--   0        0        0     8049 2023-06-01 21:59:25.158199 solutions_template-0.1.16/solutions_template/template_root/.github/workflows/e2e_gke_api_test.yaml
--rw-r--r--   0        0        0     3131 2023-06-01 21:59:25.176671 solutions_template-0.1.16/solutions_template/template_root/.github/workflows/unit_test_linter_common.yaml
--rw-r--r--   0        0        0      471 2023-05-30 15:18:57.732306 solutions_template-0.1.16/solutions_template/template_root/.gitignore
--rw-r--r--   0        0        0    14552 2023-04-18 17:18:30.552712 solutions_template-0.1.16/solutions_template/template_root/.pylintrc
--rw-r--r--   0        0        0      712 2023-05-21 07:33:08.118587 solutions_template-0.1.16/solutions_template/template_root/README.md
--rw-r--r--   0        0        0      396 2023-05-30 02:32:20.551320 solutions_template-0.1.16/solutions_template/template_root/components/README.md
--rw-r--r--   0        0        0      211 2023-05-25 05:43:28.697605 solutions_template-0.1.16/solutions_template/template_root/components/common/Dockerfile
--rw-r--r--   0        0        0      395 2023-05-25 05:42:52.638672 solutions_template-0.1.16/solutions_template/template_root/components/common/Dockerfile.unittest
--rw-r--r--   0        0        0       77 2022-12-12 19:00:31.973184 solutions_template-0.1.16/solutions_template/template_root/components/common/requirements-test.txt
--rw-r--r--   0        0        0      131 2022-12-12 19:00:25.828639 solutions_template-0.1.16/solutions_template/template_root/components/common/requirements.txt
--rw-r--r--   0        0        0      571 2023-05-24 05:29:26.584046 solutions_template-0.1.16/solutions_template/template_root/components/common/skaffold.yaml
--rw-r--r--   0        0        0        0 2022-10-04 18:33:22.397719 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/__init__.py
--rw-r--r--   0        0        0      832 2023-05-30 02:57:45.569143 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/config.py
--rw-r--r--   0        0        0      696 2023-05-30 02:57:45.625340 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/db_client.py
--rw-r--r--   0        0        0       35 2023-05-24 17:19:25.366436 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/models/README.md
--rw-r--r--   0        0        0       91 2022-10-04 18:33:22.398211 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/models/__init__.py
--rw-r--r--   0        0        0     1377 2023-05-30 02:57:45.587037 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/models/example.py
--rw-r--r--   0        0        0        0 2022-12-12 19:00:31.973251 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/testing/__init__.py
--rw-r--r--   0        0        0      755 2023-05-30 02:57:45.613334 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/testing/bq_client_fixture.py
--rw-r--r--   0        0        0     1007 2023-05-30 02:57:45.596847 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/testing/client_with_emulator.py
--rw-r--r--   0        0        0     2244 2023-05-30 02:57:45.604838 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/testing/firestore_emulator.py
--rw-r--r--   0        0        0        0 2022-10-04 18:33:22.399245 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/utils/__init__.py
--rw-r--r--   0        0        0     1003 2023-05-30 02:57:45.577363 solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/utils/logging_handler.py
--rw-r--r--   0        0        0     2015 2023-06-13 00:33:05.887322 solutions_template-0.1.16/solutions_template/template_root/copier.yaml
--rw-r--r--   0        0        0       97 2023-05-22 05:27:28.271050 solutions_template-0.1.16/solutions_template/template_root/firebase.json
--rw-r--r--   0        0        0       98 2022-10-04 18:33:22.406061 solutions_template-0.1.16/solutions_template/template_root/setup.cfg
--rw-r--r--   0        0        0      159 2023-05-23 04:16:52.790574 solutions_template-0.1.16/solutions_template/template_root/skaffold.yaml
--rw-r--r--   0        0        0      360 2023-05-25 04:16:44.183606 solutions_template-0.1.16/solutions_template/template_root/st.yaml
--rw-r--r--   0        0        0      921 2023-02-09 08:21:17.266853 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/cloudbuild/main.tf
--rw-r--r--   0        0        0      730 2023-04-06 20:09:34.304977 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/cloudbuild/variables.tf
--rw-r--r--   0        0        0     3585 2023-02-17 20:02:57.233059 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/cloudrun/main.tf
--rw-r--r--   0        0        0     1178 2023-02-09 08:21:17.269222 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/cloudrun/variables.tf
--rw-r--r--   0        0        0     5024 2023-06-01 07:44:40.709641 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/compute_backend/main.tf
--rw-r--r--   0        0        0      190 2023-06-01 07:09:48.790106 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/compute_backend/outputs.tf
--rw-r--r--   0        0        0     1185 2023-06-01 07:10:12.407650 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/compute_backend/providers.tf
--rw-r--r--   0        0        0     1601 2023-06-01 07:37:09.110897 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/compute_backend/variables.tf
--rw-r--r--   0        0        0     2364 2023-05-15 06:01:59.407051 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/firebase/main.tf
--rw-r--r--   0        0        0     1194 2023-05-21 07:19:21.355607 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/firebase/variables.tf
--rw-r--r--   0        0        0     4235 2023-04-18 16:34:06.671602 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/gke/main.tf
--rw-r--r--   0        0        0      832 2022-12-21 18:43:24.639052 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/gke/outputs.tf
--rw-r--r--   0        0        0     2739 2023-04-18 16:34:06.672029 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/gke/variables.tf
--rw-r--r--   0        0        0     2766 2023-05-28 02:23:48.828747 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_gce/main.tf
--rw-r--r--   0        0        0      670 2023-04-06 20:09:34.305878 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_gce/outputs.tf
--rw-r--r--   0        0        0     1144 2023-05-26 06:30:14.475682 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_gce/variables.tf
--rw-r--r--   0        0        0     2926 2023-05-25 03:41:05.195766 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_nginx/main.tf
--rw-r--r--   0        0        0      692 2023-04-06 20:09:34.306862 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_nginx/outputs.tf
--rw-r--r--   0        0        0     1087 2023-05-25 03:41:05.180007 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_nginx/variables.tf
--rw-r--r--   0        0        0      827 2023-02-09 08:21:17.272152 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/project_services/main.tf
--rw-r--r--   0        0        0      773 2023-02-09 08:21:17.272922 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/project_services/variables.tf
--rw-r--r--   0        0        0      953 2023-05-24 07:11:09.106862 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/service_account/main.tf
--rw-r--r--   0        0        0     1037 2023-05-24 07:10:42.362340 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/service_account/variables.tf
--rw-r--r--   0        0        0     1529 2023-02-09 08:21:17.274369 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/terraform_cicd/main.tf
--rw-r--r--   0        0        0      677 2023-02-09 08:21:17.274786 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/terraform_cicd/variables.tf
--rw-r--r--   0        0        0     1333 2023-04-18 16:34:06.672425 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/vpc_network/main.tf
--rw-r--r--   0        0        0     1269 2023-04-18 16:34:06.672853 solutions_template-0.1.16/solutions_template/template_root/terraform/modules/vpc_network/variables.tf
--rw-r--r--   0        0        0     2193 2023-06-13 00:47:55.285380 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/1-bootstrap/main.tf
--rw-r--r--   0        0        0      730 2023-05-23 17:46:04.906168 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/1-bootstrap/output.tf
--rw-r--r--   0        0        0       66 2023-05-23 15:50:30.740634 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/1-bootstrap/terraform.tfvars
--rw-r--r--   0        0        0     1071 2023-05-24 21:09:42.811911 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/1-bootstrap/variables.tf
--rw-r--r--   0        0        0      826 2023-05-25 04:52:26.974900 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/backend.tf
--rw-r--r--   0        0        0      517 2023-05-31 01:49:50.316186 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/firestore_setup.tf
--rw-r--r--   0        0        0     1568 2023-02-09 08:21:17.277689 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/iam.tf
--rw-r--r--   0        0        0     4252 2023-06-13 00:07:54.373894 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/main.tf
--rw-r--r--   0        0        0      997 2023-04-18 16:34:06.673104 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/outputs.tf
--rw-r--r--   0        0        0      835 2023-05-24 21:02:04.508401 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/providers.tf
--rw-r--r--   0        0        0      606 2023-06-13 00:43:16.927637 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/terraform.tfvars
--rw-r--r--   0        0        0     2546 2023-05-24 21:12:44.825641 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/variables.tf
--rw-r--r--   0        0        0      826 2023-05-25 04:51:02.718052 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/3-components/backend.tf
--rw-r--r--   0        0        0      835 2023-05-28 05:25:10.403140 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/3-components/providers.tf
--rw-r--r--   0        0        0      148 2023-05-24 21:13:00.091007 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/3-components/terraform.tfvars
--rw-r--r--   0        0        0     1679 2023-05-28 03:10:58.053820 solutions_template-0.1.16/solutions_template/template_root/terraform/stages/3-components/variables.tf
--rw-r--r--   0        0        0        0 2023-06-12 15:36:45.632098 solutions_template-0.1.16/solutions_template/template_root/tests/__init__.py
--rw-r--r--   0        0        0      825 2023-06-12 19:49:41.174517 solutions_template-0.1.16/solutions_template/template_root/tests/e2e/e2e_utils.py
--rwxr-xr-x   0        0        0      364 2023-06-01 05:17:15.058707 solutions_template-0.1.16/solutions_template/template_root/utils/disable_org_policies.sh
--rwxr-xr-x   0        0        0     1095 2023-05-23 21:49:37.910891 solutions_template-0.1.16/solutions_template/template_root/utils/init_env_vars.sh
--rwxr-xr-x   0        0        0    13137 2023-05-21 07:19:19.594900 solutions_template-0.1.16/solutions_template/template_root/utils/setup_all.sh
--rwxr-xr-x   0        0        0     2835 2023-04-04 14:56:36.000614 solutions_template-0.1.16/solutions_template/template_root/utils/setup_local.sh
--rw-r--r--   0        0        0       81 2023-05-21 06:56:40.727501 solutions_template-0.1.16/solutions_template/template_root/{{_copier_conf.answers_file}}
--rw-r--r--   0        0        0        0 2023-05-30 04:08:59.454480 solutions_template-0.1.16/solutions_template/tests/__init__.py
--rw-r--r--   0        0        0     5946 1970-01-01 00:00:00.000000 solutions_template-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-06-28 21:05:37.723277 solutions_template-1.9.0/LICENSE
+-rw-r--r--   0        0        0     4839 2023-06-15 18:40:51.230107 solutions_template-1.9.0/README.md
+-rw-r--r--   0        0        0     1105 2023-06-15 18:42:19.667601 solutions_template-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.883150 solutions_template-1.9.0/solutions_template/__init__.py
+-rw-r--r--   0        0        0     5659 2023-06-16 02:54:27.663884 solutions_template-1.9.0/solutions_template/cli/cli.py
+-rw-r--r--   0        0        0     4199 2023-06-15 16:31:59.883928 solutions_template-1.9.0/solutions_template/cli/cli_utils.py
+-rw-r--r--   0        0        0     6184 2023-06-16 03:59:18.084087 solutions_template-1.9.0/solutions_template/cli/component.py
+-rw-r--r--   0        0        0     5883 2023-06-15 16:31:59.884617 solutions_template-1.9.0/solutions_template/cli/infra.py
+-rw-r--r--   0        0        0     1072 2023-06-15 16:31:59.884862 solutions_template-1.9.0/solutions_template/cli/tool.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.884916 solutions_template-1.9.0/solutions_template/copier_extensions/__init__.py
+-rw-r--r--   0        0        0     3561 2023-06-15 16:31:59.885392 solutions_template-1.9.0/solutions_template/copier_extensions/st_helpers.py
+-rw-r--r--   0        0        0       80 2023-06-15 16:31:59.885841 solutions_template-1.9.0/solutions_template/modules/restful_service/.st/module_answers/{{component_name}}.yaml
+-rw-r--r--   0        0        0      545 2023-06-15 16:31:59.886671 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/Dockerfile
+-rw-r--r--   0        0        0     1258 2023-06-15 16:31:59.886951 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/README.md
+-rw-r--r--   0        0        0      215 2023-06-15 16:31:59.887289 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/manifests/cloudrun-service.yaml
+-rw-r--r--   0        0        0       77 2023-06-15 16:31:59.887400 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/requirements-test.txt
+-rw-r--r--   0        0        0      109 2023-06-15 16:31:59.887740 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/requirements.txt
+-rw-r--r--   0        0        0     3182 2023-06-16 02:53:26.841584 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/skaffold.yaml
+-rw-r--r--   0        0        0      863 2023-06-15 16:31:59.888227 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/config.py
+-rw-r--r--   0        0        0     1871 2023-06-15 16:31:59.888781 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/main.py
+-rw-r--r--   0        0        0     1664 2023-06-16 05:03:43.370908 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.889165 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/__init__.py
+-rw-r--r--   0        0        0     3876 2023-06-16 05:04:41.195170 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py
+-rw-r--r--   0        0        0     1222 2023-06-16 05:08:22.051091 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/schemas/{{data_model}}.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.890086 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/utils/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-15 16:31:59.890476 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/st_module.yaml
+-rw-r--r--   0        0        0     1191 2023-06-15 16:31:59.890863 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml
+-rw-r--r--   0        0        0      197 2023-06-15 16:31:59.891124 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/kustomization.yaml
+-rw-r--r--   0        0        0       60 2023-06-15 16:31:59.891325 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/properties.env
+-rw-r--r--   0        0        0      229 2023-06-15 16:31:59.891641 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/service.yaml
+-rw-r--r--   0        0        0      421 2023-06-15 16:31:59.891935 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/hpa.yaml
+-rw-r--r--   0        0        0      103 2023-06-15 16:31:59.892130 solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/hpa/kustomization.yaml
+-rw-r--r--   0        0        0     2255 2023-06-16 01:17:41.774796 solutions_template-1.9.0/solutions_template/modules/restful_service/copier.yaml
+-rw-r--r--   0        0        0       92 2023-06-15 16:31:59.892900 solutions_template-1.9.0/solutions_template/modules/restful_service/skaffold.yaml.patch
+-rw-r--r--   0        0        0      263 2023-06-15 16:31:59.893286 solutions_template-1.9.0/solutions_template/modules/restful_service/terraform/stages/{{'3-httplb-cloudrun' if cloudrun_neg}}/{{component_name}}_neg.tf
+-rw-r--r--   0        0        0     3461 2023-06-15 16:31:59.893746 solutions_template-1.9.0/solutions_template/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py
+-rw-r--r--   0        0        0     3269 2023-06-15 16:31:59.894288 solutions_template-1.9.0/solutions_template/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml
+-rw-r--r--   0        0        0     1165 2023-06-16 04:09:29.339712 solutions_template-1.9.0/solutions_template/modules/terraform_gke/copier.yaml
+-rw-r--r--   0        0        0      792 2023-06-15 16:31:59.894621 solutions_template-1.9.0/solutions_template/modules/terraform_gke/docs/modules/{{component_name}}.md
+-rw-r--r--   0        0        0      166 2023-06-15 16:31:59.895201 solutions_template-1.9.0/solutions_template/modules/terraform_gke/ingress/skaffold.yaml
+-rw-r--r--   0        0        0      701 2023-06-15 16:31:59.895524 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/backend.tf
+-rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.895667 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/iam.tf
+-rw-r--r--   0        0        0     2466 2023-06-15 16:31:59.895836 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/main.tf
+-rw-r--r--   0        0        0     1783 2023-06-15 16:31:59.895957 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/providers.tf
+-rw-r--r--   0        0        0      167 2023-06-15 16:31:59.896270 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/terraform.tfvars
+-rw-r--r--   0        0        0     1656 2023-06-15 16:31:59.896449 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/variables.tf
+-rw-r--r--   0        0        0      709 2023-06-15 16:31:59.896669 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/backend.tf
+-rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.896852 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/iam.tf
+-rw-r--r--   0        0        0     1765 2023-06-15 16:31:59.897192 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/main.tf
+-rw-r--r--   0        0        0     1838 2023-06-15 16:31:59.897489 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/providers.tf
+-rw-r--r--   0        0        0      327 2023-06-15 16:31:59.897664 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/terraform.tfvars
+-rw-r--r--   0        0        0     1538 2023-06-15 16:31:59.897824 solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/variables.tf
+-rw-r--r--   0        0        0     1038 2023-06-15 16:31:59.898140 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/copier.yaml
+-rw-r--r--   0        0        0      834 2023-06-15 16:31:59.898543 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf
+-rw-r--r--   0        0        0     2760 2023-06-15 16:31:59.898838 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf
+-rw-r--r--   0        0        0      671 2023-06-15 16:31:59.899283 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf
+-rw-r--r--   0        0        0     1298 2023-06-15 16:31:59.899651 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf
+-rw-r--r--   0        0        0       81 2023-06-15 16:31:59.899785 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/st_module.yaml
+-rw-r--r--   0        0        0      196 2023-06-15 16:31:59.899968 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/terraform.tfvars
+-rw-r--r--   0        0        0     1967 2023-06-15 16:31:59.900160 solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf
+-rw-r--r--   0        0        0       74 2023-06-15 16:31:59.900522 solutions_template-1.9.0/solutions_template/requirements.txt
+-rw-r--r--   0        0        0    68957 2023-06-15 16:31:59.901015 solutions_template-1.9.0/solutions_template/template_root/.github/assets/setup_local.png
+-rw-r--r--   0        0        0   239307 2023-06-15 16:31:59.902244 solutions_template-1.9.0/solutions_template/template_root/.github/assets/skaffold_dev_terminal.png
+-rw-r--r--   0        0        0     2639 2023-06-15 16:31:59.902916 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/deployment_cloudrun_dev.yaml
+-rw-r--r--   0        0        0     2690 2023-06-15 16:31:59.903239 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/deployment_gke_dev.yaml
+-rw-r--r--   0        0        0     5786 2023-06-15 16:31:59.905439 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/e2e_cloudrun_api_test.yaml
+-rw-r--r--   0        0        0     8049 2023-06-15 16:31:59.912323 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/e2e_gke_api_test.yaml
+-rw-r--r--   0        0        0     3131 2023-06-15 16:31:59.916647 solutions_template-1.9.0/solutions_template/template_root/.github/workflows/unit_test_linter_common.yaml
+-rw-r--r--   0        0        0      471 2023-06-15 16:31:59.917181 solutions_template-1.9.0/solutions_template/template_root/.gitignore
+-rw-r--r--   0        0        0    14552 2023-06-15 16:31:59.919314 solutions_template-1.9.0/solutions_template/template_root/.pylintrc
+-rw-r--r--   0        0        0      712 2023-06-15 16:31:59.919730 solutions_template-1.9.0/solutions_template/template_root/README.md
+-rw-r--r--   0        0        0      396 2023-06-15 16:31:59.920032 solutions_template-1.9.0/solutions_template/template_root/components/README.md
+-rw-r--r--   0        0        0      211 2023-06-15 16:31:59.920301 solutions_template-1.9.0/solutions_template/template_root/components/common/Dockerfile
+-rw-r--r--   0        0        0      395 2023-06-15 16:31:59.920640 solutions_template-1.9.0/solutions_template/template_root/components/common/Dockerfile.unittest
+-rw-r--r--   0        0        0       77 2023-06-15 16:31:59.920716 solutions_template-1.9.0/solutions_template/template_root/components/common/requirements-test.txt
+-rw-r--r--   0        0        0      131 2023-06-15 16:31:59.920842 solutions_template-1.9.0/solutions_template/template_root/components/common/requirements.txt
+-rw-r--r--   0        0        0      571 2023-06-15 16:31:59.921142 solutions_template-1.9.0/solutions_template/template_root/components/common/skaffold.yaml
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.921222 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-15 16:31:59.921500 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/config.py
+-rw-r--r--   0        0        0      696 2023-06-15 16:31:59.921923 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/db_client.py
+-rw-r--r--   0        0        0       35 2023-06-15 16:31:59.922651 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/models/README.md
+-rw-r--r--   0        0        0       91 2023-06-15 16:31:59.922920 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/models/__init__.py
+-rw-r--r--   0        0        0     1377 2023-06-15 16:31:59.923190 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/models/example.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.923251 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/__init__.py
+-rw-r--r--   0        0        0      755 2023-06-15 16:31:59.923525 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/bq_client_fixture.py
+-rw-r--r--   0        0        0     1007 2023-06-15 16:31:59.923771 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/client_with_emulator.py
+-rw-r--r--   0        0        0     2244 2023-06-15 16:31:59.924001 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/firestore_emulator.py
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.924090 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/utils/__init__.py
+-rw-r--r--   0        0        0     1003 2023-06-15 16:31:59.924293 solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/utils/logging_handler.py
+-rw-r--r--   0        0        0     2015 2023-06-15 16:31:59.924591 solutions_template-1.9.0/solutions_template/template_root/copier.yaml
+-rw-r--r--   0        0        0       97 2023-06-15 16:31:59.924976 solutions_template-1.9.0/solutions_template/template_root/firebase.json
+-rw-r--r--   0        0        0       98 2023-06-15 16:31:59.925120 solutions_template-1.9.0/solutions_template/template_root/setup.cfg
+-rw-r--r--   0        0        0      159 2023-06-15 16:31:59.925502 solutions_template-1.9.0/solutions_template/template_root/skaffold.yaml
+-rw-r--r--   0        0        0      360 2023-06-15 16:31:59.925681 solutions_template-1.9.0/solutions_template/template_root/st.yaml
+-rw-r--r--   0        0        0      921 2023-06-15 16:31:59.925959 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudbuild/main.tf
+-rw-r--r--   0        0        0      730 2023-06-15 16:31:59.926143 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudbuild/variables.tf
+-rw-r--r--   0        0        0     3585 2023-06-15 16:31:59.926376 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudrun/main.tf
+-rw-r--r--   0        0        0     1178 2023-06-15 16:31:59.926551 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudrun/variables.tf
+-rw-r--r--   0        0        0     5024 2023-06-15 16:31:59.927017 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/main.tf
+-rw-r--r--   0        0        0      190 2023-06-15 16:31:59.927289 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/outputs.tf
+-rw-r--r--   0        0        0     1185 2023-06-15 16:31:59.927608 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/providers.tf
+-rw-r--r--   0        0        0     1601 2023-06-15 16:31:59.927810 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/variables.tf
+-rw-r--r--   0        0        0     2364 2023-06-15 16:31:59.927994 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/firebase/main.tf
+-rw-r--r--   0        0        0     1194 2023-06-15 16:31:59.928358 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/firebase/variables.tf
+-rw-r--r--   0        0        0     4235 2023-06-15 16:31:59.928596 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/main.tf
+-rw-r--r--   0        0        0      832 2023-06-15 16:31:59.928824 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/outputs.tf
+-rw-r--r--   0        0        0     2739 2023-06-15 16:31:59.929183 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/variables.tf
+-rw-r--r--   0        0        0     2766 2023-06-15 16:31:59.929718 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/main.tf
+-rw-r--r--   0        0        0      670 2023-06-15 16:31:59.929888 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/outputs.tf
+-rw-r--r--   0        0        0     1144 2023-06-15 16:31:59.930158 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/variables.tf
+-rw-r--r--   0        0        0     2926 2023-06-15 16:31:59.930393 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/main.tf
+-rw-r--r--   0        0        0      692 2023-06-15 16:31:59.930656 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/outputs.tf
+-rw-r--r--   0        0        0     1087 2023-06-15 16:31:59.931016 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/variables.tf
+-rw-r--r--   0        0        0      827 2023-06-15 16:31:59.931291 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/project_services/main.tf
+-rw-r--r--   0        0        0      773 2023-06-15 16:31:59.931538 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/project_services/variables.tf
+-rw-r--r--   0        0        0      953 2023-06-15 16:31:59.931934 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/service_account/main.tf
+-rw-r--r--   0        0        0     1037 2023-06-15 16:31:59.932426 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/service_account/variables.tf
+-rw-r--r--   0        0        0     1529 2023-06-15 16:31:59.932733 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/terraform_cicd/main.tf
+-rw-r--r--   0        0        0      677 2023-06-15 16:31:59.933018 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/terraform_cicd/variables.tf
+-rw-r--r--   0        0        0     1333 2023-06-15 16:31:59.933248 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/vpc_network/main.tf
+-rw-r--r--   0        0        0     1269 2023-06-15 16:31:59.933426 solutions_template-1.9.0/solutions_template/template_root/terraform/modules/vpc_network/variables.tf
+-rw-r--r--   0        0        0     2193 2023-06-15 16:31:59.933834 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/main.tf
+-rw-r--r--   0        0        0      730 2023-06-15 16:31:59.934084 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/output.tf
+-rw-r--r--   0        0        0       66 2023-06-15 16:31:59.934377 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/terraform.tfvars
+-rw-r--r--   0        0        0     1071 2023-06-15 16:31:59.934790 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/variables.tf
+-rw-r--r--   0        0        0      826 2023-06-15 16:31:59.935095 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/backend.tf
+-rw-r--r--   0        0        0      517 2023-06-15 16:31:59.935395 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/firestore_setup.tf
+-rw-r--r--   0        0        0     1568 2023-06-15 16:31:59.935538 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/iam.tf
+-rw-r--r--   0        0        0     4252 2023-06-15 16:31:59.935804 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/main.tf
+-rw-r--r--   0        0        0      997 2023-06-15 16:31:59.935925 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/outputs.tf
+-rw-r--r--   0        0        0      835 2023-06-15 16:31:59.936181 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/providers.tf
+-rw-r--r--   0        0        0      606 2023-06-15 16:31:59.936549 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/terraform.tfvars
+-rw-r--r--   0        0        0     2546 2023-06-15 16:31:59.936876 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/variables.tf
+-rw-r--r--   0        0        0      826 2023-06-15 16:31:59.937252 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/backend.tf
+-rw-r--r--   0        0        0      835 2023-06-15 16:31:59.937397 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/providers.tf
+-rw-r--r--   0        0        0      148 2023-06-15 16:31:59.937688 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/terraform.tfvars
+-rw-r--r--   0        0        0     1679 2023-06-15 16:31:59.937915 solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/variables.tf
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.937992 solutions_template-1.9.0/solutions_template/template_root/tests/__init__.py
+-rw-r--r--   0        0        0      825 2023-06-15 16:31:59.938319 solutions_template-1.9.0/solutions_template/template_root/tests/e2e/e2e_utils.py
+-rwxr-xr-x   0        0        0      364 2023-06-15 16:31:59.938529 solutions_template-1.9.0/solutions_template/template_root/utils/disable_org_policies.sh
+-rwxr-xr-x   0        0        0     1095 2023-06-15 16:31:59.938794 solutions_template-1.9.0/solutions_template/template_root/utils/init_env_vars.sh
+-rwxr-xr-x   0        0        0    13137 2023-06-15 16:31:59.939050 solutions_template-1.9.0/solutions_template/template_root/utils/setup_all.sh
+-rwxr-xr-x   0        0        0     2835 2023-06-15 16:31:59.939218 solutions_template-1.9.0/solutions_template/template_root/utils/setup_local.sh
+-rw-r--r--   0        0        0       81 2023-06-15 16:31:59.939607 solutions_template-1.9.0/solutions_template/template_root/{{_copier_conf.answers_file}}
+-rw-r--r--   0        0        0        0 2023-06-15 16:31:59.939700 solutions_template-1.9.0/solutions_template/tests/__init__.py
+-rw-r--r--   0        0        0     5822 1970-01-01 00:00:00.000000 solutions_template-1.9.0/PKG-INFO
```

### Comparing `solutions_template-0.1.16/LICENSE` & `solutions_template-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/README.md` & `solutions_template-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 | Kustomize   | &gt;= v5.0.0 | https://kubectl.docs.kubernetes.io/installation/kustomize/ |
 
 ## Installing Solutions Template CLI
 
 With `pip`:
 ```
 pip install solutions-template
-
-# Alternatively, to install from PyPI-Test, run:
-pip install --index-url https://test.pypi.org/simple/ solutions-template
 ```
 
 With `pipx`:
 ```
 pip install --user pipx
 pipx install solutions-template
 ```
```

### Comparing `solutions_template-0.1.16/pyproject.toml` & `solutions_template-1.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solutions-template"
-version = "0.1.16"
+version = "1.9.0"
 description = "A solution framework to generate a project with built-in structure and modules"
 authors = ["Jon Chen <jonchen@google.com>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://github.com/GoogleCloudPlatform/solutions-template"
 repository = "https://github.com/GoogleCloudPlatform/solutions-template"
 packages = [
```

### Comparing `solutions_template-0.1.16/solutions_template/cli/cli.py` & `solutions_template-1.9.0/solutions_template/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,26 +23,33 @@
 from .component import component_app
 from .tool import tool_app
 from .infra import infra_app
 from .cli_utils import *
 
 __version__ = importlib.metadata.version("solutions-template")
 
-app = typer.Typer(add_completion=False)
+app = typer.Typer(
+    add_completion=False,
+    help=
+    "Solutions Template CLI. See https://github.com/GoogleCloudPlatform/solutions-template for details."
+)
 app.add_typer(component_app, name="component")
 app.add_typer(tool_app, name="tool")
 app.add_typer(infra_app, name="infra")
 
 
 # Create a new solution
 @app.command()
 def new(folder_name,
         output_dir: Annotated[Optional[str], typer.Argument()] = ".",
         template_path=None,
         answers=None):
+  """
+  Create a new solution folder.
+  """
   output_path = f"{output_dir}/{folder_name}"
   output_path = output_path.replace("//", "/")
   answers_dict = get_answers_dict(answers)
 
   if not template_path:
     current_dir = os.path.dirname(__file__)
     template_path = f"{current_dir}/../template_root"
@@ -59,14 +66,17 @@
 
 
 # Update a solution
 @app.command()
 def update(solution_path: Annotated[Optional[str],
                                     typer.Argument()] = ".",
            template_path=None):
+  """
+  Update an existing solution folder.
+  """
   if not solution_path:
     solution_path = "."
 
   validate_solution_folder(solution_path)
 
   if not os.path.exists(solution_path):
     raise FileNotFoundError(f"Solution folder {solution_path} does not exist.")
@@ -95,19 +105,22 @@
   write_yaml(f"{solution_path}/st.yaml", st_yaml)
 
   print_success(f"Complete. Solution folder updated at {solution_path}.\n")
 
 
 # Build and deploy services.
 @app.command()
-def deploy(profile: str = "default",
+def deploy(profile: str = "default-deploy",
            component: str = None,
            solution_path: Annotated[Optional[str],
                                     typer.Argument()] = ".",
            yes: Optional[bool] = False):
+  """
+  Build and deploy services.
+  """
   validate_solution_folder(solution_path)
 
   solution_yaml_dict = read_yaml(f"{solution_path}/st.yaml")
   project_id = solution_yaml_dict["project_id"]
 
   if component:
     component_flag = f" -m {component} "
@@ -117,21 +130,24 @@
   command = f"skaffold run -p {profile} {component_flag} --default-repo=\"gcr.io/{project_id}\""
   print("This will build and deploy all services using the command below:")
   print_highlight(command)
   confirm("\nThis may take a few minutes. Continue?", skip=yes)
   exec_shell(command, working_dir=solution_path)
 
 
-# Destory services.
+# Destory deployment.
 @app.command()
 def destroy(profile: str = "default",
             component: str = None,
             solution_path: Annotated[Optional[str],
                                      typer.Argument()] = ".",
             yes: Optional[bool] = False):
+  """
+  Destory deployment.
+  """
   validate_solution_folder(solution_path)
 
   solution_yaml_dict = read_yaml(f"{solution_path}/st.yaml")
   project_id = solution_yaml_dict["project_id"]
 
   if component:
     component_flag = f" -m {component} "
@@ -143,20 +159,26 @@
   print_highlight(command)
   confirm("\nThis may take a few minutes. Continue?", default=False, skip=yes)
   exec_shell(command, working_dir=solution_path)
 
 
 @app.command()
 def version():
+  """
+  Print version.
+  """
   print(f"Solutions Template v{__version__}")
   raise typer.Exit()
 
 
 def main():
   try:
+    print_highlight(f"Solutions Template (version " +
+                    typer.style(__version__, fg=typer.colors.CYAN, bold=True) +
+                    ")\n")
     app()
     print()
 
   except Exception as e:
     if os.getenv("DEBUG", False):
       traceback.print_exc()
     print_error(e)
```

### Comparing `solutions_template-0.1.16/solutions_template/cli/cli_utils.py` & `solutions_template-1.9.0/solutions_template/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/cli/component.py` & `solutions_template-1.9.0/solutions_template/cli/component.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,14 +143,29 @@
     new_yaml = patch_yaml(f"{solution_path}/{patch_file}",
                           f"{solution_path}/{patch_file}.patch")
     new_yaml["requires"] = dedupe(new_yaml["requires"])
     write_yaml(f"{solution_path}/{patch_file}", new_yaml)
     os.remove(f"{solution_path}/{patch_file}.patch")
 
 
-# Add specific component to the destination solution folder.
+# List installed components.
 @component_app.command()
-def list():
+def list(solution_path: Annotated[Optional[str], typer.Argument()] = ".", ):
+  root_st_yaml = read_yaml(f"{solution_path}/st.yaml")
+  components = root_st_yaml.get("components", [])
+  print("Installed components:\n")
+  for component_name, properties in components.items():
+    typer.echo(
+        typer.style(f"- {component_name} ", fg=typer.colors.WHITE, bold=True) +
+        typer.style(f"(module: {properties['component_template']})",
+                    fg=typer.colors.BLACK,
+                    bold=True))
+  print()
+
+
+# List available components to add.
+@component_app.command()
+def available():
   current_dir = os.path.dirname(__file__)
   path = current_dir + "/../modules"
   print("Available modules:\n")
   list_subfolders(path)
```

### Comparing `solutions_template-0.1.16/solutions_template/cli/infra.py` & `solutions_template-1.9.0/solutions_template/cli/infra.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/cli/tool.py` & `solutions_template-1.9.0/solutions_template/cli/tool.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/copier_extensions/st_helpers.py` & `solutions_template-1.9.0/solutions_template/copier_extensions/st_helpers.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/Dockerfile` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/README.md` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/README.md`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/skaffold.yaml` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/skaffold.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -114,17 +114,17 @@
   - resourceType: service
     resourceName: {{resource_name}}
     port: 80
     localPort: {{local_port}} # Change this when adding other microservice.
 {%- endif %}
 
 {% if default_deploy == "cloudrun" -%}
-# The default profile refer to cloudrun profile above.
+# The default-deploy profile refer to cloudrun profile above.
 - <<: *cloudrun-profile
-  name: default
+  name: default-deploy
 {%- endif %}
 
 {% if default_deploy == "gke" -%}
-# The default profile refer to gke profile above.
+# The default-deploy profile refer to gke profile above.
 - <<: *gke-profile
-  name: default
+  name: default-deploy
 {%- endif %}
```

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/config.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/config.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/main.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/main.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/models/{{data_model}}.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,43 +11,47 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 """
-Data model for {{data_model | capitalize}} list.
+Data model for {{data_model | capitalize}}. See https://octabyte.io/FireO/ for details.
 """
 
 import os
 
-from firedantic import Model
-from firedantic.exceptions import ModelNotFoundError
+from fireo.models import Model
+from fireo.fields import IDField, TextField, BooleanField, DateTime
+from fireo.queries.errors import ReferenceDocNotExist
 from datetime import datetime
 
 # GCP project_id from system's environment variable.
 PROJECT_ID = os.environ.get("PROJECT_ID", "")
 
 # Database prefix for integration and e2e test purpose.
 DATABASE_PREFIX = os.getenv("DATABASE_PREFIX", "")
 
 
 # Firebase data model in "{{data_model_plural}}" collection.
 class {{data_model | capitalize}}(Model):
   """{{data_model | capitalize}} ORM class"""
-  __collection__ = "{{data_model_plural}}"
 
-  id: str = "1234"
-  title: str = "Title"
-  description: str = "Description"
-  is_done: bool = False
-  created_at: datetime = None
-  modified_at: datetime = None
+  class Meta:
+    ignore_none_field = False
+    collection_name = DATABASE_PREFIX + "{{data_model_plural}}"
+
+  id = IDField()
+  title = TextField()
+  description = TextField()
+  status = TextField()
+  created_at = DateTime()
+  modified_at = DateTime()
 
   @classmethod
   def find_by_id(cls, id):
     try:
-      {{data_model}} = {{data_model | capitalize}}.get_by_doc_id(id)
-    except ModelNotFoundError:
+      {{data_model}} = {{data_model | capitalize}}.collection.get(id)
+    except ReferenceDocNotExist:
       return None
 
     return {{data_model}}
```

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/src/routes/{{data_model_plural}}.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from fastapi import APIRouter, HTTPException
 from models.{{data_model}} import {{data_model | capitalize}}
+from schemas.{{data_model}} import {{data_model | capitalize}}Schema
 import datetime
 
 # disabling for linting to pass
 # pylint: disable = broad-except
 
 router = APIRouter(prefix="/{{data_model}}", tags=["{{data_model}}"])
 
 SUCCESS_RESPONSE = {"status": "Success"}
 
 
-@router.get("/{id}", response_model={{data_model | capitalize}})
+@router.get("/{id}", response_model={{data_model | capitalize}}Schema)
 async def get(id: str):
   """Get a {{data_model | capitalize}}
 
   Args:
     id (str): unique id of the {{data_model}}
 
   Raises:
@@ -44,60 +45,60 @@
 
   if {{data_model}} is None:
     raise HTTPException(status_code=404, detail=f"{{data_model | capitalize}} {id} not found.")
   return {{data_model}}
 
 
 @router.post("")
-async def post({{data_model}}: {{data_model | capitalize}}):
+async def post(data: {{data_model | capitalize}}Schema):
   """Create a {{data_model | capitalize}}
 
   Args:
     data ({{data_model | capitalize}}): Required body of the {{data_model}}
 
   Raises:
     HTTPException: 500 Internal Server Error if something fails
 
   Returns:
     [JSON]: {{data_model}} ID of the {{data_model}} if the {{data_model}} is successfully created
   """
-  try:
-    id = {{data_model}}.id
-    existing_{{data_model}} = {{data_model | capitalize}}.find_by_id(id)
-
-    if existing_{{data_model}}:
-      raise HTTPException(status_code=409,
-                          detail=f"{{data_model | capitalize}} {id} already exists.")
-    {{data_model}}.created_at = datetime.datetime.utcnow()
-    {{data_model}}.modified_at = datetime.datetime.utcnow()
-    {{data_model}}.save()
-    return {{data_model}}
+  id = data.id
+  existing_{{data_model}} = {{data_model | capitalize}}.find_by_id(id)
+
+  if existing_{{data_model}}:
+    raise HTTPException(status_code=409,
+                        detail=f"{{data_model | capitalize}} {id} already exists.")
 
-  except Exception as e:
-    raise HTTPException(status_code=500, detail=e) from e
+  new_{{data_model}} = {{data_model | capitalize}}()
+  new_{{data_model}} = new_{{data_model}}.from_dict({**data.dict()})
+  new_{{data_model}}.created_at = datetime.datetime.utcnow()
+  new_{{data_model}}.modified_at = datetime.datetime.utcnow()
+  new_{{data_model}}.save()
+
+  return SUCCESS_RESPONSE
 
 
 @router.put("")
-async def put({{data_model}}: {{data_model | capitalize}}):
+async def put(data: {{data_model | capitalize}}Schema):
   """Update a {{data_model | capitalize}}
 
   Args:
     data ({{data_model | capitalize}}): Required body of the {{data_model}}
 
   Raises:
     HTTPException: 500 Internal Server Error if something fails
 
   Returns:
     [JSON]: {'status': 'Succeed'} if the {{data_model}} is updated
   """
-  id = {{data_model}}.id
-  existing_{{data_model}} = {{data_model | capitalize}}.find_by_id(id)
+  id = data.id
+  {{data_model}} = {{data_model | capitalize}}.find_by_id(id)
 
-  if existing_{{data_model}}:
-    {{data_model}}.created_at = existing_{{data_model}}.created_at
+  if {{data_model}}:
+    {{data_model}} = {{data_model}}.from_dict({**data.dict()})
     {{data_model}}.modified_at = datetime.datetime.utcnow()
     {{data_model}}.save()
 
   else:
     raise HTTPException(status_code=404, detail=f"{{data_model | capitalize}} {id} not found.")
 
   return SUCCESS_RESPONSE
@@ -117,10 +118,10 @@
     [JSON]: {'status': 'Succeed'} if the {{data_model}} is deleted
   """
 
   {{data_model}} = {{data_model | capitalize}}.find_by_id(id)
   if {{data_model}} is None:
     raise HTTPException(status_code=404, detail=f"{{data_model | capitalize}} {id} not found.")
 
-  {{data_model}}.delete()
+  {{data_model | capitalize}}.collection.delete({{data_model}}.key)
 
   return SUCCESS_RESPONSE
```

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml` & `solutions_template-1.9.0/solutions_template/modules/restful_service/components/{{component_name}}/{{'kustomize' if deploy_gke else ''}}/base/deployment.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/copier.yaml` & `solutions_template-1.9.0/solutions_template/modules/restful_service/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py` & `solutions_template-1.9.0/solutions_template/modules/restful_service/tests/e2e/{{component_name}}_e2e_test.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml` & `solutions_template-1.9.0/solutions_template/modules/restful_service/{{'.github' if use_github_action}}/workflows/unit_test_linter_{{component_name}}.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/README.md` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/docs/modules/{{component_name}}.md`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/copier.yaml` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/copier.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,19 @@
   module_name: terraform_gke
   version: 1.0.0
   destination_path: .
 
 # questions
 component_name:
   type: str
+  help: What is the name of this component (snake_case)?
+  default: terraform_gke
+
+terraform_stage_name:
+  type: str
   help: What is the name of this terraform stage?
   default: 2-gke
 
 gcp_region:
   type: str
   help: Which Google Cloud region?
   default: us-central1
@@ -39,12 +44,13 @@
   - ".terraform*"
   - ".tmp"
   - ".venv"
   - ".pytest_cache"
   - "__pycache__"
   - "*-debug.log"
   - ".skip"
+  - "README.md"
 
 _jinja_extensions:
   - jinja2_time.TimeExtension
   - copier_templates_extensions.TemplateExtensionLoader
   - ../../copier_extensions/st_helpers.py:SolutionsTemplateHelpersExtension
```

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/backend.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/iam.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/main.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/providers.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/2-gke/variables.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/2-gke/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/backend.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/iam.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/main.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/providers.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/variables.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_gke/terraform/stages/3-ingress-gke/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/copier.yaml` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf` & `solutions_template-1.9.0/solutions_template/modules/terraform_httplb_cloudrun/terraform/stages/3-httplb-cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/.github/assets/setup_local.png` & `solutions_template-1.9.0/solutions_template/template_root/.github/assets/setup_local.png`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/.github/assets/skaffold_dev_terminal.png` & `solutions_template-1.9.0/solutions_template/template_root/.github/assets/skaffold_dev_terminal.png`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/.github/workflows/deployment_cloudrun_dev.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/deployment_cloudrun_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/.github/workflows/deployment_gke_dev.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/deployment_gke_dev.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/.github/workflows/e2e_cloudrun_api_test.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/e2e_cloudrun_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/.github/workflows/e2e_gke_api_test.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/e2e_gke_api_test.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/.github/workflows/unit_test_linter_common.yaml` & `solutions_template-1.9.0/solutions_template/template_root/.github/workflows/unit_test_linter_common.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/.pylintrc` & `solutions_template-1.9.0/solutions_template/template_root/.pylintrc`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/README.md` & `solutions_template-1.9.0/solutions_template/template_root/README.md`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/components/common/skaffold.yaml` & `solutions_template-1.9.0/solutions_template/template_root/components/common/skaffold.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/config.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/config.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/db_client.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/db_client.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/models/example.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/models/example.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/testing/bq_client_fixture.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/bq_client_fixture.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/testing/client_with_emulator.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/client_with_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/testing/firestore_emulator.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/testing/firestore_emulator.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/components/common/src/common/utils/logging_handler.py` & `solutions_template-1.9.0/solutions_template/template_root/components/common/src/common/utils/logging_handler.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/copier.yaml` & `solutions_template-1.9.0/solutions_template/template_root/copier.yaml`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/cloudbuild/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudbuild/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/cloudbuild/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudbuild/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/cloudrun/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudrun/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/cloudrun/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/cloudrun/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/compute_backend/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/compute_backend/providers.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/compute_backend/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/compute_backend/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/firebase/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/firebase/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/firebase/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/firebase/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/gke/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/gke/outputs.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/gke/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/gke/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_gce/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_gce/outputs.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_gce/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_gce/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_nginx/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_nginx/outputs.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/ingress_nginx/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/ingress_nginx/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/project_services/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/project_services/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/project_services/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/project_services/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/service_account/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/service_account/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/service_account/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/service_account/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/terraform_cicd/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/terraform_cicd/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/terraform_cicd/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/terraform_cicd/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/vpc_network/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/vpc_network/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/modules/vpc_network/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/modules/vpc_network/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/1-bootstrap/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/1-bootstrap/output.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/output.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/1-bootstrap/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/1-bootstrap/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/backend.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/firestore_setup.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/firestore_setup.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/iam.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/iam.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/main.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/main.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/outputs.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/outputs.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/providers.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/terraform.tfvars` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/terraform.tfvars`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/2-foundation/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/2-foundation/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/3-components/backend.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/backend.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/3-components/providers.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/providers.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/terraform/stages/3-components/variables.tf` & `solutions_template-1.9.0/solutions_template/template_root/terraform/stages/3-components/variables.tf`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/tests/e2e/e2e_utils.py` & `solutions_template-1.9.0/solutions_template/template_root/tests/e2e/e2e_utils.py`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/utils/init_env_vars.sh` & `solutions_template-1.9.0/solutions_template/template_root/utils/init_env_vars.sh`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/utils/setup_all.sh` & `solutions_template-1.9.0/solutions_template/template_root/utils/setup_all.sh`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/solutions_template/template_root/utils/setup_local.sh` & `solutions_template-1.9.0/solutions_template/template_root/utils/setup_local.sh`

 * *Files identical despite different names*

### Comparing `solutions_template-0.1.16/PKG-INFO` & `solutions_template-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solutions-template
-Version: 0.1.16
+Version: 1.9.0
 Summary: A solution framework to generate a project with built-in structure and modules
 Home-page: https://github.com/GoogleCloudPlatform/solutions-template
 License: Apache
 Author: Jon Chen
 Author-email: jonchen@google.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -61,17 +61,14 @@
 | Kustomize   | &gt;= v5.0.0 | https://kubectl.docs.kubernetes.io/installation/kustomize/ |
 
 ## Installing Solutions Template CLI
 
 With `pip`:
 ```
 pip install solutions-template
-
-# Alternatively, to install from PyPI-Test, run:
-pip install --index-url https://test.pypi.org/simple/ solutions-template
 ```
 
 With `pipx`:
 ```
 pip install --user pipx
 pipx install solutions-template
 ```
```

