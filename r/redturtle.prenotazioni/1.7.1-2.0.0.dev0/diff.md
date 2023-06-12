# Comparing `tmp/redturtle.prenotazioni-1.7.1.tar.gz` & `tmp/redturtle.prenotazioni-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.prenotazioni-1.7.1.tar", last modified: Tue Mar 28 09:05:24 2023, max compression
+gzip compressed data, was "redturtle.prenotazioni-2.0.0.dev0.tar", last modified: Mon Jun 12 12:35:42 2023, max compression
```

## Comparing `redturtle.prenotazioni-1.7.1.tar` & `redturtle.prenotazioni-2.0.0.dev0.tar`

### file list

```diff
@@ -1,224 +1,283 @@
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.591958 redturtle.prenotazioni-1.7.1/
--rw-r--r--   0 roman      (502) staff       (20)      748 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/APP_IO.txt
--rw-r--r--   0 roman      (502) staff       (20)     5750 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/CHANGES.rst
--rw-r--r--   0 roman      (502) staff       (20)       79 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/CONTRIBUTORS.rst
--rw-r--r--   0 roman      (502) staff       (20)      586 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/DEVELOP.rst
--rw-r--r--   0 roman      (502) staff       (20)    18092 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/LICENSE.GPL
--rw-r--r--   0 roman      (502) staff       (20)      670 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/LICENSE.rst
--rw-r--r--   0 roman      (502) staff       (20)      110 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/MANIFEST.in
--rw-r--r--   0 roman      (502) staff       (20)    18280 2023-03-28 09:05:24.592184 redturtle.prenotazioni-1.7.1/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     6647 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/README.rst
--rw-r--r--   0 roman      (502) staff       (20)      164 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/TODO.txt
--rw-r--r--   0 roman      (502) staff       (20)      105 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/constraints-5.2.x.txt
--rw-r--r--   0 roman      (502) staff       (20)       27 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/constraints.txt
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.553022 redturtle.prenotazioni-1.7.1/docs/
--rw-r--r--   0 roman      (502) staff       (20)     7921 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/docs/conf.py
--rw-r--r--   0 roman      (502) staff       (20)       89 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/docs/index.rst
--rw-r--r--   0 roman      (502) staff       (20)      476 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/requirements-6.0.x.txt
--rw-r--r--   0 roman      (502) staff       (20)       48 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/requirements.txt
--rw-r--r--   0 roman      (502) staff       (20)      344 2023-03-28 09:05:24.592696 redturtle.prenotazioni-1.7.1/setup.cfg
--rw-r--r--   0 roman      (502) staff       (20)     3253 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/setup.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.543445 redturtle.prenotazioni-1.7.1/src/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.553271 redturtle.prenotazioni-1.7.1/src/redturtle/
--rw-r--r--   0 roman      (502) staff       (20)       80 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.558566 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/
--rw-r--r--   0 roman      (502) staff       (20)     2297 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.559253 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/actions/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/actions/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      166 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/actions/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     2132 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/actions/mail.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.561384 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     5418 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/booker.py
--rw-r--r--   0 roman      (502) staff       (20)     4758 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     4440 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/conflict.py
--rw-r--r--   0 roman      (502) staff       (20)     3372 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)      273 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
--rw-r--r--   0 roman      (502) staff       (20)     8479 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/slot.py
--rw-r--r--   0 roman      (502) staff       (20)     7627 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/stringinterp.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.565538 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1358 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/add_edit_view.py
--rw-r--r--   0 roman      (502) staff       (20)     1816 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/base.py
--rw-r--r--   0 roman      (502) staff       (20)     6439 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      541 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/custom_radio_input.pt
--rw-r--r--   0 roman      (502) staff       (20)     3962 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/delete_reservation.py
--rw-r--r--   0 roman      (502) staff       (20)      674 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/folderfactories.py
--rw-r--r--   0 roman      (502) staff       (20)      155 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.565758 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/overrides/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/overrides/.gitkeep
--rw-r--r--   0 roman      (502) staff       (20)     3168 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)    15415 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazione_add.py
--rw-r--r--   0 roman      (502) staff       (20)     6920 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazione_move.py
--rw-r--r--   0 roman      (502) staff       (20)     2038 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazione_print.py
--rw-r--r--   0 roman      (502) staff       (20)    28929 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
--rw-r--r--   0 roman      (502) staff       (20)     1736 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
--rw-r--r--   0 roman      (502) staff       (20)    11366 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazioni_search.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.567217 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/.gitkeep
--rw-r--r--   0 roman      (502) staff       (20)      364 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/calendar-add.png
--rw-r--r--   0 roman      (502) staff       (20)      503 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/calendar-icon.png
--rw-r--r--   0 roman      (502) staff       (20)      266 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/cross-icon.png
--rw-r--r--   0 roman      (502) staff       (20)     9794 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
--rw-r--r--   0 roman      (502) staff       (20)     2631 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
--rw-r--r--   0 roman      (502) staff       (20)      922 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/times-solid.png
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.568147 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/stats/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/stats/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      614 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
--rw-r--r--   0 roman      (502) staff       (20)     3862 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/stats/booking_stats.py
--rw-r--r--   0 roman      (502) staff       (20)      575 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/stats/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.570805 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/
--rw-r--r--   0 roman      (502) staff       (20)     2809 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
--rw-r--r--   0 roman      (502) staff       (20)     1860 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
--rw-r--r--   0 roman      (502) staff       (20)     7192 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
--rw-r--r--   0 roman      (502) staff       (20)     2300 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
--rw-r--r--   0 roman      (502) staff       (20)       42 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/nofollow.pt
--rw-r--r--   0 roman      (502) staff       (20)     7872 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
--rw-r--r--   0 roman      (502) staff       (20)    10429 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
--rw-r--r--   0 roman      (502) staff       (20)    14930 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
--rw-r--r--   0 roman      (502) staff       (20)     2266 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
--rw-r--r--   0 roman      (502) staff       (20)     6019 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
--rw-r--r--   0 roman      (502) staff       (20)     4895 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
--rw-r--r--   0 roman      (502) staff       (20)     1892 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/week.pt
--rw-r--r--   0 roman      (502) staff       (20)     9540 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/vacations.py
--rw-r--r--   0 roman      (502) staff       (20)    10867 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/week.py
--rw-r--r--   0 roman      (502) staff       (20)     6335 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
--rw-r--r--   0 roman      (502) staff       (20)      417 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/config.py
--rw-r--r--   0 roman      (502) staff       (20)     1765 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.572617 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1785 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/pause.py
--rw-r--r--   0 roman      (502) staff       (20)     6109 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)      367 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/prenotazioni_day.py
--rw-r--r--   0 roman      (502) staff       (20)    19003 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/prenotazioni_folder.py
--rw-r--r--   0 roman      (502) staff       (20)      276 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/prenotazioni_folder_container.py
--rw-r--r--   0 roman      (502) staff       (20)      371 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/prenotazioni_week.py
--rw-r--r--   0 roman      (502) staff       (20)      371 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/prenotazioni_year.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.573494 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/contentrules/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/contentrules/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     2080 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/contentrules/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      214 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/contentrules/handlers.py
--rw-r--r--   0 roman      (502) staff       (20)     6160 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.574654 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1567 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1860 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/events_logger.py
--rw-r--r--   0 roman      (502) staff       (20)      835 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/prenotazione.py
--rw-r--r--   0 roman      (502) staff       (20)     1189 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/prenotazioni_folder.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.575367 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/indexers/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/indexers/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      211 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/indexers/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      832 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/indexers/searchable_text.py
--rw-r--r--   0 roman      (502) staff       (20)     1119 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/indexes.py
--rw-r--r--   0 roman      (502) staff       (20)      400 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/interfaces.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.576355 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.545346 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/en/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.576582 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)    37211 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.545551 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/it/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.576902 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
--rw-r--r--   0 roman      (502) staff       (20)    42985 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
--rw-r--r--   0 roman      (502) staff       (20)      696 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni-manual.pot
--rw-r--r--   0 roman      (502) staff       (20)    33621 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
--rw-r--r--   0 roman      (502) staff       (20)     1585 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/update.py
--rwxr-xr-x   0 roman      (502) staff       (20)      503 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/update.sh
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.577368 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/monkeypatcher/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/monkeypatcher/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      499 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     1138 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/permissions.zcml
--rw-r--r--   0 roman      (502) staff       (20)      478 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/prenotazione_event.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.546677 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.579319 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/
--rw-r--r--   0 roman      (502) staff       (20)     2345 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/actions.xml
--rw-r--r--   0 roman      (502) staff       (20)      192 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
--rw-r--r--   0 roman      (502) staff       (20)      105 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/catalog.xml
--rw-r--r--   0 roman      (502) staff       (20)     4880 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/contentrules.xml
--rw-r--r--   0 roman      (502) staff       (20)      266 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/metadata.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.580047 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/registry/
--rw-r--r--   0 roman      (502) staff       (20)     5093 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
--rw-r--r--   0 roman      (502) staff       (20)      987 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
--rw-r--r--   0 roman      (502) staff       (20)      914 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
--rw-r--r--   0 roman      (502) staff       (20)     1441 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/rolemap.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.581477 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/
--rw-r--r--   0 roman      (502) staff       (20)     3551 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
--rw-r--r--   0 roman      (502) staff       (20)     3811 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
--rw-r--r--   0 roman      (502) staff       (20)     3181 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
--rw-r--r--   0 roman      (502) staff       (20)     3152 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolderContainer.xml
--rw-r--r--   0 roman      (502) staff       (20)     3795 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
--rw-r--r--   0 roman      (502) staff       (20)     3796 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
--rw-r--r--   0 roman      (502) staff       (20)      637 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.546551 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/workflows/
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.581702 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
--rw-r--r--   0 roman      (502) staff       (20)     7373 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.581929 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
--rw-r--r--   0 roman      (502) staff       (20)     7623 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
--rw-r--r--   0 roman      (502) staff       (20)      540 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/workflows.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.582245 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/uninstall/
--rw-r--r--   0 roman      (502) staff       (20)      132 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.582688 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/uninstall/registry/
--rw-r--r--   0 roman      (502) staff       (20)      412 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
--rw-r--r--   0 roman      (502) staff       (20)      123 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.583121 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      199 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.583515 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/serializers/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/serializers/__init__.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.584230 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      173 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      534 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
--rw-r--r--   0 roman      (502) staff       (20)      162 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.584452 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/services/
--rw-r--r--   0 roman      (502) staff       (20)      164 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/services/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.585073 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/services/week_slots/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/services/week_slots/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      392 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/services/week_slots/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)     2864 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/services/week_slots/get.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.585548 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     6955 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/app_io.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.588091 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/
--rw-r--r--   0 roman      (502) staff       (20)     5302 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/README.md
--rw-r--r--   0 roman      (502) staff       (20)      246 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     8614 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/api.py
--rw-r--r--   0 roman      (502) staff       (20)     1034 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/cli.py
--rw-r--r--   0 roman      (502) staff       (20)    16384 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/io.db
--rw-r--r--   0 roman      (502) staff       (20)       45 2023-03-28 09:05:23.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/io_tools.py
--rw-r--r--   0 roman      (502) staff       (20)     1945 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/monkey.py
--rw-r--r--   0 roman      (502) staff       (20)     2825 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py
--rw-r--r--   0 roman      (502) staff       (20)    27521 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml
--rw-r--r--   0 roman      (502) staff       (20)      961 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/storage.py
--rw-r--r--   0 roman      (502) staff       (20)      622 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/setuphandlers.py
--rw-r--r--   0 roman      (502) staff       (20)     1611 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/testing.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.588492 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/tests/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/tests/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     3081 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/tests/test_setup.py
--rw-r--r--   0 roman      (502) staff       (20)     5660 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/upgrades.py
--rw-r--r--   0 roman      (502) staff       (20)     1807 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/upgrades.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.588900 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/utilities/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/utilities/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)     1119 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/utilities/urls.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.589611 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/viewlets/
--rw-r--r--   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/viewlets/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      472 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/viewlets/app_io.py
--rw-r--r--   0 roman      (502) staff       (20)      593 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/viewlets/configure.zcml
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.589837 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/viewlets/templates/
--rw-r--r--   0 roman      (502) staff       (20)      957 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/viewlets/templates/app_io.pt
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.591752 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/
--rw-r--r--   0 roman      (502) staff       (20)       24 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/__init__.py
--rw-r--r--   0 roman      (502) staff       (20)      982 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/configure.zcml
--rw-r--r--   0 roman      (502) staff       (20)      607 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/gates.py
--rw-r--r--   0 roman      (502) staff       (20)     1010 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
--rw-r--r--   0 roman      (502) staff       (20)      598 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/review_states.py
--rw-r--r--   0 roman      (502) staff       (20)     1696 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/tipologies.py
--rw-r--r--   0 roman      (502) staff       (20)     1054 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
--rw-r--r--   0 roman      (502) staff       (20)     1367 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
-drwxr-xr-x   0 roman      (502) staff       (20)        0 2023-03-28 09:05:24.555699 redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/
--rw-r--r--   0 roman      (502) staff       (20)    18280 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/PKG-INFO
--rw-r--r--   0 roman      (502) staff       (20)     9280 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (502) staff       (20)      203 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/entry_points.txt
--rw-r--r--   0 roman      (502) staff       (20)       10 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
--rw-r--r--   0 roman      (502) staff       (20)        1 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/not-zip-safe
--rw-r--r--   0 roman      (502) staff       (20)      368 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/requires.txt
--rw-r--r--   0 roman      (502) staff       (20)       10 2023-03-28 09:05:24.000000 redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      748 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/APP_IO.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6585 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       79 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      586 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      110 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    24194 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16268 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      164 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/TODO.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/constraints-5.2.x.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       27 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/constraints.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7921 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      476 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/requirements-6.0.x.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       48 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/requirements.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      344 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3275 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2297 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2132 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/mail.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5157 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/booker.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4573 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4440 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/conflict.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/prenotazione_menu.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/slot.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6903 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/stringinterp.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1779 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/add_edit_view.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1816 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/base.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7801 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      541 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/custom_radio_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4782 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/delete_reservation.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      674 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/folderfactories.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      155 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/overrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/overrides/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3168 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    14679 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_add.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6920 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_move.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2038 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_print.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    30483 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1736 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    11366 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_search.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      364 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/calendar-add.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      503 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/calendar-icon.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      266 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/cross-icon.png
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9794 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1600 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      922 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/times-solid.png
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2108 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2377 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)   342590 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      148 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4616 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4486 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1059 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2718 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1555 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      103 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1507 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1261 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/index.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/utils/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      941 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      298 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      614 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3862 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/booking_stats.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      575 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2809 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5466 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2300 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       42 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/nofollow.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8165 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10429 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    15258 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2266 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5916 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4895 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1892 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/week.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      333 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9540 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/vacations.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1524 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/viewlets.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10867 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/week.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1193 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/widget.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6310 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      383 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/config.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2327 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1785 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/pause.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7355 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_day.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16926 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_folder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_week.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      371 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_year.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8119 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/validators.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2080 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      214 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/handlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6160 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1567 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1860 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/events_logger.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      835 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1189 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/prenotazioni_folder.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      211 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      832 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/searchable_text.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1191 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexes.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    35726 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/it/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    45854 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      830 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/manual.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    35854 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1618 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/update.sh
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/monkeypatcher/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/monkeypatcher/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      499 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/monkeypatcher/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1282 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/permissions.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      478 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/prenotazione_event.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2345 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/actions.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      192 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6189 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/contentrules.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/metadata.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5093 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1980 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/resources.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      914 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1645 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3551 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3811 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3094 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3795 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3796 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      564 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.040393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7373 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7623 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/to_1402/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1381 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/to_1500/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      196 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/to_1500/types.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      412 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      123 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      199 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      309 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3328 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      559 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      162 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4469 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/add.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1015 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1152 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/delete.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1166 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking_schema/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      409 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4198 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/bookings/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      279 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1926 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/bookings/search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      308 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/month_slots/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/month_slots/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      395 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/month_slots/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1848 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/month_slots/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2998 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6955 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/app_io.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5302 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/README.md
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      246 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8614 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1034 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/cli.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    16384 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/io.db
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       45 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/io_tools.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1945 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/monkey.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2825 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    27521 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      961 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/storage.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1062 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3197 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6283 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_booking_info.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8479 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_booking_schema.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8293 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_delete_booking.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9673 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_delete_booking_api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9236 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_month_slots.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5762 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_prenotazione.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5913 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     8811 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3536 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12116 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_week_table_overrides.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6301 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/upgrades.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2798 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/upgrades.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.048393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/dateutils.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1119 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/urls.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      472 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/app_io.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      593 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/templates/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      957 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/templates/app_io.pt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.052393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1096 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      607 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/gates.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1010 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      598 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/review_states.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1696 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/tipologies.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1054 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2549 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_months.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1367 2023-06-12 12:35:41.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-12 12:35:42.044393 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    24194 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    12223 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      179 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      392 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       10 2023-06-12 12:35:42.000000 redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/top_level.txt
```

### Comparing `redturtle.prenotazioni-1.7.1/APP_IO.txt` & `redturtle.prenotazioni-2.0.0.dev0/APP_IO.txt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/CHANGES.rst` & `redturtle.prenotazioni-2.0.0.dev0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,50 @@
 Changelog
 =========
 
 
+2.0.0.dev0 (2023-06-12)
+-----------------------
+
+- Add Booking restapi
+  [mamico]
+
+- Fix Plone6 compatibility.
+  [cekk]
+
+- Removed unused type PrenotazioniFolderContainer.
+  [cekk]
+
+- Added endpoint to get booking schema.
+  [daniele]
+
+- Avoid change gate, booking date, booking end from /edit;
+  this would allow you to skip the checks;
+  Fix profile registration name;
+  [lucabel]
+
+- Add @bookings endpoint to get booking items for a user
+  [foxtrot-dfm1]
+
+- Add a new endpoint to get booking details. (#40442).
+  [daniele]
+  
+- Add autoconfirm content rule to profile.
+  [foxtrot-dfm1]
+
+- Added field "cosa_serve" (#40445).
+  [daniele]
+
+- Refactor booking delete machinery and remove unused token.
+  [cekk]
+
+- Add DELETE endpoint for booking.
+- Add new field that allows to override week schedule for a certain date range.
+  [cekk]
+
 1.7.1 (2023-03-28)
 ------------------
 
 - Add plone5 profile to setup.
   [foxtrot-dfm1]
```

### Comparing `redturtle.prenotazioni-1.7.1/DEVELOP.rst` & `redturtle.prenotazioni-2.0.0.dev0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/LICENSE.GPL` & `redturtle.prenotazioni-2.0.0.dev0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/LICENSE.rst` & `redturtle.prenotazioni-2.0.0.dev0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/docs/conf.py` & `redturtle.prenotazioni-2.0.0.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/setup.py` & `redturtle.prenotazioni-2.0.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.prenotazioni",
-    version="1.7.1",
+    version="2.0.0.dev0",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -73,22 +73,21 @@
             "plone.app.testing",
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
             "plone.testing>=5.0.0",
             "plone.app.contenttypes",
             "plone.app.robotframework[debug]",
+            "collective.MockMailHost",
         ],
         "app_io": [
             "bravado",
             "pytz",
         ],
-        "plone5": [
-            "collective.dexteritytextindexer"
-        ],
+        "plone5": ["collective.dexteritytextindexer"],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     [console_scripts]
     update_locale = redturtle.prenotazioni.locales.update:update_locale
     app_io = redturtle.prenotazioni.scripts.app_io:main
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/__init__.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/__init__.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/actions/mail.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/actions/mail.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/booker.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/booker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # -*- coding: utf-8 -*-
-from datetime import datetime
-from datetime import time
 from datetime import timedelta
 from DateTime import DateTime
 from plone import api
 from plone.memoize.instance import memoize
 from random import choice
 from redturtle.prenotazioni import logger
-from redturtle.prenotazioni.adapters.prenotazione import IDeleteTokenProvider
-from redturtle.prenotazioni.config import DELETE_TOKEN_KEY
 from redturtle.prenotazioni.config import VERIFIED_BOOKING
 from zope.annotation.interfaces import IAnnotations
 from zope.component import Interface
 from zope.interface import implementer
 
 
 class IBooker(Interface):
@@ -97,26 +93,26 @@
             type="Prenotazione",
             container=container,
             booking_expiration_date=booking_expiration_date,
             gate=gate,
             **params
         )
 
-        # set delete token
-        expiration = datetime.combine(obj.booking_date.date(), time(0, 0, 0))
-        token = IDeleteTokenProvider(obj).generate_token(expiration=expiration)
         annotations = IAnnotations(obj)
-        annotations[DELETE_TOKEN_KEY] = token.decode("utf-8")
 
         annotations[VERIFIED_BOOKING] = False
         if not api.user.is_anonymous():
             user = api.user.get_current()
             data_fiscalcode = getattr(obj, "fiscalcode", "") or ""
             fiscalcode = data_fiscalcode.upper()
-            if user.hasProperty("fiscalcode") and fiscalcode:
+            if not fiscalcode:
+                obj.fiscalcode = (
+                    user.getProperty("fiscalcode", "") or user.getId() or ""
+                ).upper()  # noqa
+            elif user.hasProperty("fiscalcode") and fiscalcode:
                 if (user.getProperty("fiscalcode") or "").upper() == fiscalcode:
                     logger.info("Booking verified: {}".format(obj.absolute_url()))
                     annotations[VERIFIED_BOOKING] = True
 
         obj.reindexObject()
         api.content.transition(obj, "submit")
         return obj
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/configure.zcml`

 * *Files 5% similar despite different names*

```diff
@@ -23,20 +23,14 @@
   <adapter
       factory=".slot.Slot"
       provides=".slot.ISlot"
       for="redturtle.prenotazioni.content.prenotazione.IPrenotazione"
       />
 
   <adapter
-      factory=".prenotazione.DeleteToken"
-      provides=".prenotazione.IDeleteTokenProvider"
-      for="redturtle.prenotazioni.content.prenotazione.IPrenotazione"
-      />
-
-  <adapter
       factory=".slot.Slot"
       provides=".slot.ISlot"
       for="redturtle.prenotazioni.interfaces.IPause"
       />
 
   <!-- stringinterp -->
   <adapter
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/conflict.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/conflict.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/slot.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/slot.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/adapters/stringinterp.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/adapters/stringinterp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # -*- coding: utf-8 -*-
 from plone.stringinterp.adapters import BaseSubstitution
 from redturtle.prenotazioni import _
 from redturtle.prenotazioni import logger
-from redturtle.prenotazioni.config import DELETE_TOKEN_KEY
-from zope.annotation.interfaces import IAnnotations
 from zope.component import adapter
 from zope.interface import Interface
 
 
 try:
     from plone.app.event.base import spell_date
 
@@ -111,29 +109,21 @@
         return "{folder}/@@prenotazione_print?uid={uid}".format(
             folder=self.context.getPrenotazioniFolder().absolute_url(),
             uid=self.context.UID(),
         )
 
 
 @adapter(Interface)
-class BookingPrintUrlWithDeleteTokenSubstitution(BaseSubstitution):
-    category = _("Booking")
-    description = _("The booking print url with delete token.")
+class BookingPrintUrlWithDeleteTokenSubstitution(BookingUrlSubstitution):
+    """
+    This is a backward compatibility with old version with token
+    """
 
-    def safe_call(self):
-        annotations = IAnnotations(self.context)
-        token = annotations.get(DELETE_TOKEN_KEY, None)
-        if not token:
-            return ""
-        return "{folder}/@@prenotazione_print?uid={uid}&{delete_token_key}={token}".format(  # noqa
-            folder=self.context.getPrenotazioniFolder().absolute_url(),
-            uid=self.context.UID(),
-            delete_token_key=DELETE_TOKEN_KEY,
-            token=token,
-        )
+    category = _("Booking")
+    description = _("[DEPRECATED] The booking print url with delete token.")
 
 
 @adapter(Interface)
 class BookingUserPhoneSubstitution(BaseSubstitution):
     category = _("Booking")
     description = _("The phone number of the user who made the reservation.")
 
@@ -233,18 +223,11 @@
 
 @adapter(Interface)
 class BookingUrlWithDeleteToken(BaseSubstitution):
     category = _("Booking")
     description = _("The booking url with delete token")
 
     def safe_call(self):
-        annotations = IAnnotations(self.context)
-        token = annotations.get(DELETE_TOKEN_KEY, None)
-        if not token:
-            return ""
-
-        return "{booking_url}/@@delete_reservation?uid={uid}&{delete_token_key}={token}".format(
+        return "{booking_url}/@@delete_reservation?uid={uid}".format(
             booking_url=self.context.getPrenotazioniFolder().absolute_url(),
-            delete_token_key=DELETE_TOKEN_KEY,
             uid=self.context.UID(),
-            token=token,
         )
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/base.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/base.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/configure.zcml`

 * *Files 21% similar despite different names*

```diff
@@ -85,23 +85,29 @@
       permission="zope2.View"
       />
 
   <browser:page
       name="prenotazioni_search"
       for="..content.prenotazioni_folder.IPrenotazioniFolder"
       class=".prenotazioni_search.WrappedSearchForm"
-      permission="zope.Public"
+      permission="zope2.View"
       />
 
   <browser:page
       name="delete_reservation"
       for="..content.prenotazioni_folder.IPrenotazioniFolder"
       class=".delete_reservation.DeleteReservation"
       template="templates/delete_reservation.pt"
-      permission="zope.Public"
+      permission="zope2.View"
+      />
+  <browser:page
+      name="confirm-delete"
+      for="..content.prenotazioni_folder.IPrenotazioniFolder"
+      class=".delete_reservation.ConfirmDelete"
+      permission="zope2.View"
       />
 
   <browser:page
       name="vacation-booking-show"
       for="..content.prenotazioni_folder.IPrenotazioniFolder"
       class=".vacations.VacationBookingShow"
       permission="cmf.ModifyPortalContent"
@@ -223,8 +229,46 @@
   <browser:page
       name="download_reservation"
       for="*"
       class=".prenotazioni_search.DownloadReservation"
       permission="redturtle.prenotazioni.SearchPrenotazioni"
       />
 
+  <!-- define new widget -->
+  <class class=".widget.WeekTableOverridesWidget">
+    <require
+        permission="zope.Public"
+        interface=".widget.IWeekTableOverridesWidget"
+        />
+  </class>
+
+  <adapter
+      factory=".widget.WeekTableOverridesFieldWidget"
+      for="*
+           z3c.form.interfaces.IFormLayer"
+      />
+
+  <z3c:widgetTemplate
+      widget=".widget.IWeekTableOverridesWidget"
+      template="templates/week_table_overrides_widget_input.pt"
+      layer="z3c.form.interfaces.IFormLayer"
+      mode="input"
+      />
+
+  <browser:viewlet
+      name="redturtle.prenotazioni.headviewlet"
+      manager="plone.app.layout.viewlets.interfaces.IHtmlHead"
+      class=".viewlets.HeadViewlet"
+      permission="zope2.View"
+      layer="redturtle.prenotazioni.interfaces.IRedturtlePrenotazioniLayer"
+      />
+
+  <browser:viewlet
+      name="redturtle.prenotazioni.overrideswidget"
+      view=".viewlets.IHasTableOverridesMarker"
+      manager="plone.app.layout.viewlets.interfaces.IHtmlHead"
+      class=".viewlets.HasTableOverridesWidget"
+      permission="zope2.View"
+      layer="redturtle.prenotazioni.interfaces.IRedturtlePrenotazioniLayer"
+      />
+
 </configure>
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/custom_radio_input.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/custom_radio_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/folderfactories.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/folderfactories.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazione_add.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_add.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
-from datetime import timedelta
-from DateTime import DateTime
 from email.utils import formataddr
 from email.utils import parseaddr
 from os import environ
 from plone import api
 from plone.memoize.view import memoize
 from plone.registry.interfaces import IRegistry
 from plone.z3cform.layout import wrap_form
 from Products.CMFPlone.interfaces.controlpanel import IMailSchema
 from redturtle.prenotazioni import _
-from redturtle.prenotazioni import tznow
 from redturtle.prenotazioni.adapters.booker import IBooker
 from redturtle.prenotazioni.browser.week import TIPOLOGIA_PRENOTAZIONE_NAME_COOKIE
 from redturtle.prenotazioni.browser.z3c_custom_widget import CustomRadioFieldWidget
-from redturtle.prenotazioni.config import DELETE_TOKEN_KEY
 from redturtle.prenotazioni.config import REQUIRABLE_AND_VISIBLE_FIELDS
 from redturtle.prenotazioni.content.prenotazione import IPrenotazione
 from redturtle.prenotazioni.utilities.urls import urlify
+from redturtle.prenotazioni.utilities.dateutils import exceedes_date_limit
 from six.moves.urllib.parse import parse_qs
 from six.moves.urllib.parse import urlparse
 from z3c.form import button
 from z3c.form import field
 from z3c.form import form
 from z3c.form.interfaces import HIDDEN_MODE
 from z3c.form.interfaces import WidgetActionExecutionError
-from zope.annotation.interfaces import IAnnotations
 from zope.component import getUtility
 from zope.i18n import translate
 from zope.interface import implementer
 from zope.interface import Invalid
 from zope.schema import Text
 from zope.schema import TextLine
 from zope.schema.interfaces import IVocabularyFactory
 
+import pytz
 
 DEFAULT_REQUIRED_FIELDS = []
 
 
 class IAddForm(IPrenotazione):
 
     """
@@ -148,15 +145,15 @@
             return ""
         localized_date = self.localized_time(booking_date)
         return _(
             "label_selected_date",
             "Selected date: ${date} — Time: ${slot}",
             mapping={
                 "date": localized_date,
-                "slot": booking_date.asdatetime().strftime("%H:%M"),
+                "slot": booking_date.strftime("%H:%M"),
             },
         )
 
     @property
     @memoize
     def description(self):
         """
@@ -172,21 +169,17 @@
         """
         booking_date = self.request.form.get("form.booking_date", None)
         if not booking_date:
             booking_date = self.request.form.get("form.widgets.booking_date", None)
 
         if not booking_date:
             return None
-        tzname = self.get_timezone()
 
-        if len(booking_date) == 16:
-            if tzname == "RMT":
-                tzname = "CEST"
-            booking_date = " ".join((booking_date, tzname))
-        return DateTime(booking_date)
+        booking_date = datetime.fromisoformat(booking_date)
+        return pytz.timezone(self.get_timezone()).localize(booking_date)
 
     def get_timezone(self):
         """
         get from environment vars or site settings
         """
         tz = environ.get("TZ", "")
         if tz:
@@ -237,25 +230,15 @@
     def exceedes_date_limit(self, data):
         """
         Check if we can book this slot or is it too much in the future.
         """
         future_days = self.context.getFutureDays()
         if not future_days:
             return False
-        booking_date = data.get("booking_date", None)
-        if not isinstance(booking_date, datetime):
-            return False
-        date_limit = tznow() + timedelta(future_days)
-        if not booking_date.tzinfo:
-            tzinfo = date_limit.tzinfo
-            if tzinfo:
-                booking_date = tzinfo.localize(booking_date)
-        if booking_date <= date_limit:
-            return False
-        return True
+        return exceedes_date_limit(data, future_days)
 
     @button.buttonAndHandler(_("action_book", "Book"))
     def action_book(self, action):
         """
         Book this resource
         """
         data, errors = self.extractData()
@@ -292,19 +275,17 @@
             api.portal.show_message(message=msg, type="warning", request=self.request)
             target = self.back_to_booking_url
             return self.request.response.redirect(target)
         msg = _("booking_created")
         api.portal.show_message(message=msg, type="info", request=self.request)
         booking_date = data["booking_date"].strftime("%d/%m/%Y")
 
-        delete_token = IAnnotations(obj).get(DELETE_TOKEN_KEY, "")
         params = {
             "data": booking_date,
             "uid": obj.UID(),
-            "delete_token": delete_token,
         }
         target = urlify(
             self.context.absolute_url(),
             paths=["@@prenotazione_print"],
             params=params,
         )
         self.send_email_to_managers(booking=obj)
@@ -333,15 +314,15 @@
         """Redirects the user to the target, optionally with a portal message"""
         if msg:
             self.show_message(msg, msg_type)
         return self.request.response.redirect(target)
 
     def has_enough_time(self):
         """Check if we have enough time to book something"""
-        booking_date = self.booking_DateTime.asdatetime()
+        booking_date = self.booking_DateTime
         return self.prenotazioni.is_booking_date_bookable(booking_date)
 
     def __call__(self):
         """Redirects to the context if no data is found in the request"""
         # we should always have a booking date
         if not self.booking_DateTime:
             msg = _("please_pick_a_date", "Please select a time slot")
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazione_move.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_move.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazione_print.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazione_print.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_context_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,41 @@
 from redturtle.prenotazioni.config import PAUSE_PORTAL_TYPE
 from redturtle.prenotazioni.config import PAUSE_SLOT
 from redturtle.prenotazioni.content.pause import Pause
 from redturtle.prenotazioni.utilities.urls import urlify
 from six.moves import map
 from six.moves import range
 
+import json
 import six
 
 
 def hm2handm(hm):
     """This is a utility function that will return the hour and date of day
     to the value passed in the string hm
 
     :param hm: a string in the format "%H%m"
+
+    XXX: manage the case of `hm` as tuple, eg. ("0700", )
     """
+    if hm and isinstance(hm, tuple):
+        hm = hm[0]
     if (not hm) or (not isinstance(hm, six.string_types)) or (len(hm) != 4):
         raise ValueError(hm)
     return (hm[:2], hm[2:])
 
 
 def hm2DT(day, hm):
     """This is a utility function that will return the hour and date of day
     to the value passed in the string hm
 
     :param day: a datetime date
     :param hm: a string in the format "%H%m"
     """
-    if not hm:
+    if not hm or hm == "--NOVALUE--" or hm == ("--NOVALUE--",):
         return None
     date = day.strftime("%Y/%m/%d")
     h, m = hm2handm(hm)
     tzone = DateTime().timezone()
     return DateTime("%s %s:%s %s" % (date, h, m, tzone))
 
 
@@ -187,25 +192,55 @@
                 return True
         return False
 
     @memoize
     def is_configured_day(self, day):
         """Returns True if the day has been configured"""
         weekday = day.weekday()
-        week_table = getattr(self.context, "week_table", {})
+        week_table = self.get_week_table(day=day)
         day_table = week_table[weekday]
         return any(
             (
                 day_table["morning_start"],
                 day_table["morning_end"],
                 day_table["afternoon_start"],
                 day_table["afternoon_end"],
             )
         )
 
+    def get_week_table(self, day):
+        week_table = getattr(self.context, "week_table", {})
+        week_table_overrides = json.loads(
+            getattr(self.context, "week_table_overrides", "[]") or "[]"
+        )
+        if not week_table_overrides:
+            return week_table
+
+        for override in week_table_overrides:
+            from_month = int(override.get("from_month", ""))
+            from_day = int(override.get("from_day", ""))
+            to_month = int(override.get("to_month", ""))
+            to_day = int(override.get("to_day", ""))
+            toYear = day.year
+
+            if from_month > to_month:
+                # next year
+                toYear += 1
+
+            fromDate = date(day.year, from_month, from_day)
+            toDate = date(toYear, to_month, to_day)
+
+            if isinstance(day, datetime):
+                if fromDate <= day.date() <= toDate:
+                    return override["week_table"]
+            else:
+                if fromDate <= day <= toDate:
+                    return override["week_table"]
+        return week_table
+
     def is_before_allowed_period(self, day):
         """Returns True if the day is before the first bookable day"""
         date_limit = self.minimum_bookable_date
         if not date_limit:
             return False
         if day <= date_limit.date():
             return True
@@ -276,17 +311,17 @@
             if day > self.maximum_bookable_date.date():
                 return []
         date = day.strftime("%Y-%m-%d")
         params = self.remembered_params.copy()
         times = slot.get_values_hr_every(300, slot_min_size=slot_min_size)
         base_url = self.base_booking_url
         urls = []
-        now_str = tznow().strftime("%Y-%m-%d %H:%M")
+        now_str = tznow().strftime("%Y-%m-%dT%H:%M")
         for t in times:
-            form_booking_date = " ".join((date, t))
+            form_booking_date = "T".join((date, t))
             params["form.booking_date"] = form_booking_date
             if gate:
                 params["gate"] = gate
             booking_date = DateTime(params["form.booking_date"]).asdatetime()  # noqa
             urls.append(
                 {
                     "title": t,
@@ -441,15 +476,15 @@
         busy = set(self.get_busy_gates_in_slot(booking_date, booking_end_date))
         return available - busy
 
     @memoize
     def get_day_intervals(self, day):
         """Return the time ranges of this day"""
         weekday = day.weekday()
-        week_table = getattr(self.context, "week_table", {})
+        week_table = self.get_week_table(day=day)
         day_table = week_table[weekday]
         # Convert hours to DateTime
         morning_start = hm2DT(day, day_table["morning_start"])
         morning_end = hm2DT(day, day_table["morning_end"])
         afternoon_start = hm2DT(day, day_table["afternoon_start"])
         afternoon_end = hm2DT(day, day_table["afternoon_end"])
         # Get's the daily schedule
@@ -651,15 +686,16 @@
             if slot.context.portal_type == PAUSE_PORTAL_TYPE:
                 for gate in self.get_gates():
                     slots_by_gate.setdefault(gate, []).append(slot)
             else:
                 slots_by_gate.setdefault(slot.gate, []).append(slot)
         return slots_by_gate
 
-    @memoize
+    # TODO: perchè memozie qui ?
+    # @memoize
     def get_free_slots(self, booking_date, period="day"):
         """This will return the free slots divided by gate
 
         :param booking_date: a datetime object
         :param period: a string
         :return: a dictionary like:
         {'gate1': [slot1],
@@ -734,27 +770,35 @@
 
         @return a dict like this:
         {'booking_type1': 10,
          'booking_type2': 20,
          ...
         }
         """
-        return dict(
-            (x["name"], int(x["duration"]))
-            for x in getattr(self.context, "booking_types", [])
-        )
+
+        def get_duration(duration):
+            if isinstance(duration, tuple):
+                return int(duration[0])
+            return int(duration)
+
+        return {
+            typ["name"]: get_duration(typ["duration"])
+            for typ in getattr(self.context, "booking_types", [])
+            if typ["duration"]
+        }
 
     def get_booking_type_duration(self, booking_type):
         """Return the seconds for this booking_type"""
         if isinstance(booking_type, dict):
             return int(booking_type["duration"]) * 60
         if isinstance(booking_type, six.string_types) and not isinstance(
             booking_type, six.text_type
         ):
             booking_type = booking_type
+        # XXX: se il booking_type non esiste, ritorna 1 minuto, è corretto ????
         return self.booking_type_durations.get(booking_type, 1)
 
     @memoize
     def booking_types_bookability(self, booking_date):
         """
         :param  booking_date: a datetime object
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/prenotazioni_search.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/prenotazioni_search.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/redturtle-reservation.css`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/static/times-solid.png` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/static/times-solid.png`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/stats/booking_stats.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/booking_stats.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/stats/booking_stats.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/booking_stats.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/stats/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/stats/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/delete_reservation.pt`

 * *Files 22% similar despite different names*

```diff
@@ -14,43 +14,18 @@
     </head>
     <body>
 
         <metal:content fill-slot="main"
                        tal:define="prenotazione nocall:view/prenotazione;
                                    toLocalizedTime nocall:context/@@plone/toLocalizedTime"
         >
-        <tal:no_prenotazione tal:condition="not:prenotazione">
             <div tabindex="0">
-                <h1 i18n:translate="damn"></h1>
-                <p class="documentFirstHeading" tal:content="view/no_reservation_label">
-                    Seems we are not able to find your reservation
-                </p>
-            </div>
-        </tal:no_prenotazione>
-        <tal:prenotazione tal:condition="prenotazione">
-            <div tabindex="0" tal:condition="view/deleted_procedure_ended">
-                <tal:not_delete tal:condition="not:view/reservation_deleted">
-                    <h1 class="documentFirstHeading" i18n:translate="">
-                        Is not possible to delete your reservation
-                    </h1>
-                    <p i18n:translate="">
-                        It's not possbile to delete your reservation. The url is broken or it's to late to delete it
-                    </p>
-                </tal:not_delete>
-                <h1 class="documentFirstHeading" tal:condition="view/reservation_deleted" tal:content="view/deleted_label">
-                    Your booking has been deleted
-                </h1>
-            </div>
-            <div tabindex="0" tal:condition="not:view/deleted_procedure_ended">
                 <h1 class="documentFirstHeading" tal:content="view/label">
                 Booking request
                 </h1>
-                <!-- <div class="documentDescription" tal:content="view/description">
-                Booking description
-                </div> -->
                 <p>
                     Gentile <b tal:content="prenotazione/Title">Fullname</b>,
                     di seguito sono elencati i dati relativi alla sua prenotazione.<br/>
                     Verifichi se si tratta della prenotazione corretta e confermi la cancellazione.
                 </p>
                 <table class="listing">
                     <tbody>
@@ -114,23 +89,23 @@
                                 <b i18n:translate="label_booking_code">Booking code</b>
                             </td>
                             <td tal:content="prenotazione/getBookingCode"></td>
                         </tr>
                     </tbody>
                 </table>
             </div>
-        </tal:prenotazione>
         <div class="actions">
-            <div class="actions" tal:condition="python:view.deleted_procedure_ended or not prenotazione">
-                    <a title="Prenotazioni" href="prenotazioni" class="button btn btn-default"
-                    tal:attributes="href string:${context/absolute_url}?data=${request/data|nothing}">Ritorna alle prenotazioni</a>
-            </div>
-            <tal:not_deleted tal:condition="python:not view.deleted_procedure_ended and prenotazione">
-                <a tal:condition="request/delete_token|nothing"
-                    title="Cancella Prenotazione" href="delete" class="button btn btn-danger"
-                    tal:define="url string:${context/absolute_url}/@@delete_reservation?${request/QUERY_STRING}&confirm=True"
-                    tal:attributes="href python:view.protect_url(url)">Cancella questa prenotazione</a>
-            </tal:not_deleted>
+            <form action="${context/absolute_url}/confirm-delete"
+                  method="POST">
+                <span tal:replace="structure context/@@authenticator/authenticator"/>
+                <input type="hidden" id="uid" name="uid" value="${request/uid}" />
+                <input type="submit"
+                       tal:condition="prenotazione/canDeleteBooking"
+                       value="Cancella Prenotazione"
+                       id="delete"
+                       class="button btn btn-danger" />
+            </form>
+            
         </div>
         </metal:content>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,22 +1,14 @@
-
-Seems we are not able to find your reservation
-
-****** Is not possible to delete your reservation ******
-It's not possbile to delete your reservation. The url is broken or it's to late
-to delete it
-****** Your booking has been deleted ******
 ****** Booking request ******
 Gentile Fullname, di seguito sono elencati i dati relativi alla sua
 prenotazione.
 Verifichi se si tratta della prenotazione corretta e confermi la cancellazione.
 Booking type
 Email
 Phone number
 Company
 Fiscal code
 Subject
 Booking date   at
 Gate
 Booking code
-Ritorna_alle_prenotazioni
- Cancella_questa_prenotazione
+  [Cancella Prenotazione]
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/manager_notification_mail.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione.pt`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,18 @@
                     </tal:repeat>
                   </div>
                 </div>
                 <div class="field">
                     <strong i18n:translate="label_booking_code">Booking code</strong>:
                     <span tal:replace="here/getBookingCode" />
                 </div>
+                <div class="field" tal:define="cosa_serve python: here.getPrenotazioniFolder().getCosaServe()" tal:condition="cosa_serve">
+                    <strong i18n:translate="cosa_serve">Cosa serve</strong>:
+                    <span tal:replace="cosa_serve" />
+                </div>
                 <hr />
                 <p>&nbsp;</p>
                 <div class="field" tal:condition="not:not_ajax_load">
                   <a href=""
                      tal:attributes="href context_state/canonical_object_url">
                     <img width="16" height="16"
                          src="++resource++redturtle.prenotazioni.resources/calendar-icon.png"
```

#### html2text {}

```diff
@@ -12,14 +12,15 @@
 Subject:
 Booking date:
   at
 Gate: Gate no. 1
 Staff notes:
 text
 Booking code:
+Cosa serve:
 ===============================================================================
  
 [++resource++redturtle.prenotazioni.resources/calendar-icon.png] View booking
 [++resource++redturtle.prenotazioni.resources/calendar-icon.png]_Move_booking
 [${portal_url}/++plone++redturtle.prenotazioni/times-solid.png]_Reject_booking
 [++resource++redturtle.prenotazioni.resources/calendar-add.png] Go back to the
 calendar
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt`

 * *Files 2% similar despite different names*

```diff
@@ -139,22 +139,30 @@
   </div>
 </metal:macro>
 
 <!-- This is the html for a slot in the stormynight period -->
 <metal:macro metal:define-macro="stormy_slot" i18n:domain="redturtle.prenotazioni">
   <div class="slot" tal:repeat="slot python:slots[gate]">
     <div tal:condition="nocall:slot/context"
-         tal:define="booking nocall:slot/context"
+         tal:define="booking nocall:slot/context;
+                    is_pause python:getattr(booking, 'is_pause', False)"
          tal:attributes="class python:week_view.prenotazioni.get_state(booking);">
-      <a href="${booking/absolute_url}"
-         title="${booking/Title}">
-        <tal:from replace="python:week_view.DT2time(booking.getBooking_date())" />
-        &mdash;
-        <tal:to replace="python:week_view.DT2time(booking.getBooking_expiration_date())" />
-    </a>
+        <tal:is_pause condition="is_pause">
+            <div>
+              <span>${booking/Title}</span>
+            </div>
+        </tal:is_pause>
+        <tal:not_is_pause condition="not:is_pause">
+          <a href="${booking/absolute_url}"
+            title="${booking/Title}">
+            <tal:from replace="python:week_view.DT2time(booking.getBooking_date())" />
+            &mdash;
+            <tal:to replace="python:week_view.DT2time(booking.getBooking_expiration_date())" />
+          </a>
+        </tal:not_is_pause>
     </div>
   </div>
 </metal:macro>
 
 <!-- This is the html for a slot when we are in the prenotazioni_move view -->
 <metal:macro metal:define-macro="onmove_slot" i18n:domain="redturtle.prenotazioni">
   <div class="slot" tal:repeat="slot python:slots[gate]">
@@ -190,14 +198,15 @@
          tal:attributes="class python:'slot' + ' ' + (row_index%2 and 'slot-even' or 'slot-odd')">
       <div tal:define="booking nocall:slot/context;"
           class="anonymous_slot">
         <div tal:define="link python:week_view.prenotazioni.get_anonymous_booking_url(day, slot);
                          bookable python:link.get('url', '')">
           <tal:start replace="slot/start" />
           <tal:bookable condition="bookable">
+
             <tal:future condition="link/future">
               <a href=""
                  data-title="Foreseen booking time"
                  aria-label="Forseen booking time"
                  class="reservation-tooltip"
                  tal:attributes="href link/url;
                                  data-title python:week_view.get_foreseen_booking_time(day, slot);
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt`

 * *Files 8% similar despite different names*

```diff
@@ -101,18 +101,18 @@
 
             <div class="actions">
 
                     <a href="javascript:this.print();" title=""
                         tal:attributes="href view/print_action" class="button btn btn-primary">
                         <span i18n:translate="">Print</span>
                     </a>
-                    <a tal:condition="request/delete_token|nothing"
-                        title="Cancella Prenotazione" href="delete" class="button btn btn-danger"
-                        tal:define="url string:${prenotazioni_folder/absolute_url}/@@delete_reservation?${request/QUERY_STRING}&confirm=True;
-                                    protected_url python:view.protect_url(url)"
-                        tal:attributes="href protected_url">Cancella questa prenotazione</a>
+                    <a tal:condition="prenotazione/canDeleteBooking"
+                        title="Cancella Prenotazione"
+                        class="button btn btn-danger"
+                        tal:define="url string:${prenotazioni_folder/absolute_url}/@@delete_reservation?uid=${prenotazione/UID};"
+                        href="${url}">Cancella questa prenotazione</a>
                     <a title="Prenotazioni" href="prenotazioni" class="button btn btn-default"
                     tal:attributes="href string:${prenotazioni_folder/absolute_url}?data=${request/data|nothing}">Ritorna alle prenotazioni</a>
             </div>
         </metal:content>
     </body>
 </html>
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/templates/week.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/templates/week.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/vacations.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/vacations.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/week.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/week.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/browser/z3c_custom_widget.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/browser/z3c_custom_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 self.context.context.aq_inner
             )
 
     @property
     @memoize
     def booking_types_bookability(self):
         """Get booking_type bookability"""
-        booking_date = self.prenotazione_add.booking_DateTime.asdatetime()
+        booking_date = self.prenotazione_add.booking_DateTime
         prenotazioni = self.prenotazione_add.prenotazioni
         return prenotazioni.booking_types_bookability(booking_date)
 
     @property
     @memoize
     def unbookable_items(self):
         """Get booking_type bookability"""
@@ -93,15 +93,15 @@
         if voc_name:
             return getUtility(IVocabularyFactory, name=voc_name)(self.context)
 
     @property
     @memoize
     def booking_types_bookability(self):
         """Get booking_type bookability"""
-        booking_date = self.prenotazione_add.booking_DateTime.asdatetime()
+        booking_date = self.prenotazione_add.booking_DateTime
         prenotazioni = self.prenotazione_add.prenotazioni
         return prenotazioni.booking_types_bookability(booking_date)
 
     @property
     @memoize
     def bookable_items(self):
         """Get booking_type bookability"""
@@ -154,28 +154,28 @@
                     "select-option",
                     "seleziona l'opzione desiderata dal gruppo di radio button seguente",
                 )
             ),
         )
         return message
 
-    def renderForValue(self, value, index=None):
+    def renderForValue(self, value, index=0):
         # customize 'cause we need to pass index
         terms = list(self.terms)
         try:
             term = self.terms.getTermByToken(value)
         except LookupError:
             if value == SequenceWidget.noValueToken:
                 term = SimpleTerm(value)
                 terms.insert(0, term)
             else:
                 raise
         checked = self.isChecked(term)
         # id = '%s-%i' % (self.id, terms.index(term))
-        id = "%s-%i" % (self.id, index)
+        id = "{}-{}".format(self.id, index)
         item = {
             "id": id,
             "name": self.name,
             "value": term.token,
             "checked": checked,
         }
         template = zope.component.getMultiAdapter(
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/configure.zcml`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,30 @@
       title="redturtle.prenotazioni (uninstall)"
       description="Uninstalls the redturtle.prenotazioni add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
       directory="profiles/uninstall"
       post_handler=".setuphandlers.uninstall"
       />
 
+  <genericsetup:registerProfile
+      name="to_1500"
+      title="redturtle.prenotazioni (to_1500)"
+      description="redturtle.prenotazioni to 1500."
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/to_1500"
+      />
+
+  <genericsetup:registerProfile
+      name="content_rules_evolution"
+      title="Profile create to add the new default content rule: booking-confirm"
+      description="Used to add new contentrules"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/to_1402"
+      />
+
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="redturtle.prenotazioni-hiddenprofiles"
       />
 
   <adapter
       factory=".indexes.Subject_prenotazione"
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/pause.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/pause.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazione.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from .prenotazioni_folder import IPrenotazioniFolder
 from datetime import datetime
 from DateTime import DateTime
 from plone import api
+from plone.autoform import directives
 from plone.dexterity.content import Item
 from plone.supermodel import model
 from redturtle.prenotazioni import _
 from redturtle.prenotazioni import tznow
 from zope import schema
 from zope.interface import implementer
 from zope.schema import ValidationError
@@ -104,14 +105,15 @@
         return True
     raise IsNotfutureDate
 
 
 class IPrenotazione(model.Schema):
     """Marker interface and Dexterity Python Schema for Prenotazione"""
 
+    directives.mode(booking_date="display")
     booking_date = schema.Datetime(
         title=_("label_booking_time", "Booking time"),
         required=True,
         default=None,
         constraint=check_is_future_date,
     )
 
@@ -147,19 +149,20 @@
         description=_(
             "description_company",
             default="If you work for a company, please specify its name.",
         ),
         required=False,
     )
 
+    directives.mode(gate="display")
     gate = schema.TextLine(
         title=_("Gate"),
         description=_("Sportello a cui presentarsi"),
     )
-
+    directives.mode(booking_expiration_date="display")
     booking_expiration_date = schema.Datetime(
         title=_("Expiration date booking"), required=True
     )
 
     staff_notes = schema.Text(
         required=False, title=_("label_booking_staff_notes", "Staff notes")
     )
@@ -231,7 +234,39 @@
         # Return reservation date
         return DateTime(self.getBooking_date())
 
     def getBookingCode(self):
         date = self.booking_date.isoformat()
         hash_obj = hashlib.blake2b(bytes(date, encoding="utf8"), digest_size=3)
         return hash_obj.hexdigest().upper()
+
+    def canAccessBooking(self):
+        creator = self.Creator()
+        if api.user.is_anonymous():
+            if creator:
+                return False
+        else:
+            current_user = api.user.get_current()
+            if (
+                not api.user.has_permission("redturtle.prenotazioni.ManagePrenotazioni")
+                and creator != current_user.getUserName()
+            ):
+                return False
+        return True
+
+    def canDeleteBooking(self):
+        creator = self.Creator()
+        if not creator:
+            if api.user.is_anonymous():
+                return True
+            if api.user.has_permission("redturtle.prenotazioni.ManagePrenotazioni"):
+                return True
+        else:
+            if api.user.is_anonymous():
+                return False
+            current_user = api.user.get_current()
+            if (
+                api.user.has_permission("redturtle.prenotazioni.ManagePrenotazioni")
+                or creator == current_user.getUserName()
+            ):
+                return True
+        return False
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/content/prenotazioni_folder.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/content/prenotazioni_folder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # -*- coding: utf-8 -*-
 from collective.z3cform.datagridfield.datagridfield import DataGridFieldFactory
 from collective.z3cform.datagridfield.row import DictRow
 from datetime import date
-
-try:
-    from plone.app.dexterity import textindexer
-except ImportError:
-    # Plone 5.2
-    from collective import dexteritytextindexer as textindexer
 from plone.app.textfield import RichText
 from plone.autoform import directives
 from plone.autoform import directives as form
 from plone.dexterity.content import Container
 from plone.supermodel import model
 from redturtle.prenotazioni import _
-from redturtle.prenotazioni.adapters.slot import interval_is_contained
-from redturtle.prenotazioni.adapters.slot import is_intervals_overlapping
+from redturtle.prenotazioni.browser.widget import WeekTableOverridesFieldWidget
+from redturtle.prenotazioni.content.validators import checkOverrides
+from redturtle.prenotazioni.content.validators import PauseValidator
 from z3c.form import validator
 from z3c.form.browser.checkbox import CheckBoxFieldWidget
 from zope import schema
 from zope.component import provideAdapter
 from zope.interface import implementer
 from zope.interface import Interface
 from zope.interface import Invalid
 from zope.interface import invariant
 from zope.schema.vocabulary import SimpleTerm
 from zope.schema.vocabulary import SimpleVocabulary
 
+try:
+    from plone.app.dexterity import textindexer
+except ImportError:
+    # Plone 5.2
+    from collective import dexteritytextindexer as textindexer
+
 
 def get_dgf_values_from_request(request, fieldname, columns=[]):
     """
     Validator with datagridfield works in a fuzzy way. We need to extract
     values from request to be sure we are validating correct data.
     """
 
@@ -86,32 +87,29 @@
         title=_("afternoon_end_label", default="End time in the afternoon"),
         vocabulary="redturtle.prenotazioni.VocOreInizio",
         required=False,
     )
 
 
 class IPauseTableRow(model.Schema):
-    def get_options():  # noqa
-        """Return the options for the day widget"""
-        options = [
-            SimpleTerm(value=None, token=None, title=_("Select a day")),
-            SimpleTerm(value=0, token=0, title=_("Monday")),
-            SimpleTerm(value=1, token=1, title=_("Tuesday")),
-            SimpleTerm(value=2, token=2, title=_("Wednesday")),
-            SimpleTerm(value=3, token=3, title=_("Thursday")),
-            SimpleTerm(value=4, token=4, title=_("Friday")),
-            SimpleTerm(value=5, token=5, title=_("Saturday")),
-            SimpleTerm(value=6, token=6, title=_("Sunday")),
-        ]
-        return SimpleVocabulary(options)
-
     day = schema.Choice(
         title=_("day_label", default="Day of week"),
         required=True,
-        source=get_options(),
+        vocabulary=SimpleVocabulary(
+            [
+                SimpleTerm(value=None, token=None, title=_("Select a day")),
+                SimpleTerm(value=0, token=0, title=_("Monday")),
+                SimpleTerm(value=1, token=1, title=_("Tuesday")),
+                SimpleTerm(value=2, token=2, title=_("Wednesday")),
+                SimpleTerm(value=3, token=3, title=_("Thursday")),
+                SimpleTerm(value=4, token=4, title=_("Friday")),
+                SimpleTerm(value=5, token=5, title=_("Saturday")),
+                SimpleTerm(value=6, token=6, title=_("Sunday")),
+            ]
+        ),
     )
     pause_start = schema.Choice(
         title=_("pause_start_label", default="Pause start"),
         vocabulary="redturtle.prenotazioni.VocOreInizio",
         required=False,
     )
     pause_end = schema.Choice(
@@ -136,14 +134,22 @@
     textindexer.searchable("descriptionAgenda")
     descriptionAgenda = RichText(
         required=False,
         title=_("Descrizione Agenda", default="Descrizione Agenda"),
         description=_("Inserire il testo di presentazione dell'agenda corrente"),
     )
 
+    cosa_serve = schema.Text(
+        required=False,
+        title=_("Cosa serve", default="Cosa serve"),
+        description=_(
+            "Elencare le informazioni utili per il giorno della prenotazione, come ad esempio i documenti da presentare."
+        ),
+    )
+
     directives.widget(required_booking_fields=CheckBoxFieldWidget)
     required_booking_fields = schema.List(
         title=_("label_required_booking_fields", default="Required booking fields"),
         description=_(
             "help_required_booking_fields",
             "User will not be able to add a booking unless those "
             "fields are filled. "
@@ -270,14 +276,24 @@
             },
         ],
     )
     form.widget(
         "week_table", DataGridFieldFactory, frontendOptions={"widget": "data_grid"}
     )
 
+    week_table_overrides = schema.SourceText(
+        title=_("week_table_overrides_label", default="Week table overrides"),
+        description=_(
+            "week_table_overrides_help",
+            default="Insert here week schema for some custom date intervals.",
+        ),
+        required=False,
+        constraint=checkOverrides,
+    )
+    form.widget("week_table_overrides", WeekTableOverridesFieldWidget)
     pause_table = schema.List(
         title=_("Pause table"),
         description=_("Insert pause table schema."),
         required=False,
         value_type=DictRow(title="Pause row", schema=IPauseTableRow),
     )
     form.widget(
@@ -397,138 +413,65 @@
 
     complete_address = schema.Text(
         required=False,
         title=_("Complete address", default="Complete address"),
         description=_("Insert here the complete office address"),
     )
 
-    model.fieldset(
-        "contacts",
-        label=_("contacts_label", default="Contacts"),
-        description=_(
-            "contacts_help",
-            default="Show here contacts information that will be used by authomatic mail system",  # noqa
-        ),
-        fields=["how_to_get_here", "phone", "fax", "pec", "complete_address"],
-    )
-
     @invariant
     def data_validation(data):
+        """
+        Needed because is the only way to validate a datagrid field
+        """
         if not data.booking_types:
             raise Invalid(_("You should set at least one booking type."))
         for interval in data.week_table:
             if interval["morning_start"] and not interval["morning_end"]:
-                raise Invalid(_("You should set and end time for morning."))
+                raise Invalid(_("You should set an end time for morning."))
             if interval["morning_end"] and not interval["morning_start"]:
                 raise Invalid(_("You should set a start time for morning."))
             if interval["afternoon_start"] and not interval["afternoon_end"]:
-                raise Invalid(_("You should set and end time for afternoon."))
+                raise Invalid(_("You should set an end time for afternoon."))
             if interval["afternoon_end"] and not interval["afternoon_start"]:
                 raise Invalid(_("You should set a start time for afternoon."))
             if interval["morning_start"] and interval["morning_end"]:
                 if interval["morning_start"] > interval["morning_end"]:
                     raise Invalid(_("Morning start should not be greater than end."))
             if interval["afternoon_start"] and interval["afternoon_end"]:
                 if interval["afternoon_start"] > interval["afternoon_end"]:
                     raise Invalid(_("Afternoon start should not be greater than end."))
 
     # TODO: definire o descrivere quando avviee la notifica
     app_io_enabled = schema.Bool(
         title=_("App IO notification"),
         default=False,
+        required=False,
     )
 
     # TODO: inserire qui la chiave IO ? o su un config in zope.conf/environment ?
 
     model.fieldset(
+        "contacts",
+        label=_("contacts_label", default="Contacts"),
+        description=_(
+            "contacts_help",
+            default="Show here contacts information that will be used by authomatic mail system",  # noqa
+        ),
+        fields=["how_to_get_here", "phone", "fax", "pec", "complete_address"],
+    )
+
+    model.fieldset(
         "Reminders",
         label=_("reminders_label", default="Reminders"),
         fields=[
             "app_io_enabled",
         ],
     )
 
 
-class PauseValidator(validator.SimpleFieldValidator):
-    """z3c.form validator class for international phone numbers"""
-
-    def validate(self, pause_table):
-        """Validate international phone number on input"""
-        super(PauseValidator, self).validate(pause_table)
-        pause_table = get_dgf_values_from_request(
-            self.context.REQUEST,
-            "pause_table",
-            ["day", "pause_start", "pause_end"],
-        )
-        if not pause_table:
-            return
-
-        week_table = get_dgf_values_from_request(
-            self.context.REQUEST,
-            "week_table",
-            [
-                "day",
-                "morning_start",
-                "morning_end",
-                "afternoon_start",
-                "afternoon_end",
-            ],
-        )
-
-        # validate pauses
-        groups_of_pause = {}
-        for pause in pause_table:
-            groups_of_pause.setdefault(pause["day"], []).append(pause)
-
-        for day in groups_of_pause:
-            day_hours = week_table[int(day)]
-            for pause in groups_of_pause[day]:
-                #  0. Of course if we don't have a correct interval we can't do
-                # more steps
-                if (
-                    pause["pause_end"] == "--NOVALUE--"
-                    or pause["pause_start"] == "--NOVALUE--"
-                ):
-                    raise Invalid(_("You must set both start and end"))
-
-                # 1. Pause starts should always be bigger than pause ends
-                if not (pause["pause_end"] > pause["pause_start"]):
-                    raise Invalid(_("Pause end should be greater than pause start"))
-                interval = [pause["pause_start"], pause["pause_end"]]
-                # 2. a pause interval should always be contained in the morning
-                # or afternoon defined for these days
-                if not (
-                    interval_is_contained(
-                        interval,
-                        day_hours["morning_start"],
-                        day_hours["morning_end"],
-                    )
-                    or interval_is_contained(
-                        interval,
-                        day_hours["afternoon_start"],
-                        day_hours["afternoon_end"],
-                    )
-                ):
-                    raise Invalid(
-                        _(
-                            "Pause should be included in morning slot or afternoon slot"  # noqa
-                        )
-                    )
-            # 3. two pause interval on the same day should not overlap
-            if is_intervals_overlapping(
-                [
-                    (pause["pause_start"], pause["pause_end"])
-                    for pause in groups_of_pause[day]
-                ]
-            ):
-                raise Invalid(
-                    _("In the same day there are overlapping intervals")
-                )  # noqa
-
-
 validator.WidgetValidatorDiscriminators(
     PauseValidator, field=IPrenotazioniFolder["pause_table"]
 )
 provideAdapter(PauseValidator)
 
 
 @implementer(IPrenotazioniFolder)
@@ -551,7 +494,10 @@
         return self.aData
 
     def getFutureDays(self):
         return self.futureDays
 
     def getNotBeforeDays(self):
         return self.notBeforeDays
+
+    def getCosaServe(self):
+        return self.cosa_serve
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/contentrules/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/events_logger.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/events_logger.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/prenotazione.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/prenotazione.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/events/prenotazioni_folder.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/events/prenotazioni_folder.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/indexers/searchable_text.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/indexers/searchable_text.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,1127 +1,1207 @@
-# --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
-# English translations for PACKAGE package.
-# Andrea Cecchi <cekk@darthmaulcekk2.station>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-02-25 07:58+0000\n"
-"PO-Revision-Date: 2020-12-03 16:12+0100\n"
-"Last-Translator: Andrea Cecchi <cekk@darthmaulcekk2.station>\n"
-"Language-Team: English\n"
+"POT-Creation-Date: 2023-05-30 12:50+0000\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
-"Domain: redturtle.prenotazioni\n"
-"Language: en\n"
+"Domain: DOMAIN\n"
 
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:54
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:40
-#: redturtle/prenotazioni/browser/vacations.py:72
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:56
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:45
+#: redturtle/prenotazioni/browser/vacations.py:73
 msgid " format (YYYY-MM-DD)"
-msgstr " format (YYYY-MM-DD)"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "A folder that will contain booking"
-msgstr "A folder that will contain booking"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 msgid "A folder that will contain booking for this day"
-msgstr "A folder that will contain booking for this day"
+msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:166
 msgid "A mail action that sends email notify when a booking is moved in an other slot."
-msgstr "A mail action that sends email notify when a booking is moved in an other slot."
+msgstr ""
+
+msgid "Add"
+msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:165
 msgid "Add moved booking Mail Action"
-msgstr "Add moved booking Mail Action"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:424
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:441
+#: redturtle/prenotazioni/content/validators.py:212
 msgid "Afternoon start should not be greater than end."
-msgstr "Afternoon start should not be greater than end."
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:428
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:445
 msgid "App IO notification"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:22
 msgid "Attention"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:26
+#: redturtle/prenotazioni/adapters/stringinterp.py:23
 msgid "Booking"
-msgstr "Booking"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "Booking Folder"
-msgstr "Booking Folder"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
 msgid "Booking Week Folder"
-msgstr "Booking Week Folder"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
 msgid "Booking Year Folder"
-msgstr "Booking Year Folder"
+msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:33
 msgid "Booking for"
-msgstr "Booking for"
+msgstr ""
 
 #: redturtle/prenotazioni/contentrules/configure.zcml:30
 msgid "Booking moved"
-msgstr "Booking moved"
+msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:123
 msgid "Booking type name"
-msgstr "Booking type name"
+msgstr ""
 
 #. Default: "Change date/time"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "Change date/time"
-msgstr "Change date/time"
+msgstr ""
 
 #. Default: "Complete address"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:392
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:416
 msgid "Complete address"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:170
 msgid "Configure element"
-msgstr "Configure element"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:385
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:409
 msgid "Contact PEC"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:379
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:403
 msgid "Contact fax"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:373
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:397
 msgid "Contact phone"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:31
 msgid "Content listing"
-msgstr "Content listing"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:181
+#. Default: "Cosa serve"
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:143
+msgid "Cosa serve"
+msgstr ""
+
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:189
 msgid "Data fine validità"
-msgstr "Data fine validità"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:178
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:186
 msgid "Data inizio validità"
-msgstr "Data inizio validità"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:308
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:330
 msgid "Days booking is not allowed before"
-msgstr "Days booking is not allowed before"
+msgstr ""
+
+msgid "Delete"
+msgstr ""
 
 #. Default: "Descrizione Agenda"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:137
 msgid "Descrizione Agenda"
-msgstr "Descrizione Agenda"
+msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:125
 msgid "Duration value"
-msgstr "Duration value"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "Edit"
-msgstr "Edit"
+msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:185
 msgid "Edit moved booking Mail Action"
-msgstr "Edit moved booking Mail Action"
+msgstr ""
+
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:144
+msgid "Elencare le informazioni utili per il giorno della prenotazione, come ad esempio i documenti da presentare."
+msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:72
 msgid "Email report to prenotazione owner"
-msgstr "Email report to prenotazione owner"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazione.py:159
+#: redturtle/prenotazioni/content/prenotazione.py:163
 msgid "Expiration date booking"
-msgstr "Expiration date booking"
+msgstr ""
 
 #. Default: "Campo"
-#: redturtle/prenotazioni/browser/z3c_custom_widget.py:149
+#: redturtle/prenotazioni/browser/z3c_custom_widget.py:150
 msgid "Field"
-msgstr "Field"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:99
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:104
 msgid "Friday"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:81
-#: redturtle/prenotazioni/content/prenotazione.py:154
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:80
+#: redturtle/prenotazioni/content/prenotazione.py:158
 msgid "Gate"
-msgstr "Gate"
+msgstr ""
+
+msgid "Group"
+msgstr ""
 
 #. Default: "How to get here"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:368
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:392
 msgid "How to get here"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:516
+#: redturtle/prenotazioni/content/validators.py:135
 msgid "In the same day there are overlapping intervals"
 msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 msgid "Informations about a single booking"
-msgstr "Informations about a single booking"
+msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:138
 msgid "Inserire il testo di presentazione dell'agenda corrente"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:357
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:381
 msgid "Insert a list of email addresses that will be notified when new bookings get created."
-msgstr "Insert a list of email addresses that will be notified when new bookings get created."
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:369
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:393
 msgid "Insert here indications on how to reach the office"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:393
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:417
 msgid "Insert here the complete office address"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:386
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:410
 msgid "Insert here the contact PEC"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:380
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:404
 msgid "Insert here the contact fax"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:374
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:398
 msgid "Insert here the contact phone"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:275
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:295
 msgid "Insert pause table schema."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:216
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:224
 msgid "Insert week table schema."
-msgstr "Insert week table schema."
-
-#: redturtle/prenotazioni/configure.zcml:30
-msgid "Installs the redturtle.prenotazioni add-on."
-msgstr "Installs the redturtle.prenotazioni add-on."
-
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:32
-msgid "Is not possible to delete your reservation"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:35
-msgid "It's not possbile to delete your reservation. The url is broken or it's to late to delete it"
+#: redturtle/prenotazioni/configure.zcml:31
+msgid "Installs the redturtle.prenotazioni add-on."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:296
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:318
 msgid "Max days in the future"
-msgstr "Max days in the future"
+msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:42
 msgid "Message"
-msgstr "Message"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:95
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:100
 msgid "Monday"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:421
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:438
+#: redturtle/prenotazioni/content/validators.py:207
 msgid "Morning start should not be greater than end."
-msgstr "Morning start should not be greater than end."
+msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:111
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:114
 msgid "Move booking"
-msgstr "Move booking"
+msgstr ""
+
+msgid "Move down"
+msgstr ""
+
+msgid "Move up"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:194
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:202
 msgid "No"
-msgstr "No"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:195
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:203
 msgid "No, just for today"
-msgstr "No, just for today"
+msgstr ""
 
 #: redturtle/prenotazioni/content/pause.py:41
 msgid "Pause"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:487
+#: redturtle/prenotazioni/content/validators.py:99
 msgid "Pause end should be greater than pause start"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:504
+#: redturtle/prenotazioni/content/validators.py:120
 msgid "Pause should be included in morning slot or afternoon slot"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:274
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:294
 msgid "Pause table"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:278
+#: redturtle/prenotazioni/browser/prenotazione_add.py:261
 msgid "Please provide a booking date"
-msgstr "Please provide a booking date"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 msgid "Prenotazione"
-msgstr "Prenotazione"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 msgid "PrenotazioniDay"
-msgstr "PrenotazioniDay"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
 msgid "PrenotazioniWeek"
-msgstr "PrenotazioniWeek"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
 msgid "PrenotazioniYear"
-msgstr "PrenotazioniYear"
+msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:107
+#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:106
 msgid "Print"
-msgstr "Print"
+msgstr ""
+
+#: redturtle/prenotazioni/configure.zcml:56
+msgid "Profile create to add the new default content rule: booking-confirm"
+msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:274
+#: redturtle/prenotazioni/restapi/services/booking/add.py:34
+msgid "Required input '${field}' is missing."
+msgstr ""
+
+#: redturtle/prenotazioni/browser/prenotazione_add.py:257
 msgid "Required input is missing."
-msgstr "Required input is missing."
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:356
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:380
 msgid "Responsible email"
-msgstr "Responsible email"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:100
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:105
 msgid "Saturday"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:11
 msgid "Search for"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:94
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:99
 msgid "Select a day"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/configure.zcml:57
 msgid "Send Email to booking owner when a booking is moved"
-msgstr "Send Email to booking owner when a booking is moved"
+msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:32
 msgid "Sender email"
-msgstr "Sender email"
-
-#: redturtle/prenotazioni/browser/delete_reservation.py:107
-msgid "Some information to delete your reservation is missing"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:283
+#: redturtle/prenotazioni/browser/prenotazione_add.py:266
+#: redturtle/prenotazioni/restapi/services/booking/add.py:83
 msgid "Sorry, this slot is not available anymore."
-msgstr "Sorry, this slot is not available anymore."
+msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_move.py:166
+#: redturtle/prenotazioni/browser/prenotazione_move.py:164
 msgid "Sorry, this slot is not available or does not fit your booking."
-msgstr "Sorry, this slot is not available or does not fit your booking."
+msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:286
-#: redturtle/prenotazioni/browser/prenotazione_move.py:172
+#: redturtle/prenotazioni/browser/prenotazione_add.py:269
+#: redturtle/prenotazioni/browser/prenotazione_move.py:170
+#: redturtle/prenotazioni/restapi/services/booking/add.py:90
 msgid "Sorry, you can not book this slot for now."
-msgstr "Sorry, you can not book this slot for now."
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazione.py:155
+#: redturtle/prenotazioni/content/prenotazione.py:159
 msgid "Sportello a cui presentarsi"
-msgstr "Postazione a cui presentarsi"
+msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:26
 msgid "Subject"
-msgstr "Subject"
+msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:27
 msgid "Subject of the message"
-msgstr "Subject of the message"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:101
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:106
 msgid "Sunday"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:37
+#: redturtle/prenotazioni/adapters/stringinterp.py:33
 msgid "The booked date."
-msgstr "The booked date."
+msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:51
+#: redturtle/prenotazioni/adapters/stringinterp.py:46
 msgid "The booked end date."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:65
+#: redturtle/prenotazioni/adapters/stringinterp.py:59
 msgid "The booked time."
-msgstr "The booked time."
+msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:103
+#: redturtle/prenotazioni/adapters/stringinterp.py:94
 msgid "The booking code."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:228
+#: redturtle/prenotazioni/adapters/stringinterp.py:200
 msgid "The booking human readable date"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:190
+#: redturtle/prenotazioni/adapters/stringinterp.py:166
 msgid "The booking office contact fax."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:179
+#: redturtle/prenotazioni/adapters/stringinterp.py:156
 msgid "The booking office contact pec address."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:168
+#: redturtle/prenotazioni/adapters/stringinterp.py:146
 msgid "The booking office contact phone."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:129
-msgid "The booking print url with delete token."
-msgstr ""
-
-#: redturtle/prenotazioni/adapters/stringinterp.py:116
+#: redturtle/prenotazioni/adapters/stringinterp.py:106
 msgid "The booking print url."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:79
+#: redturtle/prenotazioni/adapters/stringinterp.py:72
 msgid "The booking time end."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:93
+#: redturtle/prenotazioni/adapters/stringinterp.py:85
 msgid "The booking type."
-msgstr "The booking type."
+msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:256
+#: redturtle/prenotazioni/adapters/stringinterp.py:227
 msgid "The booking url with delete token"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:214
+#: redturtle/prenotazioni/adapters/stringinterp.py:188
 msgid "The complete address information of the office whereuser book a reservation"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:158
+#: redturtle/prenotazioni/adapters/stringinterp.py:137
 msgid "The email address of the user who made the reservation."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:27
+#: redturtle/prenotazioni/adapters/stringinterp.py:24
 msgid "The gate booked."
-msgstr "The gate booked."
+msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:201
+#: redturtle/prenotazioni/adapters/stringinterp.py:176
 msgid "The information to reach the office where user book a reservation"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:148
+#: redturtle/prenotazioni/adapters/stringinterp.py:128
 msgid "The phone number of the user who made the reservation."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:98
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:103
 msgid "Thursday"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:96
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:101
 msgid "Tuesday"
 msgstr ""
 
-#: redturtle/prenotazioni/configure.zcml:39
+#: redturtle/prenotazioni/configure.zcml:40
 msgid "Uninstalls the redturtle.prenotazioni add-on."
-msgstr "Uninstalls the redturtle.prenotazioni add-on."
+msgstr ""
+
+#: redturtle/prenotazioni/restapi/services/booking/add.py:66
+msgid "Unknown booking type '${booking_type}'."
+msgstr ""
+
+#: redturtle/prenotazioni/configure.zcml:56
+msgid "Used to add new contentrules"
+msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "View"
-msgstr "View"
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:97
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:102
 msgid "Wednesday"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:215
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:223
 msgid "Week table"
-msgstr "Week table"
-
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:193
-msgid "Yes"
-msgstr "Yes"
-
-#: redturtle/prenotazioni/browser/delete_reservation.py:85
-msgid "You can't delete your reservation; it's too late"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/delete_reservation.py:72
-msgid "You can't delete your reservation; please contact the office"
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:201
+msgid "Yes"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:483
+#: redturtle/prenotazioni/content/validators.py:91
 msgid "You must set both start and end"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:418
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:435
+#: redturtle/prenotazioni/content/validators.py:202
 msgid "You should set a start time for afternoon."
-msgstr "You should set a start time for afternoon."
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:414
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:431
+#: redturtle/prenotazioni/content/validators.py:194
 msgid "You should set a start time for morning."
-msgstr "You should set a start time for morning."
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:416
-msgid "You should set and end time for afternoon."
-msgstr "You should set and end time for afternoon."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:433
+#: redturtle/prenotazioni/content/validators.py:198
+msgid "You should set an end time for afternoon."
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:412
-msgid "You should set and end time for morning."
-msgstr "You should set and end time for morning."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:429
+#: redturtle/prenotazioni/content/validators.py:190
+msgid "You should set an end time for morning."
+msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:409
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:426
 msgid "You should set at least one booking type."
-msgstr "You should set at least one booking type."
+msgstr ""
 
-#: redturtle/prenotazioni/browser/delete_reservation.py:94
-msgid "Your reservation has been deleted"
+#: redturtle/prenotazioni/adapters/stringinterp.py:122
+msgid "[DEPRECATED] The booking print url with delete token."
 msgstr ""
 
 #. Default: "Leave empty, and this Booking Folder will never expire"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:182
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:190
 msgid "aData_help"
-msgstr "aData_help"
+msgstr ""
 
 #. Default: "Book"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:256
-#: redturtle/prenotazioni/browser/vacations.py:252
+#: redturtle/prenotazioni/browser/prenotazione_add.py:239
+#: redturtle/prenotazioni/browser/vacations.py:246
 msgid "action_book"
-msgstr "action_book"
+msgstr ""
 
 #. Default: "Cancel"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:321
-#: redturtle/prenotazioni/browser/prenotazione_move.py:187
-#: redturtle/prenotazioni/browser/vacations.py:277
+#: redturtle/prenotazioni/browser/prenotazione_add.py:300
+#: redturtle/prenotazioni/browser/prenotazione_move.py:185
+#: redturtle/prenotazioni/browser/vacations.py:271
 msgid "action_cancel"
-msgstr "action_cancel"
+msgstr ""
 
 #. Default: "Move"
-#: redturtle/prenotazioni/browser/prenotazione_move.py:151
+#: redturtle/prenotazioni/browser/prenotazione_move.py:149
 msgid "action_move"
-msgstr "action_move"
+msgstr ""
 
 #. Default: "Search"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:234
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:236
 msgid "action_search"
-msgstr "action_search"
+msgstr ""
 
 #. Default: "End time in the afternoon"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:84
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:87
 msgid "afternoon_end_label"
-msgstr "afternoon_end_label"
+msgstr ""
 
 #. Default: "Start time in the afternoon"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:78
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:81
 msgid "afternoon_start_label"
-msgstr "afternoon_start_label"
+msgstr ""
 
 #. Default: "Please select a booking slot."
 #: redturtle/prenotazioni/browser/templates/week.pt:28
 msgid "book_it"
-msgstr "book_it"
+msgstr ""
 
 #. Default: "Bookable time"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:297
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:306
 msgid "bookable_time"
-msgstr "bookable_time"
+msgstr ""
 
 #. Default: "${day}, ore ${booking_time}, prenotato da ${booked_by}, prenotazione: ${booking_type} durata: ${duration} minuti"
-#: redturtle/prenotazioni/browser/week.py:257
+#: redturtle/prenotazioni/browser/week.py:276
 msgid "booked_prenotation_message"
 msgstr ""
 
 #. Default: "Booking confirmed"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:299
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:308
 msgid "booking_confirmed"
-msgstr "booking_confirmed"
+msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:303
-#: redturtle/prenotazioni/browser/vacations.py:249
+#: redturtle/prenotazioni/browser/prenotazione_add.py:278
+#: redturtle/prenotazioni/browser/vacations.py:243
 msgid "booking_created"
-msgstr "booking_created"
+msgstr ""
+
+#. Default: "Your booking has been deleted."
+#: redturtle/prenotazioni/browser/delete_reservation.py:112
+msgid "booking_deleted_success"
+msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_move.py:177
+#: redturtle/prenotazioni/browser/prenotazione_move.py:175
 msgid "booking_moved"
-msgstr "booking_moved"
+msgstr ""
 
 #. Default: "Booking pending"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:301
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:310
 msgid "booking_pending"
-msgstr "booking_pending"
+msgstr ""
 
 #. Default: "Booking refused"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:303
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:312
 msgid "booking_refused"
-msgstr "booking_refused"
+msgstr ""
 
 #. Default: "Name"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:272
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:281
 msgid "booking_type_name"
-msgstr "booking_type_name"
+msgstr ""
 
 #. Default: "Value"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:273
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:282
 msgid "booking_type_value"
-msgstr "booking_type_value"
+msgstr ""
 
 #. Default: "You may want to select another time slot to book one of these."
 #: redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt:55
 msgid "booking_type_widget_suggest_reselect"
-msgstr "booking_type_widget_suggest_reselect"
+msgstr ""
 
 #. Default: "The following tipologies will not fit the time you selected:"
 #: redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt:45
 msgid "booking_type_widget_warn_unavailable"
-msgstr "booking_type_widget_warn_unavailable"
+msgstr ""
 
 #. Default: "Put booking types there (one per line).\nIf you do not provide this field, not type selection will be available"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:319
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:341
 msgid "booking_types_help"
-msgstr "booking_types_help"
+msgstr ""
 
 #. Default: "Booking types"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:318
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:340
 msgid "booking_types_label"
-msgstr "booking_types_label"
+msgstr ""
 
 #. Default: "Bookings not in agenda"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:63
 msgid "bookings_not_in_agenda"
-msgstr "bookings_not_in_agenda"
+msgstr ""
 
 #. Default: "Busy"
-#: redturtle/prenotazioni/browser/prenotazioni_context_state.py:76
+#: redturtle/prenotazioni/browser/prenotazioni_context_state.py:81
 msgid "busy"
-msgstr "busy"
+msgstr ""
 
 #. Default: "Your booking has to be confirmed by the administrators"
 #: redturtle/prenotazioni/browser/prenotazione_print.py:19
 msgid "confirm_booking_waiting_message"
-msgstr "confirm_booking_waiting_message"
+msgstr ""
 
 #. Default: "Show here contacts information that will be used by authomatic mail system"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:399
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:455
 msgid "contacts_help"
 msgstr ""
 
 #. Default: "Contacts"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:398
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:454
 msgid "contacts_label"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:23
-msgid "damn"
+#. Default: "Cosa serve"
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:96
+msgid "cosa_serve"
 msgstr ""
 
 #. Default: "This day is not valid."
-#: redturtle/prenotazioni/browser/vacations.py:269
+#: redturtle/prenotazioni/browser/vacations.py:263
 msgid "day_error"
-msgstr "day_error"
+msgstr ""
 
 #. Default: "Day of week"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:64
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:67
 msgid "day_label"
-msgstr "day_label"
+msgstr ""
 
-#. Default: "Delete reservation request for: ${name}"
-#: redturtle/prenotazioni/browser/delete_reservation.py:20
-msgid "delete_reservation_request"
+#. Default: "You can't delete your reservation; it's too late."
+#: redturtle/prenotazioni/browser/delete_reservation.py:137
+msgid "delete_expired_booking"
 msgstr ""
 
-#. Default: "Your reservation has been deleted"
-#: redturtle/prenotazioni/browser/delete_reservation.py:41
-msgid "deleted_reservation"
+#. Default: "Delete reservation request for: ${name}"
+#: redturtle/prenotazioni/browser/delete_reservation.py:59
+msgid "delete_reservation_request"
 msgstr ""
 
 #. Default: "If you work for a company, please specify its name."
-#: redturtle/prenotazioni/content/prenotazione.py:146
-#, fuzzy
+#: redturtle/prenotazioni/content/prenotazione.py:149
 msgid "description_company"
-msgstr "description_company"
+msgstr ""
 
 #. Default: "The gate that will be unavailable"
-#: redturtle/prenotazioni/browser/vacations.py:66
+#: redturtle/prenotazioni/browser/vacations.py:67
 msgid "description_gate"
-msgstr "description_gate"
+msgstr ""
 
 #. Default: "This text will appear in the calendar cells"
-#: redturtle/prenotazioni/browser/vacations.py:59
+#: redturtle/prenotazioni/browser/vacations.py:60
 msgid "description_title"
-msgstr "description_title"
+msgstr ""
 
 #. Default: "Foreseen booking time: ${booking_time}"
-#: redturtle/prenotazioni/browser/week.py:206
+#: redturtle/prenotazioni/browser/week.py:225
 msgid "foreseen_booking_time"
-msgstr "foreseen_booking_time"
+msgstr ""
 
 #. Default: "${booking_time}, Orario non disponibile"
-#: redturtle/prenotazioni/browser/week.py:225
-#, fuzzy
+#: redturtle/prenotazioni/browser/week.py:244
 msgid "foreseen_busy_time"
-msgstr "${booking_time}, Time not avaiable"
+msgstr ""
+
+msgid "from_label"
+msgstr ""
+
+#. Default: "You should set a start range."
+#: redturtle/prenotazioni/content/validators.py:159
+msgid "from_month_error"
+msgstr ""
+
+#. Default: "Selected day is too big for that month for \"from\" field."
+#: redturtle/prenotazioni/content/validators.py:166
+msgid "from_month_too_days_error"
+msgstr ""
 
 #. Default: "Fullname"
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:40
 msgid "fullname"
-msgstr "fullname"
+msgstr ""
 
 #. Default: "Limit booking in the future to an amount of days in the future starting from the current day. \nKeep 0 to give no limits."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:297
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:319
 msgid "futureDays"
-msgstr "futureDays"
+msgstr ""
 
 #. Default: "Put gates here (one per line)."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:331
-#, fuzzy
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:355
 msgid "gates_help"
-msgstr "Put gates here (one per line)."
+msgstr ""
 
 #. Default: "Gates"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:330
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:354
 msgid "gates_label"
-msgstr "gates_label"
+msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:165
+#: redturtle/prenotazioni/browser/prenotazione_add.py:162
 msgid "help_prenotazione_add"
-msgstr "help_prenotazione_add"
+msgstr ""
 
 #. Default: "User will not be able to add a booking unless those fields are filled. Remember that, whatever you selected in this list, users have to supply at least one of \"Email\", \"Mobile\", or \"Telephone\""
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:144
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:152
 msgid "help_required_booking_fields"
-msgstr "help_required_booking_fields"
+msgstr ""
 
 #. Default: "States if it is not allowed to reserve a booking during the current day"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:205
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:213
 msgid "help_same_day_booking_disallowed"
-msgstr "help_same_day_booking_disallowed"
+msgstr ""
 
 #. Default: "List of available reservation type for the current agenda"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:269
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:278
 msgid "help_tipologies"
-msgstr "help_tipologies"
+msgstr ""
 
 #. Default: "User will not be able to add a booking unless those fields are filled. Remember that, whatever you selected in this list, users have to supply at least one of \"Email\" or \"Telephone\""
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:162
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:170
 msgid "help_visible_booking_fields"
-msgstr "help_visible_booking_fields"
+msgstr ""
 
 #. Default: "Set holidays (one for line) in DD/MM/YYYY. you can write * for the year, if this event is yearly."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:283
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:305
 msgid "holidays_help"
-msgstr "holidays_help"
+msgstr ""
 
 #. Default: "Holidays"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:282
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:304
 msgid "holidays_label"
-msgstr "holidays_label"
+msgstr ""
 
-#: redturtle/prenotazioni/browser/vacations.py:30
+#: redturtle/prenotazioni/browser/vacations.py:31
 msgid "invalid_date"
-msgstr "invalid_date"
+msgstr ""
 
 #. Default: "Invalid email address"
-#: redturtle/prenotazioni/content/prenotazione.py:26
+#: redturtle/prenotazioni/content/prenotazione.py:28
 msgid "invalid_email_address"
-msgstr "invalid_email_address"
+msgstr ""
 
 #. Default: "Invalid start or end date"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:31
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:20
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:33
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:25
 msgid "invalid_end:search_date"
-msgstr "invalid_end:search_date"
+msgstr ""
 
 #. Default: "Invalid fiscal code"
-#: redturtle/prenotazioni/content/prenotazione.py:34
+#: redturtle/prenotazioni/content/prenotazione.py:36
 msgid "invalid_fiscalcode"
 msgstr ""
 
 #. Default: "Invalid phone number"
-#: redturtle/prenotazioni/content/prenotazione.py:22
+#: redturtle/prenotazioni/content/prenotazione.py:24
 msgid "invalid_phone_number"
-msgstr "invalid_phone_number"
+msgstr ""
 
-#: redturtle/prenotazioni/browser/vacations.py:34
+#: redturtle/prenotazioni/browser/vacations.py:35
 msgid "invalid_time"
-msgstr "The time must be in the format HH: MM"
+msgstr ""
 
 #. Default: "This date is past"
-#: redturtle/prenotazioni/content/prenotazione.py:30
+#: redturtle/prenotazioni/content/prenotazione.py:32
 msgid "is_not_future_date"
-msgstr "is_not_future_date"
+msgstr ""
 
 #. Default: "Booking code"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:115
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:93
-#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:93
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:89
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:92
+#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:92
 msgid "label_booking_code"
 msgstr ""
 
 #. Default: "Company"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:77
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:52
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:36
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:57
 msgid "label_booking_company"
-msgstr "Company"
+msgstr ""
 
 #. Default: "Booking date"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:95
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:70
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:48
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:69
 msgid "label_booking_date"
-msgstr "label_booking_date"
+msgstr ""
 
-#. Default: "${from_date} from ${from} to ${to}"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:103
-#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:52
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:76
+#. Default: "${from_date} at ${at}"
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:77
+#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:51
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:75
 msgid "label_booking_date_range"
-msgstr "label_booking_date_range"
+msgstr ""
 
 #. Default: "Subject"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:53
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:89
+#: redturtle/prenotazioni/browser/prenotazione_add.py:49
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:64
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:44
 msgid "label_booking_description"
-msgstr "Subject"
+msgstr ""
 
 #. Default: "Email"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:65
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:40
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:28
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:48
 msgid "label_booking_email"
-msgstr "Email"
+msgstr ""
 
 #. Default: "Fiscal code"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:83
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:58
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:40
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:61
 msgid "label_booking_fiscalcode"
-msgstr "Fiscalcode"
+msgstr ""
 
 #. Default: "Phone number"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:71
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:46
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:32
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:53
 msgid "label_booking_phone"
-msgstr "Phone"
+msgstr ""
 
 #. Default: "Staff notes"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:85
-#: redturtle/prenotazioni/content/prenotazione.py:163
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:84
+#: redturtle/prenotazioni/content/prenotazione.py:167
 msgid "label_booking_staff_notes"
-msgstr "label_booking_staff_notes"
+msgstr ""
 
 #. Default: "Booking time"
-#: redturtle/prenotazioni/browser/prenotazione_move.py:32
-#: redturtle/prenotazioni/content/prenotazione.py:111
+#: redturtle/prenotazioni/browser/prenotazione_move.py:31
+#: redturtle/prenotazioni/content/prenotazione.py:114
 msgid "label_booking_time"
-msgstr "label_booking_time"
+msgstr ""
 
 #. Default: "Fullname"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:50
+#: redturtle/prenotazioni/browser/prenotazione_add.py:46
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:20
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:35
 msgid "label_booking_title"
-msgstr "label_booking_title"
+msgstr ""
 
 #. Default: "Booking type"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:59
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:34
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:24
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:44
 msgid "label_booking_type"
-msgstr "label_booking_type"
+msgstr ""
 
-#: redturtle/prenotazioni/vocabularies/requirable_booking_fields.py:22
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:262
+#: redturtle/prenotazioni/vocabularies/requirable_booking_fields.py:23
 msgid "label_booking_{}"
 msgstr ""
 
 #. Default: "End date"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:59
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:46
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:61
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:51
 msgid "label_end"
-msgstr "label_end"
+msgstr ""
 
 #. Default: "End time"
-#: redturtle/prenotazioni/browser/vacations.py:82
+#: redturtle/prenotazioni/browser/vacations.py:83
 msgid "label_end_time"
-msgstr "label_end_time"
+msgstr ""
 
 #. Default: "Gate"
-#: redturtle/prenotazioni/browser/prenotazione_move.py:34
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:47
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:109
+#: redturtle/prenotazioni/browser/prenotazione_move.py:32
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:49
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:83
 msgid "label_gate"
-msgstr "label_gate"
+msgstr ""
 
 #. Default: "Go to the booking to see more details and manage it: ${url}"
-#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:62
+#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:61
 msgid "label_new_booking_notify_link"
-msgstr "label_new_booking_notify_link"
+msgstr ""
 
 #. Default: "Required booking fields"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:143
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:151
 msgid "label_required_booking_fields"
-msgstr "label_required_booking_fields"
+msgstr ""
 
 #. Default: "Disallow same day booking"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:201
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:209
 msgid "label_same_day_booking_disallowed"
-msgstr "label_same_day_booking_disallowed"
+msgstr ""
 
 #. Default: "Selected date: ${date} — Time: ${slot}"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:153
+#: redturtle/prenotazioni/browser/prenotazione_add.py:147
 msgid "label_selected_date"
-msgstr "label_selected_date"
+msgstr ""
 
 #. Default: "Start date "
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:53
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:39
-#: redturtle/prenotazioni/browser/vacations.py:71
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:55
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:44
+#: redturtle/prenotazioni/browser/vacations.py:72
 msgid "label_start"
-msgstr "label_start"
+msgstr ""
 
 #. Default: "Start time"
-#: redturtle/prenotazioni/browser/vacations.py:76
+#: redturtle/prenotazioni/browser/vacations.py:77
 msgid "label_start_time"
-msgstr "label_start_time"
+msgstr ""
 
 #. Default: "Text to search"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:39
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:41
 msgid "label_text"
-msgstr "label_text"
+msgstr ""
 
 #. Default: "Reservation types"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:268
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:277
 msgid "label_tipologies"
-msgstr "label_tipologies"
+msgstr ""
 
 #. Default: "Title"
-#: redturtle/prenotazioni/browser/vacations.py:58
+#: redturtle/prenotazioni/browser/vacations.py:59
 msgid "label_title"
-msgstr "label_title"
+msgstr ""
 
 #. Default: "User"
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:37
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:42
 msgid "label_user"
-msgstr "label_user"
+msgstr ""
 
 #. Default: "Visible booking fields"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:161
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:169
 msgid "label_visible_booking_fields"
-msgstr "label_visible_booking_fields"
+msgstr ""
 
 #. Default: "Legend"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:290
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:299
 msgid "legend"
-msgstr "legend"
+msgstr ""
 
 #. Default: "Short description of available action for the booking board"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:291
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:300
 msgid "legend_description"
-msgstr "legend_description"
+msgstr ""
 
 #. Default: "The minimum value of a single slot is 5 minutes. You cannot book a reservation when the needed time exceeds the available time."
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:312
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:321
 msgid "legend_note"
-msgstr "legend_note"
+msgstr ""
 
 #. Default: "Type in here the message that you want to mail. Some defined content can be replaced: ${title} will be replaced with booking title (user fullname). ${date} will be replaced with booking new date. ${url} will be replaced by the booking url. ${portal} will be replaced by the title of the portal."
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:43
 msgid "message_help"
 msgstr ""
 
+#. Default: "Unable to find a booking with the givend id: ${uid}."
+#: redturtle/prenotazioni/browser/delete_reservation.py:42
+msgid "missing_booking"
+msgstr ""
+
+#. Default: "You need to provide a reservation id."
+#: redturtle/prenotazioni/browser/delete_reservation.py:36
+msgid "missing_uid"
+msgstr ""
+
+msgid "month_label"
+msgstr ""
+
 #. Default: "End time in the morning"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:72
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:75
 msgid "morning_end_label"
-msgstr "morning_end_label"
+msgstr ""
 
 #. Default: "Start time in the morning"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:67
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:70
 msgid "morning_start_label"
-msgstr "morning_start_label"
+msgstr ""
 
 #. Default: "Go back to the calendar"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:244
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:138
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:246
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:141
 #: redturtle/prenotazioni/browser/templates/prenotazione_add.pt:88
 msgid "move_back_message"
-msgstr "move_back_message"
+msgstr ""
 
 #. Default: "Move booking"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:118
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:121
 msgid "move_booking"
-msgstr "move_booking"
+msgstr ""
 
 #. Default: "Please move this booking into a new available slot or"
 #: redturtle/prenotazioni/browser/templates/prenotazione_move.pt:34
 msgid "move_message"
-msgstr "move_message"
+msgstr ""
 
 #. Default: "New booking for ${context}"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:409
+#: redturtle/prenotazioni/browser/prenotazione_add.py:388
 msgid "new_booking_admin_notify_subject"
-msgstr "new_booking_admin_notify_subject"
+msgstr ""
 
 #. Default: "next week"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:22
 msgid "next-week"
-msgstr "next-week"
-
-#. Default: "Seems your reservation is not existing"
-#: redturtle/prenotazioni/browser/delete_reservation.py:31
-msgid "no_reservation"
 msgstr ""
 
 #. Default: "Booking is not allowed before the amount of days specified. \nKeep 0 to give no limits."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:309
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:331
 msgid "notBeforeDays"
-msgstr "notBeforeDays"
+msgstr ""
 
 #. Default: "Pause end"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:116
 msgid "pause_end_label"
 msgstr ""
 
 #. Default: "Pause start"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:111
 msgid "pause_start_label"
 msgstr ""
 
 #. Default: "Please select a time slot"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:349
+#: redturtle/prenotazioni/browser/prenotazione_add.py:328
 msgid "please_pick_a_date"
-msgstr "please_pick_a_date"
+msgstr ""
 
 #. Default: "${day}, ore ${booking_time}"
-#: redturtle/prenotazioni/browser/week.py:237
+#: redturtle/prenotazioni/browser/week.py:256
 msgid "prenotation_slot_message"
 msgstr ""
 
 #. Default: "prenotazioni_search"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "prenotazioni_search"
-msgstr "List of contents"
+msgstr ""
 
 #. Default: "previous week"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:7
 msgid "previous-week"
-msgstr "previous-week"
+msgstr ""
 
-#: redturtle/prenotazioni/configure.zcml:30
+#: redturtle/prenotazioni/configure.zcml:31
 msgid "redturtle.prenotazioni"
-msgstr "redturtle.prenotazioni"
+msgstr ""
 
-#: redturtle/prenotazioni/configure.zcml:39
+#: redturtle/prenotazioni/configure.zcml:48
+msgid "redturtle.prenotazioni (to_1500)"
+msgstr ""
+
+#: redturtle/prenotazioni/configure.zcml:40
 msgid "redturtle.prenotazioni (uninstall)"
-msgstr "redturtle.prenotazioni (uninstall)"
+msgstr ""
+
+#: redturtle/prenotazioni/configure.zcml:48
+msgid "redturtle.prenotazioni to 1500."
+msgstr ""
 
 #. Default: "The booking state is \"refused\". If you change it, the booking time may conflict with another one."
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:23
 msgid "refused-review-state-warning"
-msgstr "refused-review-state-warning"
+msgstr ""
 
 #. Default: "Reject booking"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:128
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:131
 msgid "reject_booking"
-msgstr "reject_booking"
+msgstr ""
 
 #. Default: "Reminders"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:436
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:464
 msgid "reminders_label"
 msgstr ""
 
 #. Default: "Code"
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:41
 msgid "reservation_code"
 msgstr ""
 
 #. Default: "Reservation date"
 #: redturtle/prenotazioni/browser/templates/prenotazione_move.pt:28
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:40
 msgid "reservation_date"
-msgstr "reservation_date"
+msgstr ""
 
 #. Default: "Booking request for: ${name}"
 #: redturtle/prenotazioni/browser/prenotazione_print.py:29
 msgid "reservation_request"
-msgstr "reservation_request"
+msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:18
 msgid "resize"
-msgstr "resize"
+msgstr ""
 
 #. Default: "items matching your search terms."
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:19
 msgid "result_number"
-msgstr "result_number"
+msgstr ""
 
 #. Default: "Search by gate"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:308
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:317
 msgid "search-by-gate"
-msgstr "search-by-gate"
+msgstr ""
 
 #. Default: "Search result"
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:9
 msgid "search_result_message"
-msgstr "search_result_message"
+msgstr ""
 
 #. Default: "seleziona l'opzione desiderata dal gruppo di radio button seguente"
-#: redturtle/prenotazioni/browser/z3c_custom_widget.py:152
-#, fuzzy
+#: redturtle/prenotazioni/browser/z3c_custom_widget.py:153
 msgid "select-option"
-msgstr "select the desired option from the following group of fields"
+msgstr ""
 
 #. Default: "This gate has some booking schedule in this time period."
-#: redturtle/prenotazioni/browser/vacations.py:262
+#: redturtle/prenotazioni/browser/vacations.py:256
 msgid "slot_conflict_error"
-msgstr "slot_conflict_error"
+msgstr ""
 
 #. Default: "The email address that sends the email. If no email is provided here, it will use the address from portal."
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:33
 msgid "source_help"
-msgstr "source_help"
+msgstr ""
 
 #. Default: "You cannot book any booking_type at this time"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:353
+#: redturtle/prenotazioni/browser/prenotazione_add.py:332
 msgid "time_slot_to_short"
-msgstr "time_slot_to_short"
+msgstr ""
+
+msgid "to_label"
+msgstr ""
+
+#. Default: "You should set an end range."
+#: redturtle/prenotazioni/content/validators.py:174
+msgid "to_month_error"
+msgstr ""
+
+#. Default: "Selected day is too big for that month for \"to\" field."
+#: redturtle/prenotazioni/content/validators.py:181
+msgid "to_month_too_days_error"
+msgstr ""
 
 #. Default: "Add a gate here (one per line) if, for some reason, it is not be available.The specified gate will not be taken in to account for slot allocation. Each line should match a corresponding line in the \"Gates\" field"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:339
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:363
 msgid "unavailable_gates_help"
-msgstr "unavailable_gates_help"
+msgstr ""
 
 #. Default: "Unavailable gates"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:338
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:362
 msgid "unavailable_gates_label"
-msgstr "unavailable_gates_label"
+msgstr ""
 
 #. Default: "Unbookable time"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:295
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:304
 msgid "unbookable_time"
-msgstr "unbookable_time"
+msgstr ""
 
 #. Default: "vacation_booking"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "vacation_booking"
-msgstr "Resource lock"
+msgstr ""
 
 #. Default: "View booking"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:105
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:306
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:108
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:315
 msgid "view_booking"
-msgstr "view_booking"
+msgstr ""
+
+#. Default: "Insert here week schema for some custom date intervals."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:285
+msgid "week_table_overrides_help"
+msgstr ""
+
+#. Default: "Week table overrides"
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:284
+msgid "week_table_overrides_label"
+msgstr ""
+
+#. Default: "You tried to delete booking with a wrong action."
+#: redturtle/prenotazioni/browser/delete_reservation.py:95
+msgid "wrong_authenticator"
+msgstr ""
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,29 @@
 # Alessandro Pisa <alessandro.pisa@redturtle.it>, 2013, 2014.
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
-"POT-Creation-Date: 2022-02-25 07:58+0000\n"
+"POT-Creation-Date: 2023-05-30 12:50+0000\n"
 "PO-Revision-Date: 2014-05-27 17:36+0200\n"
 "Last-Translator: Alessandro Pisa <alessandro.pisa@redturtle.it>\n"
 "Language-Team: American English <kde-i18n-doc@kde.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: it\n"
 "Language-Name: Italian\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: redturtle.prenotazioni\n"
 "Language: en_US\n"
 "X-Generator: Lokalize 1.5\n"
 
-# Workflow prenotazioni_workflow states translation
-msgid "confirmed"
-msgstr "Confermato"
-
-msgid "refused"
-msgstr "Rifiutato"
-
-msgid "pending"
-msgstr "In attesa"
-
-msgid "private"
-msgstr "Privato"
-
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:54
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:40
-#: redturtle/prenotazioni/browser/vacations.py:72
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:56
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:45
+#: redturtle/prenotazioni/browser/vacations.py:73
 msgid " format (YYYY-MM-DD)"
 msgstr "Formato (AAAA-MM-GG)"
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "A folder that will contain booking"
 msgstr "Una cartella che conterrà le prenotazioni"
 
@@ -44,31 +31,35 @@
 msgid "A folder that will contain booking for this day"
 msgstr "Una cartella che conterrà le prenotazioni per questo day"
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:166
 msgid "A mail action that sends email notify when a booking is moved in an other slot."
 msgstr "Un'azione che spedisce una mail di notifica quando una prenotazione è spostata un un altro slot."
 
+msgid "Add"
+msgstr "Aggiungi"
+
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:165
 msgid "Add moved booking Mail Action"
 msgstr "Aggiungi Mail Action per lo spostamento delle prenotazioni"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:424
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:441
+#: redturtle/prenotazioni/content/validators.py:212
 msgid "Afternoon start should not be greater than end."
 msgstr "L'orario di inizio del pomeriggio non può essere successivo alla chiusura."
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:428
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:445
 msgid "App IO notification"
-msgstr ""
+msgstr "Notifiche App IO"
 
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:22
 msgid "Attention"
 msgstr "Attenzione!"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:26
+#: redturtle/prenotazioni/adapters/stringinterp.py:23
 msgid "Booking"
 msgstr "Prenotazioni"
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "Booking Folder"
 msgstr "Cartella prenotazioni"
 
@@ -94,50 +85,58 @@
 
 #. Default: "Change date/time"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "Change date/time"
 msgstr "Cambia la data di prenotazione."
 
 #. Default: "Complete address"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:392
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:416
 msgid "Complete address"
 msgstr "Indirizzo completo"
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:170
 msgid "Configure element"
 msgstr "Configura elemento"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:385
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:409
 msgid "Contact PEC"
 msgstr "Indirizzo PEC per il contatto"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:379
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:403
 msgid "Contact fax"
 msgstr "Numero di FAX per il contatto"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:373
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:397
 msgid "Contact phone"
 msgstr "Numero di telefono per il contatto"
 
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:31
 msgid "Content listing"
 msgstr "Elenco dei contenuti"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:181
+#. Default: "Cosa serve"
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:143
+msgid "Cosa serve"
+msgstr "Cosa serve"
+
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:189
 msgid "Data fine validità"
 msgstr "Data fine validità"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:178
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:186
 msgid "Data inizio validità"
 msgstr "Data inizio validità"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:308
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:330
 msgid "Days booking is not allowed before"
 msgstr "Giorni da cui si può effettuare una prenotazione"
 
+msgid "Delete"
+msgstr "Cancella"
+
 #. Default: "Descrizione Agenda"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:137
 msgid "Descrizione Agenda"
 msgstr "Descrizione Agenda"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:125
 msgid "Duration value"
@@ -149,142 +148,148 @@
 msgid "Edit"
 msgstr "Modifica"
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:185
 msgid "Edit moved booking Mail Action"
 msgstr "Modifica Mail Action per lo spostamento delle prenotazioni"
 
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:144
+msgid "Elencare le informazioni utili per il giorno della prenotazione, come ad esempio i documenti da presentare."
+msgstr "Elencare le informazioni utili per il giorno della prenotazione, come ad esempio i documenti da presentare."
+
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:72
 msgid "Email report to prenotazione owner"
 msgstr "Report email al creatore della prenotazione"
 
-#: redturtle/prenotazioni/content/prenotazione.py:159
+#: redturtle/prenotazioni/content/prenotazione.py:163
 msgid "Expiration date booking"
 msgstr "Data scandenza prenotazione"
 
 #. Default: "Campo"
-#: redturtle/prenotazioni/browser/z3c_custom_widget.py:149
+#: redturtle/prenotazioni/browser/z3c_custom_widget.py:150
 msgid "Field"
 msgstr "Campo"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:99
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:104
 msgid "Friday"
 msgstr "Venerdì"
 
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:81
-#: redturtle/prenotazioni/content/prenotazione.py:154
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:80
+#: redturtle/prenotazioni/content/prenotazione.py:158
 msgid "Gate"
 msgstr "Postazione"
 
+msgid "Group"
+msgstr "Gruppo"
+
 #. Default: "How to get here"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:368
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:392
 msgid "How to get here"
 msgstr "Indicazioni su come raggiungere l'ufficio"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:516
+#: redturtle/prenotazioni/content/validators.py:135
 msgid "In the same day there are overlapping intervals"
 msgstr "Ci sono pause che si sovrappongono nello stesso giorno"
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 msgid "Informations about a single booking"
 msgstr "Informazioni relativa ad una singola prenotazione"
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:138
 msgid "Inserire il testo di presentazione dell'agenda corrente"
-msgstr ""
+msgstr "Inserire il testo di presentazione dell'agenda corrente"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:357
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:381
 msgid "Insert a list of email addresses that will be notified when new bookings get created."
 msgstr "Inserisci una lista di indirizzi email che verranno notificati alla creazione di una nuova prenotazione."
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:369
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:393
 msgid "Insert here indications on how to reach the office"
 msgstr "Scrivere le indicazioni complete per raggiungere l'ufficio"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:393
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:417
 msgid "Insert here the complete office address"
 msgstr "Inserire l'indirizzo dell'ufficio"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:386
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:410
 msgid "Insert here the contact PEC"
 msgstr "Inserire l'indirizzo di posta PEC per contattare l'ufficio"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:380
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:404
 msgid "Insert here the contact fax"
 msgstr "Inserire il numero di FAX per per contattare l'ufficio"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:374
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:398
 msgid "Insert here the contact phone"
 msgstr "Inserire il numero di telefono per contattare l'ufficio"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:275
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:295
 msgid "Insert pause table schema."
 msgstr "Inserisci le pause giornaliere. Esistono tre tipi di vincolo: una data di termine pausa deve essere maggiore maggiore della data di inizio pausa; le pause nello stesso giorno non possono sovrapporsi; le pause devono essere comprese fra l'inizio e la fine dell'orario di lavoro."
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:216
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:224
 msgid "Insert week table schema."
 msgstr "Compila la tabella degli orari della settimana."
 
-#: redturtle/prenotazioni/configure.zcml:30
+#: redturtle/prenotazioni/configure.zcml:31
 msgid "Installs the redturtle.prenotazioni add-on."
 msgstr "Install redturtle.prenotazioni"
 
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:32
-msgid "Is not possible to delete your reservation"
-msgstr "Attenzione!"
-
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:35
-msgid "It's not possbile to delete your reservation. The url is broken or it's to late to delete it"
-msgstr "Non è stato possible cancellare la tua prenotazione. L'url non è corretto oppure è troppo tardi per cancellarla"
-
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:296
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:318
 msgid "Max days in the future"
 msgstr "Massimi giorni nel futuro"
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:42
 msgid "Message"
 msgstr "Messaggio"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:95
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:100
 msgid "Monday"
 msgstr "Lunedì"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:421
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:438
+#: redturtle/prenotazioni/content/validators.py:207
 msgid "Morning start should not be greater than end."
 msgstr "L'orario di inizio della mattina non può essere successivo alla fine."
 
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:111
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:114
 msgid "Move booking"
 msgstr "Sposta la prenotazione"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:194
+msgid "Move down"
+msgstr "Sposta in giù"
+
+msgid "Move up"
+msgstr "Sposta in su"
+
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:202
 msgid "No"
 msgstr "No"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:195
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:203
 msgid "No, just for today"
 msgstr "No, solo per oggi"
 
 #: redturtle/prenotazioni/content/pause.py:41
 msgid "Pause"
 msgstr "Pausa"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:487
+#: redturtle/prenotazioni/content/validators.py:99
 msgid "Pause end should be greater than pause start"
 msgstr "Il termine della pausa non può avvenire prima del suo inizio"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:504
+#: redturtle/prenotazioni/content/validators.py:120
 msgid "Pause should be included in morning slot or afternoon slot"
 msgstr "Le pause devono essere comprese tra l'orario di inizio o di termine dell'intervallo di orari di lavoro"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:274
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:294
 msgid "Pause table"
 msgstr "Schedulazione delle pause"
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:278
+#: redturtle/prenotazioni/browser/prenotazione_add.py:261
 msgid "Please provide a booking date"
 msgstr "Per favore seleziona una data."
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 msgid "Prenotazione"
 msgstr "Prenotazione"
 
@@ -296,769 +301,812 @@
 msgid "PrenotazioniWeek"
 msgstr "PrenotazioniWeek"
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
 msgid "PrenotazioniYear"
 msgstr "PrenotazioniYear"
 
-#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:107
+#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:106
 msgid "Print"
 msgstr "Stampa"
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:274
+#: redturtle/prenotazioni/configure.zcml:56
+msgid "Profile create to add the new default content rule: booking-confirm"
+msgstr "Profilo per creare una content-rule di default: booking-confirm"
+
+#: redturtle/prenotazioni/restapi/services/booking/add.py:34
+msgid "Required input '${field}' is missing."
+msgstr "Campo obbligatorio '${field}' mancante."
+
+#: redturtle/prenotazioni/browser/prenotazione_add.py:257
 msgid "Required input is missing."
 msgstr "Manca l'input obbligatorio."
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:356
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:380
 msgid "Responsible email"
 msgstr "Email del responsabile"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:100
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:105
 msgid "Saturday"
 msgstr "Sabato"
 
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:11
 msgid "Search for"
 msgstr "Parametri di ricerca"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:94
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:99
 msgid "Select a day"
 msgstr "Seleziona un giorno"
 
 #: redturtle/prenotazioni/contentrules/configure.zcml:57
 msgid "Send Email to booking owner when a booking is moved"
 msgstr "Invia un'email al creatore della prenotazione quando la prenotazione viene spostata."
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:32
 msgid "Sender email"
 msgstr "Indirizzo mittente"
 
-#: redturtle/prenotazioni/browser/delete_reservation.py:107
-msgid "Some information to delete your reservation is missing"
-msgstr "Ci sono informazioni mancanti per la cancellazione della tua prenotazione"
-
-#: redturtle/prenotazioni/browser/prenotazione_add.py:283
+#: redturtle/prenotazioni/browser/prenotazione_add.py:266
+#: redturtle/prenotazioni/restapi/services/booking/add.py:83
 msgid "Sorry, this slot is not available anymore."
 msgstr "Ci dispiace, ma questo intervallo di tempo non è più disponibile"
 
-#: redturtle/prenotazioni/browser/prenotazione_move.py:166
+#: redturtle/prenotazioni/browser/prenotazione_move.py:164
 msgid "Sorry, this slot is not available or does not fit your booking."
 msgstr "Ci dispiace questo intervallo di tempo non è disponibile o non è adatto alla tua prenotazione."
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:286
-#: redturtle/prenotazioni/browser/prenotazione_move.py:172
+#: redturtle/prenotazioni/browser/prenotazione_add.py:269
+#: redturtle/prenotazioni/browser/prenotazione_move.py:170
+#: redturtle/prenotazioni/restapi/services/booking/add.py:90
 msgid "Sorry, you can not book this slot for now."
 msgstr "Ci dispiace, ma questo intervallo di tempo non è al momento disponibile"
 
-#: redturtle/prenotazioni/content/prenotazione.py:155
+#: redturtle/prenotazioni/content/prenotazione.py:159
 msgid "Sportello a cui presentarsi"
 msgstr "Postazione a cui presentarsi"
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:26
 msgid "Subject"
 msgstr "Note"
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:27
 msgid "Subject of the message"
 msgstr "Oggetto del messaggio"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:101
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:106
 msgid "Sunday"
 msgstr "Domenica"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:37
+#: redturtle/prenotazioni/adapters/stringinterp.py:33
 msgid "The booked date."
 msgstr "La data di prenotazione."
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:51
+#: redturtle/prenotazioni/adapters/stringinterp.py:46
 msgid "The booked end date."
 msgstr "La data di fine prenotazione"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:65
+#: redturtle/prenotazioni/adapters/stringinterp.py:59
 msgid "The booked time."
 msgstr "L'orario di prenotazione"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:103
+#: redturtle/prenotazioni/adapters/stringinterp.py:94
 msgid "The booking code."
 msgstr "Il codice di prenotazione"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:228
+#: redturtle/prenotazioni/adapters/stringinterp.py:200
 msgid "The booking human readable date"
 msgstr "La data di prenotazione in formato leggibile"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:190
+#: redturtle/prenotazioni/adapters/stringinterp.py:166
 msgid "The booking office contact fax."
 msgstr "Il Fax per contattare l'ufficio"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:179
+#: redturtle/prenotazioni/adapters/stringinterp.py:156
 msgid "The booking office contact pec address."
 msgstr "L'indirizzo PEC per contattare l'ufficio"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:168
+#: redturtle/prenotazioni/adapters/stringinterp.py:146
 msgid "The booking office contact phone."
 msgstr "Il telefono per contattare l'ufficio"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:129
-msgid "The booking print url with delete token."
-msgstr "L'url per la cancellazione della prenotazione"
-
-#: redturtle/prenotazioni/adapters/stringinterp.py:116
+#: redturtle/prenotazioni/adapters/stringinterp.py:106
 msgid "The booking print url."
 msgstr "L'url per stampare la prenotazione"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:79
+#: redturtle/prenotazioni/adapters/stringinterp.py:72
 msgid "The booking time end."
 msgstr "L'orario di fine prenotazione"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:93
+#: redturtle/prenotazioni/adapters/stringinterp.py:85
 msgid "The booking type."
 msgstr "La tipologia della prenotazione."
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:256
+#: redturtle/prenotazioni/adapters/stringinterp.py:227
 msgid "The booking url with delete token"
 msgstr "L'url della prenotazione con il token per la cancellazione"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:214
+#: redturtle/prenotazioni/adapters/stringinterp.py:188
 msgid "The complete address information of the office whereuser book a reservation"
 msgstr "L'indirizzo completo dell'ufficio presso cui si prenota"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:158
+#: redturtle/prenotazioni/adapters/stringinterp.py:137
 msgid "The email address of the user who made the reservation."
 msgstr "L'indirizzo email dell'utente che ha fatto la prenotazione"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:27
+#: redturtle/prenotazioni/adapters/stringinterp.py:24
 msgid "The gate booked."
 msgstr "La postazione prenotata."
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:201
+#: redturtle/prenotazioni/adapters/stringinterp.py:176
 msgid "The information to reach the office where user book a reservation"
 msgstr "Le informazioni per raggiungere l'ufficio presso cui si prenota"
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:148
+#: redturtle/prenotazioni/adapters/stringinterp.py:128
 msgid "The phone number of the user who made the reservation."
 msgstr "Il numero di telefono di chi ha prenotato"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:98
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:103
 msgid "Thursday"
 msgstr "Giovedì"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:96
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:101
 msgid "Tuesday"
 msgstr "Martedì"
 
-#: redturtle/prenotazioni/configure.zcml:39
+#: redturtle/prenotazioni/configure.zcml:40
 msgid "Uninstalls the redturtle.prenotazioni add-on."
 msgstr "Disinstall redturtle.prenotazioni"
 
+#: redturtle/prenotazioni/restapi/services/booking/add.py:66
+msgid "Unknown booking type '${booking_type}'."
+msgstr "Tipologia di prenotazione sconosciuta '${booking_type}'."
+
+#: redturtle/prenotazioni/configure.zcml:56
+msgid "Used to add new contentrules"
+msgstr "Aggiunge una nuova contentrule"
+
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "View"
 msgstr "Vista"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:97
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:102
 msgid "Wednesday"
 msgstr "Mercoledì"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:215
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:223
 msgid "Week table"
 msgstr "Schedulazione settimanale"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:193
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:201
 msgid "Yes"
 msgstr "Si"
 
-#: redturtle/prenotazioni/browser/delete_reservation.py:85
-msgid "You can't delete your reservation; it's too late"
-msgstr "Hai superato il tempo massimo per cancellare la prenotazione"
-
-#: redturtle/prenotazioni/browser/delete_reservation.py:72
-msgid "You can't delete your reservation; please contact the office"
-msgstr "Non puoi cancellare la tua prenotazione. Contattare l'ufficio"
-
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:483
+#: redturtle/prenotazioni/content/validators.py:91
 msgid "You must set both start and end"
 msgstr "Devi impostare sia un orario di inizio che di termine della pausa"
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:418
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:435
+#: redturtle/prenotazioni/content/validators.py:202
 msgid "You should set a start time for afternoon."
 msgstr "Devi impostare una data di inizio per il pomeriggio."
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:414
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:431
+#: redturtle/prenotazioni/content/validators.py:194
 msgid "You should set a start time for morning."
 msgstr "Devi impostare una data di inizio per la mattina."
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:416
-msgid "You should set and end time for afternoon."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:433
+#: redturtle/prenotazioni/content/validators.py:198
+msgid "You should set an end time for afternoon."
 msgstr "Devi impostare una data di fine per il pomeriggio."
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:412
-msgid "You should set and end time for morning."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:429
+#: redturtle/prenotazioni/content/validators.py:190
+msgid "You should set an end time for morning."
 msgstr "Devi impostare una data di fine per la mattina."
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:409
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:426
 msgid "You should set at least one booking type."
 msgstr "Devi impostare almeno una tipologia di prenotazione."
 
-#: redturtle/prenotazioni/browser/delete_reservation.py:94
-msgid "Your reservation has been deleted"
-msgstr "La tua prenotazione è stata cancellata"
+#: redturtle/prenotazioni/adapters/stringinterp.py:122
+msgid "[DEPRECATED] The booking print url with delete token."
+msgstr "[DEPRECATO] L'url della prenotazione con il token per la cancellazione."
 
 #. Default: "Leave empty, and this Booking Folder will never expire"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:182
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:190
 msgid "aData_help"
 msgstr "Lascia vuoto, e questa Cartella Prenotazioni non avrà scadenza"
 
 #. Default: "Book"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:256
-#: redturtle/prenotazioni/browser/vacations.py:252
+#: redturtle/prenotazioni/browser/prenotazione_add.py:239
+#: redturtle/prenotazioni/browser/vacations.py:246
 msgid "action_book"
 msgstr "Prenota"
 
 #. Default: "Cancel"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:321
-#: redturtle/prenotazioni/browser/prenotazione_move.py:187
-#: redturtle/prenotazioni/browser/vacations.py:277
+#: redturtle/prenotazioni/browser/prenotazione_add.py:300
+#: redturtle/prenotazioni/browser/prenotazione_move.py:185
+#: redturtle/prenotazioni/browser/vacations.py:271
 msgid "action_cancel"
 msgstr "Cancella"
 
 #. Default: "Move"
-#: redturtle/prenotazioni/browser/prenotazione_move.py:151
+#: redturtle/prenotazioni/browser/prenotazione_move.py:149
 msgid "action_move"
 msgstr "Sposta"
 
 #. Default: "Search"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:234
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:236
 msgid "action_search"
 msgstr "Cerca"
 
 #. Default: "End time in the afternoon"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:84
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:87
 msgid "afternoon_end_label"
 msgstr "Chiusura pomeriggio"
 
 #. Default: "Start time in the afternoon"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:78
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:81
 msgid "afternoon_start_label"
 msgstr "Apertura pomeriggio"
 
 #. Default: "Please select a booking slot."
 #: redturtle/prenotazioni/browser/templates/week.pt:28
 msgid "book_it"
 msgstr "Per favore seleziona uno slot per la prenotazione"
 
 #. Default: "Bookable time"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:297
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:306
 msgid "bookable_time"
 msgstr "Tempo prenotabile "
 
 #. Default: "${day}, ore ${booking_time}, prenotato da ${booked_by}, prenotazione: ${booking_type} durata: ${duration} minuti"
-#: redturtle/prenotazioni/browser/week.py:257
+#: redturtle/prenotazioni/browser/week.py:276
 msgid "booked_prenotation_message"
-msgstr ""
+msgstr "${day}, ore ${booking_time}, prenotato da ${booked_by}, prenotazione: ${booking_type} durata: ${duration} minuti"
 
 #. Default: "Booking confirmed"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:299
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:308
 msgid "booking_confirmed"
 msgstr "Prenotazione confermata"
 
 #. Default: "Booking created"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:303
-#: redturtle/prenotazioni/browser/vacations.py:249
+#: redturtle/prenotazioni/browser/prenotazione_add.py:278
+#: redturtle/prenotazioni/browser/vacations.py:243
 msgid "booking_created"
 msgstr "Prenotazione creata"
 
-#: redturtle/prenotazioni/browser/prenotazione_move.py:177
+#. Default: "Your booking has been deleted."
+#: redturtle/prenotazioni/browser/delete_reservation.py:112
+msgid "booking_deleted_success"
+msgstr "La tua prenotazione è stata cancellata."
+
+#: redturtle/prenotazioni/browser/prenotazione_move.py:175
 msgid "booking_moved"
 msgstr "Prenotazione spostata correttamente"
 
 #. Default: "Booking pending"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:301
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:310
 msgid "booking_pending"
 msgstr "Prenotazione da confermare"
 
 #. Default: "Booking refused"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:303
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:312
 msgid "booking_refused"
 msgstr "Prenotazione rifiutata "
 
 #. Default: "Name"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:272
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:281
 msgid "booking_type_name"
 msgstr "Nome"
 
 #. Default: "Value"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:273
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:282
 msgid "booking_type_value"
 msgstr "Durata"
 
 #. Default: "You may want to select another time slot to book one of these."
 #: redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt:55
 msgid "booking_type_widget_suggest_reselect"
 msgstr "Prova a selezionare un'orario differente per prenotarle."
 
 #. Default: "The following tipologies will not fit the time you selected:"
 #: redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt:45
 msgid "booking_type_widget_warn_unavailable"
 msgstr "Le seguenti tipologie non sono selezionabili nell'orario selezionato:"
 
 #. Default: "Put booking types there (one per line).\nIf you do not provide this field, not type selection will be available"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:319
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:341
 msgid "booking_types_help"
 msgstr "Inserisci le tipologie di prenotazioni."
 
 #. Default: "Booking types"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:318
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:340
 msgid "booking_types_label"
 msgstr "Tipologie di prenotazioni"
 
 #. Default: "Bookings not in agenda"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:63
 msgid "bookings_not_in_agenda"
 msgstr "Prenotazioni non in agenda"
 
 #. Default: "Busy"
-#: redturtle/prenotazioni/browser/prenotazioni_context_state.py:76
+#: redturtle/prenotazioni/browser/prenotazioni_context_state.py:81
 msgid "busy"
 msgstr "Occupato"
 
 #. Default: "Your booking has to be confirmed by the administrators"
 #: redturtle/prenotazioni/browser/prenotazione_print.py:19
 msgid "confirm_booking_waiting_message"
 msgstr "La tua prenotazione deve essere confermata dagli amministratori"
 
 #. Default: "Show here contacts information that will be used by authomatic mail system"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:399
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:455
 msgid "contacts_help"
 msgstr "Indicare tutte le informazioni di contatto che saranno usate dal sistema  di mailing. Queste informazioni saranno usate tramite sostituzione di un testo di markup nelle \"Regole di contenuto\" pertanto qui ci sarà da inserire dei testi che si possano integrare correttamente con i testi delle regole."
 
 #. Default: "Contacts"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:398
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:454
 msgid "contacts_label"
 msgstr "Contatti"
 
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:23
-msgid "damn"
-msgstr "Attenzione!"
+#. Default: "Cosa serve"
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:96
+msgid "cosa_serve"
+msgstr "Cosa serve"
 
 #. Default: "This day is not valid."
-#: redturtle/prenotazioni/browser/vacations.py:269
+#: redturtle/prenotazioni/browser/vacations.py:263
 msgid "day_error"
 msgstr "Questo day non è valido"
 
 #. Default: "Day of week"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:64
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:67
 msgid "day_label"
 msgstr "Giorno"
 
+#. Default: "You can't delete your reservation; it's too late."
+#: redturtle/prenotazioni/browser/delete_reservation.py:137
+msgid "delete_expired_booking"
+msgstr "Non puoi cancellare questa prenotazione; è troppo tardi."
+
 #. Default: "Delete reservation request for: ${name}"
-#: redturtle/prenotazioni/browser/delete_reservation.py:20
+#: redturtle/prenotazioni/browser/delete_reservation.py:59
 msgid "delete_reservation_request"
 msgstr "Cancella la richiesta di prenotazione per: ${name}"
 
-#. Default: "Your reservation has been deleted"
-#: redturtle/prenotazioni/browser/delete_reservation.py:41
-msgid "deleted_reservation"
-msgstr "La tua prenotazione è stata cancellata"
-
 #. Default: "If you work for a company, please specify its name."
-#: redturtle/prenotazioni/content/prenotazione.py:146
+#: redturtle/prenotazioni/content/prenotazione.py:149
 msgid "description_company"
 msgstr "Se lavori per un'azienda, compila questo campo."
 
 #. Default: "The gate that will be unavailable"
-#: redturtle/prenotazioni/browser/vacations.py:66
+#: redturtle/prenotazioni/browser/vacations.py:67
 msgid "description_gate"
 msgstr "La postazione che non sarà disponibile."
 
 #. Default: "This text will appear in the calendar cells"
-#: redturtle/prenotazioni/browser/vacations.py:59
+#: redturtle/prenotazioni/browser/vacations.py:60
 msgid "description_title"
 msgstr "Questo testo apparirà nelle celle del calendario."
 
 #. Default: "Foreseen booking time: ${booking_time}"
-#: redturtle/prenotazioni/browser/week.py:206
+#: redturtle/prenotazioni/browser/week.py:225
 msgid "foreseen_booking_time"
 msgstr "Data prevista per la prenotazione: ${day}, alle ore ${booking_time}."
 
 #. Default: "${booking_time}, Orario non disponibile"
-#: redturtle/prenotazioni/browser/week.py:225
+#: redturtle/prenotazioni/browser/week.py:244
 msgid "foreseen_busy_time"
 msgstr "${booking_time}, Orario non disponibile."
 
+msgid "from_label"
+msgstr "Dal"
+
+#. Default: "You should set a start range."
+#: redturtle/prenotazioni/content/validators.py:159
+msgid "from_month_error"
+msgstr "Devi impostare una data di inizio."
+
+#. Default: "Selected day is too big for that month for \"from\" field."
+#: redturtle/prenotazioni/content/validators.py:166
+msgid "from_month_too_days_error"
+msgstr "Il giorno selezionato non è corretto per il mese selezionato nel campo \"Al\"."
+
 #. Default: "Fullname"
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:40
 msgid "fullname"
 msgstr "Nome completo"
 
 #. Default: "Limit booking in the future to an amount of days in the future starting from the current day. \nKeep 0 to give no limits."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:297
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:319
 msgid "futureDays"
 msgstr "Limita la prenotazione ad un certo numero di giorni nel futuro partendo dal day corrente.Lascia 0 per non dare limiti."
 
 #. Default: "Put gates here (one per line)."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:331
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:355
 msgid "gates_help"
 msgstr "Inserisci le postazioni preposte (uno per riga)."
 
 #. Default: "Gates"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:330
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:354
 msgid "gates_label"
 msgstr "Postazioni preposte"
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:165
+#: redturtle/prenotazioni/browser/prenotazione_add.py:162
 msgid "help_prenotazione_add"
 msgstr ""
 
 #. Default: "User will not be able to add a booking unless those fields are filled. Remember that, whatever you selected in this list, users have to supply at least one of \"Email\", \"Mobile\", or \"Telephone\""
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:144
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:152
 msgid "help_required_booking_fields"
 msgstr "Gli utenti non saranno in grado di creare una prenotazione senza compilare i seguenti campi. Gli utenti saranno comunque sempre obbligati ad inserire un'email o un recapito telefonico."
 
 #. Default: "States if it is not allowed to reserve a booking during the current day"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:205
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:213
 msgid "help_same_day_booking_disallowed"
 msgstr "Se selezionato, impedisce agli utenti di prenotare per il giorno corrente."
 
 #. Default: "List of available reservation type for the current agenda"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:269
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:278
 msgid "help_tipologies"
 msgstr "Lista dei tipi di prenotazione disponibili per l'agenda corrente"
 
 #. Default: "User will not be able to add a booking unless those fields are filled. Remember that, whatever you selected in this list, users have to supply at least one of \"Email\" or \"Telephone\""
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:162
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:170
 msgid "help_visible_booking_fields"
 msgstr "Gli utenti vedranno solo i campi selezionati all'atto della creazione della prenotazione."
 
 #. Default: "Set holidays (one for line) in DD/MM/YYYY. you can write * for the year, if this event is yearly."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:283
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:305
 msgid "holidays_help"
 msgstr "Imposta eventuali festività (una per riga) nel formato GG/MM/AAAA. Se la data si ripete ogni anno, puoi scrivere * al posto dell'anno."
 
 #. Default: "Holidays"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:282
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:304
 msgid "holidays_label"
 msgstr "Festività"
 
 #. Default: "Date should be in the format YYYY/mm/dd"
-#: redturtle/prenotazioni/browser/vacations.py:30
+#: redturtle/prenotazioni/browser/vacations.py:31
 msgid "invalid_date"
 msgstr "La data deve essere nel formato AAAA/MM/GG"
 
 #. Default: "Invalid email address"
-#: redturtle/prenotazioni/content/prenotazione.py:26
+#: redturtle/prenotazioni/content/prenotazione.py:28
 msgid "invalid_email_address"
 msgstr "Indirizzo email non valido"
 
 #. Default: "Invalid start or end date"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:31
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:20
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:33
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:25
 msgid "invalid_end:search_date"
 msgstr "Data di ricerca non valilda"
 
 #. Default: "Invalid fiscal code"
-#: redturtle/prenotazioni/content/prenotazione.py:34
+#: redturtle/prenotazioni/content/prenotazione.py:36
 msgid "invalid_fiscalcode"
 msgstr "Codice fiscale non valido"
 
 #. Default: "Invalid phone number"
-#: redturtle/prenotazioni/content/prenotazione.py:22
+#: redturtle/prenotazioni/content/prenotazione.py:24
 msgid "invalid_phone_number"
 msgstr "Numero di telefono non valido"
 
 #. Default: "Date should be in the format HH:MM"
-#: redturtle/prenotazioni/browser/vacations.py:34
+#: redturtle/prenotazioni/browser/vacations.py:35
 msgid "invalid_time"
 msgstr "L'ora deve essere nel formato HH:MM"
 
 #. Default: "This date is past"
-#: redturtle/prenotazioni/content/prenotazione.py:30
+#: redturtle/prenotazioni/content/prenotazione.py:32
 msgid "is_not_future_date"
 msgstr "La data è nel passato."
 
 #. Default: "Booking code"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:115
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:93
-#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:93
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:89
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:92
+#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:92
 msgid "label_booking_code"
 msgstr "Codice prenotazione"
 
 #. Default: "Company"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:77
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:52
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:36
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:57
 msgid "label_booking_company"
 msgstr "Azienda"
 
 #. Default: "Booking date"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:95
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:70
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:48
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:69
 msgid "label_booking_date"
 msgstr "Data prenotazione"
 
-#. Default: "${from_date} from ${from} to ${to}"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:103
-#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:52
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:76
+#. Default: "${from_date} at ${at}"
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:77
+#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:51
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:75
 msgid "label_booking_date_range"
 msgstr "${from_date} alle ore ${at}"
 
 #. Default: "Subject"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:53
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:89
+#: redturtle/prenotazioni/browser/prenotazione_add.py:49
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:64
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:44
 msgid "label_booking_description"
 msgstr "Note"
 
 #. Default: "Email"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:65
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:40
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:28
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:48
 msgid "label_booking_email"
 msgstr "Email"
 
 #. Default: "Fiscal code"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:83
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:58
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:40
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:61
 msgid "label_booking_fiscalcode"
 msgstr "Codice fiscale"
 
 #. Default: "Phone number"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:71
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:46
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:32
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:53
 msgid "label_booking_phone"
 msgstr "Numero di telefono"
 
 #. Default: "Staff notes"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:85
-#: redturtle/prenotazioni/content/prenotazione.py:163
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:84
+#: redturtle/prenotazioni/content/prenotazione.py:167
 msgid "label_booking_staff_notes"
 msgstr "Note del personale"
 
 #. Default: "Booking time"
-#: redturtle/prenotazioni/browser/prenotazione_move.py:32
-#: redturtle/prenotazioni/content/prenotazione.py:111
+#: redturtle/prenotazioni/browser/prenotazione_move.py:31
+#: redturtle/prenotazioni/content/prenotazione.py:114
 msgid "label_booking_time"
 msgstr "Data e ora"
 
 #. Default: "Fullname"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:50
+#: redturtle/prenotazioni/browser/prenotazione_add.py:46
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:20
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:35
 msgid "label_booking_title"
 msgstr "Nome completo"
 
 #. Default: "Booking type"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:59
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:34
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:24
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:44
 msgid "label_booking_type"
 msgstr "Tipologia prenotazione"
 
-#: redturtle/prenotazioni/vocabularies/requirable_booking_fields.py:22
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:262
+#: redturtle/prenotazioni/vocabularies/requirable_booking_fields.py:23
 msgid "label_booking_{}"
 msgstr ""
 
 #. Default: "End date"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:59
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:46
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:61
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:51
 msgid "label_end"
 msgstr "Data fine"
 
 #. Default: "End time"
-#: redturtle/prenotazioni/browser/vacations.py:82
+#: redturtle/prenotazioni/browser/vacations.py:83
 msgid "label_end_time"
 msgstr "Ora fine"
 
 #. Default: "Gate"
-#: redturtle/prenotazioni/browser/prenotazione_move.py:34
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:47
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:109
+#: redturtle/prenotazioni/browser/prenotazione_move.py:32
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:49
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:83
 msgid "label_gate"
 msgstr "Postazione"
 
 #. Default: "Go to the booking to see more details and manage it: ${url}"
-#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:62
+#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:61
 msgid "label_new_booking_notify_link"
 msgstr "Vai alla prenotazione per gestirla e vedere maggiori dettagli: ${url}"
 
 #. Default: "Required booking fields"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:143
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:151
 msgid "label_required_booking_fields"
 msgstr "Campi obbligatori"
 
 #. Default: "Disallow same day booking"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:201
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:209
 msgid "label_same_day_booking_disallowed"
 msgstr "Disabilita la prenotazione per lo stesso giorno"
 
 #. Default: "Selected date: ${date} — Time: ${slot}"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:153
+#: redturtle/prenotazioni/browser/prenotazione_add.py:147
 msgid "label_selected_date"
 msgstr "Data selezionata: ${date} — Alle ore: ${slot}"
 
 #. Default: "Start date "
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:53
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:39
-#: redturtle/prenotazioni/browser/vacations.py:71
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:55
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:44
+#: redturtle/prenotazioni/browser/vacations.py:72
 msgid "label_start"
 msgstr "Data inizio"
 
 #. Default: "Start time"
-#: redturtle/prenotazioni/browser/vacations.py:76
+#: redturtle/prenotazioni/browser/vacations.py:77
 msgid "label_start_time"
 msgstr "Ora inizio"
 
 #. Default: "Text to search"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:39
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:41
 msgid "label_text"
 msgstr "Testo da ricercare"
 
 #. Default: "Reservation types"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:268
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:277
 msgid "label_tipologies"
 msgstr "Tipi di prenotazione"
 
 #. Default: "Title"
-#: redturtle/prenotazioni/browser/vacations.py:58
+#: redturtle/prenotazioni/browser/vacations.py:59
 msgid "label_title"
 msgstr "Etichetta"
 
 #. Default: "User"
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:37
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:42
 msgid "label_user"
 msgstr "Utente"
 
 #. Default: "Visible booking fields"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:161
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:169
 msgid "label_visible_booking_fields"
 msgstr "Campi da visualizzare"
 
 #. Default: "Legend"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:290
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:299
 msgid "legend"
 msgstr "Legenda"
 
 #. Default: "Short description of available action for the booking board"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:291
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:300
 msgid "legend_description"
 msgstr "Breve descrizione delle azioni disponibili per l'agenda"
 
 #. Default: "The minimum value of a single slot is 5 minutes. You cannot book a reservation when the needed time exceeds the available time."
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:312
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:321
 msgid "legend_note"
 msgstr "L'unità di tempo minima è 5 minuti. La tua prenotazione non può eccedere il tempo disponibile."
 
 #. Default: "Type in here the message that you want to mail. Some defined content can be replaced: ${title} will be replaced with booking title (user fullname). ${date} will be replaced with booking new date. ${url} will be replaced by the booking url. ${portal} will be replaced by the title of the portal."
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:43
 msgid "message_help"
 msgstr "Inserisci il messaggio che vuoi inviare per mail. E' possibile inserire alcuni marcatori che verranno sostituiti con dei valori presi dall'applicazione.\"${title}\" sarà sostituito con il titolo della prenotazione (il nome e cognome dell'utente). \"${date}\" sarà sostituito con la data della prenotazione. \"${url}\" sarà sostituito  dall'url della prenotazione. ${portal} sarà sostituito  con il titolo del portale. "
 
+#. Default: "Unable to find a booking with the givend id: ${uid}."
+#: redturtle/prenotazioni/browser/delete_reservation.py:42
+msgid "missing_booking"
+msgstr "Impossibile trovare la prenotazione con id: ${uid}."
+
+#. Default: "You need to provide a reservation id."
+#: redturtle/prenotazioni/browser/delete_reservation.py:36
+msgid "missing_uid"
+msgstr "Devi fornite un'id prenotazione."
+
+#. Default: "End time in the morning"
+msgid "month_label"
+msgstr "Mese"
+
 #. Default: "End time in the morning"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:72
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:75
 msgid "morning_end_label"
 msgstr "Chiusura mattina"
 
 #. Default: "Start time in the morning"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:67
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:70
 msgid "morning_start_label"
 msgstr "Apertura mattina"
 
 #. Default: "Go back to the calendar"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:244
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:138
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:246
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:141
 #: redturtle/prenotazioni/browser/templates/prenotazione_add.pt:88
 msgid "move_back_message"
 msgstr "Ritorna al calendario"
 
 #. Default: "Move booking"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:118
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:121
 msgid "move_booking"
 msgstr "Sposta la prenotazione"
 
 #. Default: "Please move this booking into a new available slot or"
 #: redturtle/prenotazioni/browser/templates/prenotazione_move.pt:34
 msgid "move_message"
 msgstr "Spostare l'appuntamento selezionato in un area libera oppure"
 
 #. Default: "New booking for ${context}"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:409
+#: redturtle/prenotazioni/browser/prenotazione_add.py:388
 msgid "new_booking_admin_notify_subject"
 msgstr "Nuova prenotazione per ${context}"
 
 #. Default: "next week"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:22
 msgid "next-week"
 msgstr "Settimana successiva"
 
-#. Default: "Seems your reservation is not existing"
-#: redturtle/prenotazioni/browser/delete_reservation.py:31
-msgid "no_reservation"
-msgstr "Sembra che la tua prenotazione non esista. Se non l'hai già cancellata, per favore contatta l'ufficio o procedi con un'altra prenotazione."
-
 #. Default: "Booking is not allowed before the amount of days specified. \nKeep 0 to give no limits."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:309
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:331
 msgid "notBeforeDays"
 msgstr "La prenotazione non e' permessa prima del numero di giorni specificata. Impostare il valore 0 per non imporre limitazioni."
 
 #. Default: "Pause end"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:116
 msgid "pause_end_label"
 msgstr "Termine pausa"
 
 #. Default: "Pause start"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:111
 msgid "pause_start_label"
 msgstr "Inizio pausa"
 
 #. Default: "Please select a time slot"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:349
+#: redturtle/prenotazioni/browser/prenotazione_add.py:328
 msgid "please_pick_a_date"
 msgstr "Selezionare una data"
 
 #. Default: "${day}, ore ${booking_time}"
-#: redturtle/prenotazioni/browser/week.py:237
+#: redturtle/prenotazioni/browser/week.py:256
 msgid "prenotation_slot_message"
-msgstr ""
+msgstr "${day}, ore ${booking_time}"
 
 #. Default: "prenotazioni_search"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "prenotazioni_search"
 msgstr "Ricerca"
 
 #. Default: "previous week"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:7
 msgid "previous-week"
 msgstr "Settimana precedente"
 
-#: redturtle/prenotazioni/configure.zcml:30
+#: redturtle/prenotazioni/configure.zcml:31
 msgid "redturtle.prenotazioni"
 msgstr "redturtle.prenotazioni"
 
-#: redturtle/prenotazioni/configure.zcml:39
+#: redturtle/prenotazioni/configure.zcml:48
+msgid "redturtle.prenotazioni (to_1500)"
+msgstr "redturtle.prenotazioni (to_1500)"
+
+#: redturtle/prenotazioni/configure.zcml:40
 msgid "redturtle.prenotazioni (uninstall)"
 msgstr "redturtle.prenotazioni (disinstalla)"
 
+#: redturtle/prenotazioni/configure.zcml:48
+msgid "redturtle.prenotazioni to 1500."
+msgstr "redturtle.prenotazioni to 1500."
+
 #. Default: "The booking state is \"refused\". If you change it, the booking time may conflict with another one."
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:23
 msgid "refused-review-state-warning"
 msgstr "Lo stato della prenotazione è \"rifiutato\". Se lo cambi, questa prenotazione potrebbe entrare in conflitto con un'altra."
 
 #. Default: "Reject booking"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:128
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:131
 msgid "reject_booking"
 msgstr "Rifiuta la prenotazione"
 
 #. Default: "Reminders"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:436
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:464
 msgid "reminders_label"
-msgstr ""
+msgstr "Promemoria"
 
 #. Default: "Code"
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:41
 msgid "reservation_code"
 msgstr "Codice prenotazione"
 
 #. Default: "Reservation date"
@@ -1078,62 +1126,89 @@
 
 #. Default: "items matching your search terms."
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:19
 msgid "result_number"
 msgstr "elementi trovati"
 
 #. Default: "Search by gate"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:308
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:317
 msgid "search-by-gate"
 msgstr "Ricerca per postazione"
 
 #. Default: "Search result"
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:9
 msgid "search_result_message"
 msgstr "Risultato della ricerca"
 
 #. Default: "seleziona l'opzione desiderata dal gruppo di radio button seguente"
-#: redturtle/prenotazioni/browser/z3c_custom_widget.py:152
-#, fuzzy
+#: redturtle/prenotazioni/browser/z3c_custom_widget.py:153
 msgid "select-option"
 msgstr "seleziona l'opzione desiderata dal gruppo di campi seguente"
 
 #. Default: "This gate has some booking schedule in this time period."
-#: redturtle/prenotazioni/browser/vacations.py:262
+#: redturtle/prenotazioni/browser/vacations.py:256
 msgid "slot_conflict_error"
 msgstr "Questa postazione ha già appuntamenti schedulati in questo periodo."
 
 #. Default: "The email address that sends the email. If no email is provided here, it will use the address from portal."
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:33
 msgid "source_help"
 msgstr "Il mittente della mail. Se nessun indirizzo viene inserito verrà utilizzato l'indirizzo configurato nel portale."
 
 #. Default: "You cannot book any booking_type at this time"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:353
+#: redturtle/prenotazioni/browser/prenotazione_add.py:332
 msgid "time_slot_to_short"
 msgstr "Tempo insufficiente per qualsiasi tipologia di prenotazione"
 
+msgid "to_label"
+msgstr "Al"
+
+#. Default: "You should set an end range."
+#: redturtle/prenotazioni/content/validators.py:174
+msgid "to_month_error"
+msgstr "Devi impostare una data di inizio."
+
+#. Default: "Selected day is too big for that month for \"to\" field."
+#: redturtle/prenotazioni/content/validators.py:181
+msgid "to_month_too_days_error"
+msgstr "Il giorno selezionato non è compatibile col mese selezionato nel campo \"Al\"."
+
 #. Default: "Add a gate here (one per line) if, for some reason, it is not be available.The specified gate will not be taken in to account for slot allocation. Each line should match a corresponding line in the \"Gates\" field"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:339
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:363
 msgid "unavailable_gates_help"
 msgstr "Aggiungi una postazione (uno per riga) se, per qualche motivo, non è disponibile. La postazione specificata non sarà considerata per l'allocazione degli appuntamenti. Le righe devono essere uguali a quelle nel campo \"Postazioni preposte\"."
 
 #. Default: "Unavailable gates"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:338
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:362
 msgid "unavailable_gates_label"
 msgstr "Postazioni non disponibili"
 
 #. Default: "Unbookable time"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:295
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:304
 msgid "unbookable_time"
 msgstr "Tempo non prenotabile "
 
 #. Default: "vacation_booking"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "vacation_booking"
 msgstr "Blocco risorsa"
 
 #. Default: "View booking"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:105
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:306
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:108
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:315
 msgid "view_booking"
 msgstr "Vedi la prenotazione"
+
+#. Default: "Insert here week schema for some custom date intervals."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:285
+msgid "week_table_overrides_help"
+msgstr "Inserisci qui eventuali personalizzazioni nella schedulazione settimanale che andranno a vincere su quella standard per un determinato periodo di tempo."
+
+#. Default: "Week table overrides"
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:284
+msgid "week_table_overrides_label"
+msgstr "Personalizzazioni schedulazione settimanale"
+
+#. Default: "You tried to delete booking with a wrong action."
+#: redturtle/prenotazioni/browser/delete_reservation.py:95
+msgid "wrong_authenticator"
+msgstr "Stai cercando di cancellare una prenotazione con un'azione sbagliata."
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2022-02-25 07:58+0000\n"
+"POT-Creation-Date: 2023-05-30 12:51+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: redturtle.prenotazioni\n"
 
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:54
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:40
-#: redturtle/prenotazioni/browser/vacations.py:72
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:56
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:45
+#: redturtle/prenotazioni/browser/vacations.py:73
 msgid " format (YYYY-MM-DD)"
 msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "A folder that will contain booking"
 msgstr ""
 
@@ -31,31 +31,35 @@
 msgid "A folder that will contain booking for this day"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:166
 msgid "A mail action that sends email notify when a booking is moved in an other slot."
 msgstr ""
 
+msgid "Add"
+msgstr ""
+
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:165
 msgid "Add moved booking Mail Action"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:424
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:441
+#: redturtle/prenotazioni/content/validators.py:212
 msgid "Afternoon start should not be greater than end."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:428
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:445
 msgid "App IO notification"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:22
 msgid "Attention"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:26
+#: redturtle/prenotazioni/adapters/stringinterp.py:23
 msgid "Booking"
 msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "Booking Folder"
 msgstr ""
 
@@ -81,50 +85,58 @@
 
 #. Default: "Change date/time"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "Change date/time"
 msgstr ""
 
 #. Default: "Complete address"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:392
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:416
 msgid "Complete address"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:170
 msgid "Configure element"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:385
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:409
 msgid "Contact PEC"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:379
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:403
 msgid "Contact fax"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:373
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:397
 msgid "Contact phone"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:31
 msgid "Content listing"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:181
+#. Default: "Cosa serve"
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:143
+msgid "Cosa serve"
+msgstr ""
+
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:189
 msgid "Data fine validità"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:178
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:186
 msgid "Data inizio validità"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:308
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:330
 msgid "Days booking is not allowed before"
 msgstr ""
 
+msgid "Delete"
+msgstr ""
+
 #. Default: "Descrizione Agenda"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:137
 msgid "Descrizione Agenda"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:125
 msgid "Duration value"
@@ -136,142 +148,148 @@
 msgid "Edit"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:185
 msgid "Edit moved booking Mail Action"
 msgstr ""
 
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:144
+msgid "Elencare le informazioni utili per il giorno della prenotazione, come ad esempio i documenti da presentare."
+msgstr ""
+
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:72
 msgid "Email report to prenotazione owner"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazione.py:159
+#: redturtle/prenotazioni/content/prenotazione.py:163
 msgid "Expiration date booking"
 msgstr ""
 
 #. Default: "Campo"
-#: redturtle/prenotazioni/browser/z3c_custom_widget.py:149
+#: redturtle/prenotazioni/browser/z3c_custom_widget.py:150
 msgid "Field"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:99
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:104
 msgid "Friday"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:81
-#: redturtle/prenotazioni/content/prenotazione.py:154
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:80
+#: redturtle/prenotazioni/content/prenotazione.py:158
 msgid "Gate"
 msgstr ""
 
+msgid "Group"
+msgstr ""
+
 #. Default: "How to get here"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:368
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:392
 msgid "How to get here"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:516
+#: redturtle/prenotazioni/content/validators.py:135
 msgid "In the same day there are overlapping intervals"
 msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 msgid "Informations about a single booking"
 msgstr ""
 
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:138
 msgid "Inserire il testo di presentazione dell'agenda corrente"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:357
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:381
 msgid "Insert a list of email addresses that will be notified when new bookings get created."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:369
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:393
 msgid "Insert here indications on how to reach the office"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:393
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:417
 msgid "Insert here the complete office address"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:386
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:410
 msgid "Insert here the contact PEC"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:380
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:404
 msgid "Insert here the contact fax"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:374
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:398
 msgid "Insert here the contact phone"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:275
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:295
 msgid "Insert pause table schema."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:216
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:224
 msgid "Insert week table schema."
 msgstr ""
 
-#: redturtle/prenotazioni/configure.zcml:30
+#: redturtle/prenotazioni/configure.zcml:31
 msgid "Installs the redturtle.prenotazioni add-on."
 msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:32
-msgid "Is not possible to delete your reservation"
-msgstr ""
-
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:35
-msgid "It's not possbile to delete your reservation. The url is broken or it's to late to delete it"
-msgstr ""
-
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:296
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:318
 msgid "Max days in the future"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:42
 msgid "Message"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:95
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:100
 msgid "Monday"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:421
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:438
+#: redturtle/prenotazioni/content/validators.py:207
 msgid "Morning start should not be greater than end."
 msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:111
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:114
 msgid "Move booking"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:194
+msgid "Move down"
+msgstr ""
+
+msgid "Move up"
+msgstr ""
+
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:202
 msgid "No"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:195
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:203
 msgid "No, just for today"
 msgstr ""
 
 #: redturtle/prenotazioni/content/pause.py:41
 msgid "Pause"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:487
+#: redturtle/prenotazioni/content/validators.py:99
 msgid "Pause end should be greater than pause start"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:504
+#: redturtle/prenotazioni/content/validators.py:120
 msgid "Pause should be included in morning slot or afternoon slot"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:274
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:294
 msgid "Pause table"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:278
+#: redturtle/prenotazioni/browser/prenotazione_add.py:261
 msgid "Please provide a booking date"
 msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 msgid "Prenotazione"
 msgstr ""
 
@@ -283,764 +301,806 @@
 msgid "PrenotazioniWeek"
 msgstr ""
 
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
 msgid "PrenotazioniYear"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:107
+#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:106
 msgid "Print"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:274
+#: redturtle/prenotazioni/configure.zcml:56
+msgid "Profile create to add the new default content rule: booking-confirm"
+msgstr ""
+
+#: redturtle/prenotazioni/restapi/services/booking/add.py:34
+msgid "Required input '${field}' is missing."
+msgstr ""
+
+#: redturtle/prenotazioni/browser/prenotazione_add.py:257
 msgid "Required input is missing."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:356
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:380
 msgid "Responsible email"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:100
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:105
 msgid "Saturday"
 msgstr ""
 
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:11
 msgid "Search for"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:94
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:99
 msgid "Select a day"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/configure.zcml:57
 msgid "Send Email to booking owner when a booking is moved"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:32
 msgid "Sender email"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/delete_reservation.py:107
-msgid "Some information to delete your reservation is missing"
-msgstr ""
-
-#: redturtle/prenotazioni/browser/prenotazione_add.py:283
+#: redturtle/prenotazioni/browser/prenotazione_add.py:266
+#: redturtle/prenotazioni/restapi/services/booking/add.py:83
 msgid "Sorry, this slot is not available anymore."
 msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_move.py:166
+#: redturtle/prenotazioni/browser/prenotazione_move.py:164
 msgid "Sorry, this slot is not available or does not fit your booking."
 msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:286
-#: redturtle/prenotazioni/browser/prenotazione_move.py:172
+#: redturtle/prenotazioni/browser/prenotazione_add.py:269
+#: redturtle/prenotazioni/browser/prenotazione_move.py:170
+#: redturtle/prenotazioni/restapi/services/booking/add.py:90
 msgid "Sorry, you can not book this slot for now."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazione.py:155
+#: redturtle/prenotazioni/content/prenotazione.py:159
 msgid "Sportello a cui presentarsi"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:26
 msgid "Subject"
 msgstr ""
 
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:27
 msgid "Subject of the message"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:101
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:106
 msgid "Sunday"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:37
+#: redturtle/prenotazioni/adapters/stringinterp.py:33
 msgid "The booked date."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:51
+#: redturtle/prenotazioni/adapters/stringinterp.py:46
 msgid "The booked end date."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:65
+#: redturtle/prenotazioni/adapters/stringinterp.py:59
 msgid "The booked time."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:103
+#: redturtle/prenotazioni/adapters/stringinterp.py:94
 msgid "The booking code."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:228
+#: redturtle/prenotazioni/adapters/stringinterp.py:200
 msgid "The booking human readable date"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:190
+#: redturtle/prenotazioni/adapters/stringinterp.py:166
 msgid "The booking office contact fax."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:179
+#: redturtle/prenotazioni/adapters/stringinterp.py:156
 msgid "The booking office contact pec address."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:168
+#: redturtle/prenotazioni/adapters/stringinterp.py:146
 msgid "The booking office contact phone."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:129
-msgid "The booking print url with delete token."
-msgstr ""
-
-#: redturtle/prenotazioni/adapters/stringinterp.py:116
+#: redturtle/prenotazioni/adapters/stringinterp.py:106
 msgid "The booking print url."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:79
+#: redturtle/prenotazioni/adapters/stringinterp.py:72
 msgid "The booking time end."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:93
+#: redturtle/prenotazioni/adapters/stringinterp.py:85
 msgid "The booking type."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:256
+#: redturtle/prenotazioni/adapters/stringinterp.py:227
 msgid "The booking url with delete token"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:214
+#: redturtle/prenotazioni/adapters/stringinterp.py:188
 msgid "The complete address information of the office whereuser book a reservation"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:158
+#: redturtle/prenotazioni/adapters/stringinterp.py:137
 msgid "The email address of the user who made the reservation."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:27
+#: redturtle/prenotazioni/adapters/stringinterp.py:24
 msgid "The gate booked."
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:201
+#: redturtle/prenotazioni/adapters/stringinterp.py:176
 msgid "The information to reach the office where user book a reservation"
 msgstr ""
 
-#: redturtle/prenotazioni/adapters/stringinterp.py:148
+#: redturtle/prenotazioni/adapters/stringinterp.py:128
 msgid "The phone number of the user who made the reservation."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:98
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:103
 msgid "Thursday"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:96
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:101
 msgid "Tuesday"
 msgstr ""
 
-#: redturtle/prenotazioni/configure.zcml:39
+#: redturtle/prenotazioni/configure.zcml:40
 msgid "Uninstalls the redturtle.prenotazioni add-on."
 msgstr ""
 
+#: redturtle/prenotazioni/restapi/services/booking/add.py:66
+msgid "Unknown booking type '${booking_type}'."
+msgstr ""
+
+#: redturtle/prenotazioni/configure.zcml:56
+msgid "Used to add new contentrules"
+msgstr ""
+
 #: redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 #: redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
 msgid "View"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:97
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:102
 msgid "Wednesday"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:215
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:223
 msgid "Week table"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:193
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:201
 msgid "Yes"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/delete_reservation.py:85
-msgid "You can't delete your reservation; it's too late"
-msgstr ""
-
-#: redturtle/prenotazioni/browser/delete_reservation.py:72
-msgid "You can't delete your reservation; please contact the office"
-msgstr ""
-
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:483
+#: redturtle/prenotazioni/content/validators.py:91
 msgid "You must set both start and end"
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:418
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:435
+#: redturtle/prenotazioni/content/validators.py:202
 msgid "You should set a start time for afternoon."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:414
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:431
+#: redturtle/prenotazioni/content/validators.py:194
 msgid "You should set a start time for morning."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:416
-msgid "You should set and end time for afternoon."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:433
+#: redturtle/prenotazioni/content/validators.py:198
+msgid "You should set an end time for afternoon."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:412
-msgid "You should set and end time for morning."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:429
+#: redturtle/prenotazioni/content/validators.py:190
+msgid "You should set an end time for morning."
 msgstr ""
 
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:409
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:426
 msgid "You should set at least one booking type."
 msgstr ""
 
-#: redturtle/prenotazioni/browser/delete_reservation.py:94
-msgid "Your reservation has been deleted"
+#: redturtle/prenotazioni/adapters/stringinterp.py:122
+msgid "[DEPRECATED] The booking print url with delete token."
 msgstr ""
 
 #. Default: "Leave empty, and this Booking Folder will never expire"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:182
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:190
 msgid "aData_help"
 msgstr ""
 
 #. Default: "Book"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:256
-#: redturtle/prenotazioni/browser/vacations.py:252
+#: redturtle/prenotazioni/browser/prenotazione_add.py:239
+#: redturtle/prenotazioni/browser/vacations.py:246
 msgid "action_book"
 msgstr ""
 
 #. Default: "Cancel"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:321
-#: redturtle/prenotazioni/browser/prenotazione_move.py:187
-#: redturtle/prenotazioni/browser/vacations.py:277
+#: redturtle/prenotazioni/browser/prenotazione_add.py:300
+#: redturtle/prenotazioni/browser/prenotazione_move.py:185
+#: redturtle/prenotazioni/browser/vacations.py:271
 msgid "action_cancel"
 msgstr ""
 
 #. Default: "Move"
-#: redturtle/prenotazioni/browser/prenotazione_move.py:151
+#: redturtle/prenotazioni/browser/prenotazione_move.py:149
 msgid "action_move"
 msgstr ""
 
 #. Default: "Search"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:234
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:236
 msgid "action_search"
 msgstr ""
 
 #. Default: "End time in the afternoon"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:84
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:87
 msgid "afternoon_end_label"
 msgstr ""
 
 #. Default: "Start time in the afternoon"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:78
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:81
 msgid "afternoon_start_label"
 msgstr ""
 
 #. Default: "Please select a booking slot."
 #: redturtle/prenotazioni/browser/templates/week.pt:28
 msgid "book_it"
 msgstr ""
 
 #. Default: "Bookable time"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:297
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:306
 msgid "bookable_time"
 msgstr ""
 
 #. Default: "${day}, ore ${booking_time}, prenotato da ${booked_by}, prenotazione: ${booking_type} durata: ${duration} minuti"
-#: redturtle/prenotazioni/browser/week.py:257
+#: redturtle/prenotazioni/browser/week.py:276
 msgid "booked_prenotation_message"
 msgstr ""
 
 #. Default: "Booking confirmed"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:299
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:308
 msgid "booking_confirmed"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:303
-#: redturtle/prenotazioni/browser/vacations.py:249
+#: redturtle/prenotazioni/browser/prenotazione_add.py:278
+#: redturtle/prenotazioni/browser/vacations.py:243
 msgid "booking_created"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_move.py:177
+#. Default: "Your booking has been deleted."
+#: redturtle/prenotazioni/browser/delete_reservation.py:112
+msgid "booking_deleted_success"
+msgstr ""
+
+#: redturtle/prenotazioni/browser/prenotazione_move.py:175
 msgid "booking_moved"
 msgstr ""
 
 #. Default: "Booking pending"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:301
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:310
 msgid "booking_pending"
 msgstr ""
 
 #. Default: "Booking refused"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:303
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:312
 msgid "booking_refused"
 msgstr ""
 
 #. Default: "Name"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:272
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:281
 msgid "booking_type_name"
 msgstr ""
 
 #. Default: "Value"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:273
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:282
 msgid "booking_type_value"
 msgstr ""
 
 #. Default: "You may want to select another time slot to book one of these."
 #: redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt:55
 msgid "booking_type_widget_suggest_reselect"
 msgstr ""
 
 #. Default: "The following tipologies will not fit the time you selected:"
 #: redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt:45
 msgid "booking_type_widget_warn_unavailable"
 msgstr ""
 
 #. Default: "Put booking types there (one per line).\nIf you do not provide this field, not type selection will be available"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:319
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:341
 msgid "booking_types_help"
 msgstr ""
 
 #. Default: "Booking types"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:318
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:340
 msgid "booking_types_label"
 msgstr ""
 
 #. Default: "Bookings not in agenda"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:63
 msgid "bookings_not_in_agenda"
 msgstr ""
 
 #. Default: "Busy"
-#: redturtle/prenotazioni/browser/prenotazioni_context_state.py:76
+#: redturtle/prenotazioni/browser/prenotazioni_context_state.py:81
 msgid "busy"
 msgstr ""
 
 #. Default: "Your booking has to be confirmed by the administrators"
 #: redturtle/prenotazioni/browser/prenotazione_print.py:19
 msgid "confirm_booking_waiting_message"
 msgstr ""
 
 #. Default: "Show here contacts information that will be used by authomatic mail system"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:399
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:455
 msgid "contacts_help"
 msgstr ""
 
 #. Default: "Contacts"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:398
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:454
 msgid "contacts_label"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:23
-msgid "damn"
+#. Default: "Cosa serve"
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:96
+msgid "cosa_serve"
 msgstr ""
 
 #. Default: "This day is not valid."
-#: redturtle/prenotazioni/browser/vacations.py:269
+#: redturtle/prenotazioni/browser/vacations.py:263
 msgid "day_error"
 msgstr ""
 
 #. Default: "Day of week"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:64
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:67
 msgid "day_label"
 msgstr ""
 
-#. Default: "Delete reservation request for: ${name}"
-#: redturtle/prenotazioni/browser/delete_reservation.py:20
-msgid "delete_reservation_request"
+#. Default: "You can't delete your reservation; it's too late."
+#: redturtle/prenotazioni/browser/delete_reservation.py:137
+msgid "delete_expired_booking"
 msgstr ""
 
-#. Default: "Your reservation has been deleted"
-#: redturtle/prenotazioni/browser/delete_reservation.py:41
-msgid "deleted_reservation"
+#. Default: "Delete reservation request for: ${name}"
+#: redturtle/prenotazioni/browser/delete_reservation.py:59
+msgid "delete_reservation_request"
 msgstr ""
 
 #. Default: "If you work for a company, please specify its name."
-#: redturtle/prenotazioni/content/prenotazione.py:146
+#: redturtle/prenotazioni/content/prenotazione.py:149
 msgid "description_company"
 msgstr ""
 
 #. Default: "The gate that will be unavailable"
-#: redturtle/prenotazioni/browser/vacations.py:66
+#: redturtle/prenotazioni/browser/vacations.py:67
 msgid "description_gate"
 msgstr ""
 
 #. Default: "This text will appear in the calendar cells"
-#: redturtle/prenotazioni/browser/vacations.py:59
+#: redturtle/prenotazioni/browser/vacations.py:60
 msgid "description_title"
 msgstr ""
 
 #. Default: "Foreseen booking time: ${booking_time}"
-#: redturtle/prenotazioni/browser/week.py:206
+#: redturtle/prenotazioni/browser/week.py:225
 msgid "foreseen_booking_time"
 msgstr ""
 
 #. Default: "${booking_time}, Orario non disponibile"
-#: redturtle/prenotazioni/browser/week.py:225
+#: redturtle/prenotazioni/browser/week.py:244
 msgid "foreseen_busy_time"
 msgstr ""
 
+msgid "from_label"
+msgstr ""
+
+#. Default: "You should set a start range."
+#: redturtle/prenotazioni/content/validators.py:159
+msgid "from_month_error"
+msgstr ""
+
+#. Default: "Selected day is too big for that month for \"from\" field."
+#: redturtle/prenotazioni/content/validators.py:166
+msgid "from_month_too_days_error"
+msgstr ""
+
 #. Default: "Fullname"
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:40
 msgid "fullname"
 msgstr ""
 
 #. Default: "Limit booking in the future to an amount of days in the future starting from the current day. \nKeep 0 to give no limits."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:297
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:319
 msgid "futureDays"
 msgstr ""
 
 #. Default: "Put gates here (one per line)."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:331
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:355
 msgid "gates_help"
 msgstr ""
 
 #. Default: "Gates"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:330
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:354
 msgid "gates_label"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/prenotazione_add.py:165
+#: redturtle/prenotazioni/browser/prenotazione_add.py:162
 msgid "help_prenotazione_add"
 msgstr ""
 
 #. Default: "User will not be able to add a booking unless those fields are filled. Remember that, whatever you selected in this list, users have to supply at least one of \"Email\", \"Mobile\", or \"Telephone\""
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:144
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:152
 msgid "help_required_booking_fields"
 msgstr ""
 
 #. Default: "States if it is not allowed to reserve a booking during the current day"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:205
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:213
 msgid "help_same_day_booking_disallowed"
 msgstr ""
 
 #. Default: "List of available reservation type for the current agenda"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:269
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:278
 msgid "help_tipologies"
 msgstr ""
 
 #. Default: "User will not be able to add a booking unless those fields are filled. Remember that, whatever you selected in this list, users have to supply at least one of \"Email\" or \"Telephone\""
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:162
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:170
 msgid "help_visible_booking_fields"
 msgstr ""
 
 #. Default: "Set holidays (one for line) in DD/MM/YYYY. you can write * for the year, if this event is yearly."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:283
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:305
 msgid "holidays_help"
 msgstr ""
 
 #. Default: "Holidays"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:282
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:304
 msgid "holidays_label"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/vacations.py:30
+#: redturtle/prenotazioni/browser/vacations.py:31
 msgid "invalid_date"
 msgstr ""
 
 #. Default: "Invalid email address"
-#: redturtle/prenotazioni/content/prenotazione.py:26
+#: redturtle/prenotazioni/content/prenotazione.py:28
 msgid "invalid_email_address"
 msgstr ""
 
 #. Default: "Invalid start or end date"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:31
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:20
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:33
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:25
 msgid "invalid_end:search_date"
 msgstr ""
 
 #. Default: "Invalid fiscal code"
-#: redturtle/prenotazioni/content/prenotazione.py:34
+#: redturtle/prenotazioni/content/prenotazione.py:36
 msgid "invalid_fiscalcode"
 msgstr ""
 
 #. Default: "Invalid phone number"
-#: redturtle/prenotazioni/content/prenotazione.py:22
+#: redturtle/prenotazioni/content/prenotazione.py:24
 msgid "invalid_phone_number"
 msgstr ""
 
-#: redturtle/prenotazioni/browser/vacations.py:34
+#: redturtle/prenotazioni/browser/vacations.py:35
 msgid "invalid_time"
 msgstr ""
 
 #. Default: "This date is past"
-#: redturtle/prenotazioni/content/prenotazione.py:30
+#: redturtle/prenotazioni/content/prenotazione.py:32
 msgid "is_not_future_date"
 msgstr ""
 
 #. Default: "Booking code"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:115
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:93
-#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:93
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:89
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:92
+#: redturtle/prenotazioni/browser/templates/prenotazione_print.pt:92
 msgid "label_booking_code"
 msgstr ""
 
 #. Default: "Company"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:77
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:52
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:36
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:57
 msgid "label_booking_company"
 msgstr ""
 
 #. Default: "Booking date"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:95
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:70
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:48
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:69
 msgid "label_booking_date"
 msgstr ""
 
-#. Default: "${from_date} from ${from} to ${to}"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:103
-#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:52
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:76
+#. Default: "${from_date} at ${at}"
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:77
+#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:51
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:75
 msgid "label_booking_date_range"
 msgstr ""
 
 #. Default: "Subject"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:53
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:89
+#: redturtle/prenotazioni/browser/prenotazione_add.py:49
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:64
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:44
 msgid "label_booking_description"
 msgstr ""
 
 #. Default: "Email"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:65
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:40
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:28
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:48
 msgid "label_booking_email"
 msgstr ""
 
 #. Default: "Fiscal code"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:83
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:58
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:40
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:61
 msgid "label_booking_fiscalcode"
 msgstr ""
 
 #. Default: "Phone number"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:71
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:46
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:32
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:53
 msgid "label_booking_phone"
 msgstr ""
 
 #. Default: "Staff notes"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:85
-#: redturtle/prenotazioni/content/prenotazione.py:163
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:84
+#: redturtle/prenotazioni/content/prenotazione.py:167
 msgid "label_booking_staff_notes"
 msgstr ""
 
 #. Default: "Booking time"
-#: redturtle/prenotazioni/browser/prenotazione_move.py:32
-#: redturtle/prenotazioni/content/prenotazione.py:111
+#: redturtle/prenotazioni/browser/prenotazione_move.py:31
+#: redturtle/prenotazioni/content/prenotazione.py:114
 msgid "label_booking_time"
 msgstr ""
 
 #. Default: "Fullname"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:50
+#: redturtle/prenotazioni/browser/prenotazione_add.py:46
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:20
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:35
 msgid "label_booking_title"
 msgstr ""
 
 #. Default: "Booking type"
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:59
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:34
 #: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:24
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:44
 msgid "label_booking_type"
 msgstr ""
 
-#: redturtle/prenotazioni/vocabularies/requirable_booking_fields.py:22
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:262
+#: redturtle/prenotazioni/vocabularies/requirable_booking_fields.py:23
 msgid "label_booking_{}"
 msgstr ""
 
 #. Default: "End date"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:59
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:46
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:61
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:51
 msgid "label_end"
 msgstr ""
 
 #. Default: "End time"
-#: redturtle/prenotazioni/browser/vacations.py:82
+#: redturtle/prenotazioni/browser/vacations.py:83
 msgid "label_end_time"
 msgstr ""
 
 #. Default: "Gate"
-#: redturtle/prenotazioni/browser/prenotazione_move.py:34
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:47
-#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:109
+#: redturtle/prenotazioni/browser/prenotazione_move.py:32
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:49
+#: redturtle/prenotazioni/browser/templates/delete_reservation.pt:83
 msgid "label_gate"
 msgstr ""
 
 #. Default: "Go to the booking to see more details and manage it: ${url}"
-#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:62
+#: redturtle/prenotazioni/browser/templates/manager_notification_mail.pt:61
 msgid "label_new_booking_notify_link"
 msgstr ""
 
 #. Default: "Required booking fields"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:143
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:151
 msgid "label_required_booking_fields"
 msgstr ""
 
 #. Default: "Disallow same day booking"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:201
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:209
 msgid "label_same_day_booking_disallowed"
 msgstr ""
 
 #. Default: "Selected date: ${date} — Time: ${slot}"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:153
+#: redturtle/prenotazioni/browser/prenotazione_add.py:147
 msgid "label_selected_date"
 msgstr ""
 
 #. Default: "Start date "
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:53
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:39
-#: redturtle/prenotazioni/browser/vacations.py:71
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:55
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:44
+#: redturtle/prenotazioni/browser/vacations.py:72
 msgid "label_start"
 msgstr ""
 
 #. Default: "Start time"
-#: redturtle/prenotazioni/browser/vacations.py:76
+#: redturtle/prenotazioni/browser/vacations.py:77
 msgid "label_start_time"
 msgstr ""
 
 #. Default: "Text to search"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:39
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:41
 msgid "label_text"
 msgstr ""
 
 #. Default: "Reservation types"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:268
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:277
 msgid "label_tipologies"
 msgstr ""
 
 #. Default: "Title"
-#: redturtle/prenotazioni/browser/vacations.py:58
+#: redturtle/prenotazioni/browser/vacations.py:59
 msgid "label_title"
 msgstr ""
 
 #. Default: "User"
-#: redturtle/prenotazioni/browser/stats/booking_stats.py:37
+#: redturtle/prenotazioni/browser/stats/booking_stats.py:42
 msgid "label_user"
 msgstr ""
 
 #. Default: "Visible booking fields"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:161
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:169
 msgid "label_visible_booking_fields"
 msgstr ""
 
 #. Default: "Legend"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:290
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:299
 msgid "legend"
 msgstr ""
 
 #. Default: "Short description of available action for the booking board"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:291
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:300
 msgid "legend_description"
 msgstr ""
 
 #. Default: "The minimum value of a single slot is 5 minutes. You cannot book a reservation when the needed time exceeds the available time."
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:312
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:321
 msgid "legend_note"
 msgstr ""
 
 #. Default: "Type in here the message that you want to mail. Some defined content can be replaced: ${title} will be replaced with booking title (user fullname). ${date} will be replaced with booking new date. ${url} will be replaced by the booking url. ${portal} will be replaced by the title of the portal."
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:43
 msgid "message_help"
 msgstr ""
 
+#. Default: "Unable to find a booking with the givend id: ${uid}."
+#: redturtle/prenotazioni/browser/delete_reservation.py:42
+msgid "missing_booking"
+msgstr ""
+
+#. Default: "You need to provide a reservation id."
+#: redturtle/prenotazioni/browser/delete_reservation.py:36
+msgid "missing_uid"
+msgstr ""
+
+msgid "month_label"
+msgstr ""
+
 #. Default: "End time in the morning"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:72
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:75
 msgid "morning_end_label"
 msgstr ""
 
 #. Default: "Start time in the morning"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:67
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:70
 msgid "morning_start_label"
 msgstr ""
 
 #. Default: "Go back to the calendar"
-#: redturtle/prenotazioni/browser/prenotazioni_search.py:244
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:138
+#: redturtle/prenotazioni/browser/prenotazioni_search.py:246
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:141
 #: redturtle/prenotazioni/browser/templates/prenotazione_add.pt:88
 msgid "move_back_message"
 msgstr ""
 
 #. Default: "Move booking"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:118
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:121
 msgid "move_booking"
 msgstr ""
 
 #. Default: "Please move this booking into a new available slot or"
 #: redturtle/prenotazioni/browser/templates/prenotazione_move.pt:34
 msgid "move_message"
 msgstr ""
 
 #. Default: "New booking for ${context}"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:409
+#: redturtle/prenotazioni/browser/prenotazione_add.py:388
 msgid "new_booking_admin_notify_subject"
 msgstr ""
 
 #. Default: "next week"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:22
 msgid "next-week"
 msgstr ""
 
-#. Default: "Seems your reservation is not existing"
-#: redturtle/prenotazioni/browser/delete_reservation.py:31
-msgid "no_reservation"
-msgstr ""
-
 #. Default: "Booking is not allowed before the amount of days specified. \nKeep 0 to give no limits."
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:309
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:331
 msgid "notBeforeDays"
 msgstr ""
 
 #. Default: "Pause end"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:116
 msgid "pause_end_label"
 msgstr ""
 
 #. Default: "Pause start"
 #: redturtle/prenotazioni/content/prenotazioni_folder.py:111
 msgid "pause_start_label"
 msgstr ""
 
 #. Default: "Please select a time slot"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:349
+#: redturtle/prenotazioni/browser/prenotazione_add.py:328
 msgid "please_pick_a_date"
 msgstr ""
 
 #. Default: "${day}, ore ${booking_time}"
-#: redturtle/prenotazioni/browser/week.py:237
+#: redturtle/prenotazioni/browser/week.py:256
 msgid "prenotation_slot_message"
 msgstr ""
 
 #. Default: "prenotazioni_search"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "prenotazioni_search"
 msgstr ""
 
 #. Default: "previous week"
 #: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:7
 msgid "previous-week"
 msgstr ""
 
-#: redturtle/prenotazioni/configure.zcml:30
+#: redturtle/prenotazioni/configure.zcml:31
 msgid "redturtle.prenotazioni"
 msgstr ""
 
-#: redturtle/prenotazioni/configure.zcml:39
+#: redturtle/prenotazioni/configure.zcml:48
+msgid "redturtle.prenotazioni (to_1500)"
+msgstr ""
+
+#: redturtle/prenotazioni/configure.zcml:40
 msgid "redturtle.prenotazioni (uninstall)"
 msgstr ""
 
+#: redturtle/prenotazioni/configure.zcml:48
+msgid "redturtle.prenotazioni to 1500."
+msgstr ""
+
 #. Default: "The booking state is \"refused\". If you change it, the booking time may conflict with another one."
 #: redturtle/prenotazioni/browser/templates/prenotazione.pt:23
 msgid "refused-review-state-warning"
 msgstr ""
 
 #. Default: "Reject booking"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:128
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:131
 msgid "reject_booking"
 msgstr ""
 
 #. Default: "Reminders"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:436
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:464
 msgid "reminders_label"
 msgstr ""
 
 #. Default: "Code"
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:41
 msgid "reservation_code"
 msgstr ""
@@ -1062,61 +1122,89 @@
 
 #. Default: "items matching your search terms."
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:19
 msgid "result_number"
 msgstr ""
 
 #. Default: "Search by gate"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:308
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:317
 msgid "search-by-gate"
 msgstr ""
 
 #. Default: "Search result"
 #: redturtle/prenotazioni/browser/templates/prenotazioni_search.pt:9
 msgid "search_result_message"
 msgstr ""
 
 #. Default: "seleziona l'opzione desiderata dal gruppo di radio button seguente"
-#: redturtle/prenotazioni/browser/z3c_custom_widget.py:152
+#: redturtle/prenotazioni/browser/z3c_custom_widget.py:153
 msgid "select-option"
 msgstr ""
 
 #. Default: "This gate has some booking schedule in this time period."
-#: redturtle/prenotazioni/browser/vacations.py:262
+#: redturtle/prenotazioni/browser/vacations.py:256
 msgid "slot_conflict_error"
 msgstr ""
 
 #. Default: "The email address that sends the email. If no email is provided here, it will use the address from portal."
 #: redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py:33
 msgid "source_help"
 msgstr ""
 
 #. Default: "You cannot book any booking_type at this time"
-#: redturtle/prenotazioni/browser/prenotazione_add.py:353
+#: redturtle/prenotazioni/browser/prenotazione_add.py:332
 msgid "time_slot_to_short"
 msgstr ""
 
+msgid "to_label"
+msgstr ""
+
+#. Default: "You should set an end range."
+#: redturtle/prenotazioni/content/validators.py:174
+msgid "to_month_error"
+msgstr ""
+
+#. Default: "Selected day is too big for that month for \"to\" field."
+#: redturtle/prenotazioni/content/validators.py:181
+msgid "to_month_too_days_error"
+msgstr ""
+
 #. Default: "Add a gate here (one per line) if, for some reason, it is not be available.The specified gate will not be taken in to account for slot allocation. Each line should match a corresponding line in the \"Gates\" field"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:339
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:363
 msgid "unavailable_gates_help"
 msgstr ""
 
 #. Default: "Unavailable gates"
-#: redturtle/prenotazioni/content/prenotazioni_folder.py:338
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:362
 msgid "unavailable_gates_label"
 msgstr ""
 
 #. Default: "Unbookable time"
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:295
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:304
 msgid "unbookable_time"
 msgstr ""
 
 #. Default: "vacation_booking"
 #: redturtle/prenotazioni/profiles/default/actions.xml
 msgid "vacation_booking"
 msgstr ""
 
 #. Default: "View booking"
-#: redturtle/prenotazioni/browser/templates/prenotazione.pt:105
-#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:306
+#: redturtle/prenotazioni/browser/templates/prenotazione.pt:108
+#: redturtle/prenotazioni/browser/templates/prenotazione_macros.pt:315
 msgid "view_booking"
 msgstr ""
+
+#. Default: "Insert here week schema for some custom date intervals."
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:285
+msgid "week_table_overrides_help"
+msgstr ""
+
+#. Default: "Week table overrides"
+#: redturtle/prenotazioni/content/prenotazioni_folder.py:284
+msgid "week_table_overrides_label"
+msgstr ""
+
+#. Default: "You tried to delete booking with a wrong action."
+#: redturtle/prenotazioni/browser/delete_reservation.py:95
+msgid "wrong_authenticator"
+msgstr ""
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/locales/update.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/locales/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             )
             subprocess.call(cmd, shell=True)
 
     os.chdir("../../../../")
 
 
 def _rebuild():
-    cmd = "{i18ndude} rebuild-pot --pot {locale_path}/{domain}.pot --exclude {excludes} --create {domain} {target_path}".format(  # NOQA: E501
+    cmd = "{i18ndude} rebuild-pot --pot {locale_path}/{domain}.pot --exclude {excludes} --create {domain} --merge {locale_path}/manual.pot {target_path}".format(  # NOQA: E501
         i18ndude=i18ndude,
         locale_path=locale_path,
         domain=domain,
         target_path=target_path,
         excludes=excludes,
     )
     subprocess.call(cmd, shell=True)
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/permissions.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/permissions.zcml`

 * *Files 3% similar despite different names*

```diff
@@ -37,10 +37,16 @@
         />
 
     <permission
         id="redturtle.prenotazioni.SearchPrenotazioni"
         title="redturtle.prenotazioni: search prenotazioni"
         />
 
+    <permission
+        id="redturtle.prenotazioni.ManagePrenotazioni"
+        title="redturtle.prenotazioni: Manage Prenotazioni"
+        />
+
+
   </configure>
 
 </configure>
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/actions.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/contentrules.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/contentrules.xml`

 * *Files 10% similar despite different names*

#### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/contentrules.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/contentrules.xml`

```diff
@@ -15,15 +15,15 @@
     </conditions>
     <actions>
       <action type="plone.actions.MailFromField">
         <property name="source"/>
         <property name="message">La prenotazione per ${title} è stata accettata. Il codice di prenotazione è ${booking_code}</property>
         <property name="message">La prenotazione per ${title} e' stata accettata.
 
-Se desideri visualizzare, stampare o cancellare questa prenotazione puoi utilizzare il seguente link: ${booking_print_url_with_delete_token}</property>
+Se desideri visualizzare, stampare o cancellare questa prenotazione puoi utilizzare il seguente link: ${booking_print_url}</property>
         <property name="fieldName">email</property>
         <property name="target">target</property>
         <property name="subject">Prenotazione del ${booking_date} alle ${booking_time} accettata</property>
       </action>
     </actions>
   </rule>
   <rule name="booking-moved" title="Invia un'email all'utente quando la data della prenotazione viene cambiata" description="Viene inviata una mail al richiedente per avvertire dello spostamento della prenotazione" enabled="True" event="redturtle.prenotazioni.prenotazione_event.IMovedPrenotazione" stop-after="False">
@@ -94,8 +94,36 @@
         <property name="message">La prenotazione del ${booking_date} delle ore ${booking_time} è stata rifiutata.</property>
         <property name="fieldName">email</property>
         <property name="target">target</property>
         <property name="subject">Prenotazione rifiutata per ${title}</property>
       </action>
     </actions>
   </rule>
+  <rule name="booking-confirm" title="Conferma automatica prenotazioni" cascading="False" description="Conferma automatica degli appuntamenti" enabled="True" event="Products.CMFCore.interfaces.IActionSucceededEvent" stop-after="False">
+    <conditions>
+      <condition type="plone.conditions.WorkflowState">
+        <property name="wf_states">
+          <element>pending</element>
+        </property>
+      </condition>
+      <condition type="plone.conditions.PortalType">
+        <property name="check_types">
+          <element>Prenotazione</element>
+        </property>
+      </condition>
+    </conditions>
+    <actions>
+      <action type="plone.actions.Mail">
+        <property name="subject">Prenotazione del ${booking_date} alle ${booking_time} accettata</property>
+        <property name="source"/>
+        <property name="recipients">${booking_user_email}</property>
+        <property name="exclude_actor">False</property>
+        <property name="message">La prenotazione per ${title} e' stata confermata!
+     Se non hai salvato o stampato il promemoria, puoi visualizzarlo a questo link: ${booking_print_url}
+     Se desideri cancellare la prenotazione, accedi all'indirizzo ${booking_print_url}</property>
+      </action>
+      <action type="plone.actions.Workflow">
+        <property name="transition">confirm</property>
+      </action>
+    </actions>
+  </rule>
 </contentrules>
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/registry/caching.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/caching.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/registry/settings.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/registry/settings.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

 * *Files 21% similar despite different names*

#### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/rolemap.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/rolemap.xml`

```diff
@@ -1,11 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <rolemap>
   <permissions>
-    <!-- -*- extra stuff goes here -*- -->
     <permission name="redturtle.prenotazioni: Add Prenotazione" acquire="True">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
     <permission name="redturtle.prenotazioni: Add PrenotazioniDay" acquire="True">
@@ -29,11 +28,17 @@
     <permission name="redturtle.prenotazioni: Add PrenotazioniFolder" acquire="True">
       <role name="Manager"/>
       <role name="Site Administrator"/>
       <role name="Owner"/>
       <role name="Contributor"/>
     </permission>
     <permission name="redturtle.prenotazioni: search prenotazioni" acquire="True">
-      <role name="Reader"/>
+      <role name="Manager"/>
+      <role name="Site Administrator"/>
+      <role name="Contributor"/>
+    </permission>
+    <permission name="redturtle.prenotazioni: Manage Prenotazioni" acquire="True">
+      <role name="Manager"/>
+      <role name="Site Administrator"/>
     </permission>
   </permissions>
 </rolemap>
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml`

 * *Files 5% similar despite different names*

#### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml`

```diff
@@ -27,15 +27,14 @@
   <property name="behaviors" purge="false">
     <element value="plone.app.content.interfaces.INameFromTitle"/>
     <element value="plone.app.dexterity.behaviors.discussion.IAllowDiscussion"/>
     <element value="plone.app.dexterity.behaviors.exclfromnav.IExcludeFromNavigation"/>
     <element value="plone.app.dexterity.behaviors.id.IShortName"/>
     <element value="plone.app.dexterity.behaviors.metadata.IBasic"/>
     <element value="plone.app.lockingbehavior.behaviors.ILocking"/>
-    <element value="collective.dexteritytextindexer.behavior.IDexterityTextIndexer"/>
   </property>
   <!-- View information -->
   <property name="add_view_expr">string:${folder_url}/++add++PrenotazioniFolder</property>
   <property name="default_view">prenotazioni_week_view</property>
   <property name="default_view_fallback">False</property>
   <property name="immediate_view">view</property>
   <property name="view_methods">
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types.xml`

 * *Files 20% similar despite different names*

#### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/types.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/types.xml`

```diff
@@ -3,9 +3,8 @@
   <property name="title">Controls the available contenttypes in your portal</property>
   <!--<object name="example_ct" meta_type="Dexterity FTI"/>-->
   <object meta_type="Dexterity FTI" name="PrenotazioniFolder"/>
   <object meta_type="Dexterity FTI" name="PrenotazioniYear"/>
   <object meta_type="Dexterity FTI" name="PrenotazioniWeek"/>
   <object meta_type="Dexterity FTI" name="PrenotazioniDay"/>
   <object meta_type="Dexterity FTI" name="Prenotazione"/>
-  <object meta_type="Dexterity FTI" name="PrenotazioniFolderContainer"/>
 </object>
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/profiles/default/workflows.xml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# -*- coding: utf-8 -*-
+
 from plone.restapi.interfaces import ISerializeToJson
 from redturtle.prenotazioni.adapters.slot import ISlot
 from zope.component import adapter
 from zope.interface import implementer
 from zope.publisher.interfaces import IRequest
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/restapi/services/week_slots/get.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/restapi/services/week_slots/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# -*- coding: utf-8 -*-
+
 from plone import api
 from plone.restapi.interfaces import ISerializeToJson
 from plone.restapi.services import Service
 from zope.component import getMultiAdapter
 
 
 class WeekSlots(Service):
@@ -65,8 +67,11 @@
 
             for name, value in busy_slots.items():
                 response[week_day_key]["busy_slots"][name] = [
                     getMultiAdapter((item, self.request), ISerializeToJson)()
                     for item in value
                 ]
 
-        return response
+        return {
+            "@id": "{}/@week-slots".format(self.contenxt.abosolute_url()),
+            "items": response,
+        }
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/app_io.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/app_io.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/README.md` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/api.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/api.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/cli.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/cli.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/io.db` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/io.db`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/monkey.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/rdbms.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/spec.yaml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/scripts/io_tools/storage.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/scripts/io_tools/storage.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/testing.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/testing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 # -*- coding: utf-8 -*-
 from plone.app.contenttypes.testing import PLONE_APP_CONTENTTYPES_FIXTURE
 from plone.app.testing import applyProfile
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
 from plone.app.testing import PloneSandboxLayer
+from plone.restapi.testing import PloneRestApiDXLayer
+from plone.testing import z2
 
 import collective.contentrules.mailfromfield
 import collective.z3cform.datagridfield
 import plone.app.caching
 import plone.restapi
 import redturtle.prenotazioni
 
+try:
+    import collective.dexteritytextindexer
+
+    HAS_DX_TEXTINDEXER = True
+except ImportError:
+    HAS_DX_TEXTINDEXER = False
+
 
 class RedturtlePrenotazioniLayer(PloneSandboxLayer):
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         # Load any other ZCML that is required for your tests.
         # The z3c.autoinclude feature is disabled in the Plone fixture base
         # layer.
         self.loadZCML(package=plone.app.caching)
         self.loadZCML(package=plone.restapi)
         self.loadZCML(package=redturtle.prenotazioni)
         self.loadZCML(package=collective.contentrules.mailfromfield)
         self.loadZCML(package=collective.z3cform.datagridfield)
 
+        if HAS_DX_TEXTINDEXER:
+            self.loadZCML(package=collective.dexteritytextindexer)
+
     def setUpPloneSite(self, portal):
         applyProfile(portal, "plone.app.caching:default")
         applyProfile(portal, "redturtle.prenotazioni:default")
 
 
 REDTURTLE_PRENOTAZIONI_FIXTURE = RedturtlePrenotazioniLayer()
 
@@ -39,7 +51,41 @@
 )
 
 
 REDTURTLE_PRENOTAZIONI_FUNCTIONAL_TESTING = FunctionalTesting(
     bases=(REDTURTLE_PRENOTAZIONI_FIXTURE,),
     name="RedturtlePrenotazioniLayer:FunctionalTesting",
 )
+
+
+class RedturtlePrenotazioniRestApiLayer(PloneRestApiDXLayer):
+    defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
+
+    def setUpZope(self, app, configurationContext):
+        super(RedturtlePrenotazioniRestApiLayer, self).setUpZope(
+            app, configurationContext
+        )
+
+        self.loadZCML(package=plone.app.caching)
+        self.loadZCML(package=plone.restapi)
+        self.loadZCML(package=redturtle.prenotazioni)
+        self.loadZCML(package=collective.contentrules.mailfromfield)
+        self.loadZCML(package=collective.z3cform.datagridfield)
+
+        if HAS_DX_TEXTINDEXER:
+            self.loadZCML(package=collective.dexteritytextindexer)
+
+    def setUpPloneSite(self, portal):
+        applyProfile(portal, "plone.app.caching:default")
+        applyProfile(portal, "redturtle.prenotazioni:default")
+
+
+REDTURTLE_PRENOTAZIONI_API_FIXTURE = RedturtlePrenotazioniRestApiLayer()
+REDTURTLE_PRENOTAZIONI_API_INTEGRATION_TESTING = IntegrationTesting(
+    bases=(REDTURTLE_PRENOTAZIONI_API_FIXTURE,),
+    name="RedturtlePrenotazioniRestApiLayer:Integration",
+)
+
+REDTURTLE_PRENOTAZIONI_API_FUNCTIONAL_TESTING = FunctionalTesting(
+    bases=(REDTURTLE_PRENOTAZIONI_API_FIXTURE, z2.ZSERVER_FIXTURE),
+    name="RedturtlePrenotazioniRestApiLayer:Functional",
+)
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/tests/test_setup.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/tests/test_setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -40,14 +40,23 @@
     def test_browserlayer(self):
         """Test that IRedturtlePrenotazioniLayer is registered."""
         from plone.browserlayer import utils
         from redturtle.prenotazioni.interfaces import IRedturtlePrenotazioniLayer
 
         self.assertIn(IRedturtlePrenotazioniLayer, utils.registered_layers())
 
+    def test_dexteritytextindexer_behavior_enabled_only_in_plone_less_than_6(self):
+        plone_version = api.env.plone_version()
+        portal_types = api.portal.get_tool(name="portal_types")
+        behaviors = portal_types["PrenotazioniFolder"].behaviors
+        if plone_version < "6":
+            self.assertIn("collective.dexteritytextindexer", behaviors)
+        else:
+            self.assertNotIn("collective.dexteritytextindexer", behaviors)
+
 
 class TestUninstall(unittest.TestCase):
     layer = REDTURTLE_PRENOTAZIONI_INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         if get_installer:
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/upgrades.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/upgrades.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_PROFILE = "profile-redturtle.prenotazioni:default"
+CONTENT_RULES_EVOLUTION_PROFILE = (
+    "profile-redturtle.prenotazioni:content_rules_evolution"
+)
 
 
 def update_profile(context, profile):
     context.runImportStepFromProfile(DEFAULT_PROFILE, profile)
 
 
 def update_registry(context):
@@ -111,39 +114,45 @@
         "refused": "refused",
         # handle case of the upgrade step double run
         "confirmed": "confirmed",
     }
 
     # if we find the exception the code must fail
     remap_workflow(
-        context, ("Prenotazione",), ("prenotazioni_workflow",), workflow_state_map
+        context,
+        ("Prenotazione",),
+        ("prenotazioni_workflow",),
+        workflow_state_map,
     )
 
     rule_storage = queryUtility(IRuleStorage)
 
     for rule in rule_storage.items():
         rule = rule[1]
 
         portal_type_conditions = filter(
             lambda item: isinstance(item, PortalTypeCondition), rule.conditions
         )
 
         workflow_state_conditions = filter(
-            lambda item: isinstance(item, WorkflowStateCondition), rule.conditions
+            lambda item: isinstance(item, WorkflowStateCondition),
+            rule.conditions,
         )
 
         workflow_transition_conditions = filter(
-            lambda item: isinstance(item, WorkflowTransitionCondition), rule.conditions
+            lambda item: isinstance(item, WorkflowTransitionCondition),
+            rule.conditions,
         )
 
         for portal_type_condition in portal_type_conditions:
             if "Prenotazione" in getattr(portal_type_condition, "check_types", []):
                 for workflow_transition_condition in workflow_transition_conditions:
                     if isinstance(
-                        workflow_transition_condition, WorkflowTransitionCondition
+                        workflow_transition_condition,
+                        WorkflowTransitionCondition,
                     ):
                         wf_states = list(workflow_transition_condition.wf_transitions)
 
                         if "publish" in wf_states:
                             wf_states.remove("publish")
                             wf_states.append("confirm")
 
@@ -180,7 +189,25 @@
             condition
             for condition in portal_type_conditions
             if "Prenotazione" in getattr(condition, "check_types", [])
         ]:
             for workflow_action in workflow_action_conditions:
                 if workflow_action.transition == "publish":
                     workflow_action.transition = "confirm"
+
+
+def to_1402(context):
+    # load new content rules
+    context.runImportStepFromProfile(CONTENT_RULES_EVOLUTION_PROFILE, "contentrules")
+
+
+def to_1403(context):
+    update_catalog(context)
+
+    for brain in api.portal.get_tool("portal_catalog")(portal_type="Prenotazione"):
+        brain.getObject().reindexObject(idxs=["fiscalcode"])
+
+
+def to_1500(context):
+    context.runImportStepFromProfile(
+        "profile-redturtle.prenotazioni:to_1500", "typeinfo"
+    )
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/upgrades.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/upgrades.zcml`

 * *Files 17% similar despite different names*

```diff
@@ -57,8 +57,45 @@
       title="Upgrade to 1401"
       description="Upgrade prenotazioni_workflow + add type"
       profile="redturtle.prenotazioni:default"
       source="1400"
       destination="1401"
       handler=".upgrades.to_1401"
       />
+
+  <genericsetup:upgradeStep
+      title="Upgrade to 1402"
+      description="Load new content rule: booking-confirm"
+      profile="redturtle.prenotazioni:default"
+      source="1401"
+      destination="1402"
+      handler=".upgrades.to_1402"
+      />
+
+  <genericsetup:upgradeStep
+      title="Upgrade to 1403"
+      description="Add new index to Prenotazioni c.t."
+      profile="redturtle.prenotazioni:default"
+      source="1402"
+      destination="1403"
+      handler=".upgrades.to_1403"
+      />
+
+  <genericsetup:upgradeStep
+      title="Upgrade to 1500"
+      description="Remove unused type"
+      profile="redturtle.prenotazioni:default"
+      source="1403"
+      destination="1500"
+      handler=".upgrades.to_1500"
+      />
+
+  <genericsetup:upgradeStep
+      title="Upgrade to 1501"
+      description="Add new bundle for custom widget"
+      profile="redturtle.prenotazioni:default"
+      source="1500"
+      destination="1501"
+      handler=".upgrades.update_registry"
+      />
+
 </configure>
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/utilities/urls.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/utilities/urls.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/viewlets/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/viewlets/templates/app_io.pt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/viewlets/templates/app_io.pt`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/configure.zcml` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,19 @@
       />
 
 
   <utility
       name="redturtle.prenotazioni.VocOreInizio"
       component=".voc_ore_inizio.VocOreInizioFactory"
       />
+  <utility
+      name="redturtle.prenotazioni.VocMonths"
+      component=".voc_months.VocMonthsFactory"
+      />
+
 
 
   <utility
       name="redturtle.prenotazioni.gates"
       component=".gates.GatesVocabularyFactory"
       />
   <utility
```

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/gates.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/gates.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/review_states.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/review_states.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/tipologies.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/tipologies.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py`

 * *Files identical despite different names*

### Comparing `redturtle.prenotazioni-1.7.1/src/redturtle.prenotazioni.egg-info/SOURCES.txt` & `redturtle.prenotazioni-2.0.0.dev0/src/redturtle.prenotazioni.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 src/redturtle/prenotazioni/actions/__init__.py
 src/redturtle/prenotazioni/actions/configure.zcml
 src/redturtle/prenotazioni/actions/mail.py
 src/redturtle/prenotazioni/adapters/__init__.py
 src/redturtle/prenotazioni/adapters/booker.py
 src/redturtle/prenotazioni/adapters/configure.zcml
 src/redturtle/prenotazioni/adapters/conflict.py
-src/redturtle/prenotazioni/adapters/prenotazione.py
 src/redturtle/prenotazioni/adapters/prenotazione_menu.py
 src/redturtle/prenotazioni/adapters/slot.py
 src/redturtle/prenotazioni/adapters/stringinterp.py
 src/redturtle/prenotazioni/browser/__init__.py
 src/redturtle/prenotazioni/browser/add_edit_view.py
 src/redturtle/prenotazioni/browser/base.py
 src/redturtle/prenotazioni/browser/configure.zcml
@@ -58,24 +57,42 @@
 src/redturtle/prenotazioni/browser/prenotazione_add.py
 src/redturtle/prenotazioni/browser/prenotazione_move.py
 src/redturtle/prenotazioni/browser/prenotazione_print.py
 src/redturtle/prenotazioni/browser/prenotazioni_context_state.py
 src/redturtle/prenotazioni/browser/prenotazioni_portal_state.py
 src/redturtle/prenotazioni/browser/prenotazioni_search.py
 src/redturtle/prenotazioni/browser/vacations.py
+src/redturtle/prenotazioni/browser/viewlets.py
 src/redturtle/prenotazioni/browser/week.py
+src/redturtle/prenotazioni/browser/widget.py
 src/redturtle/prenotazioni/browser/z3c_custom_widget.py
 src/redturtle/prenotazioni/browser/overrides/.gitkeep
 src/redturtle/prenotazioni/browser/static/.gitkeep
 src/redturtle/prenotazioni/browser/static/calendar-add.png
 src/redturtle/prenotazioni/browser/static/calendar-icon.png
 src/redturtle/prenotazioni/browser/static/cross-icon.png
 src/redturtle/prenotazioni/browser/static/redturtle-reservation.css
 src/redturtle/prenotazioni/browser/static/redturtle-reservation.js
 src/redturtle/prenotazioni/browser/static/times-solid.png
+src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css
+src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.css.map
+src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js
+src/redturtle/prenotazioni/browser/static/widget/dist/prod/main.js.map
+src/redturtle/prenotazioni/browser/static/widget/js/index.js
+src/redturtle/prenotazioni/browser/static/widget/js/WidgetContainer/index.js
+src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.js
+src/redturtle/prenotazioni/browser/static/widget/js/WidgetDataContainer/index.less
+src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.js
+src/redturtle/prenotazioni/browser/static/widget/js/fields/DaysTableField.less
+src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.js
+src/redturtle/prenotazioni/browser/static/widget/js/fields/IntervalSelectorField.less
+src/redturtle/prenotazioni/browser/static/widget/js/fields/SelectField.js
+src/redturtle/prenotazioni/browser/static/widget/js/fields/TextLineField.js
+src/redturtle/prenotazioni/browser/static/widget/js/utils/i18n.js
+src/redturtle/prenotazioni/browser/static/widget/js/utils/widgetContext.js
 src/redturtle/prenotazioni/browser/stats/__init__.py
 src/redturtle/prenotazioni/browser/stats/booking_stats.pt
 src/redturtle/prenotazioni/browser/stats/booking_stats.py
 src/redturtle/prenotazioni/browser/stats/configure.zcml
 src/redturtle/prenotazioni/browser/templates/booking_type_radio_widget.pt
 src/redturtle/prenotazioni/browser/templates/custom_dgf_input.pt
 src/redturtle/prenotazioni/browser/templates/delete_reservation.pt
@@ -84,35 +101,36 @@
 src/redturtle/prenotazioni/browser/templates/prenotazione.pt
 src/redturtle/prenotazioni/browser/templates/prenotazione_add.pt
 src/redturtle/prenotazioni/browser/templates/prenotazione_macros.pt
 src/redturtle/prenotazioni/browser/templates/prenotazione_move.pt
 src/redturtle/prenotazioni/browser/templates/prenotazione_print.pt
 src/redturtle/prenotazioni/browser/templates/prenotazioni_search.pt
 src/redturtle/prenotazioni/browser/templates/week.pt
+src/redturtle/prenotazioni/browser/templates/week_table_overrides_widget_input.pt
 src/redturtle/prenotazioni/content/__init__.py
 src/redturtle/prenotazioni/content/pause.py
 src/redturtle/prenotazioni/content/prenotazione.py
 src/redturtle/prenotazioni/content/prenotazioni_day.py
 src/redturtle/prenotazioni/content/prenotazioni_folder.py
-src/redturtle/prenotazioni/content/prenotazioni_folder_container.py
 src/redturtle/prenotazioni/content/prenotazioni_week.py
 src/redturtle/prenotazioni/content/prenotazioni_year.py
+src/redturtle/prenotazioni/content/validators.py
 src/redturtle/prenotazioni/contentrules/__init__.py
 src/redturtle/prenotazioni/contentrules/configure.zcml
 src/redturtle/prenotazioni/contentrules/handlers.py
 src/redturtle/prenotazioni/contentrules/sendMovedPrenotazione.py
 src/redturtle/prenotazioni/events/__init__.py
 src/redturtle/prenotazioni/events/configure.zcml
 src/redturtle/prenotazioni/events/events_logger.py
 src/redturtle/prenotazioni/events/prenotazione.py
 src/redturtle/prenotazioni/events/prenotazioni_folder.py
 src/redturtle/prenotazioni/indexers/__init__.py
 src/redturtle/prenotazioni/indexers/configure.zcml
 src/redturtle/prenotazioni/indexers/searchable_text.py
-src/redturtle/prenotazioni/locales/redturtle.prenotazioni-manual.pot
+src/redturtle/prenotazioni/locales/manual.pot
 src/redturtle/prenotazioni/locales/redturtle.prenotazioni.pot
 src/redturtle/prenotazioni/locales/update.py
 src/redturtle/prenotazioni/locales/update.sh
 src/redturtle/prenotazioni/locales/en/LC_MESSAGES/redturtle.prenotazioni.po
 src/redturtle/prenotazioni/locales/it/LC_MESSAGES/redturtle.prenotazioni.po
 src/redturtle/prenotazioni/monkeypatcher/__init__.py
 src/redturtle/prenotazioni/monkeypatcher/configure.zcml
@@ -126,30 +144,46 @@
 src/redturtle/prenotazioni/profiles/default/workflows.xml
 src/redturtle/prenotazioni/profiles/default/registry/caching.xml
 src/redturtle/prenotazioni/profiles/default/registry/resources.xml
 src/redturtle/prenotazioni/profiles/default/registry/settings.xml
 src/redturtle/prenotazioni/profiles/default/types/Prenotazione.xml
 src/redturtle/prenotazioni/profiles/default/types/PrenotazioniDay.xml
 src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolder.xml
-src/redturtle/prenotazioni/profiles/default/types/PrenotazioniFolderContainer.xml
 src/redturtle/prenotazioni/profiles/default/types/PrenotazioniWeek.xml
 src/redturtle/prenotazioni/profiles/default/types/PrenotazioniYear.xml
 src/redturtle/prenotazioni/profiles/default/workflows/prenotazioni_workflow/definition.xml
 src/redturtle/prenotazioni/profiles/default/workflows/prenotazionifolder_workflow/definition.xml
+src/redturtle/prenotazioni/profiles/to_1402/contentrules.xml
+src/redturtle/prenotazioni/profiles/to_1500/types.xml
 src/redturtle/prenotazioni/profiles/uninstall/browserlayer.xml
 src/redturtle/prenotazioni/profiles/uninstall/registry/resources.xml
 src/redturtle/prenotazioni/profiles/uninstall/registry/settings.xml
 src/redturtle/prenotazioni/restapi/__init__.py
 src/redturtle/prenotazioni/restapi/configure.zcml
 src/redturtle/prenotazioni/restapi/serializers/__init__.py
 src/redturtle/prenotazioni/restapi/serializers/configure.zcml
 src/redturtle/prenotazioni/restapi/serializers/adapters/__init__.py
 src/redturtle/prenotazioni/restapi/serializers/adapters/configure.zcml
+src/redturtle/prenotazioni/restapi/serializers/adapters/prenotazione.py
 src/redturtle/prenotazioni/restapi/serializers/adapters/slot.py
 src/redturtle/prenotazioni/restapi/services/configure.zcml
+src/redturtle/prenotazioni/restapi/services/booking/__init__.py
+src/redturtle/prenotazioni/restapi/services/booking/add.py
+src/redturtle/prenotazioni/restapi/services/booking/configure.zcml
+src/redturtle/prenotazioni/restapi/services/booking/delete.py
+src/redturtle/prenotazioni/restapi/services/booking/get.py
+src/redturtle/prenotazioni/restapi/services/booking_schema/__init__.py
+src/redturtle/prenotazioni/restapi/services/booking_schema/configure.zcml
+src/redturtle/prenotazioni/restapi/services/booking_schema/get.py
+src/redturtle/prenotazioni/restapi/services/bookings/__init__.py
+src/redturtle/prenotazioni/restapi/services/bookings/configure.zcml
+src/redturtle/prenotazioni/restapi/services/bookings/search.py
+src/redturtle/prenotazioni/restapi/services/month_slots/__init__.py
+src/redturtle/prenotazioni/restapi/services/month_slots/configure.zcml
+src/redturtle/prenotazioni/restapi/services/month_slots/get.py
 src/redturtle/prenotazioni/restapi/services/week_slots/__init__.py
 src/redturtle/prenotazioni/restapi/services/week_slots/configure.zcml
 src/redturtle/prenotazioni/restapi/services/week_slots/get.py
 src/redturtle/prenotazioni/scripts/__init__.py
 src/redturtle/prenotazioni/scripts/app_io.py
 src/redturtle/prenotazioni/scripts/io_tools/README.md
 src/redturtle/prenotazioni/scripts/io_tools/__init__.py
@@ -158,22 +192,33 @@
 src/redturtle/prenotazioni/scripts/io_tools/io.db
 src/redturtle/prenotazioni/scripts/io_tools/io_tools.py
 src/redturtle/prenotazioni/scripts/io_tools/monkey.py
 src/redturtle/prenotazioni/scripts/io_tools/rdbms.py
 src/redturtle/prenotazioni/scripts/io_tools/spec.yaml
 src/redturtle/prenotazioni/scripts/io_tools/storage.py
 src/redturtle/prenotazioni/tests/__init__.py
+src/redturtle/prenotazioni/tests/test_booking_info.py
+src/redturtle/prenotazioni/tests/test_booking_schema.py
+src/redturtle/prenotazioni/tests/test_delete_booking.py
+src/redturtle/prenotazioni/tests/test_delete_booking_api.py
+src/redturtle/prenotazioni/tests/test_month_slots.py
+src/redturtle/prenotazioni/tests/test_prenotazione.py
+src/redturtle/prenotazioni/tests/test_prenotazione_searchable_item_serializer.py
+src/redturtle/prenotazioni/tests/test_prenotazioni_search.py
 src/redturtle/prenotazioni/tests/test_setup.py
+src/redturtle/prenotazioni/tests/test_week_table_overrides.py
 src/redturtle/prenotazioni/utilities/__init__.py
+src/redturtle/prenotazioni/utilities/dateutils.py
 src/redturtle/prenotazioni/utilities/urls.py
 src/redturtle/prenotazioni/viewlets/__init__.py
 src/redturtle/prenotazioni/viewlets/app_io.py
 src/redturtle/prenotazioni/viewlets/configure.zcml
 src/redturtle/prenotazioni/viewlets/templates/app_io.pt
 src/redturtle/prenotazioni/vocabularies/__init__.py
 src/redturtle/prenotazioni/vocabularies/configure.zcml
 src/redturtle/prenotazioni/vocabularies/gates.py
 src/redturtle/prenotazioni/vocabularies/requirable_booking_fields.py
 src/redturtle/prenotazioni/vocabularies/review_states.py
 src/redturtle/prenotazioni/vocabularies/tipologies.py
 src/redturtle/prenotazioni/vocabularies/voc_durata_incontro.py
+src/redturtle/prenotazioni/vocabularies/voc_months.py
 src/redturtle/prenotazioni/vocabularies/voc_ore_inizio.py
```

