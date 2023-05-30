# Comparing `tmp/pdfgpt-0.2.0.tar.gz` & `tmp/pdfgpt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfgpt-0.2.0.tar", last modified: Tue May 30 20:40:02 2023, max compression
+gzip compressed data, was "pdfgpt-0.2.1.tar", last modified: Tue May 30 21:49:33 2023, max compression
```

## Comparing `pdfgpt-0.2.0.tar` & `pdfgpt-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.140155 pdfgpt-0.2.0/
--rw-rw-rw-   0        0        0     3643 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1099 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2819 2023-05-30 20:40:02.140155 pdfgpt-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1926 2023-05-30 07:43:54.000000 pdfgpt-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.039280 pdfgpt-0.2.0/docs/
--rw-rw-rw-   0        0        0      627 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/authors.rst
--rw-rw-rw-   0        0        0     4945 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/history.rst
--rw-rw-rw-   0        0        0      323 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/index.rst
--rw-rw-rw-   0        0        0     1161 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/installation.rst
--rwxrwxrwx   0        0        0      804 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/readme.rst
--rw-rw-rw-   0        0        0       74 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.059438 pdfgpt-0.2.0/pdfgpt/
--rw-rw-rw-   0        0        0      167 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/pdfgpt/__init__.py
--rw-rw-rw-   0        0        0      412 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/pdfgpt/cli.py
--rw-rw-rw-   0        0        0     7224 2023-05-30 20:36:57.000000 pdfgpt-0.2.0/pdfgpt/pdfgpt.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.099419 pdfgpt-0.2.0/pdfgpt.egg-info/
--rw-rw-rw-   0        0        0     2819 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       77 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      401 2023-05-30 20:40:02.143378 pdfgpt-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1571 2023-05-30 15:55:03.000000 pdfgpt-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.139149 pdfgpt-0.2.0/tests/
--rw-rw-rw-   0        0        0       37 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0  3340858 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/tests/epanet_matlab_toolkit.pdf
--rw-rw-rw-   0        0        0      690 2023-05-30 20:33:58.000000 pdfgpt-0.2.0/tests/test_example.py
--rw-rw-rw-   0        0        0      878 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/tests/test_pdfgpt.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.267344 pdfgpt-0.2.1/
+-rw-rw-rw-   0        0        0     3643 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1099 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3643 2023-05-30 21:49:33.267810 pdfgpt-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2730 2023-05-30 21:46:51.000000 pdfgpt-0.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.211587 pdfgpt-0.2.1/docs/
+-rw-rw-rw-   0        0        0      627 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     4945 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/history.rst
+-rw-rw-rw-   0        0        0      323 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/index.rst
+-rw-rw-rw-   0        0        0     1161 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/installation.rst
+-rwxrwxrwx   0        0        0      804 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/readme.rst
+-rw-rw-rw-   0        0        0       74 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.221265 pdfgpt-0.2.1/pdfgpt/
+-rw-rw-rw-   0        0        0      167 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/pdfgpt/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/pdfgpt/cli.py
+-rw-rw-rw-   0        0        0     7855 2023-05-30 21:46:31.000000 pdfgpt-0.2.1/pdfgpt/pdfgpt.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.245602 pdfgpt-0.2.1/pdfgpt.egg-info/
+-rw-rw-rw-   0        0        0     3643 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-30 21:49:33.000000 pdfgpt-0.2.1/pdfgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 21:48:24.000000 pdfgpt-0.2.1/pdfgpt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       77 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 21:49:32.000000 pdfgpt-0.2.1/pdfgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      401 2023-05-30 21:49:33.271453 pdfgpt-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1571 2023-05-30 21:06:39.000000 pdfgpt-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:49:33.265335 pdfgpt-0.2.1/tests/
+-rw-rw-rw-   0        0        0       37 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0  3340858 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/tests/epanet_matlab_toolkit.pdf
+-rw-rw-rw-   0        0        0      697 2023-05-30 20:47:17.000000 pdfgpt-0.2.1/tests/test_example.py
+-rw-rw-rw-   0        0        0      878 2023-05-15 15:58:02.000000 pdfgpt-0.2.1/tests/test_pdfgpt.py
```

### Comparing `pdfgpt-0.2.0/CONTRIBUTING.rst` & `pdfgpt-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.0/LICENSE` & `pdfgpt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.0/PKG-INFO` & `pdfgpt-0.2.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: pdfgpt
-Version: 0.2.0
-Summary: pdfgpt is a Python package that provides users with the ability to engage in natural language conversations with their PDF documents.
-Home-page: https://github.com/Mariosmsk/pdfgpt
-Author: Marios S. Kyriakou
-Author-email: kiriakou.marios@ucy.ac.cy
-License: MIT license
-Keywords: pdfgpt
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-License-File: LICENSE
-
 ======
 pdfgpt
 ======
 
 
 .. image:: https://img.shields.io/pypi/v/pdfgpt.svg
         :target: https://pypi.python.org/pypi/pdfgpt
@@ -59,44 +39,48 @@
 .. code-block:: python
 
     from pdfgpt import *
 
     d = PDFBot(openai_key='OPENAI_KEY')
 
     print('Example')
-    extracted_text, num_pages = d.generateText(file_path='PDF_NAME.pdf')
+    extracted_text, num_pages = d.generateText(file_path='tests/epanet_matlab_toolkit.pdf')
     df = d.generateEmbeddings(extracted_text)
 
-    print('USER')
-    prompt = d.generatePrompt(df, num_pages, 'what is the epanet?')
-    response = d.sendPrompt(prompt)
+    print('USER: What is EPANET?')
+    prompt = d.generatePrompt(df, num_pages, 'What is EPANET?')
+    response = d.sendPrompt(prompt, model="gpt-3.5-turbo")
     print('AI')
-    print(response)
+    print(response, '\n')
+
+What is EPANET?
+
+EPANET is a software for modeling water distribution systems' hydraulic and quality dynamics, initially developed by the US Environmental Protection Agency in the C programming language in 1994. It uses a geometric representation of the pipe network, along with a set of initial conditions, rules of operation, and uses this information to compute flows, pressures, and water quality throughout the network, for a certain period of time.
 
-    print('USER')
-    prompt = d.generatePrompt(df, num_pages, 'Give me an example get the node elevations with matlab code?')
-    response = d.sendPrompt(prompt)
+.. code-block:: python
+
+    print('USER: Give me the command to load a network?')
+    prompt = d.generatePrompt(df, num_pages, 'Give me the command to load a network?')
+    response = d.sendPrompt(prompt, model="gpt-3.5-turbo", temperature=0.9)
     print('AI')
     print(response)
 
+What is the command to load a network?
+
+The command to load a network is:
+
+G = epanet( ’BWSN_Network_1 .inp’);%Load EPANET Input file
+
+G.loadMSXFile( ’Arsenite .msx’);%Load MSX file
+
 Features
 --------
 
 * TODO
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-
-
-=======
-History
-=======
-
-0.1.0 (2023-05-11)
-------------------
-
-* First release on PyPI.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pdfgpt-0.2.0/docs/Makefile` & `pdfgpt-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.0/docs/conf.py` & `pdfgpt-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.0/docs/installation.rst` & `pdfgpt-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.0/docs/make.bat` & `pdfgpt-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.0/pdfgpt/pdfgpt.py` & `pdfgpt-0.2.1/pdfgpt/pdfgpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pypdf import PdfReader
 from openai.embeddings_utils import get_embedding, cosine_similarity
 
 
 class PDFBot:
 
     def __init__(self, openai_key):
+        self.filename = 'embedding data'
         openai.api_key = openai_key
         self.slice_stop = 20000
 
     # Extract text from PDFs
     def generateText(self, file_path=None, df=None):
         if df is not None:
             extracted_text, num_pages = self.extract_any_text(df)
@@ -117,31 +118,53 @@
         similarities = cosine_similarity(df.embeddings.tolist(), query_embedding)
         result_indices = similarities.argsort()[::-1][:num_pages]
         # df[0].array[0] = df[0].array[0][:4000]
         result = df.iloc[result_indices]
         min_len = min(result['text_length'][0:3])
         if min_len > 4000:
             min_len = 4000
+        try:
+            if len(result) == 1:
+                res1 = result.iloc[0][0][:7000]
+            else:
+                res1 = result.iloc[0][0][:4000]
+
+        except:
+            res1 = result.iloc[0][0][:min_len]
 
         if len(result) == 1:
             prompt = f"""Given the question: {message} and the following embeddings as data:
-                               1. {result.iloc[0][0][:min_len]}
+                               1. {res1}
                            Give an answer based only on the data where I provide or return \"Not specified\".
                            """
         elif len(result) == 2:
+            try:
+                if min_len < 2000:
+                    res2 = result.iloc[1][0][:4000 - min_len]
+                else:
+                    res2 = result.iloc[1][0][:3500]
+            except:
+                res2 = result.iloc[1][0][:min_len]
             prompt = f"""Given the question: {message} and the following embeddings as data:
-                               1. {result.iloc[0][0][:min_len]}
-                               2. {result.iloc[1][0][:min_len-500]}
+                               1. {res1}
+                               2. {res2}
                            Give an answer based only on the data where I provide or return \"Not specified\".
                            """
         else:
+            try:
+                if min_len < 1000:
+                    res3 = result.iloc[2][0][:1000 - min_len]
+                else:
+                    res3 = result.iloc[2][0][:500]
+            except:
+                res3 = result.iloc[2][0][:min_len]
             prompt = f"""Given the question: {message} and the following embeddings as data:
-                               1. {result.iloc[0][0][:min_len]}
-                               2. {result.iloc[1][0][:min_len-500]}
-                               3. {result.iloc[2][0][:min_len-3500]}
+                               1. {res1}
+                               2. {res2}
+                               3. {res3}
                            Give an answer based only on the data where I provide or return \"Not specified\".
                            """
         return prompt
 
     # Sends a prompt to the OpenAI API and return the response
     def sendPrompt(self, prompt, model="gpt-3.5-turbo", temperature=0.9, max_tokens=1500):
```

### Comparing `pdfgpt-0.2.0/pdfgpt.egg-info/SOURCES.txt` & `pdfgpt-0.2.1/pdfgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.0/setup.py` & `pdfgpt-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     include_package_data=True,
     keywords='pdfgpt',
     name='pdfgpt',
     packages=find_packages(include=['pdfgpt', 'pdfgpt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Mariosmsk/pdfgpt',
-    version='0.2.0',
+    version='0.2.1',
     zip_safe=False,
 )
```

### Comparing `pdfgpt-0.2.0/tests/epanet_matlab_toolkit.pdf` & `pdfgpt-0.2.1/tests/epanet_matlab_toolkit.pdf`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.2.0/tests/test_example.py` & `pdfgpt-0.2.1/tests/test_example.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 
 print('USER: What is EPANET?')
 prompt = d.generatePrompt(df, num_pages, 'What is EPANET?')
 response = d.sendPrompt(prompt, model="gpt-3.5-turbo")
 print('AI')
 print(response, '\n')
 
-print('USER: Give me a minimum example code?')
+print('USER: Give me the command to load a network?')
 prompt = d.generatePrompt(df, num_pages, 'Give me the command to load a network?')
 response = d.sendPrompt(prompt, model="gpt-3.5-turbo", temperature=0.9)
 print('AI')
 print(response)
```

### Comparing `pdfgpt-0.2.0/tests/test_pdfgpt.py` & `pdfgpt-0.2.1/tests/test_pdfgpt.py`

 * *Files identical despite different names*

