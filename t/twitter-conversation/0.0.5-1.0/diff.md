# Comparing `tmp/twitter-conversation-0.0.5.tar.gz` & `tmp/twitter_conversation-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-conversation-0.0.5.tar", max compression
+gzip compressed data, was "twitter_conversation-1.0.tar", max compression
```

## Comparing `twitter-conversation-0.0.5.tar` & `twitter_conversation-1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     2539 2022-10-05 10:05:34.655741 twitter-conversation-0.0.5/README.md
--rw-r--r--   0        0        0     1357 2022-10-05 10:27:04.701089 twitter-conversation-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       22 2022-10-05 10:27:04.701089 twitter-conversation-0.0.5/twitter_conversation/__init__.py
--rw-r--r--   0        0        0    11620 2022-10-05 10:05:34.655741 twitter-conversation-0.0.5/twitter_conversation/obtain.py
--rw-r--r--   0        0        0     9631 2022-10-05 10:05:34.655741 twitter-conversation-0.0.5/twitter_conversation/scripts/reply_tree.py
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 twitter-conversation-0.0.5/setup.py
--rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 twitter-conversation-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     5882 2023-05-30 20:41:13.137071 twitter_conversation-1.0/README.md
+-rw-r--r--   0        0        0     1368 2023-05-30 20:46:44.093514 twitter_conversation-1.0/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-05-30 20:46:44.093514 twitter_conversation-1.0/twitter_conversation/__init__.py
+-rw-r--r--   0        0        0    11620 2023-05-30 20:41:13.141071 twitter_conversation-1.0/twitter_conversation/obtain.py
+-rw-r--r--   0        0        0     9813 2023-05-30 20:41:13.141071 twitter_conversation-1.0/twitter_conversation/scripts/reply_tree.py
+-rw-r--r--   0        0        0     7380 1970-01-01 00:00:00.000000 twitter_conversation-1.0/PKG-INFO
```

### Comparing `twitter-conversation-0.0.5/pyproject.toml` & `twitter_conversation-1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "twitter-conversation"
-version = "0.0.5"
+version = "1.0"
 description = "This is a project to obtain Twitter conversation over the Twitter-API v2 and to store them as csv."
 authors = ["Marc Feger <marc.feger@uni-duesseldorf.de>"]
-license = "BSD-4-Clause"
+license = "CC BY-NC-SA 4.0"
 readme = "README.md"
 repository = "https://gitlab.cs.uni-duesseldorf.de/feger/twitter-conversation"
 classifiers = [
     "Programming Language :: Python :: 3.10",
-    "License :: OSI Approved :: BSD License",
+    "License :: OSI Approved :: Common Public License",
     "Framework :: Pytest",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Topic :: Database",
     "Topic :: Database :: Database Engines/Servers",
     "Topic :: Internet",
```

### Comparing `twitter-conversation-0.0.5/twitter_conversation/obtain.py` & `twitter_conversation-1.0/twitter_conversation/obtain.py`

 * *Files identical despite different names*

### Comparing `twitter-conversation-0.0.5/twitter_conversation/scripts/reply_tree.py` & `twitter_conversation-1.0/twitter_conversation/scripts/reply_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,16 @@
                                                  max_results=500)
         single_reply_tree.obtain(only_root=args_config.get('only_root'))
         single_reply_tree.write_to_csv(path=args_config.get('path'))
 
     elif args_config.get('mode') == "multiple_conversations":
         conversation_starting_tweets: pd.DataFrame = pd.read_csv(args_config.get('starting_tweets'),
                                                                  index_col=args_config.get('index'))
+        # Drop duplicated indices and keep only the unique ones
+        conversation_starting_tweets = conversation_starting_tweets[~conversation_starting_tweets.index.duplicated()]
         for conversation_starting_tweet in conversation_starting_tweets.index:
             multiple_reply_tree: ReplyTree = ReplyTree(client,
                                                        conversation_id=conversation_starting_tweet,
                                                        start_time=args_config.get('start'),
                                                        max_results=500)
             multiple_reply_tree.obtain(only_root=args_config.get('only_root'))
             multiple_reply_tree.write_to_csv(path=args_config.get('path'))
```

