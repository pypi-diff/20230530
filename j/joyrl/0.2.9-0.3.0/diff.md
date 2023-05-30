# Comparing `tmp/joyrl-0.2.9.tar.gz` & `tmp/joyrl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joyrl-0.2.9.tar", last modified: Sun May 28 12:14:53 2023, max compression
+gzip compressed data, was "joyrl-0.3.0.tar", last modified: Tue May 30 15:58:24 2023, max compression
```

## Comparing `joyrl-0.2.9.tar` & `joyrl-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.120723 joyrl-0.2.9/
--rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     4412 2023-05-28 12:14:53.121721 joyrl-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     3951 2023-01-01 08:20:49.000000 joyrl-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.079095 joyrl-0.2.9/joyrl/
--rw-rw-rw-   0        0        0      404 2023-05-28 12:14:51.000000 joyrl-0.2.9/joyrl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.098614 joyrl-0.2.9/joyrl/algos/
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.102603 joyrl-0.2.9/joyrl/algos/DQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/algos/DQN/__init__.py
--rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.2.9/joyrl/algos/DQN/config.py
--rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.2.9/joyrl/algos/DQN/data_handler.py
--rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.2.9/joyrl/algos/DQN/policy.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.105595 joyrl-0.2.9/joyrl/algos/DoubleDQN/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/algos/DoubleDQN/__init__.py
--rw-rw-rw-   0        0        0     5273 2023-03-15 14:04:30.000000 joyrl-0.2.9/joyrl/algos/DoubleDQN/agent.py
--rw-rw-rw-   0        0        0      962 2023-03-15 14:04:45.000000 joyrl-0.2.9/joyrl/algos/DoubleDQN/config.py
--rw-rw-rw-   0        0        0     1507 2023-03-15 14:05:03.000000 joyrl-0.2.9/joyrl/algos/DoubleDQN/trainer.py
--rw-rw-rw-   0        0        0      287 2023-05-28 12:12:22.000000 joyrl-0.2.9/joyrl/algos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.106592 joyrl-0.2.9/joyrl/config/
--rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/config/__init__.py
--rw-rw-rw-   0        0        0     1711 2023-05-28 11:04:19.000000 joyrl-0.2.9/joyrl/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.114194 joyrl-0.2.9/joyrl/envs/
--rw-rw-rw-   0        0        0       54 2023-05-28 10:53:02.000000 joyrl-0.2.9/joyrl/envs/__init__.py
--rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/envs/blackjack.py
--rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/envs/cliff_walking.py
--rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/envs/gridworld.py
--rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/envs/gridworld_env.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.115192 joyrl-0.2.9/joyrl/envs/gym/
--rw-rw-rw-   0        0        0      194 2023-05-28 10:49:52.000000 joyrl-0.2.9/joyrl/envs/gym/__init__.py
--rw-rw-rw-   0        0        0      485 2023-05-27 12:55:35.000000 joyrl-0.2.9/joyrl/envs/gym/config.py
--rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/envs/racetrack.py
--rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/envs/register.py
--rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/envs/stochastic_mdp.py
--rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/envs/windy_gridworld.py
--rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.2.9/joyrl/envs/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.118728 joyrl-0.2.9/joyrl/framework/
--rw-rw-rw-   0        0        0      194 2023-05-28 10:49:40.000000 joyrl-0.2.9/joyrl/framework/__init__.py
--rw-rw-rw-   0        0        0     1332 2023-05-27 12:46:42.000000 joyrl-0.2.9/joyrl/framework/dataserver.py
--rw-rw-rw-   0        0        0     2894 2023-05-27 12:46:27.000000 joyrl-0.2.9/joyrl/framework/learners.py
--rw-rw-rw-   0        0        0     5249 2023-05-27 12:48:22.000000 joyrl-0.2.9/joyrl/framework/stats.py
--rw-rw-rw-   0        0        0     5923 2023-05-27 12:44:48.000000 joyrl-0.2.9/joyrl/framework/workers.py
--rw-rw-rw-   0        0        0     7036 2023-05-28 11:09:11.000000 joyrl-0.2.9/joyrl/run.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.120723 joyrl-0.2.9/joyrl/utils/
--rw-rw-rw-   0        0        0        2 2023-05-28 10:53:04.000000 joyrl-0.2.9/joyrl/utils/__init__.py
--rw-rw-rw-   0        0        0    36574 2023-05-27 12:50:57.000000 joyrl-0.2.9/joyrl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 12:14:53.093602 joyrl-0.2.9/joyrl.egg-info/
--rw-rw-rw-   0        0        0     4412 2023-05-28 12:14:53.000000 joyrl-0.2.9/joyrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2023-05-28 12:14:53.000000 joyrl-0.2.9/joyrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 12:14:53.000000 joyrl-0.2.9/joyrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      350 2023-05-28 12:14:53.000000 joyrl-0.2.9/joyrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 12:14:53.000000 joyrl-0.2.9/joyrl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      995 2023-05-28 12:14:53.122717 joyrl-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1820 2023-05-28 10:45:17.000000 joyrl-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.735860 joyrl-0.3.0/
+-rw-rw-rw-   0        0        0     1097 2023-01-01 08:20:49.000000 joyrl-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5074 2023-05-30 15:58:24.735860 joyrl-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4613 2023-05-28 16:47:29.000000 joyrl-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.630217 joyrl-0.3.0/joyrl/
+-rw-rw-rw-   0        0        0      406 2023-05-30 15:58:14.000000 joyrl-0.3.0/joyrl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.659115 joyrl-0.3.0/joyrl/algos/
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.662041 joyrl-0.3.0/joyrl/algos/DQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/algos/DQN/__init__.py
+-rw-rw-rw-   0        0        0     1109 2023-05-27 12:54:10.000000 joyrl-0.3.0/joyrl/algos/DQN/config.py
+-rw-rw-rw-   0        0        0      356 2023-05-27 12:54:42.000000 joyrl-0.3.0/joyrl/algos/DQN/data_handler.py
+-rw-rw-rw-   0        0        0     4101 2023-05-27 12:54:25.000000 joyrl-0.3.0/joyrl/algos/DQN/policy.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.666580 joyrl-0.3.0/joyrl/algos/DoubleDQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/algos/DoubleDQN/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-05-30 15:47:45.000000 joyrl-0.3.0/joyrl/algos/DoubleDQN/config.py
+-rw-rw-rw-   0        0        0      361 2023-05-30 15:50:22.000000 joyrl-0.3.0/joyrl/algos/DoubleDQN/data_handler.py
+-rw-rw-rw-   0        0        0     4197 2023-05-30 15:50:25.000000 joyrl-0.3.0/joyrl/algos/DoubleDQN/policy.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.672438 joyrl-0.3.0/joyrl/algos/DuelingDQN/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/algos/DuelingDQN/__init__.py
+-rw-rw-rw-   0        0        0      912 2023-05-18 10:45:45.000000 joyrl-0.3.0/joyrl/algos/DuelingDQN/config.py
+-rw-rw-rw-   0        0        0      348 2023-05-17 11:24:30.000000 joyrl-0.3.0/joyrl/algos/DuelingDQN/data_handler.py
+-rw-rw-rw-   0        0        0     4010 2023-05-30 15:19:06.000000 joyrl-0.3.0/joyrl/algos/DuelingDQN/policy.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.690189 joyrl-0.3.0/joyrl/algos/NoisyDQN/
+-rw-rw-rw-   0        0        0      194 2023-05-30 15:57:36.000000 joyrl-0.3.0/joyrl/algos/NoisyDQN/__init__.py
+-rw-rw-rw-   0        0        0     1143 2023-05-18 10:45:45.000000 joyrl-0.3.0/joyrl/algos/NoisyDQN/config.py
+-rw-rw-rw-   0        0        0      350 2023-05-18 10:45:45.000000 joyrl-0.3.0/joyrl/algos/NoisyDQN/data_handler.py
+-rw-rw-rw-   0        0        0     4550 2023-05-18 14:55:52.000000 joyrl-0.3.0/joyrl/algos/NoisyDQN/policy.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.707409 joyrl-0.3.0/joyrl/algos/PPO/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/algos/PPO/__init__.py
+-rw-rw-rw-   0        0        0     1788 2023-05-30 15:19:06.000000 joyrl-0.3.0/joyrl/algos/PPO/config.py
+-rw-rw-rw-   0        0        0     1481 2023-05-30 15:19:06.000000 joyrl-0.3.0/joyrl/algos/PPO/data_handler.py
+-rw-rw-rw-   0        0        0    11671 2023-05-30 15:19:06.000000 joyrl-0.3.0/joyrl/algos/PPO/policy.py
+-rw-rw-rw-   0        0        0      368 2023-05-30 15:57:52.000000 joyrl-0.3.0/joyrl/algos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.714794 joyrl-0.3.0/joyrl/algos/base/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/algos/base/__init__.py
+-rw-rw-rw-   0        0        0     3593 2023-05-27 12:53:20.000000 joyrl-0.3.0/joyrl/algos/base/action_layers.py
+-rw-rw-rw-   0        0        0     6561 2023-05-27 12:52:54.000000 joyrl-0.3.0/joyrl/algos/base/base_layers.py
+-rw-rw-rw-   0        0        0    87371 2023-05-28 11:05:40.000000 joyrl-0.3.0/joyrl/algos/base/buffers.py
+-rw-rw-rw-   0        0        0     1824 2023-05-27 12:53:08.000000 joyrl-0.3.0/joyrl/algos/base/data_handlers.py
+-rw-rw-rw-   0        0        0      332 2023-05-27 12:51:28.000000 joyrl-0.3.0/joyrl/algos/base/exps.py
+-rw-rw-rw-   0        0        0     8481 2023-05-27 12:52:01.000000 joyrl-0.3.0/joyrl/algos/base/networks.py
+-rw-rw-rw-   0        0        0     2667 2023-05-27 12:51:49.000000 joyrl-0.3.0/joyrl/algos/base/optims.py
+-rw-rw-rw-   0        0        0     5520 2023-05-27 12:53:43.000000 joyrl-0.3.0/joyrl/algos/base/policies.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.717728 joyrl-0.3.0/joyrl/config/
+-rw-rw-rw-   0        0        0        0 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/config/__init__.py
+-rw-rw-rw-   0        0        0     1711 2023-05-28 11:04:19.000000 joyrl-0.3.0/joyrl/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.726742 joyrl-0.3.0/joyrl/envs/
+-rw-rw-rw-   0        0        0       54 2023-05-28 10:53:02.000000 joyrl-0.3.0/joyrl/envs/__init__.py
+-rw-rw-rw-   0        0        0     4380 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/envs/blackjack.py
+-rw-rw-rw-   0        0        0     2790 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/envs/cliff_walking.py
+-rw-rw-rw-   0        0        0     3996 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/envs/gridworld.py
+-rw-rw-rw-   0        0        0     3584 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/envs/gridworld_env.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.728693 joyrl-0.3.0/joyrl/envs/gym/
+-rw-rw-rw-   0        0        0      194 2023-05-28 10:49:52.000000 joyrl-0.3.0/joyrl/envs/gym/__init__.py
+-rw-rw-rw-   0        0        0      485 2023-05-27 12:55:35.000000 joyrl-0.3.0/joyrl/envs/gym/config.py
+-rw-rw-rw-   0        0        0    10132 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/envs/racetrack.py
+-rw-rw-rw-   0        0        0     1080 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/envs/register.py
+-rw-rw-rw-   0        0        0     1364 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/envs/stochastic_mdp.py
+-rw-rw-rw-   0        0        0     2697 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/envs/windy_gridworld.py
+-rw-rw-rw-   0        0        0     2652 2023-01-01 08:20:49.000000 joyrl-0.3.0/joyrl/envs/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.732597 joyrl-0.3.0/joyrl/framework/
+-rw-rw-rw-   0        0        0      194 2023-05-28 10:49:40.000000 joyrl-0.3.0/joyrl/framework/__init__.py
+-rw-rw-rw-   0        0        0     1332 2023-05-27 12:46:42.000000 joyrl-0.3.0/joyrl/framework/dataserver.py
+-rw-rw-rw-   0        0        0     2894 2023-05-27 12:46:27.000000 joyrl-0.3.0/joyrl/framework/learners.py
+-rw-rw-rw-   0        0        0     5249 2023-05-27 12:48:22.000000 joyrl-0.3.0/joyrl/framework/stats.py
+-rw-rw-rw-   0        0        0     5923 2023-05-27 12:44:48.000000 joyrl-0.3.0/joyrl/framework/workers.py
+-rw-rw-rw-   0        0        0     8675 2023-05-30 15:46:13.000000 joyrl-0.3.0/joyrl/run.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.734622 joyrl-0.3.0/joyrl/utils/
+-rw-rw-rw-   0        0        0        2 2023-05-28 10:53:04.000000 joyrl-0.3.0/joyrl/utils/__init__.py
+-rw-rw-rw-   0        0        0    36574 2023-05-27 12:50:57.000000 joyrl-0.3.0/joyrl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:58:24.652300 joyrl-0.3.0/joyrl.egg-info/
+-rw-rw-rw-   0        0        0     5074 2023-05-30 15:58:24.000000 joyrl-0.3.0/joyrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1673 2023-05-30 15:58:24.000000 joyrl-0.3.0/joyrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 15:58:24.000000 joyrl-0.3.0/joyrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      350 2023-05-30 15:58:24.000000 joyrl-0.3.0/joyrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 15:58:24.000000 joyrl-0.3.0/joyrl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      995 2023-05-30 15:58:24.738788 joyrl-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1820 2023-05-28 10:45:17.000000 joyrl-0.3.0/setup.py
```

### Comparing `joyrl-0.2.9/LICENSE` & `joyrl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/PKG-INFO` & `joyrl-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,34 @@
-Metadata-Version: 2.1
-Name: joyrl
-Version: 0.2.9
-Summary: A Library for Deep Reinforcement Learning
-Home-page: https://github.com/datawhalechina/joyrl
-Author: johnjim0816
-Author-email: johnjim0816@gmail.com
-License: MIT
-Keywords: reinforcement learning platform pytorch
-Platform: any
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: atari
-Provides-Extra: mujoco
-Provides-Extra: pybullet
-License-File: LICENSE
-
 # JoyRL
 
 [![PyPI](https://img.shields.io/pypi/v/joyrl)](https://pypi.org/project/joyrl/)  [![GitHub issues](https://img.shields.io/github/issues/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/issues) [![GitHub stars](https://img.shields.io/github/stars/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/stargazers) [![GitHub forks](https://img.shields.io/github/forks/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/network) [![GitHub license](https://img.shields.io/github/license/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/blob/master/LICENSE)
 
+`JoyRL` is a parallel reinforcement learning library based on PyTorch and Ray. Unlike existing RL libraries, `JoyRL` is helping users to release the burden of implementing algorithms with tough details, unfriendly APIs, and etc. JoyRL is designed for users to train and test RL algorithms with **only hyperparameters configuration**, which is mush easier for beginners to learn and use. Also, JoyRL supports plenties of state-of-art RL algorithms including **RLHF(core of ChatGPT)**(See algorithms below). JoyRL provides a **modularized framework** for users as well to customize their own algorithms and environments. 
+
 ## Install
 
 ```bash
 # you need to install Anaconda first
-conda create -n joyrl python=3.7
+conda create -n joyrl python=3.8
 conda activate joyrl
 pip install -U joyrl
 ```
 
-Torch:
+Torch install:
 
 ```bash
-# CPU
+# CPU only
 conda install pytorch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0 cpuonly -c pytorch
-# GPU
+# GPU 
 conda install pytorch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0 cudatoolkit=11.3 -c pytorch -c conda-forge
-# GPU with mirrors
+# if network error, then GPU with mirrors
 pip install torch==1.10.0+cu113 torchvision==0.11.0+cu113 torchaudio==0.10.0 --extra-index-url https://download.pytorch.org/whl/cu113
 ```
 ## Usage
+
 the following presents a demo to use joyrl, you donot need to care about complicated details of code. All your need is just to set hyper parameters including `GeneralConfig()` and `AlgoConfig()`, which is also shown in [examples](./examples/) folder, and well trained results are shown in the [benchmarks](./benchmarks/) folder as well.
 ```python
 import joyrl
 class GeneralConfig():
     def __init__(self) -> None:
         self.env_name = "CartPole-v1" # name of environment
         self.algo_name = "DQN" # name of algorithm
@@ -85,9 +71,8 @@
 ## Documentation
 
 More tutorials and API documentation are hosted on [https://datawhalechina.github.io/joyrl/](https://datawhalechina.github.io/joyrl/)
 ## Algorithms
 
 |       Name       |                          Reference                           |                    Author                     | Notes |
 | :--------------: | :----------------------------------------------------------: | :-------------------------------------------: | :---: |
-| DQN | [DQN Paper](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf) | [johnjim0816](https://github.com/johnjim0816) |       |
-
+| DQN | [DQN Paper](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf) | [johnjim0816](https://github.com/johnjim0816) |       |
```

### Comparing `joyrl-0.2.9/joyrl/algos/DQN/config.py` & `joyrl-0.3.0/joyrl/algos/DQN/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/algos/DQN/policy.py` & `joyrl-0.3.0/joyrl/algos/DQN/policy.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/algos/DoubleDQN/config.py` & `joyrl-0.3.0/joyrl/algos/DuelingDQN/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from config.config import DefaultConfig
 
 class AlgoConfig(DefaultConfig):
     def __init__(self) -> None:
         # set epsilon_start=epsilon_end can obtain fixed epsilon=epsilon_end
+        self.dueling = True # use dueling network
         self.epsilon_start = 0.95  # epsilon start value
         self.epsilon_end = 0.01  # epsilon end value
         self.epsilon_decay = 500  # epsilon decay rate
         self.gamma = 0.99  # discount factor
         self.lr = 0.0001  # learning rate
         self.buffer_size = 100000  # size of replay buffer
         self.batch_size = 64  # batch size
         self.target_update = 4  # target network update frequency
+        # value network layers config
         self.value_layers = [
-            {'layer_type': 'linear', 'layer_dim': ['n_states', 256],
-             'activation': 'relu'},
-            {'layer_type': 'linear', 'layer_dim': [256, 256],
-             'activation': 'relu'},
-            {'layer_type': 'linear', 'layer_dim': [256, 'n_actions'],
-             'activation': 'none'}]
+            {'layer_type': 'Linear', 'layer_size': [256], 'activation': 'ReLU'},
+            {'layer_type': 'Linear', 'layer_size': [256], 'activation': 'ReLU'},
+        ]
```

### Comparing `joyrl-0.2.9/joyrl/config/config.py` & `joyrl-0.3.0/joyrl/config/config.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/envs/blackjack.py` & `joyrl-0.3.0/joyrl/envs/blackjack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/envs/cliff_walking.py` & `joyrl-0.3.0/joyrl/envs/cliff_walking.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/envs/gridworld.py` & `joyrl-0.3.0/joyrl/envs/gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/envs/gridworld_env.py` & `joyrl-0.3.0/joyrl/envs/gridworld_env.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/envs/racetrack.py` & `joyrl-0.3.0/joyrl/envs/racetrack.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/envs/register.py` & `joyrl-0.3.0/joyrl/envs/register.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/envs/stochastic_mdp.py` & `joyrl-0.3.0/joyrl/envs/stochastic_mdp.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/envs/windy_gridworld.py` & `joyrl-0.3.0/joyrl/envs/windy_gridworld.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/envs/wrappers.py` & `joyrl-0.3.0/joyrl/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/framework/dataserver.py` & `joyrl-0.3.0/joyrl/framework/dataserver.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/framework/learners.py` & `joyrl-0.3.0/joyrl/framework/learners.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/framework/stats.py` & `joyrl-0.3.0/joyrl/framework/stats.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/framework/workers.py` & `joyrl-0.3.0/joyrl/framework/workers.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl/run.py` & `joyrl-0.3.0/joyrl/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,57 @@
 
-import datetime,time
-import importlib
+import argparse
+import datetime, importlib, time, yaml
 import os
 import ray
 import gymnasium as gym
 from pathlib import Path
 import torch.multiprocessing as mp
 from joyrl.config.config import GeneralConfig, MergedConfig
 from joyrl.framework.dataserver import DataServer
 from joyrl.framework.stats import StatsRecorder, RayLogger, SimpleTrajCollector
 from joyrl.framework.workers import Worker, RayTester   
 from joyrl.framework.learners import Learner
 from joyrl.utils.utils import merge_class_attrs, all_seed, save_cfgs
 
 def load_cfgs(**kwargs):
+    ''' load config from config class
+    '''
     general_cfg = kwargs.get('general_cfg',None) # general config
     if general_cfg is None: general_cfg = GeneralConfig() # if not specified, use default config
     algo_cfg = kwargs.get('algo_cfg',None) # algorithm config
     if algo_cfg is None: algo_cfg = importlib.import_module(f"joyrl.algos.{general_cfg.algo_name}.config").AlgoConfig() 
     env_cfg = kwargs.get('env_cfg',None) # environment config
     if env_cfg is None: env_cfg = importlib.import_module(f"joyrl.envs.{general_cfg.env_name}.config").EnvConfig()
     return general_cfg,algo_cfg,env_cfg
+
+def load_yaml_cfg(target_cfg, load_cfg, item):
+    if load_cfg[item] is not None:
+        for k, v in load_cfg[item].items():
+            setattr(target_cfg, k, v)
+    return target_cfg
+
+def process_yaml_cfgs(general_cfg, algo_cfg, env_cfg):
+    parser = argparse.ArgumentParser(description="hyperparameters")
+    parser.add_argument('--yaml', default=None, type=str,
+
+                        help='the path of config file')
+    args = parser.parse_args()
+    # load config from yaml file
+    if args.yaml is not None:
+        with open(args.yaml) as f:
+            load_cfg = yaml.load(f, Loader=yaml.FullLoader)
+            # load general config
+            general_cfg = load_yaml_cfg(general_cfg, load_cfg, 'general_cfg')
+            # load algo config
+            algo_cfg = load_yaml_cfg(algo_cfg, load_cfg, 'algo_cfg')
+            # load env config
+            env_cfg = load_yaml_cfg(env_cfg, load_cfg, 'env_cfg')
+    return general_cfg, algo_cfg, env_cfg
+
 def merge_cfgs(general_cfg, algo_cfg, env_cfg):
     cfg = MergedConfig() # merge config
     cfg.general_cfg = general_cfg
     cfg.algo_cfg = algo_cfg
     cfg.env_cfg = env_cfg
     cfg = merge_class_attrs(cfg, general_cfg)
     cfg = merge_class_attrs(cfg, algo_cfg)
@@ -69,36 +96,48 @@
             if "support" in k: # avoid ndarray
                 v = str(v[0])
             logger.info.remote(tplt.format(k, v, str(type(v))))
         logger.info.remote(''.join(['='] * 80))
     print_cfg(cfg.general_cfg,name = 'General Configs')
     print_cfg(cfg.algo_cfg,name = 'Algo Configs')
     print_cfg(cfg.env_cfg,name = 'Env Configs')
-def check_n_workers(cfg):
-    ''' check n_workers
-    '''
+
+def check_resources(cfg):
+    # check cpu resources
     if cfg.__dict__.get('n_workers',None) is None: # set n_workers to 1 if not set
         setattr(cfg, 'n_workers', 1)
-    if not isinstance(cfg.n_workers,int) or cfg.n_workers <= 0: # n_workers must >0
+    if not isinstance(cfg.n_workers,int) or cfg.n_workers<=0: # n_workers must >0
         raise ValueError("the parameter 'n_workers' must >0!")
     if cfg.n_workers > mp.cpu_count() - 1:
         raise ValueError("the parameter 'n_workers' must less than total numbers of cpus on your machine!")
+    # check gpu resources
+    if cfg.device == "cuda" and cfg.n_learners > 1:
+        raise ValueError("the parameter 'n_learners' must be 1 when using gpu!")
+    if cfg.device == "cuda":
+        n_gpus_tester = 0.05
+        n_gpus_learner = 0.9
+    else:
+        n_gpus_tester = 0
+        n_gpus_learner = 0
+    return n_gpus_tester, n_gpus_learner
+
 def create_single_env(cfg):
     ''' create single env
     '''
     env_cfg = cfg.env_cfg
     env_cfg_dic = env_cfg.__dict__
     kwargs = {k: v for k, v in env_cfg_dic.items() if k not in env_cfg_dic['ignore_params']}
     env = gym.make(**kwargs)
     if env_cfg.wrapper is not None:
         wrapper_class_path = env_cfg.wrapper.split('.')[:-1]
         wrapper_class_name = env_cfg.wrapper.split('.')[-1]
         env_wapper = __import__('.'.join(wrapper_class_path), fromlist=[wrapper_class_name])
         env = getattr(env_wapper, wrapper_class_name)(env)
     return env
+
 def envs_config(cfg,logger):
     ''' configure environment
     '''
     # register_env(env_cfg.id)
     envs = [] # numbers of envs, equal to cfg.n_workers
     for _ in range(cfg.n_workers):
         env = create_single_env(cfg)
@@ -118,30 +157,32 @@
     if cfg.load_checkpoint:
         policy.load_model(f"tasks/{cfg.load_path}/models/{cfg.load_model_step}")
     data_handler = data_handler_mod.DataHandler(cfg)
     return policy, data_handler
 
 def run(**kwargs):
     general_cfg,algo_cfg,env_cfg = load_cfgs(**kwargs)
+    general_cfg,algo_cfg,env_cfg = process_yaml_cfgs(general_cfg,algo_cfg,env_cfg)
     cfg = merge_cfgs(general_cfg, algo_cfg, env_cfg)
     cfg = create_dirs(cfg)
     ray.shutdown()
     ray.init(include_dashboard=True)
     logger = RayLogger.remote(cfg.log_dir) # create ray logger 
     print_cfgs(cfg,logger)
+    n_gpus_tester, n_gpus_learner = check_resources(cfg)
     all_seed(cfg.seed) # set seed
     envs = envs_config(cfg,logger) # configure environment
     test_env = create_single_env(cfg) # create test environment
-    online_tester = RayTester.remote(cfg,test_env) # create online tester
+    online_tester = RayTester.options(num_gpus= n_gpus_tester).remote(cfg,test_env) # create online tester
     policy, data_handler = policy_config(cfg) # create policy and data_handler
     stats_recorder = StatsRecorder.remote(cfg) # create stats recorder
     data_server = DataServer.remote(cfg) # create data server
     learners = []
     for i in range(cfg.n_learners):
-        learner = Learner.remote(cfg, learner_id = i, policy = policy,data_handler = data_handler, online_tester = online_tester)
+        learner = Learner.options(num_gpus= n_gpus_learner / cfg.n_learners).remote(cfg, learner_id = i, policy = policy,data_handler = data_handler, online_tester = online_tester)
         learners.append(learner)
     workers = []
     for i in range(cfg.n_workers):
         worker = Worker.remote(cfg, worker_id = i,env = envs[i], logger = logger)
         worker.set_learner_id.remote(i%cfg.n_learners)
         workers.append(worker)
     s_t = time.time()
```

### Comparing `joyrl-0.2.9/joyrl/utils/utils.py` & `joyrl-0.3.0/joyrl/utils/utils.py`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/joyrl.egg-info/PKG-INFO` & `joyrl-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joyrl
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Library for Deep Reinforcement Learning
 Home-page: https://github.com/datawhalechina/joyrl
 Author: johnjim0816
 Author-email: johnjim0816@gmail.com
 License: MIT
 Keywords: reinforcement learning platform pytorch
 Platform: any
@@ -15,34 +15,37 @@
 Provides-Extra: pybullet
 License-File: LICENSE
 
 # JoyRL
 
 [![PyPI](https://img.shields.io/pypi/v/joyrl)](https://pypi.org/project/joyrl/)  [![GitHub issues](https://img.shields.io/github/issues/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/issues) [![GitHub stars](https://img.shields.io/github/stars/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/stargazers) [![GitHub forks](https://img.shields.io/github/forks/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/network) [![GitHub license](https://img.shields.io/github/license/datawhalechina/joyrl)](https://github.com/datawhalechina/joyrl/blob/master/LICENSE)
 
+`JoyRL` is a parallel reinforcement learning library based on PyTorch and Ray. Unlike existing RL libraries, `JoyRL` is helping users to release the burden of implementing algorithms with tough details, unfriendly APIs, and etc. JoyRL is designed for users to train and test RL algorithms with **only hyperparameters configuration**, which is mush easier for beginners to learn and use. Also, JoyRL supports plenties of state-of-art RL algorithms including **RLHF(core of ChatGPT)**(See algorithms below). JoyRL provides a **modularized framework** for users as well to customize their own algorithms and environments. 
+
 ## Install
 
 ```bash
 # you need to install Anaconda first
-conda create -n joyrl python=3.7
+conda create -n joyrl python=3.8
 conda activate joyrl
 pip install -U joyrl
 ```
 
-Torch:
+Torch install:
 
 ```bash
-# CPU
+# CPU only
 conda install pytorch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0 cpuonly -c pytorch
-# GPU
+# GPU 
 conda install pytorch==1.10.0 torchvision==0.11.0 torchaudio==0.10.0 cudatoolkit=11.3 -c pytorch -c conda-forge
-# GPU with mirrors
+# if network error, then GPU with mirrors
 pip install torch==1.10.0+cu113 torchvision==0.11.0+cu113 torchaudio==0.10.0 --extra-index-url https://download.pytorch.org/whl/cu113
 ```
 ## Usage
+
 the following presents a demo to use joyrl, you donot need to care about complicated details of code. All your need is just to set hyper parameters including `GeneralConfig()` and `AlgoConfig()`, which is also shown in [examples](./examples/) folder, and well trained results are shown in the [benchmarks](./benchmarks/) folder as well.
 ```python
 import joyrl
 class GeneralConfig():
     def __init__(self) -> None:
         self.env_name = "CartPole-v1" # name of environment
         self.algo_name = "DQN" # name of algorithm
```

### Comparing `joyrl-0.2.9/setup.cfg` & `joyrl-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `joyrl-0.2.9/setup.py` & `joyrl-0.3.0/setup.py`

 * *Files identical despite different names*

