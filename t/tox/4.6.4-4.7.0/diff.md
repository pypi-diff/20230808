# Comparing `tmp/tox-4.6.4.tar.gz` & `tmp/tox-4.7.0.tar.gz`

## Comparing `tox-4.6.4.tar` & `tox-4.7.0.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tox-4.6.4/tox.ini
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/__main__.py
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/provision.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/py.typed
--rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/pytest.py
--rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/report.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/run.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/__init__.py
--rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/main.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/of_type.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/set_env.py
--rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/sets.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/__init__.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/env_var.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/ini.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/parse.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/cli/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/__init__.py
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/api.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/convert.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/memory.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/section.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/str_convert.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/stringify.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/ini/__init__.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/ini/factor.py
--rw-r--r--   0        0        0    13368 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/loader/ini/replace.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/__init__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/api.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/discover.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/ini.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/ini_section.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/legacy_toml.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/setup_cfg.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/config/source/tox_ini.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/__init__.py
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/api.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/pep517_backend.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/request.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/stream.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/util.py
--rw-r--r--   0        0        0    14203 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/local_sub_process/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread_unix.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread_windows.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/journal/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/journal/env.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/journal/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/plugin/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/plugin/inline.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/plugin/manager.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/plugin/spec.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/__init__.py
--rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/env_select.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/depends.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/devenv.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/exec_.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/legacy.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/list_env.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/quickstart.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/show_config.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/version_flag.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/__init__.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/common.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/parallel.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/sequential.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/session/cmd/run/single.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/__init__.py
--rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/api.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/errors.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/info.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/installer.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/package.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/register.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/runner.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/api.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/package.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/__init__.py
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/pip_install.py
--rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req_file.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req/__init__.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req/args.py
--rw-r--r--   0        0        0    19702 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req/file.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/pip/req/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/api.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
--rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/package/pyproject.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/tox_env/python/virtual_env/package/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/ci.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/cpu.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/file_view.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/graph.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/path.py
--rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 tox-4.6.4/src/tox/util/spinner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/__init__.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.6.4/tests/conftest.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_call_modes.py
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_provision.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_report.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_run.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.4/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/__init__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/conftest.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_main.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_of_types.py
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_set_env.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_sets.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/conftest.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/test_cli_env_var.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/test_cli_ini.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/test_parse.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/cli/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/test_loader.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/test_memory_loader.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/test_section.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/test_str_convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/conftest.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/test_factor.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/test_ini_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/__init__.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/conftest.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_env_var.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_os_pathsep.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_os_sep.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_posargs.py
--rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_tox_env.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/loader/ini/replace/test_replace_tty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/test_discover.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/test_legacy_toml.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/test_setup_cfg.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.6.4/tests/config/source/test_source_ini.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.6.4/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/conftest.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/test_request.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/test_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/bad_process.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/local_subprocess_sigint.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/test_execute_util.py
--rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/test_local_subprocess.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.6.4/tests/execute/local_subprocess/tty_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/journal/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.4/tests/journal/test_main_journal.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.4/tests/plugin/conftest.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.6.4/tests/plugin/test_inline.py
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 tox-4.6.4/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.6.4/tests/plugin/test_plugin_custom_config_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/pytest_/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.6.4/tests/pytest_/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/__init__.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/test_env_select.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/test_session_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/__init__.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_depends.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_devenv.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_exec_.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_legacy.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_list_envs.py
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_parallel.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_quickstart.py
--rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_sequential.py
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_show_config.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/run/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.6.4/tests/session/cmd/run/test_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_api.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_info.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_register.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_tox_env_api.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/test_tox_env_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/__init__.py
--rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/test_python_api.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/test_python_runner.py
--rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/pip/test_pip_install.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/pip/test_req_file.py
--rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/pip/req/test_file.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/test-pkg/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/test_setuptools.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/test_virtualenv_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/conftest.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
--rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.6.4/tests/tox_env/python/virtual_env/package/test_python_package_util.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.6.4/tests/type_check/add_config_container_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/__init__.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_ci.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_cpu.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_graph.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_path.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.6.4/tests/util/test_spinner.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.4/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.4/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.4/README.md
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 tox-4.6.4/pyproject.toml
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 tox-4.6.4/PKG-INFO
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tox-4.7.0/tox.ini
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/__main__.py
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/provision.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/py.typed
+-rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/pytest.py
+-rw-r--r--   0        0        0     8303 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/report.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/run.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/__init__.py
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/main.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/of_type.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/set_env.py
+-rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/sets.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/cli/__init__.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/cli/env_var.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/cli/ini.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/cli/parse.py
+-rw-r--r--   0        0        0    13744 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/cli/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/__init__.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/api.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/convert.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/memory.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/section.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/str_convert.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/stringify.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/ini/factor.py
+-rw-r--r--   0        0        0    13385 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/loader/ini/replace.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/source/__init__.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/source/api.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/source/discover.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/source/ini.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/source/ini_section.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/source/legacy_toml.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/source/setup_cfg.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/config/source/tox_ini.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/__init__.py
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/api.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/pep517_backend.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/request.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/stream.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/util.py
+-rw-r--r--   0        0        0    14187 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/local_sub_process/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/local_sub_process/read_via_thread.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/local_sub_process/read_via_thread_unix.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/execute/local_sub_process/read_via_thread_windows.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/journal/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/journal/env.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/journal/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/plugin/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/plugin/inline.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/plugin/manager.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/plugin/spec.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/__init__.py
+-rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/env_select.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/depends.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/devenv.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/exec_.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/legacy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/list_env.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/quickstart.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/show_config.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/version_flag.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0    17664 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/run/common.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/run/parallel.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/run/sequential.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/session/cmd/run/single.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/__init__.py
+-rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/api.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/errors.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/info.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/installer.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/package.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/register.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/runner.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/api.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/package.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/pip/__init__.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/pip/pip_install.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/pip/req_file.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/pip/req/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/pip/req/args.py
+-rw-r--r--   0        0        0    19719 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/pip/req/file.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/pip/req/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/virtual_env/api.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/virtual_env/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
+-rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/virtual_env/package/pyproject.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/tox_env/python/virtual_env/package/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/util/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/util/ci.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/util/cpu.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/util/file_view.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/util/graph.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/util/path.py
+-rw-r--r--   0        0        0     6870 2020-02-02 00:00:00.000000 tox-4.7.0/src/tox/util/spinner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.7.0/tests/test_call_modes.py
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.7.0/tests/test_provision.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.7.0/tests/test_report.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.7.0/tests/test_run.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.7.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/conftest.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/test_main.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/test_of_types.py
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/test_set_env.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/test_sets.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/cli/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/cli/conftest.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/cli/test_cli_env_var.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/cli/test_cli_ini.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/cli/test_parse.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/cli/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/test_loader.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/test_memory_loader.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/test_section.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/test_str_convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/conftest.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/test_factor.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/test_ini_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/replace/__init__.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/replace/conftest.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/replace/test_replace.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/replace/test_replace_env_var.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/replace/test_replace_os_pathsep.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/replace/test_replace_os_sep.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/replace/test_replace_posargs.py
+-rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/replace/test_replace_tox_env.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/loader/ini/replace/test_replace_tty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/source/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/source/test_discover.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/source/test_legacy_toml.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/source/test_setup_cfg.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.7.0/tests/config/source/test_source_ini.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 tox-4.7.0/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.7.0/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.7.0/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.7.0/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.7.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/conftest.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/test_request.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/test_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/local_subprocess/__init__.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/local_subprocess/bad_process.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/local_subprocess/local_subprocess_sigint.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/local_subprocess/test_execute_util.py
+-rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/local_subprocess/test_local_subprocess.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.7.0/tests/execute/local_subprocess/tty_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/journal/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.7.0/tests/journal/test_main_journal.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.7.0/tests/plugin/conftest.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.7.0/tests/plugin/test_inline.py
+-rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 tox-4.7.0/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.7.0/tests/plugin/test_plugin_custom_config_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/pytest_/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.7.0/tests/pytest_/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/__init__.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/test_env_select.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/test_session_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_depends.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_devenv.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_exec_.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_legacy.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_list_envs.py
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_parallel.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_quickstart.py
+-rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_sequential.py
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_show_config.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.7.0/tests/session/cmd/run/test_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/test_api.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/test_info.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/test_register.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/test_tox_env_api.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/test_tox_env_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/test_python_api.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/test_python_runner.py
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/pip/test_pip_install.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/pip/test_req_file.py
+-rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/pip/req/test_file.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/test-pkg/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/virtual_env/test_setuptools.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/virtual_env/package/conftest.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
+-rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.7.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.7.0/tests/type_check/add_config_container_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.7.0/tests/util/__init__.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 tox-4.7.0/tests/util/test_ci.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.7.0/tests/util/test_cpu.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.7.0/tests/util/test_graph.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.7.0/tests/util/test_path.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.7.0/tests/util/test_spinner.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.7.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.7.0/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.7.0/README.md
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 tox-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tox-4.7.0/PKG-INFO
```

### Comparing `tox-4.6.4/tox.ini` & `tox-4.7.0/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     twine check {envtmpdir}{/}*
     check-wheel-contents --no-config {envtmpdir}
 
 [testenv:release]
 description = do a release, required posarg of the version number
 skip_install = true
 deps =
-    gitpython>=3.1.31
+    gitpython>=3.1.32
     packaging>=23.1
     towncrier>=23.6
 commands =
     python {toxinidir}/tasks/release.py --version {posargs}
 
 [testenv:dev]
 description = dev environment with all deps at {envdir}
```

### Comparing `tox-4.6.4/src/tox/provision.py` & `tox-4.7.0/src/tox/provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/pytest.py` & `tox-4.7.0/src/tox/pytest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/report.py` & `tox-4.7.0/src/tox/report.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/run.py` & `tox-4.7.0/src/tox/run.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/main.py` & `tox-4.7.0/src/tox/config/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             return self._key_to_conf_set[key]  # type: ignore[return-value] # expected T but found ConfigSet
         except KeyError:
             conf_set = of_type(self, section, for_env)
             self._key_to_conf_set[key] = conf_set
             if for_env is not None:
                 conf_set.loaders.extend(self.memory_seed_loaders.get(for_env, []))
             for loader in self._src.get_loaders(section, base, self._overrides, conf_set):
-                conf_set.loaders.append(loader)
+                conf_set.loaders.append(loader)  # noqa: PERF402
             if loaders is not None:
                 conf_set.loaders.extend(loaders)
             return conf_set
 
     def get_env(
         self,
         item: str,
```

### Comparing `tox-4.6.4/src/tox/config/of_type.py` & `tox-4.7.0/src/tox/config/of_type.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/set_env.py` & `tox-4.7.0/src/tox/config/set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/sets.py` & `tox-4.7.0/src/tox/config/sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/types.py` & `tox-4.7.0/src/tox/config/types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/cli/env_var.py` & `tox-4.7.0/src/tox/config/cli/env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/cli/ini.py` & `tox-4.7.0/src/tox/config/cli/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/cli/parse.py` & `tox-4.7.0/src/tox/config/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/cli/parser.py` & `tox-4.7.0/src/tox/config/cli/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         if of_type is None:
             if isinstance(action, argparse._AppendAction):  # noqa: SLF001
                 of_type = List[action.type]  # type: ignore[name-defined]
             elif isinstance(action, argparse._StoreAction) and action.choices:  # noqa: SLF001
                 loc = locals()
                 loc["Literal"] = Literal
                 as_literal = f"Literal[{', '.join(repr(i) for i in action.choices)}]"
-                of_type = eval(as_literal, globals(), loc)  # noqa: PGH001
+                of_type = eval(as_literal, globals(), loc)  # noqa: PGH001, S307
             elif action.default is not None:
                 of_type = type(action.default)
             elif isinstance(action, argparse._StoreConstAction) and action.const is not None:  # noqa: SLF001
                 of_type = type(action.const)
             else:
                 raise TypeError(action)
         return of_type
```

### Comparing `tox-4.6.4/src/tox/config/loader/api.py` & `tox-4.7.0/src/tox/config/loader/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/loader/convert.py` & `tox-4.7.0/src/tox/config/loader/convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/loader/memory.py` & `tox-4.7.0/src/tox/config/loader/memory.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/loader/section.py` & `tox-4.7.0/src/tox/config/loader/section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/loader/str_convert.py` & `tox-4.7.0/src/tox/config/loader/str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/loader/stringify.py` & `tox-4.7.0/src/tox/config/loader/stringify.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/loader/ini/__init__.py` & `tox-4.7.0/src/tox/config/loader/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/loader/ini/factor.py` & `tox-4.7.0/src/tox/config/loader/ini/factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/loader/ini/replace.py` & `tox-4.7.0/src/tox/config/loader/ini/replace.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         exception: Exception | None = None
         try:
             for src in _config_value_sources(settings["env"], settings["section"], conf_args.env_name, conf, loader):
                 try:
                     if isinstance(src, SectionProxy):
                         return loader.process_raw(conf, conf_args.env_name, src[key])
                     value = src.load(key, conf_args.chain)
-                except KeyError as exc:  # if fails, keep trying maybe another source can satisfy
+                except KeyError as exc:  # if fails, keep trying maybe another source can satisfy  # noqa: PERF203
                     exception = exc
                 else:
                     as_str, _ = stringify(value)
                     return as_str.replace("#", r"\#")  # escape comment characters as these will be stripped
         except Exception as exc:  # noqa: BLE001
             exception = exc
         if exception is not None:
```

### Comparing `tox-4.6.4/src/tox/config/source/api.py` & `tox-4.7.0/src/tox/config/source/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/source/discover.py` & `tox-4.7.0/src/tox/config/source/discover.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 def _load_exact_source(config_file: Path) -> Source:
     # if the filename matches to the letter some config file name do not fallback to other source types
     exact_match = next((s for s in SOURCE_TYPES if config_file.name == s.FILENAME), None)  # pragma: no cover
     for src_type in (exact_match,) if exact_match is not None else SOURCE_TYPES:  # pragma: no branch
         try:
             return src_type(config_file)
-        except ValueError:
+        except ValueError:  # noqa: PERF203
             pass
     msg = f"could not recognize config file {config_file}"
     raise HandledError(msg)
 
 
 def _create_default_source(root_dir: Path | None) -> Source:
     if root_dir is None:  # if set use that
```

### Comparing `tox-4.6.4/src/tox/config/source/ini.py` & `tox-4.7.0/src/tox/config/source/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/source/ini_section.py` & `tox-4.7.0/src/tox/config/source/ini_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/source/legacy_toml.py` & `tox-4.7.0/src/tox/config/source/legacy_toml.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/config/source/setup_cfg.py` & `tox-4.7.0/src/tox/config/source/setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/execute/api.py` & `tox-4.7.0/src/tox/execute/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/execute/pep517_backend.py` & `tox-4.7.0/src/tox/execute/pep517_backend.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/execute/request.py` & `tox-4.7.0/src/tox/execute/request.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/execute/stream.py` & `tox-4.7.0/src/tox/execute/stream.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/execute/util.py` & `tox-4.7.0/src/tox/execute/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/execute/local_sub_process/__init__.py` & `tox-4.7.0/src/tox/execute/local_sub_process/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 import _overlapped  # type: ignore[import]
 
                 ov = _overlapped.Overlapped(0)
                 ov.WriteFile(stdin.handle, bytes_content)  # type: ignore[attr-defined]
                 result = ov.getresult(10)  # wait up to 10ms to perform the operation
                 if result != len(bytes_content):
                     msg = f"failed to write to {stdin!r}"
-                    raise RuntimeError(msg)  # noqa: TRY301
+                    raise RuntimeError(msg)
             else:
                 stdin.write(bytes_content)
                 stdin.flush()
         except OSError:  # pragma: no cover
             if self._interrupted:  # pragma: no cover
                 pass  # pragma: no cover  # if the process was asked to exit in the meantime ignore write errors
             raise  # pragma: no cover
```

### Comparing `tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread.py` & `tox-4.7.0/src/tox/execute/local_sub_process/read_via_thread.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread_unix.py` & `tox-4.7.0/src/tox/execute/local_sub_process/read_via_thread_unix.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/execute/local_sub_process/read_via_thread_windows.py` & `tox-4.7.0/src/tox/execute/local_sub_process/read_via_thread_windows.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/journal/env.py` & `tox-4.7.0/src/tox/journal/env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/journal/main.py` & `tox-4.7.0/src/tox/journal/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/plugin/__init__.py` & `tox-4.7.0/src/tox/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/plugin/inline.py` & `tox-4.7.0/src/tox/plugin/inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/plugin/manager.py` & `tox-4.7.0/src/tox/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/plugin/spec.py` & `tox-4.7.0/src/tox/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/env_select.py` & `tox-4.7.0/src/tox/session/env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/state.py` & `tox-4.7.0/src/tox/session/state.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/cmd/depends.py` & `tox-4.7.0/src/tox/session/cmd/depends.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         print("   " * at, end="")  # noqa: T201
         print(env, end="")  # noqa: T201
         if env != "ALL":
             run_env = cast(RunToxEnv, state.envs[env])
             packager_list: list[str] = []
             try:
                 for pkg_env in run_env.package_envs:
-                    packager_list.append(pkg_env.name)
+                    packager_list.append(pkg_env.name)  # noqa: PERF401
             except Exception as exception:  # noqa: BLE001
                 packager_list.append(f"... ({exception})")
             names = " | ".join(packager_list)
             if names:
                 print(f" ~ {names}", end="")  # noqa: T201
         print("")  # noqa: T201
         at += 1
```

### Comparing `tox-4.6.4/src/tox/session/cmd/devenv.py` & `tox-4.7.0/src/tox/session/cmd/devenv.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     opt.install_pkg = None  # no explicit packages to install
     opt.skip_pkg_install = False  # always install a package in this case
     opt.no_test = True  # do not run the test phase
     loader = MemoryLoader(  # these configuration values are loaded from in-memory always (no file conf)
         usedevelop=True,  # dev environments must be of type dev
         env_dir=opt.devenv_path,  # move it in source
     )
-    state.conf.memory_seed_loaders[list(opt.env)[0]].append(loader)
+    state.conf.memory_seed_loaders[next(iter(opt.env))].append(loader)
 
     state.envs.ensure_only_run_env_is_active()
     envs = list(state.envs.iter())
     if len(envs) != 1:
         msg = f"exactly one target environment allowed in devenv mode but found {', '.join(envs)}"
         raise HandledError(msg)
     result = run_sequential(state)
```

### Comparing `tox-4.6.4/src/tox/session/cmd/exec_.py` & `tox-4.7.0/src/tox/session/cmd/exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/cmd/legacy.py` & `tox-4.7.0/src/tox/session/cmd/legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/cmd/list_env.py` & `tox-4.7.0/src/tox/session/cmd/list_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/cmd/quickstart.py` & `tox-4.7.0/src/tox/session/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/cmd/show_config.py` & `tox-4.7.0/src/tox/session/cmd/show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/cmd/version_flag.py` & `tox-4.7.0/src/tox/session/cmd/version_flag.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/cmd/run/common.py` & `tox-4.7.0/src/tox/session/cmd/run/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,22 +131,27 @@
                         if result <= 0:
                             msg = "must be greater than zero"
                             raise ValueError(msg)  # noqa: TRY301
                     except ValueError as exc:
                         raise ArgumentError(self, str(exc)) from exc
                 setattr(namespace, self.dest, result)
 
+        if os.environ.get("PYTHONHASHSEED", "random") != "random":
+            hashseed_default = int(os.environ["PYTHONHASHSEED"])
+        else:
+            hashseed_default = random.randint(1, 1024 if sys.platform == "win32" else 4294967295)  # noqa: S311
+
         parser.add_argument(
             "--hashseed",
             metavar="SEED",
             help="set PYTHONHASHSEED to SEED before running commands. Defaults to a random integer in the range "
             "[1, 4294967295] ([1, 1024] on Windows). Passing 'noset' suppresses this behavior.",
             action=SeedAction,
             of_type=Optional[int],
-            default=random.randint(1, 1024 if sys.platform == "win32" else 4294967295),  # noqa: S311
+            default=hashseed_default,
             dest="hash_seed",
         )
     parser.add_argument(
         "--discover",
         dest="discover",
         nargs="+",
         metavar="path",
@@ -259,18 +264,16 @@
             lock = getattr(thread, "_tstate_lock", None)
             if lock is not None and lock.locked():  # pragma: no branch
                 lock.release()  # pragma: no cover
                 # calling private method to fix thread state
                 thread._stop()  # type: ignore[attr-defined] # pragma: no cover # noqa: SLF001
             thread.join()
     finally:
-        ordered_results: list[ToxEnvRunResult] = []
         name_to_run = {r.name: r for r in results}
-        for env in to_run_list:
-            ordered_results.append(name_to_run[env])
+        ordered_results: list[ToxEnvRunResult] = [name_to_run[env] for env in to_run_list]
         # write the journal
         write_journal(getattr(state.conf.options, "result_json", None), state._journal)  # noqa: SLF001
         # report the outcome
         exit_code = report(
             state.conf.options.start,
             ordered_results,
             state.conf.options.is_colored,
```

### Comparing `tox-4.6.4/src/tox/session/cmd/run/parallel.py` & `tox-4.7.0/src/tox/session/cmd/run/parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/cmd/run/sequential.py` & `tox-4.7.0/src/tox/session/cmd/run/sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/session/cmd/run/single.py` & `tox-4.7.0/src/tox/session/cmd/run/single.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/api.py` & `tox-4.7.0/src/tox/tox_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/info.py` & `tox-4.7.0/src/tox/tox_env/info.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/installer.py` & `tox-4.7.0/src/tox/tox_env/installer.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/package.py` & `tox-4.7.0/src/tox/tox_env/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/register.py` & `tox-4.7.0/src/tox/tox_env/register.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/runner.py` & `tox-4.7.0/src/tox/tox_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/util.py` & `tox-4.7.0/src/tox/tox_env/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/api.py` & `tox-4.7.0/src/tox/tox_env/python/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/package.py` & `tox-4.7.0/src/tox/tox_env/python/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/runner.py` & `tox-4.7.0/src/tox/tox_env/python/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/pip/pip_install.py` & `tox-4.7.0/src/tox/tox_env/python/pip/pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/pip/req_file.py` & `tox-4.7.0/src/tox/tox_env/python/pip/req_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,16 @@
         return self._raw.splitlines()
 
     @staticmethod
     def _normalize_raw(raw: str) -> str:
         # a line ending in an unescaped \ is treated as a line continuation and the newline following it is effectively
         # ignored
         raw = "".join(raw.replace("\r", "").split("\\\n"))
-        lines: list[str] = []
-        for line in raw.splitlines():
-            # for tox<4 supporting requirement/constraint files via -rreq.txt/-creq.txt
-            lines.append(PythonDeps._normalize_line(line))
+        # for tox<4 supporting requirement/constraint files via -rreq.txt/-creq.txt
+        lines: list[str] = [PythonDeps._normalize_line(line) for line in raw.splitlines()]
         adjusted = "\n".join(lines)
         return f"{adjusted}\n" if raw.endswith("\\\n") else adjusted  # preserve trailing newline if input has it
 
     @staticmethod
     def _normalize_line(line: str) -> str:
         arg_match = next(
             (
```

### Comparing `tox-4.6.4/src/tox/tox_env/python/pip/req/args.py` & `tox-4.7.0/src/tox/tox_env/python/pip/req/args.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/pip/req/file.py` & `tox-4.7.0/src/tox/tox_env/python/pip/req/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
         if opt.require_hashes:
             base_opt.require_hashes = True
         if opt.features_enabled:
             if not hasattr(base_opt, "features_enabled"):
                 base_opt.features_enabled = []
             for feature in opt.features_enabled:
                 if feature not in base_opt.features_enabled:
-                    base_opt.features_enabled.append(feature)
+                    base_opt.features_enabled.append(feature)  # noqa: PERF401
             base_opt.features_enabled.sort()
         if opt.index_url:
             if getattr(base_opt, "index_url", []):
                 base_opt.index_url[0] = opt.index_url
             else:
                 base_opt.index_url = [opt.index_url]
         if opt.no_index is True:
```

### Comparing `tox-4.6.4/src/tox/tox_env/python/pip/req/util.py` & `tox-4.7.0/src/tox/tox_env/python/pip/req/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/virtual_env/api.py` & `tox-4.7.0/src/tox/tox_env/python/virtual_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/virtual_env/runner.py` & `tox-4.7.0/src/tox/tox_env/python/virtual_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/virtual_env/package/cmd_builder.py` & `tox-4.7.0/src/tox/tox_env/python/virtual_env/package/cmd_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             chdir: Path = self.conf["change_dir"]
             ignore_errors: bool = self.conf["ignore_errors"]
             status = run_command_set(self, "commands", chdir, ignore_errors, [])
             if status != Outcome.OK:
                 msg = "stopping as failed to build package"
                 raise Fail(msg)
             package_glob = self.conf["package_glob"]
-            found = glob.glob(package_glob)
+            found = glob.glob(package_glob)  # noqa: PTH207
             if not found:
                 msg = f"no package found in {package_glob}"
                 raise Fail(msg)
             if len(found) != 1:
                 msg = f"found more than one package {', '.join(sorted(found))}"
                 raise Fail(msg)
             path = Path(found[0])
```

### Comparing `tox-4.6.4/src/tox/tox_env/python/virtual_env/package/pyproject.py` & `tox-4.7.0/src/tox/tox_env/python/virtual_env/package/pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/tox_env/python/virtual_env/package/util.py` & `tox-4.7.0/src/tox/tox_env/python/virtual_env/package/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/util/ci.py` & `tox-4.7.0/src/tox/util/ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/util/file_view.py` & `tox-4.7.0/src/tox/util/file_view.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/util/graph.py` & `tox-4.7.0/src/tox/util/graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/util/path.py` & `tox-4.7.0/src/tox/util/path.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/src/tox/util/spinner.py` & `tox-4.7.0/src/tox/util/spinner.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     class _CursorInfo(ctypes.Structure):
         _fields_: ClassVar[list[tuple[str, Any]]] = [("size", ctypes.c_int), ("visible", ctypes.c_byte)]
 
 
 def _file_support_encoding(chars: Sequence[str], file: IO[str]) -> bool:
     encoding = getattr(file, "encoding", None)
     if encoding is not None:  # pragma: no branch  # this should be always set, unless someone passes in something bad
-        for char in chars:
-            try:
+        try:
+            for char in chars:
                 char.encode(encoding)
-            except UnicodeEncodeError:
-                break
+        except UnicodeEncodeError:
+            pass
         else:
             return True
     return False
 
 
 T = TypeVar("T", bound="Spinner")
 MISS_DURATION = 0.01
```

### Comparing `tox-4.6.4/tests/conftest.py` & `tox-4.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/test_provision.py` & `tox-4.7.0/tests/test_provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/test_report.py` & `tox-4.7.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/test_run.py` & `tox-4.7.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/test_version.py` & `tox-4.7.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/test_main.py` & `tox-4.7.0/tests/config/test_main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/test_of_types.py` & `tox-4.7.0/tests/config/test_of_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/test_set_env.py` & `tox-4.7.0/tests/config/test_set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/test_sets.py` & `tox-4.7.0/tests/config/test_sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/test_types.py` & `tox-4.7.0/tests/config/test_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/cli/conftest.py` & `tox-4.7.0/tests/config/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/cli/test_cli_env_var.py` & `tox-4.7.0/tests/config/cli/test_cli_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/cli/test_cli_ini.py` & `tox-4.7.0/tests/config/cli/test_cli_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/cli/test_parse.py` & `tox-4.7.0/tests/config/cli/test_parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/cli/test_parser.py` & `tox-4.7.0/tests/config/cli/test_parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/test_loader.py` & `tox-4.7.0/tests/config/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/test_memory_loader.py` & `tox-4.7.0/tests/config/loader/test_memory_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     ("value", "of_type", "exception", "msg"),
     [
         ("m", int, ValueError, "invalid literal for int"),
         ({"m"}, Set[int], ValueError, "invalid literal for int"),
         (["m"], List[int], ValueError, "invalid literal for int"),
         ({"m": 1}, Dict[int, int], ValueError, "invalid literal for int"),
         ({1: "m"}, Dict[int, int], ValueError, "invalid literal for int"),
-        (object, Path, TypeError, "expected str, bytes or os.PathLike object"),
+        (object, Path, TypeError, r"str(, bytes)? or (an )?os\.PathLike object"),
         (1, Command, TypeError, "1"),
         (1, EnvList, TypeError, "1"),
     ],
 )
 def test_memory_loader_fails_invalid(value: Any, of_type: type[Any], exception: Exception, msg: str) -> None:
     loader = MemoryLoader(a=value, kwargs={})
     args = ConfigLoadArgs([], "name", None)
```

### Comparing `tox-4.6.4/tests/config/loader/test_section.py` & `tox-4.7.0/tests/config/loader/test_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/test_str_convert.py` & `tox-4.7.0/tests/config/loader/test_str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/ini/conftest.py` & `tox-4.7.0/tests/config/loader/ini/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/ini/test_factor.py` & `tox-4.7.0/tests/config/loader/ini/test_factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/ini/test_ini_loader.py` & `tox-4.7.0/tests/config/loader/ini/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/ini/replace/conftest.py` & `tox-4.7.0/tests/config/loader/ini/replace/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/ini/replace/test_replace.py` & `tox-4.7.0/tests/config/loader/ini/replace/test_replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/ini/replace/test_replace_env_var.py` & `tox-4.7.0/tests/config/loader/ini/replace/test_replace_env_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     result = replace_one(r"{env:MAGIC}\\\{env:MAGIC}")
     assert result == r"something good\\{env:MAGIC}"
 
 
 def test_replace_env_set_quad_bs(replace_one: ReplaceOne, monkeypatch: MonkeyPatch) -> None:
     """Quad backslash should remain but not affect surrounding replacements."""
     monkeypatch.setenv("MAGIC", "something good")
-    result = replace_one(r"\\{env:MAGIC}\\\\{env:MAGIC}" + "\\")  # noqa: ISC003
-    assert result == r"\\something good\\\\something good" + "\\"  # noqa: ISC003
+    result = replace_one(r"\\{env:MAGIC}\\\\{env:MAGIC}" + "\\")
+    assert result == r"\\something good\\\\something good" + "\\"
 
 
 def test_replace_env_when_value_is_backslash(replace_one: ReplaceOne, monkeypatch: MonkeyPatch) -> None:
     """When the replacement value is backslash, it shouldn't affect the next replacement."""
     monkeypatch.setenv("MAGIC", "tragic")
     monkeypatch.setenv("BS", "\\")
     result = replace_one(r"{env:BS}{env:MAGIC}")
```

### Comparing `tox-4.6.4/tests/config/loader/ini/replace/test_replace_os_sep.py` & `tox-4.7.0/tests/config/loader/ini/replace/test_replace_os_sep.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/ini/replace/test_replace_posargs.py` & `tox-4.7.0/tests/config/loader/ini/replace/test_replace_posargs.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/ini/replace/test_replace_tox_env.py` & `tox-4.7.0/tests/config/loader/ini/replace/test_replace_tox_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/loader/ini/replace/test_replace_tty.py` & `tox-4.7.0/tests/config/loader/ini/replace/test_replace_tty.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/source/test_discover.py` & `tox-4.7.0/tests/config/source/test_discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/source/test_setup_cfg.py` & `tox-4.7.0/tests/config/source/test_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/config/source/test_source_ini.py` & `tox-4.7.0/tests/config/source/test_source_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/demo_pkg_inline/build.py` & `tox-4.7.0/tests/demo_pkg_inline/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,19 +38,17 @@
                     return "example"
             @impl
             def tox_register_tox_env(register: ToxEnvRegister) -> None:
                 register.add_run_env(ExampleVirtualEnvRunner)
         """,
 }
 metadata_files = {
-    entry_points: """
+    entry_points: f"""
         [tox]
-        example = {}.example_plugin""".format(
-        name,
-    ),
+        example = {name}.example_plugin""",
     metadata: """
         Metadata-Version: 2.1
         Name: {}
         Version: {}
         Summary: UNKNOWN
         Home-page: UNKNOWN
         Author: UNKNOWN
@@ -61,24 +59,20 @@
 
         UNKNOWN
        """.format(
         pkg_name,
         version,
         "\n        ".join(os.environ.get("METADATA_EXTRA", "").split("\n")),
     ),
-    wheel: """
+    wheel: f"""
         Wheel-Version: 1.0
-        Generator: {}-{}
+        Generator: {name}-{version}
         Root-Is-Purelib: true
-        Tag: py{}-none-any
-       """.format(
-        name,
-        version,
-        sys.version_info[0],
-    ),
+        Tag: py{sys.version_info[0]}-none-any
+       """,
     f"{dist_info}/top_level.txt": name,
     record: """
         {0}/__init__.py,,
         {1}/METADATA,,
         {1}/WHEEL,,
         {1}/top_level.txt,,
         {1}/RECORD,,
```

### Comparing `tox-4.6.4/tests/execute/test_request.py` & `tox-4.7.0/tests/execute/test_request.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/execute/local_subprocess/bad_process.py` & `tox-4.7.0/tests/execute/local_subprocess/bad_process.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/execute/local_subprocess/local_subprocess_sigint.py` & `tox-4.7.0/tests/execute/local_subprocess/local_subprocess_sigint.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/execute/local_subprocess/test_execute_util.py` & `tox-4.7.0/tests/execute/local_subprocess/test_execute_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/execute/local_subprocess/test_local_subprocess.py` & `tox-4.7.0/tests/execute/local_subprocess/test_local_subprocess.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/journal/test_main_journal.py` & `tox-4.7.0/tests/journal/test_main_journal.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/plugin/test_inline.py` & `tox-4.7.0/tests/plugin/test_inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/plugin/test_plugin.py` & `tox-4.7.0/tests/plugin/test_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,16 +236,16 @@
     def _cannot_extend_config(config_set: ConfigSet) -> None:
         for _conf in (
             lambda c: c.add_constant("c", "desc", "v"),
             lambda c: c.add_config("c", of_type=str, default="c", desc="d"),
         ):
             try:
                 _conf(config_set)  # type: ignore[no-untyped-call] # call to not typed function
-                raise NotImplementedError  # noqa: TRY301
-            except RuntimeError as exc:
+                raise NotImplementedError
+            except RuntimeError as exc:  # noqa: PERF203
                 assert str(exc) == "config set has been marked final and cannot be extended"  # noqa: PT017
 
     @impl
     def tox_before_run_commands(tox_env: ToxEnv) -> None:
         _cannot_extend_config(tox_env.conf)
         _cannot_extend_config(tox_env.core)
```

### Comparing `tox-4.6.4/tests/plugin/test_plugin_custom_config_set.py` & `tox-4.7.0/tests/plugin/test_plugin_custom_config_set.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/pytest_/test_init.py` & `tox-4.7.0/tests/pytest_/test_init.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/test_env_select.py` & `tox-4.7.0/tests/session/test_env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/test_session_common.py` & `tox-4.7.0/tests/session/test_session_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_depends.py` & `tox-4.7.0/tests/session/cmd/test_depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_devenv.py` & `tox-4.7.0/tests/session/cmd/test_devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_exec_.py` & `tox-4.7.0/tests/session/cmd/test_exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_legacy.py` & `tox-4.7.0/tests/session/cmd/test_legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_list_envs.py` & `tox-4.7.0/tests/session/cmd/test_list_envs.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_parallel.py` & `tox-4.7.0/tests/session/cmd/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_quickstart.py` & `tox-4.7.0/tests/session/cmd/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_sequential.py` & `tox-4.7.0/tests/session/cmd/test_sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_show_config.py` & `tox-4.7.0/tests/session/cmd/test_show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/test_state.py` & `tox-4.7.0/tests/session/cmd/test_state.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/session/cmd/run/test_common.py` & `tox-4.7.0/tests/session/cmd/run/test_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/test_api.py` & `tox-4.7.0/tests/tox_env/test_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/test_register.py` & `tox-4.7.0/tests/tox_env/test_register.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/test_tox_env_api.py` & `tox-4.7.0/tests/tox_env/test_tox_env_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/test_tox_env_runner.py` & `tox-4.7.0/tests/tox_env/test_tox_env_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/test_python_api.py` & `tox-4.7.0/tests/tox_env/python/test_python_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import sys
 from typing import TYPE_CHECKING, Callable
+from unittest.mock import patch
 
 import pytest
 
 from tox.tox_env.errors import Fail
 from tox.tox_env.python.api import Python
 
 if TYPE_CHECKING:
@@ -216,14 +217,46 @@
 
 def test_python_set_hash_seed_incorrect(tox_project: ToxProjectCreator) -> None:
     result = tox_project({"tox.ini": ""}).run("r", "-e", "py", "--hashseed", "ok")
     result.assert_failed(2)
     assert "tox run: error: argument --hashseed: invalid literal for int() with base 10: 'ok'" in result.err
 
 
+def test_python_use_hash_seed_from_env(tox_project: ToxProjectCreator) -> None:
+    ini = "[testenv]\npackage=skip"
+    with patch.dict("os.environ", {"PYTHONHASHSEED": "13"}):
+        result = tox_project({"tox.ini": ini}).run("c", "-e", "py", "-k", "setenv")
+        result.assert_success()
+        assert "PYTHONHASHSEED=13" in result.out
+
+
+def test_python_hash_seed_from_env_random(tox_project: ToxProjectCreator) -> None:
+    ini = "[testenv]\npackage=skip"
+    with patch.dict("os.environ", {"PYTHONHASHSEED": "random"}):
+        result = tox_project({"tox.ini": ini}).run("c", "-e", "py", "-k", "setenv")
+        result.assert_success()
+        assert "PYTHONHASHSEED=" in result.out
+
+
+def test_python_hash_seed_from_env_and_override(tox_project: ToxProjectCreator) -> None:
+    ini = "[testenv]\npackage=skip\ncommands=python -c 'import os; print(os.environ.get(\"PYTHONHASHSEED\"))'"
+    with patch.dict("os.environ", {"PYTHONHASHSEED": "14"}):
+        result = tox_project({"tox.ini": ini}).run("r", "-e", "py", "--hashseed", "15")
+        result.assert_success()
+        assert result.out.splitlines()[1] == "15"
+
+
+def test_python_hash_seed_from_env_and_disable(tox_project: ToxProjectCreator) -> None:
+    ini = "[testenv]\npackage=skip\ncommands=python -c 'import os; print(os.environ.get(\"PYTHONHASHSEED\"))'"
+    with patch.dict("os.environ", {"PYTHONHASHSEED": "16"}):
+        result = tox_project({"tox.ini": ini}).run("r", "-e", "py", "--hashseed", "notset")
+        result.assert_success()
+        assert result.out.splitlines()[1] == "None"
+
+
 @pytest.mark.parametrize("in_ci", [True, False])
 def test_list_installed_deps(in_ci: bool, tox_project: ToxProjectCreator, mocker: MockerFixture) -> None:
     mocker.patch("tox.session.cmd.run.common.is_ci", return_value=in_ci)
     result = tox_project({"tox.ini": "[testenv]\nskip_install = true"}).run("r", "-e", "py")
     if in_ci:
         assert "pip==" in result.out
     else:
```

### Comparing `tox-4.6.4/tests/tox_env/python/test_python_runner.py` & `tox-4.7.0/tests/tox_env/python/test_python_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/pip/test_pip_install.py` & `tox-4.7.0/tests/tox_env/python/pip/test_pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/pip/test_req_file.py` & `tox-4.7.0/tests/tox_env/python/pip/test_req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/pip/req/test_file.py` & `tox-4.7.0/tests/tox_env/python/pip/req/test_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/virtual_env/test_setuptools.py` & `tox-4.7.0/tests/tox_env/python/virtual_env/test_setuptools.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/virtual_env/test_virtualenv_api.py` & `tox-4.7.0/tests/tox_env/python/virtual_env/test_virtualenv_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/virtual_env/package/conftest.py` & `tox-4.7.0/tests/tox_env/python/virtual_env/package/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py` & `tox-4.7.0/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/virtual_env/package/test_package_pyproject.py` & `tox-4.7.0/tests/tox_env/python/virtual_env/package/test_package_pyproject.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/tox_env/python/virtual_env/package/test_python_package_util.py` & `tox-4.7.0/tests/tox_env/python/virtual_env/package/test_python_package_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/util/test_ci.py` & `tox-4.7.0/tests/util/test_ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/util/test_cpu.py` & `tox-4.7.0/tests/util/test_cpu.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/util/test_graph.py` & `tox-4.7.0/tests/util/test_graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/tests/util/test_spinner.py` & `tox-4.7.0/tests/util/test_spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/LICENSE` & `tox-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/README.md` & `tox-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tox-4.6.4/pyproject.toml` & `tox-4.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -50,20 +50,20 @@
 dependencies = [
   "cachetools>=5.3.1",
   "chardet>=5.1",
   "colorama>=0.4.6",
   "filelock>=3.12.2",
   'importlib-metadata>=6.7; python_version < "3.8"',
   "packaging>=23.1",
-  "platformdirs>=3.8",
+  "platformdirs>=3.9.1",
   "pluggy>=1.2",
-  "pyproject-api>=1.5.2",
+  "pyproject-api>=1.5.3",
   'tomli>=2.0.1; python_version < "3.11"',
-  'typing-extensions>=4.6.3; python_version < "3.8"',
-  "virtualenv>=20.23.1",
+  'typing-extensions>=4.7.1; python_version < "3.8"',
+  "virtualenv>=20.24.1",
 ]
 optional-dependencies.docs = [
   "furo>=2023.5.20",
   "sphinx>=7.0.1",
   "sphinx-argparse-cli>=1.11.1",
   "sphinx-autodoc-typehints!=1.23.4,>=1.23.3",
   "sphinx-copybutton>=0.5.2",
@@ -72,16 +72,16 @@
   "towncrier>=23.6",
 ]
 optional-dependencies.testing = [
   "build[virtualenv]>=0.10",
   "covdefaults>=2.3",
   "detect-test-pollution>=1.1.1",
   "devpi-process>=0.3.1",
-  "diff-cover>=7.6",
-  "distlib>=0.3.6",
+  "diff-cover>=7.7",
+  "distlib>=0.3.7",
   "flaky>=3.7",
   "hatch-vcs>=0.3",
   "hatchling>=1.17.1",
   "psutil>=5.9.5",
   "pytest>=7.4",
   "pytest-cov>=4.1",
   "pytest-mock>=3.11.1",
```

### Comparing `tox-4.6.4/PKG-INFO` & `tox-4.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox
-Version: 4.6.4
+Version: 4.7.0
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, http://tox.readthedocs.org
 Project-URL: Release Notes, https://tox.wiki/en/latest/changelog.html
 Project-URL: Source, https://github.com/tox-dev/tox
 Project-URL: Tracker, https://github.com/tox-dev/tox/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -32,36 +32,36 @@
 Requires-Python: >=3.7
 Requires-Dist: cachetools>=5.3.1
 Requires-Dist: chardet>=5.1
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: filelock>=3.12.2
 Requires-Dist: importlib-metadata>=6.7; python_version < '3.8'
 Requires-Dist: packaging>=23.1
-Requires-Dist: platformdirs>=3.8
+Requires-Dist: platformdirs>=3.9.1
 Requires-Dist: pluggy>=1.2
-Requires-Dist: pyproject-api>=1.5.2
+Requires-Dist: pyproject-api>=1.5.3
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
-Requires-Dist: typing-extensions>=4.6.3; python_version < '3.8'
-Requires-Dist: virtualenv>=20.23.1
+Requires-Dist: typing-extensions>=4.7.1; python_version < '3.8'
+Requires-Dist: virtualenv>=20.24.1
 Provides-Extra: docs
 Requires-Dist: furo>=2023.5.20; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.11.1; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints!=1.23.4,>=1.23.3; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs>=2023.4.21; extra == 'docs'
 Requires-Dist: sphinx>=7.0.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-towncrier>=0.2.1a0; extra == 'docs'
 Requires-Dist: towncrier>=23.6; extra == 'docs'
 Provides-Extra: testing
 Requires-Dist: build[virtualenv]>=0.10; extra == 'testing'
 Requires-Dist: covdefaults>=2.3; extra == 'testing'
 Requires-Dist: detect-test-pollution>=1.1.1; extra == 'testing'
 Requires-Dist: devpi-process>=0.3.1; extra == 'testing'
-Requires-Dist: diff-cover>=7.6; extra == 'testing'
-Requires-Dist: distlib>=0.3.6; extra == 'testing'
+Requires-Dist: diff-cover>=7.7; extra == 'testing'
+Requires-Dist: distlib>=0.3.7; extra == 'testing'
 Requires-Dist: flaky>=3.7; extra == 'testing'
 Requires-Dist: hatch-vcs>=0.3; extra == 'testing'
 Requires-Dist: hatchling>=1.17.1; extra == 'testing'
 Requires-Dist: psutil>=5.9.5; extra == 'testing'
 Requires-Dist: pytest-cov>=4.1; extra == 'testing'
 Requires-Dist: pytest-mock>=3.11.1; extra == 'testing'
 Requires-Dist: pytest-xdist>=3.3.1; extra == 'testing'
```

