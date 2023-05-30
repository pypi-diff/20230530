# Comparing `tmp/pywencai-0.8.6.tar.gz` & `tmp/pywencai-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.8.6.tar", max compression
+gzip compressed data, was "pywencai-0.8.7.tar", max compression
```

## Comparing `pywencai-0.8.6.tar` & `pywencai-0.8.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-15 02:01:42.979657 pywencai-0.8.6/LICENSE
--rw-r--r--   0        0        0     2836 2023-05-15 02:01:42.979657 pywencai-0.8.6/README.md
--rw-r--r--   0        0        0      612 2023-05-15 02:01:42.979657 pywencai-0.8.6/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-15 02:01:42.979657 pywencai-0.8.6/pywencai/__init__.py
--rw-r--r--   0        0        0     4746 2023-05-15 02:01:42.979657 pywencai-0.8.6/pywencai/convert.py
--rw-r--r--   0        0        0      433 2023-05-15 02:01:42.979657 pywencai-0.8.6/pywencai/headers.py
--rw-r--r--   0        0        0    39677 2023-05-15 02:01:42.979657 pywencai-0.8.6/pywencai/hexin-v.js
--rw-r--r--   0        0        0     4187 2023-05-15 02:01:42.983657 pywencai-0.8.6/pywencai/wencai.py
--rw-r--r--   0        0        0     3460 1970-01-01 00:00:00.000000 pywencai-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-30 16:15:26.783706 pywencai-0.8.7/LICENSE
+-rw-r--r--   0        0        0     3043 2023-05-30 16:15:26.783706 pywencai-0.8.7/README.md
+-rw-r--r--   0        0        0      612 2023-05-30 16:15:26.787706 pywencai-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/__init__.py
+-rw-r--r--   0        0        0     4816 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/convert.py
+-rw-r--r--   0        0        0      433 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/headers.py
+-rw-r--r--   0        0        0    39677 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     4303 2023-05-30 16:15:26.787706 pywencai-0.8.7/pywencai/wencai.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 pywencai-0.8.7/PKG-INFO
```

### Comparing `pywencai-0.8.6/LICENSE` & `pywencai-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.6/README.md` & `pywencai-0.8.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -87,29 +87,33 @@
 
 #### sleep
 
 非必填，默认为0，表示循环请求时，每次请求间隔多少秒。
 
 #### log
 
-非必填，默认为Flase，是否在控制台打印日志。
+非必填，默认为`False`，是否在控制台打印日志。
 
 #### cookie
 
 非必填，默认为None，付费版可以尝试传入cookie，获取付费使用权限。
 
 #### request_params
 
 非必填，默认为`{}`，可以设置额外的request参数
 
 ```python
 pywencai.get(question='昨日涨幅', sort_order='asc', loop=True, log=True, request_params={ 'proxies': proxies, 'timeout': (5, 10) })
 ```
 > 具体参数参看：[https://requests.readthedocs.io/en/latest/api/#requests.request](https://requests.readthedocs.io/en/latest/api/#requests.request)
 
+#### no_detail
+
+非必填，默认为`False`，当为`True`时，查询一些**详情类问题**不再会返回字典，而返回`None`，可以保证查询结果类型一直为`pd.DataFrame`或`None`。
+
 ### 返回值
 
 当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
 
 当查询的是详情时，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
 
 ## 联系方式
```

### Comparing `pywencai-0.8.6/pyproject.toml` & `pywencai-0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.8.6"
+version = "0.8.7"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.8.6/pywencai/convert.py` & `pywencai-0.8.7/pywencai/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,18 @@
         res = rq.request(
             method='GET',
             url=f'http://www.iwencai.com{url}',
             headers=headers()
         )
         result = json.loads(res.text)
         wcomp = result.get('data')
-        return show_type_handler(wcomp, comps)
+        if wcomp is not None:
+            return show_type_handler(wcomp, comps)
+        else:
+            return {}
     return {}
 
 
 
 show_type_handler_dict = {
     'xuangu_tableV1': xuangu_tableV1_handler,
     'container': container_handler,
```

### Comparing `pywencai-0.8.6/pywencai/hexin-v.js` & `pywencai-0.8.7/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.8.6/pywencai/wencai.py` & `pywencai-0.8.7/pywencai/wencai.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,8 +154,12 @@
     if condition is not None:
         kwargs = {**kwargs, **data}
         if loop:
             return loop_page(loop, **kwargs)
         else:
             return get_page(**kwargs)
     else:
-        return data
+        no_detail = kwargs.get('no_detail')
+        if no_detail != True:
+            return data
+        else:
+            return None
```

### Comparing `pywencai-0.8.6/PKG-INFO` & `pywencai-0.8.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.8.6
+Version: 0.8.7
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -106,29 +106,33 @@
 
 #### sleep
 
 非必填，默认为0，表示循环请求时，每次请求间隔多少秒。
 
 #### log
 
-非必填，默认为Flase，是否在控制台打印日志。
+非必填，默认为`False`，是否在控制台打印日志。
 
 #### cookie
 
 非必填，默认为None，付费版可以尝试传入cookie，获取付费使用权限。
 
 #### request_params
 
 非必填，默认为`{}`，可以设置额外的request参数
 
 ```python
 pywencai.get(question='昨日涨幅', sort_order='asc', loop=True, log=True, request_params={ 'proxies': proxies, 'timeout': (5, 10) })
 ```
 > 具体参数参看：[https://requests.readthedocs.io/en/latest/api/#requests.request](https://requests.readthedocs.io/en/latest/api/#requests.request)
 
+#### no_detail
+
+非必填，默认为`False`，当为`True`时，查询一些**详情类问题**不再会返回字典，而返回`None`，可以保证查询结果类型一直为`pd.DataFrame`或`None`。
+
 ### 返回值
 
 当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
 
 当查询的是详情时，该方法返回一个字典，字典中可能包含若干个文本和`Dataframe`
 
 ## 联系方式
```

