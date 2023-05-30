# Comparing `tmp/Signal8-1.8.tar.gz` & `tmp/Signal8-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-1.8.tar", last modified: Mon May 22 23:15:27 2023, max compression
+gzip compressed data, was "Signal8-1.9.tar", last modified: Tue May 30 21:07:16 2023, max compression
```

## Comparing `Signal8-1.8.tar` & `Signal8-1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 23:15:19.644830 Signal8-1.8/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.8/LICENSE
--rw-rw-rw-   0        0        0     4356 2023-05-22 23:15:27.502308 Signal8-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3868 2023-05-22 23:14:08.000000 Signal8-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 23:15:19.570831 Signal8-1.8/Signal8/
--rw-rw-rw-   0        0        0     6519 2023-05-19 19:59:38.000000 Signal8-1.8/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.8/Signal8/__init__.py
--rw-rw-rw-   0        0        0      130 2023-05-19 19:25:12.000000 Signal8-1.8/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:15:19.631832 Signal8-1.8/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.8/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     7867 2023-05-19 19:40:29.000000 Signal8-1.8/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2407 2023-05-22 23:12:51.000000 Signal8-1.8/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.8/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    12174 2023-05-19 19:30:46.000000 Signal8-1.8/Signal8/utils/simple_env.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:15:27.490306 Signal8-1.8/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4356 2023-05-22 23:15:27.000000 Signal8-1.8/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-05-22 23:15:27.000000 Signal8-1.8/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 23:15:27.000000 Signal8-1.8/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 23:15:27.000000 Signal8-1.8/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 23:15:27.513305 Signal8-1.8/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-05-22 23:14:59.000000 Signal8-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:07:16.093798 Signal8-1.9/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-1.9/LICENSE
+-rw-rw-rw-   0        0        0     4356 2023-05-30 21:07:16.084627 Signal8-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3868 2023-05-22 23:14:08.000000 Signal8-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 21:07:15.965630 Signal8-1.9/Signal8/
+-rw-rw-rw-   0        0        0     9650 2023-05-30 20:36:11.000000 Signal8-1.9/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       83 2023-05-19 15:45:44.000000 Signal8-1.9/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      225 2023-05-30 20:54:02.000000 Signal8-1.9/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:07:16.079629 Signal8-1.9/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-1.9/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5746 2023-05-30 18:28:08.000000 Signal8-1.9/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     4265 2023-05-30 17:26:10.000000 Signal8-1.9/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-1.9/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    12606 2023-05-30 19:27:51.000000 Signal8-1.9/Signal8/utils/simple_env.py
+drwxrwxrwx   0        0        0        0 2023-05-30 21:07:16.044627 Signal8-1.9/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4356 2023-05-30 21:07:15.000000 Signal8-1.9/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-05-30 21:07:15.000000 Signal8-1.9/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 21:07:15.000000 Signal8-1.9/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 21:07:15.000000 Signal8-1.9/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 21:07:16.093798 Signal8-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-05-30 21:07:07.000000 Signal8-1.9/setup.py
```

### Comparing `Signal8-1.8/LICENSE` & `Signal8-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-1.8/PKG-INFO` & `Signal8-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.8
+Version: 1.9
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.8/README.md` & `Signal8-1.9/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-1.8/Signal8/utils/core.py` & `Signal8-1.9/Signal8/utils/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,224 +5,165 @@
     def __init__(self):
         # physical position
         self.p_pos = None
         # physical velocity
         self.p_vel = None
 
 
-class AgentState(
-    EntityState
-):  # state of agents (including communication and internal/mental state)
+class AgentState(EntityState):  # state of agents
     def __init__(self):
         super().__init__()
-        # communication utterance
-        self.c = None
-
-
-class Action:  # action of the agent
-    def __init__(self):
-        # physical action
-        self.u = None
-        # communication action
-        self.c = None
 
 
 class Entity:  # properties and state of physical world entity
     def __init__(self):
         # name
         self.name = ""
         # properties:
-        self.size = 0.050
+        self.size = 0.1
         # entity can move / be pushed
         self.movable = False
         # entity collides with others
         self.collide = True
-        # material density (affects mass)
-        self.density = 25.0
         # color
         self.color = None
-        # max speed and accel
-        self.max_speed = None
-        self.accel = None
         # state
         self.state = EntityState()
         # mass
         self.initial_mass = 1.0
 
     @property
     def mass(self):
         return self.initial_mass
 
 
-class Landmark(Entity):  # properties of landmark entities
+class Goal(Entity): # properties of goal entities
     def __init__(self):
         super().__init__()
 
 
+class Obstacle(Entity):  # properties of obstacles entities
+    def __init__(self):
+        super().__init__()
+        # entity can be moved / pushed
+        self.movable = False
+        # action
+        self.action = None
+        # script behavior to execute
+        self.action_callback = None
+    
+    # updates the state of the obstacle
+    def move(self, dt=0.1, damping=0.25):
+        self.state.p_vel = self.state.p_vel * (1 - damping)
+        self.state.p_vel += (self.action / self.mass) * dt
+        self.state.p_pos += self.state.p_vel * dt
+        
+
 class Agent(Entity):  # properties of agent entities
     def __init__(self):
         super().__init__()
         # agents are movable by default
         self.movable = True
-        # cannot send communication signals
-        self.silent = False
-        # cannot observe the world
-        self.blind = False
-        # physical motor noise amount
-        self.u_noise = None
-        # communication noise amount
-        self.c_noise = None
-        # control range
-        self.u_range = 1.0
+        # reached goal state
+        self.reached_goal = False
+        # reached start state after reaching goal
+        self.returned_to_safety = False
+        # starting physical position
+        self.start_pos = None
         # state
         self.state = AgentState()
         # action
-        self.action = Action()
-        # script behavior to execute
-        self.action_callback = None
-
+        self.action = None
 
 class World:  # multi-agent world
-    def __init__(self, dynamic_obstacles=False):
+    def __init__(self):
         # list of agents and entities (can change at execution-time!)
         self.agents = []
-        self.landmarks = []
-        # communication channel dimensionality
-        self.dim_c = 0
+        self.goals = []
+        self.obstacles = []
         # position dimensionality
         self.dim_p = 2
         # color dimensionality
         self.dim_color = 3
         # simulation timestep
         self.dt = 0.1
         # physical damping
         self.damping = 0.25
         # contact response parameters
         self.contact_force = 1e2
         self.contact_margin = 1e-3
         # problem scenarios
-        self.dynamic_obstacles = dynamic_obstacles
-        self.problem_scenarios = None
+        self.problem_scenarios = []
         self.problem_name = None
         self.start_constr = None
         self.goal_constr = None
         self.static_obstacle_constr = None
         self.dynamic_obstacle_constr = None
         
     # return all entities in the world
     @property
     def entities(self):
-        return self.agents + self.landmarks
-
-    # return all agents controllable by external policies
-    @property
-    def policy_agents(self):
-        return [agent for agent in self.agents if agent.action_callback is None]
-
-    # return all agents controlled by world scripts
-    @property
-    def scripted_agents(self):
-        return [agent for agent in self.agents if agent.action_callback is not None]
+        return self.agents + self.goals + self.obstacles
 
     # update state of the world
     def step(self):
-        # set actions for scripted agents
-        for agent in self.scripted_agents:
-            agent.action = agent.action_callback(agent, self)
         # gather forces applied to entities
         p_force = [None] * len(self.entities)
         # apply agent physical controls
         p_force = self.apply_action_force(p_force)
         # apply environment forces
         p_force = self.apply_environment_force(p_force)
         # integrate physical state
         self.integrate_state(p_force)
-        # update agent state
-        for agent in self.agents:
-            self.update_agent_state(agent)
 
     # gather agent action forces
     def apply_action_force(self, p_force):
         # set applied forces
         for i, agent in enumerate(self.agents):
             if agent.movable:
-                noise = (
-                    np.random.randn(*agent.action.u.shape) * agent.u_noise
-                    if agent.u_noise
-                    else 0.0
-                )
-                p_force[i] = agent.action.u + noise
+                p_force[i] = agent.action
         return p_force
 
-    # gather physical forces acting on entities
+    # gather physical forces acting on agents
     def apply_environment_force(self, p_force):
         # simple (but inefficient) collision response
-        for a, entity_a in enumerate(self.entities):
-            for b, entity_b in enumerate(self.entities):
+        for a, agent_a in enumerate(self.agents):
+            for b, agent_b in enumerate(self.agents):
                 if b <= a:
                     continue
-                [f_a, f_b] = self.get_collision_force(entity_a, entity_b)
+                [f_a, f_b] = self.get_collision_force(agent_a, agent_b)
                 if f_a is not None:
                     if p_force[a] is None:
                         p_force[a] = 0.0
                     p_force[a] = f_a + p_force[a]
                 if f_b is not None:
                     if p_force[b] is None:
                         p_force[b] = 0.0
                     p_force[b] = f_b + p_force[b]
         return p_force
 
     # integrate physical state
     def integrate_state(self, p_force):
-        for i, entity in enumerate(self.entities):
-            if not entity.movable:
-                continue
-            entity.state.p_vel = entity.state.p_vel * (1 - self.damping)
+        for i, agent in enumerate(self.agents):
+            agent.state.p_vel = agent.state.p_vel * (1 - self.damping)
             if p_force[i] is not None:
-                entity.state.p_vel += (p_force[i] / entity.mass) * self.dt
-            if entity.max_speed is not None:
-                speed = np.sqrt(
-                    np.square(entity.state.p_vel[0]) +
-                    np.square(entity.state.p_vel[1])
-                )
-                if speed > entity.max_speed:
-                    entity.state.p_vel = (
-                        entity.state.p_vel
-                        / np.sqrt(
-                            np.square(entity.state.p_vel[0])
-                            + np.square(entity.state.p_vel[1])
-                        )
-                        * entity.max_speed
-                    )
-
-            entity.state.p_pos += entity.state.p_vel * self.dt
-
-    def update_agent_state(self, agent):
-        # set communication state (directly for now)
-        if agent.silent:
-            agent.state.c = np.zeros(self.dim_c)
-        else:
-            noise = (
-                np.random.randn(*agent.action.c.shape) * agent.c_noise
-                if agent.c_noise
-                else 0.0
-            )
-            agent.state.c = agent.action.c + noise
-
-    # get collision forces for any contact between two entities
-    def get_collision_force(self, entity_a, entity_b):
-        if (not entity_a.collide) or (not entity_b.collide):
+                agent.state.p_vel += (p_force[i] / agent.mass) * self.dt
+            agent.state.p_pos += agent.state.p_vel * self.dt
+
+    # get collision forces for any contact between two agents
+    def get_collision_force(self, agent_a, agent_b):
+        if (not agent_a.collide) or (not agent_b.collide):
             return [None, None]  # not a collider
-        if entity_a is entity_b:
+        if agent_a is agent_b:
             return [None, None]  # don't collide against itself
         # compute actual distance between entities
-        delta_pos = entity_a.state.p_pos - entity_b.state.p_pos
+        delta_pos = agent_a.state.p_pos - agent_b.state.p_pos
         dist = np.sqrt(np.sum(np.square(delta_pos)))
         # minimum allowable distance
-        dist_min = entity_a.size + entity_b.size
+        dist_min = agent_a.size + agent_b.size
         # softmax penetration
         k = self.contact_margin
         penetration = np.logaddexp(0, -(dist - dist_min) / k) * k
         force = self.contact_force * delta_pos / dist * penetration
-        force_a = +force if entity_a.movable else None
-        force_b = -force if entity_b.movable else None
-        return [force_a, force_b]
+        force_a = +force if agent_a.movable else None
+        force_b = -force if agent_b.movable else None
+        return [force_a, force_b]
```

### Comparing `Signal8-1.8/Signal8/utils/simple_env.py` & `Signal8-1.9/Signal8/utils/simple_env.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,36 +59,29 @@
         self.world = world
         self.continuous_actions = continuous_actions
         self.local_ratio = local_ratio
 
         self.scenario.reset_world(self.world, self.np_random)
         self.agents = [agent.name for agent in self.world.agents]
         self.possible_agents = self.agents[:]
-        self._index_map = {
-            agent.name: idx for idx, agent in enumerate(self.world.agents)
-        }
+        self._index_map = {agent.name: idx for idx, agent in enumerate(self.world.agents)}
 
         self._agent_selector = agent_selector(self.agents)
 
         # set spaces
         self.action_spaces = dict()
         self.observation_spaces = dict()
         state_dim = 0
         for agent in self.world.agents:
             if agent.movable:
                 space_dim = self.world.dim_p * 2 + 1
             elif self.continuous_actions:
                 space_dim = 0
             else:
                 space_dim = 1
-            if not agent.silent:
-                if self.continuous_actions:
-                    space_dim += self.world.dim_c
-                else:
-                    space_dim *= self.world.dim_c
 
             obs_dim = len(self.scenario.observation(agent, self.world))
             state_dim += obs_dim
             if self.continuous_actions:
                 self.action_spaces[agent.name] = spaces.Box(
                     low=0, high=1, shape=(space_dim,)
                 )
@@ -131,49 +124,47 @@
             self.scenario.observation(
                 self.world.agents[self._index_map[agent]], self.world
             ).astype(np.float32)
             for agent in self.possible_agents
         )
         return np.concatenate(states, axis=None)
 
-    def reset(self, seed=None, return_info=False, options=None):
+    def reset(self, seed=None, return_info=False, options=None):        
         if seed is not None:
             self.seed(seed=seed)
-        problem_scenario = options['problem_name'] if options is not None else 'v_cluster'
+            
+        problem_scenario = options['problem_name']
         self.scenario.reset_world(self.world, self.np_random, problem_scenario)
 
         self.agents = self.possible_agents[:]
         self.rewards = {name: 0.0 for name in self.agents}
         self._cumulative_rewards = {name: 0.0 for name in self.agents}
         self.terminations = {name: False for name in self.agents}
         self.truncations = {name: False for name in self.agents}
         self.infos = {name: {} for name in self.agents}
 
         self.agent_selection = self._agent_selector.reset()
         self.steps = 0
 
-        self.current_actions = [None] * len(self.world.policy_agents)
+        self.current_actions = [None] * len(self.world.agents)
 
     def _execute_world_step(self):
         # set action for each agent
-        for i, agent in enumerate(self.world.policy_agents):
+        for i, agent in enumerate(self.world.agents):
             action = self.current_actions[i]
             scenario_action = []
             if agent.movable:
                 mdim = self.world.dim_p * 2 + 1
                 if self.continuous_actions:
                     scenario_action.append(action[0:mdim])
                     action = action[mdim:]
                 else:
                     scenario_action.append(action % mdim)
                     action //= mdim
-            if not agent.silent:
-                scenario_action.append(action)
-            self._set_action(scenario_action, agent,
-                             self.action_spaces[agent.name])
+            self._set_action(scenario_action, agent, self.action_spaces[agent.name])
 
         self.world.step()
 
         global_reward = 0.0
         if self.local_ratio is not None:
             global_reward = float(self.scenario.global_reward(self.world))
 
@@ -187,70 +178,97 @@
             else:
                 reward = agent_reward
 
             self.rewards[agent.name] = reward
 
     # set env action for a particular agent
     def _set_action(self, action, agent, action_space, time=None):
-        agent.action.u = np.zeros(self.world.dim_p)
-        agent.action.c = np.zeros(self.world.dim_c)
-
         if agent.movable:
             # physical action
-            agent.action.u = np.zeros(self.world.dim_p)
+            agent.action = np.zeros(self.world.dim_p)
             if self.continuous_actions:
                 # Process continuous action as in OpenAI MPE
-                agent.action.u[0] += action[0][1] - action[0][2]
-                agent.action.u[1] += action[0][3] - action[0][4]
+                agent.action[0] += action[0][1] - action[0][2]
+                agent.action[1] += action[0][3] - action[0][4]
             else:
                 # process discrete action
                 if action[0] == 1:
-                    agent.action.u[0] = -1.0
-                if action[0] == 2:
-                    agent.action.u[0] = +1.0
-                if action[0] == 3:
-                    agent.action.u[1] = -1.0
-                if action[0] == 4:
-                    agent.action.u[1] = +1.0
+                    agent.action[0] = -1.0
+                elif action[0] == 2:
+                    agent.action[0] = +1.0
+                elif action[0] == 3:
+                    agent.action[1] = -1.0
+                elif action[0] == 4:
+                    agent.action[1] = +1.0
             sensitivity = 5.0
-            if agent.accel is not None:
-                sensitivity = agent.accel
-            agent.action.u *= sensitivity
-            action = action[1:]
-        if not agent.silent:
-            # communication action
-            if self.continuous_actions:
-                agent.action.c = action[0]
-            else:
-                agent.action.c = np.zeros(self.world.dim_c)
-                agent.action.c[action[0]] = 1.0
+            agent.action *= sensitivity
             action = action[1:]
         # make sure we used all elements of action
         assert len(action) == 0
+    
+    # Check if episode is terminated or truncated
+    def _episode_status(self):        
+        dynamic_obs = [obs for obs in self.world.obstacles if obs.movable]
+        static_obs = [obs for obs in self.world.obstacles if not obs.movable]
+    
+        goal_dist_threshold = self.world.agents[0].size + self.world.agents[0].goal.size
+        static_obs_threshold = self.world.agents[0].size + static_obs[0].size
+        
+        goal_dist = [np.linalg.norm(agent.state.p_pos - agent.goal.state.p_pos) for agent in self.world.agents]
+        static_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in static_obs)
+                           for agent in self.world.agents]
+        
+        crossed_threshold_static = [dist <= static_obs_threshold for dist in static_obs_dist]
+        
+        try:
+            for i in range(len(dynamic_obs)):
+                self.scenario.obstacle_locks[i].acquire()
+                dynamic_obs_dist = [min(np.linalg.norm(agent.state.p_pos - obs.state.p_pos) for obs in dynamic_obs)
+                                    for agent in self.world.agents] 
+                dynamic_obs_threshold = [agent.size + obs.size for agent, obs in zip(self.world.agents, dynamic_obs)]   
+            
+            crossed_threshold_dynamic = [dist <= threshold for dist, threshold in zip(dynamic_obs_dist, dynamic_obs_threshold)]
+                        
+            truncations = [crossed_stat or crossed_dyn for crossed_stat, crossed_dyn in zip(crossed_threshold_static, crossed_threshold_dynamic)]
+            truncations = [True] * self.num_agents if self.steps >= self.max_cycles else truncations
+            
+            terminations = [False] * self.num_agents
+            for i, dist in enumerate(goal_dist):
+                if dist <= goal_dist_threshold:
+                    self.agents[i].reached_goal = True
+            
+            for i, agent in enumerate(self.world.agents):
+                if agent.reached_goal:
+                    dist_to_start = np.linalg.norm(agent.state.p_pos - agent.start_pos)
+                    start_dist_threshold = self.world.agents[0].size * 2
+                    if dist_to_start <= start_dist_threshold:
+                        terminations[i] = True
+        finally:
+            [self.scenario.obstacle_locks[i].release() for i, _ in enumerate(dynamic_obs)]
+            return {'terminations': terminations, 'truncations': truncations}
 
     def step(self, action):
         if (
             self.terminations[self.agent_selection]
             or self.truncations[self.agent_selection]
         ):
             self._was_dead_step(action)
             return
-        
+
         current_idx = self._index_map[self.agent_selection]
+        next_idx = (current_idx + 1) % self.num_agents
+        self.agent_selection = self._agent_selector.next()
         self.current_actions[current_idx] = action
 
-        self._execute_world_step()
-        goal_dist = np.linalg.norm(self.world.agents[0].state.p_pos-self.world.agents[0].goal.state.p_pos)
-        landmark_dist = [np.linalg.norm(self.world.agents[0].state.p_pos - landmark.state.p_pos) for landmark in self.world.landmarks[1:]]
-        self.steps += 1
-        min_dist = self.world.agents[0].size + self.world.agents[0].goal.size
-        if self.steps >= self.max_cycles or min(landmark_dist) <= min_dist:
-            self.truncations[self.agent_selection] = True
-        if min_dist >= goal_dist:
-            self.terminations[self.agent_selection] = True
+        if next_idx == 0:
+            self.steps += 1
+            self._execute_world_step()
+            status = self._episode_status()
+            self.terminations = status['terminations']
+            self.truncations = status['truncations']
 
         if self.render_mode == "human":
             self.render()
 
     def enable_render(self, mode="human"):
         if not self.renderOn and mode == "human":
             self.screen = pygame.display.set_mode(self.screen.get_size())
@@ -303,35 +321,12 @@
             pygame.draw.circle(
                 self.screen, (0, 0, 0), (x, y), entity.size * 350, 1
             )  # borders
             assert (
                 0 < x < self.width and 0 < y < self.height
             ), f"Coordinates {(x, y)} are out of bounds."
 
-            # text
-            if isinstance(entity, Agent):
-                if entity.silent:
-                    continue
-                if np.all(entity.state.c == 0):
-                    word = "_"
-                elif self.continuous_actions:
-                    word = (
-                        "[" +
-                        ",".join(
-                            [f"{comm:.2f}" for comm in entity.state.c]) + "]"
-                    )
-
-                message = entity.name + " sends " + word + "   "
-                message_x_pos = self.width * 0.05
-                message_y_pos = self.height * 0.95 - \
-                    (self.height * 0.05 * text_line)
-                self.game_font.render_to(
-                    self.screen, (message_x_pos,
-                                  message_y_pos), message, (0, 0, 0)
-                )
-                text_line += 1
-
     def close(self):
         if self.renderOn:
             pygame.event.pump()
             pygame.display.quit()
             self.renderOn = False
```

### Comparing `Signal8-1.8/Signal8.egg-info/PKG-INFO` & `Signal8-1.9/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 1.8
+Version: 1.9
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-1.8/setup.py` & `Signal8-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="1.8",
+    version="1.9",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

