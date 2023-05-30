# Comparing `tmp/pref_voting-0.3.3.tar.gz` & `tmp/pref_voting-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.3.3.tar", max compression
+gzip compressed data, was "pref_voting-0.3.4.tar", max compression
```

## Comparing `pref_voting-0.3.3.tar` & `pref_voting-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.3.3/LICENSE
--rw-r--r--   0        0        0     3200 2023-05-26 16:48:07.750821 pref_voting-0.3.3/README.md
--rw-r--r--   0        0        0       22 2023-05-26 17:56:45.043572 pref_voting-0.3.3/pref_voting/__init__.py
--rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.3.3/pref_voting/analysis.py
--rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.3.3/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.3.3/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.3.3/pref_voting/axioms.py
--rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.3.3/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.3.3/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.3.3/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.3.3/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     4664 2023-05-26 14:20:44.876014 pref_voting-0.3.3/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.3.3/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.3.3/pref_voting/helper.py
--rw-r--r--   0        0        0    73193 2023-05-25 12:07:00.027553 pref_voting-0.3.3/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.3.3/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    59218 2023-05-26 17:44:51.542166 pref_voting-0.3.3/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.3.3/pref_voting/other_methods.py
--rw-r--r--   0        0        0    28609 2023-05-26 17:29:58.194223 pref_voting-0.3.3/pref_voting/profiles.py
--rw-r--r--   0        0        0    25273 2023-05-26 17:38:33.040884 pref_voting-0.3.3/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.3.3/pref_voting/rankings.py
--rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.3.3/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.3.3/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    13967 2023-05-26 12:07:03.892154 pref_voting-0.3.3/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.3.3/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.3.3/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.3.3/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    53001 2023-05-26 17:56:28.071379 pref_voting-0.3.3/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      689 2023-05-26 17:56:45.042547 pref_voting-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4153 1970-01-01 00:00:00.000000 pref_voting-0.3.3/setup.py
--rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 pref_voting-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3200 2023-05-26 17:57:30.757597 pref_voting-0.3.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-30 21:25:26.910744 pref_voting-0.3.4/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.3.4/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.3.4/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.3.4/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.3.4/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.3.4/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8551 2023-05-30 17:01:09.832556 pref_voting-0.3.4/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.3.4/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.3.4/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     4680 2023-05-30 19:57:47.963280 pref_voting-0.3.4/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.3.4/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.3.4/pref_voting/helper.py
+-rw-r--r--   0        0        0    74050 2023-05-29 22:04:12.246564 pref_voting-0.3.4/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.3.4/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    59218 2023-05-26 17:44:51.542166 pref_voting-0.3.4/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.3.4/pref_voting/other_methods.py
+-rw-r--r--   0        0        0    28614 2023-05-30 20:06:31.706933 pref_voting-0.3.4/pref_voting/profiles.py
+-rw-r--r--   0        0        0    25273 2023-05-26 17:38:33.040884 pref_voting-0.3.4/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.3.4/pref_voting/rankings.py
+-rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.3.4/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.3.4/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    15088 2023-05-30 20:17:01.412933 pref_voting-0.3.4/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.3.4/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.3.4/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.3.4/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    53001 2023-05-26 17:56:28.071379 pref_voting-0.3.4/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      689 2023-05-30 21:25:26.909630 pref_voting-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4153 1970-01-01 00:00:00.000000 pref_voting-0.3.4/setup.py
+-rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 pref_voting-0.3.4/PKG-INFO
```

### Comparing `pref_voting-0.3.3/LICENSE` & `pref_voting-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/README.md` & `pref_voting-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 - v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 - v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
 - v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
-- v0.3.1 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
+- v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.3.3/pref_voting/analysis.py` & `pref_voting-0.3.4/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/axiom.py` & `pref_voting-0.3.4/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/c1_methods.py` & `pref_voting-0.3.4/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/combined_methods.py` & `pref_voting-0.3.4/pref_voting/combined_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     
     Implementations of voting methods that combine multiple methods
 """
 
 from pref_voting.voting_method import *
 from pref_voting.scoring_methods import plurality, borda
 from pref_voting.iterative_methods import iterated_removal_cl, instant_runoff, instant_runoff_put, instant_runoff_for_truncated_linear_orders
-from pref_voting.c1_methods import smith_set, copeland
+from pref_voting.c1_methods import smith_set, copeland, top_cycle
+from pref_voting.margin_based_methods import minimax
 from pref_voting.profiles import Profile
 from pref_voting.profiles_with_ties import ProfileWithTies
 
 @vm(name="Daunou")
 def daunou(profile, curr_cands=None):
     """Implementation of Daunou's voting method as described in the paper: https://link.springer.com/article/10.1007/s00355-020-01276-w
 
@@ -229,19 +230,18 @@
     else:
         return instant_runoff_put(profile, curr_cands=curr_cands)
 
 def compose(vm1, vm2):
     """After restricting the profile to the set of vm1 winners, run vm2
 
     Args:
-        profile (Profile): An anonymous profile of linear orders on a set of candidates
-        curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
+        vm1, vm2 (VotingMethod): The voting methods to be composed.
 
     Returns:
-        A sorted list of candidates
+        A VotingMethod that composes vm1 and vm2.
 
     :Example:
 
     .. exec_code::
 
         from pref_voting.profiles import Profile
         from pref_voting.combined_methods import compose
@@ -264,18 +264,21 @@
 
         vm1_ws = vm1(edata, curr_cands=curr_cands)
 
         return vm2(edata, curr_cands=vm1_ws)
 
     return VotingMethod(_vm, name=f"{vm1.name}-{vm2.name}")
 
+smith_minimax = compose(top_cycle, minimax)
+
 copeland_borda = compose(copeland, borda)
 
 combined_vms = [
     daunou, 
     blacks, 
     condorcet_irv, 
     condorcet_irv_put, 
     smith_irv, 
     smith_irv_put, 
-    copeland_borda
-    ]
+    smith_minimax,
+    copeland_borda,
+    ]
```

### Comparing `pref_voting-0.3.3/pref_voting/dominance_axioms.py` & `pref_voting-0.3.4/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/generate_profiles.py` & `pref_voting-0.3.4/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/generate_utility_profiles.py` & `pref_voting-0.3.4/pref_voting/generate_utility_profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,29 +82,29 @@
     )
 
 
 def generate_spatial_utility_profile(num_cands, num_voters, params = None):
     """
     Create a spatial utility profile using the Rabinowitz and Macdonald (1989) mixed model described in Section 3, pp. 745 - 747 of "Voting behavior under the directional spatial model of electoral competition" by S. Merrill III. 
 
-    .. note:  When, beta = 1, it is the proximity model (i.e., utilities are the negative of the Euclidean distance), and when beta = 0, it is the directional model.
+    .. note:  When, beta = 1, it is the proximity model (i.e., utilities are the negative of the squared Euclidean distance), and when beta = 0, it is the directional model.
 
     Args:
         num_cands (int): The number of candidates.
         num_voters (int): The number of voters.
         params (tuple): A tuple of the form (num_dim, beta) where num_dim is the number of dimensions and beta is the beta parameter of the mixed model. The default is (2, 1).
 
     Returns:
         UtilityProfile: A spatial utility profile.
     """
     params = params if params is not None else (2, 1)
 
     # the first component of the parameter is the number of dimensions, 
     # the second component is used to define the mixed model: 
-    # beta = 1 is proximity model (i.e., Euclidean distance)
+    # beta = 1 is proximity model (i.e., squared Euclidean distance)
     num_dim, beta = params
 
     mean = [0] * num_dim  # mean is 0 for each dimension
     cov = np.diag([1] * num_dim)  # diagonal covariance
 
     # sample candidate/voter positions using a multivariate normal distribution
     cand_positions = np.random.multivariate_normal(np.array(mean), cov, num_cands)
```

### Comparing `pref_voting-0.3.3/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.3.4/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/helper.py` & `pref_voting-0.3.4/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/iterative_methods.py` & `pref_voting-0.3.4/pref_voting/iterative_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,25 +164,25 @@
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
      
     return sorted(winners)
 
 
 @vm(name = "Instant Runoff PUT")
 def instant_runoff_put(profile, curr_cands = None):
-    """Instant Runoff (:func:`instant_runoff`) with parallel universe tie-breaking (PUT).  Apply the Instant Runoff method with a tie-breaker for each possible linear order over the candidates. 
+    """Instant Runoff (:func:`instant_runoff`) with parallel universe tie-breaking (PUT), defined recursively: if there is a candidate with a strict majority of first-place votes, that candidate is the IRV-PUT winner; otherwise a candidate x is an IRV-PUT winner if there is some candidate y with minimal plurality score such that after removing y from the profile, x is an IRV-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
 
     .. warning:: 
-        This will take a long time on profiles with many candidates. 
+        This will take a long time on profiles with many candidates having the same plurality scores
 
     :Example: 
 
     .. exec_code:: 
 
         from pref_voting.profiles import Profile
         from pref_voting.iterative_methods import instant_runoff, instant_runoff_tb, instant_runoff_put
@@ -205,29 +205,30 @@
         print("tie_breaker = [2, 1, 0]")
         instant_runoff_tb.display(prof, tie_breaker=[2, 1, 0])
         print()
         instant_runoff_put.display(prof)
 
     """
     
-    candidates = profile.candidates if curr_cands is None else curr_cands
-    cands_to_ignore = np.empty(0) if curr_cands is None else np.array([c for c in profile.candidates if c not in curr_cands])
-    
+    candidates = profile.candidates if curr_cands is None else curr_cands 
+
     strict_maj_size = profile.strict_maj_size()
-    
-    rs, rcounts = profile.rankings_counts # get all the ranking data
-        
-    winners = [c for c in candidates 
-               if _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
+    majority_winner = [cand for cand, value in profile.plurality_scores(candidates).items() if value >= strict_maj_size]
 
-    if len(winners) == 0:
-        # run Instant Runoff with tie-breaker for each permutation of candidates
-        for tb in permutations(candidates):
-            winners += instant_runoff_tb(profile, curr_cands = curr_cands, tie_breaker = tb) 
-    return sorted(list(set(winners)))
+    if len(majority_winner) > 0:
+        return majority_winner
+
+    cands_to_remove = [cand for cand, value in profile.plurality_scores(candidates).items() if value == min(profile.plurality_scores(candidates).values())]
+    
+    winners = []
+    for cand_to_remove in cands_to_remove:
+        new_winners = instant_runoff_put(profile, curr_cands = [c for c in candidates if not c == cand_to_remove])
+        winners = winners + new_winners
+    
+    return sorted(set(winners))
 
 
 # Create some aliases for instant runoff
 instant_runoff_put.set_name("Hare PUT")
 hare_put = copy.deepcopy(instant_runoff_put)
 instant_runoff_put.set_name("Ranked Choice PUT")
 ranked_choice_put = copy.deepcopy(instant_runoff_put)
@@ -1497,15 +1498,15 @@
         sc_winners = split_cycle(edata, curr_cands = sc_winners, strength_function = strength_function)
         
     return sorted(sc_winners)
 
 @vm(name = "Benham")
 def benham(profile, curr_cands = None):
     """
-    As long as the profile has no Condorcet winner, eliminate the candidate with the lowest plurality score. Then elect the Condorcet winner of the restricted profile. 
+    As long as the profile has no Condorcet winner, eliminate the candidate with the lowest plurality score.
     
     .. important::
         If there is  more than one candidate with the fewest number of first-place votes, then *all* such candidates are removed from the profile. 
     
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
@@ -1600,41 +1601,66 @@
             if cw is not None: 
                 winners = [cw]
     return sorted(winners)
 
 
 @vm(name = "Benham PUT")
 def benham_put(profile, curr_cands = None):
-    """Benham (:func:`benham`) with parallel universe tie-breaking (PUT).  Apply the Benham method with a tie-breaker for each possible linear order over the candidates. 
+    """Benham (:func:`benham`) with parallel universe tie-breaking (PUT), defined recursively: if there is a Condorcet winner, that candidate is the Benham-PUT winner; otherwise a candidate x is a Benham-PUT winner if there is some candidate y with minimal plurality score such that after removing y from the profile, x is a Benham-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
 
     Returns: 
         A sorted list of candidates
 
     .. warning:: 
-        This will take a long time on profiles with many candidates. 
-
+        This will take a long time on profiles with many candidates having the same plurality scores.
 
     """
+    candidates = profile.candidates if curr_cands is None else curr_cands 
+
+    cw = profile.condorcet_winner(candidates)
+    if cw is not None:
+        return [cw]
+
+    cands_to_remove = [cand for cand, value in profile.plurality_scores(candidates).items() if value == min(profile.plurality_scores(candidates).values())]
     
-    candidates = profile.candidates if curr_cands is None else curr_cands
-    cands_to_ignore = np.empty(0) if curr_cands is None else np.array([c for c in profile.candidates if c not in curr_cands])
-    
-    cw = profile.condorcet_winner(curr_cands = [c for c in profile.candidates if not isin(cands_to_ignore, c)])
+    winners = []
+    for cand_to_remove in cands_to_remove:
+        new_winners = benham_put(profile, curr_cands = [c for c in candidates if not c == cand_to_remove])
+        winners = winners + new_winners
     
-    winners = [cw] if cw is not None else list()
-        
-    if len(winners) == 0:
-        # run Instant Runoff with tie-breaker for each permutation of candidates
-        for tb in permutations(candidates):
-            winners += instant_runoff_tb(profile, curr_cands = curr_cands, tie_breaker = tb) 
-    return sorted(list(set(winners)))
+    return sorted(set(winners))
+
+def iterated(vm):
+    """Iteratively restrict the set of candidates to the vm winners until reaching a fixpoint.
+
+    Args:
+        vm (VotingMethod): A voting method.
+
+    Returns:
+        A voting method that iterates vm.
+
+    """
+
+    def _vm(edata, curr_cands = None):
+
+        candidates = edata.candidates if curr_cands is None else curr_cands
+
+        vm_ws = vm(edata, curr_cands=candidates)
+
+        while not vm_ws == candidates:
+            candidates = vm_ws
+            vm_ws = vm(edata, curr_cands=candidates)
+
+        return vm_ws
+
+    return VotingMethod(_vm, name=f"Iterated {vm.name}")
     
 iterated_vms = [
     instant_runoff,
     instant_runoff_tb,
     instant_runoff_put,
     hare,
     ranked_choice,
```

### Comparing `pref_voting-0.3.3/pref_voting/maj_graph_ex1.png` & `pref_voting-0.3.4/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/margin_based_methods.py` & `pref_voting-0.3.4/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/other_methods.py` & `pref_voting-0.3.4/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/profiles.py` & `pref_voting-0.3.4/pref_voting/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,7 +674,9 @@
     """
     
     assert c != ranking[-1], "can't drop a candidate already in last place"
     
     c_idx = ranking.index(c)
     ranking[c_idx + 1], ranking[c_idx] = ranking[c_idx],ranking[c_idx + 1]
     return ranking
+
+
```

### Comparing `pref_voting-0.3.3/pref_voting/profiles_with_ties.py` & `pref_voting-0.3.4/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/rankings.py` & `pref_voting-0.3.4/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/scoring_methods.py` & `pref_voting-0.3.4/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/utility_methods.py` & `pref_voting-0.3.4/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/utility_profiles.py` & `pref_voting-0.3.4/pref_voting/utility_profiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -312,14 +312,44 @@
         return ProfileWithTies(
             [u.ranking() for u in self._utilities],
             rcounts = self.ucounts,
             candidates = self.domain, 
             cmap = self.cmap
         )
     
+    def write(self):
+        """Write the profile to a string."""
+
+        uprof_str = f"{len(self.domain)};{self.num_voters}"
+        for u in self.utilities: 
+            u_str = ''
+            for c in u.domain: 
+                if u.has_utility(c):
+                    u_str += f"{c}:{u(c)},"
+            uprof_str += f";{u_str[0:-1]}"
+        return str(uprof_str)
+
+    @classmethod
+    def from_string(cls, uprof_str): 
+        """
+        Returns a profile of utilities described by ``uprof_str``.
+
+        ``uprof_str`` must be in the format produced by the :meth:`pref_voting.UtilityProfile.write` function.
+        """
+        uprof_data = uprof_str.split(";")
+
+        num_alternatives,num_voters,utilities = int(uprof_data[0]),int(uprof_data[1]),uprof_data[2:]
+
+        util_maps = [{int(cu.split(":")[0]): float(cu.split(":")[1]) for cu in utils.split(",")} if utils != '' else {} for utils in utilities]
+
+        if len(util_maps) != num_voters: 
+            raise Exception("Number of voters does not match the number of utilities.")
+        
+        return cls(util_maps, domain=range(num_alternatives))
+
     def display(self, vmap = None, show_totals=False):
         """Display a utility profile as an ascii table (using tabulate). If ``show_totals`` is true then the sum, min, and max of the utilities are displayed.
 
         """
         
         utilities = self.utilities
```

### Comparing `pref_voting-0.3.3/pref_voting/variable_voter_axioms.py` & `pref_voting-0.3.4/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/voting_method.py` & `pref_voting-0.3.4/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.3.4/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.3/pyproject.toml` & `pref_voting-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.3.3"
+version = "0.3.4"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.3.3/setup.py` & `pref_voting-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.3.3',
+    'version': '0.3.4',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3.1 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.3.3/PKG-INFO` & `pref_voting-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.3.3
+Version: 0.3.4
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -84,15 +84,15 @@
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 - v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 - v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
 - v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
-- v0.3.1 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
+- v0.3.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

