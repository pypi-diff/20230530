# Comparing `tmp/time_series_binder-1.0.3.tar.gz` & `tmp/time_series_binder-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\time_series_binder-1.0.3.tar", last modified: Sun May 28 00:35:41 2023, max compression
+gzip compressed data, was "time_series_binder-1.0.4.tar", last modified: Tue May 30 03:45:04 2023, max compression
```

## Comparing `time_series_binder-1.0.3.tar` & `time_series_binder-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:35:41.367470 time_series_binder-1.0.3/
--rw-rw-rw-   0        0        0       96 2023-05-28 00:29:22.000000 time_series_binder-1.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1079 2023-05-28 00:29:26.000000 time_series_binder-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-05-27 11:53:42.000000 time_series_binder-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2048 2023-05-28 00:35:41.363729 time_series_binder-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      945 2023-05-28 00:30:27.000000 time_series_binder-1.0.3/README.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 00:35:41.368968 time_series_binder-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1587 2023-05-28 00:34:48.000000 time_series_binder-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 00:35:41.329758 time_series_binder-1.0.3/time_series_binder.egg-info/
--rw-rw-rw-   0        0        0     2048 2023-05-28 00:35:40.000000 time_series_binder-1.0.3/time_series_binder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-28 00:35:41.000000 time_series_binder-1.0.3/time_series_binder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:35:40.000000 time_series_binder-1.0.3/time_series_binder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-05-28 00:35:40.000000 time_series_binder-1.0.3/time_series_binder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-28 00:35:40.000000 time_series_binder-1.0.3/time_series_binder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 00:35:41.358525 time_series_binder-1.0.3/ts_binder/
--rw-rw-rw-   0        0        0       45 2023-05-27 12:36:11.000000 time_series_binder-1.0.3/ts_binder/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-05-27 13:08:55.000000 time_series_binder-1.0.3/ts_binder/data_processing.py
--rw-rw-rw-   0        0        0     4258 2023-05-27 13:13:03.000000 time_series_binder-1.0.3/ts_binder/forecaster.py
--rw-rw-rw-   0        0        0     3778 2023-05-27 13:31:35.000000 time_series_binder-1.0.3/ts_binder/helpers.py
--rw-rw-rw-   0        0        0     5989 2023-05-27 13:08:52.000000 time_series_binder-1.0.3/ts_binder/trainer.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:45:04.229298 time_series_binder-1.0.4/
+-rw-rw-rw-   0        0        0      172 2023-05-30 03:42:09.000000 time_series_binder-1.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1079 2023-05-29 01:27:30.000000 time_series_binder-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-29 01:27:30.000000 time_series_binder-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2237 2023-05-30 03:45:04.229298 time_series_binder-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      911 2023-05-30 03:43:27.000000 time_series_binder-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 03:45:04.229298 time_series_binder-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1626 2023-05-30 03:43:43.000000 time_series_binder-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:45:04.226300 time_series_binder-1.0.4/time_series_binder.egg-info/
+-rw-rw-rw-   0        0        0     2237 2023-05-30 03:45:04.000000 time_series_binder-1.0.4/time_series_binder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-30 03:45:04.000000 time_series_binder-1.0.4/time_series_binder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 03:45:04.000000 time_series_binder-1.0.4/time_series_binder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-30 03:45:04.000000 time_series_binder-1.0.4/time_series_binder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 03:45:04.000000 time_series_binder-1.0.4/time_series_binder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 03:45:04.228299 time_series_binder-1.0.4/ts_binder/
+-rw-rw-rw-   0        0        0       46 2023-05-29 01:27:30.000000 time_series_binder-1.0.4/ts_binder/__init__.py
+-rw-rw-rw-   0        0        0     5904 2023-05-30 03:40:31.000000 time_series_binder-1.0.4/ts_binder/data_processing.py
+-rw-rw-rw-   0        0        0    11671 2023-05-30 03:40:33.000000 time_series_binder-1.0.4/ts_binder/model_utils.py
+-rw-rw-rw-   0        0        0     2352 2023-05-30 03:40:35.000000 time_series_binder-1.0.4/ts_binder/visualize.py
```

### Comparing `time_series_binder-1.0.3/LICENSE.txt` & `time_series_binder-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `time_series_binder-1.0.3/PKG-INFO` & `time_series_binder-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: time_series_binder
-Version: 1.0.3
+Version: 1.0.4
 Summary: Time Series Binder is a Python library for time series analysis and forecasting. It offers a comprehensive set of tools and models, including Pandas integration, statistical methods, neural networks with Keras, and the NeuralProphet library. With Time Series Binder, you can easily manipulate, visualize, and predict time series data, making it an essential toolkit for researchers and analysts.
 Home-page: https://github.com/JhunBrian/time_series_binder
 Author: Jhun Brian Andam
 Author-email: brianandam123@gmail.com
 License: MIT
+Description: # Time Series Binder
+        
+        Time Series Binder is a Python library for time series analysis and forecasting. It provides a comprehensive set of tools and models to manipulate, visualize, and predict time series data. This library is designed to assist researchers and analysts in performing various time series tasks with ease and efficiency.
+        
+        ## Features
+        
+        - Integration with Pandas for seamless data manipulation and preprocessing.
+        - Statistical methods for analyzing time series data, including trend analysis, seasonality decomposition, and outlier detection.
+        - Neural network models powered by Keras for advanced time series forecasting.
+        - Integration with the NeuralProphet library for additional forecasting capabilities.
+        - Visualization tools for creating insightful plots and visual representations of time series data.
+        - Integration with scikit-learn for additional machine learning functionality.
+        
+        Change Log
+        ==================
+        
+        1.0.4 (30/05/2023)
+        ------------------
+        - Modified Documentation
+        - Modified classes to adapt ANN model.
+        - Created `model_utils` package.
 Keywords: Time Series Analysis,Forecasting
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Time Series Binder
-
-Time Series Binder is a Python library for time series analysis and forecasting. It provides a comprehensive set of tools and models to manipulate, visualize, and predict time series data. This library is designed to assist researchers and analysts in performing various time series tasks with ease and efficiency.
-
-## Features
-
-- Integration with Pandas for seamless data manipulation and preprocessing.
-- Statistical methods for analyzing time series data, including trend analysis, seasonality decomposition, and outlier detection.
-- Neural network models powered by Keras for advanced time series forecasting.
-- Integration with the NeuralProphet library for additional forecasting capabilities.
-- Visualization tools for creating insightful plots and visual representations of time series data.
-- Integration with scikit-learn for additional machine learning functionality.
-
-
-## Import
-
-`from ts_binder import tariner`
-
-Change Log
-==================
-
-1.0.3 (27/05/2023)
-------------------
-Modified Documentation
```

### Comparing `time_series_binder-1.0.3/README.txt` & `time_series_binder-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-# Time Series Binder
-
-Time Series Binder is a Python library for time series analysis and forecasting. It provides a comprehensive set of tools and models to manipulate, visualize, and predict time series data. This library is designed to assist researchers and analysts in performing various time series tasks with ease and efficiency.
-
-## Features
-
-- Integration with Pandas for seamless data manipulation and preprocessing.
-- Statistical methods for analyzing time series data, including trend analysis, seasonality decomposition, and outlier detection.
-- Neural network models powered by Keras for advanced time series forecasting.
-- Integration with the NeuralProphet library for additional forecasting capabilities.
-- Visualization tools for creating insightful plots and visual representations of time series data.
-- Integration with scikit-learn for additional machine learning functionality.
-
-
-## Import
-
-`from ts_binder import tariner`
+# Time Series Binder
+
+Time Series Binder is a Python library for time series analysis and forecasting. It provides a comprehensive set of tools and models to manipulate, visualize, and predict time series data. This library is designed to assist researchers and analysts in performing various time series tasks with ease and efficiency.
+
+## Features
+
+- Integration with Pandas for seamless data manipulation and preprocessing.
+- Statistical methods for analyzing time series data, including trend analysis, seasonality decomposition, and outlier detection.
+- Neural network models powered by Keras for advanced time series forecasting.
+- Integration with the NeuralProphet library for additional forecasting capabilities.
+- Visualization tools for creating insightful plots and visual representations of time series data.
+- Integration with scikit-learn for additional machine learning functionality.
```

### Comparing `time_series_binder-1.0.3/setup.py` & `time_series_binder-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from setuptools import setup, find_packages
- 
-# python setup.py sdist bdist_wheel
-# twine check dist/*
-# twine upload --repository-url https://upload.pypi.org/legacy/ dist/*
-
-classifiers = [
-  'Development Status :: 1 - Planning',
-  'Intended Audience :: Education',
-  'Operating System :: Microsoft :: Windows :: Windows 10',
-  'License :: OSI Approved :: MIT License',
-  'Programming Language :: Python :: 3'
-]
-
-desc = """Time Series Binder is a Python library for time series analysis and forecasting. It offers a comprehensive set of tools and models, including Pandas integration, statistical methods, neural networks with Keras, and the NeuralProphet library. With Time Series Binder, you can easily manipulate, visualize, and predict time series data, making it an essential toolkit for researchers and analysts."""
- 
-dependencies = ['pandas', 
-                'numpy', 
-                'matplotlib', 
-                'statsmodels', 
-                'keras', 
-                'neuralprophet', 
-                'scikit-learn', 
-                'tqdm', 
-                'tabulate']
-
-setup(
-  name='time_series_binder',
-  version='1.0.3',
-  description=desc,
-  long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
-  long_description_content_type='text/markdown',
-  url='https://github.com/JhunBrian/time_series_binder',  
-  author='Jhun Brian Andam',
-  author_email='brianandam123@gmail.com',
-  license='MIT', 
-  classifiers=classifiers,
-  keywords=['Time Series Analysis', 'Forecasting'], 
-  packages=find_packages(),
-  install_requires=dependencies
+from setuptools import setup, find_packages
+ 
+# python setup.py sdist bdist_wheel
+# twine check dist/*
+# twine upload --repository-url https://upload.pypi.org/legacy/ dist/*
+
+classifiers = [
+  'Development Status :: 1 - Planning',
+  'Intended Audience :: Education',
+  'Operating System :: Microsoft :: Windows :: Windows 10',
+  'License :: OSI Approved :: MIT License',
+  'Programming Language :: Python :: 3'
+]
+
+desc = """Time Series Binder is a Python library for time series analysis and forecasting. It offers a comprehensive set of tools and models, including Pandas integration, statistical methods, neural networks with Keras, and the NeuralProphet library. With Time Series Binder, you can easily manipulate, visualize, and predict time series data, making it an essential toolkit for researchers and analysts."""
+ 
+dependencies = ['pandas', 
+                'numpy', 
+                'matplotlib', 
+                'statsmodels', 
+                'keras', 
+                'neuralprophet', 
+                'scikit-learn', 
+                'tqdm', 
+                'tabulate']
+
+setup(
+  name='time_series_binder',
+  version='1.0.4',
+  description=desc,
+  long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
+  long_description_content_type='text/markdown',
+  url='https://github.com/JhunBrian/time_series_binder',  
+  author='Jhun Brian Andam',
+  author_email='brianandam123@gmail.com',
+  license='MIT', 
+  classifiers=classifiers,
+  keywords=['Time Series Analysis', 'Forecasting'], 
+  packages=find_packages(),
+  install_requires=dependencies
 )
```

### Comparing `time_series_binder-1.0.3/time_series_binder.egg-info/PKG-INFO` & `time_series_binder-1.0.4/time_series_binder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 Metadata-Version: 2.1
 Name: time-series-binder
-Version: 1.0.3
+Version: 1.0.4
 Summary: Time Series Binder is a Python library for time series analysis and forecasting. It offers a comprehensive set of tools and models, including Pandas integration, statistical methods, neural networks with Keras, and the NeuralProphet library. With Time Series Binder, you can easily manipulate, visualize, and predict time series data, making it an essential toolkit for researchers and analysts.
 Home-page: https://github.com/JhunBrian/time_series_binder
 Author: Jhun Brian Andam
 Author-email: brianandam123@gmail.com
 License: MIT
+Description: # Time Series Binder
+        
+        Time Series Binder is a Python library for time series analysis and forecasting. It provides a comprehensive set of tools and models to manipulate, visualize, and predict time series data. This library is designed to assist researchers and analysts in performing various time series tasks with ease and efficiency.
+        
+        ## Features
+        
+        - Integration with Pandas for seamless data manipulation and preprocessing.
+        - Statistical methods for analyzing time series data, including trend analysis, seasonality decomposition, and outlier detection.
+        - Neural network models powered by Keras for advanced time series forecasting.
+        - Integration with the NeuralProphet library for additional forecasting capabilities.
+        - Visualization tools for creating insightful plots and visual representations of time series data.
+        - Integration with scikit-learn for additional machine learning functionality.
+        
+        Change Log
+        ==================
+        
+        1.0.4 (30/05/2023)
+        ------------------
+        - Modified Documentation
+        - Modified classes to adapt ANN model.
+        - Created `model_utils` package.
 Keywords: Time Series Analysis,Forecasting
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Time Series Binder
-
-Time Series Binder is a Python library for time series analysis and forecasting. It provides a comprehensive set of tools and models to manipulate, visualize, and predict time series data. This library is designed to assist researchers and analysts in performing various time series tasks with ease and efficiency.
-
-## Features
-
-- Integration with Pandas for seamless data manipulation and preprocessing.
-- Statistical methods for analyzing time series data, including trend analysis, seasonality decomposition, and outlier detection.
-- Neural network models powered by Keras for advanced time series forecasting.
-- Integration with the NeuralProphet library for additional forecasting capabilities.
-- Visualization tools for creating insightful plots and visual representations of time series data.
-- Integration with scikit-learn for additional machine learning functionality.
-
-
-## Import
-
-`from ts_binder import tariner`
-
-Change Log
-==================
-
-1.0.3 (27/05/2023)
-------------------
-Modified Documentation
```

