# Comparing `tmp/winmail-0.2.23-py3-none-any.whl.zip` & `tmp/winmail-0.2.23.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18125 bytes, number of entries: 14
+Zip file size: 18204 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat    14874 b- defN 22-Dec-09 00:24 winmail/Api_1_2.py
 -rw-rw-rw-  2.0 fat     4032 b- defN 22-Aug-23 02:03 winmail/ComApi.py
 -rw-rw-rw-  2.0 fat     7006 b- defN 23-May-11 01:16 winmail/OpenApi.py
--rw-rw-rw-  2.0 fat    26507 b- defN 23-May-30 07:16 winmail/Winmail.py
+-rw-rw-rw-  2.0 fat    26582 b- defN 23-May-30 08:43 winmail/Winmail.py
 -rw-rw-rw-  2.0 fat      335 b- defN 23-May-30 07:25 winmail/__init__.py
 -rw-rw-rw-  2.0 fat     1983 b- defN 22-Nov-11 03:15 winmail/utils/MysqlClass.py
 -rw-rw-rw-  2.0 fat      577 b- defN 22-Sep-30 00:56 winmail/utils/Other.py
 -rw-rw-rw-  2.0 fat     1822 b- defN 22-Nov-11 04:02 winmail/utils/PostgreClass.py
 -rw-rw-rw-  2.0 fat     1728 b- defN 22-Nov-11 02:28 winmail/utils/SqliteClass.py
 -rw-rw-rw-  2.0 fat      296 b- defN 22-Nov-11 05:03 winmail/utils/__init__.py
--rw-rw-rw-  2.0 fat     5619 b- defN 23-May-30 07:34 winmail-0.2.23.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 07:34 winmail-0.2.23.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-30 07:34 winmail-0.2.23.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1091 b- defN 23-May-30 07:34 winmail-0.2.23.dist-info/RECORD
-14 files, 65970 bytes uncompressed, 16333 bytes compressed:  75.2%
+-rw-rw-rw-  2.0 fat     5764 b- defN 23-May-30 08:59 winmail-0.2.23.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 08:59 winmail-0.2.23.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-30 08:59 winmail-0.2.23.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1099 b- defN 23-May-30 08:59 winmail-0.2.23.5.dist-info/RECORD
+14 files, 66198 bytes uncompressed, 16396 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: winmail/utils/SqliteClass.py
 Comment: 
 
 Filename: winmail/utils/__init__.py
 Comment: 
 
-Filename: winmail-0.2.23.dist-info/METADATA
+Filename: winmail-0.2.23.5.dist-info/METADATA
 Comment: 
 
-Filename: winmail-0.2.23.dist-info/WHEEL
+Filename: winmail-0.2.23.5.dist-info/WHEEL
 Comment: 
 
-Filename: winmail-0.2.23.dist-info/top_level.txt
+Filename: winmail-0.2.23.5.dist-info/top_level.txt
 Comment: 
 
-Filename: winmail-0.2.23.dist-info/RECORD
+Filename: winmail-0.2.23.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## winmail/Winmail.py

```diff
@@ -253,15 +253,16 @@
             self.db_host = get_xml_element_value(self.winmail_sys_conf_path, f'./dboption/{self.db_type}/host')
             self.db_port = int(get_xml_element_value(self.winmail_sys_conf_path, f'./dboption/{self.db_type}/port'))
             if self.db_type == 'mysqlin':
                 self.db_user = 'root'
             else:
                 self.db_user = get_xml_element_value(self.winmail_sys_conf_path, f'./dboption/{self.db_type}/username')
             self.db_database = get_xml_element_value(self.winmail_sys_conf_path, f'./dboption/{self.db_type}/database')
-        else:
+
+        if self.db_type and self.db_type != 'sqlite' and self.db_type not in DB_TYPES:
             raise Exception("Get Winmail Database Type Error : self.db_type -> %s;" % self.db_type)
 
     def connect_db(self, sqlite_db_path: str = None):
         """
         按数据库类型打开数据库
 
         :return: Object
```

## Comparing `winmail-0.2.23.dist-info/METADATA` & `winmail-0.2.23.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winmail
-Version: 0.2.23
+Version: 0.2.23.5
 Summary: Winmail API
 Home-page: http://winmail.cn
 Author: Sway
 Author-email: sway_wang@foxmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
@@ -30,14 +30,22 @@
 
 ```bash
 pip install winmail
 ```
 
 ## 使用说明
 
+服务启停：
+```python
+from winmail import start_winmail_service, stop_winmail_service
+
+start_winmail_service()
+stop_winmail_service()
+```
+
 ### OpenAPI说明
 
 可以使用HTTP、HTTPS请求，不检查证书。具体OpenApi的接口完整手册请查看Winmail官方文档。
 
 ```python
 
 from winmail import OpenApi as WinmailApi
```

## Comparing `winmail-0.2.23.dist-info/RECORD` & `winmail-0.2.23.5.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 winmail/Api_1_2.py,sha256=eUWBZqWk_jOl9iT77BYl1XN0wV54Ou-c7cPSx2MfLxc,14874
 winmail/ComApi.py,sha256=iM-BVISuzKTrixfODdpZNT-itKLfJTMZwoagv7aE8tE,4032
 winmail/OpenApi.py,sha256=MWUFuTKZKa1dj90r-0COoe2z3FHBce7jH0MDtMUmz9U,7006
-winmail/Winmail.py,sha256=DcwqB-E54JPYdGl1N8aQpR0AJkd2iDAJJR1h0PVpAis,26507
+winmail/Winmail.py,sha256=f51QL0nhl9xTZYQDjH-KpGIpLtd1VOZ9VpqQH4FceZA,26582
 winmail/__init__.py,sha256=5HVsDkDQJns0UXGbCUMGv53fyaJF-C6rN7xBv7p0dzA,335
 winmail/utils/MysqlClass.py,sha256=0gm9GGCU_0c37MdORnogWWsYdsWW5S64yCc_ke5KToU,1983
 winmail/utils/Other.py,sha256=ez0jz3g-HcD5J4wqUlZzwUdMT7wflWR7v9jpmdC9l3s,577
 winmail/utils/PostgreClass.py,sha256=7k4KAg0MdR1QT70iEOnZUzWJ9py2mhemRFPWg2qzgmA,1822
 winmail/utils/SqliteClass.py,sha256=zZrfKSPADHEY_7dazwZNu9XJmN3kgXanPXa06gr7HlQ,1728
 winmail/utils/__init__.py,sha256=fnBThfIuXcBHIkYsicFl2AdvRY_3iCZzqJUMflwXAYA,296
-winmail-0.2.23.dist-info/METADATA,sha256=1sWBLwuekFKrwlalJO0BVGyujA32PREVHa2cDjM7PKc,5619
-winmail-0.2.23.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-winmail-0.2.23.dist-info/top_level.txt,sha256=uTByJGkKn9OyBL5iF3MzuuyHr6ebXz4rO1QB2QtLFBk,8
-winmail-0.2.23.dist-info/RECORD,,
+winmail-0.2.23.5.dist-info/METADATA,sha256=xP1elxW7Agdk94Od1Qe_uidEeqL4ffqWadYBjUjb4aQ,5764
+winmail-0.2.23.5.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+winmail-0.2.23.5.dist-info/top_level.txt,sha256=uTByJGkKn9OyBL5iF3MzuuyHr6ebXz4rO1QB2QtLFBk,8
+winmail-0.2.23.5.dist-info/RECORD,,
```

