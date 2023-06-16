# Comparing `tmp/sefazetllib-0.1.33.tar.gz` & `tmp/sefazetllib-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sefazetllib-0.1.33.tar", max compression
+gzip compressed data, was "sefazetllib-0.1.34.tar", max compression
```

## Comparing `sefazetllib-0.1.33.tar` & `sefazetllib-0.1.34.tar`

### file list

```diff
@@ -1,79 +1,78 @@
--rw-r--r--   0        0        0    10349 2023-03-22 02:02:06.498182 sefazetllib-0.1.33/LICENSE
--rw-r--r--   0        0        0     2535 2023-06-13 21:27:17.305610 sefazetllib-0.1.33/pyproject.toml
--rw-r--r--   0        0        0     3264 2023-04-09 18:51:54.608430 sefazetllib-0.1.33/README.md
--rw-r--r--   0        0        0      137 2023-03-22 11:22:30.166093 sefazetllib-0.1.33/sefazetllib/__init__.py
--rw-r--r--   0        0        0     1716 2023-03-22 11:35:33.508530 sefazetllib-0.1.33/sefazetllib/Builder.py
--rw-r--r--   0        0        0       53 2023-03-22 11:18:45.691953 sefazetllib-0.1.33/sefazetllib/config/__init__.py
--rw-r--r--   0        0        0     2415 2023-03-28 02:16:14.475807 sefazetllib-0.1.33/sefazetllib/config/CustomLogging.py
--rw-r--r--   0        0        0       37 2023-03-22 02:03:33.079166 sefazetllib-0.1.33/sefazetllib/etl/__init__.py
--rw-r--r--   0        0        0     8457 2023-06-07 14:35:59.685410 sefazetllib-0.1.33/sefazetllib/etl/ETL.py
--rw-r--r--   0        0        0      279 2023-03-22 11:23:55.081767 sefazetllib-0.1.33/sefazetllib/extract/__init__.py
--rw-r--r--   0        0        0      729 2023-03-22 11:35:33.511528 sefazetllib-0.1.33/sefazetllib/extract/Extract.py
--rw-r--r--   0        0        0     2047 2023-03-22 11:35:33.512538 sefazetllib-0.1.33/sefazetllib/extract/ExtractLocal.py
--rw-r--r--   0        0        0     2552 2023-03-24 02:29:17.874836 sefazetllib-0.1.33/sefazetllib/extract/ExtractS3.py
--rw-r--r--   0        0        0     2600 2023-03-22 11:24:35.794185 sefazetllib-0.1.33/sefazetllib/extract/ExtractSQL.py
--rw-r--r--   0        0        0     2351 2023-03-22 11:35:33.515528 sefazetllib-0.1.33/sefazetllib/extract/ExtractStorage.py
--rw-r--r--   0        0        0       91 2023-03-22 02:17:48.512311 sefazetllib-0.1.33/sefazetllib/factory/__init__.py
--rw-r--r--   0        0        0      967 2023-03-22 11:35:33.517536 sefazetllib-0.1.33/sefazetllib/factory/Factory.py
--rw-r--r--   0        0        0      272 2023-03-22 11:24:56.091205 sefazetllib-0.1.33/sefazetllib/factory/platform/__init__.py
--rw-r--r--   0        0        0      136 2023-05-03 17:55:22.831406 sefazetllib-0.1.33/sefazetllib/factory/platform/database/__init__.py
--rw-r--r--   0        0        0      749 2023-03-22 11:35:33.520527 sefazetllib-0.1.33/sefazetllib/factory/platform/database/MySQL.py
--rw-r--r--   0        0        0     4187 2023-05-16 16:42:56.445223 sefazetllib-0.1.33/sefazetllib/factory/platform/database/PostgreSQL.py
--rw-r--r--   0        0        0      380 2023-03-22 11:25:06.491132 sefazetllib-0.1.33/sefazetllib/factory/platform/DatabasePlatform.py
--rw-r--r--   0        0        0      198 2023-03-22 11:28:08.380181 sefazetllib-0.1.33/sefazetllib/factory/platform/dataframe/__init__.py
--rw-r--r--   0        0        0      272 2023-03-22 11:35:33.522527 sefazetllib-0.1.33/sefazetllib/factory/platform/dataframe/Default.py
--rw-r--r--   0        0        0     1854 2023-03-22 11:35:33.523528 sefazetllib-0.1.33/sefazetllib/factory/platform/dataframe/Pandas.py
--rw-r--r--   0        0        0     4830 2023-05-16 16:42:56.447222 sefazetllib-0.1.33/sefazetllib/factory/platform/dataframe/Spark.py
--rw-r--r--   0        0        0      297 2023-03-22 11:35:33.518538 sefazetllib-0.1.33/sefazetllib/factory/platform/Platform.py
--rw-r--r--   0        0        0     1077 2023-03-22 11:27:04.493215 sefazetllib-0.1.33/sefazetllib/factory/platform/PlatformFactory.py
--rw-r--r--   0        0        0      234 2023-03-22 11:35:33.533527 sefazetllib-0.1.33/sefazetllib/load/__init__.py
--rw-r--r--   0        0        0      711 2023-03-22 11:35:33.526527 sefazetllib-0.1.33/sefazetllib/load/Load.py
--rw-r--r--   0        0        0     2200 2023-06-07 14:35:59.690408 sefazetllib-0.1.33/sefazetllib/load/LoadLocal.py
--rw-r--r--   0        0        0     2458 2023-05-03 17:55:22.834392 sefazetllib-0.1.33/sefazetllib/load/LoadS3.py
--rw-r--r--   0        0        0     7809 2023-05-16 16:42:56.450557 sefazetllib-0.1.33/sefazetllib/load/LoadSQL.py
--rw-r--r--   0        0        0     2261 2023-03-22 11:35:33.532526 sefazetllib-0.1.33/sefazetllib/load/LoadStorage.py
--rw-r--r--   0        0        0      201 2023-03-22 02:12:37.861367 sefazetllib-0.1.33/sefazetllib/transform/__init__.py
--rw-r--r--   0        0        0     1523 2023-03-22 02:15:28.119480 sefazetllib-0.1.33/sefazetllib/transform/MinMaxLineTransform.py
--rw-r--r--   0        0        0     4445 2023-04-08 00:24:55.749710 sefazetllib-0.1.33/sefazetllib/transform/QuartileTransform.py
--rw-r--r--   0        0        0      577 2023-03-22 11:35:33.535526 sefazetllib-0.1.33/sefazetllib/transform/Transform.py
--rw-r--r--   0        0        0       46 2023-03-22 02:08:23.799891 sefazetllib-0.1.33/sefazetllib/utils/__init__.py
--rw-r--r--   0        0        0      161 2023-03-22 02:03:33.166061 sefazetllib-0.1.33/sefazetllib/utils/key/__init__.py
--rw-r--r--   0        0        0      339 2023-03-22 11:35:33.536528 sefazetllib-0.1.33/sefazetllib/utils/key/DefaultKey.py
--rw-r--r--   0        0        0      419 2023-03-22 11:35:33.537527 sefazetllib-0.1.33/sefazetllib/utils/key/Key.py
--rw-r--r--   0        0        0      775 2023-03-22 11:35:33.538526 sefazetllib-0.1.33/sefazetllib/utils/key/SurrogateKey.py
--rw-r--r--   0        0        0      234 2023-03-22 02:03:33.178225 sefazetllib-0.1.33/sefazetllib/utils/partition/__init__.py
--rw-r--r--   0        0        0     2172 2023-03-22 11:21:12.190698 sefazetllib-0.1.33/sefazetllib/utils/partition/DatePartition.py
--rw-r--r--   0        0        0      652 2023-03-22 11:21:29.374214 sefazetllib-0.1.33/sefazetllib/utils/partition/IncrementalRangePartition.py
--rw-r--r--   0        0        0      447 2023-03-22 11:35:33.539526 sefazetllib-0.1.33/sefazetllib/utils/partition/Partition.py
--rw-r--r--   0        0        0      112 2023-03-22 11:35:33.543527 sefazetllib-0.1.33/sefazetllib/validate/__init__.py
--rw-r--r--   0        0        0     7974 2023-06-13 21:27:17.306610 sefazetllib-0.1.33/sefazetllib/validate/DataValidate.py
--rw-r--r--   0        0        0      401 2023-06-07 14:35:59.694944 sefazetllib-0.1.33/sefazetllib/validate/Validate.py
--rw-r--r--   0        0        0     3675 2023-05-03 17:55:22.841468 sefazetllib-0.1.33/sefazetllibcli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 17:55:22.846732 sefazetllib-0.1.33/sefazetllibcli/config/__init__.py
--rw-r--r--   0        0        0     1153 2023-05-03 17:55:22.848772 sefazetllib-0.1.33/sefazetllibcli/config/logging.py
--rw-r--r--   0        0        0      188 2023-05-03 17:55:22.850781 sefazetllib-0.1.33/sefazetllibcli/errors/__init__.py
--rw-r--r--   0        0        0       78 2023-05-03 17:55:22.852785 sefazetllib-0.1.33/sefazetllibcli/errors/method_not_implemented.py
--rw-r--r--   0        0        0       54 2023-05-03 17:55:22.855787 sefazetllib-0.1.33/sefazetllibcli/errors/unsupported_file_extension.py
--rw-r--r--   0        0        0       90 2023-05-03 17:55:22.859397 sefazetllib-0.1.33/sefazetllibcli/errors/variable_processing_error.py
--rw-r--r--   0        0        0        0 2023-05-03 17:55:22.863453 sefazetllib-0.1.33/sefazetllibcli/generators/__init__.py
--rw-r--r--   0        0        0     6071 2023-05-03 17:55:22.866434 sefazetllib-0.1.33/sefazetllibcli/generators/etl_generator.py
--rw-r--r--   0        0        0      908 2023-05-03 17:55:22.867422 sefazetllib-0.1.33/sefazetllibcli/generators/generator.py
--rw-r--r--   0        0        0      390 2023-05-03 17:55:22.870098 sefazetllib-0.1.33/sefazetllibcli/templates/etl_template
--rw-r--r--   0        0        0        0 2023-05-03 17:55:22.871111 sefazetllib-0.1.33/sefazetllibcli/usecases/__init__.py
--rw-r--r--   0        0        0      533 2023-05-03 17:55:22.874111 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/__init__.py
--rw-r--r--   0        0        0     3582 2023-05-03 17:55:22.875119 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_etl_variable.py
--rw-r--r--   0        0        0     1158 2023-05-03 17:55:22.876120 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_extract_variable.py
--rw-r--r--   0        0        0     1014 2023-05-03 17:55:22.878655 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_imports_variable.py
--rw-r--r--   0        0        0     1174 2023-05-03 17:55:22.879699 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_key_variable.py
--rw-r--r--   0        0        0     1140 2023-05-03 17:55:22.880699 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_load_variable.py
--rw-r--r--   0        0        0     1640 2023-05-03 17:55:22.881700 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_partition_variable.py
--rw-r--r--   0        0        0     2148 2023-05-03 17:55:22.883701 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
--rw-r--r--   0        0        0     1106 2023-05-03 17:55:22.885700 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_validate_variable.py
--rw-r--r--   0        0        0      963 2023-05-03 17:55:22.888826 sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_variable.py
--rw-r--r--   0        0        0      101 2023-05-03 17:55:22.894836 sefazetllib-0.1.33/sefazetllibcli/usecases/replace_template/__init__.py
--rw-r--r--   0        0        0      996 2023-05-03 17:55:22.896797 sefazetllib-0.1.33/sefazetllibcli/usecases/replace_template/replace_etl_template.py
--rw-r--r--   0        0        0     1724 2023-05-03 17:55:22.899329 sefazetllib-0.1.33/sefazetllibcli/usecases/replace_template/replace_template.py
--rw-r--r--   0        0        0       33 2023-05-03 17:55:22.901426 sefazetllib-0.1.33/sefazetllibcli/utils/__init__.py
--rw-r--r--   0        0        0     3744 2023-05-03 17:55:22.902437 sefazetllib-0.1.33/sefazetllibcli/utils/parse_etl.py
--rw-r--r--   0        0        0     4971 1970-01-01 00:00:00.000000 sefazetllib-0.1.33/setup.py
--rw-r--r--   0        0        0     4930 1970-01-01 00:00:00.000000 sefazetllib-0.1.33/PKG-INFO
+-rwxr-xr-x   0        0        0    10173 2023-06-13 18:35:19.937294 sefazetllib-0.1.34/LICENSE
+-rwxr-xr-x   0        0        0     3159 2023-06-13 18:35:19.939794 sefazetllib-0.1.34/README.md
+-rwxr-xr-x   0        0        0     2445 2023-06-16 17:37:58.825654 sefazetllib-0.1.34/pyproject.toml
+-rwxr-xr-x   0        0        0     1663 2023-06-13 18:35:20.075553 sefazetllib-0.1.34/sefazetllib/Builder.py
+-rwxr-xr-x   0        0        0      135 2023-06-13 18:35:20.079795 sefazetllib-0.1.34/sefazetllib/__init__.py
+-rwxr-xr-x   0        0        0     2338 2023-06-13 18:35:20.087295 sefazetllib-0.1.34/sefazetllib/config/CustomLogging.py
+-rwxr-xr-x   0        0        0       52 2023-06-13 18:35:20.092794 sefazetllib-0.1.34/sefazetllib/config/__init__.py
+-rwxr-xr-x   0        0        0     8218 2023-06-13 18:35:20.099294 sefazetllib-0.1.34/sefazetllib/etl/ETL.py
+-rwxr-xr-x   0        0        0       36 2023-06-13 18:35:20.104294 sefazetllib-0.1.34/sefazetllib/etl/__init__.py
+-rwxr-xr-x   0        0        0      701 2023-06-13 18:35:20.109301 sefazetllib-0.1.34/sefazetllib/extract/Extract.py
+-rwxr-xr-x   0        0        0     1986 2023-06-13 18:35:20.113298 sefazetllib-0.1.34/sefazetllib/extract/ExtractLocal.py
+-rwxr-xr-x   0        0        0     2479 2023-06-13 18:35:20.119298 sefazetllib-0.1.34/sefazetllib/extract/ExtractS3.py
+-rwxr-xr-x   0        0        0     2521 2023-06-13 18:35:20.123828 sefazetllib-0.1.34/sefazetllib/extract/ExtractSQL.py
+-rwxr-xr-x   0        0        0     2282 2023-06-13 18:35:20.127293 sefazetllib-0.1.34/sefazetllib/extract/ExtractStorage.py
+-rwxr-xr-x   0        0        0      274 2023-06-13 18:35:20.131294 sefazetllib-0.1.34/sefazetllib/extract/__init__.py
+-rwxr-xr-x   0        0        0      949 2023-06-13 18:35:20.137294 sefazetllib-0.1.34/sefazetllib/factory/Factory.py
+-rwxr-xr-x   0        0        0       89 2023-06-13 18:35:20.141795 sefazetllib-0.1.34/sefazetllib/factory/__init__.py
+-rwxr-xr-x   0        0        0      362 2023-06-13 18:35:20.148794 sefazetllib-0.1.34/sefazetllib/factory/platform/DatabasePlatform.py
+-rwxr-xr-x   0        0        0      281 2023-06-13 18:35:20.156294 sefazetllib-0.1.34/sefazetllib/factory/platform/Platform.py
+-rwxr-xr-x   0        0        0     1049 2023-06-13 18:35:20.161796 sefazetllib-0.1.34/sefazetllib/factory/platform/PlatformFactory.py
+-rwxr-xr-x   0        0        0      268 2023-06-13 18:35:20.166794 sefazetllib-0.1.34/sefazetllib/factory/platform/__init__.py
+-rwxr-xr-x   0        0        0      723 2023-06-13 18:35:20.184341 sefazetllib-0.1.34/sefazetllib/factory/platform/database/Mysql.py
+-rwxr-xr-x   0        0        0     4069 2023-06-13 18:35:20.190294 sefazetllib-0.1.34/sefazetllib/factory/platform/database/PostgreSQL.py
+-rwxr-xr-x   0        0        0      134 2023-06-13 18:35:20.196307 sefazetllib-0.1.34/sefazetllib/factory/platform/database/__init__.py
+-rwxr-xr-x   0        0        0      259 2023-06-13 18:35:20.207294 sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/Default.py
+-rwxr-xr-x   0        0        0     1793 2023-06-13 18:35:20.214794 sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/Pandas.py
+-rwxr-xr-x   0        0        0     4679 2023-06-13 18:35:20.219293 sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/Spark.py
+-rwxr-xr-x   0        0        0      195 2023-06-13 18:35:20.224295 sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/__init__.py
+-rwxr-xr-x   0        0        0      683 2023-06-13 18:35:20.230795 sefazetllib-0.1.34/sefazetllib/load/Load.py
+-rwxr-xr-x   0        0        0     2134 2023-06-13 18:35:20.235296 sefazetllib-0.1.34/sefazetllib/load/LoadLocal.py
+-rwxr-xr-x   0        0        0     2386 2023-06-13 18:35:20.238796 sefazetllib-0.1.34/sefazetllib/load/LoadS3.py
+-rwxr-xr-x   0        0        0     7601 2023-06-13 18:35:20.242296 sefazetllib-0.1.34/sefazetllib/load/LoadSQL.py
+-rwxr-xr-x   0        0        0     2194 2023-06-13 18:35:20.246796 sefazetllib-0.1.34/sefazetllib/load/LoadStorage.py
+-rwxr-xr-x   0        0        0      229 2023-06-13 18:35:20.250295 sefazetllib-0.1.34/sefazetllib/load/__init__.py
+-rwxr-xr-x   0        0        0     1471 2023-06-13 18:35:20.255795 sefazetllib-0.1.34/sefazetllib/transform/MinMaxLineTransform.py
+-rwxr-xr-x   0        0        0     4331 2023-06-13 18:35:20.259795 sefazetllib-0.1.34/sefazetllib/transform/QuartileTransform.py
+-rwxr-xr-x   0        0        0      552 2023-06-13 18:35:20.263795 sefazetllib-0.1.34/sefazetllib/transform/Transform.py
+-rwxr-xr-x   0        0        0      198 2023-06-13 18:35:20.267294 sefazetllib-0.1.34/sefazetllib/transform/__init__.py
+-rwxr-xr-x   0        0        0       45 2023-06-13 18:35:20.272796 sefazetllib-0.1.34/sefazetllib/utils/__init__.py
+-rwxr-xr-x   0        0        0      325 2023-06-13 18:35:20.281294 sefazetllib-0.1.34/sefazetllib/utils/key/DefaultKey.py
+-rwxr-xr-x   0        0        0      400 2023-06-13 18:35:20.287793 sefazetllib-0.1.34/sefazetllib/utils/key/Key.py
+-rwxr-xr-x   0        0        0      747 2023-06-13 18:35:20.291793 sefazetllib-0.1.34/sefazetllib/utils/key/SurrogateKey.py
+-rwxr-xr-x   0        0        0      158 2023-06-13 18:35:20.295794 sefazetllib-0.1.34/sefazetllib/utils/key/__init__.py
+-rwxr-xr-x   0        0        0     2097 2023-06-13 18:35:20.304797 sefazetllib-0.1.34/sefazetllib/utils/partition/DatePartition.py
+-rwxr-xr-x   0        0        0      627 2023-06-13 18:35:20.310298 sefazetllib-0.1.34/sefazetllib/utils/partition/IncrementalRangePartition.py
+-rwxr-xr-x   0        0        0      425 2023-06-13 18:35:20.314794 sefazetllib-0.1.34/sefazetllib/utils/partition/Partition.py
+-rwxr-xr-x   0        0        0      229 2023-06-13 18:35:20.318794 sefazetllib-0.1.34/sefazetllib/utils/partition/__init__.py
+-rwxr-xr-x   0        0        0     7729 2023-06-16 17:37:58.844408 sefazetllib-0.1.34/sefazetllib/validate/DataValidate.py
+-rwxr-xr-x   0        0        0      383 2023-06-13 18:35:20.330793 sefazetllib-0.1.34/sefazetllib/validate/Validate.py
+-rwxr-xr-x   0        0        0      110 2023-06-13 18:35:20.333793 sefazetllib-0.1.34/sefazetllib/validate/__init__.py
+-rwxr-xr-x   0        0        0     3551 2023-06-13 18:35:20.337293 sefazetllib-0.1.34/sefazetllibcli/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 18:35:20.341293 sefazetllib-0.1.34/sefazetllibcli/config/__init__.py
+-rwxr-xr-x   0        0        0     1117 2023-06-13 18:35:20.345293 sefazetllib-0.1.34/sefazetllibcli/config/logging.py
+-rwxr-xr-x   0        0        0      185 2023-06-13 18:35:20.350794 sefazetllib-0.1.34/sefazetllibcli/errors/__init__.py
+-rwxr-xr-x   0        0        0       76 2023-06-13 18:35:20.354794 sefazetllib-0.1.34/sefazetllibcli/errors/method_not_implemented.py
+-rwxr-xr-x   0        0        0       52 2023-06-13 18:35:20.358761 sefazetllib-0.1.34/sefazetllibcli/errors/unsupported_file_extension.py
+-rwxr-xr-x   0        0        0       88 2023-06-13 18:35:20.362818 sefazetllib-0.1.34/sefazetllibcli/errors/variable_processing_error.py
+-rwxr-xr-x   0        0        0        0 2023-06-13 18:35:20.367793 sefazetllib-0.1.34/sefazetllibcli/generators/__init__.py
+-rwxr-xr-x   0        0        0     5897 2023-06-13 18:35:20.371294 sefazetllib-0.1.34/sefazetllibcli/generators/etl_generator.py
+-rwxr-xr-x   0        0        0      884 2023-06-13 18:35:20.375497 sefazetllib-0.1.34/sefazetllibcli/generators/generator.py
+-rwxr-xr-x   0        0        0      374 2023-06-13 18:35:20.383794 sefazetllib-0.1.34/sefazetllibcli/templates/etl_template
+-rwxr-xr-x   0        0        0        0 2023-06-13 18:35:20.388794 sefazetllib-0.1.34/sefazetllibcli/usecases/__init__.py
+-rwxr-xr-x   0        0        0      524 2023-06-13 18:35:20.398795 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/__init__.py
+-rwxr-xr-x   0        0        0     3484 2023-06-13 18:35:20.405793 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_etl_variable.py
+-rwxr-xr-x   0        0        0     1128 2023-06-13 18:35:20.410293 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_extract_variable.py
+-rwxr-xr-x   0        0        0      986 2023-06-13 18:35:20.414295 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_imports_variable.py
+-rwxr-xr-x   0        0        0     1142 2023-06-13 18:35:20.419294 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_key_variable.py
+-rwxr-xr-x   0        0        0     1110 2023-06-13 18:35:20.423301 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_load_variable.py
+-rwxr-xr-x   0        0        0     1595 2023-06-13 18:35:20.428294 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_partition_variable.py
+-rwxr-xr-x   0        0        0     2086 2023-06-13 18:35:20.432793 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
+-rwxr-xr-x   0        0        0     1074 2023-06-13 18:35:20.436794 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_validate_variable.py
+-rwxr-xr-x   0        0        0      935 2023-06-13 18:35:20.440793 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_variable.py
+-rwxr-xr-x   0        0        0       99 2023-06-13 18:35:20.448793 sefazetllib-0.1.34/sefazetllibcli/usecases/replace_template/__init__.py
+-rwxr-xr-x   0        0        0      963 2023-06-13 18:35:20.455293 sefazetllib-0.1.34/sefazetllibcli/usecases/replace_template/replace_etl_template.py
+-rwxr-xr-x   0        0        0     1678 2023-06-13 18:35:20.460293 sefazetllib-0.1.34/sefazetllibcli/usecases/replace_template/replace_template.py
+-rwxr-xr-x   0        0        0       32 2023-06-13 18:35:20.464793 sefazetllib-0.1.34/sefazetllibcli/utils/__init__.py
+-rwxr-xr-x   0        0        0     3631 2023-06-13 18:35:20.468794 sefazetllib-0.1.34/sefazetllibcli/utils/parse_etl.py
+-rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 sefazetllib-0.1.34/PKG-INFO
```

### Comparing `sefazetllib-0.1.33/LICENSE` & `sefazetllib-0.1.34/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
```

### Comparing `sefazetllib-0.1.33/README.md` & `sefazetllib-0.1.34/README.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-# sefazetllib
-
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
----
-
-**Documentation**: [https://main.d32to2oidohzrl.amplifyapp.com/](https://main.d32to2oidohzrl.amplifyapp.com/)
-
-**Source code**: [AWS CodeCommit](https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1)
-
----
-
-**sefazetllib** is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
-
-## Features
-
-- Easy to use and understand library for constructing ETL/ELT pipelines.
-- Compatibility with popular data processing frameworks, such as [pandas](https://pandas.pydata.org/) and [PySpark](https://spark.apache.org/).
-- Support for file formats such as CSV and Parquet.
-- Provides the ability to extract, transform and load data with customizable configurations.
-
-## Requirements
-
-**sefazetllib** requires the following to run:
-
-- [Python](https://www.python.org/) 3.7.1+
-- [pandas](https://pandas.pydata.org/) 1.3+
-- [PyArrow](https://arrow.apache.org/) 6.0+
-- [PySpark](https://spark.apache.org/) 3.0+
-- [PyDeequ](https://pydeequ.readthedocs.io/) 1.0+
-- [Boto3](https://github.com/boto/boto3) 1.24+
-
-## Installation
-
-Use [pip](https://pip.pypa.io/en/stable/) to install **sefazetllib**:
-
-```bash
-pip install sefazetllib
-```
-
-## Usage
-
-Here is an example of how to use the **sefazetllib**:
-
-```Python
-from typing import Tuple
-
-from pandas import DataFrame
-
-from sefazetllib import Builder
-from sefazetllib.etl import ETL
-from sefazetllib.extract import ExtractLocal
-from sefazetllib.factory.platform import PlatformFactory
-from sefazetllib.load import LoadLocal
-from sefazetllib.transform import Transform
-from sefazetllib.utils.key import SurrogateKey
-
-
-@Builder
-class TestingDataFrame(Transform):
-    def execute(self) -> Tuple[str, DataFrame]:
-        return (
-            "dataframe",
-            DataFrame(
-                [["tom", 10], ["nick", 15], ["juli", 14]], columns=["Name", "Age"]
-            ),
-        )
-
-
-(
-    ETL()
-    .setPlatform(PlatformFactory("Pandas").create(name="test_pandas"))
-    .transform(TestingDataFrame)
-    .load(
-        LoadLocal()
-        .setFileFormat("parquet")
-        .setEntity("load_test")
-        .setMode("overwrite")
-        .setReference("dataframe")
-        .setDuplicates(True)
-        .setKey(SurrogateKey().setColumns(["Name", "Age"]).setDistribute(False))
-    )
-    .extract(
-        ExtractLocal()
-        .setFileFormat("parquet")
-        .setUrl("load_test.parquet")
-        .setReference("extract_test")
-    )
-)
-```
-
-## Testing
-
-To run the unit tests, run the following command:
-
-```bash
-py -m unittest tests/main.py -v
-```
-
-## License
-
-**sefazetllib** is released under the [Apache-2.0](/LICENSE).
+# sefazetllib
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+---
+
+**Documentation**: [https://main.d32to2oidohzrl.amplifyapp.com/](https://main.d32to2oidohzrl.amplifyapp.com/)
+
+**Source code**: [AWS CodeCommit](https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1)
+
+---
+
+**sefazetllib** is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
+
+## Features
+
+- Easy to use and understand library for constructing ETL/ELT pipelines.
+- Compatibility with popular data processing frameworks, such as [pandas](https://pandas.pydata.org/) and [PySpark](https://spark.apache.org/).
+- Support for file formats such as CSV and Parquet.
+- Provides the ability to extract, transform and load data with customizable configurations.
+
+## Requirements
+
+**sefazetllib** requires the following to run:
+
+- [Python](https://www.python.org/) 3.7.1+
+- [pandas](https://pandas.pydata.org/) 1.3+
+- [PyArrow](https://arrow.apache.org/) 6.0+
+- [PySpark](https://spark.apache.org/) 3.0+
+- [PyDeequ](https://pydeequ.readthedocs.io/) 1.0+
+- [Boto3](https://github.com/boto/boto3) 1.24+
+
+## Installation
+
+Use [pip](https://pip.pypa.io/en/stable/) to install **sefazetllib**:
+
+```bash
+pip install sefazetllib
+```
+
+## Usage
+
+Here is an example of how to use the **sefazetllib**:
+
+```Python
+from typing import Tuple
+
+from pandas import DataFrame
+
+from sefazetllib import Builder
+from sefazetllib.etl import ETL
+from sefazetllib.extract import ExtractLocal
+from sefazetllib.factory.platform import PlatformFactory
+from sefazetllib.load import LoadLocal
+from sefazetllib.transform import Transform
+from sefazetllib.utils.key import SurrogateKey
+
+
+@Builder
+class TestingDataFrame(Transform):
+    def execute(self) -> Tuple[str, DataFrame]:
+        return (
+            "dataframe",
+            DataFrame(
+                [["tom", 10], ["nick", 15], ["juli", 14]], columns=["Name", "Age"]
+            ),
+        )
+
+
+(
+    ETL()
+    .setPlatform(PlatformFactory("Pandas").create(name="test_pandas"))
+    .transform(TestingDataFrame)
+    .load(
+        LoadLocal()
+        .setFileFormat("parquet")
+        .setEntity("load_test")
+        .setMode("overwrite")
+        .setReference("dataframe")
+        .setDuplicates(True)
+        .setKey(SurrogateKey().setColumns(["Name", "Age"]).setDistribute(False))
+    )
+    .extract(
+        ExtractLocal()
+        .setFileFormat("parquet")
+        .setUrl("load_test.parquet")
+        .setReference("extract_test")
+    )
+)
+```
+
+## Testing
+
+To run the unit tests, run the following command:
+
+```bash
+py -m unittest tests/main.py -v
+```
+
+## License
+
+**sefazetllib** is released under the [Apache-2.0](/LICENSE).
```

### Comparing `sefazetllib-0.1.33/sefazetllib/Builder.py` & `sefazetllib-0.1.34/sefazetllib/Builder.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from dataclasses import dataclass, field
-
-
-class Builder:
-    """A builder class that creates instances of a given dataclass model and sets values
-    for its non-private fields through dynamically created setter methods.
-    """
-
-    def __init__(self, model) -> None:
-        self.model = dataclass(model)
-        self.instance = None
-
-    def __call__(self):
-        """Creates an instance of the dataclass model and sets its non-private fields using
-        dynamically created setter methods.
-
-        Returns:
-            The created instance of the dataclass model.
-        """
-        self.instance = self.model()
-        self.add_setters()
-        self.instance.setup()
-        return self.instance
-
-    def add_setters(self) -> None:
-        """Adds setter methods to the instance of the dataclass model for each of its
-        non-private fields.
-        """
-        keys = [
-            {"name": field.name, "type": field.type}
-            for field in self.model.__dataclass_fields__.values()
-            if field.name[0] != "_"
-        ]
-
-        for key in keys:
-            name: str = key["name"].replace("_", " ").title().replace(" ", "")
-            setattr(self.instance, f"set{name}", self.func(key))
-
-    def func(self, key):
-        """Returns a setter function for a given field.
-
-        Parameters:
-            key: The name and type of the field.
-
-        Returns:
-            A setter function that sets the value of the field in the instance of the dataclass model and returns the instance.
-        """
-
-        def ex(value):
-            setattr(self.instance, key["name"], value)
-            return self.instance
-
-        return ex
+from dataclasses import dataclass, field
+
+
+class Builder:
+    """A builder class that creates instances of a given dataclass model and sets values
+    for its non-private fields through dynamically created setter methods.
+    """
+
+    def __init__(self, model) -> None:
+        self.model = dataclass(model)
+        self.instance = None
+
+    def __call__(self):
+        """Creates an instance of the dataclass model and sets its non-private fields using
+        dynamically created setter methods.
+
+        Returns:
+            The created instance of the dataclass model.
+        """
+        self.instance = self.model()
+        self.add_setters()
+        self.instance.setup()
+        return self.instance
+
+    def add_setters(self) -> None:
+        """Adds setter methods to the instance of the dataclass model for each of its
+        non-private fields.
+        """
+        keys = [
+            {"name": field.name, "type": field.type}
+            for field in self.model.__dataclass_fields__.values()
+            if field.name[0] != "_"
+        ]
+
+        for key in keys:
+            name: str = key["name"].replace("_", " ").title().replace(" ", "")
+            setattr(self.instance, f"set{name}", self.func(key))
+
+    def func(self, key):
+        """Returns a setter function for a given field.
+
+        Parameters:
+            key: The name and type of the field.
+
+        Returns:
+            A setter function that sets the value of the field in the instance of the dataclass model and returns the instance.
+        """
+
+        def ex(value):
+            setattr(self.instance, key["name"], value)
+            return self.instance
+
+        return ex
```

### Comparing `sefazetllib-0.1.33/sefazetllib/config/CustomLogging.py` & `sefazetllib-0.1.34/sefazetllib/config/CustomLogging.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from logging import (
-    CRITICAL,
-    DEBUG,
-    ERROR,
-    INFO,
-    WARNING,
-    Filter,
-    Formatter,
-    LogRecord,
-    StreamHandler,
-    getLogger,
-)
-from typing import Dict
-from uuid import uuid4
-
-
-class RequestIdFilter(Filter):
-    """RequestIdFilter is a custom logging filter that adds a unique request ID to each log record.
-    The request ID is generated using the UUID library and is added to the log record as the 'request_id' attribute.
-    """
-
-    # def __init__(self, name="", id=uuid4()) -> None:
-    #     super().__init__(name)
-    #     self.id = id
-    def __init__(self) -> None:
-        self.id = uuid4()
-
-    def filter(self, record: LogRecord) -> bool:
-        """Filter method adds a unique request ID to each log record.
-
-        Parameters:
-            record (LogRecord): The log record being processed.
-
-        Returns:
-            bool: Always returns True to indicate that the log record should be processed.
-        """
-        # record.request_name = self.name
-        record.request_id = str(self.id)
-        return True
-
-
-class LogColorFormatter(Formatter):
-    """LogColorFormatter is a custom logging formatter that formats log records with color coding for different log levels.
-    The log format includes the timestamp, request ID, log level, and log message.
-    """
-
-    colors: Dict[int, str] = {
-        DEBUG: "\x1b[30m",
-        INFO: "\x1b[36m",
-        WARNING: "\x1b[33m",
-        ERROR: "\x1b[31m",
-        CRITICAL: "\x1b[31;1m",
-    }
-
-    template: str = "\x1b[32m[%(asctime)s] \x1b[30m[%(request_id)s] {level_color}%(levelname)s \x1b[0m%(message)s"
-
-    def format(self, record: LogRecord) -> str:
-        """Format method that formats a log record with color coding for different log levels.
-
-        Parameters:
-            record (LogRecord): The log record being processed.
-
-        Returns:
-            str: the formatted log record.
-        """
-        # color: Optional[str] = self.colors.get(record.levelno)
-        # log_format: str = self.template.format(level_color=color)
-        log_format: str = "[%(asctime)s] [%(request_id)s] %(levelname)s %(message)s"
-        return Formatter(log_format).format(record)
-
-
-logger = getLogger("sefazetllib")
-logger.setLevel(DEBUG)
-
-handler = StreamHandler()
-handler.setFormatter(LogColorFormatter())
-logger.addHandler(handler)
+from logging import (
+    CRITICAL,
+    DEBUG,
+    ERROR,
+    INFO,
+    WARNING,
+    Filter,
+    Formatter,
+    LogRecord,
+    StreamHandler,
+    getLogger,
+)
+from typing import Dict
+from uuid import uuid4
+
+
+class RequestIdFilter(Filter):
+    """RequestIdFilter is a custom logging filter that adds a unique request ID to each log record.
+    The request ID is generated using the UUID library and is added to the log record as the 'request_id' attribute.
+    """
+
+    # def __init__(self, name="", id=uuid4()) -> None:
+    #     super().__init__(name)
+    #     self.id = id
+    def __init__(self) -> None:
+        self.id = uuid4()
+
+    def filter(self, record: LogRecord) -> bool:
+        """Filter method adds a unique request ID to each log record.
+
+        Parameters:
+            record (LogRecord): The log record being processed.
+
+        Returns:
+            bool: Always returns True to indicate that the log record should be processed.
+        """
+        # record.request_name = self.name
+        record.request_id = str(self.id)
+        return True
+
+
+class LogColorFormatter(Formatter):
+    """LogColorFormatter is a custom logging formatter that formats log records with color coding for different log levels.
+    The log format includes the timestamp, request ID, log level, and log message.
+    """
+
+    colors: Dict[int, str] = {
+        DEBUG: "\x1b[30m",
+        INFO: "\x1b[36m",
+        WARNING: "\x1b[33m",
+        ERROR: "\x1b[31m",
+        CRITICAL: "\x1b[31;1m",
+    }
+
+    template: str = "\x1b[32m[%(asctime)s] \x1b[30m[%(request_id)s] {level_color}%(levelname)s \x1b[0m%(message)s"
+
+    def format(self, record: LogRecord) -> str:
+        """Format method that formats a log record with color coding for different log levels.
+
+        Parameters:
+            record (LogRecord): The log record being processed.
+
+        Returns:
+            str: the formatted log record.
+        """
+        # color: Optional[str] = self.colors.get(record.levelno)
+        # log_format: str = self.template.format(level_color=color)
+        log_format: str = "[%(asctime)s] [%(request_id)s] %(levelname)s %(message)s"
+        return Formatter(log_format).format(record)
+
+
+logger = getLogger("sefazetllib")
+logger.setLevel(DEBUG)
+
+handler = StreamHandler()
+handler.setFormatter(LogColorFormatter())
+logger.addHandler(handler)
```

### Comparing `sefazetllib-0.1.33/sefazetllib/extract/ExtractLocal.py` & `sefazetllib-0.1.34/sefazetllib/load/LoadStorage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,67 @@
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.extract.Extract import Extract
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-
-
-@Builder
-class ExtractLocal(Extract):
-    platform: Platform = field(default_factory=Default)
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    repository: str = field(default="")
-    url: str = field(default="")
-    partition: List[str] = field(default_factory=list)
-    reference: str = field(default="")
-    columns: List = field(default_factory=list)
-    duplicates: bool = field(default=False)
-    optional: bool = field(default=False)
-
-    def build_connection_string(self):
-        if self.partition != []:
-            for partition in self.partition:
-                self.setUrl(f"{self.url}/{partition}")
-
-        return self.url
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.repository == "":
-            self.setRepository(kwargs["repository"])
-
-        url = self.build_connection_string()
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.extractRepository:
-                self.setRepository(args.extractRepository)
-
-            if args.extractPartitions:
-                self.setPartition(args.extractPartitions)
-
-            if args.extractUrl:
-                url = args.extractUrl
-
-        return (
-            self.reference,
-            self.platform.read(
-                file_format=self.file_format,
-                format_properties=self.format_properties,
-                repository=self.repository,
-                url=url,
-                reference=self.reference,
-                columns=self.columns,
-                duplicates=self.duplicates,
-                optional=self.optional,
-            ),
-        )
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.load.Load import Load
+from sefazetllib.utils.key import DefaultKey, Key
+
+
+@Builder
+class LoadStorage(Load):
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
+    reference: str = field(default="")
+    url: str = field(default="")
+    repository: str = field(default="")
+    layer: str = field(default="")
+    schema: str = field(default="")
+    entity: str = field(default="")
+    mode: str = field(default="")
+    df_writer: Any = field(default="")
+    duplicates: bool = field(default=False)
+    key: Key = field(default=DefaultKey())
+    columns: List = field(default_factory=list)
+    protocol: str = field(default="")
+
+    def build_connection_string(self):
+        self.url = f"{self.protocol}://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
+        return self.url
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        if self.repository == "":
+            self.setRepository(kwargs["repository"])
+
+        url = self.build_connection_string()
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.loadRepository:
+                self.setRepository(args.loadRepository)
+
+            if args.loadUrl:
+                url = args.loadUrl
+
+        sk_name = f"SK_{self.entity}"
+        if "/" in self.entity:
+            entity = self.entity.split("/")[1]
+            sk_name = f"SK_{entity}"
+
+        return (
+            self.reference,
+            self.platform.load(
+                df=self.df_writer,
+                sk_name=sk_name,
+                key=self.key,
+                columns=self.columns,
+                duplicates=self.duplicates,
+                file_format=self.file_format,
+                format_properties=self.format_properties,
+                url=url,
+                mode=self.mode,
+            ),
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllib/extract/ExtractS3.py` & `sefazetllib-0.1.34/sefazetllib/extract/ExtractS3.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import warnings
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.extract.Extract import Extract
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-
-
-@Builder
-class ExtractS3(Extract):
-    warnings.warn(
-        "The 'ExtractS3' class is deprecated. Please use the 'ExtractStorage' class with the protocol parameter (e.g., 's3a')."
-    )
-    platform: Platform = field(default=Default())
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    repository: str = field(default="")
-    layer: str = field(default="")
-    schema: str = field(default="")
-    entity: str = field(default="")
-    url: str = field(default="")
-    partition: List[str] = field(default_factory=list)
-    etl_partition: bool = field(default=False)
-    reference: str = field(default="")
-    duplicates: bool = field(default=False)
-    columns: List[str] = field(default_factory=list)
-    optional: bool = field(default=False)
-
-    def build_connection_string(self):
-        self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
-
-        if self.partition != []:
-            for partition in self.partition:
-                self.setUrl(f"{self.url}/{partition}")
-
-        return self.url
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        local_repository = self.repository
-        if local_repository == "":
-            self.setRepository(kwargs["repository"])
-            
-        if self.etl_partition:
-            self.setPartition(kwargs["partition"].get())
-
-        url = self.build_connection_string()
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.extractRepository and local_repository == "":
-                self.setRepository(args.extractRepository)
-
-            if args.extractPartitions:
-                self.setPartition(args.extractPartitions)
-
-            if args.extractUrl:
-                url = args.extractUrl
-
-        return (
-            self.reference,
-            self.platform.read(
-                file_format=self.file_format,
-                format_properties=self.format_properties,
-                url=url,
-                duplicates=self.duplicates,
-                columns=self.columns,
-                optional=self.optional,
-            ),
-        )
+import warnings
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.extract.Extract import Extract
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+
+
+@Builder
+class ExtractS3(Extract):
+    warnings.warn(
+        "The 'ExtractS3' class is deprecated. Please use the 'ExtractStorage' class with the protocol parameter (e.g., 's3a')."
+    )
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
+    repository: str = field(default="")
+    layer: str = field(default="")
+    schema: str = field(default="")
+    entity: str = field(default="")
+    url: str = field(default="")
+    partition: List[str] = field(default_factory=list)
+    etl_partition: bool = field(default=False)
+    reference: str = field(default="")
+    duplicates: bool = field(default=False)
+    columns: List[str] = field(default_factory=list)
+    optional: bool = field(default=False)
+
+    def build_connection_string(self):
+        self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
+
+        if self.partition != []:
+            for partition in self.partition:
+                self.setUrl(f"{self.url}/{partition}")
+
+        return self.url
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        local_repository = self.repository
+        if local_repository == "":
+            self.setRepository(kwargs["repository"])
+            
+        if self.etl_partition:
+            self.setPartition(kwargs["partition"].get())
+
+        url = self.build_connection_string()
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.extractRepository and local_repository == "":
+                self.setRepository(args.extractRepository)
+
+            if args.extractPartitions:
+                self.setPartition(args.extractPartitions)
+
+            if args.extractUrl:
+                url = args.extractUrl
+
+        return (
+            self.reference,
+            self.platform.read(
+                file_format=self.file_format,
+                format_properties=self.format_properties,
+                url=url,
+                duplicates=self.duplicates,
+                columns=self.columns,
+                optional=self.optional,
+            ),
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllib/extract/ExtractSQL.py` & `sefazetllib-0.1.34/sefazetllib/extract/ExtractStorage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,69 @@
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.extract.Extract import Extract
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.factory.platform.PlatformFactory import PlatformFactory
-
-
-@Builder
-class ExtractSQL(Extract):
-    platform: Platform = field(default=Default())
-    format: str = field(default="jdbc")
-    operator: str = field(default=":")
-    host: str = field(default="")
-    port: int = field(default=0)
-    database: str = field(default="")
-    instance: str = field(default="")
-    driver: str = field(default="")
-    schema: str = field(default="")
-    table: str = field(default="")
-    authentication: Dict[str, Any] = field(default_factory=dict)
-    url: str = field(default="")
-    reference: str = field(default="")
-    columns: List[str] = field(default_factory=list)
-    optional: bool = field(default=False)
-    duplicates: bool = field(default=False)
-
-    def __build_properties(self):
-        self.properties = {
-            "database": self.database,
-            "driver": self.driver,
-            "user": self.authentication["user"],
-            "password": self.authentication["password"],
-            "dbtable": self.table,
-            "url": self.url,
-        }
-
-        return self.properties
-
-    def build_connection_string(self):
-        platform_db = PlatformFactory(self.database).create(
-            name="get url jdbc",
-        )
-        self.url = platform_db.get_url(
-            format=self.format,
-            operator=self.operator,
-            database=self.database,
-            host=self.host,
-            instance=self.instance,
-            schema=self.schema,
-            port=self.port,
-        )
-
-        self.table = platform_db.get_table_name(table=self.table, schema=self.schema)
-
-        return self.url
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        url = self.build_connection_string()
-        properties = self.__build_properties()
-
-        if kwargs:
-            args = kwargs["args"]
-
-            if args.extractUrl:
-                url = args.extractUrl
-
-        return self.reference, self.platform.read(
-            format=self.format,
-            url=url,
-            format_properties=properties,
-            optional=self.optional,
-            columns=self.columns,
-            duplicates=self.duplicates,
-        )
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.extract.Extract import Extract
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+
+
+@Builder
+class ExtractStorage(Extract):
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
+    repository: str = field(default="")
+    layer: str = field(default="")
+    schema: str = field(default="")
+    entity: str = field(default="")
+    url: str = field(default="")
+    partition: List[str] = field(default_factory=list)
+    etl_partition: bool = field(default=False)
+    reference: str = field(default="")
+    duplicates: bool = field(default=False)
+    columns: List[str] = field(default_factory=list)
+    optional: bool = field(default=False)
+    protocol: str = field(default="")
+
+    def build_connection_string(self):
+        self.url = f"{self.protocol}://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
+
+        if self.partition != []:
+            for partition in self.partition:
+                self.setUrl(f"{self.url}/{partition}")
+
+        return self.url
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        if self.repository == "":
+            self.setRepository(kwargs["repository"])
+
+        if self.etl_partition:
+            self.setPartition(kwargs["partition"].get())
+
+        url = self.build_connection_string()
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.extractRepository:
+                self.setRepository(args.extractRepository)
+
+            if args.extractPartitions:
+                self.setPartition(args.extractPartitions)
+
+            if args.extractUrl:
+                url = args.extractUrl
+
+        return (
+            self.reference,
+            self.platform.read(
+                file_format=self.file_format,
+                format_properties=self.format_properties,
+                url=url,
+                duplicates=self.duplicates,
+                columns=self.columns,
+                optional=self.optional,
+            ),
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllib/extract/ExtractStorage.py` & `sefazetllib-0.1.34/sefazetllib/load/LoadLocal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,66 @@
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.extract.Extract import Extract
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-
-
-@Builder
-class ExtractStorage(Extract):
-    platform: Platform = field(default=Default())
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    repository: str = field(default="")
-    layer: str = field(default="")
-    schema: str = field(default="")
-    entity: str = field(default="")
-    url: str = field(default="")
-    partition: List[str] = field(default_factory=list)
-    etl_partition: bool = field(default=False)
-    reference: str = field(default="")
-    duplicates: bool = field(default=False)
-    columns: List[str] = field(default_factory=list)
-    optional: bool = field(default=False)
-    protocol: str = field(default="")
-
-    def build_connection_string(self):
-        self.url = f"{self.protocol}://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
-
-        if self.partition != []:
-            for partition in self.partition:
-                self.setUrl(f"{self.url}/{partition}")
-
-        return self.url
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.repository == "":
-            self.setRepository(kwargs["repository"])
-
-        if self.etl_partition:
-            self.setPartition(kwargs["partition"].get())
-
-        url = self.build_connection_string()
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.extractRepository:
-                self.setRepository(args.extractRepository)
-
-            if args.extractPartitions:
-                self.setPartition(args.extractPartitions)
-
-            if args.extractUrl:
-                url = args.extractUrl
-
-        return (
-            self.reference,
-            self.platform.read(
-                file_format=self.file_format,
-                format_properties=self.format_properties,
-                url=url,
-                duplicates=self.duplicates,
-                columns=self.columns,
-                optional=self.optional,
-            ),
-        )
+import os
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.load.Load import Load
+from sefazetllib.utils.key import DefaultKey, Key
+
+
+@Builder
+class LoadLocal(Load):
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
+    reference: str = field(default="")
+    url: str = field(default="")
+    repository: str = field(default="")
+    entity: str = field(default="")
+    mode: str = field(default="")
+    df_writer: Any = field(default="")
+    duplicates: bool = field(default=False)
+    key: Key = field(default=DefaultKey())
+    columns: List = field(default_factory=list)
+    load_date: bool = field(default=True)
+
+    def build_connection_string(self):
+        return f"{os.getcwd()}/{self.entity}.{self.file_format}"
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        if self.repository == "":
+            self.setRepository(kwargs["repository"])
+
+        self.url = self.build_connection_string()
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.loadRepository:
+                self.setRepository(args.loadRepository)
+
+            if args.loadUrl:
+                self.url = args.loadUrl
+
+        sk_name = f"SK_{self.entity}"
+        if "/" in self.entity:
+            entity = self.entity.split("/")[1]
+            sk_name = f"SK_{entity}"
+
+        return (
+            self.reference,
+            self.platform.load(
+                df=self.df_writer,
+                sk_name=sk_name,
+                key=self.key,
+                columns=self.columns,
+                duplicates=self.duplicates,
+                file_format=self.file_format,
+                format_properties=self.format_properties,
+                url=self.url,
+                mode=self.mode,
+                load_date=self.load_date,
+            ),
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllib/factory/Factory.py` & `sefazetllib-0.1.34/sefazetllib/factory/Factory.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from abc import ABC, abstractmethod
-
-
-class Creator(ABC):
-    """The Creator class declares the factory method that is supposed to return an object of a Platform class. The Creator's subclasses usually provide the implementation of this method."""
-
-    @abstractmethod
-    def factory_method(self):
-        """Note that the Creator may also provide some default implementation of the factory method."""
-        pass
-
-    def execute(self, **kwargs):
-        """Also note that, despite its name, the Creator's primary responsibility is not creating products. Usually, it contains some core business logic that relies on Platform objects, returned by the factory method.  Subclasses can indirectly change that business logic by overriding the factory method and returning a different type of product from it.
-
-        Parameters:
-            **kwargs: Keyword arguments for the execute method.
-        """
-        return self.factory_method(**kwargs)
+from abc import ABC, abstractmethod
+
+
+class Creator(ABC):
+    """The Creator class declares the factory method that is supposed to return an object of a Platform class. The Creator's subclasses usually provide the implementation of this method."""
+
+    @abstractmethod
+    def factory_method(self):
+        """Note that the Creator may also provide some default implementation of the factory method."""
+        pass
+
+    def execute(self, **kwargs):
+        """Also note that, despite its name, the Creator's primary responsibility is not creating products. Usually, it contains some core business logic that relies on Platform objects, returned by the factory method.  Subclasses can indirectly change that business logic by overriding the factory method and returning a different type of product from it.
+
+        Parameters:
+            **kwargs: Keyword arguments for the execute method.
+        """
+        return self.factory_method(**kwargs)
```

### Comparing `sefazetllib-0.1.33/sefazetllib/factory/platform/database/MySQL.py` & `sefazetllib-0.1.34/sefazetllib/factory/platform/database/Mysql.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from sefazetllib.factory.platform.DatabasePlatform import DatabasePlatform
-
-
-class MySQL(DatabasePlatform):
-    def __init__(self, name="MySQL Job", configs=[]) -> None:
-        self.name = name
-        self.session = None
-
-    def get_url(self, **kwargs):
-        host = kwargs["host"]
-        format = kwargs["format"]
-        operator = kwargs["operator"]
-        database = kwargs["database"].lower()
-        port = kwargs["port"]
-        schema = kwargs["schema"]
-        return f"{format}{operator}{database}://{host}:{port}/{schema}"
-
-    def get_table_name(self, **kwargs):
-        table = kwargs["table"]
-        return table
-
-    def read(self, **kwargs):
-        pass
-
-    def load(self, **kwargs):
-        pass
+from sefazetllib.factory.platform.DatabasePlatform import DatabasePlatform
+
+
+class MySQL(DatabasePlatform):
+    def __init__(self, name="MySQL Job", configs=[]) -> None:
+        self.name = name
+        self.session = None
+
+    def get_url(self, **kwargs):
+        host = kwargs["host"]
+        format = kwargs["format"]
+        operator = kwargs["operator"]
+        database = kwargs["database"].lower()
+        port = kwargs["port"]
+        schema = kwargs["schema"]
+        return f"{format}{operator}{database}://{host}:{port}/{schema}"
+
+    def get_table_name(self, **kwargs):
+        table = kwargs["table"]
+        return table
+
+    def read(self, **kwargs):
+        pass
+
+    def load(self, **kwargs):
+        pass
```

### Comparing `sefazetllib-0.1.33/sefazetllib/factory/platform/database/PostgreSQL.py` & `sefazetllib-0.1.34/sefazetllib/factory/platform/database/PostgreSQL.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-from sqlalchemy import create_engine, text
-
-from sefazetllib.factory.platform.DatabasePlatform import DatabasePlatform
-
-
-class PostgreSQL(DatabasePlatform):
-    def __init__(self, name="PostgreSQL Job", configs=[]) -> None:
-        self.name = name
-        self.session = None
-        self.conn = None
-        self.transaction = None
-
-        if configs != []:
-            url_args = configs
-            if not isinstance(configs, dict):
-                url_args = {config[0]: config[1] for config in configs}
-
-            self.session = create_engine(
-                f"postgresql+psycopg2://"
-                f'{url_args["user"]}:{url_args["password"]}@{url_args["host"]}:'
-                f'{url_args["port"]}/'
-                f'{url_args["instance"]}'
-            )
-            self.create_connection()
-
-    def get_url(self, **kwargs):
-        host = kwargs["host"]
-        port = kwargs["port"]
-        file_format = kwargs["file_format"]
-        operator = kwargs["operator"]
-        database = kwargs["database"].lower()
-        instance = kwargs["instance"]
-        return f"{file_format}{operator}{database}://{host}:{port}/{instance}"
-
-    def get_table_name(self, **kwargs):
-        schema = kwargs["schema"]
-        table = kwargs["table"]
-        return f"{schema}.{table}"
-
-    def create_connection(self):
-        self.conn = self.session.connect()
-        return
-
-    def close_connection(self):
-        self.conn.close()
-        return
-
-    def begin_transaction(self):
-        self.transaction = self.conn.begin()
-        return
-
-    def create_commit(self):
-        if self.transaction is not None:
-            self.transaction.commit()
-        return
-
-    def rollback(self):
-        if self.transaction is not None:
-            self.transaction.rollback()
-        return
-
-    def truncate(self, **kwargs):
-        schema = kwargs["schema"].lower()
-        table = kwargs["table"].lower()
-        self.conn.execute(text(f"TRUNCATE TABLE {schema}.{table}"))
-        return
-
-    def drop_constraints(self, **kwargs):
-        table = kwargs["table"].lower()
-        dependencies = [
-            row._asdict()
-            for row in self.conn.execute(
-                text(
-                    f"""
-        SELECT tc.table_schema,
-            tc.constraint_name,
-            tc.table_name,
-            kcu.column_name,
-            ccu.table_schema AS foreign_table_schema,
-            ccu.table_name AS foreign_table_name,
-            ccu.column_name AS foreign_column_name
-        FROM information_schema.table_constraints AS tc
-            JOIN information_schema.key_column_usage AS kcu ON tc.constraint_name = kcu.constraint_name
-            AND tc.table_schema = kcu.table_schema
-            JOIN information_schema.constraint_column_usage AS ccu ON ccu.constraint_name = tc.constraint_name
-            AND ccu.table_schema = tc.table_schema
-        WHERE tc.constraint_type = 'FOREIGN KEY'
-            AND (tc.table_name = '{table}' OR ccu.table_name = '{table}')
-        """
-                )
-            ).fetchall()
-        ]
-
-        alter_queries = [
-            f"""ALTER TABLE {dependencie['table_schema']}.{dependencie['table_name']} DROP CONSTRAINT {dependencie['constraint_name']};"""
-            for dependencie in dependencies
-        ]
-
-        if bool(alter_queries):
-            self.conn.execute(text("\n".join(alter_queries)))
-        return dependencies
-
-    def create_constraints(self, **kwargs):
-        dependencies = kwargs["dependencies"]
-
-        alter_queries = [
-            f"""ALTER TABLE {dependencie['table_schema']}.{dependencie['table_name']} ADD CONSTRAINT {dependencie['constraint_name']} FOREIGN KEY ({dependencie['column_name']}) REFERENCES {dependencie['foreign_table_schema']}.{dependencie['foreign_table_name']}({dependencie['foreign_column_name']});"""
-            for dependencie in dependencies
-        ]
-        if bool(alter_queries):
-            self.conn.execute(text("\n".join(alter_queries)))
-        return
-
-    def read(self, **kwargs):
-        pass
-
-    def load(self, **kwargs):
-        pass
+from sqlalchemy import create_engine, text
+
+from sefazetllib.factory.platform.DatabasePlatform import DatabasePlatform
+
+
+class PostgreSQL(DatabasePlatform):
+    def __init__(self, name="PostgreSQL Job", configs=[]) -> None:
+        self.name = name
+        self.session = None
+        self.conn = None
+        self.transaction = None
+
+        if configs != []:
+            url_args = configs
+            if not isinstance(configs, dict):
+                url_args = {config[0]: config[1] for config in configs}
+
+            self.session = create_engine(
+                f"postgresql+psycopg2://"
+                f'{url_args["user"]}:{url_args["password"]}@{url_args["host"]}:'
+                f'{url_args["port"]}/'
+                f'{url_args["instance"]}'
+            )
+            self.create_connection()
+
+    def get_url(self, **kwargs):
+        host = kwargs["host"]
+        port = kwargs["port"]
+        file_format = kwargs["file_format"]
+        operator = kwargs["operator"]
+        database = kwargs["database"].lower()
+        instance = kwargs["instance"]
+        return f"{file_format}{operator}{database}://{host}:{port}/{instance}"
+
+    def get_table_name(self, **kwargs):
+        schema = kwargs["schema"]
+        table = kwargs["table"]
+        return f"{schema}.{table}"
+
+    def create_connection(self):
+        self.conn = self.session.connect()
+        return
+
+    def close_connection(self):
+        self.conn.close()
+        return
+
+    def begin_transaction(self):
+        self.transaction = self.conn.begin()
+        return
+
+    def create_commit(self):
+        if self.transaction is not None:
+            self.transaction.commit()
+        return
+
+    def rollback(self):
+        if self.transaction is not None:
+            self.transaction.rollback()
+        return
+
+    def truncate(self, **kwargs):
+        schema = kwargs["schema"].lower()
+        table = kwargs["table"].lower()
+        self.conn.execute(text(f"TRUNCATE TABLE {schema}.{table}"))
+        return
+
+    def drop_constraints(self, **kwargs):
+        table = kwargs["table"].lower()
+        dependencies = [
+            row._asdict()
+            for row in self.conn.execute(
+                text(
+                    f"""
+        SELECT tc.table_schema,
+            tc.constraint_name,
+            tc.table_name,
+            kcu.column_name,
+            ccu.table_schema AS foreign_table_schema,
+            ccu.table_name AS foreign_table_name,
+            ccu.column_name AS foreign_column_name
+        FROM information_schema.table_constraints AS tc
+            JOIN information_schema.key_column_usage AS kcu ON tc.constraint_name = kcu.constraint_name
+            AND tc.table_schema = kcu.table_schema
+            JOIN information_schema.constraint_column_usage AS ccu ON ccu.constraint_name = tc.constraint_name
+            AND ccu.table_schema = tc.table_schema
+        WHERE tc.constraint_type = 'FOREIGN KEY'
+            AND (tc.table_name = '{table}' OR ccu.table_name = '{table}')
+        """
+                )
+            ).fetchall()
+        ]
+
+        alter_queries = [
+            f"""ALTER TABLE {dependencie['table_schema']}.{dependencie['table_name']} DROP CONSTRAINT {dependencie['constraint_name']};"""
+            for dependencie in dependencies
+        ]
+
+        if bool(alter_queries):
+            self.conn.execute(text("\n".join(alter_queries)))
+        return dependencies
+
+    def create_constraints(self, **kwargs):
+        dependencies = kwargs["dependencies"]
+
+        alter_queries = [
+            f"""ALTER TABLE {dependencie['table_schema']}.{dependencie['table_name']} ADD CONSTRAINT {dependencie['constraint_name']} FOREIGN KEY ({dependencie['column_name']}) REFERENCES {dependencie['foreign_table_schema']}.{dependencie['foreign_table_name']}({dependencie['foreign_column_name']});"""
+            for dependencie in dependencies
+        ]
+        if bool(alter_queries):
+            self.conn.execute(text("\n".join(alter_queries)))
+        return
+
+    def read(self, **kwargs):
+        pass
+
+    def load(self, **kwargs):
+        pass
```

### Comparing `sefazetllib-0.1.33/sefazetllib/factory/platform/dataframe/Pandas.py` & `sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/Pandas.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from datetime import date
-
-import pandas as pd
-from pandas.util import hash_pandas_object
-
-from sefazetllib.factory.platform.Platform import Platform
-
-
-class Pandas(Platform):
-    def __init__(self, name=None) -> None:
-        self.session = pd
-        self.name = name
-
-    def __read_csv(self, url):
-        return self.session.read_csv(url)
-
-    def __read_parquet(self, url):
-        return self.session.read_parquet(url)
-
-    def __save_csv(self, df, url, properties):
-        return df.to_csv(url, **properties)
-
-    def __save_parquet(self, df, url, properties):
-        return df.to_parquet(url, **properties)
-
-    def __get_key_method(self, name):
-        return {"SurrogateKey": hash_pandas_object}[name]
-
-    def read(self, **kwargs):
-        file_format = kwargs["file_format"]
-        url = kwargs["url"]
-        return {"csv": self.__read_csv, "parquet": self.__read_parquet}[file_format](
-            url
-        )
-
-    def load(self, **kwargs):
-        df = kwargs["df"]
-        sk_name = kwargs["sk_name"]
-        key = kwargs["key"]
-        columns = kwargs["columns"]
-        duplicates = kwargs["duplicates"]
-        file_format = kwargs["file_format"]
-        format_properties = kwargs["format_properties"]
-        url = kwargs["url"]
-
-        key.setColumns(df[key.columns])
-        key.setMethod(self.__get_key_method(type(key).__name__))
-
-        writer_format = df
-        writer_format[sk_name] = key.get()
-        writer_format["DAT_CARGA"] = date.today()
-
-        if bool(columns):
-            writer_format = writer_format[columns]
-
-        if duplicates:
-            writer_format = writer_format.drop_duplicates()
-
-        return {"csv": self.__save_csv, "parquet": self.__save_parquet}[file_format](
-            writer_format, url, format_properties
-        )
+from datetime import date
+
+import pandas as pd
+from pandas.util import hash_pandas_object
+
+from sefazetllib.factory.platform.Platform import Platform
+
+
+class Pandas(Platform):
+    def __init__(self, name=None) -> None:
+        self.session = pd
+        self.name = name
+
+    def __read_csv(self, url):
+        return self.session.read_csv(url)
+
+    def __read_parquet(self, url):
+        return self.session.read_parquet(url)
+
+    def __save_csv(self, df, url, properties):
+        return df.to_csv(url, **properties)
+
+    def __save_parquet(self, df, url, properties):
+        return df.to_parquet(url, **properties)
+
+    def __get_key_method(self, name):
+        return {"SurrogateKey": hash_pandas_object}[name]
+
+    def read(self, **kwargs):
+        file_format = kwargs["file_format"]
+        url = kwargs["url"]
+        return {"csv": self.__read_csv, "parquet": self.__read_parquet}[file_format](
+            url
+        )
+
+    def load(self, **kwargs):
+        df = kwargs["df"]
+        sk_name = kwargs["sk_name"]
+        key = kwargs["key"]
+        columns = kwargs["columns"]
+        duplicates = kwargs["duplicates"]
+        file_format = kwargs["file_format"]
+        format_properties = kwargs["format_properties"]
+        url = kwargs["url"]
+
+        key.setColumns(df[key.columns])
+        key.setMethod(self.__get_key_method(type(key).__name__))
+
+        writer_format = df
+        writer_format[sk_name] = key.get()
+        writer_format["DAT_CARGA"] = date.today()
+
+        if bool(columns):
+            writer_format = writer_format[columns]
+
+        if duplicates:
+            writer_format = writer_format.drop_duplicates()
+
+        return {"csv": self.__save_csv, "parquet": self.__save_parquet}[file_format](
+            writer_format, url, format_properties
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllib/factory/platform/PlatformFactory.py` & `sefazetllib-0.1.34/sefazetllib/factory/platform/PlatformFactory.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from sefazetllib.factory.Factory import Creator
-from sefazetllib.factory.platform.database import MySQL, PostgreSQL
-from sefazetllib.factory.platform.dataframe import Default, Pandas, Spark
-
-
-class PlatformFactory(Creator):
-    """
-    Note that the signature of the method still uses the abstract product type,
-    even though the concrete product is actually returned from the method. This
-    way the Creator can stay independent of concrete product classes.
-    """
-
-    def __init__(self, platform) -> None:
-        self.platform = platform
-
-    def create(self, **kwargs):
-        """
-        The client code works with an instance of a concrete creator, albeit through
-        its base interface. As long as the client keeps working with the creator via
-        the base interface, you can pass it any creator's subclass.
-        """
-        return self.execute(**kwargs)
-
-    def factory_method(self, **kwargs):
-        try:
-            return globals()[self.platform](**kwargs)
-        except KeyError:
-            return Default(**kwargs)
+from sefazetllib.factory.Factory import Creator
+from sefazetllib.factory.platform.database import MySQL, PostgreSQL
+from sefazetllib.factory.platform.dataframe import Default, Pandas, Spark
+
+
+class PlatformFactory(Creator):
+    """
+    Note that the signature of the method still uses the abstract product type,
+    even though the concrete product is actually returned from the method. This
+    way the Creator can stay independent of concrete product classes.
+    """
+
+    def __init__(self, platform) -> None:
+        self.platform = platform
+
+    def create(self, **kwargs):
+        """
+        The client code works with an instance of a concrete creator, albeit through
+        its base interface. As long as the client keeps working with the creator via
+        the base interface, you can pass it any creator's subclass.
+        """
+        return self.execute(**kwargs)
+
+    def factory_method(self, **kwargs):
+        try:
+            return globals()[self.platform](**kwargs)
+        except KeyError:
+            return Default(**kwargs)
```

### Comparing `sefazetllib-0.1.33/sefazetllib/load/LoadLocal.py` & `sefazetllib-0.1.34/sefazetllib/load/LoadS3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,72 @@
-import os
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.load.Load import Load
-from sefazetllib.utils.key import DefaultKey, Key
-
-
-@Builder
-class LoadLocal(Load):
-    platform: Platform = field(default=Default())
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    reference: str = field(default="")
-    url: str = field(default="")
-    repository: str = field(default="")
-    entity: str = field(default="")
-    mode: str = field(default="")
-    df_writer: Any = field(default="")
-    duplicates: bool = field(default=False)
-    key: Key = field(default=DefaultKey())
-    columns: List = field(default_factory=list)
-    load_date: bool = field(default=True)
-
-    def build_connection_string(self):
-        return f"{os.getcwd()}/{self.entity}.{self.file_format}"
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.repository == "":
-            self.setRepository(kwargs["repository"])
-
-        self.url = self.build_connection_string()
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.loadRepository:
-                self.setRepository(args.loadRepository)
-
-            if args.loadUrl:
-                self.url = args.loadUrl
-
-        sk_name = f"SK_{self.entity}"
-        if "/" in self.entity:
-            entity = self.entity.split("/")[1]
-            sk_name = f"SK_{entity}"
-
-        return (
-            self.reference,
-            self.platform.load(
-                df=self.df_writer,
-                sk_name=sk_name,
-                key=self.key,
-                columns=self.columns,
-                duplicates=self.duplicates,
-                file_format=self.file_format,
-                format_properties=self.format_properties,
-                url=self.url,
-                mode=self.mode,
-                load_date=self.load_date,
-            ),
-        )
+import warnings
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.load.Load import Load
+from sefazetllib.utils.key import DefaultKey, Key
+
+
+@Builder
+class LoadS3(Load):
+    warnings.warn(
+        "The 'LoadS3' class is deprecated. Please use the 'LoadStorage' class with the protocol parameter (e.g., 's3a')."
+    )
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="")
+    format_properties: Dict[str, Any] = field(default_factory=dict)
+    reference: str = field(default="")
+    url: str = field(default="")
+    repository: str = field(default="")
+    layer: str = field(default="")
+    schema: str = field(default="")
+    entity: str = field(default="")
+    mode: str = field(default="")
+    df_writer: Any = field(default="")
+    duplicates: bool = field(default=False)
+    key: Key = field(default=DefaultKey())
+    columns: List = field(default_factory=list)
+    load_date: bool = field(default=True)
+
+    def build_connection_string(self):
+        self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
+        return self.url
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        if self.repository == "":
+            self.setRepository(kwargs["repository"])
+
+        url = self.build_connection_string()
+
+        if kwargs:
+            args = kwargs["args"]
+            if args.loadRepository:
+                self.setRepository(args.loadRepository)
+
+            if args.loadUrl:
+                url = args.loadUrl
+
+        sk_name = f"SK_{self.entity}"
+        if "/" in self.entity:
+            entity = self.entity.split("/")[1]
+            sk_name = f"SK_{entity}"
+
+        return (
+            self.reference,
+            self.platform.load(
+                df=self.df_writer,
+                sk_name=sk_name,
+                key=self.key,
+                columns=self.columns,
+                duplicates=self.duplicates,
+                file_format=self.file_format,
+                format_properties=self.format_properties,
+                url=url,
+                mode=self.mode,
+                load_date=self.load_date,
+            ),
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllib/load/LoadS3.py` & `sefazetllib-0.1.34/sefazetllib/extract/ExtractSQL.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,79 @@
-import warnings
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.load.Load import Load
-from sefazetllib.utils.key import DefaultKey, Key
-
-
-@Builder
-class LoadS3(Load):
-    warnings.warn(
-        "The 'LoadS3' class is deprecated. Please use the 'LoadStorage' class with the protocol parameter (e.g., 's3a')."
-    )
-    platform: Platform = field(default=Default())
-    file_format: str = field(default="")
-    format_properties: Dict[str, Any] = field(default_factory=dict)
-    reference: str = field(default="")
-    url: str = field(default="")
-    repository: str = field(default="")
-    layer: str = field(default="")
-    schema: str = field(default="")
-    entity: str = field(default="")
-    mode: str = field(default="")
-    df_writer: Any = field(default="")
-    duplicates: bool = field(default=False)
-    key: Key = field(default=DefaultKey())
-    columns: List = field(default_factory=list)
-    load_date: bool = field(default=True)
-
-    def build_connection_string(self):
-        self.url = f"s3a://{self.repository}/{self.layer}/{self.schema}/{self.entity}"
-        return self.url
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.repository == "":
-            self.setRepository(kwargs["repository"])
-
-        url = self.build_connection_string()
-
-        if kwargs:
-            args = kwargs["args"]
-            if args.loadRepository:
-                self.setRepository(args.loadRepository)
-
-            if args.loadUrl:
-                url = args.loadUrl
-
-        sk_name = f"SK_{self.entity}"
-        if "/" in self.entity:
-            entity = self.entity.split("/")[1]
-            sk_name = f"SK_{entity}"
-
-        return (
-            self.reference,
-            self.platform.load(
-                df=self.df_writer,
-                sk_name=sk_name,
-                key=self.key,
-                columns=self.columns,
-                duplicates=self.duplicates,
-                file_format=self.file_format,
-                format_properties=self.format_properties,
-                url=url,
-                mode=self.mode,
-                load_date=self.load_date,
-            ),
-        )
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.extract.Extract import Extract
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.factory.platform.PlatformFactory import PlatformFactory
+
+
+@Builder
+class ExtractSQL(Extract):
+    platform: Platform = field(default=Default())
+    format: str = field(default="jdbc")
+    operator: str = field(default=":")
+    host: str = field(default="")
+    port: int = field(default=0)
+    database: str = field(default="")
+    instance: str = field(default="")
+    driver: str = field(default="")
+    schema: str = field(default="")
+    table: str = field(default="")
+    authentication: Dict[str, Any] = field(default_factory=dict)
+    url: str = field(default="")
+    reference: str = field(default="")
+    columns: List[str] = field(default_factory=list)
+    optional: bool = field(default=False)
+    duplicates: bool = field(default=False)
+
+    def __build_properties(self):
+        self.properties = {
+            "database": self.database,
+            "driver": self.driver,
+            "user": self.authentication["user"],
+            "password": self.authentication["password"],
+            "dbtable": self.table,
+            "url": self.url,
+        }
+
+        return self.properties
+
+    def build_connection_string(self):
+        platform_db = PlatformFactory(self.database).create(
+            name="get url jdbc",
+        )
+        self.url = platform_db.get_url(
+            format=self.format,
+            operator=self.operator,
+            database=self.database,
+            host=self.host,
+            instance=self.instance,
+            schema=self.schema,
+            port=self.port,
+        )
+
+        self.table = platform_db.get_table_name(table=self.table, schema=self.schema)
+
+        return self.url
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        url = self.build_connection_string()
+        properties = self.__build_properties()
+
+        if kwargs:
+            args = kwargs["args"]
+
+            if args.extractUrl:
+                url = args.extractUrl
+
+        return self.reference, self.platform.read(
+            format=self.format,
+            url=url,
+            format_properties=properties,
+            optional=self.optional,
+            columns=self.columns,
+            duplicates=self.duplicates,
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllib/load/LoadSQL.py` & `sefazetllib-0.1.34/sefazetllib/load/LoadSQL.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-from typing import Any, Dict, List
-
-from sefazetllib.Builder import Builder, field
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.factory.platform.PlatformFactory import PlatformFactory
-from sefazetllib.load.Load import Load
-from sefazetllib.utils.key import DefaultKey, Key
-
-
-@Builder
-class LoadSQL(Load):
-    platform: Platform = field(default=Default())
-    file_format: str = field(default="jdbc")
-    operator: str = field(default=":")
-    host: str = field(default="")
-    port: int = field(default=0)
-    database: str = field(default="")
-    instance: str = field(default="")
-    dbtable: str = field(default="")
-    driver: str = field(default="")
-    schema: str = field(default="")
-    table: str = field(default="")
-    authentication: Dict[str, Any] = field(default_factory=dict)
-    url: str = field(default="")
-    reference: str = field(default="")
-    df_writer: Any = field(default="")
-    mode: str = field(default="")
-    sk_name: str = field(default="")
-    key: Key = field(default=DefaultKey())
-    columns: List[str] = field(default_factory=list)
-    operation: str = field(default="")
-    optional: bool = field(default=False)
-    duplicates: bool = field(default=False)
-    truncate: bool = field(default=False)
-    load_date: bool = field(default=True)
-    fetch_size: int = field(default=100000)
-    batch_size: int = field(default=100000)
-
-    def __build_properties(self):
-        return {
-            "operation": self.operation,
-            "file_format": self.file_format,
-            "operator": self.operator,
-            "database": self.database,
-            "driver": self.driver,
-            "user": self.authentication["user"],
-            "password": self.authentication["password"],
-            "dbtable": self.dbtable,
-            "url": self.url,
-            "host": self.host,
-            "port": self.port,
-            "instance": self.instance,
-        }
-
-    def __table_properties(self):
-        return {"schema": self.schema, "table": self.table}
-
-    def __load_transaction(
-        self, platform_db, df, sk_name, truncate, mode, dependencies
-    ):
-        df_loaded = self.platform.load(
-            df=df,
-            sk_name=sk_name,
-            key=self.key,
-            columns=self.columns,
-            duplicates=self.duplicates,
-            file_format=self.file_format,
-            format_properties={
-                "driver": self.driver,
-                "user": self.authentication["user"],
-                "password": self.authentication["password"],
-                "dbtable": self.dbtable,
-                "truncate": truncate,
-                "batchsize": self.batch_size
-            },
-            url=platform_db.get_url(**self.__build_properties()),
-            mode=mode,
-            load_date=self.load_date,
-        )
-        if (not (self.operation.lower()=="insert" and mode.lower()=="append")):
-            platform_db.begin_transaction()
-            try:
-                platform_db.create_constraints(**{"dependencies": dependencies})
-            except Exception as err:
-                platform_db.rollback()
-                raise Exception("Erro ao criar constraints", str(err))
-            else:
-                platform_db.create_commit()
-
-        return df_loaded
-
-    def build_connection_string(self):
-        platform_db = PlatformFactory(self.database).create(
-            name="get url jdbc", configs=self.__build_properties()
-        )
-        self.url = platform_db.get_url(
-            file_format=self.file_format,
-            operator=self.operator,
-            database=self.database,
-            host=self.host,
-            instance=self.instance,
-            schema=self.schema,
-            port=self.port,
-        )
-
-        self.dbtable = platform_db.get_table_name(
-            table=self.table.lower(), schema=self.schema.lower()
-        )
-        return platform_db
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.sk_name == "":
-            self.sk_name = f"SK_{self.table}"
-            if "/" in self.table:
-                table = self.table.split("/")[1]
-                self.sk_name = f"SK_{table}"
-
-        platform_db = self.build_connection_string()
-        dependencies = []
-
-        if (self.operation.lower()=="insert" and self.mode.lower()=="append"):
-            df_old = self.platform.create_df(self.columns)
-        else:
-            df_old = self.platform.read(
-                file_format=self.file_format,
-                url=platform_db.get_url(**self.__build_properties()),
-                format_properties={
-                    "driver": self.driver,
-                    "user": self.authentication["user"],
-                    "password": self.authentication["password"],
-                    "dbtable": self.dbtable,
-                    "fetchsize": self.fetch_size,
-                },
-                optional=False,
-                columns="",
-                duplicates=self.duplicates,
-            )
-            
-        df_old = self.platform.columns_to_upper(df_old)
-
-        if bool(self.columns):
-            df_old = self.platform.select_columns(df_old, self.columns)
-            self.df_writer = self.platform.select_columns(self.df_writer, self.columns)
-
-        df_old = self.platform.checkpoint(df_old)
-
-        if (
-            "operation" in self.__build_properties()
-            and self.__build_properties()["operation"] == "upsert"
-        ):
-            self.df_writer = self.platform.union_by_name(
-                left=self.platform.join(
-                    left=df_old,
-                    right=self.df_writer,
-                    keys=self.sk_name,
-                    how="left_anti",
-                ),
-                right=self.df_writer,
-            )
-            self.mode = "overwrite"
-            self.truncate = True
-
-        try:
-            if (not (self.operation.lower()=="insert" and self.mode.lower()=="append")):
-                platform_db.begin_transaction()
-                try:
-                    dependencies = platform_db.drop_constraints(**self.__table_properties())
-                except Exception as err:
-                    platform_db.rollback()
-                    raise Exception(
-                        "Erro ao remover constraints. Realizando Rollback ...", str(err)
-                    )
-                else:
-                    platform_db.create_commit()
-
-            try:
-                df_loaded = self.__load_transaction(
-                    platform_db=platform_db,
-                    df=self.df_writer,
-                    sk_name=self.sk_name,
-                    truncate=self.truncate,
-                    mode=self.mode,
-                    dependencies=dependencies,
-                )
-            except Exception as err:
-                df_loaded = self.__load_transaction(
-                    platform_db=platform_db,
-                    df=df_old,
-                    sk_name=self.sk_name,
-                    truncate=True,
-                    mode="overwrite",
-                    dependencies=dependencies,
-                )
-                raise Exception(
-                    "Erro ao inserir os dados, tentando recuperar as informações antigas...",
-                    str(err),
-                )
-
-        except Exception as err:
-            raise Exception("Erro no LoadSQL ...", str(err))
-        finally:
-            platform_db.close_connection()
-
-        return self.reference, df_loaded
+from typing import Any, Dict, List
+
+from sefazetllib.Builder import Builder, field
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.factory.platform.PlatformFactory import PlatformFactory
+from sefazetllib.load.Load import Load
+from sefazetllib.utils.key import DefaultKey, Key
+
+
+@Builder
+class LoadSQL(Load):
+    platform: Platform = field(default=Default())
+    file_format: str = field(default="jdbc")
+    operator: str = field(default=":")
+    host: str = field(default="")
+    port: int = field(default=0)
+    database: str = field(default="")
+    instance: str = field(default="")
+    dbtable: str = field(default="")
+    driver: str = field(default="")
+    schema: str = field(default="")
+    table: str = field(default="")
+    authentication: Dict[str, Any] = field(default_factory=dict)
+    url: str = field(default="")
+    reference: str = field(default="")
+    df_writer: Any = field(default="")
+    mode: str = field(default="")
+    sk_name: str = field(default="")
+    key: Key = field(default=DefaultKey())
+    columns: List[str] = field(default_factory=list)
+    operation: str = field(default="")
+    optional: bool = field(default=False)
+    duplicates: bool = field(default=False)
+    truncate: bool = field(default=False)
+    load_date: bool = field(default=True)
+    fetch_size: int = field(default=100000)
+    batch_size: int = field(default=100000)
+
+    def __build_properties(self):
+        return {
+            "operation": self.operation,
+            "file_format": self.file_format,
+            "operator": self.operator,
+            "database": self.database,
+            "driver": self.driver,
+            "user": self.authentication["user"],
+            "password": self.authentication["password"],
+            "dbtable": self.dbtable,
+            "url": self.url,
+            "host": self.host,
+            "port": self.port,
+            "instance": self.instance,
+        }
+
+    def __table_properties(self):
+        return {"schema": self.schema, "table": self.table}
+
+    def __load_transaction(
+        self, platform_db, df, sk_name, truncate, mode, dependencies
+    ):
+        df_loaded = self.platform.load(
+            df=df,
+            sk_name=sk_name,
+            key=self.key,
+            columns=self.columns,
+            duplicates=self.duplicates,
+            file_format=self.file_format,
+            format_properties={
+                "driver": self.driver,
+                "user": self.authentication["user"],
+                "password": self.authentication["password"],
+                "dbtable": self.dbtable,
+                "truncate": truncate,
+                "batchsize": self.batch_size
+            },
+            url=platform_db.get_url(**self.__build_properties()),
+            mode=mode,
+            load_date=self.load_date,
+        )
+        if (not (self.operation.lower()=="insert" and mode.lower()=="append")):
+            platform_db.begin_transaction()
+            try:
+                platform_db.create_constraints(**{"dependencies": dependencies})
+            except Exception as err:
+                platform_db.rollback()
+                raise Exception("Erro ao criar constraints", str(err))
+            else:
+                platform_db.create_commit()
+
+        return df_loaded
+
+    def build_connection_string(self):
+        platform_db = PlatformFactory(self.database).create(
+            name="get url jdbc", configs=self.__build_properties()
+        )
+        self.url = platform_db.get_url(
+            file_format=self.file_format,
+            operator=self.operator,
+            database=self.database,
+            host=self.host,
+            instance=self.instance,
+            schema=self.schema,
+            port=self.port,
+        )
+
+        self.dbtable = platform_db.get_table_name(
+            table=self.table.lower(), schema=self.schema.lower()
+        )
+        return platform_db
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        if self.sk_name == "":
+            self.sk_name = f"SK_{self.table}"
+            if "/" in self.table:
+                table = self.table.split("/")[1]
+                self.sk_name = f"SK_{table}"
+
+        platform_db = self.build_connection_string()
+        dependencies = []
+
+        if (self.operation.lower()=="insert" and self.mode.lower()=="append"):
+            df_old = self.platform.create_df(self.columns)
+        else:
+            df_old = self.platform.read(
+                file_format=self.file_format,
+                url=platform_db.get_url(**self.__build_properties()),
+                format_properties={
+                    "driver": self.driver,
+                    "user": self.authentication["user"],
+                    "password": self.authentication["password"],
+                    "dbtable": self.dbtable,
+                    "fetchsize": self.fetch_size,
+                },
+                optional=False,
+                columns="",
+                duplicates=self.duplicates,
+            )
+            
+        df_old = self.platform.columns_to_upper(df_old)
+
+        if bool(self.columns):
+            df_old = self.platform.select_columns(df_old, self.columns)
+            self.df_writer = self.platform.select_columns(self.df_writer, self.columns)
+
+        df_old = self.platform.checkpoint(df_old)
+
+        if (
+            "operation" in self.__build_properties()
+            and self.__build_properties()["operation"] == "upsert"
+        ):
+            self.df_writer = self.platform.union_by_name(
+                left=self.platform.join(
+                    left=df_old,
+                    right=self.df_writer,
+                    keys=self.sk_name,
+                    how="left_anti",
+                ),
+                right=self.df_writer,
+            )
+            self.mode = "overwrite"
+            self.truncate = True
+
+        try:
+            if (not (self.operation.lower()=="insert" and self.mode.lower()=="append")):
+                platform_db.begin_transaction()
+                try:
+                    dependencies = platform_db.drop_constraints(**self.__table_properties())
+                except Exception as err:
+                    platform_db.rollback()
+                    raise Exception(
+                        "Erro ao remover constraints. Realizando Rollback ...", str(err)
+                    )
+                else:
+                    platform_db.create_commit()
+
+            try:
+                df_loaded = self.__load_transaction(
+                    platform_db=platform_db,
+                    df=self.df_writer,
+                    sk_name=self.sk_name,
+                    truncate=self.truncate,
+                    mode=self.mode,
+                    dependencies=dependencies,
+                )
+            except Exception as err:
+                df_loaded = self.__load_transaction(
+                    platform_db=platform_db,
+                    df=df_old,
+                    sk_name=self.sk_name,
+                    truncate=True,
+                    mode="overwrite",
+                    dependencies=dependencies,
+                )
+                raise Exception(
+                    "Erro ao inserir os dados, tentando recuperar as informações antigas...",
+                    str(err),
+                )
+
+        except Exception as err:
+            raise Exception("Erro no LoadSQL ...", str(err))
+        finally:
+            platform_db.close_connection()
+
+        return self.reference, df_loaded
```

### Comparing `sefazetllib-0.1.33/sefazetllib/transform/MinMaxLineTransform.py` & `sefazetllib-0.1.34/sefazetllib/transform/MinMaxLineTransform.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from typing import Any, List, Optional
-
-from pyspark.sql.functions import col, dense_rank
-from pyspark.sql.window import Window
-
-from sefazetllib import Builder, field
-from sefazetllib.transform.Transform import Transform
-
-
-@Builder
-class MinMaxLineTransform(Transform):
-    df: Optional[Any] = None
-    reference: str = field(default="")
-    output: str = field(default="")
-    order: str = field(default="")
-    orders: List[str] = field(default_factory=list)
-    window: str = field(default="")
-    max: bool = field(default=False)
-    min: bool = field(default=False)
-
-    def __get_window(self):
-        if self.max:
-            order_max = []
-
-            for unique_order in self.orders:
-                order_max.append(col(unique_order).desc())
-
-            self.window = Window.orderBy(order_max)
-
-        if self.min:
-            self.window = Window.orderBy(self.orders)
-
-        if self.order != "":
-            if self.max:
-                self.window = Window.orderBy(col(self.order).desc())
-
-            if self.min:
-                self.window = Window.orderBy(self.order)
-
-    def execute(self):
-        self.__get_window()
-        return (
-            self.output,
-            (
-                self.df.withColumn(
-                    "FLG_FILTER_LINE",
-                    dense_rank().over(self.window),
-                )
-                .filter(col("FLG_FILTER_LINE").eqNullSafe(1))
-                .drop("FLG_FILTER_LINE")
-            ),
-        )
+from typing import Any, List, Optional
+
+from pyspark.sql.functions import col, dense_rank
+from pyspark.sql.window import Window
+
+from sefazetllib import Builder, field
+from sefazetllib.transform.Transform import Transform
+
+
+@Builder
+class MinMaxLineTransform(Transform):
+    df: Optional[Any] = None
+    reference: str = field(default="")
+    output: str = field(default="")
+    order: str = field(default="")
+    orders: List[str] = field(default_factory=list)
+    window: str = field(default="")
+    max: bool = field(default=False)
+    min: bool = field(default=False)
+
+    def __get_window(self):
+        if self.max:
+            order_max = []
+
+            for unique_order in self.orders:
+                order_max.append(col(unique_order).desc())
+
+            self.window = Window.orderBy(order_max)
+
+        if self.min:
+            self.window = Window.orderBy(self.orders)
+
+        if self.order != "":
+            if self.max:
+                self.window = Window.orderBy(col(self.order).desc())
+
+            if self.min:
+                self.window = Window.orderBy(self.order)
+
+    def execute(self):
+        self.__get_window()
+        return (
+            self.output,
+            (
+                self.df.withColumn(
+                    "FLG_FILTER_LINE",
+                    dense_rank().over(self.window),
+                )
+                .filter(col("FLG_FILTER_LINE").eqNullSafe(1))
+                .drop("FLG_FILTER_LINE")
+            ),
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllib/transform/QuartileTransform.py` & `sefazetllib-0.1.34/sefazetllib/transform/QuartileTransform.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-from typing import Any, List, Optional, Tuple
-
-from pyspark.sql.functions import col, first, percentile_approx, when, avg
-from pyspark.sql.window import Window
-
-from sefazetllib import Builder, field
-from sefazetllib.transform.Transform import Transform
-
-
-@Builder
-class QuartileTransform(Transform):
-    df: Optional[Any] = None
-    reference: str = field(default="")
-    output: str = field(default="")
-    partitions: List[str] = field(default_factory=list)
-    target: str = field(default="")
-    outlier: bool = field(default=False)
-    median: bool = field(default=False)
-    average: bool = field(default=False)
-    
-    def __get_window(self):
-        if self.partitions is not None:
-            self.window = Window.partitionBy(self.partitions)
-
-    def __get_quartile(self, percentile):
-        quartile = percentile_approx(self.target, percentile)
-
-        if self.window is not None:
-            return quartile.over(self.window)
-
-        return quartile
-
-    def execute(self) -> Tuple[str, Any]:
-        self.__get_window()
-
-        df_quartile = (
-            self.df.withColumn(f"Q1_{self.target}", self.__get_quartile(0.25))
-            .withColumn(f"Q2_{self.target}", self.__get_quartile(0.5))
-            .withColumn(f"Q3_{self.target}", self.__get_quartile(0.75))
-        )
-
-        if self.outlier:
-            df_quartile = df_quartile.withColumn(
-                f"OUT_{self.target}",
-                col(f"Q3_{self.target}")
-                + 3 * (col(f"Q3_{self.target}") - col(f"Q1_{self.target}")),
-            )
-
-        if (self.median | self.average):
-            group_columns = [
-                *self.partitions,
-                f"Q1_{self.target}",
-                f"Q2_{self.target}",
-                f"Q3_{self.target}",
-            ]
-
-            if self.outlier:
-                group_columns.append(f"OUT_{self.target}")
-
-            df_quartile = (
-                df_quartile.withColumn(
-                    f"STA_R_{self.target}",
-                    when(col(self.target) <= col(f"Q1_{self.target}"), 1)
-                    .when(
-                        (col(self.target) > col(f"Q1_{self.target}"))
-                        & (col(self.target) <= col(f"Q2_{self.target}")),
-                        2,
-                    )
-                    .when(
-                        (col(self.target) > col(f"Q2_{self.target}"))
-                        & (col(self.target) <= col(f"Q3_{self.target}")),
-                        3,
-                    )
-                    .when(col(self.target) > col(f"Q3_{self.target}"), 4),
-                )
-            )
-            
-            if self.median:
-                df_quartile = (df_quartile
-                    .withColumn(
-                        f"MEDIAN_Q_{self.target}",
-                        percentile_approx(self.target, 0.5).over(
-                            Window.partitionBy([*self.partitions, f"STA_R_{self.target}"])
-                        ),
-                    )
-                    .groupBy(group_columns)
-                    .pivot(f"STA_R_{self.target}")
-                    .agg(first(col(f"MEDIAN_Q_{self.target}")))
-                    .withColumnRenamed("1", f"MEDIAN_R1_{self.target}")
-                    .withColumnRenamed("2", f"MEDIAN_R2_{self.target}")
-                    .withColumnRenamed("3", f"MEDIAN_R3_{self.target}")
-                    .withColumnRenamed("4", f"MEDIAN_R4_{self.target}")
-            )
-            if self.average:
-                df_quartile = (df_quartile
-                    .withColumn(
-                        f"AVG_Q_{self.target}",
-                        avg(self.target).over(
-                            Window.partitionBy([*self.partitions, f"STA_R_{self.target}"])
-                        ),
-                    )
-                    .groupBy(group_columns)
-                    .pivot(f"STA_R_{self.target}")
-                    .agg(first(col(f"AVG_Q_{self.target}")))
-                    .withColumnRenamed("1", f"AVG_R1_{self.target}")
-                    .withColumnRenamed("2", f"AVG_R2_{self.target}")
-                    .withColumnRenamed("3", f"AVG_R3_{self.target}")
-                    .withColumnRenamed("4", f"AVG_R4_{self.target}")
-            )
-
-        if self.output is None:
-            self.output = self.reference
-
-        return self.output, df_quartile
+from typing import Any, List, Optional, Tuple
+
+from pyspark.sql.functions import col, first, percentile_approx, when, avg
+from pyspark.sql.window import Window
+
+from sefazetllib import Builder, field
+from sefazetllib.transform.Transform import Transform
+
+
+@Builder
+class QuartileTransform(Transform):
+    df: Optional[Any] = None
+    reference: str = field(default="")
+    output: str = field(default="")
+    partitions: List[str] = field(default_factory=list)
+    target: str = field(default="")
+    outlier: bool = field(default=False)
+    median: bool = field(default=False)
+    average: bool = field(default=False)
+    
+    def __get_window(self):
+        if self.partitions is not None:
+            self.window = Window.partitionBy(self.partitions)
+
+    def __get_quartile(self, percentile):
+        quartile = percentile_approx(self.target, percentile)
+
+        if self.window is not None:
+            return quartile.over(self.window)
+
+        return quartile
+
+    def execute(self) -> Tuple[str, Any]:
+        self.__get_window()
+
+        df_quartile = (
+            self.df.withColumn(f"Q1_{self.target}", self.__get_quartile(0.25))
+            .withColumn(f"Q2_{self.target}", self.__get_quartile(0.5))
+            .withColumn(f"Q3_{self.target}", self.__get_quartile(0.75))
+        )
+
+        if self.outlier:
+            df_quartile = df_quartile.withColumn(
+                f"OUT_{self.target}",
+                col(f"Q3_{self.target}")
+                + 3 * (col(f"Q3_{self.target}") - col(f"Q1_{self.target}")),
+            )
+
+        if (self.median | self.average):
+            group_columns = [
+                *self.partitions,
+                f"Q1_{self.target}",
+                f"Q2_{self.target}",
+                f"Q3_{self.target}",
+            ]
+
+            if self.outlier:
+                group_columns.append(f"OUT_{self.target}")
+
+            df_quartile = (
+                df_quartile.withColumn(
+                    f"STA_R_{self.target}",
+                    when(col(self.target) <= col(f"Q1_{self.target}"), 1)
+                    .when(
+                        (col(self.target) > col(f"Q1_{self.target}"))
+                        & (col(self.target) <= col(f"Q2_{self.target}")),
+                        2,
+                    )
+                    .when(
+                        (col(self.target) > col(f"Q2_{self.target}"))
+                        & (col(self.target) <= col(f"Q3_{self.target}")),
+                        3,
+                    )
+                    .when(col(self.target) > col(f"Q3_{self.target}"), 4),
+                )
+            )
+            
+            if self.median:
+                df_quartile = (df_quartile
+                    .withColumn(
+                        f"MEDIAN_Q_{self.target}",
+                        percentile_approx(self.target, 0.5).over(
+                            Window.partitionBy([*self.partitions, f"STA_R_{self.target}"])
+                        ),
+                    )
+                    .groupBy(group_columns)
+                    .pivot(f"STA_R_{self.target}")
+                    .agg(first(col(f"MEDIAN_Q_{self.target}")))
+                    .withColumnRenamed("1", f"MEDIAN_R1_{self.target}")
+                    .withColumnRenamed("2", f"MEDIAN_R2_{self.target}")
+                    .withColumnRenamed("3", f"MEDIAN_R3_{self.target}")
+                    .withColumnRenamed("4", f"MEDIAN_R4_{self.target}")
+            )
+            if self.average:
+                df_quartile = (df_quartile
+                    .withColumn(
+                        f"AVG_Q_{self.target}",
+                        avg(self.target).over(
+                            Window.partitionBy([*self.partitions, f"STA_R_{self.target}"])
+                        ),
+                    )
+                    .groupBy(group_columns)
+                    .pivot(f"STA_R_{self.target}")
+                    .agg(first(col(f"AVG_Q_{self.target}")))
+                    .withColumnRenamed("1", f"AVG_R1_{self.target}")
+                    .withColumnRenamed("2", f"AVG_R2_{self.target}")
+                    .withColumnRenamed("3", f"AVG_R3_{self.target}")
+                    .withColumnRenamed("4", f"AVG_R4_{self.target}")
+            )
+
+        if self.output is None:
+            self.output = self.reference
+
+        return self.output, df_quartile
```

### Comparing `sefazetllib-0.1.33/sefazetllib/utils/partition/DatePartition.py` & `sefazetllib-0.1.34/sefazetllib/utils/partition/DatePartition.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from datetime import date
-from typing import Optional
-
-from sefazetllib.Builder import Builder
-from sefazetllib.utils.partition.IncrementalRangePartition import (
-    IncrementalRangePartition,
-)
-from sefazetllib.utils.partition.Partition import Partition
-
-
-@Builder
-class DatePartition(Partition):
-    """
-    Implementation of the abstract base class 'Partition' for date partitioning.
-
-    Defines the methods to format and build the partition.
-    """
-
-    year: Optional[str] = None
-    month: Optional[str] = None
-    day: Optional[str] = None
-    years: Optional[IncrementalRangePartition] = None
-    months: Optional[IncrementalRangePartition] = None
-    days: Optional[IncrementalRangePartition] = None
-
-    def __format_partition(self, partition):
-        """Format the given partition.
-
-        Parameters:
-            partition: The partition to be formatted.
-
-        Returns:
-            The formatted partition.
-        """
-        return f"{set(partition.get())}".replace(" ", "")
-
-    def __build_partition(self):
-        """Build the partition.
-
-        Returns:
-            The list of strings representing the partition.
-        """
-        partition = [
-            self.__format_partition(self.years) if bool(self.years) else self.year
-        ]
-
-        if bool(self.month) or bool(self.months):
-            partition.append(
-                self.__format_partition(self.months)
-                if bool(self.months)
-                else self.month
-            )
-
-        if bool(self.day) or bool(self.days):
-            partition.append(
-                self.__format_partition(self.days) if bool(self.days) else self.day
-            )
-
-        return partition
-
-    def get(self):
-        """Get the partition.
-
-        Returns:
-            The list of strings representing the partition.
-        """
-        return self.__build_partition()
-
-    def get_date(self):
-        """Get the date of the partition.
-
-        Returns:
-            The date of the partition in the format 'YYYY/MM/DD'.
-        """
-        return date(*self.__build_partition()).strftime("%Y/%m/%d")
+from datetime import date
+from typing import Optional
+
+from sefazetllib.Builder import Builder
+from sefazetllib.utils.partition.IncrementalRangePartition import (
+    IncrementalRangePartition,
+)
+from sefazetllib.utils.partition.Partition import Partition
+
+
+@Builder
+class DatePartition(Partition):
+    """
+    Implementation of the abstract base class 'Partition' for date partitioning.
+
+    Defines the methods to format and build the partition.
+    """
+
+    year: Optional[str] = None
+    month: Optional[str] = None
+    day: Optional[str] = None
+    years: Optional[IncrementalRangePartition] = None
+    months: Optional[IncrementalRangePartition] = None
+    days: Optional[IncrementalRangePartition] = None
+
+    def __format_partition(self, partition):
+        """Format the given partition.
+
+        Parameters:
+            partition: The partition to be formatted.
+
+        Returns:
+            The formatted partition.
+        """
+        return f"{set(partition.get())}".replace(" ", "")
+
+    def __build_partition(self):
+        """Build the partition.
+
+        Returns:
+            The list of strings representing the partition.
+        """
+        partition = [
+            self.__format_partition(self.years) if bool(self.years) else self.year
+        ]
+
+        if bool(self.month) or bool(self.months):
+            partition.append(
+                self.__format_partition(self.months)
+                if bool(self.months)
+                else self.month
+            )
+
+        if bool(self.day) or bool(self.days):
+            partition.append(
+                self.__format_partition(self.days) if bool(self.days) else self.day
+            )
+
+        return partition
+
+    def get(self):
+        """Get the partition.
+
+        Returns:
+            The list of strings representing the partition.
+        """
+        return self.__build_partition()
+
+    def get_date(self):
+        """Get the date of the partition.
+
+        Returns:
+            The date of the partition in the format 'YYYY/MM/DD'.
+        """
+        return date(*self.__build_partition()).strftime("%Y/%m/%d")
```

### Comparing `sefazetllib-0.1.33/sefazetllib/validate/DataValidate.py` & `sefazetllib-0.1.34/sefazetllib/validate/DataValidate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,216 +1,214 @@
-from typing import Any, List, Optional
-
-from pydeequ.checks import Check, CheckLevel
-from pydeequ.verification import VerificationResult, VerificationSuite
-from pyspark.sql import Row
-from pyspark.sql.functions import col
-
-from sefazetllib import Builder, field
-from sefazetllib.factory.platform.dataframe.Default import Default
-from sefazetllib.factory.platform.Platform import Platform
-from sefazetllib.validate.Validate import Validate
-
-
-@Builder
-class DataValidate(Validate):
-    df: Optional[Any] = None
-    check: Optional[Any] = None
-    check_name: str = field(default="")
-    custom_check: List[dict] = field(default_factory=list)
-    reference: str = field(default="")
-    output: str = field(default="")
-    platform: Platform = field(default=Default())
-    table_validation: dict = field(default_factory=dict)
-    column_validation: dict = field(default_factory=dict)
-
-    def __get_lambda_assert(self, operator, value):
-        return {
-            "gt": lambda x: x > value,
-            "gte": lambda x: x >= value,
-            "lw": lambda x: x < value,
-            "lwe": lambda x: x <= value,
-            "e": lambda x: x == value,
-        }[operator]
-
-    def __set_custom_check(self, status=False, constraint="", constraint_message=""):
-        if status:
-            self.custom_check.append(
-                {
-                    "check": self.check_name,
-                    "check_level": "Error",
-                    "check_status": "Success",
-                    "constraint": constraint,
-                    "constraint_status": "Success",
-                    "constraint_message": constraint_message,
-                }
-            )
-        else:
-            self.custom_check.append(
-                {
-                    "check": self.check_name,
-                    "check_level": "Error",
-                    "check_status": "Error",
-                    "constraint": constraint,
-                    "constraint_status": "Failure",
-                    "constraint_message": constraint_message,
-                }
-            )
-
-    def __check_columns(self, columns):
-        if set(columns) == set(self.df.columns):
-            self.__set_custom_check(
-                status=True, constraint=f"ColumnsConstraint(Columns({self.reference}))"
-            )
-        else:
-            self.__set_custom_check(
-                status=False,
-                constraint=f"ColumnsConstraint(Columns({self.reference}))",
-                constraint_message=(
-                    "Columns differs by "
-                    + f"{set(columns).symmetric_difference(self.df.columns)}"
-                ),
-            )
-
-    def __check_size(self, assertion, hook_reference):
-        if "reference" in assertion:
-            comparison_df = hook_reference(assertion["reference"])
-
-        if "operator" not in assertion:
-            assertion["operator"] = "igual"
-
-        if "column_reference" not in assertion:
-            assertion["column_reference"] = self.df.columns
-
-        if "value" not in assertion:
-            assertion["value"] = comparison_df.select(
-                assertion["column_reference"]
-            ).count()
-
-        self.check.hasSize(
-            self.__get_lambda_assert(
-                assertion["operator"],
-                assertion["value"],
-            )
-        )
-
-    def __check_distinctness(self, assertion):
-        if assertion:
-            self.check.hasDistinctness(self.df.columns, lambda x: x == 1.0)
-
-    def __unique_key(self, assertion):
-        unique_check = (
-            self.df.groupBy(assertion).count().filter(col("count") > 1).count()
-        )
-
-        if unique_check == 0:
-            self.__set_custom_check(
-                status=True,
-                constraint=f"UniqueKeyConstraint(Columns({assertion}))",
-            )
-        else:
-            self.__set_custom_check(
-                status=False,
-                constraint=f"UniqueKeyConstraint(Columns({assertion}))",
-                constraint_message=(f"Columns {assertion} are not a unique key"),
-            )
-
-    def __check_completeness(self, column, assertion):
-        if isinstance(assertion, dict):
-            self.check.hasCompleteness(
-                column,
-                self.__get_lambda_assert(assertion["operator"], assertion["value"]),
-            )
-        elif assertion:
-            self.check.isComplete(column)
-
-    def __check_uniqueness(self, column, assertion):
-        if isinstance(assertion, dict):
-            self.check.hasUniqueness(
-                [column],
-                self.__get_lambda_assert(assertion["operator"], assertion["value"]),
-            )
-        elif assertion:
-            self.check.isUnique(column)
-
-    def __check_data_type(self, column, column_type):
-        assert_column_type = dict((key, value) for key, value in self.df.dtypes)[column]
-
-        if column_type == assert_column_type:
-            self.__set_custom_check(
-                status=True,
-                constraint=f"DataTypeConstraint(DataType({column}, {column_type}))",
-            )
-        else:
-            self.__set_custom_check(
-                status=False,
-                constraint=f"DataTypeConstraint(DataType({column}, {column_type}))",
-                constraint_message=(
-                    f"{column} of type '{assert_column_type}'"
-                    f"does not meet type '{column_type}' requirement!"
-                ),
-            )
-
-    def __check_min(self, column, value):
-        self.check.hasMin(column, lambda x: x >= value)
-
-    def __check_max(self, column, value):
-        self.check.hasMax(column, lambda x: x <= value)
-
-    def execute(self, **kwargs):
-        if isinstance(self.platform, Default):
-            self.setPlatform(kwargs["platform"])
-
-        if self.check_name == "":
-            self.check_name = f"validacao_{self.reference}"
-
-        self.check = Check(self.platform.session, CheckLevel.Error, self.check_name)
-
-        check_call_map = {
-            "columns": self.__check_columns,
-            "size": self.__check_size,
-            "distinctness": self.__check_distinctness,
-            "unique_key": self.__unique_key,
-            "completeness": self.__check_completeness,
-            "uniqueness": self.__check_uniqueness,
-            "data_type": self.__check_data_type,
-            "min": self.__check_min,
-            "max": self.__check_max,
-            "contained": self.check.isContainedIn,
-        }
-
-        for verification, assertion in self.table_validation.items():
-            if verification == "size":
-                check_call_map[verification](assertion, kwargs["hook_reference"])
-            else:
-                check_call_map[verification](assertion)
-
-        for column, assertion in self.column_validation.items():
-            for verification in assertion.keys():
-                check_call_map[verification](column, assertion[verification])
-
-        if self.custom_check:
-            return (
-                self.output,
-                VerificationResult.checkResultsAsDataFrame(
-                    self.platform.session,
-                    VerificationSuite(self.platform.session)
-                    .onData(self.df)
-                    .addCheck(self.check)
-                    .run(),
-                ).union(
-                    self.platform.session.createDataFrame(
-                        Row(**i) for i in self.custom_check
-                    )
-                ),
-            )
-
-        return (
-            self.output,
-            VerificationResult.checkResultsAsDataFrame(
-                self.platform.session,
-                VerificationSuite(self.platform.session)
-                .onData(self.df)
-                .addCheck(self.check)
-                .run(),
-            ),
-        )
+from typing import Any, List, Optional
+
+from pydeequ.checks import Check, CheckLevel
+from pydeequ.verification import VerificationResult, VerificationSuite
+from pyspark.sql import Row
+from pyspark.sql.functions import col
+
+from sefazetllib import Builder, field
+from sefazetllib.factory.platform.dataframe.Default import Default
+from sefazetllib.factory.platform.Platform import Platform
+from sefazetllib.validate.Validate import Validate
+
+
+@Builder
+class DataValidate(Validate):
+    df: Optional[Any] = None
+    check: Optional[Any] = None
+    check_name: str = field(default="")
+    custom_check: List[dict] = field(default_factory=list)
+    reference: str = field(default="")
+    output: str = field(default="")
+    platform: Platform = field(default=Default())
+    table_validation: dict = field(default_factory=dict)
+    column_validation: dict = field(default_factory=dict)
+
+    def __get_lambda_assert(self, operator, value):
+        return {
+            "gt": lambda x: x > value,
+            "gte": lambda x: x >= value,
+            "lw": lambda x: x < value,
+            "lwe": lambda x: x <= value,
+            "e": lambda x: x == value,
+        }[operator]
+
+    def __set_custom_check(self, status=False, constraint="", constraint_message=""):
+        if status:
+            self.custom_check.append(
+                {
+                    "check": self.check_name,
+                    "check_level": "Error",
+                    "check_status": "Success",
+                    "constraint": constraint,
+                    "constraint_status": "Success",
+                    "constraint_message": constraint_message,
+                }
+            )
+        else:
+            self.custom_check.append(
+                {
+                    "check": self.check_name,
+                    "check_level": "Error",
+                    "check_status": "Error",
+                    "constraint": constraint,
+                    "constraint_status": "Failure",
+                    "constraint_message": constraint_message,
+                }
+            )
+
+    def __check_columns(self, columns):
+        missing_columns = list(filter(lambda col: col not in self.df.columns, columns))
+        if not missing_columns:
+            self.__set_custom_check(
+                status=True, constraint=f"ColumnsConstraint(Columns({self.reference}))"
+            )
+        else:
+            self.__set_custom_check(
+                status=False,
+                constraint=f"ColumnsConstraint(Columns({self.reference}))",
+                constraint_message=(f"Missing columns: {missing_columns}"),
+            )
+
+    def __check_size(self, assertion, hook_reference):
+        if "reference" in assertion:
+            comparison_df = hook_reference(assertion["reference"])
+
+        if "operator" not in assertion:
+            assertion["operator"] = "igual"
+
+        if "column_reference" not in assertion:
+            assertion["column_reference"] = self.df.columns
+
+        if "value" not in assertion:
+            assertion["value"] = comparison_df.select(
+                assertion["column_reference"]
+            ).count()
+
+        self.check.hasSize(
+            self.__get_lambda_assert(
+                assertion["operator"],
+                assertion["value"],
+            )
+        )
+
+    def __check_distinctness(self, assertion):
+        if assertion:
+            self.check.hasDistinctness(self.df.columns, lambda x: x == 1.0)
+
+    def __unique_key(self, assertion):
+        unique_check = (
+            self.df.groupBy(assertion).count().filter(col("count") > 1).count()
+        )
+
+        if unique_check == 0:
+            self.__set_custom_check(
+                status=True,
+                constraint=f"UniqueKeyConstraint(Columns({assertion}))",
+            )
+        else:
+            self.__set_custom_check(
+                status=False,
+                constraint=f"UniqueKeyConstraint(Columns({assertion}))",
+                constraint_message=(f"Columns {assertion} are not a unique key"),
+            )
+
+    def __check_completeness(self, column, assertion):
+        if isinstance(assertion, dict):
+            self.check.hasCompleteness(
+                column,
+                self.__get_lambda_assert(assertion["operator"], assertion["value"]),
+            )
+        elif assertion:
+            self.check.isComplete(column)
+
+    def __check_uniqueness(self, column, assertion):
+        if isinstance(assertion, dict):
+            self.check.hasUniqueness(
+                [column],
+                self.__get_lambda_assert(assertion["operator"], assertion["value"]),
+            )
+        elif assertion:
+            self.check.isUnique(column)
+
+    def __check_data_type(self, column, column_type):
+        assert_column_type = dict((key, value) for key, value in self.df.dtypes)[column]
+
+        if column_type == assert_column_type:
+            self.__set_custom_check(
+                status=True,
+                constraint=f"DataTypeConstraint(DataType({column}, {column_type}))",
+            )
+        else:
+            self.__set_custom_check(
+                status=False,
+                constraint=f"DataTypeConstraint(DataType({column}, {column_type}))",
+                constraint_message=(
+                    f"{column} of type '{assert_column_type}'"
+                    f"does not meet type '{column_type}' requirement!"
+                ),
+            )
+
+    def __check_min(self, column, value):
+        self.check.hasMin(column, lambda x: x >= value)
+
+    def __check_max(self, column, value):
+        self.check.hasMax(column, lambda x: x <= value)
+
+    def execute(self, **kwargs):
+        if isinstance(self.platform, Default):
+            self.setPlatform(kwargs["platform"])
+
+        if self.check_name == "":
+            self.check_name = f"validacao_{self.reference}"
+
+        self.check = Check(self.platform.session, CheckLevel.Error, self.check_name)
+
+        check_call_map = {
+            "columns": self.__check_columns,
+            "size": self.__check_size,
+            "distinctness": self.__check_distinctness,
+            "unique_key": self.__unique_key,
+            "completeness": self.__check_completeness,
+            "uniqueness": self.__check_uniqueness,
+            "data_type": self.__check_data_type,
+            "min": self.__check_min,
+            "max": self.__check_max,
+            "contained": self.check.isContainedIn,
+        }
+
+        for verification, assertion in self.table_validation.items():
+            if verification == "size":
+                check_call_map[verification](assertion, kwargs["hook_reference"])
+            else:
+                check_call_map[verification](assertion)
+
+        for column, assertion in self.column_validation.items():
+            for verification in assertion.keys():
+                check_call_map[verification](column, assertion[verification])
+
+        if self.custom_check:
+            return (
+                self.output,
+                VerificationResult.checkResultsAsDataFrame(
+                    self.platform.session,
+                    VerificationSuite(self.platform.session)
+                    .onData(self.df)
+                    .addCheck(self.check)
+                    .run(),
+                ).union(
+                    self.platform.session.createDataFrame(
+                        Row(**i) for i in self.custom_check
+                    )
+                ),
+            )
+
+        return (
+            self.output,
+            VerificationResult.checkResultsAsDataFrame(
+                self.platform.session,
+                VerificationSuite(self.platform.session)
+                .onData(self.df)
+                .addCheck(self.check)
+                .run(),
+            ),
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/__init__.py` & `sefazetllib-0.1.34/sefazetllibcli/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import json
-import os
-from pathlib import Path
-
-import click
-import yaml
-
-from .config.logging import logger
-from .generators.etl_generator import ETLGenerator
-
-
-def read_entities(source, source_extension, target_extension):
-    extension_file = os.path.splitext(source)[1]
-    is_folder = not extension_file
-    if is_folder:
-        sources = [
-            f"{source}/{file}"
-            for file in filter(
-                lambda file: source_extension in file, os.listdir(source)
-            )
-        ]
-    else:
-        sources = [source]
-    method = {
-        ".json": json.load,
-        ".yaml": yaml.safe_load,
-    }.get(source_extension, lambda textio: textio.read())
-
-    for src in sources:
-        try:
-            with open(src, "r", encoding="utf-8") as file:
-                yield (
-                    f"{os.path.splitext(os.path.basename(src))[0]}{target_extension}",
-                    method(file),
-                )
-        except Exception as err:
-            logger.error("Um erro ocorreu na leitura dos arquivos: %s", err)
-
-
-@click.version_option(message="Sefazetllib (v%(version)s)")
-@click.group(invoke_without_command=True)
-@click.option(
-    "-t",
-    "--type",
-    type=click.Choice(["json", "yaml"]),
-    default="json",
-    help="File Type",
-)
-@click.option(
-    "--template",
-    type=click.Choice(["sefazetllib"]),
-    default="sefazetllib",
-    help="Template",
-)
-@click.pass_context
-def cli(ctx, type, template):
-    ctx.ensure_object(dict)
-    ctx.obj["extension"] = f".{type}"
-    ctx.obj["generator"] = ETLGenerator
-
-
-@cli.command()
-@click.argument("source", type=click.Path(exists=True))
-@click.argument("target")
-@click.pass_context
-def generate(ctx, source, target):
-    entities = read_entities(source, ctx.obj["extension"], ".py")
-    generator = ctx.obj["generator"](list(entities), target=target)
-    generator.generate()
-
-
-@cli.command()
-@click.argument("source", type=click.Path(exists=True))
-@click.argument("target")
-@click.pass_context
-def derive(ctx, source, target):
-    entities = read_entities(source, ".py", ctx.obj["extension"])
-    generator = ctx.obj["generator"](list(entities), target=target)
-    generator.derive()
-
-
-@cli.command()
-@click.pass_context
-def derive_all(ctx):
-    for path in Path(Path.cwd()).rglob("*.py"):
-        entities = read_entities(str(path.absolute()), ".py", ctx.obj["extension"])
-        generator = ctx.obj["generator"](list(entities), target=f"doc")
-        generator.derive()
-
-
-@cli.command()
-@click.pass_context
-def dependencias(ctx):
-    def verify_optional(extract):
-        try:
-            extract["optional"]
-            return False
-        except:
-            return True
-
-    for path in Path(f"{Path.cwd()}/doc").rglob("*.json"):
-        dependencys = {}
-
-        with open(path) as jsonfile:
-            file_json = json.load(jsonfile)
-            extracts = list(
-                map(
-                    lambda extract: f"{extract['schema']}/{extract['entity']}",
-                    filter(
-                        verify_optional,
-                        filter(lambda etl: etl["type"] == "extract", file_json["ETL"]),
-                    ),
-                )
-            )
-
-            dependencys[file_json["platform"]["name"]] = {
-                extract: False for extract in extracts
-            }
-
-            folder = str(path).replace("doc", "dependencias")
-
-            os.makedirs(os.path.dirname(folder), exist_ok=True)
-            with open(folder, "w+") as f:
-                json.dump(dependencys, f, ensure_ascii=False, indent=4)
+import json
+import os
+from pathlib import Path
+
+import click
+import yaml
+
+from .config.logging import logger
+from .generators.etl_generator import ETLGenerator
+
+
+def read_entities(source, source_extension, target_extension):
+    extension_file = os.path.splitext(source)[1]
+    is_folder = not extension_file
+    if is_folder:
+        sources = [
+            f"{source}/{file}"
+            for file in filter(
+                lambda file: source_extension in file, os.listdir(source)
+            )
+        ]
+    else:
+        sources = [source]
+    method = {
+        ".json": json.load,
+        ".yaml": yaml.safe_load,
+    }.get(source_extension, lambda textio: textio.read())
+
+    for src in sources:
+        try:
+            with open(src, "r", encoding="utf-8") as file:
+                yield (
+                    f"{os.path.splitext(os.path.basename(src))[0]}{target_extension}",
+                    method(file),
+                )
+        except Exception as err:
+            logger.error("Um erro ocorreu na leitura dos arquivos: %s", err)
+
+
+@click.version_option(message="Sefazetllib (v%(version)s)")
+@click.group(invoke_without_command=True)
+@click.option(
+    "-t",
+    "--type",
+    type=click.Choice(["json", "yaml"]),
+    default="json",
+    help="File Type",
+)
+@click.option(
+    "--template",
+    type=click.Choice(["sefazetllib"]),
+    default="sefazetllib",
+    help="Template",
+)
+@click.pass_context
+def cli(ctx, type, template):
+    ctx.ensure_object(dict)
+    ctx.obj["extension"] = f".{type}"
+    ctx.obj["generator"] = ETLGenerator
+
+
+@cli.command()
+@click.argument("source", type=click.Path(exists=True))
+@click.argument("target")
+@click.pass_context
+def generate(ctx, source, target):
+    entities = read_entities(source, ctx.obj["extension"], ".py")
+    generator = ctx.obj["generator"](list(entities), target=target)
+    generator.generate()
+
+
+@cli.command()
+@click.argument("source", type=click.Path(exists=True))
+@click.argument("target")
+@click.pass_context
+def derive(ctx, source, target):
+    entities = read_entities(source, ".py", ctx.obj["extension"])
+    generator = ctx.obj["generator"](list(entities), target=target)
+    generator.derive()
+
+
+@cli.command()
+@click.pass_context
+def derive_all(ctx):
+    for path in Path(Path.cwd()).rglob("*.py"):
+        entities = read_entities(str(path.absolute()), ".py", ctx.obj["extension"])
+        generator = ctx.obj["generator"](list(entities), target=f"doc")
+        generator.derive()
+
+
+@cli.command()
+@click.pass_context
+def dependencias(ctx):
+    def verify_optional(extract):
+        try:
+            extract["optional"]
+            return False
+        except:
+            return True
+
+    for path in Path(f"{Path.cwd()}/doc").rglob("*.json"):
+        dependencys = {}
+
+        with open(path) as jsonfile:
+            file_json = json.load(jsonfile)
+            extracts = list(
+                map(
+                    lambda extract: f"{extract['schema']}/{extract['entity']}",
+                    filter(
+                        verify_optional,
+                        filter(lambda etl: etl["type"] == "extract", file_json["ETL"]),
+                    ),
+                )
+            )
+
+            dependencys[file_json["platform"]["name"]] = {
+                extract: False for extract in extracts
+            }
+
+            folder = str(path).replace("doc", "dependencias")
+
+            os.makedirs(os.path.dirname(folder), exist_ok=True)
+            with open(folder, "w+") as f:
+                json.dump(dependencys, f, ensure_ascii=False, indent=4)
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/config/logging.py` & `sefazetllib-0.1.34/sefazetllibcli/config/logging.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import logging
-
-
-class CustomFormatter(logging.Formatter):
-    """Logging Formatter to add colors and count warning / errors."""
-
-    grey = '\x1b[38;21m'
-    yellow = '\x1b[33;21m'
-    red = '\x1b[31;21m'
-    bold_red = '\x1b[31;1m'
-    reset = '\x1b[0m'
-    info_format = '[%(asctime)s] [%(levelname)s] %(message)s'
-    error_format = '[%(asctime)s] [%(levelname)s] %(message)s (%(module)s.%(funcName)s:%(lineno)d)'
-
-    FORMATS = {
-        logging.DEBUG: grey + info_format + reset,
-        logging.INFO: grey + info_format + reset,
-        logging.WARNING: yellow + error_format + reset,
-        logging.ERROR: red + error_format + reset,
-        logging.CRITICAL: bold_red + error_format + reset,
-    }
-
-    def format(self, record):
-        log_fmt = self.FORMATS.get(record.levelno)
-        formatter = logging.Formatter(log_fmt, datefmt='%Y-%m-%d %H:%M:%S')
-        return formatter.format(record)
-
-
-handler = logging.StreamHandler()
-handler.setFormatter(CustomFormatter())
-handler.setLevel(logging.INFO)
-
-logger = logging.getLogger('sefazetllibcli')
-
-logger.setLevel(logging.INFO)
-logger.addHandler(handler)
+import logging
+
+
+class CustomFormatter(logging.Formatter):
+    """Logging Formatter to add colors and count warning / errors."""
+
+    grey = '\x1b[38;21m'
+    yellow = '\x1b[33;21m'
+    red = '\x1b[31;21m'
+    bold_red = '\x1b[31;1m'
+    reset = '\x1b[0m'
+    info_format = '[%(asctime)s] [%(levelname)s] %(message)s'
+    error_format = '[%(asctime)s] [%(levelname)s] %(message)s (%(module)s.%(funcName)s:%(lineno)d)'
+
+    FORMATS = {
+        logging.DEBUG: grey + info_format + reset,
+        logging.INFO: grey + info_format + reset,
+        logging.WARNING: yellow + error_format + reset,
+        logging.ERROR: red + error_format + reset,
+        logging.CRITICAL: bold_red + error_format + reset,
+    }
+
+    def format(self, record):
+        log_fmt = self.FORMATS.get(record.levelno)
+        formatter = logging.Formatter(log_fmt, datefmt='%Y-%m-%d %H:%M:%S')
+        return formatter.format(record)
+
+
+handler = logging.StreamHandler()
+handler.setFormatter(CustomFormatter())
+handler.setLevel(logging.INFO)
+
+logger = logging.getLogger('sefazetllibcli')
+
+logger.setLevel(logging.INFO)
+logger.addHandler(handler)
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/generators/etl_generator.py` & `sefazetllib-0.1.34/sefazetllibcli/generators/etl_generator.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import json
-import os
-import re
-from dataclasses import dataclass, field
-from pathlib import Path
-
-import yaml
-
-from sefazetllibcli.config.logging import logger
-from sefazetllibcli.errors import UnsupportedFileExtension
-from sefazetllibcli.usecases.replace_template import ReplaceETLTemplate, ReplaceTemplate
-from sefazetllibcli.utils import ParseETL
-
-from .generator import Generator
-
-
-@dataclass
-class ETLGenerator(Generator):
-    template_file: str = field(
-        default=Path(__file__).parent / '../templates/etl_template'
-    )
-    __parse_etl: ParseETL = field(default=ParseETL())
-    replace_template: ReplaceTemplate = field(default=ReplaceETLTemplate)
-    root_path: str = field(default=os.getcwd())
-
-    def generate(self) -> None:
-        for i, entity in enumerate(self.entities):
-            try:
-                etl_name, etl = entity
-
-                logger.info(
-                    '[%s/%s] Iniciando geração do ETL `%s`',
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                )
-
-                logger.info('Executando...')
-
-                replace_template = self.replace_template(
-                    template=self.template,
-                    entity=etl,
-                    sources=None,
-                    columns=None,
-                )
-
-                output = replace_template.replace()
-
-                logger.info('Gravando...')
-
-                path = f'{self.root_path}/{self.target}/{etl_name}'
-                os.makedirs(os.path.dirname(path), exist_ok=True)
-
-                with open(
-                    path,
-                    'w',
-                    encoding='utf-8',
-                ) as file__output:
-                    file__output.write(output)
-
-                logger.info(
-                    '[%s/%s] Geração do ETL `%s` concluída!',
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                )
-            except Exception as err:
-                logger.error(
-                    '[%s/%s] Um erro ocorreu na geração do ETL `%s`: %s',
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                    err,
-                )
-
-    def derive(self) -> None:
-        for i, entity in enumerate(self.entities):
-            try:
-                etl_name, etl = entity
-
-                logger.info(
-                    '[%s/%s] Iniciando derivação do ETL `%s`',
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                )
-
-                logger.info('Executando...')
-
-                # print(self.__get_etl_context(etl))
-                # self.__get_transform_context(etl)
-                # print(self.__get_imports(etl))
-
-                output = self.__parse_etl.parse(self.__get_etl_context(etl))
-
-                path = f'{self.root_path}/{self.target}/{etl_name}'
-                os.makedirs(os.path.dirname(path), exist_ok=True)
-
-                with open(
-                    path,
-                    'w',
-                    encoding='utf-8',
-                ) as file__output:
-                    extension_file = os.path.splitext(path)[1]
-                    if extension_file == '.json':
-                        file__output.write(json.dumps(output, indent=4))
-                    elif extension_file == '.yaml':
-                        file__output.write(yaml.dump(output, indent=4))
-                    else:
-                        raise UnsupportedFileExtension(
-                            f'Extensão de arquivo não suportada: {path}'
-                        )
-
-                logger.info(
-                    '[%s/%s] Derivação do ETL `%s` concluída!',
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                )
-            except Exception as err:
-                logger.error(
-                    '[%s/%s] Um erro ocorreu na geração do ETL `%s`: %s',
-                    i + 1,
-                    len(self.entities),
-                    etl_name,
-                    err,
-                )
-
-    def __get_etl_context(self, script):
-        etl_pattern = re.compile(r'\((ETL.*)\)$')
-
-        minified = re.sub(r'\s', '', script)
-        return etl_pattern.search(minified).group(1)
-
-    def __get_transform_context(self, script):
-        etl_pattern = re.compile(r'(@Builder[\s\S]*?)(?=\n{3})')
-
-        transforms = etl_pattern.findall(script)
-
-        for transform in transforms:
-            self.__get_transform_references(transform)
-            self.__get_transform_setup(transform)
-            self.__get_transform_private_methods(transform)
-            self.__get_transform_method(transform)
-
-        # return etl_pattern.search(minified).group(1)
-
-    def __get_transform_references(self, transform):
-        etl_pattern = re.compile(
-            r'([(A-Z)|(a-z)].*?): Optional\[DataFrame\] = None')
-
-        return etl_pattern.findall(transform)
-
-    def __get_transform_setup(self, transform):
-        etl_pattern = re.compile(
-            r'self.__(\w[A-Z|a-z].*) = (Window*[\s\S]*?\)\n|[^\(][\s\S]*?\n|\([\s\S]*?\s\))')
-
-        return etl_pattern.findall(transform)
-
-    def __get_transform_private_methods(self, transform):
-        etl_pattern = re.compile(
-            r'def __(\w[A-Z|a-z].*)\(self\):([^\(][\s\S]*?\s\n)')
-
-        return etl_pattern.findall(transform)
-
-    def __get_transform_method(self, transform):
-        etl_pattern = re.compile(
-            r'def execute\(self\) \-> Tuple\[str, DataFrame\]:([\s\S]*?)\sreturn.*\n\s*.?\"([\s\S].*)\"\,([\s\S]*?)\)\n\n')
-        print(etl_pattern.findall(etl_pattern))
-
-    def __get_imports(self, etl):
-        etl_pattern = re.compile(
-            r'from ([^sefazetllib]\w.*) import ([^\(][\s\S]*?\n|[\(][\s\S]*?\s[\)])')
-        return etl_pattern.findall(etl)
+import json
+import os
+import re
+from dataclasses import dataclass, field
+from pathlib import Path
+
+import yaml
+
+from sefazetllibcli.config.logging import logger
+from sefazetllibcli.errors import UnsupportedFileExtension
+from sefazetllibcli.usecases.replace_template import ReplaceETLTemplate, ReplaceTemplate
+from sefazetllibcli.utils import ParseETL
+
+from .generator import Generator
+
+
+@dataclass
+class ETLGenerator(Generator):
+    template_file: str = field(
+        default=Path(__file__).parent / '../templates/etl_template'
+    )
+    __parse_etl: ParseETL = field(default=ParseETL())
+    replace_template: ReplaceTemplate = field(default=ReplaceETLTemplate)
+    root_path: str = field(default=os.getcwd())
+
+    def generate(self) -> None:
+        for i, entity in enumerate(self.entities):
+            try:
+                etl_name, etl = entity
+
+                logger.info(
+                    '[%s/%s] Iniciando geração do ETL `%s`',
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                )
+
+                logger.info('Executando...')
+
+                replace_template = self.replace_template(
+                    template=self.template,
+                    entity=etl,
+                    sources=None,
+                    columns=None,
+                )
+
+                output = replace_template.replace()
+
+                logger.info('Gravando...')
+
+                path = f'{self.root_path}/{self.target}/{etl_name}'
+                os.makedirs(os.path.dirname(path), exist_ok=True)
+
+                with open(
+                    path,
+                    'w',
+                    encoding='utf-8',
+                ) as file__output:
+                    file__output.write(output)
+
+                logger.info(
+                    '[%s/%s] Geração do ETL `%s` concluída!',
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                )
+            except Exception as err:
+                logger.error(
+                    '[%s/%s] Um erro ocorreu na geração do ETL `%s`: %s',
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                    err,
+                )
+
+    def derive(self) -> None:
+        for i, entity in enumerate(self.entities):
+            try:
+                etl_name, etl = entity
+
+                logger.info(
+                    '[%s/%s] Iniciando derivação do ETL `%s`',
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                )
+
+                logger.info('Executando...')
+
+                # print(self.__get_etl_context(etl))
+                # self.__get_transform_context(etl)
+                # print(self.__get_imports(etl))
+
+                output = self.__parse_etl.parse(self.__get_etl_context(etl))
+
+                path = f'{self.root_path}/{self.target}/{etl_name}'
+                os.makedirs(os.path.dirname(path), exist_ok=True)
+
+                with open(
+                    path,
+                    'w',
+                    encoding='utf-8',
+                ) as file__output:
+                    extension_file = os.path.splitext(path)[1]
+                    if extension_file == '.json':
+                        file__output.write(json.dumps(output, indent=4))
+                    elif extension_file == '.yaml':
+                        file__output.write(yaml.dump(output, indent=4))
+                    else:
+                        raise UnsupportedFileExtension(
+                            f'Extensão de arquivo não suportada: {path}'
+                        )
+
+                logger.info(
+                    '[%s/%s] Derivação do ETL `%s` concluída!',
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                )
+            except Exception as err:
+                logger.error(
+                    '[%s/%s] Um erro ocorreu na geração do ETL `%s`: %s',
+                    i + 1,
+                    len(self.entities),
+                    etl_name,
+                    err,
+                )
+
+    def __get_etl_context(self, script):
+        etl_pattern = re.compile(r'\((ETL.*)\)$')
+
+        minified = re.sub(r'\s', '', script)
+        return etl_pattern.search(minified).group(1)
+
+    def __get_transform_context(self, script):
+        etl_pattern = re.compile(r'(@Builder[\s\S]*?)(?=\n{3})')
+
+        transforms = etl_pattern.findall(script)
+
+        for transform in transforms:
+            self.__get_transform_references(transform)
+            self.__get_transform_setup(transform)
+            self.__get_transform_private_methods(transform)
+            self.__get_transform_method(transform)
+
+        # return etl_pattern.search(minified).group(1)
+
+    def __get_transform_references(self, transform):
+        etl_pattern = re.compile(
+            r'([(A-Z)|(a-z)].*?): Optional\[DataFrame\] = None')
+
+        return etl_pattern.findall(transform)
+
+    def __get_transform_setup(self, transform):
+        etl_pattern = re.compile(
+            r'self.__(\w[A-Z|a-z].*) = (Window*[\s\S]*?\)\n|[^\(][\s\S]*?\n|\([\s\S]*?\s\))')
+
+        return etl_pattern.findall(transform)
+
+    def __get_transform_private_methods(self, transform):
+        etl_pattern = re.compile(
+            r'def __(\w[A-Z|a-z].*)\(self\):([^\(][\s\S]*?\s\n)')
+
+        return etl_pattern.findall(transform)
+
+    def __get_transform_method(self, transform):
+        etl_pattern = re.compile(
+            r'def execute\(self\) \-> Tuple\[str, DataFrame\]:([\s\S]*?)\sreturn.*\n\s*.?\"([\s\S].*)\"\,([\s\S]*?)\)\n\n')
+        print(etl_pattern.findall(etl_pattern))
+
+    def __get_imports(self, etl):
+        etl_pattern = re.compile(
+            r'from ([^sefazetllib]\w.*) import ([^\(][\s\S]*?\n|[\(][\s\S]*?\s[\)])')
+        return etl_pattern.findall(etl)
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/generators/generator.py` & `sefazetllib-0.1.34/sefazetllibcli/generators/generator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
-from io import TextIOWrapper
-
-from sefazetllibcli.errors import MethodNotImplemented
-from sefazetllibcli.usecases.replace_template import ReplaceTemplate
-
-
-@dataclass(init=False)
-class Generator(ABC):
-    entities: list = field(default_factory=list)
-    template_file: str = field(default_factory=str)
-    root_path: str = field(default_factory=str)
-    target: str = field(default_factory=str)
-    replace_template: ReplaceTemplate = field(default=None)
-    template: str = field(init=False, default=None)
-
-    def __post_init__(self):
-        with open(self.template_file, 'r', encoding='utf-8') as file_template:
-            object.__setattr__(self, 'template', file_template.read())
-
-    @abstractmethod
-    def generate(self):
-        raise MethodNotImplemented('Deve implementar o método: proccess')
+from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
+from io import TextIOWrapper
+
+from sefazetllibcli.errors import MethodNotImplemented
+from sefazetllibcli.usecases.replace_template import ReplaceTemplate
+
+
+@dataclass(init=False)
+class Generator(ABC):
+    entities: list = field(default_factory=list)
+    template_file: str = field(default_factory=str)
+    root_path: str = field(default_factory=str)
+    target: str = field(default_factory=str)
+    replace_template: ReplaceTemplate = field(default=None)
+    template: str = field(init=False, default=None)
+
+    def __post_init__(self):
+        with open(self.template_file, 'r', encoding='utf-8') as file_template:
+            object.__setattr__(self, 'template', file_template.read())
+
+    @abstractmethod
+    def generate(self):
+        raise MethodNotImplemented('Deve implementar o método: proccess')
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/__init__.py` & `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .process_etl_variable import ProcessETLVariable
-from .process_extract_variable import ProcessExtractVariable
-from .process_imports_variable import ProcessImportsVariable
-from .process_key_variable import ProcessKeyVariable
-from .process_load_variable import ProcessLoadVariable
-from .process_partition_variable import ProcessPartitionVariable
-from .process_transforms_variable import ProcessTransformsVariable
-from .process_validate_variable import ProcessValidateVariable
-from .process_variable import ProcessVariable
+from .process_etl_variable import ProcessETLVariable
+from .process_extract_variable import ProcessExtractVariable
+from .process_imports_variable import ProcessImportsVariable
+from .process_key_variable import ProcessKeyVariable
+from .process_load_variable import ProcessLoadVariable
+from .process_partition_variable import ProcessPartitionVariable
+from .process_transforms_variable import ProcessTransformsVariable
+from .process_validate_variable import ProcessValidateVariable
+from .process_variable import ProcessVariable
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_etl_variable.py` & `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_etl_variable.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-import json
-
-from .process_variable import ProcessVariable
-
-
-class ProcessETLVariable(ProcessVariable):
-    """Classe `ProcessETLVariable`.
-
-    A classe implementa o procedimento da saída da variavel `ETL`.
-    """
-
-    variable = 'ETL'
-
-    def _get_platform(self, platform):
-        factory = platform['factory']
-        name = platform['name']
-        return (
-            f'.setPlatform(PlatformFactory("{factory}").create(name="{name}"))'
-        )
-
-    def _get_properties(self, properties, skip_columns=None, height=1):
-        props = []
-        for prop, value in properties.items():
-            if prop not in skip_columns:
-                prop_str = ''.join(
-                    [word.capitalize() for word in prop.split('_')]
-                )
-                if isinstance(value, str):
-                    value = f'"{value}"'
-                elif isinstance(value, dict):
-                    tabs = '\t' * height
-                    if 'factory' in value:
-                        value = (
-                            '\n'
-                            + tabs
-                            + '\t'
-                            + self._visit_factory(value, height + 1)
-                            + '\n'
-                            + tabs
-                        )
-                    else:
-                        value = (
-                            json.dumps(value, indent=4 * (height + 1))
-                            .replace('}', tabs + '}')
-                            .replace('true', 'True')
-                            .replace('false', 'False')
-                        )
-                props.append(f'.set{prop_str}({value})')
-        return props
-
-    def _visit_factory(self, factory, height):
-        name = f'{factory["factory"]}()'
-        properties = self._get_properties(factory, ['factory', 'type'], height)
-        tabs = '\n' + '\t' * height
-        properties = tabs.join(properties)
-        return name + tabs + properties
-
-    def _get_etl(self, etls):
-        list_etl = []
-        for etl in etls:
-            etl_type = etl['type']
-            value = (
-                etl['name']
-                if etl_type == 'transform'
-                else self._visit_factory(etl, 2)
-            )
-            tabs_ini = '\n\t\t'
-            tabs_end = '\n\t'
-            if etl_type == 'transform':
-                tabs_ini = ''
-                tabs_end = ''
-            list_etl.append(f'.{etl_type}({tabs_ini}{value}{tabs_end})')
-
-        return '\n\t'.join(list_etl)
-
-    def process(self, entity, sources, columns):
-        """Retorna uma string do processamento da variável.
-
-        Parâmetros:
-            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
-            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
-            notebook original da entidade.
-            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
-            original.
-        Saída:
-            `processed_variable (str)`: String do processamento da variável.
-        """
-        platform = '\n\t' + self._get_platform(entity['platform'])
-        properties = self._get_properties(
-            entity,
-            skip_columns=['platform', 'ETL'],
-            height=1,
-        )
-        properties = '\n\t' + '\n\t'.join(properties) if properties else ''
-        print('inicio')
-        etls = '\n\t' + self._get_etl(entity['ETL'])
-        print('fim')
-        return '(\n\tETL()' + f'{platform}{properties}{etls}\n)'
+import json
+
+from .process_variable import ProcessVariable
+
+
+class ProcessETLVariable(ProcessVariable):
+    """Classe `ProcessETLVariable`.
+
+    A classe implementa o procedimento da saída da variavel `ETL`.
+    """
+
+    variable = 'ETL'
+
+    def _get_platform(self, platform):
+        factory = platform['factory']
+        name = platform['name']
+        return (
+            f'.setPlatform(PlatformFactory("{factory}").create(name="{name}"))'
+        )
+
+    def _get_properties(self, properties, skip_columns=None, height=1):
+        props = []
+        for prop, value in properties.items():
+            if prop not in skip_columns:
+                prop_str = ''.join(
+                    [word.capitalize() for word in prop.split('_')]
+                )
+                if isinstance(value, str):
+                    value = f'"{value}"'
+                elif isinstance(value, dict):
+                    tabs = '\t' * height
+                    if 'factory' in value:
+                        value = (
+                            '\n'
+                            + tabs
+                            + '\t'
+                            + self._visit_factory(value, height + 1)
+                            + '\n'
+                            + tabs
+                        )
+                    else:
+                        value = (
+                            json.dumps(value, indent=4 * (height + 1))
+                            .replace('}', tabs + '}')
+                            .replace('true', 'True')
+                            .replace('false', 'False')
+                        )
+                props.append(f'.set{prop_str}({value})')
+        return props
+
+    def _visit_factory(self, factory, height):
+        name = f'{factory["factory"]}()'
+        properties = self._get_properties(factory, ['factory', 'type'], height)
+        tabs = '\n' + '\t' * height
+        properties = tabs.join(properties)
+        return name + tabs + properties
+
+    def _get_etl(self, etls):
+        list_etl = []
+        for etl in etls:
+            etl_type = etl['type']
+            value = (
+                etl['name']
+                if etl_type == 'transform'
+                else self._visit_factory(etl, 2)
+            )
+            tabs_ini = '\n\t\t'
+            tabs_end = '\n\t'
+            if etl_type == 'transform':
+                tabs_ini = ''
+                tabs_end = ''
+            list_etl.append(f'.{etl_type}({tabs_ini}{value}{tabs_end})')
+
+        return '\n\t'.join(list_etl)
+
+    def process(self, entity, sources, columns):
+        """Retorna uma string do processamento da variável.
+
+        Parâmetros:
+            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
+            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
+            notebook original da entidade.
+            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
+            original.
+        Saída:
+            `processed_variable (str)`: String do processamento da variável.
+        """
+        platform = '\n\t' + self._get_platform(entity['platform'])
+        properties = self._get_properties(
+            entity,
+            skip_columns=['platform', 'ETL'],
+            height=1,
+        )
+        properties = '\n\t' + '\n\t'.join(properties) if properties else ''
+        print('inicio')
+        etls = '\n\t' + self._get_etl(entity['ETL'])
+        print('fim')
+        return '(\n\tETL()' + f'{platform}{properties}{etls}\n)'
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_extract_variable.py` & `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_validate_variable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from .process_variable import ProcessVariable
-
-
-class ProcessExtractVariable(ProcessVariable):
-    """Classe `ProcessExtractVariable`.
-
-    A classe implementa o procedimento da saída da variavel `EXTRACT`.
-    """
-
-    variable = 'EXTRACT'
-
-    def process(self, entity, sources, columns):
-        """Retorna uma string do processamento da variável.
-
-        Parâmetros:
-            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
-            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
-            notebook original da entidade.
-            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
-            original.
-        Saída:
-            `processed_variable (str)`: String do processamento da variável.
-        """
-        factories = [
-            etl['factory'] for etl in entity['ETL'] if etl['type'] == 'extract'
-        ]
-        factories_without_duplicates = [*set(factories)]
-        factories_without_duplicates.sort()
-
-        return 'from sefazetllib.extract import '+', '.join(factories_without_duplicates) if bool(factories_without_duplicates) else ''
+from .process_variable import ProcessVariable
+
+
+class ProcessValidateVariable(ProcessVariable):
+    """Classe `ProcessExtractVariable`.
+
+    A classe implementa o procedimento da saída da variavel `EXTRACT`.
+    """
+
+    variable = 'VALIDATE'
+
+    def process(self, entity, sources, columns):
+        """Retorna uma string do processamento da variável.
+
+        Parâmetros:
+            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
+            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
+            notebook original da entidade.
+            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
+            original.
+        Saída:
+            `processed_variable (str)`: String do processamento da variável.
+        """
+        factories = [
+            etl['factory']
+            for etl in entity['ETL']
+            if etl['type'] == 'validate'
+        ]
+        factories_without_duplicates = [*set(factories)]
+        factories_without_duplicates.sort()
+
+        return ', '.join(factories_without_duplicates)
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_partition_variable.py` & `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_partition_variable.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from .process_variable import ProcessVariable
-
-
-class ProcessPartitionVariable(ProcessVariable):
-    """Classe `ProcessPartitionVariable`.
-
-    A classe implementa o procedimento da saída da variavel `PARTITION`.
-    """
-
-    variable = 'PARTITION'
-
-    def _get_factories(self, dictionary, factories):
-        for prop, value in dictionary.items():
-            if (
-                prop != 'factory'
-                and isinstance(value, dict)
-                and 'factory' in value
-            ):
-                factories.append(value['factory'])
-                self._get_factories(value, factories)
-
-    def process(self, entity, sources, columns):
-        """Retorna uma string do processamento da variável.
-
-        Parâmetros:
-            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
-            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
-            notebook original da entidade.
-            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
-            original.
-        Saída:
-            `processed_variable (str)`: String do processamento da variável.
-        """
-        if 'partition' in entity:
-            partitions = entity['partition']
-            factories = [partitions['factory']]
-            self._get_factories(entity['partition'], factories)
-
-            factories_without_duplicates = [*set(factories)]
-            factories_without_duplicates.sort()
-
-            return 'from sefazetllib.utils.partition import ' + ', '.join(
-                factories_without_duplicates
-            )
-        return ''
+from .process_variable import ProcessVariable
+
+
+class ProcessPartitionVariable(ProcessVariable):
+    """Classe `ProcessPartitionVariable`.
+
+    A classe implementa o procedimento da saída da variavel `PARTITION`.
+    """
+
+    variable = 'PARTITION'
+
+    def _get_factories(self, dictionary, factories):
+        for prop, value in dictionary.items():
+            if (
+                prop != 'factory'
+                and isinstance(value, dict)
+                and 'factory' in value
+            ):
+                factories.append(value['factory'])
+                self._get_factories(value, factories)
+
+    def process(self, entity, sources, columns):
+        """Retorna uma string do processamento da variável.
+
+        Parâmetros:
+            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
+            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
+            notebook original da entidade.
+            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
+            original.
+        Saída:
+            `processed_variable (str)`: String do processamento da variável.
+        """
+        if 'partition' in entity:
+            partitions = entity['partition']
+            factories = [partitions['factory']]
+            self._get_factories(entity['partition'], factories)
+
+            factories_without_duplicates = [*set(factories)]
+            factories_without_duplicates.sort()
+
+            return 'from sefazetllib.utils.partition import ' + ', '.join(
+                factories_without_duplicates
+            )
+        return ''
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/usecases/process_variable/process_variable.py` & `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_imports_variable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from abc import ABC, abstractmethod
-
-from sefazetllibcli.errors import MethodNotImplemented
-
-
-class ProcessVariable(ABC):
-    """Interface `ProcessVariable`.
-
-    A interface define como as suas classes que a implemêntam devem processar a
-    saída da variável em questão.
-    """
-
-    variable = ''
-
-    @abstractmethod
-    def process(self, entity, sources, columns):
-        """Retorna uma string do processamento da variável.
-
-        Parâmetros:
-            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
-            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
-            notebook original da entidade.
-            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
-            original.
-        Saída:
-            `processed_variable (str)`: String do processamento da variável.
-        """
-        raise MethodNotImplemented('Deve implementar o método: proccess')
+from .process_variable import ProcessVariable
+
+
+class ProcessImportsVariable(ProcessVariable):
+    """Classe `ProcessExtractVariable`.
+
+    A classe implementa o procedimento da saída da variavel `IMPORTS`.
+    """
+
+    variable = 'IMPORTS'
+
+    def process(self, entity, sources, columns):
+        """Retorna uma string do processamento da variável.
+
+        Parâmetros:
+            - `entity (Dict)`: Entidade que terá um notebook de teste gerado.
+            - `sources (List[Dict])`: Dataframes das fontes que são usadas no
+            notebook original da entidade.
+            - `columns (Dict)`: Colunas do Dataframe gerado pelo notebook
+            original.
+        Saída:
+            `processed_variable (str)`: String do processamento da variável.
+        """
+
+        return {
+            "Pandas": "from pandas import *",
+            "Spark": "from pyspark.sql import DataFrame, Window \nfrom pyspark.sql.functions import *"
+        }[entity['platform']['factory']]
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/usecases/replace_template/replace_etl_template.py` & `sefazetllib-0.1.34/sefazetllibcli/usecases/replace_template/replace_etl_template.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from sefazetllibcli.usecases.process_variable import (
-    ProcessETLVariable,
-    ProcessExtractVariable,
-    ProcessImportsVariable,
-    ProcessKeyVariable,
-    ProcessLoadVariable,
-    ProcessPartitionVariable,
-    ProcessTransformsVariable,
-    ProcessValidateVariable,
-)
-
-from .replace_template import ReplaceTemplate
-
-
-class ReplaceETLTemplate(ReplaceTemplate):
-    """Classe `ReplaceETLTemplate`.
-
-    A classe tem a finalidade de substituir as variáveis que estão definidas no
-    template.
-    """
-
-    def replace(self):
-        """Retorna o template com todas variáveis da lista já substituídas."""
-        return self.replace_variables(
-            ProcessETLVariable(),
-            ProcessExtractVariable(),
-            ProcessImportsVariable(),
-            ProcessKeyVariable(),
-            ProcessLoadVariable(),
-            ProcessPartitionVariable(),
-            ProcessTransformsVariable(),
-            ProcessValidateVariable(),
-        )
+from sefazetllibcli.usecases.process_variable import (
+    ProcessETLVariable,
+    ProcessExtractVariable,
+    ProcessImportsVariable,
+    ProcessKeyVariable,
+    ProcessLoadVariable,
+    ProcessPartitionVariable,
+    ProcessTransformsVariable,
+    ProcessValidateVariable,
+)
+
+from .replace_template import ReplaceTemplate
+
+
+class ReplaceETLTemplate(ReplaceTemplate):
+    """Classe `ReplaceETLTemplate`.
+
+    A classe tem a finalidade de substituir as variáveis que estão definidas no
+    template.
+    """
+
+    def replace(self):
+        """Retorna o template com todas variáveis da lista já substituídas."""
+        return self.replace_variables(
+            ProcessETLVariable(),
+            ProcessExtractVariable(),
+            ProcessImportsVariable(),
+            ProcessKeyVariable(),
+            ProcessLoadVariable(),
+            ProcessPartitionVariable(),
+            ProcessTransformsVariable(),
+            ProcessValidateVariable(),
+        )
```

### Comparing `sefazetllib-0.1.33/sefazetllibcli/utils/parse_etl.py` & `sefazetllib-0.1.34/sefazetllibcli/utils/parse_etl.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import ast
-import re
-
-
-class ParseETL:
-    def parse(self, string):
-        current_dict = {}
-        key = ''
-        value = ''
-        count = 0
-        for char in string:
-            if char == '(':
-                if count == 0:
-                    key = re.sub(r'^\.', '', value)
-                    value = ''
-                else:
-                    value += char
-                count += 1
-            elif char == ')':
-                count -= 1
-                if count == 0:
-                    key, current_dict, value = self._get_context(
-                        key, current_dict, value
-                    )
-                    value = ''
-                else:
-                    value += char
-            else:
-                value += char
-        if not key:
-            current_dict = self._parse_value(value)
-        return current_dict
-
-    def _validate_key(self, key):
-        if key != 'ETL':
-            if key.startswith('set'):
-                key = '_'.join(self._split_camel_case(key[3:]).split())
-            return key
-        return None
-
-    def __get_objects_by_pattern(self, value):
-        try:
-            platform_pattern = re.compile(
-                r"PlatformFactory\(['\"]([^'\"]+)['\"]\).create\(name=['\"]([^'\"]+)['\"]\,configs=(\[(.*?)\])"
-            )
-            [factory, name, config, *
-                args] = platform_pattern.search(value).groups()
-            return {
-                'factory': factory,
-                'name': name,
-                'config': ast.literal_eval(config)
-            }
-        except AttributeError:
-            platform_pattern = re.compile(
-                r"PlatformFactory\(['\"]([^'\"]+)['\"]\).create\(name=['\"]([^'\"]+)['\"]\)"
-            )
-            factory, name = platform_pattern.search(value).groups()
-            return {
-                'factory': factory,
-                'name': name,
-            }
-
-    def _process_platform_key(self, key, value):
-        if key == 'platform':
-            return self.__get_objects_by_pattern(value)
-        return None
-
-    def _process_etl_keys(self, key, current_dict, value):
-        if key == 'ETL':
-            if key not in current_dict:
-                current_dict[key] = []
-            current_dict[key].append(self.parse(value))
-        else:
-            current_dict[key] = self.parse(value)
-        return current_dict[key]
-
-    def _swap_key_value(self, key, value):
-        if not value:
-            value = 'factory'
-        if value == 'factory':
-            key, value = value, key
-        elif key in ['extract', 'load', 'transform', 'validate']:
-            if key == 'transform':
-                value = f'.setType({key}).setName({value})'
-            else:
-                value = f'.setType({key})' + value
-            key = 'ETL'
-        return key, value
-
-    def _get_context(self, key, current_dict, value):
-        key = self._validate_key(key)
-        processed_value = self._process_platform_key(key, value)
-        if processed_value:
-            current_dict[key] = processed_value
-        elif key:
-            key, value = self._swap_key_value(key, value)
-            current_dict[key] = self._process_etl_keys(
-                key, current_dict, value
-            )
-        return key, current_dict, value
-
-    def _split_camel_case(self, name):
-        return (
-            re.sub('([A-Z][a-z]+)', r' \1', re.sub('([A-Z]+)', r' \1', name))
-            .lower()
-            .strip()
-        )
-
-    def _parse_value(self, value):
-        try:
-            return ast.literal_eval(value)
-        except (ValueError, SyntaxError):
-            return value
+import ast
+import re
+
+
+class ParseETL:
+    def parse(self, string):
+        current_dict = {}
+        key = ''
+        value = ''
+        count = 0
+        for char in string:
+            if char == '(':
+                if count == 0:
+                    key = re.sub(r'^\.', '', value)
+                    value = ''
+                else:
+                    value += char
+                count += 1
+            elif char == ')':
+                count -= 1
+                if count == 0:
+                    key, current_dict, value = self._get_context(
+                        key, current_dict, value
+                    )
+                    value = ''
+                else:
+                    value += char
+            else:
+                value += char
+        if not key:
+            current_dict = self._parse_value(value)
+        return current_dict
+
+    def _validate_key(self, key):
+        if key != 'ETL':
+            if key.startswith('set'):
+                key = '_'.join(self._split_camel_case(key[3:]).split())
+            return key
+        return None
+
+    def __get_objects_by_pattern(self, value):
+        try:
+            platform_pattern = re.compile(
+                r"PlatformFactory\(['\"]([^'\"]+)['\"]\).create\(name=['\"]([^'\"]+)['\"]\,configs=(\[(.*?)\])"
+            )
+            [factory, name, config, *
+                args] = platform_pattern.search(value).groups()
+            return {
+                'factory': factory,
+                'name': name,
+                'config': ast.literal_eval(config)
+            }
+        except AttributeError:
+            platform_pattern = re.compile(
+                r"PlatformFactory\(['\"]([^'\"]+)['\"]\).create\(name=['\"]([^'\"]+)['\"]\)"
+            )
+            factory, name = platform_pattern.search(value).groups()
+            return {
+                'factory': factory,
+                'name': name,
+            }
+
+    def _process_platform_key(self, key, value):
+        if key == 'platform':
+            return self.__get_objects_by_pattern(value)
+        return None
+
+    def _process_etl_keys(self, key, current_dict, value):
+        if key == 'ETL':
+            if key not in current_dict:
+                current_dict[key] = []
+            current_dict[key].append(self.parse(value))
+        else:
+            current_dict[key] = self.parse(value)
+        return current_dict[key]
+
+    def _swap_key_value(self, key, value):
+        if not value:
+            value = 'factory'
+        if value == 'factory':
+            key, value = value, key
+        elif key in ['extract', 'load', 'transform', 'validate']:
+            if key == 'transform':
+                value = f'.setType({key}).setName({value})'
+            else:
+                value = f'.setType({key})' + value
+            key = 'ETL'
+        return key, value
+
+    def _get_context(self, key, current_dict, value):
+        key = self._validate_key(key)
+        processed_value = self._process_platform_key(key, value)
+        if processed_value:
+            current_dict[key] = processed_value
+        elif key:
+            key, value = self._swap_key_value(key, value)
+            current_dict[key] = self._process_etl_keys(
+                key, current_dict, value
+            )
+        return key, current_dict, value
+
+    def _split_camel_case(self, name):
+        return (
+            re.sub('([A-Z][a-z]+)', r' \1', re.sub('([A-Z]+)', r' \1', name))
+            .lower()
+            .strip()
+        )
+
+    def _parse_value(self, value):
+        try:
+            return ast.literal_eval(value)
+        except (ValueError, SyntaxError):
+            return value
```

### Comparing `sefazetllib-0.1.33/setup.py` & `sefazetllib-0.1.34/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: sefazetllib
+Version: 0.1.34
+Summary: sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
+Home-page: https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
+License: Apache-2.0
+Author: Felipe Gochi
+Author-email: felipe.gochi@elogroup.com.br
+Maintainer: Bruno Santos
+Maintainer-email: bruno.santos@elogroup.com.br
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: boto3 (>=1.24,<2.0)
+Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: pyarrow (>=6.0,<7.0)
+Requires-Dist: pydeequ (>=1.0,<2.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Documentation, https://main.d32to2oidohzrl.amplifyapp.com/
+Project-URL: Repository, https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
+Description-Content-Type: text/markdown
+
+# sefazetllib
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+---
+
+**Documentation**: [https://main.d32to2oidohzrl.amplifyapp.com/](https://main.d32to2oidohzrl.amplifyapp.com/)
+
+**Source code**: [AWS CodeCommit](https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1)
+
+---
+
+**sefazetllib** is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
+
+## Features
+
+- Easy to use and understand library for constructing ETL/ELT pipelines.
+- Compatibility with popular data processing frameworks, such as [pandas](https://pandas.pydata.org/) and [PySpark](https://spark.apache.org/).
+- Support for file formats such as CSV and Parquet.
+- Provides the ability to extract, transform and load data with customizable configurations.
+
+## Requirements
+
+**sefazetllib** requires the following to run:
+
+- [Python](https://www.python.org/) 3.7.1+
+- [pandas](https://pandas.pydata.org/) 1.3+
+- [PyArrow](https://arrow.apache.org/) 6.0+
+- [PySpark](https://spark.apache.org/) 3.0+
+- [PyDeequ](https://pydeequ.readthedocs.io/) 1.0+
+- [Boto3](https://github.com/boto/boto3) 1.24+
+
+## Installation
+
+Use [pip](https://pip.pypa.io/en/stable/) to install **sefazetllib**:
+
+```bash
+pip install sefazetllib
+```
+
+## Usage
+
+Here is an example of how to use the **sefazetllib**:
+
+```Python
+from typing import Tuple
+
+from pandas import DataFrame
+
+from sefazetllib import Builder
+from sefazetllib.etl import ETL
+from sefazetllib.extract import ExtractLocal
+from sefazetllib.factory.platform import PlatformFactory
+from sefazetllib.load import LoadLocal
+from sefazetllib.transform import Transform
+from sefazetllib.utils.key import SurrogateKey
+
+
+@Builder
+class TestingDataFrame(Transform):
+    def execute(self) -> Tuple[str, DataFrame]:
+        return (
+            "dataframe",
+            DataFrame(
+                [["tom", 10], ["nick", 15], ["juli", 14]], columns=["Name", "Age"]
+            ),
+        )
+
+
+(
+    ETL()
+    .setPlatform(PlatformFactory("Pandas").create(name="test_pandas"))
+    .transform(TestingDataFrame)
+    .load(
+        LoadLocal()
+        .setFileFormat("parquet")
+        .setEntity("load_test")
+        .setMode("overwrite")
+        .setReference("dataframe")
+        .setDuplicates(True)
+        .setKey(SurrogateKey().setColumns(["Name", "Age"]).setDistribute(False))
+    )
+    .extract(
+        ExtractLocal()
+        .setFileFormat("parquet")
+        .setUrl("load_test.parquet")
+        .setReference("extract_test")
+    )
+)
+```
+
+## Testing
+
+To run the unit tests, run the following command:
+
+```bash
+py -m unittest tests/main.py -v
+```
 
-packages = \
-['sefazetllib',
- 'sefazetllib.config',
- 'sefazetllib.etl',
- 'sefazetllib.extract',
- 'sefazetllib.factory',
- 'sefazetllib.factory.platform',
- 'sefazetllib.factory.platform.database',
- 'sefazetllib.factory.platform.dataframe',
- 'sefazetllib.load',
- 'sefazetllib.transform',
- 'sefazetllib.utils',
- 'sefazetllib.utils.key',
- 'sefazetllib.utils.partition',
- 'sefazetllib.validate',
- 'sefazetllibcli',
- 'sefazetllibcli.config',
- 'sefazetllibcli.errors',
- 'sefazetllibcli.generators',
- 'sefazetllibcli.usecases',
- 'sefazetllibcli.usecases.process_variable',
- 'sefazetllibcli.usecases.replace_template',
- 'sefazetllibcli.utils']
-
-package_data = \
-{'': ['*'], 'sefazetllibcli': ['templates/*']}
-
-install_requires = \
-['boto3>=1.24,<2.0',
- 'click>=8.1,<9.0',
- 'pandas>=1.3,<2.0',
- 'pyarrow>=6.0,<7.0',
- 'pydeequ>=1.0,<2.0',
- 'pyyaml>=6.0,<7.0']
-
-entry_points = \
-{'console_scripts': ['sefazetllib = sefazetllibcli:cli']}
-
-setup_kwargs = {
-    'name': 'sefazetllib',
-    'version': '0.1.33',
-    'description': 'sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.',
-    'long_description': '# sefazetllib\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n---\n\n**Documentation**: [https://main.d32to2oidohzrl.amplifyapp.com/](https://main.d32to2oidohzrl.amplifyapp.com/)\n\n**Source code**: [AWS CodeCommit](https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1)\n\n---\n\n**sefazetllib** is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.\n\n## Features\n\n- Easy to use and understand library for constructing ETL/ELT pipelines.\n- Compatibility with popular data processing frameworks, such as [pandas](https://pandas.pydata.org/) and [PySpark](https://spark.apache.org/).\n- Support for file formats such as CSV and Parquet.\n- Provides the ability to extract, transform and load data with customizable configurations.\n\n## Requirements\n\n**sefazetllib** requires the following to run:\n\n- [Python](https://www.python.org/) 3.7.1+\n- [pandas](https://pandas.pydata.org/) 1.3+\n- [PyArrow](https://arrow.apache.org/) 6.0+\n- [PySpark](https://spark.apache.org/) 3.0+\n- [PyDeequ](https://pydeequ.readthedocs.io/) 1.0+\n- [Boto3](https://github.com/boto/boto3) 1.24+\n\n## Installation\n\nUse [pip](https://pip.pypa.io/en/stable/) to install **sefazetllib**:\n\n```bash\npip install sefazetllib\n```\n\n## Usage\n\nHere is an example of how to use the **sefazetllib**:\n\n```Python\nfrom typing import Tuple\n\nfrom pandas import DataFrame\n\nfrom sefazetllib import Builder\nfrom sefazetllib.etl import ETL\nfrom sefazetllib.extract import ExtractLocal\nfrom sefazetllib.factory.platform import PlatformFactory\nfrom sefazetllib.load import LoadLocal\nfrom sefazetllib.transform import Transform\nfrom sefazetllib.utils.key import SurrogateKey\n\n\n@Builder\nclass TestingDataFrame(Transform):\n    def execute(self) -> Tuple[str, DataFrame]:\n        return (\n            "dataframe",\n            DataFrame(\n                [["tom", 10], ["nick", 15], ["juli", 14]], columns=["Name", "Age"]\n            ),\n        )\n\n\n(\n    ETL()\n    .setPlatform(PlatformFactory("Pandas").create(name="test_pandas"))\n    .transform(TestingDataFrame)\n    .load(\n        LoadLocal()\n        .setFileFormat("parquet")\n        .setEntity("load_test")\n        .setMode("overwrite")\n        .setReference("dataframe")\n        .setDuplicates(True)\n        .setKey(SurrogateKey().setColumns(["Name", "Age"]).setDistribute(False))\n    )\n    .extract(\n        ExtractLocal()\n        .setFileFormat("parquet")\n        .setUrl("load_test.parquet")\n        .setReference("extract_test")\n    )\n)\n```\n\n## Testing\n\nTo run the unit tests, run the following command:\n\n```bash\npy -m unittest tests/main.py -v\n```\n\n## License\n\n**sefazetllib** is released under the [Apache-2.0](/LICENSE).\n',
-    'author': 'Felipe Gochi',
-    'author_email': 'felipe.gochi@elogroup.com.br',
-    'maintainer': 'Bruno Santos',
-    'maintainer_email': 'bruno.santos@elogroup.com.br',
-    'url': 'https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
+## License
 
+**sefazetllib** is released under the [Apache-2.0](/LICENSE).
 
-setup(**setup_kwargs)
```

