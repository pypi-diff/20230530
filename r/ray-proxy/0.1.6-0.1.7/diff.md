# Comparing `tmp/ray-proxy-0.1.6.tar.gz` & `tmp/ray_proxy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ray-proxy-0.1.6.tar", max compression
+gzip compressed data, was "ray_proxy-0.1.7.tar", max compression
```

## Comparing `ray-proxy-0.1.6.tar` & `ray_proxy-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,24 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.954000 ray-proxy-0.1.6/LICENSE
--rw-r--r--   0        0        0      520 2022-10-01 12:28:22.461700 ray-proxy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      114 2022-10-01 08:27:27.593094 ray-proxy-0.1.6/ray_proxy/__init__.py
--rw-r--r--   0        0        0     4818 2022-10-01 06:48:59.099529 ray-proxy-0.1.6/ray_proxy/interface.py
--rw-r--r--   0        0        0    10139 2022-10-01 12:27:54.780112 ray-proxy-0.1.6/ray_proxy/py_environment.py
--rw-r--r--   0        0        0      746 2022-08-26 04:22:55.954688 ray-proxy-0.1.6/ray_proxy/ray_queue.py
--rw-r--r--   0        0        0     6666 2022-10-01 06:48:59.135403 ray-proxy-0.1.6/ray_proxy/remote_env.py
--rw-r--r--   0        0        0     2461 2022-10-01 06:48:59.213161 ray-proxy-0.1.6/ray_proxy/remote_prog_bar.py
--rw-r--r--   0        0        0     9440 2022-10-01 11:31:53.576530 ray-proxy-0.1.6/ray_proxy/remote_proxy.py
--rw-r--r--   0        0        0      714 2022-10-01 12:28:29.090456 ray-proxy-0.1.6/setup.py
--rw-r--r--   0        0        0      661 2022-10-01 12:28:29.090643 ray-proxy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 ray_proxy-0.1.7/LICENSE
+-rw-r--r--   0        0        0      537 2023-05-30 06:13:53.441052 ray_proxy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      114 2022-10-01 08:27:27.000000 ray_proxy-0.1.7/ray_proxy/__init__.py
+-rw-r--r--   0        0        0    13299 2022-10-18 04:07:37.000000 ray_proxy-0.1.7/ray_proxy/async_interpreter.py
+-rw-r--r--   0        0        0     8367 2023-05-30 06:13:37.245007 ray_proxy-0.1.7/ray_proxy/cluster_resource.py
+-rw-r--r--   0        0        0    16420 2022-10-18 12:38:00.000000 ray_proxy-0.1.7/ray_proxy/cluster_task_scheduler.py
+-rw-r--r--   0        0        0     2838 2022-10-19 02:45:28.000000 ray_proxy-0.1.7/ray_proxy/injected_resource.py
+-rw-r--r--   0        0        0     5025 2022-10-25 10:32:32.000000 ray_proxy-0.1.7/ray_proxy/interface.py
+-rw-r--r--   0        0        0     2398 2023-05-30 06:13:37.245690 ray_proxy-0.1.7/ray_proxy/local_var.py
+-rw-r--r--   0        0        0      272 2022-10-18 04:07:37.000000 ray_proxy-0.1.7/ray_proxy/prepared.py
+-rw-r--r--   0        0        0    11689 2023-05-30 06:13:37.246538 ray_proxy-0.1.7/ray_proxy/py_environment.py
+-rw-r--r--   0        0        0      746 2022-08-26 04:22:55.000000 ray_proxy-0.1.7/ray_proxy/ray_queue.py
+-rw-r--r--   0        0        0     1107 2022-10-24 06:03:35.000000 ray_proxy-0.1.7/ray_proxy/releasable.py
+-rw-r--r--   0        0        0     8706 2022-10-25 10:32:32.000000 ray_proxy-0.1.7/ray_proxy/remote_env.py
+-rw-r--r--   0        0        0     2461 2022-10-01 06:48:59.000000 ray_proxy-0.1.7/ray_proxy/remote_prog_bar.py
+-rw-r--r--   0        0        0    11617 2023-05-30 06:13:37.247177 ray_proxy-0.1.7/ray_proxy/remote_proxy.py
+-rw-r--r--   0        0        0     4891 2023-05-30 06:13:37.247571 ray_proxy-0.1.7/ray_proxy/resource_design.py
+-rw-r--r--   0        0        0    15326 2023-05-30 06:13:37.248223 ray_proxy-0.1.7/ray_proxy/resource_scheduler.py
+-rw-r--r--   0        0        0     9108 2023-05-30 06:13:37.248746 ray_proxy-0.1.7/ray_proxy/resource_scheduler_client.py
+-rw-r--r--   0        0        0     1170 2022-10-06 07:02:24.000000 ray_proxy-0.1.7/ray_proxy/serialization_check.py
+-rw-r--r--   0        0        0      222 2022-10-24 06:03:35.000000 ray_proxy-0.1.7/ray_proxy/type_aliases.py
+-rw-r--r--   0        0        0      239 2022-10-18 04:07:37.000000 ray_proxy-0.1.7/ray_proxy/util.py
+-rw-r--r--   0        0        0     2696 2022-11-19 11:26:29.000000 ray_proxy-0.1.7/ray_proxy/var_interface.py
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 ray_proxy-0.1.7/PKG-INFO
```

### Comparing `ray-proxy-0.1.6/LICENSE` & `ray_proxy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ray-proxy-0.1.6/pyproject.toml` & `ray_proxy-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "ray-proxy"
-version = "0.1.6"
+version = "0.1.7"
 description = "A library which enables the creation of proxy variables for remote python interpreter in ray cluster."
 authors = ["proboscis <nameissoap@gmail.com>"]
 packages = [{ include = "ray_proxy" }]
 license = "MIT"
 [tool.poetry.dependencies]
 python = "^3.7"
 ray = "^2.0.0"
-bidict = "*"
-returns = "*"
-loguru = "*"
+loguru = "^0.6.0"
+bidict = "^0.22.0"
+returns = "^0.19.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ray-proxy-0.1.6/ray_proxy/interface.py` & `ray_proxy-0.1.7/ray_proxy/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,17 @@
         """fetch the actual value of id-associated object"""
         pass
 
     @abstractmethod
     def getitem_id(self, id, item):
         """calls __getitem__ on the id-associated object"""
         pass
+    @abstractmethod
+    def setitem_id(self, id, item, value):
+        pass
 
     @abstractmethod
     def dir_of_id(self, id):
         """calls dir() on the id-associated object"""
         pass
 
     @abstractmethod
@@ -169,7 +172,15 @@
         """returns a list of names of instances of this interpreter"""
         pass
 
     @abstractmethod
     def __contains__(self, item: Union[str, UUID]):
         """returns True if item is in this interpreter"""
         pass
+
+    @abstractmethod
+    def publish_id(self,id)->ObjectRef:
+        pass
+
+    @abstractmethod
+    def destroy(self):
+        pass
```

### Comparing `ray-proxy-0.1.6/ray_proxy/py_environment.py` & `ray_proxy-0.1.7/ray_proxy/py_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 import uuid
 from collections import defaultdict
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from typing import Callable, Union, Any
 
 import ray
+from bidict import bidict
 from ray import ObjectRef
 from ray.actor import ActorHandle
 from ray.util.queue import Queue
-from bidict import bidict
+
+from ray_proxy.prepared import PreparedRef
 
 
 @dataclass
 class PyInterpreter:
+    # todo make this interpreter async so that recursive call can be accepted.
     env_id: uuid.UUID = field(default_factory=uuid.uuid4)
     instances: dict = field(default_factory=dict)  # id->instance mapping
     ref_counts: dict = field(
         default_factory=lambda: defaultdict(int))  # todo ref_counts is not reliable at this moment.
     named_instances: bidict = field(default_factory=bidict)  # mapping from name to id and vice versa.
 
     def __post_init__(self):
+        #TODO implement a
         self.host = socket.gethostname()
         print(f"PyInterpreter created at {self.host}")
 
     def reset(self):
         from loguru import logger
         logger.info(f"resetting interpreter. only named variables are kept.")
         prev_instances = self.instances
@@ -51,22 +55,30 @@
     def run(self, func: Callable, args=None, kwargs=None):
         return self.run_with_proxy(func, args, kwargs)
 
     def _unwrap(self, proxy: "RemoteProxy"):
         from ray_proxy.remote_proxy import Var
         if isinstance(proxy, Var):
             # unwrap if the proxy lives in this environment
+            # this can cause a deadlock. since two envs can try to fetch from each other at the same time.
+            # we need to stop calling ray.get here.
             from loguru import logger
             assert isinstance(proxy.env.id, ObjectRef), f"proxy.env.id is not a reference:{type(proxy.env.id)}"
-            eid = ray.get(proxy.env.id)
+            eid = ray.get(proxy.env.id)  # this fine since no actor is involved
             if self.env_id == eid:
                 return self.instances[ray.get(proxy.id)]
             else:
                 logger.warning(f"fetching from a proxy which lives in different env:{eid}")
-                return proxy.fetch()
+                # we need to somehow trace the call stack to see if the var is from the calling site...
+                logger.warning(f"beware that fetching a proxy var which lives in different env result in deadlock! if the env is the calling site")
+                #raise RuntimeError("cross interface variable passing is forbidden since this causes a deadlock.")
+                # this error should never be raised. extra care needs to be taken in the ActoRefRemoteInterpreter class.
+                # return proxy.fetch()  # this, can cause a deadlock
+        if isinstance(proxy, PreparedRef):  # this does not cause deadlock since the value is already uploaded.
+            return proxy.fetch()
         if isinstance(proxy, tuple):
             return tuple(self._unwrap(item) for item in proxy)
         if isinstance(proxy, list):
             return [self._unwrap(item) for item in proxy]
         if isinstance(proxy, dict):
             return {self._unwrap(key): self._unwrap(value) for key, value in proxy.items()}
 
@@ -93,26 +105,26 @@
         while uuid in self.instances:
             uuid = uuid.uuid4()
         self.instances[uuid] = instance
         self.incr_ref_id(uuid)
         return uuid
 
     def unregister_id(self, id):
-        from loguru import logger
         print(f"unregister_id:{id}")
         self.decr_ref_id(id)
 
     def incr_ref_id(self, id):
         # print(f"incr_ref_id:{id}")
         self.ref_counts[id] += 1
         return "incr_ref_success"
 
     def decr_ref_id(self, id):
         # assert self.ref_counts[id] > 0, "unregistering something doesn't exist"
         # print(f"decr_ref_id:{id}")
+        print(f"decr_ref_id:{id}")
         if id not in self.ref_counts:
             return "decr_ref_failure: id not found."
         self.ref_counts[id] -= 1
         if self.ref_counts[id] == 0 and id not in self.named_instances.inverse:
             # do not delete named instances.
             from loguru import logger
             # print(f"deleted instance:{self.instances[id]}")
@@ -176,14 +188,19 @@
         tgt = self.instances[id]
         setattr(tgt, attr, value)
 
     def getitem_of_id(self, id, item):
         item = self._unwrap(item)
         return self.register(self.instances[id][item])
 
+    def setitem_of_id(self, id, item, value):
+        item, value = self._unwrap(item), self._unwrap(value)
+        self.instances[id][item] = value
+        return self.register(None)
+
     def dir_of_id(self, id):
         res = dir(self.instances[id])
         return res
 
     def copy_of_id(self, id):
         item = self.instances[id]
         return self.register(item)
@@ -270,7 +287,17 @@
         return list(self.named_instances.keys())
 
     def __contains__(self, item: Union[str, uuid.UUID]):
         if isinstance(item, str):
             return item in self.named_instances
         if isinstance(item, uuid.UUID):
             return item in self.instances
+
+    def contains(self, item: Union[str, uuid.UUID]):
+        return item in self
+
+    def publish_id(self, id) -> ObjectRef:
+        """publish the object associated with this id to object store.
+        this makes it possible for user to retrieve the data without deadlock.
+        """
+        data = self.instances[id]
+        return ray.put(data)
```

### Comparing `ray-proxy-0.1.6/ray_proxy/ray_queue.py` & `ray_proxy-0.1.7/ray_proxy/ray_queue.py`

 * *Files identical despite different names*

### Comparing `ray-proxy-0.1.6/ray_proxy/remote_env.py` & `ray_proxy-0.1.7/ray_proxy/remote_env.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,98 @@
+import asyncio
 from dataclasses import dataclass, field
+from multiprocessing.pool import ThreadPool
 from typing import TypeVar, Union, List, Dict
 from uuid import UUID
 
 import ray
 from ray import ObjectRef
 from ray.actor import ActorHandle
 from ray.util.client.common import ClientActorHandle
 from returns.result import safe, Result
 
 from ray_proxy.interface import IRemoteInterpreter
+from ray_proxy.prepared import PreparedRef
 from ray_proxy.py_environment import PyInterpreter
 from ray_proxy.remote_proxy import Var, RemoteBlockingIterator
 
 
 @dataclass
 class ActorRefRemoteInterpreter(IRemoteInterpreter):
     remote_env: ActorHandle
     remote_env_refs: ActorHandle = field(default=None)
     remote_env_id_ref: ObjectRef = field(default=None)
-    remote_env_id:UUID = field(default=None)
+    remote_env_id: UUID = field(default=None)
+
+    def _blocking_prep(self, x):
+        match x:
+            case list():
+                return [self._blocking_prep(y) for y in x]
+            case tuple():
+                return tuple(self._blocking_prep(y) for y in x)
+            case dict():
+                keys = self._blocking_prep(list(x.keys()))
+                values = self._blocking_prep(list(x.values()))
+                return {k: v for k, v in zip(keys, values)}
+            case Var() as v if v.env.id != self.remote_env_id_ref:
+                ref = v.env.publish_id(v.id)
+                print(f"waiting for publish")
+                published = ray.get(ref)
+                print(f"published!")
+                return PreparedRef(published)
+            case Var() as v if v.env.id == self.remote_env_id_ref:
+                return v
+            case o:
+                return o
+
+    def _prepare(self, x):
+        return self._blocking_prep(x)
 
     def __post_init__(self):
         if self.remote_env_id_ref is None:
             self.remote_env_id_ref = self.remote_env.get_env_id.remote()
         if self.remote_env_refs is None:
             self.remote_env_refs = self.remote_env
         assert isinstance(self.remote_env_id_ref, ObjectRef), f"remote env id must be an object ref"
         assert isinstance(self.remote_env, (ActorHandle, ClientActorHandle)), \
             f"main env actor must be an instance of ActorHandle,{type(self.remote_env)}"
         assert isinstance(self.remote_env_refs, (ActorHandle, ClientActorHandle)), \
             f"main env refs must be an instance of ActorHandle,{type(self.remote_env_refs)}"
 
+    def publish_id(self, id) -> ObjectRef:
+        """an ObjectRef of an ObejctRef generated by ray.put"""
+        print(f"publishihng object to retrievable")
+        return self.remote_env.publish_id.remote(id)
+
     def delete_unnamed_vars(self):
         ray.get(self.remote_env.reset.remote())
 
     def run(self, func, args=None, kwargs=None) -> Var:
         return Var(
             self,
-            self.remote_env.run_with_proxy.remote(func, args, kwargs)
+            self.remote_env.run_with_proxy.remote(func, self._prepare(args), self._prepare(kwargs))
         )
 
     def get_host(self) -> ObjectRef:
         return self.remote_env.get_host.remote()
 
     def put(self, item) -> Var:
         # logger.info(f"put item:{item}")
         return Var(
             self,
-            self.remote_env.register.remote(item)
+            self.remote_env.register.remote(self._prepare(item))
         )
 
     def put_named(self, name: str, item) -> Var:
+        item = self._prepare(item)
+        id_ref = self.remote_env.put_named.remote(item, name)
+        # ray.get(id_ref)
         return Var(
             self,
-            self.remote_env.put_named.remote(item, name)
+            id_ref
         )
 
     def get_named_instances(self) -> Dict[str, Var]:
         return {k: Var(self, ray.put(_id)) for k, _id in
                 ray.get(self.remote_env.get_named_instances.remote()).items()}
 
     def get_named(self, name: str) -> Var:
@@ -66,64 +101,75 @@
             self.remote_env.get_named.remote(name)
         )
 
     def del_named(self, name: str) -> ObjectRef:
         return self.remote_env.del_named.remote(name)
 
     def call_id(self, id, args=None, kwargs=None) -> Var:
+        args, kwargs = self._prepare((args, kwargs))
         res_ref = self.remote_env.call_id.remote(id, args, kwargs)
         # ray.get(res_ref)
         return self.proxy(res_ref)
 
     def call_id_with_not_implemented(self, id, args=None, kwargs=None) -> Var:
+        args, kwargs = self._prepare((args, kwargs))
         ref = self.remote_env.call_id_with_not_implemented.remote(id, args, kwargs)
         if ray.get(ref) == NotImplemented:
             return NotImplemented
         else:
             return self.proxy(ref)
 
     def method_call_id(self, id, method, args=None, kwargs=None) -> Var:
+        args, kwargs = self._prepare((args, kwargs))
         return self.proxy(self.remote_env.call_method_id.remote(id, method, args, kwargs))
 
     def operator_call_id(self, id, operator, args):
         """returns NotImplementedObject if the operator returns NotImplemented"""
+        args = self._prepare(args)
         ref = self.remote_env.call_operator_id.remote(id, operator, args)
         if ray.get(ref) == NotImplemented:
             return NotImplemented
         else:
             return self.proxy(ref)
 
     def attr_id(self, id: ObjectRef, item: str) -> Var:
         return self.proxy(self.remote_env.attr_of_id.remote(id, item))
 
     def setattr_id(self, id: ObjectRef, attr, value) -> ObjectRef:
+        value = self._prepare(value)
         return self.remote_env.setattr_of_id.remote(id, attr, value)
 
     def unregister(self, id):
         return self.remote_env.unregister_id.remote(id)
 
     def fetch_id(self, id) -> ObjectRef:
         return self.remote_env.fetch_id.remote(id)
 
     def getitem_id(self, id, item) -> Var:
+        item = self._prepare(item)
         return self.proxy(self.remote_env.getitem_of_id.remote(id, item))
 
+    def setitem_id(self, id, item, value) -> Var:
+        item, value = self._prepare((item, value))
+        return self.proxy(self.remote_env.setitem_of_id.remote(id, item, value))
+
     def dir_of_id(self, id) -> List[str]:
         return ray.get(self.remote_env.dir_of_id.remote(id))
 
     def incr_ref(self, id) -> ObjectRef:
         # we need to know if the remote_env is actually remote or not.
         return self.remote_env_refs.incr_ref_id.remote(id)
 
     def decr_ref(self, id) -> ObjectRef:
         # decr_ref must not be called inside PyEnvServerProxy
         # since it will cause deadlock.
         # we need to directly call the decr_ref_id of this proxy.
         # but how? maybe using global variables?
         #
+        print(f"decr_ref is called for {ray.get(id)}")
         return self.remote_env_refs.decr_ref_id.remote(id)
 
     def type_of_id(self, id) -> Var:
         return self.func_on_id(id, type)
 
     def next_of_id(self, id) -> Var:
         return self.proxy(self.remote_env.next_of_id.remote(id))
@@ -154,28 +200,33 @@
     def id(self) -> ObjectRef:
         return self.remote_env_id_ref
 
     def instance_names(self) -> List[str]:
         return ray.get(self.remote_env.get_instance_names.remote())
 
     def __contains__(self, item: Union[str, UUID, ObjectRef]) -> bool:
-        return ray.get(self.remote_env.__contains__.remote(item))
+        item = self._prepare(item)
+        return ray.get(self.remote_env.contains.remote(item))
+
+    def destroy(self):
+        ray.kill(self.remote_env)
 
 
 @dataclass
 class RemoteInterpreterFactory:
     ray: "ray"
 
     def create(self, **options) -> IRemoteInterpreter:
         actor = self.ray.remote(PyInterpreter).options(**options).remote()
+        # actor = self.ray.remote(AsyncPyInterpreter).options(**options).remote()
         return ActorRefRemoteInterpreter(actor)
 
     def get(self, name) -> IRemoteInterpreter:
         actor = ray.get_actor(name)
-        kind = ray.get(actor.get_kind.remote())
+        # kind = ray.get(actor.get_kind.remote())
         return ActorRefRemoteInterpreter(actor)
 
     def __getitem__(self, env_name) -> IRemoteInterpreter:
         return self.get(env_name)
 
     def destroy(self, name) -> Result:
         return safe(ray.get_actor)(name).map(ray.kill)
```

### Comparing `ray-proxy-0.1.6/ray_proxy/remote_prog_bar.py` & `ray_proxy-0.1.7/ray_proxy/remote_prog_bar.py`

 * *Files identical despite different names*

### Comparing `ray-proxy-0.1.6/ray_proxy/remote_proxy.py` & `ray_proxy-0.1.7/ray_proxy/remote_proxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,71 @@
 import atexit
 from dataclasses import dataclass
-from typing import Iterable
+from typing import Iterable, Generic, TypeVar
 
 import ray
 from ray import ObjectRef
 from ray.actor import ActorHandle
 from ray.exceptions import RayTaskError
 from ray.util.queue import Queue
 
+from ray_proxy.async_interpreter import MyStopIteration
 from ray_proxy.interface import IRemoteInterpreter
+from ray_proxy.var_interface import IVar
+
+T = TypeVar("T")
 
 
 @dataclass
-class Var:
+class Var(Generic[T]):
     """
     a proxy class that represents a variable which lives in the remote python interpreter.
     this, can be copied and used from multiple remote places if I implemnt the corrent reference counting mechanism!
     until then only one process can use this.
-    todo implement an reference counting actor. which can just live in remote environment.
     then call its incr/decr upon creating/deleting this instance
     when you send thie proxy to another, call incr() un receiving side.
     """
     env: IRemoteInterpreter  # RemoteEnvironment
     id: ObjectRef  # an id which can identify the variable at remote environment.
 
     def __post_init__(self):
         assert isinstance(self.id, ObjectRef)
         self.___proxy_dirs___ = None
-        self.released = False
+        self.released = True
         atexit.register(self.__atexit__)
+        # print(f"constructed id:{id(self)}")
 
     def __atexit__(self):
         # this is required because the __del__ is called
         # after the imported modules are destroyed on interpreter shutdown.
-        self.env.decr_ref(self.id)
-        self.released = True
+        if not self.released:
+            # oid = ray.get(self.id)
+            # print(f"deleting |{id(self)}| {self}")
+            print(f"sending release request for {self.id} in __atexit__")
+            self.env.decr_ref(self.id)
+            print(f"sent release request for {self.id}")
+            self.released = True
+            # print(f"released:{self.released}")
+
+    def __del__(self):
+        # print(f"dereferencing")
+        # logger.info(f"dereferencing:{self.id}")
+        # print(f"destructor call of id:{id(self)}: released?{self.released}")
+        if not self.released:
+            print(f"sending release request for {self.id} in __del__")
+            self.env.decr_ref(self.id)
+            print(f"decr_ref:{self.id}")
+            atexit.unregister(self.__atexit__)
+            self.deleted = True
+        # print(f"dereferencing done")
 
     def fetch(self):
         return ray.get(self.fetch_ref())
 
-    def fetch_ref(self):
+    def fetch_ref(self) -> ObjectRef:
         return self.env.fetch_id(self.id)
 
     def __str__(self):
         _str: Var = self.env.func_on_id(self.id, str)  # this returns proxy
         host = self.env.get_host()
         host, _repr, _id = ray.get([host, _str.fetch_ref(), self.env.id])
         # Var@zeus[abcde]:hello world
@@ -74,16 +96,20 @@
         elif item == "__setstate__":
             raise AttributeError(item)
         # logger.debug(f"__getattr__({item})")
         if item == "__bases__":
             raise AttributeError(item)
         if item == "__remote_class__":
             return self._remote_attr("__class__")
-        if self.___proxy_dirs___ is None:
-            self.___proxy_dirs___ = set(self.__dir__())
+        # ah, since some libraries expects AttributeError to be raised immidiately, so we need to block for the remote value.
+
+        if not item.startswith("__") and not item.startswith("_repr_"):
+            # special functions and repr functions needs special care.
+            return self._remote_attr(item)
+        self.___update_proxy_dirs___()
         if item.startswith("_") and item not in self.___proxy_dirs___:
             raise AttributeError(item)
         if item not in self.___proxy_dirs___:
             raise AttributeError(item)
         if item.startswith("_repr_"):  # for ipython visualizations
             return self._remote_attr(item).fetch()
         res = self._remote_attr(item)
@@ -94,14 +120,18 @@
             def __torch_function__(func, types, args=(), kwargs=None):
                 return res.env.call_id_with_not_implemented(res.id, (func, types), dict(args=args, kwargs=kwargs))
 
             return __torch_function__
 
         return res
 
+    def ___update_proxy_dirs___(self):
+        if self.___proxy_dirs___ is None:
+            self.___proxy_dirs___ = set(self.__dir__())
+
     def __setattr__(self, key, value):
         from loguru import logger
         if key in "id env ___proxy_dirs___ released".split():
             return super().__setattr__(key, value)
         logger.info(f"setting attribute:{key}={value}")
         res = self.env.setattr_id(self.id, key, value)
         self.___proxy_dirs___ = None  # invalidate dir cache so that we can access the new attr
@@ -109,38 +139,31 @@
 
     def __call__(self, *args, **kwargs):
         return self.env.call_id(self.id, args, kwargs)
 
     def __getitem__(self, item):
         return self.env.getitem_id(self.id, item)
 
+    def __setitem__(self, item, value):
+        return self.env.setitem_id(self.id, item, value)
+
     def __iter__(self):
         return self.env.iter_of_id(self.id)
 
-    def __del__(self):
-        # print(f"dereferencing")
-        # logger.info(f"dereferencing:{self.id}")
-        if not self.released:
-            self.env.decr_ref(self.id)
-            print(f"decr_ref:{self.id}")
-            atexit.unregister(self.__atexit__)
-        # print(f"dereferencing done")
-
     def __dir__(self) -> Iterable[str]:
         _dir = self.env.dir_of_id(self.id)
         # print(f"dir is called for {self}")
         return _dir
         # return ray.get(self.remote_env.dir_of_id.remote(self.id))
 
     def ___call_method___(self, method, args, kwargs):
         return self.env.method_call_id(self.id, method, args, kwargs)
         # return self._proxy(self.remote_env.call_method_id.remote(self.id, method, args, kwargs))
 
     def ___call_operator___(self, operator, *args):
-        args = [self.env.put_if_needed(a) for a in args]
         return self.env.operator_call_id(self.id, operator, args)
 
     def ___call_left_operator___(self, operator, arg):
         res = self.___call_operator___(operator, arg)
         if res == NotImplemented:
             # regardless of the type of arg, we need to call its right operator
             op_name = operator.replace("__", "")
@@ -189,21 +212,54 @@
 
     def __eq__(self, other):
         # the behavior is, if both of them return NotImplemented, the interpreter checks for id
         # so we can safely call directly.
         return self.___call_operator___("__eq__", other)
 
     def __bool__(self):
-        return self.___call_operator___("__bool__").fetch()
+        # we need to see whether the obj implements __bool__ before actually calling it.
+        self.___update_proxy_dirs___()
+        if "__bool__" in self.___proxy_dirs___:
+            return self.___call_operator___("__bool__").fetch()
+        else:
+            return self.env.put(bool)(self).fetch()
 
     def __type__(self):
         return self.env.type_of_id(self.id).fetch()
 
     def __len__(self):
-        return self.___call_operator___("__len__").fetch()
+        #self.___update_proxy_dirs___()
+        #return self.___call_operator___("__len__").fetch()
+        return self.env.put(len)(self).fetch()
+
+    def __lt__(self, other):
+        return self.___call_left_operator___("__lt__", other)
+
+    def __le__(self, other):
+        return self.___call_left_operator___("__le__", other)
+
+    def __ge__(self, other):
+        return self.___call_left_operator___("__ge__", other)
+
+    def __gt__(self, other):
+        return self.___call_left_operator___("__gt__", other)
+
+    def __ne__(self, other):
+        return self.___call_left_operator___("__ne__", other)
+
+    def __neg__(self, other):
+        return self.___call_left_operator___("__neg__", other)
+
+    def __await__(self):
+        return self.fetch_ref().__await__()
+
+    def __code__(self):
+        return self.___call_operator___("__code__", self).fetch()
+
+
 
 
 def rp_deserializer(state):
     rp = Var(state[0], state[1])
     return rp
 
 
@@ -238,14 +294,16 @@
         try:
             proxy: Var = self.src.env.next_of_id(self.src.id)
             ray.get(proxy.id)  # this is for raising StopIteration
             return proxy
         except RayTaskError as e:
             if isinstance(e.cause, StopIteration):
                 raise e.cause
+            if isinstance(e.cause, MyStopIteration):
+                raise StopIteration()
             else:
                 raise e
 
 
 @dataclass
 class RemoteIterator:
     in_queue: Queue
```

### Comparing `ray-proxy-0.1.6/PKG-INFO` & `ray_proxy-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ray-proxy
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library which enables the creation of proxy variables for remote python interpreter in ray cluster.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: bidict
-Requires-Dist: loguru
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bidict (>=0.22.0,<0.23.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: ray (>=2.0.0,<3.0.0)
-Requires-Dist: returns
+Requires-Dist: returns (>=0.19.0,<0.20.0)
```

