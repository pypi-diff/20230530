# Comparing `tmp/torchbones-1.1.0.tar.gz` & `tmp/torchbones-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.1.0.tar", last modified: Mon May 29 18:24:28 2023, max compression
+gzip compressed data, was "torchbones-1.1.1.tar", last modified: Tue May 30 14:59:27 2023, max compression
```

## Comparing `torchbones-1.1.0.tar` & `torchbones-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:24:28.109497 torchbones-1.1.0/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:24:28.109497 torchbones-1.1.0/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-29 18:24:28.109497 torchbones-1.1.0/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-29 18:24:06.000000 torchbones-1.1.0/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:24:28.109497 torchbones-1.1.0/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.0/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16101 2023-05-29 18:24:24.000000 torchbones-1.1.0/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-29 18:24:28.109497 torchbones-1.1.0/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-29 18:24:28.000000 torchbones-1.1.0/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 14:59:27.885546 torchbones-1.1.1/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 14:59:27.885546 torchbones-1.1.1/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-30 14:59:27.885546 torchbones-1.1.1/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-30 14:58:55.000000 torchbones-1.1.1/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 14:59:27.885546 torchbones-1.1.1/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.1/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16125 2023-05-30 14:58:25.000000 torchbones-1.1.1/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 14:59:27.885546 torchbones-1.1.1/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 14:59:27.000000 torchbones-1.1.1/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-30 14:59:27.000000 torchbones-1.1.1/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-30 14:59:27.000000 torchbones-1.1.1/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-30 14:59:27.000000 torchbones-1.1.1/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-30 14:59:27.000000 torchbones-1.1.1/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.1.0/torchbones/main.py` & `torchbones-1.1.1/torchbones/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         
   
         
                 
     def run(self, **kwargs):
         if len(self.trainerr)!=len(self.testerr):
             self.trainerr = self.trainerr[:-1]
-        keys = ('lr', 'lr_decay', 'lr_min', 'epochs', 'training',)
+        keys = ('lr', 'lr_decay', 'lr_min', 'epochs', 'training', 'printev', 'plotev')
         for kwarg in kwargs.keys():
             if kwarg not in keys:
                 raise Exception(kwarg + ' is not a valid key. Valid keys: ', keys )
                 
         train, traintruth, traincov, test, testtruth, testcov = self.data
         self.epochs = kwargs.get('epochs', 20)
         self.lr = kwargs.get('lr', self.lr)
@@ -302,15 +302,15 @@
             print('rewind', float(self.trainerr[-1]), float(self.trainerr[-1 - t]), self.lr)
             self.lr = 1* self.oldlr #revert lr   
             self.net.load_state_dict(self.oldmodel) #revert weights
             #remove record of bad epochs
             self.testerr = self.testerr[:-t]  
             self.trainerr = self.trainerr[:-t]
             self.epoch -= t
-            self.optimizer = self.optim(self.net.parameters(), lr = self.lr) #delete adam's memory of the oopsie
+            self.optimizer = self.optimizer(self.net.parameters(), lr = self.lr) #delete adam's memory of the oopsie
             self.countcheck+=1
         else: 
             #create a checkpoint
             self.oldmodel = copy.deepcopy(self.net.state_dict())#create a checkpoint to return to if training goes off the rails
             self.oldlr = 1*self.lr
             self.countcheck = 0
```

