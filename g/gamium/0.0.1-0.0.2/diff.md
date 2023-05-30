# Comparing `tmp/gamium-0.0.1.tar.gz` & `tmp/gamium-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamium-0.0.1.tar", max compression
+gzip compressed data, was "gamium-0.0.2.tar", max compression
```

## Comparing `gamium-0.0.1.tar` & `gamium-0.0.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0        0 2023-05-20 09:32:59.561980 gamium-0.0.1/README.md
--rw-r--r--   0        0        0      626 2023-05-25 07:46:40.594452 gamium-0.0.1/gamium/__init__.py
--rw-r--r--   0        0        0      500 2023-05-24 13:45:20.085940 gamium-0.0.1/gamium/__main__.py
--rw-r--r--   0        0        0    11229 2023-05-27 16:29:57.716876 gamium-0.0.1/gamium/actions/action_chain.py
--rw-r--r--   0        0        0     1449 2023-05-27 15:57:54.253933 gamium-0.0.1/gamium/actions/key_by.py
--rw-r--r--   0        0        0      471 2023-05-27 16:37:25.765448 gamium-0.0.1/gamium/condition/condition.py
--rw-r--r--   0        0        0     2138 2023-05-27 17:05:44.381885 gamium-0.0.1/gamium/condition/until.py
--rw-r--r--   0        0        0      245 2023-05-27 15:36:03.742756 gamium-0.0.1/gamium/condition/wait_condition.py
--rw-r--r--   0        0        0      269 2023-05-28 09:47:38.321943 gamium-0.0.1/gamium/errors/gamium_error.py
--rw-r--r--   0        0        0     6303 2023-05-27 16:57:16.462228 gamium-0.0.1/gamium/gamium_client.py
--rw-r--r--   0        0        0     8498 2023-05-27 16:29:22.380147 gamium-0.0.1/gamium/gamium_service.py
--rw-r--r--   0        0        0     1248 2023-05-27 16:48:14.859904 gamium-0.0.1/gamium/igamium_client.py
--rw-r--r--   0        0        0       62 2023-05-20 09:32:59.575340 gamium-0.0.1/gamium/internal/__init__.py
--rw-r--r--   0        0        0     1147 2023-05-20 09:32:59.575844 gamium-0.0.1/gamium/internal/logger.py
--rw-r--r--   0        0        0      672 2023-05-24 10:00:22.753241 gamium-0.0.1/gamium/internal/size_prefixed_recv_queue.py
--rw-r--r--   0        0        0      349 2023-05-27 15:45:16.895951 gamium-0.0.1/gamium/locator/by.py
--rw-r--r--   0        0        0       59 2023-05-20 09:32:59.576661 gamium-0.0.1/gamium/locator/locator.py
--rw-r--r--   0        0        0      906 2023-05-27 15:44:54.654718 gamium-0.0.1/gamium/locator/rpc_by.py
--rw-r--r--   0        0        0       47 2023-05-22 13:59:37.380671 gamium-0.0.1/gamium/locator/rpc_locator.py
--rw-r--r--   0        0        0     1996 2023-05-27 16:48:30.437448 gamium-0.0.1/gamium/object/player.py
--rw-r--r--   0        0        0     3925 2023-05-27 16:48:34.013675 gamium-0.0.1/gamium/object/ui_element.py
--rw-r--r--   0        0        0      390 2023-05-23 10:45:11.917741 gamium-0.0.1/gamium/options/__init__.py
--rw-r--r--   0        0        0      142 2023-05-27 16:07:06.395341 gamium-0.0.1/gamium/options/action_click_options.py
--rw-r--r--   0        0        0      204 2023-05-27 16:19:40.425215 gamium-0.0.1/gamium/options/action_drag_options.py
--rw-r--r--   0        0        0       92 2023-05-24 12:03:15.929711 gamium-0.0.1/gamium/options/action_move_options.py
--rw-r--r--   0        0        0      144 2023-05-27 16:20:01.758848 gamium-0.0.1/gamium/options/action_scroll_options.py
--rw-r--r--   0        0        0      171 2023-05-27 16:20:08.327138 gamium-0.0.1/gamium/options/execute_rpc_options.py
--rw-r--r--   0        0        0      132 2023-05-27 16:20:12.178882 gamium-0.0.1/gamium/options/find_objects_options.py
--rw-r--r--   0        0        0      374 2023-05-27 16:20:21.453410 gamium-0.0.1/gamium/options/move_player_options.py
--rw-r--r--   0        0        0      262 2023-05-27 16:20:28.044046 gamium-0.0.1/gamium/options/query_object_interactable_options.py
--rw-r--r--   0        0        0      139 2023-05-27 16:20:31.256151 gamium-0.0.1/gamium/options/send_key_options.py
--rw-r--r--   0        0        0       89 2023-05-22 09:57:37.806139 gamium-0.0.1/gamium/options/set_text_options.py
--rw-r--r--   0        0        0      362 2023-05-27 16:20:41.882990 gamium-0.0.1/gamium/options/wait_options.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.787754 gamium-0.0.1/gamium/protocol/__init__.py
--rw-r--r--   0        0        0      597 2023-05-27 15:36:07.575552 gamium-0.0.1/gamium/protocol/functions.py
--rw-r--r--   0        0        0     1988 2023-05-24 06:56:59.780237 gamium-0.0.1/gamium/protocol/generated/Packets/ActionParam.py
--rw-r--r--   0        0        0     4353 2023-05-24 06:56:59.778280 gamium-0.0.1/gamium/protocol/generated/Packets/ActionParamSingle.py
--rw-r--r--   0        0        0     2917 2023-05-24 06:56:59.787464 gamium-0.0.1/gamium/protocol/generated/Packets/ActionResult.py
--rw-r--r--   0        0        0     2909 2023-05-24 06:56:59.781650 gamium-0.0.1/gamium/protocol/generated/Packets/Actions/AppQuitParam.py
--rw-r--r--   0        0        0     4175 2023-05-24 06:56:59.782913 gamium-0.0.1/gamium/protocol/generated/Packets/Actions/InputKeyParam.py
--rw-r--r--   0        0        0     5031 2023-05-24 06:56:59.782321 gamium-0.0.1/gamium/protocol/generated/Packets/Actions/InputMouseParam.py
--rw-r--r--   0        0        0     3357 2023-05-24 06:56:59.783213 gamium-0.0.1/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py
--rw-r--r--   0        0        0      156 2023-05-24 06:56:59.783916 gamium-0.0.1/gamium/protocol/generated/Packets/Actions/MovePlayerBy.py
--rw-r--r--   0        0        0     6404 2023-05-24 06:56:59.783443 gamium-0.0.1/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py
--rw-r--r--   0        0        0     2213 2023-05-24 06:56:59.783639 gamium-0.0.1/gamium/protocol/generated/Packets/Actions/SleepParam.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.782546 gamium-0.0.1/gamium/protocol/generated/Packets/Actions/__init__.py
--rw-r--r--   0        0        0     3665 2023-05-24 06:56:59.776569 gamium-0.0.1/gamium/protocol/generated/Packets/ActionsParam.py
--rw-r--r--   0        0        0     4251 2023-05-24 06:56:59.772285 gamium-0.0.1/gamium/protocol/generated/Packets/ActionsResult.py
--rw-r--r--   0        0        0     3323 2023-05-24 06:56:59.786993 gamium-0.0.1/gamium/protocol/generated/Packets/ChangeConfigurationParam.py
--rw-r--r--   0        0        0     2116 2023-05-24 06:56:59.771624 gamium-0.0.1/gamium/protocol/generated/Packets/ChangeConfigurationResult.py
--rw-r--r--   0        0        0     3503 2023-05-24 06:56:59.785128 gamium-0.0.1/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py
--rw-r--r--   0        0        0     4913 2023-05-24 06:56:59.786343 gamium-0.0.1/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py
--rw-r--r--   0        0        0     2799 2023-05-24 06:56:59.773129 gamium-0.0.1/gamium/protocol/generated/Packets/Env.py
--rw-r--r--   0        0        0     6064 2023-05-24 06:56:59.776810 gamium-0.0.1/gamium/protocol/generated/Packets/ExecuteRpcParam.py
--rw-r--r--   0        0        0     2634 2023-05-24 06:56:59.771993 gamium-0.0.1/gamium/protocol/generated/Packets/ExecuteRpcResult.py
--rw-r--r--   0        0        0     3093 2023-05-24 06:56:59.774604 gamium-0.0.1/gamium/protocol/generated/Packets/FindObjectsParam.py
--rw-r--r--   0        0        0     4307 2023-05-24 06:56:59.775272 gamium-0.0.1/gamium/protocol/generated/Packets/FindObjectsResult.py
--rw-r--r--   0        0        0     2437 2023-05-24 06:56:59.785762 gamium-0.0.1/gamium/protocol/generated/Packets/HelloParam.py
--rw-r--r--   0        0        0     8271 2023-05-24 06:56:59.786610 gamium-0.0.1/gamium/protocol/generated/Packets/HelloResult.py
--rw-r--r--   0        0        0     4330 2023-05-24 06:56:59.781201 gamium-0.0.1/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py
--rw-r--r--   0        0        0     5826 2023-05-24 06:56:59.777393 gamium-0.0.1/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py
--rw-r--r--   0        0        0     2874 2023-05-24 06:56:59.774317 gamium-0.0.1/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py
--rw-r--r--   0        0        0     3294 2023-05-24 06:56:59.772556 gamium-0.0.1/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py
--rw-r--r--   0        0        0     4413 2023-05-24 06:56:59.780925 gamium-0.0.1/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py
--rw-r--r--   0        0        0     2950 2023-05-24 06:56:59.786116 gamium-0.0.1/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py
--rw-r--r--   0        0        0     1916 2023-05-24 06:56:59.774074 gamium-0.0.1/gamium/protocol/generated/Packets/QueryProfileParam.py
--rw-r--r--   0        0        0     2466 2023-05-24 06:56:59.773381 gamium-0.0.1/gamium/protocol/generated/Packets/QueryProfileResult.py
--rw-r--r--   0        0        0     1891 2023-05-24 06:56:59.779376 gamium-0.0.1/gamium/protocol/generated/Packets/QueryScreenParam.py
--rw-r--r--   0        0        0     3030 2023-05-24 06:56:59.787227 gamium-0.0.1/gamium/protocol/generated/Packets/QueryScreenResult.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.775993 gamium-0.0.1/gamium/protocol/generated/Packets/__init__.py
--rw-r--r--   0        0        0     3468 2023-05-24 06:56:59.766267 gamium-0.0.1/gamium/protocol/generated/Param.py
--rw-r--r--   0        0        0     5120 2023-05-24 06:56:59.765275 gamium-0.0.1/gamium/protocol/generated/Request.py
--rw-r--r--   0        0        0     6299 2023-05-24 06:56:59.768250 gamium-0.0.1/gamium/protocol/generated/Response.py
--rw-r--r--   0        0        0     3536 2023-05-24 06:56:59.770804 gamium-0.0.1/gamium/protocol/generated/Result.py
--rw-r--r--   0        0        0     3222 2023-05-24 06:56:59.755793 gamium-0.0.1/gamium/protocol/generated/Types/Configuration.py
--rw-r--r--   0        0        0     1146 2023-05-24 06:56:59.764593 gamium-0.0.1/gamium/protocol/generated/Types/ErrorCode.py
--rw-r--r--   0        0        0     2962 2023-05-24 06:56:59.756771 gamium-0.0.1/gamium/protocol/generated/Types/ErrorResult.py
--rw-r--r--   0        0        0      164 2023-05-24 06:56:59.764892 gamium-0.0.1/gamium/protocol/generated/Types/ExecuteRpcBy.py
--rw-r--r--   0        0        0      161 2023-05-24 06:56:59.761605 gamium-0.0.1/gamium/protocol/generated/Types/InputKeyBy.py
--rw-r--r--   0        0        0      147 2023-05-24 06:56:59.762868 gamium-0.0.1/gamium/protocol/generated/Types/InputKeyPressType.py
--rw-r--r--   0        0        0      168 2023-05-24 06:56:59.760225 gamium-0.0.1/gamium/protocol/generated/Types/InputMouseButtonCode.py
--rw-r--r--   0        0        0      177 2023-05-24 06:56:59.757942 gamium-0.0.1/gamium/protocol/generated/Types/InputMousePressType.py
--rw-r--r--   0        0        0     5920 2023-05-24 06:56:59.762417 gamium-0.0.1/gamium/protocol/generated/Types/ObjectHierarchyNode.py
--rw-r--r--   0        0        0    10803 2023-05-24 06:56:59.759371 gamium-0.0.1/gamium/protocol/generated/Types/ObjectInfo.py
--rw-r--r--   0        0        0     2955 2023-05-24 06:56:59.760908 gamium-0.0.1/gamium/protocol/generated/Types/ObjectLocator.py
--rw-r--r--   0        0        0      146 2023-05-24 06:56:59.763178 gamium-0.0.1/gamium/protocol/generated/Types/ObjectLocatorBy.py
--rw-r--r--   0        0        0      158 2023-05-24 06:56:59.756438 gamium-0.0.1/gamium/protocol/generated/Types/ObjectType.py
--rw-r--r--   0        0        0     5147 2023-05-24 06:56:59.755545 gamium-0.0.1/gamium/protocol/generated/Types/ObjectsHierarchy.py
--rw-r--r--   0        0        0     7471 2023-05-24 06:56:59.754685 gamium-0.0.1/gamium/protocol/generated/Types/Unity/UnityKeyCode.py
--rw-r--r--   0        0        0     1944 2023-05-24 06:56:59.755240 gamium-0.0.1/gamium/protocol/generated/Types/Unity/UnityKeyboard.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.754971 gamium-0.0.1/gamium/protocol/generated/Types/Unity/__init__.py
--rw-r--r--   0        0        0     1681 2023-05-24 06:56:59.757019 gamium-0.0.1/gamium/protocol/generated/Types/Vector2.py
--rw-r--r--   0        0        0     1947 2023-05-24 06:56:59.757558 gamium-0.0.1/gamium/protocol/generated/Types/Vector3.py
--rw-r--r--   0        0        0     2212 2023-05-24 06:56:59.758210 gamium-0.0.1/gamium/protocol/generated/Types/Vector4.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.757234 gamium-0.0.1/gamium/protocol/generated/Types/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 06:56:59.766005 gamium-0.0.1/gamium/protocol/generated/__init__.py
--rw-r--r--   0        0        0     3296 2023-05-29 05:36:44.760410 gamium-0.0.1/gamium/protocol/types.py
--rw-r--r--   0        0        0     3887 2023-05-27 16:45:21.559031 gamium-0.0.1/gamium/ui/ui.py
--rw-r--r--   0        0        0       80 2023-05-27 15:33:39.715322 gamium-0.0.1/gamium/utils/generics.py
--rw-r--r--   0        0        0       79 2023-05-24 13:28:31.670844 gamium-0.0.1/gamium/utils/time.py
--rw-r--r--   0        0        0      598 2023-05-27 16:56:44.654557 gamium-0.0.1/gamium/utils/try_utils.py
--rw-r--r--   0        0        0     1873 2023-05-27 17:12:44.836551 gamium-0.0.1/gamium/utils/wait.py
--rw-r--r--   0        0        0      278 2023-05-23 05:41:36.500085 gamium-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 gamium-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1007 2023-05-30 02:32:02.321529 gamium-0.0.2/README.md
+-rw-r--r--   0        0        0      626 2023-05-25 07:46:40.594452 gamium-0.0.2/gamium/__init__.py
+-rw-r--r--   0        0        0      500 2023-05-24 13:45:20.085940 gamium-0.0.2/gamium/__main__.py
+-rw-r--r--   0        0        0    11229 2023-05-27 16:29:57.716876 gamium-0.0.2/gamium/actions/action_chain.py
+-rw-r--r--   0        0        0     1449 2023-05-27 15:57:54.253933 gamium-0.0.2/gamium/actions/key_by.py
+-rw-r--r--   0        0        0      471 2023-05-27 16:37:25.765448 gamium-0.0.2/gamium/condition/condition.py
+-rw-r--r--   0        0        0     2138 2023-05-27 17:05:44.381885 gamium-0.0.2/gamium/condition/until.py
+-rw-r--r--   0        0        0      245 2023-05-27 15:36:03.742756 gamium-0.0.2/gamium/condition/wait_condition.py
+-rw-r--r--   0        0        0      269 2023-05-28 09:47:38.321943 gamium-0.0.2/gamium/errors/gamium_error.py
+-rw-r--r--   0        0        0     6303 2023-05-27 16:57:16.462228 gamium-0.0.2/gamium/gamium_client.py
+-rw-r--r--   0        0        0     8498 2023-05-27 16:29:22.380147 gamium-0.0.2/gamium/gamium_service.py
+-rw-r--r--   0        0        0     1248 2023-05-27 16:48:14.859904 gamium-0.0.2/gamium/igamium_client.py
+-rw-r--r--   0        0        0       62 2023-05-20 09:32:59.575340 gamium-0.0.2/gamium/internal/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-20 09:32:59.575844 gamium-0.0.2/gamium/internal/logger.py
+-rw-r--r--   0        0        0      672 2023-05-24 10:00:22.753241 gamium-0.0.2/gamium/internal/size_prefixed_recv_queue.py
+-rw-r--r--   0        0        0      349 2023-05-27 15:45:16.895951 gamium-0.0.2/gamium/locator/by.py
+-rw-r--r--   0        0        0       59 2023-05-20 09:32:59.576661 gamium-0.0.2/gamium/locator/locator.py
+-rw-r--r--   0        0        0      906 2023-05-27 15:44:54.654718 gamium-0.0.2/gamium/locator/rpc_by.py
+-rw-r--r--   0        0        0       47 2023-05-22 13:59:37.380671 gamium-0.0.2/gamium/locator/rpc_locator.py
+-rw-r--r--   0        0        0     1996 2023-05-27 16:48:30.437448 gamium-0.0.2/gamium/object/player.py
+-rw-r--r--   0        0        0     3925 2023-05-27 16:48:34.013675 gamium-0.0.2/gamium/object/ui_element.py
+-rw-r--r--   0        0        0      390 2023-05-23 10:45:11.917741 gamium-0.0.2/gamium/options/__init__.py
+-rw-r--r--   0        0        0      142 2023-05-27 16:07:06.395341 gamium-0.0.2/gamium/options/action_click_options.py
+-rw-r--r--   0        0        0      204 2023-05-27 16:19:40.425215 gamium-0.0.2/gamium/options/action_drag_options.py
+-rw-r--r--   0        0        0       92 2023-05-24 12:03:15.929711 gamium-0.0.2/gamium/options/action_move_options.py
+-rw-r--r--   0        0        0      144 2023-05-27 16:20:01.758848 gamium-0.0.2/gamium/options/action_scroll_options.py
+-rw-r--r--   0        0        0      171 2023-05-27 16:20:08.327138 gamium-0.0.2/gamium/options/execute_rpc_options.py
+-rw-r--r--   0        0        0      132 2023-05-27 16:20:12.178882 gamium-0.0.2/gamium/options/find_objects_options.py
+-rw-r--r--   0        0        0      374 2023-05-27 16:20:21.453410 gamium-0.0.2/gamium/options/move_player_options.py
+-rw-r--r--   0        0        0      262 2023-05-27 16:20:28.044046 gamium-0.0.2/gamium/options/query_object_interactable_options.py
+-rw-r--r--   0        0        0      139 2023-05-27 16:20:31.256151 gamium-0.0.2/gamium/options/send_key_options.py
+-rw-r--r--   0        0        0       89 2023-05-22 09:57:37.806139 gamium-0.0.2/gamium/options/set_text_options.py
+-rw-r--r--   0        0        0      362 2023-05-27 16:20:41.882990 gamium-0.0.2/gamium/options/wait_options.py
+-rw-r--r--   0        0        0        0 2023-05-24 06:56:59.787754 gamium-0.0.2/gamium/protocol/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-27 15:36:07.575552 gamium-0.0.2/gamium/protocol/functions.py
+-rw-r--r--   0        0        0     1988 2023-05-24 06:56:59.780237 gamium-0.0.2/gamium/protocol/generated/Packets/ActionParam.py
+-rw-r--r--   0        0        0     4353 2023-05-24 06:56:59.778280 gamium-0.0.2/gamium/protocol/generated/Packets/ActionParamSingle.py
+-rw-r--r--   0        0        0     2917 2023-05-24 06:56:59.787464 gamium-0.0.2/gamium/protocol/generated/Packets/ActionResult.py
+-rw-r--r--   0        0        0     2909 2023-05-24 06:56:59.781650 gamium-0.0.2/gamium/protocol/generated/Packets/Actions/AppQuitParam.py
+-rw-r--r--   0        0        0     4175 2023-05-24 06:56:59.782913 gamium-0.0.2/gamium/protocol/generated/Packets/Actions/InputKeyParam.py
+-rw-r--r--   0        0        0     5031 2023-05-24 06:56:59.782321 gamium-0.0.2/gamium/protocol/generated/Packets/Actions/InputMouseParam.py
+-rw-r--r--   0        0        0     3357 2023-05-24 06:56:59.783213 gamium-0.0.2/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py
+-rw-r--r--   0        0        0      156 2023-05-24 06:56:59.783916 gamium-0.0.2/gamium/protocol/generated/Packets/Actions/MovePlayerBy.py
+-rw-r--r--   0        0        0     6404 2023-05-24 06:56:59.783443 gamium-0.0.2/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py
+-rw-r--r--   0        0        0     2213 2023-05-24 06:56:59.783639 gamium-0.0.2/gamium/protocol/generated/Packets/Actions/SleepParam.py
+-rw-r--r--   0        0        0        0 2023-05-24 06:56:59.782546 gamium-0.0.2/gamium/protocol/generated/Packets/Actions/__init__.py
+-rw-r--r--   0        0        0     3665 2023-05-24 06:56:59.776569 gamium-0.0.2/gamium/protocol/generated/Packets/ActionsParam.py
+-rw-r--r--   0        0        0     4251 2023-05-24 06:56:59.772285 gamium-0.0.2/gamium/protocol/generated/Packets/ActionsResult.py
+-rw-r--r--   0        0        0     3323 2023-05-24 06:56:59.786993 gamium-0.0.2/gamium/protocol/generated/Packets/ChangeConfigurationParam.py
+-rw-r--r--   0        0        0     2116 2023-05-24 06:56:59.771624 gamium-0.0.2/gamium/protocol/generated/Packets/ChangeConfigurationResult.py
+-rw-r--r--   0        0        0     3503 2023-05-24 06:56:59.785128 gamium-0.0.2/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py
+-rw-r--r--   0        0        0     4913 2023-05-24 06:56:59.786343 gamium-0.0.2/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py
+-rw-r--r--   0        0        0     2799 2023-05-24 06:56:59.773129 gamium-0.0.2/gamium/protocol/generated/Packets/Env.py
+-rw-r--r--   0        0        0     6064 2023-05-24 06:56:59.776810 gamium-0.0.2/gamium/protocol/generated/Packets/ExecuteRpcParam.py
+-rw-r--r--   0        0        0     2634 2023-05-24 06:56:59.771993 gamium-0.0.2/gamium/protocol/generated/Packets/ExecuteRpcResult.py
+-rw-r--r--   0        0        0     3093 2023-05-24 06:56:59.774604 gamium-0.0.2/gamium/protocol/generated/Packets/FindObjectsParam.py
+-rw-r--r--   0        0        0     4307 2023-05-24 06:56:59.775272 gamium-0.0.2/gamium/protocol/generated/Packets/FindObjectsResult.py
+-rw-r--r--   0        0        0     2437 2023-05-24 06:56:59.785762 gamium-0.0.2/gamium/protocol/generated/Packets/HelloParam.py
+-rw-r--r--   0        0        0     8271 2023-05-24 06:56:59.786610 gamium-0.0.2/gamium/protocol/generated/Packets/HelloResult.py
+-rw-r--r--   0        0        0     4330 2023-05-24 06:56:59.781201 gamium-0.0.2/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py
+-rw-r--r--   0        0        0     5826 2023-05-24 06:56:59.777393 gamium-0.0.2/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py
+-rw-r--r--   0        0        0     2874 2023-05-24 06:56:59.774317 gamium-0.0.2/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py
+-rw-r--r--   0        0        0     3294 2023-05-24 06:56:59.772556 gamium-0.0.2/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py
+-rw-r--r--   0        0        0     4413 2023-05-24 06:56:59.780925 gamium-0.0.2/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py
+-rw-r--r--   0        0        0     2950 2023-05-24 06:56:59.786116 gamium-0.0.2/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py
+-rw-r--r--   0        0        0     1916 2023-05-24 06:56:59.774074 gamium-0.0.2/gamium/protocol/generated/Packets/QueryProfileParam.py
+-rw-r--r--   0        0        0     2466 2023-05-24 06:56:59.773381 gamium-0.0.2/gamium/protocol/generated/Packets/QueryProfileResult.py
+-rw-r--r--   0        0        0     1891 2023-05-24 06:56:59.779376 gamium-0.0.2/gamium/protocol/generated/Packets/QueryScreenParam.py
+-rw-r--r--   0        0        0     3030 2023-05-24 06:56:59.787227 gamium-0.0.2/gamium/protocol/generated/Packets/QueryScreenResult.py
+-rw-r--r--   0        0        0        0 2023-05-24 06:56:59.775993 gamium-0.0.2/gamium/protocol/generated/Packets/__init__.py
+-rw-r--r--   0        0        0     3468 2023-05-24 06:56:59.766267 gamium-0.0.2/gamium/protocol/generated/Param.py
+-rw-r--r--   0        0        0     5120 2023-05-24 06:56:59.765275 gamium-0.0.2/gamium/protocol/generated/Request.py
+-rw-r--r--   0        0        0     6299 2023-05-24 06:56:59.768250 gamium-0.0.2/gamium/protocol/generated/Response.py
+-rw-r--r--   0        0        0     3536 2023-05-24 06:56:59.770804 gamium-0.0.2/gamium/protocol/generated/Result.py
+-rw-r--r--   0        0        0     3222 2023-05-24 06:56:59.755793 gamium-0.0.2/gamium/protocol/generated/Types/Configuration.py
+-rw-r--r--   0        0        0     1146 2023-05-24 06:56:59.764593 gamium-0.0.2/gamium/protocol/generated/Types/ErrorCode.py
+-rw-r--r--   0        0        0     2962 2023-05-24 06:56:59.756771 gamium-0.0.2/gamium/protocol/generated/Types/ErrorResult.py
+-rw-r--r--   0        0        0      164 2023-05-24 06:56:59.764892 gamium-0.0.2/gamium/protocol/generated/Types/ExecuteRpcBy.py
+-rw-r--r--   0        0        0      161 2023-05-24 06:56:59.761605 gamium-0.0.2/gamium/protocol/generated/Types/InputKeyBy.py
+-rw-r--r--   0        0        0      147 2023-05-24 06:56:59.762868 gamium-0.0.2/gamium/protocol/generated/Types/InputKeyPressType.py
+-rw-r--r--   0        0        0      168 2023-05-24 06:56:59.760225 gamium-0.0.2/gamium/protocol/generated/Types/InputMouseButtonCode.py
+-rw-r--r--   0        0        0      177 2023-05-24 06:56:59.757942 gamium-0.0.2/gamium/protocol/generated/Types/InputMousePressType.py
+-rw-r--r--   0        0        0     5920 2023-05-24 06:56:59.762417 gamium-0.0.2/gamium/protocol/generated/Types/ObjectHierarchyNode.py
+-rw-r--r--   0        0        0    10803 2023-05-24 06:56:59.759371 gamium-0.0.2/gamium/protocol/generated/Types/ObjectInfo.py
+-rw-r--r--   0        0        0     2955 2023-05-24 06:56:59.760908 gamium-0.0.2/gamium/protocol/generated/Types/ObjectLocator.py
+-rw-r--r--   0        0        0      146 2023-05-24 06:56:59.763178 gamium-0.0.2/gamium/protocol/generated/Types/ObjectLocatorBy.py
+-rw-r--r--   0        0        0      158 2023-05-24 06:56:59.756438 gamium-0.0.2/gamium/protocol/generated/Types/ObjectType.py
+-rw-r--r--   0        0        0     5147 2023-05-24 06:56:59.755545 gamium-0.0.2/gamium/protocol/generated/Types/ObjectsHierarchy.py
+-rw-r--r--   0        0        0     7471 2023-05-24 06:56:59.754685 gamium-0.0.2/gamium/protocol/generated/Types/Unity/UnityKeyCode.py
+-rw-r--r--   0        0        0     1944 2023-05-24 06:56:59.755240 gamium-0.0.2/gamium/protocol/generated/Types/Unity/UnityKeyboard.py
+-rw-r--r--   0        0        0        0 2023-05-24 06:56:59.754971 gamium-0.0.2/gamium/protocol/generated/Types/Unity/__init__.py
+-rw-r--r--   0        0        0     1681 2023-05-24 06:56:59.757019 gamium-0.0.2/gamium/protocol/generated/Types/Vector2.py
+-rw-r--r--   0        0        0     1947 2023-05-24 06:56:59.757558 gamium-0.0.2/gamium/protocol/generated/Types/Vector3.py
+-rw-r--r--   0        0        0     2212 2023-05-24 06:56:59.758210 gamium-0.0.2/gamium/protocol/generated/Types/Vector4.py
+-rw-r--r--   0        0        0        0 2023-05-24 06:56:59.757234 gamium-0.0.2/gamium/protocol/generated/Types/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 06:56:59.766005 gamium-0.0.2/gamium/protocol/generated/__init__.py
+-rw-r--r--   0        0        0     3296 2023-05-29 05:36:44.760410 gamium-0.0.2/gamium/protocol/types.py
+-rw-r--r--   0        0        0     3887 2023-05-27 16:45:21.559031 gamium-0.0.2/gamium/ui/ui.py
+-rw-r--r--   0        0        0       80 2023-05-27 15:33:39.715322 gamium-0.0.2/gamium/utils/generics.py
+-rw-r--r--   0        0        0       79 2023-05-24 13:28:31.670844 gamium-0.0.2/gamium/utils/time.py
+-rw-r--r--   0        0        0      598 2023-05-27 16:56:44.654557 gamium-0.0.2/gamium/utils/try_utils.py
+-rw-r--r--   0        0        0     1873 2023-05-27 17:12:44.836551 gamium-0.0.2/gamium/utils/wait.py
+-rw-r--r--   0        0        0      278 2023-05-30 02:32:13.413895 gamium-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 gamium-0.0.2/PKG-INFO
```

### Comparing `gamium-0.0.1/gamium/__init__.py` & `gamium-0.0.2/gamium/__init__.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/actions/action_chain.py` & `gamium-0.0.2/gamium/actions/action_chain.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/actions/key_by.py` & `gamium-0.0.2/gamium/actions/key_by.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/condition/until.py` & `gamium-0.0.2/gamium/condition/until.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/gamium_client.py` & `gamium-0.0.2/gamium/gamium_client.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/gamium_service.py` & `gamium-0.0.2/gamium/gamium_service.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/igamium_client.py` & `gamium-0.0.2/gamium/igamium_client.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/internal/logger.py` & `gamium-0.0.2/gamium/internal/logger.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/internal/size_prefixed_recv_queue.py` & `gamium-0.0.2/gamium/internal/size_prefixed_recv_queue.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/locator/rpc_by.py` & `gamium-0.0.2/gamium/locator/rpc_by.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/object/player.py` & `gamium-0.0.2/gamium/object/player.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/object/ui_element.py` & `gamium-0.0.2/gamium/object/ui_element.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/functions.py` & `gamium-0.0.2/gamium/protocol/functions.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/ActionParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/ActionParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/ActionParamSingle.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/ActionParamSingle.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/ActionResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/ActionResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/Actions/AppQuitParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/Actions/AppQuitParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/Actions/InputKeyParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/Actions/InputKeyParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/Actions/InputMouseParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/Actions/InputMouseParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/Actions/InputSetTextParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/Actions/MovePlayerParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/Actions/SleepParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/Actions/SleepParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/ActionsParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/ActionsParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/ActionsResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/ActionsResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/ChangeConfigurationParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/ChangeConfigurationParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/ChangeConfigurationResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/ChangeConfigurationResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/DumpObjectsHierarchyParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/DumpObjectsHierarchyResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/Env.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/Env.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/ExecuteRpcParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/ExecuteRpcParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/ExecuteRpcResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/ExecuteRpcResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/FindObjectsParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/FindObjectsParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/FindObjectsResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/FindObjectsResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/HelloParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/HelloParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/HelloResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/HelloResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/InspectObjectOnScreenParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/InspectObjectOnScreenResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/InspectObjectWithIdParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/InspectObjectWithIdResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/QueryObjectInteractableParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/QueryObjectInteractableResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/QueryProfileParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/QueryProfileParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/QueryProfileResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/QueryProfileResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/QueryScreenParam.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/QueryScreenParam.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Packets/QueryScreenResult.py` & `gamium-0.0.2/gamium/protocol/generated/Packets/QueryScreenResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Param.py` & `gamium-0.0.2/gamium/protocol/generated/Param.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Request.py` & `gamium-0.0.2/gamium/protocol/generated/Request.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Response.py` & `gamium-0.0.2/gamium/protocol/generated/Response.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Result.py` & `gamium-0.0.2/gamium/protocol/generated/Result.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/Configuration.py` & `gamium-0.0.2/gamium/protocol/generated/Types/Configuration.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/ErrorCode.py` & `gamium-0.0.2/gamium/protocol/generated/Types/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/ErrorResult.py` & `gamium-0.0.2/gamium/protocol/generated/Types/ErrorResult.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/ObjectHierarchyNode.py` & `gamium-0.0.2/gamium/protocol/generated/Types/ObjectHierarchyNode.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/ObjectInfo.py` & `gamium-0.0.2/gamium/protocol/generated/Types/ObjectInfo.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/ObjectLocator.py` & `gamium-0.0.2/gamium/protocol/generated/Types/ObjectLocator.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/ObjectsHierarchy.py` & `gamium-0.0.2/gamium/protocol/generated/Types/ObjectsHierarchy.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/Unity/UnityKeyCode.py` & `gamium-0.0.2/gamium/protocol/generated/Types/Unity/UnityKeyCode.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/Unity/UnityKeyboard.py` & `gamium-0.0.2/gamium/protocol/generated/Types/Unity/UnityKeyboard.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/Vector2.py` & `gamium-0.0.2/gamium/protocol/generated/Types/Vector2.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/Vector3.py` & `gamium-0.0.2/gamium/protocol/generated/Types/Vector3.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/generated/Types/Vector4.py` & `gamium-0.0.2/gamium/protocol/generated/Types/Vector4.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/protocol/types.py` & `gamium-0.0.2/gamium/protocol/types.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/ui/ui.py` & `gamium-0.0.2/gamium/ui/ui.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/utils/try_utils.py` & `gamium-0.0.2/gamium/utils/try_utils.py`

 * *Files identical despite different names*

### Comparing `gamium-0.0.1/gamium/utils/wait.py` & `gamium-0.0.2/gamium/utils/wait.py`

 * *Files identical despite different names*

