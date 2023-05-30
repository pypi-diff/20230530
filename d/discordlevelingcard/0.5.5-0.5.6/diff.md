# Comparing `tmp/discordlevelingcard-0.5.5.tar.gz` & `tmp/discordlevelingcard-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordlevelingcard-0.5.5.tar", max compression
+gzip compressed data, was "discordlevelingcard-0.5.6.tar", max compression
```

## Comparing `discordlevelingcard-0.5.5.tar` & `discordlevelingcard-0.5.6.tar`

### file list

```diff
@@ -1,20 +1,17 @@
--rw-r--r--   0        0        0      129 2023-05-29 17:20:09.194905 discordlevelingcard-0.5.5/DiscordLevelingCard/__init__.py
--rw-r--r--   0        0        0      842 2023-04-25 08:29:49.129344 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/curveborder.png
--rw-r--r--   0        0        0     2596 2023-04-25 08:29:49.129826 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/curvedoverlay.png
--rw-r--r--   0        0        0    60288 2023-04-25 08:29:49.131350 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/levelfont.otf
--rw-r--r--   0        0        0     9742 2023-04-25 08:29:49.132354 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/mask_circle.jpg
--rw-r--r--   0        0        0     4775 2023-05-29 17:05:04.175407 discordlevelingcard-0.5.5/DiscordLevelingCard/assets/overlay1.png
--rw-r--r--   0        0        0     2590 2023-04-25 08:29:49.133788 discordlevelingcard-0.5.5/DiscordLevelingCard/card_settings.py
--rw-r--r--   0        0        0    12505 2023-05-29 17:39:37.772268 discordlevelingcard-0.5.5/DiscordLevelingCard/discord_card.py
--rw-r--r--   0        0        0      531 2023-04-25 08:29:49.134664 discordlevelingcard-0.5.5/DiscordLevelingCard/error.py
--rw-r--r--   0        0        0     7459 2023-05-29 17:17:30.123452 discordlevelingcard-0.5.5/DiscordLevelingCard/sandbox.py
--rw-r--r--   0        0        0     6247 2023-05-29 17:54:43.984970 discordlevelingcard-0.5.5/DiscordLevelingCard/tester.py
--rw-r--r--   0        0        0   124130 2023-05-29 17:13:57.444261 discordlevelingcard-0.5.5/Examples/custom card examples/black_card1.png
--rw-r--r--   0        0        0   125492 2023-05-29 17:15:51.029764 discordlevelingcard-0.5.5/Examples/custom card examples/blue_card1.png
--rw-r--r--   0        0        0   125447 2023-05-29 17:15:25.624219 discordlevelingcard-0.5.5/Examples/custom card examples/white_card1.png
--rw-r--r--   0        0        0     1511 2023-05-29 17:56:46.850193 discordlevelingcard-0.5.5/Examples/tester_example.py
--rw-r--r--   0        0        0     1083 2023-04-25 08:29:49.135173 discordlevelingcard-0.5.5/LICENSE
--rw-r--r--   0        0        0      943 2023-05-29 18:37:53.626251 discordlevelingcard-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     6686 2023-05-29 18:40:04.718748 discordlevelingcard-0.5.5/README.md
--rw-r--r--   0        0        0     7488 2023-05-29 18:40:59.176058 discordlevelingcard-0.5.5/setup.py
--rw-r--r--   0        0        0     7348 2023-05-29 18:40:59.176058 discordlevelingcard-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      129 2023-05-29 17:20:09.194905 discordlevelingcard-0.5.6/DiscordLevelingCard/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-25 08:29:49.129344 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/curveborder.png
+-rw-r--r--   0        0        0     2596 2023-04-25 08:29:49.129826 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/curvedoverlay.png
+-rw-r--r--   0        0        0    60288 2023-04-25 08:29:49.131350 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/levelfont.otf
+-rw-r--r--   0        0        0     9742 2023-04-25 08:29:49.132354 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/mask_circle.jpg
+-rw-r--r--   0        0        0     3024 2023-05-30 11:34:28.727698 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/mask_hexagon.png
+-rw-r--r--   0        0        0     4775 2023-05-29 17:05:04.175407 discordlevelingcard-0.5.6/DiscordLevelingCard/assets/overlay1.png
+-rw-r--r--   0        0        0     2590 2023-04-25 08:29:49.133788 discordlevelingcard-0.5.6/DiscordLevelingCard/card_settings.py
+-rw-r--r--   0        0        0    12505 2023-05-29 17:39:37.772268 discordlevelingcard-0.5.6/DiscordLevelingCard/discord_card.py
+-rw-r--r--   0        0        0      531 2023-04-25 08:29:49.134664 discordlevelingcard-0.5.6/DiscordLevelingCard/error.py
+-rw-r--r--   0        0        0    13919 2023-05-30 18:51:58.560733 discordlevelingcard-0.5.6/DiscordLevelingCard/sandbox.py
+-rw-r--r--   0        0        0    10446 2023-05-30 17:34:42.418755 discordlevelingcard-0.5.6/DiscordLevelingCard/tester.py
+-rw-r--r--   0        0        0     1083 2023-04-25 08:29:49.135173 discordlevelingcard-0.5.6/LICENSE
+-rw-r--r--   0        0        0      929 2023-05-30 18:28:32.085735 discordlevelingcard-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     8785 2023-05-30 18:57:13.411441 discordlevelingcard-0.5.6/README.md
+-rw-r--r--   0        0        0     9587 2023-05-30 19:01:35.151432 discordlevelingcard-0.5.6/setup.py
+-rw-r--r--   0        0        0     9383 2023-05-30 19:01:35.151432 discordlevelingcard-0.5.6/PKG-INFO
```

### Comparing `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/curveborder.png` & `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/curveborder.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/curvedoverlay.png` & `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/curvedoverlay.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/levelfont.otf` & `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/levelfont.otf`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/mask_circle.jpg` & `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/mask_circle.jpg`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.5/DiscordLevelingCard/assets/overlay1.png` & `discordlevelingcard-0.5.6/DiscordLevelingCard/assets/overlay1.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.5/DiscordLevelingCard/card_settings.py` & `discordlevelingcard-0.5.6/DiscordLevelingCard/card_settings.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.5/DiscordLevelingCard/discord_card.py` & `discordlevelingcard-0.5.6/DiscordLevelingCard/discord_card.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.5/DiscordLevelingCard/error.py` & `discordlevelingcard-0.5.6/DiscordLevelingCard/error.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.5/LICENSE` & `discordlevelingcard-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.5/pyproject.toml` & `discordlevelingcard-0.5.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discordlevelingcard"
-version = "0.5.5"
+version = "0.5.6"
 readme = "README.md"
 description = "A library with leveling cards for your discord bot."
 repository = "https://github.com/krishsharma0413/DiscordLevelingCard"
 authors = ["Reset <krishsharma0413@gmail.com>"]
 license = "MIT"
 keywords = [
     "discord", "leveling", "card",
@@ -14,15 +14,15 @@
     "discord-leveling", "level-card",
     "discord-leveling-card", "discord-rank-card",
     "sandbox", "custom", "custom-card"
 ]
 packages = [
     { include = "DiscordLevelingCard"}
 ]
-include = ["DiscordLevelingCard/assets/*", "Examples/*"]
+include = ["DiscordLevelingCard/assets/*"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 aiohttp = "^3.8.1"
 Pillow = "^9.2.0"
 requests = "^2.28.1"
```

### Comparing `discordlevelingcard-0.5.5/README.md` & `discordlevelingcard-0.5.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -298,14 +298,78 @@
 
 ![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/black_card1.png)
 
 <br>
 
 </details>
 
+<details>
+
+<summary> <span style="color:yellow">custom_card3</span> method</summary>
+
+
+```py
+Sandbox.custom_card3(
+    resize:int = 100,
+
+    senstivity:int = 200,
+    card_colour: str = "black",
+
+    border_width: int = 25,
+    border_height: int = 25,
+    
+    avatar_frame: str = "curvedborder",
+    avatar_size: int = 260,
+    avatar_position: tuple = (53, 36),
+    
+    text_font: str = "levelfont.otf",
+
+    username_position: tuple = (330,130),
+    username_font_size: int = 50,
+
+    level_position: tuple = (500,40),
+    level_font_size: int = 50,
+
+    exp_position: tuple = (775,130),
+    exp_font_size: int = 50,
+
+)
+```
+
+## attribute
+- `resize` : resize the final image. (default is 100, treat it as a percentage.)
+- `senstivity` : senstivity of the avatar frame. (default is 200)
+- `card_colour` : color of the card. (default is black)
+- `border_width` : width of the border. (default is 25)
+- `border_height` : height of the border. (default is 25)
+- `avatar_frame` : avatar frame. (default is "curvedborder")
+- `avatar_size` : size of the avatar. (default is 260)
+- `avatar_position` : position of the avatar. (default is (53, 36))
+- `text_font` : font of the text. (default is "levelfont.otf")
+- `username_position` : position of the username. (default is (330,130))
+- `username_font_size` : font size of the username. (default is 50)
+- `level_position` : position of the level. (default is (500,40))
+- `level_font_size` : font size of the level. (default is 50)
+- `exp_position` : position of the exp. (default is (775,130))
+- `exp_font_size` : font size of the exp. (default is 50)
+
+## returns 
+- `bytes` which can directly be used within `discord.File` class.
+
+
+## examples
+
+![custom_card3](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20example-1.png)
+
+![custom_card3](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20unholy%20example-2.png)
+
+<br>
+
+</details>
+
 
 <br><br>
 
 if you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)
 
 <br><br>
 please star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D
```

### Comparing `discordlevelingcard-0.5.5/setup.py` & `discordlevelingcard-0.5.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'DiscordLevelingCard': ['assets/*']}
 
 install_requires = \
 ['Pillow>=9.2.0,<10.0.0', 'aiohttp>=3.8.1,<4.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'discordlevelingcard',
-    'version': '0.5.5',
+    'version': '0.5.6',
     'description': 'A library with leveling cards for your discord bot.',
-    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n<h3 style="color:yellow;"> now create your own custom rank cards!</h3>\n\n<br>\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n# card preview\n\n`card1`\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n\n`card2`\n![card2](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n\n`card3` *same as card2 but with background*\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n# installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n# How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n# Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n## methods\n\n- `card1`\n- `card2`\n- `card3`\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">Sandbox</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    cacheing:bool = True,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n- `cacheing` - if set to `True` then it will cache the image and will not regenerate it again. (default is `True`)\n  \n\n## methods\n- `custom_card1`\n  \n</details>\n\n\n\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">custom_card1</span> method</summary>\n\n\n```py\nSandbox.custom_card1(card_colour:str = "black", resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n- `card_colour` : color of the card. (default is black)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n## examples\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/blue_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/white_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/black_card1.png)\n\n<br>\n\n</details>\n\n\n<br><br>\n\nif you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
+    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n<h3 style="color:yellow;"> now create your own custom rank cards!</h3>\n\n<br>\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n# card preview\n\n`card1`\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n\n`card2`\n![card2](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n\n`card3` *same as card2 but with background*\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n# installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n# How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n# Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n## methods\n\n- `card1`\n- `card2`\n- `card3`\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">Sandbox</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    cacheing:bool = True,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n- `cacheing` - if set to `True` then it will cache the image and will not regenerate it again. (default is `True`)\n  \n\n## methods\n- `custom_card1`\n  \n</details>\n\n\n\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3(resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n\n## returns\n- `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">custom_card1</span> method</summary>\n\n\n```py\nSandbox.custom_card1(card_colour:str = "black", resize: int = 100)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n- `card_colour` : color of the card. (default is black)\n\n\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n## examples\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/blue_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/white_card1.png)\n\n![custom_card1](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/black_card1.png)\n\n<br>\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">custom_card3</span> method</summary>\n\n\n```py\nSandbox.custom_card3(\n    resize:int = 100,\n\n    senstivity:int = 200,\n    card_colour: str = "black",\n\n    border_width: int = 25,\n    border_height: int = 25,\n    \n    avatar_frame: str = "curvedborder",\n    avatar_size: int = 260,\n    avatar_position: tuple = (53, 36),\n    \n    text_font: str = "levelfont.otf",\n\n    username_position: tuple = (330,130),\n    username_font_size: int = 50,\n\n    level_position: tuple = (500,40),\n    level_font_size: int = 50,\n\n    exp_position: tuple = (775,130),\n    exp_font_size: int = 50,\n\n)\n```\n\n## attribute\n- `resize` : resize the final image. (default is 100, treat it as a percentage.)\n- `senstivity` : senstivity of the avatar frame. (default is 200)\n- `card_colour` : color of the card. (default is black)\n- `border_width` : width of the border. (default is 25)\n- `border_height` : height of the border. (default is 25)\n- `avatar_frame` : avatar frame. (default is "curvedborder")\n- `avatar_size` : size of the avatar. (default is 260)\n- `avatar_position` : position of the avatar. (default is (53, 36))\n- `text_font` : font of the text. (default is "levelfont.otf")\n- `username_position` : position of the username. (default is (330,130))\n- `username_font_size` : font size of the username. (default is 50)\n- `level_position` : position of the level. (default is (500,40))\n- `level_font_size` : font size of the level. (default is 50)\n- `exp_position` : position of the exp. (default is (775,130))\n- `exp_font_size` : font size of the exp. (default is 50)\n\n## returns \n- `bytes` which can directly be used within `discord.File` class.\n\n\n## examples\n\n![custom_card3](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20example-1.png)\n\n![custom_card3](https://raw.githubusercontent.com/krishsharma0413/DiscordLevelingCard/main/Examples/custom%20card%20examples/custom%20card3%20unholy%20example-2.png)\n\n<br>\n\n</details>\n\n\n<br><br>\n\nif you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
     'author': 'Reset',
     'author_email': 'krishsharma0413@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/krishsharma0413/DiscordLevelingCard',
     'packages': packages,
     'package_data': package_data,
```

