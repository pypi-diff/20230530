# Comparing `tmp/django-ipghrms-leave-1.1.tar.gz` & `tmp/django-ipghrms-leave-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-leave-1.1.tar", last modified: Mon Apr 10 06:02:52 2023, max compression
+gzip compressed data, was "dist\django-ipghrms-leave-1.2.tar", last modified: Tue May 30 20:04:54 2023, max compression
```

## Comparing `django-ipghrms-leave-1.1.tar` & `django-ipghrms-leave-1.2.tar`

### file list

```diff
@@ -1,355 +1,355 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:52.311910 django-ipghrms-leave-1.1/
--rw-rw-rw-   0        0        0     1065 2023-03-27 14:45:38.000000 django-ipghrms-leave-1.1/LICENSE
--rw-rw-rw-   0        0        0      214 2023-03-27 14:21:05.000000 django-ipghrms-leave-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      924 2023-04-10 06:02:52.311910 django-ipghrms-leave-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-03-27 14:21:43.000000 django-ipghrms-leave-1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:48.911491 django-ipghrms-leave-1.1/django_ipghrms_leave.egg-info/
--rw-rw-rw-   0        0        0      924 2023-04-10 06:02:48.000000 django-ipghrms-leave-1.1/django_ipghrms_leave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18263 2023-04-10 06:02:48.000000 django-ipghrms-leave-1.1/django_ipghrms_leave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 06:02:48.000000 django-ipghrms-leave-1.1/django_ipghrms_leave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-10 06:02:48.000000 django-ipghrms-leave-1.1/django_ipghrms_leave.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:48.990552 django-ipghrms-leave-1.1/leave/
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/__init__.py
--rw-rw-rw-   0        0        0      385 2022-12-20 08:39:46.000000 django-ipghrms-leave-1.1/leave/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:48.999508 django-ipghrms-leave-1.1/leave/api/
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:49.016108 django-ipghrms-leave-1.1/leave/api/__pycache__/
--rw-rw-rw-   0        0        0     1223 2023-02-05 08:06:39.000000 django-ipghrms-leave-1.1/leave/api/__pycache__/urls.cpython-310.pyc
--rw-rw-rw-   0        0        0     9993 2023-02-05 08:09:34.000000 django-ipghrms-leave-1.1/leave/api/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0     1189 2023-02-05 08:06:35.000000 django-ipghrms-leave-1.1/leave/api/urls.py
--rw-rw-rw-   0        0        0    13296 2023-02-05 08:09:31.000000 django-ipghrms-leave-1.1/leave/api/views.py
--rw-rw-rw-   0        0        0      178 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/apps.py
--rw-rw-rw-   0        0        0    11486 2023-03-15 10:07:35.000000 django-ipghrms-leave-1.1/leave/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:49.575194 django-ipghrms-leave-1.1/leave/migrations/
--rw-rw-rw-   0        0        0     4776 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      317 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0002_remove_taskdelegate_date.py
--rw-rw-rw-   0        0        0      450 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0003_rename_taskdelegate_leavedelegate.py
--rw-rw-rw-   0        0        0      619 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0004_alter_leavedelegate_employee.py
--rw-rw-rw-   0        0        0      384 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0005_rename_is_approve_leavedelegate_is_confirm.py
--rw-rw-rw-   0        0        0      430 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0006_leavedelegate_is_confirm2.py
--rw-rw-rw-   0        0        0      400 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0007_leavetype_total.py
--rw-rw-rw-   0        0        0      649 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0008_rename_de_confirm_leave_de_approve_and_more.py
--rw-rw-rw-   0        0        0      705 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0009_rename_is_lock_leave_s_is_finish_and_more.py
--rw-rw-rw-   0        0        0      980 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.py
--rw-rw-rw-   0        0        0     1507 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.py
--rw-rw-rw-   0        0        0      766 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0012_alter_leavedelegate_leave_alter_leaveunit_leave.py
--rw-rw-rw-   0        0        0      425 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0013_leave_is_finish.py
--rw-rw-rw-   0        0        0     2028 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0014_leavehr_leavede.py
--rw-rw-rw-   0        0        0     1198 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.py
--rw-rw-rw-   0        0        0      427 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0016_leave_is_print.py
--rw-rw-rw-   0        0        0      750 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.py
--rw-rw-rw-   0        0        0      464 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0018_alter_leavecount_balance.py
--rw-rw-rw-   0        0        0      406 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0019_leave_s_is_delegate.py
--rw-rw-rw-   0        0        0      331 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0020_remove_leave_s_is_delegate.py
--rw-rw-rw-   0        0        0      572 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0021_leave_is_approve_leave_is_reject.py
--rw-rw-rw-   0        0        0      664 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0022_rename_s_is_finish_leave_is_delegate_and_more.py
--rw-rw-rw-   0        0        0      359 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0023_remove_leavedelegate_is_send.py
--rw-rw-rw-   0        0        0      407 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/0024_alter_leave_is_active.py
--rw-rw-rw-   0        0        0      795 2022-12-10 14:29:58.000000 django-ipghrms-leave-1.1/leave/migrations/0025_auto_20221210_2329.py
--rw-rw-rw-   0        0        0      590 2022-12-10 14:56:41.000000 django-ipghrms-leave-1.1/leave/migrations/0026_auto_20221210_2356.py
--rw-rw-rw-   0        0        0      460 2022-12-10 15:22:16.000000 django-ipghrms-leave-1.1/leave/migrations/0027_auto_20221211_0022.py
--rw-rw-rw-   0        0        0      590 2022-12-10 17:02:09.000000 django-ipghrms-leave-1.1/leave/migrations/0028_auto_20221211_0202.py
--rw-rw-rw-   0        0        0     1255 2022-12-11 02:51:24.000000 django-ipghrms-leave-1.1/leave/migrations/0029_leavedep.py
--rw-rw-rw-   0        0        0      577 2022-12-11 03:06:33.000000 django-ipghrms-leave-1.1/leave/migrations/0030_auto_20221211_1206.py
--rw-rw-rw-   0        0        0      414 2022-12-11 04:16:56.000000 django-ipghrms-leave-1.1/leave/migrations/0031_leave_is_update.py
--rw-rw-rw-   0        0        0      413 2022-12-17 06:24:38.000000 django-ipghrms-leave-1.1/leave/migrations/0032_leave_dep_send_pr.py
--rw-rw-rw-   0        0        0      414 2022-12-17 06:40:11.000000 django-ipghrms-leave-1.1/leave/migrations/0033_leave_pr_confirm.py
--rw-rw-rw-   0        0        0      382 2022-12-17 06:43:34.000000 django-ipghrms-leave-1.1/leave/migrations/0034_rename_pr_confirm_leave_pr_approve.py
--rw-rw-rw-   0        0        0      652 2022-12-17 07:14:52.000000 django-ipghrms-leave-1.1/leave/migrations/0035_leave_file.py
--rw-rw-rw-   0        0        0      409 2022-12-17 08:47:37.000000 django-ipghrms-leave-1.1/leave/migrations/0036_leave_unit_send_pr.py
--rw-rw-rw-   0        0        0      445 2022-12-20 07:39:43.000000 django-ipghrms-leave-1.1/leave/migrations/0037_alter_leavetype_total.py
--rw-rw-rw-   0        0        0      416 2022-12-20 07:43:17.000000 django-ipghrms-leave-1.1/leave/migrations/0038_alter_leavetype_total.py
--rw-rw-rw-   0        0        0      448 2022-12-20 07:50:53.000000 django-ipghrms-leave-1.1/leave/migrations/0039_alter_leavetype_total.py
--rw-rw-rw-   0        0        0      475 2022-12-20 07:55:29.000000 django-ipghrms-leave-1.1/leave/migrations/0040_alter_leavecount_balance.py
--rw-rw-rw-   0        0        0      474 2022-12-20 07:55:59.000000 django-ipghrms-leave-1.1/leave/migrations/0041_alter_leavecount_total.py
--rw-rw-rw-   0        0        0      466 2022-12-20 07:56:29.000000 django-ipghrms-leave-1.1/leave/migrations/0042_alter_leave_days.py
--rw-rw-rw-   0        0        0      488 2022-12-20 07:58:42.000000 django-ipghrms-leave-1.1/leave/migrations/0043_leavecount_balance_carry.py
--rw-rw-rw-   0        0        0      472 2022-12-20 08:17:40.000000 django-ipghrms-leave-1.1/leave/migrations/0044_leavecount_taken.py
--rw-rw-rw-   0        0        0      740 2022-12-20 08:22:31.000000 django-ipghrms-leave-1.1/leave/migrations/0045_auto_20221220_1722.py
--rw-rw-rw-   0        0        0     1060 2022-12-20 08:25:13.000000 django-ipghrms-leave-1.1/leave/migrations/0046_month_year.py
--rw-rw-rw-   0        0        0     1850 2022-12-20 08:29:51.000000 django-ipghrms-leave-1.1/leave/migrations/0047_auto_20221220_1729.py
--rw-rw-rw-   0        0        0     1638 2022-12-21 01:08:08.000000 django-ipghrms-leave-1.1/leave/migrations/0048_auto_20221221_1008.py
--rw-rw-rw-   0        0        0      843 2022-12-21 01:09:38.000000 django-ipghrms-leave-1.1/leave/migrations/0049_auto_20221221_1009.py
--rw-rw-rw-   0        0        0      494 2022-12-21 02:48:00.000000 django-ipghrms-leave-1.1/leave/migrations/0050_leavecount_total_balance_leave.py
--rw-rw-rw-   0        0        0      493 2022-12-21 02:56:16.000000 django-ipghrms-leave-1.1/leave/migrations/0051_alter_leavecount_taken.py
--rw-rw-rw-   0        0        0      495 2022-12-25 12:08:36.000000 django-ipghrms-leave-1.1/leave/migrations/0052_leavecount_prov_total_earn.py
--rw-rw-rw-   0        0        0      499 2022-12-25 12:23:35.000000 django-ipghrms-leave-1.1/leave/migrations/0053_leavecount_total_taken.py
--rw-rw-rw-   0        0        0      777 2022-12-25 13:32:11.000000 django-ipghrms-leave-1.1/leave/migrations/0054_auto_20221225_2232.py
--rw-rw-rw-   0        0        0      461 2022-12-26 14:37:12.000000 django-ipghrms-leave-1.1/leave/migrations/0055_leave_description.py
--rw-rw-rw-   0        0        0      638 2022-12-29 17:21:13.000000 django-ipghrms-leave-1.1/leave/migrations/0056_auto_20221230_0221.py
--rw-rw-rw-   0        0        0      342 2022-12-29 17:21:30.000000 django-ipghrms-leave-1.1/leave/migrations/0057_alter_leavecount_options.py
--rw-rw-rw-   0        0        0      583 2023-01-10 05:27:23.000000 django-ipghrms-leave-1.1/leave/migrations/0058_leaveperiod_employee.py
--rw-rw-rw-   0        0        0      642 2023-01-10 06:35:47.000000 django-ipghrms-leave-1.1/leave/migrations/0059_auto_20230110_1535.py
--rw-rw-rw-   0        0        0      415 2023-01-13 15:24:54.000000 django-ipghrms-leave-1.1/leave/migrations/0060_leavecount_update_date.py
--rw-rw-rw-   0        0        0      486 2023-01-14 03:47:27.000000 django-ipghrms-leave-1.1/leave/migrations/0061_leavecount_balance_month.py
--rw-rw-rw-   0        0        0      441 2023-01-18 02:16:22.000000 django-ipghrms-leave-1.1/leave/migrations/0062_leavehr_comment.py
--rw-rw-rw-   0        0        0      409 2023-01-19 02:02:15.000000 django-ipghrms-leave-1.1/leave/migrations/0063_leave_is_done.py
--rw-rw-rw-   0        0        0      407 2023-01-22 06:45:20.000000 django-ipghrms-leave-1.1/leave/migrations/0064_leave_pr_send.py
--rw-rw-rw-   0        0        0      412 2023-01-22 08:06:42.000000 django-ipghrms-leave-1.1/leave/migrations/0065_leave_vice_send_pr.py
--rw-rw-rw-   0        0        0      414 2023-01-22 08:31:12.000000 django-ipghrms-leave-1.1/leave/migrations/0066_leave_pr_notify.py
--rw-rw-rw-   0        0        0      416 2023-01-29 06:59:00.000000 django-ipghrms-leave-1.1/leave/migrations/0067_leave_is_send_to_div.py
--rw-rw-rw-   0        0        0      858 2023-02-02 00:25:33.000000 django-ipghrms-leave-1.1/leave/migrations/0068_auto_20230202_0925.py
--rw-rw-rw-   0        0        0      427 2023-02-02 05:46:44.000000 django-ipghrms-leave-1.1/leave/migrations/0069_leave_is_special.py
--rw-rw-rw-   0        0        0      430 2023-02-02 05:47:51.000000 django-ipghrms-leave-1.1/leave/migrations/0070_leave_is_create_by_hr.py
--rw-rw-rw-   0        0        0      793 2023-03-13 10:08:08.000000 django-ipghrms-leave-1.1/leave/migrations/0071_auto_20230313_1908.py
--rw-rw-rw-   0        0        0      770 2023-03-13 14:31:35.000000 django-ipghrms-leave-1.1/leave/migrations/0072_auto_20230313_2331.py
--rw-rw-rw-   0        0        0      818 2023-03-13 14:38:15.000000 django-ipghrms-leave-1.1/leave/migrations/0073_auto_20230313_2338.py
--rw-rw-rw-   0        0        0      794 2023-03-13 14:41:54.000000 django-ipghrms-leave-1.1/leave/migrations/0074_auto_20230313_2341.py
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:51.122499 django-ipghrms-leave-1.1/leave/migrations/__pycache__/
--rw-rw-rw-   0        0        0     2438 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0     2406 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0001_initial.cpython-37.pyc
--rw-rw-rw-   0        0        0     2442 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-rw-   0        0        0      513 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-310.pyc
--rw-rw-rw-   0        0        0      499 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-37.pyc
--rw-rw-rw-   0        0        0      517 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-39.pyc
--rw-rw-rw-   0        0        0      633 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-310.pyc
--rw-rw-rw-   0        0        0      625 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-37.pyc
--rw-rw-rw-   0        0        0      637 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-39.pyc
--rw-rw-rw-   0        0        0      813 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-310.pyc
--rw-rw-rw-   0        0        0      799 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-37.pyc
--rw-rw-rw-   0        0        0      817 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-39.pyc
--rw-rw-rw-   0        0        0      589 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-310.pyc
--rw-rw-rw-   0        0        0      575 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-37.pyc
--rw-rw-rw-   0        0        0      593 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-39.pyc
--rw-rw-rw-   0        0        0      630 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-310.pyc
--rw-rw-rw-   0        0        0      616 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-37.pyc
--rw-rw-rw-   0        0        0      634 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-39.pyc
--rw-rw-rw-   0        0        0      590 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0007_leavetype_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      576 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0007_leavetype_total.cpython-37.pyc
--rw-rw-rw-   0        0        0      594 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0007_leavetype_total.cpython-39.pyc
--rw-rw-rw-   0        0        0      659 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      641 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      663 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      765 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      747 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      769 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      816 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-310.pyc
--rw-rw-rw-   0        0        0      798 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-37.pyc
--rw-rw-rw-   0        0        0      820 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-39.pyc
--rw-rw-rw-   0        0        0     1365 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0     1343 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0     1369 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      816 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-310.pyc
--rw-rw-rw-   0        0        0      800 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-37.pyc
--rw-rw-rw-   0        0        0      820 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-39.pyc
--rw-rw-rw-   0        0        0      613 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0013_leave_is_finish.cpython-310.pyc
--rw-rw-rw-   0        0        0      599 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0013_leave_is_finish.cpython-37.pyc
--rw-rw-rw-   0        0        0      617 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0013_leave_is_finish.cpython-39.pyc
--rw-rw-rw-   0        0        0     1398 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-310.pyc
--rw-rw-rw-   0        0        0     1378 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-37.pyc
--rw-rw-rw-   0        0        0     1402 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-39.pyc
--rw-rw-rw-   0        0        0      887 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      867 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      891 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      614 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0016_leave_is_print.cpython-310.pyc
--rw-rw-rw-   0        0        0      600 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0016_leave_is_print.cpython-37.pyc
--rw-rw-rw-   0        0        0      618 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0016_leave_is_print.cpython-39.pyc
--rw-rw-rw-   0        0        0      779 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      759 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      783 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      664 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-310.pyc
--rw-rw-rw-   0        0        0      650 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-37.pyc
--rw-rw-rw-   0        0        0      668 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-39.pyc
--rw-rw-rw-   0        0        0      598 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-310.pyc
--rw-rw-rw-   0        0        0      584 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-37.pyc
--rw-rw-rw-   0        0        0      602 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-39.pyc
--rw-rw-rw-   0        0        0      527 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-310.pyc
--rw-rw-rw-   0        0        0      513 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-37.pyc
--rw-rw-rw-   0        0        0      531 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-39.pyc
--rw-rw-rw-   0        0        0      655 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-310.pyc
--rw-rw-rw-   0        0        0      639 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-37.pyc
--rw-rw-rw-   0        0        0      659 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-39.pyc
--rw-rw-rw-   0        0        0      676 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-310.pyc
--rw-rw-rw-   0        0        0      658 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-37.pyc
--rw-rw-rw-   0        0        0      680 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-39.pyc
--rw-rw-rw-   0        0        0      559 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-310.pyc
--rw-rw-rw-   0        0        0      545 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-37.pyc
--rw-rw-rw-   0        0        0      563 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-39.pyc
--rw-rw-rw-   0        0        0      601 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-310.pyc
--rw-rw-rw-   0        0        0      587 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-37.pyc
--rw-rw-rw-   0        0        0      605 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-39.pyc
--rw-rw-rw-   0        0        0      767 2022-12-10 14:30:02.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0025_auto_20221210_2329.cpython-310.pyc
--rw-rw-rw-   0        0        0      636 2022-12-10 14:56:45.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0026_auto_20221210_2356.cpython-310.pyc
--rw-rw-rw-   0        0        0      551 2022-12-10 15:22:20.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0027_auto_20221211_0022.cpython-310.pyc
--rw-rw-rw-   0        0        0      636 2022-12-10 17:02:14.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0028_auto_20221211_0202.cpython-310.pyc
--rw-rw-rw-   0        0        0     1231 2022-12-11 02:51:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0029_leavedep.cpython-310.pyc
--rw-rw-rw-   0        0        0      621 2022-12-11 03:06:37.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0030_auto_20221211_1206.cpython-310.pyc
--rw-rw-rw-   0        0        0      582 2022-12-11 04:17:00.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0031_leave_is_update.cpython-310.pyc
--rw-rw-rw-   0        0        0      583 2022-12-17 06:24:49.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0032_leave_dep_send_pr.cpython-310.pyc
--rw-rw-rw-   0        0        0      583 2022-12-17 06:40:16.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0033_leave_pr_confirm.cpython-310.pyc
--rw-rw-rw-   0        0        0      557 2022-12-17 06:43:37.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0034_rename_pr_confirm_leave_pr_approve.cpython-310.pyc
--rw-rw-rw-   0        0        0      853 2022-12-17 07:14:57.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0035_leave_file.cpython-310.pyc
--rw-rw-rw-   0        0        0      580 2022-12-17 08:47:40.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0036_leave_unit_send_pr.cpython-310.pyc
--rw-rw-rw-   0        0        0      631 2022-12-20 07:39:49.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0037_alter_leavetype_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      592 2022-12-20 07:43:20.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0038_alter_leavetype_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      634 2022-12-20 07:50:58.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0039_alter_leavetype_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      665 2022-12-20 07:55:32.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0040_alter_leavecount_balance.cpython-310.pyc
--rw-rw-rw-   0        0        0      662 2022-12-20 07:56:02.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0041_alter_leavecount_total.cpython-310.pyc
--rw-rw-rw-   0        0        0      646 2022-12-20 07:56:33.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0042_alter_leave_days.cpython-310.pyc
--rw-rw-rw-   0        0        0      678 2022-12-20 07:58:45.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0043_leavecount_balance_carry.cpython-310.pyc
--rw-rw-rw-   0        0        0      654 2022-12-20 08:17:44.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0044_leavecount_taken.cpython-310.pyc
--rw-rw-rw-   0        0        0      810 2022-12-20 08:22:35.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0045_auto_20221220_1722.cpython-310.pyc
--rw-rw-rw-   0        0        0      871 2022-12-20 08:25:17.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0046_month_year.cpython-310.pyc
--rw-rw-rw-   0        0        0     1293 2022-12-20 08:29:55.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0047_auto_20221220_1729.cpython-310.pyc
--rw-rw-rw-   0        0        0      978 2022-12-21 01:08:12.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0048_auto_20221221_1008.cpython-310.pyc
--rw-rw-rw-   0        0        0      843 2022-12-21 01:09:42.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0049_auto_20221221_1009.cpython-310.pyc
--rw-rw-rw-   0        0        0      690 2022-12-21 02:48:03.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0050_leavecount_total_balance_leave.cpython-310.pyc
--rw-rw-rw-   0        0        0      688 2022-12-21 02:56:19.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0051_alter_leavecount_taken.cpython-310.pyc
--rw-rw-rw-   0        0        0      687 2022-12-25 12:08:43.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0052_leavecount_prov_total_earn.cpython-310.pyc
--rw-rw-rw-   0        0        0      694 2022-12-25 12:23:40.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0053_leavecount_total_taken.cpython-310.pyc
--rw-rw-rw-   0        0        0      885 2022-12-25 13:32:16.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0054_auto_20221225_2232.cpython-310.pyc
--rw-rw-rw-   0        0        0      635 2022-12-26 14:37:20.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0055_leave_description.cpython-310.pyc
--rw-rw-rw-   0        0        0      776 2022-12-29 17:21:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0056_auto_20221230_0221.cpython-310.pyc
--rw-rw-rw-   0        0        0      517 2022-12-29 17:21:36.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0057_alter_leavecount_options.cpython-310.pyc
--rw-rw-rw-   0        0        0      751 2023-01-10 05:27:31.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0058_leaveperiod_employee.cpython-310.pyc
--rw-rw-rw-   0        0        0      676 2023-01-10 06:35:52.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0059_auto_20230110_1535.cpython-310.pyc
--rw-rw-rw-   0        0        0      592 2023-01-13 15:25:02.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0060_leavecount_update_date.cpython-310.pyc
--rw-rw-rw-   0        0        0      676 2023-01-14 03:47:32.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0061_leavecount_balance_month.cpython-310.pyc
--rw-rw-rw-   0        0        0      612 2023-01-18 02:16:27.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0062_leavehr_comment.cpython-310.pyc
--rw-rw-rw-   0        0        0      575 2023-01-19 02:02:21.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0063_leave_is_done.cpython-310.pyc
--rw-rw-rw-   0        0        0      573 2023-01-22 06:45:26.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0064_leave_pr_send.cpython-310.pyc
--rw-rw-rw-   0        0        0      583 2023-01-22 08:06:46.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0065_leave_vice_send_pr.cpython-310.pyc
--rw-rw-rw-   0        0        0      582 2023-01-22 08:31:16.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0066_leave_pr_notify.cpython-310.pyc
--rw-rw-rw-   0        0        0      589 2023-01-29 06:59:04.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0067_leave_is_send_to_div.cpython-310.pyc
--rw-rw-rw-   0        0        0      765 2023-02-02 00:25:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0068_auto_20230202_0925.cpython-310.pyc
--rw-rw-rw-   0        0        0      593 2023-02-02 05:46:50.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0069_leave_is_special.cpython-310.pyc
--rw-rw-rw-   0        0        0      601 2023-02-02 05:47:54.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0070_leave_is_create_by_hr.cpython-310.pyc
--rw-rw-rw-   0        0        0      799 2023-03-13 10:08:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0071_auto_20230313_1908.cpython-310.pyc
--rw-rw-rw-   0        0        0      786 2023-03-13 14:31:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0072_auto_20230313_2331.cpython-310.pyc
--rw-rw-rw-   0        0        0      810 2023-03-13 14:38:19.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0073_auto_20230313_2338.cpython-310.pyc
--rw-rw-rw-   0        0        0      798 2023-03-13 14:41:58.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/0074_auto_20230313_2341.cpython-310.pyc
--rw-rw-rw-   0        0        0      145 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      143 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      151 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    11225 2023-03-13 19:02:47.000000 django-ipghrms-leave-1.1/leave/models.py
--rw-rw-rw-   0        0        0      727 2022-12-11 02:52:39.000000 django-ipghrms-leave-1.1/leave/signals.py
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:48.848955 django-ipghrms-leave-1.1/leave/templates/
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:51.647972 django-ipghrms-leave-1.1/leave/templates/leave/
--rw-rw-rw-   0        0        0     3156 2023-03-13 19:55:21.000000 django-ipghrms-leave-1.1/leave/templates/leave/bal_s_list.html
--rw-rw-rw-   0        0        0     8894 2023-03-14 15:00:37.000000 django-ipghrms-leave-1.1/leave/templates/leave/c_apply_detail.html
--rw-rw-rw-   0        0        0     2029 2023-03-13 19:58:25.000000 django-ipghrms-leave-1.1/leave/templates/leave/c_apply_list.html
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/templates/leave/c_deleg_detail.html
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/templates/leave/c_deleg_list.html
--rw-rw-rw-   0        0        0    11028 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.1/leave/templates/leave/c_ver_detail.html
--rw-rw-rw-   0        0        0     1630 2023-03-13 19:57:57.000000 django-ipghrms-leave-1.1/leave/templates/leave/c_ver_list.html
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/templates/leave/dash.html
--rw-rw-rw-   0        0        0     8646 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.1/leave/templates/leave/de_appr_detail.html
--rw-rw-rw-   0        0        0     1629 2023-02-20 14:30:10.000000 django-ipghrms-leave-1.1/leave/templates/leave/de_appr_list.html
--rw-rw-rw-   0        0        0     3714 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.1/leave/templates/leave/de_detail.html
--rw-rw-rw-   0        0        0     1993 2023-03-13 19:41:48.000000 django-ipghrms-leave-1.1/leave/templates/leave/de_list.html
--rw-rw-rw-   0        0        0     5899 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.1/leave/templates/leave/deleg_detail.html
--rw-rw-rw-   0        0        0     1715 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/templates/leave/deleg_list.html
--rw-rw-rw-   0        0        0    15438 2023-03-13 19:47:09.000000 django-ipghrms-leave-1.1/leave/templates/leave/dep_detail.html
--rw-rw-rw-   0        0        0     1979 2023-03-13 19:56:56.000000 django-ipghrms-leave-1.1/leave/templates/leave/dep_list.html
--rw-rw-rw-   0        0        0     2096 2023-03-13 19:56:32.000000 django-ipghrms-leave-1.1/leave/templates/leave/dep_req_list.html
--rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/templates/leave/detail.html
--rw-rw-rw-   0        0        0      233 2023-01-20 03:07:32.000000 django-ipghrms-leave-1.1/leave/templates/leave/error.html
--rw-rw-rw-   0        0        0        0 2023-03-13 18:02:58.000000 django-ipghrms-leave-1.1/leave/templates/leave/error2.html
--rw-rw-rw-   0        0        0     2388 2023-02-13 04:54:46.000000 django-ipghrms-leave-1.1/leave/templates/leave/form.html
--rw-rw-rw-   0        0        0     2378 2023-02-09 09:22:50.000000 django-ipghrms-leave-1.1/leave/templates/leave/form2.html
--rw-rw-rw-   0        0        0    12233 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.1/leave/templates/leave/hr_app_detail.html
--rw-rw-rw-   0        0        0     2791 2023-02-08 07:36:20.000000 django-ipghrms-leave-1.1/leave/templates/leave/hr_app_list.html
--rw-rw-rw-   0        0        0     9600 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.1/leave/templates/leave/hr_cert_detail.html
--rw-rw-rw-   0        0        0     2395 2023-02-08 07:45:08.000000 django-ipghrms-leave-1.1/leave/templates/leave/hr_cert_list.html
--rw-rw-rw-   0        0        0    12174 2023-02-09 10:12:29.000000 django-ipghrms-leave-1.1/leave/templates/leave/hr_leave_record.html
--rw-rw-rw-   0        0        0     2481 2023-04-10 02:56:35.000000 django-ipghrms-leave-1.1/leave/templates/leave/hr_period_list.html
--rw-rw-rw-   0        0        0     8049 2023-04-10 02:56:45.000000 django-ipghrms-leave-1.1/leave/templates/leave/hr_raw_list.html
--rw-rw-rw-   0        0        0     2160 2023-02-08 07:42:56.000000 django-ipghrms-leave-1.1/leave/templates/leave/list.html
--rw-rw-rw-   0        0        0    11403 2023-03-14 15:00:58.000000 django-ipghrms-leave-1.1/leave/templates/leave/s_apply_detail.html
--rw-rw-rw-   0        0        0     2355 2023-02-07 00:15:15.000000 django-ipghrms-leave-1.1/leave/templates/leave/s_apply_list.html
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:51.796157 django-ipghrms-leave-1.1/leave/templates/leave_chart/
--rw-rw-rw-   0        0        0     3992 2023-01-29 14:41:00.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/chart_leave.html
--rw-rw-rw-   0        0        0     1146 2023-01-23 16:35:15.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/emp.js
--rw-rw-rw-   0        0        0     1334 2023-01-23 16:35:32.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type.js
--rw-rw-rw-   0        0        0     2207 2023-02-05 07:02:46.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type2.js
--rw-rw-rw-   0        0        0     2240 2023-01-30 01:41:48.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type3.js
--rw-rw-rw-   0        0        0     2219 2023-02-05 07:27:37.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_month.js
--rw-rw-rw-   0        0        0     2257 2023-02-05 07:35:06.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_month_unit.js
--rw-rw-rw-   0        0        0     2211 2023-02-05 07:55:31.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_tri.js
--rw-rw-rw-   0        0        0     2215 2023-02-05 07:17:54.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_unit.js
--rw-rw-rw-   0        0        0     2211 2023-02-05 07:01:28.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year.js
--rw-rw-rw-   0        0        0     2257 2023-02-05 07:28:20.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_month.js
--rw-rw-rw-   0        0        0     2294 2023-02-05 07:57:33.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_month_unit.js
--rw-rw-rw-   0        0        0     2249 2023-02-05 07:44:38.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_tri.js
--rw-rw-rw-   0        0        0     2287 2023-02-05 08:07:00.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_tri_unit.js
--rw-rw-rw-   0        0        0     2253 2023-02-05 07:21:46.000000 django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_unit.js
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:51.816079 django-ipghrms-leave-1.1/leave/templates/leave_print/
--rw-rw-rw-   0        0        0     1869 2022-11-30 07:59:44.000000 django-ipghrms-leave-1.1/leave/templates/leave_print/layout.html
--rw-rw-rw-   0        0        0     5245 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.1/leave/templates/leave_print/leave_print.html
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:51.846717 django-ipghrms-leave-1.1/leave/templates/leave_report/
--rw-rw-rw-   0        0        0    18125 2023-02-05 10:10:59.000000 django-ipghrms-leave-1.1/leave/templates/leave_report/dash.html
--rw-rw-rw-   0        0        0     1956 2023-02-05 08:54:19.000000 django-ipghrms-leave-1.1/leave/templates/leave_report/list.html
--rw-rw-rw-   0        0        0     1917 2023-01-30 07:04:02.000000 django-ipghrms-leave-1.1/leave/templates/leave_report/list_day.html
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:51.871639 django-ipghrms-leave-1.1/leave/templates/pdf/
--rw-rw-rw-   0        0        0      128 2023-02-24 10:02:16.000000 django-ipghrms-leave-1.1/leave/templates/pdf/cop.html
--rw-rw-rw-   0        0        0      610 2023-02-02 15:25:15.000000 django-ipghrms-leave-1.1/leave/templates/pdf/layout.html
--rw-rw-rw-   0        0        0     7845 2023-03-15 14:31:17.000000 django-ipghrms-leave-1.1/leave/templates/pdf/leave.html
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:51.880153 django-ipghrms-leave-1.1/leave/templatetags/
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:51.887528 django-ipghrms-leave-1.1/leave/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      483 2023-01-14 07:10:52.000000 django-ipghrms-leave-1.1/leave/templatetags/__pycache__/orderby.cpython-310.pyc
--rw-rw-rw-   0        0        0      215 2023-01-14 07:10:49.000000 django-ipghrms-leave-1.1/leave/templatetags/orderby.py
--rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/tests.py
--rw-rw-rw-   0        0        0     5258 2023-04-10 02:56:19.000000 django-ipghrms-leave-1.1/leave/urls.py
--rw-rw-rw-   0        0        0     2788 2023-02-05 10:03:59.000000 django-ipghrms-leave-1.1/leave/urls_report.py
--rw-rw-rw-   0        0        0    15129 2023-03-13 19:53:08.000000 django-ipghrms-leave-1.1/leave/utils.py
--rw-rw-rw-   0        0        0     2737 2023-03-13 18:08:06.000000 django-ipghrms-leave-1.1/leave/utils_2.py
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:51.991536 django-ipghrms-leave-1.1/leave/views/
--rw-rw-rw-   0        0        0      325 2023-01-29 14:29:10.000000 django-ipghrms-leave-1.1/leave/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 06:02:52.308425 django-ipghrms-leave-1.1/leave/views/__pycache__/
--rw-rw-rw-   0        0        0      417 2023-01-29 14:29:14.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      370 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      378 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     3566 2023-03-15 10:05:12.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     2343 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     2331 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     2601 2023-01-29 07:19:53.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     2460 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     2469 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_v.cpython-39.pyc
--rw-rw-rw-   0        0        0      737 2023-01-23 14:19:18.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_chart.cpython-310.pyc
--rw-rw-rw-   0        0        0     2506 2023-03-15 10:08:49.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     1993 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     1980 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     2279 2023-02-20 14:30:35.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     1550 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     1574 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_v.cpython-39.pyc
--rw-rw-rw-   0        0        0    25037 2023-03-13 19:37:38.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     1813 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     1814 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_m.cpython-39.pyc
--rw-rw-rw-   0        0        0    10718 2023-03-13 18:47:18.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     2398 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     2192 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_v.cpython-39.pyc
--rw-rw-rw-   0        0        0    11609 2023-03-13 18:27:21.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     6368 2022-11-07 06:40:44.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_m.cpython-37.pyc
--rw-rw-rw-   0        0        0     6062 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_m.cpython-39.pyc
--rw-rw-rw-   0        0        0    17186 2023-02-15 01:07:16.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_report.cpython-310.pyc
--rw-rw-rw-   0        0        0     2026 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s.cpython-39.pyc
--rw-rw-rw-   0        0        0      821 2022-11-07 13:19:37.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_m.cpython-310.pyc
--rw-rw-rw-   0        0        0      819 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_m.cpython-37.pyc
--rw-rw-rw-   0        0        0      827 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     4849 2023-03-15 14:22:55.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     2143 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     2161 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     1279 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_staff.cpython-39.pyc
--rw-rw-rw-   0        0        0     3232 2023-03-13 18:30:54.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     1961 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_v.cpython-37.pyc
--rw-rw-rw-   0        0        0     1926 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/leave_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     1565 2022-11-07 13:19:37.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/print.cpython-310.pyc
--rw-rw-rw-   0        0        0     1555 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/print.cpython-37.pyc
--rw-rw-rw-   0        0        0     1571 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/__pycache__/print.cpython-39.pyc
--rw-rw-rw-   0        0        0     4191 2023-03-15 10:04:22.000000 django-ipghrms-leave-1.1/leave/views/leave_c_m.py
--rw-rw-rw-   0        0        0     2732 2023-01-29 07:19:51.000000 django-ipghrms-leave-1.1/leave/views/leave_c_v.py
--rw-rw-rw-   0        0        0      527 2023-01-23 14:19:06.000000 django-ipghrms-leave-1.1/leave/views/leave_chart.py
--rw-rw-rw-   0        0        0     2610 2023-03-15 10:08:46.000000 django-ipghrms-leave-1.1/leave/views/leave_de_m.py
--rw-rw-rw-   0        0        0     2853 2023-02-20 14:30:30.000000 django-ipghrms-leave-1.1/leave/views/leave_de_v.py
--rw-rw-rw-   0        0        0    59105 2023-03-13 19:37:35.000000 django-ipghrms-leave-1.1/leave/views/leave_hr_m.py
--rw-rw-rw-   0        0        0    44603 2023-02-09 05:04:14.000000 django-ipghrms-leave-1.1/leave/views/leave_hr_m_back.py
--rw-rw-rw-   0        0        0    16680 2023-03-13 18:47:16.000000 django-ipghrms-leave-1.1/leave/views/leave_hr_v.py
--rw-rw-rw-   0        0        0    20569 2023-03-13 18:27:19.000000 django-ipghrms-leave-1.1/leave/views/leave_m.py
--rw-rw-rw-   0        0        0    31199 2023-02-15 01:07:13.000000 django-ipghrms-leave-1.1/leave/views/leave_report.py
--rw-rw-rw-   0        0        0      514 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/leave_s_m.py
--rw-rw-rw-   0        0        0     5451 2023-03-15 14:22:52.000000 django-ipghrms-leave-1.1/leave/views/leave_s_v.py
--rw-rw-rw-   0        0        0     3684 2023-03-13 18:30:52.000000 django-ipghrms-leave-1.1/leave/views/leave_v.py
--rw-rw-rw-   0        0        0     1674 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views/print.py
--rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.1/leave/views.py
--rw-rw-rw-   0        0        0      505 2023-04-10 06:02:52.322485 django-ipghrms-leave-1.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-leave-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.793162 django-ipghrms-leave-1.2/
+-rw-rw-rw-   0        0        0     1065 2023-03-27 14:45:38.000000 django-ipghrms-leave-1.2/LICENSE
+-rw-rw-rw-   0        0        0      214 2023-03-27 14:21:05.000000 django-ipghrms-leave-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1131 2023-05-30 20:04:54.793162 django-ipghrms-leave-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-03-27 14:21:43.000000 django-ipghrms-leave-1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:52.289497 django-ipghrms-leave-1.2/django_ipghrms_leave.egg-info/
+-rw-rw-rw-   0        0        0     1131 2023-05-30 20:04:51.000000 django-ipghrms-leave-1.2/django_ipghrms_leave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18263 2023-05-30 20:04:52.000000 django-ipghrms-leave-1.2/django_ipghrms_leave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 20:04:51.000000 django-ipghrms-leave-1.2/django_ipghrms_leave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 20:04:51.000000 django-ipghrms-leave-1.2/django_ipghrms_leave.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:52.386843 django-ipghrms-leave-1.2/leave/
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/__init__.py
+-rw-rw-rw-   0        0        0      385 2022-12-20 08:39:46.000000 django-ipghrms-leave-1.2/leave/admin.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:52.393530 django-ipghrms-leave-1.2/leave/api/
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:52.398843 django-ipghrms-leave-1.2/leave/api/__pycache__/
+-rw-rw-rw-   0        0        0     1223 2023-02-05 08:06:39.000000 django-ipghrms-leave-1.2/leave/api/__pycache__/urls.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9993 2023-02-05 08:09:34.000000 django-ipghrms-leave-1.2/leave/api/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1189 2023-02-05 08:06:35.000000 django-ipghrms-leave-1.2/leave/api/urls.py
+-rw-rw-rw-   0        0        0    13296 2023-02-05 08:09:31.000000 django-ipghrms-leave-1.2/leave/api/views.py
+-rw-rw-rw-   0        0        0      178 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/apps.py
+-rw-rw-rw-   0        0        0    11646 2023-05-30 04:20:36.000000 django-ipghrms-leave-1.2/leave/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:53.545267 django-ipghrms-leave-1.2/leave/migrations/
+-rw-rw-rw-   0        0        0     4776 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      317 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0002_remove_taskdelegate_date.py
+-rw-rw-rw-   0        0        0      450 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0003_rename_taskdelegate_leavedelegate.py
+-rw-rw-rw-   0        0        0      619 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0004_alter_leavedelegate_employee.py
+-rw-rw-rw-   0        0        0      384 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0005_rename_is_approve_leavedelegate_is_confirm.py
+-rw-rw-rw-   0        0        0      430 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0006_leavedelegate_is_confirm2.py
+-rw-rw-rw-   0        0        0      400 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0007_leavetype_total.py
+-rw-rw-rw-   0        0        0      649 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0008_rename_de_confirm_leave_de_approve_and_more.py
+-rw-rw-rw-   0        0        0      705 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0009_rename_is_lock_leave_s_is_finish_and_more.py
+-rw-rw-rw-   0        0        0      980 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.py
+-rw-rw-rw-   0        0        0     1507 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.py
+-rw-rw-rw-   0        0        0      766 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0012_alter_leavedelegate_leave_alter_leaveunit_leave.py
+-rw-rw-rw-   0        0        0      425 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0013_leave_is_finish.py
+-rw-rw-rw-   0        0        0     2028 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0014_leavehr_leavede.py
+-rw-rw-rw-   0        0        0     1198 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.py
+-rw-rw-rw-   0        0        0      427 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0016_leave_is_print.py
+-rw-rw-rw-   0        0        0      750 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.py
+-rw-rw-rw-   0        0        0      464 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0018_alter_leavecount_balance.py
+-rw-rw-rw-   0        0        0      406 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0019_leave_s_is_delegate.py
+-rw-rw-rw-   0        0        0      331 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0020_remove_leave_s_is_delegate.py
+-rw-rw-rw-   0        0        0      572 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0021_leave_is_approve_leave_is_reject.py
+-rw-rw-rw-   0        0        0      664 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0022_rename_s_is_finish_leave_is_delegate_and_more.py
+-rw-rw-rw-   0        0        0      359 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0023_remove_leavedelegate_is_send.py
+-rw-rw-rw-   0        0        0      407 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/0024_alter_leave_is_active.py
+-rw-rw-rw-   0        0        0      795 2022-12-10 14:29:58.000000 django-ipghrms-leave-1.2/leave/migrations/0025_auto_20221210_2329.py
+-rw-rw-rw-   0        0        0      590 2022-12-10 14:56:41.000000 django-ipghrms-leave-1.2/leave/migrations/0026_auto_20221210_2356.py
+-rw-rw-rw-   0        0        0      460 2022-12-10 15:22:16.000000 django-ipghrms-leave-1.2/leave/migrations/0027_auto_20221211_0022.py
+-rw-rw-rw-   0        0        0      590 2022-12-10 17:02:09.000000 django-ipghrms-leave-1.2/leave/migrations/0028_auto_20221211_0202.py
+-rw-rw-rw-   0        0        0     1255 2022-12-11 02:51:24.000000 django-ipghrms-leave-1.2/leave/migrations/0029_leavedep.py
+-rw-rw-rw-   0        0        0      577 2022-12-11 03:06:33.000000 django-ipghrms-leave-1.2/leave/migrations/0030_auto_20221211_1206.py
+-rw-rw-rw-   0        0        0      414 2022-12-11 04:16:56.000000 django-ipghrms-leave-1.2/leave/migrations/0031_leave_is_update.py
+-rw-rw-rw-   0        0        0      413 2022-12-17 06:24:38.000000 django-ipghrms-leave-1.2/leave/migrations/0032_leave_dep_send_pr.py
+-rw-rw-rw-   0        0        0      414 2022-12-17 06:40:11.000000 django-ipghrms-leave-1.2/leave/migrations/0033_leave_pr_confirm.py
+-rw-rw-rw-   0        0        0      382 2022-12-17 06:43:34.000000 django-ipghrms-leave-1.2/leave/migrations/0034_rename_pr_confirm_leave_pr_approve.py
+-rw-rw-rw-   0        0        0      652 2022-12-17 07:14:52.000000 django-ipghrms-leave-1.2/leave/migrations/0035_leave_file.py
+-rw-rw-rw-   0        0        0      409 2022-12-17 08:47:37.000000 django-ipghrms-leave-1.2/leave/migrations/0036_leave_unit_send_pr.py
+-rw-rw-rw-   0        0        0      445 2022-12-20 07:39:43.000000 django-ipghrms-leave-1.2/leave/migrations/0037_alter_leavetype_total.py
+-rw-rw-rw-   0        0        0      416 2022-12-20 07:43:17.000000 django-ipghrms-leave-1.2/leave/migrations/0038_alter_leavetype_total.py
+-rw-rw-rw-   0        0        0      448 2022-12-20 07:50:53.000000 django-ipghrms-leave-1.2/leave/migrations/0039_alter_leavetype_total.py
+-rw-rw-rw-   0        0        0      475 2022-12-20 07:55:29.000000 django-ipghrms-leave-1.2/leave/migrations/0040_alter_leavecount_balance.py
+-rw-rw-rw-   0        0        0      474 2022-12-20 07:55:59.000000 django-ipghrms-leave-1.2/leave/migrations/0041_alter_leavecount_total.py
+-rw-rw-rw-   0        0        0      466 2022-12-20 07:56:29.000000 django-ipghrms-leave-1.2/leave/migrations/0042_alter_leave_days.py
+-rw-rw-rw-   0        0        0      488 2022-12-20 07:58:42.000000 django-ipghrms-leave-1.2/leave/migrations/0043_leavecount_balance_carry.py
+-rw-rw-rw-   0        0        0      472 2022-12-20 08:17:40.000000 django-ipghrms-leave-1.2/leave/migrations/0044_leavecount_taken.py
+-rw-rw-rw-   0        0        0      740 2022-12-20 08:22:31.000000 django-ipghrms-leave-1.2/leave/migrations/0045_auto_20221220_1722.py
+-rw-rw-rw-   0        0        0     1060 2022-12-20 08:25:13.000000 django-ipghrms-leave-1.2/leave/migrations/0046_month_year.py
+-rw-rw-rw-   0        0        0     1850 2022-12-20 08:29:51.000000 django-ipghrms-leave-1.2/leave/migrations/0047_auto_20221220_1729.py
+-rw-rw-rw-   0        0        0     1638 2022-12-21 01:08:08.000000 django-ipghrms-leave-1.2/leave/migrations/0048_auto_20221221_1008.py
+-rw-rw-rw-   0        0        0      843 2022-12-21 01:09:38.000000 django-ipghrms-leave-1.2/leave/migrations/0049_auto_20221221_1009.py
+-rw-rw-rw-   0        0        0      494 2022-12-21 02:48:00.000000 django-ipghrms-leave-1.2/leave/migrations/0050_leavecount_total_balance_leave.py
+-rw-rw-rw-   0        0        0      493 2022-12-21 02:56:16.000000 django-ipghrms-leave-1.2/leave/migrations/0051_alter_leavecount_taken.py
+-rw-rw-rw-   0        0        0      495 2022-12-25 12:08:36.000000 django-ipghrms-leave-1.2/leave/migrations/0052_leavecount_prov_total_earn.py
+-rw-rw-rw-   0        0        0      499 2022-12-25 12:23:35.000000 django-ipghrms-leave-1.2/leave/migrations/0053_leavecount_total_taken.py
+-rw-rw-rw-   0        0        0      777 2022-12-25 13:32:11.000000 django-ipghrms-leave-1.2/leave/migrations/0054_auto_20221225_2232.py
+-rw-rw-rw-   0        0        0      461 2022-12-26 14:37:12.000000 django-ipghrms-leave-1.2/leave/migrations/0055_leave_description.py
+-rw-rw-rw-   0        0        0      638 2022-12-29 17:21:13.000000 django-ipghrms-leave-1.2/leave/migrations/0056_auto_20221230_0221.py
+-rw-rw-rw-   0        0        0      342 2022-12-29 17:21:30.000000 django-ipghrms-leave-1.2/leave/migrations/0057_alter_leavecount_options.py
+-rw-rw-rw-   0        0        0      583 2023-01-10 05:27:23.000000 django-ipghrms-leave-1.2/leave/migrations/0058_leaveperiod_employee.py
+-rw-rw-rw-   0        0        0      642 2023-01-10 06:35:47.000000 django-ipghrms-leave-1.2/leave/migrations/0059_auto_20230110_1535.py
+-rw-rw-rw-   0        0        0      415 2023-01-13 15:24:54.000000 django-ipghrms-leave-1.2/leave/migrations/0060_leavecount_update_date.py
+-rw-rw-rw-   0        0        0      486 2023-01-14 03:47:27.000000 django-ipghrms-leave-1.2/leave/migrations/0061_leavecount_balance_month.py
+-rw-rw-rw-   0        0        0      441 2023-01-18 02:16:22.000000 django-ipghrms-leave-1.2/leave/migrations/0062_leavehr_comment.py
+-rw-rw-rw-   0        0        0      409 2023-01-19 02:02:15.000000 django-ipghrms-leave-1.2/leave/migrations/0063_leave_is_done.py
+-rw-rw-rw-   0        0        0      407 2023-01-22 06:45:20.000000 django-ipghrms-leave-1.2/leave/migrations/0064_leave_pr_send.py
+-rw-rw-rw-   0        0        0      412 2023-01-22 08:06:42.000000 django-ipghrms-leave-1.2/leave/migrations/0065_leave_vice_send_pr.py
+-rw-rw-rw-   0        0        0      414 2023-01-22 08:31:12.000000 django-ipghrms-leave-1.2/leave/migrations/0066_leave_pr_notify.py
+-rw-rw-rw-   0        0        0      416 2023-01-29 06:59:00.000000 django-ipghrms-leave-1.2/leave/migrations/0067_leave_is_send_to_div.py
+-rw-rw-rw-   0        0        0      858 2023-02-02 00:25:33.000000 django-ipghrms-leave-1.2/leave/migrations/0068_auto_20230202_0925.py
+-rw-rw-rw-   0        0        0      427 2023-02-02 05:46:44.000000 django-ipghrms-leave-1.2/leave/migrations/0069_leave_is_special.py
+-rw-rw-rw-   0        0        0      430 2023-02-02 05:47:51.000000 django-ipghrms-leave-1.2/leave/migrations/0070_leave_is_create_by_hr.py
+-rw-rw-rw-   0        0        0      793 2023-03-13 10:08:08.000000 django-ipghrms-leave-1.2/leave/migrations/0071_auto_20230313_1908.py
+-rw-rw-rw-   0        0        0      770 2023-03-13 14:31:35.000000 django-ipghrms-leave-1.2/leave/migrations/0072_auto_20230313_2331.py
+-rw-rw-rw-   0        0        0      818 2023-03-13 14:38:15.000000 django-ipghrms-leave-1.2/leave/migrations/0073_auto_20230313_2338.py
+-rw-rw-rw-   0        0        0      794 2023-03-13 14:41:54.000000 django-ipghrms-leave-1.2/leave/migrations/0074_auto_20230313_2341.py
+-rw-rw-rw-   0        0        0        0 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:53.971284 django-ipghrms-leave-1.2/leave/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     2438 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2406 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0001_initial.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2442 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-rw-   0        0        0      513 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-310.pyc
+-rw-rw-rw-   0        0        0      499 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-37.pyc
+-rw-rw-rw-   0        0        0      517 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-39.pyc
+-rw-rw-rw-   0        0        0      633 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-310.pyc
+-rw-rw-rw-   0        0        0      625 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-37.pyc
+-rw-rw-rw-   0        0        0      637 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-39.pyc
+-rw-rw-rw-   0        0        0      813 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-310.pyc
+-rw-rw-rw-   0        0        0      799 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-37.pyc
+-rw-rw-rw-   0        0        0      817 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-39.pyc
+-rw-rw-rw-   0        0        0      589 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-310.pyc
+-rw-rw-rw-   0        0        0      575 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-37.pyc
+-rw-rw-rw-   0        0        0      593 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-39.pyc
+-rw-rw-rw-   0        0        0      630 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-310.pyc
+-rw-rw-rw-   0        0        0      616 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-37.pyc
+-rw-rw-rw-   0        0        0      634 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-39.pyc
+-rw-rw-rw-   0        0        0      590 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0007_leavetype_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      576 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0007_leavetype_total.cpython-37.pyc
+-rw-rw-rw-   0        0        0      594 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0007_leavetype_total.cpython-39.pyc
+-rw-rw-rw-   0        0        0      659 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      641 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      663 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      765 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      747 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      769 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      816 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-310.pyc
+-rw-rw-rw-   0        0        0      798 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-37.pyc
+-rw-rw-rw-   0        0        0      820 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1365 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1343 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1369 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      816 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-310.pyc
+-rw-rw-rw-   0        0        0      800 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-37.pyc
+-rw-rw-rw-   0        0        0      820 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-39.pyc
+-rw-rw-rw-   0        0        0      613 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0013_leave_is_finish.cpython-310.pyc
+-rw-rw-rw-   0        0        0      599 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0013_leave_is_finish.cpython-37.pyc
+-rw-rw-rw-   0        0        0      617 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0013_leave_is_finish.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1398 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1378 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1402 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-39.pyc
+-rw-rw-rw-   0        0        0      887 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      867 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      891 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      614 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0016_leave_is_print.cpython-310.pyc
+-rw-rw-rw-   0        0        0      600 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0016_leave_is_print.cpython-37.pyc
+-rw-rw-rw-   0        0        0      618 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0016_leave_is_print.cpython-39.pyc
+-rw-rw-rw-   0        0        0      779 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      759 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      783 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      664 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-310.pyc
+-rw-rw-rw-   0        0        0      650 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-37.pyc
+-rw-rw-rw-   0        0        0      668 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      598 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-310.pyc
+-rw-rw-rw-   0        0        0      584 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-37.pyc
+-rw-rw-rw-   0        0        0      602 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-39.pyc
+-rw-rw-rw-   0        0        0      527 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-310.pyc
+-rw-rw-rw-   0        0        0      513 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-37.pyc
+-rw-rw-rw-   0        0        0      531 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-39.pyc
+-rw-rw-rw-   0        0        0      655 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-310.pyc
+-rw-rw-rw-   0        0        0      639 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-37.pyc
+-rw-rw-rw-   0        0        0      659 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-39.pyc
+-rw-rw-rw-   0        0        0      676 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-310.pyc
+-rw-rw-rw-   0        0        0      658 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-37.pyc
+-rw-rw-rw-   0        0        0      680 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-39.pyc
+-rw-rw-rw-   0        0        0      559 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-310.pyc
+-rw-rw-rw-   0        0        0      545 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-37.pyc
+-rw-rw-rw-   0        0        0      563 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-39.pyc
+-rw-rw-rw-   0        0        0      601 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-310.pyc
+-rw-rw-rw-   0        0        0      587 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-37.pyc
+-rw-rw-rw-   0        0        0      605 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-39.pyc
+-rw-rw-rw-   0        0        0      767 2022-12-10 14:30:02.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0025_auto_20221210_2329.cpython-310.pyc
+-rw-rw-rw-   0        0        0      636 2022-12-10 14:56:45.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0026_auto_20221210_2356.cpython-310.pyc
+-rw-rw-rw-   0        0        0      551 2022-12-10 15:22:20.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0027_auto_20221211_0022.cpython-310.pyc
+-rw-rw-rw-   0        0        0      636 2022-12-10 17:02:14.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0028_auto_20221211_0202.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1231 2022-12-11 02:51:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0029_leavedep.cpython-310.pyc
+-rw-rw-rw-   0        0        0      621 2022-12-11 03:06:37.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0030_auto_20221211_1206.cpython-310.pyc
+-rw-rw-rw-   0        0        0      582 2022-12-11 04:17:00.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0031_leave_is_update.cpython-310.pyc
+-rw-rw-rw-   0        0        0      583 2022-12-17 06:24:49.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0032_leave_dep_send_pr.cpython-310.pyc
+-rw-rw-rw-   0        0        0      583 2022-12-17 06:40:16.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0033_leave_pr_confirm.cpython-310.pyc
+-rw-rw-rw-   0        0        0      557 2022-12-17 06:43:37.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0034_rename_pr_confirm_leave_pr_approve.cpython-310.pyc
+-rw-rw-rw-   0        0        0      853 2022-12-17 07:14:57.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0035_leave_file.cpython-310.pyc
+-rw-rw-rw-   0        0        0      580 2022-12-17 08:47:40.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0036_leave_unit_send_pr.cpython-310.pyc
+-rw-rw-rw-   0        0        0      631 2022-12-20 07:39:49.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0037_alter_leavetype_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      592 2022-12-20 07:43:20.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0038_alter_leavetype_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      634 2022-12-20 07:50:58.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0039_alter_leavetype_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      665 2022-12-20 07:55:32.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0040_alter_leavecount_balance.cpython-310.pyc
+-rw-rw-rw-   0        0        0      662 2022-12-20 07:56:02.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0041_alter_leavecount_total.cpython-310.pyc
+-rw-rw-rw-   0        0        0      646 2022-12-20 07:56:33.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0042_alter_leave_days.cpython-310.pyc
+-rw-rw-rw-   0        0        0      678 2022-12-20 07:58:45.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0043_leavecount_balance_carry.cpython-310.pyc
+-rw-rw-rw-   0        0        0      654 2022-12-20 08:17:44.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0044_leavecount_taken.cpython-310.pyc
+-rw-rw-rw-   0        0        0      810 2022-12-20 08:22:35.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0045_auto_20221220_1722.cpython-310.pyc
+-rw-rw-rw-   0        0        0      871 2022-12-20 08:25:17.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0046_month_year.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1293 2022-12-20 08:29:55.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0047_auto_20221220_1729.cpython-310.pyc
+-rw-rw-rw-   0        0        0      978 2022-12-21 01:08:12.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0048_auto_20221221_1008.cpython-310.pyc
+-rw-rw-rw-   0        0        0      843 2022-12-21 01:09:42.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0049_auto_20221221_1009.cpython-310.pyc
+-rw-rw-rw-   0        0        0      690 2022-12-21 02:48:03.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0050_leavecount_total_balance_leave.cpython-310.pyc
+-rw-rw-rw-   0        0        0      688 2022-12-21 02:56:19.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0051_alter_leavecount_taken.cpython-310.pyc
+-rw-rw-rw-   0        0        0      687 2022-12-25 12:08:43.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0052_leavecount_prov_total_earn.cpython-310.pyc
+-rw-rw-rw-   0        0        0      694 2022-12-25 12:23:40.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0053_leavecount_total_taken.cpython-310.pyc
+-rw-rw-rw-   0        0        0      885 2022-12-25 13:32:16.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0054_auto_20221225_2232.cpython-310.pyc
+-rw-rw-rw-   0        0        0      635 2022-12-26 14:37:20.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0055_leave_description.cpython-310.pyc
+-rw-rw-rw-   0        0        0      776 2022-12-29 17:21:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0056_auto_20221230_0221.cpython-310.pyc
+-rw-rw-rw-   0        0        0      517 2022-12-29 17:21:36.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0057_alter_leavecount_options.cpython-310.pyc
+-rw-rw-rw-   0        0        0      751 2023-01-10 05:27:31.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0058_leaveperiod_employee.cpython-310.pyc
+-rw-rw-rw-   0        0        0      676 2023-01-10 06:35:52.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0059_auto_20230110_1535.cpython-310.pyc
+-rw-rw-rw-   0        0        0      592 2023-01-13 15:25:02.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0060_leavecount_update_date.cpython-310.pyc
+-rw-rw-rw-   0        0        0      676 2023-01-14 03:47:32.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0061_leavecount_balance_month.cpython-310.pyc
+-rw-rw-rw-   0        0        0      612 2023-01-18 02:16:27.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0062_leavehr_comment.cpython-310.pyc
+-rw-rw-rw-   0        0        0      575 2023-01-19 02:02:21.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0063_leave_is_done.cpython-310.pyc
+-rw-rw-rw-   0        0        0      573 2023-01-22 06:45:26.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0064_leave_pr_send.cpython-310.pyc
+-rw-rw-rw-   0        0        0      583 2023-01-22 08:06:46.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0065_leave_vice_send_pr.cpython-310.pyc
+-rw-rw-rw-   0        0        0      582 2023-01-22 08:31:16.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0066_leave_pr_notify.cpython-310.pyc
+-rw-rw-rw-   0        0        0      589 2023-01-29 06:59:04.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0067_leave_is_send_to_div.cpython-310.pyc
+-rw-rw-rw-   0        0        0      765 2023-02-02 00:25:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0068_auto_20230202_0925.cpython-310.pyc
+-rw-rw-rw-   0        0        0      593 2023-02-02 05:46:50.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0069_leave_is_special.cpython-310.pyc
+-rw-rw-rw-   0        0        0      601 2023-02-02 05:47:54.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0070_leave_is_create_by_hr.cpython-310.pyc
+-rw-rw-rw-   0        0        0      799 2023-03-13 10:08:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0071_auto_20230313_1908.cpython-310.pyc
+-rw-rw-rw-   0        0        0      786 2023-03-13 14:31:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0072_auto_20230313_2331.cpython-310.pyc
+-rw-rw-rw-   0        0        0      810 2023-03-13 14:38:19.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0073_auto_20230313_2338.cpython-310.pyc
+-rw-rw-rw-   0        0        0      798 2023-03-13 14:41:58.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/0074_auto_20230313_2341.cpython-310.pyc
+-rw-rw-rw-   0        0        0      145 2022-11-07 13:19:39.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      143 2022-10-20 01:03:56.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      151 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11410 2023-05-30 19:39:55.000000 django-ipghrms-leave-1.2/leave/models.py
+-rw-rw-rw-   0        0        0      727 2022-12-11 02:52:39.000000 django-ipghrms-leave-1.2/leave/signals.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:52.223154 django-ipghrms-leave-1.2/leave/templates/
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.035820 django-ipghrms-leave-1.2/leave/templates/leave/
+-rw-rw-rw-   0        0        0     3156 2023-03-14 11:55:22.000000 django-ipghrms-leave-1.2/leave/templates/leave/bal_s_list.html
+-rw-rw-rw-   0        0        0     8894 2023-03-15 07:00:38.000000 django-ipghrms-leave-1.2/leave/templates/leave/c_apply_detail.html
+-rw-rw-rw-   0        0        0     2029 2023-03-14 11:58:26.000000 django-ipghrms-leave-1.2/leave/templates/leave/c_apply_list.html
+-rw-rw-rw-   0        0        0        0 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.2/leave/templates/leave/c_deleg_detail.html
+-rw-rw-rw-   0        0        0        0 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.2/leave/templates/leave/c_deleg_list.html
+-rw-rw-rw-   0        0        0    11028 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.2/leave/templates/leave/c_ver_detail.html
+-rw-rw-rw-   0        0        0     1630 2023-03-14 11:57:58.000000 django-ipghrms-leave-1.2/leave/templates/leave/c_ver_list.html
+-rw-rw-rw-   0        0        0        0 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.2/leave/templates/leave/dash.html
+-rw-rw-rw-   0        0        0     8646 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.2/leave/templates/leave/de_appr_detail.html
+-rw-rw-rw-   0        0        0     1629 2023-02-21 06:30:12.000000 django-ipghrms-leave-1.2/leave/templates/leave/de_appr_list.html
+-rw-rw-rw-   0        0        0     3714 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.2/leave/templates/leave/de_detail.html
+-rw-rw-rw-   0        0        0     1993 2023-03-14 11:41:50.000000 django-ipghrms-leave-1.2/leave/templates/leave/de_list.html
+-rw-rw-rw-   0        0        0     5899 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.2/leave/templates/leave/deleg_detail.html
+-rw-rw-rw-   0        0        0     1715 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.2/leave/templates/leave/deleg_list.html
+-rw-rw-rw-   0        0        0    15438 2023-03-14 11:47:10.000000 django-ipghrms-leave-1.2/leave/templates/leave/dep_detail.html
+-rw-rw-rw-   0        0        0     1979 2023-03-14 11:56:58.000000 django-ipghrms-leave-1.2/leave/templates/leave/dep_list.html
+-rw-rw-rw-   0        0        0     2096 2023-03-14 11:56:34.000000 django-ipghrms-leave-1.2/leave/templates/leave/dep_req_list.html
+-rw-rw-rw-   0        0        0        0 2022-10-19 02:39:30.000000 django-ipghrms-leave-1.2/leave/templates/leave/detail.html
+-rw-rw-rw-   0        0        0      233 2023-01-20 19:07:34.000000 django-ipghrms-leave-1.2/leave/templates/leave/error.html
+-rw-rw-rw-   0        0        0        0 2023-03-14 10:03:00.000000 django-ipghrms-leave-1.2/leave/templates/leave/error2.html
+-rw-rw-rw-   0        0        0     2388 2023-02-13 20:54:48.000000 django-ipghrms-leave-1.2/leave/templates/leave/form.html
+-rw-rw-rw-   0        0        0     2616 2023-05-30 19:16:08.000000 django-ipghrms-leave-1.2/leave/templates/leave/form2.html
+-rw-rw-rw-   0        0        0    12233 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.2/leave/templates/leave/hr_app_detail.html
+-rw-rw-rw-   0        0        0     2791 2023-02-08 23:36:22.000000 django-ipghrms-leave-1.2/leave/templates/leave/hr_app_list.html
+-rw-rw-rw-   0        0        0     9600 2023-03-15 07:00:54.000000 django-ipghrms-leave-1.2/leave/templates/leave/hr_cert_detail.html
+-rw-rw-rw-   0        0        0     2395 2023-02-08 23:45:10.000000 django-ipghrms-leave-1.2/leave/templates/leave/hr_cert_list.html
+-rw-rw-rw-   0        0        0    13993 2023-05-30 07:43:02.000000 django-ipghrms-leave-1.2/leave/templates/leave/hr_leave_record.html
+-rw-rw-rw-   0        0        0     2481 2023-04-10 17:37:56.000000 django-ipghrms-leave-1.2/leave/templates/leave/hr_period_list.html
+-rw-rw-rw-   0        0        0     8049 2023-04-10 17:41:00.000000 django-ipghrms-leave-1.2/leave/templates/leave/hr_raw_list.html
+-rw-rw-rw-   0        0        0     2160 2023-02-08 23:42:58.000000 django-ipghrms-leave-1.2/leave/templates/leave/list.html
+-rw-rw-rw-   0        0        0    11403 2023-03-15 07:01:00.000000 django-ipghrms-leave-1.2/leave/templates/leave/s_apply_detail.html
+-rw-rw-rw-   0        0        0     2355 2023-02-07 16:15:16.000000 django-ipghrms-leave-1.2/leave/templates/leave/s_apply_list.html
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.428929 django-ipghrms-leave-1.2/leave/templates/leave_chart/
+-rw-rw-rw-   0        0        0     3992 2023-01-29 14:41:00.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/chart_leave.html
+-rw-rw-rw-   0        0        0     1146 2023-01-23 16:35:15.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/emp.js
+-rw-rw-rw-   0        0        0     1334 2023-01-23 16:35:32.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type.js
+-rw-rw-rw-   0        0        0     2207 2023-02-05 07:02:46.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type2.js
+-rw-rw-rw-   0        0        0     2240 2023-01-30 01:41:48.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type3.js
+-rw-rw-rw-   0        0        0     2219 2023-02-05 07:27:37.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_month.js
+-rw-rw-rw-   0        0        0     2257 2023-02-05 07:35:06.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_month_unit.js
+-rw-rw-rw-   0        0        0     2211 2023-02-05 07:55:31.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_tri.js
+-rw-rw-rw-   0        0        0     2215 2023-02-05 07:17:54.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_unit.js
+-rw-rw-rw-   0        0        0     2211 2023-02-05 07:01:28.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year.js
+-rw-rw-rw-   0        0        0     2257 2023-02-05 07:28:20.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_month.js
+-rw-rw-rw-   0        0        0     2294 2023-02-05 07:57:33.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_month_unit.js
+-rw-rw-rw-   0        0        0     2249 2023-02-05 07:44:38.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_tri.js
+-rw-rw-rw-   0        0        0     2287 2023-02-05 08:07:00.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_tri_unit.js
+-rw-rw-rw-   0        0        0     2253 2023-02-05 07:21:46.000000 django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_unit.js
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.441084 django-ipghrms-leave-1.2/leave/templates/leave_print/
+-rw-rw-rw-   0        0        0     1869 2022-11-30 07:59:44.000000 django-ipghrms-leave-1.2/leave/templates/leave_print/layout.html
+-rw-rw-rw-   0        0        0     5245 2023-03-14 15:00:53.000000 django-ipghrms-leave-1.2/leave/templates/leave_print/leave_print.html
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.460562 django-ipghrms-leave-1.2/leave/templates/leave_report/
+-rw-rw-rw-   0        0        0    18125 2023-02-05 10:10:59.000000 django-ipghrms-leave-1.2/leave/templates/leave_report/dash.html
+-rw-rw-rw-   0        0        0     1956 2023-02-05 08:54:19.000000 django-ipghrms-leave-1.2/leave/templates/leave_report/list.html
+-rw-rw-rw-   0        0        0     1917 2023-01-30 07:04:02.000000 django-ipghrms-leave-1.2/leave/templates/leave_report/list_day.html
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.490869 django-ipghrms-leave-1.2/leave/templates/pdf/
+-rw-rw-rw-   0        0        0      128 2023-02-24 10:02:16.000000 django-ipghrms-leave-1.2/leave/templates/pdf/cop.html
+-rw-rw-rw-   0        0        0      610 2023-02-02 15:25:15.000000 django-ipghrms-leave-1.2/leave/templates/pdf/layout.html
+-rw-rw-rw-   0        0        0     7845 2023-03-15 14:31:17.000000 django-ipghrms-leave-1.2/leave/templates/pdf/leave.html
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.493859 django-ipghrms-leave-1.2/leave/templatetags/
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.496851 django-ipghrms-leave-1.2/leave/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      483 2023-01-14 07:10:52.000000 django-ipghrms-leave-1.2/leave/templatetags/__pycache__/orderby.cpython-310.pyc
+-rw-rw-rw-   0        0        0      215 2023-01-14 07:10:49.000000 django-ipghrms-leave-1.2/leave/templatetags/orderby.py
+-rw-rw-rw-   0        0        0       60 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/tests.py
+-rw-rw-rw-   0        0        0     5470 2023-05-30 07:29:56.000000 django-ipghrms-leave-1.2/leave/urls.py
+-rw-rw-rw-   0        0        0     2788 2023-02-05 10:03:59.000000 django-ipghrms-leave-1.2/leave/urls_report.py
+-rw-rw-rw-   0        0        0    15575 2023-05-30 07:51:10.000000 django-ipghrms-leave-1.2/leave/utils.py
+-rw-rw-rw-   0        0        0     2737 2023-03-13 18:08:06.000000 django-ipghrms-leave-1.2/leave/utils_2.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.694988 django-ipghrms-leave-1.2/leave/views/
+-rw-rw-rw-   0        0        0      325 2023-01-29 14:29:10.000000 django-ipghrms-leave-1.2/leave/views/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:04:54.789717 django-ipghrms-leave-1.2/leave/views/__pycache__/
+-rw-rw-rw-   0        0        0      417 2023-01-29 14:29:14.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      370 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      378 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3566 2023-03-15 10:05:12.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2343 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2331 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2601 2023-01-29 07:19:53.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2460 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2469 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0      737 2023-01-23 14:19:18.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_chart.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2506 2023-03-15 10:08:49.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1993 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1980 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2279 2023-02-20 14:30:35.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1550 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1574 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0    25037 2023-03-13 19:37:38.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1813 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1814 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0    10718 2023-03-13 18:47:18.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2398 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2192 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11609 2023-03-13 18:27:21.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6368 2022-11-07 06:40:44.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0     6062 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0    17186 2023-02-15 01:07:16.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_report.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2026 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s.cpython-39.pyc
+-rw-rw-rw-   0        0        0      821 2022-11-07 13:19:37.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0      819 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_m.cpython-37.pyc
+-rw-rw-rw-   0        0        0      827 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4849 2023-03-15 14:22:55.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2143 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     2161 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1279 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_staff.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3232 2023-03-13 18:30:54.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1961 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_v.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1926 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/leave_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1565 2022-11-07 13:19:37.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/print.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1555 2022-10-20 01:02:26.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/print.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1571 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/__pycache__/print.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4191 2023-03-15 10:04:22.000000 django-ipghrms-leave-1.2/leave/views/leave_c_m.py
+-rw-rw-rw-   0        0        0     2732 2023-01-29 07:19:51.000000 django-ipghrms-leave-1.2/leave/views/leave_c_v.py
+-rw-rw-rw-   0        0        0      527 2023-01-23 14:19:06.000000 django-ipghrms-leave-1.2/leave/views/leave_chart.py
+-rw-rw-rw-   0        0        0     2610 2023-03-15 10:08:46.000000 django-ipghrms-leave-1.2/leave/views/leave_de_m.py
+-rw-rw-rw-   0        0        0     2853 2023-02-20 14:30:30.000000 django-ipghrms-leave-1.2/leave/views/leave_de_v.py
+-rw-rw-rw-   0        0        0    73902 2023-05-30 19:13:30.000000 django-ipghrms-leave-1.2/leave/views/leave_hr_m.py
+-rw-rw-rw-   0        0        0    44603 2023-02-09 05:04:14.000000 django-ipghrms-leave-1.2/leave/views/leave_hr_m_back.py
+-rw-rw-rw-   0        0        0    16680 2023-03-13 18:47:16.000000 django-ipghrms-leave-1.2/leave/views/leave_hr_v.py
+-rw-rw-rw-   0        0        0    20569 2023-03-13 18:27:19.000000 django-ipghrms-leave-1.2/leave/views/leave_m.py
+-rw-rw-rw-   0        0        0    31199 2023-02-15 01:07:13.000000 django-ipghrms-leave-1.2/leave/views/leave_report.py
+-rw-rw-rw-   0        0        0      514 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/leave_s_m.py
+-rw-rw-rw-   0        0        0     5451 2023-03-15 14:22:52.000000 django-ipghrms-leave-1.2/leave/views/leave_s_v.py
+-rw-rw-rw-   0        0        0     3684 2023-03-13 18:30:52.000000 django-ipghrms-leave-1.2/leave/views/leave_v.py
+-rw-rw-rw-   0        0        0     1674 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views/print.py
+-rw-rw-rw-   0        0        0       63 2022-10-18 10:39:30.000000 django-ipghrms-leave-1.2/leave/views.py
+-rw-rw-rw-   0        0        0      505 2023-05-30 20:04:54.804682 django-ipghrms-leave-1.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-leave-1.2/setup.py
```

### Comparing `django-ipghrms-leave-1.1/LICENSE` & `django-ipghrms-leave-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/django_ipghrms_leave.egg-info/SOURCES.txt` & `django-ipghrms-leave-1.2/django_ipghrms_leave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/api/__pycache__/urls.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/api/__pycache__/urls.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/api/__pycache__/views.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/api/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/api/urls.py` & `django-ipghrms-leave-1.2/leave/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/api/views.py` & `django-ipghrms-leave-1.2/leave/api/views.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/forms.py` & `django-ipghrms-leave-1.2/leave/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,25 +173,27 @@
 			),
 			HTML(""" <button class="btn btn-primary" type="submit" title="Rai">Rai <i class="fa fa-save"></i></button> """)
 		)
 
 class HRPeriodForm(forms.ModelForm):
 	class Meta:
 		model = LeavePeriod
-		fields = ['start_year','end_year']
+		fields = ['start_year','end_year', 'balance_carry']
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.helper = FormHelper()
 		self.fields['start_year'].required=True
 		self.fields['end_year'].required=True
 		self.helper.form_method = 'post'
+		self.fields['balance_carry'].label = 'Balance Carry Forward (Opsional)'
 		self.helper.layout = Layout(
 			Row(
-                Column('start_year', css_class='form-group col-md-6 mb-0'),
-				Column('end_year', css_class='form-group col-md-6 mb-0'),
+                Column('start_year', css_class='form-group col-md-4 mb-0'),
+				Column('end_year', css_class='form-group col-md-4 mb-0'),
+				Column('balance_carry', css_class='form-group col-md-4 mb-0'),
 				css_class='form-row'
 			),
 			HTML(""" <button class="btn btn-primary" type="submit" title="Rai">Rai <i class="fa fa-save"></i></button> """)
 		)
 
 class LeaveDelegateForm1(forms.ModelForm):
 	class Meta:
```

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0001_initial.py` & `django-ipghrms-leave-1.2/leave/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0004_alter_leavedelegate_employee.py` & `django-ipghrms-leave-1.2/leave/migrations/0004_alter_leavedelegate_employee.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0008_rename_de_confirm_leave_de_approve_and_more.py` & `django-ipghrms-leave-1.2/leave/migrations/0008_rename_de_confirm_leave_de_approve_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0009_rename_is_lock_leave_s_is_finish_and_more.py` & `django-ipghrms-leave-1.2/leave/migrations/0009_rename_is_lock_leave_s_is_finish_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.py` & `django-ipghrms-leave-1.2/leave/migrations/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.py` & `django-ipghrms-leave-1.2/leave/migrations/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0012_alter_leavedelegate_leave_alter_leaveunit_leave.py` & `django-ipghrms-leave-1.2/leave/migrations/0012_alter_leavedelegate_leave_alter_leaveunit_leave.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0014_leavehr_leavede.py` & `django-ipghrms-leave-1.2/leave/migrations/0014_leavehr_leavede.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.py` & `django-ipghrms-leave-1.2/leave/migrations/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.py` & `django-ipghrms-leave-1.2/leave/migrations/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0021_leave_is_approve_leave_is_reject.py` & `django-ipghrms-leave-1.2/leave/migrations/0021_leave_is_approve_leave_is_reject.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0022_rename_s_is_finish_leave_is_delegate_and_more.py` & `django-ipghrms-leave-1.2/leave/migrations/0022_rename_s_is_finish_leave_is_delegate_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0025_auto_20221210_2329.py` & `django-ipghrms-leave-1.2/leave/migrations/0025_auto_20221210_2329.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0026_auto_20221210_2356.py` & `django-ipghrms-leave-1.2/leave/migrations/0026_auto_20221210_2356.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0028_auto_20221211_0202.py` & `django-ipghrms-leave-1.2/leave/migrations/0028_auto_20221211_0202.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0029_leavedep.py` & `django-ipghrms-leave-1.2/leave/migrations/0029_leavedep.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0030_auto_20221211_1206.py` & `django-ipghrms-leave-1.2/leave/migrations/0030_auto_20221211_1206.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0035_leave_file.py` & `django-ipghrms-leave-1.2/leave/migrations/0035_leave_file.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0045_auto_20221220_1722.py` & `django-ipghrms-leave-1.2/leave/migrations/0045_auto_20221220_1722.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0046_month_year.py` & `django-ipghrms-leave-1.2/leave/migrations/0046_month_year.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0047_auto_20221220_1729.py` & `django-ipghrms-leave-1.2/leave/migrations/0047_auto_20221220_1729.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0048_auto_20221221_1008.py` & `django-ipghrms-leave-1.2/leave/migrations/0048_auto_20221221_1008.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0049_auto_20221221_1009.py` & `django-ipghrms-leave-1.2/leave/migrations/0049_auto_20221221_1009.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0054_auto_20221225_2232.py` & `django-ipghrms-leave-1.2/leave/migrations/0054_auto_20221225_2232.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0056_auto_20221230_0221.py` & `django-ipghrms-leave-1.2/leave/migrations/0056_auto_20221230_0221.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0058_leaveperiod_employee.py` & `django-ipghrms-leave-1.2/leave/migrations/0058_leaveperiod_employee.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0059_auto_20230110_1535.py` & `django-ipghrms-leave-1.2/leave/migrations/0059_auto_20230110_1535.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0068_auto_20230202_0925.py` & `django-ipghrms-leave-1.2/leave/migrations/0068_auto_20230202_0925.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0071_auto_20230313_1908.py` & `django-ipghrms-leave-1.2/leave/migrations/0071_auto_20230313_1908.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0072_auto_20230313_2331.py` & `django-ipghrms-leave-1.2/leave/migrations/0072_auto_20230313_2331.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0073_auto_20230313_2338.py` & `django-ipghrms-leave-1.2/leave/migrations/0073_auto_20230313_2338.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/0074_auto_20230313_2341.py` & `django-ipghrms-leave-1.2/leave/migrations/0074_auto_20230313_2341.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0001_initial.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0001_initial.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0002_remove_taskdelegate_date.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0003_rename_taskdelegate_leavedelegate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0004_alter_leavedelegate_employee.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0005_rename_is_approve_leavedelegate_is_confirm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0006_leavedelegate_is_confirm2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0007_leavetype_total.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0007_leavetype_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0007_leavetype_total.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0007_leavetype_total.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0007_leavetype_total.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0007_leavetype_total.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0008_rename_de_confirm_leave_de_approve_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0009_rename_is_lock_leave_s_is_finish_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0010_leave_de_obs_leave_hr_obs_leave_unit_obs.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0011_remove_leave_de_obs_remove_leave_hr_obs_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0012_alter_leavedelegate_leave_alter_leaveunit_leave.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0013_leave_is_finish.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0013_leave_is_finish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0013_leave_is_finish.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0013_leave_is_finish.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0013_leave_is_finish.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0013_leave_is_finish.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0014_leavehr_leavede.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0015_alter_leavede_obs_alter_leavedelegate_obs_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0016_leave_is_print.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0016_leave_is_print.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0016_leave_is_print.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0016_leave_is_print.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0016_leave_is_print.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0016_leave_is_print.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0017_remove_leavecount_datetime_remove_leavecount_hashed_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0018_alter_leavecount_balance.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0019_leave_s_is_delegate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0020_remove_leave_s_is_delegate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0021_leave_is_approve_leave_is_reject.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0022_rename_s_is_finish_leave_is_delegate_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0023_remove_leavedelegate_is_send.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0024_alter_leave_is_active.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0025_auto_20221210_2329.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0025_auto_20221210_2329.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0026_auto_20221210_2356.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0026_auto_20221210_2356.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0027_auto_20221211_0022.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0027_auto_20221211_0022.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0028_auto_20221211_0202.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0028_auto_20221211_0202.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0029_leavedep.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0029_leavedep.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0030_auto_20221211_1206.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0030_auto_20221211_1206.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0031_leave_is_update.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0031_leave_is_update.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0032_leave_dep_send_pr.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0032_leave_dep_send_pr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0033_leave_pr_confirm.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0033_leave_pr_confirm.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0034_rename_pr_confirm_leave_pr_approve.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0034_rename_pr_confirm_leave_pr_approve.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0035_leave_file.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0035_leave_file.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0036_leave_unit_send_pr.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0036_leave_unit_send_pr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0037_alter_leavetype_total.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0037_alter_leavetype_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0038_alter_leavetype_total.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0038_alter_leavetype_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0039_alter_leavetype_total.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0039_alter_leavetype_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0040_alter_leavecount_balance.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0040_alter_leavecount_balance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0041_alter_leavecount_total.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0041_alter_leavecount_total.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0042_alter_leave_days.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0042_alter_leave_days.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0043_leavecount_balance_carry.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0043_leavecount_balance_carry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0044_leavecount_taken.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0044_leavecount_taken.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0045_auto_20221220_1722.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0045_auto_20221220_1722.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0046_month_year.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0046_month_year.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0047_auto_20221220_1729.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0047_auto_20221220_1729.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0048_auto_20221221_1008.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0048_auto_20221221_1008.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0049_auto_20221221_1009.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0049_auto_20221221_1009.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0050_leavecount_total_balance_leave.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0050_leavecount_total_balance_leave.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0051_alter_leavecount_taken.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0051_alter_leavecount_taken.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0052_leavecount_prov_total_earn.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0052_leavecount_prov_total_earn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0053_leavecount_total_taken.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0053_leavecount_total_taken.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0054_auto_20221225_2232.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0054_auto_20221225_2232.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0055_leave_description.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0055_leave_description.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0056_auto_20221230_0221.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0056_auto_20221230_0221.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0057_alter_leavecount_options.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0057_alter_leavecount_options.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0058_leaveperiod_employee.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0058_leaveperiod_employee.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0059_auto_20230110_1535.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0059_auto_20230110_1535.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0060_leavecount_update_date.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0060_leavecount_update_date.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0061_leavecount_balance_month.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0061_leavecount_balance_month.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0062_leavehr_comment.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0062_leavehr_comment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0063_leave_is_done.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0063_leave_is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0064_leave_pr_send.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0064_leave_pr_send.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0065_leave_vice_send_pr.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0065_leave_vice_send_pr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0066_leave_pr_notify.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0066_leave_pr_notify.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0067_leave_is_send_to_div.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0067_leave_is_send_to_div.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0068_auto_20230202_0925.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0068_auto_20230202_0925.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0069_leave_is_special.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0069_leave_is_special.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0070_leave_is_create_by_hr.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0070_leave_is_create_by_hr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0071_auto_20230313_1908.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0071_auto_20230313_1908.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0072_auto_20230313_2331.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0072_auto_20230313_2331.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0073_auto_20230313_2338.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0073_auto_20230313_2338.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/migrations/__pycache__/0074_auto_20230313_2341.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/migrations/__pycache__/0074_auto_20230313_2341.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/models.py` & `django-ipghrms-leave-1.2/leave/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 	employee = models.ForeignKey(Employee, on_delete=models.CASCADE, related_name='leaveperiod', null=True)
 	start_month = models.ForeignKey(Month, on_delete=models.CASCADE, null=True, blank=True, verbose_name="Fulan Hahu", related_name="start_month")
 	start_year = models.ForeignKey(Year, on_delete=models.CASCADE, null=True, blank=True, verbose_name="Tinan Hahu", related_name="start_year")
 	start_date = models.DateField(null=True, blank=True, verbose_name="Data Hahu")
 	end_date = models.DateField(null=True, blank=True, verbose_name="Data Remate")
 	end_month = models.ForeignKey(Month, on_delete=models.CASCADE, null=True, blank=True, verbose_name="Fulan Remata", related_name="end_month")
 	end_year = models.ForeignKey(Year, on_delete=models.CASCADE, null=True, blank=True, verbose_name="Tinan Remata", related_name="end_year")
+	balance_carry = models.DecimalField(max_digits=5, decimal_places=2, null=True, blank=True, default=0.00, verbose_name="Balansu Carry Forward") # Balance Cary Forward
 	is_active = models.BooleanField(default=False)
 
 	def __str__(self):
-		return f'{self.start_month} - {self.start_year} - {self.end_month} - {self.end_year}'
+		return f'{self.employee} - {self.start_month} - {self.start_year} - {self.end_month} - {self.end_year}'
 	
 
 class LeaveType(models.Model):
 	name = models.CharField(max_length=20, null=True, blank=True, verbose_name="Naran")
 	total = models.DecimalField(max_digits=5, decimal_places=2, null=True, blank=True)
 	start_total = models.DecimalField(max_digits=5, decimal_places=2, null=True, blank=True, verbose_name="Balance Start")
 	def __str__(self):
```

### Comparing `django-ipghrms-leave-1.1/leave/signals.py` & `django-ipghrms-leave-1.2/leave/signals.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/bal_s_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/bal_s_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/c_apply_detail.html` & `django-ipghrms-leave-1.2/leave/templates/leave/c_apply_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/c_apply_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/c_apply_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/c_ver_detail.html` & `django-ipghrms-leave-1.2/leave/templates/leave/c_ver_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/c_ver_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/c_ver_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/de_appr_detail.html` & `django-ipghrms-leave-1.2/leave/templates/leave/de_appr_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/de_appr_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/de_appr_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/de_detail.html` & `django-ipghrms-leave-1.2/leave/templates/leave/de_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/de_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/de_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/deleg_detail.html` & `django-ipghrms-leave-1.2/leave/templates/leave/deleg_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/deleg_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/deleg_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/dep_detail.html` & `django-ipghrms-leave-1.2/leave/templates/leave/dep_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/dep_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/dep_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/dep_req_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/dep_req_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/form.html` & `django-ipghrms-leave-1.2/leave/templates/leave/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/form2.html` & `django-ipghrms-leave-1.2/leave/templates/leave/form2.html`

 * *Files 12% similar despite different names*

```diff
@@ -50,15 +50,20 @@
 					</table>
 				</div>
 				<div class="card-body">
 					<div class="row">
 						<div class="col-md-12">
 							<div class="alert alert-info">
 								<i class="fa fa-circle-info"> </i> 
-								<small> </i> <i>Koluna sira ne'ebe iha <strong class="text-danger">*</strong> signifika Itaboot tenke prienche</i> </small>
+								<small>  <i>Koluna sira ne'ebe iha <strong class="text-danger">*</strong> signifika Itaboot tenke prienche</i> </small>
+								{% if page == 'add-emp-record' %}
+								<br>
+								<small>  <i>Koluna <strong>Balance Carry Forward </strong> aplika deit ba Licensa Anterior nebe <strong>Lakonsege</strong> Kria  </i> </small>
+								  
+								{% endif %}
 							</div>
 						</div>
 					</div>
 					{% crispy form %}
 				</div> <!--end card-body-->
 			</div> <!--end card-->
 		</div> <!--end col-->
```

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/hr_app_detail.html` & `django-ipghrms-leave-1.2/leave/templates/leave/hr_app_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/hr_app_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/hr_app_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/hr_cert_detail.html` & `django-ipghrms-leave-1.2/leave/templates/leave/hr_cert_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/hr_cert_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/hr_cert_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/hr_leave_record.html` & `django-ipghrms-leave-1.2/leave/templates/leave/hr_leave_record.html`

 * *Files 9% similar despite different names*

```diff
@@ -14,25 +14,33 @@
 	<div class="row">
 		<div class="col-sm-12">
 			<div class="card shadow-lg border-info rounded">
 				<div class="card-header border-primary">
 
 					<center>
 						<h2>{{ legend|upper }}</h2>
-						<h5>Periode : 
+						<h5> 
 							{% if period %}
 							{{period}}
 							
 							{% else %}
 							<span class="badge bg-danger text-white">SEIDAUK IHA PERIODO</span>
 							{% endif %}
 						</h5>
 					</center>
 				</div>
 				<div class="card-body">
+					<div class="alert alert-info">
+						<i class="fa fa-info-circle"></i> Nota: 
+						<br>
+						<small>Molok Kria Periode Licensa, halo favor hare uluk Funsionariu/a nia <strong>Data Kontratu Hahu</strong></small> <br>
+						<small>Butaun <strong>Aumenta Licensa Tuir Prosesu</strong>; Aplika dei ba Funsionariu/a <strong>La Inklui</strong> Chefe Ekipa no Diretor</small>
+						<br>
+						<small>Wainhira Ita kria ona <strong>Licensa Tuir Prosesu</strong> ba Funsionariu Ida; Etapa tuir mai mak Iha parte okos Historia Licensa, klik butaun <strong>Manda</strong></small>
+					</div>
 					<p style="font-size: 13px;" class="p-0 mb-1">Name of Staff:  <b>{{employee|upper}}</b> </p>
 					<p style="font-size: 13px;" class="p-0 mb-1">Position:  <b>{{employee.curempposition.position.name|upper}}</b> </p>
 					<p style="font-size: 13px;" class="p-0 mb-1">Contract Start Date:  <b>{{contract.start_date|date:"d F Y"}}</b> </p>
 					<p style="font-size: 13px;" class="p-0 ">Contract End Date:  <b> 
 						{% if contract.end_date %}
 							{{contract.end_date|date:"d F Y"}}
 						{% else %}
@@ -51,20 +59,21 @@
 							{% if leavecheck and today <= period.end_date %}
 								<!-- <a href="{% url 'leave-hr-add' employee.hashed %}" class="btn btn-sm btn-info mb-2">Aumenta Licensa <i class="fa fa-plus"></i></a> -->
 								
 							{% elif today <= period.end_date and leavecheck %}
 								<!-- <a href="{% url 'leave-hr-leave-update-emp-record' employee.hashed  %}" class="btn btn-sm btn-info mb-2">Kria Record <i class="fa fa-gear"></i></a> -->
 							{% endif %}
 							{% if lc == False %}
-								<a href="{% url 'leave-hr-leave-update-emp-record' employee.hashed  %}" class="btn btn-sm btn-danger mb-2">Kria Record <i class="fa fa-gear"></i></a>
+								<a href="{% url 'leave-hr-leave-update-emp-record' employee.hashed  %}" id="create-record" class="btn btn-sm btn-danger mb-2">Kria Record <i class="fa fa-gear"></i></a>
 							
 							{% endif %}
 							{% if leavecheck %}
 									<a href="{% url 'leave-hr-add' employee.hashed %}" class="btn btn-sm btn-success mb-2">Aumenta Licensa <i class="fa fa-plus"></i></a>						  
 									<a href="{% url 'leave-hr-add-special' employee.hashed %}" class="btn btn-sm btn-danger mb-2">Aumenta Licensa Special <i class="fa fa-plus"></i></a>						  
+									<a href="{% url 'leave-hr-add-process' employee.hashed %}" class="btn btn-sm btn-warning mb-2">Aumenta Licensa Tuir Prosesu <i class="fa fa-plus"></i></a>						  
 							{% endif %}
 					{% else %}
 					
 					<a href="{% url 'leave-hr-leave-create-emp-record' employee.hashed %}" class="btn btn-info btn-sm mb-2">Kria Periode Licensa <i class="fa fa-plus"></i></a>
 					{% endif %}
 					<table class="table table-sm table-striped table-responsive table-bordered" id="example" width="100%" cellspacing="0">
 						<thead>
@@ -99,14 +108,19 @@
 						<tbody>
 							{% for obj in  objects %}
 								{% if last_count_period %}
 									<tr align="center">
 										<td colspan="3"  class="text-center">Balance Carry Forward {{last_count_period.period.start_year}} - {{last_count_period.period.end_year}}</td>
 										<td class="text-danger" class="text-center">{{last_count_period.total_balance}}</td>
 									</tr>
+								{% elif period.balance_carry %}
+									<tr align="center">
+										<td colspan="3"  class="text-center">Balance Carry Forward (Last Period)</td>
+										<td class="text-danger" class="text-center">{{period.balance_carry}}</td>
+									</tr>
 								{% endif %}
 							  	{% for obj1 in data  %}
 									<tr>
 										<td class="text-center"><small>{{obj1.0|date:"d-M-"}}</small></td>
 										<td class="text-center">
 											{% if obj1.1.update_date <= today %}
 												{{obj1.1.leave_earn}}
@@ -208,15 +222,16 @@
 									</th>
 									<th class="text-center">{{obj2.0.total_taken}}</th>
 									<th class="text-center">
 										
 										{% if today <= obj2.0.update_date %}
 												{{obj2.9.balance_month}}
 										{% elif obj2.7 and   today  >=  obj2.10.update_date  %}
-												{{obj2.10.total_earn}} 
+												<!-- {{obj2.10.total_earn}}  -->
+												{{obj2.0.total_balance}}
 										{% elif obj2.7 %}
 												{{obj2.9.balance_month}}
 										{% else %}
 										
 											{{obj2.0.total_balance}}
 												
 										{% endif %}
@@ -253,15 +268,15 @@
 		</div> <!--end col-->
 		<div class="col-md-12">
 			<div class="card">
 				<div class="card-header border-primary">
 
 					<center>
 						<h2>HISTORIA LICENSA</h2>
-						<h5>Periode : {{period}}</h5>
+						<h5> {{period}}</h5>
 					</center>
 				</div>
 				<div class="card-body">
 					
 					<table class="table table-md table-striped table-bordered" id="example2">
 						<thead>
 							<tr class="text-center">
@@ -271,14 +286,15 @@
 								<th>Tipu Licensa</th>
 								<th>Data Hahu</th>
 								<th>Data Remata</th>
 								<th>Loron</th>
 								<th>Status</th>
 								<th>File</th>
 								<th>Kria Husi</th>
+								<th class="text-center">#</th>
 							</tr>
 						</thead>
 						<tbody>
 							{% for obj in  leave %}
 							  <tr class="text-center">
 								<td>{{forloop.counter}}</td>
 								<td>{{obj.description}}</td>
@@ -295,14 +311,19 @@
 								</td>
 								<td>
 									{% if obj.file %}
 									  <a href="{{obj.file.url}}" target="_blank" class="btn btn-sm btn-info"> <i class="fa fa-file"></i> </a>
 									{% endif %}
 								</td>
 								<td>{{obj.user.employeeuser.employee}}</td>
+								<td>
+									{% if obj.is_create_by_hr and obj.is_lock == False and obj.is_send == False and obj.is_special == False %}
+									  	<a href="{% url 'leave-hr-send-process' obj.employee.hashed obj.hashed %}" class="btn btn-sm btn-primary">Manda <i class="fa fa-send"></i></a>
+									{% endif %}
+								</td>
 							  </tr>
 							{% endfor %}
 						</tbody>
 					</table>
 				</div>
 			</div>
 		</div>
@@ -324,8 +345,23 @@
 			$('#example2').DataTable({
 				pageLength: 13,
 				"ordering": false
 			});
 
 		} );
 	</script>
+	<script>
+		var submitLink = document.getElementById('create-record');
+		submitLink.addEventListener('click', function(e) {
+		  e.preventDefault(); 
+		  submitLink.disabled = true;
+		  submitLink.innerHTML = 'Please wait...';
+	  
+		  var href = submitLink.href;
+		  setTimeout(function() {
+			window.location.href = href;
+		  }, 500); 
+		});
+	  </script>
+	  
+	  
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,15 +1,21 @@
 {% extends "main/layout.html" %} {% load orderby %} {% block content %}
     * LISTA_APLIKASAUN
     * RAW_DATA_LICENSA
     * {{ legend|upper }}
 
                         ***** {{ legend|upper }} *****
-** Periode : {% if period %} {{period}} {% else %} SEIDAUK IHA PERIODO {% endif
-                                     %} **
+  ** {% if period %} {{period}} {% else %} SEIDAUK IHA PERIODO {% endif %} **
+ Nota:
+Molok Kria Periode Licensa, halo favor hare uluk Funsionariu/a nia Data
+Kontratu Hahu
+Butaun Aumenta Licensa Tuir Prosesu; Aplika dei ba Funsionariu/a La Inklui
+Chefe Ekipa no Diretor
+Wainhira Ita kria ona Licensa Tuir Prosesu ba Funsionariu Ida; Etapa tuir mai
+mak Iha parte okos Historia Licensa, klik butaun Manda
 Name of Staff: {{employee|upper}}
 Position: {{employee.curempposition.position.name|upper}}
 Contract Start Date: {{contract.start_date|date:"d F Y"}}
 Contract End Date: {% if contract.end_date %} {{contract.end_date|date:"d F
 Y"}} {% else %}  Indeterminable {% endif %}
 ===============================================================================
 {% if period %} {% if today >= period.end_date and lc %} {% if page != 'list-
@@ -19,22 +25,25 @@
 elif today <= period.end_date and leavecheck %}  {% endif %} {% if lc == False
 %}
 Kria_Record
  {% endif %} {% if leavecheck %}
 Aumenta_Licensa
 
 Aumenta_Licensa_Special
+
+Aumenta_Licensa_Tuir_Prosesu
  {% endif %} {% else %}
 Kria_Periode_Licensa
  {% endif %}
       Month    Annual Leave Earn          Taken (Days)                        Balance        Special Leave =            Taken (Days)                    Balance       Sick Leave = 12            Taken (days)                    Balance       Maternity Leave            Taken (days)                    Balance       Paternity Leave            Taken (days)                    Balance       Childcare Leave            Taken (days)                    Balance
               (days) = 20 Days/Year                                                            3 Days/Year                                                               Days/Year                                                             = 12 Weeks/Year                                                           = 5 Days/Year                                                            = 5 Days/Year
                      Balance Carry Forward {                              {
            {last_count_period.period.start_year}} - {     {last_count_period.total_balance}}
               {last_count_period.period.end_year}}
+                Balance Carry Forward (Last Period)              {{period.balance_carry}}
               {% if                 {% if obj1.1.taken != {% if obj1.1.update_date <= today
 {             obj1.1.update_date <= 0.00 %}  {            %} {{obj1.1.balance}} {% else %}   {                {% if obj1.3.taken != 0.00                              {                {% if obj1.2.taken != 0.00                              {                {% if obj1.4.taken != 0.00                              {                {% if obj1.5.taken != 0.00                              {                {% if obj1.6.taken != 0.00
 {obj1.0|date: today %} {            {obj1.1.taken}}  {%   {% if obj1.7 %} {                  {obj1.3.month}}- %}  {{obj1.3.taken}}  {%   {{obj1.3.total_balance}}     {obj1.2.month}}- %}  {{obj1.2.taken}}  {%   {{obj1.2.total_balance}}     {obj1.4.month}}- %}  {{obj1.4.taken}}  {%   {{obj1.4.total_balance}}     {obj1.5.month}}- %}  {{obj1.5.taken}}  {%   {{obj1.5.total_balance}}     {obj1.6.month}}- %}  {{obj1.6.taken}}  {%   {{obj1.6.total_balance}}
 "d-M-"}}      {obj1.1.leave_earn}}  else %} 0.00 {% endif {obj1.1.balance_month}} {% else %} {{obj1.3.year}}  else %} 0.00 {% endif %}                                {{obj1.2.year}}  else %} 0.00 {% endif %}                                {{obj1.4.year}}  else %} 0.00 {% endif %}                                {{obj1.5.year}}  else %} 0.00 {% endif %}                                {{obj1.6.year}}  else %} 0.00 {% endif %}
               {% else %} 0.00 {%    %}                    0.00 {% endif %} {% endif %}
               endif %}
                {% if obj2.7 %} {%
@@ -43,16 +52,16 @@
               %} {
               {obj2.10.total_earn}}
               {% elif today <
               obj2.10.update_date
               %} {                                        {% if today <= obj2.0.update_date
               {obj2.8.total_earn}}                        %} {{obj2.9.balance_month}} {%
               {% else %} {                                elif obj2.7 and today >=
-              {obj2.0.total_earn}}                        obj2.10.update_date %} {
-TOTAL         {% endif %} {% else   {                     {obj2.10.total_earn}} {% elif      -                {                          {                            -                {                          {                            -                {                          {                            -                {                          {                            -                {                          {
+              {obj2.0.total_earn}}                        obj2.10.update_date %}  {
+TOTAL         {% endif %} {% else   {                     {obj2.0.total_balance}} {% elif    -                {                          {                            -                {                          {                            -                {                          {                            -                {                          {                            -                {                          {
               %} {% if today >=     {obj2.0.total_taken}} obj2.7 %} {{obj2.9.balance_month}}                  {obj2.1.last.total_taken}} {obj2.1.last.total_balance}}                  {obj2.2.last.total_taken}} {obj2.2.last.total_balance}}                  {obj2.3.last.total_taken}} {obj2.3.last.total_balance}}                  {obj2.4.last.total_taken}} {obj2.4.last.total_balance}}                  {obj2.5.last.total_taken}} {obj2.5.last.total_balance}}
               obj2.10.update_date                         {% else %} {
               %} {                                        {obj2.0.total_balance}} {% endif
               {obj2.10.total_earn}}                       %}
               {% elif today <
               obj2.10.update_date
               %} {
@@ -61,17 +70,21 @@
               {obj2.0.total_earn}}
               {% endif %} {% endif
               %}
    1. {% for y in all_period %}
    2. {{_y.start_year_}}_-_{{y.end_year}}
    3. {% endfor %}
                          ***** HISTORIA LICENSA *****
-                          ** Periode : {{period}} **
-Nu.                Deskrisaun Licensa Data Aplika Tipu Licensa      Data Hahu             Data Remata         Loron       Status         File     Kria Husi
-                                                                                                                          {% if
-                                                                    {                     {                               obj.is_special {% if
-{                  {                  {           {                 {obj.start_date|date: {obj.end_date|date: {           %} Special  {% obj.file {
-{forloop.counter}} {obj.description}} {obj.date}} {obj.leave_type}} "d-F-Y"}}             "d-F-Y"}}           {obj.days}} else %}        %}  {%   {obj.user.employeeuser.employee}}
-                                                                                                                          Regular  {%    endif %}
-                                                                                                                          endif %}
+                               ** {{period}} **
+Nu.                Deskrisaun Licensa Data Aplika Tipu Licensa      Data Hahu             Data Remata         Loron       Status         File     Kria Husi                         #
+                                                                                                                                                                                    {% if
+                                                                                                                                                                                    obj.is_create_by_hr
+                                                                                                                          {% if                                                     and obj.is_lock ==
+                                                                    {                     {                               obj.is_special {% if                                      False and
+{                  {                  {           {                 {obj.start_date|date: {obj.end_date|date: {           %} Special  {% obj.file {                                 obj.is_send ==
+{forloop.counter}} {obj.description}} {obj.date}} {obj.leave_type}} "d-F-Y"}}             "d-F-Y"}}           {obj.days}} else %}        %}  {%   {obj.user.employeeuser.employee}} False and
+                                                                                                                          Regular  {%    endif %}                                   obj.is_special ==
+                                                                                                                          endif %}                                                  False %}
+                                                                                                                                                                                    Manda
+                                                                                                                                                                                     {% endif %}
 {% endblock %} {% block scripts %}
  {% endblock %}
```

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/hr_period_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/hr_period_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/hr_raw_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/hr_raw_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/s_apply_detail.html` & `django-ipghrms-leave-1.2/leave/templates/leave/s_apply_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave/s_apply_list.html` & `django-ipghrms-leave-1.2/leave/templates/leave/s_apply_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/chart_leave.html` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/chart_leave.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/emp.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/emp.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type2.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type2.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type3.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type3.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_month.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_month.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_month_unit.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_month_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_tri.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_tri.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_unit.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_month.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_month.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_month_unit.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_month_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_tri.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_tri.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_tri_unit.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_tri_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_chart/type_year_unit.js` & `django-ipghrms-leave-1.2/leave/templates/leave_chart/type_year_unit.js`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_print/layout.html` & `django-ipghrms-leave-1.2/leave/templates/leave_print/layout.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_print/leave_print.html` & `django-ipghrms-leave-1.2/leave/templates/leave_print/leave_print.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_report/dash.html` & `django-ipghrms-leave-1.2/leave/templates/leave_report/dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_report/list.html` & `django-ipghrms-leave-1.2/leave/templates/leave_report/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/leave_report/list_day.html` & `django-ipghrms-leave-1.2/leave/templates/leave_report/list_day.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/pdf/layout.html` & `django-ipghrms-leave-1.2/leave/templates/pdf/layout.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/templates/pdf/leave.html` & `django-ipghrms-leave-1.2/leave/templates/pdf/leave.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/urls.py` & `django-ipghrms-leave-1.2/leave/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,19 +52,21 @@
 	path('hr/leave/update/record/month/<str:hashid>/', views.hrLeaveEmpUpdatePeriodMonth, name="leave-hr-leave-update-emp-record-month"),
 	path('hr/leave/update/record/', views.hrLeaveUpdateRecord, name="leave-hr-leave-update-record"),
 	path('hr/period/set/', views.hrLeavePeriodAdd, name="leave-hr-period-set"),
 	path('hr/leave/list/', views.hrLeaveAppList, name="leave-hr-app-list"),
 	path('hr/leave/raw/list/', views.hrLeaveAppRawList, name="leave-hr-app-raw-list"),
 	path('hr/leave/add/<str:hashid>/', views.hrLeaveAdd, name="leave-hr-add"),
 	path('hr/leave/add/spec/<str:hashid>/', views.hrLeaveAddSpecial, name="leave-hr-add-special"),
+	path('hr/leave/add/proc/<str:hashid>/', views.hrLeaveAddProcess, name="leave-hr-add-process"),
 	path('hr/app/detail/<str:hashid>/', views.hrLeaveAppDetail, name="leave-hr-app-detail"),
 	path('hr/update/att/<str:hashid>/<str:hashid2>/', views.hrLeaveUpdateAtt, name="leave-hr-udpate-att"),
 	path('hr/print/<str:hashid>/', views.hrLeavePrint, name="leave-hr-print"),
 	path('hr/add/comment/<str:hashid>/', views.hrLeaveAddComment, name="leave-hr-add-comment"),
 	path('hr/pdf/<str:hashid>/', views.hrLeavePDF, name="leave-hr-pdf"),
+	path('hr/leave-send-process/<str:hashid>/<str:leave>/', views.hrLeaveSendProcess, name="leave-hr-send-process"),
 	### DE
 	path('pr/list/', views.deLeaveList, name="leave-de-list"),
 	path('pr/detail/<str:hashid>/', views.deLeaveDetail, name="leave-de-detail"),
 	path('pr/aprove/list/', views.deLeaveApprList, name="leave-de-appr-list"),
 	path('pr/aprove/detail/<str:hashid>/', views.deLeaveApprDetail, name="leave-de-appr-detail"),
 	path('pr/aprove/update/<str:hashid>/', views.deLeaveApprUpdate, name="leave-de-appr-update"),
 	path('pr/aprove/finish/<str:hashid>/', views.deLeaveApprFinish, name="leave-de-appr-finish"),
```

### Comparing `django-ipghrms-leave-1.1/leave/urls_report.py` & `django-ipghrms-leave-1.2/leave/urls_report.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/utils.py` & `django-ipghrms-leave-1.2/leave/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,14 +236,16 @@
     instance.id = newid
     instance.hashed = new_hashid
     instance.employee = employee
     instance.leave_period = leave_period
     instance.user = request.user
     instance.datetime = timezone.now()
     instance.pr_approve = True
+    instance.is_lock = True
+    instance.is_send = True
     instance.is_approve = True
     instance.is_finish = True
     instance.hr_confirm = True
     instance.is_done = True
     instance.is_create_by_hr = True
     instance.save()
 
@@ -260,14 +262,25 @@
     instance.is_finish = True
     instance.hr_confirm = True
     instance.is_done = True
     instance.is_special = True
     instance.is_create_by_hr = True
     instance.save()
 
+def createLeaveProcess(request, instance, newid, new_hashid, employee, leave_period):
+    instance.id = newid
+    instance.hashed = new_hashid
+    instance.employee = employee
+    instance.leave_period = leave_period
+    instance.user = request.user
+    instance.datetime = timezone.now()
+    instance.hr_confirm = True
+    instance.is_create_by_hr = True
+    instance.save()
+
 def check_period_date(period_date):
     check_period = False
     current_date = datetime.now()
     str_date = f"{period_date.year}-{period_date.month}-{period_date.day}"
     input_month = int(str_date.split("-")[1])
     input_day = int(str_date.split("-")[2])
```

### Comparing `django-ipghrms-leave-1.1/leave/utils_2.py` & `django-ipghrms-leave-1.2/leave/utils_2.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_m.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_m.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_m.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_v.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_v.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_c_v.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_c_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_chart.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_chart.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_m.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_m.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_m.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_v.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_v.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_de_v.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_de_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_m.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_m.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_m.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_v.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_v.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_hr_v.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_hr_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_m.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_m.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_m.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_report.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_m.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_m.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_m.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_m.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_v.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_v.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_s_v.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_s_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_staff.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_staff.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_v.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_v.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_v.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/leave_v.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/leave_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/print.cpython-310.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/print.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/print.cpython-37.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/print.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/__pycache__/print.cpython-39.pyc` & `django-ipghrms-leave-1.2/leave/views/__pycache__/print.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_c_m.py` & `django-ipghrms-leave-1.2/leave/views/leave_c_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_c_v.py` & `django-ipghrms-leave-1.2/leave/views/leave_c_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_chart.py` & `django-ipghrms-leave-1.2/leave/views/leave_chart.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_de_m.py` & `django-ipghrms-leave-1.2/leave/views/leave_de_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_de_v.py` & `django-ipghrms-leave-1.2/leave/views/leave_de_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_hr_m.py` & `django-ipghrms-leave-1.2/leave/views/leave_hr_m_back.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import datetime
 from django.shortcuts import render, redirect, get_object_or_404
 from django.contrib.auth.decorators import login_required
 from settings_app.decorators import allowed_users
 from django.contrib import messages
 from employee.models import CurEmpDivision, Employee
 from leave.models import Leave, LeaveHR, LeaveUnit, LeaveCount, LeavePeriod, Month as Mnth, Year as Yr, LeaveType
-from leave.forms import LeaveHRForm, LeaveUnitForm, LeaveForm, HRLeaveForm, HRPeriodForm, HRLeaveCommentForm, HRLeaveFormSpecial
+from leave.forms import LeaveHRForm, LeaveUnitForm, LeaveForm, HRLeaveForm, HRPeriodForm, HRLeaveCommentForm
 from settings_app.utils import getnewid
 from settings_app.user_utils import c_staff, c_unit
 from dateutil.parser import parser
 from datetime import datetime as dt
 from datetime import timedelta
 from attendance.models import Attendance, AttendanceStatus,Year, Month
 import pytz
 import pandas as pd
 from django.db.models import Q, F
 from django.utils import timezone
 from calendar import mdays
 from attendance.models import Attendance, AttendanceStatus, Year as YAten, Month as Maten
-from leave.utils import createAttendance,createAttendanceEmp, createLeave, count_day,calculate_hours, add_time, createAttendanceSpecial, createLeaveSpecial
+from leave.utils import createAttendance, createLeave
 from contract.models import Contract
 
 
-
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrLeaveCertUpdate(request, hashid):
 	leave = get_object_or_404(Leave, hashed=hashid)
 	empdiv = CurEmpDivision.objects.get(employee=leave.employee)
 	objects = LeaveHR.objects.get(leave=leave)
 	if request.method == 'POST':
@@ -88,460 +87,225 @@
 		leave_type = None
 		if employee.sex == 'Male':
 			leave_type = LeaveType.objects.exclude(pk=4)
 		else:
 			leave_type = LeaveType.objects.all()
 		today = dt.today().date()
 		leave_period = LeavePeriod.objects.filter(is_active=True, employee=employee).last()
-		if leave_period:
-			check_last_period = LeavePeriod.objects.filter(pk__lt=leave_period.pk, employee=employee).last()
-			last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
-			last_month_date = today.replace(day=1) - timedelta(days=1)
-			min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}-{leave_period.start_date.day}'
-			max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
+		check_last_period = LeavePeriod.objects.filter(pk__lt=leave_period.pk, employee=employee).last()
+		last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
+		last_month_date = today.replace(day=1) - timedelta(days=1)
+		min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}-{leave_period.start_date.day}'
+		max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
+
+		months = pd.period_range(min_month, max_month, freq='M')
+		i = 0
+		while i < len(months):
+			leave_check = LeaveCount.objects.filter(employee=employee, period=leave_period).last()
+			m = months[i]
+			get_m = get_object_or_404(Mnth, code=m.month)
+			get_y = get_object_or_404(Yr, year=m.year)
+			if leave_check:
+				for lt1 in leave_type:
+					if lt1.pk == 1:
+						print('CALLLL 1')
+						lastleaveal = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type_id=1).last()
+						earn_per_month = round(float(lt1.total/12),2)
+						date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
+						date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
+						lcnew = LeaveCount.objects.create(
+							period = leave_period,
+							employee=employee,
+							leave_type=lt1,
+							month = get_m,
+							year = get_y,
+							update_date=date_period,
+							leave_earn = earn_per_month
+						)
+						lcnew.balance = round(float(lastleaveal.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
+						lcnew.total_earn = round(float(lastleaveal.prov_total_earn) + float(lcnew.leave_earn),1)
+						lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
+						lcnew.balance_carry = lcnew.total_balance
+						lcnew.total_balance_leave = float(lt1.total) - float(lcnew.total_balance)
+						lcnew.prov_total_earn = float(lastleaveal.prov_total_earn) + float(earn_per_month)
+						lcnew.balance_month = round(float(lastleaveal.total_balance) - float(lcnew.taken),2)
+						lcnew.save()
+			else:
+				for lt in leave_type:
+					if lt.pk == 1:
+						# work: Check Balansu iha Periode Kotuk
+						date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
+						date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
+						if check_last_period:
+							print('CALLLL HEREE LAST PERIOD')
+							earn_per_month = round(float(lt.total/12),2)
 
-			months = pd.period_range(min_month, max_month, freq='M')
-			i = 0
-			while i < len(months):
-				leave_check = LeaveCount.objects.filter(employee=employee, period=leave_period).last()
-				m = months[i]
-				get_m = get_object_or_404(Mnth, code=m.month)
-				get_y = get_object_or_404(Yr, year=m.year)
-				if leave_check:
-					for lt1 in leave_type:
-						if lt1.pk == 1:
-							lastleaveal = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type_id=1).last()
-							earn_per_month = round(float(lt1.total/12),2)
-							date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
-							date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
-							lcnew = LeaveCount.objects.create(
+							lc = LeaveCount.objects.create(
 								period = leave_period,
 								employee=employee,
-								leave_type=lt1,
+								leave_type=lt,
 								month = get_m,
 								year = get_y,
 								update_date=date_period,
 								leave_earn = earn_per_month
 							)
-							lcnew.balance = round(float(lastleaveal.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
-							lcnew.total_earn = round(float(lastleaveal.prov_total_earn) + float(lcnew.leave_earn),1)
-							lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
-							lcnew.balance_carry = lcnew.total_balance
-							lcnew.total_balance_leave = float(lt1.total) - float(lcnew.total_balance)
-							lcnew.prov_total_earn = float(lastleaveal.prov_total_earn) + float(earn_per_month)
-							lcnew.balance_month = round(float(lastleaveal.total_balance) - float(lcnew.taken),2)
-							lcnew.save()
-				else:
-					for lt in leave_type:
-						if lt.pk == 1:
-							# work: Check Balance in Last Period
-							date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
-							date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
-							if check_last_period:
-								earn_per_month = round(float(lt.total/12),2)
-
-								lc = LeaveCount.objects.create(
-									period = leave_period,
-									employee=employee,
-									leave_type=lt,
-									month = get_m,
-									year = get_y,
-									update_date=date_period,
-									leave_earn = earn_per_month
-								)
-								lc.balance = round(float(last_count_period.total_balance) +   float(lc.leave_earn) - float(lc.taken),2)
-								lc.total_earn = round(float(lc.leave_earn) + float(last_count_period.total_balance),2)
-								lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
-								lc.balance_carry = lc.total_balance
-								lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
-								lc.prov_total_earn = lc.total_earn
-								lc.balance_month = round(float(lc.total_balance) - float(lc.taken),2)
-								lc.save()
-							else:
-								earn_per_month = round(float(lt.total/12),2)
-
-								lc = LeaveCount.objects.create(
-									period = leave_period,
-									employee=employee,
-									leave_type=lt,
-									month = get_m,
-									year = get_y,
-									update_date=date_period,
-									leave_earn = earn_per_month
-								)
-								lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
-								lc.total_earn = round(float(lc.leave_earn),2)
-								lc.total_balance = round(float(lc.balance),2)
-								lc.balance_carry = lc.total_balance
-								lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
-								lc.prov_total_earn = lc.leave_earn
-								lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
-								lc.save()
+							lc.balance = round(float(last_count_period.total_balance) +   float(lc.leave_earn) - float(lc.taken),2)
+							lc.total_earn = round(float(lc.leave_earn) + float(last_count_period.total_balance),2)
+							lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
+							lc.balance_carry = lc.total_balance
+							lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
+							lc.prov_total_earn = lc.total_earn
+							lc.balance_month = round(float(lc.total_balance) - float(lc.taken),2)
+							lc.save()
 						else:
-							lcall = LeaveCount.objects.create(
+							print('CALLLL HEREE LAST PERIOD ELSEE')
+							earn_per_month = round(float(lt.total/12),2)
+							# balance_per_month = round(float(earn_per_month) - float(taken),2)
+
+							lc = LeaveCount.objects.create(
 								period = leave_period,
 								employee=employee,
 								leave_type=lt,
+								month = get_m,
 								year = get_y,
+								update_date=date_period,
+								leave_earn = earn_per_month
 							)
-							lcall.total_balance = float(lt.total)
-							lcall.save()
-				
-				i+=1
+							lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
+							lc.total_earn = round(float(lc.leave_earn),2)
+							lc.total_balance = round(float(lc.balance),2)
+							lc.balance_carry = lc.total_balance
+							lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
+							lc.prov_total_earn = lc.leave_earn
+							lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
+							lc.save()
+					else:
+						lcall = LeaveCount.objects.create(
+							period = leave_period,
+							employee=employee,
+							leave_type=lt,
+							year = get_y,
+						)
+						lcall.total_balance = float(lt.total)
+						lcall.save()
+			
+			i+=1
 		messages.success(request, f'Susesu Update Record')
 		return redirect('leave-hr-leave-record', hashid=hashid)
 	else:
 		messages.error(request, f'Kontrato ba pessoal refere seidauk iha!!')
 		return redirect('leave-hr-leave-record', hashid=hashid)
 
 
 @login_required
-def hrLeaveAddSpecial(request, hashid):
-	group = request.user.groups.all()[0].name
-	employee = get_object_or_404(Employee, hashed=hashid)
-	leave_period = LeavePeriod.objects.filter(employee=employee,is_active=True).last()
-	check_last_period = LeavePeriod.objects.filter(employee=employee,  pk__lt=leave_period.pk).last()
-	last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
-	min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
-	max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
-	months = pd.period_range(min_month, max_month, freq='M')
-	today = dt.today().date()
-	c_emp = employee
-	emp = employee
-	if request.method == 'POST':
-		newid, new_hashid = getnewid(Leave)
-		form = HRLeaveFormSpecial(request.POST, request.FILES)
-		if form.is_valid():
-			leave_type = form.cleaned_data.get('leave_type')
-			start_time = form.cleaned_data.get('start_time')
-			start_time_str = start_time.strftime("%H:%M")
-			end_time = form.cleaned_data.get('end_time')
-			end_time_str = end_time.strftime("%H:%M")
-			tot_hours = calculate_hours(start_time_str, end_time_str)
-
-			days = tot_hours
-			# days = round(float(days),2)
-			if leave_type.pk == 1:
-				earn_per_month = round(float(leave_type.total/12),2)
-			else: earn_per_month = 0.00
-			start_date = form.cleaned_data.get('start_date')
-			end_date = form.cleaned_data.get('end_date')
-
-			min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
-			max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
-			date1 = pd.to_datetime(start_date, format="%Y %m").date()
-			date2 = pd.to_datetime(end_date, format="%Y %m").date()
-
-			start_date_period = pd.to_datetime(min_month, format="%Y %m").date()
-			end_date_period = pd.to_datetime(max_month, format="%Y %m").date()
-			start_month = date1
-			date_range = pd.date_range(start=start_date, end=end_date, freq="B")
-			total_length = len(date_range)
-			total_day = round(days * total_length,2)
-
-
-			# done: CHECK DATA LEAVE IHA PERIODO NIA LARAN
-			if start_date_period <= start_month <= end_date_period + datetime.timedelta(days=29):
-				current_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
-				if current_leave_count:
-					previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
-				leave_this_month = LeaveCount.objects.filter(period=leave_period, employee=employee, leave_type_id=1, update_date__lte=today).last()
-
-				if leave_this_month.balance >= 0.5:
-					if   total_day <= leave_this_month.balance or total_day <= leave_this_month.balance + 5 :
-						if total_day < 30  or total_day >= 30:
-							# check_day(days, current_leave_count, previous_leave_count)
-							# done: CHECK ANGKA LORON 0.5/1.0/1.5
-								
-								
-							# done: CHECK LEAVE TYPE BA ANNUAL
-							if leave_type.pk == 1:
-								# done: CHECK RECORD IHA FULAN IDA NE'E
-								current_leave_count = get_object_or_404(LeaveCount, period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year)
-								previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
-								# done: CHECK KARIK LEAVE IHA FULAN KLARAN
-								if previous_leave_count:
-									current_leave_count.taken = round(float(current_leave_count.taken) + total_day,2)
-									current_leave_count.total_taken = round(float(previous_leave_count.taken) + total_day)
-									current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(total_day),2 )
-									current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-									current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
-									current_leave_count.save()
-
-
-									#done: KRIA ATTENDANCE
-									createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten,start_time_str, end_time_str)							
-								# done: CHECK KARIK LEAVE IHA FULAN PRIMEIRU
-								else:
-									current_leave_count.taken = round(float(current_leave_count.taken) + total_day,2)
-									if check_last_period:
-										current_leave_count.total_earn = round(float(last_count_period.total_balance) + float(earn_per_month),1)
-										current_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) - float(current_leave_count.taken),2 )
-										current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-										current_leave_count.balance_month = round(float(current_leave_count.total_balance) - float(current_leave_count.taken),2)
-										current_leave_count.save()
-									else:
-										current_leave_count.total_taken = current_leave_count.taken
-										current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
-										current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-										current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
-										current_leave_count.save()
-
-									# done: KRIA ATTENDANCE
-									createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, start_time_str, end_time_str)
-
-
-								i = 0
-								# done: UPDATE LEAVE RECORD
-								while i < len(months):
-									m = months[i]
-									if i == int(0):
-										# work: First Month
-										if check_last_period:
-											first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
-											first_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) -  float(first_leave_count.taken),2)
-											first_leave_count.total_earn = round(float(first_leave_count.leave_earn) + float(last_count_period.total_balance),2)
-											first_leave_count.total_balance = round(float(first_leave_count.total_earn) - float(first_leave_count.total_taken),2)
-											first_leave_count.balance_carry = first_leave_count.total_balance
-											first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
-											first_leave_count.prov_total_earn = first_leave_count.total_earn
-											first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
-											first_leave_count.save()
-										else:
-											first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
-											first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
-											first_leave_count.total_earn = round(float(first_leave_count.leave_earn),2)
-											first_leave_count.total_balance = round(float(first_leave_count.balance),2)
-											first_leave_count.balance_carry = first_leave_count.total_balance
-											first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
-											first_leave_count.prov_total_earn = first_leave_count.leave_earn
-											first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
-											first_leave_count.save()
-
-									else:
-										prev_mont = m.asfreq("M", "S") - 1
-										lccurrent = get_object_or_404(LeaveCount, employee=employee, period=leave_period, leave_type=leave_type,  year__year=m.year, month__code=m.month)
-										lclast = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type,  year__year=prev_mont.year, month__code=prev_mont.month).first()
-
-
-										lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
-										lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
-										lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
-										lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
-										lccurrent.balance_carry = lccurrent.total_balance
-										lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
-										lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
-										lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
-										lccurrent.save()
-
-									i+=1
-
-								# done: KRIA LEAVE
-								instance = form.save(commit=False)
-								createLeaveSpecial(request, instance,newid,new_hashid, employee, leave_period, total_day)
-								messages.success(request, 'Leave Aumenta ho Susesu')
-								return redirect('leave-hr-leave-record', c_emp.hashed)
-
-
-
-							# done: CHECK KARIK LEAVE LAOS ANNUAL LEAVE
-							else:
-
-								lcount = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type, month__isnull=False)
-								getmonth = get_object_or_404(Mnth, code=start_date.month)
-								getyear = get_object_or_404(Yr, year=start_date.year)
-
-								# done: CHECK LEAVE COUNT NEBE IHA ONA MAIBE FULAN LAIHA
-								if lcount:
-									previous_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type=leave_type).last()
-									month_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
-									# work: Leave Nebe Iha ona
-									if days <= previous_leave_count.total_balance:
-										if month_leave_count:
-											month_leave_count.taken = round(float(month_leave_count.taken) + total_day, 2)
-											month_leave_count.total_taken = round(float(previous_leave_count.total_taken) +  total_day,2)
-											month_leave_count.total_taken = month_leave_count.taken
-											month_leave_count.total_balance = round(float(leave_type.total) - float(month_leave_count.total_taken),2)
-											month_leave_count.save()
-											instance = form.save(commit=False)
-											createLeaveSpecial(request, instance,newid,new_hashid, employee, leave_period, total_day)
-											createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, start_time_str, end_time_str)
-											messages.success(request, 'Leave Aumenta ho Susesu')
-											return redirect('leave-hr-leave-record', c_emp.hashed)
-										else:
-											lc = LeaveCount.objects.create(
-												period = leave_period,
-												employee = employee,
-												leave_type = leave_type,
-												year = getyear,
-												month = getmonth
-
-											)
-											lc.taken = total_day
-											lc.total_taken = round(float(previous_leave_count.total_taken) + float(lc.taken),2)
-											lc.total_balance = round(float(leave_type.total) - float(lc.total_taken),2)
-											lc.save()
-											instance = form.save(commit=False)
-
-											createLeaveSpecial(request, instance,newid,new_hashid, employee, leave_period, total_day)
-											createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, start_time_str, end_time_str)
-
-											messages.success(request, 'Leave Aumenta ho Susesu')
-											return redirect('leave-hr-leave-record', c_emp.hashed)
-									else:
-										messages.error(request, 'Loron nebe hili barak liu. Halo favor altera loron nebe ita prienche')
-								# done: CHECK LEAVE COUNT NEBE IHA NO FULAN ONA IHA
-								else:
-									lcount2 = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type)
-									lcount2.update(
-										month=getmonth,
-										year=getyear,
-										taken = total_day,
-										total_taken = total_day,
-										total_balance = round(float(leave_type.total) - float(total_day),2)
-									)
-									instance = form.save(commit=False)
-									createLeaveSpecial(request, instance,newid,new_hashid, employee, leave_period, total_day)
-
-									# KRIA ATTENDANCE
-									createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, start_time_str, end_time_str)
-
-									messages.success(request, 'Leave Aumenta ho Susesu')
-									return redirect('leave-hr-leave-record', c_emp.hashed)
-								
-								
-						else:
-							messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
-					else:
-						messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
-				else:
-					messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
-			# done: ERROR KARIK DATA HAHU LAIHA PERIODE NIA LARAN
-			else:
-				messages.error(request,'Data hahu laiha periode ida ne nia laran. Halo Favor Kria Uluk lai Periode Foun!!')
-
-			
-	else:
-		form = HRLeaveFormSpecial()
-	context = {
-		'group': group, 'c_emp': c_emp,  'page': 'record',
-		'form': form, 'emp':emp,
-		'title': 'Aplika Licensa', 'legend': 'Aplika Licensa'
-	}
-	return render(request, 'leave/form.html', context)
-
-
-
-@login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrLeaveUpdateRecord(request):
 	employee = Employee.objects.filter(status_id=1)
 	for emp in employee:
-		contract = Contract.objects.filter(employee=emp, is_active=True).exists()
-		if contract:
-			leave_type = None
-			if emp.sex == 'Male':
-				leave_type = LeaveType.objects.exclude(pk=4)
+		# work: Get Last Employee Leave Count
+		leave_type = None
+		if emp.sex == 'Male':
+			leave_type = LeaveType.objects.exclude(pk=4)
+		else:
+			leave_type = LeaveType.objects.all()
+		leave_type_al = LeaveType.objects.get(pk=1)
+		leave_period = LeavePeriod.objects.filter(is_active=True, employee=emp).last()
+		# work: Depois koko tan ida tan
+		check_last_period = LeavePeriod.objects.filter(pk__lt=leave_period.pk, employee=emp).last()
+		last_count_period = LeaveCount.objects.filter(employee=emp, period=check_last_period, leave_type_id=1).last()
+		min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
+		max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
+		months = pd.period_range(min_month, max_month, freq='M')
+		i = 0
+		while i < len(months):
+			leave_check = LeaveCount.objects.filter(employee=emp, period=leave_period).last()
+			m = months[i]
+			get_m = get_object_or_404(Mnth, code=m.month)
+			get_y = get_object_or_404(Yr, year=m.year)
+			if leave_check:
+				for lt1 in leave_type:
+					if lt1.pk == 1:
+						lastleaveal = LeaveCount.objects.filter(employee=emp, period=leave_period, leave_type_id=1).last()
+						earn_per_month = round(float(lt1.total/12),2)
+						date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
+						date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
+						lcnew = LeaveCount.objects.create(
+							period = leave_period,
+							employee=emp,
+							leave_type=lt1,
+							month = get_m,
+							year = get_y,
+							update_date = date_period,
+							leave_earn = earn_per_month
+						)
+						lcnew.balance = round(float(lastleaveal.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
+						lcnew.total_earn = round(float(lastleaveal.prov_total_earn) + float(lcnew.leave_earn),1)
+						lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
+						lcnew.balance_carry = lcnew.total_balance
+						lcnew.total_balance_leave = float(lt1.total) - float(lcnew.total_balance)
+						lcnew.prov_total_earn = float(lastleaveal.prov_total_earn) + float(earn_per_month)
+						lcnew.balance_month = round(float(lastleaveal.balance) - float(lcnew.taken),2)
+						lcnew.save()
 			else:
-				leave_type = LeaveType.objects.all()
-			leave_period = LeavePeriod.objects.filter(is_active=True, employee=emp).last()
-			check_last_period = LeavePeriod.objects.filter(pk__lt=leave_period.pk, employee=emp).last()
-			last_count_period = LeaveCount.objects.filter(employee=emp, period=check_last_period, leave_type_id=1).last()
-			min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
-			max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
-			months = pd.period_range(min_month, max_month, freq='M')
-			check_leave_count = LeaveCount.objects.filter(period=leave_period, employee=emp).exists()
-			if check_leave_count == False:
-				i = 0
-				while i < len(months):
-					leave_check = LeaveCount.objects.filter(employee=emp, period=leave_period).last()
-					m = months[i]
-					get_m = get_object_or_404(Mnth, code=m.month)
-					get_y = get_object_or_404(Yr, year=m.year)
-					if leave_check:
-						for lt1 in leave_type:
-							if lt1.pk == 1:
-								lastleaveal = LeaveCount.objects.filter(employee=emp, period=leave_period, leave_type_id=1).last()
-								earn_per_month = round(float(lt1.total/12),2)
-								date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
-								date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
-								lcnew = LeaveCount.objects.create(
-									period = leave_period,
-									employee=emp,
-									leave_type=lt1,
-									month = get_m,
-									year = get_y,
-									update_date = date_period,
-									leave_earn = earn_per_month
-								)
-								lcnew.balance = round(float(lastleaveal.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
-								lcnew.total_earn = round(float(lastleaveal.prov_total_earn) + float(lcnew.leave_earn),1)
-								lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
-								lcnew.balance_carry = lcnew.total_balance
-								lcnew.total_balance_leave = float(lt1.total) - float(lcnew.total_balance)
-								lcnew.prov_total_earn = float(lastleaveal.prov_total_earn) + float(earn_per_month)
-								lcnew.balance_month = round(float(lastleaveal.balance) - float(lcnew.taken),2)
-								lcnew.save()
-					else:
-						for lt in leave_type:
-							if lt.pk == 1:
-								# work: Check Balansu iha Periode Kotuk
-								date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
-								date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
-								if check_last_period:
-									earn_per_month = round(float(lt.total/12),2)
+				for lt in leave_type:
+					if lt.pk == 1:
+						# work: Check Balansu iha Periode Kotuk
+						date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
+						date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
+						if check_last_period:
+							earn_per_month = round(float(lt.total/12),2)
 
-									lc = LeaveCount.objects.create(
-										period = leave_period,
-										employee=emp,
-										leave_type=lt,
-										month = get_m,
-										year = get_y,
-										update_date=date_period,
-										leave_earn = earn_per_month
-									)
-									lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
-									lc.total_earn = round(float(lc.leave_earn) + float(last_count_period.total_balance),2)
-									lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
-									lc.balance_carry = lc.total_balance
-									lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
-									lc.prov_total_earn = lc.total_earn
-									lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
-									lc.save()
-								else:
-									earn_per_month = round(float(lt.total/12),2)
-									# balance_per_month = round(float(earn_per_month) - float(taken),2)
+							lc = LeaveCount.objects.create(
+								period = leave_period,
+								employee=emp,
+								leave_type=lt,
+								month = get_m,
+								year = get_y,
+								update_date=date_period,
+								leave_earn = earn_per_month
+							)
+							lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
+							lc.total_earn = round(float(lc.leave_earn) + float(last_count_period.total_balance),2)
+							lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
+							lc.balance_carry = lc.total_balance
+							lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
+							lc.prov_total_earn = lc.total_earn
+							lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
+							lc.save()
+						else:
+							earn_per_month = round(float(lt.total/12),2)
+							# balance_per_month = round(float(earn_per_month) - float(taken),2)
 
-									lc = LeaveCount.objects.create(
-										period = leave_period,
-										employee=emp,
-										leave_type=lt,
-										month = get_m,
-										year = get_y,
-										update_date=date_period,
-										leave_earn = earn_per_month
-									)
-									lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
-									lc.total_earn = round(float(lc.leave_earn),2)
-									lc.total_balance = round(float(lc.balance),2)
-									lc.balance_carry = lc.total_balance
-									lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
-									lc.prov_total_earn = lc.leave_earn
-									lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
-									lc.save()
-							else:
-								lcall = LeaveCount.objects.create(
-									period = leave_period,
-									employee=emp,
-									leave_type=lt,
-									year = get_y,
-								)
-								lcall.total_balance = float(lt.total)
-								lcall.save()
-					i+=1
+							lc = LeaveCount.objects.create(
+								period = leave_period,
+								employee=emp,
+								leave_type=lt,
+								month = get_m,
+								year = get_y,
+								update_date=date_period,
+								leave_earn = earn_per_month
+							)
+							lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
+							lc.total_earn = round(float(lc.leave_earn),2)
+							lc.total_balance = round(float(lc.balance),2)
+							lc.balance_carry = lc.total_balance
+							lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
+							lc.prov_total_earn = lc.leave_earn
+							lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
+							lc.save()
+					else:
+						lcall = LeaveCount.objects.create(
+							period = leave_period,
+							employee=emp,
+							leave_type=lt,
+							year = get_y,
+						)
+						lcall.total_balance = float(lt.total)
+						lcall.save()
+			i+=1
 	messages.success(request, f'Susesu Update Record')
 	return redirect('leave-hr-app-raw-list')
 	
 
 def update_leave_count(alldata, month):
 
 	for obj in alldata:
@@ -549,24 +313,24 @@
 
 
 @login_required
 def hrLeaveAdd(request, hashid):
 	group = request.user.groups.all()[0].name
 	employee = get_object_or_404(Employee, hashed=hashid)
 	leave_period = LeavePeriod.objects.filter(employee=employee,is_active=True).last()
-	check_last_period = LeavePeriod.objects.filter(employee=employee,  pk__lt=leave_period.pk).last()
+	check_last_period = LeavePeriod.objects.filter(employee=employee, is_active=True, pk__lt=leave_period.pk).last()
 	last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
 	min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
 	max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
 	months = pd.period_range(min_month, max_month, freq='M')
-	today = dt.today().date()
 	c_emp = employee
 	emp = employee
 	if request.method == 'POST':
 		newid, new_hashid = getnewid(Leave)
+		newsid2, _ = getnewid(LeaveCount)
 		form = HRLeaveForm(request.POST, request.FILES)
 		if form.is_valid():
 			leave_type = form.cleaned_data.get('leave_type')
 			days = form.cleaned_data.get('days')
 			days = round(float(days),2)
 			if leave_type.pk == 1:
 				earn_per_month = round(float(leave_type.total/12),2)
@@ -580,208 +344,202 @@
 			max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
 			date1 = pd.to_datetime(start_date, format="%Y %m").date()
 			date2 = pd.to_datetime(end_date, format="%Y %m").date()
 
 			start_date_period = pd.to_datetime(min_month, format="%Y %m").date()
 			end_date_period = pd.to_datetime(max_month, format="%Y %m").date()
 			start_month = date1
-			cal_day = count_day(start_date, end_date)
-			
-			if float(cal_day) >= days:
 
-				# done: CHECK DATA LEAVE IHA PERIODO NIA LARAN
-				if start_date_period <= start_month <= end_date_period + datetime.timedelta(days=29):
-					current_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
-					if current_leave_count:
-						previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
-					leave_this_month = LeaveCount.objects.filter(period=leave_period, employee=employee, leave_type_id=1, update_date__lte=today).last()
-							
-					if leave_this_month.balance >= 0.5:
-						if   days <= leave_this_month.balance or days <= leave_this_month.balance + 5 :
-							if days < 30  or days >= 30:
-								# check_day(days, current_leave_count, previous_leave_count)
-								# done: CHECK ANGKA LORON 0.5/1.0/1.5
-								if last_two_digits == int(5) or last_two_digits == int(0):
-									
-									
-									
-									# done: CHECK LEAVE TYPE BA ANNUAL
-									if leave_type.pk == 1:
-										# done: CHECK RECORD IHA FULAN IDA NE'E
-										# current_leave_count = get_object_or_404(LeaveCount, period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year)
-										# previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
-										# done: CHECK KARIK LEAVE IHA FULAN KLARAN
-										if previous_leave_count:
-											current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
-											current_leave_count.total_taken = round(float(previous_leave_count.taken) + days)
-											current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(days),2 )
-											current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-											current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
-											current_leave_count.save()
-
-
-											#done: KRIA ATTENDANCE
-											createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)							
-										# done: CHECK KARIK LEAVE IHA FULAN PRIMEIRU
-										else:
-											current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
-											if check_last_period:
-												current_leave_count.total_earn = round(float(last_count_period.total_balance) + float(earn_per_month),1)
-												current_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) - float(current_leave_count.taken),2 )
-												current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-												current_leave_count.balance_month = round(float(current_leave_count.total_balance) - float(current_leave_count.taken),2)
-												current_leave_count.save()
-											else:
-												current_leave_count.total_taken = current_leave_count.taken
-												current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
-												current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-												current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
-												current_leave_count.save()
-
-											# done: KRIA ATTENDANCE
-											createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
-
-
-										i = 0
-										# done: UPDATE LEAVE RECORD
-										while i < len(months):
-											m = months[i]
-											if i == int(0):
-												# work: First Month
-												if check_last_period:
-													first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
-													first_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) -  float(first_leave_count.taken),2)
-													first_leave_count.total_earn = round(float(first_leave_count.leave_earn) + float(last_count_period.total_balance),2)
-													first_leave_count.total_balance = round(float(first_leave_count.total_earn) - float(first_leave_count.total_taken),2)
-													first_leave_count.balance_carry = first_leave_count.total_balance
-													first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
-													first_leave_count.prov_total_earn = first_leave_count.total_earn
-													first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
-													first_leave_count.save()
-												else:
-													first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
-													first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
-													first_leave_count.total_earn = round(float(first_leave_count.leave_earn),2)
-													first_leave_count.total_balance = round(float(first_leave_count.balance),2)
-													first_leave_count.balance_carry = first_leave_count.total_balance
-													first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
-													first_leave_count.prov_total_earn = first_leave_count.leave_earn
-													first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
-													first_leave_count.save()
-
-											else:
-												prev_mont = m.asfreq("M", "S") - 1
-												lccurrent = get_object_or_404(LeaveCount, employee=employee, period=leave_period, leave_type=leave_type,  year__year=m.year, month__code=m.month)
-												lclast = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type,  year__year=prev_mont.year, month__code=prev_mont.month).first()
-
-
-												lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
-												lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
-												lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
-												lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
-												lccurrent.balance_carry = lccurrent.total_balance
-												lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
-												lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
-												lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
-												lccurrent.save()
 
-											i+=1
+			if days <= leave_type.total:
+				# done: CHECK ANGKA LORON 0.5/1.0/1.5
+				if last_two_digits == int(5) or last_two_digits == int(0):
+					# done: CHECK DATA LEAVE IHA PERIODO NIA LARAN
+					if start_date_period <= start_month <= end_date_period + datetime.timedelta(days=29):
+						# done: CHECK LEAVE TYPE BA ANNUAL
+						if leave_type.pk == 1:
+							print('ADDD  CALL 1')
+							# done: CHECK RECORD IHA FULAN IDA NE'E
+							current_leave_count = get_object_or_404(LeaveCount, period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year)
+							previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
+							# done: CHECK KARIK LEAVE IHA FULAN KLARAN
+							if previous_leave_count:
+								# print('ADDD  CALL 2')
+								# if check_last_period:
+								# 	print('ADDD  CALL 3')
+								# 	current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
+								# 	current_leave_count.total_taken = round(float(previous_leave_count.taken) + days)
+								# 	current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(days),2 )
+								# 	current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+								# 	current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
+								# 	current_leave_count.save()
+								# else:
+								current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
+								current_leave_count.total_taken = round(float(previous_leave_count.taken) + days)
+								current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(days),2 )
+								current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+								current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
+								current_leave_count.save()
+
+
+								#done: KRIA ATTENDANCE
+								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)							
+							# done: CHECK KARIK LEAVE IHA FULAN PRIMEIRU
+							else:
+								print('ANOTHER CALL 1')
+								current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
+								if check_last_period:
+									print('ANOTHER CALL 2')
+									current_leave_count.total_earn = round(float(last_count_period.total_balance) + float(earn_per_month),1)
+									current_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) - float(current_leave_count.taken),2 )
+									current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+									current_leave_count.balance_month = round(float(current_leave_count.total_balance) - float(current_leave_count.taken),2)
+									current_leave_count.save()
+								else:
+									print('ANOTHER CALL 3')
+									current_leave_count.total_taken = current_leave_count.taken
+									current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
+									current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+									current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
+									current_leave_count.save()
+
+								# done: KRIA ATTENDANCE
+								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+
 
-										# done: KRIA LEAVE
+							i = 0
+							# done: UPDATE LEAVE RECORD
+							while i < len(months):
+								m = months[i]
+								if i == int(0):
+									# work: First Month
+									if check_last_period:
+										print('PRINT CALL UPDATE CHEK LAST PERIOD')
+										first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+										first_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) -  float(first_leave_count.taken),2)
+										first_leave_count.total_earn = round(float(first_leave_count.leave_earn) + float(last_count_period.total_balance),2)
+										first_leave_count.total_balance = round(float(first_leave_count.total_earn) - float(first_leave_count.total_taken),2)
+										first_leave_count.balance_carry = first_leave_count.total_balance
+										first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
+										first_leave_count.prov_total_earn = first_leave_count.total_earn
+										first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+										first_leave_count.save()
+										print('PRINT CALL UPDATE CHEK LAST PERIOD ---- NOT')
+									else:
+										first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+										first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
+										first_leave_count.total_earn = round(float(first_leave_count.leave_earn),2)
+										first_leave_count.total_balance = round(float(first_leave_count.balance),2)
+										first_leave_count.balance_carry = first_leave_count.total_balance
+										first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
+										first_leave_count.prov_total_earn = first_leave_count.leave_earn
+										first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+										first_leave_count.save()
+
+								else:
+									# work: Next Month
+									prev_mont = m.asfreq("M", "S") - 1
+									lccurrent = get_object_or_404(LeaveCount, employee=employee, period=leave_period, leave_type=leave_type,  year__year=m.year, month__code=m.month)
+									lclast = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type,  year__year=prev_mont.year, month__code=prev_mont.month).first()
+
+
+									lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
+									lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
+									lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
+									lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
+									lccurrent.balance_carry = lccurrent.total_balance
+									lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
+									lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
+									lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
+									lccurrent.save()
+
+								i+=1
+
+							# done: KRIA LEAVE
+							instance = form.save(commit=False)
+							createLeave(request, instance,newid,new_hashid, employee, leave_period)
+							messages.success(request, 'Leave Aumenta ho Susesu')
+							return redirect('leave-hr-leave-record', c_emp.hashed)
+
+						# done: CHECK KARIK LEAVE LAOS ANNUAL LEAVE
+						else:
+
+							lcount = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type, month__isnull=False)
+							getmonth = get_object_or_404(Mnth, code=start_date.month)
+							getyear = get_object_or_404(Yr, year=start_date.year)
+
+							# done: CHECK LEAVE COUNT NEBE IHA ONA MAIBE FULAN LAIHA
+							if lcount:
+								previous_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type=leave_type).last()
+								month_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
+								# work: Leave Nebe Iha ona
+								if days <= previous_leave_count.total_balance:
+									if month_leave_count:
+										month_leave_count.taken = round(float(month_leave_count.taken) + days, 2)
+										month_leave_count.total_taken = round(float(previous_leave_count.total_taken) +  days,2)
+										print(month_leave_count.taken)
+										# month_leave_count.total_taken = month_leave_count.taken
+										print(month_leave_count.total_taken)
+										month_leave_count.total_balance = round(float(leave_type.total) - float(month_leave_count.total_taken),2)
+										print(month_leave_count.total_balance)
+										month_leave_count.save()
 										instance = form.save(commit=False)
 										createLeave(request, instance,newid,new_hashid, employee, leave_period)
+										createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
 										messages.success(request, 'Leave Aumenta ho Susesu')
 										return redirect('leave-hr-leave-record', c_emp.hashed)
-
-
-
-									# done: CHECK KARIK LEAVE LAOS ANNUAL LEAVE
 									else:
+										lc = LeaveCount.objects.create(
+											period = leave_period,
+											employee = employee,
+											leave_type = leave_type,
+											year = getyear,
+											month = getmonth
+
+										)
+										lc.taken = days
+										lc.total_taken = round(float(previous_leave_count.total_taken) + float(lc.taken),2)
+										lc.total_balance = round(float(leave_type.total) - float(lc.total_taken),2)
+										lc.save()
+										instance = form.save(commit=False)
+
+										createLeave(request, instance,newid,new_hashid, employee, leave_period)
+										createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
 
-										lcount = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type, month__isnull=False)
-										getmonth = get_object_or_404(Mnth, code=start_date.month)
-										getyear = get_object_or_404(Yr, year=start_date.year)
-
-										# done: CHECK LEAVE COUNT NEBE IHA ONA MAIBE FULAN LAIHA
-										if lcount:
-											previous_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type=leave_type).last()
-											month_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
-											# work: Leave Nebe Iha ona
-											if days <= previous_leave_count.total_balance:
-												if month_leave_count:
-													month_leave_count.taken = round(float(month_leave_count.taken) + days, 2)
-													month_leave_count.total_taken = round(float(previous_leave_count.total_taken) +  days,2)
-													# month_leave_count.total_taken = month_leave_count.taken
-													month_leave_count.total_balance = round(float(leave_type.total) - float(month_leave_count.total_taken),2)
-													month_leave_count.save()
-													instance = form.save(commit=False)
-													createLeave(request, instance,newid,new_hashid, employee, leave_period)
-													createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
-													messages.success(request, 'Leave Aumenta ho Susesu')
-													return redirect('leave-hr-leave-record', c_emp.hashed)
-												else:
-													lc = LeaveCount.objects.create(
-														period = leave_period,
-														employee = employee,
-														leave_type = leave_type,
-														year = getyear,
-														month = getmonth
-
-													)
-													lc.taken = days
-													lc.total_taken = round(float(previous_leave_count.total_taken) + float(lc.taken),2)
-													lc.total_balance = round(float(leave_type.total) - float(lc.total_taken),2)
-													lc.save()
-													instance = form.save(commit=False)
-
-													createLeave(request, instance,newid,new_hashid, employee, leave_period)
-													createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
-
-													messages.success(request, 'Leave Aumenta ho Susesu')
-													return redirect('leave-hr-leave-record', c_emp.hashed)
-											else:
-												messages.error(request, 'Loron nebe hili barak liu. Halo favor altera loron nebe ita prienche')
-										# done: CHECK LEAVE COUNT NEBE IHA NO FULAN ONA IHA
-										else:
-											lcount2 = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type)
-											lcount2.update(
-												month=getmonth,
-												year=getyear,
-												taken = days,
-												total_taken = days,
-												total_balance = round(float(leave_type.total) - float(days),2)
-											)
-											instance = form.save(commit=False)
-											createLeave(request, instance,newid,new_hashid, employee, leave_period)
-
-											# KRIA ATTENDANCE
-											createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
-
-											messages.success(request, 'Leave Aumenta ho Susesu')
-											return redirect('leave-hr-leave-record', c_emp.hashed)
-									
-									
-									
+										messages.success(request, 'Leave Aumenta ho Susesu')
+										return redirect('leave-hr-leave-record', c_emp.hashed)
 								else:
-									messages.error(request,'Total loron nebe ita prienche latuir formato!!')
+									messages.error(request, 'Loron nebe hili barak liu. Halo favor altera loron nebe ita prienche')
+							# done: CHECK LEAVE COUNT NEBE IHA NO FULAN ONA IHA
 							else:
-								messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
-						else:
-							messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
+								lcount2 = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type)
+								lcount2.update(
+									month=getmonth,
+									year=getyear,
+									taken = days,
+									total_taken = days,
+									total_balance = round(float(leave_type.total) - float(days),2)
+								)
+								instance = form.save(commit=False)
+								createLeave(request, instance,newid,new_hashid, employee, leave_period)
+
+								# KRIA ATTENDANCE
+								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+
+								messages.success(request, 'Leave Aumenta ho Susesu')
+								return redirect('leave-hr-leave-record', c_emp.hashed)
+						
+					# done: ERROR KARIK DATA HAHU LAIHA PERIODE NIA LARAN
 					else:
-						messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
-				
-				
-				# done: ERROR KARIK DATA HAHU LAIHA PERIODE NIA LARAN
+						messages.error(request,'Data hahu laiha periode ida ne nia laran!!')
 				else:
-					messages.error(request,'Data hahu laiha periode ida ne nia laran. Halo Favor Kria Uluk lai Periode Foun!!')
-
+					messages.error(request,'Total loron nebe ita prienche latuir formato!!')
 			else:
-				messages.error(request,"Total Loron ne'ebe ita prienche iha Data Hahu no Remata Lahanesan ho Total Loron ne'ebe ita Input")
-
+				messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
+			
 	else:
 		form = HRLeaveForm()
 	context = {
 		'group': group, 'c_emp': c_emp,  'page': 'record',
 		'form': form, 'emp':emp,
 		'title': 'Aplika Licensa', 'legend': 'Aplika Licensa'
 	}
@@ -798,70 +556,75 @@
 		form = HRPeriodForm(request.POST)
 		if form.is_valid():
 			instance = form.save(commit=False)
 			start_year = form.cleaned_data.get('start_year')
 			end_year = form.cleaned_data.get('end_year')
 			if start_year.year == end_year.year:
 				messages.error(request, "Tinan Hahu ho Tinan Remata labele hanesan tinan remata !")
-			elif start_year.year >= end_year.year:
-				messages.error(request, "Tinan Hahu Labele boot liu Tinan Remata")
 			else:
 				for emp in employee:
-					lp = LeavePeriod.objects.filter(start_year=start_year, end_year=end_year, employee=emp).exists()
-					if  lp == False:
-						contract = Contract.objects.filter(employee=emp, is_active=True).last()
-						if contract:
-							allleavep = LeavePeriod.objects.filter(employee=emp)
-							for obj in allleavep:
-								obj.is_active = False
-								obj.save()
-							# instance.is_active = True
-							# instance.employee = emp
-							date_string = f'{start_year}-{contract.start_date.month}-{contract.start_date.day}'
-							start_period = dt.strptime(date_string, "%Y-%m-%d").date()
-							next_year = pd.date_range(start=start_period, end=start_period+pd.DateOffset(years=1), freq='M')
-							end_period = next_year.max()
-							LeavePeriod.objects.create(
-								employee=emp, \
-								start_month = get_object_or_404(Mnth, code=start_period.month),\
-								end_month = get_object_or_404(Mnth, code=end_period.month), \
-								start_year = get_object_or_404(Yr, year=start_period.year), \
-								end_year = get_object_or_404(Yr, year=end_period.year), \
-								start_date = start_period,\
-								end_date = end_period,\
-								is_active = True
-							)
-					else:
-						messages.error(request, f'Funsionario {emp} Seidauk iha Kontrato')
+					contract = Contract.objects.filter(employee=emp, is_active=True).last()
+					allleavep = LeavePeriod.objects.filter(employee=emp)
+					for obj in allleavep:
+						obj.is_active = False
+						obj.save()
+					# instance.is_active = True
+					# instance.employee = emp
+					date_string = f'{start_year}-{contract.start_date.month}-{contract.start_date.day}'
+					start_period = dt.strptime(date_string, "%Y-%m-%d").date()
+					next_year = pd.date_range(start=start_period, end=start_period+pd.DateOffset(years=1), freq='M')
+					end_period = next_year.max()
+					# instance.start_month = get_object_or_404(Mnth, code=start_period.month)
+					# instance.end_month = get_object_or_404(Mnth, code=end_period.month)
+					# instance.start_year = get_object_or_404(Yr, year=start_period.year)
+					# instance.end_year = get_object_or_404(Yr, year=end_period.year)
+					# instance.start_date = start_period
+					# instance.end_date = end_period
+					# instance.save()
+					LeavePeriod.objects.create(
+						employee=emp, \
+						start_month = get_object_or_404(Mnth, code=start_period.month),\
+						end_month = get_object_or_404(Mnth, code=end_period.month), \
+						start_year = get_object_or_404(Yr, year=start_period.year), \
+						end_year = get_object_or_404(Yr, year=end_period.year), \
+						start_date = start_period,\
+						end_date = end_period,\
+						is_active = True
+					)
 				messages.success(request, 'Susesu Aumenta Periode Licensa')
 				return redirect('leave-hr-app-raw-list')
+					
+
+
+
+					# if contract:
+					# else:
+					# 	messages.error(request, f'Funsrionario/a {emp} seidauk iha Kontrato')
+					# 	return redirect('leave-hr-app-raw-list')
 	else: form = HRPeriodForm()
 	context = {
 		'group': group,  'form':form,
 		'title': 'Set Period Leave', 'legend': 'Set Period Leave'
 	}
 	return render(request, 'leave/form2.html', context)
 
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrLeaveEmpPeriodAdd(request, hashid):
 	group = request.user.groups.all()[0].name
 	employee = get_object_or_404(Employee, hashed=hashid)
 	contract = Contract.objects.filter(employee=employee, is_active=True).last()
-	period = LeavePeriod.objects.filter(employee=employee)
 	if request.method == 'POST':
 		form = HRPeriodForm(request.POST)
 		if form.is_valid():
 			instance = form.save(commit=False)
 			start_year = form.cleaned_data.get('start_year')
 			end_year = form.cleaned_data.get('end_year')
-			if start_year.year == end_year.year:
+			if start_year == end_year:
 				messages.error(request, "Tinan Hahu ho Tinan Remata labele hanesan")
-			elif start_year.year >= end_year.year:
-				messages.error(request, "Tinan Hahu labele boot liu Tinan Remata")
 			else:
 				allleavep = LeavePeriod.objects.filter(employee=employee)
 				for obj in allleavep:
 					obj.is_active = False
 					obj.save()
 				instance.is_active = True
 				instance.employee = employee
@@ -877,15 +640,15 @@
 				instance.end_date = end_period
 				instance.save()
 				messages.success(request, 'Susesu Aumenta Periode Licensa')
 				return redirect('leave-hr-leave-record', hashid)
 	else: form = HRPeriodForm()
 	context = {
 		'group': group, 'form':form, 'page': 'add-emp-record', 'hashid': hashid,
-		'title': 'Kria Periode Licensa', 'legend': 'Kria Periode Licensa', 'period': period
+		'title': 'Set Period Leave', 'legend': 'Set Period Leave'
 	}
 	return render(request, 'leave/form2.html', context)
 
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrLeaveEmpUpdatePeriodMonth(request, hashid):
 	today = dt.today().date()
@@ -903,21 +666,34 @@
 			period = leave_period,
 			employee=employee,
 			leave_type=lt,
 			month = get_m,
 			year = get_y,
 			leave_earn = earn_per_month
 		)
+		# lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
+		# lc.total_earn = round(float(lc.leave_earn) + float(leave_count_last.total_balance),2)
+		# lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
+		# lc.balance_carry = lc.total_balance
+		# lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
+		# lc.prov_total_earn = lc.total_earn
+		# lc.save()
+		# lc.taken = round(float(lc.taken) + days,2)
+		# lc.total_taken = round(float(leave_count_last.taken) + days)
+		# lc.balance = round(float(leave_count_last.balance) + float(lc.leave_earn) - float(days),2 )
+		# lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),1)
+		# lc.save()
 		lcnew.balance = round(float(leave_count_last.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
 		lcnew.total_earn = round(float(leave_count_last.prov_total_earn) + float(lcnew.leave_earn),1)
 		lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
 		lcnew.balance_carry = lcnew.total_balance
 		lcnew.total_balance_leave = float(lt.total) - float(lcnew.total_balance)
 		lcnew.prov_total_earn = float(leave_count_last.prov_total_earn) + float(earn_per_month)
 		lcnew.save()
+	# previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type_id=1, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
 		messages.success(request, 'Susesu kria Record iha fulan ida ne')
 		return redirect('leave-hr-leave-record', hashid)
 	else:
 		messages.error(request, 'Deskulpa Laiha Licensa iha Fulan kotuk')
 		return redirect('leave-hr-leave-record', hashid)
 
 
@@ -965,20 +741,23 @@
 	return redirect('leave-hr-app-detail', hashid)
 @login_required
 @allowed_users(allowed_roles=['hr','hr_s'])
 def hrLeaveUpdateAtt(request, hashid, hashid2):
 	group = request.user.groups.all()[0].name
 	employee = get_object_or_404(Employee, hashed=hashid)
 	leave_period = LeavePeriod.objects.filter(employee=employee,is_active=True).last()
-	check_last_period = LeavePeriod.objects.filter(employee=employee,  pk__lt=leave_period.pk).last()
+	check_last_period = LeavePeriod.objects.filter(employee=employee, is_active=True, pk__lt=leave_period.pk).last()
 	last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
 	min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
 	max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
 	months = pd.period_range(min_month, max_month, freq='M')
 	leave = get_object_or_404(Leave, hashed=hashid2)
+	c_emp = employee
+	newid, new_hashid = getnewid(Leave)
+	newsid2, _ = getnewid(LeaveCount)
 
 
 	leave_type = leave.leave_type
 	days = leave.days
 	days = round(float(days),2)
 
 	if leave_type.pk == 1: earn_per_month = round(float(leave_type.total/12),2)
@@ -1001,70 +780,58 @@
 	if days <= leave_type.total:
 		# done: CHECK ANGKA LORON 0.5/1.0/1.5
 		if last_two_digits == int(5) or last_two_digits == int(0):
 			# done: CHECK DATA LEAVE IHA PERIODO NIA LARAN
 			if start_date_period <= start_month <= end_date_period + datetime.timedelta(days=29):
 				# done: CHECK LEAVE TYPE BA ANNUAL
 				if leave_type.pk == 1:
-					
 					# done: CHECK RECORD IHA FULAN IDA NE'E
-					
-					current_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
-					if current_leave_count:
-						previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
+					current_leave_count = get_object_or_404(LeaveCount, period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year)
+					previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
 					# done: CHECK KARIK LEAVE IHA FULAN KLARAN
 					if previous_leave_count:
 						current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
 						current_leave_count.total_taken = round(float(previous_leave_count.taken) + days)
 						current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(days),2 )
 						current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
 						current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
 						current_leave_count.save()
 
 
-
 						#done: KRIA ATTENDANCE
-						createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)							
+						createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)							
 					# done: CHECK KARIK LEAVE IHA FULAN PRIMEIRU
 					else:
 						current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
-						if check_last_period:
-							current_leave_count.total_earn = round(float(last_count_period.total_balance) + float(earn_per_month),1)
-							current_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) - float(current_leave_count.taken),2 )
-							current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-							current_leave_count.balance_month = round(float(current_leave_count.total_balance) - float(current_leave_count.taken),2)
-							current_leave_count.save()
-						else:
-							current_leave_count.total_taken = current_leave_count.taken
-							current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
-							current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-							current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
-							current_leave_count.save()
+						current_leave_count.total_taken = current_leave_count.taken
+						current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
+						current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+						current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
+						current_leave_count.save()
 
 						# done: KRIA ATTENDANCE
-						createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)
+						createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
 
 
 					i = 0
 					# done: UPDATE LEAVE RECORD
 					while i < len(months):
 						m = months[i]
 						if i == int(0):
 							# done: FULAN PRIMEIRO
 							if check_last_period:
 								first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
-								first_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) -  float(first_leave_count.taken),2)
+								first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
 								first_leave_count.total_earn = round(float(first_leave_count.leave_earn) + float(last_count_period.total_balance),2)
 								first_leave_count.total_balance = round(float(first_leave_count.total_earn) - float(first_leave_count.total_taken),2)
 								first_leave_count.balance_carry = first_leave_count.total_balance
 								first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
 								first_leave_count.prov_total_earn = first_leave_count.total_earn
 								first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
 								first_leave_count.save()
-
 							else:
 								first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
 								first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
 								first_leave_count.total_earn = round(float(first_leave_count.leave_earn),2)
 								first_leave_count.total_balance = round(float(first_leave_count.balance),2)
 								first_leave_count.balance_carry = first_leave_count.total_balance
 								first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
@@ -1107,15 +874,15 @@
 						# work: Leave Nebe Iha ona
 						if days <= previous_leave_count.total_balance:
 							if month_leave_count:
 								month_leave_count.taken = round(float(month_leave_count.taken) + days, 2)
 								month_leave_count.total_taken = round(float(previous_leave_count.total_taken) +  days,2)
 								month_leave_count.total_balance = round(float(leave_type.total) - float(month_leave_count.total_taken),2)
 								month_leave_count.save()
-								createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)
+								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
 								messages.success(request, 'Susesu Altera')
 								return redirect('leave-hr-app-detail', hashid2)
 							else:
 								lc = LeaveCount.objects.create(
 									period = leave_period,
 									employee = employee,
 									leave_type = leave_type,
@@ -1124,15 +891,15 @@
 
 								)
 								lc.taken = days
 								lc.total_taken = round(float(previous_leave_count.total_taken) + float(lc.taken),2)
 								lc.total_balance = round(float(leave_type.total) - float(lc.total_taken),2)
 								lc.save()
 
-								createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)
+								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
 
 								messages.success(request, 'Susesu Altera')
 								return redirect('leave-hr-app-detail', hashid2)
 						else:
 							messages.error(request, 'Loron nebe hili barak liu. Halo favor altera loron nebe ita prienche')
 					# done: CHECK LEAVE COUNT NEBE IHA NO FULAN ONA IHA
 					else:
@@ -1142,26 +909,30 @@
 							year=getyear,
 							taken = days,
 							total_taken = days,
 							total_balance = round(float(leave_type.total) - float(days),2)
 						)
 
 						# KRIA ATTENDANCE
-						createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)
+						createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
 
 						messages.success(request, 'Susesu Altera')
 						return redirect('leave-hr-app-detail', hashid2)
 				
 			# done: ERROR KARIK DATA HAHU LAIHA PERIODE NIA LARAN
 			else:
 				messages.error(request,'Data hahu laiha periode ida ne nia laran!!')
 		else:
 			messages.error(request,'Total loron nebe ita prienche latuir formato!!')
 	else:
 		messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
 	
+
+
+
 	leave.hr_confirm = True
+	leave.is_done = True
 	leave.save()
 
 
 	messages.success(request, 'Susesu Altera')
 	return redirect('leave-hr-app-detail', hashid2)
```

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_hr_m_back.py` & `django-ipghrms-leave-1.2/leave/views/leave_hr_m.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import datetime
 from django.shortcuts import render, redirect, get_object_or_404
 from django.contrib.auth.decorators import login_required
 from settings_app.decorators import allowed_users
 from django.contrib import messages
 from employee.models import CurEmpDivision, Employee
-from leave.models import Leave, LeaveHR, LeaveUnit, LeaveCount, LeavePeriod, Month as Mnth, Year as Yr, LeaveType
-from leave.forms import LeaveHRForm, LeaveUnitForm, LeaveForm, HRLeaveForm, HRPeriodForm, HRLeaveCommentForm
+from leave.models import Leave, LeaveHR, LeaveUnit, LeaveCount, LeavePeriod, Month as Mnth, Year as Yr, LeaveType, LeaveDep
+from leave.forms import LeaveHRForm, LeaveUnitForm, LeaveForm, HRLeaveForm, HRPeriodForm, HRLeaveCommentForm, HRLeaveFormSpecial
 from settings_app.utils import getnewid
 from settings_app.user_utils import c_staff, c_unit
 from dateutil.parser import parser
 from datetime import datetime as dt
 from datetime import timedelta
 from attendance.models import Attendance, AttendanceStatus,Year, Month
 import pytz
 import pandas as pd
 from django.db.models import Q, F
 from django.utils import timezone
 from calendar import mdays
+from contract.models import EmpPosition
 from attendance.models import Attendance, AttendanceStatus, Year as YAten, Month as Maten
-from leave.utils import createAttendance, createLeave
+from leave.utils import createAttendance,createAttendanceEmp, createLeave, count_day,calculate_hours, add_time, createAttendanceSpecial, createLeaveSpecial, createLeaveProcess
 from contract.models import Contract
 
+from leave.utils_2 import koko2, calculate_leave_days
 
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrLeaveCertUpdate(request, hashid):
 	leave = get_object_or_404(Leave, hashed=hashid)
 	empdiv = CurEmpDivision.objects.get(employee=leave.employee)
 	objects = LeaveHR.objects.get(leave=leave)
@@ -87,468 +89,928 @@
 		leave_type = None
 		if employee.sex == 'Male':
 			leave_type = LeaveType.objects.exclude(pk=4)
 		else:
 			leave_type = LeaveType.objects.all()
 		today = dt.today().date()
 		leave_period = LeavePeriod.objects.filter(is_active=True, employee=employee).last()
-		check_last_period = LeavePeriod.objects.filter(pk__lt=leave_period.pk, employee=employee).last()
-		last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
-		last_month_date = today.replace(day=1) - timedelta(days=1)
-		min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}-{leave_period.start_date.day}'
-		max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
-
-		months = pd.period_range(min_month, max_month, freq='M')
-		i = 0
-		while i < len(months):
-			leave_check = LeaveCount.objects.filter(employee=employee, period=leave_period).last()
-			m = months[i]
-			get_m = get_object_or_404(Mnth, code=m.month)
-			get_y = get_object_or_404(Yr, year=m.year)
-			if leave_check:
-				for lt1 in leave_type:
-					if lt1.pk == 1:
-						print('CALLLL 1')
-						lastleaveal = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type_id=1).last()
-						earn_per_month = round(float(lt1.total/12),2)
-						date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
-						date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
-						lcnew = LeaveCount.objects.create(
-							period = leave_period,
-							employee=employee,
-							leave_type=lt1,
-							month = get_m,
-							year = get_y,
-							update_date=date_period,
-							leave_earn = earn_per_month
-						)
-						lcnew.balance = round(float(lastleaveal.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
-						lcnew.total_earn = round(float(lastleaveal.prov_total_earn) + float(lcnew.leave_earn),1)
-						lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
-						lcnew.balance_carry = lcnew.total_balance
-						lcnew.total_balance_leave = float(lt1.total) - float(lcnew.total_balance)
-						lcnew.prov_total_earn = float(lastleaveal.prov_total_earn) + float(earn_per_month)
-						lcnew.balance_month = round(float(lastleaveal.total_balance) - float(lcnew.taken),2)
-						lcnew.save()
-			else:
-				for lt in leave_type:
-					if lt.pk == 1:
-						# work: Check Balansu iha Periode Kotuk
-						date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
-						date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
-						if check_last_period:
-							print('CALLLL HEREE LAST PERIOD')
-							earn_per_month = round(float(lt.total/12),2)
+		if leave_period:
+			check_last_period = LeavePeriod.objects.filter(pk__lt=leave_period.pk, employee=employee).last()
+			last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
+			last_month_date = today.replace(day=1) - timedelta(days=1)
+			min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}-{leave_period.start_date.day}'
+			max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
 
-							lc = LeaveCount.objects.create(
+			months = pd.period_range(min_month, max_month, freq='M')
+			i = 0
+			while i < len(months):
+				leave_check = LeaveCount.objects.filter(employee=employee, period=leave_period).last()
+				m = months[i]
+				get_m = get_object_or_404(Mnth, code=m.month)
+				get_y = get_object_or_404(Yr, year=m.year)
+				if leave_check:
+					for lt1 in leave_type:
+						if lt1.pk == 1:
+							lastleaveal = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type_id=1).last()
+							earn_per_month = round(float(lt1.total/12),2)
+							date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
+							date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
+							lcnew = LeaveCount.objects.create(
 								period = leave_period,
 								employee=employee,
-								leave_type=lt,
+								leave_type=lt1,
 								month = get_m,
 								year = get_y,
 								update_date=date_period,
 								leave_earn = earn_per_month
 							)
-							lc.balance = round(float(last_count_period.total_balance) +   float(lc.leave_earn) - float(lc.taken),2)
-							lc.total_earn = round(float(lc.leave_earn) + float(last_count_period.total_balance),2)
-							lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
-							lc.balance_carry = lc.total_balance
-							lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
-							lc.prov_total_earn = lc.total_earn
-							lc.balance_month = round(float(lc.total_balance) - float(lc.taken),2)
-							lc.save()
-						else:
-							print('CALLLL HEREE LAST PERIOD ELSEE')
-							earn_per_month = round(float(lt.total/12),2)
-							# balance_per_month = round(float(earn_per_month) - float(taken),2)
+							if leave_period.balance_carry > 0.00:
+								# lcnew.balance = round(float(leave_period.balance_carry) +   float(lcnew.leave_earn) - float(lcnew.taken),2)
+								lcnew.balance = round(float(lastleaveal.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
+								lcnew.total_earn = round( float(leave_period.balance_carry) + float(lastleaveal.prov_total_earn) + float(lcnew.leave_earn),1)
+								lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
+								lcnew.balance_carry = lcnew.total_balance
+								lcnew.total_balance_leave = float(lt1.total) - float(lcnew.total_balance)
+								lcnew.prov_total_earn = float(lastleaveal.prov_total_earn) + float(earn_per_month)
+								lcnew.balance_month = round(float(lastleaveal.total_balance) - float(lcnew.taken),2)
+								# lcnew.balance_month = round(float(lastleaveal.total_balance_leave) - float(lcnew.taken),2)
+								lcnew.save()
+							else:
+								# lcnew.balance = round(float(lc.leave_earn) - float(lc.taken),2)
+								lcnew.balance = round(float(lastleaveal.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
+								lcnew.total_earn = round(float(lastleaveal.prov_total_earn) + float(lcnew.leave_earn),1)
+								lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
+								lcnew.balance_carry = lcnew.total_balance
+								lcnew.total_balance_leave = float(lt1.total) - float(lcnew.total_balance)
+								lcnew.prov_total_earn = float(lastleaveal.prov_total_earn) + float(earn_per_month)
+								lcnew.balance_month = round(float(lastleaveal.total_balance) - float(lcnew.taken),2)
+								# lcnew.balance_month = round(float(lastleaveal.total_balance_leave) - float(lcnew.taken),2)
+								lcnew.save()
+				else:
+					for lt in leave_type:
+						if lt.pk == 1:
+							# work: Check Balance in Last Period
+							date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
+							date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
+							if check_last_period:
+								earn_per_month = round(float(lt.total/12),2)
+
+								lc = LeaveCount.objects.create(
+									period = leave_period,
+									employee=employee,
+									leave_type=lt,
+									month = get_m,
+									year = get_y,
+									update_date=date_period,
+									leave_earn = earn_per_month
+								)
+								if leave_period.balance_carry > 0.00:
+									lc.balance = round(float(leave_period.balance_carry) +   float(lc.leave_earn) - float(lc.taken),2)
+									lc.total_earn = round(float(lc.leave_earn) + float(leave_period.total_balance),2)
+								else:
+									lc.balance = round(float(last_count_period.total_balance) +   float(lc.leave_earn) - float(lc.taken),2)
+									lc.total_earn = round(float(lc.leave_earn) + float(last_count_period.total_balance),2)
+								# lc.balance = round(float(last_count_period.total_balance) +   float(lc.leave_earn) - float(lc.taken),2)
+								# lc.total_earn = round(float(lc.leave_earn) + float(last_count_period.total_balance),2)
+								lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
+								lc.balance_carry = lc.total_balance
+								lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
+								lc.prov_total_earn = lc.total_earn
+								lc.balance_month = round(float(lc.total_balance) - float(lc.taken),2)
+								lc.save()
+							else:
+								earn_per_month = round(float(lt.total/12),2)
 
-							lc = LeaveCount.objects.create(
+								lc = LeaveCount.objects.create(
+									period = leave_period,
+									employee=employee,
+									leave_type=lt,
+									month = get_m,
+									year = get_y,
+									update_date=date_period,
+									leave_earn = earn_per_month
+								)
+								if leave_period.balance_carry > 0.00:
+									lc.balance = round(float(leave_period.balance_carry) +   float(lc.leave_earn) - float(lc.taken),2)
+									lc.total_earn = round(float(leave_period.balance_carry) + float(lc.leave_earn),2)
+								else:
+									lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
+									lc.total_earn = round(float(lc.leave_earn),2)
+								# lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
+								# lc.total_earn = round(float(lc.leave_earn),2)
+								lc.total_balance = round(float(lc.balance),2)
+								lc.balance_carry = lc.total_balance
+								lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
+								lc.prov_total_earn = lc.leave_earn
+								lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
+								lc.save()
+						else:
+							lcall = LeaveCount.objects.create(
 								period = leave_period,
 								employee=employee,
 								leave_type=lt,
-								month = get_m,
 								year = get_y,
-								update_date=date_period,
-								leave_earn = earn_per_month
 							)
-							lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
-							lc.total_earn = round(float(lc.leave_earn),2)
-							lc.total_balance = round(float(lc.balance),2)
-							lc.balance_carry = lc.total_balance
-							lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
-							lc.prov_total_earn = lc.leave_earn
-							lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
-							lc.save()
-					else:
-						lcall = LeaveCount.objects.create(
-							period = leave_period,
-							employee=employee,
-							leave_type=lt,
-							year = get_y,
-						)
-						lcall.total_balance = float(lt.total)
-						lcall.save()
-			
-			i+=1
+							lcall.total_balance = float(lt.total)
+							lcall.save()
+				
+				i+=1
 		messages.success(request, f'Susesu Update Record')
 		return redirect('leave-hr-leave-record', hashid=hashid)
 	else:
 		messages.error(request, f'Kontrato ba pessoal refere seidauk iha!!')
 		return redirect('leave-hr-leave-record', hashid=hashid)
 
-
 @login_required
-@allowed_users(allowed_roles=['admin','hr'])
-def hrLeaveUpdateRecord(request):
-	employee = Employee.objects.filter(status_id=1)
-	for emp in employee:
-		# work: Get Last Employee Leave Count
-		leave_type = None
-		if emp.sex == 'Male':
-			leave_type = LeaveType.objects.exclude(pk=4)
-		else:
-			leave_type = LeaveType.objects.all()
-		leave_type_al = LeaveType.objects.get(pk=1)
-		leave_period = LeavePeriod.objects.filter(is_active=True, employee=emp).last()
-		# work: Depois koko tan ida tan
-		check_last_period = LeavePeriod.objects.filter(pk__lt=leave_period.pk, employee=emp).last()
-		last_count_period = LeaveCount.objects.filter(employee=emp, period=check_last_period, leave_type_id=1).last()
-		min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
-		max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
-		months = pd.period_range(min_month, max_month, freq='M')
-		i = 0
-		while i < len(months):
-			leave_check = LeaveCount.objects.filter(employee=emp, period=leave_period).last()
-			m = months[i]
-			get_m = get_object_or_404(Mnth, code=m.month)
-			get_y = get_object_or_404(Yr, year=m.year)
-			if leave_check:
-				for lt1 in leave_type:
-					if lt1.pk == 1:
-						lastleaveal = LeaveCount.objects.filter(employee=emp, period=leave_period, leave_type_id=1).last()
-						earn_per_month = round(float(lt1.total/12),2)
-						date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
-						date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
-						lcnew = LeaveCount.objects.create(
-							period = leave_period,
-							employee=emp,
-							leave_type=lt1,
-							month = get_m,
-							year = get_y,
-							update_date = date_period,
-							leave_earn = earn_per_month
-						)
-						lcnew.balance = round(float(lastleaveal.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
-						lcnew.total_earn = round(float(lastleaveal.prov_total_earn) + float(lcnew.leave_earn),1)
-						lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
-						lcnew.balance_carry = lcnew.total_balance
-						lcnew.total_balance_leave = float(lt1.total) - float(lcnew.total_balance)
-						lcnew.prov_total_earn = float(lastleaveal.prov_total_earn) + float(earn_per_month)
-						lcnew.balance_month = round(float(lastleaveal.balance) - float(lcnew.taken),2)
-						lcnew.save()
-			else:
-				for lt in leave_type:
-					if lt.pk == 1:
-						# work: Check Balansu iha Periode Kotuk
-						date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
-						date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
-						if check_last_period:
-							earn_per_month = round(float(lt.total/12),2)
+def hrLeaveAdd(request, hashid):
+	group = request.user.groups.all()[0].name
+	employee = get_object_or_404(Employee, hashed=hashid)
+	leave_period = LeavePeriod.objects.filter(employee=employee,is_active=True).last()
+	check_last_period = LeavePeriod.objects.filter(employee=employee,  pk__lt=leave_period.pk).last()
+	last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
+	min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
+	max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
+	months = pd.period_range(min_month, max_month, freq='M')
+	today = dt.today().date()
+	c_emp = employee
+	emp = employee
+	if request.method == 'POST':
+		newid, new_hashid = getnewid(Leave)
+		form = HRLeaveForm(request.POST, request.FILES)
+		if form.is_valid():
+			leave_type = form.cleaned_data.get('leave_type')
+			days = form.cleaned_data.get('days')
+			days = round(float(days),2)
+			if leave_type.pk == 1:
+				earn_per_month = round(float(leave_type.total/12),2)
+			else: earn_per_month = 0.00
+			start_date = form.cleaned_data.get('start_date')
+			end_date = form.cleaned_data.get('end_date')
+			last_two_digits = str(days).split('.')[1][:2]
+			last_two_digits = int(last_two_digits)
 
-							lc = LeaveCount.objects.create(
-								period = leave_period,
-								employee=emp,
-								leave_type=lt,
-								month = get_m,
-								year = get_y,
-								update_date=date_period,
-								leave_earn = earn_per_month
-							)
-							lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
-							lc.total_earn = round(float(lc.leave_earn) + float(last_count_period.total_balance),2)
-							lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
-							lc.balance_carry = lc.total_balance
-							lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
-							lc.prov_total_earn = lc.total_earn
-							lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
-							lc.save()
-						else:
-							earn_per_month = round(float(lt.total/12),2)
-							# balance_per_month = round(float(earn_per_month) - float(taken),2)
+			min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
+			max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
+			date1 = pd.to_datetime(start_date, format="%Y %m").date()
+			date2 = pd.to_datetime(end_date, format="%Y %m").date()
 
-							lc = LeaveCount.objects.create(
-								period = leave_period,
-								employee=emp,
-								leave_type=lt,
-								month = get_m,
-								year = get_y,
-								update_date=date_period,
-								leave_earn = earn_per_month
-							)
-							lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
-							lc.total_earn = round(float(lc.leave_earn),2)
-							lc.total_balance = round(float(lc.balance),2)
-							lc.balance_carry = lc.total_balance
-							lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
-							lc.prov_total_earn = lc.leave_earn
-							lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
-							lc.save()
+			start_date_period = pd.to_datetime(min_month, format="%Y %m").date()
+			end_date_period = pd.to_datetime(max_month, format="%Y %m").date()
+			start_month = date1
+			cal_day = count_day(start_date, end_date)
+			
+			if float(cal_day) >= days:
+
+				# done: CHECK DATA LEAVE IHA PERIODO NIA LARAN
+				if start_date_period <= start_month <= end_date_period + datetime.timedelta(days=29):
+					current_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
+					if current_leave_count:
+						previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
+					leave_this_month = LeaveCount.objects.filter(period=leave_period, employee=employee, leave_type_id=1, update_date__lte=today).last()
+							
+					if leave_this_month.balance >= 0.5:
+						if   days <= leave_this_month.balance or days <= leave_this_month.balance + 5 :
+							if days < 30  or days >= 30:
+								# check_day(days, current_leave_count, previous_leave_count)
+								# done: CHECK ANGKA LORON 0.5/1.0/1.5
+								if last_two_digits == int(5) or last_two_digits == int(0):
+									
+									
+									
+									# done: CHECK LEAVE TYPE BA ANNUAL
+									if leave_type.pk == 1:
+										# done: CHECK RECORD IHA FULAN IDA NE'E
+										# current_leave_count = get_object_or_404(LeaveCount, period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year)
+										# previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
+										# done: CHECK KARIK LEAVE IHA FULAN KLARAN
+										if previous_leave_count:
+											current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
+											current_leave_count.total_taken = round(float(previous_leave_count.taken) + days)
+											current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(days),2 )
+											current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+											current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
+											current_leave_count.save()
+
+
+											#done: KRIA ATTENDANCE
+											createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)							
+										# done: CHECK KARIK LEAVE IHA FULAN PRIMEIRU
+										else:
+											current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
+											if check_last_period:
+												current_leave_count.total_taken = current_leave_count.taken
+												current_leave_count.total_earn = round(float(last_count_period.total_balance) + float(earn_per_month),1)
+												current_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) - float(current_leave_count.taken),2 )
+												current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+												current_leave_count.balance_month = round(float(current_leave_count.total_balance) - float(current_leave_count.taken),2)
+												current_leave_count.save()
+											else:
+												current_leave_count.total_taken = current_leave_count.taken
+												current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
+												current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+												current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
+												current_leave_count.save()
+
+											# done: KRIA ATTENDANCE
+											createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+
+
+										i = 0
+										# done: UPDATE LEAVE RECORD
+										while i < len(months):
+											m = months[i]
+											if i == int(0):
+												# work: First Month
+												if check_last_period:
+													first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+													first_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) -  float(first_leave_count.taken),2)
+													first_leave_count.total_earn = round(float(first_leave_count.leave_earn) + float(last_count_period.total_balance),2)
+													first_leave_count.total_balance = round(float(first_leave_count.total_earn) - float(first_leave_count.total_taken),2)
+													first_leave_count.balance_carry = first_leave_count.total_balance
+													first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
+													first_leave_count.prov_total_earn = first_leave_count.total_earn
+													first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+													first_leave_count.save()
+												else:
+													if leave_period.balance_carry > 0.00:
+														first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+														first_leave_count.balance = round(float(leave_period.balance_carry) + float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
+														first_leave_count.total_earn = round(float(leave_period.balance_carry) + float(first_leave_count.leave_earn),2)
+														first_leave_count.total_balance = round( float(first_leave_count.balance),2)
+														first_leave_count.balance_carry = first_leave_count.total_balance
+														first_leave_count.total_balance_leave = float(leave_period.balance_carry) + float(leave_type.total) - float(first_leave_count.total_balance)
+														first_leave_count.prov_total_earn =  float(leave_period.balance_carry) + float(first_leave_count.leave_earn)
+														first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+														first_leave_count.save()
+													else:
+														first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+														first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
+														first_leave_count.total_earn = round(float(first_leave_count.leave_earn),2)
+														first_leave_count.total_balance = round(float(first_leave_count.balance),2)
+														first_leave_count.balance_carry = first_leave_count.total_balance
+														first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
+														first_leave_count.prov_total_earn = first_leave_count.leave_earn
+														first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+														first_leave_count.save()
+
+											else:
+												prev_mont = m.asfreq("M", "S") - 1
+												lccurrent = get_object_or_404(LeaveCount, employee=employee, period=leave_period, leave_type=leave_type,  year__year=m.year, month__code=m.month)
+												lclast = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type,  year__year=prev_mont.year, month__code=prev_mont.month).first()
+
+												if leave_period.balance_carry > 0.00:
+													lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
+													lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
+													lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
+													lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
+													lccurrent.balance_carry = lccurrent.total_balance
+													lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
+													lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
+													lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
+													lccurrent.save()
+												else:
+													lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
+													lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
+													lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
+													lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
+													lccurrent.balance_carry = lccurrent.total_balance
+													lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
+													lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
+													lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
+													lccurrent.save()
+
+											i+=1
+
+										# done: KRIA LEAVE
+										instance = form.save(commit=False)
+										createLeave(request, instance,newid,new_hashid, employee, leave_period)
+										messages.success(request, 'Leave Aumenta ho Susesu')
+										return redirect('leave-hr-leave-record', c_emp.hashed)
+
+
+
+									# done: CHECK KARIK LEAVE LAOS ANNUAL LEAVE
+									else:
+
+										lcount = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type, month__isnull=False)
+										getmonth = get_object_or_404(Mnth, code=start_date.month)
+										getyear = get_object_or_404(Yr, year=start_date.year)
+
+										# done: CHECK LEAVE COUNT NEBE IHA ONA MAIBE FULAN LAIHA
+										if lcount:
+											previous_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type=leave_type).last()
+											month_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
+											# work: Leave Nebe Iha ona
+											if days <= previous_leave_count.total_balance:
+												if month_leave_count:
+													month_leave_count.taken = round(float(month_leave_count.taken) + days, 2)
+													month_leave_count.total_taken = round(float(previous_leave_count.total_taken) +  days,2)
+													# month_leave_count.total_taken = month_leave_count.taken
+													month_leave_count.total_balance = round(float(leave_type.total) - float(month_leave_count.total_taken),2)
+													month_leave_count.save()
+													instance = form.save(commit=False)
+													createLeave(request, instance,newid,new_hashid, employee, leave_period)
+													createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+													messages.success(request, 'Leave Aumenta ho Susesu')
+													return redirect('leave-hr-leave-record', c_emp.hashed)
+												else:
+													lc = LeaveCount.objects.create(
+														period = leave_period,
+														employee = employee,
+														leave_type = leave_type,
+														year = getyear,
+														month = getmonth
+
+													)
+													lc.taken = days
+													lc.total_taken = round(float(previous_leave_count.total_taken) + float(lc.taken),2)
+													lc.total_balance = round(float(leave_type.total) - float(lc.total_taken),2)
+													lc.save()
+													instance = form.save(commit=False)
+
+													createLeave(request, instance,newid,new_hashid, employee, leave_period)
+													createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+
+													messages.success(request, 'Leave Aumenta ho Susesu')
+													return redirect('leave-hr-leave-record', c_emp.hashed)
+											else:
+												messages.error(request, 'Loron nebe hili barak liu. Halo favor altera loron nebe ita prienche')
+										# done: CHECK LEAVE COUNT NEBE IHA NO FULAN ONA IHA
+										else:
+											lcount2 = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type)
+											lcount2.update(
+												month=getmonth,
+												year=getyear,
+												taken = days,
+												total_taken = days,
+												total_balance = round(float(leave_type.total) - float(days),2)
+											)
+											instance = form.save(commit=False)
+											createLeave(request, instance,newid,new_hashid, employee, leave_period)
+
+											# KRIA ATTENDANCE
+											createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+
+											messages.success(request, 'Leave Aumenta ho Susesu')
+											return redirect('leave-hr-leave-record', c_emp.hashed)
+									
+									
+									
+								else:
+									messages.error(request,'Total loron nebe ita prienche latuir formato!!')
+							else:
+								messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
+						else:
+							messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
 					else:
-						lcall = LeaveCount.objects.create(
-							period = leave_period,
-							employee=emp,
-							leave_type=lt,
-							year = get_y,
-						)
-						lcall.total_balance = float(lt.total)
-						lcall.save()
-			i+=1
-	messages.success(request, f'Susesu Update Record')
-	return redirect('leave-hr-app-raw-list')
-	
+						messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
+				
+				
+				# done: ERROR KARIK DATA HAHU LAIHA PERIODE NIA LARAN
+				else:
+					messages.error(request,'Data hahu laiha periode ida ne nia laran. Halo Favor Kria Uluk lai Periode Foun!!')
 
-def update_leave_count(alldata, month):
+			else:
+				messages.error(request,"Total Loron ne'ebe ita prienche iha Data Hahu no Remata Lahanesan ho Total Loron ne'ebe ita Input")
 
-	for obj in alldata:
-		print(obj)
+	else:
+		form = HRLeaveForm()
+	context = {
+		'group': group, 'c_emp': c_emp,  'page': 'record',
+		'form': form, 'emp':emp,
+		'title': 'Aplika Licensa', 'legend': 'Aplika Licensa'
+	}
+	return render(request, 'leave/form.html', context)
 
 
 @login_required
-def hrLeaveAdd(request, hashid):
+def hrLeaveAddSpecial(request, hashid):
 	group = request.user.groups.all()[0].name
 	employee = get_object_or_404(Employee, hashed=hashid)
 	leave_period = LeavePeriod.objects.filter(employee=employee,is_active=True).last()
-	check_last_period = LeavePeriod.objects.filter(employee=employee, is_active=True, pk__lt=leave_period.pk).last()
+	check_last_period = LeavePeriod.objects.filter(employee=employee,  pk__lt=leave_period.pk).last()
 	last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
 	min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
 	max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
 	months = pd.period_range(min_month, max_month, freq='M')
+	today = dt.today().date()
 	c_emp = employee
 	emp = employee
 	if request.method == 'POST':
 		newid, new_hashid = getnewid(Leave)
-		newsid2, _ = getnewid(LeaveCount)
-		form = HRLeaveForm(request.POST, request.FILES)
+		form = HRLeaveFormSpecial(request.POST, request.FILES)
 		if form.is_valid():
 			leave_type = form.cleaned_data.get('leave_type')
-			days = form.cleaned_data.get('days')
-			days = round(float(days),2)
+			start_time = form.cleaned_data.get('start_time')
+			start_time_str = start_time.strftime("%H:%M")
+			end_time = form.cleaned_data.get('end_time')
+			end_time_str = end_time.strftime("%H:%M")
+			tot_hours = calculate_hours(start_time_str, end_time_str)
+
+			days = tot_hours
+			# days = round(float(days),2)
 			if leave_type.pk == 1:
 				earn_per_month = round(float(leave_type.total/12),2)
 			else: earn_per_month = 0.00
 			start_date = form.cleaned_data.get('start_date')
 			end_date = form.cleaned_data.get('end_date')
-			last_two_digits = str(days).split('.')[1][:2]
-			last_two_digits = int(last_two_digits)
 
 			min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
 			max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
 			date1 = pd.to_datetime(start_date, format="%Y %m").date()
 			date2 = pd.to_datetime(end_date, format="%Y %m").date()
 
 			start_date_period = pd.to_datetime(min_month, format="%Y %m").date()
 			end_date_period = pd.to_datetime(max_month, format="%Y %m").date()
 			start_month = date1
+			date_range = pd.date_range(start=start_date, end=end_date, freq="B")
+			total_length = len(date_range)
+			total_day = round(days * total_length,2)
 
 
-			if days <= leave_type.total:
-				# done: CHECK ANGKA LORON 0.5/1.0/1.5
-				if last_two_digits == int(5) or last_two_digits == int(0):
-					# done: CHECK DATA LEAVE IHA PERIODO NIA LARAN
-					if start_date_period <= start_month <= end_date_period + datetime.timedelta(days=29):
-						# done: CHECK LEAVE TYPE BA ANNUAL
-						if leave_type.pk == 1:
-							print('ADDD  CALL 1')
-							# done: CHECK RECORD IHA FULAN IDA NE'E
-							current_leave_count = get_object_or_404(LeaveCount, period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year)
-							previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
-							# done: CHECK KARIK LEAVE IHA FULAN KLARAN
-							if previous_leave_count:
-								# print('ADDD  CALL 2')
-								# if check_last_period:
-								# 	print('ADDD  CALL 3')
-								# 	current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
-								# 	current_leave_count.total_taken = round(float(previous_leave_count.taken) + days)
-								# 	current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(days),2 )
-								# 	current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-								# 	current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
-								# 	current_leave_count.save()
-								# else:
-								current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
-								current_leave_count.total_taken = round(float(previous_leave_count.taken) + days)
-								current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(days),2 )
-								current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-								current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
-								current_leave_count.save()
-
-
-								#done: KRIA ATTENDANCE
-								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)							
-							# done: CHECK KARIK LEAVE IHA FULAN PRIMEIRU
-							else:
-								print('ANOTHER CALL 1')
-								current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
-								if check_last_period:
-									print('ANOTHER CALL 2')
-									current_leave_count.total_earn = round(float(last_count_period.total_balance) + float(earn_per_month),1)
-									current_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) - float(current_leave_count.taken),2 )
-									current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-									current_leave_count.balance_month = round(float(current_leave_count.total_balance) - float(current_leave_count.taken),2)
-									current_leave_count.save()
-								else:
-									print('ANOTHER CALL 3')
-									current_leave_count.total_taken = current_leave_count.taken
-									current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
+			# done: CHECK DATA LEAVE IHA PERIODO NIA LARAN
+			if start_date_period <= start_month <= end_date_period + datetime.timedelta(days=29):
+				current_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
+				if current_leave_count:
+					previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
+				leave_this_month = LeaveCount.objects.filter(period=leave_period, employee=employee, leave_type_id=1, update_date__lte=today).last()
+
+				if leave_this_month.balance >= 0.5:
+					if   total_day <= leave_this_month.balance or total_day <= leave_this_month.balance + 5 :
+						if total_day < 30  or total_day >= 30:
+							# check_day(days, current_leave_count, previous_leave_count)
+							# done: CHECK ANGKA LORON 0.5/1.0/1.5
+								
+								
+							# done: CHECK LEAVE TYPE BA ANNUAL
+							if leave_type.pk == 1:
+								# done: CHECK RECORD IHA FULAN IDA NE'E
+								current_leave_count = get_object_or_404(LeaveCount, period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year)
+								previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
+								# done: CHECK KARIK LEAVE IHA FULAN KLARAN
+								if previous_leave_count:
+									current_leave_count.taken = round(float(current_leave_count.taken) + total_day,2)
+									current_leave_count.total_taken = round(float(previous_leave_count.taken) + total_day)
+									current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(total_day),2 )
 									current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-									current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
+									current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
 									current_leave_count.save()
 
-								# done: KRIA ATTENDANCE
-								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
 
-
-							i = 0
-							# done: UPDATE LEAVE RECORD
-							while i < len(months):
-								m = months[i]
-								if i == int(0):
-									# work: First Month
+									#done: KRIA ATTENDANCE
+									createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten,start_time_str, end_time_str)							
+								# done: CHECK KARIK LEAVE IHA FULAN PRIMEIRU
+								else:
+									current_leave_count.taken = round(float(current_leave_count.taken) + total_day,2)
 									if check_last_period:
-										print('PRINT CALL UPDATE CHEK LAST PERIOD')
-										first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
-										first_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) -  float(first_leave_count.taken),2)
-										first_leave_count.total_earn = round(float(first_leave_count.leave_earn) + float(last_count_period.total_balance),2)
-										first_leave_count.total_balance = round(float(first_leave_count.total_earn) - float(first_leave_count.total_taken),2)
-										first_leave_count.balance_carry = first_leave_count.total_balance
-										first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
-										first_leave_count.prov_total_earn = first_leave_count.total_earn
-										first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
-										first_leave_count.save()
-										print('PRINT CALL UPDATE CHEK LAST PERIOD ---- NOT')
+										current_leave_count.total_taken = current_leave_count.taken
+										current_leave_count.total_earn = round(float(last_count_period.total_balance) + float(earn_per_month),1)
+										current_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) - float(current_leave_count.taken),2 )
+										current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+										current_leave_count.balance_month = round(float(current_leave_count.total_balance) - float(current_leave_count.taken),2)
+										current_leave_count.save()
 									else:
-										first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
-										first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
-										first_leave_count.total_earn = round(float(first_leave_count.leave_earn),2)
-										first_leave_count.total_balance = round(float(first_leave_count.balance),2)
-										first_leave_count.balance_carry = first_leave_count.total_balance
-										first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
-										first_leave_count.prov_total_earn = first_leave_count.leave_earn
-										first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
-										first_leave_count.save()
+										current_leave_count.total_taken = current_leave_count.taken
+										current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
+										current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+										current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
+										current_leave_count.save()
+
+									# done: KRIA ATTENDANCE
+									createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, start_time_str, end_time_str)
+
+
+								i = 0
+								# done: UPDATE LEAVE RECORD
+								while i < len(months):
+									m = months[i]
+									if i == int(0):
+										# work: First Month
+										if check_last_period:
+											first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+											first_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) -  float(first_leave_count.taken),2)
+											first_leave_count.total_earn = round(float(first_leave_count.leave_earn) + float(last_count_period.total_balance),2)
+											first_leave_count.total_balance = round(float(first_leave_count.total_earn) - float(first_leave_count.total_taken),2)
+											first_leave_count.balance_carry = first_leave_count.total_balance
+											first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
+											first_leave_count.prov_total_earn = first_leave_count.total_earn
+											first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+											first_leave_count.save()
+										else:
+											if leave_period.balance_carry > 0.00:
+												first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+												first_leave_count.balance = round(float(leave_period.balance_carry) + float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
+												first_leave_count.total_earn = round(float(leave_period.balance_carry) + float(first_leave_count.leave_earn),2)
+												first_leave_count.total_balance = round( float(first_leave_count.balance),2)
+												first_leave_count.balance_carry = first_leave_count.total_balance
+												first_leave_count.total_balance_leave = float(leave_period.balance_carry) + float(leave_type.total) - float(first_leave_count.total_balance)
+												first_leave_count.prov_total_earn =  float(leave_period.balance_carry) + float(first_leave_count.leave_earn)
+												first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+												first_leave_count.save()
+											else:
+												first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+												first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
+												first_leave_count.total_earn = round(float(first_leave_count.leave_earn),2)
+												first_leave_count.total_balance = round(float(first_leave_count.balance),2)
+												first_leave_count.balance_carry = first_leave_count.total_balance
+												first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
+												first_leave_count.prov_total_earn = first_leave_count.leave_earn
+												first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+												first_leave_count.save()
 
-								else:
-									# work: Next Month
-									prev_mont = m.asfreq("M", "S") - 1
-									lccurrent = get_object_or_404(LeaveCount, employee=employee, period=leave_period, leave_type=leave_type,  year__year=m.year, month__code=m.month)
-									lclast = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type,  year__year=prev_mont.year, month__code=prev_mont.month).first()
-
-
-									lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
-									lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
-									lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
-									lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
-									lccurrent.balance_carry = lccurrent.total_balance
-									lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
-									lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
-									lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
-									lccurrent.save()
-
-								i+=1
-
-							# done: KRIA LEAVE
-							instance = form.save(commit=False)
-							createLeave(request, instance,newid,new_hashid, employee, leave_period)
-							messages.success(request, 'Leave Aumenta ho Susesu')
-							return redirect('leave-hr-leave-record', c_emp.hashed)
+									else:
+										prev_mont = m.asfreq("M", "S") - 1
+										lccurrent = get_object_or_404(LeaveCount, employee=employee, period=leave_period, leave_type=leave_type,  year__year=m.year, month__code=m.month)
+										lclast = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type,  year__year=prev_mont.year, month__code=prev_mont.month).first()
+
+										if leave_period.balance_carry > 0.00:
+											lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
+											lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
+											lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
+											lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
+											lccurrent.balance_carry = lccurrent.total_balance
+											lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
+											lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
+											lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
+											lccurrent.save()
+										else:
+											lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
+											lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
+											lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
+											lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
+											lccurrent.balance_carry = lccurrent.total_balance
+											lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
+											lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
+											lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
+											lccurrent.save()
 
-						# done: CHECK KARIK LEAVE LAOS ANNUAL LEAVE
-						else:
+									i+=1
 
-							lcount = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type, month__isnull=False)
-							getmonth = get_object_or_404(Mnth, code=start_date.month)
-							getyear = get_object_or_404(Yr, year=start_date.year)
-
-							# done: CHECK LEAVE COUNT NEBE IHA ONA MAIBE FULAN LAIHA
-							if lcount:
-								previous_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type=leave_type).last()
-								month_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
-								# work: Leave Nebe Iha ona
-								if days <= previous_leave_count.total_balance:
-									if month_leave_count:
-										month_leave_count.taken = round(float(month_leave_count.taken) + days, 2)
-										month_leave_count.total_taken = round(float(previous_leave_count.total_taken) +  days,2)
-										print(month_leave_count.taken)
-										# month_leave_count.total_taken = month_leave_count.taken
-										print(month_leave_count.total_taken)
-										month_leave_count.total_balance = round(float(leave_type.total) - float(month_leave_count.total_taken),2)
-										print(month_leave_count.total_balance)
-										month_leave_count.save()
-										instance = form.save(commit=False)
-										createLeave(request, instance,newid,new_hashid, employee, leave_period)
-										createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
-										messages.success(request, 'Leave Aumenta ho Susesu')
-										return redirect('leave-hr-leave-record', c_emp.hashed)
-									else:
-										lc = LeaveCount.objects.create(
-											period = leave_period,
-											employee = employee,
-											leave_type = leave_type,
-											year = getyear,
-											month = getmonth
-
-										)
-										lc.taken = days
-										lc.total_taken = round(float(previous_leave_count.total_taken) + float(lc.taken),2)
-										lc.total_balance = round(float(leave_type.total) - float(lc.total_taken),2)
-										lc.save()
-										instance = form.save(commit=False)
+								# done: KRIA LEAVE
+								instance = form.save(commit=False)
+								createLeaveSpecial(request, instance,newid,new_hashid, employee, leave_period, total_day)
+								messages.success(request, 'Leave Aumenta ho Susesu')
+								return redirect('leave-hr-leave-record', c_emp.hashed)
 
-										createLeave(request, instance,newid,new_hashid, employee, leave_period)
-										createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
 
-										messages.success(request, 'Leave Aumenta ho Susesu')
-										return redirect('leave-hr-leave-record', c_emp.hashed)
-								else:
-									messages.error(request, 'Loron nebe hili barak liu. Halo favor altera loron nebe ita prienche')
-							# done: CHECK LEAVE COUNT NEBE IHA NO FULAN ONA IHA
+
+							# done: CHECK KARIK LEAVE LAOS ANNUAL LEAVE
 							else:
-								lcount2 = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type)
-								lcount2.update(
-									month=getmonth,
-									year=getyear,
-									taken = days,
-									total_taken = days,
-									total_balance = round(float(leave_type.total) - float(days),2)
-								)
-								instance = form.save(commit=False)
-								createLeave(request, instance,newid,new_hashid, employee, leave_period)
 
-								# KRIA ATTENDANCE
-								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+								lcount = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type, month__isnull=False)
+								getmonth = get_object_or_404(Mnth, code=start_date.month)
+								getyear = get_object_or_404(Yr, year=start_date.year)
+
+								# done: CHECK LEAVE COUNT NEBE IHA ONA MAIBE FULAN LAIHA
+								if lcount:
+									previous_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type=leave_type).last()
+									month_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
+									# work: Leave Nebe Iha ona
+									if days <= previous_leave_count.total_balance:
+										if month_leave_count:
+											month_leave_count.taken = round(float(month_leave_count.taken) + total_day, 2)
+											month_leave_count.total_taken = round(float(previous_leave_count.total_taken) +  total_day,2)
+											month_leave_count.total_taken = month_leave_count.taken
+											month_leave_count.total_balance = round(float(leave_type.total) - float(month_leave_count.total_taken),2)
+											month_leave_count.save()
+											instance = form.save(commit=False)
+											createLeaveSpecial(request, instance,newid,new_hashid, employee, leave_period, total_day)
+											createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, start_time_str, end_time_str)
+											messages.success(request, 'Leave Aumenta ho Susesu')
+											return redirect('leave-hr-leave-record', c_emp.hashed)
+										else:
+											lc = LeaveCount.objects.create(
+												period = leave_period,
+												employee = employee,
+												leave_type = leave_type,
+												year = getyear,
+												month = getmonth
+
+											)
+											lc.taken = total_day
+											lc.total_taken = round(float(previous_leave_count.total_taken) + float(lc.taken),2)
+											lc.total_balance = round(float(leave_type.total) - float(lc.total_taken),2)
+											lc.save()
+											instance = form.save(commit=False)
 
-								messages.success(request, 'Leave Aumenta ho Susesu')
-								return redirect('leave-hr-leave-record', c_emp.hashed)
-						
-					# done: ERROR KARIK DATA HAHU LAIHA PERIODE NIA LARAN
+											createLeaveSpecial(request, instance,newid,new_hashid, employee, leave_period, total_day)
+											createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, start_time_str, end_time_str)
+
+											messages.success(request, 'Leave Aumenta ho Susesu')
+											return redirect('leave-hr-leave-record', c_emp.hashed)
+									else:
+										messages.error(request, 'Loron nebe hili barak liu. Halo favor altera loron nebe ita prienche')
+								# done: CHECK LEAVE COUNT NEBE IHA NO FULAN ONA IHA
+								else:
+									lcount2 = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type)
+									lcount2.update(
+										month=getmonth,
+										year=getyear,
+										taken = total_day,
+										total_taken = total_day,
+										total_balance = round(float(leave_type.total) - float(total_day),2)
+									)
+									instance = form.save(commit=False)
+									createLeaveSpecial(request, instance,newid,new_hashid, employee, leave_period, total_day)
+
+									# KRIA ATTENDANCE
+									createAttendanceSpecial(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, start_time_str, end_time_str)
+
+									messages.success(request, 'Leave Aumenta ho Susesu')
+									return redirect('leave-hr-leave-record', c_emp.hashed)
+								
+								
+						else:
+							messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
 					else:
-						messages.error(request,'Data hahu laiha periode ida ne nia laran!!')
+						messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
 				else:
-					messages.error(request,'Total loron nebe ita prienche latuir formato!!')
+					messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
+			# done: ERROR KARIK DATA HAHU LAIHA PERIODE NIA LARAN
 			else:
-				messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
+				messages.error(request,'Data hahu laiha periode ida ne nia laran. Halo Favor Kria Uluk lai Periode Foun!!')
+
 			
 	else:
-		form = HRLeaveForm()
+		form = HRLeaveFormSpecial()
 	context = {
 		'group': group, 'c_emp': c_emp,  'page': 'record',
 		'form': form, 'emp':emp,
 		'title': 'Aplika Licensa', 'legend': 'Aplika Licensa'
 	}
 	return render(request, 'leave/form.html', context)
 
+
+@login_required
+def hrLeaveAddProcess(request, hashid):
+	c_emp = get_object_or_404(Employee, hashed=hashid)
+	group = c_emp.employeeuser.user.groups.all()[0].name
+	lp = LeavePeriod.objects.filter(employee=c_emp,is_active=True).exists()
+	period = LeavePeriod.objects.filter(employee=c_emp,is_active=True).last()
+	
+	if period :
+
+		empdiv = CurEmpDivision.objects.get(employee=c_emp)
+		if lp == True:
+			if request.method == 'POST':
+				newid, new_hashid = getnewid(Leave)
+				form = LeaveForm(request.POST, request.FILES)
+				if form.is_valid():
+					today = dt.today().date()
+					leave_period = LeavePeriod.objects.filter(employee=c_emp,is_active=True).last()
+					start_date = form.cleaned_data.get('start_date')
+					end_date = form.cleaned_data.get('end_date')
+					start_time_status = form.cleaned_data.get('start_time_status')
+					end_time_status = form.cleaned_data.get('end_time_status')
+
+					start_dt = dt(start_date.year, start_date.month, start_date.day)
+					end_dt = dt(end_date.year, end_date.month, end_date.day)
+					try:
+						days = calculate_leave_days(start_dt, end_dt, start_time_status, end_time_status)
+					except ValueError as e:
+						messages.warning(request, str(e))
+						return render(request, 'leave/form.html', 
+		    				{ 
+							'message':e, 
+							'group': group, 'c_emp': c_emp, 'empdiv': empdiv, 'form': form, 'page': 'apply',
+							'title': 'Formulario Aplika Licensa', 'legend': 'Formulario Aplika Licensa'
+							}
+							)
+					days = round(float(days),2)
+					last_two_digits = str(days).split('.')[1][:2]
+					last_two_digits = int(last_two_digits)
+
+					min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
+					max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
+					date1 = pd.to_datetime(start_date, format="%Y %m").date()
+					date2 = pd.to_datetime(end_date, format="%Y %m").date()
+
+					start_date_period = pd.to_datetime(min_month, format="%Y %m").date()
+					end_date_period = pd.to_datetime(max_month, format="%Y %m").date()
+					start_month = date1
+					# cal_day = count_day(start_date, end_date)
+
+					if start_date_period <= start_month <= end_date_period + datetime.timedelta(days=29):
+						
+						leave_this_month = LeaveCount.objects.filter(period=leave_period, employee=c_emp, leave_type_id=1, update_date__lte=today).last()
+						if leave_this_month.balance >= 0.5:
+							if   days <= leave_this_month.balance or days <= leave_this_month.balance + 5 :
+
+								if days < 30  or days >= 30:
+									
+									if last_two_digits == int(5) or last_two_digits == int(0):
+										instance = form.save(commit=False)
+										instance.id = newid
+										instance.employee = c_emp
+										if group == "unit":
+											instance.unit_confirm = True
+											instance.unit_send = True
+										if group == "dep":
+											instance.is_lock = True
+											instance.is_send = True
+										if group == "de":
+											instance.is_lock = True
+											instance.is_approve = True
+											instance.is_finish = True
+											instance.is_finish = True
+											instance.pr_send = True
+											instance.obs = "Sim"
+											instance.pr_approve = True
+										instance.datetime = datetime.datetime.now()
+										instance.user = request.user
+										instance.hashed = new_hashid
+										instance.leave_period  = period
+										instance.is_create_by_hr  = True
+										instance.days = days
+										instance.save()
+										if group == "unit":
+											leaveunit = LeaveUnit.objects.filter(leave_id=newid).first()
+											leaveunit.obs = "Sim"
+											leaveunit.user = request.user
+											leaveunit.datetime = datetime.datetime.now()
+											leaveunit.save()
+										if group == "dep":
+
+											leavedep = LeaveDep.objects.filter(leave_id=newid).first()
+											leavedep.obs = "Sim"
+											leavedep.user = request.user
+											leavedep.datetime = datetime.datetime.now()
+											leavedep.save()
+										
+										messages.success(request, f'Aumeta sucessu.')
+										return redirect('leave-hr-leave-record', c_emp.hashed)
+									else:
+										messages.error(request,'Total loron nebe ita prienche latuir formato!! Total Loron Nebe Valido: *.00 Sura ba loron  no  *.5 Sura ba "Stengah Hari" ')
+								else:
+									messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
+							else:
+								messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
+						else:
+							messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
+					else:
+						messages.error(request,'Data hahu laiha periode ida ne nia laran. Halo Favor Kontakto Rekurso Humano hodi Kria Uluk Periode Licensa Foun!')
+			else: form = LeaveForm()
+		else:
+			messages.error(request, 'Periode ba Lisensa seidauk determina')
+			return redirect('leave-hr-leave-record', c_emp.hashed)
+		context = {
+			'group': group, 'c_emp': c_emp, 'empdiv': empdiv, 'form': form, 'page': 'apply',
+			'title': 'Formulario Aplika Licensa', 'legend': 'Formulario Aplika Licensa'
+		}
+		return render(request, 'leave/form.html', context)
+	else:
+		return redirect('leave-hr-leave-record', c_emp.hashed)
+
+
+@login_required
+def hrLeaveSendProcess(request, hashid, leave):
+	c_emp = get_object_or_404(Employee, hashed=hashid)
+	group = c_emp.employeeuser.user.groups.all()[0].name
+	objects = get_object_or_404(Leave, hashed=leave)
+	empdiv = CurEmpDivision.objects.get(employee=c_emp)
+	if group == "staff" or group == "hr":
+		check_ekipa = EmpPosition.objects.filter(Q(department__isnull=False)&Q(department=empdiv.department), is_active=True, is_manager=True).exists()
+		check_div = EmpPosition.objects.filter(Q(unit__isnull=False)&Q(unit=empdiv.unit), is_active=True, is_manager=True).exists()
+		if check_ekipa and check_div or check_ekipa:
+			objects.is_send =  True
+			objects.is_lock =  True
+			objects.is_finish =  False
+			objects.save()
+			messages.success(request, f'Manda ona.')
+			return redirect('leave-hr-leave-record', c_emp.hashed)
+		elif check_div:
+			objects.is_send_to_div =  True
+			objects.is_lock =  True
+			objects.is_finish =  False
+			objects.save()
+			messages.success(request, f'Manda ona.')
+			return redirect('leave-hr-leave-record', c_emp.hashed)
+		else:
+			messages.error(request, "Funsionario Refere Laiha Chefe Ekipa no Chefe Divizaun, Halo favor kontakto Rekurso Humano")
+			return redirect('leave-hr-leave-record', c_emp.hashed)
+
+
+@login_required
+@allowed_users(allowed_roles=['admin','hr'])
+def hrLeaveUpdateRecord(request):
+	employee = Employee.objects.filter(status_id=1)
+	for emp in employee:
+		contract = Contract.objects.filter(employee=emp, is_active=True).exists()
+		if contract:
+			leave_type = None
+			if emp.sex == 'Male':
+				leave_type = LeaveType.objects.exclude(pk=4)
+			else:
+				leave_type = LeaveType.objects.all()
+			leave_period = LeavePeriod.objects.filter(is_active=True, employee=emp).last()
+			check_last_period = LeavePeriod.objects.filter(pk__lt=leave_period.pk, employee=emp).last()
+			last_count_period = LeaveCount.objects.filter(employee=emp, period=check_last_period, leave_type_id=1).last()
+			min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
+			max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
+			months = pd.period_range(min_month, max_month, freq='M')
+			check_leave_count = LeaveCount.objects.filter(period=leave_period, employee=emp).exists()
+			if check_leave_count == False:
+				i = 0
+				while i < len(months):
+					leave_check = LeaveCount.objects.filter(employee=emp, period=leave_period).last()
+					m = months[i]
+					get_m = get_object_or_404(Mnth, code=m.month)
+					get_y = get_object_or_404(Yr, year=m.year)
+					if leave_check:
+						for lt1 in leave_type:
+							if lt1.pk == 1:
+								lastleaveal = LeaveCount.objects.filter(employee=emp, period=leave_period, leave_type_id=1).last()
+								earn_per_month = round(float(lt1.total/12),2)
+								date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
+								date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
+								lcnew = LeaveCount.objects.create(
+									period = leave_period,
+									employee=emp,
+									leave_type=lt1,
+									month = get_m,
+									year = get_y,
+									update_date = date_period,
+									leave_earn = earn_per_month
+								)
+								lcnew.balance = round(float(lastleaveal.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
+								lcnew.total_earn = round(float(lastleaveal.prov_total_earn) + float(lcnew.leave_earn),1)
+								lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
+								lcnew.balance_carry = lcnew.total_balance
+								lcnew.total_balance_leave = float(lt1.total) - float(lcnew.total_balance)
+								lcnew.prov_total_earn = float(lastleaveal.prov_total_earn) + float(earn_per_month)
+								lcnew.balance_month = round(float(lastleaveal.balance) - float(lcnew.taken),2)
+								lcnew.save()
+					else:
+						for lt in leave_type:
+							if lt.pk == 1:
+								# work: Check Balansu iha Periode Kotuk
+								date_period_string = f"{m.year}-{m.month}-{leave_period.start_date.day}"
+								date_period = dt.strptime(date_period_string,"%Y-%m-%d").date()
+								if check_last_period:
+									earn_per_month = round(float(lt.total/12),2)
+
+									lc = LeaveCount.objects.create(
+										period = leave_period,
+										employee=emp,
+										leave_type=lt,
+										month = get_m,
+										year = get_y,
+										update_date=date_period,
+										leave_earn = earn_per_month
+									)
+									lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
+									lc.total_earn = round(float(lc.leave_earn) + float(last_count_period.total_balance),2)
+									lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
+									lc.balance_carry = lc.total_balance
+									lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
+									lc.prov_total_earn = lc.total_earn
+									lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
+									lc.save()
+								else:
+									earn_per_month = round(float(lt.total/12),2)
+									# balance_per_month = round(float(earn_per_month) - float(taken),2)
+
+									lc = LeaveCount.objects.create(
+										period = leave_period,
+										employee=emp,
+										leave_type=lt,
+										month = get_m,
+										year = get_y,
+										update_date=date_period,
+										leave_earn = earn_per_month
+									)
+									lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
+									lc.total_earn = round(float(lc.leave_earn),2)
+									lc.total_balance = round(float(lc.balance),2)
+									lc.balance_carry = lc.total_balance
+									lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
+									lc.prov_total_earn = lc.leave_earn
+									lc.balance_month = round(float(lc.balance) - float(lc.taken),2)
+									lc.save()
+							else:
+								lcall = LeaveCount.objects.create(
+									period = leave_period,
+									employee=emp,
+									leave_type=lt,
+									year = get_y,
+								)
+								lcall.total_balance = float(lt.total)
+								lcall.save()
+					i+=1
+	messages.success(request, f'Susesu Update Record')
+	return redirect('leave-hr-app-raw-list')
+	
+
+def update_leave_count(alldata, month):
+
+	for obj in alldata:
+		print(obj)
+
+
+
 # work: Work Here
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrLeavePeriodAdd(request):
 	group = request.user.groups.all()[0].name
 	employee = Employee.objects.filter(status_id=1)
 	
@@ -556,75 +1018,70 @@
 		form = HRPeriodForm(request.POST)
 		if form.is_valid():
 			instance = form.save(commit=False)
 			start_year = form.cleaned_data.get('start_year')
 			end_year = form.cleaned_data.get('end_year')
 			if start_year.year == end_year.year:
 				messages.error(request, "Tinan Hahu ho Tinan Remata labele hanesan tinan remata !")
+			elif start_year.year >= end_year.year:
+				messages.error(request, "Tinan Hahu Labele boot liu Tinan Remata")
 			else:
 				for emp in employee:
-					contract = Contract.objects.filter(employee=emp, is_active=True).last()
-					allleavep = LeavePeriod.objects.filter(employee=emp)
-					for obj in allleavep:
-						obj.is_active = False
-						obj.save()
-					# instance.is_active = True
-					# instance.employee = emp
-					date_string = f'{start_year}-{contract.start_date.month}-{contract.start_date.day}'
-					start_period = dt.strptime(date_string, "%Y-%m-%d").date()
-					next_year = pd.date_range(start=start_period, end=start_period+pd.DateOffset(years=1), freq='M')
-					end_period = next_year.max()
-					# instance.start_month = get_object_or_404(Mnth, code=start_period.month)
-					# instance.end_month = get_object_or_404(Mnth, code=end_period.month)
-					# instance.start_year = get_object_or_404(Yr, year=start_period.year)
-					# instance.end_year = get_object_or_404(Yr, year=end_period.year)
-					# instance.start_date = start_period
-					# instance.end_date = end_period
-					# instance.save()
-					LeavePeriod.objects.create(
-						employee=emp, \
-						start_month = get_object_or_404(Mnth, code=start_period.month),\
-						end_month = get_object_or_404(Mnth, code=end_period.month), \
-						start_year = get_object_or_404(Yr, year=start_period.year), \
-						end_year = get_object_or_404(Yr, year=end_period.year), \
-						start_date = start_period,\
-						end_date = end_period,\
-						is_active = True
-					)
+					lp = LeavePeriod.objects.filter(start_year=start_year, end_year=end_year, employee=emp).exists()
+					if  lp == False:
+						contract = Contract.objects.filter(employee=emp, is_active=True).last()
+						if contract:
+							allleavep = LeavePeriod.objects.filter(employee=emp)
+							for obj in allleavep:
+								obj.is_active = False
+								obj.save()
+							# instance.is_active = True
+							# instance.employee = emp
+							date_string = f'{start_year}-{contract.start_date.month}-{contract.start_date.day}'
+							start_period = dt.strptime(date_string, "%Y-%m-%d").date()
+							next_year = pd.date_range(start=start_period, end=start_period+pd.DateOffset(years=1), freq='M')
+							end_period = next_year.max()
+							LeavePeriod.objects.create(
+								employee=emp, \
+								start_month = get_object_or_404(Mnth, code=start_period.month),\
+								end_month = get_object_or_404(Mnth, code=end_period.month), \
+								start_year = get_object_or_404(Yr, year=start_period.year), \
+								end_year = get_object_or_404(Yr, year=end_period.year), \
+								start_date = start_period,\
+								end_date = end_period,\
+								is_active = True
+							)
+					else:
+						messages.error(request, f'Funsionario {emp} Seidauk iha Kontrato')
 				messages.success(request, 'Susesu Aumenta Periode Licensa')
 				return redirect('leave-hr-app-raw-list')
-					
-
-
-
-					# if contract:
-					# else:
-					# 	messages.error(request, f'Funsrionario/a {emp} seidauk iha Kontrato')
-					# 	return redirect('leave-hr-app-raw-list')
 	else: form = HRPeriodForm()
 	context = {
-		'group': group,  'form':form,
+		'group': group,  'form':form, 'page':'period',
 		'title': 'Set Period Leave', 'legend': 'Set Period Leave'
 	}
 	return render(request, 'leave/form2.html', context)
 
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrLeaveEmpPeriodAdd(request, hashid):
 	group = request.user.groups.all()[0].name
 	employee = get_object_or_404(Employee, hashed=hashid)
 	contract = Contract.objects.filter(employee=employee, is_active=True).last()
+	period = LeavePeriod.objects.filter(employee=employee)
 	if request.method == 'POST':
 		form = HRPeriodForm(request.POST)
 		if form.is_valid():
 			instance = form.save(commit=False)
 			start_year = form.cleaned_data.get('start_year')
 			end_year = form.cleaned_data.get('end_year')
-			if start_year == end_year:
+			if start_year.year == end_year.year:
 				messages.error(request, "Tinan Hahu ho Tinan Remata labele hanesan")
+			elif start_year.year >= end_year.year:
+				messages.error(request, "Tinan Hahu labele boot liu Tinan Remata")
 			else:
 				allleavep = LeavePeriod.objects.filter(employee=employee)
 				for obj in allleavep:
 					obj.is_active = False
 					obj.save()
 				instance.is_active = True
 				instance.employee = employee
@@ -640,15 +1097,15 @@
 				instance.end_date = end_period
 				instance.save()
 				messages.success(request, 'Susesu Aumenta Periode Licensa')
 				return redirect('leave-hr-leave-record', hashid)
 	else: form = HRPeriodForm()
 	context = {
 		'group': group, 'form':form, 'page': 'add-emp-record', 'hashid': hashid,
-		'title': 'Set Period Leave', 'legend': 'Set Period Leave'
+		'title': 'Kria Periode Licensa', 'legend': 'Kria Periode Licensa', 'period': period
 	}
 	return render(request, 'leave/form2.html', context)
 
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def hrLeaveEmpUpdatePeriodMonth(request, hashid):
 	today = dt.today().date()
@@ -666,34 +1123,21 @@
 			period = leave_period,
 			employee=employee,
 			leave_type=lt,
 			month = get_m,
 			year = get_y,
 			leave_earn = earn_per_month
 		)
-		# lc.balance = round(float(lc.leave_earn) - float(lc.taken),2)
-		# lc.total_earn = round(float(lc.leave_earn) + float(leave_count_last.total_balance),2)
-		# lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),2)
-		# lc.balance_carry = lc.total_balance
-		# lc.total_balance_leave = float(lt.total) - float(lc.total_balance)
-		# lc.prov_total_earn = lc.total_earn
-		# lc.save()
-		# lc.taken = round(float(lc.taken) + days,2)
-		# lc.total_taken = round(float(leave_count_last.taken) + days)
-		# lc.balance = round(float(leave_count_last.balance) + float(lc.leave_earn) - float(days),2 )
-		# lc.total_balance = round(float(lc.total_earn) - float(lc.total_taken),1)
-		# lc.save()
 		lcnew.balance = round(float(leave_count_last.balance) + float(lcnew.leave_earn) - float(lcnew.taken),2)
 		lcnew.total_earn = round(float(leave_count_last.prov_total_earn) + float(lcnew.leave_earn),1)
 		lcnew.total_balance = round(float(lcnew.total_earn) - float(lcnew.total_taken),1)
 		lcnew.balance_carry = lcnew.total_balance
 		lcnew.total_balance_leave = float(lt.total) - float(lcnew.total_balance)
 		lcnew.prov_total_earn = float(leave_count_last.prov_total_earn) + float(earn_per_month)
 		lcnew.save()
-	# previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type_id=1, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
 		messages.success(request, 'Susesu kria Record iha fulan ida ne')
 		return redirect('leave-hr-leave-record', hashid)
 	else:
 		messages.error(request, 'Deskulpa Laiha Licensa iha Fulan kotuk')
 		return redirect('leave-hr-leave-record', hashid)
 
 
@@ -741,23 +1185,20 @@
 	return redirect('leave-hr-app-detail', hashid)
 @login_required
 @allowed_users(allowed_roles=['hr','hr_s'])
 def hrLeaveUpdateAtt(request, hashid, hashid2):
 	group = request.user.groups.all()[0].name
 	employee = get_object_or_404(Employee, hashed=hashid)
 	leave_period = LeavePeriod.objects.filter(employee=employee,is_active=True).last()
-	check_last_period = LeavePeriod.objects.filter(employee=employee, is_active=True, pk__lt=leave_period.pk).last()
+	check_last_period = LeavePeriod.objects.filter(employee=employee,  pk__lt=leave_period.pk).last()
 	last_count_period = LeaveCount.objects.filter(employee=employee, period=check_last_period, leave_type_id=1).last()
 	min_month = f'{leave_period.start_year.year}-{leave_period.start_month.code}'
 	max_month = f'{leave_period.end_year.year}-{leave_period.end_month.code}'
 	months = pd.period_range(min_month, max_month, freq='M')
 	leave = get_object_or_404(Leave, hashed=hashid2)
-	c_emp = employee
-	newid, new_hashid = getnewid(Leave)
-	newsid2, _ = getnewid(LeaveCount)
 
 
 	leave_type = leave.leave_type
 	days = leave.days
 	days = round(float(days),2)
 
 	if leave_type.pk == 1: earn_per_month = round(float(leave_type.total/12),2)
@@ -780,85 +1221,119 @@
 	if days <= leave_type.total:
 		# done: CHECK ANGKA LORON 0.5/1.0/1.5
 		if last_two_digits == int(5) or last_two_digits == int(0):
 			# done: CHECK DATA LEAVE IHA PERIODO NIA LARAN
 			if start_date_period <= start_month <= end_date_period + datetime.timedelta(days=29):
 				# done: CHECK LEAVE TYPE BA ANNUAL
 				if leave_type.pk == 1:
+					
 					# done: CHECK RECORD IHA FULAN IDA NE'E
-					current_leave_count = get_object_or_404(LeaveCount, period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year)
-					previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
+					
+					current_leave_count = LeaveCount.objects.filter(period=leave_period, employee=employee,leave_type= leave_type, month__code=start_date.month, year__year=start_date.year).last()
+					if current_leave_count:
+						previous_leave_count = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type= leave_type, month__code__lt=start_date.month, year__year=current_leave_count.year.year).last()
 					# done: CHECK KARIK LEAVE IHA FULAN KLARAN
 					if previous_leave_count:
 						current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
 						current_leave_count.total_taken = round(float(previous_leave_count.taken) + days)
 						current_leave_count.balance = round(float(previous_leave_count.balance) + float(current_leave_count.leave_earn) - float(days),2 )
 						current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
 						current_leave_count.balance_month = round(float(previous_leave_count.balance) - float(current_leave_count.taken),2)
 						current_leave_count.save()
 
 
+
 						#done: KRIA ATTENDANCE
-						createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)							
+						createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)							
 					# done: CHECK KARIK LEAVE IHA FULAN PRIMEIRU
 					else:
 						current_leave_count.taken = round(float(current_leave_count.taken) + days,2)
-						current_leave_count.total_taken = current_leave_count.taken
-						current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
-						current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
-						current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
-						current_leave_count.save()
+						if check_last_period:
+							current_leave_count.total_taken = current_leave_count.taken
+							current_leave_count.total_earn = round(float(last_count_period.total_balance) + float(earn_per_month),1)
+							current_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) - float(current_leave_count.taken),2 )
+							current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+							current_leave_count.balance_month = round(float(current_leave_count.total_balance) - float(current_leave_count.taken),2)
+							current_leave_count.save()
+						else:
+							current_leave_count.total_taken = current_leave_count.taken
+							current_leave_count.balance = round(float(current_leave_count.leave_earn) - float(current_leave_count.taken),2 )
+							current_leave_count.total_balance = round(float(current_leave_count.total_earn) - float(current_leave_count.total_taken),1)
+							current_leave_count.balance_month = round(float(current_leave_count.balance) - float(current_leave_count.taken),2)
+							current_leave_count.save()
 
 						# done: KRIA ATTENDANCE
-						createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+						createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)
 
 
 					i = 0
 					# done: UPDATE LEAVE RECORD
 					while i < len(months):
 						m = months[i]
 						if i == int(0):
 							# done: FULAN PRIMEIRO
 							if check_last_period:
 								first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
-								first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
+								first_leave_count.balance = round(float(last_count_period.total_balance) + float(earn_per_month) -  float(first_leave_count.taken),2)
 								first_leave_count.total_earn = round(float(first_leave_count.leave_earn) + float(last_count_period.total_balance),2)
 								first_leave_count.total_balance = round(float(first_leave_count.total_earn) - float(first_leave_count.total_taken),2)
 								first_leave_count.balance_carry = first_leave_count.total_balance
 								first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
 								first_leave_count.prov_total_earn = first_leave_count.total_earn
 								first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
 								first_leave_count.save()
+
 							else:
-								first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
-								first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
-								first_leave_count.total_earn = round(float(first_leave_count.leave_earn),2)
-								first_leave_count.total_balance = round(float(first_leave_count.balance),2)
-								first_leave_count.balance_carry = first_leave_count.total_balance
-								first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
-								first_leave_count.prov_total_earn = first_leave_count.leave_earn
-								first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
-								first_leave_count.save()
+								if leave_period.balance_carry > 0.00:
+									first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+									first_leave_count.balance = round(float(leave_period.balance_carry) + float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
+									first_leave_count.total_earn = round(float(leave_period.balance_carry) + float(first_leave_count.leave_earn),2)
+									first_leave_count.total_balance = round( float(first_leave_count.balance),2)
+									first_leave_count.balance_carry = first_leave_count.total_balance
+									first_leave_count.total_balance_leave = float(leave_period.balance_carry) + float(leave_type.total) - float(first_leave_count.total_balance)
+									first_leave_count.prov_total_earn =  float(leave_period.balance_carry) + float(first_leave_count.leave_earn)
+									first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+									first_leave_count.save()
+								else:
+									first_leave_count = LeaveCount.objects.filter(employee=employee,month__code=m.month, year__year=m.year, period=leave_period,leave_type=leave_type).first()
+									first_leave_count.balance = round(float(first_leave_count.leave_earn) - float(first_leave_count.taken),2)
+									first_leave_count.total_earn = round(float(first_leave_count.leave_earn),2)
+									first_leave_count.total_balance = round(float(first_leave_count.balance),2)
+									first_leave_count.balance_carry = first_leave_count.total_balance
+									first_leave_count.total_balance_leave = float(leave_type.total) - float(first_leave_count.total_balance)
+									first_leave_count.prov_total_earn = first_leave_count.leave_earn
+									first_leave_count.balance_month = round(float(first_leave_count.balance) - float(first_leave_count.taken),2)
+									first_leave_count.save()
 
 						else:
 							# done: FULAN TUIR MAI
 							prev_mont = m.asfreq("M", "S") - 1
 							lccurrent = get_object_or_404(LeaveCount, employee=employee, period=leave_period, leave_type=leave_type,  year__year=m.year, month__code=m.month)
 							lclast = LeaveCount.objects.filter(employee=employee, period=leave_period, leave_type=leave_type,  year__year=prev_mont.year, month__code=prev_mont.month).first()
 
-
-							lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
-							lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
-							lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
-							lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
-							lccurrent.balance_carry = lccurrent.total_balance
-							lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
-							lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
-							lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
-							lccurrent.save()
+							if leave_period.balance_carry > 0.00:
+								lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
+								lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
+								lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
+								lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
+								lccurrent.balance_carry = lccurrent.total_balance
+								lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
+								lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
+								lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
+								lccurrent.save()
+							else:
+								lccurrent.balance = round(float(lclast.balance) + float(lccurrent.leave_earn) - float(lccurrent.taken),2)
+								lccurrent.total_earn = round(float(lclast.prov_total_earn) + float(lccurrent.leave_earn),1)
+								lccurrent.total_taken = round(float(lclast.total_taken) + float(lccurrent.taken),2)
+								lccurrent.total_balance = round(float(lccurrent.total_earn) - float(lccurrent.total_taken),1)
+								lccurrent.balance_carry = lccurrent.total_balance
+								lccurrent.total_balance_leave = float(leave_type.total) - float(lccurrent.total_balance)
+								lccurrent.prov_total_earn = float(lclast.prov_total_earn) + float(earn_per_month)
+								lccurrent.balance_month = round(float(lclast.balance) - float(lccurrent.taken),2)
+								lccurrent.save()
 
 						i+=1
 
 					# done: KRIA LEAVE
 
 				# done: CHECK KARIK LEAVE LAOS ANNUAL LEAVE
 				else:
@@ -874,15 +1349,15 @@
 						# work: Leave Nebe Iha ona
 						if days <= previous_leave_count.total_balance:
 							if month_leave_count:
 								month_leave_count.taken = round(float(month_leave_count.taken) + days, 2)
 								month_leave_count.total_taken = round(float(previous_leave_count.total_taken) +  days,2)
 								month_leave_count.total_balance = round(float(leave_type.total) - float(month_leave_count.total_taken),2)
 								month_leave_count.save()
-								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+								createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)
 								messages.success(request, 'Susesu Altera')
 								return redirect('leave-hr-app-detail', hashid2)
 							else:
 								lc = LeaveCount.objects.create(
 									period = leave_period,
 									employee = employee,
 									leave_type = leave_type,
@@ -891,15 +1366,15 @@
 
 								)
 								lc.taken = days
 								lc.total_taken = round(float(previous_leave_count.total_taken) + float(lc.taken),2)
 								lc.total_balance = round(float(leave_type.total) - float(lc.total_taken),2)
 								lc.save()
 
-								createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+								createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)
 
 								messages.success(request, 'Susesu Altera')
 								return redirect('leave-hr-app-detail', hashid2)
 						else:
 							messages.error(request, 'Loron nebe hili barak liu. Halo favor altera loron nebe ita prienche')
 					# done: CHECK LEAVE COUNT NEBE IHA NO FULAN ONA IHA
 					else:
@@ -909,30 +1384,26 @@
 							year=getyear,
 							taken = days,
 							total_taken = days,
 							total_balance = round(float(leave_type.total) - float(days),2)
 						)
 
 						# KRIA ATTENDANCE
-						createAttendance(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten)
+						createAttendanceEmp(request, leave_type, Attendance, AttendanceStatus, employee, start_date, end_date, YAten, Maten, leave)
 
 						messages.success(request, 'Susesu Altera')
 						return redirect('leave-hr-app-detail', hashid2)
 				
 			# done: ERROR KARIK DATA HAHU LAIHA PERIODE NIA LARAN
 			else:
 				messages.error(request,'Data hahu laiha periode ida ne nia laran!!')
 		else:
 			messages.error(request,'Total loron nebe ita prienche latuir formato!!')
 	else:
 		messages.error(request, f'Loron nebe hili barak liu. Halo favor hare regulamentu konaba total licenca.')
 	
-
-
-
 	leave.hr_confirm = True
-	leave.is_done = True
 	leave.save()
 
 
 	messages.success(request, 'Susesu Altera')
 	return redirect('leave-hr-app-detail', hashid2)
```

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_hr_v.py` & `django-ipghrms-leave-1.2/leave/views/leave_hr_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_m.py` & `django-ipghrms-leave-1.2/leave/views/leave_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_report.py` & `django-ipghrms-leave-1.2/leave/views/leave_report.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_s_m.py` & `django-ipghrms-leave-1.2/leave/views/leave_s_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_s_v.py` & `django-ipghrms-leave-1.2/leave/views/leave_s_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/leave_v.py` & `django-ipghrms-leave-1.2/leave/views/leave_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-leave-1.1/leave/views/print.py` & `django-ipghrms-leave-1.2/leave/views/print.py`

 * *Files identical despite different names*

