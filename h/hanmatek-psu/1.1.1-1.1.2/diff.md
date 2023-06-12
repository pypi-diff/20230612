# Comparing `tmp/hanmatek_psu-1.1.1.tar.gz` & `tmp/hanmatek_psu-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hanmatek_psu-1.1.1.tar", max compression
+gzip compressed data, was "hanmatek_psu-1.1.2.tar", max compression
```

## Comparing `hanmatek_psu-1.1.1.tar` & `hanmatek_psu-1.1.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1075 2022-12-19 22:56:00.061296 hanmatek_psu-1.1.1/LICENSE
--rw-r--r--   0        0        0     3504 2022-12-19 22:56:00.061296 hanmatek_psu-1.1.1/README.md
--rwxr-xr-x   0        0        0     4529 2022-12-19 22:56:00.061296 hanmatek_psu-1.1.1/hanmatek/HM3xxP.py
--rw-r--r--   0        0        0     3910 2022-12-19 22:56:00.062296 hanmatek_psu-1.1.1/hanmatek/HM3xxP_regmap.py
--rw-r--r--   0        0        0       98 2022-12-19 22:56:00.062296 hanmatek_psu-1.1.1/hanmatek/__init__.py
--rw-r--r--   0        0        0     4664 2022-12-19 22:56:00.062296 hanmatek_psu-1.1.1/hanmatek/__main__.py
--rw-r--r--   0        0        0        0 2022-12-19 22:56:00.062296 hanmatek_psu-1.1.1/hanmatek/py.typed
--rw-r--r--   0        0        0     1730 2022-12-19 22:56:00.062296 hanmatek_psu-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4492 1970-01-01 00:00:00.000000 hanmatek_psu-1.1.1/setup.py
--rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 hanmatek_psu-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-12 11:48:46.060900 hanmatek_psu-1.1.2/LICENSE
+-rw-r--r--   0        0        0     3504 2023-06-12 11:48:46.060900 hanmatek_psu-1.1.2/README.md
+-rwxr-xr-x   0        0        0     4574 2023-06-12 11:48:46.060900 hanmatek_psu-1.1.2/hanmatek/HM3xxP.py
+-rw-r--r--   0        0        0     3910 2023-06-12 11:48:46.061900 hanmatek_psu-1.1.2/hanmatek/HM3xxP_regmap.py
+-rw-r--r--   0        0        0       98 2023-06-12 11:48:46.061900 hanmatek_psu-1.1.2/hanmatek/__init__.py
+-rw-r--r--   0        0        0     4664 2023-06-12 11:48:46.061900 hanmatek_psu-1.1.2/hanmatek/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:48:46.083900 hanmatek_psu-1.1.2/hanmatek/py.typed
+-rw-r--r--   0        0        0     1730 2023-06-12 11:48:46.061900 hanmatek_psu-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 hanmatek_psu-1.1.2/PKG-INFO
```

### Comparing `hanmatek_psu-1.1.1/LICENSE` & `hanmatek_psu-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hanmatek_psu-1.1.1/README.md` & `hanmatek_psu-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hanmatek_psu-1.1.1/hanmatek/HM3xxP.py` & `hanmatek_psu-1.1.2/hanmatek/HM3xxP.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     def __init__(self, port: str, slave_addr: int = 1):
         self.port = port
         self.slave_addr = slave_addr
         self.instrument = minimalmodbus.Instrument(
             port=port, slaveaddress=slave_addr, mode=minimalmodbus.MODE_RTU
         )
         self.instrument.serial.baudrate = 9600
+        self.instrument.serial.timeout = 0.1
 
     def _retry(self, func: Callable[[], T], retries: int = 10, delay: float = 0.01) -> T:
         last_exc = None
         for _ in range(retries):
             try:
                 return func()
             except minimalmodbus.ModbusException as exc:
```

### Comparing `hanmatek_psu-1.1.1/hanmatek/HM3xxP_regmap.py` & `hanmatek_psu-1.1.2/hanmatek/HM3xxP_regmap.py`

 * *Files identical despite different names*

### Comparing `hanmatek_psu-1.1.1/hanmatek/__main__.py` & `hanmatek_psu-1.1.2/hanmatek/__main__.py`

 * *Files identical despite different names*

### Comparing `hanmatek_psu-1.1.1/pyproject.toml` & `hanmatek_psu-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hanmatek-psu"
-version = "1.1.1"
+version = "1.1.2"
 packages = [
     { include = "hanmatek" },
     { include = "hanmatek/py.typed" }
 ]
 readme = "README.md"
 description = "Library and CLI for the Hanmatek Power supply units (PSU) of the HM3xxP series."
 authors = ["Janos <janoskut@gmail.com>"]
```

### Comparing `hanmatek_psu-1.1.1/setup.py` & `hanmatek_psu-1.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,124 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: hanmatek-psu
+Version: 1.1.2
+Summary: Library and CLI for the Hanmatek Power supply units (PSU) of the HM3xxP series.
+Home-page: https://gitlab.com/janoskut/hanmatek-psu/-/tree/main
+License: MIT
+Keywords: power-supply,psu,equipment,lab,automation
+Author: Janos
+Author-email: janoskut@gmail.com
+Maintainer: Janos
+Maintainer-email: janoskut@gmail.com
+Requires-Python: >=3.8
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: System :: Hardware :: Hardware Drivers
+Requires-Dist: minimalmodbus (>=2.0.1,<3.0.0)
+Project-URL: Repository, https://gitlab.com/janoskut/hanmatek-psu/-/tree/main
+Description-Content-Type: text/markdown
+
+[![](https://img.shields.io/pypi/v/hanmatek-psu.svg?maxAge=3600)](https://pypi.org/project/hanmatek-psu/)
+[![Latest Release](https://gitlab.com/janoskut/hanmatek-psu/-/badges/release.svg)](https://gitlab.com/janoskut/hanmatek-psu/-/releases)
+[![pipeline status](https://gitlab.com/janoskut/hanmatek-psu/badges/main/pipeline.svg)](https://gitlab.com/janoskut/hanmatek-psu/-/commits/main)
+[![coverage report](https://gitlab.com/janoskut/hanmatek-psu/badges/main/coverage.svg)](https://gitlab.com/janoskut/hanmatek-psu/-/commits/main)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+
+
+# Hanmatek HM3xxP PSU control library and CLI
+
+Unifying library and CLI for the popular and low-cost digital lab power supplies `HM305P` and
+`HM310P`.
+
+The library provides an (almost) complete, easy to use interface to all known functions of the
+device. This project is different to the below mentioned ones, in that it provides a minimal,
+but complete interface to the device and also keeps the dependencies low.
+
+This project is based on the work done in <https://github.com/notkevinjohn/HM310P>, which uses the
+`minimalmodbus` library for device communication. Other related projects were providing
+useful register definition and hints:
+
+- <https://github.com/JackDoan/hm305_ctrl/tree/master/hm305>
+- <https://github.com/hobbyquaker/hanmatek-hm310p>
+- <https://sigrok.org/wiki/ETommens_eTM-xxxxP_Series#Protocol>
+
+
+## Installation
+
+```py
+pip install hanmatek-psu
+```
+
+If users are in the `plugdev` user group, Hanmatek devices are accessible via `/dev/ttyUSBx` without
+privileges. Adding the following `udev` rule will create a symlink `/dev/ttyHM3xxP` when a Hanmatek
+PSU device is plugged in via USB. This symlink is used by default by the `hanmatek-cli` to find
+devices:
+
+```sh
+echo 'SUBSYSTEM=="tty", ATTRS{idVendor}=="1a86", ATTRS{idProduct}=="7523", SYMLINK+="ttyHM3xxP", MODE="0666", GROUP="plugdev"' | sudo tee "/etc/udev/rules.d/99-hanmatek.rules" > /dev/null
+```
+
+## Usage
+
+### CLI Usage
+
+```sh
+hanmatek-cli -h
+hanmatek-cli --discover             # find devices
+hanmatek-cli                        # show default device info
+hanmatek-cli --device /dev/ttyUSB0  # specific device
+hanmatek-cli voltage:set 3.0        # set voltage
+hanmatek-cli current:set 0.1        # set current limit
+hanmatek-cli output on
+hanmatek-cli current                # read current
+hanmatek-cli power                  # read power
+hanmatek-cli output off
+hanmatek-cli --list                 # list all commands/registers
+```
+
+### Library Usage
+
+```py
+from hanmatek import HM3xxP
+
+device = HM3xxP("/dev/ttyHM3xxP")
+print(device.info())
+device.write("voltage:set", 3.0)
+device.write("current:set", 3.0)
+device.write("output", True)
+print(device.read("current"))
+print(device.read("power"))
+device.write("output", False)
+```
+
+## Development
+
+The following tools are used to provide clean and quality software, and made available through a
+`tox` configuration: `flake8` for linting, `black` for code formatting and checking, `mypy` for
+type checking and `pytest` for unit tests. Use as:
+
+```sh
+pip install tox
+```
+
+```sh
+tox -a       # show test environments
+tox          # run all
+tox -e test  # run unit tests
+tox -e lint  # run lint
+tox -e type  # run type checker
+```
+
+(we're using [`pyproject-flake8`](https://pypi.org/project/pyproject-flake8), so that the `flake8`
+configuration can live in `pyproject.toml` - within `tox` we then run `pflake8` instead of
+`flake8`.)
 
-packages = \
-['hanmatek']
-
-package_data = \
-{'': ['*']}
-
-modules = \
-['py']
-install_requires = \
-['minimalmodbus>=2.0.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['hanmatek-cli = hanmatek.__main__:main']}
-
-setup_kwargs = {
-    'name': 'hanmatek-psu',
-    'version': '1.1.1',
-    'description': 'Library and CLI for the Hanmatek Power supply units (PSU) of the HM3xxP series.',
-    'long_description': '[![](https://img.shields.io/pypi/v/hanmatek-psu.svg?maxAge=3600)](https://pypi.org/project/hanmatek-psu/)\n[![Latest Release](https://gitlab.com/janoskut/hanmatek-psu/-/badges/release.svg)](https://gitlab.com/janoskut/hanmatek-psu/-/releases)\n[![pipeline status](https://gitlab.com/janoskut/hanmatek-psu/badges/main/pipeline.svg)](https://gitlab.com/janoskut/hanmatek-psu/-/commits/main)\n[![coverage report](https://gitlab.com/janoskut/hanmatek-psu/badges/main/coverage.svg)](https://gitlab.com/janoskut/hanmatek-psu/-/commits/main)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\n\n\n# Hanmatek HM3xxP PSU control library and CLI\n\nUnifying library and CLI for the popular and low-cost digital lab power supplies `HM305P` and\n`HM310P`.\n\nThe library provides an (almost) complete, easy to use interface to all known functions of the\ndevice. This project is different to the below mentioned ones, in that it provides a minimal,\nbut complete interface to the device and also keeps the dependencies low.\n\nThis project is based on the work done in <https://github.com/notkevinjohn/HM310P>, which uses the\n`minimalmodbus` library for device communication. Other related projects were providing\nuseful register definition and hints:\n\n- <https://github.com/JackDoan/hm305_ctrl/tree/master/hm305>\n- <https://github.com/hobbyquaker/hanmatek-hm310p>\n- <https://sigrok.org/wiki/ETommens_eTM-xxxxP_Series#Protocol>\n\n\n## Installation\n\n```py\npip install hanmatek-psu\n```\n\nIf users are in the `plugdev` user group, Hanmatek devices are accessible via `/dev/ttyUSBx` without\nprivileges. Adding the following `udev` rule will create a symlink `/dev/ttyHM3xxP` when a Hanmatek\nPSU device is plugged in via USB. This symlink is used by default by the `hanmatek-cli` to find\ndevices:\n\n```sh\necho \'SUBSYSTEM=="tty", ATTRS{idVendor}=="1a86", ATTRS{idProduct}=="7523", SYMLINK+="ttyHM3xxP", MODE="0666", GROUP="plugdev"\' | sudo tee "/etc/udev/rules.d/99-hanmatek.rules" > /dev/null\n```\n\n## Usage\n\n### CLI Usage\n\n```sh\nhanmatek-cli -h\nhanmatek-cli --discover             # find devices\nhanmatek-cli                        # show default device info\nhanmatek-cli --device /dev/ttyUSB0  # specific device\nhanmatek-cli voltage:set 3.0        # set voltage\nhanmatek-cli current:set 0.1        # set current limit\nhanmatek-cli output on\nhanmatek-cli current                # read current\nhanmatek-cli power                  # read power\nhanmatek-cli output off\nhanmatek-cli --list                 # list all commands/registers\n```\n\n### Library Usage\n\n```py\nfrom hanmatek import HM3xxP\n\ndevice = HM3xxP("/dev/ttyHM3xxP")\nprint(device.info())\ndevice.write("voltage:set", 3.0)\ndevice.write("current:set", 3.0)\ndevice.write("output", True)\nprint(device.read("current"))\nprint(device.read("power"))\ndevice.write("output", False)\n```\n\n## Development\n\nThe following tools are used to provide clean and quality software, and made available through a\n`tox` configuration: `flake8` for linting, `black` for code formatting and checking, `mypy` for\ntype checking and `pytest` for unit tests. Use as:\n\n```sh\npip install tox\n```\n\n```sh\ntox -a       # show test environments\ntox          # run all\ntox -e test  # run unit tests\ntox -e lint  # run lint\ntox -e type  # run type checker\n```\n\n(we\'re using [`pyproject-flake8`](https://pypi.org/project/pyproject-flake8), so that the `flake8`\nconfiguration can live in `pyproject.toml` - within `tox` we then run `pflake8` instead of\n`flake8`.)\n',
-    'author': 'Janos',
-    'author_email': 'janoskut@gmail.com',
-    'maintainer': 'Janos',
-    'maintainer_email': 'janoskut@gmail.com',
-    'url': 'https://gitlab.com/janoskut/hanmatek-psu/-/tree/main',
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8',
-}
-
-
-setup(**setup_kwargs)
```

