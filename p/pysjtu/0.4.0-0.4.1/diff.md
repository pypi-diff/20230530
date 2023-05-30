# Comparing `tmp/pysjtu-0.4.0.tar.gz` & `tmp/pysjtu-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysjtu-0.4.0.tar", last modified: Sun Jan 15 01:45:11 2023, max compression
+gzip compressed data, was "pysjtu-0.4.1.tar", last modified: Tue May 30 09:14:22 2023, max compression
```

## Comparing `pysjtu-0.4.0.tar` & `pysjtu-0.4.1.tar`

### file list

```diff
@@ -1,93 +1,87 @@
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-01-15 01:44:42.104973 pysjtu-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-01-15 01:44:42.104973 pysjtu-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/api/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/api/exam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/api/gpa.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/api/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/api/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/api/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/models/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/models/exam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/models/gpa.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/models/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/models/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-01-15 01:44:42.108973 pysjtu-0.4.0/pysjtu/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1132534 2023-01-15 01:44:42.116973 pysjtu-0.4.0/pysjtu/ocr/nn_model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)  2756190 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/ocr/svm_model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/parser/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/parser/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/schemas/course.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/schemas/exam.py
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/schemas/gpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/schemas/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/schemas/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/schemas/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/schemas/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-01-15 01:44:42.124973 pysjtu-0.4.0/pysjtu/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/captcha/aoaiq.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/captcha/cqmzn.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/captcha/ghwty.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/captcha/mfobv.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/captcha/pisv.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/exam.json
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/gpa.json
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/gpa_query_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/lib_course_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/lib_course_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/schedule_course_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/schedule_course_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/score.json
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/score_factor.json
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/selection_class.json
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/selection_course.json
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/selection_sector.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/resp/selection_shared_info.json
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/cjcx_cxDgXscj.html
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/cjcx_cxXsXmcjList.html
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/common_cxGnzdxxList.html
--rw-r--r--   0 runner    (1001) docker     (123)    43791 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/funcData_cxFuncDataList_1.html
--rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/funcData_cxFuncDataList_2.html
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/funcData_cxFuncDataList_3.html
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/funcData_cxFuncDataList_initial.html
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/gpapmtj_cxGpaxjfcxIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/gpapmtj_tjGpapmtj.html
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/gpapmtj_tjGpapmtj_failure.html
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/gpapmtj_tjGpapmtj_unauthorized.html
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/index_cxshjdAreaFive.html
--rw-r--r--   0 runner    (1001) docker     (123)    22788 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/index_initMenu.html
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/jalogin
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/kscx_cxXsksxxIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/login_slogin.html
--rw-r--r--   0 runner    (1001) docker     (123)    36136 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/xsgrxxwh_cxXsgrxx.html
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/xskbcx_cxXsKb.html
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxJxbWithKchZzxkYzb.html
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxZzxkYzbDisplay.html
--rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxZzxkYzbIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxZzxkYzbIndex_not_selecting.html
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxZzxkYzbPartDisplay.html
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11589 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/test_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-01-15 01:44:42.124973 pysjtu-0.4.0/tests/test_utils.py
--rw-------   0 runner    (1001) docker     (123)     4049 2023-01-15 01:45:11.549348 pysjtu-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-05-30 09:13:51.019681 pysjtu-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3286 2023-05-30 09:13:51.019681 pysjtu-0.4.1/README.md
+-rw-r--r--   0        0        0     1469 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      216 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/__init__.py
+-rw-r--r--   0        0        0     2862 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/__init__.py
+-rw-r--r--   0        0        0      227 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/api/__init__.py
+-rw-r--r--   0        0        0     2169 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/api/course.py
+-rw-r--r--   0        0        0     1201 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/api/exam.py
+-rw-r--r--   0        0        0     2625 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/api/gpa.py
+-rw-r--r--   0        0        0      680 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/api/profile.py
+-rw-r--r--   0        0        0      768 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/api/schedule.py
+-rw-r--r--   0        0        0     1895 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/api/score.py
+-rw-r--r--   0        0        0     6915 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/api/selection.py
+-rw-r--r--   0        0        0      168 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/client/base.py
+-rw-r--r--   0        0        0     2112 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/consts.py
+-rw-r--r--   0        0        0     1399 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/exceptions.py
+-rw-r--r--   0        0        0     2995 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/fields.py
+-rw-r--r--   0        0        0      397 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/__init__.py
+-rw-r--r--   0        0        0     7365 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/base.py
+-rw-r--r--   0        0        0      145 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/common.py
+-rw-r--r--   0        0        0     3524 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/course.py
+-rw-r--r--   0        0        0     3278 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/exam.py
+-rw-r--r--   0        0        0    10928 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/gpa.py
+-rw-r--r--   0        0        0      930 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/profile.py
+-rw-r--r--   0        0        0     3562 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/schedule.py
+-rw-r--r--   0        0        0     5237 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/score.py
+-rw-r--r--   0        0        0    10622 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/models/selection.py
+-rw-r--r--   0        0        0     8263 2023-05-30 09:13:51.023681 pysjtu-0.4.1/pysjtu/ocr/__init__.py
+-rw-r--r--   0        0        0  1132534 2023-05-30 09:13:51.031681 pysjtu-0.4.1/pysjtu/ocr/nn_model.onnx
+-rw-r--r--   0        0        0  2756190 2023-05-30 09:13:51.039682 pysjtu-0.4.1/pysjtu/ocr/svm_model.onnx
+-rw-r--r--   0        0        0        0 2023-05-30 09:13:51.039682 pysjtu-0.4.1/pysjtu/parser/__init__.py
+-rw-r--r--   0        0        0     4700 2023-05-30 09:13:51.039682 pysjtu-0.4.1/pysjtu/parser/profile.py
+-rw-r--r--   0        0        0     1519 2023-05-30 09:13:51.039682 pysjtu-0.4.1/pysjtu/parser/selection.py
+-rw-r--r--   0        0        0     4089 2023-05-30 09:13:51.039682 pysjtu-0.4.1/pysjtu/schema.py
+-rw-r--r--   0        0        0    19060 2023-05-30 09:13:51.039682 pysjtu-0.4.1/pysjtu/session.py
+-rw-r--r--   0        0        0     3110 2023-05-30 09:13:51.039682 pysjtu-0.4.1/pysjtu/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0    12875 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/mock_server.py
+-rw-r--r--   0        0        0     1564 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/captcha/aoaiq.jpeg
+-rw-r--r--   0        0        0     1360 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/captcha/cqmzn.jpeg
+-rw-r--r--   0        0        0     1635 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/captcha/ghwty.jpeg
+-rw-r--r--   0        0        0     1467 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/captcha/mfobv.jpeg
+-rw-r--r--   0        0        0     1347 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/captcha/pisv.jpeg
+-rw-r--r--   0        0        0      887 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/exam.json
+-rw-r--r--   0        0        0      503 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/gpa.json
+-rw-r--r--   0        0        0     2108 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/gpa_query_params.json
+-rw-r--r--   0        0        0     1055 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/lib_course_1.json
+-rw-r--r--   0        0        0     1079 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/lib_course_2.json
+-rw-r--r--   0        0        0     1446 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/schedule_course_1.json
+-rw-r--r--   0        0        0     1832 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/schedule_course_2.json
+-rw-r--r--   0        0        0     1664 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/score.json
+-rw-r--r--   0        0        0     1659 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/score_factor.json
+-rw-r--r--   0        0        0     1419 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/selection_class.json
+-rw-r--r--   0        0        0      992 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/selection_course.json
+-rw-r--r--   0        0        0      173 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/selection_sector.json
+-rw-r--r--   0        0        0      225 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/resp/selection_shared_info.json
+-rw-r--r--   0        0        0     4250 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/cjcx_cxDgXscj.html
+-rw-r--r--   0        0        0     1920 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/cjcx_cxXsXmcjList.html
+-rw-r--r--   0        0        0     1510 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/common_cxGnzdxxList.html
+-rw-r--r--   0        0        0    43791 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/funcData_cxFuncDataList_1.html
+-rw-r--r--   0        0        0    39893 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/funcData_cxFuncDataList_2.html
+-rw-r--r--   0        0        0     9319 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/funcData_cxFuncDataList_3.html
+-rw-r--r--   0        0        0     1115 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/funcData_cxFuncDataList_initial.html
+-rw-r--r--   0        0        0      622 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/gpapmtj_cxGpaxjfcxIndex.html
+-rw-r--r--   0        0        0       17 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/gpapmtj_tjGpapmtj.html
+-rw-r--r--   0        0        0       17 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/gpapmtj_tjGpapmtj_failure.html
+-rw-r--r--   0        0        0     2390 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/gpapmtj_tjGpapmtj_unauthorized.html
+-rw-r--r--   0        0        0    16109 2023-05-30 09:13:51.039682 pysjtu-0.4.1/tests/resources/website/index_cxshjdAreaFive.html
+-rw-r--r--   0        0        0    22788 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/index_initMenu.html
+-rw-r--r--   0        0        0    20030 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/jalogin
+-rw-r--r--   0        0        0     2546 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/kscx_cxXsksxxIndex.html
+-rw-r--r--   0        0        0     9978 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/login_slogin.html
+-rw-r--r--   0        0        0    36136 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/xsgrxxwh_cxXsgrxx.html
+-rw-r--r--   0        0        0     4144 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/xskbcx_cxXsKb.html
+-rw-r--r--   0        0        0     1212 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxJxbWithKchZzxkYzb.html
+-rw-r--r--   0        0        0     4451 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxZzxkYzbDisplay.html
+-rw-r--r--   0        0        0    20009 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxZzxkYzbIndex.html
+-rw-r--r--   0        0        0    13550 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxZzxkYzbIndex_not_selecting.html
+-rw-r--r--   0        0        0      799 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxZzxkYzbPartDisplay.html
+-rw-r--r--   0        0        0    13455 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/test_api.py
+-rw-r--r--   0        0        0    11493 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/test_model.py
+-rw-r--r--   0        0        0     1329 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/test_ocr.py
+-rw-r--r--   0        0        0     3273 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/test_parser.py
+-rw-r--r--   0        0        0    14774 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/test_schema.py
+-rw-r--r--   0        0        0     3299 2023-05-30 09:13:51.043682 pysjtu-0.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 pysjtu-0.4.1/PKG-INFO
```

### Comparing `pysjtu-0.4.0/LICENSE` & `pysjtu-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/README.md` & `pysjtu-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/pyproject.toml` & `pysjtu-0.4.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,25 +6,26 @@
     { name = "LightQuantum", email = "self@lightquantum.me" },
 ]
 dependencies = [
     "marshmallow>=3.19.0",
     "lxml>=4.9.2",
     "httpx>=0.23.3",
     "importlib-resources>=5.10.2; python_version < \"3.9\"",
+    "marshmallow-dataclass>=8.5.11",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     "Operating System :: OS Independent",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.4.0"
+version = "0.4.1"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 homepage = "https://github.com/PhotonQuantum/pysjtu"
 repository = "https://github.com/PhotonQuantum/pysjtu"
```

### Comparing `pysjtu-0.4.0/pysjtu/client/__init__.py` & `pysjtu-0.4.1/pysjtu/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/pysjtu/client/api/course.py` & `pysjtu-0.4.1/pysjtu/client/api/course.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from functools import partial
 
 from pysjtu import consts
 from pysjtu import models
-from pysjtu import schemas
 from pysjtu.client.base import BaseClient
 from pysjtu.utils import range_list_to_str, schema_post_loader
 
 
 class CourseLibMixin(BaseClient):
     def __init__(self):
         super().__init__()
@@ -40,9 +39,9 @@
         req_params = {}
         for (k, v) in _args.items():
             if k in dir():
                 req_params[v] = locals()[k]
 
         req = partial(self._session.post, consts.COURSELIB_URL + str(self.student_id), **kwargs)
 
-        return models.QueryResult(req, partial(schema_post_loader, schemas.LibCourseSchema), req_params,
+        return models.QueryResult(req, partial(schema_post_loader, models.LibCourse.Schema), req_params,
                                   page_size=page_size)
```

### Comparing `pysjtu-0.4.0/pysjtu/client/api/exam.py` & `pysjtu-0.4.1/pysjtu/client/api/exam.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/pysjtu/client/api/gpa.py` & `pysjtu-0.4.1/pysjtu/client/api/gpa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import time
 
 from pysjtu import consts
 from pysjtu import models
-from pysjtu import schemas
 from pysjtu.client.base import BaseClient
 from pysjtu.exceptions import GPACalculationException
 
 
 class GPAMixin(BaseClient):
     _default_gpa_query_params: models.GPAQueryParams
 
@@ -17,15 +16,15 @@
 
     @property
     def default_gpa_query_params(self) -> models.GPAQueryParams:
         """ Get default gpa query params defined by the website. """
         if not self._default_gpa_query_params:
             rtn = self._session.get(consts.GPA_PARAMS_URL,
                                     params={"_": int(time.time() * 1000), "su": self.student_id})
-            self._default_gpa_query_params = schemas.GPAQueryParamsSchema().load(rtn.json())  # type: ignore
+            self._default_gpa_query_params = models.GPAQueryParams.Schema().load(rtn.json())  # type: ignore
 
         return self._default_gpa_query_params
 
     def gpa(self, query_params: models.GPAQueryParams, **kwargs) -> models.GPA:
         """
         Query your GP & GPA and their rankings of specific year & term.
 
@@ -37,22 +36,22 @@
             See :ref:`Timeout Configuration` for more details.
 
         See :meth:`pysjtu.session.Session.post` for more information about the keyword arguments.
 
         :param query_params: parameters for this query.
             A default one can be fetched by reading property :attr:`default_gpa_query_params`.
         """
-        compiled_params = schemas.GPAQueryParamsSchema().dump(query_params)
+        compiled_params = models.GPAQueryParams.Schema().dump(query_params)
         calc_rtn = self._session.post(consts.GPA_CALC_URL + str(self.student_id),
                                       data=compiled_params, **kwargs)
         if calc_rtn.text != "\"统计成功！\"":
             if calc_rtn.text == "\"统计失败！\"":
                 raise GPACalculationException("Calculation failure.")
             if "无功能权限" in calc_rtn.text:
                 raise GPACalculationException("Unauthorized.")
         compiled_params.update({"_search": False,
                                 "nd": int(time.time() * 1000), "queryModel.showCount": 15,
                                 "queryModel.currentPage": 1, "queryModel.sortName": "",
                                 "queryModel.sortOrder": "asc", "time": 0})
         raw = self._session.post(consts.GPA_QUERY_URL + str(self.student_id),
                                  data=compiled_params, **kwargs)
-        return schemas.GPASchema().load(raw.json()["items"][0])  # type: ignore
+        return models.GPA.Schema().load(raw.json()["items"][0])  # type: ignore
```

### Comparing `pysjtu-0.4.0/pysjtu/client/api/profile.py` & `pysjtu-0.4.1/pysjtu/client/api/profile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pysjtu import consts
 from pysjtu.client.base import BaseClient
 from pysjtu.models.profile import Profile
-from pysjtu.parser.profile import parse
-from pysjtu.schemas.profile import profile_fields
+from pysjtu.parser.profile import parse, profile_fields
 
 
 class ProfileMixin(BaseClient):
     def __init__(self):
         super().__init__()
 
     # noinspection PyProtectedMember
```

### Comparing `pysjtu-0.4.0/pysjtu/client/api/schedule.py` & `pysjtu-0.4.1/pysjtu/client/api/schedule.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/pysjtu/client/api/score.py` & `pysjtu-0.4.1/pysjtu/client/api/score.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import time
 from functools import partial
 from typing import List
 
 from pysjtu import consts
 from pysjtu import models
-from pysjtu import schemas
 from pysjtu.client.base import BaseClient
 from pysjtu.models import Scores
 
 
 class ScoreMixin(BaseClient):
     def __init__(self):
         super().__init__()
 
     def _get_score_detail(self, year: int, term: int, class_id: str, **kwargs) -> List[models.ScoreFactor]:
         raw = self._session.post(consts.SCORE_DETAIL_URL + str(self.student_id),
                                  data={"xnm": year, "xqm": consts.TERMS[term], "jxb_id": class_id, "_search": False,
                                        "nd": int(time.time() * 1000), "queryModel.showCount": 15,
                                        "queryModel.currentPage": 1, "queryModel.sortName": "",
                                        "queryModel.sortOrder": "asc", "time": 1}, **kwargs)
-        factors = schemas.ScoreFactorSchema(many=True).load(raw.json()["items"][:-1])  # type: ignore
+        factors = models.ScoreFactor.Schema(many=True).load(raw.json()["items"][:-1])  # type: ignore
         return factors
 
     def score(self, year: int, term: int, **kwargs) -> Scores:
         """
         Fetch your scores of specific year & term.
 
         See :meth:`pysjtu.session.Session.post` for more information about the keyword arguments.
```

### Comparing `pysjtu-0.4.0/pysjtu/client/api/selection.py` & `pysjtu-0.4.1/pysjtu/client/api/selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from functools import lru_cache, partial
 from typing import List
 
 from pysjtu import consts
 from pysjtu.client.base import BaseClient
 from pysjtu.exceptions import DropException, FullCapacityException, RegistrationException, \
     SelectionClassFetchException, SelectionNotAvailableException, TimeConflictException
-from pysjtu.models.selection import SelectionClass, SelectionSector, SelectionSharedInfo
+from pysjtu.models.selection import SelectionClass, SelectionSector, SelectionSharedInfo, SelectionClassLazySchema
 from pysjtu.parser.selection import parse_sector, parse_sectors, parse_shared_info
-from pysjtu.schemas.selection import SelectionClassSchema, SelectionCourseSchema, SelectionSectorSchema, \
-    SelectionSharedInfoSchema
 
 
 class SelectionMixin(BaseClient):
     def __init__(self):
         super().__init__()
         self._fetch_selection_classes = lru_cache(maxsize=1024)(self._fetch_selection_classes)
         self._get_selection_classes = lru_cache(maxsize=16)(self._get_selection_classes)
@@ -69,38 +67,38 @@
         elif drop == "5":  # pragma: no cover
             raise DropException("Validation failure.")  # pragma: no cover
         else:
             raise DropException(f"Unexpected response: {drop}")  # pragma: no cover
 
     def _fetch_selection_classes(self, sector: SelectionSector, internal_course_id: str) -> List[dict]:
         payload = {
-            **SelectionSectorSchema().dump(sector),
-            **SelectionSharedInfoSchema().dump(sector.shared_info),
+            **SelectionSector.Schema().dump(sector),
+            **SelectionSharedInfo.Schema().dump(sector.shared_info),
             "kch_id": internal_course_id
         }
         classes_query = self._session.post(f"{consts.SELECTION_QUERY_CLASSES}{self.student_id}", data=payload).json()
-        return SelectionClassSchema(many=True).load(classes_query)
+        return SelectionClassLazySchema(many=True).load(classes_query)
 
     def _fetch_selection_class(self, selection_class: SelectionClass):
         class_dicts = self._fetch_selection_classes(selection_class.sector, selection_class.internal_course_id)
         for class_dict in class_dicts:
             if class_dict["class_id"] == selection_class.class_id:
                 return class_dict
         raise SelectionClassFetchException("Unable to fetch selection class information.")  # pragma: no cover
 
     def _get_selection_classes(self, sector: SelectionSector) -> List[SelectionClass]:
         payload = {
-            **SelectionSectorSchema().dump(sector),
-            **SelectionSharedInfoSchema().dump(sector.shared_info),
+            **SelectionSector.Schema().dump(sector),
+            **SelectionSharedInfo.Schema().dump(sector.shared_info),
             "kspage": 1,
             "jspage": 5000
         }
         courses_query = self._session.post(f"{consts.SELECTION_QUERY_COURSES}{self.student_id}", data=payload).json()
-        selection_classes: List[SelectionClass] = [SelectionClass(**item) for item in
-                                                   SelectionCourseSchema(many=True).load(courses_query["tmpList"])]
+        selection_classes: List[SelectionClass] = [item for item in
+                                                   SelectionClass.Schema(many=True).load(courses_query["tmpList"])]
         for _class in selection_classes:
             _class.sector = sector
             _class._load_func = partial(self._fetch_selection_class, _class)
             _class.is_registered = partial(self._class_is_registered, _class)
             _class.register = partial(self._class_register, _class)
             _class.drop = partial(self._class_drop, _class)
         return selection_classes
@@ -112,25 +110,25 @@
         This property contains all available course sectors in this round of selection.
         """
         sectors_query = self._session.get(f"{consts.SELECTION_ALL_SECTORS_PARAM_URL}{self.student_id}").text
         if "对不起，当前不属于选课阶段" in sectors_query:
             raise SelectionNotAvailableException
 
         raw_shared_info = parse_shared_info(sectors_query)
-        shared_info: SelectionSharedInfo = SelectionSharedInfoSchema().load(raw_shared_info)
+        shared_info: SelectionSharedInfo = SelectionSharedInfo.Schema().load(raw_shared_info)
 
         raw_sectors = parse_sectors(sectors_query)
         sectors = []
         for kklxdm, xkkz_id, name in raw_sectors:
             sector_query = self._session.post(f"{consts.SELECTION_SECTOR_PARAM_URL}{self.student_id}",
                                               data={"xkkz_id": xkkz_id,
                                                     "xszxzt": shared_info.self_selecting_status,
                                                     "kspage": 0, "jspage": 0}).text
             raw_sector = parse_sector(sector_query)
-            sector: SelectionSector = SelectionSectorSchema().load(raw_sector)
+            sector: SelectionSector = SelectionSector.Schema().load(raw_sector)
             sector.name, sector.course_type_code, sector.xkkz_id, sector.shared_info = \
                 name, kklxdm, xkkz_id, shared_info
             sector._func_classes = partial(self._get_selection_classes, sector=sector)
             sectors.append(sector)
 
         return sectors
```

### Comparing `pysjtu-0.4.0/pysjtu/consts.py` & `pysjtu-0.4.1/pysjtu/consts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LOGIN_POST_URL = "https://jaccount.sjtu.edu.cn/jaccount/ulogin"
 CAPTCHA_URL = "https://jaccount.sjtu.edu.cn/jaccount/captcha"
+CAPTCHA_REFERER = "https://jaccount.sjtu.edu.cn/jaccount/jalogin"
 
 DEFAULT_BASE_URL = "https://i.sjtu.edu.cn"
 
 HOME_URL = "/xtgl/index_initMenu.html"
 SCHEDULE_URL = "/kbcx/xskbcx_cxXsKb.html?gnmkdm=N2151"
 LOGIN_URL = "/jaccountlogin"
 LOGOUT_URL = "/logout"
```

### Comparing `pysjtu-0.4.0/pysjtu/exceptions.py` & `pysjtu-0.4.1/pysjtu/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/pysjtu/models/base.py` & `pysjtu-0.4.1/pysjtu/models/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 import time
 from abc import ABC
-from enum import IntEnum
-from typing import Callable, Generic, List, Tuple, Type, TypeVar, Union
+from typing import Callable, Generic, List, Tuple, Type, TypeVar, Union, ClassVar
 
 from marshmallow import Schema  # type: ignore
 
 from pysjtu.utils import overlap, parse_slice, range_in_set
 
 
-class Gender(IntEnum):
-    male = 1
-    female = 2
+class _PARTIAL:
+    pass
 
 
 class Result:
-    """ Base class for Result """
+    """ Base class for Result. All item models inherit from this class. """
+    Schema: ClassVar[Type[Schema]] = Schema
 
     def __repr__(self):
         raise NotImplementedError  # pragma: no cover
 
 
-class PARTIAL:
-    pass
-
-
 class LazyResult(Result, ABC):
-    """ Base class for LazyResult """
+    """ Base class for LazyResult. All lazy item models inherit from this class. """
     _load_func: Callable = None
 
     def __getattribute__(self, item):
         value = super().__getattribute__(item)
-        if value == PARTIAL:
+        if value == _PARTIAL:
             update_dict = self._load_func()
             for k, v in update_dict.items():
                 super().__setattr__(k, v)
             value = super().__getattribute__(item)
         return value
 
 
-T_Result = TypeVar("T_Result", bound=Result)
+T_Item = TypeVar("T_Result", bound=Result)
 
 
-class QueryResult(Generic[T_Result]):
+class QueryResult(Generic[T_Item]):
     """
     A key accessible, sliceable, and iterable interface to query result collections.
+    All lazy container models inherit from this class.
+
+    See :ref:`Result Content` for more information.
 
     A QueryResult object is constructed with a raw data callable reference.
 
     A QueryResult object is returned by a query operation, and isn't meant to be constructed by a user.
 
     A QueryResult object is lazy, which means network I/Os won't be performed until items are actually accessed.
 
@@ -70,15 +68,15 @@
         self._query_params = query_params
         self._length = 0
         # noinspection PyTypeChecker
         self._cache = [{}] * len(self)
         self._cached_items = set()
         self._page_size = page_size
 
-    def __getitem__(self, arg: Union[int, slice]) -> T_Result:
+    def __getitem__(self, arg: Union[int, slice]) -> T_Item:
         if isinstance(arg, int):
             data = self._handle_result_by_index(arg)  # type: ignore
         elif isinstance(arg, slice):
             data = self._handle_result_by_idx_slice(arg)  # type: ignore
         else:
             raise TypeError("QueryResult indices must be integers or slices, not " + type(arg).__name__)
         data = self._post_ref(data)  # type: ignore
@@ -154,32 +152,31 @@
         return self._ref(data=new_params).json()
 
     def __iter__(self):
         for i in range(len(self)):
             yield self[i]
 
 
-class Results(List[T_Result]):
+class Results(List[T_Item]):
     """
-    Base class for Results. Almost all return types of query operations are inherited from this class.
+    Base class for Results. All eager container models inherit from this class.
 
     See :ref:`Result Content` for more information.
 
     :param year: year of the query.
     :param term: term of the query.
     """
-    _schema: Type[Schema]
-    _result_model: Type[T_Result]
+    _item: Type[T_Item]
     _valid_fields: List[str]
 
     def __init__(self, year: int = 0, term: int = 0):
         super().__init__()
         self._year = year
         self._term = term
-        self._valid_fields = list(self._result_model.__annotations__.keys())
+        self._valid_fields = list(self._item.__annotations__.keys())
 
     @property
     def year(self) -> int:
         return self._year
 
     @property
     def term(self) -> int:
@@ -188,20 +185,20 @@
     def load(self, data: dict):
         """
         Load a list of dicts into Results, and deserialize dicts to Result objects.
 
         :param data: a list of dicts.
         :meta private:
         """
-        schema = self._schema(many=True)
+        schema = self._item.Schema(many=True)
         results = schema.load(data)
         for result in results:
             self.append(result)
 
-    def filter(self, **param) -> List[T_Result]:
+    def filter(self, **param) -> List[T_Item]:
         """
         Get Result objects matching specific criteria. The criteria are specified by keyword arguments.
 
         Available fields are defined by child classes.
 
         .. note::
             There are three special time-related fields: `week`, `time` and `day`.
```

### Comparing `pysjtu-0.4.0/pysjtu/models/profile.py` & `pysjtu-0.4.1/pysjtu/models/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Optional
 
-from .base import Gender
+from .common import Gender
 
 
 @dataclass(frozen=True)
 class Profile:
     student_id: int
     name: str
     name_pinyin: Optional[str]
```

### Comparing `pysjtu-0.4.0/pysjtu/ocr/__init__.py` & `pysjtu-0.4.1/pysjtu/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/pysjtu/ocr/nn_model.onnx` & `pysjtu-0.4.1/pysjtu/ocr/nn_model.onnx`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/pysjtu/ocr/svm_model.onnx` & `pysjtu-0.4.1/pysjtu/ocr/svm_model.onnx`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/pysjtu/parser/selection.py` & `pysjtu-0.4.1/pysjtu/parser/selection.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/pysjtu/schemas/base.py` & `pysjtu-0.4.1/pysjtu/fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import typing
 
-from marshmallow import ValidationError, fields  # type: ignore
+from marshmallow import fields, ValidationError
 
 from pysjtu.utils import parse_course_week
 
 
 class StrBool(fields.Field):
+    """ Deserialize from / serialize to bool of str type ("0", "1"). """
+
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
@@ -28,27 +30,31 @@
             return "0"
         if value is True:
             return "1"
         raise ValidationError("Invalid bool value.")
 
 
 class ChineseBool(fields.Field):
+    """ Deserialize from bool of Chinese type ("是", "否"). """
+
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
         if not value:
             return None  # pragma: no cover
         return value == "是"
 
 
 class SplitField(fields.Field):
+    """ Deserialize from / serialize to a list of string split by a delimiter. """
+
     def __init__(self, sep: str, *args, **kwargs):
         self.sep = sep
         super().__init__(*args, **kwargs)
 
     def _deserialize(
             self,
             value: typing.Any,
@@ -61,14 +67,16 @@
         return value.split(self.sep)
 
     def _serialize(self, value: typing.Any, attr: str, obj: typing.Any, **kwargs):
         return self.sep.join(str(item) for item in value)
 
 
 class CourseTime(fields.Field):
+    """ Deserialize from course time range like "1-2节". """
+
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
@@ -76,14 +84,16 @@
             return None  # pragma: no cover
         value = value.replace("节", "")
         cs = list(map(int, value.split("-")))
         return list(cs) if len(cs) == 1 else range(cs[0], cs[1] + 1)
 
 
 class CourseWeek(fields.Field):
+    """ Deserialize from course week ranges like "1-16(单)". """
+
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
```

### Comparing `pysjtu-0.4.0/pysjtu/schemas/gpa.py` & `pysjtu-0.4.1/pysjtu/models/gpa.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+# flake8: noqa
 import typing
-from copy import deepcopy
+from enum import Enum, IntEnum
+from typing import List, Optional
 
-from marshmallow import EXCLUDE, Schema, fields, post_dump, post_load, pre_dump, pre_load  # type: ignore
+from marshmallow import EXCLUDE, fields
+from marshmallow_dataclass import dataclass
 
-from pysjtu.schemas.base import SplitField
-from pysjtu.utils import replace_keys
+from pysjtu.fields import SplitField
+from pysjtu.models.base import Result
+from pysjtu.schema import FinalizeHook, LoadDumpSchema, mfield, WithField
 
 
-class HasRoll(fields.Field):
+class _HasRoll(fields.Field):
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
@@ -27,15 +31,15 @@
         if value is True:
             return 1
         if value is False:
             return 0
         return -1  # pragma: no cover
 
 
-class Registered(fields.Field):
+class _Registered(fields.Field):
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
@@ -51,15 +55,15 @@
         if value is True:
             return 1
         if value is False:  # pragma: no cover
             return 0  # pragma: no cover
         return -1  # pragma: no cover
 
 
-class Attending(fields.Field):
+class _Attending(fields.Field):
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
@@ -75,192 +79,198 @@
         if value is True:
             return 1
         if value is False:
             return 0  # pragma: no cover
         return -1
 
 
-class ConditionLogic(fields.Field):
-    def _deserialize(
-            self,
-            value: typing.Any,
-            attr: typing.Optional[str],
-            data: typing.Optional[typing.Mapping[str, typing.Any]],
-            **kwargs
-    ):
-        if value == 0:  # pragma: no cover
-            return LogicEnum.AND  # pragma: no cover
-        if value == 1:  # pragma: no cover
-            return LogicEnum.OR  # pragma: no cover
-        return None  # pragma: no cover
-
-    def _serialize(self, value: typing.Any, attr: str, obj: typing.Any, **kwargs):
-        if not isinstance(value, LogicEnum):
-            raise TypeError
-        if value == LogicEnum.AND:
-            return 0
-        if value == LogicEnum.OR:  # pragma: no cover
-            return 1  # pragma: no cover
-
-
-class MakeupAsPass(fields.Field):
+class _MakeupAsPass(fields.Field):
     def _serialize(self, value: typing.Any, attr: str, obj: typing.Any, **kwargs):
         return "bk" if value else ""
 
 
-class RebuildAsPass(fields.Field):
+class _RebuildAsPass(fields.Field):
     def _serialize(self, value: typing.Any, attr: str, obj: typing.Any, **kwargs):
         return "cx" if value else ""
 
 
-class RankingField(fields.Field):
-    def _serialize(self, value: typing.Any, attr: str, obj: typing.Any, **kwargs):
-        if not isinstance(value, Ranking):
-            raise TypeError
-        return value.value
-
-
-class CourseRangeField(fields.Field):
-    def _serialize(self, value: typing.Any, attr: str, obj: typing.Any, **kwargs):
-        if not isinstance(value, CourseRange):
-            raise TypeError
-        return value.value
-
-
-class Percentage(fields.Field):
+class _Percentage(fields.Field):
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
         if not value:
             return None  # pragma: no cover
         return float(value.replace("%", "")) / 100
 
 
-class RankingResultField(fields.Field):
+class _RankingResult(fields.Field):
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
         if not value:
             return None  # pragma: no cover
         return int(value.split("/")[0])
 
 
-class StudentCountFromRanking(fields.Field):
+class _StudentCountFromRanking(fields.Field):
     def _deserialize(
             self,
             value: typing.Any,
             attr: typing.Optional[str],
             data: typing.Optional[typing.Mapping[str, typing.Any]],
             **kwargs
     ):
         if not value:
             return None  # pragma: no cover
         return int(value.split("/")[1])
 
 
-class GPAQueryParamsSchema(Schema):
-    class Meta:
-        unknown = EXCLUDE
+class LogicEnum(IntEnum):
+    """ Used by :class:`GPAQueryParams` to specify condition logic."""
+
+    AND = 0
+    """All conditions must be satisfied."""
+    OR = 1
+    """At least one condition must be satisfied."""
+
+
+class CourseRange(Enum):
+    """ Used by :class:`GPAQueryParams` to specify courses taken into account when ranking."""
+    ALL = "qbkc"
+    """All courses taken."""
+    CORE = "hxkc"
+    """Only core courses taken."""
+
+
+class Ranking(Enum):
+    """ Used by :class:`GPAQueryParams` to specify student range upon which to rank."""
+    GRADE_AND_FIELD = "njzy"
+    """Rank students in the same grade and field."""
+
 
-    start_term = fields.Int(required=True, metadata={"dump_key": "qsXnxq"}, dump_only=True)
-    end_term = fields.Int(required=True, metadata={"dump_key": "zzXnxq"}, dump_only=True)
-    condition_logic = ConditionLogic(required=True, metadata={"dump_key": "tjgx"}, dump_only=True)
-    makeup_as_60 = MakeupAsPass(required=True, dump_only=True)
-    rebuild_as_60 = RebuildAsPass(required=True, dump_only=True)
-    gp_round = fields.Int(required=True, metadata={"load_key": "cjblws", "dump_key": "sspjfblws"})
-    gpa_round = fields.Int(required=True, metadata={"load_key": "jdblws", "dump_key": "pjjdblws"})
-    exclude_gp = SplitField(required=True, data_key="bjjd", sep=",")
-    exclude_gpa = SplitField(required=True, data_key="bjpjf", sep=",")
-    course_whole = SplitField(required=True, metadata={"load_key": "tjqckc", "dump_key": "kch_ids"}, sep=",")
-    course_range = CourseRangeField(required=True, metadata={"dump_key": "kcfw"}, dump_only=True)
-    excluded_courses = fields.Str(metadata={"load_key": "bcjkc", "dump_key": "bcjkc_id"}, load_default="")
-    excluded_course_groups = fields.Str(metadata={"load_key": "bcjkz", "dump_key": "bcjkz_id"}, load_default="")
-    included_course_groups = fields.Str(metadata={"load_key": "cjkz", "dump_key": "cjkz_id"}, load_default="")
-    statistics_method = fields.Str(required=True, data_key="cjxzm")
-    ranking = RankingField(required=True, metadata={"dump_key": "tjfw"}, dump_only=True)
-    has_roll = HasRoll(required=True, data_key="atjc", load_only=True)
-    registered = Registered(required=True, data_key="atjc", load_only=True)
-    attending = Attending(required=True, data_key="atjc", load_only=True)
-    has_roll_dump = HasRoll(required=True, data_key="xjzt", dump_only=True)
-    registered_dump = Registered(required=True, data_key="zczt", dump_only=True)
-    attending_dump = Attending(required=True, data_key="sfzx", dump_only=True)
-
-    # noinspection PyUnusedLocal
-    @pre_load
-    def wrap_pre_load(self, data, **kwargs):
+class DedupMethod(Enum):
+    """ Used by :class:`GPAQueryParams` to specify which score to take if a student has taken a course multiple
+    times."""
+    LAST_SCORE = "zhyccj"
+    """Take the last score."""
+
+
+class _GPAQueryParamsExtSchema(LoadDumpSchema):
+    def pre_load(self, data, **kwargs):
         data = {item["zdm"]: item["szz"] for item in filter(lambda x: "szz" in x.keys(), data)}
-        pairs = tuple(
-            (field.metadata['load_key'], field.data_key or field_name)
-            for field_name, field in self.fields.items() if 'load_key' in field.metadata
-        )
-        return replace_keys(data, pairs)
-
-    # noinspection PyUnusedLocal
-    @post_load
-    def wrap_post_load(self, data, **kwargs):
-        return GPAQueryParams(makeup_as_60=False, rebuild_as_60=False, ranking=Ranking.GRADE_AND_FIELD,
-                              course_range=CourseRange.CORE, start_term=None, end_term=None,
-                              condition_logic=LogicEnum.AND, **data)
-
-    # noinspection PyUnusedLocal
-    @pre_dump
-    def wrap_pre_dump(self, data, **kwargs):
-        pre_dict = deepcopy(data.__dict__)
-        pre_dict["has_roll_dump"] = pre_dict.pop("has_roll")
-        pre_dict["registered_dump"] = pre_dict.pop("registered")
-        pre_dict["attending_dump"] = pre_dict.pop("attending")
-        return pre_dict
-
-    # noinspection PyUnusedLocal
-    @post_dump
-    def wrap_post_dump(self, data, **kwargs):
-        pairs = tuple(
-            (field.data_key or field_name, field.metadata['dump_key'])
-            for field_name, field in self.fields.items() if 'dump_key' in field.metadata
-        )
-        data = replace_keys(data, pairs)
+        return super().pre_load(data, **kwargs)
+
+    def post_dump(self, data, **kwargs):
+        data = super().post_dump(data, **kwargs)
 
         parse_fields = ["xjzt", "zczt", "sfzx"]
         data["alsfj"] = data.pop("makeup_as_60") + data.pop("rebuild_as_60")
         for field in parse_fields:
             if data[field] == -1:
                 data.pop(field)
 
         parse_fields = ["qsXnxq", "zzXnxq"]
         for field in parse_fields:
             if data[field] is None:
                 data[field] = ''
         return data
 
 
-class GPASchema(Schema):
+@dataclass(base_schema=FinalizeHook(_GPAQueryParamsExtSchema))
+class GPAQueryParams(Result):
+    """
+    A model which describes GPA query parameters. Used when performing gpa queries (pysjtu.Client().query_gpa(...)).
+    You may leave fields empty if you don't want to filter by them.
+
+    :param start_term: begin term of the query.
+    :param end_term: end term of the query.
+    :param condition_logic: logic applied between `has_roll`, `registered` and `attending`.
+    :param makeup_as_60: treat makeup scores (P) as 60.
+    :param rebuild_as_60: treat rebuild scores (P) as 60.
+    :param gp_round: round gp to a given precision in decimal digits.
+    :param gpa_round: round gpa to a given precision in decimal digits.
+    :param exclude_gp: exclude courses matching given criteria when calculating gp.
+    :param exclude_gpa: exclude courses matching given criteria when calculating gpa.
+    :param course_whole: unknown parameter. (统计全程的课程)
+    :param course_range: courses taken into account when ranking
+    :param excluded_courses: ids of courses excluded from statistics.
+    :param excluded_course_groups: ids of course groups excluded from statistics.
+    :param included_course_groups: ids of course groups included in statistics.
+    :param dedup_method: which score to take if a student has taken a course multiple times.
+    :param ranking: student range upon which to rank
+    :param has_roll: only include students who are enrolled in school.
+    :param registered: only include students who are registered.
+    :param attending: only include students who are attending school now.
+    """
+    start_term: Optional[int] = mfield(dump_key="qsXnxq", load_default=None)
+    end_term: Optional[int] = mfield(dump_key="zzXnxq", load_default=None)
+    condition_logic: LogicEnum = mfield(dump_key="tjgx", load_default=LogicEnum.AND, by_value=True)
+    makeup_as_60: WithField(bool, field=_MakeupAsPass) = mfield(load_default=False)
+    rebuild_as_60: WithField(bool, field=_RebuildAsPass) = mfield(load_default=False)
+    gp_round: int = mfield(required=True, load_key="cjblws", dump_key="sspjfblws")
+    gpa_round: int = mfield(required=True, load_key="jdblws", dump_key="pjjdblws")
+    exclude_gp: WithField(List[str], field=SplitField, sep=",") = mfield(required=True, data_key="bjjd")
+    exclude_gpa: WithField(List[str], field=SplitField, sep=",") = mfield(required=True, data_key="bjpjf")
+    course_whole: WithField(List[str], field=SplitField, sep=",") \
+        = mfield(required=True, load_key="tjqckc", dump_key="kch_ids")
+    course_range: CourseRange = mfield(dump_key="kcfw", load_default=CourseRange.CORE, by_value=True)
+    excluded_courses: str = mfield(load_key="bcjkc", dump_key="bcjkc_id", load_default="")
+    excluded_course_groups: str = mfield(load_key="bcjkz", dump_key="bcjkz_id", load_default="")
+    included_course_groups: str = mfield(load_key="cjkz", dump_key="cjkz_id", load_default="")
+    dedup_method: DedupMethod = mfield(required=True, data_key="cjxzm", by_value=True)
+    ranking: Ranking = mfield(dump_key="tjfw", load_default=Ranking.GRADE_AND_FIELD, by_value=True)
+    has_roll: WithField(bool, field=_HasRoll) = mfield(required=True, load_key="atjc", dump_key="xjzt")
+    registered: WithField(bool, field=_Registered) = mfield(required=True, load_key="atjc", dump_key="zczt")
+    attending: WithField(bool, field=_Attending) = mfield(required=True, load_key="atjc", dump_key="sfzx")
+
     class Meta:
         unknown = EXCLUDE
 
-    total_score = fields.Float(required=True, data_key="zf")
-    course_count = fields.Int(required=True, data_key="ms")
-    fail_count = fields.Int(required=True, data_key="bjgms")
-    total_credit = fields.Float(required=True, data_key="zxf")
-    acquired_credit = fields.Float(required=True, data_key="hdxf")
-    failed_credit = fields.Float(required=True, data_key="bjgxf")
-    pass_rate = Percentage(required=True, data_key="tgl")
-    gp = fields.Float(required=True, data_key="xjf")
-    gp_ranking = RankingResultField(required=True, data_key="xjfpm")
-    gpa = fields.Float(required=True, data_key="gpa")
-    gpa_ranking = RankingResultField(required=True, data_key="gpapm", load_only=True)
-    total_students = StudentCountFromRanking(required=True, data_key="gpapm", load_only=True)
-
-    # noinspection PyUnusedLocal
-    @post_load
-    def wrap(self, data, **kwargs):
-        return GPA(**data)
+    def __repr__(self):
+        return f"<GPAQueryParams {self.__dict__}>"
 
 
-from pysjtu.models.gpa import LogicEnum, Ranking, CourseRange, GPAQueryParams, GPA
+@dataclass
+class GPA(Result):
+    """
+    A model which describes GP & GPA and rankings.
+
+    :param total_score: summed score of all matched courses.
+    :param course_count: number of all matched courses.
+    :param fail_count: number of failed courses.
+    :param total_credit: summed credit of all matched courses.
+    :param acquired_credit: summed credit of passed courses.
+    :param failed_credit: summed credit of failed courses.
+    :param pass_rate: the pass rate of all matched courses.
+    :param gp: summed gp of all matched courses.
+    :param gp_ranking: ranking of the gp.
+    :param gpa: gpa of all matched courses.
+    :param gpa_ranking: ranking of the gpa.
+    :param total_students: number of students participates in the ranking.
+    """
+    total_score: float = mfield(required=True, data_key="zf")
+    course_count: int = mfield(required=True, data_key="ms")
+    fail_count: int = mfield(required=True, data_key="bjgms")
+    total_credit: float = mfield(required=True, data_key="zxf")
+    acquired_credit: float = mfield(required=True, data_key="hdxf")
+    failed_credit: float = mfield(required=True, data_key="bjgxf")
+    pass_rate: WithField(float, _Percentage) = mfield(required=True, data_key="tgl")
+    gp: float = mfield(required=True, data_key="xjf")
+    gp_ranking: WithField(int, _RankingResult) = mfield(required=True, data_key="xjfpm")
+    gpa: float = mfield(required=True, data_key="gpa")
+    gpa_ranking: WithField(int, _RankingResult) = mfield(required=True, data_key="gpapm", load_only=True)
+    total_students: WithField(int, _StudentCountFromRanking) = mfield(required=True, data_key="gpapm", load_only=True)
+
+    class Meta:
+        unknown = EXCLUDE
+
+    def __repr__(self):
+        return f"<GPA gp={self.gp} {self.gp_ranking}/{self.total_students} " \
+               f"gpa={self.gpa} {self.gpa_ranking}/{self.total_students}>"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pysjtu-0.4.0/pysjtu/session.py` & `pysjtu-0.4.1/pysjtu/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from urllib.parse import parse_qs, urlparse
 
 import httpx
 from httpx import Response
 
 from pysjtu.ocr import JCSSRecognizer, Recognizer
 from . import consts
+from .consts import CAPTCHA_REFERER
 from .exceptions import DumpWarning, LoadWarning, LoginException, ServiceUnavailable, SessionException
 from .utils import FileTypes
 
 CookieTypes = Union[httpx.Cookies, CookieJar]
 URLTypes = Union[httpx.URL, str]
 
 
@@ -355,15 +356,16 @@
         for i in self._retry:
             login_page_req = self._secure_req(
                 partial(self.get, consts.LOGIN_URL, validate_session=False, headers=consts.HEADERS))
             uuid = re.findall(r"(?<=uuid\": ').*(?=')", login_page_req.text)[0]
             login_params = {k: v[0] for k, v in parse_qs(urlparse(str(login_page_req.url)).query).items()}
 
             captcha_img = self.get(consts.CAPTCHA_URL,
-                                   params={"uuid": uuid, "t": int(time.time() * 1000)}).content
+                                   params={"uuid": uuid, "t": int(time.time() * 1000)},
+                                   headers={"Referer": CAPTCHA_REFERER}).content
             captcha = self._ocr.recognize(captcha_img)
 
             login_params.update({"v": "", "uuid": uuid, "user": username, "pass": password, "captcha": captcha})
             result = self._secure_req(
                 partial(self.post, consts.LOGIN_POST_URL, params=login_params, headers=consts.HEADERS))
             if b"err=" not in result.url.query:  # type: ignore
                 self._username = username
```

### Comparing `pysjtu-0.4.0/pysjtu/utils.py` & `pysjtu-0.4.1/pysjtu/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,16 +46,23 @@
 
 def has_callable(obj, name):
     return callable(getattr(obj, name, None))
 
 
 def replace_keys(data, pairs):
     for from_key, to_key in pairs:
-        if from_key in data:
-            data[to_key] = data.pop(from_key)
+        try:
+            data[to_key] = data[from_key]
+        except KeyError:
+            pass
+    for from_key, _ in pairs:
+        try:
+            del data[from_key]
+        except KeyError:
+            pass
     return data
 
 
 def schema_post_loader(schema_ref, data):
     if isinstance(data, list):
         return schema_ref(many=True).load(data)
     if isinstance(data, dict):
```

### Comparing `pysjtu-0.4.0/tests/mock_server.py` & `pysjtu-0.4.1/tests/mock_server.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/captcha/aoaiq.jpeg` & `pysjtu-0.4.1/tests/resources/captcha/aoaiq.jpeg`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/captcha/cqmzn.jpeg` & `pysjtu-0.4.1/tests/resources/captcha/cqmzn.jpeg`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/captcha/ghwty.jpeg` & `pysjtu-0.4.1/tests/resources/captcha/ghwty.jpeg`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/captcha/mfobv.jpeg` & `pysjtu-0.4.1/tests/resources/captcha/mfobv.jpeg`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/captcha/pisv.jpeg` & `pysjtu-0.4.1/tests/resources/captcha/pisv.jpeg`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/exam.json` & `pysjtu-0.4.1/tests/resources/resp/exam.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/gpa_query_params.json` & `pysjtu-0.4.1/tests/resources/resp/gpa_query_params.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/lib_course_1.json` & `pysjtu-0.4.1/tests/resources/resp/lib_course_1.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/lib_course_2.json` & `pysjtu-0.4.1/tests/resources/resp/lib_course_2.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/schedule_course_1.json` & `pysjtu-0.4.1/tests/resources/resp/schedule_course_1.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/schedule_course_2.json` & `pysjtu-0.4.1/tests/resources/resp/schedule_course_2.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/score.json` & `pysjtu-0.4.1/tests/resources/resp/score.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/score_factor.json` & `pysjtu-0.4.1/tests/resources/resp/score_factor.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/selection_class.json` & `pysjtu-0.4.1/tests/resources/resp/selection_class.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/resp/selection_course.json` & `pysjtu-0.4.1/tests/resources/resp/selection_course.json`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/cjcx_cxDgXscj.html` & `pysjtu-0.4.1/tests/resources/website/cjcx_cxDgXscj.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/cjcx_cxXsXmcjList.html` & `pysjtu-0.4.1/tests/resources/website/cjcx_cxXsXmcjList.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/common_cxGnzdxxList.html` & `pysjtu-0.4.1/tests/resources/website/common_cxGnzdxxList.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/funcData_cxFuncDataList_1.html` & `pysjtu-0.4.1/tests/resources/website/funcData_cxFuncDataList_1.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/funcData_cxFuncDataList_2.html` & `pysjtu-0.4.1/tests/resources/website/funcData_cxFuncDataList_2.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/funcData_cxFuncDataList_3.html` & `pysjtu-0.4.1/tests/resources/website/funcData_cxFuncDataList_3.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/funcData_cxFuncDataList_initial.html` & `pysjtu-0.4.1/tests/resources/website/funcData_cxFuncDataList_initial.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/gpapmtj_cxGpaxjfcxIndex.html` & `pysjtu-0.4.1/tests/resources/website/gpapmtj_cxGpaxjfcxIndex.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/gpapmtj_tjGpapmtj_unauthorized.html` & `pysjtu-0.4.1/tests/resources/website/gpapmtj_tjGpapmtj_unauthorized.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/index_cxshjdAreaFive.html` & `pysjtu-0.4.1/tests/resources/website/index_cxshjdAreaFive.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/index_initMenu.html` & `pysjtu-0.4.1/tests/resources/website/index_initMenu.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/jalogin` & `pysjtu-0.4.1/tests/resources/website/jalogin`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/kscx_cxXsksxxIndex.html` & `pysjtu-0.4.1/tests/resources/website/kscx_cxXsksxxIndex.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/login_slogin.html` & `pysjtu-0.4.1/tests/resources/website/login_slogin.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/xsgrxxwh_cxXsgrxx.html` & `pysjtu-0.4.1/tests/resources/website/xsgrxxwh_cxXsgrxx.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/xskbcx_cxXsKb.html` & `pysjtu-0.4.1/tests/resources/website/xskbcx_cxXsKb.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxJxbWithKchZzxkYzb.html` & `pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxJxbWithKchZzxkYzb.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxZzxkYzbDisplay.html` & `pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxZzxkYzbDisplay.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxZzxkYzbIndex.html` & `pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxZzxkYzbIndex.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxZzxkYzbIndex_not_selecting.html` & `pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxZzxkYzbIndex_not_selecting.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/resources/website/zzxkyzb_cxZzxkYzbPartDisplay.html` & `pysjtu-0.4.1/tests/resources/website/zzxkyzb_cxZzxkYzbPartDisplay.html`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/test_api.py` & `pysjtu-0.4.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/test_model.py` & `pysjtu-0.4.1/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from datetime import date, time
 from functools import partial
 from math import ceil
 
 import pytest
 
 from pysjtu.models import QueryResult, GPAQueryParams, GPA, LibCourse, Exam, ScoreFactor, Score, ScheduleCourse, \
-    Exams, Scores, Schedule, LazyResult, PARTIAL, SelectionClass, SelectionSector
-from pysjtu.schemas import ExamSchema, ScoreSchema, ScheduleCourseSchema
+    Exams, Scores, Schedule, LazyResult, _PARTIAL, SelectionClass, SelectionSector
 
 
 @pytest.fixture
 def dummy_req():
     class DummyResp:
         def __init__(self, resp):
             self._resp = resp
@@ -88,16 +87,16 @@
 
 def test_lazy_model(mocker):
     class DummyModel(LazyResult):
         def __repr__(self):
             return "DummyModel"
 
         normal_field: int = 0
-        lazy_field_1: int = PARTIAL
-        lazy_field_2: str = PARTIAL
+        lazy_field_1: int = _PARTIAL
+        lazy_field_2: str = _PARTIAL
 
     fake_load_func = mocker.Mock(return_value={"lazy_field_1": 1, "lazy_field_2": "2"})
     model = DummyModel()
     model._load_func = fake_load_func
 
     assert model.normal_field == 0
     fake_load_func.assert_not_called()
@@ -123,21 +122,21 @@
       "include_other_grades", "include_other_majors", "sfznkx", "zdkxms", "shared_info"],
      ({"name": "major"},
       "<SelectionSector major>")),
 
     (GPAQueryParams,
      ["start_term", "end_term", "condition_logic", "makeup_as_60", "rebuild_as_60", "gp_round", "gpa_round",
       "exclude_gp", "exclude_gpa", "course_whole", "course_range", "excluded_courses", "excluded_course_groups",
-      "included_course_groups", "statistics_method", "ranking", "has_roll", "registered", "attending"],
+      "included_course_groups", "dedup_method", "ranking", "has_roll", "registered", "attending"],
      ({"start_term": 0},
       "<GPAQueryParams {'start_term': 0, 'end_term': None, 'condition_logic': None, "
       "'makeup_as_60': None, 'rebuild_as_60': None, 'gp_round': None, 'gpa_round': "
       "None, 'exclude_gp': None, 'exclude_gpa': None, 'course_whole': None, "
       "'course_range': None, 'excluded_courses': None, 'excluded_course_groups': "
-      "None, 'included_course_groups': None, 'statistics_method': None, 'ranking': "
+      "None, 'included_course_groups': None, 'dedup_method': None, 'ranking': "
       "None, 'has_roll': None, 'registered': None, 'attending': None}>")),
 
     (GPA,
      ["total_score", "course_count", "fail_count", "total_credit", "acquired_credit", "failed_credit", "pass_rate",
       "gp", "gp_ranking", "gpa", "gpa_ranking", "total_students"],
      ({"gp": 80, "gp_ranking": 50, "gpa": 3.8, "gpa_ranking": 40, "total_students": 200},
       "<GPA gp=80 50/200 gpa=3.8 40/200>")),
@@ -227,30 +226,30 @@
 
         def __repr__(self):
             return f"<FakeModel {self.__dict__}>"
 
     return FakeModel
 
 
-@pytest.mark.parametrize("model, mock_schema, test_score",
-                         [(Exams, ExamSchema, False), (Schedule, ScheduleCourseSchema, False),
-                          (Scores, ScoreSchema, True)])
-def test_loader_model(mocker, fake_model, model, mock_schema, test_score):
+@pytest.mark.parametrize("model, mock_item, test_score",
+                         [(Exams, Exam, False), (Schedule, ScheduleCourse, False),
+                          (Scores, Score, True)])
+def test_loader_model(mocker, fake_model, model, mock_item, test_score):
     rtn_var = [
         fake_model(name="Calculus", credit=6.0),
         fake_model(name="Calculus", credit=4.0),
         fake_model(name="Chemistry", credit=4.0)
     ]
     if test_score:
         loaded_var = rtn_var.copy()
         for item in loaded_var:
             item.__dict__.update({"year": 2012, "term": 1, "_func_detail": None})
     else:
         loaded_var = rtn_var
-    mocker.patch.object(mock_schema, "load", return_value=rtn_var)
+    mocker.patch.object(mock_item.Schema, "load", return_value=rtn_var)
     if test_score:
         model_1 = model(year=2012, term=1, func_detail=None)
     else:
         model_1 = model(year=2012, term=1)
     assert model_1.year == 2012
     assert model_1.term == 1
     model_1.load(None)
@@ -264,15 +263,15 @@
 
 def test_schedule_filter(mocker, fake_model):
     rtn_var = [
         fake_model(name="Calculus", day=1, week=[range(1, 17)], time=range(1, 3)),
         fake_model(name="Chemistry", day=3, week=[range(1, 14, 2)], time=range(1, 3)),
         fake_model(name="Millitary", day=2, week=[5, 10, range(14, 16)], time=range(5, 7))
     ]
-    mocker.patch.object(ScheduleCourseSchema, "load", return_value=rtn_var)
+    mocker.patch.object(ScheduleCourse.Schema, "load", return_value=rtn_var)
     model_1 = Schedule()
     model_1.load(None)
     assert model_1.filter(week=3) == rtn_var[:2]
     assert model_1.filter(week=17) == []
     assert model_1.filter(week=[5]) == rtn_var
     assert model_1.filter(week=range(15, 17)) == [rtn_var[0], rtn_var[2]]
     assert model_1.filter(week=[3, range(16, 17)]) == rtn_var[:2]
```

### Comparing `pysjtu-0.4.0/tests/test_ocr.py` & `pysjtu-0.4.1/tests/test_ocr.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/tests/test_parser.py` & `pysjtu-0.4.1/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from datetime import date
 from os import path
 
 import pytest
 from lxml import html
 
-from pysjtu.models.base import Gender
-from pysjtu.parser.profile import ProfileField, parse
+from pysjtu.models.common import Gender
+from pysjtu.parser.profile import ProfileField, parse, profile_fields
 from pysjtu.parser.selection import parse_fields, parse_sectors
-from pysjtu.schemas.profile import profile_fields
 
 
 @pytest.fixture()
 def website_loader():
     RESP_DIR = path.join(path.dirname(path.abspath(__file__)), 'resources/website')
 
     def _resp_loader(name):
```

### Comparing `pysjtu-0.4.0/tests/test_schema.py` & `pysjtu-0.4.1/tests/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
 import json
 from os import path
 
 import pytest
 from marshmallow import ValidationError
 
-from pysjtu.models import CourseRange, LogicEnum, Ranking
-from pysjtu.models.selection import Gender, LessonTime
-from pysjtu.schemas import ExamSchema, GPAQueryParamsSchema, GPASchema, LibCourseSchema, ScheduleCourseSchema, \
-    ScoreFactorSchema, ScoreSchema, SelectionClassSchema, SelectionCourseSchema, SelectionSectorSchema, \
-    SelectionSharedInfoSchema
-from pysjtu.schemas.base import StrBool
-from pysjtu.schemas.schedule import CreditHourDetail
+from pysjtu.fields import StrBool
+from pysjtu.models import CourseRange, LogicEnum, Ranking, GPAQueryParams, GPA, LibCourse, Exam, ScoreFactor, Score, \
+    _PARTIAL
+from pysjtu.models.common import Gender
+from pysjtu.models.gpa import DedupMethod
+from pysjtu.models.schedule import _CreditHourDetail, ScheduleCourse
+from pysjtu.models.selection import LessonTime, SelectionClassLazySchema, SelectionClass, SelectionSector, \
+    SelectionSharedInfo
 
 
 @pytest.fixture()
 def resp_loader():
     RESP_DIR = path.join(path.dirname(path.abspath(__file__)), 'resources/resp')
 
     def _resp_loader(name):
@@ -23,31 +24,32 @@
             return json.load(f)
 
     return _resp_loader
 
 
 def test_selection_course_schema(resp_loader):
     raw_resp = resp_loader("selection_course")
-    schema = SelectionCourseSchema()
+    schema = SelectionClass.Schema()
     course = schema.load(raw_resp)
+    course_dict = {k: v for k, v in course.__dict__.items() if v is not _PARTIAL and v is not None}
 
-    assert course == {
+    assert course_dict == {
         "name": "问题求解与实践",
         "credit": 3.0,
         "course_id": "CS241",
         "internal_course_id": "_CS241",
         "class_name": "(2020-2021-1)-CS241-1",
         "class_id": "A86B96D4FB8A3CFEE055F8163ED16360",
         "students_registered": 11
     }
 
 
 def test_selection_class_schema(resp_loader):
     raw_resp = resp_loader("selection_class")
-    schema = SelectionClassSchema()
+    schema = SelectionClassLazySchema()
     _class = schema.load(raw_resp)
 
     assert _class == {
         "class_id": "A86B96D4FB8A3CFEE055F8163ED16360",
         "register_id": "2914000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000",
         "teachers": [("陈雨亭", "副教授"), ("沈艳艳", "讲师(高校)")],
         "locations": ["中院312", "中院312", "中院312", "中院312"],
@@ -64,15 +66,15 @@
 
     class_2 = schema.load({"xkbz": "N/A", **raw_resp})
     assert class_2["remark"] == "N/A"
 
 
 def test_selection_sector_schema(resp_loader):
     raw_resp = resp_loader("selection_sector")
-    schema = SelectionSectorSchema()
+    schema = SelectionSector.Schema()
     sector = schema.load(raw_resp)
 
     assert sector.task_type == 1
     assert sector.xkly == 1
     assert sector.pe_op_param == 30
     assert sector.sector_type_id == "0"
     assert sector.txbsfrl == 1
@@ -87,15 +89,15 @@
     assert {k: str(v) for k, v in schema.dump(sector).items()} == \
            {"kklxdm": "01", "xkkz_id": "A000000000000B76E055F8163ED16360",
             **raw_resp}
 
 
 def test_selection_shared_info_schema(resp_loader):
     raw_resp = resp_loader("selection_shared_info")
-    schema = SelectionSharedInfoSchema()
+    schema = SelectionSharedInfo.Schema()
     shared_info = schema.load(raw_resp)
 
     assert shared_info.term == "02"
     assert shared_info.selection_year == 2020
     assert shared_info.selection_term == 3
     assert shared_info.major_id == "000000"
     assert shared_info.student_grade == 2019
@@ -107,15 +109,15 @@
     assert shared_info.field_id == "wfx"
     assert shared_info.student_background == 99999
 
     assert {k: str(v) for k, v in schema.dump(shared_info).items()} == raw_resp
 
 
 def test_schedule_credit_hour_detail_field():
-    field = CreditHourDetail()
+    field = _CreditHourDetail()
     assert field.deserialize("task_1:3.0,task_2:0.5") == {"task_1": 3.0, "task_2": 0.5}
     assert field.deserialize("-") == {"N/A": 0}
 
 
 def test_str_bool_field():
     field = StrBool()
     assert field.deserialize("0") is False
@@ -126,15 +128,15 @@
     assert field.serialize("test", {"test": True}) == "1"
     with pytest.raises(ValidationError):
         field.serialize("test", {"test": -1})
 
 
 def test_schedule_course_schema_1(resp_loader):
     raw_resp = resp_loader("schedule_course_1")
-    schema = ScheduleCourseSchema()
+    schema = ScheduleCourse.Schema()
     schedule_course = schema.load(raw_resp)
 
     assert schedule_course.name == "军事理论"
     assert schedule_course.day == 1 and isinstance(schedule_course.day, int)
     assert schedule_course.week == [6, 10, range(14, 16)]
     assert schedule_course.time == range(1, 3)
     assert schedule_course.location == "下院306"
@@ -150,15 +152,15 @@
     assert schedule_course.hour_remark == {"理论": 24, "其他": 24}
     assert schedule_course.hour_week == 1 and isinstance(schedule_course.hour_week, float)
     assert schedule_course.field == "无方向"
 
 
 def test_schedule_course_schema_2(resp_loader):
     raw_resp = resp_loader("schedule_course_2")
-    schema = ScheduleCourseSchema()
+    schema = ScheduleCourse.Schema()
     schedule_course = schema.load(raw_resp)
 
     assert schedule_course.name == "形势与政策"
     assert schedule_course.day == 3 and isinstance(schedule_course.day, int)
     assert schedule_course.week == [5, 9, range(13, 16, 2)]
     assert schedule_course.time == range(9, 11)
     assert schedule_course.location == "中院411"
@@ -174,29 +176,29 @@
     assert schedule_course.hour_remark == {"理论": 8.0}
     assert schedule_course.hour_week == 0.5 and isinstance(schedule_course.hour_week, float)
     assert schedule_course.field == "无方向"
 
 
 def test_score_factor_schema(resp_loader):
     raw_resp = resp_loader("score_factor")
-    schema = ScoreFactorSchema(many=True)
+    schema = ScoreFactor.Schema(many=True)
     score_factors = schema.load(raw_resp)
 
     assert score_factors[0].name == "平时"
     assert score_factors[0].percentage == 0.4
     assert score_factors[0].score == "93"
 
     assert score_factors[1].name == "期末"
     assert score_factors[1].percentage == 0.6
     assert score_factors[1].score == "B+"
 
 
 def test_score_schema(resp_loader):
     raw_resp = resp_loader("score")
-    schema = ScoreSchema()
+    schema = Score.Schema()
     score = schema.load(raw_resp)
 
     assert score.name == "大学化学"
     assert score.teacher == "麦亦勇"
     assert score.score == "91"
     assert score.credit == 2 and isinstance(score.gp, float)
     assert score.gp == 4.0 and isinstance(score.gp, float)
@@ -208,15 +210,15 @@
     assert score.course_id == "CA001"
     assert score.class_name == "(2019-2020-1)-CA001-10"
     assert score.class_id == "90DD3334A9410650E0530200A8C03235"
 
 
 def test_exam_schema(resp_loader):
     raw_resp = resp_loader("exam")
-    schema = ExamSchema()
+    schema = Exam.Schema()
     exam = schema.load(raw_resp)
 
     assert exam.name == "2019-2020-1数学期中考"
     assert exam.location == "东上院509"
     assert exam.seat == 1
     assert exam.course_id == "MA248"
     assert exam.course_name == "高等数学I"
@@ -226,53 +228,53 @@
     assert not exam.self_study and isinstance(exam.self_study, bool)
     assert exam.date == datetime.date(2019, 11, 6)
     assert exam.time == [datetime.time(13, 10), datetime.time(15, 10)]
 
 
 def test_gpa_query_params_schema_load(resp_loader):
     raw_resp = resp_loader("gpa_query_params")
-    schema = GPAQueryParamsSchema()
+    schema = GPAQueryParams.Schema()
     gpa_query_params = schema.load(raw_resp)
 
     assert gpa_query_params.gp_round == 9
     assert gpa_query_params.gpa_round == 9
     assert gpa_query_params.exclude_gp == ['缓考', '缓考(重考)', '尚未修读', '暂不记录', '中期退课', '重考报名']
     assert gpa_query_params.exclude_gpa == ['缓考', '缓考(重考)', '尚未修读', '暂不记录', '中期退课', '重考报名']
     assert gpa_query_params.excluded_courses == ""
     assert gpa_query_params.excluded_course_groups == ""
     assert gpa_query_params.included_course_groups == ""
-    assert gpa_query_params.statistics_method == "zhyccj"
+    assert gpa_query_params.dedup_method == DedupMethod.LAST_SCORE
     assert gpa_query_params.course_whole == ['MARX1205', 'TH009', 'TH020']
     assert gpa_query_params.has_roll and isinstance(gpa_query_params.has_roll, bool)
     assert gpa_query_params.registered is None
     assert gpa_query_params.attending is None
 
 
 def test_gpa_query_params_schema_dump(resp_loader):
     raw_resp = resp_loader("gpa_query_params")
-    schema = GPAQueryParamsSchema()
+    schema = GPAQueryParams.Schema()
     gpa_query_params = schema.load(raw_resp)
 
     gpa_query_params.end_term = 2019
 
     gpa_query_params.condition_logic = 0
-    with pytest.raises(TypeError):
+    with pytest.raises(AttributeError):
         schema.dump(gpa_query_params)
     gpa_query_params.condition_logic = LogicEnum.AND
 
     gpa_query_params.makeup_as_60 = True
     gpa_query_params.rebuild_as_60 = True
 
     gpa_query_params.course_range = 0
-    with pytest.raises(TypeError):
+    with pytest.raises(AttributeError):
         schema.dump(gpa_query_params)
     gpa_query_params.course_range = CourseRange.ALL
 
     gpa_query_params.ranking = 0
-    with pytest.raises(TypeError):
+    with pytest.raises(AttributeError):
         schema.dump(gpa_query_params)
     gpa_query_params.ranking = Ranking.GRADE_AND_FIELD
 
     gpa_query_params.has_roll = False
     gpa_query_params.registered = True
     gpa_query_params.attending = None
 
@@ -283,15 +285,15 @@
                          'bjjd': '缓考,缓考(重考),尚未修读,暂不记录,中期退课,重考报名',
                          'bjpjf': '缓考,缓考(重考),尚未修读,暂不记录,中期退课,重考报名', 'cjkz_id': '',
                          'cjxzm': 'zhyccj', 'kch_ids': 'MARX1205,TH009,TH020', }
 
 
 def test_gpa_schema(resp_loader):
     raw_resp = resp_loader("gpa")
-    schema = GPASchema()
+    schema = GPA.Schema()
     gpa = schema.load(raw_resp)
 
     assert gpa.total_score == 999
     assert gpa.course_count == 14
     assert gpa.fail_count == 0
     assert gpa.total_credit == 32.5
     assert gpa.acquired_credit == 32.5
@@ -301,15 +303,15 @@
     assert gpa.gp_ranking == 21
     assert gpa.gpa == 4.123456789
     assert gpa.gpa_ranking == 20
     assert gpa.total_students == 99
 
 
 def test_lib_course_schema_1(resp_loader):
-    schema = LibCourseSchema()
+    schema = LibCourse.Schema()
     raw_resp = resp_loader("lib_course_1")
     lib_course = schema.load(raw_resp)
 
     assert lib_course.name == "高等数学I"
     assert lib_course.day == 1 and isinstance(lib_course.day, int)
     assert lib_course.week == [range(1, 17)]
     assert lib_course.time == range(1, 3)
@@ -326,15 +328,15 @@
     assert lib_course.hour_remark == {"理论": 6.0}
     assert lib_course.seats == 168
     assert lib_course.students_elected == 100
     assert lib_course.students_planned == 115
 
 
 def test_lib_course_schema_2(resp_loader):
-    schema = LibCourseSchema()
+    schema = LibCourse.Schema()
     raw_resp = resp_loader("lib_course_2")
     lib_course = schema.load(raw_resp)
 
     assert lib_course.name == "高等数学A1"
     assert lib_course.day == 1 and isinstance(lib_course.day, int)
     assert lib_course.week == [range(1, 14, 2)]
     assert lib_course.time == range(1, 3)
```

### Comparing `pysjtu-0.4.0/tests/test_utils.py` & `pysjtu-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pysjtu-0.4.0/PKG-INFO` & `pysjtu-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysjtu
-Version: 0.4.0
+Version: 0.4.1
 Summary: The Python iSJTU client for Humans.
 License: GPL-3.0-or-later
 Author-email: LightQuantum <self@lightquantum.me>
 Requires-Python: >=3.8
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pysjtu Version: 0.4.0 Summary: The Python iSJTU
+Metadata-Version: 2.1 Name: pysjtu Version: 0.4.1 Summary: The Python iSJTU
 client for Humans. License: GPL-3.0-or-later Author-email: LightQuantum
 lightquantum.me> Requires-Python: >=3.8 Classifier: Environment :: Web
 Environment Classifier: Intended Audience :: Developers Classifier: Operating
 System :: OS Independent Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic
 Content Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Provides-Extra: docs Provides-Extra: ocr Provides-Extra: tests Project-
 URL: documentation, https://pysjtu.readthedocs.io/en/latest Project-URL:
```

