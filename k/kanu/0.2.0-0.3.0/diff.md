# Comparing `tmp/kanu-0.2.0.tar.gz` & `tmp/kanu-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanu-0.2.0.tar", last modified: Fri May 26 22:21:10 2023, max compression
+gzip compressed data, was "kanu-0.3.0.tar", last modified: Tue May 30 07:11:15 2023, max compression
```

## Comparing `kanu-0.2.0.tar` & `kanu-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-26 22:21:10.800472 kanu-0.2.0/
--rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-05-26 22:20:47.000000 kanu-0.2.0/LICENSE
--rw-r--r--   0 sbslee     (501) staff       (20)      346 2023-05-26 22:21:10.800325 kanu-0.2.0/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      382 2023-05-26 22:20:47.000000 kanu-0.2.0/README.md
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-26 22:21:10.799536 kanu-0.2.0/kanu/
--rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/__init__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     3639 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/__main__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     2582 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/chatgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)     6218 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/docgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-05-26 22:20:47.000000 kanu-0.2.0/kanu/version.py
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-26 22:21:10.800147 kanu-0.2.0/kanu.egg-info/
--rw-r--r--   0 sbslee     (501) staff       (20)      346 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      250 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/SOURCES.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/dependency_links.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/entry_points.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-05-26 22:21:10.000000 kanu-0.2.0/kanu.egg-info/top_level.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-05-26 22:21:10.800511 kanu-0.2.0/setup.cfg
--rw-r--r--   0 sbslee     (501) staff       (20)      567 2023-05-26 22:20:47.000000 kanu-0.2.0/setup.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-30 07:11:15.489367 kanu-0.3.0/
+-rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-05-30 07:11:03.000000 kanu-0.3.0/LICENSE
+-rw-r--r--   0 sbslee     (501) staff       (20)      737 2023-05-30 07:11:15.489215 kanu-0.3.0/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      421 2023-05-30 07:11:03.000000 kanu-0.3.0/README.md
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-30 07:11:15.488401 kanu-0.3.0/kanu/
+-rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/__init__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     5278 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/__main__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     1847 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/chatgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     6858 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/docgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)      828 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/utils.py
+-rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-05-30 07:11:03.000000 kanu-0.3.0/kanu/version.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-05-30 07:11:15.489021 kanu-0.3.0/kanu.egg-info/
+-rw-r--r--   0 sbslee     (501) staff       (20)      737 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      264 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/entry_points.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-05-30 07:11:15.000000 kanu-0.3.0/kanu.egg-info/top_level.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-05-30 07:11:15.489413 kanu-0.3.0/setup.cfg
+-rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-05-30 07:11:03.000000 kanu-0.3.0/setup.py
```

### Comparing `kanu-0.2.0/LICENSE` & `kanu-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kanu-0.2.0/kanu/docgpt.py` & `kanu-0.3.0/kanu/docgpt.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,134 @@
 import os
 import tkinter as tk
 from tkinter import filedialog
 
 from langchain.embeddings.openai import OpenAIEmbeddings
-from langchain.text_splitter import CharacterTextSplitter
+from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores import Chroma
-from langchain.llms import OpenAI
-from langchain.document_loaders import TextLoader
+from langchain.chat_models import ChatOpenAI
 from langchain.chains import RetrievalQA
 
+from langchain.document_loaders import (
+    TextLoader,
+    PDFMinerLoader,
+    UnstructuredWordDocumentLoader
+)
+
+from .utils import Tooltip
+
+DOCUMENT_LOADERS = {
+    ".txt": TextLoader,
+    ".pdf": PDFMinerLoader,
+    ".doc": UnstructuredWordDocumentLoader,
+    ".docx": UnstructuredWordDocumentLoader,
+}
+
 class DocGPT:
-    def __init__(self, kanu, openai_key):
+    def __init__(self, kanu, openai_key, model):
         self.kanu = kanu
+        self.model = model
         os.environ["OPENAI_API_KEY"] = openai_key
 
     def run(self):
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
-        label = tk.Label(self.kanu.container, text="DocGPT")
-        label.grid(row=0, column=0, columnspan=3)
-        back_button = tk.Button(self.kanu.container, text="Go back", command=lambda: self.kanu.docgpt_config())
-        back_button.grid(row=1, column=0)
-        back_button = tk.Button(self.kanu.container, text="Reload", command=lambda: self.run())
-        back_button.grid(row=1, column=2)
-        label = tk.Message(self.kanu.container, width=300, text="Option 1. Create a new database")
-        label.grid(row=2, column=0, columnspan=3)
-        f = tk.Label(self.kanu.container, text="Document:")
-        f.grid(row=3, column=0) 
-        self.document_label = tk.Label(self.kanu.container, text="No file selected", fg="red")
+        l = tk.Label(self.kanu.container, text="DocGPT")
+        l.grid(row=0, column=0, columnspan=3)
+        b = tk.Button(self.kanu.container, text="Go back", command=lambda: self.kanu.config_docgpt())
+        b.grid(row=1, column=0)
+        b = tk.Button(self.kanu.container, text="Reload", command=lambda: self.run())
+        b.grid(row=1, column=2)
+        l = tk.Message(self.kanu.container, width=300, text="Option 1. Create a new database")
+        l.grid(row=2, column=0, columnspan=3)
+        l = tk.Label(self.kanu.container, text="Document ⓘ:")
+        Tooltip(l, "Directory containing documents for the database.")
+        l.grid(row=3, column=0) 
+        self.document_label = tk.Label(self.kanu.container, text="Not selected", fg="red")
         self.document_label.grid(row=3, column=1)
-        b = tk.Button(self.kanu.container, text="Browse", command=self.specify_document_file)
+        b = tk.Button(self.kanu.container, text="Browse", command=self.specify_document_directory)
         b.grid(row=3, column=2)
-        l = tk.Label(self.kanu.container, text="Database:")
+        l = tk.Label(self.kanu.container, text="Database ⓘ:")
+        Tooltip(l, "Directory where the database will be stored.")
         l.grid(row=4, column=0)       
-        self.new_database_label = tk.Label(self.kanu.container, text="No directory selected", fg="red")
+        self.new_database_label = tk.Label(self.kanu.container, text="Not selected", fg="red")
         self.new_database_label.grid(row=4, column=1)
         b = tk.Button(self.kanu.container, text="Browse", command=self.specify_new_database_directory)
         b.grid(row=4, column=2)
         self.option1_button = tk.Button(self.kanu.container, text="Go with Option 1", command=self.go_with_option1)
         self.option1_button.grid(row=5, column=0, columnspan=3)
         self.option1_button["state"] = tk.DISABLED
-        label = tk.Message(self.kanu.container, width=300, text="Option 2. Use an existing database")
-        label.grid(row=6, column=0, columnspan=3)
-        f = tk.Label(self.kanu.container, text="Database:")
-        f.grid(row=7, column=0)
-        self.old_database_label = tk.Label(self.kanu.container, text="No directory selected", fg="red")
+        l = tk.Message(self.kanu.container, width=300, text="Option 2. Use an existing database")
+        l.grid(row=6, column=0, columnspan=3)
+        l = tk.Label(self.kanu.container, text="Database ⓘ:")
+        Tooltip(l, "Directory where the database is stored.")
+        l.grid(row=7, column=0)
+        self.old_database_label = tk.Label(self.kanu.container, text="Not selected", fg="red")
         self.old_database_label.grid(row=7, column=1)
-        open_button = tk.Button(self.kanu.container, text="Browse", command=self.specify_old_database_directory)
-        open_button.grid(row=7, column=2)
+        b = tk.Button(self.kanu.container, text="Browse", command=self.specify_old_database_directory)
+        b.grid(row=7, column=2)
         self.option2_button = tk.Button(self.kanu.container, text="Go with Option 2", command=self.go_with_option2)
         self.option2_button.grid(row=8, column=0, columnspan=3)
         self.option2_button["state"] = tk.DISABLED
 
     def query(self):
         self.db = Chroma(persist_directory=self.database_directory, embedding_function=OpenAIEmbeddings())
-        self.qa = RetrievalQA.from_chain_type(llm=OpenAI(), chain_type="stuff", retriever=self.db.as_retriever())
+        self.qa = RetrievalQA.from_chain_type(llm=ChatOpenAI(model_name=self.model), chain_type="stuff", retriever=self.db.as_retriever())
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
-        title_label = tk.Label(self.kanu.container, text="DocGPT")
-        title_label.grid(row=0, column=0, columnspan=3)
-        session_label = tk.Label(self.kanu.container, text="Chat session")
-        session_label.grid(row=1, column=0, columnspan=3)
+        l = tk.Label(self.kanu.container, text="DocGPT")
+        l.grid(row=0, column=0, columnspan=3)    
         self.session = tk.Text(self.kanu.container, width=70, height=20)
-        self.session.grid(row=2, column=0, columnspan=3)
-        entry = tk.Entry(self.kanu.container, width=54)
-        entry.grid(row=3, column=0, columnspan=3)
-        send_button = tk.Button(self.kanu.container, text="Send", command=lambda: self._send_message(entry))
-        send_button.grid(row=4, column=0)
-        clear_butoon = tk.Button(self.kanu.container, text="Clear", command=lambda: self.clear_session())
-        clear_butoon.grid(row=4, column=1)
-        back_button = tk.Button(self.kanu.container, text="Go back", command=lambda: self.run())
-        back_button.grid(row=4, column=2)
+        self.session.grid(row=1, column=0, columnspan=3)
+        e = tk.Entry(self.kanu.container, width=54)
+        e.grid(row=2, column=0, columnspan=3)
+        b = tk.Button(self.kanu.container, text="Send", command=lambda: self.send_message(e))
+        b.grid(row=3, column=0)
+        b = tk.Button(self.kanu.container, text="Clear", command=lambda: self.clear_session())
+        b.grid(row=3, column=1)
+        b = tk.Button(self.kanu.container, text="Go back", command=lambda: self.run())
+        b.grid(row=3, column=2)
 
-    def _send_message(self, entry):
+    def send_message(self, entry):
         self.session.insert(tk.END, "You: " + entry.get() + "\n")
         response = self.qa(entry.get())["result"]
-        self.session.insert(tk.END, "Bot:" + response + "\n")
+        self.session.insert(tk.END, "Bot: " + response + "\n")
         entry.delete(0, tk.END)
 
     def go_with_option1(self):
-        loader = TextLoader(self.document_file)
-        documents = loader.load()
-        text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
-        docs = text_splitter.split_documents(documents)
-        embeddings = OpenAIEmbeddings()
-        db = Chroma.from_documents(docs, embeddings, persist_directory=self.database_directory)
+        documents = []
+        for root, dirs, files in os.walk(self.document_directory):
+            for file in files:
+                file_path = os.path.join(root, file)
+                file_ext = os.path.splitext(file_path)[1]
+                if file_ext not in DOCUMENT_LOADERS:
+                    continue
+                loader = DOCUMENT_LOADERS[file_ext](file_path)
+                document = loader.load()[0]
+                documents.append(document)
+        text_splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=50)
+        texts = text_splitter.split_documents(documents)
+        db = Chroma.from_documents(texts, OpenAIEmbeddings(), persist_directory=self.database_directory)
+        db.add_documents(texts)    
         db.persist()
         db = None
         self.query()
 
     def go_with_option2(self):
         self.query()
 
-    def specify_document_file(self):
-        file_path = filedialog.askopenfilename()
-        if not file_path:
+    def specify_document_directory(self):
+        directory_path = filedialog.askdirectory()
+        if not directory_path:
             return
-        self.document_file = file_path
-        self.document_label.configure(text=os.path.basename(file_path), fg="lime green")
-        if self.new_database_label["text"] != "No directory selected":
+        self.document_directory = directory_path
+        self.document_label.configure(text=os.path.basename(directory_path), fg="lime green")
+        if self.new_database_label["text"] != "Not selected":
             self.option1_button["state"] = tk.NORMAL
 
     def specify_new_database_directory(self):
         directory_path = filedialog.askdirectory()
         if not directory_path:
             return
         self.database_directory = directory_path
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kanu-0.2.0/setup.py` & `kanu-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+
+long_description = (Path(__file__).parent / "README.md").read_text()
 
 exec(open("kanu/version.py").read())
 
 setup(
     name="kanu",
     version=__version__,
     author='Seung-been "Steven" Lee',
     author_email="sbstevenlee@gmail.com",
     description="A minimalistic Python-based GUI for various chatbots",
     url="https://github.com/sbslee/kanu",
     packages=find_packages(),
     license="MIT",
     entry_points={"console_scripts": ["kanu=kanu.__main__:main"]},
-    long_description="A minimalistic Python-based GUI for various chatbots",
-    long_description_content_type="text/plain"
+    long_description=long_description,
+    long_description_content_type="text/markdown"
 )
```

