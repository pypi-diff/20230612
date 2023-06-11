# Comparing `tmp/plex-tvdb-alt-orderer-0.2.2.tar.gz` & `tmp/plex-tvdb-alt-orderer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-tvdb-alt-orderer-0.2.2.tar", last modified: Sun Jun 11 05:57:00 2023, max compression
+gzip compressed data, was "plex-tvdb-alt-orderer-0.2.3.tar", last modified: Sun Jun 11 22:32:39 2023, max compression
```

## Comparing `plex-tvdb-alt-orderer-0.2.2.tar` & `plex-tvdb-alt-orderer-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 05:57:00.155590 plex-tvdb-alt-orderer-0.2.2/
--rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     5870 2023-06-11 05:57:00.155590 plex-tvdb-alt-orderer-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     5250 2023-06-09 21:39:05.000000 plex-tvdb-alt-orderer-0.2.2/README.md
--rw-rw-rw-   0        0        0      877 2023-06-11 05:56:23.000000 plex-tvdb-alt-orderer-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 05:57:00.155590 plex-tvdb-alt-orderer-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 05:57:00.124971 plex-tvdb-alt-orderer-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 05:57:00.128968 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer/
--rw-rw-rw-   0        0        0     8143 2023-06-11 05:50:24.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer/main.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:57:00.154590 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/
--rw-rw-rw-   0        0        0     5870 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-11 05:57:00.000000 plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-11 22:32:39.129782 plex-tvdb-alt-orderer-0.2.3/
+-rw-rw-rw-   0        0        0     1073 2023-06-07 23:45:38.000000 plex-tvdb-alt-orderer-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     5870 2023-06-11 22:32:39.128791 plex-tvdb-alt-orderer-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5250 2023-06-09 21:39:05.000000 plex-tvdb-alt-orderer-0.2.3/README.md
+-rw-rw-rw-   0        0        0      877 2023-06-11 20:47:36.000000 plex-tvdb-alt-orderer-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-11 22:32:39.129782 plex-tvdb-alt-orderer-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-11 22:32:39.084179 plex-tvdb-alt-orderer-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-11 22:32:39.105180 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer/
+-rw-rw-rw-   0        0        0     7869 2023-06-11 22:20:51.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer/main.py
+drwxrwxrwx   0        0        0        0 2023-06-11 22:32:39.126783 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/
+-rw-rw-rw-   0        0        0     5870 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       70 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-11 22:32:39.000000 plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/top_level.txt
```

### Comparing `plex-tvdb-alt-orderer-0.2.2/LICENSE` & `plex-tvdb-alt-orderer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-tvdb-alt-orderer-0.2.2/PKG-INFO` & `plex-tvdb-alt-orderer-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-tvdb-alt-orderer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A utility that applies alternate TVDB orders to Plex.
 Author: bpoxy
 Project-URL: Homepage, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Project-URL: Bug Tracker, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plex-tvdb-alt-orderer-0.2.2/README.md` & `plex-tvdb-alt-orderer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `plex-tvdb-alt-orderer-0.2.2/pyproject.toml` & `plex-tvdb-alt-orderer-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "plex-tvdb-alt-orderer"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="bpoxy" },
 ]
 description = "A utility that applies alternate TVDB orders to Plex."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["click", "inquirer", "plexapi", "progress", "termcolor", "tvdb_v4_official", "validators"]
```

### Comparing `plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer/main.py` & `plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     tvdb = TVDB(apikey="5f119e31-f9c5-4f0c-b1c3-064b3225e7d9", pin=tvdb_pin)
     tvdb_id = next(match.group("id") for match in [re.match(r"tvdb://(?P<id>\d+)", guid.id) for guid in plex_show.guids] if match)
     tvdb_season_type = get_tvdb_season_type(tvdb, tvdb_id, tvdb_order_name)
     tvdb_episodes = tvdb.get_series_episodes(tvdb_id, season_type=tvdb_season_type, lang="eng")["episodes"]
     
     update_plex(season, plex_episodes, tvdb_episodes)
 
-def dict_to_tuple(dict: dict):
-    return [(key, value) for key, value in dict.items()]
+def dict_prompt(dict: dict, description: str):
+    return dict[inquirer.prompt([inquirer.List("answer", message=f"Select {description}", choices=dict.keys())])["answer"]]
 
 def error_exit(text: str):
     print(colored(text, "red"))
     exit()
 
 def get_plex_section(plex_server: PlexServer, section_name: str) -> ShowSection:
     sections = list(filter(lambda s: s.TYPE == "show", plex_server.library.sections()))
@@ -61,15 +61,15 @@
         return sections_dict.get(section_name, None) or error_exit(f"Your Plex server doesn't contain a TV show library named '{section_name}'.")
 
     if len(sections) == 0:
         error_exit(f"Your Plex server doesn't contain a TV show library.")
     elif len(sections) == 1:
         return sections[0]
     else:
-        return inquirer.prompt([inquirer.List("section", message="Select the library to update", choices=dict_to_tuple(sections_dict))])["section"]
+        return dict_prompt(sections_dict, "the library to update")
 
 def get_plex_server(plex_password: str, plex_server_identifier: str, plex_token: str, plex_user: str) -> PlexServer:
     plex_server_identifier = text_prompt_if_unspecified(plex_server_identifier, "your Plex server name (user/password authentication) or URL (token authentication)")
 
     if validators.url(plex_server_identifier):
         return PlexServer(plex_server_identifier, text_prompt_if_unspecified(plex_token, "your Plex token"))
 
@@ -83,33 +83,32 @@
     shows = section.search(title=show_name)
 
     if len(shows) == 0:
          error_exit(f"Your TV show library doesn't contain a show with name '{show_name}'.")
     elif len(shows) == 1:
         return shows[0]
     else:
-        shows_dict = {s.title: s for s in shows}
-        return inquirer.prompt([inquirer.List("show", message="Select the show to update", choices=dict_to_tuple(shows_dict))])["show"]
+        return dict_prompt({s.title: s for s in shows}, "the show to update")
 
 def get_tvdb_season_type(tvdb: TVDB, tvdb_id: int, order_name: str) -> str:
     season_types = tvdb.get_season_types(tvdb_id)
     season_types_dict = {s["name"]: s["type"] for s in season_types}
 
     if order_name:
         return season_types_dict.get(order_name, None) or error_exit(f"TVDB doesn't define an order with name '{order_name}'.")
 
-    return inquirer.prompt([inquirer.List("season_type", message="Select the order to apply", choices=dict_to_tuple(season_types_dict))])["season_type"]
+    return dict_prompt(season_types_dict, "the order to apply")
 
 def text_prompt_if_unspecified(value: str, description: str):
     return value or inquirer.prompt([inquirer.Text("answer", message=f"Enter {description}")])["answer"]
 
 def update_plex(season: int, plex_episodes: list[Episode], tvdb_episodes: list[dict]):
     plex_seasons_dict = {"Entire Series": UPDATE_ENTIRE_SERIES}
     plex_seasons_dict.update({f"Season {e.parentIndex}": e.parentIndex for e in plex_episodes})
-    season = season or inquirer.prompt([inquirer.List("season", message="Select the season to update", choices=dict_to_tuple(plex_seasons_dict))])["season"]
+    season = season or dict_prompt(plex_seasons_dict, "the season to update")
 
     if season != UPDATE_ENTIRE_SERIES:
         plex_episodes = list(filter(lambda e: e.parentIndex == season, plex_episodes))
         tvdb_episodes = list(filter(lambda e: e["seasonNumber"] == season, tvdb_episodes))
 
     tvdb_episode_dict = {}
```

### Comparing `plex-tvdb-alt-orderer-0.2.2/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO` & `plex-tvdb-alt-orderer-0.2.3/src/plex_tvdb_alt_orderer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-tvdb-alt-orderer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A utility that applies alternate TVDB orders to Plex.
 Author: bpoxy
 Project-URL: Homepage, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Project-URL: Bug Tracker, https://github.com/bpoxy/plex-tvdb-alt-orderer
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

