# Comparing `tmp/kfsd-0.0.80.tar.gz` & `tmp/kfsd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsd-0.0.80.tar", last modified: Tue Aug  8 00:58:11 2023, max compression
+gzip compressed data, was "kfsd-0.0.9.tar", last modified: Mon May  1 02:53:48 2023, max compression
```

## Comparing `kfsd-0.0.80.tar` & `kfsd-0.0.9.tar`

### file list

```diff
@@ -1,290 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 00:57:32.000000 kfsd-0.0.80/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-08 00:58:11.206902 kfsd-0.0.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-08 00:57:32.000000 kfsd-0.0.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.186902 kfsd-0.0.80/kfsd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.186902 kfsd-0.0.80/kfsd/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.186902 kfsd-0.0.80/kfsd/apps/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.186902 kfsd-0.0.80/kfsd/apps/core/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/auth/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/auth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/auth/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/auth/api/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/auth/api/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/auth/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/common/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/common/kubefacets_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/common/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/common/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/exceptions/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/exceptions/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/exceptions/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/exceptions/fe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/management/commands/basemsmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/management/commands/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/middleware/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/middleware/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/middleware/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/msmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/msmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/msmq/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/msmq/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/msmq/rabbitmq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/services/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/services/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/services/gateway/sso.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/base_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/tests/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/tests/v1/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/common/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/common/test_kubefacets_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/common/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/common/test_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.190902 kfsd-0.0.80/kfsd/apps/core/tests/v1/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_arr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/arr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/core/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/core/utils/http/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/django/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/django/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/django/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/django/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/core/utils/http/headers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/headers/apikey.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/headers/contenttype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/headers/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/headers/csrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/http/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/core/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/endpoints/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/endpoints/handlers/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/handlers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/handlers/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/handlers/common/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/handlers/common/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/endpoints/handlers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/handlers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/handlers/utils/arr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/handlers/utils/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/handlers/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/endpoints/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/renderers/kubefacetsjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/renderers/kubefacetstext.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/renderers/kubefacetsyaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.194902 kfsd-0.0.80/kfsd/apps/endpoints/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/cid.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/id.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/outpost.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/tid.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/common/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/serializers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/utils/arr.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/utils/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/serializers/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/endpoints_test_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/data/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/data/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/test_cid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/test_common_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/test_oid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/test_pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/test_tid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/test_uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/utils/test_utils_arr.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/utils/test_utils_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/utils/test_utils_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.198902 kfsd-0.0.80/kfsd/apps/endpoints/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/endpoints/views/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/cid.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/outpost.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/tid.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/common/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/cid.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/outpost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/tid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/cid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/outpost.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/tid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/endpoints/views/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/pagination/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/endpoints/views/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/endpoints/views/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/frontend/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/permissions/active.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/permissions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/permissions/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/permissions/signin.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/permissions/staff.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/permissions/superuser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/frontend/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.202902 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/docs/browser.html
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/docs/skeleton.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/templates/v1/errors/500.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/frontend/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/frontend/tests/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/tests/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/tests/v1/test_api_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/frontend/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/frontend/views/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/views/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/views/docs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/frontend/views/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/views/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/views/errors/custom403.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/views/errors/custom404.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/views/errors/custom500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/frontend/views/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/views/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/frontend/views/permissions/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/models/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/models/fixtures/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/fixtures/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/models/fixtures/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/fixtures/v1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/models/fixtures/v1/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/fixtures/v1/tests/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/models/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.206902 kfsd-0.0.80/kfsd/apps/models/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/cid.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/id.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/outpost.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/tid.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/apps/models/tables/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 00:57:32.000000 kfsd-0.0.80/kfsd/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 00:58:11.186902 kfsd-0.0.80/kfsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-08 00:58:11.000000 kfsd-0.0.80/kfsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-08-08 00:58:11.000000 kfsd-0.0.80/kfsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 00:58:11.000000 kfsd-0.0.80/kfsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-08 00:58:11.000000 kfsd-0.0.80/kfsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 00:58:11.000000 kfsd-0.0.80/kfsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 00:58:11.206902 kfsd-0.0.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-08 00:57:32.000000 kfsd-0.0.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.098708 kfsd-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 02:52:57.000000 kfsd-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 02:53:48.098708 kfsd-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 02:52:57.000000 kfsd-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.054707 kfsd-0.0.9/kfsd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.058708 kfsd-0.0.9/kfsd/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.058708 kfsd-0.0.9/kfsd/apps/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.058708 kfsd-0.0.9/kfsd/apps/core/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.058708 kfsd-0.0.9/kfsd/apps/core/auth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/api/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/api/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/exceptions/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/exceptions/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/exceptions/fe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/middleware/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/middleware/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/middleware/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/base_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/tests/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.066707 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.066707 kfsd-0.0.9/kfsd/apps/core/tests/v1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.066707 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.070707 kfsd-0.0.9/kfsd/apps/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.070707 kfsd-0.0.9/kfsd/apps/core/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.070707 kfsd-0.0.9/kfsd/apps/core/utils/http/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/contenttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/csrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/endpoints/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.078708 kfsd-0.0.9/kfsd/apps/endpoints/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetsjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetstext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetsyaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.078708 kfsd-0.0.9/kfsd/apps/endpoints/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.078708 kfsd-0.0.9/kfsd/apps/endpoints/serializers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/common/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/common/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.078708 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/endpoints_test_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/common/test_common_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/pagination/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.090707 kfsd-0.0.9/kfsd/apps/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/browser.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/skeleton.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/errors/500.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/tests/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/tests/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/tests/v1/test_api_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/views/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/docs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/views/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/errors/custom403.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/errors/custom404.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/errors/custom500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.098708 kfsd-0.0.9/kfsd/apps/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/models/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.054707 kfsd-0.0.9/kfsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 02:53:48.098708 kfsd-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-01 02:52:57.000000 kfsd-0.0.9/setup.py
```

### Comparing `kfsd-0.0.80/kfsd/apps/core/common/configuration.py` & `kfsd-0.0.9/kfsd/apps/core/common/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,31 @@
 import functools
-
 from kfsd.apps.core.utils.arr import ArrUtils
 from kfsd.apps.core.utils.dict import DictUtils
 
 
 class Configuration:
     def __init__(self, **kwargs):
-        self.__rawSettings = {
-            tuple(item["setting"]): item
-            for item in DictUtils.deepcopy(kwargs.pop("settings"))
-        }
-        self.__reqKeyList = [
-            "{}:{}".format(k, v) for (k, v) in kwargs.pop("dimensions").items()
-        ]
+        self.__rawSettings = {tuple(item['setting']): item for item in kwargs.pop('settings')}
+        self.__reqKeyList = ["{}:{}".format(k, v) for (k, v) in kwargs.pop('dimensions').items()]
         self.__mergeRecursive = kwargs.get("merge_recursive", True)
         self.__arr_rm_dupes = kwargs.get("arr_rm_dupes", True)
         self.__config = self.generateConfig()
 
     @staticmethod
     def findConfigValues(config, paths):
         configs = [DictUtils.get_by_path(config, path) for path in paths]
         return configs
 
     def getFinalConfig(self):
         return self.__config
 
     def findSetting(self, key):
         tupleKey = tuple(key)
-        return (
-            {} if tupleKey not in self.__rawSettings else self.__rawSettings[tupleKey]
-        )
+        return {} if tupleKey not in self.__rawSettings else self.__rawSettings[tupleKey]
 
     def getAllSubsetKeys(self, findKey):
         return [x for x in self.__rawSettings.keys() if self.isSubset(findKey, x)]
 
     def isSubset(self, tuple1, tuple2):
         set1 = set(tuple1)
         set2 = set(tuple2)
@@ -46,32 +38,25 @@
         childKeys = ArrUtils.sort_keys_by_len(self.getAllSubsetKeys(self.__reqKeyList))
         masterConfig = self.findSetting(["master"])
         for childkey in childKeys:
             masterConfig = DictUtils.merge(
                 dict1=masterConfig,
                 dict2=self.findSetting(childkey),
                 merge_recursive=self.__mergeRecursive,
-                arr_rm_dupes=self.__arr_rm_dupes,
+                arr_rm_dupes=self.__arr_rm_dupes
             )
-            masterConfig.pop("setting")
-
-        if "setting" in masterConfig:
-            masterConfig.pop("setting")
-
+            masterConfig.pop('setting')
         return masterConfig
 
     def getConfig(self, key):
         keys = key.split(".")
-        value = functools.reduce(
-            lambda d, key: (d.get(key) if isinstance(d, dict) else None) if d else None,
-            keys,
-            self.__config,
-        )
+        value = functools.reduce(lambda d, key: (d.get(key) if isinstance(d, dict) else None) if d else None, keys,
+                                 self.__config)
         if value is None:
-            raise Exception("Config key:{} not found".format(key))
+            raise Exception('Config key:{} not found'.format(key))
         return value
 
     def getConfigWithDefault(self, key, default):
         try:
             return self.getConfig(key)
         except Exception:
             return default
```

### Comparing `kfsd-0.0.80/kfsd/apps/core/common/logger.py` & `kfsd-0.0.9/kfsd/apps/core/common/logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from enum import Enum
 from functools import wraps
 from kfsd.apps.core.common.singleton import Singleton
 
 import logging
-import json
 
 
 class Logger:
-    __defaultFormat = "[%(asctime)s][%(name)s][%(levelname)s] %(message)s"
+    __defaultFormat = '[%(asctime)s][%(name)s][%(levelname)s] %(message)s'
 
     def __init__(self, fileName, logLevel, stream=None):
         self.__logger = logging.getLogger(fileName)
         self.__handler = self.setStreamHandler(stream)
         self.__getLoggerLevel(logLevel)
         self.setFormat(self.__defaultFormat)
 
@@ -60,58 +59,19 @@
             loggerLevelDict = {}
             loggerLevelDict[str(LogLevel.CRITICAL)] = logging.CRITICAL
             loggerLevelDict[str(LogLevel.ERROR)] = logging.ERROR
             loggerLevelDict[str(LogLevel.WARNING)] = logging.WARNING
             loggerLevelDict[str(LogLevel.INFO)] = logging.INFO
             loggerLevelDict[str(LogLevel.DEBUG)] = logging.DEBUG
             loggerLevelDict[str(LogLevel.NOTSET)] = logging.NOTSET
-            loggingLevel = (
-                loggerLevelDict[str(logLevel)]
-                if str(logLevel) in loggerLevelDict
-                else logging.NOTSET
-            )
+            loggingLevel = loggerLevelDict[str(logLevel)] if str(logLevel) in loggerLevelDict else logging.NOTSET
             return self.__logger.setLevel(loggingLevel)
 
         return self.__logger.setLevel(logging.NOTSET)
 
-    def getLogMethod(self, errorType):
-        logMap = {
-            "error": self.error,
-            "warn": self.warn,
-            "debug": self.debug,
-            "info": self.info,
-            "critical": self.critical,
-        }
-        if errorType in logMap:
-            return logMap[errorType]
-        else:
-            return self.error
-
-    def getAttr(self, obj, attr):
-        if hasattr(obj, attr):
-            return getattr(obj, attr)
-        return None
-
-    def logWebRequestError(self, request, error, errorType):
-        x_apikey = request.headers["X_Apikey"] if "X_Apikey" in request.headers else ""
-        errorData = {
-            "request_info": {
-                "path": request.build_absolute_uri(),
-                "method": self.getAttr(request, "method"),
-                "api_key": x_apikey,
-                "content_type": self.getAttr(request, "content_type"),
-                "query_params": self.getAttr(request, "query_params"),
-                "body": self.getAttr(request, "data")
-            },
-            "error": error,
-        }
-        errorStr = json.dumps(errorData, indent=4)
-
-        self.getLogMethod(errorType)(errorStr)
-
 
 class LogLevel(Enum):
     CRITICAL = 0
     ERROR = 1
     WARNING = 2
     INFO = 3
     DEBUG = 4
@@ -121,22 +81,19 @@
 def InstanceDebug(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         selfObj = args[0]
         result = func(*args, **kwargs)
         selfObj.getLogObj().debug("Input:{}, Output: {}".format(args, result))
         return result
-
     return wrapper
 
 
 def Debug(logger):
     def debugWrapper(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             result = func(*args, **kwargs)
             logger.debug("Input:{}, Output: {}".format(args, result))
             return result
-
         return wrapper
-
     return debugWrapper
```

### Comparing `kfsd-0.0.80/kfsd/apps/core/common/yaml.py` & `kfsd-0.0.9/kfsd/apps/core/common/yaml.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/tests/base_api.py` & `kfsd-0.0.9/kfsd/apps/core/tests/base_api.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/tests/v1/common/test_configuration.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_configuration.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/tests/v1/common/test_logger.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_logger.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/tests/v1/common/test_yaml.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_yaml.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_arr.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_arr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_attr.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_attr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_dict.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_file.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_file.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/tests/v1/utils/test_system.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_system.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/arr.py` & `kfsd-0.0.9/kfsd/apps/core/utils/arr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/attr.py` & `kfsd-0.0.9/kfsd/apps/core/utils/attr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/dict.py` & `kfsd-0.0.9/kfsd/apps/core/utils/dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from collections.abc import Mapping
 import functools
-import copy
 
 from kfsd.apps.core.common.logger import Logger, LogLevel
 
 logger = Logger.getSingleton(__name__, LogLevel.DEBUG)
 
 
 class DictUtils:
 
     @staticmethod
-    def deepcopy(d):
-        return copy.deepcopy(d)
-
-    @staticmethod
     def get_all_keys(arr, d):
         for k, v in d.items():
             arr.append(k)
             if isinstance(d.get(k), dict) and isinstance(v, Mapping):
                 DictUtils.get_all_keys(arr, d.get(k, {}))
 
     @staticmethod
```

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/file.py` & `kfsd-0.0.9/kfsd/apps/core/utils/file.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/http/base.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,52 +5,42 @@
 
 from kfsd.apps.core.exceptions.api import KubefacetsAPIException
 from kfsd.apps.core.utils.http.response import Response
 
 
 class HTTP(Response):
     def formatUrl(self, args):
-        if None in args:
-            raise KubefacetsAPIException(
-                "Invalid url paths passed for forming url",
-                "url_error",
-                status.HTTP_400_BAD_REQUEST,
-                "Probably config error, plz check if services are up?",
-            )
         return "/".join(args)
 
     def genUrlEncode(self, urlstr):
         return urllib.parse.quote(urlstr)
 
     def request(self, method, url, expStatus, **kwargs):
         try:
             resp = method(url, **kwargs)
             self.setResponse(resp)
             if self.isRespValid(expStatus):
                 return resp
-        except requests.exceptions.Timeout as e:
+        except requests.exceptions.Timeout:
             raise KubefacetsAPIException(
                 "The server took too long to respond to your request. Please try again later.",
                 "server_timed_out",
                 status.HTTP_408_REQUEST_TIMEOUT,
-                "url: {}, error: {}".format(url, str(e)),
             )
-        except requests.exceptions.ConnectionError as e:
+        except requests.exceptions.ConnectionError:
             raise KubefacetsAPIException(
                 "Service temporarily unavailable. Please try again later.",
                 "service_unavailable",
                 status.HTTP_503_SERVICE_UNAVAILABLE,
-                "url: {}, error: {}".format(url, str(e)),
             )
-        except urllib3.exceptions.NewConnectionError as e:
+        except urllib3.exceptions.NewConnectionError:
             raise KubefacetsAPIException(
                 "Service temporarily unavailable. Please try again later.",
                 "service_unavailable",
                 status.HTTP_503_SERVICE_UNAVAILABLE,
-                "url: {}, error: {}".format(url, str(e)),
             )
 
     def post(self, url, expStatus, **kwargs):
         return self.request(requests.post, url, expStatus, **kwargs)
 
     def get(self, url, expStatus, **kwargs):
         return self.request(requests.get, url, expStatus, **kwargs)
```

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/http/django/cookie.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/django/cookie.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import http.cookies
 
 from kfsd.apps.core.utils.dict import DictUtils
+from kfsd.apps.core.exceptions.exec import ExecException
 
 
 class Cookie:
     KEY = 'key'
     COOKIE = 'cookie'
-    EXPIRY_IN_SECS = 'expiry_in_secs'
+    EXPIRY_IN_MINS = 'expiry_in_mins'
     SECURE = 'secure'
     HTTP_ONLY = 'http_only'
     SAME_SITE = 'same_site'
 
     def __init__(self, httpObj):
         self.__httpObj = httpObj
 
@@ -22,23 +23,32 @@
 
     def getAllCookies(self):
         return self.__httpObj.COOKIES
 
     def getCookie(self, key):
         return self.__httpObj.COOKIES.get(key)
 
-    def setCookie(self, **kwargs):
-        self.getHttpObj().set_cookie(
+    def setCookie(self, unset=False, **kwargs):
+        if not unset:
+            requiredKeys = [self.KEY, self.COOKIE, self.EXPIRY_IN_MINS, self.SECURE, self.HTTP_ONLY, self.SAME_SITE]
+            if not DictUtils.key_exists_multi(kwargs, requiredKeys):
+                raise ExecException("Required cookie settings keys does not exist, keys: {}".format(requiredKeys))
+
+            self.getHttpObj().set_cookie(
                 key=kwargs[self.KEY],
                 value=kwargs[self.COOKIE],
-                expires=kwargs[self.EXPIRY_IN_SECS],
+                expires=kwargs[self.EXPIRY_IN_MINS]*60,
                 secure=kwargs[self.SECURE],
                 httponly=kwargs[self.HTTP_ONLY],
                 samesite=kwargs[self.SAME_SITE]
             )
+        else:
+            self.getHttpObj().delete_cookie(
+                key=kwargs[self.KEY]
+            )
 
     def cookiesToHeaderStr(self, rmCookieKeys=[]):
         cookie_string = ''
         if self.getAllCookies():
             cookie = http.cookies.SimpleCookie()
             filteredCookies = DictUtils.filter_by_keys_neg(self.getAllCookies(), rmCookieKeys)
             cookie.update(filteredCookies)
```

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/http/headers/base.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/headers/base.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/http/headers/cookie.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/headers/cookie.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/http/request.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         self.__expStatusCode = None
 
     def setExpStatusCode(self, code):
         self.__expStatusCode = code
 
     def request(self, method, url, expStatus, **kwargs):
         try:
+            print("Req Headers: {}".format(self.getReqHeaders()))
             resp = method(url, **kwargs)
             self.setResponse(resp)
             if self.isRespValid(expStatus):
                 return resp
         except requests.exceptions.Timeout:
             raise KubefacetsAPIException(
                 "The server took too long to respond to your request. Please try again later.",
```

### Comparing `kfsd-0.0.80/kfsd/apps/core/utils/system.py` & `kfsd-0.0.9/kfsd/apps/core/utils/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from kfsd.apps.core.exceptions.exec import ExecExceptionHandler
 from kfsd.apps.core.utils.file import FileUtils
 
 logger = Logger.getSingleton(__name__, LogLevel.DEBUG)
 
 
 class System:
+
     def __init__(self, **kwargs):
         self.__cmdExecStatus = False
         self.__cmdExecOutput = None
 
     def setCmdExecStatus(self, cmdStatus):
         self.__cmdExecStatus = cmdStatus
 
@@ -41,15 +42,15 @@
         return self.getCmdExecOutput()
 
     def osArch(self):
         self.cmdExec("uname -m")
         return self.getCmdExecOutput().lower()
 
     def hostIP(self):
-        return netifaces.ifaddresses(self.getNIC())[netifaces.AF_INET][0]["addr"]
+        return netifaces.ifaddresses(self.getNIC())[netifaces.AF_INET][0]['addr']
 
     def getNIC(self):
         nicPath = "/sys/class/net/{}/"
         if FileUtils.path_exists(nicPath.format("eth0")):
             return "eth0"
         elif FileUtils.path_exists(nicPath.format("enp5s0")):
             return "enp5s0"
@@ -64,18 +65,15 @@
 
     def changeFilePermission(self, permission, filePath):
         self.cmdExec("chmod {} {}".format(permission, filePath))
         return self.getCmdExecStatus()
 
     def cmdsExec(self, cmds, captureOutput=True, shell=False):
         return [
-            self.cmdExec(cmd, captureOutput, shell)
-            if not type(cmd) == list
-            else self.cmdsExec(cmd, captureOutput, shell)
-            for cmd in cmds
+            self.cmdExec(cmd, captureOutput, shell) if not type(cmd) == list else self.cmdsExec(cmd, captureOutput, shell) for cmd in cmds
         ]
 
     def cmdExec(self, cmd, captureOutput=True, shell=False):
         if captureOutput:
             cmdOutput = subprocess.getstatusoutput(cmd)
             cmdExecStatus = True if cmdOutput[0] == 0 else False
             cmdOutput = cmdOutput[1]
@@ -84,15 +82,15 @@
         else:
             logger.debug("CMD: {}".format(cmd))
             proc = subprocess.Popen(
                 shlex.split(cmd) if not shell else cmd,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
                 shell=shell,
-                universal_newlines=True,
+                universal_newlines=True
             )
             for line in iter(proc.stdout.readline, ""):
                 logger.debug("{}".format(line.strip()))
             proc.stdout.close()
 
     @staticmethod
     @ExecExceptionHandler(logger)
@@ -110,24 +108,24 @@
         if isinstance(data, str):
             formattedData = data.encode("utf-8")
         elif isinstance(data, list) or isinstance(data, dict):
             formattedData = json.dumps(data).encode("utf-8")
         else:
             formattedData = bytes(data)
 
-        return zlib.adler32(formattedData) & 0xFFFFFFFF
+        return zlib.adler32(formattedData) & 0xffffffff
 
     @staticmethod
     @ExecExceptionHandler(logger)
     def uuid(len):
-        return secrets.token_hex(int(len / 2))
+        return secrets.token_hex(int(len/2))
 
     @staticmethod
     @ExecExceptionHandler(logger)
     def secret(len):
         return secrets.token_urlsafe(len)
 
     @staticmethod
     @ExecExceptionHandler(logger)
     def api_key(len):
-        api_key_bytes = secrets.token_bytes(int(len / 2))
-        return binascii.hexlify(api_key_bytes).decode("utf-8")
+        api_key_bytes = secrets.token_bytes(int(len/2))
+        return binascii.hexlify(api_key_bytes).decode('utf-8')
```

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/handlers/common/base.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/base.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/handlers/common/configuration.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/configuration.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/handlers/utils/arr.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/arr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/handlers/utils/attr.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/attr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/handlers/utils/system.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/system.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/renderers/kubefacetsjson.py` & `kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetsjson.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/renderers/kubefacetsyaml.py` & `kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetsyaml.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/serializers/base.py` & `kfsd-0.0.9/kfsd/apps/endpoints/serializers/base.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/serializers/utils/system.py` & `kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/system.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/tests/endpoints_test_handler.py` & `kfsd-0.0.9/kfsd/apps/endpoints/tests/endpoints_test_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,56 +22,56 @@
 
     def detailView(self, name, identifier):
         return reverse(name, args=[identifier])
 
     def createView(self, name):
         return reverse(name)
 
-    def rmAttrs(self, resp, stripAttrs=["created", "updated", "id"]):
+    def stripCommonAttrs(self, resp):
         if isinstance(resp, dict):
-            return DictUtils.filter_by_keys_neg(resp, stripAttrs)
+            return DictUtils.filter_by_keys_neg(resp, ["created", "updated", "id"])
         return resp
 
-    def rmAttrsFromResults(self, resp, stripAttrs=["created", "updated", "id"]):
+    def stripCommonAttrsFromResults(self, resp):
         formattedResults = []
         results = DictUtils.get(resp, "results")
         if results:
             for item in results:
-                strippedItem = self.rmAttrs(item, stripAttrs)
+                strippedItem = self.stripCommonAttrs(item)
                 formattedResults.append(strippedItem)
 
         resp["results"] = formattedResults
         return resp
 
-    def list(self, url, currentPg, expStatus, stripAttrs=["created", "updated", "id"]):
+    def list(self, url, currentPg, expStatus, stripCommonAttrs=True):
         paginatedUrl = self.fetchPg(url, currentPg)
         response = self.client.get(paginatedUrl, format='json')
         self.assertEqual(response.status_code, expStatus, response.data)
-        return self.rmAttrsFromResults(response.data, stripAttrs) if stripAttrs else response.data
+        return self.stripCommonAttrsFromResults(response.data) if stripCommonAttrs else response.data
 
-    def get(self, name, identifier, expStatus, stripAttrs=["created", "updated", "id"]):
+    def get(self, name, identifier, expStatus, stripCommonAttrs=True):
         detailUrl = self.detailView(name, identifier)
         response = self.client.get(detailUrl, format='json')
         self.assertEqual(response.status_code, expStatus, response.data)
-        return self.rmAttrs(response.data, stripAttrs) if stripAttrs else response.data
+        return self.stripCommonAttrs(response.data) if stripCommonAttrs else response.data
 
-    def create(self, url, data, expStatus, stripAttrs=["created", "updated", "id"]):
+    def create(self, url, data, expStatus, stripCommonAttrs=True):
         response = self.client.post(url, data, format='json')
         self.assertEqual(response.status_code, expStatus, response.data)
-        return self.rmAttrs(response.data, stripAttrs) if stripAttrs else response.data
+        return self.stripCommonAttrs(response.data) if stripCommonAttrs else response.data
 
-    def post(self, url, data, expStatus, stripAttrs=["created", "updated", "id"]):
+    def post(self, url, data, expStatus, stripCommonAttrs=True):
         response = self.client.post(url, data, format='json')
         self.assertEqual(response.status_code, expStatus, response.data)
-        return self.rmAttrs(response.data, stripAttrs) if stripAttrs else response.data
+        return self.stripCommonAttrs(response.data) if stripCommonAttrs else response.data
 
-    def patch(self, name, identifier, data, expStatus, stripAttrs=["created", "updated", "id"]):
+    def patch(self, name, identifier, data, expStatus, stripCommonAttrs=True):
         detailUrl = self.detailView(name, identifier)
         response = self.client.patch(detailUrl, data=data, format='json')
         self.assertEqual(response.status_code, expStatus, response.data)
-        return self.rmAttrs(response.data, stripAttrs) if stripAttrs else response.data
+        return self.stripCommonAttrs(response.data) if stripCommonAttrs else response.data
 
     def delete(self, name, identifier, expStatus):
         detailUrl = self.detailView(name, identifier)
         response = self.client.delete(detailUrl, format='json')
         self.assertEqual(response.status_code, expStatus, response.data)
         return response
```

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/common/test_common_configuration.py` & `kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/common/test_common_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,19 @@
 
     def postYaml(self, url, data, expStatus,):
         response = self.client.post(url, data, format='yaml')
         self.assertEqual(response.status_code, expStatus)
         print(response)
 
     @patch("kfsd.apps.core.auth.api.token.TokenAuth.getTokenUserInfo")
-    @patch("kfsd.apps.core.common.kubefacets_config.KubefacetsConfig.getConfig")
-    def test_common_config_dev(self, genCommonConfigMocked, tokenUserInfoMocked):
+    def test_common_config_dev(self, mocked):
         postData = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/requests/common/config/test_common_config_dev.json')
         obsResponse = self.post(reverse("common-config"), postData, status.HTTP_200_OK)
         expResponse = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/responses/common/config/test_common_config_dev.json')
         self.assertEqual(obsResponse, expResponse)
 
     @patch("kfsd.apps.core.auth.api.token.TokenAuth.getTokenUserInfo")
-    @patch("kfsd.apps.core.common.kubefacets_config.KubefacetsConfig.getConfig")
-    def test_common_config_prod(self, genCommonConfigMocked, tokenUserInfoMocked):
+    def test_common_config_prod(self, mocked):
         postData = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/requests/common/config/test_common_config_prod.json')
         obsResponse = self.post(reverse("common-config"), postData, status.HTTP_200_OK)
         expResponse = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/responses/common/config/test_common_config_prod.json')
         self.assertEqual(obsResponse, expResponse)
```

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/utils/test_utils_arr.py` & `kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_arr.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,45 +6,40 @@
 
 
 class ArrUtilsTestCases(EndpointsTestHandler):
     def setUp(self):
         super().setUp()
 
     @patch("kfsd.apps.core.auth.api.token.TokenAuth.getTokenUserInfo")
-    @patch("kfsd.apps.core.common.kubefacets_config.KubefacetsConfig.getConfig")
-    def test_utils_arr_join(self, genCommonConfigMocked, tokenUserInfoMocked):
+    def test_utils_arr_join(self, mocked):
         postData = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/requests/utils/arr/test_utils_arr_join.json')
         obsResponse = self.post(reverse("utils-arr"), postData, status.HTTP_200_OK)
         expResponse = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/responses/utils/arr/test_utils_arr_join.json')
         self.assertEqual(obsResponse, expResponse)
 
     @patch("kfsd.apps.core.auth.api.token.TokenAuth.getTokenUserInfo")
-    @patch("kfsd.apps.core.common.kubefacets_config.KubefacetsConfig.getConfig")
-    def test_utils_arr_intersection(self, genCommonConfigMocked, tokenUserInfoMocked):
+    def test_utils_arr_intersection(self, mocked):
         postData = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/requests/utils/arr/test_utils_arr_intersection.json')
         obsResponse = self.post(reverse("utils-arr"), postData, status.HTTP_200_OK)
         expResponse = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/responses/utils/arr/test_utils_arr_intersection.json')
         self.assertEqual(obsResponse, expResponse)
 
     @patch("kfsd.apps.core.auth.api.token.TokenAuth.getTokenUserInfo")
-    @patch("kfsd.apps.core.common.kubefacets_config.KubefacetsConfig.getConfig")
-    def test_utils_arr_merge(self, genCommonConfigMocked, tokenUserInfoMocked):
+    def test_utils_arr_merge(self, mocked):
         postData = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/requests/utils/arr/test_utils_arr_merge.json')
         obsResponse = self.post(reverse("utils-arr"), postData, status.HTTP_200_OK)
         expResponse = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/responses/utils/arr/test_utils_arr_merge.json')
         self.assertEqual(obsResponse, expResponse)
 
     @patch("kfsd.apps.core.auth.api.token.TokenAuth.getTokenUserInfo")
-    @patch("kfsd.apps.core.common.kubefacets_config.KubefacetsConfig.getConfig")
-    def test_utils_arr_merge_uniq(self, genCommonConfigMocked, tokenUserInfoMocked):
+    def test_utils_arr_merge_uniq(self, mocked):
         postData = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/requests/utils/arr/test_utils_arr_merge_uniq.json')
         obsResponse = self.post(reverse("utils-arr"), postData, status.HTTP_200_OK)
         expResponse = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/responses/utils/arr/test_utils_arr_merge_uniq.json')
         self.assertEqual(obsResponse, expResponse)
 
     @patch("kfsd.apps.core.auth.api.token.TokenAuth.getTokenUserInfo")
-    @patch("kfsd.apps.core.common.kubefacets_config.KubefacetsConfig.getConfig")
-    def test_utils_arr_match_and_merge(self, genCommonConfigMocked, tokenUserInfoMocked):
+    def test_utils_arr_match_and_merge(self, mocked):
         postData = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/requests/utils/arr/test_utils_arr_match_and_merge.json')
         obsResponse = self.post(reverse("utils-arr"), postData, status.HTTP_200_OK)
         expResponse = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/responses/utils/arr/test_utils_arr_match_and_merge.json')
         self.assertEqual(list(obsResponse["output"]["value"]), expResponse["output"]["value"])
```

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/tests/v1/utils/test_utils_attr.py` & `kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_attr.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,12 @@
 
 
 class AttrUtilsTestCases(EndpointsTestHandler):
     def setUp(self):
         super().setUp()
 
     @patch("kfsd.apps.core.auth.api.token.TokenAuth.getTokenUserInfo")
-    @patch("kfsd.apps.core.common.kubefacets_config.KubefacetsConfig.getConfig")
-    def test_utils_expr(self, genCommonConfigMocked, tokenUserInfoMocked):
-        genCommonConfigMocked.side_effect = [{}]
-        tokenUserInfoMocked.side_effect = [{}]
+    def test_utils_expr(self, mocked):
         postData = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/requests/utils/attr/test_utils_expr.json')
         obsResponse = self.post(reverse("utils-attr"), postData, status.HTTP_200_OK)
         expResponse = self.readJSONData('kfsd/apps/endpoints/tests/v1/data/responses/utils/attr/test_utils_expr.json')
         self.assertEqual(obsResponse, expResponse)
```

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/views/common/list.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/common/list.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/views/common/serializer.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/common/serializer.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/views/docs/common.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/docs/common.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/views/docs/utils.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/docs/utils.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/common.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,152 +1,150 @@
 from drf_spectacular.utils import OpenApiExample
 
 
 class CommonV1Doc:
     @staticmethod
-    def outpost_failed():
-        return []
-
-    @staticmethod
     def config_examples():
         return [
             OpenApiExample(
-                "CONFIG",
-                media_type="application/json",
+                'CONFIG',
+                media_type='application/json',
                 value={
                     "output": {
                         "value": {
                             "templates": [
                                 {
                                     "template": "istio/networking.istio.io/v1alpha3/gateway.json",
                                     "dimensions": [],
-                                    "globalvars": {"__TEMPLATE_ID__": "gateway"},
+                                    "globalvars": {
+                                        "__TEMPLATE_ID__": "gateway"
+                                    }
                                 }
                             ],
                             "overrides": {
                                 "gateway": {
                                     "spec": {
                                         "servers": [
                                             {
                                                 "port": "{{ values.gateway.virtualhost0.listen }}",
-                                                "hosts": "{{ values.gateway.virtualhost0.hosts }}",
+                                                "hosts": "{{ values.gateway.virtualhost0.hosts }}"
                                             }
                                         ]
                                     }
                                 }
                             },
                             "values": {
                                 "gateway": {
                                     "metadata": {
                                         "name": "istio-gateway",
-                                        "namespace": "istio-system",
+                                        "namespace": "istio-system"
                                     },
                                     "virtualhost0": {
                                         "listen": {
                                             "number": 80,
                                             "name": "http-snappyguide",
-                                            "protocol": "HTTP",
+                                            "protocol": "HTTP"
                                         },
                                         "hosts": [
                                             "dev.snappyguide.com",
-                                            "dev.accounts.snappyguide.com",
-                                        ],
-                                    },
+                                            "dev.accounts.snappyguide.com"
+                                        ]
+                                    }
                                 }
-                            },
+                            }
                         }
                     },
-                    "op": "CONFIG",
+                    "op": "CONFIG"
                 },
                 request_only=False,
-                response_only=False,
+                response_only=False
             ),
             OpenApiExample(
-                "CONFIG",
-                media_type="application/json",
+                'CONFIG',
+                media_type='application/json',
                 value={
                     "op": "CONFIG",
                     "input": {
-                        "dimensions": {
-                            "environment": "k8s",
-                            "cluster": "mac",
-                            "type": "dev",
-                        },
+                        "dimensions": {"environment": "k8s", "cluster": "mac", "type": "dev"},
                         "raw_config": [
                             {
-                                "setting": ["master"],
+                                "setting": [
+                                    "master"
+                                ],
                                 "templates": [
                                     {
                                         "template": "istio/networking.istio.io/v1alpha3/gateway.json",
                                         "dimensions": [],
-                                        "globalvars": {"__TEMPLATE_ID__": "gateway"},
+                                        "globalvars": {
+                                            "__TEMPLATE_ID__": "gateway"
+                                        }
                                     }
                                 ],
                                 "overrides": {
                                     "gateway": {
                                         "spec": {
                                             "servers": [
                                                 {
                                                     "port": "{{ values.gateway.virtualhost0.listen }}",
-                                                    "hosts": "{{ values.gateway.virtualhost0.hosts }}",
+                                                    "hosts": "{{ values.gateway.virtualhost0.hosts }}"
                                                 }
                                             ]
                                         }
                                     }
                                 },
                                 "values": {
                                     "gateway": {
                                         "metadata": {
                                             "name": "istio-gateway",
-                                            "namespace": "istio-system",
+                                            "namespace": "istio-system"
                                         },
                                         "virtualhost0": {
                                             "listen": {
                                                 "number": 80,
                                                 "name": "http-snappyguide",
-                                                "protocol": "HTTP",
+                                                "protocol": "HTTP"
                                             }
-                                        },
+                                        }
                                     }
-                                },
+                                }
                             },
                             {
                                 "setting": [
                                     "environment:k8s",
                                     "cluster:mac",
-                                    "type:dev",
+                                    "type:dev"
                                 ],
                                 "values": {
                                     "gateway": {
                                         "virtualhost0": {
                                             "hosts": [
                                                 "dev.snappyguide.com",
-                                                "dev.accounts.snappyguide.com",
+                                                "dev.accounts.snappyguide.com"
                                             ]
                                         }
                                     }
-                                },
+                                }
                             },
                             {
                                 "setting": [
                                     "environment:k8s",
                                     "cluster:inhouse",
-                                    "type:prod",
+                                    "type:prod"
                                 ],
                                 "values": {
                                     "gateway": {
                                         "virtualhost0": {
                                             "hosts": [
                                                 "snappyguide.com",
-                                                "accounts.snappyguide.com",
+                                                "accounts.snappyguide.com"
                                             ]
                                         }
                                     }
-                                },
-                            },
-                        ],
-                    },
+                                }
+                            }
+                        ]
+                    }
                 },
                 request_only=True,
-                response_only=False,
+                response_only=False
             ),
         ]
```

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/views/docs/v1/utils.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/utils.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/views/utils/common.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/utils/common.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/endpoints/views/utils/utils.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/utils/utils.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/frontend/permissions/base.py` & `kfsd-0.0.9/kfsd/apps/core/auth/api/gateway.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from kfsd.apps.core.utils.http.base import HTTP
 from kfsd.apps.core.utils.http.django.request import DjangoRequest
-from kfsd.apps.core.utils.http.django.config import DjangoConfig
-from kfsd.apps.core.common.kubefacets_config import KubefacetsConfig
 
 
-class BasePermission(HTTP):
-    def __init__(self, request):
+class APIGateway(HTTP):
+    def __init__(self, request=None):
         self.__request = DjangoRequest(request)
-        self.__config = DjangoConfig(KubefacetsConfig().getConfig())
         HTTP.__init__(self)
 
-    def getDjangoRequest(self):
-        return self.__request
+    def getApplicationAPIKey(self):
+        return self.__request.findConfigs(["gateway.api_key"])[0]
 
-    def getDjangoConfig(self):
-        return self.__config
+    def getGatewayHost(self):
+        return self.__request.findConfigs(["gateway.host"])[0]
 
-    def getUser(self):
-        return self.getDjangoRequest().getRequest().token_user
+    def getDjangoRequest(self):
+        return self.__request
 
-    def getCurrentRequestUrl(self):
-        return self.getDjangoRequest().getRequest().build_absolute_uri()
+    def constructUrl(self, uri):
+        return self.getGatewayHost() + uri
```

### Comparing `kfsd-0.0.80/kfsd/apps/frontend/templates/v1/base.html` & `kfsd-0.0.9/kfsd/apps/frontend/templates/v1/base.html`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/frontend/templates/v1/docs/browser.html` & `kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/browser.html`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/frontend/templates/v1/docs/skeleton.html` & `kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/skeleton.html`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd/apps/models/tables/base.py` & `kfsd-0.0.9/kfsd/apps/models/base.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.80/kfsd.egg-info/SOURCES.txt` & `kfsd-0.0.9/kfsd.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,45 +19,31 @@
 kfsd/apps/core/auth/key.py
 kfsd/apps/core/auth/token.py
 kfsd/apps/core/auth/api/__init__.py
 kfsd/apps/core/auth/api/gateway.py
 kfsd/apps/core/auth/api/key.py
 kfsd/apps/core/auth/api/token.py
 kfsd/apps/core/common/__init__.py
-kfsd/apps/core/common/cache.py
 kfsd/apps/core/common/configuration.py
-kfsd/apps/core/common/kubefacets_config.py
 kfsd/apps/core/common/logger.py
 kfsd/apps/core/common/singleton.py
 kfsd/apps/core/common/yaml.py
 kfsd/apps/core/exceptions/__init__.py
 kfsd/apps/core/exceptions/api.py
-kfsd/apps/core/exceptions/api_handler.py
 kfsd/apps/core/exceptions/exec.py
 kfsd/apps/core/exceptions/fe.py
-kfsd/apps/core/management/__init__.py
-kfsd/apps/core/management/commands/__init__.py
-kfsd/apps/core/management/commands/basemsmq.py
-kfsd/apps/core/management/commands/setup.py
 kfsd/apps/core/middleware/__init__.py
 kfsd/apps/core/middleware/config.py
 kfsd/apps/core/middleware/key.py
 kfsd/apps/core/middleware/token.py
-kfsd/apps/core/msmq/__init__.py
-kfsd/apps/core/msmq/rabbitmq/__init__.py
-kfsd/apps/core/msmq/rabbitmq/base.py
-kfsd/apps/core/services/__init__.py
-kfsd/apps/core/services/gateway/__init__.py
-kfsd/apps/core/services/gateway/sso.py
 kfsd/apps/core/tests/__init__.py
 kfsd/apps/core/tests/base_api.py
 kfsd/apps/core/tests/v1/__init__.py
 kfsd/apps/core/tests/v1/common/__init__.py
 kfsd/apps/core/tests/v1/common/test_configuration.py
-kfsd/apps/core/tests/v1/common/test_kubefacets_config.py
 kfsd/apps/core/tests/v1/common/test_logger.py
 kfsd/apps/core/tests/v1/common/test_yaml.py
 kfsd/apps/core/tests/v1/data/__init__.py
 kfsd/apps/core/tests/v1/utils/__init__.py
 kfsd/apps/core/tests/v1/utils/test_arr.py
 kfsd/apps/core/tests/v1/utils/test_attr.py
 kfsd/apps/core/tests/v1/utils/test_dict.py
@@ -65,15 +51,14 @@
 kfsd/apps/core/tests/v1/utils/test_system.py
 kfsd/apps/core/utils/__init__.py
 kfsd/apps/core/utils/arr.py
 kfsd/apps/core/utils/attr.py
 kfsd/apps/core/utils/dict.py
 kfsd/apps/core/utils/file.py
 kfsd/apps/core/utils/system.py
-kfsd/apps/core/utils/time.py
 kfsd/apps/core/utils/http/__init__.py
 kfsd/apps/core/utils/http/base.py
 kfsd/apps/core/utils/http/request.py
 kfsd/apps/core/utils/http/response.py
 kfsd/apps/core/utils/http/django/__init__.py
 kfsd/apps/core/utils/http/django/config.py
 kfsd/apps/core/utils/http/django/cookie.py
@@ -88,102 +73,62 @@
 kfsd/apps/endpoints/__init__.py
 kfsd/apps/endpoints/apps.py
 kfsd/apps/endpoints/urls.py
 kfsd/apps/endpoints/handlers/__init__.py
 kfsd/apps/endpoints/handlers/common/__init__.py
 kfsd/apps/endpoints/handlers/common/base.py
 kfsd/apps/endpoints/handlers/common/configuration.py
-kfsd/apps/endpoints/handlers/common/output.py
 kfsd/apps/endpoints/handlers/utils/__init__.py
 kfsd/apps/endpoints/handlers/utils/arr.py
 kfsd/apps/endpoints/handlers/utils/attr.py
 kfsd/apps/endpoints/handlers/utils/system.py
 kfsd/apps/endpoints/renderers/__init__.py
 kfsd/apps/endpoints/renderers/kubefacetsjson.py
 kfsd/apps/endpoints/renderers/kubefacetstext.py
 kfsd/apps/endpoints/renderers/kubefacetsyaml.py
 kfsd/apps/endpoints/serializers/__init__.py
 kfsd/apps/endpoints/serializers/base.py
 kfsd/apps/endpoints/serializers/common/__init__.py
-kfsd/apps/endpoints/serializers/common/cid.py
 kfsd/apps/endpoints/serializers/common/configuration.py
-kfsd/apps/endpoints/serializers/common/id.py
 kfsd/apps/endpoints/serializers/common/model.py
-kfsd/apps/endpoints/serializers/common/oid.py
-kfsd/apps/endpoints/serializers/common/outpost.py
-kfsd/apps/endpoints/serializers/common/pid.py
-kfsd/apps/endpoints/serializers/common/tid.py
-kfsd/apps/endpoints/serializers/common/uid.py
 kfsd/apps/endpoints/serializers/utils/__init__.py
 kfsd/apps/endpoints/serializers/utils/arr.py
 kfsd/apps/endpoints/serializers/utils/attr.py
 kfsd/apps/endpoints/serializers/utils/system.py
 kfsd/apps/endpoints/tests/__init__.py
 kfsd/apps/endpoints/tests/endpoints_test_handler.py
 kfsd/apps/endpoints/tests/v1/__init__.py
 kfsd/apps/endpoints/tests/v1/common/__init__.py
-kfsd/apps/endpoints/tests/v1/common/test_cid.py
 kfsd/apps/endpoints/tests/v1/common/test_common_configuration.py
-kfsd/apps/endpoints/tests/v1/common/test_oid.py
-kfsd/apps/endpoints/tests/v1/common/test_pid.py
-kfsd/apps/endpoints/tests/v1/common/test_tid.py
-kfsd/apps/endpoints/tests/v1/common/test_uid.py
-kfsd/apps/endpoints/tests/v1/common/data/__init__.py
-kfsd/apps/endpoints/tests/v1/common/data/responses/__init__.py
 kfsd/apps/endpoints/tests/v1/data/__init__.py
 kfsd/apps/endpoints/tests/v1/utils/__init__.py
 kfsd/apps/endpoints/tests/v1/utils/test_utils_arr.py
 kfsd/apps/endpoints/tests/v1/utils/test_utils_attr.py
 kfsd/apps/endpoints/tests/v1/utils/test_utils_system.py
 kfsd/apps/endpoints/views/__init__.py
 kfsd/apps/endpoints/views/common/__init__.py
-kfsd/apps/endpoints/views/common/cid.py
 kfsd/apps/endpoints/views/common/custom_model.py
 kfsd/apps/endpoints/views/common/get.py
 kfsd/apps/endpoints/views/common/list.py
 kfsd/apps/endpoints/views/common/model.py
-kfsd/apps/endpoints/views/common/oid.py
-kfsd/apps/endpoints/views/common/outpost.py
-kfsd/apps/endpoints/views/common/pid.py
 kfsd/apps/endpoints/views/common/serializer.py
-kfsd/apps/endpoints/views/common/tid.py
-kfsd/apps/endpoints/views/common/uid.py
 kfsd/apps/endpoints/views/docs/__init__.py
-kfsd/apps/endpoints/views/docs/cid.py
 kfsd/apps/endpoints/views/docs/common.py
-kfsd/apps/endpoints/views/docs/oid.py
-kfsd/apps/endpoints/views/docs/outpost.py
-kfsd/apps/endpoints/views/docs/pid.py
-kfsd/apps/endpoints/views/docs/tid.py
-kfsd/apps/endpoints/views/docs/uid.py
 kfsd/apps/endpoints/views/docs/utils.py
 kfsd/apps/endpoints/views/docs/v1/__init__.py
-kfsd/apps/endpoints/views/docs/v1/cid.py
 kfsd/apps/endpoints/views/docs/v1/common.py
-kfsd/apps/endpoints/views/docs/v1/oid.py
-kfsd/apps/endpoints/views/docs/v1/outpost.py
-kfsd/apps/endpoints/views/docs/v1/pid.py
-kfsd/apps/endpoints/views/docs/v1/tid.py
-kfsd/apps/endpoints/views/docs/v1/uid.py
 kfsd/apps/endpoints/views/docs/v1/utils.py
 kfsd/apps/endpoints/views/pagination/__init__.py
 kfsd/apps/endpoints/views/pagination/model.py
 kfsd/apps/endpoints/views/utils/__init__.py
 kfsd/apps/endpoints/views/utils/common.py
 kfsd/apps/endpoints/views/utils/utils.py
 kfsd/apps/frontend/__init__.py
 kfsd/apps/frontend/apps.py
 kfsd/apps/frontend/urls.py
-kfsd/apps/frontend/permissions/__init__.py
-kfsd/apps/frontend/permissions/active.py
-kfsd/apps/frontend/permissions/base.py
-kfsd/apps/frontend/permissions/email.py
-kfsd/apps/frontend/permissions/signin.py
-kfsd/apps/frontend/permissions/staff.py
-kfsd/apps/frontend/permissions/superuser.py
 kfsd/apps/frontend/templates/__init__.py
 kfsd/apps/frontend/templates/v1/__init__.py
 kfsd/apps/frontend/templates/v1/base.html
 kfsd/apps/frontend/templates/v1/docs/__init__.py
 kfsd/apps/frontend/templates/v1/docs/browser.html
 kfsd/apps/frontend/templates/v1/docs/skeleton.html
 kfsd/apps/frontend/templates/v1/errors/403.html
@@ -195,29 +140,11 @@
 kfsd/apps/frontend/views/__init__.py
 kfsd/apps/frontend/views/docs/__init__.py
 kfsd/apps/frontend/views/docs/api.py
 kfsd/apps/frontend/views/errors/__init__.py
 kfsd/apps/frontend/views/errors/custom403.py
 kfsd/apps/frontend/views/errors/custom404.py
 kfsd/apps/frontend/views/errors/custom500.py
-kfsd/apps/frontend/views/permissions/__init__.py
-kfsd/apps/frontend/views/permissions/base.py
 kfsd/apps/models/__init__.py
 kfsd/apps/models/apps.py
-kfsd/apps/models/constants.py
-kfsd/apps/models/models.py
-kfsd/apps/models/fixtures/__init__.py
-kfsd/apps/models/fixtures/v1/__init__.py
-kfsd/apps/models/fixtures/v1/tests/__init__.py
-kfsd/apps/models/fixtures/v1/tests/common/__init__.py
-kfsd/apps/models/migrations/0001_initial.py
-kfsd/apps/models/migrations/__init__.py
-kfsd/apps/models/tables/__init__.py
-kfsd/apps/models/tables/base.py
-kfsd/apps/models/tables/cid.py
-kfsd/apps/models/tables/feature.py
-kfsd/apps/models/tables/id.py
-kfsd/apps/models/tables/oid.py
-kfsd/apps/models/tables/outpost.py
-kfsd/apps/models/tables/pid.py
-kfsd/apps/models/tables/tid.py
-kfsd/apps/models/tables/uid.py
+kfsd/apps/models/base.py
+kfsd/apps/models/constants.py
```

