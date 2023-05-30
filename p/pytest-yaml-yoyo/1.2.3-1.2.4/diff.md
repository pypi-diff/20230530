# Comparing `tmp/pytest-yaml-yoyo-1.2.3.tar.gz` & `tmp/pytest-yaml-yoyo-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.3.tar", last modified: Mon May 29 07:10:43 2023, max compression
+gzip compressed data, was "dist\pytest-yaml-yoyo-1.2.4.tar", last modified: Tue May 30 00:50:39 2023, max compression
```

## Comparing `pytest-yaml-yoyo-1.2.3.tar` & `pytest-yaml-yoyo-1.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:10:43.134659 pytest-yaml-yoyo-1.2.3/
--rw-rw-rw-   0        0        0    23692 2023-05-29 07:10:43.132663 pytest-yaml-yoyo-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    23193 2023-05-20 01:43:47.000000 pytest-yaml-yoyo-1.2.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-29 07:10:43.134659 pytest-yaml-yoyo-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-05-29 07:10:40.000000 pytest-yaml-yoyo-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:10:42.998644 pytest-yaml-yoyo-1.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 07:10:43.107729 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/
--rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/create_funtion.py
--rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/db.py
--rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/exceptions.py
--rw-rw-rw-   0        0        0     3741 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/extract.py
--rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/http_session.py
--rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/log.py
--rw-rw-rw-   0        0        0     2734 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/my_builtins.py
--rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/parser.py
--rw-rw-rw-   0        0        0     9720 2023-05-29 07:10:40.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/plugin.py
--rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/render_template_obj.py
--rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/report_notify.py
--rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/request_session.py
--rw-rw-rw-   0        0        0    28418 2023-05-29 07:10:40.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/runner.py
--rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/swagger_parser.py
--rw-rw-rw-   0        0        0     3666 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/validate.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:10:43.130668 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/
--rw-rw-rw-   0        0        0    23692 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      839 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      188 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-29 07:10:42.000000 pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 00:50:39.469094 pytest-yaml-yoyo-1.2.4/
+-rw-rw-rw-   0        0        0    24830 2023-05-30 00:50:39.468098 pytest-yaml-yoyo-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    24331 2023-05-30 00:38:17.000000 pytest-yaml-yoyo-1.2.4/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-30 00:50:39.469094 pytest-yaml-yoyo-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-05-30 00:16:46.000000 pytest-yaml-yoyo-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:50:39.431172 pytest-yaml-yoyo-1.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 00:50:39.457126 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/
+-rw-rw-rw-   0        0        0        0 2022-11-23 03:54:21.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/create_funtion.py
+-rw-rw-rw-   0        0        0     2057 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/db.py
+-rw-rw-rw-   0        0        0      238 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/exceptions.py
+-rw-rw-rw-   0        0        0     4113 2023-05-30 00:16:10.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/extract.py
+-rw-rw-rw-   0        0        0     2059 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/http_session.py
+-rw-rw-rw-   0        0        0     2431 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/log.py
+-rw-rw-rw-   0        0        0     2734 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/my_builtins.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/parser.py
+-rw-rw-rw-   0        0        0     9720 2023-05-29 07:10:40.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/plugin.py
+-rw-rw-rw-   0        0        0     4966 2023-05-19 16:25:21.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/render_template_obj.py
+-rw-rw-rw-   0        0        0     1854 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/report_notify.py
+-rw-rw-rw-   0        0        0     1447 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/request_session.py
+-rw-rw-rw-   0        0        0    28695 2023-05-30 00:24:02.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/runner.py
+-rw-rw-rw-   0        0        0     7722 2023-05-19 16:11:50.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/swagger_parser.py
+-rw-rw-rw-   0        0        0     3666 2023-05-22 13:47:47.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/validate.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:50:39.467099 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/
+-rw-rw-rw-   0        0        0    24830 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      188 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-30 00:50:39.000000 pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/top_level.txt
```

### Comparing `pytest-yaml-yoyo-1.2.3/PKG-INFO` & `pytest-yaml-yoyo-1.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.3
+Version: 1.2.4
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -12,39 +12,45 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 
 pypi_seed
 =========
 基于 httprunner 框架的用例结构，我自己开发了一个pytest + yaml 的框架，那么是不是重复造轮子呢？
-不可否认 httprunner 框架设计非常优秀，但是也有缺点，httprunner3.x的版本虽然也是基于pytest框架设计，结合yaml执行用例，但是会生成一个py文件去执行。
-在辅助函数的引用也很局限，只能获取函数的返回值，不能在yaml中对返回值重新二次取值。
+不可否认 httprunner 框架设计非常优秀，但是也有缺点，httprunner3.x 的版本虽然也是基于 pytest 框架设计，结合 yaml 执行用例，但是会生成一个py文件去执行。
+在辅助函数的引用也很局限，只能获取函数的返回值，不能在 yaml 中对返回值重新二次取值。
 那么我的这个框架，就是为了解决这些痛点。。。。
 
 本插件可以实现以下优势：
 
-- 1、基于 pytest 框架安装插件即可使用，环境非常简单
-- 2、只需要写 yaml 文件用例即可运行，使用 pytest 运行的命令
-- 3、extract 功能实现多个接口步骤的参数关联
-- 4、全局仅登录一次，在用例中自动在请求头部添加 Authentication token认证
-- 5、用例参数化 parameters 功能实现
-- 6、yaml 中调用 fixture 功能实现
-- 7、yaml 中调用辅助函数功能使用
-- 8、yaml 中调用 hooks 功能
-- 9、用例分层机制：API和用例层
-- 10、支持 logging 日志
-- 11、支持 allure 报告
-- 12、支持mysql 数据库增删改查
-- 13、支持钉钉机器人通知
+-  1、基于 pytest 框架安装插件即可使用，环境非常简单
+-  2、只需要写 yaml 文件用例即可运行，使用 pytest 运行的命令
+-  3、extract 提取结果支持 jmespath、jsonpath、re 正则提取实现参数关联
+-  4、validate 丰富的校验方法
+-  5、全局仅登录一次，在用例中自动在请求头部添加 Authentication token认证
+-  6、用例参数化 parameters 功能实现
+-  7、export 提升变量为 session 会话级别，可以跨 yaml 文件传参
+-  8、yaml 中调用 fixture 功能实现
+-  9、yaml 中调用辅助函数功能使用
+-  10、yaml 中调用 hooks 功能
+-  11、用例分层机制：API 和用例层
+-  12、支持 logging 日志
+-  13、支持 allure 报告
+-  14、支持 mysql 数据库增删改查
+-  15、支持钉钉/飞书机器人通知测试结果和 allure 报告地址
+-  16、支持生成随机测试数据，如字符串，姓名，手机号，邮箱等
+-  17、根据 swagger.json 自动生成 yaml 文件接口用例
+-  18、支持全局代理配置
 
 联系我们
 --------------------------
 
-作者-上海悠悠 微信/QQ交流:283340479
-blog地址 https://www.cnblogs.com/yoyoketang/
+- 作者-上海悠悠 微信/QQ交流:283340479
+- blog地址 https://www.cnblogs.com/yoyoketang/
+- 视频教学 https://study.163.com/course/courseMain.htm?courseId=1213419817&share=2&shareId=480000002230338
 
 
 版本变更记录
 --------------------------
 
 v1.0.0
 发布的第一个版本（已删除)
@@ -170,19 +176,44 @@
 - 3.优化request 下的hook 功能
 - 4.其它细节优化
 
 v1.2.1 发布时间 2023-05-20
 
 优化以下问题
 
-1.兼容python3.8, python3.9, python3.10版本
-2.支持在case 用例中针对单个用例的参数化了
-3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
-4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
-5.内置to_json() 函数，字典转 json
+- 1.兼容python3.8, python3.9, python3.10版本
+- 2.支持在case 用例中针对单个用例的参数化了
+- 3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
+- 4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
+- 5.内置to_json() 函数，字典转 json
+
+v1.2.2 发布
+
+优化以下问题
+
+- 1.解决与 pytest-base-url 不兼容问题
+- 2.解决len_eq 断言 list 长度问题
+
+v1.2.3 发布 2023-05-29
+
+优化以下问题
+
+- 1.解决请求钩子函数中传环境配置问题
+- 2.新增内置fixture environ 返回当前运行环境对象
+- 3.报告总结加skip通过数量
+
+v1.2.4 发布 2023-05-30
+
+优化以下问题
+
+- 1.解决用例全部 skip 报错问题
+- 2.解决文件上传参数全部传 files 不生效问题
+- 3.数据库配置支持 DB_INFO 参数传字典类型
+- 4.jmespath 表达式支持 length 等函数的提取
+
 
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
 - Pytest 7.2.0+
```

### Comparing `pytest-yaml-yoyo-1.2.3/README.rst` & `pytest-yaml-yoyo-1.2.4/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 pypi_seed
 =========
 基于 httprunner 框架的用例结构，我自己开发了一个pytest + yaml 的框架，那么是不是重复造轮子呢？
-不可否认 httprunner 框架设计非常优秀，但是也有缺点，httprunner3.x的版本虽然也是基于pytest框架设计，结合yaml执行用例，但是会生成一个py文件去执行。
-在辅助函数的引用也很局限，只能获取函数的返回值，不能在yaml中对返回值重新二次取值。
+不可否认 httprunner 框架设计非常优秀，但是也有缺点，httprunner3.x 的版本虽然也是基于 pytest 框架设计，结合 yaml 执行用例，但是会生成一个py文件去执行。
+在辅助函数的引用也很局限，只能获取函数的返回值，不能在 yaml 中对返回值重新二次取值。
 那么我的这个框架，就是为了解决这些痛点。。。。
 
 本插件可以实现以下优势：
 
-- 1、基于 pytest 框架安装插件即可使用，环境非常简单
-- 2、只需要写 yaml 文件用例即可运行，使用 pytest 运行的命令
-- 3、extract 功能实现多个接口步骤的参数关联
-- 4、全局仅登录一次，在用例中自动在请求头部添加 Authentication token认证
-- 5、用例参数化 parameters 功能实现
-- 6、yaml 中调用 fixture 功能实现
-- 7、yaml 中调用辅助函数功能使用
-- 8、yaml 中调用 hooks 功能
-- 9、用例分层机制：API和用例层
-- 10、支持 logging 日志
-- 11、支持 allure 报告
-- 12、支持mysql 数据库增删改查
-- 13、支持钉钉机器人通知
+-  1、基于 pytest 框架安装插件即可使用，环境非常简单
+-  2、只需要写 yaml 文件用例即可运行，使用 pytest 运行的命令
+-  3、extract 提取结果支持 jmespath、jsonpath、re 正则提取实现参数关联
+-  4、validate 丰富的校验方法
+-  5、全局仅登录一次，在用例中自动在请求头部添加 Authentication token认证
+-  6、用例参数化 parameters 功能实现
+-  7、export 提升变量为 session 会话级别，可以跨 yaml 文件传参
+-  8、yaml 中调用 fixture 功能实现
+-  9、yaml 中调用辅助函数功能使用
+-  10、yaml 中调用 hooks 功能
+-  11、用例分层机制：API 和用例层
+-  12、支持 logging 日志
+-  13、支持 allure 报告
+-  14、支持 mysql 数据库增删改查
+-  15、支持钉钉/飞书机器人通知测试结果和 allure 报告地址
+-  16、支持生成随机测试数据，如字符串，姓名，手机号，邮箱等
+-  17、根据 swagger.json 自动生成 yaml 文件接口用例
+-  18、支持全局代理配置
 
 联系我们
 --------------------------
 
-作者-上海悠悠 微信/QQ交流:283340479
-blog地址 https://www.cnblogs.com/yoyoketang/
+- 作者-上海悠悠 微信/QQ交流:283340479
+- blog地址 https://www.cnblogs.com/yoyoketang/
+- 视频教学 https://study.163.com/course/courseMain.htm?courseId=1213419817&share=2&shareId=480000002230338
 
 
 版本变更记录
 --------------------------
 
 v1.0.0
 发布的第一个版本（已删除)
@@ -155,19 +161,44 @@
 - 3.优化request 下的hook 功能
 - 4.其它细节优化
 
 v1.2.1 发布时间 2023-05-20
 
 优化以下问题
 
-1.兼容python3.8, python3.9, python3.10版本
-2.支持在case 用例中针对单个用例的参数化了
-3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
-4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
-5.内置to_json() 函数，字典转 json
+- 1.兼容python3.8, python3.9, python3.10版本
+- 2.支持在case 用例中针对单个用例的参数化了
+- 3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
+- 4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
+- 5.内置to_json() 函数，字典转 json
+
+v1.2.2 发布
+
+优化以下问题
+
+- 1.解决与 pytest-base-url 不兼容问题
+- 2.解决len_eq 断言 list 长度问题
+
+v1.2.3 发布 2023-05-29
+
+优化以下问题
+
+- 1.解决请求钩子函数中传环境配置问题
+- 2.新增内置fixture environ 返回当前运行环境对象
+- 3.报告总结加skip通过数量
+
+v1.2.4 发布 2023-05-30
+
+优化以下问题
+
+- 1.解决用例全部 skip 报错问题
+- 2.解决文件上传参数全部传 files 不生效问题
+- 3.数据库配置支持 DB_INFO 参数传字典类型
+- 4.jmespath 表达式支持 length 等函数的提取
+
 
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
 - Pytest 7.2.0+
```

### Comparing `pytest-yaml-yoyo-1.2.3/setup.py` & `pytest-yaml-yoyo-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 作者-上海悠悠 微信wx:283340479
 # blog地址 https://www.cnblogs.com/yoyoketang/
 """
 
 setup(
     name='pytest-yaml-yoyo',
     url='https://github.com/yoyoketang/pytest-yaml-yoyo',
-    version='v1.2.3',
+    version='v1.2.4',
     author="上海-悠悠",
     author_email='283340479@qq.com',
     description='http/https API run by yaml',
     long_description=open("README.rst", encoding='utf-8').read(),
     package_dir={"": "src"},
     packages=["pytest_yaml_yoyo"],
     classifiers=[
```

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/create_funtion.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/create_funtion.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/db.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/db.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/extract.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/extract.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,20 @@
             response_parse_dict = response.json()
             return extract_by_jsonpath(response_parse_dict, extract_expression)
         except Exception as msg:
             raise exceptions.ExtractExpressionError(f'expression:<{extract_expression}>, error: {msg}')
     elif '.+?' in extract_expression or '.*?' in extract_expression:
         # 正则匹配
         return extract_by_regex(response.text, extract_expression)
+    elif 'body.' in extract_expression or 'content.' in extract_expression:
+        try:
+            response_parse_dict = response.json()
+            return extract_by_jmespath({"body": response_parse_dict}, extract_expression)
+        except Exception as msg:
+            raise exceptions.ExtractExpressionError(f'expression:<{extract_expression}>, error: {msg}')
     else:
         # 其它非取值表达式，直接返回
         return extract_expression
 
 def extract_by_jsonpath(extract_value: dict, extract_expression: str): # noqa
     """
         json path 取值
```

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/http_session.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/http_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/log.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/log.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/my_builtins.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/my_builtins.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/plugin.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/render_template_obj.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/render_template_obj.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/report_notify.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/report_notify.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/request_session.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/request_session.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/runner.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,27 +501,30 @@
                         getattr(validate, check_type)(actual_value, expect_value)
                     else:
                         log.error(f'{check_type}  not valid check type')
 
     def execute_mysql(self):
         """执行 mysql 操作"""
         env_obj = self.g.get('env')  # 获取环境配置
-        if not hasattr(env_obj, 'MYSQL_HOST'):
+        if not hasattr(env_obj, 'MYSQL_HOST') and not hasattr(env_obj, 'DB_INFO'):
             return {
-                "query_sql": lambda x: log.error("MYSQL_HOST not found in config.py"),
-                "execute_sql": lambda x: log.error("MYSQL_HOST not found in config.py")
+                "query_sql": lambda x: log.error("MYSQL_HOST or DB_INFO  not found in config.py"),
+                "execute_sql": lambda x: log.error("MYSQL_HOST or DB_INFO not found in config.py")
             }
         try:
-            db = ConnectMysql(
-                host=env_obj.MYSQL_HOST,
-                user=env_obj.MYSQL_USER,
-                password=env_obj.MYSQL_PASSWORD,
-                port=env_obj.MYSQL_PORT,
-                database=env_obj.MYSQL_DATABASE,
-            )
+            if hasattr(env_obj, 'DB_INFO'):
+                db = ConnectMysql(**env_obj.DB_INFO)
+            else:
+                db = ConnectMysql(
+                    host=env_obj.MYSQL_HOST,
+                    user=env_obj.MYSQL_USER,
+                    password=env_obj.MYSQL_PASSWORD,
+                    port=env_obj.MYSQL_PORT,
+                    database=env_obj.MYSQL_DATABASE,
+                )
             return {
                 "query_sql": db.query_sql,
                 "execute_sql": db.execute_sql
             }
         except Exception as msg:
             log.error(f'mysql init error: {msg}')
             return {
@@ -547,14 +550,16 @@
             data = request_value.get('data', {})
             fields.extend(data.items())  # 添加data数据
             for key, value in request_value.get('files', {}).items():
                 if Path(root_dir).joinpath(value).is_file():
                     fields.append(
                         (key, self.upload_file(Path(root_dir).joinpath(value).resolve()))
                     )
+                else:
+                    fields.append((key, value))
             m = MultipartEncoder(
                 fields=fields
             )
             request_value.pop('files')  # 去掉 files 参数
             request_value['data'] = m
             new_headers = request_value.get('headers', {})
             new_headers.update({'Content-Type': m.content_type})
```

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/swagger_parser.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo/validate.py` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo/validate.py`

 * *Files identical despite different names*

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/PKG-INFO` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-yaml-yoyo
-Version: 1.2.3
+Version: 1.2.4
 Summary: http/https API run by yaml
 Home-page: https://github.com/yoyoketang/pytest-yaml-yoyo
 Author: 上海-悠悠
 Author-email: 283340479@qq.com
 License: proprietary
 Keywords: pytest,py.test,pytest-yaml,pytest-yaml-yoyo
 Classifier: Framework :: Pytest
@@ -12,39 +12,45 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 
 pypi_seed
 =========
 基于 httprunner 框架的用例结构，我自己开发了一个pytest + yaml 的框架，那么是不是重复造轮子呢？
-不可否认 httprunner 框架设计非常优秀，但是也有缺点，httprunner3.x的版本虽然也是基于pytest框架设计，结合yaml执行用例，但是会生成一个py文件去执行。
-在辅助函数的引用也很局限，只能获取函数的返回值，不能在yaml中对返回值重新二次取值。
+不可否认 httprunner 框架设计非常优秀，但是也有缺点，httprunner3.x 的版本虽然也是基于 pytest 框架设计，结合 yaml 执行用例，但是会生成一个py文件去执行。
+在辅助函数的引用也很局限，只能获取函数的返回值，不能在 yaml 中对返回值重新二次取值。
 那么我的这个框架，就是为了解决这些痛点。。。。
 
 本插件可以实现以下优势：
 
-- 1、基于 pytest 框架安装插件即可使用，环境非常简单
-- 2、只需要写 yaml 文件用例即可运行，使用 pytest 运行的命令
-- 3、extract 功能实现多个接口步骤的参数关联
-- 4、全局仅登录一次，在用例中自动在请求头部添加 Authentication token认证
-- 5、用例参数化 parameters 功能实现
-- 6、yaml 中调用 fixture 功能实现
-- 7、yaml 中调用辅助函数功能使用
-- 8、yaml 中调用 hooks 功能
-- 9、用例分层机制：API和用例层
-- 10、支持 logging 日志
-- 11、支持 allure 报告
-- 12、支持mysql 数据库增删改查
-- 13、支持钉钉机器人通知
+-  1、基于 pytest 框架安装插件即可使用，环境非常简单
+-  2、只需要写 yaml 文件用例即可运行，使用 pytest 运行的命令
+-  3、extract 提取结果支持 jmespath、jsonpath、re 正则提取实现参数关联
+-  4、validate 丰富的校验方法
+-  5、全局仅登录一次，在用例中自动在请求头部添加 Authentication token认证
+-  6、用例参数化 parameters 功能实现
+-  7、export 提升变量为 session 会话级别，可以跨 yaml 文件传参
+-  8、yaml 中调用 fixture 功能实现
+-  9、yaml 中调用辅助函数功能使用
+-  10、yaml 中调用 hooks 功能
+-  11、用例分层机制：API 和用例层
+-  12、支持 logging 日志
+-  13、支持 allure 报告
+-  14、支持 mysql 数据库增删改查
+-  15、支持钉钉/飞书机器人通知测试结果和 allure 报告地址
+-  16、支持生成随机测试数据，如字符串，姓名，手机号，邮箱等
+-  17、根据 swagger.json 自动生成 yaml 文件接口用例
+-  18、支持全局代理配置
 
 联系我们
 --------------------------
 
-作者-上海悠悠 微信/QQ交流:283340479
-blog地址 https://www.cnblogs.com/yoyoketang/
+- 作者-上海悠悠 微信/QQ交流:283340479
+- blog地址 https://www.cnblogs.com/yoyoketang/
+- 视频教学 https://study.163.com/course/courseMain.htm?courseId=1213419817&share=2&shareId=480000002230338
 
 
 版本变更记录
 --------------------------
 
 v1.0.0
 发布的第一个版本（已删除)
@@ -170,19 +176,44 @@
 - 3.优化request 下的hook 功能
 - 4.其它细节优化
 
 v1.2.1 发布时间 2023-05-20
 
 优化以下问题
 
-1.兼容python3.8, python3.9, python3.10版本
-2.支持在case 用例中针对单个用例的参数化了
-3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
-4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
-5.内置to_json() 函数，字典转 json
+- 1.兼容python3.8, python3.9, python3.10版本
+- 2.支持在case 用例中针对单个用例的参数化了
+- 3.参数化数据支持读取外部文件，文件格式可以支持：txt/csv/json/yaml
+- 4.函数的参数可以引用变量了，如: ${fun("hello ${key}")}
+- 5.内置to_json() 函数，字典转 json
+
+v1.2.2 发布
+
+优化以下问题
+
+- 1.解决与 pytest-base-url 不兼容问题
+- 2.解决len_eq 断言 list 长度问题
+
+v1.2.3 发布 2023-05-29
+
+优化以下问题
+
+- 1.解决请求钩子函数中传环境配置问题
+- 2.新增内置fixture environ 返回当前运行环境对象
+- 3.报告总结加skip通过数量
+
+v1.2.4 发布 2023-05-30
+
+优化以下问题
+
+- 1.解决用例全部 skip 报错问题
+- 2.解决文件上传参数全部传 files 不生效问题
+- 3.数据库配置支持 DB_INFO 参数传字典类型
+- 4.jmespath 表达式支持 length 等函数的提取
+
 
 Installation / 安装
 --------------------------
 最佳环境体验
 
 - Python 3.8, 3.9. 3.10 版本
 - Pytest 7.2.0+
```

### Comparing `pytest-yaml-yoyo-1.2.3/src/pytest_yaml_yoyo.egg-info/SOURCES.txt` & `pytest-yaml-yoyo-1.2.4/src/pytest_yaml_yoyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

