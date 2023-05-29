# Comparing `tmp/ellar-0.3.8.tar.gz` & `tmp/ellar-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar-0.3.8.tar", last modified: Thu May 11 21:02:51 2023, max compression
+gzip compressed data, was "ellar-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ellar-0.3.8.tar` & `ellar-0.4.0.tar`

### file list

```diff
@@ -1,520 +1,535 @@
--rw-r--r--   0        0        0      270 2023-05-11 21:02:05.040800 ellar-0.3.8/.coveragerc
--rw-r--r--   0        0        0       65 2023-05-11 21:02:05.040800 ellar-0.3.8/.dockerignore
--rw-r--r--   0        0        0      146 2023-05-11 21:02:05.040800 ellar-0.3.8/.flake8
--rw-r--r--   0        0        0      205 2023-05-11 21:02:05.040800 ellar-0.3.8/.github/dependabot.yml
--rw-r--r--   0        0        0      635 2023-05-11 21:02:05.040800 ellar-0.3.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      545 2023-05-11 21:02:05.040800 ellar-0.3.8/.github/workflows/test.yml
--rw-r--r--   0        0        0     1122 2023-05-11 21:02:05.044801 ellar-0.3.8/.github/workflows/test_full.yml
--rw-r--r--   0        0        0     1891 2023-05-11 21:02:05.044801 ellar-0.3.8/.gitignore
--rw-r--r--   0        0        0       53 2023-05-11 21:02:05.044801 ellar-0.3.8/.isort.cfg
--rw-r--r--   0        0        0     1073 2023-05-11 21:02:05.044801 ellar-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1083 2023-05-11 21:02:05.044801 ellar-0.3.8/LICENSE
--rw-r--r--   0        0        0     1166 2023-05-11 21:02:05.044801 ellar-0.3.8/Makefile
--rw-r--r--   0        0        0    10720 2023-05-11 21:02:05.044801 ellar-0.3.8/README.md
--rw-r--r--   0        0        0       15 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/background-task.md
--rw-r--r--   0        0        0       15 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/api-docs.md
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/custom-providers.md
--rw-r--r--   0        0        0       15 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/events.md
--rw-r--r--   0        0        0    10656 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/execution-context.md
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/file-streaming.md
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/injection-scope.md
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/model-view-controller.md
--rw-r--r--   0        0        0    14828 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/testing.md
--rw-r--r--   0        0        0     7857 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/basics/versioning.md
--rw-r--r--   0        0        0    20991 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/caching.md
--rw-r--r--   0        0        0     1177 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/command-grouping.md
--rw-r--r--   0        0        0     6586 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/create-module-command.md
--rw-r--r--   0        0        0      388 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/create-project-command.md
--rw-r--r--   0        0        0     2755 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/custom-commands.md
--rw-r--r--   0        0        0     1340 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/index.md
--rw-r--r--   0        0        0     1206 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/new-command.md
--rw-r--r--   0        0        0      803 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/commands/runserver-command.md
--rw-r--r--   0        0        0     9048 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/configurations.md
--rw-r--r--   0        0        0     1765 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/custom-setup.md
--rw-r--r--   0        0        0     6502 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/handling-response/response-model.md
--rw-r--r--   0        0        0     6571 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/handling-response/response.md
--rwxr-xr-x   0        0        0    25915 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0    26456 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/EllarLogoW.png
--rwxr-xr-x   0        0        0     3888 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/Icon.svg
--rwxr-xr-x   0        0        0     4781 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/Logo.svg
--rw-r--r--   0        0        0    92094 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/ModuleDescription.png
--rw-r--r--   0        0        0    71483 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/body-schema-doc.png
--rw-r--r--   0        0        0   233058 2023-05-11 21:02:05.044801 ellar-0.3.8/docs/img/body-schema-doc2.png
--rw-r--r--   0        0        0   196608 2023-05-11 21:02:05.048801 ellar-0.3.8/docs/img/body-schema-doc3.png
--rwxr-xr-x   0        0        0    54689 2023-05-11 21:02:05.048801 ellar-0.3.8/docs/img/car_api.png
--rw-r--r--   0        0        0  1632661 2023-05-11 21:02:05.056801 ellar-0.3.8/docs/img/car_controller.gif
--rw-r--r--   0        0        0    50364 2023-05-11 21:02:05.056801 ellar-0.3.8/docs/img/controller_description.png
--rw-r--r--   0        0        0    45273 2023-05-11 21:02:05.056801 ellar-0.3.8/docs/img/create-car-schema.png
--rw-r--r--   0        0        0    19519 2023-05-11 21:02:05.056801 ellar-0.3.8/docs/img/create-dog-schema.png
--rwxr-xr-x   0        0        0  1326350 2023-05-11 21:02:05.064801 ellar-0.3.8/docs/img/ellar_demo.gif
--rwxr-xr-x   0        0        0    69977 2023-05-11 21:02:05.064801 ellar-0.3.8/docs/img/ellar_framework.png
--rw-r--r--   0        0        0   244178 2023-05-11 21:02:05.064801 ellar-0.3.8/docs/img/enum_docs_swagger.png
--rw-r--r--   0        0        0   168505 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/event_docs_swagger.png
--rw-r--r--   0        0        0   253271 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/form-schema-doc.png
--rw-r--r--   0        0        0   170683 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/json_api_response_model.png
--rw-r--r--   0        0        0    71548 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/live_support_websocket.gif
--rw-r--r--   0        0        0   121361 2023-05-11 21:02:05.068801 ellar-0.3.8/docs/img/live_support_websocket_3.gif
--rw-r--r--   0        0        0   216500 2023-05-11 21:02:05.072801 ellar-0.3.8/docs/img/math_router.png
--rw-r--r--   0        0        0   280669 2023-05-11 21:02:05.072801 ellar-0.3.8/docs/img/math_router_with_request_object.png
--rw-r--r--   0        0        0    52280 2023-05-11 21:02:05.072801 ellar-0.3.8/docs/img/middleware.png
--rw-r--r--   0        0        0   267982 2023-05-11 21:02:05.072801 ellar-0.3.8/docs/img/query_filter_swagger.png
--rw-r--r--   0        0        0   208787 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/img/response_description.png
--rw-r--r--   0        0        0     4486 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/index.md
--rw-r--r--   0        0        0       15 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/mount.md
--rw-r--r--   0        0        0    12542 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/controllers.md
--rw-r--r--   0        0        0    22629 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/custom_decorators.md
--rw-r--r--   0        0        0     7960 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/exception_handling.md
--rw-r--r--   0        0        0     8926 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/guards.md
--rw-r--r--   0        0        0     7665 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/index.md
--rw-r--r--   0        0        0     9240 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/middleware.md
--rw-r--r--   0        0        0     4493 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/module-router.md
--rw-r--r--   0        0        0    15322 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/modules.md
--rw-r--r--   0        0        0     9375 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/overview/providers.md
--rw-r--r--   0        0        0     8879 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/body.md
--rw-r--r--   0        0        0     1371 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/cookie-params.md
--rw-r--r--   0        0        0     6588 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/file-params.md
--rw-r--r--   0        0        0     4096 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/form-params.md
--rw-r--r--   0        0        0     3795 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/header-params.md
--rw-r--r--   0        0        0     1560 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/index.md
--rw-r--r--   0        0        0     6749 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/path-params.md
--rw-r--r--   0        0        0     4920 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/parsing-inputs/query-params.md
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/release-notes.md
--rw-r--r--   0        0        0       69 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     4111 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/templating/staticfiles.md
--rw-r--r--   0        0        0    13593 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/templating/templating.md
--rw-r--r--   0        0        0     7327 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/throttling.md
--rw-r--r--   0        0        0    12688 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/websockets/index.md
--rw-r--r--   0        0        0    12825 2023-05-11 21:02:05.076801 ellar-0.3.8/docs/websockets/socketio.md
--rw-r--r--   0        0        0      143 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/__init__.py
--rw-r--r--   0        0        0      257 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/__init__.py
--rw-r--r--   0        0        0      109 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/__init__.py
--rw-r--r--   0        0        0     4841 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/_aio_cache.py.ellar
--rw-r--r--   0        0        0     4361 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/base.py
--rw-r--r--   0        0        0     5145 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/local_cache.py
--rw-r--r--   0        0        0      944 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/pylib_cache.py
--rw-r--r--   0        0        0     2215 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/pymem_cache.py
--rw-r--r--   0        0        0       72 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/redis/__init__.py
--rw-r--r--   0        0        0     6548 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/redis/backend.py
--rw-r--r--   0        0        0     1397 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/backends/serializer.py
--rw-r--r--   0        0        0     5132 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/decorator.py
--rw-r--r--   0        0        0    10943 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/interface.py
--rw-r--r--   0        0        0     2027 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/make_key_decorator.py
--rw-r--r--   0        0        0     2501 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/model.py
--rw-r--r--   0        0        0     1859 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/module.py
--rw-r--r--   0        0        0      852 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/schema.py
--rw-r--r--   0        0        0     4505 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/cache/service.py
--rw-r--r--   0        0        0     3727 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/__init__.py
--rw-r--r--   0        0        0      108 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/commands/__init__.py
--rw-r--r--   0        0        0     2234 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/commands/base.py
--rw-r--r--   0        0        0     1517 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/commands/decorator.py
--rw-r--r--   0        0        0      270 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/compatible/__init__.py
--rw-r--r--   0        0        0     1166 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/compatible/cache_properties.py
--rw-r--r--   0        0        0     1511 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/compatible/dict.py
--rw-r--r--   0        0        0      637 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/compatible/emails.py
--rw-r--r--   0        0        0     4620 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/constants.py
--rw-r--r--   0        0        0     1670 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/converters.py
--rw-r--r--   0        0        0      809 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/datastructures.py
--rw-r--r--   0        0        0      795 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/__init__.py
--rw-r--r--   0        0        0      501 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/base.py
--rw-r--r--   0        0        0     6652 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/controller.py
--rw-r--r--   0        0        0     1036 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/exception.py
--rw-r--r--   0        0        0      610 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/extra_args.py
--rw-r--r--   0        0        0     2528 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/file.py
--rw-r--r--   0        0        0      541 2023-05-11 21:02:05.076801 ellar-0.3.8/ellar/common/decorators/guards.py
--rw-r--r--   0        0        0     4748 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/html.py
--rw-r--r--   0        0        0      626 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/middleware.py
--rw-r--r--   0        0        0     3105 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/modules.py
--rw-r--r--   0        0        0      932 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/openapi.py
--rw-r--r--   0        0        0     1295 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/serializer.py
--rw-r--r--   0        0        0      402 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/decorators/versioning.py
--rw-r--r--   0        0        0      840 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/__init__.py
--rw-r--r--   0        0        0      472 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/api/__init__.py
--rw-r--r--   0        0        0     1447 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/api/base.py
--rw-r--r--   0        0        0     1239 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/api/exceptions_types.py
--rw-r--r--   0        0        0     2498 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/callable_exceptions.py
--rw-r--r--   0        0        0      103 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/context.py
--rw-r--r--   0        0        0     2517 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/handlers.py
--rw-r--r--   0        0        0      598 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/exceptions/validation.py
--rw-r--r--   0        0        0     1485 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/__init__.py
--rw-r--r--   0        0        0      658 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/enums.py
--rw-r--r--   0        0        0      389 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/event_loop.py
--rw-r--r--   0        0        0     2137 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/importer.py
--rw-r--r--   0        0        0     1272 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/modelfield.py
--rw-r--r--   0        0        0      703 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/helper/module_loading.py
--rw-r--r--   0        0        0      800 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/__init__.py
--rw-r--r--   0        0        0     3560 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/context.py
--rw-r--r--   0        0        0      278 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/controller_factory.py
--rw-r--r--   0        0        0     1356 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/exceptions.py
--rw-r--r--   0        0        0     1771 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/module.py
--rw-r--r--   0        0        0      749 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/response_model.py
--rw-r--r--   0        0        0      908 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/interfaces/templating.py
--rw-r--r--   0        0        0       52 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/logger.py
--rw-r--r--   0        0        0      274 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/models/__init__.py
--rw-r--r--   0        0        0      923 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/models/controller.py
--rw-r--r--   0        0        0     4258 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/models/guard.py
--rw-r--r--   0        0        0      476 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/__init__.py
--rw-r--r--   0        0        0      365 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/__init__.py
--rw-r--r--   0        0        0    14101 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/base.py
--rw-r--r--   0        0        0     1615 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/extra_args.py
--rw-r--r--   0        0        0     2045 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/factory.py
--rw-r--r--   0        0        0     4252 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/request_model.py
--rw-r--r--   0        0        0     5893 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/resolver_generators.py
--rw-r--r--   0        0        0     2457 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/args/websocket_model.py
--rw-r--r--   0        0        0     1235 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/helpers.py
--rw-r--r--   0        0        0     9342 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/params.py
--rw-r--r--   0        0        0     1083 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/__init__.py
--rw-r--r--   0        0        0     1678 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/base.py
--rw-r--r--   0        0        0     4460 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/bulk_parameter.py
--rw-r--r--   0        0        0      687 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/__init__.py
--rw-r--r--   0        0        0     2961 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/base.py
--rw-r--r--   0        0        0      391 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/connection.py
--rw-r--r--   0        0        0      328 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/context.py
--rw-r--r--   0        0        0     1660 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/inject.py
--rw-r--r--   0        0        0      387 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/request.py
--rw-r--r--   0        0        0      394 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/response.py
--rw-r--r--   0        0        0      524 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/session.py
--rw-r--r--   0        0        0      386 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/non_parameter/websocket.py
--rw-r--r--   0        0        0     9544 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/params/resolvers/parameter.py
--rw-r--r--   0        0        0      415 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/__init__.py
--rw-r--r--   0        0        0      925 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/__init__.py
--rw-r--r--   0        0        0     6157 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/base.py
--rw-r--r--   0        0        0       50 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/exceptions.py
--rw-r--r--   0        0        0     3129 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/file.py
--rw-r--r--   0        0        0      691 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/helper.py
--rw-r--r--   0        0        0     1952 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/html.py
--rw-r--r--   0        0        0     2336 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/json.py
--rw-r--r--   0        0        0     4256 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/route.py
--rw-r--r--   0        0        0     2167 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/models/type_converter.py
--rw-r--r--   0        0        0      995 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/responses/response_types.py
--rw-r--r--   0        0        0     1668 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/__init__.py
--rw-r--r--   0        0        0     4546 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/base.py
--rw-r--r--   0        0        0     1314 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/builder.py
--rw-r--r--   0        0        0      272 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/__init__.py
--rw-r--r--   0        0        0     1175 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/base.py
--rw-r--r--   0        0        0     1881 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/factory.py
--rw-r--r--   0        0        0     1242 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/route.py
--rw-r--r--   0        0        0      190 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/websocket/__init__.py
--rw-r--r--   0        0        0     1424 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/websocket/handler.py
--rw-r--r--   0        0        0     2011 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/controller/websocket/route.py
--rw-r--r--   0        0        0     6698 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/mount.py
--rw-r--r--   0        0        0    10992 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/operation_definitions.py
--rw-r--r--   0        0        0    10559 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/params.py
--rw-r--r--   0        0        0     4569 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/route.py
--rw-r--r--   0        0        0     3576 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/route_collections.py
--rw-r--r--   0        0        0     3201 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/schema.py
--rw-r--r--   0        0        0      161 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/websocket/__init__.py
--rw-r--r--   0        0        0     5680 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/websocket/handler.py
--rw-r--r--   0        0        0     4879 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/routing/websocket/route.py
--rw-r--r--   0        0        0      499 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/serializer/__init__.py
--rw-r--r--   0        0        0     4959 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/serializer/base.py
--rw-r--r--   0        0        0      194 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/serializer/guard.py
--rw-r--r--   0        0        0      453 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/shortcuts.py
--rw-r--r--   0        0        0      613 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/__init__.py
--rw-r--r--   0        0        0      472 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/environment.py
--rw-r--r--   0        0        0     1634 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/loader.py
--rw-r--r--   0        0        0     2895 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/model.py
--rw-r--r--   0        0        0     2482 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/renderer.py
--rw-r--r--   0        0        0      110 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/templating/schema.py
--rw-r--r--   0        0        0      585 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/common/types.py
--rw-r--r--   0        0        0      925 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/__init__.py
--rw-r--r--   0        0        0      120 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/conf/__init__.py
--rw-r--r--   0        0        0     4914 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/conf/app_settings_models.py
--rw-r--r--   0        0        0     2177 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/conf/config.py
--rw-r--r--   0        0        0     5122 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/conf/mixins.py
--rw-r--r--   0        0        0      470 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/connection/__init__.py
--rw-r--r--   0        0        0      688 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/connection/http.py
--rw-r--r--   0        0        0      245 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/connection/websocket.py
--rw-r--r--   0        0        0      458 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/context/__init__.py
--rw-r--r--   0        0        0     1453 2023-05-11 21:02:05.080801 ellar-0.3.8/ellar/core/context/execution.py
--rw-r--r--   0        0        0     2539 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/context/factory.py
--rw-r--r--   0        0        0     2091 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/context/host.py
--rw-r--r--   0        0        0     2122 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/context/http.py
--rw-r--r--   0        0        0      817 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/context/websocket.py
--rw-r--r--   0        0        0     1492 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/core_service_registration.py
--rw-r--r--   0        0        0       97 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/exceptions/__init__.py
--rw-r--r--   0        0        0     2273 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/exceptions/service.py
--rw-r--r--   0        0        0     7616 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/factory.py
--rw-r--r--   0        0        0      263 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/guard/__init__.py
--rw-r--r--   0        0        0      744 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/guard/apikey.py
--rw-r--r--   0        0        0     3318 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/guard/http.py
--rw-r--r--   0        0        0     9463 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/main.py
--rw-r--r--   0        0        0     1159 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/__init__.py
--rw-r--r--   0        0        0     2576 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/di.py
--rw-r--r--   0        0        0     2704 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/exceptions.py
--rw-r--r--   0        0        0     2256 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/function.py
--rw-r--r--   0        0        0      121 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/sessions.py
--rw-r--r--   0        0        0     1095 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/middleware/versioning.py
--rw-r--r--   0        0        0      321 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/__init__.py
--rw-r--r--   0        0        0     1287 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/base.py
--rw-r--r--   0        0        0     3139 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/builder.py
--rw-r--r--   0        0        0     5827 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/config.py
--rw-r--r--   0        0        0      787 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/helper.py
--rw-r--r--   0        0        0    10210 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/modules/ref.py
--rw-r--r--   0        0        0       75 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/routing/__init__.py
--rw-r--r--   0        0        0     3853 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/routing/app.py
--rw-r--r--   0        0        0       58 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/services/__init__.py
--rw-r--r--   0        0        0     1949 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/services/reflector.py
--rw-r--r--   0        0        0     1718 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/staticfiles.py
--rw-r--r--   0        0        0       67 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/templating/__init__.py
--rw-r--r--   0        0        0     3978 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/templating/app.py
--rw-r--r--   0        0        0      563 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/versioning/__init__.py
--rw-r--r--   0        0        0     2526 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/versioning/base.py
--rw-r--r--   0        0        0     6198 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/core/versioning/resolver.py
--rw-r--r--   0        0        0      915 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/__init__.py
--rw-r--r--   0        0        0      344 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/asgi_args.py
--rw-r--r--   0        0        0     1073 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/constants.py
--rw-r--r--   0        0        0      400 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/exceptions.py
--rw-r--r--   0        0        0      117 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/injector/__init__.py
--rw-r--r--   0        0        0     7647 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/injector/container.py
--rw-r--r--   0        0        0     5268 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/injector/ellar_injector.py
--rw-r--r--   0        0        0      845 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/providers.py
--rw-r--r--   0        0        0     2247 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/scopes.py
--rw-r--r--   0        0        0     4525 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/service_config.py
--rw-r--r--   0        0        0       39 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/types.py
--rw-r--r--   0        0        0      244 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/di/utils.py
--rw-r--r--   0        0        0     2052 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/events.py
--rw-r--r--   0        0        0      573 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/__init__.py
--rw-r--r--   0        0        0     8069 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/builder.py
--rw-r--r--   0        0        0      239 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/docs_generators/__init__.py
--rw-r--r--   0        0        0      530 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/docs_generators/base.py
--rw-r--r--   0        0        0      959 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/docs_generators/redocs.py
--rw-r--r--   0        0        0     1025 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/docs_generators/swagger.py
--rw-r--r--   0        0        0     2937 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/module.py
--rw-r--r--   0        0        0    10611 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/openapi_v3.py
--rw-r--r--   0        0        0    15879 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/route_doc_models.py
--rw-r--r--   0        0        0      115 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/schemas/__init__.py
--rw-r--r--   0        0        0      342 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/schemas/validation.py
--rw-r--r--   0        0        0      702 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/templates/redocs.html
--rw-r--r--   0        0        0      758 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/openapi/templates/swagger.html
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/py.typed
--rw-r--r--   0        0        0      180 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/reflect/__init__.py
--rw-r--r--   0        0        0     5356 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/reflect/_reflect.py
--rw-r--r--   0        0        0       34 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/reflect/constants.py
--rw-r--r--   0        0        0      238 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/reflect/contextmanager_fix.py
--rw-r--r--   0        0        0       58 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/controllers/__init__.py
--rw-r--r--   0        0        0      381 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/controllers/home.py
--rw-r--r--   0        0        0      211 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/modules.py
--rw-r--r--   0        0        0   155845 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/static/css/bootstrap.min.css
--rwxr-xr-x   0        0        0    25915 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/static/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/static/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0     3888 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/static/img/Icon.svg
--rw-r--r--   0        0        0     1312 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/samples/templates/home/index.html
--rw-r--r--   0        0        0      596 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/__init__.py
--rw-r--r--   0        0        0      423 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/adapter.py
--rw-r--r--   0        0        0      524 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/constants.py
--rw-r--r--   0        0        0     1659 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/context.py
--rw-r--r--   0        0        0      225 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/decorators/__init__.py
--rw-r--r--   0        0        0      667 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/decorators/events.py
--rw-r--r--   0        0        0     3846 2023-05-11 21:02:05.084801 ellar-0.3.8/ellar/socket_io/decorators/gateway.py
--rw-r--r--   0        0        0      578 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/decorators/subscribe_message.py
--rw-r--r--   0        0        0     2521 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/factory.py
--rw-r--r--   0        0        0     9918 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/gateway.py
--rw-r--r--   0        0        0      144 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/model.py
--rw-r--r--   0        0        0      465 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/responses.py
--rw-r--r--   0        0        0      107 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/testing/__init__.py
--rw-r--r--   0        0        0     1704 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/socket_io/testing/module.py
--rw-r--r--   0        0        0      129 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/testing/__init__.py
--rw-r--r--   0        0        0     4074 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/testing/module.py
--rw-r--r--   0        0        0     1215 2023-05-11 21:02:05.088801 ellar-0.3.8/ellar/testing/uvicorn_server.py
--rw-r--r--   0        0        0      509 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/README.md
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/__init__.py
--rw-r--r--   0        0        0     1659 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/controllers.py
--rw-r--r--   0        0        0     1077 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/module.py
--rw-r--r--   0        0        0     1146 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/routers.py
--rw-r--r--   0        0        0      629 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/schemas.py
--rw-r--r--   0        0        0      666 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/services.py
--rw-r--r--   0        0        0     1708 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/blog/blog.css
--rw-r--r--   0        0        0     1586 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css
--rw-r--r--   0        0        0     1008 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg
--rw-r--r--   0        0        0     2047 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/__init__.py
--rw-r--r--   0        0        0     2900 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_controllers.py
--rw-r--r--   0        0        0     1604 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_routers.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_services.py
--rw-r--r--   0        0        0      202 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/views/car/list.html
--rw-r--r--   0        0        0      202 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/views/cat/list.html
--rw-r--r--   0        0        0    15257 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/apps/car/views/index.html
--rw-r--r--   0        0        0      216 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/commands.py
--rw-r--r--   0        0        0      187 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/config.py
--rw-r--r--   0        0        0      598 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/root_module.py
--rw-r--r--   0        0        0      954 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/server.py
--rw-r--r--   0        0        0      134 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/carapp/tests/conftest.py
--rw-r--r--   0        0        0      241 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/01-carapp/pyproject.toml
--rw-r--r--   0        0        0      264 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/README.md
--rw-r--r--   0        0        0      283 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/__init__.py
--rw-r--r--   0        0        0      455 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/controllers.py
--rw-r--r--   0        0        0     2182 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/gateways.py
--rw-r--r--   0        0        0     1005 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/module.py
--rw-r--r--   0        0        0      295 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/routers.py
--rw-r--r--   0        0        0      542 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/schemas.py
--rw-r--r--   0        0        0      179 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/services.py
--rw-r--r--   0        0        0     3829 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/templates/events/index.html
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/tests/test_controllers.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/tests/test_routers.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/tests/test_services.py
--rw-r--r--   0        0        0     2602 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/config.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/domain/__init__.py
--rw-r--r--   0        0        0      480 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/root_module.py
--rw-r--r--   0        0        0     1045 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/socketio_app/server.py
--rw-r--r--   0        0        0       43 2023-05-11 21:02:05.088801 ellar-0.3.8/examples/02-socketio-app/tests/conftest.py
--rw-r--r--   0        0        0     3824 2023-05-11 21:02:05.088801 ellar-0.3.8/mkdocs.yml
--rw-r--r--   0        0        0      597 2023-05-11 21:02:05.088801 ellar-0.3.8/mypy.ini
--rw-r--r--   0        0        0     3037 2023-05-11 21:02:05.088801 ellar-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      207 2023-05-11 21:02:05.088801 ellar-0.3.8/pytest.ini
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/conftest.py
--rw-r--r--   0        0        0      616 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/injector_module.py
--rw-r--r--   0        0        0     5249 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/main.py
--rw-r--r--   0        0        0       23 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/private/test.css
--rw-r--r--   0        0        0      748 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/schema.py
--rw-r--r--   0        0        0        4 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/statics/example.txt
--rw-r--r--   0        0        0      160 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/ellar/index.html
--rw-r--r--   0        0        0      102 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/ellar/list.html
--rw-r--r--   0        0        0      129 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/index.html
--rw-r--r--   0        0        0      128 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/list.html
--rw-r--r--   0        0        0       65 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/templates/render_string.html
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/__init__.py
--rw-r--r--   0        0        0       84 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/config.py
--rw-r--r--   0        0        0     2854 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/sample.py
--rw-r--r--   0        0        0     3548 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_application_factory.py
--rw-r--r--   0        0        0    15855 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_application_functions.py
--rw-r--r--   0        0        0    18052 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_cors.py
--rw-r--r--   0        0        0     4284 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_replacing_app_services.py
--rw-r--r--   0        0        0     2329 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_application/test_trusted_host.py
--rw-r--r--   0        0        0      862 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_attribute_dict.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/__init__.py
--rw-r--r--   0        0        0     3625 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/_test_aio_memcache.py.ellar
--rw-r--r--   0        0        0     1893 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/pylib_mock.py
--rw-r--r--   0        0        0     2592 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/redis_mock.py
--rw-r--r--   0        0        0     2764 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_cache_decorator.py
--rw-r--r--   0        0        0     1744 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_cache_many_config.py
--rw-r--r--   0        0        0     4772 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_cache_service.py
--rw-r--r--   0        0        0     4995 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_local_cache.py
--rw-r--r--   0        0        0      596 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_module_setup.py
--rw-r--r--   0        0        0     9973 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_pylibmc_cache.py
--rw-r--r--   0        0        0     6093 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_redis_cache.py
--rw-r--r--   0        0        0      577 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_cache/test_schema.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_conf/__init__.py
--rw-r--r--   0        0        0     5223 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_conf/test_default_conf.py
--rw-r--r--   0        0        0     1151 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_conf/test_mixins.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/__init__.py
--rw-r--r--   0        0        0      387 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/sample.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/test_application_router.py
--rw-r--r--   0        0        0     4450 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/test_controller_decorator.py
--rw-r--r--   0        0        0     2442 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/test_controller_inheritance.py
--rw-r--r--   0        0        0     2628 2023-05-11 21:02:05.088801 ellar-0.3.8/tests/test_controller/test_module_router.py
--rw-r--r--   0        0        0     7165 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_controller/test_route_collection.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/__init__.py
--rw-r--r--   0        0        0     3360 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_controller.py
--rw-r--r--   0        0        0      789 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_exception.py
--rw-r--r--   0        0        0     3508 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_file.py
--rw-r--r--   0        0        0     1050 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_guards.py
--rw-r--r--   0        0        0     4082 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_html.py
--rw-r--r--   0        0        0      554 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_middleware.py
--rw-r--r--   0        0        0     2061 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_modules.py
--rw-r--r--   0        0        0      915 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_openapi.py
--rw-r--r--   0        0        0     1311 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_serializer.py
--rw-r--r--   0        0        0      475 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_decorators/test_versioning.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/__init__.py
--rw-r--r--   0        0        0     1332 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/examples.py
--rw-r--r--   0        0        0     2078 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/test_injectable_resolving.py
--rw-r--r--   0        0        0     6275 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/test_injector.py
--rw-r--r--   0        0        0     3508 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/test_provider_scopes.py
--rw-r--r--   0        0        0     3993 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_di/test_providers.py
--rw-r--r--   0        0        0     1817 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_events.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/__init__.py
--rw-r--r--   0        0        0      206 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/exception_runner.py
--rw-r--r--   0        0        0     2562 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/test_api_exception.py
--rw-r--r--   0        0        0     8609 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/test_custom_exceptions.py
--rw-r--r--   0        0        0     1195 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/test_error_details.py
--rw-r--r--   0        0        0     3722 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_exceptions/test_validation_exception.py
--rw-r--r--   0        0        0     7162 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_guard.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/__init__.py
--rw-r--r--   0        0        0      571 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/test_enum.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/test_importer.py
--rw-r--r--   0        0        0      795 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/test_model_field.py
--rw-r--r--   0        0        0      298 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_helper/test_module_loading.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_middleware/__init__.py
--rw-r--r--   0        0        0     2302 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_middleware/test_functional_middleware.py
--rw-r--r--   0        0        0     4243 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_middleware/test_service_provider_middleware.py
--rw-r--r--   0        0        0     2168 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_middleware/test_versioning_middleware.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_modules/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_modules/sample.py
--rw-r--r--   0        0        0     6760 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_modules/test_module_config.py
--rw-r--r--   0        0        0    10084 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_modules/test_module_ref.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_openapi/__init__.py
--rw-r--r--   0        0        0     8341 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_openapi/test_builder.py
--rw-r--r--   0        0        0     6680 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_openapi/test_module.py
--rw-r--r--   0        0        0    16449 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_openapi/test_open_api_route_documentation.py
--rw-r--r--   0        0        0     5571 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_reflect.py
--rw-r--r--   0        0        0     2154 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_reflector.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/__init__.py
--rw-r--r--   0        0        0     2481 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_defined_response_model.py
--rw-r--r--   0        0        0     4562 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_pydantic_response_model.py
--rw-r--r--   0        0        0     3393 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_response_file.py
--rw-r--r--   0        0        0     5063 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_response_html.py
--rw-r--r--   0        0        0     3228 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_response_streaming.py
--rw-r--r--   0        0        0     3902 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_response_type_definition_converter.py
--rw-r--r--   0        0        0     3524 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_response/test_route_response_model.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/__init__.py
--rw-r--r--   0        0        0     1126 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/sample.py
--rw-r--r--   0        0        0     3605 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_body_schema.py
--rw-r--r--   0        0        0     3666 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_body_schema_extra_properties.py
--rw-r--r--   0        0        0     4142 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_body_union_schema.py
--rw-r--r--   0        0        0     3902 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_cookie_schema.py
--rw-r--r--   0        0        0     6854 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_extra_args.py
--rw-r--r--   0        0        0     2346 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_form_schema.py
--rw-r--r--   0        0        0    10018 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_formparsers.py
--rw-r--r--   0        0        0     1282 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_forms.py
--rw-r--r--   0        0        0     1296 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0     3522 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_header_schema.py
--rw-r--r--   0        0        0     1563 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_invalid_path_param.py
--rw-r--r--   0        0        0     1760 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     5205 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_multi_body_errors.py
--rw-r--r--   0        0        0     3783 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_multi_query_errors.py
--rw-r--r--   0        0        0     9423 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_path.py
--rw-r--r--   0        0        0     2769 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_path_with_schema.py
--rw-r--r--   0        0        0     3333 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_put_with_no_body_schema.py
--rw-r--r--   0        0        0     2242 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_query.py
--rw-r--r--   0        0        0     3588 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_query_schema.py
--rw-r--r--   0        0        0     1987 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_request.py
--rw-r--r--   0        0        0     3415 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_routing/test_route_endpoint_params.py
--rw-r--r--   0        0        0      451 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_sample_project.py
--rw-r--r--   0        0        0     2712 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_schema.py
--rw-r--r--   0        0        0     6379 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_serializer.py
--rw-r--r--   0        0        0      775 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_shortcuts.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/__init__.py
--rw-r--r--   0        0        0     4110 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/sample.py
--rw-r--r--   0        0        0      718 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/test_decorators/test_events.py
--rw-r--r--   0        0        0     3592 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/test_decorators/test_gateway.py
--rw-r--r--   0        0        0      719 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/test_decorators/test_subcribe_message.py
--rw-r--r--   0        0        0     8889 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_socket_io/test_operation.py
--rw-r--r--   0        0        0    14104 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_staticfiles.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/module_statics/watever.txt
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/static/watever.txt
--rw-r--r--   0        0        0      167 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/templates/watever.html
--rw-r--r--   0        0        0     2904 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/test_module_templating.py
--rw-r--r--   0        0        0     2718 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/test_renderer.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_templating/views/watever.html
--rw-r--r--   0        0        0     2425 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_testing.py
--rw-r--r--   0        0        0        0 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/__init__.py
--rw-r--r--   0        0        0     1968 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/operations.py
--rw-r--r--   0        0        0     2138 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_default_versioning.py
--rw-r--r--   0        0        0     4449 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_default_versioning_for_controllers.py
--rw-r--r--   0        0        0     4475 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_header_versioning.py
--rw-r--r--   0        0        0     7820 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_header_versioning_controller.py
--rw-r--r--   0        0        0     3823 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_host_versioning.py
--rw-r--r--   0        0        0     3227 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_query_versioning.py
--rw-r--r--   0        0        0     2865 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_versioning/test_url_versioning.py
--rw-r--r--   0        0        0    17496 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_websocket.py
--rw-r--r--   0        0        0    11075 2023-05-11 21:02:05.092801 ellar-0.3.8/tests/test_websocket_handler.py
--rw-r--r--   0        0        0    14822 1970-01-01 00:00:00.000000 ellar-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      270 2023-05-29 23:22:51.594828 ellar-0.4.0/.coveragerc
+-rw-r--r--   0        0        0       65 2023-05-29 23:22:51.594828 ellar-0.4.0/.dockerignore
+-rw-r--r--   0        0        0      146 2023-05-29 23:22:51.594828 ellar-0.4.0/.flake8
+-rw-r--r--   0        0        0      205 2023-05-29 23:22:51.594828 ellar-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      635 2023-05-29 23:22:51.594828 ellar-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      545 2023-05-29 23:22:51.594828 ellar-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1122 2023-05-29 23:22:51.594828 ellar-0.4.0/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0     1891 2023-05-29 23:22:51.594828 ellar-0.4.0/.gitignore
+-rw-r--r--   0        0        0       53 2023-05-29 23:22:51.594828 ellar-0.4.0/.isort.cfg
+-rw-r--r--   0        0        0     1073 2023-05-29 23:22:51.594828 ellar-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1083 2023-05-29 23:22:51.594828 ellar-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1166 2023-05-29 23:22:51.594828 ellar-0.4.0/Makefile
+-rw-r--r--   0        0        0    10596 2023-05-29 23:22:51.594828 ellar-0.4.0/README.md
+-rw-r--r--   0        0        0     2289 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/background-task.md
+-rw-r--r--   0        0        0       15 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/api-docs.md
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/custom-providers.md
+-rw-r--r--   0        0        0       15 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/events.md
+-rw-r--r--   0        0        0    10686 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/execution-context.md
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/file-streaming.md
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/injection-scope.md
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/model-view-controller.md
+-rw-r--r--   0        0        0    14852 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/testing.md
+-rw-r--r--   0        0        0     7874 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/basics/versioning.md
+-rw-r--r--   0        0        0    21109 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/caching.md
+-rw-r--r--   0        0        0     1177 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/command-grouping.md
+-rw-r--r--   0        0        0     6586 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/create-module-command.md
+-rw-r--r--   0        0        0      388 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/create-project-command.md
+-rw-r--r--   0        0        0     2755 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/custom-commands.md
+-rw-r--r--   0        0        0     1340 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/index.md
+-rw-r--r--   0        0        0     1206 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/new-command.md
+-rw-r--r--   0        0        0      803 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/commands/runserver-command.md
+-rw-r--r--   0        0        0     9081 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/configurations.md
+-rw-r--r--   0        0        0     1765 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/custom-setup.md
+-rw-r--r--   0        0        0     6521 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/handling-response/response-model.md
+-rw-r--r--   0        0        0     6571 2023-05-29 23:22:51.594828 ellar-0.4.0/docs/handling-response/response.md
+-rwxr-xr-x   0        0        0    25915 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0    26456 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/EllarLogoW.png
+-rwxr-xr-x   0        0        0     3888 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/Icon.svg
+-rwxr-xr-x   0        0        0     4781 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/Logo.svg
+-rw-r--r--   0        0        0    92094 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/ModuleDescription.png
+-rw-r--r--   0        0        0    71483 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/body-schema-doc.png
+-rw-r--r--   0        0        0   233058 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/body-schema-doc2.png
+-rw-r--r--   0        0        0   196608 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/body-schema-doc3.png
+-rwxr-xr-x   0        0        0    54689 2023-05-29 23:22:51.598828 ellar-0.4.0/docs/img/car_api.png
+-rw-r--r--   0        0        0  1632661 2023-05-29 23:22:51.610828 ellar-0.4.0/docs/img/car_controller.gif
+-rw-r--r--   0        0        0    50364 2023-05-29 23:22:51.610828 ellar-0.4.0/docs/img/controller_description.png
+-rw-r--r--   0        0        0    45273 2023-05-29 23:22:51.614828 ellar-0.4.0/docs/img/create-car-schema.png
+-rw-r--r--   0        0        0    19519 2023-05-29 23:22:51.614828 ellar-0.4.0/docs/img/create-dog-schema.png
+-rwxr-xr-x   0        0        0  1326350 2023-05-29 23:22:51.618828 ellar-0.4.0/docs/img/ellar_demo.gif
+-rwxr-xr-x   0        0        0    69977 2023-05-29 23:22:51.618828 ellar-0.4.0/docs/img/ellar_framework.png
+-rw-r--r--   0        0        0   244178 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/enum_docs_swagger.png
+-rw-r--r--   0        0        0   168505 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/event_docs_swagger.png
+-rw-r--r--   0        0        0   253271 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/form-schema-doc.png
+-rw-r--r--   0        0        0   170683 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/json_api_response_model.png
+-rw-r--r--   0        0        0    71548 2023-05-29 23:22:51.622828 ellar-0.4.0/docs/img/live_support_websocket.gif
+-rw-r--r--   0        0        0   121361 2023-05-29 23:22:51.626828 ellar-0.4.0/docs/img/live_support_websocket_3.gif
+-rw-r--r--   0        0        0   216500 2023-05-29 23:22:51.626828 ellar-0.4.0/docs/img/math_router.png
+-rw-r--r--   0        0        0   280669 2023-05-29 23:22:51.626828 ellar-0.4.0/docs/img/math_router_with_request_object.png
+-rw-r--r--   0        0        0    52280 2023-05-29 23:22:51.626828 ellar-0.4.0/docs/img/middleware.png
+-rw-r--r--   0        0        0   267982 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/img/query_filter_swagger.png
+-rw-r--r--   0        0        0   208787 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/img/response_description.png
+-rw-r--r--   0        0        0     4486 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/index.md
+-rw-r--r--   0        0        0     2028 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/mount.md
+-rw-r--r--   0        0        0    12559 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/controllers.md
+-rw-r--r--   0        0        0    22477 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/custom_decorators.md
+-rw-r--r--   0        0        0     7997 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/exception_handling.md
+-rw-r--r--   0        0        0     8976 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/guards.md
+-rw-r--r--   0        0        0     7695 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/index.md
+-rw-r--r--   0        0        0     6521 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/interceptors.md
+-rw-r--r--   0        0        0     9258 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/middleware.md
+-rw-r--r--   0        0        0     4497 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/module-router.md
+-rw-r--r--   0        0        0    15337 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/modules.md
+-rw-r--r--   0        0        0     9391 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/overview/providers.md
+-rw-r--r--   0        0        0     8879 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/body.md
+-rw-r--r--   0        0        0     1371 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/cookie-params.md
+-rw-r--r--   0        0        0     6588 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/file-params.md
+-rw-r--r--   0        0        0     4096 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/form-params.md
+-rw-r--r--   0        0        0     3795 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/header-params.md
+-rw-r--r--   0        0        0     1560 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/index.md
+-rw-r--r--   0        0        0     6749 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/path-params.md
+-rw-r--r--   0        0        0     4920 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/parsing-inputs/query-params.md
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/release-notes.md
+-rw-r--r--   0        0        0       69 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     4130 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/templating/staticfiles.md
+-rw-r--r--   0        0        0    13707 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/templating/templating.md
+-rw-r--r--   0        0        0     7368 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/throttling.md
+-rw-r--r--   0        0        0    12692 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/websockets/index.md
+-rw-r--r--   0        0        0    12912 2023-05-29 23:22:51.630828 ellar-0.4.0/docs/websockets/socketio.md
+-rw-r--r--   0        0        0      143 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/__init__.py
+-rw-r--r--   0        0        0      109 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/__init__.py
+-rw-r--r--   0        0        0     4841 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/_aio_cache.py.ellar
+-rw-r--r--   0        0        0     4361 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/base.py
+-rw-r--r--   0        0        0     5145 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/local_cache.py
+-rw-r--r--   0        0        0      944 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/pylib_cache.py
+-rw-r--r--   0        0        0     2215 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/pymem_cache.py
+-rw-r--r--   0        0        0       72 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/redis/__init__.py
+-rw-r--r--   0        0        0     6548 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/redis/backend.py
+-rw-r--r--   0        0        0     1397 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/backends/serializer.py
+-rw-r--r--   0        0        0     2923 2023-05-29 23:22:51.630828 ellar-0.4.0/ellar/cache/decorator.py
+-rw-r--r--   0        0        0    10943 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/interface.py
+-rw-r--r--   0        0        0     2027 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/make_key_decorator.py
+-rw-r--r--   0        0        0     2501 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/model.py
+-rw-r--r--   0        0        0     1859 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/module.py
+-rw-r--r--   0        0        0      852 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/schema.py
+-rw-r--r--   0        0        0     4489 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/cache/service.py
+-rw-r--r--   0        0        0     3958 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/commands/__init__.py
+-rw-r--r--   0        0        0     2254 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/commands/base.py
+-rw-r--r--   0        0        0     1537 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/commands/decorator.py
+-rw-r--r--   0        0        0      270 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/compatible/__init__.py
+-rw-r--r--   0        0        0     1166 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/compatible/cache_properties.py
+-rw-r--r--   0        0        0     1511 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/compatible/dict.py
+-rw-r--r--   0        0        0      637 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/compatible/emails.py
+-rw-r--r--   0        0        0     4768 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/constants.py
+-rw-r--r--   0        0        0     1670 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/converters.py
+-rw-r--r--   0        0        0      809 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/datastructures.py
+-rw-r--r--   0        0        0      865 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/__init__.py
+-rw-r--r--   0        0        0      485 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/base.py
+-rw-r--r--   0        0        0     7141 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/controller.py
+-rw-r--r--   0        0        0     1036 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/exception.py
+-rw-r--r--   0        0        0      610 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/extra_args.py
+-rw-r--r--   0        0        0     2528 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/file.py
+-rw-r--r--   0        0        0     1025 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/guards.py
+-rw-r--r--   0        0        0     4748 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/html.py
+-rw-r--r--   0        0        0     1084 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/interceptor.py
+-rw-r--r--   0        0        0      648 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/middleware.py
+-rw-r--r--   0        0        0     3105 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/modules.py
+-rw-r--r--   0        0        0      932 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/openapi.py
+-rw-r--r--   0        0        0     1295 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/serializer.py
+-rw-r--r--   0        0        0      402 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/decorators/versioning.py
+-rw-r--r--   0        0        0      840 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/__init__.py
+-rw-r--r--   0        0        0      472 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/api/__init__.py
+-rw-r--r--   0        0        0     1447 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/api/base.py
+-rw-r--r--   0        0        0     1239 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/api/exceptions_types.py
+-rw-r--r--   0        0        0     2498 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/callable_exceptions.py
+-rw-r--r--   0        0        0      103 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/context.py
+-rw-r--r--   0        0        0     2517 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/handlers.py
+-rw-r--r--   0        0        0      598 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/exceptions/validation.py
+-rw-r--r--   0        0        0     1485 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/__init__.py
+-rw-r--r--   0        0        0      658 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/enums.py
+-rw-r--r--   0        0        0      389 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/event_loop.py
+-rw-r--r--   0        0        0     2137 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/importer.py
+-rw-r--r--   0        0        0     1272 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/modelfield.py
+-rw-r--r--   0        0        0      703 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/helper/module_loading.py
+-rw-r--r--   0        0        0      952 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/__init__.py
+-rw-r--r--   0        0        0     3560 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/context.py
+-rw-r--r--   0        0        0      278 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/controller_factory.py
+-rw-r--r--   0        0        0     1356 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/exceptions.py
+-rw-r--r--   0        0        0      400 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/guard_consumer.py
+-rw-r--r--   0        0        0      406 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/interceptor_consumer.py
+-rw-r--r--   0        0        0     1771 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/module.py
+-rw-r--r--   0        0        0      749 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/response_model.py
+-rw-r--r--   0        0        0      908 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/interfaces/templating.py
+-rw-r--r--   0        0        0       52 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/logger.py
+-rw-r--r--   0        0        0      340 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/models/__init__.py
+-rw-r--r--   0        0        0      923 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/models/controller.py
+-rw-r--r--   0        0        0     4258 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/models/guard.py
+-rw-r--r--   0        0        0      320 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/models/interceptor.py
+-rw-r--r--   0        0        0      476 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/__init__.py
+-rw-r--r--   0        0        0    14227 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/base.py
+-rw-r--r--   0        0        0     1615 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/extra_args.py
+-rw-r--r--   0        0        0     2045 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/factory.py
+-rw-r--r--   0        0        0     4252 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/request_model.py
+-rw-r--r--   0        0        0     5893 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/resolver_generators.py
+-rw-r--r--   0        0        0     2457 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/args/websocket_model.py
+-rw-r--r--   0        0        0    10559 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/decorators.py
+-rw-r--r--   0        0        0     1235 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/helpers.py
+-rw-r--r--   0        0        0     9342 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/params.py
+-rw-r--r--   0        0        0     1083 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/__init__.py
+-rw-r--r--   0        0        0     1678 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/base.py
+-rw-r--r--   0        0        0     4460 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/bulk_parameter.py
+-rw-r--r--   0        0        0      768 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/__init__.py
+-rw-r--r--   0        0        0      868 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/background.py
+-rw-r--r--   0        0        0     2961 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/base.py
+-rw-r--r--   0        0        0      391 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/connection.py
+-rw-r--r--   0        0        0      328 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/context.py
+-rw-r--r--   0        0        0     1660 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/inject.py
+-rw-r--r--   0        0        0      387 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/request.py
+-rw-r--r--   0        0        0      394 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/response.py
+-rw-r--r--   0        0        0      524 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/session.py
+-rw-r--r--   0        0        0      386 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/non_parameter/websocket.py
+-rw-r--r--   0        0        0     9544 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/params/resolvers/parameter.py
+-rw-r--r--   0        0        0      415 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/__init__.py
+-rw-r--r--   0        0        0      925 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/__init__.py
+-rw-r--r--   0        0        0     6157 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/base.py
+-rw-r--r--   0        0        0       50 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/exceptions.py
+-rw-r--r--   0        0        0     3129 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/file.py
+-rw-r--r--   0        0        0      691 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/helper.py
+-rw-r--r--   0        0        0     1952 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/html.py
+-rw-r--r--   0        0        0     2383 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/json.py
+-rw-r--r--   0        0        0     4392 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/route.py
+-rw-r--r--   0        0        0     2167 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/models/type_converter.py
+-rw-r--r--   0        0        0      995 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/responses/response_types.py
+-rw-r--r--   0        0        0     1181 2023-05-29 23:22:51.634828 ellar-0.4.0/ellar/common/routing/__init__.py
+-rw-r--r--   0        0        0     4511 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/base.py
+-rw-r--r--   0        0        0      272 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/__init__.py
+-rw-r--r--   0        0        0      877 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/base.py
+-rw-r--r--   0        0        0      689 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/route.py
+-rw-r--r--   0        0        0      190 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/websocket/__init__.py
+-rw-r--r--   0        0        0     1424 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/websocket/handler.py
+-rw-r--r--   0        0        0     1260 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/controller/websocket/route.py
+-rw-r--r--   0        0        0     6589 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/mount.py
+-rw-r--r--   0        0        0    10048 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/operation_definitions.py
+-rw-r--r--   0        0        0     4799 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/route.py
+-rw-r--r--   0        0        0     2985 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/route_collections.py
+-rw-r--r--   0        0        0     3689 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/schema.py
+-rw-r--r--   0        0        0      161 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/websocket/__init__.py
+-rw-r--r--   0        0        0     5680 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/websocket/handler.py
+-rw-r--r--   0        0        0     5158 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/routing/websocket/route.py
+-rw-r--r--   0        0        0      499 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/serializer/__init__.py
+-rw-r--r--   0        0        0     4960 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/serializer/base.py
+-rw-r--r--   0        0        0      194 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/serializer/guard.py
+-rw-r--r--   0        0        0      453 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/shortcuts.py
+-rw-r--r--   0        0        0      613 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/__init__.py
+-rw-r--r--   0        0        0      472 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/environment.py
+-rw-r--r--   0        0        0     1634 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/loader.py
+-rw-r--r--   0        0        0     2895 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/model.py
+-rw-r--r--   0        0        0     2482 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/renderer.py
+-rw-r--r--   0        0        0      110 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/templating/schema.py
+-rw-r--r--   0        0        0      585 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/common/types.py
+-rw-r--r--   0        0        0      925 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/conf/__init__.py
+-rw-r--r--   0        0        0     4914 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/conf/app_settings_models.py
+-rw-r--r--   0        0        0     2177 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/conf/config.py
+-rw-r--r--   0        0        0     5122 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/conf/mixins.py
+-rw-r--r--   0        0        0      470 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/connection/__init__.py
+-rw-r--r--   0        0        0      688 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/connection/http.py
+-rw-r--r--   0        0        0      245 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/connection/websocket.py
+-rw-r--r--   0        0        0      458 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/execution.py
+-rw-r--r--   0        0        0     2607 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/factory.py
+-rw-r--r--   0        0        0     2091 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/host.py
+-rw-r--r--   0        0        0     2122 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/http.py
+-rw-r--r--   0        0        0      817 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/context/websocket.py
+-rw-r--r--   0        0        0     1829 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/core_service_registration.py
+-rw-r--r--   0        0        0       97 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     2273 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/exceptions/service.py
+-rw-r--r--   0        0        0     7616 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/factory.py
+-rw-r--r--   0        0        0      320 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/guard/__init__.py
+-rw-r--r--   0        0        0      744 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/guard/apikey.py
+-rw-r--r--   0        0        0     1729 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/guard/consumer.py
+-rw-r--r--   0        0        0     3318 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/guard/http.py
+-rw-r--r--   0        0        0       87 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/interceptors/__init__.py
+-rw-r--r--   0        0        0     2083 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/interceptors/consumer.py
+-rw-r--r--   0        0        0     9940 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/main.py
+-rw-r--r--   0        0        0     1159 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/__init__.py
+-rw-r--r--   0        0        0     2600 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/di.py
+-rw-r--r--   0        0        0     2704 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/exceptions.py
+-rw-r--r--   0        0        0     2256 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/function.py
+-rw-r--r--   0        0        0      121 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/sessions.py
+-rw-r--r--   0        0        0     1095 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/middleware/versioning.py
+-rw-r--r--   0        0        0      321 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/__init__.py
+-rw-r--r--   0        0        0     1287 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/base.py
+-rw-r--r--   0        0        0     3143 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/builder.py
+-rw-r--r--   0        0        0     5827 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/config.py
+-rw-r--r--   0        0        0      787 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/helper.py
+-rw-r--r--   0        0        0     9876 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/modules/ref.py
+-rw-r--r--   0        0        0      351 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/__init__.py
+-rw-r--r--   0        0        0     3661 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/app.py
+-rw-r--r--   0        0        0     1865 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/builder.py
+-rw-r--r--   0        0        0     1862 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/factory.py
+-rw-r--r--   0        0        0     1971 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/helper.py
+-rw-r--r--   0        0        0      794 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/routing/module_router.py
+-rw-r--r--   0        0        0       58 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/services/__init__.py
+-rw-r--r--   0        0        0     1951 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/services/reflector.py
+-rw-r--r--   0        0        0     1718 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/staticfiles.py
+-rw-r--r--   0        0        0       67 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/templating/__init__.py
+-rw-r--r--   0        0        0     3978 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/templating/app.py
+-rw-r--r--   0        0        0      563 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/versioning/__init__.py
+-rw-r--r--   0        0        0     2526 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/versioning/base.py
+-rw-r--r--   0        0        0     6040 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/core/versioning/resolver.py
+-rw-r--r--   0        0        0      915 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/di/__init__.py
+-rw-r--r--   0        0        0      344 2023-05-29 23:22:51.638828 ellar-0.4.0/ellar/di/asgi_args.py
+-rw-r--r--   0        0        0     1073 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/constants.py
+-rw-r--r--   0        0        0      400 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/exceptions.py
+-rw-r--r--   0        0        0      117 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/injector/__init__.py
+-rw-r--r--   0        0        0     7619 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/injector/container.py
+-rw-r--r--   0        0        0     5268 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/injector/ellar_injector.py
+-rw-r--r--   0        0        0      845 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/providers.py
+-rw-r--r--   0        0        0     2247 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/scopes.py
+-rw-r--r--   0        0        0     4533 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/service_config.py
+-rw-r--r--   0        0        0       39 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/types.py
+-rw-r--r--   0        0        0      244 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/di/utils.py
+-rw-r--r--   0        0        0     2052 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/events.py
+-rw-r--r--   0        0        0      573 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/__init__.py
+-rw-r--r--   0        0        0     8069 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/builder.py
+-rw-r--r--   0        0        0      239 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/docs_generators/__init__.py
+-rw-r--r--   0        0        0      530 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/docs_generators/base.py
+-rw-r--r--   0        0        0      959 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/docs_generators/redocs.py
+-rw-r--r--   0        0        0     1025 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/docs_generators/swagger.py
+-rw-r--r--   0        0        0     2937 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/module.py
+-rw-r--r--   0        0        0    10611 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/openapi_v3.py
+-rw-r--r--   0        0        0    15879 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/route_doc_models.py
+-rw-r--r--   0        0        0      115 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/schemas/__init__.py
+-rw-r--r--   0        0        0      342 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/schemas/validation.py
+-rw-r--r--   0        0        0      702 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/templates/redocs.html
+-rw-r--r--   0        0        0      758 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/openapi/templates/swagger.html
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/py.typed
+-rw-r--r--   0        0        0      180 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/reflect/__init__.py
+-rw-r--r--   0        0        0     5356 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/reflect/_reflect.py
+-rw-r--r--   0        0        0       34 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/reflect/constants.py
+-rw-r--r--   0        0        0      238 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/reflect/contextmanager_fix.py
+-rw-r--r--   0        0        0       58 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/controllers/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/controllers/home.py
+-rw-r--r--   0        0        0      211 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/modules.py
+-rw-r--r--   0        0        0   155845 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/static/css/bootstrap.min.css
+-rwxr-xr-x   0        0        0    25915 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/static/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/static/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0     3888 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/static/img/Icon.svg
+-rw-r--r--   0        0        0     1312 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/samples/templates/home/index.html
+-rw-r--r--   0        0        0      596 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/adapter.py
+-rw-r--r--   0        0        0      524 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/constants.py
+-rw-r--r--   0        0        0     1659 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/context.py
+-rw-r--r--   0        0        0      225 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/decorators/__init__.py
+-rw-r--r--   0        0        0      667 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/decorators/events.py
+-rw-r--r--   0        0        0     3846 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/decorators/gateway.py
+-rw-r--r--   0        0        0      578 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/decorators/subscribe_message.py
+-rw-r--r--   0        0        0     2511 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/factory.py
+-rw-r--r--   0        0        0     9627 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/gateway.py
+-rw-r--r--   0        0        0      144 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/model.py
+-rw-r--r--   0        0        0      465 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/responses.py
+-rw-r--r--   0        0        0      107 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/testing/__init__.py
+-rw-r--r--   0        0        0     1704 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/socket_io/testing/module.py
+-rw-r--r--   0        0        0      129 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/testing/__init__.py
+-rw-r--r--   0        0        0     4074 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/testing/module.py
+-rw-r--r--   0        0        0     1215 2023-05-29 23:22:51.642828 ellar-0.4.0/ellar/testing/uvicorn_server.py
+-rw-r--r--   0        0        0      509 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/__init__.py
+-rw-r--r--   0        0        0     1659 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/controllers.py
+-rw-r--r--   0        0        0     1077 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/module.py
+-rw-r--r--   0        0        0     1146 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/routers.py
+-rw-r--r--   0        0        0      629 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/schemas.py
+-rw-r--r--   0        0        0      666 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/services.py
+-rw-r--r--   0        0        0     1708 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/blog/blog.css
+-rw-r--r--   0        0        0     1586 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css
+-rw-r--r--   0        0        0     1008 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg
+-rw-r--r--   0        0        0     2047 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/__init__.py
+-rw-r--r--   0        0        0     2900 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_controllers.py
+-rw-r--r--   0        0        0     1604 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_routers.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.642828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_services.py
+-rw-r--r--   0        0        0      202 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/views/car/list.html
+-rw-r--r--   0        0        0      202 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/views/cat/list.html
+-rw-r--r--   0        0        0    15257 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/apps/car/views/index.html
+-rw-r--r--   0        0        0      216 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/commands.py
+-rw-r--r--   0        0        0      187 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/config.py
+-rw-r--r--   0        0        0      598 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/root_module.py
+-rw-r--r--   0        0        0      954 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/server.py
+-rw-r--r--   0        0        0      134 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/carapp/tests/conftest.py
+-rw-r--r--   0        0        0      241 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/01-carapp/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/README.md
+-rw-r--r--   0        0        0      283 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/__init__.py
+-rw-r--r--   0        0        0      455 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/controllers.py
+-rw-r--r--   0        0        0     2182 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/gateways.py
+-rw-r--r--   0        0        0     1005 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/module.py
+-rw-r--r--   0        0        0      295 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/routers.py
+-rw-r--r--   0        0        0      542 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/schemas.py
+-rw-r--r--   0        0        0      179 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/services.py
+-rw-r--r--   0        0        0     3829 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/templates/events/index.html
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/tests/test_controllers.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/tests/test_routers.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/tests/test_services.py
+-rw-r--r--   0        0        0     2602 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/config.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/domain/__init__.py
+-rw-r--r--   0        0        0      480 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/root_module.py
+-rw-r--r--   0        0        0     1045 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/socketio_app/server.py
+-rw-r--r--   0        0        0       43 2023-05-29 23:22:51.646828 ellar-0.4.0/examples/02-socketio-app/tests/conftest.py
+-rw-r--r--   0        0        0     3872 2023-05-29 23:22:51.646828 ellar-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      597 2023-05-29 23:22:51.646828 ellar-0.4.0/mypy.ini
+-rw-r--r--   0        0        0     3037 2023-05-29 23:22:51.646828 ellar-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-05-29 23:22:51.646828 ellar-0.4.0/pytest.ini
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      616 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/injector_module.py
+-rw-r--r--   0        0        0     5249 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/main.py
+-rw-r--r--   0        0        0       23 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/private/test.css
+-rw-r--r--   0        0        0      748 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/schema.py
+-rw-r--r--   0        0        0        4 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/statics/example.txt
+-rw-r--r--   0        0        0      160 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/ellar/index.html
+-rw-r--r--   0        0        0      102 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/ellar/list.html
+-rw-r--r--   0        0        0      129 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/index.html
+-rw-r--r--   0        0        0      128 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/list.html
+-rw-r--r--   0        0        0       65 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/templates/render_string.html
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/config.py
+-rw-r--r--   0        0        0     2854 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/sample.py
+-rw-r--r--   0        0        0     3548 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_application_factory.py
+-rw-r--r--   0        0        0    15855 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_application_functions.py
+-rw-r--r--   0        0        0    18052 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_cors.py
+-rw-r--r--   0        0        0     4352 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_replacing_app_services.py
+-rw-r--r--   0        0        0     2329 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_application/test_trusted_host.py
+-rw-r--r--   0        0        0      862 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_attribute_dict.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/__init__.py
+-rw-r--r--   0        0        0     3625 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/_test_aio_memcache.py.ellar
+-rw-r--r--   0        0        0     1893 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/pylib_mock.py
+-rw-r--r--   0        0        0     2592 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/redis_mock.py
+-rw-r--r--   0        0        0     2764 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_cache_decorator.py
+-rw-r--r--   0        0        0     1744 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_cache_many_config.py
+-rw-r--r--   0        0        0     4772 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_cache_service.py
+-rw-r--r--   0        0        0     4995 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_local_cache.py
+-rw-r--r--   0        0        0      596 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_module_setup.py
+-rw-r--r--   0        0        0     9973 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_pylibmc_cache.py
+-rw-r--r--   0        0        0     6093 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_redis_cache.py
+-rw-r--r--   0        0        0      577 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_cache/test_schema.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_conf/__init__.py
+-rw-r--r--   0        0        0     5223 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_conf/test_default_conf.py
+-rw-r--r--   0        0        0     1151 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_conf/test_mixins.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/sample.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_application_router.py
+-rw-r--r--   0        0        0     4448 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_controller_decorator.py
+-rw-r--r--   0        0        0     2872 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_controller_inheritance.py
+-rw-r--r--   0        0        0     2722 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_module_router.py
+-rw-r--r--   0        0        0     7186 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_controller/test_route_collection.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/__init__.py
+-rw-r--r--   0        0        0     3366 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_controller.py
+-rw-r--r--   0        0        0      789 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_exception.py
+-rw-r--r--   0        0        0     3508 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_file.py
+-rw-r--r--   0        0        0     1059 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_guards.py
+-rw-r--r--   0        0        0     4082 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_html.py
+-rw-r--r--   0        0        0      554 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_middleware.py
+-rw-r--r--   0        0        0     2061 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_modules.py
+-rw-r--r--   0        0        0      915 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_openapi.py
+-rw-r--r--   0        0        0     1311 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_serializer.py
+-rw-r--r--   0        0        0      475 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_decorators/test_versioning.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/examples.py
+-rw-r--r--   0        0        0     2078 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/test_injectable_resolving.py
+-rw-r--r--   0        0        0     6275 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/test_injector.py
+-rw-r--r--   0        0        0     3508 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/test_provider_scopes.py
+-rw-r--r--   0        0        0     3993 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_di/test_providers.py
+-rw-r--r--   0        0        0     2094 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_events.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/exception_runner.py
+-rw-r--r--   0        0        0     2562 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/test_api_exception.py
+-rw-r--r--   0        0        0     8609 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/test_custom_exceptions.py
+-rw-r--r--   0        0        0     1195 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/test_error_details.py
+-rw-r--r--   0        0        0     3722 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_exceptions/test_validation_exception.py
+-rw-r--r--   0        0        0     7585 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_guard.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/__init__.py
+-rw-r--r--   0        0        0      571 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/test_enum.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/test_importer.py
+-rw-r--r--   0        0        0      795 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/test_model_field.py
+-rw-r--r--   0        0        0      298 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_helper/test_module_loading.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.646828 ellar-0.4.0/tests/test_interceptors/__init__.py
+-rw-r--r--   0        0        0     2945 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_interceptors/test_interceptor.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_middleware/__init__.py
+-rw-r--r--   0        0        0     3100 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_middleware/test_functional_middleware.py
+-rw-r--r--   0        0        0     4243 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_middleware/test_service_provider_middleware.py
+-rw-r--r--   0        0        0     2168 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_middleware/test_versioning_middleware.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_modules/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_modules/sample.py
+-rw-r--r--   0        0        0     6760 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_modules/test_module_config.py
+-rw-r--r--   0        0        0    10234 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_modules/test_module_ref.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_openapi/__init__.py
+-rw-r--r--   0        0        0     8341 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_openapi/test_builder.py
+-rw-r--r--   0        0        0     6680 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_openapi/test_module.py
+-rw-r--r--   0        0        0    16536 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_openapi/test_open_api_route_documentation.py
+-rw-r--r--   0        0        0     5571 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_reflect.py
+-rw-r--r--   0        0        0     2287 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_reflector.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_defined_response_model.py
+-rw-r--r--   0        0        0     4562 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_pydantic_response_model.py
+-rw-r--r--   0        0        0     3393 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_response_file.py
+-rw-r--r--   0        0        0     5063 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_response_html.py
+-rw-r--r--   0        0        0     3228 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_response_streaming.py
+-rw-r--r--   0        0        0     3902 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_response_type_definition_converter.py
+-rw-r--r--   0        0        0     3524 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_response/test_route_response_model.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/__init__.py
+-rw-r--r--   0        0        0     1126 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/sample.py
+-rw-r--r--   0        0        0     2757 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_background_tasks.py
+-rw-r--r--   0        0        0     3605 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_body_schema.py
+-rw-r--r--   0        0        0     3666 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_body_schema_extra_properties.py
+-rw-r--r--   0        0        0     4142 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_body_union_schema.py
+-rw-r--r--   0        0        0     4066 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_cookie_schema.py
+-rw-r--r--   0        0        0     6854 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_extra_args.py
+-rw-r--r--   0        0        0     2457 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_form_schema.py
+-rw-r--r--   0        0        0    10018 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_formparsers.py
+-rw-r--r--   0        0        0     1282 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_forms.py
+-rw-r--r--   0        0        0     1296 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0     3633 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_header_schema.py
+-rw-r--r--   0        0        0     1887 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_invalid_path_param.py
+-rw-r--r--   0        0        0     2006 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     5205 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_multi_body_errors.py
+-rw-r--r--   0        0        0     3783 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_multi_query_errors.py
+-rw-r--r--   0        0        0     9423 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_path.py
+-rw-r--r--   0        0        0     2933 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_path_with_schema.py
+-rw-r--r--   0        0        0     3333 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_put_with_no_body_schema.py
+-rw-r--r--   0        0        0     2242 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_query.py
+-rw-r--r--   0        0        0     3699 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_query_schema.py
+-rw-r--r--   0        0        0     1987 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_request.py
+-rw-r--r--   0        0        0     3415 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_routing/test_route_endpoint_params.py
+-rw-r--r--   0        0        0      451 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_sample_project.py
+-rw-r--r--   0        0        0     2712 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_schema.py
+-rw-r--r--   0        0        0     6379 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_serializer.py
+-rw-r--r--   0        0        0      775 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_shortcuts.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/__init__.py
+-rw-r--r--   0        0        0     4116 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/sample.py
+-rw-r--r--   0        0        0      718 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_decorators/test_events.py
+-rw-r--r--   0        0        0     3598 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_decorators/test_gateway.py
+-rw-r--r--   0        0        0      719 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_decorators/test_subcribe_message.py
+-rw-r--r--   0        0        0      859 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_gateway.py
+-rw-r--r--   0        0        0     8889 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_socket_io/test_operation.py
+-rw-r--r--   0        0        0    14104 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_staticfiles.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/module_statics/watever.txt
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/static/watever.txt
+-rw-r--r--   0        0        0      167 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/templates/watever.html
+-rw-r--r--   0        0        0     2904 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/test_module_templating.py
+-rw-r--r--   0        0        0     2718 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/test_renderer.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_templating/views/watever.html
+-rw-r--r--   0        0        0     2425 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_testing.py
+-rw-r--r--   0        0        0        0 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/__init__.py
+-rw-r--r--   0        0        0     1968 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/operations.py
+-rw-r--r--   0        0        0     2138 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_default_versioning.py
+-rw-r--r--   0        0        0     4449 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_default_versioning_for_controllers.py
+-rw-r--r--   0        0        0     4475 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_header_versioning.py
+-rw-r--r--   0        0        0     7820 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_header_versioning_controller.py
+-rw-r--r--   0        0        0     3823 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_host_versioning.py
+-rw-r--r--   0        0        0     3227 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_query_versioning.py
+-rw-r--r--   0        0        0     2865 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_versioning/test_url_versioning.py
+-rw-r--r--   0        0        0    17496 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_websocket.py
+-rw-r--r--   0        0        0    11181 2023-05-29 23:22:51.650828 ellar-0.4.0/tests/test_websocket_handler.py
+-rw-r--r--   0        0        0    14698 1970-01-01 00:00:00.000000 ellar-0.4.0/PKG-INFO
```

### Comparing `ellar-0.3.8/.github/workflows/publish.yml` & `ellar-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/.github/workflows/test.yml` & `ellar-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/.github/workflows/test_full.yml` & `ellar-0.4.0/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/.gitignore` & `ellar-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/.pre-commit-config.yaml` & `ellar-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/LICENSE` & `ellar-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/Makefile` & `ellar-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/README.md` & `ellar-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -291,9 +291,8 @@
 ```
 
 See the [Doc](https://eadwincode.github.io/ellar/templating/templating/) for more examples.
 
 ## Project Status
 Project is still in development
 - Documentation - (in progress)
-- Interceptors  -  [Aspect Oriented Programming](https://en.wikipedia.org/wiki/Aspect-oriented_programming) (AOP) technique
 - Database Plugin with [Encode/ORM](https://github.com/encode/orm)
```

### Comparing `ellar-0.3.8/docs/basics/execution-context.md` & `ellar-0.4.0/docs/basics/execution-context.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# **Execution Context**
 Execution context refers to the current context of execution, or the environment in which a specific piece of code is running. 
 It contains information about the current request, the current response in the case of http connection, and the current state of the application.
 
 The execution context is created automatically when a request is received, and it is passed along through the various layers of the application as the request is handled. 
 This allows different components of the application like **exception handlers**, **functional middlewares** and **guards** to access information about the current request.
 
 There are two class `HostContext` and `ExecutionContext` which provides set of methods and properties for accessing and manipulating the current context of execution.
@@ -262,24 +263,24 @@
 ```
 
 Next, we apply the `RoleGuard` to `CarController`
 
 ```python
 # project_name/apps/cars/controllers.py
 import typing
-from ellar.common import Body, Controller, post, set_metadata, Guards, ControllerBase
+from ellar.common import Body, Controller, post, set_metadata, UseGuards, ControllerBase
 from .schemas import CreateCarSerializer
 from .guards import RoleGuard
 
 def roles(*_roles: str) -> typing.Callable:
     return set_metadata('roles', list(_roles))
 
 
 @Controller('/car')
-@Guards(RoleGuard)
+@UseGuards(RoleGuard)
 class CarController(ControllerBase):
     @post()
     @roles('admin', 'is_staff')
     async def create(self, payload: CreateCarSerializer = Body()):
         result = payload.dict()
         result.update(message='This action adds a new car')
         return result
```

### Comparing `ellar-0.3.8/docs/basics/testing.md` & `ellar-0.4.0/docs/basics/testing.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+# **Testing**
 Automated testing is the practice of using software tools to automatically run tests on a software application or system, 
 rather than relying on manual testing by humans. It is considered an essential part of software development as it 
 helps increase productivity, ensure quality and performance goals are met, and provide faster feedback loops to developers. 
 Automated tests can include various types such as unit tests, integration tests, end-to-end tests, and more. 
 
 While setting up automated tests can be tedious, the benefits of increased test coverage and productivity make it an important aspect of software development.
 Ellar aims to encourage the use of development best practices, including effective testing, by providing various features to assist developers and teams in creating and automating tests. 
 These features include:
 
 - automatically generated default unit tests files for components testing
-- offering a util, `TestClientFactory`, that constructs an isolated module/application setup
+- offering a util, `Test` Factory class, that constructs an isolated module/application setup
 - making the Ellar dependency injection system accessible in the testing environment for convenient component mocking.
 
 Ellar is compatible with `unittest` and `pytest` testing frameworks in python but in this documentation, we will be using `pytest`.
 
 ## **Getting started**
 You will need to install `pytest`
 
@@ -147,32 +148,32 @@
     def setup(self):
         test_module = Test.create_test_module(
             controllers=[CarController,]
         ).override_provider(CarRepository, use_value=MockCarRepository())
 ```
 We this, anywhere `CarRepository` is needed, a `MockCarRepository()` instance will be applied.
 
-In same way, we can override `Guards` used in controllers during testing. For example, lets assume `CarController` has a guard `JWTGuard`
+In same way, we can override `UseGuards` used in controllers during testing. For example, lets assume `CarController` has a guard `JWTGuard`
 
 ```python
 import typing
 from ellar.common.compatible import AttributeDict
-from ellar.common import Guards, Controller, ControllerBase
+from ellar.common import UseGuards, Controller, ControllerBase
 from ellar.core.guard import HttpBearerAuth
 from ellar.di import injectable
 
 
 @injectable()
 class JWTGuard(HttpBearerAuth):
     async def authenticate(self, connection, credentials) -> typing.Any:
         # JWT verification goes here
         return AttributeDict(is_authenticated=True, first_name='Ellar', last_name='ASGI Framework') 
 
 
-@Guards(JWTGuard)
+@UseGuards(JWTGuard)
 @Controller('/car')
 class CarController(ControllerBase):
     ...
 ```
 During testing, we can replace `JWTGuard` with a `MockAuthGuard` as shown below.
 
 ```python
```

### Comparing `ellar-0.3.8/docs/basics/versioning.md` & `ellar-0.4.0/docs/basics/versioning.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# **Versioning**
 Versioning allows for the existence of multiple versions of controllers or individual routes within the same application, 
 which can be useful when making changes that may break previous versions. 
 This allows developers to support older versions of the application while still making necessary updates.
 
 There are 4 types of versioning that are supported:
 
 - [`URL Versioning`](#url-versioning): The version will be passed within the **URL** of the request
```

### Comparing `ellar-0.3.8/docs/caching.md` & `ellar-0.4.0/docs/caching.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+# **Caching**
 Caching refers to the process of storing frequently accessed data in a temporary storage area called a `cache`, 
 in order to speed up access to that data in the future.
 
 In computing, caching is used to optimize the performance of applications and systems by reducing the time it takes to retrieve data from slower or more distant storage. 
 By caching data in a faster, more local storage location, the system can quickly retrieve the data without needing to go all the way to the original source of the data.
 
 In Ellar, we provided several cache backends interface that interacts with different cache types to assist in cache endpoint responses or other relevant data.
 
-## Setting up the cache
+## **Setting up the cache**
 It's very simple to set up cache in Ellar but the crucial part is picking the cache type that is suitable for your application 
 because some cache type behave differently and perform better and faster than others.
 
 To set up cache, we need to use `CacheModule`. `CacheModule` provides two methods, `CacheModule.register_setup` and `CacheModule.setup`, for setting up `cache` in ellar applications.
 
 === "CacheModule Register Setup"
     This setup method requires you to defined `CACHES` variable containing 
@@ -292,15 +293,15 @@
 
 class DevelopmentConfig(ConfigDefaultTypesMixin):
     CACHES = {
         'default': CustomCacheBackend()
     }
 ```
 
-## Cache Arguments
+## **Cache Arguments**
 
 You can customize the behavior of each caching backend in Django by passing additional arguments when you configure the cache. The valid arguments that can be passed to each backend are as follows:
 
 - **TIMEOUT**: The default timeout, in seconds, to use for the cache. This argument defaults to **300** seconds (5 minutes). You can set **TIMEOUT** to None so that, by default, cache keys never expire. A value of 0 causes keys to immediately expire
 - **OPTIONS**: Any options that should be passed to the cache backend. The list of valid options will vary with each backend.
 - **KEY_PREFIX**: A string that will be automatically prepended to all cache keys.
 - **VERSION**: The default version number for cache keys.
@@ -319,15 +320,15 @@
             ttl=300, 
             version=1, 
             key_prefix='project_name'
         )
     }
 ```
 
-## Setting up More than One Cache Backend
+## **Setting up More than One Cache Backend**
 To set up multiple cache backends in Django, you can add additional entries to the `CACHES` variable in your `config.py` file. 
 The `default` cache backend is typically defined first, followed by any additional cache backends you want to configure.
 
 Here's an example `CACHES` setting that defines two cache backends:
 
 ```python
 # project_name/config.py
@@ -339,15 +340,15 @@
 class DevelopmentConfig(ConfigDefaultTypesMixin):
     CACHES = {
         'default': RedisCacheBackend(servers=['redis://127.0.0.1:6379'], key_prefix='project_name'),
         'secondary': LocalMemCacheBackend(ttl=300, key_prefix='project_name', version=1)
     }
 ```
  
-## CacheService (ICacheService)
+## **CacheService (ICacheService)**
 Ellar does not provide cache backends directly, but instead offers a caching service that manages all the configured cache backends in your application. 
 The `CacheService` class serves as a wrapper for these cache backends and provides a uniform interface for interacting with them.
 
 The `CacheService` class can be injected into your application's code as a dependency, allowing you to use it throughout your application without the need for direct instantiation. 
 This approach promotes a more modular and extensible design, as well as better testability of your code.
 
 The CacheService class provides methods like:
@@ -370,15 +371,15 @@
 - **decr_async**_**(key: str, delta: int = 1, version: str = None, backend: str = None)**_: asynchronous version of `decr` action
 
 !!! note
     If `backend=None`, `default` backend configuration is used.
 
 These methods are available for each of the configured cache backends and can be used interchangeably with any backend.
 
-## Injecting CacheService
+## **Injecting CacheService**
 `CacheService` is a core service registered in `EllarInjector` and can be injected as every other service.
 
 For example, lets make `CacheService` available in our route function.
 
 === "Synchronous Route Function"
     ```python
     from ellar.common import get, Provide
@@ -407,30 +408,30 @@
             return cached_value
         processed_value = 'some-value'
         await cache_service.set_async('my-key', processed_value, timeout=300) # for 5mins
         return processed_value
     ```
 
 
-## Using Cache Decorator
+## **Using Cache Decorator**
 Ellar provides a cache decorator that can be used to cache the responses of route functions. The cache decorator can be applied to a route function to automatically cache its response data for a specified amount of time.
 
 The cache decorator takes the following arguments:
 
 - `ttl`(time to live): the amount of time (in seconds) for which the response data should be cached.
 - `key_prefix` (optional): a string that is used to prefix the cache key, allowing for easy differentiation between different cache items.
 - `version` (optional): a string that is used to version the cache key, allowing for cache invalidation when the data schema changes.
 - `backend` (optional): the name of the cache backend to use for storing the cached data. By default, the `default` cache backend is used.
 - `make_key_callback` (optional): a callback function that can be used to generate a custom cache key. This function takes an `IExecutionContext` instance (which contains information about the request context) and key prefix, and should return the custom cache key to use.
 
 We can rewrite the above example using `cache` decorator:
 === "Synchronous Route Function"
     ```python
-    from ellar.common import get, cache
-    
+    from ellar.common import get
+    from ellar.cache import cache
     ...
     @get('/cache-test')
     @cache(ttl=300, version='v1', key_prefix='project_name')
     def my_route_function(self):
         processed_value = 'some-value'
         return processed_value
     ```
@@ -442,24 +443,25 @@
     @get('/cache-test')
     @cache(ttl=300, version='v1', key_prefix='project_name')
     async def my_route_function(self):
         processed_value = 'some-value'
         return processed_value
     ```
 
-### Adding Custom key gen function for cache Decorator
+### **Adding Custom key gen function for cache Decorator**
 By default, the `cache` decorator combines the route function's URL and the specified `key_prefix` value to generate the cache key used to store the response data. 
 However, you can customize this behavior by providing a `make_key_callback` function to the cache decorator.
 
 The `make_key_callback` function takes an `ExecutionContext` instance (which contains information about the request context) and the `key_prefix` value as input, and should return the custom cache key to use.
 
 Here's an example of how to use a custom `make_key_callback` function with the cache decorator:
 === "Synchronous Route Function"
     ```python
-    from ellar.common import get, cache
+    from ellar.common import get
+    from ellar.cache import cache
     from ellar.core import ExecutionContext
     from ellar.common.helper import get_name
     
     def make_key_function(ctx: ExecutionContext, key_prefix: str) -> str:
         function_name = get_name(ctx.get_handler())
         return "%s:%s:%s" % (function_name, key_prefix, ctx.switch_to_http_connection().get_client().url)
     
@@ -471,15 +473,16 @@
         processed_value = 'some-value'
         return processed_value
     ...
     ```
 === "Asynchronous Route Function"
     
     ```python
-    from ellar.common import get, cache
+    from ellar.common import get
+    from ellar.cache import cache
     from ellar.core import ExecutionContext
     from ellar.common.helper import get_name
     
     def make_key_function(ctx: ExecutionContext, key_prefix: str) -> str:
         function_name = get_name(ctx.get_handler())
         return "%s:%s:%s" % (function_name, key_prefix, ctx.switch_to_http_connection().get_client().url)
```

### Comparing `ellar-0.3.8/docs/commands/command-grouping.md` & `ellar-0.4.0/docs/commands/command-grouping.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/commands/create-module-command.md` & `ellar-0.4.0/docs/commands/create-module-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/commands/custom-commands.md` & `ellar-0.4.0/docs/commands/custom-commands.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/commands/index.md` & `ellar-0.4.0/docs/commands/index.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/commands/new-command.md` & `ellar-0.4.0/docs/commands/new-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/commands/runserver-command.md` & `ellar-0.4.0/docs/commands/runserver-command.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/configurations.md` & `ellar-0.4.0/docs/configurations.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# **Application Configurations**
 
 The `config.py` file contains all the configuration necessary in bootstrapping ellar application. 
 
 Lets in this section go through the different configuration available.
 
 ## **Configuration Variables**
 ### **SECRET_KEY**
```

### Comparing `ellar-0.3.8/docs/custom-setup.md` & `ellar-0.4.0/docs/custom-setup.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/handling-response/response-model.md` & `ellar-0.4.0/docs/handling-response/response-model.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,58 +131,58 @@
 
 ## Different Response Models 
 Let's see different `ResponseModel` available in Ellar and how you can create one too.
 
 ### **ResponseModel** 
 Response model that manages rendering of other response types.
 
-- Location: `ellar.core.response.model.base.ResponseModel`
+- Location: `ellar.common.responses.models.ResponseModel`
 - response_type: `Response`
 - model_field_or_schema: `None`
 - media_type: `text/plain`
 
 ### **JSONResponseModel** 
 Response model that manages `JSON` response.
 
-- Location: `ellar.core.response.model.json.JSONResponseModel`
+- Location: `ellar.common.responses.models.json.JSONResponseModel`
 - response_type: `JSONResponse` OR `config.DEFAULT_JSON_CLASS`
 - model_field_or_schema: `Required`
 - media_type: `application/json`
 
 ### **HTMLResponseModel** 
 Response model that manages `HTML` templating response. see [`@render`]() decorator.
 
-- Location: `ellar.core.response.model.html.HTMLResponseModel`
+- Location: `ellar.common.responses.models.html.HTMLResponseModel`
 - response_type: `TemplateResponse`
 - model_field_or_schema: `None`
 - media_type: `text/html`
 
 
 ### **FileResponseModel** 
 Response model that manages `FILE` response. see [`@file`]() decorator.
 
-- Location: `ellar.core.response.model.file.FileResponseModel`
+- Location: `ellar.common.responses.models.file.FileResponseModel`
 - response_type: `FileResponse`
 - model_field_or_schema: `None`
 - media_type: `Required`
 
 
 ### **StreamingResponseModel** 
 Response model that manages `STREAMING` response. see [`@file`]() decorator.
 
-- Location: `ellar.core.response.model.file.StreamingResponseModel`
+- Location: `ellar.common.responses.models.file.StreamingResponseModel`
 - response_type: `StreamingResponse`
 - model_field_or_schema: `None`
 - media_type: `Required`
 
 
 ### **EmptyAPIResponseModel**
 Default `ResponseModel` applied when no response is defined.
 
-- Location: `ellar.core.response.model.html.EmptyAPIResponseModel`
+- Location: `ellar.common.responses.models.json.EmptyAPIResponseModel`
 - response_type: `JSONResponse` OR `config.DEFAULT_JSON_CLASS`
 - model_field_or_schema: `dict`
 - media_type: `application/json`
 
 ## Custom Response Model
 
 Lets create a new JSON response model.
```

### Comparing `ellar-0.3.8/docs/handling-response/response.md` & `ellar-0.4.0/docs/handling-response/response.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/EllarLogoB.png` & `ellar-0.4.0/docs/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/EllarLogoIconOnly.png` & `ellar-0.4.0/docs/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/EllarLogoW.png` & `ellar-0.4.0/docs/img/EllarLogoW.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/Icon.svg` & `ellar-0.4.0/docs/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/Logo.svg` & `ellar-0.4.0/docs/img/Logo.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/ModuleDescription.png` & `ellar-0.4.0/docs/img/ModuleDescription.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/body-schema-doc.png` & `ellar-0.4.0/docs/img/body-schema-doc.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/body-schema-doc2.png` & `ellar-0.4.0/docs/img/body-schema-doc2.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/body-schema-doc3.png` & `ellar-0.4.0/docs/img/body-schema-doc3.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/car_api.png` & `ellar-0.4.0/docs/img/car_api.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/car_controller.gif` & `ellar-0.4.0/docs/img/car_controller.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/controller_description.png` & `ellar-0.4.0/docs/img/controller_description.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/create-car-schema.png` & `ellar-0.4.0/docs/img/create-car-schema.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/create-dog-schema.png` & `ellar-0.4.0/docs/img/create-dog-schema.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/ellar_demo.gif` & `ellar-0.4.0/docs/img/ellar_demo.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/ellar_framework.png` & `ellar-0.4.0/docs/img/ellar_framework.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/enum_docs_swagger.png` & `ellar-0.4.0/docs/img/enum_docs_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/event_docs_swagger.png` & `ellar-0.4.0/docs/img/event_docs_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/form-schema-doc.png` & `ellar-0.4.0/docs/img/form-schema-doc.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/json_api_response_model.png` & `ellar-0.4.0/docs/img/json_api_response_model.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/live_support_websocket.gif` & `ellar-0.4.0/docs/img/live_support_websocket.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/live_support_websocket_3.gif` & `ellar-0.4.0/docs/img/live_support_websocket_3.gif`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/math_router.png` & `ellar-0.4.0/docs/img/math_router.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/math_router_with_request_object.png` & `ellar-0.4.0/docs/img/math_router_with_request_object.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/middleware.png` & `ellar-0.4.0/docs/img/middleware.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/query_filter_swagger.png` & `ellar-0.4.0/docs/img/query_filter_swagger.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/img/response_description.png` & `ellar-0.4.0/docs/img/response_description.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/index.md` & `ellar-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/overview/controllers.md` & `ellar-0.4.0/docs/overview/controllers.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# **Controllers**
 The Controller is responsible for handling incoming requests and returning responses to the client.
 The purpose of a controller is to receive specific requests for an application `ApplicationRouter`. `ApplicationRouter` on the other hand, decides which `controller` should handle an incoming request.
 
 ![controller description image](../img/controller_description.png)
 
 Controllers can be said to be a router with many routes registered in them.
```

### Comparing `ellar-0.3.8/docs/overview/custom_decorators.md` & `ellar-0.4.0/docs/overview/custom_decorators.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# **Custom Decorators**
 Ellar provides a variety of function decorators in the `ellar.common` python module that can be used to modify the behavior of route functions. 
 
 These decorators can be used to change the response type of a route function, add filters to the response schema, define the OPENAPI context, and more. 
 In general, these decorators can help to simplify and streamline the process of creating routes.
 
 ## **HTTP Method Decorator**
 `@get`, `@post`, `@put`, `@patch`, `@delete`, `@trace`, `@options`, `@head` are decorators that define the standard HTTP methods for a route function. 
@@ -27,15 +27,15 @@
 - `File(...)`
 - `Path(...)`
 - `Header(...)`
 - `Cookie(...)`
 
 Please refer to the "How-to-Guide" on parsing inputs [here](/ellar/parsing-inputs/) to see how this input decorators work. 
 
-### WsBody(..., embed=False)
+### **WsBody(..., embed=False)**
 
 `WsBody(...)` is a decorator that defines the message format that should be transmitted from the client in a WebSocket when there is a successful connection. 
 This decorator can be used to specify the structure of the message that is sent over the WebSocket, and to validate the message against a specified schema
 but for only `use_extra_handler=True`.
 
 For example:
 ```python
@@ -60,15 +60,15 @@
 ## **Non Route Function Parameters Decorators**
 We discussed decorators that are used to define route function parameter dependencies in Ellar. 
 These decorators, such as `Query`, `Form`, and `Body`, etc. are pydantic models used to specify the expected parameters for a route function. 
 
 However, there are also some route parameters that are **system** dependent, such as the `request` or `websocket` object, and the `response` object. 
 These parameters are resolved by the application and supplied to the route function when needed, and are not specified with pydantic models or user input.
 
-### Provide(Type)
+### **Provide(Type)**
 The **Provide(Type)** decorator is used to resolve a service provider and inject it into a route function parameter. 
 This can be useful when using the ModuleRouter feature in Ellar. 
 
 It allows for easy injection of services into route functions, making it easier to manage dependencies and improve code organization. 
 This can be useful for resolving database connections, external APIs, or other resources that are used by the route function.
 
 For example:
@@ -91,15 +91,15 @@
 This allows for easy access to the objects without having to manually import and instantiate them. 
 It also makes the code more modular and easier to test.
 
 !!! info
     Only types registered in the application can be resolved, but you can set `INJECTOR_AUTO_BIND = True` in configuration for the injector to register automatically that are not found. 
     please note that this automatic registration will be scoped to singleton by the `EllarInjector`.
 
-### Context
+### **Context**
 The **Context()** decorator injects the current `IExecutionContext` to route function parameter. See [ExecutionContext](/basics/execution-context)
 
 For example:
 ```python
 from ellar.common import ModuleRouter, Context
 
 router = ModuleRouter('/test-context')
@@ -113,15 +113,15 @@
 
 In this example, the example_endpoint function is decorated with the **Context()** decorator, which injects the current `IExecutionContext` object into the `ctx` parameter of the function. 
 The `IExecutionContext` object provides access to various resources and information related to the current execution context, such as the current HTTP connection, query parameters, and more. 
 
 In this example, the `switch_to_http_connection()` method is used to access the current HTTP connection and the `get_client()` method is used to get the client object for the connection. 
 The `query_params` attribute of the client object is then accessed and included in the response returned by the endpoint.
 
-### Req
+### **Req**
 **Req()** decorator injects current `Request` object to route function parameter.
 
 For example:
 ```python
 from ellar.common import ModuleRouter, Req
 
 router = ModuleRouter('/test-req')
@@ -133,15 +133,15 @@
     return {'message': 'injected request object', 'headers': headers, 'query_params': query_params}
 
 ```
 
 In this example, the `example_endpoint` function has a parameter req decorated with `Req()`, which will be automatically populated with the current `Request` object at runtime. 
 The `headers` and `query_params` attributes of the `req` object can then be accessed and used within the function.
 
-### Res
+### **Res**
 **Res()** decorator injects current `Response` object to route function parameter.
 
 For example:
 ```python
 from ellar.common import ModuleRouter, Res
 
 router = ModuleRouter('/test-response')
@@ -152,15 +152,15 @@
     return {'message': 'inject response object'}
 
 ```
 
 In this example, the `Res()` decorator injects the current `Response` object to the `res` parameter of the `example_endpoint` function. 
 This will allow you to manipulate the headers of the response before it is sent back to the client.
 
-### Ws
+### **Ws**
 **Ws()** decorator injects current `WebSocket` object to route function parameter.
 
 For example:
 ```python
 from ellar.common import ModuleRouter, Ws
 
 router = ModuleRouter('/test-ws')
@@ -219,15 +219,15 @@
 
 ```
 
 ## **Route Function Decorators**
 These decorators are used to modify the output data of a route function, add filtering to the output schema, or add extra OPENAPI information about the route function.
 
 They include:
-### RENDER
+### **RENDER**
 **@render()** decorator converts a route function response to HTML template response. 
 
 for example: 
 ```python
 from ellar.common import get, render
 ...
 @get('/index-template')
@@ -240,15 +240,15 @@
 which will return a 200 status code and HTML content from my_template. 
 
 The return object from the index function will be used as the templating context for `my_template` during the template rendering process. 
 This allows the function to pass data to the template and have it rendered with the provided context, the rendered template will be the response body.
 
 See [HTML Templating](/ellar/templating/templating) for more information on `render` and HTML templating with Ellar.
 
-### FILE
+### **FILE**
 **@file()** decorator converts a route function response to file or streaming response type. 
 Based on the value of `streaming` parameter, file decorator creates `FileResponseModel` or `StreamingResponseModel`.
 
 #### FileResponseModel as file(streaming=False)
 When `streaming` parameter in `@file(streaming=False)` decorator is set to `False`, a `FileResponseModel` is created as the response model for the decorated route function. 
 And the route function is required to return a dictionary object that follows a `FileResponseModelSchema` format:
 
@@ -285,15 +285,15 @@
 @file(media_type='text/html', streaming=False)
 def file_download(self):
     return {'path': 'path/to/file.html', 'filename': 'code.html', 'content_disposition_type': 'attachment'}
 ```
 In the example, an additional parameter media_type is added to the @file(streaming=False) decorator to define the content-type of the file returned. This is helpful for creating the route function's OPENAPI documentation, as it allows the content-type to be defined upfront. Without this parameter, the content-type will be computed during runtime when returning a response for a request.
 It is a way to explicitly define the content-type of the file which will be returned.
 
-#### StreamingResponseModel as file(streaming=True)
+#### **StreamingResponseModel as file(streaming=True)**
 On the other hand, when `streaming` parameter in `@file(streaming=True)` decorator is set to `True`, a `StreamingResponseModel` is created as the response model for the decorated route function. 
 And the route function is required to return an `ContentStream`. `ContentStream` is an synchronous or asynchronous iterator of string or bytes. 
 Type definition is shown below.
 
 ```python
 import typing
 import asyncio
@@ -315,15 +315,15 @@
 @get('/stream')
 @file(media_type='text/html', streaming=True)
 def file_stream(self):
     # file_stream function must return ContentStream
     return slow_numbers(1, 4)
 ```
 
-### OPENAPI-INFO
+### **OPENAPI-INFO**
 **@openapi_info()** decorator adds extra route function OPENAPI properties to route function OPENAPI documentation. They include:
 
 Parameters:
 
 - `tags`: adds more OPENAPI tags to route function OPENAPI docs.
 - `deprecated`: marks route function as deprecated. Default is false
 - `descriptions`: adds description to route function OPENAPI docs
@@ -343,15 +343,15 @@
     operation_id='some-operation-id', 
     summary='some summary'
 )
 def openapi_info_function(self, query: str):
     return f"foo bar {query}"
 ```
 
-### SERIALIZER-FILTER
+### **SERIALIZER FILTER**
 **@serializer_filter()** decorator provides Pydantic filtering options to decorated route function output schema.
 
 Parameters:
 
 - `include`: fields to include in the returned dictionary
 - `exclude`: fields to exclude from the returned dictionary
 - `by_alias`: whether field aliases should be used as keys in the returned dictionary; default `False`
@@ -376,15 +376,15 @@
 def serialized_output_1(self):
     return dict(username='python', password='secret', first_name='ellar')
 
 ```
 In example, `serializer_filter` to filter values that are `None` and also excluded `password` property from been returned.
 See [Pydantic Model Export](https://docs.pydantic.dev/usage/exporting_models/#modeldict) for more examples.
 
-### VERSION
+### **VERSION**
 **@version()**  is a decorator that provides endpoint versioning for a route function. 
 This decorator allows you to specify the version of the endpoint that the function is associated with. 
 
 Based on the versioning scheme configuration in the application, versioned route functions are called. This can be useful for maintaining backward compatibility, or for rolling out new features to different versions of an application. 
 More information on how to use this decorator can be found in the [Versioning documentation]()
 
 A quick example on how to use `version` decorator:
@@ -397,43 +397,43 @@
     return {'message': 'for v2 and v3 request'}
 ```
 
 The `version` decorator takes a list of values as an argument, for example `@version('2', '3')`. 
 This indicates that the `get_item_v2_v3` route function will handle version 2 and version 3 requests of the /create endpoint. 
 This allows for multiple versions of the same endpoint to be handled by different route functions, each with their own logic and implementation.
 
-### GUARDS
-**@Guards()**  is a decorator that applies a protection class of type `GuardCanActivate` to a route function. 
+### **UseGuards**
+**@UseGuards()**  is a decorator that applies a protection class of type `GuardCanActivate` to a route function. 
 These protection classes have a `can_execute` function that is called to determine whether a route function should be executed. 
 
 This decorator allows you to apply certain conditions or checks before a route function is executed, such as `authentication` or `authorization` checks. 
 This can help to ensure that only authorized users can access certain resources. 
 
 More information on how to use this decorator can be found in the [Guard Documentation]()
 
-A quick example on how to use `Guards` decorator:
+A quick example on how to use `UseGuards` decorator:
 ```python
 import typing as t
-from ellar.common import get, Guards
+from ellar.common import get, UseGuards
 from ellar.core import APIKeyQuery, HTTPConnection
 
 
 class MyAPIKeyQuery(APIKeyQuery):
     async def authenticate(self, connection: HTTPConnection, key: t.Optional[t.Any]) -> t.Optional[t.Any]:
         if key == 'supersecret':
             return True
         return False
 
 
 @get("/")
-@Guards(MyAPIKeyQuery(), )
+@UseGuards(MyAPIKeyQuery(), )
 async def get_guarded_items(self):
     return {'message': 'worked fine with `key`=`supersecret`'}
 ```
-The `Guards` decorator, like the `version` decorator, takes a list of values as an argument. 
+The `UseGuards` decorator, like the `version` decorator, takes a list of values as an argument. 
 During a request, the provided guards are called in the order in which they are provided. 
 
 This allows you to apply multiple guards to a single route function and have them executed in a specific order. 
 This is useful for applying multiple levels of security or access control to a single endpoint. 
 
 Each guard class has a `can_execute` function that is called in the order specified by the decorator, if any of the guard's `can_execute` function returns False, the route function will not be executed.
 
@@ -449,13 +449,9 @@
 
 - `@middleware`: This decorator is used to register a function as a middleware. Middlewares are called for each incoming request and can be used to modify the request or response, or perform any other actions before or after the request is handled.
 
 - `@template_filter`: This decorator is used to register a function as a Jinja2 template filter. The function should take one or more arguments and return a modified value.
 
 - `@template_global`: This decorator is used to register a function as a global variable available in all Jinja2 templates. The function can be called without any arguments and should return a value.
 
-- `@on_shutdown`: This decorator is used to register a function that will be called when the application is shutting down.
-
-- `@on_startup`: This decorator is used to register a function that will be called when the application is starting up.
-
 These decorators can be used to define functions that will be executed at specific points in the application's lifecycle. 
 They provide a way to separate and organize the different parts of an application. See [Module Additional Configuration](../modules/#additional-module-configurations) for examples on how these decorator functions are used.
```

### Comparing `ellar-0.3.8/docs/overview/exception_handling.md` & `ellar-0.4.0/docs/overview/exception_handling.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+# **Exceptions & Exception Handling**
 The `ExceptionMiddleware` and `ExceptionMiddlewareService` handle all unhandled exceptions throughout an application and provide user-friendly responses.
 
 ```json
 {
   "status_code": 403,
   "detail": "Forbidden"
 }
```

### Comparing `ellar-0.3.8/docs/overview/guards.md` & `ellar-0.4.0/docs/overview/guards.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# **Guards**
+
 A **Guard** in Ellar is a way to add **authentication** and **authorization** checks to your application. 
 It acts as a middleware and runs before executing the route handler. If the guard returns **false**, the request is rejected and the execution is stopped. 
 
 **Guards** can be used to check for specific roles, permissions, or any other arbitrary condition. 
 They can be easily applied to individual routes or groups of routes using `@guard` decorator.
 
 Unlike middleware, a guard have access to the `ExecutionContext` which provides information for the route function to be executed and its controller.
@@ -51,62 +53,62 @@
 class RoleGuard(GuardCanActivate):
   async def can_activate(self,context: IExecutionContext) -> bool: 
     return True
 ```
 
 ## **Applying guards**
 Guards can be **`controller-scoped`**, **`method-scoped`**, or **`global-scoped`**. We apply guards to controllers or route function by using `@Guards`.
-The `@Guards` takes a single argument, or a comma-separated list of arguments of `GuardCanActivate` types or instances.
+The `@UseGuards` takes a single argument, or a comma-separated list of arguments of `GuardCanActivate` types or instances.
 
 ```python
 import typing as t
 
-def Guards(
+def UseGuards(
     *_guards: t.Type["GuardCanActivate"] | "GuardCanActivate"
 ) -> t.Callable:
     ...
 ```
 
 ### **Controller-scoped**
-We set up controller scoped guards on controller by using `@Guards` decorator. For example:
+We set up controller scoped guards on controller by using `@UseGuards` decorator. For example:
 ```python
 # project_name/cars/controllers.py
-from ellar.common import Controller, Guards
+from ellar.common import Controller, UseGuards
 from .guards import RoleGuard
 
 @Controller()
-@Guards(RoleGuard)
+@UseGuards(RoleGuard)
 class CarsController:
     ...
 
 ```
 The above example attaches the guard to every handler declared by this controller. 
-If we wish the guard to apply only to a single method, we apply the `@Guards()` decorator at the method level.
+If we wish the guard to apply only to a single method, we apply the `@UseGuards()` decorator at the method level.
 
 ### **Method-scoped**
-We can also use `@Guards()` on route-function when necessary.
+We can also use `@UseGuards()` on route-function when necessary.
 ```python
 # project_name/cars/controllers.py
-from ellar.common import Controller, Guards, get
+from ellar.common import Controller, UseGuards, get
 from .guards import RoleGuard
 
 @Controller()
-@Guards(RoleGuard)
+@UseGuards(RoleGuard)
 class CarsController:
-    @Guards(RoleGuard())
+    @UseGuards(RoleGuard())
     @get('/guarded-route')
     def guarded_route(self):
         return "Passed Guard"
 
 ```
-In the example, we decorated `guarded_route` with `@Guards(RoleGuard())` with an instance of `RoleGuard`. 
+In the example, we decorated `guarded_route` with `@UseGuards(RoleGuard())` with an instance of `RoleGuard`. 
 When request execution for `/guarded-route`, `guarded_route` guard definition will be precedence over `CarsController` guard definitions.
 
 ### **Global-scope**
-Global guards are used across the whole application, for every controller and every route function but individual controller or route function `@Guards` definition can override `global` scoped guards.
+Global guards are used across the whole application, for every controller and every route function but individual controller or route function `@UseGuards` definition can override `global` scoped guards.
 
 Global guards are applied at the `global_guards` parameter of the `AppFactory` creation level as shown below:
 ```python
 # project_name/server.py
 import os
 
 from ellar.common.constants import ELLAR_CONFIG_MODULE
```

### Comparing `ellar-0.3.8/docs/overview/index.md` & `ellar-0.4.0/docs/overview/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
+# **Step One**
 You will learn the core fundamentals of Ellar with this set of articles. We are going to build a basic CRUD application
 with features that cover a lot of ground at an introductory level.
 
 
-## Library Dependencies
+## **Library Dependencies**
 Ellar core depends on:
 
 - `python >= 3.7`
 - `Starlette`
 - `Injector`
 
 
-## Quick Step
+## **Quick Step**
 Using the Ellar CLI, you can easily set up a new project by running the following commands in your OS terminal:
 ```shell
 $(venv) pip install ellar-cli
 $(venv) ellar new project-name
 ```
 
 The `new` command will create a `project-name` project directory with other necessary files needed for the Ellar CLI tool to properly manage your project.
@@ -67,15 +67,15 @@
     ),
 )
 ```
 
 There are two ways to create an Ellar application using the `AppFactory`, `create_from_app_module` and `create_app`.
 Both provides all necessary parameter for creating Ellar application
 
-## Run your project
+## **Run your project**
 Ellar runs [UVICORN - ASGI Server](https://www.uvicorn.org/) under the hood.
 
 ```shell
 $(venv) cd project-name
 $(venv) ellar runserver --reload
 ```
 `--reload` is to watch for file changes
@@ -170,15 +170,15 @@
 Goto your browser and visit: [http://localhost:8000/car/](http://localhost:8000/car/)
 ```json
 {
   "detail": "Welcome Car Resource"
 }
 ```
 
-## Enabling OpenAPI Docs
+## **Enabling OpenAPI Docs**
 To set up OPENAPI documentation, we need to go back to the project folder. In the `server.py`
 then add the below.
 ```python
 # project_name/server.py
 
 import os
 from ellar.constants import ELLAR_CONFIG_MODULE
```

### Comparing `ellar-0.3.8/docs/overview/middleware.md` & `ellar-0.4.0/docs/overview/middleware.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# **Middlewares**
 Middlewares are functions that are called during requests before hitting a specific route handler.
 Middleware functions can modify **request** and **response** objects during the `HTTP` or `WebSocket` connection. 
 
 ![middleware description image](../img/middleware.png)
 
 Ellar Middlewares follows the [`Starlette ASGI Middleware`](https://www.starlette.io/middleware/) contract. The middlewares are set up in a pipeline fashion that creates a chain of request-response cycles.
```

### Comparing `ellar-0.3.8/docs/overview/module-router.md` & `ellar-0.4.0/docs/overview/module-router.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Module Router
+# **Module Router**
 
 ModuleRouter allows you to define your route handlers as standalone functions, providing an alternative to using classes. 
 This can be beneficial for python developers who prefer using functions. 
 It is important to note that using ModuleRouter does not limit your access to other features provided by Ellar.
 
 ## **Usage**
 The Ellar CLI tool generates a `routers.py` file in every `create-module` scaffold command.
```

### Comparing `ellar-0.3.8/docs/overview/modules.md` & `ellar-0.4.0/docs/overview/modules.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# **Modules**
+
 A module is a class annotated with a `@Module()` decorator.
 The `@Module()` decorator provides **metadata** that exports a `Module` data and defines the module structure.
 
 ![middleware description image](../img/ModuleDescription.png)
 
 The best way to organize your components is to build your projects as `Modules`.
```

### Comparing `ellar-0.3.8/docs/overview/providers.md` & `ellar-0.4.0/docs/overview/providers.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# **Providers**
 A provider is any class or object that is **injectable** as a dependency to another class, and it's required when creating an instance of that class.
 
 Providers are like services, repositories services, factories, etc., classes that manage complex tasks. These providers can be made available to a controller, a route handler, or to another provider as a dependency. This concept is known as [Dependency Injector](https://en.wikipedia.org/wiki/Dependency_injection)
 
 You can easily create a provider class by decorating that class with the `@injectable()` mark and stating the scope.
 
 ```python
```

### Comparing `ellar-0.3.8/docs/parsing-inputs/body.md` & `ellar-0.4.0/docs/parsing-inputs/body.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/parsing-inputs/cookie-params.md` & `ellar-0.4.0/docs/parsing-inputs/cookie-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/parsing-inputs/file-params.md` & `ellar-0.4.0/docs/parsing-inputs/file-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/parsing-inputs/form-params.md` & `ellar-0.4.0/docs/parsing-inputs/form-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/parsing-inputs/header-params.md` & `ellar-0.4.0/docs/parsing-inputs/header-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/parsing-inputs/index.md` & `ellar-0.4.0/docs/parsing-inputs/index.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/parsing-inputs/path-params.md` & `ellar-0.4.0/docs/parsing-inputs/path-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/parsing-inputs/query-params.md` & `ellar-0.4.0/docs/parsing-inputs/query-params.md`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/docs/templating/staticfiles.md` & `ellar-0.4.0/docs/templating/staticfiles.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# **Static Files**
 A static file is a type of file that does not change often and is not generated by a server-side script. Examples of static files include images, CSS and JavaScript files, audio and video files, and other types of media.
 
 Static files in Ellar are served using the `StaticFiles` ASGI class, which is an extension of the Starlette `StaticFiles` ASGI class. 
 This class uses the static files specified in the application's **modules** and **configuration**.
 
 In addition, Ellar creates a route that mounts the static server at the `/static` path. 
 The path can be modified by providing a new value for the `STATIC_MOUNT_PATH` configuration variable.
```

### Comparing `ellar-0.3.8/docs/templating/templating.md` & `ellar-0.4.0/docs/templating/templating.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+# **HTML Templating with [Jinja](https://jinja.palletsprojects.com/en/3.0.x/){target='_blank'}**
 Jinja2 is a powerful template engine for Python. It can be used in web applications to separate static and dynamic content, 
 making it easier to maintain and update the dynamic content. 
 
 In Ellar, a Model-View-Controller (MVC) framework, Jinja2 templates are typically used in the View layer to render dynamic content, 
 while the Model and Controller layers handle the data and logic of the application.
 
 
 ## **Installation**
-[`Jinja2`](https://jinja.palletsprojects.com/en/3.0.x/) package is installed alongside with Ellar.
+[`Jinja2`](https://jinja.palletsprojects.com/en/3.0.x/){target='_blank'} package is installed alongside with Ellar.
 
 
 ## **Quick overview on jinja2 Usage**
 A Jinja2 template is a plain text file that contains dynamic content, represented using Jinja2 syntax. 
 Here's an example template that displays a list of items:
 
 ```html
```

### Comparing `ellar-0.3.8/docs/throttling.md` & `ellar-0.4.0/docs/throttling.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# **Rate Limiting**
 A common technique to protect applications from brute-force attacks is rate-limiting. 
 
 To get started, you'll need to install the `ellar-throttler` package.
 
 ```shell
 $(venv) pip install ellar-throttler
 ```
@@ -47,26 +48,26 @@
     ),
     global_guards=[ThrottlerGuard]
 )
 ```
 The above is also a valid configuration for `ThrottleModule` registration if you want to work with config.
 
 If you add the `ThrottlerGuard` to your application `global_guards`, then all the incoming requests will be throttled by default. 
-This can also be omitted in favor of `@Guards(ThrottlerGuard)`. The global guard check can be skipped using the `@skip_throttle()` decorator mentioned later.
+This can also be omitted in favor of `@UseGuards(ThrottlerGuard)`. The global guard check can be skipped using the `@skip_throttle()` decorator mentioned later.
 
-Example with `@Guards(ThrottlerGuard)`
+Example with `@UseGuards(ThrottlerGuard)`
 ```python
 # project_name/controller.py
-from ellar.common import Controller, Guards
+from ellar.common import Controller, UseGuards
 from ellar_throttler import throttle, ThrottlerGuard
 
 @Controller()
 class AppController:
 
-  @Guards(ThrottlerGuard)
+  @UseGuards(ThrottlerGuard)
   @throttle(limit=5, ttl=30)
   def normal(self):
       pass
 
 ```
 
 ### **ThrottlerModule Configuration Options:**
@@ -90,20 +91,20 @@
 @skip_throttle(skip: bool = True)
 ```
 This decorator can be used to skip a route or a class or to negate the skipping of a route in 
 a class that is skipped.
 
 ```python
 # project_name/controller.py
-from ellar.common import Controller, Guards
+from ellar.common import Controller, UseGuards
 from ellar_throttler import ThrottlerGuard, skip_throttle
 
 @skip_throttle()
 @Controller()
-@Guards(ThrottlerGuard)
+@UseGuards(ThrottlerGuard)
 class AppController:
   
     def do_skip(self):
         pass
   
     @skip_throttle(skip=False)
     def dont_skip(self):
@@ -188,15 +189,15 @@
     def get_tracker(self, connection: HTTPConnection) -> str:
         return connection.client.host  # individualize IP extraction to meet your own needs
 
 # project_name/controller.py
 from .throttler_behind_proxy import ThrottlerBehindProxyGuard
 
 @Controller('')
-@Guards(ThrottlerBehindProxyGuard)
+@UseGuards(ThrottlerBehindProxyGuard)
 class AppController:
     pass
 ```
 
 ### **Working with WebSockets**
 To work with Websockets you can extend the `ThrottlerGuard` and override the `handle_request` method with the code below:
 ```python
```

### Comparing `ellar-0.3.8/docs/websockets/index.md` & `ellar-0.4.0/docs/websockets/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Websocket
+# **Websocket**
 
 [WebSocket](https://developer.mozilla.org/en-US/docs/Web/API/WebSockets_API) is a powerful communication protocol that allows for two-way communication between a client and a server over a single, 
 long-lived connection, making it an ideal tool for building real-time applications.
 
 ## **Creating a WebSocket Route**
 In Ellar, you create websocket route using `ws_route` decorator.
```

### Comparing `ellar-0.3.8/docs/websockets/socketio.md` & `ellar-0.4.0/docs/websockets/socketio.md`

 * *Files 1% similar despite different names*

```diff
@@ -353,10 +353,10 @@
 Also, it is possible to test with more than one client as you can see in `test_broadcast_work` in construct above.
 We created another instance of **RunWithServerContext** as `ctx_2` from the already existing `ctx` with `ctx.new_socket_client_context()`. 
 And both were used to test for message broadcast.
 
 
 ## **SocketIO Ellar Example**
 [python-socketio](https://python-socketio.readthedocs.io/en/latest/){target="_blank"} provided a sample project on how to integrate [python-socketio with django](https://github.com/miguelgrinberg/python-socketio/blob/main/examples/server/wsgi).
-The sample project was converted to ellar gateway and it can find it [here]()
+The sample project was converted to ellar gateway and it can find it [here](https://github.com/eadwinCode/ellar/tree/main/examples/02-socketio-app){target="_blank"}
 
 ![gateway_example_image](../img/live_support_websocket_3.gif)
```

### Comparing `ellar-0.3.8/ellar/cache/backends/_aio_cache.py.ellar` & `ellar-0.4.0/ellar/cache/backends/_aio_cache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/backends/base.py` & `ellar-0.4.0/ellar/cache/backends/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/backends/local_cache.py` & `ellar-0.4.0/ellar/cache/backends/local_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/backends/pylib_cache.py` & `ellar-0.4.0/ellar/cache/backends/pylib_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/backends/pymem_cache.py` & `ellar-0.4.0/ellar/cache/backends/pymem_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/backends/redis/backend.py` & `ellar-0.4.0/ellar/cache/backends/redis/backend.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/backends/serializer.py` & `ellar-0.4.0/ellar/cache/backends/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/interface.py` & `ellar-0.4.0/ellar/cache/interface.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/make_key_decorator.py` & `ellar-0.4.0/ellar/cache/make_key_decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/model.py` & `ellar-0.4.0/ellar/cache/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/module.py` & `ellar-0.4.0/ellar/cache/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/schema.py` & `ellar-0.4.0/ellar/cache/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/cache/service.py` & `ellar-0.4.0/ellar/cache/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         return _backend.touch(key, version=version, ttl=ttl)
 
     def has_key(self, key: str, version: str = None, backend: str = None) -> bool:
         _backend = self.get_backend(backend)
         return _backend.has_key(key, version=version)
 
 
-@injectable  # type: ignore
+@injectable
 class CacheService(_CacheServiceSync, ICacheService):
     """
     A Cache Backend Service that wraps Ellar cache backends
     """
 
     def __init__(self, backends: t.Dict[str, BaseCacheBackend] = None) -> None:
         if backends:
```

### Comparing `ellar-0.3.8/ellar/common/__init__.py` & `ellar-0.4.0/ellar/common/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from starlette.exceptions import WebSocketException
 
 from .commands import EllarTyper, command
 from .datastructures import UploadFile
 from .decorators import (
     Controller,
-    Guards,
     Module,
+    UseGuards,
+    UseInterceptors,
     Version,
     exception_handler,
     extra_args,
     file,
     middleware,
     openapi_info,
     render,
@@ -32,62 +33,67 @@
     UnsupportedMediaType,
 )
 from .interfaces import (
     IExceptionHandler,
     IExceptionMiddlewareService,
     IExecutionContext,
     IExecutionContextFactory,
+    IGuardsConsumer,
     IHostContext,
     IHostContextFactory,
     IHTTPConnectionContextFactory,
     IHTTPHostContext,
+    IInterceptorsConsumer,
     IModuleSetup,
     IModuleTemplateLoader,
     IResponseModel,
     IWebSocketContextFactory,
     IWebSocketHostContext,
 )
 from .models import (
     BaseAPIKey,
     BaseAuthGuard,
     BaseHttpAuth,
     ControllerBase,
     ControllerType,
+    EllarInterceptor,
     GuardCanActivate,
 )
-from .params.params import ParamFieldInfo as Param, ParamTypes
-from .responses import (
-    FileResponse,
-    HTMLResponse,
-    JSONResponse,
-    ORJSONResponse,
-    PlainTextResponse,
-    RedirectResponse,
-    Response,
-    StreamingResponse,
-    UJSONResponse,
-)
-from .routing import (
+from .params.decorators import (
     Body,
     Context,
     Cookie,
     File,
     Form,
     Header,
     Host,
     Http,
-    ModuleRouter,
     Path,
     Provide,
     Query,
     Req,
     Res,
     Session,
     Ws,
     WsBody,
+)
+from .params.params import ParamFieldInfo as Param, ParamTypes
+from .responses import (
+    FileResponse,
+    HTMLResponse,
+    JSONResponse,
+    ORJSONResponse,
+    PlainTextResponse,
+    RedirectResponse,
+    Response,
+    StreamingResponse,
+    UJSONResponse,
+)
+from .routing import (
+    ModuleRouter,
     delete,
     get,
     head,
     http_route,
     options,
     patch,
     post,
@@ -121,15 +127,15 @@
     "MethodNotAllowed",
     "render_template",
     "render_template_string",
     "command",
     "ModuleRouter",
     "render",
     "Module",
-    "Guards",
+    "UseGuards",
     "Param",
     "ParamTypes",
     "set_metadata",
     "Controller",
     "openapi_info",
     "Version",
     "delete",
@@ -185,12 +191,16 @@
     "IWebSocketHostContext",
     "IHTTPConnectionContextFactory",
     "IExceptionMiddlewareService",
     "IExceptionHandler",
     "IModuleSetup",
     "IResponseModel",
     "IModuleTemplateLoader",
+    "IInterceptorsConsumer",
+    "IGuardsConsumer",
+    "EllarInterceptor",
+    "UseInterceptors",
 ]
 
 
 def __dir__() -> t.List[str]:
     return sorted(__all__)  # pragma: no cover
```

### Comparing `ellar-0.3.8/ellar/common/commands/base.py` & `ellar-0.4.0/ellar/common/commands/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         epilog: t.Optional[str] = Default(None),
         short_help: t.Optional[str] = Default(None),
         options_metavar: str = Default("[OPTIONS]"),
         add_help_option: bool = Default(True),
         hidden: bool = Default(False),
         deprecated: bool = Default(False),
         add_completion: bool = True,
-    ) -> None:
+    ) -> None:  # pragma: no cover
         assert name is not None and name != "", "Typer name is required"
         super().__init__(
             name=name,
             cls=cls,
             invoke_without_command=invoke_without_command,
             no_args_is_help=no_args_is_help,
             subcommand_metavar=subcommand_metavar,
```

### Comparing `ellar-0.3.8/ellar/common/commands/decorator.py` & `ellar-0.4.0/ellar/common/commands/decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     epilog: t.Optional[str] = None,
     short_help: t.Optional[str] = None,
     options_metavar: str = "[OPTIONS]",
     add_help_option: bool = True,
     no_args_is_help: bool = False,
     hidden: bool = False,
     deprecated: bool = False,
-) -> t.Callable[[CommandFunctionType], CommandFunctionType]:
+) -> t.Callable[[CommandFunctionType], CommandFunctionType]:  # pragma: no cover
     """
     ========= FUNCTION DECORATOR ==============
 
     Define Application Command which will be available on ellar cli
     """
     if cls is None:
         cls = TyperCommand
```

### Comparing `ellar-0.3.8/ellar/common/compatible/cache_properties.py` & `ellar-0.4.0/ellar/common/compatible/cache_properties.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/compatible/dict.py` & `ellar-0.4.0/ellar/common/compatible/dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/compatible/emails.py` & `ellar-0.4.0/ellar/common/compatible/emails.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/constants.py` & `ellar-0.4.0/ellar/common/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 CONTROLLER_WATERMARK = "CONTROLLER_WATERMARK"
 
 MULTI_RESOLVER_KEY = "MULTI_RESOLVER_KEY"
 MULTI_RESOLVER_FORM_GROUPED_KEY = "MULTI_RESOLVER_FORM_GROUPED_KEY"
 ROUTE_OPENAPI_PARAMETERS = "ROUTE_OPENAPI_PARAMETERS"
 
 OPERATION_ENDPOINT_KEY = "OPERATION_ENDPOINT"
+ROUTE_OPERATION_PARAMETERS = "__ROUTE_OPERATION_PARAMETERS__"
+ROUTE_INTERCEPTORS = "ROUTE_INTERCEPTORS"
+ROUTE_CACHE_OPTIONS = "ROUTE_CACHE_OPTIONS"
 CONTROLLER_OPERATION_HANDLER_KEY = "CONTROLLER_OPERATION_HANDLER"
 CONTROLLER_CLASS_KEY = "CONTROLLER_CLASS_KEY"
 
 CALLABLE_COMMAND_INFO = "__CALLABLE_COMMAND_INFO__"
 GROUP_METADATA = "GROUP_METADATA"
```

### Comparing `ellar-0.3.8/ellar/common/converters.py` & `ellar-0.4.0/ellar/common/converters.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/datastructures.py` & `ellar-0.4.0/ellar/common/datastructures.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/decorators/__init__.py` & `ellar-0.4.0/ellar/common/decorators/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import typing as t
 
 from .base import set_metadata
 from .controller import Controller
 from .exception import exception_handler
 from .extra_args import extra_args
 from .file import file
-from .guards import Guards
+from .guards import UseGuards
 from .html import render, template_filter, template_global
+from .interceptor import UseInterceptors
 from .middleware import middleware
 from .modules import Module
 from .openapi import openapi_info
 from .serializer import serializer_filter
 from .versioning import Version
 
 __all__ = [
     "serializer_filter",
     "Controller",
     "Version",
-    "Guards",
+    "UseGuards",
     "template_filter",
     "template_global",
     "file",
     "render",
     "exception_handler",
     "set_metadata",
     "middleware",
     "openapi_info",
     "Module",
     "extra_args",
+    "UseInterceptors",
 ]
 
 
 def __dir__() -> t.List[str]:
     return sorted(__all__)  # pragma: no cover
```

### Comparing `ellar-0.3.8/ellar/common/decorators/controller.py` & `ellar-0.4.0/ellar/common/decorators/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,72 @@
 import inspect
 import typing as t
 from abc import ABC
-from types import FunctionType
 
 from ellar.common.compatible import AttributeDict
 from ellar.common.constants import (
     CONTROLLER_CLASS_KEY,
     CONTROLLER_METADATA,
     CONTROLLER_OPERATION_HANDLER_KEY,
     CONTROLLER_WATERMARK,
     NOT_SET,
     OPERATION_ENDPOINT_KEY,
+    ROUTE_OPERATION_PARAMETERS,
 )
 from ellar.common.exceptions import ImproperConfiguration
+from ellar.common.logger import logger
 from ellar.common.models import ControllerBase, ControllerType
-from ellar.common.routing.controller import ControllerRouteOperationBase
 from ellar.di import RequestScope, injectable
 from ellar.reflect import REFLECT_TYPE, reflect
 
+from ..routing.controller import (
+    ControllerRouteOperation,
+    ControllerWebsocketRouteOperation,
+)
+from ..routing.schema import RouteParameters, WsRouteParameters
+
 
 def get_route_functions(
     cls: t.Type,
-) -> t.Iterable[t.Union[t.Callable, ControllerRouteOperationBase]]:
+) -> t.Iterable[t.Callable]:
     for method in cls.__dict__.values():
-        if hasattr(method, OPERATION_ENDPOINT_KEY) or isinstance(
-            method, ControllerRouteOperationBase
-        ):
+        if hasattr(method, OPERATION_ENDPOINT_KEY):
             yield method
 
 
 def reflect_all_controller_type_routes(cls: t.Type[ControllerBase]) -> None:
     bases = inspect.getmro(cls)
 
     for base_cls in reversed(bases):
         if base_cls not in [ABC, ControllerBase, object]:
             for item in get_route_functions(base_cls):
-                operation = item
-                if callable(item) and type(item) == FunctionType:
-                    operation = reflect.get_metadata(  # type: ignore
-                        CONTROLLER_OPERATION_HANDLER_KEY, item
-                    )
-                endpoint_func = operation.endpoint  # type:ignore
-                if reflect.has_metadata(CONTROLLER_CLASS_KEY, endpoint_func):
+                if reflect.has_metadata(CONTROLLER_CLASS_KEY, item):
                     raise Exception(
                         f"{cls.__name__} Controller route tried to be processed more than once."
-                        f"\n-RouteFunction - {endpoint_func}."
+                        f"\n-RouteFunction - {item}."
                         f"\n-Controller route function can not be reused once its under a `@Controller` decorator."
                     )
+                reflect.define_metadata(CONTROLLER_CLASS_KEY, cls, item)
+
+                parameter = item.__dict__[ROUTE_OPERATION_PARAMETERS]
+                operation: t.Union[
+                    ControllerRouteOperation, ControllerWebsocketRouteOperation
+                ]
+                if isinstance(parameter, RouteParameters):
+                    operation = ControllerRouteOperation(**parameter.dict())
+                elif isinstance(parameter, WsRouteParameters):
+                    operation = ControllerWebsocketRouteOperation(**parameter.dict())
+                else:  # pragma: no cover
+                    logger.warning(
+                        f"Parameter type is not recognized. {type(parameter) if not isinstance(parameter, type) else parameter}"
+                    )
+                    continue
+
+                del item.__dict__[ROUTE_OPERATION_PARAMETERS]
 
-                reflect.define_metadata(CONTROLLER_CLASS_KEY, cls, endpoint_func)
                 reflect.define_metadata(
                     CONTROLLER_OPERATION_HANDLER_KEY,
                     [operation],
                     cls,
                 )
```

### Comparing `ellar-0.3.8/ellar/common/decorators/exception.py` & `ellar-0.4.0/ellar/common/decorators/exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/decorators/extra_args.py` & `ellar-0.4.0/ellar/common/decorators/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/decorators/file.py` & `ellar-0.4.0/ellar/common/decorators/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/decorators/html.py` & `ellar-0.4.0/ellar/common/decorators/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/decorators/middleware.py` & `ellar-0.4.0/ellar/common/decorators/middleware.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     )
 
 
 def middleware() -> t.Callable:
     """
     ========= MODULE DECORATOR ==============
 
-    Defines middle functions at module level
+    Defines middleware functions at  @Module decorated class level
     :return: Function
     """
 
     def decorator(func: t.Callable) -> t.Callable:
         _add_middleware(dispatch=func)
         return func
```

### Comparing `ellar-0.3.8/ellar/common/decorators/modules.py` & `ellar-0.4.0/ellar/common/decorators/modules.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/decorators/openapi.py` & `ellar-0.4.0/ellar/common/decorators/openapi.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/decorators/serializer.py` & `ellar-0.4.0/ellar/common/decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/exceptions/__init__.py` & `ellar-0.4.0/ellar/common/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/exceptions/api/base.py` & `ellar-0.4.0/ellar/common/exceptions/api/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/exceptions/api/exceptions_types.py` & `ellar-0.4.0/ellar/common/exceptions/api/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/exceptions/callable_exceptions.py` & `ellar-0.4.0/ellar/common/exceptions/callable_exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/exceptions/handlers.py` & `ellar-0.4.0/ellar/common/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/exceptions/validation.py` & `ellar-0.4.0/ellar/common/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/helper/__init__.py` & `ellar-0.4.0/ellar/common/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/helper/enums.py` & `ellar-0.4.0/ellar/common/helper/enums.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/helper/importer.py` & `ellar-0.4.0/ellar/common/helper/importer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/helper/modelfield.py` & `ellar-0.4.0/ellar/common/helper/modelfield.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/helper/module_loading.py` & `ellar-0.4.0/ellar/common/helper/module_loading.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/interfaces/__init__.py` & `ellar-0.4.0/ellar/common/interfaces/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     IHostContextFactory,
     IHTTPConnectionContextFactory,
     IHTTPHostContext,
     IWebSocketContextFactory,
     IWebSocketHostContext,
 )
 from .exceptions import IExceptionHandler, IExceptionMiddlewareService
+from .guard_consumer import IGuardsConsumer
+from .interceptor_consumer import IInterceptorsConsumer
 from .module import IModuleSetup
 from .response_model import IResponseModel
 from .templating import IModuleTemplateLoader
 
 __all__ = [
     "IHostContext",
     "IExecutionContextFactory",
@@ -23,8 +25,10 @@
     "IWebSocketHostContext",
     "IHTTPConnectionContextFactory",
     "IExceptionMiddlewareService",
     "IExceptionHandler",
     "IModuleSetup",
     "IResponseModel",
     "IModuleTemplateLoader",
+    "IInterceptorsConsumer",
+    "IGuardsConsumer",
 ]
```

### Comparing `ellar-0.3.8/ellar/common/interfaces/context.py` & `ellar-0.4.0/ellar/common/interfaces/context.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/interfaces/exceptions.py` & `ellar-0.4.0/ellar/common/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/interfaces/module.py` & `ellar-0.4.0/ellar/common/interfaces/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/interfaces/response_model.py` & `ellar-0.4.0/ellar/common/interfaces/response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/interfaces/templating.py` & `ellar-0.4.0/ellar/common/interfaces/templating.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/models/controller.py` & `ellar-0.4.0/ellar/common/models/controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/models/guard.py` & `ellar-0.4.0/ellar/common/models/guard.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/args/base.py` & `ellar-0.4.0/ellar/common/params/args/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from collections import defaultdict
 
 from pydantic import BaseModel
 from pydantic.error_wrappers import ErrorWrapper
 from pydantic.fields import FieldInfo, ModelField
 from pydantic.typing import ForwardRef, evaluate_forwardref  # type:ignore
 from pydantic.utils import Representation, lenient_issubclass
+from starlette.background import BackgroundTasks
 from starlette.convertors import Convertor
 from starlette.requests import (
     HTTPConnection as StarletteHTTPConnection,
     Request as StarletteRequest,
 )
 from starlette.responses import Response
 from starlette.websockets import WebSocket as StarletteWebSocket
@@ -28,14 +29,15 @@
 from ..helpers import is_scalar_field, is_scalar_sequence_field
 from ..resolvers import (
     BaseRouteParameterResolver,
     IRouteParameterResolver,
     NonParameterResolver,
 )
 from ..resolvers.non_parameter import (
+    BackgroundTasksParameter,
     ConnectionParam,
     ExecutionContextParameter,
     RequestParameter,
     ResponseRequestParam,
     WebSocketParameter,
 )
 from .extra_args import ExtraEndpointArg
@@ -49,14 +51,15 @@
 
 DEFAULT_RESOLVERS: t.Dict[t.Type, t.Type[NonParameterResolver]] = {
     StarletteRequest: RequestParameter,
     StarletteWebSocket: WebSocketParameter,
     Response: ResponseRequestParam,
     StarletteHTTPConnection: ConnectionParam,
     IExecutionContext: ExecutionContextParameter,
+    BackgroundTasks: BackgroundTasksParameter,
 }
 
 
 def add_default_resolver(
     type_identifier: t.Type, resolver_type: t.Type[NonParameterResolver]
 ) -> None:  # pragma: no cover
     DEFAULT_RESOLVERS.update({type_identifier: resolver_type})
```

### Comparing `ellar-0.3.8/ellar/common/params/args/extra_args.py` & `ellar-0.4.0/ellar/common/params/args/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/args/factory.py` & `ellar-0.4.0/ellar/common/params/args/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/args/request_model.py` & `ellar-0.4.0/ellar/common/params/args/request_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/args/resolver_generators.py` & `ellar-0.4.0/ellar/common/params/args/resolver_generators.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/args/websocket_model.py` & `ellar-0.4.0/ellar/common/params/args/websocket_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/helpers.py` & `ellar-0.4.0/ellar/common/params/helpers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/params.py` & `ellar-0.4.0/ellar/common/params/params.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/resolvers/__init__.py` & `ellar-0.4.0/ellar/common/params/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/resolvers/base.py` & `ellar-0.4.0/ellar/common/params/resolvers/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/resolvers/bulk_parameter.py` & `ellar-0.4.0/ellar/common/params/resolvers/bulk_parameter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/resolvers/non_parameter/base.py` & `ellar-0.4.0/ellar/common/params/resolvers/non_parameter/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/resolvers/non_parameter/inject.py` & `ellar-0.4.0/ellar/common/params/resolvers/non_parameter/inject.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/resolvers/non_parameter/session.py` & `ellar-0.4.0/ellar/common/params/resolvers/non_parameter/session.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/params/resolvers/parameter.py` & `ellar-0.4.0/ellar/common/params/resolvers/parameter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/responses/models/__init__.py` & `ellar-0.4.0/ellar/common/responses/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/responses/models/base.py` & `ellar-0.4.0/ellar/common/responses/models/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/responses/models/file.py` & `ellar-0.4.0/ellar/common/responses/models/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/responses/models/helper.py` & `ellar-0.4.0/ellar/common/responses/models/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/responses/models/html.py` & `ellar-0.4.0/ellar/common/responses/models/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/responses/models/json.py` & `ellar-0.4.0/ellar/common/responses/models/json.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     def create_response(
         self, context: IExecutionContext, response_obj: t.Any, status_code: int
     ) -> Response:
         json_response_class = t.cast(
             t.Type[JSONResponse],
             context.get_app().config.DEFAULT_JSON_CLASS or self._response_type,
         )
-        response_args, headers = self.get_context_response(context=context)
+        response_args, headers = self.get_context_response(
+            context=context, status_code=status_code
+        )
         serializer_filter = reflect.get_metadata(
             SERIALIZER_FILTER_KEY, context.get_handler()
         )
         response = json_response_class(
             **response_args,
             content=self.serialize(response_obj, serializer_filter=serializer_filter),
             headers=headers,
```

### Comparing `ellar-0.3.8/ellar/common/responses/models/route.py` & `ellar-0.4.0/ellar/common/responses/models/route.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import logging
 import typing as t
 
 from pydantic import BaseModel
 
 from ellar.common.constants import SCOPE_RESPONSE_STARTED
 from ellar.common.interfaces import IExecutionContext, IResponseModel
 
 from ..response_types import Response
 from .base import ResponseModel, ResponseResolver
 from .exceptions import RouteResponseExecution
 from .helper import create_response_model
-from .json import JSONResponseModel
+from .json import EmptyAPIResponseModel, JSONResponseModel
+
+logger = logging.getLogger("ellar")
 
 
 class RouteResponseModel:
     __slots__ = ("models",)
 
     def __init__(
         self,
@@ -76,17 +79,19 @@
             status_code, response_obj = endpoint_response_content
 
         if status_code in self.models:
             response_model = self.models[status_code]
         elif Ellipsis in self.models:
             response_model = self.models[Ellipsis]  # type: ignore
         else:
-            raise RouteResponseExecution(
+            logger.warning(
                 f"No response Schema with status_code={status_code} in response {self.models.keys()}"
             )
+            response_model = create_response_model(EmptyAPIResponseModel)
+
         response_model = t.cast(ResponseModel, response_model)
         return ResponseResolver(status_code, response_model, response_obj)
 
     def process_response(
         self, ctx: IExecutionContext, response_obj: t.Union[t.Any, t.Tuple[int, t.Any]]
     ) -> t.Optional[Response]:
         if isinstance(response_obj, Response):
```

### Comparing `ellar-0.3.8/ellar/common/responses/models/type_converter.py` & `ellar-0.4.0/ellar/common/responses/models/type_converter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/responses/response_types.py` & `ellar-0.4.0/ellar/common/responses/response_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/routing/__init__.py` & `ellar-0.4.0/ellar/common/routing/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,14 @@
 import typing as t
 
 from ellar.common.params.params import ParamFieldInfo as Param, ParamTypes
 
 from .base import RouteOperationBase
-from .controller.factory import ControllerRouterFactory
 from .mount import ModuleMount, ModuleRouter
 from .operation_definitions import OperationDefinitions
-from .params import (
-    Body,
-    Context,
-    Cookie,
-    File,
-    Form,
-    Header,
-    Host,
-    Http,
-    Path,
-    Provide,
-    Query,
-    Req,
-    Res,
-    Session,
-    Ws,
-    WsBody,
-)
 from .route import RouteOperation
 from .route_collections import RouteCollection
 from .websocket import WebsocketRouteOperation
 
 _route_definitions = OperationDefinitions()
 
 get = _route_definitions.get
@@ -42,48 +23,31 @@
 trace = _route_definitions.trace
 head = _route_definitions.head
 
 http_route = _route_definitions.http_route
 ws_route = _route_definitions.ws_route
 
 __all__ = [
-    "Context",
-    "Provide",
-    "Req",
-    "Ws",
-    "Body",
-    "WsBody",
-    "Cookie",
-    "File",
-    "Form",
-    "Header",
-    "Path",
-    "Query",
     "Param",
     "ParamTypes",
     "get",
     "post",
     "delete",
     "patch",
     "put",
     "options",
     "trace",
     "head",
     "http_route",
     "ws_route",
-    "Res",
-    "Session",
-    "Host",
-    "Http",
     "RouteCollection",
     "ModuleRouter",
     "ModuleMount",
     "RouteOperation",
     "RouteOperationBase",
     "OperationDefinitions",
     "WebsocketRouteOperation",
-    "ControllerRouterFactory",
 ]
 
 
 def __dir__() -> t.List[str]:
     return sorted(__all__)  # pragma: no cover
```

### Comparing `ellar-0.3.8/ellar/common/routing/base.py` & `ellar-0.4.0/ellar/common/routing/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,105 @@
 import typing as t
 from abc import ABC, abstractmethod
 
 from starlette.routing import Match
 
 from ellar.common.constants import (
     CONTROLLER_CLASS_KEY,
-    GUARDS_KEY,
     SCOPE_API_VERSIONING_RESOLVER,
     SCOPE_SERVICE_PROVIDER,
     VERSIONING_KEY,
 )
-from ellar.common.interfaces import IExecutionContext, IExecutionContextFactory
-from ellar.common.models import GuardCanActivate
+from ellar.common.interfaces import (
+    IExecutionContext,
+    IExecutionContextFactory,
+    IGuardsConsumer,
+    IInterceptorsConsumer,
+)
 from ellar.common.types import TReceive, TScope, TSend
 from ellar.reflect import reflect
 
 if t.TYPE_CHECKING:  # pragma: no cover
+    from ellar.common import ControllerBase
     from ellar.core.versioning.resolver import BaseAPIVersioningResolver
     from ellar.di import EllarInjector
 
 __all__ = [
     "RouteOperationBase",
     "WebsocketRouteOperationBase",
 ]
 
 
 class RouteOperationBase:
-    path: str
-    endpoint: t.Callable
     methods: t.Set[str]
 
+    def __init__(self, endpoint: t.Callable) -> None:
+        self.endpoint = endpoint
+        _controller_type: t.Type = reflect.get_metadata(  # type: ignore[assignment]
+            CONTROLLER_CLASS_KEY, self.endpoint
+        )
+        self._controller_type: t.Union[t.Type, t.Type["ControllerBase"]] = t.cast(
+            t.Union[t.Type, t.Type["ControllerBase"]], _controller_type
+        )
+
     @t.no_type_check
     def __call__(
         self, context: IExecutionContext, *args: t.Any, **kwargs: t.Any
     ) -> t.Any:
         return self.endpoint(*args, **kwargs)
 
     @abstractmethod
     def _load_model(self) -> None:
         """compute route models"""
 
-    @t.no_type_check
-    async def run_route_guards(self, context: IExecutionContext) -> None:
-        app = context.get_app()
-        reflector = app.reflector
-
-        targets = [self.endpoint, self.get_control_type()]
-
-        _guards: t.Optional[
-            t.List[t.Union[t.Type["GuardCanActivate"], "GuardCanActivate"]]
-        ] = reflector.get_all_and_override(GUARDS_KEY, *targets)
-
-        if not _guards:
-            _guards = app.get_guards()
-
-        if _guards:
-            for guard in _guards:
-                if isinstance(guard, type):
-                    guard = context.get_service_provider().get(guard)
-
-                result = await guard.can_activate(context)
-                if not result:
-                    guard.raise_exception()
-
     async def app(self, scope: TScope, receive: TReceive, send: TSend) -> None:
         service_provider: "EllarInjector" = scope[SCOPE_SERVICE_PROVIDER]
 
         execution_context_factory = service_provider.get(IExecutionContextFactory)
         context = execution_context_factory.create_context(
             operation=self, scope=scope, receive=receive, send=send
         )
+        interceptor_consumer = service_provider.get(IInterceptorsConsumer)
+        guard_consumer = service_provider.get(IGuardsConsumer)
 
-        await self.run_route_guards(context=context)
-        await self._handle_request(context=context)
+        await guard_consumer.execute(context, self)
+        await interceptor_consumer.execute(context, self)
 
-    def get_control_type(self) -> t.Type:
+    def get_controller_type(self) -> t.Type:
         """
         For operation under a controller, `get_control_type` and `get_class` will return the same result
         For operation under ModuleRouter, this will return a unique type created for the router for tracking some properties
         :return: a type that wraps the operation
         """
-        if not hasattr(self, "_control_type"):
-            _control_type = reflect.get_metadata(CONTROLLER_CLASS_KEY, self.endpoint)
-            if _control_type is None:
+        if not self._controller_type:
+            _controller_type = reflect.get_metadata(CONTROLLER_CLASS_KEY, self.endpoint)
+            if _controller_type is None or not isinstance(_controller_type, type):
                 raise Exception("Operation must have a single control type.")
-            self._control_type = t.cast(t.Type, _control_type)
+            self._controller_type = t.cast(t.Type, _controller_type)
 
-        return self._control_type
+        return self._controller_type
 
     @abstractmethod
-    async def _handle_request(self, *, context: IExecutionContext) -> None:
+    async def handle_request(self, *, context: IExecutionContext) -> t.Any:
         """return a context"""
 
+    @abstractmethod
+    async def handle_response(
+        self, context: IExecutionContext, response_obj: t.Any
+    ) -> None:
+        """returns a any"""
+
     def get_allowed_version(self) -> t.Set[t.Union[int, float, str]]:
         versions = reflect.get_metadata(VERSIONING_KEY, self.endpoint) or set()
         if not versions:
             versions = (
-                reflect.get_metadata(VERSIONING_KEY, self.get_control_type()) or set()
+                reflect.get_metadata(VERSIONING_KEY, self.get_controller_type())
+                or set()
             )
-        return t.cast(t.Set[t.Union[int, float, str]], versions)
+        return versions
 
     @classmethod
     def get_methods(cls, methods: t.Optional[t.List[str]] = None) -> t.Set[str]:
         if methods is None:
             methods = ["GET"]
 
         _methods = {method.upper() for method in methods}
```

### Comparing `ellar-0.3.8/ellar/common/routing/builder.py` & `ellar-0.4.0/ellar/core/routing/builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import typing as t
 
-from starlette.routing import Mount
+from starlette.routing import Host, Mount
+
+from ellar.common.logger import logger
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from .mount import ModuleMount
+    from ellar.common.routing.mount import ModuleMount
 
 _router_builder_factory: t.Dict[t.Type, t.Type["RouterBuilder"]] = {}
 
 
 def _register_controller_builder(
     controller_type: t.Type, factory: t.Type["RouterBuilder"]
 ) -> None:
@@ -15,18 +17,19 @@
 
 
 def get_controller_builder_factory(
     controller_type: t.Type,
 ) -> t.Type["RouterBuilder"]:
     res = _router_builder_factory.get(controller_type)
     if not res:
-        raise Exception(
+        logger.warning(
             f"Router Factory Builder was not found.\nUse `ControllerRouterBuilderFactory` "
             f"as an example create a FactoryBuilder for this type: {controller_type}"
         )
+        return _DefaultRouterBuilder
     return res
 
 
 class RouterBuilder:
     @classmethod
     def build(
         cls, controller_type: t.Union[t.Type, t.Any]
@@ -37,7 +40,23 @@
     def check_type(cls, controller_type: t.Union[t.Type, t.Any]) -> None:
         """Check controller type"""
 
     def __init_subclass__(cls, **kwargs: t.Any) -> None:
         controller_type = kwargs.get("controller_type")
         assert controller_type, "Controller type is required"
         _register_controller_builder(controller_type, cls)
+
+
+class _DefaultRouterBuilder(RouterBuilder, controller_type=Mount):
+    @classmethod
+    def check_type(cls, controller_type: t.Union[t.Type, t.Any]) -> None:
+        """Do nothing"""
+
+    @classmethod
+    def build(
+        cls, controller_type: t.Union[t.Type, t.Any]
+    ) -> t.Union["ModuleMount", Mount, t.Any]:
+        """Build controller to Mount"""
+        return controller_type
+
+
+_register_controller_builder(Host, _DefaultRouterBuilder)
```

### Comparing `ellar-0.3.8/ellar/common/routing/controller/base.py` & `ellar-0.4.0/ellar/common/routing/controller/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 import typing as t
 
-from ellar.common.constants import CONTROLLER_CLASS_KEY
 from ellar.common.interfaces import IExecutionContext
 from ellar.common.models import ControllerBase
-from ellar.reflect import reflect
 
 
 class ControllerRouteOperationBase:
     endpoint: t.Callable
+    get_controller_type: t.Callable
 
     def _get_controller_instance(self, ctx: IExecutionContext) -> ControllerBase:
-        controller_type: t.Optional[t.Type[ControllerBase]] = reflect.get_metadata(
-            CONTROLLER_CLASS_KEY, self.endpoint
-        )
-        if not controller_type or (
-            controller_type and not issubclass(controller_type, ControllerBase)
-        ):
-            raise RuntimeError("Controller Type was not found")
+        controller_type: t.Optional[t.Type[ControllerBase]] = self.get_controller_type()
 
         service_provider = ctx.get_service_provider()
 
         controller_instance: ControllerBase = service_provider.get(controller_type)
         controller_instance.context = ctx
         return controller_instance
```

### Comparing `ellar-0.3.8/ellar/common/routing/controller/factory.py` & `ellar-0.4.0/ellar/core/routing/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 
 from ellar.common.constants import (
     CONTROLLER_METADATA,
     CONTROLLER_OPERATION_HANDLER_KEY,
     CONTROLLER_WATERMARK,
 )
 from ellar.common.models import ControllerBase, ControllerType
+from ellar.common.routing import ModuleMount, RouteCollection
 from ellar.reflect import reflect
 
-from ..builder import RouterBuilder
-from ..mount import ModuleMount
-from ..route_collections import RouteCollection
+from .builder import RouterBuilder
 
 
 class ControllerRouterFactory(RouterBuilder, controller_type=type(ControllerBase)):
     @classmethod
     def build(
         cls, controller_type: t.Union[t.Type[ControllerBase], t.Any]
     ) -> ModuleMount:
```

### Comparing `ellar-0.3.8/ellar/common/routing/controller/websocket/handler.py` & `ellar-0.4.0/ellar/common/routing/controller/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/routing/mount.py` & `ellar-0.4.0/ellar/common/routing/mount.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 from starlette.types import ASGIApp
 
 from ellar.common.compatible import AttributeDict
 from ellar.common.constants import (
     CONTROLLER_CLASS_KEY,
     GUARDS_KEY,
     NOT_SET,
-    OPERATION_ENDPOINT_KEY,
     VERSIONING_KEY,
 )
 from ellar.common.helper import get_unique_control_type
 from ellar.common.models import GuardCanActivate
 from ellar.common.types import TReceive, TScope, TSend
 from ellar.reflect import reflect
 
-from .operation_definitions import OperationDefinitions, TOperation, TWebsocketOperation
+from .operation_definitions import OperationDefinitions
 from .route import RouteOperation
 from .route_collections import RouteCollection
 from .schema import RouteParameters, WsRouteParameters
 
 __all__ = ["ModuleMount", "ModuleRouter"]
 
 
@@ -142,37 +141,36 @@
             app=app,
             control_type=get_unique_control_type(),
         )
         reflect.define_metadata(GUARDS_KEY, guards or [], self.get_control_type())
         reflect.define_metadata(
             VERSIONING_KEY, set(version or []), self.get_control_type()
         )
+        self._pre_build_routes: t.List[t.Union[RouteParameters, WsRouteParameters]] = []
 
-    def _get_operation(self, route_parameter: RouteParameters) -> TOperation:
-        _operation_class = self._get_http_operations_class(route_parameter.endpoint)
-        _operation = _operation_class(**route_parameter.dict())
-        setattr(route_parameter.endpoint, OPERATION_ENDPOINT_KEY, True)
-        self._set_other_router_attributes(_operation)
-        return _operation
-
-    def _get_ws_operation(
-        self, ws_route_parameters: WsRouteParameters
-    ) -> TWebsocketOperation:
-        _ws_operation_class = self._get_ws_operations_class(
-            ws_route_parameters.endpoint
-        )
-        _operation = _ws_operation_class(**ws_route_parameters.dict())
-        setattr(ws_route_parameters.endpoint, OPERATION_ENDPOINT_KEY, True)
-        self._set_other_router_attributes(_operation)
-        return _operation
+    def get_pre_build_routes(
+        self,
+    ) -> t.List[t.Union[RouteParameters, WsRouteParameters]]:
+        return self._pre_build_routes
 
-    def _set_other_router_attributes(
-        self, operation: t.Union[TWebsocketOperation, TOperation]
-    ) -> None:
-        if not reflect.has_metadata(CONTROLLER_CLASS_KEY, operation.endpoint):
+    def clear_pre_build_routes(self) -> None:
+        self._pre_build_routes.clear()
+
+    def _get_operation(self, route_parameter: RouteParameters) -> t.Callable:
+        endpoint = super()._get_operation(route_parameter)
+        self._pre_build_routes.append(route_parameter)
+        self._set_other_router_attributes(endpoint)
+        return endpoint
+
+    def _get_ws_operation(self, ws_route_parameters: WsRouteParameters) -> t.Callable:
+        endpoint = super()._get_ws_operation(ws_route_parameters)
+        self._pre_build_routes.append(ws_route_parameters)
+        self._set_other_router_attributes(endpoint)
+        return endpoint
+
+    def _set_other_router_attributes(self, operation_handler: t.Callable) -> None:
+        if not reflect.has_metadata(CONTROLLER_CLASS_KEY, operation_handler):
             # this is need to happen before adding operation to router else we lose ability to
             # get extra information about operation that is set on the router.
             reflect.define_metadata(
-                CONTROLLER_CLASS_KEY, self.get_control_type(), operation.endpoint
+                CONTROLLER_CLASS_KEY, self.get_control_type(), operation_handler
             )
-
-        self.app.routes.append(operation)  # type:ignore
```

### Comparing `ellar-0.3.8/ellar/common/routing/operation_definitions.py` & `ellar-0.4.0/ellar/common/routing/operation_definitions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,45 @@
 import functools
 import typing as t
 from functools import partial
 from types import FunctionType
 
 from ellar.common.constants import (
-    CONTROLLER_OPERATION_HANDLER_KEY,
     DELETE,
     GET,
     HEAD,
     OPERATION_ENDPOINT_KEY,
     OPTIONS,
     PATCH,
     POST,
     PUT,
+    ROUTE_OPERATION_PARAMETERS,
     TRACE,
 )
-from ellar.common.helper import class_base_function_regex
-from ellar.common.types import TCallable
-from ellar.reflect import reflect
-
-from .controller.route import ControllerRouteOperation
-from .controller.websocket.route import ControllerWebsocketRouteOperation
-from .route import RouteOperation
-from .schema import RouteParameters, WsRouteParameters
-from .websocket import WebsocketRouteOperation
 
-TOperation = t.Union[RouteOperation, ControllerRouteOperation]
-TWebsocketOperation = t.Union[
-    WebsocketRouteOperation, ControllerWebsocketRouteOperation
-]
+from .schema import RouteParameters, WsRouteParameters
 
 
 def _websocket_connection_attributes(func: t.Callable) -> t.Callable:
     def _advance_function(
         websocket_handler: t.Callable, handler_name: str
     ) -> t.Callable:
         def _wrap(connect_handler: t.Callable) -> t.Callable:
             if not (
                 callable(websocket_handler) and type(websocket_handler) == FunctionType
             ):
                 raise Exception(
                     "Invalid type. Please make sure you passed the websocket handler."
                 )
 
-            _item: t.Optional[WebsocketRouteOperation] = reflect.get_metadata(
-                CONTROLLER_OPERATION_HANDLER_KEY, websocket_handler
+            _item: t.Optional[WsRouteParameters] = getattr(
+                websocket_handler, ROUTE_OPERATION_PARAMETERS, None
             )
 
-            if not _item or not isinstance(_item, WebsocketRouteOperation):
+            if not _item or not isinstance(_item, WsRouteParameters):
                 raise Exception(
                     "Invalid type. Please make sure you passed the websocket handler."
                 )
 
             _item.add_websocket_handler(
                 handler_name=handler_name, handler=connect_handler
             )
@@ -70,49 +58,51 @@
     )
     return func
 
 
 class OperationDefinitions:
     __slots__ = ()
 
-    def _get_http_operations_class(self, func: t.Callable) -> t.Type[TOperation]:
-        if class_base_function_regex.match(repr(func)):
-            return ControllerRouteOperation
-        return RouteOperation
-
-    def _get_ws_operations_class(self, func: t.Callable) -> t.Type[TWebsocketOperation]:
-        if class_base_function_regex.match(repr(func)):
-            return ControllerWebsocketRouteOperation
-        return WebsocketRouteOperation
-
-    def _get_operation(self, route_parameter: RouteParameters) -> TOperation:
-        _operation_class = self._get_http_operations_class(route_parameter.endpoint)
-        _operation = _operation_class(**route_parameter.dict())
+    # def _get_http_operations_class(self, func: t.Callable) -> t.Type[TOperation]:
+    #     if class_base_function_regex.match(repr(func)):
+    #         return ControllerRouteOperation
+    #     return RouteOperation
+    #
+    # def _get_ws_operations_class(self, func: t.Callable) -> t.Type[TWebsocketOperation]:
+    #     if class_base_function_regex.match(repr(func)):
+    #         return ControllerWebsocketRouteOperation
+    #     return WebsocketRouteOperation
+
+    def _get_operation(self, route_parameter: RouteParameters) -> t.Callable:
         setattr(route_parameter.endpoint, OPERATION_ENDPOINT_KEY, True)
-        return _operation
+        setattr(route_parameter.endpoint, ROUTE_OPERATION_PARAMETERS, route_parameter)
+        return route_parameter.endpoint
 
-    def _get_ws_operation(
-        self, ws_route_parameters: WsRouteParameters
-    ) -> TWebsocketOperation:
-        _ws_operation_class = self._get_ws_operations_class(
-            ws_route_parameters.endpoint
-        )
-        _operation = _ws_operation_class(**ws_route_parameters.dict())
+    def _get_ws_operation(self, ws_route_parameters: WsRouteParameters) -> t.Callable:
+        # _ws_operation_class = self._get_ws_operations_class(
+        #     ws_route_parameters.endpoint
+        # )
+        # _operation = _ws_operation_class(**ws_route_parameters.dict())
         setattr(ws_route_parameters.endpoint, OPERATION_ENDPOINT_KEY, True)
-        return _operation
+        setattr(
+            ws_route_parameters.endpoint,
+            ROUTE_OPERATION_PARAMETERS,
+            ws_route_parameters,
+        )
+        return ws_route_parameters.endpoint
 
     def _get_decorator_or_operation(
         self, path: t.Union[str, t.Callable], endpoint_parameter_partial: t.Callable
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
+    ) -> t.Callable:
         if callable(path):
             route_parameter = endpoint_parameter_partial(endpoint=path, path="/")
             self._get_operation(route_parameter=route_parameter)
             return path
 
-        def _decorator(endpoint_handler: TCallable) -> TCallable:
+        def _decorator(endpoint_handler: t.Callable) -> t.Callable:
             _route_parameter = endpoint_parameter_partial(
                 endpoint=endpoint_handler, path=path
             )
             self._get_operation(route_parameter=_route_parameter)
             return endpoint_handler
 
         return _decorator
@@ -122,15 +112,15 @@
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
             t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
+    ) -> t.Callable:
         methods = [GET]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
             include_in_schema=include_in_schema,
             response=response,
@@ -142,15 +132,15 @@
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
             t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
+    ) -> t.Callable:
         methods = [POST]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
             include_in_schema=include_in_schema,
             response=response,
@@ -162,15 +152,15 @@
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
             t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
+    ) -> t.Callable:
         methods = [PUT]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
             include_in_schema=include_in_schema,
             response=response,
@@ -182,15 +172,15 @@
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
             t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
+    ) -> t.Callable:
         methods = [PATCH]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
             include_in_schema=include_in_schema,
             response=response,
@@ -202,15 +192,15 @@
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
             t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
+    ) -> t.Callable:
         methods = [DELETE]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
             include_in_schema=include_in_schema,
             response=response,
@@ -222,15 +212,15 @@
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
             t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
+    ) -> t.Callable:
         methods = [HEAD]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
             include_in_schema=include_in_schema,
             response=response,
@@ -242,15 +232,15 @@
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
             t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
+    ) -> t.Callable:
         methods = [OPTIONS]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
             include_in_schema=include_in_schema,
             response=response,
@@ -262,15 +252,15 @@
         path: str = "/",
         *,
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
             t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
+    ) -> t.Callable:
         methods = [TRACE]
         endpoint_parameter_partial = partial(
             RouteParameters,
             name=name,
             methods=methods,
             include_in_schema=include_in_schema,
             response=response,
@@ -283,16 +273,16 @@
         *,
         methods: t.List[str],
         name: str = None,
         include_in_schema: bool = True,
         response: t.Union[
             t.Dict[int, t.Type], t.List[t.Tuple[int, t.Type]], t.Type, t.Any
         ] = None,
-    ) -> t.Callable[[TCallable], t.Union[TOperation, TCallable]]:
-        def _decorator(endpoint_handler: TCallable) -> TCallable:
+    ) -> t.Callable:
+        def _decorator(endpoint_handler: t.Callable) -> t.Callable:
             endpoint_parameter = RouteParameters(
                 name=name,
                 path=path,
                 methods=methods,
                 include_in_schema=include_in_schema,
                 response=response,
                 endpoint=endpoint_handler,
@@ -307,18 +297,18 @@
         self,
         path: str = "/",
         *,
         name: str = None,
         encoding: t.Optional[str] = "json",
         use_extra_handler: bool = False,
         extra_handler_type: t.Optional[t.Type] = None,
-    ) -> t.Callable[[TCallable], t.Union[TCallable, TWebsocketOperation]]:
+    ) -> t.Callable:
         def _decorator(
-            endpoint_handler: TCallable,
-        ) -> t.Union[TCallable, TWebsocketOperation]:
+            endpoint_handler: t.Callable,
+        ) -> t.Callable:
             endpoint_parameter = WsRouteParameters(
                 name=name,
                 path=path,
                 endpoint=endpoint_handler,
                 encoding=encoding,
                 use_extra_handler=use_extra_handler,
                 extra_handler_type=extra_handler_type,
```

### Comparing `ellar-0.3.8/ellar/common/routing/params.py` & `ellar-0.4.0/ellar/common/params/decorators.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/routing/route.py` & `ellar-0.4.0/ellar/common/routing/route.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,23 +41,23 @@
         path: str,
         methods: t.List[str],
         endpoint: t.Callable,
         response: t.Mapping[int, t.Union[t.Type, t.Any]],
         name: t.Optional[str] = None,
         include_in_schema: bool = True,
     ) -> None:
+        super().__init__(endpoint=endpoint)
         self._is_coroutine = inspect.iscoroutinefunction(endpoint)
         self._defined_responses: t.Dict[int, t.Type] = dict(response)
 
         assert path.startswith("/"), "Routed paths must start with '/'"
         self.path = path
         self.path_regex, self.path_format, self.param_convertors = compile_path(
             self.path
         )
-        self.endpoint = endpoint  # type: ignore
 
         self.name = get_name(endpoint) if name is None else name
         self.include_in_schema = include_in_schema
         self.methods = self.get_methods(methods)
 
         self.endpoint_parameter_model: RequestEndpointArgsModel = NOT_SET
         self.response_model: RouteResponseModel = NOT_SET
@@ -65,15 +65,15 @@
         reflect.define_metadata(CONTROLLER_OPERATION_HANDLER_KEY, self, self.endpoint)
         self._load_model()
 
     def _load_model(self) -> None:
         extra_route_args: t.Union[t.List["ExtraEndpointArg"], "ExtraEndpointArg"] = (
             reflect.get_metadata(EXTRA_ROUTE_ARGS_KEY, self.endpoint) or []
         )
-        if not isinstance(extra_route_args, list):
+        if not isinstance(extra_route_args, list):  # pragma: no cover
             extra_route_args = [extra_route_args]
 
         if self.endpoint_parameter_model is NOT_SET:
             self.endpoint_parameter_model = self.request_endpoint_args_model(
                 path=self.path_format,
                 endpoint=self.endpoint,
                 operation_unique_id=self.get_operation_unique_id(methods=self.methods),
@@ -102,22 +102,30 @@
         _methods: t.Sequence[str] = (
             list(methods) if isinstance(methods, set) else [t.cast(str, methods)]
         )
         return generate_operation_unique_id(
             name=self.name, path=self.path_format, methods=_methods
         )
 
-    async def _handle_request(self, context: IExecutionContext) -> None:
+    async def run(self, context: IExecutionContext, kwargs: t.Dict) -> t.Any:
+        if self._is_coroutine:
+            return await self.endpoint(**kwargs)
+        else:
+            return await run_in_threadpool(self.endpoint, **kwargs)
+
+    async def handle_request(self, context: IExecutionContext) -> t.Any:
         func_kwargs, errors = await self.endpoint_parameter_model.resolve_dependencies(
             ctx=context
         )
         if errors:
             raise RequestValidationError(errors)
-        if self._is_coroutine:
-            response_obj = await self.endpoint(**func_kwargs)
-        else:
-            response_obj = await run_in_threadpool(self.endpoint, **func_kwargs)
+
+        return await self.run(context, func_kwargs)
+
+    async def handle_response(
+        self, context: IExecutionContext, response_obj: t.Any
+    ) -> None:
         response = self.response_model.process_response(
             ctx=context, response_obj=response_obj
         )
         if isinstance(response, Response):
             await response(*context.get_args())
```

### Comparing `ellar-0.3.8/ellar/common/routing/route_collections.py` & `ellar-0.4.0/ellar/common/routing/route_collections.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,15 @@
 import typing as t
 import uuid
 from collections import OrderedDict
 
 from starlette.routing import BaseRoute, Host, Mount
 
-from ellar.common.constants import CONTROLLER_CLASS_KEY
-from ellar.common.helper import (
-    generate_controller_operation_unique_id,
-    get_unique_control_type,
-)
+from ellar.common.helper import generate_controller_operation_unique_id
 from ellar.common.logger import logger
-from ellar.reflect import reflect
-
-from .base import RouteOperationBase
-from .route import RouteOperation
-from .websocket.route import WebsocketRouteOperation
 
 
 class RouteCollection(t.Sequence[BaseRoute]):
     __slots__ = ("_routes", "_served_routes")
 
     def __init__(self, routes: t.Optional[t.Sequence[BaseRoute]] = None) -> None:
         self._routes: t.Dict[int, BaseRoute] = OrderedDict()
@@ -55,29 +46,20 @@
     def sort_routes(self) -> None:
         # TODO: flatten the routes for faster look up
         self._served_routes = list(self._routes.values())
         self._served_routes.sort(
             key=lambda e: e.host if isinstance(e, Host) else e.path  # type: ignore
         )
 
-    def _add_operation(
-        self, operation: t.Union[RouteOperation, WebsocketRouteOperation, BaseRoute]
-    ) -> None:
+    def _add_operation(self, operation: t.Union[BaseRoute]) -> None:
 
         if not isinstance(operation, BaseRoute):
             logger.warning("Tried Adding an operation that is not supported.")
             return
 
-        if isinstance(operation, RouteOperationBase) and not reflect.has_metadata(
-            CONTROLLER_CLASS_KEY, operation.endpoint
-        ):
-            reflect.define_metadata(
-                CONTROLLER_CLASS_KEY, get_unique_control_type(), operation.endpoint
-            )
-
         _methods = getattr(operation, "methods", {"WS"})
         _versioning = list(
             operation.get_allowed_version()  # type: ignore
             if hasattr(operation, "get_allowed_version")
             else {}
         )
         path = operation.host if isinstance(operation, Host) else operation.path  # type: ignore
```

### Comparing `ellar-0.3.8/ellar/common/routing/schema.py` & `ellar-0.4.0/ellar/common/routing/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 
-from pydantic import BaseModel, Field, root_validator, validator
+from pydantic import BaseModel, Field, PrivateAttr, root_validator, validator
 
 from ellar.common.constants import ROUTE_METHODS
 from ellar.common.interfaces import IResponseModel
 from ellar.common.responses.models import EmptyAPIResponseModel, create_response_model
 from ellar.common.serializer import BaseSerializer
 
 if t.TYPE_CHECKING:  # pragma: no cover
@@ -52,21 +52,21 @@
 
         if not_valid_methods:
             raise ValueError(f"Method {','.join(not_valid_methods)} not allowed")
         return methods
 
     @validator("endpoint")
     def validate_endpoint(cls, value: t.Any) -> t.Any:
-        if not callable(value):
+        if not callable(value):  # pragma: no cover
             raise ValueError("An endpoint must be a callable")
         return value
 
     @root_validator
     def validate_root(cls, values: t.Any) -> t.Any:
-        if "response" not in values:
+        if "response" not in values:  # pragma: no cover
             raise ValueError(
                 "Expected "
                 "IResponseModel | Dict[int, Any | Type[BaseModel] | "
                 "Type[BaseSerializer] | IResponseModel]  | Type[BaseModel] | Type[BaseSerializer]"
             )
 
         response = values["response"]
@@ -80,19 +80,32 @@
 class WsRouteParameters(BaseModel):
     path: str
     name: t.Optional[str] = None
     endpoint: t.Callable
     encoding: t.Optional[str] = Field("json")
     use_extra_handler: bool = Field(False)
     extra_handler_type: t.Optional[t.Type["WebSocketExtraHandler"]] = None
+    _kwargs: t.Dict = PrivateAttr()
+
+    def __init__(self, **data: t.Any) -> None:
+        super().__init__(**data)
+        self._kwargs = {}
 
     @validator("endpoint")
     def validate_endpoint(cls, value: t.Any) -> t.Any:
         return value
 
     @validator("encoding")
     def validate_encoding(cls, value: t.Any) -> t.Any:
         if value not in ["json", "text", "bytes", None]:
             raise ValueError(
                 f"Encoding type not supported. Once [json | text | bytes]. Received: {value}"
             )
         return value
+
+    def dict(self, *args: t.Any, **kwargs: t.Any) -> t.Dict:
+        data = super().dict(*args, **kwargs)
+        data.update(self._kwargs)
+        return data
+
+    def add_websocket_handler(self, handler_name: str, handler: t.Callable) -> None:
+        self._kwargs[handler_name] = handler
```

### Comparing `ellar-0.3.8/ellar/common/routing/websocket/handler.py` & `ellar-0.4.0/ellar/common/routing/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/routing/websocket/route.py` & `ellar-0.4.0/ellar/common/routing/websocket/route.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         name: t.Optional[str] = None,
         endpoint: t.Callable,
         encoding: str = "json",
         use_extra_handler: bool = False,
         extra_handler_type: t.Optional[t.Type[WebSocketExtraHandler]] = None,
         **handlers_kwargs: t.Any,
     ) -> None:
+        super().__init__(endpoint=endpoint)
         assert path.startswith("/"), "Routed paths must start with '/'"
         self._handlers_kwargs: t.Dict[str, t.Any] = dict(
             encoding=encoding,
             on_receive=None,
             on_connect=None,
             on_disconnect=None,
         )
@@ -58,15 +59,14 @@
             t.Type[WebSocketExtraHandler]
         ] = extra_handler_type
 
         self.path = path
         self.path_regex, self.path_format, self.param_convertors = compile_path(
             self.path
         )
-        self.endpoint = endpoint  # type: ignore
         self.name = get_name(endpoint) if name is None else name
 
         self.endpoint_parameter_model: WebsocketEndpointArgsModel = NOT_SET
 
         reflect.define_metadata(CONTROLLER_OPERATION_HANDLER_KEY, self, self.endpoint)
 
         if self._use_extra_handler:
@@ -80,40 +80,48 @@
     def add_websocket_handler(self, handler_name: str, handler: t.Callable) -> None:
         if handler_name not in self._handlers_kwargs:
             raise Exception(
                 f"Invalid Handler Name. Handler Name must be in {list(self._handlers_kwargs.keys())}"
             )
         self._handlers_kwargs.update({handler_name: handler})
 
-    async def _handle_request(self, context: IExecutionContext) -> None:
+    async def run(self, context: IExecutionContext, kwargs: t.Dict) -> t.Any:
+        if self._use_extra_handler:
+            ws_extra_handler_type = (
+                self._extra_handler_type or self.get_websocket_handler()
+            )
+            ws_extra_handler = ws_extra_handler_type(
+                route_parameter_model=self.endpoint_parameter_model,
+                **self._handlers_kwargs,
+            )
+            return await ws_extra_handler.dispatch(context=context, **kwargs)
+        else:
+            return await self.endpoint(**kwargs)
+
+    async def handle_request(self, context: IExecutionContext) -> t.Any:
         func_kwargs, errors = await self.endpoint_parameter_model.resolve_dependencies(
             ctx=context
         )
         if errors:
             websocket = context.switch_to_websocket().get_client()
             exc = WebSocketRequestValidationError(errors)
             if websocket.client_state == WebSocketState.CONNECTING:
                 await websocket.accept()
             await websocket.send_json(
                 dict(code=WS_1008_POLICY_VIOLATION, errors=exc.errors())
             )
             await websocket.close(code=WS_1008_POLICY_VIOLATION)
             raise exc
 
-        if self._use_extra_handler:
-            ws_extra_handler_type = (
-                self._extra_handler_type or self.get_websocket_handler()
-            )
-            ws_extra_handler = ws_extra_handler_type(
-                route_parameter_model=self.endpoint_parameter_model,
-                **self._handlers_kwargs,
-            )
-            await ws_extra_handler.dispatch(context=context, **func_kwargs)
-        else:
-            await self.endpoint(**func_kwargs)
+        return await self.run(context, func_kwargs)
+
+    async def handle_response(
+        self, context: IExecutionContext, response_obj: t.Any
+    ) -> None:
+        """Websocket has no response"""
 
     def _load_model(self) -> None:
         extra_route_args: t.List["ExtraEndpointArg"] = (
             reflect.get_metadata(EXTRA_ROUTE_ARGS_KEY, self.endpoint) or []
         )
 
         if self.endpoint_parameter_model is NOT_SET:
```

### Comparing `ellar-0.3.8/ellar/common/serializer/base.py` & `ellar-0.4.0/ellar/common/serializer/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from pydantic.json import ENCODERS_BY_TYPE
 
 __pydantic_model__ = "__pydantic_model__"
 __pydantic_config__ = "__config__"
 __pydantic_root__ = "__root__"
 
 
+@t.no_type_check
 def get_dataclass_pydantic_model(
     dataclass_type: t.Type,
 ) -> t.Optional[t.Type[BaseModel]]:
 
     if hasattr(dataclass_type, __pydantic_model__):
         return t.cast(t.Type[BaseModel], dataclass_type.__dict__[__pydantic_model__])
-    return None
 
 
 class SerializerConfig(BaseConfig):
     orm_mode = True
 
 
 @PydanticDataclasses.dataclass
```

### Comparing `ellar-0.3.8/ellar/common/templating/__init__.py` & `ellar-0.4.0/ellar/common/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/templating/loader.py` & `ellar-0.4.0/ellar/common/templating/loader.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/templating/model.py` & `ellar-0.4.0/ellar/common/templating/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/templating/renderer.py` & `ellar-0.4.0/ellar/common/templating/renderer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/common/types.py` & `ellar-0.4.0/ellar/common/types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/__init__.py` & `ellar-0.4.0/ellar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/conf/app_settings_models.py` & `ellar-0.4.0/ellar/core/conf/app_settings_models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/conf/config.py` & `ellar-0.4.0/ellar/core/conf/config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/conf/mixins.py` & `ellar-0.4.0/ellar/core/conf/mixins.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/connection/http.py` & `ellar-0.4.0/ellar/core/connection/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/context/execution.py` & `ellar-0.4.0/ellar/core/context/execution.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import typing as t
 
-from ellar.common.constants import CONTROLLER_CLASS_KEY
 from ellar.common.interfaces import IExecutionContext
 from ellar.common.models import ControllerBase
 from ellar.common.types import TReceive, TScope, TSend
 from ellar.core.services.reflector import Reflector
 
 from .host import HostContext
 
@@ -19,25 +18,23 @@
     def __init__(
         self,
         *,
         scope: TScope,
         receive: TReceive,
         send: TSend,
         operation_handler: t.Callable,
+        operation_handler_type: t.Type,
         reflector: Reflector,
     ) -> None:
         super(ExecutionContext, self).__init__(scope=scope, receive=receive, send=send)
         self._operation_handler = operation_handler
         self.reflector = reflector
-        _handler_controller_class = self.reflector.get(
-            CONTROLLER_CLASS_KEY, self.get_handler()
-        )
 
         self._handler_controller_class: t.Optional[t.Type["ControllerBase"]] = t.cast(
-            t.Optional[t.Type["ControllerBase"]], _handler_controller_class
+            t.Optional[t.Type["ControllerBase"]], operation_handler_type
         )
 
     def get_handler(self) -> t.Callable:
         assert self._operation_handler, "Operation is not available yet."
         return self._operation_handler
 
     def get_class(self) -> t.Optional[t.Type["ControllerBase"]]:
```

### Comparing `ellar-0.3.8/ellar/core/context/factory.py` & `ellar-0.4.0/ellar/core/context/factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,11 +72,12 @@
     ) -> IExecutionContext:
 
         i_execution_context = ExecutionContext(
             scope=scope,
             receive=receive,
             send=send,
             operation_handler=operation.endpoint,
+            operation_handler_type=operation.get_controller_type(),
             reflector=self.reflector,
         )
 
         return i_execution_context
```

### Comparing `ellar-0.3.8/ellar/core/context/host.py` & `ellar-0.4.0/ellar/core/context/host.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/context/http.py` & `ellar-0.4.0/ellar/core/context/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/context/websocket.py` & `ellar-0.4.0/ellar/core/context/websocket.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/core_service_registration.py` & `ellar-0.4.0/ellar/core/core_service_registration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import typing as t
 
 from ellar.common import (
     IExceptionMiddlewareService,
     IExecutionContextFactory,
+    IGuardsConsumer,
     IHostContextFactory,
     IHTTPConnectionContextFactory,
+    IInterceptorsConsumer,
     IWebSocketContextFactory,
 )
 from ellar.core.services import Reflector
 from ellar.di import EllarInjector
 
 from .context import ExecutionContextFactory, HostContextFactory
 from .context.factory import HTTPConnectionContextFactory, WebSocketContextFactory
 from .exceptions.service import ExceptionMiddlewareService
+from .guard import GuardConsumer
+from .interceptors import EllarInterceptorConsumer
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.conf import Config
 
 
 class CoreServiceRegistration:
     """Create Binding for all application service"""
@@ -42,7 +46,11 @@
         )
 
         self.injector.container.register_scoped(
             IWebSocketContextFactory, WebSocketContextFactory
         )
 
         self.injector.container.register(Reflector)
+        self.injector.container.register_singleton(
+            IInterceptorsConsumer, EllarInterceptorConsumer
+        )
+        self.injector.container.register_singleton(IGuardsConsumer, GuardConsumer)
```

### Comparing `ellar-0.3.8/ellar/core/exceptions/service.py` & `ellar-0.4.0/ellar/core/exceptions/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/factory.py` & `ellar-0.4.0/ellar/core/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/guard/apikey.py` & `ellar-0.4.0/ellar/core/guard/apikey.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/guard/http.py` & `ellar-0.4.0/ellar/core/guard/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/main.py` & `ellar-0.4.0/ellar/core/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from starlette.routing import BaseRoute, Mount
 
 from ellar.common.compatible import cached_property
 from ellar.common.constants import LOG_LEVELS
 from ellar.common.datastructures import State, URLPath
 from ellar.common.interfaces import IExceptionHandler, IExceptionMiddlewareService
 from ellar.common.logger import logger
-from ellar.common.models import GuardCanActivate
+from ellar.common.models import EllarInterceptor, GuardCanActivate
 from ellar.common.templating import Environment
 from ellar.common.types import ASGIApp, T, TReceive, TScope, TSend
 from ellar.core.middleware import (
     CORSMiddleware,
     ExceptionMiddleware,
     Middleware,
     RequestServiceProviderMiddleware,
@@ -50,14 +50,17 @@
             injector, EllarInjector
         ), "injector must instance of EllarInjector"
 
         self._config = config
         self._injector: EllarInjector = injector
 
         self._global_guards = [] if global_guards is None else list(global_guards)
+        self._global_interceptors: t.List[
+            t.Union[EllarInterceptor, t.Type[EllarInterceptor]]
+        ] = []
         self._exception_handlers = list(self.config.EXCEPTION_HANDLERS)
 
         self._user_middleware = list(t.cast(list, self.config.MIDDLEWARE))
 
         self._static_app: t.Optional[ASGIApp] = None
 
         self.state = State()
@@ -139,19 +142,29 @@
         self.rebuild_middleware_stack()
 
         return t.cast(T, module_ref.get_module_instance())
 
     def get_guards(self) -> t.List[t.Union[t.Type[GuardCanActivate], GuardCanActivate]]:
         return self._global_guards
 
+    def get_interceptors(
+        self,
+    ) -> t.List[t.Union[EllarInterceptor, t.Type[EllarInterceptor]]]:
+        return self._global_interceptors
+
     def use_global_guards(
         self, *guards: t.Union["GuardCanActivate", t.Type["GuardCanActivate"]]
     ) -> None:
         self._global_guards.extend(guards)
 
+    def use_global_interceptors(
+        self, *interceptors: t.Union[EllarInterceptor, t.Type[EllarInterceptor]]
+    ) -> None:
+        self._global_interceptors.extend(interceptors)
+
     @property
     def injector(self) -> EllarInjector:
         return self._injector
 
     @property
     def versioning_scheme(self) -> BaseAPIVersioning:
         return t.cast(BaseAPIVersioning, self._config.VERSIONING_SCHEME)
```

### Comparing `ellar-0.3.8/ellar/core/middleware/__init__.py` & `ellar-0.4.0/ellar/core/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/middleware/di.py` & `ellar-0.4.0/ellar/core/middleware/di.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,28 +34,29 @@
         if scope["type"] not in ["http", "websocket"]:  # pragma: no cover
             await super().__call__(scope, receive, send)
             return
 
         scope[SCOPE_RESPONSE_STARTED] = False
 
         async def sender(message: TMessage) -> None:
-            if message["type"] == "http.response.start":
+            if (
+                message["type"] == "http.response.start"
+                or message["type"] == "websocket.accept"
+            ):
                 scope[SCOPE_RESPONSE_STARTED] = True
             await send(message)
             return
 
-        _sender = sender if scope["type"] == "http" else send
-
         async with self.injector.create_asgi_args() as service_provider:
             scope[SCOPE_SERVICE_PROVIDER] = service_provider
 
             if scope["type"] == "http":
-                await super().__call__(scope, receive, _sender)
+                await super().__call__(scope, receive, sender)
             else:
-                await self.app(scope, receive, _sender)
+                await self.app(scope, receive, sender)
 
     async def error_handler(self, request: Request, exc: Exception) -> Response:
         host_context_factory: IHostContextFactory = request.scope[
             SCOPE_SERVICE_PROVIDER
         ].get(IHostContextFactory)
         host_context = host_context_factory.create_context(request.scope)
```

### Comparing `ellar-0.3.8/ellar/core/middleware/exceptions.py` & `ellar-0.4.0/ellar/core/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/middleware/function.py` & `ellar-0.4.0/ellar/core/middleware/function.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/middleware/versioning.py` & `ellar-0.4.0/ellar/core/middleware/versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/modules/base.py` & `ellar-0.4.0/ellar/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/modules/builder.py` & `ellar-0.4.0/ellar/core/modules/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,10 +81,10 @@
             self._cls,
         )
 
     def build(self, namespace: t.Dict) -> None:
         for name, item in namespace.items():
             for k, func in self._actions.items():
                 if hasattr(item, k):
-                    value = getattr(item, k)
+                    value = item.__dict__.pop(k)
                     func(value)
                     self._cls.__MODULE_FIELDS__[name] = item
```

### Comparing `ellar-0.3.8/ellar/core/modules/config.py` & `ellar-0.4.0/ellar/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/modules/helper.py` & `ellar-0.4.0/ellar/core/modules/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/modules/ref.py` & `ellar-0.4.0/ellar/core/modules/ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
     MODULE_METADATA,
     MODULE_WATERMARK,
     TEMPLATE_FILTER_KEY,
     TEMPLATE_GLOBAL_KEY,
 )
 from ellar.common.models import ControllerBase
 from ellar.common.routing import ModuleMount
-from ellar.common.routing.builder import get_controller_builder_factory
 from ellar.common.templating import ModuleTemplating
 from ellar.di import (
     MODULE_REF_TYPES,
     Container,
     ProviderConfig,
     injectable,
     is_decorated_with_injectable,
 )
 from ellar.di.providers import ModuleProvider
 from ellar.reflect import reflect
 
+from ..routing import get_controller_builder_factory
 from .base import ModuleBase, ModuleBaseMeta
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core import Config
 
 
 class InvalidModuleTypeException(Exception):
@@ -181,27 +181,25 @@
         self._static_folder: t.Optional[str] = reflect.get_metadata(
             MODULE_METADATA.STATIC_FOLDER, module_type
         )
         self._controllers: t.List[t.Type[ControllerBase]] = (
             reflect.get_metadata(MODULE_METADATA.CONTROLLERS, self._module_type) or []
         )
 
-        self._routers: t.Sequence[
-            t.Union[BaseRoute, ModuleMount, Mount]
-        ] = self._get_all_routers()
-        self._flatten_routes: t.List[BaseRoute] = []
+        self._routers: t.List[t.Union[BaseRoute]] = self._get_all_routers()
+        # self._flatten_routes: t.List[BaseRoute] = []
 
         if isinstance(self.module, type) and issubclass(self.module, ModuleBase):
             self.scan_templating_filters()
             self.scan_exceptions_handlers()
             self.scan_middleware()
 
         self.register_providers()
         self.register_controllers()
-        self._build_flatten_routes()
+        # self._build_flatten_routes()
 
     @property
     def module(self) -> t.Type[ModuleBase]:
         return self._module_type
 
     @property
     def container(self) -> Container:
@@ -213,31 +211,29 @@
 
     @property
     def routers(self) -> t.Sequence[t.Union[BaseRoute, ModuleMount, Mount]]:
         return self._routers
 
     @property
     def routes(self) -> t.List[BaseRoute]:
-        return self._flatten_routes
+        return self._routers
 
-    def _build_flatten_routes(self) -> None:
-        for router in self._routers:
-            # if isinstance(router, ModuleMount):
-            #     # TODO: Allow users to choose whether to run flatten route of group routes together
-            #     # router.build_child_routes()
-            #     self._flatten_routes.append(router)
-            #     continue
-            # if isinstance(router, BaseRoute):
-            #     self._flatten_routes.append(router)
-            if isinstance(router, BaseRoute):
-                self._flatten_routes.append(router)
+    # def _build_flatten_routes(self) -> None:
+    #     for router in self._routers:
+    #         # if isinstance(router, ModuleMount):
+    #         #     # TODO: Allow users to choose whether to run flatten route of group routes together
+    #         #     # router.build_child_routes()
+    #         #     self._flatten_routes.append(router)
+    #         #     continue
+    #         # if isinstance(router, BaseRoute):
+    #         #     self._flatten_routes.append(router)
+    #         if isinstance(router, BaseRoute):
+    #             self._flatten_routes.append(router)
 
     def _register_module(self) -> None:
-        if not is_decorated_with_injectable(self.module):
-            self._module_type = injectable()(self.module)
         self.container.register(
             self.module, ModuleProvider(self.module, **self._init_kwargs)
         )
 
     def scan_templating_filters(self) -> None:
         templating_filter = (
             reflect.get_metadata(TEMPLATE_FILTER_KEY, self._module_type) or {}
@@ -283,20 +279,18 @@
                 provider = ProviderConfig(item)
             provider.register(self._container)
 
     def register_controllers(self) -> None:
         for controller in self._controllers:
             ProviderConfig(controller).register(self._container)
 
-    # def run_application_ready(self, app: "App") -> None:
-    #     _module_type_instance = self._container.injector.get(self._module_type)
-    #     _module_type_instance.application_ready(app)
-
-    def _get_all_routers(self) -> t.Sequence[t.Union[ModuleMount, Mount, BaseRoute]]:
+    def _get_all_routers(self) -> t.List[BaseRoute]:
         _routers = list(
             reflect.get_metadata(MODULE_METADATA.ROUTERS, self._module_type) or []
         )
-        for controller in self._controllers:
+        result = []
+
+        for controller in self._controllers + _routers:
             factory_builder = get_controller_builder_factory(type(controller))
             factory_builder.check_type(controller)
-            _routers.append(factory_builder.build(controller))
-        return _routers
+            result.append(factory_builder.build(controller))
+        return result  # type: ignore[return-value]
```

### Comparing `ellar-0.3.8/ellar/core/routing/app.py` & `ellar-0.4.0/ellar/core/routing/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import typing as t
 from functools import wraps
-from types import FunctionType
 
 from starlette.routing import BaseRoute, Router as StarletteRouter
 
-from ellar.common.constants import (
-    CONTROLLER_OPERATION_HANDLER_KEY,
-    SCOPE_API_VERSIONING_RESOLVER,
-)
+from ellar.common.constants import SCOPE_API_VERSIONING_RESOLVER
 from ellar.common.routing import RouteCollection
 from ellar.common.types import ASGIApp, TReceive, TScope, TSend
-from ellar.reflect import reflect
+
+from .helper import build_route_handler
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.versioning.resolver import BaseAPIVersioningResolver
 
 __all__ = ["ApplicationRouter"]
 
 
@@ -52,17 +49,15 @@
             on_shutdown=on_shutdown,
             lifespan=lifespan,
         )
         self.default = router_default_decorator(self.default)
         self.routes: RouteCollection = RouteCollection(routes)
 
     def append(self, item: t.Union[BaseRoute, t.Callable]) -> None:
-        _item: t.Any = item
-        if callable(_item) and type(_item) == FunctionType:
-            _item = reflect.get_metadata(CONTROLLER_OPERATION_HANDLER_KEY, _item)
+        _item: t.Any = build_route_handler(item)
         self.routes.append(_item)
 
     def extend(self, routes: t.Sequence[t.Union[BaseRoute, t.Callable]]) -> None:
         for route in routes:
             self.append(route)
 
     def add_route(
```

### Comparing `ellar-0.3.8/ellar/core/services/reflector.py` & `ellar-0.4.0/ellar/core/services/reflector.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             item for item in self.get_all(metadata_key, *targets) if item
         ]
 
         if len(metadata_collection) == 0:
             return []
 
         if len(metadata_collection) == 1:
-            return metadata_collection[0]
+            return [metadata_collection[0]]
 
         @t.no_type_check
         def inline_function(previous_item: t.Any, next_item: t.Any) -> t.Any:
             if isinstance(previous_item, (list, tuple, set)):
                 previous_item.extend(
                     list(next_item)
                     if isinstance(next_item, (list, tuple, set))
```

### Comparing `ellar-0.3.8/ellar/core/staticfiles.py` & `ellar-0.4.0/ellar/core/staticfiles.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/templating/app.py` & `ellar-0.4.0/ellar/core/templating/app.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/versioning/__init__.py` & `ellar-0.4.0/ellar/core/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/versioning/base.py` & `ellar-0.4.0/ellar/core/versioning/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/core/versioning/resolver.py` & `ellar-0.4.0/ellar/core/versioning/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,29 +49,26 @@
             version is not None
             and version == str(self.default_version)
             or version in route_versions
         )
 
 
 class DefaultAPIVersionResolver(BaseAPIVersioningResolver):
-    def raise_exception(self) -> None:
-        raise NotFound()
-
     invalid_version_message = "Invalid API version"
 
+    def raise_exception(self) -> None:
+        raise NotFound(self.invalid_version_message)
+
     def resolve_version(self) -> str:
         return str(NOT_SET)
 
 
 class UrlPathVersionResolver(DefaultAPIVersionResolver):
     invalid_version_message = "Invalid version in URL path."
 
-    def raise_exception(self) -> None:
-        raise NotFound(self.invalid_version_message)
-
     def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         super(UrlPathVersionResolver, self).__init__(*args, **kwargs)
 
         prefix = "/{" + self.version_parameter + "}"
         self.path_regex, self.path_format, self.param_convertors = compile_path(
             prefix + "/{path:path}"
         )
@@ -133,17 +130,14 @@
         version = accept.get(self.version_parameter, self.default_version)
         return str(version)
 
 
 class QueryParameterAPIVersionResolver(DefaultAPIVersionResolver):
     invalid_version_message = "Invalid version in query parameter."
 
-    def raise_exception(self) -> None:
-        raise NotFound(self.invalid_version_message)
-
     def resolve_version(self) -> str:
         version = (
             self.connection.query_params.get(self.version_parameter)
             or self.default_version
         )
         return str(version)
```

### Comparing `ellar-0.3.8/ellar/di/__init__.py` & `ellar-0.4.0/ellar/di/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/di/constants.py` & `ellar-0.4.0/ellar/di/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/di/injector/container.py` & `ellar-0.4.0/ellar/di/injector/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     DIScope,
     RequestScope,
     ScopeDecorator,
     SingletonScope,
     TransientScope,
 )
 from ..service_config import get_scope, is_decorated_with_injectable
-from ..types import T
 
 if t.TYPE_CHECKING:  # pragma: no cover
     from ellar.core.modules import ModuleBase
 
     from .ellar_injector import EllarInjector
 
 NOT_SET = object()
@@ -51,15 +50,15 @@
     ) -> Binding:
         provider = self.provider_for(interface, to)
         scope = scope or get_scope(to or interface) or TransientScope
         if isinstance(scope, ScopeDecorator):
             scope = scope.scope
         return Binding(interface, provider, scope)
 
-    def get_binding(self, interface: type) -> t.Tuple[Binding, InjectorBinder]:
+    def get_binding(self, interface: t.Type) -> t.Tuple[Binding, InjectorBinder]:
         is_scope = isinstance(interface, type) and issubclass(interface, InjectorScope)
         is_assisted_builder = _is_specialization(interface, AssistedBuilder)
         try:
             return self._get_binding(
                 interface, only_this_binder=is_scope or is_assisted_builder
             )
         except (KeyError, UnsatisfiedRequirement):
@@ -83,15 +82,15 @@
     def register_binding(self, interface: t.Type, binding: Binding) -> None:
         self._bindings[interface] = binding
 
     @t.no_type_check
     def register(
         self,
         base_type: t.Type,
-        concrete_type: t.Union[t.Type[T], t.Type, T] = None,
+        concrete_type: t.Union[t.Type, t.Any] = None,
         scope: t.Union[t.Type[DIScope], ScopeDecorator] = None,
     ) -> None:
         try:
             if concrete_type and isinstance(concrete_type, type):
                 assert issubclass(concrete_type, base_type), (
                     f"Cannot register {base_type.__name__} for abstract class "
                     f"{concrete_type.__name__}"
@@ -111,24 +110,24 @@
 
         if isinstance(_scope, ScopeDecorator):
             _scope = _scope.scope
 
         self.register_binding(base_type, Binding(base_type, provider, _scope))
 
     def register_instance(
-        self, instance: T, concrete_type: t.Union[t.Type[T], Provider] = None
+        self, instance: t.Any, concrete_type: t.Union[t.Type, Provider] = None
     ) -> None:
         assert not isinstance(instance, type)
         _concrete_type = instance.__class__ if not concrete_type else concrete_type
         self.register(_concrete_type, instance, scope=SingletonScope)
 
     def register_singleton(
         self,
-        base_type: t.Type[T],
-        concrete_type: t.Union[t.Type[T], T, Provider] = None,
+        base_type: t.Type,
+        concrete_type: t.Union[t.Type, t.Any, Provider] = None,
     ) -> None:
         """
 
         :param base_type:
         :param concrete_type:
         :return:
         """
```

### Comparing `ellar-0.3.8/ellar/di/injector/ellar_injector.py` & `ellar-0.4.0/ellar/di/injector/ellar_injector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/di/providers.py` & `ellar-0.4.0/ellar/di/providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/di/scopes.py` & `ellar-0.4.0/ellar/di/scopes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/di/service_config.py` & `ellar-0.4.0/ellar/di/service_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     def __call__(self, func_or_class: ConstructorOrClassT) -> ConstructorOrClassT:
         fail_silently(inject, constructor_or_class=func_or_class)
         setattr(func_or_class, INJECTABLE_ATTRIBUTE, self.scope)
         return func_or_class
 
 
 def injectable(
-    scope: t.Optional[t.Union[t.Type[DIScope], ScopeDecorator]] = SingletonScope
+    scope: t.Optional[t.Union[t.Type[DIScope], ScopeDecorator, t.Type]] = SingletonScope
 ) -> t.Union[ConstructorOrClassT, t.Callable]:
     """Decorates a callable or Type with inject and Defines Type or callable scope injection scope
 
     Example use:
 
     >>> @injectable # default is 'singleton_scope'
     ... class InjectableType2:
```

### Comparing `ellar-0.3.8/ellar/events.py` & `ellar-0.4.0/ellar/events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/__init__.py` & `ellar-0.4.0/ellar/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/builder.py` & `ellar-0.4.0/ellar/openapi/builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/docs_generators/base.py` & `ellar-0.4.0/ellar/openapi/docs_generators/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/docs_generators/redocs.py` & `ellar-0.4.0/ellar/openapi/docs_generators/redocs.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/docs_generators/swagger.py` & `ellar-0.4.0/ellar/openapi/docs_generators/swagger.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/module.py` & `ellar-0.4.0/ellar/openapi/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/openapi_v3.py` & `ellar-0.4.0/ellar/openapi/openapi_v3.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/route_doc_models.py` & `ellar-0.4.0/ellar/openapi/route_doc_models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/templates/redocs.html` & `ellar-0.4.0/ellar/openapi/templates/redocs.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/openapi/templates/swagger.html` & `ellar-0.4.0/ellar/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/reflect/_reflect.py` & `ellar-0.4.0/ellar/reflect/_reflect.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/samples/static/css/bootstrap.min.css` & `ellar-0.4.0/ellar/samples/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/samples/static/img/EllarLogoB.png` & `ellar-0.4.0/ellar/samples/static/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/samples/static/img/EllarLogoIconOnly.png` & `ellar-0.4.0/ellar/samples/static/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/samples/static/img/Icon.svg` & `ellar-0.4.0/ellar/samples/static/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/samples/templates/home/index.html` & `ellar-0.4.0/ellar/samples/templates/home/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/socket_io/__init__.py` & `ellar-0.4.0/ellar/socket_io/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/socket_io/constants.py` & `ellar-0.4.0/ellar/socket_io/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/socket_io/context.py` & `ellar-0.4.0/ellar/socket_io/context.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/socket_io/decorators/events.py` & `ellar-0.4.0/ellar/socket_io/decorators/events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/socket_io/decorators/gateway.py` & `ellar-0.4.0/ellar/socket_io/decorators/gateway.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/socket_io/decorators/subscribe_message.py` & `ellar-0.4.0/ellar/socket_io/decorators/subscribe_message.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/socket_io/factory.py` & `ellar-0.4.0/ellar/socket_io/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as t
 
 import socketio
 from starlette.routing import Mount
 
-from ellar.common.routing.builder import RouterBuilder
+from ellar.core.routing import RouterBuilder
 from ellar.reflect import reflect
 from ellar.socket_io.adapter import SocketIOASGIApp
 from ellar.socket_io.constants import (
     CONNECTION_EVENT,
     DISCONNECT_EVENT,
     GATEWAY_MESSAGE_HANDLER_KEY,
     GATEWAY_METADATA,
```

### Comparing `ellar-0.3.8/ellar/socket_io/gateway.py` & `ellar-0.4.0/ellar/socket_io/gateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,47 +3,50 @@
 
 from socketio import AsyncServer
 from starlette import status
 from starlette.concurrency import run_in_threadpool
 from starlette.exceptions import WebSocketException
 from starlette.routing import compile_path
 
-from ellar.common import IExecutionContext, IExecutionContextFactory, serialize_object
+from ellar.common import (
+    IExecutionContext,
+    IExecutionContextFactory,
+    IGuardsConsumer,
+    serialize_object,
+)
 from ellar.common.constants import (
     CONTROLLER_CLASS_KEY,
+    CONTROLLER_OPERATION_HANDLER_KEY,
     EXTRA_ROUTE_ARGS_KEY,
-    GUARDS_KEY,
     NOT_SET,
     SCOPE_SERVICE_PROVIDER,
 )
 from ellar.common.exceptions import WebSocketRequestValidationError
 from ellar.common.helper import get_name
 from ellar.common.params import WebsocketEndpointArgsModel
 from ellar.core import Config
-from ellar.core.services import Reflector
 from ellar.di import EllarInjector
 from ellar.reflect import reflect
 from ellar.socket_io.context import GatewayContext
 from ellar.socket_io.model import GatewayBase
 from ellar.socket_io.responses import WsResponse
 
 if t.TYPE_CHECKING:  # pragma: no cover
-    from ellar.common import GuardCanActivate
     from ellar.common.params import ExtraEndpointArg
 
 
 class SocketOperationConnection:
     __slots__ = (
         "_event",
         "_server",
         "endpoint",
         "_name",
         "_is_coroutine",
         "endpoint_parameter_model",
-        "_control_type",
+        "_controller_type",
     )
 
     ws_endpoint_args_model: t.Type[
         WebsocketEndpointArgsModel
     ] = WebsocketEndpointArgsModel
 
     def __init__(
@@ -51,16 +54,20 @@
     ) -> None:
         self._event = event
         self._server = server
         self.endpoint = message_handler
         self._name = get_name(self.endpoint)
         self._is_coroutine = inspect.iscoroutinefunction(message_handler)
         self.endpoint_parameter_model = NOT_SET
+        self._controller_type: t.Type[GatewayBase] = reflect.get_metadata(  # type: ignore[assignment]
+            CONTROLLER_CLASS_KEY, self.endpoint
+        )
         self._load_model()
         self._register_handler()
+        reflect.define_metadata(CONTROLLER_OPERATION_HANDLER_KEY, self, self.endpoint)
 
     def _load_model(self) -> None:
         path_regex, path_format, param_convertors = compile_path("/")
 
         extra_route_args: t.Union[t.List["ExtraEndpointArg"], "ExtraEndpointArg"] = (
             reflect.get_metadata(EXTRA_ROUTE_ARGS_KEY, self.endpoint) or []
         )
@@ -75,15 +82,15 @@
                 extra_endpoint_args=extra_route_args,
             )
             self.endpoint_parameter_model.build_model()
 
     async def _run_with_exception_handling(
         self, gateway_instance: GatewayBase, sid: str
     ) -> None:
-        config = gateway_instance.context.get_service_provider().get(Config)
+
         try:
             await self.run_route_guards(context=gateway_instance.context)
             await self._run_handler(
                 context=gateway_instance.context, gateway_instance=gateway_instance
             )
 
         except WebSocketException as aex:
@@ -95,14 +102,15 @@
         except WebSocketRequestValidationError as wex:
             await self._handle_error(
                 sid=sid,
                 code=status.WS_1007_INVALID_FRAME_PAYLOAD_DATA,
                 reason=serialize_object(wex.errors()),
             )
         except Exception as ex:
+            config = gateway_instance.context.get_service_provider().get(Config)
             await self._handle_error(
                 sid=sid,
                 code=status.WS_1011_INTERNAL_ERROR,
                 reason=str(ex) if config.DEBUG else "Something went wrong",
             )
 
     async def _handle_error(self, sid: str, code: int, reason: t.Any) -> None:
@@ -162,59 +170,44 @@
         if res and isinstance(res, WsResponse):
             await self._server.emit(**res.dict())
         elif res:
             await self._server.emit(self._event, res)
 
     @t.no_type_check
     async def run_route_guards(self, context: GatewayContext) -> None:
-        reflector = context.get_service_provider().get(Reflector)
-        app = context.get_app()
-
-        targets = [self.endpoint, self.get_control_type()]
-
-        _guards: t.Optional[
-            t.List[t.Union[t.Type["GuardCanActivate"], "GuardCanActivate"]]
-        ] = reflector.get_all_and_override(GUARDS_KEY, *targets)
-
-        if not _guards:
-            _guards = app.get_guards()
-
-        if _guards:
-            for guard in _guards:
-                if isinstance(guard, type):
-                    guard = context.get_service_provider().get(guard)
-
-                result = await guard.can_activate(context)
-                if not result:
-                    await self._server.emit(
-                        "error",
-                        {
-                            "code": status.WS_1011_INTERNAL_ERROR,
-                            "reason": "Authorization Failed",
-                        },
-                        room=context.sid,
-                    )
-                    await self._server.disconnect(sid=context.sid)
+        guard_consumer = context.get_service_provider().get(IGuardsConsumer)
+        try:
+            await guard_consumer.execute(context, self)
+        except Exception:
+            await self._server.emit(
+                "error",
+                {
+                    "code": status.WS_1011_INTERNAL_ERROR,
+                    "reason": "Authorization Failed",
+                },
+                room=context.sid,
+            )
+            await self._server.disconnect(sid=context.sid)
 
-    def get_control_type(self) -> t.Type[GatewayBase]:
+    def get_controller_type(self) -> t.Type[GatewayBase]:
         """
         For operation under a controller, `get_control_type` and `get_class` will return the same result
         For operation under ModuleRouter, this will return a unique type created for the router for tracking some properties
         :return: a type that wraps the operation
         """
-        if not hasattr(self, "_control_type"):
-            _control_type = reflect.get_metadata(CONTROLLER_CLASS_KEY, self.endpoint)
-            if _control_type is None:  # pragma: no cover
+        if not self._controller_type:
+            _controller_type = reflect.get_metadata(CONTROLLER_CLASS_KEY, self.endpoint)
+            if _controller_type is None or not isinstance(_controller_type, type):
                 raise Exception("Operation must have a single control type.")
-            self._control_type = t.cast(t.Type[GatewayBase], _control_type)
+            self._controller_type = t.cast(t.Type[GatewayBase], _controller_type)
 
-        return self._control_type
+        return self._controller_type
 
     def _get_gateway_instance(self, ctx: IExecutionContext) -> GatewayBase:
-        gateway_type = self.get_control_type()
+        gateway_type = self.get_controller_type()
         if not gateway_type or (
             gateway_type and not issubclass(gateway_type, GatewayBase)
         ):  # pragma: no cover
             raise RuntimeError("GatewayBase Type was not found")
 
         service_provider = ctx.get_service_provider()
```

### Comparing `ellar-0.3.8/ellar/socket_io/testing/module.py` & `ellar-0.4.0/ellar/socket_io/testing/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         sio = socketio.AsyncClient()
         return self.__class__(sio=sio, base_url=self.base_url)
 
 
 class SocketIOTestingModule(TestingModule):
     @asynccontextmanager
     async def run_with_server(
-        self, host: str = "127.0.0.1", port: int = 8000
+        self, host: str = "127.0.0.1", port: int = 4000
     ) -> t.AsyncIterator[RunWithServerContext]:
         base_url = f"http://{host}:{port}"
 
         server = EllarUvicornServer(app=self.create_application(), host=host, port=port)
 
         await server.start_up()
         sio = socketio.AsyncClient()
```

### Comparing `ellar-0.3.8/ellar/testing/module.py` & `ellar-0.4.0/ellar/testing/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/ellar/testing/uvicorn_server.py` & `ellar-0.4.0/ellar/testing/uvicorn_server.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/controllers.py` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/controllers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/module.py` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/routers.py` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/routers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/schemas.py` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/schemas.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/services.py` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/services.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/blog/blog.css` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/blog/blog.css`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/blog/blog.rtl.css`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo-white.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/statics/brand/bootstrap-logo.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_controllers.py` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/tests/test_routers.py` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/apps/car/views/index.html` & `ellar-0.4.0/examples/01-carapp/carapp/apps/car/views/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/root_module.py` & `ellar-0.4.0/examples/01-carapp/carapp/root_module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/01-carapp/carapp/server.py` & `ellar-0.4.0/examples/01-carapp/carapp/server.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/gateways.py` & `ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/gateways.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/module.py` & `ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/schemas.py` & `ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/schemas.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/02-socketio-app/socketio_app/apps/events/templates/events/index.html` & `ellar-0.4.0/examples/02-socketio-app/socketio_app/apps/events/templates/events/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/02-socketio-app/socketio_app/config.py` & `ellar-0.4.0/examples/02-socketio-app/socketio_app/config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/examples/02-socketio-app/socketio_app/server.py` & `ellar-0.4.0/examples/02-socketio-app/socketio_app/server.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/mkdocs.yml` & `ellar-0.4.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
       - Providers:  overview/providers.md
       - Modules:  overview/modules.md
       - Middlewares:  overview/middleware.md
       - Exception Handling:  overview/exception_handling.md
       - Guards:  overview/guards.md
       - Custom Decorators:  overview/custom_decorators.md
       - Module Router:  overview/module-router.md
+      - Interceptors:  overview/interceptors.md
   - Execution Context: basics/execution-context.md
   - Configuration: configurations.md
   - How-to Guides:
       - Input Parsing: parsing-inputs/index.md
       - Path: parsing-inputs/path-params.md
       - Query: parsing-inputs/query-params.md
       - Header: parsing-inputs/header-params.md
```

#### html2text {}

```diff
@@ -15,30 +15,30 @@
 - search: separator: '[\s\-,:!=\[\]()"`/]+|\.(?!\d)|&[lg]t;|(?!\b)(?=[A-Z][a-
 z])' - minify: minify_html: true - git-revision-date-localized:
 enable_creation_date: false nav: - Introduction: index.md - Overview: - Step
 One: overview/index.md - Controllers: overview/controllers.md - Providers:
 overview/providers.md - Modules: overview/modules.md - Middlewares: overview/
 middleware.md - Exception Handling: overview/exception_handling.md - Guards:
 overview/guards.md - Custom Decorators: overview/custom_decorators.md - Module
-Router: overview/module-router.md - Execution Context: basics/execution-
-context.md - Configuration: configurations.md - How-to Guides: - Input Parsing:
-parsing-inputs/index.md - Path: parsing-inputs/path-params.md - Query: parsing-
-inputs/query-params.md - Header: parsing-inputs/header-params.md - Cookie:
-parsing-inputs/cookie-params.md - Body: parsing-inputs/body.md - Form: parsing-
-inputs/form-params.md - File: parsing-inputs/file-params.md - Handling
-Response: - Response Schema: handling-response/response.md - Response Model:
-handling-response/response-model.md - Templating: - html: templating/
-templating.md - Static Files: templating/staticfiles.md - Caching: caching.md -
-Rate Limiting: throttling.md # - Injection Scopes: basics/injection-scope.md #
-- Events: basics/events.md - Commands: - Introduction: commands/index.md - CLI
-Commands: - new: commands/new-command.md - create project: commands/create-
-project-command.md - create module: commands/create-module-command.md -
-runserver: commands/runserver-command.md - Custom Commands: commands/custom-
-commands.md - Command Grouping: commands/command-grouping.md - Versioning:
-basics/versioning.md - Testing: basics/testing.md - WebSockets: - index:
-websockets/index.md - socketio: websockets/socketio.md - Mount: mount.md -
-Background Tasks: background-task.md - Release Notes: release-notes.md
-markdown_extensions: - attr_list - toc: permalink: true - admonition - def_list
-- tables - abbr - footnotes - md_in_html - codehilite - pymdownx.superfences:
-custom_fences: - name: mermaid class: mermaid - pymdownx.details -
-pymdownx.tabbed: alternate_style: true - pymdownx.saneheaders extra_css: -
-stylesheets/extra.css
+Router: overview/module-router.md - Interceptors: overview/interceptors.md -
+Execution Context: basics/execution-context.md - Configuration:
+configurations.md - How-to Guides: - Input Parsing: parsing-inputs/index.md -
+Path: parsing-inputs/path-params.md - Query: parsing-inputs/query-params.md -
+Header: parsing-inputs/header-params.md - Cookie: parsing-inputs/cookie-
+params.md - Body: parsing-inputs/body.md - Form: parsing-inputs/form-params.md
+- File: parsing-inputs/file-params.md - Handling Response: - Response Schema:
+handling-response/response.md - Response Model: handling-response/response-
+model.md - Templating: - html: templating/templating.md - Static Files:
+templating/staticfiles.md - Caching: caching.md - Rate Limiting: throttling.md
+# - Injection Scopes: basics/injection-scope.md # - Events: basics/events.md -
+Commands: - Introduction: commands/index.md - CLI Commands: - new: commands/
+new-command.md - create project: commands/create-project-command.md - create
+module: commands/create-module-command.md - runserver: commands/runserver-
+command.md - Custom Commands: commands/custom-commands.md - Command Grouping:
+commands/command-grouping.md - Versioning: basics/versioning.md - Testing:
+basics/testing.md - WebSockets: - index: websockets/index.md - socketio:
+websockets/socketio.md - Mount: mount.md - Background Tasks: background-task.md
+- Release Notes: release-notes.md markdown_extensions: - attr_list - toc:
+permalink: true - admonition - def_list - tables - abbr - footnotes -
+md_in_html - codehilite - pymdownx.superfences: custom_fences: - name: mermaid
+class: mermaid - pymdownx.details - pymdownx.tabbed: alternate_style: true -
+pymdownx.saneheaders extra_css: - stylesheets/extra.css
```

### Comparing `ellar-0.3.8/mypy.ini` & `ellar-0.4.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/pyproject.toml` & `ellar-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/conftest.py` & `ellar-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/injector_module.py` & `ellar-0.4.0/tests/injector_module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/main.py` & `ellar-0.4.0/tests/main.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/schema.py` & `ellar-0.4.0/tests/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_application/sample.py` & `ellar-0.4.0/tests/test_application/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_application/test_application_factory.py` & `ellar-0.4.0/tests/test_application/test_application_factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_application/test_application_functions.py` & `ellar-0.4.0/tests/test_application/test_application_functions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_application/test_cors.py` & `ellar-0.4.0/tests/test_application/test_cors.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_application/test_replacing_app_services.py` & `ellar-0.4.0/tests/test_application/test_replacing_app_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         self, operation, scope, receive=None, send=None
     ) -> IExecutionContext:
         i_execution_context = NewExecutionContext(
             scope=scope,
             receive=receive,
             send=send,
             operation_handler=operation.endpoint,
+            operation_handler_type=operation.get_controller_type(),
             reflector=self.reflector,
         )
 
         return i_execution_context
 
 
 @injectable()
```

### Comparing `ellar-0.3.8/tests/test_application/test_trusted_host.py` & `ellar-0.4.0/tests/test_application/test_trusted_host.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_attribute_dict.py` & `ellar-0.4.0/tests/test_attribute_dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/_test_aio_memcache.py.ellar` & `ellar-0.4.0/tests/test_cache/_test_aio_memcache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/pylib_mock.py` & `ellar-0.4.0/tests/test_cache/pylib_mock.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/redis_mock.py` & `ellar-0.4.0/tests/test_cache/redis_mock.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/test_cache_decorator.py` & `ellar-0.4.0/tests/test_cache/test_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/test_cache_many_config.py` & `ellar-0.4.0/tests/test_cache/test_cache_many_config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/test_cache_service.py` & `ellar-0.4.0/tests/test_cache/test_cache_service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/test_local_cache.py` & `ellar-0.4.0/tests/test_cache/test_local_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/test_module_setup.py` & `ellar-0.4.0/tests/test_cache/test_module_setup.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/test_pylibmc_cache.py` & `ellar-0.4.0/tests/test_cache/test_pylibmc_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/test_redis_cache.py` & `ellar-0.4.0/tests/test_cache/test_redis_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_cache/test_schema.py` & `ellar-0.4.0/tests/test_cache/test_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_conf/test_default_conf.py` & `ellar-0.4.0/tests/test_conf/test_default_conf.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_conf/test_mixins.py` & `ellar-0.4.0/tests/test_conf/test_mixins.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_controller/test_controller_decorator.py` & `ellar-0.4.0/tests/test_controller/test_controller_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from ellar.common import Controller, ControllerBase, get, http_route, ws_route
 from ellar.common.constants import (
     CONTROLLER_CLASS_KEY,
     CONTROLLER_OPERATION_HANDLER_KEY,
 )
-from ellar.common.routing import ControllerRouterFactory
+from ellar.core.routing import ControllerRouterFactory
 from ellar.di import has_binding, is_decorated_with_injectable
 from ellar.reflect import reflect
 
 from .sample import SampleController
 
 
 @Controller(prefix="/items/{orgID:int}", name="override_name", tag="new_tag")
```

### Comparing `ellar-0.3.8/tests/test_controller/test_controller_inheritance.py` & `ellar-0.4.0/tests/test_controller/test_controller_inheritance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import pytest
 
 from ellar.common import Controller, get, ws_route
-from ellar.common.constants import CONTROLLER_CLASS_KEY
-from ellar.common.routing import ControllerRouterFactory
+from ellar.common.constants import (
+    CONTROLLER_CLASS_KEY,
+    CONTROLLER_OPERATION_HANDLER_KEY,
+)
 from ellar.core import AppFactory
+from ellar.core.routing import ControllerRouterFactory
 from ellar.reflect import reflect
 
 
 class ControllerImplementationBase:
     @get("/sample")
     def some_example(self):
         pass
@@ -41,49 +44,59 @@
         @get()
         def endpoint_once(self):
             pass
 
     reflect.define_metadata(
         CONTROLLER_CLASS_KEY,
         None,
-        AnotherSampleController.endpoint_once,
+        AnotherSampleController().endpoint_once,
+    )
+    operation = reflect.get_metadata(
+        CONTROLLER_OPERATION_HANDLER_KEY, AnotherSampleController().endpoint_once
     )
 
     with pytest.raises(Exception, match=r"Operation must have a single control type."):
+        operation._controller_type = None
         ControllerRouterFactory.build(AnotherSampleController)
 
 
 def test_controller_raise_exception_for_controller_operation_without_controller_class(
     test_client_factory,
 ):
     @Controller("/abcd")
     class Another2SampleController:
         @get("/test")
         def endpoint_once(self):
             pass
 
     app = AppFactory.create_app(controllers=(Another2SampleController,))
     reflect.delete_metadata(
-        CONTROLLER_CLASS_KEY, Another2SampleController.endpoint_once
+        CONTROLLER_CLASS_KEY, Another2SampleController().endpoint_once
+    )
+    operation = reflect.get_metadata(
+        CONTROLLER_OPERATION_HANDLER_KEY, Another2SampleController().endpoint_once
     )
     client = test_client_factory(app)
-    with pytest.raises(RuntimeError, match=r"Controller Type was not found"):
-        client.get("/abcd/test")
-
 
-def test_controller_raise_exception_for_controller_operation_for_invalid_type(
-    test_client_factory,
-):
-    @Controller("/abcd")
-    class Another3SampleController:
-        @get("/test")
-        def endpoint_once(self):
-            pass
+    with pytest.raises(Exception, match=r"Operation must have a single control type"):
+        operation._controller_type = None
+        client.get("/abcd/test")
 
-    reflect.delete_metadata(
-        CONTROLLER_CLASS_KEY, Another3SampleController.endpoint_once
-    )
-    app = AppFactory.create_app(controllers=(Another3SampleController,))
 
-    client = test_client_factory(app)
-    with pytest.raises(RuntimeError, match=r"Controller Type was not found"):
-        client.get("/abcd/test")
+# def test_controller_raise_exception_for_controller_operation_for_invalid_type(
+#     test_client_factory,
+# ):
+#     @Controller("/abcd")
+#     class Another3SampleController:
+#         @get("/test")
+#         def endpoint_once(self):
+#             pass
+#
+#     reflect.delete_metadata(
+#         CONTROLLER_CLASS_KEY, Another3SampleController.endpoint_once
+#     )
+#
+#     app = AppFactory.create_app(controllers=(Another3SampleController,))
+#
+#     client = test_client_factory(app)
+#     with pytest.raises(RuntimeError, match=r"Controller Type was not found"):
+#         client.get("/abcd/test")
```

### Comparing `ellar-0.3.8/tests/test_controller/test_module_router.py` & `ellar-0.4.0/tests/test_controller/test_module_router.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 from ellar.common.routing import ModuleRouter
+from ellar.core.routing import ModuleRouterFactory
 
 from .sample import router
 
 another_router = ModuleRouter("/prefix/another", tag="another_router", name="arouter")
 
 
 @another_router.get("/sample")
@@ -78,12 +79,14 @@
 def test_module_router_url_reverse():
     new_router = ModuleRouter("/items/{orgID:int}", name="has_name")
 
     @new_router.get
     def some_route():
         pass
 
+    ModuleRouterFactory.build(new_router)
+
     reversed_path = new_router.url_path_for(
         f"{new_router.name}:{new_router.routes[0].name}"
     )
     path = new_router.path_format.replace("/{path}", new_router.routes[0].path)
     assert reversed_path == path
```

### Comparing `ellar-0.3.8/tests/test_controller/test_route_collection.py` & `ellar-0.4.0/tests/test_controller/test_route_collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 )
 from ellar.common.helper import generate_controller_operation_unique_id
 from ellar.common.routing import (
     RouteCollection,
     RouteOperation,
     WebsocketRouteOperation,
 )
+from ellar.core.routing.helper import build_route_handler
 from ellar.core.versioning import UrlPathAPIVersioning
 from ellar.reflect import reflect
 from ellar.testing import Test
 
 
 class Configuration:
     VERSIONING_SCHEME = UrlPathAPIVersioning()
@@ -34,27 +35,27 @@
     @version_decorator(*versions)
     def endpoint_sample():
         response = JSONResponse(
             content=dict(path=path, methods=methods, versioning=versions)
         )
         return response
 
-    return reflect.get_metadata(CONTROLLER_OPERATION_HANDLER_KEY, endpoint_sample)
+    return build_route_handler(endpoint_sample)
 
 
 def create_ws_route_operation(
     path: str, versions: List[str] = []
 ) -> WebsocketRouteOperation:
     @ws_route(path)
     @version_decorator(*versions)
     def endpoint_sample():
         response = JSONResponse(content=dict(path=path, versioning=versions))
         return response
 
-    return reflect.get_metadata(CONTROLLER_OPERATION_HANDLER_KEY, endpoint_sample)
+    return build_route_handler(endpoint_sample)
 
 
 class MockHostRouteOperation(Host):
     def asgi_app(self, scope, receive, send):
         pass
 
     def __init__(self, host: str, name: str = None):
@@ -68,16 +69,20 @@
     def __init__(self, path: str, name: str = None):
         super().__init__(path=path, name=name, app=self.asgi_app)
 
 
 @pytest.mark.parametrize("collection_model", [RouteCollection])
 def test_module_route_collection_for_same_path_but_different_version(collection_model):
     routes = collection_model()
-    routes.append(create_route_operation("/sample", methods=["post"], versions=[]))
-    routes.append(create_route_operation("/sample", methods=["post"], versions=["1"]))
+    routes.extend(
+        [
+            create_route_operation("/sample", methods=["post"], versions=[]),
+            create_route_operation("/sample", methods=["post"], versions=["1"]),
+        ]
+    )
     assert len(routes) == 2
     for route in routes:
         assert route.path == "/sample"
 
     tm = Test.create_test_module(config_module=config_path)
     tm.create_application().router.extend(routes)
     client = tm.get_test_client()
```

### Comparing `ellar-0.3.8/tests/test_decorators/test_controller.py` & `ellar-0.4.0/tests/test_decorators/test_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.common import Controller, ControllerBase, Guards, Version, set_metadata
+from ellar.common import Controller, ControllerBase, UseGuards, Version, set_metadata
 from ellar.common.constants import (
     CONTROLLER_METADATA,
     GUARDS_KEY,
     NOT_SET,
     VERSIONING_KEY,
 )
 from ellar.common.exceptions import ImproperConfiguration
@@ -17,15 +17,15 @@
     description="Some description",
     external_doc_description="external",
     tag="dec",
     external_doc_url="https://example.com",
     name="test",
 )
 @Version("v1")
-@Guards()
+@UseGuards()
 class ControllerDecorationTest:
     pass
 
 
 @Controller
 class ControllerDefaultTest:
     pass
```

### Comparing `ellar-0.3.8/tests/test_decorators/test_exception.py` & `ellar-0.4.0/tests/test_decorators/test_exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_decorators/test_file.py` & `ellar-0.4.0/tests/test_decorators/test_file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_decorators/test_guards.py` & `ellar-0.4.0/tests/test_decorators/test_guards.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ellar.common import GuardCanActivate, Guards
+from ellar.common import GuardCanActivate, UseGuards
 from ellar.common.constants import GUARDS_KEY
 from ellar.core import ExecutionContext, Request
 from ellar.reflect import reflect
 
 
 class SomeGuard(GuardCanActivate):
     async def can_activate(self, context: ExecutionContext) -> bool:
@@ -10,20 +10,20 @@
 
 
 class SomeGuard2(SomeGuard):
     async def can_activate(self, context: ExecutionContext) -> bool:
         return False  # pragma: no cover
 
 
-@Guards(SomeGuard)
+@UseGuards(SomeGuard)
 def endpoint(request: Request):
     return "foo"  # pragma: no cover
 
 
-@Guards(SomeGuard, SomeGuard2)
+@UseGuards(SomeGuard, SomeGuard2)
 def endpoint2(request: Request):
     return "foo"  # pragma: no cover
 
 
 def test_guard_decorator_applies_guards_key_to_reflect():
     guard_info = reflect.get_metadata(GUARDS_KEY, endpoint)
     assert guard_info
```

### Comparing `ellar-0.3.8/tests/test_decorators/test_html.py` & `ellar-0.4.0/tests/test_decorators/test_html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_decorators/test_middleware.py` & `ellar-0.4.0/tests/test_decorators/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_decorators/test_modules.py` & `ellar-0.4.0/tests/test_decorators/test_modules.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_decorators/test_openapi.py` & `ellar-0.4.0/tests/test_decorators/test_openapi.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_decorators/test_serializer.py` & `ellar-0.4.0/tests/test_decorators/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_di/examples.py` & `ellar-0.4.0/tests/test_di/examples.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_di/test_injectable_resolving.py` & `ellar-0.4.0/tests/test_di/test_injectable_resolving.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_di/test_injector.py` & `ellar-0.4.0/tests/test_di/test_injector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_di/test_provider_scopes.py` & `ellar-0.4.0/tests/test_di/test_provider_scopes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_di/test_providers.py` & `ellar-0.4.0/tests/test_di/test_providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_events.py` & `ellar-0.4.0/tests/test_events.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,7 +63,20 @@
     def valid_function_1():
         nonlocal called
         called += 1
 
     config = Config(ON_REQUEST_STARTUP=[EventHandler(valid_function_1)])
     await config.ON_REQUEST_STARTUP[0].run()
     assert called == 1
+
+
+async def test_events_reload(anyio_backend):
+    called = 0
+
+    def valid_function_1():
+        nonlocal called
+        called += 1
+
+    manager = RouterEventManager()
+    manager.reload([EventHandler(valid_function_1)])
+    await manager.async_run()
+    assert called == 1
```

### Comparing `ellar-0.3.8/tests/test_exceptions/test_api_exception.py` & `ellar-0.4.0/tests/test_exceptions/test_api_exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_exceptions/test_custom_exceptions.py` & `ellar-0.4.0/tests/test_exceptions/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_exceptions/test_error_details.py` & `ellar-0.4.0/tests/test_exceptions/test_error_details.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_exceptions/test_validation_exception.py` & `ellar-0.4.0/tests/test_exceptions/test_validation_exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_guard.py` & `ellar-0.4.0/tests/test_guard.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from starlette.status import HTTP_401_UNAUTHORIZED
 
-from ellar.common import APIException, Guards, Req, get, serialize_object
+from ellar.common import APIException, Req, UseGuards, get, serialize_object
 from ellar.core import AppFactory, Reflector
 from ellar.core.guard import (
     APIKeyCookie,
     APIKeyHeader,
     APIKeyQuery,
     HttpBasicAuth,
     HttpBearerAuth,
@@ -91,15 +91,15 @@
     ("basic", BasicAuth()),
     ("bearer", BearerAuth),
     ("digest", DigestAuth),
     ("customexception", HeaderSecretKeyCustomException),
 ]:
 
     @get(f"/{_path}")
-    @Guards(auth)
+    @UseGuards(auth)
     def auth_demo_endpoint(request=Req()):
         return {"authentication": request.user}
 
     app.router.append(auth_demo_endpoint)
 
 client = TestClient(app)
 
@@ -236,7 +236,24 @@
         "HeaderSecretKeyCustomException": {
             "type": "apiKey",
             "in": "header",
             "name": "HeaderSecretKeyCustomException",
         },
         "DigestAuth": {"type": "http", "scheme": "digest", "name": "DigestAuth"},
     }
+
+
+def test_global_guard_works():
+    _app = AppFactory.create_app(global_guards=[DigestAuth])
+
+    @get("/global")
+    def _auth_demo_endpoint(request=Req()):
+        return {"authentication": request.user}
+
+    _app.router.append(_auth_demo_endpoint)
+    _client = TestClient(_app)
+    res = _client.get("/global")
+
+    assert res.status_code == 401
+    data = res.json()
+
+    assert data == {"detail": "Forbidden"}
```

### Comparing `ellar-0.3.8/tests/test_helper/test_enum.py` & `ellar-0.4.0/tests/test_helper/test_enum.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_helper/test_model_field.py` & `ellar-0.4.0/tests/test_helper/test_model_field.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_middleware/test_functional_middleware.py` & `ellar-0.4.0/tests/test_middleware/test_functional_middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from starlette.requests import Request
 from starlette.responses import PlainTextResponse
 
 from ellar.common import IHostContext, Module, ModuleRouter, middleware
-from ellar.core import ModuleBase
+from ellar.core import App, Config, ModuleBase
+from ellar.core.middleware import FunctionBasedMiddleware
+from ellar.di import EllarInjector
+from ellar.reflect import asynccontextmanager
 from ellar.testing import Test
 
 mr = ModuleRouter()
 
 
 @mr.get()
 def homepage(request: Request):
@@ -63,7 +66,31 @@
 def test_middleware_returns_response():
     tm = Test.create_test_module(modules=[ModuleMiddleware])
     client = tm.get_test_client()
 
     response = client.get("/", headers={"ellar": "set"})
     assert response.status_code == 200
     assert response.text == "middleware_return_response returned a response"
+
+
+def test_functional_middleware_skips_lifespan(test_client_factory):
+    async def middleware_function(context: IHostContext, call_next):
+        pass
+
+    startup_complete = False
+    cleanup_complete = False
+
+    @asynccontextmanager
+    async def lifespan(app):
+        nonlocal startup_complete, cleanup_complete
+        startup_complete = True
+        yield
+        cleanup_complete = True
+
+    app = FunctionBasedMiddleware(
+        App(config=Config(), injector=EllarInjector(), lifespan=lifespan),
+        middleware_function,
+    )
+
+    with test_client_factory(app):
+        assert startup_complete
+        assert not cleanup_complete
```

### Comparing `ellar-0.3.8/tests/test_middleware/test_service_provider_middleware.py` & `ellar-0.4.0/tests/test_middleware/test_service_provider_middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_middleware/test_versioning_middleware.py` & `ellar-0.4.0/tests/test_middleware/test_versioning_middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_modules/sample.py` & `ellar-0.4.0/tests/test_modules/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_modules/test_module_config.py` & `ellar-0.4.0/tests/test_modules/test_module_config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_modules/test_module_ref.py` & `ellar-0.4.0/tests/test_modules/test_module_ref.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 import pytest
 from starlette.routing import Route
 
 from ellar.common import (
     Module,
     exception_handler,
     middleware,
@@ -192,30 +194,32 @@
         )
         module_ref = create_module_ref_factor(
             ModuleBaseExample, config=config, container=container
         )
     assert len(module_ref.routers) == 5
 
 
-def test_module_template_ref_get_all_routers_fails_for_invalid_controller():
+def test_module_template_ref_get_all_routers_fails_for_invalid_controller(caplog):
     some_invalid_controller = type("SomeInvalidController", (), {})
     with reflect.context():
         reflect.define_metadata(
             MODULE_METADATA.CONTROLLERS, [some_invalid_controller], ModuleBaseExample
         )
         config = Config()
         container = EllarInjector(auto_bind=False).container
 
-        with pytest.raises(Exception) as ex:
+        with caplog.at_level(logging.WARNING):
             create_module_ref_factor(
                 ModuleBaseExample, config=config, container=container
             )
+
         assert (
-            str(ex.value)
-            == "Router Factory Builder was not found.\nUse `ControllerRouterBuilderFactory` as an example create a FactoryBuilder for this type: <class 'type'>"
+            "Router Factory Builder was not found.\nUse `ControllerRouterBuilderFactory` "
+            "as an example create a FactoryBuilder for this type: <class 'type'>"
+            in str(caplog.text)
         )
 
 
 def test_invalid_module_template_ref():
     config = Config()
     container = EllarInjector(auto_bind=False).container
 
@@ -247,16 +251,19 @@
             MODULE_METADATA.ROUTERS,
             [some_invalid_router(), Route("/", endpoint=lambda request: "Test")],
             ModuleBaseExample,
         )
         module_ref = create_module_ref_factor(
             ModuleBaseExample, config=config, container=container
         )
+
+        app = AppFactory.create_from_app_module(module=ModuleBaseExample)
     assert len(module_ref.routers) == 4
-    assert len(module_ref.routes) == 3
+    assert len(module_ref.routes) == 4
+    assert len(app.routes) == 3
 
 
 def test_module_template_ref_routes():
     config = Config()
     container = EllarInjector(auto_bind=False).container
 
     module_ref = create_module_ref_factor(
```

### Comparing `ellar-0.3.8/tests/test_openapi/test_builder.py` & `ellar-0.4.0/tests/test_openapi/test_builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_openapi/test_module.py` & `ellar-0.4.0/tests/test_openapi/test_module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_openapi/test_open_api_route_documentation.py` & `ellar-0.4.0/tests/test_openapi/test_open_api_route_documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pydantic.schema import get_flat_models_from_fields, get_model_name_map
 
 from ellar.common import Body, ModuleRouter, Query, openapi_info
 from ellar.common.constants import CONTROLLER_OPERATION_HANDLER_KEY, OPENAPI_KEY
 from ellar.common.responses.models import ResponseModel, ResponseModelField
 from ellar.core.connection import HTTPConnection
 from ellar.core.guard import APIKeyCookie
+from ellar.core.routing import ModuleRouterFactory
 from ellar.openapi import OpenAPIRouteDocumentation
 from ellar.reflect import reflect
 
 from ..schema import BlogObjectDTO, CreateCarSchema, Filter, NoteSchemaDC
 
 
 class CustomCookieAPIKey(APIKeyCookie):
@@ -55,14 +56,17 @@
 
 
 @router.http_route("/list", response={200: CreateCarSchema}, methods=["get", "post"])
 def list_and_create_car(car: CreateCarSchema = Body(default=None)):
     return car
 
 
+ModuleRouterFactory.build(router)
+
+
 def test_open_api_route_model_input_fields():
     route_operation = reflect.get_metadata(
         CONTROLLER_OPERATION_HANDLER_KEY, get_car_by_id
     )
     openapi_route_doc = OpenAPIRouteDocumentation(route=route_operation)
     assert len(openapi_route_doc.input_fields) == 3
```

### Comparing `ellar-0.3.8/tests/test_reflect.py` & `ellar-0.4.0/tests/test_reflect.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_reflector.py` & `ellar-0.4.0/tests/test_reflector.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,17 @@
     value = "value"
     reflect.define_metadata(key, [value], SampleTarget)
     assert reflector.get_all_and_merge(key, *[SampleTarget, SampleTarget]) == [
         value,
         value,
     ]
 
+    reflect.define_metadata("key1", value, SampleTarget)
+    assert reflector.get_all_and_merge("key1", *[SampleTarget]) == [value]
+
 
 def test_should_reflect_metadata_of_all_targets_in_an_arrays():
     key = "key"
     value = "value"
     reflect.define_metadata(key, value, SampleTarget)
     assert reflector.get_all_and_merge(
         key, *[SampleTarget, SampleTarget, SampleTarget]
```

### Comparing `ellar-0.3.8/tests/test_response/test_defined_response_model.py` & `ellar-0.4.0/tests/test_response/test_defined_response_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import List, Optional
 
-import pytest
 from pydantic import BaseModel
 
 from ellar.common import ModuleRouter
-from ellar.common.responses.models import RouteResponseExecution
 from ellar.core import AppFactory
 
 mr = ModuleRouter("")
 
 
 class Item(BaseModel):
     name: str
@@ -51,18 +49,19 @@
 def test_valid_tuple_return(test_client_factory):
     client = test_client_factory(app)
     response = client.get("/items/valid_tuple_return")
     response.raise_for_status()
     assert response.json() == {"name": "baz", "price": 2.0, "owner_ids": [1, 2, 3]}
 
 
-def test_get_not_found_res_model(test_client_factory):
+def test_get_not_found_res_model_uses_empty_model(test_client_factory):
     client = test_client_factory(app)
-    with pytest.raises(RouteResponseExecution):
-        client.get("/items/not_found_res_model")
+    res = client.get("/items/not_found_res_model")
+    assert res.status_code == 301
+    assert res.json() == {"name": "baz", "price": 2.0, "owner_ids": [1, 2, 3]}
 
 
 def test_valid(test_client_factory):
     client = test_client_factory(app)
     response = client.get("/items/valid")
     response.raise_for_status()
     assert response.json() == {"name": "valid", "price": 1.0, "owner_ids": None}
```

### Comparing `ellar-0.3.8/tests/test_response/test_pydantic_response_model.py` & `ellar-0.4.0/tests/test_response/test_pydantic_response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_response/test_response_file.py` & `ellar-0.4.0/tests/test_response/test_response_file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_response/test_response_html.py` & `ellar-0.4.0/tests/test_response/test_response_html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_response/test_response_streaming.py` & `ellar-0.4.0/tests/test_response/test_response_streaming.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_response/test_response_type_definition_converter.py` & `ellar-0.4.0/tests/test_response/test_response_type_definition_converter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_response/test_route_response_model.py` & `ellar-0.4.0/tests/test_response/test_route_response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/sample.py` & `ellar-0.4.0/tests/test_routing/sample.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_body_schema.py` & `ellar-0.4.0/tests/test_routing/test_body_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_body_schema_extra_properties.py` & `ellar-0.4.0/tests/test_routing/test_body_schema_extra_properties.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_body_union_schema.py` & `ellar-0.4.0/tests/test_routing/test_body_union_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_cookie_schema.py` & `ellar-0.4.0/tests/test_routing/test_cookie_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from ellar.common import Cookie, ModuleRouter, get, serialize_object
 from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
+from ellar.core.routing.helper import build_route_handler
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.testing import Test
 
 from .sample import Data, Filter, ListOfPrimitiveSchema, NonPrimitiveSchema
 
 router = ModuleRouter("")
 
@@ -112,25 +113,29 @@
 def test_invalid_schema_cookie():
     with pytest.raises(ImproperConfiguration) as ex:
 
         @get("/test")
         def invalid_path_parameter(cookie: NonPrimitiveSchema = Cookie()):
             pass
 
+        build_route_handler(invalid_path_parameter)
+
     assert (
         str(ex.value)
         == "field: 'filter' with annotation:'<class 'tests.test_routing.sample.Filter'>' in "
         "'<class 'tests.test_routing.sample.NonPrimitiveSchema'>'can't be processed. "
         "Field type is not a primitive type"
     )
 
     with pytest.raises(ImproperConfiguration) as ex:
 
         @get("/test")
         def invalid_path_parameter(cookie: ListOfPrimitiveSchema = Cookie()):
             pass
 
+        build_route_handler(invalid_path_parameter)
+
     assert (
         str(ex.value) == "field: 'an_int' with annotation:'typing.List[int]' in "
         "'<class 'tests.test_routing.sample.ListOfPrimitiveSchema'>'can't be processed. "
         "Field type is not a primitive type"
     )
```

### Comparing `ellar-0.3.8/tests/test_routing/test_extra_args.py` & `ellar-0.4.0/tests/test_routing/test_extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_form_schema.py` & `ellar-0.4.0/tests/test_routing/test_form_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from ellar.common import Form, ModuleRouter, post, serialize_object
 from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
+from ellar.core.routing.helper import build_route_handler
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.testing import Test
 
 from .sample import Filter, NonPrimitiveSchema
 
 mr = ModuleRouter("")
 
@@ -65,14 +66,16 @@
 def test_for_invalid_schema():
     with pytest.raises(ImproperConfiguration) as ex:
 
         @post("/test")
         def invalid_path_parameter(path: NonPrimitiveSchema = Form()):
             pass
 
+        build_route_handler(invalid_path_parameter)
+
     assert (
         str(ex.value)
         == "field: 'filter' with annotation:'<class 'tests.test_routing.sample.Filter'>' in "
         "'<class 'tests.test_routing.sample.NonPrimitiveSchema'>'can't be processed. "
         "Field type should belong to (<class 'list'>, <class 'set'>, <class 'tuple'>) "
         "or any primitive type"
     )
```

### Comparing `ellar-0.3.8/tests/test_routing/test_formparsers.py` & `ellar-0.4.0/tests/test_routing/test_formparsers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_forms.py` & `ellar-0.4.0/tests/test_routing/test_forms.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_forms_from_non_typing_sequences.py` & `ellar-0.4.0/tests/test_routing/test_forms_from_non_typing_sequences.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_header_schema.py` & `ellar-0.4.0/tests/test_routing/test_header_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from ellar.common import Header, ModuleRouter, get, serialize_object
 from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
+from ellar.core.routing.helper import build_route_handler
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.testing import Test
 
 from .sample import Data, Filter, NonPrimitiveSchema
 
 mr = ModuleRouter("")
 
@@ -112,14 +113,16 @@
 def test_invalid_schema_header():
     with pytest.raises(ImproperConfiguration) as ex:
 
         @get("/test")
         def invalid_path_parameter(cookie: NonPrimitiveSchema = Header()):
             pass
 
+        build_route_handler(invalid_path_parameter)
+
     assert (
         str(ex.value)
         == "field: 'filter' with annotation:'<class 'tests.test_routing.sample.Filter'>' in "
         "'<class 'tests.test_routing.sample.NonPrimitiveSchema'>'can't be processed. "
         "Field type should belong to (<class 'list'>, <class 'set'>, <class 'tuple'>) "
         "or any primitive type"
     )
```

### Comparing `ellar-0.3.8/tests/test_routing/test_invalid_path_param.py` & `ellar-0.4.0/tests/test_routing/test_invalid_path_param.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,88 @@
 from typing import Dict, List, Tuple
 
 import pytest
 from pydantic import BaseModel
 
 from ellar.common import ModuleRouter
+from ellar.core.routing import ModuleRouterFactory
 
 mr = ModuleRouter("")
 
 
 def test_invalid_sequence():
     with pytest.raises(AssertionError):
 
         class Item(BaseModel):
             title: str
 
         @mr.get("/items/{id}")
         def read_items(id: List[Item]):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 def test_invalid_tuple():
     with pytest.raises(AssertionError):
 
         class Item(BaseModel):
             title: str
 
         @mr.get("/items/{id}")
         def read_items(id: Tuple[Item, Item]):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 def test_invalid_dict():
     with pytest.raises(AssertionError):
 
         class Item(BaseModel):
             title: str
 
         @mr.get("/items/{id}")
         def read_items(id: Dict[str, Item]):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 def test_invalid_simple_list():
     with pytest.raises(AssertionError):
 
         @mr.get("/items/{id}")
         def read_items(id: list):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 def test_invalid_simple_tuple():
     with pytest.raises(AssertionError):
 
         @mr.get("/items/{id}")
         def read_items(id: tuple):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 def test_invalid_simple_set():
     with pytest.raises(AssertionError):
 
         @mr.get("/items/{id}")
         def read_items(id: set):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 def test_invalid_simple_dict():
     with pytest.raises(AssertionError):
 
         @mr.get("/items/{id}")
         def read_items(id: dict):
             pass  # pragma: no cover
+
+        ModuleRouterFactory.build(mr)
```

### Comparing `ellar-0.3.8/tests/test_routing/test_invalid_sequence_param.py` & `ellar-0.4.0/tests/test_routing/test_invalid_sequence_param.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict, List, Optional, Tuple
 
 import pytest
 from pydantic import BaseModel
 
 from ellar.common import Header, ModuleRouter, Query
 from ellar.common.exceptions import ImproperConfiguration
+from ellar.core.routing import ModuleRouterFactory
 
 mr = ModuleRouter("")
 
 
 class Item(BaseModel):
     title: str
 
@@ -21,42 +22,52 @@
 def test_invalid_sequence(field_parameter):
     with pytest.raises(ImproperConfiguration):
 
         @mr.get("/items/")
         def read_items(q: List[Item] = field_parameter):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 @pytest.mark.parametrize("field_parameter", [Query(None), Header(None)])
 def test_invalid_tuple(field_parameter):
     with pytest.raises(ImproperConfiguration):
 
         @mr.get("/items/")
         def read_items(q: Tuple[Item, Item] = field_parameter):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 @pytest.mark.parametrize("field_parameter", [Query(None), Header(None)])
 def test_invalid_dict(field_parameter):
     with pytest.raises(ImproperConfiguration):
 
         @mr.get("/items/")
         def read_items(q: Dict[str, Item] = field_parameter):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 @pytest.mark.parametrize("field_parameter", [Query(None), Header(None)])
 def test_invalid_simple_dict(field_parameter):
     with pytest.raises(ImproperConfiguration):
 
         @mr.get("/items/")
         def read_items(q: Optional[dict] = field_parameter):
             pass  # pragma: no cover
 
+        ModuleRouterFactory.build(mr)
+
 
 @pytest.mark.parametrize("field_parameter", [Query(None), Header(None)])
 def test_invalid_group_type(field_parameter):
     with pytest.raises(ImproperConfiguration):
 
         @mr.get("/items/")
         def read_items(q: Item2 = field_parameter):
             pass  # pragma: no cover
+
+        ModuleRouterFactory.build(mr)
```

### Comparing `ellar-0.3.8/tests/test_routing/test_multi_body_errors.py` & `ellar-0.4.0/tests/test_routing/test_multi_body_errors.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_multi_query_errors.py` & `ellar-0.4.0/tests/test_routing/test_multi_query_errors.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_path.py` & `ellar-0.4.0/tests/test_routing/test_path.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_path_with_schema.py` & `ellar-0.4.0/tests/test_routing/test_path_with_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from ellar.common import ModuleRouter, Path, get, serialize_object
 from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
+from ellar.core.routing.helper import build_route_handler
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.testing import Test
 
 from .sample import Filter, ListOfPrimitiveSchema, NonPrimitiveSchema
 
 mr = ModuleRouter("")
 
@@ -76,22 +77,26 @@
 def test_for_invalid_schema():
     with pytest.raises(ImproperConfiguration) as ex:
 
         @get("/{filter}")
         def invalid_path_parameter(path: NonPrimitiveSchema = Path()):
             pass
 
+        build_route_handler(invalid_path_parameter)
+
     assert (
         str(ex.value)
         == "Path params must be of one of the supported types. Only primitive types"
     )
 
     with pytest.raises(ImproperConfiguration) as ex:
 
         @get("/{int}/{float}")
         def invalid_path_parameter(path: ListOfPrimitiveSchema = Path()):
             pass
 
+        build_route_handler(invalid_path_parameter)
+
     assert (
         str(ex.value)
         == "Path params must be of one of the supported types. Only primitive types"
     )
```

### Comparing `ellar-0.3.8/tests/test_routing/test_put_with_no_body_schema.py` & `ellar-0.4.0/tests/test_routing/test_put_with_no_body_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_query.py` & `ellar-0.4.0/tests/test_routing/test_query.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_query_schema.py` & `ellar-0.4.0/tests/test_routing/test_query_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from ellar.common import ModuleRouter, Query, get, serialize_object
 from ellar.common.exceptions import ImproperConfiguration
 from ellar.core.connection import Request
+from ellar.core.routing.helper import build_route_handler
 from ellar.openapi import OpenAPIDocumentBuilder
 from ellar.testing import Test
 
 from .sample import Data, Filter, NonPrimitiveSchema
 
 mr = ModuleRouter("")
 
@@ -112,14 +113,16 @@
 def test_invalid_schema_query():
     with pytest.raises(ImproperConfiguration) as ex:
 
         @get("/test")
         def invalid_path_parameter(cookie: NonPrimitiveSchema = Query()):
             pass
 
+        build_route_handler(invalid_path_parameter)
+
     assert (
         str(ex.value)
         == "field: 'filter' with annotation:'<class 'tests.test_routing.sample.Filter'>' in "
         "'<class 'tests.test_routing.sample.NonPrimitiveSchema'>'can't be processed. "
         "Field type should belong to (<class 'list'>, <class 'set'>, <class 'tuple'>) "
         "or any primitive type"
     )
```

### Comparing `ellar-0.3.8/tests/test_routing/test_request.py` & `ellar-0.4.0/tests/test_routing/test_request.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_routing/test_route_endpoint_params.py` & `ellar-0.4.0/tests/test_routing/test_route_endpoint_params.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_schema.py` & `ellar-0.4.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_serializer.py` & `ellar-0.4.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_shortcuts.py` & `ellar-0.4.0/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_socket_io/sample.py` & `ellar-0.4.0/tests/test_socket_io/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 from functools import wraps
 
 from starlette import status
 from starlette.exceptions import WebSocketException
 
-from ellar.common import Guards, Header, Query, Serializer, WsBody, extra_args
+from ellar.common import Header, Query, Serializer, UseGuards, WsBody, extra_args
 from ellar.common.params import ExtraEndpointArg
 from ellar.core.connection import HTTPConnection
 from ellar.core.guard import APIKeyHeader
 from ellar.di import injectable
 from ellar.socket_io import (
     WebSocketGateway,
     WsResponse,
@@ -82,15 +82,15 @@
         )
 
     @on_disconnected()
     async def disconnect(self):
         print("Client disconnected")
 
 
-@Guards(HeaderGuard)
+@UseGuards(HeaderGuard)
 @WebSocketGateway(path="/ws-guard")
 class GatewayWithGuards(GatewayBase):
     @subscribe_message("my_event")
     async def my_event(self, message: MessageData = WsBody()):
         return WsResponse(
             "my_response",
             {
```

### Comparing `ellar-0.3.8/tests/test_socket_io/test_decorators/test_events.py` & `ellar-0.4.0/tests/test_socket_io/test_decorators/test_events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_socket_io/test_decorators/test_gateway.py` & `ellar-0.4.0/tests/test_socket_io/test_decorators/test_gateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from ellar.common import Guards
+from ellar.common import UseGuards
 from ellar.common.constants import CONTROLLER_CLASS_KEY, GUARDS_KEY
 from ellar.common.helper import get_name
 from ellar.core.guard import HttpBearerAuth
 from ellar.reflect import reflect
 from ellar.socket_io import WebSocketGateway, subscribe_message
 from ellar.socket_io.constants import (
     GATEWAY_MESSAGE_HANDLER_KEY,
@@ -13,15 +13,15 @@
     GATEWAY_WATERMARK,
     MESSAGE_METADATA,
 )
 from ellar.socket_io.model import GatewayBase, GatewayType
 
 
 @WebSocketGateway(path="/ws", namespace="/some-namespace")
-@Guards(HttpBearerAuth)
+@UseGuards(HttpBearerAuth)
 class SampleWithoutGateway:
     pass
 
 
 @WebSocketGateway(path="/ws", namespace="/some-namespace")
 class SampleWithGateway(GatewayBase):
     pass
```

### Comparing `ellar-0.3.8/tests/test_socket_io/test_decorators/test_subcribe_message.py` & `ellar-0.4.0/tests/test_socket_io/test_decorators/test_subcribe_message.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_socket_io/test_operation.py` & `ellar-0.4.0/tests/test_socket_io/test_operation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_staticfiles.py` & `ellar-0.4.0/tests/test_staticfiles.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_templating/test_module_templating.py` & `ellar-0.4.0/tests/test_templating/test_module_templating.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_templating/test_renderer.py` & `ellar-0.4.0/tests/test_templating/test_renderer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_testing.py` & `ellar-0.4.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_versioning/operations.py` & `ellar-0.4.0/tests/test_versioning/operations.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_versioning/test_default_versioning.py` & `ellar-0.4.0/tests/test_versioning/test_default_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_versioning/test_default_versioning_for_controllers.py` & `ellar-0.4.0/tests/test_versioning/test_default_versioning_for_controllers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_versioning/test_header_versioning.py` & `ellar-0.4.0/tests/test_versioning/test_header_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_versioning/test_header_versioning_controller.py` & `ellar-0.4.0/tests/test_versioning/test_header_versioning_controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_versioning/test_host_versioning.py` & `ellar-0.4.0/tests/test_versioning/test_host_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_versioning/test_query_versioning.py` & `ellar-0.4.0/tests/test_versioning/test_query_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_versioning/test_url_versioning.py` & `ellar-0.4.0/tests/test_versioning/test_url_versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_websocket.py` & `ellar-0.4.0/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `ellar-0.3.8/tests/test_websocket_handler.py` & `ellar-0.4.0/tests/test_websocket_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,25 +136,28 @@
     with client.websocket_connect(f"{prefix}/ws?query=my-query") as websocket:
         websocket.send_text("Ellar")
         message = websocket.receive_json()
         assert message == {"message": "Thanks. Ellar"}
 
 
 def test_websocket_setup_fails_when_using_body_without_handler():
+    tm = Test.create_test_module()
     with pytest.raises(
         ImproperConfiguration,
         match=r"`WsBody` should only be used when `use_extra_handler` flag is set to True in WsRoute",
     ):
 
         @router.ws_route("/ws-with-handler", use_extra_handler=False)
         async def websocket_with_handler(
             websocket: WebSocket, query: str, data: Item = WsBody()
         ):
             pass
 
+        tm.create_application().router.append(websocket_with_handler)
+
 
 def test_websocket_endpoint_on_connect():
     @Controller("/ws")
     class WebSocketSample:
         @ws_route(use_extra_handler=True)
         async def ws(self, websocket: WebSocket):
             pass
```

### Comparing `ellar-0.3.8/PKG-INFO` & `ellar-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar
-Version: 0.3.8
+Version: 0.4.0
 Summary: Ellar - Python ASGI web framework for building fast, efficient and scalable RESTAPIs and server-side application.
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -374,10 +374,9 @@
 ```
 
 See the [Doc](https://eadwincode.github.io/ellar/templating/templating/) for more examples.
 
 ## Project Status
 Project is still in development
 - Documentation - (in progress)
-- Interceptors  -  [Aspect Oriented Programming](https://en.wikipedia.org/wiki/Aspect-oriented_programming) (AOP) technique
 - Database Plugin with [Encode/ORM](https://github.com/encode/orm)
```

