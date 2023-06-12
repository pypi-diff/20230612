# Comparing `tmp/yeref-0.1.91.tar.gz` & `tmp/yeref-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.91.tar", last modified: Mon Jun 12 16:04:32 2023, max compression
+gzip compressed data, was "yeref-0.1.92.tar", last modified: Mon Jun 12 18:24:20 2023, max compression
```

## Comparing `yeref-0.1.91.tar` & `yeref-0.1.92.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 16:04:32.294782 yeref-0.1.91/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 16:04:32.294961 yeref-0.1.91/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 16:04:32.297278 yeref-0.1.91/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 16:04:17.000000 yeref-0.1.91/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 16:04:32.286559 yeref-0.1.91/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.91/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   554470 2023-06-12 16:04:06.000000 yeref-0.1.91/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   213869 2023-06-12 11:47:33.000000 yeref-0.1.91/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 16:04:32.294177 yeref-0.1.91/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 16:04:32.000000 yeref-0.1.91/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 16:04:32.000000 yeref-0.1.91/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 16:04:32.000000 yeref-0.1.91/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 16:04:32.000000 yeref-0.1.91/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 18:24:20.152635 yeref-0.1.92/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 18:24:20.152811 yeref-0.1.92/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-12 18:24:20.154101 yeref-0.1.92/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-12 18:24:03.000000 yeref-0.1.92/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 18:24:20.146036 yeref-0.1.92/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.92/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   547540 2023-06-12 16:51:53.000000 yeref-0.1.92/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   215610 2023-06-12 18:17:26.000000 yeref-0.1.92/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-12 18:24:20.152025 yeref-0.1.92/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-12 18:24:20.000000 yeref-0.1.92/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-12 18:24:20.000000 yeref-0.1.92/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-12 18:24:20.000000 yeref-0.1.92/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-12 18:24:20.000000 yeref-0.1.92/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.91/setup.py` & `yeref-0.1.92/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.91',
+      version='0.1.92',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -43,12 +43,12 @@
 
 # twine upload dist/*
 # freey.sitner.ya
 # cejwez-nosgin-vaVfe7
 
 # python3 -m pip install --upgrade yeref
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.80-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.91-py3-none-any.whl
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
 # ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.91/yeref/l_.py` & `yeref-0.1.92/yeref/l_.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     'es': "👩🏽‍💻 Me suscribí",
     'fr': "👩🏽‍💻 je me suis abonné",
     'zh': "👩🏽‍💻 我订阅了",
     'ar': "👩🏽‍💻 لقد اشتركت",
 }
 l_subscribe_all = {
     'ru': "¹ Все боты и проекты",
-    'en': "¹ All bots & projects",
+    'en': "¹ Все боты и проекты",
     'es': "¹ All bots & projects",
     'fr': "¹ All bots & projects",
     'zh': "¹ All bots & projects",
     'ar': "¹ All bots & projects",
 }
 l_subscribe_already = {
     'ru': "👩🏽‍💻 У вас уже есть активная подписка",
@@ -316,36 +316,36 @@
     'en': "☑️ No",
     'es': "☑️No",
     'fr': "☑️ Non",
     'zh': "☑️没有",
     'ar': "☑️ لا",
 }
 l_post_button = {
-    'ru': "✏️ 3. <b>Введи названия</b> для кнопок и <b>ссылки</b> в формате (одну или несколько; кликни на образец ниже, чтобы скопировать):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ Интересно][💔 Не пиши]</code>\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
-    'en': "✏️ 3. <b>Enter button names</b> and <b>links</b> in the format (one or more; click on the sample below to copy):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nor\n\n<code>[❤️ Интересно][💔 Не пиши]</code>\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
-    'es': "✏️ 3. <b>Ingrese los nombres de los botones</b> y <b>los enlaces</b> en el formato (uno o más; haga clic en la muestra a continuación para copiar):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\ni\n\n<code>[❤️ Интересно][💔 Не пиши]</code>\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
-    'fr': "✏️ 3. <b>Saisissez les noms des boutons</b> et <b>les liens</b> au format (un ou plusieurs ; cliquez sur l&#x27;exemple ci-dessous pour le copier) :\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nor\n\n<code>[❤️ Интересно][💔 Не пиши]</code>\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
-    'zh': "✏️ 3.<b>输入按钮名称</b>和<b>链接</b>格式（一个或多个；点击下方示例复制）：\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nor\n\n<code>[❤️ Интересно][💔 Не пиши]</code>\n\n（<i>或按“➡️️/Next”跳过这一步</i>）",
-    'ar': "✏️ 3. <b>أدخل أسماء الأزرار</b> <b>والارتباطات</b> بالتنسيق (واحد أو أكثر ؛ انقر على النموذج أدناه لنسخه):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\ ولا\n\n<code>[❤️ Интересно][💔 Не пиши]</code>\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
+    'ru': "✏️ 3. <b>Введи названия</b> для кнопок и <b>ссылки</b> в формате (одну или несколько; кликни на образец ниже, чтобы скопировать):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ Like][💔 Foo]</code>\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'en': "✏️ 3. <b>Enter button names</b> and <b>links</b> in the format (one or more; click on the sample below to copy):\n\n[🐳 Link | https://t.me/XXXXX]\n\nor\n\n[❤️ Интересно][💔 Не пиши]\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
+    'es': "✏️ 3. <b>Ingrese los nombres de los botones</b> y <b>los enlaces</b> en el formato (uno o más; haga clic en la muestra a continuación para copiar):\n\n[🐳 Link | https://t.me/XXXXX]\n\ni\n\n[❤️ Интересно][💔 Не пиши]\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
+    'fr': "✏️ 3. <b>Saisissez les noms des boutons</b> et <b>les liens</b> au format (un ou plusieurs ; cliquez sur l&#x27;exemple ci-dessous pour le copier) :\n\n[🐳 Link | https://t.me/XXXXX]\n\nor\n\n[❤️ Интересно][💔 Не пиши]\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
+    'zh': "✏️ 3.<b>输入按钮名称</b>和<b>链接</b>格式（一个或多个；点击下方示例复制）：\n\n[🐳 Link | https://t.me/XXXXX]\n\nor\n\n[❤️ Интересно][💔 Не пиши]\n\n（<i>或按“➡️️/Next”跳过这一步</i>）",
+    'ar': "✏️ 3. <b>أدخل أسماء الأزرار</b> <b>والارتباطات</b> بالتنسيق (واحد أو أكثر ؛ انقر على النموذج أدناه لنسخه):\n\n[🐳 Link | https://t.me/XXXXX]\n\ ولا\n\n[❤️ Интересно][💔 Не пиши]\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_button_urlinvalid = {
     'ru': "🔗 Ссылка {0} не действительна",
     'en': "🔗 Link {0} is invalid",
     'es': "🔗 El enlace {0} no es válido",
     'fr': "🔗 Le lien {0} est invalide",
     'zh': "🔗 链接 {0} 无效",
     'ar': "🔗 الرابط {0} غير صالح",
 }
 l_post_pin = {
-    'ru': "✏️ 3. Закреплять (<b>pin</b>) сообщение сверху экрана: <code>да</code> | <code>нет</code>?\n\n(<i>или нажми «➡️️/Next», чтобы <u>не закреплять</u> сообщение</i>)",
-    'en': "✏️ 3. Pin ( <b>pin</b> ) the message on top of the screen: <code>да</code> | <code>нет</code> ?\n\n( <i>or press &quot;➡️️/Next&quot; to <u>not pin</u> the message</i> )",
-    'es': "✏️ 3. Pin ( <b>pin</b> ) el mensaje en la parte superior de la pantalla: <code>да</code> | <code>нет</code> ?\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para <u>no fijar</u> el mensaje</i> )",
-    'fr': "✏️ 3. Epingler ( <b>épingler</b> ) le message en haut de l&#x27;écran : <code>да</code> | <code>нет</code> ?\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour <u>ne pas épingler</u> le message</i> )",
-    'zh': "✏️ 3. 将消息置顶（<b>置顶</b>）： <code>да</code> | <code>нет</code> ？\n\n（<i>或按“➡️️/下一步”<u>不固定</u>消息</i>）",
-    'ar': "✏️ 3. قم بتثبيت ( <b>تثبيت</b> ) الرسالة أعلى الشاشة: <code>да</code> | <code>нет</code> ؟\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لعدم <u>تثبيت</u> الرسالة</i> )",
+    'ru': "✏️ 3. Закреплять (<b>pin</b>) сообщение сверху экрана: да | нет?\n\n(<i>или нажми «➡️️/Next», чтобы <u>не закреплять</u> сообщение</i>)",
+    'en': "✏️ 3. Pin ( <b>pin</b> ) the message on top of the screen: да | нет ?\n\n( <i>or press &quot;➡️️/Next&quot; to <u>not pin</u> the message</i> )",
+    'es': "✏️ 3. Pin ( <b>pin</b> ) el mensaje en la parte superior de la pantalla: да | нет ?\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para <u>no fijar</u> el mensaje</i> )",
+    'fr': "✏️ 3. Epingler ( <b>épingler</b> ) le message en haut de l&#x27;écran : да | нет ?\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour <u>ne pas épingler</u> le message</i> )",
+    'zh': "✏️ 3. 将消息置顶（<b>置顶</b>）： да | нет ？\n\n（<i>或按“➡️️/下一步”<u>不固定</u>消息</i>）",
+    'ar': "✏️ 3. قم بتثبيت ( <b>تثبيت</b> ) الرسالة أعلى الشاشة: да | нет ؟\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لعدم <u>تثبيت</u> الرسالة</i> )",
 }
 l_post_date = {
     'ru': "✏️ 4. <b>Выбери дату</b> на календаре\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 4. <b>Select a date</b> on the calendar\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 4. <b>Selecciona una fecha</b> en el calendario\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 4. <b>Sélectionnez une date</b> sur le calendrier\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 4. 在日历上<b>选择一个日期</b>\n\n（<i>或按“➡️️/Next”跳过此步骤</i>）",
@@ -413,20 +413,20 @@
     'en': "👩🏽‍💻 Post published",
     'es': "👩🏽‍💻 Publicación publicada",
     'fr': "👩🏽‍💻 Article publié",
     'zh': "👩🏽‍💻 帖子已发布",
     'ar': "👩🏽‍💻 تم نشر المنشور",
 }
 l_post_btn_answer = {
-    'ru': "✅ Пользователь <b>{0}</b> (username={1}, id=<code>{2}</code>) <i>нажал</i> на [<b>{3}</b>] в посте #<u>{4}</u>",
-    'en': "✅ User <b>{0}</b> (username={1}, id= <code>{2}</code> ) <i>clicked</i> on [<b>{3}</b>] in post # <u>{4}</u>",
-    'es': "✅ El usuario <b>{0}</b> (username={1}, id= <code>{2}</code> ) <i>hizo clic</i> en [<b>{3}</b>] en la publicación n.º <u>{4}</u>",
-    'fr': "✅ L'utilisateur <b>{0}</b> (username={1}, id= <code>{2}</code> ) <i>a cliqué</i> sur [<b>{3}</b>] dans le post # <u>{4}</u>",
-    'zh': "✅ 用户<b>{0}</b> （用户名 = {1}，id = <code>{2}</code> ）在帖子 # <u>{4}</u>中<i>点击了</i>[<b>{3}</b>]",
-    'ar': "✅ المستخدم <b>{0}</b> (اسم المستخدم = {1} ، المعرف = <code>{2}</code> ) <i>نقر</i> على [<b>{3}</b>] في المشاركة رقم <u>{4}</u>",
+    'ru': "✅ Пользователь <b>{0}</b> (username={1}, id={2}) <i>нажал</i> на [<b>{3}</b>] в посте #<u>{4}</u>",
+    'en': "✅ User <b>{0}</b> (username={1}, id= {2} ) <i>clicked</i> on [<b>{3}</b>] in post # <u>{4}</u>",
+    'es': "✅ El usuario <b>{0}</b> (username={1}, id= {2} ) <i>hizo clic</i> en [<b>{3}</b>] en la publicación n.º <u>{4}</u>",
+    'fr': "✅ L'utilisateur <b>{0}</b> (username={1}, id= {2} ) <i>a cliqué</i> sur [<b>{3}</b>] dans le post # <u>{4}</u>",
+    'zh': "✅ 用户<b>{0}</b> （用户名 = {1}，id = {2} ）在帖子 # <u>{4}</u>中<i>点击了</i>[<b>{3}</b>]",
+    'ar': "✅ المستخدم <b>{0}</b> (اسم المستخدم = {1} ، المعرف = {2} ) <i>نقر</i> على [<b>{3}</b>] في المشاركة رقم <u>{4}</u>",
 }
 l_post_datetime = {
     'ru': "<b>Дата публикации</b>",
     'en': "<b>Publication date</b>",
     'es': "<b>Fecha de publicación</b>",
     'fr': "<b>Date de publication</b>",
     'zh': "<b>发布日期</b>",
@@ -534,20 +534,20 @@
     'en': "👩🏽‍💻 [spoiler] mode available for photo/gif/video",
     'es': "👩🏽‍💻 Modo [spoiler] disponible para foto/gif/video",
     'fr': "👩🏽‍💻 Mode [spoiler] disponible pour photo/gif/vidéo",
     'zh': "👩🏽‍💻 [剧透] 模式可用于照片/gif/视频",
     'ar': "👩🏽‍💻 وضع [المفسد] متاح للصور / gif / الفيديو",
 }
 l_post_has_restricted = {
-    'ru': "👩🏽‍💻 У вас premium-аккаунт! В настройках <b>[Конфиденциальность]</b> добавь @{0} в <i>исключения</i> для <b>[Голосовые сообщения]</b>, чтобы отобразить <code>видео-заметку</code>/<code>голосовое</code>",
-    'en': "👩🏽‍💻 You have a premium account! In the <b>[Privacy]</b> settings, add @{0} to <i>the exclusions</i> for <b>[Voice Messages]</b> to display <code>видео-заметку</code> / <code>голосовое</code>",
-    'es': "👩🏽‍💻 ¡Tienes una cuenta premium! En la configuración <b>de [Privacidad]</b> , agregue @{0} a <i>las exclusiones</i> de <b>[Mensajes de voz]</b> para mostrar <code>видео-заметку</code> / <code>голосовое</code>",
-    'fr': "👩🏽‍💻 Vous avez un compte premium ! Dans les paramètres <b>[Confidentialité]</b> , ajoutez @{0} aux <i>exclusions</i> pour <b>[Messages vocaux]</b> pour afficher <code>видео-заметку</code> / <code>голосовое</code>",
-    'zh': "👩🏽‍💻 您拥有高级帐户！在<b>[隐私]</b>设置中，将@{0}添加到<b>[语音消息]</b>的<i>排除项</i>中以显示<code>видео-заметку</code> / <code>голосовое</code>",
-    'ar': "👩🏽‍💻 لديك حساب مميز! في إعدادات <b>[الخصوصية]</b> ، أضف @ {0} إلى <i>استثناءات</i> <b>[الرسائل الصوتية]</b> لعرض <code>видео-заметку</code> / <code>голосовое</code>",
+    'ru': "👩🏽‍💻 У вас premium-аккаунт! В настройках <b>[Конфиденциальность]</b> добавь @{0} в <i>исключения</i> для <b>[Голосовые сообщения]</b>, чтобы отобразить видео-заметку/голосовое",
+    'en': "👩🏽‍💻 You have a premium account! In the <b>[Privacy]</b> settings, add @{0} to <i>the exclusions</i> for <b>[Voice Messages]</b> to display видео-заметку / голосовое",
+    'es': "👩🏽‍💻 ¡Tienes una cuenta premium! En la configuración <b>de [Privacidad]</b> , agregue @{0} a <i>las exclusiones</i> de <b>[Mensajes de voz]</b> para mostrar видео-заметку / голосовое",
+    'fr': "👩🏽‍💻 Vous avez un compte premium ! Dans les paramètres <b>[Confidentialité]</b> , ajoutez @{0} aux <i>exclusions</i> pour <b>[Messages vocaux]</b> pour afficher видео-заметку / голосовое",
+    'zh': "👩🏽‍💻 您拥有高级帐户！在<b>[隐私]</b>设置中，将@{0}添加到<b>[语音消息]</b>的<i>排除项</i>中以显示видео-заметку / голосовое",
+    'ar': "👩🏽‍💻 لديك حساب مميز! في إعدادات <b>[الخصوصية]</b> ، أضف @ {0} إلى <i>استثناءات</i> <b>[الرسائل الصوتية]</b> لعرض видео-заметку / голосовое",
 }
 l_post_tz = {
     'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 <b>Текуще</b>е время: <u>{0}</u> ({1}{2} по Гринвичу)",
     'en': "📍 Location <b>time zone</b> set\n\n🕐 <b>Current</b> time: <u>{0}</u> ({1}{2} GMT)",
     'es': "📍 Configuración <b>de la zona horaria</b> de la ubicación\n\n🕐 Hora <b>actual</b> : <u>{0}</u> ({1}{2} GMT)",
     'fr': "📍 <b>Fuseau horaire</b> de l&#x27;emplacement défini\n\n🕐 Heure <b>actuelle</b> : <u>{0}</u> ({1}{2} GMT)",
     'zh': "📍 位置<b>时区</b>设置\n\n🕐<b>当前</b>时间： <u>{0}</u> （{1}{2} GMT）",
@@ -671,20 +671,20 @@
     'es': "🏁 <b>Boletín</b> completado\n\n📧 <b>Número</b> de usuarios que recibieron el mensaje: <u>{0}</u>",
     'fr': "🏁 <b>Newsletter</b> terminée\n\n📧 <b>Nombre</b> d&#x27;utilisateurs ayant reçu le message : <u>{0}</u>",
     'zh': "🏁<b>通讯</b>已完成\n\n📧 收到消息的用户<b>数</b>： <u>{0}</u>",
     'ar': "🏁 اكتملت <b>النشرة الإخبارية</b>\n\n📧 <b>عدد</b> المستخدمين الذين تلقوا الرسالة: <u>{0}</u>",
 }
 
 l_generate_calendar_time = {
-    'ru': "🕒 <b>Отправь время</b> поста на {0} в формате <code>{1}</code>. Текущее время: <u>{2}</u> ({3} по Гринвичу)\n\n🔗 Пришли <b>геопозицию</b>, чтобы <i>автоматически</i> определить часовой пояс",
-    'en': "🕒 <b>Send the time</b> of the post to {0} in the format <code>{1}</code> . Current time: <u>{2}</u> ({3} GMT)\n\n🔗 Send <b>geolocation</b> to <i>automatically</i> determine the time zone",
-    'es': "🕒 <b>Envía la hora</b> de la publicación a {0} en el formato <code>{1}</code> . Hora actual: <u>{2}</u> ({3} GMT)\n\n🔗 Enviar <b>geolocalización</b> para determinar <i>automáticamente</i> la zona horaria",
-    'fr': "🕒 <b>Envoyez l&#x27;heure</b> de la publication à {0} au format <code>{1}</code> . Heure actuelle : <u>{2}</u> ({3} GMT)\n\n🔗 Envoyez <b>la géolocalisation</b> pour déterminer <i>automatiquement</i> le fuseau horaire",
-    'zh': "🕒 以<code>{1}</code>格式将帖子<b>时间发送到</b>{0}。当前时间： <u>{2}</u> ({3} GMT)\n\n🔗 发送<b>地理定位</b>以<i>自动</i>确定时区",
-    'ar': "🕒 <b>أرسل وقت</b> النشر إلى {0} بالتنسيق <code>{1}</code> . الوقت الحالي: <u>{2}</u> ({3} GMT)\n\n🔗 أرسل <b>الموقع الجغرافي</b> لتحديد المنطقة الزمنية <i>تلقائيًا</i>",
+    'ru': "🕒 <b>Отправь время</b> поста на {0} в формате {1}. Текущее время: <u>{2}</u> ({3} по Гринвичу)\n\n🔗 Пришли <b>геопозицию</b>, чтобы <i>автоматически</i> определить часовой пояс",
+    'en': "🕒 <b>Send the time</b> of the post to {0} in the format {1} . Current time: <u>{2}</u> ({3} GMT)\n\n🔗 Send <b>geolocation</b> to <i>automatically</i> determine the time zone",
+    'es': "🕒 <b>Envía la hora</b> de la publicación a {0} en el formato {1} . Hora actual: <u>{2}</u> ({3} GMT)\n\n🔗 Enviar <b>geolocalización</b> para determinar <i>automáticamente</i> la zona horaria",
+    'fr': "🕒 <b>Envoyez l&#x27;heure</b> de la publication à {0} au format {1} . Heure actuelle : <u>{2}</u> ({3} GMT)\n\n🔗 Envoyez <b>la géolocalisation</b> pour déterminer <i>automatiquement</i> le fuseau horaire",
+    'zh': "🕒 以{1}格式将帖子<b>时间发送到</b>{0}。当前时间： <u>{2}</u> ({3} GMT)\n\n🔗 发送<b>地理定位</b>以<i>自动</i>确定时区",
+    'ar': "🕒 <b>أرسل وقت</b> النشر إلى {0} بالتنسيق {1} . الوقت الحالي: <u>{2}</u> ({3} GMT)\n\n🔗 أرسل <b>الموقع الجغرافي</b> لتحديد المنطقة الزمنية <i>تلقائيًا</i>",
 }
 l_month_1 = {
     'ru': "Янв",
     'en': "Jan",
     'es': "Ene",
     'fr': "Jan",
     'zh': "简",
@@ -965,20 +965,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_demo_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>информация</b> обо всех проектах\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> <code>проекта</code> :\n\n▪️ <b>information</b> about all projects\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>información</b> sobre todos los proyectos\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>informations</b> sur tous les projets\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎来到<b>Ferey</b> <code>проекта</code>的<i>落地机器人</i>：\n\n▪️ 所有项目的<b>信息</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>معلومات</b> حول جميع المشاريع\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта <b>Ferey</b>:\n\n▪️<b>информация</b> обо всех проектах\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> проекта :\n\n▪️ <b>information</b> about all projects\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del проекта <b>Ferey</b> :\n\n▪️ <b>información</b> sobre todos los proyectos\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du проекта <b>Ferey</b> :\n\n▪️ <b>informations</b> sur tous les projets\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到<b>Ferey</b> проекта的<i>落地机器人</i>：\n\n▪️ 所有项目的<b>信息</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص проекта <b>Ferey</b> :\n\n▪️ <b>معلومات</b> حول جميع المشاريع\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_demo = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -1114,20 +1114,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_work_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>проекта</code> <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> <code>проекта</code> :\n\n▪️ <b>vacancies</b> of our startup\n▪️ contests and <b>events</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>vacantes</b> de nuestra startup\n▪️ concursos y <b>eventos</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>offres d&#x27;emploi</b> de notre startup\n▪️ concours et <b>événements</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎来到<b>Ferey</b> <code>проекта</code>的<i>登陆机器人</i>：\n\n▪️ 我们初创公司的<b>职位空缺</b>\n▪️ 竞赛和<b>活动</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> <code>проекта</code> <b>Ferey</b> :\n\n▪️ <b>الشواغر</b> في بدء التشغيل\n▪️ المسابقات <b>والأحداث</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> проекта <b>Ferey</b>:\n\n▪️<b>вакансии</b> нашего стартапа\n▪️конкурсы и <b>мероприятия</b>\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the <b>Ferey</b> проекта :\n\n▪️ <b>vacancies</b> of our startup\n▪️ contests and <b>events</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del проекта <b>Ferey</b> :\n\n▪️ <b>vacantes</b> de nuestra startup\n▪️ concursos y <b>eventos</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du проекта <b>Ferey</b> :\n\n▪️ <b>offres d&#x27;emploi</b> de notre startup\n▪️ concours et <b>événements</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到<b>Ferey</b> проекта的<i>登陆机器人</i>：\n\n▪️ 我们初创公司的<b>职位空缺</b>\n▪️ 竞赛和<b>活动</b>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> проекта <b>Ferey</b> :\n\n▪️ <b>الشواغر</b> في بدء التشغيل\n▪️ المسابقات <b>والأحداث</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
 }
 l_subscribe_work = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -1175,20 +1175,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_ai_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для <code>генерации</code> контента:\n\n▪️<b>текст</b>\n▪️<b>изображение</b>\n▪️<b>анализ Telegram-канала</b>\n▪️<b>распознавание</b> речи\n▪️<b>очистка истории</b> /start\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to the content <code>генерации</code> <i>landing bot</i> :\n\n▪️ <b>text</b>\n▪️ <b>image</b>\n▪️ <b>analysis of the Telegram channel</b>\n\n❗️ you can also order the development of a chat bot in our studio Ferey",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>генерации</code> de contenido :\n\n▪️ <b>texto</b>\n▪️ <b>imagen</b>\n▪️ <b>análisis del canal de Telegram</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> <code>генерации</code> de contenu :\n\n▪️ <b>texte</b>\n▪️ <b>image</b>\n▪️ <b>analyse de la chaîne Telegram</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎使用内容<code>генерации</code><i>登陆机器人</i>：\n\n▪️<b>文字</b>\n▪️<b>图片</b>\n▪️ <b>Telegram 频道分析</b>\n\n❗️ 您也可以在我们的工作室Ferey订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت إنشاء</i> <code>генерации</code> :\n\n▪️ <b>نص</b>\n▪️ <b>صورة</b>\n▪️ <b>تحليل قناة Telegram</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для генерации контента:\n\n▪️<b>текст/изображение</b>\n▪️<b>анализ @telegram-канала</b>\n▪️<b>распознавание</b> речи\n▪️<b>очистка ⁰истории</b> /start\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to the content генерации <i>landing bot</i> :\n\n▪️ <b>text</b>\n▪️ <b>image</b>\n▪️ <b>analysis of the Telegram channel</b>\n\n❗️ you can also order the development of a chat bot in our studio Ferey",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> генерации de contenido :\n\n▪️ <b>texto</b>\n▪️ <b>imagen</b>\n▪️ <b>análisis del canal de Telegram</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> генерации de contenu :\n\n▪️ <b>texte</b>\n▪️ <b>image</b>\n▪️ <b>analyse de la chaîne Telegram</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎使用内容генерации<i>登陆机器人</i>：\n\n▪️<b>文字</b>\n▪️<b>图片</b>\n▪️ <b>Telegram 频道分析</b>\n\n❗️ 您也可以在我们的工作室Ferey订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت إنشاء</i> генерации :\n\n▪️ <b>نص</b>\n▪️ <b>صورة</b>\n▪️ <b>تحليل قناة Telegram</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_ai = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️отсутствие <b>режима ожидания</b>\n▪️аналитика постов канала\n(<i>+финансовый потенциал</i>)\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -1208,15 +1208,15 @@
     'en': "🌌 Image",
     'es': "🌌 Imagen",
     'fr': "🌌 Image",
     'zh': "🌌 图片",
     'ar': "🌌 صورة",
 }
 l_gen_tlg = {
-    'ru': "👩🏽‍💻 Анализ Telegram-канала",
+    'ru': "👩🏽‍💻 Анализ @telegram-канала",
     'en': "👩🏽‍💻 Telegram channel analysis",
     'es': "👩🏽‍💻 Análisis de canales de Telegram",
     'fr': "👩🏽‍💻 Analyse des chaînes de télégrammes",
     'zh': "👩🏽‍💻电报频道分析",
     'ar': "👩🏽‍💻 تحليل قناة Telegram",
 }
 l_generate_main = {
@@ -1232,15 +1232,15 @@
     'en': "👩🏽‍💻 <b>Enter</b> a query for <b>{0}</b> 👇🏼..",
     'es': "👩🏽‍💻 <b>Ingrese</b> una consulta para <b>{0}</b> 👇🏼..",
     'fr': "👩🏽‍💻 <b>Entrez</b> une requête pour <b>{0}</b> 👇🏼..",
     'zh': "👩🏽‍💻<b>输入</b>查询<b>{0}</b> 👇🏼..",
     'ar': "👩🏽‍💻 <b>أدخل</b> استعلامًا عن <b>{0}</b> 👇🏼 ..",
 }
 l_generate_chn = {
-    'ru': "👩🏽‍💻 <b>Вставь</b> ссылку на Telegram канал для анализа финансовых показателей",
+    'ru': "👩🏽‍💻 <b>Вставь</b> ссылку на @telegram-канал для анализа финансовых показателей",
     'en': "👩🏽‍💻 <b>Insert</b> a link to the Telegram channel to analyze financial performance",
     'es': "👩🏽‍💻 <b>Inserta</b> un enlace al canal de Telegram para analizar el desempeño financiero",
     'fr': "👩🏽‍💻 <b>Insérez</b> un lien vers la chaîne Telegram pour analyser les performances financières",
     'zh': "👩🏽‍💻<b>插入</b>到 Telegram 频道的链接以分析财务绩效",
     'ar': "👩🏽‍💻 <b>أدخل</b> رابطًا إلى قناة Telegram لتحليل الأداء المالي",
 }
 l_generate_wait = {
@@ -1255,14 +1255,22 @@
     'ru': "👩🏽‍💻 Подожди {0}сек или оформи подписку",
     'en': "👩🏽‍💻 Wait {0}sec or subscribe",
     'es': "👩🏽‍💻 Espera {0}segundos o suscríbete",
     'fr': "👩🏽‍💻 Attendez {0}sec ou abonnez-vous",
     'zh': "👩🏽‍💻 等待 {0} 秒或订阅",
     'ar': "👩🏽‍💻 انتظر {0} ثانية أو اشترك",
 }
+l_generate_subcribe_channel = {
+    'ru': "👩🏽‍💻 Оформи подписку, чтобы узнать финансовый потенциал твоего @telegram-канала",
+    'en': "👩🏽‍💻 Wait {0}sec or subscribe",
+    'es': "👩🏽‍💻 Espera {0}segundos o suscríbete",
+    'fr': "👩🏽‍💻 Attendez {0}sec ou abonnez-vous",
+    'zh': "👩🏽‍💻 等待 {0} 秒或订阅",
+    'ar': "👩🏽‍💻 انتظر {0} ثانية أو اشترك",
+}
 l_generate_error = {
     'ru': "👩🏽‍💻 <b>Ошибка</b> генерации",
     'en': "👩🏽‍💻 Generation <b>Error</b>",
     'es': "👩🏽‍💻 <b>Error</b> de generación",
     'fr': "👩🏽‍💻 <b>Erreur</b> de génération",
     'zh': "👩🏽‍💻 生成<b>错误</b>",
     'ar': "👩🏽‍💻 <b>خطأ</b> في التوليد",
@@ -1292,24 +1300,24 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_ads_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных <code>постов</code> <b>Ferey</b>\n\n▪️️реклама во всех Ferey-ботах\n▪️️заказ рекламы на канале\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative <code>постов</code> <b>Ferey</b>\n\n▪️️advertising in all Ferey bots\n▪️️ ordering advertising on the channel\n\n❗️you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje</i> para crear <code>постов</code> creativas <b>Ferey</b>\n\n▪️️publicidad en todos los bots de Ferey\n▪️️solicitando publicidad en el canal\n\n❗️también puedes ordenar el desarrollo de un chatbot en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement</i> pour la création <code>постов</code> créatives <b>Ferey</b>\n\n▪️️publicité dans tous les bots Ferey\n▪️️commande de publicité sur la chaîne\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎来到<b>Ferey</b>创建创意<code>постов</code>的<i>登陆机器人</i>\n\n▪️️在所有 Ferey 机器人中投放广告\n▪️️ 在频道订购广告\n\n❗️您也可以在以下订购聊天机器人的开发我们的Ferey工作室",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء <code>постов</code> إبداعية <b>Ferey</b>\n\nالإعلان في جميع برامج Ferey\n▪️️ طلب الإعلانات على القناة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных постов <b>Ferey</b>\n\n▪️️реклама во всех Ferey-ботах\n▪️️заказ рекламы на канале\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative постов <b>Ferey</b>\n\n▪️️advertising in all Ferey bots\n▪️️ ordering advertising on the channel\n\n❗️you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje</i> para crear постов creativas <b>Ferey</b>\n\n▪️️publicidad en todos los bots de Ferey\n▪️️solicitando publicidad en el canal\n\n❗️también puedes ordenar el desarrollo de un chatbot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement</i> pour la création постов créatives <b>Ferey</b>\n\n▪️️publicité dans tous les bots Ferey\n▪️️commande de publicité sur la chaîne\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到<b>Ferey</b>创建创意постов的<i>登陆机器人</i>\n\n▪️️在所有 Ferey 机器人中投放广告\n▪️️ 在频道订购广告\n\n❗️您也可以在以下订购聊天机器人的开发我们的Ferey工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء постов إبداعية <b>Ferey</b>\n\nالإعلان في جميع برامج Ferey\n▪️️ طلب الإعلانات على القناة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_ads = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [Донат на баланс]:\n▪️возможность сделать рассылку в боте\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️рассылка по всем ботам\n▪️редактирование чаевых\n(<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️возможность сделать рассылку по всем ботам\n▪️измените значение чаевых (<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 
 l_post_media_ads = {
@@ -1337,20 +1345,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_post_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных <code>постов</code> <b>Ferey</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>уведомления</b> о нажатиях\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative <code>постов</code> <b>Ferey</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> para crear <code>постов</code> creativas <b>Ferey</b>\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> pour créer <code>постов</code> créatifs <b>Ferey</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎使用<b>Ferey</b>创建创意<code>постов</code>的<i>登陆机器人</i>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء <code>постов</code> إبداعية <b>Ferey</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> для создания креативных постов <b>Ferey</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>уведомления</b> о нажатиях\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> for creating creative постов <b>Ferey</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> para crear постов creativas <b>Ferey</b>\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> pour créer постов créatifs <b>Ferey</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎使用<b>Ferey</b>创建创意постов的<i>登陆机器人</i>\n\n❗️ 您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> لإنشاء постов إبداعية <b>Ferey</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_post = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>уведомления</b> о нажатиях\n(<i>ссылка на пользователя</i>)\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -1427,20 +1435,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_tools_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> Telegram-<code>инструментов</code>:\n\n▪️<b>преобразование</b> контента\n▪️<b>получение</b> информации о сообщ\n▪️<b>удаление</b> фона\n▪️<b>конвертация</b> в телескопы\n▪️<b>сообщение</b> 0-длины\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> of Telegram <code>инструментов</code> :\n\n▪️ content <b>conversion</b>\n▪️ <b>getting</b> information about the message\n\n❗️you can also order the development of a chat bot in our studio Ferey",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> de <code>инструментов</code> de Telegram:\n\n▪️ <b>conversión</b> de contenido\n▪️ <b>obtener</b> información sobre el mensaje\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> des <code>инструментов</code> Telegram :\n\n▪️ <b>conversion</b> de contenu\n▪️ <b>obtenir</b> des informations sur le message\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎使用 Telegram <code>инструментов</code>的<i>登陆机器人</i>：\n\n▪️ 内容<b>转换</b>\n▪️<b>获取</b>有关消息的信息\n\n❗️您也可以在我们的工作室Ferey订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص <code>инструментов</code> Telegram:\n\n▪️ <b>تحويل</b> المحتوى\n▪️ <b>الحصول على</b> معلومات حول الرسالة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> Telegram-инструментов:\n\n▪️<b>преобразование</b> контента\n▪️<b>получение</b> информации о сообщ\n▪️<b>удаление</b> фона\n▪️<b>конвертация</b> в телескопы\n▪️<b>сообщение</b> 0-длины\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> of Telegram инструментов :\n\n▪️ content <b>conversion</b>\n▪️ <b>getting</b> information about the message\n\n❗️you can also order the development of a chat bot in our studio Ferey",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> de инструментов de Telegram:\n\n▪️ <b>conversión</b> de contenido\n▪️ <b>obtener</b> información sobre el mensaje\n\n❗️también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> des инструментов Telegram :\n\n▪️ <b>conversion</b> de contenu\n▪️ <b>obtenir</b> des informations sur le message\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎使用 Telegram инструментов的<i>登陆机器人</i>：\n\n▪️ 内容<b>转换</b>\n▪️<b>获取</b>有关消息的信息\n\n❗️您也可以在我们的工作室Ferey订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص инструментов Telegram:\n\n▪️ <b>تحويل</b> المحتوى\n▪️ <b>الحصول على</b> معلومات حول الرسالة\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_tools = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -1973,20 +1981,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_media_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>медиа</code>-заметок:\n\n▪️<b>стикеры</b> из текста и фото\n▪️<b>аудио-тренды</b>\n▪️<b>видео-заметки</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>кнопочные</b> премиум-заметки\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot of</i> <code>медиа</code> notes:\n\n▪️ <b>stickers</b> from text and photos\n▪️ <b>audio sounds</b>\n▪️ <b>video notes</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje de</i> notas <code>медиа</code> :\n\n▪️ <b>pegatinas</b> de texto y fotos\n▪️ <b>sonidos de audio</b>\n▪️ <b>notas de video</b>\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement des</i> notes <code>медиа</code> :\n\n▪️ <b>autocollants</b> à partir de textes et de photos\n▪️ <b>sons audio</b>\n▪️ <b>notes vidéo</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
-    'zh': "🌱 {0}，欢迎来到<code>медиа</code>笔记<i>的登陆机器人</i>：\n\n▪️文字和照片的<b>贴纸</b>\n▪️<b>音频声音</b>\n▪️<b>视频笔记</b>\n\n❗️您也可以在我们的Ferey工作室",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الأساسي</i> لملاحظات <code>медиа</code> :\n\n▪️ <b>ملصقات</b> من النصوص والصور\n▪️ <b>الأصوات الصوتية</b>\n▪️ <b>ملاحظات الفيديو</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت الدردشة في استوديو Ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> медиа-заметок:\n\n▪️<b>стикеры</b> из текста и фото\n▪️<b>аудио-тренды</b>\n▪️<b>видео-заметки</b>\n▪️инлайн-<b>телескопы</b>\n▪️<b>кнопочные</b> премиум-заметки\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot of</i> медиа notes:\n\n▪️ <b>stickers</b> from text and photos\n▪️ <b>audio sounds</b>\n▪️ <b>video notes</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido <i>al bot de aterrizaje de</i> notas медиа :\n\n▪️ <b>pegatinas</b> de texto y fotos\n▪️ <b>sonidos de audio</b>\n▪️ <b>notas de video</b>\n\n❗️ también puedes solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans <i>le bot de débarquement des</i> notes медиа :\n\n▪️ <b>autocollants</b> à partir de textes et de photos\n▪️ <b>sons audio</b>\n▪️ <b>notes vidéo</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到медиа笔记<i>的登陆机器人</i>：\n\n▪️文字和照片的<b>贴纸</b>\n▪️<b>音频声音</b>\n▪️<b>视频笔记</b>\n\n❗️您也可以在我们的Ferey工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الأساسي</i> لملاحظات медиа :\n\n▪️ <b>ملصقات</b> من النصوص والصور\n▪️ <b>الأصوات الصوتية</b>\n▪️ <b>ملاحظات الفيديو</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت الدردشة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_media = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>кнопочные</b> премиум-заметки\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -2038,28 +2046,28 @@
     'en': "👩🏽‍💻 1/2. <b>Attach</b> audio/video, text/photo content to create a media note",
     'es': "👩🏽‍💻 1/2. <b>Adjunte</b> contenido de audio/video, texto/foto para crear una nota multimedia",
     'fr': "👩🏽‍💻 1/2. <b>Joignez</b> du contenu audio/vidéo, texte/photo pour créer une note multimédia",
     'zh': "👩🏽‍💻 1/2。<b>附加</b>音频/视频、文本/照片内容以创建媒体说明",
     'ar': "👩🏽‍💻 1/2. <b>قم بإرفاق</b> محتوى صوت / فيديو ونص / صورة لإنشاء ملاحظة وسائط",
 }
 l_media_title1 = {
-    'ru': "👩🏽‍💻 2/2. <b>Введи</b> <code>ключевые_слова</code> для твоей media-заметки\n[изменить <code>ключевые_слова</code> нельзя]",
-    'en': "👩🏽‍💻 2/2. <b>Enter</b> <code>ключевые_слова</code> for your media note\n[<code>ключевые_слова</code> cannot be changed]",
-    'es': "👩🏽‍💻 2/2. <b>Ingrese</b> <code>ключевые_слова</code> para su nota de prensa\n[<code>ключевые_слова</code> no se pueden cambiar]",
-    'fr': "👩🏽‍💻 2/2. <b>Saisissez</b> <code>ключевые_слова</code> pour votre note média\n[<code>ключевые_слова</code> ne peuvent pas être modifiés]",
-    'zh': "👩🏽‍💻 2/2。为您的媒体说明<b>输入</b><code>ключевые_слова</code>\n[无法更改<code>ключевые_слова</code>]",
-    'ar': "👩🏽‍💻 2/2. <b>أدخل</b> <code>ключевые_слова</code> لملاحظتك الإعلامية\n[لا يمكن تغيير <code>ключевые_слова</code>]",
+    'ru': "👩🏽‍💻 2/2. <b>Введи</b> ключевые_слова для твоей media-заметки\n[изменить ключевые_слова нельзя]",
+    'en': "👩🏽‍💻 2/2. <b>Enter</b> ключевые_слова for your media note\n[ключевые_слова cannot be changed]",
+    'es': "👩🏽‍💻 2/2. <b>Ingrese</b> ключевые_слова para su nota de prensa\n[ключевые_слова no se pueden cambiar]",
+    'fr': "👩🏽‍💻 2/2. <b>Saisissez</b> ключевые_слова pour votre note média\n[ключевые_слова ne peuvent pas être modifiés]",
+    'zh': "👩🏽‍💻 2/2。为您的媒体说明<b>输入</b>ключевые_слова\n[无法更改ключевые_слова]",
+    'ar': "👩🏽‍💻 2/2. <b>أدخل</b> ключевые_слова لملاحظتك الإعلامية\n[لا يمكن تغيير ключевые_слова]",
 }
 l_media_title2 = {
-    'ru': "👩🏽‍💻 2/2. <b>Текущие</b> <code>ключевые_слова</code> для твоей media-заметки\n\n{0}\n\n[пришли новые или нажми {1}]",
-    'en': "👩🏽‍💻 2/2. <b>Current</b> <code>ключевые_слова</code> for your media note\n\n{0}\n\n[new ones come in or press {1}]",
-    'es': "👩🏽‍💻 2/2. <code>ключевые_слова</code> <b>actuales</b> para su nota de prensa\n\n{0}\n\n[nuevas ingrese o presione {1}]",
-    'fr': "👩🏽‍💻 2/2. <code>ключевые_слова</code> <b>actuels</b> pour votre note multimédia\n\n{0}\n\n[les nouveaux arrivent ou appuyez sur {1}]",
-    'zh': "👩🏽‍💻 2/2。您的媒体说明的<b>当前</b><code>ключевые_слова</code>\n\n{0}\n\n[请输入新关键字或按 {1}]",
-    'ar': "👩🏽‍💻 2/2. <code>ключевые_слова</code> <b>الحالية</b> لملاحظة الوسائط الخاصة بك\n\n{0}\n\n[يتم إدخال كلمات رئيسية جديدة أو الضغط على {1}]",
+    'ru': "👩🏽‍💻 2/2. <b>Текущие</b> ключевые_слова для твоей media-заметки\n\n{0}\n\n[пришли новые или нажми {1}]",
+    'en': "👩🏽‍💻 2/2. <b>Current</b> ключевые_слова for your media note\n\n{0}\n\n[new ones come in or press {1}]",
+    'es': "👩🏽‍💻 2/2. ключевые_слова <b>actuales</b> para su nota de prensa\n\n{0}\n\n[nuevas ingrese o presione {1}]",
+    'fr': "👩🏽‍💻 2/2. ключевые_слова <b>actuels</b> pour votre note multimédia\n\n{0}\n\n[les nouveaux arrivent ou appuyez sur {1}]",
+    'zh': "👩🏽‍💻 2/2。您的媒体说明的<b>当前</b>ключевые_слова\n\n{0}\n\n[请输入新关键字或按 {1}]",
+    'ar': "👩🏽‍💻 2/2. ключевые_слова <b>الحالية</b> لملاحظة الوسائط الخاصة بك\n\n{0}\n\n[يتم إدخال كلمات رئيسية جديدة أو الضغط على {1}]",
 }
 l_media_confirm = {
     'ru': "🏁 Завершить",
     'en': "🏁 Complete",
     'es': "🏁 Completa",
     'fr': "🏁 Complet",
     'zh': "🏁 完成",
@@ -2146,20 +2154,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_find_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>поиска</code> в <b>Telegram</b>:\n\n▪️<b>top</b> каналы/группы\n▪️<b>vip</b> пользователи/боты\n▪️<b>гео</b> парсинг\n▪️<b>пассивный</b> маркетинг\n\n❗️также можно заказать разработку Telegram-продвижения в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
-    'en': "🌱 {0}, welcome to <b>Telegram</b> <code>поиска</code> <i>landing bot</i> :\n\n▪️ <b>top</b> channels/groups\n▪️ <b>vip</b> users/bots\n▪️ <b>geo</b> parsing\n▪️ <b>passive</b> marketing\n\n❗️ you can also order development Telegram promotions in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>поиска</code> <b>de Telegram</b> :\n\n▪️ canales/grupos <b>principales</b>\n▪️ usuarios <b>vip</b> /bots\n▪️ análisis <b>geográfico</b>\n▪️ marketing <b>pasivo</b>\n\n❗️ también puedes solicitar promociones de desarrollo de Telegram en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue sur <b>Telegram</b> <code>поиска</code> <i>landing bot</i> :\n\n▪️ <b>meilleurs</b> canaux/groupes\n▪️ utilisateurs/bots <b>vip</b>\n▪️ analyse <b>géographique</b>\n▪️ marketing <b>passif</b>\n\n❗️ vous pouvez également commander des promotions de développement Telegram dans notre atelier de Ferey",
-    'zh': "🌱 {0}，欢迎使用<b>Telegram</b> <code>поиска</code><i>登陆机器人</i>：\n\n▪️<b>热门</b>频道/群组\n▪️ <b>vip</b>用户/机器人\n▪️<b>地理</b>解析\n▪️<b>被动</b>营销\n\n❗️ 您也可以订购开发 Telegram 促销在我们的Ferey工作室",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوطي</i> <code>поиска</code> <b>Telegram</b> :\n\n▪️ <b>أفضل</b> القنوات / المجموعات\n▪️ مستخدمين / برامج تتبع <b>لكبار</b> الشخصيات\n▪️ تحليل <b>جغرافي</b>\n▪️ تسويق <b>سلبي</b>\n\n❗️ يمكنك أيضًا طلب ترويجات Telegram للتطوير في استوديو Ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> поиска в <b>Telegram</b>:\n\n▪️<b>top</b> каналы/группы\n▪️<b>vip</b> пользователи/боты\n▪️<b>гео</b> парсинг\n▪️<b>пассивный</b> маркетинг\n\n❗️также можно заказать разработку Telegram-продвижения в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <b>Telegram</b> поиска <i>landing bot</i> :\n\n▪️ <b>top</b> channels/groups\n▪️ <b>vip</b> users/bots\n▪️ <b>geo</b> parsing\n▪️ <b>passive</b> marketing\n\n❗️ you can also order development Telegram promotions in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> поиска <b>de Telegram</b> :\n\n▪️ canales/grupos <b>principales</b>\n▪️ usuarios <b>vip</b> /bots\n▪️ análisis <b>geográfico</b>\n▪️ marketing <b>pasivo</b>\n\n❗️ también puedes solicitar promociones de desarrollo de Telegram en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <b>Telegram</b> поиска <i>landing bot</i> :\n\n▪️ <b>meilleurs</b> canaux/groupes\n▪️ utilisateurs/bots <b>vip</b>\n▪️ analyse <b>géographique</b>\n▪️ marketing <b>passif</b>\n\n❗️ vous pouvez également commander des promotions de développement Telegram dans notre atelier de Ferey",
+    'zh': "🌱 {0}，欢迎使用<b>Telegram</b> поиска<i>登陆机器人</i>：\n\n▪️<b>热门</b>频道/群组\n▪️ <b>vip</b>用户/机器人\n▪️<b>地理</b>解析\n▪️<b>被动</b>营销\n\n❗️ 您也可以订购开发 Telegram 促销在我们的Ferey工作室",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوطي</i> поиска <b>Telegram</b> :\n\n▪️ <b>أفضل</b> القنوات / المجموعات\n▪️ مستخدمين / برامج تتبع <b>لكبار</b> الشخصيات\n▪️ تحليل <b>جغرافي</b>\n▪️ تسويق <b>سلبي</b>\n\n❗️ يمكنك أيضًا طلب ترويجات Telegram للتطوير في استوديو Ferey الخاص بنا",
 }
 l_subscribe_find = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>уведомления</b> об услуге\n(<i>ссылка на сообщение</i>)\n▪️<b>приоритетная</b> выдача при поиске\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -2643,20 +2651,20 @@
     'en': "🔎 View",
     'es': "🔎 Ver",
     'fr': "🔎 Voir",
     'zh': "🔎 查看",
     'ar': "🔎 عرض",
 }
 l_add_text = {
-    'ru': "🔎 <b>Добавь</b> свой канал/группу/пользователя/бота в базу командой: <code>/add ССЫЛКА</code>\n\n👩🏽‍💻 Условия: наличие аватара и @username/ссылки (+ для канала/группы > 100 участников + последнее сообщение < 100 дней назад + для бота и пользователя наличие описания)",
-    'en': "🔎 Add your channel/group/user/bot to the database with the command: <code>/add ССЫЛКА</code>\n\n👩🏽‍💻 Conditions: availability of an avatar and @username /link (+ for channel/group > 100 members + last message < 100 days ago + for the bot and the user, the presence of a description)",
-    'es': "🔎 Agregue su canal/grupo/usuario/bot a la base de datos con el comando: <code>/add ССЫЛКА</code>\n\n👩🏽‍💻 Condiciones: disponibilidad de un avatar y @username /link (+ para canal/grupo > 100 miembros + último mensaje < hace 100 días + para el bot y el usuario, la presencia de una descripción)",
-    'fr': "🔎 Ajoutez votre chaîne/groupe/utilisateur/bot à la base de données avec la commande : <code>/add ССЫЛКА</code>\n\n👩🏽‍💻 Conditions : disponibilité d'un avatar et @username /link (+ pour chaîne/groupe > 100 membres + dernier message il y a < 100 jours + pour le bot et l'utilisateur, la présence d'une description)",
-    'zh': "🔎 使用以下命令将您的频道/组/用户/机器人添加到数据库： <code>/add ССЫЛКА</code>\n\n👩🏽‍💻 条件：头像和@username /link 的可用性（+ 对于频道/组 > 100 个成员 + 最后一个消息 < 100 天前 + 对于机器人和用户，存在描述）",
-    'ar': "🔎 أضف قناتك / مجموعتك / مستخدم / بوت إلى قاعدة البيانات بالأمر: <code>/add ССЫЛКА</code>\n\n👩🏽‍💻 الشروط: توفر الصورة الرمزية و @username / الرابط (+ للقناة / المجموعة> 100 عضو + الأخير رسالة <100 يوم مضت + للبوت والمستخدم ، وجود وصف)",
+    'ru': "🔎 <b>Добавь</b> свой канал/группу/пользователя/бота в базу командой: /add ССЫЛКА\n\n👩🏽‍💻 Условия: наличие аватара и @username/ссылки (+ для канала/группы > 100 участников + последнее сообщение < 100 дней назад + для бота и пользователя наличие описания)",
+    'en': "🔎 Add your channel/group/user/bot to the database with the command: /add ССЫЛКА\n\n👩🏽‍💻 Conditions: availability of an avatar and @username /link (+ for channel/group > 100 members + last message < 100 days ago + for the bot and the user, the presence of a description)",
+    'es': "🔎 Agregue su canal/grupo/usuario/bot a la base de datos con el comando: /add ССЫЛКА\n\n👩🏽‍💻 Condiciones: disponibilidad de un avatar y @username /link (+ para canal/grupo > 100 miembros + último mensaje < hace 100 días + para el bot y el usuario, la presencia de una descripción)",
+    'fr': "🔎 Ajoutez votre chaîne/groupe/utilisateur/bot à la base de données avec la commande : /add ССЫЛКА\n\n👩🏽‍💻 Conditions : disponibilité d'un avatar et @username /link (+ pour chaîne/groupe > 100 membres + dernier message il y a < 100 jours + pour le bot et l'utilisateur, la présence d'une description)",
+    'zh': "🔎 使用以下命令将您的频道/组/用户/机器人添加到数据库： /add ССЫЛКА\n\n👩🏽‍💻 条件：头像和@username /link 的可用性（+ 对于频道/组 > 100 个成员 + 最后一个消息 < 100 天前 + 对于机器人和用户，存在描述）",
+    'ar': "🔎 أضف قناتك / مجموعتك / مستخدم / بوت إلى قاعدة البيانات بالأمر: /add ССЫЛКА\n\n👩🏽‍💻 الشروط: توفر الصورة الرمزية و @username / الرابط (+ للقناة / المجموعة> 100 عضو + الأخير رسالة <100 يوم مضت + للبوت والمستخدم ، وجود وصف)",
 }
 l_add_join_err = {
     'ru': "🚫 <b>Добавить</b> в базу {0} не удалось, необходимо открыть свободный доступ для присоединения",
     'en': "🚫 Failed to add {0} to the database, you need to open free access to join",
     'es': "🚫 No se pudo agregar {0} a la base de datos, debe abrir el acceso gratuito para unirse",
     'fr': "🚫 Échec de l'ajout de {0} à la base de données, vous devez ouvrir un accès gratuit pour rejoindre",
     'zh': "🚫 添加{0}到数据库失败，需要开通免费权限才能加入",
@@ -2944,20 +2952,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_chn_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>администрирования</code> <b>Telegram</b>-каналов:\n\n▪️<b>защита</b> канала от вступления шпионов\n▪️<b>организация</b> бана и антифлуда\n▪️<b>сбор</b> подписчиков\n▪️<b>счетчик</b> нажатий\n▪️<b>реакции</b> и просмотры\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to the <b>Telegram</b> channel <code>администрирования</code> <i>landing bot</i> :\n\n▪️ <b>protection</b> of the channel from spyware entry\n▪️display <b>of statistics</b> and engagement (%)\n▪️restriction of rights before <b>subscribing</b> to the channel\n▪️ <b>organization</b> of a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>администрирования</code> de canales <b>de Telegram</b> :\n\ <b>n▪️protección</b> del canal contra la entrada de software espía\n▪️visualización <b>de estadísticas</b> e interacción (%)\n▪️restricción de derechos antes de <b>suscribirse</b> al canal\n▪️ <b>organización</b> de una prohibición y anti-inundación\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> <code>администрирования</code> de la chaîne <b>Telegram</b> :\n\n▪️ <b>protection</b> de la chaîne contre l&#x27;entrée de logiciels espions\n▪️affichage <b>des statistiques</b> et de l&#x27;engagement (%)\n▪️restriction des droits avant de <b>s&#x27;abonner</b> à la chaîne\n<b>▪️organisation</b> d'une interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
-    'zh': "🌱 {0}，欢迎使用<b>Telegram</b>频道<code>администрирования</code><i>登陆机器人</i>：\n\n▪️<b>保护</b>频道免受间谍软件入侵\n▪️ 显示<b>统计信息</b>和参与度 (%)\n▪️<b>订阅</b>频道前的权利限制\n▪️<b>组织</b>禁令和反洪水\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت</i> <code>администрирования</code> قناة <b>Telegram</b> :\n\n▪️ <b>حماية</b> القناة من إدخال برامج التجسس\n▪️ <b>عرض الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> حظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> администрирования <b>Telegram</b>-каналов:\n\n▪️<b>защита</b> канала от вступления шпионов\n▪️<b>организация</b> бана и антифлуда\n▪️<b>сбор</b> подписчиков\n▪️<b>счетчик</b> нажатий\n▪️<b>реакции</b> и просмотры\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to the <b>Telegram</b> channel администрирования <i>landing bot</i> :\n\n▪️ <b>protection</b> of the channel from spyware entry\n▪️display <b>of statistics</b> and engagement (%)\n▪️restriction of rights before <b>subscribing</b> to the channel\n▪️ <b>organization</b> of a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> администрирования de canales <b>de Telegram</b> :\n\ <b>n▪️protección</b> del canal contra la entrada de software espía\n▪️visualización <b>de estadísticas</b> e interacción (%)\n▪️restricción de derechos antes de <b>suscribirse</b> al canal\n▪️ <b>organización</b> de una prohibición y anti-inundación\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans le <i>landing bot</i> администрирования de la chaîne <b>Telegram</b> :\n\n▪️ <b>protection</b> de la chaîne contre l&#x27;entrée de logiciels espions\n▪️affichage <b>des statistiques</b> et de l&#x27;engagement (%)\n▪️restriction des droits avant de <b>s&#x27;abonner</b> à la chaîne\n<b>▪️organisation</b> d'une interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
+    'zh': "🌱 {0}，欢迎使用<b>Telegram</b>频道администрирования<i>登陆机器人</i>：\n\n▪️<b>保护</b>频道免受间谍软件入侵\n▪️ 显示<b>统计信息</b>和参与度 (%)\n▪️<b>订阅</b>频道前的权利限制\n▪️<b>组织</b>禁令和反洪水\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت</i> администрирования قناة <b>Telegram</b> :\n\n▪️ <b>حماية</b> القناة من إدخال برامج التجسس\n▪️ <b>عرض الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> حظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_channel= {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>реакции</b> и просмотры\n▪️<b>выгрузка</b> базы пользователей\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -2985,20 +2993,20 @@
     'en': "➕ Add channel",
     'es': "➕ Agregar canal",
     'fr': "➕ Ajouter une chaîne",
     'zh': "➕ 添加频道",
     'ar': "➕ إضافة قناة",
 }
 l_bot_removed = {
-    'ru': "🚫 @{0}-бот удален из <b>{1}</b> (<code>{2}</code>)",
-    'en': "🚫 @{0}-bot removed from <b>{1}</b> ( <code>{2}</code> )",
-    'es': "🚫 @{0}-bot eliminado de <b>{1}</b> ( <code>{2}</code> )",
-    'fr': "🚫 @{0}-bot supprimé de <b>{1}</b> ( <code>{2}</code> )",
-    'zh': "🚫 @{0}-bot 从<b>{1}</b> ( <code>{2}</code> ) 中移除",
-    'ar': "🚫 @ {0} -إزالة الروبوت من <b>{1}</b> ( <code>{2}</code> )",
+    'ru': "🚫 @{0}-бот удален из <b>{1}</b> ({2})",
+    'en': "🚫 @{0}-bot removed from <b>{1}</b> ( {2} )",
+    'es': "🚫 @{0}-bot eliminado de <b>{1}</b> ( {2} )",
+    'fr': "🚫 @{0}-bot supprimé de <b>{1}</b> ( {2} )",
+    'zh': "🚫 @{0}-bot 从<b>{1}</b> ( {2} ) 中移除",
+    'ar': "🚫 @ {0} -إزالة الروبوت من <b>{1}</b> ( {2} )",
 }
 
 l_chn_config = {
     ("cban", "🕵🏽", "☑"): {
         'ru': "Авто-бан",
         'en': "Auto-ban",
         'es': "Prohibición automática",
@@ -3084,20 +3092,20 @@
     'en': "⚙️ <b>Select</b> option for /cmd <i>settings</i> [<b>{0}</b>] {1}",
     'es': "⚙️ <b>Seleccione</b> la opción para <i>la configuración de</i> /cmd [<b>{0}</b>] {1}",
     'fr': "⚙️ <b>Sélectionnez</b> l&#x27;option pour <i>les paramètres</i> /cmd [<b>{0}</b>] {1}",
     'zh': "⚙️<b>选择</b>/cmd<i>设置</i>选项 [<b>{0}</b>] {1}",
     'ar': "⚙️ <b>تحديد</b> خيار <i>إعدادات</i> / cmd [<b>{0}</b>] {1}",
 }
 l_chat_join_request_handler = {
-    'ru': "👮🏽 {0}, ты отправил(а) заявку на вступление в <b>{1}</b>\n\n👉🏼 <b>Выбери</b> <i>правильный вариант</i> в соответствии с <code>заданием</code> на картинке, чтобы твоя <i>заявка</i> на вступление была <b>одобрена</b>",
-    'en': "👮🏽 {0}, you submitted an application to join <b>{1}</b>\n\n👉🏼 <b>Choose</b> <i>the correct option</i> according to <code>заданием</code> in the picture so that your <i>application</i> to join is <b>approved</b>",
-    'es': "👮🏽 {0}, envió una solicitud para unirse <b>{1}</b>\n\n👉🏼 <b>Elija</b> <i>la opción correcta</i> de acuerdo con <code>заданием</code> en la imagen para que se <b>apruebe</b> su <i>solicitud</i> para unirse",
-    'fr': "👮🏽 {0}, vous avez soumis une candidature pour rejoindre <b>{1}</b>\n\n👉🏼 <b>Choisissez</b> <i>la bonne option</i> en fonction de <code>заданием</code> dans l&#x27;image afin que votre <i>candidature</i> soit <b>approuvée</b>",
-    'zh': "👮🏽 {0}，你提交了加入<b>{1}</b>的申请\n\n👉🏼 根据图片中的<code>заданием</code><b>选择</b><i>正确的选项</i>，这样你的加入<i>申请</i>就<b>通过了</b>",
-    'ar': "👮🏽 {0} ، لقد قدمت طلبًا للانضمام <b>{1}</b>\n\n👉🏼 <b>اختر</b> <i>الخيار الصحيح</i> وفقًا <code>заданием</code> الموجودة في الصورة حتى تتم <b>الموافقة على</b> <i>طلبك</i> للانضمام",
+    'ru': "👮🏽 {0}, ты отправил(а) заявку на вступление в <b>{1}</b>\n\n👉🏼 <b>Выбери</b> <i>правильный вариант</i> в соответствии с заданием на картинке, чтобы твоя <i>заявка</i> на вступление была <b>одобрена</b>",
+    'en': "👮🏽 {0}, you submitted an application to join <b>{1}</b>\n\n👉🏼 <b>Choose</b> <i>the correct option</i> according to заданием in the picture so that your <i>application</i> to join is <b>approved</b>",
+    'es': "👮🏽 {0}, envió una solicitud para unirse <b>{1}</b>\n\n👉🏼 <b>Elija</b> <i>la opción correcta</i> de acuerdo con заданием en la imagen para que se <b>apruebe</b> su <i>solicitud</i> para unirse",
+    'fr': "👮🏽 {0}, vous avez soumis une candidature pour rejoindre <b>{1}</b>\n\n👉🏼 <b>Choisissez</b> <i>la bonne option</i> en fonction de заданием dans l&#x27;image afin que votre <i>candidature</i> soit <b>approuvée</b>",
+    'zh': "👮🏽 {0}，你提交了加入<b>{1}</b>的申请\n\n👉🏼 根据图片中的заданием<b>选择</b><i>正确的选项</i>，这样你的加入<i>申请</i>就<b>通过了</b>",
+    'ar': "👮🏽 {0} ، لقد قدمت طلبًا للانضمام <b>{1}</b>\n\n👉🏼 <b>اختر</b> <i>الخيار الصحيح</i> وفقًا заданием الموجودة في الصورة حتى تتم <b>الموافقة على</b> <i>طلبك</i> للانضمام",
 }
 l_content_types_sub_button = {
     'ru': "👮🏽 Я подписался",
     'en': "👮🏽 I subscribed",
     'es': "👮🏽 me suscribí",
     'fr': "👮🏽 je me suis abonné",
     'zh': "👮🏽 我订阅了",
@@ -3168,44 +3176,44 @@
     'fr': "👮🏽 Pour <i>vérifier l&#x27;abonnement,</i> vous devez ajouter une chaîne avec la commande :\n\n/channel LIEN VERS LA CHAÎNE",
     'zh': "👮🏽 要<i>查看订阅，</i>您需要使用以下命令添加频道：\n\n/channel LINK TO THE CHANNEL",
     'ar': "👮🏽 <i>للتحقق من الاشتراك ،</i> تحتاج إلى إضافة قناة باستخدام الأمر:\n\n/ channel LINK TO THE CHANNEL",
 }
 
 # region commands
 l_update_text = {
-    'ru': "👩🏽‍💻 <b>Данные</b> о канале успешно обновлены:\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Команды</b> /cmd",
-    'en': "👩🏽‍💻 Channel <b>data</b> successfully updated:\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Commands</b> /cmd",
-    'es': "👩🏽‍💻 <b>Datos</b> del canal actualizados con éxito:\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Comandos</b> /cmd",
-    'fr': "👩🏽‍💻 <b>Les données</b> de la chaîne ont été mises à jour :\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Commandes</b> /cmd",
-    'zh': "👩🏽‍💻 频道<b>数据</b>成功更新：\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️<b>命令</b>/cmd",
-    'ar': "👩🏽‍💻 تم تحديث <b>بيانات</b> القناة بنجاح:\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>الأوامر</b> / cmd",
+    'ru': "👩🏽‍💻 <b>Данные</b> о канале успешно обновлены:\n\n<b>{0}</b> [{1}]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Команды</b> /cmd",
+    'en': "👩🏽‍💻 Channel <b>data</b> successfully updated:\n\n<b>{0}</b> [{1}]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Commands</b> /cmd",
+    'es': "👩🏽‍💻 <b>Datos</b> del canal actualizados con éxito:\n\n<b>{0}</b> [{1}]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Comandos</b> /cmd",
+    'fr': "👩🏽‍💻 <b>Les données</b> de la chaîne ont été mises à jour :\n\n<b>{0}</b> [{1}]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Commandes</b> /cmd",
+    'zh': "👩🏽‍💻 频道<b>数据</b>成功更新：\n\n<b>{0}</b> [{1}]\n{2}\n<i>{3}</i>\n\n⚙️<b>命令</b>/cmd",
+    'ar': "👩🏽‍💻 تم تحديث <b>بيانات</b> القناة بنجاح:\n\n<b>{0}</b> [{1}]\n{2}\n<i>{3}</i>\n\n⚙️ <b>الأوامر</b> / cmd",
 }
 l_chn_commands_handler = {
     'ru': "⚙️ <b>Настройка</b> канала <b>{0}</b> {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/update <i>обновление параметров</i>\n/transfer   <i>передача admin-прав</i>\n/info   <i>информация</i>\n/stat   <i>статистика</i>\n/parse  <i>выгрузка базы подписчиков</i>\n/videochat 1 1 <i>анонс видео-трансляции</i>\n/clean  <i>долгая очистка канала от deleted/scam/fake-аккаунтов, а также по 🕵🏽 Авто-бан правилам</i>\n/channel NAME   <i>добавить другой канал для проверки подписки</i>",
     'en': "⚙️ Channel <b>setup</b> <b>{0}</b> {1}\n\n<b>⛏ Admin commands @{2}</b>\n/update <i>update parameters</i>\n/transfer <i>transfer admin rights</i>\n/info <i>information</i>\n/stat <i>statistics</i>\n/parse <i>upload subscriber bases</i>\n/videochat 1 1 <i>announcement of video broadcast</i>\n/clean <i>long channel cleaning from deleted/scam/fake accounts, as well as according to 🕵🏽 Auto-ban rules</i>\n/channel NAME <i>add another channel to check subscription</i>",
     'es': "⚙️ <b>Configuración</b> del canal <b>{0}</b> {1}\n\n<b>⛏ Comandos de administrador @{2}</b>\n/actualizar <i>parámetros de actualización</i>\n/transferir <i>transferir derechos de administrador</i>\n/ <i>información</i> de información\n/ <i>estadísticas</i>\n/analizar <i>cargar bases de suscriptores</i>\n/videochat 1 1 <i>anuncio de transmisión de video</i>\n/limpie <i>la limpieza de canales largos de cuentas eliminadas/estafas/falsas, así como de acuerdo con las 🕵🏽 reglas de prohibición automática</i>\n/NOMBRE del canal <i>agregue otro canal para verificar la suscripción</i>",
     'fr': "⚙️ <b>Configuration</b> de la chaîne <b>{0}</b> {1}\n\n<b>⛏ Commandes d&#x27;administration @{2}</b>\n/update <i>update parameters</i>\n/transfer <i>transfer admin rights</i>\n/info <i>information</i>\n/stat <i>statistics</i>\n/parse <i>upload subscriber bases</i>\n/videochat 1 1 <i>annonce de la diffusion vidéo</i>\n/nettoyer <i>le nettoyage des longues chaînes des comptes supprimés/arnaques/faux, ainsi que selon les 🕵🏽 règles d&#x27;interdiction automatique</i>\n/channel NAME <i>ajouter une autre chaîne pour vérifier l&#x27;abonnement</i>",
     'zh': "⚙️ 频道<b>设置{0}</b> {1}\n\n<b>⛏ 管理员命令@{2}</b>\n/update<i>更新参数</i>\n/transfer<i>转移管理员权限</i>\n/info<i>信息</i>\n/stat<i>统计</i>\n/parse<i>上传用户群</i>\n/videochat 1 1<i>视频广播公告</i>\n/clean<i>长频道清理已删除/诈骗/假账号，以及根据🕵🏽自动封禁规则</i>\n/channel NAME<i>添加另一个频道查看订阅</i>",
     'ar': "⚙️ <b>إعداد</b> القناة <b>{0}</b> {1}\n\n<b>⛏ أوامر المسؤول @ {2}</b>\n/ <i>تحديث المعلمات</i>\n/ <i>نقل حقوق المسؤول</i>\n/ معلومات <i>المعلومات</i>\n/ <i>الإحصائيات</i> الإحصائية\n/ تحليل <i>قواعد المشتركين في التحميل</i>\n/ videochat 1 1 <i>إعلان عن بث الفيديو</i>\n/ <i>تنظيف قناة طويلة من الحسابات المحذوفة / الاحتيالية / المزيفة ، وكذلك وفقًا لقواعد 🕵🏽 الحظر التلقائي</i>\n/ <i>إضافة قناة أخرى للتحقق من الاشتراك</i>",
 }
 l_info_restrict = {
-    'ru': "<code>запрещено</code>\n",
-    'en': "<code>запрещено</code>\n",
-    'es': "<code>запрещено</code>\n",
-    'fr': "<code>запрещено</code>\n",
-    'zh': "<code>запрещено</code>\n",
-    'ar': "<code>запрещено</code>\n",
+    'ru': "запрещено\n",
+    'en': "запрещено\n",
+    'es': "запрещено\n",
+    'fr': "запрещено\n",
+    'zh': "запрещено\n",
+    'ar': "запрещено\n",
 }
 l_info_allow = {
-    'ru': "<code>разрешено</code>\n",
-    'en': "<code>разрешено</code>\n",
-    'es': "<code>разрешено</code>\n",
-    'fr': "<code>разрешено</code>\n",
-    'zh': "<code>разрешено</code>\n",
-    'ar': "<code>разрешено</code>\n",
+    'ru': "разрешено\n",
+    'en': "разрешено\n",
+    'es': "разрешено\n",
+    'fr': "разрешено\n",
+    'zh': "разрешено\n",
+    'ar': "разрешено\n",
 }
 l_info_protect = {
     'ru': "<b>Сохранение контента</b>: ",
     'en': "<b>Content saving</b> :",
     'es': "<b>Ahorro de contenido</b> :",
     'fr': "<b>Sauvegarde du contenu</b> :",
     'zh': "<b>内容保存</b>：",
@@ -3282,36 +3290,36 @@
     'en': "Invite other admins to",
     'es': "Invitar a otros administradores a",
     'fr': "Invitez d'autres administrateurs à",
     'zh': "邀请其他管理员",
     'ar': "قم بدعوة مدراء آخرين إلى",
 }
 l_chn_info_start1 = {
-    'ru': "ℹ️ <b>Общая информация о канале</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
-    'en': "ℹ️ <b>General information about the channel</b>\n\n<b>Name</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> members]{5}{6}{7}",
-    'es': "ℹ️ <b>Información general sobre el canal</b>\n\n<b>Nombre</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> miembros]{5}{6}{7}",
-    'fr': "ℹ️ <b>Informations générales sur la chaîne</b>\n\n<b>Nom</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> membres]{5}{6}{7}",
-    'zh': "ℹ️<b>有关频道的一般信息</b>\n\n<b>名称</b>：{0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u>成员]{5}{6}{7}",
-    'ar': "ℹ️ <b>معلومات عامة عن القناة</b>\n\n<b>الاسم</b> : {0} [id = <code>{1}</code> ، <i>{2} {3}</i> ، <u>{4}</u> members] {5} {6} {7}",
+    'ru': "ℹ️ <b>Общая информация о канале</b>\n\n<b>Название</b>: {0} [id={1}, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
+    'en': "ℹ️ <b>General information about the channel</b>\n\n<b>Name</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> members]{5}{6}{7}",
+    'es': "ℹ️ <b>Información general sobre el canal</b>\n\n<b>Nombre</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> miembros]{5}{6}{7}",
+    'fr': "ℹ️ <b>Informations générales sur la chaîne</b>\n\n<b>Nom</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> membres]{5}{6}{7}",
+    'zh': "ℹ️<b>有关频道的一般信息</b>\n\n<b>名称</b>：{0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u>成员]{5}{6}{7}",
+    'ar': "ℹ️ <b>معلومات عامة عن القناة</b>\n\n<b>الاسم</b> : {0} [id = {1} ، <i>{2} {3}</i> ، <u>{4}</u> members] {5} {6} {7}",
 }
 l_chn_stat_start1 = {
-    'ru': "ℹ️ <b>Общая статистика канала</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
-    'en': "ℹ️ <b>General channel statistics</b>\n\n<b>Title</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> members]{5}{6}{7}",
-    'es': "ℹ️ <b>Estadísticas generales del canal</b>\n\n<b>Nombre</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> miembros]{5}{6}{7}",
-    'fr': "ℹ️ <b>Statistiques générales de la chaîne</b>\n\n<b>Titre</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> membres]{5}{6}{7}",
-    'zh': "ℹ️<b>一般频道统计信息</b>\n\n<b>标题</b>：{0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u>成员]{5}{6}{7}",
-    'ar': "ℹ️ <b>إحصائيات القناة العامة</b>\n\n<b>العنوان</b> : {0} [id = <code>{1}</code> ، <i>{2} {3}</i> ، <u>{4}</u> members] {5} {6} {7}",
+    'ru': "ℹ️ <b>Общая статистика канала</b>\n\n<b>Название</b>: {0} [id={1}, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
+    'en': "ℹ️ <b>General channel statistics</b>\n\n<b>Title</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> members]{5}{6}{7}",
+    'es': "ℹ️ <b>Estadísticas generales del canal</b>\n\n<b>Nombre</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> miembros]{5}{6}{7}",
+    'fr': "ℹ️ <b>Statistiques générales de la chaîne</b>\n\n<b>Titre</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> membres]{5}{6}{7}",
+    'zh': "ℹ️<b>一般频道统计信息</b>\n\n<b>标题</b>：{0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u>成员]{5}{6}{7}",
+    'ar': "ℹ️ <b>إحصائيات القناة العامة</b>\n\n<b>العنوان</b> : {0} [id = {1} ، <i>{2} {3}</i> ، <u>{4}</u> members] {5} {6} {7}",
 }
 l_chn_stat_start2 = {
-    'ru': "\n<b>Ссылка</b>: {0}\n<b>Описание</b>: {1}\n<b>Привязанная группа</b>: <code>{2}</code>\n",
-    'en': "\n<b>Link</b> : {0}\n<b>Description</b> : {1}\n<b>Link Group</b> : <code>{2}</code>\n",
-    'es': "\n<b>Enlace</b> : {0}\n<b>Descripción</b> : {1}\n<b>Grupo de enlaces</b> : <code>{2}</code>\n",
-    'fr': "\n<b>Lien</b> : {0}\n<b>Description</b> : {1}\n<b>Groupe de liens</b> : <code>{2}</code>\n",
-    'zh': "\n<b>链接</b>：{0}\n<b>描述</b>：{1}\n<b>链接组</b>： <code>{2}</code>\n",
-    'ar': "\n<b>الارتباط</b> : {0}\n<b>الوصف</b> : {1}\n<b>مجموعة الروابط</b> : <code>{2}</code>\n",
+    'ru': "\n<b>Ссылка</b>: {0}\n<b>Описание</b>: {1}\n<b>Привязанная группа</b>: {2}\n",
+    'en': "\n<b>Link</b> : {0}\n<b>Description</b> : {1}\n<b>Link Group</b> : {2}\n",
+    'es': "\n<b>Enlace</b> : {0}\n<b>Descripción</b> : {1}\n<b>Grupo de enlaces</b> : {2}\n",
+    'fr': "\n<b>Lien</b> : {0}\n<b>Description</b> : {1}\n<b>Groupe de liens</b> : {2}\n",
+    'zh': "\n<b>链接</b>：{0}\n<b>描述</b>：{1}\n<b>链接组</b>： {2}\n",
+    'ar': "\n<b>الارتباط</b> : {0}\n<b>الوصف</b> : {1}\n<b>مجموعة الروابط</b> : {2}\n",
 }
 l_chn_stat_start3 = {
     'ru': "\n<b>ID последнего поста</b>: {0}\n<b>Посты</b>: {1}\n<b>Реакции</b>: {2}\n<b>Просмотры</b>: {3}\n<b>Комментарии</b>: {4}\n<b>$кэштеги</b>: {5}\n<b>#хэштеги</b>: {6}\n",
     'en': "\n<b>Last Post ID</b> : {0}\n<b>Posts</b> : {1}\n<b>Reactions</b> : {2}\n<b>Views</b> : {3}\n<b>Comments</b> : {4}\n<b>$cashtags</b> : {5}\n<b>#hashtags</b> : {6}\n",
     'es': "\n<b>ID de la última publicación</b> : {0}\n<b>Publicaciones</b> : {1}\n<b>Reacciones</b> : {2}\n<b>Vistas</b> : {3}\n<b>Comentarios</b> : {4}\n<b>$cashtags</b> : {5}\n<b>#hashtags</b> : {6}\n",
     'fr': "\n<b>ID du dernier message</b> : {0}\n<b>Messages</b> : {1}\n<b>Réactions</b> : {2}\n<b>Vues</b> : {3}\n<b>Commentaires</b> : {4}\n<b>$cashtags</b> : {5}\n<b>#hashtags</b> : {6}\n",
     'zh': "\n<b>最后的帖子 ID</b> ：{0}\n<b>帖子</b>：{1}\n<b>反应</b>：{2}\n<b>浏览量</b>：{3}\n<b>评论</b>：{4}\n<b>$cashtags</b> ：{5}\n<b>#hashtags</b> ： {6}\n",
@@ -3347,20 +3355,20 @@
     'en': "⚠️ Transfer <b>admin</b> rights to <b>{0}</b> to user {1} in @{2}-bot?",
     'es': "⚠️ ¿Transferir los derechos <b>de administrador</b> de <b>{0}</b> al usuario {1} en @{2}-bot?",
     'fr': "⚠️ Transférer les droits <b>d&#x27;administrateur</b> de <b>{0}</b> à l'utilisateur {1} dans @{2}-bot ?",
     'zh': "⚠️ 在@{2}-bot 中将<b>{0}的管理员</b>权限转让给用户 {1}？",
     'ar': "⚠️ نقل حقوق <b>المسؤول</b> إلى <b>{0}</b> إلى المستخدم {1} في @ {2} -bot؟",
 }
 l_transfer_text = {
-    'ru': "⚠️ Для передачи admin-прав канала в @{0}-боте используй команду: <code>/transfer ID-ПОЛЬЗОВАТЕЛЯ</code> (/id), где пользователь: администратор канала и участник @{0}-бота\n\n⚙️ <b>Команды</b> /cmd",
-    'en': "⚠️ To transfer channel admin rights to @{0}-bot, use the command: <code>/transfer ID-ПОЛЬЗОВАТЕЛЯ</code> (/id), where user: channel administrator and member of @{0}-bot\n\n⚙️ <b>Commands</b> /cmd",
-    'es': "⚠️ Para transferir los derechos de administrador del canal a @{0}-bot, usa el comando: <code>/transfer ID-ПОЛЬЗОВАТЕЛЯ</code> (/id), donde usuario: administrador del canal y miembro de @{0}-bot\n\n⚙️ <b>Comandos</b> /cmd",
-    'fr': "⚠️ Pour transférer les droits d'administrateur du canal à @{0}-bot, utilisez la commande : <code>/transfer ID-ПОЛЬЗОВАТЕЛЯ</code> (/id), où utilisateur : administrateur du canal et membre de @{0}-bot\n\n⚙️ <b>Commandes</b> /cmd",
-    'zh': "⚠️ 要将频道管理员权限转移给@{0}-bot，请使用命令： <code>/transfer ID-ПОЛЬЗОВАТЕЛЯ</code> (/id)，其中用户：频道管理员和@{0}-bot 的成员\n\n⚙️<b>命令</b>/cmd",
-    'ar': "⚠️ لنقل حقوق مسؤول القناة إلى @ {0} -bot ، استخدم الأمر: <code>/transfer ID-ПОЛЬЗОВАТЕЛЯ</code> (/ id) ، حيث المستخدم: مسؤول القناة وعضو @ {0} -bot\n\n⚙️ <b>Commands</b> / cmd",
+    'ru': "⚠️ Для передачи admin-прав канала в @{0}-боте используй команду: /transfer ID-ПОЛЬЗОВАТЕЛЯ (/id), где пользователь: администратор канала и участник @{0}-бота\n\n⚙️ <b>Команды</b> /cmd",
+    'en': "⚠️ To transfer channel admin rights to @{0}-bot, use the command: /transfer ID-ПОЛЬЗОВАТЕЛЯ (/id), where user: channel administrator and member of @{0}-bot\n\n⚙️ <b>Commands</b> /cmd",
+    'es': "⚠️ Para transferir los derechos de administrador del canal a @{0}-bot, usa el comando: /transfer ID-ПОЛЬЗОВАТЕЛЯ (/id), donde usuario: administrador del canal y miembro de @{0}-bot\n\n⚙️ <b>Comandos</b> /cmd",
+    'fr': "⚠️ Pour transférer les droits d'administrateur du canal à @{0}-bot, utilisez la commande : /transfer ID-ПОЛЬЗОВАТЕЛЯ (/id), où utilisateur : administrateur du canal et membre de @{0}-bot\n\n⚙️ <b>Commandes</b> /cmd",
+    'zh': "⚠️ 要将频道管理员权限转移给@{0}-bot，请使用命令： /transfer ID-ПОЛЬЗОВАТЕЛЯ (/id)，其中用户：频道管理员和@{0}-bot 的成员\n\n⚙️<b>命令</b>/cmd",
+    'ar': "⚠️ لنقل حقوق مسؤول القناة إلى @ {0} -bot ، استخدم الأمر: /transfer ID-ПОЛЬЗОВАТЕЛЯ (/ id) ، حيث المستخدم: مسؤول القناة وعضو @ {0} -bot\n\n⚙️ <b>Commands</b> / cmd",
 }
 l_transfer_done_to = {
     'ru': "⚠️ <b>Admin</b>-права на [<b>{0}</b>] успешно переданы {1}",
     'en': "⚠️ <b>Admin</b> rights to [<b>{0}</b>] successfully transferred to {1}",
     'es': "⚠️ Derechos <b>de administrador</b> de [<b>{0}</b>] transferidos con éxito a {1}",
     'fr': "⚠️ Les droits <b>d&#x27;administrateur</b> de [<b>{0}</b>] ont été transférés avec succès à {1}",
     'zh': "⚠️ [<b>{0}</b>] 的<b>管理员</b>权限已成功转移给 {1}",
@@ -3387,20 +3395,20 @@
     'en': "🎥 In the [Administrators] settings, enable the option for @{0}-bot:\n[✅ Assign administrators]\n[✅ Manage broadcasts]\n\n🕚Wait 1min",
     'es': "🎥 En la configuración de [Administradores], habilita la opción para @{0}-bot:\n[✅ Asignar administradores]\n[✅ Administrar transmisiones]\n\n🕚Espera 1 minuto",
     'fr': "🎥 Dans les paramètres [Administrateurs], activez l'option pour @{0}-bot :\n[✅ Attribuer des administrateurs]\n[✅ Gérer les diffusions]\n\n🕚Attendez 1 min",
     'zh': "🎥 在 [Administrators] 设置中，启用 @{0}-bot 的选项：\n[✅ 分配管理员]\n[✅ 管理广播]\n\n🕚等待 1 分钟",
     'ar': "🎥 في إعدادات [Administrators] ، قم بتمكين خيار @ {0} -bot:\n[✅ تعيين المسؤولين]\n[✅ إدارة عمليات البث]\n\n🕚 انتظر لمدة دقيقة",
 }
 l_videochat_handler = {
-    'ru': "🎥 Автоматическое анонсирование <b>видео-трансляции</b> <code>[/videochat d h]</code> каждый <u>d</u>-день (1-31) на <u>h</u>-часов (1-168). Текущее значение: /videochat {0}\n\n👩🏽‍💻 Например,\n<code>/videochat 1 1</code> (ежедневный видео-анонс длительностью 1 час)\n<code>/videochat 0</code> (отключение опции)\n\n⚙️ <b>Команды</b> /cmd",
-    'en': "🎥 Automatic announcement <b>of the video broadcast</b> <code>[/videochat dh]</code> every <u>d</u> -day (1-31) for <u>h</u> -hours (1-168). Current value: /videochat {0}\n\n👩🏽‍💻 For example\n<code>/videochat 1 1</code> (daily 1 hour video announcement)\n<code>/videochat 0</code> (disable option)\n\n⚙️ <b>Commands</b> /cmd",
-    'es': "🎥 Anuncio automático <b>de la transmisión de video</b> <code>[/videochat dh]</code> cada <u>d</u> -día (1-31) durante <u>h</u> -horas (1-168). Valor actual: /videochat {0}\n\n👩🏽‍💻 Por ejemplo\n<code>/videochat 1 1</code> (anuncio de video diario de 1 hora)\n<code>/videochat 0</code> (opción deshabilitada)\n\n⚙️ <b>Comandos</b> /cmd",
-    'fr': "🎥 Annonce automatique <b>de la diffusion vidéo</b> <code>[/videochat dh]</code> tous <u>les j</u> -jours (1-31) pendant <u>h</u> -heures (1-168). Valeur actuelle : /videochat {0}\n\n👩🏽‍💻 Par exemple\n<code>/videochat 1 1</code> (annonce vidéo quotidienne d&#x27;une heure)\n<code>/videochat 0</code> (option de désactivation)\n\n⚙️ <b>Commandes</b> /cmd",
-    'zh': "🎥 每<u>d</u>天（1-31）自动播报<b>视频广播</b><code>[/videochat dh]</code> ，持续<u>h</u>小时（1-168）。当前值：/videochat {0}\n\n👩🏽‍💻 例如\n<code>/videochat 1 1</code> （每日 1 小时视频公告）\n<code>/videochat 0</code> （禁用选项）\n\n⚙️<b>命令</b>/cmd",
-    'ar': "🎥 الإعلان التلقائي <b>عن بث الفيديو</b> <code>[/videochat dh]</code> كل يوم <u>يوم</u> (1-31) لمدة <u>ساعة</u> (1-168). القيمة الحالية: / videochat {0}\n\n👩🏽‍💻 على سبيل المثال\n<code>/videochat 1 1</code> (إعلان فيديو لمدة ساعة يوميًا)\n<code>/videochat 0</code> (خيار تعطيل)\n\n⚙️ <b>أوامر</b> / cmd",
+    'ru': "🎥 Автоматическое анонсирование <b>видео-трансляции</b> [/videochat d h] каждый <u>d</u>-день (1-31) на <u>h</u>-часов (1-168). Текущее значение: /videochat {0}\n\n👩🏽‍💻 Например,\n/videochat 1 1 (ежедневный видео-анонс длительностью 1 час)\n/videochat 0 (отключение опции)\n\n⚙️ <b>Команды</b> /cmd",
+    'en': "🎥 Automatic announcement <b>of the video broadcast</b> [/videochat dh] every <u>d</u> -day (1-31) for <u>h</u> -hours (1-168). Current value: /videochat {0}\n\n👩🏽‍💻 For example\n/videochat 1 1 (daily 1 hour video announcement)\n/videochat 0 (disable option)\n\n⚙️ <b>Commands</b> /cmd",
+    'es': "🎥 Anuncio automático <b>de la transmisión de video</b> [/videochat dh] cada <u>d</u> -día (1-31) durante <u>h</u> -horas (1-168). Valor actual: /videochat {0}\n\n👩🏽‍💻 Por ejemplo\n/videochat 1 1 (anuncio de video diario de 1 hora)\n/videochat 0 (opción deshabilitada)\n\n⚙️ <b>Comandos</b> /cmd",
+    'fr': "🎥 Annonce automatique <b>de la diffusion vidéo</b> [/videochat dh] tous <u>les j</u> -jours (1-31) pendant <u>h</u> -heures (1-168). Valeur actuelle : /videochat {0}\n\n👩🏽‍💻 Par exemple\n/videochat 1 1 (annonce vidéo quotidienne d&#x27;une heure)\n/videochat 0 (option de désactivation)\n\n⚙️ <b>Commandes</b> /cmd",
+    'zh': "🎥 每<u>d</u>天（1-31）自动播报<b>视频广播</b>[/videochat dh] ，持续<u>h</u>小时（1-168）。当前值：/videochat {0}\n\n👩🏽‍💻 例如\n/videochat 1 1 （每日 1 小时视频公告）\n/videochat 0 （禁用选项）\n\n⚙️<b>命令</b>/cmd",
+    'ar': "🎥 الإعلان التلقائي <b>عن بث الفيديو</b> [/videochat dh] كل يوم <u>يوم</u> (1-31) لمدة <u>ساعة</u> (1-168). القيمة الحالية: / videochat {0}\n\n👩🏽‍💻 على سبيل المثال\n/videochat 1 1 (إعلان فيديو لمدة ساعة يوميًا)\n/videochat 0 (خيار تعطيل)\n\n⚙️ <b>أوامر</b> / cmd",
 }
 l_videochat_on = {
     'ru': "🎥 Анонсирована <b>видео-трансляция</b>: каждый <u>{0}</u> день на <u>{1}</u> часов\n\n⚙️ <b>Команды</b> /cmd",
     'en': "🎥 <b>Video stream</b> announced : every <u>{0}</u> day for <u>{1}</u> hours\n\n⚙️ <b>Commands</b> /cmd",
     'es': "🎥 <b>Transmisión de video</b> anunciada: cada <u>{0}</u> día durante <u>{1}</u> horas\n\n⚙️ <b>Comandos</b> /cmd",
     'fr': "🎥 <b>Flux vidéo</b> annoncé : tous les <u>{0}</u> jours pendant <u>{1}</u> heures\n\n⚙️ <b>Commandes</b> /cmd",
     'zh': "🎥<b>视频流</b>公布：每<u>{0}</u>天<u>{1}</u>小时\n\n⚙️<b>命令</b>/cmd",
@@ -3427,20 +3435,20 @@
     'en': "👩🏽‍💻 <b>Cleanup</b> completed\n<b>Current</b> number of users in the database: <u>{0}</u> (-{1})",
     'es': "👩🏽‍💻 <b>Limpieza</b> completada\nNúmero <b>actual</b> de usuarios en la base de datos: <u>{0}</u> (-{1})",
     'fr': "👩🏽‍💻 <b>Nettoyage</b> terminé\nNombre <b>actuel</b> d&#x27;utilisateurs dans la base de données : <u>{0}</u> (-{1})",
     'zh': "👩🏽‍💻<b>清理</b>完成\n数据库中的<b>当前</b>用户数： <u>{0}</u> (-{1})",
     'ar': "👩🏽‍💻 اكتمل <b>التنظيف</b>\nالعدد <b>الحالي</b> للمستخدمين في قاعدة البيانات: <u>{0}</u> (- {1})",
 }
 l_chn_ccheck_handler = {
-    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> по сгенерированной ссылке: {0} (только для <code>ЧАСТНЫХ</code> каналов)\n\n👉🏼 Для <b>проверки подписки</b> на другой канал <i>добавь</i> @{1}-бота в канал и выполни команду: <code>/channel {2}</code>\n\n👉🏼 Для <i>защиты от атаки</i> на канал включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
-    'en': "👮🏽 <b>Click</b> on ✅/🔘 to <b>switch</b> user <i>verification</i> type when <u>joining</u> via generated link: {0} (only for <code>ЧАСТНЫХ</code> channels)\n\n👉🏼 To <b>check subscription</b> to another channel, <i>add</i> @{1}-bot to the channel and run the command: <code>/channel {2}</code>\n\n👉🏼 To <i>protect against an attack</i> on the channel, turn on <b>the anti-raid</b> mode (block <u>all</u> intruders)",
-    'es': "👮🏽 <b>Haz clic</b> en ✅/🔘 para <b>cambiar</b> el tipo <i>de verificación</i> de usuario al <u>unirse</u> a través del enlace generado: {0} (solo para canales <code>ЧАСТНЫХ</code> )\n\n👉🏼 Para <b>verificar la suscripción</b> a otro canal, <i>agrega</i> @{1}-bot al canal y ejecuta el comando: <code>/channel {2}</code>\n\n👉🏼 Para <i>protegerte contra un ataque</i> en el canal, activa <b>el modo anti-raid</b> (bloquea <u>a todos</u> los intrusos)",
-    'fr': "👮🏽 <b>Cliquez</b> sur ✅/🔘 pour <b>changer</b> le type <i>de vérification</i> de l&#x27;utilisateur lors <u>de la connexion</u> via un lien généré : {0} (uniquement pour les canaux <code>ЧАСТНЫХ</code> )\n\n👉🏼 Pour <b>vérifier l&#x27;abonnement</b> à un autre canal, <i>ajoutez</i> @{1}-bot au canal et lancez la commande : <code>/channel {2}</code>\n\n👉🏼 Pour <i>vous protéger contre une attaque</i> sur le channel, activez <b>le mode anti-raid</b> (bloquer <u>tous</u> les intrus)",
-    'zh': "👮🏽<b>点击</b>✅/🔘 在通过生成的链接<u>加入</u>时<b>切换</b>用户<i>验证</i>类型：{0}（仅适用于<code>ЧАСТНЫХ</code>频道）\n\n👉🏼 要<b>检查对另一个频道的订阅</b>，请将 @{1}-bot<i>添加</i>到频道并运行命令： <code>/channel {2}</code>\n\n👉🏼 为<i>防止通道受到攻击</i>，请开启<b>防突袭</b>模式（阻止<u>所有</u>入侵者）",
-    'ar': "👮🏽 <b>انقر</b> على ✅ / 🔘 <b>لتبديل</b> نوع <i>التحقق</i> من المستخدم عند <u>الانضمام</u> عبر الرابط الذي تم إنشاؤه: {0} (للقنوات <code>ЧАСТНЫХ</code> فقط)\n\n👉🏼 للتحقق <b>من الاشتراك</b> في قناة أخرى ، <i>أضف</i> @ {1} -bot إلى القناة وقم بتشغيل الأمر: <code>/channel {2}</code>\n\n👉🏼 <i>للحماية من هجوم</i> على القناة ، قم بتشغيل الوضع <b>المضاد للغارة</b> (حظر <u>جميع</u> المتسللين)",
+    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> по сгенерированной ссылке: {0} (только для ЧАСТНЫХ каналов)\n\n👉🏼 Для <b>проверки подписки</b> на другой канал <i>добавь</i> @{1}-бота в канал и выполни команду: /channel {2}\n\n👉🏼 Для <i>защиты от атаки</i> на канал включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
+    'en': "👮🏽 <b>Click</b> on ✅/🔘 to <b>switch</b> user <i>verification</i> type when <u>joining</u> via generated link: {0} (only for ЧАСТНЫХ channels)\n\n👉🏼 To <b>check subscription</b> to another channel, <i>add</i> @{1}-bot to the channel and run the command: /channel {2}\n\n👉🏼 To <i>protect against an attack</i> on the channel, turn on <b>the anti-raid</b> mode (block <u>all</u> intruders)",
+    'es': "👮🏽 <b>Haz clic</b> en ✅/🔘 para <b>cambiar</b> el tipo <i>de verificación</i> de usuario al <u>unirse</u> a través del enlace generado: {0} (solo para canales ЧАСТНЫХ )\n\n👉🏼 Para <b>verificar la suscripción</b> a otro canal, <i>agrega</i> @{1}-bot al canal y ejecuta el comando: /channel {2}\n\n👉🏼 Para <i>protegerte contra un ataque</i> en el canal, activa <b>el modo anti-raid</b> (bloquea <u>a todos</u> los intrusos)",
+    'fr': "👮🏽 <b>Cliquez</b> sur ✅/🔘 pour <b>changer</b> le type <i>de vérification</i> de l&#x27;utilisateur lors <u>de la connexion</u> via un lien généré : {0} (uniquement pour les canaux ЧАСТНЫХ )\n\n👉🏼 Pour <b>vérifier l&#x27;abonnement</b> à un autre canal, <i>ajoutez</i> @{1}-bot au canal et lancez la commande : /channel {2}\n\n👉🏼 Pour <i>vous protéger contre une attaque</i> sur le channel, activez <b>le mode anti-raid</b> (bloquer <u>tous</u> les intrus)",
+    'zh': "👮🏽<b>点击</b>✅/🔘 在通过生成的链接<u>加入</u>时<b>切换</b>用户<i>验证</i>类型：{0}（仅适用于ЧАСТНЫХ频道）\n\n👉🏼 要<b>检查对另一个频道的订阅</b>，请将 @{1}-bot<i>添加</i>到频道并运行命令： /channel {2}\n\n👉🏼 为<i>防止通道受到攻击</i>，请开启<b>防突袭</b>模式（阻止<u>所有</u>入侵者）",
+    'ar': "👮🏽 <b>انقر</b> على ✅ / 🔘 <b>لتبديل</b> نوع <i>التحقق</i> من المستخدم عند <u>الانضمام</u> عبر الرابط الذي تم إنشاؤه: {0} (للقنوات ЧАСТНЫХ فقط)\n\n👉🏼 للتحقق <b>من الاشتراك</b> في قناة أخرى ، <i>أضف</i> @ {1} -bot إلى القناة وقم بتشغيل الأمر: /channel {2}\n\n👉🏼 <i>للحماية من هجوم</i> على القناة ، قم بتشغيل الوضع <b>المضاد للغارة</b> (حظر <u>جميع</u> المتسللين)",
 }
 l_ccheck_call = {
     'ru': "👮🏽 Для проверки подписки необходимо добавить дополнительный канал командой:\n\n/channel ССЫЛКА НА КАНАЛ",
     'en': "👮🏽 To check the subscription, you need to add an additional channel with the command:\n\n/channel LINK TO THE CHANNEL",
     'es': "👮🏽 Para verificar la suscripción, debe agregar un canal adicional con el comando:\n\n/canal ENLACE AL CANAL",
     'fr': "👮🏽 Pour vérifier l'abonnement, vous devez ajouter une chaîne supplémentaire avec la commande :\n\n/channel LIEN VERS LA CHAÎNE",
     'zh': "👮🏽 要检查订阅，您需要使用以下命令添加一个额外的频道：\n\n/channel LINK TO THE CHANNEL",
@@ -3575,28 +3583,28 @@
     'ar': "🔘️☐ Off مكافحة الغارة",
 }
 # endregion
 
 
 # region cban_
 l_cban_add = {
-    'ru': "🕵🏽 <b>Введи</b> <code>id</code> или <code>@username</code> пользователей  через пробельные символы или разделители, чтобы добавить их в /ban-список (*даже тех, кого нет <u>{0}</u>-файле)\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
-    'en': "🕵🏽 <b>Enter</b> user <code>id</code> or <code>@username</code> separated by spaces or separators to add them to the /ban list (*even those not in the <u>{0}</u> file)\n\n👩🏽‍💻 <b>Current</b> number of users on the /ban list : <u>{1}</u>",
-    'es': "🕵🏽 <b>Ingrese</b> <code>id</code> de usuario o <code>@username</code> usuario separados por espacios o separadores para agregarlos a la lista de /ban (*incluso aquellos que no están en el archivo <u>{0}</u> )\n\n👩🏽‍💻 Número <b>actual</b> de usuarios en la lista de /ban : <u>{1}</u>",
-    'fr': "🕵🏽 <b>Entrez</b> <code>id</code> ou <code>@username</code> d&#x27;utilisateur séparés par des espaces ou des séparateurs pour les ajouter à la liste /ban (*même ceux qui ne figurent pas dans le fichier <u>{0}</u> )\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;utilisateurs sur la liste /ban : <u>{1}</u>",
-    'zh': "🕵🏽<b>输入</b>用空格或分隔符分隔的用户<code>id</code>或<code>@username</code> ，将他们添加到 /ban 列表（*即使那些不在<u>{0}</u>文件中的）\n\n👩🏽‍💻 /ban 列表中的<b>当前</b>用户数： <u>{1}</u>",
-    'ar': "🕵🏽 <b>أدخل</b> <code>id</code> المستخدم أو <code>@username</code> مفصولة بمسافات أو فواصل لإضافتهما إلى / قائمة الحظر (* حتى أولئك غير الموجودين في <u>{0}</u> الملف)\n\n👩🏽‍💻 العدد <b>الحالي</b> للمستخدمين في / قائمة الحظر : <u>{1}</u>",
+    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей  через пробельные символы или разделители, чтобы добавить их в /ban-список (*даже тех, кого нет <u>{0}</u>-файле)\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
+    'en': "🕵🏽 <b>Enter</b> user id or @username separated by spaces or separators to add them to the /ban list (*even those not in the <u>{0}</u> file)\n\n👩🏽‍💻 <b>Current</b> number of users on the /ban list : <u>{1}</u>",
+    'es': "🕵🏽 <b>Ingrese</b> id de usuario o @username usuario separados por espacios o separadores para agregarlos a la lista de /ban (*incluso aquellos que no están en el archivo <u>{0}</u> )\n\n👩🏽‍💻 Número <b>actual</b> de usuarios en la lista de /ban : <u>{1}</u>",
+    'fr': "🕵🏽 <b>Entrez</b> id ou @username d&#x27;utilisateur séparés par des espaces ou des séparateurs pour les ajouter à la liste /ban (*même ceux qui ne figurent pas dans le fichier <u>{0}</u> )\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;utilisateurs sur la liste /ban : <u>{1}</u>",
+    'zh': "🕵🏽<b>输入</b>用空格或分隔符分隔的用户id或@username ，将他们添加到 /ban 列表（*即使那些不在<u>{0}</u>文件中的）\n\n👩🏽‍💻 /ban 列表中的<b>当前</b>用户数： <u>{1}</u>",
+    'ar': "🕵🏽 <b>أدخل</b> id المستخدم أو @username مفصولة بمسافات أو فواصل لإضافتهما إلى / قائمة الحظر (* حتى أولئك غير الموجودين في <u>{0}</u> الملف)\n\n👩🏽‍💻 العدد <b>الحالي</b> للمستخدمين في / قائمة الحظر : <u>{1}</u>",
 }
 l_cban_remove = {
-    'ru': "🕵🏽 <b>Введи</b> <code>id</code> или <code>@username</code> пользователей из <u>{0}</u>-файла через пробельные символы или разделители, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
-    'en': "🕵🏽 <b>Enter</b> <code>id</code> or <code>@username</code> of users from <u>{0}</u> -file separated by spaces or separators to remove them from /ban-list\n\n👩🏽‍💻 <b>Current</b> number of users /ban-list: <u>{1}</u>",
-    'es': "🕵🏽 <b>Ingrese</b> <code>id</code> o <code>@username</code> de los usuarios de <u>{0}</u> -archivo separado por espacios o separadores para eliminarlos de /ban-list\n\n👩🏽‍💻 Número <b>actual</b> de usuarios /ban-list: <u>{1}</u>",
-    'fr': "🕵🏽 <b>Entrez</b> <code>id</code> ou <code>@username</code> utilisateur des utilisateurs de <u>{0}</u> -fichier séparés par des espaces ou des séparateurs pour les supprimer de /ban-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;utilisateurs /ban-list : <u>{1}</u>",
-    'zh': "🕵🏽<b>输入</b><u>{0}</u>文件中用户的<code>id</code>或<code>@username</code> ，以空格或分隔符分隔，以将其从 /ban-list 中删除\n\n👩🏽‍💻<b>当前</b>用户数 /ban-list： <u>{1}</u>",
-    'ar': "🕵🏽 <b>أدخل</b> <code>id</code> أو <code>@username</code> للمستخدمين من <u>{0}</u> - ملف مفصول بمسافات أو فواصل لإزالتهم من / ban-list\n\n👩🏽‍💻 العدد <b>الحالي</b> للمستخدمين / قائمة الحظر: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Введи</b> id или @username пользователей из <u>{0}</u>-файла через пробельные символы или разделители, чтобы удалить их из /ban-списка\n\n👩🏽‍💻 <b>Текущее</b> число пользователей /ban-списка: <u>{1}</u>",
+    'en': "🕵🏽 <b>Enter</b> id or @username of users from <u>{0}</u> -file separated by spaces or separators to remove them from /ban-list\n\n👩🏽‍💻 <b>Current</b> number of users /ban-list: <u>{1}</u>",
+    'es': "🕵🏽 <b>Ingrese</b> id o @username de los usuarios de <u>{0}</u> -archivo separado por espacios o separadores para eliminarlos de /ban-list\n\n👩🏽‍💻 Número <b>actual</b> de usuarios /ban-list: <u>{1}</u>",
+    'fr': "🕵🏽 <b>Entrez</b> id ou @username utilisateur des utilisateurs de <u>{0}</u> -fichier séparés par des espaces ou des séparateurs pour les supprimer de /ban-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;utilisateurs /ban-list : <u>{1}</u>",
+    'zh': "🕵🏽<b>输入</b><u>{0}</u>文件中用户的id或@username ，以空格或分隔符分隔，以将其从 /ban-list 中删除\n\n👩🏽‍💻<b>当前</b>用户数 /ban-list： <u>{1}</u>",
+    'ar': "🕵🏽 <b>أدخل</b> id أو @username للمستخدمين من <u>{0}</u> - ملف مفصول بمسافات أو فواصل لإزالتهم من / ban-list\n\n👩🏽‍💻 العدد <b>الحالي</b> للمستخدمين / قائمة الحظر: <u>{1}</u>",
 }
 l_cban_added = {
     'ru': "🕵🏽 Пользователь {0} добавлен в /ban-список (причина: <i>{1}</i>)",
     'en': "🕵🏽 User {0} added to /ban list (reason: <i>{1}</i> )",
     'es': "🕵🏽 Usuario {0} agregado a /lista de prohibición (razón: <i>{1}</i> )",
     'fr': "🕵🏽 L'utilisateur {0} a été ajouté à la liste /ban (raison : <i>{1}</i> )",
     'zh': "🕵🏽 用户 {0} 添加到 /ban 列表（原因： <i>{1}</i> ）",
@@ -3767,20 +3775,20 @@
     'en': "👍🏽 In the [Administrators] settings for @{0} on:\n[✅ Add member]\n\n🕚Wait 1min",
     'es': "👍🏽 En la configuración de [Administradores] para @{0} en:\n[✅ Agregar miembro]\n\n🕚Espera 1 minuto",
     'fr': "👍🏽 Dans les paramètres [Administrateurs] pour @{0} sur :\n[✅ Ajouter un membre]\n\n🕚Attendez 1min",
     'zh': "👍🏽在@{0}的[管理员]设置中：\n[✅添加成员]\n\n🕚等待1分钟",
     'ar': "👍🏽 في إعدادات [Administrators] لـ @ {0} على:\n[✅ إضافة عضو]\n\n🕚 انتظر دقيقة واحدة",
 }
 l_creact_correct = {
-    'ru': "👍🏽 <b>Введи</b> корректное <b>число</b> креативных авто-реакций на последний пост канала\n\n👩🏽‍💻 Используй команду <code>/react {0}</code>, чтобы задать количество авто-реакций (<b>текущее</b> количество: <u>{0}</u>)",
-    'en': "👍🏽 <b>Enter</b> the correct <b>number</b> of creative auto-reactions to the last post of the channel\n\n👩🏽‍💻 Use the <code>/react {0}</code> command to set the number of auto-reactions ( <b>current</b> number: <u>{0}</u> )",
-    'es': "👍🏽 <b>Ingresa</b> el <b>número</b> correcto de reacciones automáticas creativas a la última publicación del canal\n\n👩🏽‍💻 Usa el comando <code>/react {0}</code> para establecer el número de reacciones automáticas (número <b>actual</b> : <u>{0}</u> )",
-    'fr': "👍🏽 <b>Saisissez</b> le <b>nombre</b> correct de réactions automatiques créatives au dernier message de la chaîne\n\n👩🏽‍💻 Utilisez la commande <code>/react {0}</code> pour définir le nombre de réactions automatiques (nombre <b>actuel</b> : <u>{0}</u> )",
-    'zh': "👍🏽<b>输入</b>频道最后一个帖子的正确创意自动反应<b>数量</b>\n\n👩🏽‍💻 使用<code>/react {0}</code>命令设置自动反应数量（<b>当前</b>数量： <u>{0}</u> ）",
-    'ar': "👍🏽 <b>أدخل</b> <b>العدد</b> الصحيح من ردود الفعل التلقائية الإبداعية على آخر مشاركة للقناة\n\n👩🏽‍💻 استخدم الأمر <code>/react {0}</code> لتعيين عدد التفاعلات التلقائية (الرقم <b>الحالي</b> : <u>{0}</u> )",
+    'ru': "👍🏽 <b>Введи</b> корректное <b>число</b> креативных авто-реакций на последний пост канала\n\n👩🏽‍💻 Используй команду /react {0}, чтобы задать количество авто-реакций (<b>текущее</b> количество: <u>{0}</u>)",
+    'en': "👍🏽 <b>Enter</b> the correct <b>number</b> of creative auto-reactions to the last post of the channel\n\n👩🏽‍💻 Use the /react {0} command to set the number of auto-reactions ( <b>current</b> number: <u>{0}</u> )",
+    'es': "👍🏽 <b>Ingresa</b> el <b>número</b> correcto de reacciones automáticas creativas a la última publicación del canal\n\n👩🏽‍💻 Usa el comando /react {0} para establecer el número de reacciones automáticas (número <b>actual</b> : <u>{0}</u> )",
+    'fr': "👍🏽 <b>Saisissez</b> le <b>nombre</b> correct de réactions automatiques créatives au dernier message de la chaîne\n\n👩🏽‍💻 Utilisez la commande /react {0} pour définir le nombre de réactions automatiques (nombre <b>actuel</b> : <u>{0}</u> )",
+    'zh': "👍🏽<b>输入</b>频道最后一个帖子的正确创意自动反应<b>数量</b>\n\n👩🏽‍💻 使用/react {0}命令设置自动反应数量（<b>当前</b>数量： <u>{0}</u> ）",
+    'ar': "👍🏽 <b>أدخل</b> <b>العدد</b> الصحيح من ردود الفعل التلقائية الإبداعية على آخر مشاركة للقناة\n\n👩🏽‍💻 استخدم الأمر /react {0} لتعيين عدد التفاعلات التلقائية (الرقم <b>الحالي</b> : <u>{0}</u> )",
 }
 l_creact_on = {
     'ru': "👍🏽 <b>Готово!</b> Текущее количество <b>авто-реакций</b> на пост канала установлено в значение <u>{0}</u>",
     'en': "👍🏽 <b>Done!</b> The current number of <b>auto-reactions</b> per channel post is set to <u>{0}</u>",
     'es': "👍🏽 <b>Listo!</b> El número actual de <b>reacciones automáticas</b> por publicación de canal está establecido en <u>{0}</u>",
     'fr': "👍🏽 <b>C&#x27;est fait !</b> Le nombre actuel de <b>réactions automatiques</b> par publication de chaîne est défini sur <u>{0}</u>",
     'zh': "👍🏽<b>完成！</b>每个频道帖子的当前<b>自动反应</b>数设置为<u>{0}</u>",
@@ -3811,20 +3819,20 @@
     'en': "👁️‍🗨️ In the [Administrators] settings for @{0} on:\n[✅ Add member]\n\n🕚Please wait 1min",
     'es': "👁️‍🗨️ En la configuración de [Administradores] para @{0} en:\n[✅ Agregar miembro]\n\n🕚Espere 1 minuto",
     'fr': "👁️‍🗨️ Dans les paramètres [Administrateurs] pour @{0} sur :\n[✅ Ajouter un membre]\n\n🕚Veuillez patienter 1 min",
     'zh': "👁️‍🗨️ 在@{0}的[管理员]设置中：\n[✅添加成员]\n\n🕚请稍候1分钟",
     'ar': "👁️‍🗨️ في إعدادات [Administrators] لـ @ {0} على:\n[✅ إضافة عضو]\n\n🕚 يرجى الانتظار لمدة دقيقة",
 }
 l_cview_correct = {
-    'ru': "👁️‍🗨️ <b>Введи</b> корректное <b>число</b> авто-просмотров последнего поста канала\n\n👩🏽‍💻 Используй команду <code>/view {0}</code>, чтобы задать количество авто-просмотров (<b>текущее</b> количество: <u>{0}</u>)",
-    'en': "👁️‍🗨️ <b>Enter</b> the correct <b>number of</b> auto-views for the last post of the channel\n\n👩🏽‍💻 Use <code>/view {0}</code> to set the number of auto-views ( <b>current</b> number: <u>{0}</u> )",
-    'es': "👁️‍🗨️ <b>Ingresa</b> la <b>cantidad correcta de</b> vistas automáticas para la última publicación del canal\n\n👩🏽‍💻 Usa <code>/view {0}</code> para establecer la cantidad de vistas automáticas (número <b>actual</b> : <u>{0}</u> )",
-    'fr': "👁️‍🗨️ <b>Entrez</b> le <b>nombre correct de</b> vues automatiques pour le dernier message de la chaîne\n\n👩🏽‍💻 Utilisez <code>/view {0}</code> pour définir le nombre de vues automatiques (nombre <b>actuel</b> : <u>{0}</u> )",
-    'zh': "👁️‍🗨️ 为频道的最后一个帖子<b>输入</b>正确<b>的自动观看次数</b>\n\n👩🏽‍💻 使用<code>/view {0}</code>设置自动观看次数（<b>当前</b>次数： <u>{0}</u> ）",
-    'ar': "👁️‍🗨️ <b>أدخل</b> <b>العدد</b> الصحيح للمشاهدات التلقائية لآخر مشاركة للقناة\n\n👩🏽‍💻 استخدم <code>/view {0}</code> لتعيين عدد المشاهدات التلقائية (الرقم <b>الحالي</b> : <u>{0}</u> )",
+    'ru': "👁️‍🗨️ <b>Введи</b> корректное <b>число</b> авто-просмотров последнего поста канала\n\n👩🏽‍💻 Используй команду /view {0}, чтобы задать количество авто-просмотров (<b>текущее</b> количество: <u>{0}</u>)",
+    'en': "👁️‍🗨️ <b>Enter</b> the correct <b>number of</b> auto-views for the last post of the channel\n\n👩🏽‍💻 Use /view {0} to set the number of auto-views ( <b>current</b> number: <u>{0}</u> )",
+    'es': "👁️‍🗨️ <b>Ingresa</b> la <b>cantidad correcta de</b> vistas automáticas para la última publicación del canal\n\n👩🏽‍💻 Usa /view {0} para establecer la cantidad de vistas automáticas (número <b>actual</b> : <u>{0}</u> )",
+    'fr': "👁️‍🗨️ <b>Entrez</b> le <b>nombre correct de</b> vues automatiques pour le dernier message de la chaîne\n\n👩🏽‍💻 Utilisez /view {0} pour définir le nombre de vues automatiques (nombre <b>actuel</b> : <u>{0}</u> )",
+    'zh': "👁️‍🗨️ 为频道的最后一个帖子<b>输入</b>正确<b>的自动观看次数</b>\n\n👩🏽‍💻 使用/view {0}设置自动观看次数（<b>当前</b>次数： <u>{0}</u> ）",
+    'ar': "👁️‍🗨️ <b>أدخل</b> <b>العدد</b> الصحيح للمشاهدات التلقائية لآخر مشاركة للقناة\n\n👩🏽‍💻 استخدم /view {0} لتعيين عدد المشاهدات التلقائية (الرقم <b>الحالي</b> : <u>{0}</u> )",
 }
 l_cview_on = {
     'ru': "👁️‍🗨️ <b>Готово!</b> Текущее количество <b>авто-просмотров</b> на последний пост канала установлено в значение <u>{0}</u>",
     'en': "👁️‍🗨️ <b>Done!</b> The current number of <b>auto-views</b> for the channel&#x27;s last post is set to <u>{0}</u>",
     'es': "👁️‍🗨️ <b>Listo!</b> El número actual de <b>visualizaciones automáticas</b> de la última publicación del canal está establecido en <u>{0}.</u>",
     'fr': "👁️‍🗨️ <b>C&#x27;est fait !</b> Le nombre actuel de <b>vues automatiques</b> pour le dernier message de la chaîne est défini sur <u>{0}</u>",
     'zh': "👁️‍🗨️<b>完成！</b>频道上一篇帖子的当前<b>自动观看</b>次数设置为<u>{0}</u>",
@@ -3839,20 +3847,20 @@
     'ar': "👁️‍🗨️ / عرض-طرق العرض التلقائي معطلة",
 }
 # endregion
 
 
 # region cdecor_
 l_cdecor_text = {
-    'ru': "🪄 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-декор публикуемого поста: <i><b>пагинация</b> (порядковый номер поста)/креативный <b>формат текста</b> (<b>жирный</b>/<i>курсив</i>/<u>подчеркнутый</u>/<code>моно</code>/<tg-spoiler>спойлер</tg-spoiler>/#хэштег/<a href='{0}'>ссылка</a>)/<b>футер</b> (текстовое окончание поста)</i>\n\n👉🏼 Например, опция <b>[✅☑Вкл формат текста]</b> означает креативное изменение поста с использованием 7 стилей",
-    'en': "🪄 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> the auto-decor of the published post: <i><b>pagination</b> (post serial number)/creative <b>text format</b> ( <b>bold</b> /italic/ <u>underlined</u> /</i> <code>моно</code> <i>/spoiler/</i> <i>#хэштег</i> <i>/link)/ <b>footer</b> (post text ending)</i>\n\n👉🏼 For example, the option <b>[✅☑Enable Text Format]</b> means creative post editing using 7 styles",
-    'es': "🪄 <b>Haga clic</b> en ✅/☑️ para <b>activar/desactivar</b> la decoración automática de la publicación: <i><b>paginación</b> (número de serie de la publicación)/ <b>formato de texto</b> creativo ( <b>negrita</b> /cursiva/ <u>subrayado</u> /</i> <code>моно</code> <i>/spoiler/</i> <i>#хэштег</i> <i>/enlace)/ <b>pie de página</b> (publicación final del texto)</i>\n\n👉🏼 Por ejemplo, la opción <b>[✅☑Habilitar formato de texto]</b> significa edición creativa de publicaciones usando 7 estilos",
-    'fr': "🪄 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> le décor automatique de l&#x27;article publié : <i><b>pagination</b> (numéro de série de l&#x27;article)/ <b>format du texte</b> créatif ( <b>gras</b> /italique/ <u>souligné</u> /</i> <code>моно</code> <i>/spoiler/</i> <i>#хэштег</i> <i>/lien)/ <b>pied de page</b> (article fin du texte)</i>\n\n👉🏼 Par exemple, l&#x27;option <b>[✅☑Activer le format de texte]</b> signifie une post-édition créative utilisant 7 styles",
-    'zh': "🪄<b>点击</b>✅/☑️<b>开启/关闭</b>已发布帖子的自动装饰：<i><b>分页</b>（帖子序列号）/创意<b>文本格式</b>（<b>粗体</b>/斜体/<u>下划线</u>/</i> <code>моно</code> <i>/剧透/</i> <i>#хэштег</i> <i>/link）/<b>页脚</b>（帖子text ending)</i>\n\n👉🏼 例如选项<b>[✅☑Enable Text Format]</b>表示使用 7 种样式进行创意后期编辑",
-    'ar': "🪄 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف</b> الديكور التلقائي للمنشور المنشور: <i><b>ترقيم الصفحات</b> (الرقم التسلسلي للرسالة) / <b>تنسيق النص</b> الإبداعي ( <b>غامق</b> / مائل / <u>تحته خط</u> /</i> <code>моно</code> <i>/ سبويلر /</i> <i>#хэштег</i> <i>/ رابط) / تذييل ( <b>منشور</b> ) نهاية النص)</i>\n\n👉🏼 على سبيل المثال ، الخيار <b>[✅☑ تمكين تنسيق النص]</b> يعني تحرير المنشور الإبداعي باستخدام 7 أنماط",
+    'ru': "🪄 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-декор публикуемого поста: <i><b>пагинация</b> (порядковый номер поста)/креативный <b>формат текста</b> (<b>жирный</b>/<i>курсив</i>/<u>подчеркнутый</u>/моно/<tg-spoiler>спойлер</tg-spoiler>/#хэштег/<a href='{0}'>ссылка</a>)/<b>футер</b> (текстовое окончание поста)</i>\n\n👉🏼 Например, опция <b>[✅☑Вкл формат текста]</b> означает креативное изменение поста с использованием 7 стилей",
+    'en': "🪄 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> the auto-decor of the published post: <i><b>pagination</b> (post serial number)/creative <b>text format</b> ( <b>bold</b> /italic/ <u>underlined</u> /</i> моно <i>/spoiler/</i> <i>#хэштег</i> <i>/link)/ <b>footer</b> (post text ending)</i>\n\n👉🏼 For example, the option <b>[✅☑Enable Text Format]</b> means creative post editing using 7 styles",
+    'es': "🪄 <b>Haga clic</b> en ✅/☑️ para <b>activar/desactivar</b> la decoración automática de la publicación: <i><b>paginación</b> (número de serie de la publicación)/ <b>formato de texto</b> creativo ( <b>negrita</b> /cursiva/ <u>subrayado</u> /</i> моно <i>/spoiler/</i> <i>#хэштег</i> <i>/enlace)/ <b>pie de página</b> (publicación final del texto)</i>\n\n👉🏼 Por ejemplo, la opción <b>[✅☑Habilitar formato de texto]</b> significa edición creativa de publicaciones usando 7 estilos",
+    'fr': "🪄 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> le décor automatique de l&#x27;article publié : <i><b>pagination</b> (numéro de série de l&#x27;article)/ <b>format du texte</b> créatif ( <b>gras</b> /italique/ <u>souligné</u> /</i> моно <i>/spoiler/</i> <i>#хэштег</i> <i>/lien)/ <b>pied de page</b> (article fin du texte)</i>\n\n👉🏼 Par exemple, l&#x27;option <b>[✅☑Activer le format de texte]</b> signifie une post-édition créative utilisant 7 styles",
+    'zh': "🪄<b>点击</b>✅/☑️<b>开启/关闭</b>已发布帖子的自动装饰：<i><b>分页</b>（帖子序列号）/创意<b>文本格式</b>（<b>粗体</b>/斜体/<u>下划线</u>/</i> моно <i>/剧透/</i> <i>#хэштег</i> <i>/link）/<b>页脚</b>（帖子text ending)</i>\n\n👉🏼 例如选项<b>[✅☑Enable Text Format]</b>表示使用 7 种样式进行创意后期编辑",
+    'ar': "🪄 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف</b> الديكور التلقائي للمنشور المنشور: <i><b>ترقيم الصفحات</b> (الرقم التسلسلي للرسالة) / <b>تنسيق النص</b> الإبداعي ( <b>غامق</b> / مائل / <u>تحته خط</u> /</i> моно <i>/ سبويلر /</i> <i>#хэштег</i> <i>/ رابط) / تذييل ( <b>منشور</b> ) نهاية النص)</i>\n\n👉🏼 على سبيل المثال ، الخيار <b>[✅☑ تمكين تنسيق النص]</b> يعني تحرير المنشور الإبداعي باستخدام 7 أنماط",
 }
 l_cdecor_footer_call = {
     'ru': "🪄 Футер пустой, необходимо его ⚙️Настроить",
     'en': "🪄 The footer is empty, you need to set it up ⚙️",
     'es': "🪄 El pie de página está vacío, debes configurarlo ⚙️",
     'fr': "🪄 Le pied de page est vide, vous devez le paramétrer ⚙️",
     'zh': "🪄 footer 是空的，需要设置一下⚙️",
@@ -3992,20 +4000,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_group_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>администрирования</code> <b>Telegram</b>-групп:\n\n▪️<b>защита</b> группы от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b>\n▪️<b>организация</b> бана и антифлуда\n▪️<b>авто-ответы</b> и стоп-слова\n\n❗️Регулярно-обновляемый /content",
-    'en': "🌱 {0}, welcome to <i>the landing bot</i> <code>администрирования</code> <b>Telegram</b> groups:\n\n▪️ <b>protecting</b> the group from spyware\n▪️displaying <b>statistics</b> and engagement (%)\n▪️restricting rights before <b>subscribing</b> to the channel\n▪️ <b>organizing</b> a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>администрирования</code> grupos <b>de Telegram</b> :\n\ <b>n▪️proteger</b> al grupo de spyware\n▪️mostrar <b>estadísticas</b> e interacción (%)\n▪️restringir los derechos antes de <b>suscribirse</b> al canal\ <b>n▪️organizar</b> un prohibición y anti-inundación\n\n❗️también puede solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
-    'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> <code>администрирования</code> des groupes <b>Telegram</b> :\n\n▪️ <b>protéger</b> le groupe des spywares\n▪️afficher <b>les statistiques</b> et l&#x27;engagement (%)\n▪️restreindre les droits avant de <b>s&#x27;abonner</b> à la chaîne\n▪️ <b>organiser</b> un interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
-    'zh': "🌱 {0}，欢迎使用<code>администрирования</code> <b>Telegram</b>群组的<i>登陆机器人</i>：\n\n▪️<b>保护</b>群组免受间谍软件的侵害\n▪️ 显示<b>统计数据</b>和参与度 (%)\n▪️ 在<b>订阅</b>频道之前限制权利\n▪️<b>组织</b>一个ban 和 anti-flood\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> <code>администрирования</code> مجموعات <b>Telegram</b> :\n\n▪️ <b>حماية</b> المجموعة من برامج التجسس\n▪️ عرض <b>الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> الحظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> администрирования <b>Telegram</b>-групп:\n\n▪️<b>защита</b> группы от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b>\n▪️<b>организация</b> бана и антифлуда\n▪️<b>авто-ответы</b> и стоп-слова\n\n❗️Регулярно-обновляемый /content",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> администрирования <b>Telegram</b> groups:\n\n▪️ <b>protecting</b> the group from spyware\n▪️displaying <b>statistics</b> and engagement (%)\n▪️restricting rights before <b>subscribing</b> to the channel\n▪️ <b>organizing</b> a ban and anti-flood\n\n❗️you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> администрирования grupos <b>de Telegram</b> :\n\ <b>n▪️proteger</b> al grupo de spyware\n▪️mostrar <b>estadísticas</b> e interacción (%)\n▪️restringir los derechos antes de <b>suscribirse</b> al canal\ <b>n▪️organizar</b> un prohibición y anti-inundación\n\n❗️también puede solicitar el desarrollo de un bot de chat en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue dans <i>le landing bot</i> администрирования des groupes <b>Telegram</b> :\n\n▪️ <b>protéger</b> le groupe des spywares\n▪️afficher <b>les statistiques</b> et l&#x27;engagement (%)\n▪️restreindre les droits avant de <b>s&#x27;abonner</b> à la chaîne\n▪️ <b>organiser</b> un interdiction et anti-flood\n\n❗️vous pouvez également commander le développement d'un chat bot dans notre studio de Ferey",
+    'zh': "🌱 {0}，欢迎使用администрирования <b>Telegram</b>群组的<i>登陆机器人</i>：\n\n▪️<b>保护</b>群组免受间谍软件的侵害\n▪️ 显示<b>统计数据</b>和参与度 (%)\n▪️ 在<b>订阅</b>频道之前限制权利\n▪️<b>组织</b>一个ban 和 anti-flood\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> администрирования مجموعات <b>Telegram</b> :\n\n▪️ <b>حماية</b> المجموعة من برامج التجسس\n▪️ عرض <b>الإحصائيات</b> والمشاركة (٪)\n▪️ تقييد الحقوق قبل <b>الاشتراك</b> في القناة\n▪️ <b>تنظيم</b> الحظر ومكافحة الفيضانات\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey الخاص بنا",
 }
 l_subscribe_group = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️<b>стоп-слова</b> без ограничений\n▪️<b>старт-слова</b> без ограничений\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -4194,20 +4202,20 @@
     'ar': "👮🏽 <i>للتحقق من الاشتراك ،</i> تحتاج إلى إضافة قناة باستخدام الأمر:\n\n/ channel LINK TO THE CHANNEL",
 }
 # endregion
 
 
 # region commands
 l_group_commands_handler = {
-    'ru': "⚙️ <b>Настройка</b> группы <b>{0}</b> {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/update <i>обновление параметров</i>\n/transfer   <i>передача admin-прав</i>\n/info   <i>информация</i>\n/stat   <i>статистика</i>\n/log   <i>посмотреть логи</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>парсинг старых id-аккаунтов</i>\n\n<b>⛏ Команды администраторов</b>\n/ban 5m|1h|10d <i>удаление из группы на время</i>\n/unban\n/mute 5m|1h|10d <i>ограничение в группе на время</i>\n/unmute\n/warn+сообщ <i>предупреждение</i>\n/status\n/karma  [+|-]\n/tag+сообщ   <i>@tager random-аккаунтов</i>\n/stop  <i>добавить стоп-слово</i>\n/channel NAME   <i>добавить канал для проверки подписки</i>\n/button NAME    <i>добавить имя кнопки входного контроля</i>\n/delay MIN      <i>установить количество min для задержки 1го сообщ</i>\n/flood NUM      <i>установить количество сообщ для flood</i>\n\n<b>⛏ Команды пользователей</b>\n/help   <i>вывод команд</i>\n/rules  <i>правила группы</i>\n/report <i>сообщить о нарушении</i>\n/happy  <i>получить радость</i>\n/thanks <i>поблагодарить</i>",
-    'en': "⚙️ Group <b>setting</b> <b>{0}</b> {1}\n\n<b>⛏ Admin commands @{2}</b>\n/update <i>update parameters</i>\n/transfer <i>transfer admin rights</i>\n/info <i>information</i>\n/stat <i>statistics</i>\n/log <i>view logs</i>\n/parse <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parse old account ids</i>\n\n<b>⛏ Commands for administrators</b>\n/ban 5m|1h|10d <i>temporary removal from the group</i>\n/unban\n/mute 5m|1h|10d <i>group time limit</i>\n/unmute\n/warn+mess <i>warning</i>\n/status\n/karma [+|-]\n/tag+mess <i>@tager</i> <i>random- accounts</i>\n/stop <i>add a stopword</i>\n/channel NAME <i>add a channel for checking subscription</i>\n/button NAME <i>add a name for input control button</i>\n/delay MIN <i>set the min amount to delay 1 message</i>\n/flood NUM <i>set the number of messages for flood</i>\n\n<b>⛏ User commands</b>\n/help <i>command output</i>\n/rules <i>group rules</i>\n/report report <i>abuse</i>\n/happy <i>get joy</i>\n/thanks <i>thank</i>",
-    'es': "⚙️ <b>Configuración</b> de grupo <b>{0}</b> {1}\n\n<b>⛏ Comandos de administrador @{2}</b>\n/actualizar <i>actualizar parámetros</i>\n/transferir <i>transferir derechos de administrador</i>\n/ <i>información</i> de información\n/ <i>estadísticas</i>\n/registrar <i>ver registros</i> \ n/parse <i>[todos|antiguos|premium|activos|en línea]</i>\n<code>/parse old</code> : <i>analiza los ID de cuentas antiguos</i>\n\n<b>⛏ Comandos para administradores</b>\n/ban 5m|1h|10d <i>eliminación temporal del grupo</i>\n/unban\n/silencio 5m|1h| <i>límite de tiempo de grupo</i> 10d\n/no silenciar\n/advertencia+mensaje <i>advertencia</i>\n/estado\n/karma [+|-]\n/tag+mess <i>@tager</i> <i>cuentas aleatorias</i>\n/ detener <i>agregar una palabra vacía</i>\n/NOMBRE del canal <i>agregar un canal para verificar la suscripción</i>\n/NOMBRE del botón <i>agregar un nombre para el botón de control de entrada</i>\n/retardo MIN <i>establecer la cantidad mínima para retrasar 1 mensaje</i>\n/inundación NUM <i>establecer el número de mensajes para inundación</i>\n\n<b>⛏ Comandos de usuario</b>\n/ <i>salida de comando</i> de ayuda\n/ <i>reglas reglas de grupo</i>\n/informar informar <i>abuso</i>\n/feliz <i>obtener alegría</i>\n/gracias <i>gracias</i>",
-    'fr': "⚙️ <b>Paramètres</b> de groupe <b>{0}</b> {1}\n\n<b>⛏ Commandes d&#x27;administration @{2}</b>\n/mettre à jour <i>les paramètres de mise à jour</i>\n/transférer <i>les droits d&#x27;administrateur de transfert</i>\n/ <i>informations d&#x27;information</i>\n/ <i>statistiques</i>\n/journal <i>afficher les journaux</i> \ n/parse <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>analyse les anciens identifiants de compte</i>\n\n<b>⛏ Commandes pour les administrateurs</b>\n/ban 5m|1h|10d <i>suppression temporaire du groupe</i>\n/unban\n/mute 5m|1h|10d <i>limite de temps de groupe</i>\n/unmute\n/warn+mess <i>warning</i>\n/status\n/karma [+|-]\n/tag+mess <i>@tager</i> <i>random- accounts</i>\n/ stop <i>ajouter un mot vide</i>\n/channel NAME <i>ajouter un canal pour vérifier l&#x27;abonnement</i>\n/button NAME <i>ajouter un nom pour le bouton de contrôle d&#x27;entrée</i>\n/delay MIN <i>définir le montant minimum pour retarder 1 message</i>\n/flood NUM <i>définir le nombre de messages for flood</i>\n\n<b>⛏ Commandes utilisateur</b>\n/ <i>sortie de la commande d&#x27;</i> aide\n/ <i>rules règles du groupe</i>\n/signaler signaler un <i>abus</i>\n/happy <i>get joy</i>\n/merci <i>merci</i>",
-    'zh': "⚙️ 群组<b>设置{0}</b> {1}\n\n<b>⛏ 管理员命令@{2}</b>\n/update<i>更新参数</i>\n/transfer<i>转移admin 权限</i>\n/info<i>信息</i>\n/stat<i>统计</i>\n/log<i>查看日志</i>\ n/parse <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> -<i>解析旧帐户 ID</i>\n\n<b>⛏ 管理员命令</b>\n/ban 5m|1h|10d<i>临时从组中删除</i>\n/unban\n/mute 5m|1h|10d<i>群限时</i>\n/unmute\n/warn+mess<i>警告</i>\n/status\n/karma[+|-]\n/tag+mess <i>@tager</i> <i>random-accounts</i>\n/ stop<i>添加停用词</i>\n/channel NAME<i>添加检查订阅的频道</i>\n/button NAME<i>添加输入控制按钮的名称</i>\n/delay MIN<i>设置延迟 1 条消息的最小量</i>\n/flood NUM<i>设置消息数for flood</i>\n\n<b>⛏ 用户命令</b>\n/help<i>命令输出</i>\n/rules<i>组规则</i>\n/report 报告<i>滥用</i>\n/happy <i>get joy</i>\n/thanks <i>thank</i>",
-    'ar': "⚙️ <b>إعداد</b> المجموعة <b>{0}</b> {1}\n\n<b>⛏ أوامر المسؤول @ {2}</b>\n/ <i>تحديث المعلمات</i>\n/ <i>نقل حقوق المسؤول</i>\n/ معلومات <i>المعلومات</i>\n/ <i>الإحصائيات</i> الإحصائية\n/ <i>سجلات عرض السجل</i>\n/ parse <i>[all | old | premium | active | online]</i>\n<code>/parse old</code> - <i>تحليل معرفات الحساب القديم</i>\n\n<b>⛏ أوامر للمسؤولين</b>\n/ ban 5m | 1h | 10d <i>إزالة مؤقتة من المجموعة</i>\n/ Unban\n/ mute 5m | 1h | 10d <i>وقت المجموعة</i>\n/ unmute\n/ warn + <i>تحذير</i> الفوضى\n/ status\n/ karma [+ | -]\n/ tag + <i>@tager</i> <i>random- حسابات</i>\n/ إيقاف <i>إضافة كلمة إيقاف</i>\n/ قناة NAME <i>إضافة قناة للتحقق من الاشتراك</i>\n/ زر NAME <i>إضافة اسم لزر التحكم في الإدخال</i>\n/ تأخير MIN <i>قم بتعيين الحد الأدنى للمبلغ لتأخير رسالة واحدة</i>\n/ إغراق NUM <i>قم بتعيين عدد الرسائل من أجل الفيضان</i>\n\n<b>⛏ أوامر المستخدم</b>\n/ <i>إخراج أمر</i> المساعدة\n/ <i>قواعد المجموعة</i>\n/ الإبلاغ عن <i>إساءة استخدام</i>\n/ سعيد <i>الحصول على الفرح</i>\n/ <i>شكرًا</i> جزيلاً",
+    'ru': "⚙️ <b>Настройка</b> группы <b>{0}</b> {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/update <i>обновление параметров</i>\n/transfer   <i>передача admin-прав</i>\n/info   <i>информация</i>\n/stat   <i>статистика</i>\n/log   <i>посмотреть логи</i>\n/parse  <i>[all|old|premium|active|online]</i>\n/parse old - <i>парсинг старых id-аккаунтов</i>\n\n<b>⛏ Команды администраторов</b>\n/ban 5m|1h|10d <i>удаление из группы на время</i>\n/unban\n/mute 5m|1h|10d <i>ограничение в группе на время</i>\n/unmute\n/warn+сообщ <i>предупреждение</i>\n/status\n/karma  [+|-]\n/tag+сообщ   <i>@tager random-аккаунтов</i>\n/stop  <i>добавить стоп-слово</i>\n/channel NAME   <i>добавить канал для проверки подписки</i>\n/button NAME    <i>добавить имя кнопки входного контроля</i>\n/delay MIN      <i>установить количество min для задержки 1го сообщ</i>\n/flood NUM      <i>установить количество сообщ для flood</i>\n\n<b>⛏ Команды пользователей</b>\n/help   <i>вывод команд</i>\n/rules  <i>правила группы</i>\n/report <i>сообщить о нарушении</i>\n/happy  <i>получить радость</i>\n/thanks <i>поблагодарить</i>",
+    'en': "⚙️ Group <b>setting</b> <b>{0}</b> {1}\n\n<b>⛏ Admin commands @{2}</b>\n/update <i>update parameters</i>\n/transfer <i>transfer admin rights</i>\n/info <i>information</i>\n/stat <i>statistics</i>\n/log <i>view logs</i>\n/parse <i>[all|old|premium|active|online]</i>\n/parse old - <i>parse old account ids</i>\n\n<b>⛏ Commands for administrators</b>\n/ban 5m|1h|10d <i>temporary removal from the group</i>\n/unban\n/mute 5m|1h|10d <i>group time limit</i>\n/unmute\n/warn+mess <i>warning</i>\n/status\n/karma [+|-]\n/tag+mess <i>@tager</i> <i>random- accounts</i>\n/stop <i>add a stopword</i>\n/channel NAME <i>add a channel for checking subscription</i>\n/button NAME <i>add a name for input control button</i>\n/delay MIN <i>set the min amount to delay 1 message</i>\n/flood NUM <i>set the number of messages for flood</i>\n\n<b>⛏ User commands</b>\n/help <i>command output</i>\n/rules <i>group rules</i>\n/report report <i>abuse</i>\n/happy <i>get joy</i>\n/thanks <i>thank</i>",
+    'es': "⚙️ <b>Configuración</b> de grupo <b>{0}</b> {1}\n\n<b>⛏ Comandos de administrador @{2}</b>\n/actualizar <i>actualizar parámetros</i>\n/transferir <i>transferir derechos de administrador</i>\n/ <i>información</i> de información\n/ <i>estadísticas</i>\n/registrar <i>ver registros</i> \ n/parse <i>[todos|antiguos|premium|activos|en línea]</i>\n/parse old : <i>analiza los ID de cuentas antiguos</i>\n\n<b>⛏ Comandos para administradores</b>\n/ban 5m|1h|10d <i>eliminación temporal del grupo</i>\n/unban\n/silencio 5m|1h| <i>límite de tiempo de grupo</i> 10d\n/no silenciar\n/advertencia+mensaje <i>advertencia</i>\n/estado\n/karma [+|-]\n/tag+mess <i>@tager</i> <i>cuentas aleatorias</i>\n/ detener <i>agregar una palabra vacía</i>\n/NOMBRE del canal <i>agregar un canal para verificar la suscripción</i>\n/NOMBRE del botón <i>agregar un nombre para el botón de control de entrada</i>\n/retardo MIN <i>establecer la cantidad mínima para retrasar 1 mensaje</i>\n/inundación NUM <i>establecer el número de mensajes para inundación</i>\n\n<b>⛏ Comandos de usuario</b>\n/ <i>salida de comando</i> de ayuda\n/ <i>reglas reglas de grupo</i>\n/informar informar <i>abuso</i>\n/feliz <i>obtener alegría</i>\n/gracias <i>gracias</i>",
+    'fr': "⚙️ <b>Paramètres</b> de groupe <b>{0}</b> {1}\n\n<b>⛏ Commandes d&#x27;administration @{2}</b>\n/mettre à jour <i>les paramètres de mise à jour</i>\n/transférer <i>les droits d&#x27;administrateur de transfert</i>\n/ <i>informations d&#x27;information</i>\n/ <i>statistiques</i>\n/journal <i>afficher les journaux</i> \ n/parse <i>[all|old|premium|active|online]</i>\n/parse old - <i>analyse les anciens identifiants de compte</i>\n\n<b>⛏ Commandes pour les administrateurs</b>\n/ban 5m|1h|10d <i>suppression temporaire du groupe</i>\n/unban\n/mute 5m|1h|10d <i>limite de temps de groupe</i>\n/unmute\n/warn+mess <i>warning</i>\n/status\n/karma [+|-]\n/tag+mess <i>@tager</i> <i>random- accounts</i>\n/ stop <i>ajouter un mot vide</i>\n/channel NAME <i>ajouter un canal pour vérifier l&#x27;abonnement</i>\n/button NAME <i>ajouter un nom pour le bouton de contrôle d&#x27;entrée</i>\n/delay MIN <i>définir le montant minimum pour retarder 1 message</i>\n/flood NUM <i>définir le nombre de messages for flood</i>\n\n<b>⛏ Commandes utilisateur</b>\n/ <i>sortie de la commande d&#x27;</i> aide\n/ <i>rules règles du groupe</i>\n/signaler signaler un <i>abus</i>\n/happy <i>get joy</i>\n/merci <i>merci</i>",
+    'zh': "⚙️ 群组<b>设置{0}</b> {1}\n\n<b>⛏ 管理员命令@{2}</b>\n/update<i>更新参数</i>\n/transfer<i>转移admin 权限</i>\n/info<i>信息</i>\n/stat<i>统计</i>\n/log<i>查看日志</i>\ n/parse <i>[all|old|premium|active|online]</i>\n/parse old -<i>解析旧帐户 ID</i>\n\n<b>⛏ 管理员命令</b>\n/ban 5m|1h|10d<i>临时从组中删除</i>\n/unban\n/mute 5m|1h|10d<i>群限时</i>\n/unmute\n/warn+mess<i>警告</i>\n/status\n/karma[+|-]\n/tag+mess <i>@tager</i> <i>random-accounts</i>\n/ stop<i>添加停用词</i>\n/channel NAME<i>添加检查订阅的频道</i>\n/button NAME<i>添加输入控制按钮的名称</i>\n/delay MIN<i>设置延迟 1 条消息的最小量</i>\n/flood NUM<i>设置消息数for flood</i>\n\n<b>⛏ 用户命令</b>\n/help<i>命令输出</i>\n/rules<i>组规则</i>\n/report 报告<i>滥用</i>\n/happy <i>get joy</i>\n/thanks <i>thank</i>",
+    'ar': "⚙️ <b>إعداد</b> المجموعة <b>{0}</b> {1}\n\n<b>⛏ أوامر المسؤول @ {2}</b>\n/ <i>تحديث المعلمات</i>\n/ <i>نقل حقوق المسؤول</i>\n/ معلومات <i>المعلومات</i>\n/ <i>الإحصائيات</i> الإحصائية\n/ <i>سجلات عرض السجل</i>\n/ parse <i>[all | old | premium | active | online]</i>\n/parse old - <i>تحليل معرفات الحساب القديم</i>\n\n<b>⛏ أوامر للمسؤولين</b>\n/ ban 5m | 1h | 10d <i>إزالة مؤقتة من المجموعة</i>\n/ Unban\n/ mute 5m | 1h | 10d <i>وقت المجموعة</i>\n/ unmute\n/ warn + <i>تحذير</i> الفوضى\n/ status\n/ karma [+ | -]\n/ tag + <i>@tager</i> <i>random- حسابات</i>\n/ إيقاف <i>إضافة كلمة إيقاف</i>\n/ قناة NAME <i>إضافة قناة للتحقق من الاشتراك</i>\n/ زر NAME <i>إضافة اسم لزر التحكم في الإدخال</i>\n/ تأخير MIN <i>قم بتعيين الحد الأدنى للمبلغ لتأخير رسالة واحدة</i>\n/ إغراق NUM <i>قم بتعيين عدد الرسائل من أجل الفيضان</i>\n\n<b>⛏ أوامر المستخدم</b>\n/ <i>إخراج أمر</i> المساعدة\n/ <i>قواعد المجموعة</i>\n/ الإبلاغ عن <i>إساءة استخدام</i>\n/ سعيد <i>الحصول على الفرح</i>\n/ <i>شكرًا</i> جزيلاً",
 }
 l_update_handler00 = {
     'ru': "🛡 Для дальнейшего <b>администрирования</b> данной группы запустите @{0}-бота и добавьте его в группу как <b>Administrator</b>",
     'en': "🛡 For further <b>administration</b> of this group, run the @{0}-bot and add it to the group as <b>Administrator</b>",
     'es': "🛡 Para una mayor <b>administración</b> de este grupo, ejecute @{0}-bot y agréguelo al grupo como <b>Administrador</b>",
     'fr': "🛡 Pour <b>une administration</b> plus poussée de ce groupe, exécutez le @{0}-bot et ajoutez-le au groupe en tant <b>qu&#x27;administrateur</b>",
     'zh': "🛡 要进一步<b>管理</b>该组，请运行 @{0}-bot 并将其作为<b>管理员</b>添加到组中",
@@ -4234,44 +4242,44 @@
     'en': "🛡 Group updated, but not connected to @{0}-bot! To further <b>administer</b> this group, go to the @{0}-bot and press /start",
     'es': "🛡 ¡Grupo actualizado, pero no conectado a @{0}-bot! Para seguir <b>administrando</b> este grupo, ve al @{0}-bot y presiona /start",
     'fr': "🛡 Groupe mis à jour, mais non connecté à @{0}-bot ! Pour <b>administrer</b> davantage ce groupe, accédez au @{0}-bot et appuyez sur /start",
     'zh': "🛡 组已更新，但未连接到@{0}-bot！要进一步<b>管理</b>该组，请转到 @{0}-bot 并按 /start",
     'ar': "🛡 تم تحديث المجموعة ولكنها غير مرتبطة بـ @ {0} -bot! <b>لإدارة</b> هذه المجموعة بشكل أكبر ، انتقل إلى @ {0} -bot واضغط / ابدأ",
 }
 l_group_info_start1 = {
-    'ru': "ℹ️ <b>Общая информация о группе</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
-    'en': "ℹ️ <b>General information about the group</b>\n\n<b>Name</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> members]{5}{6}{7}",
-    'es': "ℹ️ <b>Información general sobre el grupo</b>\n\n<b>Nombre</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> miembros]{5}{6}{7}",
-    'fr': "ℹ️ <b>Informations générales sur le groupe</b>\n\n<b>Nom</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> membres]{5}{6}{7}",
-    'zh': "ℹ️<b>有关群组的一般信息</b>\n\n<b>名称</b>：{0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u>成员]{5}{6}{7}",
-    'ar': "ℹ️ <b>معلومات عامة عن المجموعة</b>\n\n<b>الاسم</b> : {0} [id = <code>{1}</code> ، <i>{2} {3}</i> ، <u>{4}</u> الأعضاء] {5} {6} {7}",
+    'ru': "ℹ️ <b>Общая информация о группе</b>\n\n<b>Название</b>: {0} [id={1}, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
+    'en': "ℹ️ <b>General information about the group</b>\n\n<b>Name</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> members]{5}{6}{7}",
+    'es': "ℹ️ <b>Información general sobre el grupo</b>\n\n<b>Nombre</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> miembros]{5}{6}{7}",
+    'fr': "ℹ️ <b>Informations générales sur le groupe</b>\n\n<b>Nom</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> membres]{5}{6}{7}",
+    'zh': "ℹ️<b>有关群组的一般信息</b>\n\n<b>名称</b>：{0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u>成员]{5}{6}{7}",
+    'ar': "ℹ️ <b>معلومات عامة عن المجموعة</b>\n\n<b>الاسم</b> : {0} [id = {1} ، <i>{2} {3}</i> ، <u>{4}</u> الأعضاء] {5} {6} {7}",
 }
 l_group_stat_start = {
     'ru': "ℹ️ <b>Общая информация о статистике группы</b>\n\n",
     'en': "ℹ️ <b>General information about group statistics</b>\n\n",
     'es': "ℹ️ <b>Información general sobre las estadísticas del grupo</b>\n\n",
     'fr': "ℹ️ <b>Informations générales sur les statistiques de groupe</b>\n\n",
     'zh': "ℹ️<b>关于组统计的一般信息</b>\n\n",
     'ar': "ℹ️ <b>معلومات عامة حول إحصائيات المجموعة</b>\n\n",
 }
 l_group_stat_start1 = {
-    'ru': "ℹ️ <b>Общая статистика группы</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
-    'en': "ℹ️ <b>General group statistics</b>\n\n<b>Name</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> members]{5}{6}{7}",
-    'es': "ℹ️ <b>Estadísticas generales del grupo</b>\n\n<b>Nombre</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> miembros]{5}{6}{7}",
-    'fr': "ℹ️ <b>Statistiques générales du groupe</b>\n\n<b>Nom</b> : {0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u> membres]{5}{6}{7}",
-    'zh': "ℹ️<b>一般群组统计信息</b>\n\n<b>姓名</b>：{0} [id= <code>{1}</code> , <i>{2} {3}</i> , <u>{4}</u>成员]{5}{6}{7}",
-    'ar': "ℹ️ <b>إحصائيات عامة للمجموعة</b>\n\n<b>الاسم</b> : {0} [id = <code>{1}</code> ، <i>{2} {3}</i> ، <u>{4}</u> أعضاء] {5} {6} {7}",
+    'ru': "ℹ️ <b>Общая статистика группы</b>\n\n<b>Название</b>: {0} [id={1}, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
+    'en': "ℹ️ <b>General group statistics</b>\n\n<b>Name</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> members]{5}{6}{7}",
+    'es': "ℹ️ <b>Estadísticas generales del grupo</b>\n\n<b>Nombre</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> miembros]{5}{6}{7}",
+    'fr': "ℹ️ <b>Statistiques générales du groupe</b>\n\n<b>Nom</b> : {0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u> membres]{5}{6}{7}",
+    'zh': "ℹ️<b>一般群组统计信息</b>\n\n<b>姓名</b>：{0} [id= {1} , <i>{2} {3}</i> , <u>{4}</u>成员]{5}{6}{7}",
+    'ar': "ℹ️ <b>إحصائيات عامة للمجموعة</b>\n\n<b>الاسم</b> : {0} [id = {1} ، <i>{2} {3}</i> ، <u>{4}</u> أعضاء] {5} {6} {7}",
 }
 l_group_stat_start2 = {
-    'ru': "\n<b>Ссылка</b>: {0}\n<b>Описание</b>: {1}\n<b>Привязанный канал</b>: <code>{2}</code>\n",
-    'en': "\n<b>Link</b> : {0}\n<b>Description</b> : {1}\n<b>Link channel</b> : <code>{2}</code>\n",
-    'es': "\n<b>Enlace</b> : {0}\n<b>Descripción</b> : {1}\n<b>Canal de enlace</b> : <code>{2}</code>\n",
-    'fr': "\n<b>Lien</b> : {0}\n<b>Description</b> : {1}\n<b>Lien canal</b> : <code>{2}</code>\n",
-    'zh': "\n<b>链接</b>：{0}\n<b>描述</b>：{1}\n<b>链接通道</b>： <code>{2}</code>\n",
-    'ar': "\n<b>الارتباط</b> : {0}\n<b>الوصف</b> : {1}\n<b>قناة الارتباط</b> : <code>{2}</code>\n",
+    'ru': "\n<b>Ссылка</b>: {0}\n<b>Описание</b>: {1}\n<b>Привязанный канал</b>: {2}\n",
+    'en': "\n<b>Link</b> : {0}\n<b>Description</b> : {1}\n<b>Link channel</b> : {2}\n",
+    'es': "\n<b>Enlace</b> : {0}\n<b>Descripción</b> : {1}\n<b>Canal de enlace</b> : {2}\n",
+    'fr': "\n<b>Lien</b> : {0}\n<b>Description</b> : {1}\n<b>Lien canal</b> : {2}\n",
+    'zh': "\n<b>链接</b>：{0}\n<b>描述</b>：{1}\n<b>链接通道</b>： {2}\n",
+    'ar': "\n<b>الارتباط</b> : {0}\n<b>الوصف</b> : {1}\n<b>قناة الارتباط</b> : {2}\n",
 }
 l_group_stat_start3 = {
     'ru': "<b>Сообщения</b>: {0}\n<b>Дата 1го сообщ</b>: ~{1}\n<b>ID последнего сообщ</b>: {2}\n",
     'en': "<b>Messages</b> : {0}\n<b>Date of 1st message</b> : ~{1}\n<b>Last message ID</b> : {2}\n",
     'es': "<b>Mensajes</b> : {0}\n<b>Fecha del primer mensaje</b> : ~{1}\n<b>ID del último mensaje</b> : {2}\n",
     'fr': "<b>Messages</b> : {0}\n<b>Date du 1er message</b> : ~{1}\n<b>ID du dernier message</b> : {2}\n",
     'zh': "<b>消息</b>：{0}\n<b>第一条消息的日期</b>：~{1}\n<b>最后一条消息 ID</b> ：{2}\n",
@@ -4282,44 +4290,44 @@
     'en': "participation.",
     'es': "participación.",
     'fr': "participation.",
     'zh': "参与。",
     'ar': "مشاركة.",
 }
 l_info_opportunity = {
-    'ru': "<b>Возможность просмотра увидевших сообщ</b>: <code>Да (до 50участ.)</code>\n",
-    'en': "<b>Ability to View Seen Messages</b> : <code>Да (до 50участ.)</code>\n",
-    'es': "<b>Capacidad para ver mensajes vistos</b> : <code>Да (до 50участ.)</code>\n",
-    'fr': "<b>Possibilité d&#x27;afficher les messages vus</b> : <code>Да (до 50участ.)</code>\n",
-    'zh': "<b>查看已读消息的能力</b>： <code>Да (до 50участ.)</code>\n",
-    'ar': "<b>القدرة على عرض الرسائل المرئية</b> : <code>Да (до 50участ.)</code>\n",
+    'ru': "<b>Возможность просмотра увидевших сообщ</b>: Да (до 50участ.)\n",
+    'en': "<b>Ability to View Seen Messages</b> : Да (до 50участ.)\n",
+    'es': "<b>Capacidad para ver mensajes vistos</b> : Да (до 50участ.)\n",
+    'fr': "<b>Possibilité d&#x27;afficher les messages vus</b> : Да (до 50участ.)\n",
+    'zh': "<b>查看已读消息的能力</b>： Да (до 50участ.)\n",
+    'ar': "<b>القدرة على عرض الرسائل المرئية</b> : Да (до 50участ.)\n",
 }
 l_info_history = {
     'ru': "<b>История для новых участников</b>: ",
     'en': "<b>History for new members</b> :",
     'es': "<b>Historial para nuevos miembros</b> :",
     'fr': "<b>Historique pour les nouveaux membres</b> :",
     'zh': "<b>新成员的历史</b>：",
     'ar': "<b>التاريخ للأعضاء الجدد</b> :",
 }
 l_info_history_show = {
-    'ru': "<code>видна</code>\n",
-    'en': "<code>видна</code>\n",
-    'es': "<code>видна</code>\n",
-    'fr': "<code>видна</code>\n",
-    'zh': "<code>видна</code>\n",
-    'ar': "<code>видна</code>\n",
+    'ru': "видна\n",
+    'en': "видна\n",
+    'es': "видна\n",
+    'fr': "видна\n",
+    'zh': "видна\n",
+    'ar': "видна\n",
 }
 l_info_history_hide = {
-    'ru': "<code>скрыта</code>\n",
-    'en': "<code>скрыта</code>\n",
-    'es': "<code>скрыта</code>\n",
-    'fr': "<code>скрыта</code>\n",
-    'zh': "<code>скрыта</code>\n",
-    'ar': "<code>скрыта</code>\n",
+    'ru': "скрыта\n",
+    'en': "скрыта\n",
+    'es': "скрыта\n",
+    'fr': "скрыта\n",
+    'zh': "скрыта\n",
+    'ar': "скрыта\n",
 }
 l_info_autodel = {
     'ru': "<b>Автоудаление сообщений</b>: ",
     'en': "<b>Auto delete messages</b> :",
     'es': "<b>Eliminar mensajes automáticamente</b> :",
     'fr': "<b>Supprimer automatiquement les messages</b> :",
     'zh': "<b>自动删除消息</b>：",
@@ -4330,20 +4338,20 @@
     'en': "<b>How often can you write</b> :",
     'es': "<b>¿Con qué frecuencia puede escribir</b> :",
     'fr': "<b>À quelle fréquence pouvez-vous écrire</b> :",
     'zh': "<b>你多久可以写一次</b>：",
     'ar': "<b>كم مرة يمكنك أن تكتب</b> :",
 }
 l_info_slowmode_limitless = {
-    'ru': "<code>без ограничений</code>\n",
-    'en': "<code>без ограничений</code>\n",
-    'es': "<code>без ограничений</code>\n",
-    'fr': "<code>без ограничений</code>\n",
-    'zh': "<code>без ограничений</code>\n",
-    'ar': "<code>без ограничений</code>\n",
+    'ru': "без ограничений\n",
+    'en': "без ограничений\n",
+    'es': "без ограничений\n",
+    'fr': "без ограничений\n",
+    'zh': "без ограничений\n",
+    'ar': "без ограничений\n",
 }
 l_info_oppforpart = {
     'ru': "Возможности участников",
     'en': "Member Opportunities",
     'es': "Oportunidades para miembros",
     'fr': "Opportunités pour les membres",
     'zh': "会员机会",
@@ -4508,20 +4516,20 @@
     'en': "👮🏽 <b>Done!</b> The current <b>button name</b> on <i>the input control</i> is set to: {0}",
     'es': "👮🏽 <b>Listo!</b> El <b>nombre del botón</b> actual en <i>el control de entrada</i> se establece en: {0}",
     'fr': "👮🏽 <b>C&#x27;est fait !</b> Le <b>nom actuel du bouton</b> sur <i>le contrôle d&#x27;entrée</i> est défini sur : {0}",
     'zh': "👮🏽<b>完成！</b><i>输入控件</i>上的当前<b>按钮名称</b>设置为：{0}",
     'ar': "👮🏽 <b>انتهى!</b> تم تعيين <b>اسم الزر</b> الحالي في <i>عنصر تحكم الإدخال</i> على: {0}",
 }
 l_button_correct = {
-    'ru': "👮🏽 <b>Введи</b> корректное название <i>для имени кнопки</i> Входного контроля\n\n👉🏼 Например, <code>/button {0}</code>",
-    'en': "👮🏽 <b>Please enter</b> a valid name <i>for the Input Control button name</i>\n\n👉🏼 For example, <code>/button {0}</code>",
-    'es': "👮🏽 <b>Ingrese</b> un nombre válido <i>para el nombre del botón de control de entrada</i>\n\n👉🏼 Por ejemplo, <code>/button {0}</code>",
-    'fr': "👮🏽 <b>Veuillez saisir</b> un nom valide <i>pour le nom du bouton de contrôle d&#x27;entrée</i>\n\n👉🏼 Par exemple, <code>/button {0}</code>",
-    'zh': "👮🏽 请<i>为输入控件按钮名称</i><b>输入</b>有效名称\n\n👉🏼 例如， <code>/button {0}</code>",
-    'ar': "👮🏽 <b>الرجاء إدخال</b> اسم صالح <i>لاسم زر التحكم في الإدخال</i>\n\n👉🏼 على سبيل المثال ، <code>/button {0}</code>",
+    'ru': "👮🏽 <b>Введи</b> корректное название <i>для имени кнопки</i> Входного контроля\n\n👉🏼 Например, /button {0}",
+    'en': "👮🏽 <b>Please enter</b> a valid name <i>for the Input Control button name</i>\n\n👉🏼 For example, /button {0}",
+    'es': "👮🏽 <b>Ingrese</b> un nombre válido <i>para el nombre del botón de control de entrada</i>\n\n👉🏼 Por ejemplo, /button {0}",
+    'fr': "👮🏽 <b>Veuillez saisir</b> un nom valide <i>pour le nom du bouton de contrôle d&#x27;entrée</i>\n\n👉🏼 Par exemple, /button {0}",
+    'zh': "👮🏽 请<i>为输入控件按钮名称</i><b>输入</b>有效名称\n\n👉🏼 例如， /button {0}",
+    'ar': "👮🏽 <b>الرجاء إدخال</b> اسم صالح <i>لاسم زر التحكم في الإدخال</i>\n\n👉🏼 على سبيل المثال ، /button {0}",
 }
 l_channel_check = {
     'ru': "⚙️ Добавь @{0}-бота в канал для проверки подписки на него. Пришли мне корректную ссылку на канал:",
     'en': "⚙️ Add @{0}-bot to the channel to check if you subscribe to it. Send me the correct link to the channel:",
     'es': "⚙️ Agrega @{0}-bot al canal para comprobar si estás suscrito. Envíame el enlace correcto al canal:",
     'fr': "⚙️ Ajoutez @{0}-bot à la chaîne pour vérifier si vous y êtes abonné. Envoyez-moi le bon lien vers la chaîne :",
     'zh': "⚙️ 将@{0}-bot 添加到频道以检查您是否订阅了它。向我发送正确的频道链接：",
@@ -4532,28 +4540,28 @@
     'en': "👮🏽 <b>Done!</b> Checking subscription to {0} is configured\n\nThe option can be enabled in the settings by pressing [✅☑Enable subscription]",
     'es': "👮🏽 <b>Listo!</b> Verificar que la suscripción a {0} está configurada\n\nLa opción se puede habilitar en la configuración presionando [✅☑Habilitar suscripción]",
     'fr': "👮🏽 <b>C&#x27;est fait !</b> Vérifier que l'abonnement à {0} est configuré\n\nL'option peut être activée dans les paramètres en appuyant sur [✅☑Activer l'abonnement]",
     'zh': "👮🏽<b>完成！</b>检查对 {0} 的订阅是否已配置\n\n可以通过按 [✅☑启用订阅] 在设置中启用该选项",
     'ar': "👮🏽 <b>انتهى!</b> التحقق من الاشتراك في {0} مهيأ\n\nيمكن تمكين الخيار في الإعدادات بالضغط على [✅☑ تمكين الاشتراك]",
 }
 l_channel_correct = {
-    'ru': "👮🏽 Добавь @{0}-бота в канал и отправь корректную <i>ссылку</i> этого канала\n\n👉🏼 Например, <code>/channel @{1}</code>",
-    'en': "👮🏽 Add @{0}-bot to the channel and send the correct <i>link</i> of this channel\n\n👉🏼 For example, <code>/channel @{1}</code>",
-    'es': "👮🏽 Agrega @{0}-bot al canal y envía el <i>enlace</i> correcto de este canal\n\n👉🏼 Por ejemplo, <code>/channel @{1}</code>",
-    'fr': "👮🏽 Ajoutez @{0}-bot au canal et envoyez le <i>lien</i> correct de ce canal\n\n👉🏼 Par exemple, <code>/channel @{1}</code>",
-    'zh': "👮🏽 将@{0}-bot 添加到频道并发送该频道的正确<i>链接</i>\n\n👉🏼 例如， <code>/channel @{1}</code>",
-    'ar': "👮🏽 Add @ {0} -bot إلى القناة وأرسل <i>الرابط</i> الصحيح لهذه القناة\n\n👉🏼 على سبيل المثال ، <code>/channel @{1}</code>",
+    'ru': "👮🏽 Добавь @{0}-бота в канал и отправь корректную <i>ссылку</i> этого канала\n\n👉🏼 Например, /channel @{1}",
+    'en': "👮🏽 Add @{0}-bot to the channel and send the correct <i>link</i> of this channel\n\n👉🏼 For example, /channel @{1}",
+    'es': "👮🏽 Agrega @{0}-bot al canal y envía el <i>enlace</i> correcto de este canal\n\n👉🏼 Por ejemplo, /channel @{1}",
+    'fr': "👮🏽 Ajoutez @{0}-bot au canal et envoyez le <i>lien</i> correct de ce canal\n\n👉🏼 Par exemple, /channel @{1}",
+    'zh': "👮🏽 将@{0}-bot 添加到频道并发送该频道的正确<i>链接</i>\n\n👉🏼 例如， /channel @{1}",
+    'ar': "👮🏽 Add @ {0} -bot إلى القناة وأرسل <i>الرابط</i> الصحيح لهذه القناة\n\n👉🏼 على سبيل المثال ، /channel @{1}",
 }
 l_delay_correct = {
-    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Например, <code>/delay 1</code>\n\nИли используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
-    'en': "👥 <b>Enter</b> the correct <i>number of</i> minutes to limit new users for the first time\n\n👉🏼 For example, <code>/delay 1</code>\n\nOr use <b>slow mode</b> in group settings for <u>1</u> message",
-    'es': "👥 <b>Ingrese</b> la <i>cantidad correcta de</i> minutos para limitar nuevos usuarios por primera vez\n\n👉🏼 Por ejemplo, <code>/delay 1</code>\n\nO use <b>el modo lento</b> en la configuración del grupo para <u>1</u> mensaje",
-    'fr': "👥 <b>Entrez</b> le <i>nombre correct de</i> minutes pour limiter les nouveaux utilisateurs pour la première fois\n\n👉🏼 Par exemple, <code>/delay 1</code>\n\nOu utilisez <b>le mode lent</b> dans les paramètres de groupe pour <u>1</u> message",
-    'zh': "👥 第一次<b>输入</b>正确的分钟<i>数</i>限制新用户\n\n👉🏼 例如<code>/delay 1</code>\n\n或者在群设置中使用<b>慢速模式</b><u>1条</u>消息",
-    'ar': "👥 <b>أدخل</b> <i>العدد</i> الصحيح للدقائق لتقييد المستخدمين الجدد لأول مرة\n\n👉🏼 على سبيل المثال ، <code>/delay 1</code>\n\nأو استخدم <b>الوضع البطيء</b> في إعدادات المجموعة لرسالة <u>واحدة</u>",
+    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Например, /delay 1\n\nИли используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
+    'en': "👥 <b>Enter</b> the correct <i>number of</i> minutes to limit new users for the first time\n\n👉🏼 For example, /delay 1\n\nOr use <b>slow mode</b> in group settings for <u>1</u> message",
+    'es': "👥 <b>Ingrese</b> la <i>cantidad correcta de</i> minutos para limitar nuevos usuarios por primera vez\n\n👉🏼 Por ejemplo, /delay 1\n\nO use <b>el modo lento</b> en la configuración del grupo para <u>1</u> mensaje",
+    'fr': "👥 <b>Entrez</b> le <i>nombre correct de</i> minutes pour limiter les nouveaux utilisateurs pour la première fois\n\n👉🏼 Par exemple, /delay 1\n\nOu utilisez <b>le mode lent</b> dans les paramètres de groupe pour <u>1</u> message",
+    'zh': "👥 第一次<b>输入</b>正确的分钟<i>数</i>限制新用户\n\n👉🏼 例如/delay 1\n\n或者在群设置中使用<b>慢速模式</b><u>1条</u>消息",
+    'ar': "👥 <b>أدخل</b> <i>العدد</i> الصحيح للدقائق لتقييد المستخدمين الجدد لأول مرة\n\n👉🏼 على سبيل المثال ، /delay 1\n\nأو استخدم <b>الوضع البطيء</b> في إعدادات المجموعة لرسالة <u>واحدة</u>",
 }
 l_parse_error = {
     'ru': "📇 Осуществить парсинг пользователей  не удалось",
     'en': "📇 Failed to parse users",
     'es': "📇 No se pudieron analizar los usuarios",
     'fr': "📇 Échec de l'analyse des utilisateurs",
     'zh': "📇 解析用户失败",
@@ -4789,28 +4797,28 @@
     'en': "🥳 Send this command as a reply to a message",
     'es': "🥳 Envía este comando como respuesta a un mensaje",
     'fr': "🥳 Envoyez cette commande en réponse à un message",
     'zh': "🥳 发送此命令作为对消息的回复",
     'ar': "🥳 أرسل هذا الأمر كرد على رسالة",
 }
 l_videochat_text = {
-    'ru': "🎥 Автоматическое анонсирование <b>видео-трансляции</b> <code>[/videochat d h]</code> каждый <u>d</u>-день (1-31) на <u>h</u>-часов (1-168). Текущее значение: /videochat {0}\n\n👩🏽‍💻 Например,\n<code>/videochat 1 1</code> (ежедневный видео-анонс длительностью 1 час)\n<code>/videochat 0</code> (отключение опции)",
-    'en': "🎥 Automatic announcement <b>of the video broadcast</b> <code>[/videochat dh]</code> every <u>d</u> -day (1-31) for <u>h</u> -hours (1-168). Current value: /videochat {0}\n\n👩🏽‍💻 For example\n<code>/videochat 1 1</code> (daily 1 hour video announcement)\n<code>/videochat 0</code> (disable option)",
-    'es': "🎥 Anuncio automático <b>de la transmisión de video</b> <code>[/videochat dh]</code> cada <u>d</u> -día (1-31) durante <u>h</u> -horas (1-168). Valor actual: /videochat {0}\n\n👩🏽‍💻 Por ejemplo\n<code>/videochat 1 1</code> (anuncio de video diario de 1 hora)\n<code>/videochat 0</code> (opción deshabilitada)",
-    'fr': "🎥 Annonce automatique <b>de la diffusion vidéo</b> <code>[/videochat dh]</code> tous <u>les j</u> -jours (1-31) pendant <u>h</u> -heures (1-168). Valeur actuelle : /videochat {0}\n\n👩🏽‍💻 Par exemple\n<code>/videochat 1 1</code> (annonce vidéo quotidienne d&#x27;une heure)\n<code>/videochat 0</code> (option de désactivation)",
-    'zh': "🎥 每<u>d</u>天（1-31）自动播报<b>视频广播</b><code>[/videochat dh]</code> ，持续<u>h</u>小时（1-168）。当前值：/videochat {0}\n\n👩🏽‍💻 例如\n<code>/videochat 1 1</code> （每天1小时视频公告）\n<code>/videochat 0</code> （禁用选项）",
-    'ar': "🎥 الإعلان التلقائي <b>عن بث الفيديو</b> <code>[/videochat dh]</code> كل يوم <u>يوم</u> (1-31) لمدة <u>ساعة</u> (1-168). القيمة الحالية: / videochat {0}\n\n👩🏽‍💻 على سبيل المثال\n<code>/videochat 1 1</code> (إعلان فيديو لمدة ساعة يوميًا)\n<code>/videochat 0</code> (خيار تعطيل)",
+    'ru': "🎥 Автоматическое анонсирование <b>видео-трансляции</b> [/videochat d h] каждый <u>d</u>-день (1-31) на <u>h</u>-часов (1-168). Текущее значение: /videochat {0}\n\n👩🏽‍💻 Например,\n/videochat 1 1 (ежедневный видео-анонс длительностью 1 час)\n/videochat 0 (отключение опции)",
+    'en': "🎥 Automatic announcement <b>of the video broadcast</b> [/videochat dh] every <u>d</u> -day (1-31) for <u>h</u> -hours (1-168). Current value: /videochat {0}\n\n👩🏽‍💻 For example\n/videochat 1 1 (daily 1 hour video announcement)\n/videochat 0 (disable option)",
+    'es': "🎥 Anuncio automático <b>de la transmisión de video</b> [/videochat dh] cada <u>d</u> -día (1-31) durante <u>h</u> -horas (1-168). Valor actual: /videochat {0}\n\n👩🏽‍💻 Por ejemplo\n/videochat 1 1 (anuncio de video diario de 1 hora)\n/videochat 0 (opción deshabilitada)",
+    'fr': "🎥 Annonce automatique <b>de la diffusion vidéo</b> [/videochat dh] tous <u>les j</u> -jours (1-31) pendant <u>h</u> -heures (1-168). Valeur actuelle : /videochat {0}\n\n👩🏽‍💻 Par exemple\n/videochat 1 1 (annonce vidéo quotidienne d&#x27;une heure)\n/videochat 0 (option de désactivation)",
+    'zh': "🎥 每<u>d</u>天（1-31）自动播报<b>视频广播</b>[/videochat dh] ，持续<u>h</u>小时（1-168）。当前值：/videochat {0}\n\n👩🏽‍💻 例如\n/videochat 1 1 （每天1小时视频公告）\n/videochat 0 （禁用选项）",
+    'ar': "🎥 الإعلان التلقائي <b>عن بث الفيديو</b> [/videochat dh] كل يوم <u>يوم</u> (1-31) لمدة <u>ساعة</u> (1-168). القيمة الحالية: / videochat {0}\n\n👩🏽‍💻 على سبيل المثال\n/videochat 1 1 (إعلان فيديو لمدة ساعة يوميًا)\n/videochat 0 (خيار تعطيل)",
 }
 l_flood_text = {
-    'ru': "💬 <b>Введи</b> корректное <i>число</i> сообщений от <u>3</u> до <u>10</u>\n\n👉🏼 <b>Текущее</b> значение <code>/flood {0}</code>\n\n👩🏽‍💻 Например, /flood 3 (идентификация 3х сообщений подряд как flood)\n/flood 0 (отключение опции)",
-    'en': "💬 Please <b>enter</b> a valid <i>number</i> of messages from <u>3</u> to <u>10</u>\n\n👉🏼 <b>Current</b> value <code>/flood {0}</code>\n\n👩🏽‍💻 For example, /flood 3 (identifies 3 messages in a row as a flood)\n/flood 0 (disables options)",
-    'es': "💬 <b>Ingrese</b> un <i>número</i> válido de mensajes de <u>3</u> a <u>10</u>\n\n👉🏼 Valor <b>actual</b> <code>/flood {0}</code>\n\n👩🏽‍💻 Por ejemplo, /inundación 3 (identifica 3 mensajes seguidos como una inundación)\n/inundación 0 (deshabilita opciones)",
-    'fr': "💬 Veuillez <b>entrer</b> un <i>nombre</i> valide de messages de <u>3</u> à <u>10</u>\n\n👉🏼 Valeur <b>actuelle</b> <code>/flood {0}</code>\n\n👩🏽‍💻 Par exemple, /flood 3 (identifie 3 messages à la suite comme une inondation)\n/flood 0 (désactive les options)",
-    'zh': "💬<b>请输入</b><u>3</u>到<u>10</u>之间的有效消息<i>数</i>\n\n👉🏼<b>当前</b>值<code>/flood {0}</code>\n\n👩🏽‍💻 例如 /flood 3（连续 3 条消息标识为洪水）\n/flood 0（禁用选项）",
-    'ar': "💬 الرجاء <b>إدخال</b> <i>رقم</i> صالح للرسائل من <u>3</u> إلى <u>10</u>\n\n👉🏼 القيمة <b>الحالية</b> <code>/flood {0}</code>\n\n👩🏽‍💻 على سبيل المثال ، / فيضان 3 (يحدد 3 رسائل في صف واحد كفيضان)\n/ فيضان 0 (تعطيل الخيارات)",
+    'ru': "💬 <b>Введи</b> корректное <i>число</i> сообщений от <u>3</u> до <u>10</u>\n\n👉🏼 <b>Текущее</b> значение /flood {0}\n\n👩🏽‍💻 Например, /flood 3 (идентификация 3х сообщений подряд как flood)\n/flood 0 (отключение опции)",
+    'en': "💬 Please <b>enter</b> a valid <i>number</i> of messages from <u>3</u> to <u>10</u>\n\n👉🏼 <b>Current</b> value /flood {0}\n\n👩🏽‍💻 For example, /flood 3 (identifies 3 messages in a row as a flood)\n/flood 0 (disables options)",
+    'es': "💬 <b>Ingrese</b> un <i>número</i> válido de mensajes de <u>3</u> a <u>10</u>\n\n👉🏼 Valor <b>actual</b> /flood {0}\n\n👩🏽‍💻 Por ejemplo, /inundación 3 (identifica 3 mensajes seguidos como una inundación)\n/inundación 0 (deshabilita opciones)",
+    'fr': "💬 Veuillez <b>entrer</b> un <i>nombre</i> valide de messages de <u>3</u> à <u>10</u>\n\n👉🏼 Valeur <b>actuelle</b> /flood {0}\n\n👩🏽‍💻 Par exemple, /flood 3 (identifie 3 messages à la suite comme une inondation)\n/flood 0 (désactive les options)",
+    'zh': "💬<b>请输入</b><u>3</u>到<u>10</u>之间的有效消息<i>数</i>\n\n👉🏼<b>当前</b>值/flood {0}\n\n👩🏽‍💻 例如 /flood 3（连续 3 条消息标识为洪水）\n/flood 0（禁用选项）",
+    'ar': "💬 الرجاء <b>إدخال</b> <i>رقم</i> صالح للرسائل من <u>3</u> إلى <u>10</u>\n\n👉🏼 القيمة <b>الحالية</b> /flood {0}\n\n👩🏽‍💻 على سبيل المثال ، / فيضان 3 (يحدد 3 رسائل في صف واحد كفيضان)\n/ فيضان 0 (تعطيل الخيارات)",
 }
 l_flood_on = {
     'ru': "💬 <b>Установлен</b> flood-режим: {0} сообщения подряд",
     'en': "💬 Set flood mode: {0} messages in a row",
     'es': "💬 Establecer modo de inundación: {0} mensajes seguidos",
     'fr': "💬 Définir le mode flood : {0} messages d'affilée",
     'zh': "💬 设置泛洪模式：连续 {0} 条消息",
@@ -4821,20 +4829,20 @@
     'en': "💬 Flood mode disabled",
     'es': "💬 Modo de inundación deshabilitado",
     'fr': "💬 Mode inondation désactivé",
     'zh': "💬洪水模式禁用",
     'ar': "💬 وضع الفيضان معطل",
 }
 l_delay_text = {
-    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 <b>Текущее</b> значение <code>/delay {0}</code>\n\n👩🏽‍💻 Например, /delay 3 (ограничение на 3 min)\n/delay 0 (отключение опции)",
-    'en': "👥 <b>Please enter</b> the correct <i>number</i> of minutes for the initial limit of new users\n\n👉🏼 <b>The current</b> value of <code>/delay {0}</code>\n\n👩🏽‍💻 For example, /delay 3 (3 min limit)\n/delay 0 (disable option )",
-    'es': "👥 <b>Ingrese</b> la <i>cantidad</i> correcta de minutos para el límite inicial de nuevos usuarios\n\n👉🏼 <b>El valor actual</b> de <code>/delay {0}</code>\n\n👩🏽‍💻 Por ejemplo, /delay 3 (límite de 3 min)\ n/delay 0 (opción deshabilitar)",
-    'fr': "👥 <b>Veuillez entrer</b> le <i>nombre</i> correct de minutes pour la limite initiale de nouveaux utilisateurs\n\n👉🏼 <b>La valeur actuelle</b> de <code>/delay {0}</code>\n\n👩🏽‍💻 Par exemple, /delay 3 (3 min limit)\ n/délai 0 (désactiver l'option )",
-    'zh': "👥<b>请输入</b>正确的新用户初始限制分钟<i>数</i>\n\n👉🏼 <code>/delay {0}</code><b>当前</b>值{0}\n\n👩🏽‍💻 例如/delay 3（3分钟限制）\ n/delay 0（禁用选项）",
-    'ar': "👥 <b>الرجاء إدخال</b> <i>العدد</i> الصحيح للدقائق للحد الأولي للمستخدمين الجدد\n\n👉🏼 القيمة <b>الحالية</b> لـ <code>/delay {0}</code>\n\n👩🏽‍💻 على سبيل المثال ، / delay 3 (3 min limit) \ ن / تأخير 0 (تعطيل الخيار)",
+    'ru': "👥 <b>Введи</b> корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 <b>Текущее</b> значение /delay {0}\n\n👩🏽‍💻 Например, /delay 3 (ограничение на 3 min)\n/delay 0 (отключение опции)",
+    'en': "👥 <b>Please enter</b> the correct <i>number</i> of minutes for the initial limit of new users\n\n👉🏼 <b>The current</b> value of /delay {0}\n\n👩🏽‍💻 For example, /delay 3 (3 min limit)\n/delay 0 (disable option )",
+    'es': "👥 <b>Ingrese</b> la <i>cantidad</i> correcta de minutos para el límite inicial de nuevos usuarios\n\n👉🏼 <b>El valor actual</b> de /delay {0}\n\n👩🏽‍💻 Por ejemplo, /delay 3 (límite de 3 min)\ n/delay 0 (opción deshabilitar)",
+    'fr': "👥 <b>Veuillez entrer</b> le <i>nombre</i> correct de minutes pour la limite initiale de nouveaux utilisateurs\n\n👉🏼 <b>La valeur actuelle</b> de /delay {0}\n\n👩🏽‍💻 Par exemple, /delay 3 (3 min limit)\ n/délai 0 (désactiver l'option )",
+    'zh': "👥<b>请输入</b>正确的新用户初始限制分钟<i>数</i>\n\n👉🏼 /delay {0}<b>当前</b>值{0}\n\n👩🏽‍💻 例如/delay 3（3分钟限制）\ n/delay 0（禁用选项）",
+    'ar': "👥 <b>الرجاء إدخال</b> <i>العدد</i> الصحيح للدقائق للحد الأولي للمستخدمين الجدد\n\n👉🏼 القيمة <b>الحالية</b> لـ /delay {0}\n\n👩🏽‍💻 على سبيل المثال ، / delay 3 (3 min limit) \ ن / تأخير 0 (تعطيل الخيار)",
 }
 l_delay_on = {
     'ru': "👥 <b>Готово!</b> Текущая первичная задержка для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) установлена в значение <u>{0}</u> min",
     'en': "👥 <b>Done!</b> The current initial delay for <u>new</u> users (before writing their <u>1st</u> message) is set to <u>{0}</u> min",
     'es': "👥 <b>Listo!</b> El retraso inicial actual para <u>nuevos</u> usuarios (antes de escribir su <u>primer</u> mensaje) se establece en <u>{0}</u> min",
     'fr': "👥 <b>C&#x27;est fait !</b> Le délai initial actuel pour <u>les nouveaux</u> utilisateurs (avant d&#x27;écrire leur <u>1er</u> message) est défini sur <u>{0}</u> min",
     'zh': "👥<b>完成！</b><u>新</u>用户的当前初始延迟（在编写他们的<u>第一条</u>消息之前）设置为<u>{0}</u>分钟",
@@ -4873,20 +4881,20 @@
     'ar': "👉🏼 لم يتم تعيين <b>القواعد</b> في المجموعة <b>{0}</b> . <u>قم بالرد على منشور</u> بالقواعد باستخدام <b>الأمر</b> / rules",
 }
 # endregion
 
 
 # region ccheck
 l_ccheck_handler = {
-    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> в группу\n\n👉🏼 Для установки имени <b>нажимаемой кнопки</b>, выполни команду: <code>/button {0}</code>\n\n👉🏼 Для <b>проверки подписки</b> на канал <i>добавь</i> @{1}-бота в канал и выполни команду: <code>/channel {2}</code>\n\n👉🏼 Для <i>защиты от атаки</i> на группу включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
-    'en': "👮🏽 <b>Click</b> on ✅/🔘 to <b>switch</b> the type of user <i>verification</i> when <u>joining</u> a group\n\n👉🏼 To set the name <b>of the button to be pressed</b> , run the command: <code>/button {0}</code>\n\n👉🏼 To <b>check the subscription</b> to the channel <i>, add</i> @ {1}-bot into the channel and execute the command: <code>/channel {2}</code>\n\n👉🏼 To <i>protect against an attack</i> on the group, turn on the <b>anti-raid</b> mode (blocking <u>all</u> joiners)",
-    'es': "👮🏽 <b>Haz clic</b> en ✅/🔘 para <b>cambiar</b> el tipo de <i>verificación</i> de usuario al <u>unirte a</u> un grupo\n\n👉🏼 Para establecer el nombre <b>del botón que se presionará</b> , ejecuta el comando: <code>/button {0}</code>\n\n👉🏼 Para <b>verificar la suscripción</b> al canal <i>, agregue</i> @ {1}-bot al canal y ejecute el comando: <code>/channel {2}</code>\n\n👉🏼 Para <i>protegerse contra un ataque</i> al grupo, active el modo <b>anti-raid</b> (bloqueando <u>a todos</u> los carpinteros)",
-    'fr': "👮🏽 <b>Cliquez</b> sur ✅/🔘 pour <b>changer</b> le type de <i>vérification</i> de l&#x27;utilisateur lors <u>de l&#x27;adhésion à</u> un groupe\n\n👉🏼 Pour définir le nom <b>du bouton à appuyer</b> , exécutez la commande : <code>/button {0}</code>\n\n👉🏼 Pour <b>vérifier l&#x27;abonnement</b> au canal <i>, ajoutez</i> @{1}-bot dans le canal et exécutez la commande : <code>/channel {2}</code>\n\n👉🏼 Pour <i>vous protéger contre une attaque</i> sur le groupe, activez le mode <b>anti-raid</b> (bloquant <u>tous</u> les participants)",
-    'zh': "👮🏽<b>点击</b>✅/🔘<b>切换</b><u>加入</u>群组时的用户<i>验证</i>类型\n\n👉🏼 要设置<b>要按下的按钮</b>的名称，运行命令： <code>/button {0}</code>\n\n👉🏼<b>查看频道订阅情况</b><i>，将@{1}-bot 添加</i>到频道，执行命令： <code>/channel {2}</code>\n\n👉🏼 为<i>防止群内攻击</i>，开启<b>防突袭</b>模式（阻止<u>所有</u>加入者）",
-    'ar': "👮🏽 <b>انقر</b> فوق ✅ / 🔘 <b>لتبديل</b> نوع <i>التحقق</i> من المستخدم عند <u>الانضمام إلى</u> مجموعة\n\n👉🏼 لتعيين اسم <b>الزر المراد الضغط عليه</b> ، قم بتشغيل الأمر: <code>/button {0}</code>\n\n👉🏼 للتحقق <b>من الاشتراك</b> في القناة <i>، أضف</i> @ {1} -bot إلى القناة ونفذ الأمر: <code>/channel {2}</code>\n\n👉🏼 <i>للحماية من هجوم</i> على المجموعة ، شغّل وضع <b>anti-raid</b> (حظر <u>جميع</u> النجارين)",
+    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> в группу\n\n👉🏼 Для установки имени <b>нажимаемой кнопки</b>, выполни команду: /button {0}\n\n👉🏼 Для <b>проверки подписки</b> на канал <i>добавь</i> @{1}-бота в канал и выполни команду: /channel {2}\n\n👉🏼 Для <i>защиты от атаки</i> на группу включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
+    'en': "👮🏽 <b>Click</b> on ✅/🔘 to <b>switch</b> the type of user <i>verification</i> when <u>joining</u> a group\n\n👉🏼 To set the name <b>of the button to be pressed</b> , run the command: /button {0}\n\n👉🏼 To <b>check the subscription</b> to the channel <i>, add</i> @ {1}-bot into the channel and execute the command: /channel {2}\n\n👉🏼 To <i>protect against an attack</i> on the group, turn on the <b>anti-raid</b> mode (blocking <u>all</u> joiners)",
+    'es': "👮🏽 <b>Haz clic</b> en ✅/🔘 para <b>cambiar</b> el tipo de <i>verificación</i> de usuario al <u>unirte a</u> un grupo\n\n👉🏼 Para establecer el nombre <b>del botón que se presionará</b> , ejecuta el comando: /button {0}\n\n👉🏼 Para <b>verificar la suscripción</b> al canal <i>, agregue</i> @ {1}-bot al canal y ejecute el comando: /channel {2}\n\n👉🏼 Para <i>protegerse contra un ataque</i> al grupo, active el modo <b>anti-raid</b> (bloqueando <u>a todos</u> los carpinteros)",
+    'fr': "👮🏽 <b>Cliquez</b> sur ✅/🔘 pour <b>changer</b> le type de <i>vérification</i> de l&#x27;utilisateur lors <u>de l&#x27;adhésion à</u> un groupe\n\n👉🏼 Pour définir le nom <b>du bouton à appuyer</b> , exécutez la commande : /button {0}\n\n👉🏼 Pour <b>vérifier l&#x27;abonnement</b> au canal <i>, ajoutez</i> @{1}-bot dans le canal et exécutez la commande : /channel {2}\n\n👉🏼 Pour <i>vous protéger contre une attaque</i> sur le groupe, activez le mode <b>anti-raid</b> (bloquant <u>tous</u> les participants)",
+    'zh': "👮🏽<b>点击</b>✅/🔘<b>切换</b><u>加入</u>群组时的用户<i>验证</i>类型\n\n👉🏼 要设置<b>要按下的按钮</b>的名称，运行命令： /button {0}\n\n👉🏼<b>查看频道订阅情况</b><i>，将@{1}-bot 添加</i>到频道，执行命令： /channel {2}\n\n👉🏼 为<i>防止群内攻击</i>，开启<b>防突袭</b>模式（阻止<u>所有</u>加入者）",
+    'ar': "👮🏽 <b>انقر</b> فوق ✅ / 🔘 <b>لتبديل</b> نوع <i>التحقق</i> من المستخدم عند <u>الانضمام إلى</u> مجموعة\n\n👉🏼 لتعيين اسم <b>الزر المراد الضغط عليه</b> ، قم بتشغيل الأمر: /button {0}\n\n👉🏼 للتحقق <b>من الاشتراك</b> في القناة <i>، أضف</i> @ {1} -bot إلى القناة ونفذ الأمر: /channel {2}\n\n👉🏼 <i>للحماية من هجوم</i> على المجموعة ، شغّل وضع <b>anti-raid</b> (حظر <u>جميع</u> النجارين)",
 }
 l_ccheck_add = {
     'ru': "\n\nВ настройках [Администраторы] вкл для {0}-бота:\n[✅ Удаление сообщ]\n[✅ Блокировка польз]\n[✅ Добавление участ]\n\n🕚Подожди 1min",
     'en': "\n\nIn [Administrators] settings, on for {0}-bot:\n[✅ Deleting messages]\n[✅ Blocking users]\n[✅ Adding members]\n\n🕚Wait 1min",
     'es': "\n\nEn la configuración de [Administradores], activado para {0}-bot:\n[✅ Eliminación de mensajes]\n[✅ Bloqueo de usuarios]\n[✅ Adición de miembros]\n\n🕚Espera 1 minuto",
     'fr': "\n\nDans les paramètres [Administrateurs], activé pour {0}-bot :\n[✅ Suppression de messages]\n[✅ Blocage d'utilisateurs]\n[✅ Ajout de membres]\n\n🕚Attendez 1 min",
     'zh': "\n\n在 [管理员] 设置中，为 {0}-bot 打开：\n[✅ 删除消息]\n[✅ 阻止用户]\n[✅ 添加成员]\n\n🕚 等待 1 分钟",
@@ -4981,20 +4989,20 @@
     'en': "Your greeting",
     'es': "Tu saludo",
     'fr': "Votre message d'accueil",
     'zh': "你的问候",
     'ar': "تحياتك",
 }
 l_chello_text = {
-    'ru': "👋🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> приветствие, а также его ⚙️Настроить\n\n👉🏼 Например, <code>{0}</code>{1}",
-    'en': "👋🏽 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> the greeting, as well as its ⚙️Customize\n\n👉🏼 For example, <code>{0}</code> {1}",
-    'es': "👋🏽 <b>Haz clic</b> en ✅/☑️ para <b>activar o desactivar</b> el saludo, así como su ⚙️Personalizar\n\n👉🏼 Por ejemplo, <code>{0}</code> {1}",
-    'fr': "👋🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> le message d&#x27;accueil, ainsi que sa ⚙️Personnaliser\n\n👉🏼 Par exemple, <code>{0}</code> {1}",
-    'zh': "👋🏽<b>点击</b>✅/☑️<b>打开/关闭</b>问候语，以及它的 ⚙️自定义\n\n👉🏼 例如， <code>{0}</code> {1}",
-    'ar': "👋🏽 <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> الترحيب ، بالإضافة إلى تخصيص\n\n👉🏼 على سبيل المثال ، <code>{0}</code> {1}",
+    'ru': "👋🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> приветствие, а также его ⚙️Настроить\n\n👉🏼 Например, {0}{1}",
+    'en': "👋🏽 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> the greeting, as well as its ⚙️Customize\n\n👉🏼 For example, {0} {1}",
+    'es': "👋🏽 <b>Haz clic</b> en ✅/☑️ para <b>activar o desactivar</b> el saludo, así como su ⚙️Personalizar\n\n👉🏼 Por ejemplo, {0} {1}",
+    'fr': "👋🏽 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> le message d&#x27;accueil, ainsi que sa ⚙️Personnaliser\n\n👉🏼 Par exemple, {0} {1}",
+    'zh': "👋🏽<b>点击</b>✅/☑️<b>打开/关闭</b>问候语，以及它的 ⚙️自定义\n\n👉🏼 例如， {0} {1}",
+    'ar': "👋🏽 <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> الترحيب ، بالإضافة إلى تخصيص\n\n👉🏼 على سبيل المثال ، {0} {1}",
 }
 l_btn_on = {
     'ru': "✅☑Вкл",
     'en': "✅☑Incl",
     'es': "✅☑Incluye",
     'fr': "✅☑Inclus",
     'zh': "✅☑包括",
@@ -5013,20 +5021,20 @@
     'en': "⚙️Customize",
     'es': "⚙️Personalizar",
     'fr': "⚙️Personnaliser",
     'zh': "⚙️自定义",
     'ar': "⚙️ تخصيص",
 }
 l_chellochange_handler = {
-    'ru': "👋🏽 Отправь мне <b>текст</b>/<b>медиа</b> контент с текстом: фото/гиф/видео/аудио/документ или запиши голосовое/видео-заметку в кружке\n\n👉🏼 Например, <code>{0}</code>",
-    'en': "👋🏽 Send me <b>text</b> / <b>media</b> content with text: photo / gif / video / audio / document or write a voice / video note in a circle\n\n👉🏼 For example, <code>{0}</code>",
-    'es': "👋🏽 Envíame <b>texto</b> /contenido <b>multimedia</b> con texto: foto/gif/video/audio/documento o escribe una nota de voz/video en un círculo\n\n👉🏼 Por ejemplo, <code>{0}</code>",
-    'fr': "👋🏽 Envoyez-moi <b>du texte</b> /du contenu <b>multimédia</b> avec du texte : photo/gif/vidéo/audio/document ou écrivez une note vocale/vidéo dans un cercle\n\n👉🏼 Par exemple, <code>{0}</code>",
-    'zh': "👋🏽 向我发送<b>文字</b>/<b>媒体</b>内容并附上文字：照片/gif/视频/音频/文档或将语音/视频笔记写成一个圆圈\n\n👉🏼 例如， <code>{0}</code>",
-    'ar': "👋🏽 أرسل لي محتوى <b>نصيًا</b> / <b>وسائط</b> مع نص: صورة / gif / فيديو / صوت / مستند أو اكتب ملاحظة صوتية / فيديو في دائرة\n\n👉🏼 على سبيل المثال ، <code>{0}</code>",
+    'ru': "👋🏽 Отправь мне <b>текст</b>/<b>медиа</b> контент с текстом: фото/гиф/видео/аудио/документ или запиши голосовое/видео-заметку в кружке\n\n👉🏼 Например, {0}",
+    'en': "👋🏽 Send me <b>text</b> / <b>media</b> content with text: photo / gif / video / audio / document or write a voice / video note in a circle\n\n👉🏼 For example, {0}",
+    'es': "👋🏽 Envíame <b>texto</b> /contenido <b>multimedia</b> con texto: foto/gif/video/audio/documento o escribe una nota de voz/video en un círculo\n\n👉🏼 Por ejemplo, {0}",
+    'fr': "👋🏽 Envoyez-moi <b>du texte</b> /du contenu <b>multimédia</b> avec du texte : photo/gif/vidéo/audio/document ou écrivez une note vocale/vidéo dans un cercle\n\n👉🏼 Par exemple, {0}",
+    'zh': "👋🏽 向我发送<b>文字</b>/<b>媒体</b>内容并附上文字：照片/gif/视频/音频/文档或将语音/视频笔记写成一个圆圈\n\n👉🏼 例如， {0}",
+    'ar': "👋🏽 أرسل لي محتوى <b>نصيًا</b> / <b>وسائط</b> مع نص: صورة / gif / فيديو / صوت / مستند أو اكتب ملاحظة صوتية / فيديو في دائرة\n\n👉🏼 على سبيل المثال ، {0}",
 }
 l_fsm_hello_finish = {
     'ru': "👋🏽 Приветствие записано!\n\nОпцию можно включить в настройках [👋🏽Авто-приветствие], нажав [✅☑Вкл]",
     'en': "👋🏽 Greeting recorded!\n\nThe option can be enabled in the settings [👋🏽Auto-greeting] by pressing [✅☑On]",
     'es': "👋🏽 ¡Saludo grabado!\n\nLa opción se puede habilitar en la configuración [👋🏽 Saludo automático] presionando [✅☑On]",
     'fr': "👋🏽 Message d'accueil enregistré !\n\nL'option peut être activée dans les paramètres [👋🏽Salutation automatique] en appuyant sur [✅☑On]",
     'zh': "👋🏽问候语已录制！\n\n可以在设置[👋🏽自动问候语]中按[✅☑开启]启用该选项",
@@ -5083,19 +5091,19 @@
     'es': "{0} fuente",
     'fr': "{0} sources",
     'zh': "{0} 个来源",
     'ar': "{0} المصدر",
 }
 l_cinvitechange_handler = {
     'ru': "🚶🏽 Пришли мне <b>ссылку</b> на группу, откуда будем брать подписчиков\n\n👉🏼 Например, <code>https://t.me/likeconcentrat</code> - <b>Жми</b> на ссылку, чтобы скопировать",
-    'en': "🚶🏽 Send me <b>a link</b> to the group from where we will take subscribers\n\n👉🏼 For example, <code>https://t.me/likeconcentrat</code> - <b>Click</b> on the link to copy",
-    'es': "🚶🏽 Envíame <b>un enlace</b> al grupo desde donde tomaremos suscriptores\n\n👉🏼 Por ejemplo, <code>https://t.me/likeconcentrat</code> - <b>Haz clic</b> en el enlace para copiar",
-    'fr': "🚶🏽 Envoyez-moi <b>un lien</b> vers le groupe d&#x27;où nous prendrons des abonnés\n\n👉🏼 Par exemple, <code>https://t.me/likeconcentrat</code> - <b>Cliquez</b> sur le lien pour copier",
-    'zh': "🚶🏽 向我发送指向我们将从中接收订阅者的群组<b>的链接</b>\n\n👉🏼 例如， <code>https://t.me/likeconcentrat</code> -<b>单击</b>链接进行复制",
-    'ar': "🚶🏽 أرسل لي <b>رابطًا</b> للمجموعة التي سنأخذ منها المشتركين\n\n👉🏼 على سبيل المثال ، <code>https://t.me/likeconcentrat</code> - <b>انقر</b> فوق الارتباط للنسخ",
+    'en': "🚶🏽 Send me <b>a link</b> to the group from where we will take subscribers\n\n👉🏼 For example, https://t.me/likeconcentrat - <b>Click</b> on the link to copy",
+    'es': "🚶🏽 Envíame <b>un enlace</b> al grupo desde donde tomaremos suscriptores\n\n👉🏼 Por ejemplo, https://t.me/likeconcentrat - <b>Haz clic</b> en el enlace para copiar",
+    'fr': "🚶🏽 Envoyez-moi <b>un lien</b> vers le groupe d&#x27;où nous prendrons des abonnés\n\n👉🏼 Par exemple, https://t.me/likeconcentrat - <b>Cliquez</b> sur le lien pour copier",
+    'zh': "🚶🏽 向我发送指向我们将从中接收订阅者的群组<b>的链接</b>\n\n👉🏼 例如， https://t.me/likeconcentrat -<b>单击</b>链接进行复制",
+    'ar': "🚶🏽 أرسل لي <b>رابطًا</b> للمجموعة التي سنأخذ منها المشتركين\n\n👉🏼 على سبيل المثال ، https://t.me/likeconcentrat - <b>انقر</b> فوق الارتباط للنسخ",
 }
 l_correct_link = {
     'ru': "👩🏽‍💻 <b>Вставь</b> корректные данные или повтори операцию",
     'en': "👩🏽‍💻 <b>Insert</b> correct data or try again",
     'es': "👩🏽‍💻 <b>Inserta</b> los datos correctos o vuelve a intentarlo",
     'fr': "👩🏽‍💻 <b>Insérez</b> les données correctes ou réessayez",
     'zh': "👩🏽‍💻<b>插入</b>正确的数据或重试",
@@ -5607,20 +5615,20 @@
     'en': "👮🏽 In the [Permissions] settings, enable the option:\n\n[✅ Send surveys]\n\n🕚Wait 1min",
     'es': "👮🏽 En la configuración de [Permisos], habilita la opción:\n\n[✅ Enviar encuestas]\n\n🕚Espera 1min",
     'fr': "👮🏽 Dans les paramètres [Autorisations], activez l'option :\n\n[✅ Envoyer des sondages]\n\n🕚Attendez 1min",
     'zh': "👮🏽 在[权限]设置中，启用选项：\n\n[✅发送调查]\n\n🕚等待1分钟",
     'ar': "👮🏽 في إعدادات [الأذونات] ، قم بتمكين الخيار:\n\n[✅ إرسال استطلاعات الرأي]\n\n🕚 انتظر دقيقة واحدة",
 }
 l_cstickerconfig_text = {
-    'ru': "🦊 <b>Исключения</b> для стикерпаков в <code>{0}</code>-файле:\n\n+ Разрешенные: <u>{1}</u>\n- Запрещенные: <u>{2}</u>\n\n[✅ Разрешить] пропускает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [☑️☐Выкл sticker]\n\n[🚫 Запретить] запрещает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [✅☑Вкл sticker]",
-    'en': "🦊 <b>Exclusions</b> for sticker packs in <code>{0}</code> -file:\n\n+ Allowed: <u>{1}</u>\n- Forbidden: <u>{2}</u>\n\n[✅ Allow] skips specified sticker packs <i>as an exception</i> when [☑️☐Off] is selected sticker]\n\n[🚫 Disable] disables the specified sticker packs <i>as an exception</i> when [✅☑Enable sticker] is selected",
-    'es': "🦊 <b>Exclusiones</b> para paquetes de pegatinas en <code>{0}</code> -archivo:\n\n+ Permitido: <u>{1}</u>\n- Prohibido: <u>{2}</u>\n\n[✅ Permitir] omite paquetes de pegatinas especificados <i>como una excepción</i> cuando [☑️☐Desactivado] es la etiqueta seleccionada]\n\n[🚫 Deshabilitar] deshabilita los paquetes de etiquetas especificados <i>como una excepción</i> cuando se selecciona [✅☑Habilitar etiqueta]",
-    'fr': "🦊 <b>Exclusions</b> pour les packs d&#x27;autocollants dans <code>{0}</code> -file :\n\n+ Autorisé : <u>{1}</u>\n- Interdit : <u>{2}</u>\n\n[✅ Autoriser] ignore les packs d&#x27;autocollants spécifiés <i>comme exception</i> lorsque [☑️☐Off] est l&#x27;autocollant sélectionné]\n\n[🚫 Désactiver] désactive les packs d&#x27;autocollants spécifiés <i>comme exception</i> lorsque [✅☑Activer l'autocollant] est sélectionné",
-    'zh': "🦊 <code>{0}</code>中贴纸包的<b>排除</b>：\n\n+ 允许： <u>{1}</u>\n- 禁止： <u>{2}</u>\n\n[✅ 允许] 跳过指定的贴纸包<i>作为例外</i>[☑️☐关闭]被选中的贴纸]\n\n[🚫禁用]在选择[✅☑启用贴纸]时<i>作为例外</i>禁用指定的贴纸包",
-    'ar': "🦊 <b>استثناءات</b> حزم الملصقات في <code>{0}</code> -الملف:\n\n+ المسموح بها: <u>{1}</u>\n- ممنوع: <u>{2}</u>\n\n[✅ السماح] بتخطي حزم الملصقات المحددة <i>كاستثناء</i> عند [☑️☐ إيقاف] هو ملصق محدد]\n\n[تعطيل] يعطل حزم الملصقات المحددة <i>كاستثناء</i> عند تحديد [✅☑ تمكين الملصق]",
+    'ru': "🦊 <b>Исключения</b> для стикерпаков в {0}-файле:\n\n+ Разрешенные: <u>{1}</u>\n- Запрещенные: <u>{2}</u>\n\n[✅ Разрешить] пропускает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [☑️☐Выкл sticker]\n\n[🚫 Запретить] запрещает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [✅☑Вкл sticker]",
+    'en': "🦊 <b>Exclusions</b> for sticker packs in {0} -file:\n\n+ Allowed: <u>{1}</u>\n- Forbidden: <u>{2}</u>\n\n[✅ Allow] skips specified sticker packs <i>as an exception</i> when [☑️☐Off] is selected sticker]\n\n[🚫 Disable] disables the specified sticker packs <i>as an exception</i> when [✅☑Enable sticker] is selected",
+    'es': "🦊 <b>Exclusiones</b> para paquetes de pegatinas en {0} -archivo:\n\n+ Permitido: <u>{1}</u>\n- Prohibido: <u>{2}</u>\n\n[✅ Permitir] omite paquetes de pegatinas especificados <i>como una excepción</i> cuando [☑️☐Desactivado] es la etiqueta seleccionada]\n\n[🚫 Deshabilitar] deshabilita los paquetes de etiquetas especificados <i>como una excepción</i> cuando se selecciona [✅☑Habilitar etiqueta]",
+    'fr': "🦊 <b>Exclusions</b> pour les packs d&#x27;autocollants dans {0} -file :\n\n+ Autorisé : <u>{1}</u>\n- Interdit : <u>{2}</u>\n\n[✅ Autoriser] ignore les packs d&#x27;autocollants spécifiés <i>comme exception</i> lorsque [☑️☐Off] est l&#x27;autocollant sélectionné]\n\n[🚫 Désactiver] désactive les packs d&#x27;autocollants spécifiés <i>comme exception</i> lorsque [✅☑Activer l'autocollant] est sélectionné",
+    'zh': "🦊 {0}中贴纸包的<b>排除</b>：\n\n+ 允许： <u>{1}</u>\n- 禁止： <u>{2}</u>\n\n[✅ 允许] 跳过指定的贴纸包<i>作为例外</i>[☑️☐关闭]被选中的贴纸]\n\n[🚫禁用]在选择[✅☑启用贴纸]时<i>作为例外</i>禁用指定的贴纸包",
+    'ar': "🦊 <b>استثناءات</b> حزم الملصقات في {0} -الملف:\n\n+ المسموح بها: <u>{1}</u>\n- ممنوع: <u>{2}</u>\n\n[✅ السماح] بتخطي حزم الملصقات المحددة <i>كاستثناء</i> عند [☑️☐ إيقاف] هو ملصق محدد]\n\n[تعطيل] يعطل حزم الملصقات المحددة <i>كاستثناء</i> عند تحديد [✅☑ تمكين الملصق]",
 }
 l_cstickerpack_1 = {
     'ru': "✅ Разрешить",
     'en': "✅ Allow",
     'es': "✅ Permitir",
     'fr': "✅ Autoriser",
     'zh': "✅ 允许",
@@ -5647,52 +5655,52 @@
     'en': "🚫 Delete",
     'es': "🚫 Eliminar",
     'fr': "🚫 Supprimer",
     'zh': "🚫 删除",
     'ar': "🚫 حذف",
 }
 l_GROUPP_CSTICKER1_NUM1 = {
-    'ru': "🦊 Текущее количество <b>разрешенных</b> стикерпаков в <code>{0}</code>-файле: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> разрешенные стикерпаки",
-    'en': "🦊 Current number of <b>allowed</b> sticker packs in <code>{0}</code> -file: <u>{1}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> allowed sticker packs",
-    'es': "🦊 Número actual de paquetes de calcomanías <b>permitidos</b> en <code>{0}</code> -archivo: <u>{1}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> paquetes de calcomanías permitidos",
-    'fr': "🦊 Nombre actuel de packs d'autocollants <b>autorisés</b> dans le fichier <code>{0}</code> : <u>{1}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des packs d'autocollants autorisés",
-    'zh': "🦊 <code>{0}</code>文件中<b>允许的</b>贴纸包的当前数量： <u>{1}</u>\n\n<b>单击</b>✅/🚫<b>添加/删除</b>允许的贴纸包",
-    'ar': "🦊 العدد الحالي لحزم الملصقات <b>المسموح بها</b> في <code>{0}</code> - الملف: <u>{1}</u>\n\n<b>انقر</b> على ✅ / 🚫 لإضافة <b>/ إزالة</b> حزم الملصقات المسموح بها",
+    'ru': "🦊 Текущее количество <b>разрешенных</b> стикерпаков в {0}-файле: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> разрешенные стикерпаки",
+    'en': "🦊 Current number of <b>allowed</b> sticker packs in {0} -file: <u>{1}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> allowed sticker packs",
+    'es': "🦊 Número actual de paquetes de calcomanías <b>permitidos</b> en {0} -archivo: <u>{1}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> paquetes de calcomanías permitidos",
+    'fr': "🦊 Nombre actuel de packs d'autocollants <b>autorisés</b> dans le fichier {0} : <u>{1}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des packs d'autocollants autorisés",
+    'zh': "🦊 {0}文件中<b>允许的</b>贴纸包的当前数量： <u>{1}</u>\n\n<b>单击</b>✅/🚫<b>添加/删除</b>允许的贴纸包",
+    'ar': "🦊 العدد الحالي لحزم الملصقات <b>المسموح بها</b> في {0} - الملف: <u>{1}</u>\n\n<b>انقر</b> على ✅ / 🚫 لإضافة <b>/ إزالة</b> حزم الملصقات المسموح بها",
 }
 l_GROUPP_CSTICKER1_NUM0 = {
     'ru': "🦊 Текущее количество <b>разрешенных</b> стикерпаков: <u>{0}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> разрешенные стикерпаки",
     'en': "🦊 Current number of <b>allowed</b> sticker packs: <u>{0}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> allowed sticker packs",
     'es': "🦊 Número actual de paquetes de pegatinas <b>permitidos</b> : <u>{0}</u>\n\n<b>Haz clic</b> en ✅/🚫 para <b>agregar o quitar</b> paquetes de pegatinas permitidos",
     'fr': "🦊 Nombre actuel de packs d'autocollants <b>autorisés</b> : <u>{0}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des packs d'autocollants autorisés",
     'zh': "🦊 当前<b>允许的</b>贴纸包数量： <u>{0}</u>\n\n<b>点击</b>✅/🚫<b>添加/删除</b>允许的贴纸包",
     'ar': "🦊 العدد الحالي لحزم الملصقات <b>المسموح بها</b> : <u>{0}</u>\n\n<b>انقر</b> فوق ✅ / 🚫 <b>لإضافة / إزالة</b> حزم الملصقات المسموح بها",
 }
 l_GROUPP_CSTICKER0_NUM1 = {
-    'ru': "🦊 Текущее количество <b>запрещенных</b> стикерпаков в <code>{0}</code>-файле: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> запрещенные стикерпаки",
-    'en': "🦊 Current number of <b>banned</b> sticker packs in <code>{0}</code> -file: <u>{1}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> banned sticker packs",
-    'es': "🦊 Número actual de paquetes de pegatinas <b>prohibidos</b> en <code>{0}</code> -archivo: <u>{1}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> paquetes de pegatinas prohibidos",
-    'fr': "🦊 Nombre actuel de packs d'autocollants <b>interdits</b> dans le fichier <code>{0}</code> : <u>{1}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des packs d'autocollants interdits",
-    'zh': "🦊 <code>{0}</code>文件中的当前<b>禁止</b>贴纸包数量： <u>{1}</u>\n\n<b>点击</b>✅/🚫<b>添加/删除</b>禁止贴纸包",
-    'ar': "🦊 العدد الحالي لحزم الملصقات <b>المحظورة</b> في <code>{0}</code> - الملف: <u>{1}</u>\n\n<b>انقر</b> على ✅ / 🚫 لإضافة <b>/ إزالة</b> حزم الملصقات المحظورة",
+    'ru': "🦊 Текущее количество <b>запрещенных</b> стикерпаков в {0}-файле: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> запрещенные стикерпаки",
+    'en': "🦊 Current number of <b>banned</b> sticker packs in {0} -file: <u>{1}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> banned sticker packs",
+    'es': "🦊 Número actual de paquetes de pegatinas <b>prohibidos</b> en {0} -archivo: <u>{1}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> paquetes de pegatinas prohibidos",
+    'fr': "🦊 Nombre actuel de packs d'autocollants <b>interdits</b> dans le fichier {0} : <u>{1}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des packs d'autocollants interdits",
+    'zh': "🦊 {0}文件中的当前<b>禁止</b>贴纸包数量： <u>{1}</u>\n\n<b>点击</b>✅/🚫<b>添加/删除</b>禁止贴纸包",
+    'ar': "🦊 العدد الحالي لحزم الملصقات <b>المحظورة</b> في {0} - الملف: <u>{1}</u>\n\n<b>انقر</b> على ✅ / 🚫 لإضافة <b>/ إزالة</b> حزم الملصقات المحظورة",
 }
 l_GROUPP_CSTICKER0_NUM0 = {
     'ru': "🦊 Текущее количество <b>запрещенных</b> стикерпаков: <u>{0}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> запрещенные стикерпаки",
     'en': "🦊 Current number of <b>banned</b> sticker packs: <u>{0}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> banned sticker packs",
     'es': "🦊 Número actual de paquetes de pegatinas <b>prohibidos</b> : <u>{0}</u>\n\n<b>Haz clic</b> en ✅/🚫 para <b>agregar o quitar</b> paquetes de pegatinas prohibidos",
     'fr': "🦊 Nombre actuel de packs d'autocollants <b>interdits</b> : <u>{0}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des packs d'autocollants interdits",
     'zh': "🦊 当前<b>禁止的</b>贴纸包数量： <u>{0}</u>\n\n<b>点击</b>✅/🚫<b>添加/删除</b>禁止的贴纸包",
     'ar': "🦊 العدد الحالي لحزم الملصقات <b>المحظورة</b> : <u>{0}</u>\n\n<b>انقر</b> فوق ✅ / 🚫 <b>لإضافة / إزالة</b> حزم الملصقات المحظورة",
 }
 l_cstickeroperation_add = {
-    'ru': "\n\n👉🏼 Например, https://t.me/addstickers/HotCherry или <code>HotCherry</code>",
-    'en': "\n\n👉🏼 For example, https://t.me/addstickers/HotCherry or <code>HotCherry</code>",
-    'es': "\n\n👉🏼 Por ejemplo, https://t.me/addstickers/HotCherry o <code>HotCherry</code>",
-    'fr': "\n\n👉🏼 Par exemple, https://t.me/addstickers/HotCherry ou <code>HotCherry</code>",
-    'zh': "\n\n👉🏼 例如， https://t.me/addstickers/HotCherry或<code>HotCherry</code>",
-    'ar': "\n\n👉🏼 على سبيل المثال ، https://t.me/addstickers/HotCherry أو <code>HotCherry</code>",
+    'ru': "\n\n👉🏼 Например, https://t.me/addstickers/HotCherry или HotCherry",
+    'en': "\n\n👉🏼 For example, https://t.me/addstickers/HotCherry or HotCherry",
+    'es': "\n\n👉🏼 Por ejemplo, https://t.me/addstickers/HotCherry o HotCherry",
+    'fr': "\n\n👉🏼 Par exemple, https://t.me/addstickers/HotCherry ou HotCherry",
+    'zh': "\n\n👉🏼 例如， https://t.me/addstickers/HotCherry或HotCherry",
+    'ar': "\n\n👉🏼 على سبيل المثال ، https://t.me/addstickers/HotCherry أو HotCherry",
 }
 l_cstickeroperation_isadd = {
     'ru': "✅ Пришли ссылку или имя <b>стикерпака</b>, чтобы <b>добавить</b> его в список разрешенных{0}",
     'en': "✅ Sent a link or <b>sticker pack</b> name to <b>add</b> it to the allowed list{0}",
     'es': "✅ Envió un enlace o nombre <b>de paquete de calcomanías</b> para <b>agregarlo</b> a la lista permitida{0}",
     'fr': "✅ Envoyé un lien ou un nom <b>de pack d&#x27;autocollants</b> pour l&#x27; <b>ajouter</b> à la liste autorisée{0}",
     'zh': "✅ 发送链接或<b>贴纸包</b>名称以将其<b>添加</b>到允许列表{0}",
@@ -5771,20 +5779,20 @@
     'en': "🚀 Use",
     'es': "🚀 Uso",
     'fr': "🚀 Utiliser",
     'zh': "🚀 使用",
     'ar': "🚀 استخدم",
 }
 l_cstartoperation_caption = {
-    'ru': "🚀 <b>Текущее</b> количество <i>старт-слов</i> для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> старт-слова",
-    'en': "🚀 <b>Current</b> number of <i>start words</i> for post #{0} in <code>{1}</code> file: <u>{2}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> start words",
-    'es': "🚀 Número <b>actual</b> de <i>palabras de inicio</i> para la publicación n.º {0} en el archivo <code>{1}</code> : <u>{2}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> palabras de inicio",
-    'fr': "🚀 Nombre <b>actuel</b> de <i>mots de départ</i> pour le message #{0} dans le fichier <code>{1}</code> : <u>{2}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots de départ",
-    'zh': "🚀 <code>{1}</code>文件中帖子 #{0} 的<b>当前</b><i>起始词</i>数： <u>{2}</u>\n\n<b>单击</b>✅/🚫<b>添加/删除</b>起始词",
-    'ar': "🚀 العدد <b>الحالي</b> <i>لكلمات البداية</i> للنشر # {0} في ملف <code>{1}</code> : <u>{2}</u>\n\n<b>انقر</b> على ✅ / 🚫 <b>لإضافة / إزالة</b> كلمات البداية",
+    'ru': "🚀 <b>Текущее</b> количество <i>старт-слов</i> для поста #{0} в {1}-файле: <u>{2}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> старт-слова",
+    'en': "🚀 <b>Current</b> number of <i>start words</i> for post #{0} in {1} file: <u>{2}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> start words",
+    'es': "🚀 Número <b>actual</b> de <i>palabras de inicio</i> para la publicación n.º {0} en el archivo {1} : <u>{2}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> palabras de inicio",
+    'fr': "🚀 Nombre <b>actuel</b> de <i>mots de départ</i> pour le message #{0} dans le fichier {1} : <u>{2}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots de départ",
+    'zh': "🚀 {1}文件中帖子 #{0} 的<b>当前</b><i>起始词</i>数： <u>{2}</u>\n\n<b>单击</b>✅/🚫<b>添加/删除</b>起始词",
+    'ar': "🚀 العدد <b>الحالي</b> <i>لكلمات البداية</i> للنشر # {0} في ملف {1} : <u>{2}</u>\n\n<b>انقر</b> على ✅ / 🚫 <b>لإضافة / إزالة</b> كلمات البداية",
 }
 l_cstartoperation_text = {
     'ru': "🚀 <b>Текущее</b> количество <i>старт-слов</i> для поста #{0}: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> старт-слова",
     'en': "🚀 <b>Current</b> number <i>of start words</i> for post #{0}: <u>{1}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> start words",
     'es': "🚀 Número <b>actual</b> <i>de palabras de inicio</i> para la publicación n.º {0}: <u>{1}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> palabras de inicio",
     'fr': "🚀 Nombre <b>actuel</b> <i>de mots de départ</i> pour le message #{0} : <u>{1}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots de départ",
     'zh': "🚀 帖子 #{0} 的<b>当前</b><i>起始词</i>数： <u>{1}</u>\n\n<b>单击</b>✅/🚫<b>添加/删除</b>起始词",
@@ -5811,20 +5819,20 @@
     'en': "🚫 <b>Enter</b> <u>start words</u> <b>separated by</b> spaces or separators to <i>remove</i> them from the database{0}",
     'es': "🚫 <b>Introduce</b> <u>palabras iniciales</u> <b>separadas por</b> espacios o separadores para <i>eliminarlas</i> de la base de datos{0}",
     'fr': "🚫 <b>Saisissez</b> <u>des mots de début</u> <b>séparés par</b> des espaces ou des séparateurs pour les <i>supprimer</i> de la base de données{0}",
     'zh': "🚫<b>输入以空格或分隔符分隔的</b><u>起始词</u>，以将其从数据库中<i>删除</i>{0}",
     'ar': "🚫 <b>أدخل</b> <u>كلمات البداية</u> <b>مفصولة</b> بمسافات أو فواصل <i>لإزالتها</i> من قاعدة البيانات {0}",
 }
 l_fsm_start_add_caption = {
-    'ru': "🚀 <b>Готово!</b> <b>Текущее</b> количество старт-слов для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>",
-    'en': "🚀 <b>Done!</b> <b>Current</b> number of start words for post #{0} in <code>{1}</code> -file: <u>{2}</u>",
-    'es': "🚀 <b>Listo!</b> Número <b>actual</b> de palabras iniciales para la publicación n.º {0} en <code>{1}</code> -archivo: <u>{2}</u>",
-    'fr': "🚀 <b>C&#x27;est fait !</b> Nombre <b>actuel</b> de mots de départ pour le message #{0} dans le fichier <code>{1}</code> : <u>{2}</u>",
-    'zh': "🚀<b>完成！</b> <code>{1}</code>文件中帖子#{0} 的<b>当前</b>起始词数： <u>{2}</u>",
-    'ar': "🚀 <b>انتهى!</b> العدد <b>الحالي</b> لكلمات البدء للمشاركة # {0} في الملف <code>{1}</code> : <u>{2}</u>",
+    'ru': "🚀 <b>Готово!</b> <b>Текущее</b> количество старт-слов для поста #{0} в {1}-файле: <u>{2}</u>",
+    'en': "🚀 <b>Done!</b> <b>Current</b> number of start words for post #{0} in {1} -file: <u>{2}</u>",
+    'es': "🚀 <b>Listo!</b> Número <b>actual</b> de palabras iniciales para la publicación n.º {0} en {1} -archivo: <u>{2}</u>",
+    'fr': "🚀 <b>C&#x27;est fait !</b> Nombre <b>actuel</b> de mots de départ pour le message #{0} dans le fichier {1} : <u>{2}</u>",
+    'zh': "🚀<b>完成！</b> {1}文件中帖子#{0} 的<b>当前</b>起始词数： <u>{2}</u>",
+    'ar': "🚀 <b>انتهى!</b> العدد <b>الحالي</b> لكلمات البدء للمشاركة # {0} في الملف {1} : <u>{2}</u>",
 }
 l_fsm_start_add_text = {
     'ru': "🚀 <b>Готово!</b> <b>Текущее</b> количество старт-слов для поста #{0}: <u>{1}</u>",
     'en': "🚀 <b>Done!</b> <b>Current</b> number of start words for post #{0}: <u>{1}</u>",
     'es': "🚀 <b>Listo!</b> Número <b>actual</b> de palabras iniciales para la publicación n.º {0}: <u>{1}</u>",
     'fr': "🚀 <b>C&#x27;est fait !</b> Nombre <b>actuel</b> de mots de départ pour le message #{0} : <u>{1}</u>",
     'zh': "🚀<b>完成！</b>帖子 #{0} 的<b>当前</b>起始词数： <u>{1}</u>",
@@ -5856,20 +5864,20 @@
     'en': "🔔 You must ⚙️Set up at least one stop word",
     'es': "🔔 Debes ⚙️Configurar al menos una palabra vacía",
     'fr': "🔔 Vous devez ⚙️Configurer au moins un mot vide",
     'zh': "🔔 你必须⚙️设置至少一个停用词",
     'ar': "🔔 يجب أن تقوم بإعداد كلمة توقف واحدة على الأقل",
 }
 l_cstopchange_caption = {
-    'ru': "🧾 Текущее количество стоп-слов в <code>{0}</code>-файле: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> стоп-слова",
-    'en': "🧾 Current number of stop words in <code>{0}</code> -file: <u>{1}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> stop words",
-    'es': "🧾 Número actual de palabras vacías en el archivo <code>{0}</code> : <u>{1}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> palabras vacías",
-    'fr': "🧾 Nombre actuel de mots vides dans le fichier <code>{0}</code> : <u>{1}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots vides",
-    'zh': "🧾 <code>{0}</code>文件中的当前停用词数： <u>{1}</u>\n\n<b>单击</b>✅/🚫<b>添加/删除</b>停用词",
-    'ar': "🧾 العدد الحالي لكلمات الإيقاف في <code>{0}</code> -ملف: <u>{1}</u>\n\n<b>انقر</b> على ✅ / 🚫 <b>لإضافة / إزالة</b> كلمات التوقف",
+    'ru': "🧾 Текущее количество стоп-слов в {0}-файле: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> стоп-слова",
+    'en': "🧾 Current number of stop words in {0} -file: <u>{1}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> stop words",
+    'es': "🧾 Número actual de palabras vacías en el archivo {0} : <u>{1}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o quitar</b> palabras vacías",
+    'fr': "🧾 Nombre actuel de mots vides dans le fichier {0} : <u>{1}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots vides",
+    'zh': "🧾 {0}文件中的当前停用词数： <u>{1}</u>\n\n<b>单击</b>✅/🚫<b>添加/删除</b>停用词",
+    'ar': "🧾 العدد الحالي لكلمات الإيقاف في {0} -ملف: <u>{1}</u>\n\n<b>انقر</b> على ✅ / 🚫 <b>لإضافة / إزالة</b> كلمات التوقف",
 }
 l_cstopchange_text = {
     'ru': "🧾 Текущее количество стоп-слов <u>{0}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> стоп-слова",
     'en': "🧾 Current number of stop words <u>{0}</u>\n\n<b>Click</b> on ✅/🚫 to <b>Add/Remove</b> stop words",
     'es': "🧾 Número actual de palabras vacías <u>{0}</u>\n\n<b>Haga clic</b> en ✅/🚫 para <b>agregar o</b> quitar palabras vacías",
     'fr': "🧾 Nombre actuel de mots vides <u>{0}</u>\n\n<b>Cliquez</b> sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots vides",
     'zh': "🧾 当前停用词数<u>{0}</u>\n\n<b>点击</b>✅/🚫<b>添加/删除</b>停用词",
@@ -5896,40 +5904,40 @@
     'en': "🚫 <b>Enter</b> <u>stop words</u> <b>separated by</b> spaces or separators to <i>remove</i> them from the database{0}",
     'es': "🚫 <b>Introduce</b> <u>palabras vacías</u> <b>separadas por</b> espacios o separadores para <i>eliminarlas</i> de la base de datos{0}",
     'fr': "🚫 <b>Saisissez</b> <u>des mots vides</u> <b>séparés par</b> des espaces ou des séparateurs pour les <i>supprimer</i> de la base de données{0}",
     'zh': "🚫<b>输入以空格或分隔符分隔的</b><u>停用词</u>以将其从数据库中<i>删除</i>{0}",
     'ar': "🚫 <b>أدخل</b> <u>كلمات التوقف</u> <b>مفصولة</b> بمسافات أو فواصل <i>لإزالتها</i> من قاعدة البيانات {0}",
 }
 l_fsm_stop_add_caption = {
-    'ru': "🧾 <b>Готово!</b> <b>Текущее</b> количество стоп-слов в <code>{0}</code>-файле: <u>{1}</u>",
-    'en': "🧾 <b>Done!</b> <b>Current</b> number of stop words in <code>{0}</code> -file: <u>{1}</u>",
-    'es': "🧾 <b>Listo!</b> Número <b>actual</b> de palabras vacías en <code>{0}</code> -archivo: <u>{1}</u>",
-    'fr': "🧾 <b>C&#x27;est fait !</b> Nombre <b>actuel</b> de mots vides dans le fichier <code>{0}</code> : <u>{1}</u>",
-    'zh': "🧾<b>完成！</b> <code>{0}</code>文件中的<b>当前</b>停用词数： <u>{1}</u>",
-    'ar': "🧾 <b>انتهى!</b> العدد <b>الحالي</b> لكلمات التوقف في ملف <code>{0}</code> : <u>{1}</u>",
+    'ru': "🧾 <b>Готово!</b> <b>Текущее</b> количество стоп-слов в {0}-файле: <u>{1}</u>",
+    'en': "🧾 <b>Done!</b> <b>Current</b> number of stop words in {0} -file: <u>{1}</u>",
+    'es': "🧾 <b>Listo!</b> Número <b>actual</b> de palabras vacías en {0} -archivo: <u>{1}</u>",
+    'fr': "🧾 <b>C&#x27;est fait !</b> Nombre <b>actuel</b> de mots vides dans le fichier {0} : <u>{1}</u>",
+    'zh': "🧾<b>完成！</b> {0}文件中的<b>当前</b>停用词数： <u>{1}</u>",
+    'ar': "🧾 <b>انتهى!</b> العدد <b>الحالي</b> لكلمات التوقف في ملف {0} : <u>{1}</u>",
 }
 l_fsm_stop_add_text = {
     'ru': "🧾 <b>Готово!</b> <b>Текущее</b> количество стоп-слов <u>{0}</u>",
     'en': "🧾 <b>Done!</b> <b>Current</b> number of stop words <u>{0}</u>",
     'es': "🧾 <b>Listo!</b> Número <b>actual</b> de palabras vacías <u>{0}</u>",
     'fr': "🧾 <b>C&#x27;est fait !</b> Nombre <b>actuel</b> de mots vides <u>{0}</u>",
     'zh': "🧾<b>完成！当前</b>停用词数<u>{0}</u>",
     'ar': "🧾 <b>انتهى!</b> العدد <b>الحالي</b> لكلمات التوقف <u>{0}</u>",
 }
 # endregion
 
 
 # region cflood_
 l_cflood_text = {
-    'ru': "💬 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>проверку</i> на частоту подряд написанных сообщ за один промежуток времени\n\n👉🏼 Например, задай количество сообщ подряд, которое будет считаться флудом командой: <code>/flood 5</code>\n\n👉🏼 Или используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
-    'en': "💬 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> <i>the check</i> for the frequency of consecutive messages written in one period of time\n\n👉🏼 For example, set the number of messages in a row that will be considered a flood with the command: <code>/flood 5</code>\n\n👉🏼 Or use <b>slow mode</b> in group settings for <u>1</u> message",
-    'es': "💬 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <i>la verificación</i> de la frecuencia de mensajes consecutivos escritos en un período de tiempo\n\n👉🏼 Por ejemplo, establece la cantidad de mensajes seguidos que se considerarán una inundación con el comando: <code>/flood 5</code>\n\n👉🏼 O usa <b>el modo lento</b> en la configuración del grupo para <u>1</u> mensaje",
-    'fr': "💬 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>la vérification</i> de la fréquence des messages consécutifs écrits dans une période de temps\n\n👉🏼 Par exemple, définissez le nombre de messages consécutifs qui seront considérés comme une inondation avec le commande : <code>/flood 5</code>\n\n👉🏼 Ou utilisez <b>le mode lent</b> dans les paramètres de groupe pour <u>1</u> message",
-    'zh': "💬<b>点击</b>✅/☑️<b>开启/关闭</b><i>检查</i>一段时间内连续写入消息的频率\n\n👉🏼 例如，设置连续消息的数量将被视为洪水命令： <code>/flood 5</code>\n\n👉🏼 或者在组设置中使用<b>慢速模式</b>发送<u>1 条</u>消息",
-    'ar': "💬 <b>انقر</b> فوق ✅ / ☑️ لتشغيل <b>/ إيقاف تشغيل</b> <i>التحقق</i> من تكرار الرسائل المتتالية المكتوبة في فترة زمنية واحدة\n\n👉🏼 على سبيل المثال ، قم بتعيين عدد الرسائل في الصف الذي سيتم اعتباره فيضانًا مع الأمر: <code>/flood 5</code>\n\n👉🏼 أو استخدم <b>الوضع البطيء</b> في إعدادات المجموعة لرسالة <u>واحدة</u>",
+    'ru': "💬 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>проверку</i> на частоту подряд написанных сообщ за один промежуток времени\n\n👉🏼 Например, задай количество сообщ подряд, которое будет считаться флудом командой: /flood 5\n\n👉🏼 Или используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
+    'en': "💬 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> <i>the check</i> for the frequency of consecutive messages written in one period of time\n\n👉🏼 For example, set the number of messages in a row that will be considered a flood with the command: /flood 5\n\n👉🏼 Or use <b>slow mode</b> in group settings for <u>1</u> message",
+    'es': "💬 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <i>la verificación</i> de la frecuencia de mensajes consecutivos escritos en un período de tiempo\n\n👉🏼 Por ejemplo, establece la cantidad de mensajes seguidos que se considerarán una inundación con el comando: /flood 5\n\n👉🏼 O usa <b>el modo lento</b> en la configuración del grupo para <u>1</u> mensaje",
+    'fr': "💬 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>la vérification</i> de la fréquence des messages consécutifs écrits dans une période de temps\n\n👉🏼 Par exemple, définissez le nombre de messages consécutifs qui seront considérés comme une inondation avec le commande : /flood 5\n\n👉🏼 Ou utilisez <b>le mode lent</b> dans les paramètres de groupe pour <u>1</u> message",
+    'zh': "💬<b>点击</b>✅/☑️<b>开启/关闭</b><i>检查</i>一段时间内连续写入消息的频率\n\n👉🏼 例如，设置连续消息的数量将被视为洪水命令： /flood 5\n\n👉🏼 或者在组设置中使用<b>慢速模式</b>发送<u>1 条</u>消息",
+    'ar': "💬 <b>انقر</b> فوق ✅ / ☑️ لتشغيل <b>/ إيقاف تشغيل</b> <i>التحقق</i> من تكرار الرسائل المتتالية المكتوبة في فترة زمنية واحدة\n\n👉🏼 على سبيل المثال ، قم بتعيين عدد الرسائل في الصف الذي سيتم اعتباره فيضانًا مع الأمر: /flood 5\n\n👉🏼 أو استخدم <b>الوضع البطيء</b> في إعدادات المجموعة لرسالة <u>واحدة</u>",
 }
 l_cflood_count_on = {
     'ru': "✅☑Вкл {0} сообщ",
     'en': "✅☑On {0} messages",
     'es': "✅☑En {0} mensajes",
     'fr': "✅☑Sur {0} messages",
     'zh': "✅☑关于 {0} 条消息",
@@ -5944,20 +5952,20 @@
     'ar': "☑️☐ إيقاف {0} الرسائل",
 }
 # endregion
 
 
 # region cuser_
 l_cuser_text = {
-    'ru': "👥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> первичную <i>задержку/свободный вход без входного контроля для premium-аккаунтов/разрешение на инвайт</i> пользователей/ботов в группу или разрешение на <i>редактирование</i> сообщений\n\n👉🏼 Например, <b>задержка</b> (<i>в мин</i>) для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) осуществляется командой: <code>/delay  {0}</code>",
-    'en': "👥 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> initial <i>delay/free entry without input control for premium accounts/permission to invite</i> users/bots to the group or permission to <i>edit</i> messages\n\n👉🏼 For example, <b>delay</b> ( <i>in min</i> ) for <u>new</u> users (before writing their <u>1st</u> message) is done with the command: <code>/delay {0}</code>",
-    'es': "👥 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <i>el retraso inicial/entrada gratuita sin control de entrada para cuentas premium/permiso para invitar</i> usuarios/bots al grupo o permiso para <i>editar</i> mensajes\n\n👉🏼 Por ejemplo, <b>retraso</b> ( <i>en minutos</i> ) para <u>nuevos</u> usuarios (antes de escribir su <u>primer</u> mensaje) se hace con el comando: <code>/delay {0}</code>",
-    'fr': "👥 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>le délai initial/entrée libre sans contrôle de saisie pour les comptes premium/autorisation d&#x27;inviter</i> des utilisateurs/bots dans le groupe ou autorisation de <i>modifier</i> des messages\n\n👉🏼 Par exemple, <b>délai</b> ( <i>en min</i> ) pour <u>les nouveaux</u> utilisateurs (avant d&#x27;écrire leur <u>1er</u> message) se fait avec la commande : <code>/delay {0}</code>",
-    'zh': "👥<b>点击</b>✅/☑️<b>启用/禁用</b>初始<i>延迟/免费进入高级帐户没有输入控制/允许邀请</i>用户/机器人加入组或允许<i>编辑</i>消息\n\n👉🏼 例如，<b>延迟</b>（<i>以分钟为单位</i>）对于<u>新</u>用户（在写他们的<u>第一条</u>消息之前）是用命令完成的： <code>/delay {0}</code>",
-    'ar': "👥 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>التأخير الأولي / الإدخال المجاني بدون التحكم في الإدخال للحسابات المتميزة / إذن لدعوة</i> المستخدمين / الروبوتات إلى المجموعة أو الإذن <i>لتحرير</i> الرسائل\n\n👉🏼 على سبيل المثال ، <b>تأخير</b> ( <i>بالدقائق</i> ) للمستخدمين <u>الجدد</u> (قبل كتابة رسالتهم <u>الأولى</u> ) يتم باستخدام الأمر: <code>/delay {0}</code>",
+    'ru': "👥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> первичную <i>задержку/свободный вход без входного контроля для premium-аккаунтов/разрешение на инвайт</i> пользователей/ботов в группу или разрешение на <i>редактирование</i> сообщений\n\n👉🏼 Например, <b>задержка</b> (<i>в мин</i>) для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) осуществляется командой: /delay  {0}",
+    'en': "👥 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> initial <i>delay/free entry without input control for premium accounts/permission to invite</i> users/bots to the group or permission to <i>edit</i> messages\n\n👉🏼 For example, <b>delay</b> ( <i>in min</i> ) for <u>new</u> users (before writing their <u>1st</u> message) is done with the command: /delay {0}",
+    'es': "👥 <b>Haz clic</b> en ✅/☑️ para <b>activar/desactivar</b> <i>el retraso inicial/entrada gratuita sin control de entrada para cuentas premium/permiso para invitar</i> usuarios/bots al grupo o permiso para <i>editar</i> mensajes\n\n👉🏼 Por ejemplo, <b>retraso</b> ( <i>en minutos</i> ) para <u>nuevos</u> usuarios (antes de escribir su <u>primer</u> mensaje) se hace con el comando: /delay {0}",
+    'fr': "👥 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>le délai initial/entrée libre sans contrôle de saisie pour les comptes premium/autorisation d&#x27;inviter</i> des utilisateurs/bots dans le groupe ou autorisation de <i>modifier</i> des messages\n\n👉🏼 Par exemple, <b>délai</b> ( <i>en min</i> ) pour <u>les nouveaux</u> utilisateurs (avant d&#x27;écrire leur <u>1er</u> message) se fait avec la commande : /delay {0}",
+    'zh': "👥<b>点击</b>✅/☑️<b>启用/禁用</b>初始<i>延迟/免费进入高级帐户没有输入控制/允许邀请</i>用户/机器人加入组或允许<i>编辑</i>消息\n\n👉🏼 例如，<b>延迟</b>（<i>以分钟为单位</i>）对于<u>新</u>用户（在写他们的<u>第一条</u>消息之前）是用命令完成的： /delay {0}",
+    'ar': "👥 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>التأخير الأولي / الإدخال المجاني بدون التحكم في الإدخال للحسابات المتميزة / إذن لدعوة</i> المستخدمين / الروبوتات إلى المجموعة أو الإذن <i>لتحرير</i> الرسائل\n\n👉🏼 على سبيل المثال ، <b>تأخير</b> ( <i>بالدقائق</i> ) للمستخدمين <u>الجدد</u> (قبل كتابة رسالتهم <u>الأولى</u> ) يتم باستخدام الأمر: /delay {0}",
 }
 l_cuser_call = {
     'ru': "👮🏽 В настройках [Разрешения] включи опцию:\n\n[✅ Добавление участ]\n\n🕚Подожди 1min",
     'en': "👮🏽 In the [Permissions] settings, enable the option:\n\n[✅ Adding a part]\n\n🕚Wait 1min",
     'es': "👮🏽 En la configuración de [Permisos], habilita la opción:\n\n[✅ Agregar una parte]\n\n🕚Espera 1 minuto",
     'fr': "👮🏽 Dans les paramètres [Autorisations], activez l'option :\n\n[✅ Ajout d'une pièce]\n\n🕚Attendez 1min",
     'zh': "👮🏽 在[权限]设置中，启用选项：\n\n[✅添加零件]\n\n🕚等待1分钟",
@@ -6121,20 +6129,20 @@
     'en': "👮🏽 {0}, on <b>Press</b> the button to join the group",
     'es': "👮🏽 {0}, en <b>Presiona</b> el botón para unirte al grupo",
     'fr': "👮🏽 {0}, sur <b>Appuyez sur</b> le bouton pour rejoindre le groupe",
     'zh': "👮🏽 {0}, on<b>按下</b>按钮加入群组",
     'ar': "👮🏽 {0} ، <b>اضغط</b> على الزر للانضمام إلى المجموعة",
 }
 l_content_types_captcha = {
-    'ru': "👮🏽 {0}, выбери <i>правильный вариант</i> ответа, чтобы вс︎тупить в группу:\n\n<code>{1}</code>",
-    'en': "👮🏽 {0}, choose <i>the correct</i> answer to join the group:\n\n<code>{1}</code>",
-    'es': "👮🏽 {0}, elige <i>la respuesta correcta</i> para unirte al grupo:\n\n<code>{1}</code>",
-    'fr': "👮🏽 {0}, choisis <i>la bonne</i> réponse pour rejoindre le groupe :\n\n<code>{1}</code>",
-    'zh': "👮🏽 {0}，选择<i>正确</i>答案加入群组：\n\n<code>{1}</code>",
-    'ar': "👮🏽 {0} ، اختر الإجابة <i>الصحيحة</i> للانضمام إلى المجموعة:\n\n<code>{1}</code>",
+    'ru': "👮🏽 {0}, выбери <i>правильный вариант</i> ответа, чтобы вс︎тупить в группу:\n\n{1}",
+    'en': "👮🏽 {0}, choose <i>the correct</i> answer to join the group:\n\n{1}",
+    'es': "👮🏽 {0}, elige <i>la respuesta correcta</i> para unirte al grupo:\n\n{1}",
+    'fr': "👮🏽 {0}, choisis <i>la bonne</i> réponse pour rejoindre le groupe :\n\n{1}",
+    'zh': "👮🏽 {0}，选择<i>正确</i>答案加入群组：\n\n{1}",
+    'ar': "👮🏽 {0} ، اختر الإجابة <i>الصحيحة</i> للانضمام إلى المجموعة:\n\n{1}",
 }
 l_hand_msg_FLOOD_USERNAME = {
     'ru': "💬 Пользователь @{0} изменил <b>name/@username</b>! Возможно, шпион!",
     'en': "💬 User @{0} changed <b>name/</b> <b>@username</b> ! Possibly a spy!",
     'es': "💬 ¡Usuario @{0} cambió <b>de nombre/</b> <b>@username</b> ! ¡Posiblemente un espía!",
     'fr': "💬 L'utilisateur @{0} a changé <b>de nom/</b> <b>@username</b> ! Peut-être un espion !",
     'zh': "💬 用户@{0} 更改了<b>名称/</b> <b>@username</b> ！可能是间谍！",
@@ -6343,20 +6351,20 @@
     'en': "🌬 Subscription",
     'es': "🌬 Suscripción",
     'fr': "🌬 Abonnement",
     'zh': "🌬订阅",
     'ar': "🌬 الاشتراك",
 }
 l_bot_welcome = {
-    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>автоматизации</code> <b>Telegram</b>-ботов:\n\n▪️авто-постинг и <b>авто-перевод</b>\n▪️<b>авто-ответы</b> и оповещения\n▪️нейросети: графика и текст бота\n▪️интеграции и платежи\n\n❗️также можно заказать разработку чат-бота в нашей <a href='https://t.me/{1}'>ferey</a>-студии",
-    'en': "🌱 {0}, welcome to the <b>Telegram</b> bot <code>автоматизации</code> <i>landing bot</i> :\n\n▪️auto-posting and <b>auto-translation</b>\n▪️ <b>auto-replies</b> and notifications\n▪️integrations and payments\n▪️users and administrators\n\n❗️You can also order the development of a chatbot in our ferey studio",
-    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> <code>автоматизации</code> de bots <b>de Telegram</b> :\n\n▪️auto-publicación y <b>auto-traducción</b>\n▪️auto <b>-respuestas</b> y notificaciones\n▪️integraciones y pagos\n▪️usuarios y administradores\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro ferey studio",
-    'fr': "🌱 {0}, bienvenue dans le <i>bot d&#x27;atterrissage</i> <code>автоматизации</code> du bot <b>Telegram</b> :\n\n▪️publication et <b>traduction automatiques</b>\n▪️ <b>réponses et notifications automatiques</b>\n▪️intégrations et paiements\n▪️utilisateurs et administrateurs\n\n❗️Vous pouvez également commander le développement d'un chatbot dans notre studio ferey",
-    'zh': "🌱 {0}，欢迎使用<b>Telegram</b>机器人<code>автоматизации</code><i>登陆机器人</i>：\n\n▪️自动发布和<b>自动翻译</b>\n▪️<b>自动回复</b>和通知\n▪️集成和支付\n▪️用户和管理员\n\n❗️您也可以在我们的ferey工作室订购聊天机器人的开发",
-    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> <code>автоматизации</code> لروبوت <b>Telegram</b> :\n\n▪️ النشر التلقائي <b>والترجمة التلقائية</b>\n▪️ <b>الردود التلقائية</b> والإشعارات\n▪️ عمليات الدمج والمدفوعات\nالمستخدمون والمسؤولون\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو ferey الخاص بنا",
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> автоматизации <b>Telegram</b>-ботов:\n\n▪️авто-постинг и <b>авто-перевод</b>\n▪️<b>авто-ответы</b> и оповещения\n▪️нейросети: графика и текст бота\n▪️интеграции и платежи\n\n❗️также можно заказать разработку чат-бота в нашей <a href='https://t.me/{1}'>ferey</a>-студии",
+    'en': "🌱 {0}, welcome to the <b>Telegram</b> bot автоматизации <i>landing bot</i> :\n\n▪️auto-posting and <b>auto-translation</b>\n▪️ <b>auto-replies</b> and notifications\n▪️integrations and payments\n▪️users and administrators\n\n❗️You can also order the development of a chatbot in our ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> автоматизации de bots <b>de Telegram</b> :\n\n▪️auto-publicación y <b>auto-traducción</b>\n▪️auto <b>-respuestas</b> y notificaciones\n▪️integraciones y pagos\n▪️usuarios y administradores\n\n❗️también puedes encargar el desarrollo de un chatbot en nuestro ferey studio",
+    'fr': "🌱 {0}, bienvenue dans le <i>bot d&#x27;atterrissage</i> автоматизации du bot <b>Telegram</b> :\n\n▪️publication et <b>traduction automatiques</b>\n▪️ <b>réponses et notifications automatiques</b>\n▪️intégrations et paiements\n▪️utilisateurs et administrateurs\n\n❗️Vous pouvez également commander le développement d'un chatbot dans notre studio ferey",
+    'zh': "🌱 {0}，欢迎使用<b>Telegram</b>机器人автоматизации<i>登陆机器人</i>：\n\n▪️自动发布和<b>自动翻译</b>\n▪️<b>自动回复</b>和通知\n▪️集成和支付\n▪️用户和管理员\n\n❗️您也可以在我们的ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>الروبوت الهبوط</i> автоматизации لروبوت <b>Telegram</b> :\n\n▪️ النشر التلقائي <b>والترجمة التلقائية</b>\n▪️ <b>الردود التلقائية</b> والإشعارات\n▪️ عمليات الدمج والمدفوعات\nالمستخدمون والمسؤولون\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو ferey الخاص بنا",
 }
 l_subscribe_bot = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [@{0}-бот]:\n▪️авто-перевод\n(<i>в том числе, текста кнопок</i>)\n▪️авто-ответ\n(<i>chatgpt видит блоки бота</i>)\n▪️приоритетная поддержка\n\n👩🏽‍💻 /balance",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -6416,20 +6424,20 @@
     'en': "©️ Bot <b>cloning</b>\n\n#duration 1 min",
     'es': "©️ <b>Clonación</b> de bots\n\n#duración 1 min",
     'fr': "©️ <b>Clonage</b> de bot\n\n#durée 1 min",
     'zh': "©️ Bot<b>克隆</b>\n\n#duration 1 分钟",
     'ar': "© ️ <b>استنساخ</b> الروبوت\n\n# المدة 1 دقيقة",
 }
 l_addbot_handler = {
-    'ru': "➕ Пришли корректный <b>ТОКЕН</b> Telegram-бота, полученный с помощью @botFather-бота\n\n👩🏽‍💻 Например, <code>117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN</code>",
-    'en': "➕ We sent the correct Telegram bot <b>TOKEN</b> received using @botFather bot\n\n👩🏽‍💻 For example, <code>117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN</code>",
-    'es': "➕ Enviamos el <b>TOKEN</b> de bot de Telegram correcto recibido usando @botFather bot\n\n👩🏽‍💻 Por ejemplo, <code>117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN</code>",
-    'fr': "➕ Nous avons envoyé le bon <b>jeton</b> de bot Telegram reçu à l&#x27;aide du bot @botFather\n\n👩🏽‍💻 Par exemple, <code>117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN</code>",
-    'zh': "➕ 我们发送了使用@botFather bot\n\n👩🏽‍💻 收到的正确的 Telegram bot <b>TOKEN</b>例如， <code>117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN</code>",
-    'ar': "➕ أرسلنا <b>برنامج</b> Telegram bot الصحيح الذي تم استلامه باستخدام @botFather bot\n\n👩🏽‍💻 على سبيل المثال ، <code>117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN</code>",
+    'ru': "➕ Пришли корректный <b>ТОКЕН</b> Telegram-бота, полученный с помощью @botFather-бота\n\n👩🏽‍💻 Например, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'en': "➕ We sent the correct Telegram bot <b>TOKEN</b> received using @botFather bot\n\n👩🏽‍💻 For example, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'es': "➕ Enviamos el <b>TOKEN</b> de bot de Telegram correcto recibido usando @botFather bot\n\n👩🏽‍💻 Por ejemplo, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'fr': "➕ Nous avons envoyé le bon <b>jeton</b> de bot Telegram reçu à l&#x27;aide du bot @botFather\n\n👩🏽‍💻 Par exemple, 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'zh': "➕ 我们发送了使用@botFather bot\n\n👩🏽‍💻 收到的正确的 Telegram bot <b>TOKEN</b>例如， 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
+    'ar': "➕ أرسلنا <b>برنامج</b> Telegram bot الصحيح الذي تم استلامه باستخدام @botFather bot\n\n👩🏽‍💻 على سبيل المثال ، 117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN",
 }
 l_wait_for_translate_bot = {
     'ru': "👩🏽‍💻 <b>Перевод</b> {0}-бота на <i>{1}</i>-язык\n\n#длительность 0мин",
     'en': "👩🏽‍💻 <b>Translation of</b> {0}-bot into <i>{1}</i> -language\n\n#duration 0min",
     'es': "👩🏽‍💻 <b>Traducción de</b> {0}-bot a <i>{1}</i> -idioma\n\n#duración 0min",
     'fr': "👩🏽‍💻 <b>Traduction de</b> {0}-bot en <i>{1}</i> -langue\n\n#durée 0min",
     'zh': "👩🏽‍💻 将 {0}-bot<b>翻译</b>成<i>{1}</i> -language\n\n#duration 0min",
@@ -6458,20 +6466,20 @@
     'fr': "👩🏽‍💻 *Code promotionnel* : `{txt}` activé",
     'zh': "👩🏽‍💻 *促销代码*：`{txt}` 激活",
     'ar': "👩🏽‍💻 * الرمز الترويجي *: '{txt}` مفعل",
 }
 
 # region commands
 l_bot_commands_handler = {
-    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/status <i>статус</i>\n/on     <i>включение</i>\n<code>/off</code>    <i>выключение</i>\n<code>/restart</code>  <i>перезагрузка</i>\n\n/parse [premium|admin|utm|ban]\n/admin [id]    <i>администраторы</i>\n/promo      <i>промокод</i>\n/ban [id/@username]   <i>список</i>\n/unban     <i>разбан</i>",
-    'en': "⚙️ <b>Commands</b> /cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n<code>/off</code> <i>disable</i>\n<code>/restart</code> <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>promo code</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'es': "⚙️ <b>Comandos</b> /cmd para <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n<code>/off</code> <i>disabled</i>\n<code>/restart</code> <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>administradores</i>\n/promo <i>código de promoción</i>\n/ban [id/ @username ] <i>lista</i>\n/unban <i>no baneado</i>",
-    'fr': "⚙️ <b>Commandes</b> /cmd pour <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n<code>/off</code> <i>disable</i>\n<code>/restart</code> <i>recharger</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>code promo</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'zh': "⚙️<b>命令</b>/cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n<code>/off</code> <i>disable</i>\n<code>/restart</code> <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo<i>促销代码</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
-    'ar': "⚙️ <b>أوامر</b> / cmd لـ <b>@ {0}</b>\n\n/ info <i>info</i>\n/ stat <i>analytics</i>\n/ status <i>status</i>\n/ on <i>تمكين</i>\n<code>/off</code> <i>تعطيل</i>\n<code>/restart</code> <i>تحميل</i>\n\n/ parse [premium | admin | utm | ban]\n/ admin [id] <i>admins</i>\n/ <i>promo code</i>\n/ ban [id / @username ] <i>list</i>\n/ <i>unsanned</i>",
+    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/status <i>статус</i>\n/on     <i>включение</i>\n/off    <i>выключение</i>\n/restart  <i>перезагрузка</i>\n\n/parse [premium|admin|utm|ban]\n/admin [id]    <i>администраторы</i>\n/promo      <i>промокод</i>\n/ban [id/@username]   <i>список</i>\n/unban     <i>разбан</i>",
+    'en': "⚙️ <b>Commands</b> /cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>promo code</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
+    'es': "⚙️ <b>Comandos</b> /cmd para <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disabled</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>administradores</i>\n/promo <i>código de promoción</i>\n/ban [id/ @username ] <i>lista</i>\n/unban <i>no baneado</i>",
+    'fr': "⚙️ <b>Commandes</b> /cmd pour <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>recharger</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo <i>code promo</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
+    'zh': "⚙️<b>命令</b>/cmd for <b>@{0}</b>\n\n/info <i>info</i>\n/stat <i>analytics</i>\n/status <i>status</i>\n/on <i>enable</i>\n/off <i>disable</i>\n/restart <i>reload</i>\n\n/parse [premium| admin|utm|ban]\n/admin [id] <i>admins</i>\n/promo<i>促销代码</i>\n/ban [id/ @username ] <i>list</i>\n/unban <i>unbanned</i>",
+    'ar': "⚙️ <b>أوامر</b> / cmd لـ <b>@ {0}</b>\n\n/ info <i>info</i>\n/ stat <i>analytics</i>\n/ status <i>status</i>\n/ on <i>تمكين</i>\n/off <i>تعطيل</i>\n/restart <i>تحميل</i>\n\n/ parse [premium | admin | utm | ban]\n/ admin [id] <i>admins</i>\n/ <i>promo code</i>\n/ ban [id / @username ] <i>list</i>\n/ <i>unsanned</i>",
 }
 l_bot_status_handler = {
     'ru': "👩🏽‍💻 <b>Статус</b> @{0}-бота: {1}",
     'en': "👩🏽‍💻 <b>Status</b> @{0}-bot: {1}",
     'es': "👩🏽‍💻 <b>Estado</b> @{0}-bot: {1}",
     'fr': "👩🏽‍💻 <b>Statut</b> @{0}-bot : {1}",
     'zh': "👩🏽‍💻<b>状态</b>@{0}-bot：{1}",
@@ -6736,36 +6744,36 @@
     'en': "💳️ You need to ⚙️Set up at least one payment token",
     'es': "💳️ Debes ⚙️Configurar al menos un token de pago",
     'fr': "💳️ Vous devez ⚙️Configurer au moins un jeton de paiement",
     'zh': "💳️您需要⚙️设置至少一个支付令牌",
     'ar': "💳️ تحتاج إلى إعداد رمز دفع واحد على الأقل",
 }
 l_cpayment_text = {
-    'ru': "💳️ <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> платежи в @{0}-боте\n\n👩🏽‍💻 <b>Текущий</b> платежный токен:\n<code>{1}</code>",
-    'en': "💳️ <b>Click</b> on ✅/☑️ to <b>turn on/off</b> payments in @{0}-bot\n\n👩🏽‍💻 <b>Current</b> payment token:\n<code>{1}</code>",
-    'es': "💳️ <b>Haz clic</b> en ✅/☑️ para <b>activar o desactivar</b> los pagos en @{0}-bot\n\n👩🏽‍💻 Token de pago <b>actual</b> :\n<code>{1}</code>",
-    'fr': "💳️ <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> les paiements dans @{0}-bot\n\n👩🏽‍💻 Jeton de paiement <b>actuel</b> :\n<code>{1}</code>",
-    'zh': "💳️<b>点击</b>✅/☑️ 在@{0}-bot 中<b>打开/关闭</b>支付\n\n👩🏽‍💻<b>当前</b>支付令牌：\n<code>{1}</code>",
-    'ar': "💳️ <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> المدفوعات في @ {0} -bot\n\n👩🏽‍💻 رمز الدفع <b>الحالي</b> :\n<code>{1}</code>",
+    'ru': "💳️ <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> платежи в @{0}-боте\n\n👩🏽‍💻 <b>Текущий</b> платежный токен:\n{1}",
+    'en': "💳️ <b>Click</b> on ✅/☑️ to <b>turn on/off</b> payments in @{0}-bot\n\n👩🏽‍💻 <b>Current</b> payment token:\n{1}",
+    'es': "💳️ <b>Haz clic</b> en ✅/☑️ para <b>activar o desactivar</b> los pagos en @{0}-bot\n\n👩🏽‍💻 Token de pago <b>actual</b> :\n{1}",
+    'fr': "💳️ <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> les paiements dans @{0}-bot\n\n👩🏽‍💻 Jeton de paiement <b>actuel</b> :\n{1}",
+    'zh': "💳️<b>点击</b>✅/☑️ 在@{0}-bot 中<b>打开/关闭</b>支付\n\n👩🏽‍💻<b>当前</b>支付令牌：\n{1}",
+    'ar': "💳️ <b>انقر</b> على ✅ / ☑️ <b>لتشغيل / إيقاف</b> المدفوعات في @ {0} -bot\n\n👩🏽‍💻 رمز الدفع <b>الحالي</b> :\n{1}",
 }
 l_cpayment_token = {
-    'ru': "💳️ <b>Вставь</b> платежный токен, полученный из @BotFather-бота\n\n👩🏽‍💻 <b>Например</b>\n<code>401643678:7049d0b3-f0267096c4a1</code>\n\n👩🏽‍💻 <b>Текущий</b> токен:\n{0}",
-    'en': "💳️ <b>Insert</b> payment token received from @BotFather -bot\n\n👩🏽‍💻 <b>For example</b>\n<code>401643678:7049d0b3-f0267096c4a1</code>\n\n👩🏽‍💻 <b>Current</b> token:\n{0}",
-    'es': "💳️ <b>Inserte</b> el token de pago recibido de @BotFather -bot\n\n👩🏽‍💻 <b>Por ejemplo,</b>\n<code>401643678:7049d0b3-f0267096c4a1</code>\n\n👩🏽‍💻 Token <b>actual</b> :\n{0}",
-    'fr': "💳️ <b>Insérez</b> le jeton de paiement reçu de @BotFather -bot\n\n👩🏽‍💻 <b>Par exemple</b>\n<code>401643678:7049d0b3-f0267096c4a1</code>\n\n👩🏽‍💻 Jeton <b>actuel</b> :\n{0}",
-    'zh': "💳️<b>插入</b>从@BotFather -bot 收到的支付令牌\n\n👩🏽‍💻<b>例如</b>\n<code>401643678:7049d0b3-f0267096c4a1</code>\n\n👩🏽‍💻<b>当前</b>令牌：\n{0}",
-    'ar': "💳️ <b>أدخل</b> رمز الدفع المستلم من @BotFather -bot\n\n👩🏽‍💻 <b>على سبيل المثال</b>\n<code>401643678:7049d0b3-f0267096c4a1</code>\n\n👩🏽‍💻 الرمز <b>المميز الحالي</b> :\n{0}",
+    'ru': "💳️ <b>Вставь</b> платежный токен, полученный из @BotFather-бота\n\n👩🏽‍💻 <b>Например</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 <b>Текущий</b> токен:\n{0}",
+    'en': "💳️ <b>Insert</b> payment token received from @BotFather -bot\n\n👩🏽‍💻 <b>For example</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 <b>Current</b> token:\n{0}",
+    'es': "💳️ <b>Inserte</b> el token de pago recibido de @BotFather -bot\n\n👩🏽‍💻 <b>Por ejemplo,</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 Token <b>actual</b> :\n{0}",
+    'fr': "💳️ <b>Insérez</b> le jeton de paiement reçu de @BotFather -bot\n\n👩🏽‍💻 <b>Par exemple</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 Jeton <b>actuel</b> :\n{0}",
+    'zh': "💳️<b>插入</b>从@BotFather -bot 收到的支付令牌\n\n👩🏽‍💻<b>例如</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻<b>当前</b>令牌：\n{0}",
+    'ar': "💳️ <b>أدخل</b> رمز الدفع المستلم من @BotFather -bot\n\n👩🏽‍💻 <b>على سبيل المثال</b>\n401643678:7049d0b3-f0267096c4a1\n\n👩🏽‍💻 الرمز <b>المميز الحالي</b> :\n{0}",
 }
 l_cpayment_done = {
-    'ru': "💳️ <b>Готово!</b>\n\n👩🏽‍💻 <b>Текущий</b> платежный токен для @{0}-бота:\n\n<code>{1}</code>",
-    'en': "💳️ <b>Done!</b>\n\n👩🏽‍💻 <b>Current</b> payment token for @{0}-bot:\n\n<code>{1}</code>",
-    'es': "💳️ <b>Listo!</b>\n\n👩🏽‍💻 Token de pago <b>actual</b> para @{0}-bot:\n\n<code>{1}</code>",
-    'fr': "💳️ <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 Jeton de paiement <b>actuel</b> pour @{0}-bot :\n\n<code>{1}</code>",
-    'zh': "💳️<b>完成！</b>\n\n👩🏽‍💻 @{0}-bot 的<b>当前</b>支付令牌：\n\n<code>{1}</code>",
-    'ar': "💳️ <b>انتهى!</b>\n\n👩🏽‍💻 رمز الدفع <b>الحالي</b> لـ @ {0} -bot:\n\n<code>{1}</code>",
+    'ru': "💳️ <b>Готово!</b>\n\n👩🏽‍💻 <b>Текущий</b> платежный токен для @{0}-бота:\n\n{1}",
+    'en': "💳️ <b>Done!</b>\n\n👩🏽‍💻 <b>Current</b> payment token for @{0}-bot:\n\n{1}",
+    'es': "💳️ <b>Listo!</b>\n\n👩🏽‍💻 Token de pago <b>actual</b> para @{0}-bot:\n\n{1}",
+    'fr': "💳️ <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 Jeton de paiement <b>actuel</b> pour @{0}-bot :\n\n{1}",
+    'zh': "💳️<b>完成！</b>\n\n👩🏽‍💻 @{0}-bot 的<b>当前</b>支付令牌：\n\n{1}",
+    'ar': "💳️ <b>انتهى!</b>\n\n👩🏽‍💻 رمز الدفع <b>الحالي</b> لـ @ {0} -bot:\n\n{1}",
 }
 # endregion
 
 
 # region cintegration_
 l_cintegration_alert = {
     'ru': "🗝️ Нужно ⚙️Настроить ССЫЛКУ доступа",
@@ -6814,48 +6822,48 @@
     'es': "☑️☐Выкл airtable-crm",
     'fr': "☑️☐Выкл airtable-crm",
     'zh': "☑️☐Выкл airtable-crm",
     'ar': "☑️☐Выкл airtable-crm",
 }
 
 l_cintegration_google = {
-    'ru': "🗝️ <b>Вставь ссылку</b> на пустую google-таблицу (<i>с открытым доступом для редактирования</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, <code>https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing</code>\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
-    'en': "🗝️ <b>Insert a link</b> to an empty google spreadsheet ( <i>with open access for editing</i> ) to integrate with the @{0}-bot user base\n\n👩🏽‍💻 <b>For example</b> , <code>https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing</code>\n\n👩🏽‍💻 <b>Current</b> URL:\n{1}",
-    'es': "🗝️ <b>Inserta un enlace</b> a una hoja de cálculo de Google vacía ( <i>con acceso abierto para editar</i> ) para integrarla con la base de usuarios de @{0}-bot\n\n👩🏽‍💻 <b>Por ejemplo</b> , <code>https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing</code>\n\n👩🏽‍💻 URL <b>actual</b> :\n{1}",
-    'fr': "🗝️ <b>Insérez un lien</b> vers une feuille de calcul Google vide ( <i>avec accès ouvert pour modification</i> ) à intégrer à la base d&#x27;utilisateurs @{0}-bot\n\n👩🏽‍💻 <b>Par exemple</b> , <code>https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing</code>\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{1}",
-    'zh': "🗝️<b>插入指向空谷歌电子表格的链接</b>（<i>开放编辑权限</i>）以与@{0}-bot 用户群集成\n\n👩🏽‍💻<b>例如</b>，https: <code>https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing</code>\n\n👩🏽‍💻<b>当前</b>网址：\n{1}",
-    'ar': "🗝️ <b>أدخل رابطًا</b> إلى جدول بيانات google فارغ ( <i>مع وصول مفتوح للتعديل</i> ) للتكامل مع @ {0} -bot user base\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، <code>https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing</code>\n\n👩🏽‍💻 عنوان URL <b>الحالي</b> :\n{1}",
+    'ru': "🗝️ <b>Вставь ссылку</b> на пустую google-таблицу (<i>с открытым доступом для редактирования</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
+    'en': "🗝️ <b>Insert a link</b> to an empty google spreadsheet ( <i>with open access for editing</i> ) to integrate with the @{0}-bot user base\n\n👩🏽‍💻 <b>For example</b> , https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 <b>Current</b> URL:\n{1}",
+    'es': "🗝️ <b>Inserta un enlace</b> a una hoja de cálculo de Google vacía ( <i>con acceso abierto para editar</i> ) para integrarla con la base de usuarios de @{0}-bot\n\n👩🏽‍💻 <b>Por ejemplo</b> , https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 URL <b>actual</b> :\n{1}",
+    'fr': "🗝️ <b>Insérez un lien</b> vers une feuille de calcul Google vide ( <i>avec accès ouvert pour modification</i> ) à intégrer à la base d&#x27;utilisateurs @{0}-bot\n\n👩🏽‍💻 <b>Par exemple</b> , https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{1}",
+    'zh': "🗝️<b>插入指向空谷歌电子表格的链接</b>（<i>开放编辑权限</i>）以与@{0}-bot 用户群集成\n\n👩🏽‍💻<b>例如</b>，https: https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻<b>当前</b>网址：\n{1}",
+    'ar': "🗝️ <b>أدخل رابطًا</b> إلى جدول بيانات google فارغ ( <i>مع وصول مفتوح للتعديل</i> ) للتكامل مع @ {0} -bot user base\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، https://docs.google.com/spreadsheets/d/1aWGYLL0WWZP/edit?usp=sharing\n\n👩🏽‍💻 عنوان URL <b>الحالي</b> :\n{1}",
 }
 l_cintegration_airtable = {
-    'ru': "🗝️ <b>Вставь ссылку</b> на пустую airtable-таблицу (<i>с открытым доступом для редактирования и любого e-mail</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, <code>https://airtable.com/invite/l?inviteId=inv4VGM&inviteToken=f1d31f9aba6b&utm_medium=email</code>\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
-    'en': "🗝️ <b>Insert a link</b> to an empty airtable-table ( <i>with open access for editing and any e-mail</i> ) for integration with the @{0}-bot user base\n\n👩🏽‍💻 <b>For example</b> , <code>https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email</code>\n\n👩🏽‍💻 <b>Current</b> URL:\n{1}",
-    'es': "🗝️ <b>Inserte un enlace</b> a una mesa de aire vacía ( <i>con acceso abierto para editar y cualquier correo electrónico</i> ) para la integración con la base de usuarios de @{0}-bot\n\n👩🏽‍💻 <b>Por ejemplo</b> , <code>https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email</code>\n\n👩🏽‍💻 URL <b>actual</b> :\n{1}",
-    'fr': "🗝️ <b>Insérez un lien</b> vers une table airtable vide ( <i>avec un accès ouvert pour l&#x27;édition et tout e-mail</i> ) pour l&#x27;intégration avec la base d&#x27;utilisateurs @{0}-bot\n\n👩🏽‍💻 <b>Par exemple</b> , <code>https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email</code>\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{1}",
-    'zh': "🗝️<b>插入一个指向空的 airtable-table 的链接</b>（<i>具有编辑和任何电子邮件的开放访问权限</i>）以与 @{0}-bot 用户群集成\n\n👩🏽‍💻<b>例如</b>， <code>https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email</code>\n\n👩🏽‍💻<b>当前</b>网址：\n{1}",
-    'ar': "🗝️ <b>أدخل ارتباطًا</b> إلى جدول airtable فارغ ( <i>مع وصول مفتوح للتحرير وأي بريد إلكتروني</i> ) للتكامل مع @ {0} -bot user base\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، <code>https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email</code> <b>؟</b>",
+    'ru': "🗝️ <b>Вставь ссылку</b> на пустую airtable-таблицу (<i>с открытым доступом для редактирования и любого e-mail</i>) для интеграции с базой пользователей @{0}-бота\n\n👩🏽‍💻 <b>Например</b>, https://airtable.com/invite/l?inviteId=inv4VGM&inviteToken=f1d31f9aba6b&utm_medium=email\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{1}",
+    'en': "🗝️ <b>Insert a link</b> to an empty airtable-table ( <i>with open access for editing and any e-mail</i> ) for integration with the @{0}-bot user base\n\n👩🏽‍💻 <b>For example</b> , https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻 <b>Current</b> URL:\n{1}",
+    'es': "🗝️ <b>Inserte un enlace</b> a una mesa de aire vacía ( <i>con acceso abierto para editar y cualquier correo electrónico</i> ) para la integración con la base de usuarios de @{0}-bot\n\n👩🏽‍💻 <b>Por ejemplo</b> , https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻 URL <b>actual</b> :\n{1}",
+    'fr': "🗝️ <b>Insérez un lien</b> vers une table airtable vide ( <i>avec un accès ouvert pour l&#x27;édition et tout e-mail</i> ) pour l&#x27;intégration avec la base d&#x27;utilisateurs @{0}-bot\n\n👩🏽‍💻 <b>Par exemple</b> , https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{1}",
+    'zh': "🗝️<b>插入一个指向空的 airtable-table 的链接</b>（<i>具有编辑和任何电子邮件的开放访问权限</i>）以与 @{0}-bot 用户群集成\n\n👩🏽‍💻<b>例如</b>， https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email\n\n👩🏽‍💻<b>当前</b>网址：\n{1}",
+    'ar': "🗝️ <b>أدخل ارتباطًا</b> إلى جدول airtable فارغ ( <i>مع وصول مفتوح للتحرير وأي بريد إلكتروني</i> ) للتكامل مع @ {0} -bot user base\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، https://airtable.com/invite/l?inviteId=inv4VGM&amp;inviteToken=f1d31f9aba6b&amp;utm_medium=email <b>؟</b>",
 }
 l_cintegration_done = {
     'ru': "🗝️ <b>Готово!</b>\n\n👩🏽‍💻 <b>Текущая</b> ссылка:\n{0}",
     'en': "🗝️ <b>Done!</b>\n\n👩🏽‍💻 <b>Current</b> URL:\n{0}",
     'es': "🗝️ <b>Listo!</b>\n\n👩🏽‍💻 URL <b>actual</b> :\n{0}",
     'fr': "🗝️ <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 URL <b>actuelle</b> :\n{0}",
     'zh': "🗝️<b>完成！</b>\n\n👩🏽‍💻<b>当前</b>网址：\n{0}",
     'ar': "🗝️ <b>انتهى!</b>\n\n👩🏽‍💻 عنوان URL <b>الحالي</b> :\n{0}",
 }
 # endregion
 
 
 # region cnotification_
 l_cnotification_text = {
-    'ru': "💬 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> оповещения о <i><b>/start-stop</b> запуске/блокировке бота пользователем и попадании пользователя в <b>/ban</b>-список/<b>нажатии</b> на кнопки пользователем/<b>диалоге</b> с администраторами/<b>всех</b> действиях пользователя</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает <code>показ</code> сообщений от пользователя администраторам бота (/admin) с возможностью реплай-ответа на сообщения",
-    'en': "💬 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> notifications about <i><b>/start-stop</b> launching/blocking the bot by the user and getting the user into the <b>/ban</b> -list/ <b>pressing</b> buttons by the user/ <b>dialog</b> with administrators/ <b>all</b> user actions</i>\n\n👩🏽‍💻 For example, the option [<b>{0}</b>] means <code>показ</code> messages from the user to bot administrators (/admin) with the ability to replay response to messages",
-    'es': "💬 <b>Haga clic</b> en ✅/☑️ para <b>activar/desactivar</b> las notificaciones sobre <i><b>/iniciar y detener</b> el lanzamiento/bloqueo del bot por parte del usuario y colocar al usuario en la <b>/lista de prohibición</b> / <b>pulsar</b> botones por parte del usuario/ <b>diálogo</b> con los administradores/ <b>todas</b> las acciones del usuario \</i> n\n👩🏽‍💻 Por ejemplo, la opción [<b>{0}</b>] significa <code>показ</code> los mensajes del usuario a los administradores del bot (/admin) con la capacidad de reproducir la respuesta a los mensajes.",
-    'fr': "💬 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> les notifications sur <i><b>/start-stop</b> lancer/bloquer le bot par l&#x27;utilisateur et faire entrer l&#x27;utilisateur dans la <b>/banni</b> -liste/ <b>appuyer sur</b> les boutons par l&#x27;utilisateur/ <b>dialogue</b> avec les administrateurs/ <b>toutes</b> les actions de l&#x27;utilisateur \</i> n\n👩🏽‍💻 Par exemple, l&#x27;option [<b>{0}</b>] signifie <code>показ</code> les messages de l'utilisateur aux administrateurs du bot (/admin) avec la possibilité de rejouer la réponse aux messages",
-    'zh': "💬<b>单击</b>✅/☑️ 以<b>打开/关闭</b><i>关于<b>/start-stop</b>启动/阻止用户的机器人并让用户进入<b>/ban</b>列表/用户<b>按下</b>按钮/与管理员<b>对话</b>/<b>所有</b>用户操作的通知 \</i> n\n👩🏽‍💻 例如，选项 [<b>{0}</b>] 表示将用户的消息<code>показ</code>给机器人管理员 (/admin)，并能够重播对消息的响应",
-    'ar': "💬 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف تشغيل</b> <i>الإشعارات حول <b>/ بدء - إيقاف</b> تشغيل / حظر الروبوت من قبل المستخدم وإدخال المستخدم في أزرار <b>/ قائمة الحظر</b> / <b>الضغط</b> بواسطة المستخدم / <b>الحوار</b> مع المسؤولين / <b>جميع</b> إجراءات المستخدم \</i> n\n👩🏽‍💻 على سبيل المثال ، الخيار [<b>{0}</b>] يعني <code>показ</code> الرسائل من المستخدم إلى المشرفين (/ admin) مع إمكانية إعادة الرد على الرسائل",
+    'ru': "💬 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> оповещения о <i><b>/start-stop</b> запуске/блокировке бота пользователем и попадании пользователя в <b>/ban</b>-список/<b>нажатии</b> на кнопки пользователем/<b>диалоге</b> с администраторами/<b>всех</b> действиях пользователя</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает показ сообщений от пользователя администраторам бота (/admin) с возможностью реплай-ответа на сообщения",
+    'en': "💬 <b>Click</b> on ✅/☑️ to <b>turn on/off</b> notifications about <i><b>/start-stop</b> launching/blocking the bot by the user and getting the user into the <b>/ban</b> -list/ <b>pressing</b> buttons by the user/ <b>dialog</b> with administrators/ <b>all</b> user actions</i>\n\n👩🏽‍💻 For example, the option [<b>{0}</b>] means показ messages from the user to bot administrators (/admin) with the ability to replay response to messages",
+    'es': "💬 <b>Haga clic</b> en ✅/☑️ para <b>activar/desactivar</b> las notificaciones sobre <i><b>/iniciar y detener</b> el lanzamiento/bloqueo del bot por parte del usuario y colocar al usuario en la <b>/lista de prohibición</b> / <b>pulsar</b> botones por parte del usuario/ <b>diálogo</b> con los administradores/ <b>todas</b> las acciones del usuario \</i> n\n👩🏽‍💻 Por ejemplo, la opción [<b>{0}</b>] significa показ los mensajes del usuario a los administradores del bot (/admin) con la capacidad de reproducir la respuesta a los mensajes.",
+    'fr': "💬 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> les notifications sur <i><b>/start-stop</b> lancer/bloquer le bot par l&#x27;utilisateur et faire entrer l&#x27;utilisateur dans la <b>/banni</b> -liste/ <b>appuyer sur</b> les boutons par l&#x27;utilisateur/ <b>dialogue</b> avec les administrateurs/ <b>toutes</b> les actions de l&#x27;utilisateur \</i> n\n👩🏽‍💻 Par exemple, l&#x27;option [<b>{0}</b>] signifie показ les messages de l'utilisateur aux administrateurs du bot (/admin) avec la possibilité de rejouer la réponse aux messages",
+    'zh': "💬<b>单击</b>✅/☑️ 以<b>打开/关闭</b><i>关于<b>/start-stop</b>启动/阻止用户的机器人并让用户进入<b>/ban</b>列表/用户<b>按下</b>按钮/与管理员<b>对话</b>/<b>所有</b>用户操作的通知 \</i> n\n👩🏽‍💻 例如，选项 [<b>{0}</b>] 表示将用户的消息показ给机器人管理员 (/admin)，并能够重播对消息的响应",
+    'ar': "💬 <b>انقر</b> فوق ✅ / ☑️ <b>لتشغيل / إيقاف تشغيل</b> <i>الإشعارات حول <b>/ بدء - إيقاف</b> تشغيل / حظر الروبوت من قبل المستخدم وإدخال المستخدم في أزرار <b>/ قائمة الحظر</b> / <b>الضغط</b> بواسطة المستخدم / <b>الحوار</b> مع المسؤولين / <b>جميع</b> إجراءات المستخدم \</i> n\n👩🏽‍💻 على سبيل المثال ، الخيار [<b>{0}</b>] يعني показ الرسائل من المستخدم إلى المشرفين (/ admin) مع إمكانية إعادة الرد على الرسائل",
 }
 l_cnotification_start_on = {
     'ru': "✅☑Вкл /start-stop-/ban",
     'en': "✅☑On /start-stop-/ban",
     'es': "✅☑Activar/iniciar-detener-/prohibir",
     'fr': "✅☑On /start-stop-/interdiction",
     'zh': "✅☑开/启-停-/禁",
@@ -6916,32 +6924,32 @@
     'es': "☑️☐Desactivar todas las acciones",
     'fr': "☑️☐Désactiver toutes les actions",
     'zh': "☑️☐关闭所有操作",
     'ar': "☑️☐ إيقاف جميع الإجراءات",
 }
 
 l_cnotification_dialog = {
-    'ru': "💬 <b>Пользователь</b>: {0} [<b>id</b>=<code>{1}</code>] написал в @{2}-боте:",
-    'en': "💬 <b>User</b> : {0} [<b>id</b> = <code>{1}</code>] wrote in @{2}-bot:",
-    'es': "💬 <b>Usuario</b> : {0} [<b>id</b> = <code>{1}</code>] escribió en @{2}-bot:",
-    'fr': "💬 <b>Utilisateur</b> : {0} [<b>id</b> = <code>{1}</code>] a écrit dans @{2}-bot :",
-    'zh': "💬<b>用户</b>：{0} [<b>id</b> = <code>{1}</code>] 在@{2}-bot 中写道：",
-    'ar': "💬 <b>المستخدم</b> : {0} [<b>id</b> = <code>{1}</code>] كتب في @ {2} -bot:",
+    'ru': "💬 <b>Пользователь</b>: {0} [<b>id</b>={1}] написал в @{2}-боте:",
+    'en': "💬 <b>User</b> : {0} [<b>id</b> = {1}] wrote in @{2}-bot:",
+    'es': "💬 <b>Usuario</b> : {0} [<b>id</b> = {1}] escribió en @{2}-bot:",
+    'fr': "💬 <b>Utilisateur</b> : {0} [<b>id</b> = {1}] a écrit dans @{2}-bot :",
+    'zh': "💬<b>用户</b>：{0} [<b>id</b> = {1}] 在@{2}-bot 中写道：",
+    'ar': "💬 <b>المستخدم</b> : {0} [<b>id</b> = {1}] كتب في @ {2} -bot:",
 }
 # endregion
 
 
 # region cuser_
 l_cuser_text2 = {
-    'ru': "👥 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>замену голосовых/телескопов на <b>audio/video</b> (*рекомендуется, если <code>premium</code>-пользователи установили такой запрет)/сервисные <b>статусы</b> бота (печатает..записывает видео..)/ведение списка <b>/utm-рефералов</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/utm - вывести utm-рефералов\n/link - создать реферальную /utm ссылку",
-    'en': "👥 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <i>the replacement of voice/telescopes with <b>audio/video</b> (*recommended if</i> <code>premium</code> <i>users have set such a ban)/bot service <b>statuses</b> (prints..records video..)/maintaining a list of <b>/utm referrals</b></i>\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/parse - display all users\n/utm - display utm referrals\n/link - create a referral /utm link",
-    'es': "👥 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> <i>el reemplazo de voz/telescopios con <b>audio/video</b> (*recomendado si</i> los usuarios <code>premium</code> <i>han establecido dicha prohibición)/ <b>estados</b> de servicio de bot (imprime... graba video...)/mantiene una lista de <b>/utm referencias</b></i>\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/parse - mostrar todos los usuarios\n/utm - mostrar referencias utm\n/link - crear un enlace de referencia /utm",
-    'fr': "👥 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>le remplacement de la voix/des télescopes par <b>l&#x27;audio/la vidéo</b> (*recommandé si</i> les utilisateurs <code>premium</code> <i>ont défini une telle interdiction)/ <b>les statuts</b> du service de bot (imprime..enregistre la vidéo..)/maintient une liste de <b>/références utm</b></i>\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/parse - afficher tous les utilisateurs\n/utm - afficher les références utm\n/lien - créer une référence /lien utm",
-    'zh': "👥<b>点击</b>✅/☑️<b>启用/禁用</b><i>用音频<b>/视频</b>替换语音/望远镜（*如果</i><code>premium</code><i>用户设置了此类禁令，则推荐）/机器人服务<b>状态</b>（打印..记录视频..）/维护列表<b>/utm referrals</b></i>\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/parse - 显示所有用户\n/utm - 显示 utm referrals\n/link - 创建一个推荐 /utm 链接",
-    'ar': "👥 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>استبدال الصوت / التلسكوبات بالصوت <b>/ الفيديو</b> (* يوصى به إذا</i> قام المستخدمون <code>premium</code> <i>بتعيين مثل هذا الحظر) / <b>حالات</b> خدمة الروبوت (طباعة .. تسجيلات فيديو ..) / الاحتفاظ بقائمة من <b>إحالات / utm</b></i>\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - كافة الأوامر\n/ parse - عرض كافة المستخدمين\n/ utm - عرض إحالات utm\n/ link - إنشاء ارتباط إحالة / utm",
+    'ru': "👥 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>замену голосовых/телескопов на <b>audio/video</b> (*рекомендуется, если premium-пользователи установили такой запрет)/сервисные <b>статусы</b> бота (печатает..записывает видео..)/ведение списка <b>/utm-рефералов</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/utm - вывести utm-рефералов\n/link - создать реферальную /utm ссылку",
+    'en': "👥 <b>Click</b> on ✅/☑️ to <b>enable/disable</b> <i>the replacement of voice/telescopes with <b>audio/video</b> (*recommended if</i> premium <i>users have set such a ban)/bot service <b>statuses</b> (prints..records video..)/maintaining a list of <b>/utm referrals</b></i>\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/parse - display all users\n/utm - display utm referrals\n/link - create a referral /utm link",
+    'es': "👥 <b>Haga clic</b> en ✅/☑️ para <b>habilitar/deshabilitar</b> <i>el reemplazo de voz/telescopios con <b>audio/video</b> (*recomendado si</i> los usuarios premium <i>han establecido dicha prohibición)/ <b>estados</b> de servicio de bot (imprime... graba video...)/mantiene una lista de <b>/utm referencias</b></i>\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/parse - mostrar todos los usuarios\n/utm - mostrar referencias utm\n/link - crear un enlace de referencia /utm",
+    'fr': "👥 <b>Cliquez</b> sur ✅/☑️ pour <b>activer/désactiver</b> <i>le remplacement de la voix/des télescopes par <b>l&#x27;audio/la vidéo</b> (*recommandé si</i> les utilisateurs premium <i>ont défini une telle interdiction)/ <b>les statuts</b> du service de bot (imprime..enregistre la vidéo..)/maintient une liste de <b>/références utm</b></i>\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/parse - afficher tous les utilisateurs\n/utm - afficher les références utm\n/lien - créer une référence /lien utm",
+    'zh': "👥<b>点击</b>✅/☑️<b>启用/禁用</b><i>用音频<b>/视频</b>替换语音/望远镜（*如果</i>premium<i>用户设置了此类禁令，则推荐）/机器人服务<b>状态</b>（打印..记录视频..）/维护列表<b>/utm referrals</b></i>\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/parse - 显示所有用户\n/utm - 显示 utm referrals\n/link - 创建一个推荐 /utm 链接",
+    'ar': "👥 <b>انقر</b> فوق ✅ / ☑️ <b>لتمكين / تعطيل</b> <i>استبدال الصوت / التلسكوبات بالصوت <b>/ الفيديو</b> (* يوصى به إذا</i> قام المستخدمون premium <i>بتعيين مثل هذا الحظر) / <b>حالات</b> خدمة الروبوت (طباعة .. تسجيلات فيديو ..) / الاحتفاظ بقائمة من <b>إحالات / utm</b></i>\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - كافة الأوامر\n/ parse - عرض كافة المستخدمين\n/ utm - عرض إحالات utm\n/ link - إنشاء ارتباط إحالة / utm",
 }
 l_cuser_restricted_on = {
     'ru': "✅☑Вкл audio/video замена",
     'en': "✅☑Includes audio/video replacement",
     'es': "✅☑Incluye reemplazo de audio/video",
     'fr': "✅☑Comprend le remplacement audio/vidéo",
     'zh': "✅☑包括音频/视频替换",
@@ -6992,52 +7000,52 @@
     'en': "👩🏽‍💻 <b>@{0}-bot</b> off\n\n/on - enable bot",
     'es': "👩🏽‍💻 <b>@{0}-bot</b> apagado\n\n/encendido - habilitar bot",
     'fr': "👩🏽‍💻 <b>@{0}-bot</b> off\n\n/on - activer le bot",
     'zh': "👩🏽‍💻 <b>@{0}-bot</b> off\n\n/on - 启用机器人",
     'ar': "👩🏽‍💻 <b>@ {0} -bot</b> off\n\n/ on - قم بتمكين الروبوت",
 }
 l_cuser_utm = {
-    'ru': "👥 <b>Готово!</b> <b>/utm-список</b> реферальных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Вывести</b> рефералов конкретного пользователя можно командой:\n<code>/utm id</code> или <code>/utm @username</code>\n\n👩🏽‍💻 <b>Текущее</b> число utm-рефералов: <u>{1}</u>",
-    'en': "👥 <b>Done!</b> <b>/utm-list</b> of referral users of @{0}-bot\n\n👩🏽‍💻 You can <b>display</b> referrals of a specific user with the command:\n<code>/utm id</code> or <code>/utm @username</code>\n\n👩🏽‍💻 <b>Current</b> number of utm-referrals : <u>{1}</u>",
-    'es': "👥 <b>Listo!</b> <b>/utm-lista</b> de usuarios de referencia de @{0}-bot\n\n👩🏽‍💻 Puede <b>mostrar</b> referencias de un usuario específico con el comando:\n<code>/utm id</code> o <code>/utm @username</code>\n\n👩🏽 ‍💻 Número <b>actual</b> de referencias utm: <u>{1}</u>",
-    'fr': "👥 <b>C&#x27;est fait !</b> <b>/utm-list</b> des utilisateurs référents de @{0}-bot\n\n👩🏽‍💻 Vous pouvez <b>afficher</b> les références d&#x27;un utilisateur spécifique avec la commande :\n<code>/utm id</code> ou <code>/utm @username</code>\n\n👩🏽 ‍💻 Nombre <b>actuel</b> de références utm : <u>{1}</u>",
-    'zh': "👥<b>完成！</b> <b>/utm-@{0}-bot 的推荐用户列表</b>\n\n👩🏽‍💻 您可以使用以下命令<b>显示</b>特定用户的推荐：\n<code>/utm id</code>或<code>/utm @username</code>\n\n👩🏽 ‍💻<b>当前</b>的 utm-referrals 数量： <u>{1}</u>",
-    'ar': "👥 <b>انتهى!</b> <b>/ utm-list</b> لمستخدمي الإحالة لـ @ {0} -bot\n\n👩🏽‍💻 يمكنك <b>عرض</b> إحالات مستخدم معين بالأمر:\n<code>/utm id</code> أو <code>/utm @username</code>\n\n👩🏽 ‍💻 العدد <b>الحالي</b> لإحالات UTM: <u>{1}</u>",
+    'ru': "👥 <b>Готово!</b> <b>/utm-список</b> реферальных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Вывести</b> рефералов конкретного пользователя можно командой:\n/utm id или /utm @username\n\n👩🏽‍💻 <b>Текущее</b> число utm-рефералов: <u>{1}</u>",
+    'en': "👥 <b>Done!</b> <b>/utm-list</b> of referral users of @{0}-bot\n\n👩🏽‍💻 You can <b>display</b> referrals of a specific user with the command:\n/utm id or /utm @username\n\n👩🏽‍💻 <b>Current</b> number of utm-referrals : <u>{1}</u>",
+    'es': "👥 <b>Listo!</b> <b>/utm-lista</b> de usuarios de referencia de @{0}-bot\n\n👩🏽‍💻 Puede <b>mostrar</b> referencias de un usuario específico con el comando:\n/utm id o /utm @username\n\n👩🏽 ‍💻 Número <b>actual</b> de referencias utm: <u>{1}</u>",
+    'fr': "👥 <b>C&#x27;est fait !</b> <b>/utm-list</b> des utilisateurs référents de @{0}-bot\n\n👩🏽‍💻 Vous pouvez <b>afficher</b> les références d&#x27;un utilisateur spécifique avec la commande :\n/utm id ou /utm @username\n\n👩🏽 ‍💻 Nombre <b>actuel</b> de références utm : <u>{1}</u>",
+    'zh': "👥<b>完成！</b> <b>/utm-@{0}-bot 的推荐用户列表</b>\n\n👩🏽‍💻 您可以使用以下命令<b>显示</b>特定用户的推荐：\n/utm id或/utm @username\n\n👩🏽 ‍💻<b>当前</b>的 utm-referrals 数量： <u>{1}</u>",
+    'ar': "👥 <b>انتهى!</b> <b>/ utm-list</b> لمستخدمي الإحالة لـ @ {0} -bot\n\n👩🏽‍💻 يمكنك <b>عرض</b> إحالات مستخدم معين بالأمر:\n/utm id أو /utm @username\n\n👩🏽 ‍💻 العدد <b>الحالي</b> لإحالات UTM: <u>{1}</u>",
 }
 l_cuser_link_done = {
-    'ru': "👥 <b>Готово!</b> Реферальная /utm ссылка на @{0}-бота (размести ее на любой площадке, чтобы понимать, что пользователи перешли в бота с этой площадки):\n\n<code>{1}</code>",
-    'en': "👥 <b>Done!</b> Referral /utm link to the @{0}-bot (place it on any site to understand that users have switched to the bot from this site):\n\n<code>{1}</code>",
-    'es': "👥 <b>Listo!</b> Enlace de referencia /utm al @{0}-bot (colóquelo en cualquier sitio para comprender que los usuarios han cambiado al bot desde este sitio):\n\n<code>{1}</code>",
-    'fr': "👥 <b>C&#x27;est fait !</b> Lien de parrainage /utm vers le @{0}-bot (placez-le sur n&#x27;importe quel site pour comprendre que les utilisateurs sont passés au bot depuis ce site) :\n\n<code>{1}</code>",
-    'zh': "👥<b>完成！</b> @{0}-bot 的引荐 /utm 链接（将其放在任何站点上以了解用户已从该站点切换到该 bot）：\n\n<code>{1}</code>",
-    'ar': "👥 <b>انتهى!</b> رابط الإحالة / utm إلى @ {0} -bot (ضعه على أي موقع لفهم أن المستخدمين قد تحولوا إلى الروبوت من هذا الموقع):\n\n<code>{1}</code>",
+    'ru': "👥 <b>Готово!</b> Реферальная /utm ссылка на @{0}-бота (размести ее на любой площадке, чтобы понимать, что пользователи перешли в бота с этой площадки):\n\n{1}",
+    'en': "👥 <b>Done!</b> Referral /utm link to the @{0}-bot (place it on any site to understand that users have switched to the bot from this site):\n\n{1}",
+    'es': "👥 <b>Listo!</b> Enlace de referencia /utm al @{0}-bot (colóquelo en cualquier sitio para comprender que los usuarios han cambiado al bot desde este sitio):\n\n{1}",
+    'fr': "👥 <b>C&#x27;est fait !</b> Lien de parrainage /utm vers le @{0}-bot (placez-le sur n&#x27;importe quel site pour comprendre que les utilisateurs sont passés au bot depuis ce site) :\n\n{1}",
+    'zh': "👥<b>完成！</b> @{0}-bot 的引荐 /utm 链接（将其放在任何站点上以了解用户已从该站点切换到该 bot）：\n\n{1}",
+    'ar': "👥 <b>انتهى!</b> رابط الإحالة / utm إلى @ {0} -bot (ضعه على أي موقع لفهم أن المستخدمين قد تحولوا إلى الروبوت من هذا الموقع):\n\n{1}",
 }
 l_cuser_link_start = {
-    'ru': "👥 <b>Придумай</b> название для /utm ссылки (*после <code>?start=</code> может быть <u>любое</u> имя источника из цифр и/или латинских букв)\n\n👩🏽‍💻 <b>Например</b>, ссылки /utm-рефералов для отслеживания:\nhttps://t.me/{0}?start={1} - <i>реферальных пользователей</i> <code>{1}</code>-<i>пользователя</i>\nhttps://t.me/{0}?start=instagram - <i>пользователей из instagram</i>",
-    'en': "👥 <b>Think of</b> a name for the /utm link (*after <code>?start=</code> there can be <u>any</u> source name from numbers and/or Latin letters)\n\n👩🏽‍💻 <b>For example</b> , /utm referral links for tracking:\nhttps://t .me/{0}?start={1} - <i>referral users</i> <code>{1}</code> - <i>user</i>\nhttps://t.me/{0}?start=instagram - <i>users from instagram</i>",
-    'es': "👥 <b>Piense en</b> un nombre para el enlace /utm (*después de <code>?start=</code> puede haber <u>cualquier</u> nombre de fuente de números y/o letras latinas)\n\n👩🏽‍💻 <b>Por ejemplo</b> , enlaces de referencia /utm para el seguimiento:\nhttps ://t .me/{0}?start={1} - <i>usuarios de referencia</i> <code>{1}</code> - <i>usuario</i>\nhttps://t.me/{0}?start=instagram - <i>usuarios de instagram</i>",
-    'fr': "👥 <b>Pensez à</b> un nom pour le lien /utm (*après <code>?start=</code> il peut y avoir <u>n&#x27;importe quel</u> nom de source à partir de chiffres et/ou de lettres latines)\n\n👩🏽‍💻 <b>Par exemple</b> , les liens de référence /utm pour le suivi :\nhttps ://t .me/{0}?start={1} - <i>utilisateurs de référence</i> <code>{1}</code> - <i>utilisateur</i>\nhttps://t.me/{0}?start=instagram - <i>utilisateurs d&#x27;instagram</i>",
-    'zh': "👥<b>为 /utm 链接想</b>一个名字（*在<code>?start=</code>之后可以有<u>任何</u>来自数字和/或拉丁字母的源名称）\n\n👩🏽‍💻<b>例如</b>，用于跟踪的 /utm 推荐链接：\nhttps ://t .me/{0}?start={1} -<i>推荐用户</i><code>{1}</code> -<i>用户</i>\nhttps://t.me/{0}?start=instagram -<i>来自 instagram 的用户</i>",
-    'ar': "👥 <b>فكر في</b> اسم ارتباط / utm (* after <code>?start=</code> يمكن أن يكون هناك <u>أي</u> اسم مصدر من الأرقام و / أو الأحرف اللاتينية)\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، روابط الإحالة / utm للتتبع:\nhttps : // t .me / {0}؟ start = {1} - <i>المستخدمون المحالون</i> <code>{1}</code> - <i>المستخدم</i>\nhttps: //t.me/ {0}؟ start = instagram - <i>المستخدمون من instagram</i>",
+    'ru': "👥 <b>Придумай</b> название для /utm ссылки (*после ?start= может быть <u>любое</u> имя источника из цифр и/или латинских букв)\n\n👩🏽‍💻 <b>Например</b>, ссылки /utm-рефералов для отслеживания:\nhttps://t.me/{0}?start={1} - <i>реферальных пользователей</i> {1}-<i>пользователя</i>\nhttps://t.me/{0}?start=instagram - <i>пользователей из instagram</i>",
+    'en': "👥 <b>Think of</b> a name for the /utm link (*after ?start= there can be <u>any</u> source name from numbers and/or Latin letters)\n\n👩🏽‍💻 <b>For example</b> , /utm referral links for tracking:\nhttps://t .me/{0}?start={1} - <i>referral users</i> {1} - <i>user</i>\nhttps://t.me/{0}?start=instagram - <i>users from instagram</i>",
+    'es': "👥 <b>Piense en</b> un nombre para el enlace /utm (*después de ?start= puede haber <u>cualquier</u> nombre de fuente de números y/o letras latinas)\n\n👩🏽‍💻 <b>Por ejemplo</b> , enlaces de referencia /utm para el seguimiento:\nhttps ://t .me/{0}?start={1} - <i>usuarios de referencia</i> {1} - <i>usuario</i>\nhttps://t.me/{0}?start=instagram - <i>usuarios de instagram</i>",
+    'fr': "👥 <b>Pensez à</b> un nom pour le lien /utm (*après ?start= il peut y avoir <u>n&#x27;importe quel</u> nom de source à partir de chiffres et/ou de lettres latines)\n\n👩🏽‍💻 <b>Par exemple</b> , les liens de référence /utm pour le suivi :\nhttps ://t .me/{0}?start={1} - <i>utilisateurs de référence</i> {1} - <i>utilisateur</i>\nhttps://t.me/{0}?start=instagram - <i>utilisateurs d&#x27;instagram</i>",
+    'zh': "👥<b>为 /utm 链接想</b>一个名字（*在?start=之后可以有<u>任何</u>来自数字和/或拉丁字母的源名称）\n\n👩🏽‍💻<b>例如</b>，用于跟踪的 /utm 推荐链接：\nhttps ://t .me/{0}?start={1} -<i>推荐用户</i>{1} -<i>用户</i>\nhttps://t.me/{0}?start=instagram -<i>来自 instagram 的用户</i>",
+    'ar': "👥 <b>فكر في</b> اسم ارتباط / utm (* after ?start= يمكن أن يكون هناك <u>أي</u> اسم مصدر من الأرقام و / أو الأحرف اللاتينية)\n\n👩🏽‍💻 <b>على سبيل المثال</b> ، روابط الإحالة / utm للتتبع:\nhttps : // t .me / {0}؟ start = {1} - <i>المستخدمون المحالون</i> {1} - <i>المستخدم</i>\nhttps: //t.me/ {0}؟ start = instagram - <i>المستخدمون من instagram</i>",
 }
 l_promo_done = {
-    'ru': "👩🏽‍💻 <b>Готово!</b>\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n<code>{0}</code>\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n<code>/promo 0</code>",
-    'en': "👩🏽‍💻 <b>Done!</b>\n\n👩🏽‍💻 <i>Current /promo code</i> :\n<code>{0}</code>\n👩🏽‍💻 <i>Delete /promo code</i> :\n<code>/promo 0</code>",
-    'es': "👩🏽‍💻 <b>Listo!</b>\n\n👩🏽‍💻 <i>Código /promocional actual</i> :\n<code>{0}</code>\n👩🏽‍💻 <i>Eliminar código /promocional</i> :\n<code>/promo 0</code>",
-    'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 <i>Code /promo actuel</i> :\n<code>{0}</code>\n👩🏽‍💻 <i>Supprimer le code /promo</i> :\n<code>/promo 0</code>",
-    'zh': "👩🏽‍💻<b>完成！</b>\n\n👩🏽‍💻<i>当前/促销代码</i>：\n<code>{0}</code>\n👩🏽‍💻<i>删除/促销代码</i>：\n<code>/promo 0</code>",
-    'ar': "👩🏽‍💻 <b>انتهى!</b>\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n<code>{0}</code>\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n<code>/promo 0</code>",
+    'ru': "👩🏽‍💻 <b>Готово!</b>\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{0}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n/promo 0",
+    'en': "👩🏽‍💻 <b>Done!</b>\n\n👩🏽‍💻 <i>Current /promo code</i> :\n{0}\n👩🏽‍💻 <i>Delete /promo code</i> :\n/promo 0",
+    'es': "👩🏽‍💻 <b>Listo!</b>\n\n👩🏽‍💻 <i>Código /promocional actual</i> :\n{0}\n👩🏽‍💻 <i>Eliminar código /promocional</i> :\n/promo 0",
+    'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b>\n\n👩🏽‍💻 <i>Code /promo actuel</i> :\n{0}\n👩🏽‍💻 <i>Supprimer le code /promo</i> :\n/promo 0",
+    'zh': "👩🏽‍💻<b>完成！</b>\n\n👩🏽‍💻<i>当前/促销代码</i>：\n{0}\n👩🏽‍💻<i>删除/促销代码</i>：\n/promo 0",
+    'ar': "👩🏽‍💻 <b>انتهى!</b>\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n{0}\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n/promo 0",
 }
 l_promo_start = {
-    'ru': "👩🏽‍💻 <b>Введи</b> /promo-код для @{0}-бота:\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n<code>{1}</code>\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n<code>/promo 0</code>",
-    'en': "👩🏽‍💻 <b>Enter</b> /promo code for @{0}-bot:\n\n👩🏽‍💻 <i>Current /promo code</i> :\n<code>{1}</code>\n👩🏽‍💻 <i>Delete /promo code</i> :\n<code>/promo 0</code>",
-    'es': "👩🏽‍💻 <b>Ingresa el</b> /código de promoción para @{0}-bot:\n\n👩🏽‍💻 <i>Actual /código de promoción</i> :\n<code>{1}</code>\n👩🏽‍💻 <i>Eliminar /código de promoción</i> :\n<code>/promo 0</code>",
-    'fr': "👩🏽‍💻 <b>Entrez</b> /code promo pour @{0}-bot :\n\n👩🏽‍💻 <i>Code /code promo actuel</i> :\n<code>{1}</code>\n👩🏽‍💻 <i>Supprimer /code promo</i> :\n<code>/promo 0</code>",
-    'zh': "👩🏽‍💻<b>输入</b>@{0}-bot 的 /promo 代码：\n\n👩🏽‍💻<i>当前 /promo 代码</i>：\n<code>{1}</code>\n👩🏽‍💻<i>删除 /promo 代码</i>：\n<code>/promo 0</code>",
-    'ar': "👩🏽‍💻 <b>أدخل</b> / الرمز الترويجي لـ @ {0} -bot:\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n<code>{1}</code>\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n<code>/promo 0</code>",
+    'ru': "👩🏽‍💻 <b>Введи</b> /promo-код для @{0}-бота:\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n{1}\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n/promo 0",
+    'en': "👩🏽‍💻 <b>Enter</b> /promo code for @{0}-bot:\n\n👩🏽‍💻 <i>Current /promo code</i> :\n{1}\n👩🏽‍💻 <i>Delete /promo code</i> :\n/promo 0",
+    'es': "👩🏽‍💻 <b>Ingresa el</b> /código de promoción para @{0}-bot:\n\n👩🏽‍💻 <i>Actual /código de promoción</i> :\n{1}\n👩🏽‍💻 <i>Eliminar /código de promoción</i> :\n/promo 0",
+    'fr': "👩🏽‍💻 <b>Entrez</b> /code promo pour @{0}-bot :\n\n👩🏽‍💻 <i>Code /code promo actuel</i> :\n{1}\n👩🏽‍💻 <i>Supprimer /code promo</i> :\n/promo 0",
+    'zh': "👩🏽‍💻<b>输入</b>@{0}-bot 的 /promo 代码：\n\n👩🏽‍💻<i>当前 /promo 代码</i>：\n{1}\n👩🏽‍💻<i>删除 /promo 代码</i>：\n/promo 0",
+    'ar': "👩🏽‍💻 <b>أدخل</b> / الرمز الترويجي لـ @ {0} -bot:\n\n👩🏽‍💻 <i>الرمز الحالي / الترويجي</i> :\n{1}\n👩🏽‍💻 <i>حذف / الرمز الترويجي</i> :\n/promo 0",
 }
 # endregion
 
 
 # region cadmin_
 l_cadmin_text2 = {
     'ru': "👮🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>доступ добавленных администраторов к функционалу <b>[💬 Оповещения]</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей",
@@ -7052,36 +7060,36 @@
     'en': "👮🏽 <b>Done!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/admin - add/remove administrator\n/parse - display all users\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{2}/10</u>",
     'es': "👮🏽 <b>Listo!</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/admin - agregar/eliminar administrador\n/parse - mostrar todos los usuarios\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{2}/10</u>",
     'fr': "👮🏽 <b>C&#x27;est fait !</b> /admin-list @{0}-bot :\n\n{1}\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/admin - ajouter/supprimer un administrateur\n/parse - afficher tous les utilisateurs\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{2}/10</u>",
     'zh': "👮🏽<b>完成！</b> /admin-list @{0}-bot:\n\n{1}\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/admin - 添加/删除管理员\n/parse - 显示所有用户\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{2}/10</u>",
     'ar': "👮🏽 <b>انتهى!</b> / admin-list @ {0} -bot:\n\n{1}\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ admin - إضافة / إزالة المسؤول\n/ parse - عرض جميع المستخدمين\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{2} / 10</u>",
 }
 l_cadmin_add = {
-    'ru': "👮🏽 <b>Введи</b> до 10 <code>id</code>-пользователей через пробельные символы или разделители, чтобы добавить их в /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
-    'en': "👮🏽 <b>Enter</b> user <code>id</code> separated by spaces or separators to add them to /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
-    'es': "👮🏽 <b>Ingrese</b> <code>id</code> de usuario separados por espacios o separadores para agregarlos a /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
-    'fr': "👮🏽 <b>Entrez</b> <code>id</code> des utilisateurs séparés par des espaces ou des séparateurs pour les ajouter à /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
-    'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户<code>id</code> ，以将其添加到 /admin-list\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{0}</u>",
-    'ar': "👮🏽 <b>أدخل</b> <code>id</code> المستخدمين مفصولة بمسافات أو فواصل لإضافتها إلى / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
+    'ru': "👮🏽 <b>Введи</b> до 10 id-пользователей через пробельные символы или разделители, чтобы добавить их в /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
+    'en': "👮🏽 <b>Enter</b> user id separated by spaces or separators to add them to /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
+    'es': "👮🏽 <b>Ingrese</b> id de usuario separados por espacios o separadores para agregarlos a /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
+    'fr': "👮🏽 <b>Entrez</b> id des utilisateurs séparés par des espaces ou des séparateurs pour les ajouter à /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
+    'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户id ，以将其添加到 /admin-list\n\n👩🏽‍💻<b>当前</b>管理员人数： <u>{0}</u>",
+    'ar': "👮🏽 <b>أدخل</b> id المستخدمين مفصولة بمسافات أو فواصل لإضافتها إلى / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
 }
 l_cadmin_remove = {
-    'ru': "👮🏽 <b>Введи</b> <code>id</code> пользователей через пробельные символы или разделители, чтобы удалить их из /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
-    'en': "👮🏽 <b>Enter</b> user <code>id</code> separated by spaces or separators to remove them from /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
-    'es': "👮🏽 <b>Ingrese</b> <code>id</code> de usuario separados por espacios o separadores para eliminarlos de /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
-    'fr': "👮🏽 <b>Entrez</b> <code>id</code> d&#x27;utilisateur séparés par des espaces ou des séparateurs pour les supprimer de /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
-    'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户<code>id</code> ，以将其从 /admin-list 中删除\n\n👩🏽‍💻<b>当前</b>管理员数量： <u>{0}</u>",
-    'ar': "👮🏽 <b>أدخل</b> <code>id</code> المستخدمين مفصولة بمسافات أو فواصل لإزالتها من / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
+    'ru': "👮🏽 <b>Введи</b> id пользователей через пробельные символы или разделители, чтобы удалить их из /admin-список\n\n👩🏽‍💻 <b>Текущее</b> число администраторов: <u>{0}</u>",
+    'en': "👮🏽 <b>Enter</b> user id separated by spaces or separators to remove them from /admin-list\n\n👩🏽‍💻 <b>Current</b> number of admins: <u>{0}</u>",
+    'es': "👮🏽 <b>Ingrese</b> id de usuario separados por espacios o separadores para eliminarlos de /admin-list\n\n👩🏽‍💻 Número <b>actual</b> de administradores: <u>{0}</u>",
+    'fr': "👮🏽 <b>Entrez</b> id d&#x27;utilisateur séparés par des espaces ou des séparateurs pour les supprimer de /admin-list\n\n👩🏽‍💻 Nombre <b>actuel</b> d&#x27;administrateurs : <u>{0}</u>",
+    'zh': "👮🏽<b>输入</b>以空格或分隔符分隔的用户id ，以将其从 /admin-list 中删除\n\n👩🏽‍💻<b>当前</b>管理员数量： <u>{0}</u>",
+    'ar': "👮🏽 <b>أدخل</b> id المستخدمين مفصولة بمسافات أو فواصل لإزالتها من / قائمة المشرف\n\n👩🏽‍💻 العدد <b>الحالي</b> للمسؤولين: <u>{0}</u>",
 }
 l_parse_text = {
-    'ru': "👩🏽‍💻 <b>Готово!</b> Парсинг пользователей (<u>{0}</u>) @{1}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n<code>/parse premium</code> - вывести premium-пользователей\n<code>/parse admin</code> - вывести admin-пользователей\n<code>/parse utm</code> - вывести utm-рефералов\n",
-    'en': "👩🏽‍💻 <b>Done!</b> Parsing users ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/parse - print all users\n<code>/parse premium</code> - print premium users\n<code>/parse admin</code> - display admin users\n<code>/parse utm</code> - display utm referrals\n",
-    'es': "👩🏽‍💻 <b>Listo!</b> Analizando usuarios ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/parse - imprimir todos los usuarios\n<code>/parse premium</code> - imprimir usuarios premium\n<code>/parse admin</code> - mostrar usuarios administradores\n<code>/parse utm</code> - mostrar referencias utm\n",
-    'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b> Analyse des utilisateurs ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/parse - imprimer tous les utilisateurs\n<code>/parse premium</code> - imprimer les utilisateurs premium\n<code>/parse admin</code> - affiche les utilisateurs administrateurs\n<code>/parse utm</code> - affiche les références utm\n",
-    'zh': "👩🏽‍💻<b>完成！</b>解析用户（ <u>{0}</u> ）@{1}-bot\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/parse - 打印所有用户\n<code>/parse premium</code> - 打印高级用户\n<code>/parse admin</code> - 显示管理员用户\n<code>/parse utm</code> - 显示 utm 引用\n",
-    'ar': "👩🏽‍💻 <b>انتهى!</b> تحليل المستخدمين ( <u>{0}</u> ) @ {1} -bot\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ تحليل - طباعة جميع المستخدمين\n<code>/parse premium</code> - طباعة المستخدمين المتميزين\n<code>/parse admin</code> - عرض المستخدمين المسؤولين\n<code>/parse utm</code> - عرض إحالات UTM\n",
+    'ru': "👩🏽‍💻 <b>Готово!</b> Парсинг пользователей (<u>{0}</u>) @{1}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/parse premium - вывести premium-пользователей\n/parse admin - вывести admin-пользователей\n/parse utm - вывести utm-рефералов\n",
+    'en': "👩🏽‍💻 <b>Done!</b> Parsing users ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commands</b> :\n/cmd - all commands\n/parse - print all users\n/parse premium - print premium users\n/parse admin - display admin users\n/parse utm - display utm referrals\n",
+    'es': "👩🏽‍💻 <b>Listo!</b> Analizando usuarios ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Comandos</b> :\n/cmd - todos los comandos\n/parse - imprimir todos los usuarios\n/parse premium - imprimir usuarios premium\n/parse admin - mostrar usuarios administradores\n/parse utm - mostrar referencias utm\n",
+    'fr': "👩🏽‍💻 <b>C&#x27;est fait !</b> Analyse des utilisateurs ( <u>{0}</u> ) @{1}-bot\n\n👩🏽‍💻 <b>Commandes</b> :\n/cmd - toutes les commandes\n/parse - imprimer tous les utilisateurs\n/parse premium - imprimer les utilisateurs premium\n/parse admin - affiche les utilisateurs administrateurs\n/parse utm - affiche les références utm\n",
+    'zh': "👩🏽‍💻<b>完成！</b>解析用户（ <u>{0}</u> ）@{1}-bot\n\n👩🏽‍💻<b>命令</b>：\n/cmd - 所有命令\n/parse - 打印所有用户\n/parse premium - 打印高级用户\n/parse admin - 显示管理员用户\n/parse utm - 显示 utm 引用\n",
+    'ar': "👩🏽‍💻 <b>انتهى!</b> تحليل المستخدمين ( <u>{0}</u> ) @ {1} -bot\n\n👩🏽‍💻 <b>الأوامر</b> :\n/ cmd - جميع الأوامر\n/ تحليل - طباعة جميع المستخدمين\n/parse premium - طباعة المستخدمين المتميزين\n/parse admin - عرض المستخدمين المسؤولين\n/parse utm - عرض إحالات UTM\n",
 }
 # endregion
 # endregion
 
 
 # region client
 l_idea = {
@@ -7089,56 +7097,56 @@
     'en': "💡 Idea!",
     'es': "💡 Idea!",
     'fr': "💡 Idée !",
     'zh': "💡 想法！",
     'ar': "💡 فكرة!",
 }
 l_have_read = {
-    'ru': "👩🏽‍💻 <code>{0}</code> прочитал сообщение",
-    'en': "👩🏽‍💻 <code>{0}</code> read the message",
-    'es': "👩🏽‍💻 <code>{0}</code> lee el mensaje",
-    'fr': "👩🏽‍💻 <code>{0}</code> lire le message",
-    'zh': "👩🏽‍💻 <code>{0}</code>阅读消息",
-    'ar': "👩🏽‍💻 <code>{0}</code> اقرأ الرسالة",
+    'ru': "👩🏽‍💻 {0} прочитал сообщение",
+    'en': "👩🏽‍💻 {0} read the message",
+    'es': "👩🏽‍💻 {0} lee el mensaje",
+    'fr': "👩🏽‍💻 {0} lire le message",
+    'zh': "👩🏽‍💻 {0}阅读消息",
+    'ar': "👩🏽‍💻 {0} اقرأ الرسالة",
 }
 l_telegraph_title = {
     'ru': "📰 Telegraph блог",
     'en': "📰 Telegraph Blog",
     'es': "📰Blog de telégrafo",
     'fr': "📰 Blog télégraphique",
     'zh': "📰 电报博客",
     'ar': "📰 مدونة التلغراف",
 }
 l_telegraph_blog = {
-    'ru': "<figure><img src='{0}'/><figcaption>Фото профиля: @{1}</figcaption></figure><blockquote>Лэндинг-блог для продвижения в <i>Telegram</i></blockquote>👩🏽‍💻 <b>бот:</b> {2}<br>[<b>id</b>=<code>{3}</code>]<br><b>Био:</b> {4}<br><aside>Описание</aside>{5}",
-    'en': "Profile photo: @{1}Landing blog for promotion in <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = <code>{3}</code>] <b>Bio:</b> {4}Description{5}",
-    'es': "Foto de perfil: @{1}Blog de aterrizaje para promoción en <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = <code>{3}</code>] <b>Bio:</b> {4}Descripción{5}",
-    'fr': "Photo de profil : @{1}Blog d'atterrissage pour la promotion dans <i>Telegram</i> 👩🏽‍💻 <b>bot :</b> {2}[<b>id</b> = <code>{3}</code>] <b>Bio :</b> {4}Description{5}",
-    'zh': "个人资料照片：@{1}登陆博客以在<i>Telegram</i> 👩🏽‍💻<b>机器人中进行推广：</b> {2}[<b>id</b> = <code>{3}</code>]<b>简介：</b> {4}说明{5}",
-    'ar': "صورة الملف الشخصي: @ {1} مدونة الهبوط للترويج في <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2} [<b>id</b> = <code>{3}</code>] <b>السيرة الذاتية:</b> {4} الوصف {5}",
+    'ru': "<figure><img src='{0}'/><figcaption>Фото профиля: @{1}</figcaption></figure><blockquote>Лэндинг-блог для продвижения в <i>Telegram</i></blockquote>👩🏽‍💻 <b>бот:</b> {2}<br>[<b>id</b>={3}]<br><b>Био:</b> {4}<br><aside>Описание</aside>{5}",
+    'en': "Profile photo: @{1}Landing blog for promotion in <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Description{5}",
+    'es': "Foto de perfil: @{1}Blog de aterrizaje para promoción en <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2}[<b>id</b> = {3}] <b>Bio:</b> {4}Descripción{5}",
+    'fr': "Photo de profil : @{1}Blog d'atterrissage pour la promotion dans <i>Telegram</i> 👩🏽‍💻 <b>bot :</b> {2}[<b>id</b> = {3}] <b>Bio :</b> {4}Description{5}",
+    'zh': "个人资料照片：@{1}登陆博客以在<i>Telegram</i> 👩🏽‍💻<b>机器人中进行推广：</b> {2}[<b>id</b> = {3}]<b>简介：</b> {4}说明{5}",
+    'ar': "صورة الملف الشخصي: @ {1} مدونة الهبوط للترويج في <i>Telegram</i> 👩🏽‍💻 <b>bot:</b> {2} [<b>id</b> = {3}] <b>السيرة الذاتية:</b> {4} الوصف {5}",
 }
 # endregion
 
 
 # region extra bot
 l_show_admin_panel_md = {
     'ru': "*👩🏽‍💻 Создание и редактирование блога*\n\n👩🏽‍💻 Вы зашли как *Администратор* и можете создавать и редактировать блоги, но не удалять их\n\n¹ Авторизация по ссылке в браузере:\n`{0}`\n\n² Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
     'en': "*👩🏽‍💻 Creating and editing a blog*\n\n👩🏽‍💻 You are logged in as *Administrator* and can create and edit blogs, but not delete them\n\n¹ Authorization via link in browser:\n`{0 }`\n\n² Go (within 10 seconds) to the desired link to edit the post (click to copy):\n\n",
     'es': "*👩🏽‍💻 Crear y editar un blog*\n\n👩🏽‍💻 Ha iniciado sesión como *Administrador* y puede crear y editar blogs, pero no eliminarlos\n\n¹ Autorización a través de un enlace en el navegador:\n`{0 }`\n\n² Vaya (dentro de 10 segundos) al enlace deseado para editar la publicación (haga clic para copiar):\n\n",
     'fr': "*👩🏽‍💻 Créer et modifier un blog*\n\n👩🏽‍💻 Vous êtes connecté en tant qu'*administrateur* et vous pouvez créer et modifier des blogs, mais pas les supprimer\n\n¹ Autorisation via un lien dans le navigateur :\n`{0 }`\n\n² Accédez (dans les 10 secondes) au lien souhaité pour modifier le message (cliquez pour copier) :\n\n",
     'zh': "*👩🏽‍💻 创建和编辑博客*\n\n👩🏽‍💻 您以*管理员*身份登录，可以创建和编辑博客，但不能删除它们\n\n¹ 通过浏览器中的链接授权：\n`{0 }`\n\n²（在 10 秒内）转到所需的链接以编辑帖子（单击以复制）：\n\n",
     'ar': "* 👩🏽‍💻 إنشاء مدونة وتحريرها *\n\n👩🏽‍💻 تم تسجيل دخولك بصفتك * المسؤول * ويمكنك إنشاء المدونات وتحريرها ، ولكن لا يمكنك حذفها\n\n¹ التفويض عبر الارتباط في المستعرض:\n'{0}`\n\n² انتقل (في غضون 10 ثوانٍ) إلى الرابط المطلوب لتعديل المشاركة (انقر للنسخ):\n\n",
 }
 l_show_admin_panel_html = {
-    'ru': "<b>👩🏽‍💻 Создание и редактирование блога</b>\n\n👩🏽‍💻 Вы зашли как <b>Администратор</b> и можете создавать и редактировать блоги, но не удалять их\n\n1. Авторизация по ссылке в браузере:\n<code>{0}</code>\n\n2. Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
-    'en': "<b>👩🏽‍💻 Creating and editing a blog</b>\n\n👩🏽‍💻 You are logged in as <b>Administrator</b> and can create and edit blogs, but not delete them\n\n1. Authorization by link in browser:\n<code>{0}</code>\n\n2. Go (within 10 seconds) to the desired link to edit the publication (click to copy):\n\n",
-    'es': "<b>👩🏽‍💻 Crear y editar un blog</b>\n\n👩🏽‍💻 Ha iniciado sesión como <b>Administrador</b> y puede crear y editar blogs, pero no borrarlos\n\n1. Autorización por enlace en el navegador:\n<code>{0}</code>\n\n2. Vaya (dentro de 10 segundos) al enlace deseado para editar la publicación (haga clic para copiar):\n\n",
-    'fr': "<b>👩🏽‍💻 Créer et modifier un blog</b>\n\n👩🏽‍💻 Vous êtes connecté en tant <b>qu&#x27;administrateur</b> et pouvez créer et modifier des blogs, mais pas les supprimer\n\n1. Autorisation par lien dans le navigateur :\n<code>{0}</code>\n\n2. Accédez (dans les 10 secondes) au lien souhaité pour modifier la publication (cliquez pour copier) :\n\n",
-    'zh': "<b>👩🏽‍💻 创建和编辑博客</b>\n\n👩🏽‍💻 您以<b>管理员</b>身份登录，可以创建和编辑博客，但不能删除它们\n\n1.通过浏览器中的链接授权：\n<code>{0}</code>\n\n2.转到（在 10 秒内）所需的链接以编辑发布（单击以复制）：\n\n",
-    'ar': "<b>👩🏽‍💻 إنشاء مدونة وتحريرها</b>\n\n👩🏽‍💻 قمت بتسجيل الدخول <b>كمسؤول</b> ويمكنك إنشاء المدونات وتحريرها ، ولكن لا يمكنك حذفها\n\n1. التفويض بالارتباط في المتصفح:\n<code>{0}</code>\n\n2. انتقل (في غضون 10 ثوانٍ) إلى الارتباط المطلوب لتحرير المنشور (انقر للنسخ):\n\n",
+    'ru': "<b>👩🏽‍💻 Создание и редактирование блога</b>\n\n👩🏽‍💻 Вы зашли как <b>Администратор</b> и можете создавать и редактировать блоги, но не удалять их\n\n1. Авторизация по ссылке в браузере:\n{0}\n\n2. Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
+    'en': "<b>👩🏽‍💻 Creating and editing a blog</b>\n\n👩🏽‍💻 You are logged in as <b>Administrator</b> and can create and edit blogs, but not delete them\n\n1. Authorization by link in browser:\n{0}\n\n2. Go (within 10 seconds) to the desired link to edit the publication (click to copy):\n\n",
+    'es': "<b>👩🏽‍💻 Crear y editar un blog</b>\n\n👩🏽‍💻 Ha iniciado sesión como <b>Administrador</b> y puede crear y editar blogs, pero no borrarlos\n\n1. Autorización por enlace en el navegador:\n{0}\n\n2. Vaya (dentro de 10 segundos) al enlace deseado para editar la publicación (haga clic para copiar):\n\n",
+    'fr': "<b>👩🏽‍💻 Créer et modifier un blog</b>\n\n👩🏽‍💻 Vous êtes connecté en tant <b>qu&#x27;administrateur</b> et pouvez créer et modifier des blogs, mais pas les supprimer\n\n1. Autorisation par lien dans le navigateur :\n{0}\n\n2. Accédez (dans les 10 secondes) au lien souhaité pour modifier la publication (cliquez pour copier) :\n\n",
+    'zh': "<b>👩🏽‍💻 创建和编辑博客</b>\n\n👩🏽‍💻 您以<b>管理员</b>身份登录，可以创建和编辑博客，但不能删除它们\n\n1.通过浏览器中的链接授权：\n{0}\n\n2.转到（在 10 秒内）所需的链接以编辑发布（单击以复制）：\n\n",
+    'ar': "<b>👩🏽‍💻 إنشاء مدونة وتحريرها</b>\n\n👩🏽‍💻 قمت بتسجيل الدخول <b>كمسؤول</b> ويمكنك إنشاء المدونات وتحريرها ، ولكن لا يمكنك حذفها\n\n1. التفويض بالارتباط في المتصفح:\n{0}\n\n2. انتقل (في غضون 10 ثوانٍ) إلى الارتباط المطلوب لتحرير المنشور (انقر للنسخ):\n\n",
 }
 l_show_admin_panel_create = {
     'ru': "🆕 Создать",
     'en': "🆕 Create",
     'es': "🆕 Crear",
     'fr': "🆕 Créer",
     'zh': "🆕 创建",
@@ -7656,15 +7664,15 @@
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 # endregion
 
 
 # region FereyTargetBot
 l_subscribe_target = {
-    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [Донат на баланс]:\n▪️возможность сделать рассылку в боте\n\n👩🏽‍💻 /balance",
-    'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
+    'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️рассылка/приглашения\n▪️редактирование чаевых\n(<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
+    'en': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>:\n\n¹ [<b>Все боты</b> и проекты (-<u>5</u>%)]\n² [<b>Донат</b> на баланс]:\n▪️возможность сделать рассылку по всем ботам\n▪️измените значение чаевых (<i>чтобы указать точную сумму</i>)\n\n👩🏽‍💻 /balance",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
     'ar': "👩🏽‍💻 <b>اشترك للحصول على</b> <i>اشتراك</i> شهري\n\n¹ في @ {0} -bot [{1} ₽]\n▪️ بلا إعلانات\n▪️ مهام إبداعية\n² اشترك في <u>جميع</u> برامج التتبُّع [{2} ₽]",
 }
 # endregion
```

### Comparing `yeref-0.1.91/yeref/yeref.py` & `yeref-0.1.92/yeref/yeref.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,15 @@
     '6236215930',
 
     '5754810063',
     '5491025132',
     '5360564451',
     '6281795468',
 ]
-channel_library_ru = -1001484489131
-channel_library_en = -1001481302043
+
 ferey_channel_europe = -1001471122743
 ferey_channel_en = -1001833151619
 ferey_channel_es = -1001988190840
 ferey_channel_fr = -1001942773697
 ferey_channel_ar = -1001913015662
 ferey_channel_zh = -1001904073819
 
@@ -118,14 +117,38 @@
 ferey_address = "Estônia, Tāllin, Mäepealse, 2/1"
 ferey_title = "Ferey Inc."
 payment_link = 'http://bagazhznaniy.ru/wp-content/uploads/2014/03/zhivaya-priroda.jpg'
 whatsup = f'https://api.whatsapp.com/send?phone={phone_number}&text=%D0%94%D0%BE%D0%B1%D1%80%D1%8B%D0%B9%20%D0%B4%D0' \
           f'%B5%D0%BD%D1%8C%2C%20%D1%8F%20%D0%BF%D0%BE%20%D0%BF%D0%BE%D0%B2%D0%BE%D0%B4%D1%83%20%D0%92%D0%B0%D1%88%D0' \
           f'%B5%D0%B3%D0%BE%20%D0%BF%D1%80%D0%BE%D0%B4%D1%83%D0%BA%D1%82%D0%B0!'
 
+placeholder = '/content'
+donate_bot_rub = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4Njc=-0xXD'
+donate_bot_eur = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NjY=-0xXD'
+donate_user_rub = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NTU=-0xXD'
+donate_user_eur = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NzE=-0xXD'
+donate_group_rub = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NTE=-0xXD'
+donate_group_eur = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4Njk=-0xXD'
+donate_channel_rub = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NTM=-0xXD'
+donate_channel_eur = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NzA=-0xXD'
+donate_ai_rub = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NDk=-0xXD'
+donate_ai_eur = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4Njg=-0xXD'
+donate_find_rub = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NjQ=-0xXD'
+donate_find_eur = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NzQ=-0xXD'
+donate_post_rub = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NTc=-0xXD'
+donate_post_eur = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NzI=-0xXD'
+donate_media_rub = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NTk=-0xXD'
+donate_media_eur = 'https://t.me/donate?start=Y2hhcml0eV9pbnZvaWNlX3JlcXVlc3QtMzE4NzM=-0xXD'
+channel_library_ru_link = 'https://t.me/+f-0AbTALTOg4ODBk'
+channel_library_en_link = 'https://t.me/+CHIMCacxEZw4YjA8'
+donate_deposit_rub = 'https://t.me/ferey_channel_europe/32'
+donate_deposit_eur = 'https://t.me/ferey_channel_europe/44'
+channel_library_ru = -1001484489131
+channel_library_en = -1001481302043
+
 ferey_thumb = 'https://telegra.ph/file/bf7d8c073cdfa91b6d624.jpg'
 ferey_theme = 'https://t.me/addtheme/lzbKZktZjqv5VDdY'
 ferey_wp = 'https://t.me/bg/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 ferey_set = 'https://t.me/addstickers/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 ferey_emoji = 'https://t.me/addemoji/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 reactions_ = ['👍', '❤', '🔥', '🥰', '👏', '😁', '🤔', '🤯', '😱', '🤬', '😢', '🎉', '🤩', '🙏',
               '👌', '🕊', '🤡', '🥱', '🥴', '😍', '🐳', '❤\u200d🔥', '🌚', '🌭', '💯', '🤣', '⚡', '🍌', '🏆',
```

