# Comparing `tmp/slac-alarm-manager-1.2.0.tar.gz` & `tmp/slac-alarm-manager-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slac-alarm-manager-1.2.0.tar", last modified: Tue Mar 21 19:55:12 2023, max compression
+gzip compressed data, was "slac-alarm-manager-1.2.1.tar", last modified: Tue May 30 16:56:34 2023, max compression
```

## Comparing `slac-alarm-manager-1.2.0.tar` & `slac-alarm-manager-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:55:12.572912 slac-alarm-manager-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-21 19:55:12.568912 slac-alarm-manager-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:55:12.568912 slac-alarm-manager-1.2.0/pydm_alarm_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/pydm_alarm_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/pydm_alarm_plugin/alarm_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 19:55:12.572912 slac-alarm-manager-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:55:12.568912 slac-alarm-manager-1.2.0/slac_alarm_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-21 19:55:12.000000 slac-alarm-manager-1.2.0/slac_alarm_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-21 19:55:12.000000 slac-alarm-manager-1.2.0/slac_alarm_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:55:12.000000 slac-alarm-manager-1.2.0/slac_alarm_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-21 19:55:12.000000 slac-alarm-manager-1.2.0/slac_alarm_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-21 19:55:12.000000 slac-alarm-manager-1.2.0/slac_alarm_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-21 19:55:12.000000 slac-alarm-manager-1.2.0/slac_alarm_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:55:12.568912 slac-alarm-manager-1.2.0/slam/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/alarm_configuration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/alarm_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/alarm_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/alarm_table_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/alarm_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/alarm_tree_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/archive_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/kafka_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:55:12.568912 slac-alarm-manager-1.2.0/slam_launcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam_launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-21 19:55:03.000000 slac-alarm-manager-1.2.0/slam_launcher/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.712424 slac-alarm-manager-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-30 16:56:34.712424 slac-alarm-manager-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.708424 slac-alarm-manager-1.2.1/pydm_alarm_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/pydm_alarm_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/pydm_alarm_plugin/alarm_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:56:34.712424 slac-alarm-manager-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.708424 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.708424 slac-alarm-manager-1.2.1/slam/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_configuration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_table_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_tree_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/archive_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/kafka_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14516 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.712424 slac-alarm-manager-1.2.1/slam_launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam_launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam_launcher/main.py
```

### Comparing `slac-alarm-manager-1.2.0/LICENSE.md` & `slac-alarm-manager-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/PKG-INFO` & `slac-alarm-manager-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slac-alarm-manager
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python interface for managing alarms
 Home-page: https://github.com/slaclab/slac-alarm-manager
 Author: SLAC National Accelerator Laboratory
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `slac-alarm-manager-1.2.0/README.md` & `slac-alarm-manager-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/pydm_alarm_plugin/alarm_plugin.py` & `slac-alarm-manager-1.2.1/pydm_alarm_plugin/alarm_plugin.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/setup.py` & `slac-alarm-manager-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 curr_dir = Path(__file__).parent
 long_description = (curr_dir/'README.md').read_text()
 
 setup(
     name='slac-alarm-manager',
-    version='1.2.0',
+    version='1.2.1',
     description='Python interface for managing alarms',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='SLAC National Accelerator Laboratory',
     url='https://github.com/slaclab/slac-alarm-manager',
     packages=['slam', 'slam_launcher', 'pydm_alarm_plugin'],
     install_requires=['kafka-python', 'pydm', 'qtpy'],
```

### Comparing `slac-alarm-manager-1.2.0/slac_alarm_manager.egg-info/PKG-INFO` & `slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slac-alarm-manager
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python interface for managing alarms
 Home-page: https://github.com/slaclab/slac-alarm-manager
 Author: SLAC National Accelerator Laboratory
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `slac-alarm-manager-1.2.0/slac_alarm_manager.egg-info/SOURCES.txt` & `slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/slam/alarm_configuration_widget.py` & `slac-alarm-manager-1.2.1/slam/alarm_configuration_widget.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/slam/alarm_item.py` & `slac-alarm-manager-1.2.1/slam/alarm_item.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/slam/alarm_table_model.py` & `slac-alarm-manager-1.2.1/slam/alarm_table_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,27 +85,25 @@
     def append(self, alarm_item: AlarmItem) -> None:
         """ Appends a row to this table with data as given by the input alarm item """
         if alarm_item.alarm_severity == AlarmSeverity.OK:
             return  # Don't want to add unnecessary items to the table
         if alarm_item.name in self.alarm_items:
             logger.warning(f'Attempting to append a row to the alarm table which is already there: {alarm_item.name}')
             return
-        self.beginInsertRows(QModelIndex(), len(self.alarm_items), len(self.alarm_items))
+        self.layoutAboutToBeChanged.emit()
         self.alarm_items[alarm_item.name] = alarm_item
-        self.endInsertRows()
         self.layoutChanged.emit()
 
     def remove_row(self, alarm_name: str):
         """ Removes the row associated with the input name from this table """
         if alarm_name not in self.alarm_items:
             return
         index_to_remove = list(self.alarm_items.keys()).index(alarm_name)
-        self.beginRemoveRows(QModelIndex(), index_to_remove, index_to_remove)
+        self.layoutAboutToBeChanged.emit()
         del self.alarm_items[alarm_name]
-        self.endRemoveRows()
         self.layoutChanged.emit()
 
     def sort(self, col: int, order=Qt.AscendingOrder):
         """ Sort the table by the input column """
         self.layoutAboutToBeChanged.emit()
         self.alarm_items = OrderedDict(sorted(self.alarm_items.items(),
                                               key=lambda alarm_item: getattr(alarm_item[1], self.column_to_attr[col]),
```

### Comparing `slac-alarm-manager-1.2.0/slam/alarm_table_view.py` & `slac-alarm-manager-1.2.1/slam/alarm_table_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import enum
 import getpass
 import socket
+from functools import partial
 from kafka.producer import KafkaProducer
-from qtpy.QtCore import QEvent, QSortFilterProxyModel, Qt, Signal
+from qtpy.QtCore import QEvent, QModelIndex, QSortFilterProxyModel, Qt, Signal
 from qtpy.QtGui import QCursor
 from qtpy.QtWidgets import (QAbstractItemView, QAction, QApplication, QHBoxLayout, QHeaderView, QLabel,
                             QLineEdit, QMenu, QPushButton, QTableView, QVBoxLayout, QWidget)
-from typing import Callable
+from typing import Callable, List
 from .alarm_table_model import AlarmItemsTableModel
 from .alarm_tree_model import AlarmItemsTreeModel
 from .permissions import UserAction, can_take_action
 
 
 class AlarmTableType(str, enum.Enum):
     """
@@ -82,16 +83,16 @@
 
         # The actions which may be taken on an alarm
         self.alarm_context_menu = QMenu(self)
         self.acknowledge_action = QAction('Acknowledge')
         self.unacknowledge_action = QAction('Unacknowledge')
         self.copy_action = QAction('Copy PV To Clipboard')
         self.plot_action = QAction('Draw Plot')
-        self.acknowledge_action.triggered.connect(self.send_acknowledgement)
-        self.unacknowledge_action.triggered.connect(self.send_unacknowledgement)
+        self.acknowledge_action.triggered.connect(partial(self.send_acknowledge_action, True))
+        self.unacknowledge_action.triggered.connect(partial(self.send_acknowledge_action, False))
         self.plot_action.triggered.connect(self.plot_pv)
         self.copy_action.triggered.connect(self.copy_alarm_name_to_clipboard)
 
         if self.table_type is AlarmTableType.ACTIVE:
             self.alarm_context_menu.addAction(self.acknowledge_action)
         if self.table_type is AlarmTableType.ACKNOWLEDGED:
             self.alarm_context_menu.addAction(self.unacknowledge_action)
@@ -117,16 +118,15 @@
         self.search_layout.addWidget(self.alarm_filter_bar)
         self.search_layout.addWidget(self.filter_button)
         self.search_layout.setAlignment(Qt.AlignLeft)
         self.layout.addLayout(self.search_layout)
         self.layout.addWidget(self.filter_active_label)
         self.layout.addWidget(self.alarmView)
 
-        self.alarmModel.rowsInserted.connect(self.update_counter_label)
-        self.alarmModel.rowsRemoved.connect(self.update_counter_label)
+        self.alarmModel.layoutChanged.connect(self.update_counter_label)
 
     def filter_table(self) -> None:
         """ Filter the table based on the text typed into the filter bar """
         if self.first_filter:
             # By delaying setting the proxy model until an actual filter request, performance is improved by a lot
             # when first loading data into the table
             self.first_filter = False
@@ -145,57 +145,56 @@
         else:
             self.alarm_count_label.setText(f'Acknowledged Alarms: {len(self.alarmModel.alarm_items)}')
 
     def alarm_context_menu_event(self, ev: QEvent) -> None:
         """ Display the right-click context menu for items in the active alarms table """
         self.alarm_context_menu.popup(QCursor.pos())
 
+    def get_selected_indices(self) -> List[QModelIndex]:
+        """ Return the indices which have been selected by the user, applying a mapping if a filter has been applied """
+        indices = self.alarmView.selectionModel().selectedRows()
+        if self.filter_active_label.isVisible():
+            indices = [self.alarm_proxy_model.mapToSource(proxy_index) for proxy_index in indices]
+        return indices
+
     def plot_pv(self) -> None:
         """ Send off the signal for plotting a PV """
-        indices = self.alarmView.selectedIndexes()
+        indices = self.get_selected_indices()
         if len(indices) > 0:
             index = indices[0]
             alarm_item = list(self.alarmModel.alarm_items.items())[index.row()][1]
             self.plot_signal.emit(alarm_item.name)
 
     def copy_alarm_name_to_clipboard(self) -> None:
         """ Copy the selected PV to the user's clipboard """
-        indices = self.alarmView.selectionModel().selectedRows()
+        indices = self.get_selected_indices()
         if len(indices) > 0:
             copy_text = ''
             for index in indices:
                 alarm_item = list(self.alarmModel.alarm_items.items())[index.row()][1]
                 copy_text += alarm_item.name + ' '
             self.clipboard.setText(copy_text[:-1], mode=self.clipboard.Selection)
             self.clipboard.setText(copy_text[:-1], mode=self.clipboard.Clipboard)
 
-    def send_acknowledgement(self) -> None:
-        """ Send the acknowledge action by sending it to the command topic in the kafka cluster """
-        if not can_take_action(UserAction.ACKNOWLEDGE, log_warning=True):
-            return
-
-        indices = self.alarmView.selectionModel().selectedRows()
-        if len(indices) > 0:
-            for index in indices:
-                alarm_item = list(self.alarmModel.alarm_items.items())[index.row()][1]
-                username = getpass.getuser()
-                hostname = socket.gethostname()
-                for alarm_path in self.tree_model.added_paths[alarm_item.name]:
-                    self.kafka_producer.send(self.topic + 'Command',
-                                             key=f'command:{alarm_path}',
-                                             value={'user': username, 'host': hostname, 'command': 'acknowledge'})
-
-    def send_unacknowledgement(self) -> None:
-        """ Send the un-acknowledge action by sending it to the command topic in the kafka cluster """
+    def send_acknowledge_action(self, acknowledged: bool) -> None:
+        """ Send the input action by sending it to the command topic in the kafka cluster """
         if not can_take_action(UserAction.ACKNOWLEDGE, log_warning=True):
             return
 
-        indices = self.alarmView.selectionModel().selectedRows()
+        indices = self.get_selected_indices()
         if len(indices) > 0:
             for index in indices:
                 alarm_item = list(self.alarmModel.alarm_items.items())[index.row()][1]
                 username = getpass.getuser()
                 hostname = socket.gethostname()
-                for alarm_path in self.tree_model.added_paths[alarm_item.name]:
-                    self.kafka_producer.send(self.topic + 'Command',
-                                             key=f'command:{alarm_path}',
-                                             value={'user': username, 'host': hostname, 'command': 'unacknowledge'})
+                if alarm_item.name not in self.tree_model.added_paths:
+                    # Alarm is no longer valid, send a None value to delete it from kafka
+                    self.kafka_producer.send(self.topic,
+                                             key=f'state:{alarm_item.path}',
+                                             value=None)
+                else:
+                    command_to_send = 'acknowledge' if acknowledged else 'unacknowledge'
+                    for alarm_path in self.tree_model.added_paths[alarm_item.name]:
+                        self.kafka_producer.send(self.topic + 'Command',
+                                                 key=f'command:{alarm_path}',
+                                                 value={'user': username, 'host': hostname, 'command': command_to_send})
+        self.alarmView.selectionModel().reset()
```

### Comparing `slac-alarm-manager-1.2.0/slam/alarm_tree_model.py` & `slac-alarm-manager-1.2.1/slam/alarm_tree_model.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/slam/alarm_tree_view.py` & `slac-alarm-manager-1.2.1/slam/alarm_tree_view.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/slam/archive_search.py` & `slac-alarm-manager-1.2.1/slam/archive_search.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/slam/kafka_reader.py` & `slac-alarm-manager-1.2.1/slam/kafka_reader.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/slam/main_window.py` & `slac-alarm-manager-1.2.1/slam/main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,16 +204,20 @@
         elif key.startswith('command'):
             pass  # Nothing for us to do
         elif key.startswith('state'):
             pv = message.key.split('/')[-1]
             alarm_config_name = key.split('/')[1]
             self.last_received_update_time[alarm_config_name] = datetime.now()
             logger.debug(f'Processing STATE message with key: {message.key} and values: {message.value}')
-            if values is None or len(values) <= 2:
-                return  # This is either a misconfigured message, or the heartbeat message which doesn't get recorded
+            if values is None:
+                self.active_alarm_tables[alarm_config_name].alarmModel.remove_row(message.key[6:].split('/')[-1])
+                self.acknowledged_alarm_tables[alarm_config_name].alarmModel.remove_row(message.key[6:].split('/')[-1])
+                return
+            if len(values) <= 2:
+                return  # This is the heartbeat message which doesn't get recorded
             time = ''
             if 'time' in values:
                 time = datetime.fromtimestamp(values['time']['seconds'])
             self.alarm_update_signal.emit(alarm_config_name, pv, message.key[6:], AlarmSeverity(values['severity']),
                                           values['message'], time, values['value'],
                                           AlarmSeverity(values['current_severity']), values['current_message'])
```

### Comparing `slac-alarm-manager-1.2.0/slam/permissions.py` & `slac-alarm-manager-1.2.1/slam/permissions.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.0/slam_launcher/main.py` & `slac-alarm-manager-1.2.1/slam_launcher/main.py`

 * *Files identical despite different names*

