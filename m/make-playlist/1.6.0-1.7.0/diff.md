# Comparing `tmp/make_playlist-1.6.0.tar.gz` & `tmp/make_playlist-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "make_playlist-1.6.0.tar", last modified: Tue Mar  7 10:35:26 2023, max compression
+gzip compressed data, was "make_playlist-1.7.0.tar", last modified: Mon Jun 12 13:19:28 2023, max compression
```

## Comparing `make_playlist-1.6.0.tar` & `make_playlist-1.7.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-03-07 10:35:26.437184 make_playlist-1.6.0/
--rwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    34916 2022-09-09 08:34:13.000000 make_playlist-1.6.0/LICENSE.md
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       19 2022-09-09 08:34:13.000000 make_playlist-1.6.0/MANIFEST.in
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8604 2023-03-07 10:35:26.436184 make_playlist-1.6.0/PKG-INFO
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     7795 2023-03-07 10:26:59.000000 make_playlist-1.6.0/README.md
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1089 2023-03-07 10:26:59.000000 make_playlist-1.6.0/__info__.py
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-03-07 10:35:26.436184 make_playlist-1.6.0/make_playlist.egg-info/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8604 2023-03-07 10:35:26.000000 make_playlist-1.6.0/make_playlist.egg-info/PKG-INFO
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      249 2023-03-07 10:35:26.000000 make_playlist-1.6.0/make_playlist.egg-info/SOURCES.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        1 2023-03-07 10:35:26.000000 make_playlist-1.6.0/make_playlist.egg-info/dependency_links.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       61 2023-03-07 10:35:26.000000 make_playlist-1.6.0/make_playlist.egg-info/entry_points.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        5 2023-03-07 10:35:26.000000 make_playlist-1.6.0/make_playlist.egg-info/top_level.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    13861 2023-03-07 10:26:59.000000 make_playlist-1.6.0/mkpl.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       38 2023-03-07 10:35:26.437184 make_playlist-1.6.0/setup.cfg
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1992 2022-09-09 09:02:21.000000 make_playlist-1.6.0/setup.py
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-06-12 13:19:28.626745 make_playlist-1.7.0/
+-rwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    34916 2022-09-09 08:34:13.000000 make_playlist-1.7.0/LICENSE.md
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       19 2022-09-09 08:34:13.000000 make_playlist-1.7.0/MANIFEST.in
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8842 2023-06-12 13:19:28.626745 make_playlist-1.7.0/PKG-INFO
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8033 2023-06-12 13:15:40.000000 make_playlist-1.7.0/README.md
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1089 2023-06-12 13:15:40.000000 make_playlist-1.7.0/__info__.py
+drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-06-12 13:19:28.625744 make_playlist-1.7.0/make_playlist.egg-info/
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8842 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/PKG-INFO
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      285 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/SOURCES.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        1 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/dependency_links.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       61 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/entry_points.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        8 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/requires.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        5 2023-06-12 13:19:28.000000 make_playlist-1.7.0/make_playlist.egg-info/top_level.txt
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    15935 2023-06-12 13:15:40.000000 make_playlist-1.7.0/mkpl.py
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       38 2023-06-12 13:19:28.626745 make_playlist-1.7.0/setup.cfg
+-rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2026 2023-06-12 13:15:40.000000 make_playlist-1.7.0/setup.py
```

### Comparing `make_playlist-1.6.0/LICENSE.md` & `make_playlist-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `make_playlist-1.6.0/PKG-INFO` & `make_playlist-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make_playlist
-Version: 1.6.0
+Version: 1.7.0
 Summary: Make M3U format playlist from command line
 Home-page: https://github.com/MatteoGuadrini/mkpl
 Author: Matteo Guadrini
 Author-email: matteo.guadrini@hotmail.it
 Maintainer: Matteo Guadrini
 Maintainer-email: matteo.guadrini@hotmail.it
 License: GNU General Public License v3.0
@@ -16,15 +16,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ``make_playlist``: Make playlist command line tool
 
-``mkpl`` is a _command line tool_ for create playlist file (**M3U format**).
+``mkpl`` is a _command line tool_ to create playlist files (**[M3U](https://en.wikipedia.org/wiki/M3U) format**).
 
 ## Installation
 
 To install ``mkpl``, see here:
 
 ```console
 $ pip install make_playlist               # for python enviroment
@@ -36,37 +36,38 @@
 $ python setup.py install                 # for others
 ```
 
 ## Command arguments
 
 ``mkpl`` have many command line arguments. They are explained in this table:
 
-| short | long           | description                                   | args                      |
-|-------|----------------|-----------------------------------------------|---------------------------|
-| -d    | --directories  | Directories that contains multimedia file     | Path of directories       |
-| -e    | --exclude-dirs | Exclude directory paths                       | Path of directories       |
-| -i    | --include      | Include other file format                     | Format of file. ex. mp3   |
-| -p    | --pattern      | Regular expression inclusion pattern          | Regular expression string |
-| -f    | --format       | Select only a file format                     | Format of file. ex. mp3   |
-| -s    | --size         | Start size in bytes                           | Bytes number              |
-| -m    | --max-tracks   | Maximum number of tracks                      | Number                    |
-| -t    | --title        | Playlist title                                | Title string              |
-| -g    | --encoding     | Text encoding                                 | UTF-8,ASCII,UNICODE       |
-| -I    | --image        | Playlist image                                | Image path                |
-| -l    | --link         | Add remote file links                         | Links                     |
-| -r    | --recursive    | Recursive search                              |                           |
-| -a    | --absolute     | Absolute file name                            |                           |
-| -s    | --shuffle      | Casual order                                  |                           |
-| -u    | --unique       | The same files are not placed in the playlist |                           |
-| -c    | --append       | Continue playlist instead of override it      |                           |
-| -w    | --windows      | Windows style folder separator                |                           |
-| -v    | --verbose      | Enable verbosity (debug mode)                 |                           |
-| -S    | --split        | Split playlist by directories                 |                           |
-| -o    | --orderby-name | Order playlist files by name                  |                           |
-| -O    | --orderby-date | Order playlist files by creation date         |                           |
+| short | long            | description                                   | args                      |
+|-------|-----------------|-----------------------------------------------|---------------------------|
+| -d    | --directories   | Directories that contains multimedia file     | Path of directories       |
+| -e    | --exclude-dirs  | Exclude directory paths                       | Path of directories       |
+| -i    | --include       | Include other file format                     | Format of file. ex. mp3   |
+| -p    | --pattern       | Regular expression inclusion pattern          | Regular expression string |
+| -f    | --format        | Select only a file format                     | Format of file. ex. mp3   |
+| -s    | --size          | Start size in bytes                           | Bytes number              |
+| -m    | --max-tracks    | Maximum number of tracks                      | Number                    |
+| -t    | --title         | Playlist title                                | Title string              |
+| -g    | --encoding      | Text encoding                                 | UTF-8,ASCII,UNICODE       |
+| -I    | --image         | Playlist image                                | Image path                |
+| -l    | --link          | Add remote file links                         | Links                     |
+| -r    | --recursive     | Recursive search                              |                           |
+| -a    | --absolute      | Absolute file name                            |                           |
+| -s    | --shuffle       | Casual order                                  |                           |
+| -u    | --unique        | The same files are not placed in the playlist |                           |
+| -c    | --append        | Continue playlist instead of override it      |                           |
+| -w    | --windows       | Windows style folder separator                |                           |
+| -v    | --verbose       | Enable verbosity (debug mode)                 |                           |
+| -S    | --split         | Split playlist by directories                 |                           |
+| -o    | --orderby-name  | Order playlist files by name                  |                           |
+| -O    | --orderby-date  | Order playlist files by creation date         |                           |
+| -T    | --orderby-track | Order playlist files by track                 |                           |
 
 ## Examples
 
 1. Create a playlist for one music album:
 
     ```bash
     cd myalbum
@@ -157,19 +158,20 @@
     my_music.m3u
     folder1.m3u
     folder2.m3u
     folder3.m3u
     ...
     ```
 
-15. Sort playlist files by name (`-o`) or by creation date (`-O`):
+15. Sort playlist files by name (`-o`), by creation date (`-O`) or by track number (`-T`):
 
     ```bash
     mkpl -d "new_collection" -r "my music.m3u" -o
     mkpl -d "new_collection" -r "my music.m3u" -O
+    mkpl -d "new_collection" -r "my music.m3u" -T
     ```
 
 ## Use it like Python module
 
 `mkpl` can also be used as a Python module to customize your scripts.
 
 ```python
```

### Comparing `make_playlist-1.6.0/README.md` & `make_playlist-1.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ``make_playlist``: Make playlist command line tool
 
-``mkpl`` is a _command line tool_ for create playlist file (**M3U format**).
+``mkpl`` is a _command line tool_ to create playlist files (**[M3U](https://en.wikipedia.org/wiki/M3U) format**).
 
 ## Installation
 
 To install ``mkpl``, see here:
 
 ```console
 $ pip install make_playlist               # for python enviroment
@@ -16,37 +16,38 @@
 $ python setup.py install                 # for others
 ```
 
 ## Command arguments
 
 ``mkpl`` have many command line arguments. They are explained in this table:
 
-| short | long           | description                                   | args                      |
-|-------|----------------|-----------------------------------------------|---------------------------|
-| -d    | --directories  | Directories that contains multimedia file     | Path of directories       |
-| -e    | --exclude-dirs | Exclude directory paths                       | Path of directories       |
-| -i    | --include      | Include other file format                     | Format of file. ex. mp3   |
-| -p    | --pattern      | Regular expression inclusion pattern          | Regular expression string |
-| -f    | --format       | Select only a file format                     | Format of file. ex. mp3   |
-| -s    | --size         | Start size in bytes                           | Bytes number              |
-| -m    | --max-tracks   | Maximum number of tracks                      | Number                    |
-| -t    | --title        | Playlist title                                | Title string              |
-| -g    | --encoding     | Text encoding                                 | UTF-8,ASCII,UNICODE       |
-| -I    | --image        | Playlist image                                | Image path                |
-| -l    | --link         | Add remote file links                         | Links                     |
-| -r    | --recursive    | Recursive search                              |                           |
-| -a    | --absolute     | Absolute file name                            |                           |
-| -s    | --shuffle      | Casual order                                  |                           |
-| -u    | --unique       | The same files are not placed in the playlist |                           |
-| -c    | --append       | Continue playlist instead of override it      |                           |
-| -w    | --windows      | Windows style folder separator                |                           |
-| -v    | --verbose      | Enable verbosity (debug mode)                 |                           |
-| -S    | --split        | Split playlist by directories                 |                           |
-| -o    | --orderby-name | Order playlist files by name                  |                           |
-| -O    | --orderby-date | Order playlist files by creation date         |                           |
+| short | long            | description                                   | args                      |
+|-------|-----------------|-----------------------------------------------|---------------------------|
+| -d    | --directories   | Directories that contains multimedia file     | Path of directories       |
+| -e    | --exclude-dirs  | Exclude directory paths                       | Path of directories       |
+| -i    | --include       | Include other file format                     | Format of file. ex. mp3   |
+| -p    | --pattern       | Regular expression inclusion pattern          | Regular expression string |
+| -f    | --format        | Select only a file format                     | Format of file. ex. mp3   |
+| -s    | --size          | Start size in bytes                           | Bytes number              |
+| -m    | --max-tracks    | Maximum number of tracks                      | Number                    |
+| -t    | --title         | Playlist title                                | Title string              |
+| -g    | --encoding      | Text encoding                                 | UTF-8,ASCII,UNICODE       |
+| -I    | --image         | Playlist image                                | Image path                |
+| -l    | --link          | Add remote file links                         | Links                     |
+| -r    | --recursive     | Recursive search                              |                           |
+| -a    | --absolute      | Absolute file name                            |                           |
+| -s    | --shuffle       | Casual order                                  |                           |
+| -u    | --unique        | The same files are not placed in the playlist |                           |
+| -c    | --append        | Continue playlist instead of override it      |                           |
+| -w    | --windows       | Windows style folder separator                |                           |
+| -v    | --verbose       | Enable verbosity (debug mode)                 |                           |
+| -S    | --split         | Split playlist by directories                 |                           |
+| -o    | --orderby-name  | Order playlist files by name                  |                           |
+| -O    | --orderby-date  | Order playlist files by creation date         |                           |
+| -T    | --orderby-track | Order playlist files by track                 |                           |
 
 ## Examples
 
 1. Create a playlist for one music album:
 
     ```bash
     cd myalbum
@@ -137,19 +138,20 @@
     my_music.m3u
     folder1.m3u
     folder2.m3u
     folder3.m3u
     ...
     ```
 
-15. Sort playlist files by name (`-o`) or by creation date (`-O`):
+15. Sort playlist files by name (`-o`), by creation date (`-O`) or by track number (`-T`):
 
     ```bash
     mkpl -d "new_collection" -r "my music.m3u" -o
     mkpl -d "new_collection" -r "my music.m3u" -O
+    mkpl -d "new_collection" -r "my music.m3u" -T
     ```
 
 ## Use it like Python module
 
 `mkpl` can also be used as a Python module to customize your scripts.
 
 ```python
```

### Comparing `make_playlist-1.6.0/__info__.py` & `make_playlist-1.7.0/__info__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # __info__ -- mkpl
 #
-#     Copyright (C) 2022 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -18,11 +18,11 @@
 #     GNU General Public License for more details.
 #
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Information variable used by modules on this package."""
 
-__version__ = '1.6.0'
+__version__ = '1.7.0'
 __author__ = 'Matteo Guadrini'
 __email__ = 'matteo.guadrini@hotmail.it'
 __homepage__ = 'https://github.com/MatteoGuadrini/mkpl'
```

### Comparing `make_playlist-1.6.0/make_playlist.egg-info/PKG-INFO` & `make_playlist-1.7.0/make_playlist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: make-playlist
-Version: 1.6.0
+Version: 1.7.0
 Summary: Make M3U format playlist from command line
 Home-page: https://github.com/MatteoGuadrini/mkpl
 Author: Matteo Guadrini
 Author-email: matteo.guadrini@hotmail.it
 Maintainer: Matteo Guadrini
 Maintainer-email: matteo.guadrini@hotmail.it
 License: GNU General Public License v3.0
@@ -16,15 +16,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ``make_playlist``: Make playlist command line tool
 
-``mkpl`` is a _command line tool_ for create playlist file (**M3U format**).
+``mkpl`` is a _command line tool_ to create playlist files (**[M3U](https://en.wikipedia.org/wiki/M3U) format**).
 
 ## Installation
 
 To install ``mkpl``, see here:
 
 ```console
 $ pip install make_playlist               # for python enviroment
@@ -36,37 +36,38 @@
 $ python setup.py install                 # for others
 ```
 
 ## Command arguments
 
 ``mkpl`` have many command line arguments. They are explained in this table:
 
-| short | long           | description                                   | args                      |
-|-------|----------------|-----------------------------------------------|---------------------------|
-| -d    | --directories  | Directories that contains multimedia file     | Path of directories       |
-| -e    | --exclude-dirs | Exclude directory paths                       | Path of directories       |
-| -i    | --include      | Include other file format                     | Format of file. ex. mp3   |
-| -p    | --pattern      | Regular expression inclusion pattern          | Regular expression string |
-| -f    | --format       | Select only a file format                     | Format of file. ex. mp3   |
-| -s    | --size         | Start size in bytes                           | Bytes number              |
-| -m    | --max-tracks   | Maximum number of tracks                      | Number                    |
-| -t    | --title        | Playlist title                                | Title string              |
-| -g    | --encoding     | Text encoding                                 | UTF-8,ASCII,UNICODE       |
-| -I    | --image        | Playlist image                                | Image path                |
-| -l    | --link         | Add remote file links                         | Links                     |
-| -r    | --recursive    | Recursive search                              |                           |
-| -a    | --absolute     | Absolute file name                            |                           |
-| -s    | --shuffle      | Casual order                                  |                           |
-| -u    | --unique       | The same files are not placed in the playlist |                           |
-| -c    | --append       | Continue playlist instead of override it      |                           |
-| -w    | --windows      | Windows style folder separator                |                           |
-| -v    | --verbose      | Enable verbosity (debug mode)                 |                           |
-| -S    | --split        | Split playlist by directories                 |                           |
-| -o    | --orderby-name | Order playlist files by name                  |                           |
-| -O    | --orderby-date | Order playlist files by creation date         |                           |
+| short | long            | description                                   | args                      |
+|-------|-----------------|-----------------------------------------------|---------------------------|
+| -d    | --directories   | Directories that contains multimedia file     | Path of directories       |
+| -e    | --exclude-dirs  | Exclude directory paths                       | Path of directories       |
+| -i    | --include       | Include other file format                     | Format of file. ex. mp3   |
+| -p    | --pattern       | Regular expression inclusion pattern          | Regular expression string |
+| -f    | --format        | Select only a file format                     | Format of file. ex. mp3   |
+| -s    | --size          | Start size in bytes                           | Bytes number              |
+| -m    | --max-tracks    | Maximum number of tracks                      | Number                    |
+| -t    | --title         | Playlist title                                | Title string              |
+| -g    | --encoding      | Text encoding                                 | UTF-8,ASCII,UNICODE       |
+| -I    | --image         | Playlist image                                | Image path                |
+| -l    | --link          | Add remote file links                         | Links                     |
+| -r    | --recursive     | Recursive search                              |                           |
+| -a    | --absolute      | Absolute file name                            |                           |
+| -s    | --shuffle       | Casual order                                  |                           |
+| -u    | --unique        | The same files are not placed in the playlist |                           |
+| -c    | --append        | Continue playlist instead of override it      |                           |
+| -w    | --windows       | Windows style folder separator                |                           |
+| -v    | --verbose       | Enable verbosity (debug mode)                 |                           |
+| -S    | --split         | Split playlist by directories                 |                           |
+| -o    | --orderby-name  | Order playlist files by name                  |                           |
+| -O    | --orderby-date  | Order playlist files by creation date         |                           |
+| -T    | --orderby-track | Order playlist files by track                 |                           |
 
 ## Examples
 
 1. Create a playlist for one music album:
 
     ```bash
     cd myalbum
@@ -157,19 +158,20 @@
     my_music.m3u
     folder1.m3u
     folder2.m3u
     folder3.m3u
     ...
     ```
 
-15. Sort playlist files by name (`-o`) or by creation date (`-O`):
+15. Sort playlist files by name (`-o`), by creation date (`-O`) or by track number (`-T`):
 
     ```bash
     mkpl -d "new_collection" -r "my music.m3u" -o
     mkpl -d "new_collection" -r "my music.m3u" -O
+    mkpl -d "new_collection" -r "my music.m3u" -T
     ```
 
 ## Use it like Python module
 
 `mkpl` can also be used as a Python module to customize your scripts.
 
 ```python
```

### Comparing `make_playlist-1.6.0/mkpl.py` & `make_playlist-1.7.0/mkpl.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,263 +20,409 @@
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """mkpl module. This is command line utility for playlist creation."""
 
 # region imports
 import argparse
-from string import capwords
-from re import findall, sub
+import re
 from filecmp import cmp
+from os.path import basename, dirname, exists, getctime, getsize, isdir, join, normpath
 from pathlib import Path
 from random import shuffle
-from os.path import (join, exists, isdir, getsize, 
-                     normpath, basename, dirname, getctime)
+from re import sub
+from string import capwords
+
+from mutagen import File
 
 # endregion
 
 # region globals
-FILE_FORMAT = {'mp1', 'mp2', 'mp3', 'mp4', 'aac', 'ogg', 'wav', 'wma', 'm4a', 'aiff',
-               'avi', 'xvid', 'divx', 'mpeg', 'mpg', 'mov', 'wmv', 'flac', 'alac', 'opus'}
-__version__ = '1.6.0'
+AUDIO_FORMAT = {
+    "mp1",
+    "mp2",
+    "mp3",
+    "aac",
+    "ogg",
+    "wav",
+    "wma",
+    "m4a",
+    "aiff",
+    "flac",
+    "alac",
+    "opus",
+}
+VIDEO_FORMAT = {"mp4", "avi", "xvid", "divx", "mpeg", "mpg", "mov", "wmv"}
+FILE_FORMAT = AUDIO_FORMAT.union(VIDEO_FORMAT)
+__version__ = "1.7.0"
 
 
 # endregion
 
+
 # region functions
 def get_args():
     """Get command-line arguments"""
 
     global FILE_FORMAT
 
     parser = argparse.ArgumentParser(
         description="Command line tool to create media playlists in M3U format.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        epilog='See latest release from https://github.com/MatteoGuadrini/mkpl'
+        epilog="See latest release from https://github.com/MatteoGuadrini/mkpl",
     )
+    orderby_group = parser.add_mutually_exclusive_group()
 
     parser.add_argument("playlist", help="Playlist file", type=str)
     parser.add_argument("-v", "--verbose", help="Enable verbosity", action="store_true")
-    parser.add_argument("-V", "--version", help="Print version", action='version', version=__version__)
-    parser.add_argument("-d", "--directories", help="Directories that contains multimedia file",
-                        nargs=argparse.ONE_OR_MORE, default=['.'])
-    parser.add_argument("-e", "--exclude-dirs", help="Exclude directory paths", nargs=argparse.ONE_OR_MORE, default=[])
-    parser.add_argument("-i", "--include", help="Include other file format", nargs=argparse.ONE_OR_MORE,
-                        metavar='FORMAT')
-    parser.add_argument("-p", "--pattern", 
-                        help="Regular expression inclusion pattern", default='.*')
-    parser.add_argument("-f", "--format", help="Select only a file format", type=str, choices=FILE_FORMAT)
-    parser.add_argument("-z", "--size", help="Start size in bytes", type=int, 
-                        default=1, metavar='BYTES')
-    parser.add_argument("-m", "--max-tracks", help="Maximum number of tracks", 
-                        type=int, default=None, metavar='NUMBER')
+    parser.add_argument(
+        "-V", "--version", help="Print version", action="version", version=__version__
+    )
+    parser.add_argument(
+        "-d",
+        "--directories",
+        help="Directories that contains multimedia file",
+        nargs=argparse.ONE_OR_MORE,
+        default=["."],
+    )
+    parser.add_argument(
+        "-e",
+        "--exclude-dirs",
+        help="Exclude directory paths",
+        nargs=argparse.ONE_OR_MORE,
+        default=[],
+    )
+    parser.add_argument(
+        "-i",
+        "--include",
+        help="Include other file format",
+        nargs=argparse.ONE_OR_MORE,
+        metavar="FORMAT",
+    )
+    parser.add_argument(
+        "-p", "--pattern", help="Regular expression inclusion pattern", default=".*"
+    )
+    parser.add_argument(
+        "-f",
+        "--format",
+        help="Select only a file format",
+        type=str,
+        choices=FILE_FORMAT,
+    )
+    parser.add_argument(
+        "-z", "--size", help="Start size in bytes", type=int, default=1, metavar="BYTES"
+    )
+    parser.add_argument(
+        "-m",
+        "--max-tracks",
+        help="Maximum number of tracks",
+        type=int,
+        default=None,
+        metavar="NUMBER",
+    )
     parser.add_argument("-t", "--title", help="Playlist title", default=None)
-    parser.add_argument("-g", "--encoding", help="Text encoding", choices=('UTF-8', 'ASCII', 'UNICODE'), default=None)
+    parser.add_argument(
+        "-g",
+        "--encoding",
+        help="Text encoding",
+        choices=("UTF-8", "ASCII", "UNICODE"),
+        default=None,
+    )
     parser.add_argument("-I", "--image", help="Playlist image", default=None)
-    parser.add_argument("-l", "--link", help="Add remote file links", nargs=argparse.ONE_OR_MORE, default=[])
-    parser.add_argument("-r", "--recursive", help="Recursive search", action='store_true')
-    parser.add_argument("-a", "--absolute", help="Absolute file name", action='store_true')
-    parser.add_argument("-s", "--shuffle", help="Casual order", action='store_true')
-    parser.add_argument("-u", "--unique", help="The same files are not placed in the playlist", action='store_true')
-    parser.add_argument("-c", "--append", help="Continue playlist instead of override it", action='store_true')
-    parser.add_argument("-w", "--windows", help="Windows style folder separator", 
-                        action='store_true')
-    parser.add_argument("-S", "--split", help="Split playlist by directories", action='store_true')
-    parser.add_argument("-o", "--orderby-name", help="Order playlist files by name", action='store_true')
-    parser.add_argument("-O", "--orderby-date", help="Order playlist files by date", action='store_true')
+    parser.add_argument(
+        "-l",
+        "--link",
+        help="Add remote file links",
+        nargs=argparse.ONE_OR_MORE,
+        default=[],
+    )
+    parser.add_argument(
+        "-r", "--recursive", help="Recursive search", action="store_true"
+    )
+    parser.add_argument(
+        "-a", "--absolute", help="Absolute file name", action="store_true"
+    )
+    parser.add_argument(
+        "-u",
+        "--unique",
+        help="The same files are not placed in the playlist",
+        action="store_true",
+    )
+    parser.add_argument(
+        "-c",
+        "--append",
+        help="Continue playlist instead of override it",
+        action="store_true",
+    )
+    parser.add_argument(
+        "-w", "--windows", help="Windows style folder separator", action="store_true"
+    )
+    parser.add_argument(
+        "-S", "--split", help="Split playlist by directories", action="store_true"
+    )
+    orderby_group.add_argument(
+        "-s", "--shuffle", help="Casual order", action="store_true"
+    )
+    orderby_group.add_argument(
+        "-o", "--orderby-name", help="Order playlist files by name", action="store_true"
+    )
+    orderby_group.add_argument(
+        "-O", "--orderby-date", help="Order playlist files by date", action="store_true"
+    )
+    orderby_group.add_argument(
+        "-T",
+        "--orderby-track",
+        help="Order playlist files by track",
+        action="store_true",
+    )
 
     args = parser.parse_args()
 
     # Check extension of playlist file
-    if not args.playlist.endswith('.m3u'):
-        if args.encoding == 'UNICODE':
-            if not args.playlist.endswith('.m3u8'):
-                args.playlist += '.m3u8'
+    if not args.playlist.endswith(".m3u"):
+        if args.encoding == "UNICODE":
+            if not args.playlist.endswith(".m3u8"):
+                args.playlist += ".m3u8"
         else:
-            args.playlist += '.m3u'
+            args.playlist += ".m3u"
 
     # Check if playlist is not a directory
     if isdir(args.playlist):
-        parser.error(f'{args.playlist} is a directory')
+        parser.error(f"{args.playlist} is a directory")
 
     # Open playlist file
-    args.open_mode = 'at+' if args.append else 'wt'
+    args.open_mode = "at+" if args.append else "wt"
     args.enabled_extensions = False
     args.enabled_title = False
     args.enabled_encoding = False
     # Verify extension attribute in append mode
     if args.append:
         with open(args.playlist, mode=args.open_mode) as opened_playlist:
             opened_playlist.seek(0)
             first_three_lines = opened_playlist.readlines(100)
             for line in first_three_lines:
-                if '#EXTM3U' in line:
+                if "#EXTM3U" in line:
                     args.enabled_extensions = True
-                if '#PLAYLIST' in line:
+                if "#PLAYLIST" in line:
                     args.enabled_title = True
-                if '#EXTENC' in line:
+                if "#EXTENC" in line:
                     args.enabled_encoding = True
             # Check if extensions are disabled and image is specified
             if getsize(args.playlist) > 0:
                 if not args.enabled_extensions and args.image:
-                    print(f'warning: image {args.image} has not been set because the extension flag'
-                          ' is not present in the playlist')
+                    print(
+                        f"warning: image {args.image} has not "
+                        "been set because the extension flag"
+                        " is not present in the playlist"
+                    )
                     args.image = None
 
     # Check if image file exists
     if args.image:
         if not exists(args.image):
-            parser.error(f'image file {args.image} does not exist')
+            parser.error(f"image file {args.image} does not exist")
 
     # Extend files format
     if args.include:
-        FILE_FORMAT.update(set([fmt.strip('*').strip('.') for fmt in args.include]))
+        FILE_FORMAT.update(set([fmt.strip("*").strip(".") for fmt in args.include]))
 
     # Select only one format
     if args.format:
-        FILE_FORMAT = {args.format.strip('*').strip('.')}
+        FILE_FORMAT = {args.format.strip("*").strip(".")}
 
     return args
 
 
 def file_in_playlist(playlist, file, root=None):
     """Check if file is in the playlist"""
     for f in playlist:
         # Skip extended tags
-        if f.startswith('#'):
+        if f.startswith("#"):
             continue
         # Check if absolute path in playlist
         if root:
             f = join(root, f)
         # Compare two files
         if cmp(f, file):
             return True
 
 
+def report_issue(exc):
+    """Report issue"""
+    print(
+        "error: {0} on line {1}, with error {2}".format(
+            type(exc).__name__, exc.__traceback__.tb_lineno, str(exc)
+        )
+    )
+    exit(1)
+
+
+def get_track(file):
+    """Sort file by track"""
+    file = File(file)
+    if hasattr(file, "tags"):
+        return file.tags.get("TRCK", "0")[0]
+
+
+def find_pattern(pattern, path):
+    """Find patter in a file and tags"""
+    file = File(path)
+    # Create compiled pattern
+    if not isinstance(pattern, re.Pattern):
+        pattern = re.compile(pattern)
+    # Check pattern into filename
+    if pattern.findall(file.filename):
+        return True
+    # Check supports of ID3 tagsadd compiled pattern
+    if hasattr(file, "ID3"):
+        # Check pattern into title
+        for title in file.tags.get("TIT2"):
+            if pattern.findall(title):
+                return True
+        # Check pattern into album
+        for album in file.tags.get("TALB"):
+            if pattern.findall(album):
+                return True
+
+
 def vprint(verbose, *messages):
     """Verbose print"""
     if verbose:
-        print('debug:', *messages)
+        print("debug:", *messages)
 
 
-def write_playlist(playlist,
-                   open_mode,
-                   files,
-                   enabled_extensions=False,
-                   image=None,
-                   ext_part=None,
-                   max_tracks=None,
-                   verbose=False):
+def write_playlist(
+        playlist,
+        open_mode,
+        files,
+        encoding,
+        enabled_extensions=False,
+        image=None,
+        ext_part=None,
+        max_tracks=None,
+        verbose=False,
+):
     """Write playlist into file"""
-    with open(playlist, mode=open_mode) as pl:
+    with open(
+            playlist,
+            mode=open_mode,
+            encoding="UTF-8" if encoding == "UNICODE" else encoding,
+            errors="ignore",
+    ) as pl:
         if image and enabled_extensions:
             vprint(verbose, f"set image {image}")
             joined_string = f"\n#EXTIMG: {image}\n"
         else:
-            joined_string = '\n'
-        end_file_string = '\n'
+            joined_string = "\n"
+        end_file_string = "\n"
         # Write extensions if exists
         if ext_part:
-            pl.write('\n'.join(files[:ext_part]) + joined_string)
+            pl.write("\n".join(files[:ext_part]) + joined_string)
         # Write all multimedia files
         vprint(verbose, f"write playlist {pl.name}")
         pl.write(joined_string.join(files[ext_part:max_tracks]) + end_file_string)
 
 
-def make_playlist(directory,
-                  pattern,
-                  file_formats,
-                  sortby_name=False,
-                  sortby_date=False,
-                  recursive=False,
-                  exclude_dirs=None,
-                  unique=False,
-                  absolute=False,
-                  min_size=1,
-                  windows=False,
-                  verbose=False):
+def make_playlist(
+        directory,
+        pattern,
+        file_formats,
+        sortby_name=False,
+        sortby_date=False,
+        sortby_track=False,
+        recursive=False,
+        exclude_dirs=None,
+        unique=False,
+        absolute=False,
+        min_size=1,
+        windows=False,
+        verbose=False,
+):
     """Make playlist list"""
     filelist = list()
     # Check if directory exists
     if not exists(directory):
-        print(f'warning: {directory} does not exists')
+        print(f"warning: {directory} does not exists")
         return filelist
     # Check if is a directory
     if not isdir(directory):
-        print(f'warning: {directory} is not a directory')
+        print(f"warning: {directory} is not a directory")
         return filelist
     # Build a Path object
     path = Path(directory)
     root = path.parent
     vprint(verbose, f"current directory={path}, root={root}")
     for fmt in file_formats:
         # Check recursive
-        folder = '**/*' if recursive else '*'
-        files = path.glob(folder + f'.{fmt}')
-        # Check sort
-        if sortby_name:
-            files = sorted(files)
-        if sortby_date:
-            files = sorted(files, key=getctime)
+        folder = "**/*" if recursive else "*"
+        files = path.glob(folder + f".{fmt}")
         for file in files:
             # Check if in exclude dirs
             if any([e_path in str(file) for e_path in exclude_dirs]):
                 continue
             # Check if file is in playlist
             if unique:
-                if file_in_playlist(filelist,
-                                    str(file),
-                                    root=root if not absolute else None):
+                if file_in_playlist(
+                        filelist, str(file), root=root if not absolute else None
+                ):
                     continue
-            # Check absolute file names
+            # Get size of file
             size = file.stat().st_size
+            # Check absolute file names
+            file_for_pattern = str(file)
             file = str(file) if absolute else str(file.relative_to(path.parent))
             # Check re pattern
-            if findall(pattern, file):
+            compiled_pattern = re.compile(pattern)
+            if find_pattern(compiled_pattern, file_for_pattern):
                 # Check file size
                 if size >= min_size:
                     vprint(verbose, f"add multimedia file {file}")
-                    filelist.append(
-                        sub('/', r"\\", file) if windows else file
-                    )
+                    filelist.append(sub("/", r"\\", file) if windows else file)
+    # Check sort
+    if sortby_name:
+        filelist = sorted(filelist)
+    elif sortby_date:
+        filelist = sorted(filelist, key=getctime)
+    elif sortby_track:
+        filelist = sorted(filelist, key=get_track)
     return filelist
 
 
 def add_extension(filelist, cli_args, verbose=False):
     """Add extension to playlist list"""
     if not isinstance(filelist, list):
-        raise ValueError(f'{filelist} is not a list object')
+        raise ValueError(f"{filelist} is not a list object")
 
     # Check if playlist is an extended M3U
     cli_args.ext_part = 0
     if cli_args.title or cli_args.encoding or cli_args.image:
         if not cli_args.enabled_extensions:
-            filelist.insert(0, '#EXTM3U')
+            filelist.insert(0, "#EXTM3U")
             vprint(verbose, "enable extension flag")
             cli_args.enabled_extensions = True
             cli_args.ext_part += 1
             if cli_args.max_tracks:
                 cli_args.max_tracks += 1
 
         # Set title
         if cli_args.title:
             if not cli_args.enabled_title:
                 title = capwords(cli_args.title)
-                filelist.insert(1, f'#PLAYLIST: {title}')
+                filelist.insert(1, f"#PLAYLIST: {title}")
                 vprint(verbose, f"set title {title}")
                 cli_args.ext_part += 1
                 if cli_args.max_tracks:
                     cli_args.max_tracks += 1
             else:
                 print("warning: title is already configured")
 
         # Set encoding
         if cli_args.encoding:
             if not cli_args.enabled_encoding:
-                filelist.insert(1, f'#EXTENC: {cli_args.encoding}')
+                filelist.insert(1, f"#EXTENC: {cli_args.encoding}")
                 vprint(verbose, f"set encoding {cli_args.encoding}")
                 cli_args.ext_part += 1
                 if cli_args.max_tracks:
                     cli_args.max_tracks += 1
             else:
                 print("warning: encoding is already configured")
 
@@ -285,68 +431,86 @@
     """Private function cli only for process arguments and make playlist"""
 
     # Add link
     files.extend(cli_args.link)
 
     # Build a playlist
     if files:
-
         # Check shuffle
         if cli_args.shuffle:
             shuffle(files)
 
         # Add extension to playlist
         add_extension(files, cli_args, verbose=cli_args.verbose)
 
         # Write playlist to file
-        write_playlist(other_playlist if other_playlist else cli_args.playlist,
-                       cli_args.open_mode,
-                       files,
-                       enabled_extensions=cli_args.enabled_extensions,
-                       image=cli_args.image,
-                       ext_part=cli_args.ext_part,
-                       max_tracks=cli_args.max_tracks,
-                       verbose=cli_args.verbose)
+        write_playlist(
+            other_playlist if other_playlist else cli_args.playlist,
+            cli_args.open_mode,
+            files,
+            encoding=cli_args.encoding,
+            enabled_extensions=cli_args.enabled_extensions,
+            image=cli_args.image,
+            ext_part=cli_args.ext_part,
+            max_tracks=cli_args.max_tracks,
+            verbose=cli_args.verbose,
+        )
     else:
-        print(f'warning: no multimedia files are found here: {",".join(cli_args.directories)}')
+        print(
+            "warning: no multimedia "
+            f'files are found here: {",".join(cli_args.directories)}'
+        )
 
 
 def main():
     """Make a playlist file"""
 
-    args = get_args()
-    multimedia_files = list()
-    vprint(args.verbose, f"formats={FILE_FORMAT}, recursive={args.recursive}, "
-                         f"pattern={args.pattern}, split={args.split}")
-
-    # Make multimedia list
-    for directory in args.directories:
-        directory_files = make_playlist(directory,
-                                        args.pattern,
-                                        FILE_FORMAT,
-                                        sortby_name=args.orderby_name,
-                                        sortby_date=args.orderby_date,
-                                        recursive=args.recursive,
-                                        exclude_dirs=args.exclude_dirs,
-                                        unique=args.unique,
-                                        absolute=args.absolute,
-                                        min_size=args.size,
-                                        windows=args.windows,
-                                        verbose=args.verbose)
-
-        multimedia_files.extend(directory_files)
-
-        # Check if you must split into directory playlist
-        if args.split:
-            playlist_name = basename(normpath(directory))
-            playlist_ext = '.m3u8' if args.encoding == 'UNICODE' else '.m3u'
-            playlist_path = join(dirname(args.playlist), playlist_name + playlist_ext)
-            _process_playlist(directory_files, args, playlist_path)
+    try:
+        args = get_args()
+        multimedia_files = list()
+        vprint(
+            args.verbose,
+            f"formats={FILE_FORMAT}, recursive={args.recursive}, "
+            f"pattern={args.pattern}, split={args.split}",
+        )
+
+        # Make multimedia list
+        for directory in args.directories:
+            directory_files = make_playlist(
+                directory,
+                args.pattern,
+                FILE_FORMAT,
+                sortby_name=args.orderby_name,
+                sortby_date=args.orderby_date,
+                sortby_track=args.orderby_track,
+                recursive=args.recursive,
+                exclude_dirs=args.exclude_dirs,
+                unique=args.unique,
+                absolute=args.absolute,
+                min_size=args.size,
+                windows=args.windows,
+                verbose=args.verbose,
+            )
+
+            multimedia_files.extend(directory_files)
+
+            # Check if you must split into directory playlist
+            if args.split:
+                playlist_name = basename(normpath(directory))
+                playlist_ext = ".m3u8" if args.encoding == "UNICODE" else ".m3u"
+                playlist_path = join(
+                    dirname(args.playlist), playlist_name + playlist_ext
+                )
+                _process_playlist(directory_files, args, playlist_path)
+                args.enabled_extensions = False
+
+        _process_playlist(multimedia_files, args)
 
-    _process_playlist(multimedia_files, args)
+    except Exception as err:
+        report_issue(err)
 
 
 # endregion
 
 # region main
 if __name__ == "__main__":
     main()
```

### Comparing `make_playlist-1.6.0/setup.py` & `make_playlist-1.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # setup -- mkpl
 #
-#     Copyright (C) 2022 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -31,14 +31,15 @@
     version=__info__.__version__,
     url=__info__.__homepage__,
     project_urls={
         'Documentation': __info__.__homepage__,
         'GitHub Project': __info__.__homepage__,
         'Issue Tracker': __info__.__homepage__ + '/issues'
     },
+    install_requires=["mutagen"],
     license='GNU General Public License v3.0',
     author=__info__.__author__,
     author_email=__info__.__email__,
     maintainer=__info__.__author__,
     maintainer_email=__info__.__email__,
     description='Make M3U format playlist from command line',
     long_description=long_description,
```

