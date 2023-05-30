# Comparing `tmp/serialdatalog-0.1.0.tar.gz` & `tmp/serialdatalog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialdatalog-0.1.0.tar", max compression
+gzip compressed data, was "serialdatalog-0.1.2.tar", max compression
```

## Comparing `serialdatalog-0.1.0.tar` & `serialdatalog-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      927 2023-04-25 12:56:01.513302 serialdatalog-0.1.0/README.md
--rw-r--r--   0        0        0      364 2023-04-25 12:57:30.646633 serialdatalog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.0/serialdatalog/__init__.py
--rw-r--r--   0        0        0     5328 2023-04-25 12:55:57.633302 serialdatalog-0.1.0/serialdatalog/datalog.py
--rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 serialdatalog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-04-25 12:59:02.329965 serialdatalog-0.1.2/README.md
+-rw-r--r--   0        0        0      364 2023-05-30 13:26:58.712423 serialdatalog-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-25 12:48:30.669977 serialdatalog-0.1.2/serialdatalog/__init__.py
+-rw-r--r--   0        0        0     5583 2023-05-30 13:26:34.445304 serialdatalog-0.1.2/serialdatalog/datalog.py
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 serialdatalog-0.1.2/PKG-INFO
```

### Comparing `serialdatalog-0.1.0/README.md` & `serialdatalog-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Serial Data Logger
 
-A simple python script that logs the input received from a serial (USB) input to an SQLite database along with logging the time stamp (in the format YYMMDDHHMMSS) of the received message.
+A simple python script that logs the input received from a serial (USB) input to an SQLite database along with logging the time stamp (in the format `YYMMDDHHMMSS`) of the received message.
 Serial data logger expects the serial inputs to be comma separated.
 
+## Install
+
+```
+pip install serialdatalog
+```
+
 ## Usage
 
 Here's an example using a Finometer pressure sensor.
 
 ```python
 import logging
 import serialdatalog as sdl
```

### Comparing `serialdatalog-0.1.0/serialdatalog/datalog.py` & `serialdatalog-0.1.2/serialdatalog/datalog.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,31 +9,33 @@
 import logging
 from datetime import datetime
 
 # Console logger
 clogger = logging.getLogger(__name__)
 def logger(
         table_dict,
-        source="/dev/ttyACM0",
-        dest="datalog.sqlite3",
+        source="/dev/ttyACM0", dest="datalog.sqlite3",
         encoding='utf-8',
-        timeout=10
+        timeout=10,
+        rtn_results=False,
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
+        rtn_results (bool, optional) : If True, will yield each successful line.
+            If False, will not yield anything.
 
     Returns:
         return val (bool) : True if successful. False otherwise.
     """
 
     # Connects to source
     with serial.Serial(source, timeout=timeout) as ser:
@@ -52,22 +54,23 @@
                     clogger.info(line)
                     line = line.rstrip().split(",")
                     line.append(datetime.now().strftime('%y%m%d%H%M%S'))
                     data_dict = {
                         h : liteval(line[i]) for i, h in enumerate(list(table_dict.keys()))
                     }
                     add_to_database(con, data_dict, table_name)
-                except IndexError:
-                    print("Index Error")
-                    pass
-                except UnicodeDecodeError:
-                    print("UnicodeDecodeError")
-                    pass
-                except KeyboardInterrupt:
-                    break
+                    yield data_dict
+                except IndexError as error:
+                    clogger.debug(error)
+                except SyntaxError as error:
+                    clogger.debug(error)
+                except UnicodeDecodeError as error:
+                    clogger.debug(error)
+                except KeyboardInterrupt as error:
+                    clogger.debug(error)
     clogger.info("Finished reading data.")
     return True
 
 def connect_to_database(database):
     """Connects to the SQLite database.
 
     Args:
```

### Comparing `serialdatalog-0.1.0/PKG-INFO` & `serialdatalog-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: serialdatalog
-Version: 0.1.0
+Version: 0.1.2
 Summary: Logs data coming from a serial port
 Author: Alex
 Author-email: adrysdale@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyserial (>=3.5,<4.0)
 Description-Content-Type: text/markdown
 
 # Serial Data Logger
 
-A simple python script that logs the input received from a serial (USB) input to an SQLite database along with logging the time stamp (in the format YYMMDDHHMMSS) of the received message.
+A simple python script that logs the input received from a serial (USB) input to an SQLite database along with logging the time stamp (in the format `YYMMDDHHMMSS`) of the received message.
 Serial data logger expects the serial inputs to be comma separated.
 
+## Install
+
+```
+pip install serialdatalog
+```
+
 ## Usage
 
 Here's an example using a Finometer pressure sensor.
 
 ```python
 import logging
 import serialdatalog as sdl
```

