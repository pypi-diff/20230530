# Comparing `tmp/ora-0.8.0.tar.gz` & `tmp/ora-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ora-0.8.0.tar", last modified: Fri Feb 24 15:35:03 2023, max compression
+gzip compressed data, was "ora-0.8.2.tar", last modified: Tue May 30 04:08:17 2023, max compression
```

## Comparing `ora-0.8.0.tar` & `ora-0.8.2.tar`

### file list

```diff
@@ -1,776 +1,776 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.314155 ora-0.8.0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1434 2018-02-04 13:58:16.000000 ora-0.8.0/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)      177 2018-01-06 02:31:51.000000 ora-0.8.0/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)     6981 2022-09-02 14:11:06.000000 ora-0.8.0/Makefile
--rw-r--r--   0 alex      (1000) alex      (1000)      852 2023-02-24 15:35:03.314155 ora-0.8.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     1827 2023-02-22 21:07:29.000000 ora-0.8.0/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.260821 ora-0.8.0/cxx/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.260821 ora-0.8.0/cxx/include/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.260821 ora-0.8.0/cxx/include/ora/
--rw-r--r--   0 alex      (1000) alex      (1000)     7624 2022-06-30 13:17:10.000000 ora-0.8.0/cxx/include/ora/calendar.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     7583 2022-08-23 15:25:52.000000 ora-0.8.0/cxx/include/ora/date_functions.hh
--rw-r--r--   0 alex      (1000) alex      (1000)    10045 2022-06-30 13:17:10.000000 ora-0.8.0/cxx/include/ora/date_math.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     8905 2019-04-26 23:55:08.000000 ora-0.8.0/cxx/include/ora/date_nex.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     8137 2019-04-25 21:58:07.000000 ora-0.8.0/cxx/include/ora/date_type.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     8138 2022-08-23 15:25:52.000000 ora-0.8.0/cxx/include/ora/daytime_functions.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     1220 2021-01-07 03:02:55.000000 ora-0.8.0/cxx/include/ora/daytime_math.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     8811 2021-02-05 14:47:42.000000 ora-0.8.0/cxx/include/ora/daytime_nex.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     7151 2019-04-25 12:21:33.000000 ora-0.8.0/cxx/include/ora/daytime_type.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     3024 2022-06-30 13:17:10.000000 ora-0.8.0/cxx/include/ora/exceptions.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     2221 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/include/ora/ez.hh
--rw-r--r--   0 alex      (1000) alex      (1000)    12600 2022-09-02 14:00:40.000000 ora-0.8.0/cxx/include/ora/format.hh
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.264155 ora-0.8.0/cxx/include/ora/lib/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3233 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/include/ora/lib/exc.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     1316 2018-06-10 22:27:05.000000 ora-0.8.0/cxx/include/ora/lib/file.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     5352 2018-02-25 19:53:06.000000 ora-0.8.0/cxx/include/ora/lib/filename.hh
--rw-r--r--   0 alex      (1000) alex      (1000)      573 2022-06-30 13:17:10.000000 ora-0.8.0/cxx/include/ora/lib/iter.hh
--rw-r--r--   0 alex      (1000) alex      (1000)    10043 2022-06-30 13:17:10.000000 ora-0.8.0/cxx/include/ora/lib/math.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     2266 2018-03-15 00:42:49.000000 ora-0.8.0/cxx/include/ora/lib/mem.hh
--rw-r--r--   0 alex      (1000) alex      (1000)      951 2018-03-23 04:22:20.000000 ora-0.8.0/cxx/include/ora/lib/num.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     2365 2018-02-24 21:31:57.000000 ora-0.8.0/cxx/include/ora/lib/string.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     2708 2022-08-23 15:28:33.000000 ora-0.8.0/cxx/include/ora/lib/string_builder.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     3913 2019-04-20 14:00:12.000000 ora-0.8.0/cxx/include/ora/lib/xsys.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     7378 2019-04-20 14:00:12.000000 ora-0.8.0/cxx/include/ora/localization.hh
--rw-r--r--   0 alex      (1000) alex      (1000)      988 2018-04-04 03:49:28.000000 ora-0.8.0/cxx/include/ora/localization_nex.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     3226 2021-02-05 14:47:42.000000 ora-0.8.0/cxx/include/ora/parse.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     2090 2022-06-30 13:17:10.000000 ora-0.8.0/cxx/include/ora/posixtz.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     5064 2022-08-23 15:25:52.000000 ora-0.8.0/cxx/include/ora/time_functions.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     1892 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/include/ora/time_interval.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     6117 2022-08-31 13:49:38.000000 ora-0.8.0/cxx/include/ora/time_math.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     6204 2019-04-26 23:55:08.000000 ora-0.8.0/cxx/include/ora/time_nex.hh
--rw-r--r--   0 alex      (1000) alex      (1000)    11989 2018-03-17 18:19:37.000000 ora-0.8.0/cxx/include/ora/time_type.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     3951 2022-04-19 00:19:42.000000 ora-0.8.0/cxx/include/ora/time_zone.hh
--rw-r--r--   0 alex      (1000) alex      (1000)    11830 2022-06-30 13:17:10.000000 ora-0.8.0/cxx/include/ora/types.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     1189 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/include/ora/tzfile.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     1309 2022-04-19 00:19:42.000000 ora-0.8.0/cxx/include/ora.hh
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.264155 ora-0.8.0/cxx/src/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.264155 ora-0.8.0/cxx/src/bin/
--rw-r--r--   0 alex      (1000) alex      (1000)      546 2022-04-19 00:19:42.000000 ora-0.8.0/cxx/src/bin/posixtz.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)      483 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/src/bin/tzdump.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     3592 2018-06-18 05:06:26.000000 ora-0.8.0/cxx/src/calendar.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)      354 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/src/date.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     5020 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/src/date_math.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)      426 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/src/daytime.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)      919 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/src/daytime_math.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)      995 2020-01-28 04:52:24.000000 ora-0.8.0/cxx/src/file.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     4718 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/src/filename.cc
--rw-r--r--   0 alex      (1000) alex      (1000)    17786 2022-09-02 14:00:40.000000 ora-0.8.0/cxx/src/format.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)    16071 2020-01-28 22:41:09.000000 ora-0.8.0/cxx/src/parse.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     4112 2022-04-19 00:19:42.000000 ora-0.8.0/cxx/src/posixtz.cc
--rw-r--r--   0 alex      (1000) alex      (1000)      553 2018-03-06 01:08:17.000000 ora-0.8.0/cxx/src/time.cc
--rw-r--r--   0 alex      (1000) alex      (1000)    14150 2022-06-30 13:17:10.000000 ora-0.8.0/cxx/src/time_zone.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     7410 2022-04-19 00:19:42.000000 ora-0.8.0/cxx/src/tzfile.cc
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.264155 ora-0.8.0/cxx/test/
--rw-r--r--   0 alex      (1000) alex      (1000)     5290 2018-06-18 05:06:26.000000 ora-0.8.0/cxx/test/calendar.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     9191 2020-01-28 20:53:07.000000 ora-0.8.0/cxx/test/date.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     2747 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/date_format.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)    19480 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/date_functions.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     7364 2022-06-30 13:17:10.000000 ora-0.8.0/cxx/test/date_math.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)    17118 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/date_nex.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     8658 2021-02-05 14:47:42.000000 ora-0.8.0/cxx/test/daytime.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     2177 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/daytime_functions.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     8319 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/daytime_nex.cc
--rw-r--r--   0 alex      (1000) alex      (1000)    13605 2022-08-30 16:05:15.000000 ora-0.8.0/cxx/test/format.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     1959 2018-03-06 01:08:17.000000 ora-0.8.0/cxx/test/from_local.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)      589 2020-01-28 22:12:58.000000 ora-0.8.0/cxx/test/parse.cc
--rw-r--r--   0 alex      (1000) alex      (1000)      842 2022-04-19 00:19:42.000000 ora-0.8.0/cxx/test/posixtz.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     1242 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/string_builder.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     8949 2022-08-30 16:05:24.000000 ora-0.8.0/cxx/test/time.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)      639 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/time128.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     2312 2018-03-06 01:08:17.000000 ora-0.8.0/cxx/test/time_format.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     1595 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/time_functions.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     1463 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/time_interval.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     2567 2017-12-29 05:42:53.000000 ora-0.8.0/cxx/test/time_nex.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     1778 2018-02-27 05:08:25.000000 ora-0.8.0/cxx/test/time_zone.cc
--rw-r--r--   0 alex      (1000) alex      (1000)      862 2018-01-15 15:41:52.000000 ora-0.8.0/cxx/test/to_local.cc
--rw-r--r--   0 alex      (1000) alex      (1000)      115 2022-08-23 15:25:46.000000 ora-0.8.0/pyproject.toml
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.264155 ora-0.8.0/python/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.267488 ora-0.8.0/python/ora/
--rw-r--r--   0 alex      (1000) alex      (1000)     8174 2023-02-24 15:34:51.000000 ora-0.8.0/python/ora/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3905 2022-06-30 13:17:10.000000 ora-0.8.0/python/ora/calendar.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.267488 ora-0.8.0/python/ora/calendars/
--rw-rw-r--   0 alex      (1000) alex      (1000)    30395 2018-07-12 17:55:16.000000 ora-0.8.0/python/ora/calendars/usa-federal-businessdays.cal
--rw-rw-r--   0 alex      (1000) alex      (1000)     3115 2018-07-12 17:55:16.000000 ora-0.8.0/python/ora/calendars/usa-federal-holidays.cal
--rw-rw-r--   0 alex      (1000) alex      (1000)     1304 2017-12-29 05:42:53.000000 ora-0.8.0/python/ora/date.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1506 2017-12-29 05:42:53.000000 ora-0.8.0/python/ora/date_expr.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1141 2017-12-29 05:42:53.000000 ora-0.8.0/python/ora/daytime.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.270821 ora-0.8.0/python/ora/ext/
--rw-r--r--   0 alex      (1000) alex      (1000)    15876 2023-02-22 21:07:05.000000 ora-0.8.0/python/ora/ext/functions.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     5374 2019-10-08 20:03:36.000000 ora-0.8.0/python/ora/ext/functions.docstrings
--rw-r--r--   0 alex      (1000) alex      (1000)     5976 2022-08-23 15:28:33.000000 ora-0.8.0/python/ora/ext/module.cc
--rw-r--r--   0 alex      (1000) alex      (1000)      358 2019-05-09 04:13:11.000000 ora-0.8.0/python/ora/ext/np.cc
--rw-r--r--   0 alex      (1000) alex      (1000)    16039 2022-08-23 15:28:33.000000 ora-0.8.0/python/ora/ext/np.hh
--rw-r--r--   0 alex      (1000) alex      (1000)      456 2019-05-09 04:13:11.000000 ora-0.8.0/python/ora/ext/np_date.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)       83 2019-04-20 14:00:12.000000 ora-0.8.0/python/ora/ext/np_date.docstrings
--rw-r--r--   0 alex      (1000) alex      (1000)    18788 2022-06-30 13:17:10.000000 ora-0.8.0/python/ora/ext/np_date.hh
--rw-r--r--   0 alex      (1000) alex      (1000)      335 2019-05-09 04:13:11.000000 ora-0.8.0/python/ora/ext/np_daytime.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)    15106 2021-02-05 14:47:42.000000 ora-0.8.0/python/ora/ext/np_daytime.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)    14660 2021-02-05 14:47:42.000000 ora-0.8.0/python/ora/ext/np_functions.cc
--rw-r--r--   0 alex      (1000) alex      (1000)      307 2019-05-09 04:13:11.000000 ora-0.8.0/python/ora/ext/np_time.cc
--rw-r--r--   0 alex      (1000) alex      (1000)    15414 2022-08-23 15:28:33.000000 ora-0.8.0/python/ora/ext/np_time.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     1884 2020-01-22 10:43:33.000000 ora-0.8.0/python/ora/ext/np_types.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     1437 2021-02-05 14:47:42.000000 ora-0.8.0/python/ora/ext/np_types.hh
--rw-r--r--   0 alex      (1000) alex      (1000)      527 2018-04-16 01:25:33.000000 ora-0.8.0/python/ora/ext/py.cc
--rw-r--r--   0 alex      (1000) alex      (1000)    42365 2023-02-22 21:07:05.000000 ora-0.8.0/python/ora/ext/py.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     2086 2018-08-17 16:12:13.000000 ora-0.8.0/python/ora/ext/py_cal_functions.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)    14379 2018-07-12 17:55:16.000000 ora-0.8.0/python/ora/ext/py_calendar.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     1509 2018-06-18 05:06:26.000000 ora-0.8.0/python/ora/ext/py_calendar.docstrings
--rw-rw-r--   0 alex      (1000) alex      (1000)     1902 2018-08-17 16:12:13.000000 ora-0.8.0/python/ora/ext/py_calendar.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     4898 2020-01-28 21:59:02.000000 ora-0.8.0/python/ora/ext/py_date.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     5158 2018-04-16 01:25:33.000000 ora-0.8.0/python/ora/ext/py_date.docstrings
--rw-r--r--   0 alex      (1000) alex      (1000)    36744 2022-08-23 15:28:33.000000 ora-0.8.0/python/ora/ext/py_date.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     5601 2022-08-23 20:21:34.000000 ora-0.8.0/python/ora/ext/py_date_fmt.cc
--rw-r--r--   0 alex      (1000) alex      (1000)      709 2022-08-23 15:28:33.000000 ora-0.8.0/python/ora/ext/py_date_fmt.hh
--rw-r--r--   0 alex      (1000) alex      (1000)      473 2018-04-16 01:25:33.000000 ora-0.8.0/python/ora/ext/py_date_inst.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     1188 2020-01-22 10:43:33.000000 ora-0.8.0/python/ora/ext/py_daytime.cc
--rw-rw-r--   0 alex      (1000) alex      (1000)     3944 2021-02-05 14:47:42.000000 ora-0.8.0/python/ora/ext/py_daytime.docstrings
--rw-r--r--   0 alex      (1000) alex      (1000)    31799 2022-08-23 15:28:33.000000 ora-0.8.0/python/ora/ext/py_daytime.hh
--rw-r--r--   0 alex      (1000) alex      (1000)      554 2018-04-16 01:25:33.000000 ora-0.8.0/python/ora/ext/py_daytime_inst.cc
--rw-r--r--   0 alex      (1000) alex      (1000)    14739 2023-02-14 15:47:00.000000 ora-0.8.0/python/ora/ext/py_local.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     1392 2018-04-16 01:25:33.000000 ora-0.8.0/python/ora/ext/py_local.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     2172 2020-01-28 22:20:23.000000 ora-0.8.0/python/ora/ext/py_time.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     1148 2018-04-16 01:25:33.000000 ora-0.8.0/python/ora/ext/py_time.docstrings
--rw-r--r--   0 alex      (1000) alex      (1000)    32458 2023-02-14 05:56:05.000000 ora-0.8.0/python/ora/ext/py_time.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     6460 2022-09-02 14:00:40.000000 ora-0.8.0/python/ora/ext/py_time_fmt.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     1001 2022-09-02 14:00:40.000000 ora-0.8.0/python/ora/ext/py_time_fmt.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     3883 2019-04-26 23:55:08.000000 ora-0.8.0/python/ora/ext/py_time_inst.cc
--rw-r--r--   0 alex      (1000) alex      (1000)    17861 2022-06-30 13:17:10.000000 ora-0.8.0/python/ora/ext/py_time_zone.cc
--rw-r--r--   0 alex      (1000) alex      (1000)     2823 2018-05-29 10:54:24.000000 ora-0.8.0/python/ora/ext/py_time_zone.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     5531 2022-08-23 15:28:33.000000 ora-0.8.0/python/ora/ext/text.hh
--rw-r--r--   0 alex      (1000) alex      (1000)     2244 2018-06-18 05:06:26.000000 ora-0.8.0/python/ora/ext/types.cc
--rw-r--r--   0 alex      (1000) alex      (1000)      280 2018-04-16 01:25:33.000000 ora-0.8.0/python/ora/ext/types.docstrings
--rw-r--r--   0 alex      (1000) alex      (1000)      440 2018-04-16 01:25:33.000000 ora-0.8.0/python/ora/ext/types.hh
--rw-rw-r--   0 alex      (1000) alex      (1000)     2348 2020-01-22 10:43:33.000000 ora-0.8.0/python/ora/ext/util.hh
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.270821 ora-0.8.0/python/ora/np/
--rw-rw-r--   0 alex      (1000) alex      (1000)      776 2020-01-22 10:43:33.000000 ora-0.8.0/python/ora/np/__init__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.270821 ora-0.8.0/python/ora/test/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1028 2017-12-29 05:42:53.000000 ora-0.8.0/python/ora/test/data.py
--rw-r--r--   0 alex      (1000) alex      (1000)       89 2018-06-18 05:06:26.000000 ora-0.8.0/python/ora/test/june18.cal
--rw-rw-r--   0 alex      (1000) alex      (1000)     6973 2018-07-12 17:55:16.000000 ora-0.8.0/python/ora/test/test_calendar.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6294 2022-08-23 15:28:33.000000 ora-0.8.0/python/ora/test/test_date_basic.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      935 2017-12-29 05:42:53.000000 ora-0.8.0/python/ora/test/test_date_datenum.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3746 2017-12-29 05:42:53.000000 ora-0.8.0/python/ora/test/test_date_math.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3971 2017-12-29 05:42:53.000000 ora-0.8.0/python/ora/test/test_date_parts.py
--rw-r--r--   0 alex      (1000) alex      (1000)    12064 2022-08-30 16:05:15.000000 ora-0.8.0/python/ora/test/test_daytime_basic.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4025 2022-09-02 14:00:40.000000 ora-0.8.0/python/ora/test/test_fmt.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3975 2022-08-23 15:28:33.000000 ora-0.8.0/python/ora/test/test_from_local.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1531 2017-12-29 05:42:53.000000 ora-0.8.0/python/ora/test/test_functions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1393 2020-01-22 10:43:33.000000 ora-0.8.0/python/ora/test/test_local.py
--rw-r--r--   0 alex      (1000) alex      (1000)    11320 2022-05-03 05:19:52.000000 ora-0.8.0/python/ora/test/test_np_date.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6487 2022-04-20 04:33:32.000000 ora-0.8.0/python/ora/test/test_np_daytime.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3090 2019-05-09 04:13:11.000000 ora-0.8.0/python/ora/test/test_np_functions.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8653 2022-05-03 05:19:52.000000 ora-0.8.0/python/ora/test/test_np_time.py
--rw-r--r--   0 alex      (1000) alex      (1000)      976 2018-04-16 01:25:33.000000 ora-0.8.0/python/ora/test/test_np_ufuncs_time.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5474 2020-01-28 21:11:33.000000 ora-0.8.0/python/ora/test/test_parse_date.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4467 2020-01-28 21:06:45.000000 ora-0.8.0/python/ora/test/test_parse_daytime.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6611 2020-01-28 22:11:02.000000 ora-0.8.0/python/ora/test/test_parse_time.py
--rw-r--r--   0 alex      (1000) alex      (1000)    14621 2022-08-30 16:05:15.000000 ora-0.8.0/python/ora/test/test_time_basic.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6289 2023-02-22 19:50:46.000000 ora-0.8.0/python/ora/test/test_time_zone.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1744 2023-02-22 21:07:05.000000 ora-0.8.0/python/ora/test/test_time_zone_dir.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1591 2022-09-02 18:47:47.000000 ora-0.8.0/python/ora/test/test_vs_zoneinfo.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      330 2018-02-27 05:06:31.000000 ora-0.8.0/python/ora/test/tools.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1903 2018-06-18 05:06:26.000000 ora-0.8.0/python/ora/util.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2285 2018-07-12 17:55:16.000000 ora-0.8.0/python/ora/weekday.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.274155 ora-0.8.0/python/ora/zoneinfo/
--rw-r--r--   0 alex      (1000) alex      (1000)        6 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/+VERSION
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.280822 ora-0.8.0/python/ora/zoneinfo/Africa/
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Abidjan
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Accra
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Addis_Ababa
--rw-r--r--   0 alex      (1000) alex      (1000)      470 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Algiers
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Asmara
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Asmera
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Bamako
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Bangui
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Banjul
--rw-r--r--   0 alex      (1000) alex      (1000)      149 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Bissau
--rw-r--r--   0 alex      (1000) alex      (1000)      131 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Blantyre
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Brazzaville
--rw-r--r--   0 alex      (1000) alex      (1000)      131 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Bujumbura
--rw-r--r--   0 alex      (1000) alex      (1000)     1276 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Cairo
--rw-r--r--   0 alex      (1000) alex      (1000)     1919 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Casablanca
--rw-r--r--   0 alex      (1000) alex      (1000)      562 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Ceuta
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Conakry
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Dakar
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Dar_es_Salaam
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Djibouti
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Douala
--rw-r--r--   0 alex      (1000) alex      (1000)     1830 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/El_Aaiun
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Freetown
--rw-r--r--   0 alex      (1000) alex      (1000)      131 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Gaborone
--rw-r--r--   0 alex      (1000) alex      (1000)      131 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Harare
--rw-r--r--   0 alex      (1000) alex      (1000)      190 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Johannesburg
--rw-r--r--   0 alex      (1000) alex      (1000)      458 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Juba
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Kampala
--rw-r--r--   0 alex      (1000) alex      (1000)      458 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Khartoum
--rw-r--r--   0 alex      (1000) alex      (1000)      131 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Kigali
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Kinshasa
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Lagos
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Libreville
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Lome
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Luanda
--rw-r--r--   0 alex      (1000) alex      (1000)      131 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Lubumbashi
--rw-r--r--   0 alex      (1000) alex      (1000)      131 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Lusaka
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Malabo
--rw-r--r--   0 alex      (1000) alex      (1000)      131 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Maputo
--rw-r--r--   0 alex      (1000) alex      (1000)      190 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Maseru
--rw-r--r--   0 alex      (1000) alex      (1000)      190 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Mbabane
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Mogadishu
--rw-r--r--   0 alex      (1000) alex      (1000)      164 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Monrovia
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Nairobi
--rw-r--r--   0 alex      (1000) alex      (1000)      160 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Ndjamena
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Niamey
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Nouakchott
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Ouagadougou
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Porto-Novo
--rw-r--r--   0 alex      (1000) alex      (1000)      173 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Sao_Tome
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Timbuktu
--rw-r--r--   0 alex      (1000) alex      (1000)      431 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Tripoli
--rw-r--r--   0 alex      (1000) alex      (1000)      449 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Tunis
--rw-r--r--   0 alex      (1000) alex      (1000)      638 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Africa/Windhoek
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.290822 ora-0.8.0/python/ora/zoneinfo/America/
--rw-r--r--   0 alex      (1000) alex      (1000)      969 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Adak
--rw-r--r--   0 alex      (1000) alex      (1000)      977 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Anchorage
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Anguilla
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Antigua
--rw-r--r--   0 alex      (1000) alex      (1000)      592 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Araguaina
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Aruba
--rw-r--r--   0 alex      (1000) alex      (1000)      884 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Asuncion
--rw-r--r--   0 alex      (1000) alex      (1000)      149 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Atikokan
--rw-r--r--   0 alex      (1000) alex      (1000)      969 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Atka
--rw-r--r--   0 alex      (1000) alex      (1000)      682 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Bahia
--rw-r--r--   0 alex      (1000) alex      (1000)      728 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Bahia_Banderas
--rw-r--r--   0 alex      (1000) alex      (1000)      278 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Barbados
--rw-r--r--   0 alex      (1000) alex      (1000)      394 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Belem
--rw-r--r--   0 alex      (1000) alex      (1000)     1045 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Belize
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Blanc-Sablon
--rw-r--r--   0 alex      (1000) alex      (1000)      430 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Boa_Vista
--rw-r--r--   0 alex      (1000) alex      (1000)      179 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Bogota
--rw-r--r--   0 alex      (1000) alex      (1000)      999 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Boise
--rw-r--r--   0 alex      (1000) alex      (1000)      708 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Buenos_Aires
--rw-r--r--   0 alex      (1000) alex      (1000)      883 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Cambridge_Bay
--rw-r--r--   0 alex      (1000) alex      (1000)      952 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Campo_Grande
--rw-r--r--   0 alex      (1000) alex      (1000)      529 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Cancun
--rw-r--r--   0 alex      (1000) alex      (1000)      190 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Caracas
--rw-r--r--   0 alex      (1000) alex      (1000)      708 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Catamarca
--rw-r--r--   0 alex      (1000) alex      (1000)      151 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Cayenne
--rw-r--r--   0 alex      (1000) alex      (1000)      149 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Cayman
--rw-r--r--   0 alex      (1000) alex      (1000)     1754 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Chicago
--rw-r--r--   0 alex      (1000) alex      (1000)      691 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Chihuahua
--rw-r--r--   0 alex      (1000) alex      (1000)      718 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Ciudad_Juarez
--rw-r--r--   0 alex      (1000) alex      (1000)      149 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Coral_Harbour
--rw-r--r--   0 alex      (1000) alex      (1000)      708 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Cordoba
--rw-r--r--   0 alex      (1000) alex      (1000)      232 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Costa_Rica
--rw-r--r--   0 alex      (1000) alex      (1000)      240 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Creston
--rw-r--r--   0 alex      (1000) alex      (1000)      934 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Cuiaba
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Curacao
--rw-r--r--   0 alex      (1000) alex      (1000)      447 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Danmarkshavn
--rw-r--r--   0 alex      (1000) alex      (1000)     1029 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Dawson
--rw-r--r--   0 alex      (1000) alex      (1000)      683 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Dawson_Creek
--rw-r--r--   0 alex      (1000) alex      (1000)     1042 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Denver
--rw-r--r--   0 alex      (1000) alex      (1000)      899 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Detroit
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Dominica
--rw-r--r--   0 alex      (1000) alex      (1000)      970 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Edmonton
--rw-r--r--   0 alex      (1000) alex      (1000)      436 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Eirunepe
--rw-r--r--   0 alex      (1000) alex      (1000)      176 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/El_Salvador
--rw-r--r--   0 alex      (1000) alex      (1000)     1025 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Ensenada
--rw-r--r--   0 alex      (1000) alex      (1000)     1448 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Fort_Nelson
--rw-r--r--   0 alex      (1000) alex      (1000)      531 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Fort_Wayne
--rw-r--r--   0 alex      (1000) alex      (1000)      484 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Fortaleza
--rw-r--r--   0 alex      (1000) alex      (1000)      880 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Glace_Bay
--rw-r--r--   0 alex      (1000) alex      (1000)      931 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Godthab
--rw-r--r--   0 alex      (1000) alex      (1000)     1580 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Goose_Bay
--rw-r--r--   0 alex      (1000) alex      (1000)      853 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Grand_Turk
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Grenada
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Guadeloupe
--rw-r--r--   0 alex      (1000) alex      (1000)      212 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Guatemala
--rw-r--r--   0 alex      (1000) alex      (1000)      179 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Guayaquil
--rw-r--r--   0 alex      (1000) alex      (1000)      181 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Guyana
--rw-r--r--   0 alex      (1000) alex      (1000)     1672 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Halifax
--rw-r--r--   0 alex      (1000) alex      (1000)     1117 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Havana
--rw-r--r--   0 alex      (1000) alex      (1000)      286 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Hermosillo
--rw-r--r--   0 alex      (1000) alex      (1000)      531 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Indianapolis
--rw-r--r--   0 alex      (1000) alex      (1000)      817 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Inuvik
--rw-r--r--   0 alex      (1000) alex      (1000)      855 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Iqaluit
--rw-r--r--   0 alex      (1000) alex      (1000)      339 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Jamaica
--rw-r--r--   0 alex      (1000) alex      (1000)      690 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Jujuy
--rw-r--r--   0 alex      (1000) alex      (1000)      966 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Juneau
--rw-r--r--   0 alex      (1000) alex      (1000)     1016 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Knox_IN
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Kralendijk
--rw-r--r--   0 alex      (1000) alex      (1000)      170 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/La_Paz
--rw-r--r--   0 alex      (1000) alex      (1000)      283 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Lima
--rw-r--r--   0 alex      (1000) alex      (1000)     1294 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Los_Angeles
--rw-r--r--   0 alex      (1000) alex      (1000)     1242 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Louisville
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Lower_Princes
--rw-r--r--   0 alex      (1000) alex      (1000)      502 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Maceio
--rw-r--r--   0 alex      (1000) alex      (1000)      295 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Managua
--rw-r--r--   0 alex      (1000) alex      (1000)      412 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Manaus
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Marigot
--rw-r--r--   0 alex      (1000) alex      (1000)      178 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Martinique
--rw-r--r--   0 alex      (1000) alex      (1000)      437 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Matamoros
--rw-r--r--   0 alex      (1000) alex      (1000)      718 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Mazatlan
--rw-r--r--   0 alex      (1000) alex      (1000)      708 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Mendoza
--rw-r--r--   0 alex      (1000) alex      (1000)      917 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Menominee
--rw-r--r--   0 alex      (1000) alex      (1000)      654 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Merida
--rw-r--r--   0 alex      (1000) alex      (1000)      595 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Metlakatla
--rw-r--r--   0 alex      (1000) alex      (1000)      773 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Mexico_City
--rw-r--r--   0 alex      (1000) alex      (1000)      550 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Miquelon
--rw-r--r--   0 alex      (1000) alex      (1000)     1493 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Moncton
--rw-r--r--   0 alex      (1000) alex      (1000)      644 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Monterrey
--rw-r--r--   0 alex      (1000) alex      (1000)      969 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Montevideo
--rw-r--r--   0 alex      (1000) alex      (1000)     1717 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Montreal
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Montserrat
--rw-r--r--   0 alex      (1000) alex      (1000)     1717 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Nassau
--rw-r--r--   0 alex      (1000) alex      (1000)     1744 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/New_York
--rw-r--r--   0 alex      (1000) alex      (1000)     1717 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Nipigon
--rw-r--r--   0 alex      (1000) alex      (1000)      975 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Nome
--rw-r--r--   0 alex      (1000) alex      (1000)      484 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Noronha
--rw-r--r--   0 alex      (1000) alex      (1000)      931 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Nuuk
--rw-r--r--   0 alex      (1000) alex      (1000)      709 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Ojinaga
--rw-r--r--   0 alex      (1000) alex      (1000)      149 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Panama
--rw-r--r--   0 alex      (1000) alex      (1000)      855 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Pangnirtung
--rw-r--r--   0 alex      (1000) alex      (1000)      187 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Paramaribo
--rw-r--r--   0 alex      (1000) alex      (1000)      240 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Phoenix
--rw-r--r--   0 alex      (1000) alex      (1000)      565 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Port-au-Prince
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Port_of_Spain
--rw-r--r--   0 alex      (1000) alex      (1000)      418 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Porto_Acre
--rw-r--r--   0 alex      (1000) alex      (1000)      394 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Porto_Velho
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Puerto_Rico
--rw-r--r--   0 alex      (1000) alex      (1000)     1218 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Punta_Arenas
--rw-r--r--   0 alex      (1000) alex      (1000)     1294 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Rainy_River
--rw-r--r--   0 alex      (1000) alex      (1000)      807 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Rankin_Inlet
--rw-r--r--   0 alex      (1000) alex      (1000)      484 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Recife
--rw-r--r--   0 alex      (1000) alex      (1000)      638 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Regina
--rw-r--r--   0 alex      (1000) alex      (1000)      807 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Resolute
--rw-r--r--   0 alex      (1000) alex      (1000)      418 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Rio_Branco
--rw-r--r--   0 alex      (1000) alex      (1000)      708 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Rosario
--rw-r--r--   0 alex      (1000) alex      (1000)     1025 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Santa_Isabel
--rw-r--r--   0 alex      (1000) alex      (1000)      409 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Santarem
--rw-r--r--   0 alex      (1000) alex      (1000)     1354 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Santiago
--rw-r--r--   0 alex      (1000) alex      (1000)      317 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Santo_Domingo
--rw-r--r--   0 alex      (1000) alex      (1000)      952 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Sao_Paulo
--rw-r--r--   0 alex      (1000) alex      (1000)      479 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Scoresbysund
--rw-r--r--   0 alex      (1000) alex      (1000)     1042 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Shiprock
--rw-r--r--   0 alex      (1000) alex      (1000)      956 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Sitka
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/St_Barthelemy
--rw-r--r--   0 alex      (1000) alex      (1000)     1878 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/St_Johns
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/St_Kitts
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/St_Lucia
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/St_Thomas
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/St_Vincent
--rw-r--r--   0 alex      (1000) alex      (1000)      368 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Swift_Current
--rw-r--r--   0 alex      (1000) alex      (1000)      194 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Tegucigalpa
--rw-r--r--   0 alex      (1000) alex      (1000)      455 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Thule
--rw-r--r--   0 alex      (1000) alex      (1000)     1717 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Thunder_Bay
--rw-r--r--   0 alex      (1000) alex      (1000)     1025 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Tijuana
--rw-r--r--   0 alex      (1000) alex      (1000)     1717 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Toronto
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Tortola
--rw-r--r--   0 alex      (1000) alex      (1000)     1330 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Vancouver
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Virgin
--rw-r--r--   0 alex      (1000) alex      (1000)     1029 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Whitehorse
--rw-r--r--   0 alex      (1000) alex      (1000)     1294 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Winnipeg
--rw-r--r--   0 alex      (1000) alex      (1000)      946 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/America/Yakutat
--rw-r--r--   0 alex      (1000) alex      (1000)      844 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/America/Yellowknife
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.290822 ora-0.8.0/python/ora/zoneinfo/Antarctica/
--rw-r--r--   0 alex      (1000) alex      (1000)      243 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/Casey
--rw-r--r--   0 alex      (1000) alex      (1000)      197 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/Davis
--rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/DumontDUrville
--rw-r--r--   0 alex      (1000) alex      (1000)      976 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/Macquarie
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/Mawson
--rw-r--r--   0 alex      (1000) alex      (1000)     1043 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/McMurdo
--rw-r--r--   0 alex      (1000) alex      (1000)      887 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/Palmer
--rw-r--r--   0 alex      (1000) alex      (1000)      132 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/Rothera
--rw-r--r--   0 alex      (1000) alex      (1000)     1043 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/South_Pole
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/Syowa
--rw-r--r--   0 alex      (1000) alex      (1000)      177 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/Troll
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Antarctica/Vostok
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.290822 ora-0.8.0/python/ora/zoneinfo/Arctic/
--rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Arctic/Longyearbyen
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.297489 ora-0.8.0/python/ora/zoneinfo/Asia/
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Aden
--rw-r--r--   0 alex      (1000) alex      (1000)      609 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Almaty
--rw-r--r--   0 alex      (1000) alex      (1000)      928 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Amman
--rw-r--r--   0 alex      (1000) alex      (1000)      743 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Anadyr
--rw-r--r--   0 alex      (1000) alex      (1000)      606 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Aqtau
--rw-r--r--   0 alex      (1000) alex      (1000)      615 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Aqtobe
--rw-r--r--   0 alex      (1000) alex      (1000)      375 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Ashgabat
--rw-r--r--   0 alex      (1000) alex      (1000)      375 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Ashkhabad
--rw-r--r--   0 alex      (1000) alex      (1000)      616 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Atyrau
--rw-r--r--   0 alex      (1000) alex      (1000)      630 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Baghdad
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Bahrain
--rw-r--r--   0 alex      (1000) alex      (1000)      744 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Baku
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Bangkok
--rw-r--r--   0 alex      (1000) alex      (1000)      753 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Barnaul
--rw-r--r--   0 alex      (1000) alex      (1000)      732 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Beirut
--rw-r--r--   0 alex      (1000) alex      (1000)      618 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Bishkek
--rw-r--r--   0 alex      (1000) alex      (1000)      320 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Brunei
--rw-r--r--   0 alex      (1000) alex      (1000)      220 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Calcutta
--rw-r--r--   0 alex      (1000) alex      (1000)      750 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Chita
--rw-r--r--   0 alex      (1000) alex      (1000)      619 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Choibalsan
--rw-r--r--   0 alex      (1000) alex      (1000)      393 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Chongqing
--rw-r--r--   0 alex      (1000) alex      (1000)      393 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Chungking
--rw-r--r--   0 alex      (1000) alex      (1000)      247 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Colombo
--rw-r--r--   0 alex      (1000) alex      (1000)      231 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Dacca
--rw-r--r--   0 alex      (1000) alex      (1000)     1234 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Damascus
--rw-r--r--   0 alex      (1000) alex      (1000)      231 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Dhaka
--rw-r--r--   0 alex      (1000) alex      (1000)      170 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Dili
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Dubai
--rw-r--r--   0 alex      (1000) alex      (1000)      366 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Dushanbe
--rw-r--r--   0 alex      (1000) alex      (1000)      940 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Famagusta
--rw-r--r--   0 alex      (1000) alex      (1000)     1258 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Gaza
--rw-r--r--   0 alex      (1000) alex      (1000)      393 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Harbin
--rw-r--r--   0 alex      (1000) alex      (1000)     1276 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Hebron
--rw-r--r--   0 alex      (1000) alex      (1000)      236 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Ho_Chi_Minh
--rw-r--r--   0 alex      (1000) alex      (1000)      775 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Hong_Kong
--rw-r--r--   0 alex      (1000) alex      (1000)      594 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Hovd
--rw-r--r--   0 alex      (1000) alex      (1000)      760 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Irkutsk
--rw-r--r--   0 alex      (1000) alex      (1000)     1200 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Istanbul
--rw-r--r--   0 alex      (1000) alex      (1000)      248 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Jakarta
--rw-r--r--   0 alex      (1000) alex      (1000)      171 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Jayapura
--rw-r--r--   0 alex      (1000) alex      (1000)     1074 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Jerusalem
--rw-r--r--   0 alex      (1000) alex      (1000)      159 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Kabul
--rw-r--r--   0 alex      (1000) alex      (1000)      727 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Kamchatka
--rw-r--r--   0 alex      (1000) alex      (1000)      266 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Karachi
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Kashgar
--rw-r--r--   0 alex      (1000) alex      (1000)      161 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Kathmandu
--rw-r--r--   0 alex      (1000) alex      (1000)      161 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Katmandu
--rw-r--r--   0 alex      (1000) alex      (1000)      775 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Khandyga
--rw-r--r--   0 alex      (1000) alex      (1000)      220 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Kolkata
--rw-r--r--   0 alex      (1000) alex      (1000)      741 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Krasnoyarsk
--rw-r--r--   0 alex      (1000) alex      (1000)      256 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Kuala_Lumpur
--rw-r--r--   0 alex      (1000) alex      (1000)      320 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Kuching
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Kuwait
--rw-r--r--   0 alex      (1000) alex      (1000)      791 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Macao
--rw-r--r--   0 alex      (1000) alex      (1000)      791 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Macau
--rw-r--r--   0 alex      (1000) alex      (1000)      751 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Magadan
--rw-r--r--   0 alex      (1000) alex      (1000)      190 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Makassar
--rw-r--r--   0 alex      (1000) alex      (1000)      238 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Manila
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Muscat
--rw-r--r--   0 alex      (1000) alex      (1000)      597 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Nicosia
--rw-r--r--   0 alex      (1000) alex      (1000)      726 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Novokuznetsk
--rw-r--r--   0 alex      (1000) alex      (1000)      753 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Novosibirsk
--rw-r--r--   0 alex      (1000) alex      (1000)      741 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Omsk
--rw-r--r--   0 alex      (1000) alex      (1000)      625 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Oral
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Phnom_Penh
--rw-r--r--   0 alex      (1000) alex      (1000)      247 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Pontianak
--rw-r--r--   0 alex      (1000) alex      (1000)      183 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Pyongyang
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Qatar
--rw-r--r--   0 alex      (1000) alex      (1000)      615 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Qostanay
--rw-r--r--   0 alex      (1000) alex      (1000)      624 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Qyzylorda
--rw-r--r--   0 alex      (1000) alex      (1000)      187 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Rangoon
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Riyadh
--rw-r--r--   0 alex      (1000) alex      (1000)      236 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Saigon
--rw-r--r--   0 alex      (1000) alex      (1000)      755 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Sakhalin
--rw-r--r--   0 alex      (1000) alex      (1000)      366 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Samarkand
--rw-r--r--   0 alex      (1000) alex      (1000)      415 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Seoul
--rw-r--r--   0 alex      (1000) alex      (1000)      393 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Shanghai
--rw-r--r--   0 alex      (1000) alex      (1000)      256 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Singapore
--rw-r--r--   0 alex      (1000) alex      (1000)      742 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Srednekolymsk
--rw-r--r--   0 alex      (1000) alex      (1000)      511 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Taipei
--rw-r--r--   0 alex      (1000) alex      (1000)      366 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Tashkent
--rw-r--r--   0 alex      (1000) alex      (1000)      629 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Tbilisi
--rw-r--r--   0 alex      (1000) alex      (1000)      812 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Tehran
--rw-r--r--   0 alex      (1000) alex      (1000)     1074 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Tel_Aviv
--rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Thimbu
--rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Thimphu
--rw-r--r--   0 alex      (1000) alex      (1000)      213 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Tokyo
--rw-r--r--   0 alex      (1000) alex      (1000)      753 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Tomsk
--rw-r--r--   0 alex      (1000) alex      (1000)      190 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Ujung_Pandang
--rw-r--r--   0 alex      (1000) alex      (1000)      594 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Ulaanbaatar
--rw-r--r--   0 alex      (1000) alex      (1000)      594 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Ulan_Bator
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Urumqi
--rw-r--r--   0 alex      (1000) alex      (1000)      771 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Ust-Nera
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Vientiane
--rw-r--r--   0 alex      (1000) alex      (1000)      742 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Vladivostok
--rw-r--r--   0 alex      (1000) alex      (1000)      741 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Yakutsk
--rw-r--r--   0 alex      (1000) alex      (1000)      187 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Yangon
--rw-r--r--   0 alex      (1000) alex      (1000)      760 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Yekaterinburg
--rw-r--r--   0 alex      (1000) alex      (1000)      708 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Asia/Yerevan
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.297489 ora-0.8.0/python/ora/zoneinfo/Atlantic/
--rw-r--r--   0 alex      (1000) alex      (1000)     1453 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Azores
--rw-r--r--   0 alex      (1000) alex      (1000)     1024 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Bermuda
--rw-r--r--   0 alex      (1000) alex      (1000)      478 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Canary
--rw-r--r--   0 alex      (1000) alex      (1000)      175 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Cape_Verde
--rw-r--r--   0 alex      (1000) alex      (1000)      441 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Faeroe
--rw-r--r--   0 alex      (1000) alex      (1000)      441 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Faroe
--rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Jan_Mayen
--rw-r--r--   0 alex      (1000) alex      (1000)     1453 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Madeira
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Reykjavik
--rw-r--r--   0 alex      (1000) alex      (1000)      132 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/South_Georgia
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/St_Helena
--rw-r--r--   0 alex      (1000) alex      (1000)      789 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Atlantic/Stanley
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.300822 ora-0.8.0/python/ora/zoneinfo/Australia/
--rw-r--r--   0 alex      (1000) alex      (1000)      904 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/ACT
--rw-r--r--   0 alex      (1000) alex      (1000)      921 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Adelaide
--rw-r--r--   0 alex      (1000) alex      (1000)      289 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Brisbane
--rw-r--r--   0 alex      (1000) alex      (1000)      941 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Broken_Hill
--rw-r--r--   0 alex      (1000) alex      (1000)      904 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Canberra
--rw-r--r--   0 alex      (1000) alex      (1000)     1003 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Currie
--rw-r--r--   0 alex      (1000) alex      (1000)      234 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Darwin
--rw-r--r--   0 alex      (1000) alex      (1000)      314 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Eucla
--rw-r--r--   0 alex      (1000) alex      (1000)     1003 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Hobart
--rw-r--r--   0 alex      (1000) alex      (1000)      692 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/LHI
--rw-r--r--   0 alex      (1000) alex      (1000)      325 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Lindeman
--rw-r--r--   0 alex      (1000) alex      (1000)      692 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Lord_Howe
--rw-r--r--   0 alex      (1000) alex      (1000)      904 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Melbourne
--rw-r--r--   0 alex      (1000) alex      (1000)      904 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/NSW
--rw-r--r--   0 alex      (1000) alex      (1000)      234 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/North
--rw-r--r--   0 alex      (1000) alex      (1000)      306 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Perth
--rw-r--r--   0 alex      (1000) alex      (1000)      289 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Queensland
--rw-r--r--   0 alex      (1000) alex      (1000)      921 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/South
--rw-r--r--   0 alex      (1000) alex      (1000)      904 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Sydney
--rw-r--r--   0 alex      (1000) alex      (1000)     1003 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Tasmania
--rw-r--r--   0 alex      (1000) alex      (1000)      904 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Victoria
--rw-r--r--   0 alex      (1000) alex      (1000)      306 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/West
--rw-r--r--   0 alex      (1000) alex      (1000)      941 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Australia/Yancowinna
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.300822 ora-0.8.0/python/ora/zoneinfo/Brazil/
--rw-r--r--   0 alex      (1000) alex      (1000)      418 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Brazil/Acre
--rw-r--r--   0 alex      (1000) alex      (1000)      484 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Brazil/DeNoronha
--rw-r--r--   0 alex      (1000) alex      (1000)      952 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Brazil/East
--rw-r--r--   0 alex      (1000) alex      (1000)      412 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Brazil/West
--rw-r--r--   0 alex      (1000) alex      (1000)      621 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/CET
--rw-r--r--   0 alex      (1000) alex      (1000)      951 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/CST6CDT
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.300822 ora-0.8.0/python/ora/zoneinfo/Canada/
--rw-r--r--   0 alex      (1000) alex      (1000)     1672 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Canada/Atlantic
--rw-r--r--   0 alex      (1000) alex      (1000)     1294 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Canada/Central
--rw-r--r--   0 alex      (1000) alex      (1000)     1717 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Canada/Eastern
--rw-r--r--   0 alex      (1000) alex      (1000)      970 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Canada/Mountain
--rw-r--r--   0 alex      (1000) alex      (1000)     1878 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Canada/Newfoundland
--rw-r--r--   0 alex      (1000) alex      (1000)     1330 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Canada/Pacific
--rw-r--r--   0 alex      (1000) alex      (1000)      638 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Canada/Saskatchewan
--rw-r--r--   0 alex      (1000) alex      (1000)     1029 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Canada/Yukon
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.300822 ora-0.8.0/python/ora/zoneinfo/Chile/
--rw-r--r--   0 alex      (1000) alex      (1000)     1354 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Chile/Continental
--rw-r--r--   0 alex      (1000) alex      (1000)     1174 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Chile/EasterIsland
--rw-r--r--   0 alex      (1000) alex      (1000)     1117 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Cuba
--rw-r--r--   0 alex      (1000) alex      (1000)      497 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/EET
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/EST
--rw-r--r--   0 alex      (1000) alex      (1000)      951 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/EST5EDT
--rw-r--r--   0 alex      (1000) alex      (1000)     1276 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Egypt
--rw-r--r--   0 alex      (1000) alex      (1000)     1496 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Eire
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.304155 ora-0.8.0/python/ora/zoneinfo/Etc/
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+0
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+1
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+10
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+11
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+12
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+2
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+3
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+4
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+5
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+6
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+7
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+8
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT+9
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-0
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-1
--rw-r--r--   0 alex      (1000) alex      (1000)      115 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-10
--rw-r--r--   0 alex      (1000) alex      (1000)      115 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-11
--rw-r--r--   0 alex      (1000) alex      (1000)      115 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-12
--rw-r--r--   0 alex      (1000) alex      (1000)      115 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-13
--rw-r--r--   0 alex      (1000) alex      (1000)      115 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-14
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-2
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-3
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-4
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-5
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-6
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-7
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-8
--rw-r--r--   0 alex      (1000) alex      (1000)      114 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT-9
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/GMT0
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/Greenwich
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/UCT
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/UTC
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/Universal
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Etc/Zulu
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.307489 ora-0.8.0/python/ora/zoneinfo/Europe/
--rw-r--r--   0 alex      (1000) alex      (1000)     1103 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Amsterdam
--rw-r--r--   0 alex      (1000) alex      (1000)      389 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Andorra
--rw-r--r--   0 alex      (1000) alex      (1000)      726 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Astrakhan
--rw-r--r--   0 alex      (1000) alex      (1000)      682 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Athens
--rw-r--r--   0 alex      (1000) alex      (1000)     1599 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Belfast
--rw-r--r--   0 alex      (1000) alex      (1000)      478 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Belgrade
--rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Berlin
--rw-r--r--   0 alex      (1000) alex      (1000)      723 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Bratislava
--rw-r--r--   0 alex      (1000) alex      (1000)     1103 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Brussels
--rw-r--r--   0 alex      (1000) alex      (1000)      661 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Bucharest
--rw-r--r--   0 alex      (1000) alex      (1000)      766 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Budapest
--rw-r--r--   0 alex      (1000) alex      (1000)      497 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Busingen
--rw-r--r--   0 alex      (1000) alex      (1000)      755 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Chisinau
--rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Copenhagen
--rw-r--r--   0 alex      (1000) alex      (1000)     1496 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Dublin
--rw-r--r--   0 alex      (1000) alex      (1000)     1220 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Gibraltar
--rw-r--r--   0 alex      (1000) alex      (1000)     1599 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Guernsey
--rw-r--r--   0 alex      (1000) alex      (1000)      481 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Helsinki
--rw-r--r--   0 alex      (1000) alex      (1000)     1599 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Isle_of_Man
--rw-r--r--   0 alex      (1000) alex      (1000)     1200 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Istanbul
--rw-r--r--   0 alex      (1000) alex      (1000)     1599 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Jersey
--rw-r--r--   0 alex      (1000) alex      (1000)      904 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Kaliningrad
--rw-r--r--   0 alex      (1000) alex      (1000)      558 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Kiev
--rw-r--r--   0 alex      (1000) alex      (1000)      717 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Kirov
--rw-r--r--   0 alex      (1000) alex      (1000)      558 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Kyiv
--rw-r--r--   0 alex      (1000) alex      (1000)     1454 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Lisbon
--rw-r--r--   0 alex      (1000) alex      (1000)      478 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Ljubljana
--rw-r--r--   0 alex      (1000) alex      (1000)     1599 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/London
--rw-r--r--   0 alex      (1000) alex      (1000)     1103 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Luxembourg
--rw-r--r--   0 alex      (1000) alex      (1000)      897 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Madrid
--rw-r--r--   0 alex      (1000) alex      (1000)      928 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Malta
--rw-r--r--   0 alex      (1000) alex      (1000)      481 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Mariehamn
--rw-r--r--   0 alex      (1000) alex      (1000)      808 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Minsk
--rw-r--r--   0 alex      (1000) alex      (1000)     1105 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Monaco
--rw-r--r--   0 alex      (1000) alex      (1000)      908 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Moscow
--rw-r--r--   0 alex      (1000) alex      (1000)      597 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Nicosia
--rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Oslo
--rw-r--r--   0 alex      (1000) alex      (1000)     1105 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Paris
--rw-r--r--   0 alex      (1000) alex      (1000)      478 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Podgorica
--rw-r--r--   0 alex      (1000) alex      (1000)      723 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Prague
--rw-r--r--   0 alex      (1000) alex      (1000)      694 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Riga
--rw-r--r--   0 alex      (1000) alex      (1000)      947 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Rome
--rw-r--r--   0 alex      (1000) alex      (1000)      732 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Samara
--rw-r--r--   0 alex      (1000) alex      (1000)      947 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/San_Marino
--rw-r--r--   0 alex      (1000) alex      (1000)      478 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Sarajevo
--rw-r--r--   0 alex      (1000) alex      (1000)      726 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Saratov
--rw-r--r--   0 alex      (1000) alex      (1000)      865 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Simferopol
--rw-r--r--   0 alex      (1000) alex      (1000)      478 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Skopje
--rw-r--r--   0 alex      (1000) alex      (1000)      592 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Sofia
--rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Stockholm
--rw-r--r--   0 alex      (1000) alex      (1000)      675 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Tallinn
--rw-r--r--   0 alex      (1000) alex      (1000)      604 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Tirane
--rw-r--r--   0 alex      (1000) alex      (1000)      755 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Tiraspol
--rw-r--r--   0 alex      (1000) alex      (1000)      760 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Ulyanovsk
--rw-r--r--   0 alex      (1000) alex      (1000)      558 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Uzhgorod
--rw-r--r--   0 alex      (1000) alex      (1000)      497 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Vaduz
--rw-r--r--   0 alex      (1000) alex      (1000)      947 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Vatican
--rw-r--r--   0 alex      (1000) alex      (1000)      658 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Vienna
--rw-r--r--   0 alex      (1000) alex      (1000)      676 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Vilnius
--rw-r--r--   0 alex      (1000) alex      (1000)      735 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Volgograd
--rw-r--r--   0 alex      (1000) alex      (1000)      923 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Warsaw
--rw-r--r--   0 alex      (1000) alex      (1000)      478 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Zagreb
--rw-r--r--   0 alex      (1000) alex      (1000)      558 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Zaporozhye
--rw-r--r--   0 alex      (1000) alex      (1000)      497 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Europe/Zurich
--rw-r--r--   0 alex      (1000) alex      (1000)      113 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Factory
--rw-r--r--   0 alex      (1000) alex      (1000)     1599 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/GB
--rw-r--r--   0 alex      (1000) alex      (1000)     1599 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/GB-Eire
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/GMT
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/GMT+0
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/GMT-0
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/GMT0
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Greenwich
--rw-r--r--   0 alex      (1000) alex      (1000)      112 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/HST
--rw-r--r--   0 alex      (1000) alex      (1000)      775 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Hongkong
--rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Iceland
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.307489 ora-0.8.0/python/ora/zoneinfo/Indian/
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Antananarivo
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Chagos
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Christmas
--rw-r--r--   0 alex      (1000) alex      (1000)      187 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Cocos
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Comoro
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Kerguelen
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Mahe
--rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Maldives
--rw-r--r--   0 alex      (1000) alex      (1000)      179 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Mauritius
--rw-r--r--   0 alex      (1000) alex      (1000)      191 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Mayotte
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Indian/Reunion
--rw-r--r--   0 alex      (1000) alex      (1000)      812 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Iran
--rw-r--r--   0 alex      (1000) alex      (1000)     1074 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Israel
--rw-r--r--   0 alex      (1000) alex      (1000)      339 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Jamaica
--rw-r--r--   0 alex      (1000) alex      (1000)      213 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Japan
--rw-r--r--   0 alex      (1000) alex      (1000)      219 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Kwajalein
--rw-r--r--   0 alex      (1000) alex      (1000)      431 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Libya
--rw-r--r--   0 alex      (1000) alex      (1000)      621 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/MET
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/MST
--rw-r--r--   0 alex      (1000) alex      (1000)      951 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/MST7MDT
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.307489 ora-0.8.0/python/ora/zoneinfo/Mexico/
--rw-r--r--   0 alex      (1000) alex      (1000)     1025 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Mexico/BajaNorte
--rw-r--r--   0 alex      (1000) alex      (1000)      718 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Mexico/BajaSur
--rw-r--r--   0 alex      (1000) alex      (1000)      773 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Mexico/General
--rw-r--r--   0 alex      (1000) alex      (1000)     1043 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/NZ
--rw-r--r--   0 alex      (1000) alex      (1000)      808 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/NZ-CHAT
--rw-r--r--   0 alex      (1000) alex      (1000)     1042 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Navajo
--rw-r--r--   0 alex      (1000) alex      (1000)      393 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/PRC
--rw-r--r--   0 alex      (1000) alex      (1000)      951 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/PST8PDT
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.310822 ora-0.8.0/python/ora/zoneinfo/Pacific/
--rw-r--r--   0 alex      (1000) alex      (1000)      407 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Apia
--rw-r--r--   0 alex      (1000) alex      (1000)     1043 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Auckland
--rw-r--r--   0 alex      (1000) alex      (1000)      201 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Bougainville
--rw-r--r--   0 alex      (1000) alex      (1000)      808 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Chatham
--rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Chuuk
--rw-r--r--   0 alex      (1000) alex      (1000)     1174 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Easter
--rw-r--r--   0 alex      (1000) alex      (1000)      342 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Efate
--rw-r--r--   0 alex      (1000) alex      (1000)      172 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Enderbury
--rw-r--r--   0 alex      (1000) alex      (1000)      153 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Fakaofo
--rw-r--r--   0 alex      (1000) alex      (1000)      396 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Fiji
--rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Funafuti
--rw-r--r--   0 alex      (1000) alex      (1000)      175 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Galapagos
--rw-r--r--   0 alex      (1000) alex      (1000)      132 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Gambier
--rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Guadalcanal
--rw-r--r--   0 alex      (1000) alex      (1000)      350 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Guam
--rw-r--r--   0 alex      (1000) alex      (1000)      221 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Honolulu
--rw-r--r--   0 alex      (1000) alex      (1000)      221 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Johnston
--rw-r--r--   0 alex      (1000) alex      (1000)      172 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Kanton
--rw-r--r--   0 alex      (1000) alex      (1000)      174 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Kiritimati
--rw-r--r--   0 alex      (1000) alex      (1000)      242 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Kosrae
--rw-r--r--   0 alex      (1000) alex      (1000)      219 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Kwajalein
--rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Majuro
--rw-r--r--   0 alex      (1000) alex      (1000)      139 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Marquesas
--rw-r--r--   0 alex      (1000) alex      (1000)      146 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Midway
--rw-r--r--   0 alex      (1000) alex      (1000)      183 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Nauru
--rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Niue
--rw-r--r--   0 alex      (1000) alex      (1000)      247 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Norfolk
--rw-r--r--   0 alex      (1000) alex      (1000)      198 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Noumea
--rw-r--r--   0 alex      (1000) alex      (1000)      146 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Pago_Pago
--rw-r--r--   0 alex      (1000) alex      (1000)      148 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Palau
--rw-r--r--   0 alex      (1000) alex      (1000)      153 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Pitcairn
--rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Pohnpei
--rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Ponape
--rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Port_Moresby
--rw-r--r--   0 alex      (1000) alex      (1000)      406 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Rarotonga
--rw-r--r--   0 alex      (1000) alex      (1000)      350 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Saipan
--rw-r--r--   0 alex      (1000) alex      (1000)      146 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Samoa
--rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Tahiti
--rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Tarawa
--rw-r--r--   0 alex      (1000) alex      (1000)      237 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Tongatapu
--rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Truk
--rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Wake
--rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Wallis
--rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Pacific/Yap
--rw-r--r--   0 alex      (1000) alex      (1000)      923 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Poland
--rw-r--r--   0 alex      (1000) alex      (1000)     1454 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Portugal
--rw-r--r--   0 alex      (1000) alex      (1000)      511 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/ROC
--rw-r--r--   0 alex      (1000) alex      (1000)      415 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/ROK
--rw-r--r--   0 alex      (1000) alex      (1000)      256 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/Singapore
--rw-r--r--   0 alex      (1000) alex      (1000)     1200 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Turkey
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/UCT
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.314155 ora-0.8.0/python/ora/zoneinfo/US/
--rw-r--r--   0 alex      (1000) alex      (1000)      977 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Alaska
--rw-r--r--   0 alex      (1000) alex      (1000)      969 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Aleutian
--rw-r--r--   0 alex      (1000) alex      (1000)      240 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Arizona
--rw-r--r--   0 alex      (1000) alex      (1000)     1754 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Central
--rw-r--r--   0 alex      (1000) alex      (1000)      531 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/East-Indiana
--rw-r--r--   0 alex      (1000) alex      (1000)     1744 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Eastern
--rw-r--r--   0 alex      (1000) alex      (1000)      221 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Hawaii
--rw-r--r--   0 alex      (1000) alex      (1000)     1016 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Indiana-Starke
--rw-r--r--   0 alex      (1000) alex      (1000)      899 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Michigan
--rw-r--r--   0 alex      (1000) alex      (1000)     1042 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Mountain
--rw-r--r--   0 alex      (1000) alex      (1000)     1294 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Pacific
--rw-r--r--   0 alex      (1000) alex      (1000)      146 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/US/Samoa
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/UTC
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Universal
--rw-r--r--   0 alex      (1000) alex      (1000)      908 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/W-SU
--rw-r--r--   0 alex      (1000) alex      (1000)      494 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/WET
--rw-r--r--   0 alex      (1000) alex      (1000)      111 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/Zulu
--rw-r--r--   0 alex      (1000) alex      (1000)     4458 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/iso3166.tab
--rw-r--r--   0 alex      (1000) alex      (1000)     3388 2023-02-17 19:17:02.000000 ora-0.8.0/python/ora/zoneinfo/leapseconds
--rw-r--r--   0 alex      (1000) alex      (1000)   107242 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/tzdata.zi
--rw-r--r--   0 alex      (1000) alex      (1000)    18955 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/zone.tab
--rw-r--r--   0 alex      (1000) alex      (1000)    17609 2023-02-17 19:24:56.000000 ora-0.8.0/python/ora/zoneinfo/zone1970.tab
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-24 15:35:03.267488 ora-0.8.0/python/ora.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)      852 2023-02-24 15:35:03.000000 ora-0.8.0/python/ora.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    24486 2023-02-24 15:35:03.000000 ora-0.8.0/python/ora.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-02-24 15:35:03.000000 ora-0.8.0/python/ora.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        6 2023-02-24 15:35:03.000000 ora-0.8.0/python/ora.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        4 2023-02-24 15:35:03.000000 ora-0.8.0/python/ora.egg-info/top_level.txt
--rwxrwxr-x   0 alex      (1000) alex      (1000)      838 2016-11-21 03:23:59.000000 ora-0.8.0/python/wrap_docstrings
--rw-r--r--   0 alex      (1000) alex      (1000)      380 2023-02-24 15:35:03.314155 ora-0.8.0/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)     3318 2023-02-24 15:34:51.000000 ora-0.8.0/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.820986 ora-0.8.2/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1434 2022-04-21 13:40:08.000000 ora-0.8.2/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-04-21 13:40:08.000000 ora-0.8.2/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)     6981 2023-05-30 04:06:23.000000 ora-0.8.2/Makefile
+-rw-r--r--   0 alex      (1000) alex      (1000)      832 2023-05-30 04:08:17.820986 ora-0.8.2/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     1827 2023-05-30 04:06:23.000000 ora-0.8.2/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.704318 ora-0.8.2/cxx/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.704318 ora-0.8.2/cxx/include/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.707651 ora-0.8.2/cxx/include/ora/
+-rw-r--r--   0 alex      (1000) alex      (1000)     7624 2022-07-13 03:09:35.000000 ora-0.8.2/cxx/include/ora/calendar.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     7583 2022-07-13 03:09:35.000000 ora-0.8.2/cxx/include/ora/date_functions.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)    10045 2022-05-11 05:46:09.000000 ora-0.8.2/cxx/include/ora/date_math.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     8905 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/date_nex.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     8137 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/date_type.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     8138 2022-07-13 03:09:35.000000 ora-0.8.2/cxx/include/ora/daytime_functions.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     1220 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/daytime_math.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     8811 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/daytime_nex.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     7151 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/daytime_type.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     3024 2022-05-11 05:46:09.000000 ora-0.8.2/cxx/include/ora/exceptions.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     2221 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/ez.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)    12600 2023-05-30 04:06:23.000000 ora-0.8.2/cxx/include/ora/format.hh
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.707651 ora-0.8.2/cxx/include/ora/lib/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3233 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/lib/exc.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     1316 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/lib/file.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     5352 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/lib/filename.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)      573 2022-07-13 03:09:35.000000 ora-0.8.2/cxx/include/ora/lib/iter.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)    10062 2023-05-30 04:06:25.000000 ora-0.8.2/cxx/include/ora/lib/math.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     2266 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/lib/mem.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)      951 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/lib/num.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     2365 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/lib/string.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     2785 2023-05-30 04:06:23.000000 ora-0.8.2/cxx/include/ora/lib/string_builder.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     3913 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/lib/xsys.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     7378 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/localization.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)      988 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/localization_nex.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     3226 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/parse.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     2090 2022-05-11 05:46:09.000000 ora-0.8.2/cxx/include/ora/posixtz.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     5064 2022-07-13 03:09:35.000000 ora-0.8.2/cxx/include/ora/time_functions.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     1892 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/time_interval.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     6117 2022-05-11 20:39:51.000000 ora-0.8.2/cxx/include/ora/time_math.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     6204 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/time_nex.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)    11989 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/time_type.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     3951 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/time_zone.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)    11830 2022-05-11 05:46:09.000000 ora-0.8.2/cxx/include/ora/types.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     1189 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora/tzfile.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     1309 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/include/ora.hh
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.710985 ora-0.8.2/cxx/src/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.710985 ora-0.8.2/cxx/src/bin/
+-rw-r--r--   0 alex      (1000) alex      (1000)      546 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/bin/posixtz.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      483 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/bin/tzdump.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     3592 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/calendar.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      354 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/date.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     5020 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/date_math.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      426 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/daytime.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      919 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/daytime_math.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      995 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/file.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     4718 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/filename.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    17805 2023-05-30 04:06:25.000000 ora-0.8.2/cxx/src/format.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    16071 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/parse.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     4112 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/posixtz.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      553 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/time.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    14150 2022-05-11 05:46:09.000000 ora-0.8.2/cxx/src/time_zone.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     7410 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/src/tzfile.cc
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.714318 ora-0.8.2/cxx/test/
+-rw-r--r--   0 alex      (1000) alex      (1000)     5290 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/calendar.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     9191 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/date.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     2747 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/date_format.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    19480 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/date_functions.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     7364 2022-05-11 05:46:09.000000 ora-0.8.2/cxx/test/date_math.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    17118 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/date_nex.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     8658 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/daytime.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     2177 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/daytime_functions.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     8319 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/daytime_nex.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    13605 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/format.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1959 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/from_local.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      589 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/parse.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      842 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/posixtz.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1242 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/string_builder.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     8949 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/time.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      639 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/time128.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     2312 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/time_format.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1595 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/time_functions.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1463 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/time_interval.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     2567 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/time_nex.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1778 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/time_zone.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      862 2022-04-21 13:40:08.000000 ora-0.8.2/cxx/test/to_local.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      115 2022-07-13 03:09:35.000000 ora-0.8.2/pyproject.toml
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.717651 ora-0.8.2/python/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.717651 ora-0.8.2/python/ora/
+-rw-r--r--   0 alex      (1000) alex      (1000)     8174 2023-05-30 04:07:38.000000 ora-0.8.2/python/ora/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3936 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/calendar.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.717651 ora-0.8.2/python/ora/calendars/
+-rw-r--r--   0 alex      (1000) alex      (1000)    30395 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/calendars/usa-federal-businessdays.cal
+-rw-r--r--   0 alex      (1000) alex      (1000)     3115 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/calendars/usa-federal-holidays.cal
+-rw-r--r--   0 alex      (1000) alex      (1000)     1304 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/date.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1506 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/date_expr.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1141 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/daytime.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.720985 ora-0.8.2/python/ora/ext/
+-rw-r--r--   0 alex      (1000) alex      (1000)    15876 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/functions.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     5374 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/functions.docstrings
+-rw-r--r--   0 alex      (1000) alex      (1000)     5976 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/module.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      358 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/np.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    16039 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/np.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)      456 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/np_date.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)       83 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/np_date.docstrings
+-rw-r--r--   0 alex      (1000) alex      (1000)    18788 2022-07-13 03:09:35.000000 ora-0.8.2/python/ora/ext/np_date.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)      335 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/np_daytime.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    15106 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/np_daytime.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)    14660 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/np_functions.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      307 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/np_time.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    15414 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/np_time.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     1884 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/np_types.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1437 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/np_types.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)      527 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    42365 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/py.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     2086 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_cal_functions.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    14379 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_calendar.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1509 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_calendar.docstrings
+-rw-r--r--   0 alex      (1000) alex      (1000)     1902 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_calendar.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     4898 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_date.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     5158 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_date.docstrings
+-rw-r--r--   0 alex      (1000) alex      (1000)    36744 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/py_date.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     5601 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/py_date_fmt.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      709 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/py_date_fmt.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)      473 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_date_inst.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1188 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_daytime.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     3944 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_daytime.docstrings
+-rw-r--r--   0 alex      (1000) alex      (1000)    31799 2022-07-13 03:09:35.000000 ora-0.8.2/python/ora/ext/py_daytime.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)      554 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_daytime_inst.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    14739 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/py_local.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1392 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_local.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     2172 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_time.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1148 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_time.docstrings
+-rw-r--r--   0 alex      (1000) alex      (1000)    32458 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/py_time.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     6460 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/py_time_fmt.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     1001 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/py_time_fmt.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     3883 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_time_inst.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)    17861 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/ext/py_time_zone.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)     2823 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/py_time_zone.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     5531 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/ext/text.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     2244 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/types.cc
+-rw-r--r--   0 alex      (1000) alex      (1000)      280 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/types.docstrings
+-rw-r--r--   0 alex      (1000) alex      (1000)      440 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/types.hh
+-rw-r--r--   0 alex      (1000) alex      (1000)     2348 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/ext/util.hh
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.720985 ora-0.8.2/python/ora/np/
+-rw-r--r--   0 alex      (1000) alex      (1000)      776 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/np/__init__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.727652 ora-0.8.2/python/ora/test/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1028 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       89 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/june18.cal
+-rw-r--r--   0 alex      (1000) alex      (1000)     6973 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_calendar.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6294 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/test/test_date_basic.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      935 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_date_datenum.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3746 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_date_math.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3971 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_date_parts.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    12064 2022-07-13 03:09:35.000000 ora-0.8.2/python/ora/test/test_daytime_basic.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4025 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/test/test_fmt.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3975 2022-07-13 03:09:35.000000 ora-0.8.2/python/ora/test/test_from_local.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1531 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_functions.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1393 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_local.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    11320 2022-05-07 05:13:09.000000 ora-0.8.2/python/ora/test/test_np_date.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6487 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_np_daytime.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3090 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_np_functions.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8653 2022-05-07 05:13:09.000000 ora-0.8.2/python/ora/test/test_np_time.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      976 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_np_ufuncs_time.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5474 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_parse_date.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4467 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_parse_daytime.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6611 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/test_parse_time.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    14621 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/test/test_time_basic.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6289 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/test/test_time_zone.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1744 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/test/test_time_zone_dir.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1591 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/test/test_vs_zoneinfo.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      330 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/test/tools.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1903 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/util.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2285 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/weekday.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.734318 ora-0.8.2/python/ora/zoneinfo/
+-rw-r--r--   0 alex      (1000) alex      (1000)        6 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/+VERSION
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.744319 ora-0.8.2/python/ora/zoneinfo/Africa/
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Abidjan
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Accra
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Addis_Ababa
+-rw-r--r--   0 alex      (1000) alex      (1000)      470 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Algiers
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Asmara
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Asmera
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Bamako
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Bangui
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Banjul
+-rw-r--r--   0 alex      (1000) alex      (1000)      149 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Bissau
+-rw-r--r--   0 alex      (1000) alex      (1000)      131 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Blantyre
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Brazzaville
+-rw-r--r--   0 alex      (1000) alex      (1000)      131 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Bujumbura
+-rw-r--r--   0 alex      (1000) alex      (1000)     1276 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Cairo
+-rw-r--r--   0 alex      (1000) alex      (1000)     1919 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Casablanca
+-rw-r--r--   0 alex      (1000) alex      (1000)      562 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Ceuta
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Conakry
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Dakar
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Dar_es_Salaam
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Djibouti
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Douala
+-rw-r--r--   0 alex      (1000) alex      (1000)     1830 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/El_Aaiun
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Freetown
+-rw-r--r--   0 alex      (1000) alex      (1000)      131 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Gaborone
+-rw-r--r--   0 alex      (1000) alex      (1000)      131 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Harare
+-rw-r--r--   0 alex      (1000) alex      (1000)      190 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Johannesburg
+-rw-r--r--   0 alex      (1000) alex      (1000)      458 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Juba
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Kampala
+-rw-r--r--   0 alex      (1000) alex      (1000)      458 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Khartoum
+-rw-r--r--   0 alex      (1000) alex      (1000)      131 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Kigali
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Kinshasa
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Lagos
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Libreville
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Lome
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Luanda
+-rw-r--r--   0 alex      (1000) alex      (1000)      131 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Lubumbashi
+-rw-r--r--   0 alex      (1000) alex      (1000)      131 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Lusaka
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Malabo
+-rw-r--r--   0 alex      (1000) alex      (1000)      131 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Maputo
+-rw-r--r--   0 alex      (1000) alex      (1000)      190 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Maseru
+-rw-r--r--   0 alex      (1000) alex      (1000)      190 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Mbabane
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Mogadishu
+-rw-r--r--   0 alex      (1000) alex      (1000)      164 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Monrovia
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Nairobi
+-rw-r--r--   0 alex      (1000) alex      (1000)      160 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Ndjamena
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Niamey
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Nouakchott
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Ouagadougou
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Porto-Novo
+-rw-r--r--   0 alex      (1000) alex      (1000)      173 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Sao_Tome
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Timbuktu
+-rw-r--r--   0 alex      (1000) alex      (1000)      431 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Tripoli
+-rw-r--r--   0 alex      (1000) alex      (1000)      449 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Tunis
+-rw-r--r--   0 alex      (1000) alex      (1000)      638 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Africa/Windhoek
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.767652 ora-0.8.2/python/ora/zoneinfo/America/
+-rw-r--r--   0 alex      (1000) alex      (1000)      969 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Adak
+-rw-r--r--   0 alex      (1000) alex      (1000)      977 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Anchorage
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Anguilla
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Antigua
+-rw-r--r--   0 alex      (1000) alex      (1000)      592 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Araguaina
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Aruba
+-rw-r--r--   0 alex      (1000) alex      (1000)      884 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Asuncion
+-rw-r--r--   0 alex      (1000) alex      (1000)      149 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Atikokan
+-rw-r--r--   0 alex      (1000) alex      (1000)      969 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Atka
+-rw-r--r--   0 alex      (1000) alex      (1000)      682 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Bahia
+-rw-r--r--   0 alex      (1000) alex      (1000)      728 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Bahia_Banderas
+-rw-r--r--   0 alex      (1000) alex      (1000)      278 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Barbados
+-rw-r--r--   0 alex      (1000) alex      (1000)      394 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Belem
+-rw-r--r--   0 alex      (1000) alex      (1000)     1045 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Belize
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Blanc-Sablon
+-rw-r--r--   0 alex      (1000) alex      (1000)      430 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Boa_Vista
+-rw-r--r--   0 alex      (1000) alex      (1000)      179 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Bogota
+-rw-r--r--   0 alex      (1000) alex      (1000)      999 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Boise
+-rw-r--r--   0 alex      (1000) alex      (1000)      708 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Buenos_Aires
+-rw-r--r--   0 alex      (1000) alex      (1000)      883 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Cambridge_Bay
+-rw-r--r--   0 alex      (1000) alex      (1000)      952 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Campo_Grande
+-rw-r--r--   0 alex      (1000) alex      (1000)      529 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Cancun
+-rw-r--r--   0 alex      (1000) alex      (1000)      190 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Caracas
+-rw-r--r--   0 alex      (1000) alex      (1000)      708 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Catamarca
+-rw-r--r--   0 alex      (1000) alex      (1000)      151 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Cayenne
+-rw-r--r--   0 alex      (1000) alex      (1000)      149 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Cayman
+-rw-r--r--   0 alex      (1000) alex      (1000)     1754 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Chicago
+-rw-r--r--   0 alex      (1000) alex      (1000)      691 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Chihuahua
+-rw-r--r--   0 alex      (1000) alex      (1000)      718 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Ciudad_Juarez
+-rw-r--r--   0 alex      (1000) alex      (1000)      149 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Coral_Harbour
+-rw-r--r--   0 alex      (1000) alex      (1000)      708 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Cordoba
+-rw-r--r--   0 alex      (1000) alex      (1000)      232 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Costa_Rica
+-rw-r--r--   0 alex      (1000) alex      (1000)      240 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Creston
+-rw-r--r--   0 alex      (1000) alex      (1000)      934 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Cuiaba
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Curacao
+-rw-r--r--   0 alex      (1000) alex      (1000)      447 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Danmarkshavn
+-rw-r--r--   0 alex      (1000) alex      (1000)     1029 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Dawson
+-rw-r--r--   0 alex      (1000) alex      (1000)      683 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Dawson_Creek
+-rw-r--r--   0 alex      (1000) alex      (1000)     1042 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Denver
+-rw-r--r--   0 alex      (1000) alex      (1000)      899 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Detroit
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Dominica
+-rw-r--r--   0 alex      (1000) alex      (1000)      970 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Edmonton
+-rw-r--r--   0 alex      (1000) alex      (1000)      436 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Eirunepe
+-rw-r--r--   0 alex      (1000) alex      (1000)      176 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/El_Salvador
+-rw-r--r--   0 alex      (1000) alex      (1000)     1025 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Ensenada
+-rw-r--r--   0 alex      (1000) alex      (1000)     1448 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Fort_Nelson
+-rw-r--r--   0 alex      (1000) alex      (1000)      531 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Fort_Wayne
+-rw-r--r--   0 alex      (1000) alex      (1000)      484 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Fortaleza
+-rw-r--r--   0 alex      (1000) alex      (1000)      880 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Glace_Bay
+-rw-r--r--   0 alex      (1000) alex      (1000)      931 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Godthab
+-rw-r--r--   0 alex      (1000) alex      (1000)     1580 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Goose_Bay
+-rw-r--r--   0 alex      (1000) alex      (1000)      853 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Grand_Turk
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Grenada
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Guadeloupe
+-rw-r--r--   0 alex      (1000) alex      (1000)      212 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Guatemala
+-rw-r--r--   0 alex      (1000) alex      (1000)      179 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Guayaquil
+-rw-r--r--   0 alex      (1000) alex      (1000)      181 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Guyana
+-rw-r--r--   0 alex      (1000) alex      (1000)     1672 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Halifax
+-rw-r--r--   0 alex      (1000) alex      (1000)     1117 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Havana
+-rw-r--r--   0 alex      (1000) alex      (1000)      286 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Hermosillo
+-rw-r--r--   0 alex      (1000) alex      (1000)      531 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Indianapolis
+-rw-r--r--   0 alex      (1000) alex      (1000)      817 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Inuvik
+-rw-r--r--   0 alex      (1000) alex      (1000)      855 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Iqaluit
+-rw-r--r--   0 alex      (1000) alex      (1000)      339 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Jamaica
+-rw-r--r--   0 alex      (1000) alex      (1000)      690 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Jujuy
+-rw-r--r--   0 alex      (1000) alex      (1000)      966 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Juneau
+-rw-r--r--   0 alex      (1000) alex      (1000)     1016 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Knox_IN
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Kralendijk
+-rw-r--r--   0 alex      (1000) alex      (1000)      170 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/La_Paz
+-rw-r--r--   0 alex      (1000) alex      (1000)      283 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Lima
+-rw-r--r--   0 alex      (1000) alex      (1000)     1294 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Los_Angeles
+-rw-r--r--   0 alex      (1000) alex      (1000)     1242 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Louisville
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Lower_Princes
+-rw-r--r--   0 alex      (1000) alex      (1000)      502 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Maceio
+-rw-r--r--   0 alex      (1000) alex      (1000)      295 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Managua
+-rw-r--r--   0 alex      (1000) alex      (1000)      412 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Manaus
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Marigot
+-rw-r--r--   0 alex      (1000) alex      (1000)      178 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Martinique
+-rw-r--r--   0 alex      (1000) alex      (1000)      437 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Matamoros
+-rw-r--r--   0 alex      (1000) alex      (1000)      718 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Mazatlan
+-rw-r--r--   0 alex      (1000) alex      (1000)      708 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Mendoza
+-rw-r--r--   0 alex      (1000) alex      (1000)      917 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Menominee
+-rw-r--r--   0 alex      (1000) alex      (1000)      654 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Merida
+-rw-r--r--   0 alex      (1000) alex      (1000)      595 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Metlakatla
+-rw-r--r--   0 alex      (1000) alex      (1000)      773 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Mexico_City
+-rw-r--r--   0 alex      (1000) alex      (1000)      550 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Miquelon
+-rw-r--r--   0 alex      (1000) alex      (1000)     1493 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Moncton
+-rw-r--r--   0 alex      (1000) alex      (1000)      644 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Monterrey
+-rw-r--r--   0 alex      (1000) alex      (1000)      969 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Montevideo
+-rw-r--r--   0 alex      (1000) alex      (1000)     1717 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Montreal
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Montserrat
+-rw-r--r--   0 alex      (1000) alex      (1000)     1717 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Nassau
+-rw-r--r--   0 alex      (1000) alex      (1000)     1744 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/New_York
+-rw-r--r--   0 alex      (1000) alex      (1000)     1717 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Nipigon
+-rw-r--r--   0 alex      (1000) alex      (1000)      975 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Nome
+-rw-r--r--   0 alex      (1000) alex      (1000)      484 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Noronha
+-rw-r--r--   0 alex      (1000) alex      (1000)      931 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Nuuk
+-rw-r--r--   0 alex      (1000) alex      (1000)      709 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Ojinaga
+-rw-r--r--   0 alex      (1000) alex      (1000)      149 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Panama
+-rw-r--r--   0 alex      (1000) alex      (1000)      855 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Pangnirtung
+-rw-r--r--   0 alex      (1000) alex      (1000)      187 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Paramaribo
+-rw-r--r--   0 alex      (1000) alex      (1000)      240 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Phoenix
+-rw-r--r--   0 alex      (1000) alex      (1000)      565 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Port-au-Prince
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Port_of_Spain
+-rw-r--r--   0 alex      (1000) alex      (1000)      418 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Porto_Acre
+-rw-r--r--   0 alex      (1000) alex      (1000)      394 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Porto_Velho
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Puerto_Rico
+-rw-r--r--   0 alex      (1000) alex      (1000)     1218 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Punta_Arenas
+-rw-r--r--   0 alex      (1000) alex      (1000)     1294 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Rainy_River
+-rw-r--r--   0 alex      (1000) alex      (1000)      807 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Rankin_Inlet
+-rw-r--r--   0 alex      (1000) alex      (1000)      484 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Recife
+-rw-r--r--   0 alex      (1000) alex      (1000)      638 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Regina
+-rw-r--r--   0 alex      (1000) alex      (1000)      807 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Resolute
+-rw-r--r--   0 alex      (1000) alex      (1000)      418 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Rio_Branco
+-rw-r--r--   0 alex      (1000) alex      (1000)      708 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Rosario
+-rw-r--r--   0 alex      (1000) alex      (1000)     1025 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Santa_Isabel
+-rw-r--r--   0 alex      (1000) alex      (1000)      409 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Santarem
+-rw-r--r--   0 alex      (1000) alex      (1000)     1354 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Santiago
+-rw-r--r--   0 alex      (1000) alex      (1000)      317 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Santo_Domingo
+-rw-r--r--   0 alex      (1000) alex      (1000)      952 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Sao_Paulo
+-rw-r--r--   0 alex      (1000) alex      (1000)      479 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Scoresbysund
+-rw-r--r--   0 alex      (1000) alex      (1000)     1042 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Shiprock
+-rw-r--r--   0 alex      (1000) alex      (1000)      956 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Sitka
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/St_Barthelemy
+-rw-r--r--   0 alex      (1000) alex      (1000)     1878 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/St_Johns
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/St_Kitts
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/St_Lucia
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/St_Thomas
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/St_Vincent
+-rw-r--r--   0 alex      (1000) alex      (1000)      368 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Swift_Current
+-rw-r--r--   0 alex      (1000) alex      (1000)      194 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Tegucigalpa
+-rw-r--r--   0 alex      (1000) alex      (1000)      455 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Thule
+-rw-r--r--   0 alex      (1000) alex      (1000)     1717 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Thunder_Bay
+-rw-r--r--   0 alex      (1000) alex      (1000)     1025 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Tijuana
+-rw-r--r--   0 alex      (1000) alex      (1000)     1717 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Toronto
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Tortola
+-rw-r--r--   0 alex      (1000) alex      (1000)     1330 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Vancouver
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/America/Virgin
+-rw-r--r--   0 alex      (1000) alex      (1000)     1029 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Whitehorse
+-rw-r--r--   0 alex      (1000) alex      (1000)     1294 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Winnipeg
+-rw-r--r--   0 alex      (1000) alex      (1000)      946 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/America/Yakutat
+-rw-r--r--   0 alex      (1000) alex      (1000)      844 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/America/Yellowknife
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.770985 ora-0.8.2/python/ora/zoneinfo/Antarctica/
+-rw-r--r--   0 alex      (1000) alex      (1000)      243 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/Casey
+-rw-r--r--   0 alex      (1000) alex      (1000)      197 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/Davis
+-rw-r--r--   0 alex      (1000) alex      (1000)      154 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/DumontDUrville
+-rw-r--r--   0 alex      (1000) alex      (1000)      976 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/Macquarie
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/Mawson
+-rw-r--r--   0 alex      (1000) alex      (1000)     1043 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/McMurdo
+-rw-r--r--   0 alex      (1000) alex      (1000)      887 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/Palmer
+-rw-r--r--   0 alex      (1000) alex      (1000)      132 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/Rothera
+-rw-r--r--   0 alex      (1000) alex      (1000)     1043 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/South_Pole
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/Syowa
+-rw-r--r--   0 alex      (1000) alex      (1000)      177 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/Troll
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Antarctica/Vostok
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.770985 ora-0.8.2/python/ora/zoneinfo/Arctic/
+-rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Arctic/Longyearbyen
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.787653 ora-0.8.2/python/ora/zoneinfo/Asia/
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Aden
+-rw-r--r--   0 alex      (1000) alex      (1000)      609 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Almaty
+-rw-r--r--   0 alex      (1000) alex      (1000)      928 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Amman
+-rw-r--r--   0 alex      (1000) alex      (1000)      743 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Anadyr
+-rw-r--r--   0 alex      (1000) alex      (1000)      606 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Aqtau
+-rw-r--r--   0 alex      (1000) alex      (1000)      615 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Aqtobe
+-rw-r--r--   0 alex      (1000) alex      (1000)      375 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Ashgabat
+-rw-r--r--   0 alex      (1000) alex      (1000)      375 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Ashkhabad
+-rw-r--r--   0 alex      (1000) alex      (1000)      616 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Atyrau
+-rw-r--r--   0 alex      (1000) alex      (1000)      630 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Baghdad
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Bahrain
+-rw-r--r--   0 alex      (1000) alex      (1000)      744 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Baku
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Bangkok
+-rw-r--r--   0 alex      (1000) alex      (1000)      753 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Barnaul
+-rw-r--r--   0 alex      (1000) alex      (1000)      732 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Beirut
+-rw-r--r--   0 alex      (1000) alex      (1000)      618 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Bishkek
+-rw-r--r--   0 alex      (1000) alex      (1000)      320 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Brunei
+-rw-r--r--   0 alex      (1000) alex      (1000)      220 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Calcutta
+-rw-r--r--   0 alex      (1000) alex      (1000)      750 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Chita
+-rw-r--r--   0 alex      (1000) alex      (1000)      619 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Choibalsan
+-rw-r--r--   0 alex      (1000) alex      (1000)      393 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Chongqing
+-rw-r--r--   0 alex      (1000) alex      (1000)      393 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Chungking
+-rw-r--r--   0 alex      (1000) alex      (1000)      247 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Colombo
+-rw-r--r--   0 alex      (1000) alex      (1000)      231 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Dacca
+-rw-r--r--   0 alex      (1000) alex      (1000)     1234 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Damascus
+-rw-r--r--   0 alex      (1000) alex      (1000)      231 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Dhaka
+-rw-r--r--   0 alex      (1000) alex      (1000)      170 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Dili
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Dubai
+-rw-r--r--   0 alex      (1000) alex      (1000)      366 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Dushanbe
+-rw-r--r--   0 alex      (1000) alex      (1000)      940 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Famagusta
+-rw-r--r--   0 alex      (1000) alex      (1000)     1258 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Gaza
+-rw-r--r--   0 alex      (1000) alex      (1000)      393 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Harbin
+-rw-r--r--   0 alex      (1000) alex      (1000)     1276 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Hebron
+-rw-r--r--   0 alex      (1000) alex      (1000)      236 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Ho_Chi_Minh
+-rw-r--r--   0 alex      (1000) alex      (1000)      775 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Hong_Kong
+-rw-r--r--   0 alex      (1000) alex      (1000)      594 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Hovd
+-rw-r--r--   0 alex      (1000) alex      (1000)      760 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Irkutsk
+-rw-r--r--   0 alex      (1000) alex      (1000)     1200 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Istanbul
+-rw-r--r--   0 alex      (1000) alex      (1000)      248 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Jakarta
+-rw-r--r--   0 alex      (1000) alex      (1000)      171 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Jayapura
+-rw-r--r--   0 alex      (1000) alex      (1000)     1074 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Jerusalem
+-rw-r--r--   0 alex      (1000) alex      (1000)      159 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Kabul
+-rw-r--r--   0 alex      (1000) alex      (1000)      727 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Kamchatka
+-rw-r--r--   0 alex      (1000) alex      (1000)      266 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Karachi
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Kashgar
+-rw-r--r--   0 alex      (1000) alex      (1000)      161 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Kathmandu
+-rw-r--r--   0 alex      (1000) alex      (1000)      161 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Katmandu
+-rw-r--r--   0 alex      (1000) alex      (1000)      775 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Khandyga
+-rw-r--r--   0 alex      (1000) alex      (1000)      220 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Kolkata
+-rw-r--r--   0 alex      (1000) alex      (1000)      741 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Krasnoyarsk
+-rw-r--r--   0 alex      (1000) alex      (1000)      256 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Kuala_Lumpur
+-rw-r--r--   0 alex      (1000) alex      (1000)      320 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Kuching
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Kuwait
+-rw-r--r--   0 alex      (1000) alex      (1000)      791 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Macao
+-rw-r--r--   0 alex      (1000) alex      (1000)      791 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Macau
+-rw-r--r--   0 alex      (1000) alex      (1000)      751 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Magadan
+-rw-r--r--   0 alex      (1000) alex      (1000)      190 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Makassar
+-rw-r--r--   0 alex      (1000) alex      (1000)      238 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Manila
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Muscat
+-rw-r--r--   0 alex      (1000) alex      (1000)      597 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Nicosia
+-rw-r--r--   0 alex      (1000) alex      (1000)      726 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Novokuznetsk
+-rw-r--r--   0 alex      (1000) alex      (1000)      753 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Novosibirsk
+-rw-r--r--   0 alex      (1000) alex      (1000)      741 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Omsk
+-rw-r--r--   0 alex      (1000) alex      (1000)      625 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Oral
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Phnom_Penh
+-rw-r--r--   0 alex      (1000) alex      (1000)      247 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Pontianak
+-rw-r--r--   0 alex      (1000) alex      (1000)      183 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Pyongyang
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Qatar
+-rw-r--r--   0 alex      (1000) alex      (1000)      615 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Qostanay
+-rw-r--r--   0 alex      (1000) alex      (1000)      624 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Qyzylorda
+-rw-r--r--   0 alex      (1000) alex      (1000)      187 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Rangoon
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Riyadh
+-rw-r--r--   0 alex      (1000) alex      (1000)      236 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Saigon
+-rw-r--r--   0 alex      (1000) alex      (1000)      755 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Sakhalin
+-rw-r--r--   0 alex      (1000) alex      (1000)      366 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Samarkand
+-rw-r--r--   0 alex      (1000) alex      (1000)      415 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Seoul
+-rw-r--r--   0 alex      (1000) alex      (1000)      393 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Shanghai
+-rw-r--r--   0 alex      (1000) alex      (1000)      256 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Singapore
+-rw-r--r--   0 alex      (1000) alex      (1000)      742 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Srednekolymsk
+-rw-r--r--   0 alex      (1000) alex      (1000)      511 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Taipei
+-rw-r--r--   0 alex      (1000) alex      (1000)      366 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Tashkent
+-rw-r--r--   0 alex      (1000) alex      (1000)      629 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Tbilisi
+-rw-r--r--   0 alex      (1000) alex      (1000)      812 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Tehran
+-rw-r--r--   0 alex      (1000) alex      (1000)     1074 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Tel_Aviv
+-rw-r--r--   0 alex      (1000) alex      (1000)      154 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Thimbu
+-rw-r--r--   0 alex      (1000) alex      (1000)      154 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Thimphu
+-rw-r--r--   0 alex      (1000) alex      (1000)      213 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Tokyo
+-rw-r--r--   0 alex      (1000) alex      (1000)      753 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Tomsk
+-rw-r--r--   0 alex      (1000) alex      (1000)      190 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Ujung_Pandang
+-rw-r--r--   0 alex      (1000) alex      (1000)      594 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Ulaanbaatar
+-rw-r--r--   0 alex      (1000) alex      (1000)      594 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Ulan_Bator
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Urumqi
+-rw-r--r--   0 alex      (1000) alex      (1000)      771 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Ust-Nera
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Vientiane
+-rw-r--r--   0 alex      (1000) alex      (1000)      742 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Vladivostok
+-rw-r--r--   0 alex      (1000) alex      (1000)      741 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Yakutsk
+-rw-r--r--   0 alex      (1000) alex      (1000)      187 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Yangon
+-rw-r--r--   0 alex      (1000) alex      (1000)      760 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Yekaterinburg
+-rw-r--r--   0 alex      (1000) alex      (1000)      708 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Asia/Yerevan
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.787653 ora-0.8.2/python/ora/zoneinfo/Atlantic/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1453 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Azores
+-rw-r--r--   0 alex      (1000) alex      (1000)     1024 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Bermuda
+-rw-r--r--   0 alex      (1000) alex      (1000)      478 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Canary
+-rw-r--r--   0 alex      (1000) alex      (1000)      175 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Cape_Verde
+-rw-r--r--   0 alex      (1000) alex      (1000)      441 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Faeroe
+-rw-r--r--   0 alex      (1000) alex      (1000)      441 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Faroe
+-rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Jan_Mayen
+-rw-r--r--   0 alex      (1000) alex      (1000)     1453 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Madeira
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Reykjavik
+-rw-r--r--   0 alex      (1000) alex      (1000)      132 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/South_Georgia
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/St_Helena
+-rw-r--r--   0 alex      (1000) alex      (1000)      789 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Atlantic/Stanley
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.790986 ora-0.8.2/python/ora/zoneinfo/Australia/
+-rw-r--r--   0 alex      (1000) alex      (1000)      904 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/ACT
+-rw-r--r--   0 alex      (1000) alex      (1000)      921 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Adelaide
+-rw-r--r--   0 alex      (1000) alex      (1000)      289 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Brisbane
+-rw-r--r--   0 alex      (1000) alex      (1000)      941 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Broken_Hill
+-rw-r--r--   0 alex      (1000) alex      (1000)      904 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Canberra
+-rw-r--r--   0 alex      (1000) alex      (1000)     1003 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Currie
+-rw-r--r--   0 alex      (1000) alex      (1000)      234 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Darwin
+-rw-r--r--   0 alex      (1000) alex      (1000)      314 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Eucla
+-rw-r--r--   0 alex      (1000) alex      (1000)     1003 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Hobart
+-rw-r--r--   0 alex      (1000) alex      (1000)      692 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/LHI
+-rw-r--r--   0 alex      (1000) alex      (1000)      325 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Lindeman
+-rw-r--r--   0 alex      (1000) alex      (1000)      692 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Lord_Howe
+-rw-r--r--   0 alex      (1000) alex      (1000)      904 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Melbourne
+-rw-r--r--   0 alex      (1000) alex      (1000)      904 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/NSW
+-rw-r--r--   0 alex      (1000) alex      (1000)      234 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/North
+-rw-r--r--   0 alex      (1000) alex      (1000)      306 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Perth
+-rw-r--r--   0 alex      (1000) alex      (1000)      289 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Queensland
+-rw-r--r--   0 alex      (1000) alex      (1000)      921 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/South
+-rw-r--r--   0 alex      (1000) alex      (1000)      904 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Sydney
+-rw-r--r--   0 alex      (1000) alex      (1000)     1003 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Tasmania
+-rw-r--r--   0 alex      (1000) alex      (1000)      904 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Victoria
+-rw-r--r--   0 alex      (1000) alex      (1000)      306 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/West
+-rw-r--r--   0 alex      (1000) alex      (1000)      941 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Australia/Yancowinna
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.794319 ora-0.8.2/python/ora/zoneinfo/Brazil/
+-rw-r--r--   0 alex      (1000) alex      (1000)      418 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Brazil/Acre
+-rw-r--r--   0 alex      (1000) alex      (1000)      484 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Brazil/DeNoronha
+-rw-r--r--   0 alex      (1000) alex      (1000)      952 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Brazil/East
+-rw-r--r--   0 alex      (1000) alex      (1000)      412 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Brazil/West
+-rw-r--r--   0 alex      (1000) alex      (1000)      621 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/CET
+-rw-r--r--   0 alex      (1000) alex      (1000)      951 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/CST6CDT
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.794319 ora-0.8.2/python/ora/zoneinfo/Canada/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1672 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Canada/Atlantic
+-rw-r--r--   0 alex      (1000) alex      (1000)     1294 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Canada/Central
+-rw-r--r--   0 alex      (1000) alex      (1000)     1717 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Canada/Eastern
+-rw-r--r--   0 alex      (1000) alex      (1000)      970 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Canada/Mountain
+-rw-r--r--   0 alex      (1000) alex      (1000)     1878 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Canada/Newfoundland
+-rw-r--r--   0 alex      (1000) alex      (1000)     1330 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Canada/Pacific
+-rw-r--r--   0 alex      (1000) alex      (1000)      638 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Canada/Saskatchewan
+-rw-r--r--   0 alex      (1000) alex      (1000)     1029 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Canada/Yukon
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.794319 ora-0.8.2/python/ora/zoneinfo/Chile/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1354 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Chile/Continental
+-rw-r--r--   0 alex      (1000) alex      (1000)     1174 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Chile/EasterIsland
+-rw-r--r--   0 alex      (1000) alex      (1000)     1117 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Cuba
+-rw-r--r--   0 alex      (1000) alex      (1000)      497 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/EET
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/EST
+-rw-r--r--   0 alex      (1000) alex      (1000)      951 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/EST5EDT
+-rw-r--r--   0 alex      (1000) alex      (1000)     1276 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Egypt
+-rw-r--r--   0 alex      (1000) alex      (1000)     1496 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Eire
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.797653 ora-0.8.2/python/ora/zoneinfo/Etc/
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+0
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+1
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+10
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+11
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+12
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+2
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+3
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+4
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+5
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+6
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+7
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+8
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT+9
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-0
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-1
+-rw-r--r--   0 alex      (1000) alex      (1000)      115 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-10
+-rw-r--r--   0 alex      (1000) alex      (1000)      115 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-11
+-rw-r--r--   0 alex      (1000) alex      (1000)      115 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-12
+-rw-r--r--   0 alex      (1000) alex      (1000)      115 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-13
+-rw-r--r--   0 alex      (1000) alex      (1000)      115 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-14
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-2
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-3
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-4
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-5
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-6
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-7
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-8
+-rw-r--r--   0 alex      (1000) alex      (1000)      114 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT-9
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/GMT0
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/Greenwich
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/UCT
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/UTC
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/Universal
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Etc/Zulu
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.810986 ora-0.8.2/python/ora/zoneinfo/Europe/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1103 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Amsterdam
+-rw-r--r--   0 alex      (1000) alex      (1000)      389 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Andorra
+-rw-r--r--   0 alex      (1000) alex      (1000)      726 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Astrakhan
+-rw-r--r--   0 alex      (1000) alex      (1000)      682 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Athens
+-rw-r--r--   0 alex      (1000) alex      (1000)     1599 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Belfast
+-rw-r--r--   0 alex      (1000) alex      (1000)      478 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Belgrade
+-rw-r--r--   0 alex      (1000) alex      (1000)      705 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Berlin
+-rw-r--r--   0 alex      (1000) alex      (1000)      723 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Bratislava
+-rw-r--r--   0 alex      (1000) alex      (1000)     1103 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Brussels
+-rw-r--r--   0 alex      (1000) alex      (1000)      661 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Bucharest
+-rw-r--r--   0 alex      (1000) alex      (1000)      766 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Budapest
+-rw-r--r--   0 alex      (1000) alex      (1000)      497 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Busingen
+-rw-r--r--   0 alex      (1000) alex      (1000)      755 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Chisinau
+-rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Copenhagen
+-rw-r--r--   0 alex      (1000) alex      (1000)     1496 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Dublin
+-rw-r--r--   0 alex      (1000) alex      (1000)     1220 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Gibraltar
+-rw-r--r--   0 alex      (1000) alex      (1000)     1599 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Guernsey
+-rw-r--r--   0 alex      (1000) alex      (1000)      481 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Helsinki
+-rw-r--r--   0 alex      (1000) alex      (1000)     1599 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Isle_of_Man
+-rw-r--r--   0 alex      (1000) alex      (1000)     1200 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Istanbul
+-rw-r--r--   0 alex      (1000) alex      (1000)     1599 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Jersey
+-rw-r--r--   0 alex      (1000) alex      (1000)      904 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Kaliningrad
+-rw-r--r--   0 alex      (1000) alex      (1000)      558 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Kiev
+-rw-r--r--   0 alex      (1000) alex      (1000)      717 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Kirov
+-rw-r--r--   0 alex      (1000) alex      (1000)      558 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Kyiv
+-rw-r--r--   0 alex      (1000) alex      (1000)     1454 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Lisbon
+-rw-r--r--   0 alex      (1000) alex      (1000)      478 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Ljubljana
+-rw-r--r--   0 alex      (1000) alex      (1000)     1599 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/London
+-rw-r--r--   0 alex      (1000) alex      (1000)     1103 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Luxembourg
+-rw-r--r--   0 alex      (1000) alex      (1000)      897 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Madrid
+-rw-r--r--   0 alex      (1000) alex      (1000)      928 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Malta
+-rw-r--r--   0 alex      (1000) alex      (1000)      481 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Mariehamn
+-rw-r--r--   0 alex      (1000) alex      (1000)      808 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Minsk
+-rw-r--r--   0 alex      (1000) alex      (1000)     1105 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Monaco
+-rw-r--r--   0 alex      (1000) alex      (1000)      908 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Moscow
+-rw-r--r--   0 alex      (1000) alex      (1000)      597 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Nicosia
+-rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Oslo
+-rw-r--r--   0 alex      (1000) alex      (1000)     1105 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Paris
+-rw-r--r--   0 alex      (1000) alex      (1000)      478 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Podgorica
+-rw-r--r--   0 alex      (1000) alex      (1000)      723 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Prague
+-rw-r--r--   0 alex      (1000) alex      (1000)      694 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Riga
+-rw-r--r--   0 alex      (1000) alex      (1000)      947 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Rome
+-rw-r--r--   0 alex      (1000) alex      (1000)      732 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Samara
+-rw-r--r--   0 alex      (1000) alex      (1000)      947 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/San_Marino
+-rw-r--r--   0 alex      (1000) alex      (1000)      478 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Sarajevo
+-rw-r--r--   0 alex      (1000) alex      (1000)      726 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Saratov
+-rw-r--r--   0 alex      (1000) alex      (1000)      865 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Simferopol
+-rw-r--r--   0 alex      (1000) alex      (1000)      478 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Skopje
+-rw-r--r--   0 alex      (1000) alex      (1000)      592 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Sofia
+-rw-r--r--   0 alex      (1000) alex      (1000)      705 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Stockholm
+-rw-r--r--   0 alex      (1000) alex      (1000)      675 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Tallinn
+-rw-r--r--   0 alex      (1000) alex      (1000)      604 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Tirane
+-rw-r--r--   0 alex      (1000) alex      (1000)      755 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Tiraspol
+-rw-r--r--   0 alex      (1000) alex      (1000)      760 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Ulyanovsk
+-rw-r--r--   0 alex      (1000) alex      (1000)      558 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Uzhgorod
+-rw-r--r--   0 alex      (1000) alex      (1000)      497 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Vaduz
+-rw-r--r--   0 alex      (1000) alex      (1000)      947 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Vatican
+-rw-r--r--   0 alex      (1000) alex      (1000)      658 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Vienna
+-rw-r--r--   0 alex      (1000) alex      (1000)      676 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Vilnius
+-rw-r--r--   0 alex      (1000) alex      (1000)      735 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Volgograd
+-rw-r--r--   0 alex      (1000) alex      (1000)      923 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Warsaw
+-rw-r--r--   0 alex      (1000) alex      (1000)      478 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Zagreb
+-rw-r--r--   0 alex      (1000) alex      (1000)      558 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Zaporozhye
+-rw-r--r--   0 alex      (1000) alex      (1000)      497 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Europe/Zurich
+-rw-r--r--   0 alex      (1000) alex      (1000)      113 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Factory
+-rw-r--r--   0 alex      (1000) alex      (1000)     1599 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/GB
+-rw-r--r--   0 alex      (1000) alex      (1000)     1599 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/GB-Eire
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/GMT
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/GMT+0
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/GMT-0
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/GMT0
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Greenwich
+-rw-r--r--   0 alex      (1000) alex      (1000)      112 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/HST
+-rw-r--r--   0 alex      (1000) alex      (1000)      775 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Hongkong
+-rw-r--r--   0 alex      (1000) alex      (1000)      130 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Iceland
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.810986 ora-0.8.2/python/ora/zoneinfo/Indian/
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Antananarivo
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Chagos
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Christmas
+-rw-r--r--   0 alex      (1000) alex      (1000)      187 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Cocos
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Comoro
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Kerguelen
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Mahe
+-rw-r--r--   0 alex      (1000) alex      (1000)      152 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Maldives
+-rw-r--r--   0 alex      (1000) alex      (1000)      179 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Mauritius
+-rw-r--r--   0 alex      (1000) alex      (1000)      191 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Mayotte
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Indian/Reunion
+-rw-r--r--   0 alex      (1000) alex      (1000)      812 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Iran
+-rw-r--r--   0 alex      (1000) alex      (1000)     1074 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Israel
+-rw-r--r--   0 alex      (1000) alex      (1000)      339 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Jamaica
+-rw-r--r--   0 alex      (1000) alex      (1000)      213 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Japan
+-rw-r--r--   0 alex      (1000) alex      (1000)      219 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Kwajalein
+-rw-r--r--   0 alex      (1000) alex      (1000)      431 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Libya
+-rw-r--r--   0 alex      (1000) alex      (1000)      621 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/MET
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/MST
+-rw-r--r--   0 alex      (1000) alex      (1000)      951 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/MST7MDT
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.810986 ora-0.8.2/python/ora/zoneinfo/Mexico/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1025 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Mexico/BajaNorte
+-rw-r--r--   0 alex      (1000) alex      (1000)      718 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Mexico/BajaSur
+-rw-r--r--   0 alex      (1000) alex      (1000)      773 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Mexico/General
+-rw-r--r--   0 alex      (1000) alex      (1000)     1043 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/NZ
+-rw-r--r--   0 alex      (1000) alex      (1000)      808 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/NZ-CHAT
+-rw-r--r--   0 alex      (1000) alex      (1000)     1042 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Navajo
+-rw-r--r--   0 alex      (1000) alex      (1000)      393 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/PRC
+-rw-r--r--   0 alex      (1000) alex      (1000)      951 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/PST8PDT
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.817653 ora-0.8.2/python/ora/zoneinfo/Pacific/
+-rw-r--r--   0 alex      (1000) alex      (1000)      407 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Apia
+-rw-r--r--   0 alex      (1000) alex      (1000)     1043 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Auckland
+-rw-r--r--   0 alex      (1000) alex      (1000)      201 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Bougainville
+-rw-r--r--   0 alex      (1000) alex      (1000)      808 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Chatham
+-rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Chuuk
+-rw-r--r--   0 alex      (1000) alex      (1000)     1174 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Easter
+-rw-r--r--   0 alex      (1000) alex      (1000)      342 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Efate
+-rw-r--r--   0 alex      (1000) alex      (1000)      172 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Enderbury
+-rw-r--r--   0 alex      (1000) alex      (1000)      153 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Fakaofo
+-rw-r--r--   0 alex      (1000) alex      (1000)      396 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Fiji
+-rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Funafuti
+-rw-r--r--   0 alex      (1000) alex      (1000)      175 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Galapagos
+-rw-r--r--   0 alex      (1000) alex      (1000)      132 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Gambier
+-rw-r--r--   0 alex      (1000) alex      (1000)      134 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Guadalcanal
+-rw-r--r--   0 alex      (1000) alex      (1000)      350 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Guam
+-rw-r--r--   0 alex      (1000) alex      (1000)      221 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Honolulu
+-rw-r--r--   0 alex      (1000) alex      (1000)      221 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Johnston
+-rw-r--r--   0 alex      (1000) alex      (1000)      172 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Kanton
+-rw-r--r--   0 alex      (1000) alex      (1000)      174 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Kiritimati
+-rw-r--r--   0 alex      (1000) alex      (1000)      242 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Kosrae
+-rw-r--r--   0 alex      (1000) alex      (1000)      219 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Kwajalein
+-rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Majuro
+-rw-r--r--   0 alex      (1000) alex      (1000)      139 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Marquesas
+-rw-r--r--   0 alex      (1000) alex      (1000)      146 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Midway
+-rw-r--r--   0 alex      (1000) alex      (1000)      183 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Nauru
+-rw-r--r--   0 alex      (1000) alex      (1000)      154 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Niue
+-rw-r--r--   0 alex      (1000) alex      (1000)      247 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Norfolk
+-rw-r--r--   0 alex      (1000) alex      (1000)      198 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Noumea
+-rw-r--r--   0 alex      (1000) alex      (1000)      146 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Pago_Pago
+-rw-r--r--   0 alex      (1000) alex      (1000)      148 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Palau
+-rw-r--r--   0 alex      (1000) alex      (1000)      153 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Pitcairn
+-rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Pohnpei
+-rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Ponape
+-rw-r--r--   0 alex      (1000) alex      (1000)      154 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Port_Moresby
+-rw-r--r--   0 alex      (1000) alex      (1000)      406 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Rarotonga
+-rw-r--r--   0 alex      (1000) alex      (1000)      350 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Saipan
+-rw-r--r--   0 alex      (1000) alex      (1000)      146 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Samoa
+-rw-r--r--   0 alex      (1000) alex      (1000)      133 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Tahiti
+-rw-r--r--   0 alex      (1000) alex      (1000)      134 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Tarawa
+-rw-r--r--   0 alex      (1000) alex      (1000)      237 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Tongatapu
+-rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Truk
+-rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Wake
+-rw-r--r--   0 alex      (1000) alex      (1000)      134 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Wallis
+-rw-r--r--   0 alex      (1000) alex      (1000)      154 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Pacific/Yap
+-rw-r--r--   0 alex      (1000) alex      (1000)      923 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Poland
+-rw-r--r--   0 alex      (1000) alex      (1000)     1454 2022-05-11 05:46:09.000000 ora-0.8.2/python/ora/zoneinfo/Portugal
+-rw-r--r--   0 alex      (1000) alex      (1000)      511 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/ROC
+-rw-r--r--   0 alex      (1000) alex      (1000)      415 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/ROK
+-rw-r--r--   0 alex      (1000) alex      (1000)      256 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/Singapore
+-rw-r--r--   0 alex      (1000) alex      (1000)     1200 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Turkey
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/UCT
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.820986 ora-0.8.2/python/ora/zoneinfo/US/
+-rw-r--r--   0 alex      (1000) alex      (1000)      977 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Alaska
+-rw-r--r--   0 alex      (1000) alex      (1000)      969 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Aleutian
+-rw-r--r--   0 alex      (1000) alex      (1000)      240 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Arizona
+-rw-r--r--   0 alex      (1000) alex      (1000)     1754 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Central
+-rw-r--r--   0 alex      (1000) alex      (1000)      531 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/East-Indiana
+-rw-r--r--   0 alex      (1000) alex      (1000)     1744 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Eastern
+-rw-r--r--   0 alex      (1000) alex      (1000)      221 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Hawaii
+-rw-r--r--   0 alex      (1000) alex      (1000)     1016 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Indiana-Starke
+-rw-r--r--   0 alex      (1000) alex      (1000)      899 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Michigan
+-rw-r--r--   0 alex      (1000) alex      (1000)     1042 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Mountain
+-rw-r--r--   0 alex      (1000) alex      (1000)     1294 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Pacific
+-rw-r--r--   0 alex      (1000) alex      (1000)      146 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/US/Samoa
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/UTC
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Universal
+-rw-r--r--   0 alex      (1000) alex      (1000)      908 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/W-SU
+-rw-r--r--   0 alex      (1000) alex      (1000)      494 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/WET
+-rw-r--r--   0 alex      (1000) alex      (1000)      111 2022-04-21 13:40:08.000000 ora-0.8.2/python/ora/zoneinfo/Zulu
+-rw-r--r--   0 alex      (1000) alex      (1000)     4458 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/iso3166.tab
+-rw-r--r--   0 alex      (1000) alex      (1000)     3388 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/leapseconds
+-rw-r--r--   0 alex      (1000) alex      (1000)   107242 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/tzdata.zi
+-rw-r--r--   0 alex      (1000) alex      (1000)    18955 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/zone.tab
+-rw-r--r--   0 alex      (1000) alex      (1000)    17609 2023-05-30 04:06:23.000000 ora-0.8.2/python/ora/zoneinfo/zone1970.tab
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-30 04:08:17.717651 ora-0.8.2/python/ora.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      832 2023-05-30 04:08:17.000000 ora-0.8.2/python/ora.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)    24486 2023-05-30 04:08:17.000000 ora-0.8.2/python/ora.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-30 04:08:17.000000 ora-0.8.2/python/ora.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        6 2023-05-30 04:08:17.000000 ora-0.8.2/python/ora.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        4 2023-05-30 04:08:17.000000 ora-0.8.2/python/ora.egg-info/top_level.txt
+-rwxr-xr-x   0 alex      (1000) alex      (1000)      838 2022-04-21 13:40:08.000000 ora-0.8.2/python/wrap_docstrings
+-rw-r--r--   0 alex      (1000) alex      (1000)      380 2023-05-30 04:08:17.820986 ora-0.8.2/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1000)     3318 2023-05-30 04:07:38.000000 ora-0.8.2/setup.py
```

### Comparing `ora-0.8.0/LICENSE` & `ora-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/Makefile` & `ora-0.8.2/Makefile`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/PKG-INFO` & `ora-0.8.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ora
-Version: 0.8.0
+Version: 0.8.2
 Summary: Alternative time and date library
 Home-page: https://github.com/alexhsamuel/ora
 Author: Alex Samuel
 Author-email: alexhsamuel@gmail.com
 License: BSD-3
 Keywords: time,date,time zone
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 License-File: LICENSE
@@ -20,9 +19,7 @@
 Ora is a freestanding time and date implementation for C++ and Python.
 
 Ora is `hosted on GitHub <http://github.com/alexhsamuel/ora>`_.  See
 the `installation instructions
 <https://github.com/alexhsamuel/ora/blob/master/README.md#installation>`_.
 
 Docs at `readthedocs <http://ora.readthedocs.io/en/latest/>`_.
-
-
```

### Comparing `ora-0.8.0/README.md` & `ora-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/calendar.hh` & `ora-0.8.2/cxx/include/ora/calendar.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/date_functions.hh` & `ora-0.8.2/cxx/include/ora/date_functions.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/date_math.hh` & `ora-0.8.2/cxx/include/ora/date_math.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/date_nex.hh` & `ora-0.8.2/cxx/include/ora/date_nex.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/date_type.hh` & `ora-0.8.2/cxx/include/ora/date_type.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/daytime_functions.hh` & `ora-0.8.2/cxx/include/ora/daytime_functions.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/daytime_math.hh` & `ora-0.8.2/cxx/include/ora/daytime_math.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/daytime_nex.hh` & `ora-0.8.2/cxx/include/ora/daytime_nex.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/daytime_type.hh` & `ora-0.8.2/cxx/include/ora/daytime_type.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/exceptions.hh` & `ora-0.8.2/cxx/include/ora/exceptions.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/ez.hh` & `ora-0.8.2/cxx/include/ora/ez.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/format.hh` & `ora-0.8.2/cxx/include/ora/format.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/lib/exc.hh` & `ora-0.8.2/cxx/include/ora/lib/exc.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/lib/file.hh` & `ora-0.8.2/cxx/include/ora/lib/file.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/lib/filename.hh` & `ora-0.8.2/cxx/include/ora/lib/filename.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/lib/iter.hh` & `ora-0.8.2/cxx/include/ora/lib/iter.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/lib/math.hh` & `ora-0.8.2/cxx/include/ora/lib/math.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #pragma once
 
 #include <cassert>
+#include <cstdint>
 #include <limits>
 #include <iostream>
 
 namespace ora {
 namespace lib {
 
 //------------------------------------------------------------------------------
```

### Comparing `ora-0.8.0/cxx/include/ora/lib/mem.hh` & `ora-0.8.2/cxx/include/ora/lib/mem.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/lib/num.hh` & `ora-0.8.2/cxx/include/ora/lib/num.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/lib/string.hh` & `ora-0.8.2/cxx/include/ora/lib/string.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/lib/string_builder.hh` & `ora-0.8.2/cxx/include/ora/lib/string_builder.hh`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,20 @@
     resize(hint);
   }
 
   size_t length() const { return length_; }
   operator char const*() const { return buffer_; }
   std::string str() const { return std::string(buffer_, length_); }
 
+  ~StringBuilder()
+  {
+    if (buffer_ != nullptr)
+      free(buffer_);
+  }
+
   StringBuilder&
   operator<<(
     char c)
   {
     maybe_resize(1);
     buffer_[length_++] = c;
     return *this;
```

### Comparing `ora-0.8.0/cxx/include/ora/lib/xsys.hh` & `ora-0.8.2/cxx/include/ora/lib/xsys.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/localization.hh` & `ora-0.8.2/cxx/include/ora/localization.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/localization_nex.hh` & `ora-0.8.2/cxx/include/ora/localization_nex.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/parse.hh` & `ora-0.8.2/cxx/include/ora/parse.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/posixtz.hh` & `ora-0.8.2/cxx/include/ora/posixtz.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/time_functions.hh` & `ora-0.8.2/cxx/include/ora/time_functions.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/time_interval.hh` & `ora-0.8.2/cxx/include/ora/time_interval.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/time_math.hh` & `ora-0.8.2/cxx/include/ora/time_math.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/time_nex.hh` & `ora-0.8.2/cxx/include/ora/time_nex.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/time_type.hh` & `ora-0.8.2/cxx/include/ora/time_type.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/time_zone.hh` & `ora-0.8.2/cxx/include/ora/time_zone.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/types.hh` & `ora-0.8.2/cxx/include/ora/types.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora/tzfile.hh` & `ora-0.8.2/cxx/include/ora/tzfile.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/include/ora.hh` & `ora-0.8.2/cxx/include/ora.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/bin/posixtz.cc` & `ora-0.8.2/cxx/src/bin/posixtz.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/calendar.cc` & `ora-0.8.2/cxx/src/calendar.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/date_math.cc` & `ora-0.8.2/cxx/src/date_math.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/daytime_math.cc` & `ora-0.8.2/cxx/src/daytime_math.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/file.cc` & `ora-0.8.2/cxx/src/file.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/filename.cc` & `ora-0.8.2/cxx/src/filename.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/format.cc` & `ora-0.8.2/cxx/src/format.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #include <algorithm>
 #include <cassert>
+#include <cstdint>
 #include <cstring>
 #include <iomanip>
 #include <iostream>
 
 #include "ora/lib/exc.hh"
 #include "ora/lib/string_builder.hh"
 #include "ora/format.hh"
```

### Comparing `ora-0.8.0/cxx/src/parse.cc` & `ora-0.8.2/cxx/src/parse.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/posixtz.cc` & `ora-0.8.2/cxx/src/posixtz.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/time.cc` & `ora-0.8.2/cxx/src/time.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/time_zone.cc` & `ora-0.8.2/cxx/src/time_zone.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/src/tzfile.cc` & `ora-0.8.2/cxx/src/tzfile.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/calendar.cc` & `ora-0.8.2/cxx/test/calendar.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/date.cc` & `ora-0.8.2/cxx/test/date.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/date_format.cc` & `ora-0.8.2/cxx/test/date_format.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/date_functions.cc` & `ora-0.8.2/cxx/test/date_functions.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/date_math.cc` & `ora-0.8.2/cxx/test/date_math.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/date_nex.cc` & `ora-0.8.2/cxx/test/date_nex.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/daytime.cc` & `ora-0.8.2/cxx/test/daytime.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/daytime_functions.cc` & `ora-0.8.2/cxx/test/daytime_functions.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/daytime_nex.cc` & `ora-0.8.2/cxx/test/daytime_nex.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/format.cc` & `ora-0.8.2/cxx/test/format.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/from_local.cc` & `ora-0.8.2/cxx/test/from_local.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/parse.cc` & `ora-0.8.2/cxx/test/parse.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/posixtz.cc` & `ora-0.8.2/cxx/test/posixtz.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/string_builder.cc` & `ora-0.8.2/cxx/test/string_builder.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/time.cc` & `ora-0.8.2/cxx/test/time.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/time128.cc` & `ora-0.8.2/cxx/test/time128.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/time_format.cc` & `ora-0.8.2/cxx/test/time_format.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/time_functions.cc` & `ora-0.8.2/cxx/test/time_functions.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/time_interval.cc` & `ora-0.8.2/cxx/test/time_interval.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/time_nex.cc` & `ora-0.8.2/cxx/test/time_nex.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/time_zone.cc` & `ora-0.8.2/cxx/test/time_zone.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/cxx/test/to_local.cc` & `ora-0.8.2/cxx/test/to_local.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/__init__.py` & `ora-0.8.2/python/ora/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     format_calendar, dump_calendar_file,
     get_calendar_dir, set_calendar_dir, get_calendar,
 )
 from   .ext import *
 from   .weekday import *
 from   .util import Range
 
-__version__ = "0.8.0"
+__version__ = "0.8.2"
 
 __all__ = (
     "Calendar",
 
     "Date",
     "Date16",
     "DATE_TYPES",
```

### Comparing `ora-0.8.0/python/ora/calendar.py` & `ora-0.8.2/python/ora/calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,16 @@
     """
     Gets a calendar.
 
     The name may be:
     - "all" or "none"
     - A weekday expression; see `parse_weekdays`.
     - The name of a calendar in the global calendar directory.
+
+    Calendars are not cached.
     """
     name = str(name)
     try:
         return _get_special_calendar(name)
     except LookupError:
         pass
```

### Comparing `ora-0.8.0/python/ora/calendars/usa-federal-businessdays.cal` & `ora-0.8.2/python/ora/calendars/usa-federal-businessdays.cal`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/calendars/usa-federal-holidays.cal` & `ora-0.8.2/python/ora/calendars/usa-federal-holidays.cal`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/date.py` & `ora-0.8.2/python/ora/date.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/date_expr.py` & `ora-0.8.2/python/ora/date_expr.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/daytime.py` & `ora-0.8.2/python/ora/daytime.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/functions.cc` & `ora-0.8.2/python/ora/ext/functions.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/functions.docstrings` & `ora-0.8.2/python/ora/ext/functions.docstrings`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/module.cc` & `ora-0.8.2/python/ora/ext/module.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/np.hh` & `ora-0.8.2/python/ora/ext/np.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/np_date.hh` & `ora-0.8.2/python/ora/ext/np_date.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/np_daytime.hh` & `ora-0.8.2/python/ora/ext/np_daytime.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/np_functions.cc` & `ora-0.8.2/python/ora/ext/np_functions.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/np_time.hh` & `ora-0.8.2/python/ora/ext/np_time.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/np_types.cc` & `ora-0.8.2/python/ora/ext/np_types.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/np_types.hh` & `ora-0.8.2/python/ora/ext/np_types.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py.cc` & `ora-0.8.2/python/ora/ext/py.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py.hh` & `ora-0.8.2/python/ora/ext/py.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_cal_functions.cc` & `ora-0.8.2/python/ora/ext/py_cal_functions.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_calendar.cc` & `ora-0.8.2/python/ora/ext/py_calendar.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_calendar.docstrings` & `ora-0.8.2/python/ora/ext/py_calendar.docstrings`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_calendar.hh` & `ora-0.8.2/python/ora/ext/py_calendar.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_date.cc` & `ora-0.8.2/python/ora/ext/py_date.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_date.docstrings` & `ora-0.8.2/python/ora/ext/py_date.docstrings`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_date.hh` & `ora-0.8.2/python/ora/ext/py_date.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_date_fmt.cc` & `ora-0.8.2/python/ora/ext/py_date_fmt.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_date_fmt.hh` & `ora-0.8.2/python/ora/ext/py_date_fmt.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_daytime.cc` & `ora-0.8.2/python/ora/ext/py_daytime.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_daytime.docstrings` & `ora-0.8.2/python/ora/ext/py_daytime.docstrings`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_daytime.hh` & `ora-0.8.2/python/ora/ext/py_daytime.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_daytime_inst.cc` & `ora-0.8.2/python/ora/ext/py_daytime_inst.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_local.cc` & `ora-0.8.2/python/ora/ext/py_local.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_local.hh` & `ora-0.8.2/python/ora/ext/py_local.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_time.cc` & `ora-0.8.2/python/ora/ext/py_time.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_time.docstrings` & `ora-0.8.2/python/ora/ext/py_time.docstrings`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_time.hh` & `ora-0.8.2/python/ora/ext/py_time.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_time_fmt.cc` & `ora-0.8.2/python/ora/ext/py_time_fmt.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_time_fmt.hh` & `ora-0.8.2/python/ora/ext/py_time_fmt.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_time_inst.cc` & `ora-0.8.2/python/ora/ext/py_time_inst.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_time_zone.cc` & `ora-0.8.2/python/ora/ext/py_time_zone.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/py_time_zone.hh` & `ora-0.8.2/python/ora/ext/py_time_zone.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/text.hh` & `ora-0.8.2/python/ora/ext/text.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/types.cc` & `ora-0.8.2/python/ora/ext/types.cc`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/ext/util.hh` & `ora-0.8.2/python/ora/ext/util.hh`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/np/__init__.py` & `ora-0.8.2/python/ora/np/__init__.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/data.py` & `ora-0.8.2/python/ora/test/data.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_calendar.py` & `ora-0.8.2/python/ora/test/test_calendar.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_date_basic.py` & `ora-0.8.2/python/ora/test/test_date_basic.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_date_datenum.py` & `ora-0.8.2/python/ora/test/test_date_datenum.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_date_math.py` & `ora-0.8.2/python/ora/test/test_date_math.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_date_parts.py` & `ora-0.8.2/python/ora/test/test_date_parts.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_daytime_basic.py` & `ora-0.8.2/python/ora/test/test_daytime_basic.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_fmt.py` & `ora-0.8.2/python/ora/test/test_fmt.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_from_local.py` & `ora-0.8.2/python/ora/test/test_from_local.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_functions.py` & `ora-0.8.2/python/ora/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_local.py` & `ora-0.8.2/python/ora/test/test_local.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_np_date.py` & `ora-0.8.2/python/ora/test/test_np_date.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_np_daytime.py` & `ora-0.8.2/python/ora/test/test_np_daytime.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_np_functions.py` & `ora-0.8.2/python/ora/test/test_np_functions.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_np_time.py` & `ora-0.8.2/python/ora/test/test_np_time.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_np_ufuncs_time.py` & `ora-0.8.2/python/ora/test/test_np_ufuncs_time.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_parse_date.py` & `ora-0.8.2/python/ora/test/test_parse_date.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_parse_daytime.py` & `ora-0.8.2/python/ora/test/test_parse_daytime.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_parse_time.py` & `ora-0.8.2/python/ora/test/test_parse_time.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_time_basic.py` & `ora-0.8.2/python/ora/test/test_time_basic.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_time_zone.py` & `ora-0.8.2/python/ora/test/test_time_zone.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_time_zone_dir.py` & `ora-0.8.2/python/ora/test/test_time_zone_dir.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/test/test_vs_zoneinfo.py` & `ora-0.8.2/python/ora/test/test_vs_zoneinfo.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/util.py` & `ora-0.8.2/python/ora/util.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/weekday.py` & `ora-0.8.2/python/ora/weekday.py`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Africa/Cairo` & `ora-0.8.2/python/ora/zoneinfo/Africa/Cairo`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Africa/Casablanca` & `ora-0.8.2/python/ora/zoneinfo/Africa/Casablanca`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Africa/Ceuta` & `ora-0.8.2/python/ora/zoneinfo/Africa/Ceuta`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Africa/El_Aaiun` & `ora-0.8.2/python/ora/zoneinfo/Africa/El_Aaiun`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Africa/Windhoek` & `ora-0.8.2/python/ora/zoneinfo/Africa/Windhoek`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Adak` & `ora-0.8.2/python/ora/zoneinfo/America/Adak`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Anchorage` & `ora-0.8.2/python/ora/zoneinfo/America/Anchorage`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Araguaina` & `ora-0.8.2/python/ora/zoneinfo/America/Araguaina`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Asuncion` & `ora-0.8.2/python/ora/zoneinfo/America/Asuncion`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Atka` & `ora-0.8.2/python/ora/zoneinfo/America/Atka`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Bahia` & `ora-0.8.2/python/ora/zoneinfo/America/Bahia`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Bahia_Banderas` & `ora-0.8.2/python/ora/zoneinfo/America/Bahia_Banderas`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Belize` & `ora-0.8.2/python/ora/zoneinfo/America/Belize`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Boise` & `ora-0.8.2/python/ora/zoneinfo/America/Boise`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Buenos_Aires` & `ora-0.8.2/python/ora/zoneinfo/America/Buenos_Aires`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Cambridge_Bay` & `ora-0.8.2/python/ora/zoneinfo/America/Cambridge_Bay`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Campo_Grande` & `ora-0.8.2/python/ora/zoneinfo/America/Campo_Grande`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Cancun` & `ora-0.8.2/python/ora/zoneinfo/America/Cancun`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Catamarca` & `ora-0.8.2/python/ora/zoneinfo/America/Catamarca`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Chicago` & `ora-0.8.2/python/ora/zoneinfo/America/Chicago`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Chihuahua` & `ora-0.8.2/python/ora/zoneinfo/America/Chihuahua`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Ciudad_Juarez` & `ora-0.8.2/python/ora/zoneinfo/America/Ciudad_Juarez`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Cordoba` & `ora-0.8.2/python/ora/zoneinfo/America/Cordoba`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Cuiaba` & `ora-0.8.2/python/ora/zoneinfo/America/Cuiaba`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Dawson` & `ora-0.8.2/python/ora/zoneinfo/America/Dawson`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Dawson_Creek` & `ora-0.8.2/python/ora/zoneinfo/America/Dawson_Creek`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Denver` & `ora-0.8.2/python/ora/zoneinfo/America/Denver`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Detroit` & `ora-0.8.2/python/ora/zoneinfo/America/Detroit`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Edmonton` & `ora-0.8.2/python/ora/zoneinfo/America/Edmonton`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Ensenada` & `ora-0.8.2/python/ora/zoneinfo/America/Ensenada`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Fort_Nelson` & `ora-0.8.2/python/ora/zoneinfo/America/Fort_Nelson`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Fort_Wayne` & `ora-0.8.2/python/ora/zoneinfo/America/Fort_Wayne`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Glace_Bay` & `ora-0.8.2/python/ora/zoneinfo/America/Glace_Bay`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Godthab` & `ora-0.8.2/python/ora/zoneinfo/America/Godthab`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Goose_Bay` & `ora-0.8.2/python/ora/zoneinfo/America/Goose_Bay`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Grand_Turk` & `ora-0.8.2/python/ora/zoneinfo/America/Grand_Turk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Halifax` & `ora-0.8.2/python/ora/zoneinfo/America/Halifax`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Havana` & `ora-0.8.2/python/ora/zoneinfo/America/Havana`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Indianapolis` & `ora-0.8.2/python/ora/zoneinfo/America/Indianapolis`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Inuvik` & `ora-0.8.2/python/ora/zoneinfo/America/Inuvik`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Iqaluit` & `ora-0.8.2/python/ora/zoneinfo/America/Iqaluit`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Jujuy` & `ora-0.8.2/python/ora/zoneinfo/America/Jujuy`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Juneau` & `ora-0.8.2/python/ora/zoneinfo/America/Juneau`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Knox_IN` & `ora-0.8.2/python/ora/zoneinfo/America/Knox_IN`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Los_Angeles` & `ora-0.8.2/python/ora/zoneinfo/America/Los_Angeles`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Louisville` & `ora-0.8.2/python/ora/zoneinfo/America/Louisville`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Mazatlan` & `ora-0.8.2/python/ora/zoneinfo/America/Mazatlan`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Mendoza` & `ora-0.8.2/python/ora/zoneinfo/America/Mendoza`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Menominee` & `ora-0.8.2/python/ora/zoneinfo/America/Menominee`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Merida` & `ora-0.8.2/python/ora/zoneinfo/America/Merida`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Metlakatla` & `ora-0.8.2/python/ora/zoneinfo/America/Metlakatla`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Mexico_City` & `ora-0.8.2/python/ora/zoneinfo/America/Mexico_City`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Miquelon` & `ora-0.8.2/python/ora/zoneinfo/America/Miquelon`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Moncton` & `ora-0.8.2/python/ora/zoneinfo/America/Moncton`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Monterrey` & `ora-0.8.2/python/ora/zoneinfo/America/Monterrey`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Montevideo` & `ora-0.8.2/python/ora/zoneinfo/America/Montevideo`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Montreal` & `ora-0.8.2/python/ora/zoneinfo/America/Montreal`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Nassau` & `ora-0.8.2/python/ora/zoneinfo/America/Nassau`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/New_York` & `ora-0.8.2/python/ora/zoneinfo/America/New_York`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Nipigon` & `ora-0.8.2/python/ora/zoneinfo/America/Nipigon`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Nome` & `ora-0.8.2/python/ora/zoneinfo/America/Nome`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Nuuk` & `ora-0.8.2/python/ora/zoneinfo/America/Nuuk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Ojinaga` & `ora-0.8.2/python/ora/zoneinfo/America/Ojinaga`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Pangnirtung` & `ora-0.8.2/python/ora/zoneinfo/America/Pangnirtung`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Port-au-Prince` & `ora-0.8.2/python/ora/zoneinfo/America/Port-au-Prince`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Punta_Arenas` & `ora-0.8.2/python/ora/zoneinfo/America/Punta_Arenas`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Rainy_River` & `ora-0.8.2/python/ora/zoneinfo/America/Rainy_River`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Rankin_Inlet` & `ora-0.8.2/python/ora/zoneinfo/America/Rankin_Inlet`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Regina` & `ora-0.8.2/python/ora/zoneinfo/America/Regina`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Resolute` & `ora-0.8.2/python/ora/zoneinfo/America/Resolute`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Rosario` & `ora-0.8.2/python/ora/zoneinfo/America/Rosario`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Santa_Isabel` & `ora-0.8.2/python/ora/zoneinfo/America/Santa_Isabel`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Santiago` & `ora-0.8.2/python/ora/zoneinfo/America/Santiago`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Sao_Paulo` & `ora-0.8.2/python/ora/zoneinfo/America/Sao_Paulo`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Shiprock` & `ora-0.8.2/python/ora/zoneinfo/America/Shiprock`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Sitka` & `ora-0.8.2/python/ora/zoneinfo/America/Sitka`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/St_Johns` & `ora-0.8.2/python/ora/zoneinfo/America/St_Johns`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Thunder_Bay` & `ora-0.8.2/python/ora/zoneinfo/America/Thunder_Bay`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Tijuana` & `ora-0.8.2/python/ora/zoneinfo/America/Tijuana`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Toronto` & `ora-0.8.2/python/ora/zoneinfo/America/Toronto`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Vancouver` & `ora-0.8.2/python/ora/zoneinfo/America/Vancouver`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Whitehorse` & `ora-0.8.2/python/ora/zoneinfo/America/Whitehorse`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Winnipeg` & `ora-0.8.2/python/ora/zoneinfo/America/Winnipeg`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Yakutat` & `ora-0.8.2/python/ora/zoneinfo/America/Yakutat`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/America/Yellowknife` & `ora-0.8.2/python/ora/zoneinfo/America/Yellowknife`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Antarctica/Macquarie` & `ora-0.8.2/python/ora/zoneinfo/Antarctica/Macquarie`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Antarctica/McMurdo` & `ora-0.8.2/python/ora/zoneinfo/Antarctica/McMurdo`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Antarctica/Palmer` & `ora-0.8.2/python/ora/zoneinfo/Antarctica/Palmer`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Antarctica/South_Pole` & `ora-0.8.2/python/ora/zoneinfo/Antarctica/South_Pole`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Arctic/Longyearbyen` & `ora-0.8.2/python/ora/zoneinfo/Arctic/Longyearbyen`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Almaty` & `ora-0.8.2/python/ora/zoneinfo/Asia/Almaty`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Amman` & `ora-0.8.2/python/ora/zoneinfo/Asia/Amman`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Anadyr` & `ora-0.8.2/python/ora/zoneinfo/Asia/Anadyr`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Aqtau` & `ora-0.8.2/python/ora/zoneinfo/Asia/Aqtau`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Aqtobe` & `ora-0.8.2/python/ora/zoneinfo/Asia/Aqtobe`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Atyrau` & `ora-0.8.2/python/ora/zoneinfo/Asia/Atyrau`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Baghdad` & `ora-0.8.2/python/ora/zoneinfo/Asia/Baghdad`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Baku` & `ora-0.8.2/python/ora/zoneinfo/Asia/Baku`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Barnaul` & `ora-0.8.2/python/ora/zoneinfo/Asia/Barnaul`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Beirut` & `ora-0.8.2/python/ora/zoneinfo/Asia/Beirut`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Bishkek` & `ora-0.8.2/python/ora/zoneinfo/Asia/Bishkek`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Chita` & `ora-0.8.2/python/ora/zoneinfo/Asia/Chita`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Choibalsan` & `ora-0.8.2/python/ora/zoneinfo/Asia/Choibalsan`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Damascus` & `ora-0.8.2/python/ora/zoneinfo/Asia/Damascus`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Famagusta` & `ora-0.8.2/python/ora/zoneinfo/Asia/Famagusta`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Gaza` & `ora-0.8.2/python/ora/zoneinfo/Asia/Gaza`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Hebron` & `ora-0.8.2/python/ora/zoneinfo/Asia/Hebron`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Hong_Kong` & `ora-0.8.2/python/ora/zoneinfo/Asia/Hong_Kong`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Hovd` & `ora-0.8.2/python/ora/zoneinfo/Asia/Hovd`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Irkutsk` & `ora-0.8.2/python/ora/zoneinfo/Asia/Irkutsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Istanbul` & `ora-0.8.2/python/ora/zoneinfo/Asia/Istanbul`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Jerusalem` & `ora-0.8.2/python/ora/zoneinfo/Asia/Jerusalem`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Kamchatka` & `ora-0.8.2/python/ora/zoneinfo/Asia/Kamchatka`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Khandyga` & `ora-0.8.2/python/ora/zoneinfo/Asia/Khandyga`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Krasnoyarsk` & `ora-0.8.2/python/ora/zoneinfo/Asia/Krasnoyarsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Macao` & `ora-0.8.2/python/ora/zoneinfo/Asia/Macao`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Macau` & `ora-0.8.2/python/ora/zoneinfo/Asia/Macau`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Magadan` & `ora-0.8.2/python/ora/zoneinfo/Asia/Magadan`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Nicosia` & `ora-0.8.2/python/ora/zoneinfo/Asia/Nicosia`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Novokuznetsk` & `ora-0.8.2/python/ora/zoneinfo/Asia/Novokuznetsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Novosibirsk` & `ora-0.8.2/python/ora/zoneinfo/Asia/Novosibirsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Omsk` & `ora-0.8.2/python/ora/zoneinfo/Asia/Omsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Oral` & `ora-0.8.2/python/ora/zoneinfo/Asia/Oral`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Qostanay` & `ora-0.8.2/python/ora/zoneinfo/Asia/Qostanay`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Qyzylorda` & `ora-0.8.2/python/ora/zoneinfo/Asia/Qyzylorda`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Sakhalin` & `ora-0.8.2/python/ora/zoneinfo/Asia/Sakhalin`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Srednekolymsk` & `ora-0.8.2/python/ora/zoneinfo/Asia/Srednekolymsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Tbilisi` & `ora-0.8.2/python/ora/zoneinfo/Asia/Tbilisi`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Tehran` & `ora-0.8.2/python/ora/zoneinfo/Asia/Tehran`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Tel_Aviv` & `ora-0.8.2/python/ora/zoneinfo/Asia/Tel_Aviv`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Tomsk` & `ora-0.8.2/python/ora/zoneinfo/Asia/Tomsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Ulaanbaatar` & `ora-0.8.2/python/ora/zoneinfo/Asia/Ulaanbaatar`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Ulan_Bator` & `ora-0.8.2/python/ora/zoneinfo/Asia/Ulan_Bator`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Ust-Nera` & `ora-0.8.2/python/ora/zoneinfo/Asia/Ust-Nera`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Vladivostok` & `ora-0.8.2/python/ora/zoneinfo/Asia/Vladivostok`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Yakutsk` & `ora-0.8.2/python/ora/zoneinfo/Asia/Yakutsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Yekaterinburg` & `ora-0.8.2/python/ora/zoneinfo/Asia/Yekaterinburg`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Asia/Yerevan` & `ora-0.8.2/python/ora/zoneinfo/Asia/Yerevan`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Atlantic/Azores` & `ora-0.8.2/python/ora/zoneinfo/Atlantic/Azores`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Atlantic/Bermuda` & `ora-0.8.2/python/ora/zoneinfo/Atlantic/Bermuda`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Atlantic/Jan_Mayen` & `ora-0.8.2/python/ora/zoneinfo/Atlantic/Jan_Mayen`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Atlantic/Madeira` & `ora-0.8.2/python/ora/zoneinfo/Atlantic/Madeira`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Atlantic/Stanley` & `ora-0.8.2/python/ora/zoneinfo/Atlantic/Stanley`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/ACT` & `ora-0.8.2/python/ora/zoneinfo/Australia/ACT`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Adelaide` & `ora-0.8.2/python/ora/zoneinfo/Australia/Adelaide`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Broken_Hill` & `ora-0.8.2/python/ora/zoneinfo/Australia/Broken_Hill`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Canberra` & `ora-0.8.2/python/ora/zoneinfo/Australia/Canberra`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Currie` & `ora-0.8.2/python/ora/zoneinfo/Australia/Currie`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Hobart` & `ora-0.8.2/python/ora/zoneinfo/Australia/Hobart`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/LHI` & `ora-0.8.2/python/ora/zoneinfo/Australia/LHI`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Lord_Howe` & `ora-0.8.2/python/ora/zoneinfo/Australia/Lord_Howe`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Melbourne` & `ora-0.8.2/python/ora/zoneinfo/Australia/Melbourne`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/NSW` & `ora-0.8.2/python/ora/zoneinfo/Australia/NSW`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/South` & `ora-0.8.2/python/ora/zoneinfo/Australia/South`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Sydney` & `ora-0.8.2/python/ora/zoneinfo/Australia/Sydney`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Tasmania` & `ora-0.8.2/python/ora/zoneinfo/Australia/Tasmania`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Victoria` & `ora-0.8.2/python/ora/zoneinfo/Australia/Victoria`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Australia/Yancowinna` & `ora-0.8.2/python/ora/zoneinfo/Australia/Yancowinna`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Brazil/East` & `ora-0.8.2/python/ora/zoneinfo/Brazil/East`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/CET` & `ora-0.8.2/python/ora/zoneinfo/CET`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/CST6CDT` & `ora-0.8.2/python/ora/zoneinfo/CST6CDT`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Canada/Atlantic` & `ora-0.8.2/python/ora/zoneinfo/Canada/Atlantic`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Canada/Central` & `ora-0.8.2/python/ora/zoneinfo/Canada/Central`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Canada/Eastern` & `ora-0.8.2/python/ora/zoneinfo/Canada/Eastern`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Canada/Mountain` & `ora-0.8.2/python/ora/zoneinfo/Canada/Mountain`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Canada/Newfoundland` & `ora-0.8.2/python/ora/zoneinfo/Canada/Newfoundland`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Canada/Pacific` & `ora-0.8.2/python/ora/zoneinfo/Canada/Pacific`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Canada/Saskatchewan` & `ora-0.8.2/python/ora/zoneinfo/Canada/Saskatchewan`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Canada/Yukon` & `ora-0.8.2/python/ora/zoneinfo/Canada/Yukon`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Chile/Continental` & `ora-0.8.2/python/ora/zoneinfo/Chile/Continental`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Chile/EasterIsland` & `ora-0.8.2/python/ora/zoneinfo/Chile/EasterIsland`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Cuba` & `ora-0.8.2/python/ora/zoneinfo/Cuba`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/EST5EDT` & `ora-0.8.2/python/ora/zoneinfo/EST5EDT`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Egypt` & `ora-0.8.2/python/ora/zoneinfo/Egypt`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Eire` & `ora-0.8.2/python/ora/zoneinfo/Eire`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Amsterdam` & `ora-0.8.2/python/ora/zoneinfo/Europe/Amsterdam`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Astrakhan` & `ora-0.8.2/python/ora/zoneinfo/Europe/Astrakhan`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Athens` & `ora-0.8.2/python/ora/zoneinfo/Europe/Athens`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Belfast` & `ora-0.8.2/python/ora/zoneinfo/Europe/Belfast`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Berlin` & `ora-0.8.2/python/ora/zoneinfo/Europe/Berlin`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Bratislava` & `ora-0.8.2/python/ora/zoneinfo/Europe/Bratislava`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Brussels` & `ora-0.8.2/python/ora/zoneinfo/Europe/Brussels`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Bucharest` & `ora-0.8.2/python/ora/zoneinfo/Europe/Bucharest`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Budapest` & `ora-0.8.2/python/ora/zoneinfo/Europe/Budapest`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Chisinau` & `ora-0.8.2/python/ora/zoneinfo/Europe/Chisinau`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Copenhagen` & `ora-0.8.2/python/ora/zoneinfo/Europe/Copenhagen`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Dublin` & `ora-0.8.2/python/ora/zoneinfo/Europe/Dublin`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Gibraltar` & `ora-0.8.2/python/ora/zoneinfo/Europe/Gibraltar`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Guernsey` & `ora-0.8.2/python/ora/zoneinfo/Europe/Guernsey`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Isle_of_Man` & `ora-0.8.2/python/ora/zoneinfo/Europe/Isle_of_Man`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Istanbul` & `ora-0.8.2/python/ora/zoneinfo/Europe/Istanbul`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Jersey` & `ora-0.8.2/python/ora/zoneinfo/Europe/Jersey`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Kaliningrad` & `ora-0.8.2/python/ora/zoneinfo/Europe/Kaliningrad`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Kiev` & `ora-0.8.2/python/ora/zoneinfo/Europe/Kiev`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Kirov` & `ora-0.8.2/python/ora/zoneinfo/Europe/Kirov`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Kyiv` & `ora-0.8.2/python/ora/zoneinfo/Europe/Kyiv`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Lisbon` & `ora-0.8.2/python/ora/zoneinfo/Europe/Lisbon`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/London` & `ora-0.8.2/python/ora/zoneinfo/Europe/London`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Luxembourg` & `ora-0.8.2/python/ora/zoneinfo/Europe/Luxembourg`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Madrid` & `ora-0.8.2/python/ora/zoneinfo/Europe/Madrid`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Malta` & `ora-0.8.2/python/ora/zoneinfo/Europe/Malta`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Minsk` & `ora-0.8.2/python/ora/zoneinfo/Europe/Minsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Monaco` & `ora-0.8.2/python/ora/zoneinfo/Europe/Monaco`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Moscow` & `ora-0.8.2/python/ora/zoneinfo/Europe/Moscow`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Nicosia` & `ora-0.8.2/python/ora/zoneinfo/Europe/Nicosia`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Oslo` & `ora-0.8.2/python/ora/zoneinfo/Europe/Oslo`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Paris` & `ora-0.8.2/python/ora/zoneinfo/Europe/Paris`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Prague` & `ora-0.8.2/python/ora/zoneinfo/Europe/Prague`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Riga` & `ora-0.8.2/python/ora/zoneinfo/Europe/Riga`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Rome` & `ora-0.8.2/python/ora/zoneinfo/Europe/Rome`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Samara` & `ora-0.8.2/python/ora/zoneinfo/Europe/Samara`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/San_Marino` & `ora-0.8.2/python/ora/zoneinfo/Europe/San_Marino`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Saratov` & `ora-0.8.2/python/ora/zoneinfo/Europe/Saratov`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Simferopol` & `ora-0.8.2/python/ora/zoneinfo/Europe/Simferopol`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Sofia` & `ora-0.8.2/python/ora/zoneinfo/Europe/Sofia`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Stockholm` & `ora-0.8.2/python/ora/zoneinfo/Europe/Stockholm`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Tallinn` & `ora-0.8.2/python/ora/zoneinfo/Europe/Tallinn`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Tirane` & `ora-0.8.2/python/ora/zoneinfo/Europe/Tirane`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Tiraspol` & `ora-0.8.2/python/ora/zoneinfo/Europe/Tiraspol`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Ulyanovsk` & `ora-0.8.2/python/ora/zoneinfo/Europe/Ulyanovsk`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Uzhgorod` & `ora-0.8.2/python/ora/zoneinfo/Europe/Uzhgorod`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Vatican` & `ora-0.8.2/python/ora/zoneinfo/Europe/Vatican`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Vienna` & `ora-0.8.2/python/ora/zoneinfo/Europe/Vienna`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Vilnius` & `ora-0.8.2/python/ora/zoneinfo/Europe/Vilnius`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Volgograd` & `ora-0.8.2/python/ora/zoneinfo/Europe/Volgograd`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Warsaw` & `ora-0.8.2/python/ora/zoneinfo/Europe/Warsaw`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Europe/Zaporozhye` & `ora-0.8.2/python/ora/zoneinfo/Europe/Zaporozhye`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/GB` & `ora-0.8.2/python/ora/zoneinfo/GB`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/GB-Eire` & `ora-0.8.2/python/ora/zoneinfo/GB-Eire`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Hongkong` & `ora-0.8.2/python/ora/zoneinfo/Hongkong`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Iran` & `ora-0.8.2/python/ora/zoneinfo/Iran`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Israel` & `ora-0.8.2/python/ora/zoneinfo/Israel`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/MET` & `ora-0.8.2/python/ora/zoneinfo/MET`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/MST7MDT` & `ora-0.8.2/python/ora/zoneinfo/MST7MDT`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Mexico/BajaNorte` & `ora-0.8.2/python/ora/zoneinfo/Mexico/BajaNorte`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Mexico/BajaSur` & `ora-0.8.2/python/ora/zoneinfo/Mexico/BajaSur`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Mexico/General` & `ora-0.8.2/python/ora/zoneinfo/Mexico/General`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/NZ` & `ora-0.8.2/python/ora/zoneinfo/NZ`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/NZ-CHAT` & `ora-0.8.2/python/ora/zoneinfo/NZ-CHAT`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Navajo` & `ora-0.8.2/python/ora/zoneinfo/Navajo`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/PST8PDT` & `ora-0.8.2/python/ora/zoneinfo/PST8PDT`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Pacific/Auckland` & `ora-0.8.2/python/ora/zoneinfo/Pacific/Auckland`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Pacific/Chatham` & `ora-0.8.2/python/ora/zoneinfo/Pacific/Chatham`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Pacific/Easter` & `ora-0.8.2/python/ora/zoneinfo/Pacific/Easter`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Poland` & `ora-0.8.2/python/ora/zoneinfo/Poland`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Portugal` & `ora-0.8.2/python/ora/zoneinfo/Portugal`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/Turkey` & `ora-0.8.2/python/ora/zoneinfo/Turkey`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/US/Alaska` & `ora-0.8.2/python/ora/zoneinfo/US/Alaska`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/US/Aleutian` & `ora-0.8.2/python/ora/zoneinfo/US/Aleutian`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/US/Central` & `ora-0.8.2/python/ora/zoneinfo/US/Central`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/US/East-Indiana` & `ora-0.8.2/python/ora/zoneinfo/US/East-Indiana`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/US/Eastern` & `ora-0.8.2/python/ora/zoneinfo/US/Eastern`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/US/Indiana-Starke` & `ora-0.8.2/python/ora/zoneinfo/US/Indiana-Starke`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/US/Michigan` & `ora-0.8.2/python/ora/zoneinfo/US/Michigan`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/US/Mountain` & `ora-0.8.2/python/ora/zoneinfo/US/Mountain`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/US/Pacific` & `ora-0.8.2/python/ora/zoneinfo/US/Pacific`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/W-SU` & `ora-0.8.2/python/ora/zoneinfo/W-SU`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/iso3166.tab` & `ora-0.8.2/python/ora/zoneinfo/iso3166.tab`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/leapseconds` & `ora-0.8.2/python/ora/zoneinfo/leapseconds`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/tzdata.zi` & `ora-0.8.2/python/ora/zoneinfo/tzdata.zi`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/zone.tab` & `ora-0.8.2/python/ora/zoneinfo/zone.tab`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora/zoneinfo/zone1970.tab` & `ora-0.8.2/python/ora/zoneinfo/zone1970.tab`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/ora.egg-info/PKG-INFO` & `ora-0.8.2/python/ora.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ora
-Version: 0.8.0
+Version: 0.8.2
 Summary: Alternative time and date library
 Home-page: https://github.com/alexhsamuel/ora
 Author: Alex Samuel
 Author-email: alexhsamuel@gmail.com
 License: BSD-3
 Keywords: time,date,time zone
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 License-File: LICENSE
@@ -20,9 +19,7 @@
 Ora is a freestanding time and date implementation for C++ and Python.
 
 Ora is `hosted on GitHub <http://github.com/alexhsamuel/ora>`_.  See
 the `installation instructions
 <https://github.com/alexhsamuel/ora/blob/master/README.md#installation>`_.
 
 Docs at `readthedocs <http://ora.readthedocs.io/en/latest/>`_.
-
-
```

### Comparing `ora-0.8.0/python/ora.egg-info/SOURCES.txt` & `ora-0.8.2/python/ora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/python/wrap_docstrings` & `ora-0.8.2/python/wrap_docstrings`

 * *Files identical despite different names*

### Comparing `ora-0.8.0/setup.py` & `ora-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     for dir, _, files in os.walk(dir):
         yield dir, [ os.path.join(dir, f) for f in files ]
 
 
 setup(
     name            ="ora",
-    version         ="0.8.0",
+    version         ="0.8.2",
     description     ="Alternative time and date library",
     long_description=__doc__,
     url             ="https://github.com/alexhsamuel/ora",
     author          ="Alex Samuel",
     author_email    ="alexhsamuel@gmail.com",
     license         ="BSD-3",
     keywords        =["time", "date", "time zone"],
```

