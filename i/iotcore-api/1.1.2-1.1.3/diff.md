# Comparing `tmp/iotcore_api-1.1.2.tar.gz` & `tmp/iotcore_api-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotcore_api-1.1.2.tar", max compression
+gzip compressed data, was "iotcore_api-1.1.3.tar", max compression
```

## Comparing `iotcore_api-1.1.2.tar` & `iotcore_api-1.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.2/iotcoreapi/__init__.py
--rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.2/iotcoreapi/exceptions.py
--rw-r--r--   0        0        0    56483 2023-05-29 14:54:04.396063 iotcore_api-1.1.2/iotcoreapi/iotcoreapi.py
--rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.2/iotcoreapi/nan_treatment.py
--rw-r--r--   0        0        0      678 2023-05-29 14:46:52.907219 iotcore_api-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    34546 2023-05-29 14:44:23.253425 iotcore_api-1.1.2/README.md
--rw-r--r--   0        0        0    34019 1970-01-01 00:00:00.000000 iotcore_api-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.3/iotcoreapi/__init__.py
+-rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.3/iotcoreapi/exceptions.py
+-rw-r--r--   0        0        0    56452 2023-05-30 15:26:21.704664 iotcore_api-1.1.3/iotcoreapi/iotcoreapi.py
+-rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.3/iotcoreapi/nan_treatment.py
+-rw-r--r--   0        0        0      967 2023-05-30 15:36:32.642125 iotcore_api-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    34547 2023-05-30 15:37:22.814144 iotcore_api-1.1.3/README.md
+-rw-r--r--   0        0        0    34182 1970-01-01 00:00:00.000000 iotcore_api-1.1.3/PKG-INFO
```

### Comparing `iotcore_api-1.1.2/iotcoreapi/exceptions.py` & `iotcore_api-1.1.3/iotcoreapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.2/iotcoreapi/iotcoreapi.py` & `iotcore_api-1.1.3/iotcoreapi/iotcoreapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         return response
 
     return wrapper
 
 
 class IoTCoreAPI:
 
-    def __init__(self, ip: str = "localhost", port: int = 56000, token: str = "", version: typing.Union[str, int] = "3.0",
+    def __init__(self, ip: str = "localhost", port: int = 56000, token: str = "", version: str = "3.0",
                  logger: logging.Logger = None):
         """
         Init method for iotcoreapi. Needs API configuration parameters
 
         Args:
             ip: IoT Core base endpoint
             port: API Port. Defaults to 56000
@@ -80,15 +80,15 @@
         version_regex = r'^\d+\.\d+$'
         if not bool(re.match(version_regex, version)):
             raise ValueError('Version number does not match correct format. Should be "1.0", "2.0"...')
         self.version = version
         self._version_number = float(version)
         self._time_formats = ['datetime', 'unix']
         self._output_formats = ['dataframe', 'json']
-        self.url_NX = "http://" + ip + ":" + str(port)
+        self.url_NX = ip + ":" + str(port)
         self.header = {
             "nexustoken": self.token,
             "nexusapiversion": self.version,
             "Content-Type": "application/json",
         }
         self.logger = logger
         self._log_print("Created new instance of IoTCoreAPI")
```

### Comparing `iotcore_api-1.1.2/iotcoreapi/nan_treatment.py` & `iotcore_api-1.1.3/iotcoreapi/nan_treatment.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.2/README.md` & `iotcore_api-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 1. [Installation](#how-to-install)
 2. [Use](#use)
 3. [Explanation](#explanation)
 4. [Reference](#reference)
 
 # How to install
-This library requieres Python 3.8 or higher. 
+This library requieres Python 3.8 or higher.
 IoTCore API can be installed with ```pip```. Dependencies will be installed along with the library.
 
 ```bash
 pip install iotcore-api
 ```
 
 # Use
@@ -222,15 +222,15 @@
 
 #### \_\_init\_\_
 
 ```python
 def __init__(ip: str = "localhost",
              port: int = 56000,
              token: str = "",
-             version: typing.Union[str, int] = "3.0",
+             version: str = "3.0",
              logger: logging.Logger = None)
 ```
 
 Init method for iotcoreapi. Needs API configuration parameters
 
 **Arguments**:
 
@@ -252,15 +252,15 @@
 
 Return all tags available for the token
 
 **Arguments**:
 
 - `include_attributes` _optional_ - if version >3.0, bool to return attributes or not
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_filtered"></a>
 
@@ -280,15 +280,15 @@
 **Arguments**:
 
 - `installations` - name of the installations
 - `drivers` - name of drivers
 - `tags` - name of tags
 - `attributes` - not implemented yet
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_attributes"></a>
 
@@ -300,15 +300,15 @@
 ```
 
 Obtaining the list of possible attributes within the system and, when limited to a set of values, the list of possible values
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_writable"></a>
 
@@ -320,15 +320,15 @@
 ```
 
 Return tags available for writing. If version is under 3.0, returned array does not have attribute information
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_documents"></a>
 
@@ -340,15 +340,15 @@
 ```
 
 Returns all tagviews shared in the token
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tagview_detail"></a>
 
@@ -362,15 +362,15 @@
 
 Return all variables from a given tagview
 
 **Arguments**:
 
 - `uid` - uid of the tagview
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarms"></a>
 
@@ -385,15 +385,15 @@
 
 Returns information of the alarms in the token
 
 **Arguments**:
 
 - `group_uid` - Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarm_groups"></a>
 
@@ -406,71 +406,71 @@
 ```
 
 Returns information of the alarm groups in the token
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime"></a>
 
 #### read\_tags\_realtime
 
 ```python
 def read_tags_realtime(
         tags_uids: typing.List[str],
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Reads real time value of the tags provided in the array tags_uids
 
 **Arguments**:
 
 - `tags_uids` - list with uids of the tags
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime"></a>
 
 #### read\_tagview\_realtime
 
 ```python
 def read_tagview_realtime(
         uid: str,
         uids_tags: typing.List[str] = None,
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Returns real time value for the uids variables provided in a given tagview
 
 **Arguments**:
 
 - `uid` - uid of the tagview
 - `uids_tags` - list of uids
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_historic"></a>
 
@@ -481,15 +481,15 @@
         uids: typing.List[str],
         start_ts: typing.Union[int, float],
         end_ts: typing.Union[int, float],
         data_source: typing.Union[str, int] = 'RAW',
         resolution: typing.Union[str, int] = 'RES_1_HOUR',
         agg_operation: typing.Union[str, int] = "LAST_VALUE",
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Obtain historic data of the specified tags
 
 **Arguments**:
@@ -499,15 +499,15 @@
 - `end_ts` - end time in unix time or datetime
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_rawhistoric"></a>
 
@@ -515,30 +515,30 @@
 
 ```python
 def read_tags_rawhistoric(
         uids,
         start_ts,
         end_ts,
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 To obtain raw data with no aggregation or normalization applied
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix time or datetime
 - `end_ts` - end time in unix time or datetime
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_transient"></a>
 
@@ -548,15 +548,15 @@
 def read_tags_transient(
         uids: typing.List[str],
         start_ts: typing.Union[int, float],
         end_ts: typing.Union[int, float],
         data_source: typing.Union[str, int] = None,
         resolution: typing.Union[str, int] = 'RES_1_SEC',
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
 aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
 please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
@@ -568,15 +568,15 @@
 - `start_ts` - time in unix time or datetime
 - `end_ts` - end time in unix time or datetime. Timespan must be smaller than 15 mins
 - `data_source` - Can be set to null or empty. Not needed
 - `resolution` - RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_historic"></a>
 
@@ -587,15 +587,15 @@
         uid: str,
         start_ts: typing.Union[datetime.datetime, float, int],
         end_ts: typing.Union[datetime.datetime, float, int],
         tags_uids: typing.List[str] = None,
         data_source='RAW',
         resolution='RES_1_HOUR',
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
 
 **Arguments**:
@@ -605,15 +605,15 @@
 - `end_ts` - end time in unix or datetime
 - `tags_uids` _optional_ - list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_historic_text_filters"></a>
 
@@ -633,15 +633,15 @@
 - `end_ts` - end time in unix or datetime
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
 - `name` - name of tag
 - `value` - value of tag
@@ -666,15 +666,15 @@
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
 - `name` - name of tag
 - `value` - value of tag
@@ -709,15 +709,15 @@
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime_text_filters"></a>
 
@@ -736,15 +736,15 @@
 
 **Arguments**:
 
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   dataframe or json:
   columns:
 - `name` - name of tag
 - `value` - value of tag
@@ -759,15 +759,15 @@
 ```
 
 Reads alarm status for a given alarm
 
 **Arguments**:
 
 - `alarm_guid` - guid of the alarm
-  
+
 
 **Returns**:
 
   Dictionary with following data:
   {
 - `"name"` - "BasicAlarm1",
 - `"uid"` - "b926bfb0-3f2f-49df-a2eb-138452296903",
@@ -795,15 +795,15 @@
 ```
 
 Check if provided tag names exist, then create them if not
 
 **Arguments**:
 
 - `tags` - tags name or names to be created
-  
+
 
 **Returns**:
 
   response object in json format:
   [
   {
 - `"Uid"` - "unique tag identifier",
@@ -822,29 +822,30 @@
   ]
 
 <a id="iotcoreapi.IoTCoreAPI.write_tag_insert_or_update"></a>
 
 #### write\_tag\_insert\_or\_update
 
 ```python
-def write_tag_insert_or_update(tagname, **attributes) -> typing.List[dict]
+def write_tag_insert_or_update(tagname: str,
+                               **attributes) -> typing.List[dict]
 ```
 
 This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
 **Arguments**:
 
 - `tagname` - name of the new tag
 - `**attributes` - dictionary of attributes and their values
-  
+
 
 **Returns**:
 
   response in json format
-  
+
 
 **Examples**:
 
   Call the function with a tag name and any number of attributes
   response = write_tag_insert_or_update(tagname="mytag", attribute1="value1", attribute2="value2", attribute3="value3")
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_insert_or_update_by_json"></a>
@@ -870,15 +871,15 @@
 - `"AttributeName"` - "NameOfAttribute1",
 - `"Value"` - "ValueOfAttribute1"
   }
   ]
   }
   ],
   ...
-  
+
 
 **Returns**:
 
   response in json format
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_historic_insert"></a>
 
@@ -896,15 +897,15 @@
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
 - `value` - value of the tag
 - `timeStamp` - timeStamp in unix
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
-  
+
 
 **Returns**:
 
   response in json format
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_realtime_insert"></a>
 
@@ -921,15 +922,15 @@
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
 - `value` - value of the tag
 - `timeStamp` _optional_ - timeStamp in unix. If not provided, will take current time
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
-  
+
 
 **Returns**:
 
   response text (None if OK)
 
 <a id="iotcoreapi.IoTCoreAPI.write_tag_realtime_insert"></a>
 
@@ -944,15 +945,15 @@
 Update realtime data for a single tag. Tag needs to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `name` - tag name
 - `value` - value of the tag
 - `timeStamp` _optional_ - time in unix time. If None, will take current time
-  
+
 
 **Returns**:
 
   response text (None if OK)
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_transient_insert"></a>
 
@@ -970,15 +971,15 @@
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
 - `value` - value of the tag
 - `timeStamp` - timeStamp in unix
   skip_errors  = True: If true, not created tags will be dropped from dataframe
-  
+
 
 **Returns**:
 
   response in json format
 
 <a id="iotcoreapi.IoTCoreAPI.write_alarm_acknowledge"></a>
 
@@ -990,15 +991,15 @@
 
 Used to change the status of an alarm from ANR or ENR to ARE o EXR.
 
 **Arguments**:
 
 - `guid` - guid of the alarm
 - `status` - 'ARE' or 'EXR', 'ANR' or 'ENR'
-  
+
 
 **Returns**:
 
   response text (None if OK)
 
 <a id="iotcoreapi.IoTCoreAPI.write_alarm_event"></a>
 
@@ -1042,8 +1043,7 @@
 
 If the token has access to operate against a Conector associated with a PLC, this method can be used to write values to the actual Plc's tags.
 
 **Arguments**:
 
 - `tag_uid` - nombre de la variable a escribir en el PLC
 - `value` - valor de la variable a escribir
-
```

### Comparing `iotcore_api-1.1.2/PKG-INFO` & `iotcore_api-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 Metadata-Version: 2.1
 Name: iotcore-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: IoT core connection methods and utilities
-Author: Idrica
+Keywords: iotcoreapi,goaigua
+Author: Ricardo Gomez
+Author-email: ricardo.gomez.aldaravi@idrica.com
+Maintainer: Ricardo Gomez
+Maintainer-email: ricardo.gomez.aldaravi@idrica.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
@@ -21,15 +25,15 @@
 
 1. [Installation](#how-to-install)
 2. [Use](#use)
 3. [Explanation](#explanation)
 4. [Reference](#reference)
 
 # How to install
-This library requieres Python 3.8 or higher. 
+This library requieres Python 3.8 or higher.
 IoTCore API can be installed with ```pip```. Dependencies will be installed along with the library.
 
 ```bash
 pip install iotcore-api
 ```
 
 # Use
@@ -237,15 +241,15 @@
 
 #### \_\_init\_\_
 
 ```python
 def __init__(ip: str = "localhost",
              port: int = 56000,
              token: str = "",
-             version: typing.Union[str, int] = "3.0",
+             version: str = "3.0",
              logger: logging.Logger = None)
 ```
 
 Init method for iotcoreapi. Needs API configuration parameters
 
 **Arguments**:
 
@@ -267,15 +271,15 @@
 
 Return all tags available for the token
 
 **Arguments**:
 
 - `include_attributes` _optional_ - if version >3.0, bool to return attributes or not
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_filtered"></a>
 
@@ -295,15 +299,15 @@
 **Arguments**:
 
 - `installations` - name of the installations
 - `drivers` - name of drivers
 - `tags` - name of tags
 - `attributes` - not implemented yet
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_attributes"></a>
 
@@ -315,15 +319,15 @@
 ```
 
 Obtaining the list of possible attributes within the system and, when limited to a set of values, the list of possible values
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_writable"></a>
 
@@ -335,15 +339,15 @@
 ```
 
 Return tags available for writing. If version is under 3.0, returned array does not have attribute information
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_documents"></a>
 
@@ -355,15 +359,15 @@
 ```
 
 Returns all tagviews shared in the token
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tagview_detail"></a>
 
@@ -377,15 +381,15 @@
 
 Return all variables from a given tagview
 
 **Arguments**:
 
 - `uid` - uid of the tagview
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarms"></a>
 
@@ -400,15 +404,15 @@
 
 Returns information of the alarms in the token
 
 **Arguments**:
 
 - `group_uid` - Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarm_groups"></a>
 
@@ -421,71 +425,71 @@
 ```
 
 Returns information of the alarm groups in the token
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime"></a>
 
 #### read\_tags\_realtime
 
 ```python
 def read_tags_realtime(
         tags_uids: typing.List[str],
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Reads real time value of the tags provided in the array tags_uids
 
 **Arguments**:
 
 - `tags_uids` - list with uids of the tags
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime"></a>
 
 #### read\_tagview\_realtime
 
 ```python
 def read_tagview_realtime(
         uid: str,
         uids_tags: typing.List[str] = None,
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Returns real time value for the uids variables provided in a given tagview
 
 **Arguments**:
 
 - `uid` - uid of the tagview
 - `uids_tags` - list of uids
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_historic"></a>
 
@@ -496,15 +500,15 @@
         uids: typing.List[str],
         start_ts: typing.Union[int, float],
         end_ts: typing.Union[int, float],
         data_source: typing.Union[str, int] = 'RAW',
         resolution: typing.Union[str, int] = 'RES_1_HOUR',
         agg_operation: typing.Union[str, int] = "LAST_VALUE",
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Obtain historic data of the specified tags
 
 **Arguments**:
@@ -514,15 +518,15 @@
 - `end_ts` - end time in unix time or datetime
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_rawhistoric"></a>
 
@@ -530,30 +534,30 @@
 
 ```python
 def read_tags_rawhistoric(
         uids,
         start_ts,
         end_ts,
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 To obtain raw data with no aggregation or normalization applied
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix time or datetime
 - `end_ts` - end time in unix time or datetime
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_transient"></a>
 
@@ -563,15 +567,15 @@
 def read_tags_transient(
         uids: typing.List[str],
         start_ts: typing.Union[int, float],
         end_ts: typing.Union[int, float],
         data_source: typing.Union[str, int] = None,
         resolution: typing.Union[str, int] = 'RES_1_SEC',
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
 aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
 please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
@@ -583,15 +587,15 @@
 - `start_ts` - time in unix time or datetime
 - `end_ts` - end time in unix time or datetime. Timespan must be smaller than 15 mins
 - `data_source` - Can be set to null or empty. Not needed
 - `resolution` - RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_historic"></a>
 
@@ -602,15 +606,15 @@
         uid: str,
         start_ts: typing.Union[datetime.datetime, float, int],
         end_ts: typing.Union[datetime.datetime, float, int],
         tags_uids: typing.List[str] = None,
         data_source='RAW',
         resolution='RES_1_HOUR',
         output_format: str = 'dataframe',
-        time_format='datetime',
+        time_format: str = 'datetime',
         nan_method: str = None
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
 
 **Arguments**:
@@ -620,15 +624,15 @@
 - `end_ts` - end time in unix or datetime
 - `tags_uids` _optional_ - list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_historic_text_filters"></a>
 
@@ -648,15 +652,15 @@
 - `end_ts` - end time in unix or datetime
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
 - `name` - name of tag
 - `value` - value of tag
@@ -681,15 +685,15 @@
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
 - `name` - name of tag
 - `value` - value of tag
@@ -724,15 +728,15 @@
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime_text_filters"></a>
 
@@ -751,15 +755,15 @@
 
 **Arguments**:
 
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 - `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
-  
+
 
 **Returns**:
 
   dataframe or json:
   columns:
 - `name` - name of tag
 - `value` - value of tag
@@ -774,15 +778,15 @@
 ```
 
 Reads alarm status for a given alarm
 
 **Arguments**:
 
 - `alarm_guid` - guid of the alarm
-  
+
 
 **Returns**:
 
   Dictionary with following data:
   {
 - `"name"` - "BasicAlarm1",
 - `"uid"` - "b926bfb0-3f2f-49df-a2eb-138452296903",
@@ -810,15 +814,15 @@
 ```
 
 Check if provided tag names exist, then create them if not
 
 **Arguments**:
 
 - `tags` - tags name or names to be created
-  
+
 
 **Returns**:
 
   response object in json format:
   [
   {
 - `"Uid"` - "unique tag identifier",
@@ -837,29 +841,30 @@
   ]
 
 <a id="iotcoreapi.IoTCoreAPI.write_tag_insert_or_update"></a>
 
 #### write\_tag\_insert\_or\_update
 
 ```python
-def write_tag_insert_or_update(tagname, **attributes) -> typing.List[dict]
+def write_tag_insert_or_update(tagname: str,
+                               **attributes) -> typing.List[dict]
 ```
 
 This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
 **Arguments**:
 
 - `tagname` - name of the new tag
 - `**attributes` - dictionary of attributes and their values
-  
+
 
 **Returns**:
 
   response in json format
-  
+
 
 **Examples**:
 
   Call the function with a tag name and any number of attributes
   response = write_tag_insert_or_update(tagname="mytag", attribute1="value1", attribute2="value2", attribute3="value3")
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_insert_or_update_by_json"></a>
@@ -885,15 +890,15 @@
 - `"AttributeName"` - "NameOfAttribute1",
 - `"Value"` - "ValueOfAttribute1"
   }
   ]
   }
   ],
   ...
-  
+
 
 **Returns**:
 
   response in json format
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_historic_insert"></a>
 
@@ -911,15 +916,15 @@
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
 - `value` - value of the tag
 - `timeStamp` - timeStamp in unix
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
-  
+
 
 **Returns**:
 
   response in json format
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_realtime_insert"></a>
 
@@ -936,15 +941,15 @@
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
 - `value` - value of the tag
 - `timeStamp` _optional_ - timeStamp in unix. If not provided, will take current time
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
-  
+
 
 **Returns**:
 
   response text (None if OK)
 
 <a id="iotcoreapi.IoTCoreAPI.write_tag_realtime_insert"></a>
 
@@ -959,15 +964,15 @@
 Update realtime data for a single tag. Tag needs to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `name` - tag name
 - `value` - value of the tag
 - `timeStamp` _optional_ - time in unix time. If None, will take current time
-  
+
 
 **Returns**:
 
   response text (None if OK)
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_transient_insert"></a>
 
@@ -985,15 +990,15 @@
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
 - `value` - value of the tag
 - `timeStamp` - timeStamp in unix
   skip_errors  = True: If true, not created tags will be dropped from dataframe
-  
+
 
 **Returns**:
 
   response in json format
 
 <a id="iotcoreapi.IoTCoreAPI.write_alarm_acknowledge"></a>
 
@@ -1005,15 +1010,15 @@
 
 Used to change the status of an alarm from ANR or ENR to ARE o EXR.
 
 **Arguments**:
 
 - `guid` - guid of the alarm
 - `status` - 'ARE' or 'EXR', 'ANR' or 'ENR'
-  
+
 
 **Returns**:
 
   response text (None if OK)
 
 <a id="iotcoreapi.IoTCoreAPI.write_alarm_event"></a>
 
@@ -1058,8 +1063,7 @@
 If the token has access to operate against a Conector associated with a PLC, this method can be used to write values to the actual Plc's tags.
 
 **Arguments**:
 
 - `tag_uid` - nombre de la variable a escribir en el PLC
 - `value` - valor de la variable a escribir
 
-
```

