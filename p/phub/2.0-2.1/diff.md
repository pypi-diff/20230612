# Comparing `tmp/phub-2.0.tar.gz` & `tmp/phub-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-2.0.tar", last modified: Mon Jun 12 16:51:18 2023, max compression
+gzip compressed data, was "phub-2.1.tar", last modified: Mon Jun 12 19:20:20 2023, max compression
```

## Comparing `phub-2.0.tar` & `phub-2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:18.135808 phub-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 16:51:04.000000 phub-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 16:51:18.135808 phub-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-12 16:51:04.000000 phub-2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 16:51:04.000000 phub-2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 16:51:18.139808 phub-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 16:51:04.000000 phub-2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:18.131808 phub-2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:18.135808 phub-2.0/src/phub/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-12 16:51:04.000000 phub-2.0/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-06-12 16:51:04.000000 phub-2.0/src/phub/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-12 16:51:04.000000 phub-2.0/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-12 16:51:04.000000 phub-2.0/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 16:51:04.000000 phub-2.0/src/phub/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-12 16:51:04.000000 phub-2.0/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:18.135808 phub-2.0/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 16:51:18.000000 phub-2.0/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:20:20.017775 phub-2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 19:20:05.000000 phub-2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 19:20:20.017775 phub-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-12 19:20:05.000000 phub-2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 19:20:05.000000 phub-2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 19:20:20.017775 phub-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 19:20:05.000000 phub-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:20:20.013775 phub-2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:20:20.017775 phub-2.1/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-12 19:20:05.000000 phub-2.1/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17067 2023-06-12 19:20:05.000000 phub-2.1/src/phub/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-12 19:20:05.000000 phub-2.1/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-12 19:20:05.000000 phub-2.1/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 19:20:05.000000 phub-2.1/src/phub/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-12 19:20:05.000000 phub-2.1/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:20:20.017775 phub-2.1/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/top_level.txt
```

### Comparing `phub-2.0/LICENSE` & `phub-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-2.0/PKG-INFO` & `phub-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.0
+Version: 2.1
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

### Comparing `phub-2.0/README.md` & `phub-2.1/README.md`

 * *Files identical despite different names*

### Comparing `phub-2.0/setup.cfg` & `phub-2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phub
-version = 2.0
+version = 2.1
 description = An API for PornHub
 author = Egsagon
 author_email = egsagon12@gmail.com
 url = https://github.com/Egsagon/PHUB/
 license = GPLv3
 license_file = LICENSE
 long_description = file: README.md
```

### Comparing `phub-2.0/src/phub/__init__.py` & `phub-2.1/src/phub/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 
 # Debugging controls
 from sys import stdout
 from io import TextIOBase
 
 def debug(boolean: bool, file: TextIOBase = stdout) -> None:
     '''
-    Whether to log everything to stdout.
+    #### Whether to log everything to stdout. ####
+    ----------------------------------------------
     
-    Arguments
-        boolean: Value to set debug to.
-        file (optional): File to output logs to.
+    Arguments:
+    - `boolean`          -- Value to set debug to.
+    - `file` (=`stdout`) -- File to output logs to.
     '''
     
     utils.DEBUG = boolean
     utils.DEBUG_FILE = file
     
     utils.log('init_', 'Switching logging to', boolean)
 
-# EOF
+# EOF
```

### Comparing `phub-2.0/src/phub/classes.py` & `phub-2.1/src/phub/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
                 quality: utils.Quality,
                 process: bool = True) -> str | list[str]:
         '''
         #### Get the raw M3U url for a certain quality. ####
         ----------------------------------------------------
         
         Arguments:
-        - `quality` -- The desired quality as an object.
+        - `quality`           -- The desired quality as an object.
         - `process` (=`True`) -- Whether to parse the file.
         
         ----------------------------------------------------
         Returns a list of segment URLs if `process` is `True`,
         else the URL of the M3U file.
         '''
         
@@ -417,16 +417,16 @@
     
     def __init__(self, client: Client, url: str, corrector: Callable = None) -> None:
         '''
         #### Generate a new video iterator object. ####
         -----------------------------------------------
         
         Arguments:
-        - `client` -- The client to base from.
-        - `url` -- The URL of the page that contains the playlist.
+        - `client`              -- The client to base from.
+        - `url`                 -- The URL of the page that contains the playlist.
         - `corrector` (=`None`) -- Function to call to correct parsing in edge cases.
         '''
         
         log('viter', 'Initialising new Video Iterator', level = 6)
         
         self.client = client
         self.url = (url + '?&'['?' in url] + 'page=').replace(consts.ROOT, '')
@@ -552,8 +552,8 @@
         except IndexError:
             log('viter', 'Reached end of generation')
             raise StopIteration
         
         self.index += 1
         return result
         
-# EOF
+# EOF
```

### Comparing `phub-2.0/src/phub/consts.py` & `phub-2.1/src/phub/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,20 +37,20 @@
     # Searching regexes
     video_search_counter = re.compile( r'showingCounter\">.*? (\d+) +</',                                  re.DOTALL ).findall   # Extract video counter from research responses
     video_likes          = re.compile( r'span class=\"votes(Up|Down)\" data-rating.*?>(.*?)<'                        ).findall   # Extract likes from a video page
     video_interactions   = re.compile( r'interactionStatistic\": \[(.*?)\]',                               re.DOTALL ).findall   # Find interaction stats from a video page
     video_flashvar       = re.compile( r'var (flashvars_\d*) = ({.*});\n'                                            ).findall   # Video obfuscation script part
     video_datalayer      = re.compile( r'window\.dataLayer\.push\(({.*?})\);',                             re.DOTALL ).findall   # Get video advanced datalayer
     video_channel        = re.compile( r'href=\"(.*?)\" data-event=\"Video Underplayer\".*?bolded\">(.*?)<'          ).findall   # Get video author if channel
-    video_model          = re.compile( r'n class=\"usernameBadgesWrapper.*? href=\"(.*?)\"  class=\"bolded\">(.*?)<' ).findall # Get video author if model
+    video_model          = re.compile( r'n class=\"usernameBadgesWrapper.*? href=\"(.*?)\"  class=\"bolded\">(.*?)<' ).findall   # Get video author if model
     
     # Substraction regexes
     sub_js_comments      = re.compile( r'\/\*.*?\*\/'                                                                ).sub       # Remove js comments
     sub_root             = re.compile( r'https://.{2,3}\.pornhub\.com/'                                              ).sub       # Substitue URL roots
     
     # Match regexes
     is_valid_video_url   = re.compile( r'https://.{2,3}\.pornhub\.com/view_video\.php\?viewkey=[a-z\d]{13,15}'       ).fullmatch # Verify video URL validity
     
     # Old
     # video_model          = re.compile( r'<span class=\"usernameBadgesWrapper\"><a rel=\"\" href=\"(.*?)\"  class=\"bolded\">(.*?)</a>').findall # Get video author if model
 
-# EOF
+# EOF
```

### Comparing `phub-2.0/src/phub/core.py` & `phub-2.1/src/phub/core.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -100,16 +100,16 @@
         -----------------------------------
         
         Arguments
         - `username`   (=`None`) -- Account to connect to username.
         - `password`   (=`None`) -- Account to connect to password.
         - `session`    (=`None`) -- Recovery requests session.
         - `autologin` (=`False`) -- Whether to login after initialisation.
-        -----------------------------------
         
+        -----------------------------------
         Returns a `Client` object.
         '''
         
         # Initialise session
         self.session = session or requests.Session()
         self.session.cookies.set('accessAgeDisclaimerPH', '1')
         
@@ -142,16 +142,16 @@
         '''
         #### Generate a new client from credentials. ####
         -------------------------------------------------
         
         Arguments:
         - `data` -- Dictionnary, JSON file or JSON string to get
                     username and password from.
-        -------------------------------------------------
         
+        -------------------------------------------------
         Returns a `Client` object.
         '''
         
         if isinstance(data, TextIOWrapper):
             data = data.read()
         
         if isinstance(data, str):
@@ -305,8 +305,8 @@
         Returns a `VideoIterator` object.
         '''
         
         log('client', 'Opening new search query:', query, level = 6)
         url = consts.ROOT + 'video/search?search=' + query
         return classes.VideoIterator(self.client, url)
 
-# EOF
+# EOF
```

### Comparing `phub-2.0/src/phub/parser.py` & `phub-2.1/src/phub/parser.py`

 * *Files identical despite different names*

### Comparing `phub-2.0/src/phub/utils.py` & `phub-2.1/src/phub/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 def pathify(string: str) -> str:
     '''
     #### Set a string to be path safe. ####
     ---------------------------------------
     
     Arguments:
-    - ``string` -- The string.
+    - `string` -- The string.
     
     ---------------------------------------
     Returns a path-safe string.
     '''
     
     return ''.join(c for c in string if c in ascii_letters + '- _()')
 
@@ -270,8 +270,8 @@
 
 
 # Define presets as objects
 Quality.BEST = Quality(Quality.BEST)
 Quality.MIDDLE = Quality(Quality.MIDDLE)
 Quality.WORST = Quality(Quality.WORST)
 
-# EOF
+# EOF
```

### Comparing `phub-2.0/src/phub.egg-info/PKG-INFO` & `phub-2.1/src/phub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.0
+Version: 2.1
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

