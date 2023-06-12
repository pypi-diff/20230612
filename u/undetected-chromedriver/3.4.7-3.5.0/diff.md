# Comparing `tmp/undetected-chromedriver-3.4.7.tar.gz` & `tmp/undetected-chromedriver-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undetected-chromedriver-3.4.7.tar", last modified: Tue May  9 20:27:03 2023, max compression
+gzip compressed data, was "undetected-chromedriver-3.5.0.tar", last modified: Mon Jun 12 09:39:23 2023, max compression
```

## Comparing `undetected-chromedriver-3.4.7.tar` & `undetected-chromedriver-3.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 20:27:03.496985 undetected-chromedriver-3.4.7/
--rw-rw-rw-   0        0        0    35823 2023-02-04 20:28:40.000000 undetected-chromedriver-3.4.7/LICENSE
--rw-rw-rw-   0        0        0    76699 2023-05-09 20:27:03.495982 undetected-chromedriver-3.4.7/PKG-INFO
--rw-rw-rw-   0        0        0    75683 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 20:27:03.496985 undetected-chromedriver-3.4.7/setup.cfg
--rw-rw-rw-   0        0        0     2670 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 20:27:03.462915 undetected-chromedriver-3.4.7/undetected_chromedriver/
--rw-rw-rw-   0        0        0    34297 2023-05-09 20:19:13.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/__init__.py
--rw-rw-rw-   0        0        0     3498 2023-02-04 20:28:40.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/cdp.py
--rw-rw-rw-   0        0        0     5937 2023-02-04 20:28:40.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/devtool.py
--rw-rw-rw-   0        0        0     1837 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/dprocess.py
--rw-rw-rw-   0        0        0     2751 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/options.py
--rw-rw-rw-   0        0        0    11782 2023-05-09 20:10:37.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/patcher.py
--rw-rw-rw-   0        0        0     3065 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/reactor.py
--rw-rw-rw-   0        0        0     2900 2023-05-09 16:23:12.000000 undetected-chromedriver-3.4.7/undetected_chromedriver/webelement.py
-drwxrwxrwx   0        0        0        0 2023-05-09 20:27:03.483421 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/
--rw-rw-rw-   0        0        0    76699 2023-05-09 20:27:02.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      541 2023-05-09 20:27:03.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 20:27:02.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-09 20:27:03.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-09 20:27:03.000000 undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 09:39:23.644458 undetected-chromedriver-3.5.0/
+-rw-rw-rw-   0        0        0    35823 2023-06-12 09:02:34.000000 undetected-chromedriver-3.5.0/LICENSE
+-rw-rw-rw-   0        0        0    76699 2023-06-12 09:39:23.632458 undetected-chromedriver-3.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    75683 2023-06-12 09:02:34.000000 undetected-chromedriver-3.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 09:39:23.648458 undetected-chromedriver-3.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2605 2023-06-12 09:34:25.000000 undetected-chromedriver-3.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:39:23.144007 undetected-chromedriver-3.5.0/undetected_chromedriver/
+-rw-rw-rw-   0        0        0    32896 2023-06-12 09:38:17.000000 undetected-chromedriver-3.5.0/undetected_chromedriver/__init__.py
+-rw-rw-rw-   0        0        0     3386 2023-06-12 09:02:34.000000 undetected-chromedriver-3.5.0/undetected_chromedriver/cdp.py
+-rw-rw-rw-   0        0        0     5747 2023-06-12 09:02:34.000000 undetected-chromedriver-3.5.0/undetected_chromedriver/devtool.py
+-rw-rw-rw-   0        0        0     1763 2023-06-12 09:02:34.000000 undetected-chromedriver-3.5.0/undetected_chromedriver/dprocess.py
+-rw-rw-rw-   0        0        0     2666 2023-06-12 09:02:34.000000 undetected-chromedriver-3.5.0/undetected_chromedriver/options.py
+-rw-rw-rw-   0        0        0    11434 2023-06-12 09:02:34.000000 undetected-chromedriver-3.5.0/undetected_chromedriver/patcher.py
+-rw-rw-rw-   0        0        0     2966 2023-06-12 09:02:34.000000 undetected-chromedriver-3.5.0/undetected_chromedriver/reactor.py
+-rw-rw-rw-   0        0        0     2814 2023-06-12 09:02:34.000000 undetected-chromedriver-3.5.0/undetected_chromedriver/webelement.py
+drwxrwxrwx   0        0        0        0 2023-06-12 09:39:23.571339 undetected-chromedriver-3.5.0/undetected_chromedriver.egg-info/
+-rw-rw-rw-   0        0        0    76699 2023-06-12 09:39:20.000000 undetected-chromedriver-3.5.0/undetected_chromedriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      541 2023-06-12 09:39:21.000000 undetected-chromedriver-3.5.0/undetected_chromedriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 09:39:20.000000 undetected-chromedriver-3.5.0/undetected_chromedriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-12 09:39:20.000000 undetected-chromedriver-3.5.0/undetected_chromedriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-12 09:39:20.000000 undetected-chromedriver-3.5.0/undetected_chromedriver.egg-info/top_level.txt
```

### Comparing `undetected-chromedriver-3.4.7/LICENSE` & `undetected-chromedriver-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.7/PKG-INFO` & `undetected-chromedriver-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undetected-chromedriver
-Version: 3.4.7
+Version: 3.5.0
 Summary: ('Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.', 'Not triggered by CloudFlare/Imperva/hCaptcha and such.', 'NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.')
 Home-page: https://github.com/ultrafunkamsterdam/undetected-chromedriver
 Author: UltrafunkAmsterdam
 Author-email: info@blackhat-security.nl
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `undetected-chromedriver-3.4.7/README.md` & `undetected-chromedriver-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `undetected-chromedriver-3.4.7/setup.py` & `undetected-chromedriver-3.5.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-"""
-
-         888                                                  888         d8b
-         888                                                  888         Y8P
-         888                                                  888
- .d8888b 88888b.  888d888 .d88b.  88888b.d88b.   .d88b.   .d88888 888d888 888 888  888  .d88b.  888d888
-d88P"    888 "88b 888P"  d88""88b 888 "888 "88b d8P  Y8b d88" 888 888P"   888 888  888 d8P  Y8b 888P"
-888      888  888 888    888  888 888  888  888 88888888 888  888 888     888 Y88  88P 88888888 888
-Y88b.    888  888 888    Y88..88P 888  888  888 Y8b.     Y88b 888 888     888  Y8bd8P  Y8b.     888
- "Y8888P 888  888 888     "Y88P"  888  888  888  "Y8888   "Y88888 888     888   Y88P    "Y8888  888   88888888
-
-BY ULTRAFUNKAMSTERDAM (https://github.com/ultrafunkamsterdam)"""
-
-import codecs
-import os
-import re
-
-from setuptools import setup
-
-
-dirname = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(
-    os.path.join(dirname, "undetected_chromedriver", "__init__.py"),
-    mode="r",
-    encoding="utf-8",
-) as fp:
-    try:
-        version = re.findall(r"^__version__ = ['\"]([^'\"]*)['\"]", fp.read(), re.M)[0]
-    except Exception:
-        raise RuntimeError("unable to determine version")
-
-description = (
-    "Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.",
-    "Not triggered by CloudFlare/Imperva/hCaptcha and such.",
-    "NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.",
-)
-
-setup(
-    name="undetected-chromedriver",
-    version=version,
-    packages=["undetected_chromedriver"],
-    install_requires=[
-        "selenium>=4.0.0",
-        "requests",
-        "websockets",
-    ],
-    package_data={"undetected_chromedriver": [os.path.join("example", "example.py")]},
-    url="https://github.com/ultrafunkamsterdam/undetected-chromedriver",
-    license="GPL-3.0",
-    author="UltrafunkAmsterdam",
-    author_email="info@blackhat-security.nl",
-    description=description,
-    long_description=open(os.path.join(dirname, "README.md"), encoding="utf-8").read(),
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
-)
+"""
+
+         888                                                  888         d8b
+         888                                                  888         Y8P
+         888                                                  888
+ .d8888b 88888b.  888d888 .d88b.  88888b.d88b.   .d88b.   .d88888 888d888 888 888  888  .d88b.  888d888
+d88P"    888 "88b 888P"  d88""88b 888 "888 "88b d8P  Y8b d88" 888 888P"   888 888  888 d8P  Y8b 888P"
+888      888  888 888    888  888 888  888  888 88888888 888  888 888     888 Y88  88P 88888888 888
+Y88b.    888  888 888    Y88..88P 888  888  888 Y8b.     Y88b 888 888     888  Y8bd8P  Y8b.     888
+ "Y8888P 888  888 888     "Y88P"  888  888  888  "Y8888   "Y88888 888     888   Y88P    "Y8888  888   88888888
+
+BY ULTRAFUNKAMSTERDAM (https://github.com/ultrafunkamsterdam)"""
+
+import codecs
+import os
+import re
+
+from setuptools import setup
+
+
+dirname = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(
+    os.path.join(dirname, "undetected_chromedriver", "__init__.py"),
+    mode="r",
+    encoding="utf-8",
+) as fp:
+    try:
+        version = re.findall(r"^__version__ = ['\"]([^'\"]*)['\"]", fp.read(), re.M)[0]
+    except Exception:
+        raise RuntimeError("unable to determine version")
+
+description = (
+    "Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.",
+    "Not triggered by CloudFlare/Imperva/hCaptcha and such.",
+    "NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.",
+)
+
+setup(
+    name="undetected-chromedriver",
+    version=version,
+    packages=["undetected_chromedriver"],
+    install_requires=[
+        "selenium>=4.9.0",
+        "requests",
+        "websockets",
+    ],
+    package_data={"undetected_chromedriver": [os.path.join("example", "example.py")]},
+    url="https://github.com/ultrafunkamsterdam/undetected-chromedriver",
+    license="GPL-3.0",
+    author="UltrafunkAmsterdam",
+    author_email="info@blackhat-security.nl",
+    description=description,
+    long_description=open(os.path.join(dirname, "README.md"), encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+)
```

### Comparing `undetected-chromedriver-3.4.7/undetected_chromedriver/__init__.py` & `undetected-chromedriver-3.5.0/undetected_chromedriver/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,856 +1,851 @@
-#!/usr/bin/env python3
-
-"""
-
-         888                                                  888         d8b
-         888                                                  888         Y8P
-         888                                                  888
- .d8888b 88888b.  888d888 .d88b.  88888b.d88b.   .d88b.   .d88888 888d888 888 888  888  .d88b.  888d888
-d88P"    888 "88b 888P"  d88""88b 888 "888 "88b d8P  Y8b d88" 888 888P"   888 888  888 d8P  Y8b 888P"
-888      888  888 888    888  888 888  888  888 88888888 888  888 888     888 Y88  88P 88888888 888
-Y88b.    888  888 888    Y88..88P 888  888  888 Y8b.     Y88b 888 888     888  Y8bd8P  Y8b.     888
- "Y8888P 888  888 888     "Y88P"  888  888  888  "Y8888   "Y88888 888     888   Y88P    "Y8888  888   88888888
-
-by UltrafunkAmsterdam (https://github.com/ultrafunkamsterdam)
-
-"""
-from __future__ import annotations
-
-
-__version__ = "3.4.7"
-
-import json
-import logging
-import os
-import re
-import shutil
-import subprocess
-import sys
-import tempfile
-import time
-from weakref import finalize
-
-import selenium.webdriver.chrome.service
-import selenium.webdriver.chrome.webdriver
-from selenium.webdriver.common.by import By
-import selenium.webdriver.common.service
-import selenium.webdriver.remote.command
-import selenium.webdriver.remote.webdriver
-
-from .cdp import CDP
-from .dprocess import start_detached
-from .options import ChromeOptions
-from .patcher import IS_POSIX
-from .patcher import Patcher
-from .reactor import Reactor
-from .webelement import UCWebElement
-from .webelement import WebElement
-
-
-__all__ = (
-    "Chrome",
-    "ChromeOptions",
-    "Patcher",
-    "Reactor",
-    "CDP",
-    "find_chrome_executable",
-)
-
-logger = logging.getLogger("uc")
-logger.setLevel(logging.getLogger().getEffectiveLevel())
-
-
-class Chrome(selenium.webdriver.chrome.webdriver.WebDriver):
-    """
-
-    Controls the ChromeDriver and allows you to drive the browser.
-
-    The webdriver file will be downloaded by this module automatically,
-    you do not need to specify this. however, you may if you wish.
-
-    Attributes
-    ----------
-
-    Methods
-    -------
-
-    reconnect()
-
-        this can be useful in case of heavy detection methods
-        -stops the chromedriver service which runs in the background
-        -starts the chromedriver service which runs in the background
-        -recreate session
-
-
-    start_session(capabilities=None, browser_profile=None)
-
-        differentiates from the regular method in that it does not
-        require a capabilities argument. The capabilities are automatically
-        recreated from the options at creation time.
-
-    --------------------------------------------------------------------------
-        NOTE:
-            Chrome has everything included to work out of the box.
-            it does not `need` customizations.
-            any customizations MAY lead to trigger bot migitation systems.
-
-    --------------------------------------------------------------------------
-    """
-
-    _instances = set()
-    session_id = None
-    debug = False
-
-    def __init__(
-        self,
-        options=None,
-        user_data_dir=None,
-        driver_executable_path=None,
-        browser_executable_path=None,
-        port=0,
-        enable_cdp_events=False,
-        service_args=None,
-        service_creationflags=None,
-        desired_capabilities=None,
-        advanced_elements=False,
-        service_log_path=None,
-        keep_alive=True,
-        log_level=0,
-        headless=False,
-        version_main=None,
-        patcher_force_close=False,
-        suppress_welcome=True,
-        use_subprocess=True,
-        debug=False,
-        no_sandbox=True,
-        user_multi_procs: bool = False,
-        **kw,
-    ):
-        """
-        Creates a new instance of the chrome driver.
-
-        Starts the service and then creates new instance of chrome driver.
-
-        Parameters
-        ----------
-
-        options: ChromeOptions, optional, default: None - automatic useful defaults
-            this takes an instance of ChromeOptions, mainly to customize browser behavior.
-            anything other dan the default, for example extensions or startup options
-            are not supported in case of failure, and can probably lowers your undetectability.
-
-
-        user_data_dir: str , optional, default: None (creates temp profile)
-            if user_data_dir is a path to a valid chrome profile directory, use it,
-            and turn off automatic removal mechanism at exit.
-
-        driver_executable_path: str, optional, default: None(=downloads and patches new binary)
-
-        browser_executable_path: str, optional, default: None - use find_chrome_executable
-            Path to the browser executable.
-            If not specified, make sure the executable's folder is in $PATH
-
-        port: int, optional, default: 0
-            port to be used by the chromedriver executable, this is NOT the debugger port.
-            leave it at 0 unless you know what you are doing.
-            the default value of 0 automatically picks an available port.
-
-        enable_cdp_events: bool, default: False
-            :: currently for chrome only
-            this enables the handling of wire messages
-            when enabled, you can subscribe to CDP events by using:
-
-                driver.add_cdp_listener("Network.dataReceived", yourcallback)
-                # yourcallback is an callable which accepts exactly 1 dict as parameter
-
-
-        service_args: list of str, optional, default: None
-            arguments to pass to the driver service
-
-        desired_capabilities: dict, optional, default: None - auto from config
-            Dictionary object with non-browser specific capabilities only, such as "item" or "loggingPref".
-
-        advanced_elements:  bool, optional, default: False
-            makes it easier to recognize elements like you know them from html/browser inspection, especially when working
-            in an interactive environment
-
-            default webelement repr:
-            <selenium.webdriver.remote.webelement.WebElement (session="85ff0f671512fa535630e71ee951b1f2", element="6357cb55-92c3-4c0f-9416-b174f9c1b8c4")>
-
-            advanced webelement repr
-            <WebElement(<a class="mobile-show-inline-block mc-update-infos init-ok" href="#" id="main-cat-switcher-mobile">)>
-
-            note: when retrieving large amounts of elements ( example: find_elements_by_tag("*") ) and print them, it does take a little more time.
-
-
-        service_log_path: str, optional, default: None
-             path to log information from the driver.
-
-        keep_alive: bool, optional, default: True
-             Whether to configure ChromeRemoteConnection to use HTTP keep-alive.
-
-        log_level: int, optional, default: adapts to python global log level
-
-        headless: bool, optional, default: False
-            can also be specified in the options instance.
-            Specify whether you want to use the browser in headless mode.
-            warning: this lowers undetectability and not fully supported.
-
-        version_main: int, optional, default: None (=auto)
-            if you, for god knows whatever reason, use
-            an older version of Chrome. You can specify it's full rounded version number
-            here. Example: 87 for all versions of 87
-
-        patcher_force_close: bool, optional, default: False
-            instructs the patcher to do whatever it can to access the chromedriver binary
-            if the file is locked, it will force shutdown all instances.
-            setting it is not recommended, unless you know the implications and think
-            you might need it.
-
-        suppress_welcome: bool, optional , default: True
-            a "welcome" alert might show up on *nix-like systems asking whether you want to set
-            chrome as your default browser, and if you want to send even more data to google.
-            now, in case you are nag-fetishist, or a diagnostics data feeder to google, you can set this to False.
-            Note: if you don't handle the nag screen in time, the browser loses it's connection and throws an Exception.
-
-        use_subprocess: bool, optional , default: True,
-
-            False (the default) makes sure Chrome will get it's own process (so no subprocess of chromedriver.exe or python
-                This fixes a LOT of issues, like multithreaded run, but mst importantly. shutting corectly after
-                program exits or using .quit()
-                you should be knowing what you're doing, and know how python works.
-
-              unfortunately, there  is always an edge case in which one would like to write an single script with the only contents being:
-              --start script--
-              import undetected_chromedriver as uc
-              d = uc.Chrome()
-              d.get('https://somesite/')
-              ---end script --
-
-              and will be greeted with an error, since the program exists before chrome has a change to launch.
-              in that case you can set this to `True`. The browser will start via subprocess, and will keep running most of times.
-              ! setting it to True comes with NO support when being detected. !
-
-        no_sandbox: bool, optional, default=True
-             uses the --no-sandbox option, and additionally does suppress the "unsecure option" status bar
-             this option has a default of True since many people seem to run this as root (....) , and chrome does not start
-             when running as root without using --no-sandbox flag.
-
-        user_multi_procs:
-            set to true when you are using multithreads/multiprocessing
-            ensures not all processes are trying to modify a binary which is in use by another.
-            for this to work. YOU MUST HAVE AT LEAST 1 UNDETECTED_CHROMEDRIVER BINARY IN YOUR ROAMING DATA FOLDER.
-            this requirement can be easily satisfied, by just running this program "normal" and close/kill it.
-
-
-        """
-
-        finalize(self, self._ensure_close, self)
-        self.debug = debug
-        self.patcher = Patcher(
-            executable_path=driver_executable_path,
-            force=patcher_force_close,
-            version_main=version_main,
-            user_multi_procs=user_multi_procs,
-        )
-        # self.patcher.auto(user_multiprocess = user_multi_num_procs)
-        self.patcher.auto()
-
-        # self.patcher = patcher
-        if not options:
-            options = ChromeOptions()
-
-        try:
-            if hasattr(options, "_session") and options._session is not None:
-                #  prevent reuse of options,
-                #  as it just appends arguments, not replace them
-                #  you'll get conflicts starting chrome
-                raise RuntimeError("you cannot reuse the ChromeOptions object")
-        except AttributeError:
-            pass
-
-        options._session = self
-
-        if not options.debugger_address:
-            debug_port = (
-                port
-                if port != 0
-                else selenium.webdriver.common.service.utils.free_port()
-            )
-            debug_host = "127.0.0.1"
-            options.debugger_address = "%s:%d" % (debug_host, debug_port)
-        else:
-            debug_host, debug_port = options.debugger_address.split(":")
-            debug_port = int(debug_port)
-
-        if enable_cdp_events:
-            options.set_capability(
-                "goog:loggingPrefs", {"performance": "ALL", "browser": "ALL"}
-            )
-
-        options.add_argument("--remote-debugging-host=%s" % debug_host)
-        options.add_argument("--remote-debugging-port=%s" % debug_port)
-
-        if user_data_dir:
-            options.add_argument("--user-data-dir=%s" % user_data_dir)
-
-        language, keep_user_data_dir = None, bool(user_data_dir)
-
-        # see if a custom user profile is specified in options
-        for arg in options.arguments:
-
-            if any([_ in arg for _ in ("--headless", "headless")]):
-                options.arguments.remove(arg)
-                options.headless = True
-
-            if "lang" in arg:
-                m = re.search("(?:--)?lang(?:[ =])?(.*)", arg)
-                try:
-                    language = m[1]
-                except IndexError:
-                    logger.debug("will set the language to en-US,en;q=0.9")
-                    language = "en-US,en;q=0.9"
-
-            if "user-data-dir" in arg:
-                m = re.search("(?:--)?user-data-dir(?:[ =])?(.*)", arg)
-                try:
-                    user_data_dir = m[1]
-                    logger.debug(
-                        "user-data-dir found in user argument %s => %s" % (arg, m[1])
-                    )
-                    keep_user_data_dir = True
-
-                except IndexError:
-                    logger.debug(
-                        "no user data dir could be extracted from supplied argument %s "
-                        % arg
-                    )
-
-        if not user_data_dir:
-            # backward compatiblity
-            # check if an old uc.ChromeOptions is used, and extract the user data dir
-
-            if hasattr(options, "user_data_dir") and getattr(
-                options, "user_data_dir", None
-            ):
-                import warnings
-
-                warnings.warn(
-                    "using ChromeOptions.user_data_dir might stop working in future versions."
-                    "use uc.Chrome(user_data_dir='/xyz/some/data') in case you need existing profile folder"
-                )
-                options.add_argument("--user-data-dir=%s" % options.user_data_dir)
-                keep_user_data_dir = True
-                logger.debug(
-                    "user_data_dir property found in options object: %s" % user_data_dir
-                )
-
-            else:
-                user_data_dir = os.path.normpath(tempfile.mkdtemp())
-                keep_user_data_dir = False
-                arg = "--user-data-dir=%s" % user_data_dir
-                options.add_argument(arg)
-                logger.debug(
-                    "created a temporary folder in which the user-data (profile) will be stored during this\n"
-                    "session, and added it to chrome startup arguments: %s" % arg
-                )
-
-        if not language:
-            try:
-                import locale
-
-                language = locale.getdefaultlocale()[0].replace("_", "-")
-            except Exception:
-                pass
-            if not language:
-                language = "en-US"
-
-        options.add_argument("--lang=%s" % language)
-
-        if not options.binary_location:
-            options.binary_location = (
-                browser_executable_path or find_chrome_executable()
-            )
-
-        self._delay = 3
-
-        self.user_data_dir = user_data_dir
-        self.keep_user_data_dir = keep_user_data_dir
-
-        if suppress_welcome:
-            options.arguments.extend(["--no-default-browser-check", "--no-first-run"])
-        if no_sandbox:
-            options.arguments.extend(["--no-sandbox", "--test-type"])
-
-        if headless or options.headless:
-            if self.patcher.version_main < 108:
-                options.add_argument("--headless=chrome")
-            elif self.patcher.version_main >= 108:
-                options.add_argument("--headless=new")
-
-        options.add_argument("--window-size=1920,1080")
-        options.add_argument("--start-maximized")
-        options.add_argument("--no-sandbox")
-        # fixes "could not connect to chrome" error when running
-        # on linux using privileged user like root (which i don't recommend)
-
-        options.add_argument(
-            "--log-level=%d" % log_level
-            or divmod(logging.getLogger().getEffectiveLevel(), 10)[0]
-        )
-
-        if hasattr(options, "handle_prefs"):
-            options.handle_prefs(user_data_dir)
-
-        # fix exit_type flag to prevent tab-restore nag
-        try:
-            with open(
-                os.path.join(user_data_dir, "Default/Preferences"),
-                encoding="latin1",
-                mode="r+",
-            ) as fs:
-                config = json.load(fs)
-                if config["profile"]["exit_type"] is not None:
-                    # fixing the restore-tabs-nag
-                    config["profile"]["exit_type"] = None
-                fs.seek(0, 0)
-                json.dump(config, fs)
-                fs.truncate()  # the file might be shorter
-                logger.debug("fixed exit_type flag")
-        except Exception as e:
-            logger.debug("did not find a bad exit_type flag ")
-
-        self.options = options
-
-        if not desired_capabilities:
-            desired_capabilities = options.to_capabilities()
-
-        if not use_subprocess:
-            self.browser_pid = start_detached(
-                options.binary_location, *options.arguments
-            )
-        else:
-            browser = subprocess.Popen(
-                [options.binary_location, *options.arguments],
-                stdin=subprocess.PIPE,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-                close_fds=IS_POSIX,
-            )
-            self.browser_pid = browser.pid
-
-        if service_creationflags:
-            service = selenium.webdriver.common.service.Service(
-                self.patcher.executable_path, port, service_args, service_log_path
-            )
-            for attr_name in ("creationflags", "creation_flags"):
-                if hasattr(service, attr_name):
-                    setattr(service, attr_name, service_creationflags)
-                    break
-        else:
-            service = None
-
-        super(Chrome, self).__init__(
-            executable_path=self.patcher.executable_path,
-            port=port,
-            options=options,
-            service_args=service_args,
-            desired_capabilities=desired_capabilities,
-            service_log_path=service_log_path,
-            keep_alive=keep_alive,
-            service=service,  # needed or the service will be re-created
-        )
-
-        self.reactor = None
-
-        if enable_cdp_events:
-            if logging.getLogger().getEffectiveLevel() == logging.DEBUG:
-                logging.getLogger(
-                    "selenium.webdriver.remote.remote_connection"
-                ).setLevel(20)
-            reactor = Reactor(self)
-            reactor.start()
-            self.reactor = reactor
-
-        if advanced_elements:
-            self._web_element_cls = UCWebElement
-        else:
-            self._web_element_cls = WebElement
-
-        if options.headless:
-            self._configure_headless()
-
-    def _configure_headless(self):
-        orig_get = self.get
-        logger.info("setting properties for headless")
-
-        def get_wrapped(*args, **kwargs):
-            if self.execute_script("return navigator.webdriver"):
-                logger.info("patch navigator.webdriver")
-                self.execute_cdp_cmd(
-                    "Page.addScriptToEvaluateOnNewDocument",
-                    {
-                        "source": """
-
-                           Object.defineProperty(window, "navigator", {
-                                Object.defineProperty(window, "navigator", {
-                                  value: new Proxy(navigator, {
-                                    has: (target, key) => (key === "webdriver" ? false : key in target),
-                                    get: (target, key) =>
-                                      key === "webdriver"
-                                        ? false
-                                        : typeof target[key] === "function"
-                                        ? target[key].bind(target)
-                                        : target[key],
-                                  }),
-                                });
-                    """
-                    },
-                )
-
-                logger.info("patch user-agent string")
-                self.execute_cdp_cmd(
-                    "Network.setUserAgentOverride",
-                    {
-                        "userAgent": self.execute_script(
-                            "return navigator.userAgent"
-                        ).replace("Headless", "")
-                    },
-                )
-                self.execute_cdp_cmd(
-                    "Page.addScriptToEvaluateOnNewDocument",
-                    {
-                        "source": """
-                            Object.defineProperty(navigator, 'maxTouchPoints', {get: () => 1});
-                            Object.defineProperty(navigator.connection, 'rtt', {get: () => 100});
-
-                            // https://github.com/microlinkhq/browserless/blob/master/packages/goto/src/evasions/chrome-runtime.js
-                            window.chrome = {
-                                app: {
-                                    isInstalled: false,
-                                    InstallState: {
-                                        DISABLED: 'disabled',
-                                        INSTALLED: 'installed',
-                                        NOT_INSTALLED: 'not_installed'
-                                    },
-                                    RunningState: {
-                                        CANNOT_RUN: 'cannot_run',
-                                        READY_TO_RUN: 'ready_to_run',
-                                        RUNNING: 'running'
-                                    }
-                                },
-                                runtime: {
-                                    OnInstalledReason: {
-                                        CHROME_UPDATE: 'chrome_update',
-                                        INSTALL: 'install',
-                                        SHARED_MODULE_UPDATE: 'shared_module_update',
-                                        UPDATE: 'update'
-                                    },
-                                    OnRestartRequiredReason: {
-                                        APP_UPDATE: 'app_update',
-                                        OS_UPDATE: 'os_update',
-                                        PERIODIC: 'periodic'
-                                    },
-                                    PlatformArch: {
-                                        ARM: 'arm',
-                                        ARM64: 'arm64',
-                                        MIPS: 'mips',
-                                        MIPS64: 'mips64',
-                                        X86_32: 'x86-32',
-                                        X86_64: 'x86-64'
-                                    },
-                                    PlatformNaclArch: {
-                                        ARM: 'arm',
-                                        MIPS: 'mips',
-                                        MIPS64: 'mips64',
-                                        X86_32: 'x86-32',
-                                        X86_64: 'x86-64'
-                                    },
-                                    PlatformOs: {
-                                        ANDROID: 'android',
-                                        CROS: 'cros',
-                                        LINUX: 'linux',
-                                        MAC: 'mac',
-                                        OPENBSD: 'openbsd',
-                                        WIN: 'win'
-                                    },
-                                    RequestUpdateCheckStatus: {
-                                        NO_UPDATE: 'no_update',
-                                        THROTTLED: 'throttled',
-                                        UPDATE_AVAILABLE: 'update_available'
-                                    }
-                                }
-                            }
-
-                            // https://github.com/microlinkhq/browserless/blob/master/packages/goto/src/evasions/navigator-permissions.js
-                            if (!window.Notification) {
-                                window.Notification = {
-                                    permission: 'denied'
-                                }
-                            }
-
-                            const originalQuery = window.navigator.permissions.query
-                            window.navigator.permissions.__proto__.query = parameters =>
-                                parameters.name === 'notifications'
-                                    ? Promise.resolve({ state: window.Notification.permission })
-                                    : originalQuery(parameters)
-
-                            const oldCall = Function.prototype.call
-                            function call() {
-                                return oldCall.apply(this, arguments)
-                            }
-                            Function.prototype.call = call
-
-                            const nativeToStringFunctionString = Error.toString().replace(/Error/g, 'toString')
-                            const oldToString = Function.prototype.toString
-
-                            function functionToString() {
-                                if (this === window.navigator.permissions.query) {
-                                    return 'function query() { [native code] }'
-                                }
-                                if (this === functionToString) {
-                                    return nativeToStringFunctionString
-                                }
-                                return oldCall.call(oldToString, this)
-                            }
-                            // eslint-disable-next-line
-                            Function.prototype.toString = functionToString
-                            """
-                    },
-                )
-            return orig_get(*args, **kwargs)
-
-        self.get = get_wrapped
-
-    # def _get_cdc_props(self):
-    #     return self.execute_script(
-    #         """
-    #         let objectToInspect = window,
-    #             result = [];
-    #         while(objectToInspect !== null)
-    #         { result = result.concat(Object.getOwnPropertyNames(objectToInspect));
-    #           objectToInspect = Object.getPrototypeOf(objectToInspect); }
-    #
-    #         return result.filter(i => i.match(/^([a-zA-Z]){27}(Array|Promise|Symbol)$/ig))
-    #         """
-    #     )
-    #
-    # def _hook_remove_cdc_props(self):
-    #     self.execute_cdp_cmd(
-    #         "Page.addScriptToEvaluateOnNewDocument",
-    #         {
-    #             "source": """
-    #                 let objectToInspect = window,
-    #                     result = [];
-    #                 while(objectToInspect !== null)
-    #                 { result = result.concat(Object.getOwnPropertyNames(objectToInspect));
-    #                   objectToInspect = Object.getPrototypeOf(objectToInspect); }
-    #                 result.forEach(p => p.match(/^([a-zA-Z]){27}(Array|Promise|Symbol)$/ig)
-    #                                     &&delete window[p]&&console.log('removed',p))
-    #                 """
-    #         },
-    #     )
-
-    def get(self, url):
-        # if self._get_cdc_props():
-        #     self._hook_remove_cdc_props()
-        return super().get(url)
-
-    def add_cdp_listener(self, event_name, callback):
-        if (
-            self.reactor
-            and self.reactor is not None
-            and isinstance(self.reactor, Reactor)
-        ):
-            self.reactor.add_event_handler(event_name, callback)
-            return self.reactor.handlers
-        return False
-
-    def clear_cdp_listeners(self):
-        if self.reactor and isinstance(self.reactor, Reactor):
-            self.reactor.handlers.clear()
-
-    def window_new(self):
-        self.execute(
-            selenium.webdriver.remote.command.Command.NEW_WINDOW, {"type": "window"}
-        )
-
-    def tab_new(self, url: str):
-        """
-        this opens a url in a new tab.
-        apparently, that passes all tests directly!
-
-        Parameters
-        ----------
-        url
-
-        Returns
-        -------
-
-        """
-        if not hasattr(self, "cdp"):
-            from .cdp import CDP
-
-            cdp = CDP(self.options)
-            cdp.tab_new(url)
-
-    def reconnect(self, timeout=0.1):
-        try:
-            self.service.stop()
-        except Exception as e:
-            logger.debug(e)
-        time.sleep(timeout)
-        try:
-            self.service.start()
-        except Exception as e:
-            logger.debug(e)
-
-        try:
-            self.start_session()
-        except Exception as e:
-            logger.debug(e)
-
-    def start_session(self, capabilities=None, browser_profile=None):
-        if not capabilities:
-            capabilities = self.options.to_capabilities()
-        super(selenium.webdriver.chrome.webdriver.WebDriver, self).start_session(
-            capabilities, browser_profile
-        )
-        # super(Chrome, self).start_session(capabilities, browser_profile)
-
-    def quit(self):
-        try:
-            self.service.process.kill()
-            logger.debug("webdriver process ended")
-        except (AttributeError, RuntimeError, OSError):
-            pass
-        try:
-            self.reactor.event.set()
-            logger.debug("shutting down reactor")
-        except AttributeError:
-            pass
-        try:
-            os.kill(self.browser_pid, 15)
-            logger.debug("gracefully closed browser")
-        except Exception as e:  # noqa
-            logger.debug(e, exc_info=True)
-        if (
-            hasattr(self, "keep_user_data_dir")
-            and hasattr(self, "user_data_dir")
-            and not self.keep_user_data_dir
-        ):
-            for _ in range(5):
-                try:
-                    shutil.rmtree(self.user_data_dir, ignore_errors=False)
-                except FileNotFoundError:
-                    pass
-                except (RuntimeError, OSError, PermissionError) as e:
-                    logger.debug(
-                        "When removing the temp profile, a %s occured: %s\nretrying..."
-                        % (e.__class__.__name__, e)
-                    )
-                else:
-                    logger.debug("successfully removed %s" % self.user_data_dir)
-                    break
-                time.sleep(0.1)
-
-        # dereference patcher, so patcher can start cleaning up as well.
-        # this must come last, otherwise it will throw 'in use' errors
-        self.patcher = None
-
-    def __getattribute__(self, item):
-        if not super().__getattribute__("debug"):
-            return super().__getattribute__(item)
-        else:
-            import inspect
-
-            original = super().__getattribute__(item)
-            if inspect.ismethod(original) and not inspect.isclass(original):
-
-                def newfunc(*args, **kwargs):
-                    logger.debug(
-                        "calling %s with args %s and kwargs %s\n"
-                        % (original.__qualname__, args, kwargs)
-                    )
-                    return original(*args, **kwargs)
-
-                return newfunc
-            return original
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.service.stop()
-        time.sleep(self._delay)
-        self.service.start()
-        self.start_session()
-
-    def __hash__(self):
-        return hash(self.options.debugger_address)
-
-    def __dir__(self):
-        return object.__dir__(self)
-
-    def __del__(self):
-        try:
-            self.service.process.kill()
-        except:  # noqa
-            pass
-        self.quit()
-
-    @classmethod
-    def _ensure_close(cls, self):
-        # needs to be a classmethod so finalize can find the reference
-        logger.info("ensuring close")
-        if (
-            hasattr(self, "service")
-            and hasattr(self.service, "process")
-            and hasattr(self.service.process, "kill")
-        ):
-            self.service.process.kill()
-
-
-def find_chrome_executable():
-    """
-    Finds the chrome, chrome beta, chrome canary, chromium executable
-
-    Returns
-    -------
-    executable_path :  str
-        the full file path to found executable
-
-    """
-    candidates = set()
-    if IS_POSIX:
-        for item in os.environ.get("PATH").split(os.pathsep):
-            for subitem in (
-                "google-chrome",
-                "chromium",
-                "chromium-browser",
-                "chrome",
-                "google-chrome-stable",
-            ):
-                candidates.add(os.sep.join((item, subitem)))
-        if "darwin" in sys.platform:
-            candidates.update(
-                [
-                    "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
-                    "/Applications/Chromium.app/Contents/MacOS/Chromium",
-                ]
-            )
-    else:
-        for item in map(
-            os.environ.get,
-            ("PROGRAMFILES", "PROGRAMFILES(X86)", "LOCALAPPDATA", "PROGRAMW6432"),
-        ):
-            if item is not None:
-                for subitem in (
-                    "Google/Chrome/Application",
-                    "Google/Chrome Beta/Application",
-                    "Google/Chrome Canary/Application",
-                ):
-                    candidates.add(os.sep.join((item, subitem, "chrome.exe")))
-    for candidate in candidates:
-        if os.path.exists(candidate) and os.access(candidate, os.X_OK):
-            return os.path.normpath(candidate)
+#!/usr/bin/env python3
+
+"""
+
+         888                                                  888         d8b
+         888                                                  888         Y8P
+         888                                                  888
+ .d8888b 88888b.  888d888 .d88b.  88888b.d88b.   .d88b.   .d88888 888d888 888 888  888  .d88b.  888d888
+d88P"    888 "88b 888P"  d88""88b 888 "888 "88b d8P  Y8b d88" 888 888P"   888 888  888 d8P  Y8b 888P"
+888      888  888 888    888  888 888  888  888 88888888 888  888 888     888 Y88  88P 88888888 888
+Y88b.    888  888 888    Y88..88P 888  888  888 Y8b.     Y88b 888 888     888  Y8bd8P  Y8b.     888
+ "Y8888P 888  888 888     "Y88P"  888  888  888  "Y8888   "Y88888 888     888   Y88P    "Y8888  888   88888888
+
+by UltrafunkAmsterdam (https://github.com/ultrafunkamsterdam)
+
+"""
+from __future__ import annotations
+
+
+__version__ = "3.5.0"
+
+import json
+import logging
+import os
+import re
+import shutil
+import subprocess
+import sys
+import tempfile
+import time
+from weakref import finalize
+
+import selenium.webdriver.chrome.service
+import selenium.webdriver.chrome.webdriver
+from selenium.webdriver.common.by import By
+import selenium.webdriver.chromium.service
+import selenium.webdriver.remote.command
+import selenium.webdriver.remote.webdriver
+
+from .cdp import CDP
+from .dprocess import start_detached
+from .options import ChromeOptions
+from .patcher import IS_POSIX
+from .patcher import Patcher
+from .reactor import Reactor
+from .webelement import UCWebElement
+from .webelement import WebElement
+
+
+__all__ = (
+    "Chrome",
+    "ChromeOptions",
+    "Patcher",
+    "Reactor",
+    "CDP",
+    "find_chrome_executable",
+)
+
+logger = logging.getLogger("uc")
+logger.setLevel(logging.getLogger().getEffectiveLevel())
+
+
+class Chrome(selenium.webdriver.chrome.webdriver.WebDriver):
+    """
+
+    Controls the ChromeDriver and allows you to drive the browser.
+
+    The webdriver file will be downloaded by this module automatically,
+    you do not need to specify this. however, you may if you wish.
+
+    Attributes
+    ----------
+
+    Methods
+    -------
+
+    reconnect()
+
+        this can be useful in case of heavy detection methods
+        -stops the chromedriver service which runs in the background
+        -starts the chromedriver service which runs in the background
+        -recreate session
+
+
+    start_session(capabilities=None, browser_profile=None)
+
+        differentiates from the regular method in that it does not
+        require a capabilities argument. The capabilities are automatically
+        recreated from the options at creation time.
+
+    --------------------------------------------------------------------------
+        NOTE:
+            Chrome has everything included to work out of the box.
+            it does not `need` customizations.
+            any customizations MAY lead to trigger bot migitation systems.
+
+    --------------------------------------------------------------------------
+    """
+
+    _instances = set()
+    session_id = None
+    debug = False
+
+    def __init__(
+        self,
+        options=None,
+        user_data_dir=None,
+        driver_executable_path=None,
+        browser_executable_path=None,
+        port=0,
+        enable_cdp_events=False,
+        desired_capabilities=None,
+        advanced_elements=False,
+        keep_alive=True,
+        log_level=0,
+        headless=False,
+        version_main=None,
+        patcher_force_close=False,
+        suppress_welcome=True,
+        use_subprocess=True,
+        debug=False,
+        no_sandbox=True,
+        user_multi_procs: bool = False,
+        **kw,
+    ):
+        """
+        Creates a new instance of the chrome driver.
+
+        Starts the service and then creates new instance of chrome driver.
+
+        Parameters
+        ----------
+
+        options: ChromeOptions, optional, default: None - automatic useful defaults
+            this takes an instance of ChromeOptions, mainly to customize browser behavior.
+            anything other dan the default, for example extensions or startup options
+            are not supported in case of failure, and can probably lowers your undetectability.
+
+
+        user_data_dir: str , optional, default: None (creates temp profile)
+            if user_data_dir is a path to a valid chrome profile directory, use it,
+            and turn off automatic removal mechanism at exit.
+
+        driver_executable_path: str, optional, default: None(=downloads and patches new binary)
+
+        browser_executable_path: str, optional, default: None - use find_chrome_executable
+            Path to the browser executable.
+            If not specified, make sure the executable's folder is in $PATH
+
+        port: int, optional, default: 0
+            port to be used by the chromedriver executable, this is NOT the debugger port.
+            leave it at 0 unless you know what you are doing.
+            the default value of 0 automatically picks an available port.
+
+        enable_cdp_events: bool, default: False
+            :: currently for chrome only
+            this enables the handling of wire messages
+            when enabled, you can subscribe to CDP events by using:
+
+                driver.add_cdp_listener("Network.dataReceived", yourcallback)
+                # yourcallback is an callable which accepts exactly 1 dict as parameter
+
+
+        service_args: list of str, optional, default: None
+            arguments to pass to the driver service
+
+        desired_capabilities: dict, optional, default: None - auto from config
+            Dictionary object with non-browser specific capabilities only, such as "item" or "loggingPref".
+
+        advanced_elements:  bool, optional, default: False
+            makes it easier to recognize elements like you know them from html/browser inspection, especially when working
+            in an interactive environment
+
+            default webelement repr:
+            <selenium.webdriver.remote.webelement.WebElement (session="85ff0f671512fa535630e71ee951b1f2", element="6357cb55-92c3-4c0f-9416-b174f9c1b8c4")>
+
+            advanced webelement repr
+            <WebElement(<a class="mobile-show-inline-block mc-update-infos init-ok" href="#" id="main-cat-switcher-mobile">)>
+
+            note: when retrieving large amounts of elements ( example: find_elements_by_tag("*") ) and print them, it does take a little more time.
+
+        log_level: int, optional, default: adapts to python global log level
+
+        headless: bool, optional, default: False
+            can also be specified in the options instance.
+            Specify whether you want to use the browser in headless mode.
+            warning: this lowers undetectability and not fully supported.
+
+        version_main: int, optional, default: None (=auto)
+            if you, for god knows whatever reason, use
+            an older version of Chrome. You can specify it's full rounded version number
+            here. Example: 87 for all versions of 87
+
+        patcher_force_close: bool, optional, default: False
+            instructs the patcher to do whatever it can to access the chromedriver binary
+            if the file is locked, it will force shutdown all instances.
+            setting it is not recommended, unless you know the implications and think
+            you might need it.
+
+        suppress_welcome: bool, optional , default: True
+            a "welcome" alert might show up on *nix-like systems asking whether you want to set
+            chrome as your default browser, and if you want to send even more data to google.
+            now, in case you are nag-fetishist, or a diagnostics data feeder to google, you can set this to False.
+            Note: if you don't handle the nag screen in time, the browser loses it's connection and throws an Exception.
+
+        use_subprocess: bool, optional , default: True,
+
+            False (the default) makes sure Chrome will get it's own process (so no subprocess of chromedriver.exe or python
+                This fixes a LOT of issues, like multithreaded run, but mst importantly. shutting corectly after
+                program exits or using .quit()
+                you should be knowing what you're doing, and know how python works.
+
+              unfortunately, there  is always an edge case in which one would like to write an single script with the only contents being:
+              --start script--
+              import undetected_chromedriver as uc
+              d = uc.Chrome()
+              d.get('https://somesite/')
+              ---end script --
+
+              and will be greeted with an error, since the program exists before chrome has a change to launch.
+              in that case you can set this to `True`. The browser will start via subprocess, and will keep running most of times.
+              ! setting it to True comes with NO support when being detected. !
+
+        no_sandbox: bool, optional, default=True
+             uses the --no-sandbox option, and additionally does suppress the "unsecure option" status bar
+             this option has a default of True since many people seem to run this as root (....) , and chrome does not start
+             when running as root without using --no-sandbox flag.
+
+        user_multi_procs:
+            set to true when you are using multithreads/multiprocessing
+            ensures not all processes are trying to modify a binary which is in use by another.
+            for this to work. YOU MUST HAVE AT LEAST 1 UNDETECTED_CHROMEDRIVER BINARY IN YOUR ROAMING DATA FOLDER.
+            this requirement can be easily satisfied, by just running this program "normal" and close/kill it.
+
+
+        """
+
+        finalize(self, self._ensure_close, self)
+        self.debug = debug
+        self.patcher = Patcher(
+            executable_path=driver_executable_path,
+            force=patcher_force_close,
+            version_main=version_main,
+            user_multi_procs=user_multi_procs,
+        )
+        # self.patcher.auto(user_multiprocess = user_multi_num_procs)
+        self.patcher.auto()
+
+        # self.patcher = patcher
+        if not options:
+            options = ChromeOptions()
+
+        try:
+            if hasattr(options, "_session") and options._session is not None:
+                #  prevent reuse of options,
+                #  as it just appends arguments, not replace them
+                #  you'll get conflicts starting chrome
+                raise RuntimeError("you cannot reuse the ChromeOptions object")
+        except AttributeError:
+            pass
+
+        options._session = self
+
+        if not options.debugger_address:
+            debug_port = (
+                port
+                if port != 0
+                else selenium.webdriver.common.service.utils.free_port()
+            )
+            debug_host = "127.0.0.1"
+            options.debugger_address = "%s:%d" % (debug_host, debug_port)
+        else:
+            debug_host, debug_port = options.debugger_address.split(":")
+            debug_port = int(debug_port)
+
+        if enable_cdp_events:
+            options.set_capability(
+                "goog:loggingPrefs", {"performance": "ALL", "browser": "ALL"}
+            )
+
+        options.add_argument("--remote-debugging-host=%s" % debug_host)
+        options.add_argument("--remote-debugging-port=%s" % debug_port)
+
+        if user_data_dir:
+            options.add_argument("--user-data-dir=%s" % user_data_dir)
+
+        language, keep_user_data_dir = None, bool(user_data_dir)
+
+        # see if a custom user profile is specified in options
+        for arg in options.arguments:
+
+            if any([_ in arg for _ in ("--headless", "headless")]):
+                options.arguments.remove(arg)
+                options.headless = True
+
+            if "lang" in arg:
+                m = re.search("(?:--)?lang(?:[ =])?(.*)", arg)
+                try:
+                    language = m[1]
+                except IndexError:
+                    logger.debug("will set the language to en-US,en;q=0.9")
+                    language = "en-US,en;q=0.9"
+
+            if "user-data-dir" in arg:
+                m = re.search("(?:--)?user-data-dir(?:[ =])?(.*)", arg)
+                try:
+                    user_data_dir = m[1]
+                    logger.debug(
+                        "user-data-dir found in user argument %s => %s" % (arg, m[1])
+                    )
+                    keep_user_data_dir = True
+
+                except IndexError:
+                    logger.debug(
+                        "no user data dir could be extracted from supplied argument %s "
+                        % arg
+                    )
+
+        if not user_data_dir:
+            # backward compatiblity
+            # check if an old uc.ChromeOptions is used, and extract the user data dir
+
+            if hasattr(options, "user_data_dir") and getattr(
+                options, "user_data_dir", None
+            ):
+                import warnings
+
+                warnings.warn(
+                    "using ChromeOptions.user_data_dir might stop working in future versions."
+                    "use uc.Chrome(user_data_dir='/xyz/some/data') in case you need existing profile folder"
+                )
+                options.add_argument("--user-data-dir=%s" % options.user_data_dir)
+                keep_user_data_dir = True
+                logger.debug(
+                    "user_data_dir property found in options object: %s" % user_data_dir
+                )
+
+            else:
+                user_data_dir = os.path.normpath(tempfile.mkdtemp())
+                keep_user_data_dir = False
+                arg = "--user-data-dir=%s" % user_data_dir
+                options.add_argument(arg)
+                logger.debug(
+                    "created a temporary folder in which the user-data (profile) will be stored during this\n"
+                    "session, and added it to chrome startup arguments: %s" % arg
+                )
+
+        if not language:
+            try:
+                import locale
+
+                language = locale.getdefaultlocale()[0].replace("_", "-")
+            except Exception:
+                pass
+            if not language:
+                language = "en-US"
+
+        options.add_argument("--lang=%s" % language)
+
+        if not options.binary_location:
+            options.binary_location = (
+                browser_executable_path or find_chrome_executable()
+            )
+
+        self._delay = 3
+
+        self.user_data_dir = user_data_dir
+        self.keep_user_data_dir = keep_user_data_dir
+
+        if suppress_welcome:
+            options.arguments.extend(["--no-default-browser-check", "--no-first-run"])
+        if no_sandbox:
+            options.arguments.extend(["--no-sandbox", "--test-type"])
+
+        if headless or options.headless:
+            #workaround until a better checking is found
+            try:
+                if self.patcher.version_main < 108:
+                    options.add_argument("--headless=chrome")
+                elif self.patcher.version_main >= 108:
+                    options.add_argument("--headless=new")
+            except:
+                logger.warning("could not detect version_main."
+                               "therefore, we are assuming it is chrome 108 or higher")
+                options.add_argument("--headless=new")
+
+        options.add_argument("--window-size=1920,1080")
+        options.add_argument("--start-maximized")
+        options.add_argument("--no-sandbox")
+        # fixes "could not connect to chrome" error when running
+        # on linux using privileged user like root (which i don't recommend)
+
+        options.add_argument(
+            "--log-level=%d" % log_level
+            or divmod(logging.getLogger().getEffectiveLevel(), 10)[0]
+        )
+
+        if hasattr(options, "handle_prefs"):
+            options.handle_prefs(user_data_dir)
+
+        # fix exit_type flag to prevent tab-restore nag
+        try:
+            with open(
+                os.path.join(user_data_dir, "Default/Preferences"),
+                encoding="latin1",
+                mode="r+",
+            ) as fs:
+                config = json.load(fs)
+                if config["profile"]["exit_type"] is not None:
+                    # fixing the restore-tabs-nag
+                    config["profile"]["exit_type"] = None
+                fs.seek(0, 0)
+                json.dump(config, fs)
+                fs.truncate()  # the file might be shorter
+                logger.debug("fixed exit_type flag")
+        except Exception as e:
+            logger.debug("did not find a bad exit_type flag ")
+
+        self.options = options
+
+        if not desired_capabilities:
+            desired_capabilities = options.to_capabilities()
+
+        if not use_subprocess:
+            self.browser_pid = start_detached(
+                options.binary_location, *options.arguments
+            )
+        else:
+            browser = subprocess.Popen(
+                [options.binary_location, *options.arguments],
+                stdin=subprocess.PIPE,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                close_fds=IS_POSIX,
+            )
+            self.browser_pid = browser.pid
+
+
+        service = selenium.webdriver.chromium.service.ChromiumService(
+            self.patcher.executable_path
+        )
+
+        super(Chrome, self).__init__(
+            service=service,
+            options=options,
+            keep_alive=keep_alive,
+        )
+
+        self.reactor = None
+
+        if enable_cdp_events:
+            if logging.getLogger().getEffectiveLevel() == logging.DEBUG:
+                logging.getLogger(
+                    "selenium.webdriver.remote.remote_connection"
+                ).setLevel(20)
+            reactor = Reactor(self)
+            reactor.start()
+            self.reactor = reactor
+
+        if advanced_elements:
+            self._web_element_cls = UCWebElement
+        else:
+            self._web_element_cls = WebElement
+
+        if options.headless:
+            self._configure_headless()
+
+    def _configure_headless(self):
+        orig_get = self.get
+        logger.info("setting properties for headless")
+
+        def get_wrapped(*args, **kwargs):
+            if self.execute_script("return navigator.webdriver"):
+                logger.info("patch navigator.webdriver")
+                self.execute_cdp_cmd(
+                    "Page.addScriptToEvaluateOnNewDocument",
+                    {
+                        "source": """
+
+                           Object.defineProperty(window, "navigator", {
+                                Object.defineProperty(window, "navigator", {
+                                  value: new Proxy(navigator, {
+                                    has: (target, key) => (key === "webdriver" ? false : key in target),
+                                    get: (target, key) =>
+                                      key === "webdriver"
+                                        ? false
+                                        : typeof target[key] === "function"
+                                        ? target[key].bind(target)
+                                        : target[key],
+                                  }),
+                                });
+                    """
+                    },
+                )
+
+                logger.info("patch user-agent string")
+                self.execute_cdp_cmd(
+                    "Network.setUserAgentOverride",
+                    {
+                        "userAgent": self.execute_script(
+                            "return navigator.userAgent"
+                        ).replace("Headless", "")
+                    },
+                )
+                self.execute_cdp_cmd(
+                    "Page.addScriptToEvaluateOnNewDocument",
+                    {
+                        "source": """
+                            Object.defineProperty(navigator, 'maxTouchPoints', {get: () => 1});
+                            Object.defineProperty(navigator.connection, 'rtt', {get: () => 100});
+
+                            // https://github.com/microlinkhq/browserless/blob/master/packages/goto/src/evasions/chrome-runtime.js
+                            window.chrome = {
+                                app: {
+                                    isInstalled: false,
+                                    InstallState: {
+                                        DISABLED: 'disabled',
+                                        INSTALLED: 'installed',
+                                        NOT_INSTALLED: 'not_installed'
+                                    },
+                                    RunningState: {
+                                        CANNOT_RUN: 'cannot_run',
+                                        READY_TO_RUN: 'ready_to_run',
+                                        RUNNING: 'running'
+                                    }
+                                },
+                                runtime: {
+                                    OnInstalledReason: {
+                                        CHROME_UPDATE: 'chrome_update',
+                                        INSTALL: 'install',
+                                        SHARED_MODULE_UPDATE: 'shared_module_update',
+                                        UPDATE: 'update'
+                                    },
+                                    OnRestartRequiredReason: {
+                                        APP_UPDATE: 'app_update',
+                                        OS_UPDATE: 'os_update',
+                                        PERIODIC: 'periodic'
+                                    },
+                                    PlatformArch: {
+                                        ARM: 'arm',
+                                        ARM64: 'arm64',
+                                        MIPS: 'mips',
+                                        MIPS64: 'mips64',
+                                        X86_32: 'x86-32',
+                                        X86_64: 'x86-64'
+                                    },
+                                    PlatformNaclArch: {
+                                        ARM: 'arm',
+                                        MIPS: 'mips',
+                                        MIPS64: 'mips64',
+                                        X86_32: 'x86-32',
+                                        X86_64: 'x86-64'
+                                    },
+                                    PlatformOs: {
+                                        ANDROID: 'android',
+                                        CROS: 'cros',
+                                        LINUX: 'linux',
+                                        MAC: 'mac',
+                                        OPENBSD: 'openbsd',
+                                        WIN: 'win'
+                                    },
+                                    RequestUpdateCheckStatus: {
+                                        NO_UPDATE: 'no_update',
+                                        THROTTLED: 'throttled',
+                                        UPDATE_AVAILABLE: 'update_available'
+                                    }
+                                }
+                            }
+
+                            // https://github.com/microlinkhq/browserless/blob/master/packages/goto/src/evasions/navigator-permissions.js
+                            if (!window.Notification) {
+                                window.Notification = {
+                                    permission: 'denied'
+                                }
+                            }
+
+                            const originalQuery = window.navigator.permissions.query
+                            window.navigator.permissions.__proto__.query = parameters =>
+                                parameters.name === 'notifications'
+                                    ? Promise.resolve({ state: window.Notification.permission })
+                                    : originalQuery(parameters)
+
+                            const oldCall = Function.prototype.call
+                            function call() {
+                                return oldCall.apply(this, arguments)
+                            }
+                            Function.prototype.call = call
+
+                            const nativeToStringFunctionString = Error.toString().replace(/Error/g, 'toString')
+                            const oldToString = Function.prototype.toString
+
+                            function functionToString() {
+                                if (this === window.navigator.permissions.query) {
+                                    return 'function query() { [native code] }'
+                                }
+                                if (this === functionToString) {
+                                    return nativeToStringFunctionString
+                                }
+                                return oldCall.call(oldToString, this)
+                            }
+                            // eslint-disable-next-line
+                            Function.prototype.toString = functionToString
+                            """
+                    },
+                )
+            return orig_get(*args, **kwargs)
+
+        self.get = get_wrapped
+
+
+
+    def get(self, url):
+        # if self._get_cdc_props():
+        #     self._hook_remove_cdc_props()
+        return super().get(url)
+
+    def add_cdp_listener(self, event_name, callback):
+        if (
+            self.reactor
+            and self.reactor is not None
+            and isinstance(self.reactor, Reactor)
+        ):
+            self.reactor.add_event_handler(event_name, callback)
+            return self.reactor.handlers
+        return False
+
+    def clear_cdp_listeners(self):
+        if self.reactor and isinstance(self.reactor, Reactor):
+            self.reactor.handlers.clear()
+
+    def window_new(self):
+        self.execute(
+            selenium.webdriver.remote.command.Command.NEW_WINDOW, {"type": "window"}
+        )
+
+    def tab_new(self, url: str):
+        """
+        this opens a url in a new tab.
+        apparently, that passes all tests directly!
+
+        Parameters
+        ----------
+        url
+
+        Returns
+        -------
+
+        """
+        if not hasattr(self, "cdp"):
+            from .cdp import CDP
+
+            cdp = CDP(self.options)
+            cdp.tab_new(url)
+
+    def reconnect(self, timeout=0.1):
+        try:
+            self.service.stop()
+        except Exception as e:
+            logger.debug(e)
+        time.sleep(timeout)
+        try:
+            self.service.start()
+        except Exception as e:
+            logger.debug(e)
+
+        try:
+            self.start_session()
+        except Exception as e:
+            logger.debug(e)
+
+    def start_session(self, capabilities=None, browser_profile=None):
+        if not capabilities:
+            capabilities = self.options.to_capabilities()
+        super(selenium.webdriver.chrome.webdriver.WebDriver, self).start_session(
+            capabilities
+        )
+        # super(Chrome, self).start_session(capabilities, browser_profile)
+
+    def find_elements_recursive(self, by, value):
+        """
+        find elements in all frames
+        this is a generator function, which is needed
+            since if it would return a list of elements, they
+            will be stale on arrival.
+        using generator, when the element is returned we are in the correct frame
+        to use it directly
+        Args:
+            by: By
+            value: str
+        Returns: Generator[webelement.WebElement]
+        """
+        def search_frame(f=None):
+            if not f:
+                # ensure we are on main content frame
+                self.switch_to.default_content()
+            else:
+                self.switch_to.frame(f)
+            for elem in self.find_elements(by, value):
+                yield elem
+            # switch back to main content, otherwise we will get StaleElementReferenceException
+            self.switch_to.default_content()
+
+        # search root frame
+        for elem in search_frame():
+            yield elem
+        # get iframes
+        frames = self.find_elements('css selector', 'iframe')
+
+        # search per frame
+        for f in frames:
+            for elem in search_frame(f):
+                yield elem
+
+    def quit(self):
+        try:
+            self.service.process.kill()
+            logger.debug("webdriver process ended")
+        except (AttributeError, RuntimeError, OSError):
+            pass
+        try:
+            self.reactor.event.set()
+            logger.debug("shutting down reactor")
+        except AttributeError:
+            pass
+        try:
+            os.kill(self.browser_pid, 15)
+            logger.debug("gracefully closed browser")
+        except Exception as e:  # noqa
+            pass
+        if (
+            hasattr(self, "keep_user_data_dir")
+            and hasattr(self, "user_data_dir")
+            and not self.keep_user_data_dir
+        ):
+            for _ in range(5):
+                try:
+                    shutil.rmtree(self.user_data_dir, ignore_errors=False)
+                except FileNotFoundError:
+                    pass
+                except (RuntimeError, OSError, PermissionError) as e:
+                    logger.debug(
+                        "When removing the temp profile, a %s occured: %s\nretrying..."
+                        % (e.__class__.__name__, e)
+                    )
+                else:
+                    logger.debug("successfully removed %s" % self.user_data_dir)
+                    break
+                time.sleep(0.1)
+
+        # dereference patcher, so patcher can start cleaning up as well.
+        # this must come last, otherwise it will throw 'in use' errors
+        self.patcher = None
+
+    def __getattribute__(self, item):
+        if not super().__getattribute__("debug"):
+            return super().__getattribute__(item)
+        else:
+            import inspect
+
+            original = super().__getattribute__(item)
+            if inspect.ismethod(original) and not inspect.isclass(original):
+
+                def newfunc(*args, **kwargs):
+                    logger.debug(
+                        "calling %s with args %s and kwargs %s\n"
+                        % (original.__qualname__, args, kwargs)
+                    )
+                    return original(*args, **kwargs)
+
+                return newfunc
+            return original
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.service.stop()
+        time.sleep(self._delay)
+        self.service.start()
+        self.start_session()
+
+    def __hash__(self):
+        return hash(self.options.debugger_address)
+
+    def __dir__(self):
+        return object.__dir__(self)
+
+    def __del__(self):
+        try:
+            self.service.process.kill()
+        except:  # noqa
+            pass
+        self.quit()
+
+    @classmethod
+    def _ensure_close(cls, self):
+        # needs to be a classmethod so finalize can find the reference
+        logger.info("ensuring close")
+        if (
+            hasattr(self, "service")
+            and hasattr(self.service, "process")
+            and hasattr(self.service.process, "kill")
+        ):
+            self.service.process.kill()
+
+
+def find_chrome_executable():
+    """
+    Finds the chrome, chrome beta, chrome canary, chromium executable
+
+    Returns
+    -------
+    executable_path :  str
+        the full file path to found executable
+
+    """
+    candidates = set()
+    if IS_POSIX:
+        for item in os.environ.get("PATH").split(os.pathsep):
+            for subitem in (
+                "google-chrome",
+                "chromium",
+                "chromium-browser",
+                "chrome",
+                "google-chrome-stable",
+            ):
+                candidates.add(os.sep.join((item, subitem)))
+        if "darwin" in sys.platform:
+            candidates.update(
+                [
+                    "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
+                    "/Applications/Chromium.app/Contents/MacOS/Chromium",
+                ]
+            )
+    else:
+        for item in map(
+            os.environ.get,
+            ("PROGRAMFILES", "PROGRAMFILES(X86)", "LOCALAPPDATA", "PROGRAMW6432"),
+        ):
+            if item is not None:
+                for subitem in (
+                    "Google/Chrome/Application",
+                    "Google/Chrome Beta/Application",
+                    "Google/Chrome Canary/Application",
+                ):
+                    candidates.add(os.sep.join((item, subitem, "chrome.exe")))
+    for candidate in candidates:
+        logger.debug('checking if %s exists and is executable' % candidate)
+        if os.path.exists(candidate) and os.access(candidate, os.X_OK):
+            logger.debug('found! using %s' % candidate)
+            return os.path.normpath(candidate)
```

### Comparing `undetected-chromedriver-3.4.7/undetected_chromedriver/cdp.py` & `undetected-chromedriver-3.5.0/undetected_chromedriver/cdp.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-#!/usr/bin/env python3
-# this module is part of undetected_chromedriver
-
-import json
-import logging
-
-import requests
-import websockets
-
-
-log = logging.getLogger(__name__)
-
-
-class CDPObject(dict):
-    def __init__(self, *a, **k):
-        super().__init__(*a, **k)
-        self.__dict__ = self
-        for k in self.__dict__:
-            if isinstance(self.__dict__[k], dict):
-                self.__dict__[k] = CDPObject(self.__dict__[k])
-            elif isinstance(self.__dict__[k], list):
-                for i in range(len(self.__dict__[k])):
-                    if isinstance(self.__dict__[k][i], dict):
-                        self.__dict__[k][i] = CDPObject(self)
-
-    def __repr__(self):
-        tpl = f"{self.__class__.__name__}(\n\t{{}}\n\t)"
-        return tpl.format("\n  ".join(f"{k} = {v}" for k, v in self.items()))
-
-
-class PageElement(CDPObject):
-    pass
-
-
-class CDP:
-    log = logging.getLogger("CDP")
-
-    endpoints = CDPObject(
-        {
-            "json": "/json",
-            "protocol": "/json/protocol",
-            "list": "/json/list",
-            "new": "/json/new?{url}",
-            "activate": "/json/activate/{id}",
-            "close": "/json/close/{id}",
-        }
-    )
-
-    def __init__(self, options: "ChromeOptions"):  # noqa
-        self.server_addr = "http://{0}:{1}".format(*options.debugger_address.split(":"))
-
-        self._reqid = 0
-        self._session = requests.Session()
-        self._last_resp = None
-        self._last_json = None
-
-        resp = self.get(self.endpoints.json)  # noqa
-        self.sessionId = resp[0]["id"]
-        self.wsurl = resp[0]["webSocketDebuggerUrl"]
-
-    def tab_activate(self, id=None):
-        if not id:
-            active_tab = self.tab_list()[0]
-            id = active_tab.id  # noqa
-            self.wsurl = active_tab.webSocketDebuggerUrl  # noqa
-        return self.post(self.endpoints["activate"].format(id=id))
-
-    def tab_list(self):
-        retval = self.get(self.endpoints["list"])
-        return [PageElement(o) for o in retval]
-
-    def tab_new(self, url):
-        return self.post(self.endpoints["new"].format(url=url))
-
-    def tab_close_last_opened(self):
-        sessions = self.tab_list()
-        opentabs = [s for s in sessions if s["type"] == "page"]
-        return self.post(self.endpoints["close"].format(id=opentabs[-1]["id"]))
-
-    async def send(self, method: str, params: dict):
-        self._reqid += 1
-        async with websockets.connect(self.wsurl) as ws:
-            await ws.send(
-                json.dumps({"method": method, "params": params, "id": self._reqid})
-            )
-            self._last_resp = await ws.recv()
-            self._last_json = json.loads(self._last_resp)
-            self.log.info(self._last_json)
-
-    def get(self, uri):
-        resp = self._session.get(self.server_addr + uri)
-        try:
-            self._last_resp = resp
-            self._last_json = resp.json()
-        except Exception:
-            return
-        else:
-            return self._last_json
-
-    def post(self, uri, data: dict = None):
-        if not data:
-            data = {}
-        resp = self._session.post(self.server_addr + uri, json=data)
-        try:
-            self._last_resp = resp
-            self._last_json = resp.json()
-        except Exception:
-            return self._last_resp
-
-    @property
-    def last_json(self):
-        return self._last_json
+#!/usr/bin/env python3
+# this module is part of undetected_chromedriver
+
+import json
+import logging
+
+import requests
+import websockets
+
+
+log = logging.getLogger(__name__)
+
+
+class CDPObject(dict):
+    def __init__(self, *a, **k):
+        super().__init__(*a, **k)
+        self.__dict__ = self
+        for k in self.__dict__:
+            if isinstance(self.__dict__[k], dict):
+                self.__dict__[k] = CDPObject(self.__dict__[k])
+            elif isinstance(self.__dict__[k], list):
+                for i in range(len(self.__dict__[k])):
+                    if isinstance(self.__dict__[k][i], dict):
+                        self.__dict__[k][i] = CDPObject(self)
+
+    def __repr__(self):
+        tpl = f"{self.__class__.__name__}(\n\t{{}}\n\t)"
+        return tpl.format("\n  ".join(f"{k} = {v}" for k, v in self.items()))
+
+
+class PageElement(CDPObject):
+    pass
+
+
+class CDP:
+    log = logging.getLogger("CDP")
+
+    endpoints = CDPObject(
+        {
+            "json": "/json",
+            "protocol": "/json/protocol",
+            "list": "/json/list",
+            "new": "/json/new?{url}",
+            "activate": "/json/activate/{id}",
+            "close": "/json/close/{id}",
+        }
+    )
+
+    def __init__(self, options: "ChromeOptions"):  # noqa
+        self.server_addr = "http://{0}:{1}".format(*options.debugger_address.split(":"))
+
+        self._reqid = 0
+        self._session = requests.Session()
+        self._last_resp = None
+        self._last_json = None
+
+        resp = self.get(self.endpoints.json)  # noqa
+        self.sessionId = resp[0]["id"]
+        self.wsurl = resp[0]["webSocketDebuggerUrl"]
+
+    def tab_activate(self, id=None):
+        if not id:
+            active_tab = self.tab_list()[0]
+            id = active_tab.id  # noqa
+            self.wsurl = active_tab.webSocketDebuggerUrl  # noqa
+        return self.post(self.endpoints["activate"].format(id=id))
+
+    def tab_list(self):
+        retval = self.get(self.endpoints["list"])
+        return [PageElement(o) for o in retval]
+
+    def tab_new(self, url):
+        return self.post(self.endpoints["new"].format(url=url))
+
+    def tab_close_last_opened(self):
+        sessions = self.tab_list()
+        opentabs = [s for s in sessions if s["type"] == "page"]
+        return self.post(self.endpoints["close"].format(id=opentabs[-1]["id"]))
+
+    async def send(self, method: str, params: dict):
+        self._reqid += 1
+        async with websockets.connect(self.wsurl) as ws:
+            await ws.send(
+                json.dumps({"method": method, "params": params, "id": self._reqid})
+            )
+            self._last_resp = await ws.recv()
+            self._last_json = json.loads(self._last_resp)
+            self.log.info(self._last_json)
+
+    def get(self, uri):
+        resp = self._session.get(self.server_addr + uri)
+        try:
+            self._last_resp = resp
+            self._last_json = resp.json()
+        except Exception:
+            return
+        else:
+            return self._last_json
+
+    def post(self, uri, data: dict = None):
+        if not data:
+            data = {}
+        resp = self._session.post(self.server_addr + uri, json=data)
+        try:
+            self._last_resp = resp
+            self._last_json = resp.json()
+        except Exception:
+            return self._last_resp
+
+    @property
+    def last_json(self):
+        return self._last_json
```

### Comparing `undetected-chromedriver-3.4.7/undetected_chromedriver/dprocess.py` & `undetected-chromedriver-3.5.0/undetected_chromedriver/dprocess.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-import atexit
-import logging
-import multiprocessing
-import os
-import platform
-import signal
-from subprocess import PIPE
-from subprocess import Popen
-import sys
-
-
-CREATE_NEW_PROCESS_GROUP = 0x00000200
-DETACHED_PROCESS = 0x00000008
-
-REGISTERED = []
-
-
-def start_detached(executable, *args):
-    """
-    Starts a fully independent subprocess (with no parent)
-    :param executable: executable
-    :param args: arguments to the executable, eg: ['--param1_key=param1_val', '-vvv' ...]
-    :return: pid of the grandchild process
-    """
-
-    # create pipe
-    reader, writer = multiprocessing.Pipe(False)
-
-    # do not keep reference
-    multiprocessing.Process(
-        target=_start_detached,
-        args=(executable, *args),
-        kwargs={"writer": writer},
-        daemon=True,
-    ).start()
-    # receive pid from pipe
-    pid = reader.recv()
-    REGISTERED.append(pid)
-    # close pipes
-    writer.close()
-    reader.close()
-
-    return pid
-
-
-def _start_detached(executable, *args, writer: multiprocessing.Pipe = None):
-    # configure launch
-    kwargs = {}
-    if platform.system() == "Windows":
-        kwargs.update(creationflags=DETACHED_PROCESS | CREATE_NEW_PROCESS_GROUP)
-    elif sys.version_info < (3, 2):
-        # assume posix
-        kwargs.update(preexec_fn=os.setsid)
-    else:  # Python 3.2+ and Unix
-        kwargs.update(start_new_session=True)
-
-    # run
-    p = Popen([executable, *args], stdin=PIPE, stdout=PIPE, stderr=PIPE, **kwargs)
-
-    # send pid to pipe
-    writer.send(p.pid)
-    sys.exit()
-
-
-def _cleanup():
-    for pid in REGISTERED:
-        try:
-            logging.getLogger(__name__).debug("cleaning up pid %d " % pid)
-            os.kill(pid, signal.SIGTERM)
-        except:  # noqa
-            pass
-
-
-atexit.register(_cleanup)
+import atexit
+import logging
+import multiprocessing
+import os
+import platform
+import signal
+from subprocess import PIPE
+from subprocess import Popen
+import sys
+
+
+CREATE_NEW_PROCESS_GROUP = 0x00000200
+DETACHED_PROCESS = 0x00000008
+
+REGISTERED = []
+
+
+def start_detached(executable, *args):
+    """
+    Starts a fully independent subprocess (with no parent)
+    :param executable: executable
+    :param args: arguments to the executable, eg: ['--param1_key=param1_val', '-vvv' ...]
+    :return: pid of the grandchild process
+    """
+
+    # create pipe
+    reader, writer = multiprocessing.Pipe(False)
+
+    # do not keep reference
+    multiprocessing.Process(
+        target=_start_detached,
+        args=(executable, *args),
+        kwargs={"writer": writer},
+        daemon=True,
+    ).start()
+    # receive pid from pipe
+    pid = reader.recv()
+    REGISTERED.append(pid)
+    # close pipes
+    writer.close()
+    reader.close()
+
+    return pid
+
+
+def _start_detached(executable, *args, writer: multiprocessing.Pipe = None):
+    # configure launch
+    kwargs = {}
+    if platform.system() == "Windows":
+        kwargs.update(creationflags=DETACHED_PROCESS | CREATE_NEW_PROCESS_GROUP)
+    elif sys.version_info < (3, 2):
+        # assume posix
+        kwargs.update(preexec_fn=os.setsid)
+    else:  # Python 3.2+ and Unix
+        kwargs.update(start_new_session=True)
+
+    # run
+    p = Popen([executable, *args], stdin=PIPE, stdout=PIPE, stderr=PIPE, **kwargs)
+
+    # send pid to pipe
+    writer.send(p.pid)
+    sys.exit()
+
+
+def _cleanup():
+    for pid in REGISTERED:
+        try:
+            logging.getLogger(__name__).debug("cleaning up pid %d " % pid)
+            os.kill(pid, signal.SIGTERM)
+        except:  # noqa
+            pass
+
+
+atexit.register(_cleanup)
```

### Comparing `undetected-chromedriver-3.4.7/undetected_chromedriver/patcher.py` & `undetected-chromedriver-3.5.0/undetected_chromedriver/patcher.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,348 +1,348 @@
-#!/usr/bin/env python3
-# this module is part of undetected_chromedriver
-
-from distutils.version import LooseVersion
-import io
-import logging
-import os
-import pathlib
-import random
-import re
-import shutil
-import string
-import sys
-import time
-from urllib.request import urlopen
-from urllib.request import urlretrieve
-import zipfile
-from multiprocessing import Lock
-
-logger = logging.getLogger(__name__)
-
-IS_POSIX = sys.platform.startswith(("darwin", "cygwin", "linux", "linux2"))
-
-
-class Patcher(object):
-    lock = Lock()
-    url_repo = "https://chromedriver.storage.googleapis.com"
-    zip_name = "chromedriver_%s.zip"
-    exe_name = "chromedriver%s"
-
-    platform = sys.platform
-    if platform.endswith("win32"):
-        zip_name %= "win32"
-        exe_name %= ".exe"
-    if platform.endswith(("linux", "linux2")):
-        zip_name %= "linux64"
-        exe_name %= ""
-    if platform.endswith("darwin"):
-        zip_name %= "mac64"
-        exe_name %= ""
-
-    if platform.endswith("win32"):
-        d = "~/appdata/roaming/undetected_chromedriver"
-    elif "LAMBDA_TASK_ROOT" in os.environ:
-        d = "/tmp/undetected_chromedriver"
-    elif platform.startswith(("linux", "linux2")):
-        d = "~/.local/share/undetected_chromedriver"
-    elif platform.endswith("darwin"):
-        d = "~/Library/Application Support/undetected_chromedriver"
-    else:
-        d = "~/.undetected_chromedriver"
-    data_path = os.path.abspath(os.path.expanduser(d))
-
-    def __init__(
-        self,
-        executable_path=None,
-        force=False,
-        version_main: int = 0,
-        user_multi_procs=False,
-    ):
-        """
-        Args:
-            executable_path: None = automatic
-                             a full file path to the chromedriver executable
-            force: False
-                    terminate processes which are holding lock
-            version_main: 0 = auto
-                specify main chrome version (rounded, ex: 82)
-        """
-        self.force = force
-        self._custom_exe_path = False
-        prefix = "undetected"
-        self.user_multi_procs = user_multi_procs
-
-        if not os.path.exists(self.data_path):
-            os.makedirs(self.data_path, exist_ok=True)
-
-        if not executable_path:
-            self.executable_path = os.path.join(
-                self.data_path, "_".join([prefix, self.exe_name])
-            )
-
-        if not IS_POSIX:
-            if executable_path:
-                if not executable_path[-4:] == ".exe":
-                    executable_path += ".exe"
-
-        self.zip_path = os.path.join(self.data_path, prefix)
-
-        if not executable_path:
-            if not self.user_multi_procs:
-                self.executable_path = os.path.abspath(
-                    os.path.join(".", self.executable_path)
-                )
-
-        if executable_path:
-            self._custom_exe_path = True
-            self.executable_path = executable_path
-
-        self.version_main = version_main
-        self.version_full = None
-
-    def auto(self, executable_path=None, force=False, version_main=None, _=None):
-        """
-
-        Args:
-            executable_path:
-            force:
-            version_main:
-
-        Returns:
-
-        """
-        # if self.user_multi_procs and \
-        #         self.user_multi_procs != -1:
-        #     # -1 being a skip value used later in this block
-        #
-        p = pathlib.Path(self.data_path)
-        with Lock():
-            files = list(p.rglob("*chromedriver*?"))
-            for file in files:
-                if self.is_binary_patched(file):
-                    self.executable_path = str(file)
-                    return True
-
-        if executable_path:
-            self.executable_path = executable_path
-            self._custom_exe_path = True
-
-        if self._custom_exe_path:
-            ispatched = self.is_binary_patched(self.executable_path)
-            if not ispatched:
-                return self.patch_exe()
-            else:
-                return
-
-        if version_main:
-            self.version_main = version_main
-        if force is True:
-            self.force = force
-
-        try:
-            os.unlink(self.executable_path)
-        except PermissionError:
-            if self.force:
-                self.force_kill_instances(self.executable_path)
-                return self.auto(force=not self.force)
-            try:
-                if self.is_binary_patched():
-                    # assumes already running AND patched
-                    return True
-            except PermissionError:
-                pass
-            # return False
-        except FileNotFoundError:
-            pass
-
-        release = self.fetch_release_number()
-        self.version_main = release.version[0]
-        self.version_full = release
-        self.unzip_package(self.fetch_package())
-        return self.patch()
-
-    def driver_binary_in_use(self, path: str = None) -> bool:
-        """
-        naive test to check if a found chromedriver binary is
-        currently in use
-
-        Args:
-            path: a string or PathLike object to the binary to check.
-                  if not specified, we check use this object's executable_path
-        """
-        if not path:
-            path = self.executable_path
-        p = pathlib.Path(path)
-
-        if not p.exists():
-            raise OSError("file does not exist: %s" % p)
-        try:
-            with open(p, mode="a+b") as fs:
-                exc = []
-                try:
-
-                    fs.seek(0, 0)
-                except PermissionError as e:
-                    exc.append(e)  # since some systems apprently allow seeking
-                    # we conduct another test
-                try:
-                    fs.readline()
-                except PermissionError as e:
-                    exc.append(e)
-
-                if exc:
-
-                    return True
-                return False
-            # ok safe to assume this is in use
-        except Exception as e:
-            # logger.exception("whoops ", e)
-            pass
-
-    def cleanup_unused_files(self):
-        p = pathlib.Path(self.data_path)
-        items = list(p.glob("*undetected*"))
-        print(items)
-
-    def patch(self):
-        self.patch_exe()
-        return self.is_binary_patched()
-
-    def fetch_release_number(self):
-        """
-        Gets the latest major version available, or the latest major version of self.target_version if set explicitly.
-        :return: version string
-        :rtype: LooseVersion
-        """
-        path = "/latest_release"
-        if self.version_main:
-            path += f"_{self.version_main}"
-        path = path.upper()
-        logger.debug("getting release number from %s" % path)
-        return LooseVersion(urlopen(self.url_repo + path).read().decode())
-
-    def parse_exe_version(self):
-        with io.open(self.executable_path, "rb") as f:
-            for line in iter(lambda: f.readline(), b""):
-                match = re.search(rb"platform_handle\x00content\x00([0-9.]*)", line)
-                if match:
-                    return LooseVersion(match[1].decode())
-
-    def fetch_package(self):
-        """
-        Downloads ChromeDriver from source
-
-        :return: path to downloaded file
-        """
-        u = "%s/%s/%s" % (self.url_repo, self.version_full.vstring, self.zip_name)
-        logger.debug("downloading from %s" % u)
-        # return urlretrieve(u, filename=self.data_path)[0]
-        return urlretrieve(u)[0]
-
-    def unzip_package(self, fp):
-        """
-        Does what it says
-
-        :return: path to unpacked executable
-        """
-        logger.debug("unzipping %s" % fp)
-        try:
-            os.unlink(self.zip_path)
-        except (FileNotFoundError, OSError):
-            pass
-
-        os.makedirs(self.zip_path, mode=0o755, exist_ok=True)
-        with zipfile.ZipFile(fp, mode="r") as zf:
-            zf.extract(self.exe_name, self.zip_path)
-        os.rename(os.path.join(self.zip_path, self.exe_name), self.executable_path)
-        os.remove(fp)
-        os.rmdir(self.zip_path)
-        os.chmod(self.executable_path, 0o755)
-        return self.executable_path
-
-    @staticmethod
-    def force_kill_instances(exe_name):
-        """
-        kills running instances.
-        :param: executable name to kill, may be a path as well
-
-        :return: True on success else False
-        """
-        exe_name = os.path.basename(exe_name)
-        if IS_POSIX:
-            r = os.system("kill -f -9 $(pidof %s)" % exe_name)
-        else:
-            r = os.system("taskkill /f /im %s" % exe_name)
-        return not r
-
-    @staticmethod
-    def gen_random_cdc():
-        cdc = random.choices(string.ascii_letters, k=27)
-        return "".join(cdc).encode()
-
-    def is_binary_patched(self, executable_path=None):
-        executable_path = executable_path or self.executable_path
-        try:
-            with io.open(executable_path, "rb") as fh:
-                return fh.read().find(b"undetected chromedriver") != -1
-        except FileNotFoundError:
-            return False
-
-    def patch_exe(self):
-        start = time.perf_counter()
-        logger.info("patching driver executable %s" % self.executable_path)
-        with io.open(self.executable_path, "r+b") as fh:
-            content = fh.read()
-            # match_injected_codeblock = re.search(rb"{window.*;}", content)
-            match_injected_codeblock = re.search(rb"\{window\.cdc.*?;\}", content)
-            if match_injected_codeblock:
-                target_bytes = match_injected_codeblock[0]
-                new_target_bytes = (
-                    b'{console.log("undetected chromedriver 1337!")}'.ljust(
-                        len(target_bytes), b" "
-                    )
-                )
-                new_content = content.replace(target_bytes, new_target_bytes)
-                if new_content == content:
-                    logger.warning(
-                        "something went wrong patching the driver binary. could not find injection code block"
-                    )
-                else:
-                    logger.debug(
-                        "found block:\n%s\nreplacing with:\n%s"
-                        % (target_bytes, new_target_bytes)
-                    )
-                fh.seek(0)
-                fh.write(new_content)
-        logger.debug(
-            "patching took us {:.2f} seconds".format(time.perf_counter() - start)
-        )
-
-    def __repr__(self):
-        return "{0:s}({1:s})".format(
-            self.__class__.__name__,
-            self.executable_path,
-        )
-
-    def __del__(self):
-        if self._custom_exe_path:
-            # if the driver binary is specified by user
-            # we assume it is important enough to not delete it
-            return
-        else:
-            timeout = 3  # stop trying after this many seconds
-            t = time.monotonic()
-            now = lambda: time.monotonic()
-            while now() - t > timeout:
-                # we don't want to wait until the end of time
-                try:
-                    if self.user_multi_procs:
-                        break
-                    os.unlink(self.executable_path)
-                    logger.debug("successfully unlinked %s" % self.executable_path)
-                    break
-                except (OSError, RuntimeError, PermissionError):
-                    time.sleep(0.01)
-                    continue
-                except FileNotFoundError:
-                    break
+#!/usr/bin/env python3
+# this module is part of undetected_chromedriver
+
+from distutils.version import LooseVersion
+import io
+import logging
+import os
+import pathlib
+import random
+import re
+import shutil
+import string
+import sys
+import time
+from urllib.request import urlopen
+from urllib.request import urlretrieve
+import zipfile
+from multiprocessing import Lock
+
+logger = logging.getLogger(__name__)
+
+IS_POSIX = sys.platform.startswith(("darwin", "cygwin", "linux", "linux2"))
+
+
+class Patcher(object):
+    lock = Lock()
+    url_repo = "https://chromedriver.storage.googleapis.com"
+    zip_name = "chromedriver_%s.zip"
+    exe_name = "chromedriver%s"
+
+    platform = sys.platform
+    if platform.endswith("win32"):
+        zip_name %= "win32"
+        exe_name %= ".exe"
+    if platform.endswith(("linux", "linux2")):
+        zip_name %= "linux64"
+        exe_name %= ""
+    if platform.endswith("darwin"):
+        zip_name %= "mac64"
+        exe_name %= ""
+
+    if platform.endswith("win32"):
+        d = "~/appdata/roaming/undetected_chromedriver"
+    elif "LAMBDA_TASK_ROOT" in os.environ:
+        d = "/tmp/undetected_chromedriver"
+    elif platform.startswith(("linux", "linux2")):
+        d = "~/.local/share/undetected_chromedriver"
+    elif platform.endswith("darwin"):
+        d = "~/Library/Application Support/undetected_chromedriver"
+    else:
+        d = "~/.undetected_chromedriver"
+    data_path = os.path.abspath(os.path.expanduser(d))
+
+    def __init__(
+        self,
+        executable_path=None,
+        force=False,
+        version_main: int = 0,
+        user_multi_procs=False,
+    ):
+        """
+        Args:
+            executable_path: None = automatic
+                             a full file path to the chromedriver executable
+            force: False
+                    terminate processes which are holding lock
+            version_main: 0 = auto
+                specify main chrome version (rounded, ex: 82)
+        """
+        self.force = force
+        self._custom_exe_path = False
+        prefix = "undetected"
+        self.user_multi_procs = user_multi_procs
+
+        if not os.path.exists(self.data_path):
+            os.makedirs(self.data_path, exist_ok=True)
+
+        if not executable_path:
+            self.executable_path = os.path.join(
+                self.data_path, "_".join([prefix, self.exe_name])
+            )
+
+        if not IS_POSIX:
+            if executable_path:
+                if not executable_path[-4:] == ".exe":
+                    executable_path += ".exe"
+
+        self.zip_path = os.path.join(self.data_path, prefix)
+
+        if not executable_path:
+            if not self.user_multi_procs:
+                self.executable_path = os.path.abspath(
+                    os.path.join(".", self.executable_path)
+                )
+
+        if executable_path:
+            self._custom_exe_path = True
+            self.executable_path = executable_path
+
+        self.version_main = version_main
+        self.version_full = None
+
+    def auto(self, executable_path=None, force=False, version_main=None, _=None):
+        """
+
+        Args:
+            executable_path:
+            force:
+            version_main:
+
+        Returns:
+
+        """
+        # if self.user_multi_procs and \
+        #         self.user_multi_procs != -1:
+        #     # -1 being a skip value used later in this block
+        #
+        p = pathlib.Path(self.data_path)
+        with Lock():
+            files = list(p.rglob("*chromedriver*?"))
+            for file in files:
+                if self.is_binary_patched(file):
+                    self.executable_path = str(file)
+                    return True
+
+        if executable_path:
+            self.executable_path = executable_path
+            self._custom_exe_path = True
+
+        if self._custom_exe_path:
+            ispatched = self.is_binary_patched(self.executable_path)
+            if not ispatched:
+                return self.patch_exe()
+            else:
+                return
+
+        if version_main:
+            self.version_main = version_main
+        if force is True:
+            self.force = force
+
+        try:
+            os.unlink(self.executable_path)
+        except PermissionError:
+            if self.force:
+                self.force_kill_instances(self.executable_path)
+                return self.auto(force=not self.force)
+            try:
+                if self.is_binary_patched():
+                    # assumes already running AND patched
+                    return True
+            except PermissionError:
+                pass
+            # return False
+        except FileNotFoundError:
+            pass
+
+        release = self.fetch_release_number()
+        self.version_main = release.version[0]
+        self.version_full = release
+        self.unzip_package(self.fetch_package())
+        return self.patch()
+
+    def driver_binary_in_use(self, path: str = None) -> bool:
+        """
+        naive test to check if a found chromedriver binary is
+        currently in use
+
+        Args:
+            path: a string or PathLike object to the binary to check.
+                  if not specified, we check use this object's executable_path
+        """
+        if not path:
+            path = self.executable_path
+        p = pathlib.Path(path)
+
+        if not p.exists():
+            raise OSError("file does not exist: %s" % p)
+        try:
+            with open(p, mode="a+b") as fs:
+                exc = []
+                try:
+
+                    fs.seek(0, 0)
+                except PermissionError as e:
+                    exc.append(e)  # since some systems apprently allow seeking
+                    # we conduct another test
+                try:
+                    fs.readline()
+                except PermissionError as e:
+                    exc.append(e)
+
+                if exc:
+
+                    return True
+                return False
+            # ok safe to assume this is in use
+        except Exception as e:
+            # logger.exception("whoops ", e)
+            pass
+
+    def cleanup_unused_files(self):
+        p = pathlib.Path(self.data_path)
+        items = list(p.glob("*undetected*"))
+        print(items)
+
+    def patch(self):
+        self.patch_exe()
+        return self.is_binary_patched()
+
+    def fetch_release_number(self):
+        """
+        Gets the latest major version available, or the latest major version of self.target_version if set explicitly.
+        :return: version string
+        :rtype: LooseVersion
+        """
+        path = "/latest_release"
+        if self.version_main:
+            path += f"_{self.version_main}"
+        path = path.upper()
+        logger.debug("getting release number from %s" % path)
+        return LooseVersion(urlopen(self.url_repo + path).read().decode())
+
+    def parse_exe_version(self):
+        with io.open(self.executable_path, "rb") as f:
+            for line in iter(lambda: f.readline(), b""):
+                match = re.search(rb"platform_handle\x00content\x00([0-9.]*)", line)
+                if match:
+                    return LooseVersion(match[1].decode())
+
+    def fetch_package(self):
+        """
+        Downloads ChromeDriver from source
+
+        :return: path to downloaded file
+        """
+        u = "%s/%s/%s" % (self.url_repo, self.version_full.vstring, self.zip_name)
+        logger.debug("downloading from %s" % u)
+        # return urlretrieve(u, filename=self.data_path)[0]
+        return urlretrieve(u)[0]
+
+    def unzip_package(self, fp):
+        """
+        Does what it says
+
+        :return: path to unpacked executable
+        """
+        logger.debug("unzipping %s" % fp)
+        try:
+            os.unlink(self.zip_path)
+        except (FileNotFoundError, OSError):
+            pass
+
+        os.makedirs(self.zip_path, mode=0o755, exist_ok=True)
+        with zipfile.ZipFile(fp, mode="r") as zf:
+            zf.extract(self.exe_name, self.zip_path)
+        os.rename(os.path.join(self.zip_path, self.exe_name), self.executable_path)
+        os.remove(fp)
+        os.rmdir(self.zip_path)
+        os.chmod(self.executable_path, 0o755)
+        return self.executable_path
+
+    @staticmethod
+    def force_kill_instances(exe_name):
+        """
+        kills running instances.
+        :param: executable name to kill, may be a path as well
+
+        :return: True on success else False
+        """
+        exe_name = os.path.basename(exe_name)
+        if IS_POSIX:
+            r = os.system("kill -f -9 $(pidof %s)" % exe_name)
+        else:
+            r = os.system("taskkill /f /im %s" % exe_name)
+        return not r
+
+    @staticmethod
+    def gen_random_cdc():
+        cdc = random.choices(string.ascii_letters, k=27)
+        return "".join(cdc).encode()
+
+    def is_binary_patched(self, executable_path=None):
+        executable_path = executable_path or self.executable_path
+        try:
+            with io.open(executable_path, "rb") as fh:
+                return fh.read().find(b"undetected chromedriver") != -1
+        except FileNotFoundError:
+            return False
+
+    def patch_exe(self):
+        start = time.perf_counter()
+        logger.info("patching driver executable %s" % self.executable_path)
+        with io.open(self.executable_path, "r+b") as fh:
+            content = fh.read()
+            # match_injected_codeblock = re.search(rb"{window.*;}", content)
+            match_injected_codeblock = re.search(rb"\{window\.cdc.*?;\}", content)
+            if match_injected_codeblock:
+                target_bytes = match_injected_codeblock[0]
+                new_target_bytes = (
+                    b'{console.log("undetected chromedriver 1337!")}'.ljust(
+                        len(target_bytes), b" "
+                    )
+                )
+                new_content = content.replace(target_bytes, new_target_bytes)
+                if new_content == content:
+                    logger.warning(
+                        "something went wrong patching the driver binary. could not find injection code block"
+                    )
+                else:
+                    logger.debug(
+                        "found block:\n%s\nreplacing with:\n%s"
+                        % (target_bytes, new_target_bytes)
+                    )
+                fh.seek(0)
+                fh.write(new_content)
+        logger.debug(
+            "patching took us {:.2f} seconds".format(time.perf_counter() - start)
+        )
+
+    def __repr__(self):
+        return "{0:s}({1:s})".format(
+            self.__class__.__name__,
+            self.executable_path,
+        )
+
+    def __del__(self):
+        if self._custom_exe_path:
+            # if the driver binary is specified by user
+            # we assume it is important enough to not delete it
+            return
+        else:
+            timeout = 3  # stop trying after this many seconds
+            t = time.monotonic()
+            now = lambda: time.monotonic()
+            while now() - t > timeout:
+                # we don't want to wait until the end of time
+                try:
+                    if self.user_multi_procs:
+                        break
+                    os.unlink(self.executable_path)
+                    logger.debug("successfully unlinked %s" % self.executable_path)
+                    break
+                except (OSError, RuntimeError, PermissionError):
+                    time.sleep(0.01)
+                    continue
+                except FileNotFoundError:
+                    break
```

### Comparing `undetected-chromedriver-3.4.7/undetected_chromedriver/webelement.py` & `undetected-chromedriver-3.5.0/undetected_chromedriver/webelement.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from typing import List
-
-from selenium.webdriver.common.by import By
-import selenium.webdriver.remote.webelement
-
-
-class WebElement(selenium.webdriver.remote.webelement.WebElement):
-    def click_safe(self):
-        super().click()
-        self._parent.reconnect(0.1)
-
-    def children(
-        self, tag=None, recursive=False
-    ) -> List[selenium.webdriver.remote.webelement.WebElement]:
-        """
-        returns direct child elements of current element
-        :param tag: str,  if supplied, returns <tag> nodes only
-        """
-        script = "return [... arguments[0].children]"
-        if tag:
-            script += ".filter( node => node.tagName === '%s')" % tag.upper()
-        if recursive:
-            return list(_recursive_children(self, tag))
-        return list(self._parent.execute_script(script, self))
-
-
-class UCWebElement(WebElement):
-    """
-    Custom WebElement class which makes it easier to view elements when
-    working in an interactive environment.
-
-    standard webelement repr:
-    <selenium.webdriver.remote.webelement.WebElement (session="85ff0f671512fa535630e71ee951b1f2", element="6357cb55-92c3-4c0f-9416-b174f9c1b8c4")>
-
-    using this WebElement class:
-    <WebElement(<a class="mobile-show-inline-block mc-update-infos init-ok" href="#" id="main-cat-switcher-mobile">)>
-
-    """
-
-    def __init__(self, parent, id_):
-        super().__init__(parent, id_)
-        self._attrs = None
-
-    @property
-    def attrs(self):
-        if not self._attrs:
-            self._attrs = self._parent.execute_script(
-                """
-                var items = {}; 
-                for (index = 0; index < arguments[0].attributes.length; ++index) 
-                {
-                 items[arguments[0].attributes[index].name] = arguments[0].attributes[index].value 
-                }; 
-                return items;
-                """,
-                self,
-            )
-        return self._attrs
-
-    def __repr__(self):
-        strattrs = " ".join([f'{k}="{v}"' for k, v in self.attrs.items()])
-        if strattrs:
-            strattrs = " " + strattrs
-        return f"{self.__class__.__name__} <{self.tag_name}{strattrs}>"
-
-
-def _recursive_children(element, tag: str = None, _results=None):
-    """
-    returns all children of <element> recursively
-
-    :param element: `WebElement` object.
-            find children below this <element>
-
-    :param tag: str = None.
-            if provided, return only <tag> elements. example: 'a', or 'img'
-    :param _results: do not use!
-    """
-    results = _results or set()
-    for element in element.children():
-        if tag:
-            if element.tag_name == tag:
-                results.add(element)
-        else:
-            results.add(element)
-        results |= _recursive_children(element, tag, results)
-    return results
+from typing import List
+
+from selenium.webdriver.common.by import By
+import selenium.webdriver.remote.webelement
+
+
+class WebElement(selenium.webdriver.remote.webelement.WebElement):
+    def click_safe(self):
+        super().click()
+        self._parent.reconnect(0.1)
+
+    def children(
+        self, tag=None, recursive=False
+    ) -> List[selenium.webdriver.remote.webelement.WebElement]:
+        """
+        returns direct child elements of current element
+        :param tag: str,  if supplied, returns <tag> nodes only
+        """
+        script = "return [... arguments[0].children]"
+        if tag:
+            script += ".filter( node => node.tagName === '%s')" % tag.upper()
+        if recursive:
+            return list(_recursive_children(self, tag))
+        return list(self._parent.execute_script(script, self))
+
+
+class UCWebElement(WebElement):
+    """
+    Custom WebElement class which makes it easier to view elements when
+    working in an interactive environment.
+
+    standard webelement repr:
+    <selenium.webdriver.remote.webelement.WebElement (session="85ff0f671512fa535630e71ee951b1f2", element="6357cb55-92c3-4c0f-9416-b174f9c1b8c4")>
+
+    using this WebElement class:
+    <WebElement(<a class="mobile-show-inline-block mc-update-infos init-ok" href="#" id="main-cat-switcher-mobile">)>
+
+    """
+
+    def __init__(self, parent, id_):
+        super().__init__(parent, id_)
+        self._attrs = None
+
+    @property
+    def attrs(self):
+        if not self._attrs:
+            self._attrs = self._parent.execute_script(
+                """
+                var items = {}; 
+                for (index = 0; index < arguments[0].attributes.length; ++index) 
+                {
+                 items[arguments[0].attributes[index].name] = arguments[0].attributes[index].value 
+                }; 
+                return items;
+                """,
+                self,
+            )
+        return self._attrs
+
+    def __repr__(self):
+        strattrs = " ".join([f'{k}="{v}"' for k, v in self.attrs.items()])
+        if strattrs:
+            strattrs = " " + strattrs
+        return f"{self.__class__.__name__} <{self.tag_name}{strattrs}>"
+
+
+def _recursive_children(element, tag: str = None, _results=None):
+    """
+    returns all children of <element> recursively
+
+    :param element: `WebElement` object.
+            find children below this <element>
+
+    :param tag: str = None.
+            if provided, return only <tag> elements. example: 'a', or 'img'
+    :param _results: do not use!
+    """
+    results = _results or set()
+    for element in element.children():
+        if tag:
+            if element.tag_name == tag:
+                results.add(element)
+        else:
+            results.add(element)
+        results |= _recursive_children(element, tag, results)
+    return results
```

### Comparing `undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/PKG-INFO` & `undetected-chromedriver-3.5.0/undetected_chromedriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undetected-chromedriver
-Version: 3.4.7
+Version: 3.5.0
 Summary: ('Selenium.webdriver.Chrome replacement with compatiblity for Brave, and other Chromium based browsers.', 'Not triggered by CloudFlare/Imperva/hCaptcha and such.', 'NOTE: results may vary due to many factors. No guarantees are given, except for ongoing efforts in understanding detection algorithms.')
 Home-page: https://github.com/ultrafunkamsterdam/undetected-chromedriver
 Author: UltrafunkAmsterdam
 Author-email: info@blackhat-security.nl
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `undetected-chromedriver-3.4.7/undetected_chromedriver.egg-info/SOURCES.txt` & `undetected-chromedriver-3.5.0/undetected_chromedriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

