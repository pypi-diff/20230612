# Comparing `tmp/micropython-package-template-0.8.0.tar.gz` & `tmp/micropython-package-template-0.8.1.tar.gz`

## Comparing `micropython-package-template-0.8.0.tar` & `micropython-package-template-0.8.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 20:38:13.000000 micropython-package-template-0.8.0/be_upy_blink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-18 20:38:13.000000 micropython-package-template-0.8.0/be_upy_blink/blink.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-18 20:38:22.000000 micropython-package-template-0.8.0/be_upy_blink/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-18 20:38:23.000000 micropython-package-template-0.8.0/micropython_package_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 19:27:22.000000 micropython-package-template-0.8.1/be_upy_blink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-12 19:27:22.000000 micropython-package-template-0.8.1/be_upy_blink/blink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-12 19:27:34.000000 micropython-package-template-0.8.1/be_upy_blink/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-06-12 19:27:35.000000 micropython-package-template-0.8.1/micropython_package_template.egg-info/PKG-INFO
```

### Comparing `micropython-package-template-0.8.0/be_upy_blink/blink.py` & `micropython-package-template-0.8.1/be_upy_blink/blink.py`

 * *Files identical despite different names*

### Comparing `micropython-package-template-0.8.0/micropython_package_template.egg-info/PKG-INFO` & `micropython-package-template-0.8.1/micropython_package_template.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: micropython-package-template
-Version: 0.8.0
+Version: 0.8.1
 Summary: MicroPython PyPi package template project with auto deploy
 Home-page: https://github.com/brainelectronics/micropython-package-template
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 License: MIT
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-template/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-template
-Keywords: micropython,template
+Keywords: micropython,template,package
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -87,14 +87,15 @@
 ### Install package with upip
 
 Connect the MicroPython device to a network (if possible)
 
 ```python
 import network
 station = network.WLAN(network.STA_IF)
+station.active(True)
 station.connect('SSID', 'PASSWORD')
 station.isconnected()
 ```
 
 #### General
 
 Install the latest package version of this lib on the MicroPython device
@@ -119,40 +120,42 @@
 import mip
 # install a verions of a specific branch
 mip.install("github:brainelectronics/micropython-package-template", version="feature/initial-implementation")
 # install a tag version
 mip.install("github:brainelectronics/micropython-package-template", version="0.6.0")
 ```
 
-For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`
+For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`.
+With `upip` always the latest available version will be installed.
 
 ```python
 import upip
-upip.install('micropython-package-template==0.1.1')
+upip.install('micropython-package-template')
 ```
 
 #### Test version
 
 Install a specific release candidate version uploaded to
 [Test Python Package Index](https://test.pypi.org/) on every PR on the
 MicroPython device. If no specific version is set, the latest stable version
 will be used.
 
 ```python
 import mip
 mip.install("github:brainelectronics/micropython-package-template", version="0.6.0-rc9.dev13")
 ```
 
-For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`
+For MicroPython versions below 1.19.1 use the `upip` package instead of `mip`.
+With `upip` always the latest available version will be installed.
 
 ```python
 import upip
 # overwrite index_urls to only take artifacts from test.pypi.org
 upip.index_urls = ['https://test.pypi.org/pypi']
-upip.install('micropython-package-template==0.2.0rc1.dev6')
+upip.install('micropython-package-template')
 ```
 
 See also [brainelectronics Test PyPi Server in Docker][ref-brainelectronics-test-pypiserver]
 for a test PyPi server running on Docker.
 
 ### Manually
```

