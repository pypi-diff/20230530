# Comparing `tmp/openirt-0.1.2.tar.gz` & `tmp/openirt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openirt-0.1.2.tar", last modified: Mon May 29 12:12:37 2023, max compression
+gzip compressed data, was "openirt-0.1.3.tar", last modified: Tue May 30 08:40:22 2023, max compression
```

## Comparing `openirt-0.1.2.tar` & `openirt-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 12:12:37.266515 openirt-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-29 12:12:15.000000 openirt-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-29 12:12:37.266515 openirt-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-29 12:12:15.000000 openirt-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 12:12:37.264515 openirt-0.1.2/openirt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6938 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/bayes3PL.py
--rw-rw-rw-   0 root         (0) root         (0)     2081 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3930 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/irt_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/item_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1491 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/logistic_1P_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/logistic_3PM.py
--rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/norm_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3049 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/pl2.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 12:12:37.265515 openirt-0.1.2/openirt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-29 12:12:37.000000 openirt-0.1.2/openirt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      376 2023-05-29 12:12:37.000000 openirt-0.1.2/openirt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 12:12:37.000000 openirt-0.1.2/openirt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-29 12:12:37.000000 openirt-0.1.2/openirt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 12:12:37.266515 openirt-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-29 12:12:15.000000 openirt-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 12:12:37.265515 openirt-0.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-29 12:12:15.000000 openirt-0.1.2/tests/test_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:40:22.726702 openirt-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-30 08:40:03.000000 openirt-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 08:40:22.725702 openirt-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-30 08:40:03.000000 openirt-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:40:22.724702 openirt-0.1.3/openirt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 08:40:03.000000 openirt-0.1.3/openirt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6938 2023-05-30 08:40:03.000000 openirt-0.1.3/openirt/bayes3PL.py
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2023-05-30 08:40:03.000000 openirt-0.1.3/openirt/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2023-05-30 08:40:03.000000 openirt-0.1.3/openirt/irt_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-30 08:40:03.000000 openirt-0.1.3/openirt/item_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3387 2023-05-30 08:40:03.000000 openirt-0.1.3/openirt/norm_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2646 2023-05-30 08:40:03.000000 openirt-0.1.3/openirt/pl1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2023-05-30 08:40:03.000000 openirt-0.1.3/openirt/pl2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5893 2023-05-30 08:40:03.000000 openirt-0.1.3/openirt/pl3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:40:22.725702 openirt-0.1.3/openirt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 08:40:22.000000 openirt-0.1.3/openirt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-30 08:40:22.000000 openirt-0.1.3/openirt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 08:40:22.000000 openirt-0.1.3/openirt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-30 08:40:22.000000 openirt-0.1.3/openirt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 08:40:22.726702 openirt-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-30 08:40:03.000000 openirt-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:40:22.725702 openirt-0.1.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-30 08:40:03.000000 openirt-0.1.3/tests/test_func.py
```

### Comparing `openirt-0.1.2/LICENSE` & `openirt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openirt-0.1.2/openirt/bayes3PL.py` & `openirt-0.1.3/openirt/bayes3PL.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.2/openirt/cli.py` & `openirt-0.1.3/openirt/cli.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.2/openirt/irt_instance.py` & `openirt-0.1.3/openirt/irt_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             
     def check_item_params(self):
         if self.item_params is not None:
             if not self.items.equals(self.item_params.columns):
                 raise ValueError('Items in results file and item parameters file must be the same.')
     
     def train_model(self):
-        print(self.results)
+        # print(self.results)
         abilities, params = self.model.train_em_mle(self.results)
         
         # self.model.plot_item_curve(params)
         pass
     
     def estimate_item_params(self):
         pass
```

### Comparing `openirt-0.1.2/openirt/item_model.py` & `openirt-0.1.3/openirt/item_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Union
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 class ItemModel():
-
     def __init__(self) -> None:
         pass
     
     @abstractmethod
     def prob(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
         pass
```

### Comparing `openirt-0.1.2/openirt/logistic_3PM.py` & `openirt-0.1.3/openirt/pl2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,116 @@
+import sys
+sys.path.append('./openirt')
 from item_model import ItemModel
 from typing import Union
 import numpy as np
 import matplotlib.pyplot as plt
-from scipy.optimize import minimize    
 
+class PL2(ItemModel):
+    def prob(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
+        """
+        Calculate the probability of a correct response given the ability and item parameters.
 
-class Logistic3PM(ItemModel):
-    
-    def prob(self, 
-             ability: Union[list, np.ndarray, float], 
-             params: Union[list, np.ndarray])  -> np.ndarray:
-        items = np.array(params).shape[1]
-        num_abilities = 1
-        if np.array(ability).shape != ():
-            num_abilities = np.array(ability).shape[0]
-        ability = np.tile(np.array([ability]).transpose(), (1, items))
+        Args:
+            ability: A list, numpy array, or float representing the ability of the individual.
+            params: A list or numpy array containing the item parameters.
 
-        params = np.tile(params, num_abilities).reshape(
-            (3, num_abilities, items))
-        return params[2] + (1 - params[2]) / (1 + np.exp(-params[0] * (ability - params[1])))
-    
-    def prob2PM(self,
-                ability: Union[list, np.ndarray, float],
-                params: Union[list, np.ndarray]) -> np.ndarray:
+        Returns:
+            A numpy array representing the probabilities of correct responses.
+        """
         items = np.array(params).shape[1]
         num_abilities = 1
         if np.array(ability).shape != ():
             num_abilities = np.array(ability).shape[0]
         ability = np.tile(np.array([ability]).transpose(), (1, items))
 
-        params = np.tile(params, num_abilities).reshape(
-            (3, num_abilities, items))
-        return 1 / (1 + np.exp(-params[0] * (ability - params[1])))
-    
-    def estimate_parameters(self, 
-                            ability: Union[list, np.ndarray], 
-                            result: Union[list, np.ndarray],
-                            a_orig=1,
-                            b_orig=0.1, 
-                            c_orig=0.1,
-                            end=0.0000001,  
-                            eps=0.1) -> np.ndarray:
-        # use orig_params?
+        params = np.tile(params, num_abilities).reshape((2, num_abilities, items))
+        return 1 / (1 + np.exp(-params[0] - (params[1] * ability)))
+
+    def estimate_parameters(self, ability: Union[list, np.ndarray], result: Union[list, np.ndarray],
+                            sigm_orig=-1, lamb_orig=1, end=0.00001, eps=0.1) -> np.ndarray:
+        """
+        Estimate the parameters of the model given the abilities and item responses.
+
+        Args:
+            ability: A list or numpy array containing the abilities of individuals.
+            result: A list or numpy array representing the item responses.
+            sigm_orig: The initial value for the parameter sigm.
+            lamb_orig: The initial value for the parameter lamb.
+            end: The convergence threshold.
+            eps: The threshold for detecting a near-singular matrix.
+
+        Returns:
+            A numpy array representing the estimated parameters.
+        """
         ability = np.array(ability)
         result = np.array(result)
-        est = np.array([a_orig, b_orig, c_orig])
-        prev_est = est + 2 * end
-        while np.all(np.abs(prev_est - est) > end):
-            # self.plot_item_curve(est.reshape((3,1)))
-            P = self.prob(ability, est.reshape((3,1))).T[0]
-            Q = 1 - P
-            P_2pm = self.prob2PM(ability, est.reshape((3,1))).T[0]
-            
-            L11 = -np.sum((ability-est[1])**2 * P * Q * (P_2pm/P)**2)
-            L12 = np.sum(est[0] * (ability - est[1]) * P * Q * (P_2pm/P))
-            L13 = -np.sum((ability - est[1]) * (Q / (1 - est[2])) * (P_2pm/P))
-            
-            L22 = -est[0]**2 * np.sum(P * Q * (P_2pm/P))
-            L23 = np.sum(est[0] * (Q / (1 - est[2])) * (P_2pm/P))
-            
-            L33 = -np.sum((Q / (1 - est[2])) / (P - est[2]) * (P_2pm/P))
-
-            L = np.array([[L11, L12, L13], [L12, L22, L23], [L13, L23, L33]])
-            
+        est = [sigm_orig, lamb_orig]
+        prev_est = [0, 0]
+        while abs(est[0] - prev_est[0]) > end or abs(est[1] - prev_est[1]) > end:
+            P = self.prob(ability, [[est[0]], [est[1]]]).transpose()[0]
+            W = P * (1 - P)
+            L11 = -np.sum(W)
+            L12 = -np.sum(ability * W)
+            L22 = -np.sum(ability**2 * W)
+            L = np.array([[L11, L12], [L12, L22]])
             if abs(np.linalg.det(L)) < eps:
-                print('break')
                 break
             L_inv = np.linalg.inv(L)
-            
-            L1 = np.sum((result - P) * (ability - est[1]) * (P_2pm/P))
-            L2 = -est[0] * np.sum((result - P) * (P_2pm/P))
-            L3 = np.sum((result - P) / (P - est[2]) * (P_2pm/P))
-            obs_mat = np.array([L1, L2, L3])
+
+            obs_mat = np.array([np.sum(result - P), np.sum((result - P) * ability)])
             prev_est = est
             est = est - np.matmul(L_inv, obs_mat)
         return est
-    
-    def estimate_ability(self,
-                         params: Union[list, np.ndarray],
-                         results: Union[list, np.ndarray],
-                         end=0.00000001,
-                         eps=0.01) -> np.ndarray:
+
+    def estimate_ability(self, params: Union[list, np.ndarray], results: Union[list, np.ndarray],
+                         end=0.00000001, eps=0.01) -> np.ndarray:
+        """
+        Estimate the ability of an individual given the item parameters and responses.
+
+        Args:
+            params: A list or numpy array representing the item parameters.
+            results: A list or numpy array representing the item responses.
+            end: The convergence threshold.
+            eps: The threshold for detecting a near-singular matrix.
+
+        Returns:
+            A numpy array representing the estimated ability.
+        """
         params = np.array(params)
         results = np.array(results)
         est = 0.5
         prev_est = 0
         while abs(est - prev_est) > end:
             P = self.prob(est, params)[0]
-            Q = 1 - P
-            P_2pm = self.prob2PM(est, params)[0]
-            W = P_2pm * (1 - P_2pm)
-            
-            denom = - np.sum(params[0]**2 * W * (P_2pm/P)**2)
-            
-            print(denom)
-            if abs(denom) < eps:
+            W = (1 - P) * P
+            denom = np.sum(params[1]**2 * W)
+            if abs(denom) < eps or np.any(np.abs(W) < eps):
                 break
-            num = np.sum(params[0] * W * ((results - P) / (P * Q)) * (P_2pm/P))
             prev_est = est
-            est = est + (num / denom)
+            est = est + (np.sum(params[1] * W * ((results - P) / W)) / denom)
         return est
     
+    def convert_param_form(self, params):
+        """
+        Convert item parameters from one form to another.
+
+        Args:
+            params: A list or numpy array representing the item parameters.
+
+        Returns:
+            A numpy array representing the converted item parameters.
+        """
+        return np.array([-params[0] / params[1], 1 / params[1]])
+
     def plot_item_curve(self, p):
-        ability = np.linspace(-5, 5, 100)
+        """
+        Plot item curves for given item parameters.
+
+        Args:
+            p: A numpy array representing the item parameters.
+        """
+        ability = np.linspace(-4, 4, 100)
         for i in range(p.shape[1]):
-            plt.plot(ability, self.prob(ability, p[:,i].reshape(p.shape[0], 1)), label=f'Question{i+1}')        
+            plt.plot(ability, self.prob(ability, p[:,i].reshape(p.shape[0], 1)), label=f'Question{i+1}')
         plt.legend()
         plt.show()
```

### Comparing `openirt-0.1.2/openirt/norm_model.py` & `openirt-0.1.3/openirt/norm_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,14 @@
             W = h**2 / (P * (1 - P))
             L11 = -np.sum(W)
             L12 = -np.sum(ability * W)
             L22 = -np.sum(ability**2 * W)
             L = np.array([[L11, L12], [L12, L22]])
 
             if abs(np.linalg.det(L)) < eps:
-                print('break')
                 break
             L_inv = np.linalg.inv(L)
 
             v = (result - P) / h
             obs_mat = np.array([np.sum(W * v), np.sum(W * v * ability)])
             prev_est = est
             est = est - np.matmul(L_inv, obs_mat)
```

### Comparing `openirt-0.1.2/openirt/pl2.py` & `openirt-0.1.3/openirt/pl1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,67 @@
+import sys
+sys.path.append('./openirt')
 from item_model import ItemModel
 from typing import Union
 import numpy as np
-import matplotlib.pyplot as plt
+from pl2 import PL2
 
-class PL2(ItemModel):
-    def prob(self, 
-             ability: Union[list, np.ndarray, float], 
-             params: Union[list, np.ndarray])  -> np.ndarray:
-        items = np.array(params).shape[1]
-        num_abilities = 1
-        if np.array(ability).shape != ():
-            num_abilities = np.array(ability).shape[0]
-        ability = np.tile(np.array([ability]).transpose(), (1, items))
-
-        params = np.tile(params, num_abilities).reshape(
-            (2, num_abilities, items))
-        return 1 / (1 + np.exp(-params[0] - (params[1] * ability)))
-
-    def estimate_parameters(self, 
-                            ability: Union[list, np.ndarray], 
-                            result: Union[list, np.ndarray], 
-                            sigm_orig=-1, 
-                            lamb_orig=1, 
-                            end=0.00001,  
-                            eps=0.1) -> np.ndarray:
+class PL1(ItemModel):
+    def prob(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
+        """
+        Calculate the probability of a correct response given the ability and item parameters.
+
+        Args:
+            ability: A list, numpy array, or float representing the ability of the individual.
+            params: A list or numpy array containing the item parameters.
+
+        Returns:
+            A numpy array representing the probabilities of correct responses.
+        """
+        return PL2().prob(ability, [params[0], np.ones(len(params[0]))])
+
+    def estimate_parameters(self, ability: Union[list, np.ndarray], result: Union[list, np.ndarray],
+                            sigm_orig=0, end=0.0000001, eps=0.0001) -> np.ndarray:
+        """
+        Estimate the parameters of the model given the abilities and item responses.
+
+        Args:
+            ability: A list or numpy array containing the abilities of individuals.
+            result: A list or numpy array representing the item responses.
+            sigm_orig: The initial value for the parameter sigm.
+            end: The convergence threshold.
+            eps: The threshold for detecting a near-singular matrix.
+
+        Returns:
+            A numpy array representing the estimated parameters.
+        """
         ability = np.array(ability)
         result = np.array(result)
-        est = [sigm_orig, lamb_orig]
-        prev_est = [0, 0]
-        while abs(est[0] - prev_est[0]) > end or abs(est[1] - prev_est[1]) > end:
-            P = self.prob(
-                ability, [[est[0]], [est[1]]]).transpose()[0]
-            W = P * (1 - P)
-            L11 = -np.sum(W)
-            L12 = -np.sum(ability * W)
-            L22 = -np.sum(ability**2 * W)
-            L = np.array([[L11, L12], [L12, L22]])
-            if abs(np.linalg.det(L)) < eps:
+        est = sigm_orig
+        prev_est = est + 2 * end
+        while abs(est - prev_est) > end:
+            P = self.prob(ability, [[est]]).transpose()[0]
+            L1 = np.sum(result - P)
+            L2 = -np.sum(P * (1 - P))
+
+            if abs(L2) < eps:
                 break
-            L_inv = np.linalg.inv(L)
 
-            obs_mat = np.array(
-                [np.sum(result - P), np.sum((result - P) * ability)])
             prev_est = est
-            est = est - np.matmul(L_inv, obs_mat)
-        return est
+            est = est - L1 / L2
+        return np.array([est])
 
-    def estimate_ability(self,
-                         params: Union[list, np.ndarray],
-                         results: Union[list, np.ndarray],
-                         end=0.00000001,
-                         eps=0.01) -> np.ndarray:
-        params = np.array(params)
-        results = np.array(results)
-        est = 0.5
-        prev_est = 0
-        while abs(est - prev_est) > end:
-            P = self.prob(est, params)[0]
-            W = (1 - P) * P
-            denom = np.sum(params[1]**2 * W)
-            if abs(denom) < eps or np.any(np.abs(W) < eps):
-                break            
-            prev_est = est
-            est = est + (np.sum(params[1] * W  * ((results - P)/ W)) / denom)
-        return est
-    
-    def convert_param_form(self, params):
-        return np.array([-params[0] / params[1], 1 / params[1]])
-    
-    
-    # def train_em_mle(self, data) -> tuple:
-    #     return super().train_em_mle(data)
-    
-    # def plot_item_curve(self, p):
-    #     ability = np.linspace(-4, 4, 100)
-    #     for i in range(p.shape[1]):
-    #         plt.plot(ability, self.prob(ability, p[:,i].reshape(p.shape[0], 1)), label=f'Question{i+1}')        
-    #     plt.legend()
-    #     plt.savefig('item_curve.png')
-        
+    def estimate_ability(self, params: Union[list, np.ndarray], results: Union[list, np.ndarray],
+                         end=0.00000001, eps=0.01) -> np.ndarray:
+        """
+        Estimate the ability of an individual given the item parameters and responses.
+
+        Args:
+            params: A list or numpy array representing the item parameters.
+            results: A list or numpy array representing the item responses.
+            end: The convergence threshold.
+            eps: The threshold for detecting a near-singular matrix.
+
+        Returns:
+            A numpy array representing the estimated ability.
+        """
+        return PL2().estimate_ability([params[0], np.ones(len(params[0]))], results, end, eps)
```

### Comparing `openirt-0.1.2/setup.py` & `openirt-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 
 setup(
     name='openirt',
     packages = find_packages(include=['openirt']),
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     url='https://gitlab.com/pleased/...',
-    version='0.1.2',
+    version='0.1.3',
     description='Item response theory toolkit',
     author='Johan Hay',
     license='MIT',
 )
```

