# Comparing `tmp/smartdash-0.0.1.dev5.tar.gz` & `tmp/smartdash-0.0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdash-0.0.1.dev5.tar", last modified: Tue May 30 10:15:46 2023, max compression
+gzip compressed data, was "smartdash-0.0.1.dev6.tar", last modified: Tue May 30 10:25:46 2023, max compression
```

## Comparing `smartdash-0.0.1.dev5.tar` & `smartdash-0.0.1.dev6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:15:46.599138 smartdash-0.0.1.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 10:15:46.599138 smartdash-0.0.1.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:15:46.599138 smartdash-0.0.1.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:15:46.595138 smartdash-0.0.1.dev5/smartdash/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/smartdash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/smartdash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/smartdash/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-30 10:15:34.000000 smartdash-0.0.1.dev5/smartdash/smartdash_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:15:46.599138 smartdash-0.0.1.dev5/smartdash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 10:15:46.000000 smartdash-0.0.1.dev5/smartdash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/smartdash/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/smartdash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/smartdash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/smartdash/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/smartdash/smartdash_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/smartdash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/top_level.txt
```

### Comparing `smartdash-0.0.1.dev5/PKG-INFO` & `smartdash-0.0.1.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev5
+Version: 0.0.1.dev6
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `smartdash-0.0.1.dev5/setup.py` & `smartdash-0.0.1.dev6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "smartdash"
 DESCRIPTION = "python logging client for SmartDash"
 URL = "https://github.com/notAI-tech/smartdash"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev5"
+VERSION = "0.0.1.dev6"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["requests", "liteindex", "streamlit", "plotly"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

### Comparing `smartdash-0.0.1.dev5/smartdash/__init__.py` & `smartdash-0.0.1.dev6/smartdash/__init__.py`

 * *Files identical despite different names*

### Comparing `smartdash-0.0.1.dev5/smartdash/dash.py` & `smartdash-0.0.1.dev6/smartdash/dash.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,135 +39,167 @@
 
 # Main function to run the Streamlit app
 def main():
     st.set_page_config(page_title="SmartDash", layout="wide")
 
     st.sidebar.title("SmartDash - App Dashboard")
 
-    # Dropdowns for app_name and last_n_hours in the sidebar
-    st.sidebar.markdown("## Settings")
-    app_name = st.sidebar.selectbox(
-        "Select App",
-        requests.get(f"{SERVER_URL}/app_names").json()["app_names"],
-        index=0,
-    )
-    time_range = st.sidebar.selectbox(
-        "Select Time Range", ["8 hours", "12 hours", "Last day", "Last week"], index=0
-    )
-
-    in_process_range = st.sidebar.selectbox(
-        "Highlight long running uids", ["1 hour", "15 min", "30 min"], index=0
-    )
-
-    time_mapping = {"8 hours": 8, "12 hours": 12, "Last day": 24, "Last week": 168}
-    last_n_hours = time_mapping[time_range]
-
-    data_by_uid, _ = fetch_dash_data(app_name, last_n_hours)
-
-    all_tags, all_levels, all_stages = get_all_tags_levels_stages(data_by_uid)
-
-    # Add filters in the sidebar
-    st.sidebar.markdown("## Filter Logs")
-    filter_tags = st.sidebar.multiselect("Tags", all_tags)
-    filter_level = st.sidebar.selectbox("Level", ["All"] + all_levels, index=0)
-    filter_stage = st.sidebar.selectbox("Stage", ["All"] + all_stages, index=0)
-    filter_uid = st.sidebar.text_input("UID")
-
-    # Calculate total time per unique ID
-    total_times = {}
-    for uid, data in data_by_uid.items():
-        if data["logs"]:
-            first_log_time = data["logs"][0]["timestamp"]
-            last_log_time = data["logs"][-1]["timestamp"]
-            total_times[uid] = last_log_time - first_log_time
-
-    # Create a pie chart showing the distribution of times taken by each stage
-    stage_times = {}
-    for uid, data in data_by_uid.items():
-        for stage, times in data["stage_wise_times"].items():
-            if stage not in stage_times:
-                stage_times[stage] = times["end"] - times["start"]
-            else:
-                stage_times[stage] += times["end"] - times["start"]
-
-    stage_time_pie = px.pie(
-        values=list(stage_times.values()),
-        names=list(stage_times.keys()),
-        title="Time distribution by stage",
-    )
-
-    # Create a line chart showing the time taken by each stage with unique IDs on the x-axis and time taken on the y-axis
-    line_chart_data = []
-    for uid, data in data_by_uid.items():
-        for stage, times in data["stage_wise_times"].items():
-            line_chart_data.append(
-                {
-                    "uid": uid,
-                    "stage": stage,
-                    "time_taken": times["end"] - times["start"],
-                }
-            )
+    try:
+        # Dropdowns for app_name and last_n_hours in the sidebar
+        st.sidebar.markdown("## Settings")
+        app_name = st.sidebar.selectbox(
+            "Select App",
+            requests.get(f"{SERVER_URL}/app_names").json()["app_names"],
+            index=0,
+        )
+        time_range = st.sidebar.selectbox(
+            "Select Time Range",
+            ["8 hours", "12 hours", "Last day", "Last week"],
+            index=0,
+        )
+
+        long_running_range = st.sidebar.selectbox(
+            "Highlight long running uids", ["1 hour", "30 min", "15 min"], index=0
+        )
+
+        time_mapping = {
+            "8 hours": 8,
+            "12 hours": 12,
+            "Last day": 24,
+            "Last week": 168,
+            "1 hour": 1,
+            "15 min": 0.25,
+            "30 min": 0.5,
+        }
+
+        long_running_n_hours = time_mapping[long_running_range]
+        last_n_hours = time_mapping[time_range]
+
+        data_by_uid, _ = fetch_dash_data(app_name, last_n_hours, long_running_n_hours)
+
+        all_tags, all_levels, all_stages = get_all_tags_levels_stages(data_by_uid)
+
+        # Add filters in the sidebar
+        st.sidebar.markdown("## Filter Logs")
+        filter_tags = st.sidebar.multiselect("Tags", all_tags)
+        filter_level = st.sidebar.selectbox("Level", ["All"] + all_levels, index=0)
+        filter_stage = st.sidebar.selectbox("Stage", ["All"] + all_stages, index=0)
+        filter_uid = st.sidebar.text_input("UID")
+
+        graphs = []
 
-    line_chart_df = pd.DataFrame(line_chart_data)
-    stage_time_line = px.line(
-        line_chart_df,
-        x="uid",
-        y="time_taken",
-        color="stage",
-        title="Time taken by each stage",
-    )
-
-    # Pie chart showing number of failed, success, and in-process uids
-    metrics_pie = px.pie(
-        values=[
-            sum([1 for uid, data in data_by_uid.items() if data["success"]]),
-            sum([1 for uid, data in data_by_uid.items() if data["in_process"]]),
-            sum([1 for uid, data in data_by_uid.items() if data["failed"]]),
-            sum([1 for uid, data in data_by_uid.items() if data["long_running"]]),
-        ],
-        names=["Success", "In Process", "Failed", "Long running"],
-        title="Uids by Status",
-    )
-
-    graphs = [stage_time_pie, stage_time_line, metrics_pie]
-
-    cols = st.columns(2, gap="small")
-    for i, graph in enumerate(graphs):
-        cols[i % 2].write(graph)
+        # Calculate total time per unique ID
+        total_times = {}
+        for uid, data in data_by_uid.items():
+            if data["logs"]:
+                first_log_time = data["logs"][0]["timestamp"]
+                last_log_time = data["logs"][-1]["timestamp"]
+                total_times[uid] = last_log_time - first_log_time
 
-    with st.expander("Show/hide logs"):
-        logs_data = []
+        # Create a pie chart showing the distribution of times taken by each stage
+        stage_times = {}
         for uid, data in data_by_uid.items():
-            logs_data.extend(data["logs"])
-            if data["success"]:
-                logs_data[-1]["status"] = "Success"
-            elif data["failed"]:
-                logs_data[-1]["status"] = "Failed"
-            elif data["in_process"]:
-                logs_data[-1]["status"] = "In Process"
-            elif data["long_running"]:
-                logs_data[-1]["status"] = "Long running"
-            else:
-                logs_data[-1]["status"] = "Unknown"
-
-        # Convert timestamp to datetime format
-        for log in logs_data:
-            log["timestamp"] = datetime.fromtimestamp(log["timestamp"])
-
-        # Apply filters
-        if filter_tags:
-            logs_data = [
-                log for log in logs_data if set(log["tags"]) & set(filter_tags)
-            ]
-        if filter_level != "All":
-            logs_data = [log for log in logs_data if log["level"] == filter_level]
-        if filter_stage != "All":
-            logs_data = [log for log in logs_data if log["stage"] == filter_stage]
-        if filter_uid:
-            logs_data = [log for log in logs_data if log["u_id"] == filter_uid]
+            for stage, times in data["stage_wise_times"].items():
+                if stage not in stage_times:
+                    stage_times[stage] = times["end"] - times["start"]
+                else:
+                    stage_times[stage] += times["end"] - times["start"]
+
+        if stage_times:
+            stage_time_pie = px.pie(
+                values=list(stage_times.values()),
+                names=list(stage_times.keys()),
+                title="Time distribution by stage",
+            )
+            graphs.append(stage_time_pie)
+
+        # Create a line chart showing the time taken by each stage with unique IDs on the x-axis and time taken on the y-axis
+        line_chart_data = []
+        for uid, data in data_by_uid.items():
+            for stage, times in data["stage_wise_times"].items():
+                line_chart_data.append(
+                    {
+                        "uid": uid,
+                        "stage": stage,
+                        "time_taken": times["end"] - times["start"],
+                    }
+                )
+
+        if line_chart_data:
+            line_chart_df = pd.DataFrame(line_chart_data)
+            stage_time_line = px.line(
+                line_chart_df,
+                x="uid",
+                y="time_taken",
+                color="stage",
+                title="Time taken by each stage",
+            )
+            graphs.append(stage_time_line)
+
+        if data_by_uid:
+            # Pie chart showing number of failed, success, and in-process uids
+            metrics_pie = px.pie(
+                values=[
+                    sum([1 for uid, data in data_by_uid.items() if data["success"]]),
+                    sum([1 for uid, data in data_by_uid.items() if data["in_process"]]),
+                    sum([1 for uid, data in data_by_uid.items() if data["failed"]]),
+                    sum(
+                        [1 for uid, data in data_by_uid.items() if data["long_running"]]
+                    ),
+                ],
+                names=["Success", "In Process", "Failed", "Long running"],
+                title="Uids by Status",
+            )
+            graphs.append(metrics_pie)
 
-        logs_df = pd.DataFrame(logs_data)
-        st.dataframe(logs_df)
+        cols = st.columns(2, gap="small")
+        for i, graph in enumerate(graphs):
+            cols[i % 2].write(graph)
+
+        with st.expander("Show/hide logs"):
+            logs_data = []
+            for uid, data in data_by_uid.items():
+                logs_data.extend(data["logs"])
+                if data["success"]:
+                    logs_data[-1]["status"] = "Success"
+                elif data["failed"]:
+                    logs_data[-1]["status"] = "Failed"
+                elif data["in_process"]:
+                    logs_data[-1]["status"] = "In Process"
+                elif data["long_running"]:
+                    logs_data[-1]["status"] = "Long running"
+                else:
+                    logs_data[-1]["status"] = "Unknown"
+
+            if logs_data:
+                # Convert timestamp to datetime format
+                for log in logs_data:
+                    log["timestamp"] = datetime.fromtimestamp(log["timestamp"])
+
+                # Apply filters
+                if filter_tags:
+                    logs_data = [
+                        log for log in logs_data if set(log["tags"]) & set(filter_tags)
+                    ]
+                if filter_level != "All":
+                    logs_data = [
+                        log for log in logs_data if log["level"] == filter_level
+                    ]
+                if filter_stage != "All":
+                    logs_data = [
+                        log for log in logs_data if log["stage"] == filter_stage
+                    ]
+                if filter_uid:
+                    logs_data = [log for log in logs_data if log["u_id"] == filter_uid]
+
+                logs_df = pd.DataFrame(logs_data)
+                st.dataframe(logs_df)
+
+    except Exception as e:
+        st.warning(
+            "No Apps uploaded logs yet. Please upload logs using the smartlogger CLI."
+        )
+        st.stop()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `smartdash-0.0.1.dev5/smartdash/smartdash_server.py` & `smartdash-0.0.1.dev6/smartdash/smartdash_server.py`

 * *Files identical despite different names*

### Comparing `smartdash-0.0.1.dev5/smartdash.egg-info/PKG-INFO` & `smartdash-0.0.1.dev6/smartdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev5
+Version: 0.0.1.dev6
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

