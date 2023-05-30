# Comparing `tmp/drf-stripe-subscription-1.1.9.tar.gz` & `tmp/drf-stripe-subscription-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-stripe-subscription-1.1.9.tar", last modified: Mon Feb 14 03:27:56 2022, max compression
+gzip compressed data, was "drf-stripe-subscription-1.2.0.tar", last modified: Tue May 30 16:17:11 2023, max compression
```

## Comparing `drf-stripe-subscription-1.1.9.tar` & `drf-stripe-subscription-1.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2022-02-14 03:27:56.696796 drf-stripe-subscription-1.1.9/
--rw-r--r--   0 oscarchen   (501) staff       (20)     1069 2022-01-13 07:52:03.000000 drf-stripe-subscription-1.1.9/LICENSE
--rw-r--r--   0 oscarchen   (501) staff       (20)       68 2022-01-12 23:37:56.000000 drf-stripe-subscription-1.1.9/MANIFEST.in
--rw-r--r--   0 oscarchen   (501) staff       (20)    13009 2022-02-14 03:27:56.696935 drf-stripe-subscription-1.1.9/PKG-INFO
--rw-r--r--   0 oscarchen   (501) staff       (20)     9567 2022-02-13 20:00:27.000000 drf-stripe-subscription-1.1.9/README.md
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2022-02-14 03:27:56.692627 drf-stripe-subscription-1.1.9/drf_stripe/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-01-06 23:11:07.000000 drf-stripe-subscription-1.1.9/drf_stripe/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      158 2022-02-08 16:33:41.000000 drf-stripe-subscription-1.1.9/drf_stripe/admin.py
--rw-r--r--   0 oscarchen   (501) staff       (20)       94 2022-01-07 23:54:41.000000 drf-stripe-subscription-1.1.9/drf_stripe/apps.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2022-02-14 03:27:56.692746 drf-stripe-subscription-1.1.9/drf_stripe/management/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-01-11 05:52:45.000000 drf-stripe-subscription-1.1.9/drf_stripe/management/__init__.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2022-02-14 03:27:56.693359 drf-stripe-subscription-1.1.9/drf_stripe/management/commands/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-01-11 05:52:37.000000 drf-stripe-subscription-1.1.9/drf_stripe/management/commands/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      368 2022-01-16 00:21:38.000000 drf-stripe-subscription-1.1.9/drf_stripe/management/commands/pull_stripe.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      592 2022-01-15 22:46:42.000000 drf-stripe-subscription-1.1.9/drf_stripe/management/commands/update_stripe_customers.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      349 2022-01-15 21:48:02.000000 drf-stripe-subscription-1.1.9/drf_stripe/management/commands/update_stripe_products.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      605 2022-01-15 22:44:32.000000 drf-stripe-subscription-1.1.9/drf_stripe/management/commands/update_stripe_subscriptions.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2022-02-14 03:27:56.693871 drf-stripe-subscription-1.1.9/drf_stripe/migrations/
--rw-r--r--   0 oscarchen   (501) staff       (20)     5146 2022-01-13 22:48:52.000000 drf-stripe-subscription-1.1.9/drf_stripe/migrations/0001_initial.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     2168 2022-02-08 15:58:27.000000 drf-stripe-subscription-1.1.9/drf_stripe/migrations/0002_alter_feature_description_alter_price_freq_and_more.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      471 2022-02-09 01:53:49.000000 drf-stripe-subscription-1.1.9/drf_stripe/migrations/0003_price_currency.py
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-01-08 00:18:02.000000 drf-stripe-subscription-1.1.9/drf_stripe/migrations/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     4978 2022-02-13 18:47:45.000000 drf-stripe-subscription-1.1.9/drf_stripe/models.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     4450 2022-02-09 01:53:49.000000 drf-stripe-subscription-1.1.9/drf_stripe/serializers.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1987 2022-02-14 03:24:27.000000 drf-stripe-subscription-1.1.9/drf_stripe/settings.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2022-02-14 03:27:56.694661 drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-01-08 20:56:39.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      169 2022-01-14 09:47:14.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/api.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     5274 2022-02-14 03:24:27.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/checkout.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      555 2022-01-11 04:48:15.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/customer_portal.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     5914 2022-01-16 21:38:36.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/customers.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     3956 2022-02-09 01:53:49.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/products.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     7077 2022-01-16 00:04:47.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/subscriptions.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2022-02-14 03:27:56.695582 drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-01-07 06:44:49.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     2233 2022-01-07 03:03:28.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/currency.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1307 2022-01-15 21:31:01.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/customer.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     3070 2022-01-12 07:20:15.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/event.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1350 2022-01-11 18:20:51.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/invoice.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1407 2022-01-16 00:44:56.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/price.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1286 2022-01-12 05:42:40.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/product.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     2324 2022-01-15 21:55:42.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/subscription.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2022-02-14 03:27:56.696132 drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/
--rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-01-11 17:49:45.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/__init__.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     1654 2022-01-15 22:37:59.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/customer_subscription.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     2766 2022-01-14 09:51:24.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/handler.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      797 2022-02-09 01:53:49.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/price.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      608 2022-01-14 09:52:17.000000 drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/product.py
--rw-r--r--   0 oscarchen   (501) staff       (20)      474 2022-01-13 06:52:10.000000 drf-stripe-subscription-1.1.9/drf_stripe/urls.py
--rw-r--r--   0 oscarchen   (501) staff       (20)     3045 2022-02-08 05:37:22.000000 drf-stripe-subscription-1.1.9/drf_stripe/views.py
-drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2022-02-14 03:27:56.696695 drf-stripe-subscription-1.1.9/drf_stripe_subscription.egg-info/
--rw-r--r--   0 oscarchen   (501) staff       (20)    13009 2022-02-14 03:27:56.000000 drf-stripe-subscription-1.1.9/drf_stripe_subscription.egg-info/PKG-INFO
--rw-r--r--   0 oscarchen   (501) staff       (20)     1693 2022-02-14 03:27:56.000000 drf-stripe-subscription-1.1.9/drf_stripe_subscription.egg-info/SOURCES.txt
--rw-r--r--   0 oscarchen   (501) staff       (20)        1 2022-02-14 03:27:56.000000 drf-stripe-subscription-1.1.9/drf_stripe_subscription.egg-info/dependency_links.txt
--rw-r--r--   0 oscarchen   (501) staff       (20)       37 2022-02-14 03:27:56.000000 drf-stripe-subscription-1.1.9/drf_stripe_subscription.egg-info/requires.txt
--rw-r--r--   0 oscarchen   (501) staff       (20)       17 2022-02-14 03:27:56.000000 drf-stripe-subscription-1.1.9/drf_stripe_subscription.egg-info/top_level.txt
--rw-r--r--   0 oscarchen   (501) staff       (20)     1135 2022-02-14 03:27:56.697364 drf-stripe-subscription-1.1.9/setup.cfg
--rw-r--r--   0 oscarchen   (501) staff       (20)      153 2022-01-12 23:37:56.000000 drf-stripe-subscription-1.1.9/setup.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.115735 drf-stripe-subscription-1.2.0/
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1069 2023-02-26 17:26:47.000000 drf-stripe-subscription-1.2.0/LICENSE
+-rw-r--r--   0 oscarchen   (501) staff       (20)       68 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/MANIFEST.in
+-rw-r--r--   0 oscarchen   (501) staff       (20)    13927 2023-05-30 16:17:11.115875 drf-stripe-subscription-1.2.0/PKG-INFO
+-rw-r--r--   0 oscarchen   (501) staff       (20)    10294 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/README.md
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.111434 drf-stripe-subscription-1.2.0/drf_stripe/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      158 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/admin.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)       94 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/apps.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.111548 drf-stripe-subscription-1.2.0/drf_stripe/management/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/__init__.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.112145 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      368 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/pull_stripe.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      592 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_customers.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      349 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_products.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      605 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_subscriptions.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.112635 drf-stripe-subscription-1.2.0/drf_stripe/migrations/
+-rw-r--r--   0 oscarchen   (501) staff       (20)     5146 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/migrations/0001_initial.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2168 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/migrations/0002_alter_feature_description_alter_price_freq_and_more.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      471 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/migrations/0003_price_currency.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/migrations/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     4978 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/models.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     4554 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/serializers.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2176 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/settings.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.113434 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      169 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/api.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     5764 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/checkout.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      555 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/customer_portal.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)    11631 2023-05-30 16:07:47.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/customers.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     3956 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/products.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     7694 2023-05-30 16:07:47.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/subscriptions.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.114409 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2233 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/currency.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1307 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/customer.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     3070 2023-01-20 04:18:32.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/event.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1344 2023-01-20 04:18:32.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/invoice.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1407 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/price.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1286 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/product.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2329 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/subscription.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.115018 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/
+-rw-r--r--   0 oscarchen   (501) staff       (20)        0 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/__init__.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1654 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/customer_subscription.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     2803 2023-01-20 04:18:32.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/handler.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      797 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/price.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      608 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/product.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)      474 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/urls.py
+-rw-r--r--   0 oscarchen   (501) staff       (20)     3045 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/drf_stripe/views.py
+drwxr-xr-x   0 oscarchen   (501) staff       (20)        0 2023-05-30 16:17:11.115623 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/
+-rw-r--r--   0 oscarchen   (501) staff       (20)    13927 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/PKG-INFO
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1693 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/SOURCES.txt
+-rw-r--r--   0 oscarchen   (501) staff       (20)        1 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/dependency_links.txt
+-rw-r--r--   0 oscarchen   (501) staff       (20)       64 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/requires.txt
+-rw-r--r--   0 oscarchen   (501) staff       (20)       17 2023-05-30 16:17:11.000000 drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/top_level.txt
+-rw-r--r--   0 oscarchen   (501) staff       (20)     1196 2023-05-30 16:17:11.116215 drf-stripe-subscription-1.2.0/setup.cfg
+-rw-r--r--   0 oscarchen   (501) staff       (20)      153 2022-11-26 20:11:20.000000 drf-stripe-subscription-1.2.0/setup.py
```

### Comparing `drf-stripe-subscription-1.1.9/LICENSE` & `drf-stripe-subscription-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/PKG-INFO` & `drf-stripe-subscription-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-stripe-subscription
-Version: 1.1.9
+Version: 1.2.0
 Summary: A Django app that provides subscription features with Stripe and REST endpoints.
 Home-page: https://github.com/oscarychen/drf-stripe-subscription
 Author: Oscar Chen
 Author-email: quacky@duck.com
 License: MIT
 Description: # drf-stripe-subscription
         
@@ -283,21 +283,41 @@
         Pulls customers from Stripe and updates Django database.
         
         ```commandline
         python manage.py update_stripe_subscriptions
         ```
         
         Pulls subscriptions from Stripe and updates Django database.
+        
+        ## Working with customized Django User models
+        
+        The following DRF_STRIPE settings can be used to customize how Django creates User instance using Stripe Customer
+        attributes (default values shown):
+        
+        ```python
+        DRF_STRIPE = {
+            "DJANGO_USER_EMAIL_FIELD": "email",
+            "USER_CREATE_DEFAULTS_ATTRIBUTE_MAP": {"username": "email"},
+        }
+        ```
+        
+        The `DJANGO_USER_EMAIL_FIELD` specifies name of the Django User attribute to be used to store Stripe Customer email. It
+        will be used to look up existing Django User using Stripe Customer email.
+        
+        The `USER_CREATE_DEFAULTS_ATTRIBUTE_MAP` maps the name of Django User attribute to name of corresponding Stripe Customer
+        attribute, and is used during the automated Django User instance creation.
+        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `drf-stripe-subscription-1.1.9/README.md` & `drf-stripe-subscription-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -274,8 +274,26 @@
 
 Pulls customers from Stripe and updates Django database.
 
 ```commandline
 python manage.py update_stripe_subscriptions
 ```
 
-Pulls subscriptions from Stripe and updates Django database.
+Pulls subscriptions from Stripe and updates Django database.
+
+## Working with customized Django User models
+
+The following DRF_STRIPE settings can be used to customize how Django creates User instance using Stripe Customer
+attributes (default values shown):
+
+```python
+DRF_STRIPE = {
+    "DJANGO_USER_EMAIL_FIELD": "email",
+    "USER_CREATE_DEFAULTS_ATTRIBUTE_MAP": {"username": "email"},
+}
+```
+
+The `DJANGO_USER_EMAIL_FIELD` specifies name of the Django User attribute to be used to store Stripe Customer email. It
+will be used to look up existing Django User using Stripe Customer email.
+
+The `USER_CREATE_DEFAULTS_ATTRIBUTE_MAP` maps the name of Django User attribute to name of corresponding Stripe Customer
+attribute, and is used during the automated Django User instance creation.
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/management/commands/update_stripe_customers.py` & `drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_customers.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/management/commands/update_stripe_subscriptions.py` & `drf-stripe-subscription-1.2.0/drf_stripe/management/commands/update_stripe_subscriptions.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/migrations/0001_initial.py` & `drf-stripe-subscription-1.2.0/drf_stripe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/migrations/0002_alter_feature_description_alter_price_freq_and_more.py` & `drf-stripe-subscription-1.2.0/drf_stripe/migrations/0002_alter_feature_description_alter_price_freq_and_more.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/models.py` & `drf-stripe-subscription-1.2.0/drf_stripe/models.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/serializers.py` & `drf-stripe-subscription-1.2.0/drf_stripe/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,17 @@
     owner = serializers.HiddenField(default=serializers.CurrentUserDefault())
 
     def validate(self, attrs):
         stripe_user = get_or_create_stripe_user(user_id=self.context['request'].user.id)
         try:
             checkout_session = stripe_api_create_checkout_session(
                 customer_id=stripe_user.customer_id,
-                price_id=attrs['price_id'])
+                price_id=attrs['price_id'],
+                trial_end='auto' if stripe_user.subscription_items.count() == 0 else None
+            )
             attrs['session_id'] = checkout_session['id']
         except StripeError as e:
             raise ValidationError(e.error)
         return attrs
 
     def update(self, instance, validated_data):
         pass
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/settings.py` & `drf-stripe-subscription-1.2.0/drf_stripe/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 
 USER_SETTINGS = getattr(settings, "DRF_STRIPE", None)
 
 DEFAULTS = {
     "STRIPE_API_SECRET": "my_stripe_api_key",
     "STRIPE_WEBHOOK_SECRET": "my_stripe_webhook_key",
     "FRONT_END_BASE_URL": "http://localhost:3000",
-    "NEW_USER_FREE_TRIAL_DAYS": 15,
+    "NEW_USER_FREE_TRIAL_DAYS": None,
     "CHECKOUT_SUCCESS_URL_PATH": "payment",
     "CHECKOUT_CANCEL_URL_PATH": "manage-subscription",
     "DEFAULT_PAYMENT_METHOD_TYPES": ["card"],
     "DEFAULT_CHECKOUT_MODE": "subscription",
     "DEFAULT_DISCOUNTS": None,
     "ALLOW_PROMOTION_CODES": True,
+    "DJANGO_USER_EMAIL_FIELD": "email",  # used to match Stripe customer email
+    "USER_CREATE_DEFAULTS_ATTRIBUTE_MAP": {  # attributes to copy from Stripe customer when creating new Django user
+        "username": "email"
+    }
 }
 
 
 class DrfStripeSettings:
     def __init__(self, user_settings=None, defaults=None):
         self._user_settings = user_settings or {}
         self.defaults = defaults or DEFAULTS
@@ -53,14 +57,13 @@
             delattr(self, "_user_settings")
 
 
 drf_stripe_settings = DrfStripeSettings(USER_SETTINGS, DEFAULTS)
 
 
 def reload_drf_stripe_settings(*args, **kwargs):
-    print("Reloading drf_stripe settings")
     setting = kwargs["setting"]
     if setting == "DRF_STRIPE":
         drf_stripe_settings.reload()
 
 
 setting_changed.connect(reload_drf_stripe_settings)
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/checkout.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/checkout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import timedelta, datetime
 from functools import reduce
-from typing import overload, List
+from typing import overload, List, Union
 from urllib.parse import urljoin
 
 from django.contrib.auth import get_user_model
 from django.utils import timezone
 
 from drf_stripe.stripe_api.api import stripe_api as stripe
 from ..settings import drf_stripe_settings
@@ -76,16 +76,16 @@
         customer_id=user_instance.stripe_user.customer_id,
         **kwargs
     )
 
 
 def _make_stripe_checkout_params(
         customer_id: str, price_id: str = None, quantity: int = 1, line_items: List[dict] = None,
-        trial_end: datetime = None, discounts: List[dict] = None,
-        payment_method_types=None, checkout_mode=drf_stripe_settings.DEFAULT_CHECKOUT_MODE
+        trial_end: Union[str, datetime, None] = 'auto', discounts: List[dict] = None,
+        payment_method_types: List[str] = None, checkout_mode: str = drf_stripe_settings.DEFAULT_CHECKOUT_MODE
 ):
     if price_id is None and line_items is None:
         raise ValueError("Invalid arguments: must provide either a 'price_id' or 'line_items'.")
     elif price_id is not None and line_items is not None:
         raise ValueError("Invalid arguments: 'price_id' and 'line_items' should be used at the same time.")
 
     if price_id is not None:
@@ -97,44 +97,53 @@
     success_url = reduce(urljoin, (drf_stripe_settings.FRONT_END_BASE_URL,
                                    drf_stripe_settings.CHECKOUT_SUCCESS_URL_PATH,
                                    "?session={CHECKOUT_SESSION_ID}"))
 
     cancel_url = reduce(urljoin, (drf_stripe_settings.FRONT_END_BASE_URL,
                                   drf_stripe_settings.CHECKOUT_CANCEL_URL_PATH))
 
-    ret = {
+    params = {
         "customer": customer_id,
         "success_url": success_url,
         "cancel_url": cancel_url,
         "payment_method_types": payment_method_types,
         "mode": checkout_mode,
         "line_items": line_items,
         "subscription_data": {
-            "trial_end": int(_make_trial_end_datetime(trial_end=trial_end).timestamp())
+            "trial_end": _make_trial_end_timestamp(trial_end=trial_end)
         }
     }
-    
+
     allow_promotion_codes = drf_stripe_settings.ALLOW_PROMOTION_CODES
-    
+
     if allow_promotion_codes:
-        ret.update({"allow_promotion_codes": allow_promotion_codes})
+        params.update({"allow_promotion_codes": allow_promotion_codes})
     else:
-        ret.update({"discounts": discounts if discounts else drf_stripe_settings.DEFAULT_DISCOUNTS})
-    
-    return ret
+        params.update({"discounts": discounts if discounts else drf_stripe_settings.DEFAULT_DISCOUNTS})
 
+    return params
 
-def _make_trial_end_datetime(trial_end=None):
+
+def _make_trial_end_timestamp(trial_end: Union[str, None, datetime] = 'auto'):
     """
     Returns a new trial_end time to be used for setting up new Stripe Subscription.
     Stripe requires new Subscription trial_end to be at least 48 hours in the future.
-    Return None if less than 48 hours left to set up trialing with Stripe
 
+    :param trial_end: Explicitly set trial end datetime.
+        Defaults to 'auto', which will return a calculated trial_end based on NEW_USER_FREE_TRIAL_DAYS setting.
+        If set to less than 48 hours from now, will return the minimum required trial_end acceptable to Stripe API.
+        If set to None, no trial, returns None.
     """
     if trial_end is None:
-        trial_end = timezone.now() + timezone.timedelta(days=drf_stripe_settings.NEW_USER_FREE_TRIAL_DAYS)
+        return
+
+    if trial_end == 'auto':
+        if drf_stripe_settings.NEW_USER_FREE_TRIAL_DAYS is None:
+            return
+        else:
+            trial_end = timezone.now() + timezone.timedelta(days=drf_stripe_settings.NEW_USER_FREE_TRIAL_DAYS + 1)
 
     min_trial_end = timezone.now() + timedelta(hours=49)
     if trial_end < min_trial_end:
         trial_end = min_trial_end
 
-    return trial_end.replace(microsecond=0)
+    return int(trial_end.replace(microsecond=0).timestamp())
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/customer_portal.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/customer_portal.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/products.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/products.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_api/subscriptions.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_api/subscriptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Literal, List
 
 from django.db.models import Q
 from django.db.models import QuerySet
 from django.db.transaction import atomic
 
 from drf_stripe.stripe_api.api import stripe_api as stripe
-from .customers import get_or_create_stripe_user
+from .customers import get_or_create_stripe_user, CreatingNewUsersDisabledError
 from ..models import Subscription, Price, SubscriptionItem
 from ..stripe_models.subscription import ACCESS_GRANTING_STATUSES, StripeSubscriptions
 
 """
 status argument, see https://stripe.com/docs/api/subscriptions/list?lang=python#list_subscriptions-status
 """
 STATUS_ARG = Literal[
@@ -25,22 +25,25 @@
     "all",
     "ended"
 ]
 
 
 @atomic
 def stripe_api_update_subscriptions(status: STATUS_ARG = None, limit: int = 100, starting_after: str = None,
-                                    test_data=None):
+                                    test_data=None, ignore_new_user_creation_errors = False):
     """
     Retrieve all subscriptions. Updates database.
 
+    Called from management command.
+
     :param STATUS_ARG status: subscription status to retrieve.
     :param int limit: number of instances to retrieve( between 0 and 100).
     :param str starting_after: subscription id to start retrieving.
     :param test_data: response data from Stripe API stripe.Subscription.list, used for testing
+    :param ignore_new_user_creation_errors: if True, CreatingNewUsersDisabledError thrown by get_or_create_stripe_user() will be skipped
     """
 
     if limit < 0 or limit > 100:
         raise ValueError("Argument limit should be a positive integer no greater than 100.")
 
     if test_data is None:
         subscriptions_response = stripe.Subscription.list(status=status, limit=limit, starting_after=starting_after)
@@ -48,34 +51,40 @@
         subscriptions_response = test_data
 
     stripe_subscriptions = StripeSubscriptions(**subscriptions_response).data
 
     creation_count = 0
 
     for subscription in stripe_subscriptions:
-        stripe_user = get_or_create_stripe_user(customer_id=subscription.customer)
+        try:
+            stripe_user = get_or_create_stripe_user(customer_id=subscription.customer)
 
-        _, created = Subscription.objects.update_or_create(
-            subscription_id=subscription.id,
-            defaults={
-                "stripe_user": stripe_user,
-                "period_start": subscription.current_period_start,
-                "period_end": subscription.current_period_end,
-                "cancel_at": subscription.cancel_at,
-                "cancel_at_period_end": subscription.cancel_at_period_end,
-                "ended_at": subscription.ended_at,
-                "status": subscription.status,
-                "trial_end": subscription.trial_end,
-                "trial_start": subscription.trial_start
-            }
-        )
-        print(f"Updated subscription {subscription.id}")
-        _update_subscription_items(subscription.id, subscription.items.data)
-        if created is True:
-            creation_count += 1
+            _, created = Subscription.objects.update_or_create(
+                subscription_id=subscription.id,
+                defaults={
+                    "stripe_user": stripe_user,
+                    "period_start": subscription.current_period_start,
+                    "period_end": subscription.current_period_end,
+                    "cancel_at": subscription.cancel_at,
+                    "cancel_at_period_end": subscription.cancel_at_period_end,
+                    "ended_at": subscription.ended_at,
+                    "status": subscription.status,
+                    "trial_end": subscription.trial_end,
+                    "trial_start": subscription.trial_start
+                }
+            )
+            print(f"Updated subscription {subscription.id}")
+            _update_subscription_items(subscription.id, subscription.items.data)
+            if created is True:
+                creation_count += 1
+        except CreatingNewUsersDisabledError as e:
+            if not ignore_new_user_creation_errors:
+                raise e
+            else:
+                print(f"User for customer id '{subscription.customer}' with subscription '{subscription.id}' does not exist, skipping.")
 
     print(f"Created {creation_count} new Subscriptions.")
 
 
 def _update_subscription_items(subscription_id, items_data):
     SubscriptionItem.objects.filter(subscription=subscription_id).delete()
     for item in items_data:
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/currency.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/currency.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/customer.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/customer.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/event.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Based on https://stripe.com/docs/api/events/object
     This is the base event template for more specific Stripe event classes
     """
     id: str
     api_version: str
     request: StripeEventRequest
     data: Any  # overwrite this attribute when inheriting
-    type: Literal[str]  # overwrite this attribute when inheriting
+    type: Literal[Any]  # overwrite this attribute when inheriting
 
 
 class StripeInvoiceEvent(StripeBaseEvent):
     data: StripeInvoiceEventData
     type: Literal[
         EventType.INVOICE_PAID,
         EventType.INVOICE_CREATED,
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/invoice.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,14 @@
     auto_advance: Optional[bool]
     charge: str = None
     collection_method: Optional[str]
     currency: str
     customer: str
     description: str = None
     hosted_invoice_url: Optional[str]
-    lines: Optional[List[StripeInvoiceLines]]
+    lines: Optional[StripeInvoiceLines]
 
 
 class StripeInvoiceEventData(BaseModel):
     """Based on https://stripe.com/docs/api/events/object#event_object-data"""
     object: StripeInvoice
     previous_attributes: Optional[StripeInvoice]
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/price.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/price.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/product.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/product.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_models/subscription.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_models/subscription.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from enum import Enum
-from typing import List, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel
 
 from .price import StripePrice
 
 
 class StripeSubscriptionStatus(str, Enum):
@@ -57,15 +57,15 @@
     current_period_start: Optional[datetime]
     customer: Optional[str]
     default_payment_method: str = None
     items: Optional[StripeSubscriptionItems]
     latest_invoice: Optional[str]
     metadata: Optional[Dict]
     pending_setup_intent: str = None
-    pending_update: str = None
+    pending_update: Any = None
     status: Optional[StripeSubscriptionStatus]
 
 
 class StripeSubscriptions(BaseModel):
     """Based on https://stripe.com/docs/api/subscriptions/list"""
     data: List[StripeSubscription]
     has_more: bool = None
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/customer_subscription.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/customer_subscription.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/handler.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     ignores the error if it is caused by unimplemented event.type;
     Otherwise, raise the error.
     """
     event_type_error = False
 
     for error in err.errors():
         error_loc = error['loc']
-        if error_loc[0] == 'event' and error_loc[1] == 'type':
+        if error_loc[0] == 'event' and error.get('ctx', {}).get('discriminator_key', {}) == 'type':
             event_type_error = True
             break
 
     if event_type_error is False:
         raise err
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/price.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/price.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/stripe_webhooks/product.py` & `drf-stripe-subscription-1.2.0/drf_stripe/stripe_webhooks/product.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe/views.py` & `drf-stripe-subscription-1.2.0/drf_stripe/views.py`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe_subscription.egg-info/PKG-INFO` & `drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-stripe-subscription
-Version: 1.1.9
+Version: 1.2.0
 Summary: A Django app that provides subscription features with Stripe and REST endpoints.
 Home-page: https://github.com/oscarychen/drf-stripe-subscription
 Author: Oscar Chen
 Author-email: quacky@duck.com
 License: MIT
 Description: # drf-stripe-subscription
         
@@ -283,21 +283,41 @@
         Pulls customers from Stripe and updates Django database.
         
         ```commandline
         python manage.py update_stripe_subscriptions
         ```
         
         Pulls subscriptions from Stripe and updates Django database.
+        
+        ## Working with customized Django User models
+        
+        The following DRF_STRIPE settings can be used to customize how Django creates User instance using Stripe Customer
+        attributes (default values shown):
+        
+        ```python
+        DRF_STRIPE = {
+            "DJANGO_USER_EMAIL_FIELD": "email",
+            "USER_CREATE_DEFAULTS_ATTRIBUTE_MAP": {"username": "email"},
+        }
+        ```
+        
+        The `DJANGO_USER_EMAIL_FIELD` specifies name of the Django User attribute to be used to store Stripe Customer email. It
+        will be used to look up existing Django User using Stripe Customer email.
+        
+        The `USER_CREATE_DEFAULTS_ATTRIBUTE_MAP` maps the name of Django User attribute to name of corresponding Stripe Customer
+        attribute, and is used during the automated Django User instance creation.
+        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `drf-stripe-subscription-1.1.9/drf_stripe_subscription.egg-info/SOURCES.txt` & `drf-stripe-subscription-1.2.0/drf_stripe_subscription.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-stripe-subscription-1.1.9/setup.cfg` & `drf-stripe-subscription-1.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [metadata]
 name = drf-stripe-subscription
-version = 1.1.9
+version = 1.2.0
 description = A Django app that provides subscription features with Stripe and REST endpoints.
 long_description = file: README.md
 url = https://github.com/oscarychen/drf-stripe-subscription
 author = Oscar Chen
 author_email = quacky@duck.com
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.0
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
@@ -30,12 +31,14 @@
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	Django >= 3.0
 	djangorestframework >= 3.0
+	pydantic >= 1.8
+	stripe >= 2.63
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

