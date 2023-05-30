# Comparing `tmp/torchbones-1.1.2.tar.gz` & `tmp/torchbones-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.1.2.tar", last modified: Tue May 30 15:04:44 2023, max compression
+gzip compressed data, was "torchbones-1.1.3.tar", last modified: Tue May 30 15:25:15 2023, max compression
```

## Comparing `torchbones-1.1.2.tar` & `torchbones-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:04:44.665544 torchbones-1.1.2/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:04:44.665544 torchbones-1.1.2/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-30 15:04:44.665544 torchbones-1.1.2/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-30 15:04:41.000000 torchbones-1.1.2/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:04:44.665544 torchbones-1.1.2/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.2/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    16154 2023-05-30 15:04:37.000000 torchbones-1.1.2/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:04:44.665544 torchbones-1.1.2/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:04:44.000000 torchbones-1.1.2/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-30 15:04:44.000000 torchbones-1.1.2/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-30 15:04:44.000000 torchbones-1.1.2/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-30 15:04:44.000000 torchbones-1.1.2/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-30 15:04:44.000000 torchbones-1.1.2/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:25:15.115541 torchbones-1.1.3/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:25:15.115541 torchbones-1.1.3/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-30 15:25:15.115541 torchbones-1.1.3/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-05-30 15:24:54.000000 torchbones-1.1.3/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:25:15.115541 torchbones-1.1.3/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.1.3/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    16187 2023-05-30 15:23:55.000000 torchbones-1.1.3/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-30 15:25:15.115541 torchbones-1.1.3/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-30 15:25:15.000000 torchbones-1.1.3/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.1.2/torchbones/main.py` & `torchbones-1.1.3/torchbones/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,42 +330,45 @@
             ax[2].set_xlabel('Epoch')
             ax[2].set_ylabel('Loss')
             ax[2].legend()
             ax[2].set_yscale('log')
         else: fig, ax = plt.subplots(1, 2, figsize = (15, 4))
             
         x, y = self.data[4], np.squeeze(np.squeeze(self.testout.detach().numpy()))
-        yt, xt = torch.squeeze(torch.squeeze(self.output)).detach().numpy(), self.truetrain
+        yt, xt = self.net(self.data[0]).squeeze().squeeze().detach().numpy(), self.data[1]
         
-        ax[0].set_xlabel('train truth')
-        ax[0].set_ylabel('train predication') 
+         
         ax[1].set_xlabel('test truth')
-        ax[1].set_ylabel('test predication') 
+        ax[1].set_ylabel('test predication')
+        ax[0].set_xlabel('train truth')
+        ax[0].set_ylabel('train predication')
         
         if str(self.cost) == 'CrossEntropyLoss()':
             classes = np.unique(self.truth)
             num_classes = len(classes)
             cm = []
-            cm.append(confusion_matrix(x, classes[np.argmax(y, axis = 1)]))
+            
             cm.append(confusion_matrix(xt, classes[np.argmax(yt, axis = 1)]))
+            cm.append(confusion_matrix(x, classes[np.argmax(y, axis = 1)]))
             for i in (0, 1):
                 ax[i].set_xticks(np.arange(num_classes))
                 ax[i].set_yticks(np.arange(num_classes))
                 ax[i].set_xticklabels(classes)
                 ax[i].set_yticklabels(classes)
                 cbar = ax[i].figure.colorbar(ax[i].imshow(cm[i], cmap='Blues'), ax=ax[i])
 
                 # Display values inside the plot
                 thresh = cm[i].max() / 2
                 for k in range(num_classes):
                     for j in range(num_classes):
                         ax[i].text(j, k, cm[i][k, j], ha='center', va='center', color='white' if cm[i][k, j] > thresh else 'black')
         else:
-            ax[0].hist2d(x, y, bins = 30)
-            ax[1].hist2d(xt, yt, bins = 30)
+            ax[0].hist2d(xt, yt, bins = 30)
+            ax[1].hist2d(x, y, bins = 30)
+            
         fig.tight_layout()
         plt.show()
     
     def data_prep(self):
         data = torch.tensor(self.indata).double()
         
         if len(data.shape) == 1:
```

