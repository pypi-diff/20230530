# Comparing `tmp/djangosaml2-1.5.7.tar.gz` & `tmp/djangosaml2-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangosaml2-1.5.7.tar", last modified: Sun May  7 19:41:51 2023, max compression
+gzip compressed data, was "djangosaml2-1.5.8.tar", last modified: Tue May 30 08:44:29 2023, max compression
```

## Comparing `djangosaml2-1.5.7.tar` & `djangosaml2-1.5.8.tar`

### file list

```diff
@@ -1,1580 +1,85 @@
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.254062 djangosaml2-1.5.7/.tox/py3.6-django2.2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.254062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.254062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:01.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.254062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.274062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:02.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:04.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:32:55.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:01.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:32:55.000000 djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:10.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.278062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.282062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:12.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:13.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:06.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:11.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:06.000000 djangosaml2-1.5.7/.tox/py3.6-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:20.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.286062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.258062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.290062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:21.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:23.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:16.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:20.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:16.000000 djangosaml2-1.5.7/.tox/py3.6-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.294062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.298062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:31.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:33.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:25.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:30.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:25.000000 djangosaml2-1.5.7/.tox/py3.6-django3.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:39.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      268 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      527 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1200 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      385 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      310 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2339 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3656 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      316 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3043 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2983 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      370 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1569 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2397 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2312 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2405 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4324 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      330 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      188 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3181 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      437 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1870 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1444 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      553 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      358 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      245 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1020 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1024 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      568 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      346 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1454 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.302062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      374 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      671 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2046 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      505 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      669 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      582 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      966 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1333 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1313 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      734 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1824 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1322 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      995 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1747 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1703 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      896 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1682 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1867 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      479 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.262062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      461 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    16595 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2453 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17182 2021-06-04 20:33:40.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.306062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:42.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:35.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:39.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:35.000000 djangosaml2-1.5.7/.tox/py3.7-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1245 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1686 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2262 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4341 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      361 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3051 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3258 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1550 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      518 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2426 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2341 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2561 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4485 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      338 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1787 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1861 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1912 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      276 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1472 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      214 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1044 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1052 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      341 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.310062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      592 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1980 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1382 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      885 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      185 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1897 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      431 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.314062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      462 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11150 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17606 2021-06-04 20:33:50.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13708 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3547 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3539 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10326 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2448 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-04 20:33:52.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:44.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2021-06-04 20:33:49.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:44.000000 djangosaml2-1.5.7/.tox/py3.7-django3.0/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   259465 2021-06-04 20:33:58.000000 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   263774 2021-06-04 20:33:54.000000 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2021-06-04 20:33:54.000000 djangosaml2-1.5.7/.tox/py3.7-django3.1/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    13512 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/CHANGES
--rw-rw-r--   0 wert      (1000) wert      (1000)    11358 2021-01-23 23:44:15.000000 djangosaml2-1.5.7/COPYING
--rw-rw-r--   0 wert      (1000) wert      (1000)      164 2021-01-23 23:44:15.000000 djangosaml2-1.5.7/MANIFEST.in
--rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)     1681 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/README.md
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/__init__.py
--rw-rw-r--   0 wert      (1000) wert      (1000)      190 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/apps.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    14380 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/backends.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     2894 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/cache.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     2568 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/conf.py
--rw-rw-r--   0 wert      (1000) wert      (1000)       51 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/exceptions.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     3511 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/middleware.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1045 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/overrides.py
--rw-rw-r--   0 wert      (1000) wert      (1000)      726 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/signals.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/djangosaml2/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/
--rw-rw-r--   0 wert      (1000) wert      (1000)      668 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/auth_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      561 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/echo_attributes.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      484 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/example_post_binding_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/login_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      763 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/logout_error.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      666 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templates/djangosaml2/wayf.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/djangosaml2/templatetags/
--rw-rw-r--   0 wert      (1000) wert      (1000)        0 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/templatetags/__init__.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/templatetags/idplist.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/djangosaml2/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)    42515 2023-05-07 19:41:25.000000 djangosaml2-1.5.7/djangosaml2/tests/__init__.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/
--rw-rw-r--   0 wert      (1000) wert      (1000)      555 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/django_saml_uri.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    11106 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/saml_uri.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     5095 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/auth_response.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     4177 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/conf.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/idpcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/idpcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/idpcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      997 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/mycert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/mycert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/mycert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)    13780 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_no_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3565 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_one_idp.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     3557 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_post_binding.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)    10380 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/remote_metadata_three_idps.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)     2466 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/tests/sp_metadata.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/spcert.csr
--rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/spcert.key
--rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/spcert.pem
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2021-06-16 13:28:16.000000 djangosaml2-1.5.7/djangosaml2/tests/utils.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     1190 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/urls.py
--rw-rw-r--   0 wert      (1000) wert      (1000)     6333 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/djangosaml2/utils.py
--rw-rw-r--   0 wert      (1000) wert      (1000)    33757 2023-05-07 19:41:25.000000 djangosaml2-1.5.7/djangosaml2/views.py
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.318062 djangosaml2-1.5.7/djangosaml2.egg-info/
--rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/PKG-INFO
--rw-rw-r--   0 wert      (1000) wert      (1000)   110776 2023-05-07 19:41:51.000000 djangosaml2-1.5.7/djangosaml2.egg-info/SOURCES.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/dependency_links.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/not-zip-safe
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/requires.txt
--rw-rw-r--   0 wert      (1000) wert      (1000)       12 2023-05-07 19:41:50.000000 djangosaml2-1.5.7/djangosaml2.egg-info/top_level.txt
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/docs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/docs/build/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/docs/build/html/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/docs/build/html/contents/
--rw-rw-r--   0 wert      (1000) wert      (1000)    12974 2021-04-04 23:22:05.000000 djangosaml2-1.5.7/docs/build/html/contents/developer.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     7950 2021-04-04 23:22:05.000000 djangosaml2-1.5.7/docs/build/html/contents/faq.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    15144 2021-04-04 23:22:05.000000 djangosaml2-1.5.7/docs/build/html/contents/miscellanea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    54956 2021-04-05 09:22:50.000000 djangosaml2-1.5.7/docs/build/html/contents/setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     8497 2021-04-05 09:22:28.000000 djangosaml2-1.5.7/docs/build/html/contents/usage.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6153 2021-04-05 09:22:50.000000 djangosaml2-1.5.7/docs/build/html/genindex.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    11611 2021-04-05 09:22:50.000000 djangosaml2-1.5.7/docs/build/html/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6624 2021-04-05 09:22:50.000000 djangosaml2-1.5.7/docs/build/html/search.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/docs/source/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/docs/source/_templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/docs/source/_templates/pplnx_template/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1829 2021-04-04 22:43:59.000000 djangosaml2-1.5.7/docs/source/_templates/pplnx_template/footer.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1486 2021-04-04 22:43:59.000000 djangosaml2-1.5.7/docs/source/_templates/pplnx_template/layout.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/coverage/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/coverage/htmlfiles/
--rw-rw-r--   0 wert      (1000) wert      (1000)     5400 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/coverage/htmlfiles/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6434 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/coverage/htmlfiles/pyfile.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)      282 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      551 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/500.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1235 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/actions.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      389 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1716 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/app_list.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/
--rw-rw-r--   0 wert      (1000) wert      (1000)      320 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2515 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     6110 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      448 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/base_site.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3019 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      403 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     3290 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1502 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/change_list_results.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      697 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/color_theme_toggle.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      453 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/date_hierarchy.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2539 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_confirmation.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2241 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2580 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     4086 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/filter.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/
--rw-rw-r--   0 wert      (1000) wert      (1000)     2200 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/fieldset.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      192 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1849 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      447 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/invalid_setup.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1899 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/login.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      486 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/nav_sidebar.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2136 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/object_history.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      549 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/pagination.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      327 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/popup_response.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      209 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1257 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/search_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1093 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/submit_line.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      618 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      339 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2096 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      238 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      218 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/admin/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.322062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/
--rw-rw-r--   0 wert      (1000) wert      (1000)      425 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/logged_out.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      745 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2428 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_change_form.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      417 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_complete.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1366 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      588 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_done.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      612 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      869 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admin/templates/registration/password_reset_form.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1281 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/bookmarklets.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1369 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      786 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/missing_docutils.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1880 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1346 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/model_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1049 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1775 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_filter_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1731 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/template_tag_index.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      928 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_detail.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1734 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/admindocs/templates/admin_doc/view_index.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      196 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/auth/templates/auth/widgets/read_only_password_hash.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/
--rw-rw-r--   0 wert      (1000) wert      (1000)     1441 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/openlayers.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      111 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/admin/osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers-osm.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     1587 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/gis/templates/gis/openlayers.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.266062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/jinja2/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/postgres/templates/postgres/widgets/split_array.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/sitemaps/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      683 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      360 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/contrib/sitemaps/templates/sitemap_index.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      865 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/div.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/
--rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/dict/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/
--rw-rw-r--   0 wert      (1000) wert      (1000)       49 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      119 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/errors/list/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/div.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       88 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       85 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/formsets/ul.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      147 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/label.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      673 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      814 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      712 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      395 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      365 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      110 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/jinja2/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/
--rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       40 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      874 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/div.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      137 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/dict/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      118 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/errors/list/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.326062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/
--rw-rw-r--   0 wert      (1000) wert      (1000)       77 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/default.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       84 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/div.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       82 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       86 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       83 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/formsets/ul.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      122 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/label.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      684 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/p.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      825 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/table.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      723 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/ul.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/
--rw-rw-r--   0 wert      (1000) wert      (1000)      172 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/attrs.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/checkbox_select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      511 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/clearable_file_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/datetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/email.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/file.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      189 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      219 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/input_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_hidden.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      426 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiple_input.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      117 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/multiwidget.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/number.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/password.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       57 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       55 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/radio_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      384 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_date.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      127 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/select_option.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splitdatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       54 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/splithiddendatetime.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/text.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      145 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/textarea.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/time.html
--rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/forms/templates/django/forms/widgets/url.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)    11184 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/default_urlconf.html
--rw-rw-r--   0 wert      (1000) wert      (1000)     2706 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/technical_404.html
--rw-rw-r--   0 wert      (1000) wert      (1000)    17662 2023-05-01 09:55:03.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/django/views/templates/technical_500.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/
--rw-rw-r--   0 wert      (1000) wert      (1000)    26094 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/SOURCES.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      968 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/dependency_links.html
--rw-rw-r--   0 wert      (1000) wert      (1000)      969 2023-05-01 09:54:30.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/docutils-0.19.dist-info/top_level.html
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/jeepney/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/jeepney/tests/
--rw-rw-r--   0 wert      (1000) wert      (1000)     4575 2023-05-07 19:41:47.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/pip/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/pip/_vendor/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-01 09:54:29.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/saml2/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/saml2/data/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/saml2/data/templates/
--rw-rw-r--   0 wert      (1000) wert      (1000)      769 2023-05-01 09:55:04.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/saml2/data/templates/template_enc.xml
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.270062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/setuptools/
-drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/env/lib/python3.10/site-packages/setuptools/command/
--rw-rw-r--   0 wert      (1000) wert      (1000)      628 2023-05-01 09:54:28.000000 djangosaml2-1.5.7/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
--rw-rw-r--   0 wert      (1000) wert      (1000)      439 2023-04-05 16:19:28.000000 djangosaml2-1.5.7/pyproject.toml
--rw-rw-r--   0 wert      (1000) wert      (1000)      197 2023-05-07 19:41:51.330062 djangosaml2-1.5.7/setup.cfg
--rw-rw-r--   0 wert      (1000) wert      (1000)     2436 2023-05-07 19:41:25.000000 djangosaml2-1.5.7/setup.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13512 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/CHANGES
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11358 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/COPYING
+-rw-rw-r--   0 wert      (1000) wert      (1000)      164 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/MANIFEST.in
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/PKG-INFO
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1681 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/README.md
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/__init__.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)      190 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/apps.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)    14380 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/backends.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2894 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/cache.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2568 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/conf.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)       51 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/exceptions.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3511 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/middleware.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1045 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/overrides.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)      726 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/signals.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/djangosaml2/templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      668 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/auth_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      561 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/echo_attributes.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      484 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/example_post_binding_form.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      378 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/login_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      763 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/logout_error.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)      666 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/wayf.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/templatetags/
+-rw-rw-r--   0 wert      (1000) wert      (1000)        0 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templatetags/__init__.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1490 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/templatetags/idplist.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)    42515 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/__init__.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      555 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/django_saml_uri.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)    11106 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/saml_uri.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     5095 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/auth_response.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4177 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/conf.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1005 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/idpcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/idpcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1204 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/idpcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      997 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/mycert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1679 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/mycert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1184 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/mycert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)    13780 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      165 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_no_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3565 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_one_idp.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3557 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_post_binding.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)    10380 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_three_idps.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2466 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/sp_metadata.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      968 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/spcert.csr
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1675 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/spcert.key
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1131 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/spcert.pem
+-rw-rw-r--   0 wert      (1000) wert      (1000)      417 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/tests/utils.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1190 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/urls.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)     6333 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/utils.py
+-rw-rw-r--   0 wert      (1000) wert      (1000)    33758 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/djangosaml2/views.py
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/djangosaml2.egg-info/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     3017 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/PKG-INFO
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2042 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/SOURCES.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/dependency_links.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)        1 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/not-zip-safe
+-rw-rw-r--   0 wert      (1000) wert      (1000)       48 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/requires.txt
+-rw-rw-r--   0 wert      (1000) wert      (1000)       12 2023-05-30 08:44:29.000000 djangosaml2-1.5.8/djangosaml2.egg-info/top_level.txt
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/docs/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/docs/source/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/docs/source/_templates/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/docs/source/_templates/pplnx_template/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1829 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/docs/source/_templates/pplnx_template/footer.html
+-rw-rw-r--   0 wert      (1000) wert      (1000)     1486 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/docs/source/_templates/pplnx_template/layout.html
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   278952 2023-05-30 08:44:24.000000 djangosaml2-1.5.8/env/lib/python3.10/site-packages/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/jeepney/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/jeepney/tests/
+-rw-rw-r--   0 wert      (1000) wert      (1000)     4575 2023-05-30 08:44:24.000000 djangosaml2-1.5.8/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/_vendor/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 wert      (1000) wert      (1000)   275233 2023-05-30 08:44:11.000000 djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.396716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/setuptools/
+drwxrwxr-x   0 wert      (1000) wert      (1000)        0 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/env/lib/python3.10/site-packages/setuptools/command/
+-rw-rw-r--   0 wert      (1000) wert      (1000)      628 2023-05-30 08:44:11.000000 djangosaml2-1.5.8/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      439 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/pyproject.toml
+-rw-rw-r--   0 wert      (1000) wert      (1000)      197 2023-05-30 08:44:29.400716 djangosaml2-1.5.8/setup.cfg
+-rw-rw-r--   0 wert      (1000) wert      (1000)     2436 2023-05-30 08:43:57.000000 djangosaml2-1.5.8/setup.py
```

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/certifi/cacert.pem` & `djangosaml2-1.5.8/env/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files 3% similar despite different names*

```diff
@@ -24,44 +24,14 @@
 yj1hTdNGCbM+w6DjY1Ub8rrvrTnhQ7k4o+YviiY776BQVvnGCv04zcQLcFGUl5gE
 38NflNUVyRRBnMRddWQVDf9VMOyGj/8N7yy5Y0b2qvzfvGn9LhJIZJrglfCm7ymP
 AbEVtQwdpf5pLGkkeB6zpxxxYu7KyJesF12KwvhHhm4qxFYxldBniYUr+WymXUad
 DKqC5JlR3XC321Y9YeRq4VzW9v493kHMB65jUr9TU/Qr6cf9tveCX4XSQRjbgbME
 HMUfpIBvFSDJ3gyICh3WZlXi/EjJKSZp4A==
 -----END CERTIFICATE-----
 
-# Issuer: CN=GlobalSign O=GlobalSign OU=GlobalSign Root CA - R2
-# Subject: CN=GlobalSign O=GlobalSign OU=GlobalSign Root CA - R2
-# Label: "GlobalSign Root CA - R2"
-# Serial: 4835703278459682885658125
-# MD5 Fingerprint: 94:14:77:7e:3e:5e:fd:8f:30:bd:41:b0:cf:e7:d0:30
-# SHA1 Fingerprint: 75:e0:ab:b6:13:85:12:27:1c:04:f8:5f:dd:de:38:e4:b7:24:2e:fe
-# SHA256 Fingerprint: ca:42:dd:41:74:5f:d0:b8:1e:b9:02:36:2c:f9:d8:bf:71:9d:a1:bd:1b:1e:fc:94:6f:5b:4c:99:f4:2c:1b:9e
------BEGIN CERTIFICATE-----
-MIIDujCCAqKgAwIBAgILBAAAAAABD4Ym5g0wDQYJKoZIhvcNAQEFBQAwTDEgMB4G
-A1UECxMXR2xvYmFsU2lnbiBSb290IENBIC0gUjIxEzARBgNVBAoTCkdsb2JhbFNp
-Z24xEzARBgNVBAMTCkdsb2JhbFNpZ24wHhcNMDYxMjE1MDgwMDAwWhcNMjExMjE1
-MDgwMDAwWjBMMSAwHgYDVQQLExdHbG9iYWxTaWduIFJvb3QgQ0EgLSBSMjETMBEG
-A1UEChMKR2xvYmFsU2lnbjETMBEGA1UEAxMKR2xvYmFsU2lnbjCCASIwDQYJKoZI
-hvcNAQEBBQADggEPADCCAQoCggEBAKbPJA6+Lm8omUVCxKs+IVSbC9N/hHD6ErPL
-v4dfxn+G07IwXNb9rfF73OX4YJYJkhD10FPe+3t+c4isUoh7SqbKSaZeqKeMWhG8
-eoLrvozps6yWJQeXSpkqBy+0Hne/ig+1AnwblrjFuTosvNYSuetZfeLQBoZfXklq
-tTleiDTsvHgMCJiEbKjNS7SgfQx5TfC4LcshytVsW33hoCmEofnTlEnLJGKRILzd
-C9XZzPnqJworc5HGnRusyMvo4KD0L5CLTfuwNhv2GXqF4G3yYROIXJ/gkwpRl4pa
-zq+r1feqCapgvdzZX99yqWATXgAByUr6P6TqBwMhAo6CygPCm48CAwEAAaOBnDCB
-mTAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUm+IH
-V2ccHsBqBt5ZtJot39wZhi4wNgYDVR0fBC8wLTAroCmgJ4YlaHR0cDovL2NybC5n
-bG9iYWxzaWduLm5ldC9yb290LXIyLmNybDAfBgNVHSMEGDAWgBSb4gdXZxwewGoG
-3lm0mi3f3BmGLjANBgkqhkiG9w0BAQUFAAOCAQEAmYFThxxol4aR7OBKuEQLq4Gs
-J0/WwbgcQ3izDJr86iw8bmEbTUsp9Z8FHSbBuOmDAGJFtqkIk7mpM0sYmsL4h4hO
-291xNBrBVNpGP+DTKqttVCL1OmLNIG+6KYnX3ZHu01yiPqFbQfXf5WRDLenVOavS
-ot+3i9DAgBkcRcAtjOj4LaR0VknFBbVPFd5uRHg5h6h+u/N5GJG79G+dwfCMNYxd
-AfvDbbnvRG15RjF+Cv6pgsH/76tuIMRQyV+dTZsXjAzlAcmgQWpzU/qlULRuJQ/7
-TBj0/VLZjmmx6BEP3ojY+x1J96relc8geMJgEtslQIxq/H5COEBkEveegeGTLg==
------END CERTIFICATE-----
-
 # Issuer: CN=Entrust.net Certification Authority (2048) O=Entrust.net OU=www.entrust.net/CPS_2048 incorp. by ref. (limits liab.)/(c) 1999 Entrust.net Limited
 # Subject: CN=Entrust.net Certification Authority (2048) O=Entrust.net OU=www.entrust.net/CPS_2048 incorp. by ref. (limits liab.)/(c) 1999 Entrust.net Limited
 # Label: "Entrust.net Premium 2048 Secure Server CA"
 # Serial: 946069240
 # MD5 Fingerprint: ee:29:31:bc:32:7e:9a:e6:e8:b5:f7:51:b4:34:71:90
 # SHA1 Fingerprint: 50:30:06:09:1d:97:d4:f5:ae:39:f7:cb:e7:92:7d:7d:65:2d:34:31
 # SHA256 Fingerprint: 6d:c4:71:72:e0:1c:bc:b0:bf:62:58:0d:89:5f:e2:b8:ac:9a:d4:f8:73:80:1e:0c:10:b9:c8:37:d2:1e:b1:77
@@ -487,42 +457,14 @@
 eM7b41N5cdblIZQB2lWHmiRk9opmzN6cN82oNLFpmyPInngiK3BD41VHMWEZ71jF
 hS9OMPagMRYjyOfiZRYzy78aG6A9+MpeizGLYAiJLQwGXFK3xPkKmNEVX58Svnw2
 Yzi9RKR/5CYrCsSXaQ3pjOLAEFe4yHYSkVXySGnYvCoCWw9E1CAx2/S6cCZdkGCe
 vEsXCS+0yx5DaMkHJ8HSXPfqIbloEpw8nL+e/IBcm2PN7EeqJSdnoDfzAIJ9VNep
 +OkuE6N36B9K
 -----END CERTIFICATE-----
 
-# Issuer: CN=DST Root CA X3 O=Digital Signature Trust Co.
-# Subject: CN=DST Root CA X3 O=Digital Signature Trust Co.
-# Label: "DST Root CA X3"
-# Serial: 91299735575339953335919266965803778155
-# MD5 Fingerprint: 41:03:52:dc:0f:f7:50:1b:16:f0:02:8e:ba:6f:45:c5
-# SHA1 Fingerprint: da:c9:02:4f:54:d8:f6:df:94:93:5f:b1:73:26:38:ca:6a:d7:7c:13
-# SHA256 Fingerprint: 06:87:26:03:31:a7:24:03:d9:09:f1:05:e6:9b:cf:0d:32:e1:bd:24:93:ff:c6:d9:20:6d:11:bc:d6:77:07:39
------BEGIN CERTIFICATE-----
-MIIDSjCCAjKgAwIBAgIQRK+wgNajJ7qJMDmGLvhAazANBgkqhkiG9w0BAQUFADA/
-MSQwIgYDVQQKExtEaWdpdGFsIFNpZ25hdHVyZSBUcnVzdCBDby4xFzAVBgNVBAMT
-DkRTVCBSb290IENBIFgzMB4XDTAwMDkzMDIxMTIxOVoXDTIxMDkzMDE0MDExNVow
-PzEkMCIGA1UEChMbRGlnaXRhbCBTaWduYXR1cmUgVHJ1c3QgQ28uMRcwFQYDVQQD
-Ew5EU1QgUm9vdCBDQSBYMzCCASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEB
-AN+v6ZdQCINXtMxiZfaQguzH0yxrMMpb7NnDfcdAwRgUi+DoM3ZJKuM/IUmTrE4O
-rz5Iy2Xu/NMhD2XSKtkyj4zl93ewEnu1lcCJo6m67XMuegwGMoOifooUMM0RoOEq
-OLl5CjH9UL2AZd+3UWODyOKIYepLYYHsUmu5ouJLGiifSKOeDNoJjj4XLh7dIN9b
-xiqKqy69cK3FCxolkHRyxXtqqzTWMIn/5WgTe1QLyNau7Fqckh49ZLOMxt+/yUFw
-7BZy1SbsOFU5Q9D8/RhcQPGX69Wam40dutolucbY38EVAjqr2m7xPi71XAicPNaD
-aeQQmxkqtilX4+U9m5/wAl0CAwEAAaNCMEAwDwYDVR0TAQH/BAUwAwEB/zAOBgNV
-HQ8BAf8EBAMCAQYwHQYDVR0OBBYEFMSnsaR7LHH62+FLkHX/xBVghYkQMA0GCSqG
-SIb3DQEBBQUAA4IBAQCjGiybFwBcqR7uKGY3Or+Dxz9LwwmglSBd49lZRNI+DT69
-ikugdB/OEIKcdBodfpga3csTS7MgROSR6cz8faXbauX+5v3gTt23ADq1cEmv8uXr
-AvHRAosZy5Q6XkjEGB5YGV8eAlrwDPGxrancWYaLbumR9YbK+rlmM6pZW87ipxZz
-R8srzJmwN0jP41ZL9c8PDHIyh8bwRLtTcm1D9SZImlJnt1ir/md2cXjbDaJWFBM5
-JDGFoqgCWjBH4d1QB7wCCZAA62RjYJsWvIjJEubSfZGL+T0yjWW06XyxV3bqxbYo
-Ob8VZRzI9neWagqNdwvYkQsEjgfbKbYK7p2CNTUQ
------END CERTIFICATE-----
-
 # Issuer: CN=SwissSign Gold CA - G2 O=SwissSign AG
 # Subject: CN=SwissSign Gold CA - G2 O=SwissSign AG
 # Label: "SwissSign Gold CA - G2"
 # Serial: 13492815561806991280
 # MD5 Fingerprint: 24:77:d9:a8:91:d1:3b:fa:88:2d:c2:ff:f8:cd:33:93
 # SHA1 Fingerprint: d8:c5:38:8a:b7:30:1b:1b:6e:d4:7a:e6:45:25:3a:6f:9f:1a:27:61
 # SHA256 Fingerprint: 62:dd:0b:e9:b9:f5:0a:16:3e:a0:f8:e7:5c:05:3b:1e:ca:57:ea:55:c8:68:8f:64:7c:68:81:f2:c8:35:7b:95
@@ -690,45 +632,14 @@
 IC9Bi5HcSEW88cbeunZrM8gALTFGTO3nnc+IlP8zwFboJIYmuNg4ON8qa90SzMc/
 RxdMosIGlgnW2/4/PEZB31jiVg88O8EckzXZOFKs7sjsLjBOlDW0JB9LeGna8gI4
 zJVSk/BwJVmcIGfE7vmLV2H0knZ9P4SNVbfo5azV8fUZVqZa+5Acr5Pr5RzUZ5dd
 BA6+C4OmF4O5MBKgxTMVBbkN+8cFduPYSo38NBejxiEovjBFMR7HeL5YYTisO+IB
 ZQ==
 -----END CERTIFICATE-----
 
-# Issuer: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Subject: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Label: "Network Solutions Certificate Authority"
-# Serial: 116697915152937497490437556386812487904
-# MD5 Fingerprint: d3:f3:a6:16:c0:fa:6b:1d:59:b1:2d:96:4d:0e:11:2e
-# SHA1 Fingerprint: 74:f8:a3:c3:ef:e7:b3:90:06:4b:83:90:3c:21:64:60:20:e5:df:ce
-# SHA256 Fingerprint: 15:f0:ba:00:a3:ac:7a:f3:ac:88:4c:07:2b:10:11:a0:77:bd:77:c0:97:f4:01:64:b2:f8:59:8a:bd:83:86:0c
------BEGIN CERTIFICATE-----
-MIID5jCCAs6gAwIBAgIQV8szb8JcFuZHFhfjkDFo4DANBgkqhkiG9w0BAQUFADBi
-MQswCQYDVQQGEwJVUzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMu
-MTAwLgYDVQQDEydOZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3Jp
-dHkwHhcNMDYxMjAxMDAwMDAwWhcNMjkxMjMxMjM1OTU5WjBiMQswCQYDVQQGEwJV
-UzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMuMTAwLgYDVQQDEydO
-ZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkwggEiMA0GCSqG
-SIb3DQEBAQUAA4IBDwAwggEKAoIBAQDkvH6SMG3G2I4rC7xGzuAnlt7e+foS0zwz
-c7MEL7xxjOWftiJgPl9dzgn/ggwbmlFQGiaJ3dVhXRncEg8tCqJDXRfQNJIg6nPP
-OCwGJgl6cvf6UDL4wpPTaaIjzkGxzOTVHzbRijr4jGPiFFlp7Q3Tf2vouAPlT2rl
-mGNpSAW+Lv8ztumXWWn4Zxmuk2GWRBXTcrA/vGp97Eh/jcOrqnErU2lBUzS1sLnF
-BgrEsEX1QV1uiUV7PTsmjHTC5dLRfbIR1PtYMiKagMnc/Qzpf14Dl847ABSHJ3A4
-qY5usyd2mFHgBeMhqxrVhSI8KbWaFsWAqPS7azCPL0YCorEMIuDTAgMBAAGjgZcw
-gZQwHQYDVR0OBBYEFCEwyfsA106Y2oeqKtCnLrFAMadMMA4GA1UdDwEB/wQEAwIB
-BjAPBgNVHRMBAf8EBTADAQH/MFIGA1UdHwRLMEkwR6BFoEOGQWh0dHA6Ly9jcmwu
-bmV0c29sc3NsLmNvbS9OZXR3b3JrU29sdXRpb25zQ2VydGlmaWNhdGVBdXRob3Jp
-dHkuY3JsMA0GCSqGSIb3DQEBBQUAA4IBAQC7rkvnt1frf6ott3NHhWrB5KUd5Oc8
-6fRZZXe1eltajSU24HqXLjjAV2CDmAaDn7l2em5Q4LqILPxFzBiwmZVRDuwduIj/
-h1AcgsLj4DKAv6ALR8jDMe+ZZzKATxcheQxpXN5eNK4CtSbqUN9/GGUsyfJj4akH
-/nxxH2szJGoeBfcFaMBqEssuXmHLrijTfsK0ZpEmXzwuJF/LWA/rKOyvEZbz3Htv
-wKeI8lN3s2Berq4o2jUsbzRF0ybh3uxbTydrFny9RAQYgrOJeRcQcT16ohZO9QHN
-pGxlaKFJdlxDydi8NmdspZS11My5vWo1ViHe2MPr+8ukYEywVaCge1ey
------END CERTIFICATE-----
-
 # Issuer: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Subject: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Label: "COMODO ECC Certification Authority"
 # Serial: 41578283867086692638256921589707938090
 # MD5 Fingerprint: 7c:62:ff:74:9d:31:53:5e:68:4a:d5:78:aa:1e:bf:23
 # SHA1 Fingerprint: 9f:74:4e:9f:2b:4d:ba:ec:0f:31:2c:50:b6:56:3b:8e:2d:93:c3:11
 # SHA256 Fingerprint: 17:93:92:7a:06:14:54:97:89:ad:ce:2f:8f:34:f7:f0:b6:6d:0f:3a:e3:a3:b8:4d:21:ec:15:db:ba:4f:ad:c7
@@ -775,44 +686,14 @@
 bV6lUmPOEvjvKtpv6zf+EwLHyzs+ImvaYS5/1HI93TDhHkxAGYwP15zRgzB7mFnc
 fca5DClMoTOi62c6ZYTTluLtdkVwj7Ur3vkj1kluPBS1xp81HlDQwY9qcEQCYsuu
 HWhBp6pX6FOqB9IG9tUUBguRA3UsbHK1YZWaDYu5Def131TN3ubY1gkIl2PlwS6w
 t0QmwCbAr1UwnjvVNioZBPRcHv/PLLf/0P2HQBHVESO7SMAhqaQoLf0V+LBOK/Qw
 WyH8EZE0vkHve52Xdf+XlcCWWC/qu0bXu+TZLg==
 -----END CERTIFICATE-----
 
-# Issuer: CN=Cybertrust Global Root O=Cybertrust, Inc
-# Subject: CN=Cybertrust Global Root O=Cybertrust, Inc
-# Label: "Cybertrust Global Root"
-# Serial: 4835703278459682877484360
-# MD5 Fingerprint: 72:e4:4a:87:e3:69:40:80:77:ea:bc:e3:f4:ff:f0:e1
-# SHA1 Fingerprint: 5f:43:e5:b1:bf:f8:78:8c:ac:1c:c7:ca:4a:9a:c6:22:2b:cc:34:c6
-# SHA256 Fingerprint: 96:0a:df:00:63:e9:63:56:75:0c:29:65:dd:0a:08:67:da:0b:9c:bd:6e:77:71:4a:ea:fb:23:49:ab:39:3d:a3
------BEGIN CERTIFICATE-----
-MIIDoTCCAomgAwIBAgILBAAAAAABD4WqLUgwDQYJKoZIhvcNAQEFBQAwOzEYMBYG
-A1UEChMPQ3liZXJ0cnVzdCwgSW5jMR8wHQYDVQQDExZDeWJlcnRydXN0IEdsb2Jh
-bCBSb290MB4XDTA2MTIxNTA4MDAwMFoXDTIxMTIxNTA4MDAwMFowOzEYMBYGA1UE
-ChMPQ3liZXJ0cnVzdCwgSW5jMR8wHQYDVQQDExZDeWJlcnRydXN0IEdsb2JhbCBS
-b290MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA+Mi8vRRQZhP/8NN5
-7CPytxrHjoXxEnOmGaoQ25yiZXRadz5RfVb23CO21O1fWLE3TdVJDm71aofW0ozS
-J8bi/zafmGWgE07GKmSb1ZASzxQG9Dvj1Ci+6A74q05IlG2OlTEQXO2iLb3VOm2y
-HLtgwEZLAfVJrn5GitB0jaEMAs7u/OePuGtm839EAL9mJRQr3RAwHQeWP032a7iP
-t3sMpTjr3kfb1V05/Iin89cqdPHoWqI7n1C6poxFNcJQZZXcY4Lv3b93TZxiyWNz
-FtApD0mpSPCzqrdsxacwOUBdrsTiXSZT8M4cIwhhqJQZugRiQOwfOHB3EgZxpzAY
-XSUnpQIDAQABo4GlMIGiMA4GA1UdDwEB/wQEAwIBBjAPBgNVHRMBAf8EBTADAQH/
-MB0GA1UdDgQWBBS2CHsNesysIEyGVjJez6tuhS1wVzA/BgNVHR8EODA2MDSgMqAw
-hi5odHRwOi8vd3d3Mi5wdWJsaWMtdHJ1c3QuY29tL2NybC9jdC9jdHJvb3QuY3Js
-MB8GA1UdIwQYMBaAFLYIew16zKwgTIZWMl7Pq26FLXBXMA0GCSqGSIb3DQEBBQUA
-A4IBAQBW7wojoFROlZfJ+InaRcHUowAl9B8Tq7ejhVhpwjCt2BWKLePJzYFa+HMj
-Wqd8BfP9IjsO0QbE2zZMcwSO5bAi5MXzLqXZI+O4Tkogp24CJJ8iYGd7ix1yCcUx
-XOl5n4BHPa2hCwcUPUf/A2kaDAtE52Mlp3+yybh2hO0j9n0Hq0V+09+zv+mKts2o
-omcrUtW3ZfA5TGOgkXmTUg9U3YO7n9GPp1Nzw8v/MOx8BLjYRB+TX3EJIrduPuoc
-A06dGiBh+4E37F78CkWr1+cXVdCg6mCbpvbjjFspwgZgFJ0tl0ypkxWdYcQBX0jW
-WL1WMRJOEcgh4LMRkWXbtKaIOM5V
------END CERTIFICATE-----
-
 # Issuer: O=Chunghwa Telecom Co., Ltd. OU=ePKI Root Certification Authority
 # Subject: O=Chunghwa Telecom Co., Ltd. OU=ePKI Root Certification Authority
 # Label: "ePKI Root Certification Authority"
 # Serial: 28956088682735189655030529057352760477
 # MD5 Fingerprint: 1b:2e:00:ca:26:06:90:3d:ad:fe:6f:15:68:d3:6b:b3
 # SHA1 Fingerprint: 67:65:0d:f1:7e:8e:7e:5b:82:40:a4:f4:56:4b:cf:e2:3d:69:c6:f0
 # SHA256 Fingerprint: c0:a6:f4:dc:63:a2:4b:fd:cf:54:ef:2a:6a:08:2a:0a:72:de:35:80:3e:2f:f5:ff:52:7a:e5:d8:72:06:df:d5
@@ -1407,86 +1288,14 @@
 coJxDjrSzG+ntKEju/Ykn8sX/oymzsLS28yN/HH8AynBbF0zX2S2ZTuJbxh2ePXc
 okgfGT+Ok+vx+hfuzU7jBBJV1uXk3fs+BXziHV7Gp7yXT2g69ekuCkO2r1dcYmh8
 t/2jioSgrGK+KwmHNPBqAbubKVY8/gA3zyNs8U6qtnRGEmyR7jTV7JqR50S+kDFy
 1UkC9gLl9B/rfNmWVan/7Ir5mUf/NVoCqgTLiluHcSmRvaS0eg29mvVXIwAHIRc/
 SjnRBUkLp7Y3gaVdjKozXoEofKd9J+sAro03
 -----END CERTIFICATE-----
 
-# Issuer: CN=EC-ACC O=Agencia Catalana de Certificacio (NIF Q-0801176-I) OU=Serveis Publics de Certificacio/Vegeu https://www.catcert.net/verarrel (c)03/Jerarquia Entitats de Certificacio Catalanes
-# Subject: CN=EC-ACC O=Agencia Catalana de Certificacio (NIF Q-0801176-I) OU=Serveis Publics de Certificacio/Vegeu https://www.catcert.net/verarrel (c)03/Jerarquia Entitats de Certificacio Catalanes
-# Label: "EC-ACC"
-# Serial: -23701579247955709139626555126524820479
-# MD5 Fingerprint: eb:f5:9d:29:0d:61:f9:42:1f:7c:c2:ba:6d:e3:15:09
-# SHA1 Fingerprint: 28:90:3a:63:5b:52:80:fa:e6:77:4c:0b:6d:a7:d6:ba:a6:4a:f2:e8
-# SHA256 Fingerprint: 88:49:7f:01:60:2f:31:54:24:6a:e2:8c:4d:5a:ef:10:f1:d8:7e:bb:76:62:6f:4a:e0:b7:f9:5b:a7:96:87:99
------BEGIN CERTIFICATE-----
-MIIFVjCCBD6gAwIBAgIQ7is969Qh3hSoYqwE893EATANBgkqhkiG9w0BAQUFADCB
-8zELMAkGA1UEBhMCRVMxOzA5BgNVBAoTMkFnZW5jaWEgQ2F0YWxhbmEgZGUgQ2Vy
-dGlmaWNhY2lvIChOSUYgUS0wODAxMTc2LUkpMSgwJgYDVQQLEx9TZXJ2ZWlzIFB1
-YmxpY3MgZGUgQ2VydGlmaWNhY2lvMTUwMwYDVQQLEyxWZWdldSBodHRwczovL3d3
-dy5jYXRjZXJ0Lm5ldC92ZXJhcnJlbCAoYykwMzE1MDMGA1UECxMsSmVyYXJxdWlh
-IEVudGl0YXRzIGRlIENlcnRpZmljYWNpbyBDYXRhbGFuZXMxDzANBgNVBAMTBkVD
-LUFDQzAeFw0wMzAxMDcyMzAwMDBaFw0zMTAxMDcyMjU5NTlaMIHzMQswCQYDVQQG
-EwJFUzE7MDkGA1UEChMyQWdlbmNpYSBDYXRhbGFuYSBkZSBDZXJ0aWZpY2FjaW8g
-KE5JRiBRLTA4MDExNzYtSSkxKDAmBgNVBAsTH1NlcnZlaXMgUHVibGljcyBkZSBD
-ZXJ0aWZpY2FjaW8xNTAzBgNVBAsTLFZlZ2V1IGh0dHBzOi8vd3d3LmNhdGNlcnQu
-bmV0L3ZlcmFycmVsIChjKTAzMTUwMwYDVQQLEyxKZXJhcnF1aWEgRW50aXRhdHMg
-ZGUgQ2VydGlmaWNhY2lvIENhdGFsYW5lczEPMA0GA1UEAxMGRUMtQUNDMIIBIjAN
-BgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAsyLHT+KXQpWIR4NA9h0X84NzJB5R
-85iKw5K4/0CQBXCHYMkAqbWUZRkiFRfCQ2xmRJoNBD45b6VLeqpjt4pEndljkYRm
-4CgPukLjbo73FCeTae6RDqNfDrHrZqJyTxIThmV6PttPB/SnCWDaOkKZx7J/sxaV
-HMf5NLWUhdWZXqBIoH7nF2W4onW4HvPlQn2v7fOKSGRdghST2MDk/7NQcvJ29rNd
-QlB50JQ+awwAvthrDk4q7D7SzIKiGGUzE3eeml0aE9jD2z3Il3rucO2n5nzbcc8t
-lGLfbdb1OL4/pYUKGbio2Al1QnDE6u/LDsg0qBIimAy4E5S2S+zw0JDnJwIDAQAB
-o4HjMIHgMB0GA1UdEQQWMBSBEmVjX2FjY0BjYXRjZXJ0Lm5ldDAPBgNVHRMBAf8E
-BTADAQH/MA4GA1UdDwEB/wQEAwIBBjAdBgNVHQ4EFgQUoMOLRKo3pUW/l4Ba0fF4
-opvpXY0wfwYDVR0gBHgwdjB0BgsrBgEEAfV4AQMBCjBlMCwGCCsGAQUFBwIBFiBo
-dHRwczovL3d3dy5jYXRjZXJ0Lm5ldC92ZXJhcnJlbDA1BggrBgEFBQcCAjApGidW
-ZWdldSBodHRwczovL3d3dy5jYXRjZXJ0Lm5ldC92ZXJhcnJlbCAwDQYJKoZIhvcN
-AQEFBQADggEBAKBIW4IB9k1IuDlVNZyAelOZ1Vr/sXE7zDkJlF7W2u++AVtd0x7Y
-/X1PzaBB4DSTv8vihpw3kpBWHNzrKQXlxJ7HNd+KDM3FIUPpqojlNcAZQmNaAl6k
-SBg6hW/cnbw/nZzBh7h6YQjpdwt/cKt63dmXLGQehb+8dJahw3oS7AwaboMMPOhy
-Rp/7SNVel+axofjk70YllJyJ22k4vuxcDlbHZVHlUIiIv0LVKz3l+bqeLrPK9HOS
-Agu+TGbrIP65y7WZf+a2E/rKS03Z7lNGBjvGTq2TWoF+bCpLagVFjPIhpDGQh2xl
-nJ2lYJU6Un/10asIbvPuW/mIPX64b24D5EI=
------END CERTIFICATE-----
-
-# Issuer: CN=Hellenic Academic and Research Institutions RootCA 2011 O=Hellenic Academic and Research Institutions Cert. Authority
-# Subject: CN=Hellenic Academic and Research Institutions RootCA 2011 O=Hellenic Academic and Research Institutions Cert. Authority
-# Label: "Hellenic Academic and Research Institutions RootCA 2011"
-# Serial: 0
-# MD5 Fingerprint: 73:9f:4c:4b:73:5b:79:e9:fa:ba:1c:ef:6e:cb:d5:c9
-# SHA1 Fingerprint: fe:45:65:9b:79:03:5b:98:a1:61:b5:51:2e:ac:da:58:09:48:22:4d
-# SHA256 Fingerprint: bc:10:4f:15:a4:8b:e7:09:dc:a5:42:a7:e1:d4:b9:df:6f:05:45:27:e8:02:ea:a9:2d:59:54:44:25:8a:fe:71
------BEGIN CERTIFICATE-----
-MIIEMTCCAxmgAwIBAgIBADANBgkqhkiG9w0BAQUFADCBlTELMAkGA1UEBhMCR1Ix
-RDBCBgNVBAoTO0hlbGxlbmljIEFjYWRlbWljIGFuZCBSZXNlYXJjaCBJbnN0aXR1
-dGlvbnMgQ2VydC4gQXV0aG9yaXR5MUAwPgYDVQQDEzdIZWxsZW5pYyBBY2FkZW1p
-YyBhbmQgUmVzZWFyY2ggSW5zdGl0dXRpb25zIFJvb3RDQSAyMDExMB4XDTExMTIw
-NjEzNDk1MloXDTMxMTIwMTEzNDk1MlowgZUxCzAJBgNVBAYTAkdSMUQwQgYDVQQK
-EztIZWxsZW5pYyBBY2FkZW1pYyBhbmQgUmVzZWFyY2ggSW5zdGl0dXRpb25zIENl
-cnQuIEF1dGhvcml0eTFAMD4GA1UEAxM3SGVsbGVuaWMgQWNhZGVtaWMgYW5kIFJl
-c2VhcmNoIEluc3RpdHV0aW9ucyBSb290Q0EgMjAxMTCCASIwDQYJKoZIhvcNAQEB
-BQADggEPADCCAQoCggEBAKlTAOMupvaO+mDYLZU++CwqVE7NuYRhlFhPjz2L5EPz
-dYmNUeTDN9KKiE15HrcS3UN4SoqS5tdI1Q+kOilENbgH9mgdVc04UfCMJDGFr4PJ
-fel3r+0ae50X+bOdOFAPplp5kYCvN66m0zH7tSYJnTxa71HFK9+WXesyHgLacEns
-bgzImjeN9/E2YEsmLIKe0HjzDQ9jpFEw4fkrJxIH2Oq9GGKYsFk3fb7u8yBRQlqD
-75O6aRXxYp2fmTmCobd0LovUxQt7L/DICto9eQqakxylKHJzkUOap9FNhYS5qXSP
-FEDH3N6sQWRstBmbAmNtJGSPRLIl6s5ddAxjMlyNh+UCAwEAAaOBiTCBhjAPBgNV
-HRMBAf8EBTADAQH/MAsGA1UdDwQEAwIBBjAdBgNVHQ4EFgQUppFC/RNhSiOeCKQp
-5dgTBCPuQSUwRwYDVR0eBEAwPqA8MAWCAy5ncjAFggMuZXUwBoIELmVkdTAGggQu
-b3JnMAWBAy5ncjAFgQMuZXUwBoEELmVkdTAGgQQub3JnMA0GCSqGSIb3DQEBBQUA
-A4IBAQAf73lB4XtuP7KMhjdCSk4cNx6NZrokgclPEg8hwAOXhiVtXdMiKahsog2p
-6z0GW5k6x8zDmjR/qw7IThzh+uTczQ2+vyT+bOdrwg3IBp5OjWEopmr95fZi6hg8
-TqBTnbI6nOulnJEWtk2C4AwFSKls9cz4y51JtPACpf1wA+2KIaWuE4ZJwzNzvoc7
-dIsXRSZMFpGD/md9zU1jZ/rzAxKWeAaNsWftjj++n08C9bMJL/NMh98qy5V8Acys
-Nnq/onN694/BtZqhFLKPM58N7yLcZnuEvUUXBj08yrl3NI/K6s8/MT7jiOOASSXI
-l7WdmplNsDz4SgCbZN2fOUvRJ9e4
------END CERTIFICATE-----
-
 # Issuer: CN=Actalis Authentication Root CA O=Actalis S.p.A./03358520967
 # Subject: CN=Actalis Authentication Root CA O=Actalis S.p.A./03358520967
 # Label: "Actalis Authentication Root CA"
 # Serial: 6271844772424770508
 # MD5 Fingerprint: 69:c1:0d:4f:07:a3:1b:c3:fe:56:3d:04:bc:11:f6:a6
 # SHA1 Fingerprint: f3:73:b3:87:06:5a:28:84:8a:f2:f3:4a:ce:19:2b:dd:c7:8e:9c:ac
 # SHA256 Fingerprint: 55:92:60:84:ec:96:3a:64:b9:6e:2a:be:01:ce:0b:a8:6a:64:fb:fe:bc:c7:aa:b5:af:c1:55:b3:7f:d7:60:66
@@ -2338,35 +2147,14 @@
 o4N+LZfQYcTxmdwlkWOrfzCjtHDix6EznPO/LlxTsV+zfTJ/ijTjeXmjQjBAMB0G
 A1UdDgQWBBQ64QmG1M8ZwpZ2dEl23OA1xmNjmjAOBgNVHQ8BAf8EBAMCAQYwDwYD
 VR0TAQH/BAUwAwEB/zAKBggqhkjOPQQDAwNoADBlAjA2Z6EWCNzklwBBHU6+4WMB
 zzuqQhFkoJ2UOQIReVx7Hfpkue4WQrO/isIJxOzksU0CMQDpKmFHjFJKS04YcPbW
 RNZu9YO6bVi9JNlWSOrvxKJGgYhqOkbRqZtNyWHa0V1Xahg=
 -----END CERTIFICATE-----
 
-# Issuer: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R4
-# Subject: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R4
-# Label: "GlobalSign ECC Root CA - R4"
-# Serial: 14367148294922964480859022125800977897474
-# MD5 Fingerprint: 20:f0:27:68:d1:7e:a0:9d:0e:e6:2a:ca:df:5c:89:8e
-# SHA1 Fingerprint: 69:69:56:2e:40:80:f4:24:a1:e7:19:9f:14:ba:f3:ee:58:ab:6a:bb
-# SHA256 Fingerprint: be:c9:49:11:c2:95:56:76:db:6c:0a:55:09:86:d7:6e:3b:a0:05:66:7c:44:2c:97:62:b4:fb:b7:73:de:22:8c
------BEGIN CERTIFICATE-----
-MIIB4TCCAYegAwIBAgIRKjikHJYKBN5CsiilC+g0mAIwCgYIKoZIzj0EAwIwUDEk
-MCIGA1UECxMbR2xvYmFsU2lnbiBFQ0MgUm9vdCBDQSAtIFI0MRMwEQYDVQQKEwpH
-bG9iYWxTaWduMRMwEQYDVQQDEwpHbG9iYWxTaWduMB4XDTEyMTExMzAwMDAwMFoX
-DTM4MDExOTAzMTQwN1owUDEkMCIGA1UECxMbR2xvYmFsU2lnbiBFQ0MgUm9vdCBD
-QSAtIFI0MRMwEQYDVQQKEwpHbG9iYWxTaWduMRMwEQYDVQQDEwpHbG9iYWxTaWdu
-MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEuMZ5049sJQ6fLjkZHAOkrprlOQcJ
-FspjsbmG+IpXwVfOQvpzofdlQv8ewQCybnMO/8ch5RikqtlxP6jUuc6MHaNCMEAw
-DgYDVR0PAQH/BAQDAgEGMA8GA1UdEwEB/wQFMAMBAf8wHQYDVR0OBBYEFFSwe61F
-uOJAf/sKbvu+M8k8o4TVMAoGCCqGSM49BAMCA0gAMEUCIQDckqGgE6bPA7DmxCGX
-kPoUVy0D7O48027KqGx2vKLeuwIgJ6iFJzWbVsaj8kfSt24bAgAXqmemFZHe+pTs
-ewv4n4Q=
------END CERTIFICATE-----
-
 # Issuer: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R5
 # Subject: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R5
 # Label: "GlobalSign ECC Root CA - R5"
 # Serial: 32785792099990507226680698011560947931244
 # MD5 Fingerprint: 9f:ad:3b:1c:02:1e:8a:ba:17:74:38:81:0c:a2:bc:08
 # SHA1 Fingerprint: 1f:24:c6:30:cd:a4:18:ef:20:69:ff:ad:4f:dd:5f:46:3a:1b:69:aa
 # SHA256 Fingerprint: 17:9f:bc:14:8a:3d:d0:0f:d2:4e:a1:34:58:cc:43:bf:a7:f5:9c:81:82:d7:83:a5:13:f6:eb:ec:10:0c:89:24
@@ -2381,54 +2169,14 @@
 hOvRnkmSh5SHDDqFSmafnVmTTZdhBoZKo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYD
 VR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUPeYpSJvqB8ohREom3m7e0oPQn1kwCgYI
 KoZIzj0EAwMDaAAwZQIxAOVpEslu28YxuglB4Zf4+/2a4n0Sye18ZNPLBSWLVtmg
 515dTguDnFt2KaAJJiFqYgIwcdK1j1zqO+F4CYWodZI7yFz9SO8NdCKoCOJuxUnO
 xwy8p2Fp8fc74SrL+SvzZpA3
 -----END CERTIFICATE-----
 
-# Issuer: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Subject: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Label: "Staat der Nederlanden EV Root CA"
-# Serial: 10000013
-# MD5 Fingerprint: fc:06:af:7b:e8:1a:f1:9a:b4:e8:d2:70:1f:c0:f5:ba
-# SHA1 Fingerprint: 76:e2:7e:c1:4f:db:82:c1:c0:a6:75:b5:05:be:3d:29:b4:ed:db:bb
-# SHA256 Fingerprint: 4d:24:91:41:4c:fe:95:67:46:ec:4c:ef:a6:cf:6f:72:e2:8a:13:29:43:2f:9d:8a:90:7a:c4:cb:5d:ad:c1:5a
------BEGIN CERTIFICATE-----
-MIIFcDCCA1igAwIBAgIEAJiWjTANBgkqhkiG9w0BAQsFADBYMQswCQYDVQQGEwJO
-TDEeMBwGA1UECgwVU3RhYXQgZGVyIE5lZGVybGFuZGVuMSkwJwYDVQQDDCBTdGFh
-dCBkZXIgTmVkZXJsYW5kZW4gRVYgUm9vdCBDQTAeFw0xMDEyMDgxMTE5MjlaFw0y
-MjEyMDgxMTEwMjhaMFgxCzAJBgNVBAYTAk5MMR4wHAYDVQQKDBVTdGFhdCBkZXIg
-TmVkZXJsYW5kZW4xKTAnBgNVBAMMIFN0YWF0IGRlciBOZWRlcmxhbmRlbiBFViBS
-b290IENBMIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEA48d+ifkkSzrS
-M4M1LGns3Amk41GoJSt5uAg94JG6hIXGhaTK5skuU6TJJB79VWZxXSzFYGgEt9nC
-UiY4iKTWO0Cmws0/zZiTs1QUWJZV1VD+hq2kY39ch/aO5ieSZxeSAgMs3NZmdO3d
-Z//BYY1jTw+bbRcwJu+r0h8QoPnFfxZpgQNH7R5ojXKhTbImxrpsX23Wr9GxE46p
-rfNeaXUmGD5BKyF/7otdBwadQ8QpCiv8Kj6GyzyDOvnJDdrFmeK8eEEzduG/L13l
-pJhQDBXd4Pqcfzho0LKmeqfRMb1+ilgnQ7O6M5HTp5gVXJrm0w912fxBmJc+qiXb
-j5IusHsMX/FjqTf5m3VpTCgmJdrV8hJwRVXj33NeN/UhbJCONVrJ0yPr08C+eKxC
-KFhmpUZtcALXEPlLVPxdhkqHz3/KRawRWrUgUY0viEeXOcDPusBCAUCZSCELa6fS
-/ZbV0b5GnUngC6agIk440ME8MLxwjyx1zNDFjFE7PZQIZCZhfbnDZY8UnCHQqv0X
-cgOPvZuM5l5Tnrmd74K74bzickFbIZTTRTeU0d8JOV3nI6qaHcptqAqGhYqCvkIH
-1vI4gnPah1vlPNOePqc7nvQDs/nxfRN0Av+7oeX6AHkcpmZBiFxgV6YuCcS6/ZrP
-px9Aw7vMWgpVSzs4dlG4Y4uElBbmVvMCAwEAAaNCMEAwDwYDVR0TAQH/BAUwAwEB
-/zAOBgNVHQ8BAf8EBAMCAQYwHQYDVR0OBBYEFP6rAJCYniT8qcwaivsnuL8wbqg7
-MA0GCSqGSIb3DQEBCwUAA4ICAQDPdyxuVr5Os7aEAJSrR8kN0nbHhp8dB9O2tLsI
-eK9p0gtJ3jPFrK3CiAJ9Brc1AsFgyb/E6JTe1NOpEyVa/m6irn0F3H3zbPB+po3u
-2dfOWBfoqSmuc0iH55vKbimhZF8ZE/euBhD/UcabTVUlT5OZEAFTdfETzsemQUHS
-v4ilf0X8rLiltTMMgsT7B/Zq5SWEXwbKwYY5EdtYzXc7LMJMD16a4/CrPmEbUCTC
-wPTxGfARKbalGAKb12NMcIxHowNDXLldRqANb/9Zjr7dn3LDWyvfjFvO5QxGbJKy
-CqNMVEIYFRIYvdr8unRu/8G2oGTYqV9Vrp9canaW2HNnh/tNf1zuacpzEPuKqf2e
-vTY4SUmH9A4U8OmHuD+nT3pajnnUk+S7aFKErGzp85hwVXIy+TSrK0m1zSBi5Dp6
-Z2Orltxtrpfs/J92VoguZs9btsmksNcFuuEnL5O7Jiqik7Ab846+HUCjuTaPPoIa
-Gl6I6lD4WeKDRikL40Rc4ZW2aZCaFG+XroHPaO+Zmr615+F/+PoTRxZMzG0IQOeL
-eG9QgkRQP2YGiqtDhFZKDyAthg710tvSeopLzaXoTvFeJiUBWSOgftL2fiFX1ye8
-FVdMpEbB4IMeDExNH08GGeL5qPQ6gqGyeUN51q1veieQA6TqJIc/2b3Z6fJfUEkc
-7uzXLg==
------END CERTIFICATE-----
-
 # Issuer: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Subject: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Label: "IdenTrust Commercial Root CA 1"
 # Serial: 13298821034946342390520003877796839426
 # MD5 Fingerprint: b3:3e:77:73:75:ee:a0:d3:e3:7e:49:63:49:59:bb:c7
 # SHA1 Fingerprint: df:71:7e:aa:4a:d9:4e:c9:55:84:99:60:2d:48:de:5f:bc:f0:3a:25
 # SHA256 Fingerprint: 5d:56:49:9b:e4:d2:e0:8b:cf:ca:d0:8a:3e:38:72:3d:50:50:3b:de:70:69:48:e4:2f:55:60:30:19:e5:28:ae
@@ -3028,124 +2776,14 @@
 2c9Si1vIY9RCPqAzekYu9wogRlR+ak8x8YF+QnQ4ZXMn7sZ8uI7XpTrXmKGcjBBV
 09tL7ECQ8s1uV9JiDnxXk7Gnbc2dg7sq5+W2O3FYrf3RRbxake5TFW/TRQl1brqQ
 XR4EzzffHqhmsYzmIGrv/EhOdJhCrylvLmrH+33RZjEizIYAfmaDDEL0vTSSwxrq
 T8p+ck0LcIymSLumoRT2+1hEmRSuqguTaaApJUqlyyvdimYHFngVV3Eb7PVHhPOe
 MTd61X8kreS8/f3MboPoDKi3QWwH3b08hpcv0g==
 -----END CERTIFICATE-----
 
-# Issuer: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-1"
-# Serial: 15752444095811006489
-# MD5 Fingerprint: 6e:85:f1:dc:1a:00:d3:22:d5:b2:b2:ac:6b:37:05:45
-# SHA1 Fingerprint: ff:bd:cd:e7:82:c8:43:5e:3c:6f:26:86:5c:ca:a8:3a:45:5b:c3:0a
-# SHA256 Fingerprint: d4:0e:9c:86:cd:8f:e4:68:c1:77:69:59:f4:9e:a7:74:fa:54:86:84:b6:c4:06:f3:90:92:61:f4:dc:e2:57:5c
------BEGIN CERTIFICATE-----
-MIIEMDCCAxigAwIBAgIJANqb7HHzA7AZMA0GCSqGSIb3DQEBCwUAMIGkMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRydXN0Q29y
-IFJvb3RDZXJ0IENBLTEwHhcNMTYwMjA0MTIzMjE2WhcNMjkxMjMxMTcyMzE2WjCB
-pDELMAkGA1UEBhMCUEExDzANBgNVBAgMBlBhbmFtYTEUMBIGA1UEBwwLUGFuYW1h
-IENpdHkxJDAiBgNVBAoMG1RydXN0Q29yIFN5c3RlbXMgUy4gZGUgUi5MLjEnMCUG
-A1UECwweVHJ1c3RDb3IgQ2VydGlmaWNhdGUgQXV0aG9yaXR5MR8wHQYDVQQDDBZU
-cnVzdENvciBSb290Q2VydCBDQS0xMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
-CgKCAQEAv463leLCJhJrMxnHQFgKq1mqjQCj/IDHUHuO1CAmujIS2CNUSSUQIpid
-RtLByZ5OGy4sDjjzGiVoHKZaBeYei0i/mJZ0PmnK6bV4pQa81QBeCQryJ3pS/C3V
-seq0iWEk8xoT26nPUu0MJLq5nux+AHT6k61sKZKuUbS701e/s/OojZz0JEsq1pme
-9J7+wH5COucLlVPat2gOkEz7cD+PSiyU8ybdY2mplNgQTsVHCJCZGxdNuWxu72CV
-EY4hgLW9oHPY0LJ3xEXqWib7ZnZ2+AYfYW0PVcWDtxBWcgYHpfOxGgMFZA6dWorW
-hnAbJN7+KIor0Gqw/Hqi3LJ5DotlDwIDAQABo2MwYTAdBgNVHQ4EFgQU7mtJPHo/
-DeOxCbeKyKsZn3MzUOcwHwYDVR0jBBgwFoAU7mtJPHo/DeOxCbeKyKsZn3MzUOcw
-DwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYwDQYJKoZIhvcNAQELBQAD
-ggEBACUY1JGPE+6PHh0RU9otRCkZoB5rMZ5NDp6tPVxBb5UrJKF5mDo4Nvu7Zp5I
-/5CQ7z3UuJu0h3U/IJvOcs+hVcFNZKIZBqEHMwwLKeXx6quj7LUKdJDHfXLy11yf
-ke+Ri7fc7Waiz45mO7yfOgLgJ90WmMCV1Aqk5IGadZQ1nJBfiDcGrVmVCrDRZ9MZ
-yonnMlo2HD6CqFqTvsbQZJG2z9m2GM/bftJlo6bEjhcxwft+dtvTheNYsnd6djts
-L1Ac59v2Z3kf9YKVmgenFK+P3CghZwnS1k1aHBkcjndcw5QkPTJrS37UeJSDvjdN
-zl/HHk484IkzlQsPpTLWPFp5LBk=
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-2"
-# Serial: 2711694510199101698
-# MD5 Fingerprint: a2:e1:f8:18:0b:ba:45:d5:c7:41:2a:bb:37:52:45:64
-# SHA1 Fingerprint: b8:be:6d:cb:56:f1:55:b9:63:d4:12:ca:4e:06:34:c7:94:b2:1c:c0
-# SHA256 Fingerprint: 07:53:e9:40:37:8c:1b:d5:e3:83:6e:39:5d:ae:a5:cb:83:9e:50:46:f1:bd:0e:ae:19:51:cf:10:fe:c7:c9:65
------BEGIN CERTIFICATE-----
-MIIGLzCCBBegAwIBAgIIJaHfyjPLWQIwDQYJKoZIhvcNAQELBQAwgaQxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEfMB0GA1UEAwwWVHJ1c3RDb3Ig
-Um9vdENlcnQgQ0EtMjAeFw0xNjAyMDQxMjMyMjNaFw0zNDEyMzExNzI2MzlaMIGk
-MQswCQYDVQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEg
-Q2l0eTEkMCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYD
-VQQLDB5UcnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRy
-dXN0Q29yIFJvb3RDZXJ0IENBLTIwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIK
-AoICAQCnIG7CKqJiJJWQdsg4foDSq8GbZQWU9MEKENUCrO2fk8eHyLAnK0IMPQo+
-QVqedd2NyuCb7GgypGmSaIwLgQ5WoD4a3SwlFIIvl9NkRvRUqdw6VC0xK5mC8tkq
-1+9xALgxpL56JAfDQiDyitSSBBtlVkxs1Pu2YVpHI7TYabS3OtB0PAx1oYxOdqHp
-2yqlO/rOsP9+aij9JxzIsekp8VduZLTQwRVtDr4uDkbIXvRR/u8OYzo7cbrPb1nK
-DOObXUm4TOJXsZiKQlecdu/vvdFoqNL0Cbt3Nb4lggjEFixEIFapRBF37120Hape
-az6LMvYHL1cEksr1/p3C6eizjkxLAjHZ5DxIgif3GIJ2SDpxsROhOdUuxTTCHWKF
-3wP+TfSvPd9cW436cOGlfifHhi5qjxLGhF5DUVCcGZt45vz27Ud+ez1m7xMTiF88
-oWP7+ayHNZ/zgp6kPwqcMWmLmaSISo5uZk3vFsQPeSghYA2FFn3XVDjxklb9tTNM
-g9zXEJ9L/cb4Qr26fHMC4P99zVvh1Kxhe1fVSntb1IVYJ12/+CtgrKAmrhQhJ8Z3
-mjOAPF5GP/fDsaOGM8boXg25NSyqRsGFAnWAoOsk+xWq5Gd/bnc/9ASKL3x74xdh
-8N0JqSDIvgmk0H5Ew7IwSjiqqewYmgeCK9u4nBit2uBGF6zPXQIDAQABo2MwYTAd
-BgNVHQ4EFgQU2f4hQG6UnrybPZx9mCAZ5YwwYrIwHwYDVR0jBBgwFoAU2f4hQG6U
-nrybPZx9mCAZ5YwwYrIwDwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYw
-DQYJKoZIhvcNAQELBQADggIBAJ5Fngw7tu/hOsh80QA9z+LqBrWyOrsGS2h60COX
-dKcs8AjYeVrXWoSK2BKaG9l9XE1wxaX5q+WjiYndAfrs3fnpkpfbsEZC89NiqpX+
-MWcUaViQCqoL7jcjx1BRtPV+nuN79+TMQjItSQzL/0kMmx40/W5ulop5A7Zv2wnL
-/V9lFDfhOPXzYRZY5LVtDQsEGz9QLX+zx3oaFoBg+Iof6Rsqxvm6ARppv9JYx1RX
-CI/hOWB3S6xZhBqI8d3LT3jX5+EzLfzuQfogsL7L9ziUwOHQhQ+77Sxzq+3+knYa
-ZH9bDTMJBzN7Bj8RpFxwPIXAz+OQqIN3+tvmxYxoZxBnpVIt8MSZj3+/0WvitUfW
-2dCFmU2Umw9Lje4AWkcdEQOsQRivh7dvDDqPys/cA8GiCcjl/YBeyGBCARsaU1q7
-N6a3vLqE6R5sGtRk2tRD/pOLS/IseRYQ1JMLiI+h2IYURpFHmygk71dSTlxCnKr3
-Sewn6EAes6aJInKc9Q0ztFijMDvd1GpUk74aTfOTlPf8hAs/hCBcNANExdqtvArB
-As8e5ZTZ845b2EzwnexhF7sUMlQMAimTHpKG9n/v55IFDlndmQguLvqcAFLTxWYp
-5KeXRKQOKIETNcX2b2TmQcTVL8w0RSXPQQCWPUouwpaYT05KnJe32x+SMsj/D1Fu
-1uwJ
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor ECA-1"
-# Serial: 9548242946988625984
-# MD5 Fingerprint: 27:92:23:1d:0a:f5:40:7c:e9:e6:6b:9d:d8:f5:e7:6c
-# SHA1 Fingerprint: 58:d1:df:95:95:67:6b:63:c0:f0:5b:1c:17:4d:8b:84:0b:c8:78:bd
-# SHA256 Fingerprint: 5a:88:5d:b1:9c:01:d9:12:c5:75:93:88:93:8c:af:bb:df:03:1a:b2:d4:8e:91:ee:15:58:9b:42:97:1d:03:9c
------BEGIN CERTIFICATE-----
-MIIEIDCCAwigAwIBAgIJAISCLF8cYtBAMA0GCSqGSIb3DQEBCwUAMIGcMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxFzAVBgNVBAMMDlRydXN0Q29y
-IEVDQS0xMB4XDTE2MDIwNDEyMzIzM1oXDTI5MTIzMTE3MjgwN1owgZwxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEXMBUGA1UEAwwOVHJ1c3RDb3Ig
-RUNBLTEwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDPj+ARtZ+odnbb
-3w9U73NjKYKtR8aja+3+XzP4Q1HpGjORMRegdMTUpwHmspI+ap3tDvl0mEDTPwOA
-BoJA6LHip1GnHYMma6ve+heRK9jGrB6xnhkB1Zem6g23xFUfJ3zSCNV2HykVh0A5
-3ThFEXXQmqc04L/NyFIduUd+Dbi7xgz2c1cWWn5DkR9VOsZtRASqnKmcp0yJF4Ou
-owReUoCLHhIlERnXDH19MURB6tuvsBzvgdAsxZohmz3tQjtQJvLsznFhBmIhVE5/
-wZ0+fyCMgMsq2JdiyIMzkX2woloPV+g7zPIlstR8L+xNxqE6FXrntl019fZISjZF
-ZtS6mFjBAgMBAAGjYzBhMB0GA1UdDgQWBBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAf
-BgNVHSMEGDAWgBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAPBgNVHRMBAf8EBTADAQH/
-MA4GA1UdDwEB/wQEAwIBhjANBgkqhkiG9w0BAQsFAAOCAQEABT41XBVwm8nHc2Fv
-civUwo/yQ10CzsSUuZQRg2dd4mdsdXa/uwyqNsatR5Nj3B5+1t4u/ukZMjgDfxT2
-AHMsWbEhBuH7rBiVDKP/mZb3Kyeb1STMHd3BOuCYRLDE5D53sXOpZCz2HAF8P11F
-hcCF5yWPldwX8zyfGm6wyuMdKulMY/okYWLW2n62HGz1Ah3UKt1VkOsqEUc8Ll50
-soIipX1TH0XsJ5F95yIW6MBoNtjG8U+ARDL54dHRHareqKucBK+tIA5kmE2la8BI
-WJZpTdwHjFGTot+fDz2LYLSCjaoITmJF4PkL0uDgPFveXHEnJcLmA4GLEFPjx1Wi
-tJ/X5g==
------END CERTIFICATE-----
-
 # Issuer: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Subject: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Label: "SSL.com Root Certification Authority RSA"
 # Serial: 8875640296558310041
 # MD5 Fingerprint: 86:69:12:c0:70:f1:ec:ac:ac:c2:d5:bc:a5:5b:a1:29
 # SHA1 Fingerprint: b7:ab:33:08:d1:ea:44:77:ba:14:80:12:5a:6f:bd:a9:36:49:0c:bb
 # SHA256 Fingerprint: 85:66:6a:56:2e:e0:be:5c:e9:25:c1:d8:89:0a:6f:76:a8:7e:c1:6d:4d:7d:5f:29:ea:74:19:cf:20:12:3b:69
@@ -3333,134 +2971,14 @@
 p2OQ0jnUsYd4XxiWD1AbNTcPasbc2RNNpI6QN+a9WzGRo1QwUjAOBgNVHQ8BAf8E
 BAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUSIcUrOPDnpBgOtfKie7T
 rYy0UGYwEAYJKwYBBAGCNxUBBAMCAQAwCgYIKoZIzj0EAwMDaAAwZQIwJsdpW9zV
 57LnyAyMjMPdeYwbY9XJUpROTYJKcx6ygISpJcBMWm1JKWB4E+J+SOtkAjEA2zQg
 Mgj/mkkCtojeFK9dbJlxjRo/i9fgojaGHAeCOnZT/cKi7e97sIBPWA9LUzm9
 -----END CERTIFICATE-----
 
-# Issuer: CN=GTS Root R1 O=Google Trust Services LLC
-# Subject: CN=GTS Root R1 O=Google Trust Services LLC
-# Label: "GTS Root R1"
-# Serial: 146587175971765017618439757810265552097
-# MD5 Fingerprint: 82:1a:ef:d4:d2:4a:f2:9f:e2:3d:97:06:14:70:72:85
-# SHA1 Fingerprint: e1:c9:50:e6:ef:22:f8:4c:56:45:72:8b:92:20:60:d7:d5:a7:a3:e8
-# SHA256 Fingerprint: 2a:57:54:71:e3:13:40:bc:21:58:1c:bd:2c:f1:3e:15:84:63:20:3e:ce:94:bc:f9:d3:cc:19:6b:f0:9a:54:72
------BEGIN CERTIFICATE-----
-MIIFWjCCA0KgAwIBAgIQbkepxUtHDA3sM9CJuRz04TANBgkqhkiG9w0BAQwFADBH
-MQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExM
-QzEUMBIGA1UEAxMLR1RTIFJvb3QgUjEwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIy
-MDAwMDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNl
-cnZpY2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjEwggIiMA0GCSqGSIb3DQEB
-AQUAA4ICDwAwggIKAoICAQC2EQKLHuOhd5s73L+UPreVp0A8of2C+X0yBoJx9vaM
-f/vo27xqLpeXo4xL+Sv2sfnOhB2x+cWX3u+58qPpvBKJXqeqUqv4IyfLpLGcY9vX
-mX7wCl7raKb0xlpHDU0QM+NOsROjyBhsS+z8CZDfnWQpJSMHobTSPS5g4M/SCYe7
-zUjwTcLCeoiKu7rPWRnWr4+wB7CeMfGCwcDfLqZtbBkOtdh+JhpFAz2weaSUKK0P
-fyblqAj+lug8aJRT7oM6iCsVlgmy4HqMLnXWnOunVmSPlk9orj2XwoSPwLxAwAtc
-vfaHszVsrBhQf4TgTM2S0yDpM7xSma8ytSmzJSq0SPly4cpk9+aCEI3oncKKiPo4
-Zor8Y/kB+Xj9e1x3+naH+uzfsQ55lVe0vSbv1gHR6xYKu44LtcXFilWr06zqkUsp
-zBmkMiVOKvFlRNACzqrOSbTqn3yDsEB750Orp2yjj32JgfpMpf/VjsPOS+C12LOO
-Rc92wO1AK/1TD7Cn1TsNsYqiA94xrcx36m97PtbfkSIS5r762DL8EGMUUXLeXdYW
-k70paDPvOmbsB4om3xPXV2V4J95eSRQAogB/mqghtqmxlbCluQ0WEdrHbEg8QOB+
-DVrNVjzRlwW5y0vtOUucxD/SVRNuJLDWcfr0wbrM7Rv1/oFB2ACYPTrIrnqYNxgF
-lQIDAQABo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNV
-HQ4EFgQU5K8rJnEaK0gnhS9SZizv8IkTcT4wDQYJKoZIhvcNAQEMBQADggIBADiW
-Cu49tJYeX++dnAsznyvgyv3SjgofQXSlfKqE1OXyHuY3UjKcC9FhHb8owbZEKTV1
-d5iyfNm9dKyKaOOpMQkpAWBz40d8U6iQSifvS9efk+eCNs6aaAyC58/UEBZvXw6Z
-XPYfcX3v73svfuo21pdwCxXu11xWajOl40k4DLh9+42FpLFZXvRq4d2h9mREruZR
-gyFmxhE+885H7pwoHyXa/6xmld01D1zvICxi/ZG6qcz8WpyTgYMpl0p8WnK0OdC3
-d8t5/Wk6kjftbjhlRn7pYL15iJdfOBL07q9bgsiG1eGZbYwE8na6SfZu6W0eX6Dv
-J4J2QPim01hcDyxC2kLGe4g0x8HYRZvBPsVhHdljUEn2NIVq4BjFbkerQUIpm/Zg
-DdIx02OYI5NaAIFItO/Nis3Jz5nu2Z6qNuFoS3FJFDYoOj0dzpqPJeaAcWErtXvM
-+SUWgeExX6GjfhaknBZqlxi9dnKlC54dNuYvoS++cJEPqOba+MSSQGwlfnuzCdyy
-F62ARPBopY+Udf90WuioAnwMCeKpSwughQtiue+hMZL77/ZRBIls6Kl0obsXs7X9
-SQ98POyDGCBDTtWTurQ0sR8WNh8M5mQ5Fkzc4P4dyKliPUDqysU0ArSuiYgzNdws
-E3PYJ/HQcu51OyLemGhmW/HGY0dVHLqlCFF1pkgl
------END CERTIFICATE-----
-
-# Issuer: CN=GTS Root R2 O=Google Trust Services LLC
-# Subject: CN=GTS Root R2 O=Google Trust Services LLC
-# Label: "GTS Root R2"
-# Serial: 146587176055767053814479386953112547951
-# MD5 Fingerprint: 44:ed:9a:0e:a4:09:3b:00:f2:ae:4c:a3:c6:61:b0:8b
-# SHA1 Fingerprint: d2:73:96:2a:2a:5e:39:9f:73:3f:e1:c7:1e:64:3f:03:38:34:fc:4d
-# SHA256 Fingerprint: c4:5d:7b:b0:8e:6d:67:e6:2e:42:35:11:0b:56:4e:5f:78:fd:92:ef:05:8c:84:0a:ea:4e:64:55:d7:58:5c:60
------BEGIN CERTIFICATE-----
-MIIFWjCCA0KgAwIBAgIQbkepxlqz5yDFMJo/aFLybzANBgkqhkiG9w0BAQwFADBH
-MQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExM
-QzEUMBIGA1UEAxMLR1RTIFJvb3QgUjIwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIy
-MDAwMDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNl
-cnZpY2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjIwggIiMA0GCSqGSIb3DQEB
-AQUAA4ICDwAwggIKAoICAQDO3v2m++zsFDQ8BwZabFn3GTXd98GdVarTzTukk3Lv
-CvptnfbwhYBboUhSnznFt+4orO/LdmgUud+tAWyZH8QiHZ/+cnfgLFuv5AS/T3Kg
-GjSY6Dlo7JUle3ah5mm5hRm9iYz+re026nO8/4Piy33B0s5Ks40FnotJk9/BW9Bu
-XvAuMC6C/Pq8tBcKSOWIm8Wba96wyrQD8Nr0kLhlZPdcTK3ofmZemde4wj7I0BOd
-re7kRXuJVfeKH2JShBKzwkCX44ofR5GmdFrS+LFjKBC4swm4VndAoiaYecb+3yXu
-PuWgf9RhD1FLPD+M2uFwdNjCaKH5wQzpoeJ/u1U8dgbuak7MkogwTZq9TwtImoS1
-mKPV+3PBV2HdKFZ1E66HjucMUQkQdYhMvI35ezzUIkgfKtzra7tEscszcTJGr61K
-8YzodDqs5xoic4DSMPclQsciOzsSrZYuxsN2B6ogtzVJV+mSSeh2FnIxZyuWfoqj
-x5RWIr9qS34BIbIjMt/kmkRtWVtd9QCgHJvGeJeNkP+byKq0rxFROV7Z+2et1VsR
-nTKaG73VululycslaVNVJ1zgyjbLiGH7HrfQy+4W+9OmTN6SpdTi3/UGVN4unUu0
-kzCqgc7dGtxRcw1PcOnlthYhGXmy5okLdWTK1au8CcEYof/UVKGFPP0UJAOyh9Ok
-twIDAQABo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNV
-HQ4EFgQUu//KjiOfT5nK2+JopqUVJxce2Q4wDQYJKoZIhvcNAQEMBQADggIBALZp
-8KZ3/p7uC4Gt4cCpx/k1HUCCq+YEtN/L9x0Pg/B+E02NjO7jMyLDOfxA325BS0JT
-vhaI8dI4XsRomRyYUpOM52jtG2pzegVATX9lO9ZY8c6DR2Dj/5epnGB3GFW1fgiT
-z9D2PGcDFWEJ+YF59exTpJ/JjwGLc8R3dtyDovUMSRqodt6Sm2T4syzFJ9MHwAiA
-pJiS4wGWAqoC7o87xdFtCjMwc3i5T1QWvwsHoaRc5svJXISPD+AVdyx+Jn7axEvb
-pxZ3B7DNdehyQtaVhJ2Gg/LkkM0JR9SLA3DaWsYDQvTtN6LwG1BUSw7YhN4ZKJmB
-R64JGz9I0cNv4rBgF/XuIwKl2gBbbZCr7qLpGzvpx0QnRY5rn/WkhLx3+WuXrD5R
-RaIRpsyF7gpo8j5QOHokYh4XIDdtak23CZvJ/KRY9bb7nE4Yu5UC56GtmwfuNmsk
-0jmGwZODUNKBRqhfYlcsu2xkiAhu7xNUX90txGdj08+JN7+dIPT7eoOboB6BAFDC
-5AwiWVIQ7UNWhwD4FFKnHYuTjKJNRn8nxnGbJN7k2oaLDX5rIMHAnuFl2GqjpuiF
-izoHCBy69Y9Vmhh1fuXsgWbRIXOhNUQLgD1bnF5vKheW0YMjiGZt5obicDIvUiLn
-yOd/xCxgXS/Dr55FBcOEArf9LAhST4Ldo/DUhgkC
------END CERTIFICATE-----
-
-# Issuer: CN=GTS Root R3 O=Google Trust Services LLC
-# Subject: CN=GTS Root R3 O=Google Trust Services LLC
-# Label: "GTS Root R3"
-# Serial: 146587176140553309517047991083707763997
-# MD5 Fingerprint: 1a:79:5b:6b:04:52:9c:5d:c7:74:33:1b:25:9a:f9:25
-# SHA1 Fingerprint: 30:d4:24:6f:07:ff:db:91:89:8a:0b:e9:49:66:11:eb:8c:5e:46:e5
-# SHA256 Fingerprint: 15:d5:b8:77:46:19:ea:7d:54:ce:1c:a6:d0:b0:c4:03:e0:37:a9:17:f1:31:e8:a0:4e:1e:6b:7a:71:ba:bc:e5
------BEGIN CERTIFICATE-----
-MIICDDCCAZGgAwIBAgIQbkepx2ypcyRAiQ8DVd2NHTAKBggqhkjOPQQDAzBHMQsw
-CQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEU
-MBIGA1UEAxMLR1RTIFJvb3QgUjMwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAw
-MDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZp
-Y2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjMwdjAQBgcqhkjOPQIBBgUrgQQA
-IgNiAAQfTzOHMymKoYTey8chWEGJ6ladK0uFxh1MJ7x/JlFyb+Kf1qPKzEUURout
-736GjOyxfi//qXGdGIRFBEFVbivqJn+7kAHjSxm65FSWRQmx1WyRRK2EE46ajA2A
-DDL24CejQjBAMA4GA1UdDwEB/wQEAwIBBjAPBgNVHRMBAf8EBTADAQH/MB0GA1Ud
-DgQWBBTB8Sa6oC2uhYHP0/EqEr24Cmf9vDAKBggqhkjOPQQDAwNpADBmAjEAgFuk
-fCPAlaUs3L6JbyO5o91lAFJekazInXJ0glMLfalAvWhgxeG4VDvBNhcl2MG9AjEA
-njWSdIUlUfUk7GRSJFClH9voy8l27OyCbvWFGFPouOOaKaqW04MjyaR7YbPMAuhd
------END CERTIFICATE-----
-
-# Issuer: CN=GTS Root R4 O=Google Trust Services LLC
-# Subject: CN=GTS Root R4 O=Google Trust Services LLC
-# Label: "GTS Root R4"
-# Serial: 146587176229350439916519468929765261721
-# MD5 Fingerprint: 5d:b6:6a:c4:60:17:24:6a:1a:99:a8:4b:ee:5e:b4:26
-# SHA1 Fingerprint: 2a:1d:60:27:d9:4a:b1:0a:1c:4d:91:5c:cd:33:a0:cb:3e:2d:54:cb
-# SHA256 Fingerprint: 71:cc:a5:39:1f:9e:79:4b:04:80:25:30:b3:63:e1:21:da:8a:30:43:bb:26:66:2f:ea:4d:ca:7f:c9:51:a4:bd
------BEGIN CERTIFICATE-----
-MIICCjCCAZGgAwIBAgIQbkepyIuUtui7OyrYorLBmTAKBggqhkjOPQQDAzBHMQsw
-CQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEU
-MBIGA1UEAxMLR1RTIFJvb3QgUjQwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAw
-MDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZp
-Y2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjQwdjAQBgcqhkjOPQIBBgUrgQQA
-IgNiAATzdHOnaItgrkO4NcWBMHtLSZ37wWHO5t5GvWvVYRg1rkDdc/eJkTBa6zzu
-hXyiQHY7qca4R9gq55KRanPpsXI5nymfopjTX15YhmUPoYRlBtHci8nHc8iMai/l
-xKvRHYqjQjBAMA4GA1UdDwEB/wQEAwIBBjAPBgNVHRMBAf8EBTADAQH/MB0GA1Ud
-DgQWBBSATNbrdP9JNqPV2Py1PsVq8JQdjDAKBggqhkjOPQQDAwNnADBkAjBqUFJ0
-CMRw3J5QdCHojXohw0+WbhXRIjVhLfoIN+4Zba3bssx9BzT1YBkstTTZbyACMANx
-sbqjYAuG7ZoIapVon+Kz4ZNkfF6Tpt95LY2F45TPI11xzPKwTdb+mciUqXWi4w==
------END CERTIFICATE-----
-
 # Issuer: CN=UCA Global G2 Root O=UniTrust
 # Subject: CN=UCA Global G2 Root O=UniTrust
 # Label: "UCA Global G2 Root"
 # Serial: 124779693093741543919145257850076631279
 # MD5 Fingerprint: 80:fe:f0:c4:4a:f0:5c:62:32:9f:1c:ba:78:a9:50:f8
 # SHA1 Fingerprint: 28:f9:78:16:19:7a:ff:18:25:18:aa:44:fe:c1:a0:ce:5c:b6:4c:8a
 # SHA256 Fingerprint: 9b:ea:11:c9:76:fe:01:47:64:c1:be:56:a6:f9:14:b5:a5:60:31:7a:bd:99:88:39:33:82:e5:16:1a:a0:49:3c
@@ -4251,7 +3769,759 @@
 5ePBAFmo+eggvIksDkc0C+pXwlM2/KfUrzHN/gLldfq5Jwn58/U7yn2fqSLLiMmq
 0Uc9NneoWWRrJ8/vJ8HjJLWG965+Mk2weWjROeiQWMODvA8s1pfrzgzhIMfatz7D
 P78v3DSk+yshzWePS/Tj6tQ/50+6uaWTRRxmHyH6ZF5v4HaUMst19W7l9o/HuKTM
 qJZ9ZPskWkoDbGs4xugDQ5r3V7mzKWmTOPQD8rv7gmsHINFSH5pkAnuYZttcTVoP
 0ISVoDwUQwbKytu4QTbaakRnh6+v40URFWkIsr4WOZckbxJF0WddCajJFdr60qZf
 E2Efv4WstK2tBZQIgx51F9NxO5NQI1mg7TyRVJ12AMXDuDjb
 -----END CERTIFICATE-----
+
+# Issuer: CN=TunTrust Root CA O=Agence Nationale de Certification Electronique
+# Subject: CN=TunTrust Root CA O=Agence Nationale de Certification Electronique
+# Label: "TunTrust Root CA"
+# Serial: 108534058042236574382096126452369648152337120275
+# MD5 Fingerprint: 85:13:b9:90:5b:36:5c:b6:5e:b8:5a:f8:e0:31:57:b4
+# SHA1 Fingerprint: cf:e9:70:84:0f:e0:73:0f:9d:f6:0c:7f:2c:4b:ee:20:46:34:9c:bb
+# SHA256 Fingerprint: 2e:44:10:2a:b5:8c:b8:54:19:45:1c:8e:19:d9:ac:f3:66:2c:af:bc:61:4b:6a:53:96:0a:30:f7:d0:e2:eb:41
+-----BEGIN CERTIFICATE-----
+MIIFszCCA5ugAwIBAgIUEwLV4kBMkkaGFmddtLu7sms+/BMwDQYJKoZIhvcNAQEL
+BQAwYTELMAkGA1UEBhMCVE4xNzA1BgNVBAoMLkFnZW5jZSBOYXRpb25hbGUgZGUg
+Q2VydGlmaWNhdGlvbiBFbGVjdHJvbmlxdWUxGTAXBgNVBAMMEFR1blRydXN0IFJv
+b3QgQ0EwHhcNMTkwNDI2MDg1NzU2WhcNNDQwNDI2MDg1NzU2WjBhMQswCQYDVQQG
+EwJUTjE3MDUGA1UECgwuQWdlbmNlIE5hdGlvbmFsZSBkZSBDZXJ0aWZpY2F0aW9u
+IEVsZWN0cm9uaXF1ZTEZMBcGA1UEAwwQVHVuVHJ1c3QgUm9vdCBDQTCCAiIwDQYJ
+KoZIhvcNAQEBBQADggIPADCCAgoCggIBAMPN0/y9BFPdDCA61YguBUtB9YOCfvdZ
+n56eY+hz2vYGqU8ftPkLHzmMmiDQfgbU7DTZhrx1W4eI8NLZ1KMKsmwb60ksPqxd
+2JQDoOw05TDENX37Jk0bbjBU2PWARZw5rZzJJQRNmpA+TkBuimvNKWfGzC3gdOgF
+VwpIUPp6Q9p+7FuaDmJ2/uqdHYVy7BG7NegfJ7/Boce7SBbdVtfMTqDhuazb1YMZ
+GoXRlJfXyqNlC/M4+QKu3fZnz8k/9YosRxqZbwUN/dAdgjH8KcwAWJeRTIAAHDOF
+li/LQcKLEITDCSSJH7UP2dl3RxiSlGBcx5kDPP73lad9UKGAwqmDrViWVSHbhlnU
+r8a83YFuB9tgYv7sEG7aaAH0gxupPqJbI9dkxt/con3YS7qC0lH4Zr8GRuR5KiY2
+eY8fTpkdso8MDhz/yV3A/ZAQprE38806JG60hZC/gLkMjNWb1sjxVj8agIl6qeIb
+MlEsPvLfe/ZdeikZjuXIvTZxi11Mwh0/rViizz1wTaZQmCXcI/m4WEEIcb9PuISg
+jwBUFfyRbVinljvrS5YnzWuioYasDXxU5mZMZl+QviGaAkYt5IPCgLnPSz7ofzwB
+7I9ezX/SKEIBlYrilz0QIX32nRzFNKHsLA4KUiwSVXAkPcvCFDVDXSdOvsC9qnyW
+5/yeYa1E0wCXAgMBAAGjYzBhMB0GA1UdDgQWBBQGmpsfU33x9aTI04Y+oXNZtPdE
+ITAPBgNVHRMBAf8EBTADAQH/MB8GA1UdIwQYMBaAFAaamx9TffH1pMjThj6hc1m0
+90QhMA4GA1UdDwEB/wQEAwIBBjANBgkqhkiG9w0BAQsFAAOCAgEAqgVutt0Vyb+z
+xiD2BkewhpMl0425yAA/l/VSJ4hxyXT968pk21vvHl26v9Hr7lxpuhbI87mP0zYu
+QEkHDVneixCwSQXi/5E/S7fdAo74gShczNxtr18UnH1YeA32gAm56Q6XKRm4t+v4
+FstVEuTGfbvE7Pi1HE4+Z7/FXxttbUcoqgRYYdZ2vyJ/0Adqp2RT8JeNnYA/u8EH
+22Wv5psymsNUk8QcCMNE+3tjEUPRahphanltkE8pjkcFwRJpadbGNjHh/PqAulxP
+xOu3Mqz4dWEX1xAZufHSCe96Qp1bWgvUxpVOKs7/B9dPfhgGiPEZtdmYu65xxBzn
+dFlY7wyJz4sfdZMaBBSSSFCp61cpABbjNhzI+L/wM9VBD8TMPN3pM0MBkRArHtG5
+Xc0yGYuPjCB31yLEQtyEFpslbei0VXF/sHyz03FJuc9SpAQ/3D2gu68zngowYI7b
+nV2UqL1g52KAdoGDDIzMMEZJ4gzSqK/rYXHv5yJiqfdcZGyfFoxnNidF9Ql7v/YQ
+CvGwjVRDjAS6oz/v4jXH+XTgbzRB0L9zZVcg+ZtnemZoJE6AZb0QmQZZ8mWvuMZH
+u/2QeItBcy6vVR/cO5JyboTT0GFMDcx2V+IthSIVNg3rAZ3r2OvEhJn7wAzMMujj
+d9qDRIueVSjAi1jTkD5OGwDxFa2DK5o=
+-----END CERTIFICATE-----
+
+# Issuer: CN=HARICA TLS RSA Root CA 2021 O=Hellenic Academic and Research Institutions CA
+# Subject: CN=HARICA TLS RSA Root CA 2021 O=Hellenic Academic and Research Institutions CA
+# Label: "HARICA TLS RSA Root CA 2021"
+# Serial: 76817823531813593706434026085292783742
+# MD5 Fingerprint: 65:47:9b:58:86:dd:2c:f0:fc:a2:84:1f:1e:96:c4:91
+# SHA1 Fingerprint: 02:2d:05:82:fa:88:ce:14:0c:06:79:de:7f:14:10:e9:45:d7:a5:6d
+# SHA256 Fingerprint: d9:5d:0e:8e:da:79:52:5b:f9:be:b1:1b:14:d2:10:0d:32:94:98:5f:0c:62:d9:fa:bd:9c:d9:99:ec:cb:7b:1d
+-----BEGIN CERTIFICATE-----
+MIIFpDCCA4ygAwIBAgIQOcqTHO9D88aOk8f0ZIk4fjANBgkqhkiG9w0BAQsFADBs
+MQswCQYDVQQGEwJHUjE3MDUGA1UECgwuSGVsbGVuaWMgQWNhZGVtaWMgYW5kIFJl
+c2VhcmNoIEluc3RpdHV0aW9ucyBDQTEkMCIGA1UEAwwbSEFSSUNBIFRMUyBSU0Eg
+Um9vdCBDQSAyMDIxMB4XDTIxMDIxOTEwNTUzOFoXDTQ1MDIxMzEwNTUzN1owbDEL
+MAkGA1UEBhMCR1IxNzA1BgNVBAoMLkhlbGxlbmljIEFjYWRlbWljIGFuZCBSZXNl
+YXJjaCBJbnN0aXR1dGlvbnMgQ0ExJDAiBgNVBAMMG0hBUklDQSBUTFMgUlNBIFJv
+b3QgQ0EgMjAyMTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBAIvC569l
+mwVnlskNJLnQDmT8zuIkGCyEf3dRywQRNrhe7Wlxp57kJQmXZ8FHws+RFjZiPTgE
+4VGC/6zStGndLuwRo0Xua2s7TL+MjaQenRG56Tj5eg4MmOIjHdFOY9TnuEFE+2uv
+a9of08WRiFukiZLRgeaMOVig1mlDqa2YUlhu2wr7a89o+uOkXjpFc5gH6l8Cct4M
+pbOfrqkdtx2z/IpZ525yZa31MJQjB/OCFks1mJxTuy/K5FrZx40d/JiZ+yykgmvw
+Kh+OC19xXFyuQnspiYHLA6OZyoieC0AJQTPb5lh6/a6ZcMBaD9YThnEvdmn8kN3b
+LW7R8pv1GmuebxWMevBLKKAiOIAkbDakO/IwkfN4E8/BPzWr8R0RI7VDIp4BkrcY
+AuUR0YLbFQDMYTfBKnya4dC6s1BG7oKsnTH4+yPiAwBIcKMJJnkVU2DzOFytOOqB
+AGMUuTNe3QvboEUHGjMJ+E20pwKmafTCWQWIZYVWrkvL4N48fS0ayOn7H6NhStYq
+E613TBoYm5EPWNgGVMWX+Ko/IIqmhaZ39qb8HOLubpQzKoNQhArlT4b4UEV4AIHr
+W2jjJo3Me1xR9BQsQL4aYB16cmEdH2MtiKrOokWQCPxrvrNQKlr9qEgYRtaQQJKQ
+CoReaDH46+0N0x3GfZkYVVYnZS6NRcUk7M7jAgMBAAGjQjBAMA8GA1UdEwEB/wQF
+MAMBAf8wHQYDVR0OBBYEFApII6ZgpJIKM+qTW8VX6iVNvRLuMA4GA1UdDwEB/wQE
+AwIBhjANBgkqhkiG9w0BAQsFAAOCAgEAPpBIqm5iFSVmewzVjIuJndftTgfvnNAU
+X15QvWiWkKQUEapobQk1OUAJ2vQJLDSle1mESSmXdMgHHkdt8s4cUCbjnj1AUz/3
+f5Z2EMVGpdAgS1D0NTsY9FVqQRtHBmg8uwkIYtlfVUKqrFOFrJVWNlar5AWMxaja
+H6NpvVMPxP/cyuN+8kyIhkdGGvMA9YCRotxDQpSbIPDRzbLrLFPCU3hKTwSUQZqP
+JzLB5UkZv/HywouoCjkxKLR9YjYsTewfM7Z+d21+UPCfDtcRj88YxeMn/ibvBZ3P
+zzfF0HvaO7AWhAw6k9a+F9sPPg4ZeAnHqQJyIkv3N3a6dcSFA1pj1bF1BcK5vZSt
+jBWZp5N99sXzqnTPBIWUmAD04vnKJGW/4GKvyMX6ssmeVkjaef2WdhW+o45WxLM0
+/L5H9MG0qPzVMIho7suuyWPEdr6sOBjhXlzPrjoiUevRi7PzKzMHVIf6tLITe7pT
+BGIBnfHAT+7hOtSLIBD6Alfm78ELt5BGnBkpjNxvoEppaZS3JGWg/6w/zgH7IS79
+aPib8qXPMThcFarmlwDB31qlpzmq6YR/PFGoOtmUW4y/Twhx5duoXNTSpv4Ao8YW
+xw/ogM4cKGR0GQjTQuPOAF1/sdwTsOEFy9EgqoZ0njnnkf3/W9b3raYvAwtt41dU
+63ZTGI0RmLo=
+-----END CERTIFICATE-----
+
+# Issuer: CN=HARICA TLS ECC Root CA 2021 O=Hellenic Academic and Research Institutions CA
+# Subject: CN=HARICA TLS ECC Root CA 2021 O=Hellenic Academic and Research Institutions CA
+# Label: "HARICA TLS ECC Root CA 2021"
+# Serial: 137515985548005187474074462014555733966
+# MD5 Fingerprint: ae:f7:4c:e5:66:35:d1:b7:9b:8c:22:93:74:d3:4b:b0
+# SHA1 Fingerprint: bc:b0:c1:9d:e9:98:92:70:19:38:57:e9:8d:a7:b4:5d:6e:ee:01:48
+# SHA256 Fingerprint: 3f:99:cc:47:4a:cf:ce:4d:fe:d5:87:94:66:5e:47:8d:15:47:73:9f:2e:78:0f:1b:b4:ca:9b:13:30:97:d4:01
+-----BEGIN CERTIFICATE-----
+MIICVDCCAdugAwIBAgIQZ3SdjXfYO2rbIvT/WeK/zjAKBggqhkjOPQQDAzBsMQsw
+CQYDVQQGEwJHUjE3MDUGA1UECgwuSGVsbGVuaWMgQWNhZGVtaWMgYW5kIFJlc2Vh
+cmNoIEluc3RpdHV0aW9ucyBDQTEkMCIGA1UEAwwbSEFSSUNBIFRMUyBFQ0MgUm9v
+dCBDQSAyMDIxMB4XDTIxMDIxOTExMDExMFoXDTQ1MDIxMzExMDEwOVowbDELMAkG
+A1UEBhMCR1IxNzA1BgNVBAoMLkhlbGxlbmljIEFjYWRlbWljIGFuZCBSZXNlYXJj
+aCBJbnN0aXR1dGlvbnMgQ0ExJDAiBgNVBAMMG0hBUklDQSBUTFMgRUNDIFJvb3Qg
+Q0EgMjAyMTB2MBAGByqGSM49AgEGBSuBBAAiA2IABDgI/rGgltJ6rK9JOtDA4MM7
+KKrxcm1lAEeIhPyaJmuqS7psBAqIXhfyVYf8MLA04jRYVxqEU+kw2anylnTDUR9Y
+STHMmE5gEYd103KUkE+bECUqqHgtvpBBWJAVcqeht6NCMEAwDwYDVR0TAQH/BAUw
+AwEB/zAdBgNVHQ4EFgQUyRtTgRL+BNUW0aq8mm+3oJUZbsowDgYDVR0PAQH/BAQD
+AgGGMAoGCCqGSM49BAMDA2cAMGQCMBHervjcToiwqfAircJRQO9gcS3ujwLEXQNw
+SaSS6sUUiHCm0w2wqsosQJz76YJumgIwK0eaB8bRwoF8yguWGEEbo/QwCZ61IygN
+nxS2PFOiTAZpffpskcYqSUXm7LcT4Tps
+-----END CERTIFICATE-----
+
+# Issuer: CN=Autoridad de Certificacion Firmaprofesional CIF A62634068
+# Subject: CN=Autoridad de Certificacion Firmaprofesional CIF A62634068
+# Label: "Autoridad de Certificacion Firmaprofesional CIF A62634068"
+# Serial: 1977337328857672817
+# MD5 Fingerprint: 4e:6e:9b:54:4c:ca:b7:fa:48:e4:90:b1:15:4b:1c:a3
+# SHA1 Fingerprint: 0b:be:c2:27:22:49:cb:39:aa:db:35:5c:53:e3:8c:ae:78:ff:b6:fe
+# SHA256 Fingerprint: 57:de:05:83:ef:d2:b2:6e:03:61:da:99:da:9d:f4:64:8d:ef:7e:e8:44:1c:3b:72:8a:fa:9b:cd:e0:f9:b2:6a
+-----BEGIN CERTIFICATE-----
+MIIGFDCCA/ygAwIBAgIIG3Dp0v+ubHEwDQYJKoZIhvcNAQELBQAwUTELMAkGA1UE
+BhMCRVMxQjBABgNVBAMMOUF1dG9yaWRhZCBkZSBDZXJ0aWZpY2FjaW9uIEZpcm1h
+cHJvZmVzaW9uYWwgQ0lGIEE2MjYzNDA2ODAeFw0xNDA5MjMxNTIyMDdaFw0zNjA1
+MDUxNTIyMDdaMFExCzAJBgNVBAYTAkVTMUIwQAYDVQQDDDlBdXRvcmlkYWQgZGUg
+Q2VydGlmaWNhY2lvbiBGaXJtYXByb2Zlc2lvbmFsIENJRiBBNjI2MzQwNjgwggIi
+MA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQDKlmuO6vj78aI14H9M2uDDUtd9
+thDIAl6zQyrET2qyyhxdKJp4ERppWVevtSBC5IsP5t9bpgOSL/UR5GLXMnE42QQM
+cas9UX4PB99jBVzpv5RvwSmCwLTaUbDBPLutN0pcyvFLNg4kq7/DhHf9qFD0sefG
+L9ItWY16Ck6WaVICqjaY7Pz6FIMMNx/Jkjd/14Et5cS54D40/mf0PmbR0/RAz15i
+NA9wBj4gGFrO93IbJWyTdBSTo3OxDqqHECNZXyAFGUftaI6SEspd/NYrspI8IM/h
+X68gvqB2f3bl7BqGYTM+53u0P6APjqK5am+5hyZvQWyIplD9amML9ZMWGxmPsu2b
+m8mQ9QEM3xk9Dz44I8kvjwzRAv4bVdZO0I08r0+k8/6vKtMFnXkIoctXMbScyJCy
+Z/QYFpM6/EfY0XiWMR+6KwxfXZmtY4laJCB22N/9q06mIqqdXuYnin1oKaPnirja
+EbsXLZmdEyRG98Xi2J+Of8ePdG1asuhy9azuJBCtLxTa/y2aRnFHvkLfuwHb9H/T
+KI8xWVvTyQKmtFLKbpf7Q8UIJm+K9Lv9nyiqDdVF8xM6HdjAeI9BZzwelGSuewvF
+6NkBiDkal4ZkQdU7hwxu+g/GvUgUvzlN1J5Bto+WHWOWk9mVBngxaJ43BjuAiUVh
+OSPHG0SjFeUc+JIwuwIDAQABo4HvMIHsMB0GA1UdDgQWBBRlzeurNR4APn7VdMAc
+tHNHDhpkLzASBgNVHRMBAf8ECDAGAQH/AgEBMIGmBgNVHSAEgZ4wgZswgZgGBFUd
+IAAwgY8wLwYIKwYBBQUHAgEWI2h0dHA6Ly93d3cuZmlybWFwcm9mZXNpb25hbC5j
+b20vY3BzMFwGCCsGAQUFBwICMFAeTgBQAGEAcwBlAG8AIABkAGUAIABsAGEAIABC
+AG8AbgBhAG4AbwB2AGEAIAA0ADcAIABCAGEAcgBjAGUAbABvAG4AYQAgADAAOAAw
+ADEANzAOBgNVHQ8BAf8EBAMCAQYwDQYJKoZIhvcNAQELBQADggIBAHSHKAIrdx9m
+iWTtj3QuRhy7qPj4Cx2Dtjqn6EWKB7fgPiDL4QjbEwj4KKE1soCzC1HA01aajTNF
+Sa9J8OA9B3pFE1r/yJfY0xgsfZb43aJlQ3CTkBW6kN/oGbDbLIpgD7dvlAceHabJ
+hfa9NPhAeGIQcDq+fUs5gakQ1JZBu/hfHAsdCPKxsIl68veg4MSPi3i1O1ilI45P
+Vf42O+AMt8oqMEEgtIDNrvx2ZnOorm7hfNoD6JQg5iKj0B+QXSBTFCZX2lSX3xZE
+EAEeiGaPcjiT3SC3NL7X8e5jjkd5KAb881lFJWAiMxujX6i6KtoaPc1A6ozuBRWV
+1aUsIC+nmCjuRfzxuIgALI9C2lHVnOUTaHFFQ4ueCyE8S1wF3BqfmI7avSKecs2t
+CsvMo2ebKHTEm9caPARYpoKdrcd7b/+Alun4jWq9GJAd/0kakFI3ky88Al2CdgtR
+5xbHV/g4+afNmyJU72OwFW1TZQNKXkqgsqeOSQBZONXH9IBk9W6VULgRfhVwOEqw
+f9DEMnDAGf/JOC0ULGb0QkTmVXYbgBVX/8Cnp6o5qtjTcNAuuuuUavpfNIbnYrX9
+ivAwhZTJryQCL2/W3Wf+47BVTwSYT6RBVuKT0Gro1vP7ZeDOdcQxWQzugsgMYDNK
+GbqEZycPvEJdvSRUDewdcAZfpLz6IHxV
+-----END CERTIFICATE-----
+
+# Issuer: CN=vTrus ECC Root CA O=iTrusChina Co.,Ltd.
+# Subject: CN=vTrus ECC Root CA O=iTrusChina Co.,Ltd.
+# Label: "vTrus ECC Root CA"
+# Serial: 630369271402956006249506845124680065938238527194
+# MD5 Fingerprint: de:4b:c1:f5:52:8c:9b:43:e1:3e:8f:55:54:17:8d:85
+# SHA1 Fingerprint: f6:9c:db:b0:fc:f6:02:13:b6:52:32:a6:a3:91:3f:16:70:da:c3:e1
+# SHA256 Fingerprint: 30:fb:ba:2c:32:23:8e:2a:98:54:7a:f9:79:31:e5:50:42:8b:9b:3f:1c:8e:eb:66:33:dc:fa:86:c5:b2:7d:d3
+-----BEGIN CERTIFICATE-----
+MIICDzCCAZWgAwIBAgIUbmq8WapTvpg5Z6LSa6Q75m0c1towCgYIKoZIzj0EAwMw
+RzELMAkGA1UEBhMCQ04xHDAaBgNVBAoTE2lUcnVzQ2hpbmEgQ28uLEx0ZC4xGjAY
+BgNVBAMTEXZUcnVzIEVDQyBSb290IENBMB4XDTE4MDczMTA3MjY0NFoXDTQzMDcz
+MTA3MjY0NFowRzELMAkGA1UEBhMCQ04xHDAaBgNVBAoTE2lUcnVzQ2hpbmEgQ28u
+LEx0ZC4xGjAYBgNVBAMTEXZUcnVzIEVDQyBSb290IENBMHYwEAYHKoZIzj0CAQYF
+K4EEACIDYgAEZVBKrox5lkqqHAjDo6LN/llWQXf9JpRCux3NCNtzslt188+cToL0
+v/hhJoVs1oVbcnDS/dtitN9Ti72xRFhiQgnH+n9bEOf+QP3A2MMrMudwpremIFUd
+e4BdS49nTPEQo0IwQDAdBgNVHQ4EFgQUmDnNvtiyjPeyq+GtJK97fKHbH88wDwYD
+VR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAQYwCgYIKoZIzj0EAwMDaAAwZQIw
+V53dVvHH4+m4SVBrm2nDb+zDfSXkV5UTQJtS0zvzQBm8JsctBp61ezaf9SXUY2sA
+AjEA6dPGnlaaKsyh2j/IZivTWJwghfqrkYpwcBE4YGQLYgmRWAD5Tfs0aNoJrSEG
+GJTO
+-----END CERTIFICATE-----
+
+# Issuer: CN=vTrus Root CA O=iTrusChina Co.,Ltd.
+# Subject: CN=vTrus Root CA O=iTrusChina Co.,Ltd.
+# Label: "vTrus Root CA"
+# Serial: 387574501246983434957692974888460947164905180485
+# MD5 Fingerprint: b8:c9:37:df:fa:6b:31:84:64:c5:ea:11:6a:1b:75:fc
+# SHA1 Fingerprint: 84:1a:69:fb:f5:cd:1a:25:34:13:3d:e3:f8:fc:b8:99:d0:c9:14:b7
+# SHA256 Fingerprint: 8a:71:de:65:59:33:6f:42:6c:26:e5:38:80:d0:0d:88:a1:8d:a4:c6:a9:1f:0d:cb:61:94:e2:06:c5:c9:63:87
+-----BEGIN CERTIFICATE-----
+MIIFVjCCAz6gAwIBAgIUQ+NxE9izWRRdt86M/TX9b7wFjUUwDQYJKoZIhvcNAQEL
+BQAwQzELMAkGA1UEBhMCQ04xHDAaBgNVBAoTE2lUcnVzQ2hpbmEgQ28uLEx0ZC4x
+FjAUBgNVBAMTDXZUcnVzIFJvb3QgQ0EwHhcNMTgwNzMxMDcyNDA1WhcNNDMwNzMx
+MDcyNDA1WjBDMQswCQYDVQQGEwJDTjEcMBoGA1UEChMTaVRydXNDaGluYSBDby4s
+THRkLjEWMBQGA1UEAxMNdlRydXMgUm9vdCBDQTCCAiIwDQYJKoZIhvcNAQEBBQAD
+ggIPADCCAgoCggIBAL1VfGHTuB0EYgWgrmy3cLRB6ksDXhA/kFocizuwZotsSKYc
+IrrVQJLuM7IjWcmOvFjai57QGfIvWcaMY1q6n6MLsLOaXLoRuBLpDLvPbmyAhykU
+AyyNJJrIZIO1aqwTLDPxn9wsYTwaP3BVm60AUn/PBLn+NvqcwBauYv6WTEN+VRS+
+GrPSbcKvdmaVayqwlHeFXgQPYh1jdfdr58tbmnDsPmcF8P4HCIDPKNsFxhQnL4Z9
+8Cfe/+Z+M0jnCx5Y0ScrUw5XSmXX+6KAYPxMvDVTAWqXcoKv8R1w6Jz1717CbMdH
+flqUhSZNO7rrTOiwCcJlwp2dCZtOtZcFrPUGoPc2BX70kLJrxLT5ZOrpGgrIDajt
+J8nU57O5q4IikCc9Kuh8kO+8T/3iCiSn3mUkpF3qwHYw03dQ+A0Em5Q2AXPKBlim
+0zvc+gRGE1WKyURHuFE5Gi7oNOJ5y1lKCn+8pu8fA2dqWSslYpPZUxlmPCdiKYZN
+pGvu/9ROutW04o5IWgAZCfEF2c6Rsffr6TlP9m8EQ5pV9T4FFL2/s1m02I4zhKOQ
+UqqzApVg+QxMaPnu1RcN+HFXtSXkKe5lXa/R7jwXC1pDxaWG6iSe4gUH3DRCEpHW
+OXSuTEGC2/KmSNGzm/MzqvOmwMVO9fSddmPmAsYiS8GVP1BkLFTltvA8Kc9XAgMB
+AAGjQjBAMB0GA1UdDgQWBBRUYnBj8XWEQ1iO0RYgscasGrz2iTAPBgNVHRMBAf8E
+BTADAQH/MA4GA1UdDwEB/wQEAwIBBjANBgkqhkiG9w0BAQsFAAOCAgEAKbqSSaet
+8PFww+SX8J+pJdVrnjT+5hpk9jprUrIQeBqfTNqK2uwcN1LgQkv7bHbKJAs5EhWd
+nxEt/Hlk3ODg9d3gV8mlsnZwUKT+twpw1aA08XXXTUm6EdGz2OyC/+sOxL9kLX1j
+bhd47F18iMjrjld22VkE+rxSH0Ws8HqA7Oxvdq6R2xCOBNyS36D25q5J08FsEhvM
+Kar5CKXiNxTKsbhm7xqC5PD48acWabfbqWE8n/Uxy+QARsIvdLGx14HuqCaVvIiv
+TDUHKgLKeBRtRytAVunLKmChZwOgzoy8sHJnxDHO2zTlJQNgJXtxmOTAGytfdELS
+S8VZCAeHvsXDf+eW2eHcKJfWjwXj9ZtOyh1QRwVTsMo554WgicEFOwE30z9J4nfr
+I8iIZjs9OXYhRvHsXyO466JmdXTBQPfYaJqT4i2pLr0cox7IdMakLXogqzu4sEb9
+b91fUlV1YvCXoHzXOP0l382gmxDPi7g4Xl7FtKYCNqEeXxzP4padKar9mK5S4fNB
+UvupLnKWnyfjqnN9+BojZns7q2WwMgFLFT49ok8MKzWixtlnEjUwzXYuFrOZnk1P
+Ti07NEPhmg4NpGaXutIcSkwsKouLgU9xGqndXHt7CMUADTdA43x7VF8vhV929ven
+sBxXVsFy6K2ir40zSbofitzmdHxghm+Hl3s=
+-----END CERTIFICATE-----
+
+# Issuer: CN=ISRG Root X2 O=Internet Security Research Group
+# Subject: CN=ISRG Root X2 O=Internet Security Research Group
+# Label: "ISRG Root X2"
+# Serial: 87493402998870891108772069816698636114
+# MD5 Fingerprint: d3:9e:c4:1e:23:3c:a6:df:cf:a3:7e:6d:e0:14:e6:e5
+# SHA1 Fingerprint: bd:b1:b9:3c:d5:97:8d:45:c6:26:14:55:f8:db:95:c7:5a:d1:53:af
+# SHA256 Fingerprint: 69:72:9b:8e:15:a8:6e:fc:17:7a:57:af:b7:17:1d:fc:64:ad:d2:8c:2f:ca:8c:f1:50:7e:34:45:3c:cb:14:70
+-----BEGIN CERTIFICATE-----
+MIICGzCCAaGgAwIBAgIQQdKd0XLq7qeAwSxs6S+HUjAKBggqhkjOPQQDAzBPMQsw
+CQYDVQQGEwJVUzEpMCcGA1UEChMgSW50ZXJuZXQgU2VjdXJpdHkgUmVzZWFyY2gg
+R3JvdXAxFTATBgNVBAMTDElTUkcgUm9vdCBYMjAeFw0yMDA5MDQwMDAwMDBaFw00
+MDA5MTcxNjAwMDBaME8xCzAJBgNVBAYTAlVTMSkwJwYDVQQKEyBJbnRlcm5ldCBT
+ZWN1cml0eSBSZXNlYXJjaCBHcm91cDEVMBMGA1UEAxMMSVNSRyBSb290IFgyMHYw
+EAYHKoZIzj0CAQYFK4EEACIDYgAEzZvVn4CDCuwJSvMWSj5cz3es3mcFDR0HttwW
++1qLFNvicWDEukWVEYmO6gbf9yoWHKS5xcUy4APgHoIYOIvXRdgKam7mAHf7AlF9
+ItgKbppbd9/w+kHsOdx1ymgHDB/qo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0T
+AQH/BAUwAwEB/zAdBgNVHQ4EFgQUfEKWrt5LSDv6kviejM9ti6lyN5UwCgYIKoZI
+zj0EAwMDaAAwZQIwe3lORlCEwkSHRhtFcP9Ymd70/aTSVaYgLXTWNLxBo1BfASdW
+tL4ndQavEi51mI38AjEAi/V3bNTIZargCyzuFJ0nN6T5U6VR5CmD1/iQMVtCnwr1
+/q4AaOeMSQ+2b1tbFfLn
+-----END CERTIFICATE-----
+
+# Issuer: CN=HiPKI Root CA - G1 O=Chunghwa Telecom Co., Ltd.
+# Subject: CN=HiPKI Root CA - G1 O=Chunghwa Telecom Co., Ltd.
+# Label: "HiPKI Root CA - G1"
+# Serial: 60966262342023497858655262305426234976
+# MD5 Fingerprint: 69:45:df:16:65:4b:e8:68:9a:8f:76:5f:ff:80:9e:d3
+# SHA1 Fingerprint: 6a:92:e4:a8:ee:1b:ec:96:45:37:e3:29:57:49:cd:96:e3:e5:d2:60
+# SHA256 Fingerprint: f0:15:ce:3c:c2:39:bf:ef:06:4b:e9:f1:d2:c4:17:e1:a0:26:4a:0a:94:be:1f:0c:8d:12:18:64:eb:69:49:cc
+-----BEGIN CERTIFICATE-----
+MIIFajCCA1KgAwIBAgIQLd2szmKXlKFD6LDNdmpeYDANBgkqhkiG9w0BAQsFADBP
+MQswCQYDVQQGEwJUVzEjMCEGA1UECgwaQ2h1bmdod2EgVGVsZWNvbSBDby4sIEx0
+ZC4xGzAZBgNVBAMMEkhpUEtJIFJvb3QgQ0EgLSBHMTAeFw0xOTAyMjIwOTQ2MDRa
+Fw0zNzEyMzExNTU5NTlaME8xCzAJBgNVBAYTAlRXMSMwIQYDVQQKDBpDaHVuZ2h3
+YSBUZWxlY29tIENvLiwgTHRkLjEbMBkGA1UEAwwSSGlQS0kgUm9vdCBDQSAtIEcx
+MIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEA9B5/UnMyDHPkvRN0o9Qw
+qNCuS9i233VHZvR85zkEHmpwINJaR3JnVfSl6J3VHiGh8Ge6zCFovkRTv4354twv
+Vcg3Px+kwJyz5HdcoEb+d/oaoDjq7Zpy3iu9lFc6uux55199QmQ5eiY29yTw1S+6
+lZgRZq2XNdZ1AYDgr/SEYYwNHl98h5ZeQa/rh+r4XfEuiAU+TCK72h8q3VJGZDnz
+Qs7ZngyzsHeXZJzA9KMuH5UHsBffMNsAGJZMoYFL3QRtU6M9/Aes1MU3guvklQgZ
+KILSQjqj2FPseYlgSGDIcpJQ3AOPgz+yQlda22rpEZfdhSi8MEyr48KxRURHH+CK
+FgeW0iEPU8DtqX7UTuybCeyvQqww1r/REEXgphaypcXTT3OUM3ECoWqj1jOXTyFj
+HluP2cFeRXF3D4FdXyGarYPM+l7WjSNfGz1BryB1ZlpK9p/7qxj3ccC2HTHsOyDr
+y+K49a6SsvfhhEvyovKTmiKe0xRvNlS9H15ZFblzqMF8b3ti6RZsR1pl8w4Rm0bZ
+/W3c1pzAtH2lsN0/Vm+h+fbkEkj9Bn8SV7apI09bA8PgcSojt/ewsTu8mL3WmKgM
+a/aOEmem8rJY5AIJEzypuxC00jBF8ez3ABHfZfjcK0NVvxaXxA/VLGGEqnKG/uY6
+fsI/fe78LxQ+5oXdUG+3Se0CAwEAAaNCMEAwDwYDVR0TAQH/BAUwAwEB/zAdBgNV
+HQ4EFgQU8ncX+l6o/vY9cdVouslGDDjYr7AwDgYDVR0PAQH/BAQDAgGGMA0GCSqG
+SIb3DQEBCwUAA4ICAQBQUfB13HAE4/+qddRxosuej6ip0691x1TPOhwEmSKsxBHi
+7zNKpiMdDg1H2DfHb680f0+BazVP6XKlMeJ45/dOlBhbQH3PayFUhuaVevvGyuqc
+SE5XCV0vrPSltJczWNWseanMX/mF+lLFjfiRFOs6DRfQUsJ748JzjkZ4Bjgs6Fza
+ZsT0pPBWGTMpWmWSBUdGSquEwx4noR8RkpkndZMPvDY7l1ePJlsMu5wP1G4wB9Tc
+XzZoZjmDlicmisjEOf6aIW/Vcobpf2Lll07QJNBAsNB1CI69aO4I1258EHBGG3zg
+iLKecoaZAeO/n0kZtCW+VmWuF2PlHt/o/0elv+EmBYTksMCv5wiZqAxeJoBF1Pho
+L5aPruJKHJwWDBNvOIf2u8g0X5IDUXlwpt/L9ZlNec1OvFefQ05rLisY+GpzjLrF
+Ne85akEez3GoorKGB1s6yeHvP2UEgEcyRHCVTjFnanRbEEV16rCf0OY1/k6fi8wr
+kkVbbiVghUbN0aqwdmaTd5a+g744tiROJgvM7XpWGuDpWsZkrUx6AEhEL7lAuxM+
+vhV4nYWBSipX3tUZQ9rbyltHhoMLP7YNdnhzeSJesYAfz77RP1YQmCuVh6EfnWQU
+YDksswBVLuT1sw5XxJFBAJw/6KXf6vb/yPCtbVKoF6ubYfwSUTXkJf2vqmqGOQ==
+-----END CERTIFICATE-----
+
+# Issuer: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R4
+# Subject: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R4
+# Label: "GlobalSign ECC Root CA - R4"
+# Serial: 159662223612894884239637590694
+# MD5 Fingerprint: 26:29:f8:6d:e1:88:bf:a2:65:7f:aa:c4:cd:0f:7f:fc
+# SHA1 Fingerprint: 6b:a0:b0:98:e1:71:ef:5a:ad:fe:48:15:80:77:10:f4:bd:6f:0b:28
+# SHA256 Fingerprint: b0:85:d7:0b:96:4f:19:1a:73:e4:af:0d:54:ae:7a:0e:07:aa:fd:af:9b:71:dd:08:62:13:8a:b7:32:5a:24:a2
+-----BEGIN CERTIFICATE-----
+MIIB3DCCAYOgAwIBAgINAgPlfvU/k/2lCSGypjAKBggqhkjOPQQDAjBQMSQwIgYD
+VQQLExtHbG9iYWxTaWduIEVDQyBSb290IENBIC0gUjQxEzARBgNVBAoTCkdsb2Jh
+bFNpZ24xEzARBgNVBAMTCkdsb2JhbFNpZ24wHhcNMTIxMTEzMDAwMDAwWhcNMzgw
+MTE5MDMxNDA3WjBQMSQwIgYDVQQLExtHbG9iYWxTaWduIEVDQyBSb290IENBIC0g
+UjQxEzARBgNVBAoTCkdsb2JhbFNpZ24xEzARBgNVBAMTCkdsb2JhbFNpZ24wWTAT
+BgcqhkjOPQIBBggqhkjOPQMBBwNCAAS4xnnTj2wlDp8uORkcA6SumuU5BwkWymOx
+uYb4ilfBV85C+nOh92VC/x7BALJucw7/xyHlGKSq2XE/qNS5zowdo0IwQDAOBgNV
+HQ8BAf8EBAMCAYYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUVLB7rUW44kB/
++wpu+74zyTyjhNUwCgYIKoZIzj0EAwIDRwAwRAIgIk90crlgr/HmnKAWBVBfw147
+bmF0774BxL4YSFlhgjICICadVGNA3jdgUM/I2O2dgq43mLyjj0xMqTQrbO/7lZsm
+-----END CERTIFICATE-----
+
+# Issuer: CN=GTS Root R1 O=Google Trust Services LLC
+# Subject: CN=GTS Root R1 O=Google Trust Services LLC
+# Label: "GTS Root R1"
+# Serial: 159662320309726417404178440727
+# MD5 Fingerprint: 05:fe:d0:bf:71:a8:a3:76:63:da:01:e0:d8:52:dc:40
+# SHA1 Fingerprint: e5:8c:1c:c4:91:3b:38:63:4b:e9:10:6e:e3:ad:8e:6b:9d:d9:81:4a
+# SHA256 Fingerprint: d9:47:43:2a:bd:e7:b7:fa:90:fc:2e:6b:59:10:1b:12:80:e0:e1:c7:e4:e4:0f:a3:c6:88:7f:ff:57:a7:f4:cf
+-----BEGIN CERTIFICATE-----
+MIIFVzCCAz+gAwIBAgINAgPlk28xsBNJiGuiFzANBgkqhkiG9w0BAQwFADBHMQsw
+CQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEU
+MBIGA1UEAxMLR1RTIFJvb3QgUjEwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAw
+MDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZp
+Y2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjEwggIiMA0GCSqGSIb3DQEBAQUA
+A4ICDwAwggIKAoICAQC2EQKLHuOhd5s73L+UPreVp0A8of2C+X0yBoJx9vaMf/vo
+27xqLpeXo4xL+Sv2sfnOhB2x+cWX3u+58qPpvBKJXqeqUqv4IyfLpLGcY9vXmX7w
+Cl7raKb0xlpHDU0QM+NOsROjyBhsS+z8CZDfnWQpJSMHobTSPS5g4M/SCYe7zUjw
+TcLCeoiKu7rPWRnWr4+wB7CeMfGCwcDfLqZtbBkOtdh+JhpFAz2weaSUKK0Pfybl
+qAj+lug8aJRT7oM6iCsVlgmy4HqMLnXWnOunVmSPlk9orj2XwoSPwLxAwAtcvfaH
+szVsrBhQf4TgTM2S0yDpM7xSma8ytSmzJSq0SPly4cpk9+aCEI3oncKKiPo4Zor8
+Y/kB+Xj9e1x3+naH+uzfsQ55lVe0vSbv1gHR6xYKu44LtcXFilWr06zqkUspzBmk
+MiVOKvFlRNACzqrOSbTqn3yDsEB750Orp2yjj32JgfpMpf/VjsPOS+C12LOORc92
+wO1AK/1TD7Cn1TsNsYqiA94xrcx36m97PtbfkSIS5r762DL8EGMUUXLeXdYWk70p
+aDPvOmbsB4om3xPXV2V4J95eSRQAogB/mqghtqmxlbCluQ0WEdrHbEg8QOB+DVrN
+VjzRlwW5y0vtOUucxD/SVRNuJLDWcfr0wbrM7Rv1/oFB2ACYPTrIrnqYNxgFlQID
+AQABo0IwQDAOBgNVHQ8BAf8EBAMCAYYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4E
+FgQU5K8rJnEaK0gnhS9SZizv8IkTcT4wDQYJKoZIhvcNAQEMBQADggIBAJ+qQibb
+C5u+/x6Wki4+omVKapi6Ist9wTrYggoGxval3sBOh2Z5ofmmWJyq+bXmYOfg6LEe
+QkEzCzc9zolwFcq1JKjPa7XSQCGYzyI0zzvFIoTgxQ6KfF2I5DUkzps+GlQebtuy
+h6f88/qBVRRiClmpIgUxPoLW7ttXNLwzldMXG+gnoot7TiYaelpkttGsN/H9oPM4
+7HLwEXWdyzRSjeZ2axfG34arJ45JK3VmgRAhpuo+9K4l/3wV3s6MJT/KYnAK9y8J
+ZgfIPxz88NtFMN9iiMG1D53Dn0reWVlHxYciNuaCp+0KueIHoI17eko8cdLiA6Ef
+MgfdG+RCzgwARWGAtQsgWSl4vflVy2PFPEz0tv/bal8xa5meLMFrUKTX5hgUvYU/
+Z6tGn6D/Qqc6f1zLXbBwHSs09dR2CQzreExZBfMzQsNhFRAbd03OIozUhfJFfbdT
+6u9AWpQKXCBfTkBdYiJ23//OYb2MI3jSNwLgjt7RETeJ9r/tSQdirpLsQBqvFAnZ
+0E6yove+7u7Y/9waLd64NnHi/Hm3lCXRSHNboTXns5lndcEZOitHTtNCjv0xyBZm
+2tIMPNuzjsmhDYAPexZ3FL//2wmUspO8IFgV6dtxQ/PeEMMA3KgqlbbC1j+Qa3bb
+bP6MvPJwNQzcmRk13NfIRmPVNnGuV/u3gm3c
+-----END CERTIFICATE-----
+
+# Issuer: CN=GTS Root R2 O=Google Trust Services LLC
+# Subject: CN=GTS Root R2 O=Google Trust Services LLC
+# Label: "GTS Root R2"
+# Serial: 159662449406622349769042896298
+# MD5 Fingerprint: 1e:39:c0:53:e6:1e:29:82:0b:ca:52:55:36:5d:57:dc
+# SHA1 Fingerprint: 9a:44:49:76:32:db:de:fa:d0:bc:fb:5a:7b:17:bd:9e:56:09:24:94
+# SHA256 Fingerprint: 8d:25:cd:97:22:9d:bf:70:35:6b:da:4e:b3:cc:73:40:31:e2:4c:f0:0f:af:cf:d3:2d:c7:6e:b5:84:1c:7e:a8
+-----BEGIN CERTIFICATE-----
+MIIFVzCCAz+gAwIBAgINAgPlrsWNBCUaqxElqjANBgkqhkiG9w0BAQwFADBHMQsw
+CQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEU
+MBIGA1UEAxMLR1RTIFJvb3QgUjIwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAw
+MDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZp
+Y2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjIwggIiMA0GCSqGSIb3DQEBAQUA
+A4ICDwAwggIKAoICAQDO3v2m++zsFDQ8BwZabFn3GTXd98GdVarTzTukk3LvCvpt
+nfbwhYBboUhSnznFt+4orO/LdmgUud+tAWyZH8QiHZ/+cnfgLFuv5AS/T3KgGjSY
+6Dlo7JUle3ah5mm5hRm9iYz+re026nO8/4Piy33B0s5Ks40FnotJk9/BW9BuXvAu
+MC6C/Pq8tBcKSOWIm8Wba96wyrQD8Nr0kLhlZPdcTK3ofmZemde4wj7I0BOdre7k
+RXuJVfeKH2JShBKzwkCX44ofR5GmdFrS+LFjKBC4swm4VndAoiaYecb+3yXuPuWg
+f9RhD1FLPD+M2uFwdNjCaKH5wQzpoeJ/u1U8dgbuak7MkogwTZq9TwtImoS1mKPV
++3PBV2HdKFZ1E66HjucMUQkQdYhMvI35ezzUIkgfKtzra7tEscszcTJGr61K8Yzo
+dDqs5xoic4DSMPclQsciOzsSrZYuxsN2B6ogtzVJV+mSSeh2FnIxZyuWfoqjx5RW
+Ir9qS34BIbIjMt/kmkRtWVtd9QCgHJvGeJeNkP+byKq0rxFROV7Z+2et1VsRnTKa
+G73VululycslaVNVJ1zgyjbLiGH7HrfQy+4W+9OmTN6SpdTi3/UGVN4unUu0kzCq
+gc7dGtxRcw1PcOnlthYhGXmy5okLdWTK1au8CcEYof/UVKGFPP0UJAOyh9OktwID
+AQABo0IwQDAOBgNVHQ8BAf8EBAMCAYYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4E
+FgQUu//KjiOfT5nK2+JopqUVJxce2Q4wDQYJKoZIhvcNAQEMBQADggIBAB/Kzt3H
+vqGf2SdMC9wXmBFqiN495nFWcrKeGk6c1SuYJF2ba3uwM4IJvd8lRuqYnrYb/oM8
+0mJhwQTtzuDFycgTE1XnqGOtjHsB/ncw4c5omwX4Eu55MaBBRTUoCnGkJE+M3DyC
+B19m3H0Q/gxhswWV7uGugQ+o+MePTagjAiZrHYNSVc61LwDKgEDg4XSsYPWHgJ2u
+NmSRXbBoGOqKYcl3qJfEycel/FVL8/B/uWU9J2jQzGv6U53hkRrJXRqWbTKH7QMg
+yALOWr7Z6v2yTcQvG99fevX4i8buMTolUVVnjWQye+mew4K6Ki3pHrTgSAai/Gev
+HyICc/sgCq+dVEuhzf9gR7A/Xe8bVr2XIZYtCtFenTgCR2y59PYjJbigapordwj6
+xLEokCZYCDzifqrXPW+6MYgKBesntaFJ7qBFVHvmJ2WZICGoo7z7GJa7Um8M7YNR
+TOlZ4iBgxcJlkoKM8xAfDoqXvneCbT+PHV28SSe9zE8P4c52hgQjxcCMElv924Sg
+JPFI/2R80L5cFtHvma3AH/vLrrw4IgYmZNralw4/KBVEqE8AyvCazM90arQ+POuV
+7LXTWtiBmelDGDfrs7vRWGJB82bSj6p4lVQgw1oudCvV0b4YacCs1aTPObpRhANl
+6WLAYv7YTVWW4tAR+kg0Eeye7QUd5MjWHYbL
+-----END CERTIFICATE-----
+
+# Issuer: CN=GTS Root R3 O=Google Trust Services LLC
+# Subject: CN=GTS Root R3 O=Google Trust Services LLC
+# Label: "GTS Root R3"
+# Serial: 159662495401136852707857743206
+# MD5 Fingerprint: 3e:e7:9d:58:02:94:46:51:94:e5:e0:22:4a:8b:e7:73
+# SHA1 Fingerprint: ed:e5:71:80:2b:c8:92:b9:5b:83:3c:d2:32:68:3f:09:cd:a0:1e:46
+# SHA256 Fingerprint: 34:d8:a7:3e:e2:08:d9:bc:db:0d:95:65:20:93:4b:4e:40:e6:94:82:59:6e:8b:6f:73:c8:42:6b:01:0a:6f:48
+-----BEGIN CERTIFICATE-----
+MIICCTCCAY6gAwIBAgINAgPluILrIPglJ209ZjAKBggqhkjOPQQDAzBHMQswCQYD
+VQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEUMBIG
+A1UEAxMLR1RTIFJvb3QgUjMwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAwMDAw
+WjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2Vz
+IExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjMwdjAQBgcqhkjOPQIBBgUrgQQAIgNi
+AAQfTzOHMymKoYTey8chWEGJ6ladK0uFxh1MJ7x/JlFyb+Kf1qPKzEUURout736G
+jOyxfi//qXGdGIRFBEFVbivqJn+7kAHjSxm65FSWRQmx1WyRRK2EE46ajA2ADDL2
+4CejQjBAMA4GA1UdDwEB/wQEAwIBhjAPBgNVHRMBAf8EBTADAQH/MB0GA1UdDgQW
+BBTB8Sa6oC2uhYHP0/EqEr24Cmf9vDAKBggqhkjOPQQDAwNpADBmAjEA9uEglRR7
+VKOQFhG/hMjqb2sXnh5GmCCbn9MN2azTL818+FsuVbu/3ZL3pAzcMeGiAjEA/Jdm
+ZuVDFhOD3cffL74UOO0BzrEXGhF16b0DjyZ+hOXJYKaV11RZt+cRLInUue4X
+-----END CERTIFICATE-----
+
+# Issuer: CN=GTS Root R4 O=Google Trust Services LLC
+# Subject: CN=GTS Root R4 O=Google Trust Services LLC
+# Label: "GTS Root R4"
+# Serial: 159662532700760215368942768210
+# MD5 Fingerprint: 43:96:83:77:19:4d:76:b3:9d:65:52:e4:1d:22:a5:e8
+# SHA1 Fingerprint: 77:d3:03:67:b5:e0:0c:15:f6:0c:38:61:df:7c:e1:3b:92:46:4d:47
+# SHA256 Fingerprint: 34:9d:fa:40:58:c5:e2:63:12:3b:39:8a:e7:95:57:3c:4e:13:13:c8:3f:e6:8f:93:55:6c:d5:e8:03:1b:3c:7d
+-----BEGIN CERTIFICATE-----
+MIICCTCCAY6gAwIBAgINAgPlwGjvYxqccpBQUjAKBggqhkjOPQQDAzBHMQswCQYD
+VQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEUMBIG
+A1UEAxMLR1RTIFJvb3QgUjQwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAwMDAw
+WjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2Vz
+IExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjQwdjAQBgcqhkjOPQIBBgUrgQQAIgNi
+AATzdHOnaItgrkO4NcWBMHtLSZ37wWHO5t5GvWvVYRg1rkDdc/eJkTBa6zzuhXyi
+QHY7qca4R9gq55KRanPpsXI5nymfopjTX15YhmUPoYRlBtHci8nHc8iMai/lxKvR
+HYqjQjBAMA4GA1UdDwEB/wQEAwIBhjAPBgNVHRMBAf8EBTADAQH/MB0GA1UdDgQW
+BBSATNbrdP9JNqPV2Py1PsVq8JQdjDAKBggqhkjOPQQDAwNpADBmAjEA6ED/g94D
+9J+uHXqnLrmvT/aDHQ4thQEd0dlq7A/Cr8deVl5c1RxYIigL9zC2L7F8AjEA8GE8
+p/SgguMh1YQdc4acLa/KNJvxn7kjNuK8YAOdgLOaVsjh4rsUecrNIdSUtUlD
+-----END CERTIFICATE-----
+
+# Issuer: CN=Telia Root CA v2 O=Telia Finland Oyj
+# Subject: CN=Telia Root CA v2 O=Telia Finland Oyj
+# Label: "Telia Root CA v2"
+# Serial: 7288924052977061235122729490515358
+# MD5 Fingerprint: 0e:8f:ac:aa:82:df:85:b1:f4:dc:10:1c:fc:99:d9:48
+# SHA1 Fingerprint: b9:99:cd:d1:73:50:8a:c4:47:05:08:9c:8c:88:fb:be:a0:2b:40:cd
+# SHA256 Fingerprint: 24:2b:69:74:2f:cb:1e:5b:2a:bf:98:89:8b:94:57:21:87:54:4e:5b:4d:99:11:78:65:73:62:1f:6a:74:b8:2c
+-----BEGIN CERTIFICATE-----
+MIIFdDCCA1ygAwIBAgIPAWdfJ9b+euPkrL4JWwWeMA0GCSqGSIb3DQEBCwUAMEQx
+CzAJBgNVBAYTAkZJMRowGAYDVQQKDBFUZWxpYSBGaW5sYW5kIE95ajEZMBcGA1UE
+AwwQVGVsaWEgUm9vdCBDQSB2MjAeFw0xODExMjkxMTU1NTRaFw00MzExMjkxMTU1
+NTRaMEQxCzAJBgNVBAYTAkZJMRowGAYDVQQKDBFUZWxpYSBGaW5sYW5kIE95ajEZ
+MBcGA1UEAwwQVGVsaWEgUm9vdCBDQSB2MjCCAiIwDQYJKoZIhvcNAQEBBQADggIP
+ADCCAgoCggIBALLQPwe84nvQa5n44ndp586dpAO8gm2h/oFlH0wnrI4AuhZ76zBq
+AMCzdGh+sq/H1WKzej9Qyow2RCRj0jbpDIX2Q3bVTKFgcmfiKDOlyzG4OiIjNLh9
+vVYiQJ3q9HsDrWj8soFPmNB06o3lfc1jw6P23pLCWBnglrvFxKk9pXSW/q/5iaq9
+lRdU2HhE8Qx3FZLgmEKnpNaqIJLNwaCzlrI6hEKNfdWV5Nbb6WLEWLN5xYzTNTOD
+n3WhUidhOPFZPY5Q4L15POdslv5e2QJltI5c0BE0312/UqeBAMN/mUWZFdUXyApT
+7GPzmX3MaRKGwhfwAZ6/hLzRUssbkmbOpFPlob/E2wnW5olWK8jjfN7j/4nlNW4o
+6GwLI1GpJQXrSPjdscr6bAhR77cYbETKJuFzxokGgeWKrLDiKca5JLNrRBH0pUPC
+TEPlcDaMtjNXepUugqD0XBCzYYP2AgWGLnwtbNwDRm41k9V6lS/eINhbfpSQBGq6
+WT0EBXWdN6IOLj3rwaRSg/7Qa9RmjtzG6RJOHSpXqhC8fF6CfaamyfItufUXJ63R
+DolUK5X6wK0dmBR4M0KGCqlztft0DbcbMBnEWg4cJ7faGND/isgFuvGqHKI3t+ZI
+pEYslOqodmJHixBTB0hXbOKSTbauBcvcwUpej6w9GU7C7WB1K9vBykLVAgMBAAGj
+YzBhMB8GA1UdIwQYMBaAFHKs5DN5qkWH9v2sHZ7Wxy+G2CQ5MB0GA1UdDgQWBBRy
+rOQzeapFh/b9rB2e1scvhtgkOTAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0TAQH/BAUw
+AwEB/zANBgkqhkiG9w0BAQsFAAOCAgEAoDtZpwmUPjaE0n4vOaWWl/oRrfxn83EJ
+8rKJhGdEr7nv7ZbsnGTbMjBvZ5qsfl+yqwE2foH65IRe0qw24GtixX1LDoJt0nZi
+0f6X+J8wfBj5tFJ3gh1229MdqfDBmgC9bXXYfef6xzijnHDoRnkDry5023X4blMM
+A8iZGok1GTzTyVR8qPAs5m4HeW9q4ebqkYJpCh3DflminmtGFZhb069GHWLIzoBS
+SRE/yQQSwxN8PzuKlts8oB4KtItUsiRnDe+Cy748fdHif64W1lZYudogsYMVoe+K
+TTJvQS8TUoKU1xrBeKJR3Stwbbca+few4GeXVtt8YVMJAygCQMez2P2ccGrGKMOF
+6eLtGpOg3kuYooQ+BXcBlj37tCAPnHICehIv1aO6UXivKitEZU61/Qrowc15h2Er
+3oBXRb9n8ZuRXqWk7FlIEA04x7D6w0RtBPV4UBySllva9bguulvP5fBqnUsvWHMt
+Ty3EHD70sz+rFQ47GUGKpMFXEmZxTPpT41frYpUJnlTd0cI8Vzy9OK2YZLe4A5pT
+VmBds9hCG1xLEooc6+t9xnppxyd/pPiL8uSUZodL6ZQHCRJ5irLrdATczvREWeAW
+ysUsWNc8e89ihmpQfTU2Zqf7N+cox9jQraVplI/owd8k+BsHMYeB2F326CjYSlKA
+rBPuUBQemMc=
+-----END CERTIFICATE-----
+
+# Issuer: CN=D-TRUST BR Root CA 1 2020 O=D-Trust GmbH
+# Subject: CN=D-TRUST BR Root CA 1 2020 O=D-Trust GmbH
+# Label: "D-TRUST BR Root CA 1 2020"
+# Serial: 165870826978392376648679885835942448534
+# MD5 Fingerprint: b5:aa:4b:d5:ed:f7:e3:55:2e:8f:72:0a:f3:75:b8:ed
+# SHA1 Fingerprint: 1f:5b:98:f0:e3:b5:f7:74:3c:ed:e6:b0:36:7d:32:cd:f4:09:41:67
+# SHA256 Fingerprint: e5:9a:aa:81:60:09:c2:2b:ff:5b:25:ba:d3:7d:f3:06:f0:49:79:7c:1f:81:d8:5a:b0:89:e6:57:bd:8f:00:44
+-----BEGIN CERTIFICATE-----
+MIIC2zCCAmCgAwIBAgIQfMmPK4TX3+oPyWWa00tNljAKBggqhkjOPQQDAzBIMQsw
+CQYDVQQGEwJERTEVMBMGA1UEChMMRC1UcnVzdCBHbWJIMSIwIAYDVQQDExlELVRS
+VVNUIEJSIFJvb3QgQ0EgMSAyMDIwMB4XDTIwMDIxMTA5NDUwMFoXDTM1MDIxMTA5
+NDQ1OVowSDELMAkGA1UEBhMCREUxFTATBgNVBAoTDEQtVHJ1c3QgR21iSDEiMCAG
+A1UEAxMZRC1UUlVTVCBCUiBSb290IENBIDEgMjAyMDB2MBAGByqGSM49AgEGBSuB
+BAAiA2IABMbLxyjR+4T1mu9CFCDhQ2tuda38KwOE1HaTJddZO0Flax7mNCq7dPYS
+zuht56vkPE4/RAiLzRZxy7+SmfSk1zxQVFKQhYN4lGdnoxwJGT11NIXe7WB9xwy0
+QVK5buXuQqOCAQ0wggEJMA8GA1UdEwEB/wQFMAMBAf8wHQYDVR0OBBYEFHOREKv/
+VbNafAkl1bK6CKBrqx9tMA4GA1UdDwEB/wQEAwIBBjCBxgYDVR0fBIG+MIG7MD6g
+PKA6hjhodHRwOi8vY3JsLmQtdHJ1c3QubmV0L2NybC9kLXRydXN0X2JyX3Jvb3Rf
+Y2FfMV8yMDIwLmNybDB5oHegdYZzbGRhcDovL2RpcmVjdG9yeS5kLXRydXN0Lm5l
+dC9DTj1ELVRSVVNUJTIwQlIlMjBSb290JTIwQ0ElMjAxJTIwMjAyMCxPPUQtVHJ1
+c3QlMjBHbWJILEM9REU/Y2VydGlmaWNhdGVyZXZvY2F0aW9ubGlzdDAKBggqhkjO
+PQQDAwNpADBmAjEAlJAtE/rhY/hhY+ithXhUkZy4kzg+GkHaQBZTQgjKL47xPoFW
+wKrY7RjEsK70PvomAjEA8yjixtsrmfu3Ubgko6SUeho/5jbiA1czijDLgsfWFBHV
+dWNbFJWcHwHP2NVypw87
+-----END CERTIFICATE-----
+
+# Issuer: CN=D-TRUST EV Root CA 1 2020 O=D-Trust GmbH
+# Subject: CN=D-TRUST EV Root CA 1 2020 O=D-Trust GmbH
+# Label: "D-TRUST EV Root CA 1 2020"
+# Serial: 126288379621884218666039612629459926992
+# MD5 Fingerprint: 8c:2d:9d:70:9f:48:99:11:06:11:fb:e9:cb:30:c0:6e
+# SHA1 Fingerprint: 61:db:8c:21:59:69:03:90:d8:7c:9c:12:86:54:cf:9d:3d:f4:dd:07
+# SHA256 Fingerprint: 08:17:0d:1a:a3:64:53:90:1a:2f:95:92:45:e3:47:db:0c:8d:37:ab:aa:bc:56:b8:1a:a1:00:dc:95:89:70:db
+-----BEGIN CERTIFICATE-----
+MIIC2zCCAmCgAwIBAgIQXwJB13qHfEwDo6yWjfv/0DAKBggqhkjOPQQDAzBIMQsw
+CQYDVQQGEwJERTEVMBMGA1UEChMMRC1UcnVzdCBHbWJIMSIwIAYDVQQDExlELVRS
+VVNUIEVWIFJvb3QgQ0EgMSAyMDIwMB4XDTIwMDIxMTEwMDAwMFoXDTM1MDIxMTA5
+NTk1OVowSDELMAkGA1UEBhMCREUxFTATBgNVBAoTDEQtVHJ1c3QgR21iSDEiMCAG
+A1UEAxMZRC1UUlVTVCBFViBSb290IENBIDEgMjAyMDB2MBAGByqGSM49AgEGBSuB
+BAAiA2IABPEL3YZDIBnfl4XoIkqbz52Yv7QFJsnL46bSj8WeeHsxiamJrSc8ZRCC
+/N/DnU7wMyPE0jL1HLDfMxddxfCxivnvubcUyilKwg+pf3VlSSowZ/Rk99Yad9rD
+wpdhQntJraOCAQ0wggEJMA8GA1UdEwEB/wQFMAMBAf8wHQYDVR0OBBYEFH8QARY3
+OqQo5FD4pPfsazK2/umLMA4GA1UdDwEB/wQEAwIBBjCBxgYDVR0fBIG+MIG7MD6g
+PKA6hjhodHRwOi8vY3JsLmQtdHJ1c3QubmV0L2NybC9kLXRydXN0X2V2X3Jvb3Rf
+Y2FfMV8yMDIwLmNybDB5oHegdYZzbGRhcDovL2RpcmVjdG9yeS5kLXRydXN0Lm5l
+dC9DTj1ELVRSVVNUJTIwRVYlMjBSb290JTIwQ0ElMjAxJTIwMjAyMCxPPUQtVHJ1
+c3QlMjBHbWJILEM9REU/Y2VydGlmaWNhdGVyZXZvY2F0aW9ubGlzdDAKBggqhkjO
+PQQDAwNpADBmAjEAyjzGKnXCXnViOTYAYFqLwZOZzNnbQTs7h5kXO9XMT8oi96CA
+y/m0sRtW9XLS/BnRAjEAkfcwkz8QRitxpNA7RJvAKQIFskF3UfN5Wp6OFKBOQtJb
+gfM0agPnIjhQW+0ZT0MW
+-----END CERTIFICATE-----
+
+# Issuer: CN=DigiCert TLS ECC P384 Root G5 O=DigiCert, Inc.
+# Subject: CN=DigiCert TLS ECC P384 Root G5 O=DigiCert, Inc.
+# Label: "DigiCert TLS ECC P384 Root G5"
+# Serial: 13129116028163249804115411775095713523
+# MD5 Fingerprint: d3:71:04:6a:43:1c:db:a6:59:e1:a8:a3:aa:c5:71:ed
+# SHA1 Fingerprint: 17:f3:de:5e:9f:0f:19:e9:8e:f6:1f:32:26:6e:20:c4:07:ae:30:ee
+# SHA256 Fingerprint: 01:8e:13:f0:77:25:32:cf:80:9b:d1:b1:72:81:86:72:83:fc:48:c6:e1:3b:e9:c6:98:12:85:4a:49:0c:1b:05
+-----BEGIN CERTIFICATE-----
+MIICGTCCAZ+gAwIBAgIQCeCTZaz32ci5PhwLBCou8zAKBggqhkjOPQQDAzBOMQsw
+CQYDVQQGEwJVUzEXMBUGA1UEChMORGlnaUNlcnQsIEluYy4xJjAkBgNVBAMTHURp
+Z2lDZXJ0IFRMUyBFQ0MgUDM4NCBSb290IEc1MB4XDTIxMDExNTAwMDAwMFoXDTQ2
+MDExNDIzNTk1OVowTjELMAkGA1UEBhMCVVMxFzAVBgNVBAoTDkRpZ2lDZXJ0LCBJ
+bmMuMSYwJAYDVQQDEx1EaWdpQ2VydCBUTFMgRUNDIFAzODQgUm9vdCBHNTB2MBAG
+ByqGSM49AgEGBSuBBAAiA2IABMFEoc8Rl1Ca3iOCNQfN0MsYndLxf3c1TzvdlHJS
+7cI7+Oz6e2tYIOyZrsn8aLN1udsJ7MgT9U7GCh1mMEy7H0cKPGEQQil8pQgO4CLp
+0zVozptjn4S1mU1YoI71VOeVyaNCMEAwHQYDVR0OBBYEFMFRRVBZqz7nLFr6ICIS
+B4CIfBFqMA4GA1UdDwEB/wQEAwIBhjAPBgNVHRMBAf8EBTADAQH/MAoGCCqGSM49
+BAMDA2gAMGUCMQCJao1H5+z8blUD2WdsJk6Dxv3J+ysTvLd6jLRl0mlpYxNjOyZQ
+LgGheQaRnUi/wr4CMEfDFXuxoJGZSZOoPHzoRgaLLPIxAJSdYsiJvRmEFOml+wG4
+DXZDjC5Ty3zfDBeWUA==
+-----END CERTIFICATE-----
+
+# Issuer: CN=DigiCert TLS RSA4096 Root G5 O=DigiCert, Inc.
+# Subject: CN=DigiCert TLS RSA4096 Root G5 O=DigiCert, Inc.
+# Label: "DigiCert TLS RSA4096 Root G5"
+# Serial: 11930366277458970227240571539258396554
+# MD5 Fingerprint: ac:fe:f7:34:96:a9:f2:b3:b4:12:4b:e4:27:41:6f:e1
+# SHA1 Fingerprint: a7:88:49:dc:5d:7c:75:8c:8c:de:39:98:56:b3:aa:d0:b2:a5:71:35
+# SHA256 Fingerprint: 37:1a:00:dc:05:33:b3:72:1a:7e:eb:40:e8:41:9e:70:79:9d:2b:0a:0f:2c:1d:80:69:31:65:f7:ce:c4:ad:75
+-----BEGIN CERTIFICATE-----
+MIIFZjCCA06gAwIBAgIQCPm0eKj6ftpqMzeJ3nzPijANBgkqhkiG9w0BAQwFADBN
+MQswCQYDVQQGEwJVUzEXMBUGA1UEChMORGlnaUNlcnQsIEluYy4xJTAjBgNVBAMT
+HERpZ2lDZXJ0IFRMUyBSU0E0MDk2IFJvb3QgRzUwHhcNMjEwMTE1MDAwMDAwWhcN
+NDYwMTE0MjM1OTU5WjBNMQswCQYDVQQGEwJVUzEXMBUGA1UEChMORGlnaUNlcnQs
+IEluYy4xJTAjBgNVBAMTHERpZ2lDZXJ0IFRMUyBSU0E0MDk2IFJvb3QgRzUwggIi
+MA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQCz0PTJeRGd/fxmgefM1eS87IE+
+ajWOLrfn3q/5B03PMJ3qCQuZvWxX2hhKuHisOjmopkisLnLlvevxGs3npAOpPxG0
+2C+JFvuUAT27L/gTBaF4HI4o4EXgg/RZG5Wzrn4DReW+wkL+7vI8toUTmDKdFqgp
+wgscONyfMXdcvyej/Cestyu9dJsXLfKB2l2w4SMXPohKEiPQ6s+d3gMXsUJKoBZM
+pG2T6T867jp8nVid9E6P/DsjyG244gXazOvswzH016cpVIDPRFtMbzCe88zdH5RD
+nU1/cHAN1DrRN/BsnZvAFJNY781BOHW8EwOVfH/jXOnVDdXifBBiqmvwPXbzP6Po
+sMH976pXTayGpxi0KcEsDr9kvimM2AItzVwv8n/vFfQMFawKsPHTDU9qTXeXAaDx
+Zre3zu/O7Oyldcqs4+Fj97ihBMi8ez9dLRYiVu1ISf6nL3kwJZu6ay0/nTvEF+cd
+Lvvyz6b84xQslpghjLSR6Rlgg/IwKwZzUNWYOwbpx4oMYIwo+FKbbuH2TbsGJJvX
+KyY//SovcfXWJL5/MZ4PbeiPT02jP/816t9JXkGPhvnxd3lLG7SjXi/7RgLQZhNe
+XoVPzthwiHvOAbWWl9fNff2C+MIkwcoBOU+NosEUQB+cZtUMCUbW8tDRSHZWOkPL
+tgoRObqME2wGtZ7P6wIDAQABo0IwQDAdBgNVHQ4EFgQUUTMc7TZArxfTJc1paPKv
+TiM+s0EwDgYDVR0PAQH/BAQDAgGGMA8GA1UdEwEB/wQFMAMBAf8wDQYJKoZIhvcN
+AQEMBQADggIBAGCmr1tfV9qJ20tQqcQjNSH/0GEwhJG3PxDPJY7Jv0Y02cEhJhxw
+GXIeo8mH/qlDZJY6yFMECrZBu8RHANmfGBg7sg7zNOok992vIGCukihfNudd5N7H
+PNtQOa27PShNlnx2xlv0wdsUpasZYgcYQF+Xkdycx6u1UQ3maVNVzDl92sURVXLF
+O4uJ+DQtpBflF+aZfTCIITfNMBc9uPK8qHWgQ9w+iUuQrm0D4ByjoJYJu32jtyoQ
+REtGBzRj7TG5BO6jm5qu5jF49OokYTurWGT/u4cnYiWB39yhL/btp/96j1EuMPik
+AdKFOV8BmZZvWltwGUb+hmA+rYAQCd05JS9Yf7vSdPD3Rh9GOUrYU9DzLjtxpdRv
+/PNn5AeP3SYZ4Y1b+qOTEZvpyDrDVWiakuFSdjjo4bq9+0/V77PnSIMx8IIh47a+
+p6tv75/fTM8BuGJqIz3nCU2AG3swpMPdB380vqQmsvZB6Akd4yCYqjdP//fx4ilw
+MUc/dNAUFvohigLVigmUdy7yWSiLfFCSCmZ4OIN1xLVaqBHG5cGdZlXPU8Sv13WF
+qUITVuwhd4GTWgzqltlJyqEI8pc7bZsEGCREjnwB8twl2F6GmrE52/WRMmrRpnCK
+ovfepEWFJqgejF0pW8hL2JpqA15w8oVPbEtoL8pU9ozaMv7Da4M/OMZ+
+-----END CERTIFICATE-----
+
+# Issuer: CN=Certainly Root R1 O=Certainly
+# Subject: CN=Certainly Root R1 O=Certainly
+# Label: "Certainly Root R1"
+# Serial: 188833316161142517227353805653483829216
+# MD5 Fingerprint: 07:70:d4:3e:82:87:a0:fa:33:36:13:f4:fa:33:e7:12
+# SHA1 Fingerprint: a0:50:ee:0f:28:71:f4:27:b2:12:6d:6f:50:96:25:ba:cc:86:42:af
+# SHA256 Fingerprint: 77:b8:2c:d8:64:4c:43:05:f7:ac:c5:cb:15:6b:45:67:50:04:03:3d:51:c6:0c:62:02:a8:e0:c3:34:67:d3:a0
+-----BEGIN CERTIFICATE-----
+MIIFRzCCAy+gAwIBAgIRAI4P+UuQcWhlM1T01EQ5t+AwDQYJKoZIhvcNAQELBQAw
+PTELMAkGA1UEBhMCVVMxEjAQBgNVBAoTCUNlcnRhaW5seTEaMBgGA1UEAxMRQ2Vy
+dGFpbmx5IFJvb3QgUjEwHhcNMjEwNDAxMDAwMDAwWhcNNDYwNDAxMDAwMDAwWjA9
+MQswCQYDVQQGEwJVUzESMBAGA1UEChMJQ2VydGFpbmx5MRowGAYDVQQDExFDZXJ0
+YWlubHkgUm9vdCBSMTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBANA2
+1B/q3avk0bbm+yLA3RMNansiExyXPGhjZjKcA7WNpIGD2ngwEc/csiu+kr+O5MQT
+vqRoTNoCaBZ0vrLdBORrKt03H2As2/X3oXyVtwxwhi7xOu9S98zTm/mLvg7fMbed
+aFySpvXl8wo0tf97ouSHocavFwDvA5HtqRxOcT3Si2yJ9HiG5mpJoM610rCrm/b0
+1C7jcvk2xusVtyWMOvwlDbMicyF0yEqWYZL1LwsYpfSt4u5BvQF5+paMjRcCMLT5
+r3gajLQ2EBAHBXDQ9DGQilHFhiZ5shGIXsXwClTNSaa/ApzSRKft43jvRl5tcdF5
+cBxGX1HpyTfcX35pe0HfNEXgO4T0oYoKNp43zGJS4YkNKPl6I7ENPT2a/Z2B7yyQ
+wHtETrtJ4A5KVpK8y7XdeReJkd5hiXSSqOMyhb5OhaRLWcsrxXiOcVTQAjeZjOVJ
+6uBUcqQRBi8LjMFbvrWhsFNunLhgkR9Za/kt9JQKl7XsxXYDVBtlUrpMklZRNaBA
+2CnbrlJ2Oy0wQJuK0EJWtLeIAaSHO1OWzaMWj/Nmqhexx2DgwUMFDO6bW2BvBlyH
+Wyf5QBGenDPBt+U1VwV/J84XIIwc/PH72jEpSe31C4SnT8H2TsIonPru4K8H+zMR
+eiFPCyEQtkA6qyI6BJyLm4SGcprSp6XEtHWRqSsjAgMBAAGjQjBAMA4GA1UdDwEB
+/wQEAwIBBjAPBgNVHRMBAf8EBTADAQH/MB0GA1UdDgQWBBTgqj8ljZ9EXME66C6u
+d0yEPmcM9DANBgkqhkiG9w0BAQsFAAOCAgEAuVevuBLaV4OPaAszHQNTVfSVcOQr
+PbA56/qJYv331hgELyE03fFo8NWWWt7CgKPBjcZq91l3rhVkz1t5BXdm6ozTaw3d
+8VkswTOlMIAVRQdFGjEitpIAq5lNOo93r6kiyi9jyhXWx8bwPWz8HA2YEGGeEaIi
+1wrykXprOQ4vMMM2SZ/g6Q8CRFA3lFV96p/2O7qUpUzpvD5RtOjKkjZUbVwlKNrd
+rRT90+7iIgXr0PK3aBLXWopBGsaSpVo7Y0VPv+E6dyIvXL9G+VoDhRNCX8reU9di
+taY1BMJH/5n9hN9czulegChB8n3nHpDYT3Y+gjwN/KUD+nsa2UUeYNrEjvn8K8l7
+lcUq/6qJ34IxD3L/DCfXCh5WAFAeDJDBlrXYFIW7pw0WwfgHJBu6haEaBQmAupVj
+yTrsJZ9/nbqkRxWbRHDxakvWOF5D8xh+UG7pWijmZeZ3Gzr9Hb4DJqPb1OG7fpYn
+Kx3upPvaJVQTA945xsMfTZDsjxtK0hzthZU4UHlG1sGQUDGpXJpuHfUzVounmdLy
+yCwzk5Iwx06MZTMQZBf9JBeW0Y3COmor6xOLRPIh80oat3df1+2IpHLlOR+Vnb5n
+wXARPbv0+Em34yaXOp/SX3z7wJl8OSngex2/DaeP0ik0biQVy96QXr8axGbqwua6
+OV+KmalBWQewLK8=
+-----END CERTIFICATE-----
+
+# Issuer: CN=Certainly Root E1 O=Certainly
+# Subject: CN=Certainly Root E1 O=Certainly
+# Label: "Certainly Root E1"
+# Serial: 8168531406727139161245376702891150584
+# MD5 Fingerprint: 0a:9e:ca:cd:3e:52:50:c6:36:f3:4b:a3:ed:a7:53:e9
+# SHA1 Fingerprint: f9:e1:6d:dc:01:89:cf:d5:82:45:63:3e:c5:37:7d:c2:eb:93:6f:2b
+# SHA256 Fingerprint: b4:58:5f:22:e4:ac:75:6a:4e:86:12:a1:36:1c:5d:9d:03:1a:93:fd:84:fe:bb:77:8f:a3:06:8b:0f:c4:2d:c2
+-----BEGIN CERTIFICATE-----
+MIIB9zCCAX2gAwIBAgIQBiUzsUcDMydc+Y2aub/M+DAKBggqhkjOPQQDAzA9MQsw
+CQYDVQQGEwJVUzESMBAGA1UEChMJQ2VydGFpbmx5MRowGAYDVQQDExFDZXJ0YWlu
+bHkgUm9vdCBFMTAeFw0yMTA0MDEwMDAwMDBaFw00NjA0MDEwMDAwMDBaMD0xCzAJ
+BgNVBAYTAlVTMRIwEAYDVQQKEwlDZXJ0YWlubHkxGjAYBgNVBAMTEUNlcnRhaW5s
+eSBSb290IEUxMHYwEAYHKoZIzj0CAQYFK4EEACIDYgAE3m/4fxzf7flHh4axpMCK
++IKXgOqPyEpeKn2IaKcBYhSRJHpcnqMXfYqGITQYUBsQ3tA3SybHGWCA6TS9YBk2
+QNYphwk8kXr2vBMj3VlOBF7PyAIcGFPBMdjaIOlEjeR2o0IwQDAOBgNVHQ8BAf8E
+BAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQU8ygYy2R17ikq6+2uI1g4
+hevIIgcwCgYIKoZIzj0EAwMDaAAwZQIxALGOWiDDshliTd6wT99u0nCK8Z9+aozm
+ut6Dacpps6kFtZaSF4fC0urQe87YQVt8rgIwRt7qy12a7DLCZRawTDBcMPPaTnOG
+BtjOiQRINzf43TNRnXCve1XYAS59BWQOhriR
+-----END CERTIFICATE-----
+
+# Issuer: CN=E-Tugra Global Root CA RSA v3 O=E-Tugra EBG A.S. OU=E-Tugra Trust Center
+# Subject: CN=E-Tugra Global Root CA RSA v3 O=E-Tugra EBG A.S. OU=E-Tugra Trust Center
+# Label: "E-Tugra Global Root CA RSA v3"
+# Serial: 75951268308633135324246244059508261641472512052
+# MD5 Fingerprint: 22:be:10:f6:c2:f8:03:88:73:5f:33:29:47:28:47:a4
+# SHA1 Fingerprint: e9:a8:5d:22:14:52:1c:5b:aa:0a:b4:be:24:6a:23:8a:c9:ba:e2:a9
+# SHA256 Fingerprint: ef:66:b0:b1:0a:3c:db:9f:2e:36:48:c7:6b:d2:af:18:ea:d2:bf:e6:f1:17:65:5e:28:c4:06:0d:a1:a3:f4:c2
+-----BEGIN CERTIFICATE-----
+MIIF8zCCA9ugAwIBAgIUDU3FzRYilZYIfrgLfxUGNPt5EDQwDQYJKoZIhvcNAQEL
+BQAwgYAxCzAJBgNVBAYTAlRSMQ8wDQYDVQQHEwZBbmthcmExGTAXBgNVBAoTEEUt
+VHVncmEgRUJHIEEuUy4xHTAbBgNVBAsTFEUtVHVncmEgVHJ1c3QgQ2VudGVyMSYw
+JAYDVQQDEx1FLVR1Z3JhIEdsb2JhbCBSb290IENBIFJTQSB2MzAeFw0yMDAzMTgw
+OTA3MTdaFw00NTAzMTIwOTA3MTdaMIGAMQswCQYDVQQGEwJUUjEPMA0GA1UEBxMG
+QW5rYXJhMRkwFwYDVQQKExBFLVR1Z3JhIEVCRyBBLlMuMR0wGwYDVQQLExRFLVR1
+Z3JhIFRydXN0IENlbnRlcjEmMCQGA1UEAxMdRS1UdWdyYSBHbG9iYWwgUm9vdCBD
+QSBSU0EgdjMwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQCiZvCJt3J7
+7gnJY9LTQ91ew6aEOErxjYG7FL1H6EAX8z3DeEVypi6Q3po61CBxyryfHUuXCscx
+uj7X/iWpKo429NEvx7epXTPcMHD4QGxLsqYxYdE0PD0xesevxKenhOGXpOhL9hd8
+7jwH7eKKV9y2+/hDJVDqJ4GohryPUkqWOmAalrv9c/SF/YP9f4RtNGx/ardLAQO/
+rWm31zLZ9Vdq6YaCPqVmMbMWPcLzJmAy01IesGykNz709a/r4d+ABs8qQedmCeFL
+l+d3vSFtKbZnwy1+7dZ5ZdHPOrbRsV5WYVB6Ws5OUDGAA5hH5+QYfERaxqSzO8bG
+wzrwbMOLyKSRBfP12baqBqG3q+Sx6iEUXIOk/P+2UNOMEiaZdnDpwA+mdPy70Bt4
+znKS4iicvObpCdg604nmvi533wEKb5b25Y08TVJ2Glbhc34XrD2tbKNSEhhw5oBO
+M/J+JjKsBY04pOZ2PJ8QaQ5tndLBeSBrW88zjdGUdjXnXVXHt6woq0bM5zshtQoK
+5EpZ3IE1S0SVEgpnpaH/WwAH0sDM+T/8nzPyAPiMbIedBi3x7+PmBvrFZhNb/FAH
+nnGGstpvdDDPk1Po3CLW3iAfYY2jLqN4MpBs3KwytQXk9TwzDdbgh3cXTJ2w2Amo
+DVf3RIXwyAS+XF1a4xeOVGNpf0l0ZAWMowIDAQABo2MwYTAPBgNVHRMBAf8EBTAD
+AQH/MB8GA1UdIwQYMBaAFLK0ruYt9ybVqnUtdkvAG1Mh0EjvMB0GA1UdDgQWBBSy
+tK7mLfcm1ap1LXZLwBtTIdBI7zAOBgNVHQ8BAf8EBAMCAQYwDQYJKoZIhvcNAQEL
+BQADggIBAImocn+M684uGMQQgC0QDP/7FM0E4BQ8Tpr7nym/Ip5XuYJzEmMmtcyQ
+6dIqKe6cLcwsmb5FJ+Sxce3kOJUxQfJ9emN438o2Fi+CiJ+8EUdPdk3ILY7r3y18
+Tjvarvbj2l0Upq7ohUSdBm6O++96SmotKygY/r+QLHUWnw/qln0F7psTpURs+APQ
+3SPh/QMSEgj0GDSz4DcLdxEBSL9htLX4GdnLTeqjjO/98Aa1bZL0SmFQhO3sSdPk
+vmjmLuMxC1QLGpLWgti2omU8ZgT5Vdps+9u1FGZNlIM7zR6mK7L+d0CGq+ffCsn9
+9t2HVhjYsCxVYJb6CH5SkPVLpi6HfMsg2wY+oF0Dd32iPBMbKaITVaA9FCKvb7jQ
+mhty3QUBjYZgv6Rn7rWlDdF/5horYmbDB7rnoEgcOMPpRfunf/ztAmgayncSd6YA
+VSgU7NbHEqIbZULpkejLPoeJVF3Zr52XnGnnCv8PWniLYypMfUeUP95L6VPQMPHF
+9p5J3zugkaOj/s1YzOrfr28oO6Bpm4/srK4rVJ2bBLFHIK+WEj5jlB0E5y67hscM
+moi/dkfv97ALl2bSRM9gUgfh1SxKOidhd8rXj+eHDjD/DLsE4mHDosiXYY60MGo8
+bcIHX0pzLz/5FooBZu+6kcpSV3uu1OYP3Qt6f4ueJiDPO++BcYNZ
+-----END CERTIFICATE-----
+
+# Issuer: CN=E-Tugra Global Root CA ECC v3 O=E-Tugra EBG A.S. OU=E-Tugra Trust Center
+# Subject: CN=E-Tugra Global Root CA ECC v3 O=E-Tugra EBG A.S. OU=E-Tugra Trust Center
+# Label: "E-Tugra Global Root CA ECC v3"
+# Serial: 218504919822255052842371958738296604628416471745
+# MD5 Fingerprint: 46:bc:81:bb:f1:b5:1e:f7:4b:96:bc:14:e2:e7:27:64
+# SHA1 Fingerprint: 8a:2f:af:57:53:b1:b0:e6:a1:04:ec:5b:6a:69:71:6d:f6:1c:e2:84
+# SHA256 Fingerprint: 87:3f:46:85:fa:7f:56:36:25:25:2e:6d:36:bc:d7:f1:6f:c2:49:51:f2:64:e4:7e:1b:95:4f:49:08:cd:ca:13
+-----BEGIN CERTIFICATE-----
+MIICpTCCAiqgAwIBAgIUJkYZdzHhT28oNt45UYbm1JeIIsEwCgYIKoZIzj0EAwMw
+gYAxCzAJBgNVBAYTAlRSMQ8wDQYDVQQHEwZBbmthcmExGTAXBgNVBAoTEEUtVHVn
+cmEgRUJHIEEuUy4xHTAbBgNVBAsTFEUtVHVncmEgVHJ1c3QgQ2VudGVyMSYwJAYD
+VQQDEx1FLVR1Z3JhIEdsb2JhbCBSb290IENBIEVDQyB2MzAeFw0yMDAzMTgwOTQ2
+NThaFw00NTAzMTIwOTQ2NThaMIGAMQswCQYDVQQGEwJUUjEPMA0GA1UEBxMGQW5r
+YXJhMRkwFwYDVQQKExBFLVR1Z3JhIEVCRyBBLlMuMR0wGwYDVQQLExRFLVR1Z3Jh
+IFRydXN0IENlbnRlcjEmMCQGA1UEAxMdRS1UdWdyYSBHbG9iYWwgUm9vdCBDQSBF
+Q0MgdjMwdjAQBgcqhkjOPQIBBgUrgQQAIgNiAASOmCm/xxAeJ9urA8woLNheSBkQ
+KczLWYHMjLiSF4mDKpL2w6QdTGLVn9agRtwcvHbB40fQWxPa56WzZkjnIZpKT4YK
+fWzqTTKACrJ6CZtpS5iB4i7sAnCWH/31Rs7K3IKjYzBhMA8GA1UdEwEB/wQFMAMB
+Af8wHwYDVR0jBBgwFoAU/4Ixcj75xGZsrTie0bBRiKWQzPUwHQYDVR0OBBYEFP+C
+MXI++cRmbK04ntGwUYilkMz1MA4GA1UdDwEB/wQEAwIBBjAKBggqhkjOPQQDAwNp
+ADBmAjEA5gVYaWHlLcoNy/EZCL3W/VGSGn5jVASQkZo1kTmZ+gepZpO6yGjUij/6
+7W4WAie3AjEA3VoXK3YdZUKWpqxdinlW2Iob35reX8dQj7FbcQwm32pAAOwzkSFx
+vmjkI6TZraE3
+-----END CERTIFICATE-----
+
+# Issuer: CN=Security Communication RootCA3 O=SECOM Trust Systems CO.,LTD.
+# Subject: CN=Security Communication RootCA3 O=SECOM Trust Systems CO.,LTD.
+# Label: "Security Communication RootCA3"
+# Serial: 16247922307909811815
+# MD5 Fingerprint: 1c:9a:16:ff:9e:5c:e0:4d:8a:14:01:f4:35:5d:29:26
+# SHA1 Fingerprint: c3:03:c8:22:74:92:e5:61:a2:9c:5f:79:91:2b:1e:44:13:91:30:3a
+# SHA256 Fingerprint: 24:a5:5c:2a:b0:51:44:2d:06:17:76:65:41:23:9a:4a:d0:32:d7:c5:51:75:aa:34:ff:de:2f:bc:4f:5c:52:94
+-----BEGIN CERTIFICATE-----
+MIIFfzCCA2egAwIBAgIJAOF8N0D9G/5nMA0GCSqGSIb3DQEBDAUAMF0xCzAJBgNV
+BAYTAkpQMSUwIwYDVQQKExxTRUNPTSBUcnVzdCBTeXN0ZW1zIENPLixMVEQuMScw
+JQYDVQQDEx5TZWN1cml0eSBDb21tdW5pY2F0aW9uIFJvb3RDQTMwHhcNMTYwNjE2
+MDYxNzE2WhcNMzgwMTE4MDYxNzE2WjBdMQswCQYDVQQGEwJKUDElMCMGA1UEChMc
+U0VDT00gVHJ1c3QgU3lzdGVtcyBDTy4sTFRELjEnMCUGA1UEAxMeU2VjdXJpdHkg
+Q29tbXVuaWNhdGlvbiBSb290Q0EzMIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIIC
+CgKCAgEA48lySfcw3gl8qUCBWNO0Ot26YQ+TUG5pPDXC7ltzkBtnTCHsXzW7OT4r
+CmDvu20rhvtxosis5FaU+cmvsXLUIKx00rgVrVH+hXShuRD+BYD5UpOzQD11EKzA
+lrenfna84xtSGc4RHwsENPXY9Wk8d/Nk9A2qhd7gCVAEF5aEt8iKvE1y/By7z/MG
+TfmfZPd+pmaGNXHIEYBMwXFAWB6+oHP2/D5Q4eAvJj1+XCO1eXDe+uDRpdYMQXF7
+9+qMHIjH7Iv10S9VlkZ8WjtYO/u62C21Jdp6Ts9EriGmnpjKIG58u4iFW/vAEGK7
+8vknR+/RiTlDxN/e4UG/VHMgly1s2vPUB6PmudhvrvyMGS7TZ2crldtYXLVqAvO4
+g160a75BflcJdURQVc1aEWEhCmHCqYj9E7wtiS/NYeCVvsq1e+F7NGcLH7YMx3we
+GVPKp7FKFSBWFHA9K4IsD50VHUeAR/94mQ4xr28+j+2GaR57GIgUssL8gjMunEst
++3A7caoreyYn8xrC3PsXuKHqy6C0rtOUfnrQq8PsOC0RLoi/1D+tEjtCrI8Cbn3M
+0V9hvqG8OmpI6iZVIhZdXw3/JzOfGAN0iltSIEdrRU0id4xVJ/CvHozJgyJUt5rQ
+T9nO/NkuHJYosQLTA70lUhw0Zk8jq/R3gpYd0VcwCBEF/VfR2ccCAwEAAaNCMEAw
+HQYDVR0OBBYEFGQUfPxYchamCik0FW8qy7z8r6irMA4GA1UdDwEB/wQEAwIBBjAP
+BgNVHRMBAf8EBTADAQH/MA0GCSqGSIb3DQEBDAUAA4ICAQDcAiMI4u8hOscNtybS
+YpOnpSNyByCCYN8Y11StaSWSntkUz5m5UoHPrmyKO1o5yGwBQ8IibQLwYs1OY0PA
+FNr0Y/Dq9HHuTofjcan0yVflLl8cebsjqodEV+m9NU1Bu0soo5iyG9kLFwfl9+qd
+9XbXv8S2gVj/yP9kaWJ5rW4OH3/uHWnlt3Jxs/6lATWUVCvAUm2PVcTJ0rjLyjQI
+UYWg9by0F1jqClx6vWPGOi//lkkZhOpn2ASxYfQAW0q3nHE3GYV5v4GwxxMOdnE+
+OoAGrgYWp421wsTL/0ClXI2lyTrtcoHKXJg80jQDdwj98ClZXSEIx2C/pHF7uNke
+gr4Jr2VvKKu/S7XuPghHJ6APbw+LP6yVGPO5DtxnVW5inkYO0QR4ynKudtml+LLf
+iAlhi+8kTtFZP1rUPcmTPCtk9YENFpb3ksP+MW/oKjJ0DvRMmEoYDjBU1cXrvMUV
+nuiZIesnKwkK2/HmcBhWuwzkvvnoEKQTkrgc4NtnHVMDpCKn3F2SEDzq//wbEBrD
+2NCcnWXL0CsnMQMeNuE9dnUM/0Umud1RvCPHX9jYhxBAEg09ODfnRDwYwFMJZI//
+1ZqmfHAuc1Uh6N//g7kdPjIe1qZ9LPFm6Vwdp6POXiUyK+OVrCoHzrQoeIY8Laad
+TdJ0MN1kURXbg4NR16/9M51NZg==
+-----END CERTIFICATE-----
+
+# Issuer: CN=Security Communication ECC RootCA1 O=SECOM Trust Systems CO.,LTD.
+# Subject: CN=Security Communication ECC RootCA1 O=SECOM Trust Systems CO.,LTD.
+# Label: "Security Communication ECC RootCA1"
+# Serial: 15446673492073852651
+# MD5 Fingerprint: 7e:43:b0:92:68:ec:05:43:4c:98:ab:5d:35:2e:7e:86
+# SHA1 Fingerprint: b8:0e:26:a9:bf:d2:b2:3b:c0:ef:46:c9:ba:c7:bb:f6:1d:0d:41:41
+# SHA256 Fingerprint: e7:4f:bd:a5:5b:d5:64:c4:73:a3:6b:44:1a:a7:99:c8:a6:8e:07:74:40:e8:28:8b:9f:a1:e5:0e:4b:ba:ca:11
+-----BEGIN CERTIFICATE-----
+MIICODCCAb6gAwIBAgIJANZdm7N4gS7rMAoGCCqGSM49BAMDMGExCzAJBgNVBAYT
+AkpQMSUwIwYDVQQKExxTRUNPTSBUcnVzdCBTeXN0ZW1zIENPLixMVEQuMSswKQYD
+VQQDEyJTZWN1cml0eSBDb21tdW5pY2F0aW9uIEVDQyBSb290Q0ExMB4XDTE2MDYx
+NjA1MTUyOFoXDTM4MDExODA1MTUyOFowYTELMAkGA1UEBhMCSlAxJTAjBgNVBAoT
+HFNFQ09NIFRydXN0IFN5c3RlbXMgQ08uLExURC4xKzApBgNVBAMTIlNlY3VyaXR5
+IENvbW11bmljYXRpb24gRUNDIFJvb3RDQTEwdjAQBgcqhkjOPQIBBgUrgQQAIgNi
+AASkpW9gAwPDvTH00xecK4R1rOX9PVdu12O/5gSJko6BnOPpR27KkBLIE+Cnnfdl
+dB9sELLo5OnvbYUymUSxXv3MdhDYW72ixvnWQuRXdtyQwjWpS4g8EkdtXP9JTxpK
+ULGjQjBAMB0GA1UdDgQWBBSGHOf+LaVKiwj+KBH6vqNm+GBZLzAOBgNVHQ8BAf8E
+BAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAKBggqhkjOPQQDAwNoADBlAjAVXUI9/Lbu
+9zuxNuie9sRGKEkz0FhDKmMpzE2xtHqiuQ04pV1IKv3LsnNdo4gIxwwCMQDAqy0O
+be0YottT6SXbVQjgUMzfRGEWgqtJsLKB7HOHeLRMsmIbEvoWTSVLY70eN9k=
+-----END CERTIFICATE-----
```

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/auth_error.html` & `djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/auth_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/echo_attributes.html` & `djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/echo_attributes.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/logout_error.html` & `djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/logout_error.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/templates/djangosaml2/wayf.html` & `djangosaml2-1.5.8/djangosaml2/templates/djangosaml2/wayf.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.csr` & `djangosaml2-1.5.8/djangosaml2/tests/idpcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.key` & `djangosaml2-1.5.8/djangosaml2/tests/idpcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/idpcert.pem` & `djangosaml2-1.5.8/djangosaml2/tests/idpcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.csr` & `djangosaml2-1.5.8/djangosaml2/tests/mycert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.key` & `djangosaml2-1.5.8/djangosaml2/tests/mycert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/mycert.pem` & `djangosaml2-1.5.8/djangosaml2/tests/mycert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata.xml`

 * *Files 1% similar despite different names*

#### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata.xml` & `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata.xml`

```diff
@@ -23,15 +23,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp1.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -53,15 +53,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp1.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp1.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp2.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -83,15 +83,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp2.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp2.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp3.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -113,11 +113,11 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp3.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp3.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_one_idp.xml`

 * *Files 2% similar despite different names*

#### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_one_idp.xml` & `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_one_idp.xml`

```diff
@@ -23,11 +23,11 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_post_binding.xml`

 * *Files 3% similar despite different names*

#### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_post_binding.xml` & `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_post_binding.xml`

```diff
@@ -23,11 +23,11 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_three_idps.xml`

 * *Files 2% similar despite different names*

#### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/remote_metadata_three_idps.xml` & `djangosaml2-1.5.8/djangosaml2/tests/remote_metadata_three_idps.xml`

```diff
@@ -23,15 +23,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp1.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp1.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp2.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -53,15 +53,15 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp2.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp2.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
   <md:EntityDescriptor entityID="https://idp3.example.com/simplesaml/saml2/idp/metadata.php">
     <md:IDPSSODescriptor protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
       <md:KeyDescriptor use="signing">
         <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
           <ds:X509Data>
@@ -83,11 +83,11 @@
     <md:Organization>
       <md:OrganizationName xml:lang="en">Lorenzo's test IdP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">idp3.example.com IdP</md:OrganizationDisplayName>
       <md:OrganizationURL xml:lang="en">http://idp3.example.com/</md:OrganizationURL>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.5.8/djangosaml2/tests/sp_metadata.xml`

 * *Files 5% similar despite different names*

#### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/sp_metadata.xml` & `djangosaml2-1.5.8/djangosaml2/tests/sp_metadata.xml`

```diff
@@ -31,11 +31,11 @@
     <md:Organization>
       <md:OrganizationURL xml:lang="en">http://sp.example.com/</md:OrganizationURL>
       <md:OrganizationName xml:lang="en">Lorenzo's test SP</md:OrganizationName>
       <md:OrganizationDisplayName xml:lang="en">sp.example.com</md:OrganizationDisplayName>
     </md:Organization>
     <md:ContactPerson contactType="technical">
       <md:SurName>Administrator</md:SurName>
-      <md:EmailAddress>lgs@yaco.es</md:EmailAddress>
+      <md:EmailAddress>lorenzo.gil.sanchez@gmail.com</md:EmailAddress>
     </md:ContactPerson>
   </md:EntityDescriptor>
 </md:EntitiesDescriptor>
```

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.csr` & `djangosaml2-1.5.8/djangosaml2/tests/spcert.csr`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.key` & `djangosaml2-1.5.8/djangosaml2/tests/spcert.key`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/djangosaml2/tests/spcert.pem` & `djangosaml2-1.5.8/djangosaml2/tests/spcert.pem`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `djangosaml2-1.5.8/env/lib/python3.10/site-packages/certifi/cacert.pem`

 * *Files 4% similar despite different names*

```diff
@@ -24,44 +24,14 @@
 yj1hTdNGCbM+w6DjY1Ub8rrvrTnhQ7k4o+YviiY776BQVvnGCv04zcQLcFGUl5gE
 38NflNUVyRRBnMRddWQVDf9VMOyGj/8N7yy5Y0b2qvzfvGn9LhJIZJrglfCm7ymP
 AbEVtQwdpf5pLGkkeB6zpxxxYu7KyJesF12KwvhHhm4qxFYxldBniYUr+WymXUad
 DKqC5JlR3XC321Y9YeRq4VzW9v493kHMB65jUr9TU/Qr6cf9tveCX4XSQRjbgbME
 HMUfpIBvFSDJ3gyICh3WZlXi/EjJKSZp4A==
 -----END CERTIFICATE-----
 
-# Issuer: CN=GlobalSign O=GlobalSign OU=GlobalSign Root CA - R2
-# Subject: CN=GlobalSign O=GlobalSign OU=GlobalSign Root CA - R2
-# Label: "GlobalSign Root CA - R2"
-# Serial: 4835703278459682885658125
-# MD5 Fingerprint: 94:14:77:7e:3e:5e:fd:8f:30:bd:41:b0:cf:e7:d0:30
-# SHA1 Fingerprint: 75:e0:ab:b6:13:85:12:27:1c:04:f8:5f:dd:de:38:e4:b7:24:2e:fe
-# SHA256 Fingerprint: ca:42:dd:41:74:5f:d0:b8:1e:b9:02:36:2c:f9:d8:bf:71:9d:a1:bd:1b:1e:fc:94:6f:5b:4c:99:f4:2c:1b:9e
------BEGIN CERTIFICATE-----
-MIIDujCCAqKgAwIBAgILBAAAAAABD4Ym5g0wDQYJKoZIhvcNAQEFBQAwTDEgMB4G
-A1UECxMXR2xvYmFsU2lnbiBSb290IENBIC0gUjIxEzARBgNVBAoTCkdsb2JhbFNp
-Z24xEzARBgNVBAMTCkdsb2JhbFNpZ24wHhcNMDYxMjE1MDgwMDAwWhcNMjExMjE1
-MDgwMDAwWjBMMSAwHgYDVQQLExdHbG9iYWxTaWduIFJvb3QgQ0EgLSBSMjETMBEG
-A1UEChMKR2xvYmFsU2lnbjETMBEGA1UEAxMKR2xvYmFsU2lnbjCCASIwDQYJKoZI
-hvcNAQEBBQADggEPADCCAQoCggEBAKbPJA6+Lm8omUVCxKs+IVSbC9N/hHD6ErPL
-v4dfxn+G07IwXNb9rfF73OX4YJYJkhD10FPe+3t+c4isUoh7SqbKSaZeqKeMWhG8
-eoLrvozps6yWJQeXSpkqBy+0Hne/ig+1AnwblrjFuTosvNYSuetZfeLQBoZfXklq
-tTleiDTsvHgMCJiEbKjNS7SgfQx5TfC4LcshytVsW33hoCmEofnTlEnLJGKRILzd
-C9XZzPnqJworc5HGnRusyMvo4KD0L5CLTfuwNhv2GXqF4G3yYROIXJ/gkwpRl4pa
-zq+r1feqCapgvdzZX99yqWATXgAByUr6P6TqBwMhAo6CygPCm48CAwEAAaOBnDCB
-mTAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUm+IH
-V2ccHsBqBt5ZtJot39wZhi4wNgYDVR0fBC8wLTAroCmgJ4YlaHR0cDovL2NybC5n
-bG9iYWxzaWduLm5ldC9yb290LXIyLmNybDAfBgNVHSMEGDAWgBSb4gdXZxwewGoG
-3lm0mi3f3BmGLjANBgkqhkiG9w0BAQUFAAOCAQEAmYFThxxol4aR7OBKuEQLq4Gs
-J0/WwbgcQ3izDJr86iw8bmEbTUsp9Z8FHSbBuOmDAGJFtqkIk7mpM0sYmsL4h4hO
-291xNBrBVNpGP+DTKqttVCL1OmLNIG+6KYnX3ZHu01yiPqFbQfXf5WRDLenVOavS
-ot+3i9DAgBkcRcAtjOj4LaR0VknFBbVPFd5uRHg5h6h+u/N5GJG79G+dwfCMNYxd
-AfvDbbnvRG15RjF+Cv6pgsH/76tuIMRQyV+dTZsXjAzlAcmgQWpzU/qlULRuJQ/7
-TBj0/VLZjmmx6BEP3ojY+x1J96relc8geMJgEtslQIxq/H5COEBkEveegeGTLg==
------END CERTIFICATE-----
-
 # Issuer: CN=Entrust.net Certification Authority (2048) O=Entrust.net OU=www.entrust.net/CPS_2048 incorp. by ref. (limits liab.)/(c) 1999 Entrust.net Limited
 # Subject: CN=Entrust.net Certification Authority (2048) O=Entrust.net OU=www.entrust.net/CPS_2048 incorp. by ref. (limits liab.)/(c) 1999 Entrust.net Limited
 # Label: "Entrust.net Premium 2048 Secure Server CA"
 # Serial: 946069240
 # MD5 Fingerprint: ee:29:31:bc:32:7e:9a:e6:e8:b5:f7:51:b4:34:71:90
 # SHA1 Fingerprint: 50:30:06:09:1d:97:d4:f5:ae:39:f7:cb:e7:92:7d:7d:65:2d:34:31
 # SHA256 Fingerprint: 6d:c4:71:72:e0:1c:bc:b0:bf:62:58:0d:89:5f:e2:b8:ac:9a:d4:f8:73:80:1e:0c:10:b9:c8:37:d2:1e:b1:77
@@ -184,56 +154,14 @@
 GE8mTgHj5rCl7r+8dFRBv/38ErjHT1r0iWAFf2C3BUrz9vHCv8S5dIa2LX1rzNLz
 Rt0vxuBqw8M0Ayx9lt1awg6nCpnBBYurDC/zXDrPbDdVCYfeU0BsWO/8tqtlbgT2
 G9w84FoVxp7Z8VlIMCFlA2zs6SFz7JsDoeA3raAVGI/6ugLOpyypEBMs1OUIJqsi
 l2D4kF501KKaU73yqWjgom7C12yxow+ev+to51byrvLjKzg6CYG1a4XXvi3tPxq3
 smPi9WIsgtRqAEFQ8TmDn5XpNpaYbg==
 -----END CERTIFICATE-----
 
-# Issuer: CN=QuoVadis Root Certification Authority O=QuoVadis Limited OU=Root Certification Authority
-# Subject: CN=QuoVadis Root Certification Authority O=QuoVadis Limited OU=Root Certification Authority
-# Label: "QuoVadis Root CA"
-# Serial: 985026699
-# MD5 Fingerprint: 27:de:36:fe:72:b7:00:03:00:9d:f4:f0:1e:6c:04:24
-# SHA1 Fingerprint: de:3f:40:bd:50:93:d3:9b:6c:60:f6:da:bc:07:62:01:00:89:76:c9
-# SHA256 Fingerprint: a4:5e:de:3b:bb:f0:9c:8a:e1:5c:72:ef:c0:72:68:d6:93:a2:1c:99:6f:d5:1e:67:ca:07:94:60:fd:6d:88:73
------BEGIN CERTIFICATE-----
-MIIF0DCCBLigAwIBAgIEOrZQizANBgkqhkiG9w0BAQUFADB/MQswCQYDVQQGEwJC
-TTEZMBcGA1UEChMQUXVvVmFkaXMgTGltaXRlZDElMCMGA1UECxMcUm9vdCBDZXJ0
-aWZpY2F0aW9uIEF1dGhvcml0eTEuMCwGA1UEAxMlUXVvVmFkaXMgUm9vdCBDZXJ0
-aWZpY2F0aW9uIEF1dGhvcml0eTAeFw0wMTAzMTkxODMzMzNaFw0yMTAzMTcxODMz
-MzNaMH8xCzAJBgNVBAYTAkJNMRkwFwYDVQQKExBRdW9WYWRpcyBMaW1pdGVkMSUw
-IwYDVQQLExxSb290IENlcnRpZmljYXRpb24gQXV0aG9yaXR5MS4wLAYDVQQDEyVR
-dW9WYWRpcyBSb290IENlcnRpZmljYXRpb24gQXV0aG9yaXR5MIIBIjANBgkqhkiG
-9w0BAQEFAAOCAQ8AMIIBCgKCAQEAv2G1lVO6V/z68mcLOhrfEYBklbTRvM16z/Yp
-li4kVEAkOPcahdxYTMukJ0KX0J+DisPkBgNbAKVRHnAEdOLB1Dqr1607BxgFjv2D
-rOpm2RgbaIr1VxqYuvXtdj182d6UajtLF8HVj71lODqV0D1VNk7feVcxKh7YWWVJ
-WCCYfqtffp/p1k3sg3Spx2zY7ilKhSoGFPlU5tPaZQeLYzcS19Dsw3sgQUSj7cug
-F+FxZc4dZjH3dgEZyH0DWLaVSR2mEiboxgx24ONmy+pdpibu5cxfvWenAScOospU
-xbF6lR1xHkopigPcakXBpBlebzbNw6Kwt/5cOOJSvPhEQ+aQuwIDAQABo4ICUjCC
-Ak4wPQYIKwYBBQUHAQEEMTAvMC0GCCsGAQUFBzABhiFodHRwczovL29jc3AucXVv
-dmFkaXNvZmZzaG9yZS5jb20wDwYDVR0TAQH/BAUwAwEB/zCCARoGA1UdIASCAREw
-ggENMIIBCQYJKwYBBAG+WAABMIH7MIHUBggrBgEFBQcCAjCBxxqBxFJlbGlhbmNl
-IG9uIHRoZSBRdW9WYWRpcyBSb290IENlcnRpZmljYXRlIGJ5IGFueSBwYXJ0eSBh
-c3N1bWVzIGFjY2VwdGFuY2Ugb2YgdGhlIHRoZW4gYXBwbGljYWJsZSBzdGFuZGFy
-ZCB0ZXJtcyBhbmQgY29uZGl0aW9ucyBvZiB1c2UsIGNlcnRpZmljYXRpb24gcHJh
-Y3RpY2VzLCBhbmQgdGhlIFF1b1ZhZGlzIENlcnRpZmljYXRlIFBvbGljeS4wIgYI
-KwYBBQUHAgEWFmh0dHA6Ly93d3cucXVvdmFkaXMuYm0wHQYDVR0OBBYEFItLbe3T
-KbkGGew5Oanwl4Rqy+/fMIGuBgNVHSMEgaYwgaOAFItLbe3TKbkGGew5Oanwl4Rq
-y+/foYGEpIGBMH8xCzAJBgNVBAYTAkJNMRkwFwYDVQQKExBRdW9WYWRpcyBMaW1p
-dGVkMSUwIwYDVQQLExxSb290IENlcnRpZmljYXRpb24gQXV0aG9yaXR5MS4wLAYD
-VQQDEyVRdW9WYWRpcyBSb290IENlcnRpZmljYXRpb24gQXV0aG9yaXR5ggQ6tlCL
-MA4GA1UdDwEB/wQEAwIBBjANBgkqhkiG9w0BAQUFAAOCAQEAitQUtf70mpKnGdSk
-fnIYj9lofFIk3WdvOXrEql494liwTXCYhGHoG+NpGA7O+0dQoE7/8CQfvbLO9Sf8
-7C9TqnN7Az10buYWnuulLsS/VidQK2K6vkscPFVcQR0kvoIgR13VRH56FmjffU1R
-cHhXHTMe/QKZnAzNCgVPx7uOpHX6Sm2xgI4JVrmcGmD+XcHXetwReNDWXcG31a0y
-mQM6isxUJTkxgXsTIlG6Rmyhu576BGxJJnSP0nPrzDCi5upZIof4l/UO/erMkqQW
-xFIY6iHOsfHmhIHluqmGKPJDWl0Snawe2ajlCmqnf6CHKc/yiU3U7MXi5nrQNiOK
-SnQ2+Q==
------END CERTIFICATE-----
-
 # Issuer: CN=QuoVadis Root CA 2 O=QuoVadis Limited
 # Subject: CN=QuoVadis Root CA 2 O=QuoVadis Limited
 # Label: "QuoVadis Root CA 2"
 # Serial: 1289
 # MD5 Fingerprint: 5e:39:7b:dd:f8:ba:ec:82:e9:ac:62:ba:0c:54:00:2b
 # SHA1 Fingerprint: ca:3a:fb:cf:12:40:36:4b:44:b2:16:20:88:80:48:39:19:93:7c:f7
 # SHA256 Fingerprint: 85:a0:dd:7d:d7:20:ad:b7:ff:05:f8:3d:54:2b:20:9d:c7:ff:45:28:f7:d6:77:b1:83:89:fe:a5:e5:c4:9e:86
@@ -341,41 +269,14 @@
 kl3g0dNq/vu+m22/xwVtWSDEHPC32oRYAmP6SBbvT6UL90qY8j+eG61Ha2POCEfr
 Uj94nK9NrvjVT8+amCoQQTlSxN3Zmw7vkwGusi7KaEIkQmywszo+zenaSMQVy+n5
 Bw+SUEmK3TGXX8npN6o7WWWXlDLJs58+OmJYxUmtYg5xpTKqL8aJdkNAExNnPaJU
 JRDL8Try2frbSVa7pv6nQTXD4IhhyYjH3zYQIphZ6rBK+1YWc26sTfcioU+tHXot
 RSflMMFe8toTyyVCUZVHA4xsIcx0Qu1T/zOLjw9XARYvz6buyXAiFL39vmwLAw==
 -----END CERTIFICATE-----
 
-# Issuer: CN=Sonera Class2 CA O=Sonera
-# Subject: CN=Sonera Class2 CA O=Sonera
-# Label: "Sonera Class 2 Root CA"
-# Serial: 29
-# MD5 Fingerprint: a3:ec:75:0f:2e:88:df:fa:48:01:4e:0b:5c:48:6f:fb
-# SHA1 Fingerprint: 37:f7:6d:e6:07:7c:90:c5:b1:3e:93:1a:b7:41:10:b4:f2:e4:9a:27
-# SHA256 Fingerprint: 79:08:b4:03:14:c1:38:10:0b:51:8d:07:35:80:7f:fb:fc:f8:51:8a:00:95:33:71:05:ba:38:6b:15:3d:d9:27
------BEGIN CERTIFICATE-----
-MIIDIDCCAgigAwIBAgIBHTANBgkqhkiG9w0BAQUFADA5MQswCQYDVQQGEwJGSTEP
-MA0GA1UEChMGU29uZXJhMRkwFwYDVQQDExBTb25lcmEgQ2xhc3MyIENBMB4XDTAx
-MDQwNjA3Mjk0MFoXDTIxMDQwNjA3Mjk0MFowOTELMAkGA1UEBhMCRkkxDzANBgNV
-BAoTBlNvbmVyYTEZMBcGA1UEAxMQU29uZXJhIENsYXNzMiBDQTCCASIwDQYJKoZI
-hvcNAQEBBQADggEPADCCAQoCggEBAJAXSjWdyvANlsdE+hY3/Ei9vX+ALTU74W+o
-Z6m/AxxNjG8yR9VBaKQTBME1DJqEQ/xcHf+Js+gXGM2RX/uJ4+q/Tl18GybTdXnt
-5oTjV+WtKcT0OijnpXuENmmz/V52vaMtmdOQTiMofRhj8VQ7Jp12W5dCsv+u8E7s
-3TmVToMGf+dJQMjFAbJUWmYdPfz56TwKnoG4cPABi+QjVHzIrviQHgCWctRUz2Ej
-vOr7nQKV0ba5cTppCD8PtOFCx4j1P5iop7oc4HFx71hXgVB6XGt0Rg6DA5jDjqhu
-8nYybieDwnPz3BjotJPqdURrBGAgcVeHnfO+oJAjPYok4doh28MCAwEAAaMzMDEw
-DwYDVR0TAQH/BAUwAwEB/zARBgNVHQ4ECgQISqCqWITTXjwwCwYDVR0PBAQDAgEG
-MA0GCSqGSIb3DQEBBQUAA4IBAQBazof5FnIVV0sd2ZvnoiYw7JNn39Yt0jSv9zil
-zqsWuasvfDXLrNAPtEwr/IDva4yRXzZ299uzGxnq9LIR/WFxRL8oszodv7ND6J+/
-3DEIcbCdjdY0RzKQxmUk96BKfARzjzlvF4xytb1LyHr4e4PDKE6cCepnP7JnBBvD
-FNr450kkkdAdavphOe9r5yF1BgfYErQhIHBCcYHaPJo2vqZbDWpsmh+Re/n570K6
-Tk6ezAyNlNzZRZxe7EJQY670XcSxEtzKO6gunRRaBXW37Ndj4ro1tgQIkejanZz2
-ZrUYrAqmVCY0M9IbwdR/GjqOC6oybtv8TyWf2TLHllpwrN9M
------END CERTIFICATE-----
-
 # Issuer: CN=XRamp Global Certification Authority O=XRamp Security Services Inc OU=www.xrampsecurity.com
 # Subject: CN=XRamp Global Certification Authority O=XRamp Security Services Inc OU=www.xrampsecurity.com
 # Label: "XRamp Global CA Root"
 # Serial: 107108908803651509692980124233745014957
 # MD5 Fingerprint: a1:0b:44:b3:ca:10:d8:00:6e:9d:0f:d8:0f:92:0a:d1
 # SHA1 Fingerprint: b8:01:86:d1:eb:9c:86:a5:41:04:cf:30:54:f3:4c:52:b7:e5:58:c6
 # SHA256 Fingerprint: ce:cd:dc:90:50:99:d8:da:df:c5:b1:d2:09:b7:37:cb:e2:c1:8c:fb:2c:10:c0:ff:0b:cf:0d:32:86:fc:1a:a2
@@ -556,42 +457,14 @@
 eM7b41N5cdblIZQB2lWHmiRk9opmzN6cN82oNLFpmyPInngiK3BD41VHMWEZ71jF
 hS9OMPagMRYjyOfiZRYzy78aG6A9+MpeizGLYAiJLQwGXFK3xPkKmNEVX58Svnw2
 Yzi9RKR/5CYrCsSXaQ3pjOLAEFe4yHYSkVXySGnYvCoCWw9E1CAx2/S6cCZdkGCe
 vEsXCS+0yx5DaMkHJ8HSXPfqIbloEpw8nL+e/IBcm2PN7EeqJSdnoDfzAIJ9VNep
 +OkuE6N36B9K
 -----END CERTIFICATE-----
 
-# Issuer: CN=DST Root CA X3 O=Digital Signature Trust Co.
-# Subject: CN=DST Root CA X3 O=Digital Signature Trust Co.
-# Label: "DST Root CA X3"
-# Serial: 91299735575339953335919266965803778155
-# MD5 Fingerprint: 41:03:52:dc:0f:f7:50:1b:16:f0:02:8e:ba:6f:45:c5
-# SHA1 Fingerprint: da:c9:02:4f:54:d8:f6:df:94:93:5f:b1:73:26:38:ca:6a:d7:7c:13
-# SHA256 Fingerprint: 06:87:26:03:31:a7:24:03:d9:09:f1:05:e6:9b:cf:0d:32:e1:bd:24:93:ff:c6:d9:20:6d:11:bc:d6:77:07:39
------BEGIN CERTIFICATE-----
-MIIDSjCCAjKgAwIBAgIQRK+wgNajJ7qJMDmGLvhAazANBgkqhkiG9w0BAQUFADA/
-MSQwIgYDVQQKExtEaWdpdGFsIFNpZ25hdHVyZSBUcnVzdCBDby4xFzAVBgNVBAMT
-DkRTVCBSb290IENBIFgzMB4XDTAwMDkzMDIxMTIxOVoXDTIxMDkzMDE0MDExNVow
-PzEkMCIGA1UEChMbRGlnaXRhbCBTaWduYXR1cmUgVHJ1c3QgQ28uMRcwFQYDVQQD
-Ew5EU1QgUm9vdCBDQSBYMzCCASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEB
-AN+v6ZdQCINXtMxiZfaQguzH0yxrMMpb7NnDfcdAwRgUi+DoM3ZJKuM/IUmTrE4O
-rz5Iy2Xu/NMhD2XSKtkyj4zl93ewEnu1lcCJo6m67XMuegwGMoOifooUMM0RoOEq
-OLl5CjH9UL2AZd+3UWODyOKIYepLYYHsUmu5ouJLGiifSKOeDNoJjj4XLh7dIN9b
-xiqKqy69cK3FCxolkHRyxXtqqzTWMIn/5WgTe1QLyNau7Fqckh49ZLOMxt+/yUFw
-7BZy1SbsOFU5Q9D8/RhcQPGX69Wam40dutolucbY38EVAjqr2m7xPi71XAicPNaD
-aeQQmxkqtilX4+U9m5/wAl0CAwEAAaNCMEAwDwYDVR0TAQH/BAUwAwEB/zAOBgNV
-HQ8BAf8EBAMCAQYwHQYDVR0OBBYEFMSnsaR7LHH62+FLkHX/xBVghYkQMA0GCSqG
-SIb3DQEBBQUAA4IBAQCjGiybFwBcqR7uKGY3Or+Dxz9LwwmglSBd49lZRNI+DT69
-ikugdB/OEIKcdBodfpga3csTS7MgROSR6cz8faXbauX+5v3gTt23ADq1cEmv8uXr
-AvHRAosZy5Q6XkjEGB5YGV8eAlrwDPGxrancWYaLbumR9YbK+rlmM6pZW87ipxZz
-R8srzJmwN0jP41ZL9c8PDHIyh8bwRLtTcm1D9SZImlJnt1ir/md2cXjbDaJWFBM5
-JDGFoqgCWjBH4d1QB7wCCZAA62RjYJsWvIjJEubSfZGL+T0yjWW06XyxV3bqxbYo
-Ob8VZRzI9neWagqNdwvYkQsEjgfbKbYK7p2CNTUQ
------END CERTIFICATE-----
-
 # Issuer: CN=SwissSign Gold CA - G2 O=SwissSign AG
 # Subject: CN=SwissSign Gold CA - G2 O=SwissSign AG
 # Label: "SwissSign Gold CA - G2"
 # Serial: 13492815561806991280
 # MD5 Fingerprint: 24:77:d9:a8:91:d1:3b:fa:88:2d:c2:ff:f8:cd:33:93
 # SHA1 Fingerprint: d8:c5:38:8a:b7:30:1b:1b:6e:d4:7a:e6:45:25:3a:6f:9f:1a:27:61
 # SHA256 Fingerprint: 62:dd:0b:e9:b9:f5:0a:16:3e:a0:f8:e7:5c:05:3b:1e:ca:57:ea:55:c8:68:8f:64:7c:68:81:f2:c8:35:7b:95
@@ -759,45 +632,14 @@
 IC9Bi5HcSEW88cbeunZrM8gALTFGTO3nnc+IlP8zwFboJIYmuNg4ON8qa90SzMc/
 RxdMosIGlgnW2/4/PEZB31jiVg88O8EckzXZOFKs7sjsLjBOlDW0JB9LeGna8gI4
 zJVSk/BwJVmcIGfE7vmLV2H0knZ9P4SNVbfo5azV8fUZVqZa+5Acr5Pr5RzUZ5dd
 BA6+C4OmF4O5MBKgxTMVBbkN+8cFduPYSo38NBejxiEovjBFMR7HeL5YYTisO+IB
 ZQ==
 -----END CERTIFICATE-----
 
-# Issuer: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Subject: CN=Network Solutions Certificate Authority O=Network Solutions L.L.C.
-# Label: "Network Solutions Certificate Authority"
-# Serial: 116697915152937497490437556386812487904
-# MD5 Fingerprint: d3:f3:a6:16:c0:fa:6b:1d:59:b1:2d:96:4d:0e:11:2e
-# SHA1 Fingerprint: 74:f8:a3:c3:ef:e7:b3:90:06:4b:83:90:3c:21:64:60:20:e5:df:ce
-# SHA256 Fingerprint: 15:f0:ba:00:a3:ac:7a:f3:ac:88:4c:07:2b:10:11:a0:77:bd:77:c0:97:f4:01:64:b2:f8:59:8a:bd:83:86:0c
------BEGIN CERTIFICATE-----
-MIID5jCCAs6gAwIBAgIQV8szb8JcFuZHFhfjkDFo4DANBgkqhkiG9w0BAQUFADBi
-MQswCQYDVQQGEwJVUzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMu
-MTAwLgYDVQQDEydOZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3Jp
-dHkwHhcNMDYxMjAxMDAwMDAwWhcNMjkxMjMxMjM1OTU5WjBiMQswCQYDVQQGEwJV
-UzEhMB8GA1UEChMYTmV0d29yayBTb2x1dGlvbnMgTC5MLkMuMTAwLgYDVQQDEydO
-ZXR3b3JrIFNvbHV0aW9ucyBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkwggEiMA0GCSqG
-SIb3DQEBAQUAA4IBDwAwggEKAoIBAQDkvH6SMG3G2I4rC7xGzuAnlt7e+foS0zwz
-c7MEL7xxjOWftiJgPl9dzgn/ggwbmlFQGiaJ3dVhXRncEg8tCqJDXRfQNJIg6nPP
-OCwGJgl6cvf6UDL4wpPTaaIjzkGxzOTVHzbRijr4jGPiFFlp7Q3Tf2vouAPlT2rl
-mGNpSAW+Lv8ztumXWWn4Zxmuk2GWRBXTcrA/vGp97Eh/jcOrqnErU2lBUzS1sLnF
-BgrEsEX1QV1uiUV7PTsmjHTC5dLRfbIR1PtYMiKagMnc/Qzpf14Dl847ABSHJ3A4
-qY5usyd2mFHgBeMhqxrVhSI8KbWaFsWAqPS7azCPL0YCorEMIuDTAgMBAAGjgZcw
-gZQwHQYDVR0OBBYEFCEwyfsA106Y2oeqKtCnLrFAMadMMA4GA1UdDwEB/wQEAwIB
-BjAPBgNVHRMBAf8EBTADAQH/MFIGA1UdHwRLMEkwR6BFoEOGQWh0dHA6Ly9jcmwu
-bmV0c29sc3NsLmNvbS9OZXR3b3JrU29sdXRpb25zQ2VydGlmaWNhdGVBdXRob3Jp
-dHkuY3JsMA0GCSqGSIb3DQEBBQUAA4IBAQC7rkvnt1frf6ott3NHhWrB5KUd5Oc8
-6fRZZXe1eltajSU24HqXLjjAV2CDmAaDn7l2em5Q4LqILPxFzBiwmZVRDuwduIj/
-h1AcgsLj4DKAv6ALR8jDMe+ZZzKATxcheQxpXN5eNK4CtSbqUN9/GGUsyfJj4akH
-/nxxH2szJGoeBfcFaMBqEssuXmHLrijTfsK0ZpEmXzwuJF/LWA/rKOyvEZbz3Htv
-wKeI8lN3s2Berq4o2jUsbzRF0ybh3uxbTydrFny9RAQYgrOJeRcQcT16ohZO9QHN
-pGxlaKFJdlxDydi8NmdspZS11My5vWo1ViHe2MPr+8ukYEywVaCge1ey
------END CERTIFICATE-----
-
 # Issuer: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Subject: CN=COMODO ECC Certification Authority O=COMODO CA Limited
 # Label: "COMODO ECC Certification Authority"
 # Serial: 41578283867086692638256921589707938090
 # MD5 Fingerprint: 7c:62:ff:74:9d:31:53:5e:68:4a:d5:78:aa:1e:bf:23
 # SHA1 Fingerprint: 9f:74:4e:9f:2b:4d:ba:ec:0f:31:2c:50:b6:56:3b:8e:2d:93:c3:11
 # SHA256 Fingerprint: 17:93:92:7a:06:14:54:97:89:ad:ce:2f:8f:34:f7:f0:b6:6d:0f:3a:e3:a3:b8:4d:21:ec:15:db:ba:4f:ad:c7
@@ -844,44 +686,14 @@
 bV6lUmPOEvjvKtpv6zf+EwLHyzs+ImvaYS5/1HI93TDhHkxAGYwP15zRgzB7mFnc
 fca5DClMoTOi62c6ZYTTluLtdkVwj7Ur3vkj1kluPBS1xp81HlDQwY9qcEQCYsuu
 HWhBp6pX6FOqB9IG9tUUBguRA3UsbHK1YZWaDYu5Def131TN3ubY1gkIl2PlwS6w
 t0QmwCbAr1UwnjvVNioZBPRcHv/PLLf/0P2HQBHVESO7SMAhqaQoLf0V+LBOK/Qw
 WyH8EZE0vkHve52Xdf+XlcCWWC/qu0bXu+TZLg==
 -----END CERTIFICATE-----
 
-# Issuer: CN=Cybertrust Global Root O=Cybertrust, Inc
-# Subject: CN=Cybertrust Global Root O=Cybertrust, Inc
-# Label: "Cybertrust Global Root"
-# Serial: 4835703278459682877484360
-# MD5 Fingerprint: 72:e4:4a:87:e3:69:40:80:77:ea:bc:e3:f4:ff:f0:e1
-# SHA1 Fingerprint: 5f:43:e5:b1:bf:f8:78:8c:ac:1c:c7:ca:4a:9a:c6:22:2b:cc:34:c6
-# SHA256 Fingerprint: 96:0a:df:00:63:e9:63:56:75:0c:29:65:dd:0a:08:67:da:0b:9c:bd:6e:77:71:4a:ea:fb:23:49:ab:39:3d:a3
------BEGIN CERTIFICATE-----
-MIIDoTCCAomgAwIBAgILBAAAAAABD4WqLUgwDQYJKoZIhvcNAQEFBQAwOzEYMBYG
-A1UEChMPQ3liZXJ0cnVzdCwgSW5jMR8wHQYDVQQDExZDeWJlcnRydXN0IEdsb2Jh
-bCBSb290MB4XDTA2MTIxNTA4MDAwMFoXDTIxMTIxNTA4MDAwMFowOzEYMBYGA1UE
-ChMPQ3liZXJ0cnVzdCwgSW5jMR8wHQYDVQQDExZDeWJlcnRydXN0IEdsb2JhbCBS
-b290MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA+Mi8vRRQZhP/8NN5
-7CPytxrHjoXxEnOmGaoQ25yiZXRadz5RfVb23CO21O1fWLE3TdVJDm71aofW0ozS
-J8bi/zafmGWgE07GKmSb1ZASzxQG9Dvj1Ci+6A74q05IlG2OlTEQXO2iLb3VOm2y
-HLtgwEZLAfVJrn5GitB0jaEMAs7u/OePuGtm839EAL9mJRQr3RAwHQeWP032a7iP
-t3sMpTjr3kfb1V05/Iin89cqdPHoWqI7n1C6poxFNcJQZZXcY4Lv3b93TZxiyWNz
-FtApD0mpSPCzqrdsxacwOUBdrsTiXSZT8M4cIwhhqJQZugRiQOwfOHB3EgZxpzAY
-XSUnpQIDAQABo4GlMIGiMA4GA1UdDwEB/wQEAwIBBjAPBgNVHRMBAf8EBTADAQH/
-MB0GA1UdDgQWBBS2CHsNesysIEyGVjJez6tuhS1wVzA/BgNVHR8EODA2MDSgMqAw
-hi5odHRwOi8vd3d3Mi5wdWJsaWMtdHJ1c3QuY29tL2NybC9jdC9jdHJvb3QuY3Js
-MB8GA1UdIwQYMBaAFLYIew16zKwgTIZWMl7Pq26FLXBXMA0GCSqGSIb3DQEBBQUA
-A4IBAQBW7wojoFROlZfJ+InaRcHUowAl9B8Tq7ejhVhpwjCt2BWKLePJzYFa+HMj
-Wqd8BfP9IjsO0QbE2zZMcwSO5bAi5MXzLqXZI+O4Tkogp24CJJ8iYGd7ix1yCcUx
-XOl5n4BHPa2hCwcUPUf/A2kaDAtE52Mlp3+yybh2hO0j9n0Hq0V+09+zv+mKts2o
-omcrUtW3ZfA5TGOgkXmTUg9U3YO7n9GPp1Nzw8v/MOx8BLjYRB+TX3EJIrduPuoc
-A06dGiBh+4E37F78CkWr1+cXVdCg6mCbpvbjjFspwgZgFJ0tl0ypkxWdYcQBX0jW
-WL1WMRJOEcgh4LMRkWXbtKaIOM5V
------END CERTIFICATE-----
-
 # Issuer: O=Chunghwa Telecom Co., Ltd. OU=ePKI Root Certification Authority
 # Subject: O=Chunghwa Telecom Co., Ltd. OU=ePKI Root Certification Authority
 # Label: "ePKI Root Certification Authority"
 # Serial: 28956088682735189655030529057352760477
 # MD5 Fingerprint: 1b:2e:00:ca:26:06:90:3d:ad:fe:6f:15:68:d3:6b:b3
 # SHA1 Fingerprint: 67:65:0d:f1:7e:8e:7e:5b:82:40:a4:f4:56:4b:cf:e2:3d:69:c6:f0
 # SHA256 Fingerprint: c0:a6:f4:dc:63:a2:4b:fd:cf:54:ef:2a:6a:08:2a:0a:72:de:35:80:3e:2f:f5:ff:52:7a:e5:d8:72:06:df:d5
@@ -943,75 +755,14 @@
 MnQ8SG4Pn0vU9x7Tk4ZkVJdjclDVVc/6IJMCopvDI5NOFlV2oHB5bc0hH88vLbwZ
 44gx+FkagQnIl6Z0x2DEW8xXjrJ1/RsCCdtZb3KTafcxQdaIOL+Hsr0Wefmq5L6I
 Jd1hJyMctTEHBDa0GpC9oHRxUIltvBTjD4au8as+x6AJzKNI0eDbZOeStc+vckNw
 i/nDhDwTqn6Sm1dTk/pwwpEOMfmbZ13pljheX7NzTogVZ96edhBiIL5VaZVDADlN
 9u6wWk5JRFRYX0KD
 -----END CERTIFICATE-----
 
-# Issuer: CN=GeoTrust Primary Certification Authority - G2 O=GeoTrust Inc. OU=(c) 2007 GeoTrust Inc. - For authorized use only
-# Subject: CN=GeoTrust Primary Certification Authority - G2 O=GeoTrust Inc. OU=(c) 2007 GeoTrust Inc. - For authorized use only
-# Label: "GeoTrust Primary Certification Authority - G2"
-# Serial: 80682863203381065782177908751794619243
-# MD5 Fingerprint: 01:5e:d8:6b:bd:6f:3d:8e:a1:31:f8:12:e0:98:73:6a
-# SHA1 Fingerprint: 8d:17:84:d5:37:f3:03:7d:ec:70:fe:57:8b:51:9a:99:e6:10:d7:b0
-# SHA256 Fingerprint: 5e:db:7a:c4:3b:82:a0:6a:87:61:e8:d7:be:49:79:eb:f2:61:1f:7d:d7:9b:f9:1c:1c:6b:56:6a:21:9e:d7:66
------BEGIN CERTIFICATE-----
-MIICrjCCAjWgAwIBAgIQPLL0SAoA4v7rJDteYD7DazAKBggqhkjOPQQDAzCBmDEL
-MAkGA1UEBhMCVVMxFjAUBgNVBAoTDUdlb1RydXN0IEluYy4xOTA3BgNVBAsTMChj
-KSAyMDA3IEdlb1RydXN0IEluYy4gLSBGb3IgYXV0aG9yaXplZCB1c2Ugb25seTE2
-MDQGA1UEAxMtR2VvVHJ1c3QgUHJpbWFyeSBDZXJ0aWZpY2F0aW9uIEF1dGhvcml0
-eSAtIEcyMB4XDTA3MTEwNTAwMDAwMFoXDTM4MDExODIzNTk1OVowgZgxCzAJBgNV
-BAYTAlVTMRYwFAYDVQQKEw1HZW9UcnVzdCBJbmMuMTkwNwYDVQQLEzAoYykgMjAw
-NyBHZW9UcnVzdCBJbmMuIC0gRm9yIGF1dGhvcml6ZWQgdXNlIG9ubHkxNjA0BgNV
-BAMTLUdlb1RydXN0IFByaW1hcnkgQ2VydGlmaWNhdGlvbiBBdXRob3JpdHkgLSBH
-MjB2MBAGByqGSM49AgEGBSuBBAAiA2IABBWx6P0DFUPlrOuHNxFi79KDNlJ9RVcL
-So17VDs6bl8VAsBQps8lL33KSLjHUGMcKiEIfJo22Av+0SbFWDEwKCXzXV2juLal
-tJLtbCyf691DiaI8S0iRHVDsJt/WYC69IaNCMEAwDwYDVR0TAQH/BAUwAwEB/zAO
-BgNVHQ8BAf8EBAMCAQYwHQYDVR0OBBYEFBVfNVdRVfslsq0DafwBo/q+EVXVMAoG
-CCqGSM49BAMDA2cAMGQCMGSWWaboCd6LuvpaiIjwH5HTRqjySkwCY/tsXzjbLkGT
-qQ7mndwxHLKgpxgceeHHNgIwOlavmnRs9vuD4DPTCF+hnMJbn0bWtsuRBmOiBucz
-rD6ogRLQy7rQkgu2npaqBA+K
------END CERTIFICATE-----
-
-# Issuer: CN=VeriSign Universal Root Certification Authority O=VeriSign, Inc. OU=VeriSign Trust Network/(c) 2008 VeriSign, Inc. - For authorized use only
-# Subject: CN=VeriSign Universal Root Certification Authority O=VeriSign, Inc. OU=VeriSign Trust Network/(c) 2008 VeriSign, Inc. - For authorized use only
-# Label: "VeriSign Universal Root Certification Authority"
-# Serial: 85209574734084581917763752644031726877
-# MD5 Fingerprint: 8e:ad:b5:01:aa:4d:81:e4:8c:1d:d1:e1:14:00:95:19
-# SHA1 Fingerprint: 36:79:ca:35:66:87:72:30:4d:30:a5:fb:87:3b:0f:a7:7b:b7:0d:54
-# SHA256 Fingerprint: 23:99:56:11:27:a5:71:25:de:8c:ef:ea:61:0d:df:2f:a0:78:b5:c8:06:7f:4e:82:82:90:bf:b8:60:e8:4b:3c
------BEGIN CERTIFICATE-----
-MIIEuTCCA6GgAwIBAgIQQBrEZCGzEyEDDrvkEhrFHTANBgkqhkiG9w0BAQsFADCB
-vTELMAkGA1UEBhMCVVMxFzAVBgNVBAoTDlZlcmlTaWduLCBJbmMuMR8wHQYDVQQL
-ExZWZXJpU2lnbiBUcnVzdCBOZXR3b3JrMTowOAYDVQQLEzEoYykgMjAwOCBWZXJp
-U2lnbiwgSW5jLiAtIEZvciBhdXRob3JpemVkIHVzZSBvbmx5MTgwNgYDVQQDEy9W
-ZXJpU2lnbiBVbml2ZXJzYWwgUm9vdCBDZXJ0aWZpY2F0aW9uIEF1dGhvcml0eTAe
-Fw0wODA0MDIwMDAwMDBaFw0zNzEyMDEyMzU5NTlaMIG9MQswCQYDVQQGEwJVUzEX
-MBUGA1UEChMOVmVyaVNpZ24sIEluYy4xHzAdBgNVBAsTFlZlcmlTaWduIFRydXN0
-IE5ldHdvcmsxOjA4BgNVBAsTMShjKSAyMDA4IFZlcmlTaWduLCBJbmMuIC0gRm9y
-IGF1dGhvcml6ZWQgdXNlIG9ubHkxODA2BgNVBAMTL1ZlcmlTaWduIFVuaXZlcnNh
-bCBSb290IENlcnRpZmljYXRpb24gQXV0aG9yaXR5MIIBIjANBgkqhkiG9w0BAQEF
-AAOCAQ8AMIIBCgKCAQEAx2E3XrEBNNti1xWb/1hajCMj1mCOkdeQmIN65lgZOIzF
-9uVkhbSicfvtvbnazU0AtMgtc6XHaXGVHzk8skQHnOgO+k1KxCHfKWGPMiJhgsWH
-H26MfF8WIFFE0XBPV+rjHOPMee5Y2A7Cs0WTwCznmhcrewA3ekEzeOEz4vMQGn+H
-LL729fdC4uW/h2KJXwBL38Xd5HVEMkE6HnFuacsLdUYI0crSK5XQz/u5QGtkjFdN
-/BMReYTtXlT2NJ8IAfMQJQYXStrxHXpma5hgZqTZ79IugvHw7wnqRMkVauIDbjPT
-rJ9VAMf2CGqUuV/c4DPxhGD5WycRtPwW8rtWaoAljQIDAQABo4GyMIGvMA8GA1Ud
-EwEB/wQFMAMBAf8wDgYDVR0PAQH/BAQDAgEGMG0GCCsGAQUFBwEMBGEwX6FdoFsw
-WTBXMFUWCWltYWdlL2dpZjAhMB8wBwYFKw4DAhoEFI/l0xqGrI2Oa8PPgGrUSBgs
-exkuMCUWI2h0dHA6Ly9sb2dvLnZlcmlzaWduLmNvbS92c2xvZ28uZ2lmMB0GA1Ud
-DgQWBBS2d/ppSEefUxLVwuoHMnYH0ZcHGTANBgkqhkiG9w0BAQsFAAOCAQEASvj4
-sAPmLGd75JR3Y8xuTPl9Dg3cyLk1uXBPY/ok+myDjEedO2Pzmvl2MpWRsXe8rJq+
-seQxIcaBlVZaDrHC1LGmWazxY8u4TB1ZkErvkBYoH1quEPuBUDgMbMzxPcP1Y+Oz
-4yHJJDnp/RVmRvQbEdBNc6N9Rvk97ahfYtTxP/jgdFcrGJ2BtMQo2pSXpXDrrB2+
-BxHw1dvd5Yzw1TKwg+ZX4o+/vqGqvz0dtdQ46tewXDpPaj+PwGZsY6rp2aQW9IHR
-lRQOfc2VNNnSj3BzgXucfr2YYdhFh5iQxeuGMMY1v/D/w1WIg0vvBZIGcfK4mJO3
-7M2CYfE45k+XmCpajQ==
------END CERTIFICATE-----
-
 # Issuer: CN=NetLock Arany (Class Gold) F\u0151tan\xfas\xedtv\xe1ny O=NetLock Kft. OU=Tan\xfas\xedtv\xe1nykiad\xf3k (Certification Services)
 # Subject: CN=NetLock Arany (Class Gold) F\u0151tan\xfas\xedtv\xe1ny O=NetLock Kft. OU=Tan\xfas\xedtv\xe1nykiad\xf3k (Certification Services)
 # Label: "NetLock Arany (Class Gold) F\u0151tan\xfas\xedtv\xe1ny"
 # Serial: 80544274841616
 # MD5 Fingerprint: c5:a1:b7:ff:73:dd:d6:d7:34:32:18:df:fc:3c:ad:88
 # SHA1 Fingerprint: 06:08:3f:59:3f:15:a1:04:a0:69:a4:6b:a9:03:d0:06:b7:97:09:91
 # SHA256 Fingerprint: 6c:61:da:c3:a2:de:f0:31:50:6b:e0:36:d2:a6:fe:40:19:94:fb:d1:3d:f9:c8:d4:66:59:92:74:c4:46:ec:98
@@ -1239,113 +990,14 @@
 LhObNA5me0mrZJfQRsN5nXJQY6aYWwa9SG3YOYNw6DXwBdGqvOPbyALqfP2C2sJb
 UjWumDqtujWTI6cfSN01RpiyEGjkpTHCClguGYEQyVB1/OpaFs4R1+7vUIgtYf8/
 QnMFlEPVjjxOAToZpR9GTnfQXeWBIiGH/pR9hNiTrdZoQ0iy2+tzJOeRf1SktoA+
 naM8THLCV8Sg1Mw4J87VBp6iSNnpn86CcDaTmjvfliHjWbcM2pE38P1ZWrOZyGls
 QyYBNWNgVYkDOnXYukrZVP/u3oDYLdE41V4tC5h9Pmzb/CaIxw==
 -----END CERTIFICATE-----
 
-# Issuer: CN=Chambers of Commerce Root - 2008 O=AC Camerfirma S.A.
-# Subject: CN=Chambers of Commerce Root - 2008 O=AC Camerfirma S.A.
-# Label: "Chambers of Commerce Root - 2008"
-# Serial: 11806822484801597146
-# MD5 Fingerprint: 5e:80:9e:84:5a:0e:65:0b:17:02:f3:55:18:2a:3e:d7
-# SHA1 Fingerprint: 78:6a:74:ac:76:ab:14:7f:9c:6a:30:50:ba:9e:a8:7e:fe:9a:ce:3c
-# SHA256 Fingerprint: 06:3e:4a:fa:c4:91:df:d3:32:f3:08:9b:85:42:e9:46:17:d8:93:d7:fe:94:4e:10:a7:93:7e:e2:9d:96:93:c0
------BEGIN CERTIFICATE-----
-MIIHTzCCBTegAwIBAgIJAKPaQn6ksa7aMA0GCSqGSIb3DQEBBQUAMIGuMQswCQYD
-VQQGEwJFVTFDMEEGA1UEBxM6TWFkcmlkIChzZWUgY3VycmVudCBhZGRyZXNzIGF0
-IHd3dy5jYW1lcmZpcm1hLmNvbS9hZGRyZXNzKTESMBAGA1UEBRMJQTgyNzQzMjg3
-MRswGQYDVQQKExJBQyBDYW1lcmZpcm1hIFMuQS4xKTAnBgNVBAMTIENoYW1iZXJz
-IG9mIENvbW1lcmNlIFJvb3QgLSAyMDA4MB4XDTA4MDgwMTEyMjk1MFoXDTM4MDcz
-MTEyMjk1MFowga4xCzAJBgNVBAYTAkVVMUMwQQYDVQQHEzpNYWRyaWQgKHNlZSBj
-dXJyZW50IGFkZHJlc3MgYXQgd3d3LmNhbWVyZmlybWEuY29tL2FkZHJlc3MpMRIw
-EAYDVQQFEwlBODI3NDMyODcxGzAZBgNVBAoTEkFDIENhbWVyZmlybWEgUy5BLjEp
-MCcGA1UEAxMgQ2hhbWJlcnMgb2YgQ29tbWVyY2UgUm9vdCAtIDIwMDgwggIiMA0G
-CSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQCvAMtwNyuAWko6bHiUfaN/Gh/2NdW9
-28sNRHI+JrKQUrpjOyhYb6WzbZSm891kDFX29ufyIiKAXuFixrYp4YFs8r/lfTJq
-VKAyGVn+H4vXPWCGhSRv4xGzdz4gljUha7MI2XAuZPeEklPWDrCQiorjh40G072Q
-DuKZoRuGDtqaCrsLYVAGUvGef3bsyw/QHg3PmTA9HMRFEFis1tPo1+XqxQEHd9ZR
-5gN/ikilTWh1uem8nk4ZcfUyS5xtYBkL+8ydddy/Js2Pk3g5eXNeJQ7KXOt3EgfL
-ZEFHcpOrUMPrCXZkNNI5t3YRCQ12RcSprj1qr7V9ZS+UWBDsXHyvfuK2GNnQm05a
-Sd+pZgvMPMZ4fKecHePOjlO+Bd5gD2vlGts/4+EhySnB8esHnFIbAURRPHsl18Tl
-UlRdJQfKFiC4reRB7noI/plvg6aRArBsNlVq5331lubKgdaX8ZSD6e2wsWsSaR6s
-+12pxZjptFtYer49okQ6Y1nUCyXeG0+95QGezdIp1Z8XGQpvvwyQ0wlf2eOKNcx5
-Wk0ZN5K3xMGtr/R5JJqyAQuxr1yW84Ay+1w9mPGgP0revq+ULtlVmhduYJ1jbLhj
-ya6BXBg14JC7vjxPNyK5fuvPnnchpj04gftI2jE9K+OJ9dC1vX7gUMQSibMjmhAx
-hduub+84Mxh2EQIDAQABo4IBbDCCAWgwEgYDVR0TAQH/BAgwBgEB/wIBDDAdBgNV
-HQ4EFgQU+SSsD7K1+HnA+mCIG8TZTQKeFxkwgeMGA1UdIwSB2zCB2IAU+SSsD7K1
-+HnA+mCIG8TZTQKeFxmhgbSkgbEwga4xCzAJBgNVBAYTAkVVMUMwQQYDVQQHEzpN
-YWRyaWQgKHNlZSBjdXJyZW50IGFkZHJlc3MgYXQgd3d3LmNhbWVyZmlybWEuY29t
-L2FkZHJlc3MpMRIwEAYDVQQFEwlBODI3NDMyODcxGzAZBgNVBAoTEkFDIENhbWVy
-ZmlybWEgUy5BLjEpMCcGA1UEAxMgQ2hhbWJlcnMgb2YgQ29tbWVyY2UgUm9vdCAt
-IDIwMDiCCQCj2kJ+pLGu2jAOBgNVHQ8BAf8EBAMCAQYwPQYDVR0gBDYwNDAyBgRV
-HSAAMCowKAYIKwYBBQUHAgEWHGh0dHA6Ly9wb2xpY3kuY2FtZXJmaXJtYS5jb20w
-DQYJKoZIhvcNAQEFBQADggIBAJASryI1wqM58C7e6bXpeHxIvj99RZJe6dqxGfwW
-PJ+0W2aeaufDuV2I6A+tzyMP3iU6XsxPpcG1Lawk0lgH3qLPaYRgM+gQDROpI9CF
-5Y57pp49chNyM/WqfcZjHwj0/gF/JM8rLFQJ3uIrbZLGOU8W6jx+ekbURWpGqOt1
-glanq6B8aBMz9p0w8G8nOSQjKpD9kCk18pPfNKXG9/jvjA9iSnyu0/VU+I22mlaH
-FoI6M6taIgj3grrqLuBHmrS1RaMFO9ncLkVAO+rcf+g769HsJtg1pDDFOqxXnrN2
-pSB7+R5KBWIBpih1YJeSDW4+TTdDDZIVnBgizVGZoCkaPF+KMjNbMMeJL0eYD6MD
-xvbxrN8y8NmBGuScvfaAFPDRLLmF9dijscilIeUcE5fuDr3fKanvNFNb0+RqE4QG
-tjICxFKuItLcsiFCGtpA8CnJ7AoMXOLQusxI0zcKzBIKinmwPQN/aUv0NCB9szTq
-jktk9T79syNnFQ0EuPAtwQlRPLJsFfClI9eDdOTlLsn+mCdCxqvGnrDQWzilm1De
-fhiYtUU79nm06PcaewaD+9CL2rvHvRirCG88gGtAPxkZumWK5r7VXNM21+9AUiRg
-OGcEMeyP84LG3rlV8zsxkVrctQgVrXYlCg17LofiDKYGvCYQbTed7N14jHyAxfDZ
-d0jQ
------END CERTIFICATE-----
-
-# Issuer: CN=Global Chambersign Root - 2008 O=AC Camerfirma S.A.
-# Subject: CN=Global Chambersign Root - 2008 O=AC Camerfirma S.A.
-# Label: "Global Chambersign Root - 2008"
-# Serial: 14541511773111788494
-# MD5 Fingerprint: 9e:80:ff:78:01:0c:2e:c1:36:bd:fe:96:90:6e:08:f3
-# SHA1 Fingerprint: 4a:bd:ee:ec:95:0d:35:9c:89:ae:c7:52:a1:2c:5b:29:f6:d6:aa:0c
-# SHA256 Fingerprint: 13:63:35:43:93:34:a7:69:80:16:a0:d3:24:de:72:28:4e:07:9d:7b:52:20:bb:8f:bd:74:78:16:ee:be:ba:ca
------BEGIN CERTIFICATE-----
-MIIHSTCCBTGgAwIBAgIJAMnN0+nVfSPOMA0GCSqGSIb3DQEBBQUAMIGsMQswCQYD
-VQQGEwJFVTFDMEEGA1UEBxM6TWFkcmlkIChzZWUgY3VycmVudCBhZGRyZXNzIGF0
-IHd3dy5jYW1lcmZpcm1hLmNvbS9hZGRyZXNzKTESMBAGA1UEBRMJQTgyNzQzMjg3
-MRswGQYDVQQKExJBQyBDYW1lcmZpcm1hIFMuQS4xJzAlBgNVBAMTHkdsb2JhbCBD
-aGFtYmVyc2lnbiBSb290IC0gMjAwODAeFw0wODA4MDExMjMxNDBaFw0zODA3MzEx
-MjMxNDBaMIGsMQswCQYDVQQGEwJFVTFDMEEGA1UEBxM6TWFkcmlkIChzZWUgY3Vy
-cmVudCBhZGRyZXNzIGF0IHd3dy5jYW1lcmZpcm1hLmNvbS9hZGRyZXNzKTESMBAG
-A1UEBRMJQTgyNzQzMjg3MRswGQYDVQQKExJBQyBDYW1lcmZpcm1hIFMuQS4xJzAl
-BgNVBAMTHkdsb2JhbCBDaGFtYmVyc2lnbiBSb290IC0gMjAwODCCAiIwDQYJKoZI
-hvcNAQEBBQADggIPADCCAgoCggIBAMDfVtPkOpt2RbQT2//BthmLN0EYlVJH6xed
-KYiONWwGMi5HYvNJBL99RDaxccy9Wglz1dmFRP+RVyXfXjaOcNFccUMd2drvXNL7
-G706tcuto8xEpw2uIRU/uXpbknXYpBI4iRmKt4DS4jJvVpyR1ogQC7N0ZJJ0YPP2
-zxhPYLIj0Mc7zmFLmY/CDNBAspjcDahOo7kKrmCgrUVSY7pmvWjg+b4aqIG7HkF4
-ddPB/gBVsIdU6CeQNR1MM62X/JcumIS/LMmjv9GYERTtY/jKmIhYF5ntRQOXfjyG
-HoiMvvKRhI9lNNgATH23MRdaKXoKGCQwoze1eqkBfSbW+Q6OWfH9GzO1KTsXO0G2
-Id3UwD2ln58fQ1DJu7xsepeY7s2MH/ucUa6LcL0nn3HAa6x9kGbo1106DbDVwo3V
-yJ2dwW3Q0L9R5OP4wzg2rtandeavhENdk5IMagfeOx2YItaswTXbo6Al/3K1dh3e
-beksZixShNBFks4c5eUzHdwHU1SjqoI7mjcv3N2gZOnm3b2u/GSFHTynyQbehP9r
-6GsaPMWis0L7iwk+XwhSx2LE1AVxv8Rk5Pihg+g+EpuoHtQ2TS9x9o0o9oOpE9Jh
-wZG7SMA0j0GMS0zbaRL/UJScIINZc+18ofLx/d33SdNDWKBWY8o9PeU1VlnpDsog
-zCtLkykPAgMBAAGjggFqMIIBZjASBgNVHRMBAf8ECDAGAQH/AgEMMB0GA1UdDgQW
-BBS5CcqcHtvTbDprru1U8VuTBjUuXjCB4QYDVR0jBIHZMIHWgBS5CcqcHtvTbDpr
-ru1U8VuTBjUuXqGBsqSBrzCBrDELMAkGA1UEBhMCRVUxQzBBBgNVBAcTOk1hZHJp
-ZCAoc2VlIGN1cnJlbnQgYWRkcmVzcyBhdCB3d3cuY2FtZXJmaXJtYS5jb20vYWRk
-cmVzcykxEjAQBgNVBAUTCUE4Mjc0MzI4NzEbMBkGA1UEChMSQUMgQ2FtZXJmaXJt
-YSBTLkEuMScwJQYDVQQDEx5HbG9iYWwgQ2hhbWJlcnNpZ24gUm9vdCAtIDIwMDiC
-CQDJzdPp1X0jzjAOBgNVHQ8BAf8EBAMCAQYwPQYDVR0gBDYwNDAyBgRVHSAAMCow
-KAYIKwYBBQUHAgEWHGh0dHA6Ly9wb2xpY3kuY2FtZXJmaXJtYS5jb20wDQYJKoZI
-hvcNAQEFBQADggIBAICIf3DekijZBZRG/5BXqfEv3xoNa/p8DhxJJHkn2EaqbylZ
-UohwEurdPfWbU1Rv4WCiqAm57OtZfMY18dwY6fFn5a+6ReAJ3spED8IXDneRRXoz
-X1+WLGiLwUePmJs9wOzL9dWCkoQ10b42OFZyMVtHLaoXpGNR6woBrX/sdZ7LoR/x
-fxKxueRkf2fWIyr0uDldmOghp+G9PUIadJpwr2hsUF1Jz//7Dl3mLEfXgTpZALVz
-a2Mg9jFFCDkO9HB+QHBaP9BrQql0PSgvAm11cpUJjUhjxsYjV5KTXjXBjfkK9yyd
-Yhz2rXzdpjEetrHHfoUm+qRqtdpjMNHvkzeyZi99Bffnt0uYlDXA2TopwZ2yUDMd
-SqlapskD7+3056huirRXhOukP9DuqqqHW2Pok+JrqNS4cnhrG+055F3Lm6qH1U9O
-AP7Zap88MQ8oAgF9mOinsKJknnn4SPIVqczmyETrP3iZ8ntxPjzxmKfFGBI/5rso
-M0LpRQp8bfKGeS/Fghl9CYl8slR2iK7ewfPM4W7bMdaTrpmg7yVqc5iJWzouE4ge
-v8CSlDQb4ye3ix5vQv/n6TebUB0tovkC7stYWDpxvGjjqsGvHCgfotwjZT+B6q6Z
-09gwzxMNTxXJhLynSC34MCN32EZLeW32jO06f2ARePTpm67VVMB0gNELQp/B
------END CERTIFICATE-----
-
 # Issuer: CN=Go Daddy Root Certificate Authority - G2 O=GoDaddy.com, Inc.
 # Subject: CN=Go Daddy Root Certificate Authority - G2 O=GoDaddy.com, Inc.
 # Label: "Go Daddy Root Certificate Authority - G2"
 # Serial: 0
 # MD5 Fingerprint: 80:3a:bc:22:c1:e6:fb:8d:9b:3b:27:4a:32:1b:9a:01
 # SHA1 Fingerprint: 47:be:ab:c9:22:ea:e8:0e:78:78:34:62:a7:9f:45:c2:54:fd:e6:8b
 # SHA256 Fingerprint: 45:14:0b:32:47:eb:9c:c8:c5:b4:f0:d7:b5:30:91:f7:32:92:08:9e:6e:5a:63:e2:74:9d:d3:ac:a9:19:8e:da
@@ -1636,86 +1288,14 @@
 coJxDjrSzG+ntKEju/Ykn8sX/oymzsLS28yN/HH8AynBbF0zX2S2ZTuJbxh2ePXc
 okgfGT+Ok+vx+hfuzU7jBBJV1uXk3fs+BXziHV7Gp7yXT2g69ekuCkO2r1dcYmh8
 t/2jioSgrGK+KwmHNPBqAbubKVY8/gA3zyNs8U6qtnRGEmyR7jTV7JqR50S+kDFy
 1UkC9gLl9B/rfNmWVan/7Ir5mUf/NVoCqgTLiluHcSmRvaS0eg29mvVXIwAHIRc/
 SjnRBUkLp7Y3gaVdjKozXoEofKd9J+sAro03
 -----END CERTIFICATE-----
 
-# Issuer: CN=EC-ACC O=Agencia Catalana de Certificacio (NIF Q-0801176-I) OU=Serveis Publics de Certificacio/Vegeu https://www.catcert.net/verarrel (c)03/Jerarquia Entitats de Certificacio Catalanes
-# Subject: CN=EC-ACC O=Agencia Catalana de Certificacio (NIF Q-0801176-I) OU=Serveis Publics de Certificacio/Vegeu https://www.catcert.net/verarrel (c)03/Jerarquia Entitats de Certificacio Catalanes
-# Label: "EC-ACC"
-# Serial: -23701579247955709139626555126524820479
-# MD5 Fingerprint: eb:f5:9d:29:0d:61:f9:42:1f:7c:c2:ba:6d:e3:15:09
-# SHA1 Fingerprint: 28:90:3a:63:5b:52:80:fa:e6:77:4c:0b:6d:a7:d6:ba:a6:4a:f2:e8
-# SHA256 Fingerprint: 88:49:7f:01:60:2f:31:54:24:6a:e2:8c:4d:5a:ef:10:f1:d8:7e:bb:76:62:6f:4a:e0:b7:f9:5b:a7:96:87:99
------BEGIN CERTIFICATE-----
-MIIFVjCCBD6gAwIBAgIQ7is969Qh3hSoYqwE893EATANBgkqhkiG9w0BAQUFADCB
-8zELMAkGA1UEBhMCRVMxOzA5BgNVBAoTMkFnZW5jaWEgQ2F0YWxhbmEgZGUgQ2Vy
-dGlmaWNhY2lvIChOSUYgUS0wODAxMTc2LUkpMSgwJgYDVQQLEx9TZXJ2ZWlzIFB1
-YmxpY3MgZGUgQ2VydGlmaWNhY2lvMTUwMwYDVQQLEyxWZWdldSBodHRwczovL3d3
-dy5jYXRjZXJ0Lm5ldC92ZXJhcnJlbCAoYykwMzE1MDMGA1UECxMsSmVyYXJxdWlh
-IEVudGl0YXRzIGRlIENlcnRpZmljYWNpbyBDYXRhbGFuZXMxDzANBgNVBAMTBkVD
-LUFDQzAeFw0wMzAxMDcyMzAwMDBaFw0zMTAxMDcyMjU5NTlaMIHzMQswCQYDVQQG
-EwJFUzE7MDkGA1UEChMyQWdlbmNpYSBDYXRhbGFuYSBkZSBDZXJ0aWZpY2FjaW8g
-KE5JRiBRLTA4MDExNzYtSSkxKDAmBgNVBAsTH1NlcnZlaXMgUHVibGljcyBkZSBD
-ZXJ0aWZpY2FjaW8xNTAzBgNVBAsTLFZlZ2V1IGh0dHBzOi8vd3d3LmNhdGNlcnQu
-bmV0L3ZlcmFycmVsIChjKTAzMTUwMwYDVQQLEyxKZXJhcnF1aWEgRW50aXRhdHMg
-ZGUgQ2VydGlmaWNhY2lvIENhdGFsYW5lczEPMA0GA1UEAxMGRUMtQUNDMIIBIjAN
-BgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAsyLHT+KXQpWIR4NA9h0X84NzJB5R
-85iKw5K4/0CQBXCHYMkAqbWUZRkiFRfCQ2xmRJoNBD45b6VLeqpjt4pEndljkYRm
-4CgPukLjbo73FCeTae6RDqNfDrHrZqJyTxIThmV6PttPB/SnCWDaOkKZx7J/sxaV
-HMf5NLWUhdWZXqBIoH7nF2W4onW4HvPlQn2v7fOKSGRdghST2MDk/7NQcvJ29rNd
-QlB50JQ+awwAvthrDk4q7D7SzIKiGGUzE3eeml0aE9jD2z3Il3rucO2n5nzbcc8t
-lGLfbdb1OL4/pYUKGbio2Al1QnDE6u/LDsg0qBIimAy4E5S2S+zw0JDnJwIDAQAB
-o4HjMIHgMB0GA1UdEQQWMBSBEmVjX2FjY0BjYXRjZXJ0Lm5ldDAPBgNVHRMBAf8E
-BTADAQH/MA4GA1UdDwEB/wQEAwIBBjAdBgNVHQ4EFgQUoMOLRKo3pUW/l4Ba0fF4
-opvpXY0wfwYDVR0gBHgwdjB0BgsrBgEEAfV4AQMBCjBlMCwGCCsGAQUFBwIBFiBo
-dHRwczovL3d3dy5jYXRjZXJ0Lm5ldC92ZXJhcnJlbDA1BggrBgEFBQcCAjApGidW
-ZWdldSBodHRwczovL3d3dy5jYXRjZXJ0Lm5ldC92ZXJhcnJlbCAwDQYJKoZIhvcN
-AQEFBQADggEBAKBIW4IB9k1IuDlVNZyAelOZ1Vr/sXE7zDkJlF7W2u++AVtd0x7Y
-/X1PzaBB4DSTv8vihpw3kpBWHNzrKQXlxJ7HNd+KDM3FIUPpqojlNcAZQmNaAl6k
-SBg6hW/cnbw/nZzBh7h6YQjpdwt/cKt63dmXLGQehb+8dJahw3oS7AwaboMMPOhy
-Rp/7SNVel+axofjk70YllJyJ22k4vuxcDlbHZVHlUIiIv0LVKz3l+bqeLrPK9HOS
-Agu+TGbrIP65y7WZf+a2E/rKS03Z7lNGBjvGTq2TWoF+bCpLagVFjPIhpDGQh2xl
-nJ2lYJU6Un/10asIbvPuW/mIPX64b24D5EI=
------END CERTIFICATE-----
-
-# Issuer: CN=Hellenic Academic and Research Institutions RootCA 2011 O=Hellenic Academic and Research Institutions Cert. Authority
-# Subject: CN=Hellenic Academic and Research Institutions RootCA 2011 O=Hellenic Academic and Research Institutions Cert. Authority
-# Label: "Hellenic Academic and Research Institutions RootCA 2011"
-# Serial: 0
-# MD5 Fingerprint: 73:9f:4c:4b:73:5b:79:e9:fa:ba:1c:ef:6e:cb:d5:c9
-# SHA1 Fingerprint: fe:45:65:9b:79:03:5b:98:a1:61:b5:51:2e:ac:da:58:09:48:22:4d
-# SHA256 Fingerprint: bc:10:4f:15:a4:8b:e7:09:dc:a5:42:a7:e1:d4:b9:df:6f:05:45:27:e8:02:ea:a9:2d:59:54:44:25:8a:fe:71
------BEGIN CERTIFICATE-----
-MIIEMTCCAxmgAwIBAgIBADANBgkqhkiG9w0BAQUFADCBlTELMAkGA1UEBhMCR1Ix
-RDBCBgNVBAoTO0hlbGxlbmljIEFjYWRlbWljIGFuZCBSZXNlYXJjaCBJbnN0aXR1
-dGlvbnMgQ2VydC4gQXV0aG9yaXR5MUAwPgYDVQQDEzdIZWxsZW5pYyBBY2FkZW1p
-YyBhbmQgUmVzZWFyY2ggSW5zdGl0dXRpb25zIFJvb3RDQSAyMDExMB4XDTExMTIw
-NjEzNDk1MloXDTMxMTIwMTEzNDk1MlowgZUxCzAJBgNVBAYTAkdSMUQwQgYDVQQK
-EztIZWxsZW5pYyBBY2FkZW1pYyBhbmQgUmVzZWFyY2ggSW5zdGl0dXRpb25zIENl
-cnQuIEF1dGhvcml0eTFAMD4GA1UEAxM3SGVsbGVuaWMgQWNhZGVtaWMgYW5kIFJl
-c2VhcmNoIEluc3RpdHV0aW9ucyBSb290Q0EgMjAxMTCCASIwDQYJKoZIhvcNAQEB
-BQADggEPADCCAQoCggEBAKlTAOMupvaO+mDYLZU++CwqVE7NuYRhlFhPjz2L5EPz
-dYmNUeTDN9KKiE15HrcS3UN4SoqS5tdI1Q+kOilENbgH9mgdVc04UfCMJDGFr4PJ
-fel3r+0ae50X+bOdOFAPplp5kYCvN66m0zH7tSYJnTxa71HFK9+WXesyHgLacEns
-bgzImjeN9/E2YEsmLIKe0HjzDQ9jpFEw4fkrJxIH2Oq9GGKYsFk3fb7u8yBRQlqD
-75O6aRXxYp2fmTmCobd0LovUxQt7L/DICto9eQqakxylKHJzkUOap9FNhYS5qXSP
-FEDH3N6sQWRstBmbAmNtJGSPRLIl6s5ddAxjMlyNh+UCAwEAAaOBiTCBhjAPBgNV
-HRMBAf8EBTADAQH/MAsGA1UdDwQEAwIBBjAdBgNVHQ4EFgQUppFC/RNhSiOeCKQp
-5dgTBCPuQSUwRwYDVR0eBEAwPqA8MAWCAy5ncjAFggMuZXUwBoIELmVkdTAGggQu
-b3JnMAWBAy5ncjAFgQMuZXUwBoEELmVkdTAGgQQub3JnMA0GCSqGSIb3DQEBBQUA
-A4IBAQAf73lB4XtuP7KMhjdCSk4cNx6NZrokgclPEg8hwAOXhiVtXdMiKahsog2p
-6z0GW5k6x8zDmjR/qw7IThzh+uTczQ2+vyT+bOdrwg3IBp5OjWEopmr95fZi6hg8
-TqBTnbI6nOulnJEWtk2C4AwFSKls9cz4y51JtPACpf1wA+2KIaWuE4ZJwzNzvoc7
-dIsXRSZMFpGD/md9zU1jZ/rzAxKWeAaNsWftjj++n08C9bMJL/NMh98qy5V8Acys
-Nnq/onN694/BtZqhFLKPM58N7yLcZnuEvUUXBj08yrl3NI/K6s8/MT7jiOOASSXI
-l7WdmplNsDz4SgCbZN2fOUvRJ9e4
------END CERTIFICATE-----
-
 # Issuer: CN=Actalis Authentication Root CA O=Actalis S.p.A./03358520967
 # Subject: CN=Actalis Authentication Root CA O=Actalis S.p.A./03358520967
 # Label: "Actalis Authentication Root CA"
 # Serial: 6271844772424770508
 # MD5 Fingerprint: 69:c1:0d:4f:07:a3:1b:c3:fe:56:3d:04:bc:11:f6:a6
 # SHA1 Fingerprint: f3:73:b3:87:06:5a:28:84:8a:f2:f3:4a:ce:19:2b:dd:c7:8e:9c:ac
 # SHA256 Fingerprint: 55:92:60:84:ec:96:3a:64:b9:6e:2a:be:01:ce:0b:a8:6a:64:fb:fe:bc:c7:aa:b5:af:c1:55:b3:7f:d7:60:66
@@ -1749,43 +1329,14 @@
 fcvHlXHo2qN8xcL4dJIEG4aspCJTQLas/kx2z/uUMsA1n3Y/buWQbqCmJqK4LL7R
 K4X9p2jIugErsWx0Hbhzlefut8cl8ABMALJ+tguLHPPAUJ4lueAI3jZm/zel0btU
 ZCzJJ7VLkn5l/9Mt4blOvH+kQSGQQXemOR/qnuOf0GZvBeyqdn6/axag67XH/JJU
 LysRJyU3eExRarDzzFhdFPFqSBX/wge2sY0PjlxQRrM9vwGYT7JZVEc+NHt4bVaT
 LnPqZih4zR0Uv6CPLy64Lo7yFIrM6bV8+2ydDKXhlg==
 -----END CERTIFICATE-----
 
-# Issuer: O=Trustis Limited OU=Trustis FPS Root CA
-# Subject: O=Trustis Limited OU=Trustis FPS Root CA
-# Label: "Trustis FPS Root CA"
-# Serial: 36053640375399034304724988975563710553
-# MD5 Fingerprint: 30:c9:e7:1e:6b:e6:14:eb:65:b2:16:69:20:31:67:4d
-# SHA1 Fingerprint: 3b:c0:38:0b:33:c3:f6:a6:0c:86:15:22:93:d9:df:f5:4b:81:c0:04
-# SHA256 Fingerprint: c1:b4:82:99:ab:a5:20:8f:e9:63:0a:ce:55:ca:68:a0:3e:da:5a:51:9c:88:02:a0:d3:a6:73:be:8f:8e:55:7d
------BEGIN CERTIFICATE-----
-MIIDZzCCAk+gAwIBAgIQGx+ttiD5JNM2a/fH8YygWTANBgkqhkiG9w0BAQUFADBF
-MQswCQYDVQQGEwJHQjEYMBYGA1UEChMPVHJ1c3RpcyBMaW1pdGVkMRwwGgYDVQQL
-ExNUcnVzdGlzIEZQUyBSb290IENBMB4XDTAzMTIyMzEyMTQwNloXDTI0MDEyMTEx
-MzY1NFowRTELMAkGA1UEBhMCR0IxGDAWBgNVBAoTD1RydXN0aXMgTGltaXRlZDEc
-MBoGA1UECxMTVHJ1c3RpcyBGUFMgUm9vdCBDQTCCASIwDQYJKoZIhvcNAQEBBQAD
-ggEPADCCAQoCggEBAMVQe547NdDfxIzNjpvto8A2mfRC6qc+gIMPpqdZh8mQRUN+
-AOqGeSoDvT03mYlmt+WKVoaTnGhLaASMk5MCPjDSNzoiYYkchU59j9WvezX2fihH
-iTHcDnlkH5nSW7r+f2C/revnPDgpai/lkQtV/+xvWNUtyd5MZnGPDNcE2gfmHhjj
-vSkCqPoc4Vu5g6hBSLwacY3nYuUtsuvffM/bq1rKMfFMIvMFE/eC+XN5DL7XSxzA
-0RU8k0Fk0ea+IxciAIleH2ulrG6nS4zto3Lmr2NNL4XSFDWaLk6M6jKYKIahkQlB
-OrTh4/L68MkKokHdqeMDx4gVOxzUGpTXn2RZEm0CAwEAAaNTMFEwDwYDVR0TAQH/
-BAUwAwEB/zAfBgNVHSMEGDAWgBS6+nEleYtXQSUhhgtx67JkDoshZzAdBgNVHQ4E
-FgQUuvpxJXmLV0ElIYYLceuyZA6LIWcwDQYJKoZIhvcNAQEFBQADggEBAH5Y//01
-GX2cGE+esCu8jowU/yyg2kdbw++BLa8F6nRIW/M+TgfHbcWzk88iNVy2P3UnXwmW
-zaD+vkAMXBJV+JOCyinpXj9WV4s4NvdFGkwozZ5BuO1WTISkQMi4sKUraXAEasP4
-1BIy+Q7DsdwyhEQsb8tGD+pmQQ9P8Vilpg0ND2HepZ5dfWWhPBfnqFVO76DH7cZE
-f1T1o+CP8HxVIo8ptoGj4W1OLBuAZ+ytIJ8MYmHVl/9D7S3B2l0pKoU/rGXuhg8F
-jZBf3+6f9L/uHfuY5H+QK4R4EA5sSVPvFVtlRkpdr7r7OnIdzfYliB6XzCGcKQEN
-ZetX2fNXlrtIzYE=
------END CERTIFICATE-----
-
 # Issuer: CN=Buypass Class 2 Root CA O=Buypass AS-983163327
 # Subject: CN=Buypass Class 2 Root CA O=Buypass AS-983163327
 # Label: "Buypass Class 2 Root CA"
 # Serial: 2
 # MD5 Fingerprint: 46:a7:d2:fe:45:fb:64:5a:a8:59:90:9b:78:44:9b:29
 # SHA1 Fingerprint: 49:0a:75:74:de:87:0a:47:fe:58:ee:f6:c7:6b:eb:c6:0b:12:40:99
 # SHA256 Fingerprint: 9a:11:40:25:19:7c:5b:b9:5d:94:e6:3d:55:cd:43:79:08:47:b6:46:b2:3c:df:11:ad:a4:a0:0e:ff:15:fb:48
@@ -2596,35 +2147,14 @@
 o4N+LZfQYcTxmdwlkWOrfzCjtHDix6EznPO/LlxTsV+zfTJ/ijTjeXmjQjBAMB0G
 A1UdDgQWBBQ64QmG1M8ZwpZ2dEl23OA1xmNjmjAOBgNVHQ8BAf8EBAMCAQYwDwYD
 VR0TAQH/BAUwAwEB/zAKBggqhkjOPQQDAwNoADBlAjA2Z6EWCNzklwBBHU6+4WMB
 zzuqQhFkoJ2UOQIReVx7Hfpkue4WQrO/isIJxOzksU0CMQDpKmFHjFJKS04YcPbW
 RNZu9YO6bVi9JNlWSOrvxKJGgYhqOkbRqZtNyWHa0V1Xahg=
 -----END CERTIFICATE-----
 
-# Issuer: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R4
-# Subject: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R4
-# Label: "GlobalSign ECC Root CA - R4"
-# Serial: 14367148294922964480859022125800977897474
-# MD5 Fingerprint: 20:f0:27:68:d1:7e:a0:9d:0e:e6:2a:ca:df:5c:89:8e
-# SHA1 Fingerprint: 69:69:56:2e:40:80:f4:24:a1:e7:19:9f:14:ba:f3:ee:58:ab:6a:bb
-# SHA256 Fingerprint: be:c9:49:11:c2:95:56:76:db:6c:0a:55:09:86:d7:6e:3b:a0:05:66:7c:44:2c:97:62:b4:fb:b7:73:de:22:8c
------BEGIN CERTIFICATE-----
-MIIB4TCCAYegAwIBAgIRKjikHJYKBN5CsiilC+g0mAIwCgYIKoZIzj0EAwIwUDEk
-MCIGA1UECxMbR2xvYmFsU2lnbiBFQ0MgUm9vdCBDQSAtIFI0MRMwEQYDVQQKEwpH
-bG9iYWxTaWduMRMwEQYDVQQDEwpHbG9iYWxTaWduMB4XDTEyMTExMzAwMDAwMFoX
-DTM4MDExOTAzMTQwN1owUDEkMCIGA1UECxMbR2xvYmFsU2lnbiBFQ0MgUm9vdCBD
-QSAtIFI0MRMwEQYDVQQKEwpHbG9iYWxTaWduMRMwEQYDVQQDEwpHbG9iYWxTaWdu
-MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEuMZ5049sJQ6fLjkZHAOkrprlOQcJ
-FspjsbmG+IpXwVfOQvpzofdlQv8ewQCybnMO/8ch5RikqtlxP6jUuc6MHaNCMEAw
-DgYDVR0PAQH/BAQDAgEGMA8GA1UdEwEB/wQFMAMBAf8wHQYDVR0OBBYEFFSwe61F
-uOJAf/sKbvu+M8k8o4TVMAoGCCqGSM49BAMCA0gAMEUCIQDckqGgE6bPA7DmxCGX
-kPoUVy0D7O48027KqGx2vKLeuwIgJ6iFJzWbVsaj8kfSt24bAgAXqmemFZHe+pTs
-ewv4n4Q=
------END CERTIFICATE-----
-
 # Issuer: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R5
 # Subject: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R5
 # Label: "GlobalSign ECC Root CA - R5"
 # Serial: 32785792099990507226680698011560947931244
 # MD5 Fingerprint: 9f:ad:3b:1c:02:1e:8a:ba:17:74:38:81:0c:a2:bc:08
 # SHA1 Fingerprint: 1f:24:c6:30:cd:a4:18:ef:20:69:ff:ad:4f:dd:5f:46:3a:1b:69:aa
 # SHA256 Fingerprint: 17:9f:bc:14:8a:3d:d0:0f:d2:4e:a1:34:58:cc:43:bf:a7:f5:9c:81:82:d7:83:a5:13:f6:eb:ec:10:0c:89:24
@@ -2639,94 +2169,14 @@
 hOvRnkmSh5SHDDqFSmafnVmTTZdhBoZKo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYD
 VR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUPeYpSJvqB8ohREom3m7e0oPQn1kwCgYI
 KoZIzj0EAwMDaAAwZQIxAOVpEslu28YxuglB4Zf4+/2a4n0Sye18ZNPLBSWLVtmg
 515dTguDnFt2KaAJJiFqYgIwcdK1j1zqO+F4CYWodZI7yFz9SO8NdCKoCOJuxUnO
 xwy8p2Fp8fc74SrL+SvzZpA3
 -----END CERTIFICATE-----
 
-# Issuer: CN=Staat der Nederlanden Root CA - G3 O=Staat der Nederlanden
-# Subject: CN=Staat der Nederlanden Root CA - G3 O=Staat der Nederlanden
-# Label: "Staat der Nederlanden Root CA - G3"
-# Serial: 10003001
-# MD5 Fingerprint: 0b:46:67:07:db:10:2f:19:8c:35:50:60:d1:0b:f4:37
-# SHA1 Fingerprint: d8:eb:6b:41:51:92:59:e0:f3:e7:85:00:c0:3d:b6:88:97:c9:ee:fc
-# SHA256 Fingerprint: 3c:4f:b0:b9:5a:b8:b3:00:32:f4:32:b8:6f:53:5f:e1:72:c1:85:d0:fd:39:86:58:37:cf:36:18:7f:a6:f4:28
------BEGIN CERTIFICATE-----
-MIIFdDCCA1ygAwIBAgIEAJiiOTANBgkqhkiG9w0BAQsFADBaMQswCQYDVQQGEwJO
-TDEeMBwGA1UECgwVU3RhYXQgZGVyIE5lZGVybGFuZGVuMSswKQYDVQQDDCJTdGFh
-dCBkZXIgTmVkZXJsYW5kZW4gUm9vdCBDQSAtIEczMB4XDTEzMTExNDExMjg0MloX
-DTI4MTExMzIzMDAwMFowWjELMAkGA1UEBhMCTkwxHjAcBgNVBAoMFVN0YWF0IGRl
-ciBOZWRlcmxhbmRlbjErMCkGA1UEAwwiU3RhYXQgZGVyIE5lZGVybGFuZGVuIFJv
-b3QgQ0EgLSBHMzCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBAL4yolQP
-cPssXFnrbMSkUeiFKrPMSjTysF/zDsccPVMeiAho2G89rcKezIJnByeHaHE6n3WW
-IkYFsO2tx1ueKt6c/DrGlaf1F2cY5y9JCAxcz+bMNO14+1Cx3Gsy8KL+tjzk7FqX
-xz8ecAgwoNzFs21v0IJyEavSgWhZghe3eJJg+szeP4TrjTgzkApyI/o1zCZxMdFy
-KJLZWyNtZrVtB0LrpjPOktvA9mxjeM3KTj215VKb8b475lRgsGYeCasH/lSJEULR
-9yS6YHgamPfJEf0WwTUaVHXvQ9Plrk7O53vDxk5hUUurmkVLoR9BvUhTFXFkC4az
-5S6+zqQbwSmEorXLCCN2QyIkHxcE1G6cxvx/K2Ya7Irl1s9N9WMJtxU51nus6+N8
-6U78dULI7ViVDAZCopz35HCz33JvWjdAidiFpNfxC95DGdRKWCyMijmev4SH8RY7
-Ngzp07TKbBlBUgmhHbBqv4LvcFEhMtwFdozL92TkA1CvjJFnq8Xy7ljY3r735zHP
-bMk7ccHViLVlvMDoFxcHErVc0qsgk7TmgoNwNsXNo42ti+yjwUOH5kPiNL6VizXt
-BznaqB16nzaeErAMZRKQFWDZJkBE41ZgpRDUajz9QdwOWke275dhdU/Z/seyHdTt
-XUmzqWrLZoQT1Vyg3N9udwbRcXXIV2+vD3dbAgMBAAGjQjBAMA8GA1UdEwEB/wQF
-MAMBAf8wDgYDVR0PAQH/BAQDAgEGMB0GA1UdDgQWBBRUrfrHkleuyjWcLhL75Lpd
-INyUVzANBgkqhkiG9w0BAQsFAAOCAgEAMJmdBTLIXg47mAE6iqTnB/d6+Oea31BD
-U5cqPco8R5gu4RV78ZLzYdqQJRZlwJ9UXQ4DO1t3ApyEtg2YXzTdO2PCwyiBwpwp
-LiniyMMB8jPqKqrMCQj3ZWfGzd/TtiunvczRDnBfuCPRy5FOCvTIeuXZYzbB1N/8
-Ipf3YF3qKS9Ysr1YvY2WTxB1v0h7PVGHoTx0IsL8B3+A3MSs/mrBcDCw6Y5p4ixp
-gZQJut3+TcCDjJRYwEYgr5wfAvg1VUkvRtTA8KCWAg8zxXHzniN9lLf9OtMJgwYh
-/WA9rjLA0u6NpvDntIJ8CsxwyXmA+P5M9zWEGYox+wrZ13+b8KKaa8MFSu1BYBQw
-0aoRQm7TIwIEC8Zl3d1Sd9qBa7Ko+gE4uZbqKmxnl4mUnrzhVNXkanjvSr0rmj1A
-fsbAddJu+2gw7OyLnflJNZoaLNmzlTnVHpL3prllL+U9bTpITAjc5CgSKL59NVzq
-4BZ+Extq1z7XnvwtdbLBFNUjA9tbbws+eC8N3jONFrdI54OagQ97wUNNVQQXOEpR
-1VmiiXTTn74eS9fGbbeIJG9gkaSChVtWQbzQRKtqE77RLFi3EjNYsjdj3BP1lB0/
-QFH1T/U67cjF68IeHRaVesd+QnGTbksVtzDfqu1XhUisHWrdOWnk4Xl4vs4Fv6EM
-94B7IWcnMFk=
------END CERTIFICATE-----
-
-# Issuer: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Subject: CN=Staat der Nederlanden EV Root CA O=Staat der Nederlanden
-# Label: "Staat der Nederlanden EV Root CA"
-# Serial: 10000013
-# MD5 Fingerprint: fc:06:af:7b:e8:1a:f1:9a:b4:e8:d2:70:1f:c0:f5:ba
-# SHA1 Fingerprint: 76:e2:7e:c1:4f:db:82:c1:c0:a6:75:b5:05:be:3d:29:b4:ed:db:bb
-# SHA256 Fingerprint: 4d:24:91:41:4c:fe:95:67:46:ec:4c:ef:a6:cf:6f:72:e2:8a:13:29:43:2f:9d:8a:90:7a:c4:cb:5d:ad:c1:5a
------BEGIN CERTIFICATE-----
-MIIFcDCCA1igAwIBAgIEAJiWjTANBgkqhkiG9w0BAQsFADBYMQswCQYDVQQGEwJO
-TDEeMBwGA1UECgwVU3RhYXQgZGVyIE5lZGVybGFuZGVuMSkwJwYDVQQDDCBTdGFh
-dCBkZXIgTmVkZXJsYW5kZW4gRVYgUm9vdCBDQTAeFw0xMDEyMDgxMTE5MjlaFw0y
-MjEyMDgxMTEwMjhaMFgxCzAJBgNVBAYTAk5MMR4wHAYDVQQKDBVTdGFhdCBkZXIg
-TmVkZXJsYW5kZW4xKTAnBgNVBAMMIFN0YWF0IGRlciBOZWRlcmxhbmRlbiBFViBS
-b290IENBMIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEA48d+ifkkSzrS
-M4M1LGns3Amk41GoJSt5uAg94JG6hIXGhaTK5skuU6TJJB79VWZxXSzFYGgEt9nC
-UiY4iKTWO0Cmws0/zZiTs1QUWJZV1VD+hq2kY39ch/aO5ieSZxeSAgMs3NZmdO3d
-Z//BYY1jTw+bbRcwJu+r0h8QoPnFfxZpgQNH7R5ojXKhTbImxrpsX23Wr9GxE46p
-rfNeaXUmGD5BKyF/7otdBwadQ8QpCiv8Kj6GyzyDOvnJDdrFmeK8eEEzduG/L13l
-pJhQDBXd4Pqcfzho0LKmeqfRMb1+ilgnQ7O6M5HTp5gVXJrm0w912fxBmJc+qiXb
-j5IusHsMX/FjqTf5m3VpTCgmJdrV8hJwRVXj33NeN/UhbJCONVrJ0yPr08C+eKxC
-KFhmpUZtcALXEPlLVPxdhkqHz3/KRawRWrUgUY0viEeXOcDPusBCAUCZSCELa6fS
-/ZbV0b5GnUngC6agIk440ME8MLxwjyx1zNDFjFE7PZQIZCZhfbnDZY8UnCHQqv0X
-cgOPvZuM5l5Tnrmd74K74bzickFbIZTTRTeU0d8JOV3nI6qaHcptqAqGhYqCvkIH
-1vI4gnPah1vlPNOePqc7nvQDs/nxfRN0Av+7oeX6AHkcpmZBiFxgV6YuCcS6/ZrP
-px9Aw7vMWgpVSzs4dlG4Y4uElBbmVvMCAwEAAaNCMEAwDwYDVR0TAQH/BAUwAwEB
-/zAOBgNVHQ8BAf8EBAMCAQYwHQYDVR0OBBYEFP6rAJCYniT8qcwaivsnuL8wbqg7
-MA0GCSqGSIb3DQEBCwUAA4ICAQDPdyxuVr5Os7aEAJSrR8kN0nbHhp8dB9O2tLsI
-eK9p0gtJ3jPFrK3CiAJ9Brc1AsFgyb/E6JTe1NOpEyVa/m6irn0F3H3zbPB+po3u
-2dfOWBfoqSmuc0iH55vKbimhZF8ZE/euBhD/UcabTVUlT5OZEAFTdfETzsemQUHS
-v4ilf0X8rLiltTMMgsT7B/Zq5SWEXwbKwYY5EdtYzXc7LMJMD16a4/CrPmEbUCTC
-wPTxGfARKbalGAKb12NMcIxHowNDXLldRqANb/9Zjr7dn3LDWyvfjFvO5QxGbJKy
-CqNMVEIYFRIYvdr8unRu/8G2oGTYqV9Vrp9canaW2HNnh/tNf1zuacpzEPuKqf2e
-vTY4SUmH9A4U8OmHuD+nT3pajnnUk+S7aFKErGzp85hwVXIy+TSrK0m1zSBi5Dp6
-Z2Orltxtrpfs/J92VoguZs9btsmksNcFuuEnL5O7Jiqik7Ab846+HUCjuTaPPoIa
-Gl6I6lD4WeKDRikL40Rc4ZW2aZCaFG+XroHPaO+Zmr615+F/+PoTRxZMzG0IQOeL
-eG9QgkRQP2YGiqtDhFZKDyAthg710tvSeopLzaXoTvFeJiUBWSOgftL2fiFX1ye8
-FVdMpEbB4IMeDExNH08GGeL5qPQ6gqGyeUN51q1veieQA6TqJIc/2b3Z6fJfUEkc
-7uzXLg==
------END CERTIFICATE-----
-
 # Issuer: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Subject: CN=IdenTrust Commercial Root CA 1 O=IdenTrust
 # Label: "IdenTrust Commercial Root CA 1"
 # Serial: 13298821034946342390520003877796839426
 # MD5 Fingerprint: b3:3e:77:73:75:ee:a0:d3:e3:7e:49:63:49:59:bb:c7
 # SHA1 Fingerprint: df:71:7e:aa:4a:d9:4e:c9:55:84:99:60:2d:48:de:5f:bc:f0:3a:25
 # SHA256 Fingerprint: 5d:56:49:9b:e4:d2:e0:8b:cf:ca:d0:8a:3e:38:72:3d:50:50:3b:de:70:69:48:e4:2f:55:60:30:19:e5:28:ae
@@ -3326,124 +2776,14 @@
 2c9Si1vIY9RCPqAzekYu9wogRlR+ak8x8YF+QnQ4ZXMn7sZ8uI7XpTrXmKGcjBBV
 09tL7ECQ8s1uV9JiDnxXk7Gnbc2dg7sq5+W2O3FYrf3RRbxake5TFW/TRQl1brqQ
 XR4EzzffHqhmsYzmIGrv/EhOdJhCrylvLmrH+33RZjEizIYAfmaDDEL0vTSSwxrq
 T8p+ck0LcIymSLumoRT2+1hEmRSuqguTaaApJUqlyyvdimYHFngVV3Eb7PVHhPOe
 MTd61X8kreS8/f3MboPoDKi3QWwH3b08hpcv0g==
 -----END CERTIFICATE-----
 
-# Issuer: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-1"
-# Serial: 15752444095811006489
-# MD5 Fingerprint: 6e:85:f1:dc:1a:00:d3:22:d5:b2:b2:ac:6b:37:05:45
-# SHA1 Fingerprint: ff:bd:cd:e7:82:c8:43:5e:3c:6f:26:86:5c:ca:a8:3a:45:5b:c3:0a
-# SHA256 Fingerprint: d4:0e:9c:86:cd:8f:e4:68:c1:77:69:59:f4:9e:a7:74:fa:54:86:84:b6:c4:06:f3:90:92:61:f4:dc:e2:57:5c
------BEGIN CERTIFICATE-----
-MIIEMDCCAxigAwIBAgIJANqb7HHzA7AZMA0GCSqGSIb3DQEBCwUAMIGkMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRydXN0Q29y
-IFJvb3RDZXJ0IENBLTEwHhcNMTYwMjA0MTIzMjE2WhcNMjkxMjMxMTcyMzE2WjCB
-pDELMAkGA1UEBhMCUEExDzANBgNVBAgMBlBhbmFtYTEUMBIGA1UEBwwLUGFuYW1h
-IENpdHkxJDAiBgNVBAoMG1RydXN0Q29yIFN5c3RlbXMgUy4gZGUgUi5MLjEnMCUG
-A1UECwweVHJ1c3RDb3IgQ2VydGlmaWNhdGUgQXV0aG9yaXR5MR8wHQYDVQQDDBZU
-cnVzdENvciBSb290Q2VydCBDQS0xMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
-CgKCAQEAv463leLCJhJrMxnHQFgKq1mqjQCj/IDHUHuO1CAmujIS2CNUSSUQIpid
-RtLByZ5OGy4sDjjzGiVoHKZaBeYei0i/mJZ0PmnK6bV4pQa81QBeCQryJ3pS/C3V
-seq0iWEk8xoT26nPUu0MJLq5nux+AHT6k61sKZKuUbS701e/s/OojZz0JEsq1pme
-9J7+wH5COucLlVPat2gOkEz7cD+PSiyU8ybdY2mplNgQTsVHCJCZGxdNuWxu72CV
-EY4hgLW9oHPY0LJ3xEXqWib7ZnZ2+AYfYW0PVcWDtxBWcgYHpfOxGgMFZA6dWorW
-hnAbJN7+KIor0Gqw/Hqi3LJ5DotlDwIDAQABo2MwYTAdBgNVHQ4EFgQU7mtJPHo/
-DeOxCbeKyKsZn3MzUOcwHwYDVR0jBBgwFoAU7mtJPHo/DeOxCbeKyKsZn3MzUOcw
-DwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYwDQYJKoZIhvcNAQELBQAD
-ggEBACUY1JGPE+6PHh0RU9otRCkZoB5rMZ5NDp6tPVxBb5UrJKF5mDo4Nvu7Zp5I
-/5CQ7z3UuJu0h3U/IJvOcs+hVcFNZKIZBqEHMwwLKeXx6quj7LUKdJDHfXLy11yf
-ke+Ri7fc7Waiz45mO7yfOgLgJ90WmMCV1Aqk5IGadZQ1nJBfiDcGrVmVCrDRZ9MZ
-yonnMlo2HD6CqFqTvsbQZJG2z9m2GM/bftJlo6bEjhcxwft+dtvTheNYsnd6djts
-L1Ac59v2Z3kf9YKVmgenFK+P3CghZwnS1k1aHBkcjndcw5QkPTJrS37UeJSDvjdN
-zl/HHk484IkzlQsPpTLWPFp5LBk=
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor RootCert CA-2 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor RootCert CA-2"
-# Serial: 2711694510199101698
-# MD5 Fingerprint: a2:e1:f8:18:0b:ba:45:d5:c7:41:2a:bb:37:52:45:64
-# SHA1 Fingerprint: b8:be:6d:cb:56:f1:55:b9:63:d4:12:ca:4e:06:34:c7:94:b2:1c:c0
-# SHA256 Fingerprint: 07:53:e9:40:37:8c:1b:d5:e3:83:6e:39:5d:ae:a5:cb:83:9e:50:46:f1:bd:0e:ae:19:51:cf:10:fe:c7:c9:65
------BEGIN CERTIFICATE-----
-MIIGLzCCBBegAwIBAgIIJaHfyjPLWQIwDQYJKoZIhvcNAQELBQAwgaQxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEfMB0GA1UEAwwWVHJ1c3RDb3Ig
-Um9vdENlcnQgQ0EtMjAeFw0xNjAyMDQxMjMyMjNaFw0zNDEyMzExNzI2MzlaMIGk
-MQswCQYDVQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEg
-Q2l0eTEkMCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYD
-VQQLDB5UcnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxHzAdBgNVBAMMFlRy
-dXN0Q29yIFJvb3RDZXJ0IENBLTIwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIK
-AoICAQCnIG7CKqJiJJWQdsg4foDSq8GbZQWU9MEKENUCrO2fk8eHyLAnK0IMPQo+
-QVqedd2NyuCb7GgypGmSaIwLgQ5WoD4a3SwlFIIvl9NkRvRUqdw6VC0xK5mC8tkq
-1+9xALgxpL56JAfDQiDyitSSBBtlVkxs1Pu2YVpHI7TYabS3OtB0PAx1oYxOdqHp
-2yqlO/rOsP9+aij9JxzIsekp8VduZLTQwRVtDr4uDkbIXvRR/u8OYzo7cbrPb1nK
-DOObXUm4TOJXsZiKQlecdu/vvdFoqNL0Cbt3Nb4lggjEFixEIFapRBF37120Hape
-az6LMvYHL1cEksr1/p3C6eizjkxLAjHZ5DxIgif3GIJ2SDpxsROhOdUuxTTCHWKF
-3wP+TfSvPd9cW436cOGlfifHhi5qjxLGhF5DUVCcGZt45vz27Ud+ez1m7xMTiF88
-oWP7+ayHNZ/zgp6kPwqcMWmLmaSISo5uZk3vFsQPeSghYA2FFn3XVDjxklb9tTNM
-g9zXEJ9L/cb4Qr26fHMC4P99zVvh1Kxhe1fVSntb1IVYJ12/+CtgrKAmrhQhJ8Z3
-mjOAPF5GP/fDsaOGM8boXg25NSyqRsGFAnWAoOsk+xWq5Gd/bnc/9ASKL3x74xdh
-8N0JqSDIvgmk0H5Ew7IwSjiqqewYmgeCK9u4nBit2uBGF6zPXQIDAQABo2MwYTAd
-BgNVHQ4EFgQU2f4hQG6UnrybPZx9mCAZ5YwwYrIwHwYDVR0jBBgwFoAU2f4hQG6U
-nrybPZx9mCAZ5YwwYrIwDwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAYYw
-DQYJKoZIhvcNAQELBQADggIBAJ5Fngw7tu/hOsh80QA9z+LqBrWyOrsGS2h60COX
-dKcs8AjYeVrXWoSK2BKaG9l9XE1wxaX5q+WjiYndAfrs3fnpkpfbsEZC89NiqpX+
-MWcUaViQCqoL7jcjx1BRtPV+nuN79+TMQjItSQzL/0kMmx40/W5ulop5A7Zv2wnL
-/V9lFDfhOPXzYRZY5LVtDQsEGz9QLX+zx3oaFoBg+Iof6Rsqxvm6ARppv9JYx1RX
-CI/hOWB3S6xZhBqI8d3LT3jX5+EzLfzuQfogsL7L9ziUwOHQhQ+77Sxzq+3+knYa
-ZH9bDTMJBzN7Bj8RpFxwPIXAz+OQqIN3+tvmxYxoZxBnpVIt8MSZj3+/0WvitUfW
-2dCFmU2Umw9Lje4AWkcdEQOsQRivh7dvDDqPys/cA8GiCcjl/YBeyGBCARsaU1q7
-N6a3vLqE6R5sGtRk2tRD/pOLS/IseRYQ1JMLiI+h2IYURpFHmygk71dSTlxCnKr3
-Sewn6EAes6aJInKc9Q0ztFijMDvd1GpUk74aTfOTlPf8hAs/hCBcNANExdqtvArB
-As8e5ZTZ845b2EzwnexhF7sUMlQMAimTHpKG9n/v55IFDlndmQguLvqcAFLTxWYp
-5KeXRKQOKIETNcX2b2TmQcTVL8w0RSXPQQCWPUouwpaYT05KnJe32x+SMsj/D1Fu
-1uwJ
------END CERTIFICATE-----
-
-# Issuer: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Subject: CN=TrustCor ECA-1 O=TrustCor Systems S. de R.L. OU=TrustCor Certificate Authority
-# Label: "TrustCor ECA-1"
-# Serial: 9548242946988625984
-# MD5 Fingerprint: 27:92:23:1d:0a:f5:40:7c:e9:e6:6b:9d:d8:f5:e7:6c
-# SHA1 Fingerprint: 58:d1:df:95:95:67:6b:63:c0:f0:5b:1c:17:4d:8b:84:0b:c8:78:bd
-# SHA256 Fingerprint: 5a:88:5d:b1:9c:01:d9:12:c5:75:93:88:93:8c:af:bb:df:03:1a:b2:d4:8e:91:ee:15:58:9b:42:97:1d:03:9c
------BEGIN CERTIFICATE-----
-MIIEIDCCAwigAwIBAgIJAISCLF8cYtBAMA0GCSqGSIb3DQEBCwUAMIGcMQswCQYD
-VQQGEwJQQTEPMA0GA1UECAwGUGFuYW1hMRQwEgYDVQQHDAtQYW5hbWEgQ2l0eTEk
-MCIGA1UECgwbVHJ1c3RDb3IgU3lzdGVtcyBTLiBkZSBSLkwuMScwJQYDVQQLDB5U
-cnVzdENvciBDZXJ0aWZpY2F0ZSBBdXRob3JpdHkxFzAVBgNVBAMMDlRydXN0Q29y
-IEVDQS0xMB4XDTE2MDIwNDEyMzIzM1oXDTI5MTIzMTE3MjgwN1owgZwxCzAJBgNV
-BAYTAlBBMQ8wDQYDVQQIDAZQYW5hbWExFDASBgNVBAcMC1BhbmFtYSBDaXR5MSQw
-IgYDVQQKDBtUcnVzdENvciBTeXN0ZW1zIFMuIGRlIFIuTC4xJzAlBgNVBAsMHlRy
-dXN0Q29yIENlcnRpZmljYXRlIEF1dGhvcml0eTEXMBUGA1UEAwwOVHJ1c3RDb3Ig
-RUNBLTEwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDPj+ARtZ+odnbb
-3w9U73NjKYKtR8aja+3+XzP4Q1HpGjORMRegdMTUpwHmspI+ap3tDvl0mEDTPwOA
-BoJA6LHip1GnHYMma6ve+heRK9jGrB6xnhkB1Zem6g23xFUfJ3zSCNV2HykVh0A5
-3ThFEXXQmqc04L/NyFIduUd+Dbi7xgz2c1cWWn5DkR9VOsZtRASqnKmcp0yJF4Ou
-owReUoCLHhIlERnXDH19MURB6tuvsBzvgdAsxZohmz3tQjtQJvLsznFhBmIhVE5/
-wZ0+fyCMgMsq2JdiyIMzkX2woloPV+g7zPIlstR8L+xNxqE6FXrntl019fZISjZF
-ZtS6mFjBAgMBAAGjYzBhMB0GA1UdDgQWBBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAf
-BgNVHSMEGDAWgBREnkj1zG1I1KBLf/5ZJC+Dl5mahjAPBgNVHRMBAf8EBTADAQH/
-MA4GA1UdDwEB/wQEAwIBhjANBgkqhkiG9w0BAQsFAAOCAQEABT41XBVwm8nHc2Fv
-civUwo/yQ10CzsSUuZQRg2dd4mdsdXa/uwyqNsatR5Nj3B5+1t4u/ukZMjgDfxT2
-AHMsWbEhBuH7rBiVDKP/mZb3Kyeb1STMHd3BOuCYRLDE5D53sXOpZCz2HAF8P11F
-hcCF5yWPldwX8zyfGm6wyuMdKulMY/okYWLW2n62HGz1Ah3UKt1VkOsqEUc8Ll50
-soIipX1TH0XsJ5F95yIW6MBoNtjG8U+ARDL54dHRHareqKucBK+tIA5kmE2la8BI
-WJZpTdwHjFGTot+fDz2LYLSCjaoITmJF4PkL0uDgPFveXHEnJcLmA4GLEFPjx1Wi
-tJ/X5g==
------END CERTIFICATE-----
-
 # Issuer: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Subject: CN=SSL.com Root Certification Authority RSA O=SSL Corporation
 # Label: "SSL.com Root Certification Authority RSA"
 # Serial: 8875640296558310041
 # MD5 Fingerprint: 86:69:12:c0:70:f1:ec:ac:ac:c2:d5:bc:a5:5b:a1:29
 # SHA1 Fingerprint: b7:ab:33:08:d1:ea:44:77:ba:14:80:12:5a:6f:bd:a9:36:49:0c:bb
 # SHA256 Fingerprint: 85:66:6a:56:2e:e0:be:5c:e9:25:c1:d8:89:0a:6f:76:a8:7e:c1:6d:4d:7d:5f:29:ea:74:19:cf:20:12:3b:69
@@ -3631,134 +2971,14 @@
 p2OQ0jnUsYd4XxiWD1AbNTcPasbc2RNNpI6QN+a9WzGRo1QwUjAOBgNVHQ8BAf8E
 BAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUSIcUrOPDnpBgOtfKie7T
 rYy0UGYwEAYJKwYBBAGCNxUBBAMCAQAwCgYIKoZIzj0EAwMDaAAwZQIwJsdpW9zV
 57LnyAyMjMPdeYwbY9XJUpROTYJKcx6ygISpJcBMWm1JKWB4E+J+SOtkAjEA2zQg
 Mgj/mkkCtojeFK9dbJlxjRo/i9fgojaGHAeCOnZT/cKi7e97sIBPWA9LUzm9
 -----END CERTIFICATE-----
 
-# Issuer: CN=GTS Root R1 O=Google Trust Services LLC
-# Subject: CN=GTS Root R1 O=Google Trust Services LLC
-# Label: "GTS Root R1"
-# Serial: 146587175971765017618439757810265552097
-# MD5 Fingerprint: 82:1a:ef:d4:d2:4a:f2:9f:e2:3d:97:06:14:70:72:85
-# SHA1 Fingerprint: e1:c9:50:e6:ef:22:f8:4c:56:45:72:8b:92:20:60:d7:d5:a7:a3:e8
-# SHA256 Fingerprint: 2a:57:54:71:e3:13:40:bc:21:58:1c:bd:2c:f1:3e:15:84:63:20:3e:ce:94:bc:f9:d3:cc:19:6b:f0:9a:54:72
------BEGIN CERTIFICATE-----
-MIIFWjCCA0KgAwIBAgIQbkepxUtHDA3sM9CJuRz04TANBgkqhkiG9w0BAQwFADBH
-MQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExM
-QzEUMBIGA1UEAxMLR1RTIFJvb3QgUjEwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIy
-MDAwMDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNl
-cnZpY2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjEwggIiMA0GCSqGSIb3DQEB
-AQUAA4ICDwAwggIKAoICAQC2EQKLHuOhd5s73L+UPreVp0A8of2C+X0yBoJx9vaM
-f/vo27xqLpeXo4xL+Sv2sfnOhB2x+cWX3u+58qPpvBKJXqeqUqv4IyfLpLGcY9vX
-mX7wCl7raKb0xlpHDU0QM+NOsROjyBhsS+z8CZDfnWQpJSMHobTSPS5g4M/SCYe7
-zUjwTcLCeoiKu7rPWRnWr4+wB7CeMfGCwcDfLqZtbBkOtdh+JhpFAz2weaSUKK0P
-fyblqAj+lug8aJRT7oM6iCsVlgmy4HqMLnXWnOunVmSPlk9orj2XwoSPwLxAwAtc
-vfaHszVsrBhQf4TgTM2S0yDpM7xSma8ytSmzJSq0SPly4cpk9+aCEI3oncKKiPo4
-Zor8Y/kB+Xj9e1x3+naH+uzfsQ55lVe0vSbv1gHR6xYKu44LtcXFilWr06zqkUsp
-zBmkMiVOKvFlRNACzqrOSbTqn3yDsEB750Orp2yjj32JgfpMpf/VjsPOS+C12LOO
-Rc92wO1AK/1TD7Cn1TsNsYqiA94xrcx36m97PtbfkSIS5r762DL8EGMUUXLeXdYW
-k70paDPvOmbsB4om3xPXV2V4J95eSRQAogB/mqghtqmxlbCluQ0WEdrHbEg8QOB+
-DVrNVjzRlwW5y0vtOUucxD/SVRNuJLDWcfr0wbrM7Rv1/oFB2ACYPTrIrnqYNxgF
-lQIDAQABo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNV
-HQ4EFgQU5K8rJnEaK0gnhS9SZizv8IkTcT4wDQYJKoZIhvcNAQEMBQADggIBADiW
-Cu49tJYeX++dnAsznyvgyv3SjgofQXSlfKqE1OXyHuY3UjKcC9FhHb8owbZEKTV1
-d5iyfNm9dKyKaOOpMQkpAWBz40d8U6iQSifvS9efk+eCNs6aaAyC58/UEBZvXw6Z
-XPYfcX3v73svfuo21pdwCxXu11xWajOl40k4DLh9+42FpLFZXvRq4d2h9mREruZR
-gyFmxhE+885H7pwoHyXa/6xmld01D1zvICxi/ZG6qcz8WpyTgYMpl0p8WnK0OdC3
-d8t5/Wk6kjftbjhlRn7pYL15iJdfOBL07q9bgsiG1eGZbYwE8na6SfZu6W0eX6Dv
-J4J2QPim01hcDyxC2kLGe4g0x8HYRZvBPsVhHdljUEn2NIVq4BjFbkerQUIpm/Zg
-DdIx02OYI5NaAIFItO/Nis3Jz5nu2Z6qNuFoS3FJFDYoOj0dzpqPJeaAcWErtXvM
-+SUWgeExX6GjfhaknBZqlxi9dnKlC54dNuYvoS++cJEPqOba+MSSQGwlfnuzCdyy
-F62ARPBopY+Udf90WuioAnwMCeKpSwughQtiue+hMZL77/ZRBIls6Kl0obsXs7X9
-SQ98POyDGCBDTtWTurQ0sR8WNh8M5mQ5Fkzc4P4dyKliPUDqysU0ArSuiYgzNdws
-E3PYJ/HQcu51OyLemGhmW/HGY0dVHLqlCFF1pkgl
------END CERTIFICATE-----
-
-# Issuer: CN=GTS Root R2 O=Google Trust Services LLC
-# Subject: CN=GTS Root R2 O=Google Trust Services LLC
-# Label: "GTS Root R2"
-# Serial: 146587176055767053814479386953112547951
-# MD5 Fingerprint: 44:ed:9a:0e:a4:09:3b:00:f2:ae:4c:a3:c6:61:b0:8b
-# SHA1 Fingerprint: d2:73:96:2a:2a:5e:39:9f:73:3f:e1:c7:1e:64:3f:03:38:34:fc:4d
-# SHA256 Fingerprint: c4:5d:7b:b0:8e:6d:67:e6:2e:42:35:11:0b:56:4e:5f:78:fd:92:ef:05:8c:84:0a:ea:4e:64:55:d7:58:5c:60
------BEGIN CERTIFICATE-----
-MIIFWjCCA0KgAwIBAgIQbkepxlqz5yDFMJo/aFLybzANBgkqhkiG9w0BAQwFADBH
-MQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExM
-QzEUMBIGA1UEAxMLR1RTIFJvb3QgUjIwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIy
-MDAwMDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNl
-cnZpY2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjIwggIiMA0GCSqGSIb3DQEB
-AQUAA4ICDwAwggIKAoICAQDO3v2m++zsFDQ8BwZabFn3GTXd98GdVarTzTukk3Lv
-CvptnfbwhYBboUhSnznFt+4orO/LdmgUud+tAWyZH8QiHZ/+cnfgLFuv5AS/T3Kg
-GjSY6Dlo7JUle3ah5mm5hRm9iYz+re026nO8/4Piy33B0s5Ks40FnotJk9/BW9Bu
-XvAuMC6C/Pq8tBcKSOWIm8Wba96wyrQD8Nr0kLhlZPdcTK3ofmZemde4wj7I0BOd
-re7kRXuJVfeKH2JShBKzwkCX44ofR5GmdFrS+LFjKBC4swm4VndAoiaYecb+3yXu
-PuWgf9RhD1FLPD+M2uFwdNjCaKH5wQzpoeJ/u1U8dgbuak7MkogwTZq9TwtImoS1
-mKPV+3PBV2HdKFZ1E66HjucMUQkQdYhMvI35ezzUIkgfKtzra7tEscszcTJGr61K
-8YzodDqs5xoic4DSMPclQsciOzsSrZYuxsN2B6ogtzVJV+mSSeh2FnIxZyuWfoqj
-x5RWIr9qS34BIbIjMt/kmkRtWVtd9QCgHJvGeJeNkP+byKq0rxFROV7Z+2et1VsR
-nTKaG73VululycslaVNVJ1zgyjbLiGH7HrfQy+4W+9OmTN6SpdTi3/UGVN4unUu0
-kzCqgc7dGtxRcw1PcOnlthYhGXmy5okLdWTK1au8CcEYof/UVKGFPP0UJAOyh9Ok
-twIDAQABo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNV
-HQ4EFgQUu//KjiOfT5nK2+JopqUVJxce2Q4wDQYJKoZIhvcNAQEMBQADggIBALZp
-8KZ3/p7uC4Gt4cCpx/k1HUCCq+YEtN/L9x0Pg/B+E02NjO7jMyLDOfxA325BS0JT
-vhaI8dI4XsRomRyYUpOM52jtG2pzegVATX9lO9ZY8c6DR2Dj/5epnGB3GFW1fgiT
-z9D2PGcDFWEJ+YF59exTpJ/JjwGLc8R3dtyDovUMSRqodt6Sm2T4syzFJ9MHwAiA
-pJiS4wGWAqoC7o87xdFtCjMwc3i5T1QWvwsHoaRc5svJXISPD+AVdyx+Jn7axEvb
-pxZ3B7DNdehyQtaVhJ2Gg/LkkM0JR9SLA3DaWsYDQvTtN6LwG1BUSw7YhN4ZKJmB
-R64JGz9I0cNv4rBgF/XuIwKl2gBbbZCr7qLpGzvpx0QnRY5rn/WkhLx3+WuXrD5R
-RaIRpsyF7gpo8j5QOHokYh4XIDdtak23CZvJ/KRY9bb7nE4Yu5UC56GtmwfuNmsk
-0jmGwZODUNKBRqhfYlcsu2xkiAhu7xNUX90txGdj08+JN7+dIPT7eoOboB6BAFDC
-5AwiWVIQ7UNWhwD4FFKnHYuTjKJNRn8nxnGbJN7k2oaLDX5rIMHAnuFl2GqjpuiF
-izoHCBy69Y9Vmhh1fuXsgWbRIXOhNUQLgD1bnF5vKheW0YMjiGZt5obicDIvUiLn
-yOd/xCxgXS/Dr55FBcOEArf9LAhST4Ldo/DUhgkC
------END CERTIFICATE-----
-
-# Issuer: CN=GTS Root R3 O=Google Trust Services LLC
-# Subject: CN=GTS Root R3 O=Google Trust Services LLC
-# Label: "GTS Root R3"
-# Serial: 146587176140553309517047991083707763997
-# MD5 Fingerprint: 1a:79:5b:6b:04:52:9c:5d:c7:74:33:1b:25:9a:f9:25
-# SHA1 Fingerprint: 30:d4:24:6f:07:ff:db:91:89:8a:0b:e9:49:66:11:eb:8c:5e:46:e5
-# SHA256 Fingerprint: 15:d5:b8:77:46:19:ea:7d:54:ce:1c:a6:d0:b0:c4:03:e0:37:a9:17:f1:31:e8:a0:4e:1e:6b:7a:71:ba:bc:e5
------BEGIN CERTIFICATE-----
-MIICDDCCAZGgAwIBAgIQbkepx2ypcyRAiQ8DVd2NHTAKBggqhkjOPQQDAzBHMQsw
-CQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEU
-MBIGA1UEAxMLR1RTIFJvb3QgUjMwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAw
-MDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZp
-Y2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjMwdjAQBgcqhkjOPQIBBgUrgQQA
-IgNiAAQfTzOHMymKoYTey8chWEGJ6ladK0uFxh1MJ7x/JlFyb+Kf1qPKzEUURout
-736GjOyxfi//qXGdGIRFBEFVbivqJn+7kAHjSxm65FSWRQmx1WyRRK2EE46ajA2A
-DDL24CejQjBAMA4GA1UdDwEB/wQEAwIBBjAPBgNVHRMBAf8EBTADAQH/MB0GA1Ud
-DgQWBBTB8Sa6oC2uhYHP0/EqEr24Cmf9vDAKBggqhkjOPQQDAwNpADBmAjEAgFuk
-fCPAlaUs3L6JbyO5o91lAFJekazInXJ0glMLfalAvWhgxeG4VDvBNhcl2MG9AjEA
-njWSdIUlUfUk7GRSJFClH9voy8l27OyCbvWFGFPouOOaKaqW04MjyaR7YbPMAuhd
------END CERTIFICATE-----
-
-# Issuer: CN=GTS Root R4 O=Google Trust Services LLC
-# Subject: CN=GTS Root R4 O=Google Trust Services LLC
-# Label: "GTS Root R4"
-# Serial: 146587176229350439916519468929765261721
-# MD5 Fingerprint: 5d:b6:6a:c4:60:17:24:6a:1a:99:a8:4b:ee:5e:b4:26
-# SHA1 Fingerprint: 2a:1d:60:27:d9:4a:b1:0a:1c:4d:91:5c:cd:33:a0:cb:3e:2d:54:cb
-# SHA256 Fingerprint: 71:cc:a5:39:1f:9e:79:4b:04:80:25:30:b3:63:e1:21:da:8a:30:43:bb:26:66:2f:ea:4d:ca:7f:c9:51:a4:bd
------BEGIN CERTIFICATE-----
-MIICCjCCAZGgAwIBAgIQbkepyIuUtui7OyrYorLBmTAKBggqhkjOPQQDAzBHMQsw
-CQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEU
-MBIGA1UEAxMLR1RTIFJvb3QgUjQwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAw
-MDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZp
-Y2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjQwdjAQBgcqhkjOPQIBBgUrgQQA
-IgNiAATzdHOnaItgrkO4NcWBMHtLSZ37wWHO5t5GvWvVYRg1rkDdc/eJkTBa6zzu
-hXyiQHY7qca4R9gq55KRanPpsXI5nymfopjTX15YhmUPoYRlBtHci8nHc8iMai/l
-xKvRHYqjQjBAMA4GA1UdDwEB/wQEAwIBBjAPBgNVHRMBAf8EBTADAQH/MB0GA1Ud
-DgQWBBSATNbrdP9JNqPV2Py1PsVq8JQdjDAKBggqhkjOPQQDAwNnADBkAjBqUFJ0
-CMRw3J5QdCHojXohw0+WbhXRIjVhLfoIN+4Zba3bssx9BzT1YBkstTTZbyACMANx
-sbqjYAuG7ZoIapVon+Kz4ZNkfF6Tpt95LY2F45TPI11xzPKwTdb+mciUqXWi4w==
------END CERTIFICATE-----
-
 # Issuer: CN=UCA Global G2 Root O=UniTrust
 # Subject: CN=UCA Global G2 Root O=UniTrust
 # Label: "UCA Global G2 Root"
 # Serial: 124779693093741543919145257850076631279
 # MD5 Fingerprint: 80:fe:f0:c4:4a:f0:5c:62:32:9f:1c:ba:78:a9:50:f8
 # SHA1 Fingerprint: 28:f9:78:16:19:7a:ff:18:25:18:aa:44:fe:c1:a0:ce:5c:b6:4c:8a
 # SHA256 Fingerprint: 9b:ea:11:c9:76:fe:01:47:64:c1:be:56:a6:f9:14:b5:a5:60:31:7a:bd:99:88:39:33:82:e5:16:1a:a0:49:3c
@@ -4319,7 +3539,1051 @@
 p/8Dvq1wkNoL3chtl1+afwkyQf3NosxabUzyqkn+Zvjp2DXrDige7kgvOtB5CTh8
 piKCk5XQA76+AqAF3SAi428diDRgxuYKuQl1C/AH6GmWNcf7I4GOODm4RStDeKLR
 LBT/DShycpWbXgnbiUSYqqFJu3FS8r/2/yehNq+4tneI3TqkbZs0kNwUXTC/t+sX
 5Ie3cdCh13cV1ELX8vMxmV2b3RZtP+oGI/hGoiLtk/bdmuYqh7GYVPEi92tF4+KO
 dh2ajcQGjTa3FPOdVGm3jjzVpG2Tgbet9r1ke8LJaDmgkpzNNIaRkPpkUZ3+/uul
 9XXeifdy
 -----END CERTIFICATE-----
+
+# Issuer: CN=AC RAIZ FNMT-RCM SERVIDORES SEGUROS O=FNMT-RCM OU=Ceres
+# Subject: CN=AC RAIZ FNMT-RCM SERVIDORES SEGUROS O=FNMT-RCM OU=Ceres
+# Label: "AC RAIZ FNMT-RCM SERVIDORES SEGUROS"
+# Serial: 131542671362353147877283741781055151509
+# MD5 Fingerprint: 19:36:9c:52:03:2f:d2:d1:bb:23:cc:dd:1e:12:55:bb
+# SHA1 Fingerprint: 62:ff:d9:9e:c0:65:0d:03:ce:75:93:d2:ed:3f:2d:32:c9:e3:e5:4a
+# SHA256 Fingerprint: 55:41:53:b1:3d:2c:f9:dd:b7:53:bf:be:1a:4e:0a:e0:8d:0a:a4:18:70:58:fe:60:a2:b8:62:b2:e4:b8:7b:cb
+-----BEGIN CERTIFICATE-----
+MIICbjCCAfOgAwIBAgIQYvYybOXE42hcG2LdnC6dlTAKBggqhkjOPQQDAzB4MQsw
+CQYDVQQGEwJFUzERMA8GA1UECgwIRk5NVC1SQ00xDjAMBgNVBAsMBUNlcmVzMRgw
+FgYDVQRhDA9WQVRFUy1RMjgyNjAwNEoxLDAqBgNVBAMMI0FDIFJBSVogRk5NVC1S
+Q00gU0VSVklET1JFUyBTRUdVUk9TMB4XDTE4MTIyMDA5MzczM1oXDTQzMTIyMDA5
+MzczM1oweDELMAkGA1UEBhMCRVMxETAPBgNVBAoMCEZOTVQtUkNNMQ4wDAYDVQQL
+DAVDZXJlczEYMBYGA1UEYQwPVkFURVMtUTI4MjYwMDRKMSwwKgYDVQQDDCNBQyBS
+QUlaIEZOTVQtUkNNIFNFUlZJRE9SRVMgU0VHVVJPUzB2MBAGByqGSM49AgEGBSuB
+BAAiA2IABPa6V1PIyqvfNkpSIeSX0oNnnvBlUdBeh8dHsVnyV0ebAAKTRBdp20LH
+sbI6GA60XYyzZl2hNPk2LEnb80b8s0RpRBNm/dfF/a82Tc4DTQdxz69qBdKiQ1oK
+Um8BA06Oi6NCMEAwDwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAQYwHQYD
+VR0OBBYEFAG5L++/EYZg8k/QQW6rcx/n0m5JMAoGCCqGSM49BAMDA2kAMGYCMQCu
+SuMrQMN0EfKVrRYj3k4MGuZdpSRea0R7/DjiT8ucRRcRTBQnJlU5dUoDzBOQn5IC
+MQD6SmxgiHPz7riYYqnOK8LZiqZwMR2vsJRM60/G49HzYqc8/5MuB1xJAWdpEgJy
+v+c=
+-----END CERTIFICATE-----
+
+# Issuer: CN=GlobalSign Root R46 O=GlobalSign nv-sa
+# Subject: CN=GlobalSign Root R46 O=GlobalSign nv-sa
+# Label: "GlobalSign Root R46"
+# Serial: 1552617688466950547958867513931858518042577
+# MD5 Fingerprint: c4:14:30:e4:fa:66:43:94:2a:6a:1b:24:5f:19:d0:ef
+# SHA1 Fingerprint: 53:a2:b0:4b:ca:6b:d6:45:e6:39:8a:8e:c4:0d:d2:bf:77:c3:a2:90
+# SHA256 Fingerprint: 4f:a3:12:6d:8d:3a:11:d1:c4:85:5a:4f:80:7c:ba:d6:cf:91:9d:3a:5a:88:b0:3b:ea:2c:63:72:d9:3c:40:c9
+-----BEGIN CERTIFICATE-----
+MIIFWjCCA0KgAwIBAgISEdK7udcjGJ5AXwqdLdDfJWfRMA0GCSqGSIb3DQEBDAUA
+MEYxCzAJBgNVBAYTAkJFMRkwFwYDVQQKExBHbG9iYWxTaWduIG52LXNhMRwwGgYD
+VQQDExNHbG9iYWxTaWduIFJvb3QgUjQ2MB4XDTE5MDMyMDAwMDAwMFoXDTQ2MDMy
+MDAwMDAwMFowRjELMAkGA1UEBhMCQkUxGTAXBgNVBAoTEEdsb2JhbFNpZ24gbnYt
+c2ExHDAaBgNVBAMTE0dsb2JhbFNpZ24gUm9vdCBSNDYwggIiMA0GCSqGSIb3DQEB
+AQUAA4ICDwAwggIKAoICAQCsrHQy6LNl5brtQyYdpokNRbopiLKkHWPd08EsCVeJ
+OaFV6Wc0dwxu5FUdUiXSE2te4R2pt32JMl8Nnp8semNgQB+msLZ4j5lUlghYruQG
+vGIFAha/r6gjA7aUD7xubMLL1aa7DOn2wQL7Id5m3RerdELv8HQvJfTqa1VbkNud
+316HCkD7rRlr+/fKYIje2sGP1q7Vf9Q8g+7XFkyDRTNrJ9CG0Bwta/OrffGFqfUo
+0q3v84RLHIf8E6M6cqJaESvWJ3En7YEtbWaBkoe0G1h6zD8K+kZPTXhc+CtI4wSE
+y132tGqzZfxCnlEmIyDLPRT5ge1lFgBPGmSXZgjPjHvjK8Cd+RTyG/FWaha/LIWF
+zXg4mutCagI0GIMXTpRW+LaCtfOW3T3zvn8gdz57GSNrLNRyc0NXfeD412lPFzYE
++cCQYDdF3uYM2HSNrpyibXRdQr4G9dlkbgIQrImwTDsHTUB+JMWKmIJ5jqSngiCN
+I/onccnfxkF0oE32kRbcRoxfKWMxWXEM2G/CtjJ9++ZdU6Z+Ffy7dXxd7Pj2Fxzs
+x2sZy/N78CsHpdlseVR2bJ0cpm4O6XkMqCNqo98bMDGfsVR7/mrLZqrcZdCinkqa
+ByFrgY/bxFn63iLABJzjqls2k+g9vXqhnQt2sQvHnf3PmKgGwvgqo6GDoLclcqUC
+4wIDAQABo0IwQDAOBgNVHQ8BAf8EBAMCAYYwDwYDVR0TAQH/BAUwAwEB/zAdBgNV
+HQ4EFgQUA1yrc4GHqMywptWU4jaWSf8FmSwwDQYJKoZIhvcNAQEMBQADggIBAHx4
+7PYCLLtbfpIrXTncvtgdokIzTfnvpCo7RGkerNlFo048p9gkUbJUHJNOxO97k4Vg
+JuoJSOD1u8fpaNK7ajFxzHmuEajwmf3lH7wvqMxX63bEIaZHU1VNaL8FpO7XJqti
+2kM3S+LGteWygxk6x9PbTZ4IevPuzz5i+6zoYMzRx6Fcg0XERczzF2sUyQQCPtIk
+pnnpHs6i58FZFZ8d4kuaPp92CC1r2LpXFNqD6v6MVenQTqnMdzGxRBF6XLE+0xRF
+FRhiJBPSy03OXIPBNvIQtQ6IbbjhVp+J3pZmOUdkLG5NrmJ7v2B0GbhWrJKsFjLt
+rWhV/pi60zTe9Mlhww6G9kuEYO4Ne7UyWHmRVSyBQ7N0H3qqJZ4d16GLuc1CLgSk
+ZoNNiTW2bKg2SnkheCLQQrzRQDGQob4Ez8pn7fXwgNNgyYMqIgXQBztSvwyeqiv5
+u+YfjyW6hY0XHgL+XVAEV8/+LbzvXMAaq7afJMbfc2hIkCwU9D9SGuTSyxTDYWnP
+4vkYxboznxSjBF25cfe1lNj2M8FawTSLfJvdkzrnE6JwYZ+vj+vYxXX4M2bUdGc6
+N3ec592kD3ZDZopD8p/7DEJ4Y9HiD2971KE9dJeFt0g5QdYg/NA6s/rob8SKunE3
+vouXsXgxT7PntgMTzlSdriVZzH81Xwj3QEUxeCp6
+-----END CERTIFICATE-----
+
+# Issuer: CN=GlobalSign Root E46 O=GlobalSign nv-sa
+# Subject: CN=GlobalSign Root E46 O=GlobalSign nv-sa
+# Label: "GlobalSign Root E46"
+# Serial: 1552617690338932563915843282459653771421763
+# MD5 Fingerprint: b5:b8:66:ed:de:08:83:e3:c9:e2:01:34:06:ac:51:6f
+# SHA1 Fingerprint: 39:b4:6c:d5:fe:80:06:eb:e2:2f:4a:bb:08:33:a0:af:db:b9:dd:84
+# SHA256 Fingerprint: cb:b9:c4:4d:84:b8:04:3e:10:50:ea:31:a6:9f:51:49:55:d7:bf:d2:e2:c6:b4:93:01:01:9a:d6:1d:9f:50:58
+-----BEGIN CERTIFICATE-----
+MIICCzCCAZGgAwIBAgISEdK7ujNu1LzmJGjFDYQdmOhDMAoGCCqGSM49BAMDMEYx
+CzAJBgNVBAYTAkJFMRkwFwYDVQQKExBHbG9iYWxTaWduIG52LXNhMRwwGgYDVQQD
+ExNHbG9iYWxTaWduIFJvb3QgRTQ2MB4XDTE5MDMyMDAwMDAwMFoXDTQ2MDMyMDAw
+MDAwMFowRjELMAkGA1UEBhMCQkUxGTAXBgNVBAoTEEdsb2JhbFNpZ24gbnYtc2Ex
+HDAaBgNVBAMTE0dsb2JhbFNpZ24gUm9vdCBFNDYwdjAQBgcqhkjOPQIBBgUrgQQA
+IgNiAAScDrHPt+ieUnd1NPqlRqetMhkytAepJ8qUuwzSChDH2omwlwxwEwkBjtjq
+R+q+soArzfwoDdusvKSGN+1wCAB16pMLey5SnCNoIwZD7JIvU4Tb+0cUB+hflGdd
+yXqBPCCjQjBAMA4GA1UdDwEB/wQEAwIBhjAPBgNVHRMBAf8EBTADAQH/MB0GA1Ud
+DgQWBBQxCpCPtsad0kRLgLWi5h+xEk8blTAKBggqhkjOPQQDAwNoADBlAjEA31SQ
+7Zvvi5QCkxeCmb6zniz2C5GMn0oUsfZkvLtoURMMA/cVi4RguYv/Uo7njLwcAjA8
++RHUjE7AwWHCFUyqqx0LMV87HOIAl0Qx5v5zli/altP+CAezNIm8BZ/3Hobui3A=
+-----END CERTIFICATE-----
+
+# Issuer: CN=GLOBALTRUST 2020 O=e-commerce monitoring GmbH
+# Subject: CN=GLOBALTRUST 2020 O=e-commerce monitoring GmbH
+# Label: "GLOBALTRUST 2020"
+# Serial: 109160994242082918454945253
+# MD5 Fingerprint: 8a:c7:6f:cb:6d:e3:cc:a2:f1:7c:83:fa:0e:78:d7:e8
+# SHA1 Fingerprint: d0:67:c1:13:51:01:0c:aa:d0:c7:6a:65:37:31:16:26:4f:53:71:a2
+# SHA256 Fingerprint: 9a:29:6a:51:82:d1:d4:51:a2:e3:7f:43:9b:74:da:af:a2:67:52:33:29:f9:0f:9a:0d:20:07:c3:34:e2:3c:9a
+-----BEGIN CERTIFICATE-----
+MIIFgjCCA2qgAwIBAgILWku9WvtPilv6ZeUwDQYJKoZIhvcNAQELBQAwTTELMAkG
+A1UEBhMCQVQxIzAhBgNVBAoTGmUtY29tbWVyY2UgbW9uaXRvcmluZyBHbWJIMRkw
+FwYDVQQDExBHTE9CQUxUUlVTVCAyMDIwMB4XDTIwMDIxMDAwMDAwMFoXDTQwMDYx
+MDAwMDAwMFowTTELMAkGA1UEBhMCQVQxIzAhBgNVBAoTGmUtY29tbWVyY2UgbW9u
+aXRvcmluZyBHbWJIMRkwFwYDVQQDExBHTE9CQUxUUlVTVCAyMDIwMIICIjANBgkq
+hkiG9w0BAQEFAAOCAg8AMIICCgKCAgEAri5WrRsc7/aVj6B3GyvTY4+ETUWiD59b
+RatZe1E0+eyLinjF3WuvvcTfk0Uev5E4C64OFudBc/jbu9G4UeDLgztzOG53ig9Z
+YybNpyrOVPu44sB8R85gfD+yc/LAGbaKkoc1DZAoouQVBGM+uq/ufF7MpotQsjj3
+QWPKzv9pj2gOlTblzLmMCcpL3TGQlsjMH/1WljTbjhzqLL6FLmPdqqmV0/0plRPw
+yJiT2S0WR5ARg6I6IqIoV6Lr/sCMKKCmfecqQjuCgGOlYx8ZzHyyZqjC0203b+J+
+BlHZRYQfEs4kUmSFC0iAToexIiIwquuuvuAC4EDosEKAA1GqtH6qRNdDYfOiaxaJ
+SaSjpCuKAsR49GiKweR6NrFvG5Ybd0mN1MkGco/PU+PcF4UgStyYJ9ORJitHHmkH
+r96i5OTUawuzXnzUJIBHKWk7buis/UDr2O1xcSvy6Fgd60GXIsUf1DnQJ4+H4xj0
+4KlGDfV0OoIu0G4skaMxXDtG6nsEEFZegB31pWXogvziB4xiRfUg3kZwhqG8k9Me
+dKZssCz3AwyIDMvUclOGvGBG85hqwvG/Q/lwIHfKN0F5VVJjjVsSn8VoxIidrPIw
+q7ejMZdnrY8XD2zHc+0klGvIg5rQmjdJBKuxFshsSUktq6HQjJLyQUp5ISXbY9e2
+nKd+Qmn7OmMCAwEAAaNjMGEwDwYDVR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMC
+AQYwHQYDVR0OBBYEFNwuH9FhN3nkq9XVsxJxaD1qaJwiMB8GA1UdIwQYMBaAFNwu
+H9FhN3nkq9XVsxJxaD1qaJwiMA0GCSqGSIb3DQEBCwUAA4ICAQCR8EICaEDuw2jA
+VC/f7GLDw56KoDEoqoOOpFaWEhCGVrqXctJUMHytGdUdaG/7FELYjQ7ztdGl4wJC
+XtzoRlgHNQIw4Lx0SsFDKv/bGtCwr2zD/cuz9X9tAy5ZVp0tLTWMstZDFyySCstd
+6IwPS3BD0IL/qMy/pJTAvoe9iuOTe8aPmxadJ2W8esVCgmxcB9CpwYhgROmYhRZf
++I/KARDOJcP5YBugxZfD0yyIMaK9MOzQ0MAS8cE54+X1+NZK3TTN+2/BT+MAi1bi
+kvcoskJ3ciNnxz8RFbLEAwW+uxF7Cr+obuf/WEPPm2eggAe2HcqtbepBEX4tdJP7
+wry+UUTF72glJ4DjyKDUEuzZpTcdN3y0kcra1LGWge9oXHYQSa9+pTeAsRxSvTOB
+TI/53WXZFM2KJVj04sWDpQmQ1GwUY7VA3+vA/MRYfg0UFodUJ25W5HCEuGwyEn6C
+MUO+1918oa2u1qsgEu8KwxCMSZY13At1XrFP1U80DhEgB3VDRemjEdqso5nCtnkn
+4rnvyOL2NSl6dPrFf4IFYqYK6miyeUcGbvJXqBUzxvd4Sj1Ce2t+/vdG6tHrju+I
+aFvowdlxfv1k7/9nR4hYJS8+hge9+6jlgqispdNpQ80xiEmEU5LAsTkbOYMBMMTy
+qfrQA71yN2BWHzZ8vTmR9W0Nv3vXkg==
+-----END CERTIFICATE-----
+
+# Issuer: CN=ANF Secure Server Root CA O=ANF Autoridad de Certificacion OU=ANF CA Raiz
+# Subject: CN=ANF Secure Server Root CA O=ANF Autoridad de Certificacion OU=ANF CA Raiz
+# Label: "ANF Secure Server Root CA"
+# Serial: 996390341000653745
+# MD5 Fingerprint: 26:a6:44:5a:d9:af:4e:2f:b2:1d:b6:65:b0:4e:e8:96
+# SHA1 Fingerprint: 5b:6e:68:d0:cc:15:b6:a0:5f:1e:c1:5f:ae:02:fc:6b:2f:5d:6f:74
+# SHA256 Fingerprint: fb:8f:ec:75:91:69:b9:10:6b:1e:51:16:44:c6:18:c5:13:04:37:3f:6c:06:43:08:8d:8b:ef:fd:1b:99:75:99
+-----BEGIN CERTIFICATE-----
+MIIF7zCCA9egAwIBAgIIDdPjvGz5a7EwDQYJKoZIhvcNAQELBQAwgYQxEjAQBgNV
+BAUTCUc2MzI4NzUxMDELMAkGA1UEBhMCRVMxJzAlBgNVBAoTHkFORiBBdXRvcmlk
+YWQgZGUgQ2VydGlmaWNhY2lvbjEUMBIGA1UECxMLQU5GIENBIFJhaXoxIjAgBgNV
+BAMTGUFORiBTZWN1cmUgU2VydmVyIFJvb3QgQ0EwHhcNMTkwOTA0MTAwMDM4WhcN
+MzkwODMwMTAwMDM4WjCBhDESMBAGA1UEBRMJRzYzMjg3NTEwMQswCQYDVQQGEwJF
+UzEnMCUGA1UEChMeQU5GIEF1dG9yaWRhZCBkZSBDZXJ0aWZpY2FjaW9uMRQwEgYD
+VQQLEwtBTkYgQ0EgUmFpejEiMCAGA1UEAxMZQU5GIFNlY3VyZSBTZXJ2ZXIgUm9v
+dCBDQTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBANvrayvmZFSVgpCj
+cqQZAZ2cC4Ffc0m6p6zzBE57lgvsEeBbphzOG9INgxwruJ4dfkUyYA8H6XdYfp9q
+yGFOtibBTI3/TO80sh9l2Ll49a2pcbnvT1gdpd50IJeh7WhM3pIXS7yr/2WanvtH
+2Vdy8wmhrnZEE26cLUQ5vPnHO6RYPUG9tMJJo8gN0pcvB2VSAKduyK9o7PQUlrZX
+H1bDOZ8rbeTzPvY1ZNoMHKGESy9LS+IsJJ1tk0DrtSOOMspvRdOoiXsezx76W0OL
+zc2oD2rKDF65nkeP8Nm2CgtYZRczuSPkdxl9y0oukntPLxB3sY0vaJxizOBQ+OyR
+p1RMVwnVdmPF6GUe7m1qzwmd+nxPrWAI/VaZDxUse6mAq4xhj0oHdkLePfTdsiQz
+W7i1o0TJrH93PB0j7IKppuLIBkwC/qxcmZkLLxCKpvR/1Yd0DVlJRfbwcVw5Kda/
+SiOL9V8BY9KHcyi1Swr1+KuCLH5zJTIdC2MKF4EA/7Z2Xue0sUDKIbvVgFHlSFJn
+LNJhiQcND85Cd8BEc5xEUKDbEAotlRyBr+Qc5RQe8TZBAQIvfXOn3kLMTOmJDVb3
+n5HUA8ZsyY/b2BzgQJhdZpmYgG4t/wHFzstGH6wCxkPmrqKEPMVOHj1tyRRM4y5B
+u8o5vzY8KhmqQYdOpc5LMnndkEl/AgMBAAGjYzBhMB8GA1UdIwQYMBaAFJxf0Gxj
+o1+TypOYCK2Mh6UsXME3MB0GA1UdDgQWBBScX9BsY6Nfk8qTmAitjIelLFzBNzAO
+BgNVHQ8BAf8EBAMCAYYwDwYDVR0TAQH/BAUwAwEB/zANBgkqhkiG9w0BAQsFAAOC
+AgEATh65isagmD9uw2nAalxJUqzLK114OMHVVISfk/CHGT0sZonrDUL8zPB1hT+L
+9IBdeeUXZ701guLyPI59WzbLWoAAKfLOKyzxj6ptBZNscsdW699QIyjlRRA96Gej
+rw5VD5AJYu9LWaL2U/HANeQvwSS9eS9OICI7/RogsKQOLHDtdD+4E5UGUcjohybK
+pFtqFiGS3XNgnhAY3jyB6ugYw3yJ8otQPr0R4hUDqDZ9MwFsSBXXiJCZBMXM5gf0
+vPSQ7RPi6ovDj6MzD8EpTBNO2hVWcXNyglD2mjN8orGoGjR0ZVzO0eurU+AagNjq
+OknkJjCb5RyKqKkVMoaZkgoQI1YS4PbOTOK7vtuNknMBZi9iPrJyJ0U27U1W45eZ
+/zo1PqVUSlJZS2Db7v54EX9K3BR5YLZrZAPbFYPhor72I5dQ8AkzNqdxliXzuUJ9
+2zg/LFis6ELhDtjTO0wugumDLmsx2d1Hhk9tl5EuT+IocTUW0fJz/iUrB0ckYyfI
++PbZa/wSMVYIwFNCr5zQM378BvAxRAMU8Vjq8moNqRGyg77FGr8H6lnco4g175x2
+MjxNBiLOFeXdntiP2t7SxDnlF4HPOEfrf4htWRvfn0IUrn7PqLBmZdo3r5+qPeoo
+tt7VMVgWglvquxl1AnMaykgaIZOQCo6ThKd9OyMYkomgjaw=
+-----END CERTIFICATE-----
+
+# Issuer: CN=Certum EC-384 CA O=Asseco Data Systems S.A. OU=Certum Certification Authority
+# Subject: CN=Certum EC-384 CA O=Asseco Data Systems S.A. OU=Certum Certification Authority
+# Label: "Certum EC-384 CA"
+# Serial: 160250656287871593594747141429395092468
+# MD5 Fingerprint: b6:65:b3:96:60:97:12:a1:ec:4e:e1:3d:a3:c6:c9:f1
+# SHA1 Fingerprint: f3:3e:78:3c:ac:df:f4:a2:cc:ac:67:55:69:56:d7:e5:16:3c:e1:ed
+# SHA256 Fingerprint: 6b:32:80:85:62:53:18:aa:50:d1:73:c9:8d:8b:da:09:d5:7e:27:41:3d:11:4c:f7:87:a0:f5:d0:6c:03:0c:f6
+-----BEGIN CERTIFICATE-----
+MIICZTCCAeugAwIBAgIQeI8nXIESUiClBNAt3bpz9DAKBggqhkjOPQQDAzB0MQsw
+CQYDVQQGEwJQTDEhMB8GA1UEChMYQXNzZWNvIERhdGEgU3lzdGVtcyBTLkEuMScw
+JQYDVQQLEx5DZXJ0dW0gQ2VydGlmaWNhdGlvbiBBdXRob3JpdHkxGTAXBgNVBAMT
+EENlcnR1bSBFQy0zODQgQ0EwHhcNMTgwMzI2MDcyNDU0WhcNNDMwMzI2MDcyNDU0
+WjB0MQswCQYDVQQGEwJQTDEhMB8GA1UEChMYQXNzZWNvIERhdGEgU3lzdGVtcyBT
+LkEuMScwJQYDVQQLEx5DZXJ0dW0gQ2VydGlmaWNhdGlvbiBBdXRob3JpdHkxGTAX
+BgNVBAMTEENlcnR1bSBFQy0zODQgQ0EwdjAQBgcqhkjOPQIBBgUrgQQAIgNiAATE
+KI6rGFtqvm5kN2PkzeyrOvfMobgOgknXhimfoZTy42B4mIF4Bk3y7JoOV2CDn7Tm
+Fy8as10CW4kjPMIRBSqniBMY81CE1700LCeJVf/OTOffph8oxPBUw7l8t1Ot68Kj
+QjBAMA8GA1UdEwEB/wQFMAMBAf8wHQYDVR0OBBYEFI0GZnQkdjrzife81r1HfS+8
+EF9LMA4GA1UdDwEB/wQEAwIBBjAKBggqhkjOPQQDAwNoADBlAjADVS2m5hjEfO/J
+UG7BJw+ch69u1RsIGL2SKcHvlJF40jocVYli5RsJHrpka/F2tNQCMQC0QoSZ/6vn
+nvuRlydd3LBbMHHOXjgaatkl5+r3YZJW+OraNsKHZZYuciUvf9/DE8k=
+-----END CERTIFICATE-----
+
+# Issuer: CN=Certum Trusted Root CA O=Asseco Data Systems S.A. OU=Certum Certification Authority
+# Subject: CN=Certum Trusted Root CA O=Asseco Data Systems S.A. OU=Certum Certification Authority
+# Label: "Certum Trusted Root CA"
+# Serial: 40870380103424195783807378461123655149
+# MD5 Fingerprint: 51:e1:c2:e7:fe:4c:84:af:59:0e:2f:f4:54:6f:ea:29
+# SHA1 Fingerprint: c8:83:44:c0:18:ae:9f:cc:f1:87:b7:8f:22:d1:c5:d7:45:84:ba:e5
+# SHA256 Fingerprint: fe:76:96:57:38:55:77:3e:37:a9:5e:7a:d4:d9:cc:96:c3:01:57:c1:5d:31:76:5b:a9:b1:57:04:e1:ae:78:fd
+-----BEGIN CERTIFICATE-----
+MIIFwDCCA6igAwIBAgIQHr9ZULjJgDdMBvfrVU+17TANBgkqhkiG9w0BAQ0FADB6
+MQswCQYDVQQGEwJQTDEhMB8GA1UEChMYQXNzZWNvIERhdGEgU3lzdGVtcyBTLkEu
+MScwJQYDVQQLEx5DZXJ0dW0gQ2VydGlmaWNhdGlvbiBBdXRob3JpdHkxHzAdBgNV
+BAMTFkNlcnR1bSBUcnVzdGVkIFJvb3QgQ0EwHhcNMTgwMzE2MTIxMDEzWhcNNDMw
+MzE2MTIxMDEzWjB6MQswCQYDVQQGEwJQTDEhMB8GA1UEChMYQXNzZWNvIERhdGEg
+U3lzdGVtcyBTLkEuMScwJQYDVQQLEx5DZXJ0dW0gQ2VydGlmaWNhdGlvbiBBdXRo
+b3JpdHkxHzAdBgNVBAMTFkNlcnR1bSBUcnVzdGVkIFJvb3QgQ0EwggIiMA0GCSqG
+SIb3DQEBAQUAA4ICDwAwggIKAoICAQDRLY67tzbqbTeRn06TpwXkKQMlzhyC93yZ
+n0EGze2jusDbCSzBfN8pfktlL5On1AFrAygYo9idBcEq2EXxkd7fO9CAAozPOA/q
+p1x4EaTByIVcJdPTsuclzxFUl6s1wB52HO8AU5853BSlLCIls3Jy/I2z5T4IHhQq
+NwuIPMqw9MjCoa68wb4pZ1Xi/K1ZXP69VyywkI3C7Te2fJmItdUDmj0VDT06qKhF
+8JVOJVkdzZhpu9PMMsmN74H+rX2Ju7pgE8pllWeg8xn2A1bUatMn4qGtg/BKEiJ3
+HAVz4hlxQsDsdUaakFjgao4rpUYwBI4Zshfjvqm6f1bxJAPXsiEodg42MEx51UGa
+mqi4NboMOvJEGyCI98Ul1z3G4z5D3Yf+xOr1Uz5MZf87Sst4WmsXXw3Hw09Omiqi
+7VdNIuJGmj8PkTQkfVXjjJU30xrwCSss0smNtA0Aq2cpKNgB9RkEth2+dv5yXMSF
+ytKAQd8FqKPVhJBPC/PgP5sZ0jeJP/J7UhyM9uH3PAeXjA6iWYEMspA90+NZRu0P
+qafegGtaqge2Gcu8V/OXIXoMsSt0Puvap2ctTMSYnjYJdmZm/Bo/6khUHL4wvYBQ
+v3y1zgD2DGHZ5yQD4OMBgQ692IU0iL2yNqh7XAjlRICMb/gv1SHKHRzQ+8S1h9E6
+Tsd2tTVItQIDAQABo0IwQDAPBgNVHRMBAf8EBTADAQH/MB0GA1UdDgQWBBSM+xx1
+vALTn04uSNn5YFSqxLNP+jAOBgNVHQ8BAf8EBAMCAQYwDQYJKoZIhvcNAQENBQAD
+ggIBAEii1QALLtA/vBzVtVRJHlpr9OTy4EA34MwUe7nJ+jW1dReTagVphZzNTxl4
+WxmB82M+w85bj/UvXgF2Ez8sALnNllI5SW0ETsXpD4YN4fqzX4IS8TrOZgYkNCvo
+zMrnadyHncI013nR03e4qllY/p0m+jiGPp2Kh2RX5Rc64vmNueMzeMGQ2Ljdt4NR
+5MTMI9UGfOZR0800McD2RrsLrfw9EAUqO0qRJe6M1ISHgCq8CYyqOhNf6DR5UMEQ
+GfnTKB7U0VEwKbOukGfWHwpjscWpxkIxYxeU72nLL/qMFH3EQxiJ2fAyQOaA4kZf
+5ePBAFmo+eggvIksDkc0C+pXwlM2/KfUrzHN/gLldfq5Jwn58/U7yn2fqSLLiMmq
+0Uc9NneoWWRrJ8/vJ8HjJLWG965+Mk2weWjROeiQWMODvA8s1pfrzgzhIMfatz7D
+P78v3DSk+yshzWePS/Tj6tQ/50+6uaWTRRxmHyH6ZF5v4HaUMst19W7l9o/HuKTM
+qJZ9ZPskWkoDbGs4xugDQ5r3V7mzKWmTOPQD8rv7gmsHINFSH5pkAnuYZttcTVoP
+0ISVoDwUQwbKytu4QTbaakRnh6+v40URFWkIsr4WOZckbxJF0WddCajJFdr60qZf
+E2Efv4WstK2tBZQIgx51F9NxO5NQI1mg7TyRVJ12AMXDuDjb
+-----END CERTIFICATE-----
+
+# Issuer: CN=TunTrust Root CA O=Agence Nationale de Certification Electronique
+# Subject: CN=TunTrust Root CA O=Agence Nationale de Certification Electronique
+# Label: "TunTrust Root CA"
+# Serial: 108534058042236574382096126452369648152337120275
+# MD5 Fingerprint: 85:13:b9:90:5b:36:5c:b6:5e:b8:5a:f8:e0:31:57:b4
+# SHA1 Fingerprint: cf:e9:70:84:0f:e0:73:0f:9d:f6:0c:7f:2c:4b:ee:20:46:34:9c:bb
+# SHA256 Fingerprint: 2e:44:10:2a:b5:8c:b8:54:19:45:1c:8e:19:d9:ac:f3:66:2c:af:bc:61:4b:6a:53:96:0a:30:f7:d0:e2:eb:41
+-----BEGIN CERTIFICATE-----
+MIIFszCCA5ugAwIBAgIUEwLV4kBMkkaGFmddtLu7sms+/BMwDQYJKoZIhvcNAQEL
+BQAwYTELMAkGA1UEBhMCVE4xNzA1BgNVBAoMLkFnZW5jZSBOYXRpb25hbGUgZGUg
+Q2VydGlmaWNhdGlvbiBFbGVjdHJvbmlxdWUxGTAXBgNVBAMMEFR1blRydXN0IFJv
+b3QgQ0EwHhcNMTkwNDI2MDg1NzU2WhcNNDQwNDI2MDg1NzU2WjBhMQswCQYDVQQG
+EwJUTjE3MDUGA1UECgwuQWdlbmNlIE5hdGlvbmFsZSBkZSBDZXJ0aWZpY2F0aW9u
+IEVsZWN0cm9uaXF1ZTEZMBcGA1UEAwwQVHVuVHJ1c3QgUm9vdCBDQTCCAiIwDQYJ
+KoZIhvcNAQEBBQADggIPADCCAgoCggIBAMPN0/y9BFPdDCA61YguBUtB9YOCfvdZ
+n56eY+hz2vYGqU8ftPkLHzmMmiDQfgbU7DTZhrx1W4eI8NLZ1KMKsmwb60ksPqxd
+2JQDoOw05TDENX37Jk0bbjBU2PWARZw5rZzJJQRNmpA+TkBuimvNKWfGzC3gdOgF
+VwpIUPp6Q9p+7FuaDmJ2/uqdHYVy7BG7NegfJ7/Boce7SBbdVtfMTqDhuazb1YMZ
+GoXRlJfXyqNlC/M4+QKu3fZnz8k/9YosRxqZbwUN/dAdgjH8KcwAWJeRTIAAHDOF
+li/LQcKLEITDCSSJH7UP2dl3RxiSlGBcx5kDPP73lad9UKGAwqmDrViWVSHbhlnU
+r8a83YFuB9tgYv7sEG7aaAH0gxupPqJbI9dkxt/con3YS7qC0lH4Zr8GRuR5KiY2
+eY8fTpkdso8MDhz/yV3A/ZAQprE38806JG60hZC/gLkMjNWb1sjxVj8agIl6qeIb
+MlEsPvLfe/ZdeikZjuXIvTZxi11Mwh0/rViizz1wTaZQmCXcI/m4WEEIcb9PuISg
+jwBUFfyRbVinljvrS5YnzWuioYasDXxU5mZMZl+QviGaAkYt5IPCgLnPSz7ofzwB
+7I9ezX/SKEIBlYrilz0QIX32nRzFNKHsLA4KUiwSVXAkPcvCFDVDXSdOvsC9qnyW
+5/yeYa1E0wCXAgMBAAGjYzBhMB0GA1UdDgQWBBQGmpsfU33x9aTI04Y+oXNZtPdE
+ITAPBgNVHRMBAf8EBTADAQH/MB8GA1UdIwQYMBaAFAaamx9TffH1pMjThj6hc1m0
+90QhMA4GA1UdDwEB/wQEAwIBBjANBgkqhkiG9w0BAQsFAAOCAgEAqgVutt0Vyb+z
+xiD2BkewhpMl0425yAA/l/VSJ4hxyXT968pk21vvHl26v9Hr7lxpuhbI87mP0zYu
+QEkHDVneixCwSQXi/5E/S7fdAo74gShczNxtr18UnH1YeA32gAm56Q6XKRm4t+v4
+FstVEuTGfbvE7Pi1HE4+Z7/FXxttbUcoqgRYYdZ2vyJ/0Adqp2RT8JeNnYA/u8EH
+22Wv5psymsNUk8QcCMNE+3tjEUPRahphanltkE8pjkcFwRJpadbGNjHh/PqAulxP
+xOu3Mqz4dWEX1xAZufHSCe96Qp1bWgvUxpVOKs7/B9dPfhgGiPEZtdmYu65xxBzn
+dFlY7wyJz4sfdZMaBBSSSFCp61cpABbjNhzI+L/wM9VBD8TMPN3pM0MBkRArHtG5
+Xc0yGYuPjCB31yLEQtyEFpslbei0VXF/sHyz03FJuc9SpAQ/3D2gu68zngowYI7b
+nV2UqL1g52KAdoGDDIzMMEZJ4gzSqK/rYXHv5yJiqfdcZGyfFoxnNidF9Ql7v/YQ
+CvGwjVRDjAS6oz/v4jXH+XTgbzRB0L9zZVcg+ZtnemZoJE6AZb0QmQZZ8mWvuMZH
+u/2QeItBcy6vVR/cO5JyboTT0GFMDcx2V+IthSIVNg3rAZ3r2OvEhJn7wAzMMujj
+d9qDRIueVSjAi1jTkD5OGwDxFa2DK5o=
+-----END CERTIFICATE-----
+
+# Issuer: CN=HARICA TLS RSA Root CA 2021 O=Hellenic Academic and Research Institutions CA
+# Subject: CN=HARICA TLS RSA Root CA 2021 O=Hellenic Academic and Research Institutions CA
+# Label: "HARICA TLS RSA Root CA 2021"
+# Serial: 76817823531813593706434026085292783742
+# MD5 Fingerprint: 65:47:9b:58:86:dd:2c:f0:fc:a2:84:1f:1e:96:c4:91
+# SHA1 Fingerprint: 02:2d:05:82:fa:88:ce:14:0c:06:79:de:7f:14:10:e9:45:d7:a5:6d
+# SHA256 Fingerprint: d9:5d:0e:8e:da:79:52:5b:f9:be:b1:1b:14:d2:10:0d:32:94:98:5f:0c:62:d9:fa:bd:9c:d9:99:ec:cb:7b:1d
+-----BEGIN CERTIFICATE-----
+MIIFpDCCA4ygAwIBAgIQOcqTHO9D88aOk8f0ZIk4fjANBgkqhkiG9w0BAQsFADBs
+MQswCQYDVQQGEwJHUjE3MDUGA1UECgwuSGVsbGVuaWMgQWNhZGVtaWMgYW5kIFJl
+c2VhcmNoIEluc3RpdHV0aW9ucyBDQTEkMCIGA1UEAwwbSEFSSUNBIFRMUyBSU0Eg
+Um9vdCBDQSAyMDIxMB4XDTIxMDIxOTEwNTUzOFoXDTQ1MDIxMzEwNTUzN1owbDEL
+MAkGA1UEBhMCR1IxNzA1BgNVBAoMLkhlbGxlbmljIEFjYWRlbWljIGFuZCBSZXNl
+YXJjaCBJbnN0aXR1dGlvbnMgQ0ExJDAiBgNVBAMMG0hBUklDQSBUTFMgUlNBIFJv
+b3QgQ0EgMjAyMTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBAIvC569l
+mwVnlskNJLnQDmT8zuIkGCyEf3dRywQRNrhe7Wlxp57kJQmXZ8FHws+RFjZiPTgE
+4VGC/6zStGndLuwRo0Xua2s7TL+MjaQenRG56Tj5eg4MmOIjHdFOY9TnuEFE+2uv
+a9of08WRiFukiZLRgeaMOVig1mlDqa2YUlhu2wr7a89o+uOkXjpFc5gH6l8Cct4M
+pbOfrqkdtx2z/IpZ525yZa31MJQjB/OCFks1mJxTuy/K5FrZx40d/JiZ+yykgmvw
+Kh+OC19xXFyuQnspiYHLA6OZyoieC0AJQTPb5lh6/a6ZcMBaD9YThnEvdmn8kN3b
+LW7R8pv1GmuebxWMevBLKKAiOIAkbDakO/IwkfN4E8/BPzWr8R0RI7VDIp4BkrcY
+AuUR0YLbFQDMYTfBKnya4dC6s1BG7oKsnTH4+yPiAwBIcKMJJnkVU2DzOFytOOqB
+AGMUuTNe3QvboEUHGjMJ+E20pwKmafTCWQWIZYVWrkvL4N48fS0ayOn7H6NhStYq
+E613TBoYm5EPWNgGVMWX+Ko/IIqmhaZ39qb8HOLubpQzKoNQhArlT4b4UEV4AIHr
+W2jjJo3Me1xR9BQsQL4aYB16cmEdH2MtiKrOokWQCPxrvrNQKlr9qEgYRtaQQJKQ
+CoReaDH46+0N0x3GfZkYVVYnZS6NRcUk7M7jAgMBAAGjQjBAMA8GA1UdEwEB/wQF
+MAMBAf8wHQYDVR0OBBYEFApII6ZgpJIKM+qTW8VX6iVNvRLuMA4GA1UdDwEB/wQE
+AwIBhjANBgkqhkiG9w0BAQsFAAOCAgEAPpBIqm5iFSVmewzVjIuJndftTgfvnNAU
+X15QvWiWkKQUEapobQk1OUAJ2vQJLDSle1mESSmXdMgHHkdt8s4cUCbjnj1AUz/3
+f5Z2EMVGpdAgS1D0NTsY9FVqQRtHBmg8uwkIYtlfVUKqrFOFrJVWNlar5AWMxaja
+H6NpvVMPxP/cyuN+8kyIhkdGGvMA9YCRotxDQpSbIPDRzbLrLFPCU3hKTwSUQZqP
+JzLB5UkZv/HywouoCjkxKLR9YjYsTewfM7Z+d21+UPCfDtcRj88YxeMn/ibvBZ3P
+zzfF0HvaO7AWhAw6k9a+F9sPPg4ZeAnHqQJyIkv3N3a6dcSFA1pj1bF1BcK5vZSt
+jBWZp5N99sXzqnTPBIWUmAD04vnKJGW/4GKvyMX6ssmeVkjaef2WdhW+o45WxLM0
+/L5H9MG0qPzVMIho7suuyWPEdr6sOBjhXlzPrjoiUevRi7PzKzMHVIf6tLITe7pT
+BGIBnfHAT+7hOtSLIBD6Alfm78ELt5BGnBkpjNxvoEppaZS3JGWg/6w/zgH7IS79
+aPib8qXPMThcFarmlwDB31qlpzmq6YR/PFGoOtmUW4y/Twhx5duoXNTSpv4Ao8YW
+xw/ogM4cKGR0GQjTQuPOAF1/sdwTsOEFy9EgqoZ0njnnkf3/W9b3raYvAwtt41dU
+63ZTGI0RmLo=
+-----END CERTIFICATE-----
+
+# Issuer: CN=HARICA TLS ECC Root CA 2021 O=Hellenic Academic and Research Institutions CA
+# Subject: CN=HARICA TLS ECC Root CA 2021 O=Hellenic Academic and Research Institutions CA
+# Label: "HARICA TLS ECC Root CA 2021"
+# Serial: 137515985548005187474074462014555733966
+# MD5 Fingerprint: ae:f7:4c:e5:66:35:d1:b7:9b:8c:22:93:74:d3:4b:b0
+# SHA1 Fingerprint: bc:b0:c1:9d:e9:98:92:70:19:38:57:e9:8d:a7:b4:5d:6e:ee:01:48
+# SHA256 Fingerprint: 3f:99:cc:47:4a:cf:ce:4d:fe:d5:87:94:66:5e:47:8d:15:47:73:9f:2e:78:0f:1b:b4:ca:9b:13:30:97:d4:01
+-----BEGIN CERTIFICATE-----
+MIICVDCCAdugAwIBAgIQZ3SdjXfYO2rbIvT/WeK/zjAKBggqhkjOPQQDAzBsMQsw
+CQYDVQQGEwJHUjE3MDUGA1UECgwuSGVsbGVuaWMgQWNhZGVtaWMgYW5kIFJlc2Vh
+cmNoIEluc3RpdHV0aW9ucyBDQTEkMCIGA1UEAwwbSEFSSUNBIFRMUyBFQ0MgUm9v
+dCBDQSAyMDIxMB4XDTIxMDIxOTExMDExMFoXDTQ1MDIxMzExMDEwOVowbDELMAkG
+A1UEBhMCR1IxNzA1BgNVBAoMLkhlbGxlbmljIEFjYWRlbWljIGFuZCBSZXNlYXJj
+aCBJbnN0aXR1dGlvbnMgQ0ExJDAiBgNVBAMMG0hBUklDQSBUTFMgRUNDIFJvb3Qg
+Q0EgMjAyMTB2MBAGByqGSM49AgEGBSuBBAAiA2IABDgI/rGgltJ6rK9JOtDA4MM7
+KKrxcm1lAEeIhPyaJmuqS7psBAqIXhfyVYf8MLA04jRYVxqEU+kw2anylnTDUR9Y
+STHMmE5gEYd103KUkE+bECUqqHgtvpBBWJAVcqeht6NCMEAwDwYDVR0TAQH/BAUw
+AwEB/zAdBgNVHQ4EFgQUyRtTgRL+BNUW0aq8mm+3oJUZbsowDgYDVR0PAQH/BAQD
+AgGGMAoGCCqGSM49BAMDA2cAMGQCMBHervjcToiwqfAircJRQO9gcS3ujwLEXQNw
+SaSS6sUUiHCm0w2wqsosQJz76YJumgIwK0eaB8bRwoF8yguWGEEbo/QwCZ61IygN
+nxS2PFOiTAZpffpskcYqSUXm7LcT4Tps
+-----END CERTIFICATE-----
+
+# Issuer: CN=Autoridad de Certificacion Firmaprofesional CIF A62634068
+# Subject: CN=Autoridad de Certificacion Firmaprofesional CIF A62634068
+# Label: "Autoridad de Certificacion Firmaprofesional CIF A62634068"
+# Serial: 1977337328857672817
+# MD5 Fingerprint: 4e:6e:9b:54:4c:ca:b7:fa:48:e4:90:b1:15:4b:1c:a3
+# SHA1 Fingerprint: 0b:be:c2:27:22:49:cb:39:aa:db:35:5c:53:e3:8c:ae:78:ff:b6:fe
+# SHA256 Fingerprint: 57:de:05:83:ef:d2:b2:6e:03:61:da:99:da:9d:f4:64:8d:ef:7e:e8:44:1c:3b:72:8a:fa:9b:cd:e0:f9:b2:6a
+-----BEGIN CERTIFICATE-----
+MIIGFDCCA/ygAwIBAgIIG3Dp0v+ubHEwDQYJKoZIhvcNAQELBQAwUTELMAkGA1UE
+BhMCRVMxQjBABgNVBAMMOUF1dG9yaWRhZCBkZSBDZXJ0aWZpY2FjaW9uIEZpcm1h
+cHJvZmVzaW9uYWwgQ0lGIEE2MjYzNDA2ODAeFw0xNDA5MjMxNTIyMDdaFw0zNjA1
+MDUxNTIyMDdaMFExCzAJBgNVBAYTAkVTMUIwQAYDVQQDDDlBdXRvcmlkYWQgZGUg
+Q2VydGlmaWNhY2lvbiBGaXJtYXByb2Zlc2lvbmFsIENJRiBBNjI2MzQwNjgwggIi
+MA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQDKlmuO6vj78aI14H9M2uDDUtd9
+thDIAl6zQyrET2qyyhxdKJp4ERppWVevtSBC5IsP5t9bpgOSL/UR5GLXMnE42QQM
+cas9UX4PB99jBVzpv5RvwSmCwLTaUbDBPLutN0pcyvFLNg4kq7/DhHf9qFD0sefG
+L9ItWY16Ck6WaVICqjaY7Pz6FIMMNx/Jkjd/14Et5cS54D40/mf0PmbR0/RAz15i
+NA9wBj4gGFrO93IbJWyTdBSTo3OxDqqHECNZXyAFGUftaI6SEspd/NYrspI8IM/h
+X68gvqB2f3bl7BqGYTM+53u0P6APjqK5am+5hyZvQWyIplD9amML9ZMWGxmPsu2b
+m8mQ9QEM3xk9Dz44I8kvjwzRAv4bVdZO0I08r0+k8/6vKtMFnXkIoctXMbScyJCy
+Z/QYFpM6/EfY0XiWMR+6KwxfXZmtY4laJCB22N/9q06mIqqdXuYnin1oKaPnirja
+EbsXLZmdEyRG98Xi2J+Of8ePdG1asuhy9azuJBCtLxTa/y2aRnFHvkLfuwHb9H/T
+KI8xWVvTyQKmtFLKbpf7Q8UIJm+K9Lv9nyiqDdVF8xM6HdjAeI9BZzwelGSuewvF
+6NkBiDkal4ZkQdU7hwxu+g/GvUgUvzlN1J5Bto+WHWOWk9mVBngxaJ43BjuAiUVh
+OSPHG0SjFeUc+JIwuwIDAQABo4HvMIHsMB0GA1UdDgQWBBRlzeurNR4APn7VdMAc
+tHNHDhpkLzASBgNVHRMBAf8ECDAGAQH/AgEBMIGmBgNVHSAEgZ4wgZswgZgGBFUd
+IAAwgY8wLwYIKwYBBQUHAgEWI2h0dHA6Ly93d3cuZmlybWFwcm9mZXNpb25hbC5j
+b20vY3BzMFwGCCsGAQUFBwICMFAeTgBQAGEAcwBlAG8AIABkAGUAIABsAGEAIABC
+AG8AbgBhAG4AbwB2AGEAIAA0ADcAIABCAGEAcgBjAGUAbABvAG4AYQAgADAAOAAw
+ADEANzAOBgNVHQ8BAf8EBAMCAQYwDQYJKoZIhvcNAQELBQADggIBAHSHKAIrdx9m
+iWTtj3QuRhy7qPj4Cx2Dtjqn6EWKB7fgPiDL4QjbEwj4KKE1soCzC1HA01aajTNF
+Sa9J8OA9B3pFE1r/yJfY0xgsfZb43aJlQ3CTkBW6kN/oGbDbLIpgD7dvlAceHabJ
+hfa9NPhAeGIQcDq+fUs5gakQ1JZBu/hfHAsdCPKxsIl68veg4MSPi3i1O1ilI45P
+Vf42O+AMt8oqMEEgtIDNrvx2ZnOorm7hfNoD6JQg5iKj0B+QXSBTFCZX2lSX3xZE
+EAEeiGaPcjiT3SC3NL7X8e5jjkd5KAb881lFJWAiMxujX6i6KtoaPc1A6ozuBRWV
+1aUsIC+nmCjuRfzxuIgALI9C2lHVnOUTaHFFQ4ueCyE8S1wF3BqfmI7avSKecs2t
+CsvMo2ebKHTEm9caPARYpoKdrcd7b/+Alun4jWq9GJAd/0kakFI3ky88Al2CdgtR
+5xbHV/g4+afNmyJU72OwFW1TZQNKXkqgsqeOSQBZONXH9IBk9W6VULgRfhVwOEqw
+f9DEMnDAGf/JOC0ULGb0QkTmVXYbgBVX/8Cnp6o5qtjTcNAuuuuUavpfNIbnYrX9
+ivAwhZTJryQCL2/W3Wf+47BVTwSYT6RBVuKT0Gro1vP7ZeDOdcQxWQzugsgMYDNK
+GbqEZycPvEJdvSRUDewdcAZfpLz6IHxV
+-----END CERTIFICATE-----
+
+# Issuer: CN=vTrus ECC Root CA O=iTrusChina Co.,Ltd.
+# Subject: CN=vTrus ECC Root CA O=iTrusChina Co.,Ltd.
+# Label: "vTrus ECC Root CA"
+# Serial: 630369271402956006249506845124680065938238527194
+# MD5 Fingerprint: de:4b:c1:f5:52:8c:9b:43:e1:3e:8f:55:54:17:8d:85
+# SHA1 Fingerprint: f6:9c:db:b0:fc:f6:02:13:b6:52:32:a6:a3:91:3f:16:70:da:c3:e1
+# SHA256 Fingerprint: 30:fb:ba:2c:32:23:8e:2a:98:54:7a:f9:79:31:e5:50:42:8b:9b:3f:1c:8e:eb:66:33:dc:fa:86:c5:b2:7d:d3
+-----BEGIN CERTIFICATE-----
+MIICDzCCAZWgAwIBAgIUbmq8WapTvpg5Z6LSa6Q75m0c1towCgYIKoZIzj0EAwMw
+RzELMAkGA1UEBhMCQ04xHDAaBgNVBAoTE2lUcnVzQ2hpbmEgQ28uLEx0ZC4xGjAY
+BgNVBAMTEXZUcnVzIEVDQyBSb290IENBMB4XDTE4MDczMTA3MjY0NFoXDTQzMDcz
+MTA3MjY0NFowRzELMAkGA1UEBhMCQ04xHDAaBgNVBAoTE2lUcnVzQ2hpbmEgQ28u
+LEx0ZC4xGjAYBgNVBAMTEXZUcnVzIEVDQyBSb290IENBMHYwEAYHKoZIzj0CAQYF
+K4EEACIDYgAEZVBKrox5lkqqHAjDo6LN/llWQXf9JpRCux3NCNtzslt188+cToL0
+v/hhJoVs1oVbcnDS/dtitN9Ti72xRFhiQgnH+n9bEOf+QP3A2MMrMudwpremIFUd
+e4BdS49nTPEQo0IwQDAdBgNVHQ4EFgQUmDnNvtiyjPeyq+GtJK97fKHbH88wDwYD
+VR0TAQH/BAUwAwEB/zAOBgNVHQ8BAf8EBAMCAQYwCgYIKoZIzj0EAwMDaAAwZQIw
+V53dVvHH4+m4SVBrm2nDb+zDfSXkV5UTQJtS0zvzQBm8JsctBp61ezaf9SXUY2sA
+AjEA6dPGnlaaKsyh2j/IZivTWJwghfqrkYpwcBE4YGQLYgmRWAD5Tfs0aNoJrSEG
+GJTO
+-----END CERTIFICATE-----
+
+# Issuer: CN=vTrus Root CA O=iTrusChina Co.,Ltd.
+# Subject: CN=vTrus Root CA O=iTrusChina Co.,Ltd.
+# Label: "vTrus Root CA"
+# Serial: 387574501246983434957692974888460947164905180485
+# MD5 Fingerprint: b8:c9:37:df:fa:6b:31:84:64:c5:ea:11:6a:1b:75:fc
+# SHA1 Fingerprint: 84:1a:69:fb:f5:cd:1a:25:34:13:3d:e3:f8:fc:b8:99:d0:c9:14:b7
+# SHA256 Fingerprint: 8a:71:de:65:59:33:6f:42:6c:26:e5:38:80:d0:0d:88:a1:8d:a4:c6:a9:1f:0d:cb:61:94:e2:06:c5:c9:63:87
+-----BEGIN CERTIFICATE-----
+MIIFVjCCAz6gAwIBAgIUQ+NxE9izWRRdt86M/TX9b7wFjUUwDQYJKoZIhvcNAQEL
+BQAwQzELMAkGA1UEBhMCQ04xHDAaBgNVBAoTE2lUcnVzQ2hpbmEgQ28uLEx0ZC4x
+FjAUBgNVBAMTDXZUcnVzIFJvb3QgQ0EwHhcNMTgwNzMxMDcyNDA1WhcNNDMwNzMx
+MDcyNDA1WjBDMQswCQYDVQQGEwJDTjEcMBoGA1UEChMTaVRydXNDaGluYSBDby4s
+THRkLjEWMBQGA1UEAxMNdlRydXMgUm9vdCBDQTCCAiIwDQYJKoZIhvcNAQEBBQAD
+ggIPADCCAgoCggIBAL1VfGHTuB0EYgWgrmy3cLRB6ksDXhA/kFocizuwZotsSKYc
+IrrVQJLuM7IjWcmOvFjai57QGfIvWcaMY1q6n6MLsLOaXLoRuBLpDLvPbmyAhykU
+AyyNJJrIZIO1aqwTLDPxn9wsYTwaP3BVm60AUn/PBLn+NvqcwBauYv6WTEN+VRS+
+GrPSbcKvdmaVayqwlHeFXgQPYh1jdfdr58tbmnDsPmcF8P4HCIDPKNsFxhQnL4Z9
+8Cfe/+Z+M0jnCx5Y0ScrUw5XSmXX+6KAYPxMvDVTAWqXcoKv8R1w6Jz1717CbMdH
+flqUhSZNO7rrTOiwCcJlwp2dCZtOtZcFrPUGoPc2BX70kLJrxLT5ZOrpGgrIDajt
+J8nU57O5q4IikCc9Kuh8kO+8T/3iCiSn3mUkpF3qwHYw03dQ+A0Em5Q2AXPKBlim
+0zvc+gRGE1WKyURHuFE5Gi7oNOJ5y1lKCn+8pu8fA2dqWSslYpPZUxlmPCdiKYZN
+pGvu/9ROutW04o5IWgAZCfEF2c6Rsffr6TlP9m8EQ5pV9T4FFL2/s1m02I4zhKOQ
+UqqzApVg+QxMaPnu1RcN+HFXtSXkKe5lXa/R7jwXC1pDxaWG6iSe4gUH3DRCEpHW
+OXSuTEGC2/KmSNGzm/MzqvOmwMVO9fSddmPmAsYiS8GVP1BkLFTltvA8Kc9XAgMB
+AAGjQjBAMB0GA1UdDgQWBBRUYnBj8XWEQ1iO0RYgscasGrz2iTAPBgNVHRMBAf8E
+BTADAQH/MA4GA1UdDwEB/wQEAwIBBjANBgkqhkiG9w0BAQsFAAOCAgEAKbqSSaet
+8PFww+SX8J+pJdVrnjT+5hpk9jprUrIQeBqfTNqK2uwcN1LgQkv7bHbKJAs5EhWd
+nxEt/Hlk3ODg9d3gV8mlsnZwUKT+twpw1aA08XXXTUm6EdGz2OyC/+sOxL9kLX1j
+bhd47F18iMjrjld22VkE+rxSH0Ws8HqA7Oxvdq6R2xCOBNyS36D25q5J08FsEhvM
+Kar5CKXiNxTKsbhm7xqC5PD48acWabfbqWE8n/Uxy+QARsIvdLGx14HuqCaVvIiv
+TDUHKgLKeBRtRytAVunLKmChZwOgzoy8sHJnxDHO2zTlJQNgJXtxmOTAGytfdELS
+S8VZCAeHvsXDf+eW2eHcKJfWjwXj9ZtOyh1QRwVTsMo554WgicEFOwE30z9J4nfr
+I8iIZjs9OXYhRvHsXyO466JmdXTBQPfYaJqT4i2pLr0cox7IdMakLXogqzu4sEb9
+b91fUlV1YvCXoHzXOP0l382gmxDPi7g4Xl7FtKYCNqEeXxzP4padKar9mK5S4fNB
+UvupLnKWnyfjqnN9+BojZns7q2WwMgFLFT49ok8MKzWixtlnEjUwzXYuFrOZnk1P
+Ti07NEPhmg4NpGaXutIcSkwsKouLgU9xGqndXHt7CMUADTdA43x7VF8vhV929ven
+sBxXVsFy6K2ir40zSbofitzmdHxghm+Hl3s=
+-----END CERTIFICATE-----
+
+# Issuer: CN=ISRG Root X2 O=Internet Security Research Group
+# Subject: CN=ISRG Root X2 O=Internet Security Research Group
+# Label: "ISRG Root X2"
+# Serial: 87493402998870891108772069816698636114
+# MD5 Fingerprint: d3:9e:c4:1e:23:3c:a6:df:cf:a3:7e:6d:e0:14:e6:e5
+# SHA1 Fingerprint: bd:b1:b9:3c:d5:97:8d:45:c6:26:14:55:f8:db:95:c7:5a:d1:53:af
+# SHA256 Fingerprint: 69:72:9b:8e:15:a8:6e:fc:17:7a:57:af:b7:17:1d:fc:64:ad:d2:8c:2f:ca:8c:f1:50:7e:34:45:3c:cb:14:70
+-----BEGIN CERTIFICATE-----
+MIICGzCCAaGgAwIBAgIQQdKd0XLq7qeAwSxs6S+HUjAKBggqhkjOPQQDAzBPMQsw
+CQYDVQQGEwJVUzEpMCcGA1UEChMgSW50ZXJuZXQgU2VjdXJpdHkgUmVzZWFyY2gg
+R3JvdXAxFTATBgNVBAMTDElTUkcgUm9vdCBYMjAeFw0yMDA5MDQwMDAwMDBaFw00
+MDA5MTcxNjAwMDBaME8xCzAJBgNVBAYTAlVTMSkwJwYDVQQKEyBJbnRlcm5ldCBT
+ZWN1cml0eSBSZXNlYXJjaCBHcm91cDEVMBMGA1UEAxMMSVNSRyBSb290IFgyMHYw
+EAYHKoZIzj0CAQYFK4EEACIDYgAEzZvVn4CDCuwJSvMWSj5cz3es3mcFDR0HttwW
++1qLFNvicWDEukWVEYmO6gbf9yoWHKS5xcUy4APgHoIYOIvXRdgKam7mAHf7AlF9
+ItgKbppbd9/w+kHsOdx1ymgHDB/qo0IwQDAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0T
+AQH/BAUwAwEB/zAdBgNVHQ4EFgQUfEKWrt5LSDv6kviejM9ti6lyN5UwCgYIKoZI
+zj0EAwMDaAAwZQIwe3lORlCEwkSHRhtFcP9Ymd70/aTSVaYgLXTWNLxBo1BfASdW
+tL4ndQavEi51mI38AjEAi/V3bNTIZargCyzuFJ0nN6T5U6VR5CmD1/iQMVtCnwr1
+/q4AaOeMSQ+2b1tbFfLn
+-----END CERTIFICATE-----
+
+# Issuer: CN=HiPKI Root CA - G1 O=Chunghwa Telecom Co., Ltd.
+# Subject: CN=HiPKI Root CA - G1 O=Chunghwa Telecom Co., Ltd.
+# Label: "HiPKI Root CA - G1"
+# Serial: 60966262342023497858655262305426234976
+# MD5 Fingerprint: 69:45:df:16:65:4b:e8:68:9a:8f:76:5f:ff:80:9e:d3
+# SHA1 Fingerprint: 6a:92:e4:a8:ee:1b:ec:96:45:37:e3:29:57:49:cd:96:e3:e5:d2:60
+# SHA256 Fingerprint: f0:15:ce:3c:c2:39:bf:ef:06:4b:e9:f1:d2:c4:17:e1:a0:26:4a:0a:94:be:1f:0c:8d:12:18:64:eb:69:49:cc
+-----BEGIN CERTIFICATE-----
+MIIFajCCA1KgAwIBAgIQLd2szmKXlKFD6LDNdmpeYDANBgkqhkiG9w0BAQsFADBP
+MQswCQYDVQQGEwJUVzEjMCEGA1UECgwaQ2h1bmdod2EgVGVsZWNvbSBDby4sIEx0
+ZC4xGzAZBgNVBAMMEkhpUEtJIFJvb3QgQ0EgLSBHMTAeFw0xOTAyMjIwOTQ2MDRa
+Fw0zNzEyMzExNTU5NTlaME8xCzAJBgNVBAYTAlRXMSMwIQYDVQQKDBpDaHVuZ2h3
+YSBUZWxlY29tIENvLiwgTHRkLjEbMBkGA1UEAwwSSGlQS0kgUm9vdCBDQSAtIEcx
+MIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEA9B5/UnMyDHPkvRN0o9Qw
+qNCuS9i233VHZvR85zkEHmpwINJaR3JnVfSl6J3VHiGh8Ge6zCFovkRTv4354twv
+Vcg3Px+kwJyz5HdcoEb+d/oaoDjq7Zpy3iu9lFc6uux55199QmQ5eiY29yTw1S+6
+lZgRZq2XNdZ1AYDgr/SEYYwNHl98h5ZeQa/rh+r4XfEuiAU+TCK72h8q3VJGZDnz
+Qs7ZngyzsHeXZJzA9KMuH5UHsBffMNsAGJZMoYFL3QRtU6M9/Aes1MU3guvklQgZ
+KILSQjqj2FPseYlgSGDIcpJQ3AOPgz+yQlda22rpEZfdhSi8MEyr48KxRURHH+CK
+FgeW0iEPU8DtqX7UTuybCeyvQqww1r/REEXgphaypcXTT3OUM3ECoWqj1jOXTyFj
+HluP2cFeRXF3D4FdXyGarYPM+l7WjSNfGz1BryB1ZlpK9p/7qxj3ccC2HTHsOyDr
+y+K49a6SsvfhhEvyovKTmiKe0xRvNlS9H15ZFblzqMF8b3ti6RZsR1pl8w4Rm0bZ
+/W3c1pzAtH2lsN0/Vm+h+fbkEkj9Bn8SV7apI09bA8PgcSojt/ewsTu8mL3WmKgM
+a/aOEmem8rJY5AIJEzypuxC00jBF8ez3ABHfZfjcK0NVvxaXxA/VLGGEqnKG/uY6
+fsI/fe78LxQ+5oXdUG+3Se0CAwEAAaNCMEAwDwYDVR0TAQH/BAUwAwEB/zAdBgNV
+HQ4EFgQU8ncX+l6o/vY9cdVouslGDDjYr7AwDgYDVR0PAQH/BAQDAgGGMA0GCSqG
+SIb3DQEBCwUAA4ICAQBQUfB13HAE4/+qddRxosuej6ip0691x1TPOhwEmSKsxBHi
+7zNKpiMdDg1H2DfHb680f0+BazVP6XKlMeJ45/dOlBhbQH3PayFUhuaVevvGyuqc
+SE5XCV0vrPSltJczWNWseanMX/mF+lLFjfiRFOs6DRfQUsJ748JzjkZ4Bjgs6Fza
+ZsT0pPBWGTMpWmWSBUdGSquEwx4noR8RkpkndZMPvDY7l1ePJlsMu5wP1G4wB9Tc
+XzZoZjmDlicmisjEOf6aIW/Vcobpf2Lll07QJNBAsNB1CI69aO4I1258EHBGG3zg
+iLKecoaZAeO/n0kZtCW+VmWuF2PlHt/o/0elv+EmBYTksMCv5wiZqAxeJoBF1Pho
+L5aPruJKHJwWDBNvOIf2u8g0X5IDUXlwpt/L9ZlNec1OvFefQ05rLisY+GpzjLrF
+Ne85akEez3GoorKGB1s6yeHvP2UEgEcyRHCVTjFnanRbEEV16rCf0OY1/k6fi8wr
+kkVbbiVghUbN0aqwdmaTd5a+g744tiROJgvM7XpWGuDpWsZkrUx6AEhEL7lAuxM+
+vhV4nYWBSipX3tUZQ9rbyltHhoMLP7YNdnhzeSJesYAfz77RP1YQmCuVh6EfnWQU
+YDksswBVLuT1sw5XxJFBAJw/6KXf6vb/yPCtbVKoF6ubYfwSUTXkJf2vqmqGOQ==
+-----END CERTIFICATE-----
+
+# Issuer: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R4
+# Subject: CN=GlobalSign O=GlobalSign OU=GlobalSign ECC Root CA - R4
+# Label: "GlobalSign ECC Root CA - R4"
+# Serial: 159662223612894884239637590694
+# MD5 Fingerprint: 26:29:f8:6d:e1:88:bf:a2:65:7f:aa:c4:cd:0f:7f:fc
+# SHA1 Fingerprint: 6b:a0:b0:98:e1:71:ef:5a:ad:fe:48:15:80:77:10:f4:bd:6f:0b:28
+# SHA256 Fingerprint: b0:85:d7:0b:96:4f:19:1a:73:e4:af:0d:54:ae:7a:0e:07:aa:fd:af:9b:71:dd:08:62:13:8a:b7:32:5a:24:a2
+-----BEGIN CERTIFICATE-----
+MIIB3DCCAYOgAwIBAgINAgPlfvU/k/2lCSGypjAKBggqhkjOPQQDAjBQMSQwIgYD
+VQQLExtHbG9iYWxTaWduIEVDQyBSb290IENBIC0gUjQxEzARBgNVBAoTCkdsb2Jh
+bFNpZ24xEzARBgNVBAMTCkdsb2JhbFNpZ24wHhcNMTIxMTEzMDAwMDAwWhcNMzgw
+MTE5MDMxNDA3WjBQMSQwIgYDVQQLExtHbG9iYWxTaWduIEVDQyBSb290IENBIC0g
+UjQxEzARBgNVBAoTCkdsb2JhbFNpZ24xEzARBgNVBAMTCkdsb2JhbFNpZ24wWTAT
+BgcqhkjOPQIBBggqhkjOPQMBBwNCAAS4xnnTj2wlDp8uORkcA6SumuU5BwkWymOx
+uYb4ilfBV85C+nOh92VC/x7BALJucw7/xyHlGKSq2XE/qNS5zowdo0IwQDAOBgNV
+HQ8BAf8EBAMCAYYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQUVLB7rUW44kB/
++wpu+74zyTyjhNUwCgYIKoZIzj0EAwIDRwAwRAIgIk90crlgr/HmnKAWBVBfw147
+bmF0774BxL4YSFlhgjICICadVGNA3jdgUM/I2O2dgq43mLyjj0xMqTQrbO/7lZsm
+-----END CERTIFICATE-----
+
+# Issuer: CN=GTS Root R1 O=Google Trust Services LLC
+# Subject: CN=GTS Root R1 O=Google Trust Services LLC
+# Label: "GTS Root R1"
+# Serial: 159662320309726417404178440727
+# MD5 Fingerprint: 05:fe:d0:bf:71:a8:a3:76:63:da:01:e0:d8:52:dc:40
+# SHA1 Fingerprint: e5:8c:1c:c4:91:3b:38:63:4b:e9:10:6e:e3:ad:8e:6b:9d:d9:81:4a
+# SHA256 Fingerprint: d9:47:43:2a:bd:e7:b7:fa:90:fc:2e:6b:59:10:1b:12:80:e0:e1:c7:e4:e4:0f:a3:c6:88:7f:ff:57:a7:f4:cf
+-----BEGIN CERTIFICATE-----
+MIIFVzCCAz+gAwIBAgINAgPlk28xsBNJiGuiFzANBgkqhkiG9w0BAQwFADBHMQsw
+CQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEU
+MBIGA1UEAxMLR1RTIFJvb3QgUjEwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAw
+MDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZp
+Y2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjEwggIiMA0GCSqGSIb3DQEBAQUA
+A4ICDwAwggIKAoICAQC2EQKLHuOhd5s73L+UPreVp0A8of2C+X0yBoJx9vaMf/vo
+27xqLpeXo4xL+Sv2sfnOhB2x+cWX3u+58qPpvBKJXqeqUqv4IyfLpLGcY9vXmX7w
+Cl7raKb0xlpHDU0QM+NOsROjyBhsS+z8CZDfnWQpJSMHobTSPS5g4M/SCYe7zUjw
+TcLCeoiKu7rPWRnWr4+wB7CeMfGCwcDfLqZtbBkOtdh+JhpFAz2weaSUKK0Pfybl
+qAj+lug8aJRT7oM6iCsVlgmy4HqMLnXWnOunVmSPlk9orj2XwoSPwLxAwAtcvfaH
+szVsrBhQf4TgTM2S0yDpM7xSma8ytSmzJSq0SPly4cpk9+aCEI3oncKKiPo4Zor8
+Y/kB+Xj9e1x3+naH+uzfsQ55lVe0vSbv1gHR6xYKu44LtcXFilWr06zqkUspzBmk
+MiVOKvFlRNACzqrOSbTqn3yDsEB750Orp2yjj32JgfpMpf/VjsPOS+C12LOORc92
+wO1AK/1TD7Cn1TsNsYqiA94xrcx36m97PtbfkSIS5r762DL8EGMUUXLeXdYWk70p
+aDPvOmbsB4om3xPXV2V4J95eSRQAogB/mqghtqmxlbCluQ0WEdrHbEg8QOB+DVrN
+VjzRlwW5y0vtOUucxD/SVRNuJLDWcfr0wbrM7Rv1/oFB2ACYPTrIrnqYNxgFlQID
+AQABo0IwQDAOBgNVHQ8BAf8EBAMCAYYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4E
+FgQU5K8rJnEaK0gnhS9SZizv8IkTcT4wDQYJKoZIhvcNAQEMBQADggIBAJ+qQibb
+C5u+/x6Wki4+omVKapi6Ist9wTrYggoGxval3sBOh2Z5ofmmWJyq+bXmYOfg6LEe
+QkEzCzc9zolwFcq1JKjPa7XSQCGYzyI0zzvFIoTgxQ6KfF2I5DUkzps+GlQebtuy
+h6f88/qBVRRiClmpIgUxPoLW7ttXNLwzldMXG+gnoot7TiYaelpkttGsN/H9oPM4
+7HLwEXWdyzRSjeZ2axfG34arJ45JK3VmgRAhpuo+9K4l/3wV3s6MJT/KYnAK9y8J
+ZgfIPxz88NtFMN9iiMG1D53Dn0reWVlHxYciNuaCp+0KueIHoI17eko8cdLiA6Ef
+MgfdG+RCzgwARWGAtQsgWSl4vflVy2PFPEz0tv/bal8xa5meLMFrUKTX5hgUvYU/
+Z6tGn6D/Qqc6f1zLXbBwHSs09dR2CQzreExZBfMzQsNhFRAbd03OIozUhfJFfbdT
+6u9AWpQKXCBfTkBdYiJ23//OYb2MI3jSNwLgjt7RETeJ9r/tSQdirpLsQBqvFAnZ
+0E6yove+7u7Y/9waLd64NnHi/Hm3lCXRSHNboTXns5lndcEZOitHTtNCjv0xyBZm
+2tIMPNuzjsmhDYAPexZ3FL//2wmUspO8IFgV6dtxQ/PeEMMA3KgqlbbC1j+Qa3bb
+bP6MvPJwNQzcmRk13NfIRmPVNnGuV/u3gm3c
+-----END CERTIFICATE-----
+
+# Issuer: CN=GTS Root R2 O=Google Trust Services LLC
+# Subject: CN=GTS Root R2 O=Google Trust Services LLC
+# Label: "GTS Root R2"
+# Serial: 159662449406622349769042896298
+# MD5 Fingerprint: 1e:39:c0:53:e6:1e:29:82:0b:ca:52:55:36:5d:57:dc
+# SHA1 Fingerprint: 9a:44:49:76:32:db:de:fa:d0:bc:fb:5a:7b:17:bd:9e:56:09:24:94
+# SHA256 Fingerprint: 8d:25:cd:97:22:9d:bf:70:35:6b:da:4e:b3:cc:73:40:31:e2:4c:f0:0f:af:cf:d3:2d:c7:6e:b5:84:1c:7e:a8
+-----BEGIN CERTIFICATE-----
+MIIFVzCCAz+gAwIBAgINAgPlrsWNBCUaqxElqjANBgkqhkiG9w0BAQwFADBHMQsw
+CQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEU
+MBIGA1UEAxMLR1RTIFJvb3QgUjIwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAw
+MDAwWjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZp
+Y2VzIExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjIwggIiMA0GCSqGSIb3DQEBAQUA
+A4ICDwAwggIKAoICAQDO3v2m++zsFDQ8BwZabFn3GTXd98GdVarTzTukk3LvCvpt
+nfbwhYBboUhSnznFt+4orO/LdmgUud+tAWyZH8QiHZ/+cnfgLFuv5AS/T3KgGjSY
+6Dlo7JUle3ah5mm5hRm9iYz+re026nO8/4Piy33B0s5Ks40FnotJk9/BW9BuXvAu
+MC6C/Pq8tBcKSOWIm8Wba96wyrQD8Nr0kLhlZPdcTK3ofmZemde4wj7I0BOdre7k
+RXuJVfeKH2JShBKzwkCX44ofR5GmdFrS+LFjKBC4swm4VndAoiaYecb+3yXuPuWg
+f9RhD1FLPD+M2uFwdNjCaKH5wQzpoeJ/u1U8dgbuak7MkogwTZq9TwtImoS1mKPV
++3PBV2HdKFZ1E66HjucMUQkQdYhMvI35ezzUIkgfKtzra7tEscszcTJGr61K8Yzo
+dDqs5xoic4DSMPclQsciOzsSrZYuxsN2B6ogtzVJV+mSSeh2FnIxZyuWfoqjx5RW
+Ir9qS34BIbIjMt/kmkRtWVtd9QCgHJvGeJeNkP+byKq0rxFROV7Z+2et1VsRnTKa
+G73VululycslaVNVJ1zgyjbLiGH7HrfQy+4W+9OmTN6SpdTi3/UGVN4unUu0kzCq
+gc7dGtxRcw1PcOnlthYhGXmy5okLdWTK1au8CcEYof/UVKGFPP0UJAOyh9OktwID
+AQABo0IwQDAOBgNVHQ8BAf8EBAMCAYYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4E
+FgQUu//KjiOfT5nK2+JopqUVJxce2Q4wDQYJKoZIhvcNAQEMBQADggIBAB/Kzt3H
+vqGf2SdMC9wXmBFqiN495nFWcrKeGk6c1SuYJF2ba3uwM4IJvd8lRuqYnrYb/oM8
+0mJhwQTtzuDFycgTE1XnqGOtjHsB/ncw4c5omwX4Eu55MaBBRTUoCnGkJE+M3DyC
+B19m3H0Q/gxhswWV7uGugQ+o+MePTagjAiZrHYNSVc61LwDKgEDg4XSsYPWHgJ2u
+NmSRXbBoGOqKYcl3qJfEycel/FVL8/B/uWU9J2jQzGv6U53hkRrJXRqWbTKH7QMg
+yALOWr7Z6v2yTcQvG99fevX4i8buMTolUVVnjWQye+mew4K6Ki3pHrTgSAai/Gev
+HyICc/sgCq+dVEuhzf9gR7A/Xe8bVr2XIZYtCtFenTgCR2y59PYjJbigapordwj6
+xLEokCZYCDzifqrXPW+6MYgKBesntaFJ7qBFVHvmJ2WZICGoo7z7GJa7Um8M7YNR
+TOlZ4iBgxcJlkoKM8xAfDoqXvneCbT+PHV28SSe9zE8P4c52hgQjxcCMElv924Sg
+JPFI/2R80L5cFtHvma3AH/vLrrw4IgYmZNralw4/KBVEqE8AyvCazM90arQ+POuV
+7LXTWtiBmelDGDfrs7vRWGJB82bSj6p4lVQgw1oudCvV0b4YacCs1aTPObpRhANl
+6WLAYv7YTVWW4tAR+kg0Eeye7QUd5MjWHYbL
+-----END CERTIFICATE-----
+
+# Issuer: CN=GTS Root R3 O=Google Trust Services LLC
+# Subject: CN=GTS Root R3 O=Google Trust Services LLC
+# Label: "GTS Root R3"
+# Serial: 159662495401136852707857743206
+# MD5 Fingerprint: 3e:e7:9d:58:02:94:46:51:94:e5:e0:22:4a:8b:e7:73
+# SHA1 Fingerprint: ed:e5:71:80:2b:c8:92:b9:5b:83:3c:d2:32:68:3f:09:cd:a0:1e:46
+# SHA256 Fingerprint: 34:d8:a7:3e:e2:08:d9:bc:db:0d:95:65:20:93:4b:4e:40:e6:94:82:59:6e:8b:6f:73:c8:42:6b:01:0a:6f:48
+-----BEGIN CERTIFICATE-----
+MIICCTCCAY6gAwIBAgINAgPluILrIPglJ209ZjAKBggqhkjOPQQDAzBHMQswCQYD
+VQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEUMBIG
+A1UEAxMLR1RTIFJvb3QgUjMwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAwMDAw
+WjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2Vz
+IExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjMwdjAQBgcqhkjOPQIBBgUrgQQAIgNi
+AAQfTzOHMymKoYTey8chWEGJ6ladK0uFxh1MJ7x/JlFyb+Kf1qPKzEUURout736G
+jOyxfi//qXGdGIRFBEFVbivqJn+7kAHjSxm65FSWRQmx1WyRRK2EE46ajA2ADDL2
+4CejQjBAMA4GA1UdDwEB/wQEAwIBhjAPBgNVHRMBAf8EBTADAQH/MB0GA1UdDgQW
+BBTB8Sa6oC2uhYHP0/EqEr24Cmf9vDAKBggqhkjOPQQDAwNpADBmAjEA9uEglRR7
+VKOQFhG/hMjqb2sXnh5GmCCbn9MN2azTL818+FsuVbu/3ZL3pAzcMeGiAjEA/Jdm
+ZuVDFhOD3cffL74UOO0BzrEXGhF16b0DjyZ+hOXJYKaV11RZt+cRLInUue4X
+-----END CERTIFICATE-----
+
+# Issuer: CN=GTS Root R4 O=Google Trust Services LLC
+# Subject: CN=GTS Root R4 O=Google Trust Services LLC
+# Label: "GTS Root R4"
+# Serial: 159662532700760215368942768210
+# MD5 Fingerprint: 43:96:83:77:19:4d:76:b3:9d:65:52:e4:1d:22:a5:e8
+# SHA1 Fingerprint: 77:d3:03:67:b5:e0:0c:15:f6:0c:38:61:df:7c:e1:3b:92:46:4d:47
+# SHA256 Fingerprint: 34:9d:fa:40:58:c5:e2:63:12:3b:39:8a:e7:95:57:3c:4e:13:13:c8:3f:e6:8f:93:55:6c:d5:e8:03:1b:3c:7d
+-----BEGIN CERTIFICATE-----
+MIICCTCCAY6gAwIBAgINAgPlwGjvYxqccpBQUjAKBggqhkjOPQQDAzBHMQswCQYD
+VQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2VzIExMQzEUMBIG
+A1UEAxMLR1RTIFJvb3QgUjQwHhcNMTYwNjIyMDAwMDAwWhcNMzYwNjIyMDAwMDAw
+WjBHMQswCQYDVQQGEwJVUzEiMCAGA1UEChMZR29vZ2xlIFRydXN0IFNlcnZpY2Vz
+IExMQzEUMBIGA1UEAxMLR1RTIFJvb3QgUjQwdjAQBgcqhkjOPQIBBgUrgQQAIgNi
+AATzdHOnaItgrkO4NcWBMHtLSZ37wWHO5t5GvWvVYRg1rkDdc/eJkTBa6zzuhXyi
+QHY7qca4R9gq55KRanPpsXI5nymfopjTX15YhmUPoYRlBtHci8nHc8iMai/lxKvR
+HYqjQjBAMA4GA1UdDwEB/wQEAwIBhjAPBgNVHRMBAf8EBTADAQH/MB0GA1UdDgQW
+BBSATNbrdP9JNqPV2Py1PsVq8JQdjDAKBggqhkjOPQQDAwNpADBmAjEA6ED/g94D
+9J+uHXqnLrmvT/aDHQ4thQEd0dlq7A/Cr8deVl5c1RxYIigL9zC2L7F8AjEA8GE8
+p/SgguMh1YQdc4acLa/KNJvxn7kjNuK8YAOdgLOaVsjh4rsUecrNIdSUtUlD
+-----END CERTIFICATE-----
+
+# Issuer: CN=Telia Root CA v2 O=Telia Finland Oyj
+# Subject: CN=Telia Root CA v2 O=Telia Finland Oyj
+# Label: "Telia Root CA v2"
+# Serial: 7288924052977061235122729490515358
+# MD5 Fingerprint: 0e:8f:ac:aa:82:df:85:b1:f4:dc:10:1c:fc:99:d9:48
+# SHA1 Fingerprint: b9:99:cd:d1:73:50:8a:c4:47:05:08:9c:8c:88:fb:be:a0:2b:40:cd
+# SHA256 Fingerprint: 24:2b:69:74:2f:cb:1e:5b:2a:bf:98:89:8b:94:57:21:87:54:4e:5b:4d:99:11:78:65:73:62:1f:6a:74:b8:2c
+-----BEGIN CERTIFICATE-----
+MIIFdDCCA1ygAwIBAgIPAWdfJ9b+euPkrL4JWwWeMA0GCSqGSIb3DQEBCwUAMEQx
+CzAJBgNVBAYTAkZJMRowGAYDVQQKDBFUZWxpYSBGaW5sYW5kIE95ajEZMBcGA1UE
+AwwQVGVsaWEgUm9vdCBDQSB2MjAeFw0xODExMjkxMTU1NTRaFw00MzExMjkxMTU1
+NTRaMEQxCzAJBgNVBAYTAkZJMRowGAYDVQQKDBFUZWxpYSBGaW5sYW5kIE95ajEZ
+MBcGA1UEAwwQVGVsaWEgUm9vdCBDQSB2MjCCAiIwDQYJKoZIhvcNAQEBBQADggIP
+ADCCAgoCggIBALLQPwe84nvQa5n44ndp586dpAO8gm2h/oFlH0wnrI4AuhZ76zBq
+AMCzdGh+sq/H1WKzej9Qyow2RCRj0jbpDIX2Q3bVTKFgcmfiKDOlyzG4OiIjNLh9
+vVYiQJ3q9HsDrWj8soFPmNB06o3lfc1jw6P23pLCWBnglrvFxKk9pXSW/q/5iaq9
+lRdU2HhE8Qx3FZLgmEKnpNaqIJLNwaCzlrI6hEKNfdWV5Nbb6WLEWLN5xYzTNTOD
+n3WhUidhOPFZPY5Q4L15POdslv5e2QJltI5c0BE0312/UqeBAMN/mUWZFdUXyApT
+7GPzmX3MaRKGwhfwAZ6/hLzRUssbkmbOpFPlob/E2wnW5olWK8jjfN7j/4nlNW4o
+6GwLI1GpJQXrSPjdscr6bAhR77cYbETKJuFzxokGgeWKrLDiKca5JLNrRBH0pUPC
+TEPlcDaMtjNXepUugqD0XBCzYYP2AgWGLnwtbNwDRm41k9V6lS/eINhbfpSQBGq6
+WT0EBXWdN6IOLj3rwaRSg/7Qa9RmjtzG6RJOHSpXqhC8fF6CfaamyfItufUXJ63R
+DolUK5X6wK0dmBR4M0KGCqlztft0DbcbMBnEWg4cJ7faGND/isgFuvGqHKI3t+ZI
+pEYslOqodmJHixBTB0hXbOKSTbauBcvcwUpej6w9GU7C7WB1K9vBykLVAgMBAAGj
+YzBhMB8GA1UdIwQYMBaAFHKs5DN5qkWH9v2sHZ7Wxy+G2CQ5MB0GA1UdDgQWBBRy
+rOQzeapFh/b9rB2e1scvhtgkOTAOBgNVHQ8BAf8EBAMCAQYwDwYDVR0TAQH/BAUw
+AwEB/zANBgkqhkiG9w0BAQsFAAOCAgEAoDtZpwmUPjaE0n4vOaWWl/oRrfxn83EJ
+8rKJhGdEr7nv7ZbsnGTbMjBvZ5qsfl+yqwE2foH65IRe0qw24GtixX1LDoJt0nZi
+0f6X+J8wfBj5tFJ3gh1229MdqfDBmgC9bXXYfef6xzijnHDoRnkDry5023X4blMM
+A8iZGok1GTzTyVR8qPAs5m4HeW9q4ebqkYJpCh3DflminmtGFZhb069GHWLIzoBS
+SRE/yQQSwxN8PzuKlts8oB4KtItUsiRnDe+Cy748fdHif64W1lZYudogsYMVoe+K
+TTJvQS8TUoKU1xrBeKJR3Stwbbca+few4GeXVtt8YVMJAygCQMez2P2ccGrGKMOF
+6eLtGpOg3kuYooQ+BXcBlj37tCAPnHICehIv1aO6UXivKitEZU61/Qrowc15h2Er
+3oBXRb9n8ZuRXqWk7FlIEA04x7D6w0RtBPV4UBySllva9bguulvP5fBqnUsvWHMt
+Ty3EHD70sz+rFQ47GUGKpMFXEmZxTPpT41frYpUJnlTd0cI8Vzy9OK2YZLe4A5pT
+VmBds9hCG1xLEooc6+t9xnppxyd/pPiL8uSUZodL6ZQHCRJ5irLrdATczvREWeAW
+ysUsWNc8e89ihmpQfTU2Zqf7N+cox9jQraVplI/owd8k+BsHMYeB2F326CjYSlKA
+rBPuUBQemMc=
+-----END CERTIFICATE-----
+
+# Issuer: CN=D-TRUST BR Root CA 1 2020 O=D-Trust GmbH
+# Subject: CN=D-TRUST BR Root CA 1 2020 O=D-Trust GmbH
+# Label: "D-TRUST BR Root CA 1 2020"
+# Serial: 165870826978392376648679885835942448534
+# MD5 Fingerprint: b5:aa:4b:d5:ed:f7:e3:55:2e:8f:72:0a:f3:75:b8:ed
+# SHA1 Fingerprint: 1f:5b:98:f0:e3:b5:f7:74:3c:ed:e6:b0:36:7d:32:cd:f4:09:41:67
+# SHA256 Fingerprint: e5:9a:aa:81:60:09:c2:2b:ff:5b:25:ba:d3:7d:f3:06:f0:49:79:7c:1f:81:d8:5a:b0:89:e6:57:bd:8f:00:44
+-----BEGIN CERTIFICATE-----
+MIIC2zCCAmCgAwIBAgIQfMmPK4TX3+oPyWWa00tNljAKBggqhkjOPQQDAzBIMQsw
+CQYDVQQGEwJERTEVMBMGA1UEChMMRC1UcnVzdCBHbWJIMSIwIAYDVQQDExlELVRS
+VVNUIEJSIFJvb3QgQ0EgMSAyMDIwMB4XDTIwMDIxMTA5NDUwMFoXDTM1MDIxMTA5
+NDQ1OVowSDELMAkGA1UEBhMCREUxFTATBgNVBAoTDEQtVHJ1c3QgR21iSDEiMCAG
+A1UEAxMZRC1UUlVTVCBCUiBSb290IENBIDEgMjAyMDB2MBAGByqGSM49AgEGBSuB
+BAAiA2IABMbLxyjR+4T1mu9CFCDhQ2tuda38KwOE1HaTJddZO0Flax7mNCq7dPYS
+zuht56vkPE4/RAiLzRZxy7+SmfSk1zxQVFKQhYN4lGdnoxwJGT11NIXe7WB9xwy0
+QVK5buXuQqOCAQ0wggEJMA8GA1UdEwEB/wQFMAMBAf8wHQYDVR0OBBYEFHOREKv/
+VbNafAkl1bK6CKBrqx9tMA4GA1UdDwEB/wQEAwIBBjCBxgYDVR0fBIG+MIG7MD6g
+PKA6hjhodHRwOi8vY3JsLmQtdHJ1c3QubmV0L2NybC9kLXRydXN0X2JyX3Jvb3Rf
+Y2FfMV8yMDIwLmNybDB5oHegdYZzbGRhcDovL2RpcmVjdG9yeS5kLXRydXN0Lm5l
+dC9DTj1ELVRSVVNUJTIwQlIlMjBSb290JTIwQ0ElMjAxJTIwMjAyMCxPPUQtVHJ1
+c3QlMjBHbWJILEM9REU/Y2VydGlmaWNhdGVyZXZvY2F0aW9ubGlzdDAKBggqhkjO
+PQQDAwNpADBmAjEAlJAtE/rhY/hhY+ithXhUkZy4kzg+GkHaQBZTQgjKL47xPoFW
+wKrY7RjEsK70PvomAjEA8yjixtsrmfu3Ubgko6SUeho/5jbiA1czijDLgsfWFBHV
+dWNbFJWcHwHP2NVypw87
+-----END CERTIFICATE-----
+
+# Issuer: CN=D-TRUST EV Root CA 1 2020 O=D-Trust GmbH
+# Subject: CN=D-TRUST EV Root CA 1 2020 O=D-Trust GmbH
+# Label: "D-TRUST EV Root CA 1 2020"
+# Serial: 126288379621884218666039612629459926992
+# MD5 Fingerprint: 8c:2d:9d:70:9f:48:99:11:06:11:fb:e9:cb:30:c0:6e
+# SHA1 Fingerprint: 61:db:8c:21:59:69:03:90:d8:7c:9c:12:86:54:cf:9d:3d:f4:dd:07
+# SHA256 Fingerprint: 08:17:0d:1a:a3:64:53:90:1a:2f:95:92:45:e3:47:db:0c:8d:37:ab:aa:bc:56:b8:1a:a1:00:dc:95:89:70:db
+-----BEGIN CERTIFICATE-----
+MIIC2zCCAmCgAwIBAgIQXwJB13qHfEwDo6yWjfv/0DAKBggqhkjOPQQDAzBIMQsw
+CQYDVQQGEwJERTEVMBMGA1UEChMMRC1UcnVzdCBHbWJIMSIwIAYDVQQDExlELVRS
+VVNUIEVWIFJvb3QgQ0EgMSAyMDIwMB4XDTIwMDIxMTEwMDAwMFoXDTM1MDIxMTA5
+NTk1OVowSDELMAkGA1UEBhMCREUxFTATBgNVBAoTDEQtVHJ1c3QgR21iSDEiMCAG
+A1UEAxMZRC1UUlVTVCBFViBSb290IENBIDEgMjAyMDB2MBAGByqGSM49AgEGBSuB
+BAAiA2IABPEL3YZDIBnfl4XoIkqbz52Yv7QFJsnL46bSj8WeeHsxiamJrSc8ZRCC
+/N/DnU7wMyPE0jL1HLDfMxddxfCxivnvubcUyilKwg+pf3VlSSowZ/Rk99Yad9rD
+wpdhQntJraOCAQ0wggEJMA8GA1UdEwEB/wQFMAMBAf8wHQYDVR0OBBYEFH8QARY3
+OqQo5FD4pPfsazK2/umLMA4GA1UdDwEB/wQEAwIBBjCBxgYDVR0fBIG+MIG7MD6g
+PKA6hjhodHRwOi8vY3JsLmQtdHJ1c3QubmV0L2NybC9kLXRydXN0X2V2X3Jvb3Rf
+Y2FfMV8yMDIwLmNybDB5oHegdYZzbGRhcDovL2RpcmVjdG9yeS5kLXRydXN0Lm5l
+dC9DTj1ELVRSVVNUJTIwRVYlMjBSb290JTIwQ0ElMjAxJTIwMjAyMCxPPUQtVHJ1
+c3QlMjBHbWJILEM9REU/Y2VydGlmaWNhdGVyZXZvY2F0aW9ubGlzdDAKBggqhkjO
+PQQDAwNpADBmAjEAyjzGKnXCXnViOTYAYFqLwZOZzNnbQTs7h5kXO9XMT8oi96CA
+y/m0sRtW9XLS/BnRAjEAkfcwkz8QRitxpNA7RJvAKQIFskF3UfN5Wp6OFKBOQtJb
+gfM0agPnIjhQW+0ZT0MW
+-----END CERTIFICATE-----
+
+# Issuer: CN=DigiCert TLS ECC P384 Root G5 O=DigiCert, Inc.
+# Subject: CN=DigiCert TLS ECC P384 Root G5 O=DigiCert, Inc.
+# Label: "DigiCert TLS ECC P384 Root G5"
+# Serial: 13129116028163249804115411775095713523
+# MD5 Fingerprint: d3:71:04:6a:43:1c:db:a6:59:e1:a8:a3:aa:c5:71:ed
+# SHA1 Fingerprint: 17:f3:de:5e:9f:0f:19:e9:8e:f6:1f:32:26:6e:20:c4:07:ae:30:ee
+# SHA256 Fingerprint: 01:8e:13:f0:77:25:32:cf:80:9b:d1:b1:72:81:86:72:83:fc:48:c6:e1:3b:e9:c6:98:12:85:4a:49:0c:1b:05
+-----BEGIN CERTIFICATE-----
+MIICGTCCAZ+gAwIBAgIQCeCTZaz32ci5PhwLBCou8zAKBggqhkjOPQQDAzBOMQsw
+CQYDVQQGEwJVUzEXMBUGA1UEChMORGlnaUNlcnQsIEluYy4xJjAkBgNVBAMTHURp
+Z2lDZXJ0IFRMUyBFQ0MgUDM4NCBSb290IEc1MB4XDTIxMDExNTAwMDAwMFoXDTQ2
+MDExNDIzNTk1OVowTjELMAkGA1UEBhMCVVMxFzAVBgNVBAoTDkRpZ2lDZXJ0LCBJ
+bmMuMSYwJAYDVQQDEx1EaWdpQ2VydCBUTFMgRUNDIFAzODQgUm9vdCBHNTB2MBAG
+ByqGSM49AgEGBSuBBAAiA2IABMFEoc8Rl1Ca3iOCNQfN0MsYndLxf3c1TzvdlHJS
+7cI7+Oz6e2tYIOyZrsn8aLN1udsJ7MgT9U7GCh1mMEy7H0cKPGEQQil8pQgO4CLp
+0zVozptjn4S1mU1YoI71VOeVyaNCMEAwHQYDVR0OBBYEFMFRRVBZqz7nLFr6ICIS
+B4CIfBFqMA4GA1UdDwEB/wQEAwIBhjAPBgNVHRMBAf8EBTADAQH/MAoGCCqGSM49
+BAMDA2gAMGUCMQCJao1H5+z8blUD2WdsJk6Dxv3J+ysTvLd6jLRl0mlpYxNjOyZQ
+LgGheQaRnUi/wr4CMEfDFXuxoJGZSZOoPHzoRgaLLPIxAJSdYsiJvRmEFOml+wG4
+DXZDjC5Ty3zfDBeWUA==
+-----END CERTIFICATE-----
+
+# Issuer: CN=DigiCert TLS RSA4096 Root G5 O=DigiCert, Inc.
+# Subject: CN=DigiCert TLS RSA4096 Root G5 O=DigiCert, Inc.
+# Label: "DigiCert TLS RSA4096 Root G5"
+# Serial: 11930366277458970227240571539258396554
+# MD5 Fingerprint: ac:fe:f7:34:96:a9:f2:b3:b4:12:4b:e4:27:41:6f:e1
+# SHA1 Fingerprint: a7:88:49:dc:5d:7c:75:8c:8c:de:39:98:56:b3:aa:d0:b2:a5:71:35
+# SHA256 Fingerprint: 37:1a:00:dc:05:33:b3:72:1a:7e:eb:40:e8:41:9e:70:79:9d:2b:0a:0f:2c:1d:80:69:31:65:f7:ce:c4:ad:75
+-----BEGIN CERTIFICATE-----
+MIIFZjCCA06gAwIBAgIQCPm0eKj6ftpqMzeJ3nzPijANBgkqhkiG9w0BAQwFADBN
+MQswCQYDVQQGEwJVUzEXMBUGA1UEChMORGlnaUNlcnQsIEluYy4xJTAjBgNVBAMT
+HERpZ2lDZXJ0IFRMUyBSU0E0MDk2IFJvb3QgRzUwHhcNMjEwMTE1MDAwMDAwWhcN
+NDYwMTE0MjM1OTU5WjBNMQswCQYDVQQGEwJVUzEXMBUGA1UEChMORGlnaUNlcnQs
+IEluYy4xJTAjBgNVBAMTHERpZ2lDZXJ0IFRMUyBSU0E0MDk2IFJvb3QgRzUwggIi
+MA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQCz0PTJeRGd/fxmgefM1eS87IE+
+ajWOLrfn3q/5B03PMJ3qCQuZvWxX2hhKuHisOjmopkisLnLlvevxGs3npAOpPxG0
+2C+JFvuUAT27L/gTBaF4HI4o4EXgg/RZG5Wzrn4DReW+wkL+7vI8toUTmDKdFqgp
+wgscONyfMXdcvyej/Cestyu9dJsXLfKB2l2w4SMXPohKEiPQ6s+d3gMXsUJKoBZM
+pG2T6T867jp8nVid9E6P/DsjyG244gXazOvswzH016cpVIDPRFtMbzCe88zdH5RD
+nU1/cHAN1DrRN/BsnZvAFJNY781BOHW8EwOVfH/jXOnVDdXifBBiqmvwPXbzP6Po
+sMH976pXTayGpxi0KcEsDr9kvimM2AItzVwv8n/vFfQMFawKsPHTDU9qTXeXAaDx
+Zre3zu/O7Oyldcqs4+Fj97ihBMi8ez9dLRYiVu1ISf6nL3kwJZu6ay0/nTvEF+cd
+Lvvyz6b84xQslpghjLSR6Rlgg/IwKwZzUNWYOwbpx4oMYIwo+FKbbuH2TbsGJJvX
+KyY//SovcfXWJL5/MZ4PbeiPT02jP/816t9JXkGPhvnxd3lLG7SjXi/7RgLQZhNe
+XoVPzthwiHvOAbWWl9fNff2C+MIkwcoBOU+NosEUQB+cZtUMCUbW8tDRSHZWOkPL
+tgoRObqME2wGtZ7P6wIDAQABo0IwQDAdBgNVHQ4EFgQUUTMc7TZArxfTJc1paPKv
+TiM+s0EwDgYDVR0PAQH/BAQDAgGGMA8GA1UdEwEB/wQFMAMBAf8wDQYJKoZIhvcN
+AQEMBQADggIBAGCmr1tfV9qJ20tQqcQjNSH/0GEwhJG3PxDPJY7Jv0Y02cEhJhxw
+GXIeo8mH/qlDZJY6yFMECrZBu8RHANmfGBg7sg7zNOok992vIGCukihfNudd5N7H
+PNtQOa27PShNlnx2xlv0wdsUpasZYgcYQF+Xkdycx6u1UQ3maVNVzDl92sURVXLF
+O4uJ+DQtpBflF+aZfTCIITfNMBc9uPK8qHWgQ9w+iUuQrm0D4ByjoJYJu32jtyoQ
+REtGBzRj7TG5BO6jm5qu5jF49OokYTurWGT/u4cnYiWB39yhL/btp/96j1EuMPik
+AdKFOV8BmZZvWltwGUb+hmA+rYAQCd05JS9Yf7vSdPD3Rh9GOUrYU9DzLjtxpdRv
+/PNn5AeP3SYZ4Y1b+qOTEZvpyDrDVWiakuFSdjjo4bq9+0/V77PnSIMx8IIh47a+
+p6tv75/fTM8BuGJqIz3nCU2AG3swpMPdB380vqQmsvZB6Akd4yCYqjdP//fx4ilw
+MUc/dNAUFvohigLVigmUdy7yWSiLfFCSCmZ4OIN1xLVaqBHG5cGdZlXPU8Sv13WF
+qUITVuwhd4GTWgzqltlJyqEI8pc7bZsEGCREjnwB8twl2F6GmrE52/WRMmrRpnCK
+ovfepEWFJqgejF0pW8hL2JpqA15w8oVPbEtoL8pU9ozaMv7Da4M/OMZ+
+-----END CERTIFICATE-----
+
+# Issuer: CN=Certainly Root R1 O=Certainly
+# Subject: CN=Certainly Root R1 O=Certainly
+# Label: "Certainly Root R1"
+# Serial: 188833316161142517227353805653483829216
+# MD5 Fingerprint: 07:70:d4:3e:82:87:a0:fa:33:36:13:f4:fa:33:e7:12
+# SHA1 Fingerprint: a0:50:ee:0f:28:71:f4:27:b2:12:6d:6f:50:96:25:ba:cc:86:42:af
+# SHA256 Fingerprint: 77:b8:2c:d8:64:4c:43:05:f7:ac:c5:cb:15:6b:45:67:50:04:03:3d:51:c6:0c:62:02:a8:e0:c3:34:67:d3:a0
+-----BEGIN CERTIFICATE-----
+MIIFRzCCAy+gAwIBAgIRAI4P+UuQcWhlM1T01EQ5t+AwDQYJKoZIhvcNAQELBQAw
+PTELMAkGA1UEBhMCVVMxEjAQBgNVBAoTCUNlcnRhaW5seTEaMBgGA1UEAxMRQ2Vy
+dGFpbmx5IFJvb3QgUjEwHhcNMjEwNDAxMDAwMDAwWhcNNDYwNDAxMDAwMDAwWjA9
+MQswCQYDVQQGEwJVUzESMBAGA1UEChMJQ2VydGFpbmx5MRowGAYDVQQDExFDZXJ0
+YWlubHkgUm9vdCBSMTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBANA2
+1B/q3avk0bbm+yLA3RMNansiExyXPGhjZjKcA7WNpIGD2ngwEc/csiu+kr+O5MQT
+vqRoTNoCaBZ0vrLdBORrKt03H2As2/X3oXyVtwxwhi7xOu9S98zTm/mLvg7fMbed
+aFySpvXl8wo0tf97ouSHocavFwDvA5HtqRxOcT3Si2yJ9HiG5mpJoM610rCrm/b0
+1C7jcvk2xusVtyWMOvwlDbMicyF0yEqWYZL1LwsYpfSt4u5BvQF5+paMjRcCMLT5
+r3gajLQ2EBAHBXDQ9DGQilHFhiZ5shGIXsXwClTNSaa/ApzSRKft43jvRl5tcdF5
+cBxGX1HpyTfcX35pe0HfNEXgO4T0oYoKNp43zGJS4YkNKPl6I7ENPT2a/Z2B7yyQ
+wHtETrtJ4A5KVpK8y7XdeReJkd5hiXSSqOMyhb5OhaRLWcsrxXiOcVTQAjeZjOVJ
+6uBUcqQRBi8LjMFbvrWhsFNunLhgkR9Za/kt9JQKl7XsxXYDVBtlUrpMklZRNaBA
+2CnbrlJ2Oy0wQJuK0EJWtLeIAaSHO1OWzaMWj/Nmqhexx2DgwUMFDO6bW2BvBlyH
+Wyf5QBGenDPBt+U1VwV/J84XIIwc/PH72jEpSe31C4SnT8H2TsIonPru4K8H+zMR
+eiFPCyEQtkA6qyI6BJyLm4SGcprSp6XEtHWRqSsjAgMBAAGjQjBAMA4GA1UdDwEB
+/wQEAwIBBjAPBgNVHRMBAf8EBTADAQH/MB0GA1UdDgQWBBTgqj8ljZ9EXME66C6u
+d0yEPmcM9DANBgkqhkiG9w0BAQsFAAOCAgEAuVevuBLaV4OPaAszHQNTVfSVcOQr
+PbA56/qJYv331hgELyE03fFo8NWWWt7CgKPBjcZq91l3rhVkz1t5BXdm6ozTaw3d
+8VkswTOlMIAVRQdFGjEitpIAq5lNOo93r6kiyi9jyhXWx8bwPWz8HA2YEGGeEaIi
+1wrykXprOQ4vMMM2SZ/g6Q8CRFA3lFV96p/2O7qUpUzpvD5RtOjKkjZUbVwlKNrd
+rRT90+7iIgXr0PK3aBLXWopBGsaSpVo7Y0VPv+E6dyIvXL9G+VoDhRNCX8reU9di
+taY1BMJH/5n9hN9czulegChB8n3nHpDYT3Y+gjwN/KUD+nsa2UUeYNrEjvn8K8l7
+lcUq/6qJ34IxD3L/DCfXCh5WAFAeDJDBlrXYFIW7pw0WwfgHJBu6haEaBQmAupVj
+yTrsJZ9/nbqkRxWbRHDxakvWOF5D8xh+UG7pWijmZeZ3Gzr9Hb4DJqPb1OG7fpYn
+Kx3upPvaJVQTA945xsMfTZDsjxtK0hzthZU4UHlG1sGQUDGpXJpuHfUzVounmdLy
+yCwzk5Iwx06MZTMQZBf9JBeW0Y3COmor6xOLRPIh80oat3df1+2IpHLlOR+Vnb5n
+wXARPbv0+Em34yaXOp/SX3z7wJl8OSngex2/DaeP0ik0biQVy96QXr8axGbqwua6
+OV+KmalBWQewLK8=
+-----END CERTIFICATE-----
+
+# Issuer: CN=Certainly Root E1 O=Certainly
+# Subject: CN=Certainly Root E1 O=Certainly
+# Label: "Certainly Root E1"
+# Serial: 8168531406727139161245376702891150584
+# MD5 Fingerprint: 0a:9e:ca:cd:3e:52:50:c6:36:f3:4b:a3:ed:a7:53:e9
+# SHA1 Fingerprint: f9:e1:6d:dc:01:89:cf:d5:82:45:63:3e:c5:37:7d:c2:eb:93:6f:2b
+# SHA256 Fingerprint: b4:58:5f:22:e4:ac:75:6a:4e:86:12:a1:36:1c:5d:9d:03:1a:93:fd:84:fe:bb:77:8f:a3:06:8b:0f:c4:2d:c2
+-----BEGIN CERTIFICATE-----
+MIIB9zCCAX2gAwIBAgIQBiUzsUcDMydc+Y2aub/M+DAKBggqhkjOPQQDAzA9MQsw
+CQYDVQQGEwJVUzESMBAGA1UEChMJQ2VydGFpbmx5MRowGAYDVQQDExFDZXJ0YWlu
+bHkgUm9vdCBFMTAeFw0yMTA0MDEwMDAwMDBaFw00NjA0MDEwMDAwMDBaMD0xCzAJ
+BgNVBAYTAlVTMRIwEAYDVQQKEwlDZXJ0YWlubHkxGjAYBgNVBAMTEUNlcnRhaW5s
+eSBSb290IEUxMHYwEAYHKoZIzj0CAQYFK4EEACIDYgAE3m/4fxzf7flHh4axpMCK
++IKXgOqPyEpeKn2IaKcBYhSRJHpcnqMXfYqGITQYUBsQ3tA3SybHGWCA6TS9YBk2
+QNYphwk8kXr2vBMj3VlOBF7PyAIcGFPBMdjaIOlEjeR2o0IwQDAOBgNVHQ8BAf8E
+BAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAdBgNVHQ4EFgQU8ygYy2R17ikq6+2uI1g4
+hevIIgcwCgYIKoZIzj0EAwMDaAAwZQIxALGOWiDDshliTd6wT99u0nCK8Z9+aozm
+ut6Dacpps6kFtZaSF4fC0urQe87YQVt8rgIwRt7qy12a7DLCZRawTDBcMPPaTnOG
+BtjOiQRINzf43TNRnXCve1XYAS59BWQOhriR
+-----END CERTIFICATE-----
+
+# Issuer: CN=E-Tugra Global Root CA RSA v3 O=E-Tugra EBG A.S. OU=E-Tugra Trust Center
+# Subject: CN=E-Tugra Global Root CA RSA v3 O=E-Tugra EBG A.S. OU=E-Tugra Trust Center
+# Label: "E-Tugra Global Root CA RSA v3"
+# Serial: 75951268308633135324246244059508261641472512052
+# MD5 Fingerprint: 22:be:10:f6:c2:f8:03:88:73:5f:33:29:47:28:47:a4
+# SHA1 Fingerprint: e9:a8:5d:22:14:52:1c:5b:aa:0a:b4:be:24:6a:23:8a:c9:ba:e2:a9
+# SHA256 Fingerprint: ef:66:b0:b1:0a:3c:db:9f:2e:36:48:c7:6b:d2:af:18:ea:d2:bf:e6:f1:17:65:5e:28:c4:06:0d:a1:a3:f4:c2
+-----BEGIN CERTIFICATE-----
+MIIF8zCCA9ugAwIBAgIUDU3FzRYilZYIfrgLfxUGNPt5EDQwDQYJKoZIhvcNAQEL
+BQAwgYAxCzAJBgNVBAYTAlRSMQ8wDQYDVQQHEwZBbmthcmExGTAXBgNVBAoTEEUt
+VHVncmEgRUJHIEEuUy4xHTAbBgNVBAsTFEUtVHVncmEgVHJ1c3QgQ2VudGVyMSYw
+JAYDVQQDEx1FLVR1Z3JhIEdsb2JhbCBSb290IENBIFJTQSB2MzAeFw0yMDAzMTgw
+OTA3MTdaFw00NTAzMTIwOTA3MTdaMIGAMQswCQYDVQQGEwJUUjEPMA0GA1UEBxMG
+QW5rYXJhMRkwFwYDVQQKExBFLVR1Z3JhIEVCRyBBLlMuMR0wGwYDVQQLExRFLVR1
+Z3JhIFRydXN0IENlbnRlcjEmMCQGA1UEAxMdRS1UdWdyYSBHbG9iYWwgUm9vdCBD
+QSBSU0EgdjMwggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQCiZvCJt3J7
+7gnJY9LTQ91ew6aEOErxjYG7FL1H6EAX8z3DeEVypi6Q3po61CBxyryfHUuXCscx
+uj7X/iWpKo429NEvx7epXTPcMHD4QGxLsqYxYdE0PD0xesevxKenhOGXpOhL9hd8
+7jwH7eKKV9y2+/hDJVDqJ4GohryPUkqWOmAalrv9c/SF/YP9f4RtNGx/ardLAQO/
+rWm31zLZ9Vdq6YaCPqVmMbMWPcLzJmAy01IesGykNz709a/r4d+ABs8qQedmCeFL
+l+d3vSFtKbZnwy1+7dZ5ZdHPOrbRsV5WYVB6Ws5OUDGAA5hH5+QYfERaxqSzO8bG
+wzrwbMOLyKSRBfP12baqBqG3q+Sx6iEUXIOk/P+2UNOMEiaZdnDpwA+mdPy70Bt4
+znKS4iicvObpCdg604nmvi533wEKb5b25Y08TVJ2Glbhc34XrD2tbKNSEhhw5oBO
+M/J+JjKsBY04pOZ2PJ8QaQ5tndLBeSBrW88zjdGUdjXnXVXHt6woq0bM5zshtQoK
+5EpZ3IE1S0SVEgpnpaH/WwAH0sDM+T/8nzPyAPiMbIedBi3x7+PmBvrFZhNb/FAH
+nnGGstpvdDDPk1Po3CLW3iAfYY2jLqN4MpBs3KwytQXk9TwzDdbgh3cXTJ2w2Amo
+DVf3RIXwyAS+XF1a4xeOVGNpf0l0ZAWMowIDAQABo2MwYTAPBgNVHRMBAf8EBTAD
+AQH/MB8GA1UdIwQYMBaAFLK0ruYt9ybVqnUtdkvAG1Mh0EjvMB0GA1UdDgQWBBSy
+tK7mLfcm1ap1LXZLwBtTIdBI7zAOBgNVHQ8BAf8EBAMCAQYwDQYJKoZIhvcNAQEL
+BQADggIBAImocn+M684uGMQQgC0QDP/7FM0E4BQ8Tpr7nym/Ip5XuYJzEmMmtcyQ
+6dIqKe6cLcwsmb5FJ+Sxce3kOJUxQfJ9emN438o2Fi+CiJ+8EUdPdk3ILY7r3y18
+Tjvarvbj2l0Upq7ohUSdBm6O++96SmotKygY/r+QLHUWnw/qln0F7psTpURs+APQ
+3SPh/QMSEgj0GDSz4DcLdxEBSL9htLX4GdnLTeqjjO/98Aa1bZL0SmFQhO3sSdPk
+vmjmLuMxC1QLGpLWgti2omU8ZgT5Vdps+9u1FGZNlIM7zR6mK7L+d0CGq+ffCsn9
+9t2HVhjYsCxVYJb6CH5SkPVLpi6HfMsg2wY+oF0Dd32iPBMbKaITVaA9FCKvb7jQ
+mhty3QUBjYZgv6Rn7rWlDdF/5horYmbDB7rnoEgcOMPpRfunf/ztAmgayncSd6YA
+VSgU7NbHEqIbZULpkejLPoeJVF3Zr52XnGnnCv8PWniLYypMfUeUP95L6VPQMPHF
+9p5J3zugkaOj/s1YzOrfr28oO6Bpm4/srK4rVJ2bBLFHIK+WEj5jlB0E5y67hscM
+moi/dkfv97ALl2bSRM9gUgfh1SxKOidhd8rXj+eHDjD/DLsE4mHDosiXYY60MGo8
+bcIHX0pzLz/5FooBZu+6kcpSV3uu1OYP3Qt6f4ueJiDPO++BcYNZ
+-----END CERTIFICATE-----
+
+# Issuer: CN=E-Tugra Global Root CA ECC v3 O=E-Tugra EBG A.S. OU=E-Tugra Trust Center
+# Subject: CN=E-Tugra Global Root CA ECC v3 O=E-Tugra EBG A.S. OU=E-Tugra Trust Center
+# Label: "E-Tugra Global Root CA ECC v3"
+# Serial: 218504919822255052842371958738296604628416471745
+# MD5 Fingerprint: 46:bc:81:bb:f1:b5:1e:f7:4b:96:bc:14:e2:e7:27:64
+# SHA1 Fingerprint: 8a:2f:af:57:53:b1:b0:e6:a1:04:ec:5b:6a:69:71:6d:f6:1c:e2:84
+# SHA256 Fingerprint: 87:3f:46:85:fa:7f:56:36:25:25:2e:6d:36:bc:d7:f1:6f:c2:49:51:f2:64:e4:7e:1b:95:4f:49:08:cd:ca:13
+-----BEGIN CERTIFICATE-----
+MIICpTCCAiqgAwIBAgIUJkYZdzHhT28oNt45UYbm1JeIIsEwCgYIKoZIzj0EAwMw
+gYAxCzAJBgNVBAYTAlRSMQ8wDQYDVQQHEwZBbmthcmExGTAXBgNVBAoTEEUtVHVn
+cmEgRUJHIEEuUy4xHTAbBgNVBAsTFEUtVHVncmEgVHJ1c3QgQ2VudGVyMSYwJAYD
+VQQDEx1FLVR1Z3JhIEdsb2JhbCBSb290IENBIEVDQyB2MzAeFw0yMDAzMTgwOTQ2
+NThaFw00NTAzMTIwOTQ2NThaMIGAMQswCQYDVQQGEwJUUjEPMA0GA1UEBxMGQW5r
+YXJhMRkwFwYDVQQKExBFLVR1Z3JhIEVCRyBBLlMuMR0wGwYDVQQLExRFLVR1Z3Jh
+IFRydXN0IENlbnRlcjEmMCQGA1UEAxMdRS1UdWdyYSBHbG9iYWwgUm9vdCBDQSBF
+Q0MgdjMwdjAQBgcqhkjOPQIBBgUrgQQAIgNiAASOmCm/xxAeJ9urA8woLNheSBkQ
+KczLWYHMjLiSF4mDKpL2w6QdTGLVn9agRtwcvHbB40fQWxPa56WzZkjnIZpKT4YK
+fWzqTTKACrJ6CZtpS5iB4i7sAnCWH/31Rs7K3IKjYzBhMA8GA1UdEwEB/wQFMAMB
+Af8wHwYDVR0jBBgwFoAU/4Ixcj75xGZsrTie0bBRiKWQzPUwHQYDVR0OBBYEFP+C
+MXI++cRmbK04ntGwUYilkMz1MA4GA1UdDwEB/wQEAwIBBjAKBggqhkjOPQQDAwNp
+ADBmAjEA5gVYaWHlLcoNy/EZCL3W/VGSGn5jVASQkZo1kTmZ+gepZpO6yGjUij/6
+7W4WAie3AjEA3VoXK3YdZUKWpqxdinlW2Iob35reX8dQj7FbcQwm32pAAOwzkSFx
+vmjkI6TZraE3
+-----END CERTIFICATE-----
+
+# Issuer: CN=Security Communication RootCA3 O=SECOM Trust Systems CO.,LTD.
+# Subject: CN=Security Communication RootCA3 O=SECOM Trust Systems CO.,LTD.
+# Label: "Security Communication RootCA3"
+# Serial: 16247922307909811815
+# MD5 Fingerprint: 1c:9a:16:ff:9e:5c:e0:4d:8a:14:01:f4:35:5d:29:26
+# SHA1 Fingerprint: c3:03:c8:22:74:92:e5:61:a2:9c:5f:79:91:2b:1e:44:13:91:30:3a
+# SHA256 Fingerprint: 24:a5:5c:2a:b0:51:44:2d:06:17:76:65:41:23:9a:4a:d0:32:d7:c5:51:75:aa:34:ff:de:2f:bc:4f:5c:52:94
+-----BEGIN CERTIFICATE-----
+MIIFfzCCA2egAwIBAgIJAOF8N0D9G/5nMA0GCSqGSIb3DQEBDAUAMF0xCzAJBgNV
+BAYTAkpQMSUwIwYDVQQKExxTRUNPTSBUcnVzdCBTeXN0ZW1zIENPLixMVEQuMScw
+JQYDVQQDEx5TZWN1cml0eSBDb21tdW5pY2F0aW9uIFJvb3RDQTMwHhcNMTYwNjE2
+MDYxNzE2WhcNMzgwMTE4MDYxNzE2WjBdMQswCQYDVQQGEwJKUDElMCMGA1UEChMc
+U0VDT00gVHJ1c3QgU3lzdGVtcyBDTy4sTFRELjEnMCUGA1UEAxMeU2VjdXJpdHkg
+Q29tbXVuaWNhdGlvbiBSb290Q0EzMIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIIC
+CgKCAgEA48lySfcw3gl8qUCBWNO0Ot26YQ+TUG5pPDXC7ltzkBtnTCHsXzW7OT4r
+CmDvu20rhvtxosis5FaU+cmvsXLUIKx00rgVrVH+hXShuRD+BYD5UpOzQD11EKzA
+lrenfna84xtSGc4RHwsENPXY9Wk8d/Nk9A2qhd7gCVAEF5aEt8iKvE1y/By7z/MG
+TfmfZPd+pmaGNXHIEYBMwXFAWB6+oHP2/D5Q4eAvJj1+XCO1eXDe+uDRpdYMQXF7
+9+qMHIjH7Iv10S9VlkZ8WjtYO/u62C21Jdp6Ts9EriGmnpjKIG58u4iFW/vAEGK7
+8vknR+/RiTlDxN/e4UG/VHMgly1s2vPUB6PmudhvrvyMGS7TZ2crldtYXLVqAvO4
+g160a75BflcJdURQVc1aEWEhCmHCqYj9E7wtiS/NYeCVvsq1e+F7NGcLH7YMx3we
+GVPKp7FKFSBWFHA9K4IsD50VHUeAR/94mQ4xr28+j+2GaR57GIgUssL8gjMunEst
++3A7caoreyYn8xrC3PsXuKHqy6C0rtOUfnrQq8PsOC0RLoi/1D+tEjtCrI8Cbn3M
+0V9hvqG8OmpI6iZVIhZdXw3/JzOfGAN0iltSIEdrRU0id4xVJ/CvHozJgyJUt5rQ
+T9nO/NkuHJYosQLTA70lUhw0Zk8jq/R3gpYd0VcwCBEF/VfR2ccCAwEAAaNCMEAw
+HQYDVR0OBBYEFGQUfPxYchamCik0FW8qy7z8r6irMA4GA1UdDwEB/wQEAwIBBjAP
+BgNVHRMBAf8EBTADAQH/MA0GCSqGSIb3DQEBDAUAA4ICAQDcAiMI4u8hOscNtybS
+YpOnpSNyByCCYN8Y11StaSWSntkUz5m5UoHPrmyKO1o5yGwBQ8IibQLwYs1OY0PA
+FNr0Y/Dq9HHuTofjcan0yVflLl8cebsjqodEV+m9NU1Bu0soo5iyG9kLFwfl9+qd
+9XbXv8S2gVj/yP9kaWJ5rW4OH3/uHWnlt3Jxs/6lATWUVCvAUm2PVcTJ0rjLyjQI
+UYWg9by0F1jqClx6vWPGOi//lkkZhOpn2ASxYfQAW0q3nHE3GYV5v4GwxxMOdnE+
+OoAGrgYWp421wsTL/0ClXI2lyTrtcoHKXJg80jQDdwj98ClZXSEIx2C/pHF7uNke
+gr4Jr2VvKKu/S7XuPghHJ6APbw+LP6yVGPO5DtxnVW5inkYO0QR4ynKudtml+LLf
+iAlhi+8kTtFZP1rUPcmTPCtk9YENFpb3ksP+MW/oKjJ0DvRMmEoYDjBU1cXrvMUV
+nuiZIesnKwkK2/HmcBhWuwzkvvnoEKQTkrgc4NtnHVMDpCKn3F2SEDzq//wbEBrD
+2NCcnWXL0CsnMQMeNuE9dnUM/0Umud1RvCPHX9jYhxBAEg09ODfnRDwYwFMJZI//
+1ZqmfHAuc1Uh6N//g7kdPjIe1qZ9LPFm6Vwdp6POXiUyK+OVrCoHzrQoeIY8Laad
+TdJ0MN1kURXbg4NR16/9M51NZg==
+-----END CERTIFICATE-----
+
+# Issuer: CN=Security Communication ECC RootCA1 O=SECOM Trust Systems CO.,LTD.
+# Subject: CN=Security Communication ECC RootCA1 O=SECOM Trust Systems CO.,LTD.
+# Label: "Security Communication ECC RootCA1"
+# Serial: 15446673492073852651
+# MD5 Fingerprint: 7e:43:b0:92:68:ec:05:43:4c:98:ab:5d:35:2e:7e:86
+# SHA1 Fingerprint: b8:0e:26:a9:bf:d2:b2:3b:c0:ef:46:c9:ba:c7:bb:f6:1d:0d:41:41
+# SHA256 Fingerprint: e7:4f:bd:a5:5b:d5:64:c4:73:a3:6b:44:1a:a7:99:c8:a6:8e:07:74:40:e8:28:8b:9f:a1:e5:0e:4b:ba:ca:11
+-----BEGIN CERTIFICATE-----
+MIICODCCAb6gAwIBAgIJANZdm7N4gS7rMAoGCCqGSM49BAMDMGExCzAJBgNVBAYT
+AkpQMSUwIwYDVQQKExxTRUNPTSBUcnVzdCBTeXN0ZW1zIENPLixMVEQuMSswKQYD
+VQQDEyJTZWN1cml0eSBDb21tdW5pY2F0aW9uIEVDQyBSb290Q0ExMB4XDTE2MDYx
+NjA1MTUyOFoXDTM4MDExODA1MTUyOFowYTELMAkGA1UEBhMCSlAxJTAjBgNVBAoT
+HFNFQ09NIFRydXN0IFN5c3RlbXMgQ08uLExURC4xKzApBgNVBAMTIlNlY3VyaXR5
+IENvbW11bmljYXRpb24gRUNDIFJvb3RDQTEwdjAQBgcqhkjOPQIBBgUrgQQAIgNi
+AASkpW9gAwPDvTH00xecK4R1rOX9PVdu12O/5gSJko6BnOPpR27KkBLIE+Cnnfdl
+dB9sELLo5OnvbYUymUSxXv3MdhDYW72ixvnWQuRXdtyQwjWpS4g8EkdtXP9JTxpK
+ULGjQjBAMB0GA1UdDgQWBBSGHOf+LaVKiwj+KBH6vqNm+GBZLzAOBgNVHQ8BAf8E
+BAMCAQYwDwYDVR0TAQH/BAUwAwEB/zAKBggqhkjOPQQDAwNoADBlAjAVXUI9/Lbu
+9zuxNuie9sRGKEkz0FhDKmMpzE2xtHqiuQ04pV1IKv3LsnNdo4gIxwwCMQDAqy0O
+be0YottT6SXbVQjgUMzfRGEWgqtJsLKB7HOHeLRMsmIbEvoWTSVLY70eN9k=
+-----END CERTIFICATE-----
+
+# Issuer: CN=BJCA Global Root CA1 O=BEIJING CERTIFICATE AUTHORITY
+# Subject: CN=BJCA Global Root CA1 O=BEIJING CERTIFICATE AUTHORITY
+# Label: "BJCA Global Root CA1"
+# Serial: 113562791157148395269083148143378328608
+# MD5 Fingerprint: 42:32:99:76:43:33:36:24:35:07:82:9b:28:f9:d0:90
+# SHA1 Fingerprint: d5:ec:8d:7b:4c:ba:79:f4:e7:e8:cb:9d:6b:ae:77:83:10:03:21:6a
+# SHA256 Fingerprint: f3:89:6f:88:fe:7c:0a:88:27:66:a7:fa:6a:d2:74:9f:b5:7a:7f:3e:98:fb:76:9c:1f:a7:b0:9c:2c:44:d5:ae
+-----BEGIN CERTIFICATE-----
+MIIFdDCCA1ygAwIBAgIQVW9l47TZkGobCdFsPsBsIDANBgkqhkiG9w0BAQsFADBU
+MQswCQYDVQQGEwJDTjEmMCQGA1UECgwdQkVJSklORyBDRVJUSUZJQ0FURSBBVVRI
+T1JJVFkxHTAbBgNVBAMMFEJKQ0EgR2xvYmFsIFJvb3QgQ0ExMB4XDTE5MTIxOTAz
+MTYxN1oXDTQ0MTIxMjAzMTYxN1owVDELMAkGA1UEBhMCQ04xJjAkBgNVBAoMHUJF
+SUpJTkcgQ0VSVElGSUNBVEUgQVVUSE9SSVRZMR0wGwYDVQQDDBRCSkNBIEdsb2Jh
+bCBSb290IENBMTCCAiIwDQYJKoZIhvcNAQEBBQADggIPADCCAgoCggIBAPFmCL3Z
+xRVhy4QEQaVpN3cdwbB7+sN3SJATcmTRuHyQNZ0YeYjjlwE8R4HyDqKYDZ4/N+AZ
+spDyRhySsTphzvq3Rp4Dhtczbu33RYx2N95ulpH3134rhxfVizXuhJFyV9xgw8O5
+58dnJCNPYwpj9mZ9S1WnP3hkSWkSl+BMDdMJoDIwOvqfwPKcxRIqLhy1BDPapDgR
+at7GGPZHOiJBhyL8xIkoVNiMpTAK+BcWyqw3/XmnkRd4OJmtWO2y3syJfQOcs4ll
+5+M7sSKGjwZteAf9kRJ/sGsciQ35uMt0WwfCyPQ10WRjeulumijWML3mG90Vr4Tq
+nMfK9Q7q8l0ph49pczm+LiRvRSGsxdRpJQaDrXpIhRMsDQa4bHlW/KNnMoH1V6XK
+V0Jp6VwkYe/iMBhORJhVb3rCk9gZtt58R4oRTklH2yiUAguUSiz5EtBP6DF+bHq/
+pj+bOT0CFqMYs2esWz8sgytnOYFcuX6U1WTdno9uruh8W7TXakdI136z1C2OVnZO
+z2nxbkRs1CTqjSShGL+9V/6pmTW12xB3uD1IutbB5/EjPtffhZ0nPNRAvQoMvfXn
+jSXWgXSHRtQpdaJCbPdzied9v3pKH9MiyRVVz99vfFXQpIsHETdfg6YmV6YBW37+
+WGgHqel62bno/1Afq8K0wM7o6v0PvY1NuLxxAgMBAAGjQjBAMB0GA1UdDgQWBBTF
+7+3M2I0hxkjk49cULqcWk+WYATAPBgNVHRMBAf8EBTADAQH/MA4GA1UdDwEB/wQE
+AwIBBjANBgkqhkiG9w0BAQsFAAOCAgEAUoKsITQfI/Ki2Pm4rzc2IInRNwPWaZ+4
+YRC6ojGYWUfo0Q0lHhVBDOAqVdVXUsv45Mdpox1NcQJeXyFFYEhcCY5JEMEE3Kli
+awLwQ8hOnThJdMkycFRtwUf8jrQ2ntScvd0g1lPJGKm1Vrl2i5VnZu69mP6u775u
++2D2/VnGKhs/I0qUJDAnyIm860Qkmss9vk/Ves6OF8tiwdneHg56/0OGNFK8YT88
+X7vZdrRTvJez/opMEi4r89fO4aL/3Xtw+zuhTaRjAv04l5U/BXCga99igUOLtFkN
+SoxUnMW7gZ/NfaXvCyUeOiDbHPwfmGcCCtRzRBPbUYQaVQNW4AB+dAb/OMRyHdOo
+P2gxXdMJxy6MW2Pg6Nwe0uxhHvLe5e/2mXZgLR6UcnHGCyoyx5JO1UbXHfmpGQrI
++pXObSOYqgs4rZpWDW+N8TEAiMEXnM0ZNjX+VVOg4DwzX5Ze4jLp3zO7Bkqp2IRz
+znfSxqxx4VyjHQy7Ct9f4qNx2No3WqB4K/TUfet27fJhcKVlmtOJNBir+3I+17Q9
+eVzYH6Eze9mCUAyTF6ps3MKCuwJXNq+YJyo5UOGwifUll35HaBC07HPKs5fRJNz2
+YqAo07WjuGS3iGJCz51TzZm+ZGiPTx4SSPfSKcOYKMryMguTjClPPGAyzQWWYezy
+r/6zcCwupvI=
+-----END CERTIFICATE-----
+
+# Issuer: CN=BJCA Global Root CA2 O=BEIJING CERTIFICATE AUTHORITY
+# Subject: CN=BJCA Global Root CA2 O=BEIJING CERTIFICATE AUTHORITY
+# Label: "BJCA Global Root CA2"
+# Serial: 58605626836079930195615843123109055211
+# MD5 Fingerprint: 5e:0a:f6:47:5f:a6:14:e8:11:01:95:3f:4d:01:eb:3c
+# SHA1 Fingerprint: f4:27:86:eb:6e:b8:6d:88:31:67:02:fb:ba:66:a4:53:00:aa:7a:a6
+# SHA256 Fingerprint: 57:4d:f6:93:1e:27:80:39:66:7b:72:0a:fd:c1:60:0f:c2:7e:b6:6d:d3:09:29:79:fb:73:85:64:87:21:28:82
+-----BEGIN CERTIFICATE-----
+MIICJTCCAaugAwIBAgIQLBcIfWQqwP6FGFkGz7RK6zAKBggqhkjOPQQDAzBUMQsw
+CQYDVQQGEwJDTjEmMCQGA1UECgwdQkVJSklORyBDRVJUSUZJQ0FURSBBVVRIT1JJ
+VFkxHTAbBgNVBAMMFEJKQ0EgR2xvYmFsIFJvb3QgQ0EyMB4XDTE5MTIxOTAzMTgy
+MVoXDTQ0MTIxMjAzMTgyMVowVDELMAkGA1UEBhMCQ04xJjAkBgNVBAoMHUJFSUpJ
+TkcgQ0VSVElGSUNBVEUgQVVUSE9SSVRZMR0wGwYDVQQDDBRCSkNBIEdsb2JhbCBS
+b290IENBMjB2MBAGByqGSM49AgEGBSuBBAAiA2IABJ3LgJGNU2e1uVCxA/jlSR9B
+IgmwUVJY1is0j8USRhTFiy8shP8sbqjV8QnjAyEUxEM9fMEsxEtqSs3ph+B99iK+
++kpRuDCK/eHeGBIK9ke35xe/J4rUQUyWPGCWwf0VHKNCMEAwHQYDVR0OBBYEFNJK
+sVF/BvDRgh9Obl+rg/xI1LCRMA8GA1UdEwEB/wQFMAMBAf8wDgYDVR0PAQH/BAQD
+AgEGMAoGCCqGSM49BAMDA2gAMGUCMBq8W9f+qdJUDkpd0m2xQNz0Q9XSSpkZElaA
+94M04TVOSG0ED1cxMDAtsaqdAzjbBgIxAMvMh1PLet8gUXOQwKhbYdDFUDn9hf7B
+43j4ptZLvZuHjw/l1lOWqzzIQNph91Oj9w==
+-----END CERTIFICATE-----
```

### Comparing `djangosaml2-1.5.7/.tox/py3.6-django2.2/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `djangosaml2-1.5.8/env/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/CHANGES` & `djangosaml2-1.5.8/CHANGES`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/COPYING` & `djangosaml2-1.5.8/COPYING`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/PKG-INFO` & `djangosaml2-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.5.7
+Version: 1.5.8
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.5.7/README.md` & `djangosaml2-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/backends.py` & `djangosaml2-1.5.8/djangosaml2/backends.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/cache.py` & `djangosaml2-1.5.8/djangosaml2/cache.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/conf.py` & `djangosaml2-1.5.8/djangosaml2/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/middleware.py` & `djangosaml2-1.5.8/djangosaml2/middleware.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/overrides.py` & `djangosaml2-1.5.8/djangosaml2/overrides.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/signals.py` & `djangosaml2-1.5.8/djangosaml2/signals.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/templatetags/idplist.py` & `djangosaml2-1.5.8/djangosaml2/templatetags/idplist.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/tests/__init__.py` & `djangosaml2-1.5.8/djangosaml2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/django_saml_uri.py` & `djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/django_saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/tests/attribute-maps/saml_uri.py` & `djangosaml2-1.5.8/djangosaml2/tests/attribute-maps/saml_uri.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/tests/auth_response.py` & `djangosaml2-1.5.8/djangosaml2/tests/auth_response.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/tests/conf.py` & `djangosaml2-1.5.8/djangosaml2/tests/conf.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/urls.py` & `djangosaml2-1.5.8/djangosaml2/urls.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/utils.py` & `djangosaml2-1.5.8/djangosaml2/utils.py`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/djangosaml2/views.py` & `djangosaml2-1.5.8/djangosaml2/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,29 +170,31 @@
 
     def load_sso_kwargs(self, sso_kwargs):
         """Inherit me if you want to put your desidered things in sso_kwargs"""
 
     def add_idp_hinting(self, http_response):
         return add_idp_hinting(self.request, http_response) or http_response
 
-    def get(self, request, *args, **kwargs):
-        logger.debug("Login process started")
-        next_path = self.get_next_path(request)
-
-        # if the user is already authenticated that maybe because of two reasons:
+    def should_prevent_auth(self, request) -> bool:
+        # If the user is already authenticated that maybe because of two reasons:
         # A) He has this URL in two browser windows and in the other one he
         #    has already initiated the authenticated session.
         # B) He comes from a view that (incorrectly) send him here because
         #    he does not have enough permissions. That view should have shown
         #    an authorization error in the first place.
-        # We can only make one thing here and that is configurable with the
-        # SAML_IGNORE_AUTHENTICATED_USERS_ON_LOGIN setting. If that setting
-        # is True (default value) we will redirect him to the next_path path.
-        # Otherwise, we will show an (configurable) authorization error.
-        if request.user.is_authenticated:
+        return request.user.is_authenticated
+
+    def get(self, request, *args, **kwargs):
+        logger.debug("Login process started")
+        next_path = self.get_next_path(request)
+
+        if self.should_prevent_auth(request):
+            # If the SAML_IGNORE_AUTHENTICATED_USERS_ON_LOGIN setting is True
+            # (default value), redirect to the next_path. Otherwise, show a
+            # configurable authorization error.
             if get_custom_setting("SAML_IGNORE_AUTHENTICATED_USERS_ON_LOGIN", True):
                 return HttpResponseRedirect(next_path)
             logger.debug("User is already logged in")
             return render(
                 request,
                 self.authorization_error_template,
                 {
```

### Comparing `djangosaml2-1.5.7/djangosaml2.egg-info/PKG-INFO` & `djangosaml2-1.5.8/djangosaml2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml2
-Version: 1.5.7
+Version: 1.5.8
 Summary: pysaml2 integration for Django
 Home-page: https://github.com/IdentityPython/djangosaml2
 Download-URL: https://pypi.org/project/djangosaml2/
 Author: Yaco Sistemas and independent contributors
 Author-email: lorenzo.gil.sanchez@gmail.com
 Maintainer: Giuseppe De Marco
 License: Apache 2.0
```

### Comparing `djangosaml2-1.5.7/docs/source/_templates/pplnx_template/footer.html` & `djangosaml2-1.5.8/docs/source/_templates/pplnx_template/footer.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/docs/source/_templates/pplnx_template/layout.html` & `djangosaml2-1.5.8/docs/source/_templates/pplnx_template/layout.html`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml` & `djangosaml2-1.5.8/env/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml`

 * *Files identical despite different names*

### Comparing `djangosaml2-1.5.7/setup.py` & `djangosaml2-1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return codecs.open(
         os.path.join(os.path.dirname(__file__), *rnames), encoding="utf-8"
     ).read()
 
 
 setup(
     name="djangosaml2",
-    version="1.5.7",
+    version="1.5.8",
     description="pysaml2 integration for Django",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
```

