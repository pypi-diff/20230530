# Comparing `tmp/klaviyo-api-2.0.0.tar.gz` & `tmp/klaviyo-api-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klaviyo-api-2.0.0.tar", last modified: Wed Apr  5 22:13:49 2023, max compression
+gzip compressed data, was "klaviyo-api-2.0.1.tar", last modified: Tue May 30 20:18:45 2023, max compression
```

## Comparing `klaviyo-api-2.0.0.tar` & `klaviyo-api-2.0.1.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-05 22:13:49.160639 klaviyo-api-2.0.0/
--rw-r--r--   0 local      (503) staff       (20)     1063 2023-04-05 22:13:38.000000 klaviyo-api-2.0.0/LICENSE
--rw-r--r--   0 local      (503) staff       (20)    53409 2023-04-05 22:13:49.160875 klaviyo-api-2.0.0/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)    52892 2023-04-05 22:13:38.000000 klaviyo-api-2.0.0/README.md
--rw-r--r--   0 local      (503) staff       (20)      103 2023-04-05 22:13:38.000000 klaviyo-api-2.0.0/pyproject.toml
--rw-r--r--   0 local      (503) staff       (20)      801 2023-04-05 22:13:49.161617 klaviyo-api-2.0.0/setup.cfg
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-05 22:13:48.883114 klaviyo-api-2.0.0/src/
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-05 22:13:48.890541 klaviyo-api-2.0.0/src/klaviyo_api/
--rw-r--r--   0 local      (503) staff       (20)      130 2023-04-05 22:13:38.000000 klaviyo-api-2.0.0/src/klaviyo_api/__init__.py
--rw-r--r--   0 local      (503) staff       (20)      501 2023-04-05 22:13:38.000000 klaviyo-api-2.0.0/src/klaviyo_api/custom_retry.py
--rw-r--r--   0 local      (503) staff       (20)    25887 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/klaviyo_api/wrapper.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-05 22:13:48.893983 klaviyo-api-2.0.0/src/klaviyo_api.egg-info/
--rw-r--r--   0 local      (503) staff       (20)    53409 2023-04-05 22:13:48.000000 klaviyo-api-2.0.0/src/klaviyo_api.egg-info/PKG-INFO
--rw-r--r--   0 local      (503) staff       (20)    16572 2023-04-05 22:13:48.000000 klaviyo-api-2.0.0/src/klaviyo_api.egg-info/SOURCES.txt
--rw-r--r--   0 local      (503) staff       (20)        1 2023-04-05 22:13:48.000000 klaviyo-api-2.0.0/src/klaviyo_api.egg-info/dependency_links.txt
--rw-r--r--   0 local      (503) staff       (20)      119 2023-04-05 22:13:48.000000 klaviyo-api-2.0.0/src/klaviyo_api.egg-info/requires.txt
--rw-r--r--   0 local      (503) staff       (20)       27 2023-04-05 22:13:48.000000 klaviyo-api-2.0.0/src/klaviyo_api.egg-info/top_level.txt
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-05 22:13:48.899325 klaviyo-api-2.0.0/src/openapi_client/
--rw-r--r--   0 local      (503) staff       (20)      788 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/__init__.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-05 22:13:48.912398 klaviyo-api-2.0.0/src/openapi_client/api/
--rw-r--r--   0 local      (503) staff       (20)      220 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/api/__init__.py
--rw-r--r--   0 local      (503) staff       (20)   108410 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/campaigns_api.py
--rw-r--r--   0 local      (503) staff       (20)   351426 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/catalogs_api.py
--rw-r--r--   0 local      (503) staff       (20)    19405 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/client_api.py
--rw-r--r--   0 local      (503) staff       (20)     7236 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/data_privacy_api.py
--rw-r--r--   0 local      (503) staff       (20)    58131 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/events_api.py
--rw-r--r--   0 local      (503) staff       (20)   106404 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/flows_api.py
--rw-r--r--   0 local      (503) staff       (20)    70579 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/lists_api.py
--rw-r--r--   0 local      (503) staff       (20)    21644 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/metrics_api.py
--rw-r--r--   0 local      (503) staff       (20)    87637 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/profiles_api.py
--rw-r--r--   0 local      (503) staff       (20)    48387 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/segments_api.py
--rw-r--r--   0 local      (503) staff       (20)   147862 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/tags_api.py
--rw-r--r--   0 local      (503) staff       (20)    42674 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/api/templates_api.py
--rw-r--r--   0 local      (503) staff       (20)    39451 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/api_client.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-05 22:13:48.913195 klaviyo-api-2.0.0/src/openapi_client/apis/
--rw-r--r--   0 local      (503) staff       (20)     1084 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/apis/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    17158 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/configuration.py
--rw-r--r--   0 local      (503) staff       (20)     5120 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/exceptions.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-05 22:13:49.158811 klaviyo-api-2.0.0/src/openapi_client/model/
--rw-r--r--   0 local      (503) staff       (20)      348 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/model/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    11834 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/audiences_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    11849 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_clone_query.py
--rw-r--r--   0 local      (503) staff       (20)    12354 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_clone_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11954 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12364 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13914 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11633 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12011 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_assign_template_query.py
--rw-r--r--   0 local      (503) staff       (20)    12566 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12055 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12001 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12786 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12109 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11930 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12667 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13373 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11942 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12082 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12744 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11768 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11999 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11931 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12487 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11675 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11762 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12002 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12848 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11850 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_bulk_update_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12022 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12671 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12179 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11930 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    13136 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13243 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12022 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_delete_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12671 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12179 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12422 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_delete_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12114 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_item_op.py
--rw-r--r--   0 local      (503) staff       (20)    12022 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12671 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12179 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11930 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    13736 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11663 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12102 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py
--rw-r--r--   0 local      (503) staff       (20)    12225 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py
--rw-r--r--   0 local      (503) staff       (20)    12137 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11921 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11921 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11921 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_bulk_update_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12121 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_category_op.py
--rw-r--r--   0 local      (503) staff       (20)    11982 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12603 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12074 2023-04-05 22:13:34.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11890 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    13040 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    17029 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12122 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py
--rw-r--r--   0 local      (503) staff       (20)    12235 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py
--rw-r--r--   0 local      (503) staff       (20)    12172 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11982 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_delete_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12603 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12074 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12374 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_delete_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11690 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11982 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12603 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12074 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11890 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    13632 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    15281 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12792 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_job_error_payload.py
--rw-r--r--   0 local      (503) staff       (20)    11966 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11966 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11966 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12012 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12654 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12143 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    13119 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    19026 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12012 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12654 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12143 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12410 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_delete_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11735 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12012 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12654 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12143 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    13066 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    17148 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12224 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/collection_links.py
--rw-r--r--   0 local      (503) staff       (20)    13057 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/content_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    12002 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query.py
--rw-r--r--   0 local      (503) staff       (20)    12608 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12449 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11879 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/data_privacy_deletion_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11685 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/email_channel.py
--rw-r--r--   0 local      (503) staff       (20)    14791 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/email_marketing.py
--rw-r--r--   0 local      (503) staff       (20)    12468 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/email_marketing_list_suppression.py
--rw-r--r--   0 local      (503) staff       (20)    12135 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/email_marketing_suppression.py
--rw-r--r--   0 local      (503) staff       (20)    12321 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/email_message_content.py
--rw-r--r--   0 local      (503) staff       (20)    12694 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/email_tracking_options.py
--rw-r--r--   0 local      (503) staff       (20)    11790 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/error_source.py
--rw-r--r--   0 local      (503) staff       (20)    11829 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/event_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12313 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/event_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    17076 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/event_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11588 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/event_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11675 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/flow_action_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11573 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/flow_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11690 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/flow_message_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11819 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/flow_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12538 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/flow_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11764 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/flow_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11999 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response.py
--rw-r--r--   0 local      (503) staff       (20)    12816 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11775 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py
--rw-r--r--   0 local      (503) staff       (20)    11819 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/list_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12296 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/list_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11668 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/list_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11573 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/list_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11831 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/list_members_add_query.py
--rw-r--r--   0 local      (503) staff       (20)    11980 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/list_members_add_query_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11840 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/list_members_delete_query.py
--rw-r--r--   0 local      (503) staff       (20)    11890 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/list_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12625 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/list_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11750 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11869 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_query.py
--rw-r--r--   0 local      (503) staff       (20)    12424 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    21013 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12259 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_row_dto.py
--rw-r--r--   0 local      (503) staff       (20)    11996 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/metric_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    11603 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/metric_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11495 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/object_links.py
--rw-r--r--   0 local      (503) staff       (20)    11910 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12758 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    15425 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11894 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_meta.py
--rw-r--r--   0 local      (503) staff       (20)    13575 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_meta_identifiers.py
--rw-r--r--   0 local      (503) staff       (20)    11960 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/onsite_subscription_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12493 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/onsite_subscription_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    13508 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    14569 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/predictive_analytics.py
--rw-r--r--   0 local      (503) staff       (20)    11765 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_aggregate_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11849 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12347 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    15156 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11618 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_enum.py
--rw-r--r--   0 local      (503) staff       (20)    13961 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_location.py
--rw-r--r--   0 local      (503) staff       (20)    11301 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_location_latitude.py
--rw-r--r--   0 local      (503) staff       (20)    11304 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_location_longitude.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12725 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12041 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12026 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12071 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12056 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11618 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/segment_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11920 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/segment_partial_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12586 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/segment_partial_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11632 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11956 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/send_options.py
--rw-r--r--   0 local      (503) staff       (20)    11612 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/send_options_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    13115 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/send_strategy_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    12019 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/send_time_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    11665 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/sms_channel.py
--rw-r--r--   0 local      (503) staff       (20)    12982 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/sms_marketing.py
--rw-r--r--   0 local      (503) staff       (20)    11704 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/sms_message_content.py
--rw-r--r--   0 local      (503) staff       (20)    12566 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/sms_render_options.py
--rw-r--r--   0 local      (503) staff       (20)    12005 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/sms_tracking_options.py
--rw-r--r--   0 local      (503) staff       (20)    12702 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/static_schedule_options.py
--rw-r--r--   0 local      (503) staff       (20)    11547 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/sto_schedule_options.py
--rw-r--r--   0 local      (503) staff       (20)    12979 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/subscription.py
--rw-r--r--   0 local      (503) staff       (20)    12200 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/subscription_channels.py
--rw-r--r--   0 local      (503) staff       (20)    11991 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/subscription_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12668 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12750 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11693 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/subscription_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11949 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/subscriptions.py
--rw-r--r--   0 local      (503) staff       (20)    11598 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/suppression.py
--rw-r--r--   0 local      (503) staff       (20)    11981 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/suppression_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12651 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11983 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11770 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_campaign_op.py
--rw-r--r--   0 local      (503) staff       (20)    11970 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_campaign_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11809 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12279 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12174 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11558 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11730 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_flow_op.py
--rw-r--r--   0 local      (503) staff       (20)    11926 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_flow_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11860 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_group_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12366 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_group_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11858 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11645 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_group_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11860 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_group_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12568 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_group_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11881 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11730 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_list_op.py
--rw-r--r--   0 local      (503) staff       (20)    11926 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_list_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11760 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_segment_op.py
--rw-r--r--   0 local      (503) staff       (20)    11959 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_segment_op_data_inner.py
--rw-r--r--   0 local      (503) staff       (20)    11809 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12469 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11625 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/tag_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11849 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_clone_query.py
--rw-r--r--   0 local      (503) staff       (20)    12354 2023-04-05 22:13:35.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_clone_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12223 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_clone_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12364 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12887 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11633 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_render_query.py
--rw-r--r--   0 local      (503) staff       (20)    12364 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_render_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12898 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_render_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11859 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_update_query.py
--rw-r--r--   0 local      (503) staff       (20)    12570 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_update_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12475 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/template_update_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11879 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/test_api_analytics_sample_enum.py
--rw-r--r--   0 local      (503) staff       (20)    11645 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/test_list_enum.py
--rw-r--r--   0 local      (503) staff       (20)    12184 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/throttled_schedule_options.py
--rw-r--r--   0 local      (503) staff       (20)    13204 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/tracking_options_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    12011 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/unsubscription_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12702 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    12305 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    12001 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/unsuppression_create_job_create_query.py
--rw-r--r--   0 local      (503) staff       (20)    12685 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py
--rw-r--r--   0 local      (503) staff       (20)    11989 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py
--rw-r--r--   0 local      (503) staff       (20)    11689 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/utm_param_info.py
--rw-r--r--   0 local      (503) staff       (20)    11845 2023-04-05 22:13:36.000000 klaviyo-api-2.0.0/src/openapi_client/model/utm_params_sub_object.py
--rw-r--r--   0 local      (503) staff       (20)    82630 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/model_utils.py
-drwxr-xr-x   0 local      (503) staff       (20)        0 2023-04-05 22:13:49.159579 klaviyo-api-2.0.0/src/openapi_client/models/
--rw-r--r--   0 local      (503) staff       (20)    24813 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/models/__init__.py
--rw-r--r--   0 local      (503) staff       (20)    14324 2023-04-05 22:13:37.000000 klaviyo-api-2.0.0/src/openapi_client/rest.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.932567 klaviyo-api-2.0.1/
+-rw-r--r--   0 local      (503) staff       (20)     1063 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/LICENSE
+-rw-r--r--   0 local      (503) staff       (20)    53409 2023-05-30 20:18:45.932790 klaviyo-api-2.0.1/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)    52892 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/README.md
+-rw-r--r--   0 local      (503) staff       (20)      103 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/pyproject.toml
+-rw-r--r--   0 local      (503) staff       (20)      801 2023-05-30 20:18:45.933422 klaviyo-api-2.0.1/setup.cfg
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.740355 klaviyo-api-2.0.1/src/
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.744953 klaviyo-api-2.0.1/src/klaviyo_api/
+-rw-r--r--   0 local      (503) staff       (20)      130 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/src/klaviyo_api/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)      501 2023-05-30 20:18:37.000000 klaviyo-api-2.0.1/src/klaviyo_api/custom_retry.py
+-rw-r--r--   0 local      (503) staff       (20)    25983 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/klaviyo_api/wrapper.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.747154 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/
+-rw-r--r--   0 local      (503) staff       (20)    53409 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/PKG-INFO
+-rw-r--r--   0 local      (503) staff       (20)    16572 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/SOURCES.txt
+-rw-r--r--   0 local      (503) staff       (20)        1 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/dependency_links.txt
+-rw-r--r--   0 local      (503) staff       (20)      119 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/requires.txt
+-rw-r--r--   0 local      (503) staff       (20)       27 2023-05-30 20:18:45.000000 klaviyo-api-2.0.1/src/klaviyo_api.egg-info/top_level.txt
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.750729 klaviyo-api-2.0.1/src/openapi_client/
+-rw-r--r--   0 local      (503) staff       (20)      788 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/__init__.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.759585 klaviyo-api-2.0.1/src/openapi_client/api/
+-rw-r--r--   0 local      (503) staff       (20)      220 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/api/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)   108410 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/campaigns_api.py
+-rw-r--r--   0 local      (503) staff       (20)   351426 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/catalogs_api.py
+-rw-r--r--   0 local      (503) staff       (20)    19405 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/client_api.py
+-rw-r--r--   0 local      (503) staff       (20)     7236 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/data_privacy_api.py
+-rw-r--r--   0 local      (503) staff       (20)    58131 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/events_api.py
+-rw-r--r--   0 local      (503) staff       (20)   106404 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/flows_api.py
+-rw-r--r--   0 local      (503) staff       (20)    70579 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/lists_api.py
+-rw-r--r--   0 local      (503) staff       (20)    21644 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/metrics_api.py
+-rw-r--r--   0 local      (503) staff       (20)    87637 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/profiles_api.py
+-rw-r--r--   0 local      (503) staff       (20)    48387 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/segments_api.py
+-rw-r--r--   0 local      (503) staff       (20)   147862 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/tags_api.py
+-rw-r--r--   0 local      (503) staff       (20)    42674 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/api/templates_api.py
+-rw-r--r--   0 local      (503) staff       (20)    39451 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/api_client.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.760182 klaviyo-api-2.0.1/src/openapi_client/apis/
+-rw-r--r--   0 local      (503) staff       (20)     1084 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/apis/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)    17158 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/configuration.py
+-rw-r--r--   0 local      (503) staff       (20)     5120 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/exceptions.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.931737 klaviyo-api-2.0.1/src/openapi_client/model/
+-rw-r--r--   0 local      (503) staff       (20)      348 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/model/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)    11834 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/audiences_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11849 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12354 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11954 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11859 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12364 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13914 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11633 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12011 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12566 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12055 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11750 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12001 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12786 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12109 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11930 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12667 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13373 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11942 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12082 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12744 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11768 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11999 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11931 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12487 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11675 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11762 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12002 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12848 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11850 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11981 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11981 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11981 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_update_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12022 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12671 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12179 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11930 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13136 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13243 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12022 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12671 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12179 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12422 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11750 2023-05-30 20:18:33.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12114 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_item_op.py
+-rw-r--r--   0 local      (503) staff       (20)    12022 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12671 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12179 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11930 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13736 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11663 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12102 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)    12225 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py
+-rw-r--r--   0 local      (503) staff       (20)    12137 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11921 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11921 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11921 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_update_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12121 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_category_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11982 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12603 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12074 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11890 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13040 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    17029 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12122 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py
+-rw-r--r--   0 local      (503) staff       (20)    12235 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py
+-rw-r--r--   0 local      (503) staff       (20)    12172 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11982 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12603 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12074 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12374 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11690 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11982 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12603 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12074 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11890 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13632 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    15281 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12792 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_job_error_payload.py
+-rw-r--r--   0 local      (503) staff       (20)    11966 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11966 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11966 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12012 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12654 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12143 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11920 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13119 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    19026 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12012 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12654 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12143 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12410 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11735 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12012 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12654 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12143 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11920 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    13066 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    17148 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12224 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/collection_links.py
+-rw-r--r--   0 local      (503) staff       (20)    13057 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/content_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12002 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12608 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12449 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11879 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_deletion_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11685 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_channel.py
+-rw-r--r--   0 local      (503) staff       (20)    14791 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_marketing.py
+-rw-r--r--   0 local      (503) staff       (20)    12468 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_marketing_list_suppression.py
+-rw-r--r--   0 local      (503) staff       (20)    12135 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_marketing_suppression.py
+-rw-r--r--   0 local      (503) staff       (20)    12321 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_message_content.py
+-rw-r--r--   0 local      (503) staff       (20)    12694 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/email_tracking_options.py
+-rw-r--r--   0 local      (503) staff       (20)    11790 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/error_source.py
+-rw-r--r--   0 local      (503) staff       (20)    11829 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/event_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12313 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/event_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    17076 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/event_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11588 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/event_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11675 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_action_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11573 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11690 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_message_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11819 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12538 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11764 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11999 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response.py
+-rw-r--r--   0 local      (503) staff       (20)    12816 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11775 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py
+-rw-r--r--   0 local      (503) staff       (20)    11819 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12296 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11668 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11573 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11831 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_members_add_query.py
+-rw-r--r--   0 local      (503) staff       (20)    11980 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_members_add_query_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11840 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_members_delete_query.py
+-rw-r--r--   0 local      (503) staff       (20)    11890 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12625 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/list_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11750 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11869 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12424 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    21013 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12259 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_row_dto.py
+-rw-r--r--   0 local      (503) staff       (20)    11996 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    11603 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/metric_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11495 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/object_links.py
+-rw-r--r--   0 local      (503) staff       (20)    11910 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12758 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    15425 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11894 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_meta.py
+-rw-r--r--   0 local      (503) staff       (20)    13575 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_meta_identifiers.py
+-rw-r--r--   0 local      (503) staff       (20)    11960 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12493 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13508 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    14569 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/predictive_analytics.py
+-rw-r--r--   0 local      (503) staff       (20)    11765 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_aggregate_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11849 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12347 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    15156 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11618 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    13961 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_location.py
+-rw-r--r--   0 local      (503) staff       (20)    11301 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_location_latitude.py
+-rw-r--r--   0 local      (503) staff       (20)    11304 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_location_longitude.py
+-rw-r--r--   0 local      (503) staff       (20)    11920 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12725 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12041 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12026 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12071 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12056 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11618 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/segment_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11920 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12586 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11632 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11956 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/send_options.py
+-rw-r--r--   0 local      (503) staff       (20)    11612 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/send_options_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    13115 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/send_strategy_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12019 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/send_time_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11665 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_channel.py
+-rw-r--r--   0 local      (503) staff       (20)    12982 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_marketing.py
+-rw-r--r--   0 local      (503) staff       (20)    11704 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_message_content.py
+-rw-r--r--   0 local      (503) staff       (20)    12566 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_render_options.py
+-rw-r--r--   0 local      (503) staff       (20)    12005 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sms_tracking_options.py
+-rw-r--r--   0 local      (503) staff       (20)    12702 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/static_schedule_options.py
+-rw-r--r--   0 local      (503) staff       (20)    11547 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/sto_schedule_options.py
+-rw-r--r--   0 local      (503) staff       (20)    12979 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription.py
+-rw-r--r--   0 local      (503) staff       (20)    12200 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_channels.py
+-rw-r--r--   0 local      (503) staff       (20)    11991 2023-05-30 20:18:34.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12668 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12750 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11693 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscription_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11949 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/subscriptions.py
+-rw-r--r--   0 local      (503) staff       (20)    11598 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/suppression.py
+-rw-r--r--   0 local      (503) staff       (20)    11981 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12651 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11983 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11770 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_campaign_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11970 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_campaign_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11809 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12279 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12174 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11558 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11730 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_flow_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11926 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_flow_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11860 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12366 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11858 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11645 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11860 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12568 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11881 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11730 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_list_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11926 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_list_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11760 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_segment_op.py
+-rw-r--r--   0 local      (503) staff       (20)    11959 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_segment_op_data_inner.py
+-rw-r--r--   0 local      (503) staff       (20)    11809 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12469 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11625 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tag_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11849 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_clone_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12354 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_clone_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12223 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_clone_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11859 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12364 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12887 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11633 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11859 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_render_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12364 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_render_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12898 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_render_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11859 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_update_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12570 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_update_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12475 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/template_update_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11879 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/test_api_analytics_sample_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    11645 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/test_list_enum.py
+-rw-r--r--   0 local      (503) staff       (20)    12184 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/throttled_schedule_options.py
+-rw-r--r--   0 local      (503) staff       (20)    13204 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/tracking_options_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12011 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsubscription_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12702 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    12305 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    12001 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsuppression_create_job_create_query.py
+-rw-r--r--   0 local      (503) staff       (20)    12685 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py
+-rw-r--r--   0 local      (503) staff       (20)    11989 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py
+-rw-r--r--   0 local      (503) staff       (20)    11689 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/utm_param_info.py
+-rw-r--r--   0 local      (503) staff       (20)    11845 2023-05-30 20:18:35.000000 klaviyo-api-2.0.1/src/openapi_client/model/utm_params_sub_object.py
+-rw-r--r--   0 local      (503) staff       (20)    82630 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/model_utils.py
+drwxr-xr-x   0 local      (503) staff       (20)        0 2023-05-30 20:18:45.932219 klaviyo-api-2.0.1/src/openapi_client/models/
+-rw-r--r--   0 local      (503) staff       (20)    24813 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/models/__init__.py
+-rw-r--r--   0 local      (503) staff       (20)    14324 2023-05-30 20:18:36.000000 klaviyo-api-2.0.1/src/openapi_client/rest.py
```

### Comparing `klaviyo-api-2.0.0/LICENSE` & `klaviyo-api-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/PKG-INFO` & `klaviyo-api-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: klaviyo-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: Klaviyo Python SDK
 Home-page: https://github.com/klaviyo/klaviyo-api-python
 Author: Klaviyo Developers
 Author-email: developers@klaviyo.com
 Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Klaviyo Python SDK
 
-- SDK version: 2.0.0
+- SDK version: 2.0.1
 - API revision: 2023-02-22
 
 ## Helpful Resources
 
 - [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference)
 - [API Guides](https://developers.klaviyo.com/en/v2023-02-22/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
```

### Comparing `klaviyo-api-2.0.0/README.md` & `klaviyo-api-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Klaviyo Python SDK
 
-- SDK version: 2.0.0
+- SDK version: 2.0.1
 - API revision: 2023-02-22
 
 ## Helpful Resources
 
 - [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference)
 - [API Guides](https://developers.klaviyo.com/en/v2023-02-22/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
```

### Comparing `klaviyo-api-2.0.0/setup.cfg` & `klaviyo-api-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = klaviyo-api
-version = 2.0.0
+version = 2.0.1
 author = Klaviyo Developers
 author_email = developers@klaviyo.com
 description = Klaviyo Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klaviyo/klaviyo-api-python
 project_urls =
```

### Comparing `klaviyo-api-2.0.0/src/klaviyo_api/wrapper.py` & `klaviyo-api-2.0.1/src/klaviyo_api/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,24 +28,26 @@
     api_key: str
     max_delay: int = 60
     max_retries: int = 3
     test_host: str = ''
 
     _REVISION = "2023-02-22"
 
+    _STATUS_CODE_CONNECTION_RESET_BY_PEER = 104
     _STATUS_CODE_TOO_MANY_REQUESTS = 429
     _STATUS_CODE_SERVICE_UNAVAILABLE = 503
     _STATUS_CODE_GATEWAY_TIMEOUT = 504
     _STATUS_CODE_A_TIMEOUT_OCCURED = 524
 
     _RETRY_CODES = {
+        _STATUS_CODE_CONNECTION_RESET_BY_PEER,
         _STATUS_CODE_TOO_MANY_REQUESTS,
         _STATUS_CODE_SERVICE_UNAVAILABLE,
         _STATUS_CODE_GATEWAY_TIMEOUT,
-        _STATUS_CODE_A_TIMEOUT_OCCURED
+        _STATUS_CODE_A_TIMEOUT_OCCURED,
         }
 
     _CURSOR_SEARCH_TOKENS = ['page%5Bcursor%5D','page[cursor]']
 
     def __post_init__(self):
 
         self.configuration = openapi_client.Configuration(
```

### Comparing `klaviyo-api-2.0.0/src/klaviyo_api.egg-info/PKG-INFO` & `klaviyo-api-2.0.1/src/klaviyo_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: klaviyo-api
-Version: 2.0.0
+Version: 2.0.1
 Summary: Klaviyo Python SDK
 Home-page: https://github.com/klaviyo/klaviyo-api-python
 Author: Klaviyo Developers
 Author-email: developers@klaviyo.com
 Project-URL: API Docs, https://developers.klaviyo.com/en/reference/api_overview
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Klaviyo Python SDK
 
-- SDK version: 2.0.0
+- SDK version: 2.0.1
 - API revision: 2023-02-22
 
 ## Helpful Resources
 
 - [API Reference](https://developers.klaviyo.com/en/v2023-02-22/reference)
 - [API Guides](https://developers.klaviyo.com/en/v2023-02-22/docs)
 - [Postman Workspace](https://www.postman.com/klaviyo/workspace/klaviyo-developers)
```

### Comparing `klaviyo-api-2.0.0/src/klaviyo_api.egg-info/SOURCES.txt` & `klaviyo-api-2.0.1/src/klaviyo_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/__init__.py` & `klaviyo-api-2.0.1/src/openapi_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 2023-02-22
     Contact: developers@klaviyo.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 # import ApiClient
 from openapi_client.api_client import ApiClient
 
 # import Configuration
 from openapi_client.configuration import Configuration
```

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/campaigns_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/campaigns_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/catalogs_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/catalogs_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/client_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/client_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/data_privacy_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/data_privacy_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/events_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/flows_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/flows_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/lists_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/lists_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/metrics_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/profiles_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/profiles_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/segments_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/segments_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/tags_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api/templates_api.py` & `klaviyo-api-2.0.1/src/openapi_client/api/templates_api.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/api_client.py` & `klaviyo-api-2.0.1/src/openapi_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'klaviyo-api-python/2.0.0'
+        self.user_agent = 'klaviyo-api-python/2.0.1'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `klaviyo-api-2.0.0/src/openapi_client/apis/__init__.py` & `klaviyo-api-2.0.1/src/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/configuration.py` & `klaviyo-api-2.0.1/src/openapi_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2023-02-22\n"\
-               "SDK Package Version: 2.0.0".\
+               "SDK Package Version: 2.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `klaviyo-api-2.0.0/src/openapi_client/exceptions.py` & `klaviyo-api-2.0.1/src/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/audiences_sub_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/audiences_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_clone_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_clone_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_clone_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_assign_template_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_assign_template_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_partial_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_message_partial_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_partial_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_partial_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_recipient_estimation_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_recipient_estimation_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_partial_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/campaign_send_job_partial_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_bulk_create_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_delete_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_bulk_update_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_bulk_update_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_delete_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_delete_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_delete_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_item_op.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_item_op.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_category_update_query_resource_object_relationships_items_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_bulk_create_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_delete_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_bulk_update_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_bulk_update_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_category_op.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_category_op.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_create_query_resource_object_relationships_categories_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_delete_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_delete_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_delete_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_item_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_job_error_payload.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_job_error_payload.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_delete_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_bulk_update_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_delete_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_delete_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/catalog_variant_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/collection_links.py` & `klaviyo-api-2.0.1/src/openapi_client/model/collection_links.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/content_sub_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/content_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_create_deletion_job_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/data_privacy_deletion_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/data_privacy_deletion_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/email_channel.py` & `klaviyo-api-2.0.1/src/openapi_client/model/email_channel.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/email_marketing.py` & `klaviyo-api-2.0.1/src/openapi_client/model/email_marketing.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/email_marketing_list_suppression.py` & `klaviyo-api-2.0.1/src/openapi_client/model/email_marketing_list_suppression.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/email_marketing_suppression.py` & `klaviyo-api-2.0.1/src/openapi_client/model/email_marketing_suppression.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/email_message_content.py` & `klaviyo-api-2.0.1/src/openapi_client/model/email_message_content.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/email_tracking_options.py` & `klaviyo-api-2.0.1/src/openapi_client/model/email_tracking_options.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/error_source.py` & `klaviyo-api-2.0.1/src/openapi_client/model/error_source.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/event_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/event_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/event_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/event_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/event_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/event_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/event_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/event_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/flow_action_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/flow_action_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/flow_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/flow_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/flow_message_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/flow_message_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/flow_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/flow_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/flow_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/flow_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response.py` & `klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py` & `klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py` & `klaviyo-api-2.0.1/src/openapi_client/model/get_create_variants_jobs5_xx_response_errors_inner_source.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/list_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/list_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/list_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/list_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/list_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/list_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/list_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/list_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/list_members_add_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/list_members_add_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/list_members_add_query_data_inner.py` & `klaviyo-api-2.0.1/src/openapi_client/model/list_members_add_query_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/list_members_delete_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/list_members_delete_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/list_partial_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/list_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/list_partial_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/list_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/metric_aggregate_row_dto.py` & `klaviyo-api-2.0.1/src/openapi_client/model/metric_aggregate_row_dto.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/metric_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/metric_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/metric_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/metric_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/object_links.py` & `klaviyo-api-2.0.1/src/openapi_client/model/object_links.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_meta.py` & `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_meta.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/onsite_profile_meta_identifiers.py` & `klaviyo-api-2.0.1/src/openapi_client/model/onsite_profile_meta_identifiers.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/onsite_subscription_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/onsite_subscription_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/onsite_subscription_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/predictive_analytics.py` & `klaviyo-api-2.0.1/src/openapi_client/model/predictive_analytics.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_aggregate_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_aggregate_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_location.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_location.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_location_latitude.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_location_latitude.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_location_longitude.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_location_longitude.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_partial_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_partial_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_subscription_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_suppression_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_unsubscription_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/profile_unsuppression_bulk_create_job_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/segment_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/segment_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/segment_partial_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/segment_partial_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/segment_partial_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/send_options.py` & `klaviyo-api-2.0.1/src/openapi_client/model/send_options.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/send_options_sub_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/send_options_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/send_strategy_sub_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/send_strategy_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/send_time_sub_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/send_time_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/sms_channel.py` & `klaviyo-api-2.0.1/src/openapi_client/model/sms_channel.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/sms_marketing.py` & `klaviyo-api-2.0.1/src/openapi_client/model/sms_marketing.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/sms_message_content.py` & `klaviyo-api-2.0.1/src/openapi_client/model/sms_message_content.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/sms_render_options.py` & `klaviyo-api-2.0.1/src/openapi_client/model/sms_render_options.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/sms_tracking_options.py` & `klaviyo-api-2.0.1/src/openapi_client/model/sms_tracking_options.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/static_schedule_options.py` & `klaviyo-api-2.0.1/src/openapi_client/model/static_schedule_options.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/sto_schedule_options.py` & `klaviyo-api-2.0.1/src/openapi_client/model/sto_schedule_options.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/subscription.py` & `klaviyo-api-2.0.1/src/openapi_client/model/subscription.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/subscription_channels.py` & `klaviyo-api-2.0.1/src/openapi_client/model/subscription_channels.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/subscription_create_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/subscription_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/subscription_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/subscription_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/subscriptions.py` & `klaviyo-api-2.0.1/src/openapi_client/model/subscriptions.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/suppression.py` & `klaviyo-api-2.0.1/src/openapi_client/model/suppression.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/suppression_create_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/suppression_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_campaign_op.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_campaign_op.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_campaign_op_data_inner.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_campaign_op_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_flow_op.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_flow_op.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_flow_op_data_inner.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_flow_op_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_group_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_group_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_group_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_group_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_group_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_group_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_list_op.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_list_op.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_list_op_data_inner.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_list_op_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_segment_op.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_segment_op.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_segment_op_data_inner.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_segment_op_data_inner.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tag_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tag_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_clone_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_clone_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_clone_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_clone_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_clone_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_clone_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_render_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_render_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_render_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_render_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_render_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_render_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_update_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_update_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_update_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_update_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/template_update_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/template_update_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/test_api_analytics_sample_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/test_api_analytics_sample_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/test_list_enum.py` & `klaviyo-api-2.0.1/src/openapi_client/model/test_list_enum.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/throttled_schedule_options.py` & `klaviyo-api-2.0.1/src/openapi_client/model/throttled_schedule_options.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/tracking_options_sub_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/tracking_options_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/unsubscription_create_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/unsubscription_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/unsubscription_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/unsubscription_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/unsuppression_create_job_create_query.py` & `klaviyo-api-2.0.1/src/openapi_client/model/unsuppression_create_job_create_query.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/unsuppression_create_job_create_query_resource_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py` & `klaviyo-api-2.0.1/src/openapi_client/model/unsuppression_create_job_create_query_resource_object_attributes.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/utm_param_info.py` & `klaviyo-api-2.0.1/src/openapi_client/model/utm_param_info.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model/utm_params_sub_object.py` & `klaviyo-api-2.0.1/src/openapi_client/model/utm_params_sub_object.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/model_utils.py` & `klaviyo-api-2.0.1/src/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/models/__init__.py` & `klaviyo-api-2.0.1/src/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `klaviyo-api-2.0.0/src/openapi_client/rest.py` & `klaviyo-api-2.0.1/src/openapi_client/rest.py`

 * *Files identical despite different names*

