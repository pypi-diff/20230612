# Comparing `tmp/python-rtmidi-1.5.0.tar.gz` & `tmp/python-rtmidi-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-rtmidi-1.5.0.tar", last modified: Tue May 23 15:02:06 2023, max compression
+gzip compressed data, was "python-rtmidi-1.5.1.tar", last modified: Mon Jun 12 14:09:30 2023, max compression
```

## Comparing `python-rtmidi-1.5.0.tar` & `python-rtmidi-1.5.1.tar`

### file list

```diff
@@ -1,176 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:02:01.428790 python-rtmidi-1.5.0/
--rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.flake8
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (123)     2232 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/workflows/development.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     2124 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/workflows/production.yml
--rw-rw-r--   0 runner    (1001) docker     (123)     1553 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/workflows/tests.yml
--rw-rw-r--   0 runner    (1001) docker     (123)      571 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (123)      118 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.gitmodules
--rw-rw-r--   0 runner    (1001) docker     (123)      246 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/AUTHORS.md
--rw-rw-r--   0 runner    (1001) docker     (123)    21032 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (123)     3849 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/INSTALL-windows.md
--rw-rw-r--   0 runner    (1001) docker     (123)     8352 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/INSTALL.md
--rw-rw-r--   0 runner    (1001) docker     (123)     2771 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/LICENSE.md
--rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/MANIFEST.in
--rw-rw-r--   0 runner    (1001) docker     (123)     2497 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/Makefile
--rw-rw-r--   0 runner    (1001) docker     (123)     2778 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/README.md
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/
--rw-rw-r--   0 runner    (1001) docker     (123)     6778 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/Makefile
--rw-rw-r--   0 runner    (1001) docker     (123)      759 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/api.rst.inc
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/authors.md
--rwxrwxr-x   0 runner    (1001) docker     (123)     8521 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/conf.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3257 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/contributing.rst
--rw-rw-r--   0 runner    (1001) docker     (123)       33 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/history.md
--rw-rw-r--   0 runner    (1001) docker     (123)      478 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (123)       39 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/install-windows.md
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/installation.md
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/license.md
--rw-rw-r--   0 runner    (1001) docker     (123)     6467 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/make.bat
--rw-rw-r--   0 runner    (1001) docker     (123)       55 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/modules.rst
--rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/readme.md
--rw-rw-r--   0 runner    (1001) docker     (123)     1337 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/rtmidi.rst
--rw-rw-r--   0 runner    (1001) docker     (123)     1129 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/usage.rst
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/
--rw-rw-r--   0 runner    (1001) docker     (123)     1687 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/ccstore.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2398 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/midiclock.py
--rw-rw-r--   0 runner    (1001) docker     (123)     8741 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/midioutwrapper.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2585 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/recvrpn.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/
--rw-rw-r--   0 runner    (1001) docker     (123)      545 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/contextmanager.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1359 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/midiin_callback.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1050 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/midiin_poll.py
--rwxrwxr-x   0 runner    (1001) docker     (123)      991 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/midiout.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1012 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/noteon2osc.py
--rw-rw-r--   0 runner    (1001) docker     (123)      765 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/panic.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1571 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/probe_ports.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/
--rw-rw-r--   0 runner    (1001) docker     (123)     2195 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/README.rst
--rw-rw-r--   0 runner    (1001) docker     (123)      275 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/break-on-through.txt
--rwxrwxr-x   0 runner    (1001) docker     (123)     6485 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/drumseq.py
--rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_01.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_02.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      255 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_03.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      206 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_04.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      294 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_05.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_06.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_07.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_08.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_09.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      435 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_10.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      299 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_11.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_12.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      157 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/funkydrummer.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      205 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/rosanna-shuffle.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/template.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/
--rw-rw-r--   0 runner    (1001) docker     (123)    45974 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/000-playback.mp3
--rw-rw-r--   0 runner    (1001) docker     (123)     2506 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/000-sheet.pdf
--rw-rw-r--   0 runner    (1001) docker     (123)     5624 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/README.rst
--rw-rw-r--   0 runner    (1001) docker     (123)      522 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/example.cfg
--rw-rw-r--   0 runner    (1001) docker     (123)     7132 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/midi2command.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midifilter/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midifilter/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3667 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midifilter/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3119 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midifilter/filters.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     5328 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sendsysex.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sequencer/
--rw-rw-r--   0 runner    (1001) docker     (123)     7155 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sequencer/sequencer.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysex/
--rwxrwxr-x   0 runner    (1001) docker     (123)      745 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysex/send_sysex.py
--rwxrwxr-x   0 runner    (1001) docker     (123)     1067 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysex/send_sysex_file.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     7022 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (123)    11493 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/manufacturers.csv
--rw-rw-r--   0 runner    (1001) docker     (123)    12337 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/manufacturers.py
--rw-rw-r--   0 runner    (1001) docker     (123)    12147 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/models.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3247 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/wavetablemodstep.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2687 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)      801 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/meson_options.txt
--rwxrwxr-x   0 runner    (1001) docker     (123)      405 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/meson_postinstall.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3004 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (123)       91 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/requirements-dev.in
--rw-rw-r--   0 runner    (1001) docker     (123)     2845 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/requirements-dev.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/
--rw-rw-r--   0 runner    (1001) docker     (123)      165 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1826 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (123)     7533 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/midiconstants.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9261 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/midiutil.py
--rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/version.py.in
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:02:02.088810 python-rtmidi-1.5.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)   735881 2023-05-23 15:02:02.088810 python-rtmidi-1.5.0/src/_rtmidi.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)    39464 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/src/_rtmidi.pyx
--rw-rw-r--   0 runner    (1001) docker     (123)      857 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/src/meson.build
--rwxrwxr-x   0 runner    (1001) docker     (123)     1260 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/src/meson_dist_cython.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/
--rw-rw-r--   0 runner    (1001) docker     (123)     9589 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/CMakeLists.txt
--rw-rw-r--   0 runner    (1001) docker     (123)     1349 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (123)      533 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/Makefile.am
--rw-rw-r--   0 runner    (1001) docker     (123)     2396 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/README.md
--rw-rw-r--   0 runner    (1001) docker     (123)   126832 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/RtMidi.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)    27069 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/RtMidi.h
--rwxrwxr-x   0 runner    (1001) docker     (123)     2884 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/autogen.sh
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/cmake/
--rw-rw-r--   0 runner    (1001) docker     (123)      252 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/cmake/RtMidi-config.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (123)      940 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in
--rw-rw-r--   0 runner    (1001) docker     (123)     9307 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/configure.ac
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/
--rw-rw-r--   0 runner    (1001) docker     (123)     8909 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi.go
--rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.h
--rw-rw-r--   0 runner    (1001) docker     (123)      758 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/
--rw-rw-r--   0 runner    (1001) docker     (123)      682 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/Makefile.am
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/
--rw-rw-r--   0 runner    (1001) docker     (123)    81155 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/Doxyfile.in
--rw-rw-r--   0 runner    (1001) docker     (123)      254 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/footer.html
--rw-rw-r--   0 runner    (1001) docker     (123)      494 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/header.html
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/samples/
--rw-rw-r--   0 runner    (1001) docker     (123)      173 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/samples/getting_started.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)    21717 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/tutorial.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/images/
--rw-rw-r--   0 runner    (1001) docker     (123)     3527 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/images/ccrma.gif
--rw-rw-r--   0 runner    (1001) docker     (123)     4614 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/images/mcgill.gif
--rw-rw-r--   0 runner    (1001) docker     (123)     7130 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/release.txt
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/m4/
--rw-rw-r--   0 runner    (1001) docker     (123)    19367 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/msw/
--rw-rw-r--   0 runner    (1001) docker     (123)      171 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/msw/readme
--rwxrwxr-x   0 runner    (1001) docker     (123)      883 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/msw/rtmidilib.sln
--rwxrwxr-x   0 runner    (1001) docker     (123)     3734 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/msw/rtmidilib.vcproj
--rw-rw-r--   0 runner    (1001) docker     (123)      388 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/rtmidi-config.in
--rw-rw-r--   0 runner    (1001) docker     (123)      369 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/rtmidi.pc.in
--rw-rw-r--   0 runner    (1001) docker     (123)    10140 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/rtmidi_c.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     9470 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/rtmidi_c.h
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Debug/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Debug/.placeholder
--rw-rw-r--   0 runner    (1001) docker     (123)     1018 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Makefile.am
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Release/
--rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Release/.placeholder
--rw-rw-r--   0 runner    (1001) docker     (123)     1311 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/RtMidi.dsw
--rw-rw-r--   0 runner    (1001) docker     (123)     5284 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/apinames.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     2873 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/cmidiin.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/cmidiin.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     5541 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiclock.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     3147 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiout.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiout.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     2138 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiprobe.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4356 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiprobe.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     2361 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/qmidiin.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/qmidiin.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)     3926 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/sysextest.cpp
--rw-rw-r--   0 runner    (1001) docker     (123)     4360 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/sysextest.dsp
--rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/testcapi.c
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/
--rw-rw-r--   0 runner    (1001) docker     (123)     2484 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/test_delete.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2100 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/test_errorcallback.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2299 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/test_errors.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9256 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/test_rtmidi.py
--rw-rw-r--   0 runner    (1001) docker     (123)      298 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tox.ini
--rwxrwxr-x   0 runner    (1001) docker     (123)      346 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/update-docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-05-23 15:02:06.152952 python-rtmidi-1.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:09:25.630277 python-rtmidi-1.5.1/
+-rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.flake8
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2384 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/workflows/development.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     2276 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/workflows/production.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     1707 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.github/workflows/tests.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      571 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (123)      118 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/.gitmodules
+-rw-rw-r--   0 runner    (1001) docker     (123)      246 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/AUTHORS.md
+-rw-rw-r--   0 runner    (1001) docker     (123)    21032 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     3849 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/INSTALL-windows.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     8352 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/INSTALL.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     2771 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/LICENSE.md
+-rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/MANIFEST.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     2497 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (123)     2778 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/README.md
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/
+-rw-rw-r--   0 runner    (1001) docker     (123)     6778 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (123)      759 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/api.rst.inc
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/authors.md
+-rwxrwxr-x   0 runner    (1001) docker     (123)     8521 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/conf.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3257 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/contributing.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)       33 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/history.md
+-rw-rw-r--   0 runner    (1001) docker     (123)      478 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)       39 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/install-windows.md
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/installation.md
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/license.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     6467 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/make.bat
+-rw-rw-r--   0 runner    (1001) docker     (123)       55 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/modules.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/readme.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     1337 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/rtmidi.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)     1129 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/docs/usage.rst
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1687 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/ccstore.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2398 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/midiclock.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     8741 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/midioutwrapper.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2585 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/advanced/recvrpn.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/
+-rw-rw-r--   0 runner    (1001) docker     (123)      545 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/contextmanager.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1359 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/midiin_callback.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1050 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/midiin_poll.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)      991 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/midiout.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1012 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/noteon2osc.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      765 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/panic.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1571 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/basic/probe_ports.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2195 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)      275 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/break-on-through.txt
+-rwxrwxr-x   0 runner    (1001) docker     (123)     6485 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/drumseq.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_01.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_02.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      255 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_03.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      206 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_04.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      294 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_05.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_06.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_07.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_08.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_09.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      435 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_10.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      299 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_11.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/example_12.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      157 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/funkydrummer.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      205 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/rosanna-shuffle.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/drumseq/template.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/
+-rw-rw-r--   0 runner    (1001) docker     (123)    45974 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/000-playback.mp3
+-rw-rw-r--   0 runner    (1001) docker     (123)     2506 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/000-sheet.pdf
+-rw-rw-r--   0 runner    (1001) docker     (123)     5624 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)      522 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/example.cfg
+-rw-rw-r--   0 runner    (1001) docker     (123)     7132 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midi2command/midi2command.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midifilter/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midifilter/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3667 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midifilter/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3119 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/midifilter/filters.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     5328 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sendsysex.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sequencer/
+-rw-rw-r--   0 runner    (1001) docker     (123)     7155 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sequencer/sequencer.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysex/
+-rwxrwxr-x   0 runner    (1001) docker     (123)      745 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysex/send_sysex.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1067 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysex/send_sysex_file.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     7022 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    11493 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/manufacturers.csv
+-rw-rw-r--   0 runner    (1001) docker     (123)    12337 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/manufacturers.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    12147 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/sysexsaver/models.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3247 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/examples/wavetablemodstep.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3018 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)      801 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/meson_options.txt
+-rwxrwxr-x   0 runner    (1001) docker     (123)      405 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/meson_postinstall.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3122 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (123)       91 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/requirements-dev.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     2845 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/requirements-dev.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/
+-rw-rw-r--   0 runner    (1001) docker     (123)      165 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1881 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)     7533 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/midiconstants.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9261 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/midiutil.py
+-rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/rtmidi/version.py.in
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:09:26.274290 python-rtmidi-1.5.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   737320 2023-06-12 14:09:26.274290 python-rtmidi-1.5.1/src/_rtmidi.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)    39588 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/src/_rtmidi.pyx
+-rw-rw-r--   0 runner    (1001) docker     (123)      857 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/src/meson.build
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1261 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/src/meson_dist_cython.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/
+-rw-rw-r--   0 runner    (1001) docker     (123)     9589 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)     1349 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (123)      533 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/Makefile.am
+-rw-rw-r--   0 runner    (1001) docker     (123)     2396 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/README.md
+-rw-rw-r--   0 runner    (1001) docker     (123)   126832 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/RtMidi.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)    27069 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/RtMidi.h
+-rwxrwxr-x   0 runner    (1001) docker     (123)     2884 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/autogen.sh
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/cmake/
+-rw-rw-r--   0 runner    (1001) docker     (123)      252 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/cmake/RtMidi-config.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      940 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     9307 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/configure.ac
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/
+-rw-rw-r--   0 runner    (1001) docker     (123)     8909 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi.go
+-rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      758 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/
+-rw-rw-r--   0 runner    (1001) docker     (123)      682 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/Makefile.am
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/
+-rw-rw-r--   0 runner    (1001) docker     (123)    81155 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/Doxyfile.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      254 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/footer.html
+-rw-rw-r--   0 runner    (1001) docker     (123)      494 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/header.html
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/samples/
+-rw-rw-r--   0 runner    (1001) docker     (123)      173 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/samples/getting_started.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)    21717 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/tutorial.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/images/
+-rw-rw-r--   0 runner    (1001) docker     (123)     3527 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/images/ccrma.gif
+-rw-rw-r--   0 runner    (1001) docker     (123)     4614 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/images/mcgill.gif
+-rw-rw-r--   0 runner    (1001) docker     (123)     7130 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/doc/release.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/m4/
+-rw-rw-r--   0 runner    (1001) docker     (123)    19367 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/msw/
+-rw-rw-r--   0 runner    (1001) docker     (123)      171 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/msw/readme
+-rwxrwxr-x   0 runner    (1001) docker     (123)      883 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/msw/rtmidilib.sln
+-rwxrwxr-x   0 runner    (1001) docker     (123)     3734 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/msw/rtmidilib.vcproj
+-rw-rw-r--   0 runner    (1001) docker     (123)      388 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/rtmidi-config.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      369 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/rtmidi.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (123)    10208 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/rtmidi_c.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     9525 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/rtmidi_c.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Debug/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Debug/.placeholder
+-rw-rw-r--   0 runner    (1001) docker     (123)     1018 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Makefile.am
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Release/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/Release/.placeholder
+-rw-rw-r--   0 runner    (1001) docker     (123)     1311 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/RtMidi.dsw
+-rw-rw-r--   0 runner    (1001) docker     (123)     5284 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/apinames.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     2873 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/cmidiin.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/cmidiin.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     5541 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiclock.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     3147 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiout.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiout.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     2138 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiprobe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4356 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/midiprobe.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     2361 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/qmidiin.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/qmidiin.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     3926 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/sysextest.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4360 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/sysextest.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-06-06 16:06:52.000000 python-rtmidi-1.5.1/src/rtmidi/tests/testcapi.c
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2922 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_basic.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2484 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_delete.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2100 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_errorcallback.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2299 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_errors.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9256 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tests/test_rtmidi.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      298 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/tox.ini
+-rwxrwxr-x   0 runner    (1001) docker     (123)      346 2023-06-12 14:06:46.000000 python-rtmidi-1.5.1/update-docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-06-12 14:09:30.826380 python-rtmidi-1.5.1/PKG-INFO
```

### Comparing `python-rtmidi-1.5.0/.github/workflows/development.yml` & `python-rtmidi-1.5.1/.github/workflows/development.yml`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,17 @@
    - uses: actions/checkout@v3
      with:
        submodules: true
 
    - name: Install ninja
      run: pipx install ninja
 
+   - name: Install alsa deps
+     run: sudo apt-get install libasound2-dev
+
    - name: Build sdist
      run: pipx run build --sdist
 
    - name: Check metadata
      run: pipx run twine check --strict dist/*
 
    - uses: actions/upload-artifact@v3
@@ -40,14 +43,17 @@
         os: [ubuntu-latest, windows-latest, macos-latest]
     steps:
 
     - uses: actions/checkout@v3
       with:
         submodules: true
 
+    - uses: ilammy/msvc-dev-cmd@v1
+      if: matrix.os == 'windows-latest'
+
     - name: Build wheels
       uses: pypa/cibuildwheel@v2.12.3
 
     - uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
```

### Comparing `python-rtmidi-1.5.0/.github/workflows/production.yml` & `python-rtmidi-1.5.1/.github/workflows/production.yml`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,17 @@
    - uses: actions/checkout@v3
      with:
        submodules: true
 
    - name: Install ninja
      run: pipx install ninja
 
+   - name: Install alsa deps
+     run: sudo apt-get install libasound2-dev
+
    - name: Build sdist
      run: pipx run build --sdist
 
    - name: Check metadata
      run: pipx run twine check --strict dist/*
 
    - uses: actions/upload-artifact@v3
@@ -40,14 +43,17 @@
         os: [ubuntu-latest, windows-latest, macos-latest]
     steps:
 
     - uses: actions/checkout@v3
       with:
         submodules: true
 
+    - uses: ilammy/msvc-dev-cmd@v1
+      if: matrix.os == 'windows-latest'
+
     - name: Build wheels
       uses: pypa/cibuildwheel@v2.12.3
 
     - uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
```

### Comparing `python-rtmidi-1.5.0/.github/workflows/tests.yml` & `python-rtmidi-1.5.1/.github/workflows/tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 name: Build sdist and wheel for testing purposes
 
 on:
   push:
     branches:
-      - rtmidi-5.0.0
+      - improve-build
   pull_request:
     branches:
-      - rtmidi-5.0.0
+      - improve-build
 
 jobs:
   build_sdist:
    name: Build sdist
    runs-on: ubuntu-latest
    steps:
 
    - uses: actions/checkout@v3
      with:
        submodules: true
 
    - name: Install ninja
      run: pipx install ninja
 
+   - name: Install alsa deps
+     run: sudo apt-get install libasound2-dev
+
    - name: Build sdist
      run: pipx run build --sdist
 
    - name: Check metadata
      run: pipx run twine check --strict dist/*
 
    - uses: actions/upload-artifact@v3
@@ -40,14 +43,17 @@
         os: [ubuntu-latest, windows-latest, macos-latest]
     steps:
 
     - uses: actions/checkout@v3
       with:
         submodules: true
 
+    - uses: ilammy/msvc-dev-cmd@v1
+      if: matrix.os == 'windows-latest'
+
     - name: Build wheels
       uses: pypa/cibuildwheel@v2.12.3
 
     - uses: actions/upload-artifact@v3
       with:
         path: wheelhouse/*.whl
```

### Comparing `python-rtmidi-1.5.0/.gitignore` & `python-rtmidi-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/CHANGELOG.md` & `python-rtmidi-1.5.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/INSTALL-windows.md` & `python-rtmidi-1.5.1/INSTALL-windows.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/INSTALL.md` & `python-rtmidi-1.5.1/INSTALL.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/LICENSE.md` & `python-rtmidi-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/Makefile` & `python-rtmidi-1.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/README.md` & `python-rtmidi-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/docs/Makefile` & `python-rtmidi-1.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/docs/api.rst.inc` & `python-rtmidi-1.5.1/docs/api.rst.inc`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/docs/conf.py` & `python-rtmidi-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/docs/contributing.rst` & `python-rtmidi-1.5.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/docs/make.bat` & `python-rtmidi-1.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/docs/rtmidi.rst` & `python-rtmidi-1.5.1/docs/rtmidi.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/docs/usage.rst` & `python-rtmidi-1.5.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/advanced/ccstore.py` & `python-rtmidi-1.5.1/examples/advanced/ccstore.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/advanced/midiclock.py` & `python-rtmidi-1.5.1/examples/advanced/midiclock.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/advanced/midioutwrapper.py` & `python-rtmidi-1.5.1/examples/advanced/midioutwrapper.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/advanced/recvrpn.py` & `python-rtmidi-1.5.1/examples/advanced/recvrpn.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/basic/contextmanager.py` & `python-rtmidi-1.5.1/examples/basic/contextmanager.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/basic/midiin_callback.py` & `python-rtmidi-1.5.1/examples/basic/midiin_callback.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/basic/midiin_poll.py` & `python-rtmidi-1.5.1/examples/basic/midiin_poll.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/basic/midiout.py` & `python-rtmidi-1.5.1/examples/basic/midiout.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/basic/noteon2osc.py` & `python-rtmidi-1.5.1/examples/basic/noteon2osc.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/basic/panic.py` & `python-rtmidi-1.5.1/examples/basic/panic.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/basic/probe_ports.py` & `python-rtmidi-1.5.1/examples/basic/probe_ports.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/drumseq/README.rst` & `python-rtmidi-1.5.1/examples/drumseq/README.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/drumseq/drumseq.py` & `python-rtmidi-1.5.1/examples/drumseq/drumseq.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/midi2command/000-playback.mp3` & `python-rtmidi-1.5.1/examples/midi2command/000-playback.mp3`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/midi2command/000-sheet.pdf` & `python-rtmidi-1.5.1/examples/midi2command/000-sheet.pdf`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/midi2command/README.rst` & `python-rtmidi-1.5.1/examples/midi2command/README.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/midi2command/example.cfg` & `python-rtmidi-1.5.1/examples/midi2command/example.cfg`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/midi2command/midi2command.py` & `python-rtmidi-1.5.1/examples/midi2command/midi2command.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/midifilter/__main__.py` & `python-rtmidi-1.5.1/examples/midifilter/__main__.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/midifilter/filters.py` & `python-rtmidi-1.5.1/examples/midifilter/filters.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/sendsysex.py` & `python-rtmidi-1.5.1/examples/sendsysex.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/sequencer/sequencer.py` & `python-rtmidi-1.5.1/examples/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/sysex/send_sysex.py` & `python-rtmidi-1.5.1/examples/sysex/send_sysex.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/sysex/send_sysex_file.py` & `python-rtmidi-1.5.1/examples/sysex/send_sysex_file.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/sysexsaver/__main__.py` & `python-rtmidi-1.5.1/examples/sysexsaver/__main__.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/sysexsaver/manufacturers.csv` & `python-rtmidi-1.5.1/examples/sysexsaver/manufacturers.csv`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/sysexsaver/manufacturers.py` & `python-rtmidi-1.5.1/examples/sysexsaver/manufacturers.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/sysexsaver/models.py` & `python-rtmidi-1.5.1/examples/sysexsaver/models.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/examples/wavetablemodstep.py` & `python-rtmidi-1.5.1/examples/wavetablemodstep.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/meson.build` & `python-rtmidi-1.5.1/meson.build`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,77 @@
 project(
     'python-rtmidi',
     'cpp',
-    version: '1.5.0',
+    version: '1.5.1',
     license: 'MIT',
     default_options: [
         'warning_level=2'
     ],
     meson_version: '>=0.63.0'
 )
 
 cpp = meson.get_compiler('cpp')
 
-## From https://github.com/numpy/numpy/blob/main/numpy/meson.build
-# Platform detection
-if host_machine.system() == 'windows' and cpp.get_id() == 'gcc'
-  # For mingw-w64, link statically against the UCRT.
-  gcc_link_args = ['-lucrt', '-static']
-
-  add_project_link_arguments(gcc_link_args, language: ['c', 'cpp'])
-  # Force gcc to float64 long doubles for compatibility with MSVC
-  # builds, for C only.
-  add_project_arguments('-mlong-double-64', language: 'c')
-  # Make fprintf("%zd") work (see https://github.com/rgommers/scipy/issues/118)
-  add_project_arguments('-D__USE_MINGW_ANSI_STDIO=1', language: ['c', 'cpp'])
-  # Manual add of MS_WIN64 macro when not using MSVC.
-  # https://bugs.python.org/issue28267
-  add_project_arguments('-DMS_WIN64', language: ['c', 'cpp'])
-endif
-##
-
-if host_machine.system() == 'darwin'
-  # Enable c++11 support
-  add_project_arguments('-std=c++11', language: ['cpp'])
-endif
-
-# Dependencies
+# Jack API (portable)
 jack2_dep = dependency('jack', version: '>=1.9.11', required: false)
 jack1_dep = dependency('jack', version: ['>=0.125.0', '<1.0'], required: false)
-alsa_dep = dependency('alsa', required: false)
-threads_dep = dependency('threads')
-coremidi_dep = dependency(
-    'appleframeworks',
-    modules: ['coreaudio', 'coremidi', 'foundation'],
-    required: false
-)
-winmm_dep = cpp.find_library('winmm', required: false)
 
 if not jack2_dep.found() and jack1_dep.found()
     jack_dep = jack1_dep
 elif jack2_dep.found()
     jack_dep = jack2_dep
 else
     warning('No version of JACK found, which is recent enough (jack2>=1.9.11 or jack1>=0.125.0)')
     jack_dep = disabler()
 endif
 
+
+jack_not_found = jack_dep.found() ? false : true
+
+## From https://github.com/numpy/numpy/blob/main/numpy/meson.build
+# Platform dependent config
+if host_machine.system() == 'windows'
+    # WINDOWS
+    if cpp.get_id() == 'gcc'
+        # For mingw-w64, link statically against the UCRT.
+        gcc_link_args = ['-lucrtbase', '-static']
+        add_project_link_arguments(gcc_link_args, language: ['c', 'cpp'])
+        # Make fprintf("%zd") work (see https://github.com/rgommers/scipy/issues/118)
+        add_project_arguments('-D__USE_MINGW_ANSI_STDIO=1', language: ['c', 'cpp'])
+        # Manual add of MS_WIN64 macro when not using MSVC.
+        # https://bugs.python.org/issue28267
+        add_project_arguments('-DMS_WIN64', language: ['c', 'cpp'])
+    elif cpp.get_id() == 'msvc'
+        # Force gcc to float64 long doubles for compatibility with MSVC
+        # builds, for C only.
+        add_project_arguments('-mlong-double-64', language: 'c')
+    endif
+
+    # API
+    winmm_dep = cpp.find_library('winmm', required: jack_not_found)
+elif host_machine.system() == 'darwin'
+    # OSX
+
+    # Enable c++11 support
+    add_project_arguments('-std=c++11', language: ['cpp'])
+
+    # API
+    coremidi_dep = dependency(
+        'appleframeworks',
+        modules: ['coreaudio', 'coremidi', 'foundation'],
+        required: jack_not_found
+    )
+else
+    # LINUX
+
+    # API
+    alsa_dep = dependency('alsa', required: jack_not_found)
+    threads_dep = dependency('threads')
+endif # Platform detection
+
 pymod = import('python')
 python = pymod.find_installation(get_option('python'), required: true)
 
 # Generate _rtmidi extension source
 subdir('src')
 
 # Build & install C++ extension module and Python package
@@ -68,12 +81,13 @@
     postinstall_script = files('meson_postinstall.py')
     meson.add_install_script(python, postinstall_script)
 endif
 
 summary({
     'Debug messages (verbose)': get_option('verbose'),
     'Build for wheel': get_option('wheel'),
+    'JACK support': jack_dep.found() and get_option('jack'),
     'ALSA support': host_machine.system() == 'linux' and alsa_dep.found() and get_option('alsa'),
     'CoreMIDI support': host_machine.system() == 'darwin' and coremidi_dep.found() and get_option('coremidi'),
-    'JACK support': jack_dep.found() and get_option('jack'),
     'Window MM support': host_machine.system() == 'windows' and winmm_dep.found() and get_option('winmm'),
 }, section: 'Configuration')
+
```

### Comparing `python-rtmidi-1.5.0/meson_options.txt` & `python-rtmidi-1.5.1/meson_options.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/pyproject.toml` & `python-rtmidi-1.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     "multimedia",
     "music",
     "rtmidi",
 ]
 meson-python-option-name = "python"
 meson-options = [
     "-Dwheel=true",
+    "-Dverbose=true",
     "--buildtype=plain"
 ]
 
 [project.license]
 file = "LICENSE.md"
 
 [project.urls]
@@ -80,14 +81,18 @@
 [tool.cibuildwheel]
 # Switch to using build
 build-frontend = "build"
 skip = "pp*"
 manylinux-x86_64-image = "manylinux_2_28"
 manylinux-aarch64-image = "manylinux_2_28"
 
+# Run the package tests using `pytest`
+test-command = "pytest {package}/tests/test_basic.py"
+test-requires = "pytest"
+
 # Install system library
 [tool.cibuildwheel.linux]
 build = "cp3{8,9,10,11}-manylinux*"
 archs = ["auto64"]
 before-all = [
     "dnf -y install alsa-lib-devel alsa-utils",
     "pipx install ninja",
@@ -106,10 +111,8 @@
 before-all = [
     "pipx install ninja",
 ]
 
 [tool.cibuildwheel.windows]
 build = "cp3{8,9,10,11}-win*"
 archs = ["AMD64"]
-before-all = [
-    "pipx install ninja",
-]
+build-verbosity = 1
```

### Comparing `python-rtmidi-1.5.0/requirements-dev.txt` & `python-rtmidi-1.5.1/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/rtmidi/meson.build` & `python-rtmidi-1.5.1/rtmidi/meson.build`

 * *Files 14% similar despite different names*

```diff
@@ -21,26 +21,29 @@
 
 if host_machine.system() == 'linux' and alsa_dep.found() and get_option('alsa')
     defines += ['-D__LINUX_ALSA__']
     dependencies += [alsa_dep]
 endif
 
 if host_machine.system() == 'windows' and get_option('winmm')
+    defines += ['-D__WINDOWS_MM__']
     if meson.get_compiler('cpp').get_id() != 'gcc'
-        defines += ['-D__WINDOWS_MM__', '/EHsc']
+        defines += ['/EHsc']
     endif
     dependencies += [winmm_dep]
 endif
 
 if jack_dep.found() and get_option('jack')
     defines += ['-D__UNIX_JACK__', '-DJACK_HAS_PORT_RENAME']
     dependencies += [jack_dep]
 endif
 
-if not get_option('verbose')
+if get_option('verbose')
+    defines += ['-D__RTMIDI_DEBUG__']
+else
     defines += ['-D__RTMIDI_SILENCE_WARNINGS__']
 endif
 
 
 # Build and install the extension module
 module = python.extension_module(
     '_rtmidi',
```

### Comparing `python-rtmidi-1.5.0/rtmidi/midiconstants.py` & `python-rtmidi-1.5.1/rtmidi/midiconstants.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/rtmidi/midiutil.py` & `python-rtmidi-1.5.1/rtmidi/midiutil.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/_rtmidi.cpp` & `python-rtmidi-1.5.1/src/_rtmidi.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -989,15 +993,15 @@
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_7_rtmidi_MidiBase;
 struct __pyx_obj_7_rtmidi_MidiIn;
 struct __pyx_obj_7_rtmidi_MidiOut;
 
-/* "_rtmidi.pyx":430
+/* "_rtmidi.pyx":435
  * 
  * 
  * cdef class MidiBase:             # <<<<<<<<<<<<<<
  *     cdef object _port
  *     cdef object _error_callback
  */
 struct __pyx_obj_7_rtmidi_MidiBase {
@@ -1005,71 +1009,71 @@
   struct __pyx_vtabstruct_7_rtmidi_MidiBase *__pyx_vtab;
   PyObject *_port;
   PyObject *_error_callback;
   PyObject *_deleted;
 };
 
 
-/* "_rtmidi.pyx":756
+/* "_rtmidi.pyx":761
  * 
  * 
  * cdef class MidiIn(MidiBase):             # <<<<<<<<<<<<<<
  *     """Midi input client interface.
  * 
  */
 struct __pyx_obj_7_rtmidi_MidiIn {
   struct __pyx_obj_7_rtmidi_MidiBase __pyx_base;
   RtMidiIn *thisptr;
   PyObject *_callback;
 };
 
 
-/* "_rtmidi.pyx":968
+/* "_rtmidi.pyx":973
  * 
  * 
  * cdef class MidiOut(MidiBase):             # <<<<<<<<<<<<<<
  *     """Midi output client interface.
  * 
  */
 struct __pyx_obj_7_rtmidi_MidiOut {
   struct __pyx_obj_7_rtmidi_MidiBase __pyx_base;
   RtMidiOut *thisptr;
 };
 
 
 
-/* "_rtmidi.pyx":430
+/* "_rtmidi.pyx":435
  * 
  * 
  * cdef class MidiBase:             # <<<<<<<<<<<<<<
  *     cdef object _port
  *     cdef object _error_callback
  */
 
 struct __pyx_vtabstruct_7_rtmidi_MidiBase {
   RtMidi *(*baseptr)(struct __pyx_obj_7_rtmidi_MidiBase *);
 };
 static struct __pyx_vtabstruct_7_rtmidi_MidiBase *__pyx_vtabptr_7_rtmidi_MidiBase;
 
 
-/* "_rtmidi.pyx":756
+/* "_rtmidi.pyx":761
  * 
  * 
  * cdef class MidiIn(MidiBase):             # <<<<<<<<<<<<<<
  *     """Midi input client interface.
  * 
  */
 
 struct __pyx_vtabstruct_7_rtmidi_MidiIn {
   struct __pyx_vtabstruct_7_rtmidi_MidiBase __pyx_base;
 };
 static struct __pyx_vtabstruct_7_rtmidi_MidiIn *__pyx_vtabptr_7_rtmidi_MidiIn;
 
 
-/* "_rtmidi.pyx":968
+/* "_rtmidi.pyx":973
  * 
  * 
  * cdef class MidiOut(MidiBase):             # <<<<<<<<<<<<<<
  *     """Midi output client interface.
  * 
  */
 
@@ -1853,14 +1857,15 @@
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_startswith[] = "startswith";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_RtMidiError[] = "RtMidiError";
 static const char __pyx_k_SystemError[] = "SystemError";
+static const char __pyx_k_API_WEB_MIDI[] = "API_WEB_MIDI";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_active_sense[] = "active_sense";
 static const char __pyx_k_get_api_name[] = "get_api_name";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_string_types[] = "string_types";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_API_UNIX_JACK[] = "API_UNIX_JACK";
@@ -1912,15 +1917,15 @@
 static const char __pyx_k_UnsupportedOperationError[] = "UnsupportedOperationError";
 static const char __pyx_k_message_must_not_be_empty[] = "'message' must not be empty.";
 static const char __pyx_k_r_already_opened_s_port_i[] = "%r already opened %s port %i.";
 static const char __pyx_k_ERRORTYPE_NO_DEVICES_FOUND[] = "ERRORTYPE_NO_DEVICES_FOUND";
 static const char __pyx_k_ERRORTYPE_INVALID_PARAMETER[] = "ERRORTYPE_INVALID_PARAMETER";
 static const char __pyx_k_error_looking_for_port_name[] = "error looking for port name!";
 static const char __pyx_k_home_runner_work_python_rtmidi[] = "/home/runner/work/python-rtmidi/python-rtmidi/src/_rtmidi.pyx";
-static const char __pyx_k_A_Python_binding_for_the_RtMidi[] = "A Python binding for the RtMidi C++ library implemented using Cython.\n\nOverview\n========\n\n**RtMidi** is a set of C++ classes which provides a concise and simple,\ncross-platform API (Application Programming Interface) for realtime MIDI\ninput / output across Linux (ALSA & JACK), macOS / OS X (CoreMIDI & JACK),\nand Windows (MultiMedia System) operating systems.\n\n**python-rtmidi** is a Python binding for RtMidi implemented using Cython_ and\nprovides a thin wrapper around the RtMidi C++ interface. The API is basically\nthe same as the C++ one but with the naming scheme of classes, methods and\nparameters adapted to the Python PEP-8 conventions and requirements of the\nPython package naming structure. **python-rtmidi** supports Python 3 (3.6, 3.7,\n3.8, and 3.9).\n\n\nUsage example\n=============\n\nHere's a short example of how to use **python-rtmidi** to open the first\navailable MIDI output port and send a middle C note on MIDI channel 1::\n\n    import time\n    import rtmidi\n\n    midiout = rtmidi.MidiOut()\n    available_ports = midiout.get_ports()\n\n    if available_ports:\n        midiout.open_port(0)\n    else:\n        midiout.open_virtual_port(\"My virtual output\")\n\n    with midiout:\n        note_on = [0x90, 60, 112] # channel 1, middle C, velocity 112\n        note_off = [0x80, 60, 0]\n        midiout.send_message(note_on)\n        time.sleep(0.5)\n        midiout.send_message(note_off)\n        time.sleep(0.1)\n\n    del midiout\n\n\nConstants\n=========\n\n\nLow-level APIs\n--------------\n\nThese constants are returned by the ``get_compiled_api`` function and the\n``MidiIn.get_current_api`` resp. ``MidiOut.get_current_api`` methods and are\nused to specify the low-level MIDI backend API to use when creating a\n``MidiIn`` or ``MidiOut`` instance.\n\n``API_UNSPECIFIED``\n    Use first compiled-in API, which has any input resp. output ports\n``API_MACOSX_CORE``\n    macOS (OS X) CoreMIDI\n``API_LINUX_ALSA``\n    Linux ALSA\n``API_UNIX_JACK``""\n    Jack Client\n``API_WINDOWS_MM``\n    Windows MultiMedia\n``API_RTMIDI_DUMMY``\n    RtMidi Dummy API (used when no suitable API was found)\n\n\nError types\n-----------\n\nThese constants are passed as the first argument to an error handler\nfunction registered with ``set_error_callback`` method of a ``MidiIn``\nor ``MidiOut`` instance. For the meaning of each value, please see\nthe `RtMidi API reference`_.\n\n* ``ERRORTYPE_DEBUG_WARNING``\n* ``ERRORTYPE_DRIVER_ERROR``\n* ``ERRORTYPE_INVALID_DEVICE``\n* ``ERRORTYPE_INVALID_PARAMETER``\n* ``ERRORTYPE_INVALID_USE``\n* ``ERRORTYPE_MEMORY_ERROR``\n* ``ERRORTYPE_NO_DEVICES_FOUND``\n* ``ERRORTYPE_SYSTEM_ERROR``\n* ``ERRORTYPE_THREAD_ERROR``\n* ``ERRORTYPE_UNSPECIFIED``\n* ``ERRORTYPE_WARNING``\n\n\n.. _cython: http://cython.org/\n.. _rtmidi api reference:\n    http://www.music.mcgill.ca/~gary/rtmidi/classRtMidiError.html\n\n";
+static const char __pyx_k_A_Python_binding_for_the_RtMidi[] = "A Python binding for the RtMidi C++ library implemented using Cython.\n\nOverview\n========\n\n**RtMidi** is a set of C++ classes which provides a concise and simple,\ncross-platform API (Application Programming Interface) for realtime MIDI\ninput / output across Linux (ALSA & JACK), macOS / OS X (CoreMIDI & JACK),\nand Windows (MultiMedia System) operating systems.\n\n**python-rtmidi** is a Python binding for RtMidi implemented using Cython_ and\nprovides a thin wrapper around the RtMidi C++ interface. The API is basically\nthe same as the C++ one but with the naming scheme of classes, methods and\nparameters adapted to the Python PEP-8 conventions and requirements of the\nPython package naming structure. **python-rtmidi** supports Python 3 (3.6, 3.7,\n3.8, and 3.9).\n\n\nUsage example\n=============\n\nHere's a short example of how to use **python-rtmidi** to open the first\navailable MIDI output port and send a middle C note on MIDI channel 1::\n\n    import time\n    import rtmidi\n\n    midiout = rtmidi.MidiOut()\n    available_ports = midiout.get_ports()\n\n    if available_ports:\n        midiout.open_port(0)\n    else:\n        midiout.open_virtual_port(\"My virtual output\")\n\n    with midiout:\n        note_on = [0x90, 60, 112] # channel 1, middle C, velocity 112\n        note_off = [0x80, 60, 0]\n        midiout.send_message(note_on)\n        time.sleep(0.5)\n        midiout.send_message(note_off)\n        time.sleep(0.1)\n\n    del midiout\n\n\nConstants\n=========\n\n\nLow-level APIs\n--------------\n\nThese constants are returned by the ``get_compiled_api`` function and the\n``MidiIn.get_current_api`` resp. ``MidiOut.get_current_api`` methods and are\nused to specify the low-level MIDI backend API to use when creating a\n``MidiIn`` or ``MidiOut`` instance.\n\n``API_UNSPECIFIED``\n    Use first compiled-in API, which has any input resp. output ports\n``API_MACOSX_CORE``\n    macOS (OS X) CoreMIDI\n``API_LINUX_ALSA``\n    Linux ALSA\n``API_UNIX_JACK``""\n    Jack Client\n``API_WINDOWS_MM``\n    Windows MultiMedia\n``API_RTMIDI_DUMMY``\n    RtMidi Dummy API (used when no suitable API was found)\n``API_RWEB_MIDI``\n    W3C Web MIDI API\n\n\n\nError types\n-----------\n\nThese constants are passed as the first argument to an error handler\nfunction registered with ``set_error_callback`` method of a ``MidiIn``\nor ``MidiOut`` instance. For the meaning of each value, please see\nthe `RtMidi API reference`_.\n\n* ``ERRORTYPE_DEBUG_WARNING``\n* ``ERRORTYPE_DRIVER_ERROR``\n* ``ERRORTYPE_INVALID_DEVICE``\n* ``ERRORTYPE_INVALID_PARAMETER``\n* ``ERRORTYPE_INVALID_USE``\n* ``ERRORTYPE_MEMORY_ERROR``\n* ``ERRORTYPE_NO_DEVICES_FOUND``\n* ``ERRORTYPE_SYSTEM_ERROR``\n* ``ERRORTYPE_THREAD_ERROR``\n* ``ERRORTYPE_UNSPECIFIED``\n* ``ERRORTYPE_WARNING``\n\n\n.. _cython: http://cython.org/\n.. _rtmidi api reference:\n    http://www.music.mcgill.ca/~gary/rtmidi/classRtMidiError.html\n\n";
 static const char __pyx_k_Virtual_ports_are_not_supported[] = "Virtual ports are not supported by the Windows MultiMedia API.";
 static const char __pyx_k_message_longer_than_3_bytes_but[] = "'message' longer than 3 bytes but does not start with 0xF0.";
 static const char __pyx_k_API_backend_does_not_support_cha[] = "API backend does not support changing the client name.";
 static const char __pyx_k_Base_general_RtMidi_exception_Al[] = "Base general RtMidi exception.\n\n    All other exceptions in this module derive form this exception.\n\n    Instances have a ``type`` attribute that maps to one of the\n    ``ERRORTYPE_*`` constants.\n\n    ";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x9171c0f, 0x2133db3, 0x021d8b9) = (_deleted, _error_callback, _port))";
 static const char __pyx_k_Raised_if_a_memory_allocation_fa[] = "Raised if a memory allocation failed on the C++ level.\n\n    Also derives from ``MemoryError``.\n\n    ";
 static const char __pyx_k_Raised_if_a_method_is_not_suppor[] = "Raised if a method is not supported by the low-level API.\n\n    Also derives from ``RuntimeError``.\n\n    ";
@@ -1939,14 +1944,16 @@
 static PyObject *__pyx_n_u_API_MACOSX_CORE;
 static PyObject *__pyx_n_s_API_RTMIDI_DUMMY;
 static PyObject *__pyx_n_u_API_RTMIDI_DUMMY;
 static PyObject *__pyx_n_s_API_UNIX_JACK;
 static PyObject *__pyx_n_u_API_UNIX_JACK;
 static PyObject *__pyx_n_s_API_UNSPECIFIED;
 static PyObject *__pyx_n_u_API_UNSPECIFIED;
+static PyObject *__pyx_n_s_API_WEB_MIDI;
+static PyObject *__pyx_n_u_API_WEB_MIDI;
 static PyObject *__pyx_n_s_API_WINDOWS_MM;
 static PyObject *__pyx_n_u_API_WINDOWS_MM;
 static PyObject *__pyx_kp_u_API_backend_does_not_support_cha;
 static PyObject *__pyx_kp_u_API_backend_does_not_support_cha_2;
 static PyObject *__pyx_kp_s_Base_general_RtMidi_exception_Al;
 static PyObject *__pyx_n_s_ERRORTYPE_DEBUG_WARNING;
 static PyObject *__pyx_n_u_ERRORTYPE_DEBUG_WARNING;
@@ -2200,15 +2207,15 @@
 static PyObject *__pyx_codeobj__24;
 static PyObject *__pyx_codeobj__26;
 static PyObject *__pyx_codeobj__27;
 static PyObject *__pyx_codeobj__29;
 static PyObject *__pyx_codeobj__31;
 /* Late includes */
 
-/* "_rtmidi.pyx":207
+/* "_rtmidi.pyx":211
  * # internal functions
  * 
  * cdef void _cb_func(double delta_time, vector[unsigned char] *msg_v,             # <<<<<<<<<<<<<<
  *                    void *cb_info) with gil:
  *     """Wrapper for a Python callback function for MIDI input."""
  */
 
@@ -2233,113 +2240,113 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_cb_func", 0);
 
-  /* "_rtmidi.pyx":210
+  /* "_rtmidi.pyx":214
  *                    void *cb_info) with gil:
  *     """Wrapper for a Python callback function for MIDI input."""
  *     func, data = (<object> cb_info)             # <<<<<<<<<<<<<<
  *     message = [msg_v.at(i) for i in range(msg_v.size())]
  *     func((message, delta_time), data)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_cb_info);
   __Pyx_INCREF(__pyx_t_1);
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 210, __pyx_L1_error)
+      __PYX_ERR(0, 214, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_5 = Py_TYPE(__pyx_t_4)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_4), 2) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_4), 2) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
     __pyx_t_5 = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 210, __pyx_L1_error)
+    __PYX_ERR(0, 214, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_func = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "_rtmidi.pyx":211
+  /* "_rtmidi.pyx":215
  *     """Wrapper for a Python callback function for MIDI input."""
  *     func, data = (<object> cb_info)
  *     message = [msg_v.at(i) for i in range(msg_v.size())]             # <<<<<<<<<<<<<<
  *     func((message, delta_time), data)
  * 
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = __pyx_v_msg_v->size();
     __pyx_t_7 = __pyx_t_6;
     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_7genexpr__pyx_v_i = __pyx_t_8;
       try {
         __pyx_t_9 = __pyx_v_msg_v->at(__pyx_7genexpr__pyx_v_i);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 211, __pyx_L1_error)
+        __PYX_ERR(0, 215, __pyx_L1_error)
       }
-      __pyx_t_3 = __Pyx_PyInt_From_unsigned_char(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 211, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_unsigned_char(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 211, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 215, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
   } /* exit inner scope */
   __pyx_v_message = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":212
+  /* "_rtmidi.pyx":216
  *     func, data = (<object> cb_info)
  *     message = [msg_v.at(i) for i in range(msg_v.size())]
  *     func((message, delta_time), data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_message);
   __Pyx_GIVEREF(__pyx_v_message);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_message);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_3 = 0;
@@ -2355,49 +2362,49 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_10 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, __pyx_t_2);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_10, __pyx_v_data);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":207
+  /* "_rtmidi.pyx":211
  * # internal functions
  * 
  * cdef void _cb_func(double delta_time, vector[unsigned char] *msg_v,             # <<<<<<<<<<<<<<
  *                    void *cb_info) with gil:
  *     """Wrapper for a Python callback function for MIDI input."""
  */
 
@@ -2416,15 +2423,15 @@
   __Pyx_XDECREF(__pyx_v_message);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "_rtmidi.pyx":215
+/* "_rtmidi.pyx":219
  * 
  * 
  * cdef void _cb_error_func(ErrorType errorType, const string &errorText,             # <<<<<<<<<<<<<<
  *                          void *cb_info) except * with gil:
  *     """Wrapper for a Python callback function for errors."""
  */
 
@@ -2445,30 +2452,30 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_cb_error_func", 0);
 
-  /* "_rtmidi.pyx":218
+  /* "_rtmidi.pyx":222
  *                          void *cb_info) except * with gil:
  *     """Wrapper for a Python callback function for errors."""
  *     func, data, decoder = (<object> cb_info)             # <<<<<<<<<<<<<<
  *     func(errorType, decoder(errorText), data)
  * 
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_cb_info);
   __Pyx_INCREF(__pyx_t_1);
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 218, __pyx_L1_error)
+      __PYX_ERR(0, 222, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -2476,62 +2483,62 @@
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 222, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 2; __pyx_t_4 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
     __pyx_t_6 = NULL;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 218, __pyx_L1_error)
+    __PYX_ERR(0, 222, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_func = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_data = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_decoder = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "_rtmidi.pyx":219
+  /* "_rtmidi.pyx":223
  *     """Wrapper for a Python callback function for errors."""
  *     func, data, decoder = (<object> cb_info)
  *     func(errorType, decoder(errorText), data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(__pyx_v_errorType); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(__pyx_v_errorType); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_errorText); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_errorText); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_decoder);
   __pyx_t_5 = __pyx_v_decoder; __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -2539,15 +2546,15 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_INCREF(__pyx_v_func);
   __pyx_t_5 = __pyx_v_func; __pyx_t_2 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
@@ -2558,54 +2565,54 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_4, __pyx_t_3, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_4, __pyx_t_3, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_t_3);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_8, __pyx_v_data);
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":215
+  /* "_rtmidi.pyx":219
  * 
  * 
  * cdef void _cb_error_func(ErrorType errorType, const string &errorText,             # <<<<<<<<<<<<<<
  *                          void *cb_info) except * with gil:
  *     """Wrapper for a Python callback function for errors."""
  */
 
@@ -2625,15 +2632,15 @@
   __Pyx_XDECREF(__pyx_v_decoder);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "_rtmidi.pyx":222
+/* "_rtmidi.pyx":226
  * 
  * 
  * def _to_bytes(name):             # <<<<<<<<<<<<<<
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  */
 
@@ -2669,29 +2676,29 @@
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_to_bytes", 0);
   __Pyx_INCREF(__pyx_v_name);
 
-  /* "_rtmidi.pyx":225
+  /* "_rtmidi.pyx":229
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):             # <<<<<<<<<<<<<<
  *         try:
  *             name = bytes(name, 'utf-8')  # Python 3
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_string_types); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_string_types); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_name, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_name, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "_rtmidi.pyx":226
+    /* "_rtmidi.pyx":230
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):
  *         try:             # <<<<<<<<<<<<<<
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:
  */
     {
@@ -2699,36 +2706,36 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_4, &__pyx_t_5, &__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       /*try:*/ {
 
-        /* "_rtmidi.pyx":227
+        /* "_rtmidi.pyx":231
  *     if isinstance(name, string_types):
  *         try:
  *             name = bytes(name, 'utf-8')  # Python 3             # <<<<<<<<<<<<<<
  *         except TypeError:
  *             name = name.encode('utf-8')  # Python 2
  */
-        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L4_error)
+        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_INCREF(__pyx_v_name);
         __Pyx_GIVEREF(__pyx_v_name);
         PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_name);
         __Pyx_INCREF(__pyx_kp_u_utf_8);
         __Pyx_GIVEREF(__pyx_kp_u_utf_8);
         PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u_utf_8);
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_t_1, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 227, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_t_1, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 231, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF_SET(__pyx_v_name, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "_rtmidi.pyx":226
+        /* "_rtmidi.pyx":230
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):
  *         try:             # <<<<<<<<<<<<<<
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:
  */
       }
@@ -2736,64 +2743,64 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "_rtmidi.pyx":228
+      /* "_rtmidi.pyx":232
  *         try:
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:             # <<<<<<<<<<<<<<
  *             name = name.encode('utf-8')  # Python 2
  * 
  */
       __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_8) {
         __Pyx_AddTraceback("_rtmidi._to_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_1, &__pyx_t_9) < 0) __PYX_ERR(0, 228, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_1, &__pyx_t_9) < 0) __PYX_ERR(0, 232, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GOTREF(__pyx_t_9);
 
-        /* "_rtmidi.pyx":229
+        /* "_rtmidi.pyx":233
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:
  *             name = name.encode('utf-8')  # Python 2             # <<<<<<<<<<<<<<
  * 
  *     if not isinstance(name, bytes):
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 229, __pyx_L6_except_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 233, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
             __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
         __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_12, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_kp_u_utf_8);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 229, __pyx_L6_except_error)
+        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 233, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF_SET(__pyx_v_name, __pyx_t_10);
         __pyx_t_10 = 0;
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L5_exception_handled;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "_rtmidi.pyx":226
+      /* "_rtmidi.pyx":230
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):
  *         try:             # <<<<<<<<<<<<<<
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:
  */
       __Pyx_XGIVEREF(__pyx_t_4);
@@ -2805,69 +2812,69 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_XGIVEREF(__pyx_t_6);
       __Pyx_ExceptionReset(__pyx_t_4, __pyx_t_5, __pyx_t_6);
       __pyx_L9_try_end:;
     }
 
-    /* "_rtmidi.pyx":225
+    /* "_rtmidi.pyx":229
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):             # <<<<<<<<<<<<<<
  *         try:
  *             name = bytes(name, 'utf-8')  # Python 3
  */
   }
 
-  /* "_rtmidi.pyx":231
+  /* "_rtmidi.pyx":235
  *             name = name.encode('utf-8')  # Python 2
  * 
  *     if not isinstance(name, bytes):             # <<<<<<<<<<<<<<
  *         raise TypeError("name must be bytes or (unicode) string.")
  * 
  */
   __pyx_t_3 = PyBytes_Check(__pyx_v_name); 
   __pyx_t_2 = ((!(__pyx_t_3 != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "_rtmidi.pyx":232
+    /* "_rtmidi.pyx":236
  * 
  *     if not isinstance(name, bytes):
  *         raise TypeError("name must be bytes or (unicode) string.")             # <<<<<<<<<<<<<<
  * 
  *     return name
  */
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 236, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_Raise(__pyx_t_9, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __PYX_ERR(0, 232, __pyx_L1_error)
+    __PYX_ERR(0, 236, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":231
+    /* "_rtmidi.pyx":235
  *             name = name.encode('utf-8')  # Python 2
  * 
  *     if not isinstance(name, bytes):             # <<<<<<<<<<<<<<
  *         raise TypeError("name must be bytes or (unicode) string.")
  * 
  */
   }
 
-  /* "_rtmidi.pyx":234
+  /* "_rtmidi.pyx":238
  *         raise TypeError("name must be bytes or (unicode) string.")
  * 
  *     return name             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_name);
   __pyx_r = __pyx_v_name;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":222
+  /* "_rtmidi.pyx":226
  * 
  * 
  * def _to_bytes(name):             # <<<<<<<<<<<<<<
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  */
 
@@ -2884,15 +2891,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":276
+/* "_rtmidi.pyx":281
  *     type = ERR_UNSPECIFIED
  * 
  *     def __init__(self, msg, type=None):             # <<<<<<<<<<<<<<
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type
  */
 
@@ -2932,25 +2939,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_msg)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 276, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 281, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_type);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 276, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 281, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -2960,15 +2967,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_msg = values[1];
     __pyx_v_type = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 276, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 281, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.RtMidiError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_11RtMidiError___init__(__pyx_self, __pyx_v_self, __pyx_v_msg, __pyx_v_type);
 
@@ -2985,76 +2992,76 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "_rtmidi.pyx":277
+  /* "_rtmidi.pyx":282
  * 
  *     def __init__(self, msg, type=None):
  *         super().__init__(msg)             # <<<<<<<<<<<<<<
  *         self.type = self.type if type is None else type
  * 
  */
   __pyx_t_2 = __Pyx_CyFunction_GetClassObj(__pyx_self);
-  if (!__pyx_t_2) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 277, __pyx_L1_error) }
+  if (!__pyx_t_2) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 282, __pyx_L1_error) }
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_INCREF(__pyx_v_self);
   __Pyx_GIVEREF(__pyx_v_self);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_self);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_msg);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":278
+  /* "_rtmidi.pyx":283
  *     def __init__(self, msg, type=None):
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_4 = (__pyx_v_type == Py_None);
   if ((__pyx_t_4 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 278, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 283, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_type);
     __pyx_t_1 = __pyx_v_type;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 278, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":276
+  /* "_rtmidi.pyx":281
  *     type = ERR_UNSPECIFIED
  * 
  *     def __init__(self, msg, type=None):             # <<<<<<<<<<<<<<
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type
  */
 
@@ -3069,15 +3076,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":337
+/* "_rtmidi.pyx":342
  * # wrappers for RtMidi's static methods and classes
  * 
  * def get_api_display_name(api):             # <<<<<<<<<<<<<<
  *     """Return the display name of a specified MIDI API.
  * 
  */
 
@@ -3102,30 +3109,30 @@
   enum RtMidi::Api __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_api_display_name", 0);
 
-  /* "_rtmidi.pyx":350
+  /* "_rtmidi.pyx":355
  * 
  *     """
  *     return RtMidi_getApiDisplayName(api).decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(__pyx_v_api)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 350, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_decode_cpp_string(RtMidi::getApiDisplayName(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_1 = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(__pyx_v_api)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 355, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(RtMidi::getApiDisplayName(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":337
+  /* "_rtmidi.pyx":342
  * # wrappers for RtMidi's static methods and classes
  * 
  * def get_api_display_name(api):             # <<<<<<<<<<<<<<
  *     """Return the display name of a specified MIDI API.
  * 
  */
 
@@ -3136,15 +3143,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":353
+/* "_rtmidi.pyx":358
  * 
  * 
  * def get_api_name(api):             # <<<<<<<<<<<<<<
  *     """Return the name of a specified MIDI API.
  * 
  */
 
@@ -3169,30 +3176,30 @@
   enum RtMidi::Api __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_api_name", 0);
 
-  /* "_rtmidi.pyx":366
+  /* "_rtmidi.pyx":371
  * 
  *     """
  *     return RtMidi_getApiName(api).decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(__pyx_v_api)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_decode_cpp_string(RtMidi::getApiName(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_1 = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(__pyx_v_api)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(RtMidi::getApiName(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":353
+  /* "_rtmidi.pyx":358
  * 
  * 
  * def get_api_name(api):             # <<<<<<<<<<<<<<
  *     """Return the name of a specified MIDI API.
  * 
  */
 
@@ -3203,15 +3210,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":369
+/* "_rtmidi.pyx":374
  * 
  * 
  * def get_compiled_api():             # <<<<<<<<<<<<<<
  *     """Return a list of low-level MIDI backend APIs this module supports.
  * 
  */
 
@@ -3241,49 +3248,49 @@
   std::vector<enum RtMidi::Api> ::size_type __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_compiled_api", 0);
 
-  /* "_rtmidi.pyx":381
+  /* "_rtmidi.pyx":386
  *     cdef vector[Api] api_v
  * 
  *     RtMidi_getCompiledApi(api_v)             # <<<<<<<<<<<<<<
  *     return [api_v[i] for i in range(api_v.size())]
  * 
  */
   RtMidi::getCompiledApi(__pyx_v_api_v);
 
-  /* "_rtmidi.pyx":382
+  /* "_rtmidi.pyx":387
  * 
  *     RtMidi_getCompiledApi(api_v)
  *     return [api_v[i] for i in range(api_v.size())]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_v_api_v.size();
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_8genexpr1__pyx_v_i = __pyx_t_4;
-      __pyx_t_5 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api((__pyx_v_api_v[__pyx_8genexpr1__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api((__pyx_v_api_v[__pyx_8genexpr1__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 382, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 387, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":369
+  /* "_rtmidi.pyx":374
  * 
  * 
  * def get_compiled_api():             # <<<<<<<<<<<<<<
  *     """Return a list of low-level MIDI backend APIs this module supports.
  * 
  */
 
@@ -3295,15 +3302,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":385
+/* "_rtmidi.pyx":390
  * 
  * 
  * def get_compiled_api_by_name(name):             # <<<<<<<<<<<<<<
  *     """Return the compiled MIDI API having the given name.
  * 
  */
 
@@ -3330,48 +3337,48 @@
   PyObject *__pyx_t_3 = NULL;
   std::string __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_compiled_api_by_name", 0);
 
-  /* "_rtmidi.pyx":393
+  /* "_rtmidi.pyx":398
  * 
  *     """
  *     return RtMidi_getCompiledApiByName(_to_bytes(name))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::getCompiledApiByName(__pyx_t_4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::getCompiledApiByName(__pyx_t_4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":385
+  /* "_rtmidi.pyx":390
  * 
  * 
  * def get_compiled_api_by_name(name):             # <<<<<<<<<<<<<<
  *     """Return the compiled MIDI API having the given name.
  * 
  */
 
@@ -3384,15 +3391,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":396
+/* "_rtmidi.pyx":401
  * 
  * 
  * def get_rtmidi_version():             # <<<<<<<<<<<<<<
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')
  */
 
@@ -3416,29 +3423,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_rtmidi_version", 0);
 
-  /* "_rtmidi.pyx":398
+  /* "_rtmidi.pyx":403
  * def get_rtmidi_version():
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_cpp_string(RtMidi::getVersion(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(RtMidi::getVersion(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":396
+  /* "_rtmidi.pyx":401
  * 
  * 
  * def get_rtmidi_version():             # <<<<<<<<<<<<<<
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')
  */
 
@@ -3449,15 +3456,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":401
+/* "_rtmidi.pyx":406
  * 
  * 
  * def _default_error_handler(etype, msg, data=None):             # <<<<<<<<<<<<<<
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  */
 
@@ -3497,25 +3504,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_etype)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_msg)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_default_error_handler", 0, 2, 3, 1); __PYX_ERR(0, 401, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_default_error_handler", 0, 2, 3, 1); __PYX_ERR(0, 406, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_default_error_handler") < 0)) __PYX_ERR(0, 401, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_default_error_handler") < 0)) __PYX_ERR(0, 406, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -3525,15 +3532,15 @@
     }
     __pyx_v_etype = values[0];
     __pyx_v_msg = values[1];
     __pyx_v_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_default_error_handler", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 401, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_default_error_handler", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 406, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi._default_error_handler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_12_default_error_handler(__pyx_self, __pyx_v_etype, __pyx_v_msg, __pyx_v_data);
 
@@ -3553,758 +3560,758 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_default_error_handler", 0);
 
-  /* "_rtmidi.pyx":402
+  /* "_rtmidi.pyx":407
  * 
  * def _default_error_handler(etype, msg, data=None):
  *     if etype == ERR_MEMORY_ERROR:             # <<<<<<<<<<<<<<
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_etype, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_etype, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "_rtmidi.pyx":403
+    /* "_rtmidi.pyx":408
  * def _default_error_handler(etype, msg, data=None):
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)             # <<<<<<<<<<<<<<
  *     elif etype == ERR_INVALID_PARAMETER:
  *         raise InvalidPortError(msg)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MemoryAllocationError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MemoryAllocationError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_msg);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 403, __pyx_L1_error)
+    __PYX_ERR(0, 408, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":402
+    /* "_rtmidi.pyx":407
  * 
  * def _default_error_handler(etype, msg, data=None):
  *     if etype == ERR_MEMORY_ERROR:             # <<<<<<<<<<<<<<
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:
  */
   }
 
-  /* "_rtmidi.pyx":404
+  /* "_rtmidi.pyx":409
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:             # <<<<<<<<<<<<<<
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_etype, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_etype, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 409, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "_rtmidi.pyx":405
+    /* "_rtmidi.pyx":410
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:
  *         raise InvalidPortError(msg)             # <<<<<<<<<<<<<<
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  *         raise SystemError(msg, type=etype)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 405, __pyx_L1_error)
+    __PYX_ERR(0, 410, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":404
+    /* "_rtmidi.pyx":409
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:             # <<<<<<<<<<<<<<
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  */
   }
 
-  /* "_rtmidi.pyx":406
+  /* "_rtmidi.pyx":411
  *     elif etype == ERR_INVALID_PARAMETER:
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):             # <<<<<<<<<<<<<<
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  */
   __Pyx_INCREF(__pyx_v_etype);
   __pyx_t_1 = __pyx_v_etype;
-  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_3 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::SYSTEM_ERROR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::SYSTEM_ERROR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_3 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::THREAD_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::THREAD_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 411, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = (__pyx_t_3 != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "_rtmidi.pyx":407
+    /* "_rtmidi.pyx":412
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  *         raise SystemError(msg, type=etype)             # <<<<<<<<<<<<<<
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_msg);
     __Pyx_GIVEREF(__pyx_v_msg);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_msg);
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_type, __pyx_v_etype) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 407, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_type, __pyx_v_etype) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 407, __pyx_L1_error)
+    __PYX_ERR(0, 412, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":406
+    /* "_rtmidi.pyx":411
  *     elif etype == ERR_INVALID_PARAMETER:
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):             # <<<<<<<<<<<<<<
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  */
   }
 
-  /* "_rtmidi.pyx":408
+  /* "_rtmidi.pyx":413
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):             # <<<<<<<<<<<<<<
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)
  */
   __Pyx_INCREF(__pyx_v_etype);
   __pyx_t_6 = __pyx_v_etype;
-  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::WARNING); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::WARNING); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_6, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_6, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!__pyx_t_3) {
   } else {
     __pyx_t_5 = __pyx_t_3;
     goto __pyx_L7_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DEBUG_WARNING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DEBUG_WARNING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 408, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 413, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_5 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_3 = (__pyx_t_5 != 0);
   if (__pyx_t_3) {
 
-    /* "_rtmidi.pyx":409
+    /* "_rtmidi.pyx":414
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):
  */
-    __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_portNumber, __pyx_v_msg, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_portNumber, __pyx_v_msg, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 414, __pyx_L1_error)
     __pyx_t_7 = (__pyx_t_5 != 0);
     if (__pyx_t_7) {
     } else {
       __pyx_t_3 = __pyx_t_7;
       goto __pyx_L10_bool_binop_done;
     }
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_is_invalid) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_is_invalid);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 409, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_3 = __pyx_t_7;
     __pyx_L10_bool_binop_done:;
     if (unlikely(__pyx_t_3)) {
 
-      /* "_rtmidi.pyx":410
+      /* "_rtmidi.pyx":415
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('no ports available!'):
  *             raise InvalidPortError(msg)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 415, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 410, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 410, __pyx_L1_error)
+      __PYX_ERR(0, 415, __pyx_L1_error)
 
-      /* "_rtmidi.pyx":409
+      /* "_rtmidi.pyx":414
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):
  */
     }
 
-    /* "_rtmidi.pyx":411
+    /* "_rtmidi.pyx":416
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_no_ports_available) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_no_ports_available);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 411, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "_rtmidi.pyx":412
+      /* "_rtmidi.pyx":417
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):
  *             raise InvalidPortError(msg)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('error looking for port name!'):
  *             raise InvalidPortError(msg)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 417, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 412, __pyx_L1_error)
+      __PYX_ERR(0, 417, __pyx_L1_error)
 
-      /* "_rtmidi.pyx":411
+      /* "_rtmidi.pyx":416
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):
  */
     }
 
-    /* "_rtmidi.pyx":413
+    /* "_rtmidi.pyx":418
  *         elif msg.endswith('no ports available!'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_error_looking_for_port_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_error_looking_for_port_name);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "_rtmidi.pyx":414
+      /* "_rtmidi.pyx":419
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):
  *             raise InvalidPortError(msg)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('event parsing error!'):
  *             raise ValueError(msg)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 419, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 414, __pyx_L1_error)
+      __PYX_ERR(0, 419, __pyx_L1_error)
 
-      /* "_rtmidi.pyx":413
+      /* "_rtmidi.pyx":418
  *         elif msg.endswith('no ports available!'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):
  */
     }
 
-    /* "_rtmidi.pyx":415
+    /* "_rtmidi.pyx":420
  *         elif msg.endswith('error looking for port name!'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):             # <<<<<<<<<<<<<<
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_event_parsing_error) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_event_parsing_error);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 420, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "_rtmidi.pyx":416
+      /* "_rtmidi.pyx":421
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):
  *             raise ValueError(msg)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('error sending MIDI message to port.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  */
-      __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_v_msg); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_v_msg); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 416, __pyx_L1_error)
+      __PYX_ERR(0, 421, __pyx_L1_error)
 
-      /* "_rtmidi.pyx":415
+      /* "_rtmidi.pyx":420
  *         elif msg.endswith('error looking for port name!'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):             # <<<<<<<<<<<<<<
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):
  */
     }
 
-    /* "_rtmidi.pyx":417
+    /* "_rtmidi.pyx":422
  *         elif msg.endswith('event parsing error!'):
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_error_sending_MIDI_message_to_po) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_error_sending_MIDI_message_to_po);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 417, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 417, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 422, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "_rtmidi.pyx":418
+      /* "_rtmidi.pyx":423
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_v_msg);
       __Pyx_GIVEREF(__pyx_v_msg);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_msg);
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 418, __pyx_L1_error)
+      __PYX_ERR(0, 423, __pyx_L1_error)
 
-      /* "_rtmidi.pyx":417
+      /* "_rtmidi.pyx":422
  *         elif msg.endswith('event parsing error!'):
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  */
     }
 
-    /* "_rtmidi.pyx":419
+    /* "_rtmidi.pyx":424
  *         elif msg.endswith('error sending MIDI message to port.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_kp_u_error_sending_MIDI_to_virtual_de) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_error_sending_MIDI_to_virtual_de);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 424, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 419, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 424, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "_rtmidi.pyx":420
+      /* "_rtmidi.pyx":425
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('JACK server not running?'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_v_msg);
       __Pyx_GIVEREF(__pyx_v_msg);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_msg);
-      __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 425, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 425, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_type, __pyx_t_6) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_type, __pyx_t_6) < 0) __PYX_ERR(0, 425, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 425, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 420, __pyx_L1_error)
+      __PYX_ERR(0, 425, __pyx_L1_error)
 
-      /* "_rtmidi.pyx":419
+      /* "_rtmidi.pyx":424
  *         elif msg.endswith('error sending MIDI message to port.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):
  */
     }
 
-    /* "_rtmidi.pyx":421
+    /* "_rtmidi.pyx":426
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         else:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 426, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_JACK_server_not_running) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_JACK_server_not_running);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 426, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 421, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 426, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "_rtmidi.pyx":422
+      /* "_rtmidi.pyx":427
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  *         else:
  *             warnings.warn(msg)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 422, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_v_msg);
       __Pyx_GIVEREF(__pyx_v_msg);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_msg);
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 422, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 422, __pyx_L1_error)
+      __PYX_ERR(0, 427, __pyx_L1_error)
 
-      /* "_rtmidi.pyx":421
+      /* "_rtmidi.pyx":426
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         else:
  */
     }
 
-    /* "_rtmidi.pyx":424
+    /* "_rtmidi.pyx":429
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         else:
  *             warnings.warn(msg)             # <<<<<<<<<<<<<<
  *             return
  * 
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_warnings); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_warnings); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 429, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warn); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 424, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warn); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 429, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 424, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "_rtmidi.pyx":425
+      /* "_rtmidi.pyx":430
  *         else:
  *             warnings.warn(msg)
  *             return             # <<<<<<<<<<<<<<
  * 
  *     raise RtMidiError(msg, type=etype)
  */
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L0;
     }
 
-    /* "_rtmidi.pyx":408
+    /* "_rtmidi.pyx":413
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):             # <<<<<<<<<<<<<<
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)
  */
   }
 
-  /* "_rtmidi.pyx":427
+  /* "_rtmidi.pyx":432
  *             return
  * 
  *     raise RtMidiError(msg, type=etype)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_msg);
   __Pyx_GIVEREF(__pyx_v_msg);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_msg);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_v_etype) < 0) __PYX_ERR(0, 427, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_v_etype) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_Raise(__pyx_t_6, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __PYX_ERR(0, 427, __pyx_L1_error)
+  __PYX_ERR(0, 432, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":401
+  /* "_rtmidi.pyx":406
  * 
  * 
  * def _default_error_handler(etype, msg, data=None):             # <<<<<<<<<<<<<<
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  */
 
@@ -4318,52 +4325,52 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":435
+/* "_rtmidi.pyx":440
  *     cdef object _deleted
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return NULL
  * 
  */
 
 static RtMidi *__pyx_f_7_rtmidi_8MidiBase_baseptr(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   RtMidi *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("baseptr", 0);
 
-  /* "_rtmidi.pyx":436
+  /* "_rtmidi.pyx":441
  * 
  *     cdef RtMidi* baseptr(self):
  *         return NULL             # <<<<<<<<<<<<<<
  * 
  *     # context management
  */
   __pyx_r = NULL;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":435
+  /* "_rtmidi.pyx":440
  *     cdef object _deleted
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return NULL
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":439
+/* "_rtmidi.pyx":444
  * 
  *     # context management
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         """Support context manager protocol.
  * 
  */
 
@@ -4382,42 +4389,42 @@
 }
 
 static PyObject *__pyx_pf_7_rtmidi_8MidiBase___enter__(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "_rtmidi.pyx":465
+  /* "_rtmidi.pyx":470
  * 
  *         """
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, *exc_info):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":439
+  /* "_rtmidi.pyx":444
  * 
  *     # context management
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         """Support context manager protocol.
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":467
+/* "_rtmidi.pyx":472
  *         return self
  * 
  *     def __exit__(self, *exc_info):             # <<<<<<<<<<<<<<
  *         """Support context manager protocol.
  * 
  */
 
@@ -4447,41 +4454,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "_rtmidi.pyx":474
+  /* "_rtmidi.pyx":479
  * 
  *         """
  *         self.close_port()             # <<<<<<<<<<<<<<
  * 
  *     def _check_port(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":467
+  /* "_rtmidi.pyx":472
  *         return self
  * 
  *     def __exit__(self, *exc_info):             # <<<<<<<<<<<<<<
  *         """Support context manager protocol.
  * 
  */
 
@@ -4496,15 +4503,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":476
+/* "_rtmidi.pyx":481
  *         self.close_port()
  * 
  *     def _check_port(self):             # <<<<<<<<<<<<<<
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:
  */
 
@@ -4535,15 +4542,15 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_check_port", 0);
 
-  /* "_rtmidi.pyx":477
+  /* "_rtmidi.pyx":482
  * 
  *     def _check_port(self):
  *         inout = "input" if isinstance(self, MidiIn) else "output"             # <<<<<<<<<<<<<<
  *         if self._port == -1:
  *             raise InvalidUseError("%r already opened virtual %s port." %
  */
   __pyx_t_2 = __Pyx_TypeCheck(((PyObject *)__pyx_v_self), __pyx_ptype_7_rtmidi_MidiIn); 
@@ -4553,79 +4560,79 @@
   } else {
     __Pyx_INCREF(__pyx_n_u_output);
     __pyx_t_1 = __pyx_n_u_output;
   }
   __pyx_v_inout = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":478
+  /* "_rtmidi.pyx":483
  *     def _check_port(self):
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))
  */
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_self->_port, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_self->_port, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 478, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 483, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "_rtmidi.pyx":479
+    /* "_rtmidi.pyx":484
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:
  *             raise InvalidUseError("%r already opened virtual %s port." %             # <<<<<<<<<<<<<<
  *                                   (self, inout))
  *         elif self._port is not None:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 479, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 479, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
 
-    /* "_rtmidi.pyx":480
+    /* "_rtmidi.pyx":485
  *         if self._port == -1:
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))             # <<<<<<<<<<<<<<
  *         elif self._port is not None:
  *             raise InvalidUseError("%r already opened %s port %i." %
  */
-    __pyx_t_7 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(((PyObject *)__pyx_v_self)), __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(((PyObject *)__pyx_v_self)), __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 485, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_already_opened_virtual);
     __pyx_t_5 += 24;
     __Pyx_GIVEREF(__pyx_kp_u_already_opened_virtual);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_kp_u_already_opened_virtual);
-    __pyx_t_7 = __Pyx_PyUnicode_Unicode(__pyx_v_inout); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Unicode(__pyx_v_inout); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 485, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_port);
     __pyx_t_5 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_port);
     PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_kp_u_port);
 
-    /* "_rtmidi.pyx":479
+    /* "_rtmidi.pyx":484
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:
  *             raise InvalidUseError("%r already opened virtual %s port." %             # <<<<<<<<<<<<<<
  *                                   (self, inout))
  *         elif self._port is not None:
  */
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 479, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4633,78 +4640,78 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 479, __pyx_L1_error)
+    __PYX_ERR(0, 484, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":478
+    /* "_rtmidi.pyx":483
  *     def _check_port(self):
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))
  */
   }
 
-  /* "_rtmidi.pyx":481
+  /* "_rtmidi.pyx":486
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))
  *         elif self._port is not None:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("%r already opened %s port %i." %
  *                                   (self, inout, self._port))
  */
   __pyx_t_2 = (__pyx_v_self->_port != Py_None);
   __pyx_t_8 = (__pyx_t_2 != 0);
   if (unlikely(__pyx_t_8)) {
 
-    /* "_rtmidi.pyx":482
+    /* "_rtmidi.pyx":487
  *                                   (self, inout))
  *         elif self._port is not None:
  *             raise InvalidUseError("%r already opened %s port %i." %             # <<<<<<<<<<<<<<
  *                                   (self, inout, self._port))
  *         return inout
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 482, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "_rtmidi.pyx":483
+    /* "_rtmidi.pyx":488
  *         elif self._port is not None:
  *             raise InvalidUseError("%r already opened %s port %i." %
  *                                   (self, inout, self._port))             # <<<<<<<<<<<<<<
  *         return inout
  * 
  */
-    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 483, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 488, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
     PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)__pyx_v_self));
     __Pyx_INCREF(__pyx_v_inout);
     __Pyx_GIVEREF(__pyx_v_inout);
     PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_v_inout);
     __Pyx_INCREF(__pyx_v_self->_port);
     __Pyx_GIVEREF(__pyx_v_self->_port);
     PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_v_self->_port);
 
-    /* "_rtmidi.pyx":482
+    /* "_rtmidi.pyx":487
  *                                   (self, inout))
  *         elif self._port is not None:
  *             raise InvalidUseError("%r already opened %s port %i." %             # <<<<<<<<<<<<<<
  *                                   (self, inout, self._port))
  *         return inout
  */
-    __pyx_t_4 = PyUnicode_Format(__pyx_kp_u_r_already_opened_s_port_i, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 482, __pyx_L1_error)
+    __pyx_t_4 = PyUnicode_Format(__pyx_kp_u_r_already_opened_s_port_i, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4712,43 +4719,43 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_7, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 482, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 482, __pyx_L1_error)
+    __PYX_ERR(0, 487, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":481
+    /* "_rtmidi.pyx":486
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))
  *         elif self._port is not None:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("%r already opened %s port %i." %
  *                                   (self, inout, self._port))
  */
   }
 
-  /* "_rtmidi.pyx":484
+  /* "_rtmidi.pyx":489
  *             raise InvalidUseError("%r already opened %s port %i." %
  *                                   (self, inout, self._port))
  *         return inout             # <<<<<<<<<<<<<<
  * 
  *     def _decode_string(self, s, encoding='auto'):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_inout);
   __pyx_r = __pyx_v_inout;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":476
+  /* "_rtmidi.pyx":481
  *         self.close_port()
  * 
  *     def _check_port(self):             # <<<<<<<<<<<<<<
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:
  */
 
@@ -4763,15 +4770,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_inout);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":486
+/* "_rtmidi.pyx":491
  *         return inout
  * 
  *     def _decode_string(self, s, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':
  */
 
@@ -4811,15 +4818,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_decode_string") < 0)) __PYX_ERR(0, 486, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_decode_string") < 0)) __PYX_ERR(0, 491, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -4827,15 +4834,15 @@
       }
     }
     __pyx_v_s = values[0];
     __pyx_v_encoding = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_decode_string", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 486, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_decode_string", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 491, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiBase._decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_6_decode_string(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_s, __pyx_v_encoding);
 
@@ -4856,192 +4863,192 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_string", 0);
   __Pyx_INCREF(__pyx_v_encoding);
 
-  /* "_rtmidi.pyx":488
+  /* "_rtmidi.pyx":493
  *     def _decode_string(self, s, encoding='auto'):
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':             # <<<<<<<<<<<<<<
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_encoding, __pyx_n_u_auto, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 488, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_encoding, __pyx_n_u_auto, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 493, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "_rtmidi.pyx":489
+    /* "_rtmidi.pyx":494
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':
  *             if sys.platform.startswith('win'):             # <<<<<<<<<<<<<<
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_sys); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_sys); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_platform); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_platform); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_u_win) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_win);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 489, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 489, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_1) {
 
-      /* "_rtmidi.pyx":490
+      /* "_rtmidi.pyx":495
  *         if encoding == 'auto':
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'             # <<<<<<<<<<<<<<
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  *                   sys.platform == 'darwin'):
  */
       __Pyx_INCREF(__pyx_n_u_latin1);
       __Pyx_DECREF_SET(__pyx_v_encoding, __pyx_n_u_latin1);
 
-      /* "_rtmidi.pyx":489
+      /* "_rtmidi.pyx":494
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':
  *             if sys.platform.startswith('win'):             # <<<<<<<<<<<<<<
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  */
       goto __pyx_L4;
     }
 
-    /* "_rtmidi.pyx":491
+    /* "_rtmidi.pyx":496
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and             # <<<<<<<<<<<<<<
  *                   sys.platform == 'darwin'):
  *                 encoding = 'macroman'
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 491, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 496, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_5) {
     } else {
       __pyx_t_1 = __pyx_t_5;
       goto __pyx_L5_bool_binop_done;
     }
 
-    /* "_rtmidi.pyx":492
+    /* "_rtmidi.pyx":497
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  *                   sys.platform == 'darwin'):             # <<<<<<<<<<<<<<
  *                 encoding = 'macroman'
  *             else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_sys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_sys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 497, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_platform); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_platform); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_darwin, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_darwin, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 497, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_1 = __pyx_t_5;
     __pyx_L5_bool_binop_done:;
 
-    /* "_rtmidi.pyx":491
+    /* "_rtmidi.pyx":496
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and             # <<<<<<<<<<<<<<
  *                   sys.platform == 'darwin'):
  *                 encoding = 'macroman'
  */
     if (__pyx_t_1) {
 
-      /* "_rtmidi.pyx":493
+      /* "_rtmidi.pyx":498
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  *                   sys.platform == 'darwin'):
  *                 encoding = 'macroman'             # <<<<<<<<<<<<<<
  *             else:
  *                 encoding = 'utf-8'
  */
       __Pyx_INCREF(__pyx_n_u_macroman);
       __Pyx_DECREF_SET(__pyx_v_encoding, __pyx_n_u_macroman);
 
-      /* "_rtmidi.pyx":491
+      /* "_rtmidi.pyx":496
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and             # <<<<<<<<<<<<<<
  *                   sys.platform == 'darwin'):
  *                 encoding = 'macroman'
  */
       goto __pyx_L4;
     }
 
-    /* "_rtmidi.pyx":495
+    /* "_rtmidi.pyx":500
  *                 encoding = 'macroman'
  *             else:
  *                 encoding = 'utf-8'             # <<<<<<<<<<<<<<
  * 
  *         return s.decode(encoding, "ignore")
  */
     /*else*/ {
       __Pyx_INCREF(__pyx_kp_u_utf_8);
       __Pyx_DECREF_SET(__pyx_v_encoding, __pyx_kp_u_utf_8);
     }
     __pyx_L4:;
 
-    /* "_rtmidi.pyx":488
+    /* "_rtmidi.pyx":493
  *     def _decode_string(self, s, encoding='auto'):
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':             # <<<<<<<<<<<<<<
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  */
   }
 
-  /* "_rtmidi.pyx":497
+  /* "_rtmidi.pyx":502
  *                 encoding = 'utf-8'
  * 
  *         return s.decode(encoding, "ignore")             # <<<<<<<<<<<<<<
  * 
  *     def get_port_count(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 497, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 502, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -5050,49 +5057,49 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_encoding, __pyx_n_u_ignore};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_encoding, __pyx_n_u_ignore};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 502, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_v_encoding);
     __Pyx_GIVEREF(__pyx_v_encoding);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_encoding);
     __Pyx_INCREF(__pyx_n_u_ignore);
     __Pyx_GIVEREF(__pyx_n_u_ignore);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_n_u_ignore);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 502, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":486
+  /* "_rtmidi.pyx":491
  *         return inout
  * 
  *     def _decode_string(self, s, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':
  */
 
@@ -5107,15 +5114,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_encoding);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":499
+/* "_rtmidi.pyx":504
  *         return s.decode(encoding, "ignore")
  * 
  *     def get_port_count(self):             # <<<<<<<<<<<<<<
  *         """Return the number of available MIDI input or output ports."""
  *         return self.baseptr().getPortCount()
  */
 
@@ -5139,30 +5146,30 @@
   unsigned int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_port_count", 0);
 
-  /* "_rtmidi.pyx":501
+  /* "_rtmidi.pyx":506
  *     def get_port_count(self):
  *         """Return the number of available MIDI input or output ports."""
  *         return self.baseptr().getPortCount()             # <<<<<<<<<<<<<<
  * 
  *     def get_port_name(self, unsigned int port, encoding='auto'):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->getPortCount(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 501, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->getPortCount(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":499
+  /* "_rtmidi.pyx":504
  *         return s.decode(encoding, "ignore")
  * 
  *     def get_port_count(self):             # <<<<<<<<<<<<<<
  *         """Return the number of available MIDI input or output ports."""
  *         return self.baseptr().getPortCount()
  */
 
@@ -5173,15 +5180,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":503
+/* "_rtmidi.pyx":508
  *         return self.baseptr().getPortCount()
  * 
  *     def get_port_name(self, unsigned int port, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Return the name of the MIDI input or output port with given number.
  * 
  */
 
@@ -5221,31 +5228,31 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_port_name") < 0)) __PYX_ERR(0, 503, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_port_name") < 0)) __PYX_ERR(0, 508, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_port = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_port == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 503, __pyx_L3_error)
+    __pyx_v_port = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_port == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 508, __pyx_L3_error)
     __pyx_v_encoding = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_port_name", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 503, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_port_name", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 508, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiBase.get_port_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_10get_port_name(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_port, __pyx_v_encoding);
 
@@ -5269,51 +5276,51 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_port_name", 0);
 
-  /* "_rtmidi.pyx":517
+  /* "_rtmidi.pyx":522
  * 
  *         """
  *         cdef string name = self.baseptr().getPortName(port)             # <<<<<<<<<<<<<<
  * 
  *         if len(name):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->getPortName(__pyx_v_port); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 517, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->getPortName(__pyx_v_port); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 522, __pyx_L1_error)
   __pyx_v_name = __pyx_t_1;
 
-  /* "_rtmidi.pyx":519
+  /* "_rtmidi.pyx":524
  *         cdef string name = self.baseptr().getPortName(port)
  * 
  *         if len(name):             # <<<<<<<<<<<<<<
  *             return self._decode_string(name, encoding) if encoding else name
  * 
  */
-  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 524, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 519, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 524, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "_rtmidi.pyx":520
+    /* "_rtmidi.pyx":525
  * 
  *         if len(name):
  *             return self._decode_string(name, encoding) if encoding else name             # <<<<<<<<<<<<<<
  * 
  *     def get_ports(self, encoding='auto'):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_encoding); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 520, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_encoding); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 525, __pyx_L1_error)
     if (__pyx_t_4) {
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 520, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 525, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 520, __pyx_L1_error)
+      __pyx_t_7 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 525, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -5322,68 +5329,68 @@
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_7, __pyx_v_encoding};
-        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 525, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_7, __pyx_v_encoding};
-        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 525, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       {
-        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 520, __pyx_L1_error)
+        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 525, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (__pyx_t_8) {
           __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_7);
         __Pyx_INCREF(__pyx_v_encoding);
         __Pyx_GIVEREF(__pyx_v_encoding);
         PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_v_encoding);
         __pyx_t_7 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 525, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_2 = __pyx_t_5;
       __pyx_t_5 = 0;
     } else {
-      __pyx_t_5 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
+      __pyx_t_5 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 525, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_2 = __pyx_t_5;
       __pyx_t_5 = 0;
     }
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "_rtmidi.pyx":519
+    /* "_rtmidi.pyx":524
  *         cdef string name = self.baseptr().getPortName(port)
  * 
  *         if len(name):             # <<<<<<<<<<<<<<
  *             return self._decode_string(name, encoding) if encoding else name
  * 
  */
   }
 
-  /* "_rtmidi.pyx":503
+  /* "_rtmidi.pyx":508
  *         return self.baseptr().getPortCount()
  * 
  *     def get_port_name(self, unsigned int port, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Return the name of the MIDI input or output port with given number.
  * 
  */
 
@@ -5401,15 +5408,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":522
+/* "_rtmidi.pyx":527
  *             return self._decode_string(name, encoding) if encoding else name
  * 
  *     def get_ports(self, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Return a list of names of available MIDI input or output ports.
  * 
  */
 
@@ -5442,29 +5449,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_ports") < 0)) __PYX_ERR(0, 522, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_ports") < 0)) __PYX_ERR(0, 527, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_encoding = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_ports", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 522, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_ports", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 527, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiBase.get_ports", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_12get_ports(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_encoding);
 
@@ -5486,122 +5493,122 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_ports", 0);
 
-  /* "_rtmidi.pyx":534
+  /* "_rtmidi.pyx":539
  * 
  *         """
  *         return [self.get_port_name(p, encoding=encoding)             # <<<<<<<<<<<<<<
  *                 for p in range(self.get_port_count())]
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 534, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 539, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "_rtmidi.pyx":535
+    /* "_rtmidi.pyx":540
  *         """
  *         return [self.get_port_name(p, encoding=encoding)
  *                 for p in range(self.get_port_count())]             # <<<<<<<<<<<<<<
  * 
  *     def is_port_open(self):
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_port_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_port_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 535, __pyx_L5_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 540, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
       __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 535, __pyx_L5_error)
+      __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 540, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 535, __pyx_L5_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 540, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 535, __pyx_L5_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 540, __pyx_L5_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L5_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 535, __pyx_L5_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 540, __pyx_L5_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L5_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 540, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_6(__pyx_t_2);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 535, __pyx_L5_error)
+            else __PYX_ERR(0, 540, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_p, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "_rtmidi.pyx":534
+      /* "_rtmidi.pyx":539
  * 
  *         """
  *         return [self.get_port_name(p, encoding=encoding)             # <<<<<<<<<<<<<<
  *                 for p in range(self.get_port_count())]
  * 
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_port_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 534, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_port_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 539, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 534, __pyx_L5_error)
+      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 539, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_8genexpr2__pyx_v_p);
       __Pyx_GIVEREF(__pyx_8genexpr2__pyx_v_p);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_8genexpr2__pyx_v_p);
-      __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 534, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 539, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_encoding, __pyx_v_encoding) < 0) __PYX_ERR(0, 534, __pyx_L5_error)
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 534, __pyx_L5_error)
+      if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_encoding, __pyx_v_encoding) < 0) __PYX_ERR(0, 539, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 539, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 534, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 539, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "_rtmidi.pyx":535
+      /* "_rtmidi.pyx":540
  *         """
  *         return [self.get_port_name(p, encoding=encoding)
  *                 for p in range(self.get_port_count())]             # <<<<<<<<<<<<<<
  * 
  *     def is_port_open(self):
  */
     }
@@ -5613,15 +5620,15 @@
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":522
+  /* "_rtmidi.pyx":527
  *             return self._decode_string(name, encoding) if encoding else name
  * 
  *     def get_ports(self, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Return a list of names of available MIDI input or output ports.
  * 
  */
 
@@ -5638,15 +5645,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_p);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":537
+/* "_rtmidi.pyx":542
  *                 for p in range(self.get_port_count())]
  * 
  *     def is_port_open(self):             # <<<<<<<<<<<<<<
  *         """Return ``True`` if a port has been opened and ``False`` if not.
  * 
  */
 
@@ -5670,30 +5677,30 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_port_open", 0);
 
-  /* "_rtmidi.pyx":546
+  /* "_rtmidi.pyx":551
  * 
  *         """
  *         return self._port is not None             # <<<<<<<<<<<<<<
  * 
  *     def open_port(self, unsigned int port=0, name=None):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = (__pyx_v_self->_port != Py_None);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 551, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":537
+  /* "_rtmidi.pyx":542
  *                 for p in range(self.get_port_count())]
  * 
  *     def is_port_open(self):             # <<<<<<<<<<<<<<
  *         """Return ``True`` if a port has been opened and ``False`` if not.
  * 
  */
 
@@ -5704,15 +5711,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":548
+/* "_rtmidi.pyx":553
  *         return self._port is not None
  * 
  *     def open_port(self, unsigned int port=0, name=None):             # <<<<<<<<<<<<<<
  *         """Open the MIDI input or output port with the given port number.
  * 
  */
 
@@ -5754,36 +5761,36 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open_port") < 0)) __PYX_ERR(0, 548, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open_port") < 0)) __PYX_ERR(0, 553, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_port = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_port == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 548, __pyx_L3_error)
+      __pyx_v_port = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_port == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 553, __pyx_L3_error)
     } else {
       __pyx_v_port = ((unsigned int)0);
     }
     __pyx_v_name = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open_port", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 548, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open_port", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 553, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiBase.open_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_16open_port(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_port, __pyx_v_name);
 
@@ -5804,129 +5811,129 @@
   std::string __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open_port", 0);
   __Pyx_INCREF(__pyx_v_name);
 
-  /* "_rtmidi.pyx":580
+  /* "_rtmidi.pyx":585
  * 
  *         """
  *         inout = self._check_port()             # <<<<<<<<<<<<<<
  * 
  *         if name is None:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_check_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_check_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_inout = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":582
+  /* "_rtmidi.pyx":587
  *         inout = self._check_port()
  * 
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidi %s" % inout
  * 
  */
   __pyx_t_4 = (__pyx_v_name == Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "_rtmidi.pyx":583
+    /* "_rtmidi.pyx":588
  * 
  *         if name is None:
  *             name = "RtMidi %s" % inout             # <<<<<<<<<<<<<<
  * 
  *         self.baseptr().openPort(port, _to_bytes(name))
  */
-    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_RtMidi_s, __pyx_v_inout); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 583, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_RtMidi_s, __pyx_v_inout); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_name, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "_rtmidi.pyx":582
+    /* "_rtmidi.pyx":587
  *         inout = self._check_port()
  * 
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidi %s" % inout
  * 
  */
   }
 
-  /* "_rtmidi.pyx":585
+  /* "_rtmidi.pyx":590
  *             name = "RtMidi %s" % inout
  * 
  *         self.baseptr().openPort(port, _to_bytes(name))             # <<<<<<<<<<<<<<
  *         self._port = port
  *         return self
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 585, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 585, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 585, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 590, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->openPort(__pyx_v_port, __pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 585, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->openPort(__pyx_v_port, __pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 590, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":586
+  /* "_rtmidi.pyx":591
  * 
  *         self.baseptr().openPort(port, _to_bytes(name))
  *         self._port = port             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_unsigned_int(__pyx_v_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_unsigned_int(__pyx_v_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_port);
   __Pyx_DECREF(__pyx_v_self->_port);
   __pyx_v_self->_port = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":587
+  /* "_rtmidi.pyx":592
  *         self.baseptr().openPort(port, _to_bytes(name))
  *         self._port = port
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def open_virtual_port(self, name=None):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":548
+  /* "_rtmidi.pyx":553
  *         return self._port is not None
  * 
  *     def open_port(self, unsigned int port=0, name=None):             # <<<<<<<<<<<<<<
  *         """Open the MIDI input or output port with the given port number.
  * 
  */
 
@@ -5941,15 +5948,15 @@
   __Pyx_XDECREF(__pyx_v_inout);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":589
+/* "_rtmidi.pyx":594
  *         return self
  * 
  *     def open_virtual_port(self, name=None):             # <<<<<<<<<<<<<<
  *         """Open a virtual MIDI input or output port.
  * 
  */
 
@@ -5982,29 +5989,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open_virtual_port") < 0)) __PYX_ERR(0, 589, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open_virtual_port") < 0)) __PYX_ERR(0, 594, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_name = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open_virtual_port", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 589, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open_virtual_port", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 594, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiBase.open_virtual_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_18open_virtual_port(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_name);
 
@@ -6024,130 +6031,130 @@
   PyObject *__pyx_t_5 = NULL;
   std::string __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open_virtual_port", 0);
 
-  /* "_rtmidi.pyx":640
+  /* "_rtmidi.pyx":645
  * 
  *         """
  *         if self.get_current_api() == API_WINDOWS_MM:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError("Virtual ports are not supported "
  *                                       "by the Windows MultiMedia API.")
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 640, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 640, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 640, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 640, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 640, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_t_4)) {
 
-    /* "_rtmidi.pyx":641
+    /* "_rtmidi.pyx":646
  *         """
  *         if self.get_current_api() == API_WINDOWS_MM:
  *             raise NotImplementedError("Virtual ports are not supported "             # <<<<<<<<<<<<<<
  *                                       "by the Windows MultiMedia API.")
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 641, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 646, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 641, __pyx_L1_error)
+    __PYX_ERR(0, 646, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":640
+    /* "_rtmidi.pyx":645
  * 
  *         """
  *         if self.get_current_api() == API_WINDOWS_MM:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError("Virtual ports are not supported "
  *                                       "by the Windows MultiMedia API.")
  */
   }
 
-  /* "_rtmidi.pyx":644
+  /* "_rtmidi.pyx":649
  *                                       "by the Windows MultiMedia API.")
  * 
  *         inout = self._check_port()             # <<<<<<<<<<<<<<
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)
  *                                                 if name is None else name))
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_check_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_check_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 644, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_inout = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "_rtmidi.pyx":645
+  /* "_rtmidi.pyx":650
  * 
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)             # <<<<<<<<<<<<<<
  *                                                 if name is None else name))
  *         self._port = -1
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 645, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "_rtmidi.pyx":646
+  /* "_rtmidi.pyx":651
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)
  *                                                 if name is None else name))             # <<<<<<<<<<<<<<
  *         self._port = -1
  *         return self
  */
   __pyx_t_4 = (__pyx_v_name == Py_None);
   if ((__pyx_t_4 != 0)) {
 
-    /* "_rtmidi.pyx":645
+    /* "_rtmidi.pyx":650
  * 
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)             # <<<<<<<<<<<<<<
  *                                                 if name is None else name))
  *         self._port = -1
  */
-    __pyx_t_5 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_RtMidi_virtual_s, __pyx_v_inout); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 645, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_RtMidi_virtual_s, __pyx_v_inout); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 650, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = __pyx_t_5;
     __pyx_t_5 = 0;
   } else {
 
-    /* "_rtmidi.pyx":646
+    /* "_rtmidi.pyx":651
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)
  *                                                 if name is None else name))             # <<<<<<<<<<<<<<
  *         self._port = -1
  *         return self
  */
     __Pyx_INCREF(__pyx_v_name);
@@ -6162,55 +6169,55 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 645, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "_rtmidi.pyx":645
+  /* "_rtmidi.pyx":650
  * 
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)             # <<<<<<<<<<<<<<
  *                                                 if name is None else name))
  *         self._port = -1
  */
-  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->openVirtualPort(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->openVirtualPort(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 650, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":647
+  /* "_rtmidi.pyx":652
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)
  *                                                 if name is None else name))
  *         self._port = -1             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
   __Pyx_GOTREF(__pyx_v_self->_port);
   __Pyx_DECREF(__pyx_v_self->_port);
   __pyx_v_self->_port = __pyx_int_neg_1;
 
-  /* "_rtmidi.pyx":648
+  /* "_rtmidi.pyx":653
  *                                                 if name is None else name))
  *         self._port = -1
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def close_port(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":589
+  /* "_rtmidi.pyx":594
  *         return self
  * 
  *     def open_virtual_port(self, name=None):             # <<<<<<<<<<<<<<
  *         """Open a virtual MIDI input or output port.
  * 
  */
 
@@ -6225,15 +6232,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_inout);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":650
+/* "_rtmidi.pyx":655
  *         return self
  * 
  *     def close_port(self):             # <<<<<<<<<<<<<<
  *         """Close the MIDI input or output port opened via ``open_port``.
  * 
  */
 
@@ -6257,59 +6264,59 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close_port", 0);
 
-  /* "_rtmidi.pyx":662
+  /* "_rtmidi.pyx":667
  * 
  *         """
  *         if self._port != -1:             # <<<<<<<<<<<<<<
  *             self._port = None
  *         self.baseptr().closePort()
  */
-  __pyx_t_1 = __Pyx_PyInt_NeObjC(__pyx_v_self->_port, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_NeObjC(__pyx_v_self->_port, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 662, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 667, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "_rtmidi.pyx":663
+    /* "_rtmidi.pyx":668
  *         """
  *         if self._port != -1:
  *             self._port = None             # <<<<<<<<<<<<<<
  *         self.baseptr().closePort()
  * 
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_port);
     __Pyx_DECREF(__pyx_v_self->_port);
     __pyx_v_self->_port = Py_None;
 
-    /* "_rtmidi.pyx":662
+    /* "_rtmidi.pyx":667
  * 
  *         """
  *         if self._port != -1:             # <<<<<<<<<<<<<<
  *             self._port = None
  *         self.baseptr().closePort()
  */
   }
 
-  /* "_rtmidi.pyx":664
+  /* "_rtmidi.pyx":669
  *         if self._port != -1:
  *             self._port = None
  *         self.baseptr().closePort()             # <<<<<<<<<<<<<<
  * 
  *     def set_client_name(self, name):
  */
-  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->closePort(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 664, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->closePort(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 669, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":650
+  /* "_rtmidi.pyx":655
  *         return self
  * 
  *     def close_port(self):             # <<<<<<<<<<<<<<
  *         """Close the MIDI input or output port opened via ``open_port``.
  * 
  */
 
@@ -6322,15 +6329,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":666
+/* "_rtmidi.pyx":671
  *         self.baseptr().closePort()
  * 
  *     def set_client_name(self, name):             # <<<<<<<<<<<<<<
  *         """Set the name of the MIDI client.
  * 
  */
 
@@ -6358,123 +6365,123 @@
   int __pyx_t_5;
   std::string __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_client_name", 0);
 
-  /* "_rtmidi.pyx":684
+  /* "_rtmidi.pyx":689
  * 
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_UNIX_JACK, API_WINDOWS_MM):             # <<<<<<<<<<<<<<
  *             raise NotImplementedError(
  *                 "API backend does not support changing the client name.")
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 684, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_UNIX_JACK); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_UNIX_JACK); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "_rtmidi.pyx":685
+    /* "_rtmidi.pyx":690
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_UNIX_JACK, API_WINDOWS_MM):
  *             raise NotImplementedError(             # <<<<<<<<<<<<<<
  *                 "API backend does not support changing the client name.")
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 685, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 690, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 685, __pyx_L1_error)
+    __PYX_ERR(0, 690, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":684
+    /* "_rtmidi.pyx":689
  * 
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_UNIX_JACK, API_WINDOWS_MM):             # <<<<<<<<<<<<<<
  *             raise NotImplementedError(
  *                 "API backend does not support changing the client name.")
  */
   }
 
-  /* "_rtmidi.pyx":688
+  /* "_rtmidi.pyx":693
  *                 "API backend does not support changing the client name.")
  * 
  *         self.baseptr().setClientName(_to_bytes(name))             # <<<<<<<<<<<<<<
  * 
  *     def set_port_name(self, name):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 688, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 688, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setClientName(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 688, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setClientName(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 693, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":666
+  /* "_rtmidi.pyx":671
  *         self.baseptr().closePort()
  * 
  *     def set_client_name(self, name):             # <<<<<<<<<<<<<<
  *         """Set the name of the MIDI client.
  * 
  */
 
@@ -6489,15 +6496,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":690
+/* "_rtmidi.pyx":695
  *         self.baseptr().setClientName(_to_bytes(name))
  * 
  *     def set_port_name(self, name):             # <<<<<<<<<<<<<<
  *         """Set the name of the currently opened port.
  * 
  */
 
@@ -6525,175 +6532,175 @@
   int __pyx_t_5;
   std::string __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_port_name", 0);
 
-  /* "_rtmidi.pyx":710
+  /* "_rtmidi.pyx":715
  * 
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_WINDOWS_MM):             # <<<<<<<<<<<<<<
  *             raise UnsupportedOperationError(
  *                 "API backend does not support changing the port name.")
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 710, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 710, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 715, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "_rtmidi.pyx":711
+    /* "_rtmidi.pyx":716
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_WINDOWS_MM):
  *             raise UnsupportedOperationError(             # <<<<<<<<<<<<<<
  *                 "API backend does not support changing the port name.")
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnsupportedOperationError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnsupportedOperationError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 716, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_API_backend_does_not_support_cha_2) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_API_backend_does_not_support_cha_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 711, __pyx_L1_error)
+    __PYX_ERR(0, 716, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":710
+    /* "_rtmidi.pyx":715
  * 
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_WINDOWS_MM):             # <<<<<<<<<<<<<<
  *             raise UnsupportedOperationError(
  *                 "API backend does not support changing the port name.")
  */
   }
 
-  /* "_rtmidi.pyx":714
+  /* "_rtmidi.pyx":719
  *                 "API backend does not support changing the port name.")
  * 
  *         if self._port is None:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("No port currently opened.")
  * 
  */
   __pyx_t_5 = (__pyx_v_self->_port == Py_None);
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "_rtmidi.pyx":715
+    /* "_rtmidi.pyx":720
  * 
  *         if self._port is None:
  *             raise InvalidUseError("No port currently opened.")             # <<<<<<<<<<<<<<
  * 
  *         self.baseptr().setPortName(_to_bytes(name))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 715, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 720, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_No_port_currently_opened) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_No_port_currently_opened);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 720, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 715, __pyx_L1_error)
+    __PYX_ERR(0, 720, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":714
+    /* "_rtmidi.pyx":719
  *                 "API backend does not support changing the port name.")
  * 
  *         if self._port is None:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("No port currently opened.")
  * 
  */
   }
 
-  /* "_rtmidi.pyx":717
+  /* "_rtmidi.pyx":722
  *             raise InvalidUseError("No port currently opened.")
  * 
  *         self.baseptr().setPortName(_to_bytes(name))             # <<<<<<<<<<<<<<
  * 
  *     def set_error_callback(self, func, data=None):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 717, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 722, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 717, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 722, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 717, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 722, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setPortName(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 717, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setPortName(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 722, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":690
+  /* "_rtmidi.pyx":695
  *         self.baseptr().setClientName(_to_bytes(name))
  * 
  *     def set_port_name(self, name):             # <<<<<<<<<<<<<<
  *         """Set the name of the currently opened port.
  * 
  */
 
@@ -6708,15 +6715,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":719
+/* "_rtmidi.pyx":724
  *         self.baseptr().setPortName(_to_bytes(name))
  * 
  *     def set_error_callback(self, func, data=None):             # <<<<<<<<<<<<<<
  *         """Register a callback function for errors.
  * 
  */
 
@@ -6756,15 +6763,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_error_callback") < 0)) __PYX_ERR(0, 719, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_error_callback") < 0)) __PYX_ERR(0, 724, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -6772,15 +6779,15 @@
       }
     }
     __pyx_v_func = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_error_callback", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 719, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_error_callback", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 724, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiBase.set_error_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_26set_error_callback(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_func, __pyx_v_data);
 
@@ -6795,24 +6802,24 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_error_callback", 0);
 
-  /* "_rtmidi.pyx":742
+  /* "_rtmidi.pyx":747
  * 
  *         """
  *         self._error_callback = (func, data, self._decode_string)             # <<<<<<<<<<<<<<
  *         self.baseptr().setErrorCallback(&_cb_error_func,
  *                                         <void *>self._error_callback)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 742, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 742, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_func);
   __Pyx_GIVEREF(__pyx_v_func);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_func);
   __Pyx_INCREF(__pyx_v_data);
   __Pyx_GIVEREF(__pyx_v_data);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_data);
@@ -6821,24 +6828,24 @@
   __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_error_callback);
   __Pyx_DECREF(__pyx_v_self->_error_callback);
   __pyx_v_self->_error_callback = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "_rtmidi.pyx":743
+  /* "_rtmidi.pyx":748
  *         """
  *         self._error_callback = (func, data, self._decode_string)
  *         self.baseptr().setErrorCallback(&_cb_error_func,             # <<<<<<<<<<<<<<
  *                                         <void *>self._error_callback)
  * 
  */
-  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setErrorCallback((&__pyx_f_7_rtmidi__cb_error_func), ((void *)__pyx_v_self->_error_callback)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 743, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setErrorCallback((&__pyx_f_7_rtmidi__cb_error_func), ((void *)__pyx_v_self->_error_callback)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 748, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":719
+  /* "_rtmidi.pyx":724
  *         self.baseptr().setPortName(_to_bytes(name))
  * 
  *     def set_error_callback(self, func, data=None):             # <<<<<<<<<<<<<<
  *         """Register a callback function for errors.
  * 
  */
 
@@ -6852,15 +6859,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":746
+/* "_rtmidi.pyx":751
  *                                         <void *>self._error_callback)
  * 
  *     def cancel_error_callback(self):             # <<<<<<<<<<<<<<
  *         """Remove the registered callback function for errors.
  * 
  */
 
@@ -6886,44 +6893,44 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cancel_error_callback", 0);
 
-  /* "_rtmidi.pyx":753
+  /* "_rtmidi.pyx":758
  * 
  *         """
  *         self.set_error_callback(_default_error_handler)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 753, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 758, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 753, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 758, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 753, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 758, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":746
+  /* "_rtmidi.pyx":751
  *                                         <void *>self._error_callback)
  * 
  *     def cancel_error_callback(self):             # <<<<<<<<<<<<<<
  *         """Remove the registered callback function for errors.
  * 
  */
 
@@ -7258,52 +7265,52 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":800
+/* "_rtmidi.pyx":805
  *     cdef object _callback
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr
  * 
  */
 
 static RtMidi *__pyx_f_7_rtmidi_6MidiIn_baseptr(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   RtMidi *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("baseptr", 0);
 
-  /* "_rtmidi.pyx":801
+  /* "_rtmidi.pyx":806
  * 
  *     cdef RtMidi* baseptr(self):
  *         return self.thisptr             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None,
  */
   __pyx_r = __pyx_v_self->thisptr;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":800
+  /* "_rtmidi.pyx":805
  *     cdef object _callback
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":803
+/* "_rtmidi.pyx":808
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None,             # <<<<<<<<<<<<<<
  *                   unsigned int queue_size_limit=1024):
  *         """Create a new client instance for MIDI input.
  */
 
@@ -7353,43 +7360,43 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_queue_size_limit);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 803, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 808, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_rtapi = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 803, __pyx_L3_error)
+      __pyx_v_rtapi = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 808, __pyx_L3_error)
     } else {
       __pyx_v_rtapi = __pyx_k__4;
     }
     __pyx_v_name = values[1];
     if (values[2]) {
-      __pyx_v_queue_size_limit = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_queue_size_limit == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 804, __pyx_L3_error)
+      __pyx_v_queue_size_limit = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_queue_size_limit == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 809, __pyx_L3_error)
     } else {
       __pyx_v_queue_size_limit = ((unsigned int)0x400);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 803, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 808, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiIn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_6MidiIn___cinit__(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self), __pyx_v_rtapi, __pyx_v_name, __pyx_v_queue_size_limit);
 
@@ -7427,45 +7434,45 @@
   PyObject *__pyx_t_23 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
   __Pyx_INCREF(__pyx_v_name);
 
-  /* "_rtmidi.pyx":810
+  /* "_rtmidi.pyx":815
  * 
  *         """
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidiIn Client"
  * 
  */
   __pyx_t_1 = (__pyx_v_name == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "_rtmidi.pyx":811
+    /* "_rtmidi.pyx":816
  *         """
  *         if name is None:
  *             name = "RtMidiIn Client"             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
     __Pyx_INCREF(__pyx_kp_u_RtMidiIn_Client);
     __Pyx_DECREF_SET(__pyx_v_name, __pyx_kp_u_RtMidiIn_Client);
 
-    /* "_rtmidi.pyx":810
+    /* "_rtmidi.pyx":815
  * 
  *         """
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidiIn Client"
  * 
  */
   }
 
-  /* "_rtmidi.pyx":813
+  /* "_rtmidi.pyx":818
  *             name = "RtMidiIn Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:
  */
   {
@@ -7473,49 +7480,49 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_5);
     /*try:*/ {
 
-      /* "_rtmidi.pyx":814
+      /* "_rtmidi.pyx":819
  * 
  *         try:
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)             # <<<<<<<<<<<<<<
  *         except RuntimeError as exc:
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 814, __pyx_L4_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 819, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_name);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 814, __pyx_L4_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 819, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 814, __pyx_L4_error)
+      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 819, __pyx_L4_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       try {
         __pyx_t_10 = new RtMidiIn(__pyx_v_rtapi, __pyx_t_9, __pyx_v_queue_size_limit);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 814, __pyx_L4_error)
+        __PYX_ERR(0, 819, __pyx_L4_error)
       }
       __pyx_v_self->thisptr = __pyx_t_10;
 
-      /* "_rtmidi.pyx":813
+      /* "_rtmidi.pyx":818
  *             name = "RtMidiIn Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:
  */
     }
@@ -7524,65 +7531,65 @@
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L9_try_end;
     __pyx_L4_error:;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "_rtmidi.pyx":815
+    /* "_rtmidi.pyx":820
  *         try:
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:             # <<<<<<<<<<<<<<
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  */
     __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_RuntimeError);
     if (__pyx_t_11) {
       __Pyx_AddTraceback("_rtmidi.MidiIn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 815, __pyx_L6_except_error)
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 820, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __pyx_v_exc = __pyx_t_7;
       /*try:*/ {
 
-        /* "_rtmidi.pyx":816
+        /* "_rtmidi.pyx":821
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  * 
  *         self.set_error_callback(_default_error_handler)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 816, __pyx_L15_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 821, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_exc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 816, __pyx_L15_error)
+        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_exc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 821, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 816, __pyx_L15_error)
+        __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 821, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_GIVEREF(__pyx_t_13);
         PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13);
         __pyx_t_13 = 0;
-        __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 816, __pyx_L15_error)
+        __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 821, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_15 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 816, __pyx_L15_error)
+        __pyx_t_15 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 821, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_15);
-        if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_type, __pyx_t_15) < 0) __PYX_ERR(0, 816, __pyx_L15_error)
+        if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_type, __pyx_t_15) < 0) __PYX_ERR(0, 821, __pyx_L15_error)
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 816, __pyx_L15_error)
+        __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 821, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_Raise(__pyx_t_15, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __PYX_ERR(0, 816, __pyx_L15_error)
+        __PYX_ERR(0, 821, __pyx_L15_error)
       }
 
-      /* "_rtmidi.pyx":815
+      /* "_rtmidi.pyx":820
  *         try:
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:             # <<<<<<<<<<<<<<
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  */
       /*finally:*/ {
@@ -7623,98 +7630,98 @@
           goto __pyx_L6_except_error;
         }
       }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
-    /* "_rtmidi.pyx":813
+    /* "_rtmidi.pyx":818
  *             name = "RtMidiIn Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:
  */
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     goto __pyx_L1_error;
     __pyx_L9_try_end:;
   }
 
-  /* "_rtmidi.pyx":818
+  /* "_rtmidi.pyx":823
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  *         self.set_error_callback(_default_error_handler)             # <<<<<<<<<<<<<<
  *         self._callback = None
  *         self._port = None
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 818, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 823, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 818, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 823, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_8 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_15, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 818, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 823, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "_rtmidi.pyx":819
+  /* "_rtmidi.pyx":824
  * 
  *         self.set_error_callback(_default_error_handler)
  *         self._callback = None             # <<<<<<<<<<<<<<
  *         self._port = None
  *         self._deleted = False
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_callback);
   __Pyx_DECREF(__pyx_v_self->_callback);
   __pyx_v_self->_callback = Py_None;
 
-  /* "_rtmidi.pyx":820
+  /* "_rtmidi.pyx":825
  *         self.set_error_callback(_default_error_handler)
  *         self._callback = None
  *         self._port = None             # <<<<<<<<<<<<<<
  *         self._deleted = False
  * 
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base._port);
   __Pyx_DECREF(__pyx_v_self->__pyx_base._port);
   __pyx_v_self->__pyx_base._port = Py_None;
 
-  /* "_rtmidi.pyx":821
+  /* "_rtmidi.pyx":826
  *         self._callback = None
  *         self._port = None
  *         self._deleted = False             # <<<<<<<<<<<<<<
  * 
  *     def get_current_api(self):
  */
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base._deleted);
   __Pyx_DECREF(__pyx_v_self->__pyx_base._deleted);
   __pyx_v_self->__pyx_base._deleted = Py_False;
 
-  /* "_rtmidi.pyx":803
+  /* "_rtmidi.pyx":808
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None,             # <<<<<<<<<<<<<<
  *                   unsigned int queue_size_limit=1024):
  *         """Create a new client instance for MIDI input.
  */
 
@@ -7734,15 +7741,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_exc);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":823
+/* "_rtmidi.pyx":828
  *         self._deleted = False
  * 
  *     def get_current_api(self):             # <<<<<<<<<<<<<<
  *         """Return the low-level MIDI backend API used by this instance.
  * 
  */
 
@@ -7765,29 +7772,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_current_api", 0);
 
-  /* "_rtmidi.pyx":835
+  /* "_rtmidi.pyx":840
  * 
  *         """
  *         return self.thisptr.getCurrentApi()             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(__pyx_v_self->thisptr->getCurrentApi()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 835, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(__pyx_v_self->thisptr->getCurrentApi()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 840, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":823
+  /* "_rtmidi.pyx":828
  *         self._deleted = False
  * 
  *     def get_current_api(self):             # <<<<<<<<<<<<<<
  *         """Return the low-level MIDI backend API used by this instance.
  * 
  */
 
@@ -7798,15 +7805,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":837
+/* "_rtmidi.pyx":842
  *         return self.thisptr.getCurrentApi()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  */
 
@@ -7826,44 +7833,44 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "_rtmidi.pyx":839
+  /* "_rtmidi.pyx":844
  *     def __dealloc__(self):
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):             # <<<<<<<<<<<<<<
  *             del self.thisptr
  * 
  */
-  __pyx_t_1 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_thisptr); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 839, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_thisptr); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 844, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "_rtmidi.pyx":840
+    /* "_rtmidi.pyx":845
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  *             del self.thisptr             # <<<<<<<<<<<<<<
  * 
  *     def delete(self):
  */
     delete __pyx_v_self->thisptr;
 
-    /* "_rtmidi.pyx":839
+    /* "_rtmidi.pyx":844
  *     def __dealloc__(self):
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):             # <<<<<<<<<<<<<<
  *             del self.thisptr
  * 
  */
   }
 
-  /* "_rtmidi.pyx":837
+  /* "_rtmidi.pyx":842
  *         return self.thisptr.getCurrentApi()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  */
 
@@ -7871,15 +7878,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("_rtmidi.MidiIn.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "_rtmidi.pyx":842
+/* "_rtmidi.pyx":847
  *             del self.thisptr
  * 
  *     def delete(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance.
  * 
  */
 
@@ -7903,57 +7910,57 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("delete", 0);
 
-  /* "_rtmidi.pyx":859
+  /* "_rtmidi.pyx":864
  * 
  *         """
  *         if not self._deleted:             # <<<<<<<<<<<<<<
  *             del self.thisptr
  *             self._deleted = True
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->__pyx_base._deleted); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 859, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->__pyx_base._deleted); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 864, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (__pyx_t_2) {
 
-    /* "_rtmidi.pyx":860
+    /* "_rtmidi.pyx":865
  *         """
  *         if not self._deleted:
  *             del self.thisptr             # <<<<<<<<<<<<<<
  *             self._deleted = True
  * 
  */
     delete __pyx_v_self->thisptr;
 
-    /* "_rtmidi.pyx":861
+    /* "_rtmidi.pyx":866
  *         if not self._deleted:
  *             del self.thisptr
  *             self._deleted = True             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
     __Pyx_INCREF(Py_True);
     __Pyx_GIVEREF(Py_True);
     __Pyx_GOTREF(__pyx_v_self->__pyx_base._deleted);
     __Pyx_DECREF(__pyx_v_self->__pyx_base._deleted);
     __pyx_v_self->__pyx_base._deleted = Py_True;
 
-    /* "_rtmidi.pyx":859
+    /* "_rtmidi.pyx":864
  * 
  *         """
  *         if not self._deleted:             # <<<<<<<<<<<<<<
  *             del self.thisptr
  *             self._deleted = True
  */
   }
 
-  /* "_rtmidi.pyx":842
+  /* "_rtmidi.pyx":847
  *             del self.thisptr
  * 
  *     def delete(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance.
  * 
  */
 
@@ -7965,15 +7972,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":864
+/* "_rtmidi.pyx":869
  * 
  *     @property
  *     def is_deleted(self):             # <<<<<<<<<<<<<<
  *         return self._deleted
  * 
  */
 
@@ -7991,42 +7998,42 @@
 }
 
 static PyObject *__pyx_pf_7_rtmidi_6MidiIn_10is_deleted___get__(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_rtmidi.pyx":865
+  /* "_rtmidi.pyx":870
  *     @property
  *     def is_deleted(self):
  *         return self._deleted             # <<<<<<<<<<<<<<
  * 
  *     def cancel_callback(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->__pyx_base._deleted);
   __pyx_r = __pyx_v_self->__pyx_base._deleted;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":864
+  /* "_rtmidi.pyx":869
  * 
  *     @property
  *     def is_deleted(self):             # <<<<<<<<<<<<<<
  *         return self._deleted
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":867
+/* "_rtmidi.pyx":872
  *         return self._deleted
  * 
  *     def cancel_callback(self):             # <<<<<<<<<<<<<<
  *         """Remove the registered callback function for MIDI input.
  * 
  */
 
@@ -8049,56 +8056,56 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cancel_callback", 0);
 
-  /* "_rtmidi.pyx":874
+  /* "_rtmidi.pyx":879
  * 
  *         """
  *         if self._callback:             # <<<<<<<<<<<<<<
  *             self.thisptr.cancelCallback()
  *             self._callback = None
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 874, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 879, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "_rtmidi.pyx":875
+    /* "_rtmidi.pyx":880
  *         """
  *         if self._callback:
  *             self.thisptr.cancelCallback()             # <<<<<<<<<<<<<<
  *             self._callback = None
  * 
  */
-    __pyx_v_self->thisptr->cancelCallback(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 875, __pyx_L1_error)
+    __pyx_v_self->thisptr->cancelCallback(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 880, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":876
+    /* "_rtmidi.pyx":881
  *         if self._callback:
  *             self.thisptr.cancelCallback()
  *             self._callback = None             # <<<<<<<<<<<<<<
  * 
  *     def close_port(self):
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_callback);
     __Pyx_DECREF(__pyx_v_self->_callback);
     __pyx_v_self->_callback = Py_None;
 
-    /* "_rtmidi.pyx":874
+    /* "_rtmidi.pyx":879
  * 
  *         """
  *         if self._callback:             # <<<<<<<<<<<<<<
  *             self.thisptr.cancelCallback()
  *             self._callback = None
  */
   }
 
-  /* "_rtmidi.pyx":867
+  /* "_rtmidi.pyx":872
  *         return self._deleted
  * 
  *     def cancel_callback(self):             # <<<<<<<<<<<<<<
  *         """Remove the registered callback function for MIDI input.
  * 
  */
 
@@ -8110,15 +8117,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":878
+/* "_rtmidi.pyx":883
  *             self._callback = None
  * 
  *     def close_port(self):             # <<<<<<<<<<<<<<
  *         self.cancel_callback()
  *         MidiBase.close_port(self)
  */
 
@@ -8143,67 +8150,67 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close_port", 0);
 
-  /* "_rtmidi.pyx":879
+  /* "_rtmidi.pyx":884
  * 
  *     def close_port(self):
  *         self.cancel_callback()             # <<<<<<<<<<<<<<
  *         MidiBase.close_port(self)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cancel_callback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 879, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cancel_callback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 879, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 884, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":880
+  /* "_rtmidi.pyx":885
  *     def close_port(self):
  *         self.cancel_callback()
  *         MidiBase.close_port(self)             # <<<<<<<<<<<<<<
  * 
  *     close_port.__doc__ == MidiBase.close_port.__doc__
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7_rtmidi_MidiBase), __pyx_n_s_close_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 880, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7_rtmidi_MidiBase), __pyx_n_s_close_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 885, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_self)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_self));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 880, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 885, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":878
+  /* "_rtmidi.pyx":883
  *             self._callback = None
  * 
  *     def close_port(self):             # <<<<<<<<<<<<<<
  *         self.cancel_callback()
  *         MidiBase.close_port(self)
  */
 
@@ -8218,15 +8225,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":884
+/* "_rtmidi.pyx":889
  *     close_port.__doc__ == MidiBase.close_port.__doc__
  * 
  *     def get_message(self):             # <<<<<<<<<<<<<<
  *         """Poll for MIDI input.
  * 
  */
 
@@ -8260,95 +8267,95 @@
   __Pyx_FakeReference<unsigned char> __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_message", 0);
 
-  /* "_rtmidi.pyx":898
+  /* "_rtmidi.pyx":903
  *         """
  *         cdef vector[unsigned char] msg_v
  *         cdef double delta_time = self.thisptr.getMessage(&msg_v)             # <<<<<<<<<<<<<<
  * 
  *         if not msg_v.empty():
  */
-  __pyx_t_1 = __pyx_v_self->thisptr->getMessage((&__pyx_v_msg_v)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 898, __pyx_L1_error)
+  __pyx_t_1 = __pyx_v_self->thisptr->getMessage((&__pyx_v_msg_v)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 903, __pyx_L1_error)
   __pyx_v_delta_time = __pyx_t_1;
 
-  /* "_rtmidi.pyx":900
+  /* "_rtmidi.pyx":905
  *         cdef double delta_time = self.thisptr.getMessage(&msg_v)
  * 
  *         if not msg_v.empty():             # <<<<<<<<<<<<<<
  *             message = [msg_v.at(i) for i in range(msg_v.size())]
  *             return (message, delta_time)
  */
   __pyx_t_2 = ((!(__pyx_v_msg_v.empty() != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "_rtmidi.pyx":901
+    /* "_rtmidi.pyx":906
  * 
  *         if not msg_v.empty():
  *             message = [msg_v.at(i) for i in range(msg_v.size())]             # <<<<<<<<<<<<<<
  *             return (message, delta_time)
  * 
  */
     { /* enter inner scope */
-      __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 901, __pyx_L1_error)
+      __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 906, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = __pyx_v_msg_v.size();
       __pyx_t_5 = __pyx_t_4;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
         __pyx_8genexpr3__pyx_v_i = __pyx_t_6;
         try {
           __pyx_t_7 = __pyx_v_msg_v.at(__pyx_8genexpr3__pyx_v_i);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 901, __pyx_L1_error)
+          __PYX_ERR(0, 906, __pyx_L1_error)
         }
-        __pyx_t_8 = __Pyx_PyInt_From_unsigned_char(__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 901, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyInt_From_unsigned_char(__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 906, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 901, __pyx_L1_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 906, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
     } /* exit inner scope */
     __pyx_v_message = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "_rtmidi.pyx":902
+    /* "_rtmidi.pyx":907
  *         if not msg_v.empty():
  *             message = [msg_v.at(i) for i in range(msg_v.size())]
  *             return (message, delta_time)             # <<<<<<<<<<<<<<
  * 
  *     def ignore_types(self, sysex=True, timing=True, active_sense=True):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 902, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 907, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 902, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 907, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_INCREF(__pyx_v_message);
     __Pyx_GIVEREF(__pyx_v_message);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_message);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_3);
     __pyx_t_3 = 0;
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "_rtmidi.pyx":900
+    /* "_rtmidi.pyx":905
  *         cdef double delta_time = self.thisptr.getMessage(&msg_v)
  * 
  *         if not msg_v.empty():             # <<<<<<<<<<<<<<
  *             message = [msg_v.at(i) for i in range(msg_v.size())]
  *             return (message, delta_time)
  */
   }
 
-  /* "_rtmidi.pyx":884
+  /* "_rtmidi.pyx":889
  *     close_port.__doc__ == MidiBase.close_port.__doc__
  * 
  *     def get_message(self):             # <<<<<<<<<<<<<<
  *         """Poll for MIDI input.
  * 
  */
 
@@ -8363,15 +8370,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_message);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":904
+/* "_rtmidi.pyx":909
  *             return (message, delta_time)
  * 
  *     def ignore_types(self, sysex=True, timing=True, active_sense=True):             # <<<<<<<<<<<<<<
  *         """Enable/Disable input filtering of certain types of MIDI events.
  * 
  */
 
@@ -8424,15 +8431,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_active_sense);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "ignore_types") < 0)) __PYX_ERR(0, 904, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "ignore_types") < 0)) __PYX_ERR(0, 909, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -8444,15 +8451,15 @@
     }
     __pyx_v_sysex = values[0];
     __pyx_v_timing = values[1];
     __pyx_v_active_sense = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("ignore_types", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 904, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("ignore_types", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 909, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiIn.ignore_types", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_14ignore_types(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self), __pyx_v_sysex, __pyx_v_timing, __pyx_v_active_sense);
 
@@ -8468,27 +8475,27 @@
   bool __pyx_t_2;
   bool __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("ignore_types", 0);
 
-  /* "_rtmidi.pyx":940
+  /* "_rtmidi.pyx":945
  * 
  *         """
  *         self.thisptr.ignoreTypes(sysex, timing, active_sense)             # <<<<<<<<<<<<<<
  * 
  *     def set_callback(self, func, data=None):
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_sysex); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 940, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_timing); if (unlikely((__pyx_t_2 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 940, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_active_sense); if (unlikely((__pyx_t_3 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 940, __pyx_L1_error)
-  __pyx_v_self->thisptr->ignoreTypes(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 940, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_sysex); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_timing); if (unlikely((__pyx_t_2 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_active_sense); if (unlikely((__pyx_t_3 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_v_self->thisptr->ignoreTypes(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 945, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":904
+  /* "_rtmidi.pyx":909
  *             return (message, delta_time)
  * 
  *     def ignore_types(self, sysex=True, timing=True, active_sense=True):             # <<<<<<<<<<<<<<
  *         """Enable/Disable input filtering of certain types of MIDI events.
  * 
  */
 
@@ -8500,15 +8507,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":942
+/* "_rtmidi.pyx":947
  *         self.thisptr.ignoreTypes(sysex, timing, active_sense)
  * 
  *     def set_callback(self, func, data=None):             # <<<<<<<<<<<<<<
  *         """Register a callback function for MIDI input.
  * 
  */
 
@@ -8548,15 +8555,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_callback") < 0)) __PYX_ERR(0, 942, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_callback") < 0)) __PYX_ERR(0, 947, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -8564,15 +8571,15 @@
       }
     }
     __pyx_v_func = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_callback", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 942, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_callback", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 947, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiIn.set_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_16set_callback(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self), __pyx_v_func, __pyx_v_data);
 
@@ -8589,90 +8596,90 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_callback", 0);
 
-  /* "_rtmidi.pyx":961
+  /* "_rtmidi.pyx":966
  * 
  *         """
  *         if self._callback:             # <<<<<<<<<<<<<<
  *             self.cancel_callback()
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 961, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 966, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "_rtmidi.pyx":962
+    /* "_rtmidi.pyx":967
  *         """
  *         if self._callback:
  *             self.cancel_callback()             # <<<<<<<<<<<<<<
  * 
  *         self._callback = (func, data)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cancel_callback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 962, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cancel_callback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 967, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 962, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 967, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "_rtmidi.pyx":961
+    /* "_rtmidi.pyx":966
  * 
  *         """
  *         if self._callback:             # <<<<<<<<<<<<<<
  *             self.cancel_callback()
  * 
  */
   }
 
-  /* "_rtmidi.pyx":964
+  /* "_rtmidi.pyx":969
  *             self.cancel_callback()
  * 
  *         self._callback = (func, data)             # <<<<<<<<<<<<<<
  *         self.thisptr.setCallback(&_cb_func, <void *>self._callback)
  * 
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 964, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 969, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_func);
   __Pyx_GIVEREF(__pyx_v_func);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_func);
   __Pyx_INCREF(__pyx_v_data);
   __Pyx_GIVEREF(__pyx_v_data);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_data);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_callback);
   __Pyx_DECREF(__pyx_v_self->_callback);
   __pyx_v_self->_callback = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "_rtmidi.pyx":965
+  /* "_rtmidi.pyx":970
  * 
  *         self._callback = (func, data)
  *         self.thisptr.setCallback(&_cb_func, <void *>self._callback)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_v_self->thisptr->setCallback((&__pyx_f_7_rtmidi__cb_func), ((void *)__pyx_v_self->_callback)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 965, __pyx_L1_error)
+  __pyx_v_self->thisptr->setCallback((&__pyx_f_7_rtmidi__cb_func), ((void *)__pyx_v_self->_callback)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 970, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":942
+  /* "_rtmidi.pyx":947
  *         self.thisptr.ignoreTypes(sysex, timing, active_sense)
  * 
  *     def set_callback(self, func, data=None):             # <<<<<<<<<<<<<<
  *         """Register a callback function for MIDI input.
  * 
  */
 
@@ -8802,52 +8809,52 @@
   __Pyx_AddTraceback("_rtmidi.MidiIn.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":1005
+/* "_rtmidi.pyx":1010
  *     cdef RtMidiOut *thisptr
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr
  * 
  */
 
 static RtMidi *__pyx_f_7_rtmidi_7MidiOut_baseptr(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self) {
   RtMidi *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("baseptr", 0);
 
-  /* "_rtmidi.pyx":1006
+  /* "_rtmidi.pyx":1011
  * 
  *     cdef RtMidi* baseptr(self):
  *         return self.thisptr             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None):
  */
   __pyx_r = __pyx_v_self->thisptr;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":1005
+  /* "_rtmidi.pyx":1010
  *     cdef RtMidiOut *thisptr
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":1008
+/* "_rtmidi.pyx":1013
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None):             # <<<<<<<<<<<<<<
  *         """Create a new client instance for MIDI output.
  * 
  */
 
@@ -8888,36 +8895,36 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 1008, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 1013, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_rtapi = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1008, __pyx_L3_error)
+      __pyx_v_rtapi = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1013, __pyx_L3_error)
     } else {
       __pyx_v_rtapi = __pyx_k__7;
     }
     __pyx_v_name = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1008, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1013, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("_rtmidi.MidiOut.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7_rtmidi_7MidiOut___cinit__(((struct __pyx_obj_7_rtmidi_MidiOut *)__pyx_v_self), __pyx_v_rtapi, __pyx_v_name);
 
@@ -8955,45 +8962,45 @@
   PyObject *__pyx_t_23 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
   __Pyx_INCREF(__pyx_v_name);
 
-  /* "_rtmidi.pyx":1014
+  /* "_rtmidi.pyx":1019
  * 
  *         """
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidiOut Client"
  * 
  */
   __pyx_t_1 = (__pyx_v_name == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "_rtmidi.pyx":1015
+    /* "_rtmidi.pyx":1020
  *         """
  *         if name is None:
  *             name = "RtMidiOut Client"             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
     __Pyx_INCREF(__pyx_kp_u_RtMidiOut_Client);
     __Pyx_DECREF_SET(__pyx_v_name, __pyx_kp_u_RtMidiOut_Client);
 
-    /* "_rtmidi.pyx":1014
+    /* "_rtmidi.pyx":1019
  * 
  *         """
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidiOut Client"
  * 
  */
   }
 
-  /* "_rtmidi.pyx":1017
+  /* "_rtmidi.pyx":1022
  *             name = "RtMidiOut Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:
  */
   {
@@ -9001,49 +9008,49 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_5);
     /*try:*/ {
 
-      /* "_rtmidi.pyx":1018
+      /* "_rtmidi.pyx":1023
  * 
  *         try:
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))             # <<<<<<<<<<<<<<
  *         except RuntimeError as exc:
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1018, __pyx_L4_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1023, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_name);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1018, __pyx_L4_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1023, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1018, __pyx_L4_error)
+      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1023, __pyx_L4_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       try {
         __pyx_t_10 = new RtMidiOut(__pyx_v_rtapi, __pyx_t_9);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 1018, __pyx_L4_error)
+        __PYX_ERR(0, 1023, __pyx_L4_error)
       }
       __pyx_v_self->thisptr = __pyx_t_10;
 
-      /* "_rtmidi.pyx":1017
+      /* "_rtmidi.pyx":1022
  *             name = "RtMidiOut Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:
  */
     }
@@ -9052,65 +9059,65 @@
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L9_try_end;
     __pyx_L4_error:;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "_rtmidi.pyx":1019
+    /* "_rtmidi.pyx":1024
  *         try:
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:             # <<<<<<<<<<<<<<
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  */
     __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_RuntimeError);
     if (__pyx_t_11) {
       __Pyx_AddTraceback("_rtmidi.MidiOut.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 1019, __pyx_L6_except_error)
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 1024, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __pyx_v_exc = __pyx_t_7;
       /*try:*/ {
 
-        /* "_rtmidi.pyx":1020
+        /* "_rtmidi.pyx":1025
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  * 
  *         self.set_error_callback(_default_error_handler)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1020, __pyx_L15_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1025, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_exc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1020, __pyx_L15_error)
+        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_exc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1025, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1020, __pyx_L15_error)
+        __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1025, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_GIVEREF(__pyx_t_13);
         PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13);
         __pyx_t_13 = 0;
-        __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1020, __pyx_L15_error)
+        __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1025, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_15 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 1020, __pyx_L15_error)
+        __pyx_t_15 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 1025, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_15);
-        if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_type, __pyx_t_15) < 0) __PYX_ERR(0, 1020, __pyx_L15_error)
+        if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_type, __pyx_t_15) < 0) __PYX_ERR(0, 1025, __pyx_L15_error)
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 1020, __pyx_L15_error)
+        __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 1025, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_Raise(__pyx_t_15, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __PYX_ERR(0, 1020, __pyx_L15_error)
+        __PYX_ERR(0, 1025, __pyx_L15_error)
       }
 
-      /* "_rtmidi.pyx":1019
+      /* "_rtmidi.pyx":1024
  *         try:
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:             # <<<<<<<<<<<<<<
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  */
       /*finally:*/ {
@@ -9151,85 +9158,85 @@
           goto __pyx_L6_except_error;
         }
       }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
-    /* "_rtmidi.pyx":1017
+    /* "_rtmidi.pyx":1022
  *             name = "RtMidiOut Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:
  */
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     goto __pyx_L1_error;
     __pyx_L9_try_end:;
   }
 
-  /* "_rtmidi.pyx":1022
+  /* "_rtmidi.pyx":1027
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  *         self.set_error_callback(_default_error_handler)             # <<<<<<<<<<<<<<
  *         self._port = None
  *         self._deleted = False
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1022, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1027, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1022, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1027, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_8 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_15, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1022, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1027, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "_rtmidi.pyx":1023
+  /* "_rtmidi.pyx":1028
  * 
  *         self.set_error_callback(_default_error_handler)
  *         self._port = None             # <<<<<<<<<<<<<<
  *         self._deleted = False
  * 
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base._port);
   __Pyx_DECREF(__pyx_v_self->__pyx_base._port);
   __pyx_v_self->__pyx_base._port = Py_None;
 
-  /* "_rtmidi.pyx":1024
+  /* "_rtmidi.pyx":1029
  *         self.set_error_callback(_default_error_handler)
  *         self._port = None
  *         self._deleted = False             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base._deleted);
   __Pyx_DECREF(__pyx_v_self->__pyx_base._deleted);
   __pyx_v_self->__pyx_base._deleted = Py_False;
 
-  /* "_rtmidi.pyx":1008
+  /* "_rtmidi.pyx":1013
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None):             # <<<<<<<<<<<<<<
  *         """Create a new client instance for MIDI output.
  * 
  */
 
@@ -9249,15 +9256,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_exc);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":1026
+/* "_rtmidi.pyx":1031
  *         self._deleted = False
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  */
 
@@ -9277,44 +9284,44 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "_rtmidi.pyx":1028
+  /* "_rtmidi.pyx":1033
  *     def __dealloc__(self):
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):             # <<<<<<<<<<<<<<
  *             del self.thisptr
  * 
  */
-  __pyx_t_1 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_thisptr); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1028, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_thisptr); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1033, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "_rtmidi.pyx":1029
+    /* "_rtmidi.pyx":1034
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  *             del self.thisptr             # <<<<<<<<<<<<<<
  * 
  *     def delete(self):
  */
     delete __pyx_v_self->thisptr;
 
-    /* "_rtmidi.pyx":1028
+    /* "_rtmidi.pyx":1033
  *     def __dealloc__(self):
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):             # <<<<<<<<<<<<<<
  *             del self.thisptr
  * 
  */
   }
 
-  /* "_rtmidi.pyx":1026
+  /* "_rtmidi.pyx":1031
  *         self._deleted = False
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  */
 
@@ -9322,15 +9329,15 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("_rtmidi.MidiOut.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "_rtmidi.pyx":1031
+/* "_rtmidi.pyx":1036
  *             del self.thisptr
  * 
  *     def delete(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance.
  * 
  */
 
@@ -9354,57 +9361,57 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("delete", 0);
 
-  /* "_rtmidi.pyx":1048
+  /* "_rtmidi.pyx":1053
  * 
  *         """
  *         if not self._deleted:             # <<<<<<<<<<<<<<
  *             del self.thisptr
  *             self._deleted = True
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->__pyx_base._deleted); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1048, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->__pyx_base._deleted); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1053, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (__pyx_t_2) {
 
-    /* "_rtmidi.pyx":1049
+    /* "_rtmidi.pyx":1054
  *         """
  *         if not self._deleted:
  *             del self.thisptr             # <<<<<<<<<<<<<<
  *             self._deleted = True
  * 
  */
     delete __pyx_v_self->thisptr;
 
-    /* "_rtmidi.pyx":1050
+    /* "_rtmidi.pyx":1055
  *         if not self._deleted:
  *             del self.thisptr
  *             self._deleted = True             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
     __Pyx_INCREF(Py_True);
     __Pyx_GIVEREF(Py_True);
     __Pyx_GOTREF(__pyx_v_self->__pyx_base._deleted);
     __Pyx_DECREF(__pyx_v_self->__pyx_base._deleted);
     __pyx_v_self->__pyx_base._deleted = Py_True;
 
-    /* "_rtmidi.pyx":1048
+    /* "_rtmidi.pyx":1053
  * 
  *         """
  *         if not self._deleted:             # <<<<<<<<<<<<<<
  *             del self.thisptr
  *             self._deleted = True
  */
   }
 
-  /* "_rtmidi.pyx":1031
+  /* "_rtmidi.pyx":1036
  *             del self.thisptr
  * 
  *     def delete(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance.
  * 
  */
 
@@ -9416,15 +9423,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":1053
+/* "_rtmidi.pyx":1058
  * 
  *     @property
  *     def is_deleted(self):             # <<<<<<<<<<<<<<
  *         return self._deleted
  * 
  */
 
@@ -9442,42 +9449,42 @@
 }
 
 static PyObject *__pyx_pf_7_rtmidi_7MidiOut_10is_deleted___get__(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "_rtmidi.pyx":1054
+  /* "_rtmidi.pyx":1059
  *     @property
  *     def is_deleted(self):
  *         return self._deleted             # <<<<<<<<<<<<<<
  * 
  *     def get_current_api(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->__pyx_base._deleted);
   __pyx_r = __pyx_v_self->__pyx_base._deleted;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":1053
+  /* "_rtmidi.pyx":1058
  * 
  *     @property
  *     def is_deleted(self):             # <<<<<<<<<<<<<<
  *         return self._deleted
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":1056
+/* "_rtmidi.pyx":1061
  *         return self._deleted
  * 
  *     def get_current_api(self):             # <<<<<<<<<<<<<<
  *         """Return the low-level MIDI backend API used by this instance.
  * 
  */
 
@@ -9500,29 +9507,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_current_api", 0);
 
-  /* "_rtmidi.pyx":1068
+  /* "_rtmidi.pyx":1073
  * 
  *         """
  *         return self.thisptr.getCurrentApi()             # <<<<<<<<<<<<<<
  * 
  *     def send_message(self, message):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(__pyx_v_self->thisptr->getCurrentApi()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1068, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(__pyx_v_self->thisptr->getCurrentApi()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1073, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "_rtmidi.pyx":1056
+  /* "_rtmidi.pyx":1061
  *         return self._deleted
  * 
  *     def get_current_api(self):             # <<<<<<<<<<<<<<
  *         """Return the low-level MIDI backend API used by this instance.
  * 
  */
 
@@ -9533,15 +9540,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "_rtmidi.pyx":1070
+/* "_rtmidi.pyx":1075
  *         return self.thisptr.getCurrentApi()
  * 
  *     def send_message(self, message):             # <<<<<<<<<<<<<<
  *         """Send a MIDI message to the output port.
  * 
  */
 
@@ -9572,191 +9579,191 @@
   PyObject *(*__pyx_t_6)(PyObject *);
   unsigned char __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("send_message", 0);
 
-  /* "_rtmidi.pyx":1098
+  /* "_rtmidi.pyx":1103
  *         cdef vector[unsigned char] msg_v
  * 
  *         if not message:             # <<<<<<<<<<<<<<
  *             raise ValueError("'message' must not be empty.")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_message); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1098, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_message); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1103, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "_rtmidi.pyx":1099
+    /* "_rtmidi.pyx":1104
  * 
  *         if not message:
  *             raise ValueError("'message' must not be empty.")             # <<<<<<<<<<<<<<
  * 
  *         if len(message) > 3 and message[0] != 0xF0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1099, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 1099, __pyx_L1_error)
+    __PYX_ERR(0, 1104, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":1098
+    /* "_rtmidi.pyx":1103
  *         cdef vector[unsigned char] msg_v
  * 
  *         if not message:             # <<<<<<<<<<<<<<
  *             raise ValueError("'message' must not be empty.")
  * 
  */
   }
 
-  /* "_rtmidi.pyx":1101
+  /* "_rtmidi.pyx":1106
  *             raise ValueError("'message' must not be empty.")
  * 
  *         if len(message) > 3 and message[0] != 0xF0:             # <<<<<<<<<<<<<<
  *             raise ValueError("'message' longer than 3 bytes but does not "
  *                              "start with 0xF0.")
  */
-  __pyx_t_4 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1101, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1106, __pyx_L1_error)
   __pyx_t_1 = ((__pyx_t_4 > 3) != 0);
   if (__pyx_t_1) {
   } else {
     __pyx_t_2 = __pyx_t_1;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_message, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1101, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_message, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_NeObjC(__pyx_t_3, __pyx_int_240, 0xF0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1101, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_NeObjC(__pyx_t_3, __pyx_int_240, 0xF0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1101, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1106, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_2 = __pyx_t_1;
   __pyx_L5_bool_binop_done:;
   if (unlikely(__pyx_t_2)) {
 
-    /* "_rtmidi.pyx":1102
+    /* "_rtmidi.pyx":1107
  * 
  *         if len(message) > 3 and message[0] != 0xF0:
  *             raise ValueError("'message' longer than 3 bytes but does not "             # <<<<<<<<<<<<<<
  *                              "start with 0xF0.")
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1102, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1107, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 1102, __pyx_L1_error)
+    __PYX_ERR(0, 1107, __pyx_L1_error)
 
-    /* "_rtmidi.pyx":1101
+    /* "_rtmidi.pyx":1106
  *             raise ValueError("'message' must not be empty.")
  * 
  *         if len(message) > 3 and message[0] != 0xF0:             # <<<<<<<<<<<<<<
  *             raise ValueError("'message' longer than 3 bytes but does not "
  *                              "start with 0xF0.")
  */
   }
 
-  /* "_rtmidi.pyx":1105
+  /* "_rtmidi.pyx":1110
  *                              "start with 0xF0.")
  * 
  *         for c in message:             # <<<<<<<<<<<<<<
  *             msg_v.push_back(c)
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_message)) || PyTuple_CheckExact(__pyx_v_message)) {
     __pyx_t_5 = __pyx_v_message; __Pyx_INCREF(__pyx_t_5); __pyx_t_4 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1105, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1105, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1110, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1105, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1110, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1105, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1110, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1105, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1110, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1105, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1110, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_6(__pyx_t_5);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 1105, __pyx_L1_error)
+          else __PYX_ERR(0, 1110, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_c, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "_rtmidi.pyx":1106
+    /* "_rtmidi.pyx":1111
  * 
  *         for c in message:
  *             msg_v.push_back(c)             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-    __pyx_t_7 = __Pyx_PyInt_As_unsigned_char(__pyx_v_c); if (unlikely((__pyx_t_7 == (unsigned char)-1) && PyErr_Occurred())) __PYX_ERR(0, 1106, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_As_unsigned_char(__pyx_v_c); if (unlikely((__pyx_t_7 == (unsigned char)-1) && PyErr_Occurred())) __PYX_ERR(0, 1111, __pyx_L1_error)
     try {
       __pyx_v_msg_v.push_back(__pyx_t_7);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 1106, __pyx_L1_error)
+      __PYX_ERR(0, 1111, __pyx_L1_error)
     }
 
-    /* "_rtmidi.pyx":1105
+    /* "_rtmidi.pyx":1110
  *                              "start with 0xF0.")
  * 
  *         for c in message:             # <<<<<<<<<<<<<<
  *             msg_v.push_back(c)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "_rtmidi.pyx":1108
+  /* "_rtmidi.pyx":1113
  *             msg_v.push_back(c)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             self.thisptr.sendMessage(&msg_v)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "_rtmidi.pyx":1109
+        /* "_rtmidi.pyx":1114
  * 
  *         with nogil:
  *             self.thisptr.sendMessage(&msg_v)             # <<<<<<<<<<<<<<
  */
-        __pyx_v_self->thisptr->sendMessage((&__pyx_v_msg_v)); if (unlikely(__Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 1109, __pyx_L10_error)
+        __pyx_v_self->thisptr->sendMessage((&__pyx_v_msg_v)); if (unlikely(__Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 1114, __pyx_L10_error)
       }
 
-      /* "_rtmidi.pyx":1108
+      /* "_rtmidi.pyx":1113
  *             msg_v.push_back(c)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             self.thisptr.sendMessage(&msg_v)
  */
       /*finally:*/ {
         /*normal exit:*/{
@@ -9773,15 +9780,15 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L11:;
       }
   }
 
-  /* "_rtmidi.pyx":1070
+  /* "_rtmidi.pyx":1075
  *         return self.thisptr.getCurrentApi()
  * 
  *     def send_message(self, message):             # <<<<<<<<<<<<<<
  *         """Send a MIDI message to the output port.
  * 
  */
 
@@ -10799,15 +10806,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7_rtmidi_MidiIn __pyx_vtable_7_rtmidi_MidiIn;
 
 static PyObject *__pyx_tp_new_7_rtmidi_MidiIn(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7_rtmidi_MidiIn *p;
@@ -10949,15 +10956,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7_rtmidi_MidiOut __pyx_vtable_7_rtmidi_MidiOut;
 
 static PyObject *__pyx_tp_new_7_rtmidi_MidiOut(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7_rtmidi_MidiOut *p;
@@ -11072,15 +11079,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -11133,14 +11140,16 @@
   {&__pyx_n_u_API_MACOSX_CORE, __pyx_k_API_MACOSX_CORE, sizeof(__pyx_k_API_MACOSX_CORE), 0, 1, 0, 1},
   {&__pyx_n_s_API_RTMIDI_DUMMY, __pyx_k_API_RTMIDI_DUMMY, sizeof(__pyx_k_API_RTMIDI_DUMMY), 0, 0, 1, 1},
   {&__pyx_n_u_API_RTMIDI_DUMMY, __pyx_k_API_RTMIDI_DUMMY, sizeof(__pyx_k_API_RTMIDI_DUMMY), 0, 1, 0, 1},
   {&__pyx_n_s_API_UNIX_JACK, __pyx_k_API_UNIX_JACK, sizeof(__pyx_k_API_UNIX_JACK), 0, 0, 1, 1},
   {&__pyx_n_u_API_UNIX_JACK, __pyx_k_API_UNIX_JACK, sizeof(__pyx_k_API_UNIX_JACK), 0, 1, 0, 1},
   {&__pyx_n_s_API_UNSPECIFIED, __pyx_k_API_UNSPECIFIED, sizeof(__pyx_k_API_UNSPECIFIED), 0, 0, 1, 1},
   {&__pyx_n_u_API_UNSPECIFIED, __pyx_k_API_UNSPECIFIED, sizeof(__pyx_k_API_UNSPECIFIED), 0, 1, 0, 1},
+  {&__pyx_n_s_API_WEB_MIDI, __pyx_k_API_WEB_MIDI, sizeof(__pyx_k_API_WEB_MIDI), 0, 0, 1, 1},
+  {&__pyx_n_u_API_WEB_MIDI, __pyx_k_API_WEB_MIDI, sizeof(__pyx_k_API_WEB_MIDI), 0, 1, 0, 1},
   {&__pyx_n_s_API_WINDOWS_MM, __pyx_k_API_WINDOWS_MM, sizeof(__pyx_k_API_WINDOWS_MM), 0, 0, 1, 1},
   {&__pyx_n_u_API_WINDOWS_MM, __pyx_k_API_WINDOWS_MM, sizeof(__pyx_k_API_WINDOWS_MM), 0, 1, 0, 1},
   {&__pyx_kp_u_API_backend_does_not_support_cha, __pyx_k_API_backend_does_not_support_cha, sizeof(__pyx_k_API_backend_does_not_support_cha), 0, 1, 0, 0},
   {&__pyx_kp_u_API_backend_does_not_support_cha_2, __pyx_k_API_backend_does_not_support_cha_2, sizeof(__pyx_k_API_backend_does_not_support_cha_2), 0, 1, 0, 0},
   {&__pyx_kp_s_Base_general_RtMidi_exception_Al, __pyx_k_Base_general_RtMidi_exception_Al, sizeof(__pyx_k_Base_general_RtMidi_exception_Al), 0, 0, 1, 0},
   {&__pyx_n_s_ERRORTYPE_DEBUG_WARNING, __pyx_k_ERRORTYPE_DEBUG_WARNING, sizeof(__pyx_k_ERRORTYPE_DEBUG_WARNING), 0, 0, 1, 1},
   {&__pyx_n_u_ERRORTYPE_DEBUG_WARNING, __pyx_k_ERRORTYPE_DEBUG_WARNING, sizeof(__pyx_k_ERRORTYPE_DEBUG_WARNING), 0, 1, 0, 1},
@@ -11310,61 +11319,61 @@
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
   {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
   {&__pyx_n_u_win, __pyx_k_win, sizeof(__pyx_k_win), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 281, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 290, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 299, __pyx_L1_error)
-  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(0, 308, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 211, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 228, __pyx_L1_error)
-  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 277, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 641, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(0, 313, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 646, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "_rtmidi.pyx":232
+  /* "_rtmidi.pyx":236
  * 
  *     if not isinstance(name, bytes):
  *         raise TypeError("name must be bytes or (unicode) string.")             # <<<<<<<<<<<<<<
  * 
  *     return name
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_name_must_be_bytes_or_unicode_st); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_name_must_be_bytes_or_unicode_st); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "_rtmidi.pyx":641
+  /* "_rtmidi.pyx":646
  *         """
  *         if self.get_current_api() == API_WINDOWS_MM:
  *             raise NotImplementedError("Virtual ports are not supported "             # <<<<<<<<<<<<<<
  *                                       "by the Windows MultiMedia API.")
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Virtual_ports_are_not_supported); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Virtual_ports_are_not_supported); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "_rtmidi.pyx":685
+  /* "_rtmidi.pyx":690
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_UNIX_JACK, API_WINDOWS_MM):
  *             raise NotImplementedError(             # <<<<<<<<<<<<<<
  *                 "API backend does not support changing the client name.")
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_API_backend_does_not_support_cha); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_API_backend_does_not_support_cha); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 690, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -11379,33 +11388,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "_rtmidi.pyx":1099
+  /* "_rtmidi.pyx":1104
  * 
  *         if not message:
  *             raise ValueError("'message' must not be empty.")             # <<<<<<<<<<<<<<
  * 
  *         if len(message) > 3 and message[0] != 0xF0:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_message_must_not_be_empty); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 1099, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_message_must_not_be_empty); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 1104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "_rtmidi.pyx":1102
+  /* "_rtmidi.pyx":1107
  * 
  *         if len(message) > 3 and message[0] != 0xF0:
  *             raise ValueError("'message' longer than 3 bytes but does not "             # <<<<<<<<<<<<<<
  *                              "start with 0xF0.")
  * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_message_longer_than_3_bytes_but); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 1102, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_message_longer_than_3_bytes_but); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 1107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -11423,120 +11432,120 @@
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
   __pyx_tuple__12 = PyTuple_Pack(3, __pyx_int_152509455, __pyx_int_34815411, __pyx_int_2218169); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "_rtmidi.pyx":115
+  /* "_rtmidi.pyx":118
  * 
  * __all__ = (
  *     'API_UNSPECIFIED', 'API_MACOSX_CORE', 'API_LINUX_ALSA', 'API_UNIX_JACK',             # <<<<<<<<<<<<<<
- *     'API_WINDOWS_MM', 'API_RTMIDI_DUMMY', 'ERRORTYPE_DEBUG_WARNING',
+ *     'API_WINDOWS_MM', 'API_RTMIDI_DUMMY', 'API_WEB_MIDI', 'ERRORTYPE_DEBUG_WARNING',
  *     'ERRORTYPE_DRIVER_ERROR', 'ERRORTYPE_INVALID_DEVICE',
  */
-  __pyx_tuple__13 = PyTuple_Pack(31, __pyx_n_u_API_UNSPECIFIED, __pyx_n_u_API_MACOSX_CORE, __pyx_n_u_API_LINUX_ALSA, __pyx_n_u_API_UNIX_JACK, __pyx_n_u_API_WINDOWS_MM, __pyx_n_u_API_RTMIDI_DUMMY, __pyx_n_u_ERRORTYPE_DEBUG_WARNING, __pyx_n_u_ERRORTYPE_DRIVER_ERROR, __pyx_n_u_ERRORTYPE_INVALID_DEVICE, __pyx_n_u_ERRORTYPE_INVALID_PARAMETER, __pyx_n_u_ERRORTYPE_INVALID_USE, __pyx_n_u_ERRORTYPE_MEMORY_ERROR, __pyx_n_u_ERRORTYPE_NO_DEVICES_FOUND, __pyx_n_u_ERRORTYPE_SYSTEM_ERROR, __pyx_n_u_ERRORTYPE_THREAD_ERROR, __pyx_n_u_ERRORTYPE_UNSPECIFIED, __pyx_n_u_ERRORTYPE_WARNING, __pyx_n_u_InvalidPortError, __pyx_n_u_InvalidUseError, __pyx_n_u_MemoryAllocationError, __pyx_n_u_MidiIn, __pyx_n_u_MidiOut, __pyx_n_u_NoDevicesError, __pyx_n_u_RtMidiError, __pyx_n_u_SystemError, __pyx_n_u_UnsupportedOperationError, __pyx_n_u_get_api_display_name, __pyx_n_u_get_api_name, __pyx_n_u_get_compiled_api, __pyx_n_u_get_compiled_api_by_name, __pyx_n_u_get_rtmidi_version); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(32, __pyx_n_u_API_UNSPECIFIED, __pyx_n_u_API_MACOSX_CORE, __pyx_n_u_API_LINUX_ALSA, __pyx_n_u_API_UNIX_JACK, __pyx_n_u_API_WINDOWS_MM, __pyx_n_u_API_RTMIDI_DUMMY, __pyx_n_u_API_WEB_MIDI, __pyx_n_u_ERRORTYPE_DEBUG_WARNING, __pyx_n_u_ERRORTYPE_DRIVER_ERROR, __pyx_n_u_ERRORTYPE_INVALID_DEVICE, __pyx_n_u_ERRORTYPE_INVALID_PARAMETER, __pyx_n_u_ERRORTYPE_INVALID_USE, __pyx_n_u_ERRORTYPE_MEMORY_ERROR, __pyx_n_u_ERRORTYPE_NO_DEVICES_FOUND, __pyx_n_u_ERRORTYPE_SYSTEM_ERROR, __pyx_n_u_ERRORTYPE_THREAD_ERROR, __pyx_n_u_ERRORTYPE_UNSPECIFIED, __pyx_n_u_ERRORTYPE_WARNING, __pyx_n_u_InvalidPortError, __pyx_n_u_InvalidUseError, __pyx_n_u_MemoryAllocationError, __pyx_n_u_MidiIn, __pyx_n_u_MidiOut, __pyx_n_u_NoDevicesError, __pyx_n_u_RtMidiError, __pyx_n_u_SystemError, __pyx_n_u_UnsupportedOperationError, __pyx_n_u_get_api_display_name, __pyx_n_u_get_api_name, __pyx_n_u_get_compiled_api, __pyx_n_u_get_compiled_api_by_name, __pyx_n_u_get_rtmidi_version); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 118, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "_rtmidi.pyx":222
+  /* "_rtmidi.pyx":226
  * 
  * 
  * def _to_bytes(name):             # <<<<<<<<<<<<<<
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_n_s_name); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_n_s_name); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_to_bytes, 222, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_to_bytes, 226, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 226, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":276
+  /* "_rtmidi.pyx":281
  *     type = ERR_UNSPECIFIED
  * 
  *     def __init__(self, msg, type=None):             # <<<<<<<<<<<<<<
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type
  */
-  __pyx_tuple__16 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_type); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_type); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_init, 276, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 276, __pyx_L1_error)
-  __pyx_tuple__18 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_init, 281, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "_rtmidi.pyx":337
+  /* "_rtmidi.pyx":342
  * # wrappers for RtMidi's static methods and classes
  * 
  * def get_api_display_name(api):             # <<<<<<<<<<<<<<
  *     """Return the display name of a specified MIDI API.
  * 
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_api); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_api); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_api_display_name, 337, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_api_display_name, 342, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 342, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":353
+  /* "_rtmidi.pyx":358
  * 
  * 
  * def get_api_name(api):             # <<<<<<<<<<<<<<
  *     """Return the name of a specified MIDI API.
  * 
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_n_s_api); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_n_s_api); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_api_name, 353, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_api_name, 358, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 358, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":369
+  /* "_rtmidi.pyx":374
  * 
  * 
  * def get_compiled_api():             # <<<<<<<<<<<<<<
  *     """Return a list of low-level MIDI backend APIs this module supports.
  * 
  */
-  __pyx_tuple__23 = PyTuple_Pack(2, __pyx_n_s_api_v, __pyx_n_s_i); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(2, __pyx_n_s_api_v, __pyx_n_s_i); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_GIVEREF(__pyx_tuple__23);
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_compiled_api, 369, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_compiled_api, 374, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 374, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":385
+  /* "_rtmidi.pyx":390
  * 
  * 
  * def get_compiled_api_by_name(name):             # <<<<<<<<<<<<<<
  *     """Return the compiled MIDI API having the given name.
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_n_s_name); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_n_s_name); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 390, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_compiled_api_by_name, 385, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_compiled_api_by_name, 390, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 390, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":396
+  /* "_rtmidi.pyx":401
  * 
  * 
  * def get_rtmidi_version():             # <<<<<<<<<<<<<<
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')
  */
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_rtmidi_version, 396, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_rtmidi_version, 401, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 401, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":401
+  /* "_rtmidi.pyx":406
  * 
  * 
  * def _default_error_handler(etype, msg, data=None):             # <<<<<<<<<<<<<<
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  */
-  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_etype, __pyx_n_s_msg, __pyx_n_s_data); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_etype, __pyx_n_s_msg, __pyx_n_s_data); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_default_error_handler, 401, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_default_error_handler, 406, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 406, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_MidiBase(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
   __pyx_tuple__30 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -11599,54 +11608,54 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_7_rtmidi_MidiBase = &__pyx_vtable_7_rtmidi_MidiBase;
   __pyx_vtable_7_rtmidi_MidiBase.baseptr = (RtMidi *(*)(struct __pyx_obj_7_rtmidi_MidiBase *))__pyx_f_7_rtmidi_8MidiBase_baseptr;
-  if (PyType_Ready(&__pyx_type_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 435, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7_rtmidi_MidiBase.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7_rtmidi_MidiBase.tp_dictoffset && __pyx_type_7_rtmidi_MidiBase.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7_rtmidi_MidiBase.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_7_rtmidi_MidiBase.tp_dict, __pyx_vtabptr_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiBase, (PyObject *)&__pyx_type_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7_rtmidi_MidiBase.tp_dict, __pyx_vtabptr_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 435, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiBase, (PyObject *)&__pyx_type_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 435, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 435, __pyx_L1_error)
   __pyx_ptype_7_rtmidi_MidiBase = &__pyx_type_7_rtmidi_MidiBase;
   __pyx_vtabptr_7_rtmidi_MidiIn = &__pyx_vtable_7_rtmidi_MidiIn;
   __pyx_vtable_7_rtmidi_MidiIn.__pyx_base = *__pyx_vtabptr_7_rtmidi_MidiBase;
   __pyx_vtable_7_rtmidi_MidiIn.__pyx_base.baseptr = (RtMidi *(*)(struct __pyx_obj_7_rtmidi_MidiBase *))__pyx_f_7_rtmidi_6MidiIn_baseptr;
   __pyx_type_7_rtmidi_MidiIn.tp_base = __pyx_ptype_7_rtmidi_MidiBase;
-  if (PyType_Ready(&__pyx_type_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7_rtmidi_MidiIn.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7_rtmidi_MidiIn.tp_dictoffset && __pyx_type_7_rtmidi_MidiIn.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7_rtmidi_MidiIn.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_7_rtmidi_MidiIn.tp_dict, __pyx_vtabptr_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiIn, (PyObject *)&__pyx_type_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7_rtmidi_MidiIn.tp_dict, __pyx_vtabptr_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiIn, (PyObject *)&__pyx_type_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
   __pyx_ptype_7_rtmidi_MidiIn = &__pyx_type_7_rtmidi_MidiIn;
   __pyx_vtabptr_7_rtmidi_MidiOut = &__pyx_vtable_7_rtmidi_MidiOut;
   __pyx_vtable_7_rtmidi_MidiOut.__pyx_base = *__pyx_vtabptr_7_rtmidi_MidiBase;
   __pyx_vtable_7_rtmidi_MidiOut.__pyx_base.baseptr = (RtMidi *(*)(struct __pyx_obj_7_rtmidi_MidiBase *))__pyx_f_7_rtmidi_7MidiOut_baseptr;
   __pyx_type_7_rtmidi_MidiOut.tp_base = __pyx_ptype_7_rtmidi_MidiBase;
-  if (PyType_Ready(&__pyx_type_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 973, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_7_rtmidi_MidiOut.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7_rtmidi_MidiOut.tp_dictoffset && __pyx_type_7_rtmidi_MidiOut.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_7_rtmidi_MidiOut.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_7_rtmidi_MidiOut.tp_dict, __pyx_vtabptr_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiOut, (PyObject *)&__pyx_type_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7_rtmidi_MidiOut.tp_dict, __pyx_vtabptr_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 973, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiOut, (PyObject *)&__pyx_type_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 973, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 973, __pyx_L1_error)
   __pyx_ptype_7_rtmidi_MidiOut = &__pyx_type_7_rtmidi_MidiOut;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -11877,748 +11886,760 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "_rtmidi.pyx":106
+  /* "_rtmidi.pyx":109
  * """
  * 
  * import sys             # <<<<<<<<<<<<<<
  * import warnings
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_sys, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_sys, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sys, __pyx_t_1) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sys, __pyx_t_1) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":107
+  /* "_rtmidi.pyx":110
  * 
  * import sys
  * import warnings             # <<<<<<<<<<<<<<
  * 
  * from libcpp cimport bool
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_1) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_1) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":115
+  /* "_rtmidi.pyx":118
  * 
  * __all__ = (
  *     'API_UNSPECIFIED', 'API_MACOSX_CORE', 'API_LINUX_ALSA', 'API_UNIX_JACK',             # <<<<<<<<<<<<<<
- *     'API_WINDOWS_MM', 'API_RTMIDI_DUMMY', 'ERRORTYPE_DEBUG_WARNING',
+ *     'API_WINDOWS_MM', 'API_RTMIDI_DUMMY', 'API_WEB_MIDI', 'ERRORTYPE_DEBUG_WARNING',
  *     'ERRORTYPE_DRIVER_ERROR', 'ERRORTYPE_INVALID_DEVICE',
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_tuple__13) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_tuple__13) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
 
-  /* "_rtmidi.pyx":128
+  /* "_rtmidi.pyx":131
  * )
  * 
  * if bytes is str:             # <<<<<<<<<<<<<<
  *     string_types = (str, unicode)
  * else:
  */
   __pyx_t_2 = ((&PyBytes_Type) == (&PyUnicode_Type));
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "_rtmidi.pyx":129
+    /* "_rtmidi.pyx":132
  * 
  * if bytes is str:
  *     string_types = (str, unicode)             # <<<<<<<<<<<<<<
  * else:
  *     string_types = (str,)
  */
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)(&PyUnicode_Type)));
     __Pyx_GIVEREF(((PyObject *)(&PyUnicode_Type)));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&PyUnicode_Type)));
     __Pyx_INCREF(((PyObject *)(&PyUnicode_Type)));
     __Pyx_GIVEREF(((PyObject *)(&PyUnicode_Type)));
     PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)(&PyUnicode_Type)));
-    if (PyDict_SetItem(__pyx_d, __pyx_n_s_string_types, __pyx_t_1) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_d, __pyx_n_s_string_types, __pyx_t_1) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "_rtmidi.pyx":128
+    /* "_rtmidi.pyx":131
  * )
  * 
  * if bytes is str:             # <<<<<<<<<<<<<<
  *     string_types = (str, unicode)
  * else:
  */
     goto __pyx_L2;
   }
 
-  /* "_rtmidi.pyx":131
+  /* "_rtmidi.pyx":134
  *     string_types = (str, unicode)
  * else:
  *     string_types = (str,)             # <<<<<<<<<<<<<<
  * 
  * cdef extern from "Python.h":
  */
   /*else*/ {
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)(&PyUnicode_Type)));
     __Pyx_GIVEREF(((PyObject *)(&PyUnicode_Type)));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&PyUnicode_Type)));
-    if (PyDict_SetItem(__pyx_d, __pyx_n_s_string_types, __pyx_t_1) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_d, __pyx_n_s_string_types, __pyx_t_1) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L2:;
 
-  /* "_rtmidi.pyx":136
+  /* "_rtmidi.pyx":139
  *     void Py_Initialize()
  * 
  * Py_Initialize()             # <<<<<<<<<<<<<<
  * 
  * # Declarations for RtMidi C++ classes and their methods we use
  */
   Py_Initialize();
 
-  /* "_rtmidi.pyx":222
+  /* "_rtmidi.pyx":226
  * 
  * 
  * def _to_bytes(name):             # <<<<<<<<<<<<<<
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_1_to_bytes, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_1_to_bytes, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_bytes, __pyx_t_1) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_bytes, __pyx_t_1) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":241
+  /* "_rtmidi.pyx":245
  * # export Api enum values to Python
  * 
  * API_UNSPECIFIED = UNSPECIFIED             # <<<<<<<<<<<<<<
  * API_MACOSX_CORE = MACOSX_CORE
  * API_LINUX_ALSA = LINUX_ALSA
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::UNSPECIFIED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::UNSPECIFIED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_UNSPECIFIED, __pyx_t_1) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_UNSPECIFIED, __pyx_t_1) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":242
+  /* "_rtmidi.pyx":246
  * 
  * API_UNSPECIFIED = UNSPECIFIED
  * API_MACOSX_CORE = MACOSX_CORE             # <<<<<<<<<<<<<<
  * API_LINUX_ALSA = LINUX_ALSA
  * API_UNIX_JACK = UNIX_JACK
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::MACOSX_CORE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::MACOSX_CORE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_MACOSX_CORE, __pyx_t_1) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_MACOSX_CORE, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":243
+  /* "_rtmidi.pyx":247
  * API_UNSPECIFIED = UNSPECIFIED
  * API_MACOSX_CORE = MACOSX_CORE
  * API_LINUX_ALSA = LINUX_ALSA             # <<<<<<<<<<<<<<
  * API_UNIX_JACK = UNIX_JACK
  * API_WINDOWS_MM = WINDOWS_MM
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::LINUX_ALSA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::LINUX_ALSA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_LINUX_ALSA, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_LINUX_ALSA, __pyx_t_1) < 0) __PYX_ERR(0, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":244
+  /* "_rtmidi.pyx":248
  * API_MACOSX_CORE = MACOSX_CORE
  * API_LINUX_ALSA = LINUX_ALSA
  * API_UNIX_JACK = UNIX_JACK             # <<<<<<<<<<<<<<
  * API_WINDOWS_MM = WINDOWS_MM
  * API_RTMIDI_DUMMY = RTMIDI_DUMMY
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::UNIX_JACK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::UNIX_JACK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_UNIX_JACK, __pyx_t_1) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_UNIX_JACK, __pyx_t_1) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":245
+  /* "_rtmidi.pyx":249
  * API_LINUX_ALSA = LINUX_ALSA
  * API_UNIX_JACK = UNIX_JACK
  * API_WINDOWS_MM = WINDOWS_MM             # <<<<<<<<<<<<<<
  * API_RTMIDI_DUMMY = RTMIDI_DUMMY
- * 
+ * API_WEB_MIDI = WEB_MIDI
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::WINDOWS_MM); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::WINDOWS_MM); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_WINDOWS_MM, __pyx_t_1) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_WINDOWS_MM, __pyx_t_1) < 0) __PYX_ERR(0, 249, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":246
+  /* "_rtmidi.pyx":250
  * API_UNIX_JACK = UNIX_JACK
  * API_WINDOWS_MM = WINDOWS_MM
  * API_RTMIDI_DUMMY = RTMIDI_DUMMY             # <<<<<<<<<<<<<<
+ * API_WEB_MIDI = WEB_MIDI
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::RTMIDI_DUMMY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_RTMIDI_DUMMY, __pyx_t_1) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "_rtmidi.pyx":251
+ * API_WINDOWS_MM = WINDOWS_MM
+ * API_RTMIDI_DUMMY = RTMIDI_DUMMY
+ * API_WEB_MIDI = WEB_MIDI             # <<<<<<<<<<<<<<
  * 
  * # export error values to Python
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::RTMIDI_DUMMY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::WEB_MIDI_API); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_RTMIDI_DUMMY, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_WEB_MIDI, __pyx_t_1) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":250
+  /* "_rtmidi.pyx":255
  * # export error values to Python
  * 
  * ERRORTYPE_WARNING = ERR_WARNING             # <<<<<<<<<<<<<<
  * ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::WARNING); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::WARNING); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_WARNING, __pyx_t_1) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_WARNING, __pyx_t_1) < 0) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":251
+  /* "_rtmidi.pyx":256
  * 
  * ERRORTYPE_WARNING = ERR_WARNING
  * ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING             # <<<<<<<<<<<<<<
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DEBUG_WARNING); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DEBUG_WARNING); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_DEBUG_WARNING, __pyx_t_1) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_DEBUG_WARNING, __pyx_t_1) < 0) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":252
+  /* "_rtmidi.pyx":257
  * ERRORTYPE_WARNING = ERR_WARNING
  * ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED             # <<<<<<<<<<<<<<
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::UNSPECIFIED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::UNSPECIFIED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_UNSPECIFIED, __pyx_t_1) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_UNSPECIFIED, __pyx_t_1) < 0) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":253
+  /* "_rtmidi.pyx":258
  * ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND             # <<<<<<<<<<<<<<
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::NO_DEVICES_FOUND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::NO_DEVICES_FOUND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_NO_DEVICES_FOUND, __pyx_t_1) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_NO_DEVICES_FOUND, __pyx_t_1) < 0) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":254
+  /* "_rtmidi.pyx":259
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE             # <<<<<<<<<<<<<<
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_DEVICE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_DEVICE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_DEVICE, __pyx_t_1) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_DEVICE, __pyx_t_1) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":255
+  /* "_rtmidi.pyx":260
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR             # <<<<<<<<<<<<<<
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_MEMORY_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 255, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_MEMORY_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":256
+  /* "_rtmidi.pyx":261
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER             # <<<<<<<<<<<<<<
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_PARAMETER, __pyx_t_1) < 0) __PYX_ERR(0, 256, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_PARAMETER, __pyx_t_1) < 0) __PYX_ERR(0, 261, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":257
+  /* "_rtmidi.pyx":262
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE             # <<<<<<<<<<<<<<
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR
  * ERRORTYPE_SYSTEM_ERROR = ERR_SYSTEM_ERROR
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_USE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_USE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_USE, __pyx_t_1) < 0) __PYX_ERR(0, 257, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_USE, __pyx_t_1) < 0) __PYX_ERR(0, 262, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":258
+  /* "_rtmidi.pyx":263
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR             # <<<<<<<<<<<<<<
  * ERRORTYPE_SYSTEM_ERROR = ERR_SYSTEM_ERROR
  * ERRORTYPE_THREAD_ERROR = ERR_THREAD_ERROR
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_DRIVER_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 258, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_DRIVER_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 263, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":259
+  /* "_rtmidi.pyx":264
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR
  * ERRORTYPE_SYSTEM_ERROR = ERR_SYSTEM_ERROR             # <<<<<<<<<<<<<<
  * ERRORTYPE_THREAD_ERROR = ERR_THREAD_ERROR
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::SYSTEM_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::SYSTEM_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_SYSTEM_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_SYSTEM_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 264, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":260
+  /* "_rtmidi.pyx":265
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR
  * ERRORTYPE_SYSTEM_ERROR = ERR_SYSTEM_ERROR
  * ERRORTYPE_THREAD_ERROR = ERR_THREAD_ERROR             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::THREAD_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::THREAD_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_THREAD_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 260, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_THREAD_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":265
+  /* "_rtmidi.pyx":270
  * # custom exceptions
  * 
  * class RtMidiError(Exception):             # <<<<<<<<<<<<<<
  *     """Base general RtMidi exception.
  * 
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_RtMidiError, __pyx_n_s_RtMidiError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Base_general_RtMidi_exception_Al); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_RtMidiError, __pyx_n_s_RtMidiError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Base_general_RtMidi_exception_Al); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "_rtmidi.pyx":274
+  /* "_rtmidi.pyx":279
  * 
  *     """
  *     type = ERR_UNSPECIFIED             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, msg, type=None):
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::UNSPECIFIED); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::UNSPECIFIED); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "_rtmidi.pyx":276
+  /* "_rtmidi.pyx":281
  *     type = ERR_UNSPECIFIED
  * 
  *     def __init__(self, msg, type=None):             # <<<<<<<<<<<<<<
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7_rtmidi_11RtMidiError_1__init__, 0, __pyx_n_s_RtMidiError___init, NULL, __pyx_n_s_rtmidi, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7_rtmidi_11RtMidiError_1__init__, 0, __pyx_n_s_RtMidiError___init, NULL, __pyx_n_s_rtmidi, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_t_7);
   PyList_Append(__pyx_t_6, __pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_7);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__18);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_init, __pyx_t_7) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_init, __pyx_t_7) < 0) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "_rtmidi.pyx":265
+  /* "_rtmidi.pyx":270
  * # custom exceptions
  * 
  * class RtMidiError(Exception):             # <<<<<<<<<<<<<<
  *     """Base general RtMidi exception.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_RtMidiError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_RtMidiError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_CyFunction_InitClassCell(__pyx_t_6, __pyx_t_7) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
+  if (__Pyx_CyFunction_InitClassCell(__pyx_t_6, __pyx_t_7) < 0) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RtMidiError, __pyx_t_7) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RtMidiError, __pyx_t_7) < 0) __PYX_ERR(0, 270, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":281
+  /* "_rtmidi.pyx":286
  * 
  * 
  * class InvalidPortError(RtMidiError, ValueError):             # <<<<<<<<<<<<<<
  *     """Raised when an invalid port number is used.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_builtin_ValueError);
   __Pyx_GIVEREF(__pyx_builtin_ValueError);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_builtin_ValueError);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_InvalidPortError, __pyx_n_s_InvalidPortError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_when_an_invalid_port_numb); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_InvalidPortError, __pyx_n_s_InvalidPortError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_when_an_invalid_port_numb); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "_rtmidi.pyx":287
+  /* "_rtmidi.pyx":292
  * 
  *     """
  *     type = ERR_INVALID_PARAMETER             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 287, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "_rtmidi.pyx":281
+  /* "_rtmidi.pyx":286
  * 
  * 
  * class InvalidPortError(RtMidiError, ValueError):             # <<<<<<<<<<<<<<
  *     """Raised when an invalid port number is used.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_InvalidPortError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_InvalidPortError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InvalidPortError, __pyx_t_7) < 0) __PYX_ERR(0, 281, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InvalidPortError, __pyx_t_7) < 0) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_rtmidi.pyx":290
+  /* "_rtmidi.pyx":295
  * 
  * 
  * class InvalidUseError(RtMidiError, RuntimeError):             # <<<<<<<<<<<<<<
  *     """Raised when an method call is not allowed in the current state.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 295, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __Pyx_INCREF(__pyx_builtin_RuntimeError);
   __Pyx_GIVEREF(__pyx_builtin_RuntimeError);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_builtin_RuntimeError);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 295, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_InvalidUseError, __pyx_n_s_InvalidUseError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_when_an_method_call_is_no); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_InvalidUseError, __pyx_n_s_InvalidUseError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_when_an_method_call_is_no); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 295, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "_rtmidi.pyx":296
+  /* "_rtmidi.pyx":301
  * 
  *     """
  *     type = ERR_INVALID_USE             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_USE); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 296, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_USE); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 296, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 301, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "_rtmidi.pyx":290
+  /* "_rtmidi.pyx":295
  * 
  * 
  * class InvalidUseError(RtMidiError, RuntimeError):             # <<<<<<<<<<<<<<
  *     """Raised when an method call is not allowed in the current state.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_InvalidUseError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_InvalidUseError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 295, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InvalidUseError, __pyx_t_7) < 0) __PYX_ERR(0, 290, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InvalidUseError, __pyx_t_7) < 0) __PYX_ERR(0, 295, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":299
+  /* "_rtmidi.pyx":304
  * 
  * 
  * class MemoryAllocationError(RtMidiError, MemoryError):             # <<<<<<<<<<<<<<
  *     """Raised if a memory allocation failed on the C++ level.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_builtin_MemoryError);
   __Pyx_GIVEREF(__pyx_builtin_MemoryError);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_builtin_MemoryError);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_MemoryAllocationError, __pyx_n_s_MemoryAllocationError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_a_memory_allocation_fa); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_MemoryAllocationError, __pyx_n_s_MemoryAllocationError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_a_memory_allocation_fa); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "_rtmidi.pyx":305
+  /* "_rtmidi.pyx":310
  * 
  *     """
  *     type = ERR_MEMORY_ERROR             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 305, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 310, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 305, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "_rtmidi.pyx":299
+  /* "_rtmidi.pyx":304
  * 
  * 
  * class MemoryAllocationError(RtMidiError, MemoryError):             # <<<<<<<<<<<<<<
  *     """Raised if a memory allocation failed on the C++ level.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_MemoryAllocationError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_MemoryAllocationError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MemoryAllocationError, __pyx_t_7) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MemoryAllocationError, __pyx_t_7) < 0) __PYX_ERR(0, 304, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_rtmidi.pyx":308
+  /* "_rtmidi.pyx":313
  * 
  * 
  * class SystemError(RtMidiError, OSError):             # <<<<<<<<<<<<<<
  *     """Raised if an error happened at the MIDI driver or OS level.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __Pyx_INCREF(__pyx_builtin_OSError);
   __Pyx_GIVEREF(__pyx_builtin_OSError);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_builtin_OSError);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_SystemError, __pyx_n_s_SystemError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_an_error_happened_at_t); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_SystemError, __pyx_n_s_SystemError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_an_error_happened_at_t); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_SystemError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_SystemError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SystemError, __pyx_t_7) < 0) __PYX_ERR(0, 308, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SystemError, __pyx_t_7) < 0) __PYX_ERR(0, 313, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":317
+  /* "_rtmidi.pyx":322
  * 
  * 
  * class NoDevicesError(SystemError):             # <<<<<<<<<<<<<<
  *     """Raised if no MIDI devices are found.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_NoDevicesError, __pyx_n_s_NoDevicesError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_no_MIDI_devices_are_fo); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_NoDevicesError, __pyx_n_s_NoDevicesError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_no_MIDI_devices_are_fo); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "_rtmidi.pyx":323
+  /* "_rtmidi.pyx":328
  * 
  *     """
  *     type = ERR_NO_DEVICES_FOUND             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::NO_DEVICES_FOUND); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::NO_DEVICES_FOUND); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "_rtmidi.pyx":317
+  /* "_rtmidi.pyx":322
  * 
  * 
  * class NoDevicesError(SystemError):             # <<<<<<<<<<<<<<
  *     """Raised if no MIDI devices are found.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_NoDevicesError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_NoDevicesError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NoDevicesError, __pyx_t_7) < 0) __PYX_ERR(0, 317, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NoDevicesError, __pyx_t_7) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "_rtmidi.pyx":326
+  /* "_rtmidi.pyx":331
  * 
  * 
  * class UnsupportedOperationError(RtMidiError, RuntimeError):             # <<<<<<<<<<<<<<
  *     """Raised if a method is not supported by the low-level API.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __Pyx_INCREF(__pyx_builtin_RuntimeError);
   __Pyx_GIVEREF(__pyx_builtin_RuntimeError);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_builtin_RuntimeError);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_UnsupportedOperationError, __pyx_n_s_UnsupportedOperationError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_a_method_is_not_suppor); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_UnsupportedOperationError, __pyx_n_s_UnsupportedOperationError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_a_method_is_not_suppor); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_UnsupportedOperationError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_UnsupportedOperationError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnsupportedOperationError, __pyx_t_7) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnsupportedOperationError, __pyx_t_7) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":337
+  /* "_rtmidi.pyx":342
  * # wrappers for RtMidi's static methods and classes
  * 
  * def get_api_display_name(api):             # <<<<<<<<<<<<<<
  *     """Return the display name of a specified MIDI API.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_3get_api_display_name, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_3get_api_display_name, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_api_display_name, __pyx_t_1) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_api_display_name, __pyx_t_1) < 0) __PYX_ERR(0, 342, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":353
+  /* "_rtmidi.pyx":358
  * 
  * 
  * def get_api_name(api):             # <<<<<<<<<<<<<<
  *     """Return the name of a specified MIDI API.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_5get_api_name, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_5get_api_name, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_api_name, __pyx_t_1) < 0) __PYX_ERR(0, 353, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_api_name, __pyx_t_1) < 0) __PYX_ERR(0, 358, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":369
+  /* "_rtmidi.pyx":374
  * 
  * 
  * def get_compiled_api():             # <<<<<<<<<<<<<<
  *     """Return a list of low-level MIDI backend APIs this module supports.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_7get_compiled_api, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_7get_compiled_api, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_compiled_api, __pyx_t_1) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_compiled_api, __pyx_t_1) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":385
+  /* "_rtmidi.pyx":390
  * 
  * 
  * def get_compiled_api_by_name(name):             # <<<<<<<<<<<<<<
  *     """Return the compiled MIDI API having the given name.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_9get_compiled_api_by_name, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_9get_compiled_api_by_name, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 390, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_compiled_api_by_name, __pyx_t_1) < 0) __PYX_ERR(0, 385, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_compiled_api_by_name, __pyx_t_1) < 0) __PYX_ERR(0, 390, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":396
+  /* "_rtmidi.pyx":401
  * 
  * 
  * def get_rtmidi_version():             # <<<<<<<<<<<<<<
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_11get_rtmidi_version, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_11get_rtmidi_version, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_rtmidi_version, __pyx_t_1) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_rtmidi_version, __pyx_t_1) < 0) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":401
+  /* "_rtmidi.pyx":406
  * 
  * 
  * def _default_error_handler(etype, msg, data=None):             # <<<<<<<<<<<<<<
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_13_default_error_handler, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_13_default_error_handler, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_default_error_handler, __pyx_t_1) < 0) __PYX_ERR(0, 401, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_default_error_handler, __pyx_t_1) < 0) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":803
+  /* "_rtmidi.pyx":808
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None,             # <<<<<<<<<<<<<<
  *                   unsigned int queue_size_limit=1024):
  *         """Create a new client instance for MIDI input.
  */
   __pyx_k__4 = RtMidi::UNSPECIFIED;
 
-  /* "_rtmidi.pyx":882
+  /* "_rtmidi.pyx":887
  *         MidiBase.close_port(self)
  * 
  *     close_port.__doc__ == MidiBase.close_port.__doc__             # <<<<<<<<<<<<<<
  * 
  *     def get_message(self):
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_7_rtmidi_MidiIn, __pyx_n_s_close_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_7_rtmidi_MidiIn, __pyx_n_s_close_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 887, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_doc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 882, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_doc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 887, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7_rtmidi_MidiBase), __pyx_n_s_close_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7_rtmidi_MidiBase), __pyx_n_s_close_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 887, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_doc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 882, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_doc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 887, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyObject_RichCompare(__pyx_t_4, __pyx_t_5, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_4, __pyx_t_5, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 887, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "_rtmidi.pyx":1008
+  /* "_rtmidi.pyx":1013
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None):             # <<<<<<<<<<<<<<
  *         """Create a new client instance for MIDI output.
  * 
  */
   __pyx_k__7 = RtMidi::UNSPECIFIED;
@@ -15183,15 +15204,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -15741,15 +15765,15 @@
                         } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
                             return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15937,15 +15961,15 @@
                         } else if (8 * sizeof(enum RtMidi::Api) >= 4 * PyLong_SHIFT) {
                             return (enum RtMidi::Api) (((((((((enum RtMidi::Api)digits[3]) << PyLong_SHIFT) | (enum RtMidi::Api)digits[2]) << PyLong_SHIFT) | (enum RtMidi::Api)digits[1]) << PyLong_SHIFT) | (enum RtMidi::Api)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16133,15 +16157,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16329,15 +16353,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16639,15 +16663,15 @@
                         } else if (8 * sizeof(unsigned char) >= 4 * PyLong_SHIFT) {
                             return (unsigned char) (((((((((unsigned char)digits[3]) << PyLong_SHIFT) | (unsigned char)digits[2]) << PyLong_SHIFT) | (unsigned char)digits[1]) << PyLong_SHIFT) | (unsigned char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -16835,15 +16859,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `python-rtmidi-1.5.0/src/_rtmidi.pyx` & `python-rtmidi-1.5.1/src/_rtmidi.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,17 @@
     Linux ALSA
 ``API_UNIX_JACK``
     Jack Client
 ``API_WINDOWS_MM``
     Windows MultiMedia
 ``API_RTMIDI_DUMMY``
     RtMidi Dummy API (used when no suitable API was found)
+``API_RWEB_MIDI``
+    W3C Web MIDI API
+
 
 
 Error types
 -----------
 
 These constants are passed as the first argument to an error handler
 function registered with ``set_error_callback`` method of a ``MidiIn``
@@ -109,15 +112,15 @@
 from libcpp cimport bool
 from libcpp.string cimport string
 from libcpp.vector cimport vector
 
 
 __all__ = (
     'API_UNSPECIFIED', 'API_MACOSX_CORE', 'API_LINUX_ALSA', 'API_UNIX_JACK',
-    'API_WINDOWS_MM', 'API_RTMIDI_DUMMY', 'ERRORTYPE_DEBUG_WARNING',
+    'API_WINDOWS_MM', 'API_RTMIDI_DUMMY', 'API_WEB_MIDI', 'ERRORTYPE_DEBUG_WARNING',
     'ERRORTYPE_DRIVER_ERROR', 'ERRORTYPE_INVALID_DEVICE',
     'ERRORTYPE_INVALID_PARAMETER', 'ERRORTYPE_INVALID_USE',
     'ERRORTYPE_MEMORY_ERROR', 'ERRORTYPE_NO_DEVICES_FOUND',
     'ERRORTYPE_SYSTEM_ERROR', 'ERRORTYPE_THREAD_ERROR',
     'ERRORTYPE_UNSPECIFIED', 'ERRORTYPE_WARNING', 'InvalidPortError',
     'InvalidUseError', 'MemoryAllocationError', 'MidiIn', 'MidiOut',
     'NoDevicesError', 'RtMidiError', 'SystemError',
@@ -144,14 +147,15 @@
     cdef enum Api "RtMidi::Api":
         UNSPECIFIED  "RtMidi::UNSPECIFIED"
         MACOSX_CORE  "RtMidi::MACOSX_CORE"
         LINUX_ALSA   "RtMidi::LINUX_ALSA"
         UNIX_JACK    "RtMidi::UNIX_JACK"
         WINDOWS_MM   "RtMidi::WINDOWS_MM"
         RTMIDI_DUMMY "RtMidi::RTMIDI_DUMMY"
+        WEB_MIDI     "RtMidi::WEB_MIDI_API"
 
     cdef enum ErrorType "RtMidiError::Type":
         ERR_WARNING           "RtMidiError::WARNING"
         ERR_DEBUG_WARNING     "RtMidiError::DEBUG_WARNING"
         ERR_UNSPECIFIED       "RtMidiError::UNSPECIFIED"
         ERR_NO_DEVICES_FOUND  "RtMidiError::NO_DEVICES_FOUND"
         ERR_INVALID_DEVICE    "RtMidiError::INVALID_DEVICE"
@@ -240,14 +244,15 @@
 
 API_UNSPECIFIED = UNSPECIFIED
 API_MACOSX_CORE = MACOSX_CORE
 API_LINUX_ALSA = LINUX_ALSA
 API_UNIX_JACK = UNIX_JACK
 API_WINDOWS_MM = WINDOWS_MM
 API_RTMIDI_DUMMY = RTMIDI_DUMMY
+API_WEB_MIDI = WEB_MIDI
 
 # export error values to Python
 
 ERRORTYPE_WARNING = ERR_WARNING
 ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING
 ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
 ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
```

### Comparing `python-rtmidi-1.5.0/src/meson.build` & `python-rtmidi-1.5.1/src/meson.build`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/meson_dist_cython.py` & `python-rtmidi-1.5.1/src/meson_dist_cython.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 verbose = environ.get("MESON_INSTALL_QUIET") is None
 
 ap = argparse.ArgumentParser()
 ap.add_argument("-v", "--verbose", action="store_true", default=verbose, help="Be more verbose.")
 ap.add_argument("mod_source", nargs="*", help="Cython module C++ source target(s) (*.cpp).")
 args = ap.parse_args()
 
+
 if args.verbose:
     print("cwd:", getcwd())
     print("build root:", build_root)
     print("dist root:", dist_root)
     print("source root:", source_root)
     print("sys.argv:", sys.argv)
```

### Comparing `python-rtmidi-1.5.0/src/rtmidi/CMakeLists.txt` & `python-rtmidi-1.5.1/src/rtmidi/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/LICENSE` & `python-rtmidi-1.5.1/src/rtmidi/LICENSE`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/Makefile.am` & `python-rtmidi-1.5.1/src/rtmidi/Makefile.am`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/README.md` & `python-rtmidi-1.5.1/src/rtmidi/README.md`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/RtMidi.cpp` & `python-rtmidi-1.5.1/src/rtmidi/RtMidi.cpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -374,16 +374,16 @@
 extern "C" {
 const char* rtmidi_api_names[][2] = {
   { "unspecified" , "Unknown" },
   { "core"        , "CoreMidi" },
   { "alsa"        , "ALSA" },
   { "jack"        , "Jack" },
   { "winmm"       , "Windows MultiMedia" },
-  { "web"         , "Web MIDI API" },
   { "dummy"       , "Dummy" },
+  { "web"         , "Web MIDI API" },
 };
 const unsigned int rtmidi_num_api_names =
   sizeof(rtmidi_api_names)/sizeof(rtmidi_api_names[0]);
 
 // The order here will control the order of RtMidi's API search in
 // the constructor.
 extern "C" const RtMidi::Api rtmidi_compiled_apis[] = {
```

### Comparing `python-rtmidi-1.5.0/src/rtmidi/RtMidi.h` & `python-rtmidi-1.5.1/src/rtmidi/RtMidi.h`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/autogen.sh` & `python-rtmidi-1.5.1/src/rtmidi/autogen.sh`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in` & `python-rtmidi-1.5.1/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/configure.ac` & `python-rtmidi-1.5.1/src/rtmidi/configure.ac`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi.go` & `python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi.go`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go` & `python-rtmidi-1.5.1/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/doc/Makefile.am` & `python-rtmidi-1.5.1/src/rtmidi/doc/Makefile.am`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/Doxyfile.in` & `python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/tutorial.txt` & `python-rtmidi-1.5.1/src/rtmidi/doc/doxygen/tutorial.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/doc/images/ccrma.gif` & `python-rtmidi-1.5.1/src/rtmidi/doc/images/ccrma.gif`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/doc/images/mcgill.gif` & `python-rtmidi-1.5.1/src/rtmidi/doc/images/mcgill.gif`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/doc/release.txt` & `python-rtmidi-1.5.1/src/rtmidi/doc/release.txt`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4` & `python-rtmidi-1.5.1/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/msw/rtmidilib.sln` & `python-rtmidi-1.5.1/src/rtmidi/msw/rtmidilib.sln`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/msw/rtmidilib.vcproj` & `python-rtmidi-1.5.1/src/rtmidi/msw/rtmidilib.vcproj`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/rtmidi_c.cpp` & `python-rtmidi-1.5.1/src/rtmidi/rtmidi_c.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 class StaticAssertions { StaticAssertions() {
     ENUM_EQUAL( RTMIDI_API_UNSPECIFIED,     RtMidi::UNSPECIFIED );
     ENUM_EQUAL( RTMIDI_API_MACOSX_CORE,     RtMidi::MACOSX_CORE );
     ENUM_EQUAL( RTMIDI_API_LINUX_ALSA,      RtMidi::LINUX_ALSA );
     ENUM_EQUAL( RTMIDI_API_UNIX_JACK,       RtMidi::UNIX_JACK );
     ENUM_EQUAL( RTMIDI_API_WINDOWS_MM,      RtMidi::WINDOWS_MM );
     ENUM_EQUAL( RTMIDI_API_RTMIDI_DUMMY,    RtMidi::RTMIDI_DUMMY );
+    ENUM_EQUAL( RTMIDI_API_WEB_MIDI_API,    RtMidi::WEB_MIDI_API );
 
     ENUM_EQUAL( RTMIDI_ERROR_WARNING,            RtMidiError::WARNING );
     ENUM_EQUAL( RTMIDI_ERROR_DEBUG_WARNING,      RtMidiError::DEBUG_WARNING );
     ENUM_EQUAL( RTMIDI_ERROR_UNSPECIFIED,        RtMidiError::UNSPECIFIED );
     ENUM_EQUAL( RTMIDI_ERROR_NO_DEVICES_FOUND,   RtMidiError::NO_DEVICES_FOUND );
     ENUM_EQUAL( RTMIDI_ERROR_INVALID_DEVICE,     RtMidiError::INVALID_DEVICE );
     ENUM_EQUAL( RTMIDI_ERROR_MEMORY_ERROR,       RtMidiError::MEMORY_ERROR );
```

### Comparing `python-rtmidi-1.5.0/src/rtmidi/rtmidi_c.h` & `python-rtmidi-1.5.1/src/rtmidi/rtmidi_c.h`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 enum RtMidiApi {
     RTMIDI_API_UNSPECIFIED,    /*!< Search for a working compiled API. */
     RTMIDI_API_MACOSX_CORE,    /*!< Macintosh OS-X CoreMIDI API. */
     RTMIDI_API_LINUX_ALSA,     /*!< The Advanced Linux Sound Architecture API. */
     RTMIDI_API_UNIX_JACK,      /*!< The Jack Low-Latency MIDI Server API. */
     RTMIDI_API_WINDOWS_MM,     /*!< The Microsoft Multimedia MIDI API. */
     RTMIDI_API_RTMIDI_DUMMY,   /*!< A compilable but non-functional API. */
+    RTMIDI_API_WEB_MIDI_API,   /*!< W3C Web MIDI API. */
     RTMIDI_API_NUM             /*!< Number of values in this enum. */
 };
 
 //! \brief Defined RtMidiError types. See \ref RtMidiError::Type.
 enum RtMidiErrorType {
   RTMIDI_ERROR_WARNING,           /*!< A non-critical error. */
   RTMIDI_ERROR_DEBUG_WARNING,     /*!< A non-critical error which might be useful for debugging. */
@@ -152,18 +153,18 @@
 
 /*! \brief Return the number of available MIDI ports.
  * See RtMidi::getPortCount().
  */
 RTMIDIAPI unsigned int rtmidi_get_port_count (RtMidiPtr device);
 
 /*! \brief Access a string identifier for the specified MIDI input port number.
- * 
+ *
  * To prevent memory leaks a char buffer must be passed to this function.
  * NULL can be passed as bufOut parameter, and that will write the required buffer length in the bufLen.
- * 
+ *
  * See RtMidi::getPortName().
  */
 RTMIDIAPI int rtmidi_get_port_name (RtMidiPtr device, unsigned int portNumber, char * bufOut, int * bufLen);
 
 /* RtMidiIn API */
 
 //! \brief Create a default RtMidiInPtr value, with no initialization.
```

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/Makefile.am` & `python-rtmidi-1.5.1/src/rtmidi/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/RtMidi.dsw` & `python-rtmidi-1.5.1/src/rtmidi/tests/RtMidi.dsw`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/apinames.cpp` & `python-rtmidi-1.5.1/src/rtmidi/tests/apinames.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/cmidiin.cpp` & `python-rtmidi-1.5.1/src/rtmidi/tests/cmidiin.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/cmidiin.dsp` & `python-rtmidi-1.5.1/src/rtmidi/tests/cmidiin.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/midiclock.cpp` & `python-rtmidi-1.5.1/src/rtmidi/tests/midiclock.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/midiout.cpp` & `python-rtmidi-1.5.1/src/rtmidi/tests/midiout.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/midiout.dsp` & `python-rtmidi-1.5.1/src/rtmidi/tests/midiout.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/midiprobe.cpp` & `python-rtmidi-1.5.1/src/rtmidi/tests/midiprobe.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/midiprobe.dsp` & `python-rtmidi-1.5.1/src/rtmidi/tests/midiprobe.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/qmidiin.cpp` & `python-rtmidi-1.5.1/src/rtmidi/tests/qmidiin.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/qmidiin.dsp` & `python-rtmidi-1.5.1/src/rtmidi/tests/qmidiin.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/sysextest.cpp` & `python-rtmidi-1.5.1/src/rtmidi/tests/sysextest.cpp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/sysextest.dsp` & `python-rtmidi-1.5.1/src/rtmidi/tests/sysextest.dsp`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/src/rtmidi/tests/testcapi.c` & `python-rtmidi-1.5.1/src/rtmidi/tests/testcapi.c`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/tests/test_delete.py` & `python-rtmidi-1.5.1/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/tests/test_errorcallback.py` & `python-rtmidi-1.5.1/tests/test_errorcallback.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/tests/test_errors.py` & `python-rtmidi-1.5.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/tests/test_rtmidi.py` & `python-rtmidi-1.5.1/tests/test_rtmidi.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.5.0/PKG-INFO` & `python-rtmidi-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-rtmidi
-Version: 1.5.0
+Version: 1.5.1
 Summary: A Python binding for the RtMidi C++ library implemented using Cython.
 Keywords: MIDI, multimedia, music, rtmidi
 Author: Christopher Arndt
 Author-email: info@chrisarndt.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
```

