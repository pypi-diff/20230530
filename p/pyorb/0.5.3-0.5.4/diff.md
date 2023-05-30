# Comparing `tmp/pyorb-0.5.3.tar.gz` & `tmp/pyorb-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyorb-0.5.3.tar", last modified: Fri Mar 17 09:04:17 2023, max compression
+gzip compressed data, was "pyorb-0.5.4.tar", last modified: Tue May 30 13:30:07 2023, max compression
```

## Comparing `pyorb-0.5.3.tar` & `pyorb-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 09:04:17.766128 pyorb-0.5.3/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-03-02 14:58:25.000000 pyorb-0.5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7814 2023-03-17 09:04:17.766128 pyorb-0.5.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6208 2023-03-15 12:10:26.000000 pyorb-0.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 09:04:17.762128 pyorb-0.5.3/pyorb/
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-03-02 22:10:59.000000 pyorb-0.5.3/pyorb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    45316 2023-03-02 14:58:25.000000 pyorb-0.5.3/pyorb/kepler.py
--rw-rw-rw-   0 root         (0) root         (0)    35308 2023-03-02 14:58:25.000000 pyorb-0.5.3/pyorb/orbit.py
--rw-rw-rw-   0 root         (0) root         (0)     2884 2023-03-02 14:58:25.000000 pyorb-0.5.3/pyorb/unit.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-17 08:49:23.000000 pyorb-0.5.3/pyorb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 09:04:17.762128 pyorb-0.5.3/pyorb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7814 2023-03-17 09:04:17.000000 pyorb-0.5.3/pyorb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2023-03-17 09:04:17.000000 pyorb-0.5.3/pyorb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 09:04:17.000000 pyorb-0.5.3/pyorb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2023-03-17 09:04:17.000000 pyorb-0.5.3/pyorb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-17 09:04:17.000000 pyorb-0.5.3/pyorb.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-03-17 09:04:17.766128 pyorb-0.5.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-03-02 14:58:25.000000 pyorb-0.5.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 09:04:17.766128 pyorb-0.5.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)    11596 2023-03-02 14:58:25.000000 pyorb-0.5.3/tests/test_kepler_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    15329 2023-03-02 14:58:25.000000 pyorb-0.5.3/tests/test_orbit.py
--rw-rw-rw-   0 root         (0) root         (0)    14953 2023-03-15 12:10:26.000000 pyorb-0.5.3/tests/test_orbit_transformations.py
--rw-rw-rw-   0 root         (0) root         (0)     1123 2023-03-02 14:58:25.000000 pyorb-0.5.3/tests/test_rotations.py
--rw-rw-rw-   0 root         (0) root         (0)     2492 2023-03-15 12:10:26.000000 pyorb-0.5.3/tests/test_solvers.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-03-02 14:58:25.000000 pyorb-0.5.3/tests/test_units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:30:07.377869 pyorb-0.5.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-03-02 14:58:25.000000 pyorb-0.5.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7814 2023-05-30 13:30:07.377869 pyorb-0.5.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6208 2023-03-15 12:10:26.000000 pyorb-0.5.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:30:07.369870 pyorb-0.5.4/pyorb/
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-03-02 22:10:59.000000 pyorb-0.5.4/pyorb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    45210 2023-05-30 13:12:35.000000 pyorb-0.5.4/pyorb/kepler.py
+-rw-rw-rw-   0 root         (0) root         (0)    35308 2023-03-02 14:58:25.000000 pyorb-0.5.4/pyorb/orbit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2023-05-30 13:12:35.000000 pyorb-0.5.4/pyorb/unit.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-30 13:12:35.000000 pyorb-0.5.4/pyorb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:30:07.369870 pyorb-0.5.4/pyorb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7814 2023-05-30 13:30:07.000000 pyorb-0.5.4/pyorb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-30 13:30:07.000000 pyorb-0.5.4/pyorb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:30:07.000000 pyorb-0.5.4/pyorb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 13:30:07.000000 pyorb-0.5.4/pyorb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-30 13:30:07.000000 pyorb-0.5.4/pyorb.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-05-30 13:12:35.000000 pyorb-0.5.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-05-30 13:30:07.377869 pyorb-0.5.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-03-02 14:58:25.000000 pyorb-0.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:30:07.377869 pyorb-0.5.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    11596 2023-03-02 14:58:25.000000 pyorb-0.5.4/tests/test_kepler_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    16686 2023-05-30 13:12:35.000000 pyorb-0.5.4/tests/test_orbit.py
+-rw-rw-rw-   0 root         (0) root         (0)    14953 2023-03-15 12:10:26.000000 pyorb-0.5.4/tests/test_orbit_transformations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2023-03-02 14:58:25.000000 pyorb-0.5.4/tests/test_rotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2023-03-15 12:10:26.000000 pyorb-0.5.4/tests/test_solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3354 2023-05-30 13:12:35.000000 pyorb-0.5.4/tests/test_units.py
```

### Comparing `pyorb-0.5.3/LICENSE` & `pyorb-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyorb-0.5.3/PKG-INFO` & `pyorb-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorb
-Version: 0.5.3
+Version: 0.5.4
 Summary: Keplerian orbit functions in Python
 Author: Daniel Kastinen
 Author-email: daniel.kastinen@irf.se
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pyorb-0.5.3/README.md` & `pyorb-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyorb-0.5.3/pyorb/kepler.py` & `pyorb-0.5.4/pyorb/kepler.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,46 +19,47 @@
 
 **Reference**: NIST - http://physics.nist.gov/cgi-bin/cuu/Value?bg
 '''
 
 AU = 1.495978707e11
 '''float: Astronomical Unit [m]
 
-The mean distance between the sun and the earth as defined in 
+The mean distance between the sun and the earth as defined in
 "International Astronomical Union, 31 August 2012"
 '''
 
 
 M_earth = 398600.5e9/G
 '''float: Mass of the Earth using the WGS84 convention [kg]
 '''
 
 M_sol = 1.98847e30
 """float: The mass of the sun :math:`M_\\odot` given in kg
 
-**Reference**: The Astronomical Almanac - 
+**Reference**: The Astronomical Almanac -
 http://asa.usno.navy.mil/static/files/2014/Astronomical_Constants_2014.pdf
 """
 
 e_lim = 1e-9
 """float: The limit on eccentricity below witch an orbit is considered circular
 """
 
 i_lim = np.pi*1e-9
-"""float: The limit on inclination in radians below witch an orbit is 
+"""float: The limit on inclination in radians below witch an orbit is
 considered not inclined
 """
 
 
 def cart_to_equi(cart, mu=M_sol*G, degrees=False):
     '''TODO
 
-    Converts set of Cartesian state vectors to set of Equinoctial orbital 
+    Converts set of Cartesian state vectors to set of Equinoctial orbital
     elements.
     '''
+    raise NotImplementedError()
     if not isinstance(cart, np.ndarray):
         raise TypeError('Input type {} not supported: must be {}'.format(
             type(cart), np.ndarray))
     if cart.shape[0] != 6:
         raise ValueError(
             f'Input data must have at least 6 variables along axis 0: \
             input shape is {cart.shape}')
@@ -77,23 +78,22 @@
     if degrees:
         pass
 
     if input_is_vector:
         cart.shape = (6,)
         # o.shape = (6,)
 
-    raise NotImplementedError()
-
 
 def equi_to_cart(equi, mu=M_sol*G, degrees=False):
     '''TODO
 
-    Converts set of Equinoctial orbital elements to set of Cartesian state 
+    Converts set of Equinoctial orbital elements to set of Cartesian state
     vectors.
     '''
+    raise NotImplementedError()
     if not isinstance(equi, np.ndarray):
         raise TypeError('Input type {} not supported: must be {}'.format(
             type(equi), np.ndarray))
     if equi.shape[0] != 6:
         raise ValueError(
             f'Input data must have at least 6 variables along axis 0: \
             input shape is {equi.shape}')
@@ -112,27 +112,26 @@
     if degrees:
         pass
 
     if input_is_vector:
         equi.shape = (6,)
         # o.shape = (6,)
 
-    raise NotImplementedError()
-
 
 def kep_to_equi(kep, degrees=False):
     '''TODO
 
     a, h, k, p, q, lambda0,
 
     **Reference:**
-        Broucke, R.A., Cefola, P.J., 1972. On the equinoctial orbit elements. 
+        Broucke, R.A., Cefola, P.J., 1972. On the equinoctial orbit elements.
         Celestial Mechanics 5, 303–310. https://doi.org/10.1007/BF01228432
 
     '''
+    raise NotImplementedError()
 
     om_bar = kep[3, ...] + kep[4, ...]
     om = kep[4, ...]
     hi = 0.5*kep[2, ...]
     lambda0 = om_bar + kep[5, ...]
     if degrees:
         om_bar = np.radians(om_bar)
@@ -152,14 +151,15 @@
 
     return elems
 
 
 def equi_to_kep(equi, degrees=False):
     '''TODO
     '''
+    raise NotImplementedError()
 
     kep = np.empty(equi.shape, dtype=equi.dtype)
 
     kep[0, ...] = equi[0, ...]
     kep[1, ...] = np.sqrt(equi[1, ...]**2 + equi[2, ...]**2)
     hi = np.arcsin(np.sqrt(equi[3, ...]**2 + equi[4, ...]**2))
     kep[2, ...] = 2*hi
@@ -174,112 +174,112 @@
     kep[3, ...] = lam - kep[4, ...]
     kep[5, ...] = equi[5, ...] - lam
 
     return kep
 
 
 def cart_to_kep(cart, mu=M_sol*G, degrees=False):
-    '''Converts set of Cartesian state vectors to set of Keplerian orbital 
+    '''Converts set of Cartesian state vectors to set of Keplerian orbital
     elements.
 
     Parameters
     ----------
-    kep : numpy.ndarray kep
-        (6, N) or (6, ) array of Cartesian state vectors where rows correspond 
-        to :math:`x`, :math:`y`, :math:`z`, :math:`v_x`, :math:`v_y`, 
+    kep : numpy.ndarray
+        (6, N) or (6, ) array of Cartesian state vectors where rows correspond
+        to :math:`x`, :math:`y`, :math:`z`, :math:`v_x`, :math:`v_y`,
         :math:`v_z` and columns correspond to different objects.
     mu : float or numpy.ndarray
-        Float or (N, ) array with the standard gravitational parameter of 
-        objects. If :code:`mu` is a numpy vector, the element corresponding to 
-        each column of :code:`cart` will be used for its element calculation, 
+        Float or (N, ) array with the standard gravitational parameter of
+        objects. If :code:`mu` is a numpy vector, the element corresponding to
+        each column of :code:`cart` will be used for its element calculation,
         Default value is in SI units a massless object orbiting the Sun.
     degrees : bool
         If :code:`True`, use degrees. Else all angles are given in radians.
 
     Returns
     -------
     numpy.ndarray
-        (6, N) or (6, ) array of Keplerian orbital elements where rows 
-        correspond to :math:`a`, :math:`e`, :math:`i`, :math:`\\omega`, 
-        :math:`\\Omega`, :math:`\\nu` and columns correspond to different 
+        (6, N) or (6, ) array of Keplerian orbital elements where rows
+        correspond to :math:`a`, :math:`e`, :math:`i`, :math:`\\omega`,
+        :math:`\\Omega`, :math:`\\nu` and columns correspond to different
         objects.
-    
+
     Notes
     -----
     Transform
-        Basic functionality is largley based on standard literature like [1]_. 
+        Basic functionality is largley based on standard literature like [1]_.
         Some open source material is avalible like these `Orbital-mechanics notes on GitHub <https://orbital-mechanics.space/intro.html>`_ .
 
     Arbitrary constants used
        * :mod:`~pyorb.kepler.e_lim`: Used to determine circular orbits
        * :mod:`~pyorb.kepler.i_lim`: Used to determine non-inclined orbits
 
     Variables
         * :math:`a`: Semi-major axis
         * :math:`e`: Eccentricity
         * :math:`i`: Inclination
         * :math:`\\omega`: Argument of perihelion
         * :math:`\\Omega`: Longitude of ascending node
         * :math:`\\nu`: True anoamly
         * :math:`\\mu`: Standard gravitational parameter for the two body problem: :math:`G(M_1 + M_2)`.
-    
+
     Units
-       Using default standard gravitational parameter :code:`mu` 
-       (:math:`\\mu`), all variables are in `SI Units 
-       <https://www.nist.gov/pml/weights-and-measures/metric-si/si-units>`_ 
-       If a :code:`mu` is given in other units, all other input variables 
-       should also use the same unit system. Angles are by default given as 
-       radians, all angles are radians internally in functions, input and 
-       output angles can be both radians and degrees depending on the 
+       Using default standard gravitational parameter :code:`mu`
+       (:math:`\\mu`), all variables are in `SI Units
+       <https://www.nist.gov/pml/weights-and-measures/metric-si/si-units>`_
+       If a :code:`mu` is given in other units, all other input variables
+       should also use the same unit system. Angles are by default given as
+       radians, all angles are radians internally in functions, input and
+       output angles can be both radians and degrees depending on the
        :code:`degrees` boolean.
 
 
     Orientation of the ellipse in the coordinate system [2]_
         For 0 inclination :math:`i`: the ellipse is located in the x-y plane.
 
-        The direction of motion as True anoamly :math:`\\nu`: increases for a 
-        zero inclination :math:`i`: orbit is anti-coockwise, i.e. from +x 
+        The direction of motion as True anoamly :math:`\\nu`: increases for a
+        zero inclination :math:`i`: orbit is anti-coockwise, i.e. from +x
         towards +y.
 
-        If the eccentricity :math:`e`: is increased, the periapsis will lie in 
+        If the eccentricity :math:`e`: is increased, the periapsis will lie in
         +x direction.
 
-        If the inclination :math:`i`: is increased, the ellipse will rotate 
+        If the inclination :math:`i`: is increased, the ellipse will rotate
         around the x-axis, so that +y is rotated toward +z.
 
-        An increase in Longitude of ascending node :math:`\\Omega`: 
-        corresponds to a rotation around the z-axis so that +x is rotated 
+        An increase in Longitude of ascending node :math:`\\Omega`:
+        corresponds to a rotation around the z-axis so that +x is rotated
         toward +y.
 
-        Changing argument of perihelion :math:`\\omega`: will not change the 
+        Changing argument of perihelion :math:`\\omega`: will not change the
         plane of the orbit, it will rotate the orbit in the plane.
 
         The periapsis is shifted in the direction of motion.
 
     .. [1] A.E. Roy. "Orbital Motion"
     .. [2] D.A. Vallado. "Fundamentals of Astrodynamics and Applications"
 
     Examples
     --------
-    
+
     Example of using the base conversion function to transform from
     kepler elements to cartesian coordinates
 
     >>> import pyorb
     >>> import numpy as np
     >>> G = pyorb.get_G(length='AU', mass='Msol', time='y')
     >>> G
     39.47812018693255
     >>> cart = np.array([
     ...     0.70710678,  0.70710678, 0.,
     ...     -4.4428662, 4.4428662, 0.,
     ... ])
     >>> kep = pyorb.cart_to_kep(
-    ...     cart, 
-    ...     mu=1*G, 
+    ...     cart,
+    ...     mu=1*G,
     ...     degrees=True,
     ... )
 
     See Also
     --------
     kep_to_cart : Convert from cartesian to kepler
 
@@ -415,15 +415,15 @@
     cos_nu = np.empty_like(hn)
 
     # three cases
     # elliptical and hyperbolic: (angle from periapsis using e and r)
     cos_nu[eg] = np.sum(e[:, eg]*r[:, eg], axis=0)/(o[1, eg]*rn[eg])
 
     # circular and inclined: (angle from periapsis using n and r)
-    # if e=0 and omega := 0, with inclination +y -> +z perihelion is ascending 
+    # if e=0 and omega := 0, with inclination +y -> +z perihelion is ascending
     # node
     cos_nu[el_ig] = np.sum(
         (n[:, el_ig]/nn[el_ig])*(r[:, el_ig]/rn[el_ig]),
         axis=0,
     )
 
     # circular and planar: (use angle of position vector)
@@ -465,45 +465,45 @@
 
     return o
 
 
 def orbit_total_angular_momentum(a, e, mu):
     '''Calculates the total angular momentum from orbital parameters.
 
-    :param float/numpy.ndarray a: Semi-major axis of (>0) ellipse or (<0) 
+    :param float/numpy.ndarray a: Semi-major axis of (>0) ellipse or (<0)
         hyperbola.
-    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), parabola 
+    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), parabola
         (e==1) or hyperbola (e>1).
-    :param float/numpy.ndarray mu: Standard gravitation parameter 
+    :param float/numpy.ndarray mu: Standard gravitation parameter
         :math:`\\mu = G(m_1 + m_2)` of the orbit.
 
     :return: Total angular momentum.
     '''
     return np.sqrt(mu*a*(1 - e**2))
 
 
 def parabolic_total_angular_momentum(q, mu):
     '''Calculates the total angular momentum from orbital parameters.
 
     :param float/numpy.ndarray q: Periapsis-distance of parabola.
-    :param float/numpy.ndarray mu: Standard gravitation parameter 
+    :param float/numpy.ndarray mu: Standard gravitation parameter
         :math:`\\mu = G(m_1 + m_2)` of the orbit.
 
     :return: Total angular momentum.
     '''
     return np.sqrt(mu*2*q)
 
 
 def true_to_eccentric(nu, e, degrees=False):
     '''Calculates the eccentric anomaly from the true anomaly.
 
     :param float/numpy.ndarray nu: True anomaly.
-    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), parabola 
+    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), parabola
         (e==1) or hyperbola (e>1).
-    :param bool degrees: If true degrees are used, else all angles are given in 
+    :param bool degrees: If true degrees are used, else all angles are given in
         radians
 
     :return: Eccentric anomaly.
     :rtype: numpy.ndarray or float
     '''
     if degrees:
         _nu = np.radians(nu)
@@ -545,19 +545,19 @@
 
     return E
 
 
 def eccentric_to_true(E, e, degrees=False):
     '''Calculates the true anomaly from the eccentric anomaly.
 
-    :param float/numpy.ndarray E: elliptic, parabolic or hyperbolic eccentric 
+    :param float/numpy.ndarray E: elliptic, parabolic or hyperbolic eccentric
         anomaly.
-    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), 
+    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1),
         parabola (e==1) or hyperbola (e>1).
-    :param bool degrees: If true degrees are used, else all angles are given in 
+    :param bool degrees: If true degrees are used, else all angles are given in
         radians
 
     :return: True anomaly.
     :rtype: numpy.ndarray or float
     '''
     if degrees:
         _E = np.radians(E)
@@ -596,22 +596,22 @@
     if degrees:
         nu = np.degrees(nu)
 
     return nu
 
 
 def eccentric_to_mean(E, e, degrees=False):
-    '''Calculates the mean anomaly from the (elliptic, parabolic or hyperbolic) 
+    '''Calculates the mean anomaly from the (elliptic, parabolic or hyperbolic)
     eccentric anomaly using Kepler equation.
 
-    :param float/numpy.ndarray E: elliptic, parabolic or hyperbolic eccentric 
+    :param float/numpy.ndarray E: elliptic, parabolic or hyperbolic eccentric
         anomaly.
-    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), 
+    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1),
         parabola (e==1) or hyperbola (e>1).
-    :param bool degrees: If true degrees are used, else all angles are given in 
+    :param bool degrees: If true degrees are used, else all angles are given in
         radians
 
     :return: Mean anomaly.
     :rtype: numpy.ndarray or float
     '''
     if degrees:
         _E = np.radians(E)
@@ -647,17 +647,17 @@
     return M
 
 
 def true_to_mean(nu, e, degrees=False):
     '''Transforms true anomaly to mean anomaly.
 
     :param float/numpy.ndarray nu: True anomaly.
-    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), 
+    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1),
         parabola (e==1) or hyperbola (e>1).
-    :param bool degrees: If true degrees are used, else all angles are given in 
+    :param bool degrees: If true degrees are used, else all angles are given in
         radians
 
     :return: Mean anomaly.
     :rtype: numpy.ndarray or float
     '''
     if degrees:
         _nu = np.radians(nu)
@@ -669,86 +669,86 @@
 
     if degrees:
         M = np.degrees(M)
     return M
 
 
 def orbital_distance(h, mu, e, nu, degrees=False):
-    '''Calculates the distance between the left focus point of an 
+    '''Calculates the distance between the left focus point of an
     ellipse (e<1), parabola (e==1) or hyperbola (e>1) and a
     point on the orbit defined by the true anomaly.
 
     :param float/numpy.ndarray h: Orbit total angular momentum.
     :param float/numpy.ndarray mu: Standard gravitation parameter.
-    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), 
+    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1),
         parabola (e==1) or hyperbola (e>1).
     :param float/numpy.ndarray nu: True anomaly.
-    :param bool degrees: If true degrees are used, else all angles are given in 
+    :param bool degrees: If true degrees are used, else all angles are given in
         radians
 
     :return: Radius from left focus point.
     :rtype: numpy.ndarray or float
     '''
     if degrees:
         _nu = np.radians(nu)
     else:
         _nu = nu
 
     return h**2/(mu*(1 + e*np.cos(_nu)))
 
 
 def elliptic_radius(E, a, e, degrees=False):
-    '''Calculates the distance between the left focus point of an ellipse and a 
+    '''Calculates the distance between the left focus point of an ellipse and a
     point on the ellipse defined by the eccentric anomaly.
 
     :param float/numpy.ndarray E: Eccentric anomaly.
     :param float/numpy.ndarray a: Semi-major axis of ellipse.
     :param float/numpy.ndarray e: Eccentricity of ellipse.
-    :param bool degrees: If true degrees are used, else all angles are given in 
+    :param bool degrees: If true degrees are used, else all angles are given in
         radians
 
     :return: Radius from left focus point.
     :rtype: numpy.ndarray or float
     '''
     if degrees:
         _E = np.radians(E)
     else:
         _E = E
 
     return a*(1.0 - e*np.cos(_E))
 
 
 def parabolic_radius(nu, q, degrees=False):
-    '''Calculates the distance between the left focus point of an parabola and 
+    '''Calculates the distance between the left focus point of an parabola and
     a point on the parabola defined by the eccentric anomaly.
 
     :param float/numpy.ndarray nu: True anomaly.
     :param float/numpy.ndarray q: Periapsis-distance of parabola.
-    :param bool degrees: If true degrees are used, else all angles are given in 
+    :param bool degrees: If true degrees are used, else all angles are given in
         radians
 
     :return: Radius from left focus point.
     :rtype: numpy.ndarray or float
     '''
     if degrees:
         _nu = np.radians(nu)
     else:
         _nu = nu
 
     return 2.0*q/(1.0 + np.cos(_nu))
 
 
 def hyperbolic_radius(nu, a, e, degrees=False):
-    '''Calculates the distance between the left focus point of an hyperbola and 
+    '''Calculates the distance between the left focus point of an hyperbola and
         a point on the hyperbola defined by the hyperbolic anomaly.
 
     :param float/numpy.ndarray nu: True anomaly.
     :param float/numpy.ndarray a: Semi-transverse axis of hyperbola (positive).
     :param float/numpy.ndarray e: Eccentricity of hyperbola.
-    :param bool degrees: If true degrees are used, else all angles are given in 
+    :param bool degrees: If true degrees are used, else all angles are given in
         radians
 
     :return: Radius from left focus point.
     :rtype: numpy.ndarray or float
     '''
     if degrees:
         _nu = np.radians(nu)
@@ -809,37 +809,37 @@
     R[1, 0] = np.sin(theta)
     R[1, 1] = np.cos(theta)
     R[2, 2] = 1.0
     return R
 
 
 def laguerre_solve_kepler(E0, M, e, tol=1e-12, max_iter=5000, degree=5):
-    '''Solve the Kepler equation using the The Laguerre Algorithm, a algorithm 
+    '''Solve the Kepler equation using the The Laguerre Algorithm, a algorithm
     that guarantees global convergence.
 
-    Absolute numerical tolerance is defined as :math:`|f(E)| < tol` where 
-    :math:`f(E) = M - E + e \\sin(E)` or where 
+    Absolute numerical tolerance is defined as :math:`|f(E)| < tol` where
+    :math:`f(E) = M - E + e \\sin(E)` or where
     :math:`f(E) = M + E - e \\sinh(E)`.
 
     # TODO: implement in C and bind using ctypes
 
-    *Note:* Choice of polynomial degree does not matter significantly for 
+    *Note:* Choice of polynomial degree does not matter significantly for
         convergence rate.
 
     :param float E0: Initial guess for eccentric anomaly.
     :param float M: Mean anomaly.
     :param float e: Eccentricity of ellipse or hyperbola.
     :param float tol: Absolute numerical tolerance eccentric anomaly.
     :param int max_iter: Maximum number of iterations before solver is aborted.
     :param int degree: Polynomial degree in derivation of Laguerre Algorithm.
     :return: Eccentric anomaly and number of iterations.
     :rtype: tuple of (float, int)
 
-    *Reference:* Conway, B. A. (1986). An improved algorithm due to Laguerre 
-        for the solution of Kepler's equation. 
+    *Reference:* Conway, B. A. (1986). An improved algorithm due to Laguerre
+        for the solution of Kepler's equation.
         Celestial mechanics, 39(2), 199-211.
 
     **Example:**
 
     .. code-block:: python
 
        import pyorb.kepler as pykep
@@ -854,30 +854,30 @@
           tol = 1e-12,
        )
     '''
 
     degree = float(degree)
 
     if e > 1:
-        def _f(E): 
+        def _f(E):
             return M + E - e*np.sinh(E)
 
-        def _fp(E): 
+        def _fp(E):
             return 1.0 - e*np.cosh(E)
 
-        def _fpp(E): 
+        def _fpp(E):
             return -e*np.sinh(E)
     else:
-        def _f(E): 
+        def _f(E):
             return M - E + e*np.sin(E)
 
-        def _fp(E): 
+        def _fp(E):
             return e*np.cos(E) - 1.0
 
-        def _fpp(E): 
+        def _fpp(E):
             return -e*np.sin(E)
 
     E = E0
 
     f_eval = _f(E)
 
     it_num = 0
@@ -906,43 +906,43 @@
         if it_num >= max_iter:
             break
 
     return E, it_num
 
 
 def _get_hyperbolic_kepler_guess(M, e):
-    '''The different initial guesses for solving the Kepler equation based on 
+    '''The different initial guesses for solving the Kepler equation based on
     input mean anomaly
 
     :param float M: Mean anomaly in radians.
     :param float e: Eccentricity of hyperbola.
     :return: Guess for eccentric anomaly in radians.
     :rtype: float
 
-    Reference: T. M. Burkardt and J. M. A. Danby, “The solutions of Kepler’s 
-        equation. II,” Celestial Mechanics, vol. 31, pp. 317–328, Nov. 1983, 
+    Reference: T. M. Burkardt and J. M. A. Danby, “The solutions of Kepler’s
+        equation. II,” Celestial Mechanics, vol. 31, pp. 317–328, Nov. 1983,
         doi: 10.1007/BF01844230.
     '''
 
     E0 = np.log(2*M/e + 1.8)
 
     return E0
 
 
 def _get_kepler_guess(M, e):
-    '''The different initial guesses for solving the Kepler equation based on 
+    '''The different initial guesses for solving the Kepler equation based on
     input mean anomaly
 
     :param float M: Mean anomaly in radians.
     :param float e: Eccentricity of ellipse.
     :return: Guess for eccentric anomaly in radians.
     :rtype: float
 
-    Reference: Esmaelzadeh, R., & Ghadiri, H. (2014). Appropriate starter for 
-        solving the Kepler's equation. 
+    Reference: Esmaelzadeh, R., & Ghadiri, H. (2014). Appropriate starter for
+        solving the Kepler's equation.
         International Journal of Computer Applications, 89(7).
     '''
     if M > np.pi:
         _M = 2.0*np.pi - M
     else:
         _M = M
 
@@ -959,24 +959,24 @@
     return E0
 
 
 def kepler_guess(M, e):
     '''Guess the initial iteration point for newtons method.
 
     :param float/numpy.ndarray M: Mean anomaly in radians.
-    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), 
+    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1),
         parabola (e==1) or hyperbola (e>1).
     :return: Guess for eccentric anomaly in radians.
     :rtype: numpy.ndarray or float
 
-    *Reference:* Esmaelzadeh, R., & Ghadiri, H. (2014). Appropriate starter for 
-        solving the Kepler's equation. 
+    *Reference:* Esmaelzadeh, R., & Ghadiri, H. (2014). Appropriate starter for
+        solving the Kepler's equation.
         International Journal of Computer Applications, 89(7).
-    *Reference:* T. M. Burkardt and J. M. A. Danby, “The solutions of Kepler’s 
-        equation. II,” Celestial Mechanics, vol. 31, pp. 317–328, Nov. 1983, 
+    *Reference:* T. M. Burkardt and J. M. A. Danby, “The solutions of Kepler’s
+        equation. II,” Celestial Mechanics, vol. 31, pp. 317–328, Nov. 1983,
         doi: 10.1007/BF01844230.
     '''
 
     if isinstance(M, np.ndarray) or isinstance(e, np.ndarray):
         if not isinstance(M, np.ndarray):
             M = np.ones(e.shape, dtype=e.dtype)*M
         if not isinstance(e, np.ndarray):
@@ -1009,34 +1009,34 @@
         else:
             E0 = _get_kepler_guess(M, e)
 
     return E0
 
 
 def mean_to_eccentric(M, e, solver_options=None, degrees=False):
-    '''Calculates the eccentric anomaly from the mean anomaly by solving the 
+    '''Calculates the eccentric anomaly from the mean anomaly by solving the
     Kepler equation.
 
     :param float/numpy.ndarray M: Mean anomaly.
-    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), 
+    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1),
         parabola (e==1) or hyperbola (e>1).
-    :param dict solver_options: Options for the numerical solution of Kepler's 
+    :param dict solver_options: Options for the numerical solution of Kepler's
         equation. See `pyorb.kepler.laguerre_solve_kepler` for information.
     :param bool degrees: If true degrees are used, else all angles are given in
         radians
 
     :return: True anomaly.
     :rtype: numpy.ndarray or float
 
     **Note:**
-        * For parabolic orbits the equation is analytic and solvable, ref: 
-            *Montenbruck, Oliver; Pfleger, Thomas (2009). Astronomy on the 
-            Personal Computer. Springer-Verlag Berlin Heidelberg. 
+        * For parabolic orbits the equation is analytic and solvable, ref:
+            *Montenbruck, Oliver; Pfleger, Thomas (2009). Astronomy on the
+            Personal Computer. Springer-Verlag Berlin Heidelberg.
             ISBN 978-3-540-67221-0. p 64*
-        * For hyperbolic orbits the hyperbolic sine is used in the Kepler 
+        * For hyperbolic orbits the hyperbolic sine is used in the Kepler
             equation.
 
     **Uses:**
        * :func:`~pyorb.kepler._get_kepler_guess`
        * :func:`~pyorb.kepler.laguerre_solve_kepler`
     '''
     if solver_options is None:
@@ -1104,19 +1104,19 @@
     return E
 
 
 def mean_to_true(M, e, solver_options=None, degrees=False):
     '''Transforms mean anomaly to true anomaly.
 
     :param float/numpy.ndarray M: Mean anomaly.
-    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1), 
+    :param float/numpy.ndarray e: Eccentricity of ellipse (e<1),
         parabola (e==1) or hyperbola (e>1).
-    :param dict solver_options: Options for the numerical solution of Kepler's 
+    :param dict solver_options: Options for the numerical solution of Kepler's
         equation. See `pyorb.kepler.laguerre_solve_kepler` for information.
-    :param bool degrees: If true degrees are used, else all angles are given 
+    :param bool degrees: If true degrees are used, else all angles are given
         in radians
 
     :return: True anomaly.
     :rtype: numpy.ndarray or float
     '''
     if degrees:
         _M = np.radians(M)
@@ -1129,46 +1129,46 @@
     if degrees:
         nu = np.degrees(nu)
 
     return nu
 
 
 def orbital_speed(r, a, mu):
-    '''Calculates the orbital speed at a given radius for an Keplerian orbit 
+    '''Calculates the orbital speed at a given radius for an Keplerian orbit
     :math:`v = \\sqrt{\\mu \\left (\\frac{2}{r} - \\frac{1}{a} \\right )}`.
 
     :param float/numpy.ndarray r: Radius from the pericenter.
-    :param float/numpy.ndarray a: Semi-major axis of (>0) ellipse or (<0) 
+    :param float/numpy.ndarray a: Semi-major axis of (>0) ellipse or (<0)
         hyperbola.
-    :param float/numpy.ndarray mu: Standard gravitation parameter 
+    :param float/numpy.ndarray mu: Standard gravitation parameter
         :math:`\\mu = G(m_1 + m_2)` of the orbit.
     :return: Orbital speed.
     '''
     return np.sqrt(mu*(2.0/r - 1.0/a))
 
 
 def orbital_period(a, mu):
-    '''Calculates the orbital period of an Keplerian orbit based on the 
+    '''Calculates the orbital period of an Keplerian orbit based on the
     semi-major axis :math:`P = 2\\pi\\sqrt{\\frac{a^3}{\\mu}}`.
 
     :param float/numpy.ndarray a: Semi-major axis of ellipse.
-    :param float/numpy.ndarray mu: Standard gravitation parameter 
+    :param float/numpy.ndarray mu: Standard gravitation parameter
         :math:`\\mu = G(m_1 + m_2)` of the orbit.
     :return: Orbital period.
     '''
     return 2.0*np.pi*np.sqrt(a**3.0/mu)
 
 
 def semi_major_axis(P, mu):
-    '''Calculates the orbital semi-major axis of an Keplerian orbit based on 
+    '''Calculates the orbital semi-major axis of an Keplerian orbit based on
     the orbital period :math:`a = \\mu^{\\frac{1}{3}}
     (\\frac{P}{2\\pi})^{\\frac{2}{3}}`.
 
     :param float/numpy.ndarray P: Orbital period
-    :param float/numpy.ndarray mu: Standard gravitation parameter 
+    :param float/numpy.ndarray mu: Standard gravitation parameter
         :math:`\\mu = G(m_1 + m_2)` of the orbit.
     :return: semi-major axis.
     '''
     a = np.cbrt((P/(2.0*np.pi))**2*mu)
     return a
 
 
@@ -1185,15 +1185,15 @@
 
     return theta_inf
 
 
 def stumpff0(x):
     '''Calculates the Stumpff function number 0 value.
 
-    **Reference**: Fundamentals of Celestial Mechanics 
+    **Reference**: Fundamentals of Celestial Mechanics
         (Second Edition) (Hardback) [J.M.A. Danby - 1992]
 
     :param numpy.ndarray x: Stumpff input variable.
     :return: Stumpff function value.
     '''
     c0 = np.empty_like(x)
     inds = x > 0
@@ -1205,15 +1205,15 @@
     c0[inds] = np.cosh(np.sqrt(-x[inds]))
     return c0
 
 
 def stumpff1(x):
     '''Calculates the Stumpff function number 1 value.
 
-    **Reference**: Fundamentals of Celestial Mechanics 
+    **Reference**: Fundamentals of Celestial Mechanics
         (Second Edition) (Hardback) [J.M.A. Danby - 1992]
 
     :param numpy.ndarray x: Stumpff input variable.
     :return: Stumpff function value.
     '''
     c1 = np.empty_like(x)
     inds = x > 0
@@ -1225,15 +1225,15 @@
     c1[inds] = np.sinh(np.sqrt(-x[inds]))/np.sqrt(-x[inds])
     return c1
 
 
 def stumpff2(x):
     '''Calculates the Stumpff function number 2 value.
 
-    **Reference**: Fundamentals of Celestial Mechanics 
+    **Reference**: Fundamentals of Celestial Mechanics
         (Second Edition) (Hardback) [J.M.A. Danby - 1992]
 
     :param numpy.ndarray x: Stumpff input variable.
     :return: Stumpff function value.
     '''
     c2 = np.empty_like(x)
     inds = x > 0
@@ -1245,15 +1245,15 @@
     c2[inds] = (1 - np.cosh(np.sqrt(-x[inds])))/x[inds]
     return c2
 
 
 def stumpff3(x):
     '''Calculates the Stumpff function number 3 value.
 
-    **Reference**: Fundamentals of Celestial Mechanics 
+    **Reference**: Fundamentals of Celestial Mechanics
         (Second Edition) (Hardback) [J.M.A. Danby - 1992]
 
     :param numpy.ndarray x: Stumpff input variable.
     :return: Stumpff function value.
     '''
     c3 = np.empty_like(x)
     inds = x > 0
@@ -1267,37 +1267,37 @@
     c3[inds] = (xsq - np.sinh(xsq))/(xsq*x[inds])
     return c3
 
 
 def stumpff(x):
     '''Calculate the 0-3 stumpff functions.
 
-    These Stumpff function are used in the universal variable 
-    formulation of the kepler orbit. 
+    These Stumpff function are used in the universal variable
+    formulation of the kepler orbit.
 
     The `n`'th' Stumpff function is defined as:
     :math:`c_{n}(x) = \\sum^{\\infty}_{j=0} \\frac{(-1)^j x^j}{(n + 2j)!}`.
 
-    However, it can be found that the first Stumpff functions can be expressed 
+    However, it can be found that the first Stumpff functions can be expressed
     in terms of trigonometric functions,
-    as this is implemented here and only `c0, c1, c2, c3` are used in the 
+    as this is implemented here and only `c0, c1, c2, c3` are used in the
     universal variable formulation of a kepler orbit.
     '''
     return stumpff0(x), stumpff1(x), stumpff2(x), stumpff3(x)
 
 
 def euler_rotation_matrix(inc, omega, Omega, degrees=False):
-    '''Generate the rotation matrix for the intrinsic rotation sequence Z-X-Z 
-    used by keplerian orbital elements of (i, Omega, omega). 
+    '''Generate the rotation matrix for the intrinsic rotation sequence Z-X-Z
+    used by keplerian orbital elements of (i, Omega, omega).
 
-    If any of the input angles are vectors the matrix will expand along a the 
+    If any of the input angles are vectors the matrix will expand along a the
     remaining axis.
 
-    Appendix I (p. 483) of: Roithmayr, Carlos M.; Hodges, Dewey H. (2016), 
-    Dynamics: Theory and Application of Kane's Method (1st ed.), 
+    Appendix I (p. 483) of: Roithmayr, Carlos M.; Hodges, Dewey H. (2016),
+    Dynamics: Theory and Application of Kane's Method (1st ed.),
     Cambridge University Press
     '''
     if isinstance(inc, np.ndarray):
         R = np.empty((3, 3, inc.size), dtype=np.float64)
     elif isinstance(omega, np.ndarray):
         R = np.empty((3, 3, omega.size), dtype=np.float64)
     elif isinstance(Omega, np.ndarray):
@@ -1338,104 +1338,104 @@
     R[1, 2, ...] = -c1*s2
     R[2, 2, ...] = c2
 
     return R
 
 
 def kep_to_cart(kep, mu=M_sol*G, degrees=False):
-    '''Converts set of Keplerian orbital elements to set of Cartesian state 
+    '''Converts set of Keplerian orbital elements to set of Cartesian state
     vectors.
 
     Parameters
     ----------
     kep : numpy.ndarray kep
-        (6, N) or (6, ) array of Keplerian orbital elements where rows 
-        correspond to :math:`a`, :math:`e`, :math:`i`, :math:`\\omega`, 
-        :math:`\\Omega`, :math:`\\nu` and columns correspond to different 
+        (6, N) or (6, ) array of Keplerian orbital elements where rows
+        correspond to :math:`a`, :math:`e`, :math:`i`, :math:`\\omega`,
+        :math:`\\Omega`, :math:`\\nu` and columns correspond to different
         objects.
     mu : float or numpy.ndarray
-        Float or (N, ) array with the standard gravitational parameter of 
-        objects. If :code:`mu` is a numpy vector, the element corresponding to 
-        each column of :code:`cart` will be used for its element calculation, 
+        Float or (N, ) array with the standard gravitational parameter of
+        objects. If :code:`mu` is a numpy vector, the element corresponding to
+        each column of :code:`cart` will be used for its element calculation,
         Default value is in SI units a massless object orbiting the Sun.
     degrees : bool
         If :code:`True`, use degrees. Else all angles are given in radians.
 
     Returns
     -------
     numpy.ndarray
-        (6, N) or (6, ) array of cartesian state vector(s) where rows 
-        correspond to :math:`x`, :math:`y`, :math:`z`, :math:`v_x`, 
+        (6, N) or (6, ) array of cartesian state vector(s) where rows
+        correspond to :math:`x`, :math:`y`, :math:`z`, :math:`v_x`,
         :math:`v_y`, :math:`v_z` and columns correspond to different objects.
-    
+
     Notes
     -----
     Transform
-        Basic functionality is largley based on standard literature like [1]_. 
+        Basic functionality is largley based on standard literature like [1]_.
         Some open source material is avalible like these `Orbital-mechanics notes on GitHub <https://orbital-mechanics.space/intro.html>`_ .
 
     Variables
         * :math:`a`: Semi-major axis
         * :math:`e`: Eccentricity
         * :math:`i`: Inclination
         * :math:`\\omega`: Argument of perihelion
         * :math:`\\Omega`: Longitude of ascending node
         * :math:`\\nu`: True anoamly
         * :math:`\\mu`: Standard gravitational parameter for the two body problem: :math:`G(M_1 + M_2)`.
-    
+
     Units
-       Using default standard gravitational parameter :code:`mu` 
-       (:math:`\\mu`), all variables are in `SI Units 
-       <https://www.nist.gov/pml/weights-and-measures/metric-si/si-units>`_ 
-       If a :code:`mu` is given in other units, all other input variables 
-       should also use the same unit system. Angles are by default given as 
-       radians, all angles are radians internally in functions, input and 
-       output angles can be both radians and degrees depending on the 
+       Using default standard gravitational parameter :code:`mu`
+       (:math:`\\mu`), all variables are in `SI Units
+       <https://www.nist.gov/pml/weights-and-measures/metric-si/si-units>`_
+       If a :code:`mu` is given in other units, all other input variables
+       should also use the same unit system. Angles are by default given as
+       radians, all angles are radians internally in functions, input and
+       output angles can be both radians and degrees depending on the
        :code:`degrees` boolean.
 
     Orientation of the ellipse in the coordinate system [2]_
         For 0 inclination :math:`i`: the ellipse is located in the x-y plane.
 
-        The direction of motion as True anoamly :math:`\\nu`: increases for a 
-        zero inclination :math:`i`: orbit is anti-coockwise, i.e. from +x 
+        The direction of motion as True anoamly :math:`\\nu`: increases for a
+        zero inclination :math:`i`: orbit is anti-coockwise, i.e. from +x
         towards +y.
 
-        If the eccentricity :math:`e`: is increased, the periapsis will lie in 
+        If the eccentricity :math:`e`: is increased, the periapsis will lie in
         +x direction.
 
-        If the inclination :math:`i`: is increased, the ellipse will rotate 
+        If the inclination :math:`i`: is increased, the ellipse will rotate
         around the x-axis, so that +y is rotated toward +z.
 
-        An increase in Longitude of ascending node :math:`\\Omega`: 
-        corresponds to a rotation around the z-axis so that +x is rotated 
+        An increase in Longitude of ascending node :math:`\\Omega`:
+        corresponds to a rotation around the z-axis so that +x is rotated
         toward +y.
 
-        Changing argument of perihelion :math:`\\omega`: will not change the 
+        Changing argument of perihelion :math:`\\omega`: will not change the
         plane of the orbit, it will rotate the orbit in the plane.
 
         The periapsis is shifted in the direction of motion.
 
     .. [1] A.E. Roy. "Orbital Motion"
     .. [2] D.A. Vallado. "Fundamentals of Astrodynamics and Applications"
 
     Examples
     --------
-    
+
     Example of using the base conversion function to transform from
     kepler elements to cartesian coordinates
 
     >>> import pyorb
     >>> import numpy as np
     >>> G = pyorb.get_G(length='AU', mass='Msol', time='y')
     >>> G
     39.47812018693255
     >>> kep = np.array([1, 0, 0, 0, 0, 45.0])
     >>> cart = pyorb.kep_to_cart(
-    ...     kep, 
-    ...     mu=1*G, 
+    ...     kep,
+    ...     mu=1*G,
     ...     degrees=True,
     ... )
     >>> cart
     array([ 0.70710678,  0.70710678,  0.        , -4.4428662 ,  4.4428662 ,
             0.        ])
 
     See Also
@@ -1456,15 +1456,15 @@
             kep.shape = (6, 1)
         except ValueError as e:
             print(f'Error {e} while trying to cast vector into single column.')
             print(f'Input array shape: {kep.shape}')
             raise
     else:
         input_is_vector = False
-    
+
     if not isinstance(mu, np.ndarray):
         mu = np.full((kep.shape[1],), mu, dtype=np.float64)
 
     x = np.empty(kep.shape, dtype=kep.dtype)
 
     if degrees:
         kep[2:, :] = np.radians(kep[2:, :])
```

### Comparing `pyorb-0.5.3/pyorb/orbit.py` & `pyorb-0.5.4/pyorb/orbit.py`

 * *Files identical despite different names*

### Comparing `pyorb-0.5.3/pyorb/unit.py` & `pyorb-0.5.4/pyorb/unit.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,36 +68,41 @@
         _length = length
     else:
         raise TypeError(f'Type "{type(length)}" for length not supported')
 
     return G_SI*(_mass*_time**2/_length**3)
 
 
-def angle_units(in_arg_inds, in_arg_keys, out_arg_inds):
-    '''Wrapper to automatically convert input arguemnts from degrees to radians 
-    and back to degrees if the keyword argument `degrees = True`.
+def angle_units(in_arg_inds, in_arg_keys, out_arg_inds, degrees=False):
+    '''Wrapper to automatically convert input arguments from degrees to radians
+    and back to degrees if the keyword argument `degrees = True`. The default
+    behavior is dictated by the wrapper `degrees` keyword argument.
     '''
 
     def angle_converter_warpper(func):
         def wrapped_func(*args, **kwargs):
-            if not kwargs.pop('degrees', False):
+            if not kwargs.pop('degrees', degrees):
                 return func(*args, **kwargs)
 
             args = list(args)
             if in_arg_inds is not None:
                 for ind in in_arg_inds:
                     args[ind] = np.radians(args[ind])
             if in_arg_keys is not None:
                 for key in in_arg_keys:
                     if key in kwargs:
                         kwargs[key] = np.radians(kwargs[key])
 
             ret = func(*args, **kwargs)
 
-            ret = list(ret)
-            if out_arg_inds is not None:
-                for ind in out_arg_inds:
-                    ret[ind] = np.degrees(ret[ind])
+            if out_arg_inds is not None and ret is not None:
+                if isinstance(out_arg_inds, bool):
+                    ret = np.degrees(ret)
+                else:
+                    ret = list(ret)
+                    for ind in out_arg_inds:
+                        ret[ind] = np.degrees(ret[ind])
+                    ret = tuple(ret)
 
-                return ret
+            return ret
         return wrapped_func
     return angle_converter_warpper
```

### Comparing `pyorb-0.5.3/pyorb.egg-info/PKG-INFO` & `pyorb-0.5.4/pyorb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyorb
-Version: 0.5.3
+Version: 0.5.4
 Summary: Keplerian orbit functions in Python
 Author: Daniel Kastinen
 Author-email: daniel.kastinen@irf.se
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pyorb-0.5.3/setup.cfg` & `pyorb-0.5.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -26,25 +26,30 @@
 develop = 
 	pytest >= 6.2.5
 	sphinx >= 4.2.0
 	flake8 >= 4.0.1
 	wheel >= 0.37.0
 	build >= 0.7.0
 	twine >= 3.4.2
-	coverage >= 6.0.2
+	pytest-cov >= 4.1.0
 	sphinx-gallery >= 0.3.1
 	matplotlib >= 3.5.1
 	nbsphinx >= 0.8.8
 	ipykernel >= 6.9.1
 	radon >= 5.1.0
 	numpydoc >= 1.2
 	pre-commit > 3.0.0
+	black >= 23.3.0
 
 [flake8]
 ignore = D203,E251,E126,E226,W291
 max-line-length = 79
 exclude = pyorb/__pycache__,pyorb/__init__.py
 
+[radon]
+exclude = test_*.py
+cc_min = B
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyorb-0.5.3/tests/test_kepler_functions.py` & `pyorb-0.5.4/tests/test_kepler_functions.py`

 * *Files identical despite different names*

### Comparing `pyorb-0.5.3/tests/test_orbit.py` & `pyorb-0.5.4/tests/test_orbit.py`

 * *Files 6% similar despite different names*

```diff
@@ -368,18 +368,19 @@
         nt.assert_almost_equal(anom, orb.true_anomaly)
 
 
 class TestOrbitProperties(unittest.TestCase):
 
     def setUp(self):
         self.kep_orb = dict(
-            a=1, e=0.2, i=3, 
-            omega=10, Omega=20, anom=90, 
-            degrees=True,
+            a=1, e=0.2, i=3,
+            omega=10, Omega=20, anom=90,
+            degrees=True, type='true',
         )
+        self.d_ang = 130.0
         self.G = pyorb.get_G(length='AU', mass='Msol', time='y')
         self.M0 = 1
         self.m = 0.1
         self.orb = Orbit(M0=self.M0, G=self.G, m=self.m, **self.kep_orb)
         self.cart = self.orb.cartesian
         self.kep = self.orb.kepler
 
@@ -456,14 +457,53 @@
         self.orb.Omega = 0
         with self.assertRaises(AssertionError):
             nt.assert_array_almost_equal(self.orb.cartesian, self.cart)
 
     def test_anom(self):
         assert self.orb.anom == self.kep_orb['anom']
 
+    def test_mean_anomaly(self):
+        M = pyorb.true_to_mean(
+            self.kep_orb['anom'],
+            self.kep_orb['e'],
+            degrees=self.kep_orb['degrees'],
+        )
+        assert self.orb.mean_anomaly[0] == M
+
+        self.orb.mean_anomaly = M + self.d_ang
+        nt.assert_almost_equal(self.orb.mean_anomaly[0], M + self.d_ang)
+        assert self.orb.anom[0] == pyorb.mean_to_true(
+            M + self.d_ang,
+            self.kep_orb['e'],
+            degrees=self.kep_orb['degrees'],
+        )
+
+    def test_eccentric_anomaly(self):
+        ecc = pyorb.true_to_eccentric(
+            self.kep_orb['anom'],
+            self.kep_orb['e'],
+            degrees=self.kep_orb['degrees'],
+        )
+        assert self.orb.eccentric_anomaly[0] == ecc
+
+        self.orb.eccentric_anomaly = ecc + self.d_ang
+
+        nt.assert_almost_equal(self.orb.eccentric_anomaly[0], ecc + self.d_ang)
+        assert self.orb.anom[0] == pyorb.eccentric_to_true(
+            ecc + self.d_ang,
+            self.kep_orb['e'],
+            degrees=self.kep_orb['degrees'],
+        )
+
+    def test_true_anomaly(self):
+        assert self.orb.true_anomaly == self.kep_orb['anom']
+        self.orb.true_anomaly = self.kep_orb['anom'] + self.d_ang
+        assert self.orb.true_anomaly == self.kep_orb['anom'] + self.d_ang
+
+
     def test_set_anom(self):
         self.orb.anom = 0
         with self.assertRaises(AssertionError):
             nt.assert_array_almost_equal(self.orb.cartesian, self.cart)
 
     def test_x(self):
         assert self.orb.x == self.cart[0]
```

### Comparing `pyorb-0.5.3/tests/test_orbit_transformations.py` & `pyorb-0.5.4/tests/test_orbit_transformations.py`

 * *Files identical despite different names*

### Comparing `pyorb-0.5.3/tests/test_rotations.py` & `pyorb-0.5.4/tests/test_rotations.py`

 * *Files identical despite different names*

### Comparing `pyorb-0.5.3/tests/test_solvers.py` & `pyorb-0.5.4/tests/test_solvers.py`

 * *Files identical despite different names*

