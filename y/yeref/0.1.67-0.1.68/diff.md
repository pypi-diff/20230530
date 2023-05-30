# Comparing `tmp/yeref-0.1.67.tar.gz` & `tmp/yeref-0.1.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.67.tar", last modified: Sun May 28 15:01:58 2023, max compression
+gzip compressed data, was "yeref-0.1.68.tar", last modified: Tue May 30 08:22:17 2023, max compression
```

## Comparing `yeref-0.1.67.tar` & `yeref-0.1.68.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-28 15:01:58.185911 yeref-0.1.67/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-28 15:01:58.186205 yeref-0.1.67/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-28 15:01:58.187826 yeref-0.1.67/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-28 15:01:46.000000 yeref-0.1.67/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-28 15:01:58.176803 yeref-0.1.67/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.67/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   489139 2023-05-27 17:27:42.000000 yeref-0.1.67/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   204736 2023-05-27 15:53:48.000000 yeref-0.1.67/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-28 15:01:58.185030 yeref-0.1.67/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-28 15:01:58.000000 yeref-0.1.67/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-28 15:01:58.000000 yeref-0.1.67/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-28 15:01:58.000000 yeref-0.1.67/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-28 15:01:58.000000 yeref-0.1.67/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 08:22:17.258000 yeref-0.1.68/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 08:22:17.258251 yeref-0.1.68/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-30 08:22:17.259239 yeref-0.1.68/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-30 08:22:03.000000 yeref-0.1.68/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 08:22:17.251550 yeref-0.1.68/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.68/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   489265 2023-05-29 15:12:40.000000 yeref-0.1.68/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   205872 2023-05-29 13:36:05.000000 yeref-0.1.68/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-30 08:22:17.257171 yeref-0.1.68/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-30 08:22:17.000000 yeref-0.1.68/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-30 08:22:17.000000 yeref-0.1.68/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-30 08:22:17.000000 yeref-0.1.68/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-30 08:22:17.000000 yeref-0.1.68/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.67/setup.py` & `yeref-0.1.68/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.67',
+      version='0.1.68',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.67/yeref/l_.py` & `yeref-0.1.68/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,15 +477,15 @@
     'en': "👩🏽‍💻 In the <b>[Privacy]</b> settings, add @{0} to <i>the exclusions</i> for <b>[Voice Messages]</b> to display <code>видео-заметку</code> / <code>голосовое</code>",
     'es': "👩🏽‍💻 En la configuración <b>de [Privacidad]</b> , agregue @{0} a <i>las exclusiones</i> de <b>[Mensajes de voz]</b> para mostrar <code>видео-заметку</code> / <code>голосовое</code>",
     'fr': "👩🏽‍💻 Dans les paramètres <b>[Confidentialité]</b> , ajoutez @{0} aux <i>exclusions</i> pour <b>[Messages vocaux]</b> pour afficher <code>видео-заметку</code> / <code>голосовое</code>",
     'zh': "👩🏽‍💻在<b>【隐私】</b>设置中，添加@{0}到<b>【语音消息】</b>的<i>排除项</i>中，以显示<code>видео-заметку</code> / <code>голосовое</code>",
     'ar': "👩🏽‍💻 في إعدادات <b>[الخصوصية]</b> ، أضف @ {0} إلى <i>استثناءات</i> <b>[الرسائل الصوتية]</b> لعرض <code>видео-заметку</code> / <code>голосовое</code>",
 }
 l_post_tz = {
-    'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 Текущее время: <u>{0}</u> ({1}{2} по Гринвичу)",
+    'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 <b>Текуще</b>е время: <u>{0}</u> ({1}{2} по Гринвичу)",
     'en': "📍 Location <b>time zone</b> set\n\n🕐 Current time: <u>{0}</u> ({1}{2} GMT)",
     'es': "📍 Configuración <b>de la zona horaria</b> de la ubicación\n\n🕐 Hora actual: <u>{0}</u> ({1}{2} GMT)",
     'fr': "📍 <b>Fuseau horaire</b> de l&#x27;emplacement défini\n\n🕐 Heure actuelle : <u>{0}</u> ({1}{2} GMT)",
     'zh': "📍 位置<b>时区</b>设置\n\n🕐 当前时间： <u>{0}</u> （{1}{2} GMT）",
     'ar': "📍 تعيين <b>المنطقة الزمنية</b> للموقع\n\n🕐 الوقت الحالي: <u>{0}</u> ({1} {2} GMT)",
 }
 l_post_time_future = {
@@ -557,15 +557,15 @@
     'en': "👩🏽‍💻 <b>Enter</b> recipient Ids separated by spaces or separator characters",
     'es': "👩🏽‍💻 <b>Ingrese</b> las identificaciones de los destinatarios separadas por espacios o caracteres separadores",
     'fr': "👩🏽‍💻 <b>Entrez</b> les identifiants des destinataires séparés par des espaces ou des caractères de séparation",
     'zh': "👩🏽‍💻<b>输入</b>以空格或分隔符分隔的收件人 ID",
     'ar': "<b>أدخل</b> معرفات المستلمين مفصولة بمسافات أو أحرف فاصلة",
 }
 l_post_time_zone = {
-    'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 Текущее время: <u>{0}</u> ({1}{2} по Гринвичу)",
+    'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 <b>Текущее</b> время: <u>{0}</u> ({1}{2} по Гринвичу)",
     'en': "📍 Location <b>time zone</b> set\n\n🕐 Current time: <u>{0}</u> ({1}{2} GMT)",
     'es': "📍 Configuración <b>de la zona horaria</b> de la ubicación\n\n🕐 Hora actual: <u>{0}</u> ({1}{2} GMT)",
     'fr': "📍 <b>Fuseau horaire</b> de l&#x27;emplacement défini\n\n🕐 Heure actuelle : <u>{0}</u> ({1}{2} GMT)",
     'zh': "📍 位置<b>时区</b>设置\n\n🕐 当前时间： <u>{0}</u> （{1}{2} GMT）",
     'ar': "📍 تعيين <b>المنطقة الزمنية</b> للموقع\n\n🕐 الوقت الحالي: <u>{0}</u> ({1} {2} GMT)",
 }
 l_broadcast_plan = {
@@ -598,15 +598,15 @@
     'es': "🏁 <b>Boletín</b> finalizado\n\n🗝️ Número de usuarios que recibieron el mensaje: <u>{0}</u>",
     'fr': "🏁 <b>Newsletter</b> terminée\n\n🗝️ Nombre d&#x27;utilisateurs ayant reçu le message : <u>{0}</u>",
     'zh': "🏁<b>通讯</b>结束\n\n🗝️ 收到消息的用户数： <u>{0}</u>",
     'ar': "🏁 انتهت <b>الرسالة الإخبارية</b>\n\n🗝️ عدد المستخدمين الذين تلقوا الرسالة: <u>{0}</u>",
 }
 
 l_generate_calendar_time = {
-    'ru': "🕒 Отправь <b>время</b> поста на {0} в формате <code>{1}</code>. Текущее время: <u>{2}</u> ({3} по Гринвичу)\n\n🔗 Пришли <b>геопозицию</b>, чтобы <i>автоматически</i> определить часовой пояс",
+    'ru': "🕒 <b>Отправь время</b> поста на {0} в формате <code>{1}</code>. Текущее время: <u>{2}</u> ({3} по Гринвичу)\n\n🔗 Пришли <b>геопозицию</b>, чтобы <i>автоматически</i> определить часовой пояс",
     'en': "🕒 Send <b>the time</b> of the post to {0} in the format <code>{1}</code> . Current time: <u>{2}</u> ({3} GMT)\n\n🔗 Send <b>geolocation</b> to <i>automatically</i> determine the time zone",
     'es': "🕒 Envía <b>la hora</b> de la publicación a {0} en el formato <code>{1}</code> . Hora actual: <u>{2}</u> ({3} GMT)\n\n🔗 Enviar <b>geolocalización</b> para determinar <i>automáticamente</i> la zona horaria",
     'fr': "🕒 Envoyez <b>l&#x27;heure</b> de la publication à {0} au format <code>{1}</code> . Heure actuelle : <u>{2}</u> ({3} GMT)\n\n🔗 Envoyez <b>la géolocalisation</b> pour déterminer <i>automatiquement</i> le fuseau horaire",
     'zh': "🕒 以<code>{1}</code>格式将帖子<b>时间</b>发送到 {0}。当前时间： <u>{2}</u> ({3} GMT)\n\n🔗 发送<b>地理定位</b>以<i>自动</i>确定时区",
     'ar': "🕒 أرسل <b>وقت</b> النشر إلى {0} بالتنسيق <code>{1}</code> . الوقت الحالي: <u>{2}</u> ({3} GMT)\n\n🔗 أرسل <b>الموقع الجغرافي</b> لتحديد المنطقة الزمنية <i>تلقائيًا</i>",
 }
 l_month_1 = {
@@ -3415,23 +3415,23 @@
     'ar': "🔘️☐ تعطيل مكافحة الغارة",
 }
 # endregion
 
 
 # region cban_
 l_cban_add = {
-    'ru': "🕵🏽 <b>Введи</b> <code>id</code> или <code>@username</code> пользователей  через пробельные символы или разделители, чтобы добавить их в /ban-список (*даже тех, кого нет <u>{0}</u>-файле)\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Введи</b> <code>id</code> или <code>@username</code> пользователей  через пробельные символы или разделители, чтобы добавить их в /ban-список (*даже тех, кого нет <u>{0}</u>-файле)\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cban_remove = {
-    'ru': "🕵🏽 <b>Введи</b> <code>id</code> или <code>@username</code> пользователей из <u>{0}</u>-файла через пробельные символы или разделители, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Введи</b> <code>id</code> или <code>@username</code> пользователей из <u>{0}</u>-файла через пробельные символы или разделители, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cban_added = {
@@ -3447,15 +3447,15 @@
     'en': "🕵🏽 Push the ✅/☑️ to <b>On/Off</b> <u>auto</u>-ban <i>bots with recently registered new-id/without @username/bots from <a href='https://cas.chat'>Anti-Spam System</a>/bots with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 For example, option <b>new-id</b> blocks bots with <i>fresh</i> <u>id</u> and with the same photo upload <u>date</u> <i>many avatars</i>",
     'es': "🕵🏽 Presiona ✅/☑️ para <b>Encender/Apagar</b> <u>Auto</u>-banear <i>cuentas con nueva identificación registrada recientemente/cuentas eliminadas/cuentas de <a href='https://cas.chat'>Anti-Spam System</a>/cuentas con 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 Por ejemplo, la opción <b>deleted-ban</b> elimina dichas cuentas: <i>👻 Cuenta eliminada [estafa, falsa]</i>",
     'fr': "🕵🏽 Appuyez sur ✅/☑️ pour <b>On/Off</b> <u>auto</u>-bannir <i>les comptes avec un nouvel identifiant/des comptes supprimés/des comptes récemment enregistrés depuis <a href='https://cas.chat'>Anti-Spam System</a>/comptes avec 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 Par exemple, l'option <b>deleted-ban</b> supprime ces comptes : <i>👻 Compte supprimé [arnaque, faux]</i>",
     'zh': "🕵🏽 按下 ✅/☑️，以 <b>On/Off</b> <u>auto</u>-禁止 <i>具有最近從 註冊的 new-id/deleted-bots/bots <a href='https://cas.chat'>Anti-Spam System</a>/bots with text-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 例如，選項 <b>deleted-ban</b> 刪除此類帳戶：<i>👻 Deleted bot [scam,fake]</i>",
     'ar': "🕵🏽 اضغط على ✅ / ☑️ ، إلى <b> تشغيل / إيقاف </b> <u> تلقائي </u> -حظر <i> الحسابات ذات المعرف الجديد / الحسابات / الحسابات المحذوفة حديثًا من <a href='https://cas.chat'> نظام مكافحة البريد العشوائي </a> / حسابات مع 文 -glif، ب- arab، <a href='https://www.zalgo.org'> zalgo-icons </a> </i> \n\n👩🏽‍💻 على سبيل المثال ، الخيار <b> حذف-حظر </b> يحذف مثل هذه الحسابات: <i> 👻 الحساب المحذوف [احتيال ، وهمي] </i>",
 }
 l_cban_done = {
-    'ru': "🕵🏽 <b>Готово!</b> /ban-список нежелательных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Готово!</b> /ban-список нежелательных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 l_cban_correct = {
@@ -3563,15 +3563,15 @@
     'en': "🔔 You have to  ⚙️Configure at least one post",
     'es': "🔔 Tienes que ⚙️Configurar al menos una publicación",
     'fr': "🔔 Vous devez ⚙️Configurer au moins une publication",
     'zh': "🔔 你必須⚙️至少配置一篇帖子",
     'ar': "🔔 يجب عليك ⚙️ تكوين منشور واحد على الأقل",
 }
 l_cpost_text = {
-    'ru': "🔔 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <b>авто</b>-постинг по дате\n\n👉🏼 Текущее количество постов <u>{0}</u>",
+    'ru': "🔔 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <b>авто</b>-постинг по дате\n\n👉🏼 <b>Текущее</b> количество постов <u>{0}</u>",
     'en': "🔔 Push the ✅/☑️, to <b>On/Off</b> <b>auto</b>-posting of messages to channel by datetime\n\n👉🏼 Current post number is <u>{0}</u>",
     'es': "🔔 Presiona ✅/☑️ para <b>activar/desactivar</b> <b>automático</b>: publicación de mensajes para agrupar por fecha y hora\n\n👉🏼 El número de publicación actual es <u>{0}</u>",
     'fr': "🔔 Appuyez sur ✅/☑️, sur <b>On/Off</b> <b>auto</b>-publication des messages pour channeler par datetime\n\n👉🏼 Le numéro de publication actuel est <u>{0}</u>",
     'zh': "🔔 將 ✅/☑️ 推到 <b>On/Off</b> <b>auto</b>- 將消息發佈到按日期時間分組\n\n👉🏼 當前帖子編號是 <u>{0}</u>",
     'ar': "🔔 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> <b> تلقائي </b> - النشر التلقائي للرسائل إلى التجميع حسب التاريخ والوقت \n\n👉🏼 رقم المنشور الحالي هو <u>{0}</u>"
 }
 l_fsm_post_call = {
@@ -4628,15 +4628,15 @@
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_flood_text = {
-    'ru': "💬 <b>Введи</b> корректное <i>число</i> сообщений от <u>3</u> до <u>10</u>\n\n👉🏼 Текущее значение <code>/flood {0}</code>\n\n👩🏽‍💻 Например, /flood 3 (идентификация 3х сообщений подряд как flood)\n/flood 0 (отключение опции)",
+    'ru': "💬 <b>Введи</b> корректное <i>число</i> сообщений от <u>3</u> до <u>10</u>\n\n👉🏼 <b>Текущее</b> значение <code>/flood {0}</code>\n\n👩🏽‍💻 Например, /flood 3 (идентификация 3х сообщений подряд как flood)\n/flood 0 (отключение опции)",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_flood_on = {
@@ -4652,15 +4652,15 @@
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_delay_text = {
-    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Текущее значение <code>/delay {0}</code>\n\n👩🏽‍💻 Например, /delay 3 (ограничение на 3 min)\n/delay 0 (отключение опции)",
+    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 <b>Текущее</b> значение <code>/delay {0}</code>\n\n👩🏽‍💻 Например, /delay 3 (ограничение на 3 min)\n/delay 0 (отключение опции)",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_delay_on = {
@@ -5562,15 +5562,15 @@
     'ar': "🦊 جاهز! <b> استثناءات </b> لحزم الملصقات: \n\n + المسموح بها: <u>{0}</u>\n- محظور: <u>{1}</u>\n\n [✅ السماح] السماح بحزم الملصقات المحددة <i> كاستثناء </i> ، عندما [☑️☐ ملصق إيقاف]\n[🚫 منع] يحظر حزم الملصقات المحددة <i> كاستثناء </i> ، عندما [✅☑ على الملصق]",
 }
 # endregion
 
 
 # region cstart_
 l_cstart_text = {
-    'ru': "🚀 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-ответ на триггер-сообщения, содержащие конкретные старт-слова\n\n👉🏼 Текущее количество старт-слов <u>{0}</u>",
+    'ru': "🚀 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-ответ на триггер-сообщения, содержащие конкретные старт-слова\n\n👉🏼 <b>Текущее</b> количество старт-слов <u>{0}</u>",
     'en': "🚀 Push the ✅/☑️, to <b>On/Off</b> auto-answer on trigger-messages, containing specific start-words\n\n👉🏼 Current number of start-words <u>{0}</u>",
     'es': "🚀 Presiona ✅/☑️, para <b>Activar/Desactivar</b> la respuesta automática en mensajes desencadenantes, que contienen palabras de inicio específicas\n\n👉🏼 Número actual de palabras de inicio <u>{0}</u>",
     'fr': "🚀 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> la réponse automatique aux messages déclencheurs, contenant des mots de départ spécifiques\n\n👉🏼 Nombre actuel de mots de départ <u>{0}</u>",
     'zh': "🚀 將 ✅/☑️ 推到 <b>On/Off</b> 觸發消息上的自動應答，包含特定的起始詞\n\n👉🏼 當前起始詞的數量<u>{0}</u>",
     'ar': "🚀 اضغط على ✅ / ☑️ ، لإجراء تشغيل / إيقاف الرد التلقائي على الرسائل المشغلة ، التي تحتوي على كلمات بداية محددة \n\n👉🏼 العدد الحالي لكلمات البداية {0} / ش",
 }
 l_cstart_call = {
@@ -5671,15 +5671,15 @@
 }
 
 # endregion
 
 
 # region cstop_
 l_cstop_text = {
-    'ru': "🧾 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-удаление сообщений, содержащие запрещенные стоп-слова\n\n👉🏼 Текущее количество стоп-слов <u>{0}</u>",
+    'ru': "🧾 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-удаление сообщений, содержащие запрещенные стоп-слова\n\n👉🏼 <b>Текущее</b> количество стоп-слов <u>{0}</u>",
     'en': "🧾 Push the ✅/☑️, to <b>On/Off</b> auto-delete of messages, containing prohibited stop-words\n\n👉🏼 Current number of stop-words <u>{0}</u>",
     'es': "🧾 Pulsa ✅/☑️ para <b>activar/desactivar</b> la eliminación automática de mensajes que contengan palabras vacías prohibidas\n\n👉🏼 Número actual de palabras vacías <u>{0}</u>",
     'fr': "🧾 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> la suppression automatique des messages contenant des mots vides interdits\n\n👉🏼 Nombre actuel de mots vides <u>{0}</u>",
     'zh': "🧾 按下 ✅/☑️, 以<b>開/關</b>自動刪除包含禁止停用詞的消息\n\n👉🏼 當前停用詞數量<u>{0}</u>",
     'ar': "🧾 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> للحذف التلقائي للرسائل ، التي تحتوي على كلمات إيقاف محظورة \n\n👉🏼 العدد الحالي لكلمات التوقف <u>{0}</u>",
 }
 l_cstop_call = {
@@ -6567,15 +6567,15 @@
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 l_cpayment_token = {
-    'ru': "💳️ <b>Вставь</b> платежный токен, полученный из @BotFather-бота\n\n👩🏽‍💻 <b>Например</b>\n<code>401643678:7049d0b3-f0267096c4a1</code>\n\n👩🏽‍💻 Текущий токен:\n{0}",
+    'ru': "💳️ <b>Вставь</b> платежный токен, полученный из @BotFather-бота\n\n👩🏽‍💻 <b>Например</b>\n<code>401643678:7049d0b3-f0267096c4a1</code>\n\n👩🏽‍💻 <b>Текущий</b> токен:\n{0}",
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 l_cpayment_done = {
@@ -6637,31 +6637,31 @@
     'es': "☑️☐De nueva-id-ban",
     'fr': "☑️☐De nouveau-id-ban",
     'zh': "☑️☐關閉新身份證",
     'ar': "☑️☐ تعطيل حظر معرف جديد",
 }
 
 l_cintegration_google = {
-    'ru': "🗝️ <b>Вставь ссылку</b> на пустую google-таблицу (<i>с открытым доступом для редактирования</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, <code>https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing</code>\n\n👩🏽‍💻 Текущая ссылка:\n{1}",
+    'ru': "🗝️ <b>Вставь ссылку</b> на пустую google-таблицу (<i>с открытым доступом для редактирования</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, <code>https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing</code>\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 l_cintegration_airtable = {
-    'ru': "🗝️ <b>Вставь ссылку</b> на пустую airtable-таблицу (<i>с открытым доступом для редактирования и любого e-mail</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, <code>https://airtable.com/invite/l?inviteId=inv4VGM&inviteToken=f1d31f9aba6b&utm_medium=email</code>\n\n👩🏽‍💻 Текущая ссылка:\n{1}",
+    'ru': "🗝️ <b>Вставь ссылку</b> на пустую airtable-таблицу (<i>с открытым доступом для редактирования и любого e-mail</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, <code>https://airtable.com/invite/l?inviteId=inv4VGM&inviteToken=f1d31f9aba6b&utm_medium=email</code>\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 l_cintegration_done = {
-    'ru': "🗝️ <b>Готово!</b>\n\n👩🏽‍💻 Текущая ссылка:\n{0}",
+    'ru': "🗝️ <b>Готово!</b>\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{0}",
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 # endregion
@@ -6815,15 +6815,15 @@
     'en': "👩🏽‍💻 <b>Account:</b> is off\n\n/on - to on bot",
     'es': "💳 Agregar grupo",
     'fr': "💳 Ajouter un bote",
     'zh': "💳 添加組",
     'ar': "💳 إضافة مجموعة",
 }
 l_cuser_utm = {
-    'ru': "👥 <b>Готово!</b> <b>/utm-список</b> реферальных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Вывести</b> рефералов конкретного пользователя можно командой:\n<code>/utm id</code> или <code>/utm @username</code>\n\n👩🏽‍💻 Текущее число utm-рефералов: <u>{1}</u>",
+    'ru': "👥 <b>Готово!</b> <b>/utm-список</b> реферальных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Вывести</b> рефералов конкретного пользователя можно командой:\n<code>/utm id</code> или <code>/utm @username</code>\n\n👩🏽‍💻 <b>Текущее</b> число utm-рефералов: <u>{1}</u>",
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 l_cuser_link_done = {
@@ -6867,31 +6867,31 @@
     'en': "👮🏽 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "👮🏽 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "👮🏽 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "👮🏽 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cadmin_done = {
-    'ru': "👮🏽 <b>Готово!</b>/admin-список @{0}-бота:\n\n{1}\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 Текущее число администраторов: <u>{2}/10</u>",
+    'ru': "👮🏽 <b>Готово!</b>/admin-список @{0}-бота:\n\n{1}\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{2}/10</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cadmin_add = {
-    'ru': "👮🏽 <b>Введи</b> <code>id</code> пользователей через пробельные символы или разделители, чтобы добавить их в /admin-список\n\n👩🏽‍💻 Текущее число администраторов: <u>{0}</u>",
+    'ru': "👮🏽 <b>Введи</b> <code>id</code> пользователей через пробельные символы или разделители, чтобы добавить их в /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cadmin_remove = {
-    'ru': "👮🏽 <b>Введи</b> <code>id</code> пользователей через пробельные символы или разделители, чтобы удалить их из /admin-список\n\n👩🏽‍💻 Текущее число администраторов: <u>{0}</u>",
+    'ru': "👮🏽 <b>Введи</b> <code>id</code> пользователей через пробельные символы или разделители, чтобы удалить их из /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_parse_text = {
```

### Comparing `yeref-0.1.67/yeref/yeref.py` & `yeref-0.1.68/yeref/yeref.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 markupAdmin = types.ReplyKeyboardMarkup(keyboard=[
     [types.KeyboardButton(text='⬅️ Prev'), types.KeyboardButton(text='↩️ Menu'),
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
 
 BOT_VARS_ = '{"DATE_TIME": 0, "BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0}'
 BOT_LSTS_ = '{"ADMIN_USERS": [], "PREMIUM_USERS": [], "CHANNEL_USERS": [], "GROUP_USERS": [], "PROMO_USERS": [], "UTM_USERS": []}'
-USER_VARS_ = '{"USER_TEXT": "", "USER_PHONE": "", "USER_GEO": "", "USER_PROMO": "", "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "USER_UTM": "", "USER_ID": 0, "USER_TZ": 0, "USER_LC": "", "USER_DT": "", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "DATE_TIME": 0}'
+USER_VARS_ = '{"USER_TEXT": "", "USER_PHONE": "", "USER_EMAIL": "", "USER_GEO": "", "USER_PROMO": "", "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "USER_UTM": "", "USER_ID": 0, "USER_TZ": 0, "USER_LC": "", "USER_DT": "", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "DATE_TIME": 0}'
 USER_LSTS_ = '{"USER_UTMREF": []}'
 # endregion
 
 
 # region db
 def sqlite_lower(value_):
     return value_.lower() if value_ else None
@@ -284,14 +284,41 @@
             
             MSG_TEXT        VARCHAR,
             MSG_BUTTONS     VARCHAR,
             MSG_TEXTF       VARCHAR,
             MSG_BUTTONSF    VARCHAR
         )''')
 
+        # POST
+        cur.execute('''CREATE TABLE IF NOT EXISTS POST ( 
+            POST_ID            INTEGER      PRIMARY KEY AUTOINCREMENT
+                                            UNIQUE
+                                            NOT NULL,
+            POST_CHATTID       BIGINT       NOT NULL,
+            POST_USERTID       BIGINT       NOT NULL,
+            POST_TEXT          VARCHAR,
+            POST_MEDIATYPE     VARCHAR,
+            POST_FILEID        VARCHAR,
+            POST_FILEIDNOTE    VARCHAR,
+            POST_FILENAME      VARCHAR,
+
+            POST_TGPHLINK      VARCHAR,
+            POST_ISTGPH        BOOLEAN     DEFAULT 0,
+            POST_BUTTON        VARCHAR,
+            POST_ISBUTTON      BOOLEAN     DEFAULT 0,
+            POST_ISSPOILER     BOOLEAN     DEFAULT 0,
+            POST_ISPIN         BOOLEAN     DEFAULT 0,
+            POST_ISSILENCE     BOOLEAN     DEFAULT 0,
+            POST_ISGALLERY     BOOLEAN     DEFAULT 0,
+
+            POST_STATUS        BOOLEAN     DEFAULT 0,
+            POST_TZ            VARCHAR,
+            POST_DT            VARCHAR
+        )''')
+        
         # USER
         cur.execute(f'''CREATE TABLE IF NOT EXISTS USER ( 
             USER_ID         INTEGER     PRIMARY KEY AUTOINCREMENT
                                         UNIQUE
                                         NOT NULL,
             USER_TID        BIGINT      UNIQUE
                                         NOT NULL,
```

