# Comparing `tmp/localstack-plugin-persistence-1.0.3.tar.gz` & `tmp/localstack-plugin-persistence-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-plugin-persistence-1.0.3.tar", last modified: Fri May  5 13:09:20 2023, max compression
+gzip compressed data, was "localstack-plugin-persistence-1.0.4.tar", last modified: Tue May 30 14:26:42 2023, max compression
```

## Comparing `localstack-plugin-persistence-1.0.3.tar` & `localstack-plugin-persistence-1.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.610731 localstack-plugin-persistence-1.0.3/
--rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-05 13:09:20.610791 localstack-plugin-persistence-1.0.3/PKG-INFO
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.605920 localstack-plugin-persistence-1.0.3/localstack_persistence/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      175 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/constants.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.606194 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      372 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/__plugins__.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.606788 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/
--rw-r--r--   0 giograno   (501) staff       (20)      533 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      259 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/botocore.py
--rw-r--r--   0 giograno   (501) staff       (20)     1514 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/cryptography.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.607062 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/services/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/services/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      391 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/services/acm.py
--rw-r--r--   0 giograno   (501) staff       (20)     1710 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/stdlib.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.607905 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      333 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/__plugins__.py
--rw-r--r--   0 giograno   (501) staff       (20)     1754 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/endpoints.py
--rw-r--r--   0 giograno   (501) staff       (20)     3155 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/load.py
--rw-r--r--   0 giograno   (501) staff       (20)     2038 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/manager.py
--rw-r--r--   0 giograno   (501) staff       (20)     1638 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/save.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.608449 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      337 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/__plugins__.py
--rw-r--r--   0 giograno   (501) staff       (20)      766 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/endpoints.py
--rw-r--r--   0 giograno   (501) staff       (20)     2478 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/reset.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.609426 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)     3410 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/__plugins__.py
--rw-r--r--   0 giograno   (501) staff       (20)     1030 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/api.py
--rw-r--r--   0 giograno   (501) staff       (20)      580 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/endpoints.py
--rw-r--r--   0 giograno   (501) staff       (20)     1640 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/load.py
--rw-r--r--   0 giograno   (501) staff       (20)     6973 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/manager.py
--rw-r--r--   0 giograno   (501) staff       (20)     1361 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/save.py
--rw-r--r--   0 giograno   (501) staff       (20)      584 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/utils.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.610597 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/
--rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/PKG-INFO
--rw-r--r--   0 giograno   (501) staff       (20)     1679 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/SOURCES.txt
--rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/dependency_links.txt
--rw-r--r--   0 giograno   (501) staff       (20)      925 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/entry_points.txt
--rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/not-zip-safe
--rw-r--r--   0 giograno   (501) staff       (20)      940 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/plux.json
--rw-r--r--   0 giograno   (501) staff       (20)      277 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/requires.txt
--rw-r--r--   0 giograno   (501) staff       (20)       23 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/top_level.txt
--rw-r--r--   0 giograno   (501) staff       (20)      571 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/pyproject.toml
--rw-r--r--   0 giograno   (501) staff       (20)      843 2023-05-05 13:09:20.611100 localstack-plugin-persistence-1.0.3/setup.cfg
--rwxr-xr-x   0 giograno   (501) staff       (20)       60 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/setup.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:42.122172 localstack-plugin-persistence-1.0.4/
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-30 14:26:42.122242 localstack-plugin-persistence-1.0.4/PKG-INFO
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:42.116899 localstack-plugin-persistence-1.0.4/localstack_persistence/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      175 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/constants.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:42.117179 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      370 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/__plugins__.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:42.117791 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/
+-rw-r--r--   0 giograno   (501) staff       (20)      533 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      259 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/botocore.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1514 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/cryptography.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:42.118220 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/services/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/services/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      391 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/services/acm.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1708 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/stdlib.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:42.119131 localstack-plugin-persistence-1.0.4/localstack_persistence/pods/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pods/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pods/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1753 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pods/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     3151 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pods/load.py
+-rw-r--r--   0 giograno   (501) staff       (20)     2035 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pods/manager.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1628 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/pods/save.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:42.119727 localstack-plugin-persistence-1.0.4/localstack_persistence/reset/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/reset/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      336 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/reset/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      765 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/reset/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     2474 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/reset/reset.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:42.120831 localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     3405 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1030 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/api.py
+-rw-r--r--   0 giograno   (501) staff       (20)      579 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1633 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/load.py
+-rw-r--r--   0 giograno   (501) staff       (20)     6970 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/manager.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1361 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/save.py
+-rw-r--r--   0 giograno   (501) staff       (20)      584 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_persistence/utils.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-30 14:26:42.122038 localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-30 14:26:42.000000 localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/PKG-INFO
+-rw-r--r--   0 giograno   (501) staff       (20)     1679 2023-05-30 14:26:42.000000 localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-30 14:26:42.000000 localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 giograno   (501) staff       (20)      925 2023-05-30 14:26:42.000000 localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/entry_points.txt
+-rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/not-zip-safe
+-rw-r--r--   0 giograno   (501) staff       (20)      940 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/plux.json
+-rw-r--r--   0 giograno   (501) staff       (20)      277 2023-05-30 14:26:42.000000 localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/requires.txt
+-rw-r--r--   0 giograno   (501) staff       (20)       23 2023-05-30 14:26:42.000000 localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/top_level.txt
+-rw-r--r--   0 giograno   (501) staff       (20)      571 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/pyproject.toml
+-rw-r--r--   0 giograno   (501) staff       (20)      843 2023-05-30 14:26:42.122578 localstack-plugin-persistence-1.0.4/setup.cfg
+-rwxr-xr-x   0 giograno   (501) staff       (20)       60 2023-05-30 14:26:41.000000 localstack-plugin-persistence-1.0.4/setup.py
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/__init__.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/cryptography.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/cryptography.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/stdlib.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/pickling/reducers/stdlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 @pickle.reducer(defaultdict,_create_defaultdict,subclasses=True)
 def pickle_defaultdict(obj):
 	A=obj
 	if type(A)==defaultdict:return defaultdict,A.default_factory,dict(A),None
 	return type(A),A.default_factory,dict(A),A.__dict__
 def _create_context(name_to_value):
 	A=contextvars.copy_context()
-	for (B,D) in A.items():
+	for(B,D)in A.items():
 		if(C:=name_to_value.get(B.name)):A.run(B.set,C)
 	return A
 @pickle.register(contextvars.Context)
 def pickle_contextvars_context(pickler,obj):A={A.name:B for(A,B)in list(obj.items())};return pickler.save_reduce(_create_context,(A,),obj=obj)
 def _create_context_vars(name,value):A=contextvars.ContextVar(name);A.set(value);return A
 @pickle.register(contextvars.ContextVar)
 def pickle_contextvars_contextvars(pickler,obj):A=obj;return pickler.save_reduce(_create_context_vars,(A.name,A.get()),obj=A)
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/pods/endpoints.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/pods/endpoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging,os,tempfile,time
 from zipfile import ZipFile
 from localstack.http import route
 from werkzeug import Request,Response
 from werkzeug.exceptions import BadRequest
 from werkzeug.utils import send_file
-from .manager import PodStateManager
+from.manager import PodStateManager
 LOG=logging.getLogger(__name__)
 class PublicPodsResource:
 	manager:0
 	def __init__(A,manager):A.manager=manager
 	@route('/_localstack/pods/environment')
 	def get_environment(self,request):
 		'TODO: we can add store versions in the future to this endpoint';import localstack.constants;from localstack import __version__ as B,config as C;from moto import __version__ as D
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/pods/load.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/pods/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 	def __init__(A,zip_file,decoder=None):A.zip=zip_file;A.pod=CloudPodArchive(A.zip);A.decoder=decoder or pickle.PickleDecoder()
 	@singledispatchmethod
 	def visit(self,state_container):LOG.warning('cannot save state container of type %s',type(state_container))
 	@visit.register(AccountRegionBundle)
 	def _(self,state_container):
 		B=state_container;A=self;C=B.service_name
 		if C not in A.pod.stores_index:return
-		for (D,E,F) in A.pod.stores_index[C]:
+		for(D,E,F)in A.pod.stores_index[C]:
 			with A.zip.open(F)as G:H=A.decoder.decode(G);B[D][E].__dict__.update(H.__dict__)
 	@visit.register(BackendDict)
 	def _(self,state_container):
 		B=state_container;A=self;C=B.service_name
 		if C not in A.pod.moto_backend_index:return
-		for (D,E,F) in A.pod.moto_backend_index[C]:
+		for(D,E,F)in A.pod.moto_backend_index[C]:
 			with A.zip.open(F)as G:H=A.decoder.decode(G);B[D][E].__dict__.update(H.__dict__)
 	@visit.register(AssetDirectory)
 	def _(self,state_container):
 		B=state_container
 		if not B.path.startswith(config.dirs.data):return
 		C=os.path.relpath(B.path,config.dirs.data)+_A;D=[A for A in self.zip.infolist()if A.filename.startswith(os.path.join(constants.ASSETS_DIRECTORY,C))]
 		for A in D:A.filename=A.filename.replace(f"{constants.ASSETS_DIRECTORY}{os.sep}",'');self.zip.extract(A,config.dirs.data)
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/pods/manager.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/pods/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging,zipfile
 from localstack.services.plugins import Service,ServiceManager
 from localstack.utils.functions import call_safe
-from ..utils import DefaultPrioritySorter,ServiceSorter
-from .load import CloudPodArchive,InjectPodVisitor
-from .save import CreatePodVisitor
+from..utils import DefaultPrioritySorter,ServiceSorter
+from.load import CloudPodArchive,InjectPodVisitor
+from.save import CreatePodVisitor
 LOG=logging.getLogger(__name__)
 class PodStateManager:
 	service_manager:0;service_sorter:0
 	def __init__(A,service_manager,service_sorter=None):A.service_manager=service_manager;A.service_sorter=service_sorter or DefaultPrioritySorter()
 	def extract_into(B,pod_archive,service_names=None):
 		'\n        Extracts the state of the currently running localstack instance and writes it into the given cloudpod.\n        :param pod_archive: the cloudpod archive to write to\n        :param service_names: a list of service to write in the cloudpod\n        :return: returns the list of services that have been extracted into the zip file\n        ';C=service_names;E=CreatePodVisitor(pod_archive);D=B.service_manager.values()if not C else[B.service_manager.get_service(A)for A in C]
 		for A in D:
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/pods/save.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/pods/save.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 	zip:0
 	def __init__(A,zip_file,encoder=None):A.zip=zip_file;A.encoder=encoder or pickle.PickleEncoder()
 	@singledispatchmethod
 	def visit(self,state_container):LOG.warning('cannot save state container of type %s',type(state_container))
 	@visit.register(AccountRegionBundle)
 	def _(self,state_container):
 		A=state_container;B=A.service_name
-		for (C,D) in A.items():
-			for (E,F) in D.items():
+		for(C,D)in A.items():
+			for(E,F)in D.items():
 				G=os.path.join(constants.API_STATES_DIRECTORY,C,B,E,constants.LOCALSTACK_STORE_STATE_FILE)
 				with self.zip.open(G,'w')as H:self.encoder.encode(F,H)
 	@visit.register(BackendDict)
 	def _(self,state_container):
 		A=state_container;B=A.service_name
-		for (C,D) in A.items():
-			for (E,F) in D.items():
+		for(C,D)in A.items():
+			for(E,F)in D.items():
 				G=os.path.join(constants.API_STATES_DIRECTORY,C,B,E,constants.MOTO_BACKEND_STATE_FILE)
 				with self.zip.open(G,'w')as H:self.encoder.encode(F,H)
 	@visit.register(AssetDirectory)
 	def _(self,state_container):
 		A=config.dirs.data;A=A.rstrip('/')
-		for (C,H,F) in os.walk(state_container.path):
+		for(C,H,F)in os.walk(state_container.path):
 			B=os.path.relpath(C,A).lstrip('/');B=os.path.join(constants.ASSETS_DIRECTORY,B);self.zip.writestr(zipfile.ZipInfo.from_file(A,B),'')
 			for D in F:
 				E=os.path.join(C,D)
 				if os.path.exists(E):G=os.path.join(B,D);self.zip.write(E,G)
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/reset/endpoints.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/reset/endpoints.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from localstack.http import Request,route
 from localstack.services.plugins import ServiceManager
-from .reset import reset_all,reset_state
+from.reset import reset_all,reset_state
 LOG=logging.getLogger(__name__)
 class StateResetResource:
 	'\n    Internal endpoints to trigger state reset.\n    ';service_manager:0
 	def __init__(A,service_manager):A.service_manager=service_manager
 	@route('/_localstack/state/<service>/reset',methods=['POST'])
 	def reset_service_state(self,request,service):
 		A=service
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/reset/reset.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/reset/reset.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 	@singledispatchmethod
 	def visit(self,state_container):LOG.warning('Cannot reset state container of type %s',type(state_container))
 	@visit.register(AccountRegionBundle)
 	def _(self,state_container):state_container.reset()
 	@visit.register(BackendDict)
 	def _(self,state_container):
 		A=state_container
-		for (E,B) in A.items():
+		for(E,B)in A.items():
 			for C in B.keys():
 				try:self._reset_moto_backend_state(B,C)
 				except Exception as D:
 					if LOG.isEnabledFor(logging.DEBUG):LOG.exception('failed to reset the state for BackendDict %s',A)
 					else:LOG.error('failed to reset the state for BackendDict %s: %s',A,D)
 	@visit.register(AssetDirectory)
 	def _(self,state_container):
@@ -41,8 +41,8 @@
 	def _reset_moto_backend_state(J,state_container,region_key):
 		D=state_container;B=region_key;A=D.get(B);E=getattr(A,'reset',None)
 		if E and callable(E):E();return A
 		from moto.applicationautoscaling.models import ApplicationAutoscalingBackend as G;from moto.autoscaling.models import AutoScalingBackend as H;from moto.redshift.models import RedshiftBackend as I;F=type(A);C=[B]if len(inspect.signature(F.__init__).parameters)>1 else[]
 		if isinstance(A,G):C.append(A.ecs_backend)
 		elif isinstance(A,I):C.insert(0,A.ec2_backend)
 		elif isinstance(A,H):C=[A.ec2_backend,A.elb_backend,A.elbv2_backend]
-		D[B]=F(*(C));return D[B]
+		D[B]=F(*C);return D[B]
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/__plugins__.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/__plugins__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging,os
 from localstack import config
 from localstack.aws.handlers import serve_custom_service_request_handlers
 from localstack.runtime import hooks,shutdown
 from localstack.utils.objects import singleton_factory
-from .api import LoadStrategy,SaveStrategy
+from.api import LoadStrategy,SaveStrategy
 LOG=logging.getLogger(__name__)
 DEFAULT_SAVE_STRATEGY=SaveStrategy.SCHEDULED
 def is_persistence_activated():return config.PERSISTENCE and'LOCALSTACK_API_KEY'in os.environ
 @singleton_factory
 def get_save_strategy():
 	try:
 		if config.SNAPSHOT_SAVE_STRATEGY:return SaveStrategy(config.SNAPSHOT_SAVE_STRATEGY)
@@ -16,31 +16,31 @@
 @singleton_factory
 def get_load_strategy():
 	try:
 		if config.SNAPSHOT_LOAD_STRATEGY:return LoadStrategy(config.SNAPSHOT_LOAD_STRATEGY)
 	except ValueError as A:LOG.warning('Invalid load strategy, falling back to on_startup: %s',A)
 	return LoadStrategy.ON_REQUEST
 @singleton_factory
-def get_service_state_manager():from localstack import config as A;from localstack.services.plugins import SERVICE_PLUGINS as B;from .manager import SnapshotManager as C;return C(B,A.dirs.data)
+def get_service_state_manager():from localstack import config as A;from localstack.services.plugins import SERVICE_PLUGINS as B;from.manager import SnapshotManager as C;return C(B,A.dirs.data)
 @hooks.on_infra_start(should_load=is_persistence_activated())
-def register_state_resource():from localstack.services.internal import get_internal_apis as A;from .endpoints import StateResource as B;C=B(get_service_state_manager());A().add(C)
+def register_state_resource():from localstack.services.internal import get_internal_apis as A;from.endpoints import StateResource as B;C=B(get_service_state_manager());A().add(C)
 @hooks.on_infra_start(should_load=is_persistence_activated(),priority=1)
 def register_state_load_strategy():
 	A=get_load_strategy();from localstack_persistence.snapshot.manager import LoadOnRequestHandler as B
 	match A:
 		case LoadStrategy.ON_STARTUP:LOG.info('registering ON_STARTUP load strategy');return
 		case LoadStrategy.ON_REQUEST:LOG.warning('registering ON_REQUEST load strategy: this strategy has known limitations to not restore state correctly for certain services');C=B(get_service_state_manager());serve_custom_service_request_handlers.append(C.on_request)
 		case LoadStrategy.MANUAL:LOG.info('registering MANUAL load strategy (call /_localstack/state endpoints to load state)')
 		case _:LOG.warning('Unknown load strategy %s',A)
 @hooks.on_infra_ready(should_load=is_persistence_activated(),priority=-10)
 def do_run_state_load_all():
 	A=get_load_strategy()
 	if A==LoadStrategy.ON_STARTUP:LOG.info('restoring state of all services');get_service_state_manager().load_all()
 @hooks.on_infra_start(should_load=is_persistence_activated())
 def register_state_save_strategy():
-	from localstack.aws.handlers import run_custom_response_handlers as C,serve_custom_service_request_handlers as D;from .api import SaveStrategy as A;from .manager import SaveOnRequestHandler as H,SaveStateScheduler as I;E=get_save_strategy();F=get_service_state_manager()
+	from localstack.aws.handlers import run_custom_response_handlers as C,serve_custom_service_request_handlers as D;from.api import SaveStrategy as A;from.manager import SaveOnRequestHandler as H,SaveStateScheduler as I;E=get_save_strategy();F=get_service_state_manager()
 	match E:
 		case A.ON_SHUTDOWN:LOG.info('registering ON_SHUTDOWN save strategy');shutdown.SHUTDOWN_HANDLERS.register(F.save_all)
 		case A.ON_REQUEST:LOG.info('registering ON_REQUEST save strategy');G=H(get_service_state_manager());D.append(G.on_request);C.append(G.on_response)
 		case A.SCHEDULED:LOG.info('registering SCHEDULED save strategy');B=I(F,period=15);shutdown.SHUTDOWN_HANDLERS.register(B.close);D.append(B.on_request);C.append(B.on_response);B.start()
 		case A.MANUAL:LOG.info('registering MANUAL save strategy (call /_localstack/state endpoints to save state)')
 		case _:LOG.warning('Unknown save strategy %s',E)
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/api.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/api.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/endpoints.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from localstack.http import Request,route
-from .manager import SnapshotManager
+from.manager import SnapshotManager
 class StateResource:
 	'\n    Internal endpoints to trigger state management operations.\n    ';service_state_manager:0
 	def __init__(A,service_state_manager):A.service_state_manager=service_state_manager
 	@route('/_localstack/state/<service>/load',methods=['POST'])
 	def load_service_state(self,request,service):self.service_state_manager.load(service)
 	@route('/_localstack/state/<service>/save',methods=['POST'])
 	def save_service_state(self,request,service):self.service_state_manager.save(service)
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/load.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 		if B is _A:return
 		A.update(dict(B));A.__dict__.update(B.__dict__)
 	@visit.register(BackendDict)
 	def _(self,state_container):
 		A=state_container;C=os.path.join(self.data_dir,A.service_name,constants.MOTO_BACKEND_STATE_FILE);B=self._deserialize_file(C)
 		if B is _A:return
 		A.update(B);A.__dict__.update(B.__dict__)
-		for (D,E) in B.items():
-			for (F,G) in E.items():A[D][F].__dict__.update(G.__dict__)
+		for(D,E)in B.items():
+			for(F,G)in E.items():A[D][F].__dict__.update(G.__dict__)
 	@visit.register(AssetDirectory)
 	def _(self,state_container):0
 	def _deserialize_file(B,fpath):
 		A=fpath
-		if not os.path.exists(A):return _A
+		if not os.path.exists(A):return
 		with open(A,'rb')as C:return B.decoder.decode(C)
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/manager.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from localstack.utils.functions import call_safe
 from localstack.utils.json import FileMappedDocument
 from localstack.utils.scheduler import Scheduler
 from localstack.utils.sync import SynchronizedDefaultDict
 from plugin import PluginManager
 from readerwriterlock import rwlock
 from localstack_persistence import constants
-from ..utils import DefaultPrioritySorter,ServiceSorter
-from .load import LoadSnapshotVisitor
-from .save import SaveSnapshotVisitor
+from..utils import DefaultPrioritySorter,ServiceSorter
+from.load import LoadSnapshotVisitor
+from.save import SaveSnapshotVisitor
 LOG=logging.getLogger(__name__)
 class SnapshotManager:
 	'\n    This implements the glue for making the simple disk-based persistence strategy work. It instantiates\n    the correct visitors, uses a ``ServiceManager`` to locate service plugins, and makes sure\n    ``StateLifecycleHook``s are invoked appropriately.\n    ';service_manager:0;data_dir:0;persistence_plugin_manager:0;service_sorter:0
 	def __init__(A,service_manager,data_dir,service_sorter=None):B=data_dir;A.data_dir=B;A.service_manager=service_manager;A.tracker=FileMappedDocument(os.path.join(B,constants.API_STATES_JSON));A.persistence_plugin_manager=PluginManager(SnapshotPersistencePlugin.namespace);A.service_sorter=service_sorter or DefaultPrioritySorter()
 	def load(C,service_name):
 		A=service_name;D=C._create_load_state_visitor(A)
 		if(B:=C.service_manager.get_service(A)):
```

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/save.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/snapshot/save.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.3/localstack_persistence/utils.py` & `localstack-plugin-persistence-1.0.4/localstack_persistence/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/SOURCES.txt` & `localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/entry_points.txt` & `localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/plux.json` & `localstack-plugin-persistence-1.0.4/localstack_plugin_persistence.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809524%*

 * *Differences: {"'localstack.hooks.on_infra_start'": '{insert: [(0, '*

 * *                                      "'register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource')], "*

 * *                                      'delete: [2]}'}*

```diff
@@ -1,15 +1,15 @@
 {
     "localstack.hooks.on_infra_ready": [
         "do_run_state_load_all=localstack_persistence.snapshot.__plugins__:do_run_state_load_all"
     ],
     "localstack.hooks.on_infra_start": [
+        "register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource",
         "register_public_cloudpods_endpoints=localstack_persistence.pods.__plugins__:register_public_cloudpods_endpoints",
         "register_pickle_patches_runtime=localstack_persistence.pickling.__plugins__:register_pickle_patches_runtime",
-        "register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource",
         "register_state_load_strategy=localstack_persistence.snapshot.__plugins__:register_state_load_strategy",
         "register_state_resource=localstack_persistence.snapshot.__plugins__:register_state_resource",
         "register_state_save_strategy=localstack_persistence.snapshot.__plugins__:register_state_save_strategy"
     ],
     "localstack.hooks.prepare_host": [
         "register_pickle_patches_host=localstack_persistence.pickling.__plugins__:register_pickle_patches_host"
     ]
```

### Comparing `localstack-plugin-persistence-1.0.3/pyproject.toml` & `localstack-plugin-persistence-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.3/setup.cfg` & `localstack-plugin-persistence-1.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = localstack-plugin-persistence
-version = 1.0.3
+version = 1.0.4
 url = https://github.com/localstack/localstack-plugin-persistence
 author = LocalStack Contributors
 author_email = info@localstack.cloud
 description = plugin containing persistence code
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
```

