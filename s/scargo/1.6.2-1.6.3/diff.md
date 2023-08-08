# Comparing `tmp/scargo-1.6.2.tar.gz` & `tmp/scargo-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scargo-1.6.2.tar", last modified: Mon Jul 31 11:57:05 2023, max compression
+gzip compressed data, was "scargo-1.6.3.tar", last modified: Tue Aug  8 05:20:00 2023, max compression
```

## Comparing `scargo-1.6.2.tar` & `scargo-1.6.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     4508 2023-07-31 11:56:59.364710 scargo-1.6.2/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-07-31 11:56:59.364710 scargo-1.6.2/LICENSE
--rw-r--r--   0        0        0     2494 2023-07-31 11:56:59.364710 scargo-1.6.2/README.md
--rw-r--r--   0        0        0     2748 2023-07-31 11:56:59.380711 scargo-1.6.2/pyproject.toml
--rw-r--r--   0        0        0      108 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/__init__.py
--rwxr-xr-x   0        0        0    19734 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/certs/certGen.sh
--rwxr-xr-x   0        0        0     4629 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/certs/generateAllCertificates.sh
--rw-r--r--   0        0        0     3967 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/certs/openssl_device_intermediate_ca.cnf
--rw-r--r--   0        0        0     3957 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/certs/openssl_root_ca.cnf
--rw-r--r--   0        0        0      698 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/clang_utils.py
--rw-r--r--   0        0        0    12896 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/cli.py
--rw-r--r--   0        0        0       86 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/__init__.py
--rw-r--r--   0        0        0     1854 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/build.py
--rw-r--r--   0        0        0    12319 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/check.py
--rw-r--r--   0        0        0     1142 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/clean.py
--rw-r--r--   0        0        0     4168 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/debug.py
--rw-r--r--   0        0        0     3402 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/doc.py
--rw-r--r--   0        0        0     3872 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/docker.py
--rw-r--r--   0        0        0     1124 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/fix.py
--rw-r--r--   0        0        0     3835 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/flash.py
--rw-r--r--   0        0        0     6677 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/gen.py
--rw-r--r--   0        0        0     2996 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/new.py
--rw-r--r--   0        0        0     3649 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/publish.py
--rw-r--r--   0        0        0     1688 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/run.py
--rw-r--r--   0        0        0     3651 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/test.py
--rw-r--r--   0        0        0     4553 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/update.py
--rw-r--r--   0        0        0      228 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/commands/version.py
--rw-r--r--   0        0        0     7288 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/config.py
--rw-r--r--   0        0        0     2255 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/config_utils.py
--rw-r--r--   0        0        0     2290 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/docker_utils.py
--rw-r--r--   0        0        0       86 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/__init__.py
--rw-r--r--   0        0        0     1658 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/base_gen.py
--rw-r--r--   0        0        0      441 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/cicd_gen.py
--rw-r--r--   0        0        0       86 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/clang_parser/__init__.py
--rw-r--r--   0        0        0     2251 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/clang_parser/data_classes.py
--rw-r--r--   0        0        0     1197 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/clang_parser/header_parser.py
--rw-r--r--   0        0        0     2385 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/clang_parser/params_extractor.py
--rw-r--r--   0        0        0      395 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/cmake_gen.py
--rw-r--r--   0        0        0     2049 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/conan_gen.py
--rw-r--r--   0        0        0     2602 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/cpp_gen.py
--rw-r--r--   0        0        0     3186 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/docker_gen.py
--rw-r--r--   0        0        0     1115 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/env_gen.py
--rwxr-xr-x   0        0        0     1607 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/mock_gen.py
--rw-r--r--   0        0        0      454 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/readme_gen.py
--rw-r--r--   0        0        0     4834 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/templates/.gitlab-ci.yml.j2
--rw-r--r--   0        0        0     1221 2023-07-31 11:56:59.380711 scargo-1.6.2/scargo/file_generators/templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0     4275 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/README.md.j2
--rw-r--r--   0        0        0     2232 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/conanfile.py.j2
--rw-r--r--   0        0        0     1539 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/conanfiletest.j2
--rw-r--r--   0        0        0      287 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/profile.j2
--rw-r--r--   0        0        0     1079 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/profile_esp32.j2
--rw-r--r--   0        0        0     1545 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/profile_stm32.j2
--rw-r--r--   0        0        0     1244 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/profile_x86.j2
--rw-r--r--   0        0        0      280 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/stm32_gcc_toolchain_wrapper.cmake.j2
--rw-r--r--   0        0        0      342 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/test_package/CMakeLists.txt.j2
--rw-r--r--   0        0        0      749 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/test_package/conanfile.py.j2
--rw-r--r--   0        0        0       59 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/conan/test_package/example.cpp.j2
--rw-r--r--   0        0        0      150 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
--rw-r--r--   0        0        0     3031 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
--rw-r--r--   0        0        0      879 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/cmake-src-x86.j2
--rw-r--r--   0        0        0      181 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/lib.cpp.j2
--rw-r--r--   0        0        0      213 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/lib.h.j2
--rw-r--r--   0        0        0      715 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/cpp/main.cpp.j2
--rw-r--r--   0        0        0      124 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-custom.j2
--rw-r--r--   0        0        0     2126 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
--rw-r--r--   0        0        0      754 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
--rw-r--r--   0        0        0       49 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-x86.j2
--rw-r--r--   0        0        0     2376 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile.j2
--rw-r--r--   0        0        0      684 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/devcontainer.json.j2
--rw-r--r--   0        0        0     1105 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/docker-compose.yaml.j2
--rw-r--r--   0        0        0      287 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/env.txt.j2
--rw-r--r--   0        0        0       22 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/docker/stm32.cfg.j2
--rw-r--r--   0        0        0      697 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/esp32.cmake.j2
--rw-r--r--   0        0        0       39 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/.clang-format
--rw-r--r--   0        0        0      475 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/CMakeLists.txt
--rw-r--r--   0        0        0      594 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/class_interface.h.j2
--rw-r--r--   0        0        0      835 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/class_mock.cpp.j2
--rw-r--r--   0        0        0      697 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/mock/class_mock.h.j2
--rw-r--r--   0        0        0      371 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/project.cmake.j2
--rw-r--r--   0        0        0     2228 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/scargo.toml.j2
--rw-r--r--   0        0        0      227 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/stm32.cmake.j2
--rw-r--r--   0        0        0       91 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
--rw-r--r--   0        0        0      100 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
--rw-r--r--   0        0        0     1079 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
--rw-r--r--   0        0        0       84 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
--rw-r--r--   0        0        0      326 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
--rw-r--r--   0        0        0     1046 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/tests/static_mock/static_mock.h
--rw-r--r--   0        0        0       39 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/ut/.clang-format
--rw-r--r--   0        0        0      575 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/ut/CMakeLists.txt.j2
--rw-r--r--   0        0        0      716 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/ut/ut.cpp.j2
--rw-r--r--   0        0        0       33 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/templates/x86.cmake.j2
--rw-r--r--   0        0        0     1597 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/tests_gen.py
--rw-r--r--   0        0        0      550 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/toml_gen.py
--rw-r--r--   0        0        0     5357 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/file_generators/ut_gen.py
--rw-r--r--   0        0        0      629 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/global_values.py
--rw-r--r--   0        0        0     2044 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/logger.py
--rw-r--r--   0        0        0     1137 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/path_utils.py
--rw-r--r--   0        0        0     2953 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/templates/.clang-format
--rw-r--r--   0        0        0     8780 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/templates/.clang-tidy
--rw-r--r--   0        0        0     2361 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/templates/.gitignore
--rw-r--r--   0        0        0     1066 2023-07-31 11:56:59.384711 scargo-1.6.2/scargo/templates/LICENSE
--rw-r--r--   0        0        0      519 2023-07-31 11:56:59.384711 scargo-1.6.2/setup.cfg
--rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 scargo-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     4508 2023-08-08 05:19:54.253430 scargo-1.6.3/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-08-08 05:19:54.253430 scargo-1.6.3/LICENSE
+-rw-r--r--   0        0        0     2494 2023-08-08 05:19:54.253430 scargo-1.6.3/README.md
+-rw-r--r--   0        0        0     2748 2023-08-08 05:19:54.265430 scargo-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/__init__.py
+-rwxr-xr-x   0        0        0    19734 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/certs/certGen.sh
+-rwxr-xr-x   0        0        0     4632 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/certs/generateAllCertificates.sh
+-rw-r--r--   0        0        0     3967 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/certs/openssl_device_intermediate_ca.cnf
+-rw-r--r--   0        0        0     3957 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/certs/openssl_root_ca.cnf
+-rw-r--r--   0        0        0      698 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/clang_utils.py
+-rw-r--r--   0        0        0    12896 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/cli.py
+-rw-r--r--   0        0        0       86 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/commands/__init__.py
+-rw-r--r--   0        0        0     2366 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/commands/build.py
+-rw-r--r--   0        0        0    12319 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/commands/check.py
+-rw-r--r--   0        0        0     1142 2023-08-08 05:19:54.265430 scargo-1.6.3/scargo/commands/clean.py
+-rw-r--r--   0        0        0     4168 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/debug.py
+-rw-r--r--   0        0        0     3402 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/doc.py
+-rw-r--r--   0        0        0     3872 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/docker.py
+-rw-r--r--   0        0        0     1124 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/fix.py
+-rw-r--r--   0        0        0     3835 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/flash.py
+-rw-r--r--   0        0        0     6677 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/gen.py
+-rw-r--r--   0        0        0     2996 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/new.py
+-rw-r--r--   0        0        0     3649 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/publish.py
+-rw-r--r--   0        0        0     1688 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/run.py
+-rw-r--r--   0        0        0     3651 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/test.py
+-rw-r--r--   0        0        0     4553 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/update.py
+-rw-r--r--   0        0        0      228 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/commands/version.py
+-rw-r--r--   0        0        0     7933 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/config.py
+-rw-r--r--   0        0        0     2255 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/config_utils.py
+-rw-r--r--   0        0        0     2290 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/docker_utils.py
+-rw-r--r--   0        0        0       86 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/__init__.py
+-rw-r--r--   0        0        0     1658 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/base_gen.py
+-rw-r--r--   0        0        0      441 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/cicd_gen.py
+-rw-r--r--   0        0        0       86 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/clang_parser/__init__.py
+-rw-r--r--   0        0        0     2251 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/clang_parser/data_classes.py
+-rw-r--r--   0        0        0     1197 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/clang_parser/header_parser.py
+-rw-r--r--   0        0        0     2385 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/clang_parser/params_extractor.py
+-rw-r--r--   0        0        0      395 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/cmake_gen.py
+-rw-r--r--   0        0        0     1880 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/conan_gen.py
+-rw-r--r--   0        0        0     2643 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/cpp_gen.py
+-rw-r--r--   0        0        0     3186 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/docker_gen.py
+-rw-r--r--   0        0        0     1115 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/env_gen.py
+-rwxr-xr-x   0        0        0     1607 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/mock_gen.py
+-rw-r--r--   0        0        0      454 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/readme_gen.py
+-rw-r--r--   0        0        0     4994 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/.gitlab-ci.yml.j2
+-rw-r--r--   0        0        0     1221 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/CMakeLists.txt.j2
+-rw-r--r--   0        0        0     4275 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/README.md.j2
+-rw-r--r--   0        0        0     2194 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/conanfile.py.j2
+-rw-r--r--   0        0        0     1539 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/conanfiletest.j2
+-rw-r--r--   0        0        0      287 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/profile.j2
+-rw-r--r--   0        0        0      750 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/profile_esp32.j2
+-rw-r--r--   0        0        0     1225 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/profile_stm32.j2
+-rw-r--r--   0        0        0      922 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/profile_x86.j2
+-rw-r--r--   0        0        0      280 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/stm32_gcc_toolchain_wrapper.cmake.j2
+-rw-r--r--   0        0        0      342 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/test_package/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      749 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/test_package/conanfile.py.j2
+-rw-r--r--   0        0        0       59 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/conan/test_package/example.cpp.j2
+-rw-r--r--   0        0        0      150 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
+-rw-r--r--   0        0        0     2945 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
+-rw-r--r--   0        0        0      837 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/cpp/cmake-src-x86.j2
+-rw-r--r--   0        0        0      181 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/cpp/lib.cpp.j2
+-rw-r--r--   0        0        0      213 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/cpp/lib.h.j2
+-rw-r--r--   0        0        0      715 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/cpp/main.cpp.j2
+-rw-r--r--   0        0        0      124 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/docker/Dockerfile-custom.j2
+-rw-r--r--   0        0        0     2126 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
+-rw-r--r--   0        0        0      754 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
+-rw-r--r--   0        0        0       49 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/docker/Dockerfile-x86.j2
+-rw-r--r--   0        0        0     2381 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/docker/Dockerfile.j2
+-rw-r--r--   0        0        0      684 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/docker/devcontainer.json.j2
+-rw-r--r--   0        0        0     1105 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/docker/docker-compose.yaml.j2
+-rw-r--r--   0        0        0      287 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/docker/env.txt.j2
+-rw-r--r--   0        0        0       22 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/docker/stm32.cfg.j2
+-rw-r--r--   0        0        0      697 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/esp32.cmake.j2
+-rw-r--r--   0        0        0       39 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/mock/.clang-format
+-rw-r--r--   0        0        0      475 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/mock/CMakeLists.txt
+-rw-r--r--   0        0        0      594 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/mock/class_interface.h.j2
+-rw-r--r--   0        0        0      835 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/mock/class_mock.cpp.j2
+-rw-r--r--   0        0        0      697 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/mock/class_mock.h.j2
+-rw-r--r--   0        0        0      371 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/project.cmake.j2
+-rw-r--r--   0        0        0     2802 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/scargo.toml.j2
+-rw-r--r--   0        0        0      227 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/stm32.cmake.j2
+-rw-r--r--   0        0        0       91 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
+-rw-r--r--   0        0        0      100 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
+-rw-r--r--   0        0        0     1079 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
+-rw-r--r--   0        0        0       84 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
+-rw-r--r--   0        0        0      326 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1046 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/tests/static_mock/static_mock.h
+-rw-r--r--   0        0        0       39 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/ut/.clang-format
+-rw-r--r--   0        0        0      575 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/ut/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      716 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/ut/ut.cpp.j2
+-rw-r--r--   0        0        0       33 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/templates/x86.cmake.j2
+-rw-r--r--   0        0        0     1597 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/tests_gen.py
+-rw-r--r--   0        0        0      550 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/toml_gen.py
+-rw-r--r--   0        0        0     5357 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/file_generators/ut_gen.py
+-rw-r--r--   0        0        0      629 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/global_values.py
+-rw-r--r--   0        0        0     2044 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/logger.py
+-rw-r--r--   0        0        0     1137 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/path_utils.py
+-rw-r--r--   0        0        0     2953 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/templates/.clang-format
+-rw-r--r--   0        0        0     8780 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/templates/.clang-tidy
+-rw-r--r--   0        0        0     2361 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/templates/.gitignore
+-rw-r--r--   0        0        0     1066 2023-08-08 05:19:54.269431 scargo-1.6.3/scargo/templates/LICENSE
+-rw-r--r--   0        0        0      519 2023-08-08 05:19:54.273431 scargo-1.6.3/setup.cfg
+-rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 scargo-1.6.3/PKG-INFO
```

### Comparing `scargo-1.6.2/CODE-OF-CONDUCT.md` & `scargo-1.6.3/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/LICENSE` & `scargo-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/README.md` & `scargo-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/pyproject.toml` & `scargo-1.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/certs/certGen.sh` & `scargo-1.6.3/scargo/certs/certGen.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/certs/generateAllCertificates.sh` & `scargo-1.6.3/scargo/certs/generateAllCertificates.sh`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
 if [ -f "$DIGIROOT_CERT" ]; then
     echo "$DIGIROOT_CERT already exists."
 else
     wget https://cacerts.digicert.com/DigiCertGlobalRootG2.crt.pem -O ${DIGIROOT_CERT}
     if [ $? -ne 0 ]; then
         echo -e "${RED} Failed to download Digiroot certificate" >&2
-        rm ${DIGIROOT_CERT}
+        rm -f ${DIGIROOT_CERT}
         exit 1
     fi
 fi
 
 cp ${DIGIROOT_CERT} ${CA_PEM}
 
 if [ ${MODE} == "Device-certificate" ]; then
```

### Comparing `scargo-1.6.2/scargo/certs/openssl_device_intermediate_ca.cnf` & `scargo-1.6.3/scargo/certs/openssl_device_intermediate_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/certs/openssl_root_ca.cnf` & `scargo-1.6.3/scargo/certs/openssl_root_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/clang_utils.py` & `scargo-1.6.3/scargo/clang_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/cli.py` & `scargo-1.6.3/scargo/cli.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/build.py` & `scargo-1.6.3/scargo/commands/build.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,28 +49,42 @@
         subprocess.check_call(
             [
                 "conan",
                 "install",
                 ".",
                 "-if",
                 build_dir,
+                "-of",
+                build_dir,
                 "-pr:b",
                 "default",
                 "-pr:h",
                 f"./.conan/profiles/{config.project.target.family}_{profile}",
                 "-b",
                 "missing",
             ],
             cwd=project_dir,
         )
         subprocess.check_call(
             [
                 "conan",
                 "build",
                 f"{project_dir}",
+                "-bf",
+                build_dir,
             ],
             cwd=build_dir,
         )
 
+        get_logger().info("Copying artifacts...")
+        # This is a workaround so that different profiles can work together with conan
+        # Conan always calls CMake with '
+        subprocess.check_call(
+            f"cp -r -l -f {build_dir}/build/{config.profiles[profile].cmake_build_type}/* .",
+            cwd=build_dir,
+            shell=True,
+        )
+        get_logger().info("Artifacts copied")
+
     except subprocess.CalledProcessError:
         logger.error("Unable to build exec file")
         sys.exit(1)
```

### Comparing `scargo-1.6.2/scargo/commands/check.py` & `scargo-1.6.3/scargo/commands/check.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/clean.py` & `scargo-1.6.3/scargo/commands/clean.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/debug.py` & `scargo-1.6.3/scargo/commands/debug.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/doc.py` & `scargo-1.6.3/scargo/commands/doc.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/docker.py` & `scargo-1.6.3/scargo/commands/docker.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/fix.py` & `scargo-1.6.3/scargo/commands/fix.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/flash.py` & `scargo-1.6.3/scargo/commands/flash.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/gen.py` & `scargo-1.6.3/scargo/commands/gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/new.py` & `scargo-1.6.3/scargo/commands/new.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/publish.py` & `scargo-1.6.3/scargo/commands/publish.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/run.py` & `scargo-1.6.3/scargo/commands/run.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/test.py` & `scargo-1.6.3/scargo/commands/test.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/commands/update.py` & `scargo-1.6.3/scargo/commands/update.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/config.py` & `scargo-1.6.3/scargo/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     @property
     def source_dir_path(self) -> Path:
         return self.project_root / self.project.target.source_dir
 
     @property
     def include_dir_path(self) -> Path:
-        return self.project_root / self.project.target.include_dir
+        return self.source_dir_path / self.project.target.include_dir
 
     def get_stm32_config(self) -> "Stm32Config":
         if not self.stm32:
             raise ConfigError("No [stm32] section in config")
         return self.stm32
 
     def get_esp32_config(self) -> "Esp32Config":
@@ -60,14 +60,30 @@
     ) -> Dict[str, Any]:
         if "project" in values:
             target_id = values["project"].target_id
             if target_id == "stm32" and not values["stm32"]:
                 raise ConfigError("No [stm32] section in config")
             if target_id == "esp32" and not values["esp32"]:
                 raise ConfigError("No [esp32] section in config")
+
+        # Set default value of cmake_build_type - Debug for non-stanard profiles,
+        # If profile is on standard_profiles list, use it's name instead
+        standard_profiles: List[str] = [
+            "Debug",
+            "Release",
+            "RelWithDebInfo",
+            "MinSizeRel",
+        ]
+        if "profiles" in values:
+            for name, profile in values["profiles"].items():
+                if profile.cmake_build_type is None:
+                    if name in standard_profiles:
+                        profile.cmake_build_type = name
+                    else:
+                        profile.cmake_build_type = "Debug"
         return values
 
 
 class ProjectConfig(BaseModel):
     name: str
     version: str
     description: Optional[str]
@@ -154,15 +170,15 @@
 
 
 class ProfileConfig(BaseModel, extra=Extra.allow):
     cflags: Optional[str]
     cxxflags: Optional[str]
     cc: Optional[str] = None
     cxx: Optional[str] = None
-    cmake_build_type: Optional[str] = Field("Debug", alias="cmake-build-type")
+    cmake_build_type: Optional[str] = Field(None, alias="cmake-build-type")
 
     @property
     def extras(self) -> Dict[str, Any]:
         return {
             key: value
             for key, value in dict(self).items()
             if key not in self.__fields__
```

### Comparing `scargo-1.6.2/scargo/config_utils.py` & `scargo-1.6.3/scargo/config_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/docker_utils.py` & `scargo-1.6.3/scargo/docker_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/base_gen.py` & `scargo-1.6.3/scargo/file_generators/base_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/clang_parser/data_classes.py` & `scargo-1.6.3/scargo/file_generators/clang_parser/data_classes.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/clang_parser/header_parser.py` & `scargo-1.6.3/scargo/file_generators/clang_parser/header_parser.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/clang_parser/params_extractor.py` & `scargo-1.6.3/scargo/file_generators/clang_parser/params_extractor.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/conan_gen.py` & `scargo-1.6.3/scargo/file_generators/conan_gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # #
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
-from typing import List
-
 from scargo.config import Config
 from scargo.file_generators.base_gen import create_file_from_template
 
 
 def generate_conanfile(config: Config) -> None:
     create_file_from_template(
         "conan/conanfile.py.j2",
@@ -21,15 +19,14 @@
         template_params={"config": config},
         config=config,
     )
 
 
 def generate_conanprofile(config: Config) -> None:
     profiles = config.profiles.keys()
-    standard_profiles: List[str] = ["Debug", "Release", "RelWithDebInfo", "MinSizeRel"]
 
     if config.project.target.family == "stm32":
         create_file_from_template(
             "conan/stm32_gcc_toolchain_wrapper.cmake.j2",
             ".conan/profiles/stm32_gcc_toolchain_wrapper.cmake",
             template_params={},
             config=config,
@@ -38,15 +35,14 @@
     for profile in profiles:
         create_file_from_template(
             "conan/profile.j2",
             f".conan/profiles/{config.project.target.family}_{profile}",
             template_params={
                 "config": config,
                 "profile": profile,
-                "standard_profiles": standard_profiles,
             },
             config=config,
         )
 
 
 def generate_test_package(config: Config) -> None:
     create_file_from_template(
```

### Comparing `scargo-1.6.2/scargo/file_generators/cpp_gen.py` & `scargo-1.6.3/scargo/file_generators/cpp_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         """Function which creates a lib files using jinja"""
 
         lib_name = lib_name.lower()
         class_name = "".join(lib_name.replace("_", " ").title().split())
 
         create_file_from_template(
             "cpp/lib.cpp.j2",
-            self._src_dir / f"{lib_name}.cpp",
+            self._src_dir / f"{self._config.project.target.source_dir}/{lib_name}.cpp",
             template_params={"class_name": class_name, "lib_name": lib_name},
             config=self._config,
         )
         create_file_from_template(
             "cpp/lib.h.j2",
             self._inc_dir / f"{lib_name}.h",
             template_params={"class_name": class_name},
```

### Comparing `scargo-1.6.2/scargo/file_generators/docker_gen.py` & `scargo-1.6.3/scargo/file_generators/docker_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/env_gen.py` & `scargo-1.6.3/scargo/file_generators/env_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/mock_gen.py` & `scargo-1.6.3/scargo/file_generators/mock_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/.gitlab-ci.yml.j2` & `scargo-1.6.3/scargo/file_generators/templates/.gitlab-ci.yml.j2`

 * *Files 3% similar despite different names*

```diff
@@ -35,27 +35,31 @@
 debug:
   stage: build
   extends: .merge_request
   script:
   {% if project.target.family == "esp32" %}
     - source /opt/esp/entrypoint.sh
   {% endif %}
-    - scargo build
+    - CONAN_LOGIN_USERNAME=ci_user
+    - CONAN_PASSWORD=${CI_JOB_TOKEN}
+    - scargo build --profile Debug
   artifacts:
     paths:
       - build/Debug/bin
       - build/Debug/lib
     when: always
 
 #_______________________________________________________________________________________________TEST
 tests:
   stage: test
   extends: .merge_request
   allow_failure: true
   script:
+    - CONAN_LOGIN_USERNAME=ci_user
+    - CONAN_PASSWORD=${CI_JOB_TOKEN}
     - scargo test
   artifacts:
     paths:
       - build/tests/ut-coverage.html
 
 #______________________________________________________________________________________________CLANG_FORMAT
 clang format:
```

### Comparing `scargo-1.6.2/scargo/file_generators/templates/CMakeLists.txt.j2` & `scargo-1.6.3/scargo/file_generators/templates/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/README.md.j2` & `scargo-1.6.3/scargo/file_generators/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/conan/conanfile.py.j2` & `scargo-1.6.3/scargo/file_generators/templates/conan/conanfile.py.j2`

 * *Files 5% similar despite different names*

```diff
@@ -24,50 +24,49 @@
     def build_requirements(self) -> None:
         {% for dep in config.dependencies.build %}
         self.requires("{{ dep }}")
         {% endfor %}
         {% for tool_dep in config.dependencies.tool %}
         self.tool_requires("{{ tool_dep }}")
         {% endfor %}
-
     {% endif %}
+
     {% if config.dependencies.general %}
     def requirements(self) -> None:
         {% for dep in config.dependencies.general %}
         self.requires("{{ dep }}")
         {% endfor %}
     {% endif %}
 
     {% if config.project.target.family == "stm32" %}
     def source(self) -> None:
         git = tools.Git(folder="third-party/stm32-cmake")
         git.clone("https://github.com/ObKo/stm32-cmake.git", "master")
     {% endif %}
 
-    def layout(self):
+    def layout(self) -> None:
         cmake_layout(self)
 
-    def generate(self):
+    def generate(self) -> None:
         tc = CMakeToolchain(self)
         tc.generate()
 
     def build(self) -> None:
         cmake = CMake(self)
         cmake.configure()
         cmake.build()
 
     def package(self) -> None:
-        {% if config.project.lib_name %}
+    {% if config.project.lib_name %}
         cmake = CMake(self)
         cmake.install()
-        {% endif %}
-        {% if config.project.bin_name %}
+    {% else %}
         self.copy("*.bin")
         self.copy("*.elf")
-        {% endif %}
+    {% endif %}
 
     {% if config.project.lib_name %}
     def package_info(self) -> None:
         self.cpp_info.libs = ["{{ config.project.name }}"]
     {% endif %}
```

### Comparing `scargo-1.6.2/scargo/file_generators/templates/conan/conanfiletest.j2` & `scargo-1.6.3/scargo/file_generators/templates/conan/conanfiletest.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/conan/profile_esp32.j2` & `scargo-1.6.3/scargo/file_generators/templates/conan/profile_x86.j2`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-[buildenv]
-WORKAROUND_FOR_ESP32_C_FLAGS="{{ config.project.cflags if config.project.cflags}} {{config.profiles.get(profile).cflags if config.profiles.get(profile).cflags}}"
-WORKAROUND_FOR_ESP32_IDF_CXX_FLAGS="{{ config.project.cxxflags if config.project.cxxflags }} {{ config.profiles.get(profile).cxxflags if config.profiles.get(profile).cxxflags }}"
+[env]
+
+{% if config.profiles[profile].cc %}
+CC={{ config.profiles[profile].cc }}
+{% else %}
+CC=gcc
+{% endif %}
+
+{% if config.profiles[profile].cxx %}
+CXX={{ config.profiles[profile].cxx }}
+{% else %}
+CXX=g++
+{% endif %}
+
 
 [settings]
 compiler=gcc
-compiler.version=8
-compiler.cppstd={{ config.project.cxxstandard }}
+compiler.version=9
 compiler.libcxx=libstdc++
+compiler.cppstd={{ config.project.cxxstandard }}
+os=Linux
+arch=x86_64
 os_build=Linux
 arch_build=x86_64
 
-os=baremetal
-arch=xtensalx6
-{# TODO: [kta] Here there is a code smell due to satisfy backwards-compatibility. Change in scargo 2.0 to: #}
-{# cmake_build_type = {{ config.profiles[profile].cmake_build_type }} #}
-{# This will enforce definition of cmake_build_type in scargo.toml [profile.X] section #}
-build_type={{ profile if (profile in standard_profiles) else config.profiles[profile].cmake_build_type }}
+build_type={{ config.profiles[profile].cmake_build_type }}
+
 
 [conf]
-tools.cmake.cmaketoolchain:toolchain_file=/opt/esp-idf/tools/cmake/toolchain-esp32.cmake
-tools.cmake.cmaketoolchain:generator=Ninja
+tools.build:cflags=["{{ config.project.cflags if config.project.cflags}} {{config.profiles.get(profile).cflags if config.profiles.get(profile).cflags}}"]
+tools.build:cxxflags=["{{ config.project.cxxflags if config.project.cxxflags }} {{ config.profiles.get(profile).cxxflags if config.profiles.get(profile).cxxflags }}"]
+{% if config.project.max_build_jobs != None %}
+tools.build:jobs={{config.project.max_build_jobs}}
+{% endif %}
 
 [options]
-[build_requires]
+[build_requires]
```

### Comparing `scargo-1.6.2/scargo/file_generators/templates/conan/profile_stm32.j2` & `scargo-1.6.3/scargo/file_generators/templates/conan/profile_stm32.j2`

 * *Files 25% similar despite different names*

```diff
@@ -21,18 +21,15 @@
 compiler.libcxx=libstdc++
 compiler.cppstd={{ config.project.cxxstandard }}
 os=baremetal
 arch=armv7
 os_build=Linux
 arch_build=x86_64
 
-{# TODO: [kta] Here there is a code smell due to satisfy backwards-compatibility. Change in scargo 2.0 to: #}
-{# cmake_build_type = {{ config.profiles[profile].cmake_build_type }} #}
-{# This will enforce definition of cmake_build_type in scargo.toml [profile.X] section #}
-build_type={{ profile if (profile in standard_profiles) else config.profiles[profile].cmake_build_type }}
+build_type={{ config.profiles[profile].cmake_build_type }}
 
 [conf]
 tools.build:cflags=["{{ config.project.cflags if config.project.cflags}} {{config.profiles.get(profile).cflags if config.profiles.get(profile).cflags}}"]
 tools.build:cxxflags=["{{ config.project.cxxflags if config.project.cxxflags }} {{ config.profiles.get(profile).cxxflags if config.profiles.get(profile).cxxflags }}"]
 
 tools.cmake.cmaketoolchain:user_toolchain=["/workspace/.conan/profiles/stm32_gcc_toolchain_wrapper.cmake"]
 {% if config.project.max_build_jobs != None %}
```

### Comparing `scargo-1.6.2/scargo/file_generators/templates/conan/profile_x86.j2` & `scargo-1.6.3/scargo/file_generators/templates/conan/profile_esp32.j2`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,22 @@
 [env]
-
-{% if config.profiles[profile].cc %}
-CC={{ config.profiles[profile].cc }}
-{% else %}
-CC=gcc
-{% endif %}
-
-{% if config.profiles[profile].cxx %}
-CXX={{ config.profiles[profile].cxx }}
-{% else %}
-CXX=g++
-{% endif %}
-
+WORKAROUND_FOR_ESP32_C_FLAGS="{{ config.project.cflags if config.project.cflags}} {{config.profiles.get(profile).cflags if config.profiles.get(profile).cflags}}"
+WORKAROUND_FOR_ESP32_CXX_FLAGS="{{ config.project.cxxflags if config.project.cxxflags }} {{ config.profiles.get(profile).cxxflags if config.profiles.get(profile).cxxflags }}"
 
 [settings]
 compiler=gcc
-compiler.version=9
-compiler.libcxx=libstdc++
+compiler.version=8
 compiler.cppstd={{ config.project.cxxstandard }}
-os=Linux
-arch=x86_64
+compiler.libcxx=libstdc++
 os_build=Linux
 arch_build=x86_64
 
-{# TODO: [kta] Here there is a code smell due to satisfy backwards-compatibility. Change in scargo 2.0 to: #}
-{# cmake_build_type = {{ config.profiles[profile].cmake_build_type }} #}
-{# This will enforce definition of cmake_build_type in scargo.toml [profile.X] section #}
-build_type={{ profile if (profile in standard_profiles) else config.profiles[profile].cmake_build_type }}
-
+os=baremetal
+arch=xtensalx6
+build_type={{ config.profiles[profile].cmake_build_type }}
 
 [conf]
-tools.build:cflags=["{{ config.project.cflags if config.project.cflags}} {{config.profiles.get(profile).cflags if config.profiles.get(profile).cflags}}"]
-tools.build:cxxflags=["{{ config.project.cxxflags if config.project.cxxflags }} {{ config.profiles.get(profile).cxxflags if config.profiles.get(profile).cxxflags }}"]
-
-
-{% if config.project.max_build_jobs != None %}
-tools.build:jobs={{config.project.max_build_jobs}}
-{% endif %}
+tools.cmake.cmaketoolchain:toolchain_file=/opt/esp-idf/tools/cmake/toolchain-esp32.cmake
+tools.cmake.cmaketoolchain:generator=Ninja
 
 [options]
-[build_requires]
+[build_requires]
```

### Comparing `scargo-1.6.2/scargo/file_generators/templates/conan/test_package/conanfile.py.j2` & `scargo-1.6.3/scargo/file_generators/templates/conan/test_package/conanfile.py.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/cpp/cmake-src-stm32.j2` & `scargo-1.6.3/scargo/file_generators/templates/cpp/cmake-src-stm32.j2`

 * *Files 16% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
 {% if  config.project.bin_name %}
 add_executable(${PROJECT_NAME}
      {{ config.project.bin_name|lower }}.cpp
 )
 {% elif config.project.lib_name%}
 add_library(${PROJECT_NAME} STATIC
-    ${CMAKE_CURRENT_SOURCE_DIR}/{{ config.include_dir_path.relative_to(config.project_root) }}/{{ config.project.lib_name|lower }}.h
+    ${CMAKE_CURRENT_SOURCE_DIR}/{{ config.project.target.source_dir }}/{{ config.project.lib_name|lower }}.cpp
 )
 
 target_include_directories(${PROJECT_NAME}
     PUBLIC
-        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>/{{ config.include_dir_path.relative_to(config.project_root) }}
+        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>/{{ config.project.target.include_dir }}
     PRIVATE
-        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>/{{ config.source_dir_path.relative_to(config.project_root) }}
+        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>/{{ config.project.target.source_dir }}
 )
 {% endif %}
 
 target_link_libraries(${PROJECT_NAME}
     CMSIS::STM32::${STM32_DEVICE}
     # HAL::STM32::${STM32_FAMILY}
     STM32::NoSys
@@ -71,9 +71,9 @@
     COMMAND ${CMAKE_OBJCOPY} -O ihex $<TARGET_FILE:${PROJECT_NAME}> ${CMAKE_RUNTIME_OUTPUT_DIRECTORY}/${PROJECT_NAME}.hex
     BYPRODUCTS ${PROJECT_NAME}.hex
     COMMENT "Generating hex file ${CMAKE_PROJECT_NAME}.hex"
 )
 {% endif %}
 {% if config.project.lib_name %}
 install(TARGETS ${PROJECT_NAME} DESTINATION lib)
-install(DIRECTORY {{ config.include_dir_path.relative_to(config.project_root) }}/ DESTINATION {{ config.include_dir_path.relative_to(config.project_root) }})
+install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/{{ config.project.target.include_dir }}/ DESTINATION {{ config.project.target.include_dir }})
 {% endif %}
```

### Comparing `scargo-1.6.2/scargo/file_generators/templates/cpp/cmake-src-x86.j2` & `scargo-1.6.3/scargo/file_generators/templates/cpp/cmake-src-x86.j2`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 {% if config.project.bin_name %}
-add_executable({{ config.project.bin_name|lower }})
-target_sources({{ config.project.bin_name|lower }} PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/{{ config.project.bin_name|lower }}.cpp)
+add_executable(${PROJECT_NAME}
+    ${CMAKE_CURRENT_SOURCE_DIR}/{{ config.project.bin_name|lower }}.cpp
+)
 
 {% endif %}
 {% if config.project.lib_name %}
 add_library(${PROJECT_NAME} STATIC
-    ${CMAKE_CURRENT_SOURCE_DIR}/{{ config.project.lib_name|lower }}.cpp
+    ${CMAKE_CURRENT_SOURCE_DIR}/{{ config.project.target.source_dir }}/{{ config.project.lib_name|lower }}.cpp
 )
 
 target_include_directories(${PROJECT_NAME}
     PUBLIC
-        $<BUILD_INTERFACE:${CMAKE_SOURCE_DIR}>/{{ config.include_dir_path.relative_to(config.project_root) }}
+        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>/{{ config.project.target.include_dir }}
     PRIVATE
-        $<BUILD_INTERFACE:${CMAKE_SOURCE_DIR}>
+        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>/{{ config.project.target.source_dir }}
 )
 
 {% endif %}
 {% if config.project.lib_name %}
 install(TARGETS ${PROJECT_NAME} DESTINATION lib)
-install(DIRECTORY ${CMAKE_SOURCE_DIR}/{{ config.include_dir_path.relative_to(config.project_root) }}/ DESTINATION {{ config.include_dir_path.relative_to(config.project_root) }})
+install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/{{ config.project.target.include_dir }}/ DESTINATION {{ config.project.target.include_dir }})
 {% endif %}
```

### Comparing `scargo-1.6.2/scargo/file_generators/templates/cpp/main.cpp.j2` & `scargo-1.6.3/scargo/file_generators/templates/cpp/main.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-esp32.j2` & `scargo-1.6.3/scargo/file_generators/templates/docker/Dockerfile-esp32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile-stm32.j2` & `scargo-1.6.3/scargo/file_generators/templates/docker/Dockerfile-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/docker/Dockerfile.j2` & `scargo-1.6.3/scargo/file_generators/templates/docker/Dockerfile.j2`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     apt -y install sudo && \
     rm -rf /var/lib/apt/lists/* && \
     update-alternatives --install /usr/bin/python python /usr/bin/python3 1
 
 FROM base AS cpp
 
 RUN apt update --fix-missing && apt -y --no-install-recommends install cppcheck lib32z1 \
-    make cmake clang clang-format clang-tidy gcovr doxygen libcmocka0 libcmocka-dev gdb screen && \
+    make cmake clang clang-format clang-tidy gcovr doxygen libcmocka0 libcmocka-dev gdb screen wget && \
     rm -rf /var/lib/apt/lists/*
 
 FROM cpp AS {{ project.target.family }}
 {% include 'docker/Dockerfile-' + project.target.family + '.j2' %}
 
 WORKDIR /opt
```

### Comparing `scargo-1.6.2/scargo/file_generators/templates/docker/devcontainer.json.j2` & `scargo-1.6.3/scargo/file_generators/templates/docker/devcontainer.json.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/docker/docker-compose.yaml.j2` & `scargo-1.6.3/scargo/file_generators/templates/docker/docker-compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/esp32.cmake.j2` & `scargo-1.6.3/scargo/file_generators/templates/esp32.cmake.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/mock/class_interface.h.j2` & `scargo-1.6.3/scargo/file_generators/templates/mock/class_interface.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/mock/class_mock.cpp.j2` & `scargo-1.6.3/scargo/file_generators/templates/mock/class_mock.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/mock/class_mock.h.j2` & `scargo-1.6.3/scargo/file_generators/templates/mock/class_mock.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/scargo.toml.j2` & `scargo-1.6.3/scargo/file_generators/templates/scargo.toml.j2`

 * *Files 27% similar despite different names*

```diff
@@ -72,28 +72,34 @@
 cxx = "g++"
 
 cflags   = "-Wall -Wextra -Og --coverage -fkeep-inline-functions -fkeep-static-consts"
 cxxflags = "-Wall -Wextra -Og --coverage -fkeep-inline-functions -fkeep-static-consts"
 
 gcov-executable = "" # Empty string -> use default gcov executable
 
-# conan dependencies "lib_name/version"
+# Underhood scargo use conan. All string valid for conan tool are valid here. eg "gtest/1.13.0"
 [dependencies]
+#general -> public conan dependencies of project they will be added to package info (eg. bianry dynamic linkage libary) they will be added also to scargo test. 
 general = [
 ]
+#build -> private conan dependencies usedn only during build process(eg. private static linkage library)
 build = [
 ]
+#tool -> special conan "not library" dependencies like cmake/3.22.
 tool = [
 ]
+#test-> conan dependencies used only for testing targets
 test = [
-    "gtest/cci.20210126"
+    "gtest/1.13.0"
 ]
 
 [conan.repo]
-# conancenter = "https://center.conan.io"
+#Passing conancenter here is not nessary as scargo adds it by default
+#Below example of private binary artifacts repository 
+#gitlab = "https://git.my_extra_gitlab_server.com"
 
 {% if target.family == "esp32" %}
 [esp32]
 extra_component_dirs=[]
 partitions = [
     "nvs,      data, nvs,     0x9000,  0x4000,",
     "otadata,  data, ota,     0xd000,  0x2000,",
```

### Comparing `scargo-1.6.2/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2` & `scargo-1.6.3/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/tests/static_mock/static_mock.h` & `scargo-1.6.3/scargo/file_generators/templates/tests/static_mock/static_mock.h`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/ut/CMakeLists.txt.j2` & `scargo-1.6.3/scargo/file_generators/templates/ut/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/templates/ut/ut.cpp.j2` & `scargo-1.6.3/scargo/file_generators/templates/ut/ut.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/tests_gen.py` & `scargo-1.6.3/scargo/file_generators/tests_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/toml_gen.py` & `scargo-1.6.3/scargo/file_generators/toml_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/file_generators/ut_gen.py` & `scargo-1.6.3/scargo/file_generators/ut_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/global_values.py` & `scargo-1.6.3/scargo/global_values.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/logger.py` & `scargo-1.6.3/scargo/logger.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/path_utils.py` & `scargo-1.6.3/scargo/path_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/templates/.clang-format` & `scargo-1.6.3/scargo/templates/.clang-format`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/templates/.clang-tidy` & `scargo-1.6.3/scargo/templates/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/templates/.gitignore` & `scargo-1.6.3/scargo/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/scargo/templates/LICENSE` & `scargo-1.6.3/scargo/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/setup.cfg` & `scargo-1.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `scargo-1.6.2/PKG-INFO` & `scargo-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scargo
-Version: 1.6.2
+Version: 1.6.3
 Summary: C/C++ package and software development life cycle manager inspired by RUST cargo idea.
 Keywords: scargo,Package manager,C++
 Author-email: "Spyrosoft Solutions S.A." <aak@spyro-soft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

