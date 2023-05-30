# Comparing `tmp/miniagent-0.0.7-py3-none-any.whl.zip` & `tmp/miniagent-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,23 @@
-Zip file size: 17124 bytes, number of entries: 19
+Zip file size: 18788 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-29 08:47 miniadmin/__init__.py
 -rw-rw-r--  2.0 unx     2440 b- defN 23-Apr-29 08:47 miniadmin/admin.py
--rw-rw-r--  2.0 unx     3177 b- defN 23-May-19 08:01 miniagent/__init__.py
--rw-rw-r--  2.0 unx     1760 b- defN 23-May-19 08:01 miniagent/adapter.py
--rw-rw-r--  2.0 unx     3296 b- defN 23-May-19 08:01 miniagent/app_config.py
--rw-rw-r--  2.0 unx     2018 b- defN 23-May-19 08:01 miniagent/command_reciever.py
--rw-rw-r--  2.0 unx     1718 b- defN 23-May-19 08:01 miniagent/common.py
--rw-rw-r--  2.0 unx      752 b- defN 23-May-19 08:01 miniagent/event_reciever.py
--rw-rw-r--  2.0 unx     3310 b- defN 23-May-19 08:01 miniagent/executer.py
--rw-rw-r--  2.0 unx    11633 b- defN 23-May-19 08:01 miniagent/flask_zipkin.py
--rw-rw-r--  2.0 unx     1076 b- defN 23-May-19 08:01 miniagent/job_reciever.py
--rw-rw-r--  2.0 unx     3449 b- defN 23-May-19 08:01 miniagent/message_reciever.py
--rw-rw-r--  2.0 unx      275 b- defN 23-May-19 08:01 miniagent/models.py
--rw-rw-r--  2.0 unx     1063 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4395 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       71 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       20 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1527 b- defN 23-May-19 08:03 miniagent-0.0.7.dist-info/RECORD
-19 files, 42072 bytes uncompressed, 14642 bytes compressed:  65.2%
+-rw-rw-r--  2.0 unx     3307 b- defN 23-May-30 06:45 miniagent/__init__.py
+-rw-rw-r--  2.0 unx     1769 b- defN 23-May-30 06:45 miniagent/adapter.py
+-rw-rw-r--  2.0 unx     3296 b- defN 23-May-30 06:45 miniagent/app_config.py
+-rw-rw-r--  2.0 unx     2296 b- defN 23-May-30 06:45 miniagent/command_reciever.py
+-rw-rw-r--  2.0 unx     1970 b- defN 23-May-30 06:45 miniagent/common.py
+-rw-rw-r--  2.0 unx      752 b- defN 23-May-30 06:45 miniagent/event_reciever.py
+-rw-rw-r--  2.0 unx     1455 b- defN 23-May-30 06:45 miniagent/event_sender.py
+-rw-rw-r--  2.0 unx     4054 b- defN 23-May-30 06:45 miniagent/executer.py
+-rw-rw-r--  2.0 unx    11638 b- defN 23-May-30 06:45 miniagent/flask_zipkin.py
+-rw-rw-r--  2.0 unx     1077 b- defN 23-May-30 06:45 miniagent/job_reciever.py
+-rw-rw-r--  2.0 unx     3450 b- defN 23-May-30 06:45 miniagent/message_reciever.py
+-rw-rw-r--  2.0 unx     1267 b- defN 23-May-30 06:45 miniagent/message_sender.py
+-rw-rw-r--  2.0 unx      275 b- defN 23-May-30 06:45 miniagent/models.py
+-rw-rw-r--  2.0 unx     1063 b- defN 23-May-30 06:49 miniagent-0.0.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4395 b- defN 23-May-30 06:49 miniagent-0.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-30 06:49 miniagent-0.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       71 b- defN 23-May-30 06:49 miniagent-0.0.8.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       20 b- defN 23-May-30 06:49 miniagent-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1693 b- defN 23-May-30 06:49 miniagent-0.0.8.dist-info/RECORD
+21 files, 46380 bytes uncompressed, 16050 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -18,41 +18,47 @@
 
 Filename: miniagent/common.py
 Comment: 
 
 Filename: miniagent/event_reciever.py
 Comment: 
 
+Filename: miniagent/event_sender.py
+Comment: 
+
 Filename: miniagent/executer.py
 Comment: 
 
 Filename: miniagent/flask_zipkin.py
 Comment: 
 
 Filename: miniagent/job_reciever.py
 Comment: 
 
 Filename: miniagent/message_reciever.py
 Comment: 
 
+Filename: miniagent/message_sender.py
+Comment: 
+
 Filename: miniagent/models.py
 Comment: 
 
-Filename: miniagent-0.0.7.dist-info/LICENSE
+Filename: miniagent-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: miniagent-0.0.7.dist-info/METADATA
+Filename: miniagent-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: miniagent-0.0.7.dist-info/WHEEL
+Filename: miniagent-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: miniagent-0.0.7.dist-info/entry_points.txt
+Filename: miniagent-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: miniagent-0.0.7.dist-info/top_level.txt
+Filename: miniagent-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: miniagent-0.0.7.dist-info/RECORD
+Filename: miniagent-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## miniagent/__init__.py

```diff
@@ -5,24 +5,24 @@
 from time import sleep
 from importlib import import_module
 from flask import Flask
 from flask_cors import CORS
 from flask_restful import Api
 from flask_apscheduler import APScheduler
 from flask_sqlalchemy import SQLAlchemy
-import logging
-import logging.handlers
+#import logging
+#import logging.handlers
 from .app_config import AppConfig
 from .executer import ExecuterCaller
 from .command_reciever import CommandsReciever
 from .event_reciever import Command
 from .message_reciever import MessageReciever
 from .flask_zipkin import Zipkin
 
-__version__ = '0.0.7'
+__version__ = '0.0.8'
 
 #Load configuration
 configure = AppConfig(os.getcwd())
 configure.from_pyfile('config.py')
 
 #Set logging
 """
@@ -54,23 +54,25 @@
     zipkin = Zipkin(app, sample_rate=100)
     app.config['ZIPKIN_ADDRESS']=configure['ZIPKIN_ADDRESS']
 
 #REST API
 api = Api(app, prefix="/api/v1")
 api.add_resource(Command, '/command')
 
+if configure.get('CUSTOM_APIS_PATH'):
+    import_module(configure['CUSTOM_APIS_PATH'])
+
 #local database
 if not configure.get('SQLALCHEMY_DATABASE_URI'):
     base_dir = os.path.abspath(os.path.dirname(__file__))
     configure['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///' + os.path.join(base_dir, 'app.db')
 
 app.config ['SQLALCHEMY_DATABASE_URI'] = configure['SQLALCHEMY_DATABASE_URI']
 
 db = SQLAlchemy(app)
-
 #Job Scheduler
 scheduler = APScheduler()
 scheduler.init_app(app)
 scheduler.start()
 
 #Executer
 executer = ExecuterCaller.instance(configure)
@@ -89,15 +91,17 @@
 
 #Command Reciever (Web url polling)
 command_reciever = None
 if configure.get('COMMANDER_SERVER_URL'):
     command_reciever = CommandsReciever(configure['COMMANDER_SERVER_URL'], stop_event)
 
 #Table creation
+# 1. miniagent tables
 from . import models
+# 2. custom tables
 if configure.get('CUSTOM_MODELS_PATH'):
     mdl = import_module(configure['CUSTOM_MODELS_PATH'])
     cls_objs = [x for x in mdl.__dict__ if not x.startswith("_")]
     globals().update({k: getattr(mdl, k) for k in cls_objs})
 
 with app.app_context():
     db.create_all()
```

## miniagent/adapter.py

```diff
@@ -1,18 +1,18 @@
 import abc
 from importlib import import_module
 from datetime import datetime
-from .common import split_class_path, get_class_object
+from .common import split_class_path, get_callable_object
 
 class AdapterFactory:
 
     @staticmethod
     def create_adapter(class_path: str):
 
-        class_obj = get_class_object(class_path)
+        class_obj = get_callable_object(class_path)
 
         if not issubclass(class_obj, Adapter):
             raise RuntimeError("Class [{}] must be a subclass of"
                                " miniagent.adapter.Adapter"\
                             .format(class_obj.__name__))
 
         class_instance = class_obj()
@@ -50,15 +50,15 @@
     def _create_adaptee(self, class_path: str):
 
         if not class_path:
             self.adaptee_name = ""
             self._adaptee = None
             return 1, "No Adaptee"
         
-        class_obj = get_class_object(class_path)
+        class_obj = get_callable_object(class_path)
 
         self._adaptee = class_obj()
         self.adaptee_name = class_path
 
         return 1, "OK"
 
     @abc.abstractmethod
```

## miniagent/command_reciever.py

```diff
@@ -1,14 +1,15 @@
 import json
 import requests
 import threading
 from time import sleep
 from polling2 import *
 from .executer import ExecuterCaller
-        
+from .common import get_callable_object
+
 class CommandsReciever:
 
     def __init__(self, url: str, event: threading.Event) -> None:
         self.event = event
         self._start_polling(url)
 
     def get_thread(self):
@@ -33,29 +34,34 @@
                 sleep(10)
                 continue
 
             
             print('result : ',type(result.text), result.text)
             result_dict = json.loads(result.text)
 
-            from . import app, zipkin
+            from . import app, zipkin, configure
             with app.app_context():
 
                 if zipkin:
 
                     header = result.headers
                     trace_id = header.get('x-b3-traceid')
                     parent_span_id = header.get('x-b3-spanid')
 
-                    zipkin.create_span('CommandsReciever.url='+ url,
+                    zipkin.create_span('command_reciever.url='+ url,
                                         trace_id = trace_id,
                                         parent_span_id = parent_span_id,
                                       )
-                    
-                rtn, comment = ExecuterCaller.instance().execute_command(result_dict)
+
+                callback = None
+                if configure.get('COMMANDER_MESSAGE_CONVERTER'):
+                    function_path = configure.get('COMMANDER_MESSAGE_CONVERTER')
+                    callback = get_callable_object(function_path)
+
+                rtn, comment = ExecuterCaller.instance().execute_command(result_dict, callback)
 
                 if zipkin:
                     zipkin.update_tags(
                         param  = result_dict,
                         result = comment,
                         )
```

## miniagent/common.py

```diff
@@ -1,11 +1,22 @@
 import json
 import sys
 import os
 from importlib import import_module
+from typing import Any
+
+def is_valid_return(rtn:Any)-> bool:
+    
+    if isinstance(rtn, tuple) \
+        and len(rtn)==2 \
+        and isinstance(rtn[0], int) \
+        and isinstance(rtn[1], dict):
+       return True
+    else:
+       return False
 
 def split_class_path(class_path: str) -> tuple[str, str]:
 
     package_name = '.'.join(class_path.split('.')[:-1])
     class_name = class_path.split('.')[-1]
 
     return package_name, class_name
@@ -18,15 +29,15 @@
     except FileNotFoundError as e:
         return -1, dict(error="JsonFile is not found : {}".format(jsonFile))
     except json.decoder.JSONDecodeError as e:
         return -2, dict(error="JSONDecodeError occured : {}".format(sys.exc_info()[1]))
     
     return 1, data
 
-def get_class_object(class_path: str) -> object:
+def get_callable_object(class_path: str) -> object:
         
     package_name, class_name = split_class_path(class_path)
 
     if package_name is None:
         raise RuntimeError("There is no package name in [{}].",format(class_path))
 
     try:
```

## miniagent/executer.py

```diff
@@ -1,14 +1,15 @@
 import sys
 import inspect
 import types
 import abc
+from typing import Callable
 from importlib import import_module
 from typing import TypeVar
-from .common import SingletonInstane, get_class_object
+from .common import SingletonInstane, get_callable_object, is_valid_return
 from .adapter import AdapterFactory
 
 class ExecuterInterface(metaclass=abc.ABCMeta):
 
     @classmethod
     def __subclasshook__(cls, subclass):
         return (hasattr(subclass, 'execute_command') and 
@@ -25,15 +26,15 @@
         raise NotImplementedError
 
 class ExecuterFactory:
 
     @staticmethod
     def create_executer(class_path: str):
 
-        class_obj = get_class_object(class_path)
+        class_obj = get_callable_object(class_path)
 
         if not issubclass(class_obj, ExecuterInterface):
             raise RuntimeError("Class [{}] must be a subclass of"
                                " miniagent.executer.ExecuterInterface"\
                             .format(class_obj.__name__))
 
         return class_obj()
@@ -52,27 +53,37 @@
         rtn, msg = padapter.set_adaptee(adaptee_name)
 
         if not rtn:
             return None
         else:    
             return padapter
 
-    def execute_command(self, message: dict) -> dict:
+    def execute_command(self, message: dict, message_converter: Callable[[dict], dict]=None) -> dict:
         """
         sample message :
         {
             "initial_param":{
                 "product_code":"00011",
                 "payment_amount":50000,
             },
             "executer":"addin.executer.purchase_card.PurchaseCard",
         }
         """
-        initial_params = message['initial_param'] if message.get('initial_param') else {}
-        executer_path = message['executer']
+        if message_converter==None:
+            initial_params = message['initial_param'] if message.get('initial_param') else {}
+            
+            if not message.get('executer'):
+                raise RuntimeError("message must contain 'executer' item, which is not exists."
+                               " message : [{}]"\
+                            .format(str(message)))
+
+            executer_path = message['executer']
+
+        else:
+            initial_params, executer_path = message_converter(message)
 
         executer = ExecuterFactory.create_executer(executer_path)
 
         sig = inspect.signature(executer.execute_command)
 
         adapters = dict()
 
@@ -89,10 +100,15 @@
                 adapter_instance = self._create_adapter(dadapter, dadaptee)
                 adapters[param.name] = adapter_instance
 
         #from . import app
 
         #with app.app_context():
         #    rtn, message = executer.execute_command(initial_params, **adapters)
-        rtn, message = executer.execute_command(initial_params, **adapters)
+        rtn = executer.execute_command(initial_params, **adapters)
+
+        if not is_valid_return(rtn):
+            raise RuntimeError("Return value of execute_command method must be tuple[int, dict].\n"
+                               " class : [{}] , return value : [{}]"\
+                        .format(executer_path, str(rtn)))            
 
-        return rtn, message
+        return rtn
```

## miniagent/flask_zipkin.py

```diff
@@ -211,15 +211,15 @@
             parent_span_id=parent_span_id,
             flags=flags,
             is_sampled=is_sampled,
         )
 
         span = hennry_zipkin_span(
             service_name=self.app.name,
-            span_name='{0}.{1}'.format(request.endpoint, request.method),
+            span_name='rest.{0}.{1}'.format(request.endpoint, request.method),
             transport_handler=self._transport_handler,
             sample_rate=self._sample_rate,
             zipkin_attrs=self._zipkin_attrs
         )
         g._zipkin_span = span
         g._zipkin_span.start()
```

## miniagent/job_reciever.py

```diff
@@ -23,15 +23,15 @@
     
     def _call_execute_command(self, id: str, message: dict):
 
         from . import app, zipkin
         with app.app_context():
 
             if zipkin:
-                zipkin.create_span('ScheduledJob.'+ id)
+                zipkin.create_span('scheduled_job.'+ id)
                 zipkin.update_tags(param=message)
 
             rtn, comment = self.caller.execute_command(message)
 
             if zipkin:
                 zipkin.update_tags(
                     param  = message,
```

## miniagent/message_reciever.py

```diff
@@ -61,15 +61,15 @@
 
                         if zipkin:
 
                             header = result_dict['header']
                             trace_id = header.get('trace_id')
                             parent_span_id = header.get('span_id')
 
-                            zipkin.create_span('KafkaConsumer.topic='+ topic_partition.topic,
+                            zipkin.create_span('Kafka_consumer.topic='+ topic_partition.topic,
                                                trace_id = trace_id,
                                                parent_span_id = parent_span_id,
                                                )
                             zipkin.update_tags(param=message.value)
 
                         rtn, comment = ExecuterCaller.instance().execute_command(result_dict)
```

## Comparing `miniagent-0.0.7.dist-info/LICENSE` & `miniagent-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `miniagent-0.0.7.dist-info/METADATA` & `miniagent-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniagent
-Version: 0.0.7
+Version: 0.0.8
 Summary: Multi-adaptable and lightweight server framework based on Flask
 Home-page: https://github.com/tanminkwan/local-agent
 Author: tanminkwan
 Author-email: tanminkwan@gmail.com
 License: MIT
 Keywords: flask,sqlalchemy,scheduler,zipkin,kafka
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `miniagent-0.0.7.dist-info/RECORD` & `miniagent-0.0.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 miniadmin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 miniadmin/admin.py,sha256=MejGCYRC8vHuGFRQ5xaZaVBEpio1FCaFl6xNtSkyD-k,2440
-miniagent/__init__.py,sha256=2k_sCauZy61c-tO3Ed242MUd3Vo1gDwUjnX1uG7R2UE,3177
-miniagent/adapter.py,sha256=rAGgRrwuSKqfkAsmnM7v2yEqQ6EAQFIAjDQkova_W6c,1760
+miniagent/__init__.py,sha256=PLO-02uKVD90RMKIpWP1X3ybPi-mTYr81TFXs8p3tBc,3307
+miniagent/adapter.py,sha256=sIL0d6jLOwterm9ve4zS4BULE3l3_sC9ZlWo5lM69hE,1769
 miniagent/app_config.py,sha256=B-K-5ebnUIekZlrDoLdVttGzewTNjCpu6DDVmKqPB2M,3296
-miniagent/command_reciever.py,sha256=zxM1OlJ2EWAF3C7OssBlMsErybDdUkoOzz5j1HKVf4Q,2018
-miniagent/common.py,sha256=JqvF73z43erW1DR9RQ2Cy0-zCYcsnsW6vX8F9kLCmcA,1718
+miniagent/command_reciever.py,sha256=LXSG-ePf6zAlpPtQ4O_NPsr6vqBPOxKobxgkwJ6C648,2296
+miniagent/common.py,sha256=L3mOezGksJWsx07cLP3TlBzMe0PSAZ54jqZhk-DpFjk,1970
 miniagent/event_reciever.py,sha256=utVPqGFQAiUJXq6N2n93jcGib_8A5cjwMRNWl3OOm9g,752
-miniagent/executer.py,sha256=75WSHJhS62hjRF1yKQ8O4ZNgXh8noI2fYgMGo3H4RTM,3310
-miniagent/flask_zipkin.py,sha256=05-NnH6-Mif9rw-HSx1eUEGqoY_mTcXDICqQ8IvasRY,11633
-miniagent/job_reciever.py,sha256=xTrgUhL8hSkl4n5KOYyB28aeBTWqQkAluzneKpiRDaM,1076
-miniagent/message_reciever.py,sha256=0yU6qRqCKyMfveJjT3dmXgpiYw0nUDk-wB33z0egJls,3449
+miniagent/event_sender.py,sha256=Tav6jOUUUT_eQGo-me1NkuSLdXha32Wlr9lLH6cWg0U,1455
+miniagent/executer.py,sha256=1C4cC3ffRxyMSiIrF18KGY0ofgvVjpXijCsaY4IfW40,4054
+miniagent/flask_zipkin.py,sha256=tGLTf79rZGEn71fVI2q7eI9UIotcT_c9jXQGolnB5p4,11638
+miniagent/job_reciever.py,sha256=jPXAMj3Ri8_56-e-a29SxLMDtRaajO3rZLK2W0xdUlM,1077
+miniagent/message_reciever.py,sha256=nrP1wmNc_VaMifac1FfDtdIqqMKmDgkxn2vKAYp1Vgo,3450
+miniagent/message_sender.py,sha256=-V2iLL8c3X5r-iv9KH91cxRF39xDXIGR7DCyl769SFg,1267
 miniagent/models.py,sha256=oEWOA0awWmcjo_nm0IVwoY9_FTkssLG6pX-oLYvFnTo,275
-miniagent-0.0.7.dist-info/LICENSE,sha256=nj6HxIMEUT6XKDHjyJYPnIS37d5NKErlNwbV0XbxcsQ,1063
-miniagent-0.0.7.dist-info/METADATA,sha256=5a4Rf6ieGLGYhGDsmi795XfM2IZfvflAUstFcuAh5J4,4395
-miniagent-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-miniagent-0.0.7.dist-info/entry_points.txt,sha256=v6HAev-cy1ey5C3hnCdS589pljKD1wOW6zURhAq5P6Q,71
-miniagent-0.0.7.dist-info/top_level.txt,sha256=AMyT-pye0DyB9Q8Ow_lGVtXb3COCxNZoS0yIdptLgzU,20
-miniagent-0.0.7.dist-info/RECORD,,
+miniagent-0.0.8.dist-info/LICENSE,sha256=nj6HxIMEUT6XKDHjyJYPnIS37d5NKErlNwbV0XbxcsQ,1063
+miniagent-0.0.8.dist-info/METADATA,sha256=QGs8pjhe2K93kqx6vZCTkTcfSjBj4nG9e83GzIAx4Zc,4395
+miniagent-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+miniagent-0.0.8.dist-info/entry_points.txt,sha256=v6HAev-cy1ey5C3hnCdS589pljKD1wOW6zURhAq5P6Q,71
+miniagent-0.0.8.dist-info/top_level.txt,sha256=AMyT-pye0DyB9Q8Ow_lGVtXb3COCxNZoS0yIdptLgzU,20
+miniagent-0.0.8.dist-info/RECORD,,
```

