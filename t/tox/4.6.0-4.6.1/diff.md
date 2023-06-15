# Comparing `tmp/tox-4.6.0.tar.gz` & `tmp/tox-4.6.1.tar.gz`

## Comparing `tox-4.6.0.tar` & `tox-4.6.1.tar`

### file list

```diff
@@ -1,222 +1,221 @@
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 tox-4.6.0/tox.ini
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/__main__.py
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/provision.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/py.typed
--rw-r--r--   0        0        0    19145 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/pytest.py
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/report.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/run.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/__init__.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/main.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/of_type.py
--rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/set_env.py
--rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/sets.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/__init__.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/env_var.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/ini.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/parse.py
--rw-r--r--   0        0        0    13671 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/cli/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/__init__.py
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/api.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/convert.py
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/memory.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/section.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/str_convert.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/stringify.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/ini/__init__.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/ini/factor.py
--rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/loader/ini/replace.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/__init__.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/api.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/discover.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/ini.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/ini_section.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/legacy_toml.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/setup_cfg.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/config/source/tox_ini.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/__init__.py
--rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/api.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/pep517_backend.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/request.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/stream.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/util.py
--rw-r--r--   0        0        0    13863 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/local_sub_process/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread_unix.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread_windows.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/journal/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/journal/env.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/journal/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/plugin/__init__.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/plugin/inline.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/plugin/manager.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/plugin/spec.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/__init__.py
--rw-r--r--   0        0        0    18083 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/env_select.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/__init__.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/depends.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/devenv.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/exec_.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/legacy.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/list_env.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/quickstart.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/show_config.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/version_flag.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/__init__.py
--rw-r--r--   0        0        0    17112 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/common.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/parallel.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/sequential.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/session/cmd/run/single.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/__init__.py
--rw-r--r--   0        0        0    20134 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/api.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/errors.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/info.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/installer.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/package.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/register.py
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/runner.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/api.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/package.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/__init__.py
--rw-r--r--   0        0        0    10355 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/pip_install.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req_file.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req/__init__.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req/args.py
--rw-r--r--   0        0        0    19406 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req/file.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/pip/req/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/api.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
--rw-r--r--   0        0        0    17577 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/package/pyproject.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/tox_env/python/virtual_env/package/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/ci.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/cpu.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/file_view.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/graph.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/path.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 tox-4.6.0/src/tox/util/spinner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/__init__.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 tox-4.6.0/tests/conftest.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_call_modes.py
--rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_provision.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_report.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_run.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.0/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/__init__.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/conftest.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_main.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_of_types.py
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_set_env.py
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_sets.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/conftest.py
--rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/test_cli_env_var.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/test_cli_ini.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/test_parse.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/cli/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/__init__.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/test_loader.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/test_memory_loader.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/test_section.py
--rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/test_str_convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/__init__.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/conftest.py
--rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/test_factor.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/test_ini_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/conftest.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_env_var.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_os_pathsep.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_os_sep.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_posargs.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_tox_env.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/loader/ini/replace/test_replace_tty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/__init__.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/test_discover.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/test_legacy_toml.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/test_setup_cfg.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tox-4.6.0/tests/config/source/test_source_ini.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_inline/build.pyi
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 tox-4.6.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/conftest.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/test_request.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/test_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/__init__.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/bad_process.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/local_subprocess_sigint.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/test_execute_util.py
--rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/test_local_subprocess.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tox-4.6.0/tests/execute/local_subprocess/tty_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/journal/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.0/tests/journal/test_main_journal.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.0/tests/plugin/conftest.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 tox-4.6.0/tests/plugin/test_inline.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 tox-4.6.0/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 tox-4.6.0/tests/plugin/test_plugin_custom_config_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/pytest_/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 tox-4.6.0/tests/pytest_/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/__init__.py
--rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/test_env_select.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/test_session_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_depends.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_devenv.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_exec_.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_legacy.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_list_envs.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_parallel.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_quickstart.py
--rw-r--r--   0        0        0    18713 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_sequential.py
--rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_show_config.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/run/__init__.py
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tox-4.6.0/tests/session/cmd/run/test_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_api.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_info.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_register.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_tox_env_api.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/test_tox_env_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/__init__.py
--rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/test_python_api.py
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/test_python_runner.py
--rw-r--r--   0        0        0    17036 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/pip/test_pip_install.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/pip/test_req_file.py
--rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/pip/req/test_file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/test-pkg/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/test_setuptools.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/conftest.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 tox-4.6.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 tox-4.6.0/tests/type_check/add_config_container_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/__init__.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_ci.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_cpu.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_graph.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_path.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 tox-4.6.0/tests/util/test_spinner.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.0/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.0/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.0/README.md
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 tox-4.6.0/pyproject.toml
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 tox-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 tox-4.6.1/tox.ini
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/__main__.py
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/provision.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/py.typed
+-rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/pytest.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/report.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/run.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/__init__.py
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/main.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/of_type.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/set_env.py
+-rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/sets.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/__init__.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/env_var.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/ini.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/parse.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/cli/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/__init__.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/api.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/convert.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/memory.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/section.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/str_convert.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/stringify.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/ini/factor.py
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/loader/ini/replace.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/__init__.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/api.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/discover.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/ini.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/ini_section.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/legacy_toml.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/setup_cfg.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/config/source/tox_ini.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/__init__.py
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/api.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/pep517_backend.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/request.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/stream.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/util.py
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/local_sub_process/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread_unix.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread_windows.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/journal/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/journal/env.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/journal/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/plugin/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/plugin/inline.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/plugin/manager.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/plugin/spec.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/__init__.py
+-rw-r--r--   0        0        0    18474 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/env_select.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/depends.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/devenv.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/exec_.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/legacy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/list_env.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/quickstart.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/show_config.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/version_flag.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/common.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/parallel.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/sequential.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/session/cmd/run/single.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/__init__.py
+-rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/api.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/errors.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/info.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/installer.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/package.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/register.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/runner.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/api.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/package.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/__init__.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/pip_install.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req_file.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req/args.py
+-rw-r--r--   0        0        0    19762 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req/file.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/pip/req/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/api.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
+-rw-r--r--   0        0        0    17983 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/package/pyproject.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/tox_env/python/virtual_env/package/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/ci.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/cpu.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/file_view.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/graph.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/path.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 tox-4.6.1/src/tox/util/spinner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.6.1/tests/conftest.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_call_modes.py
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_provision.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_report.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_run.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.1/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/conftest.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_main.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_of_types.py
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_set_env.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_sets.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/conftest.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/test_cli_env_var.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/test_cli_ini.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/test_parse.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/cli/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/test_loader.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/test_memory_loader.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/test_section.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/test_str_convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/conftest.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/test_factor.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/test_ini_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/__init__.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/conftest.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_env_var.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_os_pathsep.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_os_sep.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_posargs.py
+-rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_tox_env.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/loader/ini/replace/test_replace_tty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/test_discover.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/test_legacy_toml.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/test_setup_cfg.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.6.1/tests/config/source/test_source_ini.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.6.1/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/conftest.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/test_request.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/test_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/__init__.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/bad_process.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/local_subprocess_sigint.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/test_execute_util.py
+-rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/test_local_subprocess.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.6.1/tests/execute/local_subprocess/tty_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/journal/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.1/tests/journal/test_main_journal.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.1/tests/plugin/conftest.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.6.1/tests/plugin/test_inline.py
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 tox-4.6.1/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.6.1/tests/plugin/test_plugin_custom_config_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/pytest_/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.6.1/tests/pytest_/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/__init__.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/test_env_select.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/test_session_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_depends.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_devenv.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_exec_.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_legacy.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_list_envs.py
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_parallel.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_quickstart.py
+-rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_sequential.py
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_show_config.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.6.1/tests/session/cmd/run/test_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_api.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_info.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_register.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_tox_env_api.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/test_tox_env_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/__init__.py
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/test_python_api.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/test_python_runner.py
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/pip/test_pip_install.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/pip/test_req_file.py
+-rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/pip/req/test_file.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/test-pkg/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/test_setuptools.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/test_virtualenv_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/conftest.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
+-rw-r--r--   0        0        0    10178 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.6.1/tests/tox_env/python/virtual_env/package/test_python_package_util.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.6.1/tests/type_check/add_config_container_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/__init__.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_ci.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_cpu.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_graph.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_path.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.6.1/tests/util/test_spinner.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.1/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.1/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.1/README.md
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 tox-4.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 tox-4.6.1/PKG-INFO
```

### Comparing `tox-4.6.0/tox.ini` & `tox-4.6.1/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
       tests --durations 5 --run-integration}
     diff-cover --compare-branch {env:DIFF_AGAINST:origin/main} {toxworkdir}{/}coverage.{envname}.xml
 
 [testenv:fix]
 description = format the code base to adhere to our styles, and complain about what we cannot do automatically
 skip_install = true
 deps =
-    pre-commit>=3.3.2
+    pre-commit>=3.3.3
 pass_env =
     {[testenv]passenv}
     PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure {posargs}
     python -c 'print(r"hint: run {envbindir}{/}pre-commit install to add checks as pre-commit hook")'
 
@@ -81,15 +81,15 @@
 
 [testenv:release]
 description = do a release, required posarg of the version number
 skip_install = true
 deps =
     gitpython>=3.1.31
     packaging>=23.1
-    towncrier>=22.12
+    towncrier>=23.6
 commands =
     python {toxinidir}/tasks/release.py --version {posargs}
 
 [testenv:dev]
 description = dev environment with all deps at {envdir}
 package = editable
 deps =
```

### Comparing `tox-4.6.0/src/tox/provision.py` & `tox-4.6.1/src/tox/provision.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-"""
-This package handles provisioning an appropriate tox version per requirements.
-"""
+"""This package handles provisioning an appropriate tox version per requirements."""
 from __future__ import annotations
 
 import json
 import logging
 import sys
-from argparse import ArgumentParser
 from pathlib import Path
 from typing import TYPE_CHECKING, List, cast
 
 from packaging.requirements import Requirement
 from packaging.utils import canonicalize_name
 from packaging.version import Version
 
@@ -24,14 +21,16 @@
 
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from importlib.metadata import PackageNotFoundError, distribution
 else:  # pragma: no cover (py38+)
     from importlib_metadata import PackageNotFoundError, distribution
 
 if TYPE_CHECKING:
+    from argparse import ArgumentParser
+
     from tox.session.state import State
 
 
 @impl
 def tox_add_option(parser: ArgumentParser) -> None:
     parser.add_argument(
         "--no-provision",
@@ -58,15 +57,15 @@
 
 def provision(state: State) -> int | bool:
     # remove the dev and marker to allow local development of the package
     state.conf.core.add_config(
         keys=["min_version", "minversion"],
         of_type=Version,
         # do not include local version specifier (because it's not allowed in version spec per PEP-440)
-        default=None,  # type: ignore # Optional[Version] translates to object
+        default=None,  # type: ignore[arg-type] # Optional[Version] translates to object
         desc="Define the minimal tox version required to run",
     )
     state.conf.core.add_config(
         keys="provision_tox_env",
         of_type=str,
         default=".tox",
         desc="Name of the virtual environment used to provision a tox.",
@@ -99,29 +98,29 @@
         # use our own dependency specification
         deps=PythonDeps("\n".join(str(r) for r in requires), root=state.conf.core["tox_root"]),
         pass_env=["*"],  # do not filter environment variables, will be handled by provisioned tox
         recreate=state.conf.options.recreate and not state.conf.options.no_recreate_provision,
     )
     provision_tox_env: str = state.conf.core["provision_tox_env"]
     state.conf.memory_seed_loaders[provision_tox_env].append(loader)
-    state.envs._mark_provision(bool(missing), provision_tox_env)
+    state.envs._mark_provision(bool(missing), provision_tox_env)  # noqa: SLF001
 
     if not missing:
         return False
 
     miss_msg = f"is missing [requires (has)]: {deps}"
 
     no_provision: bool | str = state.conf.options.no_provision
     if no_provision:
         msg = f"provisioning explicitly disabled within {sys.executable}, but {miss_msg}"
         if isinstance(no_provision, str):
             msg += f" and wrote to {no_provision}"
             min_version = str(next(i.specifier for i in requires if i.name == "tox")).split("=")
             requires_dict = {
-                "minversion": min_version[1] if len(min_version) >= 2 else None,
+                "minversion": min_version[1] if len(min_version) >= 2 else None,  # noqa: PLR2004
                 "requires": [str(i) for i in requires],
             }
             Path(no_provision).write_text(json.dumps(requires_dict, indent=4))
         raise HandledError(msg)
 
     logging.warning("will run in automatically provisioned tox, host %s %s", sys.executable, miss_msg)
     return run_provision(provision_tox_env, state)
@@ -144,12 +143,13 @@
 def run_provision(name: str, state: State) -> int:
     tox_env: PythonRun = cast(PythonRun, state.envs[name])
     env_python = tox_env.env_python()
     logging.info("will run in a automatically provisioned python environment under %s", env_python)
     try:
         tox_env.setup()
     except Skip as exception:
-        raise HandledError(f"cannot provision tox environment {tox_env.conf['env_name']} because {exception}")
+        msg = f"cannot provision tox environment {tox_env.conf['env_name']} because {exception}"
+        raise HandledError(msg) from exception
     args: list[str] = [str(env_python), "-m", "tox"]
     args.extend(state.args)
     outcome = tox_env.execute(cmd=args, stdin=StdinSource.user_only(), show=True, run_id="provision", cwd=Path.cwd())
     return cast(int, outcome.exit_code)
```

### Comparing `tox-4.6.0/src/tox/pytest.py` & `tox-4.6.1/src/tox/pytest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-"""
-A pytest plugin useful to test tox itself (and its plugins).
-"""
+"""A pytest plugin useful to test tox itself (and its plugins)."""
 from __future__ import annotations
 
 import inspect
 import os
 import re
 import shutil
 import socket
 import sys
 import textwrap
 import warnings
 from contextlib import closing, contextmanager
 from pathlib import Path
 from types import ModuleType, TracebackType
 from typing import TYPE_CHECKING, Any, Callable, Iterator, Sequence, cast
-from unittest.mock import MagicMock
 
 import pytest
 from _pytest.capture import CaptureFixture as _CaptureFixture
-from _pytest.config import Config as PyTestConfig
-from _pytest.config.argparsing import Parser
 from _pytest.fixtures import SubRequest
 from _pytest.logging import LogCaptureFixture
 from _pytest.monkeypatch import MonkeyPatch
-from _pytest.python import Function
 from _pytest.tmpdir import TempPathFactory
 from devpi_process import IndexServer
-from pytest_mock import MockerFixture
 from virtualenv.info import fs_supports_symlink
 
 import tox.run
-from tox.config.sets import EnvConfigSet
 from tox.execute.api import Execute, ExecuteInstance, ExecuteOptions, ExecuteStatus, Outcome
 from tox.execute.request import ExecuteRequest, shell_cmd
-from tox.execute.stream import SyncWrite
 from tox.plugin import manager
 from tox.report import LOGGER, OutErr
 from tox.run import run as tox_run
 from tox.run import setup_state as previous_setup_state
 from tox.session.cmd.run.parallel import ENV_VAR_KEY
-from tox.session.state import State
 from tox.tox_env import api as tox_env_api
 from tox.tox_env.api import ToxEnv
 
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from typing import Protocol
 else:  # pragma: no cover (<py38)
     from typing_extensions import Protocol
 
 if TYPE_CHECKING:
+    from unittest.mock import MagicMock
+
+    from _pytest.config import Config as PyTestConfig
+    from _pytest.config.argparsing import Parser
+    from _pytest.python import Function
+    from pytest_mock import MockerFixture
+
+    from tox.config.sets import EnvConfigSet
+    from tox.execute.stream import SyncWrite
+    from tox.session.state import State
+
     CaptureFixture = _CaptureFixture[str]
 else:
     CaptureFixture = _CaptureFixture
 
 os.environ["PIP_DISABLE_PIP_VERSION_CHECK"] = "1"
 os.environ["PIP_NO_PYTHON_VERSION_WARNING"] = "1"
 
@@ -67,17 +68,17 @@
     before_handlers = list(LOGGER.handlers)
     yield
     LOGGER.handlers = before_handlers
 
 
 @pytest.fixture(autouse=True)
 def _disable_root_tox_py(request: SubRequest, mocker: MockerFixture) -> Iterator[None]:
-    """unless this is a plugin test do not allow loading toxfile.py"""
+    """Unless this is a plugin test do not allow loading toxfile.py."""
     if request.node.get_closest_marker("plugin_test"):  # unregister inline plugin
-        module, load_inline = None, manager._load_inline
+        module, load_inline = None, manager._load_inline  # noqa: SLF001
 
         def _load_inline(path: Path) -> ModuleType | None:  # register only on first run, and unregister at end
             nonlocal module
             module = load_inline(path)
             return module
 
         mocker.patch.object(manager, "_load_inline", _load_inline)
@@ -88,15 +89,15 @@
         mocker.patch("tox.plugin.inline._load_plugin", return_value=None)
         yield
 
 
 @contextmanager
 def check_os_environ() -> Iterator[None]:
     old = os.environ.copy()
-    to_clean = {k: os.environ.pop(k, None) for k in {ENV_VAR_KEY, "TOX_WORK_DIR", "PYTHONPATH", "COV_CORE_CONTEXT"}}
+    to_clean = {k: os.environ.pop(k, None) for k in (ENV_VAR_KEY, "TOX_WORK_DIR", "PYTHONPATH", "COV_CORE_CONTEXT")}
 
     yield
 
     for key, value in to_clean.items():
         if value is not None:
             os.environ[key] = value
 
@@ -122,20 +123,20 @@
 def check_os_environ_stable(monkeypatch: MonkeyPatch) -> Iterator[None]:  # noqa: PT004
     with check_os_environ():
         yield
         monkeypatch.undo()
 
 
 @pytest.fixture(autouse=True)
-def no_color(monkeypatch: MonkeyPatch, check_os_environ_stable: None) -> None:  # noqa: PT004, U100
+def no_color(monkeypatch: MonkeyPatch, check_os_environ_stable: None) -> None:  # noqa: ARG001, PT004
     monkeypatch.setenv("NO_COLOR", "yes")
 
 
 class ToxProject:
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         files: dict[str, Any],
         base: Path | None,
         path: Path,
         capfd: CaptureFixture,
         monkeypatch: MonkeyPatch,
         mocker: MockerFixture,
@@ -149,32 +150,34 @@
     @staticmethod
     def _setup_files(dest: Path, base: Path | None, content: dict[str, Any]) -> None:
         if base is not None:
             shutil.copytree(str(base), str(dest))
         dest.mkdir(exist_ok=True)
         for key, value in content.items():
             if not isinstance(key, str):
-                raise TypeError(f"{key!r} at {dest}")  # pragma: no cover
+                msg = f"{key!r} at {dest}"
+                raise TypeError(msg)  # pragma: no cover
             at_path = dest / key
             if callable(value):
-                value = textwrap.dedent("\n".join(inspect.getsourcelines(value)[0][1:]))
+                value = textwrap.dedent("\n".join(inspect.getsourcelines(value)[0][1:]))  # noqa: PLW2901
+                value = f"from __future__ import annotations\n{value}"  # noqa: PLW2901
             if isinstance(value, dict):
                 at_path.mkdir(exist_ok=True)
-                ToxProject._setup_files(at_path, None, value)
+                ToxProject._setup_files(at_path, None, value)  # noqa: SLF001
             elif isinstance(value, str):
                 at_path.write_text(textwrap.dedent(value), encoding="utf-8")
             elif value is None:
                 at_path.mkdir()
             else:
                 msg = f"could not handle {at_path / key} with content {value!r}"  # pragma: no cover
                 raise TypeError(msg)  # pragma: no cover
 
-    def patch_execute(self, handle: Callable[[ExecuteRequest], int | None]) -> MagicMock:
+    def patch_execute(self, handle: Callable[[ExecuteRequest], int | None]) -> MagicMock:  # noqa: C901
         class MockExecute(Execute):
-            def __init__(self, colored: bool, exit_code: int) -> None:
+            def __init__(self, colored: bool, exit_code: int) -> None:  # noqa: FBT001
                 self.exit_code = exit_code
                 super().__init__(colored)
 
             def build_instance(
                 self,
                 request: ExecuteRequest,
                 options: ExecuteOptions,
@@ -188,25 +191,25 @@
                 super().__init__(options, out, err)
                 self._exit_code = exit_code
 
             @property
             def exit_code(self) -> int | None:
                 return self._exit_code
 
-            def wait(self, timeout: float | None = None) -> int | None:  # noqa: U100
+            def wait(self, timeout: float | None = None) -> int | None:  # noqa: ARG002
                 return self._exit_code
 
-            def write_stdin(self, content: str) -> None:  # noqa: U100
+            def write_stdin(self, content: str) -> None:  # noqa: ARG002
                 return None  # pragma: no cover
 
             def interrupt(self) -> None:
                 return None  # pragma: no cover
 
         class MockExecuteInstance(ExecuteInstance):
-            def __init__(
+            def __init__(  # noqa: PLR0913
                 self,
                 request: ExecuteRequest,
                 options: ExecuteOptions,
                 out: SyncWrite,
                 err: SyncWrite,
                 exit_code: int,
             ) -> None:
@@ -214,41 +217,40 @@
                 self.exit_code = exit_code
 
             def __enter__(self) -> ExecuteStatus:
                 return MockExecuteStatus(self.options, self._out, self._err, self.exit_code)
 
             def __exit__(
                 self,
-                exc_type: type[BaseException] | None,  # noqa: U100
-                exc_val: BaseException | None,  # noqa: U100
-                exc_tb: TracebackType | None,  # noqa: U100
+                exc_type: type[BaseException] | None,
+                exc_val: BaseException | None,
+                exc_tb: TracebackType | None,
             ) -> None:
                 pass
 
             @property
             def cmd(self) -> Sequence[str]:
                 return self.request.cmd
 
         @contextmanager
         def _execute_call(
             self: ToxEnv,
             executor: Execute,
             out_err: OutErr,
             request: ExecuteRequest,
-            show: bool,
+            show: bool,  # noqa: FBT001
         ) -> Iterator[ExecuteStatus]:
             exit_code = handle(request)
             if exit_code is not None:
-                executor = MockExecute(colored=executor._colored, exit_code=exit_code)
+                executor = MockExecute(colored=executor._colored, exit_code=exit_code)  # noqa: SLF001
             with original_execute_call(self, executor, out_err, request, show) as status:
                 yield status
 
-        original_execute_call = ToxEnv._execute_call
-        result = self.mocker.patch.object(ToxEnv, "_execute_call", side_effect=_execute_call, autospec=True)
-        return result
+        original_execute_call = ToxEnv._execute_call  # noqa: SLF001
+        return self.mocker.patch.object(ToxEnv, "_execute_call", side_effect=_execute_call, autospec=True)
 
     @property
     def structure(self) -> dict[str, Any]:
         result: dict[str, Any] = {}
         for dir_name, _, files in os.walk(str(self.path)):
             dir_path = Path(dir_name)
             into = result
@@ -257,16 +259,16 @@
                 into = into.setdefault(elem, {})
             for file_name in files:
                 into[file_name] = (dir_path / file_name).read_text()
         return result
 
     @contextmanager
     def chdir(self, to: Path | None = None) -> Iterator[None]:
-        cur_dir = os.getcwd()
-        os.chdir(str(to or self.path))
+        cur_dir = Path.cwd()
+        os.chdir(to or self.path)
         try:
             yield
         finally:
             os.chdir(cur_dir)
 
     def run(self, *args: str, from_cwd: Path | None = None) -> ToxRunOutcome:
         with self.chdir(from_cwd):
@@ -279,26 +281,27 @@
                 nonlocal state
                 state = previous_setup_state(value)
                 return state
 
             with self.monkeypatch.context() as m:
                 m.setattr(tox_env_api, "_CWD", self.path)
                 m.setattr(tox.run, "setup_state", our_setup_state)
-                m.setattr(sys, "argv", [sys.executable, "-m", "tox"] + list(args))
+                m.setattr(sys, "argv", [sys.executable, "-m", "tox", *list(args)])
                 m.setenv("VIRTUALENV_SYMLINK_APP_DATA", "1")
                 m.setenv("VIRTUALENV_SYMLINKS", "1")
                 m.setenv("VIRTUALENV_PIP", "embed")
                 m.setenv("VIRTUALENV_WHEEL", "embed")
                 m.setenv("VIRTUALENV_SETUPTOOLS", "embed")
                 try:
                     tox_run(args)
                 except SystemExit as exception:
                     code = exception.code
                 if code is None:  # pragma: no branch
-                    raise RuntimeError("exit code not set")
+                    msg = "exit code not set"
+                    raise RuntimeError(msg)
             out, err = self._capfd.readouterr()
             return ToxRunOutcome(args, self.path, cast(int, code), out, err, state)
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}(path={self.path}) at {id(self)}"
 
 
@@ -313,52 +316,61 @@
     from tox.tox_env.python.virtual_env.package.pyproject import Pep517VirtualEnvPackager
 
     def default_pass_env(self: Pep517VirtualEnvPackager) -> list[str]:
         result = previous(self)
         result.append("COV_*")
         return result
 
-    previous = Pep517VirtualEnvPackager._default_pass_env
+    previous = Pep517VirtualEnvPackager._default_pass_env  # noqa: SLF001
     try:
-        Pep517VirtualEnvPackager._default_pass_env = default_pass_env  # type: ignore
+        Pep517VirtualEnvPackager._default_pass_env = default_pass_env  # type: ignore[assignment]  # noqa: SLF001
         yield
     finally:
-        Pep517VirtualEnvPackager._default_pass_env = previous  # type: ignore
+        Pep517VirtualEnvPackager._default_pass_env = previous  # type: ignore[method-assign]  # noqa: SLF001
 
 
 class ToxRunOutcome:
-    def __init__(self, cmd: Sequence[str], cwd: Path, code: int, out: str, err: str, state: State | None) -> None:
+    def __init__(  # noqa: PLR0913
+        self,
+        cmd: Sequence[str],
+        cwd: Path,
+        code: int,
+        out: str,
+        err: str,
+        state: State | None,
+    ) -> None:
         extended_cmd = [sys.executable, "-m", "tox"]
         extended_cmd.extend(cmd)
         self.cmd: list[str] = extended_cmd
         self.cwd: Path = cwd
         self.code: int = code
         self.out: str = out
         self.err: str = err
         self._state: State | None = state
 
     @property
     def state(self) -> State:
         if self._state is None:
-            raise RuntimeError("no state")
+            msg = "no state"
+            raise RuntimeError(msg)
         return self._state
 
     def env_conf(self, name: str) -> EnvConfigSet:
         return self.state.conf.get_env(name)
 
     @property
     def success(self) -> bool:
         return self.code == Outcome.OK
 
     def assert_success(self) -> None:
-        assert self.success, repr(self)
+        assert self.success, repr(self)  # noqa: S101
 
     def assert_failed(self, code: int | None = None) -> None:
         status_match = self.code != 0 if code is None else self.code == code
-        assert status_match, f"should be {code}, got {self}"
+        assert status_match, f"should be {code}, got {self}"  # noqa: S101
 
     def __repr__(self) -> str:
         return "\n".join(
             "{}{}{}".format(k, "\n" if "\n" in v else ": ", v)
             for k, v in (
                 ("code", str(self.code)),
                 ("cmd", self.shell_cmd),
@@ -375,54 +387,54 @@
 
     def assert_out_err(self, out: str, err: str, *, dedent: bool = True, regex: bool = False) -> None:
         if dedent:
             out = textwrap.dedent(out).lstrip()
         if regex:
             self.matches(out, self.out, re.MULTILINE | re.DOTALL)
         else:
-            assert self.out == out
+            assert self.out == out  # noqa: S101
         if dedent:
             err = textwrap.dedent(err).lstrip()
         if regex:
             self.matches(err, self.err, re.MULTILINE | re.DOTALL)
         else:
-            assert self.err == err
+            assert self.err == err  # noqa: S101
 
     @staticmethod
     def matches(pattern: str, text: str, flags: int = 0) -> None:
         try:
             from re_assert import Matches
         except ImportError:  # pragma: no cover # hard to test
             match = re.match(pattern, text, flags)
             if match is None:
                 warnings.warn("install the re-assert PyPI package for bette error message", UserWarning, stacklevel=1)
-            assert match
+            assert match  # noqa: S101
         else:
-            assert Matches(pattern, flags=flags) == text
+            assert Matches(pattern, flags=flags) == text  # noqa: S101
 
 
 class ToxProjectCreator(Protocol):
     def __call__(
         self,
-        files: dict[str, Any],  # noqa: U100
-        base: Path | None = None,  # noqa: U100
-        prj_path: Path | None = None,  # noqa: U100
+        files: dict[str, Any],
+        base: Path | None = None,
+        prj_path: Path | None = None,
     ) -> ToxProject:
         ...
 
 
 @pytest.fixture(name="tox_project")
 def init_fixture(
     tmp_path: Path,
     capfd: CaptureFixture,
     monkeypatch: MonkeyPatch,
     mocker: MockerFixture,
 ) -> ToxProjectCreator:
     def _init(files: dict[str, Any], base: Path | None = None, prj_path: Path | None = None) -> ToxProject:
-        """create tox  projects"""
+        """Create tox  projects."""
         return ToxProject(files, base, prj_path or tmp_path / "p", capfd, monkeypatch, mocker)
 
     return _init
 
 
 @pytest.fixture()
 def empty_project(tox_project: ToxProjectCreator, monkeypatch: MonkeyPatch) -> ToxProject:
@@ -439,15 +451,15 @@
 
 
 def pytest_configure(config: PyTestConfig) -> None:
     config.addinivalue_line("markers", "integration")
     config.addinivalue_line("markers", "plugin_test")
 
 
-@pytest.hookimpl(trylast=True)  # type: ignore # not typed decorator
+@pytest.hookimpl(trylast=True)  # type: ignore[misc] # not typed decorator
 def pytest_collection_modifyitems(config: PyTestConfig, items: list[Function]) -> None:
     # do not require flags if called directly
     if len(items) == 1:  # pragma: no cover # hard to test
         return
 
     skip_int = pytest.mark.skip(reason=f"integration tests not run (no {_RUN_INTEGRATION_TEST_FLAG} flag)")
 
@@ -486,38 +498,38 @@
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as socket_handler:
         socket_handler.bind(("", 0))
         return cast(int, socket_handler.getsockname()[1])
 
 
 @pytest.fixture(autouse=True)
 def disable_pip_pypi_access(_invalid_index_fake_port: int, monkeypatch: MonkeyPatch) -> tuple[str, str | None]:
-    """set a fake pip index url, tests that want to use a pypi server should create and overwrite this"""
+    """Set a fake pip index url, tests that want to use a pypi server should create and overwrite this."""
     previous_url = os.environ.get("PIP_INDEX_URL")
     new_url = f"http://localhost:{_invalid_index_fake_port}/bad-pypi-server"
     monkeypatch.setenv("PIP_INDEX_URL", new_url)
     monkeypatch.setenv("PIP_RETRIES", str(0))
     monkeypatch.setenv("PIP_TIMEOUT", str(0.001))
     return new_url, previous_url
 
 
 @pytest.fixture(name="enable_pip_pypi_access")
 def enable_pip_pypi_access_fixture(
     disable_pip_pypi_access: tuple[str, str | None],
     monkeypatch: MonkeyPatch,
 ) -> str | None:
-    """set a fake pip index url, tests that want to use a pypi server should create and overwrite this"""
+    """Set a fake pip index url, tests that want to use a pypi server should create and overwrite this."""
     _, previous_url = disable_pip_pypi_access
     enable_pypi_server(monkeypatch, previous_url)
     return previous_url
 
 
 def register_inline_plugin(mocker: MockerFixture, *args: Callable[..., Any]) -> None:
     frame_info = inspect.stack()[1]
     caller_module = inspect.getmodule(frame_info[0])
-    assert caller_module is not None
+    assert caller_module is not None  # noqa: S101
     plugin = ModuleType(f"{caller_module.__name__}|{frame_info[3]}")
     plugin.__file__ = caller_module.__file__
     plugin.__dict__.update({f.__name__: f for f in args})
     mocker.patch("tox.plugin.manager.load_inline", return_value=plugin)
 
 
 __all__ = (
```

### Comparing `tox-4.6.0/src/tox/report.py` & `tox-4.6.1/src/tox/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""Handle reporting from within tox"""
+"""Handle reporting from within tox."""
 from __future__ import annotations
 
 import logging
 import os
 import sys
 from contextlib import contextmanager
 from io import BytesIO, TextIOWrapper
+from pathlib import Path
 from threading import Thread, current_thread, enumerate, local
 from typing import IO, Iterator, Tuple
 
-from colorama import Fore, Style, deinit, init
+from colorama import Fore, Style, init
 
 LEVELS = {
     0: logging.CRITICAL,
     1: logging.ERROR,
     2: logging.WARNING,
     3: logging.INFO,
     4: logging.DEBUG,
@@ -22,15 +23,15 @@
 
 MAX_LEVEL = max(LEVELS.keys())
 LOGGER = logging.getLogger()
 OutErr = Tuple[TextIOWrapper, TextIOWrapper]
 
 
 class _LogThreadLocal(local):
-    """A thread local variable that inherits values from its parent"""
+    """A thread local variable that inherits values from its parent."""
 
     _ident_to_data: dict[int | None, str] = {}
 
     def __init__(self, out_err: OutErr) -> None:
         self.name = self._ident_to_data.get(getattr(current_thread(), "parent_ident", None), "ROOT")
         self.out_err = out_err
 
@@ -64,15 +65,15 @@
         previous, self.name = self.name, name
         try:
             yield
         finally:
             self.name = previous
 
     @contextmanager
-    def suspend_out_err(self, yes: bool, out_err: OutErr | None = None) -> Iterator[OutErr]:
+    def suspend_out_err(self, yes: bool, out_err: OutErr | None = None) -> Iterator[OutErr]:  # noqa: FBT001
         previous_out, previous_err = self.out_err
         try:
             if yes:
                 if out_err is None:  # pragma: no branch
                     out = self._make(f"out-{self.name}", previous_out)
                     err = self._make(f"err-{self.name}", previous_err)
                 else:
@@ -93,33 +94,32 @@
         super().__init__()
         self.name: str = name
 
 
 class ToxHandler(logging.StreamHandler):  # type: ignore[type-arg] # is generic but at runtime doesn't take a type arg
     # """Controls tox output."""
 
-    def __init__(self, level: int, is_colored: bool, out_err: OutErr) -> None:
+    def __init__(self, level: int, is_colored: bool, out_err: OutErr) -> None:  # noqa: FBT001
         self._local = _LogThreadLocal(out_err)
         super().__init__(stream=self.stdout)
         if is_colored:
-            deinit()
             init()
         self._is_colored = is_colored
         self._setup_level(is_colored, level)
 
-    def _setup_level(self, is_colored: bool, level: int) -> None:
+    def _setup_level(self, is_colored: bool, level: int) -> None:  # noqa: FBT001
         self.setLevel(level)
         self._error_formatter = self._get_formatter(logging.ERROR, level, is_colored)
         self._warning_formatter = self._get_formatter(logging.WARNING, level, is_colored)
         self._remaining_formatter = self._get_formatter(logging.INFO, level, is_colored)
 
     @contextmanager
     def with_context(self, name: str) -> Iterator[None]:
         """
-        Set a new tox environment context
+        Set a new tox environment context.
 
         :param name: the name of the tox environment
         """
         with self._local.with_name(name):
             yield
 
     @property
@@ -139,29 +139,29 @@
 
     @property  # type: ignore[override]
     def stream(self) -> IO[str]:
         """:return: the current stream to write to (alias for the current standard output)"""
         return self.stdout
 
     @stream.setter
-    def stream(self, value: IO[str]) -> None:  # noqa: U100
-        """ignore anyone changing this"""
+    def stream(self, value: IO[str]) -> None:
+        """Ignore anyone changing this."""
 
     @contextmanager
-    def suspend_out_err(self, yes: bool, out_err: OutErr | None = None) -> Iterator[OutErr]:
+    def suspend_out_err(self, yes: bool, out_err: OutErr | None = None) -> Iterator[OutErr]:  # noqa: FBT001
         with self._local.suspend_out_err(yes, out_err) as out_err_res:
             yield out_err_res
 
     def write_out_err(self, out_err: tuple[bytes, bytes]) -> None:
         # read/write through the buffer as we collect bytes to print bytes (no transcoding needed)
         self.stdout.buffer.write(out_err[0])
         self.stderr.buffer.write(out_err[1])
 
     @staticmethod
-    def _get_formatter(level: int, enabled_level: int, is_colored: bool) -> logging.Formatter:
+    def _get_formatter(level: int, enabled_level: int, is_colored: bool) -> logging.Formatter:  # noqa: FBT001
         color: int | str = ""
         if is_colored:
             if level >= logging.ERROR:
                 color = Fore.RED
             elif level >= logging.WARNING:
                 color = Fore.CYAN
             else:
@@ -173,21 +173,20 @@
         fmt = f"{color} %(message)s{_c(Style.RESET_ALL)}"
         if enabled_level <= logging.DEBUG:
             fmt = (
                 f"{_c(Fore.GREEN)} %(relativeCreated)d %(levelname).1s{_c(Style.RESET_ALL)}{fmt}{_c(Style.DIM)}"
                 f" [%(pathname)s:%(lineno)d]{_c(Style.RESET_ALL)}"
             )
         fmt = f"{_c(Style.BRIGHT)}{_c(Fore.MAGENTA)}%(env_name)s:{_c(Style.RESET_ALL)}" + fmt
-        formatter = logging.Formatter(fmt)
-        return formatter
+        return logging.Formatter(fmt)
 
-    def format(self, record: logging.LogRecord) -> str:
+    def format(self, record: logging.LogRecord) -> str:  # noqa: A003
         # shorten the pathname to start from within the site-packages folder
         record.env_name = "root" if self._local.name is None else self._local.name
-        basename = os.path.dirname(record.pathname)
+        basename = str(Path(record.pathname).parent)
         len_sys_path_match = max((len(p) for p in sys.path if basename.startswith(p)), default=-1)
         record.pathname = record.pathname[len_sys_path_match + 1 :]
 
         if record.levelno >= logging.ERROR:
             return self._error_formatter.format(record)
         if record.levelno >= logging.WARNING:
             if self._is_colored and record.msg == "%s%s> %s" and record.args:
@@ -203,36 +202,32 @@
 
     def update_verbosity(self, verbosity: int) -> None:
         level = _get_level(verbosity)
         LOGGER.setLevel(level)
         self._setup_level(self._is_colored, level)
 
 
-def setup_report(verbosity: int, is_colored: bool) -> ToxHandler:
+def setup_report(verbosity: int, is_colored: bool) -> ToxHandler:  # noqa: FBT001
     _clean_handlers(LOGGER)
     level = _get_level(verbosity)
     LOGGER.setLevel(level)
     for name in ("distlib.util", "filelock"):
         logger = logging.getLogger(name)
         logger.disabled = True
     out_err: OutErr = (sys.stdout, sys.stderr)  # type: ignore[assignment]
     handler = ToxHandler(level, is_colored, out_err)
     LOGGER.addHandler(handler)
-
     logging.debug("setup logging to %s on pid %s", logging.getLevelName(level), os.getpid())
     return handler
 
 
 def _get_level(verbosity: int) -> int:
-    if verbosity > MAX_LEVEL:
-        verbosity = MAX_LEVEL
-    level = LEVELS[verbosity]
-    return level
+    return LEVELS[min(verbosity, MAX_LEVEL)]
 
 
 def _clean_handlers(log: logging.Logger) -> None:
     for log_handler in list(log.handlers):  # remove handlers of libraries
         log.removeHandler(log_handler)
 
 
 class HandledError(RuntimeError):
-    """Error that has been handled so no need for stack trace"""
+    """Error that has been handled so no need for stack trace."""
```

### Comparing `tox-4.6.0/src/tox/run.py` & `tox-4.6.1/src/tox/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,47 +13,46 @@
 from tox.session.state import State
 
 
 def run(args: Sequence[str] | None = None) -> None:
     try:
         with ToxHandler.patch_thread():
             result = main(sys.argv[1:] if args is None else args)
-    except Exception as exception:
+    except Exception as exception:  # noqa: BLE001
         if isinstance(exception, HandledError):
-            logging.error("%s| %s", type(exception).__name__, str(exception))
+            logging.error("%s| %s", type(exception).__name__, str(exception))  # noqa: TRY400
             result = -2
         else:
             raise
     except KeyboardInterrupt:
         result = -2
     finally:
         if "_TOX_SHOW_THREAD" in os.environ:  # pragma: no cover
             import threading  # pragma: no cover
 
             for thread in threading.enumerate():  # pragma: no cover
-                print(thread)  # pragma: no cover
+                print(thread)  # pragma: no cover  # noqa: T201
     raise SystemExit(result)
 
 
 def main(args: Sequence[str]) -> int:
     state = setup_state(args)
     from tox.provision import provision
 
     result = provision(state)
     if result is not False:
         return result
-    handler = state._options.cmd_handlers[state.conf.options.command]
+    handler = state._options.cmd_handlers[state.conf.options.command]  # noqa: SLF001
     result = handler(state)
     return result
 
 
 def setup_state(args: Sequence[str]) -> State:
     """Setup the state object of this run."""
     start = time.monotonic()
     # parse CLI arguments
     options = get_options(*args)
     options.parsed.start = start
     if options.parsed.exit_and_dump_after:
         faulthandler.dump_traceback_later(timeout=options.parsed.exit_and_dump_after, exit=True)  # pragma: no cover
     # build tox environment config objects
-    state = State(options, args)
-    return state
+    return State(options, args)
```

### Comparing `tox-4.6.0/src/tox/config/main.py` & `tox-4.6.1/src/tox/config/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from __future__ import annotations
 
 import os
 from collections import OrderedDict, defaultdict
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterator, Sequence, TypeVar
 
-from tox.config.loader.api import Loader, OverrideMap
-
-from .loader.memory import MemoryLoader
-from .loader.section import Section
 from .sets import ConfigSet, CoreConfigSet, EnvConfigSet
-from .source import Source
 
 if TYPE_CHECKING:
+    from tox.config.loader.api import Loader, OverrideMap
+
     from .cli.parser import Parsed
+    from .loader.memory import MemoryLoader
+    from .loader.section import Section
+    from .source import Source
 
 
 T = TypeVar("T", bound=ConfigSet)
 
 
 class Config:
     """Main configuration object for tox."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         config_source: Source,
         options: Parsed,
         root: Path,
         pos_args: Sequence[str] | None,
         work_dir: Path,
     ) -> None:
@@ -47,20 +47,23 @@
     def pos_args(self, to_path: Path | None) -> tuple[str, ...] | None:
         """
         :param to_path: if not None rewrite relative posargs paths from cwd to to_path
         :return: positional argument
         """
         if self._pos_args is not None and to_path is not None and Path.cwd() != to_path:
             args = []
-            to_path_str = os.path.abspath(str(to_path))  # we use os.path to unroll .. in path without resolve
+            # we use os.path to unroll .. in path without resolve
+            to_path_str = os.path.abspath(str(to_path))  # noqa: PTH100
             for arg in self._pos_args:
                 path_arg = Path(arg)
                 if path_arg.exists() and not path_arg.is_absolute():
-                    path_arg_str = os.path.abspath(str(path_arg))  # we use os.path to unroll .. in path without resolve
-                    relative = os.path.relpath(path_arg_str, to_path_str)  # we use os.path to not fail when not within
+                    # we use os.path to unroll .. in path without resolve
+                    path_arg_str = os.path.abspath(str(path_arg))  # noqa: PTH100
+                    # we use os.path to not fail when not within
+                    relative = os.path.relpath(path_arg_str, to_path_str)
                     args.append(relative)
                 else:
                     args.append(arg)
             return tuple(args)
         return self._pos_args
 
     @property
@@ -116,15 +119,15 @@
             return self._core_set
         core_section = self._src.get_core_section()
         core = CoreConfigSet(self, core_section, self._root, self.src_path)
         core.loaders.extend(self._src.get_loaders(core_section, base=[], override_map=self._overrides, conf=core))
         self._core_set = core
         return core
 
-    def get_section_config(
+    def get_section_config(  # noqa: PLR0913
         self,
         section: Section,
         base: list[str] | None,
         of_type: type[T],
         for_env: str | None,
         loaders: Sequence[Loader[Any]] | None = None,
     ) -> T:
@@ -141,34 +144,33 @@
             if loaders is not None:
                 conf_set.loaders.extend(loaders)
             return conf_set
 
     def get_env(
         self,
         item: str,
-        package: bool = False,
+        package: bool = False,  # noqa: FBT001, FBT002
         loaders: Sequence[Loader[Any]] | None = None,
     ) -> EnvConfigSet:
         """
         Return the configuration for a given tox environment (will create if not exist yet).
 
         :param item: the name of the environment
         :param package: a flag indicating if the environment is of type packaging or not (only used for creation)
         :param loaders: loaders to use for this configuration (only used for creation)
         :return: the tox environments config
         """
         section, base_test, base_pkg = self._src.get_tox_env_section(item)
-        conf_set = self.get_section_config(
+        return self.get_section_config(
             section,
             base=base_pkg if package else base_test,
             of_type=EnvConfigSet,
             for_env=item,
             loaders=loaders,
         )
-        return conf_set
 
     def clear_env(self, name: str) -> None:
         section, _, __ = self._src.get_tox_env_section(name)
         del self._key_to_conf_set[(section.key, name)]
 
 
 ___all__ = [
```

### Comparing `tox-4.6.0/src/tox/config/of_type.py` & `tox-4.6.1/src/tox/config/of_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-"""
-Group together configuration values that belong together (such as base tox configuration, tox environment configs)
-"""
+"""Group together configuration values (such as base tox configuration, tox environment configs)."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from itertools import product
 from typing import TYPE_CHECKING, Any, Callable, Generic, Iterable, TypeVar, cast
 
 from tox.config.loader.api import ConfigLoadArgs, Loader
-from tox.config.loader.convert import Factory
 
 if TYPE_CHECKING:
+    from tox.config.loader.convert import Factory
     from tox.config.main import Config  # pragma: no cover
 
 
 T = TypeVar("T")
 V = TypeVar("V")
 
 
 class ConfigDefinition(ABC, Generic[T]):
-    """Abstract base class for configuration definitions"""
+    """Abstract base class for configuration definitions."""
 
     def __init__(self, keys: Iterable[str], desc: str) -> None:
         self.keys = keys
         self.desc = desc
 
     @abstractmethod
     def __call__(self, conf: Config, loaders: list[Loader[T]], args: ConfigLoadArgs) -> T:
@@ -33,48 +31,44 @@
         return type(self) == type(o) and (self.keys, self.desc) == (o.keys, o.desc)
 
     def __ne__(self, o: Any) -> bool:
         return not (self == o)
 
 
 class ConfigConstantDefinition(ConfigDefinition[T]):
-    """A configuration definition whose value is defined upfront (such as the tox environment name)"""
+    """A configuration definition whose value is defined upfront (such as the tox environment name)."""
 
     def __init__(
         self,
         keys: Iterable[str],
         desc: str,
         value: Callable[[], T] | T,
     ) -> None:
         super().__init__(keys, desc)
         self.value = value
 
     def __call__(
         self,
-        conf: Config,  # noqa: U100
-        loaders: list[Loader[T]],  # noqa: U100
-        args: ConfigLoadArgs,  # noqa: U100
+        conf: Config,  # noqa: ARG002
+        loaders: list[Loader[T]],  # noqa: ARG002
+        args: ConfigLoadArgs,  # noqa: ARG002
     ) -> T:
-        if callable(self.value):
-            value = self.value()
-        else:
-            value = self.value
-        return value
+        return self.value() if callable(self.value) else self.value
 
     def __eq__(self, o: Any) -> bool:
         return type(self) == type(o) and super().__eq__(o) and self.value == o.value
 
 
 _PLACE_HOLDER = object()
 
 
 class ConfigDynamicDefinition(ConfigDefinition[T]):
-    """A configuration definition that comes from a source (such as in memory, an ini file, a toml file, etc.)"""
+    """A configuration definition that comes from a source (such as in memory, an ini file, a toml file, etc.)."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         keys: Iterable[str],
         desc: str,
         of_type: type[T],
         default: Callable[[Config, str | None], T] | T,
         post_process: Callable[[T], T] | None = None,
         factory: Factory[T] = None,
@@ -92,15 +86,16 @@
         loaders: list[Loader[T]],
         args: ConfigLoadArgs,
     ) -> T:
         if self._cache is _PLACE_HOLDER:
             for key, loader in product(self.keys, loaders):
                 chain_key = f"{loader.section.key}.{key}"
                 if chain_key in args.chain:
-                    raise ValueError(f"circular chain detected {', '.join(args.chain[args.chain.index(chain_key):])}")
+                    msg = f"circular chain detected {', '.join(args.chain[args.chain.index(chain_key):])}"
+                    raise ValueError(msg)
                 args.chain.append(chain_key)
                 try:
                     value = loader.load(key, self.of_type, self.factory, conf, args)
                 except KeyError:
                     continue
                 else:
                     break
```

### Comparing `tox-4.6.0/src/tox/config/set_env.py` & `tox-4.6.1/src/tox/config/set_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,27 +12,28 @@
 class SetEnv:
     def __init__(self, raw: str, name: str, env_name: str | None, root: Path) -> None:
         self.changed = False
         self._materialized: dict[str, str] = {}  # env vars we already loaded
         self._raw: dict[str, str] = {}  # could still need replacement
         self._needs_replacement: list[str] = []  # env vars that need replacement
         self._env_files: list[str] = []
-        self._replacer: Replacer = lambda s, c: s  # noqa: U100
+        self._replacer: Replacer = lambda s, c: s  # noqa: ARG005
         self._name, self._env_name, self._root = name, env_name, root
         from .loader.ini.replace import MatchExpression, find_replace_expr
 
         for line in raw.splitlines():
             if line.strip():
                 if line.startswith("file|"):
                     self._env_files.append(line[len("file|") :])
                 else:
                     try:
                         key, value = self._extract_key_value(line)
                         if "{" in key:
-                            raise ValueError(f"invalid line {line!r} in set_env")
+                            msg = f"invalid line {line!r} in set_env"
+                            raise ValueError(msg)  # noqa: TRY301
                     except ValueError:
                         for expr in find_replace_expr(line):
                             if isinstance(expr, MatchExpression):
                                 self._needs_replacement.append(line)
                                 break
                         else:
                             raise
@@ -47,29 +48,30 @@
     def _read_env_file(self, filename: str, args: ConfigLoadArgs) -> None:
         # Our rules in the documentation, some upstream environment file rules (we follow mostly the docker one):
         # - https://www.npmjs.com/package/dotenv#rules
         # - https://docs.docker.com/compose/env-file/
         env_file = Path(self._replacer(filename, args.copy()))  # apply any replace options
         env_file = env_file if env_file.is_absolute() else self._root / env_file
         if not env_file.exists():
-            raise Fail(f"{env_file} does not exist for set_env")
+            msg = f"{env_file} does not exist for set_env"
+            raise Fail(msg)
         for env_line in env_file.read_text().splitlines():
-            env_line = env_line.strip()
+            env_line = env_line.strip()  # noqa: PLW2901
             if not env_line or env_line.startswith("#"):
                 continue
             key, value = self._extract_key_value(env_line)
             self._raw[key] = value
 
     @staticmethod
     def _extract_key_value(line: str) -> tuple[str, str]:
         key, sep, value = line.partition("=")
         if sep:
             return key.strip(), value.strip()
-        else:
-            raise ValueError(f"invalid line {line!r} in set_env")
+        msg = f"invalid line {line!r} in set_env"
+        raise ValueError(msg)
 
     def load(self, item: str, args: ConfigLoadArgs | None = None) -> str:
         if item in self._materialized:
             return self._materialized[item]
         raw = self._raw[item]
         args = ConfigLoadArgs([], self._name, self._env_name) if args is None else args
         args.chain.append(f"env:{item}")
```

### Comparing `tox-4.6.0/src/tox/config/sets.py` & `tox-4.6.1/src/tox/config/sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from __future__ import annotations
 
 import sys
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Iterator, Mapping, Sequence, TypeVar, cast
 
-from .loader.convert import Factory
-from .loader.section import Section
 from .of_type import ConfigConstantDefinition, ConfigDefinition, ConfigDynamicDefinition, ConfigLoadArgs
 from .set_env import SetEnv
 from .types import EnvList
 
 if TYPE_CHECKING:
     from tox.config.loader.api import Loader
     from tox.config.main import Config
 
+    from .loader.convert import Factory
+    from .loader.section import Section
+
 V = TypeVar("V")
 
 
 class ConfigSet(ABC):
-    """A set of configuration that belong together (such as a tox environment settings, core tox settings)"""
+    """A set of configuration that belong together (such as a tox environment settings, core tox settings)."""
 
-    def __init__(self, conf: Config, section: Section, env_name: str | None):
+    def __init__(self, conf: Config, section: Section, env_name: str | None) -> None:
         self._section = section
         self._env_name = env_name
         self._conf = conf
         self.loaders: list[Loader[Any]] = []  #: active configuration loaders, can alter to change configuration values
         self._defined: dict[str, ConfigDefinition[Any]] = {}
         self._keys: dict[str, None] = {}
         self._alias: dict[str, str] = {}
@@ -35,15 +36,15 @@
     @abstractmethod
     def register_config(self) -> None:
         raise NotImplementedError
 
     def mark_finalized(self) -> None:
         self._final = True
 
-    def add_config(
+    def add_config(  # noqa: PLR0913
         self,
         keys: str | Sequence[str],
         of_type: type[V],
         default: Callable[[Config, str | None], V] | V,
         desc: str,
         post_process: Callable[[V], V] | None = None,
         factory: Factory[Any] = None,
@@ -57,15 +58,16 @@
         :param desc: a help message describing the configuration
         :param post_process: a callback to post-process the configuration value after it has been loaded
         :param factory: factory method used to build contained objects (if ``of_type`` is a container type it
           should perform the contained item creation, otherwise creates objects that match the type)
         :return: the new dynamic config definition
         """
         if self._final:
-            raise RuntimeError("config set has been marked final and cannot be extended")
+            msg = "config set has been marked final and cannot be extended"
+            raise RuntimeError(msg)
         keys_ = self._make_keys(keys)
         definition = ConfigDynamicDefinition(keys_, desc, of_type, default, post_process, factory)
         result = self._add_conf(keys_, definition)
         return cast(ConfigDynamicDefinition[V], result)
 
     def add_constant(self, keys: str | Sequence[str], desc: str, value: V) -> ConfigConstantDefinition[V]:
         """
@@ -73,15 +75,16 @@
 
         :param keys: the keys under what to register the config (first is primary key)
         :param desc: a help message describing the configuration
         :param value: the config value to use
         :return: the new constant config value
         """
         if self._final:
-            raise RuntimeError("config set has been marked final and cannot be extended")
+            msg = "config set has been marked final and cannot be extended"
+            raise RuntimeError(msg)
         keys_ = self._make_keys(keys)
         definition = ConfigConstantDefinition(keys_, desc, value)
         result = self._add_conf(keys_, definition)
         return cast(ConfigConstantDefinition[V], result)
 
     @staticmethod
     def _make_keys(keys: str | Sequence[str]) -> Sequence[str]:
@@ -98,15 +101,16 @@
             for key in keys:
                 self._defined[key] = definition
         return definition
 
     def _on_duplicate_conf(self, key: str, definition: ConfigDefinition[V]) -> None:
         earlier = self._defined[key]
         if definition != earlier:  # pragma: no branch
-            raise ValueError(f"config {key} already defined")
+            msg = f"config {key} already defined"
+            raise ValueError(msg)
 
     def __getitem__(self, item: str) -> Any:
         """
         Get the config value for a given key (will materialize in case of dynamic config).
 
         :param item: the config key
         :return: the configuration value
@@ -166,31 +170,31 @@
 
     @property
     def env_name(self) -> str | None:
         return self._env_name
 
 
 class CoreConfigSet(ConfigSet):
-    """Configuration set for the core tox config"""
+    """Configuration set for the core tox config."""
 
     def __init__(self, conf: Config, section: Section, root: Path, src_path: Path) -> None:
         self._root = root
         self._src_path = src_path
         super().__init__(conf, section=section, env_name=None)
         desc = "define environments to automatically run"
         self.add_config(keys=["env_list", "envlist"], of_type=EnvList, default=EnvList([]), desc=desc)
 
-    def _default_work_dir(self, conf: Config, env_name: str | None) -> Path:  # noqa: U100
+    def _default_work_dir(self, conf: Config, env_name: str | None) -> Path:  # noqa: ARG002
         return cast(Path, self["tox_root"] / ".tox")
 
-    def _default_temp_dir(self, conf: Config, env_name: str | None) -> Path:  # noqa: U100
+    def _default_temp_dir(self, conf: Config, env_name: str | None) -> Path:  # noqa: ARG002
         return cast(Path, self["work_dir"] / ".tmp")
 
-    def _work_dir_post_process(self, dir: Path) -> Path:
-        return self._conf.work_dir if self._conf.options.work_dir else dir
+    def _work_dir_post_process(self, folder: Path) -> Path:
+        return self._conf.work_dir if self._conf.options.work_dir else folder
 
     def register_config(self) -> None:
         self.add_constant(keys=["config_file_path"], desc="path to the configuration file", value=self._src_path)
         self.add_config(
             keys=["tox_root", "toxinidir"],
             of_type=Path,
             default=self._root,
@@ -208,20 +212,20 @@
             keys=["temp_dir"],
             of_type=Path,
             default=self._default_temp_dir,
             desc="a folder for temporary files (is not cleaned at start)",
         )
         self.add_constant("host_python", "the host python executable path", sys.executable)
 
-    def _on_duplicate_conf(self, key: str, definition: ConfigDefinition[V]) -> None:  # noqa: U100
+    def _on_duplicate_conf(self, key: str, definition: ConfigDefinition[V]) -> None:
         pass  # core definitions may be defined multiple times as long as all their options match, first defined wins
 
 
 class EnvConfigSet(ConfigSet):
-    """Configuration set for a tox environment"""
+    """Configuration set for a tox environment."""
 
     def __init__(self, conf: Config, section: Section, env_name: str) -> None:
         super().__init__(conf, section, env_name)
         self.default_set_env_loader: Callable[[], Mapping[str, str]] = lambda: {}
 
     def register_config(self) -> None:
         def set_env_post_process(values: SetEnv) -> SetEnv:
```

### Comparing `tox-4.6.0/src/tox/config/types.py` & `tox-4.6.1/src/tox/config/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class Command:
     """A command to execute."""
 
     def __init__(self, args: list[str]) -> None:
         """
-        Create a new command to execute
+        Create a new command to execute.
 
         :param args: the command line arguments (first value can be ``-`` to indicate ignore the exit code)
         """
         self.ignore_exit_code: bool = args[0] == "-"  #: a flag indicating if the exit code should be ignored
         self.args: list[str] = args[1:] if self.ignore_exit_code else args  #: the command line arguments
 
     def __repr__(self) -> str:
@@ -30,15 +30,15 @@
     @property
     def shell(self) -> str:
         """:return: a shell representation of the command (platform dependent)"""
         return shell_cmd(self.args)
 
 
 class EnvList:
-    """A tox environment list"""
+    """A tox environment list."""
 
     def __init__(self, envs: Sequence[str]) -> None:
         """
         Crate a new tox environment list.
 
         :param envs: the list of tox environments
         """
```

### Comparing `tox-4.6.0/src/tox/config/cli/env_var.py` & `tox-4.6.1/src/tox/config/cli/env_var.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-"""
-Provides configuration values from the environment variables.
-"""
+"""Provides configuration values from the environment variables."""
 from __future__ import annotations
 
 import logging
 import os
 from typing import Any
 
 from tox.config.loader.str_convert import StrConvert
 
 CONVERT = StrConvert()
 
 
 def get_env_var(key: str, of_type: type[Any]) -> tuple[Any, str] | None:
-    """Get the environment variable option.
+    """
+    Get the environment variable option.
 
     :param key: the config key requested
     :param of_type: the type we would like to convert it to
     :return:
     """
     key_upper = key.upper()
     for environ_key in (f"TOX_{key_upper}", f"TOX{key_upper}"):
         if environ_key in os.environ:
             value = os.environ[environ_key]
             try:
-                source = f"env var {environ_key}"
                 result = CONVERT.to(raw=value, of_type=of_type, factory=None)
-                return result, source
-            except Exception as exception:
+            except Exception as exception:  # noqa: BLE001
                 logging.warning(
                     "env var %s=%r cannot be transformed to %r because %r",
                     environ_key,
                     value,
                     of_type,
                     exception,
                 )
+            else:
+                return result, f"env var {environ_key}"
     return None
 
 
 __all__ = ("get_env_var",)
```

### Comparing `tox-4.6.0/src/tox/config/cli/ini.py` & `tox-4.6.1/src/tox/config/cli/ini.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Provides configuration values from tox.ini files.
-"""
+"""Provides configuration values from tox.ini files."""
 from __future__ import annotations
 
 import logging
 import os
 from configparser import ConfigParser
 from pathlib import Path
 from typing import Any
@@ -35,16 +33,16 @@
             try:
                 parser = ConfigParser(interpolation=None)
                 with self.config_file.open() as file_handler:
                     parser.read_file(file_handler)
                 self.has_tox_section = parser.has_section(CORE.key)
                 if self.has_tox_section:
                     self.ini = IniLoader(CORE, parser, overrides=[], core_section=CORE)
-            except Exception as exception:
-                logging.error("failed to read config file %s because %r", config_file, exception)
+            except Exception as exception:  # noqa: BLE001
+                logging.error("failed to read config file %s because %r", config_file, exception)  # noqa: TRY400
                 self.has_config_file = None
 
     def get(self, key: str, of_type: type[Any]) -> Any:
         cache_key = key, of_type
         if cache_key in self._cache:
             result = self._cache[cache_key]
         else:
@@ -54,15 +52,15 @@
                 else:
                     source = "file"
                     args = ConfigLoadArgs(chain=[key], name=CORE.prefix, env_name=None)
                     value = self.ini.load(key, of_type=of_type, conf=None, factory=None, args=args)
                     result = value, source
             except KeyError:  # just not found
                 result = None
-            except Exception as exception:
+            except Exception as exception:  # noqa: BLE001
                 logging.warning("%s key %s as type %r failed with %r", self.config_file, key, of_type, exception)
                 result = None
         self._cache[cache_key] = result
         return result
 
     def __bool__(self) -> bool:
         return bool(self.has_config_file) and bool(self.has_tox_section)
```

### Comparing `tox-4.6.0/src/tox/config/cli/parse.py` & `tox-4.6.1/src/tox/config/cli/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-This module pulls together this package: create and parse CLI arguments for tox.
-"""
+"""This module pulls together this package: create and parse CLI arguments for tox."""
 from __future__ import annotations
 
 import os
 from contextlib import redirect_stderr
 from pathlib import Path
 from typing import TYPE_CHECKING, Callable, NamedTuple, Sequence, cast
 
@@ -43,17 +41,16 @@
 
 
 def _get_base(args: Sequence[str]) -> tuple[int, ToxHandler, Source]:
     """First just load the base options (verbosity+color) to setup the logging framework."""
     tox_parser = ToxParser.base()
     parsed = Parsed()
     try:
-        with open(os.devnull, "w") as file_handler:
-            with redirect_stderr(file_handler):
-                tox_parser.parse_known_args(args, namespace=parsed)
+        with Path(os.devnull).open("w") as file_handler, redirect_stderr(file_handler):
+            tox_parser.parse_known_args(args, namespace=parsed)
     except SystemExit:
         ...  # ignore parse errors, such as -va raises ignored explicit argument 'a'
     guess_verbosity = parsed.verbosity
     handler = setup_report(guess_verbosity, parsed.is_colored)
     from tox.plugin.manager import MANAGER  # load the plugin system right after we set up report
 
     source = discover_source(parsed.config_file, parsed.root_dir)
```

### Comparing `tox-4.6.0/src/tox/config/cli/parser.py` & `tox-4.6.1/src/tox/config/cli/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Customize argparse logic for tox (also contains the base options).
-"""
+"""Customize argparse logic for tox (also contains the base options)."""
 from __future__ import annotations
 
 import argparse
 import logging
 import os
 import sys
 from argparse import SUPPRESS, Action, ArgumentDefaultsHelpFormatter, ArgumentParser, Namespace
@@ -23,17 +21,15 @@
     from typing_extensions import Literal
 
 if TYPE_CHECKING:
     from tox.session.state import State
 
 
 class ArgumentParserWithEnvAndConfig(ArgumentParser):
-    """
-    Argument parser which updates its defaults by checking the configuration files and environmental variables.
-    """
+    """Argument parser which updates its defaults by checking the configuration files and environmental variables."""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         # sub-parsers also construct an instance of the parser, but they don't get their own file config, but inherit
         self.file_config = kwargs.pop("file_config") if "file_config" in kwargs else IniConfig()
         kwargs["epilog"] = self.file_config.epilog
         super().__init__(*args, **kwargs)
 
@@ -47,57 +43,56 @@
             key = action.dest
             outcome = get_env_var(key, of_type=of_type)
             if outcome is None and self.file_config:
                 outcome = self.file_config.get(key, of_type=of_type)
             if outcome is not None:
                 action.default, default_value = outcome
                 action.default_source = default_value  # type: ignore[attr-defined]
-        if isinstance(action, argparse._SubParsersAction):
+        if isinstance(action, argparse._SubParsersAction):  # noqa: SLF001
             for values in action.choices.values():
                 if not isinstance(values, ToxParser):  # pragma: no cover
-                    raise RuntimeError("detected sub-parser added without using our own add command")
+                    msg = "detected sub-parser added without using our own add command"
+                    raise RuntimeError(msg)  # noqa: TRY004
                 values.fix_defaults()
 
     @staticmethod
     def get_type(action: Action) -> type[Any]:
         of_type: type[Any] | None = getattr(action, "of_type", None)
         if of_type is None:
-            if isinstance(action, argparse._AppendAction):
+            if isinstance(action, argparse._AppendAction):  # noqa: SLF001
                 of_type = List[action.type]  # type: ignore[name-defined]
-            elif isinstance(action, argparse._StoreAction) and action.choices:
+            elif isinstance(action, argparse._StoreAction) and action.choices:  # noqa: SLF001
                 loc = locals()
                 loc["Literal"] = Literal
                 as_literal = f"Literal[{', '.join(repr(i) for i in action.choices)}]"
-                of_type = eval(as_literal, globals(), loc)
+                of_type = eval(as_literal, globals(), loc)  # noqa: PGH001
             elif action.default is not None:
                 of_type = type(action.default)
-            elif isinstance(action, argparse._StoreConstAction) and action.const is not None:
+            elif isinstance(action, argparse._StoreConstAction) and action.const is not None:  # noqa: SLF001
                 of_type = type(action.const)
             else:
                 raise TypeError(action)
         return of_type
 
-    def parse_args(  # type: ignore # avoid defining all overloads
+    def parse_args(  # type: ignore[override] # avoid defining all overloads
         self,
         args: Sequence[str] | None = None,
         namespace: Namespace | None = None,
     ) -> Namespace:
         res, argv = self.parse_known_args(args, namespace)
         if argv:
             self.error(
                 f'unrecognized arguments: {" ".join(argv)}\n'
                 "hint: if you tried to pass arguments to a command use -- to separate them from tox ones",
             )
         return res
 
 
 class HelpFormatter(ArgumentDefaultsHelpFormatter):
-    """
-    A help formatter that provides the default value and the source it comes from.
-    """
+    """A help formatter that provides the default value and the source it comes from."""
 
     def __init__(self, prog: str) -> None:
         super().__init__(prog, max_help_position=30, width=240)
 
     def _get_help_string(self, action: Action) -> str | None:
         text: str = super()._get_help_string(action) or ""
         if hasattr(action, "default_source"):
@@ -115,15 +110,15 @@
 
 
 ToxParserT = TypeVar("ToxParserT", bound="ToxParser")
 DEFAULT_VERBOSITY = 2
 
 
 class Parsed(Namespace):
-    """CLI options"""
+    """CLI options."""
 
     @property
     def verbosity(self) -> int:
         """:return: reporting verbosity"""
         result: int = max(self.verbose - self.quiet, 0)
         return result
 
@@ -161,15 +156,16 @@
         self,
         cmd: str,
         aliases: Sequence[str],
         help_msg: str,
         handler: Callable[[State], int],
     ) -> ArgumentParser:
         if self._cmd is None:
-            raise RuntimeError("no sub-command group allowed")
+            msg = "no sub-command group allowed"
+            raise RuntimeError(msg)
         sub_parser: ToxParser = self._cmd.add_parser(
             cmd,
             help=help_msg,
             aliases=aliases,
             formatter_class=HelpFormatter,
             file_config=self.file_config,
         )
@@ -186,34 +182,33 @@
                 excl_group = group.add_mutually_exclusive_group(**e_kwargs)
                 for a_args, _, a_kwargs in arguments:
                     excl_group.add_argument(*a_args, **a_kwargs)
         return sub_parser
 
     def add_argument_group(self, *args: Any, **kwargs: Any) -> Any:
         result = super().add_argument_group(*args, **kwargs)
-        if self.of_cmd is None:
-            if args not in (("positional arguments",), ("optional arguments",)):
+        if self.of_cmd is None and args not in (("positional arguments",), ("optional arguments",)):
 
-                def add_mutually_exclusive_group(**e_kwargs: Any) -> Any:
-                    def add_argument(*a_args: str, of_type: type[Any] | None = None, **a_kwargs: Any) -> Action:
-                        res_args: Action = prev_add_arg(*a_args, **a_kwargs)  # type: ignore[has-type]
-                        arguments.append((a_args, of_type, a_kwargs))
-                        return res_args
-
-                    arguments: list[ArgumentArgs] = []
-                    excl.append((e_kwargs, arguments))
-                    res_excl = prev_excl(**kwargs)
-                    prev_add_arg = res_excl.add_argument
-                    res_excl.add_argument = add_argument  # type: ignore[method-assign]
-                    return res_excl
-
-                prev_excl = result.add_mutually_exclusive_group
-                result.add_mutually_exclusive_group = add_mutually_exclusive_group  # type: ignore[method-assign]
-                excl: list[tuple[dict[str, Any], list[ArgumentArgs]]] = []
-                self._groups.append((args, kwargs, excl))
+            def add_mutually_exclusive_group(**e_kwargs: Any) -> Any:
+                def add_argument(*a_args: str, of_type: type[Any] | None = None, **a_kwargs: Any) -> Action:
+                    res_args: Action = prev_add_arg(*a_args, **a_kwargs)  # type: ignore[has-type]
+                    arguments.append((a_args, of_type, a_kwargs))
+                    return res_args
+
+                arguments: list[ArgumentArgs] = []
+                excl.append((e_kwargs, arguments))
+                res_excl = prev_excl(**kwargs)
+                prev_add_arg = res_excl.add_argument
+                res_excl.add_argument = add_argument  # type: ignore[method-assign]
+                return res_excl
+
+            prev_excl = result.add_mutually_exclusive_group
+            result.add_mutually_exclusive_group = add_mutually_exclusive_group  # type: ignore[method-assign]
+            excl: list[tuple[dict[str, Any], list[ArgumentArgs]]] = []
+            self._groups.append((args, kwargs, excl))
         return result
 
     def add_argument(self, *args: str, of_type: type[Any] | None = None, **kwargs: Any) -> Action:
         result = super().add_argument(*args, **kwargs)
         if self.of_cmd is None and result.dest != "help":
             self._arguments.append((args, of_type, kwargs))
             if hasattr(self, "_cmd") and self._cmd is not None and hasattr(self._cmd, "choices"):
@@ -266,15 +261,15 @@
         _, args = super().parse_known_args(args, namespace=result)
         return result, args
 
 
 def add_verbosity_flags(parser: ArgumentParser) -> None:
     from tox.report import LEVELS
 
-    level_map = "|".join(f"{c}={logging.getLevelName(l)}" for c, l in sorted(LEVELS.items()))
+    level_map = "|".join(f"{c}={logging.getLevelName(level)}" for c, level in sorted(LEVELS.items()))
     verbosity_group = parser.add_argument_group("verbosity")
     verbosity_group.description = (
         f"every -v increases, every -q decreases verbosity level, "
         f"default {logging.getLevelName(LEVELS[DEFAULT_VERBOSITY])}, map {level_map}"
     )
     verbosity = verbosity_group.add_mutually_exclusive_group()
     verbosity.add_argument(
@@ -286,15 +281,15 @@
         default=DEFAULT_VERBOSITY,
     )
     verbosity.add_argument("-q", "--quiet", action="count", dest="quiet", help="decrease verbosity", default=0)
 
 
 def add_color_flags(parser: ArgumentParser) -> None:
     converter = StrConvert()
-    if os.environ.get("NO_COLOR", "") != "":
+    if os.environ.get("NO_COLOR", ""):
         color = "no"
     elif converter.to_bool(os.environ.get("FORCE_COLOR", "")):
         color = "yes"
     elif os.environ.get("TERM", "") == "dumb":
         color = "no"
     else:
         color = "yes" if sys.stdout.isatty() else "no"
```

### Comparing `tox-4.6.0/src/tox/config/loader/api.py` & `tox-4.6.1/src/tox/config/loader/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from abc import abstractmethod
 from argparse import ArgumentTypeError
 from typing import TYPE_CHECKING, Any, List, Mapping, TypeVar
 
 from tox.plugin import impl
 
 from .convert import Convert, Factory
-from .section import Section
 from .str_convert import StrConvert
 
 if TYPE_CHECKING:
     from tox.config.cli.parser import ToxParser
     from tox.config.main import Config
 
+    from .section import Section
+
 
 class Override:
-    """
-    An override for config definitions.
-    """
+    """An override for config definitions."""
 
     def __init__(self, value: str) -> None:
         key, equal, self.value = value.partition("=")
         if not equal:
-            raise ArgumentTypeError(f"override {value} has no = sign in it")
+            msg = f"override {value} has no = sign in it"
+            raise ArgumentTypeError(msg)
         self.namespace, _, self.key = key.rpartition(".")
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}('{self}')"
 
     def __str__(self) -> str:
         return f"{self.namespace}{'.' if self.namespace else ''}{self.key}={self.value}"
@@ -40,15 +40,15 @@
     def __ne__(self, other: Any) -> bool:
         return not (self == other)
 
 
 class ConfigLoadArgs:
     """Arguments that help loading a configuration value."""
 
-    def __init__(self, chain: list[str] | None, name: str | None, env_name: str | None):
+    def __init__(self, chain: list[str] | None, name: str | None, env_name: str | None) -> None:
         """
         :param chain: the configuration chain (useful to detect circular references)
         :param name: the name of the configuration
         :param env_name: the tox environment this load is for
         """
         self.chain: list[str] = chain or []
         self.name = name
@@ -95,15 +95,15 @@
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}"
 
     def __contains__(self, item: str) -> bool:
         return item in self.found_keys()
 
-    def load(
+    def load(  # noqa: PLR0913
         self,
         key: str,
         of_type: type[V],
         factory: Factory[V],
         conf: Config | None,
         args: ConfigLoadArgs,
     ) -> V:
@@ -118,22 +118,22 @@
         :return: the converted type
         """
         if key in self.overrides:
             return _STR_CONVERT.to(self.overrides[key].value, of_type, factory)
         raw = self.load_raw(key, conf, args.env_name)
         return self.build(key, of_type, factory, conf, raw, args)
 
-    def build(
+    def build(  # noqa: PLR0913
         self,
-        key: str,  # noqa: U100
+        key: str,  # noqa: ARG002
         of_type: type[V],
         factory: Factory[V],
-        conf: Config | None,  # noqa: U100
+        conf: Config | None,  # noqa: ARG002
         raw: T,
-        args: ConfigLoadArgs,  # noqa: U100
+        args: ConfigLoadArgs,  # noqa: ARG002
     ) -> V:
         """
         Materialize the raw configuration value from the loader.
 
         :param future: a future which when called will provide the converted config value
         :param key: the config key
         :param of_type: the config type
```

### Comparing `tox-4.6.0/src/tox/config/loader/convert.py` & `tox-4.6.1/src/tox/config/loader/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from pathlib import Path
 from typing import Any, Callable, Dict, Generic, Iterator, List, Optional, Set, TypeVar, Union, cast
 
-from ..types import Command, EnvList
+from tox.config.types import Command, EnvList
 
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from typing import Literal
 else:  # pragma: no cover (py38+)
     from typing_extensions import Literal
 
 
@@ -18,19 +18,19 @@
 T = TypeVar("T")
 V = TypeVar("V")
 
 Factory = Optional[Callable[[object], T]]  # note the argument is anything, due e.g. memory loader can inject anything
 
 
 class Convert(ABC, Generic[T]):
-    """A class that converts a raw type to a given tox (python) type"""
+    """A class that converts a raw type to a given tox (python) type."""
 
-    def to(self, raw: T, of_type: type[V], factory: Factory[V]) -> V:
+    def to(self, raw: T, of_type: type[V], factory: Factory[V]) -> V:  # noqa: PLR0911
         """
-        Convert given raw type to python type
+        Convert given raw type to python type.
 
         :param raw: the raw type
         :param of_type: python type
         :param factory: factory method to build the object
         :return: the converted type
         """
         from_module = getattr(of_type, "__module__", None)
@@ -49,15 +49,15 @@
         if isinstance(raw, of_type):  # already target type no need to transform it
             # do it this late to allow normalization - e.g. string strip
             return raw
         if factory:
             return factory(raw)
         return of_type(raw)  # type: ignore[call-arg]
 
-    def _to_typing(self, raw: T, of_type: type[V], factory: Factory[V]) -> V:
+    def _to_typing(self, raw: T, of_type: type[V], factory: Factory[V]) -> V:  # noqa: C901
         origin = getattr(of_type, "__origin__", of_type.__class__)
         result: Any = _NO_MAPPING
         if origin in (list, List):
             entry_type = of_type.__args__[0]  # type: ignore[attr-defined]
             result = [self.to(i, entry_type, factory) for i in self.to_list(raw, entry_type)]
         elif origin in (set, Set):
             entry_type = of_type.__args__[0]  # type: ignore[attr-defined]
@@ -67,30 +67,32 @@
             result = OrderedDict(
                 (self.to(k, key_type, factory), self.to(v, value_type, factory))
                 for k, v in self.to_dict(raw, (key_type, value_type))
             )
         elif origin == Union:  # handle Optional values
             args: list[type[Any]] = of_type.__args__  # type: ignore[attr-defined]
             none = type(None)
-            if len(args) == 2 and none in args:  # type: ignore[comparison-overlap]
+            if len(args) == 2 and none in args:  # type: ignore[comparison-overlap]  # noqa: PLR2004
                 if isinstance(raw, str):
                     raw = raw.strip()  # type: ignore[assignment]
                 if not raw:
                     result = None
                 else:
-                    new_type = next(i for i in args if i != none)  # type: ignore # pragma: no cover
+                    new_type = next(i for i in args if i != none)  # type: ignore[comparison-overlap] # pragma: no cover
                     result = self.to(raw, new_type, factory)
         elif origin in (Literal, type(Literal)):
             choice = of_type.__args__  # type: ignore[attr-defined]
             if raw not in choice:
-                raise ValueError(f"{raw} must be one of {choice}")
+                msg = f"{raw} must be one of {choice}"
+                raise ValueError(msg)
             result = raw
         if result is not _NO_MAPPING:
             return cast(V, result)
-        raise TypeError(f"{raw} cannot cast to {of_type!r}")
+        msg = f"{raw} cannot cast to {of_type!r}"
+        raise TypeError(msg)
 
     @staticmethod
     @abstractmethod
     def to_str(value: T) -> str:
         """
         Convert to string.
```

### Comparing `tox-4.6.0/src/tox/config/loader/memory.py` & `tox-4.6.1/src/tox/config/loader/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,38 +14,38 @@
 
 
 class MemoryLoader(Loader[Any]):
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(Section(prefix="<memory>", name=str(id(self))), [])
         self.raw: dict[str, Any] = {**kwargs}
 
-    def load_raw(self, key: Any, conf: Config | None, env_name: str | None) -> Any:  # noqa: U100
+    def load_raw(self, key: Any, conf: Config | None, env_name: str | None) -> Any:  # noqa: ARG002
         return self.raw[key]
 
     def found_keys(self) -> set[str]:
         return set(self.raw.keys())
 
     @staticmethod
     def to_bool(value: Any) -> bool:
         return bool(value)
 
     @staticmethod
     def to_str(value: Any) -> str:
         return str(value)
 
     @staticmethod
-    def to_list(value: Any, of_type: type[Any]) -> Iterator[Any]:  # noqa: U100
+    def to_list(value: Any, of_type: type[Any]) -> Iterator[Any]:  # noqa: ARG004
         return iter(value)
 
     @staticmethod
-    def to_set(value: Any, of_type: type[Any]) -> Iterator[Any]:  # noqa: U100
+    def to_set(value: Any, of_type: type[Any]) -> Iterator[Any]:  # noqa: ARG004
         return iter(value)
 
     @staticmethod
-    def to_dict(value: Any, of_type: tuple[type[Any], type[Any]]) -> Iterator[tuple[Any, Any]]:  # noqa: U100
+    def to_dict(value: Any, of_type: tuple[type[Any], type[Any]]) -> Iterator[tuple[Any, Any]]:  # noqa: ARG004
         return value.items()  # type: ignore[no-any-return]
 
     @staticmethod
     def to_path(value: Any) -> Path:
         return Path(value)
 
     @staticmethod
```

### Comparing `tox-4.6.0/src/tox/config/loader/section.py` & `tox-4.6.1/src/tox/config/loader/section.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Any, TypeVar
 
 _Section = TypeVar("_Section", bound="Section")
 
 
 class Section:
-    """tox configuration section"""
+    """tox configuration section."""
 
     SEP = ":"  #: string used to separate the prefix and the section in the key
 
     def __init__(self, prefix: str | None, name: str) -> None:
         self._prefix = prefix
         self._name = name
 
@@ -47,13 +47,16 @@
     def __str__(self) -> str:
         return self.key
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(prefix={self._prefix!r}, name={self._name!r})"
 
     def __eq__(self, other: Any) -> bool:
-        return isinstance(other, self.__class__) and (self._prefix, self._name) == (other._prefix, other.name)
+        return isinstance(other, self.__class__) and (self._prefix, self._name) == (
+            other._prefix,  # noqa: SLF001
+            other.name,
+        )
 
 
 __all__ = [
     "Section",
 ]
```

### Comparing `tox-4.6.0/src/tox/config/loader/str_convert.py` & `tox-4.6.1/src/tox/config/loader/str_convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any, Iterator
 
 from tox.config.loader.convert import Convert
 from tox.config.types import Command, EnvList
 
 
 class StrConvert(Convert[str]):
-    """A class converting string values to tox types"""
+    """A class converting string values to tox types."""
 
     @staticmethod
     def to_str(value: str) -> str:
         return str(value).strip()
 
     @staticmethod
     def to_path(value: str) -> Path:
@@ -32,22 +32,23 @@
                 yield value
 
     @staticmethod
     def to_set(value: str, of_type: type[Any]) -> Iterator[str]:
         yield from StrConvert.to_list(value, of_type)
 
     @staticmethod
-    def to_dict(value: str, of_type: tuple[type[Any], type[Any]]) -> Iterator[tuple[str, str]]:  # noqa: U100
+    def to_dict(value: str, of_type: tuple[type[Any], type[Any]]) -> Iterator[tuple[str, str]]:  # noqa: ARG004
         for row in value.split("\n"):
             if row.strip():
                 key, sep, value = row.partition("=")
                 if sep:
                     yield key.strip(), value.strip()
                 else:
-                    raise TypeError(f"dictionary lines must be of form key=value, found {row!r}")
+                    msg = f"dictionary lines must be of form key=value, found {row!r}"
+                    raise TypeError(msg)
 
     @staticmethod
     def _win32_process_path_backslash(value: str, escape: str, special_chars: str) -> str:
         """
         Escape backslash in value that is not followed by a special character.
 
         This allows windows paths to be written without double backslash, while
@@ -86,24 +87,25 @@
         splitter.commenters = ""  # comments handled earlier, and the shlex does not know escaped comment characters
         args: list[str] = []
         pos = 0
         try:
             for arg in splitter:
                 if is_win and len(arg) > 1 and arg[0] == arg[-1] and arg.startswith(("'", '"')):  # pragma: win32 cover
                     # on Windows quoted arguments will remain quoted, strip it
-                    arg = arg[1:-1]
+                    arg = arg[1:-1]  # noqa: PLW2901
                 args.append(arg)
                 pos = splitter.instream.tell()
         except ValueError:
             args.append(value[pos:])
         if len(args) == 0:
-            raise ValueError(f"attempting to parse {value!r} into a command failed")
+            msg = f"attempting to parse {value!r} into a command failed"
+            raise ValueError(msg)
         if args[0] != "-" and args[0].startswith("-"):
             args[0] = args[0][1:]
-            args = ["-"] + args
+            args = ["-", *args]
         return Command(args)
 
     @staticmethod
     def to_env_list(value: str) -> EnvList:
         from tox.config.loader.ini.factor import extend_factors
 
         elements = list(chain.from_iterable(extend_factors(expr) for expr in value.split("\n")))
@@ -114,16 +116,15 @@
     VALID_BOOL = sorted(TRUTHFUL_VALUES | FALSE_VALUES)
 
     @staticmethod
     def to_bool(value: str) -> bool:
         norm = str(value).strip().lower()
         if norm in StrConvert.TRUTHFUL_VALUES:
             return True
-        elif norm in StrConvert.FALSE_VALUES:
+        if norm in StrConvert.FALSE_VALUES:
             return False
-        else:
-            raise TypeError(
-                f"value {value!r} cannot be transformed to bool, valid: {', '.join(StrConvert.VALID_BOOL)}",
-            )
+
+        msg = f"value {value!r} cannot be transformed to bool, valid: {', '.join(StrConvert.VALID_BOOL)}"
+        raise TypeError(msg)
 
 
 __all__ = ("StrConvert",)
```

### Comparing `tox-4.6.0/src/tox/config/loader/stringify.py` & `tox-4.6.1/src/tox/config/loader/stringify.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Mapping, Sequence, Set
 
 from tox.config.set_env import SetEnv
 from tox.config.types import Command, EnvList
 from tox.tox_env.python.pip.req_file import PythonDeps
 
 
-def stringify(value: Any) -> tuple[str, bool]:
+def stringify(value: Any) -> tuple[str, bool]:  # noqa: PLR0911
     """
     Transform a value into a string representation.
 
     :param value: the value in question
     :return: a tuple, first the value as str, second a flag if the value if a multi-line one
     """
     if isinstance(value, str):
```

### Comparing `tox-4.6.0/src/tox/config/loader/ini/__init__.py` & `tox-4.6.1/src/tox/config/loader/ini/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 
 import inspect
 import re
-from configparser import ConfigParser, SectionProxy
 from typing import TYPE_CHECKING, TypeVar
 
 from tox.config.loader.api import ConfigLoadArgs, Loader, Override
-from tox.config.loader.convert import Factory
 from tox.config.loader.ini.factor import filter_for_env
 from tox.config.loader.ini.replace import replace
-from tox.config.loader.section import Section
 from tox.config.loader.str_convert import StrConvert
 from tox.config.set_env import SetEnv
 from tox.report import HandledError
 
 if TYPE_CHECKING:
+    from configparser import ConfigParser, SectionProxy
+
+    from tox.config.loader.convert import Factory
+    from tox.config.loader.section import Section
     from tox.config.main import Config
 
 V = TypeVar("V")
 _COMMENTS = re.compile(r"(\s)*(?<!\\)#.*")
 
 
 class IniLoader(StrConvert, Loader[str]):
-    """Load configuration from an ini section (ini file is a string to string dictionary)"""
+    """Load configuration from an ini section (ini file is a string to string dictionary)."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         section: Section,
         parser: ConfigParser,
         overrides: list[Override],
         core_section: Section,
         section_key: str | None = None,
     ) -> None:
@@ -45,22 +46,21 @@
         # strip comments
         elements: list[str] = []
         for line in value.split("\n"):
             if not line.startswith("#"):
                 part = _COMMENTS.sub("", line)
                 elements.append(part.replace("\\#", "#"))
         strip_comments = "\n".join(elements)
-        if conf is None:  # conf is None when we're loading the global tox configuration file for the CLI
+        if conf is None:  # noqa: SIM108 # conf is None when we're loading the global tox configuration file for the CLI
             factor_filtered = strip_comments  # we don't support factor and replace functionality there
         else:
             factor_filtered = filter_for_env(strip_comments, env_name)  # select matching factors
-        collapsed = factor_filtered.replace("\r", "").replace("\\\n", "")  # collapse explicit new-line escape
-        return collapsed
+        return factor_filtered.replace("\r", "").replace("\\\n", "")  # collapse explicit new-line escape
 
-    def build(
+    def build(  # noqa: PLR0913
         self,
         key: str,
         of_type: type[V],
         factory: Factory[V],
         conf: Config | None,
         raw: str,
         args: ConfigLoadArgs,
@@ -69,15 +69,15 @@
 
         def replacer(raw_: str, args_: ConfigLoadArgs) -> str:
             if conf is None:
                 replaced = raw_  # no replacement supported in the core section
             else:
                 try:
                     replaced = replace(conf, self, raw_, args_)  # do replacements
-                except Exception as exception:
+                except Exception as exception:  # noqa: BLE001
                     if isinstance(exception, HandledError):
                         raise
                     name = self.core_section.key if args_.env_name is None else args_.env_name
                     msg = f"replace failed in {name}.{key} with {exception!r}"
                     raise HandledError(msg) from exception
             return replaced
```

### Comparing `tox-4.6.0/src/tox/config/loader/ini/factor.py` & `tox-4.6.1/src/tox/config/loader/ini/factor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Expand tox factor expressions to tox environment list.
-"""
+"""Expand tox factor expressions to tox environment list."""
 from __future__ import annotations
 
 import re
 from itertools import chain, groupby, product
 from typing import Iterator
 
 
@@ -18,16 +16,15 @@
             if content:
                 overall.append(content)
         else:
             for group in factors:
                 if all((a_name in current) ^ negate for a_name, negate in group):
                     overall.append(content)
                     break  # if any match we use it, and then bail
-    result = "\n".join(overall)
-    return result
+    return "\n".join(overall)
 
 
 def find_envs(value: str) -> Iterator[str]:
     seen = set()
     for factors, _ in expand_factors(value):
         if factors is not None:
             for group in factors:
@@ -58,25 +55,25 @@
                 pass  # when cannot extract factors keep the entire line
             else:
                 content = line[marker_at + 1 :].strip()
         yield factors, content
 
 
 def find_factor_groups(value: str) -> Iterator[list[tuple[str, bool]]]:
-    """transform '{py,!pi}-{a,b},c' to [{'py', 'a'}, {'py', 'b'}, {'pi', 'a'}, {'pi', 'b'}, {'c'}]"""
+    """Transform '{py,!pi}-{a,b},c' to [{'py', 'a'}, {'py', 'b'}, {'pi', 'a'}, {'pi', 'b'}, {'c'}]."""
     for env in expand_env_with_negation(value):
         result = [name_with_negate(f) for f in env.split("-")]
         yield result
 
 
 _FACTOR_RE = re.compile(r"!?[\w._][\w._-]*")
 
 
 def expand_env_with_negation(value: str) -> Iterator[str]:
-    """transform '{py,!pi}-{a,b},c' to ['py-a', 'py-b', '!pi-a', '!pi-b', 'c']"""
+    """Transform '{py,!pi}-{a,b},c' to ['py-a', 'py-b', '!pi-a', '!pi-b', 'c']."""
     for key, group in groupby(re.split(r"((?:{[^}]+})+)|,", value), key=bool):
         if key:
             group_str = "".join(group).strip()
             elements = re.split(r"{([^}]+)}", group_str)
             parts = [[i.strip() for i in elem.split(",")] for elem in elements]
             for variant in product(*parts):
                 variant_str = "".join(variant)
```

### Comparing `tox-4.6.0/src/tox/config/loader/ini/replace.py` & `tox-4.6.1/src/tox/config/loader/ini/replace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-"""
-Apply value substitution (replacement) on tox strings.
-"""
+"""Apply value substitution (replacement) on tox strings."""
 from __future__ import annotations
 
 import logging
 import os
 import re
 import sys
 from configparser import SectionProxy
 from functools import lru_cache
-from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterator, Pattern, Sequence, Union
 
-from tox.config.loader.api import ConfigLoadArgs
 from tox.config.loader.stringify import stringify
-from tox.config.set_env import SetEnv
-from tox.config.sets import ConfigSet
 from tox.execute.request import shell_cmd
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.config.loader.api import ConfigLoadArgs
     from tox.config.loader.ini import IniLoader
     from tox.config.main import Config
+    from tox.config.set_env import SetEnv
+    from tox.config.sets import ConfigSet
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 # split alongside :, unless it's preceded by a single capital letter (Windows drive letter in paths)
 ARG_DELIMITER = ":"
@@ -49,22 +48,23 @@
     """Find all replaceable tokens within value."""
     return MatchExpression.parse_and_split_to_terminator(value)[0][0]
 
 
 def replace(conf: Config, loader: IniLoader, value: str, args: ConfigLoadArgs, depth: int = 0) -> str:
     """Replace all active tokens within value according to the config."""
     if depth > MAX_REPLACE_DEPTH:
-        raise MatchRecursionError(f"Could not expand {value} after recursing {depth} frames")
+        msg = f"Could not expand {value} after recursing {depth} frames"
+        raise MatchRecursionError(msg)
     return Replacer(conf, loader, conf_args=args, depth=depth).join(find_replace_expr(value))
 
 
 class MatchExpression:
     """An expression that is handled specially by the Replacer."""
 
-    def __init__(self, expr: Sequence[MatchArg], term_pos: int | None = None):
+    def __init__(self, expr: Sequence[MatchArg], term_pos: int | None = None) -> None:
         self.expr = expr
         self.term_pos = term_pos
 
     def __repr__(self) -> str:
         return f"MatchExpression(expr={self.expr!r}, term_pos={self.term_pos!r})"
 
     def __eq__(self, other: Any) -> bool:
@@ -143,15 +143,16 @@
                 last_arg.append(expr)
                 continue
             # default case: consume the next character
             last_arg.append(value[pos])
             pos += 1
         else:  # fell out of the loop
             if terminator:
-                raise MatchError(f"{terminator!r} remains unmatched in {value!r}")
+                msg = f"{terminator!r} remains unmatched in {value!r}"
+                raise MatchError(msg)
         args.append(last_arg)
         return [_flatten_string_fragments(a) for a in args], pos
 
 
 def _flatten_string_fragments(seq_of_str_or_other: Sequence[str | Any]) -> Sequence[str | Any]:
     """Join runs of contiguous str values in a sequence; nny non-str items in the sequence are left as-is."""
     result = []
@@ -168,48 +169,44 @@
         result.append("".join(last_str))
     return result
 
 
 class Replacer:
     """Recursively expand MatchExpression against the config and loader."""
 
-    def __init__(self, conf: Config, loader: IniLoader, conf_args: ConfigLoadArgs, depth: int = 0):
+    def __init__(self, conf: Config, loader: IniLoader, conf_args: ConfigLoadArgs, depth: int = 0) -> None:
         self.conf = conf
         self.loader = loader
         self.conf_args = conf_args
         self.depth = depth
 
     def __call__(self, value: MatchArg) -> Sequence[str]:
         return [self._replace_match(me) if isinstance(me, MatchExpression) else str(me) for me in value]
 
     def join(self, value: MatchArg) -> str:
         return "".join(self(value))
 
     def _replace_match(self, value: MatchExpression) -> str:
-        # use a copy of conf_args so any changes from this replacement do NOT
-        # affect adjacent substitutions (#2869)
+        # use a copy of conf_args so any changes from this replacement do NOT, affect adjacent substitutions (#2869)
         conf_args = self.conf_args.copy()
-        of_type, *args = flattened_args = [self.join(arg) for arg in value.expr]
+        flattened_args = [self.join(arg) for arg in value.expr]
+        of_type, *args = flattened_args
         if of_type == "/":
             replace_value: str | None = os.sep
-        elif of_type == "" and args == [""]:
+        elif not of_type and args == [""]:
             replace_value = os.pathsep
         elif of_type == "env":
             replace_value = replace_env(self.conf, args, conf_args)
         elif of_type == "tty":
             replace_value = replace_tty(args)
         elif of_type == "posargs":
             replace_value = replace_pos_args(self.conf, args, conf_args)
         else:
-            replace_value = replace_reference(
-                self.conf,
-                self.loader,
-                ARG_DELIMITER.join(flattened_args),
-                conf_args,
-            )
+            arg_value = ARG_DELIMITER.join(flattened_args)
+            replace_value = replace_reference(self.conf, self.loader, arg_value, conf_args)
         if replace_value is not None:
             needs_expansion = any(isinstance(m, MatchExpression) for m in find_replace_expr(replace_value))
             if needs_expansion:
                 try:
                     return replace(self.conf, self.loader, replace_value, conf_args, self.depth + 1)
                 except MatchRecursionError as err:
                     LOGGER.warning(str(err))
@@ -231,15 +228,20 @@
     (:(?P<default>.*))? # default value
     $
 """,
         re.VERBOSE,
     )
 
 
-def replace_reference(conf: Config, loader: IniLoader, value: str, conf_args: ConfigLoadArgs) -> str | None:
+def replace_reference(  # noqa: PLR0912, C901
+    conf: Config,
+    loader: IniLoader,
+    value: str,
+    conf_args: ConfigLoadArgs,
+) -> str | None:
     # a return value of None indicates could not replace
     pattern = _replace_ref(loader.section.prefix or loader.section.name)
     match = pattern.match(value)
     if match:
         settings = match.groupdict()
 
         key = settings["key"]
@@ -249,20 +251,21 @@
         exception: Exception | None = None
         try:
             for src in _config_value_sources(settings["env"], settings["section"], conf_args.env_name, conf, loader):
                 try:
                     if isinstance(src, SectionProxy):
                         return loader.process_raw(conf, conf_args.env_name, src[key])
                     value = src.load(key, conf_args.chain)
+                except KeyError as exc:  # if fails, keep trying maybe another source can satisfy
+                    exception = exc
+                else:
                     as_str, _ = stringify(value)
                     as_str = as_str.replace("#", r"\#")  # escape comment characters as these will be stripped
                     return as_str
-                except KeyError as exc:  # if fails, keep trying maybe another source can satisfy
-                    exception = exc
-        except Exception as exc:
+        except Exception as exc:  # noqa: BLE001
             exception = exc
         if exception is not None:
             if isinstance(exception, KeyError):  # if the lookup failed replace - else keep
                 default = settings["default"]
                 if default is not None:
                     return default
                 # we cannot raise here as that would mean users could not write factorials: depends = {py39,py38}-{,b}
@@ -275,17 +278,16 @@
     env: str | None,
     section: str | None,
     current_env: str | None,
     conf: Config,
     loader: IniLoader,
 ) -> Iterator[SectionProxy | ConfigSet]:
     # if we have an env name specified take only from there
-    if env is not None:
-        if env in conf:
-            yield conf.get_env(env)
+    if env is not None and env in conf:
+        yield conf.get_env(env)
 
     if section is None:
         # if no section specified perhaps it's an unregistered config:
         # 1. try first from core conf
         yield conf.core
         # 2. and then fallback to our own environment
         if current_env is not None:
@@ -306,50 +308,45 @@
         env_conf = conf.get_env(conf_args.env_name)
         try:
             if env_conf["args_are_paths"]:  # pragma: no branch
                 to_path = env_conf["change_dir"]
         except KeyError:
             pass
     pos_args = conf.pos_args(to_path)
-    if pos_args is None:
-        replace_value = ARG_DELIMITER.join(args)  # if we use the defaults join back remaining args
-    else:
-        replace_value = shell_cmd(pos_args)
-    return replace_value
+    # if we use the defaults join back remaining args else take shell cmd
+    return ARG_DELIMITER.join(args) if pos_args is None else shell_cmd(pos_args)
 
 
 def replace_env(conf: Config, args: list[str], conf_args: ConfigLoadArgs) -> str:
     if not args or not args[0]:
-        raise MatchError("No variable name was supplied in {env} substitution")
+        msg = "No variable name was supplied in {env} substitution"
+        raise MatchError(msg)
     key = args[0]
     new_key = f"env:{key}"
 
     if conf_args.env_name is not None:  # on core no set env support # pragma: no branch
         if new_key not in conf_args.chain:  # check if set env
             conf_args.chain.append(new_key)
             env_conf = conf.get_env(conf_args.env_name)
             set_env: SetEnv = env_conf["set_env"]
             if key in set_env:
                 return set_env.load(key, conf_args)
         elif conf_args.chain[-1] != new_key:  # if there's a chain but only self-refers than use os.environ
             circular = ", ".join(i[4:] for i in conf_args.chain[conf_args.chain.index(new_key) :])
-            raise MatchRecursionError(f"circular chain between set env {circular}")
+            msg = f"circular chain between set env {circular}"
+            raise MatchRecursionError(msg)
 
     if key in os.environ:
         return os.environ[key]
 
     return "" if len(args) == 1 else ARG_DELIMITER.join(args[1:])
 
 
 def replace_tty(args: list[str]) -> str:
-    if sys.stdout.isatty():
-        result = args[0] if len(args) > 0 else ""
-    else:
-        result = args[1] if len(args) > 1 else ""
-    return result
+    return (args[0] if len(args) > 0 else "") if sys.stdout.isatty() else args[1] if len(args) > 1 else ""
 
 
 __all__ = (
     "find_replace_expr",
     "MatchArg",
     "MatchError",
     "MatchExpression",
```

### Comparing `tox-4.6.0/src/tox/config/source/api.py` & `tox-4.6.1/src/tox/config/source/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Sources."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from pathlib import Path
-from typing import Any, Iterator, List
+from typing import TYPE_CHECKING, Any, Iterator, List
 
-from tox.config.loader.api import Loader, OverrideMap
+from tox.config.loader.section import Section
 
-from ..loader.section import Section
-from ..sets import ConfigSet, CoreConfigSet
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.config.loader.api import Loader, OverrideMap
+    from tox.config.sets import ConfigSet, CoreConfigSet
 
 
 class Source(ABC):
-    """
-    Source is able to return a configuration value (for either the core or per environment source).
-    """
+    """Source is able to return a configuration value (for either the core or per environment source)."""
 
     FILENAME = ""
 
     def __init__(self, path: Path) -> None:
         self.path: Path = path  #: the path to the configuration source
         self._section_to_loaders: dict[str, list[Loader[Any]]] = {}
```

### Comparing `tox-4.6.0/src/tox/config/source/discover.py` & `tox-4.6.1/src/tox/config/source/discover.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 import logging
 from itertools import chain
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 from tox.report import HandledError
 
-from .api import Source
 from .legacy_toml import LegacyToml
 from .setup_cfg import SetupCfg
 from .tox_ini import ToxIni
 
+if TYPE_CHECKING:
+    from .api import Source
+
 SOURCE_TYPES: tuple[type[Source], ...] = (ToxIni, SetupCfg, LegacyToml)
 
 
 def discover_source(config_file: Path | None, root_dir: Path | None) -> Source:
     """
     Discover a source for configuration.
 
@@ -32,15 +35,16 @@
             candidate: Path = config_file / src_type.FILENAME
             try:
                 src = src_type(candidate)
                 break
             except ValueError:
                 continue
         if src is None:
-            raise HandledError(f"could not find any config file in {config_file}")
+            msg = f"could not find any config file in {config_file}"
+            raise HandledError(msg)
     else:
         src = _load_exact_source(config_file)
     return src
 
 
 def _locate_source() -> Source | None:
     folder = Path.cwd()
@@ -58,25 +62,25 @@
     # if the filename matches to the letter some config file name do not fallback to other source types
     exact_match = next((s for s in SOURCE_TYPES if config_file.name == s.FILENAME), None)  # pragma: no cover
     for src_type in (exact_match,) if exact_match is not None else SOURCE_TYPES:  # pragma: no branch
         try:
             return src_type(config_file)
         except ValueError:
             pass
-    raise HandledError(f"could not recognize config file {config_file}")
+    msg = f"could not recognize config file {config_file}"
+    raise HandledError(msg)
 
 
 def _create_default_source(root_dir: Path | None) -> Source:
     if root_dir is None:  # if set use that
         empty = Path.cwd()
         for base in chain([empty], empty.parents):
             if (base / "pyproject.toml").exists():
                 empty = base
                 break
     else:  # if not set use where we find pyproject.toml in the tree or cwd
         empty = root_dir
-    logging.warning(f"No {' or '.join(i.FILENAME for i in SOURCE_TYPES)} found, assuming empty tox.ini at {empty}")
-    src = ToxIni(empty / "tox.ini", content="")
-    return src
+    logging.warning("No %s found, assuming empty tox.ini at %s", " or ".join(i.FILENAME for i in SOURCE_TYPES), empty)
+    return ToxIni(empty / "tox.ini", content="")
 
 
 __all__ = ("discover_source",)
```

### Comparing `tox-4.6.0/src/tox/config/source/ini.py` & `tox-4.6.1/src/tox/config/source/ini.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-"""Load """
+"""Load."""
 from __future__ import annotations
 
 from collections import defaultdict
 from configparser import ConfigParser
 from itertools import chain
-from pathlib import Path
-from typing import DefaultDict, Iterable, Iterator
+from typing import TYPE_CHECKING, Iterable, Iterator
 
+from tox.config.loader.ini import IniLoader
 from tox.config.loader.ini.factor import find_envs
+from tox.config.loader.section import Section
 
-from ..loader.api import OverrideMap
-from ..loader.ini import IniLoader
-from ..loader.section import Section
-from ..sets import ConfigSet
 from .api import Source
 from .ini_section import CORE, PKG_ENV_PREFIX, TEST_ENV_PREFIX, IniSection
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.config.loader.api import OverrideMap
+    from tox.config.sets import ConfigSet
+
 
 class IniSource(Source):
-    """Configuration sourced from a ini file (such as tox.ini)"""
+    """Configuration sourced from a ini file (such as tox.ini)."""
 
     CORE_SECTION = CORE
 
     def __init__(self, path: Path, content: str | None = None) -> None:
         super().__init__(path)
         self._parser = ConfigParser(interpolation=None)
         if content is None:
             if not path.exists():
                 raise ValueError
             content = path.read_text()
         self._parser.read_string(content, str(path))
-        self._section_mapping: DefaultDict[str, list[str]] = defaultdict(list)
+        self._section_mapping: defaultdict[str, list[str]] = defaultdict(list)
 
     def transform_section(self, section: Section) -> Section:
         return IniSection(section.prefix, section.name)
 
     def sections(self) -> Iterator[IniSection]:
         for section in self._parser.sections():
             yield IniSection.from_key(section)
```

### Comparing `tox-4.6.0/src/tox/config/source/ini_section.py` & `tox-4.6.1/src/tox/config/source/ini_section.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     @property
     def is_test_env(self) -> bool:
         return self.prefix == TEST_ENV_PREFIX
 
     @property
     def names(self) -> list[str]:
-        elements = list(extend_factors(self.name))
-        return elements
+        return list(extend_factors(self.name))
 
 
 TEST_ENV_PREFIX = "testenv"
 PKG_ENV_PREFIX = "pkgenv"
 CORE = IniSection(None, "tox")
 
 __all__ = [
```

### Comparing `tox-4.6.0/src/tox/config/source/legacy_toml.py` & `tox-4.6.1/src/tox/config/source/legacy_toml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from __future__ import annotations
 
 import sys
-from pathlib import Path
 
 if sys.version_info >= (3, 11):  # pragma: no cover (py311+)
     import tomllib
 else:  # pragma: no cover (py311+)
     import tomli as tomllib
 
 
+from typing import TYPE_CHECKING
+
 from .ini import IniSource
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 class LegacyToml(IniSource):
     FILENAME = "pyproject.toml"
 
-    def __init__(self, path: Path):
+    def __init__(self, path: Path) -> None:
         if path.name != self.FILENAME or not path.exists():
             raise ValueError
         with path.open("rb") as file_handler:
             toml_content = tomllib.load(file_handler)
         try:
             content = toml_content["tool"]["tox"]["legacy_tox_ini"]
-        except KeyError:
-            raise ValueError
+        except KeyError as exc:
+            raise ValueError(path) from exc
         super().__init__(path, content=content)
 
 
 __all__ = ("LegacyToml",)
```

### Comparing `tox-4.6.0/src/tox/execute/api.py` & `tox-4.6.1/src/tox/execute/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-"""
-Abstract base API for executing commands within tox environments.
-"""
+"""Abstract base API for executing commands within tox environments."""
 from __future__ import annotations
 
 import logging
 import sys
 import time
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
-from types import TracebackType
 from typing import TYPE_CHECKING, Any, Callable, Iterator, NoReturn, Sequence, cast
 
 from colorama import Fore
 
-from tox.report import OutErr
-
 from .request import ExecuteRequest, StdinSource
 from .stream import SyncWrite
 
 if TYPE_CHECKING:
+    from types import TracebackType
+
+    from tox.report import OutErr
     from tox.tox_env.api import ToxEnv
 
 ContentHandler = Callable[[bytes], None]
 Executor = Callable[[ExecuteRequest, ContentHandler, ContentHandler], int]
 LOGGER = logging.getLogger(__name__)
 
 
@@ -103,23 +101,29 @@
 
     @property
     def metadata(self) -> dict[str, Any]:
         return {}
 
 
 class Execute(ABC):
-    """Abstract API for execution of a tox environment"""
+    """Abstract API for execution of a tox environment."""
 
     _option_class: type[ExecuteOptions] = ExecuteOptions
 
-    def __init__(self, colored: bool) -> None:
+    def __init__(self, colored: bool) -> None:  # noqa: FBT001
         self._colored = colored
 
     @contextmanager
-    def call(self, request: ExecuteRequest, show: bool, out_err: OutErr, env: ToxEnv) -> Iterator[ExecuteStatus]:
+    def call(
+        self,
+        request: ExecuteRequest,
+        show: bool,  # noqa: FBT001
+        out_err: OutErr,
+        env: ToxEnv,
+    ) -> Iterator[ExecuteStatus]:
         start = time.monotonic()
         try:
             # collector is what forwards the content from the file streams to the standard streams
             out, err = out_err[0].buffer, out_err[1].buffer
             out_sync = SyncWrite(out.name, out if show else None)
             err_sync = SyncWrite(err.name, err if show else None, Fore.RED if self._colored else None)
             with out_sync, err_sync:
@@ -153,15 +157,15 @@
 
     @classmethod
     def register_conf(cls, env: ToxEnv) -> None:
         cls._option_class.register_conf(env)
 
 
 class ExecuteInstance(ABC):
-    """An instance of a command execution"""
+    """An instance of a command execution."""
 
     def __init__(self, request: ExecuteRequest, options: ExecuteOptions, out: SyncWrite, err: SyncWrite) -> None:
         self.request = request
         self.options = options
         self._out = out
         self._err = err
 
@@ -189,30 +193,30 @@
     @property
     @abstractmethod
     def cmd(self) -> Sequence[str]:
         raise NotImplementedError
 
 
 class Outcome:
-    """Result of a command execution"""
+    """Result of a command execution."""
 
     OK = 0
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         request: ExecuteRequest,
-        show_on_standard: bool,
+        show_on_standard: bool,  # noqa: FBT001
         exit_code: int | None,
         out: str,
         err: str,
         start: float,
         end: float,
         cmd: Sequence[str],
         metadata: dict[str, Any],
-    ):
+    ) -> None:
         """
         Create a new execution outcome.
 
         :param request: the execution request
         :param show_on_standard: a flag indicating if the execution was shown on stdout/stderr
         :param exit_code: the exit code for the execution
         :param out: the standard output of the execution
@@ -238,15 +242,15 @@
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}: exit {self.exit_code} in {self.elapsed:.2f} seconds"
             f" for {self.request.shell_cmd}"
         )
 
     def assert_success(self) -> None:
-        """Assert that the execution succeeded"""
+        """Assert that the execution succeeded."""
         if self.exit_code is not None and self.exit_code != self.OK:
             self._assert_fail()
         self.log_run_done(logging.INFO)
 
     def _assert_fail(self) -> NoReturn:
         if self.show_on_standard is False:
             if self.out:
```

### Comparing `tox-4.6.0/src/tox/execute/pep517_backend.py` & `tox-4.6.1/src/tox/execute/pep517_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-"""A executor that reuses a single subprocess for all backend calls (saving on python startup/import overhead)"""
+"""A executor that reuses a single subprocess for all backend calls (saving on python startup/import overhead)."""
 from __future__ import annotations
 
 import time
-from pathlib import Path
 from subprocess import TimeoutExpired
 from threading import Lock
-from types import TracebackType
-from typing import Sequence
+from typing import TYPE_CHECKING, Sequence
 
 from pyproject_api import BackendFailed
 
 from tox.execute import ExecuteRequest
 from tox.execute.api import Execute, ExecuteInstance, ExecuteOptions, ExecuteStatus
 from tox.execute.local_sub_process import LocalSubProcessExecuteInstance
 from tox.execute.request import StdinSource
 from tox.execute.stream import SyncWrite
 
+if TYPE_CHECKING:
+    from pathlib import Path
+    from types import TracebackType
+
 
 class LocalSubProcessPep517Executor(Execute):
-    """Executor holding the backend process"""
+    """Executor holding the backend process."""
 
-    def __init__(self, colored: bool, cmd: Sequence[str], env: dict[str, str], cwd: Path):
+    def __init__(self, colored: bool, cmd: Sequence[str], env: dict[str, str], cwd: Path) -> None:  # noqa: FBT001
         super().__init__(colored)
         self.cmd = cmd
         self.env = env
         self.cwd = cwd
         self._local_execute: tuple[LocalSubProcessExecuteInstance, ExecuteStatus] | None = None
         self._exc: Exception | None = None
         self.is_alive: bool = False
@@ -32,16 +34,15 @@
     def build_instance(
         self,
         request: ExecuteRequest,
         options: ExecuteOptions,
         out: SyncWrite,
         err: SyncWrite,
     ) -> ExecuteInstance:
-        result = LocalSubProcessPep517ExecuteInstance(request, options, out, err, self.local_execute(options))
-        return result
+        return LocalSubProcessPep517ExecuteInstance(request, options, out, err, self.local_execute(options))
 
     def local_execute(self, options: ExecuteOptions) -> tuple[LocalSubProcessExecuteInstance, ExecuteStatus]:
         if self._exc is not None:
             raise self._exc
         if self._local_execute is None:
             request = ExecuteRequest(cmd=self.cmd, cwd=self.cwd, env=self.env, stdin=StdinSource.API, run_id="pep517")
 
@@ -73,41 +74,40 @@
                     self._exc = ToxBackendFailed(failure)
                     raise self._exc
                 time.sleep(0.01)  # wait a short while for the output to populate
         return self._local_execute
 
     @staticmethod
     def _handler(into: bytearray, content: bytes) -> None:
-        """ignore content generated"""
+        """Ignore content generated."""
         into.extend(content)  # pragma: no cover
 
     def close(self) -> None:
         if self._local_execute is not None:  # pragma: no branch
             execute, status = self._local_execute
             execute.__exit__(None, None, None)
-            if execute.process is not None:  # pragma: no branch
-                if execute.process.returncode is None:  # pragma: no cover
-                    try:  # pragma: no cover
-                        execute.process.wait(timeout=0.1)  # pragma: no cover
-                    except TimeoutExpired:  # pragma: no cover
-                        execute.process.terminate()  # pragma: no cover  # if does not stop on its own kill it
+            if execute.process is not None and execute.process.returncode is None:  # pragma: no cover
+                try:  # pragma: no cover
+                    execute.process.wait(timeout=0.1)  # pragma: no cover
+                except TimeoutExpired:  # pragma: no cover
+                    execute.process.terminate()  # pragma: no cover  # if does not stop on its own kill it
         self.is_alive = False
 
 
 class LocalSubProcessPep517ExecuteInstance(ExecuteInstance):
-    """A backend invocation"""
+    """A backend invocation."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         request: ExecuteRequest,
         options: ExecuteOptions,
         out: SyncWrite,
         err: SyncWrite,
         instance_status: tuple[LocalSubProcessExecuteInstance, ExecuteStatus],
-    ):
+    ) -> None:
         super().__init__(request, options, out, err)
         self._instance, self._status = instance_status
         self._lock = Lock()
 
     @property
     def cmd(self) -> Sequence[str]:
         return self._instance.cmd
@@ -115,17 +115,17 @@
     def __enter__(self) -> ExecuteStatus:
         self._lock.acquire()
         self._swap_out_err()
         return self._status
 
     def __exit__(
         self,
-        exc_type: type[BaseException] | None,  # noqa: U100
-        exc_val: BaseException | None,  # noqa: U100
-        exc_tb: TracebackType | None,  # noqa: U100
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         self._swap_out_err()
         self._lock.release()
 
     def _swap_out_err(self) -> None:
         out, err = self._out, self._err
         # update status to see the newly collected content
```

### Comparing `tox-4.6.0/src/tox/execute/request.py` & `tox-4.6.1/src/tox/execute/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     @staticmethod
     def user_only() -> StdinSource:
         """:return: ``USER`` if the standard input is tty type else ``OFF``"""
         return StdinSource.USER if sys.stdin.isatty() else StdinSource.OFF
 
 
 class ExecuteRequest:
-    """Defines a commands execution request"""
+    """Defines a commands execution request."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         cmd: Sequence[str | Path],
         cwd: Path,
         env: dict[str, str],
         stdin: StdinSource,
         run_id: str,
         allow: list[str] | None = None,
@@ -36,15 +36,16 @@
         :param cmd: the command to run
         :param cwd: the current working directory
         :param env: the environment variables
         :param stdin: the type of standard input allowed
         :param run_id: an id to identify this run
         """
         if len(cmd) == 0:
-            raise ValueError("cannot execute an empty command")
+            msg = "cannot execute an empty command"
+            raise ValueError(msg)
         self.cmd: list[str] = [str(i) for i in cmd]  #: the command to run
         self.cwd = cwd  #: the working directory to use
         self.env = env  #: the environment variables to use
         self.stdin = stdin  #: the type of standard input interaction allowed
         self.run_id = run_id  #: an id to identify this run
         if allow is not None and "*" in allow:
             allow = None  # if we allow everything we can just disable the check
@@ -66,18 +67,18 @@
 
 
 def shell_cmd(cmd: Sequence[str]) -> str:
     if sys.platform == "win32":  # pragma: win32 cover
         from subprocess import list2cmdline
 
         return list2cmdline(tuple(str(x) for x in cmd))
-    else:  # pragma: win32 no cover
-        from shlex import quote as shlex_quote
+    # pragma: win32 no cover
+    from shlex import quote as shlex_quote
 
-        return " ".join(shlex_quote(str(x)) for x in cmd)
+    return " ".join(shlex_quote(str(x)) for x in cmd)
 
 
 __all__ = (
     "StdinSource",
     "ExecuteRequest",
     "shell_cmd",
 )
```

### Comparing `tox-4.6.0/src/tox/execute/stream.py` & `tox-4.6.1/src/tox/execute/stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
 from threading import Event, Lock, Timer
-from types import TracebackType
-from typing import IO, Iterator
+from typing import IO, TYPE_CHECKING, Iterator
 
 from colorama import Fore
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
 
 class SyncWrite:
     """
     Make sure data collected is synced in-memory and to the target stream on every newline and time period.
 
     Used to propagate executed commands output to the standard output/error streams visible to the user.
     """
@@ -34,24 +36,24 @@
     def __enter__(self) -> SyncWrite:
         if self._target_enabled:
             self._start()
         return self
 
     def __exit__(
         self,
-        exc_type: type[BaseException] | None,  # noqa: U100
-        exc_val: BaseException | None,  # noqa: U100
-        exc_tb: TracebackType | None,  # noqa: U100
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         if self._target_enabled:
             self._cancel()
             self._write(len(self._content))
 
     def handler(self, content: bytes) -> None:
-        """A callback called whenever content is written"""
+        """A callback called whenever content is written."""
         with self._content_lock:
             self._content.extend(content)
             if self._target_enabled is False:
                 return
             at = content.rfind(b"\n")
             if at != -1:  # pragma: no branch
                 at = len(self._content) - len(content) + at + 1
@@ -72,15 +74,15 @@
 
     def _trigger_timer(self) -> None:
         with self._content_lock:
             at = len(self._content)
         self._write(at)
 
     def _write(self, at: int) -> None:
-        assert self._target is not None  # because _do_print is guarding the call of this method
+        assert self._target is not None  # because _do_print is guarding the call of this method  # noqa: S101
         with self._lock:
             if at > self._at:  # pragma: no branch
                 try:
                     with self.colored():
                         self._target.write(self._content[self._at : at])
                     self._target.flush()
                 finally:
```

### Comparing `tox-4.6.0/src/tox/execute/util.py` & `tox-4.6.1/src/tox/execute/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
+from pathlib import Path
+
 
 def shebang(exe: str) -> list[str] | None:
     """
     :param exe: the executable
     :return: the shebang interpreter arguments
     """
     # When invoking a command using a shebang line that exceeds the OS shebang limit (e.g. Linux has a limit of 128;
     # BINPRM_BUF_SIZE) the invocation will fail. In this case you'd want to replace the shebang invocation with an
     # explicit invocation.
     # see https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git/tree/fs/binfmt_script.c#n34
     try:
-        with open(exe, "rb") as file_handler:
+        with Path(exe).open("rb") as file_handler:
             marker = file_handler.read(2)
             if marker != b"#!":
                 return None
             shebang_line = file_handler.readline()
     except OSError:
         return None
     try:
```

### Comparing `tox-4.6.0/src/tox/execute/local_sub_process/__init__.py` & `tox-4.6.1/src/tox/execute/local_sub_process/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-"""Execute that runs on local file system via subprocess-es"""
+"""Execute that runs on local file system via subprocess-es."""
 from __future__ import annotations
 
 import fnmatch
-import io
 import logging
 import os
 import shutil
 import sys
 from subprocess import DEVNULL, PIPE, TimeoutExpired
-from types import TracebackType
 from typing import TYPE_CHECKING, Any, Generator, Sequence
 
+from tox.execute.api import Execute, ExecuteInstance, ExecuteOptions, ExecuteStatus
+from tox.execute.request import ExecuteRequest, StdinSource
+from tox.execute.util import shebang
 from tox.tox_env.errors import Fail
 
-from ..api import Execute, ExecuteInstance, ExecuteOptions, ExecuteStatus
-from ..request import ExecuteRequest, StdinSource
-from ..stream import SyncWrite
-from ..util import shebang
+if TYPE_CHECKING:
+    import io
+    from types import TracebackType
+
+    from tox.execute.stream import SyncWrite
 
 # mypy: warn-unused-ignores=false
 
 if sys.platform == "win32":  # explicit check for mypy # pragma: win32 cover
     # needs stdin/stdout handlers backed by overlapped IO
     if TYPE_CHECKING:  # the typeshed libraries don't contain this, so replace it with normal one
         from subprocess import Popen
@@ -50,15 +52,15 @@
         out: SyncWrite,
         err: SyncWrite,
     ) -> ExecuteInstance:
         return LocalSubProcessExecuteInstance(request, options, out, err)
 
 
 class LocalSubprocessExecuteStatus(ExecuteStatus):
-    def __init__(self, options: ExecuteOptions, out: SyncWrite, err: SyncWrite, process: Popen[bytes]):
+    def __init__(self, options: ExecuteOptions, out: SyncWrite, err: SyncWrite, process: Popen[bytes]) -> None:
         self._process: Popen[bytes] = process
         super().__init__(options, out, err)
         self._interrupted = False
 
     @property
     def exit_code(self) -> int | None:
         return self._process.returncode
@@ -106,15 +108,16 @@
                 # on Windows we have a PipeHandle object here rather than a file stream
                 import _overlapped  # type: ignore[import]
 
                 ov = _overlapped.Overlapped(0)
                 ov.WriteFile(stdin.handle, bytes_content)  # type: ignore[attr-defined]
                 result = ov.getresult(10)  # wait up to 10ms to perform the operation
                 if result != len(bytes_content):
-                    raise RuntimeError(f"failed to write to {stdin!r}")
+                    msg = f"failed to write to {stdin!r}"
+                    raise RuntimeError(msg)  # noqa: TRY301
             else:
                 stdin.write(bytes_content)
                 stdin.flush()
         except OSError:  # pragma: no cover
             if self._interrupted:  # pragma: no cover
                 pass  # pragma: no cover  # if the process was asked to exit in the meantime ignore write errors
             raise  # pragma: no cover
@@ -132,32 +135,32 @@
         super().__init__(options, out, err)
         self._exit_code = exit_code
 
     @property
     def exit_code(self) -> int | None:
         return self._exit_code
 
-    def wait(self, timeout: float | None = None) -> int | None:  # noqa: U100
+    def wait(self, timeout: float | None = None) -> int | None:  # noqa: ARG002
         return self._exit_code  # pragma: no cover
 
-    def write_stdin(self, content: str) -> None:  # noqa: U100
-        """cannot write"""
+    def write_stdin(self, content: str) -> None:
+        """Cannot write."""
 
     def interrupt(self) -> None:
         return None  # pragma: no cover # nothing running so nothing to interrupt
 
 
 class LocalSubProcessExecuteInstance(ExecuteInstance):
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         request: ExecuteRequest,
         options: ExecuteOptions,
         out: SyncWrite,
         err: SyncWrite,
-        on_exit_drain: bool = True,
+        on_exit_drain: bool = True,  # noqa: FBT001, FBT002
     ) -> None:
         super().__init__(request, options, out, err)
         self.process: Popen[bytes] | None = None
         self._cmd: list[str] | None = None
         self._read_stderr: ReadViaThread | None = None
         self._read_stdout: ReadViaThread | None = None
         self._on_exit_drain = on_exit_drain
@@ -174,15 +177,16 @@
                     for allow in self.request.allow:
                         # 1. allow matches just the original name of the executable
                         # 2. allow matches the entire resolved path
                         if fnmatch.fnmatch(self.request.cmd[0], allow) or fnmatch.fnmatch(executable, allow):
                             break
                     else:
                         msg = f"{base} (resolves to {executable})" if base == executable else base
-                        raise Fail(f"{msg} is not allowed, use allowlist_externals to allow it")
+                        msg = f"{msg} is not allowed, use allowlist_externals to allow it"
+                        raise Fail(msg)
                 cmd = [executable]
                 if sys.platform != "win32" and self.request.env.get("TOX_LIMITED_SHEBANG", "").strip():
                     shebang_line = shebang(executable)
                     if shebang_line:
                         cmd = [*shebang_line, executable]
                 cmd.extend(self.request.cmd[1:])
             self._cmd = cmd
@@ -195,15 +199,15 @@
             self.request.env.setdefault("COLUMNS", str(columns))
         if lines != -1:  # pragma: no branch
             self.request.env.setdefault("LINES", str(lines))
 
         stdout, stderr = self.get_stream_file_no("stdout"), self.get_stream_file_no("stderr")
         try:
             self.process = process = Popen(
-                self.cmd,
+                self.cmd,  # noqa: S603
                 stdout=next(stdout),
                 stderr=next(stderr),
                 stdin={StdinSource.USER: None, StdinSource.OFF: DEVNULL, StdinSource.API: PIPE}[self.request.stdin],
                 cwd=str(self.request.cwd),
                 env=self.request.env,
             )
         except OSError as exception:
@@ -213,16 +217,16 @@
         drain, pid = self._on_exit_drain, self.process.pid
         self._read_stderr = ReadViaThread(stderr.send(process), self.err_handler, name=f"err-{pid}", drain=drain)
         self._read_stderr.__enter__()
         self._read_stdout = ReadViaThread(stdout.send(process), self.out_handler, name=f"out-{pid}", drain=drain)
         self._read_stdout.__enter__()
 
         if sys.platform == "win32":  # explicit check for mypy:  # pragma: win32 cover
-            process.stderr.read = self._read_stderr._drain_stream  # type: ignore[assignment,union-attr]
-            process.stdout.read = self._read_stdout._drain_stream  # type: ignore[assignment,union-attr]
+            process.stderr.read = self._read_stderr._drain_stream  # type: ignore[assignment,union-attr]  # noqa: SLF001
+            process.stdout.read = self._read_stdout._drain_stream  # type: ignore[assignment,union-attr]  # noqa: SLF001
         return status
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
```

### Comparing `tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread.py` & `tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-A reader that drain a stream via its file no on a background thread.
-"""
+"""A reader that drain a stream via its file no on a background thread."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from threading import Event, Thread
-from types import TracebackType
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
+
+if TYPE_CHECKING:
+    from types import TracebackType
 
 WAIT_GENERAL = 0.05  # stop thread join every so often (give chance to a signal interrupt)
 
 
 class ReadViaThread(ABC):
-    def __init__(self, file_no: int, handler: Callable[[bytes], None], name: str, drain: bool) -> None:
+    def __init__(self, file_no: int, handler: Callable[[bytes], None], name: str, drain: bool) -> None:  # noqa: FBT001
         self.file_no = file_no
         self.stop = Event()
         self.thread = Thread(target=self._read_stream, name=f"tox-r-{name}-{file_no}")
         self.handler = handler
         self._on_exit_drain = drain
 
     def __enter__(self) -> ReadViaThread:
         self.thread.start()
         return self
 
     def __exit__(
         self,
-        exc_type: type[BaseException] | None,  # noqa: U100
-        exc_val: BaseException | None,  # noqa: U100
-        exc_tb: TracebackType | None,  # noqa: U100
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         self.stop.set()  # signal thread to stop
         while self.thread.is_alive():  # wait until it stops
             self.thread.join(WAIT_GENERAL)
         self._drain_stream()  # read anything left
 
     @abstractmethod
```

### Comparing `tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread_unix.py` & `tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread_unix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-"""
-On UNIX we use select.select to ensure we drain in a non-blocking fashion.
-"""
+"""On UNIX we use select.select to ensure we drain in a non-blocking fashion."""
 from __future__ import annotations
 
 import errno  # pragma: win32 no cover
 import os  # pragma: win32 no cover
 import select  # pragma: win32 no cover
 from typing import Callable
 
 from .read_via_thread import ReadViaThread  # pragma: win32 no cover
 
 STOP_EVENT_CHECK_PERIODICITY_IN_MS = 0.01  # pragma: win32 no cover
 
 
 class ReadViaThreadUnix(ReadViaThread):  # pragma: win32 no cover
-    def __init__(self, file_no: int, handler: Callable[[bytes], None], name: str, drain: bool) -> None:
+    def __init__(self, file_no: int, handler: Callable[[bytes], None], name: str, drain: bool) -> None:  # noqa: FBT001
         super().__init__(file_no, handler, name, drain)
 
     def _read_stream(self) -> None:
         while not self.stop.is_set():
             # we need to drain the stream, but periodically give chance for the thread to break if the stop event has
             # been set (this is so that an interrupt can be handled)
             if self._read_available() is None:  # pragma: no branch
@@ -35,13 +33,14 @@
             ready, __, ___ = select.select([self.file_no], [], [], timeout)
             if ready:
                 data = os.read(self.file_no, 1024)  # read up to 1024 characters
                 # If the end of the file referred to by fd has been reached, an empty bytes object is returned.
                 if data:
                     self.handler(data)
                     return True
-            return False
         except OSError as exception:  # pragma: no cover
             # Bad file descriptor or Input/output error
             if exception.errno in (errno.EBADF, errno.EIO):
                 return None
             raise
+        else:
+            return False
```

### Comparing `tox-4.6.0/src/tox/execute/local_sub_process/read_via_thread_windows.py` & `tox-4.6.1/src/tox/execute/local_sub_process/read_via_thread_windows.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-"""
-On Windows we use overlapped mechanism, borrowing it from asyncio (but without the event loop).
-"""
+"""On Windows we use overlapped mechanism, borrowing it from asyncio (but without the event loop)."""
 from __future__ import annotations  # pragma: win32 cover
 
 import logging  # pragma: win32 cover
-from asyncio.windows_utils import BUFSIZE  # type: ignore # pragma: win32 cover
+from asyncio.windows_utils import BUFSIZE  # type: ignore[attr-defined] # pragma: win32 cover
 from time import sleep  # pragma: win32 cover
 from typing import Callable  # pragma: win32 cover
 
 import _overlapped  # type: ignore[import]  # pragma: win32 cover
 
 from .read_via_thread import ReadViaThread  # pragma: win32 cover
 
 # mypy: warn-unused-ignores=false
 
 
 class ReadViaThreadWindows(ReadViaThread):  # pragma: win32 cover
-    def __init__(self, file_no: int, handler: Callable[[bytes], None], name: str, drain: bool) -> None:
+    def __init__(self, file_no: int, handler: Callable[[bytes], None], name: str, drain: bool) -> None:  # noqa: FBT001
         super().__init__(file_no, handler, name, drain)
         self.closed = False
         self._ov: _overlapped.Overlapped | None = None
         self._waiting_for_read = False
 
     def _read_stream(self) -> None:
         keep_reading = True
@@ -44,25 +42,24 @@
             try:  # read up to BUFSIZE at a time
                 self._ov.ReadFile(self.file_no, BUFSIZE)  # type: ignore[attr-defined]
                 self._waiting_for_read = True
             except OSError:
                 self.closed = True
                 return None
         try:  # wait=False to not block and give chance for the stop check
-            data = self._ov.getresult(False)  # type: ignore[union-attr]
+            data = self._ov.getresult(False)  # type: ignore[union-attr]  # noqa: FBT003
         except OSError as exception:
             # 996 (0x3E4) Overlapped I/O event is not in a signaled state.
             # 995 (0x3E3) The I/O operation has been aborted because of either a thread exit or an application request.
             win_error = getattr(exception, "winerror", None)
-            if win_error == 996:
+            if win_error == 996:  # noqa: PLR2004
                 return True
-            else:
-                if win_error != 995:
-                    logging.error("failed to read %r", exception)
-                return None
+            if win_error != 995:  # noqa: PLR2004
+                logging.error("failed to read %r", exception)  # noqa: TRY400
+            return None
         else:
             self._ov = None
             self._waiting_for_read = False
             if data:
                 self.handler(data)
             else:
                 return None
```

### Comparing `tox-4.6.0/src/tox/journal/env.py` & `tox-4.6.1/src/tox/journal/env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""Record information about tox environments"""
+"""Record information about tox environments."""
 from __future__ import annotations
 
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-from tox.execute import Outcome
+if TYPE_CHECKING:
+    from tox.execute import Outcome
 
 
 class EnvJournal:
-    """Report the status of a tox environment"""
+    """Report the status of a tox environment."""
 
-    def __init__(self, enabled: bool, name: str) -> None:
+    def __init__(self, enabled: bool, name: str) -> None:  # noqa: FBT001
         self._enabled = enabled
         self.name = name
         self._content: dict[str, Any] = {}
         self._executes: list[tuple[str, Outcome]] = []
 
     def __setitem__(self, key: str, value: Any) -> None:
         """
@@ -50,15 +51,15 @@
                 "retcode": outcome.exit_code,
                 "elapsed": outcome.elapsed,
                 "show_on_standard": outcome.show_on_standard,
                 "run_id": run_id,
                 "start": outcome.start,
                 "end": outcome.end,
             }
-            if run_id.startswith("commands") or run_id.startswith("build"):
+            if run_id.startswith(("commands", "build")):
                 tests.append(one)
             else:
                 setup.append(one)
         if tests:
             self["test"] = tests
         if setup:
             self["setup"] = setup
```

### Comparing `tox-4.6.0/src/tox/journal/main.py` & `tox-4.6.1/src/tox/journal/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""Generate json report of a tox run"""
+"""Generate json report of a tox run."""
 from __future__ import annotations
 
 import socket
 import sys
 from typing import Any
 
 from tox.version import version
 
 from .env import EnvJournal
 
 
 class Journal:
-    """The result of a tox session"""
+    """The result of a tox session."""
 
-    def __init__(self, enabled: bool) -> None:
+    def __init__(self, enabled: bool) -> None:  # noqa: FBT001
         self._enabled = enabled
         self._content: dict[str, Any] = {}
         self._env: dict[str, EnvJournal] = {}
 
         if self._enabled:
             self._content.update(
                 {
@@ -25,15 +25,15 @@
                     "toxversion": version,
                     "platform": sys.platform,
                     "host": socket.getfqdn(),
                 },
             )
 
     def get_env_journal(self, name: str) -> EnvJournal:
-        """Return the env log of an environment (create on first call)"""
+        """Return the env log of an environment (create on first call)."""
         if name not in self._env:
             env = EnvJournal(self._enabled, name)
             self._env[name] = env
         return self._env[name]
 
     @property
     def content(self) -> dict[str, Any]:
```

### Comparing `tox-4.6.0/src/tox/plugin/__init__.py` & `tox-4.6.1/src/tox/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/src/tox/plugin/inline.py` & `tox-4.6.1/src/tox/plugin/inline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
 import importlib
 import sys
-from pathlib import Path
-from types import ModuleType
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from pathlib import Path
+    from types import ModuleType
 
 
 def load_inline(path: Path) -> ModuleType | None:
     # nox uses here the importlib.machinery.SourceFileLoader but I consider this similarly good, and we can keep any
     # name for the tox file, its content will always be loaded in this module from a system point of view
     for name in ("toxfile", "☣"):
         candidate = path.parent / f"{name}.py"
```

### Comparing `tox-4.6.0/src/tox/plugin/manager.py` & `tox-4.6.1/src/tox/plugin/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-"""Contains the plugin manager object"""
+"""Contains the plugin manager object."""
 from __future__ import annotations
 
-from pathlib import Path
-from types import ModuleType
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import pluggy
 
 from tox import provision
-from tox.config.cli.parser import ToxParser
 from tox.config.loader import api as loader_api
-from tox.config.sets import ConfigSet, EnvConfigSet
 from tox.session.cmd.run import parallel, sequential
 from tox.tox_env import package as package_api
 from tox.tox_env.python.virtual_env import runner
 from tox.tox_env.python.virtual_env.package import cmd_builder, pyproject
 from tox.tox_env.register import REGISTER, ToxEnvRegister
 
-from ..execute import Outcome
-from ..session.state import State
-from ..tox_env.api import ToxEnv
 from . import NAME, spec
 from .inline import load_inline
 
+if TYPE_CHECKING:
+    from pathlib import Path
+    from types import ModuleType
+
+    from tox.config.cli.parser import ToxParser
+    from tox.config.sets import ConfigSet, EnvConfigSet
+    from tox.execute import Outcome
+    from tox.session.state import State
+    from tox.tox_env.api import ToxEnv
+
 
 class Plugin:
     def __init__(self) -> None:
         self.manager: pluggy.PluginManager = pluggy.PluginManager(NAME)
         self.manager.add_hookspecs(spec)
 
     def _register_plugins(self, inline: ModuleType | None) -> None:
@@ -84,15 +87,15 @@
         self.manager.hook.tox_env_teardown(tox_env=tox_env)
 
     def load_plugins(self, path: Path) -> None:
         for _plugin in self.manager.get_plugins():  # make sure we start with a clean state, repeated in memory run
             self.manager.unregister(_plugin)
         inline = _load_inline(path)
         self._register_plugins(inline)
-        REGISTER._register_tox_env_types(self)
+        REGISTER._register_tox_env_types(self)  # noqa: SLF001
 
 
 def _load_inline(path: Path) -> ModuleType | None:  # used to be able to unregister plugin tests
     return load_inline(path)
 
 
 MANAGER = Plugin()
```

### Comparing `tox-4.6.0/src/tox/plugin/spec.py` & `tox-4.6.1/src/tox/plugin/spec.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,106 +1,107 @@
 from __future__ import annotations
 
-from typing import Any, Callable, TypeVar, cast
+from typing import TYPE_CHECKING, Any, Callable, TypeVar, cast
 
 import pluggy
 
-from tox.config.sets import ConfigSet, EnvConfigSet
-from tox.tox_env.register import ToxEnvRegister
-
-from ..config.cli.parser import ToxParser
-from ..execute import Outcome
-from ..session.state import State
-from ..tox_env.api import ToxEnv
 from . import NAME
 
+if TYPE_CHECKING:
+    from tox.config.cli.parser import ToxParser
+    from tox.config.sets import ConfigSet, EnvConfigSet
+    from tox.execute import Outcome
+    from tox.session.state import State
+    from tox.tox_env.api import ToxEnv
+    from tox.tox_env.register import ToxEnvRegister
+
 _F = TypeVar("_F", bound=Callable[..., Any])
 _spec_marker = pluggy.HookspecMarker(NAME)
 
 
 def _spec(func: _F) -> _F:
     return cast(_F, _spec_marker(func))
 
 
 @_spec
-def tox_register_tox_env(register: ToxEnvRegister) -> None:  # noqa: U100
+def tox_register_tox_env(register: ToxEnvRegister) -> None:  # noqa: ARG001
     """
     Register new tox environment type. You can register:
 
     - **run environment**: by default this is a local subprocess backed virtualenv Python
     - **packaging environment**: by default this is a PEP-517 compliant local subprocess backed virtualenv Python
 
     :param register: a object that can be used to register new tox environment types
     """
 
 
 @_spec
-def tox_add_option(parser: ToxParser) -> None:  # noqa: U100
+def tox_add_option(parser: ToxParser) -> None:  # noqa: ARG001
     """
     Add a command line argument. This is the first hook to be called, right after the logging setup and config source
     discovery.
 
     :param parser: the command line parser
     """
 
 
 @_spec
-def tox_add_core_config(core_conf: ConfigSet, state: State) -> None:  # noqa: U100
+def tox_add_core_config(core_conf: ConfigSet, state: State) -> None:  # noqa: ARG001
     """
     Called when the core configuration is built for a tox environment.
 
     :param core_conf: the core configuration object
     :param state: the global tox state object
     """
 
 
 @_spec
-def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:  # noqa: U100
+def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:  # noqa: ARG001
     """
     Called when configuration is built for a tox environment.
 
     :param env_conf: the core configuration object
     :param state: the global tox state object
     """
 
 
 @_spec
-def tox_before_run_commands(tox_env: ToxEnv) -> None:  # noqa: U100
+def tox_before_run_commands(tox_env: ToxEnv) -> None:  # noqa: ARG001
     """
     Called before the commands set is executed.
 
     :param tox_env: the tox environment being executed
     """
 
 
 @_spec
-def tox_after_run_commands(tox_env: ToxEnv, exit_code: int, outcomes: list[Outcome]) -> None:  # noqa: U100
+def tox_after_run_commands(tox_env: ToxEnv, exit_code: int, outcomes: list[Outcome]) -> None:  # noqa: ARG001
     """
     Called after the commands set is executed.
 
     :param tox_env: the tox environment being executed
     :param exit_code: exit code of the command
     :param outcomes: outcome of each command execution
     """
 
 
 @_spec
-def tox_on_install(tox_env: ToxEnv, arguments: Any, section: str, of_type: str) -> None:  # noqa: U100
+def tox_on_install(tox_env: ToxEnv, arguments: Any, section: str, of_type: str) -> None:  # noqa: ARG001
     """
     Called before executing an installation command.
 
     :param tox_env: the tox environment where the command runs in
     :param arguments: installation arguments
     :param section: section of the installation
     :param of_type: type of the installation
     """
 
 
 @_spec
-def tox_env_teardown(tox_env: ToxEnv) -> None:  # noqa: U100
+def tox_env_teardown(tox_env: ToxEnv) -> None:  # noqa: ARG001
     """
     Called before executing an installation command.
 
     :param tox_env: the tox environment
     """
```

### Comparing `tox-4.6.0/src/tox/session/env_select.py` & `tox-4.6.1/src/tox/session/env_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from __future__ import annotations
 
 import logging
 import re
-from argparse import ArgumentParser
 from collections import Counter
 from dataclasses import dataclass
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Dict, Iterable, Iterator, List, cast
 
 from tox.config.loader.str_convert import StrConvert
+from tox.config.types import EnvList
+from tox.report import HandledError
 from tox.tox_env.api import ToxEnvCreateArgs
+from tox.tox_env.errors import Skip
+from tox.tox_env.package import PackageToxEnv
 from tox.tox_env.register import REGISTER
 from tox.tox_env.runner import RunToxEnv
 
-from ..config.types import EnvList
-from ..report import HandledError
-from ..tox_env.errors import Skip
-from ..tox_env.package import PackageToxEnv
-
 if TYPE_CHECKING:
+    from argparse import ArgumentParser
+
     from tox.session.state import State
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class CliEnv:
-    """CLI tox env selection"""
+    """CLI tox env selection."""
 
-    def __init__(self, value: None | list[str] | str = None):
+    def __init__(self, value: None | list[str] | str = None) -> None:
         if isinstance(value, str):
             value = StrConvert().to(value, of_type=List[str], factory=None)
         self._names: list[str] | None = value
 
     def __iter__(self) -> Iterator[str]:
         if not self.is_all and self._names is not None:  # pragma: no branch
             yield from self._names
@@ -43,15 +43,15 @@
     def __str__(self) -> str:
         return "ALL" if self.is_all else ("<env_list>" if self.is_default_list else ",".join(self))
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({'' if self.is_default_list else repr(str(self))})"
 
     def __eq__(self, other: Any) -> bool:
-        return type(self) == type(other) and self._names == other._names
+        return type(self) == type(other) and self._names == other._names  # noqa: SLF001
 
     def __ne__(self, other: Any) -> bool:
         return not (self == other)
 
     @property
     def is_all(self) -> bool:
         return self._names is not None and "ALL" in self._names
@@ -60,29 +60,29 @@
     def is_default_list(self) -> bool:
         return not (self._names or [])
 
 
 def register_env_select_flags(
     parser: ArgumentParser,
     default: CliEnv | None,
-    multiple: bool = True,
-    group_only: bool = False,
+    multiple: bool = True,  # noqa: FBT001, FBT002
+    group_only: bool = False,  # noqa: FBT001, FBT002
 ) -> ArgumentParser:
     """
     Register environment selection flags.
 
     :param parser: the parser to register to
     :param default: the default value for env selection
     :param multiple: allow selecting multiple environments
     :param group_only:
     :return:
     """
     if multiple:
         group = parser.add_argument_group("select target environment(s)")
-        add_to: ArgumentParser = group.add_mutually_exclusive_group(required=False)  # type: ignore
+        add_to: ArgumentParser = group.add_mutually_exclusive_group(required=False)  # type: ignore[assignment]
     else:
         add_to = parser
     if not group_only:
         if multiple:
             help_msg = "enumerate (ALL -> all environments, not set -> use <env_list> from config)"
         else:
             help_msg = "environment to run"
@@ -106,15 +106,15 @@
     help_msg = "exclude all environments selected that match this regular expression"
     add_to.add_argument("--skip-env", dest="skip_env", metavar="re", help=help_msg, default="", type=str)
     return add_to
 
 
 @dataclass
 class _ToxEnvInfo:
-    """tox environment information"""
+    """tox environment information."""
 
     env: PackageToxEnv | RunToxEnv  #: the tox environment
     is_active: bool  #: a flag indicating if the environment is marked as active in the current run
     package_skip: tuple[str, Skip] | None = None  #: if set the creation of the packaging environment failed
 
 
 class EnvSelector:
@@ -126,16 +126,16 @@
         self._warned_about: set[str] = set()  #: shared set of skipped environments that were already warned about
         self._state = state
         self._defined_envs_: None | dict[str, _ToxEnvInfo] = None
         self._pkg_env_counter: Counter[str] = Counter()
         from tox.plugin.manager import MANAGER
 
         self._manager = MANAGER
-        self._log_handler = self._state._options.log_handler
-        self._journal = self._state._journal
+        self._log_handler = self._state._options.log_handler  # noqa: SLF001
+        self._journal = self._state._journal  # noqa: SLF001
         self._provision: None | tuple[bool, str] = None
 
         self._state.conf.core.add_config("labels", Dict[str, EnvList], {}, "core labels")
         tox_env_filter_regex = getattr(state.conf.options, "skip_env", "").strip()
         self._filter_re = re.compile(tox_env_filter_regex) if tox_env_filter_regex else None
 
     @property
@@ -161,22 +161,25 @@
     def _env_name_to_active(self) -> dict[str, bool]:
         env_name_to_active_map = {}
         for a_collection, is_active in self._collect_names():
             for name in a_collection:
                 if name not in env_name_to_active_map:
                     env_name_to_active_map[name] = is_active
         # for factor/label selection update the active flag
-        if not (getattr(self._state.conf.options, "labels", []) or getattr(self._state.conf.options, "factors", [])):
+        if (
+            not (getattr(self._state.conf.options, "labels", []) or getattr(self._state.conf.options, "factors", []))
             # if no active environment is defined fallback to py
-            if self.on_empty_fallback_py and not any(env_name_to_active_map.values()):
-                env_name_to_active_map["py"] = True
+            and self.on_empty_fallback_py
+            and not any(env_name_to_active_map.values())
+        ):
+            env_name_to_active_map["py"] = True
         return env_name_to_active_map
 
     @property
-    def _defined_envs(self) -> dict[str, _ToxEnvInfo]:
+    def _defined_envs(self) -> dict[str, _ToxEnvInfo]:  # noqa: C901, PLR0912
         # The problem of classifying run/package environments:
         # There can be two type of tox environments: run or package. Given a tox environment name there's no easy way to
         # find out which it is.  Intuitively a run environment is any environment that's not used for packaging by
         # another run environment. To find out what are the packaging environments for a run environment you have to
         # first construct it. This implies a two phase solution: construct all environments and query their packaging
         # environments. The run environments are the ones not marked as of packaging type. This requires being able
         # to change tox environments type, if it was earlier discovered as a run environment and is marked as packaging
@@ -198,15 +201,15 @@
                     pkg_name_type = run_env.get_package_env_types()
                 if pkg_name_type is not None:
                     # build package env and assign it, then register the run environment which can trigger generation
                     # of additional run environments
                     start_package_env_use_counter = self._pkg_env_counter.copy()
                     try:
                         run_env.package_env = self._build_pkg_env(pkg_name_type, name, env_name_to_active)
-                    except Exception as exception:
+                    except Exception as exception:  # noqa: BLE001
                         # if it's not a run environment,  wait to see if ends up being a packaging one -> rollback
                         failed[name] = exception
                         for key in self._pkg_env_counter - start_package_env_use_counter:
                             del self._defined_envs_[key]
                             self._state.conf.clear_env(key)
                         self._pkg_env_counter = start_package_env_use_counter
                         del self._defined_envs_[name]
@@ -216,16 +219,16 @@
                             for env in run_env.package_envs:
                                 # check if any packaging envs are already run and remove them
                                 other_env_info = self._defined_envs_.get(env.name)
                                 if other_env_info is not None and isinstance(other_env_info.env, RunToxEnv):
                                     del self._defined_envs_[env.name]  # pragma: no cover
                                     for _pkg_env in other_env_info.env.package_envs:  # pragma: no cover
                                         self._pkg_env_counter[_pkg_env.name] -= 1  # pragma: no cover
-                        except Exception:
-                            assert self._defined_envs_[name].package_skip is not None
+                        except Exception:  # noqa: BLE001
+                            assert self._defined_envs_[name].package_skip is not None  # noqa: S101
             failed_to_create = failed.keys() - self._defined_envs_.keys()
             if failed_to_create:
                 raise failed[next(iter(failed_to_create))]
             for name, count in self._pkg_env_counter.items():
                 if not count:
                     self._defined_envs_.pop(name)  # pragma: no cover
 
@@ -233,15 +236,15 @@
             order = chain(env_name_to_active, (i for i in self._defined_envs_ if i not in env_name_to_active))
             self._defined_envs_ = {name: self._defined_envs_[name] for name in order if name in self._defined_envs_}
             self._finalize_config()
             self._mark_active()
         return self._defined_envs_
 
     def _finalize_config(self) -> None:
-        assert self._defined_envs_ is not None
+        assert self._defined_envs_ is not None  # noqa: S101
         for tox_env in self._defined_envs_.values():
             tox_env.env.conf.mark_finalized()
         self._state.conf.core.mark_finalized()
 
     def _build_run_env(self, name: str) -> RunToxEnv | None:
         if self._provision is not None and self._provision[0] is False and name == self._provision[1]:
             # ignore provision env unless this is a provision run
@@ -259,45 +262,45 @@
         self._manager.tox_add_env_config(env_conf, self._state)
         return run_env
 
     def _build_pkg_env(self, name_type: tuple[str, str], run_env_name: str, active: dict[str, bool]) -> PackageToxEnv:
         name, core_type = name_type
         with self._log_handler.with_context(name):
             if run_env_name == name:
-                raise HandledError(f"{run_env_name} cannot self-package")
+                msg = f"{run_env_name} cannot self-package"
+                raise HandledError(msg)
             missing_active = self._cli_envs is not None and self._cli_envs.is_all
             try:
                 package_tox_env = self._get_package_env(core_type, name, active.get(name, missing_active))
                 self._pkg_env_counter[name] += 1
-                run_env: RunToxEnv = self._defined_envs_[run_env_name].env  # type: ignore
+                run_env: RunToxEnv = self._defined_envs_[run_env_name].env  # type: ignore[index,assignment]
                 child_package_envs = package_tox_env.register_run_env(run_env)
                 try:
                     name_type = next(child_package_envs)
                     while True:
                         child_pkg_env = self._build_pkg_env(name_type, run_env_name, active)
                         self._pkg_env_counter[name_type[0]] += 1
                         name_type = child_package_envs.send(child_pkg_env)
                 except StopIteration:
                     pass
             except Skip as exception:
-                assert self._defined_envs_ is not None
+                assert self._defined_envs_ is not None  # noqa: S101
                 self._defined_envs_[run_env_name].package_skip = (name_type[0], exception)
             return package_tox_env
 
-    def _get_package_env(self, packager: str, name: str, is_active: bool) -> PackageToxEnv:
-        assert self._defined_envs_ is not None
+    def _get_package_env(self, packager: str, name: str, is_active: bool) -> PackageToxEnv:  # noqa: FBT001
+        assert self._defined_envs_ is not None  # noqa: S101
         if name in self._defined_envs_:
             env = self._defined_envs_[name].env
             if isinstance(env, PackageToxEnv):
                 if env.id() != packager:  # pragma: no branch # same env name is used by different packaging
                     msg = f"{name} is already defined as a {env.id()}, cannot be {packager} too"  # pragma: no cover
                     raise HandledError(msg)  # pragma: no cover
                 return env
-            else:
-                self._state.conf.clear_env(name)
+            self._state.conf.clear_env(name)
         package_type = REGISTER.package(packager)
         pkg_conf = self._state.conf.get_env(name, package=True)
         journal = self._journal.get_env_journal(name)
         args = ToxEnvCreateArgs(pkg_conf, self._state.conf.core, self._state.conf.options, journal, self._log_handler)
         pkg_env: PackageToxEnv = package_type(args)
         self._defined_envs_[name] = _ToxEnvInfo(pkg_env, is_active)
         self._manager.tox_add_env_config(pkg_conf, self._state)
@@ -306,19 +309,19 @@
     def _parse_factors(self) -> tuple[set[str], ...]:
         # factors is a list of lists, from the combination of nargs="+" and action="append"
         # also parse hyphenated factors into lists of factors
         # so that `-f foo-bar` and `-f foo bar` are treated equivalently
         raw_factors = getattr(self._state.conf.options, "factors", [])
         return tuple({f for factor in factor_list for f in factor.split("-")} for factor_list in raw_factors)
 
-    def _mark_active(self) -> None:
+    def _mark_active(self) -> None:  # noqa: C901
         labels = set(getattr(self._state.conf.options, "labels", []))
         factors = self._parse_factors()
 
-        assert self._defined_envs_ is not None
+        assert self._defined_envs_ is not None  # noqa: S101
         if labels or factors:
             for env_info in self._defined_envs_.values():
                 env_info.is_active = False  # if any was selected reset
             # ignore labels when provisioning will occur
             if labels and (self._provision is None or not self._provision[0]):
                 for label in labels:
                     for env_name in self._state.conf.core["labels"].get(label, []):
@@ -336,15 +339,15 @@
     def __getitem__(self, item: str) -> RunToxEnv | PackageToxEnv:
         """
         :param item: the name of the environment
         :return: the tox environment
         """
         return self._defined_envs[item].env
 
-    def iter(
+    def iter(  # noqa: A003
         self,
         *,
         only_active: bool = True,
         package: bool = False,
     ) -> Iterator[str]:
         """
         Get tox environments.
@@ -366,17 +369,18 @@
                 continue
             yield name
 
     def ensure_only_run_env_is_active(self) -> None:
         envs, active = self._defined_envs, self._env_name_to_active()
         invalid = [n for n, a in active.items() if a and isinstance(envs[n].env, PackageToxEnv)]
         if invalid:
-            raise HandledError(f"cannot run packaging environment(s) {','.join(invalid)}")
+            msg = f"cannot run packaging environment(s) {','.join(invalid)}"
+            raise HandledError(msg)
 
-    def _mark_provision(self, on: bool, provision_tox_env: str) -> None:
+    def _mark_provision(self, on: bool, provision_tox_env: str) -> None:  # noqa: FBT001
         self._provision = on, provision_tox_env
 
 
 __all__ = [
     "register_env_select_flags",
     "EnvSelector",
     "CliEnv",
```

### Comparing `tox-4.6.0/src/tox/session/state.py` & `tox-4.6.1/src/tox/session/state.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/src/tox/session/cmd/depends.py` & `tox-4.6.1/src/tox/session/cmd/depends.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
-from typing import cast
+from typing import TYPE_CHECKING, cast
 
-from tox.config.cli.parser import ToxParser
 from tox.plugin import impl
 from tox.session.cmd.run.common import env_run_create_flags, run_order
-from tox.session.state import State
 from tox.tox_env.runner import RunToxEnv
 
+if TYPE_CHECKING:
+    from tox.config.cli.parser import ToxParser
+    from tox.session.state import State
+
 
 @impl
 def tox_add_option(parser: ToxParser) -> None:
     our = parser.add_command(
         "depends",
         ["de"],
         "visualize tox environment dependencies",
@@ -19,33 +21,33 @@
     )
     env_run_create_flags(our, mode="depends")
 
 
 def depends(state: State) -> int:
     to_run_list = list(state.envs.iter(only_active=False))
     order, todo = run_order(state, to_run_list)
-    print(f"Execution order: {', '.join(order)}")
+    print(f"Execution order: {', '.join(order)}")  # noqa: T201
 
     deps: dict[str, list[str]] = {k: [o for o in order if o in v] for k, v in todo.items()}
     deps["ALL"] = to_run_list
 
     def _handle(at: int, env: str) -> None:
-        print("   " * at, end="")
-        print(env, end="")
+        print("   " * at, end="")  # noqa: T201
+        print(env, end="")  # noqa: T201
         if env != "ALL":
             run_env = cast(RunToxEnv, state.envs[env])
             packager_list: list[str] = []
             try:
                 for pkg_env in run_env.package_envs:
                     packager_list.append(pkg_env.name)
-            except Exception as exception:
+            except Exception as exception:  # noqa: BLE001
                 packager_list.append(f"... ({exception})")
             names = " | ".join(packager_list)
             if names:
-                print(f" ~ {names}", end="")
-        print("")
+                print(f" ~ {names}", end="")  # noqa: T201
+        print("")  # noqa: T201
         at += 1
         for dep in deps[env]:
             _handle(at, dep)
 
     _handle(0, "ALL")
     return 0
```

### Comparing `tox-4.6.0/src/tox/session/cmd/devenv.py` & `tox-4.6.1/src/tox/session/cmd/devenv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 import logging
 from pathlib import Path
+from typing import TYPE_CHECKING
 
-from tox.config.cli.parser import ToxParser
 from tox.config.loader.memory import MemoryLoader
 from tox.plugin import impl
 from tox.report import HandledError
 from tox.session.cmd.run.common import env_run_create_flags
 from tox.session.cmd.run.sequential import run_sequential
 from tox.session.env_select import CliEnv, register_env_select_flags
-from tox.session.state import State
+
+if TYPE_CHECKING:
+    from tox.config.cli.parser import ToxParser
+    from tox.session.state import State
 
 
 @impl
 def tox_add_option(parser: ToxParser) -> None:
     help_msg = "sets up a development environment at ENVDIR based on the tox configuration specified "
     our = parser.add_command("devenv", ["d"], help_msg, devenv)
     our.add_argument("devenv_path", metavar="path", default=Path("venv"), nargs="?", type=Path)
@@ -36,12 +39,13 @@
         env_dir=opt.devenv_path,  # move it in source
     )
     state.conf.memory_seed_loaders[list(opt.env)[0]].append(loader)
 
     state.envs.ensure_only_run_env_is_active()
     envs = list(state.envs.iter())
     if len(envs) != 1:
-        raise HandledError(f"exactly one target environment allowed in devenv mode but found {', '.join(envs)}")
+        msg = f"exactly one target environment allowed in devenv mode but found {', '.join(envs)}"
+        raise HandledError(msg)
     result = run_sequential(state)
     if result == 0:
-        logging.warning(f"created development environment under {opt.devenv_path}")
+        logging.warning("created development environment under %s", opt.devenv_path)
     return result
```

### Comparing `tox-4.6.0/src/tox/session/cmd/exec_.py` & `tox-4.6.1/src/tox/session/cmd/exec_.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-"""
-Execute a command in a tox environment.
-"""
+"""Execute a command in a tox environment."""
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
-from tox.config.cli.parser import ToxParser
 from tox.config.loader.memory import MemoryLoader
 from tox.config.types import Command
 from tox.plugin import impl
 from tox.report import HandledError
 from tox.session.cmd.run.common import env_run_create_flags
 from tox.session.cmd.run.sequential import run_sequential
 from tox.session.env_select import CliEnv, register_env_select_flags
-from tox.session.state import State
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.config.cli.parser import ToxParser
+    from tox.session.state import State
 
 
 @impl
 def tox_add_option(parser: ToxParser) -> None:
     our = parser.add_command("exec", ["e"], "execute an arbitrary command within a tox environment", exec_)
     our.epilog = "For example: tox exec -e py39 -- python --version"
     register_env_select_flags(our, default=CliEnv("py"), multiple=False)
     env_run_create_flags(our, mode="exec")
 
 
 def exec_(state: State) -> int:
     envs = list(state.envs.iter())
     if len(envs) != 1:
-        raise HandledError(f"exactly one target environment allowed in exec mode but found {', '.join(envs)}")
+        msg = f"exactly one target environment allowed in exec mode but found {', '.join(envs)}"
+        raise HandledError(msg)
     loader = MemoryLoader(  # these configuration values are loaded from in-memory always (no file conf)
         commands_pre=[],
         commands=[],
         commands_post=[],
     )
     conf = state.envs[envs[0]].conf
     conf.loaders.insert(0, loader)
     to_path: Path | None = conf["change_dir"] if conf["args_are_paths"] else None
     pos_args = state.conf.pos_args(to_path)
     if not pos_args:
-        raise HandledError("You must specify a command as positional arguments, use -- <command>")
+        msg = "You must specify a command as positional arguments, use -- <command>"
+        raise HandledError(msg)
     loader.raw["commands"] = [Command(list(pos_args))]
     return run_sequential(state)
```

### Comparing `tox-4.6.0/src/tox/session/cmd/legacy.py` & `tox-4.6.1/src/tox/session/cmd/legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import cast
+from typing import TYPE_CHECKING, cast
 
 from packaging.requirements import InvalidRequirement, Requirement
 
 from tox.config.cli.parser import DEFAULT_VERBOSITY, Parsed, ToxParser
 from tox.config.loader.memory import MemoryLoader
 from tox.config.set_env import SetEnv
 from tox.plugin import impl
 from tox.session.cmd.run.common import env_run_create_flags
 from tox.session.cmd.run.parallel import OFF_VALUE, parallel_flags, run_parallel
 from tox.session.cmd.run.sequential import run_sequential
-from tox.session.state import State
+from tox.session.env_select import CliEnv, EnvSelector, register_env_select_flags
 from tox.tox_env.python.pip.req_file import PythonDeps
 
-from ..env_select import CliEnv, EnvSelector, register_env_select_flags
 from .devenv import devenv
 from .list_env import list_env
 from .show_config import show_config
 
+if TYPE_CHECKING:
+    from tox.session.state import State
+
 
 @impl
 def tox_add_option(parser: ToxParser) -> None:
     our = parser.add_command("legacy", ["le"], "legacy entry-point command", legacy)
     our.add_argument("--help-ini", "--hi", action="store_true", help="show live configuration", dest="show_config")
     our.add_argument(
         "--showconfig",
@@ -109,15 +111,15 @@
         option.devenv_path = Path(option.devenv_path)
         return devenv(state)
     if option.parallel != 0:  # only 0 means sequential
         return run_parallel(state)
     return run_sequential(state)
 
 
-def _handle_legacy_only_flags(option: Parsed, envs: EnvSelector) -> None:
+def _handle_legacy_only_flags(option: Parsed, envs: EnvSelector) -> None:  # noqa: C901
     override = {}
     if getattr(option, "site_packages", False):
         override["system_site_packages"] = True
     if getattr(option, "always_copy", False):
         override["always_copy"] = True
     set_env = {}
     if getattr(option, "pre", False):
```

### Comparing `tox-4.6.0/src/tox/session/cmd/quickstart.py` & `tox-4.6.1/src/tox/session/cmd/quickstart.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 import sys
 from pathlib import Path
 from textwrap import dedent
+from typing import TYPE_CHECKING
 
 from packaging.version import Version
 
-from tox.config.cli.parser import ToxParser
 from tox.plugin import impl
-from tox.session.state import State
 from tox.version import version as __version__
 
+if TYPE_CHECKING:
+    from tox.config.cli.parser import ToxParser
+    from tox.session.state import State
+
 
 @impl
 def tox_add_option(parser: ToxParser) -> None:
     our = parser.add_command(
         "quickstart",
         ["q"],
         "Command line script to quickly create a tox config file for a Python project",
@@ -29,15 +32,15 @@
     )
 
 
 def quickstart(state: State) -> int:
     root = state.conf.options.quickstart_root.absolute()
     tox_ini = root / "tox.ini"
     if tox_ini.exists():
-        print(f"{tox_ini} already exist, refusing to overwrite")
+        print(f"{tox_ini} already exist, refusing to overwrite")  # noqa: T201
         return 1
     version = str(Version(__version__.split("+")[0]))
     text = f"""
         [tox]
         env_list =
             py{''.join(str(i) for i in sys.version_info[0:2])}
         minversion = {version}
@@ -49,13 +52,13 @@
         deps =
             pytest>=6
         commands =
             pytest {{tty:--color=yes}} {{posargs}}
     """
     content = dedent(text).lstrip()
 
-    print(f"tox {__version__} quickstart utility, will create {tox_ini}:")
-    print(content, end="")
+    print(f"tox {__version__} quickstart utility, will create {tox_ini}:")  # noqa: T201
+    print(content, end="")  # noqa: T201
 
     root.mkdir(parents=True, exist_ok=True)
     tox_ini.write_text(content)
     return 0
```

### Comparing `tox-4.6.0/src/tox/session/cmd/show_config.py` & `tox-4.6.1/src/tox/session/cmd/show_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""
-Show materialized configuration of tox environments.
-"""
+"""Show materialized configuration of tox environments."""
 from __future__ import annotations
 
 from textwrap import indent
-from typing import Iterable
+from typing import TYPE_CHECKING, Iterable
 
 from colorama import Fore
 
-from tox.config.cli.parser import ToxParser
 from tox.config.loader.stringify import stringify
-from tox.config.sets import ConfigSet
 from tox.plugin import impl
 from tox.session.cmd.run.common import env_run_create_flags
 from tox.session.env_select import CliEnv, register_env_select_flags
-from tox.session.state import State
-from tox.tox_env.api import ToxEnv
+
+if TYPE_CHECKING:
+    from tox.config.cli.parser import ToxParser
+    from tox.config.sets import ConfigSet
+    from tox.session.state import State
+    from tox.tox_env.api import ToxEnv
 
 
 @impl
 def tox_add_option(parser: ToxParser) -> None:
     our = parser.add_command("config", ["c"], "show tox configuration", show_config)
     our.add_argument(
         "-k",
@@ -45,67 +45,67 @@
     is_first = True
 
     def _print_env(tox_env: ToxEnv) -> None:
         nonlocal is_first
         if is_first:
             is_first = False
         else:
-            print("")
+            print("")  # noqa: T201
         print_section_header(is_colored, f"[testenv:{tox_env.conf.name}]")
         if not keys:
             print_key_value(is_colored, "type", type(tox_env).__name__)
         print_conf(is_colored, tox_env.conf, keys)
 
     show_everything = state.conf.options.env.is_all
     done: set[str] = set()
     for name in state.envs.iter(package=True):  # now go through selected ones
         done.add(name)
         _print_env(state.envs[name])
 
     # environments may define core configuration flags, so we must exhaust first the environments to tell the core part
     if show_everything or state.conf.options.show_core:
-        print("")
+        print("")  # noqa: T201
         print_section_header(is_colored, "[tox]")
         print_conf(is_colored, state.conf.core, keys)
     return 0
 
 
-def _colored(is_colored: bool, color: int, msg: str) -> str:
+def _colored(is_colored: bool, color: int, msg: str) -> str:  # noqa: FBT001
     return f"{color}{msg}{Fore.RESET}" if is_colored else msg
 
 
-def print_section_header(is_colored: bool, name: str) -> None:
-    print(_colored(is_colored, Fore.YELLOW, name))
+def print_section_header(is_colored: bool, name: str) -> None:  # noqa: FBT001
+    print(_colored(is_colored, Fore.YELLOW, name))  # noqa: T201
 
 
-def print_comment(is_colored: bool, comment: str) -> None:
-    print(_colored(is_colored, Fore.CYAN, comment))
+def print_comment(is_colored: bool, comment: str) -> None:  # noqa: FBT001
+    print(_colored(is_colored, Fore.CYAN, comment))  # noqa: T201
 
 
-def print_key_value(is_colored: bool, key: str, value: str, multi_line: bool = False) -> None:
-    print(_colored(is_colored, Fore.GREEN, key), end="")
-    print(" =", end="")
+def print_key_value(is_colored: bool, key: str, value: str, multi_line: bool = False) -> None:  # noqa: FBT001, FBT002
+    print(_colored(is_colored, Fore.GREEN, key), end="")  # noqa: T201
+    print(" =", end="")  # noqa: T201
     if multi_line:
-        print("")
+        print("")  # noqa: T201
         value_str = indent(value, prefix="  ")
     else:
-        print(" ", end="")
+        print(" ", end="")  # noqa: T201
         value_str = value
-    print(value_str)
+    print(value_str)  # noqa: T201
 
 
-def print_conf(is_colored: bool, conf: ConfigSet, keys: Iterable[str]) -> None:
+def print_conf(is_colored: bool, conf: ConfigSet, keys: Iterable[str]) -> None:  # noqa: FBT001
     for key in keys if keys else conf:
         if key not in conf:
             continue
-        key = conf.primary_key(key)
+        key = conf.primary_key(key)  # noqa: PLW2901
         try:
             value = conf[key]
             as_str, multi_line = stringify(value)
-        except Exception as exception:  # because e.g. the interpreter cannot be found
+        except Exception as exception:  # because e.g. the interpreter cannot be found  # noqa: BLE001
             as_str, multi_line = _colored(is_colored, Fore.LIGHTRED_EX, f"# Exception: {exception!r}"), False
         if multi_line and "\n" not in as_str:
             multi_line = False
         print_key_value(is_colored, key, as_str, multi_line=multi_line)
     unused = conf.unused()
     if unused and not keys:
         print_comment(is_colored, f"# !!! unused: {', '.join(unused)}")
```

### Comparing `tox-4.6.0/src/tox/session/cmd/version_flag.py` & `tox-4.6.1/src/tox/session/cmd/version_flag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Display the version information about tox.
-"""
+"""Display the version information about tox."""
 from __future__ import annotations
 
 import sys
 from argparse import SUPPRESS, Action, ArgumentParser, Namespace
 from pathlib import Path
 from typing import Any, Sequence, cast
 
@@ -21,21 +19,21 @@
         def __init__(self, option_strings: Sequence[str], dest: str = SUPPRESS) -> None:
             help_msg = "show program's and plugins version number and exit"
             super().__init__(option_strings=option_strings, dest=dest, nargs=0, help=help_msg, default=SUPPRESS)
 
         def __call__(
             self,
             parser: ArgumentParser,
-            namespace: Namespace,  # noqa: U100
-            values: str | Sequence[Any] | None,  # noqa: U100
-            option_string: str | None = None,  # noqa: U100
+            namespace: Namespace,  # noqa: ARG002
+            values: str | Sequence[Any] | None,  # noqa: ARG002
+            option_string: str | None = None,  # noqa: ARG002
         ) -> None:
-            formatter = cast(HelpFormatter, parser._get_formatter())
+            formatter = cast(HelpFormatter, parser._get_formatter())  # noqa: SLF001
             formatter.add_raw_text(get_version_info())
-            parser._print_message(formatter.format_help(), sys.stdout)
+            parser._print_message(formatter.format_help(), sys.stdout)  # noqa: SLF001
             parser.exit()
 
     parser.add_argument("--version", action=_V)
 
 
 def get_version_info() -> str:
     out = [f"{version} from {Path(tox.__file__).absolute()}"]
```

### Comparing `tox-4.6.0/src/tox/session/cmd/run/common.py` & `tox-4.6.1/src/tox/session/cmd/run/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,71 @@
-"""Common functionality shared across multiple type of runs"""
+"""Common functionality shared across multiple type of runs."""
 from __future__ import annotations
 
 import logging
 import os
 import random
 import sys
 import time
 from argparse import Action, ArgumentError, ArgumentParser, Namespace
 from concurrent.futures import CancelledError, Future, ThreadPoolExecutor, as_completed
 from pathlib import Path
 from signal import SIGINT, Handlers, signal
 from threading import Event, Thread
-from typing import Any, Iterator, Optional, Sequence, cast
+from typing import TYPE_CHECKING, Any, Iterator, Optional, Sequence, cast
 
 from colorama import Fore
 
 from tox.config.types import EnvList
 from tox.execute import Outcome
 from tox.journal import write_journal
 from tox.session.cmd.run.single import ToxEnvRunResult, run_one
-from tox.session.state import State
-from tox.tox_env.api import ToxEnv
 from tox.tox_env.runner import RunToxEnv
 from tox.util.ci import is_ci
 from tox.util.graph import stable_topological_sort
 from tox.util.spinner import MISS_DURATION, Spinner
 
+if TYPE_CHECKING:
+    from tox.session.state import State
+    from tox.tox_env.api import ToxEnv
+
 
 class SkipMissingInterpreterAction(Action):
     def __call__(
         self,
-        parser: ArgumentParser,  # noqa: U100
+        parser: ArgumentParser,  # noqa: ARG002
         namespace: Namespace,
         values: str | Sequence[Any] | None,
-        option_string: str | None = None,  # noqa: U100
+        option_string: str | None = None,  # noqa: ARG002
     ) -> None:
         value = "true" if values is None else values
         if value not in ("config", "true", "false"):
             raise ArgumentError(self, f"value must be 'config', 'true', or 'false' (got {value!r})")
         setattr(namespace, self.dest, value)
 
 
 class InstallPackageAction(Action):
     def __call__(
         self,
-        parser: ArgumentParser,  # noqa: U100
+        parser: ArgumentParser,  # noqa: ARG002
         namespace: Namespace,
         values: str | Sequence[Any] | None,
-        option_string: str | None = None,  # noqa: U100
+        option_string: str | None = None,  # noqa: ARG002
     ) -> None:
         if not values:
             raise ArgumentError(self, "cannot be empty")
         path = Path(cast(str, values)).absolute()
         if not path.exists():
             raise ArgumentError(self, f"{path} does not exist")
         if not path.is_file():
             raise ArgumentError(self, f"{path} is not a file")
         setattr(namespace, self.dest, path)
 
 
-def env_run_create_flags(parser: ArgumentParser, mode: str) -> None:
+def env_run_create_flags(parser: ArgumentParser, mode: str) -> None:  # noqa: C901
     # mode can be one of: run, run-parallel, legacy, devenv, config
     if mode not in ("config", "depends"):
         parser.add_argument(
             "--result-json",
             dest="result_json",
             metavar="path",
             of_type=Path,
@@ -112,38 +114,39 @@
             dest="develop",
         )
     if mode not in ("depends",):
 
         class SeedAction(Action):
             def __call__(
                 self,
-                parser: ArgumentParser,  # noqa: U100
+                parser: ArgumentParser,  # noqa: ARG002
                 namespace: Namespace,
                 values: str | Sequence[Any] | None,
-                option_string: str | None = None,  # noqa: U100
+                option_string: str | None = None,  # noqa: ARG002
             ) -> None:
                 if values == "notset":
                     result = None
                 else:
                     try:
                         result = int(cast(str, values))
                         if result <= 0:
-                            raise ValueError("must be greater than zero")
+                            msg = "must be greater than zero"
+                            raise ValueError(msg)  # noqa: TRY301
                     except ValueError as exc:
-                        raise ArgumentError(self, str(exc))
+                        raise ArgumentError(self, str(exc)) from exc
                 setattr(namespace, self.dest, result)
 
         parser.add_argument(
             "--hashseed",
             metavar="SEED",
             help="set PYTHONHASHSEED to SEED before running commands. Defaults to a random integer in the range "
             "[1, 4294967295] ([1, 1024] on Windows). Passing 'noset' suppresses this behavior.",
             action=SeedAction,
             of_type=Optional[int],
-            default=random.randint(1, 1024 if sys.platform == "win32" else 4294967295),
+            default=random.randint(1, 1024 if sys.platform == "win32" else 4294967295),  # noqa: S311
             dest="hash_seed",
         )
     parser.add_argument(
         "--discover",
         dest="discover",
         nargs="+",
         metavar="path",
@@ -175,24 +178,24 @@
             "--skip-pkg-install",
             dest="skip_pkg_install",
             help="skip package installation for this run",
             action="store_true",
         )
 
 
-def report(start: float, runs: list[ToxEnvRunResult], is_colored: bool, verbosity: int) -> int:
+def report(start: float, runs: list[ToxEnvRunResult], is_colored: bool, verbosity: int) -> int:  # noqa: FBT001
     def _print(color_: int, message: str) -> None:
         if verbosity:
-            print(f"{color_ if is_colored else ''}{message}{Fore.RESET if is_colored else ''}")
+            print(f"{color_ if is_colored else ''}{message}{Fore.RESET if is_colored else ''}")  # noqa: T201
 
     successful, skipped = [], []
     for run in runs:
         successful.append(run.code == Outcome.OK or run.ignore_outcome)
         skipped.append(run.skipped)
-        duration_individual = [o.elapsed for o in run.outcomes] if verbosity >= 2 else []
+        duration_individual = [o.elapsed for o in run.outcomes] if verbosity >= 2 else []  # noqa: PLR2004
         extra = f"+cmd[{','.join(f'{i:.2f}' for i in duration_individual)}]" if duration_individual else ""
         setup = run.duration - sum(duration_individual)
         msg, color = _get_outcome_message(run)
         out = f"  {run.name}: {msg} ({run.duration:.2f}{f'=setup[{setup:.2f}]{extra}' if extra else ''} seconds)"
         _print(color, out)
 
     duration = time.monotonic() - start
@@ -207,26 +210,25 @@
 
 
 def _get_outcome_message(run: ToxEnvRunResult) -> tuple[str, int]:
     if run.skipped:
         msg, color = "SKIP", Fore.YELLOW
     elif run.code == Outcome.OK:
         msg, color = "OK", Fore.GREEN
+    elif run.ignore_outcome:
+        msg, color = f"IGNORED FAIL code {run.code}", Fore.YELLOW
     else:
-        if run.ignore_outcome:
-            msg, color = f"IGNORED FAIL code {run.code}", Fore.YELLOW
-        else:
-            msg, color = f"FAIL code {run.code}", Fore.RED
+        msg, color = f"FAIL code {run.code}", Fore.RED
     return msg, color
 
 
 logger = logging.getLogger(__name__)
 
 
-def execute(state: State, max_workers: int | None, has_spinner: bool, live: bool) -> int:
+def execute(state: State, max_workers: int | None, has_spinner: bool, live: bool) -> int:  # noqa: FBT001
     interrupt, done = Event(), Event()
     results: list[ToxEnvRunResult] = []
     future_to_env: dict[Future[ToxEnvRunResult], ToxEnv] = {}
     state.envs.ensure_only_run_env_is_active()
     to_run_list: list[str] = list(state.envs.iter())
     for name in to_run_list:
         cast(RunToxEnv, state.envs[name]).mark_active()
@@ -240,78 +242,76 @@
         )
         thread.start()
         try:
             thread.join()
         except KeyboardInterrupt:
             previous, has_previous = signal(SIGINT, Handlers.SIG_IGN), True
             spinner.print_report = False  # no need to print reports at this point, final report coming up
-            logger.error(f"[{os.getpid()}] KeyboardInterrupt - teardown started")
+            logger.error("[%s] KeyboardInterrupt - teardown started", os.getpid())  # noqa: TRY400
             interrupt.set()
             # cancel in reverse order to not allow submitting new jobs as we cancel running ones
             for future, tox_env in reversed(list(future_to_env.items())):
                 cancelled = future.cancel()
                 # if cannot be cancelled and not done -> still runs
                 if cancelled is False and not future.done():  # pragma: no branch
                     tox_env.interrupt()
             done.wait()
             # workaround for https://bugs.python.org/issue45274
             lock = getattr(thread, "_tstate_lock", None)
             if lock is not None and lock.locked():  # pragma: no branch
                 lock.release()  # pragma: no cover
-                thread._stop()  # type: ignore  # pragma: no cover # calling private method to fix thread state
+                # calling private method to fix thread state
+                thread._stop()  # type: ignore[attr-defined] # pragma: no cover # noqa: SLF001
             thread.join()
     finally:
         ordered_results: list[ToxEnvRunResult] = []
         name_to_run = {r.name: r for r in results}
         for env in to_run_list:
             ordered_results.append(name_to_run[env])
         # write the journal
-        write_journal(getattr(state.conf.options, "result_json", None), state._journal)
+        write_journal(getattr(state.conf.options, "result_json", None), state._journal)  # noqa: SLF001
         # report the outcome
         exit_code = report(
             state.conf.options.start,
             ordered_results,
             state.conf.options.is_colored,
             state.conf.options.verbosity,
         )
         if has_previous:
             signal(SIGINT, previous)
     return exit_code
 
 
 class ToxSpinner(Spinner):
-    def __init__(self, enabled: bool, state: State, total: int) -> None:
+    def __init__(self, enabled: bool, state: State, total: int) -> None:  # noqa: FBT001
         super().__init__(
             enabled=enabled,
             colored=state.conf.options.is_colored,
-            stream=state._options.log_handler.stdout,
+            stream=state._options.log_handler.stdout,  # noqa: SLF001
             total=total,
         )
 
-    def update_spinner(self, result: ToxEnvRunResult, success: bool) -> None:
-        if success:
-            done = self.skip if result.skipped else self.succeed
-        else:
-            done = self.fail
+    def update_spinner(self, result: ToxEnvRunResult, success: bool) -> None:  # noqa: FBT001
+        done = (self.skip if result.skipped else self.succeed) if success else self.fail
         done(result.name)
 
 
-def _queue_and_wait(
+def _queue_and_wait(  # noqa: C901, PLR0913, PLR0915
     state: State,
     to_run_list: list[str],
     results: list[ToxEnvRunResult],
     future_to_env: dict[Future[ToxEnvRunResult], ToxEnv],
     interrupt: Event,
     done: Event,
     max_workers: int | None,
     spinner: ToxSpinner,
-    live: bool,
+    live: bool,  # noqa: FBT001
 ) -> None:
     try:
-        options = state._options
+        options = state._options  # noqa: SLF001
         with spinner:
             max_workers = len(to_run_list) if max_workers is None else max_workers
             completed: set[str] = set()
             envs_to_run_generator = ready_to_run_envs(state, to_run_list, completed)
 
             def _run(tox_env: RunToxEnv) -> ToxEnvRunResult:
                 spinner.add(tox_env.conf.name)
@@ -376,15 +376,20 @@
             # call teardown - configuration only environments for example could not be finished
             for name in to_run_list:
                 state.envs[name].teardown()
         finally:
             done.set()
 
 
-def _handle_one_run_done(result: ToxEnvRunResult, spinner: ToxSpinner, state: State, live: bool) -> None:
+def _handle_one_run_done(
+    result: ToxEnvRunResult,
+    spinner: ToxSpinner,
+    state: State,
+    live: bool,  # noqa: FBT001
+) -> None:
     success = result.code == Outcome.OK
     spinner.update_spinner(result, success)
     tox_env = cast(RunToxEnv, state.envs[result.name])
     if tox_env.journal:  # add overall journal entry
         tox_env.journal["result"] = {
             "success": success,
             "exit_code": result.code,
@@ -395,21 +400,21 @@
         pkg_out_err_list = []
         for package_env in tox_env.package_envs:
             pkg_out_err = package_env.close_and_read_out_err()
             if pkg_out_err is not None:  # pragma: no branch
                 pkg_out_err_list.append(pkg_out_err)
         if not success or tox_env.conf["parallel_show_output"]:
             for pkg_out_err in pkg_out_err_list:
-                state._options.log_handler.write_out_err(pkg_out_err)  # pragma: no cover
+                state._options.log_handler.write_out_err(pkg_out_err)  # pragma: no cover  # noqa: SLF001
             if out_err is not None:  # pragma: no branch # first show package build
-                state._options.log_handler.write_out_err(out_err)
+                state._options.log_handler.write_out_err(out_err)  # noqa: SLF001
 
 
 def ready_to_run_envs(state: State, to_run: list[str], completed: set[str]) -> Iterator[list[str]]:
-    """Generate tox environments ready to run"""
+    """Generate tox environments ready to run."""
     order, todo = run_order(state, to_run)
     while order:
         ready_to_run: list[str] = []
         new_order: list[str] = []
         for env in order:  # collect next batch of ready to run
             if todo[env] - completed:
                 new_order.append(env)
```

### Comparing `tox-4.6.0/src/tox/session/cmd/run/parallel.py` & `tox-4.6.1/src/tox/session/cmd/run/parallel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-"""
-Run tox environments in parallel.
-"""
+"""Run tox environments in parallel."""
 from __future__ import annotations
 
 import logging
 from argparse import ArgumentParser, ArgumentTypeError
+from typing import TYPE_CHECKING
 
-from tox.config.cli.parser import ToxParser
 from tox.plugin import impl
-from tox.session.state import State
+from tox.session.env_select import CliEnv, register_env_select_flags
 from tox.util.cpu import auto_detect_cpus
 
-from ...env_select import CliEnv, register_env_select_flags
 from .common import env_run_create_flags, execute
 
+if TYPE_CHECKING:
+    from tox.config.cli.parser import ToxParser
+    from tox.session.state import State
+
 logger = logging.getLogger(__name__)
 
 ENV_VAR_KEY = "TOX_PARALLEL_ENV"
 OFF_VALUE = 0
 DEFAULT_PARALLEL = OFF_VALUE
 
 
@@ -33,32 +34,34 @@
     if str_value == "all":
         return None
     if str_value == "auto":
         return auto_detect_cpus()
     try:
         value = int(str_value)
     except ValueError as exc:
-        raise ArgumentTypeError(f"value must be a positive number, is {str_value!r}") from exc
+        msg = f"value must be a positive number, is {str_value!r}"
+        raise ArgumentTypeError(msg) from exc
     if value < 0:
-        raise ArgumentTypeError(f"value must be positive, is {value!r}")
+        msg = f"value must be positive, is {value!r}"
+        raise ArgumentTypeError(msg)
     return value
 
 
-def parallel_flags(our: ArgumentParser, default_parallel: int, no_args: bool = False) -> None:
+def parallel_flags(our: ArgumentParser, default_parallel: int, no_args: bool = False) -> None:  # noqa: FBT001, FBT002
     our.add_argument(
         "-p",
         "--parallel",
         dest="parallel",
         help="run tox environments in parallel, the argument controls limit: all,"
         " auto - cpu count, some positive number, zero is turn off",
         action="store",
-        type=parse_num_processes,  # type: ignore # nargs confuses it
+        type=parse_num_processes,  # type: ignore[arg-type]  # nargs confuses it
         default=default_parallel,
         metavar="VAL",
-        **({"nargs": "?"} if no_args else {}),  # type: ignore # type checker can't unroll it
+        **({"nargs": "?"} if no_args else {}),  # type: ignore[arg-type] # type checker can't unroll it
     )
     our.add_argument(
         "-o",
         "--parallel-live",
         action="store_true",
         dest="parallel_live",
         help="connect to stdout while running environments",
@@ -68,15 +71,15 @@
         action="store_true",
         dest="parallel_no_spinner",
         help="do not show the spinner",
     )
 
 
 def run_parallel(state: State) -> int:
-    """here we'll just start parallel sub-processes"""
+    """Here we'll just start parallel sub-processes."""
     option = state.conf.options
     return execute(
         state,
         max_workers=option.parallel,
         has_spinner=option.parallel_no_spinner is False and option.parallel_live is False,
         live=option.parallel_live,
     )
```

### Comparing `tox-4.6.0/src/tox/session/cmd/run/sequential.py` & `tox-4.6.1/src/tox/session/cmd/run/sequential.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-"""
-Run tox environments in sequential order.
-"""
+"""Run tox environments in sequential order."""
 from __future__ import annotations
 
-from tox.config.cli.parser import ToxParser
+from typing import TYPE_CHECKING
+
 from tox.plugin import impl
-from tox.session.state import State
+from tox.session.env_select import CliEnv, register_env_select_flags
 
-from ...env_select import CliEnv, register_env_select_flags
 from .common import env_run_create_flags, execute
 
+if TYPE_CHECKING:
+    from tox.config.cli.parser import ToxParser
+    from tox.session.state import State
+
 
 @impl
 def tox_add_option(parser: ToxParser) -> None:
     our = parser.add_command("run", ["r"], "run environments", run_sequential)
     register_env_select_flags(our, default=CliEnv())
     env_run_create_flags(our, mode="run")
```

### Comparing `tox-4.6.0/src/tox/session/cmd/run/single.py` & `tox-4.6.1/src/tox/session/cmd/run/single.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,75 @@
-"""
-Defines how to run a single tox environment.
-"""
+"""Defines how to run a single tox environment."""
 from __future__ import annotations
 
 import logging
 import time
-from pathlib import Path
-from typing import NamedTuple, cast
+from typing import TYPE_CHECKING, NamedTuple, cast
 
-from tox.config.types import Command
 from tox.execute.api import Outcome, StdinSource
-from tox.tox_env.api import ToxEnv
 from tox.tox_env.errors import Fail, Skip
 from tox.tox_env.python.virtual_env.package.pyproject import ToxBackendFailed
-from tox.tox_env.runner import RunToxEnv
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.config.types import Command
+    from tox.tox_env.api import ToxEnv
+    from tox.tox_env.runner import RunToxEnv
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ToxEnvRunResult(NamedTuple):
     name: str
     skipped: bool
     code: int
     outcomes: list[Outcome]
     duration: float
     ignore_outcome: bool = False
 
 
-def run_one(tox_env: RunToxEnv, no_test: bool, suspend_display: bool) -> ToxEnvRunResult:
+def run_one(tox_env: RunToxEnv, no_test: bool, suspend_display: bool) -> ToxEnvRunResult:  # noqa: FBT001
     start_one = time.monotonic()
     name = tox_env.conf.name
     with tox_env.display_context(suspend_display):
         skipped, code, outcomes = _evaluate(tox_env, no_test)
     duration = time.monotonic() - start_one
     return ToxEnvRunResult(name, skipped, code, outcomes, duration, tox_env.conf["ignore_outcome"])
 
 
-def _evaluate(tox_env: RunToxEnv, no_test: bool) -> tuple[bool, int, list[Outcome]]:
+def _evaluate(tox_env: RunToxEnv, no_test: bool) -> tuple[bool, int, list[Outcome]]:  # noqa: FBT001
     skipped = False
     code: int = 0
     outcomes: list[Outcome] = []
     try:
         try:
             tox_env.setup()
             code, outcomes = run_commands(tox_env, no_test)
         except Skip as exception:
             LOGGER.warning("skipped because %s", exception)
             code = 0
             skipped = True
         except ToxBackendFailed as exception:
             LOGGER.error("%s", exception)
-            raise SystemExit(exception.code)
+            raise SystemExit(exception.code)  # noqa: B904, TRY200
         except Fail as exception:
             LOGGER.error("failed with %s", exception)
             code = 1
-        except Exception:  # pragma: no cover
+        except Exception:  # pragma: no cover  # noqa: BLE001
             LOGGER.exception("internal error")  # pragma: no cover
             code = 2  # pragma: no cover
         finally:
             tox_env.teardown()
     except SystemExit as exception:  # setup command fails (interrupted or via invocation)
         code = cast(int, exception.code)
     return skipped, code, outcomes
 
 
-def run_commands(tox_env: RunToxEnv, no_test: bool) -> tuple[int, list[Outcome]]:
+def run_commands(tox_env: RunToxEnv, no_test: bool) -> tuple[int, list[Outcome]]:  # noqa: FBT001
     outcomes: list[Outcome] = []
     if no_test:
         exit_code = Outcome.OK
     else:
         from tox.plugin.manager import MANAGER  # importing this here to avoid circular import
 
         chdir: Path = tox_env.conf["change_dir"]
@@ -87,15 +88,21 @@
                 status_post = run_command_set(tox_env, "commands_post", chdir, ignore_errors, outcomes)
         finally:
             exit_code = status_pre or status_main or status_post  # first non-success
             MANAGER.tox_after_run_commands(tox_env, exit_code, outcomes)
     return exit_code, outcomes
 
 
-def run_command_set(tox_env: ToxEnv, key: str, cwd: Path, ignore_errors: bool, outcomes: list[Outcome]) -> int:
+def run_command_set(
+    tox_env: ToxEnv,
+    key: str,
+    cwd: Path,
+    ignore_errors: bool,  # noqa: FBT001
+    outcomes: list[Outcome],
+) -> int:
     exit_code = Outcome.OK
     command_set: list[Command] = tox_env.conf[key]
     for at, cmd in enumerate(command_set):
         current_outcome = tox_env.execute(
             cmd.args,
             cwd=cwd,
             stdin=StdinSource.user_only(),
```

### Comparing `tox-4.6.0/src/tox/tox_env/api.py` & `tox-4.6.1/src/tox/tox_env/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-"""
-Defines the abstract base traits of a tox environment.
-"""
+"""Defines the abstract base traits of a tox environment."""
 from __future__ import annotations
 
 import fnmatch
 import logging
 import os
 import re
 import string
 import sys
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from io import BytesIO
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterator, List, NamedTuple, Sequence, Set, cast
 
-from tox.config.main import Config
-from tox.config.set_env import SetEnv
-from tox.config.sets import CoreConfigSet, EnvConfigSet
-from tox.execute.api import Execute, ExecuteStatus, Outcome, StdinSource
 from tox.execute.request import ExecuteRequest
-from tox.journal import EnvJournal
-from tox.report import OutErr, ToxHandler
 from tox.tox_env.errors import Fail, Recreate, Skip
 from tox.tox_env.info import Info
-from tox.tox_env.installer import Installer
 from tox.util.path import ensure_empty_dir
 
 if TYPE_CHECKING:
     from tox.config.cli.parser import Parsed
+    from tox.config.main import Config
+    from tox.config.set_env import SetEnv
+    from tox.config.sets import CoreConfigSet, EnvConfigSet
+    from tox.execute.api import Execute, ExecuteStatus, Outcome, StdinSource
+    from tox.journal import EnvJournal
+    from tox.report import OutErr, ToxHandler
+    from tox.tox_env.installer import Installer
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ToxEnvCreateArgs(NamedTuple):
-    """Arguments to pass on when creating a tox environment"""
+    """Arguments to pass on when creating a tox environment."""
 
     conf: EnvConfigSet
     core: CoreConfigSet
     options: Parsed
     journal: EnvJournal
     log_handler: ToxHandler
 
 
 class ToxEnv(ABC):
     """A tox environment."""
 
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
-        """Create a new tox environment.
+        """
+        Create a new tox environment.
 
         :param create_args: tox env create args
         """
         self.journal: EnvJournal = create_args.journal  #: handler to the tox reporting system
         self.conf: EnvConfigSet = create_args.conf  #: the config set to use for this environment
         self.core: CoreConfigSet = create_args.core  #: the core tox config set
         self.options: Parsed = create_args.options  #: CLI options
@@ -72,15 +71,15 @@
 
     @property
     def cache(self) -> Info:
         return Info(self.env_dir)
 
     @staticmethod
     @abstractmethod
-    def id() -> str:
+    def id() -> str:  # noqa: A003
         raise NotImplementedError
 
     @property
     @abstractmethod
     def executor(self) -> Execute:
         raise NotImplementedError
 
@@ -109,27 +108,27 @@
             of_type=Set[str],
             default=set(),
             desc="labels attached to the tox environment",
         )
         self.conf.add_config(
             keys=["env_dir", "envdir"],
             of_type=Path,
-            default=lambda conf, name: cast(Path, conf.core["work_dir"]) / self.name,  # noqa: U100
+            default=lambda conf, name: cast(Path, conf.core["work_dir"]) / self.name,  # noqa: ARG005
             desc="directory assigned to the tox environment",
         )
         self.conf.add_config(
             keys=["env_tmp_dir", "envtmpdir"],
             of_type=Path,
-            default=lambda conf, name: cast(Path, conf.core["work_dir"]) / self.name / "tmp",  # noqa: U100
+            default=lambda conf, name: cast(Path, conf.core["work_dir"]) / self.name / "tmp",  # noqa: ARG005
             desc="a folder that is always reset at the start of the run",
         )
         self.conf.add_config(
             keys=["env_log_dir", "envlogdir"],
             of_type=Path,
-            default=lambda conf, name: cast(Path, conf.core["work_dir"]) / self.name / "log",  # noqa: U100
+            default=lambda conf, name: cast(Path, conf.core["work_dir"]) / self.name / "log",  # noqa: ARG005
             desc="a folder for logging where tox will put logs of tool invocation",
         )
         self.executor.register_conf(self)
         self.conf.default_set_env_loader = self._default_set_env
         self.conf.add_config(
             keys=["platform"],
             of_type=str,
@@ -140,18 +139,19 @@
         def pass_env_post_process(values: list[str]) -> list[str]:
             values.extend(self._default_pass_env())
             result = sorted({k: None for k in values}.keys())
             invalid_chars = set(string.whitespace)
             invalid = [v for v in result if any(c in invalid_chars for c in v)]
             if invalid:
                 invalid_repr = ", ".join(repr(i) for i in invalid)
-                raise Fail(
-                    f"pass_env values cannot contain whitespace, use comma to have multiple values in a single line, "
-                    f"invalid values found {invalid_repr}",
+                msg = (
+                    f"pass_env values cannot contain whitespace, use comma to have multiple values in a single line,"
+                    f" invalid values found {invalid_repr}"
                 )
+                raise Fail(msg)
             return result
 
         self.conf.add_config(
             keys=["pass_env", "passenv"],
             of_type=List[str],
             default=[],
             desc="environment variables to pass on to the tox environment",
@@ -171,17 +171,17 @@
         )
         self.conf.add_config(
             "allowlist_externals",
             of_type=List[str],
             default=[],
             desc="external command glob to allow calling",
         )
-        assert self.installer is not None  # trigger installer creation to allow configuration registration
+        assert self.installer is not None  # noqa: S101 # trigger installer creation to allow config registration
 
-    def _recreate_default(self, conf: Config, value: str | None) -> bool:  # noqa: U100
+    def _recreate_default(self, conf: Config, value: str | None) -> bool:  # noqa: ARG002
         return cast(bool, self.options.recreate)
 
     @property
     def env_dir(self) -> Path:
         """:return: the tox environments environment folder"""
         return cast(Path, self.conf["env_dir"])
 
@@ -233,28 +233,26 @@
                 ],
             )
         else:  # pragma: win32 no cover
             env.append("TMPDIR")  # temporary file location
         return env
 
     def setup(self) -> None:
-        """
-        Setup the tox environment.
-        """
+        """Setup the tox environment."""
         if self._run_state["setup"] is False:  # pragma: no branch
             self._platform_check()
             recreate = cast(bool, self.conf["recreate"])
             if recreate:
                 self._clean(transitive=True)
             try:
                 self._setup_env()
                 self._setup_with_env()
             except Recreate as exception:  # once we might try over
                 if not recreate:  # pragma: no cover
-                    logging.warning(f"recreate env because {exception.args[0]}")
+                    logging.warning("recreate env because %s", exception.args[0])
                     self._clean(transitive=False)
                     self._setup_env()
                     self._setup_with_env()
             else:
                 self._done_with_setup()
             finally:
                 self._run_state["setup"] = True
@@ -269,56 +267,58 @@
                 MANAGER.tox_env_teardown(self)
                 self._run_state["teardown"] = True
 
     def _teardown(self) -> None:  # noqa: B027 # empty abstract base class
         pass
 
     def _platform_check(self) -> None:
-        """skip env when platform does not match"""
+        """Skip env when platform does not match."""
         platform_str: str = self.conf["platform"]
         if platform_str:
             match = re.fullmatch(platform_str, self.runs_on_platform)
             if match is None:
-                raise Skip(f"platform {self.runs_on_platform} does not match {platform_str}")
+                msg = f"platform {self.runs_on_platform} does not match {platform_str}"
+                raise Skip(msg)
 
     @property
     @abstractmethod
     def runs_on_platform(self) -> str:
         raise NotImplementedError
 
     def _setup_env(self) -> None:
         """
         1. env dir exists
         2. contains a runner with the same type.
         """
         conf = {"name": self.conf.name, "type": type(self).__name__}
         with self.cache.compare(conf, ToxEnv.__name__) as (eq, old):
             if eq is False and old is not None:  # pragma: no branch  # recreate if already created and not equals
-                raise Recreate(f"env type changed from {old} to {conf}")
+                msg = f"env type changed from {old} to {conf}"
+                raise Recreate(msg)
         self._handle_env_tmp_dir()
         self._handle_core_tmp_dir()
 
     def _setup_with_env(self) -> None:  # noqa: B027 # empty abstract base class
         pass
 
     def _done_with_setup(self) -> None:  # noqa: B027 # empty abstract base class
-        """called when setup is done"""
+        """Called when setup is done."""
 
     def _handle_env_tmp_dir(self) -> None:
-        """Ensure exists and empty"""
+        """Ensure exists and empty."""
         env_tmp_dir = self.env_tmp_dir
         if env_tmp_dir.exists() and next(env_tmp_dir.iterdir(), None) is not None:
             LOGGER.debug("clear env temp folder %s", env_tmp_dir)
             ensure_empty_dir(env_tmp_dir)
         env_tmp_dir.mkdir(parents=True, exist_ok=True)
 
     def _handle_core_tmp_dir(self) -> None:
         self.core["temp_dir"].mkdir(parents=True, exist_ok=True)
 
-    def _clean(self, transitive: bool = False) -> None:  # noqa: U100
+    def _clean(self, transitive: bool = False) -> None:  # noqa: ARG002, FBT001, FBT002
         if self._run_state["clean"]:  # pragma: no branch
             return  # pragma: no cover
         env_dir = self.env_dir
         if env_dir.exists():
             LOGGER.warning("remove tox env folder %s", env_dir)
             ensure_empty_dir(env_dir, except_filename="file.lock")
         self._log_id = 0  # we deleted logs, so start over counter
@@ -371,18 +371,17 @@
         result: list[str] = [f"{i}{os.sep}*" for i in self._paths]
         result.extend(i.strip() for i in self.conf["allowlist_externals"])
         return result
 
     def _make_path(self) -> str:
         values = dict.fromkeys(str(i) for i in self._paths)
         values.update(dict.fromkeys(os.environ.get("PATH", "").split(os.pathsep)))
-        result = os.pathsep.join(values)
-        return result
+        return os.pathsep.join(values)
 
-    def execute(
+    def execute(  # noqa: PLR0913
         self,
         cmd: Sequence[Path | str],
         stdin: StdinSource,
         show: bool | None = None,
         cwd: Path | None = None,
         run_id: str = "",
         executor: Execute | None = None,
@@ -398,31 +397,31 @@
         """Interrupt the execution of a tox environment."""
         logging.warning("interrupt tox environment: %s", self.conf.name)
         self._interrupted = True
         for status in list(self._execute_statuses.values()):
             status.interrupt()
 
     @contextmanager
-    def execute_async(
+    def execute_async(  # noqa: PLR0913
         self,
         cmd: Sequence[Path | str],
         stdin: StdinSource,
         show: bool | None = None,
         cwd: Path | None = None,
         run_id: str = "",
         executor: Execute | None = None,
     ) -> Iterator[ExecuteStatus]:
         if self._interrupted:
             raise SystemExit(-2)  # pragma: no cover
         if cwd is None:
             cwd = self.core["tox_root"]
         if show is None:
-            show = self.options.verbosity > 3
+            show = self.options.verbosity > 3  # noqa: PLR2004
         request = ExecuteRequest(cmd, cwd, self.environment_variables, stdin, run_id, allow=self._allow_externals)
-        if _CWD == request.cwd:
+        if request.cwd == _CWD:
             repr_cwd = ""
         else:
             try:
                 repr_cwd = f" {_CWD.relative_to(cwd)}"
             except ValueError:
                 repr_cwd = f" {cwd}"
         LOGGER.warning("%s%s> %s", run_id, repr_cwd, request.shell_cmd)
@@ -432,17 +431,17 @@
         with self._execute_call(executor, out_err, request, show) as execute_status:
             execute_id = id(execute_status)
             try:
                 self._execute_statuses[execute_id] = execute_status
                 yield execute_status
             finally:
                 self._execute_statuses.pop(execute_id)
-        if show and self._hidden_outcomes is not None:
-            if execute_status.outcome is not None:  # pragma: no cover # if it gets cancelled before even starting
-                self._hidden_outcomes.append(execute_status.outcome)
+        if show and self._hidden_outcomes is not None and execute_status.outcome is not None:
+            # if it gets cancelled before even starting
+            self._hidden_outcomes.append(execute_status.outcome)
         if self.journal and execute_status.outcome is not None:
             self.journal.add_execute(execute_status.outcome, run_id)
         self._log_execute(request, execute_status)
 
     def _log_execute(self, request: ExecuteRequest, status: ExecuteStatus) -> None:
         if self._log_id == 0:  # start with fresh slate on new run
             ensure_empty_dir(self.env_log_dir)
@@ -474,31 +473,30 @@
 
     @contextmanager
     def _execute_call(
         self,
         executor: Execute,
         out_err: OutErr,
         request: ExecuteRequest,
-        show: bool,
+        show: bool,  # noqa: FBT001
     ) -> Iterator[ExecuteStatus]:
         with executor.call(
             request=request,
             env=self,
             show=show,
             out_err=out_err,
         ) as execute_status:
             yield execute_status
 
     @contextmanager
-    def display_context(self, suspend: bool) -> Iterator[None]:
-        with self._log_context():
-            with self.log_handler.suspend_out_err(suspend, self._suspended_out_err) as out_err:
-                if suspend:  # only set if suspended
-                    self._suspended_out_err = out_err
-                yield
+    def display_context(self, suspend: bool) -> Iterator[None]:  # noqa: FBT001
+        with self._log_context(), self.log_handler.suspend_out_err(suspend, self._suspended_out_err) as out_err:
+            if suspend:  # only set if suspended
+                self._suspended_out_err = out_err
+            yield
 
     def close_and_read_out_err(self) -> tuple[bytes, bytes] | None:
         if self._suspended_out_err is None:  # pragma: no branch
             return None  # pragma: no cover
         (out, err), self._suspended_out_err = self._suspended_out_err, None
         out_b, err_b = cast(BytesIO, out.buffer).getvalue(), cast(BytesIO, err.buffer).getvalue()
         out.close()
```

### Comparing `tox-4.6.0/src/tox/tox_env/info.py` & `tox-4.6.1/src/tox/tox_env/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 Declare and handle the tox env info file (a file at the root of every tox environment that contains information about
 the status of the tox environment - python version of the environment, installed packages, etc.).
 """
 from __future__ import annotations
 
 import json
 from contextlib import contextmanager
-from pathlib import Path
-from typing import Any, Iterator
+from typing import TYPE_CHECKING, Any, Iterator
+
+if TYPE_CHECKING:
+    from pathlib import Path
 
 
 class Info:
     """Stores metadata about the tox environment."""
 
     def __init__(self, path: Path) -> None:
         self._path = path / ".tox-info.json"
@@ -46,19 +48,18 @@
         if old == value:
             yield True, old
         else:
             yield False, old
             # if no exception thrown update
             if sub_section is None:
                 self._content[section] = value
+            elif self._content.get(section) is None:
+                self._content[section] = {sub_section: value}
             else:
-                if self._content.get(section) is None:
-                    self._content[section] = {sub_section: value}
-                else:
-                    self._content[section][sub_section] = value
+                self._content[section][sub_section] = value
             self._write()
 
     def reset(self) -> None:
         self._content = {}
 
     def _write(self) -> None:
         self._path.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `tox-4.6.0/src/tox/tox_env/installer.py` & `tox-4.6.1/src/tox/tox_env/installer.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Installer(ABC, Generic[T]):
     def __init__(self, tox_env: T) -> None:
         self._env = tox_env
         self._register_config()
 
     @abstractmethod
     def _register_config(self) -> None:
-        """Register configurations for the installer"""
+        """Register configurations for the installer."""
         raise NotImplementedError
 
     @abstractmethod
     def installed(self) -> Any:
         """:returns: a list of packages installed (JSON dump-able)"""
         raise NotImplementedError
```

### Comparing `tox-4.6.0/src/tox/tox_env/package.py` & `tox-4.6.1/src/tox/tox_env/package.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-"""
-A tox environment that can build packages.
-"""
+"""A tox environment that can build packages."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 from threading import RLock
 from types import MethodType
 from typing import TYPE_CHECKING, Any, Callable, Generator, Iterator, cast
 
 from filelock import FileLock
 
-from tox.config.main import Config
-from tox.config.sets import EnvConfigSet
-
 from .api import ToxEnv, ToxEnvCreateArgs
 
 if TYPE_CHECKING:
+    from tox.config.main import Config
+    from tox.config.sets import EnvConfigSet
+
     from .runner import RunToxEnv
 
 
 class Package:
-    """package"""
+    """package."""
 
 
 class PathPackage(Package):
     def __init__(self, path: Path) -> None:
         super().__init__()
         self.path = path
 
@@ -87,15 +85,15 @@
     def _recreate_default(self, conf: Config, value: str | None) -> bool:
         return self.options.no_recreate_pkg is False and super()._recreate_default(conf, value)
 
     @abstractmethod
     def perform_packaging(self, for_env: EnvConfigSet) -> list[Package]:
         raise NotImplementedError
 
-    def register_run_env(self, run_env: RunToxEnv) -> Generator[tuple[str, str], PackageToxEnv, None]:  # noqa: U100
+    def register_run_env(self, run_env: RunToxEnv) -> Generator[tuple[str, str], PackageToxEnv, None]:  # noqa: ARG002
         yield from ()  # empty generator by default
 
     def mark_active_run_env(self, run_env: RunToxEnv) -> None:
         self._envs.add(run_env.conf.name)
 
     def teardown_env(self, conf: EnvConfigSet) -> None:
         self._envs.remove(conf.name)
```

### Comparing `tox-4.6.0/src/tox/tox_env/register.py` & `tox-4.6.1/src/tox/tox_env/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-"""
-Manages the tox environment registry.
-"""
+"""Manages the tox environment registry."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Iterable
 
-from .package import PackageToxEnv
-from .runner import RunToxEnv
-
 if TYPE_CHECKING:
     from tox.plugin.manager import Plugin
 
+    from .package import PackageToxEnv
+    from .runner import RunToxEnv
+
 
 class ToxEnvRegister:
-    """tox environment registry"""
+    """tox environment registry."""
 
     def __init__(self) -> None:
         self._run_envs: dict[str, type[RunToxEnv]] = {}
         self._package_envs: dict[str, type[PackageToxEnv]] = {}
         self._default_run_env: str = ""
 
     def _register_tox_env_types(self, manager: Plugin) -> None:
@@ -55,15 +53,16 @@
     def default_env_runner(self, value: str) -> None:
         """
         Change the default run environment type.
 
         :param value: the new run environment type by name
         """
         if value not in self._run_envs:
-            raise ValueError("run env must be registered before setting it as default")
+            msg = "run env must be registered before setting it as default"
+            raise ValueError(msg)
         self._default_run_env = value
 
     def runner(self, name: str) -> type[RunToxEnv]:
         """
         Lookup a run tox environment type by name.
 
         :param name: the name of the runner type
```

### Comparing `tox-4.6.0/src/tox/tox_env/runner.py` & `tox-4.6.1/src/tox/tox_env/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import logging
 import os
 import re
 from abc import ABC, abstractmethod
 from hashlib import sha256
-from typing import Any, Iterable, List
+from typing import TYPE_CHECKING, Any, Iterable, List
 
 from tox.config.types import Command, EnvList
-from tox.journal import EnvJournal
 
 from .api import ToxEnv, ToxEnvCreateArgs
 from .package import Package, PackageToxEnv, PathPackage
 from .util import add_change_dir_conf
 
+if TYPE_CHECKING:
+    from tox.journal import EnvJournal
+
 
 class RunToxEnv(ToxEnv, ABC):
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
         self.package_env: PackageToxEnv | None = None
         self._packages: list[Package] = []
         super().__init__(create_args)
         self._package_envs: list[PackageToxEnv | Exception] | None = None
@@ -111,15 +113,15 @@
         return None
 
     def _call_pkg_envs(self, method_name: str, *args: Any) -> None:
         for package_env in self.package_envs:
             with package_env.display_context(suspend=self._has_display_suspended):
                 getattr(package_env, method_name)(*args)
 
-    def _clean(self, transitive: bool = False) -> None:
+    def _clean(self, transitive: bool = False) -> None:  # noqa: FBT001, FBT002
         super()._clean(transitive)
         if transitive:
             self._call_pkg_envs("_clean")
 
     @property
     def _default_package_env(self) -> str:
         return ".pkg"
@@ -139,15 +141,15 @@
             skip_pkg_install: bool = getattr(self.options, "skip_pkg_install", False)
             if skip_pkg_install is True:
                 logging.warning("skip building and installing the package")
             else:
                 self._setup_pkg()
 
     def _register_package_conf(self) -> bool:
-        """If this returns True package_env and package_tox_env_type configurations must be defined"""
+        """If this returns True package_env and package_tox_env_type configurations must be defined."""
         self.core.add_config(
             keys=["no_package", "skipsdist"],
             of_type=bool,
             default=False,
             desc="is there any packaging involved in this project",
         )
         core_no_package: bool = self.core["no_package"]
```

### Comparing `tox-4.6.0/src/tox/tox_env/util.py` & `tox-4.6.1/src/tox/tox_env/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import cast
+from typing import TYPE_CHECKING, cast
 
-from tox.config.sets import CoreConfigSet, EnvConfigSet
+if TYPE_CHECKING:
+    from tox.config.sets import CoreConfigSet, EnvConfigSet
 
 
 def add_change_dir_conf(config: EnvConfigSet, core: CoreConfigSet) -> None:
     def _post_process_change_dir(value: Path) -> Path:
         if not value.is_absolute():
             value = (core["tox_root"] / value).resolve()
         return value
 
     config.add_config(
         keys=["change_dir", "changedir"],
         of_type=Path,
-        default=lambda conf, name: cast(Path, conf.core["tox_root"]),  # noqa: U100
+        default=lambda conf, name: cast(Path, conf.core["tox_root"]),  # noqa: ARG005
         desc="change to this working directory when executing the test command",
         post_process=_post_process_change_dir,
     )
 
 
 __all__ = [
     "add_change_dir_conf",
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/api.py` & `tox-4.6.1/src/tox/tox_env/python/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-"""
-Declare the abstract base class for tox environments that handle the Python language.
-"""
+"""Declare the abstract base class for tox environments that handle the Python language."""
 from __future__ import annotations
 
 import logging
 import re
 import sys
 from abc import ABC, abstractmethod
-from pathlib import Path
-from typing import Any, List, NamedTuple, cast
+from typing import TYPE_CHECKING, Any, List, NamedTuple, cast
 
 from virtualenv.discovery.py_spec import PythonSpec
 
-from tox.config.main import Config
 from tox.tox_env.api import ToxEnv, ToxEnvCreateArgs
 from tox.tox_env.errors import Fail, Recreate, Skip
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.config.main import Config
+
 
 class VersionInfo(NamedTuple):
     major: int
     minor: int
     micro: int
     releaselevel: str
     serial: int
@@ -128,37 +129,38 @@
                 ],
             )
         binary_extension_build = ["PKG_CONFIG", "PKG_CONFIG_PATH", "PKG_CONFIG_SYSROOT_DIR"]
         env.extend(binary_extension_build)  # used by binary extensions during installation
         env.extend(["REQUESTS_CA_BUNDLE"])
         return env
 
-    def default_base_python(self, conf: Config, env_name: str | None) -> list[str]:  # noqa: U100
+    def default_base_python(self, conf: Config, env_name: str | None) -> list[str]:  # noqa: ARG002
         base_python = None if env_name is None else self.extract_base_python(env_name)
         return [sys.executable if base_python is None else base_python]
 
     @classmethod
     def extract_base_python(cls, env_name: str) -> str | None:
         candidates: list[str] = []
         for factor in env_name.split("-"):
             match = PY_FACTORS_RE.match(factor)
             if match:
                 candidates.append(factor)
         if candidates:
             if len(candidates) > 1:
-                raise ValueError(f"conflicting factors {', '.join(candidates)} in {env_name}")
+                msg = f"conflicting factors {', '.join(candidates)} in {env_name}"
+                raise ValueError(msg)
             return next(iter(candidates))
         return None
 
     @classmethod
     def _validate_base_python(
         cls,
         env_name: str,
         base_pythons: list[str],
-        ignore_base_python_conflict: bool,
+        ignore_base_python_conflict: bool,  # noqa: FBT001
     ) -> list[str]:
         env_base_python = cls.extract_base_python(env_name)
         if env_base_python is not None:
             spec_name = PythonSpec.from_string_spec(env_base_python)
             for base_python in base_pythons:
                 spec_base = PythonSpec.from_string_spec(base_python)
                 if any(
@@ -179,24 +181,24 @@
         If we have the python we just need to look at the last path under prefix.
         E.g., Debian derivatives change the site-packages to dist-packages, so we need to fix it for site-packages.
         """
         raise NotImplementedError
 
     @abstractmethod
     def env_python(self) -> Path:
-        """The python executable within the tox environment"""
+        """The python executable within the tox environment."""
         raise NotImplementedError
 
     @abstractmethod
     def env_bin_dir(self) -> Path:
-        """The binary folder within the tox environment"""
+        """The binary folder within the tox environment."""
         raise NotImplementedError
 
     def _setup_env(self) -> None:
-        """setup a virtual python environment"""
+        """Setup a virtual python environment."""
         super()._setup_env()
         self.ensure_python_env()
         self._paths = self.prepend_env_var_path()  # now that the environment exist we can add them to the path
 
     def ensure_python_env(self) -> None:
         conf = self.python_cache()
         with self.cache.compare(conf, Python.__name__) as (eq, old):
@@ -220,15 +222,15 @@
         return f'python {", ".join(result)}'
 
     @abstractmethod
     def prepend_env_var_path(self) -> list[Path]:
         raise NotImplementedError
 
     def _done_with_setup(self) -> None:
-        """called when setup is done"""
+        """Called when setup is done."""
         super()._done_with_setup()
         if self.journal or self.options.list_dependencies:
             outcome = self.installer.installed()
             if self.journal:
                 self.journal["installed_packages"] = outcome
             if self.options.list_dependencies:
                 logging.warning(",".join(outcome))
@@ -236,27 +238,28 @@
     def python_cache(self) -> dict[str, Any]:
         return {
             "version_info": list(self.base_python.version_info),
         }
 
     @property
     def base_python(self) -> PythonInfo:
-        """Resolve base python"""
+        """Resolve base python."""
         base_pythons: list[str] = self.conf["base_python"]
 
         if self._base_python_searched is False:
             self._base_python_searched = True
             self._base_python = self._get_python(base_pythons)
             if self._base_python is not None and self.journal:
                 value = self._get_env_journal_python()
                 self.journal["python"] = value
 
         if self._base_python is None:
             if self.core["skip_missing_interpreters"]:
-                raise Skip(f"could not find python interpreter with spec(s): {', '.join(base_pythons)}")
+                msg = f"could not find python interpreter with spec(s): {', '.join(base_pythons)}"
+                raise Skip(msg)
             raise NoInterpreter(base_pythons)
 
         return cast(PythonInfo, self._base_python)
 
     def _get_env_journal_python(self) -> dict[str, Any]:
         return {
             "implementation": self.base_python.implementation,
@@ -273,14 +276,14 @@
 
     @abstractmethod
     def create_python_env(self) -> None:
         raise NotImplementedError
 
 
 class NoInterpreter(Fail):
-    """could not find interpreter"""
+    """could not find interpreter."""
 
     def __init__(self, base_pythons: list[str]) -> None:
         self.base_pythons = base_pythons
 
     def __str__(self) -> str:
         return f"could not find python interpreter matching any of the specs {', '.join(self.base_pythons)}"
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/package.py` & `tox-4.6.1/src/tox/tox_env/python/package.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,63 +1,64 @@
-"""
-A tox build environment that handles Python packages.
-"""
+"""A tox build environment that handles Python packages."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from pathlib import Path
 from typing import TYPE_CHECKING, Any, Generator, Iterator, List, Sequence, cast
 
 from packaging.requirements import Requirement
 
-from ...config.sets import EnvConfigSet
-from ..api import ToxEnvCreateArgs
-from ..errors import Skip
-from ..package import Package, PackageToxEnv, PathPackage
-from ..runner import RunToxEnv
+from tox.tox_env.errors import Skip
+from tox.tox_env.package import Package, PackageToxEnv, PathPackage
+
 from .api import NoInterpreter, Python
-from .pip.req_file import PythonDeps
 
 if TYPE_CHECKING:
+    from pathlib import Path
+
     from tox.config.main import Config
+    from tox.config.sets import EnvConfigSet
+    from tox.tox_env.api import ToxEnvCreateArgs
+    from tox.tox_env.runner import RunToxEnv
+
+    from .pip.req_file import PythonDeps
 
 
 class PythonPackage(Package):
-    """python package"""
+    """python package."""
 
 
 class PythonPathPackageWithDeps(PathPackage):
     def __init__(self, path: Path, deps: Sequence[Any]) -> None:
         super().__init__(path=path)
         self.deps: Sequence[Package] = deps
 
 
 class WheelPackage(PythonPathPackageWithDeps):
-    """wheel package"""
+    """wheel package."""
 
 
 class SdistPackage(PythonPathPackageWithDeps):
-    """sdist package"""
+    """sdist package."""
 
 
 class EditableLegacyPackage(PythonPathPackageWithDeps):
-    """legacy editable package"""
+    """legacy editable package."""
 
 
 class EditablePackage(PythonPathPackageWithDeps):
-    """PEP-660 editable package"""
+    """PEP-660 editable package."""
 
 
 class PythonPackageToxEnv(Python, PackageToxEnv, ABC):
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
         self._wheel_build_envs: dict[str, PythonPackageToxEnv] = {}
         super().__init__(create_args)
 
     def _setup_env(self) -> None:
-        """setup the tox environment"""
+        """Setup the tox environment."""
         super()._setup_env()
         self._install(self.requires(), PythonPackageToxEnv.__name__, "requires")
         self._install(self.conf["deps"], PythonPackageToxEnv.__name__, "deps")
 
     @abstractmethod
     def requires(self) -> tuple[Requirement, ...] | PythonDeps:
         raise NotImplementedError
@@ -75,30 +76,31 @@
         if (
             not isinstance(run_env, Python)
             or run_env.conf["package"] not in {"wheel", "editable"}
             or "wheel_build_env" in run_env.conf
         ):
             return
 
-        def default_wheel_tag(conf: Config, env_name: str | None) -> str:  # noqa: U100
+        def default_wheel_tag(conf: Config, env_name: str | None) -> str:  # noqa: ARG001
             # https://www.python.org/dev/peps/pep-0427/#file-name-convention
             # when building wheels we need to ensure that the built package is compatible with the target env
             # compatibility is documented within https://www.python.org/dev/peps/pep-0427/#file-name-convention
             # a wheel tag example: {distribution}-{version}(-{build tag})?-{python tag}-{abi tag}-{platform tag}.whl
             # python only code are often compatible at major level (unless universal wheel in which case both 2/3)
             # c-extension codes are trickier, but as of today both poetry/setuptools uses pypa/wheels logic
             # https://github.com/pypa/wheel/blob/master/src/wheel/bdist_wheel.py#L234-L280
             try:
                 run_py = cast(Python, run_env).base_python
             except NoInterpreter:
                 run_py = None
 
             if run_py is None:
                 base = ",".join(run_env.conf["base_python"])
-                raise Skip(f"could not resolve base python with {base}")
+                msg = f"could not resolve base python with {base}"
+                raise Skip(msg)
 
             default_pkg_py = self.base_python
             if (
                 default_pkg_py.version_no_dot == run_py.version_no_dot
                 and default_pkg_py.impl_lower == run_py.impl_lower
             ):
                 return self.conf.name
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/runner.py` & `tox-4.6.1/src/tox/tox_env/python/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""
-A tox run environment that handles the Python language.
-"""
+"""A tox run environment that handles the Python language."""
 from __future__ import annotations
 
 from functools import partial
-from typing import Set
+from typing import TYPE_CHECKING, Set
 
 from packaging.utils import canonicalize_name
 
+from tox.config.loader.str_convert import StrConvert
 from tox.report import HandledError
 from tox.tox_env.errors import Skip
-from tox.tox_env.package import Package
 from tox.tox_env.python.pip.req_file import PythonDeps
+from tox.tox_env.runner import RunToxEnv
 
-from ...config.loader.str_convert import StrConvert
-from ..api import ToxEnvCreateArgs
-from ..runner import RunToxEnv
 from .api import Python
 
+if TYPE_CHECKING:
+    from tox.tox_env.api import ToxEnvCreateArgs
+    from tox.tox_env.package import Package
+
 
 class PythonRun(Python, RunToxEnv):
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
         super().__init__(create_args)
 
     def register_config(self) -> None:
         super().register_config()
@@ -30,15 +30,15 @@
             keys="deps",
             of_type=PythonDeps,
             factory=partial(PythonDeps.factory, root),
             default=PythonDeps("", root),
             desc="Name of the python dependencies as specified by PEP-440",
         )
 
-        def skip_missing_interpreters_post_process(value: bool) -> bool:
+        def skip_missing_interpreters_post_process(value: bool) -> bool:  # noqa: FBT001
             if getattr(self.options, "skip_missing_interpreters", "config") != "config":
                 return StrConvert().to_bool(self.options.skip_missing_interpreters)
             return value
 
         self.core.add_config(
             keys=["skip_missing_interpreters"],
             default=True,
@@ -95,27 +95,29 @@
         return "sdist"
 
     @property
     def pkg_type(self) -> str:
         pkg_type: str = self.conf["package"]
         if pkg_type not in self._package_types:
             values = ", ".join(self._package_types)
-            raise HandledError(f"invalid package config type {pkg_type} requested, must be one of {values}")
+            msg = f"invalid package config type {pkg_type} requested, must be one of {values}"
+            raise HandledError(msg)
         return pkg_type
 
     def _setup_env(self) -> None:
         super()._setup_env()
         self._install_deps()
 
     def _install_deps(self) -> None:
         requirements_file: PythonDeps = self.conf["deps"]
         self._install(requirements_file, PythonRun.__name__, "deps")
 
     def _build_packages(self) -> list[Package]:
         package_env = self.package_env
-        assert package_env is not None
+        assert package_env is not None  # noqa: S101
         with package_env.display_context(self._has_display_suspended):
             try:
                 packages = package_env.perform_packaging(self.conf)
             except Skip as exception:
-                raise Skip(f"{exception.args[0]} for package environment {package_env.conf['env_name']}")
+                msg = f"{exception.args[0]} for package environment {package_env.conf['env_name']}"
+                raise Skip(msg) from exception
         return packages
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/pip/pip_install.py` & `tox-4.6.1/src/tox/tox_env/python/pip/pip_install.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
 
 import logging
 from collections import defaultdict
 from pathlib import Path
-from typing import Any, Callable, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 from packaging.requirements import Requirement
 
-from tox.config.main import Config
 from tox.config.types import Command
 from tox.execute.request import StdinSource
 from tox.tox_env.errors import Fail, Recreate
 from tox.tox_env.installer import Installer
-from tox.tox_env.package import PathPackage
 from tox.tox_env.python.api import Python
 from tox.tox_env.python.package import EditableLegacyPackage, EditablePackage, SdistPackage, WheelPackage
 from tox.tox_env.python.pip.req_file import PythonDeps
 
+if TYPE_CHECKING:
+    from tox.config.main import Config
+    from tox.tox_env.package import PathPackage
+
 
 class Pip(Installer[Python]):
-    """Pip is a python installer that can install packages as defined by PEP-508 and PEP-517"""
+    """Pip is a python installer that can install packages as defined by PEP-508 and PEP-517."""
 
-    def __init__(self, tox_env: Python, with_list_deps: bool = True) -> None:
+    def __init__(self, tox_env: Python, with_list_deps: bool = True) -> None:  # noqa: FBT001, FBT002
         self._with_list_deps = with_list_deps
         super().__init__(tox_env)
 
     def _register_config(self) -> None:
         self._env.conf.add_config(
             keys=["pip_pre"],
             of_type=bool,
@@ -55,16 +57,16 @@
             self._env.conf.add_config(
                 keys=["list_dependencies_command"],
                 of_type=Command,
                 default=Command(["python", "-m", "pip", "freeze", "--all"]),
                 desc="command used to list isntalled packages",
             )
 
-    def default_install_command(self, conf: Config, env_name: str | None) -> Command:  # noqa: U100
-        isolated_flag = "-E" if self._env.base_python.version_info.major == 2 else "-I"
+    def default_install_command(self, conf: Config, env_name: str | None) -> Command:  # noqa: ARG002
+        isolated_flag = "-E" if self._env.base_python.version_info.major == 2 else "-I"  # noqa: PLR2004
         cmd = Command(["python", isolated_flag, "-m", "pip", "install", "{opts}", "{packages}"])
         return self.post_process_install_command(cmd)
 
     def post_process_install_command(self, cmd: Command) -> Command:
         install_command = cmd.args
         pip_pre: bool = self._env.conf["pip_pre"]
         try:
@@ -87,15 +89,15 @@
 
     def install(self, arguments: Any, section: str, of_type: str) -> None:
         if isinstance(arguments, PythonDeps):
             self._install_requirement_file(arguments, section, of_type)
         elif isinstance(arguments, Sequence):
             self._install_list_of_deps(arguments, section, of_type)
         else:
-            logging.warning(f"pip cannot install {arguments!r}")
+            logging.warning("pip cannot install %r", arguments)
             raise SystemExit(1)
 
     def constraints_file(self) -> Path:
         return Path(self._env.env_dir) / "constraints.txt"
 
     @property
     def constrain_package_deps(self) -> bool:
@@ -105,15 +107,16 @@
     def use_frozen_constraints(self) -> bool:
         return bool(self._env.conf["use_frozen_constraints"])
 
     def _install_requirement_file(self, arguments: PythonDeps, section: str, of_type: str) -> None:
         try:
             new_options, new_reqs = arguments.unroll()
         except ValueError as exception:
-            raise Fail(f"{exception} for tox env py within deps")
+            msg = f"{exception} for tox env py within deps"
+            raise Fail(msg) from exception
         new_requirements: list[str] = []
         new_constraints: list[str] = []
         for req in new_reqs:
             (new_constraints if req.startswith("-c ") else new_requirements).append(req)
         constraint_options = {
             "constrain_package_deps": self.constrain_package_deps,
             "use_frozen_constraints": self.use_frozen_constraints,
@@ -128,15 +131,16 @@
         with self._env.cache.compare(new, section, of_type) as (eq, old):
             if not eq:  # pragma: no branch
                 if old is not None:
                     self._recreate_if_diff("install flag(s)", new_options, old["options"], lambda i: i)
                     self._recreate_if_diff("constraint(s)", new_constraints, old["constraints"], lambda i: i[3:])
                     missing_requirement = set(old["requirements"]) - set(new_requirements)
                     if missing_requirement:
-                        raise Recreate(f"requirements removed: {' '.join(missing_requirement)}")
+                        msg = f"requirements removed: {' '.join(missing_requirement)}"
+                        raise Recreate(msg)
                     old_constraint_options = old.get("constraint_options")
                     if old_constraint_options != constraint_options:
                         msg = f"constraint options changed: old={old_constraint_options} new={constraint_options}"
                         raise Recreate(msg)
                 args = arguments.as_root_args
                 if args:  # pragma: no branch
                     self._execute_installer(args, of_type)
@@ -148,17 +152,18 @@
     def _recreate_if_diff(of_type: str, new_opts: list[str], old_opts: list[str], fmt: Callable[[str], str]) -> None:
         if old_opts == new_opts:
             return
         removed_opts = set(old_opts) - set(new_opts)
         removed = f" removed {', '.join(sorted(fmt(i) for i in removed_opts))}" if removed_opts else ""
         added_opts = set(new_opts) - set(old_opts)
         added = f" added {', '.join(sorted(fmt(i) for i in added_opts))}" if added_opts else ""
-        raise Recreate(f"changed {of_type}{removed}{added}")
+        msg = f"changed {of_type}{removed}{added}"
+        raise Recreate(msg)
 
-    def _install_list_of_deps(
+    def _install_list_of_deps(  # noqa: C901
         self,
         arguments: Sequence[
             Requirement | WheelPackage | SdistPackage | EditableLegacyPackage | EditablePackage | PathPackage
         ],
         section: str,
         of_type: str,
     ) -> None:
@@ -169,24 +174,25 @@
             elif isinstance(arg, (WheelPackage, SdistPackage, EditablePackage)):
                 groups["req"].extend(str(i) for i in arg.deps)
                 groups["pkg"].append(str(arg.path))
             elif isinstance(arg, EditableLegacyPackage):
                 groups["req"].extend(str(i) for i in arg.deps)
                 groups["dev_pkg"].append(str(arg.path))
             else:
-                logging.warning(f"pip cannot install {arg!r}")
+                logging.warning("pip cannot install %r", arg)
                 raise SystemExit(1)
         req_of_type = f"{of_type}_deps" if groups["pkg"] or groups["dev_pkg"] else of_type
         for value in groups.values():
             value.sort()
         with self._env.cache.compare(groups["req"], section, req_of_type) as (eq, old):
             if not eq:  # pragma: no branch
                 miss = sorted(set(old or []) - set(groups["req"]))
                 if miss:  # no way yet to know what to uninstall here (transitive dependencies?)
-                    raise Recreate(f"dependencies removed: {', '.join(str(i) for i in miss)}")  # pragma: no branch
+                    msg = f"dependencies removed: {', '.join(str(i) for i in miss)}"
+                    raise Recreate(msg)  # pragma: no branch
                 new_deps = sorted(set(groups["req"]) - set(old or []))
                 if new_deps:  # pragma: no branch
                     self._execute_installer(new_deps, req_of_type)
         install_args = ["--force-reinstall", "--no-deps"]
         if groups["pkg"]:
             self._execute_installer(install_args + groups["pkg"], of_type)
         if groups["dev_pkg"]:
@@ -208,18 +214,18 @@
             # freeze installed deps for use as constraints
             self.constraints_file().write_text("\n".join(self.installed()))
 
     def build_install_cmd(self, args: Sequence[str]) -> list[str]:
         try:
             cmd: Command = self._env.conf["install_command"]
         except ValueError as exc:
-            raise Fail(f"unable to determine pip install command: {str(exc)}") from exc
+            msg = f"unable to determine pip install command: {exc!s}"
+            raise Fail(msg) from exc
         install_command = cmd.args
         try:
             opts_at = install_command.index("{packages}")
         except ValueError:
             opts_at = len(install_command)
-        result = install_command[:opts_at] + list(args) + install_command[opts_at + 1 :]
-        return result
+        return install_command[:opts_at] + list(args) + install_command[opts_at + 1 :]
 
 
 __all__ = ("Pip",)
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/pip/req_file.py` & `tox-4.6.1/src/tox/tox_env/python/pip/req_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 import re
-from argparse import ArgumentParser, Namespace
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 from .req.file import ParsedRequirement, ReqFileLines, RequirementsFile
 
+if TYPE_CHECKING:
+    from argparse import ArgumentParser, Namespace
+    from pathlib import Path
+
 
 class PythonDeps(RequirementsFile):
     # these options are valid in requirements.txt, but not via pip cli and
     # thus cannot be used in the testenv `deps` list
     _illegal_options = ["hash"]
 
-    def __init__(self, raw: str, root: Path):
+    def __init__(self, raw: str, root: Path) -> None:
         super().__init__(root / "tox.ini", constraint=False)
         self._raw = self._normalize_raw(raw)
         self._unroll: tuple[list[str], list[str]] | None = None
         self._req_parser_: RequirementsFile | None = None
 
     def _extend_parser(self, parser: ArgumentParser) -> None:
         parser.add_argument("--no-deps", action="store_true", dest="no_deps", default=False)
@@ -45,52 +48,58 @@
 
     def _is_url_self(self, url: str) -> bool:
         return url == str(self._path)
 
     def _pre_process(self, content: str) -> ReqFileLines:
         for at, line in super()._pre_process(content):
             if line.startswith("-r") or line.startswith("-c") and line[2].isalpha():
-                line = f"{line[0:2]} {line[2:]}"
-            yield at, line
+                found_line = f"{line[0:2]} {line[2:]}"
+            else:
+                found_line = line
+            yield at, found_line
 
     def lines(self) -> list[str]:
         return self._raw.splitlines()
 
     @staticmethod
     def _normalize_raw(raw: str) -> str:
         # a line ending in an unescaped \ is treated as a line continuation and the newline following it is effectively
         # ignored
         raw = "".join(raw.replace("\r", "").split("\\\n"))
         lines: list[str] = []
         for line in raw.splitlines():
             # for tox<4 supporting requirement/constraint files via -rreq.txt/-creq.txt
-            arg_match = next(
-                (
-                    arg
-                    for arg in ONE_ARG
-                    if line.startswith(arg)
-                    and len(line) > len(arg)
-                    and not (line[len(arg)].isspace() or line[len(arg)] == "=")
-                ),
-                None,
-            )
-            if arg_match is not None:
-                line = f"{arg_match} {line[len(arg_match):]}"
-            # escape spaces
-            escape_match = next((e for e in ONE_ARG_ESCAPE if line.startswith(e) and line[len(e)].isspace()), None)
-            if escape_match is not None:
-                # escape not already escaped spaces
-                escaped = re.sub(r"(?<!\\)(\s)", r"\\\1", line[len(escape_match) + 1 :])
-                line = f"{line[:len(escape_match)]} {escaped}"
-            lines.append(line)
+            lines.append(PythonDeps._normalize_line(line))
         adjusted = "\n".join(lines)
         raw = f"{adjusted}\n" if raw.endswith("\\\n") else adjusted  # preserve trailing newline if input has it
         return raw
 
-    def _parse_requirements(self, opt: Namespace, recurse: bool) -> list[ParsedRequirement]:
+    @staticmethod
+    def _normalize_line(line: str) -> str:
+        arg_match = next(
+            (
+                arg
+                for arg in ONE_ARG
+                if line.startswith(arg)
+                and len(line) > len(arg)
+                and not (line[len(arg)].isspace() or line[len(arg)] == "=")
+            ),
+            None,
+        )
+        if arg_match is not None:
+            line = f"{arg_match} {line[len(arg_match):]}"
+        # escape spaces
+        escape_match = next((e for e in ONE_ARG_ESCAPE if line.startswith(e) and line[len(e)].isspace()), None)
+        if escape_match is not None:
+            # escape not already escaped spaces
+            escaped = re.sub(r"(?<!\\)(\s)", r"\\\1", line[len(escape_match) + 1 :])
+            line = f"{line[:len(escape_match)]} {escaped}"
+        return line
+
+    def _parse_requirements(self, opt: Namespace, recurse: bool) -> list[ParsedRequirement]:  # noqa: FBT001
         # check for any invalid options in the deps list
         # (requirements recursively included from other files are not checked)
         requirements = super()._parse_requirements(opt, recurse)
         for req in requirements:
             if req.from_file != str(self.path):
                 continue
             for illegal_option in self._illegal_options:
@@ -99,15 +108,16 @@
                     raise ValueError(msg)
         return requirements
 
     def unroll(self) -> tuple[list[str], list[str]]:
         if self._unroll is None:
             opts_dict = vars(self.options)
             if not self.requirements and opts_dict:
-                raise ValueError("no dependencies")
+                msg = "no dependencies"
+                raise ValueError(msg)
             result_opts: list[str] = [f"{key}={value}" for key, value in opts_dict.items()]
             result_req = [str(req) for req in self.requirements]
             self._unroll = result_opts, result_req
         return self._unroll
 
     @classmethod
     def factory(cls, root: Path, raw: object) -> PythonDeps:
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/pip/req/args.py` & `tox-4.6.1/src/tox/tox_env/python/pip/req/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from argparse import Action, ArgumentParser, ArgumentTypeError, Namespace
 from typing import IO, Any, NoReturn, Sequence
 
 from tox.tox_env.python.pip.req.util import handle_binary_option
 
 
 class _OurArgumentParser(ArgumentParser):
-    def print_usage(self, file: IO[str] | None = None) -> None:  # noqa: U100
+    def print_usage(self, file: IO[str] | None = None) -> None:
         """ """
 
-    def exit(self, status: int = 0, message: str | None = None) -> NoReturn:  # noqa: U100
+    def exit(self, status: int = 0, message: str | None = None) -> NoReturn:  # noqa: A003, ARG002
         message = "" if message is None else message
         msg = message.lstrip(": ").rstrip()
         if msg.startswith("error: "):
             msg = msg[len("error: ") :]
         raise ValueError(msg)
 
 
@@ -63,54 +63,54 @@
         raise ArgumentTypeError(value)
     return value
 
 
 class AddSortedUniqueAction(Action):
     def __call__(
         self,
-        parser: ArgumentParser,  # noqa: U100
+        parser: ArgumentParser,  # noqa: ARG002
         namespace: Namespace,
         values: str | Sequence[Any] | None,
-        option_string: str | None = None,  # noqa: U100
+        option_string: str | None = None,  # noqa: ARG002
     ) -> None:
         if getattr(namespace, self.dest, None) is None:
             setattr(namespace, self.dest, [])
         current = getattr(namespace, self.dest)
         if values not in current:
             bisect.insort(current, values)
 
 
 class AddUniqueAction(Action):
     def __call__(
         self,
-        parser: ArgumentParser,  # noqa: U100
+        parser: ArgumentParser,  # noqa: ARG002
         namespace: Namespace,
         values: str | Sequence[Any] | None,
-        option_string: str | None = None,  # noqa: U100
+        option_string: str | None = None,  # noqa: ARG002
     ) -> None:
         if getattr(namespace, self.dest, None) is None:
             setattr(namespace, self.dest, [])
         current = getattr(namespace, self.dest)
         if values not in current:
             current.append(values)
 
 
 class BinaryAction(Action):
     def __call__(
         self,
-        parser: ArgumentParser,  # noqa: U100
+        parser: ArgumentParser,  # noqa: ARG002
         namespace: Namespace,
         values: str | Sequence[Any] | None,
-        option_string: str | None = None,  # noqa: U100
+        option_string: str | None = None,  # noqa: ARG002
     ) -> None:
         if getattr(namespace, "no_binary", None) is None:
             namespace.no_binary = set()
         if getattr(namespace, "only_binary", None) is None:
             namespace.only_binary = set()
 
         args = (
             (namespace.no_binary, namespace.only_binary)
             if self.dest == "no_binary"
             else (namespace.only_binary, namespace.no_binary)
         )
-        assert values is not None
+        assert values is not None  # noqa: S101
         handle_binary_option(values[0], *args)
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/pip/req/file.py` & `tox-4.6.1/src/tox/tox_env/python/pip/req/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Adapted from the pip code base"""
+"""Adapted from the pip code base."""
 from __future__ import annotations
 
 import os
 import re
 import shlex
 import sys
 import urllib.parse
@@ -27,28 +27,28 @@
 _EXTRA_ELEMENT = re.compile(r"[a-zA-Z0-9]*[-._a-zA-Z0-9]")
 ReqFileLines = Iterator[Tuple[int, str]]
 
 DEFAULT_INDEX_URL = "https://pypi.org/simple"
 
 
 class ParsedRequirement:
-    def __init__(self, req: str, options: dict[str, Any], from_file: str, lineno: int) -> None:
+    def __init__(self, req: str, options: dict[str, Any], from_file: str, lineno: int) -> None:  # noqa: PLR0912
         req = req.encode("utf-8").decode("utf-8")
         try:
             self._requirement: Requirement | Path | str = Requirement(req)
         except InvalidRequirement:
             if is_url(req) or any(req.startswith(f"{v}+") and is_url(req[len(v) + 1 :]) for v in VCS):
                 self._requirement = req
             else:
                 root = Path(from_file).parent
                 extras: list[str] = []
                 match = _EXTRA_PATH.fullmatch(Path(req).name)
                 if match:
                     for extra in match.group(2).split(","):
-                        extra = extra.strip()
+                        extra = extra.strip()  # noqa: PLW2901
                         if not extra:
                             continue
                         if not _EXTRA_ELEMENT.fullmatch(extra):
                             extras = []
                             path = root / req
                             break
                         extras.append(extra)
@@ -106,15 +106,22 @@
     def as_args(self) -> Iterator[str]:
         if self.options.get("is_editable"):
             yield "-e"
         yield str(self._requirement)
 
 
 class ParsedLine:
-    def __init__(self, filename: str, lineno: int, args: str, opts: Namespace, constraint: bool) -> None:
+    def __init__(  # noqa: PLR0913
+        self,
+        filename: str,
+        lineno: int,
+        args: str,
+        opts: Namespace,
+        constraint: bool,  # noqa: FBT001
+    ) -> None:
         self.filename = filename
         self.lineno = lineno
         self.opts = opts
         self.constraint = constraint
         if args:
             self.is_requirement = True
             self.is_editable = False
@@ -125,15 +132,15 @@
             # We don't support multiple -e on one line
             self.requirement = opts.editables[0]
         else:
             self.is_requirement = False
 
 
 class RequirementsFile:
-    def __init__(self, path: Path, constraint: bool) -> None:
+    def __init__(self, path: Path, constraint: bool) -> None:  # noqa: FBT001
         self._path = path
         self._is_constraint: bool = constraint
         self._opt = Namespace()
         self._requirements: list[ParsedRequirement] | None = None
         self._as_root_args: list[str] | None = None
         self._parser_private: ArgumentParser | None = None
 
@@ -165,22 +172,22 @@
     @property
     def _parser(self) -> ArgumentParser:
         if self._parser_private is None:
             self._parser_private = build_parser()
             self._extend_parser(self._parser_private)
         return self._parser_private
 
-    def _extend_parser(self, parser: ArgumentParser) -> None:  # noqa: U100
+    def _extend_parser(self, parser: ArgumentParser) -> None:
         ...
 
     def _ensure_requirements_parsed(self) -> None:
         if self._requirements is None:
             self._requirements = self._parse_requirements(opt=self._opt, recurse=True)
 
-    def _parse_requirements(self, opt: Namespace, recurse: bool) -> list[ParsedRequirement]:
+    def _parse_requirements(self, opt: Namespace, recurse: bool) -> list[ParsedRequirement]:  # noqa: FBT001
         result, found = [], set()
         for parsed_line in self._parse_and_recurse(str(self._path), self.is_constraint, recurse):
             if parsed_line.is_requirement:
                 parsed_req = self._handle_requirement_line(parsed_line)
                 key = str(parsed_req)
                 if key not in found:
                     found.add(key)
@@ -195,72 +202,77 @@
         between = of_type, str(line.requirement).lower(), str(line.options)
         if "is_constraint" in line.options:
             return 2, between
         if "is_editable" in line.options:
             return 1, between
         return 0, between
 
-    def _parse_and_recurse(self, filename: str, constraint: bool, recurse: bool) -> Iterator[ParsedLine]:
+    def _parse_and_recurse(
+        self,
+        filename: str,
+        constraint: bool,  # noqa: FBT001
+        recurse: bool,  # noqa: FBT001
+    ) -> Iterator[ParsedLine]:
         for line in self._parse_file(filename, constraint):
             if not line.is_requirement and (line.opts.requirements or line.opts.constraints):
                 if line.opts.requirements:  # parse a nested requirements file
                     nested_constraint, req_path = False, line.opts.requirements[0]
                 else:
                     nested_constraint, req_path = True, line.opts.constraints[0]
                 if _SCHEME_RE.search(filename):  # original file is over http
                     req_path = urllib.parse.urljoin(filename, req_path)  # do a url join so relative paths work
                 elif not _SCHEME_RE.search(req_path):  # original file and nested file are paths
-                    # do a join so relative paths work
-                    req_path = os.path.join(os.path.dirname(filename), req_path)
+                    req_path = str(Path(filename).parent / req_path)  # do a join so relative paths work
                 if recurse:
-                    yield from self._req_parser._parse_and_recurse(req_path, nested_constraint, recurse)
+                    yield from self._req_parser._parse_and_recurse(req_path, nested_constraint, recurse)  # noqa: SLF001
                 else:
                     line.filename = req_path
                     yield line
             else:
                 yield line
 
-    def _parse_file(self, url: str, constraint: bool) -> Iterator[ParsedLine]:
+    def _parse_file(self, url: str, constraint: bool) -> Iterator[ParsedLine]:  # noqa: FBT001
         content = self._get_file_content(url)
         for line_number, line in self._pre_process(content):
             args_str, opts = self._parse_line(line)
             yield ParsedLine(url, line_number, args_str, opts, constraint)
 
     def _get_file_content(self, url: str) -> str:
         """
         Gets the content of a file; it may be a filename, file: URL, or http: URL.  Returns (location, content).
         Content is unicode. Respects # -*- coding: declarations on the retrieved files.
 
         :param url:         File path or url.
         """
         scheme = get_url_scheme(url)
         if scheme in ["http", "https"]:
-            with urlopen(url) as response:
+            with urlopen(url) as response:  # noqa: S310
                 text = self._read_decode(response)
                 return text
         elif scheme == "file":
             url = url_to_path(url)
         try:
-            with open(url, "rb") as file_handler:
+            with Path(url).open("rb") as file_handler:
                 text = self._read_decode(file_handler)
         except OSError as exc:
-            raise ValueError(f"Could not open requirements file {url}: {exc}") from exc
+            msg = f"Could not open requirements file {url}: {exc}"
+            raise ValueError(msg) from exc
         return text
 
     @staticmethod
     def _read_decode(file_handler: IO[bytes]) -> str:
         raw = file_handler.read()
         if not raw:
             return ""
         codec = chardet.detect(raw)["encoding"]
-        text = raw.decode(codec)
-        return text
+        return raw.decode(codec)
 
     def _pre_process(self, content: str) -> ReqFileLines:
-        """Split, filter, and join lines, and return a line iterator
+        """
+        Split, filter, and join lines, and return a line iterator.
 
         :param content: the content of the requirements file
         """
         lines_enum: ReqFileLines = enumerate(content.splitlines(), start=1)
         lines_enum = self._join_lines(lines_enum)
         lines_enum = self._ignore_comments(lines_enum)
         lines_enum = self._expand_env_variables(lines_enum)
@@ -282,15 +294,20 @@
         if line.constraint:
             req_options["is_constraint"] = line.constraint
         hash_values = getattr(line.opts, "hash", [])
         if hash_values:
             req_options["hash"] = hash_values
         return ParsedRequirement(line.requirement, req_options, line.filename, line.lineno)
 
-    def _merge_option_line(self, base_opt: Namespace, opt: Namespace, filename: str) -> None:  # noqa: C901
+    def _merge_option_line(  # noqa: C901, PLR0912, PLR0915
+        self,
+        base_opt: Namespace,
+        opt: Namespace,
+        filename: str,
+    ) -> None:
         # percolate options upward
         if opt.requirements:
             if not hasattr(base_opt, "requirements"):
                 base_opt.requirements = []
             if opt.requirements[0] not in base_opt.requirements:
                 base_opt.requirements.append(opt.requirements[0])
         if opt.constraints:
@@ -317,23 +334,22 @@
         if opt.extra_index_url:
             if not getattr(base_opt, "index_url", []):
                 base_opt.index_url = [DEFAULT_INDEX_URL]
             for url in opt.extra_index_url:
                 if url not in base_opt.index_url:
                     base_opt.index_url.extend(opt.extra_index_url)
         if opt.find_links:
-            # FIXME: it would be nice to keep track of the source of the find_links: support a find-links local path
             # relative to a requirements file.
             if not hasattr(base_opt, "find_links"):
                 base_opt.find_links = []
             value = opt.find_links[0]
-            req_dir = os.path.dirname(os.path.abspath(filename))
-            relative_to_reqs_file = os.path.join(req_dir, value)
-            if os.path.exists(relative_to_reqs_file):
-                value = relative_to_reqs_file  # pragma: no cover
+            req_dir = Path(filename).absolute().parent
+            relative_to_reqs_file = req_dir / value
+            if os.path.exists(str(relative_to_reqs_file)):  # noqa: PTH110 # Path.exists fails on win32 <=3.7 with URI
+                value = str(relative_to_reqs_file)  # pragma: no cover
             if value not in base_opt.find_links:
                 base_opt.find_links.append(value)
         if opt.pre:
             base_opt.pre = True
         if opt.prefer_binary:
             base_opt.prefer_binary = True
         for host in opt.trusted_host or []:
@@ -354,92 +370,92 @@
         """
         tokens = line.split(" ")
         args = []
         options = tokens[:]
         for token in tokens:
             if token.startswith("-"):  # both `-` and `--` accepted
                 break
-            else:
-                args.append(token)
-                options.pop(0)
+            args.append(token)
+            options.pop(0)
         return " ".join(args).strip(), " ".join(options)
 
     @staticmethod
     def _join_lines(lines_enum: ReqFileLines) -> ReqFileLines:
         """
         Joins a line ending in '\' with the previous line (except when following comments). The joined line takes on the
         index of the first line.
         """
         primary_line_number = None
         new_line: list[str] = []
         for line_number, line in lines_enum:
             if not line.endswith("\\") or _COMMENT_RE.match(line):
                 if _COMMENT_RE.match(line):
-                    line = f" {line}"  # this ensures comments are always matched later
+                    line = f" {line}"  # noqa: PLW2901 # this ensures comments are always matched later
                 if new_line:
                     new_line.append(line)
-                    assert primary_line_number is not None
+                    assert primary_line_number is not None  # noqa: S101
                     yield primary_line_number, "".join(new_line)
                     new_line = []
                 else:
                     yield line_number, line
             else:
                 if not new_line:  # pragma: no branch
                     primary_line_number = line_number
                 new_line.append(line.strip("\\"))
         # last line contains \
         if new_line:
-            assert primary_line_number is not None
+            assert primary_line_number is not None  # noqa: S101
             yield primary_line_number, "".join(new_line)
 
     @staticmethod
     def _ignore_comments(lines_enum: ReqFileLines) -> ReqFileLines:
         """Strips comments and filter empty lines."""
         for line_number, line in lines_enum:
-            line = _COMMENT_RE.sub("", line)
-            line = line.strip()
-            if line:
-                yield line_number, line
+            processed_line = _COMMENT_RE.sub("", line).strip()
+            if processed_line:
+                yield line_number, processed_line
 
     @staticmethod
     def _expand_env_variables(lines_enum: ReqFileLines) -> ReqFileLines:
-        """Replace all environment variables that can be retrieved via `os.getenv`.
+        """
+        Replace all environment variables that can be retrieved via `os.getenv`.
 
         The only allowed format for environment variables defined in the requirement file is `${MY_VARIABLE_1}` to
         ensure two things:
 
         1. Strings that contain a `$` aren't accidentally (partially) expanded.
         2. Ensure consistency across platforms for requirement files.
 
         These points are the result of a discussion on the `github pull request #3514
         <https://github.com/pypa/pip/pull/3514>`_. Valid characters in variable names follow the `POSIX standard
         <http://pubs.opengroup.org/onlinepubs/9699919799/>`_ and are limited to uppercase letter, digits and the `_`.
         """
         for line_number, line in lines_enum:
-            for env_var, var_name in _ENV_VAR_RE.findall(line):
+            expanded_line = line
+            for env_var, var_name in _ENV_VAR_RE.findall(expanded_line):
                 value = os.getenv(var_name)
                 if not value:
                     continue
-                line = line.replace(env_var, value)
-            yield line_number, line
+                expanded_line = expanded_line.replace(env_var, value)
+            yield line_number, expanded_line
 
     @property
     def as_root_args(self) -> list[str]:
         if self._as_root_args is None:
             opt = Namespace()
             result: list[str] = []
             for req in self._parse_requirements(opt=opt, recurse=False):
                 result.extend(req.as_args())
             option_args = self._option_to_args(opt)
             result.extend(option_args)
 
             self._as_root_args = result
         return self._as_root_args
 
-    def _option_to_args(self, opt: Namespace) -> list[str]:
+    def _option_to_args(self, opt: Namespace) -> list[str]:  # noqa: C901, PLR0912
         result: list[str] = []
         for req in getattr(opt, "requirements", []):
             result.extend(("-r", req))
         for req in getattr(opt, "constraints", []):
             result.extend(("-c", req))
         index_url = getattr(opt, "index_url", None)
         if index_url is not None:
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/pip/req/util.py` & `tox-4.6.1/src/tox/tox_env/python/pip/req/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Borrowed from the pip code base"""
+"""Borrowed from the pip code base."""
 from __future__ import annotations
 
 from urllib.parse import urlsplit
 from urllib.request import url2pathname
 
 from packaging.utils import canonicalize_name
 
 VCS = ["ftp", "ssh", "git", "hg", "bzr", "sftp", "svn"]
-VALID_SCHEMAS = ["http", "https", "file"] + VCS
+VALID_SCHEMAS = ["http", "https", "file", *VCS]
 
 
 def is_url(name: str) -> bool:
     return get_url_scheme(name) in VALID_SCHEMAS
 
 
 def get_url_scheme(url: str) -> str | None:
@@ -21,15 +21,16 @@
 
 
 def url_to_path(url: str) -> str:
     _, netloc, path, _, _ = urlsplit(url)
     if not netloc or netloc == "localhost":  # According to RFC 8089, same as empty authority.
         netloc = ""
     else:
-        raise ValueError(f"non-local file URIs are not supported on this platform: {url!r}")
+        msg = f"non-local file URIs are not supported on this platform: {url!r}"
+        raise ValueError(msg)
     path = url2pathname(netloc + path)
     return path
 
 
 def handle_binary_option(value: str, target: set[str], other: set[str]) -> None:
     new = value.split(",")
     while ":all:" in new:
@@ -39,10 +40,10 @@
         del new[: new.index(":all:") + 1]
         if ":none:" not in new:
             return
     for name in new:
         if name == ":none:":
             target.clear()
             continue
-        name = canonicalize_name(name)
-        other.discard(name)
-        target.add(name)
+        normalized_name = canonicalize_name(name)
+        other.discard(normalized_name)
+        target.add(normalized_name)
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/virtual_env/api.py` & `tox-4.6.1/src/tox/tox_env/python/virtual_env/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-"""
-Declare the abstract base class for tox environments that handle the Python language via the virtualenv project.
-"""
+"""Declare the abstract base class for tox environments that handle the Python language via the virtualenv project."""
 from __future__ import annotations
 
 import os
 import sys
 from pathlib import Path
-from typing import Any, cast
+from typing import TYPE_CHECKING, Any, cast
 
 from virtualenv import __version__ as virtualenv_version
 from virtualenv import session_via_cli
-from virtualenv.create.creator import Creator
-from virtualenv.run.session import Session
 
 from tox.config.loader.str_convert import StrConvert
-from tox.execute.api import Execute
 from tox.execute.local_sub_process import LocalSubProcessExecutor
+from tox.tox_env.python.api import Python, PythonInfo
 from tox.tox_env.python.pip.pip_install import Pip
 
-from ...api import ToxEnvCreateArgs
-from ..api import Python, PythonInfo
+if TYPE_CHECKING:
+    from virtualenv.create.creator import Creator
+    from virtualenv.run.session import Session
+
+    from tox.execute.api import Execute
+    from tox.tox_env.api import ToxEnvCreateArgs
 
 
 class VirtualEnv(Python):
-    """A python executor that uses the virtualenv project with pip"""
+    """A python executor that uses the virtualenv project with pip."""
 
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
         self._virtualenv_session: Session | None = None
         self._executor: Execute | None = None
         self._installer: Pip | None = None
         super().__init__(create_args)
 
     def register_config(self) -> None:
         super().register_config()
         self.conf.add_config(
             keys=["system_site_packages", "sitepackages"],
             of_type=bool,
-            default=lambda conf, name: StrConvert().to_bool(  # noqa: U100
+            default=lambda conf, name: StrConvert().to_bool(  # noqa: ARG005
                 self.environment_variables.get("VIRTUALENV_SYSTEM_SITE_PACKAGES", "False"),
             ),
             desc="create virtual environments that also have access to globally installed packages.",
         )
         self.conf.add_config(
             keys=["always_copy", "alwayscopy"],
             of_type=bool,
-            default=lambda conf, name: StrConvert().to_bool(  # noqa: U100
+            default=lambda conf, name: StrConvert().to_bool(  # noqa: ARG005
                 self.environment_variables.get(
                     "VIRTUALENV_COPIES",
                     self.environment_variables.get("VIRTUALENV_ALWAYS_COPY", "False"),
                 ),
             ),
             desc="force virtualenv to always copy rather than symlink",
         )
         self.conf.add_config(
             keys=["download"],
             of_type=bool,
-            default=lambda conf, name: StrConvert().to_bool(  # noqa: U100
+            default=lambda conf, name: StrConvert().to_bool(  # noqa: ARG005
                 self.environment_variables.get("VIRTUALENV_DOWNLOAD", "False"),
             ),
             desc="true if you want virtualenv to upgrade pip/wheel/setuptools to the latest version",
         )
 
     @property
     def executor(self) -> Execute:
@@ -124,31 +124,31 @@
     @property
     def creator(self) -> Creator:
         return self.session.creator
 
     def create_python_env(self) -> None:
         self.session.run()
 
-    def _get_python(self, base_python: list[str]) -> PythonInfo | None:  # noqa: U100
+    def _get_python(self, base_python: list[str]) -> PythonInfo | None:  # noqa: ARG002
         # the base pythons are injected into the virtualenv_env_vars, so we don't need to use it here
         try:
             interpreter = self.creator.interpreter
         except RuntimeError:  # if can't find
             return None
         return PythonInfo(
             implementation=interpreter.implementation,
             version_info=interpreter.version_info,
             version=interpreter.version,
-            is_64=(interpreter.architecture == 64),
+            is_64=(interpreter.architecture == 64),  # noqa: PLR2004
             platform=interpreter.platform,
             extra={"executable": Path(interpreter.system_executable).resolve()},
         )
 
     def prepend_env_var_path(self) -> list[Path]:
-        """Paths to add to the executable"""
+        """Paths to add to the executable."""
         # we use the original executable as shims may be somewhere else
         return list(dict.fromkeys((self.creator.bin_dir, self.creator.script_dir)))
 
     def env_site_package_dir(self) -> Path:
         return cast(Path, self.creator.purelib)
 
     def env_python(self) -> Path:
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/virtual_env/runner.py` & `tox-4.6.1/src/tox/tox_env/python/virtual_env/runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-"""
-A tox python environment runner that uses the virtualenv project.
-"""
+"""A tox python environment runner that uses the virtualenv project."""
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 from tox.plugin import impl
-from tox.tox_env.register import ToxEnvRegister
+from tox.tox_env.python.runner import PythonRun
 
-from ..runner import PythonRun
 from .api import VirtualEnv
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.tox_env.register import ToxEnvRegister
+
 
 class VirtualEnvRunner(VirtualEnv, PythonRun):
-    """local file system python virtual environment via the virtualenv package"""
+    """local file system python virtual environment via the virtualenv package."""
 
     @staticmethod
-    def id() -> str:
+    def id() -> str:  # noqa: A003
         return "virtualenv"
 
     @property
     def _package_tox_env_type(self) -> str:
         return "virtualenv-pep-517"
 
     @property
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py` & `tox-4.6.1/src/tox/tox_env/python/virtual_env/package/cmd_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,52 +2,55 @@
 
 import glob
 import shutil
 import sys
 import tarfile
 from functools import partial
 from io import TextIOWrapper
-from os import PathLike
 from pathlib import Path
-from typing import Generator, Iterator, List, cast
+from typing import TYPE_CHECKING, Generator, Iterator, List, cast
 from zipfile import ZipFile
 
 from packaging.requirements import Requirement
 
-from tox.config.sets import EnvConfigSet
 from tox.config.types import Command
 from tox.execute import Outcome
 from tox.plugin import impl
 from tox.session.cmd.run.single import run_command_set
-from tox.tox_env.api import ToxEnvCreateArgs
 from tox.tox_env.errors import Fail
-from tox.tox_env.package import Package, PackageToxEnv
 from tox.tox_env.python.package import PythonPackageToxEnv, SdistPackage, WheelPackage
 from tox.tox_env.python.pip.req_file import PythonDeps
 from tox.tox_env.python.virtual_env.api import VirtualEnv
-from tox.tox_env.register import ToxEnvRegister
-from tox.tox_env.runner import RunToxEnv
 from tox.tox_env.util import add_change_dir_conf
 
 from .pyproject import Pep517VirtualEnvPackager
 from .util import dependencies_with_extras
 
+if TYPE_CHECKING:
+    from os import PathLike
+
+    from tox.config.sets import EnvConfigSet
+    from tox.tox_env.api import ToxEnvCreateArgs
+    from tox.tox_env.package import Package, PackageToxEnv
+    from tox.tox_env.register import ToxEnvRegister
+    from tox.tox_env.runner import RunToxEnv
+
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from importlib.metadata import Distribution
 else:  # pragma: no cover (py38+)
     from importlib_metadata import Distribution
 
 
 class VirtualEnvCmdBuilder(PythonPackageToxEnv, VirtualEnv):
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
         super().__init__(create_args)
         self._sdist_meta_tox_env: Pep517VirtualEnvPackager | None = None
 
     @staticmethod
-    def id() -> str:
+    def id() -> str:  # noqa: A003
         return "virtualenv-cmd-builder"
 
     def register_config(self) -> None:
         super().register_config()
         root = self.core["toxinidir"]
         self.conf.add_config(
             keys="deps",
@@ -83,21 +86,24 @@
         self.setup()
         path: Path | None = getattr(self.options, "install_pkg", None)
         if path is None:  # use install_pkg if specified, otherwise build via commands
             chdir: Path = self.conf["change_dir"]
             ignore_errors: bool = self.conf["ignore_errors"]
             status = run_command_set(self, "commands", chdir, ignore_errors, [])
             if status != Outcome.OK:
-                raise Fail("stopping as failed to build package")
+                msg = "stopping as failed to build package"
+                raise Fail(msg)
             package_glob = self.conf["package_glob"]
             found = glob.glob(package_glob)
             if not found:
-                raise Fail(f"no package found in {package_glob}")
-            elif len(found) != 1:
-                raise Fail(f"found more than one package {', '.join(sorted(found))}")
+                msg = f"no package found in {package_glob}"
+                raise Fail(msg)
+            if len(found) != 1:
+                msg = f"found more than one package {', '.join(sorted(found))}"
+                raise Fail(msg)
             path = Path(found[0])
         return self.extract_install_info(for_env, path)
 
     def extract_install_info(self, for_env: EnvConfigSet, path: Path) -> list[Package]:
         extras: set[str] = for_env["extras"]
         if path.suffix == ".whl":
             wheel_dist = WheelDistribution(path)
@@ -107,29 +113,30 @@
         else:  # must be source distribution
             work_dir = self.env_tmp_dir / "sdist-extract"
             if work_dir.exists():  # pragma: no branch
                 shutil.rmtree(work_dir)  # pragma: no cover
             work_dir.mkdir()
             with tarfile.open(str(path), "r:gz") as tar:
                 tar.extractall(path=str(work_dir))
-            assert self._sdist_meta_tox_env is not None  # the register run env is guaranteed to be called before this
+            # the register run env is guaranteed to be called before this
+            assert self._sdist_meta_tox_env is not None  # noqa: S101
             with self._sdist_meta_tox_env.display_context(self._has_display_suspended):
                 self._sdist_meta_tox_env.root = next(work_dir.iterdir())  # contains a single egg info folder
                 deps = self._sdist_meta_tox_env.get_package_dependencies(for_env)
                 name = self._sdist_meta_tox_env.get_package_name(for_env)
             package = SdistPackage(path, dependencies_with_extras(deps, extras, name))
         return [package]
 
     def register_run_env(self, run_env: RunToxEnv) -> Generator[tuple[str, str], PackageToxEnv, None]:
         yield from super().register_run_env(run_env)
         # in case the outcome is a sdist we'll use this to find out its metadata
         result = yield f"{self.conf.name}_sdist_meta", Pep517VirtualEnvPackager.id()
         self._sdist_meta_tox_env = cast(Pep517VirtualEnvPackager, result)
 
-    def child_pkg_envs(self, run_conf: EnvConfigSet) -> Iterator[PackageToxEnv]:  # noqa: U100
+    def child_pkg_envs(self, run_conf: EnvConfigSet) -> Iterator[PackageToxEnv]:  # noqa: ARG002
         if self._sdist_meta_tox_env is not None:  # pragma: no branch
             yield self._sdist_meta_tox_env
 
 
 class WheelDistribution(Distribution):  # cannot subclass has type Any
     def __init__(self, wheel: Path) -> None:
         self._wheel = wheel
@@ -141,15 +148,16 @@
             with ZipFile(self._wheel) as zip_file:
                 for name in zip_file.namelist():
                     root = name.split("/")[0]
                     if root.endswith(".dist-info"):
                         self._dist_name = root
                         break
                 else:
-                    raise Fail(f"no .dist-info inside {self._wheel}")
+                    msg = f"no .dist-info inside {self._wheel}"
+                    raise Fail(msg)
         return self._dist_name
 
     def read_text(self, filename: str) -> str | None:
         with ZipFile(self._wheel) as zip_file:
             try:
                 with TextIOWrapper(zip_file.open(f"{self.dist_name}/{filename}"), encoding="utf-8") as file_handler:
                     return file_handler.read()
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/virtual_env/package/pyproject.py` & `tox-4.6.1/src/tox/tox_env/python/virtual_env/package/pyproject.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,42 +3,44 @@
 import logging
 import os
 import sys
 from collections import defaultdict
 from contextlib import contextmanager
 from pathlib import Path
 from threading import RLock
-from typing import Any, Dict, Generator, Iterator, NoReturn, Optional, Sequence, cast
+from typing import TYPE_CHECKING, Any, Dict, Generator, Iterator, NoReturn, Optional, Sequence, cast
 
 from cachetools import cached
 from packaging.requirements import Requirement
 from pyproject_api import BackendFailed, CmdStatus, Frontend
 
-from tox.config.sets import EnvConfigSet
-from tox.execute.api import ExecuteStatus
 from tox.execute.pep517_backend import LocalSubProcessPep517Executor
 from tox.execute.request import StdinSource
 from tox.plugin import impl
-from tox.tox_env.api import ToxEnvCreateArgs
 from tox.tox_env.errors import Fail
-from tox.tox_env.package import Package, PackageToxEnv
 from tox.tox_env.python.package import (
     EditableLegacyPackage,
     EditablePackage,
     PythonPackageToxEnv,
     SdistPackage,
     WheelPackage,
 )
-from tox.tox_env.register import ToxEnvRegister
-from tox.tox_env.runner import RunToxEnv
+from tox.tox_env.python.virtual_env.api import VirtualEnv
 from tox.util.file_view import create_session_view
 
-from ..api import VirtualEnv
 from .util import dependencies_with_extras, dependencies_with_extras_from_markers
 
+if TYPE_CHECKING:
+    from tox.config.sets import EnvConfigSet
+    from tox.execute.api import ExecuteStatus
+    from tox.tox_env.api import ToxEnvCreateArgs
+    from tox.tox_env.package import Package, PackageToxEnv
+    from tox.tox_env.register import ToxEnvRegister
+    from tox.tox_env.runner import RunToxEnv
+
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from importlib.metadata import Distribution, PathDistribution
 else:  # pragma: no cover (<py38)
     from importlib_metadata import Distribution, PathDistribution
 
 if sys.version_info >= (3, 11):  # pragma: no cover (py311+)
     import tomllib
@@ -60,16 +62,16 @@
             self,
             result,
             backend_failed.out,
             backend_failed.err,
         )
 
 
-class BuildEditableNotSupported(RuntimeError):
-    """raised when build editable is not supported"""
+class BuildEditableNotSupportedError(RuntimeError):
+    """raised when build editable is not supported."""
 
 
 class ToxCmdStatus(CmdStatus):
     def __init__(self, execute_status: ExecuteStatus) -> None:
         self._execute_status = execute_status
 
     @property
@@ -85,49 +87,49 @@
         status = self._execute_status
         if status is None or status.outcome is None:  # interrupt before status create # pragma: no branch
             return "", ""  # pragma: no cover
         return status.outcome.out_err()
 
 
 class Pep517VirtualEnvPackager(PythonPackageToxEnv, VirtualEnv):
-    """local file system python virtual environment via the virtualenv package"""
+    """local file system python virtual environment via the virtualenv package."""
 
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
         super().__init__(create_args)
         self._frontend_: Pep517VirtualEnvFrontend | None = None
         self.builds: defaultdict[str, list[EnvConfigSet]] = defaultdict(list)
         self._distribution_meta: PathDistribution | None = None
         self._package_dependencies: list[Requirement] | None = None
         self._package_name: str | None = None
         self._pkg_lock = RLock()  # can build only one package at a time
         self.root = self.conf["package_root"]
         self._package_paths: set[Path] = set()
 
     @staticmethod
-    def id() -> str:
+    def id() -> str:  # noqa: A003
         return "virtualenv-pep-517"
 
     @property
     def _frontend(self) -> Pep517VirtualEnvFrontend:
         if self._frontend_ is None:
             self._frontend_ = Pep517VirtualEnvFrontend(self.root, self)
         return self._frontend_
 
     def register_config(self) -> None:
         super().register_config()
         self.conf.add_config(
             keys=["meta_dir"],
             of_type=Path,
-            default=lambda conf, name: self.env_dir / ".meta",  # noqa: U100
+            default=lambda conf, name: self.env_dir / ".meta",  # noqa: ARG005
             desc="directory where to put the project metadata files",
         )
         self.conf.add_config(
             keys=["pkg_dir"],
             of_type=Path,
-            default=lambda conf, name: self.env_dir / "dist",  # noqa: U100
+            default=lambda conf, name: self.env_dir / "dist",  # noqa: ARG005
             desc="directory where to put project packages",
         )
 
     @property
     def pkg_dir(self) -> Path:
         return cast(Path, self.conf["pkg_dir"])
 
@@ -150,59 +152,62 @@
         build_type = run_env.conf["package"]
         self.builds[build_type].append(run_env.conf)
 
     def _setup_env(self) -> None:
         super()._setup_env()
         if "editable" in self.builds:
             if not self._frontend.optional_hooks["build_editable"]:
-                raise BuildEditableNotSupported
+                raise BuildEditableNotSupportedError
             build_requires = self._frontend.get_requires_for_build_editable().requires
             self._install(build_requires, PythonPackageToxEnv.__name__, "requires_for_build_editable")
         if "wheel" in self.builds:
             build_requires = self._frontend.get_requires_for_build_wheel().requires
             self._install(build_requires, PythonPackageToxEnv.__name__, "requires_for_build_wheel")
         if "sdist" in self.builds or "external" in self.builds:
             build_requires = self._frontend.get_requires_for_build_sdist().requires
             self._install(build_requires, PythonPackageToxEnv.__name__, "requires_for_build_sdist")
 
     def _teardown(self) -> None:
         executor = self._frontend.backend_executor
         if executor is not None:  # pragma: no branch
             try:
                 if executor.is_alive:
-                    self._frontend._send("_exit")  # try first on amicable shutdown
+                    self._frontend._send("_exit")  # try first on amicable shutdown  # noqa: SLF001
             except SystemExit:  # pragma: no cover  # if already has been interrupted ignore
                 pass
             finally:
                 executor.close()
         for path in self._package_paths:
             if path.exists():
                 logging.debug("delete package %s", path)
                 path.unlink()
         super()._teardown()
 
     def perform_packaging(self, for_env: EnvConfigSet) -> list[Package]:
-        """build the package to install"""
+        """Build the package to install."""
         try:
             deps = self._load_deps(for_env)
-        except BuildEditableNotSupported:
+        except BuildEditableNotSupportedError:
             targets = [e for e in self.builds.pop("editable") if e["package"] == "editable"]
             names = ", ".join(sorted({t.env_name for t in targets if t.env_name}))
-            logging.error(
-                f"package config for {names} is editable, however the build backend {self._frontend.backend}"
-                f" does not support PEP-660, falling back to editable-legacy - change your configuration to it",
+
+            logging.error(  # noqa: TRY400
+                "package config for %s is editable, however the build backend %s does not support PEP-660, falling "
+                "back to editable-legacy - change your configuration to it",
+                names,
+                cast(Pep517VirtualEnvFrontend, self._frontend_).backend,
             )
             for env in targets:
-                env._defined["package"].value = "editable-legacy"  # type: ignore
+                env._defined["package"].value = "editable-legacy"  # type: ignore[attr-defined]  # noqa: SLF001
                 self.builds["editable-legacy"].append(env)
             deps = self._load_deps(for_env)
         of_type: str = for_env["package"]
         if of_type == "editable-legacy":
             self.setup()
-            deps = [*self.requires(), *self._frontend.get_requires_for_build_sdist().requires] + deps
+            deps = [*self.requires(), *self._frontend.get_requires_for_build_sdist().requires, *deps]
             package: Package = EditableLegacyPackage(self.core["tox_root"], deps)  # the folder itself is the package
         elif of_type == "sdist":
             self.setup()
             with self._pkg_lock:
                 sdist = self._frontend.build_sdist(sdist_directory=self.pkg_dir).sdist
                 sdist = create_session_view(sdist, self._package_temp_path)
                 self._package_paths.add(sdist)
@@ -221,15 +226,16 @@
                         metadata_directory=self.meta_folder_if_populated,
                         config_settings=self._wheel_config_settings,
                     ).wheel
                     wheel = create_session_view(wheel, self._package_temp_path)
                     self._package_paths.add(wheel)
                 package = (EditablePackage if of_type == "editable" else WheelPackage)(wheel, deps)
         else:  # pragma: no cover # for when we introduce new packaging types and don't implement
-            raise TypeError(f"cannot handle package type {of_type}")  # pragma: no cover
+            msg = f"cannot handle package type {of_type}"
+            raise TypeError(msg)  # pragma: no cover
         return [package]
 
     @property
     def _package_temp_path(self) -> Path:
         return cast(Path, self.core["temp_dir"]) / "package"
 
     def _load_deps(self, for_env: EnvConfigSet) -> list[Requirement]:
@@ -279,16 +285,15 @@
                         reqs, name = w_env.get_package_dependencies(for_env), w_env.get_package_name(for_env)
                     else:
                         reqs = []
         if reqs is None:
             reqs = self.get_package_dependencies(for_env)
             name = self.get_package_name(for_env)
         extras: set[str] = for_env["extras"]
-        deps = dependencies_with_extras(reqs, extras, name)
-        return deps
+        return dependencies_with_extras(reqs, extras, name)
 
     def get_package_dependencies(self, for_env: EnvConfigSet) -> list[Requirement]:
         with self._pkg_lock:
             if self._package_dependencies is None:  # pragma: no branch
                 self._ensure_meta_present(for_env)
                 requires: list[str] = cast(PathDistribution, self._distribution_meta).requires or []
                 self._package_dependencies = [Requirement(i) for i in requires]  # pragma: no branch
@@ -324,39 +329,41 @@
     def __init__(self, root: Path, env: Pep517VirtualEnvPackager) -> None:
         super().__init__(*Frontend.create_args_from_folder(root))
         self._tox_env = env
         self._backend_executor_: LocalSubProcessPep517Executor | None = None
         into: dict[str, Any] = {}
         pkg_cache = cached(
             into,
-            key=lambda *args, **kwargs: "wheel" if "wheel_directory" in kwargs else "sdist",  # noqa: U100
+            key=lambda *args, **kwargs: "wheel" if "wheel_directory" in kwargs else "sdist",  # noqa: ARG005
         )
-        self.build_wheel = pkg_cache(self.build_wheel)  # type: ignore
-        self.build_sdist = pkg_cache(self.build_sdist)  # type: ignore
-        self.build_editable = pkg_cache(self.build_editable)  # type: ignore
+        self.build_wheel = pkg_cache(self.build_wheel)  # type: ignore[method-assign]
+        self.build_sdist = pkg_cache(self.build_sdist)  # type: ignore[method-assign]
+        self.build_editable = pkg_cache(self.build_editable)  # type: ignore[method-assign]
 
     @property
     def backend_cmd(self) -> Sequence[str]:
-        return ["python"] + self.backend_args
+        return ["python", *self.backend_args]
 
     def _send(self, cmd: str, **kwargs: Any) -> tuple[Any, str, str]:
         try:
-            if cmd in ("prepare_metadata_for_build_wheel", "prepare_metadata_for_build_editable"):
+            if (
+                cmd in ("prepare_metadata_for_build_wheel", "prepare_metadata_for_build_editable")
                 # given we'll build a wheel we might skip the prepare step
-                if "wheel" in self._tox_env.builds or "editable" in self._tox_env.builds:
-                    return None, "", ""  # will need to build wheel either way, avoid prepare
+                and ("wheel" in self._tox_env.builds or "editable" in self._tox_env.builds)
+            ):
+                return None, "", ""  # will need to build wheel either way, avoid prepare
             return super()._send(cmd, **kwargs)
         except BackendFailed as exception:
             raise exception if isinstance(exception, ToxBackendFailed) else ToxBackendFailed(exception) from exception
 
     @contextmanager
     def _send_msg(
         self,
         cmd: str,
-        result_file: Path,  # noqa: U100
+        result_file: Path,  # noqa: ARG002
         msg: str,
     ) -> Iterator[ToxCmdStatus]:
         with self._tox_env.execute_async(
             cmd=self.backend_cmd,
             cwd=self._root,
             stdin=StdinSource.API,
             show=None,
@@ -365,15 +372,22 @@
         ) as execute_status:
             execute_status.write_stdin(f"{msg}{os.linesep}")
             yield ToxCmdStatus(execute_status)
         outcome = execute_status.outcome
         if outcome is not None:  # pragma: no branch
             outcome.assert_success()
 
-    def _unexpected_response(self, cmd: str, got: Any, expected_type: Any, out: str, err: str) -> NoReturn:
+    def _unexpected_response(  # noqa: PLR0913
+        self,
+        cmd: str,
+        got: Any,
+        expected_type: Any,
+        out: str,
+        err: str,
+    ) -> NoReturn:
         try:
             super()._unexpected_response(cmd, got, expected_type, out, err)
         except BackendFailed as exception:
             raise exception if isinstance(exception, ToxBackendFailed) else ToxBackendFailed(exception) from exception
 
     @property
     def backend_executor(self) -> LocalSubProcessPep517Executor:
```

### Comparing `tox-4.6.0/src/tox/tox_env/python/virtual_env/package/util.py` & `tox-4.6.1/src/tox/tox_env/python/virtual_env/package/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import Optional, Set, cast
+from typing import TYPE_CHECKING, Optional, Set, cast
 
 from packaging.markers import Marker, Op, Variable  # type: ignore[attr-defined]
-from packaging.requirements import Requirement
+
+if TYPE_CHECKING:
+    from packaging.requirements import Requirement
 
 
 def dependencies_with_extras(deps: list[Requirement], extras: set[str], package_name: str) -> list[Requirement]:
     return dependencies_with_extras_from_markers(extract_extra_markers(deps), extras, package_name)
 
 
 def dependencies_with_extras_from_markers(
@@ -39,16 +41,15 @@
 def extract_extra_markers(deps: list[Requirement]) -> list[tuple[Requirement, set[str | None]]]:
     """
     Extract extra markers from dependencies.
 
     :param deps: the dependencies
     :return: a list of requirement, extras set
     """
-    result = [_extract_extra_markers(d) for d in deps]
-    return result
+    return [_extract_extra_markers(d) for d in deps]
 
 
 def _extract_extra_markers(req: Requirement) -> tuple[Requirement, set[str | None]]:
     req = deepcopy(req)
     markers: list[str | tuple[Variable, Op, Variable]] = getattr(req.marker, "_markers", []) or []
     new_markers: list[str | tuple[Variable, Op, Variable]] = []
     extra_markers: set[str] = set()  # markers that have a key of extra
@@ -62,17 +63,22 @@
             marker = markers.pop(0) if markers else None
             if marker in ("and", "or"):
                 marker = markers.pop(0) if markers else None
         else:
             new_markers.append(marker)
             marker = markers.pop(0) if markers else None
     if new_markers:
-        cast(Marker, req.marker)._markers = new_markers
+        cast(Marker, req.marker)._markers = new_markers  # noqa: SLF001
     else:
         req.marker = None
     return req, cast(Set[Optional[str]], extra_markers) or {None}
 
 
 def _get_extra(_marker: str | tuple[Variable, Op, Variable]) -> str | None:
-    if isinstance(_marker, tuple) and len(_marker) == 3 and _marker[0].value == "extra" and _marker[1].value == "==":
+    if (
+        isinstance(_marker, tuple)
+        and len(_marker) == 3  # noqa: PLR2004
+        and _marker[0].value == "extra"
+        and _marker[1].value == "=="
+    ):
         return _marker[2].value
     return None
```

### Comparing `tox-4.6.0/src/tox/util/ci.py` & `tox-4.6.1/src/tox/util/ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/src/tox/util/file_view.py` & `tox-4.6.1/src/tox/util/file_view.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 import logging
 import os
 import shutil
 from itertools import chain
 from os.path import commonpath
-from pathlib import Path
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from pathlib import Path
 
 
 def create_session_view(package: Path, temp_path: Path) -> Path:
-    """Allows using the file after you no longer holding a lock to it by moving it into a temp folder"""
+    """Allows using the file after you no longer holding a lock to it by moving it into a temp folder."""
     # we'll number the active instances, and use the max value as session folder for a new build
     # note we cannot change package names as PEP-491 (wheel binary format)
     # is strict about file name structure
 
     temp_path.mkdir(parents=True, exist_ok=True)
     exists = [i.name for i in temp_path.iterdir()]
     file_id = max(chain((0,), (int(i) for i in exists if str(i).isnumeric())))
```

### Comparing `tox-4.6.0/src/tox/util/graph.py` & `tox-4.6.1/src/tox/util/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Helper methods related to graph theory."""
 from __future__ import annotations
 
 from collections import OrderedDict, defaultdict
 
 
-def stable_topological_sort(graph: dict[str, set[str]]) -> list[str]:
+def stable_topological_sort(graph: dict[str, set[str]]) -> list[str]:  # noqa: C901
     to_order = set(graph.keys())  # keep a log of what  we need to order
 
     # normalize graph - fill missing nodes (assume no dependency)
     for values in list(graph.values()):
         for value in values:
             if value not in graph:
                 graph[value] = set()
@@ -17,15 +17,15 @@
     for key, depends in graph.items():
         for depend in depends:
             inverse_graph[depend].add(key)
 
     topology = []
     degree = {k: len(v) for k, v in graph.items()}
     ready_to_visit = {n for n, d in degree.items() if not d}
-    need_to_visit = OrderedDict((i, None) for i in graph.keys())
+    need_to_visit = OrderedDict((i, None) for i in graph)
     while need_to_visit:
         # to keep stable, pick the first node ready to visit in the original order
         for node in need_to_visit:
             if node in ready_to_visit:
                 break
         else:
             break
@@ -62,8 +62,9 @@
                 return path
         del path[vertex]
         return None
 
     for node in graph:  # pragma: no branch # we never get here if the graph is empty
         result = visit(node)
         if result is not None:
-            raise ValueError(f"{' | '.join(result.keys())}")
+            msg = f"{' | '.join(result.keys())}"
+            raise ValueError(msg)
```

### Comparing `tox-4.6.0/src/tox/util/spinner.py` & `tox-4.6.1/src/tox/util/spinner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-"""A minimal non-colored version of https://pypi.org/project/halo, to track list progress"""
+"""A minimal non-colored version of https://pypi.org/project/halo, to track list progress."""
 from __future__ import annotations
 
 import os
 import sys
 import textwrap
 import threading
 import time
 from collections import OrderedDict
-from types import TracebackType
-from typing import IO, NamedTuple, Sequence, TypeVar
+from typing import IO, TYPE_CHECKING, NamedTuple, Sequence, TypeVar
 
 from colorama import Fore
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
 if sys.platform == "win32":  # pragma: win32 cover
     import ctypes
 
     class _CursorInfo(ctypes.Structure):
         _fields_ = [("size", ctypes.c_int), ("visible", ctypes.c_byte)]
 
 
@@ -46,19 +48,19 @@
     CLEAR_LINE = "\033[K"
     max_width = 120
     UNICODE_FRAMES = ["⠋", "⠙", "⠹", "⠸", "⠼", "⠴", "⠦", "⠧", "⠇", "⠏"]
     ASCII_FRAMES = ["|", "-", "+", "x", "*"]
     UNICODE_OUTCOME = Outcome(ok="✔", fail="✖", skip="⚠")
     ASCII_OUTCOME = Outcome(ok="+", fail="!", skip="?")
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
-        enabled: bool = True,
+        enabled: bool = True,  # noqa: FBT001, FBT002
         refresh_rate: float = 0.1,
-        colored: bool = True,
+        colored: bool = True,  # noqa: FBT001, FBT002
         stream: IO[str] | None = None,
         total: int | None = None,
     ) -> None:
         self.is_colored = colored
         self.refresh_rate = refresh_rate
         self.enabled = enabled
         stream = sys.stdout if stream is None else stream
@@ -108,17 +110,17 @@
         self._spinner_thread = threading.Thread(target=self.render)
         self._spinner_thread.daemon = True
         self._spinner_thread.start()
         return self
 
     def __exit__(
         self,
-        exc_type: type[BaseException] | None,  # noqa: U100
-        exc_val: BaseException | None,  # noqa: U100
-        exc_tb: TracebackType | None,  # noqa: U100
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
         if not self._stop_spinner.is_set():  # pragma: no branch
             if self._spinner_thread:  # pragma: no branch # hard to test
                 self._stop_spinner.set()
                 self._spinner_thread.join()
 
             self._frame_index = 0
@@ -181,15 +183,15 @@
 ]
 
 
 def td_human_readable(seconds: float) -> str:
     texts: list[str] = []
     for period_name, period_seconds in _PERIODS:
         period_str = None
-        if period_name == "second" and (seconds >= 0.01 or not texts):
+        if period_name == "second" and (seconds >= 0.01 or not texts):  # noqa: PLR2004
             period_str = f"{seconds:.2f}".rstrip("0").rstrip(".")
         elif seconds >= period_seconds:
             period_value, seconds = divmod(seconds, period_seconds)
             period_str = f"{period_value:.0f}"
         if period_str is not None:
             texts.append(f"{period_str} {period_name}{'' if period_str == '1' else 's'}")
     return " ".join(texts)
```

### Comparing `tox-4.6.0/tests/conftest.py` & `tox-4.6.1/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
 import os
 import sys
 from pathlib import Path
-from typing import Callable, Iterator, Sequence
+from typing import TYPE_CHECKING, Callable, Iterator, Sequence
 from unittest.mock import patch
 from uuid import uuid4
 
 import pytest
-from _pytest.monkeypatch import MonkeyPatch  # cannot import from tox.pytest yet
-from _pytest.tmpdir import TempPathFactory
 from distlib.scripts import ScriptMaker
 from filelock import FileLock
-from pytest_mock import MockerFixture
 from virtualenv import cli_run
 
 from tox.config.cli.parser import Parsed
-from tox.config.loader.api import Override
 from tox.config.main import Config
 from tox.config.source import discover_source
 from tox.tox_env.python.api import PythonInfo, VersionInfo
 from tox.tox_env.python.virtual_env.api import VirtualEnv
 
+if TYPE_CHECKING:
+    from _pytest.monkeypatch import MonkeyPatch
+    from _pytest.tmpdir import TempPathFactory
+    from pytest_mock import MockerFixture
+
+    from tox.config.loader.api import Override
+
 pytest_plugins = "tox.pytest"
 HERE = Path(__file__).absolute().parent
 
 
 @pytest.fixture(scope="session")
 def value_error() -> Callable[[str], str]:
     def _fmt(msg: str) -> str:
@@ -43,35 +46,34 @@
 collect_ignore = []
 if sys.implementation.name == "pypy":
     # time-machine causes segfaults on PyPy
     collect_ignore.append("util/test_spinner.py")
 
 
 class ToxIniCreator(Protocol):
-    def __call__(self, conf: str, override: Sequence[Override] | None = None) -> Config:  # noqa: U100
+    def __call__(self, conf: str, override: Sequence[Override] | None = None) -> Config:
         ...
 
 
 @pytest.fixture()
 def tox_ini_conf(tmp_path: Path, monkeypatch: MonkeyPatch) -> ToxIniCreator:
     def func(conf: str, override: Sequence[Override] | None = None) -> Config:
         dest = tmp_path / "c"
         dest.mkdir()
         config_file = dest / "tox.ini"
         config_file.write_bytes(conf.encode("utf-8"))
         with monkeypatch.context() as context:
             context.chdir(tmp_path)
         source = discover_source(config_file, None)
 
-        config = Config.make(
+        return Config.make(
             Parsed(work_dir=dest, override=override or [], config_file=config_file, root_dir=None),
             pos_args=[],
             source=source,
         )
-        return config
 
     return func
 
 
 @pytest.fixture(scope="session")
 def demo_pkg_setuptools() -> Path:
     return HERE / "demo_pkg_setuptools"
@@ -88,15 +90,15 @@
 def patch_prev_py(mocker: MockerFixture) -> Callable[[bool], tuple[str, str]]:
     def _func(has_prev: bool) -> tuple[str, str]:
         ver = sys.version_info[0:2]
         prev_ver = "".join(str(i) for i in (ver[0], ver[1] - 1))
         prev_py = f"py{prev_ver}"
         impl = sys.implementation.name.lower()
 
-        def get_python(self: VirtualEnv, base_python: list[str]) -> PythonInfo | None:
+        def get_python(self: VirtualEnv, base_python: list[str]) -> PythonInfo | None:  # noqa: ARG001
             if base_python[0] == "py31" or (base_python[0] == prev_py and not has_prev):
                 return None
             raw = list(sys.version_info)
             if base_python[0] == prev_py:
                 raw[1] -= 1  # type: ignore[operator]
             ver_info = VersionInfo(*raw)  # type: ignore[arg-type]
             return PythonInfo(
@@ -142,14 +144,13 @@
     return build_pkg(tmp_path_factory.mktemp("dist"), demo_pkg_inline, ["wheel"])
 
 
 def build_pkg(dist_dir: Path, of: Path, distributions: list[str], isolation: bool = True) -> Path:
     from build.__main__ import build_package
 
     build_package(str(of), str(dist_dir), distributions=distributions, isolation=isolation)
-    package = next(dist_dir.iterdir())
-    return package
+    return next(dist_dir.iterdir())
 
 
 @pytest.fixture(scope="session")
 def pkg_builder() -> Callable[[Path, Path, list[str], bool], Path]:
     return build_pkg
```

### Comparing `tox-4.6.0/tests/test_provision.py` & `tox-4.6.1/tests/test_provision.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import json
 import os
 import sys
 import time
 from contextlib import contextmanager
 from pathlib import Path
 from subprocess import check_call
-from typing import Callable, Iterator
+from typing import TYPE_CHECKING, Callable, Iterator
 from unittest import mock
 from zipfile import ZipFile
 
 import pytest
-from devpi_process import Index, IndexServer
 from filelock import FileLock
 from packaging.requirements import Requirement
 
-from tox.pytest import MonkeyPatch, TempPathFactory, ToxProjectCreator
+if TYPE_CHECKING:
+    from devpi_process import Index, IndexServer
+
+    from tox.pytest import MonkeyPatch, TempPathFactory, ToxProjectCreator
 
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from importlib.metadata import Distribution
 else:  # pragma: no cover (<py38)
     from importlib_metadata import Distribution
 
 ROOT = Path(__file__).parents[1]
@@ -28,15 +30,15 @@
 
 @contextmanager
 def elapsed(msg: str) -> Iterator[None]:
     start = time.monotonic()
     try:
         yield
     finally:
-        print(f"done in {time.monotonic() - start}s {msg}")
+        print(f"done in {time.monotonic() - start}s {msg}")  # noqa: T201
 
 
 @pytest.fixture(scope="session")
 def tox_wheel(
     tmp_path_factory: TempPathFactory,
     worker_id: str,
     pkg_builder: Callable[[Path, Path, list[str], bool], Path],
@@ -61,28 +63,28 @@
 ) -> Path:
     with elapsed("acquire current tox wheel"):  # takes around 3.2s on build
         into = tmp_path_factory.mktemp("dist")  # pragma: no cover
         from tox.version import version_tuple
 
         version = f"{version_tuple[0]}.{version_tuple[1]}.{version_tuple[2] +1}"
         with mock.patch.dict(os.environ, {"SETUPTOOLS_SCM_PRETEND_VERSION": version}):
-            package = pkg_builder(into, Path(__file__).parents[1], ["wheel"], False)  # pragma: no cover
-        return package
+            return pkg_builder(into, Path(__file__).parents[1], ["wheel"], False)  # pragma: no cover
 
 
 @pytest.fixture(scope="session")
 def tox_wheels(tox_wheel: Path, tmp_path_factory: TempPathFactory) -> list[Path]:
     with elapsed("acquire dependencies for current tox"):  # takes around 1.5s if already cached
         result: list[Path] = [tox_wheel]
         info = tmp_path_factory.mktemp("info")
         with ZipFile(str(tox_wheel), "r") as zip_file:
             zip_file.extractall(path=info)
         dist_info = next((i for i in info.iterdir() if i.suffix == ".dist-info"), None)
         if dist_info is None:  # pragma: no cover
-            raise RuntimeError(f"no tox.dist-info inside {tox_wheel}")
+            msg = f"no tox.dist-info inside {tox_wheel}"
+            raise RuntimeError(msg)
         distribution = Distribution.at(dist_info)
         wheel_cache = ROOT / ".wheel_cache" / f"{sys.version_info.major}.{sys.version_info.minor}"
         wheel_cache.mkdir(parents=True, exist_ok=True)
         cmd = [sys.executable, "-I", "-m", "pip", "download", "-d", str(wheel_cache)]
         assert distribution.requires is not None
         for req in distribution.requires:
             requirement = Requirement(req)
@@ -223,13 +225,10 @@
 
 @pytest.mark.integration()
 @pytest.mark.usefixtures("_pypi_index_self")
 @pytest.mark.parametrize("relative_path", [True, False], ids=["relative", "absolute"])
 def test_provision_conf_file(tox_project: ToxProjectCreator, tmp_path: Path, relative_path: bool) -> None:
     ini = "[tox]\nrequires = demo-pkg-inline\nskipsdist=true\n"
     project = tox_project({"tox.ini": ini}, prj_path=tmp_path / "sub")
-    if relative_path:
-        conf_path = os.path.join(project.path.name, "tox.ini")
-    else:
-        conf_path = str(project.path / "tox.ini")
+    conf_path = str(Path(project.path.name) / "tox.ini") if relative_path else str(project.path / "tox.ini")
     result = project.run("c", "--conf", conf_path, "-e", "py", from_cwd=tmp_path)
     result.assert_success()
```

### Comparing `tox-4.6.0/tests/test_report.py` & `tox-4.6.1/tests/test_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
 import logging
 import os
+from typing import TYPE_CHECKING
 
 import pytest
 from colorama import Style, deinit
-from pytest_mock import MockerFixture
 
-from tox.pytest import CaptureFixture
 from tox.report import setup_report
 
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import CaptureFixture
+
 
 @pytest.mark.parametrize("color", [True, False], ids=["on", "off"])
 @pytest.mark.parametrize("verbosity", range(7))
 def test_setup_report(mocker: MockerFixture, capsys: CaptureFixture, verbosity: int, color: bool) -> None:
     color_init = mocker.patch("tox.report.init")
 
     setup_report(verbosity=verbosity, is_colored=color)
@@ -24,18 +28,18 @@
         logging.warning("%s%s> %s", "warning", "foo", "bar")
         logging.info("info")
         logging.debug("debug")
         logging.log(logging.NOTSET, "not-set")  # this should not be logged
         disabled = "distlib.util", "filelock"
         for name in disabled:
             logger = logging.getLogger(name)
-            logger.warning(f"{name}-warn")
-            logger.info(f"{name}-info")
-            logger.debug(f"{name}-debug")
-            logger.log(logging.NOTSET, f"{name}-notset")
+            logger.warning("%s-warn", name)
+            logger.info("%s-info", name)
+            logger.debug("%s-debug", name)
+            logger.log(logging.NOTSET, "%s-notset", name)
     finally:
         deinit()
 
     assert color_init.call_count == (1 if color else 0)
 
     msg_count = min(verbosity + 1, 5)
     is_debug_or_more = verbosity >= 4
```

### Comparing `tox-4.6.0/tests/test_run.py` & `tox-4.6.1/tests/test_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
-from pytest_mock import MockerFixture
 
-from tox.pytest import ToxProjectCreator
 from tox.report import HandledError
 from tox.run import run
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import ToxProjectCreator
+
 
 @pytest.mark.parametrize("exception", [HandledError, KeyboardInterrupt])
 def test_exit_code_minus_2_on_expected_exit(exception: Exception, mocker: MockerFixture) -> None:
     mocker.patch("tox.run.main", side_effect=exception)
     with pytest.raises(SystemExit) as system_exit:
         run()
     assert system_exit.value.code == -2
```

### Comparing `tox-4.6.0/tests/test_version.py` & `tox-4.6.1/tests/test_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 from types import SimpleNamespace
-
-from pytest_mock import MockFixture
+from typing import TYPE_CHECKING
 
 from tox import __version__
 from tox.plugin.manager import MANAGER
-from tox.pytest import ToxProjectCreator
+
+if TYPE_CHECKING:
+    from pytest_mock import MockFixture
+
+    from tox.pytest import ToxProjectCreator
 
 
 def test_version() -> None:
     assert __version__
 
 
 def test_version_without_plugin(tox_project: ToxProjectCreator) -> None:
```

### Comparing `tox-4.6.0/tests/config/test_main.py` & `tox-4.6.1/tests/config/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
+from typing import TYPE_CHECKING
 
-from tests.conftest import ToxIniCreator
 from tox.config.loader.api import Override
 from tox.config.loader.memory import MemoryLoader
-from tox.config.main import Config
 from tox.config.sets import ConfigSet
-from tox.pytest import ToxProjectCreator
+
+if TYPE_CHECKING:
+    from tests.conftest import ToxIniCreator
+    from tox.config.main import Config
+    from tox.pytest import ToxProjectCreator
 
 
 def test_empty_config_repr(empty_config: Config) -> None:
     text = repr(empty_config)
     assert str(empty_config.core["tox_root"]) in text
     assert "config_source=ToxIni" in text
```

### Comparing `tox-4.6.0/tests/config/test_of_types.py` & `tox-4.6.1/tests/config/test_of_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/tests/config/test_set_env.py` & `tox-4.6.1/tests/config/test_set_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 import sys
 from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from unittest.mock import ANY
 
 import pytest
-from pytest_mock import MockerFixture
 
 from tox.config.set_env import SetEnv
-from tox.pytest import MonkeyPatch, ToxProjectCreator
+
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import MonkeyPatch, ToxProjectCreator
 
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from typing import Protocol
 else:  # pragma: no cover (<py38)
     from typing_extensions import Protocol
 
 
@@ -35,17 +38,17 @@
     with pytest.raises(ValueError, match="A"):
         SetEnv("A", "py", "py", Path())
 
 
 class EvalSetEnv(Protocol):
     def __call__(
         self,
-        tox_ini: str,  # noqa: U100
-        extra_files: dict[str, Any] | None = ...,  # noqa: U100
-        from_cwd: Path | None = ...,  # noqa: U100
+        tox_ini: str,
+        extra_files: dict[str, Any] | None = ...,
+        from_cwd: Path | None = ...,
     ) -> SetEnv:
         ...
 
 
 @pytest.fixture()
 def eval_set_env(tox_project: ToxProjectCreator) -> EvalSetEnv:
     def func(tox_ini: str, extra_files: dict[str, Any] | None = None, from_cwd: Path | None = None) -> SetEnv:
```

### Comparing `tox-4.6.0/tests/config/test_sets.py` & `tox-4.6.1/tests/config/test_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
 from collections import OrderedDict
 from pathlib import Path
-from typing import Callable, Dict, Optional, Set, TypeVar
+from typing import TYPE_CHECKING, Callable, Dict, Optional, Set, TypeVar
 
 import pytest
-from pytest_mock import MockerFixture
 
-from tests.conftest import ToxIniCreator
 from tox.config.cli.parser import Parsed
 from tox.config.loader.memory import MemoryLoader
 from tox.config.main import Config
 from tox.config.sets import ConfigSet, EnvConfigSet
 from tox.config.source.api import Section
-from tox.pytest import ToxProjectCreator
+
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tests.conftest import ToxIniCreator
+    from tox.pytest import ToxProjectCreator
 
 ConfBuilder = Callable[[str], ConfigSet]
 
 
 @pytest.fixture(name="conf_builder")
 def _conf_builder(tox_ini_conf: ToxIniCreator) -> ConfBuilder:  # noqa: PT005
     def _make(conf_str: str) -> ConfigSet:
@@ -150,23 +153,23 @@
 
     project = tox_project({"tox.ini": "[testenv]\npackage=skip\n[A]\na=1\n[magic]\nb = ok"})
     result = project.run()
     section = MagicConfigSet.SECTION
     conf = result.state.conf.get_section_config(section, base=["A"], of_type=MagicConfigSet, for_env=None)
     assert conf["a"] == 1
     assert conf["b"] == "ok"
-    exp = "MagicConfigSet(loaders=[IniLoader(section=magic, overrides={}), " "IniLoader(section=A, overrides={})])"
+    exp = "MagicConfigSet(loaders=[IniLoader(section=magic, overrides={}), IniLoader(section=A, overrides={})])"
     assert repr(conf) == exp
 
-    assert isinstance(result.state.conf._options, Parsed)
+    assert isinstance(result.state.conf._options, Parsed)  # noqa: SLF001
 
 
 def test_do_not_allow_create_config_set(mocker: MockerFixture) -> None:
     with pytest.raises(TypeError, match="Can't instantiate"):
-        ConfigSet(mocker.create_autospec(Config))  # type: ignore # the type checker also warns that ABC
+        ConfigSet(mocker.create_autospec(Config))  # type: ignore[abstract,call-arg]
 
 
 def test_set_env_raises_on_non_str(mocker: MockerFixture) -> None:
     env_set = EnvConfigSet(mocker.create_autospec(Config), Section("a", "b"), "b")
     env_set.loaders.insert(0, MemoryLoader(set_env=1))
     with pytest.raises(TypeError, match="1"):
         assert env_set["set_env"]
```

### Comparing `tox-4.6.0/tests/config/test_types.py` & `tox-4.6.1/tests/config/test_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/tests/config/cli/conftest.py` & `tox-4.6.1/tests/config/cli/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 import pytest
 
 from tox.session.cmd.depends import depends
 from tox.session.cmd.devenv import devenv
 from tox.session.cmd.exec_ import exec_
 from tox.session.cmd.legacy import legacy
 from tox.session.cmd.list_env import list_env
 from tox.session.cmd.quickstart import quickstart
 from tox.session.cmd.run.parallel import run_parallel
 from tox.session.cmd.run.sequential import run_sequential
 from tox.session.cmd.show_config import show_config
-from tox.session.state import State
+
+if TYPE_CHECKING:
+    from tox.session.state import State
 
 
 @pytest.fixture()
 def core_handlers() -> dict[str, Callable[[State], int]]:
     return {
         "config": show_config,
         "c": show_config,
```

### Comparing `tox-4.6.0/tests/config/cli/test_cli_env_var.py` & `tox-4.6.1/tests/config/cli/test_cli_env_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 from unittest.mock import ANY
 
 import pytest
 
 from tox.config.cli.parse import get_options
 from tox.config.loader.api import Override
-from tox.pytest import CaptureFixture, LogCaptureFixture, MonkeyPatch
 from tox.session.env_select import CliEnv
-from tox.session.state import State
 from tox.util.ci import is_ci
 
+if TYPE_CHECKING:
+    from tox.pytest import CaptureFixture, LogCaptureFixture, MonkeyPatch
+    from tox.session.state import State
+
 
 def test_verbose() -> None:
     parsed, _, __, ___, ____ = get_options("-v", "-v")
     assert parsed.verbosity == 4
 
 
 def test_verbose_compound() -> None:
```

### Comparing `tox-4.6.0/tests/config/cli/test_cli_ini.py` & `tox-4.6.1/tests/config/cli/test_cli_ini.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from __future__ import annotations
 
 import logging
 import sys
 import textwrap
 from pathlib import Path
-from typing import Any, Callable
+from typing import TYPE_CHECKING, Any, Callable
 from unittest.mock import ANY
 
 import pytest
-from pytest_mock import MockerFixture
 
 from tox.config.cli.ini import IniConfig
 from tox.config.cli.parse import get_options
 from tox.config.cli.parser import Parsed
 from tox.config.loader.api import Override
 from tox.config.main import Config
 from tox.config.source import discover_source
-from tox.pytest import CaptureFixture, LogCaptureFixture, MonkeyPatch
 from tox.session.env_select import CliEnv
-from tox.session.state import State
 from tox.util.ci import is_ci
 
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import CaptureFixture, LogCaptureFixture, MonkeyPatch
+    from tox.session.state import State
+
 
 @pytest.fixture()
 def exhaustive_ini(tmp_path: Path, monkeypatch: MonkeyPatch) -> Path:
     to = tmp_path / "tox.ini"
     to.write_text(
         textwrap.dedent(
             """
@@ -46,15 +49,15 @@
         ),
     )
     monkeypatch.setenv("TOX_USER_CONFIG_FILE", str(to))
     return to
 
 
 @pytest.mark.parametrize("content", ["[tox]", ""])
-def test_ini_empty(
+def test_ini_empty(  # noqa: PLR0913
     tmp_path: Path,
     core_handlers: dict[str, Callable[[State], int]],
     default_options: dict[str, Any],
     mocker: MockerFixture,
     monkeypatch: MonkeyPatch,
     content: str,
 ) -> None:
@@ -103,14 +106,25 @@
         "labels": [],
         "exit_and_dump_after": 0,
         "skip_env": "",
         "list_dependencies": is_ci(),
     }
 
 
+def test_ini_help(exhaustive_ini: Path, capfd: CaptureFixture) -> None:
+    with pytest.raises(SystemExit) as context:
+        get_options("-h")
+    assert context.value.code == 0
+    out, err = capfd.readouterr()
+    assert not err
+    res = out.splitlines()[-1]
+    msg = f"config file {str(exhaustive_ini)!r} active (changed via env var TOX_USER_CONFIG_FILE)"
+    assert res == msg
+
+
 @pytest.mark.usefixtures("exhaustive_ini")
 def test_ini_exhaustive_parallel_values(core_handlers: dict[str, Callable[[State], int]]) -> None:
     options = get_options("p")
     assert vars(options.parsed) == {
         "colored": "yes",
         "command": "p",
         "default_runner": "virtualenv",
@@ -143,23 +157,14 @@
         "skip_env": "",
         "list_dependencies": is_ci(),
     }
     assert options.parsed.verbosity == 4
     assert options.cmd_handlers == core_handlers
 
 
-def test_ini_help(exhaustive_ini: Path, capsys: CaptureFixture) -> None:
-    with pytest.raises(SystemExit) as context:
-        get_options("-h")
-    assert context.value.code == 0
-    out, err = capsys.readouterr()
-    assert not err
-    assert f"config file '{exhaustive_ini}' active (changed via env var TOX_USER_CONFIG_FILE)"
-
-
 def test_bad_cli_ini(
     tmp_path: Path,
     monkeypatch: MonkeyPatch,
     caplog: LogCaptureFixture,
     default_options: dict[str, Any],
     mocker: MockerFixture,
 ) -> None:
```

### Comparing `tox-4.6.0/tests/config/cli/test_parse.py` & `tox-4.6.1/tests/config/cli/test_parse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 import logging
+from typing import TYPE_CHECKING
 
 import pytest
 
 from tox.config.cli.parse import get_options
-from tox.pytest import CaptureFixture
+
+if TYPE_CHECKING:
+    from tox.pytest import CaptureFixture
 
 
 def test_help_does_not_default_cmd(capsys: CaptureFixture) -> None:
     with pytest.raises(SystemExit):
         get_options("-h")
     out, err = capsys.readouterr()
     assert not err
```

### Comparing `tox-4.6.0/tests/config/cli/test_parser.py` & `tox-4.6.1/tests/config/cli/test_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 import sys
 from argparse import Action
+from typing import TYPE_CHECKING
 
 import pytest
-from pytest_mock import MockerFixture
 
 from tox.config.cli.parser import Parsed, ToxParser
-from tox.pytest import CaptureFixture, MonkeyPatch
+
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import CaptureFixture, MonkeyPatch
 
 
 def test_parser_const_with_default_none(monkeypatch: MonkeyPatch) -> None:
     monkeypatch.setenv("TOX_ALPHA", "2")
     parser = ToxParser.base()
     parser.add_argument(
         "-a",
@@ -28,15 +32,15 @@
 
 
 @pytest.mark.parametrize("is_atty", [True, False])
 @pytest.mark.parametrize("no_color", [None, "0", "1", "", "\t", " ", "false", "true"])
 @pytest.mark.parametrize("force_color", [None, "0", "1"])
 @pytest.mark.parametrize("tox_color", [None, "bad", "no", "yes"])
 @pytest.mark.parametrize("term", [None, "xterm", "dumb"])
-def test_parser_color(
+def test_parser_color(  # noqa: PLR0913
     monkeypatch: MonkeyPatch,
     mocker: MockerFixture,
     no_color: str | None,
     force_color: str | None,
     tox_color: str | None,
     is_atty: bool,
     term: str | None,
@@ -78,15 +82,20 @@
     assert isinstance(action, Action)
     assert action.dest == "magic"
 
 
 def test_sub_sub_command() -> None:
     parser = ToxParser.base()
     with pytest.raises(RuntimeError, match="no sub-command group allowed"):
-        parser.add_command("c", [], "help", lambda s: 0)  # pragma: no cover - the lambda will never be run # noqa: U100
+        parser.add_command(
+            "c",
+            [],
+            "help",
+            lambda s: 0,  # noqa: ARG005
+        )  # pragma: no cover - the lambda will never be run
 
 
 def test_parse_known_args_not_set(mocker: MockerFixture) -> None:
     mocker.patch.object(sys, "argv", ["a", "--help"])
     parser = ToxParser.base()
     _, unknown = parser.parse_known_args(None)
     assert unknown == ["--help"]
```

### Comparing `tox-4.6.0/tests/config/loader/test_loader.py` & `tox-4.6.1/tests/config/loader/test_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 import pytest
 
 from tox.config.cli.parse import get_options
 from tox.config.loader.api import Override
-from tox.pytest import CaptureFixture
+
+if TYPE_CHECKING:
+    from tox.pytest import CaptureFixture
 
 
 @pytest.mark.parametrize("flag", ["-x", "--override"])
 def test_override_incorrect(flag: str, capsys: CaptureFixture) -> None:
     with pytest.raises(SystemExit):
         get_options(flag, "magic")
     out, err = capsys.readouterr()
@@ -19,15 +23,15 @@
 @pytest.mark.parametrize("flag", ["-x", "--override"])
 def test_override_add(flag: str) -> None:
     parsed, _, __, ___, ____ = get_options(flag, "magic=true")
     assert len(parsed.override) == 1
     value = parsed.override[0]
     assert value.key == "magic"
     assert value.value == "true"
-    assert value.namespace == ""
+    assert not value.namespace
 
 
 def test_override_equals() -> None:
     assert Override("a=b") == Override("a=b")
 
 
 def test_override_not_equals() -> None:
```

### Comparing `tox-4.6.0/tests/config/loader/test_memory_loader.py` & `tox-4.6.1/tests/config/loader/test_memory_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,22 +41,22 @@
         (0, bool, False),
         (1, bool, True),
         ("1", int, 1),
         (1, str, "1"),
         ({1}, Set[str], {"1"}),
         ({"1"}, List[int], [1]),
         ({"1": "2"}, Dict[int, int], {1: 2}),
-        (os.getcwd(), Path, Path.cwd()),
+        (os.getcwd(), Path, Path.cwd()),  # noqa: PTH109
         ("pip list", Command, Command(["pip", "list"])),
         ("a\nb", EnvList, EnvList(["a", "b"])),
         ("1", Optional[int], 1),
     ],
 )
 def test_memory_loader(value: Any, of_type: type[Any], outcome: Any) -> None:
-    loader = MemoryLoader(**{"a": value}, kwargs={})
+    loader = MemoryLoader(a=value, kwargs={})
     args = ConfigLoadArgs([], "name", None)
     loaded = loader.load("a", of_type=of_type, conf=None, factory=None, args=args)
     assert loaded == outcome
 
 
 @pytest.mark.parametrize(
     ("value", "of_type", "exception", "msg"),
@@ -68,15 +68,15 @@
         ({1: "m"}, Dict[int, int], ValueError, "invalid literal for int"),
         (object, Path, TypeError, "expected str, bytes or os.PathLike object"),
         (1, Command, TypeError, "1"),
         (1, EnvList, TypeError, "1"),
     ],
 )
 def test_memory_loader_fails_invalid(value: Any, of_type: type[Any], exception: Exception, msg: str) -> None:
-    loader = MemoryLoader(**{"a": value}, kwargs={})
+    loader = MemoryLoader(a=value, kwargs={})
     args = ConfigLoadArgs([], "name", None)
     with pytest.raises(exception, match=msg):  # type: ignore[call-overload]
         loader.load("a", of_type=of_type, conf=None, factory=None, args=args)
 
 
 def test_memory_found_keys() -> None:
     loader = MemoryLoader(a=1, c=2)
```

### Comparing `tox-4.6.0/tests/config/loader/test_section.py` & `tox-4.6.1/tests/config/loader/test_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/tests/config/loader/test_str_convert.py` & `tox-4.6.1/tests/config/loader/test_str_convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import sys
 from pathlib import Path
 from textwrap import dedent
-from typing import Any, Dict, List, Optional, Set, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set, TypeVar, Union
 
 import pytest
 
 from tox.config.loader.str_convert import StrConvert
 from tox.config.types import Command, EnvList
-from tox.pytest import MonkeyPatch, SubRequest, ToxProjectCreator
+
+if TYPE_CHECKING:
+    from tox.pytest import MonkeyPatch, SubRequest, ToxProjectCreator
 
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from typing import Literal
 else:  # pragma: no cover (py38+)
     from typing_extensions import Literal
 
 
@@ -115,18 +117,16 @@
     (r"X:\\foo\\bar --quuz='baz atan'", [r"X:\foo\bar", "--quuz=baz atan"]),
     ("/foo/bar --quuz='baz atan'", ["/foo/bar", "--quuz=baz atan"]),
     ('cc --arg "C:\\\\Users\\""', ["cc", "--arg", 'C:\\Users"']),
     ('cc --arg "C:\\\\Users\\"', ["cc", "--arg", '"C:\\\\Users\\"']),
     ('cc --arg "C:\\\\Users"', ["cc", "--arg", "C:\\Users"]),
     ('cc --arg \\"C:\\\\Users"', ["cc", "--arg", '\\"C:\\\\Users"']),
     ('cc --arg "C:\\\\Users\\ "', ["cc", "--arg", "C:\\Users\\ "]),
-    # ('cc --arg "C:\\\\Users\\ ', ["cc", "--arg", '"C:\\\\Users\\ ']),
     ('cc --arg "C:\\\\Users\\\\"', ["cc", "--arg", "C:\\Users\\"]),
     ('cc --arg "C:\\\\Users\\\\ "', ["cc", "--arg", "C:\\Users\\ "]),
-    # ('cc --arg "C:\\\\Users\\\\ ', ["cc", "--arg", '"C:\\\\Users\\\\ ']),
     (
         r'cc --arg C:\\Users\\ --arg2 "SPECIAL:\Temp\f o o" --arg3="\\FOO\share\Path name" --arg4 SPECIAL:\Temp\ '[:-1],
         [
             "cc",
             "--arg",
             "C:\\Users\\",
             "--arg2",
```

### Comparing `tox-4.6.0/tests/config/loader/ini/conftest.py` & `tox-4.6.1/tests/config/loader/ini/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 from configparser import ConfigParser
-from pathlib import Path
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 import pytest
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 @pytest.fixture()
 def mk_ini_conf(tmp_path: Path) -> Callable[[str], ConfigParser]:
     def _func(raw: str) -> ConfigParser:
         filename = tmp_path / "demo.ini"
         filename.write_bytes(raw.encode("utf-8"))  # win32: avoid CR normalization - what you pass is what you get
         parser = ConfigParser(interpolation=None)
```

### Comparing `tox-4.6.0/tests/config/loader/ini/test_factor.py` & `tox-4.6.1/tests/config/loader/ini/test_factor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from __future__ import annotations
 
-from configparser import ConfigParser
 from textwrap import dedent
-from typing import Callable, List
+from typing import TYPE_CHECKING, Callable, List
 
 import pytest
 
-from tests.conftest import ToxIniCreator
 from tox.config.loader.ini import IniLoader
 from tox.config.loader.ini.factor import filter_for_env, find_envs
-from tox.config.main import Config
 from tox.config.source.ini_section import IniSection
 
+if TYPE_CHECKING:
+    from configparser import ConfigParser
+
+    from tests.conftest import ToxIniCreator
+    from tox.config.main import Config
+
 
 def test_factor_env_discover_empty() -> None:
     result = list(find_envs("\n\n"))
     assert result == []
 
 
 @pytest.fixture(scope="session")
@@ -83,15 +86,15 @@
     assert "no:space" in result
     if "py" in env:
         assert "py only" in result
         assert "not py" not in result
     else:
         assert "py only" not in result
         assert "not py" in result
-    if "extra" == env:
+    if env == "extra":
         assert "extra" in result
     else:
         assert "extra" not in result
     if env in {"py-a", "py-a-dev", "py-b", "py-b-dev", "c"}:
         assert "complex" in result
     else:
         assert "complex" not in result
@@ -144,15 +147,15 @@
             assert "unittest2" in deps
             assert "negation-or" in deps
         if "django15" in env:
             assert "Django>=1.5,<1.6" in deps
             assert "negation-or" in deps
         if "django16" in env:
             assert "Django>=1.6,<1.7" in deps
-        if "py36-django15" == env_config.name:
+        if env_config.name == "py36-django15":
             assert "negation-and" in deps
 
 
 def test_factor_config_do_not_replace_unescaped_comma(tox_ini_conf: ToxIniCreator) -> None:
     config = tox_ini_conf("[tox]\nenv_list = py37-{base,i18n},b")
     assert list(config) == ["py37-base", "py37-i18n", "b"]
```

### Comparing `tox-4.6.0/tests/config/loader/ini/test_ini_loader.py` & `tox-4.6.1/tests/config/loader/ini/test_ini_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
-from configparser import ConfigParser
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 import pytest
 
 from tox.config.loader.api import ConfigLoadArgs, Override
 from tox.config.loader.ini import IniLoader
 from tox.config.source.ini_section import IniSection
 
+if TYPE_CHECKING:
+    from configparser import ConfigParser
+
 
 def test_ini_loader_keys(mk_ini_conf: Callable[[str], ConfigParser]) -> None:
     core = IniSection(None, "tox")
     loader = IniLoader(core, mk_ini_conf("\n[tox]\n\na=b\nc=d\n\n"), [], core_section=core)
     assert loader.found_keys() == {"a", "c"}
```

### Comparing `tox-4.6.0/tests/config/loader/ini/replace/conftest.py` & `tox-4.6.1/tests/config/loader/ini/replace/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 import sys
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
 
 from tox.config.cli.parser import Parsed
 from tox.config.loader.api import ConfigLoadArgs
 from tox.config.main import Config
 from tox.config.source.tox_ini import ToxIni
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from typing import Protocol
 else:  # pragma: no cover (<py38)
     from typing_extensions import Protocol
 
 
 class ReplaceOne(Protocol):
-    def __call__(self, conf: str, pos_args: list[str] | None = None) -> str:  # noqa: U100
+    def __call__(self, conf: str, pos_args: list[str] | None = None) -> str:
         ...
 
 
 @pytest.fixture()
 def replace_one(tmp_path: Path) -> ReplaceOne:
     def example(conf: str, pos_args: list[str] | None = None) -> str:
         tox_ini_file = tmp_path / "tox.ini"
```

### Comparing `tox-4.6.0/tests/config/loader/ini/replace/test_replace.py` & `tox-4.6.1/tests/config/loader/ini/replace/test_replace.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 import pytest
 
-from tests.config.loader.ini.replace.conftest import ReplaceOne
 from tox.config.loader.ini.replace import MatchExpression, find_replace_expr
 from tox.report import HandledError
 
+if TYPE_CHECKING:
+    from tests.config.loader.ini.replace.conftest import ReplaceOne
+
 
 @pytest.mark.parametrize(
     ("value", "exp_output"),
     [
         ("[]", [MatchExpression([["posargs"]])]),
         ("123[]", ["123", MatchExpression([["posargs"]])]),
         ("[]123", [MatchExpression([["posargs"]]), "123"]),
@@ -85,9 +89,9 @@
     [
         (MatchExpression([["posargs"]]), "MatchExpression(expr=[['posargs']], term_pos=None)"),
         (MatchExpression([["posargs"]], 1), "MatchExpression(expr=[['posargs']], term_pos=1)"),
         (MatchExpression("foo", -42), "MatchExpression(expr='foo', term_pos=-42)"),
     ],
 )
 def test_match_expression_repr(match_expression: MatchExpression, exp_repr: str) -> None:
-    print(match_expression)
+    print(match_expression)  # noqa: T201
     assert repr(match_expression) == exp_repr
```

### Comparing `tox-4.6.0/tests/config/loader/ini/replace/test_replace_env_var.py` & `tox-4.6.1/tests/config/loader/ini/replace/test_replace_env_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import threading
-from typing import Generator
+from typing import TYPE_CHECKING, Generator
 
 import pytest
 
-from tests.config.loader.ini.replace.conftest import ReplaceOne
-from tox.pytest import LogCaptureFixture, MonkeyPatch
+if TYPE_CHECKING:
+    from tests.config.loader.ini.replace.conftest import ReplaceOne
+    from tox.pytest import LogCaptureFixture, MonkeyPatch
 
 
 def test_replace_env_set(replace_one: ReplaceOne, monkeypatch: MonkeyPatch) -> None:
     """If we have a factor that is not specified within the core env-list then that's also an environment"""
     monkeypatch.setenv("MAGIC", "something good")
     result = replace_one("{env:MAGIC}")
     assert result == "something good"
@@ -29,16 +30,16 @@
     result = replace_one(r"{env:MAGIC}\\\{env:MAGIC}")
     assert result == r"something good\\{env:MAGIC}"
 
 
 def test_replace_env_set_quad_bs(replace_one: ReplaceOne, monkeypatch: MonkeyPatch) -> None:
     """Quad backslash should remain but not affect surrounding replacements."""
     monkeypatch.setenv("MAGIC", "something good")
-    result = replace_one(r"\\{env:MAGIC}\\\\{env:MAGIC}" + "\\")
-    assert result == r"\\something good\\\\something good" + "\\"
+    result = replace_one(r"\\{env:MAGIC}\\\\{env:MAGIC}" + "\\")  # noqa: ISC003
+    assert result == r"\\something good\\\\something good" + "\\"  # noqa: ISC003
 
 
 def test_replace_env_when_value_is_backslash(replace_one: ReplaceOne, monkeypatch: MonkeyPatch) -> None:
     """When the replacement value is backslash, it shouldn't affect the next replacement."""
     monkeypatch.setenv("MAGIC", "tragic")
     monkeypatch.setenv("BS", "\\")
     result = replace_one(r"{env:BS}{env:MAGIC}")
@@ -53,15 +54,15 @@
     assert result == r"stuff\tragic"
 
 
 def test_replace_env_missing(replace_one: ReplaceOne, monkeypatch: MonkeyPatch) -> None:
     """If we have a factor that is not specified within the core env-list then that's also an environment"""
     monkeypatch.delenv("MAGIC", raising=False)
     result = replace_one("{env:MAGIC}")
-    assert result == ""
+    assert not result
 
 
 def test_replace_env_missing_default(replace_one: ReplaceOne, monkeypatch: MonkeyPatch) -> None:
     """If we have a factor that is not specified within the core env-list then that's also an environment"""
     monkeypatch.delenv("MAGIC", raising=False)
     result = replace_one("{env:MAGIC:def}")
     assert result == "def"
```

### Comparing `tox-4.6.0/tests/config/loader/ini/replace/test_replace_os_sep.py` & `tox-4.6.1/tests/config/loader/ini/replace/test_replace_os_sep.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import os
+from typing import TYPE_CHECKING
 
 import pytest
 
-from tests.config.loader.ini.replace.conftest import ReplaceOne
-from tox.pytest import MonkeyPatch
+if TYPE_CHECKING:
+    from tests.config.loader.ini.replace.conftest import ReplaceOne
+    from tox.pytest import MonkeyPatch
 
 
 def test_replace_os_sep(replace_one: ReplaceOne) -> None:
     result = replace_one("{/}")
     assert result == os.sep
```

### Comparing `tox-4.6.0/tests/config/loader/ini/replace/test_replace_posargs.py` & `tox-4.6.1/tests/config/loader/ini/replace/test_replace_posargs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 import sys
+from typing import TYPE_CHECKING
 
 import pytest
 
-from tests.config.loader.ini.replace.conftest import ReplaceOne
+if TYPE_CHECKING:
+    from tests.config.loader.ini.replace.conftest import ReplaceOne
 
 
 @pytest.mark.parametrize("syntax", ["{posargs}", "[]"])
 def test_replace_pos_args_none_sys_argv(syntax: str, replace_one: ReplaceOne) -> None:
     result = replace_one(syntax, None)
-    assert result == ""
+    assert not result
 
 
 @pytest.mark.parametrize("syntax", ["{posargs}", "[]"])
 def test_replace_pos_args_empty_sys_argv(syntax: str, replace_one: ReplaceOne) -> None:
     result = replace_one(syntax, [])
-    assert result == ""
+    assert not result
 
 
 @pytest.mark.parametrize("syntax", ["{posargs}", "[]"])
 def test_replace_pos_args_extra_sys_argv(syntax: str, replace_one: ReplaceOne) -> None:
     result = replace_one(syntax, [sys.executable, "magic"])
     assert result == f"{sys.executable} magic"
 
@@ -77,8 +79,8 @@
     outcome = replace_one(value, ["foo"])
     assert result == outcome
 
 
 def test_half_escaped_braces(replace_one: ReplaceOne) -> None:
     """See https://github.com/tox-dev/tox/issues/1956"""
     outcome = replace_one(r"\{posargs} {posargs}", ["foo"])
-    assert "{posargs} foo" == outcome
+    assert outcome == "{posargs} foo"
```

### Comparing `tox-4.6.0/tests/config/loader/ini/replace/test_replace_tox_env.py` & `tox-4.6.1/tests/config/loader/ini/replace/test_replace_tox_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 import pytest
 
-from tests.config.loader.ini.replace.conftest import ReplaceOne
-from tests.conftest import ToxIniCreator
 from tox.config.loader.ini.replace import MAX_REPLACE_DEPTH
 from tox.config.sets import ConfigSet
-from tox.pytest import LogCaptureFixture
 from tox.report import HandledError
 
+if TYPE_CHECKING:
+    from tests.config.loader.ini.replace.conftest import ReplaceOne
+    from tests.conftest import ToxIniCreator
+    from tox.pytest import LogCaptureFixture
+
 EnvConfigCreator = Callable[[str], ConfigSet]
 
 
 @pytest.fixture()
 def example(tox_ini_conf: ToxIniCreator) -> EnvConfigCreator:
     def func(conf: str) -> ConfigSet:
         config = tox_ini_conf(f"""[tox]\nenv_list = a\n[testenv]\n{conf}\n""")
-        env_config = config.get_env("a")
-        return env_config
+        return config.get_env("a")
 
     return func
 
 
 def test_replace_within_tox_env(example: EnvConfigCreator) -> None:
     env_config = example("r = 1\no = {r}")
     env_config.add_config(keys="r", of_type=str, default="r", desc="r")
```

### Comparing `tox-4.6.0/tests/config/loader/ini/replace/test_replace_tty.py` & `tox-4.6.1/tests/config/loader/ini/replace/test_replace_tty.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
 import sys
+from typing import TYPE_CHECKING
 
 import pytest
-from pytest_mock import MockFixture
 
-from tests.config.loader.ini.replace.conftest import ReplaceOne
+if TYPE_CHECKING:
+    from pytest_mock import MockFixture
+
+    from tests.config.loader.ini.replace.conftest import ReplaceOne
 
 
 @pytest.mark.parametrize("is_atty", [True, False])
 def test_replace_env_set(replace_one: ReplaceOne, mocker: MockFixture, is_atty: bool) -> None:
     mocker.patch.object(sys.stdout, "isatty", return_value=is_atty)
 
     result = replace_one("1 {tty} 2")
```

### Comparing `tox-4.6.0/tests/config/source/test_discover.py` & `tox-4.6.1/tests/config/source/test_discover.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
-from tox.pytest import ToxProjectCreator
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import ToxProjectCreator
 
 
 def out_no_src(path: Path) -> str:
     return (
         f"ROOT: No tox.ini or setup.cfg or pyproject.toml found, assuming empty tox.ini at {path}\n"
         f"default environments:\npy -> [no description]\n"
     )
```

### Comparing `tox-4.6.0/tests/config/source/test_setup_cfg.py` & `tox-4.6.1/tests/config/source/test_setup_cfg.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
-from tox.pytest import ToxProjectCreator
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from tox.pytest import ToxProjectCreator
 
 
 def test_conf_in_setup_cfg(tox_project: ToxProjectCreator) -> None:
     project = tox_project({"setup.cfg": "[tox:tox]\nenv_list=\n a\n b"})
 
     outcome = project.run("l")
     outcome.assert_success()
```

### Comparing `tox-4.6.0/tests/config/source/test_source_ini.py` & `tox-4.6.1/tests/config/source/test_source_ini.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
-from tests.conftest import ToxIniCreator
 from tox.config.loader.section import Section
 from tox.config.sets import ConfigSet
 from tox.config.source.ini import IniSource
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tests.conftest import ToxIniCreator
+
 
 def test_source_ini_with_interpolated(tmp_path: Path) -> None:
     loader = IniSource(tmp_path, content="[tox]\na = %(c)s").get_loader(Section(None, "tox"), {})
     assert loader is not None
     loader.load_raw("a", None, None)
 
 
 def test_source_ini_ignore_non_testenv_sections(tmp_path: Path) -> None:
     loader = IniSource(tmp_path, content="[mypy-rest_framework.compat.*]")
-    res = list(loader.envs({"env_list": []}))  # type: ignore
+    res = list(loader.envs({"env_list": []}))  # type: ignore[arg-type]
     assert not res
 
 
 def test_source_ini_ignore_invalid_factor_filters(tmp_path: Path) -> None:
     loader = IniSource(tmp_path, content="[a]\nb= if c: d")
-    res = list(loader.envs({"env_list": []}))  # type: ignore
+    res = list(loader.envs({"env_list": []}))  # type: ignore[arg-type]
     assert not res
 
 
 def test_source_ini_custom_non_testenv_sections(tox_ini_conf: ToxIniCreator) -> None:
     """Validate that a plugin can load section with custom prefix overlapping testenv name."""
 
     class CustomConfigSet(ConfigSet):
@@ -35,15 +39,15 @@
                 keys=["a"],
                 of_type=str,
                 default="",
                 desc="d",
             )
 
     config = tox_ini_conf("[testenv:foo]\n[custom:foo]\na = b")
-    known_envs = list(config._src.envs(config.core))
+    known_envs = list(config._src.envs(config.core))  # noqa: SLF001
     assert known_envs
     custom_section = config.get_section_config(
         section=Section("custom", "foo"),
         base=[],
         of_type=CustomConfigSet,
         for_env=None,
     )
```

### Comparing `tox-4.6.0/tests/demo_pkg_inline/build.py` & `tox-4.6.1/tests/demo_pkg_inline/build.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
 Please keep this file Python 2.7 compatible.
 See https://tox.readthedocs.io/en/rewrite/development.html#code-style-guide
 """
+from __future__ import annotations
+
 import os
 import sys
 import tarfile
+from pathlib import Path
 from textwrap import dedent
 from zipfile import ZipFile
 
 name = "demo_pkg_inline"
 pkg_name = name.replace("_", "-")
 
 version = "1.0.0"
-dist_info = "{}-{}.dist-info".format(name, version)
-logic = "{}/__init__.py".format(name)
-plugin = "{}/example_plugin.py".format(name)
-entry_points = "{}/entry_points.txt".format(dist_info)
-metadata = "{}/METADATA".format(dist_info)
-wheel = "{}/WHEEL".format(dist_info)
-record = "{}/RECORD".format(dist_info)
+dist_info = f"{name}-{version}.dist-info"
+logic = f"{name}/__init__.py"
+plugin = f"{name}/example_plugin.py"
+entry_points = f"{dist_info}/entry_points.txt"
+metadata = f"{dist_info}/METADATA"
+wheel = f"{dist_info}/WHEEL"
+record = f"{dist_info}/RECORD"
 content = {
-    logic: "def do():\n    print('greetings from {}')".format(name),
+    logic: f"def do():\n    print('greetings from {name}')",
     plugin: """
         try:
             from tox.plugin import impl
             from tox.tox_env.python.virtual_env.runner import VirtualEnvRunner
             from tox.tox_env.register import ToxEnvRegister
         except ImportError:
             pass
@@ -68,56 +71,60 @@
         Root-Is-Purelib: true
         Tag: py{}-none-any
        """.format(
         name,
         version,
         sys.version_info[0],
     ),
-    "{}/top_level.txt".format(dist_info): name,
+    f"{dist_info}/top_level.txt": name,
     record: """
         {0}/__init__.py,,
         {1}/METADATA,,
         {1}/WHEEL,,
         {1}/top_level.txt,,
         {1}/RECORD,,
        """.format(
         name,
         dist_info,
     ),
 }
 
 
-def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):  # noqa: U100
-    base_name = "{}-{}-py{}-none-any.whl".format(name, version, sys.version_info[0])
-    path = os.path.join(wheel_directory, base_name)
-    with ZipFile(path, "w") as zip_file_handler:
+def build_wheel(
+    wheel_directory: str,
+    config_settings: dict[str, str] | None = None,  # noqa: ARG001
+    metadata_directory: str | None = None,
+) -> str:
+    base_name = f"{name}-{version}-py{sys.version_info[0]}-none-any.whl"
+    path = Path(wheel_directory) / base_name
+    with ZipFile(str(path), "w") as zip_file_handler:
         for arc_name, data in content.items():  # pragma: no branch
             zip_file_handler.writestr(arc_name, dedent(data).strip())
         if metadata_directory is not None:
             for sub_directory, _, filenames in os.walk(metadata_directory):
                 for filename in filenames:
                     zip_file_handler.write(
-                        os.path.join(metadata_directory, sub_directory, filename),
-                        os.path.join(sub_directory, filename),
+                        str(Path(metadata_directory) / sub_directory / filename),
+                        str(Path(sub_directory) / filename),
                     )
         else:
             for arc_name, data in metadata_files.items():  # pragma: no branch
                 zip_file_handler.writestr(arc_name, dedent(data).strip())
-    print("created wheel {}".format(path))
+    print(f"created wheel {path}")  # noqa: T201
     return base_name
 
 
-def get_requires_for_build_wheel(config_settings=None):  # noqa: U100
+def get_requires_for_build_wheel(config_settings: dict[str, str] | None = None) -> list[str]:  # noqa: ARG001
     return []  # pragma: no cover # only executed in non-host pythons
 
 
-def build_sdist(sdist_directory, config_settings=None):  # noqa: U100
-    result = "{}-{}.tar.gz".format(name, version)  # pragma: win32 cover
-    with tarfile.open(os.path.join(sdist_directory, result), "w:gz") as tar:  # pragma: win32 cover
-        root = os.path.dirname(os.path.abspath(__file__))  # pragma: win32 cover
-        tar.add(os.path.join(root, "build.py"), "build.py")  # pragma: win32 cover
-        tar.add(os.path.join(root, "pyproject.toml"), "pyproject.toml")  # pragma: win32 cover
+def build_sdist(sdist_directory: str, config_settings: dict[str, str] | None = None) -> str:  # noqa: ARG001
+    result = f"{name}-{version}.tar.gz"  # pragma: win32 cover
+    with tarfile.open(str(Path(sdist_directory) / result), "w:gz") as tar:  # pragma: win32 cover
+        root = Path(__file__).parent  # pragma: win32 cover
+        tar.add(str(root / "build.py"), "build.py")  # pragma: win32 cover
+        tar.add(str(root / "pyproject.toml"), "pyproject.toml")  # pragma: win32 cover
     return result  # pragma: win32 cover
 
 
-def get_requires_for_build_sdist(config_settings=None):  # noqa: U100
+def get_requires_for_build_sdist(config_settings: dict[str, str] | None = None) -> list[str]:  # noqa: ARG001
     return []  # pragma: no cover # only executed in non-host pythons
```

### Comparing `tox-4.6.0/tests/execute/test_request.py` & `tox-4.6.1/tests/execute/test_request.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/tests/execute/local_subprocess/bad_process.py` & `tox-4.6.1/tests/execute/local_subprocess/bad_process.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 from __future__ import annotations
 
 import os
 import signal
 import sys
 import time
 from pathlib import Path
-from types import FrameType
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from types import FrameType
 
 out = sys.stdout
 
 
-def handler(signum: int, _: FrameType | None) -> None:  # noqa: U101
+def handler(signum: int, _: FrameType | None) -> None:
     _p(f"how about no signal {signum!r}")
 
 
 def _p(m: str) -> None:
     out.write(f"{m}{os.linesep}")
     out.flush()  # force output flush in case we get killed
```

### Comparing `tox-4.6.0/tests/execute/local_subprocess/local_subprocess_sigint.py` & `tox-4.6.1/tests/execute/local_subprocess/local_subprocess_sigint.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 
 import logging
 import os
 import signal
 import sys
 from io import TextIOWrapper
 from pathlib import Path
-from types import FrameType
+from typing import TYPE_CHECKING
 from unittest.mock import MagicMock
 
-from tox.execute import Outcome
 from tox.execute.local_sub_process import LocalSubProcessExecutor
 from tox.execute.request import ExecuteRequest, StdinSource
 from tox.report import NamedBytesIO
 
+if TYPE_CHECKING:
+    from types import FrameType
+
+    from tox.execute import Outcome
+
 logging.basicConfig(level=logging.DEBUG, format="%(relativeCreated)d\t%(levelname).1s\t%(message)s")
 bad_process = Path(__file__).parent / "bad_process.py"
 
 executor = LocalSubProcessExecutor(colored=False)
 request = ExecuteRequest(
     cmd=[sys.executable, bad_process, sys.argv[1]],
     cwd=Path().absolute(),
@@ -26,40 +30,40 @@
     run_id="",
 )
 out_err = TextIOWrapper(NamedBytesIO("out")), TextIOWrapper(NamedBytesIO("err"))
 
 
 def show_outcome(outcome: Outcome | None) -> None:
     if outcome is not None:  # pragma: no branch
-        print(outcome.exit_code)
-        print(repr(outcome.out))
-        print(repr(outcome.err))
-        print(outcome.elapsed, end="")
-        print("done show outcome", file=sys.stderr)
+        print(outcome.exit_code)  # noqa: T201
+        print(repr(outcome.out))  # noqa: T201
+        print(repr(outcome.err))  # noqa: T201
+        print(outcome.elapsed, end="")  # noqa: T201
+        print("done show outcome", file=sys.stderr)  # noqa: T201
 
 
 def handler(s: int, f: FrameType | None) -> None:
-    logging.info(f"signal {s} at {f}")
-    global interrupt_done
+    logging.info("signal %s at %s", s, f)
+    global interrupt_done  # noqa: PLW0603
     if interrupt_done is False:  # pragma: no branch
         interrupt_done = True
-        logging.info(f"interrupt via {status}")
+        logging.info("interrupt via %s", status)
         status.interrupt()
-        logging.info(f"interrupt finished via {status}")
+        logging.info("interrupt finished via %s", status)
 
 
 interrupt_done = False
 signal.signal(signal.SIGINT, handler)
 logging.info("PID %d start %r", os.getpid(), request)
 tox_env = MagicMock(conf={"suicide_timeout": 0.01, "interrupt_timeout": 0.05, "terminate_timeout": 0.07})
 try:
     with executor.call(request, show=False, out_err=out_err, env=tox_env) as status:
         logging.info("wait on %r", status)
         while status.exit_code is None:
             status.wait(timeout=0.01)  # use wait here with timeout to not block the main thread
         logging.info("wait over on %r", status)
     show_outcome(status.outcome)
 except Exception as exception:  # pragma: no cover
-    logging.exception(exception)  # pragma: no cover
+    logging.exception(exception)  # noqa: TRY401 # pragma: no cover
 finally:
     logging.info("done")
     logging.shutdown()
```

### Comparing `tox-4.6.0/tests/execute/local_subprocess/test_execute_util.py` & `tox-4.6.1/tests/execute/local_subprocess/test_execute_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 from tox.execute.util import shebang
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 def test_shebang_found(tmp_path: Path) -> None:
     script_path = tmp_path / "a"
     script_path.write_text("#!  /bin/python \t-c\t")
     assert shebang(str(script_path)) == ["/bin/python", "-c"]
```

### Comparing `tox-4.6.0/tests/execute/local_subprocess/test_local_subprocess.py` & `tox-4.6.1/tests/execute/local_subprocess/test_local_subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,44 +5,48 @@
 import os
 import shutil
 import stat
 import subprocess
 import sys
 from io import TextIOWrapper
 from pathlib import Path
+from typing import TYPE_CHECKING
 from unittest.mock import MagicMock, create_autospec
 
 import psutil
 import pytest
 from colorama import Fore
 from psutil import AccessDenied
-from pytest_mock import MockerFixture
 
 from tox.execute.api import ExecuteOptions, Outcome
 from tox.execute.local_sub_process import SIG_INTERRUPT, LocalSubProcessExecuteInstance, LocalSubProcessExecutor
 from tox.execute.request import ExecuteRequest, StdinSource
 from tox.execute.stream import SyncWrite
-from tox.pytest import CaptureFixture, LogCaptureFixture, MonkeyPatch
 from tox.report import NamedBytesIO
 
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import CaptureFixture, LogCaptureFixture, MonkeyPatch
+
 
 class FakeOutErr:
     def __init__(self) -> None:
         self.out_err = TextIOWrapper(NamedBytesIO("out")), TextIOWrapper(NamedBytesIO("err"))
 
     def read_out_err(self) -> tuple[str, str]:
         out_got = self.out_err[0].buffer.getvalue().decode(self.out_err[0].encoding)  # type: ignore[attr-defined]
         err_got = self.out_err[1].buffer.getvalue().decode(self.out_err[1].encoding)  # type: ignore[attr-defined]
         return out_got, err_got
 
 
 @pytest.mark.parametrize("color", [True, False], ids=["color", "no_color"])
 @pytest.mark.parametrize(("out", "err"), [("out", "err"), ("", "")], ids=["simple", "nothing"])
 @pytest.mark.parametrize("show", [True, False], ids=["show", "no_show"])
-def test_local_execute_basic_pass(
+def test_local_execute_basic_pass(  # noqa: PLR0913
     caplog: LogCaptureFixture,
     os_env: dict[str, str],
     out: str,
     err: str,
     show: bool,
     color: bool,
 ) -> None:
@@ -212,16 +216,16 @@
         while status.exit_code is None:  # pragma: no branch
             status.wait()  # pragma: no cover
     outcome = status.outcome
     assert outcome is not None
 
     assert bool(outcome) is False, outcome
     assert outcome.exit_code != Outcome.OK
-    assert outcome.out == ""
-    assert outcome.err == ""
+    assert not outcome.out
+    assert not outcome.err
     assert not caplog.records
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="You need a conhost shell for keyboard interrupt")
 @pytest.mark.flaky(max_runs=3, min_passes=1)
 def test_command_keyboard_interrupt(tmp_path: Path, monkeypatch: MonkeyPatch, capfd: CaptureFixture) -> None:
     monkeypatch.chdir(tmp_path)
@@ -233,15 +237,15 @@
     root = process.pid
     try:
         child = next(iter(psutil.Process(pid=root).children())).pid
     except AccessDenied as exc:  # pragma: no cover # on termux for example
         pytest.skip(str(exc))  # pragma: no cover
         raise  # pragma: no cover
 
-    print(f"test running in {os.getpid()} and sending CTRL+C to {process.pid}", file=sys.stderr)
+    print(f"test running in {os.getpid()} and sending CTRL+C to {process.pid}", file=sys.stderr)  # noqa: T201
     process.send_signal(SIG_INTERRUPT)
     try:
         process.communicate(timeout=3)
     except subprocess.TimeoutExpired:  # pragma: no cover
         process.kill()
         raise
```

### Comparing `tox-4.6.0/tests/journal/test_main_journal.py` & `tox-4.6.1/tests/journal/test_main_journal.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/tests/plugin/test_inline.py` & `tox-4.6.1/tests/plugin/test_inline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
-from tox.pytest import ToxProjectCreator
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from tox.config.cli.parser import ToxParser
+    from tox.pytest import ToxProjectCreator
 
 
 def test_inline_tox_py(tox_project: ToxProjectCreator) -> None:
     def plugin() -> None:  # pragma: no cover # the code is copied to a python file
         import logging
 
-        from tox.config.cli.parser import ToxParser
         from tox.plugin import impl
 
         @impl
         def tox_add_option(parser: ToxParser) -> None:
             logging.warning("Add magic")
             parser.add_argument("--magic", action="store_true")
```

### Comparing `tox-4.6.0/tests/plugin/test_plugin.py` & `tox-4.6.1/tests/plugin/test_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from __future__ import annotations
 
 import logging
 import os
 import sys
-from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from unittest.mock import patch
 
 import pytest
-from pytest_mock import MockerFixture
 
 from tox.config.cli.parser import ToxParser
 from tox.config.loader.memory import MemoryLoader
 from tox.config.sets import ConfigSet, CoreConfigSet, EnvConfigSet
 from tox.execute import Outcome
 from tox.plugin import impl
 from tox.pytest import ToxProjectCreator, register_inline_plugin
 from tox.session.state import State
 from tox.tox_env.api import ToxEnv
 from tox.tox_env.register import ToxEnvRegister
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytest_mock import MockerFixture
+
 
 def test_plugin_hooks_and_order(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     @impl
     def tox_register_tox_env(register: ToxEnvRegister) -> None:
         assert isinstance(register, ToxEnvRegister)
         logging.warning("tox_register_tox_env")
 
@@ -51,15 +54,15 @@
 
     @impl
     def tox_on_install(tox_env: ToxEnv, arguments: Any, section: str, of_type: str) -> None:
         assert isinstance(tox_env, ToxEnv)
         assert arguments is not None
         assert isinstance(section, str)
         assert isinstance(of_type, str)
-        logging.warning(f"tox_on_install {section} {of_type}")
+        logging.warning("tox_on_install %s %s", section, of_type)
 
     @impl
     def tox_after_run_commands(tox_env: ToxEnv, exit_code: int, outcomes: list[Outcome]) -> None:
         assert isinstance(tox_env, ToxEnv)
         assert exit_code == 0
         assert isinstance(outcomes, list)
         assert all(isinstance(i, Outcome) for i in outcomes)
@@ -114,29 +117,29 @@
 def test_plugin_can_set_core_conf(
     tox_project: ToxProjectCreator,
     mocker: MockerFixture,
     dir_name: str,
     tmp_path: Path,
 ) -> None:
     @impl
-    def tox_add_core_config(core_conf: CoreConfigSet, state: State) -> None:  # noqa: U100
+    def tox_add_core_config(core_conf: CoreConfigSet, state: State) -> None:  # noqa: ARG001
         core_conf.loaders.insert(0, MemoryLoader(**{dir_name: tmp_path}))
 
     register_inline_plugin(mocker, tox_add_core_config)
 
     project = tox_project({})
     result = project.run("c")
     result.assert_success()
 
     assert result.state.conf.core[dir_name] == tmp_path
 
 
 def test_plugin_can_read_env_list(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     @impl
-    def tox_add_core_config(core_conf: CoreConfigSet, state: State) -> None:  # noqa: U100
+    def tox_add_core_config(core_conf: CoreConfigSet, state: State) -> None:  # noqa: ARG001
         logging.warning("All envs: %s", ", ".join(state.envs.iter(only_active=False)))
         logging.warning("Default envs: %s", ", ".join(state.envs.iter(only_active=True)))
 
     register_inline_plugin(mocker, tox_add_core_config)
     ini = """
     [tox]
     env_list = explicit
@@ -150,15 +153,15 @@
     result = project.run()
     assert "ROOT: All envs: explicit, section, implicit" in result.out
     assert "ROOT: Default envs: explicit" in result.out
 
 
 def test_plugin_can_read_sections(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     @impl
-    def tox_add_core_config(core_conf: CoreConfigSet, state: State) -> None:  # noqa: U100
+    def tox_add_core_config(core_conf: CoreConfigSet, state: State) -> None:  # noqa: ARG001
         logging.warning("Sections: %s", ", ".join(i.key for i in state.conf.sections()))
 
     register_inline_plugin(mocker, tox_add_core_config)
     ini = """
     [tox]
     [testenv]
     package = skip
@@ -169,29 +172,29 @@
     result = project.run()
     result.assert_success()
     assert "ROOT: Sections: tox, testenv, testenv:section, other:section" in result.out
 
 
 def test_plugin_injects_invalid_python_run(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     @impl
-    def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:  # noqa: U100
+    def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:  # noqa: ARG001
         env_conf.loaders.insert(0, MemoryLoader(deps=[1]))
         with pytest.raises(TypeError, match="1"):
             assert env_conf["deps"]
 
     register_inline_plugin(mocker, tox_add_env_config)
     project = tox_project({"tox.ini": "[testenv]\npackage=skip"})
     result = project.run()
     result.assert_failed()
     assert "raise TypeError(raw)" in result.out
 
 
 def test_plugin_extend_pass_env(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     @impl
-    def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:  # noqa: U100
+    def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:  # noqa: ARG001
         env_conf["pass_env"].append("MAGIC_*")
 
     register_inline_plugin(mocker, tox_add_env_config)
     ini = """
     [testenv]
     package=skip
     commands=python -c 'import os; print(os.environ["MAGIC_1"]); print(os.environ["MAGIC_2"])'
@@ -206,15 +209,15 @@
     result_conf = project.run("c", "-e", "py", "-k", "pass_env")
     result_conf.assert_success()
     assert "MAGIC_*" in result_conf.out
 
 
 def test_plugin_extend_set_env(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     @impl
-    def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:  # noqa: U100
+    def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:  # noqa: ARG001
         env_conf["set_env"].update({"MAGI_CAL": "magi_cal"})
 
     register_inline_plugin(mocker, tox_add_env_config)
     ini = """
     [testenv]
     package=skip
     commands=python -c 'import os; print(os.environ["MAGI_CAL"])'
@@ -232,26 +235,26 @@
 def test_plugin_config_frozen_past_add_env(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     def _cannot_extend_config(config_set: ConfigSet) -> None:
         for _conf in (
             lambda c: c.add_constant("c", "desc", "v"),
             lambda c: c.add_config("c", of_type=str, default="c", desc="d"),
         ):
             try:
-                _conf(config_set)  # type: ignore # call to not typed function
-                raise NotImplementedError
+                _conf(config_set)  # type: ignore[no-untyped-call] # call to not typed function
+                raise NotImplementedError  # noqa: TRY301
             except RuntimeError as exc:
-                assert str(exc) == "config set has been marked final and cannot be extended"
+                assert str(exc) == "config set has been marked final and cannot be extended"  # noqa: PT017
 
     @impl
     def tox_before_run_commands(tox_env: ToxEnv) -> None:
         _cannot_extend_config(tox_env.conf)
         _cannot_extend_config(tox_env.core)
 
     @impl
-    def tox_after_run_commands(tox_env: ToxEnv, exit_code: int, outcomes: list[Outcome]) -> None:  # noqa: U100
+    def tox_after_run_commands(tox_env: ToxEnv, exit_code: int, outcomes: list[Outcome]) -> None:  # noqa: ARG001
         _cannot_extend_config(tox_env.conf)
         _cannot_extend_config(tox_env.core)
 
     register_inline_plugin(mocker, tox_before_run_commands, tox_after_run_commands)
 
     project = tox_project({"tox.ini": "[testenv]\npackage=skip"})
     result = project.run("r")
```

### Comparing `tox-4.6.0/tests/plugin/test_plugin_custom_config_set.py` & `tox-4.6.1/tests/plugin/test_plugin_custom_config_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from __future__ import annotations
 
 import logging
 from functools import partial
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 import pytest
-from pytest_mock import MockerFixture
 
 from tox.config.loader.section import Section
 from tox.config.sets import ConfigSet, EnvConfigSet
 from tox.plugin import impl
 from tox.pytest import ToxProjectCreator, register_inline_plugin
-from tox.session.state import State
-from tox.tox_env.api import ToxEnv
+
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tox.session.state import State
+    from tox.tox_env.api import ToxEnv
 
 
 @pytest.fixture(autouse=True)
 def _custom_config_set(mocker: MockerFixture) -> None:
     class DockerConfigSet(ConfigSet):
         def register_config(self) -> None:
             self.add_config(keys="A", of_type=int, default=0, desc="a config")
 
     @impl
     def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:
         def factory(for_env: str, raw: object) -> DockerConfigSet:
             assert isinstance(raw, str)
             section = Section("docker", raw)
-            conf_set = state.conf.get_section_config(section, base=["docker"], of_type=DockerConfigSet, for_env=for_env)
-            return conf_set
+            return state.conf.get_section_config(section, base=["docker"], of_type=DockerConfigSet, for_env=for_env)
 
         env_conf.add_config(
             "docker",
             of_type=Optional[DockerConfigSet],  # type: ignore[arg-type] # mypy fails to understand the type info
             default=None,
             desc="docker env",
             factory=partial(factory, env_conf.name),
```

### Comparing `tox-4.6.0/tests/pytest_/test_init.py` & `tox-4.6.1/tests/pytest_/test_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 import os
 import sys
 from itertools import chain, combinations
-from pathlib import Path
 from textwrap import dedent
-from typing import Sequence
+from typing import TYPE_CHECKING, Sequence
 
 import pytest
-from pytest_mock import MockerFixture
 
 from tox.pytest import MonkeyPatch, ToxProjectCreator, check_os_environ
 from tox.report import HandledError
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytest_mock import MockerFixture
+
 
 def test_tox_project_no_base(tox_project: ToxProjectCreator) -> None:
     project = tox_project(
         {
             "tox.ini": "[tox]",
             "src": {"__init__.py": "pass", "a": "out", "b": {"c": "out"}, "e": {"f": ""}},
         },
@@ -107,15 +110,15 @@
     assert repr(outcome) == msg
     assert outcome.shell_cmd == f"{sys.executable} -m tox l"
 
 
 def test_tox_run_assert_out_err_no_dedent(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     project = tox_project({"tox.ini": ""})
 
-    def _main(args: Sequence[str]) -> int:  # noqa: U100
-        print(" goes on out", file=sys.stdout)
-        print(" goes on err", file=sys.stderr)
+    def _main(args: Sequence[str]) -> int:  # noqa: ARG001
+        print(" goes on out", file=sys.stdout)  # noqa: T201
+        print(" goes on err", file=sys.stderr)  # noqa: T201
         return 0
 
     mocker.patch("tox.run.main", side_effect=_main)
     outcome = project.run("c")
     outcome.assert_out_err(" goes on out\n", " goes on err\n", dedent=False)
```

### Comparing `tox-4.6.0/tests/session/test_env_select.py` & `tox-4.6.1/tests/session/test_env_select.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 import pytest
 
 from tox.config.cli.parse import get_options
-from tox.pytest import MonkeyPatch, ToxProjectCreator
 from tox.session.env_select import CliEnv, EnvSelector
 from tox.session.state import State
 
+if TYPE_CHECKING:
+    from tox.pytest import MonkeyPatch, ToxProjectCreator
+
 
 def test_label_core_can_define(tox_project: ToxProjectCreator) -> None:
     ini = """
         [tox]
         labels =
             test = py3{10,9}
             static = flake8, type
```

### Comparing `tox-4.6.0/tests/session/test_session_common.py` & `tox-4.6.1/tests/session/test_session_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/tests/session/cmd/test_depends.py` & `tox-4.6.1/tests/session/cmd/test_depends.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import sys
 from textwrap import dedent
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
-from tox.pytest import ToxProjectCreator
+if TYPE_CHECKING:
+    from tox.pytest import ToxProjectCreator
 
 
 def test_depends(tox_project: ToxProjectCreator, patch_prev_py: Callable[[bool], tuple[str, str]]) -> None:
     prev_ver, impl = patch_prev_py(True)  # has previous python
     ver = sys.version_info[0:2]
     py = f"py{''.join(str(i) for i in ver)}"
     prev_py = f"py{prev_ver}"
```

### Comparing `tox-4.6.0/tests/session/cmd/test_devenv.py` & `tox-4.6.1/tests/session/cmd/test_devenv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 import pytest
 
-from tox.pytest import ToxProjectCreator
+if TYPE_CHECKING:
+    from tox.pytest import ToxProjectCreator
 
 
 def test_devenv_fail_multiple_target(tox_project: ToxProjectCreator) -> None:
     outcome = tox_project({"tox.ini": ""}).run("d", "-e", "a,b")
     outcome.assert_failed()
     msg = "ROOT: HandledError| exactly one target environment allowed in devenv mode but found a, b\n"
     outcome.assert_out_err(msg, "")
 
 
 @pytest.mark.integration()
-def test_devenv_ok(tox_project: ToxProjectCreator, enable_pip_pypi_access: str | None) -> None:  # noqa: U100
+def test_devenv_ok(tox_project: ToxProjectCreator, enable_pip_pypi_access: str | None) -> None:  # noqa: ARG001
     content = {
         "setup.py": "from setuptools import setup\nsetup(name='demo', version='1.0')",
         "tox.ini": "[tox]\nenv_list = py\n[testenv]\nusedevelop = True",
     }
     project = tox_project(content)
     outcome = project.run("d", "-e", "py")
```

### Comparing `tox-4.6.0/tests/session/cmd/test_exec_.py` & `tox-4.6.1/tests/session/cmd/test_exec_.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import sys
+from typing import TYPE_CHECKING
 
 import pytest
 
-from tox.pytest import ToxProjectCreator
+if TYPE_CHECKING:
+    from tox.pytest import ToxProjectCreator
 
 
 @pytest.mark.parametrize("trail", [[], ["--"]], ids=["no_posargs", "empty_posargs"])
 def test_exec_fail_no_posargs(tox_project: ToxProjectCreator, trail: list[str]) -> None:
     outcome = tox_project({"tox.ini": ""}).run("e", "-e", "py39", *trail)
     outcome.assert_failed()
     msg = "ROOT: HandledError| You must specify a command as positional arguments, use -- <command>\n"
```

### Comparing `tox-4.6.0/tests/session/cmd/test_legacy.py` & `tox-4.6.1/tests/session/cmd/test_legacy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
-from pytest_mock import MockerFixture
 
-from tox.pytest import ToxProjectCreator
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import ToxProjectCreator
 
 
 def test_legacy_show_config(tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     show_config = mocker.patch("tox.session.cmd.legacy.show_config")
 
     outcome = tox_project({"tox.ini": ""}).run("le", "--showconfig")
```

### Comparing `tox-4.6.0/tests/session/cmd/test_list_envs.py` & `tox-4.6.1/tests/session/cmd/test_list_envs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 import pytest
 
-from tox.pytest import ToxProject, ToxProjectCreator
+if TYPE_CHECKING:
+    from tox.pytest import ToxProject, ToxProjectCreator
 
 
 @pytest.fixture()
 def project(tox_project: ToxProjectCreator) -> ToxProject:
     ini = """
     [tox]
     env_list=py32,py31,py
```

### Comparing `tox-4.6.0/tests/session/cmd/test_parallel.py` & `tox-4.6.1/tests/session/cmd/test_parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from __future__ import annotations
 
 import sys
 from argparse import ArgumentTypeError
-from pathlib import Path
 from signal import SIGINT
 from subprocess import PIPE, Popen
 from time import sleep
+from typing import TYPE_CHECKING
 
 import pytest
-from pytest_mock import MockerFixture
 
-from tox.pytest import MonkeyPatch, ToxProjectCreator
 from tox.session.cmd.run.parallel import parse_num_processes
 from tox.tox_env.api import ToxEnv
 from tox.tox_env.errors import Fail
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import MonkeyPatch, ToxProjectCreator
+
 
 def test_parse_num_processes_all() -> None:
     assert parse_num_processes("all") is None
 
 
 def test_parse_num_processes_auto() -> None:
     auto = parse_num_processes("auto")
@@ -39,18 +44,19 @@
     with pytest.raises(ArgumentTypeError, match="value must be positive"):
         parse_num_processes("-1")
 
 
 def test_parallel_general(tox_project: ToxProjectCreator, monkeypatch: MonkeyPatch, mocker: MockerFixture) -> None:
     def setup(self: ToxEnv) -> None:
         if self.name == "f":
-            raise Fail("something bad happened")
+            msg = "something bad happened"
+            raise Fail(msg)
         return prev_setup(self)
 
-    prev_setup = ToxEnv._setup_env
+    prev_setup = ToxEnv._setup_env  # noqa: SLF001
     mocker.patch.object(ToxEnv, "_setup_env", autospec=True, side_effect=setup)
     monkeypatch.setenv("PATH", "")
 
     ini = """
     [tox]
     no_package=true
     skip_missing_interpreters = true
@@ -118,27 +124,27 @@
 @pytest.mark.flaky(max_runs=3, min_passes=1)
 def test_keyboard_interrupt(tox_project: ToxProjectCreator, demo_pkg_inline: Path, tmp_path: Path) -> None:
     marker = tmp_path / "a"
     ini = f"""
     [testenv]
     package=wheel
     commands=python -c 'from time import sleep; from pathlib import Path; \
-                        p = Path("{str(marker)}"); p.write_text(""); sleep(100)'
+                        p = Path("{marker!s}"); p.write_text(""); sleep(100)'
     [testenv:dep]
     depends=py
     """
     proj = tox_project(
         {
             "tox.ini": ini,
             "pyproject.toml": (demo_pkg_inline / "pyproject.toml").read_text(),
             "build.py": (demo_pkg_inline / "build.py").read_text(),
         },
     )
     cmd = ["-c", str(proj.path / "tox.ini"), "p", "-p", "1", "-e", f"py,py{sys.version_info[0]},dep"]
-    process = Popen([sys.executable, "-m", "tox"] + cmd, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+    process = Popen([sys.executable, "-m", "tox", *cmd], stdout=PIPE, stderr=PIPE, universal_newlines=True)
     while not marker.exists():
         sleep(0.05)
     process.send_signal(SIGINT)
     out, err = process.communicate()
     assert process.returncode != 0
     assert "KeyboardInterrupt" in err, err
     assert "KeyboardInterrupt - teardown started\n" in out, out
```

### Comparing `tox-4.6.0/tests/session/cmd/test_quickstart.py` & `tox-4.6.1/tests/session/cmd/test_quickstart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 import sys
 from textwrap import dedent
+from typing import TYPE_CHECKING
 
 from packaging.version import Version
 
-from tox.pytest import ToxProjectCreator
 from tox.version import version as __version__
 
+if TYPE_CHECKING:
+    from tox.pytest import ToxProjectCreator
+
 
 def test_quickstart_ok(tox_project: ToxProjectCreator) -> None:
     project = tox_project({})
     tox_ini = project.path / "demo" / "tox.ini"
     assert not tox_ini.exists()
 
     outcome = project.run("q", str(tox_ini.parent))
```

### Comparing `tox-4.6.0/tests/session/cmd/test_sequential.py` & `tox-4.6.1/tests/session/cmd/test_sequential.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
 import json
 import os
 import re
 import sys
 from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import pytest
 from re_assert import Matches
 from virtualenv.discovery.py_info import PythonInfo
 
 from tox import __version__
-from tox.pytest import ToxProjectCreator
 from tox.tox_env.api import ToxEnv
 from tox.tox_env.info import Info
 
+if TYPE_CHECKING:
+    from tox.pytest import ToxProjectCreator
+
 
 @pytest.mark.parametrize("prefix", ["-", "- "])
 def test_run_ignore_cmd_exit_code(tox_project: ToxProjectCreator, prefix: str) -> None:
     cmd = [
         f"{prefix}python -c 'import sys; print(\"magic fail\", file=sys.stderr); sys.exit(1)'",
         "python -c 'import sys; print(\"magic pass\", file=sys.stdout); sys.exit(0)'",
     ]
@@ -53,15 +55,15 @@
     assert Matches(r"  congratulations :\) \(.* seconds\)") == reports[-1]
     assert Matches(r"  a: OK \([\d.]+ seconds\)") == reports[-2]
 
 
 @pytest.mark.integration()
 def test_result_json_sequential(
     tox_project: ToxProjectCreator,
-    enable_pip_pypi_access: str | None,  # noqa: U100
+    enable_pip_pypi_access: str | None,  # noqa: ARG001
 ) -> None:
     cmd = [
         "- python -c 'import sys; print(\"magic fail\", file=sys.stderr); sys.exit(1)'",
         "python -c 'import sys; print(\"magic pass\"); sys.exit(0)'",
     ]
     project = tox_project(
         {
@@ -184,15 +186,15 @@
     proj.patch_execute(lambda r: 0 if "install" in r.run_id else None)
 
     result_first = proj.run("r")
     result_first.assert_success()
     assert ".pkg: install" not in result_first.out  # no deps initially
 
     # new deps are picked up
-    (proj.path / "pyproject.toml").write_text(toml.replace("requires = []", 'requires = ["wheel"]'))
+    (proj.path / "pyproject.toml").write_text(toml.replace("requires = [\n]", 'requires = ["wheel"]'))
     (proj.path / "build.py").write_text(build.replace("return []", "return ['setuptools']"))
 
     result_rerun = proj.run("r")
     result_rerun.assert_success()
 
     # and installed
     rerun_install = [i for i in result_rerun.out.splitlines() if i.startswith(".pkg: install")]
```

### Comparing `tox-4.6.0/tests/session/cmd/test_show_config.py` & `tox-4.6.1/tests/session/cmd/test_show_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from __future__ import annotations
 
 import platform
 import sys
 from configparser import ConfigParser
-from pathlib import Path
 from textwrap import dedent
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 import pytest
-from pytest_mock import MockerFixture
 
 from tox.config.types import Command
-from tox.pytest import MonkeyPatch, ToxProjectCreator
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import MonkeyPatch, ToxProjectCreator
 
 
 def test_show_config_default_run_env(tox_project: ToxProjectCreator, monkeypatch: MonkeyPatch) -> None:
     py_ver = sys.version_info[0:2]
     name = f"py{py_ver[0]}{py_ver[1]}" if platform.python_implementation() == "CPython" else "pypy3"
     project = tox_project({"tox.ini": f"[tox]\nenv_list = {name}\n[testenv:{name}]\ncommands={{posargs}}"})
     result = project.run("c", "-e", name, "--core", "--", "magic")
@@ -99,15 +103,15 @@
     assert txt in outcome.out
 
 
 def test_show_config_empty_install_command_exception(tox_project: ToxProjectCreator) -> None:
     project = tox_project({"tox.ini": "[testenv:a]\ninstall_command="})
     outcome = project.run("c", "-e", "a", "-k", "install_command")
     outcome.assert_success()
-    txt = "\ninstall_command = # Exception: " "ValueError(\"attempting to parse '' into a command failed\")"
+    txt = "\ninstall_command = # Exception: ValueError(\"attempting to parse '' into a command failed\")"
     assert txt in outcome.out
 
 
 @pytest.mark.parametrize("stdout_is_atty", [True, False])
 def test_pass_env_config_default(tox_project: ToxProjectCreator, stdout_is_atty: bool, mocker: MockerFixture) -> None:
     mocker.patch("sys.stdout.isatty", return_value=stdout_is_atty)
     project = tox_project({"tox.ini": ""})
```

### Comparing `tox-4.6.0/tests/session/cmd/test_state.py` & `tox-4.6.1/tests/session/cmd/test_state.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
-from tox.pytest import ToxProjectCreator
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from tox.pytest import ToxProjectCreator
 
 
 def test_env_already_packaging(tox_project: ToxProjectCreator) -> None:
     proj = tox_project(
         {
             "tox.ini": "[testenv]\npackage=wheel",
             "pyproject.toml": '[build-system]\nrequires=[]\nbuild-backend="build"',
```

### Comparing `tox-4.6.0/tests/session/cmd/run/test_common.py` & `tox-4.6.1/tests/session/cmd/run/test_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
 import os
 import re
 from argparse import ArgumentError, ArgumentParser, Namespace
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
 
-from tox.pytest import ToxProjectCreator
 from tox.session.cmd.run.common import InstallPackageAction, SkipMissingInterpreterAction
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import ToxProjectCreator
+
 
 @pytest.mark.parametrize("values", ["config", None, "true", "false"])
 def test_skip_missing_interpreter_action_ok(values: str | None) -> None:
     args_namespace = Namespace()
     SkipMissingInterpreterAction(option_strings=["-i"], dest="into")(ArgumentParser(), args_namespace, values)
     expected = "true" if values is None else values
     assert args_namespace.into == expected
```

### Comparing `tox-4.6.0/tests/tox_env/test_api.py` & `tox-4.6.1/tests/tox_env/test_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
-from tox.pytest import ToxProjectCreator
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import ToxProjectCreator
 
 
 def test_ensure_temp_dir_exists(tox_project: ToxProjectCreator) -> None:
     ini = "[testenv]\ncommands=python -c 'import os; os.path.exists(r\"{temp_dir}\")'"
     project = tox_project({"tox.ini": ini})
     result = project.run()
     result.assert_success()
```

### Comparing `tox-4.6.0/tests/tox_env/test_register.py` & `tox-4.6.1/tests/tox_env/test_register.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with pytest.raises(ValueError, match="run env must be registered before setting it as default"):
         register.default_env_runner = "new-env"
 
 
 def test_register_set_new_default_with_register() -> None:
     class B(VirtualEnvRunner):
         @staticmethod
-        def id() -> str:
+        def id() -> str:  # noqa: A003
             return "B"
 
     register = ToxEnvRegister()
     register.add_run_env(VirtualEnvRunner)
     assert register.default_env_runner == VirtualEnvRunner.id()
     register.add_run_env(B)
     assert register.default_env_runner == VirtualEnvRunner.id()
```

### Comparing `tox-4.6.0/tests/tox_env/test_tox_env_api.py` & `tox-4.6.1/tests/tox_env/test_tox_env_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from __future__ import annotations
 
-from pathlib import Path
 from textwrap import dedent
+from typing import TYPE_CHECKING
 from unittest.mock import patch
 
 import pytest
 
-from tox.pytest import ToxProjectCreator
 from tox.tox_env.api import ToxEnv
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import ToxProjectCreator
+
 
 def test_recreate(tox_project: ToxProjectCreator) -> None:
     prj = tox_project({"tox.ini": "[testenv]\npackage=skip\nrecreate=True"})
     result_first = prj.run("r")
     result_first.assert_success()
 
     result_second = prj.run("r")
@@ -67,21 +71,21 @@
     result_second.assert_success()
     filename = {i.name for i in log_dir.iterdir()}
     assert filename == {"1-commands[0].log"}
 
 
 def test_tox_env_pass_env_literal_exist() -> None:
     with patch("os.environ", {"A": "1"}):
-        env = ToxEnv._load_pass_env(["A"])
+        env = ToxEnv._load_pass_env(["A"])  # noqa: SLF001
     assert env == {"A": "1"}
 
 
 def test_tox_env_pass_env_literal_miss() -> None:
     with patch("os.environ", {}):
-        env = ToxEnv._load_pass_env(["A"])
+        env = ToxEnv._load_pass_env(["A"])  # noqa: SLF001
     assert not env
 
 
 def test_tox_env_pass_env_fails_on_whitespace(tox_project: ToxProjectCreator) -> None:
     first, second = "A B", "C D"
     prj = tox_project({"tox.ini": f"[testenv]\npackage=skip\npass_env = {first}\n {second}\n  E"})
     result = prj.run("c", "-k", "pass_env")
@@ -101,15 +105,15 @@
     assert msg in result.out
 
 
 @pytest.mark.parametrize("glob", ["*", "?"])
 @pytest.mark.parametrize("char", ["a", "A"])
 def test_tox_env_pass_env_match_ignore_case(char: str, glob: str) -> None:
     with patch("os.environ", {"A1": "1", "a2": "2", "A2": "3", "B": "4"}):
-        env = ToxEnv._load_pass_env([f"{char}{glob}"])
+        env = ToxEnv._load_pass_env([f"{char}{glob}"])  # noqa: SLF001
     assert env == {"A1": "1", "a2": "2", "A2": "3"}
 
 
 def test_change_dir_is_created_if_not_exist(tox_project: ToxProjectCreator) -> None:
     prj = tox_project({"tox.ini": "[testenv]\npackage=skip\nchange_dir=a{/}b\ncommands=python --version"})
     result_first = prj.run("r")
     result_first.assert_success()
```

### Comparing `tox-4.6.0/tests/tox_env/test_tox_env_runner.py` & `tox-4.6.1/tests/tox_env/test_tox_env_runner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
-from pathlib import Path
+from typing import TYPE_CHECKING
 
-from tox.pytest import ToxProjectCreator
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import ToxProjectCreator
 
 
 def test_package_only(
     tox_project: ToxProjectCreator,
     demo_pkg_inline: Path,
 ) -> None:
     ini = "[testenv]\ncommands = python -c 'print('foo')'"
```

### Comparing `tox-4.6.0/tests/tox_env/python/test_python_api.py` & `tox-4.6.1/tests/tox_env/python/test_python_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
 
 import sys
-from pathlib import Path
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 
 import pytest
-from pytest_mock import MockerFixture
 
-from tox.pytest import ToxProjectCreator
 from tox.tox_env.errors import Fail
 from tox.tox_env.python.api import Python
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import ToxProjectCreator
+
 
 def test_requirements_txt(tox_project: ToxProjectCreator) -> None:
     prj = tox_project(
         {
             "tox.ini": "[testenv]\npackage=skip\ndeps=-rrequirements.txt",
             "requirements.txt": "nose",
         },
@@ -60,19 +64,19 @@
     ]
 
 
 def test_diff_msg_added_removed_changed() -> None:
     before = {"A": "1", "F": "8", "C": "3", "D": "4", "E": "6"}
     after = {"G": "9", "B": "2", "C": "3", "D": "5", "E": "7"}
     expected = "python added A='1' | F='8', removed G='9' | B='2', changed D='5'->'4' | E='7'->'6'"
-    assert Python._diff_msg(before, after) == expected
+    assert Python._diff_msg(before, after) == expected  # noqa: SLF001
 
 
 def test_diff_msg_no_diff() -> None:
-    assert Python._diff_msg({}, {}) == "python "
+    assert Python._diff_msg({}, {}) == "python "  # noqa: SLF001
 
 
 @pytest.mark.parametrize(
     ("env", "base_python"),
     [
         ("py3", "py3"),
         ("py311", "py311"),
@@ -107,15 +111,15 @@
     [
         ("magic", ["pypy"]),
         ("magic", ["py39"]),
     ],
     ids=lambda a: "|".join(a) if isinstance(a, list) else str(a),
 )
 def test_base_python_env_no_conflict(env: str, base_python: list[str], ignore_conflict: bool) -> None:
-    result = Python._validate_base_python(env, base_python, ignore_conflict)
+    result = Python._validate_base_python(env, base_python, ignore_conflict)  # noqa: SLF001
     assert result is base_python
 
 
 @pytest.mark.parametrize("ignore_conflict", [True, False])
 @pytest.mark.parametrize(
     ("env", "base_python", "expected", "conflict"),
     [
@@ -135,20 +139,20 @@
     env: str,
     base_python: list[str],
     expected: str,
     conflict: list[str],
     ignore_conflict: bool,
 ) -> None:
     if ignore_conflict:
-        result = Python._validate_base_python(env, base_python, ignore_conflict)
+        result = Python._validate_base_python(env, base_python, ignore_conflict)  # noqa: SLF001
         assert result == [expected]
     else:
         msg = f"env name {env} conflicting with base python {conflict[0]}"
         with pytest.raises(Fail, match=msg):
-            Python._validate_base_python(env, base_python, ignore_conflict)
+            Python._validate_base_python(env, base_python, ignore_conflict)  # noqa: SLF001
 
 
 @pytest.mark.parametrize("ignore_conflict", [True, False, None])
 def test_base_python_env_conflict_show_conf(tox_project: ToxProjectCreator, ignore_conflict: bool) -> None:
     py_ver = "".join(str(i) for i in sys.version_info[0:2])
     py_ver_next = "".join(str(i) for i in (sys.version_info[0], sys.version_info[1] + 2))
     ini = f"[testenv]\npackage=skip\nbase_python=py{py_ver_next}"
```

### Comparing `tox-4.6.0/tests/tox_env/python/test_python_runner.py` & `tox-4.6.1/tests/tox_env/python/test_python_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 import sys
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
 
 from tox.journal import EnvJournal
-from tox.pytest import ToxProjectCreator
 from tox.tox_env.package import PathPackage
 from tox.tox_env.python.runner import PythonRun
 
+if TYPE_CHECKING:
+    from tox.pytest import ToxProjectCreator
+
 
 def test_deps_config_path_req(tox_project: ToxProjectCreator) -> None:
     project = tox_project(
         {
             "tox.ini": "[testenv:py]\ndeps =-rpath.txt\n -r {toxinidir}{/}path2.txt\n pytest",
             "path.txt": "alpha",
             "path2.txt": "beta",
@@ -26,26 +29,26 @@
     assert deps.as_root_args == ["pytest", "-r", "path.txt", "-r", str(project.path / "path2.txt")]
     assert str(deps) == f"-r {project.path / 'tox.ini'}"
 
 
 def test_journal_package_empty() -> None:
     journal = EnvJournal(enabled=True, name="a")
 
-    PythonRun._handle_journal_package(journal, [])
+    PythonRun._handle_journal_package(journal, [])  # noqa: SLF001
 
     content = journal.content
     assert content == {}
 
 
 def test_journal_one_wheel_file(tmp_path: Path) -> None:
     wheel = tmp_path / "a.whl"
     wheel.write_bytes(b"magical")
     journal = EnvJournal(enabled=True, name="a")
 
-    PythonRun._handle_journal_package(journal, [PathPackage(wheel)])
+    PythonRun._handle_journal_package(journal, [PathPackage(wheel)])  # noqa: SLF001
 
     content = journal.content
     assert content == {
         "installpkg": {
             "basename": "a.whl",
             "sha256": "0ce2d4c7087733c06b1087b28db95e114d7caeb515b841c6cdec8960cf884654",
             "type": "file",
@@ -56,15 +59,15 @@
 def test_journal_multiple_wheel_file(tmp_path: Path) -> None:
     wheel_1 = tmp_path / "a.whl"
     wheel_1.write_bytes(b"magical")
     wheel_2 = tmp_path / "b.whl"
     wheel_2.write_bytes(b"magic")
     journal = EnvJournal(enabled=True, name="a")
 
-    PythonRun._handle_journal_package(journal, [PathPackage(wheel_1), PathPackage(wheel_2)])
+    PythonRun._handle_journal_package(journal, [PathPackage(wheel_1), PathPackage(wheel_2)])  # noqa: SLF001
 
     content = journal.content
     assert content == {
         "installpkg": [
             {
                 "basename": "a.whl",
                 "sha256": "0ce2d4c7087733c06b1087b28db95e114d7caeb515b841c6cdec8960cf884654",
@@ -78,15 +81,15 @@
         ],
     }
 
 
 def test_journal_package_dir(tmp_path: Path) -> None:
     journal = EnvJournal(enabled=True, name="a")
 
-    PythonRun._handle_journal_package(journal, [PathPackage(tmp_path)])
+    PythonRun._handle_journal_package(journal, [PathPackage(tmp_path)])  # noqa: SLF001
 
     content = journal.content
     assert content == {
         "installpkg": {
             "basename": tmp_path.name,
             "type": "dir",
         },
```

### Comparing `tox-4.6.0/tests/tox_env/python/pip/test_pip_install.py` & `tox-4.6.1/tests/tox_env/python/pip/test_pip_install.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 
 import os
-from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from unittest.mock import Mock
 
 import pytest
 from packaging.requirements import Requirement
 
-from tox.pytest import CaptureFixture, SubRequest, ToxProject, ToxProjectCreator
 from tox.tox_env.errors import Fail
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import CaptureFixture, SubRequest, ToxProject, ToxProjectCreator
+
 
 @pytest.mark.parametrize("arg", [object, [object]])
 def test_pip_install_bad_type(tox_project: ToxProjectCreator, capfd: CaptureFixture, arg: Any) -> None:
     proj = tox_project({"tox.ini": ""})
     result = proj.run("l")
     result.assert_success()
     pip = result.state.envs["py"].installer
@@ -97,24 +100,24 @@
     proj = tox_project({"tox.ini": f"[testenv:py]\ndeps={content}\nskip_install=true"})
     execute_calls = proj.patch_execute(lambda r: 0 if "install" in r.run_id else None)
 
     result = proj.run("r")
     result.assert_success()
 
     assert execute_calls.call_count == 1
-    assert execute_calls.call_args[0][3].cmd == ["python", "-I", "-m", "pip", "install"] + args
+    assert execute_calls.call_args[0][3].cmd == ["python", "-I", "-m", "pip", "install", *args]
 
     # check that adding a new dependency correctly finds the previous one
     (proj.path / "tox.ini").write_text(f"[testenv:py]\ndeps={content}\n a\nskip_install=true")
     execute_calls.reset_mock()
 
     result_second = proj.run("r")
     result_second.assert_success()
     assert execute_calls.call_count == 1
-    assert execute_calls.call_args[0][3].cmd == ["python", "-I", "-m", "pip", "install", "a"] + args
+    assert execute_calls.call_args[0][3].cmd == ["python", "-I", "-m", "pip", "install", "a", *args]
 
 
 def test_pip_req_path(tox_project: ToxProjectCreator) -> None:
     proj = tox_project({"tox.ini": "[testenv:py]\ndeps=.\nskip_install=true"})
     execute_calls = proj.patch_execute(lambda r: 0 if "install" in r.run_id else None)
 
     result = proj.run("r")
@@ -122,15 +125,15 @@
 
     assert execute_calls.call_count == 1
     assert execute_calls.call_args[0][3].cmd == ["python", "-I", "-m", "pip", "install", "."]
 
 
 def test_deps_remove_recreate(tox_project: ToxProjectCreator) -> None:
     proj = tox_project({"tox.ini": "[testenv]\npackage=skip\ndeps=wheel\n setuptools"})
-    execute_calls = proj.patch_execute(lambda request: 0)  # noqa: U100
+    execute_calls = proj.patch_execute(lambda request: 0)  # noqa: ARG005
     result_first = proj.run("r")
     result_first.assert_success()
     assert execute_calls.call_count == 1
 
     (proj.path / "tox.ini").write_text("[testenv]\npackage=skip\ndeps=setuptools\n")
     result_second = proj.run("r")
     result_second.assert_success()
@@ -172,15 +175,15 @@
 
 
 def test_pkg_env_dep_remove_recreate(tox_project: ToxProjectCreator, demo_pkg_inline: Path) -> None:
     toml = (demo_pkg_inline / "pyproject.toml").read_text()
     proj = tox_project(
         {
             "tox.ini": "[testenv]\npackage=wheel",
-            "pyproject.toml": toml.replace("requires = []", 'requires = ["setuptools"]'),
+            "pyproject.toml": toml.replace("requires = [\n]", 'requires = ["setuptools"]'),
             "build.py": (demo_pkg_inline / "build.py").read_text(),
         },
     )
     execute_calls = proj.patch_execute(lambda r: 0 if "install" in r.run_id else None)
     result_first = proj.run("r")
     result_first.assert_success()
     run_ids = [i[0][3].run_id for i in execute_calls.call_args_list]
@@ -297,15 +300,15 @@
     tox_project: ToxProjectCreator,
     demo_pkg_inline: Path,
     constrain_package_deps: bool,
     use_frozen_constraints: bool,
 ) -> tuple[ToxProject, list[str]]:
     toml = (demo_pkg_inline / "pyproject.toml").read_text()
     files = {
-        "pyproject.toml": toml.replace("requires = []", 'requires = ["setuptools"]')
+        "pyproject.toml": toml.replace("requires = [\n]", 'requires = ["setuptools"]')
         + '\n[project]\nname = "demo"\nversion = "0.1"\ndependencies = ["foo > 2"]',
         "build.py": (demo_pkg_inline / "build.py").read_text(),
     }
     exp_constraints: list[str] = []
     requirement = "foo==1.2.3"
     constraint = "foo<2"
     if request.param == "explicit":
```

### Comparing `tox-4.6.0/tests/tox_env/python/pip/test_req_file.py` & `tox-4.6.1/tests/tox_env/python/pip/test_req_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 from argparse import Namespace
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
 
 from tox.tox_env.python.pip.req_file import PythonDeps
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 @pytest.mark.parametrize("legacy_flag", ["-r", "-c"])
 def test_legacy_requirement_file(tmp_path: Path, legacy_flag: str) -> None:
     python_deps = PythonDeps(f"{legacy_flag}a.txt", tmp_path)
     (tmp_path / "a.txt").write_text("b")
     assert python_deps.as_root_args == [legacy_flag, "a.txt"]
     assert vars(python_deps.options) == {}
@@ -52,15 +55,15 @@
     assert python_deps.as_root_args == ["-r", "r.txt", "--no-deps"]
 
 
 def test_req_with_no_deps(tmp_path: Path) -> None:
     (tmp_path / "r.txt").write_text("--no-deps")
     python_deps = PythonDeps(raw="-rr.txt", root=tmp_path)
     with pytest.raises(ValueError, match="unrecognized arguments: --no-deps"):
-        python_deps.requirements
+        python_deps.requirements  # noqa: B018
 
 
 def test_opt_only_req_file(tmp_path: Path) -> None:
     (tmp_path / "r.txt").write_text("--use-feature fast-deps")
     python_deps = PythonDeps(raw="-rr.txt", root=tmp_path)
     assert not python_deps.requirements
     assert python_deps.options == Namespace(features_enabled=["fast-deps"])
```

### Comparing `tox-4.6.0/tests/tox_env/python/pip/req/test_file.py` & `tox-4.6.1/tests/tox_env/python/pip/req/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from __future__ import annotations
 
 import os
 import sys
 from contextlib import contextmanager
 from io import BytesIO
-from pathlib import Path
-from typing import IO, Any, Iterator
+from typing import IO, TYPE_CHECKING, Any, Iterator
 
 import pytest
-from pytest_mock import MockerFixture
 
-from tox.pytest import CaptureFixture, MonkeyPatch
 from tox.tox_env.python.pip.req.file import ParsedRequirement, RequirementsFile
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import CaptureFixture, MonkeyPatch
+
 _REQ_FILE_TEST_CASES = [
     pytest.param("--pre", {"pre": True}, [], ["--pre"], id="pre"),
     pytest.param("--no-index", {"index_url": []}, [], ["--no-index"], id="no-index"),
     pytest.param("--no-index\n-i a\n--no-index", {"index_url": []}, [], ["--no-index"], id="no-index overwrites index"),
     pytest.param("--prefer-binary", {"prefer_binary": True}, [], ["--prefer-binary"], id="prefer-binary"),
     pytest.param("--require-hashes", {"require_hashes": True}, [], ["--require-hashes"], id="requires-hashes"),
     pytest.param("--pre ", {"pre": True}, [], ["--pre"], id="space after"),
@@ -414,15 +418,15 @@
     assert found == ["-c magic", "-c magical"]
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason=r"on windows the escaped \ is overloaded by path separator")
 def test_req_path_with_space_escape(tmp_path: Path) -> None:
     dep_requirements_file = tmp_path / "a b"
     dep_requirements_file.write_text("c")
-    path = f"-r {str(dep_requirements_file)}"
+    path = f"-r {dep_requirements_file!s}"
     path = f'{path[:-len("a b")]}a\\ b'
 
     requirements_file = tmp_path / "req.txt"
     requirements_file.write_text(path)
     req_file = RequirementsFile(requirements_file, constraint=False)
 
     assert vars(req_file.options) == {}
```

### Comparing `tox-4.6.0/tests/tox_env/python/virtual_env/test_setuptools.py` & `tox-4.6.1/tests/tox_env/python/virtual_env/test_setuptools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 import os
 import sys
-from pathlib import Path
-from typing import cast
+from typing import TYPE_CHECKING, cast
 
 import pytest
 
-from tox.pytest import ToxProjectCreator
 from tox.tox_env.python.package import WheelPackage
 from tox.tox_env.python.virtual_env.package.pyproject import Pep517VirtualEnvPackager
 from tox.tox_env.runner import RunToxEnv
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import ToxProjectCreator
+
 
 @pytest.mark.integration()
 def test_setuptools_package(
     tox_project: ToxProjectCreator,
     demo_pkg_setuptools: Path,
-    enable_pip_pypi_access: str | None,  # noqa: U100
+    enable_pip_pypi_access: str | None,  # noqa: ARG001
 ) -> None:
     tox_ini = """
         [testenv]
         package = wheel
         commands_pre = python -c 'import sys; print("start", sys.executable)'
         commands = python -c 'from demo_pkg_setuptools import do; do()'
         commands_post = python -c 'import sys; print("end", sys.executable)'
```

### Comparing `tox-4.6.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py` & `tox-4.6.1/tests/tox_env/python/virtual_env/test_virtualenv_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
 import os
 import sys
+from typing import TYPE_CHECKING
 
 import pytest
-from pytest_mock import MockerFixture
 from virtualenv import __version__ as virtualenv_version
 from virtualenv import session_via_cli
 from virtualenv.config.cli.parser import VirtualEnvOptions
 
-from tox.execute import ExecuteRequest
-from tox.pytest import MonkeyPatch, ToxProject, ToxProjectCreator
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tox.execute import ExecuteRequest
+    from tox.pytest import MonkeyPatch, ToxProject, ToxProjectCreator
 
 
 @pytest.fixture()
 def virtualenv_opt(monkeypatch: MonkeyPatch, mocker: MockerFixture) -> VirtualEnvOptions:
     for key in os.environ:
         if key.startswith("VIRTUALENV_"):  # pragma: no cover
             monkeypatch.delenv(key)  # pragma: no cover
     opts = VirtualEnvOptions()
     mocker.patch(
         "tox.tox_env.python.virtual_env.api.session_via_cli",
-        side_effect=lambda args, options, setup_logging, env: session_via_cli(  # noqa: U100
+        side_effect=lambda args, options, setup_logging, env: session_via_cli(  # noqa: ARG005
             args,
             opts,
             setup_logging,
             env,
         ),
     )
     return opts
```

### Comparing `tox-4.6.0/tests/tox_env/python/virtual_env/package/conftest.py` & `tox-4.6.1/tests/tox_env/python/virtual_env/package/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
 import sys
-from pathlib import Path
 from textwrap import dedent
+from typing import TYPE_CHECKING
 
 import pytest
-from _pytest.tmpdir import TempPathFactory
+
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from _pytest.tmpdir import TempPathFactory
 
 
 @pytest.fixture(scope="session")
 def pkg_with_extras_project(tmp_path_factory: TempPathFactory) -> Path:
     py_ver = ".".join(str(i) for i in sys.version_info[0:2])
     setup_cfg = f"""
     [metadata]
```

### Comparing `tox-4.6.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py` & `tox-4.6.1/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
-from pathlib import Path
-from typing import Callable
+from typing import TYPE_CHECKING, Callable
 from zipfile import ZipFile
 
 import pytest
 
-from tox.pytest import ToxProjectCreator
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import ToxProjectCreator
 
 
 @pytest.fixture(scope="session")
 def pkg_with_extras_project_wheel(
     pkg_with_extras_project: Path,
     pkg_builder: Callable[[Path, Path, list[str], bool], Path],
 ) -> Path:
@@ -85,15 +87,15 @@
     [testenv:.ext]
     deps = build
     package_glob = {envtmpdir}{/}dist{/}*.whl
     commands =
         pyproject-build -w . -o {envtmpdir}{/}dist
     """
     project = tox_project({"tox.ini": ini})
-    result = project.run("r", "--root", str(demo_pkg_inline))
+    result = project.run("r", "--root", str(demo_pkg_inline), "--workdir", str(project.path))
 
     result.assert_success()
     assert "greetings from demo_pkg_inline" in result.out
 
 
 def test_build_wheel_external_fail_build(tox_project: ToxProjectCreator) -> None:
     ini = """
```

### Comparing `tox-4.6.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py` & `tox-4.6.1/tests/tox_env/python/virtual_env/package/test_package_pyproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
-from pathlib import Path
 from textwrap import dedent
+from typing import TYPE_CHECKING
 
 import pytest
 
-from tox.pytest import ToxProjectCreator
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    from tox.pytest import ToxProjectCreator
 
 
 @pytest.mark.parametrize(
     "pkg_type",
     ["editable-legacy", "editable", "sdist", "wheel"],
 )
 def test_tox_ini_package_type_valid(tox_project: ToxProjectCreator, pkg_type: str) -> None:
@@ -163,15 +166,15 @@
     if deps:
         expected_calls.append(("py", "install_package_deps"))
     expected_calls.extend((("py", "install_package"), (".pkg", "_exit")))
     found_calls = [(i[0][0].conf.name, i[0][3].run_id) for i in execute_calls.call_args_list]
     assert found_calls == expected_calls
 
     if deps:
-        expected_args = ["python", "-I", "-m", "pip", "install"] + deps
+        expected_args = ["python", "-I", "-m", "pip", "install", *deps]
         args = execute_calls.call_args_list[-3][0][3].cmd
         assert expected_args == args
 
 
 @pytest.mark.parametrize(
     ("metadata", "dynamic", "deps"),
     [
@@ -186,15 +189,15 @@
             "Requires-Dist: A\nRequires-Dist: B;extra=='alpha'",
             "['optional-dependencies']",
             ["A", "B"],
             id="deps_extra_dynamic_opt",
         ),
     ],
 )
-def test_pyproject_deps_static_with_dynamic(
+def test_pyproject_deps_static_with_dynamic(  # noqa: PLR0913
     tox_project: ToxProjectCreator,
     demo_pkg_inline: Path,
     monkeypatch: pytest.MonkeyPatch,
     metadata: str,
     dynamic: str,
     deps: list[str],
 ) -> None:
```

### Comparing `tox-4.6.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py` & `tox-4.6.1/tests/tox_env/python/virtual_env/package/test_python_package_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 import sys
 from itertools import zip_longest
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
 from packaging.requirements import Requirement
 from pyproject_api import SubprocessFrontend
 
 from tox.tox_env.python.virtual_env.package.util import dependencies_with_extras
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 if sys.version_info >= (3, 8):  # pragma: no cover (py38+)
     from importlib.metadata import Distribution, PathDistribution
 else:  # pragma: no cover (<py38)
     from importlib_metadata import Distribution, PathDistribution
 
 
 @pytest.fixture(scope="session")
```

### Comparing `tox-4.6.0/tests/util/test_ci.py` & `tox-4.6.1/tests/util/test_ci.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         "GITHUB_ACTIONS": "true",  # GitHub Actions
         "GITLAB_CI": None,  # GitLab CI
         "HEROKU_TEST_RUN_ID": None,  # Heroku CI
         "BUILD_ID": None,  # Hudson
         "TEAMCITY_VERSION": None,  # TeamCity
         "TRAVIS": "true",  # Travis CI
     }.items(),
-    ids=lambda v: v[0],  # type: ignore
+    ids=lambda v: v[0],  # type: ignore[no-any-return]
 )
 def test_is_ci(env_var: tuple[str, str | None], monkeypatch: pytest.MonkeyPatch) -> None:
     for var in _ENV_VARS:
         monkeypatch.delenv(var, raising=False)
     monkeypatch.setenv(env_var[0], env_var[1] or "")
     assert is_ci()
 
@@ -37,15 +37,15 @@
         "TF_BUILD": "",  # Azure Pipelines
         "BUILDKITE": "",  # Buildkite
         "CIRCLECI": "",  # Circle CI
         "CIRRUS_CI": "",  # Cirrus CI
         "GITHUB_ACTIONS": "",  # GitHub Actions
         "TRAVIS": "",  # Travis CI
     }.items(),
-    ids=lambda v: v[0],  # type: ignore
+    ids=lambda v: v[0],  # type: ignore[no-any-return]
 )
 def test_is_ci_bad_set(env_var: tuple[str, str], monkeypatch: pytest.MonkeyPatch) -> None:
     for var in _ENV_VARS:
         monkeypatch.delenv(var, raising=False)
     monkeypatch.setenv(env_var[0], env_var[1])
     assert not is_ci()
```

### Comparing `tox-4.6.0/tests/util/test_graph.py` & `tox-4.6.1/tests/util/test_graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/tests/util/test_spinner.py` & `tox-4.6.1/tests/util/test_spinner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from __future__ import annotations
 
 import os
 import sys
 import time
+from typing import TYPE_CHECKING
 
 import pytest
 import time_machine
 from colorama import Fore
-from pytest_mock import MockerFixture
 
-from tox.pytest import CaptureFixture, MonkeyPatch
 from tox.util import spinner
 
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
+    from tox.pytest import CaptureFixture, MonkeyPatch
+
 
 @time_machine.travel("2012-01-14", tick=False)
 def test_spinner(capfd: CaptureFixture, monkeypatch: MonkeyPatch) -> None:
     monkeypatch.setattr(sys.stdout, "isatty", lambda: False)
     with spinner.Spinner(refresh_rate=100) as spin:
         for _ in range(len(spin.frames)):
             spin.stream.write("\n")
@@ -36,15 +40,15 @@
         spin.add("x")
         for _ in range(len(spin.frames)):
             spin.render_frame()
         spin.finalize("x", "done", Fore.GREEN)
         spin.clear()
     out, err = capfd.readouterr()
     assert out == f"{Fore.GREEN}x: done in 0 seconds{Fore.RESET}{os.linesep}", out
-    assert err == ""
+    assert not err
 
 
 @time_machine.travel("2012-01-14", tick=False)
 def test_spinner_progress(capfd: CaptureFixture, monkeypatch: MonkeyPatch) -> None:
     monkeypatch.setattr(sys.stdout, "isatty", lambda: False)
     with spinner.Spinner() as spin:
         for _ in range(len(spin.frames)):  # pragma: no branch
```

### Comparing `tox-4.6.0/LICENSE` & `tox-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/README.md` & `tox-4.6.1/README.md`

 * *Files identical despite different names*

### Comparing `tox-4.6.0/pyproject.toml` & `tox-4.6.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.17",
+  "hatchling>=1.17.1",
 ]
 
 [project]
 name = "tox"
 description = "tox is a generic virtualenv management and test command line tool"
 readme.content-type = "text/markdown"
 readme.file = "README.md"
@@ -29,87 +29,91 @@
   "Development Status :: 5 - Production/Stable",
   "Framework :: tox",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
-  "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Testing",
   "Topic :: Utilities",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "cachetools>=5.3",
+  "cachetools>=5.3.1",
   "chardet>=5.1",
   "colorama>=0.4.6",
-  "filelock>=3.12",
+  "filelock>=3.12.2",
   'importlib-metadata>=6.6; python_version < "3.8"',
   "packaging>=23.1",
-  "platformdirs>=3.5.1",
+  "platformdirs>=3.5.3",
   "pluggy>=1",
   "pyproject-api>=1.5.1",
   'tomli>=2.0.1; python_version < "3.11"',
-  'typing-extensions>=4.6.2; python_version < "3.8"',
+  'typing-extensions>=4.6.3; python_version < "3.8"',
   "virtualenv>=20.23",
 ]
 optional-dependencies.docs = [
   "furo>=2023.5.20",
   "sphinx>=7.0.1",
   "sphinx-argparse-cli>=1.11",
   "sphinx-autodoc-typehints!=1.23.4,>=1.23",
   "sphinx-copybutton>=0.5.2",
   "sphinx-inline-tabs>=2023.4.21",
   "sphinxcontrib-towncrier>=0.2.1a0",
-  "towncrier>=22.12",
+  "towncrier>=23.6",
 ]
 optional-dependencies.testing = [
   "build[virtualenv]>=0.10",
   "covdefaults>=2.3",
+  "detect-test-pollution>=1.1.1",
   "devpi-process>=0.3",
-  "diff-cover>=7.5",
+  "diff-cover>=7.6",
   "distlib>=0.3.6",
   "flaky>=3.7",
   "hatch-vcs>=0.3",
-  "hatchling>=1.17",
+  "hatchling>=1.17.1",
   "psutil>=5.9.5",
-  "pytest>=7.3.1",
+  "pytest>=7.3.2",
   "pytest-cov>=4.1",
   "pytest-mock>=3.10",
   "pytest-xdist>=3.3.1",
   "re-assert>=1.1",
   'time-machine>=2.9; implementation_name != "pypy"',
   "wheel>=0.40",
 ]
 urls.Documentation = "https://tox.wiki"
 urls.Homepage = "http://tox.readthedocs.org"
 urls."Release Notes" = "https://tox.wiki/en/latest/changelog.html"
 urls.Source = "https://github.com/tox-dev/tox"
 urls.Tracker = "https://github.com/tox-dev/tox/issues"
 scripts.tox = "tox.run:run"
 
-
 [tool.hatch]
 build.dev-mode-dirs = ["src"]
 build.hooks.vcs.version-file = "src/tox/version.py"
 build.targets.sdist.include = ["/src", "/tests", "/tox.ini"]
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+addopts = "--tb=auto -ra --showlocals --no-success-flaky-report"
+
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
 paths.source = [
   "src",
   ".tox*/*/lib/python*/site-packages",
   ".tox*/pypy*/site-packages",
@@ -118,19 +122,14 @@
   "*\\src",
 ]
 report.fail_under = 88
 report.omit = ["src/tox/config/cli/for_docs.py", "tests/execute/local_subprocess/bad_process.py", "tests/type_check/*"]
 run.parallel = true
 run.plugins = ["covdefaults"]
 
-[tool.isort]
-known_first_party = ["tox", "tests"]
-profile = "black"
-line_length = 120
-
 [tool.mypy]
 python_version = "3.11"
 show_error_codes = true
 strict = true
 overrides = [
   { module = [
     "colorama.*",
@@ -141,33 +140,40 @@
     "pluggy.*",
     "psutil.*",
     "re_assert.*",
     "virtualenv.*",
   ], ignore_missing_imports = true },
 ]
 
-[tool.pep8]
-max-line-length = "120"
-
-[tool.flake8]
-max-complexity = 22
-max-line-length = 120
-unused-arguments-ignore-abstract-functions = true
-noqa-require-code = true
-dictionaries = ["en_US", "python", "technical", "django"]
-ignore = [
-  "E203", # whitespace before ':'
-  "W503", #  line break before binary operator
-]
-
-[tool.pytest.ini_options]
-testpaths = ["tests"]
-addopts = "--tb=auto -ra --showlocals --no-success-flaky-report"
-
 [tool.towncrier]
 name = "tox"
 filename = "docs/changelog.rst"
 directory = "docs/changelog"
 title_format = false
 issue_format = ":issue:`{issue}`"
 template = "docs/changelog/template.jinja2"
 # possible types, all default: feature, bugfix, doc, removal, misc
+
+[tool.ruff]
+select = ["ALL"]
+line-length = 120
+target-version = "py37"
+isort = {known-first-party = ["tox", "tests"], required-imports = ["from __future__ import annotations"]}
+ignore = [
+  "INP001",  # no implicit namespaces here
+  "D",  # ignore documentation for now
+  "ANN401",  # Dynamically typed expressions (typing.Any) are disallowed in `arg`"
+  "ANN101",  # Missing type annotation for `self` in method
+  "ANN102",  # Missing type annotation for `cls` in classmethod"
+  "D203",  # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
+  "D212",  # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
+  "S104",  # Possible binding to all interface
+]
+[tool.ruff.per-file-ignores]
+"tests/**/*.py" = [
+  "S101",  # asserts allowed in tests...
+  "FBT",  # don"t care about booleans as positional arguments in tests
+  "INP001", # no implicit namespace
+  "D",  # don"t care about documentation in tests
+  "S603",  # `subprocess` call: check for execution of untrusted input
+  "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
+]
```

### Comparing `tox-4.6.0/PKG-INFO` & `tox-4.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox
-Version: 4.6.0
+Version: 4.6.1
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, http://tox.readthedocs.org
 Project-URL: Release Notes, https://tox.wiki/en/latest/changelog.html
 Project-URL: Source, https://github.com/tox-dev/tox
 Project-URL: Tracker, https://github.com/tox-dev/tox/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -15,60 +15,61 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Requires-Dist: cachetools>=5.3
+Requires-Dist: cachetools>=5.3.1
 Requires-Dist: chardet>=5.1
 Requires-Dist: colorama>=0.4.6
-Requires-Dist: filelock>=3.12
+Requires-Dist: filelock>=3.12.2
 Requires-Dist: importlib-metadata>=6.6; python_version < '3.8'
 Requires-Dist: packaging>=23.1
-Requires-Dist: platformdirs>=3.5.1
+Requires-Dist: platformdirs>=3.5.3
 Requires-Dist: pluggy>=1
 Requires-Dist: pyproject-api>=1.5.1
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
-Requires-Dist: typing-extensions>=4.6.2; python_version < '3.8'
+Requires-Dist: typing-extensions>=4.6.3; python_version < '3.8'
 Requires-Dist: virtualenv>=20.23
 Provides-Extra: docs
 Requires-Dist: furo>=2023.5.20; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.11; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs>=2023.4.21; extra == 'docs'
 Requires-Dist: sphinx>=7.0.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-towncrier>=0.2.1a0; extra == 'docs'
-Requires-Dist: towncrier>=22.12; extra == 'docs'
+Requires-Dist: towncrier>=23.6; extra == 'docs'
 Provides-Extra: testing
 Requires-Dist: build[virtualenv]>=0.10; extra == 'testing'
 Requires-Dist: covdefaults>=2.3; extra == 'testing'
+Requires-Dist: detect-test-pollution>=1.1.1; extra == 'testing'
 Requires-Dist: devpi-process>=0.3; extra == 'testing'
-Requires-Dist: diff-cover>=7.5; extra == 'testing'
+Requires-Dist: diff-cover>=7.6; extra == 'testing'
 Requires-Dist: distlib>=0.3.6; extra == 'testing'
 Requires-Dist: flaky>=3.7; extra == 'testing'
 Requires-Dist: hatch-vcs>=0.3; extra == 'testing'
-Requires-Dist: hatchling>=1.17; extra == 'testing'
+Requires-Dist: hatchling>=1.17.1; extra == 'testing'
 Requires-Dist: psutil>=5.9.5; extra == 'testing'
 Requires-Dist: pytest-cov>=4.1; extra == 'testing'
 Requires-Dist: pytest-mock>=3.10; extra == 'testing'
 Requires-Dist: pytest-xdist>=3.3.1; extra == 'testing'
-Requires-Dist: pytest>=7.3.1; extra == 'testing'
+Requires-Dist: pytest>=7.3.2; extra == 'testing'
 Requires-Dist: re-assert>=1.1; extra == 'testing'
 Requires-Dist: time-machine>=2.9; implementation_name != 'pypy' and extra == 'testing'
 Requires-Dist: wheel>=0.40; extra == 'testing'
 Description-Content-Type: text/markdown
 
 # tox
```

