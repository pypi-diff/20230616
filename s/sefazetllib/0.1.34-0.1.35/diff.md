# Comparing `tmp/sefazetllib-0.1.34.tar.gz` & `tmp/sefazetllib-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sefazetllib-0.1.34.tar", max compression
+gzip compressed data, was "sefazetllib-0.1.35.tar", max compression
```

## Comparing `sefazetllib-0.1.34.tar` & `sefazetllib-0.1.35.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rwxr-xr-x   0        0        0    10173 2023-06-13 18:35:19.937294 sefazetllib-0.1.34/LICENSE
--rwxr-xr-x   0        0        0     3159 2023-06-13 18:35:19.939794 sefazetllib-0.1.34/README.md
--rwxr-xr-x   0        0        0     2445 2023-06-16 17:37:58.825654 sefazetllib-0.1.34/pyproject.toml
--rwxr-xr-x   0        0        0     1663 2023-06-13 18:35:20.075553 sefazetllib-0.1.34/sefazetllib/Builder.py
--rwxr-xr-x   0        0        0      135 2023-06-13 18:35:20.079795 sefazetllib-0.1.34/sefazetllib/__init__.py
--rwxr-xr-x   0        0        0     2338 2023-06-13 18:35:20.087295 sefazetllib-0.1.34/sefazetllib/config/CustomLogging.py
--rwxr-xr-x   0        0        0       52 2023-06-13 18:35:20.092794 sefazetllib-0.1.34/sefazetllib/config/__init__.py
--rwxr-xr-x   0        0        0     8218 2023-06-13 18:35:20.099294 sefazetllib-0.1.34/sefazetllib/etl/ETL.py
--rwxr-xr-x   0        0        0       36 2023-06-13 18:35:20.104294 sefazetllib-0.1.34/sefazetllib/etl/__init__.py
--rwxr-xr-x   0        0        0      701 2023-06-13 18:35:20.109301 sefazetllib-0.1.34/sefazetllib/extract/Extract.py
--rwxr-xr-x   0        0        0     1986 2023-06-13 18:35:20.113298 sefazetllib-0.1.34/sefazetllib/extract/ExtractLocal.py
--rwxr-xr-x   0        0        0     2479 2023-06-13 18:35:20.119298 sefazetllib-0.1.34/sefazetllib/extract/ExtractS3.py
--rwxr-xr-x   0        0        0     2521 2023-06-13 18:35:20.123828 sefazetllib-0.1.34/sefazetllib/extract/ExtractSQL.py
--rwxr-xr-x   0        0        0     2282 2023-06-13 18:35:20.127293 sefazetllib-0.1.34/sefazetllib/extract/ExtractStorage.py
--rwxr-xr-x   0        0        0      274 2023-06-13 18:35:20.131294 sefazetllib-0.1.34/sefazetllib/extract/__init__.py
--rwxr-xr-x   0        0        0      949 2023-06-13 18:35:20.137294 sefazetllib-0.1.34/sefazetllib/factory/Factory.py
--rwxr-xr-x   0        0        0       89 2023-06-13 18:35:20.141795 sefazetllib-0.1.34/sefazetllib/factory/__init__.py
--rwxr-xr-x   0        0        0      362 2023-06-13 18:35:20.148794 sefazetllib-0.1.34/sefazetllib/factory/platform/DatabasePlatform.py
--rwxr-xr-x   0        0        0      281 2023-06-13 18:35:20.156294 sefazetllib-0.1.34/sefazetllib/factory/platform/Platform.py
--rwxr-xr-x   0        0        0     1049 2023-06-13 18:35:20.161796 sefazetllib-0.1.34/sefazetllib/factory/platform/PlatformFactory.py
--rwxr-xr-x   0        0        0      268 2023-06-13 18:35:20.166794 sefazetllib-0.1.34/sefazetllib/factory/platform/__init__.py
--rwxr-xr-x   0        0        0      723 2023-06-13 18:35:20.184341 sefazetllib-0.1.34/sefazetllib/factory/platform/database/Mysql.py
--rwxr-xr-x   0        0        0     4069 2023-06-13 18:35:20.190294 sefazetllib-0.1.34/sefazetllib/factory/platform/database/PostgreSQL.py
--rwxr-xr-x   0        0        0      134 2023-06-13 18:35:20.196307 sefazetllib-0.1.34/sefazetllib/factory/platform/database/__init__.py
--rwxr-xr-x   0        0        0      259 2023-06-13 18:35:20.207294 sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/Default.py
--rwxr-xr-x   0        0        0     1793 2023-06-13 18:35:20.214794 sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/Pandas.py
--rwxr-xr-x   0        0        0     4679 2023-06-13 18:35:20.219293 sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/Spark.py
--rwxr-xr-x   0        0        0      195 2023-06-13 18:35:20.224295 sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/__init__.py
--rwxr-xr-x   0        0        0      683 2023-06-13 18:35:20.230795 sefazetllib-0.1.34/sefazetllib/load/Load.py
--rwxr-xr-x   0        0        0     2134 2023-06-13 18:35:20.235296 sefazetllib-0.1.34/sefazetllib/load/LoadLocal.py
--rwxr-xr-x   0        0        0     2386 2023-06-13 18:35:20.238796 sefazetllib-0.1.34/sefazetllib/load/LoadS3.py
--rwxr-xr-x   0        0        0     7601 2023-06-13 18:35:20.242296 sefazetllib-0.1.34/sefazetllib/load/LoadSQL.py
--rwxr-xr-x   0        0        0     2194 2023-06-13 18:35:20.246796 sefazetllib-0.1.34/sefazetllib/load/LoadStorage.py
--rwxr-xr-x   0        0        0      229 2023-06-13 18:35:20.250295 sefazetllib-0.1.34/sefazetllib/load/__init__.py
--rwxr-xr-x   0        0        0     1471 2023-06-13 18:35:20.255795 sefazetllib-0.1.34/sefazetllib/transform/MinMaxLineTransform.py
--rwxr-xr-x   0        0        0     4331 2023-06-13 18:35:20.259795 sefazetllib-0.1.34/sefazetllib/transform/QuartileTransform.py
--rwxr-xr-x   0        0        0      552 2023-06-13 18:35:20.263795 sefazetllib-0.1.34/sefazetllib/transform/Transform.py
--rwxr-xr-x   0        0        0      198 2023-06-13 18:35:20.267294 sefazetllib-0.1.34/sefazetllib/transform/__init__.py
--rwxr-xr-x   0        0        0       45 2023-06-13 18:35:20.272796 sefazetllib-0.1.34/sefazetllib/utils/__init__.py
--rwxr-xr-x   0        0        0      325 2023-06-13 18:35:20.281294 sefazetllib-0.1.34/sefazetllib/utils/key/DefaultKey.py
--rwxr-xr-x   0        0        0      400 2023-06-13 18:35:20.287793 sefazetllib-0.1.34/sefazetllib/utils/key/Key.py
--rwxr-xr-x   0        0        0      747 2023-06-13 18:35:20.291793 sefazetllib-0.1.34/sefazetllib/utils/key/SurrogateKey.py
--rwxr-xr-x   0        0        0      158 2023-06-13 18:35:20.295794 sefazetllib-0.1.34/sefazetllib/utils/key/__init__.py
--rwxr-xr-x   0        0        0     2097 2023-06-13 18:35:20.304797 sefazetllib-0.1.34/sefazetllib/utils/partition/DatePartition.py
--rwxr-xr-x   0        0        0      627 2023-06-13 18:35:20.310298 sefazetllib-0.1.34/sefazetllib/utils/partition/IncrementalRangePartition.py
--rwxr-xr-x   0        0        0      425 2023-06-13 18:35:20.314794 sefazetllib-0.1.34/sefazetllib/utils/partition/Partition.py
--rwxr-xr-x   0        0        0      229 2023-06-13 18:35:20.318794 sefazetllib-0.1.34/sefazetllib/utils/partition/__init__.py
--rwxr-xr-x   0        0        0     7729 2023-06-16 17:37:58.844408 sefazetllib-0.1.34/sefazetllib/validate/DataValidate.py
--rwxr-xr-x   0        0        0      383 2023-06-13 18:35:20.330793 sefazetllib-0.1.34/sefazetllib/validate/Validate.py
--rwxr-xr-x   0        0        0      110 2023-06-13 18:35:20.333793 sefazetllib-0.1.34/sefazetllib/validate/__init__.py
--rwxr-xr-x   0        0        0     3551 2023-06-13 18:35:20.337293 sefazetllib-0.1.34/sefazetllibcli/__init__.py
--rwxr-xr-x   0        0        0        0 2023-06-13 18:35:20.341293 sefazetllib-0.1.34/sefazetllibcli/config/__init__.py
--rwxr-xr-x   0        0        0     1117 2023-06-13 18:35:20.345293 sefazetllib-0.1.34/sefazetllibcli/config/logging.py
--rwxr-xr-x   0        0        0      185 2023-06-13 18:35:20.350794 sefazetllib-0.1.34/sefazetllibcli/errors/__init__.py
--rwxr-xr-x   0        0        0       76 2023-06-13 18:35:20.354794 sefazetllib-0.1.34/sefazetllibcli/errors/method_not_implemented.py
--rwxr-xr-x   0        0        0       52 2023-06-13 18:35:20.358761 sefazetllib-0.1.34/sefazetllibcli/errors/unsupported_file_extension.py
--rwxr-xr-x   0        0        0       88 2023-06-13 18:35:20.362818 sefazetllib-0.1.34/sefazetllibcli/errors/variable_processing_error.py
--rwxr-xr-x   0        0        0        0 2023-06-13 18:35:20.367793 sefazetllib-0.1.34/sefazetllibcli/generators/__init__.py
--rwxr-xr-x   0        0        0     5897 2023-06-13 18:35:20.371294 sefazetllib-0.1.34/sefazetllibcli/generators/etl_generator.py
--rwxr-xr-x   0        0        0      884 2023-06-13 18:35:20.375497 sefazetllib-0.1.34/sefazetllibcli/generators/generator.py
--rwxr-xr-x   0        0        0      374 2023-06-13 18:35:20.383794 sefazetllib-0.1.34/sefazetllibcli/templates/etl_template
--rwxr-xr-x   0        0        0        0 2023-06-13 18:35:20.388794 sefazetllib-0.1.34/sefazetllibcli/usecases/__init__.py
--rwxr-xr-x   0        0        0      524 2023-06-13 18:35:20.398795 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/__init__.py
--rwxr-xr-x   0        0        0     3484 2023-06-13 18:35:20.405793 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_etl_variable.py
--rwxr-xr-x   0        0        0     1128 2023-06-13 18:35:20.410293 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_extract_variable.py
--rwxr-xr-x   0        0        0      986 2023-06-13 18:35:20.414295 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_imports_variable.py
--rwxr-xr-x   0        0        0     1142 2023-06-13 18:35:20.419294 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_key_variable.py
--rwxr-xr-x   0        0        0     1110 2023-06-13 18:35:20.423301 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_load_variable.py
--rwxr-xr-x   0        0        0     1595 2023-06-13 18:35:20.428294 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_partition_variable.py
--rwxr-xr-x   0        0        0     2086 2023-06-13 18:35:20.432793 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
--rwxr-xr-x   0        0        0     1074 2023-06-13 18:35:20.436794 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_validate_variable.py
--rwxr-xr-x   0        0        0      935 2023-06-13 18:35:20.440793 sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_variable.py
--rwxr-xr-x   0        0        0       99 2023-06-13 18:35:20.448793 sefazetllib-0.1.34/sefazetllibcli/usecases/replace_template/__init__.py
--rwxr-xr-x   0        0        0      963 2023-06-13 18:35:20.455293 sefazetllib-0.1.34/sefazetllibcli/usecases/replace_template/replace_etl_template.py
--rwxr-xr-x   0        0        0     1678 2023-06-13 18:35:20.460293 sefazetllib-0.1.34/sefazetllibcli/usecases/replace_template/replace_template.py
--rwxr-xr-x   0        0        0       32 2023-06-13 18:35:20.464793 sefazetllib-0.1.34/sefazetllibcli/utils/__init__.py
--rwxr-xr-x   0        0        0     3631 2023-06-13 18:35:20.468794 sefazetllib-0.1.34/sefazetllibcli/utils/parse_etl.py
--rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 sefazetllib-0.1.34/PKG-INFO
+-rwxr-xr-x   0        0        0    10173 2023-06-16 18:57:34.239206 sefazetllib-0.1.35/LICENSE
+-rwxr-xr-x   0        0        0     3159 2023-06-16 18:57:34.241708 sefazetllib-0.1.35/README.md
+-rwxr-xr-x   0        0        0     2445 2023-06-16 18:57:34.368626 sefazetllib-0.1.35/pyproject.toml
+-rwxr-xr-x   0        0        0     1663 2023-06-16 18:57:34.382151 sefazetllib-0.1.35/sefazetllib/Builder.py
+-rwxr-xr-x   0        0        0      135 2023-06-16 18:57:34.386125 sefazetllib-0.1.35/sefazetllib/__init__.py
+-rwxr-xr-x   0        0        0     2338 2023-06-16 18:57:34.393628 sefazetllib-0.1.35/sefazetllib/config/CustomLogging.py
+-rwxr-xr-x   0        0        0       52 2023-06-16 18:57:34.402125 sefazetllib-0.1.35/sefazetllib/config/__init__.py
+-rwxr-xr-x   0        0        0     8218 2023-06-16 18:57:34.409125 sefazetllib-0.1.35/sefazetllib/etl/ETL.py
+-rwxr-xr-x   0        0        0       36 2023-06-16 18:57:34.415125 sefazetllib-0.1.35/sefazetllib/etl/__init__.py
+-rwxr-xr-x   0        0        0      701 2023-06-16 18:57:34.421902 sefazetllib-0.1.35/sefazetllib/extract/Extract.py
+-rwxr-xr-x   0        0        0     1986 2023-06-16 18:57:34.427125 sefazetllib-0.1.35/sefazetllib/extract/ExtractLocal.py
+-rwxr-xr-x   0        0        0     2479 2023-06-16 18:57:34.432625 sefazetllib-0.1.35/sefazetllib/extract/ExtractS3.py
+-rwxr-xr-x   0        0        0     2521 2023-06-16 18:57:34.437126 sefazetllib-0.1.35/sefazetllib/extract/ExtractSQL.py
+-rwxr-xr-x   0        0        0     2282 2023-06-16 18:57:34.442127 sefazetllib-0.1.35/sefazetllib/extract/ExtractStorage.py
+-rwxr-xr-x   0        0        0      274 2023-06-16 18:57:34.446628 sefazetllib-0.1.35/sefazetllib/extract/__init__.py
+-rwxr-xr-x   0        0        0      949 2023-06-16 18:57:34.455648 sefazetllib-0.1.35/sefazetllib/factory/Factory.py
+-rwxr-xr-x   0        0        0       89 2023-06-16 18:57:34.460125 sefazetllib-0.1.35/sefazetllib/factory/__init__.py
+-rwxr-xr-x   0        0        0      362 2023-06-16 18:57:34.467624 sefazetllib-0.1.35/sefazetllib/factory/platform/DatabasePlatform.py
+-rwxr-xr-x   0        0        0      281 2023-06-16 18:57:34.473625 sefazetllib-0.1.35/sefazetllib/factory/platform/Platform.py
+-rwxr-xr-x   0        0        0     1049 2023-06-16 18:57:34.478627 sefazetllib-0.1.35/sefazetllib/factory/platform/PlatformFactory.py
+-rwxr-xr-x   0        0        0      268 2023-06-16 18:57:34.483126 sefazetllib-0.1.35/sefazetllib/factory/platform/__init__.py
+-rwxr-xr-x   0        0        0      723 2023-06-16 18:57:34.495627 sefazetllib-0.1.35/sefazetllib/factory/platform/database/MySQL.py
+-rwxr-xr-x   0        0        0     4069 2023-06-16 18:57:34.501626 sefazetllib-0.1.35/sefazetllib/factory/platform/database/PostgreSQL.py
+-rwxr-xr-x   0        0        0      134 2023-06-16 18:57:34.506624 sefazetllib-0.1.35/sefazetllib/factory/platform/database/__init__.py
+-rwxr-xr-x   0        0        0      259 2023-06-16 18:57:34.515125 sefazetllib-0.1.35/sefazetllib/factory/platform/dataframe/Default.py
+-rwxr-xr-x   0        0        0     1793 2023-06-16 18:57:34.521624 sefazetllib-0.1.35/sefazetllib/factory/platform/dataframe/Pandas.py
+-rwxr-xr-x   0        0        0     4679 2023-06-16 18:57:34.526624 sefazetllib-0.1.35/sefazetllib/factory/platform/dataframe/Spark.py
+-rwxr-xr-x   0        0        0      195 2023-06-16 18:57:34.531124 sefazetllib-0.1.35/sefazetllib/factory/platform/dataframe/__init__.py
+-rwxr-xr-x   0        0        0      683 2023-06-16 18:57:34.537126 sefazetllib-0.1.35/sefazetllib/load/Load.py
+-rwxr-xr-x   0        0        0     2134 2023-06-16 18:57:34.541625 sefazetllib-0.1.35/sefazetllib/load/LoadLocal.py
+-rwxr-xr-x   0        0        0     2386 2023-06-16 18:57:34.545625 sefazetllib-0.1.35/sefazetllib/load/LoadS3.py
+-rwxr-xr-x   0        0        0     7601 2023-06-16 18:57:34.549625 sefazetllib-0.1.35/sefazetllib/load/LoadSQL.py
+-rwxr-xr-x   0        0        0     2194 2023-06-16 18:57:34.553125 sefazetllib-0.1.35/sefazetllib/load/LoadStorage.py
+-rwxr-xr-x   0        0        0      229 2023-06-16 18:57:34.557125 sefazetllib-0.1.35/sefazetllib/load/__init__.py
+-rwxr-xr-x   0        0        0     1471 2023-06-16 18:57:34.563125 sefazetllib-0.1.35/sefazetllib/transform/MinMaxLineTransform.py
+-rwxr-xr-x   0        0        0     4331 2023-06-16 18:57:34.569126 sefazetllib-0.1.35/sefazetllib/transform/QuartileTransform.py
+-rwxr-xr-x   0        0        0      552 2023-06-16 18:57:34.573626 sefazetllib-0.1.35/sefazetllib/transform/Transform.py
+-rwxr-xr-x   0        0        0      198 2023-06-16 18:57:34.578125 sefazetllib-0.1.35/sefazetllib/transform/__init__.py
+-rwxr-xr-x   0        0        0       45 2023-06-16 18:57:34.584771 sefazetllib-0.1.35/sefazetllib/utils/__init__.py
+-rwxr-xr-x   0        0        0      325 2023-06-16 18:57:34.593670 sefazetllib-0.1.35/sefazetllib/utils/key/DefaultKey.py
+-rwxr-xr-x   0        0        0      400 2023-06-16 18:57:34.599624 sefazetllib-0.1.35/sefazetllib/utils/key/Key.py
+-rwxr-xr-x   0        0        0      747 2023-06-16 18:57:34.603124 sefazetllib-0.1.35/sefazetllib/utils/key/SurrogateKey.py
+-rwxr-xr-x   0        0        0      158 2023-06-16 18:57:34.607625 sefazetllib-0.1.35/sefazetllib/utils/key/__init__.py
+-rwxr-xr-x   0        0        0     2097 2023-06-16 18:57:34.615125 sefazetllib-0.1.35/sefazetllib/utils/partition/DatePartition.py
+-rwxr-xr-x   0        0        0      627 2023-06-16 18:57:34.620626 sefazetllib-0.1.35/sefazetllib/utils/partition/IncrementalRangePartition.py
+-rwxr-xr-x   0        0        0      425 2023-06-16 18:57:34.624700 sefazetllib-0.1.35/sefazetllib/utils/partition/Partition.py
+-rwxr-xr-x   0        0        0      229 2023-06-16 18:57:34.629124 sefazetllib-0.1.35/sefazetllib/utils/partition/__init__.py
+-rwxr-xr-x   0        0        0     7729 2023-06-16 18:57:34.634626 sefazetllib-0.1.35/sefazetllib/validate/DataValidate.py
+-rwxr-xr-x   0        0        0      383 2023-06-16 18:57:34.639627 sefazetllib-0.1.35/sefazetllib/validate/Validate.py
+-rwxr-xr-x   0        0        0      110 2023-06-16 18:57:34.643811 sefazetllib-0.1.35/sefazetllib/validate/__init__.py
+-rwxr-xr-x   0        0        0     3551 2023-06-16 18:57:34.650625 sefazetllib-0.1.35/sefazetllibcli/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-06-16 18:57:34.661662 sefazetllib-0.1.35/sefazetllibcli/config/__init__.py
+-rwxr-xr-x   0        0        0     1117 2023-06-16 18:57:34.672625 sefazetllib-0.1.35/sefazetllibcli/config/logging.py
+-rwxr-xr-x   0        0        0      185 2023-06-16 18:57:34.679205 sefazetllib-0.1.35/sefazetllibcli/errors/__init__.py
+-rwxr-xr-x   0        0        0       76 2023-06-16 18:57:34.684125 sefazetllib-0.1.35/sefazetllibcli/errors/method_not_implemented.py
+-rwxr-xr-x   0        0        0       52 2023-06-16 18:57:34.688141 sefazetllib-0.1.35/sefazetllibcli/errors/unsupported_file_extension.py
+-rwxr-xr-x   0        0        0       88 2023-06-16 18:57:34.692627 sefazetllib-0.1.35/sefazetllibcli/errors/variable_processing_error.py
+-rwxr-xr-x   0        0        0        0 2023-06-16 18:57:34.698124 sefazetllib-0.1.35/sefazetllibcli/generators/__init__.py
+-rwxr-xr-x   0        0        0     5897 2023-06-16 18:57:34.704125 sefazetllib-0.1.35/sefazetllibcli/generators/etl_generator.py
+-rwxr-xr-x   0        0        0      884 2023-06-16 18:57:34.708625 sefazetllib-0.1.35/sefazetllibcli/generators/generator.py
+-rwxr-xr-x   0        0        0      374 2023-06-16 18:57:34.715625 sefazetllib-0.1.35/sefazetllibcli/templates/etl_template
+-rwxr-xr-x   0        0        0        0 2023-06-16 18:57:34.721227 sefazetllib-0.1.35/sefazetllibcli/usecases/__init__.py
+-rwxr-xr-x   0        0        0      524 2023-06-16 18:57:34.731625 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/__init__.py
+-rwxr-xr-x   0        0        0     3484 2023-06-16 18:57:34.738145 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_etl_variable.py
+-rwxr-xr-x   0        0        0     1128 2023-06-16 18:57:34.743625 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_extract_variable.py
+-rwxr-xr-x   0        0        0      986 2023-06-16 18:57:34.749625 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_imports_variable.py
+-rwxr-xr-x   0        0        0     1142 2023-06-16 18:57:34.758625 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_key_variable.py
+-rwxr-xr-x   0        0        0     1110 2023-06-16 18:57:34.763827 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_load_variable.py
+-rwxr-xr-x   0        0        0     1595 2023-06-16 18:57:34.769125 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_partition_variable.py
+-rwxr-xr-x   0        0        0     2086 2023-06-16 18:57:34.774125 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_transforms_variable.py
+-rwxr-xr-x   0        0        0     1074 2023-06-16 18:57:34.779624 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_validate_variable.py
+-rwxr-xr-x   0        0        0      935 2023-06-16 18:57:34.784631 sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_variable.py
+-rwxr-xr-x   0        0        0       99 2023-06-16 18:57:34.793926 sefazetllib-0.1.35/sefazetllibcli/usecases/replace_template/__init__.py
+-rwxr-xr-x   0        0        0      963 2023-06-16 18:57:34.800126 sefazetllib-0.1.35/sefazetllibcli/usecases/replace_template/replace_etl_template.py
+-rwxr-xr-x   0        0        0     1678 2023-06-16 18:57:34.805124 sefazetllib-0.1.35/sefazetllibcli/usecases/replace_template/replace_template.py
+-rwxr-xr-x   0        0        0       32 2023-06-16 18:57:34.811627 sefazetllib-0.1.35/sefazetllibcli/utils/__init__.py
+-rwxr-xr-x   0        0        0     3631 2023-06-16 18:57:34.816125 sefazetllib-0.1.35/sefazetllibcli/utils/parse_etl.py
+-rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 sefazetllib-0.1.35/PKG-INFO
```

### Comparing `sefazetllib-0.1.34/LICENSE` & `sefazetllib-0.1.35/LICENSE`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/README.md` & `sefazetllib-0.1.35/README.md`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/pyproject.toml` & `sefazetllib-0.1.35/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sefazetllib"
-version = "0.1.34"
+version = "0.1.35"
 description = "sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines."
 license = "Apache-2.0"
 authors = ["Felipe Gochi <felipe.gochi@elogroup.com.br>"]
 maintainers = [
     "Bruno Santos <bruno.santos@elogroup.com.br>",
     "Felipe Alcantara <felipe.alcantara@elogroup.com.br>",
     "Felipe Gochi <felipe.gochi@elogroup.com.br>",
```

### Comparing `sefazetllib-0.1.34/sefazetllib/Builder.py` & `sefazetllib-0.1.35/sefazetllib/Builder.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/config/CustomLogging.py` & `sefazetllib-0.1.35/sefazetllib/config/CustomLogging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/etl/ETL.py` & `sefazetllib-0.1.35/sefazetllib/etl/ETL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/extract/Extract.py` & `sefazetllib-0.1.35/sefazetllib/extract/Extract.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/extract/ExtractLocal.py` & `sefazetllib-0.1.35/sefazetllib/extract/ExtractLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/extract/ExtractS3.py` & `sefazetllib-0.1.35/sefazetllib/extract/ExtractS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/extract/ExtractSQL.py` & `sefazetllib-0.1.35/sefazetllib/extract/ExtractSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/extract/ExtractStorage.py` & `sefazetllib-0.1.35/sefazetllib/extract/ExtractStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/factory/Factory.py` & `sefazetllib-0.1.35/sefazetllib/factory/Factory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/factory/platform/PlatformFactory.py` & `sefazetllib-0.1.35/sefazetllib/factory/platform/PlatformFactory.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/factory/platform/database/Mysql.py` & `sefazetllib-0.1.35/sefazetllib/factory/platform/database/MySQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/factory/platform/database/PostgreSQL.py` & `sefazetllib-0.1.35/sefazetllib/factory/platform/database/PostgreSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/Pandas.py` & `sefazetllib-0.1.35/sefazetllib/factory/platform/dataframe/Pandas.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/factory/platform/dataframe/Spark.py` & `sefazetllib-0.1.35/sefazetllib/factory/platform/dataframe/Spark.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/load/Load.py` & `sefazetllib-0.1.35/sefazetllib/load/Load.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/load/LoadLocal.py` & `sefazetllib-0.1.35/sefazetllib/load/LoadLocal.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/load/LoadS3.py` & `sefazetllib-0.1.35/sefazetllib/load/LoadS3.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/load/LoadSQL.py` & `sefazetllib-0.1.35/sefazetllib/load/LoadSQL.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/load/LoadStorage.py` & `sefazetllib-0.1.35/sefazetllib/load/LoadStorage.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/transform/MinMaxLineTransform.py` & `sefazetllib-0.1.35/sefazetllib/transform/MinMaxLineTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/transform/QuartileTransform.py` & `sefazetllib-0.1.35/sefazetllib/transform/QuartileTransform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/transform/Transform.py` & `sefazetllib-0.1.35/sefazetllib/transform/Transform.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/utils/key/SurrogateKey.py` & `sefazetllib-0.1.35/sefazetllib/utils/key/SurrogateKey.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/utils/partition/DatePartition.py` & `sefazetllib-0.1.35/sefazetllib/utils/partition/DatePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/utils/partition/IncrementalRangePartition.py` & `sefazetllib-0.1.35/sefazetllib/utils/partition/IncrementalRangePartition.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllib/validate/DataValidate.py` & `sefazetllib-0.1.35/sefazetllib/validate/DataValidate.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/__init__.py` & `sefazetllib-0.1.35/sefazetllibcli/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/config/logging.py` & `sefazetllib-0.1.35/sefazetllibcli/config/logging.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/generators/etl_generator.py` & `sefazetllib-0.1.35/sefazetllibcli/generators/etl_generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/generators/generator.py` & `sefazetllib-0.1.35/sefazetllibcli/generators/generator.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/__init__.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_etl_variable.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_etl_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_extract_variable.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_extract_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_imports_variable.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_imports_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_key_variable.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_key_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_load_variable.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_load_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_partition_variable.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_partition_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_transforms_variable.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_transforms_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_validate_variable.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_validate_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/process_variable/process_variable.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/process_variable/process_variable.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/replace_template/replace_etl_template.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/replace_template/replace_etl_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/usecases/replace_template/replace_template.py` & `sefazetllib-0.1.35/sefazetllibcli/usecases/replace_template/replace_template.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/sefazetllibcli/utils/parse_etl.py` & `sefazetllib-0.1.35/sefazetllibcli/utils/parse_etl.py`

 * *Files identical despite different names*

### Comparing `sefazetllib-0.1.34/PKG-INFO` & `sefazetllib-0.1.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sefazetllib
-Version: 0.1.34
+Version: 0.1.35
 Summary: sefazetllib is a library that provides a simplified and abstracted way to construct ETL/ELT pipelines.
 Home-page: https://sa-east-1.console.aws.amazon.com/codesuite/codecommit/repositories/jobs-lib-sefaz-ce/browse?region=sa-east-1
 License: Apache-2.0
 Author: Felipe Gochi
 Author-email: felipe.gochi@elogroup.com.br
 Maintainer: Bruno Santos
 Maintainer-email: bruno.santos@elogroup.com.br
```

