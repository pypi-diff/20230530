# Comparing `tmp/underactuated-2023.4.17.tar.gz` & `tmp/underactuated-2023.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "underactuated-2023.4.17.tar", last modified: Mon Apr 17 15:18:20 2023, max compression
+gzip compressed data, was "underactuated-2023.5.29.tar", last modified: Tue May 30 09:58:27 2023, max compression
```

## Comparing `underactuated-2023.4.17.tar` & `underactuated-2023.5.29.tar`

### file list

```diff
@@ -1,120 +1,122 @@
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.027175 underactuated-2023.4.17/
--rw-r--r--   0 russt      (504) staff       (20)     1703 2021-12-11 10:13:05.000000 underactuated-2023.4.17/LICENSE.TXT
--rw-r--r--   0 russt      (504) staff       (20)       85 2023-04-16 10:35:33.000000 underactuated-2023.4.17/MANIFEST.in
--rw-r--r--   0 russt      (504) staff       (20)     1065 2023-04-17 15:18:20.027270 underactuated-2023.4.17/PKG-INFO
--rw-r--r--   0 russt      (504) staff       (20)      550 2022-10-02 15:34:42.000000 underactuated-2023.4.17/README.md
--rw-r--r--   0 russt      (504) staff       (20)      609 2023-03-16 10:55:11.000000 underactuated-2023.4.17/pyproject.toml
--rw-r--r--   0 russt      (504) staff       (20)     3169 2023-04-17 15:18:20.027966 underactuated-2023.4.17/setup.cfg
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:19.999704 underactuated-2023.4.17/underactuated/
--rw-r--r--   0 russt      (504) staff       (20)      311 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/__init__.py
--rw-r--r--   0 russt      (504) staff       (20)     1692 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/double_integrator.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.000847 underactuated-2023.4.17/underactuated/exercises/
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.001547 underactuated-2023.4.17/underactuated/exercises/acrobot/
--rw-r--r--   0 russt      (504) staff       (20)    14129 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/acrobot/test_cartpole_balancing.py
--rw-r--r--   0 russt      (504) staff       (20)    12035 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/acrobot/test_cartpoles_urdf.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.001848 underactuated-2023.4.17/underactuated/exercises/contact/
--rw-r--r--   0 russt      (504) staff       (20)     7965 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/contact/test_compass_gait_limit_cycle.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.002848 underactuated-2023.4.17/underactuated/exercises/dp/
--rw-r--r--   0 russt      (504) staff       (20)     5595 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/exercises/dp/minimum_time_utils.py
--rw-r--r--   0 russt      (504) staff       (20)      796 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/dp/test_lp_dp.py
--rw-r--r--   0 russt      (504) staff       (20)     1315 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/dp/test_minimum_time.py
--rw-r--r--   0 russt      (504) staff       (20)     9872 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/dp/test_pendulum_cvi.py
--rw-r--r--   0 russt      (504) staff       (20)     4542 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/grader.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.003094 underactuated-2023.4.17/underactuated/exercises/humanoids/
--rw-r--r--   0 russt      (504) staff       (20)     6496 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/humanoids/test_footstep_planning.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.003311 underactuated-2023.4.17/underactuated/exercises/intro/
--rw-r--r--   0 russt      (504) staff       (20)     1802 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/intro/test_drake_systems.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.003549 underactuated-2023.4.17/underactuated/exercises/lqr/
--rw-r--r--   0 russt      (504) staff       (20)     5253 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/exercises/lqr/test_drake_diagrams.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.004480 underactuated-2023.4.17/underactuated/exercises/lyapunov/
--rw-r--r--   0 russt      (504) staff       (20)     7516 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/lyapunov/test_control.py
--rw-r--r--   0 russt      (504) staff       (20)     1302 2023-03-23 11:35:19.000000 underactuated-2023.4.17/underactuated/exercises/lyapunov/test_sos_and_psd.py
--rw-r--r--   0 russt      (504) staff       (20)     5349 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/lyapunov/test_van_der_pol.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.004849 underactuated-2023.4.17/underactuated/exercises/pend/
--rw-r--r--   0 russt      (504) staff       (20)     2636 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/pend/test_hopfield_network.py
--rw-r--r--   0 russt      (504) staff       (20)     1127 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/pend/test_vibrating_pendulum.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.005032 underactuated-2023.4.17/underactuated/exercises/planning/
--rw-r--r--   0 russt      (504) staff       (20)     5523 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/planning/test_rrt_planning.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.005197 underactuated-2023.4.17/underactuated/exercises/simple_legs/
--rw-r--r--   0 russt      (504) staff       (20)     6829 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/simple_legs/test_one_d_hopper.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.006672 underactuated-2023.4.17/underactuated/exercises/sysid/
--rw-r--r--   0 russt      (504) staff       (20)     1891 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/sysid/test_glider_sysid.py
--rw-r--r--   0 russt      (504) staff       (20)     2382 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/sysid/test_linear_sysid.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.007452 underactuated-2023.4.17/underactuated/exercises/trajopt/
--rw-r--r--   0 russt      (504) staff       (20)    10059 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/trajopt/test_ilqr_driving.py
--rw-r--r--   0 russt      (504) staff       (20)     4662 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/trajopt/test_orbital_transfer.py
--rw-r--r--   0 russt      (504) staff       (20)     9970 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/exercises/trajopt/test_shooting_vs_transcription.py
--rw-r--r--   0 russt      (504) staff       (20)     6016 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/jupyter.py
--rw-r--r--   0 russt      (504) staff       (20)      259 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/meshcat_cpp_utils.py
--rw-r--r--   0 russt      (504) staff       (20)    22418 2023-03-16 10:57:53.000000 underactuated-2023.4.17/underactuated/meshcat_utils.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.009859 underactuated-2023.4.17/underactuated/models/
--rw-r--r--   0 russt      (504) staff       (20)     2331 2022-07-13 01:24:22.000000 underactuated-2023.4.17/underactuated/models/cartpole.urdf
--rw-r--r--   0 russt      (504) staff       (20)     2879 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/compass_gait_limit_cycle.urdf
--rw-r--r--   0 russt      (504) staff       (20)     2151 2022-07-13 01:24:22.000000 underactuated-2023.4.17/underactuated/models/double_pendulum.sdf
--rw-r--r--   0 russt      (504) staff       (20)     2417 2022-07-13 01:24:22.000000 underactuated-2023.4.17/underactuated/models/double_pendulum.urdf
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.010161 underactuated-2023.4.17/underactuated/models/glider/
--rw-r--r--   0 russt      (504) staff       (20)     5943 2023-03-12 01:00:41.000000 underactuated-2023.4.17/underactuated/models/glider/glider.urdf
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.012122 underactuated-2023.4.17/underactuated/models/glider/meshes/
--rw-r--r--   0 russt      (504) staff       (20)     4411 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/elevator.obj
--rw-r--r--   0 russt      (504) staff       (20)     1192 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselageh_hstab.obj
--rw-r--r--   0 russt      (504) staff       (20)    17609 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselageh_main.obj
--rw-r--r--   0 russt      (504) staff       (20)    11270 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_main.obj
--rw-r--r--   0 russt      (504) staff       (20)     1664 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_top.obj
--rw-r--r--   0 russt      (504) staff       (20)     2316 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_vstab.obj
--rw-r--r--   0 russt      (504) staff       (20)     1460 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/wing_left.obj
--rw-r--r--   0 russt      (504) staff       (20)     1577 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/glider/meshes/wing_right.obj
--rw-r--r--   0 russt      (504) staff       (20)     5297 2023-04-09 21:56:41.000000 underactuated-2023.4.17/underactuated/models/kneed_compass_gait.urdf
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.013460 underactuated-2023.4.17/underactuated/models/littledog/
--rw-r--r--   0 russt      (504) staff       (20)     1679 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/LICENSE.txt
--rw-r--r--   0 russt      (504) staff       (20)    13333 2023-03-12 01:00:41.000000 underactuated-2023.4.17/underactuated/models/littledog/LittleDog.urdf
--rw-r--r--   0 russt      (504) staff       (20)      411 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/README.md
--rw-r--r--   0 russt      (504) staff       (20)      666 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/ground.urdf
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.026934 underactuated-2023.4.17/underactuated/models/littledog/meshes/
--rw-r--r--   0 russt      (504) staff       (20)    50176 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_hip.obj
--rw-r--r--   0 russt      (504) staff       (20)      200 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_hip.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)   121081 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_lower.obj
--rw-r--r--   0 russt      (504) staff       (20)      528 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_lower.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)   104694 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_upper.obj
--rw-r--r--   0 russt      (504) staff       (20)      512 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_upper.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)    51166 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_hip.obj
--rw-r--r--   0 russt      (504) staff       (20)      200 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_hip.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)   120989 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_lower.obj
--rw-r--r--   0 russt      (504) staff       (20)      528 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_lower.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)   105531 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_upper.obj
--rw-r--r--   0 russt      (504) staff       (20)      512 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_upper.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)  1036654 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/body.obj
--rw-r--r--   0 russt      (504) staff       (20)      357 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/body.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)    25320 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/body2.jpg
--rw-r--r--   0 russt      (504) staff       (20)    11322 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/body3.jpg
--rw-r--r--   0 russt      (504) staff       (20)    29266 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/foot.jpg
--rw-r--r--   0 russt      (504) staff       (20)    49151 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_hip.obj
--rw-r--r--   0 russt      (504) staff       (20)      200 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_hip.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)   121747 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_lower.obj
--rw-r--r--   0 russt      (504) staff       (20)      528 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_lower.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)   104401 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_upper.obj
--rw-r--r--   0 russt      (504) staff       (20)      512 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_upper.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)    58904 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_hip.obj
--rw-r--r--   0 russt      (504) staff       (20)      200 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_hip.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)   121685 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_lower.obj
--rw-r--r--   0 russt      (504) staff       (20)      528 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_lower.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)   104294 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_upper.obj
--rw-r--r--   0 russt      (504) staff       (20)      512 2022-01-14 11:58:31.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_upper.obj.mtl
--rw-r--r--   0 russt      (504) staff       (20)    21971 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/littledog/meshes/leg.jpg
--rw-r--r--   0 russt      (504) staff       (20)     2820 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/one_d_hopper.urdf
--rw-r--r--   0 russt      (504) staff       (20)     1723 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/undamped_cartpole.urdf
--rw-r--r--   0 russt      (504) staff       (20)     1444 2021-12-11 10:13:05.000000 underactuated-2023.4.17/underactuated/models/vibrating_pendulum.urdf
--rw-r--r--   0 russt      (504) staff       (20)      687 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/multibody.py
--rw-r--r--   0 russt      (504) staff       (20)     2341 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/optimizers.py
--rw-r--r--   0 russt      (504) staff       (20)      369 2023-03-12 01:00:41.000000 underactuated-2023.4.17/underactuated/package.xml
--rw-r--r--   0 russt      (504) staff       (20)     2296 2023-03-16 11:05:00.000000 underactuated-2023.4.17/underactuated/pendulum.py
--rw-r--r--   0 russt      (504) staff       (20)     1887 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/plot_utils.py
--rw-r--r--   0 russt      (504) staff       (20)      957 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/pyplot_visualizer.py
--rw-r--r--   0 russt      (504) staff       (20)     5263 2023-03-16 10:52:43.000000 underactuated-2023.4.17/underactuated/quadrotor2d.py
--rw-r--r--   0 russt      (504) staff       (20)     3971 2023-03-12 02:22:59.000000 underactuated-2023.4.17/underactuated/scenarios.py
--rw-r--r--   0 russt      (504) staff       (20)     2220 2023-04-14 12:16:55.000000 underactuated-2023.4.17/underactuated/utils.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-04-17 15:18:20.000677 underactuated-2023.4.17/underactuated.egg-info/
--rw-r--r--   0 russt      (504) staff       (20)     1065 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/PKG-INFO
--rw-r--r--   0 russt      (504) staff       (20)     4567 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/SOURCES.txt
--rw-r--r--   0 russt      (504) staff       (20)        1 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/dependency_links.txt
--rw-r--r--   0 russt      (504) staff       (20)       96 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/requires.txt
--rw-r--r--   0 russt      (504) staff       (20)       14 2023-04-17 15:18:19.000000 underactuated-2023.4.17/underactuated.egg-info/top_level.txt
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.024682 underactuated-2023.5.29/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1703 2022-03-07 00:40:42.000000 underactuated-2023.5.29/LICENSE.TXT
+-rw-rw-r--   0 russt     (1002) russt     (1002)       85 2023-04-29 22:17:35.000000 underactuated-2023.5.29/MANIFEST.in
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1065 2023-05-30 09:58:27.024682 underactuated-2023.5.29/PKG-INFO
+-rw-rw-r--   0 russt     (1002) russt     (1002)      550 2022-10-02 16:20:06.000000 underactuated-2023.5.29/README.md
+-rw-rw-r--   0 russt     (1002) russt     (1002)      609 2023-03-17 02:32:04.000000 underactuated-2023.5.29/pyproject.toml
+-rw-rw-r--   0 russt     (1002) russt     (1002)     3169 2023-05-30 09:58:27.028682 underactuated-2023.5.29/setup.cfg
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/
+-rw-rw-r--   0 russt     (1002) russt     (1002)      311 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/__init__.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1692 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/double_integrator.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/acrobot/
+-rw-rw-r--   0 russt     (1002) russt     (1002)    14129 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/acrobot/test_cartpole_balancing.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)    12035 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/acrobot/test_cartpoles_urdf.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/contact/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     7965 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/contact/test_compass_gait_limit_cycle.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/dp/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     5595 2023-03-14 16:52:01.000000 underactuated-2023.5.29/underactuated/exercises/dp/minimum_time_utils.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)      796 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/dp/test_lp_dp.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1315 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/dp/test_minimum_time.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     9872 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/dp/test_pendulum_cvi.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     4542 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/grader.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/humanoids/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2676 2023-04-29 22:17:35.000000 underactuated-2023.5.29/underactuated/exercises/humanoids/footstep_planning_gcs_utils.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     6496 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/humanoids/test_footstep_planning.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     4279 2023-04-29 22:17:35.000000 underactuated-2023.5.29/underactuated/exercises/humanoids/test_footstep_planning_gcs.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/intro/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1802 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/intro/test_drake_systems.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/lqr/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     5253 2023-03-14 16:52:01.000000 underactuated-2023.5.29/underactuated/exercises/lqr/test_drake_diagrams.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/lyapunov/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     7516 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/lyapunov/test_control.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1302 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/lyapunov/test_sos_and_psd.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     5349 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/lyapunov/test_van_der_pol.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/pend/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2636 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/pend/test_hopfield_network.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1127 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/pend/test_vibrating_pendulum.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/planning/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     5523 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/planning/test_rrt_planning.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/simple_legs/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     6829 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/simple_legs/test_one_d_hopper.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/sysid/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1891 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/sysid/test_glider_sysid.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2382 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/sysid/test_linear_sysid.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated/exercises/trajopt/
+-rw-rw-r--   0 russt     (1002) russt     (1002)    10059 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/trajopt/test_ilqr_driving.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     4662 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/trajopt/test_orbital_transfer.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     9970 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/exercises/trajopt/test_shooting_vs_transcription.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     6017 2023-05-29 23:58:39.000000 underactuated-2023.5.29/underactuated/jupyter.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)      259 2023-03-14 16:52:01.000000 underactuated-2023.5.29/underactuated/meshcat_cpp_utils.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)    22418 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/meshcat_utils.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.020682 underactuated-2023.5.29/underactuated/models/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2331 2022-08-16 10:06:31.000000 underactuated-2023.5.29/underactuated/models/cartpole.urdf
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2879 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/compass_gait_limit_cycle.urdf
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2151 2022-08-16 10:06:31.000000 underactuated-2023.5.29/underactuated/models/double_pendulum.sdf
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2417 2022-08-16 10:06:31.000000 underactuated-2023.5.29/underactuated/models/double_pendulum.urdf
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.020682 underactuated-2023.5.29/underactuated/models/glider/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     5943 2023-03-10 02:39:33.000000 underactuated-2023.5.29/underactuated/models/glider/glider.urdf
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.020682 underactuated-2023.5.29/underactuated/models/glider/meshes/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     4411 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/glider/meshes/elevator.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1192 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/glider/meshes/fuselageh_hstab.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)    17609 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/glider/meshes/fuselageh_main.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)    11270 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/glider/meshes/fuselagev_main.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1664 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/glider/meshes/fuselagev_top.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2316 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/glider/meshes/fuselagev_vstab.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1460 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/glider/meshes/wing_left.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1577 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/glider/meshes/wing_right.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)     5297 2023-04-29 22:17:35.000000 underactuated-2023.5.29/underactuated/models/kneed_compass_gait.urdf
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.020682 underactuated-2023.5.29/underactuated/models/littledog/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1679 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/LICENSE.txt
+-rw-rw-r--   0 russt     (1002) russt     (1002)    13333 2023-03-10 02:39:33.000000 underactuated-2023.5.29/underactuated/models/littledog/LittleDog.urdf
+-rw-rw-r--   0 russt     (1002) russt     (1002)      411 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/README.md
+-rw-rw-r--   0 russt     (1002) russt     (1002)      666 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/ground.urdf
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.024682 underactuated-2023.5.29/underactuated/models/littledog/meshes/
+-rw-rw-r--   0 russt     (1002) russt     (1002)    50176 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_hip.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      200 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_hip.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)   121081 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_lower.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      528 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_lower.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)   104694 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_upper.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      512 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_upper.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)    51166 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_hip.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      200 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_hip.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)   120989 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_lower.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      528 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_lower.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)   105531 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_upper.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      512 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_upper.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)  1036654 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/body.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      357 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/body.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)    25320 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/body2.jpg
+-rw-rw-r--   0 russt     (1002) russt     (1002)    11322 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/body3.jpg
+-rw-rw-r--   0 russt     (1002) russt     (1002)    29266 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/foot.jpg
+-rw-rw-r--   0 russt     (1002) russt     (1002)    49151 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_hip.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      200 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_hip.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)   121747 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_lower.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      528 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_lower.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)   104401 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_upper.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      512 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_upper.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)    58904 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_hip.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      200 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_hip.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)   121685 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_lower.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      528 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_lower.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)   104294 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_upper.obj
+-rw-rw-r--   0 russt     (1002) russt     (1002)      512 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_upper.obj.mtl
+-rw-rw-r--   0 russt     (1002) russt     (1002)    21971 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/littledog/meshes/leg.jpg
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2820 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/one_d_hopper.urdf
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1723 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/undamped_cartpole.urdf
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1444 2022-03-07 00:40:42.000000 underactuated-2023.5.29/underactuated/models/vibrating_pendulum.urdf
+-rw-rw-r--   0 russt     (1002) russt     (1002)      687 2023-03-14 16:52:01.000000 underactuated-2023.5.29/underactuated/multibody.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2341 2023-03-14 16:52:01.000000 underactuated-2023.5.29/underactuated/optimizers.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)      369 2023-03-10 02:39:33.000000 underactuated-2023.5.29/underactuated/package.xml
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2296 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/pendulum.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1887 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/plot_utils.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)      957 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/pyplot_visualizer.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     5263 2023-03-17 02:32:04.000000 underactuated-2023.5.29/underactuated/quadrotor2d.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     3971 2023-03-14 16:52:01.000000 underactuated-2023.5.29/underactuated/scenarios.py
+-rw-rw-r--   0 russt     (1002) russt     (1002)     2220 2023-04-29 22:17:35.000000 underactuated-2023.5.29/underactuated/utils.py
+drwxrwxr-x   0 russt     (1002) russt     (1002)        0 2023-05-30 09:58:27.016682 underactuated-2023.5.29/underactuated.egg-info/
+-rw-rw-r--   0 russt     (1002) russt     (1002)     1065 2023-05-30 09:58:26.000000 underactuated-2023.5.29/underactuated.egg-info/PKG-INFO
+-rw-rw-r--   0 russt     (1002) russt     (1002)     4696 2023-05-30 09:58:27.000000 underactuated-2023.5.29/underactuated.egg-info/SOURCES.txt
+-rw-rw-r--   0 russt     (1002) russt     (1002)        1 2023-05-30 09:58:26.000000 underactuated-2023.5.29/underactuated.egg-info/dependency_links.txt
+-rw-rw-r--   0 russt     (1002) russt     (1002)       96 2023-05-30 09:58:26.000000 underactuated-2023.5.29/underactuated.egg-info/requires.txt
+-rw-rw-r--   0 russt     (1002) russt     (1002)       14 2023-05-30 09:58:26.000000 underactuated-2023.5.29/underactuated.egg-info/top_level.txt
```

### Comparing `underactuated-2023.4.17/LICENSE.TXT` & `underactuated-2023.5.29/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/PKG-INFO` & `underactuated-2023.5.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: underactuated
-Version: 2023.4.17
+Version: 2023.5.29
 Summary: MIT 6.832 - Underactuated Robotics
 Home-page: https://underactuated.csail.mit.edu
 Author: Russ Tedrake
 Author-email: russt@mit.edu
 Project-URL: Bug Tracker, https://github.com/RussTedrake/underactuated/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `underactuated-2023.4.17/README.md` & `underactuated-2023.5.29/README.md`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/pyproject.toml` & `underactuated-2023.5.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/setup.cfg` & `underactuated-2023.5.29/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = underactuated
-version = 2023.04.17
+version = 2023.05.29
 author = Russ Tedrake
 author_email = russt@mit.edu
 description = MIT 6.832 - Underactuated Robotics
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://underactuated.csail.mit.edu
 project_urls = 
@@ -16,15 +16,15 @@
 
 [options]
 package_dir = 
 include_package_data = True
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	drake>=1.14.0
+	drake>=1.17.0
 	pandas
 	gradescope-utils>=0.4.0
 	mpld3>=0.5.1
 	pydot>=1.3.0
 	timeout-decorator>=0.4.1
 
 [pycodestyle]
```

### Comparing `underactuated-2023.4.17/underactuated/double_integrator.py` & `underactuated-2023.5.29/underactuated/double_integrator.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/acrobot/test_cartpole_balancing.py` & `underactuated-2023.5.29/underactuated/exercises/acrobot/test_cartpole_balancing.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/acrobot/test_cartpoles_urdf.py` & `underactuated-2023.5.29/underactuated/exercises/acrobot/test_cartpoles_urdf.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/contact/test_compass_gait_limit_cycle.py` & `underactuated-2023.5.29/underactuated/exercises/contact/test_compass_gait_limit_cycle.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/dp/minimum_time_utils.py` & `underactuated-2023.5.29/underactuated/exercises/dp/minimum_time_utils.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/dp/test_lp_dp.py` & `underactuated-2023.5.29/underactuated/exercises/dp/test_lp_dp.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/dp/test_minimum_time.py` & `underactuated-2023.5.29/underactuated/exercises/dp/test_minimum_time.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/dp/test_pendulum_cvi.py` & `underactuated-2023.5.29/underactuated/exercises/dp/test_pendulum_cvi.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/grader.py` & `underactuated-2023.5.29/underactuated/exercises/grader.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/humanoids/test_footstep_planning.py` & `underactuated-2023.5.29/underactuated/exercises/humanoids/test_footstep_planning.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/intro/test_drake_systems.py` & `underactuated-2023.5.29/underactuated/exercises/intro/test_drake_systems.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/lqr/test_drake_diagrams.py` & `underactuated-2023.5.29/underactuated/exercises/lqr/test_drake_diagrams.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/lyapunov/test_control.py` & `underactuated-2023.5.29/underactuated/exercises/lyapunov/test_control.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/lyapunov/test_sos_and_psd.py` & `underactuated-2023.5.29/underactuated/exercises/lyapunov/test_sos_and_psd.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/lyapunov/test_van_der_pol.py` & `underactuated-2023.5.29/underactuated/exercises/lyapunov/test_van_der_pol.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/pend/test_hopfield_network.py` & `underactuated-2023.5.29/underactuated/exercises/pend/test_hopfield_network.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/pend/test_vibrating_pendulum.py` & `underactuated-2023.5.29/underactuated/exercises/pend/test_vibrating_pendulum.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/planning/test_rrt_planning.py` & `underactuated-2023.5.29/underactuated/exercises/planning/test_rrt_planning.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/simple_legs/test_one_d_hopper.py` & `underactuated-2023.5.29/underactuated/exercises/simple_legs/test_one_d_hopper.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/sysid/test_glider_sysid.py` & `underactuated-2023.5.29/underactuated/exercises/sysid/test_glider_sysid.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/sysid/test_linear_sysid.py` & `underactuated-2023.5.29/underactuated/exercises/sysid/test_linear_sysid.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/trajopt/test_ilqr_driving.py` & `underactuated-2023.5.29/underactuated/exercises/trajopt/test_ilqr_driving.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/trajopt/test_orbital_transfer.py` & `underactuated-2023.5.29/underactuated/exercises/trajopt/test_orbital_transfer.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/exercises/trajopt/test_shooting_vs_transcription.py` & `underactuated-2023.5.29/underactuated/exercises/trajopt/test_shooting_vs_transcription.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/jupyter.py` & `underactuated-2023.5.29/underactuated/jupyter.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 def setup_matplotlib_backend(**kwargs):
     SetupMatplotlibBackend(**kwargs)
 
 
 # Inspired by https://github.com/Kirill888/jupyter-ui-poll but there *must* be a
 # better way. Ideas:
 #  - provide init() and cleanup() methods that could be called to pull out and
-#    replace the irrelevant events just once (instead of on every timestep).
+#    replace the irrelevant events just once (instead of on every time step).
 #    E.g. init(), simulator.AdvanceTo(10), cleanup().
 #  - whitelist widget events and only process them (instead of black-listing the
 #    execute_request).
 #  - do I actually need asyncio?  can I just write the events back?
 #
 # But I'll wait to see how much we use this before spending too much time on it.
 # BTW,
```

### Comparing `underactuated-2023.4.17/underactuated/meshcat_utils.py` & `underactuated-2023.5.29/underactuated/meshcat_utils.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/cartpole.urdf` & `underactuated-2023.5.29/underactuated/models/cartpole.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/compass_gait_limit_cycle.urdf` & `underactuated-2023.5.29/underactuated/models/compass_gait_limit_cycle.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/double_pendulum.sdf` & `underactuated-2023.5.29/underactuated/models/double_pendulum.sdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/double_pendulum.urdf` & `underactuated-2023.5.29/underactuated/models/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/glider/glider.urdf` & `underactuated-2023.5.29/underactuated/models/glider/glider.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/glider/meshes/elevator.obj` & `underactuated-2023.5.29/underactuated/models/glider/meshes/elevator.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselageh_hstab.obj` & `underactuated-2023.5.29/underactuated/models/glider/meshes/fuselageh_hstab.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselageh_main.obj` & `underactuated-2023.5.29/underactuated/models/glider/meshes/fuselageh_main.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_main.obj` & `underactuated-2023.5.29/underactuated/models/glider/meshes/fuselagev_main.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_top.obj` & `underactuated-2023.5.29/underactuated/models/glider/meshes/fuselagev_top.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/glider/meshes/fuselagev_vstab.obj` & `underactuated-2023.5.29/underactuated/models/glider/meshes/fuselagev_vstab.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/glider/meshes/wing_left.obj` & `underactuated-2023.5.29/underactuated/models/glider/meshes/wing_left.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/glider/meshes/wing_right.obj` & `underactuated-2023.5.29/underactuated/models/glider/meshes/wing_right.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/kneed_compass_gait.urdf` & `underactuated-2023.5.29/underactuated/models/kneed_compass_gait.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/LICENSE.txt` & `underactuated-2023.5.29/underactuated/models/littledog/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/LittleDog.urdf` & `underactuated-2023.5.29/underactuated/models/littledog/LittleDog.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/ground.urdf` & `underactuated-2023.5.29/underactuated/models/littledog/ground.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_hip.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_lower.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_lower.obj.mtl` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_upper.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_left_upper.obj.mtl` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_left_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_hip.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_lower.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_lower.obj.mtl` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_upper.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/back_right_upper.obj.mtl` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/back_right_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/body.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/body.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/body2.jpg` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/body2.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/body3.jpg` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/body3.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/foot.jpg` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/foot.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_hip.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_lower.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_lower.obj.mtl` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_upper.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_left_upper.obj.mtl` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_left_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_hip.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_hip.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_lower.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_lower.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_lower.obj.mtl` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_lower.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_upper.obj` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_upper.obj`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/front_right_upper.obj.mtl` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/front_right_upper.obj.mtl`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/littledog/meshes/leg.jpg` & `underactuated-2023.5.29/underactuated/models/littledog/meshes/leg.jpg`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/one_d_hopper.urdf` & `underactuated-2023.5.29/underactuated/models/one_d_hopper.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/undamped_cartpole.urdf` & `underactuated-2023.5.29/underactuated/models/undamped_cartpole.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/models/vibrating_pendulum.urdf` & `underactuated-2023.5.29/underactuated/models/vibrating_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/multibody.py` & `underactuated-2023.5.29/underactuated/multibody.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/optimizers.py` & `underactuated-2023.5.29/underactuated/optimizers.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/pendulum.py` & `underactuated-2023.5.29/underactuated/pendulum.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/plot_utils.py` & `underactuated-2023.5.29/underactuated/plot_utils.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/pyplot_visualizer.py` & `underactuated-2023.5.29/underactuated/pyplot_visualizer.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/quadrotor2d.py` & `underactuated-2023.5.29/underactuated/quadrotor2d.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/scenarios.py` & `underactuated-2023.5.29/underactuated/scenarios.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated/utils.py` & `underactuated-2023.5.29/underactuated/utils.py`

 * *Files identical despite different names*

### Comparing `underactuated-2023.4.17/underactuated.egg-info/PKG-INFO` & `underactuated-2023.5.29/underactuated.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: underactuated
-Version: 2023.4.17
+Version: 2023.5.29
 Summary: MIT 6.832 - Underactuated Robotics
 Home-page: https://underactuated.csail.mit.edu
 Author: Russ Tedrake
 Author-email: russt@mit.edu
 Project-URL: Bug Tracker, https://github.com/RussTedrake/underactuated/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `underactuated-2023.4.17/underactuated.egg-info/SOURCES.txt` & `underactuated-2023.5.29/underactuated.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 underactuated/exercises/acrobot/test_cartpole_balancing.py
 underactuated/exercises/acrobot/test_cartpoles_urdf.py
 underactuated/exercises/contact/test_compass_gait_limit_cycle.py
 underactuated/exercises/dp/minimum_time_utils.py
 underactuated/exercises/dp/test_lp_dp.py
 underactuated/exercises/dp/test_minimum_time.py
 underactuated/exercises/dp/test_pendulum_cvi.py
+underactuated/exercises/humanoids/footstep_planning_gcs_utils.py
 underactuated/exercises/humanoids/test_footstep_planning.py
+underactuated/exercises/humanoids/test_footstep_planning_gcs.py
 underactuated/exercises/intro/test_drake_systems.py
 underactuated/exercises/lqr/test_drake_diagrams.py
 underactuated/exercises/lyapunov/test_control.py
 underactuated/exercises/lyapunov/test_sos_and_psd.py
 underactuated/exercises/lyapunov/test_van_der_pol.py
 underactuated/exercises/pend/test_hopfield_network.py
 underactuated/exercises/pend/test_vibrating_pendulum.py
```

