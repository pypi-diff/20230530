# Comparing `tmp/ocs-0.9.2.tar.gz` & `tmp/ocs-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocs-0.9.2.tar", last modified: Mon May  2 18:16:06 2022, max compression
+gzip compressed data, was "ocs-0.9.3.tar", last modified: Tue Jun 14 14:04:03 2022, max compression
```

## Comparing `ocs-0.9.2.tar` & `ocs-0.9.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 18:16:06.491720 ocs-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-05-02 18:15:47.000000 ocs-0.9.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-02 18:15:47.000000 ocs-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6291 2022-05-02 18:16:06.491720 ocs-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5599 2022-05-02 18:15:47.000000 ocs-0.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 18:16:06.495721 ocs-0.9.2/ocs/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-05-02 18:16:06.495721 ocs-0.9.2/ocs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 18:16:06.491720 ocs-0.9.2/ocs/agent/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23872 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/agent/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (121)    15431 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/agent/host_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7592 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/agent/influxdb_publisher.py
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8654 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/checkdata.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8530 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/client_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/client_http.py
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/client_t.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/matched_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    52236 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/ocs_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     6053 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/ocs_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13415 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/ocs_feed.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6604 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/ocs_systemd.py
--rw-r--r--   0 runner    (1001) docker     (121)     6974 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/ocs_twisted.py
--rw-r--r--   0 runner    (1001) docker     (121)    39619 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/ocsbow.py
--rw-r--r--   0 runner    (1001) docker     (121)     3807 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/rename.py
--rw-r--r--   0 runner    (1001) docker     (121)    27103 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/site_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 18:16:06.491720 ocs-0.9.2/ocs/support/
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/support/crossbar_config.json
--rw-r--r--   0 runner    (1001) docker     (121)     4641 2022-05-02 18:15:47.000000 ocs-0.9.2/ocs/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 18:16:06.491720 ocs-0.9.2/ocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6291 2022-05-02 18:16:05.000000 ocs-0.9.2/ocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-05-02 18:16:06.000000 ocs-0.9.2/ocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-02 18:16:06.000000 ocs-0.9.2/ocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-02 18:16:06.000000 ocs-0.9.2/ocs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-05-02 18:16:06.000000 ocs-0.9.2/ocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-05-02 18:16:06.000000 ocs-0.9.2/ocs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-05-02 18:15:47.000000 ocs-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-05-02 18:16:06.491720 ocs-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-05-02 18:15:47.000000 ocs-0.9.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    69019 2022-05-02 18:15:47.000000 ocs-0.9.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 14:04:03.808024 ocs-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-06-14 14:03:45.000000 ocs-0.9.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-14 14:03:45.000000 ocs-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6254 2022-06-14 14:04:03.808024 ocs-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5599 2022-06-14 14:03:45.000000 ocs-0.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 14:04:03.808024 ocs-0.9.3/ocs/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-06-14 14:04:03.808024 ocs-0.9.3/ocs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 14:04:03.808024 ocs-0.9.3/ocs/agent/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23872 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/agent/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15463 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/agent/host_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7592 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/agent/influxdb_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8654 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/checkdata.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8530 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/client_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3499 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/client_http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/client_t.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/matched_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52236 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/ocs_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6128 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/ocs_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13322 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/ocs_feed.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6604 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/ocs_systemd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6974 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/ocs_twisted.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39619 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/ocsbow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3807 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/rename.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27103 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/site_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 14:04:03.808024 ocs-0.9.3/ocs/support/
+-rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/support/crossbar_config.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4641 2022-06-14 14:03:45.000000 ocs-0.9.3/ocs/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 14:04:03.804024 ocs-0.9.3/ocs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6254 2022-06-14 14:04:03.000000 ocs-0.9.3/ocs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-06-14 14:04:03.000000 ocs-0.9.3/ocs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-14 14:04:03.000000 ocs-0.9.3/ocs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-06-14 14:04:03.000000 ocs-0.9.3/ocs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-06-14 14:04:03.000000 ocs-0.9.3/ocs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-06-14 14:04:03.000000 ocs-0.9.3/ocs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-06-14 14:03:45.000000 ocs-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-06-14 14:04:03.808024 ocs-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-06-14 14:03:45.000000 ocs-0.9.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69019 2022-06-14 14:03:45.000000 ocs-0.9.3/versioneer.py
```

### Comparing `ocs-0.9.2/LICENSE.txt` & `ocs-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/PKG-INFO` & `ocs-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ocs
-Version: 0.9.2
+Version: 0.9.3
 Summary: Observatory Control System
 Home-page: https://github.com/simonsobs/ocs
-License: UNKNOWN
 Project-URL: Source Code, https://github.com/simonsobs/ocs
 Project-URL: Documentation, https://ocs.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/simonsobs/ocs/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Framework :: Twisted
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -171,9 +169,7 @@
 
 License
 --------
 This project is licensed under the BSD 2-Clause License - see the
 `LICENSE.txt`_ file for details.
 
 .. _LICENSE.txt: https://github.com/simonsobs/ocs/blob/master/LICENSE.txt
-
-
```

### Comparing `ocs-0.9.2/README.rst` & `ocs-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/agent/aggregator.py` & `ocs-0.9.3/ocs/agent/aggregator.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/agent/host_manager.py` & `ocs-0.9.3/ocs/agent/host_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 
 
 def _run_docker_compose(args, docker_compose_bin=None):
     # Help avoid some boilerplate.
     if docker_compose_bin is None:
         docker_compose_bin = shutil.which('docker-compose')
     return utils.getProcessOutputAndValue(
-        docker_compose_bin, args)
+        docker_compose_bin, args, env=os.environ)
 
 
 class DockerContainerHelper:
 
     """Class for managing the docker container associated with some
     service.  Provides some of the same interface as
     AgentProcessHelper in HostManager agent.  Pass in a service
@@ -366,15 +366,15 @@
 
     cont_ids = [line.strip() for line in out.decode('utf8').split('\n')
                 if line.strip() != '']
 
     # Run docker inspect.
     for cont_id in cont_ids:
         out, err, code = yield utils.getProcessOutputAndValue(
-            'docker', ['inspect', cont_id])
+            'docker', ['inspect', cont_id], env=os.environ)
         if code != 0 and 'No such object' in err.decode('utf8'):
             # This is likely due to a race condition where some
             # container was brought down since we ran docker-compose.
             # Just drop the entry.
             print(f'(no such object: {cont_id}')
             continue
         elif code != 0:
```

### Comparing `ocs-0.9.2/ocs/agent/influxdb_publisher.py` & `ocs-0.9.3/ocs/agent/influxdb_publisher.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/base.py` & `ocs-0.9.3/ocs/base.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/checkdata.py` & `ocs-0.9.3/ocs/checkdata.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/client_cli.py` & `ocs-0.9.3/ocs/client_cli.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/client_http.py` & `ocs-0.9.3/ocs/client_http.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/client_t.py` & `ocs-0.9.3/ocs/client_t.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/ocs_agent.py` & `ocs-0.9.3/ocs/ocs_agent.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/ocs_client.py` & `ocs-0.9.3/ocs/ocs_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,17 @@
             setattr(self, _opname_to_attr(name),
                     _get_op('task', name, encoded, self._client))
 
         for name, _, encoded in self._api['processes']:
             setattr(self, _opname_to_attr(name),
                     _get_op('process', name, encoded, self._client))
 
+    def __repr__(self):
+        return f"OCSClient('{self.instance_id}')"
+
 
 def _humanized_time(t):
     if abs(t) < 1.:
         return '%.6f s' % t
     if abs(t) < 120:
         return '%.1f s' % t
     if abs(t) < 120*60:
```

### Comparing `ocs-0.9.2/ocs/ocs_feed.py` & `ocs-0.9.3/ocs/ocs_feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,16 @@
     def encoded(self):
         return {
             "agent_address": self.agent_address,
             "agg_params": self.agg_params,
             "feed_name": self.feed_name,
             "address": self.address,
             "record": self.record,
-            "session_id": self.agent.agent_session_id
+            "session_id": self.agent.agent_session_id,
+            "agent_class": self.agent.class_name
         }
 
     def flush_buffer(self):
         """Publishes all messages in buffer and empties it."""
 
         if not in_reactor_context():
             return reactor.callFromThread(self.flush_buffer)
@@ -243,33 +244,31 @@
     @staticmethod
     def verify_message_data_type(value):
         """Aggregated Feeds can only store certain types of data. Here we check
         that the type of all data contained in a message's 'data' dictionary are
         supported types.
 
         Args:
-            value (list, float, int):
+            value (list, float, int, bool):
                 'data' dictionary value published (see Feed.publish_message for details).
 
         """
-        valid_types = (float, int, str)
+        valid_types = (float, int, str, bool)
 
-        # separate bool checks since bool is a subclass of int
         # multi-sample check
         if isinstance(value, list):
-            if (any(isinstance(x, bool) for x in value)
-                    or not all(isinstance(x, valid_types) for x in value)):
+            if not all(isinstance(x, valid_types) for x in value):
                 type_set = set([type(x) for x in value])
                 invalid_types = type_set.difference(valid_types)
                 raise TypeError("message 'data' block contains invalid data" +
                                 f"types: {invalid_types}")
 
         # single sample check
         else:
-            if isinstance(value, bool) or not isinstance(value, valid_types):
+            if not isinstance(value, valid_types):
                 invalid_type = type(value)
                 raise TypeError("message 'data' block contains invalid " +
                                 f"data type: {invalid_type}")
 
     @staticmethod
     def verify_data_field_string(field):
         """There are strict rules for the characters allowed in field names.
```

### Comparing `ocs-0.9.2/ocs/ocs_systemd.py` & `ocs-0.9.3/ocs/ocs_systemd.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/ocs_twisted.py` & `ocs-0.9.3/ocs/ocs_twisted.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/ocsbow.py` & `ocs-0.9.3/ocs/ocsbow.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/rename.py` & `ocs-0.9.3/ocs/rename.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/site_config.py` & `ocs-0.9.3/ocs/site_config.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/support/crossbar_config.json` & `ocs-0.9.3/ocs/support/crossbar_config.json`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs/testing.py` & `ocs-0.9.3/ocs/testing.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/ocs.egg-info/PKG-INFO` & `ocs-0.9.3/ocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ocs
-Version: 0.9.2
+Version: 0.9.3
 Summary: Observatory Control System
 Home-page: https://github.com/simonsobs/ocs
-License: UNKNOWN
 Project-URL: Source Code, https://github.com/simonsobs/ocs
 Project-URL: Documentation, https://ocs.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/simonsobs/ocs/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Framework :: Twisted
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -171,9 +169,7 @@
 
 License
 --------
 This project is licensed under the BSD 2-Clause License - see the
 `LICENSE.txt`_ file for details.
 
 .. _LICENSE.txt: https://github.com/simonsobs/ocs/blob/master/LICENSE.txt
-
-
```

### Comparing `ocs-0.9.2/ocs.egg-info/SOURCES.txt` & `ocs-0.9.3/ocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/setup.py` & `ocs-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `ocs-0.9.2/versioneer.py` & `ocs-0.9.3/versioneer.py`

 * *Files identical despite different names*

