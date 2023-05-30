# Comparing `tmp/PyDust-0.0.8.tar.gz` & `tmp/PyDust-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDust-0.0.8.tar", last modified: Fri May  6 09:50:52 2022, max compression
+gzip compressed data, was "PyDust-0.0.9.tar", last modified: Fri May 13 12:52:31 2022, max compression
```

## Comparing `PyDust-0.0.8.tar` & `PyDust-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zsolthorvath   (501) staff       (20)        0 2022-05-06 09:50:52.544855 PyDust-0.0.8/
--rw-r--r--   0 zsolthorvath   (501) staff       (20)    11357 2022-03-23 10:58:58.000000 PyDust-0.0.8/LICENSE
--rw-r--r--   0 zsolthorvath   (501) staff       (20)      475 2022-05-06 09:50:52.544276 PyDust-0.0.8/PKG-INFO
-drwxr-xr-x   0 zsolthorvath   (501) staff       (20)        0 2022-05-06 09:50:52.529887 PyDust-0.0.8/PyDust.egg-info/
--rw-r--r--   0 zsolthorvath   (501) staff       (20)      475 2022-05-06 09:50:52.000000 PyDust-0.0.8/PyDust.egg-info/PKG-INFO
--rw-r--r--   0 zsolthorvath   (501) staff       (20)      382 2022-05-06 09:50:52.000000 PyDust-0.0.8/PyDust.egg-info/SOURCES.txt
--rw-r--r--   0 zsolthorvath   (501) staff       (20)        1 2022-05-06 09:50:52.000000 PyDust-0.0.8/PyDust.egg-info/dependency_links.txt
--rw-r--r--   0 zsolthorvath   (501) staff       (20)       67 2022-05-06 09:50:52.000000 PyDust-0.0.8/PyDust.egg-info/requires.txt
--rw-r--r--   0 zsolthorvath   (501) staff       (20)        5 2022-05-06 09:50:52.000000 PyDust-0.0.8/PyDust.egg-info/top_level.txt
--rw-r--r--   0 zsolthorvath   (501) staff       (20)        5 2022-03-23 11:07:36.000000 PyDust-0.0.8/README.md
-drwxr-xr-x   0 zsolthorvath   (501) staff       (20)        0 2022-05-06 09:50:52.537562 PyDust-0.0.8/dust/
--rw-r--r--   0 zsolthorvath   (501) staff       (20)     1078 2022-03-25 10:51:15.000000 PyDust-0.0.8/dust/__init__.py
--rw-r--r--   0 zsolthorvath   (501) staff       (20)    25621 2022-05-04 11:19:32.000000 PyDust-0.0.8/dust/entity.py
--rw-r--r--   0 zsolthorvath   (501) staff       (20)     2882 2022-05-05 15:53:13.000000 PyDust-0.0.8/dust/events.py
--rw-r--r--   0 zsolthorvath   (501) staff       (20)    16075 2022-05-03 14:48:19.000000 PyDust-0.0.8/dust/messages.py
-drwxr-xr-x   0 zsolthorvath   (501) staff       (20)        0 2022-05-06 09:50:52.542719 PyDust-0.0.8/dust/persist/
--rw-r--r--   0 zsolthorvath   (501) staff       (20)       40 2022-05-05 14:50:01.000000 PyDust-0.0.8/dust/persist/__init__.py
--rw-r--r--   0 zsolthorvath   (501) staff       (20)     5410 2022-05-05 16:05:38.000000 PyDust-0.0.8/dust/persist/mysqlpersist.py
--rw-r--r--   0 zsolthorvath   (501) staff       (20)     4408 2022-05-06 09:38:14.000000 PyDust-0.0.8/dust/persist/sqlitepersist.py
--rw-r--r--   0 zsolthorvath   (501) staff       (20)    14372 2022-05-06 09:27:28.000000 PyDust-0.0.8/dust/persist/sqlpersist.py
--rw-r--r--   0 zsolthorvath   (501) staff       (20)     4994 2022-05-03 14:48:32.000000 PyDust-0.0.8/dust/slack.py
--rw-r--r--   0 zsolthorvath   (501) staff       (20)     1073 2022-05-04 11:23:06.000000 PyDust-0.0.8/dust/templates.py
--rw-r--r--   0 zsolthorvath   (501) staff       (20)       38 2022-05-06 09:50:52.545026 PyDust-0.0.8/setup.cfg
--rw-r--r--   0 zsolthorvath   (501) staff       (20)     1562 2022-05-06 09:42:44.000000 PyDust-0.0.8/setup.py
+drwxr-xr-x   0 zsolthorvath   (501) staff       (20)        0 2022-05-13 12:52:31.064390 PyDust-0.0.9/
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)    11357 2022-03-23 10:58:58.000000 PyDust-0.0.9/LICENSE
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)      444 2022-05-13 12:52:31.064054 PyDust-0.0.9/PKG-INFO
+drwxr-xr-x   0 zsolthorvath   (501) staff       (20)        0 2022-05-13 12:52:31.056797 PyDust-0.0.9/PyDust.egg-info/
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)      444 2022-05-13 12:52:30.000000 PyDust-0.0.9/PyDust.egg-info/PKG-INFO
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)      382 2022-05-13 12:52:30.000000 PyDust-0.0.9/PyDust.egg-info/SOURCES.txt
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)        1 2022-05-13 12:52:30.000000 PyDust-0.0.9/PyDust.egg-info/dependency_links.txt
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)       67 2022-05-13 12:52:30.000000 PyDust-0.0.9/PyDust.egg-info/requires.txt
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)        5 2022-05-13 12:52:30.000000 PyDust-0.0.9/PyDust.egg-info/top_level.txt
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)        5 2022-03-23 11:07:36.000000 PyDust-0.0.9/README.md
+drwxr-xr-x   0 zsolthorvath   (501) staff       (20)        0 2022-05-13 12:52:31.060473 PyDust-0.0.9/dust/
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)     1164 2022-05-11 12:36:11.000000 PyDust-0.0.9/dust/__init__.py
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)    27474 2022-05-12 14:40:12.000000 PyDust-0.0.9/dust/entity.py
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)     2882 2022-05-05 15:53:13.000000 PyDust-0.0.9/dust/events.py
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)    16075 2022-05-03 14:48:19.000000 PyDust-0.0.9/dust/messages.py
+drwxr-xr-x   0 zsolthorvath   (501) staff       (20)        0 2022-05-13 12:52:31.063053 PyDust-0.0.9/dust/persist/
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)       40 2022-05-05 14:50:01.000000 PyDust-0.0.9/dust/persist/__init__.py
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)     5889 2022-05-11 13:54:23.000000 PyDust-0.0.9/dust/persist/mysqlpersist.py
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)     4838 2022-05-11 13:54:30.000000 PyDust-0.0.9/dust/persist/sqlitepersist.py
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)    16664 2022-05-11 13:51:08.000000 PyDust-0.0.9/dust/persist/sqlpersist.py
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)     4994 2022-05-03 14:48:32.000000 PyDust-0.0.9/dust/slack.py
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)     1073 2022-05-04 11:23:06.000000 PyDust-0.0.9/dust/templates.py
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)       38 2022-05-13 12:52:31.064522 PyDust-0.0.9/setup.cfg
+-rw-r--r--   0 zsolthorvath   (501) staff       (20)     1531 2022-05-13 12:52:02.000000 PyDust-0.0.9/setup.py
```

### Comparing `PyDust-0.0.8/LICENSE` & `PyDust-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDust-0.0.8/dust/__init__.py` & `PyDust-0.0.9/dust/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,14 +28,20 @@
     ADD = 1
     GET = 2
     PEEK = 3
     VISIT = 4
     CHANGE = 5
     DEL = 6
 
+class Committed(Enum):
+    CREATED = 0
+    UPDATED = 1
+    DELETED = 2
+    SAVED = 3
+
 class MetaProps(Enum):
     @property
     def datatype(self):
         return self.value[0]
 
     @property
     def valuetype(self):
```

### Comparing `PyDust-0.0.8/dust/entity.py` & `PyDust-0.0.9/dust/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import yaml
 import traceback
 import inspect
 from enum import Enum
 from collections import namedtuple
 from datetime import datetime
-from dust import Datatypes, ValueTypes, Operation, MetaProps, FieldProps
+from dust import Datatypes, ValueTypes, Operation, MetaProps, FieldProps, Committed
 from importlib import import_module
 
 import threading
 
 _messages_create_message = None
 _store_lock = threading.RLock()
 
@@ -33,15 +33,15 @@
     global_name = (Datatypes.STRING, ValueTypes.SINGLE, 2, 301)
     field_order = (Datatypes.INT, ValueTypes.SINGLE, 3, 302)
 
 class EntityBaseMeta(MetaProps):
     unit = (Datatypes.ENTITY, ValueTypes.SINGLE, 1, 400)
     meta_type = (Datatypes.ENTITY, ValueTypes.SINGLE, 2, 401)
     entity_id = (Datatypes.INT, ValueTypes.SINGLE, 3, 402)
-    committed = (Datatypes.BOOL, ValueTypes.SINGLE, 4 ,403)
+    committed = (Datatypes.STRING, ValueTypes.SINGLE, 4 ,403)
 
 class EntityTypes(FieldProps):
     type_meta = (UNIT_ENTITY_META, TypeMeta, 1)
     _entity_base = (UNIT_ENTITY_META, EntityBaseMeta, 2)
     unit = (UNIT_ENTITY_META, UnitMeta, 3)
     meta_field = (UNIT_ENTITY_META, MetaField, 4)
 
@@ -150,15 +150,15 @@
 
         unit_field, meta_type_field, entity_id_field, committed_field = Store._get_base_fields()
 
         entity_map[e.global_id()] = ({
             unit_field: e.unit.global_id(), 
             entity_id_field: e.entity_id, 
             meta_type_field: e.meta_type.global_id(),
-            committed_field: e.committed
+            committed_field: e.committed.name
         }, e)
 
 
     @staticmethod
     def increment_unit_counter(unit, requested_id):
         if isinstance(unit, str):
             unit = globals()["_enum_map"][unit]
@@ -358,17 +358,19 @@
                 e_map[global_field_name] = set()
             elif field_config["valuetype"] == ValueTypes.LIST:
                 e_map[global_field_name] = []
                 return e_map[global_name]
 
     @staticmethod
     def _set_uncommitted(e, e_map):
-        e.committed = False
+        if e.committed == Committed.SAVED:
+            e.committed = Committed.UPDATED
+
         committed_field = Store._get_base_fields()[3]
-        e_map[committed_field] = False
+        e_map[committed_field] = e.committed.name
 
         return True
 
     @staticmethod
     def _access_data_set_value(obj, field, value, operation):
         if isinstance(obj, Entity):
             changed = False
@@ -489,21 +491,56 @@
     def from_json(objects):
         entities = []
         for e_map in objects:
             entities.append(Entity.from_json(e_map))
 
         return entities
 
+    @staticmethod
+    def get_meta_type_enum(entity):
+        enum_map = globals()["_enum_map"]
+        if isinstance(entity, Entity):
+            return enum_map[entity.meta_type]
+        elif isinstance(entity, dict):
+            _, meta_type_field, _,  _ = Store._get_base_fields()
+            return enum_map[entity[meta_type_field]]
+
+    @staticmethod
+    def get_global_fieldname(field):
+        enum_map = globals()["_enum_map"]
+        return enum_map[field]
+
+    @staticmethod
+    def global_id(entity):
+        if isinstance(entity, Entity):
+            return entity.global_id()
+        elif isinstance(entity, dict):
+            unit_field, meta_type_field, entity_id_field,  _ = Store._get_base_fields()
+            unit = Store.access(Operation.GET, None, entity[unit_field])
+            meta_type = Store.access(Operation.GET, None, entity[meta_type_field])
+            return Entity._ref(unit, entity[entity_id_field], meta_type)
+
+    @staticmethod
+    def concat_field_values(entity, fields, separator="#"):
+        values = []
+        template = separator.join(["{}" for i in range(len(fields))])
+        for field in fields:
+            if isinstance(entity, Entity):
+                values.append(entity.access(Operation.GET, None, field))
+            elif isinstance(entity, dict):
+                values.append(entity.get(Store.get_global_fieldname(field)))
+
+        return template.format(*values)
 
 class Entity():
     def __init__(self, unit, entity_id, meta_type):
         self.unit = unit
         self.entity_id = entity_id
         self.meta_type = meta_type
-        self.committed = False
+        self.committed = Committed.CREATED
 
     def access(self, operation, value, *path):
         enum_map = globals()["_enum_map"]
         return Store.access(operation, value, enum_map[self.unit], self.entity_id, enum_map[self.meta_type], *path)
 
     @staticmethod
     def _ref(unit, entity_id, meta_type):
@@ -525,15 +562,15 @@
                 entity_id = int(parts[1])
             except:
                 pass
             if len(parts) == 3 and not entity_id is None:
                 entity = globals()["_entity_map"].get(value, (None, None))[1]
                 unit = enum_map.get(parts[0], None)
                 if unit and isinstance(unit, Entity) and enum_map[unit.meta_type] == EntityTypes.unit:
-                    if entity.meta_type and isinstance(entity.meta_type, Entity) and entity.meta_type in enum_map:
+                    if entity and entity.meta_type and isinstance(entity.meta_type, Entity) and entity.meta_type in enum_map:
                         return (unit, entity_id, entity.meta_type)
 
         return (None, None, None)
 
     def get_meta_type_enum(self):
         enum_map = globals()["_enum_map"]
         return _enum_map[self.meta_type]
@@ -556,43 +593,51 @@
     def to_json(self):
         json_map = {}
         self.__to_json(json_map)
         return json_map
 
     def set_committed(self):
         entity_map = globals()["_entity_map"]
-        self.committed = True
+        self.committed = Committed.SAVED
 
         _, _, _, committed_field = Store._get_base_fields()
 
-        entity_map[self.global_id()][0][committed_field] = True
+        entity_map[self.global_id()][0][committed_field] = self.committed.name
 
     @staticmethod
-    def from_json(e_map):
+    def from_json(e_map, force_new_id=False):
         entity_map = globals()["_entity_map"]
         enum_map = globals()["_enum_map"]
 
-        unit_field, meta_type_field, entity_id_field, _ = Store._get_base_fields()
+        unit_field, meta_type_field, entity_id_field, committed_field = Store._get_base_fields()
 
         unit_parts = e_map[unit_field].split(":")
 
+        if force_new_id:
+            entity_id = None
+        else:
+            entity_id = int(e_map[entity_id_field])
+
         unit = Store.access(Operation.GET, None, UNIT_ENTITY, int(unit_parts[1]), EntityTypes.unit)
         unit_name = unit.access(Operation.GET, None, UnitMeta.name)
         meta_type = enum_map[e_map[meta_type_field]]
 
-        e = Store.access(Operation.GET, None, unit_name, int(e_map[entity_id_field]), meta_type)
+        e = Store.access(Operation.GET, None, unit_name, entity_id, meta_type)
 
         for field, value in e_map.items():
-            if not field in [unit_field, meta_type_field, entity_id_field]:
+            if not field in [unit_field, meta_type_field, entity_id_field, committed_field]:
                 field_parts = field.split(":")
                 field_config = Store._get_field_config(field_parts[0], field_parts[1], field_parts[2])
                 if field_config["valuetype"] == ValueTypes.SET and isinstance(value, list):
                     e.access(Operation.SET, set(value), field_config["_enum"])
                 else:
                     e.access(Operation.SET, value, field_config["_enum"])
+            elif field == committed_field:
+                if Committed[value] == Committed.SAVED:
+                    self.set_committed()
         return e
 
 _entity_map = {}
 _enum_map = {}
 
 Store.load_types_from_enum(EntityTypes, UNIT_META_ID)
 _messages_module = import_module("dust.messages")
```

### Comparing `PyDust-0.0.8/dust/events.py` & `PyDust-0.0.9/dust/events.py`

 * *Files identical despite different names*

### Comparing `PyDust-0.0.8/dust/messages.py` & `PyDust-0.0.9/dust/messages.py`

 * *Files identical despite different names*

### Comparing `PyDust-0.0.8/dust/persist/mysqlpersist.py` & `PyDust-0.0.9/dust/persist/mysqlpersist.py`

 * *Files 18% similar despite different names*

```diff
@@ -58,14 +58,23 @@
 WHERE \
 {% for filter in filters %}\
 {{ filter[0] }} {{ filter[1] }} %({{ filter[0] }})s {% if not loop.last %}AND {% endif %}\
 {% endfor %}\
 {% endif %}\
 "
 
+UPDATE_TEMPLATE = "\
+UPDATE {{sql_table.table_name}} SET \
+{% for field in sql_table.fields %}\
+{% if not field.primary_key and not field.base_field %}{{ field.field_name }} = %({{ field.field_name }})s{% if not loop.last %},{% endif %}{% endif %} \
+{% endfor %}\
+WHERE \
+{% for field in sql_table.primary_keys %}{{ field.field_name }} = %({{ field.field_name }})s{% if not loop.last %},{% endif %}{% endfor %} \
+"
+
 MYSQL_USER = os.environ.get('MYSQL_USER')
 MYSQL_PASSWORD = os.environ.get('MYSQL_PASSWORD')
 MYSQL_HOST = os.environ.get('MYSQL_HOST')
 MYSQL_DB = os.environ.get('MYSQL_DB')
 
 class MySQLPersist(SqlPersist):
     def __init__(self):
@@ -147,14 +156,17 @@
 
     def insert_into_table_template(self):
         return INSERT_INTO_TABLE_TEMPLATE
 
     def select_template(self, filters):
         return SELECT_TEMPLATE
 
+    def update_template(self):
+        return UPDATE_TEMPLATE
+
     def convert_value_to_db(self, field, value):
         if field.datatype == Datatypes.BOOL:
             if value == True:
                 return 1
             else:
                 return 0
         elif field.datatype == Datatypes.ENTITY and isinstance(value, Entity):
```

### Comparing `PyDust-0.0.8/dust/persist/sqlitepersist.py` & `PyDust-0.0.9/dust/persist/sqlitepersist.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,14 +56,24 @@
 WHERE \
 {% for filter in filters %}\
 filter[0] filter[1] ? {% if not loop.last %}AND {% endif %}\
 {% endfor %}\
 {% endif %}\
 "
 
+UPDATE_TEMPLATE = "\
+UPDATE {{sql_table.table_name}} SET \
+{% for field in sql_table.fields %}\
+{% if not field.primary_key and not field.base_field %}{{ field.field_name }} = ?{% if not loop.last %},{% endif %}{% endif %} \
+{% endfor %}\
+WHERE \
+{% for field in sql_table.primary_keys %}{{ field.field_name }} = ?{% if not loop.last %},{% endif %}{% endfor %} \
+"
+
+
 DB_FILE = "dust.db"
 
 class SqlitePersist(SqlPersist):
     def __init__(self):
         super().__init__(**self.__db_api_kwargs())
 
     def __create_connection(self):
@@ -133,14 +143,17 @@
 
     def insert_into_table_template(self):
         return INSERT_INTO_TABLE_TEMPLATE
 
     def select_template(self, filters):
         return SELECT_TEMPLATE
 
+    def update_template(self):
+        return UPDATE_TEMPLATE
+
     def convert_value_to_db(self, field, value):
         if field.datatype == Datatypes.BOOL:
             if value == True:
                 return 1
             else:
                 return 0
         elif field.datatype == Datatypes.ENTITY and isinstance(value, Entity):
```

### Comparing `PyDust-0.0.8/dust/persist/sqlpersist.py` & `PyDust-0.0.9/dust/persist/sqlpersist.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 from jinja2 import Template
 import traceback
 import json
 
-from dust import Datatypes, ValueTypes, Operation, MetaProps, FieldProps
+from dust import Datatypes, ValueTypes, Operation, MetaProps, FieldProps, Committed
 from dust.entity import UNIT_ENTITY, EntityTypes, EntityBaseMeta, Store, UnitMeta
 from dust.events import UNIT_EVENTS, EventTypes
 
 _sql_persister = None
 _types_initiated = set()
 
 def init_sql_persist(unit_name, persist_class, meta_type_enums, deps_func):
@@ -30,32 +30,41 @@
                 for dep_unit_name, dep_meta_type_enums, dep_deps_func in unit_dependencies:
                     init_sql_persist(dep_unit_name, persist_class, dep_meta_type_enums, dep_deps_func)
 
 def load_all():
     global _sql_persister
     return _sql_persister.load_all()    
 
+def load_units():
+    global _sql_persister
+    return _sql_persister.load_units()    
+
+def load_unit_type(unit_meta_type):
+    global _sql_persister
+    return _sql_persister.load_type(unit_meta_type)    
+
 def persist_entities(entities):
     global _sql_persister
     _sql_persister.persist_entities(entities)    
 
 class SqlField():
-    def __init__(self, field_name, field_type, primary_key=False):
+    def __init__(self, field_name, field_type, primary_key=False, base_field=False):
         self.field_name = field_name
         self.field_type = field_type
         self.primary_key = primary_key
+        self.base_field = base_field
 
 class SqlTable():
     def __init__(self, table_name):
         self.table_name = table_name
         self.fields = []
         self.primary_keys = []
 
-    def add_field(self, sql_field, sql_type, primary_key=False):
-        field = SqlField(sql_field, sql_type, primary_key)
+    def add_field(self, sql_field, sql_type, primary_key=False, base_field=False):
+        field = SqlField(sql_field, sql_type, primary_key, base_field)
         self.fields.append(field)
         if primary_key:
             self.primary_keys.append(field)
 
 class SqlPersist():
     def __init__(self, **kwargs):
         for key, value in kwargs.items():
@@ -77,14 +86,17 @@
 
     def insert_into_table_template(self):
         pass
 
     def select_template(self, filters):
         pass
 
+    def update_template(self):
+        pass
+
     def convert_value_to_db(self, field, value):
         pass
 
     def create_cursor(self, conn):
         pass
 
     def close_cursor(self, conn):
@@ -123,16 +135,30 @@
 
             elif field.valuetype == ValueTypes.MAP:
                 return json.loads(value)
 
     def load_all(self):
         entities = []
         for unit_meta in self.__persisted_types:
-            if unit_meta.type_name[0] != "_":
-                entities.extend(self.load_entities(unit_meta, filters=None, conn=None))
+            entities.extend(self.load_type(unit_meta))
+
+        return entities
+
+    def load_units(self):
+        entities = []
+        for unit_meta in EntityTypes:
+            entities.extend(self.load_type(unit_meta))
+
+        return entities
+
+    def load_type(self, unit_meta):
+        entities = []
+
+        if unit_meta.type_name[0] != "_":
+            entities = self.load_entities(unit_meta, filters=None, conn=None)
 
         return entities
 
     def load_entities(self, meta_type, filters=None, conn=None):
         entities = {}
 
         close_connection = ( conn is None )
@@ -165,25 +191,25 @@
                     unit_global_id = row[1]
                     meta_type_global_id = row[2]
                     entity_id = row[3]
                     unit_entity = Store.access(Operation.GET, None, row[1])
                     meta_type_entity = Store.access(Operation.GET, None, row[2])
                     #print("{}:{}:{}".format(unit_entity, row[3], meta_type_entity))
                     entity = Store.access(Operation.GET, None, unit_entity, row[3], meta_type_entity)
-                    entity.set_committed()
 
                     index = 4 # 0 - global_id 1-3: base fields
                     for field in meta_type.fields_enum:
                         if not field.valuetype in [ValueTypes.LIST, ValueTypes.SET]:
                             value = self.map_value_from_db(field, row[index])
                             if not value is None:
                                 entity.access(Operation.SET, value, field)
 
                             index += 1
 
+                    entity.set_committed()
                     entities[row[0]] = entity
             finally:
                 self._close_cursor(c)
 
             # Do multivalue fields
             for field in meta_type.fields_enum:
                 if field.valuetype in [ValueTypes.LIST, ValueTypes.SET]:
@@ -197,14 +223,15 @@
                         c = self._create_cursor(conn)
                         #print("{}".format(multivalue_select_sql))
                         c.execute(multivalue_select_sql)
                         rows = c.fetchall()
                         for row in rows:
                             if row[0] in global_ids:
                                 entities[row[0]].access(Operation.ADD, self.map_value_from_db(field, row[2]), field)
+                                entities[row[0]].set_committed()
 
                     finally:
                         self._close_cursor(c)
         finally:
             if close_connection:
                 self._close_connection(conn)
 
@@ -233,54 +260,90 @@
                 if not field.valuetype in [ValueTypes.LIST, ValueTypes.SET]:
                     self.add_execute_param(values, "_"+field.name, self.map_value_to_db(field, entity))
                 else:
                     multivalue_tablename = "{}_{}".format(sql_tables[0].table_name, field.name)
                     multivalues[multivalue_tablename] = (field.name, self.map_value_to_db(field, entity))
 
             try:
-                return_value = self.__insert_entity_values(insert_sql, values, conn)
+                return_value = self.__update_entity_values(insert_sql, values, conn)
                 if return_value and len(sql_tables) > 1:
                     #print(json.dumps(multivalues, indent=4))
                     for idx, sql_table in enumerate(sql_tables[1:], start=1):
                         if return_value:
                             field_name, multivalues_array = multivalues[sql_table.table_name]
                             if multivalues_array:
                                 insert_sql = self.__render_tempate(self.insert_into_table_template, sql_table=sql_table)
                                 for value_cnt, value in enumerate(multivalues_array):
                                     values = self.create_exectute_params()
                                     self.add_execute_param(values, "_global_id", entity.global_id())
                                     self.add_execute_param(values, "_value_cnt", value_cnt)
                                     self.add_execute_param(values, "_"+field_name+"_value", value)
-                                    return_value = self.__insert_entity_values(insert_sql, values, conn)
+                                    return_value = self.__update_entity_values(insert_sql, values, conn)
+            finally:
+                if close_connection:
+                    self._close_connection(conn)
+
+        if return_value:
+            entity.set_committed()
+
+        return return_value
+
+    def update_entity(self, entity, conn=None):
+        return_value = False
+
+        close_connection = ( conn is None )
+        if conn is None:
+            conn = self._create_connection()
+        meta_type = entity.get_meta_type_enum()
+        if meta_type in self.__persisted_types:
+            sql_tables = self.__sql_tables(self.__table_name(meta_type), meta_type.fields_enum)
+            try:
+                update_sql = self.__render_tempate(self.update_template, sql_table=sql_tables[0])
+                values = self.create_exectute_params()
+                self.add_execute_param(values, "_global_id", entity.global_id())
+                for field in meta_type.fields_enum:
+                    if not field.valuetype in [ValueTypes.LIST, ValueTypes.SET]:
+                        self.add_execute_param(values, "_"+field.name, self.map_value_to_db(field, entity))
+                return_value = self.__update_entity_values(update_sql, values, conn)
+
             finally:
                 if close_connection:
                     self._close_connection(conn)
 
-        return False
+        if return_value:
+            entity.set_committed()
+
+        return return_value
 
-    def __insert_entity_values(self, insert_sql, values, conn):
+    def __update_entity_values(self, update_sql, values, conn):
         return_value = False
 
         try:
             c = self._create_cursor(conn)
-            #print("Inserting {} with {}".format(values, insert_sql))
-            c.execute(insert_sql, values)
+            if update_sql.startswith("UPDATE"):
+                print("Updating {} with {}".format(values, update_sql))
+            c.execute(update_sql, values)
 
             return_value = True
         finally:
             self._close_cursor(c)
 
         return return_value
 
     def persist_entities(self, entities):
         conn = None
         try:
             conn = self._create_connection()
             for e in entities:
-                self.insert_entity(e, conn)
+                if e.committed == Committed.CREATED:
+                    self.insert_entity(e, conn)
+                elif e.committed == Committed.UPDATED:
+                    self.update_entity(e, conn)
+                elif e.committed == Committed.DELETED:
+                    pass
         finally:
             self._close_connection(conn)
 
     def __render_tempate(self, template_func, *args, **kwargs):
         try: 
             template = Template(template_func(*args))
             return template.render(**kwargs)
@@ -290,23 +353,23 @@
     def __table_name(self, unit_meta):
         return "{}_{}".format(self.__unit_meta_unit[unit_meta], unit_meta.type_name)
 
     def __sql_tables(self, table_name, fields_enum):
         sql_tables = []
         sql_table = SqlTable(table_name)
         sql_tables.append(sql_table)
-        sql_table.add_field("_global_id", self.sql_type(Datatypes.STRING, ValueTypes.SINGLE, primary_key=True), primary_key=True)
+        sql_table.add_field("_global_id", self.sql_type(Datatypes.STRING, ValueTypes.SINGLE, primary_key=True), primary_key=True, base_field=True)
         for base_field in EntityTypes._entity_base.fields_enum:
             if base_field != EntityBaseMeta.committed:
-                sql_table.add_field("_"+base_field.name, self.sql_type(base_field.datatype, base_field.valuetype))
+                sql_table.add_field("_"+base_field.name, self.sql_type(base_field.datatype, base_field.valuetype), base_field=True)
         for field in fields_enum:
             if field.valuetype in [ValueTypes.LIST, ValueTypes.SET]:
                 multivalue_sql_table = SqlTable("{}_{}".format(table_name, field.name))
-                multivalue_sql_table.add_field("_global_id", self.sql_type(Datatypes.STRING, ValueTypes.SINGLE, primary_key=True), primary_key=True)
-                multivalue_sql_table.add_field("_value_cnt", self.sql_type(Datatypes.INT, ValueTypes.SINGLE), primary_key=True)
+                multivalue_sql_table.add_field("_global_id", self.sql_type(Datatypes.STRING, ValueTypes.SINGLE, primary_key=True), primary_key=True, base_field=True)
+                multivalue_sql_table.add_field("_value_cnt", self.sql_type(Datatypes.INT, ValueTypes.SINGLE), primary_key=True, base_field=True)
                 multivalue_sql_table.add_field("_"+field.name+"_value", self.sql_type(field.datatype, ValueTypes.SINGLE))
                 sql_tables.append(multivalue_sql_table)
             else:
                 sql_table.add_field("_"+field.name, self.sql_type(field.datatype, field.valuetype))
 
         return sql_tables
```

### Comparing `PyDust-0.0.8/dust/slack.py` & `PyDust-0.0.9/dust/slack.py`

 * *Files identical despite different names*

### Comparing `PyDust-0.0.8/dust/templates.py` & `PyDust-0.0.9/dust/templates.py`

 * *Files identical despite different names*

### Comparing `PyDust-0.0.8/setup.py` & `PyDust-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PyDust",
-    version="0.0.8",
-    description="Read the latest Real Python tutorials",
+    version="0.0.9",
+    description="PyDust",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MondoAurora/pydust/dust",
     author="Zsolt Horvath",
     author_email="zsolte@gmail.com",
     license="Apache License 2.0",
     classifiers=[
```

