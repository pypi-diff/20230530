# Comparing `tmp/torchbones-1.1.3.tar.gz` & `tmp/torchbones-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.1.3.tar", last modified: Tue May 30 15:25:15 2023, max compression
+gzip compressed data, was "torchbones-1.1.4.tar", last modified: Tue May 30 15:37:40 2023, max compression
```

## Comparing `torchbones-1.1.3.tar` & `torchbones-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:25:15.115541 torchbones-1.1.3/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:25:15.115541 torchbones-1.1.3/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-30 15:25:15.115541 torchbones-1.1.3/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-30 15:24:54.000000 torchbones-1.1.3/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:25:15.115541 torchbones-1.1.3/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.3/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16187 2023-05-30 15:23:55.000000 torchbones-1.1.3/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:25:15.115541 torchbones-1.1.3/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:37:40.795534 torchbones-1.1.4/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:37:40.795534 torchbones-1.1.4/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-30 15:37:40.795534 torchbones-1.1.4/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-30 15:37:30.000000 torchbones-1.1.4/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:37:40.795534 torchbones-1.1.4/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.4/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16242 2023-05-30 15:37:25.000000 torchbones-1.1.4/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:37:40.795534 torchbones-1.1.4/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-30 15:37:40.000000 torchbones-1.1.4/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.1.3/torchbones/main.py` & `torchbones-1.1.4/torchbones/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,34 +244,36 @@
         self.lr = kwargs.get('lr', self.lr)
         self.lr_decay = kwargs.get('lr_decay', self.lr_decay)
         self.lr_min = kwargs.get('lr_min', self.lr_min)
         training = kwargs.get('training', True)
         self.printev = kwargs.get('print_ev', self.printev)
         self.plotev = kwargs.get('plot_ev', self.plotev)
         e0 = self.epoch
+        batches = round(len(traintruth)/self.batch_size)
         
         while self.epoch - e0 < self.epochs:
+            l = 0
             shuffle = torch.randperm(len(traintruth)) #shuffle training set
             self.lr = max(self.lr * self.lr_decay, self.lr_min)  #lr decay
-            for i in range(round(len(traintruth)/self.batch_size)):
+            for i in range(batches):
                 self.optimizer.param_groups[0]['lr'] = self.lr
                 where = shuffle[i * self.batch_size:(i + 1) * self.batch_size] #take batch of training set
                 self.output = self.net(train[where])
                 self.truetrain = traintruth[where]
                 if type(self.cov)== int:
                     loss = torch.mean(self.cost(self.output.squeeze().squeeze(), torch.tensor(traintruth[where])))
                 else:
                     loss = torch.mean(self.cost(self.output.squeeze().squeeze(), torch.tensor(traintruth[where]), traincov))
-                    
+                l+= loss
                 if training: #turn off training to run without optimization
                     self.optimizer.zero_grad()
                     loss.backward(retain_graph = True)
                     self.optimizer.step()
                          
-            self.trainerr.append(loss.detach().numpy())
+            self.trainerr.append((l/batches).detach().numpy())
             self.testout = self.net(test)
             if type(self.cov) == int:
                 self.err = self.cost(torch.squeeze(self.testout), torch.tensor(testtruth)).mean().detach().numpy()
             else:
                 self.err = self.cost(torch.squeeze(self.testout), torch.tensor(testtruth), testcov).mean().detach().numpy()
             self.testerr.append(self.err)
             if not (self.epoch-e0) % self.plotev:
```

