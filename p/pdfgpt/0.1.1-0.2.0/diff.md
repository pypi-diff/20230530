# Comparing `tmp/pdfgpt-0.1.1.tar.gz` & `tmp/pdfgpt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfgpt-0.1.1.tar", last modified: Wed May 17 12:23:36 2023, max compression
+gzip compressed data, was "pdfgpt-0.2.0.tar", last modified: Tue May 30 20:40:02 2023, max compression
```

## Comparing `pdfgpt-0.1.1.tar` & `pdfgpt-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 12:23:36.193583 pdfgpt-0.1.1/
--rw-rw-rw-   0        0        0     3643 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1099 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1749 2023-05-17 12:23:36.194422 pdfgpt-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      856 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 12:23:36.142238 pdfgpt-0.1.1/docs/
--rw-rw-rw-   0        0        0      627 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/authors.rst
--rw-rw-rw-   0        0        0     4945 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/history.rst
--rw-rw-rw-   0        0        0      323 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/index.rst
--rw-rw-rw-   0        0        0     1161 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/installation.rst
--rwxrwxrwx   0        0        0      804 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/readme.rst
--rw-rw-rw-   0        0        0       74 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 12:23:36.155250 pdfgpt-0.1.1/pdfgpt/
--rw-rw-rw-   0        0        0      167 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/pdfgpt/__init__.py
--rw-rw-rw-   0        0        0      412 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/pdfgpt/cli.py
--rw-rw-rw-   0        0        0     5031 2023-05-17 10:43:05.000000 pdfgpt-0.1.1/pdfgpt/pdfgpt.py
-drwxrwxrwx   0        0        0        0 2023-05-17 12:23:36.180268 pdfgpt-0.1.1/pdfgpt.egg-info/
--rw-rw-rw-   0        0        0     1749 2023-05-17 12:23:35.000000 pdfgpt-0.1.1/pdfgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-17 12:23:36.000000 pdfgpt-0.1.1/pdfgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 12:23:35.000000 pdfgpt-0.1.1/pdfgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-17 12:23:35.000000 pdfgpt-0.1.1/pdfgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 12:23:35.000000 pdfgpt-0.1.1/pdfgpt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-05-17 12:23:35.000000 pdfgpt-0.1.1/pdfgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-17 12:23:35.000000 pdfgpt-0.1.1/pdfgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      401 2023-05-17 12:23:36.197334 pdfgpt-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1560 2023-05-17 12:22:34.000000 pdfgpt-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 12:23:36.192582 pdfgpt-0.1.1/tests/
--rw-rw-rw-   0        0        0       37 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0  3340858 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/tests/epanet_matlab_toolkit.pdf
--rw-rw-rw-   0        0        0      556 2023-05-17 10:45:34.000000 pdfgpt-0.1.1/tests/test_example.py
--rw-rw-rw-   0        0        0      878 2023-05-15 15:58:02.000000 pdfgpt-0.1.1/tests/test_pdfgpt.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.140155 pdfgpt-0.2.0/
+-rw-rw-rw-   0        0        0     3643 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1099 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2819 2023-05-30 20:40:02.140155 pdfgpt-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1926 2023-05-30 07:43:54.000000 pdfgpt-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.039280 pdfgpt-0.2.0/docs/
+-rw-rw-rw-   0        0        0      627 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4945 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/history.rst
+-rw-rw-rw-   0        0        0      323 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1161 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      804 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/readme.rst
+-rw-rw-rw-   0        0        0       74 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.059438 pdfgpt-0.2.0/pdfgpt/
+-rw-rw-rw-   0        0        0      167 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/pdfgpt/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/pdfgpt/cli.py
+-rw-rw-rw-   0        0        0     7224 2023-05-30 20:36:57.000000 pdfgpt-0.2.0/pdfgpt/pdfgpt.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.099419 pdfgpt-0.2.0/pdfgpt.egg-info/
+-rw-rw-rw-   0        0        0     2819 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       77 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 20:40:01.000000 pdfgpt-0.2.0/pdfgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      401 2023-05-30 20:40:02.143378 pdfgpt-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1571 2023-05-30 15:55:03.000000 pdfgpt-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:40:02.139149 pdfgpt-0.2.0/tests/
+-rw-rw-rw-   0        0        0       37 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0  3340858 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/tests/epanet_matlab_toolkit.pdf
+-rw-rw-rw-   0        0        0      690 2023-05-30 20:33:58.000000 pdfgpt-0.2.0/tests/test_example.py
+-rw-rw-rw-   0        0        0      878 2023-05-15 15:58:02.000000 pdfgpt-0.2.0/tests/test_pdfgpt.py
```

### Comparing `pdfgpt-0.1.1/CONTRIBUTING.rst` & `pdfgpt-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.1.1/LICENSE` & `pdfgpt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.1.1/docs/Makefile` & `pdfgpt-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.1.1/docs/conf.py` & `pdfgpt-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.1.1/docs/installation.rst` & `pdfgpt-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.1.1/docs/make.bat` & `pdfgpt-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.1.1/pdfgpt/pdfgpt.py` & `pdfgpt-0.2.0/pdfgpt/pdfgpt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,34 @@
 """Main module."""
+import os
 import openai
+import tiktoken
+import textwrap
 import pandas as pd
 from pypdf import PdfReader
 from openai.embeddings_utils import get_embedding, cosine_similarity
 
 
-def split_text_to_pages(text, max_length=2000):
-    pages = []
-    current_page = ''
-    for line in text.split('\n'):
-        if len(current_page) + len(line) + 1 > max_length:
-            pages.append(current_page.strip())
-            current_page = ''
-        current_page += line + '\n'
-    if current_page:
-        pages.append(current_page.strip())
-    return pages
-
-
-def extract_any_text(df):
-    string_columns = list(df.keys())
-    text_column = df[string_columns].apply(lambda x: ' '.join([str(x[col]) for col in x.index]), axis=1)
-    extracted_text = ' '.join(text_column.tolist())
-    extracted_text = split_text_to_pages(extracted_text)
-    extracted_text = [{'text': page_text} for page_text in extracted_text if page_text.strip() != '']
-    num_pages = len(extracted_text)
-    return extracted_text, num_pages
-
-
 class PDFBot:
 
     def __init__(self, openai_key):
         openai.api_key = openai_key
-        self.cnt = 4000
+        self.slice_stop = 20000
 
     # Extract text from PDFs
     def generateText(self, file_path=None, df=None):
-        extracted_text = []
         if df is not None:
-            extracted_text, num_pages = extract_any_text(df)
+            extracted_text, num_pages = self.extract_any_text(df)
             return extracted_text, num_pages
 
+        self.filename = os.path.basename(file_path)
+
         pdf_document = PdfReader(file_path)
         num_pages = len(pdf_document.pages)
-
+        extracted_text = ''
         for page_num in range(num_pages):
             processed_text = []
             current_font_size = None
             current_blob_text = ''
             page = pdf_document.pages[page_num]
             page_text = page.extract_text()
             page_text = [
@@ -69,48 +50,112 @@
                     if current_font_size is not None and len(current_blob_text) >= 1:
                         processed_text.append({
                             'font_size': current_font_size,
                             'text': current_blob_text,
                             'page': page_num
                         })
                     current_font_size = text['font_size']
-                    current_blob_text = text['text']
-            extracted_text += processed_text
+                    current_blob_text = current_blob_text
+            extracted_text += text['text']
+        text_chunks = self.generateChunkText(extracted_text)
+        return text_chunks, num_pages
+
+    def split_text_to_pages(self, text):
+        extracted_text = textwrap.wrap(text, width=self.slice_stop)
+        return extracted_text
+
+    def extract_any_text(self, df):
+        string_columns = list(df.keys())
+        text_column = df[string_columns].apply(lambda x: ' '.join([str(x[col]) for col in x.index]), axis=1)
+        extracted_text = ' '.join(text_column.tolist())
+        extracted_text = self.split_text_to_pages(extracted_text)
+        # extracted_text = [{'text': page_text} for page_text in extracted_text if page_text.strip() != '']
+        num_pages = len(extracted_text)
         return extracted_text, num_pages
 
+    def generateChunkText(self, extracted_text):
+        # Initialise tokenizer
+        tokenizer = tiktoken.get_encoding("cl100k_base")
+        chunks = self.create_chunks(extracted_text, 1000, tokenizer)
+        text_chunks = [tokenizer.decode(chunk) for chunk in chunks]
+        return text_chunks
+
+    ###################################################
+    # Source: Openai - https://github.com/openai/openai-cookbook
+    # Split a text into smaller chunks of size n, preferably ending at the end of a sentence
+    def create_chunks(self, text, n, tokenizer):
+        tokens = tokenizer.encode(text)
+        """Yield successive n-sized chunks from text."""
+        i = 0
+        while i < len(tokens):
+            # Find the nearest end of sentence within a range of 0.5 * n and 1.5 * n tokens
+            j = min(i + int(1.5 * n), len(tokens))
+            while j > i + int(0.5 * n):
+                # Decode the tokens and check for full stop or newline
+                chunk = tokenizer.decode(tokens[i:j])
+                if chunk.endswith(".") or chunk.endswith("\n"):
+                    break
+                j -= 1
+            # If no end of sentence found, use n tokens as the chunk size
+            if j == i + int(0.5 * n):
+                j = min(i + n, len(tokens))
+            yield tokens[i:j]
+            i = j
+    ###################################################
+
     # Generate embeddings from PDFs
     def generateEmbeddings(self, extracted_text='', model_embeddings="text-embedding-ada-002"):
-        filtered_text = [row for row in extracted_text if len(row['text']) >= 30]
-        unique_text = [dict(t) for t in {tuple(d.items()) for d in filtered_text}]
-        df = pd.DataFrame(unique_text)
-        df['text'] = df['text'].str.slice(stop=26000)
-        df['text_length'] = df['text'].str.len()
-        embeddings = df.text.apply(lambda x: get_embedding(x, engine=model_embeddings))
+        df = pd.DataFrame(extracted_text)
+        df[0] = df[0].str.slice(stop=self.slice_stop )
+        df['text_length'] = df[0].str.len()
+        embeddings = df[0].apply(lambda x: get_embedding(x, engine=model_embeddings))
         df["embeddings"] = embeddings
         return df
 
-    # Generate prompt based on embeddings
+    # Generate prompt
     def generatePrompt(self, df, num_pages, message, model_embeddings="text-embedding-ada-002"):
         query_embedding = get_embedding(message, engine=model_embeddings)
         similarities = cosine_similarity(df.embeddings.tolist(), query_embedding)
         result_indices = similarities.argsort()[::-1][:num_pages]
-        df['text'].array[0] = df['text'].array[0][:self.cnt]
+        # df[0].array[0] = df[0].array[0][:4000]
         result = df.iloc[result_indices]
-
-        index = min(len(result), 3) - 2
-        len_res = len(result)
-
-        prompt = f"""Given the question: {message} and the following embeddings as data:
-                    1. {result.iloc[index]['text']}
-                    2. {result.iloc[(index + 1) % len_res]['text']}
-                    3. {result.iloc[(index + 2) % len_res]['text']}
-                    Give an answer based only on the data where I provide or return not available information.
-                    """
+        min_len = min(result['text_length'][0:3])
+        if min_len > 4000:
+            min_len = 4000
+
+        if len(result) == 1:
+            prompt = f"""Given the question: {message} and the following embeddings as data:
+                               1. {result.iloc[0][0][:min_len]}
+                           Give an answer based only on the data where I provide or return \"Not specified\".
+                           """
+        elif len(result) == 2:
+            prompt = f"""Given the question: {message} and the following embeddings as data:
+                               1. {result.iloc[0][0][:min_len]}
+                               2. {result.iloc[1][0][:min_len-500]}
+                           Give an answer based only on the data where I provide or return \"Not specified\".
+                           """
+        else:
+            prompt = f"""Given the question: {message} and the following embeddings as data:
+                               1. {result.iloc[0][0][:min_len]}
+                               2. {result.iloc[1][0][:min_len-500]}
+                               3. {result.iloc[2][0][:min_len-3500]}
+                           Give an answer based only on the data where I provide or return \"Not specified\".
+                           """
         return prompt
 
     # Sends a prompt to the OpenAI API and return the response
-    def sendPrompt(self, prompt, model="text-davinci-003", temperature=0.4, max_tokens=1250, frequency_penalty=0.0,
-                   top_p=1, presence_penalty=0.6):
-        response = openai.Completion.create(model=model, prompt=prompt, temperature=temperature,
-                                            max_tokens=max_tokens, top_p=top_p, frequency_penalty=frequency_penalty,
-                                            presence_penalty=presence_penalty)
-        return response.choices[0]['text']
+    def sendPrompt(self, prompt, model="gpt-3.5-turbo", temperature=0.9, max_tokens=1500):
+
+        # response = openai.Completion.create(
+        #     model=model, prompt=prompt, temperature=temperature, max_tokens=max_tokens,
+        #     top_p=top_p, frequency_penalty=frequency_penalty, presence_penalty=presence_penalty)
+
+        response = openai.ChatCompletion.create(
+            messages=[
+                {'role': 'system', 'content': f'You answer questions about the {self.filename}.'},
+                {'role': 'user', 'content': prompt},
+            ],
+            model=model,
+            max_tokens=max_tokens,
+            temperature=temperature,
+        )
+        return response['choices'][0]['message']['content']
```

### Comparing `pdfgpt-0.1.1/pdfgpt.egg-info/SOURCES.txt` & `pdfgpt-0.2.0/pdfgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.1.1/setup.py` & `pdfgpt-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['Click>=7.0', 'openai', 'pandas', 'pypdf', 'matplotlib', 'plotly', 'scipy', 'scikit-learn']
+requirements = ['Click>=7.0', 'openai', 'pandas', 'pypdf', 'matplotlib', 'plotly', 'scipy', 'scikit-learn', 'tiktoken']
 
-test_requirements = [ ]
+test_requirements = []
 
 setup(
     author="Marios S. Kyriakou",
     author_email='kiriakou.marios@ucy.ac.cy',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -41,10 +41,10 @@
     include_package_data=True,
     keywords='pdfgpt',
     name='pdfgpt',
     packages=find_packages(include=['pdfgpt', 'pdfgpt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Mariosmsk/pdfgpt',
-    version='0.1.1',
+    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `pdfgpt-0.1.1/tests/epanet_matlab_toolkit.pdf` & `pdfgpt-0.2.0/tests/epanet_matlab_toolkit.pdf`

 * *Files identical despite different names*

### Comparing `pdfgpt-0.1.1/tests/test_example.py` & `pdfgpt-0.2.0/tests/test_example.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Unit test package for pdfgpt."""
 from pdfgpt import *
 
-d = PDFBot(openai_key='OPENAI_KEY')
+d = PDFBot(openai_key='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')
 
 print('Example')
 extracted_text, num_pages = d.generateText(file_path='epanet_matlab_toolkit.pdf')
 df = d.generateEmbeddings(extracted_text)
 
-print('USER')
-prompt = d.generatePrompt(df, num_pages, 'what is the epanet?')
-response = d.sendPrompt(prompt)
+print('USER: What is EPANET?')
+prompt = d.generatePrompt(df, num_pages, 'What is EPANET?')
+response = d.sendPrompt(prompt, model="gpt-3.5-turbo")
 print('AI')
-print(response)
+print(response, '\n')
 
-print('USER')
-prompt = d.generatePrompt(df, num_pages, 'Give me an example get the node elevations with matlab code?')
-response = d.sendPrompt(prompt)
+print('USER: Give me a minimum example code?')
+prompt = d.generatePrompt(df, num_pages, 'Give me the command to load a network?')
+response = d.sendPrompt(prompt, model="gpt-3.5-turbo", temperature=0.9)
 print('AI')
 print(response)
```

### Comparing `pdfgpt-0.1.1/tests/test_pdfgpt.py` & `pdfgpt-0.2.0/tests/test_pdfgpt.py`

 * *Files identical despite different names*

