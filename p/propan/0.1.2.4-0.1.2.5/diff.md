# Comparing `tmp/propan-0.1.2.4.tar.gz` & `tmp/propan-0.1.2.5.tar.gz`

## Comparing `propan-0.1.2.4.tar` & `propan-0.1.2.5.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.4/SECURITY.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 propan-0.1.2.4/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.4/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.4/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.4/examples/sqs/1_basic.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/__about__.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/__main__.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/py.typed
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/log/logging.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/nats.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/redis.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/sqs.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.4/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.4/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.4/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.4/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.4/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.2.4/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.4/LICENSE
--rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.4/README.md
--rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.4/pyproject.toml
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.5/SECURITY.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.5/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.5/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.5/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.5/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/__about__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/__main__.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/py.typed
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    10695 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/log/logging.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/nats.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/redis.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/sqs.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.5/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.5/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.5/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.5/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.5/scripts/test.sh
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.2.5/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.5/LICENSE
+-rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.5/README.md
+-rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.5/pyproject.toml
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.5/PKG-INFO
```

### Comparing `propan-0.1.2.4/CONTRIBUTING.md` & `propan-0.1.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/SECURITY.md` & `propan-0.1.2.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/.github/workflows/documentation.yml` & `propan-0.1.2.5/.github/workflows/documentation.yml`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 on:
   push:
     branches:
       - main
     paths:
       - docs/**
+      - .github/workflows/documentation.yml
 
 permissions:
   contents: write
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
```

### Comparing `propan-0.1.2.4/.github/workflows/publish_coverage.yml` & `propan-0.1.2.5/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/.github/workflows/publish_pypi.yml` & `propan-0.1.2.5/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/.github/workflows/tests.yml` & `propan-0.1.2.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/3_lifespan_events.py` & `propan-0.1.2.5/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/4_cli_attributes_promotion.py` & `propan-0.1.2.5/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/5_publishing.py` & `propan-0.1.2.5/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/6_arguments_casting.py` & `propan-0.1.2.5/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/7_handler_errors_processing.py` & `propan-0.1.2.5/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/dependencies/1_dependency_injection.py` & `propan-0.1.2.5/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.2.5/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.2.5/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.2.5/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.2.5/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/dependencies/7_annotated.py` & `propan-0.1.2.5/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.2.5/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.2.5/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.2.5/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.2.5/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/http_frameworks_integrations/quart.py` & `propan-0.1.2.5/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.2.5/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.2.5/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/rabbit/direct.py` & `propan-0.1.2.5/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/rabbit/fanout.py` & `propan-0.1.2.5/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/rabbit/header.py` & `propan-0.1.2.5/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/rabbit/topic.py` & `propan-0.1.2.5/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/redis/direct.py` & `propan-0.1.2.5/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/examples/redis/pattern.py` & `propan-0.1.2.5/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/__init__.py` & `propan-0.1.2.5/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/annotations.py` & `propan-0.1.2.5/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/types.py` & `propan-0.1.2.5/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/push_back_watcher.py` & `propan-0.1.2.5/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/_model/broker_usecase.py` & `propan-0.1.2.5/propan/brokers/_model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/_model/schemas.py` & `propan-0.1.2.5/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/_model/utils.py` & `propan-0.1.2.5/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.2.5/propan/brokers/kafka/kafka_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,19 @@
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
     async def start(self) -> None:
+        context.set_local(
+            "log_context",
+            self._get_log_context(None, ""),
+        )
+
         await super().start()
 
         for handler in self.handlers:  # pragma: no branch
             c = self._get_log_context(None, handler.topics)
             self._log(f"`{handler.callback.__name__}` waiting for messages", extra=c)
 
             consumer = self._connection(*handler.topics, **handler.consumer_kwargs)
@@ -189,16 +194,18 @@
     def _get_log_context(
         self,
         message: Optional[PropanMessage],
         topics: Sequence[str] = (),
     ) -> Dict[str, Any]:
         if topics:
             topic = ", ".join(topics)
-        else:
+        elif message is not None:
             topic = message.raw_message.topic
+        else:
+            topic = ""
 
         return {
             "topic": topic,
             **super()._get_log_context(message),
         }
 
     async def _consume(self, handler: Handler) -> NoReturn:
```

### Comparing `propan-0.1.2.4/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.2.5/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/nats/nats_broker.py` & `propan-0.1.2.5/propan/brokers/nats/nats_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from nats.aio.msg import Msg
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.types import AnyDict, DecoratedCallable, SendableMessage
+from propan.utils import context
 
 T = TypeVar("T")
 
 
 class NatsBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Optional[Client]
@@ -68,14 +69,19 @@
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
     async def start(self) -> None:
+        context.set_local(
+            "log_context",
+            self._get_log_context(None, ""),
+        )
+
         await super().start()
 
         for handler in self.handlers:
             func = handler.callback
 
             c = self._get_log_context(None, handler.subject, handler.queue)
             self._log(f"`{func.__name__}` waiting for messages", extra=c)
```

### Comparing `propan-0.1.2.4/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.2.5/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.2.5/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/nats/schemas.py` & `propan-0.1.2.5/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.2.5/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from aio_pika.abc import DeliveryMode
 
 from propan.brokers._model import BrokerUsecase
 from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.types import AnyDict, DecoratedCallable, HandlerWrapper, SendableMessage
+from propan.utils import context
 
 TimeoutType = Optional[Union[int, float]]
 PikaSendableMessage = Union[aio_pika.message.Message, SendableMessage]
 T = TypeVar("T")
 
 
 class RabbitBroker(BrokerUsecase):
@@ -92,14 +93,19 @@
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
     async def start(self) -> None:
+        context.set_local(
+            "log_context",
+            self._get_log_context(None, RabbitQueue(""), RabbitExchange("")),
+        )
+
         await super().start()
 
         for handler in self.handlers:
             queue = await self._init_handler(handler)
 
             func = handler.callback
```

### Comparing `propan-0.1.2.4/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.2.5/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/redis/redis_broker.py` & `propan-0.1.2.5/propan/brokers/redis/redis_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from propan.types import (
     AnyCallable,
     DecodedMessage,
     DecoratedCallable,
     HandlerWrapper,
     SendableMessage,
 )
+from propan.utils import context
 
 T = TypeVar("T")
 
 
 class RedisBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Redis
@@ -109,14 +110,19 @@
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
     async def start(self) -> None:
+        context.set_local(
+            "log_context",
+            self._get_log_context(None, ""),
+        )
+
         await super().start()
 
         for handler in self.handlers:  # pragma: no branch
             c = self._get_log_context(None, handler.channel)
             self._log(f"`{handler.callback.__name__}` waiting for messages", extra=c)
 
             psub = self._connection.pubsub()
```

### Comparing `propan-0.1.2.4/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.2.5/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/redis/schemas.py` & `propan-0.1.2.5/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.2.5/propan/brokers/sqs/sqs_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,19 @@
             handler = Handler(callback=func, queue=queue, consumer_params=params)
             self.handlers.append(handler)
             return func
 
         return wrapper
 
     async def start(self) -> None:
+        context.set_local(
+            "log_context",
+            self._get_log_context(None, ""),
+        )
+
         await super().start()
 
         for handler in self.handlers:  # pragma: no branch
             c = self._get_log_context(None, handler.queue.name)
             self._log(f"`{handler.callback.__name__}` waiting for messages", extra=c)
 
             url = await self.create_queue(handler.queue)
```

### Comparing `propan-0.1.2.4/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.2.5/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/app.py` & `propan-0.1.2.5/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/main.py` & `propan-0.1.2.5/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/startproject/core.py` & `propan-0.1.2.5/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/startproject/async_app/app.py` & `propan-0.1.2.5/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/startproject/async_app/core.py` & `propan-0.1.2.5/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.2.5/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/startproject/async_app/nats.py` & `propan-0.1.2.5/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.2.5/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/startproject/async_app/redis.py` & `propan-0.1.2.5/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.2.5/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/supervisors/basereload.py` & `propan-0.1.2.5/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/supervisors/multiprocess.py` & `propan-0.1.2.5/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/supervisors/utils.py` & `propan-0.1.2.5/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/supervisors/watchfiles.py` & `propan-0.1.2.5/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/utils/imports.py` & `propan-0.1.2.5/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/utils/logs.py` & `propan-0.1.2.5/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/cli/utils/parser.py` & `propan-0.1.2.5/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/fastapi/__init__.py` & `propan-0.1.2.5/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/fastapi/core/route.py` & `propan-0.1.2.5/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/fastapi/core/router.py` & `propan-0.1.2.5/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/fastapi/kafka/router.pyi` & `propan-0.1.2.5/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/fastapi/nats/router.pyi` & `propan-0.1.2.5/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/fastapi/rabbit/router.pyi` & `propan-0.1.2.5/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/fastapi/redis/router.pyi` & `propan-0.1.2.5/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/fastapi/sqs/router.pyi` & `propan-0.1.2.5/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/log/formatter.py` & `propan-0.1.2.5/propan/log/formatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import logging
 import sys
 from collections import defaultdict
-from typing import Callable, DefaultDict, Optional
+from types import TracebackType
+from typing import Callable, DefaultDict, Mapping, Optional, Tuple, Type, Union
 
 import click
 from typing_extensions import Literal
 
 from propan.utils.context.main import context
 
+original_makeRecord = logging.Logger.makeRecord
+
 
 class ColourizedFormatter(logging.Formatter):
     level_name_colors: DefaultDict[str, Callable[[str], str]] = defaultdict(
         lambda: str,
         **{
             str(logging.DEBUG): lambda level_name: click.style(
                 str(level_name), fg="cyan"
@@ -63,21 +66,40 @@
         levelname = expand_log_field(record.levelname, 8)
         if self.use_colors is True:  # pragma: no cover
             levelname = self.color_level_name(levelname, record.levelno)
         record.__dict__["levelname"] = levelname
         return super().formatMessage(record)
 
 
-class DefaultFormatter(ColourizedFormatter):
-    pass
+def make_record_with_extra(
+    self: logging.Logger,
+    name: str,
+    level: int,
+    fn: str,
+    lno: int,
+    msg: str,
+    args: Tuple[str],
+    exc_info: Optional[
+        Union[
+            Tuple[Type[BaseException], BaseException, Optional[TracebackType]],
+            Tuple[None, None, None],
+        ]
+    ],
+    func: Optional[str] = None,
+    extra: Optional[Mapping[str, object]] = None,
+    sinfo: Optional[str] = None,
+) -> logging.LogRecord:
+    if extra is None:
+        extra = context.get_local("log_context")
 
+    record = original_makeRecord(
+        self, name, level, fn, lno, msg, args, exc_info, func, extra, sinfo
+    )
 
-class AccessFormatter(ColourizedFormatter):
-    def formatMessage(self, record: logging.LogRecord) -> str:
-        c = context.get_local("log_context")
-        if c:  # pragma: no cover
-            record.__dict__.update(c)
-        return super().formatMessage(record)
+    return record
 
 
 def expand_log_field(field: str, symbols: int) -> str:
     return field + (" " * (symbols - len(field)))
+
+
+logging.Logger.makeRecord = make_record_with_extra  # type: ignore
```

### Comparing `propan-0.1.2.4/propan/log/logging.py` & `propan-0.1.2.5/propan/log/logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import logging
 import logging.config
 from functools import partial
 from typing import Any, Dict, Type
 
-from propan.log.formatter import AccessFormatter, DefaultFormatter
+from propan.log.formatter import ColourizedFormatter
 
 
 def configure_formatter(
     formatter: Type[logging.Formatter], *args: Any, **kwargs: Any
 ) -> logging.Formatter:
     return formatter(*args, **kwargs)
 
 
 LOGGING_CONFIG: Dict[str, Any] = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
         "default": {
-            "()": partial(configure_formatter, DefaultFormatter),
+            "()": partial(configure_formatter, ColourizedFormatter),
             "fmt": "%(asctime)s %(levelname)s - %(message)s",
             "use_colors": True,
         },
         "access": {
-            "()": partial(configure_formatter, AccessFormatter),
+            "()": partial(configure_formatter, ColourizedFormatter),
             "fmt": "%(asctime)s %(levelname)s - %(message)s",
             "use_colors": True,
         },
     },
     "handlers": {
         "default": {
             "formatter": "default",
```

### Comparing `propan-0.1.2.4/propan/test/__init__.py` & `propan-0.1.2.5/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/test/kafka.py` & `propan-0.1.2.5/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/test/nats.py` & `propan-0.1.2.5/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/test/rabbit.py` & `propan-0.1.2.5/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/test/redis.py` & `propan-0.1.2.5/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/test/sqs.py` & `propan-0.1.2.5/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/test/utils.py` & `propan-0.1.2.5/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/utils/functions.py` & `propan-0.1.2.5/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/utils/context/main.py` & `propan-0.1.2.5/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/propan/utils/context/types.py` & `propan-0.1.2.5/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/LICENSE` & `propan-0.1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/README.md` & `propan-0.1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/pyproject.toml` & `propan-0.1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.4/PKG-INFO` & `propan-0.1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.2.4
+Version: 0.1.2.5
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.2.4 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.2.5 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-File: LICENSE Keywords: framework,message brokers,rabbitmq
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

