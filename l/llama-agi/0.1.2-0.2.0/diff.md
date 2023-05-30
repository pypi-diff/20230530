# Comparing `tmp/llama_agi-0.1.2.tar.gz` & `tmp/llama_agi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_agi-0.1.2.tar", max compression
+gzip compressed data, was "llama_agi-0.2.0.tar", max compression
```

## Comparing `llama_agi-0.1.2.tar` & `llama_agi-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1093 2023-04-24 02:20:57.763744 llama_agi-0.1.2/LICENSE
--rw-r--r--   0        0        0     1865 2023-04-24 02:20:57.763744 llama_agi-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/__init__.py
--rw-r--r--   0        0        0     4588 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/default_task_prompts.py
--rw-r--r--   0        0        0     2471 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/execution_agent/SimpleExecutionAgent.py
--rw-r--r--   0        0        0     3306 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/execution_agent/ToolExecutionAgent.py
--rw-r--r--   0        0        0      177 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/execution_agent/__init__.py
--rw-r--r--   0        0        0     1991 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/execution_agent/base.py
--rw-r--r--   0        0        0     3007 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/runners/AutoAGIRunner.py
--rw-r--r--   0        0        0     5245 2023-04-25 01:24:45.683530 llama_agi-0.1.2/llama_agi/runners/AutoStreamlitAGIRunner.py
--rw-r--r--   0        0        0      166 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/runners/__init__.py
--rw-r--r--   0        0        0      692 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/runners/base.py
--rw-r--r--   0        0        0     6990 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/task_manager/LlamaTaskManager.py
--rw-r--r--   0        0        0       87 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/task_manager/__init__.py
--rw-r--r--   0        0        0     2446 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/task_manager/base.py
--rw-r--r--   0        0        0      721 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/tools/NoteTakingTools.py
--rw-r--r--   0        0        0     1188 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/tools/WebpageSearchTool.py
--rw-r--r--   0        0        0      178 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/tools/__init__.py
--rw-r--r--   0        0        0     1261 2023-04-24 02:20:57.763744 llama_agi-0.1.2/llama_agi/utils.py
--rw-r--r--   0        0        0     1052 2023-04-25 01:30:58.533532 llama_agi-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 llama_agi-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-24 02:20:57.763744 llama_agi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1865 2023-04-24 02:20:57.763744 llama_agi-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 02:20:57.763744 llama_agi-0.2.0/llama_agi/__init__.py
+-rw-r--r--   0        0        0     4588 2023-04-24 02:20:57.763744 llama_agi-0.2.0/llama_agi/default_task_prompts.py
+-rw-r--r--   0        0        0     2460 2023-05-30 00:04:06.255324 llama_agi-0.2.0/llama_agi/execution_agent/SimpleExecutionAgent.py
+-rw-r--r--   0        0        0     3332 2023-05-30 00:04:06.255324 llama_agi-0.2.0/llama_agi/execution_agent/ToolExecutionAgent.py
+-rw-r--r--   0        0        0      164 2023-05-30 00:04:06.235324 llama_agi-0.2.0/llama_agi/execution_agent/__init__.py
+-rw-r--r--   0        0        0     1977 2023-05-30 00:04:06.255324 llama_agi-0.2.0/llama_agi/execution_agent/base.py
+-rw-r--r--   0        0        0     3039 2023-05-30 00:04:06.255324 llama_agi-0.2.0/llama_agi/runners/AutoAGIRunner.py
+-rw-r--r--   0        0        0     5385 2023-05-30 00:04:06.275324 llama_agi-0.2.0/llama_agi/runners/AutoStreamlitAGIRunner.py
+-rw-r--r--   0        0        0      155 2023-05-30 00:04:06.235324 llama_agi-0.2.0/llama_agi/runners/__init__.py
+-rw-r--r--   0        0        0      692 2023-04-24 02:20:57.763744 llama_agi-0.2.0/llama_agi/runners/base.py
+-rw-r--r--   0        0        0     7031 2023-05-30 00:04:06.295324 llama_agi-0.2.0/llama_agi/task_manager/LlamaTaskManager.py
+-rw-r--r--   0        0        0       89 2023-05-30 00:04:06.235324 llama_agi-0.2.0/llama_agi/task_manager/__init__.py
+-rw-r--r--   0        0        0     2442 2023-05-30 00:04:06.245324 llama_agi-0.2.0/llama_agi/task_manager/base.py
+-rw-r--r--   0        0        0      729 2023-05-30 00:04:06.235324 llama_agi-0.2.0/llama_agi/tools/NoteTakingTools.py
+-rw-r--r--   0        0        0     1155 2023-05-29 22:50:39.265294 llama_agi-0.2.0/llama_agi/tools/WebpageSearchTool.py
+-rw-r--r--   0        0        0      160 2023-05-30 00:04:06.235324 llama_agi-0.2.0/llama_agi/tools/__init__.py
+-rw-r--r--   0        0        0     1280 2023-05-30 00:04:06.245324 llama_agi-0.2.0/llama_agi/utils.py
+-rw-r--r--   0        0        0     1136 2023-05-30 00:05:45.895325 llama_agi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 llama_agi-0.2.0/PKG-INFO
```

### Comparing `llama_agi-0.1.2/LICENSE` & `llama_agi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.2/README.md` & `llama_agi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.2/llama_agi/default_task_prompts.py` & `llama_agi-0.2.0/llama_agi/default_task_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.2/llama_agi/execution_agent/SimpleExecutionAgent.py` & `llama_agi-0.2.0/llama_agi/execution_agent/SimpleExecutionAgent.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,30 +11,31 @@
 
 
 class SimpleExecutionAgent(BaseExecutionAgent):
     """Simple Execution Agent
 
     This agent uses an LLM to execute a basic action without tools.
     The LlamaAgentPrompts.execution_prompt defines how this execution agent
-    behaves. 
+    behaves.
 
     Usually, this is used for simple tasks, like generating the initial list of tasks.
-    
-    The execution template kwargs are automatically extracted and expected to be 
+
+    The execution template kwargs are automatically extracted and expected to be
     specified in execute_task().
-    
+
     Args:
         llm (Union[BaseLLM, BaseChatModel]): The langchain LLM class to use.
-        model_name: (str): The name of the OpenAI model to use, if the LLM is 
+        model_name: (str): The name of the OpenAI model to use, if the LLM is
         not provided.
         max_tokens: (int): The maximum number of tokens the LLM can generate.
-        prompts: (LlamaAgentPrompts): The prompt templates used during execution. 
-        The only prompt used byt the SimpleExecutionAgent is 
+        prompts: (LlamaAgentPrompts): The prompt templates used during execution.
+        The only prompt used byt the SimpleExecutionAgent is
         LlamaAgentPrompts.execution_prompt.
     """
+
     def __init__(
         self,
         llm: Optional[Union[BaseLLM, BaseChatModel]] = None,
         model_name: str = "text-davinci-003",
         max_tokens: int = 512,
         prompts: LlamaAgentPrompts = LlamaAgentPrompts(),
         tools: Optional[List[Tool]] = None,
```

### Comparing `llama_agi-0.1.2/llama_agi/execution_agent/ToolExecutionAgent.py` & `llama_agi-0.2.0/llama_agi/execution_agent/ToolExecutionAgent.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from langchain.chat_models.base import BaseChatModel
 
 from llama_agi.execution_agent.base import BaseExecutionAgent, LlamaAgentPrompts
 
 
 class ToolExecutionAgent(BaseExecutionAgent):
     """Tool Execution Agent
-    
+
     This agent is a wrapper around the zero-shot agent from Langchain. Using
-    a set of tools, the agent is expected to carry out and complete some task 
+    a set of tools, the agent is expected to carry out and complete some task
     that will help achieve an overall objective.
-    
-    The agents overall behavior is controlled by the LlamaAgentPrompts.agent_prefix 
+
+    The agents overall behavior is controlled by the LlamaAgentPrompts.agent_prefix
     and LlamaAgentPrompts.agent_suffix prompt templates.
 
-    The execution template kwargs are automatically extracted and expected to be 
-    specified in execute_task(). 
+    The execution template kwargs are automatically extracted and expected to be
+    specified in execute_task().
 
     execute_task() also returns the intermediate steps, for additional debugging and is
-    used for the streamlit example. 
+    used for the streamlit example.
 
     Args:
         llm (Union[BaseLLM, BaseChatModel]): The langchain LLM class to use.
-        model_name: (str): The name of the OpenAI model to use, if the LLM is 
+        model_name: (str): The name of the OpenAI model to use, if the LLM is
         not provided.
         max_tokens: (int): The maximum number of tokens the LLM can generate.
-        prompts: (LlamaAgentPrompts): The prompt templates used during execution. 
-        The Tool Execution Agent uses LlamaAgentPrompts.agent_prefix and 
+        prompts: (LlamaAgentPrompts): The prompt templates used during execution.
+        The Tool Execution Agent uses LlamaAgentPrompts.agent_prefix and
         LlamaAgentPrompts.agent_suffix.
         tools: (List[Tool]): The list of langchain tools for the execution agent to use.
     """
+
     def __init__(
         self,
         llm: Optional[Union[BaseLLM, BaseChatModel]] = None,
         model_name: str = "text-davinci-003",
         max_tokens: int = 512,
         prompts: LlamaAgentPrompts = LlamaAgentPrompts(),
         tools: Optional[List[Tool]] = None,
@@ -67,14 +68,17 @@
             input_variables=input_variables,
         )
         self._llm_chain = LLMChain(llm=self._llm, prompt=self._agent_prompt)
         self._agent = ZeroShotAgent(
             llm_chain=self._llm_chain, tools=self.tools, verbose=True
         )
         self._execution_chain = AgentExecutor.from_agent_and_tools(
-            agent=self._agent, tools=self.tools, verbose=True, return_intermediate_steps=True
+            agent=self._agent,
+            tools=self.tools,
+            verbose=True,
+            return_intermediate_steps=True,
         )
 
     def execute_task(self, **prompt_kwargs: Any) -> Dict[str, str]:
         """Execute a task, using tools."""
         result = self._execution_chain(prompt_kwargs)
         return result
```

### Comparing `llama_agi-0.1.2/llama_agi/execution_agent/base.py` & `llama_agi-0.2.0/llama_agi/execution_agent/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,37 @@
 from typing import Any, Dict, List, Optional, Union
 
 from langchain.agents.tools import Tool
 from langchain.llms import OpenAI, BaseLLM
 from langchain.chat_models.base import BaseChatModel
 from langchain.chat_models import ChatOpenAI
 
-from llama_agi.default_task_prompts import (
-    LC_PREFIX, LC_SUFFIX, LC_EXECUTION_PROMPT
-)
+from llama_agi.default_task_prompts import LC_PREFIX, LC_SUFFIX, LC_EXECUTION_PROMPT
 
 
 @dataclass
 class LlamaAgentPrompts:
     execution_prompt: str = LC_EXECUTION_PROMPT
     agent_prefix: str = LC_PREFIX
     agent_suffix: str = LC_SUFFIX
 
 
 class BaseExecutionAgent:
     """Base Execution Agent
-    
+
     Args:
         llm (Union[BaseLLM, BaseChatModel]): The langchain LLM class to use.
-        model_name: (str): The name of the OpenAI model to use, if the LLM is 
+        model_name: (str): The name of the OpenAI model to use, if the LLM is
         not provided.
         max_tokens: (int): The maximum number of tokens the LLM can generate.
         prompts: (LlamaAgentPrompts): The prompt templates used during execution.
-        tools: (List[Tool]): The list of langchain tools for the execution 
+        tools: (List[Tool]): The list of langchain tools for the execution
         agent to use.
     """
+
     def __init__(
         self,
         llm: Optional[Union[BaseLLM, BaseChatModel]] = None,
         model_name: str = "text-davinci-003",
         max_tokens: int = 512,
         prompts: LlamaAgentPrompts = LlamaAgentPrompts(),
         tools: Optional[List[Tool]] = None,
```

### Comparing `llama_agi-0.1.2/llama_agi/runners/AutoAGIRunner.py` & `llama_agi-0.2.0/llama_agi/runners/AutoAGIRunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,17 @@
             )
             initial_task_list_result = simple_execution_agent.execute_task(
                 objective=objective,
                 task=initial_task_prompt,
                 completed_tasks_summary=initial_completed_tasks_summary,
             )
 
-            initial_task_list = self.task_manager.parse_task_list(initial_task_list_result['output'])
+            initial_task_list = self.task_manager.parse_task_list(
+                initial_task_list_result["output"]
+            )
 
             # add tasks to the task manager
             self.task_manager.add_new_tasks(initial_task_list)
 
         # prioritize initial tasks
         self.task_manager.prioritize_tasks(objective)
 
@@ -49,15 +51,15 @@
             cur_task = self.task_manager.get_next_task()
 
             # Execute current task
             result = self.execution_agent.execute_task(
                 objective=objective,
                 cur_task=cur_task,
                 completed_tasks_summary=completed_tasks_summary,
-            )['output']
+            )["output"]
 
             # store the task and result as completed
             self.task_manager.add_completed_task(cur_task, result)
 
             # generate new task(s), if needed
             self.task_manager.generate_new_tasks(objective, cur_task, result)
```

### Comparing `llama_agi-0.1.2/llama_agi/runners/AutoStreamlitAGIRunner.py` & `llama_agi-0.2.0/llama_agi/runners/AutoStreamlitAGIRunner.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,35 +23,35 @@
 class AutoStreamlitAGIRunner(BaseAGIRunner):
     def run(
         self,
         objective: str,
         initial_task: str,
         sleep_time: int,
         initial_task_list: Optional[List[str]] = None,
-        max_iterations: Optional[int] = None
+        max_iterations: Optional[int] = None,
     ) -> None:
-        
+
         run_initial_task = False
-        if 'logs' not in st.session_state:
-            st.session_state['logs'] = []
-            st.session_state['state_str'] = "No state yet!"
-            st.session_state['tasks_summary'] = ""
+        if "logs" not in st.session_state:
+            st.session_state["logs"] = []
+            st.session_state["state_str"] = "No state yet!"
+            st.session_state["tasks_summary"] = ""
             run_initial_task = True
 
         logs_col, state_col = st.columns(2)
 
         with logs_col:
             st.subheader("Execution Log")
             st_logs = st.empty()
-        st_logs.write(st.session_state['logs'])
-        
+        st_logs.write(st.session_state["logs"])
+
         with state_col:
             st.subheader("AGI State")
             st_state = st.empty()
-        st_state.write(st.session_state['state_str'])
+        st_state.write(st.session_state["state_str"])
 
         if run_initial_task:
             # get initial list of tasks
             if initial_task_list:
                 self.task_manager.add_new_tasks(initial_task_list)
             else:
                 initial_completed_tasks_summary = (
@@ -67,69 +67,78 @@
                 )
                 initial_task_list_result = simple_execution_agent.execute_task(
                     objective=objective,
                     task=initial_task_prompt,
                     completed_tasks_summary=initial_completed_tasks_summary,
                 )
 
-                initial_task_list = self.task_manager.parse_task_list(initial_task_list_result['output'])
+                initial_task_list = self.task_manager.parse_task_list(
+                    initial_task_list_result["output"]
+                )
 
                 # add tasks to the task manager
                 self.task_manager.add_new_tasks(initial_task_list)
 
             # prioritize initial tasks
             self.task_manager.prioritize_tasks(objective)
 
             tasks_summary = initial_completed_tasks_summary
-            st.session_state['tasks_summary'] = tasks_summary
+            st.session_state["tasks_summary"] = tasks_summary
 
             # update streamlit state
-            st.session_state['state_str'] = log_current_status(initial_task, initial_task_list_result['output'], tasks_summary, self.task_manager.current_tasks, return_str=True)
-            if st.session_state['state_str']:
-                st_state.markdown(st.session_state['state_str'].replace("\n", "\n\n"))
+            st.session_state["state_str"] = log_current_status(
+                initial_task,
+                initial_task_list_result["output"],
+                tasks_summary,
+                self.task_manager.current_tasks,
+                return_str=True,
+            )
+            if st.session_state["state_str"]:
+                st_state.markdown(st.session_state["state_str"].replace("\n", "\n\n"))
 
         for _ in range(0, max_iterations):
             # Get the next task
             cur_task = self.task_manager.get_next_task()
 
             # Execute current task
             result_dict = self.execution_agent.execute_task(
                 objective=objective,
                 cur_task=cur_task,
-                completed_tasks_summary=st.session_state['tasks_summary'],
+                completed_tasks_summary=st.session_state["tasks_summary"],
             )
-            result = result_dict['output']
-            
-            # update logs 
-            log = make_intermediate_steps_pretty(json.dumps(result_dict['intermediate_steps'])) + [result]
-            st.session_state['logs'].append(log)
-            st_logs.write(st.session_state['logs'])
+            result = result_dict["output"]
+
+            # update logs
+            log = make_intermediate_steps_pretty(
+                json.dumps(result_dict["intermediate_steps"])
+            ) + [result]
+            st.session_state["logs"].append(log)
+            st_logs.write(st.session_state["logs"])
 
             # store the task and result as completed
             self.task_manager.add_completed_task(cur_task, result)
 
             # generate new task(s), if needed
             self.task_manager.generate_new_tasks(objective, cur_task, result)
 
             # Summarize completed tasks
             completed_tasks_summary = self.task_manager.get_completed_tasks_summary()
-            st.session_state['tasks_summary'] = completed_tasks_summary
+            st.session_state["tasks_summary"] = completed_tasks_summary
 
             # log state of AGI to streamlit
-            st.session_state['state_str'] = log_current_status(
+            st.session_state["state_str"] = log_current_status(
                 cur_task,
                 result,
                 completed_tasks_summary,
                 self.task_manager.current_tasks,
-                return_str=True
+                return_str=True,
             )
-            if st.session_state['state_str'] is not None:
-                st_state.markdown(st.session_state['state_str'].replace("\n", "\n\n"))
+            if st.session_state["state_str"] is not None:
+                st_state.markdown(st.session_state["state_str"].replace("\n", "\n\n"))
 
             # Quit the loop?
             if len(self.task_manager.current_tasks) == 0:
                 st.success("Out of tasks! Objective Accomplished?")
                 break
 
             # wait a bit to let you read what's happening
             time.sleep(sleep_time)
-
```

### Comparing `llama_agi-0.1.2/llama_agi/runners/base.py` & `llama_agi-0.2.0/llama_agi/runners/base.py`

 * *Files identical despite different names*

### Comparing `llama_agi-0.1.2/llama_agi/task_manager/LlamaTaskManager.py` & `llama_agi-0.2.0/llama_agi/task_manager/LlamaTaskManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 from llama_agi.task_manager.base import BaseTaskManager, LlamaTaskPrompts
 from llama_agi.utils import initialize_task_list_index
 from llama_agi.default_task_prompts import NO_COMPLETED_TASKS_SUMMARY
 
 
 class LlamaTaskManager(BaseTaskManager):
     """Llama Task Manager
-    
+
     This task manager uses LlamaIndex to create and prioritize tasks. Using
     the LlamaTaskPrompts, the task manager will create tasks that work
     towards achieving an overall objective.
 
     New tasks are created based on the prev task+result, completed tasks summary,
     and the overall objective.
 
     Tasks are then prioritized using the overall objective and current list of tasks.
 
     Args:
         tasks (List[str]): The initial list of tasks to complete.
-        prompts: (LlamaTaskPrompts): The prompts to control the task creation 
+        prompts: (LlamaTaskPrompts): The prompts to control the task creation
         and prioritization.
-        tasK_service_context (ServiceContext): The LlamaIndex service context to use 
+        tasK_service_context (ServiceContext): The LlamaIndex service context to use
         for task creation and prioritization.
 
     """
+
     def __init__(
         self,
         tasks: List[str],
         prompts: LlamaTaskPrompts = LlamaTaskPrompts(),
         task_service_context: Optional[ServiceContext] = None,
     ) -> None:
         super().__init__(
@@ -47,15 +48,17 @@
             self.completed_tasks, service_context=self.task_service_context
         )
 
         self.task_create_qa_template = self.prompts.task_create_qa_template
         self.task_create_refine_template = self.prompts.task_create_refine_template
 
         self.task_prioritize_qa_template = self.prompts.task_prioritize_qa_template
-        self.task_prioritize_refine_template = self.prompts.task_prioritize_refine_template
+        self.task_prioritize_refine_template = (
+            self.prompts.task_prioritize_refine_template
+        )
 
     def _get_task_create_templates(
         self, prev_task: str, prev_result: str
     ) -> Tuple[QuestionAnswerPrompt, RefinePrompt]:
         """Fetch the task create prompts as llama_index objects."""
         text_qa_template = self.task_create_qa_template.format(
             prev_result=prev_result,
@@ -100,27 +103,27 @@
             ]
         return new_tasks
 
     def get_completed_tasks_summary(self) -> str:
         """Generate a summary of completed tasks."""
         if len(self.completed_tasks) == 0:
             return NO_COMPLETED_TASKS_SUMMARY
-        summary = self.completed_tasks_index.query(
-            "Summarize the current completed tasks", response_mode="tree_summarize"
+        summary = self.completed_tasks_index.as_query_engine(
+            response_mode="tree_summarize"
+        ).query(
+            "Summarize the current completed tasks",
         )
         return str(summary)
 
     def prioritize_tasks(self, objective: str) -> None:
         """Prioritize the current list of incomplete tasks."""
         (text_qa_template, refine_template) = self._get_task_prioritize_templates()
-        prioritized_tasks = self.current_tasks_index.query(
-            objective,
-            text_qa_template=text_qa_template,
-            refine_template=refine_template,
-        )
+        prioritized_tasks = self.current_tasks_index.as_query_engine(
+            text_qa_template=text_qa_template, refine_template=refine_template
+        ).query(objective)
 
         new_tasks = []
         for task in str(prioritized_tasks).split("\n"):
             task = re.sub(r"^[0-9]+\.", "", task).strip()
             if len(task) > 10:
                 new_tasks.append(task)
         self.current_tasks = [Document(x) for x in new_tasks]
@@ -131,19 +134,17 @@
     def generate_new_tasks(
         self, objective: str, prev_task: str, prev_result: str
     ) -> None:
         """Generate new tasks given the previous task and result."""
         (text_qa_template, refine_template) = self._get_task_create_templates(
             prev_task, prev_result
         )
-        task_list_response = self.completed_tasks_index.query(
-            objective,
-            text_qa_template=text_qa_template,
-            refine_template=refine_template,
-        )
+        task_list_response = self.completed_tasks_index.as_query_engine(
+            text_qa_template=text_qa_template, refine_template=refine_template
+        ).query(objective)
         new_tasks = self.parse_task_list(str(task_list_response))
         self.add_new_tasks(new_tasks)
 
     def get_next_task(self) -> str:
         """Get the next task to complete."""
         next_task = self.current_tasks.pop().get_text()
         self.current_tasks_index = initialize_task_list_index(
```

### Comparing `llama_agi-0.1.2/llama_agi/task_manager/base.py` & `llama_agi-0.2.0/llama_agi/task_manager/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,24 @@
     task_create_refine_template: str = DEFAULT_REFINE_TASK_CREATE_TMPL
     task_prioritize_qa_template: str = DEFAULT_TASK_PRIORITIZE_TMPL
     task_prioritize_refine_template: str = DEFAULT_REFINE_TASK_PRIORITIZE_TMPL
 
 
 class BaseTaskManager:
     """Base Task Manager
-    
+
     Args:
         tasks (List[str]): The initial list of tasks to complete.
-        prompts: (LlamaTaskPrompts): The prompts to control the task creation 
+        prompts: (LlamaTaskPrompts): The prompts to control the task creation
         and prioritization.
-        tasK_service_context (ServiceContext): The LlamaIndex service context to use 
+        tasK_service_context (ServiceContext): The LlamaIndex service context to use
         for task creation and prioritization.
 
     """
+
     def __init__(
         self,
         tasks: List[str],
         prompts: LlamaTaskPrompts = LlamaTaskPrompts(),
         task_service_context: Optional[ServiceContext] = None,
     ) -> None:
         self.current_tasks = [Document(x) for x in tasks]
```

### Comparing `llama_agi-0.1.2/llama_agi/tools/NoteTakingTools.py` & `llama_agi-0.2.0/llama_agi/tools/NoteTakingTools.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,9 +13,11 @@
     return "Note successfully recorded."
 
 
 @tool("Search Notes")
 def search_notes(query_str: str) -> str:
     """Useful for searching through notes that you previously recorded."""
     global note_index
-    response = note_index.query(query_str, similarity_top_k=3, response_mode="compact")
+    response = note_index.as_query_engine(
+        similarity_top_k=3,
+    ).query(query_str)
     return str(response)
```

### Comparing `llama_agi-0.1.2/llama_agi/tools/WebpageSearchTool.py` & `llama_agi-0.2.0/llama_agi/tools/WebpageSearchTool.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,13 @@
     url = prompt.split("\n")[0]
     query_str = " ".join(prompt.split("\n")[1:])
 
     try:
         documents = loader.load_data(urls=[url])
         service_context = ServiceContext.from_defaults(chunk_size_limit=512)
         index = initialize_search_index(documents, service_context=service_context)
-        query_result = index.query(
-            query_str, similarity_top_k=3, response_mode="compact"
-        )
+        query_result = index.as_query_engine(similarity_top_k=3).query(query_str)
         return str(query_result)
     except ValueError as e:
         return str(e)
     except Exception:
         return "Encountered an error while searching the webpage."
```

### Comparing `llama_agi-0.1.2/llama_agi/utils.py` & `llama_agi-0.2.0/llama_agi/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from typing import Any, List, Optional
 
-from llama_index import GPTSimpleVectorIndex, GPTListIndex, ServiceContext, Document
+from llama_index import GPTVectorStoreIndex, GPTListIndex, ServiceContext, Document
 from llama_index.indices.base import BaseGPTIndex
 
 
 def initialize_task_list_index(
     documents: List[Document], service_context: Optional[ServiceContext] = None
 ) -> BaseGPTIndex[Any]:
     return GPTListIndex.from_documents(documents, service_context=service_context)
 
 
 def initialize_search_index(
     documents: List[Document], service_context: Optional[ServiceContext] = None
 ) -> BaseGPTIndex[Any]:
-    return GPTSimpleVectorIndex.from_documents(
+    return GPTVectorStoreIndex.from_documents(
         documents, service_context=service_context
     )
 
 
 def log_current_status(
-    cur_task: str, result: str, completed_tasks_summary: str, task_list: List[Document], return_str: bool = False
+    cur_task: str,
+    result: str,
+    completed_tasks_summary: str,
+    task_list: List[Document],
+    return_str: bool = False,
 ) -> Optional[str]:
     status_string = f"""
     __________________________________
     Completed Tasks Summary: {completed_tasks_summary.strip()}
     Current Task: {cur_task.strip()}
     Result: {result.strip()}
     Task List: {", ".join([x.get_text().strip() for x in task_list])}
```

### Comparing `llama_agi-0.1.2/pyproject.toml` & `llama_agi-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "llama_agi"
-version = "0.1.2"
+version = "0.2.0"
 description = "Building AGI loops using LlamaIndex and Langchain"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/run-llama/llama-lab/tree/main/llama_agi"
 include = [
     "LICENSE",
 ]
 keywords = ["LLM", "LlamaIndex", "Langchain", "AGI"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain = "==0.0.141"
-llama-index = "==0.5.16"
-streamlit = ">=1.21.0"
-
+altair = "==4.2.2"
+langchain = "==0.0.154"
+llama-index = "==0.6.13"
+streamlit = "==1.21.0"
+transformers = ">=0.4.29"
+google-api-python-client = ">=2.87.0"
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.0.249"
 black = "^23.1.0"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
```

### Comparing `llama_agi-0.1.2/PKG-INFO` & `llama_agi-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: llama-agi
-Version: 0.1.2
+Version: 0.2.0
 Summary: Building AGI loops using LlamaIndex and Langchain
 Home-page: https://github.com/run-llama/llama-lab/tree/main/llama_agi
 License: MIT
 Keywords: LLM,LlamaIndex,Langchain,AGI
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: langchain (==0.0.141)
-Requires-Dist: llama-index (==0.5.16)
-Requires-Dist: streamlit (>=1.21.0)
+Requires-Dist: altair (==4.2.2)
+Requires-Dist: google-api-python-client (>=2.87.0)
+Requires-Dist: langchain (==0.0.154)
+Requires-Dist: llama-index (==0.6.13)
+Requires-Dist: streamlit (==1.21.0)
+Requires-Dist: transformers (>=0.4.29)
 Project-URL: Repository, https://github.com/run-llama/llama-lab/tree/main/llama_agi
 Description-Content-Type: text/markdown
 
 # 🤖 Llama AGI 🦙
 
 This python package allows you to quickly create Auto-GPT-like agents, using LlamaIndex and Langchain.
```

