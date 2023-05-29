# Comparing `tmp/skip-django-security-logger-1.5.15.1.tar.gz` & `tmp/skip-django-security-logger-1.5.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-security-logger-1.5.15.1.tar", last modified: Mon Jan 30 02:04:45 2023, max compression
+gzip compressed data, was "skip-django-security-logger-1.5.15.2.tar", last modified: Mon May 29 22:57:15 2023, max compression
```

## Comparing `skip-django-security-logger-1.5.15.1.tar` & `skip-django-security-logger-1.5.15.2.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.623009 skip-django-security-logger-1.5.15.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-01-30 02:04:45.623009 skip-django-security-logger-1.5.15.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.595009 skip-django-security-logger-1.5.15.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.595009 skip-django-security-logger-1.5.15.1/example/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.595009 skip-django-security-logger-1.5.15.1/example/apps/test_security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.595009 skip-django-security-logger-1.5.15.1/example/apps/test_security/management/
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.595009 skip-django-security-logger-1.5.15.1/example/apps/test_security/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/management/commands/create_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/management/commands/create_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/management/commands/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/management/commands/test_command_with_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/management/commands/test_error_command.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.599009 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    53788 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/celery_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/command_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    31077 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/input_request_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    20624 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/output_request_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/throttling_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/apps/test_security/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.599009 skip-django-security-logger-1.5.15.1/example/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/settings/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/test_elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/example/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.607009 skip-django-security-logger-1.5.15.1/security/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.607009 skip-django-security-logger-1.5.15.1/security/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.607009 skip-django-security-logger-1.5.15.1/security/backends/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18939 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/common/is_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/common/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.607009 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.611009 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/is_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/is_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/is_core/cores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/is_core/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.611009 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/logstash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/logstash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/logstash/handler_tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/logstash/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.611009 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.611009 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/management/commands/init_elasticsearch_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.611009 skip-django-security-logger-1.5.15.1/security/backends/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/logging/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/logging/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/purge_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.611009 skip-django-security-logger-1.5.15.1/security/backends/sql/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/db_router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.615009 skip-django-security-logger-1.5.15.1/security/backends/sql/is_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/is_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/is_core/cores.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/is_core/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.615009 skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/0002_auto_20211119_1940.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/0003_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/0004_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/sql/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.615009 skip-django-security-logger-1.5.15.1/security/backends/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/testing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/testing/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/testing/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/backends/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.615009 skip-django-security-logger-1.5.15.1/security/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.615009 skip-django-security-logger-1.5.15.1/security/contrib/debug_toolbar_log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/contrib/debug_toolbar_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/contrib/debug_toolbar_log/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.615009 skip-django-security-logger-1.5.15.1/security/contrib/pyston/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/contrib/pyston/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/contrib/pyston/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.591009 skip-django-security-logger-1.5.15.1/security/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.591009 skip-django-security-logger-1.5.15.1/security/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.615009 skip-django-security-logger-1.5.15.1/security/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/log_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.619009 skip-django-security-logger-1.5.15.1/security/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.619009 skip-django-security-logger-1.5.15.1/security/logging/celery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/logging/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/logging/celery/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.619009 skip-django-security-logger-1.5.15.1/security/logging/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/logging/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/logging/commands/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/logging/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.619009 skip-django-security-logger-1.5.15.1/security/logging/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/logging/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/logging/requests/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/logging/requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.619009 skip-django-security-logger-1.5.15.1/security/management/
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.619009 skip-django-security-logger-1.5.15.1/security/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/management/commands/purge_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/management/commands/set_celery_task_log_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/storages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/suds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.619009 skip-django-security-logger-1.5.15.1/security/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/templates/429.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.619009 skip-django-security-logger-1.5.15.1/security/throttling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/throttling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/throttling/default_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/throttling/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/throttling/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/throttling/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/security/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 02:04:45.623009 skip-django-security-logger-1.5.15.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-01-30 02:04:34.000000 skip-django-security-logger-1.5.15.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 02:04:45.623009 skip-django-security-logger-1.5.15.1/skip_django_security_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-01-30 02:04:45.000000 skip-django-security-logger-1.5.15.1/skip_django_security_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-01-30 02:04:45.000000 skip-django-security-logger-1.5.15.1/skip_django_security_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 02:04:45.000000 skip-django-security-logger-1.5.15.1/skip_django_security_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 02:04:45.000000 skip-django-security-logger-1.5.15.1/skip_django_security_logger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-30 02:04:45.000000 skip-django-security-logger-1.5.15.1/skip_django_security_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-30 02:04:45.000000 skip-django-security-logger-1.5.15.1/skip_django_security_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.759430 skip-django-security-logger-1.5.15.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-29 22:57:15.759430 skip-django-security-logger-1.5.15.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.739430 skip-django-security-logger-1.5.15.2/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.739430 skip-django-security-logger-1.5.15.2/example/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.739430 skip-django-security-logger-1.5.15.2/example/apps/test_security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.739430 skip-django-security-logger-1.5.15.2/example/apps/test_security/management/
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.739430 skip-django-security-logger-1.5.15.2/example/apps/test_security/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/management/commands/create_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/management/commands/create_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/management/commands/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/management/commands/test_command_with_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/management/commands/test_error_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.743430 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53788 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/celery_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/command_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31077 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/input_request_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20624 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/output_request_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/throttling_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/apps/test_security/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.743430 skip-django-security-logger-1.5.15.2/example/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/settings/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/test_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/example/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.747430 skip-django-security-logger-1.5.15.2/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.747430 skip-django-security-logger-1.5.15.2/security/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.747430 skip-django-security-logger-1.5.15.2/security/backends/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18939 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/common/is_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/common/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.747430 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.747430 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/is_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/is_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/is_core/cores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/is_core/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.751430 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/logstash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/logstash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/logstash/handler_tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/logstash/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.751430 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.751430 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/management/commands/init_elasticsearch_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.751430 skip-django-security-logger-1.5.15.2/security/backends/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/logging/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/logging/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/purge_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.751430 skip-django-security-logger-1.5.15.2/security/backends/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/db_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.751430 skip-django-security-logger-1.5.15.2/security/backends/sql/is_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/is_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/is_core/cores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/is_core/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/0002_auto_20211119_1940.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/0003_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/0004_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/sql/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/backends/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/testing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/testing/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/testing/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/backends/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/contrib/debug_toolbar_log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/contrib/debug_toolbar_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/contrib/debug_toolbar_log/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/contrib/pyston/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/contrib/pyston/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/contrib/pyston/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.731429 skip-django-security-logger-1.5.15.2/security/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.731429 skip-django-security-logger-1.5.15.2/security/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/log_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/logging/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/logging/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/logging/celery/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/logging/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/logging/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/logging/commands/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/logging/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/logging/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/logging/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/logging/requests/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/logging/requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.755430 skip-django-security-logger-1.5.15.2/security/management/
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.759430 skip-django-security-logger-1.5.15.2/security/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/management/commands/purge_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/management/commands/set_celery_task_log_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/suds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.759430 skip-django-security-logger-1.5.15.2/security/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/templates/429.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.759430 skip-django-security-logger-1.5.15.2/security/throttling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/throttling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/throttling/default_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/throttling/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/throttling/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/throttling/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/security/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:57:15.759430 skip-django-security-logger-1.5.15.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-29 22:57:07.000000 skip-django-security-logger-1.5.15.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:57:15.759430 skip-django-security-logger-1.5.15.2/skip_django_security_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-29 22:57:15.000000 skip-django-security-logger-1.5.15.2/skip_django_security_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-29 22:57:15.000000 skip-django-security-logger-1.5.15.2/skip_django_security_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:57:15.000000 skip-django-security-logger-1.5.15.2/skip_django_security_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:57:15.000000 skip-django-security-logger-1.5.15.2/skip_django_security_logger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 22:57:15.000000 skip-django-security-logger-1.5.15.2/skip_django_security_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 22:57:15.000000 skip-django-security-logger-1.5.15.2/skip_django_security_logger.egg-info/top_level.txt
```

### Comparing `skip-django-security-logger-1.5.15.1/LICENSE` & `skip-django-security-logger-1.5.15.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/PKG-INFO` & `skip-django-security-logger-1.5.15.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-security-logger
-Version: 1.5.15.1
+Version: 1.5.15.2
 Summary: Django security library.
 Home-page: https://github.com/skip-pay/django-security
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,throttling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/management/__init__.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/management/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/tasks.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/tasks.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/base.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/celery_log.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/celery_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/command_log.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/command_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/commands.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/commands.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/input_request_log.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/input_request_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/output_request_log.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/output_request_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/tests/utils.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/apps/test_security/views.py` & `skip-django-security-logger-1.5.15.2/example/apps/test_security/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/settings/base.py` & `skip-django-security-logger-1.5.15.2/example/settings/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/settings/settings.py` & `skip-django-security-logger-1.5.15.2/example/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/test_elastic.py` & `skip-django-security-logger-1.5.15.2/example/test_elastic.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/urls.py` & `skip-django-security-logger-1.5.15.2/example/urls.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/example/wsgi.py` & `skip-django-security-logger-1.5.15.2/example/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/app.py` & `skip-django-security-logger-1.5.15.2/security/backends/app.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/common/is_core.py` & `skip-django-security-logger-1.5.15.2/security/backends/common/is_core.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/common/mixins.py` & `skip-django-security-logger-1.5.15.2/security/backends/common/mixins.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/connection.py` & `skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
     def connect(self, init_documents):
         if not self.connection:
             if not settings.ELASTICSEARCH_DATABASE:
                 raise ImproperlyConfigured('You must set "SECURITY_ELASTICSEARCH_DATABASE" setting')
 
             connection.connection = connections.create_connection(
-                **settings.ELASTICSEARCH_DATABASE
+                **settings.ELASTICSEARCH_DATABASE,
+                timeout=settings.ELASTICSEARCH_TIMEOUT,
             )
             if init_documents:
                 self.init_documents()
 
     def init_documents(self):
         from security.backends.elasticsearch.models import (
             InputRequestLog, OutputRequestLog, CommandLog, CeleryTaskRunLog, CeleryTaskInvocationLog
```

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/is_core/cores.py` & `skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/is_core/cores.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/is_core/filters.py` & `skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/is_core/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/logstash/handler_tcp.py` & `skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/logstash/handler_tcp.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/management/commands/init_elasticsearch_log.py` & `skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/management/commands/init_elasticsearch_log.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/models.py` & `skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/reader.py` & `skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/reader.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/tests.py` & `skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/tests.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/elasticsearch/writer.py` & `skip-django-security-logger-1.5.15.2/security/backends/elasticsearch/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/logging/writer.py` & `skip-django-security-logger-1.5.15.2/security/backends/logging/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/purge_logs.py` & `skip-django-security-logger-1.5.15.2/security/backends/purge_logs.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/reader.py` & `skip-django-security-logger-1.5.15.2/security/backends/reader.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/signals.py` & `skip-django-security-logger-1.5.15.2/security/backends/signals.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/app.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/app.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/db_router.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/db_router.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/is_core/cores.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/is_core/cores.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/is_core/filters.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/is_core/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/0001_initial.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/0002_auto_20211119_1940.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/0002_auto_20211119_1940.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/0003_migration.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/0003_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/migrations/0004_migration.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/migrations/0004_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/models.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/reader.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/reader.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/sql/writer.py` & `skip-django-security-logger-1.5.15.2/security/backends/sql/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/testing/reader.py` & `skip-django-security-logger-1.5.15.2/security/backends/testing/reader.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/testing/writer.py` & `skip-django-security-logger-1.5.15.2/security/backends/testing/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/backends/writer.py` & `skip-django-security-logger-1.5.15.2/security/backends/writer.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/command.py` & `skip-django-security-logger-1.5.15.2/security/command.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/config.py` & `skip-django-security-logger-1.5.15.2/security/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     'ELASTICSEARCH_AUTO_REFRESH': False,
     'ELASTICSEARCH_CLEAN_LOGS_READ_BATCH_SIZE': 1000,
     'ELASTICSEARCH_CLEAN_LOGS_DELETE_BATCH_SIZE': 1000,
     'ELASTICSEARCH_CLEAN_LOGS_DELETE_REQUEST_TIMEOUT': 30,
     'ELASTICSEARCH_CLEAN_LOGS_DELETE_ATTEMPTS': 10,
     'ELASTICSEARCH_CLEAN_LOGS_DELETE_ATTEMPT_SLEEP': 5,
     'ELASTICSEARCH_MAX_NUMBER_OF_TERMS': 65536,
+    'ELASTICSEARCH_TIMEOUT': 10,
     'SQL_CLEAN_LOGS_DELETE_BATCH_SIZE': 1000,
     'BACKEND_WRITERS': None,
     'BACKEND_READER': None,
     'LOG_STRING_IO_FLUSH_TIMEOUT': 5,
     'SET_STALE_CELERY_INVOCATIONS_LIMIT_PER_RUN': 1000,
     'RELEASE': None,
     'LOG_MAX_REVISIONS_COUNT': 20,
```

### Comparing `skip-django-security-logger-1.5.15.1/security/contrib/debug_toolbar_log/middleware.py` & `skip-django-security-logger-1.5.15.2/security/contrib/debug_toolbar_log/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/contrib/pyston/resources.py` & `skip-django-security-logger-1.5.15.2/security/contrib/pyston/resources.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/decorators.py` & `skip-django-security-logger-1.5.15.2/security/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/enums.py` & `skip-django-security-logger-1.5.15.2/security/enums.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/locale/cs/LC_MESSAGES/django.mo` & `skip-django-security-logger-1.5.15.2/security/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/locale/cs/LC_MESSAGES/django.po` & `skip-django-security-logger-1.5.15.2/security/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/logging/celery/logger.py` & `skip-django-security-logger-1.5.15.2/security/logging/celery/logger.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/logging/commands/logger.py` & `skip-django-security-logger-1.5.15.2/security/logging/commands/logger.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/logging/common.py` & `skip-django-security-logger-1.5.15.2/security/logging/common.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/logging/requests/logger.py` & `skip-django-security-logger-1.5.15.2/security/logging/requests/logger.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/logging/requests/utils.py` & `skip-django-security-logger-1.5.15.2/security/logging/requests/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/management/__init__.py` & `skip-django-security-logger-1.5.15.2/security/management/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/management/commands/purge_logs.py` & `skip-django-security-logger-1.5.15.2/security/management/commands/purge_logs.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/middleware.py` & `skip-django-security-logger-1.5.15.2/security/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/requests.py` & `skip-django-security-logger-1.5.15.2/security/requests.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/suds.py` & `skip-django-security-logger-1.5.15.2/security/suds.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/task.py` & `skip-django-security-logger-1.5.15.2/security/task.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/throttling/validators.py` & `skip-django-security-logger-1.5.15.2/security/throttling/validators.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/security/utils.py` & `skip-django-security-logger-1.5.15.2/security/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/setup.py` & `skip-django-security-logger-1.5.15.2/setup.py`

 * *Files identical despite different names*

### Comparing `skip-django-security-logger-1.5.15.1/skip_django_security_logger.egg-info/PKG-INFO` & `skip-django-security-logger-1.5.15.2/skip_django_security_logger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-security-logger
-Version: 1.5.15.1
+Version: 1.5.15.2
 Summary: Django security library.
 Home-page: https://github.com/skip-pay/django-security
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,throttling
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip-django-security-logger-1.5.15.1/skip_django_security_logger.egg-info/SOURCES.txt` & `skip-django-security-logger-1.5.15.2/skip_django_security_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

