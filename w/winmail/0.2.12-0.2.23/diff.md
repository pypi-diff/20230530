# Comparing `tmp/winmail-0.2.12-py3-none-any.whl.zip` & `tmp/winmail-0.2.23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 17888 bytes, number of entries: 14
+Zip file size: 18125 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    14874 b- defN 22-Dec-09 00:24 winmail/Api_1_2.py
 -rw-rw-rw-  2.0 fat     4032 b- defN 22-Aug-23 02:03 winmail/ComApi.py
--rw-rw-rw-  2.0 fat     6839 b- defN 22-Dec-09 08:02 winmail/OpenApi.py
--rw-rw-rw-  2.0 fat    26241 b- defN 22-Nov-11 05:07 winmail/Winmail.py
--rw-rw-rw-  2.0 fat      273 b- defN 22-Sep-30 00:58 winmail/__init__.py
+-rw-rw-rw-  2.0 fat     7006 b- defN 23-May-11 01:16 winmail/OpenApi.py
+-rw-rw-rw-  2.0 fat    26507 b- defN 23-May-30 07:16 winmail/Winmail.py
+-rw-rw-rw-  2.0 fat      335 b- defN 23-May-30 07:25 winmail/__init__.py
 -rw-rw-rw-  2.0 fat     1983 b- defN 22-Nov-11 03:15 winmail/utils/MysqlClass.py
 -rw-rw-rw-  2.0 fat      577 b- defN 22-Sep-30 00:56 winmail/utils/Other.py
 -rw-rw-rw-  2.0 fat     1822 b- defN 22-Nov-11 04:02 winmail/utils/PostgreClass.py
 -rw-rw-rw-  2.0 fat     1728 b- defN 22-Nov-11 02:28 winmail/utils/SqliteClass.py
 -rw-rw-rw-  2.0 fat      296 b- defN 22-Nov-11 05:03 winmail/utils/__init__.py
--rw-rw-rw-  2.0 fat     5614 b- defN 22-Dec-09 09:37 winmail-0.2.12.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Dec-09 09:37 winmail-0.2.12.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 22-Dec-09 09:37 winmail-0.2.12.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1091 b- defN 22-Dec-09 09:37 winmail-0.2.12.dist-info/RECORD
-14 files, 65470 bytes uncompressed, 16096 bytes compressed:  75.4%
+-rw-rw-rw-  2.0 fat     5619 b- defN 23-May-30 07:34 winmail-0.2.23.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 07:34 winmail-0.2.23.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-30 07:34 winmail-0.2.23.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1091 b- defN 23-May-30 07:34 winmail-0.2.23.dist-info/RECORD
+14 files, 65970 bytes uncompressed, 16333 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: winmail/utils/SqliteClass.py
 Comment: 
 
 Filename: winmail/utils/__init__.py
 Comment: 
 
-Filename: winmail-0.2.12.dist-info/METADATA
+Filename: winmail-0.2.23.dist-info/METADATA
 Comment: 
 
-Filename: winmail-0.2.12.dist-info/WHEEL
+Filename: winmail-0.2.23.dist-info/WHEEL
 Comment: 
 
-Filename: winmail-0.2.12.dist-info/top_level.txt
+Filename: winmail-0.2.23.dist-info/top_level.txt
 Comment: 
 
-Filename: winmail-0.2.12.dist-info/RECORD
+Filename: winmail-0.2.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## winmail/OpenApi.py

```diff
@@ -171,16 +171,23 @@
 
         :return: JSON {result: ok/error, info: ""}
         """
 
         param_dict: Dict[str, Any] = kwargs
 
         if not self.url or not self.sessid:
+
+            self_name = self.__class__.__name__
+
+            for name, obj in globals().items():
+                if obj is self:
+                    self_name = repr(name)
+
             return {"result": "error",
-                    "info": "Use login first %s.login(user, pwd, manage_path) " % self.__class__.__name__}
+                    "info": "Use login first %s.login(user, pwd, manage_path) " % self_name}
 
         timestamp = str(int(time.time()))
 
         if 'sessid' not in param_dict:
             param_dict.update({'sessid': self.sessid})
         if 'apikey' not in param_dict:
             param_dict.update({"apikey": self.apikey})
```

## winmail/Winmail.py

```diff
@@ -209,14 +209,15 @@
     else:
         raise Exception(error_info)
 
 
 class Winmail:
     """
     获取各Winmail相关的路径
+    建议使用OpenAPI接口，此方法直接读取后台配置文件和数据库。对版本符合度要求高。测试版本为Winmail 6.7、7.0
     """
 
     def __init__(self, db_pwd=None):
 
         self.winmail_path = get_winmail_path()
 
         self.winmail_sys_conf_path = os.path.join(self.winmail_path, "data//system.cfg")
@@ -252,14 +253,16 @@
             self.db_host = get_xml_element_value(self.winmail_sys_conf_path, f'./dboption/{self.db_type}/host')
             self.db_port = int(get_xml_element_value(self.winmail_sys_conf_path, f'./dboption/{self.db_type}/port'))
             if self.db_type == 'mysqlin':
                 self.db_user = 'root'
             else:
                 self.db_user = get_xml_element_value(self.winmail_sys_conf_path, f'./dboption/{self.db_type}/username')
             self.db_database = get_xml_element_value(self.winmail_sys_conf_path, f'./dboption/{self.db_type}/database')
+        else:
+            raise Exception("Get Winmail Database Type Error : self.db_type -> %s;" % self.db_type)
 
     def connect_db(self, sqlite_db_path: str = None):
         """
         按数据库类型打开数据库
 
         :return: Object
         """
```

## winmail/__init__.py

```diff
@@ -1,8 +1,13 @@
 # -*- coding:utf-8 -*-
 
 from .OpenApi import OpenApi
-from .ComApi import ComApi
 from .Winmail import Winmail
 from .utils import start_winmail_service, stop_winmail_service
 
-__all__ = ["OpenApi", "ComApi", "Winmail", "start_winmail_service", "stop_winmail_service"]
+__all__ = ["OpenApi", "Winmail", "start_winmail_service", "stop_winmail_service"]
+
+import os
+if os.name == "nt":
+    from .ComApi import ComApi
+    
+    __all__.append("ComApi")
```

## Comparing `winmail-0.2.12.dist-info/METADATA` & `winmail-0.2.23.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winmail
-Version: 0.2.12
+Version: 0.2.23
 Summary: Winmail API
 Home-page: http://winmail.cn
 Author: Sway
 Author-email: sway_wang@foxmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
@@ -30,70 +30,23 @@
 
 ```bash
 pip install winmail
 ```
 
 ## 使用说明
 
-### Winmail模块说明
-
-:warning:Python必须运行在Winmail服务器上。
-
-Winmail模板主要提供Winmail相关的参数路径获取。比如安装目录，域的邮件、网盘存储目录，用户邮件、网盘存储目录等。
-
-也可以获取域名，用户，组列表。但比较建议使用后面一项的OpenAPI接口。
-
-#### 初始化和数据库连接说明
-
-已经支持的数据库为Sqlite、mysql。
-
-##### 导入Winmail
-```python
-from winmail import Winmail
-wm = Winmail()
-print(wm.get_mailarchive_path())
-print(wm.get_user_alias_list())
-# 按XML路径获取system.cfg中的配置项
-print(wm.get_sys_config("./dboption/dbtype"))
-```
-属性包含：
-```python
-winmail_path,winmail_sys_conf_path,winmail_domain_conf_path,winmail_mailgroup_conf_path,winmail_mailuser_stat_conf_path,winmail_mailuser_conf_path,db_type
-```
-
-方法包含：
-
-```python
-connect_db,get_sys_config,get_db_type,check_winmail_path,get_user_mailstore_path,get_user_netstore_path,get_domain_mailstore_path,get_domain_netstore_path,get_mailbackup_path,get_mailarchive_path,get_pri_domain,get_domain_list,get_all_domain_list,	get_domain_tuple_list,get_user_list,get_user_alias_list,get_group_list,check_pri_domain
-```
-
-
-
-Winmail中如果使用了Mysql数据库，请在实例化时初始化数据库密码。如：
-```python
-from winmail import Winmail
-wm = Winmail('mysql-password')
-wm.connect_db()
-```
-如果Winmail中使用了Sqlite数据库，实例化时不需要密码。但在使用connect_db时，必须指定Sqlite操作的数据库文件路径，如：
-```python
-from winmail import Winmail
-wm = Winmail()
-wm.connect_db(wm.winmail_mailuser_conf_path)
-```
-
 ### OpenAPI说明
 
 可以使用HTTP、HTTPS请求，不检查证书。具体OpenApi的接口完整手册请查看Winmail官方文档。
 
 ```python
 
 from winmail import OpenApi as WinmailApi
 
-server = '192.168.120.195'
+server = '192.168.1.195'
 port = 6080
 apikey = 'bt66oa8d5b'
 apisecret = 'btt87e78f6871aea2016a3916eb65299b7affb18'
 
 # 管理员接口示例
 manage_path = 'admin'
 user = 'admin'
@@ -150,24 +103,24 @@
     method_result = api.get_api(**method_params)
     if method_result['result'] != 'ok':
         print(method_result)
 
     # 第一次上传多个附件
     method_params = {
         "method": "upload.upload",
-        "attachfile": ['E://magic winmail//server//logs//webmail.log',
-                'E://magic winmail//server//logs//system.log']
+        "attachfile": ['E://logs//webmail.log',
+                'E://logs//system.log']
     }
     method_result = api.get_api(**method_params)
     if method_result['result'] != 'ok':
         print(method_result)
     # 第二次上传单个附件
     method_params = {
         "method": "upload.upload",
-        "attachfile": 'E://magic winmail//server//logs//admin.log'
+        "attachfile": 'E://logs//admin.log'
     }
     method_result = api.get_api(**method_params)
     if method_result['result'] != 'ok':
         print(method_result)
 
     # 写邮件信体
     method_params = {
@@ -186,14 +139,84 @@
     else:
         print(method_result)
 
 else:
     print(login_result)
 ```
 
+### Winmail模块说明
+
+:warning:Python必须运行在Winmail服务器上。
+
+Winmail模板主要提供Winmail相关的参数路径获取。比如安装目录，域的邮件、网盘存储目录，用户邮件、网盘存储目录等。
+
+也可以获取域名，用户，组列表。因为是直接读取配置文件和数据库，Openapi有接口的，建议使用OpenAPI接口。
+
+#### 初始化和数据库连接说明
+
+已经支持的数据库为Sqlite、mysql、postgresql。
+
+##### 导入Winmail
+```python
+from winmail import Winmail
+wm = Winmail()
+print(wm.get_mailarchive_path())
+print(wm.get_user_alias_list())
+# 按XML路径获取system.cfg中的配置项
+print(wm.get_sys_config("./dboption/dbtype"))
+```
+属性包含：
+```txt
+winmail_path,
+winmail_sys_conf_path,
+winmail_domain_conf_path,
+winmail_mailgroup_conf_path,
+winmail_mailuser_stat_conf_path,
+winmail_mailuser_conf_path,
+db_type
+```
+
+方法包含：
+
+```txt
+connect_db,
+get_sys_config,
+get_db_type,
+check_winmail_path,
+get_user_mailstore_path,
+get_user_netstore_path,
+get_domain_mailstore_path,
+get_domain_netstore_path,
+get_mailbackup_path,
+get_mailarchive_path,
+get_pri_domain,
+get_domain_list,
+get_all_domain_list,	
+get_domain_tuple_list,
+get_user_list,
+get_user_alias_list,
+get_group_list,
+check_pri_domain
+```
+
+
+
+Winmail中如果使用了Mysql数据库，请在实例化时初始化数据库密码。如：
+```python
+from winmail import Winmail
+wm = Winmail('mysql-password')
+wm.connect_db()
+```
+如果Winmail中使用了Sqlite数据库，实例化时不需要密码。但在使用connect_db时，必须指定Sqlite操作的数据库文件路径，如：
+```python
+from winmail import Winmail
+wm = Winmail()
+wm.connect_db(wm.winmail_mailuser_conf_path)
+```
+
 ### Com接口说明
 
 :warning:Python必须运行在Winmail服务器上。
 
 请参考Winmail的Com接口文档。
 暂未全部完成Com接口。
```

