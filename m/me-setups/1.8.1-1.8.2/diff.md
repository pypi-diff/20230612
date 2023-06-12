# Comparing `tmp/me_setups-1.8.1.tar.gz` & `tmp/me_setups-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.8.1.tar", last modified: Sun Jun  4 13:25:36 2023, max compression
+gzip compressed data, was "me_setups-1.8.2.tar", last modified: Mon Jun 12 06:30:19 2023, max compression
```

## Comparing `me_setups-1.8.1.tar` & `me_setups-1.8.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.335495 me_setups-1.8.1/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-04 13:25:36.335564 me_setups-1.8.1/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.1/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-04 13:25:36.337496 me_setups-1.8.1/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.1/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.304516 me_setups-1.8.1/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.312517 me_setups-1.8.1/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.1/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.326502 me_setups-1.8.1/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.1/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.1/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11273 2023-06-04 12:44:08.000000 me_setups-1.8.1/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.1/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.333598 me_setups-1.8.1/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.1/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8664 2023-06-04 12:17:51.000000 me_setups-1.8.1/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    12717 2023-06-04 12:44:08.000000 me_setups-1.8.1/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.1/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.1/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     2826 2023-06-04 13:24:16.000000 me_setups-1.8.1/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.319558 me_setups-1.8.1/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.323285 me_setups-1.8.2/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-12 06:30:19.323332 me_setups-1.8.2/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.2/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-12 06:30:19.326290 me_setups-1.8.2/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.2/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.263336 me_setups-1.8.2/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.275775 me_setups-1.8.2/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.2/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.302761 me_setups-1.8.2/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.2/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.2/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11657 2023-06-04 13:52:01.000000 me_setups-1.8.2/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.2/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.321291 me_setups-1.8.2/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.2/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8597 2023-06-06 17:26:44.000000 me_setups-1.8.2/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    12933 2023-06-04 13:52:01.000000 me_setups-1.8.2/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.2/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.2/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-06-06 17:26:44.000000 me_setups-1.8.2/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-12 06:30:19.289737 me_setups-1.8.2/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-12 06:30:19.000000 me_setups-1.8.2/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.8.1/PKG-INFO` & `me_setups-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.8.1
+Version: 1.8.2
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.1/setup.cfg` & `me_setups-1.8.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.8.1
+version = 1.8.2
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.8.1/src/me_setups/boards/default_boards.py` & `me_setups-1.8.2/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.1/src/me_setups/boards/gas52.py` & `me_setups-1.8.2/src/me_setups/boards/gas52.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,24 @@
         Returns:
             list[CompletedProcess[str]]: list off all commands proccesses
         """
         with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
             fs = [executor.submit(eq.run_ssh_cmd, cmd, **kwargs) for eq in self.eqs]
         return [f.result() for f in fs]
 
+    def list_cores(self) -> dict[EyeQ5, list[str]]:
+        """Returns all cores found on board.
+
+        Returns:
+            dict[EyeQ5, list[str]]: cores for each EQ.
+        """
+        with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
+            fs = {eq: executor.submit(eq.list_cores) for eq in self.eqs}
+        return {eq: fs[eq].result() for eq in self.eqs}
+
     def run_serial_cmd_all(self, cmd: str) -> None:
         """run serial command on all eqs.
 
         Args:
             cmd (str): the command to run
         """
         with ThreadPoolExecutor(max_workers=len(self.eqs)) as executor:
```

### Comparing `me_setups-1.8.1/src/me_setups/components/comp.py` & `me_setups-1.8.2/src/me_setups/components/comp.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     from typing_extensions import Literal
 
 from serial import Serial
 from serial import SerialException
 from serial.threaded import LineReader
 
 from me_setups.utils import filter_ansi_escape
-from me_setups.utils import lock_port
 
 logger = logging.getLogger(__name__)
 
 
 def add_line_timestamp(line: str) -> str:
     """adds timestamp to a given line
 
@@ -188,15 +187,14 @@
 
         Args:
             pbcm (str): pbcm for the Component
             port (str): path to the serial port.
         """
         self._pbcm = pbcm
         self.serial = SerialSniffer(port=port, baudrate=115200, timeout=5)
-        lock_port(port=port)
         self.logger = logging.getLogger(self.name)
 
     @property
     def prompt(self) -> bytes:
         raise NotImplementedError
 
     @property
```

### Comparing `me_setups-1.8.1/src/me_setups/components/eqs.py` & `me_setups-1.8.2/src/me_setups/components/eqs.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,27 +188,35 @@
         Args:
             dst (pathlib.Path | str): Path to folder to extract to.
             timeout (float, optional): timeout for the copy process. Defaults to 180.
 
         Returns:
             CompletedProcess[str] | None: status of extracting process None if no cores
         """
-        cores = self.ssh_cmd_stdout("find /media/storage/crash/ -type f").splitlines()
+        cores = self.list_cores()
         if not cores:
             return None
         if not all(core.endswith(".zip") for core in cores):
             self.wait_for_core_write(core_type=CoreType.PCD)  # pragma: no cover
         return self.copy_from(
             f"{self.crash_folder}/*",
             pathlib.Path(dst) / self.name,
             timeout=timeout,
             recurcive=True,
             mkdir=True,
         )
 
+    def list_cores(self) -> list[str]:
+        """returns list for all cores on EyeQ
+
+        Returns:
+            list[str]: list of string paths for cores on the setup
+        """
+        return self.ssh_cmd_stdout("find /media/storage/crash/ -type f").splitlines()
+
     def wait_for_linux_boot(self) -> bool:
         """waits to Linux boot msg "Welcome to EyeQ5"
 
         Returns:
             bool: boot msg recived
         """
         boot_msg = b"Welcome to EyeQ5"
```

### Comparing `me_setups-1.8.1/src/me_setups/components/mcu.py` & `me_setups-1.8.2/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.1/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.8.2/src/me_setups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.8.1
+Version: 1.8.2
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.1/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.8.2/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

