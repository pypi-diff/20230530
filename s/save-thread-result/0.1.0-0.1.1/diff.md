# Comparing `tmp/save-thread-result-0.1.0.tar.gz` & `tmp/save-thread-result-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "save-thread-result-0.1.0.tar", last modified: Sat Dec 31 23:57:12 2022, max compression
+gzip compressed data, was "save-thread-result-0.1.1.tar", last modified: Tue May 30 00:18:57 2023, max compression
```

## Comparing `save-thread-result-0.1.0.tar` & `save-thread-result-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 shail      (503) staff       (20)        0 2022-12-31 23:57:12.806118 save-thread-result-0.1.0/
--rw-r--r--   0 shail      (503) staff       (20)    18918 2022-12-31 23:57:12.805707 save-thread-result-0.1.0/PKG-INFO
--rw-r--r--   0 shail      (503) staff       (20)     3824 2022-09-06 22:29:23.000000 save-thread-result-0.1.0/README.md
-drwxr-xr-x   0 shail      (503) staff       (20)        0 2022-12-31 23:57:12.803598 save-thread-result-0.1.0/save_thread_result/
--rw-r--r--   0 shail      (503) staff       (20)    12097 2022-12-31 23:53:14.000000 save-thread-result-0.1.0/save_thread_result/__init__.py
-drwxr-xr-x   0 shail      (503) staff       (20)        0 2022-12-31 23:57:12.805088 save-thread-result-0.1.0/save_thread_result.egg-info/
--rw-r--r--   0 shail      (503) staff       (20)    18918 2022-12-31 23:57:12.000000 save-thread-result-0.1.0/save_thread_result.egg-info/PKG-INFO
--rw-r--r--   0 shail      (503) staff       (20)      217 2022-12-31 23:57:12.000000 save-thread-result-0.1.0/save_thread_result.egg-info/SOURCES.txt
--rw-r--r--   0 shail      (503) staff       (20)        1 2022-12-31 23:57:12.000000 save-thread-result-0.1.0/save_thread_result.egg-info/dependency_links.txt
--rw-r--r--   0 shail      (503) staff       (20)       19 2022-12-31 23:57:12.000000 save-thread-result-0.1.0/save_thread_result.egg-info/top_level.txt
--rw-r--r--   0 shail      (503) staff       (20)       38 2022-12-31 23:57:12.806231 save-thread-result-0.1.0/setup.cfg
--rw-r--r--   0 shail      (503) staff       (20)    19102 2022-12-31 23:53:14.000000 save-thread-result-0.1.0/setup.py
+drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-05-30 00:18:57.599896 save-thread-result-0.1.1/
+-rw-r--r--   0 shail      (503) staff       (20)    19072 2023-05-30 00:18:57.599369 save-thread-result-0.1.1/PKG-INFO
+-rw-r--r--   0 shail      (503) staff       (20)     3981 2023-05-29 23:34:08.000000 save-thread-result-0.1.1/README.md
+drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-05-30 00:18:57.596168 save-thread-result-0.1.1/save_thread_result/
+-rw-r--r--   0 shail      (503) staff       (20)    16023 2023-05-30 00:16:54.000000 save-thread-result-0.1.1/save_thread_result/__init__.py
+drwxr-xr-x   0 shail      (503) staff       (20)        0 2023-05-30 00:18:57.598467 save-thread-result-0.1.1/save_thread_result.egg-info/
+-rw-r--r--   0 shail      (503) staff       (20)    19072 2023-05-30 00:18:57.000000 save-thread-result-0.1.1/save_thread_result.egg-info/PKG-INFO
+-rw-r--r--   0 shail      (503) staff       (20)      217 2023-05-30 00:18:57.000000 save-thread-result-0.1.1/save_thread_result.egg-info/SOURCES.txt
+-rw-r--r--   0 shail      (503) staff       (20)        1 2023-05-30 00:18:57.000000 save-thread-result-0.1.1/save_thread_result.egg-info/dependency_links.txt
+-rw-r--r--   0 shail      (503) staff       (20)       19 2023-05-30 00:18:57.000000 save-thread-result-0.1.1/save_thread_result.egg-info/top_level.txt
+-rw-r--r--   0 shail      (503) staff       (20)       38 2023-05-30 00:18:57.600051 save-thread-result-0.1.1/setup.cfg
+-rw-r--r--   0 shail      (503) staff       (20)    19099 2023-05-30 00:16:54.000000 save-thread-result-0.1.1/setup.py
```

### Comparing `save-thread-result-0.1.0/PKG-INFO` & `save-thread-result-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: save-thread-result
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple subclass wrapper around `threading.Thread` to get the return value from a thread in python. Exact same interface as `threading.Thread`! 🌟 Star this repo if you found it useful! 🌟
 Home-page: https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Author: slow-but-steady
 Author-email: slowbutsteady1234@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/slow-but-steady/save-thread-result/issues
 Project-URL: PyPi Funding, https://donate.pypi.org
@@ -270,15 +270,15 @@
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
-Requires-Python: >=3.0.*, <4
+Requires-Python: >3.0, <4
 Description-Content-Type: text/markdown
 
 # Python API
 
 ## Quickstart
 
 Installing the `save_thread_result` module:
@@ -330,37 +330,37 @@
 
 ## Examples
 
 Dummy example:
 ```
 from save_thread_result import ThreadWithResult
 
-import time, random
+import time, random, threading
 
 
 def function_to_thread(n):
     count = 0
     while count < 3:
-            print(f'Still running thread {n}...')
+            print(f'Still running {threading.current_thread().name}...')
             count +=1
             time.sleep(3)
     result = random.random()
-    print(f'Return value of thread {n} should be: {result}')
+    print(f'Return value of {threading.current_thread().name} should be: {result}')
     return result
 
 
 def main():
     thread1 = ThreadWithResult(target=function_to_thread, args=(1,))
     thread2 = ThreadWithResult(target=function_to_thread, args=(2,))
     thread1.start()
     thread2.start()
     thread1.join()
     thread2.join()
-    print(thread1.result)
-    print(thread2.result)
+    print(f'The `result` attribute of {thread1.name} is: {thread1.result}')
+    print(f'The `result` attribute of {thread2.name} is: {thread2.result}')
 
 main()
 ```
 
 <details>
   <summary><b>More information</b></summary>
```

### Comparing `save-thread-result-0.1.0/README.md` & `save-thread-result-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -51,37 +51,37 @@
 
 ## Examples
 
 Dummy example:
 ```
 from save_thread_result import ThreadWithResult
 
-import time, random
+import time, random, threading
 
 
 def function_to_thread(n):
     count = 0
     while count < 3:
-            print(f'Still running thread {n}...')
+            print(f'Still running {threading.current_thread().name}...')
             count +=1
             time.sleep(3)
     result = random.random()
-    print(f'Return value of thread {n} should be: {result}')
+    print(f'Return value of {threading.current_thread().name} should be: {result}')
     return result
 
 
 def main():
     thread1 = ThreadWithResult(target=function_to_thread, args=(1,))
     thread2 = ThreadWithResult(target=function_to_thread, args=(2,))
     thread1.start()
     thread2.start()
     thread1.join()
     thread2.join()
-    print(thread1.result)
-    print(thread2.result)
+    print(f'The `result` attribute of {thread1.name} is: {thread1.result}')
+    print(f'The `result` attribute of {thread2.name} is: {thread2.result}')
 
 main()
 ```
 
 <details>
   <summary><b>More information</b></summary>
```

### Comparing `save-thread-result-0.1.0/save_thread_result/__init__.py` & `save-thread-result-0.1.1/save_thread_result/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 '''
 import sys
 import time
 import threading
 from datetime import datetime
 
 
-__version__              = '0.1.0'
+__version__              = '0.1.1'
 
 
-class ThreadWithResult(threading.Thread):
-    '''
+_general_documentation = '''
     The `threading.Thread` subclass `ThreadWithResult` saves the result of a thread
     as its `result` attribute - i.e. call `thread_with_result_instance_1.result`
     after `thread_with_result_instance_1` finishes running to get the return
     value from the function that ran on that thread:
 
     >>> thread = ThreadWithResult(
         target = my_function,
@@ -72,42 +71,14 @@
     You can also specify `threading.Thread` attributes such as
     `group`, `name`, and `daemon` by passing in the value you want to
     set them to as keyword arguments to `ThreadWithResult`
 
 
 
 
-    EXPLANATION:
-    We create a closure function to run the actual function we want
-    to run on a separate thread, enclose the function passed to
-    `target` - along with the arguments provided to `args` and `kwargs` -
-    inside the closure function, and pass the CLOSURE FUNCTION
-    as the function to the `target` argument in the
-    `super.__init__()` call to `threading.Thread`:
-    super().__init__(group=group, target=closure_function, name=name, daemon=daemon)
-
-    Since the function we want to run on a separate thread is no longer
-    the function passed directly to `threading.Thread` (remember,
-    we pass the closure function instead!), we save the result of
-    the enclosed function to the `self.result` attribute of the
-    instance.
-
-    We use inheritance to initialize this instance with the
-    closure function as the `target` function and no arguments
-    for `args` or `kwargs` (since we pass
-    the `args` and `kwargs` arguments to the original
-    `target` function INSIDE the closure function).
-
-    All other attributes (`group`, `name`, and `daemon`)
-    are initialized in the parent `threading.Thread` class
-    during the `super().__init__()` call.
-
-
-
-
     NOTE that with release 0.0.7, you can also specify if
     you want the `ThreadWithResult` instance to log when the
     thread starts, ends, and how long the thread takes to execute!
 
 
     If you want to mute logging this message to the terminal for all
     `ThreadWithResult` instances, set the
@@ -158,36 +129,92 @@
       - class attributes vs instance attributes in python
       - scope resolution using the LEGB rule for python
 
     Also note, by default the `log_thread_status`
     class attribute is set to `True`, and the `log_files`
     class attribute set to `None` - neither attributes
     exist as instance attributes by default!
+
     '''
+
+
+
+
+class _runOverrideThreadWithResult(threading.Thread):
+    __doc__ = _general_documentation
+
+    log_thread_status = True
+    log_files         = None
+
+    def run(self):
+        '''
+        Method representing the thread's activity that is overriden to
+        save the result of a thread (if the thread completes) in the
+        `result` attribute of the instance.
+
+        This is the only change to the functionality of the `run` method.
+        This method still invokes the callable object passed to the object's constructor as the
+        target argument, if any, with sequential and keyword arguments taken
+        from the `args` and `kwargs` arguments, respectively.
+        '''
+        # uses the try/finally blocks for consistency with the CPython implementation:
+        # https://github.com/python/cpython/blob/89ac665891dec1988bedec2ce9b2c4d016502a49/Lib/threading.py#L987
+        log_condition = self.log_thread_status is True or self.log_files is not None
+        try:
+            if self._target is not None:
+                if log_condition: time_time_start, perf_counter_start = _log_start_of_thread(self)
+                self.result                                           = self._target(*self._args, **self._kwargs)
+                if log_condition: _                                   = _log_end_of_thread(self, time_time_start, perf_counter_start)
+        finally:
+            # Avoid a refcycle if the thread is running a function with
+            # an argument that has a member that points to the thread.
+            del self._target, self._args, self._kwargs
+
+
+
+
+
+class ___init__OverrideThreadWithResult(threading.Thread):
+    __doc__ = _general_documentation
+
     log_thread_status = True
     log_files         = None
 
     def __init__(self, group=None, target=None, name=None, args=(), kwargs={}, *, daemon=None):
+        '''
+        IMPLEMENTATION EXPLANATION:
+        We create a closure function inside the __init__ method to run the
+        actual function we want to run on a separate thread, enclose the function passed to
+        `target` - along with the arguments provided to `args` and `kwargs` -
+        inside the closure function, and pass the CLOSURE FUNCTION
+        as the function to the `target` argument in the
+        `super.__init__()` call to `threading.Thread`:
+        super().__init__(group=group, target=closure_function, name=name, daemon=daemon)
+
+        Since the function we want to run on a separate thread is no longer
+        the function passed directly to `threading.Thread` (remember,
+        we pass the closure function instead!), we save the result of
+        the enclosed function to the `self.result` attribute of the
+        instance.
+
+        We use inheritance to initialize this instance with the
+        closure function as the `target` function and no arguments
+        for `args` or `kwargs` (since we pass
+        the `args` and `kwargs` arguments to the original
+        `target` function INSIDE the closure function).
+
+        All other attributes (`group`, `name`, and `daemon`)
+        are initialized in the parent `threading.Thread` class
+        during the `super().__init__()` call.
+        '''
         def closure_function():
             log_condition = self.log_thread_status is True or self.log_files is not None
-            if log_condition:
-                time_start         = time.time()
-                perf_counter_start = self.__time_perf_counter()
-                thread_name        = '[' + threading.current_thread().name + ']'
-                utc_offset         = time.strftime('%z')
-                now                = lambda: datetime.now().isoformat() + utc_offset + ' '
-                message            = now() + thread_name.rjust(12) + ' Starting thread...'
-                self.__log(message)
-            self.result = target(*args, **kwargs)
-            if log_condition:
-                time_end         = time.time()
-                perf_counter_end = self.__time_perf_counter()
-                formatted_perf   = self.__format_perf_counter_info(perf_counter_start, perf_counter_end)
-                message          = now() + thread_name.rjust(12) + ' Finished thread! This thread took ' + str(time_end - time_start) + ' time.time() seconds' + formatted_perf + ' to complete.'
-                self.__log(message)
+            if log_condition: time_time_start, perf_counter_start = _log_start_of_thread(self)
+            self.result                                           = target(*args, **kwargs)
+            if log_condition: _                                   = _log_end_of_thread(self, time_time_start, perf_counter_start)
         if sys.version_info.major == 3 and sys.version_info.minor >= 10:
             # commit 98c16c991d6e70a48f4280a7cd464d807bdd9f2b in the cpython repository starts adding
             # the function name of the `target` argument to the thread name:
             #     *name* is the thread name. By default, a unique name is constructed
             #     of the form "Thread-*N*" where *N* is a small decimal number,
             #     or "Thread-*N* (target)" where "target" is ``target.__name__`` if the
             #     *target* argument is specified BUT the *name* argument is omitted.
@@ -204,56 +231,107 @@
             #     - https://github.com/python/cpython/pull/22357
             #     - https://github.com/python/cpython/issues/85999
             #     - https://bugs.python.org/issue41833
             if name is None and target is not None:
                 closure_function.__name__ = self.__class__.__name__ + '.' + 'closure_function' + '(' + str(target.__name__) + ')'
         super().__init__(group=group, target=closure_function, name=name, daemon=daemon)
 
-    def __log(self, message):
-        '''
-        Helper function to print when the thread
-        starts, ends, and how long the thread takes to execute.
 
-        This function runs and prints the thread information to the
-        terminal when any of the following statements are true:
-          * the instance attribute `log_thread_status` is `True`
-          * the instance attribute `log_thread_status` is unset but
-               the class attribute `log_thread_status` is `True`
-          * the instance attribute `log_files` is
-            an iterable object containing objects that support the .write() method
-          * the instance attribute `log_files` is unset but
-               the class attribute is an iterable object containing objects that support the .write() method
-
-        This function also logs the information to every location in
-        `log_files` in addition to printing the thread information
-        to the terminal if the instance or class attribute `log_files` is an
-        iterable object containing objects that support the .write() method.
-        '''
-        if self.log_files is not None:
-            try:
-                for file in self.log_files:
-                    try:
-                        file.write(message + '\n')
-                    except AttributeError as error_message:
-                        # example exception:
-                        # AttributeError: 'str' object has no attribute 'write'
-                        print('ERROR! Could not write to ' + str(file) + '. Please make sure that every object in ' + str(self.log_files) + ' supports the .write() method. The exact error was:\n' + str(error_message))
-            except TypeError as error_message:
-                # example exception:
-                # TypeError: 'int' object is not iterable
-                print('ERROR! Could not write to ' + str(self.log_files) + '. Please make sure that the log_files attribute for ' + str(self.__class__.name) + ' is an iterable object containing objects that support the .write() method. The exact error was:\n' + str(error_message))
-        if self.log_thread_status is True:
-            print(message)
-
-
-    # use helper functions for time.perf_counter() since function became available only after python release 3.3
-    @staticmethod
-    def __time_perf_counter():
-        if sys.version_info.major == 3 and sys.version_info.minor >= 3:
-            return time.perf_counter()
-        return None
-
-    @staticmethod
-    def __format_perf_counter_info(perf_counter_start, perf_counter_end):
-        if sys.version_info.major == 3 and sys.version_info.minor >= 3:
-            return ' (' + str(perf_counter_end - perf_counter_start) + ' time.perf_counter() seconds)'
-        return ''
+def _log_start_of_thread(thread_with_result_instance):
+    time_time_start, perf_counter_start = _measure_time()
+    thread_name                         = format_thread_name()
+    formatted_datetime_with_offset      = format_datetime_for_message()
+    message                             = formatted_datetime_with_offset + thread_name + ' Starting thread...'
+    _log(thread_with_result_instance, message)
+    return time_time_start, perf_counter_start
+
+def _log_end_of_thread(thread_with_result_instance, time_time_start, perf_counter_start):
+    time_time_end, perf_counter_end     = _measure_time()
+    thread_name                         = format_thread_name()
+    formatted_time_time                 = str(time_time_end - time_time_start) + ' time.time() seconds'
+    formatted_time_perf_counter         = _format_perf_counter_info(perf_counter_start, perf_counter_end)
+    formatted_datetime_with_offset      = format_datetime_for_message()
+    message                             = formatted_datetime_with_offset + thread_name + ' Finished thread! This thread took ' + formatted_time_time + formatted_time_perf_counter + ' to complete.'
+    _log(thread_with_result_instance, message)
+
+def _measure_time():
+    current_time         = time.time()
+    current_perf_counter = _time_perf_counter()
+    return current_time, current_perf_counter
+
+# use helper function to check if time.perf_counter() can be called since function became available only after python release 3.3
+def _time_perf_counter():
+    if sys.version_info.major == 3 and sys.version_info.minor >= 3:
+        return time.perf_counter()
+    return None
+
+def _format_perf_counter_info(perf_counter_start, perf_counter_end):
+    if sys.version_info.major == 3 and sys.version_info.minor >= 3:
+        return ' (' + str(perf_counter_end - perf_counter_start) + ' time.perf_counter() seconds)'
+    return ''
+
+def format_thread_name():
+    thread_name        = '[' + threading.current_thread().name + ']'
+    return thread_name.rjust(12)
+
+def format_datetime_for_message():
+    utc_offset                     = time.strftime('%z')
+    formatted_datetime_with_offset = datetime.now().isoformat() + utc_offset + ' '
+    return formatted_datetime_with_offset
+
+
+
+def _log(thread_with_result_instance, message):
+    '''
+    Helper function to print when the thread
+    starts, ends, and how long the thread takes to execute.
+
+    This function runs and prints the thread information to the
+    terminal when any of the following statements are true:
+        * the instance attribute `log_thread_status` is `True`
+        * the instance attribute `log_thread_status` is unset but
+            the class attribute `log_thread_status` is `True`
+        * the instance attribute `log_files` is
+        an iterable object containing objects that support the .write() method
+        * the instance attribute `log_files` is unset but
+            the class attribute is an iterable object containing objects that support the .write() method
+
+    This function also logs the information to every location in
+    `log_files` in addition to printing the thread information
+    to the terminal if the instance or class attribute `log_files` is an
+    iterable object containing objects that support the .write() method.
+    '''
+    if thread_with_result_instance.log_files is not None:
+        try:
+            for file in thread_with_result_instance.log_files:
+                try:
+                    file.write(message + '\n')
+                except AttributeError as error_message:
+                    # example exception:
+                    # AttributeError: 'str' object has no attribute 'write'
+                    print('ERROR! Could not write to ' + str(file) + '. Please make sure that every object in ' + str(thread_with_result_instance.log_files) + ' supports the .write() method. The exact error was:\n' + str(error_message))
+        except TypeError as error_message:
+            # example exception:
+            # TypeError: 'int' object is not iterable
+            print('ERROR! Could not write to ' + str(thread_with_result_instance.log_files) + '. Please make sure that the log_files attribute for ' + str(thread_with_result_instance.__class__.name) + ' is an iterable object containing objects that support the .write() method. The exact error was:\n' + str(error_message))
+    if thread_with_result_instance.log_thread_status is True:
+        print(message)
+
+
+
+
+
+
+ThreadWithResult = _runOverrideThreadWithResult
+
+# without the `_runOverrideThreadWithResult` assignment to `ThreadWithResult`:
+#   any existing code already using this module trying to use the new changes in release 0.1.1
+#   would require updating all references to `ThreadWithResult` to either
+#   `_runOverrideThreadWithResult` or `___init__OverrideThreadWithResult`
+# binding `ThreadWithResult` to `_runOverrideThreadWithResult` avoids this problem
+# `ThreadWithResult` can also be bound to `___init__OverrideThreadWithResult` but
+#    `_runOverrideThreadWithResult` is the chosen default since
+#    the threading.Thread class does additional work in the __init__ method,
+#    such as attribute modifications (https://github.com/python/cpython/blob/89ac665891dec1988bedec2ce9b2c4d016502a49/Lib/threading.py#L892)
+#    and private attribute additions (https://github.com/python/cpython/blob/89ac665891dec1988bedec2ce9b2c4d016502a49/Lib/threading.py#L905)
+#    that `___init__OverrideThreadWithResult` does not currently do, and therefore
+#    using `___init__OverrideThreadWithResult` might cause difficult-to-debug bugs
```

### Comparing `save-thread-result-0.1.0/save_thread_result.egg-info/PKG-INFO` & `save-thread-result-0.1.1/save_thread_result.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: save-thread-result
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple subclass wrapper around `threading.Thread` to get the return value from a thread in python. Exact same interface as `threading.Thread`! 🌟 Star this repo if you found it useful! 🌟
 Home-page: https://github.com/slow-but-steady/save-thread-result/tree/main/python
 Author: slow-but-steady
 Author-email: slowbutsteady1234@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/slow-but-steady/save-thread-result/issues
 Project-URL: PyPi Funding, https://donate.pypi.org
@@ -270,15 +270,15 @@
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
-Requires-Python: >=3.0.*, <4
+Requires-Python: >3.0, <4
 Description-Content-Type: text/markdown
 
 # Python API
 
 ## Quickstart
 
 Installing the `save_thread_result` module:
@@ -330,37 +330,37 @@
 
 ## Examples
 
 Dummy example:
 ```
 from save_thread_result import ThreadWithResult
 
-import time, random
+import time, random, threading
 
 
 def function_to_thread(n):
     count = 0
     while count < 3:
-            print(f'Still running thread {n}...')
+            print(f'Still running {threading.current_thread().name}...')
             count +=1
             time.sleep(3)
     result = random.random()
-    print(f'Return value of thread {n} should be: {result}')
+    print(f'Return value of {threading.current_thread().name} should be: {result}')
     return result
 
 
 def main():
     thread1 = ThreadWithResult(target=function_to_thread, args=(1,))
     thread2 = ThreadWithResult(target=function_to_thread, args=(2,))
     thread1.start()
     thread2.start()
     thread1.join()
     thread2.join()
-    print(thread1.result)
-    print(thread2.result)
+    print(f'The `result` attribute of {thread1.name} is: {thread1.result}')
+    print(f'The `result` attribute of {thread2.name} is: {thread2.result}')
 
 main()
 ```
 
 <details>
   <summary><b>More information</b></summary>
```

### Comparing `save-thread-result-0.1.0/setup.py` & `save-thread-result-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # For new projects, the recommended versioning scheme is based on Semantic Versioning, but adopts a different approach to handling pre-releases and build metadata.
     # The essence of semantic versioning is a 3-part MAJOR.MINOR.MAINTENANCE numbering scheme, where the project author increments:
     # 1. MAJOR version when they make incompatible API changes,
     # 2. MINOR version when they add functionality in a backwards-compatible manner, and
     # 3. MAINTENANCE version when they make backwards-compatible bug fixes.
     # Adopting this approach as a project author allows users to make use of “compatible release” specifiers, where name ~= X.Y requires at least release X.Y, but also allows any later release with a matching MAJOR version.
     # Python projects adopting semantic versioning should abide by clauses 1-8 of the Semantic Versioning 2.0.0 specification: https://semver.org/.
-    version                       = '0.1.0',
+    version                       = '0.1.1',
     name                          = 'save-thread-result',
     description                   = 'Simple subclass wrapper around `threading.Thread` to get the return value from a thread in python. Exact same interface as `threading.Thread`! 🌟 Star this repo if you found it useful! 🌟',
     long_description              = long_description,
     long_description_content_type = 'text/markdown',
     url                           = 'https://github.com/slow-but-steady/save-thread-result/tree/main/python',
     author                        = 'slow-but-steady',
     author_email                  = 'slowbutsteady1234@gmail.com',
@@ -310,15 +310,15 @@
     # http://code.nabla.net/doc/setuptools/api/setuptools/setuptools.find_packages.html
     # https://stackoverflow.com/questions/51286928/what-is-where-argument-for-in-setuptools-find-packages
     packages=find_packages(exclude=['*dev*']),
     # packages=find_namespace_packages(include=['ship']),
     # package_dir={'':'src'},
 
 
-    python_requires  = '>=3.0.*, <4',
+    python_requires  = '>3.0, <4',
     install_requires = [],  # Optional
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
 
 
     # If there are data files included in your packages that need to be installed, specify them here.
     # If using Python 2.6 or earlier, then these have to be included in MANIFEST.in as well.
     package_data = {  # Optional
```

