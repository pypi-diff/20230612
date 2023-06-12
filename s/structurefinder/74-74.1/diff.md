# Comparing `tmp/structurefinder-74.tar.gz` & `tmp/structurefinder-74.1.tar.gz`

## Comparing `structurefinder-74.tar` & `structurefinder-74.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 structurefinder-74/.gitattributes
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 structurefinder-74/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 structurefinder-74/StructureFinder.spec
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 structurefinder-74/StructureFinder_linux.spec
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 structurefinder-74/StructureFinder_mac.spec
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 structurefinder-74/install_all_requirements
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 structurefinder-74/install_all_requirements.bat
--rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 structurefinder-74/install_min_requirements
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 structurefinder-74/pytest.ini
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 structurefinder-74/requirements.txt
--rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 structurefinder-74/strf
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 structurefinder-74/strf.bat
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 structurefinder-74/strf_cmd
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 structurefinder-74/strf_cmd.bat
--rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 structurefinder-74/strf_web
--rw-r--r--   0        0        0  8071400 2020-02-02 00:00:00.000000 structurefinder-74/update.exe
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 structurefinder-74/docs/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/docs/__init__.py
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 structurefinder-74/docs/changes.txt
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 structurefinder-74/docs/commandline.rst
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 structurefinder-74/docs/conf.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 structurefinder-74/docs/example.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 structurefinder-74/docs/index.rst
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 structurefinder-74/docs/indexing.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 structurefinder-74/docs/installation.rst
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 structurefinder-74/docs/main.rst
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 structurefinder-74/docs/make.bat
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 structurefinder-74/docs/misc.rst
--rw-r--r--   0        0        0   112698 2020-02-02 00:00:00.000000 structurefinder-74/docs/pics/strf_1.png
--rw-r--r--   0        0        0    58105 2020-02-02 00:00:00.000000 structurefinder-74/docs/pics/strf_2.png
--rw-r--r--   0        0        0    18946 2020-02-02 00:00:00.000000 structurefinder-74/docs/pics/strf_4.png
--rw-r--r--   0        0        0    32402 2020-02-02 00:00:00.000000 structurefinder-74/docs/pics/strf_adv.png
--rw-r--r--   0        0        0   167550 2020-02-02 00:00:00.000000 structurefinder-74/docs/pics/strf_web.png
--rw-r--r--   0        0        0    35368 2020-02-02 00:00:00.000000 structurefinder-74/icons/strf.ico
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 structurefinder-74/icons/strf.png
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/__init__.py
--rw-r--r--   0        0        0    56921 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/strf.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/strf_cmd.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/ccdc/__init__.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/ccdc/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/__init__.py
--rw-r--r--   0        0        0   170898 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/bottle.py
--rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/strf_web.py
--rw-r--r--   0        0        0    35368 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/favicon.ico
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/strf_web.css
--rw-r--r--   0        0        0    20998 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/strf_web.js
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/strf_web_csd.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/custom.css
--rw-r--r--   0        0        0    26132 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css
--rw-r--r--   0        0        0    47706 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css.map
--rw-r--r--   0        0        0    23409 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css
--rw-r--r--   0        0        0    25648 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css.map
--rw-r--r--   0        0        0   146010 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css
--rw-r--r--   0        0        0   389287 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css.map
--rw-r--r--   0        0        0   121200 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css
--rw-r--r--   0        0        0   542194 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css.map
--rw-r--r--   0        0        0    22707 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/font-awesome.css
--rw-r--r--   0        0        0    63008 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/FontAwesome.otf
--rw-r--r--   0        0        0    38239 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   202471 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0    80776 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    44476 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0    62850 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    41236 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23292 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0    18028 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0        0        0    69707 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.js
--rw-r--r--   0        0        0    37045 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.min.js
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/npm.js
--rw-r--r--   0        0        0    24977 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/clipboard/clipboard.js
--rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/clipboard/clipboard.min.js
--rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/jquery/jquery-3.2.1.min.js
--rw-r--r--   0        0        0   128442 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/jsmol/JSmol_dk.nojq.lite.js
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/bower.json
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/license.txt
--rw-r--r--   0        0        0    88141 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.css
--rw-r--r--   0        0        0   678867 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.js
--rw-r--r--   0        0        0    75404 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.css
--rw-r--r--   0        0        0   299228 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.js
--rw-r--r--   0        0        0   107093 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.css
--rw-r--r--   0        0        0   943882 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.js
--rw-r--r--   0        0        0    92412 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.css
--rw-r--r--   0        0        0   405298 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.js
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/bg-bg.json
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/de-de.json
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/en-us.json
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/es-mx.json
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/fr-fr.json
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/it-it.json
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/ja-jp.json
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/ko-kr.json
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/nl-nl.json
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/pl-pl.json
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/pt-br.json
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/ru-ru.json
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/tr-tr.json
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/zh-cn.json
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/views/advanced_search.tpl
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/views/cellcheckcsd.tpl
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/views/simpl_search.tpl
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/views/spgr.tpl
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/views/strf_base.tpl
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/cgi_ui/views/strf_web.tpl
--rw-r--r--   0        0        0   128445 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/displaymol/JSmol_dk.nojq.lite.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/displaymol/__init__.py
--rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/displaymol/jquery.min.js
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/displaymol/mol_file_writer.py
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/displaymol/molecule2D.py
--rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/displaymol/sdm.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/displaymol/write_html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/gui/__init__.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/gui/strf_dbpasswd.py
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/gui/strf_dbpasswd.ui
--rw-r--r--   0        0        0   109362 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/gui/strf_main.py
--rw-r--r--   0        0        0   127483 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/gui/strf_main.ui
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/gui/table_model.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/gui/table_view.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/gui/table_view_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/misc/__init__.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/misc/dialogs.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/misc/download.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/misc/exporter.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/misc/settings.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/misc/update_check.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/misc/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/p4pfile/__init__.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/p4pfile/p4p_reader.py
--rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/pg8000/__init__.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/pg8000/_version.py
--rw-r--r--   0        0        0    89534 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/pg8000/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/pymatgen/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/pymatgen/core/__init__.py
--rw-r--r--   0        0        0    42399 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/pymatgen/core/lattice.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/pymatgen/util/__init__.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/pymatgen/util/num_utils.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/pymatgen/util/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/cif.textx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/compare.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/constants.py
--rw-r--r--   0        0        0    54741 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/database_handler.py
--rw-r--r--   0        0        0    12330 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/filecrawler.py
--rw-r--r--   0        0        0    20554 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/fileparser.py
--rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/misc.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/spinner.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/unitcell.py
--rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/searcher/worker.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/shelxfile/__init__.py
--rw-r--r--   0        0        0    22722 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/shelxfile/atoms.py
--rw-r--r--   0        0        0    53857 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/shelxfile/cards.py
--rw-r--r--   0        0        0    44739 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/shelxfile/dsrmath.py
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/shelxfile/elements.py
--rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/shelxfile/misc.py
--rw-r--r--   0        0        0    45843 2020-02-02 00:00:00.000000 structurefinder-74/src/structurefinder/shelxfile/shelx.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 structurefinder-74/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 structurefinder-74/LICENSE
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 structurefinder-74/pyproject.toml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 structurefinder-74/PKG-INFO
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 structurefinder-74.1/.gitattributes
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 structurefinder-74.1/StructureFinder.spec
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 structurefinder-74.1/StructureFinder_linux.spec
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 structurefinder-74.1/StructureFinder_mac.spec
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 structurefinder-74.1/install_all_requirements
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 structurefinder-74.1/install_all_requirements.bat
+-rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 structurefinder-74.1/install_min_requirements
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 structurefinder-74.1/pytest.ini
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 structurefinder-74.1/requirements.txt
+-rwxr-xr-x   0        0        0      240 2020-02-02 00:00:00.000000 structurefinder-74.1/strf
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 structurefinder-74.1/strf.bat
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 structurefinder-74.1/strf_cmd
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 structurefinder-74.1/strf_cmd.bat
+-rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 structurefinder-74.1/strf_web
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 structurefinder-74.1/update.exe
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/__init__.py
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/changes.txt
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/commandline.rst
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/conf.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/example.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/index.rst
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/indexing.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/installation.rst
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/main.rst
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/make.bat
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/misc.rst
+-rw-r--r--   0        0        0   112698 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/pics/strf_1.png
+-rw-r--r--   0        0        0    58105 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/pics/strf_2.png
+-rw-r--r--   0        0        0    18946 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/pics/strf_4.png
+-rw-r--r--   0        0        0    32402 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/pics/strf_adv.png
+-rw-r--r--   0        0        0   167550 2020-02-02 00:00:00.000000 structurefinder-74.1/docs/pics/strf_web.png
+-rw-r--r--   0        0        0    35368 2020-02-02 00:00:00.000000 structurefinder-74.1/icons/strf.ico
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 structurefinder-74.1/icons/strf.png
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/__init__.py
+-rw-r--r--   0        0        0    56921 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/strf.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/strf_cmd.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/ccdc/__init__.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/ccdc/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/__init__.py
+-rw-r--r--   0        0        0   170898 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/bottle.py
+-rw-r--r--   0        0        0    28033 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/strf_web.py
+-rw-r--r--   0        0        0    35368 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/favicon.ico
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/strf_web.css
+-rw-r--r--   0        0        0    20998 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/strf_web.js
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/strf_web_csd.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/custom.css
+-rw-r--r--   0        0        0    26132 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css
+-rw-r--r--   0        0        0    47706 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css.map
+-rw-r--r--   0        0        0    23409 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css
+-rw-r--r--   0        0        0    25648 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css.map
+-rw-r--r--   0        0        0   146010 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css
+-rw-r--r--   0        0        0   389287 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css.map
+-rw-r--r--   0        0        0   121200 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css
+-rw-r--r--   0        0        0   542194 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0    22707 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/font-awesome.css
+-rw-r--r--   0        0        0    63008 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/FontAwesome.otf
+-rw-r--r--   0        0        0    38239 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   202471 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0    80776 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    44476 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    20290 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0    62850 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    41236 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23292 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    18028 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0        0        0    69707 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.js
+-rw-r--r--   0        0        0    37045 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.min.js
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/npm.js
+-rw-r--r--   0        0        0    24977 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/clipboard/clipboard.js
+-rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/clipboard/clipboard.min.js
+-rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/jquery/jquery-3.2.1.min.js
+-rw-r--r--   0        0        0   128442 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/jsmol/JSmol_dk.nojq.lite.js
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/bower.json
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/license.txt
+-rw-r--r--   0        0        0    88141 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.css
+-rw-r--r--   0        0        0   678867 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.js
+-rw-r--r--   0        0        0    75404 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.css
+-rw-r--r--   0        0        0   299228 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.js
+-rw-r--r--   0        0        0   107093 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.css
+-rw-r--r--   0        0        0   943882 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.js
+-rw-r--r--   0        0        0    92412 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.css
+-rw-r--r--   0        0        0   405298 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.js
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/bg-bg.json
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/de-de.json
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/en-us.json
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/es-mx.json
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/fr-fr.json
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/it-it.json
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/ja-jp.json
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/ko-kr.json
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/nl-nl.json
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/pl-pl.json
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/pt-br.json
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/ru-ru.json
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/tr-tr.json
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/zh-cn.json
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/views/advanced_search.tpl
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/views/cellcheckcsd.tpl
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/views/simpl_search.tpl
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/views/spgr.tpl
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/views/strf_base.tpl
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/cgi_ui/views/strf_web.tpl
+-rw-r--r--   0        0        0   128445 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/displaymol/JSmol_dk.nojq.lite.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/displaymol/__init__.py
+-rw-r--r--   0        0        0    86659 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/displaymol/jquery.min.js
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/displaymol/mol_file_writer.py
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/displaymol/molecule2D.py
+-rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/displaymol/sdm.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/displaymol/write_html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/gui/__init__.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/gui/strf_dbpasswd.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/gui/strf_dbpasswd.ui
+-rw-r--r--   0        0        0   109362 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/gui/strf_main.py
+-rw-r--r--   0        0        0   127483 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/gui/strf_main.ui
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/gui/table_model.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/gui/table_view.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/gui/table_view_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/misc/__init__.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/misc/dialogs.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/misc/download.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/misc/exporter.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/misc/settings.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/misc/update_check.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/misc/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/p4pfile/__init__.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/p4pfile/p4p_reader.py
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/pg8000/__init__.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/pg8000/_version.py
+-rw-r--r--   0        0        0    89534 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/pg8000/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/pymatgen/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/pymatgen/core/__init__.py
+-rw-r--r--   0        0        0    42399 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/pymatgen/core/lattice.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/pymatgen/util/__init__.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/pymatgen/util/num_utils.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/pymatgen/util/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/cif.textx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/compare.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/constants.py
+-rw-r--r--   0        0        0    54741 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/database_handler.py
+-rw-r--r--   0        0        0    12330 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/filecrawler.py
+-rw-r--r--   0        0        0    20554 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/fileparser.py
+-rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/misc.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/spinner.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/unitcell.py
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/searcher/worker.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/shelxfile/__init__.py
+-rw-r--r--   0        0        0    22722 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/shelxfile/atoms.py
+-rw-r--r--   0        0        0    53857 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/shelxfile/cards.py
+-rw-r--r--   0        0        0    44739 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/shelxfile/dsrmath.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/shelxfile/elements.py
+-rw-r--r--   0        0        0    15618 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/shelxfile/misc.py
+-rw-r--r--   0        0        0    45843 2020-02-02 00:00:00.000000 structurefinder-74.1/src/structurefinder/shelxfile/shelx.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 structurefinder-74.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 structurefinder-74.1/LICENSE
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 structurefinder-74.1/README.md
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 structurefinder-74.1/pyproject.toml
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 structurefinder-74.1/PKG-INFO
```

### Comparing `structurefinder-74/README.md` & `structurefinder-74.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-00000000: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000010: 2f72 6570 6f6c 6f67 792e 6f72 672f 7072  /repology.org/pr
-00000020: 6f6a 6563 742f 7079 7468 6f6e 3a73 7472  oject/python:str
-00000030: 7563 7475 7265 6669 6e64 6572 2f76 6572  ucturefinder/ver
-00000040: 7369 6f6e 7322 3e0a 2020 2020 3c69 6d67  sions">.    <img
-00000050: 2073 7263 3d22 6874 7470 733a 2f2f 7265   src="https://re
-00000060: 706f 6c6f 6779 2e6f 7267 2f62 6164 6765  pology.org/badge
-00000070: 2f76 6572 7469 6361 6c2d 616c 6c72 6570  /vertical-allrep
-00000080: 6f73 2f70 7974 686f 6e3a 7374 7275 6374  os/python:struct
-00000090: 7572 6566 696e 6465 722e 7376 6722 2061  urefinder.svg" a
-000000a0: 6c74 3d22 5061 636b 6167 696e 6720 7374  lt="Packaging st
-000000b0: 6174 7573 2220 616c 6967 6e3d 2272 6967  atus" align="rig
-000000c0: 6874 223e 0a3c 2f61 3e0a 0a21 5b4c 6174  ht">.</a>..![Lat
-000000d0: 6573 2052 656c 6561 7365 5d28 6874 7470  es Release](http
-000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000000f0: 696f 2f67 6974 6875 622f 762f 7461 672f  io/github/v/tag/
-00000100: 646b 7261 747a 6572 742f 5374 7275 6374  dkratzert/Struct
-00000110: 7572 6546 696e 6465 723f 6c61 6265 6c3d  ureFinder?label=
-00000120: 4c61 7465 7374 2532 3052 656c 6561 7365  Latest%20Release
-00000130: 290a 5b21 5b55 6e69 7420 5465 7374 735d  ).[![Unit Tests]
-00000140: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000150: 636f 6d2f 646b 7261 747a 6572 742f 5374  com/dkratzert/St
-00000160: 7275 6374 7572 6546 696e 6465 722f 6163  ructureFinder/ac
-00000170: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000180: 7079 7468 6f6e 2d61 7070 5f77 696e 646f  python-app_windo
-00000190: 7773 2e79 6d6c 2f62 6164 6765 2e73 7667  ws.yml/badge.svg
-000001a0: 3f62 7261 6e63 683d 6d61 7374 6572 295d  ?branch=master)]
-000001b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000001c0: 636f 6d2f 646b 7261 747a 6572 742f 5374  com/dkratzert/St
-000001d0: 7275 6374 7572 6546 696e 6465 722f 6163  ructureFinder/ac
-000001e0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-000001f0: 7079 7468 6f6e 2d61 7070 5f77 696e 646f  python-app_windo
-00000200: 7773 2e79 6d6c 290a 215b 436f 6e74 7269  ws.yml).![Contri
-00000210: 6275 7469 6f6e 735d 2868 7474 7073 3a2f  butions](https:/
-00000220: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000230: 6261 6467 652f 636f 6e74 7269 6275 7469  badge/contributi
-00000240: 6f6e 732d 7765 6c63 6f6d 652d 626c 7565  ons-welcome-blue
-00000250: 290a 0a23 2053 7472 7563 7475 7265 4669  )..# StructureFi
-00000260: 6e64 6572 0a41 2063 7279 7374 616c 2073  nder.A crystal s
-00000270: 7472 7563 7475 7265 2066 696e 6465 7220  tructure finder 
-00000280: 7772 6974 7465 6e20 696e 2050 7951 7435  written in PyQt5
-00000290: 2061 6e64 2050 7974 686f 6e33 2077 6974   and Python3 wit
-000002a0: 6820 5351 6c69 7465 2e0a 0a5b 486f 6d65  h SQlite...[Home
-000002b0: 7061 6765 3a20 6874 7470 733a 2f2f 646b  page: https://dk
-000002c0: 7261 747a 6572 742e 6465 2f73 7472 7563  ratzert.de/struc
-000002d0: 7475 7265 6669 6e64 6572 2e68 746d 6c5d  turefinder.html]
-000002e0: 2868 7474 7073 3a2f 2f64 6b72 6174 7a65  (https://dkratze
-000002f0: 7274 2e64 652f 7374 7275 6374 7572 6566  rt.de/structuref
-00000300: 696e 6465 722e 6874 6d6c 290a 0a21 5b50  inder.html)..![P
-00000310: 726f 6772 616d 2057 696e 646f 775d 2868  rogram Window](h
-00000320: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000330: 6d2f 646b 7261 747a 6572 742f 5374 7275  m/dkratzert/Stru
-00000340: 6374 7572 6546 696e 6465 722f 626c 6f62  ctureFinder/blob
-00000350: 2f6d 6173 7465 722f 646f 6373 2f70 6963  /master/docs/pic
-00000360: 732f 7374 7266 5f31 2e70 6e67 3f72 6177  s/strf_1.png?raw
-00000370: 3d74 7275 6529 0a                        =true).
+00000000: 5b21 5b50 6163 6b61 6769 6e67 2053 7461  [![Packaging Sta
+00000010: 7475 735d 2868 7474 7073 3a2f 2f72 6570  tus](https://rep
+00000020: 6f6c 6f67 792e 6f72 672f 6261 6467 652f  ology.org/badge/
+00000030: 7665 7274 6963 616c 2d61 6c6c 7265 706f  vertical-allrepo
+00000040: 732f 7079 7468 6f6e 3a73 7472 7563 7475  s/python:structu
+00000050: 7265 6669 6e64 6572 2e73 7667 295d 2868  refinder.svg)](h
+00000060: 7474 7073 3a2f 2f72 6570 6f6c 6f67 792e  ttps://repology.
+00000070: 6f72 672f 7072 6f6a 6563 742f 7079 7468  org/project/pyth
+00000080: 6f6e 3a73 7472 7563 7475 7265 6669 6e64  on:structurefind
+00000090: 6572 2f76 6572 7369 6f6e 7329 0a0a 0a21  er/versions)...!
+000000a0: 5b4c 6174 6573 2052 656c 6561 7365 5d28  [Lates Release](
+000000b0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000000c0: 6c64 732e 696f 2f67 6974 6875 622f 762f  lds.io/github/v/
+000000d0: 7461 672f 646b 7261 747a 6572 742f 5374  tag/dkratzert/St
+000000e0: 7275 6374 7572 6546 696e 6465 723f 6c61  ructureFinder?la
+000000f0: 6265 6c3d 4c61 7465 7374 2532 3052 656c  bel=Latest%20Rel
+00000100: 6561 7365 290a 5b21 5b55 6e69 7420 5465  ease).[![Unit Te
+00000110: 7374 735d 2868 7474 7073 3a2f 2f67 6974  sts](https://git
+00000120: 6875 622e 636f 6d2f 646b 7261 747a 6572  hub.com/dkratzer
+00000130: 742f 5374 7275 6374 7572 6546 696e 6465  t/StructureFinde
+00000140: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
+00000150: 6f77 732f 7079 7468 6f6e 2d61 7070 5f77  ows/python-app_w
+00000160: 696e 646f 7773 2e79 6d6c 2f62 6164 6765  indows.yml/badge
+00000170: 2e73 7667 3f62 7261 6e63 683d 6d61 7374  .svg?branch=mast
+00000180: 6572 295d 2868 7474 7073 3a2f 2f67 6974  er)](https://git
+00000190: 6875 622e 636f 6d2f 646b 7261 747a 6572  hub.com/dkratzer
+000001a0: 742f 5374 7275 6374 7572 6546 696e 6465  t/StructureFinde
+000001b0: 722f 6163 7469 6f6e 732f 776f 726b 666c  r/actions/workfl
+000001c0: 6f77 732f 7079 7468 6f6e 2d61 7070 5f77  ows/python-app_w
+000001d0: 696e 646f 7773 2e79 6d6c 290a 215b 436f  indows.yml).![Co
+000001e0: 6e74 7269 6275 7469 6f6e 735d 2868 7474  ntributions](htt
+000001f0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000200: 2e69 6f2f 6261 6467 652f 636f 6e74 7269  .io/badge/contri
+00000210: 6275 7469 6f6e 732d 7765 6c63 6f6d 652d  butions-welcome-
+00000220: 626c 7565 290a 0a23 2053 7472 7563 7475  blue)..# Structu
+00000230: 7265 4669 6e64 6572 0a41 2063 7279 7374  reFinder.A cryst
+00000240: 616c 2073 7472 7563 7475 7265 2066 696e  al structure fin
+00000250: 6465 7220 7772 6974 7465 6e20 696e 2050  der written in P
+00000260: 7951 7435 2061 6e64 2050 7974 686f 6e33  yQt5 and Python3
+00000270: 2077 6974 6820 5351 6c69 7465 2e0a 0a5b   with SQlite...[
+00000280: 486f 6d65 7061 6765 3a20 6874 7470 733a  Homepage: https:
+00000290: 2f2f 646b 7261 747a 6572 742e 6465 2f73  //dkratzert.de/s
+000002a0: 7472 7563 7475 7265 6669 6e64 6572 2e68  tructurefinder.h
+000002b0: 746d 6c5d 2868 7474 7073 3a2f 2f64 6b72  tml](https://dkr
+000002c0: 6174 7a65 7274 2e64 652f 7374 7275 6374  atzert.de/struct
+000002d0: 7572 6566 696e 6465 722e 6874 6d6c 290a  urefinder.html).
+000002e0: 0a21 5b50 726f 6772 616d 2057 696e 646f  .![Program Windo
+000002f0: 775d 2868 7474 7073 3a2f 2f67 6974 6875  w](https://githu
+00000300: 622e 636f 6d2f 646b 7261 747a 6572 742f  b.com/dkratzert/
+00000310: 5374 7275 6374 7572 6546 696e 6465 722f  StructureFinder/
+00000320: 626c 6f62 2f6d 6173 7465 722f 646f 6373  blob/master/docs
+00000330: 2f70 6963 732f 7374 7266 5f31 2e70 6e67  /pics/strf_1.png
+00000340: 3f72 6177 3d74 7275 6529 0a              ?raw=true).
```

### Comparing `structurefinder-74/StructureFinder.spec` & `structurefinder-74.1/StructureFinder.spec`

 * *Files identical despite different names*

### Comparing `structurefinder-74/StructureFinder_linux.spec` & `structurefinder-74.1/StructureFinder_linux.spec`

 * *Files identical despite different names*

### Comparing `structurefinder-74/StructureFinder_mac.spec` & `structurefinder-74.1/StructureFinder_mac.spec`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/Makefile` & `structurefinder-74.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/changes.txt` & `structurefinder-74.1/docs/changes.txt`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/commandline.rst` & `structurefinder-74.1/docs/commandline.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/conf.py` & `structurefinder-74.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/example.rst` & `structurefinder-74.1/docs/example.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/indexing.rst` & `structurefinder-74.1/docs/indexing.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/installation.rst` & `structurefinder-74.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/main.rst` & `structurefinder-74.1/docs/main.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/make.bat` & `structurefinder-74.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/misc.rst` & `structurefinder-74.1/docs/misc.rst`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/pics/strf_1.png` & `structurefinder-74.1/docs/pics/strf_1.png`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/pics/strf_2.png` & `structurefinder-74.1/docs/pics/strf_2.png`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/pics/strf_4.png` & `structurefinder-74.1/docs/pics/strf_4.png`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/pics/strf_adv.png` & `structurefinder-74.1/docs/pics/strf_adv.png`

 * *Files identical despite different names*

### Comparing `structurefinder-74/docs/pics/strf_web.png` & `structurefinder-74.1/docs/pics/strf_web.png`

 * *Files identical despite different names*

### Comparing `structurefinder-74/icons/strf.ico` & `structurefinder-74.1/icons/strf.ico`

 * *Files identical despite different names*

### Comparing `structurefinder-74/icons/strf.png` & `structurefinder-74.1/icons/strf.png`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/strf.py` & `structurefinder-74.1/src/structurefinder/strf.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/strf_cmd.py` & `structurefinder-74.1/src/structurefinder/strf_cmd.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/ccdc/query.py` & `structurefinder-74.1/src/structurefinder/ccdc/query.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/bottle.py` & `structurefinder-74.1/src/structurefinder/cgi_ui/bottle.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/strf_web.py` & `structurefinder-74.1/src/structurefinder/cgi_ui/strf_web.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/favicon.ico` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/strf_web.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/strf_web.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/strf_web.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/strf_web.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/strf_web_csd.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/strf_web_csd.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css.map` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css.map` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css.map` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css.map` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/font-awesome.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/FontAwesome.otf` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.eot` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.svg` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.ttf` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.woff` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.eot` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.svg` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.ttf` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff2` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.min.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/bootstrap-3.3.7/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/clipboard/clipboard.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/clipboard/clipboard.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/clipboard/clipboard.min.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/clipboard/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/jquery/jquery-3.2.1.min.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/jquery/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/jsmol/JSmol_dk.nojq.lite.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/jsmol/JSmol_dk.nojq.lite.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/bower.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/bower.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/license.txt` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/license.txt`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.4.3.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.css` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.css`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.js` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/w2ui-1.5.rc1.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/bg-bg.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/bg-bg.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/de-de.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/de-de.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/en-us.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/en-us.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/es-mx.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/es-mx.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/fr-fr.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/fr-fr.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/it-it.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/it-it.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/ja-jp.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/ja-jp.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/ko-kr.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/ko-kr.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/nl-nl.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/nl-nl.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/pl-pl.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/pl-pl.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/pt-br.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/pt-br.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/ru-ru.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/ru-ru.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/tr-tr.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/tr-tr.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/static/w2ui/locale/zh-cn.json` & `structurefinder-74.1/src/structurefinder/cgi_ui/static/w2ui/locale/zh-cn.json`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/views/advanced_search.tpl` & `structurefinder-74.1/src/structurefinder/cgi_ui/views/advanced_search.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/views/cellcheckcsd.tpl` & `structurefinder-74.1/src/structurefinder/cgi_ui/views/cellcheckcsd.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/views/simpl_search.tpl` & `structurefinder-74.1/src/structurefinder/cgi_ui/views/simpl_search.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/views/spgr.tpl` & `structurefinder-74.1/src/structurefinder/cgi_ui/views/spgr.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/views/strf_base.tpl` & `structurefinder-74.1/src/structurefinder/cgi_ui/views/strf_base.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/cgi_ui/views/strf_web.tpl` & `structurefinder-74.1/src/structurefinder/cgi_ui/views/strf_web.tpl`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/displaymol/JSmol_dk.nojq.lite.js` & `structurefinder-74.1/src/structurefinder/displaymol/JSmol_dk.nojq.lite.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/displaymol/jquery.min.js` & `structurefinder-74.1/src/structurefinder/displaymol/jquery.min.js`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/displaymol/mol_file_writer.py` & `structurefinder-74.1/src/structurefinder/displaymol/mol_file_writer.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/displaymol/molecule2D.py` & `structurefinder-74.1/src/structurefinder/displaymol/molecule2D.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/displaymol/sdm.py` & `structurefinder-74.1/src/structurefinder/displaymol/sdm.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/displaymol/write_html.py` & `structurefinder-74.1/src/structurefinder/displaymol/write_html.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/gui/strf_dbpasswd.py` & `structurefinder-74.1/src/structurefinder/gui/strf_dbpasswd.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/gui/strf_dbpasswd.ui` & `structurefinder-74.1/src/structurefinder/gui/strf_dbpasswd.ui`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/gui/strf_main.py` & `structurefinder-74.1/src/structurefinder/gui/strf_main.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/gui/strf_main.ui` & `structurefinder-74.1/src/structurefinder/gui/strf_main.ui`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/gui/table_model.py` & `structurefinder-74.1/src/structurefinder/gui/table_model.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/gui/table_view.py` & `structurefinder-74.1/src/structurefinder/gui/table_view.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/gui/table_view_example.py` & `structurefinder-74.1/src/structurefinder/gui/table_view_example.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/misc/dialogs.py` & `structurefinder-74.1/src/structurefinder/misc/dialogs.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/misc/download.py` & `structurefinder-74.1/src/structurefinder/misc/download.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/misc/exporter.py` & `structurefinder-74.1/src/structurefinder/misc/exporter.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/misc/settings.py` & `structurefinder-74.1/src/structurefinder/misc/settings.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/misc/update_check.py` & `structurefinder-74.1/src/structurefinder/misc/update_check.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/p4pfile/p4p_reader.py` & `structurefinder-74.1/src/structurefinder/p4pfile/p4p_reader.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/pg8000/__init__.py` & `structurefinder-74.1/src/structurefinder/pg8000/__init__.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/pg8000/core.py` & `structurefinder-74.1/src/structurefinder/pg8000/core.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/pymatgen/core/lattice.py` & `structurefinder-74.1/src/structurefinder/pymatgen/core/lattice.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/pymatgen/util/num_utils.py` & `structurefinder-74.1/src/structurefinder/pymatgen/util/num_utils.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/searcher/compare.py` & `structurefinder-74.1/src/structurefinder/searcher/compare.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/searcher/constants.py` & `structurefinder-74.1/src/structurefinder/searcher/constants.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/searcher/database_handler.py` & `structurefinder-74.1/src/structurefinder/searcher/database_handler.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/searcher/filecrawler.py` & `structurefinder-74.1/src/structurefinder/searcher/filecrawler.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/searcher/fileparser.py` & `structurefinder-74.1/src/structurefinder/searcher/fileparser.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/searcher/misc.py` & `structurefinder-74.1/src/structurefinder/searcher/misc.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/searcher/spinner.py` & `structurefinder-74.1/src/structurefinder/searcher/spinner.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/searcher/unitcell.py` & `structurefinder-74.1/src/structurefinder/searcher/unitcell.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/searcher/worker.py` & `structurefinder-74.1/src/structurefinder/searcher/worker.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/shelxfile/atoms.py` & `structurefinder-74.1/src/structurefinder/shelxfile/atoms.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/shelxfile/cards.py` & `structurefinder-74.1/src/structurefinder/shelxfile/cards.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/shelxfile/dsrmath.py` & `structurefinder-74.1/src/structurefinder/shelxfile/dsrmath.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/shelxfile/elements.py` & `structurefinder-74.1/src/structurefinder/shelxfile/elements.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/shelxfile/misc.py` & `structurefinder-74.1/src/structurefinder/shelxfile/misc.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/src/structurefinder/shelxfile/shelx.py` & `structurefinder-74.1/src/structurefinder/shelxfile/shelx.py`

 * *Files identical despite different names*

### Comparing `structurefinder-74/.gitignore` & `structurefinder-74.1/.gitignore`

 * *Files identical despite different names*

### Comparing `structurefinder-74/LICENSE` & `structurefinder-74.1/LICENSE`

 * *Files identical despite different names*

### Comparing `structurefinder-74/pyproject.toml` & `structurefinder-74.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
-[project]
-name = "structurefinder"
-dynamic = ["version", "dependencies"]
-
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
 
+[project]
+name = "structurefinder"
+dynamic = ["version", "dependencies"]
 authors = [
     { name = "Daniel Kratzert", email = "dkratzert@gmx.de" },
 ]
 description = "Search X-ray structures on your hard drive"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -26,15 +25,15 @@
 
 [project.urls]
 "Homepage" = "https://dkratzert.de/structurefinder.html"
 "Bug Tracker" = "https://github.com/dkratzert/StructureFinder/issues"
 
 [tool.hatch.version]
 path = "src/structurefinder/misc/version.py"
-pattern = "VERSION\\s*=\\s*(?P<version>\\d+)"
+pattern = "VERSION\\s*=\\s*(?P<version>\\d+\\.\\d{0,1})"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     "/.github",
     "/pictures",
     "/scripts",
     "/setup",
```

