# Comparing `tmp/sev-snp-measure-0.0.5.tar.gz` & `tmp/sev-snp-measure-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sev-snp-measure-0.0.5.tar", last modified: Thu Apr 13 09:52:59 2023, max compression
+gzip compressed data, was "sev-snp-measure-0.0.6.tar", last modified: Mon Jun 12 05:30:37 2023, max compression
```

## Comparing `sev-snp-measure-0.0.5.tar` & `sev-snp-measure-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/
--rw-r--r--   0 dubek     (1000) dubek     (1000)    11358 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.5/LICENSE
--rw-r--r--   0 dubek     (1000) dubek     (1000)     6770 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/PKG-INFO
--rw-r--r--   0 dubek     (1000) dubek     (1000)     6025 2023-04-13 07:47:31.000000 sev-snp-measure-0.0.5/README.md
--rw-r--r--   0 dubek     (1000) dubek     (1000)       85 2022-04-11 09:47:58.000000 sev-snp-measure-0.0.5/pyproject.toml
--rw-r--r--   0 dubek     (1000) dubek     (1000)      973 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/setup.cfg
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/
--rw-r--r--   0 dubek     (1000) dubek     (1000)     6770 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/PKG-INFO
--rw-r--r--   0 dubek     (1000) dubek     (1000)      590 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/SOURCES.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)        1 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/dependency_links.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)      109 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/entry_points.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)       40 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/requires.txt
--rw-r--r--   0 dubek     (1000) dubek     (1000)       14 2023-04-13 09:52:59.000000 sev-snp-measure-0.0.5/sev_snp_measure.egg-info/top_level.txt
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/sevsnpmeasure/
--rw-r--r--   0 dubek     (1000) dubek     (1000)       89 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.5/sevsnpmeasure/__init__.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3616 2023-04-13 09:51:04.000000 sev-snp-measure-0.0.5/sevsnpmeasure/cli.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     2462 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.5/sevsnpmeasure/gctx.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     4035 2023-04-13 07:59:29.000000 sev-snp-measure-0.0.5/sevsnpmeasure/guest.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     5591 2023-04-13 07:47:31.000000 sev-snp-measure-0.0.5/sevsnpmeasure/id_block.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     4765 2023-04-13 07:59:29.000000 sev-snp-measure-0.0.5/sevsnpmeasure/ovmf.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3488 2022-06-08 14:31:05.000000 sev-snp-measure-0.0.5/sevsnpmeasure/sev_hashes.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)      600 2022-04-24 09:17:37.000000 sev-snp-measure-0.0.5/sevsnpmeasure/sev_mode.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     1609 2023-03-07 15:16:17.000000 sev-snp-measure-0.0.5/sevsnpmeasure/vcpu_types.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     5727 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.5/sevsnpmeasure/vmsa.py
-drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-04-13 09:52:59.877793 sev-snp-measure-0.0.5/tests/
--rw-r--r--   0 dubek     (1000) dubek     (1000)     3130 2023-04-13 07:59:29.000000 sev-snp-measure-0.0.5/tests/test_guest.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)     1149 2023-04-13 07:47:31.000000 sev-snp-measure-0.0.5/tests/test_id_block.py
--rw-r--r--   0 dubek     (1000) dubek     (1000)      480 2022-06-08 12:42:41.000000 sev-snp-measure-0.0.5/tests/test_vcpu_types.py
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)    11358 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.6/LICENSE
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     7370 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/PKG-INFO
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     6625 2023-06-09 08:37:27.000000 sev-snp-measure-0.0.6/README.md
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       85 2022-04-11 09:47:58.000000 sev-snp-measure-0.0.6/pyproject.toml
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      973 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/setup.cfg
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     7370 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/PKG-INFO
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      617 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/SOURCES.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)        1 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/dependency_links.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      109 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/entry_points.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       40 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/requires.txt
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       14 2023-06-12 05:30:37.000000 sev-snp-measure-0.0.6/sev_snp_measure.egg-info/top_level.txt
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/sevsnpmeasure/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       89 2022-03-09 13:11:47.000000 sev-snp-measure-0.0.6/sevsnpmeasure/__init__.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     4647 2023-06-12 05:25:14.000000 sev-snp-measure-0.0.6/sevsnpmeasure/cli.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     2462 2023-04-10 12:16:34.000000 sev-snp-measure-0.0.6/sevsnpmeasure/gctx.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5303 2023-06-08 08:08:31.000000 sev-snp-measure-0.0.6/sevsnpmeasure/guest.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5638 2023-06-08 05:52:47.000000 sev-snp-measure-0.0.6/sevsnpmeasure/id_block.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     5078 2023-06-08 08:08:31.000000 sev-snp-measure-0.0.6/sevsnpmeasure/ovmf.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     3488 2023-06-08 09:35:10.000000 sev-snp-measure-0.0.6/sevsnpmeasure/sev_hashes.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      600 2022-04-24 09:17:37.000000 sev-snp-measure-0.0.6/sevsnpmeasure/sev_mode.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     1732 2023-05-28 09:56:41.000000 sev-snp-measure-0.0.6/sevsnpmeasure/vcpu_types.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)       70 2023-05-22 17:48:16.000000 sev-snp-measure-0.0.6/sevsnpmeasure/vmm_types.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     6338 2023-05-22 17:48:16.000000 sev-snp-measure-0.0.6/sevsnpmeasure/vmsa.py
+drwxr-xr-x   0 dubek     (1000) dubek     (1000)        0 2023-06-12 05:30:37.365026 sev-snp-measure-0.0.6/tests/
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     8260 2023-06-09 08:37:27.000000 sev-snp-measure-0.0.6/tests/test_guest.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)     1149 2023-04-13 07:47:31.000000 sev-snp-measure-0.0.6/tests/test_id_block.py
+-rw-r--r--   0 dubek     (1000) dubek     (1000)      480 2022-06-08 12:42:41.000000 sev-snp-measure-0.0.6/tests/test_vcpu_types.py
```

### Comparing `sev-snp-measure-0.0.5/LICENSE` & `sev-snp-measure-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.5/PKG-INFO` & `sev-snp-measure-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: sev-snp-measure
-Version: 0.0.5
-Summary: Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
-Home-page: https://github.com/IBM/sev-snp-measure
-Author: Dov Murik
-Author-email: dov.murik1@il.ibm.com
-Project-URL: Bug Tracker, https://github.com/IBM/sev-snp-measure/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Security
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sev-snp-measure
 
 ## Scope
 
 Command-line tool and Python library to calculate expected measurement of an
 AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing.
 
@@ -46,17 +27,17 @@
 ## Command-line usage
 
 ### sev-snp-measure
 ```
 $ sev-snp-measure --help
 usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp,snp:ovmf-hash} [--vcpus N]
                        [--vcpu-type CPUTYPE] [--vcpu-sig VALUE] [--vcpu-family FAMILY]
-                       [--vcpu-model MODEL] [--vcpu-stepping STEPPING] --ovmf PATH [--kernel PATH]
-                       [--initrd PATH] [--append CMDLINE] [--output-format {hex,base64}]
-                       [--snp-ovmf-hash HASH]
+                       [--vcpu-model MODEL] [--vcpu-stepping STEPPING] [--vmm-type VMMTYPE] --ovmf
+                       PATH [--kernel PATH] [--initrd PATH] [--append CMDLINE]
+                       [--output-format {hex,base64}] [--snp-ovmf-hash HASH]
 
 Calculate AMD SEV/SEV-ES/SEV-SNP guest launch measurement
 
 optional arguments:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose
@@ -67,14 +48,15 @@
                         EPYC-Rome, EPYC-Rome-v1, EPYC-Rome-v2, EPYC-Rome-v3, EPYC-Milan, EPYC-
                         Milan-v1, EPYC-Milan-v2)
   --vcpu-sig VALUE      Guest vcpu signature value
   --vcpu-family FAMILY  Guest vcpu family
   --vcpu-model MODEL    Guest vcpu model
   --vcpu-stepping STEPPING
                         Guest vcpu stepping
+  --vmm-type VMMTYPE    Type of guest vmm (QEMU, ec2)
   --ovmf PATH           OVMF file to calculate hash from
   --kernel PATH         Kernel file to calculate hash from
   --initrd PATH         Initrd file to calculate hash from (use with --kernel)
   --append CMDLINE      Kernel command line to calculate hash from (use with --kernel)
   --output-format {hex,base64}
                         Measurement output format
   --snp-ovmf-hash HASH  Precalculated hash of the OVMF binary (hex string)
@@ -116,17 +98,17 @@
 block = id_block.snp_calc_id_block(ld,"id_key_file","author_key_file")
 print("Calculated id block in base64", block)
 ```
 
 ## Choosing guest CPU type
 
 For SEV-ES and SEV-SNP, the initial CPU state (VMSA) includes the guest CPU
-signature in the edx register.  Therefore, starting the VM with a different
-type of guest CPU will modify the content of the VMSA, and therefore modify the
-calculated measurement.
+signature in the edx register when you use the QEMU vmm.  Therefore, starting
+the VM with a different type of guest CPU will modify the content of the VMSA,
+and therefore modify the calculated measurement.
 
 You can choose the guest CPU type using `--vcpu-type`, or `--vcpu-sig`, or a
 combination of `--vcpu-family`, `--vcpu-model`, and `--vcpu-stepping`. For
 example, the following 3 invocations are identical:
 
 1. `sev-snp-measure --vcpu-type=EPYC-v4 ...`
 2. `sev-snp-measure --vcpu-sig=0x800f12 ...`
@@ -152,19 +134,43 @@
     $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd.old --ovmf-hash cab7e[...]
     d52697c3e056fb8d698d19cc29adfbed5a8ec9170cb9eb63c2ac957d22b4eb647e25780162036d063a0cf418b8830acc
 
 ## Related projects
 
 * libvirt tools: [virt-dom-sev-validate](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-validate.py),
   [virt-dom-sev-vmsa-tool](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-vmsa-tool.py)
-* [sev Rust crate](https://github.com/virtee/sev)
+* [sev Rust crate](https://github.com/virtee/sev) and [snpguest CLI tool](https://github.com/virtee/snpguest)
 * [snp-digest-rs](https://github.com/slp/snp-digest-rs)
-* [AMD SEV-Tool](https://github.com/AMDESE/sev-tool)
+* AMD [sev-tool](https://github.com/AMDESE/sev-tool), [sev-guest](https://github.com/AMDESE/sev-guest),
+  and [sev-utils](https://github.com/amd/sev-utils)
 * [go-sev-guest](https://github.com/google/go-sev-guest)
 
+## Development
+
+Run all unit tests:
+
+    pip install -r requirements.txt
+    make test
+
+Check unit tests coverage:
+
+    pip install coverage
+    make coverage
+    # See HTML coverage report in htmlcov/
+
+Check Python type hints:
+
+    pip install mypy
+    make typecheck
+
+Check Python coding style:
+
+    pip install flake8
+    make lint
+
 ## Notes
 
 If you have any questions or issues you can create a new [issue
 here](https://github.com/IBM/sev-snp-measure/issues/new)
 
 Pull requests are welcome!
```

### Comparing `sev-snp-measure-0.0.5/README.md` & `sev-snp-measure-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: sev-snp-measure
+Version: 0.0.6
+Summary: Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
+Home-page: https://github.com/IBM/sev-snp-measure
+Author: Dov Murik
+Author-email: dov.murik1@il.ibm.com
+Project-URL: Bug Tracker, https://github.com/IBM/sev-snp-measure/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Security
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sev-snp-measure
 
 ## Scope
 
 Command-line tool and Python library to calculate expected measurement of an
 AMD SEV/SEV-ES/SEV-SNP guest VM for confidential computing.
 
@@ -27,17 +46,17 @@
 ## Command-line usage
 
 ### sev-snp-measure
 ```
 $ sev-snp-measure --help
 usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp,snp:ovmf-hash} [--vcpus N]
                        [--vcpu-type CPUTYPE] [--vcpu-sig VALUE] [--vcpu-family FAMILY]
-                       [--vcpu-model MODEL] [--vcpu-stepping STEPPING] --ovmf PATH [--kernel PATH]
-                       [--initrd PATH] [--append CMDLINE] [--output-format {hex,base64}]
-                       [--snp-ovmf-hash HASH]
+                       [--vcpu-model MODEL] [--vcpu-stepping STEPPING] [--vmm-type VMMTYPE] --ovmf
+                       PATH [--kernel PATH] [--initrd PATH] [--append CMDLINE]
+                       [--output-format {hex,base64}] [--snp-ovmf-hash HASH]
 
 Calculate AMD SEV/SEV-ES/SEV-SNP guest launch measurement
 
 optional arguments:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose
@@ -48,14 +67,15 @@
                         EPYC-Rome, EPYC-Rome-v1, EPYC-Rome-v2, EPYC-Rome-v3, EPYC-Milan, EPYC-
                         Milan-v1, EPYC-Milan-v2)
   --vcpu-sig VALUE      Guest vcpu signature value
   --vcpu-family FAMILY  Guest vcpu family
   --vcpu-model MODEL    Guest vcpu model
   --vcpu-stepping STEPPING
                         Guest vcpu stepping
+  --vmm-type VMMTYPE    Type of guest vmm (QEMU, ec2)
   --ovmf PATH           OVMF file to calculate hash from
   --kernel PATH         Kernel file to calculate hash from
   --initrd PATH         Initrd file to calculate hash from (use with --kernel)
   --append CMDLINE      Kernel command line to calculate hash from (use with --kernel)
   --output-format {hex,base64}
                         Measurement output format
   --snp-ovmf-hash HASH  Precalculated hash of the OVMF binary (hex string)
@@ -97,17 +117,17 @@
 block = id_block.snp_calc_id_block(ld,"id_key_file","author_key_file")
 print("Calculated id block in base64", block)
 ```
 
 ## Choosing guest CPU type
 
 For SEV-ES and SEV-SNP, the initial CPU state (VMSA) includes the guest CPU
-signature in the edx register.  Therefore, starting the VM with a different
-type of guest CPU will modify the content of the VMSA, and therefore modify the
-calculated measurement.
+signature in the edx register when you use the QEMU vmm.  Therefore, starting
+the VM with a different type of guest CPU will modify the content of the VMSA,
+and therefore modify the calculated measurement.
 
 You can choose the guest CPU type using `--vcpu-type`, or `--vcpu-sig`, or a
 combination of `--vcpu-family`, `--vcpu-model`, and `--vcpu-stepping`. For
 example, the following 3 invocations are identical:
 
 1. `sev-snp-measure --vcpu-type=EPYC-v4 ...`
 2. `sev-snp-measure --vcpu-sig=0x800f12 ...`
@@ -133,19 +153,43 @@
     $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd.old --ovmf-hash cab7e[...]
     d52697c3e056fb8d698d19cc29adfbed5a8ec9170cb9eb63c2ac957d22b4eb647e25780162036d063a0cf418b8830acc
 
 ## Related projects
 
 * libvirt tools: [virt-dom-sev-validate](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-validate.py),
   [virt-dom-sev-vmsa-tool](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-vmsa-tool.py)
-* [sev Rust crate](https://github.com/virtee/sev)
+* [sev Rust crate](https://github.com/virtee/sev) and [snpguest CLI tool](https://github.com/virtee/snpguest)
 * [snp-digest-rs](https://github.com/slp/snp-digest-rs)
-* [AMD SEV-Tool](https://github.com/AMDESE/sev-tool)
+* AMD [sev-tool](https://github.com/AMDESE/sev-tool), [sev-guest](https://github.com/AMDESE/sev-guest),
+  and [sev-utils](https://github.com/amd/sev-utils)
 * [go-sev-guest](https://github.com/google/go-sev-guest)
 
+## Development
+
+Run all unit tests:
+
+    pip install -r requirements.txt
+    make test
+
+Check unit tests coverage:
+
+    pip install coverage
+    make coverage
+    # See HTML coverage report in htmlcov/
+
+Check Python type hints:
+
+    pip install mypy
+    make typecheck
+
+Check Python coding style:
+
+    pip install flake8
+    make lint
+
 ## Notes
 
 If you have any questions or issues you can create a new [issue
 here](https://github.com/IBM/sev-snp-measure/issues/new)
 
 Pull requests are welcome!
```

### Comparing `sev-snp-measure-0.0.5/setup.cfg` & `sev-snp-measure-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sev-snp-measure
-version = 0.0.5
+version = 0.0.6
 author = Dov Murik
 author_email = dov.murik1@il.ibm.com
 description = Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/IBM/sev-snp-measure
 project_urls =
```

### Comparing `sev-snp-measure-0.0.5/sev_snp_measure.egg-info/PKG-INFO` & `sev-snp-measure-0.0.6/sev_snp_measure.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sev-snp-measure
-Version: 0.0.5
+Version: 0.0.6
 Summary: Calculate expected measurement of an AMD SEV-SNP guest VM for confidential computing
 Home-page: https://github.com/IBM/sev-snp-measure
 Author: Dov Murik
 Author-email: dov.murik1@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/sev-snp-measure/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -46,17 +46,17 @@
 ## Command-line usage
 
 ### sev-snp-measure
 ```
 $ sev-snp-measure --help
 usage: sev-snp-measure [-h] [--version] [-v] --mode {sev,seves,snp,snp:ovmf-hash} [--vcpus N]
                        [--vcpu-type CPUTYPE] [--vcpu-sig VALUE] [--vcpu-family FAMILY]
-                       [--vcpu-model MODEL] [--vcpu-stepping STEPPING] --ovmf PATH [--kernel PATH]
-                       [--initrd PATH] [--append CMDLINE] [--output-format {hex,base64}]
-                       [--snp-ovmf-hash HASH]
+                       [--vcpu-model MODEL] [--vcpu-stepping STEPPING] [--vmm-type VMMTYPE] --ovmf
+                       PATH [--kernel PATH] [--initrd PATH] [--append CMDLINE]
+                       [--output-format {hex,base64}] [--snp-ovmf-hash HASH]
 
 Calculate AMD SEV/SEV-ES/SEV-SNP guest launch measurement
 
 optional arguments:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose
@@ -67,14 +67,15 @@
                         EPYC-Rome, EPYC-Rome-v1, EPYC-Rome-v2, EPYC-Rome-v3, EPYC-Milan, EPYC-
                         Milan-v1, EPYC-Milan-v2)
   --vcpu-sig VALUE      Guest vcpu signature value
   --vcpu-family FAMILY  Guest vcpu family
   --vcpu-model MODEL    Guest vcpu model
   --vcpu-stepping STEPPING
                         Guest vcpu stepping
+  --vmm-type VMMTYPE    Type of guest vmm (QEMU, ec2)
   --ovmf PATH           OVMF file to calculate hash from
   --kernel PATH         Kernel file to calculate hash from
   --initrd PATH         Initrd file to calculate hash from (use with --kernel)
   --append CMDLINE      Kernel command line to calculate hash from (use with --kernel)
   --output-format {hex,base64}
                         Measurement output format
   --snp-ovmf-hash HASH  Precalculated hash of the OVMF binary (hex string)
@@ -116,17 +117,17 @@
 block = id_block.snp_calc_id_block(ld,"id_key_file","author_key_file")
 print("Calculated id block in base64", block)
 ```
 
 ## Choosing guest CPU type
 
 For SEV-ES and SEV-SNP, the initial CPU state (VMSA) includes the guest CPU
-signature in the edx register.  Therefore, starting the VM with a different
-type of guest CPU will modify the content of the VMSA, and therefore modify the
-calculated measurement.
+signature in the edx register when you use the QEMU vmm.  Therefore, starting
+the VM with a different type of guest CPU will modify the content of the VMSA,
+and therefore modify the calculated measurement.
 
 You can choose the guest CPU type using `--vcpu-type`, or `--vcpu-sig`, or a
 combination of `--vcpu-family`, `--vcpu-model`, and `--vcpu-stepping`. For
 example, the following 3 invocations are identical:
 
 1. `sev-snp-measure --vcpu-type=EPYC-v4 ...`
 2. `sev-snp-measure --vcpu-sig=0x800f12 ...`
@@ -152,19 +153,43 @@
     $ sev-snp-measure --mode snp --vcpus=1 --vcpu-type=EPYC-v4 --ovmf=OVMF.fd.old --ovmf-hash cab7e[...]
     d52697c3e056fb8d698d19cc29adfbed5a8ec9170cb9eb63c2ac957d22b4eb647e25780162036d063a0cf418b8830acc
 
 ## Related projects
 
 * libvirt tools: [virt-dom-sev-validate](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-validate.py),
   [virt-dom-sev-vmsa-tool](https://gitlab.com/berrange/libvirt/-/blob/lgtm/tools/virt-dom-sev-vmsa-tool.py)
-* [sev Rust crate](https://github.com/virtee/sev)
+* [sev Rust crate](https://github.com/virtee/sev) and [snpguest CLI tool](https://github.com/virtee/snpguest)
 * [snp-digest-rs](https://github.com/slp/snp-digest-rs)
-* [AMD SEV-Tool](https://github.com/AMDESE/sev-tool)
+* AMD [sev-tool](https://github.com/AMDESE/sev-tool), [sev-guest](https://github.com/AMDESE/sev-guest),
+  and [sev-utils](https://github.com/amd/sev-utils)
 * [go-sev-guest](https://github.com/google/go-sev-guest)
 
+## Development
+
+Run all unit tests:
+
+    pip install -r requirements.txt
+    make test
+
+Check unit tests coverage:
+
+    pip install coverage
+    make coverage
+    # See HTML coverage report in htmlcov/
+
+Check Python type hints:
+
+    pip install mypy
+    make typecheck
+
+Check Python coding style:
+
+    pip install flake8
+    make lint
+
 ## Notes
 
 If you have any questions or issues you can create a new [issue
 here](https://github.com/IBM/sev-snp-measure/issues/new)
 
 Pull requests are welcome!
```

### Comparing `sev-snp-measure-0.0.5/sev_snp_measure.egg-info/SOURCES.txt` & `sev-snp-measure-0.0.6/sev_snp_measure.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 sevsnpmeasure/gctx.py
 sevsnpmeasure/guest.py
 sevsnpmeasure/id_block.py
 sevsnpmeasure/ovmf.py
 sevsnpmeasure/sev_hashes.py
 sevsnpmeasure/sev_mode.py
 sevsnpmeasure/vcpu_types.py
+sevsnpmeasure/vmm_types.py
 sevsnpmeasure/vmsa.py
 tests/test_guest.py
 tests/test_id_block.py
 tests/test_vcpu_types.py
```

### Comparing `sev-snp-measure-0.0.5/sevsnpmeasure/gctx.py` & `sev-snp-measure-0.0.6/sevsnpmeasure/gctx.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.5/sevsnpmeasure/guest.py` & `sev-snp-measure-0.0.6/sevsnpmeasure/guest.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import hashlib
 from typing import Optional
 
 from .gctx import GCTX
-from .ovmf import OVMF, SectionType
+from .ovmf import OVMF, SectionType, OvmfSevMetadataSectionDesc
 from .sev_hashes import SevHashes
 from .vmsa import VMSA
 from .sev_mode import SevMode
+from .vmm_types import VMMType
 
 PAGE_MASK = 0xfff
 
 
 def calc_launch_digest(mode: SevMode, vcpus: int, vcpu_sig: int, ovmf_file: str,
-                       kernel: str, initrd: str, append: str, snp_ovmf_hash_str: str = '') -> bytes:
+                       kernel: str, initrd: str, append: str, snp_ovmf_hash_str: str = '',
+                       vmm_type: VMMType = VMMType.QEMU) -> bytes:
     if snp_ovmf_hash_str and mode != SevMode.SEV_SNP:
         raise ValueError("SNP OVMF hash only works with SNP")
 
     if mode == SevMode.SEV_SNP:
-        return snp_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append, snp_ovmf_hash_str)
+        return snp_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append, snp_ovmf_hash_str, vmm_type)
     elif mode == SevMode.SEV_ES:
-        return seves_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append)
+        return seves_calc_launch_digest(vcpus, vcpu_sig, ovmf_file, kernel, initrd, append, vmm_type=vmm_type)
     elif mode == SevMode.SEV:
         return sev_calc_launch_digest(ovmf_file, kernel, initrd, append)
     else:
         raise ValueError("unknown mode")
 
 
 def snp_update_kernel_hashes(gctx: GCTX, ovmf: OVMF, sev_hashes: Optional[SevHashes], gpa: int, size: int) -> None:
@@ -37,38 +39,53 @@
         sev_hashes_page = sev_hashes.construct_page(offset_in_page)
         assert size == len(sev_hashes_page)
         gctx.update_normal_pages(gpa, sev_hashes_page)
     else:
         gctx.update_zero_pages(gpa, size)
 
 
-def snp_update_metadata_pages(gctx: GCTX, ovmf: OVMF, sev_hashes: Optional[SevHashes]) -> None:
-    for desc in ovmf.metadata_items():
-        if desc.section_type() == SectionType.SNP_SEC_MEM:
-            gctx.update_zero_pages(desc.gpa, desc.size)
-        elif desc.section_type() == SectionType.SNP_SECRETS:
-            gctx.update_secrets_page(desc.gpa)
-        elif desc.section_type() == SectionType.CPUID:
+def snp_update_section(desc: OvmfSevMetadataSectionDesc, gctx: GCTX, ovmf: OVMF,
+                       sev_hashes: Optional[SevHashes], vmm_type: VMMType) -> None:
+    if desc.section_type() == SectionType.SNP_SEC_MEM:
+        gctx.update_zero_pages(desc.gpa, desc.size)
+    elif desc.section_type() == SectionType.SNP_SECRETS:
+        gctx.update_secrets_page(desc.gpa)
+    elif desc.section_type() == SectionType.CPUID:
+        if not vmm_type == VMMType.ec2:
             gctx.update_cpuid_page(desc.gpa)
-        elif desc.section_type() == SectionType.SNP_KERNEL_HASHES:
-            snp_update_kernel_hashes(gctx, ovmf, sev_hashes, desc.gpa, desc.size)
-        else:
-            raise ValueError("unknown OVMF metadata section type")
+    elif desc.section_type() == SectionType.SNP_KERNEL_HASHES:
+        snp_update_kernel_hashes(gctx, ovmf, sev_hashes, desc.gpa, desc.size)
+    else:
+        raise ValueError("unknown OVMF metadata section type")
+
+
+def snp_update_metadata_pages(gctx: GCTX, ovmf: OVMF, sev_hashes: Optional[SevHashes], vmm_type: VMMType) -> None:
+    for desc in ovmf.metadata_items():
+        snp_update_section(desc, gctx, ovmf, sev_hashes, vmm_type)
+
+    if vmm_type == VMMType.ec2:
+        for desc in ovmf.metadata_items():
+            if desc.section_type() == SectionType.CPUID:
+                gctx.update_cpuid_page(desc.gpa)
+
+    if sev_hashes is not None and not ovmf.has_metadata_section(SectionType.SNP_KERNEL_HASHES):
+        raise RuntimeError("Kernel specified but OVMF metadata doesn't include SNP_KERNEL_HASHES section")
 
 
 def calc_snp_ovmf_hash(ovmf_file: str) -> bytes:
     ovmf = OVMF(ovmf_file)
 
     gctx = GCTX()
     gctx.update_normal_pages(ovmf.gpa(), ovmf.data())
     return gctx.ld()
 
 
 def snp_calc_launch_digest(vcpus: int, vcpu_sig: int, ovmf_file: str,
-                           kernel: str, initrd: str, append: str, ovmf_hash_str: str) -> bytes:
+                           kernel: str, initrd: str, append: str, ovmf_hash_str: str,
+                           vmm_type: VMMType = VMMType.QEMU) -> bytes:
 
     gctx = GCTX()
     ovmf = OVMF(ovmf_file)
 
     # Allow users to provide a precalculated OVMF hash.
     # Ignores the contents of the OVMF file in front of us.
     if ovmf_hash_str:
@@ -77,35 +94,40 @@
     else:
         gctx.update_normal_pages(ovmf.gpa(), ovmf.data())
 
     sev_hashes = None
     if kernel:
         sev_hashes = SevHashes(kernel, initrd, append)
 
-    snp_update_metadata_pages(gctx, ovmf, sev_hashes)
+    snp_update_metadata_pages(gctx, ovmf, sev_hashes, vmm_type)
 
-    vmsa = VMSA(SevMode.SEV_SNP, ovmf.sev_es_reset_eip(), vcpu_sig)
+    vmsa = VMSA(SevMode.SEV_SNP, ovmf.sev_es_reset_eip(), vcpu_sig, vmm_type)
     for vmsa_page in vmsa.pages(vcpus):
         gctx.update_vmsa_page(vmsa_page)
 
     return gctx.ld()
 
 
-def seves_calc_launch_digest(vcpus: int, vcpu_sig: int, ovmf_file: str, kernel: str, initrd: str, append: str) -> bytes:
+def seves_calc_launch_digest(vcpus: int, vcpu_sig: int, ovmf_file: str, kernel: str, initrd: str, append: str,
+                             vmm_type: VMMType = VMMType.QEMU) -> bytes:
     ovmf = OVMF(ovmf_file)
     launch_hash = hashlib.sha256(ovmf.data())
     if kernel:
+        if not ovmf.is_sev_hashes_table_supported():
+            raise RuntimeError("Kernel specified but OVMF doesn't support kernel/initrd/cmdline measurement")
         sev_hashes_table = SevHashes(kernel, initrd, append).construct_table()
         launch_hash.update(sev_hashes_table)
-    vmsa = VMSA(SevMode.SEV_ES, ovmf.sev_es_reset_eip(), vcpu_sig)
+    vmsa = VMSA(SevMode.SEV_ES, ovmf.sev_es_reset_eip(), vcpu_sig, vmm_type)
     for vmsa_page in vmsa.pages(vcpus):
         launch_hash.update(vmsa_page)
     return launch_hash.digest()
 
 
 def sev_calc_launch_digest(ovmf_file: str, kernel: str, initrd: str, append: str) -> bytes:
     ovmf = OVMF(ovmf_file)
     launch_hash = hashlib.sha256(ovmf.data())
     if kernel:
+        if not ovmf.is_sev_hashes_table_supported():
+            raise RuntimeError("Kernel specified but OVMF doesn't support kernel/initrd/cmdline measurement")
         sev_hashes_table = SevHashes(kernel, initrd, append).construct_table()
         launch_hash.update(sev_hashes_table)
     return launch_hash.digest()
```

### Comparing `sev-snp-measure-0.0.5/sevsnpmeasure/id_block.py` & `sev-snp-measure-0.0.6/sevsnpmeasure/id_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from cryptography.hazmat.primitives import serialization, hashes
 from cryptography.hazmat.backends import default_backend
 
 LaunchDigest = c_uint8 * 48
 ECParam = c_uint8 * 52
 ECSignature = c_uint8 * 512
 ECPubKey = c_uint8 * 1028
+Qx = c_uint8 * 72
+Qy = c_uint8 * 72
 
 DefaultIDs = bytes(0x20)
 DefaultVersion = 1
 DefaultGuestSVN = bytes(4)
 DefaultPolicy = 196608  # [0,0,3,0,0,0,0,0]
 DefaultKeyAlgo = 1
 CurveP384 = 2
@@ -70,16 +72,16 @@
         ("reserved3", ctypes.c_char * 892),
     ]
 
 
 class ECPublicKey(ctypes.Structure):
     _fields_ = [
         ("curve", ctypes.c_uint32),
-        ("qx", ctypes.c_char * 72),
-        ("qy", ctypes.c_char * 72),
+        ("qx", Qx),
+        ("qy", Qy),
         ("reserved", ctypes.c_char * 0x370)
     ]
 
 
 class SnpSignature(ctypes.Structure):
     _fields_ = [
         ("sig_r", ctypes.c_char * SnpSigLength),
@@ -153,16 +155,16 @@
     pub_key = priv_key.public_key()
     x = pub_key.public_numbers().x
     y = pub_key.public_numbers().y
     qx = x.to_bytes(0x48, byteorder="little")
     qy = y.to_bytes(0x48, byteorder="little")
     result = ECPublicKey(
         curve=CurveP384,
-        qx=qx,
-        qy=qy
+        qx=Qx.from_buffer_copy(qx),
+        qy=Qy.from_buffer_copy(qy),
     )
     return bytes(result)
 
 
 def pub_to_digest(priv_key: ec.EllipticCurvePrivateKey) -> bytes:
     hasher = hashlib.new("sha384")
     pub_bytes = marshal_ec_public_key(priv_key)
```

### Comparing `sev-snp-measure-0.0.5/sevsnpmeasure/ovmf.py` & `sev-snp-measure-0.0.6/sevsnpmeasure/ovmf.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,20 @@
 
     def table_item(self, guid: str) -> bytes:
         return self._table[guid]
 
     def metadata_items(self):
         return self._metadata_items
 
+    def has_metadata_section(self, section_type: SectionType) -> bool:
+        return any(True for s in self.metadata_items() if s.section_type() == section_type)
+
+    def is_sev_hashes_table_supported(self) -> bool:
+        return self.SEV_HASH_TABLE_RV_GUID in self._table and self.sev_hashes_table_gpa() != 0
+
     def sev_hashes_table_gpa(self) -> int:
         if self.SEV_HASH_TABLE_RV_GUID not in self._table:
             raise RuntimeError("Can't find SEV_HASH_TABLE_RV_GUID entry in OVMF table")
         entry = self._table[self.SEV_HASH_TABLE_RV_GUID]
         return int.from_bytes(entry[:4], byteorder='little')
 
     def sev_es_reset_eip(self) -> int:
```

### Comparing `sev-snp-measure-0.0.5/sevsnpmeasure/sev_hashes.py` & `sev-snp-measure-0.0.6/sevsnpmeasure/sev_hashes.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.5/sevsnpmeasure/sev_mode.py` & `sev-snp-measure-0.0.6/sevsnpmeasure/sev_mode.py`

 * *Files identical despite different names*

### Comparing `sev-snp-measure-0.0.5/sevsnpmeasure/vcpu_types.py` & `sev-snp-measure-0.0.6/sevsnpmeasure/vcpu_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,8 +35,10 @@
     'EPYC-Rome': cpu_sig(family=23, model=49, stepping=0),
     'EPYC-Rome-v1': cpu_sig(family=23, model=49, stepping=0),
     'EPYC-Rome-v2': cpu_sig(family=23, model=49, stepping=0),
     'EPYC-Rome-v3': cpu_sig(family=23, model=49, stepping=0),
     'EPYC-Milan': cpu_sig(family=25, model=1, stepping=1),
     'EPYC-Milan-v1': cpu_sig(family=25, model=1, stepping=1),
     'EPYC-Milan-v2': cpu_sig(family=25, model=1, stepping=1),
+    'EPYC-Genoa': cpu_sig(family=25, model=17, stepping=0),
+    'EPYC-Genoa-v1': cpu_sig(family=25, model=17, stepping=0),
 }
```

### Comparing `sev-snp-measure-0.0.5/sevsnpmeasure/vmsa.py` & `sev-snp-measure-0.0.6/sevsnpmeasure/vmsa.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 
 import ctypes
 from ctypes import c_uint8, c_uint16, c_uint32, c_uint64
 from typing import Iterator
 from .sev_mode import SevMode
+from .vmm_types import VMMType
 
 
 # VMCB Segment (struct vmcb_seg in the linux kernel)
 class VmcbSeg(ctypes.Structure):
     _pack_ = 1
     _fields_ = [
         ("selector", c_uint16),
@@ -136,48 +137,64 @@
     ]
 
 
 class VMSA(object):
     BSP_EIP = 0xfffffff0
 
     @staticmethod
-    def build_save_area(eip: int, sev_features: int, vcpu_sig: int):
+    def build_save_area(eip: int, sev_features: int, vcpu_sig: int, vmm_type: VMMType = VMMType.QEMU):
+        # QEMU and EC2 differ slightly on initial register state
+        if vmm_type == VMMType.QEMU:
+            cs_flags = 0x9b
+            ss_flags = 0x93
+            tr_flags = 0x8b
+            rdx = vcpu_sig
+        elif vmm_type == VMMType.ec2:
+            cs_flags = 0x9b
+            if eip == 0xfffffff0:
+                cs_flags = 0x9a
+            ss_flags = 0x92
+            tr_flags = 0x83
+            rdx = 0
+        else:
+            raise ValueError("unknown VMM type")
+
         return SevEsSaveArea(
             es=VmcbSeg(0, 0x93, 0xffff, 0),
-            cs=VmcbSeg(0xf000, 0x9b, 0xffff, eip & 0xffff0000),
-            ss=VmcbSeg(0, 0x93, 0xffff, 0),
+            cs=VmcbSeg(0xf000, cs_flags, 0xffff, eip & 0xffff0000),
+            ss=VmcbSeg(0, ss_flags, 0xffff, 0),
             ds=VmcbSeg(0, 0x93, 0xffff, 0),
             fs=VmcbSeg(0, 0x93, 0xffff, 0),
             gs=VmcbSeg(0, 0x93, 0xffff, 0),
             gdtr=VmcbSeg(0, 0, 0xffff, 0),
             idtr=VmcbSeg(0, 0, 0xffff, 0),
             ldtr=VmcbSeg(0, 0x82, 0xffff, 0),
-            tr=VmcbSeg(0, 0x8b, 0xffff, 0),
+            tr=VmcbSeg(0, tr_flags, 0xffff, 0),
             efer=0x1000,  # KVM enables EFER_SVME
             cr4=0x40,     # KVM enables X86_CR4_MCE
             cr0=0x10,
             dr7=0x400,
             dr6=0xffff0ff0,
             rflags=0x2,
             rip=eip & 0xffff,
             g_pat=0x7040600070406,  # PAT MSR: See AMD APM Vol 2, Section A.3
-            rdx=vcpu_sig,
+            rdx=rdx,
             sev_features=sev_features,
             xcr0=0x1,
         )
 
-    def __init__(self, sev_mode: SevMode, ap_eip: int, vcpu_sig: int):
+    def __init__(self, sev_mode: SevMode, ap_eip: int, vcpu_sig: int, vmm_type: VMMType = VMMType.QEMU):
         if sev_mode == SevMode.SEV_SNP:
             sev_features = 0x1
         else:
             sev_features = 0x0
 
-        self.bsp_save_area = VMSA.build_save_area(self.BSP_EIP, sev_features, vcpu_sig)
+        self.bsp_save_area = VMSA.build_save_area(self.BSP_EIP, sev_features, vcpu_sig, vmm_type)
         if ap_eip:
-            self.ap_save_area = VMSA.build_save_area(ap_eip, sev_features, vcpu_sig)
+            self.ap_save_area = VMSA.build_save_area(ap_eip, sev_features, vcpu_sig, vmm_type)
 
     def pages(self, vcpus: int) -> Iterator[bytes]:
         """
         Generate VMSA pages
         """
         for i in range(vcpus):
             if i == 0:
```

### Comparing `sev-snp-measure-0.0.5/tests/test_id_block.py` & `sev-snp-measure-0.0.6/tests/test_id_block.py`

 * *Files identical despite different names*

