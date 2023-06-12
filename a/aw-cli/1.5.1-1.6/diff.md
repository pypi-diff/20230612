# Comparing `tmp/aw-cli-1.5.1.tar.gz` & `tmp/aw-cli-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aw-cli-1.5.1.tar", last modified: Sun May 14 12:34:12 2023, max compression
+gzip compressed data, was "aw-cli-1.6.tar", last modified: Mon Jun 12 14:56:35 2023, max compression
```

## Comparing `aw-cli-1.5.1.tar` & `aw-cli-1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:34:12.579430 aw-cli-1.5.1/
--rw-r--r--   0 fexh      (1000) fexh      (1000)    35149 2023-05-14 12:33:54.000000 aw-cli-1.5.1/LICENSE
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2374 2023-05-14 12:34:12.579430 aw-cli-1.5.1/PKG-INFO
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2111 2023-05-14 12:33:54.000000 aw-cli-1.5.1/README.md
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:34:12.579430 aw-cli-1.5.1/aw_cli.egg-info/
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2374 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/PKG-INFO
--rw-r--r--   0 fexh      (1000) fexh      (1000)      300 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/SOURCES.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)        1 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/dependency_links.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)       42 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/entry_points.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)       47 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/requires.txt
--rw-r--r--   0 fexh      (1000) fexh      (1000)        6 2023-05-14 12:34:12.000000 aw-cli-1.5.1/aw_cli.egg-info/top_level.txt
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:34:12.579430 aw-cli-1.5.1/awcli/
--rw-r--r--   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:33:54.000000 aw-cli-1.5.1/awcli/__init__.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)    24766 2023-05-14 12:33:54.000000 aw-cli-1.5.1/awcli/run.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)    12080 2023-05-14 12:33:54.000000 aw-cli-1.5.1/awcli/utilities.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)       38 2023-05-14 12:34:12.579430 aw-cli-1.5.1/setup.cfg
--rw-r--r--   0 fexh      (1000) fexh      (1000)      920 2023-05-14 12:33:54.000000 aw-cli-1.5.1/setup.py
-drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-05-14 12:34:12.579430 aw-cli-1.5.1/tests/
--rw-r--r--   0 fexh      (1000) fexh      (1000)      473 2023-05-14 12:33:54.000000 aw-cli-1.5.1/tests/test_run.py
--rw-r--r--   0 fexh      (1000) fexh      (1000)     2880 2023-05-14 12:33:54.000000 aw-cli-1.5.1/tests/test_utilities.py
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-06-12 14:56:35.669304 aw-cli-1.6/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)    35149 2023-06-12 14:56:21.000000 aw-cli-1.6/LICENSE
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2466 2023-06-12 14:56:35.669304 aw-cli-1.6/PKG-INFO
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2205 2023-06-12 14:56:21.000000 aw-cli-1.6/README.md
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-06-12 14:56:35.669304 aw-cli-1.6/aw_cli.egg-info/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2466 2023-06-12 14:56:35.000000 aw-cli-1.6/aw_cli.egg-info/PKG-INFO
+-rw-r--r--   0 fexh      (1000) fexh      (1000)      300 2023-06-12 14:56:35.000000 aw-cli-1.6/aw_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)        1 2023-06-12 14:56:35.000000 aw-cli-1.6/aw_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       42 2023-06-12 14:56:35.000000 aw-cli-1.6/aw_cli.egg-info/entry_points.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       47 2023-06-12 14:56:35.000000 aw-cli-1.6/aw_cli.egg-info/requires.txt
+-rw-r--r--   0 fexh      (1000) fexh      (1000)        6 2023-06-12 14:56:35.000000 aw-cli-1.6/aw_cli.egg-info/top_level.txt
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-06-12 14:56:35.669304 aw-cli-1.6/awcli/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)        0 2023-06-12 14:56:21.000000 aw-cli-1.6/awcli/__init__.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)    27128 2023-06-12 14:56:21.000000 aw-cli-1.6/awcli/run.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)    14169 2023-06-12 14:56:21.000000 aw-cli-1.6/awcli/utilities.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)       38 2023-06-12 14:56:35.669304 aw-cli-1.6/setup.cfg
+-rw-r--r--   0 fexh      (1000) fexh      (1000)      918 2023-06-12 14:56:21.000000 aw-cli-1.6/setup.py
+drwxr-xr-x   0 fexh      (1000) fexh      (1000)        0 2023-06-12 14:56:35.669304 aw-cli-1.6/tests/
+-rw-r--r--   0 fexh      (1000) fexh      (1000)      473 2023-06-12 14:56:21.000000 aw-cli-1.6/tests/test_run.py
+-rw-r--r--   0 fexh      (1000) fexh      (1000)     2880 2023-06-12 14:56:21.000000 aw-cli-1.6/tests/test_utilities.py
```

### Comparing `aw-cli-1.5.1/LICENSE` & `aw-cli-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aw-cli-1.5.1/PKG-INFO` & `aw-cli-1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aw-cli
-Version: 1.5.1
+Version: 1.6
 Summary: guarda anime dal terminale e molto altro!
 Home-page: https://github.com/fexh10/aw-cli
 Author: fexh10
 License: GPL-3.0
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -45,27 +45,28 @@
 
 ```
 python3 -m pip uninstall aw-cli
 ```
 
 ## Utilizzo
 ```
-usage: aw-cli [-h] [-a] [-c] [-d] [-i] [-l [{a,s,d}]] [-o] [-s]
+usage: aw-cli [-h] [-a] [-c] [-d] [-i] [-l [{a,s,d}]] [-o] [-p] [-s]
 
 Guarda anime dal terminale e molto altro!
 
 options:
   -h, --help            show this help message and exit
   -a, --configurazione  avvia il menu di configurazione
   -c, --cronologia      continua a guardare un anime dalla cronologia
   -d, --download        scarica gli episodi che preferisci
   -i, --info            visualizza le informazioni e la trama di un anime
   -l [{a,s,d}], --lista [{a,s,d}]
                         lista degli ultimi anime usciti su AnimeWorld. a = all, s = sub, d = dub
   -o, --offline         apri gli episodi scaricati precedentemente direttamente dal terminale
+  -p, --privato         guarda un episodio senza che si aggiorni la cronologia o AniList
   -s, --syncplay        usa syncplay per guardare un anime insieme ai tuoi amici
                                                              
 ```
 
 ## Crediti
 Progetto ispirato a <a href="https://github.com/pystardust/ani-cli">ani-cli</a>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aw-cli Version: 1.5.1 Summary: guarda anime dal
+Metadata-Version: 2.1 Name: aw-cli Version: 1.6 Summary: guarda anime dal
 terminale e molto altro! Home-page: https://github.com/fexh10/aw-cli Author:
 fexh10 License: GPL-3.0 Requires-Python: >3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # aw-cli
                 **** Guarda anime dal terminale e molto altro!
                   Gli anime vengono presi da AnimeWorld ****
 ## Anteprima https://user-images.githubusercontent.com/90156014/210212814-
 e73ba7af-ce12-43ad-95ff-dcd85b39a45c.mp4 ## Indice - [Installazione]
@@ -13,17 +13,18 @@
 Se si utilizza Windows e MPV, occorrerÃ  scaricare inoltre "mpv-2.dll"
 (scaricabile da questo [link](https://sourceforge.net/projects/mpv-player-
 windows/files/libmpv/)) e aggiungerlo al path. Ã possibile installare aw-cli
 da pip: ``` python3 -m pip install aw-cli --upgrade ``` O se si preferisce da
 sorgente (potrebbe essere piÃ¹ aggiornato): ``` python3 -m pip install
 git+https://github.com/fexh10/aw-cli.git ``` ## Disinstallazione ``` python3 -
 m pip uninstall aw-cli ``` ## Utilizzo ``` usage: aw-cli [-h] [-a] [-c] [-d] [-
-i] [-l [{a,s,d}]] [-o] [-s] Guarda anime dal terminale e molto altro! options:
--h, --help show this help message and exit -a, --configurazione avvia il menu
-di configurazione -c, --cronologia continua a guardare un anime dalla
+i] [-l [{a,s,d}]] [-o] [-p] [-s] Guarda anime dal terminale e molto altro!
+options: -h, --help show this help message and exit -a, --configurazione avvia
+il menu di configurazione -c, --cronologia continua a guardare un anime dalla
 cronologia -d, --download scarica gli episodi che preferisci -i, --info
 visualizza le informazioni e la trama di un anime -l [{a,s,d}], --lista [
 {a,s,d}] lista degli ultimi anime usciti su AnimeWorld. a = all, s = sub, d =
 dub -o, --offline apri gli episodi scaricati precedentemente direttamente dal
-terminale -s, --syncplay usa syncplay per guardare un anime insieme ai tuoi
+terminale -p, --privato guarda un episodio senza che si aggiorni la cronologia
+o AniList -s, --syncplay usa syncplay per guardare un anime insieme ai tuoi
 amici ``` ## Crediti Progetto ispirato a ani-cli. Un ringraziamento speciale a
 axtrat per l'aiuto nella realizzazione del progetto.
```

### Comparing `aw-cli-1.5.1/README.md` & `aw-cli-1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,27 +34,28 @@
 
 ```
 python3 -m pip uninstall aw-cli
 ```
 
 ## Utilizzo
 ```
-usage: aw-cli [-h] [-a] [-c] [-d] [-i] [-l [{a,s,d}]] [-o] [-s]
+usage: aw-cli [-h] [-a] [-c] [-d] [-i] [-l [{a,s,d}]] [-o] [-p] [-s]
 
 Guarda anime dal terminale e molto altro!
 
 options:
   -h, --help            show this help message and exit
   -a, --configurazione  avvia il menu di configurazione
   -c, --cronologia      continua a guardare un anime dalla cronologia
   -d, --download        scarica gli episodi che preferisci
   -i, --info            visualizza le informazioni e la trama di un anime
   -l [{a,s,d}], --lista [{a,s,d}]
                         lista degli ultimi anime usciti su AnimeWorld. a = all, s = sub, d = dub
   -o, --offline         apri gli episodi scaricati precedentemente direttamente dal terminale
+  -p, --privato         guarda un episodio senza che si aggiorni la cronologia o AniList
   -s, --syncplay        usa syncplay per guardare un anime insieme ai tuoi amici
                                                              
 ```
 
 ## Crediti
 Progetto ispirato a <a href="https://github.com/pystardust/ani-cli">ani-cli</a>.
```

#### html2text {}

```diff
@@ -10,17 +10,18 @@
 Se si utilizza Windows e MPV, occorrerÃ  scaricare inoltre "mpv-2.dll"
 (scaricabile da questo [link](https://sourceforge.net/projects/mpv-player-
 windows/files/libmpv/)) e aggiungerlo al path. Ã possibile installare aw-cli
 da pip: ``` python3 -m pip install aw-cli --upgrade ``` O se si preferisce da
 sorgente (potrebbe essere piÃ¹ aggiornato): ``` python3 -m pip install
 git+https://github.com/fexh10/aw-cli.git ``` ## Disinstallazione ``` python3 -
 m pip uninstall aw-cli ``` ## Utilizzo ``` usage: aw-cli [-h] [-a] [-c] [-d] [-
-i] [-l [{a,s,d}]] [-o] [-s] Guarda anime dal terminale e molto altro! options:
--h, --help show this help message and exit -a, --configurazione avvia il menu
-di configurazione -c, --cronologia continua a guardare un anime dalla
+i] [-l [{a,s,d}]] [-o] [-p] [-s] Guarda anime dal terminale e molto altro!
+options: -h, --help show this help message and exit -a, --configurazione avvia
+il menu di configurazione -c, --cronologia continua a guardare un anime dalla
 cronologia -d, --download scarica gli episodi che preferisci -i, --info
 visualizza le informazioni e la trama di un anime -l [{a,s,d}], --lista [
 {a,s,d}] lista degli ultimi anime usciti su AnimeWorld. a = all, s = sub, d =
 dub -o, --offline apri gli episodi scaricati precedentemente direttamente dal
-terminale -s, --syncplay usa syncplay per guardare un anime insieme ai tuoi
+terminale -p, --privato guarda un episodio senza che si aggiorni la cronologia
+o AniList -s, --syncplay usa syncplay per guardare un anime insieme ai tuoi
 amici ``` ## Crediti Progetto ispirato a ani-cli. Un ringraziamento speciale a
 axtrat per l'aiuto nella realizzazione del progetto.
```

### Comparing `aw-cli-1.5.1/aw_cli.egg-info/PKG-INFO` & `aw-cli-1.6/aw_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aw-cli
-Version: 1.5.1
+Version: 1.6
 Summary: guarda anime dal terminale e molto altro!
 Home-page: https://github.com/fexh10/aw-cli
 Author: fexh10
 License: GPL-3.0
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -45,27 +45,28 @@
 
 ```
 python3 -m pip uninstall aw-cli
 ```
 
 ## Utilizzo
 ```
-usage: aw-cli [-h] [-a] [-c] [-d] [-i] [-l [{a,s,d}]] [-o] [-s]
+usage: aw-cli [-h] [-a] [-c] [-d] [-i] [-l [{a,s,d}]] [-o] [-p] [-s]
 
 Guarda anime dal terminale e molto altro!
 
 options:
   -h, --help            show this help message and exit
   -a, --configurazione  avvia il menu di configurazione
   -c, --cronologia      continua a guardare un anime dalla cronologia
   -d, --download        scarica gli episodi che preferisci
   -i, --info            visualizza le informazioni e la trama di un anime
   -l [{a,s,d}], --lista [{a,s,d}]
                         lista degli ultimi anime usciti su AnimeWorld. a = all, s = sub, d = dub
   -o, --offline         apri gli episodi scaricati precedentemente direttamente dal terminale
+  -p, --privato         guarda un episodio senza che si aggiorni la cronologia o AniList
   -s, --syncplay        usa syncplay per guardare un anime insieme ai tuoi amici
                                                              
 ```
 
 ## Crediti
 Progetto ispirato a <a href="https://github.com/pystardust/ani-cli">ani-cli</a>.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aw-cli Version: 1.5.1 Summary: guarda anime dal
+Metadata-Version: 2.1 Name: aw-cli Version: 1.6 Summary: guarda anime dal
 terminale e molto altro! Home-page: https://github.com/fexh10/aw-cli Author:
 fexh10 License: GPL-3.0 Requires-Python: >3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # aw-cli
                 **** Guarda anime dal terminale e molto altro!
                   Gli anime vengono presi da AnimeWorld ****
 ## Anteprima https://user-images.githubusercontent.com/90156014/210212814-
 e73ba7af-ce12-43ad-95ff-dcd85b39a45c.mp4 ## Indice - [Installazione]
@@ -13,17 +13,18 @@
 Se si utilizza Windows e MPV, occorrerÃ  scaricare inoltre "mpv-2.dll"
 (scaricabile da questo [link](https://sourceforge.net/projects/mpv-player-
 windows/files/libmpv/)) e aggiungerlo al path. Ã possibile installare aw-cli
 da pip: ``` python3 -m pip install aw-cli --upgrade ``` O se si preferisce da
 sorgente (potrebbe essere piÃ¹ aggiornato): ``` python3 -m pip install
 git+https://github.com/fexh10/aw-cli.git ``` ## Disinstallazione ``` python3 -
 m pip uninstall aw-cli ``` ## Utilizzo ``` usage: aw-cli [-h] [-a] [-c] [-d] [-
-i] [-l [{a,s,d}]] [-o] [-s] Guarda anime dal terminale e molto altro! options:
--h, --help show this help message and exit -a, --configurazione avvia il menu
-di configurazione -c, --cronologia continua a guardare un anime dalla
+i] [-l [{a,s,d}]] [-o] [-p] [-s] Guarda anime dal terminale e molto altro!
+options: -h, --help show this help message and exit -a, --configurazione avvia
+il menu di configurazione -c, --cronologia continua a guardare un anime dalla
 cronologia -d, --download scarica gli episodi che preferisci -i, --info
 visualizza le informazioni e la trama di un anime -l [{a,s,d}], --lista [
 {a,s,d}] lista degli ultimi anime usciti su AnimeWorld. a = all, s = sub, d =
 dub -o, --offline apri gli episodi scaricati precedentemente direttamente dal
-terminale -s, --syncplay usa syncplay per guardare un anime insieme ai tuoi
+terminale -p, --privato guarda un episodio senza che si aggiorni la cronologia
+o AniList -s, --syncplay usa syncplay per guardare un anime insieme ai tuoi
 amici ``` ## Crediti Progetto ispirato a ani-cli. Un ringraziamento speciale a
 axtrat per l'aiuto nella realizzazione del progetto.
```

### Comparing `aw-cli-1.5.1/awcli/run.py` & `aw-cli-1.6/awcli/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import time
 import hpcomt
 import argparse
 import warnings
 import subprocess
 import csv
+import concurrent.futures
 from pySmartDL import SmartDL
 from pathlib import Path
 from threading import Thread
 from awcli.utilities import *
 
 def safeExit():
     with open(f"{os.path.dirname(__file__)}/aw-cronologia.csv", 'w', newline='') as file:
@@ -222,26 +223,27 @@
         url_server (str): il link del video o il percorso del file.
         nome_video (str): il nome del video.
     """
 
     if nome_os == 'Linux':
         os.system(f'''vlc "{url_server}" --meta-title "{nome_video}" --fullscreen &>/dev/null''')
     elif nome_os == "Windows":
-        comando = f"& 'C:\\Program Files\\VideoLAN\\VLC\\vlc.exe' '{url_server}' --fullscreen --meta-title='{nome_video}'"
+        comando = f"""& 'C:\\Program Files\\VideoLAN\\VLC\\vlc.exe' "{url_server}" --fullscreen --meta-title="{nome_video}" """
         subprocess.Popen(['powershell.exe', comando])
         isRunning("vlc.exe")
     elif nome_os == "Android":
         os.system(f'''am start --user 0 -a android.intent.action.VIEW -d "{url_server}" -n org.videolan.vlc/.StartActivity -e "title" "{nome_video}" > /dev/null 2>&1 &''')    
 
 
 def addToCronologia(ep: int):
     """
     Viene aggiunta alla cronologia locale il nome del video,
-    il numero dell'ultimo episodio visualizzato
-    e il link di AnimeWorld relativo all'anime.
+    il numero dell'ultimo episodio visualizzato,
+    il link di AnimeWorld relativo all'anime
+    e il numero reale di episodi totali della serie.
     La cronologia viene salvata su un file csv nella stessa 
     directory dello script. Se il file non esiste viene creato.
 
     Args:
         ep (int): il numero dell'episodio visualizzato.
     """
     for i, riga in enumerate(log):
@@ -250,55 +252,57 @@
             #se l'ep riprodotto è l'ultimo allora non lo inserisco più
             if ep == anime.ep and anime.status == 1:
                 log.pop(i)
             else: 
                 #sovrascrivo la riga   
                 log[i][1] = ep
                 temp = log.pop(i)
+                temp[-1] = anime.ep_totali
                 #se l'anime è in corso e l'ep visualizzato è l'ultimo, metto l'anime alla fine della cronologia
                 if anime.status == 0 and ep == anime.ep:
                     log.insert(len(log), temp)
                 #altrimenti all'inizio
                 else:
                     log.insert(0, temp)
             return
     if (ep == anime.ep and anime.status == 0) or ep != anime.ep:
         if anime.status == 0 and ep == anime.ep:
-            log.insert(len(log), [anime.name, ep, anime.url])
+            log.insert(len(log), [anime.name, ep, anime.url, anime.ep_totali])
         else:
-            log.insert(0, [anime.name, ep, anime.url]) 
+            log.insert(0, [anime.name, ep, anime.url, anime.ep_totali]) 
 
 
-def updateAnilist(tokenAnilist: str, ratingAnilist: bool, preferitoAnilist: bool,  ep: int):
+def updateAnilist(tokenAnilist: str, ratingAnilist: bool, preferitoAnilist: bool,  ep: int, voto_anilist: str):
     """
     Procede ad aggiornare l'anime su AniList.
     Se l'episodio riprodotto è l'ultimo e
     l'utente ha scelto di votare gli anime,
     verrà chiesto il voto da dare.
 
     Args:
         tokenAnilist (str): il token di accesso ad AniList.
         ratingAnilist (bool): valore impostato a True se l'utente ha scelto di votare l'anime una volta finito, altrimenti False.
         preferitoAnilist(bool): True se l'utente ha scelto di far chiedere se mettere l'anime tra i preferiti, altrimenti False.
         ep (int): il numero dell'episodio visualizzato.
+        voto_anilist (str): il voto dato dall'utente all'anime su Anilist.
     """
 
     voto = 0
     preferiti = False
     status_list = 'CURRENT'
     #se ho finito di vedere l'anime
     if ep == anime.ep and anime.status == 1:
         status_list = 'COMPLETED'
         #chiedo di votare
         if ratingAnilist:
             def is_number(n):
                 if n.isdigit():
                     return n
 
-            voto = my_input("Inserisci un voto per l'anime", is_number)
+            voto = my_input(f"Inserisci un voto per l'anime (voto corrente: {voto_anilist})", is_number)
     
             voto = float(voto)
         #chiedo di mettere tra i preferiti
         if preferitoAnilist:
             def check_string(s: str):
                 s = s.lower()
                 if s == "s":
@@ -308,15 +312,15 @@
 
             preferiti = my_input("Mettere l'anime tra i preferiti? (s/N)", check_string)
     
     thread = Thread(target=anilistApi, args=(tokenAnilist, anime.id_anilist, ep, voto, status_list, preferiti))
     thread.start()
 
 
-def openVideos(ep_iniziale: int, ep_finale: int, mpv: bool, tokenAnilist: str, ratingAnilist: bool, preferitoAnilist: bool):
+def openVideos(ep_iniziale: int, ep_finale: int, mpv: bool, tokenAnilist: str, ratingAnilist: bool, preferitoAnilist: bool, user_id: int):
     """
     Riproduce gli episodi dell'anime, a partire da ep_iniziale fino a ep_finale.
     Se un episodio è già stato scaricato, viene riprodotto dal file scaricato.
     Altrimenti, viene riprodotto in streaming.
 
     Args:
         ep_iniziale (int): il numero di episodio iniziale da riprodurre.
@@ -339,39 +343,53 @@
             my_print(f"Episodio {nome_video} non scaricato, skippo...", color='giallo')
             sleep(1)
             continue
         else:
             url_server = anime.get_episodio(ep)
 
         my_print(f"Riproduco {nome_video}...", color="giallo", cls=True)
+
+        #se è l'episodio finale e l'utente deve votare l'anime, controllo se l'id è presente
+        # e ottengo il voto dell'anime se già inserito in precedenza
+        #prendo l'id dell'utente tramite query
+        voto_anilist = "n.d."
+        if ep == anime.ep and ratingAnilist == True and not offline and not privato:         
+            #prendo il voto se presente
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                future_rating = executor.submit(getAnimePrivateRating, tokenAnilist, user_id, anime.id_anilist)
+                voto_anilist = future_rating.result()
+
         openMPV(url_server, nome_video) if mpv else openVLC(url_server, nome_video)
 
-        #se non sono in modalità offline aggiungo l'anime alla cronologia
-        if not offline:
+        #se non sono in modalità offline o privata aggiungo l'anime alla cronologia
+        if not offline and not privato:
             addToCronologia(ep)
 
         #update watchlist anilist se ho fatto l'accesso
-        if tokenAnilist != 'tokenAnilist: False' and not offline:
-            updateAnilist(tokenAnilist, ratingAnilist, preferitoAnilist, ep)
+        if tokenAnilist != 'tokenAnilist: False' and not offline and not privato:
+            updateAnilist(tokenAnilist, ratingAnilist, preferitoAnilist, ep, voto_anilist)
 
 
-def getCronologia() -> tuple[list, list]:
+def getCronologia() -> tuple[list, list, list]:
     """
     Prende i dati dalla cronologia.
 
     Returns:
         tuple[list, list]: una tupla con la lista degli anime trovati e
         la lista degli ultimi episodi visualizzati.
 
     """
     episodi = []
     animes = []
     for riga in log:
+        if len(riga) == 3:
+            riga.append("??")
         episodi.append(riga[1])
-        animes.append(Anime(riga[0], riga[2], riga[1]))
+        animes.append(Anime(riga[0], riga[2], riga[1], riga[3]))
+
     #se il file esiste ma non contiene dati stampo un messaggio di errore
     if len(animes) == 0:
         my_print("Cronologia inesistente!", color='rosso')
         safeExit()
     return animes, episodi
 
 
@@ -411,78 +429,103 @@
         anilist = my_input("Aggiornare automaticamente la watchlist con AniList? (s/N)", check_string)
 
         if anilist:
             if nome_os == "Linux" or nome_os == "Android":
                 os.system("xdg-open 'https://anilist.co/api/v2/oauth/authorize?client_id=11388&response_type=token' &>/dev/null")
             elif nome_os == "Windows":
                 subprocess.Popen(['powershell.exe', "explorer https://anilist.co/api/v2/oauth/authorize?client_id=11388&response_type=token"])
+            #inserimento token
             tokenAnilist = my_input("Inserire il token di AniList", cls=True)
-            ratingAnilist = "ratingAnilist: True " if my_input("Votare l'anime una volta completato? (s/N)", check_string) else "ratingAnilist: False"
+            #chiede se votare l'anime
+            if my_input("Votare l'anime una volta completato? (s/N)", check_string):
+                ratingAnilist = "ratingAnilist: True "
+                #prendo l'id dell'utente tramite query
+                with concurrent.futures.ThreadPoolExecutor() as executor:
+                    future = executor.submit(getAnilistUserId, tokenAnilist)
+                    user_id = future.result()
+            else:
+                ratingAnilist = "ratingAnilist: False"
+                user_id = 0
             preferitoAnilist = "preferitoAnilist: True" if my_input("Chiedere se mettere l'anime tra i preferiti una volta completato? (s/N)", check_string) else "preferitoAnilist: False"
+
         else:
             tokenAnilist = "tokenAnilist: False"
             ratingAnilist = "ratingAnilist: False"
             preferitoAnilist = "preferitoAnilist: False"
+            user_id = 0
     except KeyboardInterrupt:
         safeExit()
     #creo il file
     config = f"{os.path.dirname(__file__)}/aw.config"
     with open(config, 'w') as config_file:
         config_file.write(f"{player}\n")
         config_file.write(f"{tokenAnilist}\n")
         config_file.write(f"{ratingAnilist}\n")
-        config_file.write(preferitoAnilist)
+        config_file.write(f"{preferitoAnilist}\n")
+        config_file.write(f"{user_id}")
 
 
-def getConfig() -> tuple[bool, str, bool, bool]:
+def getConfig() -> tuple[bool, str, bool, bool, int]:
     """
     Prende le impostazioni scelte dall'utente
     dal file di configurazione.
 
     Returns:
-        tuple[bool, str, bool]: mpv ritorna True se è stato scelto mpv, altrimenti false se è VLC.
+        tuple[bool, str, bool, int]: mpv ritorna True se è stato scelto mpv, altrimenti false se è VLC.
         tokenAnilist ritorna il token di Anilist se è stato inserito. ratingAnilist ritorna True
         se l'utente ha scelto di votare gli anime, altrimenti False. preferitoAnilist ritorna
         True se l'utente ha scelto di chiedere se l'anime deve essere aggiunto tra i preferiti,
-        altrimenti False.
+        altrimenti False. user_id ritorna l'id dell'utente.  
     """
 
     config = f"{os.path.dirname(__file__)}/aw.config"
-    with open(config, 'r') as config_file:
+    with open(config, 'r+') as config_file:
         lines = config_file.readlines()
         mpv = True if lines[0].strip() == "Player: MPV" else False
         tokenAnilist = lines[1].strip()
         ratingAnilist = True if lines[2].strip() == "ratingAnilist: True" else False
         preferitoAnilist = True if lines[3].strip() == "preferitoAnilist: True" else False
+        if len(lines) == 4 and ratingAnilist == False:
+            user_id = 0
+        elif len(lines) == 4 and ratingAnilist == True:
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                    future = executor.submit(getAnilistUserId, tokenAnilist)
+                    user_id = future.result()
+                    config_file.write(f"{user_id}")
+        else:
+            user_id = lines[4]
 
-    return mpv, tokenAnilist, ratingAnilist, preferitoAnilist
+    return mpv, tokenAnilist, ratingAnilist, preferitoAnilist, user_id
 
 
 def main():
     global log
     global syncpl
     global downl
     global lista
     global offline
     global cronologia
     global info
+    global privato
     global anime
     try:
         with open(f"{os.path.dirname(__file__)}/aw-cronologia.csv") as file:
             log = [riga for riga in csv.reader(file)]
     except FileNotFoundError:
         pass
     # args
     parser = argparse.ArgumentParser("aw-cli", description="Guarda anime dal terminale e molto altro!")
     parser.add_argument('-a', '--configurazione', action='store_true', dest='avvia_config', help='avvia il menu di configurazione')
     parser.add_argument('-c', '--cronologia', action='store_true', dest='cronologia', help='continua a guardare un anime dalla cronologia')
     parser.add_argument('-d', '--download', action='store_true', dest='download', help='scarica gli episodi che preferisci')
     parser.add_argument('-i', '--info', action='store_true', dest='info', help='visualizza le informazioni e la trama di un anime')
     parser.add_argument('-l', '--lista', nargs='?', choices=['a', 's', 'd'], dest='lista', help='lista degli ultimi anime usciti su AnimeWorld. a = all, s = sub, d = dub')
     parser.add_argument('-o', '--offline', action='store_true', dest='offline', help='apri gli episodi scaricati precedentemente direttamente dal terminale')
+    parser.add_argument('-p', '--privato', action='store_true', dest='privato', help="guarda un episodio senza che si aggiorni la cronologia o AniList")
+
     if nome_os != "Android":
         parser.add_argument('-s', '--syncplay', action='store_true', dest='syncpl', help='usa syncplay per guardare un anime insieme ai tuoi amici')
     args = parser.parse_args()
 
 
     if  '-l' in sys.argv and args.lista == None:
         args.lista = 'a'
@@ -494,38 +537,42 @@
         setupConfig()
     if args.info:
         info = True
     if args.download:
         downl = True
     if args.lista:
         lista = True
+    if args.privato:
+        privato = True
     elif args.offline:
         offline = True
     elif args.cronologia:
         cronologia = True
 
     #se il file di configurazione non esiste viene chiesto all'utente di fare il setup
     if not os.path.exists(f"{os.path.dirname(__file__)}/aw.config"):
         setupConfig()
-    mpv, tokenAnilist, ratingAnilist, preferitoAnilist = getConfig()
+    mpv, tokenAnilist, ratingAnilist, preferitoAnilist, user_id = getConfig()
 
     while True:
         try:
             if not cronologia:
                 animelist = latest(args.lista) if lista else animeScaricati(downloadPath()) if offline else RicercaAnime()
             else:
                 animelist, episodi = getCronologia()
 
             while True:
                 my_print("", end="", cls=True)
                 # stampo i nomi degli anime
                 for i, a in reversed(list(enumerate(animelist))):
                     my_print(f"{i + 1} ", color="verde", end=" ")
-                    if lista or cronologia:
-                        my_print(f"{a.name} [Ep {a.ep}]")
+                    if cronologia:
+                        my_print(f"{a.name} [Ep {a.ep}/{a.ep_totali}]")
+                    elif lista:
+                       my_print(f"{a.name} [Ep {a.ep}]") 
                     else:
                         my_print(a.name)
 
                 def check_index(s: str):
                     if s.isdigit():
                         index = int(s) - 1
                         if index in range(len(animelist)):
@@ -578,21 +625,21 @@
                 if nome_os == "Android":
                     my_print("Movies/Anime", color="verde")
                 else:
                     my_print("Video/Anime", color="verde")
                     
                     #chiedi all'utente se aprire ora i video scaricati
                     if my_input("Aprire ora il player con gli episodi scaricati? (S/n)", lambda i: i.lower()) in ['s', '']:
-                        openVideos(ep_iniziale, ep_finale, mpv, tokenAnilist, ratingAnilist, preferitoAnilist)
+                        openVideos(ep_iniziale, ep_finale, mpv, tokenAnilist, ratingAnilist, preferitoAnilist, user_id)
                 safeExit()
 
             ris_valida = True
             while True:
                 if ris_valida:
-                    openVideos(ep_iniziale,ep_finale, mpv, tokenAnilist, ratingAnilist, preferitoAnilist)
+                    openVideos(ep_iniziale,ep_finale, mpv, tokenAnilist, ratingAnilist, preferitoAnilist, user_id)
                 else:
                     my_print("Seleziona una risposta valida", color="rosso")
                     ris_valida = True
 
                 prossimo = True
                 antecedente = True
                 seleziona = True
@@ -643,13 +690,14 @@
 #args
 syncpl = False
 downl = False
 lista = False
 offline = False
 cronologia = False
 info = False
+privato = False
 log = []
 
 anime = Anime("", "")
 
 if __name__ == "__main__":
     main()
```

### Comparing `aw-cli-1.5.1/awcli/utilities.py` & `aw-cli-1.6/awcli/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,28 @@
     """
     Classe che rappresenta un anime.
 
     Attributes:
         name (str): il nome dell'anime.
         url (str): l'URL della pagina dell'anime su AnimeWorld.
         ep (int): il numero di episodi dell'anime.
-        ep_ini (int): il numero dell'episodio di inizio. Valore predefinito 1
+        ep_totali (str): il numero reale di episodi totali dell'anime.
     """ 
 
-    def __init__(self, name, url, ep=0) -> None:
+    def __init__(self, name, url, ep=0, ep_totali="") -> None:
         self.name = name
         self.url = url
         self.ep = ep
+        self.ep_totali = ep_totali
 
     def load_episodes(self, tokenAnilist) -> None:
         """
         Cerca gli URL degli episodi dell'anime e salva il numero di episodi trovati.
         """
-        self.url_episodi, self.status, self.id_anilist = episodes(self.url, tokenAnilist)
+        self.url_episodi, self.status, self.id_anilist, self.ep_totali = episodes(self.url, tokenAnilist)
         self.ep = len(self.url_episodi)
         self.ep_ini = 1
 
     def get_episodio(self, ep: int) -> str:
         """
         Restituisce il link dell'episodio specificato.
 
@@ -193,16 +194,17 @@
     div = bs.find("div", {"data-name": data_name})
     for div in div.find_all(class_='inner'):
         url = _url + div.a.get('href')
         
         for a in div.find_all(class_='name'):
             name = a.text
         for div in div.find_all(class_='ep'):
-            ep = int(float(div.text[3:]))
-        animes.append(Anime(name, url, ep))
+            ep = div.text[3:]
+            if ".5" not in ep:
+                animes.append(Anime(name, url, int(ep)))
         
 
     return animes
 
 def download(url_ep: str) -> str:
     """
     Cerca il link di download alternativo nella pagina selezionata.
@@ -214,53 +216,58 @@
         str: il link di download
     """
     bs = BeautifulSoup(requests.get(url_ep, headers=headers).text, "lxml")
 
     links = bs.find(id="download").find_all("a")
     return links[1].get('href')
 
-def episodes(url_ep: str, tokenAnilist: str) -> tuple[str, int, int]:
+def episodes(url_ep: str, tokenAnilist: str) -> tuple[str, int, int, str]:
     """
     Cerca i link degli episodi dell'anime nella pagina selezionata e 
     controlla se è ancora in corso.
 
     Args:
         url_ep (str): indica la pagina dell'episodio.
         tokenAnilist (str): il token di accesso ad AniList.
 
     Returns:
-        tuple[str, int, int]: la lista con gli URL dei vari episodi trovati, 
-        lo stato dell'anime e l'id di AniList se si ha effettuato l'accesso.
+        tuple[str, int, int, str]: la lista con gli URL dei vari episodi trovati, 
+        lo stato dell'anime, l'id di AniList se si ha effettuato l'accesso
+        e il numero reale degli episodi totali dell'anime.
     """
 
     # prendo l'html dalla pagina web di AW
     bs = BeautifulSoup(requests.get(url_ep, headers=headers).text, "lxml")
 
     url_episodi = list[str]()
     # cerco gli url di tutti gli episodi
     for div in bs.find_all(class_='server active'):
         for li in div.find_all(class_="episode"):
+            if ".5" in li.a.get('data-num'):
+                continue
             temp = "https://www.animeworld.tv" + (li.a.get('href'))
             url_episodi.append(temp)
     #cerco lo stato dell'anime. 1 se è finito, altrimenti 0
     status = 1
     dl = bs.find_all(class_='meta col-sm-6')
     for a in dl[1].find_all("a"):
         if "filter?status=0"in a.get('href'):
             status = 0
             break
+    #cerco il numero reale di episodi totali dell'anime
+    ep_totali = bs.find_all("dd")[12].string if status == 0 else len(url_episodi) 
     #cerco l'id di anilist
     id_anilist = 0
     try:
         if tokenAnilist != 'tokenAnilist: False':
             id_anilist = bs.find(class_='anilist control tip tippy-desktop-only').get('href').replace("https://anilist.co/anime/", "")
     except AttributeError:
         pass
 
-    return url_episodi, status, id_anilist
+    return url_episodi, status, id_anilist, ep_totali
 
 def printAnimeInfo(dt: list, dd: list, trama: str) -> str:
     """
     Stampa a schermo le informazioni
     e la trama relative all'anime selezioanto.
     Chiede all'utente se guardare l'anime oppure tornare indietro.
 
@@ -293,15 +300,15 @@
             return s
 
 
     my_print("\n(g) guardare", color='verde')
     my_print("(i) indietro", color='magenta', end="")
     return my_input("", check_string)
 
-def anilistApi(tokenAnilist: str, id_anilist: int, ep: int, voto: float, status_list: str, preferiti: bool):
+def anilistApi(tokenAnilist: str, id_anilist: int, ep: int, voto: float, status_list: str, preferiti: bool) -> None:
     """
     Collegamento alle API di AniList per aggiornare
     automaticamente gli anime.
 
     Args:
         tokenAnilist (str): il token di accesso ad AniList.
         id_anilist (int): l'id dell'anime su AniList.
@@ -346,10 +353,69 @@
         "episodio" : ep,
     }
     if voto != 0:
         var["score"] = voto
     header_anilist = {'Authorization': 'Bearer ' + tokenAnilist, 'Content-Type': 'application/json', 'Accept': 'application/json'}
     requests.post('https://graphql.anilist.co',headers=header_anilist,json={'query' : query, 'variables' : var}) 
 
+def getAnilistUserId(tokenAnilist: str) -> int: 
+    """
+    Collegamento alle API di AniList per trovare
+    l'id dell'utente.
+
+    Args:
+        tokenAnilist (str): il token di accesso ad AniList.
+
+    Returns:
+        int: l'id dell'utente.
+    """
+
+    query = """
+        query {
+            Viewer {
+                id
+            }
+        }
+    """
+
+    header_anilist = {'Authorization': 'Bearer ' + tokenAnilist, 'Content-Type': 'application/json', 'Accept': 'application/json'}
+    risposta = requests.post('https://graphql.anilist.co',headers=header_anilist,json={'query' : query}) 
+    user_id = int(risposta.json()["data"]["Viewer"]["id"])
+
+    return user_id
+
+def getAnimePrivateRating(tokenAnilist: str, user_id: int, id_anime: int) -> str:
+    """
+    Collegamento alle API di AniList per trovare
+    il voto dato all'anime dall'utente.
+
+    Args:
+        tokenAnilist (str): il token di accesso ad AniList.
+        user_id (int): l'id dell'utente su AniList.
+        id_anime (int): l'id dell'anime su Anilist.
+
+    Returns:
+        str: il voto dell'utente sotto forma di stringa.
+    """
+
+    query = """
+    query ($idAnime: Int, $userId: Int) {
+        MediaList(userId: $userId, mediaId: $idAnime) {
+            score
+        }
+    }
+    """
+    var = {
+    "idAnime": id_anime,
+    "userId": user_id
+}
+
+    header_anilist = {'Authorization': 'Bearer ' + tokenAnilist, 'Content-Type': 'application/json', 'Accept': 'application/json'}
+    risposta = requests.post('https://graphql.anilist.co',headers=header_anilist,json={'query' : query, 'variables' : var}) 
+    voto = str(risposta.json()["data"]["MediaList"]["score"])
+    if voto == "0":
+        voto = "n.d."
+    return voto
+
 headers = {
     'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36'
 }
```

### Comparing `aw-cli-1.5.1/setup.py` & `aw-cli-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     installRequires.append("psutil")
     installRequires.append("pywinauto")
     installRequires.append("python-mpv")
 
 setup(
     name="aw-cli",
     packages=find_packages(include=["awcli"]),
-    version="1.5.1",
+    version="1.6",
     python_requires=">3.10",
     description="guarda anime dal terminale e molto altro!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="fexh10",
     url="https://github.com/fexh10/aw-cli",
     license="GPL-3.0",
```

### Comparing `aw-cli-1.5.1/tests/test_utilities.py` & `aw-cli-1.6/tests/test_utilities.py`

 * *Files identical despite different names*

