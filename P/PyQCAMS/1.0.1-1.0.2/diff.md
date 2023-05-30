# Comparing `tmp/PyQCAMS-1.0.1.tar.gz` & `tmp/PyQCAMS-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQCAMS-1.0.1.tar", last modified: Sat May 27 21:38:30 2023, max compression
+gzip compressed data, was "PyQCAMS-1.0.2.tar", last modified: Tue May 30 00:05:48 2023, max compression
```

## Comparing `PyQCAMS-1.0.1.tar` & `PyQCAMS-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-27 21:38:30.076899 PyQCAMS-1.0.1/
--rwxrwxrwx   0 roots     (1000) roots     (1000)     1063 2023-03-30 15:34:08.000000 PyQCAMS-1.0.1/LICENSE
--rwxrwxrwx   0 roots     (1000) roots     (1000)     1416 2023-05-27 21:38:30.072898 PyQCAMS-1.0.1/PKG-INFO
-drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-27 21:38:29.790670 PyQCAMS-1.0.1/PyQCAMS.egg-info/
--rwxrwxrwx   0 roots     (1000) roots     (1000)     1416 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/PKG-INFO
--rwxrwxrwx   0 roots     (1000) roots     (1000)      307 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/SOURCES.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)        1 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/dependency_links.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)       96 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/requires.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)        8 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/top_level.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)      915 2023-05-27 21:12:06.000000 PyQCAMS-1.0.1/README.md
-drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-27 21:38:30.033182 PyQCAMS-1.0.1/pyqcams/
--rwxrwxrwx   0 roots     (1000) roots     (1000)       15 2023-04-03 15:05:00.000000 PyQCAMS-1.0.1/pyqcams/__init__.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)      273 2023-03-30 15:34:08.000000 PyQCAMS-1.0.1/pyqcams/constants.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)     2616 2023-05-22 15:19:49.000000 PyQCAMS-1.0.1/pyqcams/numv.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)     4528 2023-05-10 15:47:15.000000 PyQCAMS-1.0.1/pyqcams/plotters.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)     1986 2023-05-10 15:44:49.000000 PyQCAMS-1.0.1/pyqcams/psave.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)    33310 2023-05-27 21:05:23.000000 PyQCAMS-1.0.1/pyqcams/pymar.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)     5029 2023-05-27 21:05:26.000000 PyQCAMS-1.0.1/pyqcams/util.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)       38 2023-05-27 21:38:30.078899 PyQCAMS-1.0.1/setup.cfg
--rwxrwxrwx   0 roots     (1000) roots     (1000)      839 2023-05-27 21:37:45.000000 PyQCAMS-1.0.1/setup.py
+drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-30 00:05:48.794749 PyQCAMS-1.0.2/
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1063 2023-03-30 15:34:08.000000 PyQCAMS-1.0.2/LICENSE
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1049 2023-05-30 00:05:48.782381 PyQCAMS-1.0.2/PKG-INFO
+drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-30 00:05:48.250156 PyQCAMS-1.0.2/PyQCAMS.egg-info/
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1049 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/PKG-INFO
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      291 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/SOURCES.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)        1 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/dependency_links.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)       96 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/requires.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)        8 2023-05-30 00:05:47.000000 PyQCAMS-1.0.2/PyQCAMS.egg-info/top_level.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      564 2023-05-29 15:22:21.000000 PyQCAMS-1.0.2/README.md
+drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-30 00:05:48.686720 PyQCAMS-1.0.2/pyqcams/
+-rwxrwxrwx   0 roots     (1000) roots     (1000)       15 2023-04-03 15:05:00.000000 PyQCAMS-1.0.2/pyqcams/__init__.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      273 2023-03-30 15:34:08.000000 PyQCAMS-1.0.2/pyqcams/constants.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     4528 2023-05-10 15:47:15.000000 PyQCAMS-1.0.2/pyqcams/plotters.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1986 2023-05-10 15:44:49.000000 PyQCAMS-1.0.2/pyqcams/psave.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)    33455 2023-05-30 00:04:32.000000 PyQCAMS-1.0.2/pyqcams/pymar.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     4094 2023-05-30 00:04:16.000000 PyQCAMS-1.0.2/pyqcams/util.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)       38 2023-05-30 00:05:48.799754 PyQCAMS-1.0.2/setup.cfg
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      839 2023-05-30 00:05:42.000000 PyQCAMS-1.0.2/setup.py
```

### Comparing `PyQCAMS-1.0.1/LICENSE` & `PyQCAMS-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQCAMS-1.0.1/pyqcams/plotters.py` & `PyQCAMS-1.0.2/pyqcams/plotters.py`

 * *Files identical despite different names*

### Comparing `PyQCAMS-1.0.1/pyqcams/psave.py` & `PyQCAMS-1.0.2/pyqcams/psave.py`

 * *Files identical despite different names*

### Comparing `PyQCAMS-1.0.1/pyqcams/pymar.py` & `PyQCAMS-1.0.2/pyqcams/pymar.py`

 * *Files 3% similar despite different names*

```diff
@@ -423,20 +423,14 @@
             -self.dv1(r12)*r12drho1x-self.dv2(r32)*r32drho1x-self.dv3(r31)*r31drho1x,
             -self.dv1(r12)*r12drho1y-self.dv2(r32)*r32drho1y-self.dv3(r31)*r31drho1y,
             -self.dv1(r12)*r12drho1z-self.dv2(r32)*r32drho1z-self.dv3(r31)*r31drho1z,
             -self.dv2(r32)*r32drho2x-self.dv3(r31)*r31drho2x,
             -self.dv2(r32)*r32drho2y-self.dv3(r31)*r31drho2y,
             -self.dv2(r32)*r32drho2z-self.dv3(r31)*r31drho2z]
 
-        # No atom-molecule interaction
-        # f = [p1x/mu12, p1y/mu12, p1z/mu12, p2x/mu123, p2y/mu123, p2z/mu123,
-        #     -H2_Vdr(r12)*r12drho1x,
-        #     -H2_Vdr(r12)*r12drho1y,
-        #     -H2_Vdr(r12)*r12drho1z,
-        #     0,0,0]
         return f 
 
     
     def runT(self, doplot = False):
         '''Run the trajectory at impact parameter b.
         b, float
             impact parameter (bohr)
@@ -728,53 +722,46 @@
         dV = lambda r: -m*cm/r**(m+1)+n*cn/r**(n+1)
         return V, dV
 
     def buckingham(self, a=1., b=1., c6 = 1., max = .1,**kwargs):
         '''Usage:
             V = buckingham(**kwargs)
         Buckingham potentials tend to come back down at low r. 
-        We fix this by adding a piecewise wall.
+        We fix this by imposing xmin at the turning point "max."
         Return a one-dimensional Buckingham potential:
         V(r) = a*exp(-b*r) - c6/r^6 for r > r_x
-        V(r) = 
 
         Keyword arguments:
         a, float
             short-range multiplicative factor
         b, float
             short-range exponential factor
         c6, float
             dispersion coefficient
         tp, float
             guess of turning point
         xmin, float
             minimum of potential (cutoff at local maximum)        
         xmax, float
             maximum of potential
+
+        Outputs:
+        Buck, function
+            buckingham potential
+        dBuck, function
+            derivative of buckingham potential
+        xi, float
+            minimum x-value where Buck is defined
         '''
         Buck = lambda r: a*np.exp(-b*r) - c6/r**6
         dBuck = lambda r: -a*b*np.exp(-b*r) + 6*c6/r**7
         ddBuck = lambda r: a*b**2*np.exp(-b*r) - 6*7*c6/r**8
 
         # Find the maximum of potential
         xi = fsolve(dBuck,max)
-        # xi = fsolve(ddBuck,ip)
-        # m =  dBuck(xi)
-        # yi = Buck(xi)
-        # Wall = lambda r:2*m*r + (yi - 2*m*xi)
-        # dWall =  lambda r: 2*m
-
-        # # Define piecewise nd_array within interpolation bounds
-        # x = np.linspace(xmin,xmax,n)
-        # Vx = np.piecewise(x,[x<xi,x>=xi], [Wall,Buck])
-        # dVx = np.piecewise(x,[x<xi,x>=xi], [dWall,dBuck])
-
-        # #Interpolate the nd array into a new function
-        # V = interp1d(x,Vx)
-        # dV = interp1d(x,dVx)
         
         return Buck, dBuck, xi
     
     
 
 ### make potentials ### 
 def start(input_file):
@@ -787,14 +774,15 @@
     potential_AB = data['potential_AB'] # which potential
     potential_BC = data['potential_BC']
     potential_CA = data['potential_CA']
     vList = ['morse','buck','lj']
     vF = Potential()
     m1,m2,m3 = data['masses'].values() # masses
     m12 = m1*m2/(m1+m2)
+    xmin = None
 
     if potential_AB in vList:
         mol1 = data['potential_params']["AB"][f"{potential_AB}"]  # potential parameters
         if potential_AB == 'morse':
                 mol1_V, mol1_dV = vF.morse(**mol1)
         elif potential_AB == 'lj':
             mol1_V, mol1_dV = vF.lj(**mol1)
@@ -808,39 +796,50 @@
         xvals, mol1_V, mol1_dV, mol1['re'] = util.numToV(f'{potential_AB}') # Find V, dV via spline
         xmin = min(xvals)
         xmax = max(xvals)
 
     # Create energy object according to chosen potential
     AB = Energy(mu=m12, npts=data['potential_params']["AB"]['npts'], xmin = xmin,
                 xmax = xmax, j = data['ji'])
-    AB.turningPts(mol1_V,mol1['re'], v= data['vi']) # Assign attributies evals, rm, rp
-        
+    AB.turningPts(mol1_V,mol1['re'], v= data['vi']) # Assign attributies evals, rm, rp    
     if potential_BC in vList:
         mol2 = data['potential_params']["BC"][f"{potential_BC}"]
         if potential_BC == 'morse':
             mol2_V, mol2_dV = vF.morse(**mol2)
         elif potential_BC == 'lj':
             mol2_V, mol2_dV = vF.lj(**mol2)
         elif potential_BC == 'buck':
             mol2_V, mol2_dV, _ = vF.buckingham(**mol2)
     else:
         mol2 = {}
-        _, mol2_V, mol2_dV, mol2['re'] = util.numToV(f'{potential_BC}')
-
+        r_bc, mol2_V, mol2_dV, mol2['re'] = util.numToV(f'{potential_BC}')
+        # Ensure calculation is within bounds of potential data 
+        if data['r0'] < min(r_bc):
+            print(f'Initial distance must be greater than minimum r value provided ({min(r_bc)}).')
+            quit()
+        if data['int_params']['r_stop'] > max(r_bc):
+            print(f'Stop condition too large! Ensure "r_stop" <= maximum r value of potential ({max(r_bc)}).')
+            quit()
     if potential_CA in vList:
         mol3 = data['potential_params']["CA"][f"{potential_CA}"]
         if potential_CA == 'morse':
             mol3_V, mol3_dV = vF.morse(**mol3)
         elif potential_CA == 'lj':
             mol3_V, mol3_dV = vF.lj(**mol3)
         elif potential_CA == 'buck':
             mol3_V, mol3_dV, _ = vF.buckingham(**mol3)
     else:
         mol3 = {}
-        _, mol3_V, mol3_dV, mol3['re'] = util.numToV(f'{potential_CA}')
+        r_ca, mol3_V, mol3_dV, mol3['re'] = util.numToV(f'{potential_CA}')
+        # Ensure calculation is within bounds of potential data 
+        if data['r0'] < min(r_ca):
+            print(f'Initial distance must be greater than minimum r value provided ({min(r_bc)}).')
+            quit()
+        if data['int_params']['r_stop'] > max(r_ca):
+            print(f'Stop condition too large! Ensure "r_stop" < maximum r value of potential ({max(r_ca)}).')
 
     # Calculate relevant attributes
     inputs = {'m1' : m1, 'm2': m2, 'm3': m3, 
          'd0' : data['r0'], 'e0' : data['Ec (K)']*constants.cEK2H,
          'b': data['b'],'mol': AB, 'v1' : mol1_V, 'v2' : mol2_V, 'v3':mol3_V,
          'dv1' : mol1_dV,'dv2': mol2_dV, 'dv3': mol3_dV,
          're1' : mol1['re'], 're2': mol2['re'], 're3': mol3['re'],
@@ -850,11 +849,7 @@
 ### Run a trajectory ###
 def main(plot = False,**kwargs):
     a = QCT(**kwargs)
     a.runT(doplot = plot)
     # result = {'d_e': a.delta_e}
     # return result
     return util.get_results(a)
-
-if __name__ == '__main__':
-    calc = start('example/h2_ca/inputs.json')
-    print(main(plot = True, **calc))
```

### Comparing `PyQCAMS-1.0.1/pyqcams/util.py` & `PyQCAMS-1.0.2/pyqcams/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -97,46 +97,27 @@
     num_V, function
         interpolated potential
     num_dV, function
         interpolated potential derivative
     num_re, float
         equilibrium point (min of potential)
     '''
-    types = ['.csv','.txt','.dat']
-    split = os.path.splitext(f'{file}')
-    filetype = split[1]
-    if filetype in types:
-        try:
-            # comma separated
-            df = pd.read_csv(f'{file}',header = None)
-            num_x = np.array([float(i) for i in df[0][:].values.tolist()])
-            num_y = np.array([float(i) for i in df[1][:].values.tolist()])
-        except:
-            try:
-                # tab separated
-                df = pd.read_csv(f'{file}',header = None, sep = '\s+')
-                num_x = np.array([float(i) for i in df[0][:].values.tolist()])
-                num_y = np.array([float(i) for i in df[1][:].values.tolist()])
-            except:
-                print('Please use either comma or tab separated data.')
-                quit()
-    else: 
-        print('Please specify filetype. Choose from "csv", "dat", or "txt".')
+    # types = ['.csv','.txt','.dat']
+    # split = os.path.splitext(f'{file}')
+    # filetype = split[1]
+    try:
+        df = pd.read_csv(f'{file}',header = None, sep = None, engine='python')
+        num_x = np.array([float(i) for i in df[0][:].values.tolist()])
+        num_y = np.array([float(i) for i in df[1][:].values.tolist()])
+    except Exception as e:
+            print(e)
+            quit()
     num_y -= num_y[-1] # Shift values to make curve approach 0 by setting final point to 0
-    num_V = InterpolatedUnivariateSpline(num_x,num_y, k = 4, ext = 'raise') # Use k = 4 to find roots of derivative
+    num_V = InterpolatedUnivariateSpline(num_x,num_y, k = 4) # Use k = 4 to find roots of derivative
     num_dV = num_V.derivative()
     cr_pts = num_dV.roots()
     cr_pts = np.append(cr_pts, (num_x[0], num_x[-1]))  # also check the endpoints of the interval
     cr_vals = num_V(cr_pts)
     min_index = np.argmin(cr_vals)
     num_re = cr_pts[min_index] # Equilibrium distance
     return num_x, num_V, num_dV, num_re
 
-if __name__ == '__main__':
-    import matplotlib.pyplot as plt
-    # num_x, num_V, num_dV, num_re = numToV(r"C:\Users\Rian\Documents\research\jesusgroup\cah_pec\cah_au.txt")
-    num_x, num_V, num_dV, num_re = numToV(r"C:\Users\Rian\Documents\research\jesusgroup\cah_pec\h2_pec.dat")
-    x = np.linspace(min(num_x),max(num_x),500)
-    # plt.scatter(num_x, num_y)
-    plt.plot(x, num_V(x))
-    plt.plot(num_re, num_V(num_re), marker = 'o')
-    plt.show()
```

### Comparing `PyQCAMS-1.0.1/setup.py` & `PyQCAMS-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory/"README.md").read_text()
 
 setup(
     name = 'PyQCAMS',
-    version = '1.0.1',
+    version = '1.0.2',
     description = 'Python Quasi Classical Atom Molecule Scattering',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Rian Koots',
     author_email = 'rian.koots@stonybrook.edu',
     url = 'https://github.com/Rkoost/PyQCAMS',
     packages = find_packages(),
```

