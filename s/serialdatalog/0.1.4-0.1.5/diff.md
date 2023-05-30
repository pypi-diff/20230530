# Comparing `tmp/serialdatalog-0.1.4.tar.gz` & `tmp/serialdatalog-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialdatalog-0.1.4.tar", max compression
+gzip compressed data, was "serialdatalog-0.1.5.tar", max compression
```

## Comparing `serialdatalog-0.1.4.tar` & `serialdatalog-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      976 2023-04-25 12:59:02.329965 serialdatalog-0.1.4/README.md
--rw-r--r--   0        0        0      364 2023-05-30 20:52:27.707201 serialdatalog-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.4/serialdatalog/__init__.py
--rw-r--r--   0        0        0     5631 2023-05-30 20:38:31.011039 serialdatalog-0.1.4/serialdatalog/datalog.py
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 serialdatalog-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-04-25 12:59:02.329965 serialdatalog-0.1.5/README.md
+-rw-r--r--   0        0        0      364 2023-05-30 21:01:24.762753 serialdatalog-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.5/serialdatalog/__init__.py
+-rw-r--r--   0        0        0     5401 2023-05-30 21:01:19.519333 serialdatalog-0.1.5/serialdatalog/datalog.py
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 serialdatalog-0.1.5/PKG-INFO
```

### Comparing `serialdatalog-0.1.4/README.md` & `serialdatalog-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `serialdatalog-0.1.4/serialdatalog/datalog.py` & `serialdatalog-0.1.5/serialdatalog/datalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,30 +13,27 @@
 clogger = logging.getLogger(__name__)
 def logger(
         table_dict,
         source="/dev/ttyACM0",
         dest="datalog.sqlite3",
         encoding='utf-8',
         timeout=10,
-        rtn_results=False,
     ):
     """Logs serial readings
 
     Args:
         table_dict (dict) : A dictionary containing the "table header" : "data type".
         source (string, optional) : Source port of the serial device.
             Defaults to "/dev/ttyACM0".
         dest (string, optional) : Destination database to write serial output to.
             Defaults to 'datalog.db'
         encoding (string, optional) : Encoding of serial device. 
             Defaults to 'utf-8'.
         timeout (float, optional) : Timeout for reading from the serial port.
             Defaults to 10.
-        rtn_results (bool, optional) : If True, will yield each successful line.
-            If False, will not yield anything.
 
     Returns:
         return val (bool) : True if successful. False otherwise.
     """
 
     # Connects to source
     with serial.Serial(source, timeout=timeout) as ser:
@@ -55,16 +52,15 @@
                     clogger.info(line)
                     line = line.rstrip().split(",")
                     line.append(datetime.now().strftime('%y%m%d%H%M%S'))
                     data_dict = {
                         h : liteval(line[i]) for i, h in enumerate(list(table_dict.keys()))
                     }
                     add_to_database(con, data_dict, table_name)
-                    if rtn_results:
-                        yield data_dict
+
                 except IndexError as error:
                     clogger.debug(error)
                 except SyntaxError as error:
                     clogger.debug(error)
                 except UnicodeDecodeError as error:
                     clogger.debug(error)
                 except KeyboardInterrupt as error:
```

### Comparing `serialdatalog-0.1.4/PKG-INFO` & `serialdatalog-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialdatalog
-Version: 0.1.4
+Version: 0.1.5
 Summary: Logs data coming from a serial port
 Author: Alex
 Author-email: adrysdale@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

