# Comparing `tmp/Python_Road-0.0.0.1.tar.gz` & `tmp/Python_Road-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python_Road-0.0.0.1.tar", last modified: Wed May 24 13:42:58 2023, max compression
+gzip compressed data, was "Python_Road-0.0.0.2.tar", last modified: Tue May 30 12:35:32 2023, max compression
```

## Comparing `Python_Road-0.0.0.1.tar` & `Python_Road-0.0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 13:42:58.356243 Python_Road-0.0.0.1/
--rw-rw-rw-   0        0        0       77 2023-05-24 13:42:58.356243 Python_Road-0.0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 13:42:58.356243 Python_Road-0.0.0.1/Python_Road.egg-info/
--rw-rw-rw-   0        0        0       77 2023-05-24 13:42:58.000000 Python_Road-0.0.0.1/Python_Road.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-05-24 13:42:58.000000 Python_Road-0.0.0.1/Python_Road.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 13:42:58.000000 Python_Road-0.0.0.1/Python_Road.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 13:42:58.000000 Python_Road-0.0.0.1/Python_Road.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3275 2023-05-24 13:41:56.000000 Python_Road-0.0.0.1/Python_Road.py
--rw-rw-rw-   0        0        0       42 2023-05-24 13:42:58.356243 Python_Road-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      211 2023-05-24 13:03:48.000000 Python_Road-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:35:32.526504 Python_Road-0.0.0.2/
+-rw-rw-rw-   0        0        0      134 2023-05-30 12:35:32.521983 Python_Road-0.0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 12:35:32.519372 Python_Road-0.0.0.2/Python_Road.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-05-30 12:35:32.000000 Python_Road-0.0.0.2/Python_Road.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-30 12:35:32.000000 Python_Road-0.0.0.2/Python_Road.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:35:32.000000 Python_Road-0.0.0.2/Python_Road.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:35:32.000000 Python_Road-0.0.0.2/Python_Road.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4144 2023-05-30 12:31:03.000000 Python_Road-0.0.0.2/Python_Road.py
+-rw-rw-rw-   0        0        0       42 2023-05-30 12:35:32.527506 Python_Road-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-05-30 12:34:29.000000 Python_Road-0.0.0.2/setup.py
```

### Comparing `Python_Road-0.0.0.1/Python_Road.py` & `Python_Road-0.0.0.2/Python_Road.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import os
+import pygame
+import turtle
+import traceback
 import random
 
 
 class Size:
 	def find_file_size(self, path="C:\\", max_or_min="max"):
 		size_path, size_list = self.__get_all_size(path)
 		if max_or_min == "max":
@@ -87,16 +90,18 @@
 						return sum(*args[0]) / sum(*args[1])
 
 
 class Random:
 	def random_number(self):
 		return random.random() * 100
 
-	def random_choice(self, list):
-		return random.choice(list)
+
+	def random_choice(lis):
+		return random.choice(lis)
+
 
 	def random_number_with_step(self, first=0, end=100, step=1):
 		while True:
 			num = random.randint(first, end)
 			if (num - first) % step == 0:
 				return num
 
@@ -105,10 +110,49 @@
 	if flush:
 		print(*args, "\r", end=end)
 		sys.stdout.flush()
 	else:
 		print(*args, end=end)
 
 
+def eval_inputer(string):
+	inputer = input(string)
+	try:
+		return eval(inputer)
+	except:
+		return inputer
+
+
+def Download_with_progress_bar(url, fname):
+	resp = requests.get(url, stream=True)
+	total = int(resp.headers.get('content-length', 0))
+	with open(fname, 'wb') as file, tqdm(
+			desc=fname,
+			total=total,
+			unit='iB',
+			unit_scale=True,
+			unit_divisor=1024,
+	) as bar:
+		for data in resp.iter_content(chunk_size=1024):
+			size = file.write(data)
+			bar.update(size)
+
+
+def if_not_error(*args,func):
+	try:
+		print("------------------------------")
+		print("运行成功")
+		print(f"运行结果：{func(*args)}")
+		print("------------------------------")
+	except:
+		print("------------------------------")
+		print("运行失败")
+		print("错误提示：")
+		print(traceback.format_exc())
+		print("------------------------------")
+
+
+
+
 math = Math()
 size = Size()
-print(math.pi)
+
```

