# Comparing `tmp/modular_rl-0.2.2.tar.gz` & `tmp/modular_rl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.2.2.tar", last modified: Fri May 12 13:15:17 2023, max compression
+gzip compressed data, was "modular_rl-0.2.3.tar", last modified: Tue May 30 13:36:16 2023, max compression
```

## Comparing `modular_rl-0.2.2.tar` & `modular_rl-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 13:15:17.493587 modular_rl-0.2.2/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      781 2023-05-12 13:15:17.492585 modular_rl-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3963 2023-05-12 13:14:22.000000 modular_rl-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 13:15:17.412614 modular_rl-0.2.2/modular_rl/
--rw-rw-rw-   0        0        0       36 2023-05-07 02:39:54.000000 modular_rl-0.2.2/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:15:17.460581 modular_rl-0.2.2/modular_rl/agents/
--rw-rw-rw-   0        0        0       54 2023-05-07 02:39:10.000000 modular_rl-0.2.2/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0     8892 2023-05-07 06:52:16.000000 modular_rl-0.2.2/modular_rl/agents/_agent.py
--rw-rw-rw-   0        0        0    11655 2023-05-07 07:04:46.000000 modular_rl-0.2.2/modular_rl/agents/mcts.py
--rw-rw-rw-   0        0        0    15806 2023-05-12 13:09:46.000000 modular_rl-0.2.2/modular_rl/agents/ppo.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:15:17.469581 modular_rl-0.2.2/modular_rl/networks/
--rw-rw-rw-   0        0        0       66 2023-05-07 02:38:25.000000 modular_rl-0.2.2/modular_rl/networks/__init__.py
--rw-rw-rw-   0        0        0     2121 2023-05-07 06:40:47.000000 modular_rl-0.2.2/modular_rl/networks/actor_critic.py
--rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.2.2/modular_rl/networks/policy.py
--rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.2.2/modular_rl/networks/value.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:15:17.475581 modular_rl-0.2.2/modular_rl/params/
--rw-rw-rw-   0        0        0       54 2023-05-07 02:39:30.000000 modular_rl-0.2.2/modular_rl/params/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-05-07 06:43:45.000000 modular_rl-0.2.2/modular_rl/params/mcts.py
--rw-rw-rw-   0        0        0     2015 2023-05-07 06:44:07.000000 modular_rl-0.2.2/modular_rl/params/ppo.py
--rw-rw-rw-   0        0        0     1113 2023-05-07 06:45:58.000000 modular_rl-0.2.2/modular_rl/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:15:17.481583 modular_rl-0.2.2/modular_rl/tester/
--rw-rw-rw-   0        0        0       59 2023-05-07 06:49:12.000000 modular_rl-0.2.2/modular_rl/tester/__init__.py
--rw-rw-rw-   0        0        0      353 2023-05-07 06:48:36.000000 modular_rl-0.2.2/modular_rl/tester/mcts.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.2.2/modular_rl/tester/ppo.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:15:17.484585 modular_rl-0.2.2/modular_rl/util/
--rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.2.2/modular_rl/util/__init__.py
--rw-rw-rw-   0        0        0     2371 2023-05-05 09:56:27.000000 modular_rl-0.2.2/modular_rl/util/node.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:15:17.451579 modular_rl-0.2.2/modular_rl.egg-info/
--rw-rw-rw-   0        0        0      781 2023-05-12 13:15:16.000000 modular_rl-0.2.2/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      769 2023-05-12 13:15:16.000000 modular_rl-0.2.2/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 13:15:16.000000 modular_rl-0.2.2/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-12 13:15:16.000000 modular_rl-0.2.2/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-12 13:15:16.000000 modular_rl-0.2.2/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1414 2023-05-12 13:13:36.000000 modular_rl-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 13:15:17.494587 modular_rl-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-05-12 13:13:28.000000 modular_rl-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 13:15:17.490584 modular_rl-0.2.2/tests/
--rw-rw-rw-   0        0        0       93 2023-05-07 06:51:17.000000 modular_rl-0.2.2/tests/test_mcts.py
--rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.2.2/tests/test_ppo.py
--rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.2.2/tests/test_ppo_modular.py
+drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.599220 modular_rl-0.2.3/
+-rw-r--r--   0 sjm        (501) staff       (20)     1068 2023-05-13 00:53:55.000000 modular_rl-0.2.3/LICENSE
+-rw-r--r--   0 sjm        (501) staff       (20)     5305 2023-05-30 13:36:16.598637 modular_rl-0.2.3/PKG-INFO
+-rw-r--r--   0 sjm        (501) staff       (20)     3963 2023-05-13 00:53:55.000000 modular_rl-0.2.3/README.md
+drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.542870 modular_rl-0.2.3/modular_rl/
+-rw-r--r--   0 sjm        (501) staff       (20)       36 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/__init__.py
+drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.561426 modular_rl-0.2.3/modular_rl/agents/
+-rw-r--r--   0 sjm        (501) staff       (20)       82 2023-05-29 21:48:43.000000 modular_rl-0.2.3/modular_rl/agents/__init__.py
+-rw-r--r--   0 sjm        (501) staff       (20)     9785 2023-05-30 12:42:39.000000 modular_rl-0.2.3/modular_rl/agents/_agent.py
+-rw-r--r--   0 sjm        (501) staff       (20)    11169 2023-05-30 13:01:06.000000 modular_rl-0.2.3/modular_rl/agents/mcis.py
+-rw-r--r--   0 sjm        (501) staff       (20)    11655 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/agents/mcts.py
+-rw-r--r--   0 sjm        (501) staff       (20)    15091 2023-05-30 12:43:22.000000 modular_rl-0.2.3/modular_rl/agents/ppo.py
+drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.568544 modular_rl-0.2.3/modular_rl/networks/
+-rw-r--r--   0 sjm        (501) staff       (20)       66 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/networks/__init__.py
+-rw-r--r--   0 sjm        (501) staff       (20)     2121 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/networks/actor_critic.py
+-rw-r--r--   0 sjm        (501) staff       (20)     2802 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/networks/policy.py
+-rw-r--r--   0 sjm        (501) staff       (20)     2616 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/networks/value.py
+drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.576163 modular_rl-0.2.3/modular_rl/params/
+-rw-r--r--   0 sjm        (501) staff       (20)       82 2023-05-29 21:49:11.000000 modular_rl-0.2.3/modular_rl/params/__init__.py
+-rw-r--r--   0 sjm        (501) staff       (20)     2124 2023-05-29 12:03:11.000000 modular_rl-0.2.3/modular_rl/params/mcis.py
+-rw-r--r--   0 sjm        (501) staff       (20)     2305 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/params/mcts.py
+-rw-r--r--   0 sjm        (501) staff       (20)     2015 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/params/ppo.py
+-rw-r--r--   0 sjm        (501) staff       (20)     1248 2023-05-29 21:50:50.000000 modular_rl-0.2.3/modular_rl/settings.py
+drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.583572 modular_rl-0.2.3/modular_rl/tester/
+-rw-r--r--   0 sjm        (501) staff       (20)       59 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/tester/__init__.py
+-rw-r--r--   0 sjm        (501) staff       (20)      945 2023-05-30 12:20:33.000000 modular_rl-0.2.3/modular_rl/tester/mcis.py
+-rw-r--r--   0 sjm        (501) staff       (20)      353 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/tester/mcts.py
+-rw-r--r--   0 sjm        (501) staff       (20)     1505 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/tester/ppo.py
+drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.587074 modular_rl-0.2.3/modular_rl/util/
+-rw-r--r--   0 sjm        (501) staff       (20)        0 2023-05-13 00:53:55.000000 modular_rl-0.2.3/modular_rl/util/__init__.py
+-rw-r--r--   0 sjm        (501) staff       (20)     2468 2023-05-30 11:09:00.000000 modular_rl-0.2.3/modular_rl/util/node.py
+drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.549749 modular_rl-0.2.3/modular_rl.egg-info/
+-rw-r--r--   0 sjm        (501) staff       (20)     5305 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/PKG-INFO
+-rw-r--r--   0 sjm        (501) staff       (20)      893 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 sjm        (501) staff       (20)        1 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 sjm        (501) staff       (20)       26 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/requires.txt
+-rw-r--r--   0 sjm        (501) staff       (20)       11 2023-05-30 13:36:16.000000 modular_rl-0.2.3/modular_rl.egg-info/top_level.txt
+-rw-r--r--   0 sjm        (501) staff       (20)     1414 2023-05-29 21:51:26.000000 modular_rl-0.2.3/pyproject.toml
+-rw-r--r--   0 sjm        (501) staff       (20)       38 2023-05-30 13:36:16.599360 modular_rl-0.2.3/setup.cfg
+-rw-r--r--   0 sjm        (501) staff       (20)      937 2023-05-29 21:51:36.000000 modular_rl-0.2.3/setup.py
+drwxr-xr-x   0 sjm        (501) staff       (20)        0 2023-05-30 13:36:16.594842 modular_rl-0.2.3/tests/
+-rw-r--r--   0 sjm        (501) staff       (20)       93 2023-05-29 21:52:50.000000 modular_rl-0.2.3/tests/test_mcis.py
+-rw-r--r--   0 sjm        (501) staff       (20)      101 2023-05-30 12:23:04.000000 modular_rl-0.2.3/tests/test_mcis_modular.py
+-rw-r--r--   0 sjm        (501) staff       (20)       93 2023-05-13 00:53:55.000000 modular_rl-0.2.3/tests/test_mcts.py
+-rw-r--r--   0 sjm        (501) staff       (20)       58 2023-05-13 00:53:55.000000 modular_rl-0.2.3/tests/test_ppo.py
+-rw-r--r--   0 sjm        (501) staff       (20)       66 2023-05-13 00:53:55.000000 modular_rl-0.2.3/tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.2.2/LICENSE` & `modular_rl-0.2.3/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 horrible-gh
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 horrible-gh
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `modular_rl-0.2.2/README.md` & `modular_rl-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.2/modular_rl/agents/_agent.py` & `modular_rl-0.2.3/modular_rl/agents/_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,28 +64,41 @@
         self.avg_reward = 0
 
         # Set learn parameters (If necessary)
         self.state = None
         self.action = None
         self.reward = None
         self.done = None
+        self.reset()
 
         # Logger initialize
         self.log_level = setting.get('log_level', 'debug')
         self.log_init_pass = setting.get('log_init_pass', False)
         if self.log_init_pass == False:
             Logger.init(
                 dir_name=None,
                 file_name=None,
                 log_level=self.log_level,
                 out_console=True,
                 out_file=None,
                 prev_log_remove=None
             )
 
+    def reset(self):
+        """
+        Reset the lists that contain information about the states, actions, rewards, and other values for the agent.
+        """
+
+        self.states = []
+        self.actions = []
+        self.rewards = []
+        self.next_states = []
+        self.dones = []
+        self.log_probs = []
+
     def init_policy_value(self):
         """
         Initializes policy and value networks, and their respective optimizers.
         """
 
         # Create neural network instances and optimizer
         self.policy_net = PolicyNetwork(
@@ -117,14 +130,15 @@
         '''
 
         state_num = len(state)
         if state_num == 2:
             state, _ = state  # Unpack the tuple
         return state
 
+
     def learn_reset(self):
         """
         Reset the agent's state and episode reward.
         """
 
         self.state = self.env.reset()
         return self._check_state(self.state)
@@ -222,7 +236,24 @@
         """
 
         checkpoint = torch.load(file_name)
         self.actor_critic_net.load_state_dict(
             checkpoint['actor_critic_net_state_dict'])
         self.actor_critic_optimizer.load_state_dict(
             checkpoint['optimizer_state_dict'])
+
+    def step_unpack(self, step_output):
+        step_output_num = len(step_output)
+        if step_output_num == 4:
+            next_state, reward, is_done, _ = step_output
+        elif step_output_num == 5:
+            next_state, reward, is_done, _, _ = step_output
+        return next_state, reward, is_done
+
+    def update_reward(self, reward) :
+        self.episode_reward += reward
+        self.total_reward += reward
+        self.prev_reward = reward
+
+    def update_episode(self):
+        self.episode += 1
+        self.episode_reward = 0
```

### Comparing `modular_rl-0.2.2/modular_rl/agents/mcts.py` & `modular_rl-0.2.3/modular_rl/agents/mcts.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.2/modular_rl/agents/ppo.py` & `modular_rl-0.2.3/modular_rl/agents/ppo.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         # Set learn modular parameters
         self.state = None
         self.dist = None
 
     # Implement PPO algorithm
 
-    def compute_advantages(self, rewards, values, done, gamma=0.99, lam=0.95):
+    def compute_advantages(self, rewards, values, dones, gamma=0.99, lam=0.95):
         """
         Compute advantages given the rewards, values, done flags, and discount factors.
 
         :param rewards: The rewards obtained from the environment.
         :type rewards: numpy.ndarray
         :param values: The predicted state-value from the critic network.
         :type values: numpy.ndarray
@@ -72,17 +72,17 @@
         :rtype: numpy.ndarray
         """
 
         advantages = np.zeros_like(rewards)
         last_advantage = 0
         for t in reversed(range(len(rewards))):
             delta = rewards[t] + gamma * \
-                values[t + 1] * (1 - done[t]) - values[t]
+                values[t + 1] * (1 - dones[t]) - values[t]
             advantages[t] = delta + gamma * lam * \
-                last_advantage * (1 - done[t])
+                last_advantage * (1 - dones[t])
             last_advantage = advantages[t]
         return advantages
 
     def ppo_iter(self, mini_batch_size, states, actions, log_probs, returns, advantages):
         """
         Generate random mini-batches of data for PPO algorithm.
 
@@ -204,36 +204,29 @@
         """
 
         if dist == None and self.dist:
             dist = self.dist
 
         if auto_step:
             step_output = self.env.step(action.item())
-            step_output_num = len(step_output)
-
-            if step_output_num == 4:
-                next_state, reward, is_done, _ = step_output
-            elif step_output_num == 5:
-                next_state, reward, is_done, _, _ = step_output
+            next_state, reward, is_done = self.step_unpack(step_output)
 
         else:
             if next_state is None:
                 next_state = state
 
-        self.episode_reward += reward
-        self.total_reward += reward
-        self.prev_reward = reward
+        self.update_reward(reward)
 
         state = self._check_state(state)
 
         self.states.append(state)
         self.actions.append(action)
         self.rewards.append(reward)
         self.next_states.append(next_state)
-        self.done.append(is_done)
+        self.dones.append(is_done)
         self.log_probs.append(dist.log_prob(action))
 
         self.state = next_state
 
         if timestep > 0:
             timestep += 1
 
@@ -244,21 +237,21 @@
 
     def update(self):
         """
         Perform an update of the PPO algorithm, using the stored information about the environment from the previous learning iterations.
         """
 
         Logger.verb('agents:ppo:update',
-                    f'states={self.states}, next_states={self.next_states}, actions={self.actions}, rewards={self.rewards}, done={self.done}')
+                    f'states={self.states}, next_states={self.next_states}, actions={self.actions}, rewards={self.rewards}, dones={self.dones}')
         states_tensor = torch.tensor(np.array(self.states, dtype=np.float32))
         actions_tensor = torch.tensor(np.array(self.actions))
         rewards_tensor = torch.tensor(np.array(self.rewards, dtype=np.float32))
         next_states_tensor = torch.tensor(
             np.array(self.next_states, dtype=np.float32))
-        done_tensor = torch.tensor(np.array(self.done, dtype=np.float32))
+        done_tensor = torch.tensor(np.array(self.dones, dtype=np.float32))
         log_probs_tensor = torch.stack(self.log_probs)
 
         values = self.value_net(states_tensor).detach().squeeze(1)
         next_values = self.value_net(next_states_tensor).detach().squeeze(1)
 
         if len(next_states_tensor) > 0:
             last_value = next_values[-1].item()
@@ -276,17 +269,15 @@
         else:
             returns = np.add(advantages, values)
 
         self.ppo_update(self.ppo_epochs, self.mini_batch_size, states_tensor,
                         actions_tensor, log_probs_tensor, returns, advantages_tensor)
 
         self.reset()
-
-        self.episode += 1
-        self.episode_reward = 0
+        self.update_episode()
 
     def train(self):
         """
         Execute the learning loop, where the PPO algorithm is used to train the agent on the specified environment.
         """
         self.learn()
 
@@ -327,44 +318,26 @@
                 if self.episode + 1 >= self.max_episodes:
                     break
 
             self.env.close()
         else:
             self.reset()
 
-    def reset(self):
-        """
-        Reset the lists that contain information about the states, actions, rewards, and other values for the agent.
-        """
-
-        self.states = []
-        self.actions = []
-        self.rewards = []
-        self.next_states = []
-        self.done = []
-        self.log_probs = []
-
-    def learn_reset(self):
-        """
-        Reset the agent's state and episode reward.
-        """
-
-        return super().learn_reset()
 
     def learn_next(self):
         """
         Perform a single learning step and update the episode and total rewards.
 
         :return: The action taken, the resulting reward, and whether the episode is done or not.
         :rtype: tuple(torch.Tensor, float, bool)
         """
 
-        action, reward, is_done = self.learn_step(self.state, -1)
+        action, reward, is_done, timestep = self.learn_step(self.state, -1)
 
-        return action, reward, is_done
+        return action, reward, is_done, timestep
 
     def learn_close(self):
         """
         Close the environment and reset the agent's total reward, episode count, and episode reward.
         """
 
         super().learn_close()
```

### Comparing `modular_rl-0.2.2/modular_rl/networks/actor_critic.py` & `modular_rl-0.2.3/modular_rl/networks/actor_critic.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.2/modular_rl/networks/policy.py` & `modular_rl-0.2.3/modular_rl/networks/policy.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible
-
-PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
-The purpose of this network is to determine the best action to take in the current state.
-
-ValueNetwork, on the other hand, 
-is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
-The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
-
-Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
-which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
-
-This software includes the following third-party libraries:
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-
-"""
-import torch.nn as nn
-import torch
-
-
-class PolicyNetwork(nn.Module):
-    def __init__(self, input_dim, output_dim, hidden_option='medium', num_layers=2):
-        """
-        Initialize the PolicyNetwork class with the specified input dimension, output dimension, and network settings.
-
-        :param input_dim: The dimension of the input layer.
-        :type input_dim: int
-        :param output_dim: The dimension of the output layer.
-        :type output_dim: int
-        :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
-        :type hidden_option: str
-        :param num_layers: The number of hidden layers.
-        :type num_layers: int
-        """
-
-        super(PolicyNetwork, self).__init__()
-
-        hidden_dim_map = {
-            'small': 32,
-            'medium': 64,
-            'large': 128,
-            'huge': 256,
-            'exhuge': 512
-        }
-
-        hidden_dim = hidden_dim_map[hidden_option]
-
-        # Create each layer
-        layers = []
-        for i in range(num_layers):
-            if i == 0:
-                layers.append(nn.Linear(input_dim, hidden_dim))
-            elif i == num_layers - 1:
-                layers.append(nn.Linear(hidden_dim, output_dim))
-            else:
-                layers.append(nn.Linear(hidden_dim * i, hidden_dim * (i + 1)))
-            layers.append(nn.ReLU())
-        self.net = nn.Sequential(*layers)
-
-    def forward(self, x):
-        """
-        Compute a forward pass of the policy network.
-
-        :param x: The input tensor.
-        :type x: torch.Tensor
-        :return: The output tensor.
-        :rtype: torch.Tensor
-        """
-
-        x = self.net(x)
-        x = torch.softmax(x, dim=-1)
-        return x
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible
+
+PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
+The purpose of this network is to determine the best action to take in the current state.
+
+ValueNetwork, on the other hand, 
+is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
+The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
+
+Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
+which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
+
+This software includes the following third-party libraries:
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+
+"""
+import torch.nn as nn
+import torch
+
+
+class PolicyNetwork(nn.Module):
+    def __init__(self, input_dim, output_dim, hidden_option='medium', num_layers=2):
+        """
+        Initialize the PolicyNetwork class with the specified input dimension, output dimension, and network settings.
+
+        :param input_dim: The dimension of the input layer.
+        :type input_dim: int
+        :param output_dim: The dimension of the output layer.
+        :type output_dim: int
+        :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
+        :type hidden_option: str
+        :param num_layers: The number of hidden layers.
+        :type num_layers: int
+        """
+
+        super(PolicyNetwork, self).__init__()
+
+        hidden_dim_map = {
+            'small': 32,
+            'medium': 64,
+            'large': 128,
+            'huge': 256,
+            'exhuge': 512
+        }
+
+        hidden_dim = hidden_dim_map[hidden_option]
+
+        # Create each layer
+        layers = []
+        for i in range(num_layers):
+            if i == 0:
+                layers.append(nn.Linear(input_dim, hidden_dim))
+            elif i == num_layers - 1:
+                layers.append(nn.Linear(hidden_dim, output_dim))
+            else:
+                layers.append(nn.Linear(hidden_dim * i, hidden_dim * (i + 1)))
+            layers.append(nn.ReLU())
+        self.net = nn.Sequential(*layers)
+
+    def forward(self, x):
+        """
+        Compute a forward pass of the policy network.
+
+        :param x: The input tensor.
+        :type x: torch.Tensor
+        :return: The output tensor.
+        :rtype: torch.Tensor
+        """
+
+        x = self.net(x)
+        x = torch.softmax(x, dim=-1)
+        return x
```

### Comparing `modular_rl-0.2.2/modular_rl/networks/value.py` & `modular_rl-0.2.3/modular_rl/networks/value.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible
-
-PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
-The purpose of this network is to determine the best action to take in the current state.
-
-ValueNetwork, on the other hand, 
-is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
-The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
-
-Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
-which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
-
-This software includes the following third-party libraries:
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-
-"""
-import torch.nn as nn
-
-
-class ValueNetwork(nn.Module):
-    def __init__(self, input_dim, hidden_option='medium', num_layers=2):
-        """
-        Initialize the ValueNetwork class with the specified input dimension and network settings.
-
-        :param input_dim: The dimension of the input layer.
-        :type input_dim: int
-        :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
-        :type hidden_option: str
-        :param num_layers: The number of hidden layers.
-        :type num_layers: int
-        """
-
-        super(ValueNetwork, self).__init__()
-
-        hidden_dim_map = {
-            'small': 32,
-            'medium': 64,
-            'large': 128,
-            'huge': 256,
-            'exhuge': 512
-        }
-
-        hidden_dim = hidden_dim_map[hidden_option]
-
-        # Create each layer
-        layers = []
-        for i in range(num_layers):
-            if i == 0:
-                layers.append(nn.Linear(input_dim, hidden_dim))
-            elif i == num_layers - 1:
-                layers.append(nn.Linear(hidden_dim, 1))
-            else:
-                layers.append(nn.Linear(hidden_dim * i, hidden_dim * (i + 1)))
-            layers.append(nn.ReLU())
-        self.net = nn.Sequential(*layers)
-
-    def forward(self, x):
-        """
-        Compute a forward pass of the value network.
-
-        :param x: The input tensor.
-        :type x: torch.Tensor
-        :return: The output tensor.
-        :rtype: torch.Tensor
-        """
-
-        x = self.net(x)
-        return x
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible
+
+PolicyNetwork is a neural network that takes in the current state of the environment as input and outputs a probability distribution over the available actions. 
+The purpose of this network is to determine the best action to take in the current state.
+
+ValueNetwork, on the other hand, 
+is a neural network that takes in the current state of the environment as input and outputs a value that represents the expected future reward that can be obtained from that state. 
+The purpose of this network is to estimate the value of a given state so that the agent can make decisions that lead to the most reward in the long term.
+
+Both networks are important components of the Proximal Policy Optimization (PPO) algorithm, 
+which is a type of reinforcement learning algorithm used for training agents to perform tasks in an environment.
+
+This software includes the following third-party libraries:
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+
+"""
+import torch.nn as nn
+
+
+class ValueNetwork(nn.Module):
+    def __init__(self, input_dim, hidden_option='medium', num_layers=2):
+        """
+        Initialize the ValueNetwork class with the specified input dimension and network settings.
+
+        :param input_dim: The dimension of the input layer.
+        :type input_dim: int
+        :param hidden_option: The size of the hidden layers (options are 'small', 'medium', 'large', 'huge', or 'exhuge').
+        :type hidden_option: str
+        :param num_layers: The number of hidden layers.
+        :type num_layers: int
+        """
+
+        super(ValueNetwork, self).__init__()
+
+        hidden_dim_map = {
+            'small': 32,
+            'medium': 64,
+            'large': 128,
+            'huge': 256,
+            'exhuge': 512
+        }
+
+        hidden_dim = hidden_dim_map[hidden_option]
+
+        # Create each layer
+        layers = []
+        for i in range(num_layers):
+            if i == 0:
+                layers.append(nn.Linear(input_dim, hidden_dim))
+            elif i == num_layers - 1:
+                layers.append(nn.Linear(hidden_dim, 1))
+            else:
+                layers.append(nn.Linear(hidden_dim * i, hidden_dim * (i + 1)))
+            layers.append(nn.ReLU())
+        self.net = nn.Sequential(*layers)
+
+    def forward(self, x):
+        """
+        Compute a forward pass of the value network.
+
+        :param x: The input tensor.
+        :type x: torch.Tensor
+        :return: The output tensor.
+        :rtype: torch.Tensor
+        """
+
+        x = self.net(x)
+        return x
```

### Comparing `modular_rl-0.2.2/modular_rl/params/mcts.py` & `modular_rl-0.2.3/modular_rl/params/mcts.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.2/modular_rl/params/ppo.py` & `modular_rl-0.2.3/modular_rl/params/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.2/modular_rl/settings.py` & `modular_rl-0.2.3/modular_rl/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 with more flexibility for specific use cases. These default values can be modified by passing in a dictionary of
 key-value pairs to the AgentSettings constructor.
 
 '''
 
 from modular_rl.params.ppo import ParamPPO
 from modular_rl.params.mcts import ParamMCTS
+from modular_rl.params.mcis import ParamMCIS
 
 
 class AgentSettings:
     default_ppo = ParamPPO.default
     default_ppo_modular = ParamPPO.default_modular
     default_mcts = ParamMCTS.default
     default_mcts_modular = ParamMCTS.default_modular
+    default_mcis = ParamMCIS.default
+    default_mcis_modular = ParamMCIS.default_modular
```

### Comparing `modular_rl-0.2.2/modular_rl/tester/ppo.py` & `modular_rl-0.2.3/modular_rl/tester/ppo.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# -*- coding: utf-8 -*-
-from modular_rl.agents.ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-'''
-This code is a Python script that initializes and trains an instance of the AgentPPO class with default settings using the init_ppo() function. 
-Additionally, the init_ppo_modular() function is provided to demonstrate the usage of the AgentPPO class with modified settings.
-
-In init_ppo_modular(), an instance of AgentPPO is created with a modified default_modular settings dictionary. 
-The function then calls various methods of the instance, such as reset(), learn_reset(), learn_next(), and update() to demonstrate the functionality of the class. 
-The instance is then saved to a file using the save_model() method, which is not shown in the provided code.
-
-'''
-
-
-def init_ppo():
-    env = AgentPPO(env=None, setting=AgentSettings.default_ppo)
-    env.learn()
-
-
-def init_ppo_modular():
-    env = AgentPPO(env=None, setting=AgentSettings.default_ppo_modular)
-    env.reset()
-    env.learn_reset()
-    env.learn_next()
-    env.learn_check()
-    env.learn_next()
-    env.learn_check()
-    env.update()
-
-    env.reset()
-    ppo_manual_step(env)
-    env.learn_check()
-    ppo_manual_step(env)
-    env.learn_check()
-    env.update()
-
-    env.learn_close()
-
-    # env.save_model('test.pth')
-
-
-def ppo_manual_step(env):
-    initial_state = env.learn_reset()
-    action, _ = env.select_action(initial_state)
-    next_state = env.learn_reset()
-    env.update_step(next_state, None, action, -1)
+# -*- coding: utf-8 -*-
+from modular_rl.agents.ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+'''
+This code is a Python script that initializes and trains an instance of the AgentPPO class with default settings using the init_ppo() function. 
+Additionally, the init_ppo_modular() function is provided to demonstrate the usage of the AgentPPO class with modified settings.
+
+In init_ppo_modular(), an instance of AgentPPO is created with a modified default_modular settings dictionary. 
+The function then calls various methods of the instance, such as reset(), learn_reset(), learn_next(), and update() to demonstrate the functionality of the class. 
+The instance is then saved to a file using the save_model() method, which is not shown in the provided code.
+
+'''
+
+
+def init_ppo():
+    env = AgentPPO(env=None, setting=AgentSettings.default_ppo)
+    env.learn()
+
+
+def init_ppo_modular():
+    env = AgentPPO(env=None, setting=AgentSettings.default_ppo_modular)
+    env.reset()
+    env.learn_reset()
+    env.learn_next()
+    env.learn_check()
+    env.learn_next()
+    env.learn_check()
+    env.update()
+
+    env.reset()
+    ppo_manual_step(env)
+    env.learn_check()
+    ppo_manual_step(env)
+    env.learn_check()
+    env.update()
+
+    env.learn_close()
+
+    # env.save_model('test.pth')
+
+
+def ppo_manual_step(env):
+    initial_state = env.learn_reset()
+    action, _ = env.select_action(initial_state)
+    next_state = env.learn_reset()
+    env.update_step(next_state, None, action, -1)
```

### Comparing `modular_rl-0.2.2/modular_rl/util/node.py` & `modular_rl-0.2.3/modular_rl/util/node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,65 @@
-import math
-from LogAssist.log import Logger
-import numpy as np
-
-
-class Node:
-    def __init__(self, state, prior, action=None):
-        self.state = state
-        self.prior = prior
-        self.action = action  # 액션 정보를 저장하는 속성 추가
-        self.visit_count = 0
-        self.value_sum = 0
-        self.children = {}
-        self.total_value = 0
-
-    def __repr__(self):
-        return f'Node(state={self.state}, total_value={self.total_value}, visit_count={self.visit_count}, is_expanded={self.expanded()}, action_probs={self.action}, children={self.children})'
-
-    def expanded(self):
-        return len(self.children) > 0
-
-    def value(self):
-        if self.visit_count == 0:
-            return 0
-        return self.total_value / self.visit_count  # 총 보상을 방문 횟수로 나누어 평균 보상을 반환
-
-    def select_child(self, cpuct):
-        best_score = -math.inf
-        best_action = -1
-        best_child = None
-
-        for action, child in self.children.items():
-            uct_score = child.value() + cpuct * child.prior * math.sqrt(self.visit_count) / \
-                (1 + child.visit_count)
-            if uct_score > best_score:
-                best_score = uct_score
-                best_action = action
-                best_child = child
-
-        return best_action, best_child
-
-    def expand(self, action_space, child_priors):
-        for action, prior in zip(range(action_space), child_priors):
-            if action not in self.children:
-                self.children[action] = Node(self.state, prior, action)
-
-    def update_stats(self, reward):
-        self.total_value += reward  # 총 보상 업데이트
-        self.visit_count += 1  # 방문 횟수 증가
-
-    def select_action(self, temperature=1):
-        visit_counts = np.array(
-            [child.visit_count for child in self.children.values()])
-        actions = [action for action in self.children.keys()]
-        if temperature == 0:
-            action = actions[np.argmax(visit_counts)]
-        else:
-            visit_counts = visit_counts ** (1/temperature)  # apply temperature
-            # normalize to get probabilities
-            visit_counts = visit_counts / sum(visit_counts)
-            action = np.random.choice(actions, p=visit_counts)
-
-        return action
+import math
+from LogAssist.log import Logger
+import numpy as np
+
+
+class Node:
+    def __init__(self, state, prior, action=None, done=False):
+        self.state = state
+        self.prior = prior
+        self.action = action  # 액션 정보를 저장하는 속성 추가
+        self.visit_count = 0
+        self.value_sum = 0
+        self.children = {}
+        self.total_value = 0
+        self.done = done  # Assign the done attribute
+
+
+    def __repr__(self):
+        return f'Node(state={self.state}, total_value={self.total_value}, visit_count={self.visit_count}, is_expanded={self.expanded()}, action_probs={self.action}, children={self.children})'
+
+    def expanded(self):
+        return len(self.children) > 0
+
+    def value(self):
+        if self.visit_count == 0:
+            return 0
+        return self.total_value / self.visit_count  # 총 보상을 방문 횟수로 나누어 평균 보상을 반환
+
+    def select_child(self, cpuct):
+        best_score = -math.inf
+        best_action = -1
+        best_child = None
+
+        for action, child in self.children.items():
+            uct_score = child.value() + cpuct * child.prior * math.sqrt(self.visit_count) / \
+                (1 + child.visit_count)
+            if uct_score > best_score:
+                best_score = uct_score
+                best_action = action
+                best_child = child
+
+        return best_action, best_child
+
+    def expand(self, action_space, child_priors, child_done):  # Add a child_done parameter
+        for action, prior in zip(range(action_space), child_priors):
+            if action not in self.children:
+                self.children[action] = Node(self.state, prior, action, child_done)  # Pass the child_done to the new Node
+
+    def update_stats(self, reward):
+        self.total_value += reward  # 총 보상 업데이트
+        self.visit_count += 1  # 방문 횟수 증가
+
+    def select_action(self, temperature=1):
+        visit_counts = np.array(
+            [child.visit_count for child in self.children.values()])
+        actions = [action for action in self.children.keys()]
+        if temperature == 0:
+            action = actions[np.argmax(visit_counts)]
+        else:
+            visit_counts = visit_counts ** (1/temperature)  # apply temperature
+            # normalize to get probabilities
+            visit_counts = visit_counts / sum(visit_counts)
+            action = np.random.choice(actions, p=visit_counts)
+
+        return action
```

### Comparing `modular_rl-0.2.2/modular_rl.egg-info/SOURCES.txt` & `modular_rl-0.2.3/modular_rl.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,29 @@
 modular_rl.egg-info/PKG-INFO
 modular_rl.egg-info/SOURCES.txt
 modular_rl.egg-info/dependency_links.txt
 modular_rl.egg-info/requires.txt
 modular_rl.egg-info/top_level.txt
 modular_rl/agents/__init__.py
 modular_rl/agents/_agent.py
+modular_rl/agents/mcis.py
 modular_rl/agents/mcts.py
 modular_rl/agents/ppo.py
 modular_rl/networks/__init__.py
 modular_rl/networks/actor_critic.py
 modular_rl/networks/policy.py
 modular_rl/networks/value.py
 modular_rl/params/__init__.py
+modular_rl/params/mcis.py
 modular_rl/params/mcts.py
 modular_rl/params/ppo.py
 modular_rl/tester/__init__.py
+modular_rl/tester/mcis.py
 modular_rl/tester/mcts.py
 modular_rl/tester/ppo.py
 modular_rl/util/__init__.py
 modular_rl/util/node.py
+tests/test_mcis.py
+tests/test_mcis_modular.py
 tests/test_mcts.py
 tests/test_ppo.py
 tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.2.2/pyproject.toml` & `modular_rl-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `modular_rl-0.2.2/setup.py` & `modular_rl-0.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.2.2',
+    version='0.2.3',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/ModularRL',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

