# Comparing `tmp/redturtle.prenotazioni-2.0.0.dev0.tar.gz` & `tmp/redturtle.prenotazioni-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.prenotazioni-2.0.0.dev0.tar", last modified: Mon Jun 12 12:35:42 2023, max compression
+gzip compressed data, was "redturtle.prenotazioni-2.0.0.dev1.tar", last modified: Mon Jun 12 13:12:19 2023, max compression
```

## Comparing `redturtle.prenotazioni-2.0.0.dev0.tar` & `redturtle.prenotazioni-2.0.0.dev1.tar`

### file list

```diff
@@ -1,283 +1,283 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      748 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/APP_IO.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6585 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       79 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      110 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    24194 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16268 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      164 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/TODO.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/constraints-5.2.x.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       27 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/constraints.txt
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7921 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      476 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/requirements-6.0.x.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       48 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/requirements.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      344 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3275 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2297 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2132 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/mail.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5157 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/booker.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4573 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4440 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/conflict.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/slot.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6903 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/stringinterp.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1779 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/add_edit_view.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1816 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/base.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7801 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      541 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/custom_radio_input.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4782 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/delete_reservation.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      674 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/folderfactories.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      155 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/overrides/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/overrides/.gitkeep
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3168 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    14679 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_add.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6920 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_move.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2038 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_print.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    30483 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1736 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11366 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_search.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/.gitkeep
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      364 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/calendar-add.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      503 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/calendar-icon.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      266 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/cross-icon.png
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9794 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1600 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      922 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/times-solid.png
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2108 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2377 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
--rw-rw-r--   0 mauro     (1000) mauro     (1000)   342590 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      148 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4616 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4486 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1059 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2718 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1555 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      103 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1507 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1261 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/index.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/utils/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      941 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      298 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      614 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3862 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/booking_stats.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      575 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2809 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5466 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2300 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       42 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/nofollow.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8165 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    10429 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    15258 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2266 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5916 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4895 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1892 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/week.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      333 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9540 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/vacations.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1524 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/viewlets.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    10867 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/week.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1193 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/widget.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6310 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      383 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/config.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2327 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1785 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/pause.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7355 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_day.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16926 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_folder.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_week.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_year.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8119 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/validators.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2080 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      214 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/handlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6160 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1567 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/events_logger.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      835 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1189 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/prenotazioni_folder.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      211 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      832 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/searchable_text.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1191 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexes.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    35726 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/it/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    45854 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      830 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/manual.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    35854 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1618 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/update.sh
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/monkeypatcher/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/monkeypatcher/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      499 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1282 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/permissions.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/prenotazione_event.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2345 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/actions.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      192 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6189 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/contentrules.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/metadata.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5093 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1980 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      914 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1645 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3551 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3811 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3094 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3795 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3796 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      564 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7373 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7623 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/to_1402/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1381 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/to_1500/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      196 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/to_1500/types.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/registry/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      412 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      123 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      199 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      309 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3328 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      559 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      162 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4469 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/add.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1152 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/delete.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1166 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking_schema/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      409 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4198 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/bookings/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      279 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1926 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/bookings/search.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      308 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/month_slots/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/month_slots/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      395 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/month_slots/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1848 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/month_slots/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2998 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6955 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/app_io.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5302 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/README.md
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      246 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8614 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1034 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/cli.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    16384 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/io.db
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       45 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/io_tools.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1945 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/monkey.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2825 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    27521 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/storage.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1062 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3197 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6283 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_booking_info.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_booking_schema.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8293 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_delete_booking.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9673 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9236 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_month_slots.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5762 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_prenotazione.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5913 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     8811 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3536 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    12116 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6301 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/upgrades.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2798 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/upgrades.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/dateutils.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1119 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/urls.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      472 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/app_io.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/templates/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      957 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/templates/app_io.pt
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1096 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      607 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/gates.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1010 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      598 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/review_states.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1696 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/tipologies.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1054 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2549 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_months.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1367 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    24194 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    12223 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      179 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      748 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/APP_IO.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6585 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       79 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      110 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    24194 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16268 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      164 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/TODO.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/constraints-5.2.x.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       27 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/constraints.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7921 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      476 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/requirements-6.0.x.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       48 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/requirements.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      344 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3275 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2297 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2132 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/mail.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5157 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/booker.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4573 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4440 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/conflict.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/slot.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6903 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/stringinterp.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1779 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/add_edit_view.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1816 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/base.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7801 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      541 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/custom_radio_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4782 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/delete_reservation.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      674 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/folderfactories.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      155 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/overrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/overrides/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3168 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    14679 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_add.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6920 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_move.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2038 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_print.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    30483 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1736 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    11366 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_search.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      364 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/calendar-add.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      503 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/calendar-icon.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      266 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/cross-icon.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9794 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1600 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      922 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/times-solid.png
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2108 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2377 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)   342590 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      148 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4616 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4486 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1059 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2718 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1555 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      103 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1507 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1261 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/index.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/utils/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      941 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      298 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      614 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3862 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/booking_stats.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      575 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2809 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5466 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2300 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       42 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/nofollow.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8165 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10429 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    15258 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2266 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5916 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4895 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1892 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/week.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      333 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9540 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/vacations.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1524 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/viewlets.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10867 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/week.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1193 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/widget.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6310 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      383 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/config.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2327 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1785 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/pause.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7355 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_day.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16926 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_folder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_week.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_year.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8119 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/validators.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2080 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      214 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/handlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6160 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1567 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/events_logger.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      835 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1189 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/prenotazioni_folder.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      211 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      832 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/searchable_text.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1191 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexes.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    35726 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/it/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    45854 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      830 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/manual.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    35854 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1618 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/update.sh
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/monkeypatcher/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/monkeypatcher/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      499 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1282 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/permissions.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/prenotazione_event.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2345 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/actions.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      192 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6189 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/contentrules.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/metadata.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.525067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5093 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1980 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      914 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1645 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3551 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3811 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3094 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3795 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3796 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      564 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7373 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7623 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1402/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1381 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1500/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      196 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1500/types.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      412 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      123 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      199 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      309 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3328 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      559 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      162 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4469 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/add.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1152 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/delete.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1166 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      409 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4198 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      279 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1926 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      308 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      395 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1848 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2998 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6955 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/app_io.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5302 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/README.md
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      246 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8614 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1034 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/cli.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16384 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/io.db
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       45 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/io_tools.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1945 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/monkey.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2825 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    27521 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/storage.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1062 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3197 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6283 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_booking_info.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_booking_schema.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8293 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_delete_booking.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9673 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9236 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_month_slots.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5762 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5913 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8811 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3536 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12116 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6301 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/upgrades.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2798 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/upgrades.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/dateutils.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1119 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/urls.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      472 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/app_io.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/templates/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      957 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/templates/app_io.pt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.529067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1096 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      607 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/gates.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1010 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      598 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/review_states.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1696 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/tipologies.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1054 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2549 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_months.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1367 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 13:12:19.521067 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    24194 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12223 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      179 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-12 13:12:19.000000 redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/top_level.txt
```

### Comparing `redturtle.prenotazioni-2.0.0.dev0/APP_IO.txt` & `redturtle.prenotazioni-2.0.0.dev1/APP_IO.txt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/CHANGES.rst` & `redturtle.prenotazioni-2.0.0.dev1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Changelog
 =========
 
 
-2.0.0.dev0 (2023-06-12)
+2.0.0.dev1 (2023-06-12)
 -----------------------
 
 - Add Booking restapi
   [mamico]
 
 - Fix Plone6 compatibility.
   [cekk]
```

### Comparing `redturtle.prenotazioni-2.0.0.dev0/DEVELOP.rst` & `redturtle.prenotazioni-2.0.0.dev1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/LICENSE.GPL` & `redturtle.prenotazioni-2.0.0.dev1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/LICENSE.rst` & `redturtle.prenotazioni-2.0.0.dev1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/PKG-INFO` & `redturtle.prenotazioni-2.0.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -633,15 +633,15 @@
 - Daniele Andreotti, daniele.andreotti@redturtle.it
 
 
 Changelog
 =========
 
 
-2.0.0.dev0 (2023-06-12)
+2.0.0.dev1 (2023-06-12)
 -----------------------
 
 - Add Booking restapi
   [mamico]
 
 - Fix Plone6 compatibility.
   [cekk]
```

### Comparing `redturtle.prenotazioni-2.0.0.dev0/README.rst` & `redturtle.prenotazioni-2.0.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/docs/conf.py` & `redturtle.prenotazioni-2.0.0.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/setup.py` & `redturtle.prenotazioni-2.0.0.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.prenotazioni",
-    version="2.0.0.dev0",
+    version="2.0.0.dev1",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/__init__.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/mail.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/actions/mail.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/booker.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/booker.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/conflict.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/conflict.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/slot.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/stringinterp.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/add_edit_view.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/add_edit_view.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/base.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/base.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/custom_radio_input.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/custom_radio_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/delete_reservation.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/delete_reservation.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/folderfactories.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_add.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_move.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_print.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazione_print.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_search.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/times-solid.png` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/times-solid.png`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/index.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/index.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/booking_stats.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/booking_stats.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/stats/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/week.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/templates/week.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/vacations.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/vacations.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/viewlets.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/week.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/week.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/widget.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/pause.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/pause.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_folder.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/validators.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/content/validators.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/events_logger.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/events_logger.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/prenotazioni_folder.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/events/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/searchable_text.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexers/searchable_text.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexes.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/indexes.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/interfaces.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/manual.pot` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/update.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/permissions.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/permissions.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/actions.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/contentrules.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/contentrules.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/resources.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/add.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/add.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/delete.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/delete.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/get.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/bookings/search.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/bookings/search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/month_slots/get.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/month_slots/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/get.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/restapi/services/week_slots/get.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/app_io.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/app_io.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/README.md` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/api.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/cli.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/cli.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/io.db` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/io.db`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/monkey.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/storage.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/scripts/io_tools/storage.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/setuphandlers.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/testing.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_booking_info.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_booking_info.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_booking_schema.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_booking_schema.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_delete_booking.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_delete_booking.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_delete_booking_api.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_delete_booking_api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_month_slots.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_month_slots.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_setup.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_week_table_overrides.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/tests/test_week_table_overrides.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/upgrades.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/upgrades.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/upgrades.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/dateutils.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/dateutils.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/urls.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/utilities/urls.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/templates/app_io.pt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/viewlets/templates/app_io.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/gates.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/review_states.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/review_states.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/tipologies.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/tipologies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_months.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_months.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/PKG-INFO` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.prenotazioni
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: An add-on for Plone
 Home-page: https://github.com/redturtle/redturtle.prenotazioni
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.org/project/redturtle.prenotazioni
 Project-URL: Source, https://github.com/redturtle/redturtle.prenotazioni
@@ -633,15 +633,15 @@
 - Daniele Andreotti, daniele.andreotti@redturtle.it
 
 
 Changelog
 =========
 
 
-2.0.0.dev0 (2023-06-12)
+2.0.0.dev1 (2023-06-12)
 -----------------------
 
 - Add Booking restapi
   [mamico]
 
 - Fix Plone6 compatibility.
   [cekk]
```

### Comparing `redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/SOURCES.txt` & `redturtle.prenotazioni-2.0.0.dev1/src/redturtle.prenotazioni.egg-info/SOURCES.txt`

 * *Files identical despite different names*

