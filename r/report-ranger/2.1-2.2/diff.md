# Comparing `tmp/report_ranger-2.1.tar.gz` & `tmp/report_ranger-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report_ranger-2.1.tar", max compression
+gzip compressed data, was "report_ranger-2.2.tar", max compression
```

## Comparing `report_ranger-2.1.tar` & `report_ranger-2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0      696 2023-05-29 10:02:23.845368 report_ranger-2.1/pyproject.toml
--rwxr-xr-x   0        0        0       33 2021-09-15 13:25:33.000000 report_ranger-2.1/report_ranger/__init__.py
--rwxr-xr-x   0        0        0     1582 2023-05-29 09:44:19.406291 report_ranger-2.1/report_ranger/config.py
--rwxr-xr-x   0        0        0     8812 2023-05-02 03:51:52.380891 report_ranger-2.1/report_ranger/contentassistant.py
--rwxr-xr-x   0        0        0     3806 2023-05-02 06:44:16.057745 report_ranger-2.1/report_ranger/environment.py
--rwxr-xr-x   0        0        0      217 2021-09-15 13:25:33.000000 report_ranger-2.1/report_ranger/errors.py
--rwxr-xr-x   0        0        0    12991 2023-04-13 07:20:23.609912 report_ranger-2.1/report_ranger/helpers.py
--rwxr-xr-x   0        0        0     3034 2023-03-23 05:17:42.138978 report_ranger-2.1/report_ranger/imports/imports.py
--rwxr-xr-x   0        0        0     4473 2023-05-23 22:45:26.028951 report_ranger-2.1/report_ranger/imports/section.py
--rwxr-xr-x   0        0        0    20287 2023-05-23 07:27:07.987448 report_ranger-2.1/report_ranger/imports/vulnerability.py
--rwxr-xr-x   0        0        0     3210 2023-03-23 05:17:42.140109 report_ranger-2.1/report_ranger/markdown_renderer/csvrenderer.py
--rwxr-xr-x   0        0        0     4266 2023-04-28 02:59:32.119136 report_ranger-2.1/report_ranger/markdown_renderer/latexrenderer.py
--rwxr-xr-x   0        0        0     2682 2023-04-29 06:11:16.074523 report_ranger-2.1/report_ranger/markdown_renderer/typstrenderer.py
--rwxr-xr-x   0        0        0     3810 2023-05-23 07:19:00.069356 report_ranger-2.1/report_ranger/output_formatter/csvformatter.py
--rwxr-xr-x   0        0        0     1336 2023-05-23 07:18:57.380497 report_ranger-2.1/report_ranger/output_formatter/docxformatter.py
--rwxr-xr-x   0        0        0     4519 2023-05-23 07:18:54.540800 report_ranger-2.1/report_ranger/output_formatter/htmlformatter.py
--rwxr-xr-x   0        0        0    20061 2023-05-23 07:18:51.519431 report_ranger-2.1/report_ranger/output_formatter/latexformatter.py
--rwxr-xr-x   0        0        0    32470 2023-05-24 01:30:53.846118 report_ranger-2.1/report_ranger/output_formatter/outputformatter.py
--rwxr-xr-x   0        0        0     5764 2023-05-23 07:19:04.716847 report_ranger-2.1/report_ranger/output_formatter/typstformatter.py
--rwxr-xr-x   0        0        0    11488 2023-05-24 01:37:48.702425 report_ranger-2.1/report_ranger/report.py
--rwxr-xr-x   0        0        0     9434 2023-05-29 09:44:01.878256 report_ranger-2.1/report_ranger/report_ranger.py
--rwxr-xr-x   0        0        0     8290 2023-03-23 05:17:42.147623 report_ranger-2.1/report_ranger/riskassessment.py
--rwxr-xr-x   0        0        0     3019 2022-05-27 05:01:58.000000 report_ranger-2.1/report_ranger/styles.py
--rwxr-xr-x   0        0        0    19313 2023-03-23 05:17:42.148620 report_ranger-2.1/report_ranger/table.py
--rwxr-xr-x   0        0        0     1442 2023-05-02 06:37:25.929867 report_ranger-2.1/report_ranger/template.py
--rwxr-xr-x   0        0        0     2119 2023-03-23 05:17:42.150976 report_ranger-2.1/report_ranger/templatemapper.py
--rwxr-xr-x   0        0        0      555 2023-04-28 02:54:06.713280 report_ranger-2.1/report_ranger/utils/jinja_helpers.py
--rwxr-xr-x   0        0        0    20774 2023-05-24 08:00:56.417779 report_ranger-2.1/report_ranger/utils/mdread.py
--rwxr-xr-x   0        0        0     1138 2022-05-27 05:01:58.000000 report_ranger-2.1/report_ranger/validation.py
--rwxr-xr-x   0        0        0     2833 2023-05-23 22:43:39.663890 report_ranger-2.1/report_ranger/watcher.py
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 report_ranger-2.1/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 report_ranger-2.1/PKG-INFO
+-rwxr-xr-x   0        0        0      696 2023-05-30 01:32:13.781120 report_ranger-2.2/pyproject.toml
+-rwxr-xr-x   0        0        0       33 2021-09-15 13:25:33.000000 report_ranger-2.2/report_ranger/__init__.py
+-rwxr-xr-x   0        0        0     1542 2023-05-30 01:05:33.767221 report_ranger-2.2/report_ranger/config.py
+-rwxr-xr-x   0        0        0     8812 2023-05-02 03:51:52.380891 report_ranger-2.2/report_ranger/contentassistant.py
+-rwxr-xr-x   0        0        0     3806 2023-05-02 06:44:16.057745 report_ranger-2.2/report_ranger/environment.py
+-rwxr-xr-x   0        0        0      217 2021-09-15 13:25:33.000000 report_ranger-2.2/report_ranger/errors.py
+-rwxr-xr-x   0        0        0    12991 2023-04-13 07:20:23.609912 report_ranger-2.2/report_ranger/helpers.py
+-rwxr-xr-x   0        0        0     3034 2023-03-23 05:17:42.138978 report_ranger-2.2/report_ranger/imports/imports.py
+-rwxr-xr-x   0        0        0     4473 2023-05-23 22:45:26.028951 report_ranger-2.2/report_ranger/imports/section.py
+-rwxr-xr-x   0        0        0    20761 2023-05-30 01:13:38.343243 report_ranger-2.2/report_ranger/imports/vulnerability.py
+-rwxr-xr-x   0        0        0     3210 2023-03-23 05:17:42.140109 report_ranger-2.2/report_ranger/markdown_renderer/csvrenderer.py
+-rwxr-xr-x   0        0        0     4266 2023-04-28 02:59:32.119136 report_ranger-2.2/report_ranger/markdown_renderer/latexrenderer.py
+-rwxr-xr-x   0        0        0     2682 2023-04-29 06:11:16.074523 report_ranger-2.2/report_ranger/markdown_renderer/typstrenderer.py
+-rwxr-xr-x   0        0        0     3810 2023-05-23 07:19:00.069356 report_ranger-2.2/report_ranger/output_formatter/csvformatter.py
+-rwxr-xr-x   0        0        0     1336 2023-05-23 07:18:57.380497 report_ranger-2.2/report_ranger/output_formatter/docxformatter.py
+-rwxr-xr-x   0        0        0     4519 2023-05-23 07:18:54.540800 report_ranger-2.2/report_ranger/output_formatter/htmlformatter.py
+-rwxr-xr-x   0        0        0    20061 2023-05-23 07:18:51.519431 report_ranger-2.2/report_ranger/output_formatter/latexformatter.py
+-rwxr-xr-x   0        0        0    33026 2023-05-30 01:22:34.176985 report_ranger-2.2/report_ranger/output_formatter/outputformatter.py
+-rwxr-xr-x   0        0        0     5764 2023-05-23 07:19:04.716847 report_ranger-2.2/report_ranger/output_formatter/typstformatter.py
+-rwxr-xr-x   0        0        0    11958 2023-05-30 01:05:33.769221 report_ranger-2.2/report_ranger/report.py
+-rwxr-xr-x   0        0        0     9722 2023-05-30 01:30:18.770785 report_ranger-2.2/report_ranger/report_ranger.py
+-rwxr-xr-x   0        0        0     8290 2023-03-23 05:17:42.147623 report_ranger-2.2/report_ranger/riskassessment.py
+-rwxr-xr-x   0        0        0     3019 2022-05-27 05:01:58.000000 report_ranger-2.2/report_ranger/styles.py
+-rwxr-xr-x   0        0        0    19313 2023-03-23 05:17:42.148620 report_ranger-2.2/report_ranger/table.py
+-rwxr-xr-x   0        0        0     1442 2023-05-30 00:59:09.589466 report_ranger-2.2/report_ranger/template.py
+-rwxr-xr-x   0        0        0     2119 2023-03-23 05:17:42.150976 report_ranger-2.2/report_ranger/templatemapper.py
+-rwxr-xr-x   0        0        0      555 2023-04-28 02:54:06.713280 report_ranger-2.2/report_ranger/utils/jinja_helpers.py
+-rwxr-xr-x   0        0        0    21313 2023-05-30 01:29:21.109099 report_ranger-2.2/report_ranger/utils/mdread.py
+-rwxr-xr-x   0        0        0     1138 2022-05-27 05:01:58.000000 report_ranger-2.2/report_ranger/validation.py
+-rwxr-xr-x   0        0        0     2833 2023-05-23 22:43:39.663890 report_ranger-2.2/report_ranger/watcher.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 report_ranger-2.2/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 report_ranger-2.2/PKG-INFO
```

### Comparing `report_ranger-2.1/pyproject.toml` & `report_ranger-2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Report-Ranger"
-version = "2.1"
+version = "2.2"
 description = "Create a report using markdown files."
 license = "MIT"
 authors = ["Matthew Strahan <matt@volkis.com.au>"]
 repository = "https://gitlab.com/volkis/report-ranger/"
 documentation = "https://gitlab.com/volkis/report-ranger/-/wikis/home"
 packages = [
     { include = "report_ranger" }
```

### Comparing `report_ranger-2.1/report_ranger/config.py` & `report_ranger-2.2/report_ranger/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     'RR_INPUT_FILE': 'default_input_file'
 }
 
 def get_config_from_file(file):
     try:
         with open(file, 'r') as vf:
             config = yaml.safe_load(vf)
-            log.info(f"Processing file {file}")
+            log.info(f"Processing config file {file}")
             return config
     except:
         log.info(f"Could not open config file {file}")
         return {}
 
 def get_config(arg_file = None):
     final_config = copy.copy(config)
@@ -48,10 +48,9 @@
         var = os.getenv(envvar)
         if var != None:
             final_config[envvars[envvar]] = var
     
     for config_location in [user_config_dir('reportranger', 'Volkis') + '/config.yml', 'config.yml', arg_file]:
         if config_location:
             final_config.update(get_config_from_file(config_location))
-    log.info(f"Final config: {final_config}")
     return final_config
```

### Comparing `report_ranger-2.1/report_ranger/contentassistant.py` & `report_ranger-2.2/report_ranger/contentassistant.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/environment.py` & `report_ranger-2.2/report_ranger/environment.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/helpers.py` & `report_ranger-2.2/report_ranger/helpers.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/imports/imports.py` & `report_ranger-2.2/report_ranger/imports/imports.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/imports/section.py` & `report_ranger-2.2/report_ranger/imports/section.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/imports/vulnerability.py` & `report_ranger-2.2/report_ranger/imports/vulnerability.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 from report_ranger.helpers import make_list
 
 log = logging.getLogger(__name__)
 
 
 def vuln_from_file(file_loc, riskassessment, env=None, vulnerability_validation={}, scope=None, watcher=None):
     ''' Get the vulnerability markdown from a file, process the headers and make sure they're there. Return a Vulnerability object.'''
-    log.debug("Loading vulnerability file {}".format(file_loc))
-
-    headers, vulnmarkdown = markdown_from_file(file_loc, env=env, watcher=watcher)
+    log.debug(f"Loading vulnerability file {file_loc}")
+    try:
+        headers, vulnmarkdown = markdown_from_file(file_loc, env=env, watcher=watcher)
+    except:
+        log.warn(f"Could not read vulnerability file {file_loc}")
 
     if 'name' in headers:
         if not isinstance(headers['name'], str):
-            log.warn("Vulnerability name not a string for file {}".format(file_loc))
+            log.warn(f"Vulnerability name not a string for file {file_loc}")
             name = file_loc
             headers['name'] = file_loc
         else:
             name = headers['name']
     elif 'Name' in headers:  # This is for legacy reasons, it used to be case insensitive so we still accept "Name"
         name = headers['Name']
         headers['name'] = headers['Name']
@@ -83,16 +85,19 @@
                 log.info(
                     "* New vulnerability scope in directory '{}'".format((os.path.join(vulndir, f))))
                 vdir = os.path.join(vulndir, f)
                 for v in os.listdir(vdir):
                     if v == "template.md" or v == "template.md.rr":
                         continue
                     if v == "introduction.md" or v == "introduction.md.rr":
-                        scopeintroductions[f] = markdown_from_file(
-                            os.path.join(vdir, v), env=env, watcher=watcher)
+                        try:
+                            scopeintroductions[f] = markdown_from_file(
+                                os.path.join(vdir, v), env=env, watcher=watcher)
+                        except:
+                            log.warn(f"Could not read introduction file {v} in vulnerability directory {vdir}")
                         continue
                     fn, ext = os.path.splitext(v)
                     if ext == ".md" or ext == ".rr":  # Only process markdown files
                         filename = os.path.join(vdir, v)
                         log.info(
                             "  - Reading vulnerability file '{}'".format(filename))
                         try:
@@ -107,22 +112,26 @@
                             log.error(
                                 "Removing markdown for vulnerability {}".format(self.name))
                             self.markdown = ""
             else:  # It's a file
                 if f == "template.md" or f == "template.md.rr":
                     continue
                 if f == "introduction.md" or f == "introduction.md.rr":
-                    scopeintroduction = markdown_from_file(
-                        os.path.join(vulndir, f), env=env, watcher=watcher)
-                    if "scope" in scopeintroduction[0]:
-                        # There's a scope defined in the headers of the introduction
-                        scopeintroductions[f] = scopeintroduction
-                    else:
-                        scopeintroductions[''] = scopeintroduction
+                    try:
+                        scopeintroduction = markdown_from_file(
+                            os.path.join(vulndir, f), env=env, watcher=watcher)
+                        if "scope" in scopeintroduction[0]:
+                            # There's a scope defined in the headers of the introduction
+                            scopeintroductions[f] = scopeintroduction
+                        else:
+                            scopeintroductions[''] = scopeintroduction
+                    except:
+                        log.warn(f"Could not read introduction file {v} in vulnerability directory {vdir}")
                     continue
+                    
                 log.info(
                     "* Reading vulnerability file '{}'".format(os.path.join(vulndir, f)))
                 fn, ext = os.path.splitext(f)
                 if ext == ".md" or ext == ".rr":  # Only process markdown files
                     try:
                         vulnerabilities += [vuln_from_file(
                             os.path.join(vulndir, f), riskassessment=riskassessment, env=env, watcher=watcher)]
```

### Comparing `report_ranger-2.1/report_ranger/markdown_renderer/csvrenderer.py` & `report_ranger-2.2/report_ranger/markdown_renderer/csvrenderer.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/markdown_renderer/latexrenderer.py` & `report_ranger-2.2/report_ranger/markdown_renderer/latexrenderer.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/markdown_renderer/typstrenderer.py` & `report_ranger-2.2/report_ranger/markdown_renderer/typstrenderer.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/output_formatter/csvformatter.py` & `report_ranger-2.2/report_ranger/output_formatter/csvformatter.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/output_formatter/docxformatter.py` & `report_ranger-2.2/report_ranger/output_formatter/docxformatter.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/output_formatter/htmlformatter.py` & `report_ranger-2.2/report_ranger/output_formatter/htmlformatter.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/output_formatter/latexformatter.py` & `report_ranger-2.2/report_ranger/output_formatter/latexformatter.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/output_formatter/outputformatter.py` & `report_ranger-2.2/report_ranger/output_formatter/outputformatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import plotly.express as px
 from pathlib import Path
 from report_ranger.environment import Environment
 from tabulate import tabulate
 from report_ranger.imports.imports import import_csv, import_xlsx
 import traceback
 import logging
+import ipaddress
 from report_ranger.styles import TableStyles, ColorList, test_color
 from report_ranger.imports.section import Section
 import plotly.io as pio
 import plotly.graph_objects as go
 from report_ranger.helpers import table_aggregate, table_aggregate_value, filter_rows, table_to_dict, tables_outer_join, table_separate_column, table_add_row, table_separate_column_groups, sort_table, separate_sequences
 
 # Mathjax fix for plotly
@@ -36,24 +37,14 @@
     'c': 'tclosed',
     'cb': 'tclosedbold',
     'O': 'topenbold',
     'ob': 'topenbold',
     'b': 'bold'
 }
 
-
-# For sorting IP addresses
-def split_ip(ip):
-    """Split a IP address given as string into a 4-tuple of integers."""
-    return tuple(int(part) for part in ip.split('.'))
-
-def sort_ips(item):
-    ''' Helper function for sorting IPs, used as key in sorted function. '''
-    return split_ip(item)
-
 def oxfordcomma(listed):
     if len(listed) == 0:
         return ''
     if len(listed) == 1:
         return listed[0]
     if len(listed) == 2:
         return listed[0] + ' and ' + listed[1]
@@ -64,14 +55,18 @@
     def __init__(self, templateheaders=dict(), timer=None, watcher=None):
         self.templateheaders = templateheaders
         self.figformat = "png"
         self.watcher=watcher
         log.info(f"watcher is {watcher}")
 
         self.timer = timer
+        self.watcher=watcher
+        log.info(f"watcher is {watcher}")
+
+        self.timer = timer
 
         self.timer = timer
 
         # Initial filling in the environment
         log.info(f"{self.time()}: Initialising new environment for output formatter")
         env = Environment()
         env.set_static('file_exists', self.file_exists)
@@ -215,20 +210,37 @@
         return newsection.get_chapters(self.env)
 
     def iplist(self, listofips, heading="IP list", columns=4):
         '''Build a table from a list of IPs. Automatically format based on number of columns and sort IPs into order.'''
 
         log.debug("iplist(): Building IP list")
 
-        try:
-            sortedips = sorted(listofips, key=sort_ips)
-        except Exception as e:
-            log.warn(
-                "IP list failed sorting, just leaving it unsorted: {}".format(e.args))
-            sortedips = listofips
+        # Separate IPv4 and IPv6 addresses
+        ipv4_nets = []
+        ipv6_nets = []
+
+        for _ip in listofips:
+            try:
+                ip_net = ipaddress.ip_network(_ip)
+                if ip_net.version == 4:
+                    ipv4_nets.append(ip_net)
+                else:
+                    ipv6_nets.append(ip_net)
+            except Exception as e:
+                log.warn(
+                    "Invalid IP address or subnet: {}. Error: {}".format(_ip,e))
+
+        # Collapse and sort IPv4 and IPv6 addresses separately
+        sorted_ipv4_nets = list(ipaddress.collapse_addresses(ipv4_nets))
+        sorted_ipv6_nets = list(ipaddress.collapse_addresses(ipv6_nets))
+
+        # Combine sorted lists
+        sorted_nets = sorted_ipv4_nets + sorted_ipv6_nets
+
+        sortedips = [str(net) for net in sorted_nets]
 
         if(len(sortedips) < columns):
             columns = len(sortedips)
 
         iptable = [[heading]]
         for i in range(len(sortedips)):
             row = int(i / columns) + 1
@@ -464,17 +476,21 @@
             return ''
 
     def include_file(self, file_loc, include_headers=True, custom_headers=None):
         """ Process the file, template it, and return just the markdown """
         fn, ext = os.path.splitext(file_loc)
         if ext != ".md" and ext != ".rr":
             return ""
-        headers, markdown = markdown_from_file(file_loc, env=self.env, watcher=self.watcher)
-        headers['cwd'] = os.path.dirname(
-            os.path.join(os.path.curdir, file_loc))
+        try:
+            headers, markdown = markdown_from_file(file_loc, env=self.env, watcher=self.watcher)
+            headers['cwd'] = os.path.dirname(
+                os.path.join(os.path.curdir, file_loc))
+        except:
+            log.warn(f"Could not read included file {file_loc}")
+            return ""
 
         if not include_headers:
             headers = {}
 
         if custom_headers != None:
             headers.update(custom_headers)
```

### Comparing `report_ranger-2.1/report_ranger/output_formatter/typstformatter.py` & `report_ranger-2.2/report_ranger/output_formatter/typstformatter.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/report.py` & `report_ranger-2.2/report_ranger/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,20 @@
             try:
                 self.template = retrieve_template(default_template, templatemapper)
                 log.info("Adding default template")
                 retrieved_template = True
             except Exception as e:
                 log.warning(f"Default template cannot be loaded ({e.args}): {default_template}")
 
+        if self.template == None:
+            log.warn("Could not figure out a template. Please set a template with the '-t' flag.")
+            log.warn("Alternatively, use a config file. If you want to know where config files can be then use the '-v' flag and it will tell you.")
+            log.warn("Configuration files are YAML, so you need to put in `template: template_location` in the config file.")
+            raise Exception("Could not find template")
+
         log.info(f"{self.timer.time()}: Finished report init")
 
     # If the "change_template" header is there the report can set its own template variables
     def _change_template_headers(self, templateheaders, reportheaders):
         if 'change_template' in reportheaders:
             log.info("change_template header detected")
             if not isinstance(reportheaders['change_template'], dict):
```

### Comparing `report_ranger-2.1/report_ranger/report_ranger.py` & `report_ranger-2.2/report_ranger/report_ranger.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,21 @@
     else:
         logging.basicConfig(format='%(levelname)s: %(message)s',
                             level=logging.WARNING)
 
     config = get_config(args.config)
 
     input = args.input if args.input else config['default_input_file'] if 'default_input_file' in config else None
-    if input == None:
-        raise Exception("Could not figure out an input file")
+    if input == None or input == '':
+        log.warn("Report Ranger needs a file as input. Please use the -i flag to set an input file.")
+        return
     output_file = args.output if args.output else config['default_output_file'] if 'default_output_file' in config else None
     if output_file == None:
-        raise Exception("Could not figure out an output file")
+        log.warn("Report Ranger needs a file as output. Please use the -o flag to set an output file. Set the output file as '-' to output to stdout.")
+        return
 
     parentdir = os.path.dirname(os.path.join(os.path.curdir, input))
 
     # We need to change the current working directory to the directory of the template otherwise relative
     # paths inside the template won't work. For instance you won't be able to include executivesummary.md
     rr_parent_folder = os.path.abspath(os.path.curdir)
 
@@ -77,20 +79,24 @@
     else:
         templatefile = ''
 
     os.chdir(parentdir)
     parentdir = '.'
     mdfile = os.path.basename(input)
 
-    # Get the template
-    report = Report(
-        mdfile,
-        templatefile=templatefile,
-        templatemapper=templatemapper,
-        default_template=config['default_template'])
+    # Initialise the report
+    try:
+        report = Report(
+            mdfile,
+            templatefile=templatefile,
+            templatemapper=templatemapper,
+            default_template=config['default_template'])
+    except:
+        log.warn("Could not initialise report.")
+        return
 
     # Get the extension of the output file
     if output_file:
         fn, ext = os.path.splitext(output_file)
     else:
         ext = 'md'
 
@@ -153,15 +159,14 @@
         os.symlink('/dev/stdout', stdout_link)
         output_file = stdout_link
 
     # Convert output file path into full path if relative path is given
     if output_file and output_file[0] != '/':
         output_file = os.path.join(rr_parent_folder, output_file)
 
-
     if args.watch:
         log.info("Starting watch")
         try:
             watcher = Watcher(log.info, "Callback")
             watcher.set_callback(report.process_file, mdfile, target, docformat, output_file, default_output_file=config.get('default_output_file'), watcher=watcher)
             watcher.set_watch_mode(args.watch_mode)
             output = report.process_file(mdfile, target, docformat, output_file, default_output_file=config.get('default_output_file'), watcher=watcher)
```

### Comparing `report_ranger-2.1/report_ranger/riskassessment.py` & `report_ranger-2.2/report_ranger/riskassessment.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/styles.py` & `report_ranger-2.2/report_ranger/styles.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/table.py` & `report_ranger-2.2/report_ranger/table.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/template.py` & `report_ranger-2.2/report_ranger/template.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/templatemapper.py` & `report_ranger-2.2/report_ranger/templatemapper.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/utils/jinja_helpers.py` & `report_ranger-2.2/report_ranger/utils/jinja_helpers.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/utils/mdread.py` & `report_ranger-2.2/report_ranger/utils/mdread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import copy
+import copy
 from report_ranger.errors import InputError
 import os
 from pathlib import Path
 import re
 from jinja2 import Template
 import jinja2
 from jinja2.runtime import Macro
+from jinja2.runtime import Macro
 import yaml
 import json
 from report_ranger.imports.imports import import_csv, import_xlsx
 import logging
 from report_ranger.imports import section
 from report_ranger.helpers import make_list
 from report_ranger.imports import vulnerability
@@ -289,15 +291,19 @@
                     continue
                 try:
                     macrofile = _get_resultant_path(macrofile, includemapper, pathlist)
                 except:
                     log.warn(f"Could not find {macrofile}")
                     continue
 
-                mdheaders, markdown = markdown_from_file(macrofile, env=env, watcher=watcher)
+                try:
+                    mdheaders, markdown = markdown_from_file(macrofile, env=env, watcher=watcher)
+                except:
+                    log.warn(f"Could not read macro file {macrofile}")
+                    continue
                 mdheaders['cwd'] = os.path.dirname(
                     os.path.join(os.path.curdir, macrofile))
 
                 try:
                     jenv = jinja2.Environment()
                     # Add in the env to the globals. We want the existing globals to take precedence
                     globals = env.get_env()
@@ -338,21 +344,26 @@
     Arguments:
     - file_loc: The location of the file to read
     - env: The environment in its current context. The stack for this environment will be extended.
     - process_includes: Whether or not to process the include header, allowing the including of headers and markdown from other files.
     - process_imports: Whether or not to process the import header, allowing importing of sections, vulns, csv and xlsx files.
     - watcher: if a watcher is configured then add_path will automatically be called
     
+    - watcher: if a watcher is configured then add_path will automatically be called
+    
     Returns (headers, markdown) where headers is a dict and markdown is a long string """
 
     log.debug(f"Reading markdown from file {file_loc}")
 
     if not os.path.exists(file_loc):
         log.warn(f"Trying to read file {file_loc} but it doesn't exist")
-        return dict(), ""
+        raise InputError("Could not read markdown file.")
+
+    if watcher:
+        watcher.add_path(file_loc)
 
     if watcher:
         watcher.add_path(file_loc)
 
     with open(file_loc, 'r') as vf:
         # If the first line starts with "---" that's our headers We have to make sure that it starts with "---"
         firstline = vf.readline()
@@ -421,15 +432,19 @@
 
     for f in os.listdir(dir_loc):
         mdfile = os.path.join(dir_loc, f)
         if os.path.isfile(mdfile):
             dir, filename = os.path.split(mdfile)
             fn, ext = os.path.splitext(filename)
             if ext == ".md" or ext == ".rr":
-                mdfromfile=markdown_from_file(mdfile, env, watcher=watcher)
-                mdfromfile[0]["filename"] = filename
-                mdfromfile[0]["filename_noext"] = fn
-                mdfromfile[0]["filename_full"] = mdfile
-                files.extend([mdfromfile])
+                try:
+                    mdfromfile=markdown_from_file(mdfile, env, watcher=watcher)
+                    mdfromfile[0]["filename"] = filename
+                    mdfromfile[0]["filename_noext"] = fn
+                    mdfromfile[0]["filename_full"] = mdfile
+                    files.extend([mdfromfile])
+                except:
+                    log.warn(f"Could not read file {mdfile}")
+                    continue
                 
 
     return files
```

### Comparing `report_ranger-2.1/report_ranger/validation.py` & `report_ranger-2.2/report_ranger/validation.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/report_ranger/watcher.py` & `report_ranger-2.2/report_ranger/watcher.py`

 * *Files identical despite different names*

### Comparing `report_ranger-2.1/setup.py` & `report_ranger-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'watchdog']
 
 entry_points = \
 {'console_scripts': ['reportranger = report_ranger:main']}
 
 setup_kwargs = {
     'name': 'report-ranger',
-    'version': '2.1',
+    'version': '2.2',
     'description': 'Create a report using markdown files.',
     'long_description': 'None',
     'author': 'Matthew Strahan',
     'author_email': 'matt@volkis.com.au',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/volkis/report-ranger/',
```

### Comparing `report_ranger-2.1/PKG-INFO` & `report_ranger-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-ranger
-Version: 2.1
+Version: 2.2
 Summary: Create a report using markdown files.
 Home-page: https://gitlab.com/volkis/report-ranger/
 License: MIT
 Author: Matthew Strahan
 Author-email: matt@volkis.com.au
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

