# Comparing `tmp/text2phonemesequence-0.0.7.tar.gz` & `tmp/text2phonemesequence-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/text2phonemesequence-0.0.7.tar", last modified: Mon May 29 10:28:43 2023, max compression
+gzip compressed data, was "dist/text2phonemesequence-0.0.8.tar", last modified: Tue May 30 14:16:49 2023, max compression
```

## Comparing `text2phonemesequence-0.0.7.tar` & `text2phonemesequence-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.0.7/setup.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1777 2023-05-20 04:58:56.000000 text2phonemesequence-0.0.7/README.md
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2405 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/PKG-INFO
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2405 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/top_level.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/dependency_links.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/SOURCES.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/requires.txt
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     7256 2023-05-29 10:27:51.000000 text2phonemesequence-0.0.7/text2phonemesequence/text2phonemesequence.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-05-29 10:27:40.000000 text2phonemesequence-0.0.7/text2phonemesequence/__init__.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/setup.cfg
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1777 2023-05-20 04:58:56.000000 text2phonemesequence-0.0.8/README.md
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/setup.cfg
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.0.8/setup.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/text2phonemesequence/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-05-30 14:12:16.000000 text2phonemesequence-0.0.8/text2phonemesequence/__init__.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     7358 2023-05-30 14:15:58.000000 text2phonemesequence-0.0.8/text2phonemesequence/text2phonemesequence.py
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/text2phonemesequence.egg-info/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/text2phonemesequence.egg-info/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/text2phonemesequence.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/text2phonemesequence.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/text2phonemesequence.egg-info/requires.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-05-30 14:16:49.000000 text2phonemesequence-0.0.8/text2phonemesequence.egg-info/top_level.txt
```

### Comparing `text2phonemesequence-0.0.7/setup.py` & `text2phonemesequence-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.0.7/README.md` & `text2phonemesequence-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.0.7/PKG-INFO` & `text2phonemesequence-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
+Description: # Text2PhonemeSequence: A Python Library to convert text to phoneme sequences used for [XPhoneBERT](https://github.com/VinAIResearch/XPhoneBERT) 
+        
+        - [Installation](#install)
+        - [Usage example](#example)
+        
+        ## Installation <a name="install"></a>
+        
+        - To install **Text2PhonemeSequence**, users have to run the following command:
+        
+            `$ pip install text2phonemesequence` 
+        
+        ## Usage example <a name="example"></a>
+        The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
+        
+        ```python
+        from text2phonemesequence import Text2PhonemeSequence
+        
+        # Load Text2PhonemeSequence
+        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
+        
+        
+        # Convert a raw corpus
+        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
+        
+        # Convert a raw sentence
+        model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
+        ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
+        ```
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-
-# Text2PhonemeSequence: A Python Library to convert text to phoneme sequences used for [XPhoneBERT](https://github.com/VinAIResearch/XPhoneBERT) 
-
-- [Installation](#install)
-- [Usage example](#example)
-
-## Installation <a name="install"></a>
-
-- To install **Text2PhonemeSequence**, users have to run the following command:
-
-    `$ pip install text2phonemesequence` 
-
-## Usage example <a name="example"></a>
-The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
-
-```python
-from text2phonemesequence import Text2PhonemeSequence
-
-# Load Text2PhonemeSequence
-model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
-
-
-# Convert a raw corpus
-model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
-
-# Convert a raw sentence
-model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
-##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
-```
-
-
```

### Comparing `text2phonemesequence-0.0.7/text2phonemesequence.egg-info/PKG-INFO` & `text2phonemesequence-0.0.8/text2phonemesequence.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
+Description: # Text2PhonemeSequence: A Python Library to convert text to phoneme sequences used for [XPhoneBERT](https://github.com/VinAIResearch/XPhoneBERT) 
+        
+        - [Installation](#install)
+        - [Usage example](#example)
+        
+        ## Installation <a name="install"></a>
+        
+        - To install **Text2PhonemeSequence**, users have to run the following command:
+        
+            `$ pip install text2phonemesequence` 
+        
+        ## Usage example <a name="example"></a>
+        The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
+        
+        ```python
+        from text2phonemesequence import Text2PhonemeSequence
+        
+        # Load Text2PhonemeSequence
+        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
+        
+        
+        # Convert a raw corpus
+        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
+        
+        # Convert a raw sentence
+        model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
+        ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
+        ```
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-
-# Text2PhonemeSequence: A Python Library to convert text to phoneme sequences used for [XPhoneBERT](https://github.com/VinAIResearch/XPhoneBERT) 
-
-- [Installation](#install)
-- [Usage example](#example)
-
-## Installation <a name="install"></a>
-
-- To install **Text2PhonemeSequence**, users have to run the following command:
-
-    `$ pip install text2phonemesequence` 
-
-## Usage example <a name="example"></a>
-The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
-
-```python
-from text2phonemesequence import Text2PhonemeSequence
-
-# Load Text2PhonemeSequence
-model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
-
-
-# Convert a raw corpus
-model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
-
-# Convert a raw sentence
-model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
-##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
-```
-
-
```

### Comparing `text2phonemesequence-0.0.7/text2phonemesequence/text2phonemesequence.py` & `text2phonemesequence-0.0.8/text2phonemesequence/text2phonemesequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from transformers import T5ForConditionalGeneration, AutoTokenizer
 from segments import Tokenizer
 import os
 from tqdm import tqdm
 
 class Text2PhonemeSequence:
-    def __init__(self, pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='vie-c', is_cuda=True):
-        self.tokenizer = AutoTokenizer.from_pretrained('google/byt5-small')
+    def __init__(self, pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', tokenizer= 'google/byt5-small', language='vie-c', is_cuda=True):
+        self.tokenizer = AutoTokenizer.from_pretrained(tokenizer)
         self.model = T5ForConditionalGeneration.from_pretrained(pretrained_g2p_model)
         self.is_cuda = is_cuda
         if self.is_cuda:
             self.model = self.model.cuda()
         self.punctuation = list('.?!,:;-()[]{}<>"') + list("'/‘”“/&#~@^|") + ['...', '*']
         self.segment_tool = Tokenizer()
         self.language = language
@@ -76,14 +76,15 @@
             f.write("\n")
         f.close()
     
     def infer_sentence(self, sentence="", seperate_syllabel_token="_"):
         list_words = sentence.split(" ")
         list_phones = []
         for i in range(len(list_words)):
+            list_words[i] = list_words[i].replace(seperate_syllabel_token, " ")
             if list_words[i] in self.phone_dict:
                 list_phones.append(self.phone_dict[list_words[i]][0])
             elif list_words[i] in self.punctuation:
                 list_phones.append(list_words[i])   
             else:
                 out = self.tokenizer('<' + self.language + '>: ' + list_words[i], padding=True, add_special_tokens=False, return_tensors='pt')
                 if self.is_cuda:
```

