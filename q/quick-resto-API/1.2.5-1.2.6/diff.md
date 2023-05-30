# Comparing `tmp/quick_resto_API-1.2.5.tar.gz` & `tmp/quick_resto_API-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quick_resto_API-1.2.5.tar", last modified: Wed May 24 09:49:41 2023, max compression
+gzip compressed data, was "quick_resto_API-1.2.6.tar", last modified: Tue May 30 10:14:43 2023, max compression
```

## Comparing `quick_resto_API-1.2.5.tar` & `quick_resto_API-1.2.6.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.649672 quick_resto_API-1.2.5/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-24 09:49:41.648672 quick_resto_API-1.2.5/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      219 2023-05-02 14:35:20.000000 quick_resto_API-1.2.5/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.622673 quick_resto_API-1.2.5/quick_resto_API/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5150 2023-05-11 17:27:16.000000 quick_resto_API-1.2.5/quick_resto_API/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.623673 quick_resto_API-1.2.5/quick_resto_API/class_generator/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2391 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/class_generator/class_generator.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.623673 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.623673 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/list_request/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1153 2023-05-10 14:11:39.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/list_request/filter.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1765 2023-05-10 14:11:30.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/list_request/list_request.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.631672 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4595 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/account_type_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4792 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4656 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4623 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4488 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/business_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4621 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/cancellation_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4585 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/company_info_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4704 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4647 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4580 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4882 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4704 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5817 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/dish_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4488 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/employee_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4548 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/encashment_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4738 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4656 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4360 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/hall_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4738 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4804 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6061 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4417 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/markup_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4603 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6024 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/modifier_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4850 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4520 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/order_info_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4738 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4603 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4604 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/payment_type_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6061 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4622 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4806 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8126 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/providers_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4797 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4545 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/sale_place_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4792 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6125 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/semi_product_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4380 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/shift_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6239 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/single_product_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4645 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4386 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/store_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4394 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/table_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4595 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4486 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/terminal_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4636 2023-05-24 09:40:44.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4813 2023-05-24 09:45:31.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/operations_with_objects.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       25 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/system_object.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2947 2023-05-10 13:24:23.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_api.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4045 2022-07-25 09:16:26.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_interface.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.631672 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.620673 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.631672 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/alcohol/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1432 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1139 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.633672 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2082 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/business.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2043 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/company_info.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2335 2022-08-08 09:56:10.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1084 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1523 2022-07-25 09:16:26.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/payment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4413 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/payment_types.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      554 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.634672 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      922 2023-04-03 12:13:12.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1050 2023-04-03 12:13:17.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/account_type.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3641 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1109 2023-04-03 12:13:08.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3911 2023-04-03 12:35:57.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/customer.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1166 2023-04-03 12:13:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1974 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3104 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1091 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/group.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4490 2022-08-29 09:39:40.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/markup.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3599 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.638672 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3912 2022-08-29 07:33:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/cancellation.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      944 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/device_command.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/encashment.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1150 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/hall.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1837 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8027 2023-04-28 14:05:39.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/order_info.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4908 2023-02-09 11:42:24.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/order_item.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3107 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2661 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2285 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7697 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/shift.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2502 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2060 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3783 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4101 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1851 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3121 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.638672 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/personnel/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1478 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/personnel/employee.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1353 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/personnel/user.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.644672 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1267 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2128 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2146 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2792 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1492 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4215 2023-05-10 13:10:59.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2810 2023-05-10 13:46:52.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1069 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      678 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2008 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2708 2022-12-15 17:43:37.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2223 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4389 2023-02-09 11:48:16.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2565 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1271 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1264 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3405 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2137 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      802 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4986 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3366 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1819 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3241 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1097 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/store.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1815 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.647672 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/platform/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      393 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/platform/right.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      557 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/platform/right_link.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1447 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/platform/role.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2191 2023-05-10 13:31:30.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/quick_resto_object.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      735 2022-07-15 09:27:22.000000 quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/styler.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-24 09:49:41.622673 quick_resto_API-1.2.5/quick_resto_API.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-24 09:49:41.000000 quick_resto_API-1.2.5/quick_resto_API.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8703 2023-05-24 09:49:41.000000 quick_resto_API-1.2.5/quick_resto_API.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-24 09:49:41.000000 quick_resto_API-1.2.5/quick_resto_API.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       16 2023-05-24 09:49:41.000000 quick_resto_API-1.2.5/quick_resto_API.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2023-05-24 09:49:41.649672 quick_resto_API-1.2.5/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      403 2023-05-24 09:49:31.000000 quick_resto_API-1.2.5/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.690326 quick_resto_API-1.2.6/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-30 10:14:43.690326 quick_resto_API-1.2.6/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      219 2023-05-02 14:35:20.000000 quick_resto_API-1.2.6/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.614328 quick_resto_API-1.2.6/quick_resto_API/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5150 2023-05-11 17:27:16.000000 quick_resto_API-1.2.6/quick_resto_API/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.615328 quick_resto_API-1.2.6/quick_resto_API/class_generator/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2391 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/class_generator/class_generator.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.616328 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.618328 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/list_request/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1153 2023-05-10 14:11:39.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/list_request/filter.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1765 2023-05-10 14:11:30.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/list_request/list_request.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.643327 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4595 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/account_type_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4792 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4656 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4623 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4488 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/business_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4621 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/cancellation_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4585 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/company_info_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4704 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4647 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4580 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4882 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4704 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5817 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/dish_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4488 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/employee_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4548 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/encashment_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4738 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4656 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4360 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/hall_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4738 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4804 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6061 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4417 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/markup_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4603 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6024 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/modifier_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4850 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4520 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/order_info_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4738 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4603 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4604 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/payment_type_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6061 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4622 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4806 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8126 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/providers_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4797 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4545 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/sale_place_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4792 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6125 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/semi_product_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4380 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/shift_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6239 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/single_product_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4645 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4386 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/store_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4394 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/table_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4595 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4486 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/terminal_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4636 2023-05-24 09:40:44.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4813 2023-05-24 09:45:31.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/operations_with_objects.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       25 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/system_object.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2947 2023-05-10 13:24:23.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_api.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4045 2022-07-25 09:16:26.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_interface.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.644327 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.612328 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.645327 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/alcohol/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1297 2023-05-30 09:56:21.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1004 2023-05-30 09:56:38.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.647327 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1947 2023-05-30 09:56:52.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/business.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1907 2023-05-30 09:57:06.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/company_info.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1768 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2189 2023-05-30 09:57:23.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1084 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1523 2022-07-25 09:16:26.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/payment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4413 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/payment_types.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      425 2023-05-30 09:57:37.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/store_item_tag.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.650327 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      922 2023-04-03 12:13:12.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      914 2023-05-30 10:00:36.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/account_type.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3506 2023-05-30 10:00:46.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1109 2023-04-03 12:13:08.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3911 2023-04-03 12:35:57.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/customer.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1089 2023-05-30 10:01:45.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/customer_account.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1974 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2969 2023-05-30 10:00:59.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      956 2023-05-30 10:01:10.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/group.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4355 2023-05-30 10:01:21.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/markup.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3464 2023-05-30 10:01:33.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.665327 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3912 2022-08-29 07:33:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/cancellation.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      944 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/device_command.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/encashment.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      997 2023-05-30 10:02:06.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/hall.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1685 2023-05-30 10:00:03.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8027 2023-04-28 14:05:39.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/order_info.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4773 2023-05-30 09:59:48.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/order_item.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2955 2023-05-30 09:59:18.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2661 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2157 2023-05-30 09:59:32.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7697 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/shift.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2367 2023-05-30 09:58:00.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1925 2023-05-30 10:02:15.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3656 2023-05-30 09:58:16.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3966 2023-05-30 09:59:05.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1699 2023-05-30 09:58:43.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2969 2023-05-30 09:56:02.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.672327 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/personnel/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1478 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/personnel/employee.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1218 2023-05-30 09:55:28.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/personnel/user.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.689326 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1267 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2128 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2146 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2792 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1492 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4215 2023-05-10 13:10:59.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2810 2023-05-10 13:46:52.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1069 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      678 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2008 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2708 2022-12-15 17:43:37.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2223 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4260 2023-05-30 10:00:19.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2435 2023-05-30 09:55:46.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1271 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1264 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3405 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2137 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      802 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4986 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3366 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1819 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3241 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1097 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/store.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1815 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.689326 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/platform/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      393 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/platform/right.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      557 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/platform/right_link.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1447 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/platform/role.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2356 2023-05-30 09:54:32.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/quick_resto_object.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      735 2022-07-15 09:27:22.000000 quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/styler.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-30 10:14:43.615328 quick_resto_API-1.2.6/quick_resto_API.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      405 2023-05-30 10:14:43.000000 quick_resto_API-1.2.6/quick_resto_API.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8703 2023-05-30 10:14:43.000000 quick_resto_API-1.2.6/quick_resto_API.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-30 10:14:43.000000 quick_resto_API-1.2.6/quick_resto_API.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       16 2023-05-30 10:14:43.000000 quick_resto_API-1.2.6/quick_resto_API.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2023-05-30 10:14:43.690326 quick_resto_API-1.2.6/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      403 2023-05-30 10:13:44.000000 quick_resto_API-1.2.6/setup.py
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/__init__.py` & `quick_resto_API-1.2.6/quick_resto_API/__init__.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/class_generator/class_generator.py` & `quick_resto_API-1.2.6/quick_resto_API/class_generator/class_generator.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/list_request/filter.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/list_request/filter.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/list_request/list_request.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/list_request/list_request.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/account_type_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/account_type_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/alcohol_dictionary_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/alcohol_report_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/bonus_program_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/business_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/business_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/cancellation_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/cancellation_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/company_info_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/company_info_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/cooking_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/cooking_place_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/crm_customer_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/decomposition_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/discard_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/dish_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/dish_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/employee_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/employee_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/encashment_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/encashment_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/exchange_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/fixed_discount_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/hall_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/hall_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/incoming_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/inventory_document_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/kkm_terminal_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/markup_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/markup_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/measure_unit_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/modifier_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/modifier_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/order_discard_reason_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/order_info_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/order_info_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/outgoing_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/packing_unit_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/payment_type_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/payment_type_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/pos_terminal_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/preorder_info_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/processing_invoice_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/providers_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/providers_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/raspberry_terminal_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/sale_place_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/sale_place_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/scheduled_discount_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/semi_product_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/semi_product_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/shift_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/shift_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/single_product_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/single_product_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/store_item_tag_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/store_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/store_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/table_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/table_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/table_scheme_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/terminal_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/terminal_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/modules/ticket_device_operations.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/operations_with_objects/operations_with_objects.py` & `quick_resto_API-1.2.6/quick_resto_API/operations_with_objects/operations_with_objects.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_api.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_api.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_interface.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_interface.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_dictionary.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from quick_resto_API.quick_resto_objects.modules.warehouse.dish import Dish
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 class AlcoholDictionary(QuickRestoObject):
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def egais_name(self) -> str:
         return self._egais_name
 
     @property
     def egais_size(self) -> int:
         return self._egais_size
 
@@ -22,21 +18,20 @@
     def show_on_terminal(self) -> bool:
         return self._show_on_terminal
 
     @property
     def store_product(self) -> Dish:
         return self._store_product
 
-    def __init__(self, deleted: bool = None, egaisName: str = None, egaisSize: int = None, egaisTypeCode: str = None,
+    def __init__(self, egaisName: str = None, egaisSize: int = None, egaisTypeCode: str = None,
                  showOnTerminal: bool = None, storeProduct: dict = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.alcohol.dictionary.AlcoholDictionary"
 
         super().__init__(class_name=class_name, **kwargs)
 
-        self._deleted: bool = deleted
         self._egais_name: str = egaisName
         self._egais_size: int = egaisSize
         self._egais_type_code: str = egaisTypeCode
         self._show_on_terminal: bool = showOnTerminal
 
         if storeProduct is not None:
             self._store_product = Dish(**storeProduct)
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/alcohol/alcohol_report.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 from quick_resto_API.quick_resto_objects.modules.alcohol.alcohol_dictionary import AlcoholDictionary
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
 class AlcoholReport(QuickRestoObject):
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def tap_time(self) -> int:
         return self._tap_time
 
     @property
     def count(self) -> int:
         return self._count
 
     @property
     def alcohol_dictionary(self) -> AlcoholDictionary:
         return self._alcohol_dictionary
 
-    def __init__(self, deleted: bool = None, tapTime: int = None, count: int = None, alcoholDictionary: dict = None,
+    def __init__(self, tapTime: int = None, count: int = None, alcoholDictionary: dict = None,
                  **kwargs):
         class_name = "ru.edgex.quickresto.modules.alcohol.report.AlcoholReport"
 
         super().__init__(class_name=class_name, **kwargs)
 
-        self._deleted: bool = deleted
         self._tap_time: int = tapTime
         self._count: int = count
         
         if alcoholDictionary is not None: 
             self._alcohol_dictionary = AlcoholDictionary(**alcoholDictionary)
         else:
             self._alcohol_dictionary = None
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/business.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/company_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
-class Business(QuickRestoObject):
+class CompanyInfo(QuickRestoObject):
     @property
     def account(self) -> str:
         return self._account
 
     @property
     def address(self) -> str:
         return self._address
@@ -23,18 +23,14 @@
         return self._correspondent_account
 
     @property
     def delivery_address(self) -> str:
         return self._delivery_address
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def inn_code(self) -> str:
         return self._inn_code
 
     @property
     def kpp_code(self) -> str:
         return self._kpp_code
 
@@ -46,28 +42,26 @@
     def okpo_code(self) -> str:
         return self._okpo_code
 
     @property
     def short_name(self) -> str:
         return self._short_name
 
-    def __init__(self, account: str = None, address: str = None, bankId: str = None, bankName: str = None,
-                 correspondentAccount: str = None,
-                 deliveryAddress: str = None, deleted: bool = None, innCode: str = None, kppCode: str = None,
-                 name: str = None, okpoCode: str = None,
-                 shortName: str = None, **kwargs):
-        class_name = "ru.edgex.quickresto.modules.core.company.businesses.Business"
+    def __init__(self, account: str = None, address: str = None, bankId: str = None, bankName: str = None, 
+                correspondentAccount: str = None, deliveryAddress: str = None,innCode: str = None, 
+                kppCode: str = None, name: str = None, okpoCode: str = None,shortName: str = None, **kwargs):
+
+        class_name = "ru.edgex.quickresto.modules.core.company.CompanyInfo"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._account: str = account
         self._address: str = address
         self._bank_id: str = bankId
         self._bank_name: str = bankName
         self._correspondent_account: str = correspondentAccount
         self._delivery_address: str = deliveryAddress
-        self._deleted: bool = deleted
         self._inn_code: str = innCode
         self._kpp_code: str = kppCode
         self._name: str = name
         self._okpo_code: str = okpoCode
         self._short_name: str = shortName
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/company_info.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/business.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
-class CompanyInfo(QuickRestoObject):
+class Business(QuickRestoObject):
     @property
     def account(self) -> str:
         return self._account
 
     @property
     def address(self) -> str:
         return self._address
@@ -23,18 +23,14 @@
         return self._correspondent_account
 
     @property
     def delivery_address(self) -> str:
         return self._delivery_address
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def inn_code(self) -> str:
         return self._inn_code
 
     @property
     def kpp_code(self) -> str:
         return self._kpp_code
 
@@ -46,27 +42,27 @@
     def okpo_code(self) -> str:
         return self._okpo_code
 
     @property
     def short_name(self) -> str:
         return self._short_name
 
-    def __init__(self, account: str = None, address: str = None, bankId: str = None, bankName: str = None, 
-                correspondentAccount: str = None, deliveryAddress: str = None, deleted: bool = None, innCode: str = None, 
-                kppCode: str = None, name: str = None, okpoCode: str = None,shortName: str = None, **kwargs):
-
-        class_name = "ru.edgex.quickresto.modules.core.company.CompanyInfo"
+    def __init__(self, account: str = None, address: str = None, bankId: str = None, bankName: str = None,
+                 correspondentAccount: str = None,
+                 deliveryAddress: str = None, innCode: str = None, kppCode: str = None,
+                 name: str = None, okpoCode: str = None,
+                 shortName: str = None, **kwargs):
+        class_name = "ru.edgex.quickresto.modules.core.company.businesses.Business"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._account: str = account
         self._address: str = address
         self._bank_id: str = bankId
         self._bank_name: str = bankName
         self._correspondent_account: str = correspondentAccount
         self._delivery_address: str = deliveryAddress
-        self._deleted: bool = deleted
         self._inn_code: str = innCode
         self._kpp_code: str = kppCode
         self._name: str = name
         self._okpo_code: str = okpoCode
         self._short_name: str = shortName
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/measure_unit.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/order_discard_reason.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,14 @@
         return StrToSystemOrderDiscardReason[value]
 
     return SystemOrderDiscardReason.NONE
 
 
 class OrderDiscardReason(QuickRestoObject):
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def save_to_terminals(self) -> bool:
         return self._save_to_terminals
 
     @property
     def description(self) -> str:
         return self._description
 
@@ -49,20 +45,18 @@
         return self._withdraw_from_store
 
     @property
     def system_order_discard_reason(self) -> SystemOrderDiscardReason:
         return self._system_order_discard_reason
 
     def __init__(self, saveToTerminals: bool = None, description: str = None, systemOrderDiscardReason: str = None, title: str = None,
-                 useComment: bool = None,
-                 withdrawFromStore: bool = None, deleted: bool = None, **kwargs):
+                 useComment: bool = None, withdrawFromStore: bool = None, **kwargs):
         class_name: str = "ru.edgex.quickresto.modules.core.dictionaries.orderdiscardreasons.OrderDiscardReason"
 
         super().__init__(class_name=class_name, **kwargs)
 
-        self._deleted = deleted
         self._save_to_terminals = saveToTerminals
         self._description = description
         self._title = title
         self._use_comment = useComment
         self._withdraw_from_store = withdrawFromStore
         self._system_order_discard_reason = convert_str_to_system_order_discard_reason(systemOrderDiscardReason)
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/packing_unit.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/payment.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/payment.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/core/payment_types.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/core/payment_types.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/account_balance.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/account_type.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/account_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,23 @@
         return self._name
 
     @property
     def account_guid(self) -> str:
         return self._account_guid
 
     @property
-    def deleted(self) -> float:
-        return self._deleted
-
-    @property
     def max_usage(self) -> float:
         return self._max_usage
 
     @property
     def reset_period(self) -> float:
         return self._reset_period
 
-    def __init__(self, accountGuid: str = None, deleted: bool = None, maxUsage: float = None, name: str = None,
+    def __init__(self, accountGuid: str = None, maxUsage: float = None, name: str = None,
                  resetPeriod: float = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.crm.accounting.account.account_balance.AccountType"
 
         super().__init__(class_name=class_name, **kwargs)
         self._name: str = name
         self._account_guid: str = accountGuid
-        self._deleted: bool = deleted
         self._max_usage: float = maxUsage
         self._reset_period: float = resetPeriod
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/bonus_program.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 
 class BonusProgram(QuickRestoObject):
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def days(self) -> list:
         return self._days
 
     @property
     def groups(self) -> list:
         return self._groups
 
@@ -59,26 +55,25 @@
     def dishes(self) -> list:
         return self._dishes
 
     @property
     def tags(self) -> list:
         return self._tags
 
-    def __init__(self, name: str = None, deleted: bool = None, days: list = None, groups: list = None,
+    def __init__(self, name: str = None, days: list = None, groups: list = None,
                  startDate: str = None, endDate: str = None,
                  accValue: float = None, accountType: dict = None, doNotAccumulateWhileRedeeming: bool = None,
                  greetingBonus: float = None,
                  birthdayBonus: float = None, categories: list = None, dishes: list = None, tags: list = None,
                  **kwargs):
         class_name = "ru.edgex.quickresto.modules.crm.settings.bonus.BonusProgram"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._name: str = name
-        self._deleted: bool = deleted
 
         if days is not None: 
             self._days: list = [Day(**day) for day in days]
         else:
             self._days = None 
 
         if groups is not None:
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/contact_method.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/customer.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/customer.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/customer_token.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/fixed_discount.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,14 @@
 
 class FixedDiscount(QuickRestoObject):
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def type_discount(self) -> TypeDiscount:
         return self._type_discount
 
     @property
     def value(self) -> float:
         return self._value
 
@@ -62,23 +58,22 @@
     def sale_places(self) -> set:
         return self._sale_places
 
     @property
     def index(self) -> int:
         return self._index
 
-    def __init__(self, name: str = None, deleted: bool = None, typeDiscount: str = None, value: float = None,
+    def __init__(self, name: str = None, typeDiscount: str = None, value: float = None,
                  categories: set = None, dishes: set = None,
                  tags: set = None, modifierGroups: list = None, salePlaces: set = None, index: int = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.crm.settings.fixed.FixedDiscount"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._name: str = name
-        self._deleted: bool = deleted
         self._type_discount = convert_str_to_type_discount(typeDiscount)
         self._value: float = value
 
         if categories is not None: 
             self._categories: set = [DishCategory(**category) for category in categories]
         else:
             self._categories = None
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/group.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/group.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,29 +7,24 @@
         return self._name
 
     @property
     def group_id(self) -> int:
         return self._group_id
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def discount_value(self) -> float:
         return self._discount_value
 
     @property
     def customer_operation_limit(self) -> int:
         return self._customer_operation_limit
 
-    def __init__(self, groupId: int = None, deleted: bool = None, name: str = None, discountValue: float = None,
+    def __init__(self, groupId: int = None, name: str = None, discountValue: float = None,
                  customerOperationLimit: int = None,
                  **kwargs):
         class_name = "ru.edgex.quickresto.modules.crm.customer.group.Group"
 
         super().__init__(class_name=class_name, **kwargs)
         self._group_id: int = groupId
-        self._deleted: bool = deleted
         self._name: str = name
         self._discount_value: float = discountValue
         self._customer_operation_limit: int = customerOperationLimit
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/markup.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/markup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,18 +49,14 @@
 
 class Markup(QuickRestoObject):
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def type_discount(self) -> TypeDiscount:
         return self._type_discount
 
     @property
     def value(self) -> float:
         return self._value
 
@@ -92,25 +88,24 @@
     def sale_places(self) -> list:
         return self._sale_places
 
     @property
     def days(self) -> list:
         return self._days
 
-    def __init__(self, name: str = None, deleted: bool = None, typeDiscount: str = None, value: float = None,
+    def __init__(self, name: str = None, typeDiscount: str = None, value: float = None,
                  operatorCancellable: bool = None,
                  dateRange: dict = None, categories: list = None, dishes: list = None, tags: list = None,
                  modifierGroups: list = None, salePlaces: list = None,
                  days: list = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.crm.settings.markup.Markup"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._name: str = name
-        self._deleted: bool = deleted
         self._type_discount = convert_str_to_type_discount(typeDiscount)
         self._value: float = value
         self._operator_cancellable: bool = operatorCancellable
 
         if dateRange is not None: 
             self._date_range = TimeRange(**dateRange)
         else:
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/crm/scheduled_discount.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 
 class ScheduledDiscount(QuickRestoObject):
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def type_discount(self) -> TypeDiscount:
         return self._type_discount
 
     @property
     def date_range(self) -> TimeRange:
         return self._date_range
 
@@ -53,25 +49,24 @@
     def sale_places(self) -> set:
         return self._sale_places
 
     @property
     def days(self) -> list:
         return self._days
 
-    def __init__(self, name: str = None, deleted: bool = None, typeDiscount: str = None, value: float = None,
+    def __init__(self, name: str = None, typeDiscount: str = None, value: float = None,
                  categories: set = None, dishes: set = None,
                  tags: set = None, modifierGroups: list = None, salePlaces: set = None, dateRange: dict = None,
                  days: list = None,
                  operatorCancellable: bool = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.crm.settings.scheduled.ScheduledDiscount"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._name: str = name
-        self._deleted: bool = deleted
         self._type_discount = convert_str_to_type_discount(typeDiscount)
 
         if dateRange is not None: 
             self._date_range = TimeRange(**dateRange)
         else:
             self._date_range = None
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/cancellation.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/cancellation.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/device_command.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/device_command.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/encashment.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/encashment.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/hall.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/hall.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from quick_resto_API.quick_resto_objects.modules.front.table import Table
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
 class Hall(QuickRestoObject):
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def tables(self) -> list:
         return self._tables
 
     @property
     def width(self) -> int:
         return self._width
 
@@ -19,21 +15,18 @@
     def height(self) -> int:
         return self._height
 
     @property
     def title(self) -> str:
         return self._title
 
-    def __init__(self, deleted: bool = None, tables: list = None, width: int = None,
-                 height: int = None, title: str = None, **kwargs):
+    def __init__(self, tables: list = None, width: int = None, height: int = None, title: str = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.front.tablemanagement.hall.Hall"
         
         super().__init__(class_name=class_name, **kwargs)
-
-        self._deleted: bool = deleted
         
         if tables is not None: 
             self._tables: list = [Table(**value) for value in tables]
         else:
             self._tables = None
 
         self._width: int = width
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/kkm_terminal.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/table.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,92 @@
-from quick_resto_API.quick_resto_objects.modules.front.device_command import DeviceCommand
+from enum import Enum
+
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
-class KkmTerminal(QuickRestoObject):
+class TableShape(Enum):
+    RECT = 'rect'
+    CIRCLE = 'circle'
+    NONE = 'NONE'
+
+
+StrToTableShape = {
+    TableShape.RECT.value: TableShape.RECT,
+    TableShape.CIRCLE.value: TableShape.CIRCLE
+}
+
+def convert_str_to_table_shape(table_shape: str) -> TableShape:
+    if table_shape in StrToTableShape.keys():
+        return StrToTableShape[table_shape]
+
+    return TableShape.NONE
+
+
+class Table(QuickRestoObject):
     @property
-    def device_id(self) -> str:
-        return self._device_id
+    def angle(self) -> int:
+        return self._angle
 
     @property
-    def manufacturer(self) -> str:
-        return self._manufacturer
+    def x(self) -> int:
+        return self._x
 
     @property
-    def model(self) -> str:
-        return self._model
+    def y(self) -> int:
+        return self._y
 
     @property
-    def connected(self) -> bool:
-        return self._connected
+    def width(self) -> int:
+        return self._width
 
     @property
-    def name(self) -> str:
-        return self._name
+    def height(self) -> int:
+        return self._height
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
+    def is_busy(self) -> bool:
+        return self._is_busy
 
     @property
-    def activate_on_current_terminal(self) -> bool:
-        return self._activate_on_current_terminal
+    def item_title(self) -> str:
+        return self._item_title
 
     @property
-    def state(self) -> str:
-        return self._state
+    def min_capacity(self) -> int:
+        return self._min_capacity
 
     @property
-    def command(self) -> DeviceCommand:
-        return self._command
+    def max_capacity(self) -> int:
+        return self._max_capacity
 
-    def __init__(self, deviceId: str = None, manufacturer: str = None, model: str = None, connected: bool = None,
-                 name: str = None, deleted: bool = None,
-                 activateOnCurrentTerminal: bool = None, state: str = None, command: dict = None, **kwargs):
-        class_name = "ru.edgex.quickresto.modules.front.terminals.kkm.KkmTerminal"
+    @property
+    def reservable(self) -> bool:
+        return self._reservable
 
-        super().__init__(class_name=class_name, **kwargs)
+    @property
+    def shape(self) -> TableShape:
+        return self._shape
 
-        self._device_id: str = deviceId
-        self._manufacturer: str = manufacturer
-        self._model: str = model
-        self._connected: bool = connected
-        self._name: str = name
-        self._deleted: bool = deleted
-        self._activate_on_current_terminal: bool = activateOnCurrentTerminal
-        self._state: str = state
-
-        if command is not None: 
-            self._command = DeviceCommand(**command)
-        else:
-            self._command = None
+    @property
+    def title(self) -> str:
+        return self._title
+
+    def __init__(self, angle: int = None, width: int = None, height: int = None,
+                 isBusy: bool = None, itemTitle: str = None,
+                 minCapacity: int = None, maxCapacity: int = None, reservable: bool = None, shape: str = None,
+                 title: str = None, x: int = None, y: int = None,
+                 **kwargs):
+        class_name = "ru.edgex.quickresto.modules.front.tablemanagement.table.Table"
+
+        super().__init__(class_name=class_name, **kwargs)
+        self._angle: int = angle
+        self._x: int = x
+        self._y: int = y
+        self._width: int = width
+        self._height: int = height
+        self._is_busy: bool = isBusy
+        self._item_title: str = itemTitle
+        self._min_capacity: int = minCapacity
+        self._max_capacity: int = maxCapacity
+        self._reservable: bool = reservable
+        self._title: str = title
+        self._shape: TableShape = convert_str_to_table_shape(shape)
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/order_info.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/order_info.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/order_item.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/order_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,14 @@
         return self._cost_price
 
     @property
     def surcharge(self) -> float:
         return self._surcharge
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def price(self) -> float:
         return self._price
 
     @property
     def amount(self) -> float:
         return self._amount
 
@@ -83,25 +79,24 @@
     def total_amount(self) -> float:
         return self._total_amount
 
     @property
     def name(self) -> str:
         return self._name
 
-    def __init__(self, costPrice: float = None, surcharge: float = None, deleted: bool = None, price: float = None, 
+    def __init__(self, costPrice: float = None, surcharge: float = None, price: float = None, 
                 amount: float = None, salePlace: dict = None, seqNumber: int = None, product: dict = None, store: dict = None, 
                 costPriceKg: float = None, productQuantityKg: float = None, effectiveRatio: float = None, effectivePack: float = None, 
                 storeItem: dict = None, cookingPlace: dict = None, totalPrice: float = None, totalAbsoluteDiscount: float = None, 
                 totalAbsoluteCharge: float = None, totalAmount: float = None, name: str = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.front.orders.OrderItem"
         super().__init__(class_name=class_name, **kwargs)
 
         self._cost_price: float = costPrice
         self._surcharge: float = surcharge
-        self._deleted: bool = deleted
         self._price: float = price
         self._amount: float = amount
         self._seq_number: int = seqNumber
         self._cost_price_kg: float = costPriceKg
         self._product_quantity_kg: float = productQuantityKg
         self._effective_ratio: float = effectiveRatio
         self._effective_pack: float = effectivePack
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/pos_terminal.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,14 @@
         return self._connected
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def activate_on_current_terminal(self) -> bool:
         return self._activate_on_current_terminal
 
     @property
     def state(self) -> str:
         return self._state
 
@@ -61,30 +57,28 @@
         return self._arcus2_protocol
 
     @property
     def pos_printing_type(self) -> str:
         return self._pos_printing_type
 
     def __init__(self, deviceId: str = None, manufacturer: str = None, model: str = None, connected: bool = None,
-                 name: str = None,
-                 deleted: bool = None, activateOnCurrentTerminal: bool = None, state: str = None,
+                 name: str = None, activateOnCurrentTerminal: bool = None, state: str = None,
                  tableScheme: dict = None, command: dict = None,
                  business: dict = None, connectionKind: str = None, posAdditionalInfo: str = None,
                  arcus2Protocol: str = None,
                  posPrintingType: str = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.front.terminals.pos.PosTerminal"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._device_id: str = deviceId
         self._manufacturer: str = manufacturer
         self._model: str = model
         self._connected: bool = connected
         self._name: str = name
-        self._deleted: bool = deleted
         self._activate_on_current_terminal: bool = activateOnCurrentTerminal
         self._state: str = state
 
         if tableScheme is not None: 
             self._table_scheme = TableScheme(**tableScheme)
         else:
             self._table_scheme = None
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/preorder_info.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/raspberry_terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,14 @@
         return self._model
 
     @property
     def connected(self) -> bool:
         return self._connected
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def name(self) -> str:
         return self._name
 
     @property
     def serial_number(self) -> str:
         return self._serial_number
 
@@ -55,27 +51,26 @@
         return self._product
 
     @property
     def online(self) -> bool:
         return self._online
 
     def __init__(self, code1C: str, deviceId: str, macAddress: str, manufacturer: str, model: str, connected: bool,
-                 deleted: bool, name: str, serialNumber: str, hardwareVersion: str, lastSyncTime: str,
+                 name: str, serialNumber: str, hardwareVersion: str, lastSyncTime: str,
                  softwareVersion: str, product: str, online: bool, **kwargs):
         class_name = "ru.edgex.quickresto.modules.front.terminals.raspberry.RaspberryTerminal"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._code1_c: str = code1C
         self._device_id: str = deviceId
         self._mac_address: str = macAddress
         self._manufacturer: str = manufacturer
         self._model: str = model
         self._connected: bool = connected
-        self._deleted: bool = deleted
         self._name: str = name
         self._serial_number: str = serialNumber
         self._hardware_version: str = hardwareVersion
         self._last_sync_time: str = lastSyncTime
         self._software_version: str = softwareVersion
         self._product: str = product
         self._online: bool = online
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/shift.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/shift.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/table.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/single_product.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,103 @@
-from enum import Enum
-
+from quick_resto_API.quick_resto_objects.modules.core.measure_unit import MeasureUnit
+from quick_resto_API.quick_resto_objects.modules.core.store_item_tag import StoreItemTag
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
-class TableShape(Enum):
-    RECT = 'rect'
-    CIRCLE = 'circle'
-    NONE = 'NONE'
-
-
-StrToTableShape = {
-    TableShape.RECT.value: TableShape.RECT,
-    TableShape.CIRCLE.value: TableShape.CIRCLE
-}
-
-def convert_str_to_table_shape(table_shape: str) -> TableShape:
-    if table_shape in StrToTableShape.keys():
-        return StrToTableShape[table_shape]
-
-    return TableShape.NONE
+class SingleProduct(QuickRestoObject):
+    @property
+    def name(self) -> str:
+        return self._name
 
+    @property
+    def article(self) -> str:
+        return self._article
 
-class Table(QuickRestoObject):
     @property
-    def angle(self) -> int:
-        return self._angle
+    def measure_unit(self) -> MeasureUnit:
+        return self._measure_unit
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
+    def ratio(self) -> float:
+        return self._ratio
 
     @property
-    def x(self) -> int:
-        return self._x
+    def store_item_tag(self) -> StoreItemTag:
+        return self._store_item_tag
 
     @property
-    def y(self) -> int:
-        return self._y
+    def minimal_price(self) -> float:
+        return self._minimal_price
 
     @property
-    def width(self) -> int:
-        return self._width
+    def exclude_discount(self) -> bool:
+        return self._exclude_discount
 
     @property
-    def height(self) -> int:
-        return self._height
+    def exclude_markup(self) -> bool:
+        return self._exclude_markup
 
     @property
-    def is_busy(self) -> bool:
-        return self._is_busy
+    def store_quantity_kg(self) -> float:
+        return self._store_quantity_kg
 
     @property
     def item_title(self) -> str:
         return self._item_title
 
     @property
-    def min_capacity(self) -> int:
-        return self._min_capacity
+    def base_price_in_list(self) -> float:
+        return self._base_price_in_list
 
     @property
-    def max_capacity(self) -> int:
-        return self._max_capacity
+    def pack(self) -> float:
+        return self._pack
 
     @property
-    def reservable(self) -> bool:
-        return self._reservable
+    def recipe(self) -> str:
+        return self._recipe
 
     @property
-    def shape(self) -> TableShape:
-        return self._shape
+    def parent_id(self) -> int:
+        return self._parent_id
 
     @property
-    def title(self) -> str:
-        return self._title
+    def parent_item(self) -> dict:
+        return self._parent_item
 
-    def __init__(self, angle: int = None, deleted: bool = None, width: int = None, height: int = None,
-                 isBusy: bool = None, itemTitle: str = None,
-                 minCapacity: int = None, maxCapacity: int = None, reservable: bool = None, shape: str = None,
-                 title: str = None, x: int = None, y: int = None,
+    def __init__(self, version: int = None, serverRegisterTime: str = None, name: str = None, article: str = None,
+                 measureUnit: dict = None, ratio: float = None, parentId:int = None, parentItem:dict = None,
+                 minimalPrice: float = None, excludeDiscount: bool = None, excludeMarkup: bool = None,
+                 storeQuantityKg: float = None, itemTitle: str = None,
+                 basePriceInList: float = None, pack: float = None, recipe: str = None, storeItemTag: dict = None,
                  **kwargs):
-        class_name = "ru.edgex.quickresto.modules.front.tablemanagement.table.Table"
-
+        class_name = "ru.edgex.quickresto.modules.warehouse.nomenclature.singleproduct.SingleProduct"
         super().__init__(class_name=class_name, **kwargs)
-        self._angle: int = angle
-        self._deleted: bool = deleted
-        self._x: int = x
-        self._y: int = y
-        self._width: int = width
-        self._height: int = height
-        self._is_busy: bool = isBusy
+
+        self._version: int = version
+        self._server_register_time: str = serverRegisterTime
+        self._name: str = name
+        self._article: str = article
+
+        if measureUnit is not None: 
+            self._measure_unit: MeasureUnit = MeasureUnit(**measureUnit)
+        else:
+            self._measure_unit = None
+
+        self._ratio: float = ratio
+
+        if storeItemTag is not None:
+            self._store_item_tag = StoreItemTag(**storeItemTag)
+        else:
+            self._store_item_tag = None
+            
+        self._minimal_price: float = minimalPrice
+        self._exclude_discount: bool = excludeDiscount
+        self._exclude_markup: bool = excludeMarkup
+        self._store_quantity_kg: float = storeQuantityKg
         self._item_title: str = itemTitle
-        self._min_capacity: int = minCapacity
-        self._max_capacity: int = maxCapacity
-        self._reservable: bool = reservable
-        self._title: str = title
-        self._shape: TableShape = convert_str_to_table_shape(shape)
+        self._base_price_in_list: float = basePriceInList
+        self._pack: float = pack
+        self._recipe: str = recipe
+
+        self._parent_id = parentId
+        self._parent_item = parentItem
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/table_scheme.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 
 class TableScheme(QuickRestoObject):
     @property
     def current_load(self) -> int:
         return self._current_load
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def width(self) -> int:
         return self._width
 
     @property
     def height(self) -> int:
         return self._height
 
@@ -40,22 +36,21 @@
     def tables(self) -> list:
         return self._tables
 
     @property
     def halls(self) -> list:
         return self._halls
 
-    def __init__(self, currentLoad: int = None, deleted: bool = None, width: int = None, height: int = None,
+    def __init__(self, currentLoad: int = None, width: int = None, height: int = None,
                  itemTitle: str = None, maxCapacity: int = None,
                  name: str = None, tables: list = None, reservations: list = None, halls: list = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.front.tablemanagement.TableScheme"
 
         super().__init__(class_name=class_name, **kwargs)
         self._current_load: int = currentLoad
-        self._deleted: bool = deleted
         self._width: int = width
         self._height: int = height
         self._title: str = itemTitle
         self._max_capacity: int = maxCapacity
         self._name: str = name
         self._reservations: list = reservations
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/terminal.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,14 @@
 
 class Terminal(QuickRestoObject):
     @property
     def cooking_place(self) -> dict:
         return self._cooking_place
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def device_manufacturer(self) -> str:
         return self._device_manufacturer
 
     @property
     def device_model(self) -> str:
         return self._device_model
 
@@ -94,27 +90,26 @@
     def terminal_subtype(self) -> TerminalSubtype:
         return self._terminal_subtype
 
     @property
     def terminal_type(self) -> TerminalType:
         return self._terminal_type
 
-    def __init__(self, cookingPlace: dict = None, deleted: bool = None, deviceManufacturer: str = None,
+    def __init__(self, cookingPlace: dict = None, deviceManufacturer: str = None,
                  deviceModel: str = None,
                  lastSync: str = None, name: str = None, online: bool = None, registrationDate: str = None,
                  salePlace: dict = None,
                  shortName: str = None, tableScheme: dict = None, terminalSubtype: dict = None,
                  terminalType: dict = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.front.terminals.ipad.Terminal"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._cooking_place = cookingPlace
-
-        self._deleted: bool = deleted
+        
         self._device_manufacturer: str = deviceManufacturer
         self._device_model: str = deviceModel
         self._last_sync: str = lastSync
         self._name: str = name
         self._online: bool = online
         self._registration_date: str = registrationDate
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/ticket_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,14 @@
         return self._connected
 
     @property
     def device_id(self) -> str:
         return self._device_id
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def name(self) -> str:
         return self._name
 
     @property
     def serial_number(self) -> str:
         return self._serial_number
 
@@ -96,29 +92,28 @@
 
     @property
     def organization(self) -> Organization:
         return self._organization
 
     def __init__(self, code1C: str = None, macAddress: str = None, manufacturer: str = None, model: str = None,
                  connected: bool = None,
-                 deviceId: str = None, deleted: bool = None, name: str = None, serialNumber: str = None,
+                 deviceId: str = None, name: str = None, serialNumber: str = None,
                  command: dict = None, tableScheme: dict = None,
                  business: dict = None, state: str = None, kkmMode: bool = None, symbolsPerLine: int = None,
                  organization: dict = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.front.terminals.ticketdevices.TicketDevice"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._code1_c: str = code1C
         self._mac_address: str = macAddress
         self._manufacturer: str = manufacturer
         self._model: str = model
         self._connected: bool = connected
         self._device_id: str = deviceId
-        self._deleted: bool = deleted
         self._name: str = name
         self._serial_number: str = serialNumber
 
         if tableScheme is not None: 
             self._table_scheme = TableScheme(**tableScheme)
         else:
             self._table_scheme = None
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/virtual_kkm_terminal.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,78 @@
-from quick_resto_API.quick_resto_objects.modules.front.device_command import DeviceCommand
+from quick_resto_API.quick_resto_objects.modules.core.measure_unit import MeasureUnit
+from quick_resto_API.quick_resto_objects.modules.core.store_item_tag import StoreItemTag
+from quick_resto_API.quick_resto_objects.modules.warehouse.dish_sale import DishSale
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
-class VirtualKkmTerminal(QuickRestoObject):
+class ModifierGroup(QuickRestoObject):
     @property
-    def device_id(self) -> str:
-        return self._device_id
+    def name(self) -> str:
+        return self._name
 
     @property
-    def manufacturer(self) -> str:
-        return self._manufacturer
+    def measure_unit(self) -> MeasureUnit:
+        return self._measure_unit
 
     @property
-    def model(self) -> str:
-        return self._model
+    def color(self) -> str:
+        return self._color
 
     @property
-    def connected(self) -> bool:
-        return self._connected
+    def display_on_terminal(self) -> bool:
+        return self._display_on_terminal
 
     @property
-    def name(self) -> str:
-        return self._name
+    def min_value(self) -> int:
+        return self._min_value
+
+    @property
+    def max_value(self) -> int:
+        return self._max_value
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
+    def with_dish(self) -> bool:
+        return self._with_dish
 
     @property
-    def activate_on_current_terminal(self) -> bool:
-        return self._activate_on_current_terminal
+    def modifier_sales(self) -> list:
+        return self._modifier_sales
 
     @property
-    def state(self) -> str:
-        return self._state
+    def item_title(self) -> str:
+        return self._item_title
 
     @property
-    def command(self) -> DeviceCommand:
-        return self._command
+    def store_item_tag(self) -> StoreItemTag:
+        return self._store_item_tag
 
-    def __init__(self, deviceId: str = None, manufacturer: str = None, model: str = None, connected: bool = None,
-                 name: str = None, deleted: bool = None,
-                 activateOnCurrentTerminal: bool = None, state: str = None, command: dict = None, **kwargs):
-        class_name = "ru.edgex.quickresto.modules.front.terminals.kkm.VirtualKkmTerminal"
+    def __init__(self, name: str = None, measureUnit: dict = None, color: str = None, displayOnTerminal: bool = None,
+                 minValue: int = None, maxValue: int = None, withDish: bool = None,
+                 modifierSales: list = None, itemTitle: str = None,storeItemTag=None, **kwargs):
+        class_name = "ru.edgex.quickresto.modules.warehouse.nomenclature.mods.ModifierGroup"
 
         super().__init__(class_name=class_name, **kwargs)
 
-        self._device_id: str = deviceId
-        self._manufacturer: str = manufacturer
-        self._model: str = model
-        self._connected: bool = connected
-        self._name: str = name
-        self._deleted: bool = deleted
-        self._activate_on_current_terminal: bool = activateOnCurrentTerminal
-        self._state: str = state
+        self._name = name
+
+        if measureUnit is not None: 
+            self._measure_unit: MeasureUnit = MeasureUnit(**measureUnit)
+        else:
+            self._measure_unit = None
+
+        self._color = color
+        self._display_on_terminal = displayOnTerminal
+        self._min_value = minValue
+        self._max_value = maxValue
+        self._with_dish = withDish
+
+        if modifierSales is not None:
+            self._modifier_sales: list = [DishSale(**dish_sale) for dish_sale in modifierSales]
+        else:
+            self._modifier_sales = None
+        
+        self._item_title = itemTitle
 
-        if command is not None: 
-            self._command = DeviceCommand(**command)
+        if storeItemTag is not None:
+            self._store_item_tag = StoreItemTag(**storeItemTag)
         else:
-            self._command = None
+            self._store_item_tag = None
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/front/virtual_pos_terminal.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,14 @@
         return self._connected
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def activate_on_current_terminal(self) -> bool:
         return self._activate_on_current_terminal
 
     @property
     def state(self) -> str:
         return self._state
 
@@ -61,30 +57,28 @@
         return self._arcus2_protocol
 
     @property
     def pos_printing_type(self) -> str:
         return self._pos_printing_type
 
     def __init__(self, deviceId: str = None, manufacturer: str = None, model: str = None, connected: bool = None,
-                 name: str = None,
-                 deleted: bool = None, activateOnCurrentTerminal: bool = None, state: str = None,
+                 name: str = None, activateOnCurrentTerminal: bool = None, state: str = None,
                  tableScheme: dict = None, command: dict = None,
                  business: dict = None, connectionKind: str = None, posAdditionalInfo: str = None,
                  arcus2Protocol: str = None,
                  posPrintingType: str = None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.front.terminals.pos.VirtualPosTerminal"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._device_id: str = deviceId
         self._manufacturer: str = manufacturer
         self._model: str = model
         self._connected: bool = connected
         self._name: str = name
-        self._deleted: bool = deleted
         self._activate_on_current_terminal: bool = activateOnCurrentTerminal
         self._state: str = state
 
         if tableScheme is not None: 
             self._table_scheme = TableScheme(**tableScheme)
         else:
             self._table_scheme = None
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/personnel/employee.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/personnel/employee.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/personnel/user.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/personnel/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,35 +14,30 @@
         return self._login
 
     @property
     def language(self) -> dict:
         return self._language
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def hidden(self) -> bool:
         return self._hidden
 
     @property
     def last_login_time(self) -> str:
         return self._last_login_time
 
     @property
     def tokens(self) -> list:
         return self._tokens
 
-    def __init__(self, userKind: str = None, lastName: str = None, login: str = None, language: dict = None, deleted: bool = None, 
+    def __init__(self, userKind: str = None, lastName: str = None, login: str = None, language: dict = None, 
                 hidden: bool = None, lastLoginTime: str = None, tokens: list = None, **kwargs):
         class_name = ""
         super().__init__(class_name=class_name, **kwargs)
 
         self._user_kind: str = userKind
         self._last_name: str = lastName
         self._login: str = login
         self._language: dict = language
-        self._deleted: bool = deleted
         self._hidden: bool = hidden
         self._last_login_time: str = lastLoginTime
         self._tokens: list = tokens
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/businessman.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/cooking_place.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/decomposition_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/discard_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/discard_reason.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/dish.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/dish_category.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/dish_sale.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/employee.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/exchange_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/incoming_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/inventory_document.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/modifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 
 class Modifier(QuickRestoObject):
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
-
-    @property
     def article(self) -> int:
         return self._article
 
     @property
     def with_dish(self) -> bool:
         return self._with_dish
 
@@ -95,21 +91,20 @@
 
     def __init__(self, name: str = None, measureUnit: dict = None, color: str = None, displayOnTerminal: bool = None,
                  minValue: int = None, maxValue: int = None, withDish: bool = None,
                  modifierSales: list = None, excludeDiscount: bool = None, excludeMarkup: bool = None,
                  article: int = None, itemTitle: str = None, parentId:int = None, parentItem:dict = None,
                  titleInPrice: str = None, storeQuantityKg: float = None, defaultValue: int = None,
                  basePriceInList: float = None, pack: float = None, recipe: str = None,
-                 price: float = None, minimalPrice: float = None, deleted: bool = None, storeItemTag=None, **kwargs):
+                 price: float = None, minimalPrice: float = None, storeItemTag=None, **kwargs):
         class_name = "ru.edgex.quickresto.modules.warehouse.nomenclature.mods.Modifier"
 
         super().__init__(class_name=class_name, **kwargs)
 
         self._name = name
-        self._deleted = deleted
 
         if measureUnit is not None: 
             self._measure_unit: MeasureUnit = MeasureUnit(**measureUnit)
         else:
             self._measure_unit = None
         
         self._color = color
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/modifier_group.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,107 @@
 from quick_resto_API.quick_resto_objects.modules.core.measure_unit import MeasureUnit
 from quick_resto_API.quick_resto_objects.modules.core.store_item_tag import StoreItemTag
-from quick_resto_API.quick_resto_objects.modules.warehouse.dish_sale import DishSale
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
-class ModifierGroup(QuickRestoObject):
+class SemiProduct(QuickRestoObject):
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def deleted(self) -> bool:
-        return self._deleted
+    def article(self) -> str:
+        return self._article
 
     @property
     def measure_unit(self) -> MeasureUnit:
         return self._measure_unit
 
     @property
-    def color(self) -> str:
-        return self._color
+    def store_item_tag(self) -> StoreItemTag:
+        return self._store_item_tag
+
+    @property
+    def ratio(self) -> float:
+        return self._ratio
 
     @property
-    def display_on_terminal(self) -> bool:
-        return self._display_on_terminal
+    def minimal_price(self) -> float:
+        return self._minimal_price
 
     @property
-    def min_value(self) -> int:
-        return self._min_value
+    def exclude_discount(self) -> bool:
+        return self._exclude_discount
 
     @property
-    def max_value(self) -> int:
-        return self._max_value
+    def exclude_markup(self) -> bool:
+        return self._exclude_markup
 
     @property
-    def with_dish(self) -> bool:
-        return self._with_dish
+    def store_quantity_kg(self) -> float:
+        return self._store_quantity_kg
 
     @property
-    def modifier_sales(self) -> list:
-        return self._modifier_sales
+    def limit(self) -> float:
+        return self._limit
 
     @property
     def item_title(self) -> str:
         return self._item_title
 
     @property
-    def store_item_tag(self) -> StoreItemTag:
-        return self._store_item_tag
+    def base_price_in_list(self) -> float:
+        return self._base_price_in_list
 
-    def __init__(self, name: str = None, measureUnit: dict = None, color: str = None, displayOnTerminal: bool = None,
-                 minValue: int = None, maxValue: int = None, withDish: bool = None,
-                 modifierSales: list = None, itemTitle: str = None, deleted: bool = None, storeItemTag=None, **kwargs):
-        class_name = "ru.edgex.quickresto.modules.warehouse.nomenclature.mods.ModifierGroup"
+    @property
+    def pack(self) -> float:
+        return self._pack
 
-        super().__init__(class_name=class_name, **kwargs)
+    @property
+    def recipe(self) -> str:
+        return self._recipe
 
-        self._name = name
-        self._deleted = deleted
+    @property
+    def parent_id(self) -> int:
+        return self._parent_id
 
+    @property
+    def parent_item(self) -> dict:
+        return self._parent_item
+
+    def __init__(self, version: int = None, serverRegisterTime: str = None, name: str = None, article: str = None,
+                 measureUnit: dict = None, storeItemTag: dict = None, parentId:int = None, parentItem:dict = None,
+                 ratio: float = None, minimalPrice: float = None, excludeDiscount: bool = None,
+                 excludeMarkup: bool = None, storeQuantityKg: float = None,
+                 limit: float = None, itemTitle: str = None, basePriceInList: float = None, pack: float = None,
+                 recipe: str = None, **kwargs):
+        class_name = "ru.edgex.quickresto.modules.warehouse.nomenclature.semiproduct.SemiProduct"
+        super().__init__(class_name=class_name, **kwargs)
+
+        self._version: int = version
+        self._server_register_time: str = serverRegisterTime
+        self._name: str = name
+        self._article: str = article
+        
         if measureUnit is not None: 
             self._measure_unit: MeasureUnit = MeasureUnit(**measureUnit)
         else:
             self._measure_unit = None
 
-        self._color = color
-        self._display_on_terminal = displayOnTerminal
-        self._min_value = minValue
-        self._max_value = maxValue
-        self._with_dish = withDish
-
-        if modifierSales is not None:
-            self._modifier_sales: list = [DishSale(**dish_sale) for dish_sale in modifierSales]
-        else:
-            self._modifier_sales = None
-        
-        self._item_title = itemTitle
-
         if storeItemTag is not None:
             self._store_item_tag = StoreItemTag(**storeItemTag)
         else:
             self._store_item_tag = None
+
+        self._ratio: float = ratio
+        self._minimal_price: float = minimalPrice
+        self._exclude_discount: bool = excludeDiscount
+        self._exclude_markup: bool = excludeMarkup
+        self._store_quantity_kg: float = storeQuantityKg
+        self._limit: float = limit
+        self._item_title: str = itemTitle
+        self._base_price_in_list: float = basePriceInList
+        self._pack: float = pack
+        self._recipe: str = recipe
+        
+        self._parent_id = parentId
+        self._parent_item = parentItem
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/natural_person.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/organization.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/outgoing_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/processing_invoice.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/provider_group.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/sale_place.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/semi_product.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,53 @@
 from quick_resto_API.quick_resto_objects.modules.core.measure_unit import MeasureUnit
 from quick_resto_API.quick_resto_objects.modules.core.store_item_tag import StoreItemTag
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
-class SemiProduct(QuickRestoObject):
+class SingleCategory(QuickRestoObject):
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def article(self) -> str:
-        return self._article
-
-    @property
     def measure_unit(self) -> MeasureUnit:
         return self._measure_unit
 
     @property
     def store_item_tag(self) -> StoreItemTag:
         return self._store_item_tag
 
     @property
-    def ratio(self) -> float:
-        return self._ratio
-
-    @property
-    def minimal_price(self) -> float:
-        return self._minimal_price
-
-    @property
-    def exclude_discount(self) -> bool:
-        return self._exclude_discount
+    def color(self) -> str:
+        return self._color
 
     @property
-    def exclude_markup(self) -> bool:
-        return self._exclude_markup
-
-    @property
-    def store_quantity_kg(self) -> float:
-        return self._store_quantity_kg
-
-    @property
-    def limit(self) -> float:
-        return self._limit
+    def display_on_terminal(self) -> bool:
+        return self._display_on_terminal
 
     @property
     def item_title(self) -> str:
         return self._item_title
 
-    @property
-    def base_price_in_list(self) -> float:
-        return self._base_price_in_list
-
-    @property
-    def pack(self) -> float:
-        return self._pack
-
-    @property
-    def recipe(self) -> str:
-        return self._recipe
-
-    @property
-    def parent_id(self) -> int:
-        return self._parent_id
-
-    @property
-    def parent_item(self) -> dict:
-        return self._parent_item
-
-    def __init__(self, version: int = None, serverRegisterTime: str = None, name: str = None, article: str = None,
-                 measureUnit: dict = None, storeItemTag: dict = None, parentId:int = None, parentItem:dict = None,
-                 ratio: float = None, minimalPrice: float = None, excludeDiscount: bool = None,
-                 excludeMarkup: bool = None, storeQuantityKg: float = None,
-                 limit: float = None, itemTitle: str = None, basePriceInList: float = None, pack: float = None,
-                 recipe: str = None, **kwargs):
-        class_name = "ru.edgex.quickresto.modules.warehouse.nomenclature.semiproduct.SemiProduct"
+    def __init__(self, version: int = None, serverRegisterTime: str = None, name: str = None, measureUnit: dict = None,
+                 storeItemTag: dict = None,
+                 color: str = None, displayOnTerminal: bool = None, itemTitle: str = None, **kwargs):
+        class_name = "ru.edgex.quickresto.modules.warehouse.nomenclature.singleproduct.SingleCategory"
         super().__init__(class_name=class_name, **kwargs)
 
         self._version: int = version
         self._server_register_time: str = serverRegisterTime
         self._name: str = name
-        self._article: str = article
-        
+
         if measureUnit is not None: 
             self._measure_unit: MeasureUnit = MeasureUnit(**measureUnit)
         else:
             self._measure_unit = None
 
         if storeItemTag is not None:
             self._store_item_tag = StoreItemTag(**storeItemTag)
         else:
             self._store_item_tag = None
 
-        self._ratio: float = ratio
-        self._minimal_price: float = minimalPrice
-        self._exclude_discount: bool = excludeDiscount
-        self._exclude_markup: bool = excludeMarkup
-        self._store_quantity_kg: float = storeQuantityKg
-        self._limit: float = limit
+        self._color: str = color
+        self._display_on_terminal: bool = displayOnTerminal
         self._item_title: str = itemTitle
-        self._base_price_in_list: float = basePriceInList
-        self._pack: float = pack
-        self._recipe: str = recipe
-        
-        self._parent_id = parentId
-        self._parent_item = parentItem
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/single_category.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/store_category.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from quick_resto_API.quick_resto_objects.modules.core.measure_unit import MeasureUnit
 from quick_resto_API.quick_resto_objects.modules.core.store_item_tag import StoreItemTag
 from quick_resto_API.quick_resto_objects.quick_resto_object import QuickRestoObject
 
 
-class SingleCategory(QuickRestoObject):
+class StoreCategory(QuickRestoObject):
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def measure_unit(self) -> MeasureUnit:
         return self._measure_unit
@@ -27,15 +27,15 @@
     @property
     def item_title(self) -> str:
         return self._item_title
 
     def __init__(self, version: int = None, serverRegisterTime: str = None, name: str = None, measureUnit: dict = None,
                  storeItemTag: dict = None,
                  color: str = None, displayOnTerminal: bool = None, itemTitle: str = None, **kwargs):
-        class_name = "ru.edgex.quickresto.modules.warehouse.nomenclature.singleproduct.SingleCategory"
+        class_name = "ru.edgex.quickresto.modules.warehouse.nomenclature.StoreCategory"
         super().__init__(class_name=class_name, **kwargs)
 
         self._version: int = version
         self._server_register_time: str = serverRegisterTime
         self._name: str = name
 
         if measureUnit is not None: 
@@ -43,11 +43,11 @@
         else:
             self._measure_unit = None
 
         if storeItemTag is not None:
             self._store_item_tag = StoreItemTag(**storeItemTag)
         else:
             self._store_item_tag = None
-
+            
         self._color: str = color
         self._display_on_terminal: bool = displayOnTerminal
         self._item_title: str = itemTitle
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/modules/warehouse/store.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/modules/warehouse/store.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/platform/right_link.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/platform/right_link.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/platform/role.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/platform/role.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/quick_resto_object.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/quick_resto_object.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     @property
     def class_name(self) -> str:
         return self._class_name
 
     @property
     def server_register_time(self) -> str:
         return self._server_register_time
+    
+    @property
+    def deleted(self) -> bool:
+        return self._deleted
 
     def get_json_object(self) -> dict:
         as_dict = self.__dict__
         result = dict()
 
         for key, value in as_dict.items():
             parameter_name = styler.to_camel_case(key)
@@ -46,25 +50,28 @@
 
     def __str__(self) -> str:
         return self.__repr__()
 
     def __repr__(self) -> str:
         return json.dumps(self.get_json_object(), cls=QuickRestoObjectEncoder, indent=4, ensure_ascii=False)
 
-    def __init__(self, class_name: str, id: int = 0,  className: str = "", _id: int = 0, serverRegisterTime: str = None, **kwargs):
+    def __init__(
+            self, class_name: str, id: int = 0,  className: str = "", _id: int = 0, deleted: bool = None, 
+            serverRegisterTime: str = None, **kwargs):
         self._id: int = id
         self._global_id: int = _id
 
         # Server do not always return className
         if className == "":
             self._class_name: str = class_name
         else:
             self._class_name: str = className
 
         self._server_register_time = serverRegisterTime
+        self._deleted: bool = deleted
 
 class QuickRestoObjectEncoder(json.JSONEncoder):
     def default(self, obj):
 
         if isinstance(obj, QuickRestoObject):
             return obj.__dict__
         elif isinstance(obj, Enum):
```

### Comparing `quick_resto_API-1.2.5/quick_resto_API/quick_resto_objects/styler.py` & `quick_resto_API-1.2.6/quick_resto_API/quick_resto_objects/styler.py`

 * *Files identical despite different names*

### Comparing `quick_resto_API-1.2.5/quick_resto_API.egg-info/SOURCES.txt` & `quick_resto_API-1.2.6/quick_resto_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

