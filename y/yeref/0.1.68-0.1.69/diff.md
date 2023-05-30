# Comparing `tmp/yeref-0.1.68.tar.gz` & `tmp/yeref-0.1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.68.tar", last modified: Tue May 30 08:22:17 2023, max compression
+gzip compressed data, was "yeref-0.1.69.tar", last modified: Tue May 30 11:54:26 2023, max compression
```

## Comparing `yeref-0.1.68.tar` & `yeref-0.1.69.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 08:22:17.258000 yeref-0.1.68/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 08:22:17.258251 yeref-0.1.68/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-30 08:22:17.259239 yeref-0.1.68/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-30 08:22:03.000000 yeref-0.1.68/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 08:22:17.251550 yeref-0.1.68/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.68/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   489265 2023-05-29 15:12:40.000000 yeref-0.1.68/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   205872 2023-05-29 13:36:05.000000 yeref-0.1.68/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 08:22:17.257171 yeref-0.1.68/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 08:22:17.000000 yeref-0.1.68/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-30 08:22:17.000000 yeref-0.1.68/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-30 08:22:17.000000 yeref-0.1.68/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-30 08:22:17.000000 yeref-0.1.68/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 11:54:26.657080 yeref-0.1.69/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 11:54:26.657357 yeref-0.1.69/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-30 11:54:26.659049 yeref-0.1.69/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1372 2023-05-30 11:54:26.000000 yeref-0.1.69/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 11:54:26.646666 yeref-0.1.69/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.69/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   489276 2023-05-30 09:13:09.000000 yeref-0.1.69/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   205925 2023-05-30 11:53:26.000000 yeref-0.1.69/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 11:54:26.654743 yeref-0.1.69/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 11:54:26.000000 yeref-0.1.69/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-30 11:54:26.000000 yeref-0.1.69/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-30 11:54:26.000000 yeref-0.1.69/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-30 11:54:26.000000 yeref-0.1.69/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.68/setup.py` & `yeref-0.1.69/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.68',
+      version='0.1.69',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -38,14 +38,16 @@
 #
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
+# freey.sitner.ya
+# 
 
 # python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.66-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
```

### Comparing `yeref-0.1.68/yeref/l_.py` & `yeref-0.1.69/yeref/l_.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,23 +171,23 @@
     'ar': "💔 مثل",
 }
 # endregion
 
 
 # region post
 l_post_text = {
-    'ru': "✏️ 1. Напиши <b>текст</b> для нового поста (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'ru': "✏️ 1. <b>Введи текст</b> для нового поста (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 1. <b>Text</b> me for a new post (don&#x27;t forget to use <i>formatting</i> )\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 1. <b>Envíame un mensaje de texto</b> para una nueva publicación (no olvides usar <i>formato</i> )\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 1. <b>Envoyez</b> -moi un SMS pour un nouveau message (n&#x27;oubliez pas d&#x27;utiliser <i>le formatage</i> )\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 1.<b>发短信</b>给我（不要忘记使用<i>格式</i>）\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
     'ar': "✏️ 1. <b>أرسل</b> لي رسالة نصية لمنشور جديد (لا تنس استخدام <i>التنسيق</i> )\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_text_limit = {
-    'ru': "❗️ Количество <b>символов</b> текста (<i>включая форматирование</i>): <u>{0}</u> больше допустимых 1024",
+    'ru': "❗️ <b>Количество символов</b> текста (<i>включая форматирование</i>): <u>{0}</u> больше допустимых 1024",
     'en': "❗️ Number of <b>characters</b> of text ( <i>including formatting</i> ): <u>{0}</u> more than allowed 1024",
     'es': "❗️ Número de <b>caracteres</b> de texto ( <i>incluido el formato</i> ): <u>{0}</u> más de los permitidos 1024",
     'fr': "❗️ Nombre de <b>caractères</b> de texte ( <i>y compris le formatage</i> ) : <u>{0}</u> plus que autorisé 1024",
     'zh': "❗️ 文本<b>字符</b>数（<i>包括格式</i>）： <u>{0}</u>超过允许的 1024",
     'ar': "❗️ عدد <b>أحرف</b> النص ( <i>بما في ذلك التنسيق</i> ): <u>{0}</u> أكثر من العدد المسموح به وهو 1024",
 }
 l_post_text_empty = {
@@ -195,23 +195,23 @@
     'en': "❗️ post is empty, try again\n\n{0}",
     'es': "❗️ la publicación está vacía, inténtalo de nuevo\n\n{0}",
     'fr': "❗️ la publication est vide, réessayez\n\n{0}",
     'zh': "❗️ 帖子为空，请重试\n\n{0}",
     'ar': "❗️ المنشور فارغ ، حاول مرة أخرى\n\n{0}",
 }
 l_post_edit = {
-    'ru': "✏️ 1. Отправь измененный <b>текст</b> для текущего поста\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'ru': "✏️ 1. <b>Введи измененный текст</b> для текущего поста\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 1. Submit the modified <b>text</b> for the current post\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 1. Envíe el <b>texto</b> modificado para la publicación actual\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 1. Soumettez le <b>texte</b> modifié pour le message actuel\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 1.提交当前帖子的修改<b>文本</b>\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
     'ar': "✏️ 1. قم بإرسال <b>النص</b> المعدل للنشر الحالي\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_media = {
-    'ru': "✏️ 2. Прикрепи <b>медиа</b> контент: фото/гиф/видео/аудио/документ/стикер или запиши голосовое/видео-заметку в кружке\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'ru': "✏️ 2. <b>Прикрепи медиа</b> контент: фото/гиф/видео/аудио/документ/стикер или запиши голосовое/видео-заметку в кружке\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 2. Attach <b>media</b> content: photo/gif/video/audio/document/sticker or write a voice/video note in a circle\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 2. Adjunte contenido <b>multimedia</b> : foto/gif/video/audio/documento/pegatina o escriba una nota de voz/video en un círculo\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 2. Joignez du contenu <b>multimédia</b> : photo/gif/vidéo/audio/document/autocollant ou écrivez une note vocale/vidéo dans un cercle\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 2.附上<b>媒体</b>内容：照片/gif/视频/音频/文档/贴纸或在圈内写语音/视频备注\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
     'ar': "✏️ 2. أرفق محتوى <b>وسائط</b> : صورة / gif / فيديو / صوت / مستند / ملصق أو اكتب ملاحظة صوتية / فيديو في دائرة\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_media_wait = {
@@ -251,15 +251,15 @@
     'en': "☑️ No",
     'es': "☑️No",
     'fr': "☑️ Non",
     'zh': "☑️没有",
     'ar': "☑️ لا",
 }
 l_post_button = {
-    'ru': "✏️ 3. Отправь <b>названия</b> для кнопок и <b>ссылки</b> в формате (одну или несколько; кликни на образец ниже, чтобы скопировать):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ Интересно][💔 Не пиши]</code>\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'ru': "✏️ 3. <b>Введи названия</b> для кнопок и <b>ссылки</b> в формате (одну или несколько; кликни на образец ниже, чтобы скопировать):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ Интересно][💔 Не пиши]</code>\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 3. Submit button <b>names</b> and <b>links</b> in the format (one or more; click on the sample below to copy):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nor\n\n<code>[❤️ Nice][💔 Don't disturb]</code>\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 3. Envíe <b>nombres</b> de botones y <b>enlaces</b> en el formato (uno o más; haga clic en la muestra a continuación para copiar):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nor\n\n<code>[❤️ Nice][💔 Don't disturb]</code>\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 3. Soumettez <b>les noms</b> des boutons et <b>les liens</b> au format (un ou plusieurs ; cliquez sur l&#x27;exemple ci-dessous pour le copier) :\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nor\n\n<code>[❤️ Nice][💔 Don't disturb]</code>\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 3. 提交按钮<b>名称</b>和<b>链接</b>格式（一个或多个；点击下方示例复制）：\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nor\n\n<code>[❤️ Nice][💔 Don't disturb]</code>\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
     'ar': "✏️ 3. إرسال <b>أسماء</b> الأزرار <b>والروابط</b> بالتنسيق (واحد أو أكثر ؛ انقر فوق النموذج أدناه لنسخه):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\ ولا\n\n<code>[❤️ Nice][💔 Don't disturb]</code>\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_button_urlinvalid = {
@@ -275,15 +275,15 @@
     'en': "✏️ 3. Pin ( <b>pin</b> ) the message in the channel at the top of the screen: <code>да</code> | <code>нет</code> ?\n\n( <i>or press &quot;➡️️/Next&quot; to <u>not pin</u> the message</i> )",
     'es': "✏️ 3. Pin ( <b>pin</b> ) el mensaje en el canal en la parte superior de la pantalla: <code>да</code> | <code>нет</code> ?\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para <u>no fijar</u> el mensaje</i> )",
     'fr': "✏️ 3. Epingler ( <b>épingler</b> ) le message dans la chaîne en haut de l&#x27;écran : <code>да</code> | <code>нет</code> ?\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour <u>ne pas épingler</u> le message</i> )",
     'zh': "✏️ 3. 置顶（ <b>pin</b> ）屏幕上方频道中的消息： <code>да</code> | <code>нет</code> ？\n\n（<i>或按“➡️️/下一步”<u>不固定</u>消息</i>）",
     'ar': "✏️ 3. ثبّت ( <b>تثبيت</b> ) الرسالة في القناة أعلى الشاشة: <code>да</code> | <code>нет</code> ؟\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لعدم <u>تثبيت</u> الرسالة</i> )",
 }
 l_post_date = {
-    'ru': "✏️ 4. Выбери дату на календаре\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'ru': "✏️ 4. <b>Выбери дату</b> на календаре\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 4. Select a date on the calendar\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 4. Selecciona una fecha en el calendario\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 4. Sélectionnez une date sur le calendrier\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 4. 在日历上选择一个日期\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
     'ar': "✏️ 4. حدد تاريخًا في التقويم\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_finish = {
@@ -2232,39 +2232,39 @@
     'es': "🫥Tg bots",
     'fr': "🫥 Robots Tg",
     'zh': "🫥 Tg 机器人",
     'ar': "🫥 Tg bots",
 }
 
 l_find_chn_choose = {
-    'ru': "📰 Выбери <b>категорию</b> для выгрузки каналов",
+    'ru': "📰 <b>Выбери категорию</b> для выгрузки каналов",
     'en': "📰 Choose <b>a category</b> for uploading channels",
     'es': "📰 Elige <b>una categoría</b> para subir canales",
     'fr': "📰 Choisissez <b>une catégorie</b> pour télécharger des chaînes",
     'zh': "📰 选择上传频道的<b>类别</b>",
     'ar': "📰 اختر <b>فئة</b> لتحميل القنوات",
 }
 l_find_grp_choose = {
-    'ru': "📁 Выбери <b>категорию</b> для выгрузки групп",
+    'ru': "📁 <b>Выбери категорию</b> для выгрузки групп",
     'en': "📁 Choose <b>a category</b> for uploading groups",
     'es': "📁 Elige <b>una categoría</b> para subir grupos",
     'fr': "📁 Choisissez <b>une catégorie</b> pour télécharger des groupes",
     'zh': "📁 选择上传群组的<b>类别</b>",
     'ar': "📁 اختر <b>فئة</b> لتحميل المجموعات",
 }
 l_find_usr_choose = {
-    'ru': "🕵️ Выбери <b>категорию</b> для выгрузки пользователей",
+    'ru': "🕵️ <b>Выбери категорию</b> для выгрузки пользователей",
     'en': "🕵️ Choose <b>a category</b> to upload users",
     'es': "🕵️ Elige <b>una categoría</b> para subir usuarios",
     'fr': "🕵️ Choisissez <b>une catégorie</b> pour télécharger des utilisateurs",
     'zh': "🕵️选择<b>一个类别</b>上传用户",
     'ar': "🕵️ اختر <b>فئة</b> لتحميل المستخدمين",
 }
 l_find_bot_choose = {
-    'ru': "🥾 Выбери <b>категорию</b> для выгрузки ботов",
+    'ru': "🥾 <b>Выбери категорию</b> для выгрузки ботов",
     'en': "🥾 Choose <b>a category</b> for uploading bots",
     'es': "🥾 Elija <b>una categoría</b> para cargar bots",
     'fr': "🥾 Choisissez <b>une catégorie</b> pour télécharger des bots",
     'zh': "🥾 选择上传机器人的<b>类别</b>",
     'ar': "🥾 اختر <b>فئة</b> لتحميل الروبوتات",
 }
 
@@ -2924,15 +2924,15 @@
     'en': "⚙️ <b>Choose</b> option for <i>settings</i> /cmd <b>{0}</b> {1}",
     'es': "⚙️ <b>Elegir</b> opción para <i>configuración</i> /cmd <b>{0}</b> {1}",
     'fr': "⚙️ <b>Choisir</b> l'option pour les <i>paramètres</i> /cmd <b>{0}</b> {1}",
     'zh': "⚙️ <i>設置</i> /cmd <b>{0}</b>{1}的<b>選擇</b>選項",
     'ar': "⚙️ <b> اختر </b> خيار <i> الإعدادات </i> /cmd <b>{0}</b>{1}",
 }
 l_chat_join_request_handler = {
-    'ru': "👮🏽 {0}, ты отправил(а) заявку на вступление в <b>{1}</b>\n\n👉🏼 Выбери <i>правильный вариант</i> в соответствии с <code>заданием</code> на картинке, чтобы твоя <i>заявка</i> на вступление была <b>одобрена</b>",
+    'ru': "👮🏽 {0}, ты отправил(а) заявку на вступление в <b>{1}</b>\n\n👉🏼 <b>Выбери</b> <i>правильный вариант</i> в соответствии с <code>заданием</code> на картинке, чтобы твоя <i>заявка</i> на вступление была <b>одобрена</b>",
     'en': "👮🏽 {0}, you send join-request to channel <b>{1}</b>\n\n👉🏼 Choose <i>correct option</i> according to the <code>task</code> on picture to Approve your join-<i>request</i>",
     'es': "👮🏽 {0}, envías una solicitud de unión al grupo <b>{1}</b>\n\n👉🏼 Elige la <i>opción correcta</i> según la <code>tarea</code> en la imagen para aprobar su <i>solicitud de unión</i>",
     'fr': "👮🏽 {0}, vous envoyez une demande de participation au channele <b>{1}</b>\n\n👉🏼 Choisissez <i>l'option correcte</i> en fonction de la <code>tâche</code> sur l'image pour approuver votre inscription-<i>demande</i>",
     'zh': "👮🏽 {0}，你發送加入請求到組 <b>{1}</b>\n\n👉🏼 根據<code>task</code>選擇<i>正確的選項</i> 在圖片上批准您的加入-<i>請求</i>",
     'ar': "👮🏽 {0} ، ترسل طلب انضمام إلى المجموعة <b>{1}</b> \n\n👉🏼 اختر <i> الخيار الصحيح </i> وفقًا لـ <code> المهمة </code> على الصورة للموافقة على انضمامك- <i> طلب </i>",
 }
 l_content_types_sub_button = {
@@ -5025,15 +5025,15 @@
     'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
     'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
     'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
 }
 l_cinvite_choose_src = {
-    'ru': "🚶🏽 Выбери <b>источник</b>, откуда будем брать @username для авто-инвайта",
+    'ru': "🚶🏽 <b>Выбери источник</b>, откуда будем брать @username для авто-инвайта",
     'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
     'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
     'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
 }
 l_cinvite_choose_cnt = {
@@ -5586,15 +5586,15 @@
     'en': "🚀 You have to ⚙️Configure at least one post via 🔔Auto-posting",
     'es': "🚀 Tienes que ⚙️Configurar al menos una publicación a través de 🔔Publicación automática",
     'fr': "🚀 Vous devez ⚙️Configurer au moins une publication via 🔔Auto-publication",
     'zh': "🚀您必須通過🔔自動發布⚙️配置至少一篇帖子",
     'ar': "🚀 عليك تكوين منشور واحد على الأقل عبر النشر التلقائي",
 }
 l_cstartconfig_text = {
-    'ru': "🚀 Выбери <b>пост</b>, который будет присылаться в ответ на <b>старт</b>-слова и жми [🚀 <b>Использовать</b>] под выбранным постом\n\n👉🏼 Общее количество старт-слов: <u>{0}</u>",
+    'ru': "🚀 <b>Выбери пост</b>, который будет присылаться в ответ на <b>старт</b>-слова и жми [🚀 <b>Использовать</b>] под выбранным постом\n\n👉🏼 Общее количество старт-слов: <u>{0}</u>",
     'en': "🚀 At first, choose the auto-reply (from posts), which will be sent in response to the start-words",
     'es': "🚀 Al principio, elija la respuesta automática (de las publicaciones), que se enviará en respuesta a las palabras de inicio",
     'fr': "🚀 Dans un premier temps, choisissez la réponse automatique (à partir des messages), qui sera envoyée en réponse aux mots de départ",
     'zh': "🚀 首先，選擇自動回复（來自帖子），它將響應起始詞發送",
     'ar': "🚀 في البداية ، اختر الرد التلقائي (من المشاركات) ، والذي سيتم إرساله ردًا على كلمات البداية",
 }
 l_cstartconfig_use = {
@@ -6450,15 +6450,15 @@
     'es': "🐋 <b>Grupos añadidos</b>\n\n[comandos /cmd]",
     'fr': "🐋 <b>botes ajoutés</b>\n\n[commands /cmd]",
     'zh': "🐋 <b>添加組</b>\n\n[命令 /cmd]",
     'ar': "🐋 <b> المجموعات المضافة </b> \n\n [أوامر /cmd]",
 }
 
 l_creturntext = {
-    'ru': "✖️ Сбросить настройки по умолчанию (до рекомендуемых) для бота [<b>{0}</b>]?",
+    'ru': "✖️ <b>Сбросить</b> настройки по умолчанию (до рекомендуемых) для бота [<b>{0}</b>]?",
     'en': "✖️ Restore settings to default for bot [<b>{0}</b>]?",
     'es': "✖️ ¿Restaurar la configuración predeterminada para el grupo [<b>{0}</b>]?",
     'fr': "✖️ Restaurer les paramètres par défaut pour le bote [<b>{0}</b>] ?",
     'zh': "✖️ 將組 [<b>{0}</b>] 的設置恢復為默認設置？",
     'ar': "✖️ هل تريد استعادة الإعدادات الافتراضية للمجموعة [<b>{0}</b>]؟",
 }
 l_creturnanswer = {
```

### Comparing `yeref-0.1.68/yeref/yeref.py` & `yeref-0.1.69/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,16 @@
         # POST
         cur.execute('''CREATE TABLE IF NOT EXISTS POST ( 
             POST_ID            INTEGER      PRIMARY KEY AUTOINCREMENT
                                             UNIQUE
                                             NOT NULL,
             POST_CHATTID       BIGINT       NOT NULL,
             POST_USERTID       BIGINT       NOT NULL,
+            
+            POST_TARGET        VARCHAR,
             POST_TEXT          VARCHAR,
             POST_MEDIATYPE     VARCHAR,
             POST_FILEID        VARCHAR,
             POST_FILEIDNOTE    VARCHAR,
             POST_FILENAME      VARCHAR,
 
             POST_TGPHLINK      VARCHAR,
```

