# Comparing `tmp/esmerald-2.0.2.tar.gz` & `tmp/esmerald-2.0.3.tar.gz`

## Comparing `esmerald-2.0.2.tar` & `esmerald-2.0.3.tar`

### file list

```diff
@@ -1,188 +1,194 @@
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/__init__.py
--rw-r--r--   0        0        0    39505 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/applications.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/concurrency.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/enums.py
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/exceptions.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/injector.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/logging.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/param_functions.py
--rw-r--r--   0        0        0    22750 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/params.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/py.typed
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/requests.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/staticfiles.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/testclient.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/types.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/typing.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/websockets.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/enums.py
--rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/app_template/v1/views.py-tpl
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/cors.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/csrf.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/jwt.py
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/openapi.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/session.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/static_files.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/urls/__init__.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/core/urls/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/json.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/multidict.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/basic.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/cors.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/https.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/_internal.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/constants.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/docs.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/models.py
--rw-r--r--   0        0        0    17141 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/openapi.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/params.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/utils.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/openapi/validation.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/permissions/base.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/utils/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/protocols/utils/protocols.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/base.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/json.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/__init__.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/_internal.py
--rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/base.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/events.py
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/gateways.py
--rw-r--r--   0        0        0    22735 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    42063 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/router.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/routing/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/helpers.py
--rw-r--r--   0        0        0    14627 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/model.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/signature.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/types.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/transformers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/constants.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/helpers.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/models.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/pydantic/__init__.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esmerald-2.0.2/esmerald/utils/pydantic/schema.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-2.0.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-2.0.2/LICENSE
--rw-r--r--   0        0        0    15936 2020-02-02 00:00:00.000000 esmerald-2.0.2/README.md
--rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 esmerald-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    21120 2020-02-02 00:00:00.000000 esmerald-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/__init__.py
+-rw-r--r--   0        0        0    39505 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/applications.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/concurrency.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/enums.py
+-rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/exceptions.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/injector.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/logging.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/param_functions.py
+-rw-r--r--   0        0        0    22750 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/params.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/py.typed
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/requests.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/testclient.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/types.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/typing.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/websockets.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    14905 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/app_template/v1/views.py-tpl
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/conf/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/config/cors.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/config/csrf.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/config/jwt.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/config/openapi.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/config/session.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/config/static_files.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8616 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/shell/__init__.py
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/shell/enums.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/directives/operations/shell/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/multidict.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/basic.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/_internal.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/constants.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/docs.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/models.py
+-rw-r--r--   0        0        0    17141 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/openapi.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/params.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/openapi/validation.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/protocols/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/protocols/utils/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/protocols/utils/protocols.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/responses/base.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/routing/_internal.py
+-rw-r--r--   0        0        0    22141 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/routing/events.py
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0    22735 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    42063 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/routing/router.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/routing/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/transformers/datastructures.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/transformers/helpers.py
+-rw-r--r--   0        0        0    14627 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/transformers/model.py
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/transformers/types.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/constants.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/models.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 esmerald-2.0.3/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 esmerald-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-2.0.3/LICENSE
+-rw-r--r--   0        0        0    16233 2020-02-02 00:00:00.000000 esmerald-2.0.3/README.md
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 esmerald-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    21620 2020-02-02 00:00:00.000000 esmerald-2.0.3/PKG-INFO
```

### Comparing `esmerald-2.0.2/esmerald/__init__.py` & `esmerald-2.0.3/esmerald/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 
 from starlette import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.injector import Inject
```

### Comparing `esmerald-2.0.2/esmerald/applications.py` & `esmerald-2.0.3/esmerald/applications.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/backgound.py` & `esmerald-2.0.3/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/enums.py` & `esmerald-2.0.3/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/exception_handlers.py` & `esmerald-2.0.3/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/exceptions.py` & `esmerald-2.0.3/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/injector.py` & `esmerald-2.0.3/esmerald/injector.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/logging.py` & `esmerald-2.0.3/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/params.py` & `esmerald-2.0.3/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/parsers.py` & `esmerald-2.0.3/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/requests.py` & `esmerald-2.0.3/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/testclient.py` & `esmerald-2.0.3/esmerald/testclient.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/types.py` & `esmerald-2.0.3/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/websockets.py` & `esmerald-2.0.3/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/conf/__init__.py` & `esmerald-2.0.3/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/conf/global_settings.py` & `esmerald-2.0.3/esmerald/conf/global_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,18 @@
     )
     swagger_css_url: str = "https://cdn.jsdelivr.net/npm/swagger-ui-dist@5.1.3/swagger-ui.min.css"
     swagger_favicon_url: str = "https://esmerald.dev/statics/images/favicon.ico"
 
     # Model configuration
     model_config = SettingsConfigDict(extra="allow", ignored_types=(cached_property,))
 
+    # Shell configuration
+    ipython_args: List[str] = ["--no-banner"]
+    ptpython_config_file: str = "~/.config/ptpython/config.py"
+
     @property
     def reload(self) -> bool:
         """
         Returns reloading for dev and test environments.
         """
         if self.environment in [EnvironmentType.DEVELOPMENT, EnvironmentType.TESTING]:
             return True
```

### Comparing `esmerald-2.0.2/esmerald/conf/project_template/.gitignore.e-tpl` & `esmerald-2.0.3/esmerald/conf/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/conf/project_template/Makefile.e-tpl` & `esmerald-2.0.3/esmerald/conf/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/conf/project_template/project_name/main.py-tpl` & `esmerald-2.0.3/esmerald/conf/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/conf/project_template/project_name/serve.py-tpl` & `esmerald-2.0.3/esmerald/conf/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/conf/project_template/project_name/urls.py-tpl` & `esmerald-2.0.3/esmerald/conf/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/conf/project_template/project_name/configs/settings.py-tpl` & `esmerald-2.0.3/esmerald/conf/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/config/jwt.py` & `esmerald-2.0.3/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/config/openapi.py` & `esmerald-2.0.3/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/config/session.py` & `esmerald-2.0.3/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/config/static_files.py` & `esmerald-2.0.3/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/contrib/encoding.py` & `esmerald-2.0.3/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/contrib/auth/hashers.py` & `esmerald-2.0.3/esmerald/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/contrib/auth/common/middleware.py` & `esmerald-2.0.3/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-2.0.3/esmerald/contrib/auth/saffier/base_user.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-2.0.3/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/base.py` & `esmerald-2.0.3/esmerald/core/directives/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/cli.py` & `esmerald-2.0.3/esmerald/core/directives/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from esmerald.core.directives.env import DirectiveEnv
 from esmerald.core.directives.operations import (
     create_app,
     create_project,
     list,
     run,
     runserver,
+    shell,
     show_urls,
 )
 from esmerald.core.directives.operations._constants import ESMERALD_SETTINGS_MODULE
 from esmerald.core.terminal.print import Print
 
 T = TypeVar("T")
 
@@ -124,7 +125,8 @@
 
 esmerald_cli.add_command(list)
 esmerald_cli.add_command(show_urls)
 esmerald_cli.add_command(run)
 esmerald_cli.add_command(create_project)
 esmerald_cli.add_command(create_app)
 esmerald_cli.add_command(runserver)
+esmerald_cli.add_command(shell)
```

### Comparing `esmerald-2.0.2/esmerald/core/directives/env.py` & `esmerald-2.0.3/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/templates.py` & `esmerald-2.0.3/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/utils.py` & `esmerald-2.0.3/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/operations/createapp.py` & `esmerald-2.0.3/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/operations/createproject.py` & `esmerald-2.0.3/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/operations/list.py` & `esmerald-2.0.3/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/operations/run.py` & `esmerald-2.0.3/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/operations/runserver.py` & `esmerald-2.0.3/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/directives/operations/show_urls.py` & `esmerald-2.0.3/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/terminal/base.py` & `esmerald-2.0.3/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/terminal/print.py` & `esmerald-2.0.3/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/terminal/terminal.py` & `esmerald-2.0.3/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/core/urls/base.py` & `esmerald-2.0.3/esmerald/core/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/datastructures/__init__.py` & `esmerald-2.0.3/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/datastructures/base.py` & `esmerald-2.0.3/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/datastructures/encoders.py` & `esmerald-2.0.3/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/datastructures/file.py` & `esmerald-2.0.3/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/datastructures/json.py` & `esmerald-2.0.3/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/datastructures/redirect.py` & `esmerald-2.0.3/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/datastructures/stream.py` & `esmerald-2.0.3/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/datastructures/template.py` & `esmerald-2.0.3/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/interceptors/interceptor.py` & `esmerald-2.0.3/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/middleware/__init__.py` & `esmerald-2.0.3/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/middleware/_exception_handlers.py` & `esmerald-2.0.3/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/middleware/asyncexitstack.py` & `esmerald-2.0.3/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/middleware/authentication.py` & `esmerald-2.0.3/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/middleware/basic.py` & `esmerald-2.0.3/esmerald/middleware/basic.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/middleware/csrf.py` & `esmerald-2.0.3/esmerald/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/middleware/errors.py` & `esmerald-2.0.3/esmerald/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/middleware/exceptions.py` & `esmerald-2.0.3/esmerald/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/middleware/settings_middleware.py` & `esmerald-2.0.3/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/openapi/_internal.py` & `esmerald-2.0.3/esmerald/openapi/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/openapi/datastructures.py` & `esmerald-2.0.3/esmerald/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/openapi/docs.py` & `esmerald-2.0.3/esmerald/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/openapi/models.py` & `esmerald-2.0.3/esmerald/openapi/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/openapi/openapi.py` & `esmerald-2.0.3/esmerald/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/openapi/responses.py` & `esmerald-2.0.3/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/openapi/utils.py` & `esmerald-2.0.3/esmerald/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/openapi/validation.py` & `esmerald-2.0.3/esmerald/openapi/validation.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/permissions/base.py` & `esmerald-2.0.3/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/permissions/utils.py` & `esmerald-2.0.3/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/pluggables/base.py` & `esmerald-2.0.3/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/protocols/asyncdao.py` & `esmerald-2.0.3/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/protocols/dao.py` & `esmerald-2.0.3/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/protocols/interceptor.py` & `esmerald-2.0.3/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/protocols/template.py` & `esmerald-2.0.3/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/responses/base.py` & `esmerald-2.0.3/esmerald/responses/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/responses/encoders.py` & `esmerald-2.0.3/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/responses/json.py` & `esmerald-2.0.3/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/responses/template.py` & `esmerald-2.0.3/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/routing/_internal.py` & `esmerald-2.0.3/esmerald/routing/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/routing/base.py` & `esmerald-2.0.3/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/routing/events.py` & `esmerald-2.0.3/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/routing/gateways.py` & `esmerald-2.0.3/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/routing/handlers.py` & `esmerald-2.0.3/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/routing/router.py` & `esmerald-2.0.3/esmerald/routing/router.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/routing/views.py` & `esmerald-2.0.3/esmerald/routing/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/security/jwt/token.py` & `esmerald-2.0.3/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/template/jinja.py` & `esmerald-2.0.3/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/template/mako.py` & `esmerald-2.0.3/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/transformers/datastructures.py` & `esmerald-2.0.3/esmerald/transformers/datastructures.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/transformers/helpers.py` & `esmerald-2.0.3/esmerald/transformers/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/transformers/model.py` & `esmerald-2.0.3/esmerald/transformers/model.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/transformers/signature.py` & `esmerald-2.0.3/esmerald/transformers/signature.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/transformers/types.py` & `esmerald-2.0.3/esmerald/transformers/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/transformers/utils.py` & `esmerald-2.0.3/esmerald/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/utils/constants.py` & `esmerald-2.0.3/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/utils/crypto.py` & `esmerald-2.0.3/esmerald/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/utils/dependency.py` & `esmerald-2.0.3/esmerald/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/utils/functional.py` & `esmerald-2.0.3/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/utils/helpers.py` & `esmerald-2.0.3/esmerald/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/utils/models.py` & `esmerald-2.0.3/esmerald/utils/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/utils/module_loading.py` & `esmerald-2.0.3/esmerald/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/utils/sync.py` & `esmerald-2.0.3/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/esmerald/utils/pydantic/schema.py` & `esmerald-2.0.3/esmerald/utils/pydantic/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/LICENSE` & `esmerald-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-2.0.2/README.md` & `esmerald-2.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,70 +60,79 @@
 
 * <a href="https://www.starlette.io/" class="external-link" target="_blank">Starlette</a>
 * <a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a>
 
 ## Installation
 
 ```shell
-pip install esmerald
+$ pip install esmerald
 ```
 
 An ASGI server is also needed to run in production, we recommend [Uvicorn](https://www.uvicorn.org) but it is entirely
 up to you.
 
 ```shell
-pip install uvicorn
+$ pip install uvicorn
 
 ```
 
 If you want install esmerald with specifics:
 
 **Support for template system such as jinja2 and mako**:
 
 ```shell
-pip install esmerald[templates]
+$ pip install esmerald[templates]
 ```
 
 **Support for the internal scheduler**:
 
 ```shell
-pip install esmerald[schedulers]
+$ pip install esmerald[schedulers]
 ```
 
 **Support for the jwt used internally by Esmerald**:
 
 ```shell
-pip install esmerald[jwt]
+$ pip install esmerald[jwt]
 ```
 
 **Support for ORJSON and UJSON**:
 
 ```shell
-pip install esmerald[encoders]
+$ pip install esmerald[encoders]
 ```
 
 **If you want to use the esmerald testing client**:
 
 ```shell
-pip install esmerald[test]
+$ pip install esmerald[test]
+```
+
+**If you want to use the esmerald shell**:
+
+More [details](https://esmerald.dev/directives/shell) about this topic [in the docs](https://esmerald.dev/directives/shell)
+
+```shell
+$ pip install esmerald[ipython] # default shell
+$ pip install esmerald[ptpython] # ptpython shell
 ```
 
 ### Start a project using directives
 
 If you wish to start an Esmerald project with a default suggested structure.
 
 ```
 esmerald createproject <YOUR-PROJECT-NAME>
 ```
 
 This will generate a scaffold for your project with some pre-defined files in a simple fashion.
 This will also generate a file for the tests using the EsmeraldTestClient, so make sure you run:
 
 ```shell
-pip install esmerald[test]
+$ pip install esmerald[test]
 ```
 
 Or you can jump this step if you don't want to use the EsmeraldTestClient.
 
 You can find [more information](https://esmerald.dymmond.com/management/directives) about this directive and how to
 use it.
```

#### html2text {}

```diff
@@ -20,68 +20,71 @@
 but with business in mind as well. Starlite, for example, gave the inspiration
 for the transformers and for the Signature models, something very useful that
 helped Esmerald integerating with pydantic. FastAPI gave the inspiration for
 API designing, Django for the permissions, Flask for the simplicity, NestJS for
 the controllers and the list goes on. For a job to be done properly, usually it
 is never done alone and there is always a driver and inspiration to it. ##
 Requirements * python 3.8+ Esmerald wouldn't be possible without two colossals:
-* Starlette * Pydantic ## Installation ```shell pip install esmerald ``` An
+* Starlette * Pydantic ## Installation ```shell $ pip install esmerald ``` An
 ASGI server is also needed to run in production, we recommend [Uvicorn](https:/
-/www.uvicorn.org) but it is entirely up to you. ```shell pip install uvicorn
+/www.uvicorn.org) but it is entirely up to you. ```shell $ pip install uvicorn
 ``` If you want install esmerald with specifics: **Support for template system
-such as jinja2 and mako**: ```shell pip install esmerald[templates] ```
-**Support for the internal scheduler**: ```shell pip install esmerald
+such as jinja2 and mako**: ```shell $ pip install esmerald[templates] ```
+**Support for the internal scheduler**: ```shell $ pip install esmerald
 [schedulers] ``` **Support for the jwt used internally by Esmerald**: ```shell
-pip install esmerald[jwt] ``` **Support for ORJSON and UJSON**: ```shell pip
-install esmerald[encoders] ``` **If you want to use the esmerald testing
-client**: ```shell pip install esmerald[test] ``` ### Start a project using
-directives If you wish to start an Esmerald project with a default suggested
-structure. ``` esmerald createproject  ``` This will generate a scaffold for
-your project with some pre-defined files in a simple fashion. This will also
-generate a file for the tests using the EsmeraldTestClient, so make sure you
-run: ```shell pip install esmerald[test] ``` Or you can jump this step if you
-don't want to use the EsmeraldTestClient. You can find [more information]
-(https://esmerald.dymmond.com/management/directives) about this directive and
-how to use it. ## Key Features * **Fluid and Fast**: Thanks to Starlette and
-Pydantic. * **Fast to develop**: Thanks to the simplicity of design, the
-development times can be reduced exponentially. * **Intuitive**: If you are
-used to the other frameworks, Esmerald is a no brainer to develop. * **Easy**:
-Developed with design in mind and easy learning. * **Short**: With the OOP
-available natively there is no need for code duplication. SOLID. * **Ready**:
-Get your application up and running with production-ready code. * **OOP and
-Functional**: Design APIs in any desired way. OOP or Functional is available. *
-**Async and Sync**: Do you prefer sync or async? You can have both. *
-**Middleware**: Apply middlewares on the application level or API level. *
-**Exception Handlers**: Apply exception handlers on any desired level. *
-**Permissions**: Apply specific rules and permissions on each API. *
-**Interceptors**: Intercept requests and add logic before reaching the
-endpoint. * **Pluggables**: Create plugins for Esmerald and hook them into any
-application and/or distribute them. * **DAO and AsyncDAO**: Avoid database
-calls directly from the APIs. Use business objects instead. * **Saffier ORM**:
-Native support for [Saffier ORM](./databases/saffier/motivation.md). *
-**APIView**: Class Based endpoints for your beloved OOP design. * **JSON
-serialization/deserialization**: Both UJSON and ORJON support. * **Lifespan**:
-Support for the newly lifespan and on_start/on_shutdown events. *
-**Scheduler**: Yes, that's right, it comes with a scheduler for those automated
-tasks. * **Dependency Injection**: Like any other great framework out there. *
-**Simplicity from settings**: Yes, we have a way to make the code even cleaner
-by introducing settings based systems. * **Database**: Out of the box support
-for async databases. ## Relation to Starlette and other frameworks Esmerald
-uses Starlette under the hood. The reason behind this decison comes with the
-fact that performance is there and no issues with routing. Once the application
-is up, all the routes are mounted and therefore the url paths are defined.
-Esmerald encourages standard practices and design in mind which means that any
-application, big or small, custom or enterprise, fits within Esmerald ecosystem
-without scalability issues. ## Settings Like every other framework, when
-starting an application, a lot of [settings](./application/settings.md) can/
-need to be passed to the main object and this can be very dauting and hugly to
-maintain and see. Esmerald comes with the [settings](./application/settings.md)
-in mind. A set of defaults that can be overridden by your very own settings
-module but not limited to it as you can still use the classic approach of
-passing everything into a Esmerald instance directly when instantiating.
+$ pip install esmerald[jwt] ``` **Support for ORJSON and UJSON**: ```shell $
+pip install esmerald[encoders] ``` **If you want to use the esmerald testing
+client**: ```shell $ pip install esmerald[test] ``` **If you want to use the
+esmerald shell**: More [details](https://esmerald.dev/directives/shell) about
+this topic [in the docs](https://esmerald.dev/directives/shell) ```shell $ pip
+install esmerald[ipython] # default shell $ pip install esmerald[ptpython] #
+ptpython shell ``` ### Start a project using directives If you wish to start an
+Esmerald project with a default suggested structure. ``` esmerald createproject
+``` This will generate a scaffold for your project with some pre-defined files
+in a simple fashion. This will also generate a file for the tests using the
+EsmeraldTestClient, so make sure you run: ```shell $ pip install esmerald[test]
+``` Or you can jump this step if you don't want to use the EsmeraldTestClient.
+You can find [more information](https://esmerald.dymmond.com/management/
+directives) about this directive and how to use it. ## Key Features * **Fluid
+and Fast**: Thanks to Starlette and Pydantic. * **Fast to develop**: Thanks to
+the simplicity of design, the development times can be reduced exponentially. *
+**Intuitive**: If you are used to the other frameworks, Esmerald is a no
+brainer to develop. * **Easy**: Developed with design in mind and easy
+learning. * **Short**: With the OOP available natively there is no need for
+code duplication. SOLID. * **Ready**: Get your application up and running with
+production-ready code. * **OOP and Functional**: Design APIs in any desired
+way. OOP or Functional is available. * **Async and Sync**: Do you prefer sync
+or async? You can have both. * **Middleware**: Apply middlewares on the
+application level or API level. * **Exception Handlers**: Apply exception
+handlers on any desired level. * **Permissions**: Apply specific rules and
+permissions on each API. * **Interceptors**: Intercept requests and add logic
+before reaching the endpoint. * **Pluggables**: Create plugins for Esmerald and
+hook them into any application and/or distribute them. * **DAO and AsyncDAO**:
+Avoid database calls directly from the APIs. Use business objects instead. *
+**Saffier ORM**: Native support for [Saffier ORM](./databases/saffier/
+motivation.md). * **APIView**: Class Based endpoints for your beloved OOP
+design. * **JSON serialization/deserialization**: Both UJSON and ORJON support.
+* **Lifespan**: Support for the newly lifespan and on_start/on_shutdown events.
+* **Scheduler**: Yes, that's right, it comes with a scheduler for those
+automated tasks. * **Dependency Injection**: Like any other great framework out
+there. * **Simplicity from settings**: Yes, we have a way to make the code even
+cleaner by introducing settings based systems. * **Database**: Out of the box
+support for async databases. ## Relation to Starlette and other frameworks
+Esmerald uses Starlette under the hood. The reason behind this decison comes
+with the fact that performance is there and no issues with routing. Once the
+application is up, all the routes are mounted and therefore the url paths are
+defined. Esmerald encourages standard practices and design in mind which means
+that any application, big or small, custom or enterprise, fits within Esmerald
+ecosystem without scalability issues. ## Settings Like every other framework,
+when starting an application, a lot of [settings](./application/settings.md)
+can/need to be passed to the main object and this can be very dauting and hugly
+to maintain and see. Esmerald comes with the [settings](./application/
+settings.md) in mind. A set of defaults that can be overridden by your very own
+settings module but not limited to it as you can still use the classic approach
+of passing everything into a Esmerald instance directly when instantiating.
 **Example of classic approach**: ```python from example import ExampleObject #
 ExampleObject is an instance of another application # and it serves only for
 example app = ExampleObject(setting_one=..., setting_two=...,
 setting_three=...) ``` Inspired by the great [Django](https://
 www.djangoproject.com/) and using pydantic, Esmerald has a default object ready
 to be used out-of-the-box. **Esmerald**: ```python from esmerald import
 Esmerald app = Esmerald() ``` And that's it! All the default settings are
```

### Comparing `esmerald-2.0.2/pyproject.toml` & `esmerald-2.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 
     # types
     "types-ujson==5.8.0.0",
     "types-orjson==3.6.2",
 ]
 
 dev = [
+    "ipdb",
     "autoflake>=1.4.0",
     "flake8>=3.8.3,<6.0.0",
     "uvicorn[standard]>=0.19.0",
     "pre-commit>=3.0.4,<4.0.0",
     "watchfiles>=0.16.1,<0.20.0",
 ]
 
@@ -138,20 +139,19 @@
     "mdx-include>=1.4.2,<2.0.0",
     "mkdocs-markdownextradata-plugin>=0.2.5,<0.3.0",
     "mkdocstrings>=0.20.0,<0.30.0",
     "pyyaml>=6.0,<7.0.0",
 ]
 
 templates = ["mako==1.2.4"]
-
 jwt = ["passlib==1.7.4", "python-jose>=3.3.0,<4"]
-
 encoders = ["orjson>=3.8.5,<4.0.0", "ujson>=5.7.0,<6"]
-
 schedulers = ["asyncz>=0.4.0"]
+ptpython = ["ptpython>=3.0.23,<4.0.0"]
+ipython = ["ipython>=8.10.0,<9.0.0"]
 
 [tool.hatch.version]
 path = "esmerald/__init__.py"
 
 [project.scripts]
 esmerald = "esmerald.core.directives.cli:esmerald_cli"
 
@@ -173,15 +173,14 @@
 exclude = "esmerald/conf,esmerald/utils"
 warn_unused_ignores = true
 warn_redundant_casts = true
 no_implicit_optional = false
 strict_equality = false
 strict_optional = false
 
-
 [tool.ruff]
 select = [
     "E", # pycodestyle errors
     "W", # pycodestyle warnings
     "F", # pyflakes
     "C", # flake8-comprehensions
     "B", # flake8-bugbear
@@ -211,14 +210,15 @@
     "slugify.*",
     "pytz",
     "jose.*",
     "mako.*",
     "passlib.*",
     "esmerald.contrib.auth.saffier.*",
     "openapi_schemas_pydantic.*",
+    "nest_asyncio.*",
 ]
 ignore_missing_imports = true
 ignore_errors = true
 
 [tool.pytest.ini_options]
 addopts = ["--strict-config", "--strict-markers"]
 xfail_strict = true
```

### Comparing `esmerald-2.0.2/PKG-INFO` & `esmerald-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esmerald
-Version: 2.0.2
+Version: 2.0.3
 Summary: Highly scalable, performant, easy to learn, easy to code and for every application.
 Project-URL: Homepage, https://github.com/dymmond/esmerald
 Project-URL: Documentation, https://esmerald.dymmond.com/
 Project-URL: Changelog, https://esmerald.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/esmerald
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
@@ -53,31 +53,36 @@
 Requires-Dist: pydantic<3.0.0,>=2.0.1
 Requires-Dist: python-multipart>=0.0.5
 Requires-Dist: rich<14.0.0,>=13.3.1
 Requires-Dist: starlette<1.0,>=0.30.0
 Provides-Extra: dev
 Requires-Dist: autoflake>=1.4.0; extra == 'dev'
 Requires-Dist: flake8<6.0.0,>=3.8.3; extra == 'dev'
+Requires-Dist: ipdb; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.0.4; extra == 'dev'
 Requires-Dist: uvicorn[standard]>=0.19.0; extra == 'dev'
 Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.2; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.2.5; extra == 'doc'
 Requires-Dist: mkdocs-material<10.0.0,>=9.0.13; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc'
 Requires-Dist: mkdocstrings<0.30.0,>=0.20.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc'
 Provides-Extra: encoders
 Requires-Dist: orjson<4.0.0,>=3.8.5; extra == 'encoders'
 Requires-Dist: ujson<6,>=5.7.0; extra == 'encoders'
+Provides-Extra: ipython
+Requires-Dist: ipython<9.0.0,>=8.10.0; extra == 'ipython'
 Provides-Extra: jwt
 Requires-Dist: passlib==1.7.4; extra == 'jwt'
 Requires-Dist: python-jose<4,>=3.3.0; extra == 'jwt'
+Provides-Extra: ptpython
+Requires-Dist: ptpython<4.0.0,>=3.0.23; extra == 'ptpython'
 Provides-Extra: schedulers
 Requires-Dist: asyncz>=0.4.0; extra == 'schedulers'
 Provides-Extra: templates
 Requires-Dist: mako==1.2.4; extra == 'templates'
 Provides-Extra: test
 Requires-Dist: a2wsgi<2,>=1.7.0; extra == 'test'
 Requires-Dist: aiofiles<24,>=0.8.0; extra == 'test'
@@ -169,70 +174,79 @@
 
 * <a href="https://www.starlette.io/" class="external-link" target="_blank">Starlette</a>
 * <a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a>
 
 ## Installation
 
 ```shell
-pip install esmerald
+$ pip install esmerald
 ```
 
 An ASGI server is also needed to run in production, we recommend [Uvicorn](https://www.uvicorn.org) but it is entirely
 up to you.
 
 ```shell
-pip install uvicorn
+$ pip install uvicorn
 
 ```
 
 If you want install esmerald with specifics:
 
 **Support for template system such as jinja2 and mako**:
 
 ```shell
-pip install esmerald[templates]
+$ pip install esmerald[templates]
 ```
 
 **Support for the internal scheduler**:
 
 ```shell
-pip install esmerald[schedulers]
+$ pip install esmerald[schedulers]
 ```
 
 **Support for the jwt used internally by Esmerald**:
 
 ```shell
-pip install esmerald[jwt]
+$ pip install esmerald[jwt]
 ```
 
 **Support for ORJSON and UJSON**:
 
 ```shell
-pip install esmerald[encoders]
+$ pip install esmerald[encoders]
 ```
 
 **If you want to use the esmerald testing client**:
 
 ```shell
-pip install esmerald[test]
+$ pip install esmerald[test]
+```
+
+**If you want to use the esmerald shell**:
+
+More [details](https://esmerald.dev/directives/shell) about this topic [in the docs](https://esmerald.dev/directives/shell)
+
+```shell
+$ pip install esmerald[ipython] # default shell
+$ pip install esmerald[ptpython] # ptpython shell
 ```
 
 ### Start a project using directives
 
 If you wish to start an Esmerald project with a default suggested structure.
 
 ```
 esmerald createproject <YOUR-PROJECT-NAME>
 ```
 
 This will generate a scaffold for your project with some pre-defined files in a simple fashion.
 This will also generate a file for the tests using the EsmeraldTestClient, so make sure you run:
 
 ```shell
-pip install esmerald[test]
+$ pip install esmerald[test]
 ```
 
 Or you can jump this step if you don't want to use the EsmeraldTestClient.
 
 You can find [more information](https://esmerald.dymmond.com/management/directives) about this directive and how to
 use it.
```

