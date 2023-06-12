# Comparing `tmp/five_card_draw-1.0.8.tar.gz` & `tmp/five_card_draw-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five_card_draw-1.0.8.tar", last modified: Mon Jun 12 16:35:51 2023, max compression
+gzip compressed data, was "five_card_draw-1.1.0.tar", last modified: Mon Jun 12 17:14:37 2023, max compression
```

## Comparing `five_card_draw-1.0.8.tar` & `five_card_draw-1.1.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 16:35:51.155023 five_card_draw-1.0.8/
--rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       55 2023-06-12 13:48:00.000000 five_card_draw-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7300 2023-06-12 16:35:51.155023 five_card_draw-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6996 2023-06-12 15:44:46.000000 five_card_draw-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 16:35:50.930230 five_card_draw-1.0.8/five_card_draw/
-drwxrwxrwx   0        0        0        0 2023-06-12 16:35:51.154026 five_card_draw-1.0.8/five_card_draw/data/
--rw-rw-rw-   0        0        0    56484 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/C10.png
--rw-rw-rw-   0        0        0   187958 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/C11.png
--rw-rw-rw-   0        0        0   205820 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/C12.png
--rw-rw-rw-   0        0        0   189382 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C13.png
--rw-rw-rw-   0        0        0    37544 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C14.png
--rw-rw-rw-   0        0        0    23382 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C2.png
--rw-rw-rw-   0        0        0    29340 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C3.png
--rw-rw-rw-   0        0        0    29132 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C4.png
--rw-rw-rw-   0        0        0    35845 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C5.png
--rw-rw-rw-   0        0        0    40916 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C6.png
--rw-rw-rw-   0        0        0    41816 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C7.png
--rw-rw-rw-   0        0        0    48567 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C8.png
--rw-rw-rw-   0        0        0    52318 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C9.png
--rw-rw-rw-   0        0        0   432659 2021-11-02 01:23:17.000000 five_card_draw-1.0.8/five_card_draw/data/CardBack.png
--rw-rw-rw-   0        0        0    46699 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/D10.png
--rw-rw-rw-   0        0        0   197802 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/D11.png
--rw-rw-rw-   0        0        0   180712 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/D12.png
--rw-rw-rw-   0        0        0   198565 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D13.png
--rw-rw-rw-   0        0        0    30901 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D14.png
--rw-rw-rw-   0        0        0    19170 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D2.png
--rw-rw-rw-   0        0        0    23815 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D3.png
--rw-rw-rw-   0        0        0    24296 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D4.png
--rw-rw-rw-   0        0        0    29806 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D5.png
--rw-rw-rw-   0        0        0    33800 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D6.png
--rw-rw-rw-   0        0        0    34176 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D7.png
--rw-rw-rw-   0        0        0    40724 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D8.png
--rw-rw-rw-   0        0        0    43365 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/D9.png
--rw-rw-rw-   0        0        0    49317 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/H10.png
--rw-rw-rw-   0        0        0   203728 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/H11.png
--rw-rw-rw-   0        0        0   197792 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/H12.png
--rw-rw-rw-   0        0        0   207052 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H13.png
--rw-rw-rw-   0        0        0    36444 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H14.png
--rw-rw-rw-   0        0        0    20058 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H2.png
--rw-rw-rw-   0        0        0    24919 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H3.png
--rw-rw-rw-   0        0        0    25320 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H4.png
--rw-rw-rw-   0        0        0    31082 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H5.png
--rw-rw-rw-   0        0        0    35239 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H6.png
--rw-rw-rw-   0        0        0    35904 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H7.png
--rw-rw-rw-   0        0        0    42890 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H8.png
--rw-rw-rw-   0        0        0    45669 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/H9.png
--rw-rw-rw-   0        0        0    50853 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/S10.png
--rw-rw-rw-   0        0        0   190953 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/S11.png
--rw-rw-rw-   0        0        0   186480 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S12.png
--rw-rw-rw-   0        0        0   183329 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S13.png
--rw-rw-rw-   0        0        0    56051 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S14.png
--rw-rw-rw-   0        0        0    21104 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S2.png
--rw-rw-rw-   0        0        0    26211 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S3.png
--rw-rw-rw-   0        0        0    26311 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S4.png
--rw-rw-rw-   0        0        0    32110 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S5.png
--rw-rw-rw-   0        0        0    36726 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S6.png
--rw-rw-rw-   0        0        0    37510 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S7.png
--rw-rw-rw-   0        0        0    43823 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S8.png
--rw-rw-rw-   0        0        0    46996 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/S9.png
--rw-rw-rw-   0        0        0   560393 2023-06-08 17:03:00.000000 five_card_draw-1.0.8/five_card_draw/data/ScoringImage.png
--rw-rw-rw-   0        0        0    43719 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/black_joker.png
--rw-rw-rw-   0        0        0    44079 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/red_joker.png
--rw-rw-rw-   0        0        0        4 2023-06-09 00:26:49.000000 five_card_draw-1.0.8/five_card_draw/fcd_bank.txt
--rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.8/five_card_draw/fcd_functions.py
--rw-rw-rw-   0        0        0    15557 2023-06-12 16:33:46.000000 five_card_draw-1.0.8/five_card_draw/fcd_pagegui.py
--rw-rw-rw-   0        0        0      486 2023-06-12 15:31:35.000000 five_card_draw-1.0.8/five_card_draw/poker_start.py
-drwxrwxrwx   0        0        0        0 2023-06-12 16:35:50.944480 five_card_draw-1.0.8/five_card_draw.egg-info/
--rw-rw-rw-   0        0        0     7300 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1915 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 16:35:51.155023 five_card_draw-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1687 2023-06-12 16:35:28.000000 five_card_draw-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:14:37.530204 five_card_draw-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-12 17:14:37.530204 five_card_draw-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:14:37.518204 five_card_draw-1.1.0/five_card_draw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:14:37.530204 five_card_draw-1.1.0/five_card_draw/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    56484 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C10.png
+-rw-r--r--   0 runner    (1001) docker     (123)   187958 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C11.png
+-rw-r--r--   0 runner    (1001) docker     (123)   205820 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C12.png
+-rw-r--r--   0 runner    (1001) docker     (123)   189382 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C13.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37544 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C14.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23382 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29340 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35845 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40916 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C6.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41816 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C7.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C8.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/C9.png
+-rw-r--r--   0 runner    (1001) docker     (123)   432659 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/CardBack.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46699 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D10.png
+-rw-r--r--   0 runner    (1001) docker     (123)   197802 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D11.png
+-rw-r--r--   0 runner    (1001) docker     (123)   180712 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D12.png
+-rw-r--r--   0 runner    (1001) docker     (123)   198565 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D13.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30901 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D14.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19170 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24296 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29806 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33800 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D6.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34176 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D7.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40724 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D8.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43365 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/D9.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49317 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H10.png
+-rw-r--r--   0 runner    (1001) docker     (123)   203728 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H11.png
+-rw-r--r--   0 runner    (1001) docker     (123)   197792 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H12.png
+-rw-r--r--   0 runner    (1001) docker     (123)   207052 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H13.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36444 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H14.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20058 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24919 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31082 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35239 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H6.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H7.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42890 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H8.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45669 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/H9.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50853 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S10.png
+-rw-r--r--   0 runner    (1001) docker     (123)   190953 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S11.png
+-rw-r--r--   0 runner    (1001) docker     (123)   186480 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S12.png
+-rw-r--r--   0 runner    (1001) docker     (123)   183329 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S13.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56051 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S14.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26211 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26311 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32110 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S5.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36726 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S6.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37510 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S7.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43823 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S8.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46996 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/S9.png
+-rw-r--r--   0 runner    (1001) docker     (123)   560393 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/ScoringImage.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43719 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/black_joker.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44079 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/data/red_joker.png
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/fcd_bank.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/fcd_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/fcd_pagegui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/five_card_draw/poker_start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:14:37.518204 five_card_draw-1.1.0/five_card_draw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-12 17:14:37.000000 five_card_draw-1.1.0/five_card_draw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-12 17:14:37.000000 five_card_draw-1.1.0/five_card_draw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:14:37.000000 five_card_draw-1.1.0/five_card_draw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 17:14:37.000000 five_card_draw-1.1.0/five_card_draw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 17:14:37.000000 five_card_draw-1.1.0/five_card_draw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:14:37.530204 five_card_draw-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-12 17:14:27.000000 five_card_draw-1.1.0/setup.py
```

### Comparing `five_card_draw-1.0.8/PKG-INFO` & `five_card_draw-1.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,187 +1,176 @@
-Metadata-Version: 2.1
-Name: five_card_draw
-Version: 1.0.8
-Summary: 5 Card Draw Video Poker application
-Home-page: https://github.com/ralbee1/5_card_draw
-Author: Richard Albee
-Author-email: Ralbee1@iwu.edu
-License: LICENSE.txt
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-<a name="readme-top"></a>
-
-<!-- VideoPoker-5CardRedraw -->
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-[![LinkedIn][linkedin-shield]][linkedin-url]
-
-
-<!-- PROJECT LOGO -->
-<br />
-<div align="center">
-  <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw">
-    <img src="documentation/logo.png" alt="Logo" width="80" height="80">
-  </a>
-
-<h3 align="center">VideoPoker-5CardRedraw</h3>
-
-  <p align="center">
-    A pythonic creation of a 5 card redraw video poker.
-    <br />
-    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
-    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw">View Demo</a>
-    ·
-    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw/issues">Report Bug</a>
-    ·
-    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw/issues">Request Feature</a>
-  </p>
-</div>
-
-
-
-<!-- TABLE OF CONTENTS -->
-<details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li>
-      <a href="#about-the-project">About The Project</a>
-      <ul>
-        <li><a href="#built-with">Built With</a></li>
-        <li><a href="#Features">Features</a></li>
-      </ul>
-    </li>
-    <li>
-      <a href="#getting-started">Getting Started</a>
-      <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
-        <li><a href="#installation">Installation</a></li>
-      </ul>
-    </li>
-    <li><a href="#usage">Usage</a></li>
-    <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgments">Acknowledgments</a></li>
-  </ol>
-</details>
-
-
-<!-- ABOUT THE PROJECT -->
-## About The Project
-<!-- 
-[![Product Name Screen Shot][product-screenshot]](https://example.com)
--->
-5 Card Draw is a playable Python 5 card draw poker application. This project served as a hands-on Python learning experience in 2021. On my journey, I learned about creating graphical user interfaces in python, pythonic best practices, CI/CD workflows, PyPi deployments, and much more. The beautiful learning opportunity provided this project was balancing desired learning opportunities and refining 5 Card Draw into a polished application. This project is currently archived with the last remaining features involved further polishing the UI/UX experience, adding sound, and cashing out player credits. If I were to start over, I'd rank poker hands with a symantic system over a integer score.
- 
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-### Features
-
-- [ ] **5 Card Redraw**
-  - [ ] Modular Hand Ranking and Scoring
-  - [ ] Player Hand and Deck creation
-  - [ ] Playable GUI interface
-  - [ ] Bank text file
-- [ ] **PyPi Installs**
-- [ ] **Pep 8 Standards**
-- [ ] **GitHub CI/CD Pipelines**
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-<!-- GETTING STARTED -->
-## Getting Started
-
-The following is an guide for running 5 card redraw poker locally.
-
-### Prerequisites
-
-1. [Python 3.10.8 or Newer](https://www.python.org/downloads/release/python-3108/)
-
-
-### Installation
-
-Local Repo Install:
-<br/>
-Summary: The developer install is for those who want to contribute to or clone VideoPoker-5CardRedraw.
-1. Clone the repo (or use Github Desktop)
-   ```sh
-   git clone https://github.com/ralbee1/5_card_draw.git
-   ```
-2. Open the CLI and navigate the current working directory to where you cloned VideoPoker-5CardDraw
-3. Install the Pip Package from the CLI, copy and run this command:
-   ```sh
-   py -m pip install -e .
-   ```
-<br/>
-<br/>
-User Install
-<br/>
-1. Automatic User Install from the Command line via PyPi.
-   ```sh
-   pip install five-card-draw
-   ```
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-<!-- USAGE EXAMPLES -->
-## Usage / How to Play
-If your python files open with Python by default then from the commmand line run:
-
-  ```js
-  poker_start.py;
-  ```
-
-Troubleshooting:
-1. "'poker_start.py' is not recognized as an internal or external command, operable program or batch file."
-  Your terminal needs to be able to find the file. For windows, you need to ensure your python "script" folder is in your path variable
-  For example: C:\Users\{username}\AppData\Roaming\Python\{pythonversion}\Scripts
-  You may also navigate to where the pip was installed and run poker_start.py with python manually.
-
-The game is played by aiming to make the best poker hand possible. The top of the interface shows the hand ranking and the payouts sorted by how many credits you bet per round, 1 thru 5. To begin, click DEAL. You hold cards with the intent of keeping them and drawing new cards to try to improve your hand ranking. After drawing new cards, your hand is automatically scored and profits are payed out. You may then click "DEAL" and start over.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-<!-- CONTACT -->
-## Contact
-
-* []()Email - ralbee1@iwu.edu
-* []()Project Link: [https://github.com/ralbee1/VideoPoker-5CardRedraw](https://github.com/ralbee1/VideoPoker-5CardRedraw)
-
-
-
-<!-- ACKNOWLEDGMENTS -->
-## Acknowledgments
-
-* []() This variant of poker was inspired by Super Double Double as found in Las Vegas Casinos.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[contributors-shield]: https://img.shields.io/github/contributors/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[contributors-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[forks-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/network/members
-[stars-shield]: https://img.shields.io/github/stars/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[stars-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/stargazers
-[issues-shield]: https://img.shields.io/github/issues/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[issues-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/issues
-[license-shield]: https://img.shields.io/github/license/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[license-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/blob/master/LICENSE.txt
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
-[linkedin-url]: https://linkedin.com/in/Richard-Albee
-[product-screenshot]: images/screenshot.png
-[python.org]: https://www.python.org/static/img/python-logo.png
-[python-url]: https://www.python.org/
-[pypi.org]: https://pypi.org/static/images/logo-small.2a411bc6.svg
-[pypi-url]: https://pypi.org/project/pip/
+<a name="readme-top"></a>
+
+<!-- VideoPoker-5CardRedraw -->
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+[![LinkedIn][linkedin-shield]][linkedin-url]
+
+
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw">
+    <img src="documentation/logo.png" alt="Logo" width="80" height="80">
+  </a>
+
+<h3 align="center">VideoPoker-5CardRedraw</h3>
+
+  <p align="center">
+    A pythonic creation of a 5 card redraw video poker.
+    <br />
+    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw"><strong>Explore the docs »</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw">View Demo</a>
+    ·
+    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw/issues">Report Bug</a>
+    ·
+    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw/issues">Request Feature</a>
+  </p>
+</div>
+
+
+
+<!-- TABLE OF CONTENTS -->
+<details>
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+      <ul>
+        <li><a href="#built-with">Built With</a></li>
+        <li><a href="#Features">Features</a></li>
+      </ul>
+    </li>
+    <li>
+      <a href="#getting-started">Getting Started</a>
+      <ul>
+        <li><a href="#prerequisites">Prerequisites</a></li>
+        <li><a href="#installation">Installation</a></li>
+      </ul>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#contact">Contact</a></li>
+    <li><a href="#acknowledgments">Acknowledgments</a></li>
+  </ol>
+</details>
+
+
+<!-- ABOUT THE PROJECT -->
+## About The Project
+<!-- 
+[![Product Name Screen Shot][product-screenshot]](https://example.com)
+-->
+5 Card Draw is a playable Python 5-card draw poker application. This project served as a hands-on Python learning experience in 2021. On my journey, I learned about creating graphical user interfaces in Python, pythonic best practices, CI/CD workflows, PyPi deployments, and much more. The beautiful learning opportunity this project provided was balancing desired learning opportunities and refining 5 Card Draw into a polished application. This project archived with the last remaining features involved in further polishing the UI/UX experience, adding sound, and cashing out player credits. If I were to start over, I'd rank poker hands with a semantic system over an integer score.
+ 
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+### Features
+
+- [ ] **5 Card Redraw**
+  - [ ] Modular Hand Ranking and Scoring
+  - [ ] Player Hand and Deck creation
+  - [ ] Playable GUI interface
+  - [ ] Bank text file
+- [ ] **PyPi Installs**
+- [ ] **Pep 8 Standards**
+- [ ] **GitHub CI/CD Pipelines**
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- GETTING STARTED -->
+## Getting Started
+
+The following is an guide for running 5 card redraw poker locally.
+
+### Prerequisites
+
+1. [Python 3.10.8 or Newer](https://www.python.org/downloads/release/python-3108/)
+
+
+### Installation
+
+Local Repo Install:
+<br/>
+Summary: The developer install is for those who want to contribute to or clone VideoPoker-5CardRedraw.
+1. Clone the repo (or use Github Desktop)
+   ```sh
+   git clone https://github.com/ralbee1/5_card_draw.git
+   ```
+2. Open the CLI and navigate the current working directory to where you cloned VideoPoker-5CardDraw
+3. Install the Pip Package from the CLI, copy and run this command:
+   ```sh
+   py -m pip install -e .
+   ```
+<br/>
+<br/>
+User Install
+<br/>
+1. Automatic User Install from the Command line via PyPi.
+   ```sh
+   pip install five-card-draw
+   ```
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+<!-- USAGE EXAMPLES -->
+## Usage / How to Play
+If your python files open with Python by default then from the commmand line run:
+
+  ```js
+  poker_start.py;
+  ```
+
+Troubleshooting:
+1. "'poker_start.py' is not recognized as an internal or external command, operable program or batch file."
+  Your terminal needs to be able to find the file. For windows, you need to ensure your python "script" folder is in your path variable
+  For example: C:\Users\{username}\AppData\Roaming\Python\{pythonversion}\Scripts
+  You may also navigate to where the pip was installed and run poker_start.py with python manually.
+
+The game is played by aiming to make the best poker hand possible. The top of the interface shows the hand ranking and the payouts sorted by how many credits you bet per round, 1 thru 5. To begin, click DEAL. You hold cards with the intent of keeping them and drawing new cards to try to improve your hand ranking. After drawing new cards, your hand is automatically scored and profits paid out. You may then click "DEAL" and start over.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- CONTACT -->
+## Contact
+
+* []()Email - ralbee1@iwu.edu
+* []()Project Link: [https://github.com/ralbee1/VideoPoker-5CardRedraw](https://github.com/ralbee1/VideoPoker-5CardRedraw)
+
+
+
+<!-- ACKNOWLEDGMENTS -->
+## Acknowledgments
+
+* []() This variant of poker was inspired by Super Double Double as found in Las Vegas Casinos.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[contributors-shield]: https://img.shields.io/github/contributors/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[contributors-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[forks-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/network/members
+[stars-shield]: https://img.shields.io/github/stars/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[stars-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/stargazers
+[issues-shield]: https://img.shields.io/github/issues/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[issues-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/issues
+[license-shield]: https://img.shields.io/github/license/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[license-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/blob/master/LICENSE.txt
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+[linkedin-url]: https://linkedin.com/in/Richard-Albee
+[product-screenshot]: images/screenshot.png
+[python.org]: https://www.python.org/static/img/python-logo.png
+[python-url]: https://www.python.org/
+[pypi.org]: https://pypi.org/static/images/logo-small.2a411bc6.svg
+[pypi-url]: https://pypi.org/project/pip/
```

#### html2text {}

```diff
@@ -1,14 +1,10 @@
-Metadata-Version: 2.1 Name: five_card_draw Version: 1.0.8 Summary: 5 Card Draw
-Video Poker application Home-page: https://github.com/ralbee1/5_card_draw
-Author: Richard Albee Author-email: Ralbee1@iwu.edu License: LICENSE.txt
-Description-Content-Type: text/markdown License-File: LICENSE.txt   [!
-[Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
-[forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
-[issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
+  [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
+shield]][issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
 [linkedin-shield]][linkedin-url]
                                     [Logo]
                        **** VideoPoker-5CardRedraw ****
              A pythonic creation of a 5 card redraw video poker.
                              Explore_the_docs_Â»
 
                   View_Demo Â· Report_Bug Â· Request_Feature
@@ -18,24 +14,24 @@
           o Features
    2. Getting_Started
           o Prerequisites
           o Installation
    3. Usage
    4. Contact
    5. Acknowledgments
-  ## About The Project  5 Card Draw is a playable Python 5 card draw poker
+  ## About The Project  5 Card Draw is a playable Python 5-card draw poker
 application. This project served as a hands-on Python learning experience in
 2021. On my journey, I learned about creating graphical user interfaces in
-python, pythonic best practices, CI/CD workflows, PyPi deployments, and much
-more. The beautiful learning opportunity provided this project was balancing
+Python, pythonic best practices, CI/CD workflows, PyPi deployments, and much
+more. The beautiful learning opportunity this project provided was balancing
 desired learning opportunities and refining 5 Card Draw into a polished
-application. This project is currently archived with the last remaining
-features involved further polishing the UI/UX experience, adding sound, and
-cashing out player credits. If I were to start over, I'd rank poker hands with
-a symantic system over a integer score.
+application. This project archived with the last remaining features involved in
+further polishing the UI/UX experience, adding sound, and cashing out player
+credits. If I were to start over, I'd rank poker hands with a semantic system
+over an integer score.
                                                                   (back_to_top)
 ### Features - [ ] **5 Card Redraw** - [ ] Modular Hand Ranking and Scoring -
 [ ] Player Hand and Deck creation - [ ] Playable GUI interface - [ ] Bank text
 file - [ ] **PyPi Installs** - [ ] **Pep 8 Standards** - [ ] **GitHub CI/CD
 Pipelines**
                                                                   (back_to_top)
  ## Getting Started The following is an guide for running 5 card redraw poker
@@ -60,15 +56,15 @@
 path variable For example: C:\Users\{username}\AppData\Roaming\Python\
 {pythonversion}\Scripts You may also navigate to where the pip was installed
 and run poker_start.py with python manually. The game is played by aiming to
 make the best poker hand possible. The top of the interface shows the hand
 ranking and the payouts sorted by how many credits you bet per round, 1 thru 5.
 To begin, click DEAL. You hold cards with the intent of keeping them and
 drawing new cards to try to improve your hand ranking. After drawing new cards,
-your hand is automatically scored and profits are payed out. You may then click
+your hand is automatically scored and profits paid out. You may then click
 "DEAL" and start over.
                                                                   (back_to_top)
  ## Contact * []()Email - ralbee1@iwu.edu * []()Project Link: [https://
 github.com/ralbee1/VideoPoker-5CardRedraw](https://github.com/ralbee1/
 VideoPoker-5CardRedraw)  ## Acknowledgments * []() This variant of poker was
 inspired by Super Double Double as found in Las Vegas Casinos.
                                                                   (back_to_top)
```

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C10.png` & `five_card_draw-1.1.0/five_card_draw/data/C10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C11.png` & `five_card_draw-1.1.0/five_card_draw/data/C11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C12.png` & `five_card_draw-1.1.0/five_card_draw/data/C12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C13.png` & `five_card_draw-1.1.0/five_card_draw/data/C13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C14.png` & `five_card_draw-1.1.0/five_card_draw/data/C14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C2.png` & `five_card_draw-1.1.0/five_card_draw/data/C2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C3.png` & `five_card_draw-1.1.0/five_card_draw/data/C3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C4.png` & `five_card_draw-1.1.0/five_card_draw/data/C4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C5.png` & `five_card_draw-1.1.0/five_card_draw/data/C5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C6.png` & `five_card_draw-1.1.0/five_card_draw/data/C6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C7.png` & `five_card_draw-1.1.0/five_card_draw/data/C7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C8.png` & `five_card_draw-1.1.0/five_card_draw/data/C8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/C9.png` & `five_card_draw-1.1.0/five_card_draw/data/C9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/CardBack.png` & `five_card_draw-1.1.0/five_card_draw/data/CardBack.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D10.png` & `five_card_draw-1.1.0/five_card_draw/data/D10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D11.png` & `five_card_draw-1.1.0/five_card_draw/data/D11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D12.png` & `five_card_draw-1.1.0/five_card_draw/data/D12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D13.png` & `five_card_draw-1.1.0/five_card_draw/data/D13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D14.png` & `five_card_draw-1.1.0/five_card_draw/data/D14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D2.png` & `five_card_draw-1.1.0/five_card_draw/data/D2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D3.png` & `five_card_draw-1.1.0/five_card_draw/data/D3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D4.png` & `five_card_draw-1.1.0/five_card_draw/data/D4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D5.png` & `five_card_draw-1.1.0/five_card_draw/data/D5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D6.png` & `five_card_draw-1.1.0/five_card_draw/data/D6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D7.png` & `five_card_draw-1.1.0/five_card_draw/data/D7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D8.png` & `five_card_draw-1.1.0/five_card_draw/data/D8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/D9.png` & `five_card_draw-1.1.0/five_card_draw/data/D9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H10.png` & `five_card_draw-1.1.0/five_card_draw/data/H10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H11.png` & `five_card_draw-1.1.0/five_card_draw/data/H11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H12.png` & `five_card_draw-1.1.0/five_card_draw/data/H12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H13.png` & `five_card_draw-1.1.0/five_card_draw/data/H13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H14.png` & `five_card_draw-1.1.0/five_card_draw/data/H14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H2.png` & `five_card_draw-1.1.0/five_card_draw/data/H2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H3.png` & `five_card_draw-1.1.0/five_card_draw/data/H3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H4.png` & `five_card_draw-1.1.0/five_card_draw/data/H4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H5.png` & `five_card_draw-1.1.0/five_card_draw/data/H5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H6.png` & `five_card_draw-1.1.0/five_card_draw/data/H6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H7.png` & `five_card_draw-1.1.0/five_card_draw/data/H7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H8.png` & `five_card_draw-1.1.0/five_card_draw/data/H8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/H9.png` & `five_card_draw-1.1.0/five_card_draw/data/H9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S10.png` & `five_card_draw-1.1.0/five_card_draw/data/S10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S11.png` & `five_card_draw-1.1.0/five_card_draw/data/S11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S12.png` & `five_card_draw-1.1.0/five_card_draw/data/S12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S13.png` & `five_card_draw-1.1.0/five_card_draw/data/S13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S14.png` & `five_card_draw-1.1.0/five_card_draw/data/S14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S2.png` & `five_card_draw-1.1.0/five_card_draw/data/S2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S3.png` & `five_card_draw-1.1.0/five_card_draw/data/S3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S4.png` & `five_card_draw-1.1.0/five_card_draw/data/S4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S5.png` & `five_card_draw-1.1.0/five_card_draw/data/S5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S6.png` & `five_card_draw-1.1.0/five_card_draw/data/S6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S7.png` & `five_card_draw-1.1.0/five_card_draw/data/S7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S8.png` & `five_card_draw-1.1.0/five_card_draw/data/S8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/S9.png` & `five_card_draw-1.1.0/five_card_draw/data/S9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/ScoringImage.png` & `five_card_draw-1.1.0/five_card_draw/data/ScoringImage.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/black_joker.png` & `five_card_draw-1.1.0/five_card_draw/data/black_joker.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/data/red_joker.png` & `five_card_draw-1.1.0/five_card_draw/data/red_joker.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/five_card_draw/fcd_functions.py` & `five_card_draw-1.1.0/five_card_draw/fcd_functions.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,257 +1,257 @@
-'''Back end Poker functions for deck and hand creation, drawing or shuffling cards from a deck, and hand scoring.'''
-import random
-import os
-
-
-def build_deck() -> list[str]:
-    '''Create a deck of cards in suit+number format with the number being an integer and the suit is a letter:
-    Heart (H)
-    Spades (S)
-    Club (C)
-    Diamond (D)'''
-    numbers=list(range(2,15))
-    suits = ['H','S','C','D']
-    deck = []
-    for number in numbers:
-        for suit in suits:
-            card = suit+str(number)
-            deck.append(card)
-    return deck
-
-
-def shuffle_deck(cards_being_shuffled: list) -> list[str]:
-    '''Given a list, returns the list in a random order.'''
-    random.shuffle(cards_being_shuffled)
-    return cards_being_shuffled
-
-
-def draw_cards(deck: list, draw_number: int) -> tuple[list[str], list[str]]:
-    '''Draws cards from the deck provided. Returns hand and remaining deck '''
-    cards_drawn = []
-    i = 0
-    while i < draw_number:
-        cards_drawn.append(deck.pop(0))
-        i += 1
-    return cards_drawn, deck
-
-
-def create_hand(deck: list) -> tuple[list[str], list[str]]:
-    '''
-    Provided a deck, shuffles, and creates a hand.
-    Returns a tuple, (Hand,Remaining Deck)
-    '''
-    deck = build_deck()
-    deck = shuffle_deck(deck)
-    return draw_cards(deck,5)
-
-
-def score_four_of_a_kind(numbers: list) -> int:
-    '''Evaluates a int list to determine the score of quads - does not check the hand'''
-    for i in numbers:
-        if numbers.count(i) == 4:
-            four_of_a_kind = i
-        elif numbers.count(i) == 1:
-            card = i
-    return 105 + four_of_a_kind + card/100
-
-
-def score_full_house(numbers: list) -> int:
-    '''Evaluates a int list to determine the score of a full house - does not check the hand'''
-    for i in numbers:
-        if numbers.count(i) == 3:
-            trips = i
-        elif numbers.count(i) == 2:
-            pair = i
-    return 90 + trips + pair/100
-
-
-def score_three_of_a_kind(numbers: list) -> int:
-    '''Evaluates a int list to determine the score of a three of a kind - does not check the hand'''
-    trips = 0
-    cards = []
-    for i in numbers:
-        if numbers.count(i) == 3:
-            trips = i
-        else:
-            cards.append(i)
-    return 45 + trips
-
-
-def score_two_pair(numbers: list) -> int:
-    '''Evaluates a int list to determine the score of a two pair hand - does not check the hand'''
-    pairs = []
-    cards = []
-    for i in numbers:
-        if numbers.count(i) == 2:
-            pairs.append(i)
-        elif numbers.count(i) == 1:
-            cards.append(i)
-            cards = sorted(cards,reverse=True)
-    return 30 + max(pairs) + min(pairs)/100 + cards[0]/1000
-
-
-def score_pair(numbers: list) -> int:
-    '''Evaluates a int list to determine the score of a pair - does not check the hand'''
-    pair = []
-    cards  = []
-    for i in numbers:
-        if numbers.count(i) == 2:
-            pair.append(i)
-        elif numbers.count(i) == 1:
-            cards.append(i)
-            cards = sorted(cards,reverse=True)
-    return 15 + pair[0] + cards[0]/100 + cards[1]/1000 + cards[2]/10000
-
-
-def score_hand(hand: list) -> int:
-    ''' Given a hand in ['5H','3H','5C','5D','C14'] format return the poker score.
-
-    Scoring Table:
-    	                MIN	MAX
-        Royal Flush	    135	135
-        Straight Flush	120	134
-        Four of a Kind	105	119
-        Full House	    90	104
-        Flush	        75	89
-        Straight	    60	74
-        Three of a Kind	45	59
-        Two Pair        30	44
-        Pair	        15	29
-        High Card	     0	14
-    
-    Scoring for each hand has ranges to allow for payouts of different types four of a kinds.
-    '''
-    letters = [hand[i][:1] for i in range(5)] # We get the suit for each card in the hand
-    repeat_suit = [letters.count(i) for i in letters]  # We count repetitions for each suit ex [5,5,5,5,5] for flush
-
-    numbers = [int(hand[i][1:]) for i in range(5)]  # We get the number for each card in the hand
-    repeat_number = [numbers.count(i) for i in numbers] # We create a list with the repetitions of each number ex) [2,2,3,3,3] for fullhouse
-
-    dif = max(numbers) - min(numbers) # The difference between the greater and smallest number
-    handtype = 'Hand Ranking'
-    score = 0
-
-    #If all cards in hand share a suit, evaluate the type of flush.
-    if 5 in repeat_suit:
-        if numbers ==[14,13,12,11,10]:
-            handtype = 'ROYAL FLUSH'
-            score = 135
-            print(f'this hand is a {handtype}: with score: {score}')
-        elif dif == 4 and max(repeat_number) == 1:
-            handtype = 'STRAIGHT FLUSH'
-            score = 120 + max(numbers)
-            print(f'this hand is a {handtype}: with score: {score}')
-        else:
-            handtype = 'FLUSH'
-            score = 75 + max(numbers)
-            print(f'this hand is a {handtype}: with score: {score}')
-
-    #Evaluate other hands in decending ranking
-    elif 4 in repeat_number:
-        handtype = 'FOUR OF A KIND'
-        score = score_four_of_a_kind(numbers)
-        print(f'this hand is a {handtype}: with score: {score}')
-    elif sorted(repeat_number) == [2,2,3,3,3]:
-        handtype = 'FULL HOUSE'
-        score = score_full_house(numbers)
-        print(f'this hand is a {handtype}: with score: {score}')
-    elif dif == 4 and max(repeat_number) == 1:
-        handtype = 'STRAIGHT'
-        score = 60 + max(numbers)
-        print(f'this hand is a {handtype}: with score: {score}')
-    elif 3 in repeat_number:
-        handtype = 'TRIPS'
-        score = score_three_of_a_kind(numbers)
-        print(f'this hand is a {handtype}: with score: {score}')
-    elif repeat_number.count(2) == 4:
-        handtype = 'TWO PAIR'
-        score = score_two_pair(numbers)
-        print(f'this hand is a {handtype}: with score: {score}')
-    elif repeat_number.count(2) == 2:
-        handtype = 'PAIR'
-        score = score_pair(numbers)
-        print(f'this hand is a {handtype}: with score: {score}')
-    else:
-        handtype= 'HIGH CARD'
-        num = sorted(numbers,reverse=True)
-        score = num[0] + num[1]/100 + num[2]/1000 + num[3]/10000 + num[4]/100000
-        print(f'this hand is a {handtype}: with score: {score}')
-    return score, handtype
-
-
-def calculate_payout(input_score: int, input_credits: int) -> int:
-    '''Takes a score and number of paid credits, returns payout
-    
-    input_score = Accepts a number between 5 and 135.
-    input_credits = Accepts a number between 0 and 4.
-    '''
-    score_dict = {
-        'royal_flush': {'payout': [250,500,750,1000,4000]},
-        'straight_flush': {'payout': [50,100,150,200,250]},
-        'quad_aces_234_kicker': {'payout': [400,800,1200,1600,2000]},
-        'quad_aces_jackqueenking_kicker': {'payout': [320,640,960,1280,1600]},
-        'quad_234_ace_kicker': {'payout': [160,320,480,640,800]},
-        'quad_jackqueenking_face_kicker': {'payout': [160,320,480,640,800]},
-        'quad_aces': {'payout': [160,320,480,640,800]},
-        'quad_234': {'payout': [80,160,240,320,400]},
-        'quad_5toking': {'payout': [50,100,150,200,250]},
-        'full_house': {'payout': [7,14,21,28,35]},
-        'flush': {'payout': [5,10,15,25,25]},
-        'straight': {'payout': [4,8,12,16,20]},
-        'trips': {'payout': [3,6,9,12,15]},
-        'two_pair': {'payout': [1,2,3,4,5]},
-        'pair_jacks_better': {'payout': [1,2,3,4,5]}
-    }
-
-    if input_score == 135:
-        return score_dict['royal_flush']['payout'][input_credits]
-
-    elif input_score > 120:
-        return score_dict['straight_flush']['payout'][input_credits]
-
-    elif input_score > 119.10:
-        return score_dict['quad_aces_jackqueenking_kicker']['payout'][input_credits]
-
-    elif input_score > 119.4:
-        return score_dict['quad_aces']['payout'][input_credits]
-
-    elif input_score > 119.0:
-        return score_dict['quad_jackqueenking_face_kicker']['payout'][input_credits]
-
-    elif input_score > 110.0:
-        return score_dict['quad_5toking']['payout'][input_credits]
-    
-    elif input_score == 106.14 or input_score == 107.14 or input_score == 108.14:
-        return score_dict['quad_234_ace_kicker']['payout'][input_credits]
-
-    elif input_score > 107.0:
-        return score_dict['quad_234']['payout'][input_credits]
-
-    elif input_score > 90:
-        return score_dict['full_house']['payout'][input_credits]
-
-    elif input_score > 89.00:
-        return score_dict['flush']['payout'][input_credits]
-
-    elif input_score > 70.00:
-        return score_dict['straight']['payout'][input_credits]
-
-    elif input_score > 51:
-        return score_dict['trips']['payout'][input_credits]
-
-    elif input_score > 30:
-        return score_dict['two_pair']['payout'][input_credits]
-
-    elif input_score > 26:
-        return score_dict['pair_jacks_better']['payout'][input_credits]
-
-    else:
-        #Hand does not meet minimum payout
-        return 0
-
-
-def load_player_balance(bank_file_location = os.path.dirname(os.path.realpath(__file__))) -> int:
-    '''Load the player balance from bank.txt'''
-    bank_store_path = os.path.join(bank_file_location, 'fcd_bank.txt' )
-    bank_store = open(bank_store_path, 'r', encoding = 'utf-8')
-    return int(bank_store.read())
+'''Back end Poker functions for deck and hand creation, drawing or shuffling cards from a deck, and hand scoring.'''
+import random
+import os
+
+
+def build_deck() -> list[str]:
+    '''Create a deck of cards in suit+number format with the number being an integer and the suit is a letter:
+    Heart (H)
+    Spades (S)
+    Club (C)
+    Diamond (D)'''
+    numbers=list(range(2,15))
+    suits = ['H','S','C','D']
+    deck = []
+    for number in numbers:
+        for suit in suits:
+            card = suit+str(number)
+            deck.append(card)
+    return deck
+
+
+def shuffle_deck(cards_being_shuffled: list) -> list[str]:
+    '''Given a list, returns the list in a random order.'''
+    random.shuffle(cards_being_shuffled)
+    return cards_being_shuffled
+
+
+def draw_cards(deck: list, draw_number: int) -> tuple[list[str], list[str]]:
+    '''Draws cards from the deck provided. Returns hand and remaining deck '''
+    cards_drawn = []
+    i = 0
+    while i < draw_number:
+        cards_drawn.append(deck.pop(0))
+        i += 1
+    return cards_drawn, deck
+
+
+def create_hand(deck: list) -> tuple[list[str], list[str]]:
+    '''
+    Provided a deck, shuffles, and creates a hand.
+    Returns a tuple, (Hand,Remaining Deck)
+    '''
+    deck = build_deck()
+    deck = shuffle_deck(deck)
+    return draw_cards(deck,5)
+
+
+def score_four_of_a_kind(numbers: list) -> int:
+    '''Evaluates a int list to determine the score of quads - does not check the hand'''
+    for i in numbers:
+        if numbers.count(i) == 4:
+            four_of_a_kind = i
+        elif numbers.count(i) == 1:
+            card = i
+    return 105 + four_of_a_kind + card/100
+
+
+def score_full_house(numbers: list) -> int:
+    '''Evaluates a int list to determine the score of a full house - does not check the hand'''
+    for i in numbers:
+        if numbers.count(i) == 3:
+            trips = i
+        elif numbers.count(i) == 2:
+            pair = i
+    return 90 + trips + pair/100
+
+
+def score_three_of_a_kind(numbers: list) -> int:
+    '''Evaluates a int list to determine the score of a three of a kind - does not check the hand'''
+    trips = 0
+    cards = []
+    for i in numbers:
+        if numbers.count(i) == 3:
+            trips = i
+        else:
+            cards.append(i)
+    return 45 + trips
+
+
+def score_two_pair(numbers: list) -> int:
+    '''Evaluates a int list to determine the score of a two pair hand - does not check the hand'''
+    pairs = []
+    cards = []
+    for i in numbers:
+        if numbers.count(i) == 2:
+            pairs.append(i)
+        elif numbers.count(i) == 1:
+            cards.append(i)
+            cards = sorted(cards,reverse=True)
+    return 30 + max(pairs) + min(pairs)/100 + cards[0]/1000
+
+
+def score_pair(numbers: list) -> int:
+    '''Evaluates a int list to determine the score of a pair - does not check the hand'''
+    pair = []
+    cards  = []
+    for i in numbers:
+        if numbers.count(i) == 2:
+            pair.append(i)
+        elif numbers.count(i) == 1:
+            cards.append(i)
+            cards = sorted(cards,reverse=True)
+    return 15 + pair[0] + cards[0]/100 + cards[1]/1000 + cards[2]/10000
+
+
+def score_hand(hand: list) -> int:
+    ''' Given a hand in ['5H','3H','5C','5D','C14'] format return the poker score.
+
+    Scoring Table:
+    	                MIN	MAX
+        Royal Flush	    135	135
+        Straight Flush	120	134
+        Four of a Kind	105	119
+        Full House	    90	104
+        Flush	        75	89
+        Straight	    60	74
+        Three of a Kind	45	59
+        Two Pair        30	44
+        Pair	        15	29
+        High Card	     0	14
+    
+    Scoring for each hand has ranges to allow for payouts of different types four of a kinds.
+    '''
+    letters = [hand[i][:1] for i in range(5)] # We get the suit for each card in the hand
+    repeat_suit = [letters.count(i) for i in letters]  # We count repetitions for each suit ex [5,5,5,5,5] for flush
+
+    numbers = [int(hand[i][1:]) for i in range(5)]  # We get the number for each card in the hand
+    repeat_number = [numbers.count(i) for i in numbers] # We create a list with the repetitions of each number ex) [2,2,3,3,3] for fullhouse
+
+    dif = max(numbers) - min(numbers) # The difference between the greater and smallest number
+    handtype = 'Hand Ranking'
+    score = 0
+
+    #If all cards in hand share a suit, evaluate the type of flush.
+    if 5 in repeat_suit:
+        if numbers ==[14,13,12,11,10]:
+            handtype = 'ROYAL FLUSH'
+            score = 135
+            print(f'this hand is a {handtype}: with score: {score}')
+        elif dif == 4 and max(repeat_number) == 1:
+            handtype = 'STRAIGHT FLUSH'
+            score = 120 + max(numbers)
+            print(f'this hand is a {handtype}: with score: {score}')
+        else:
+            handtype = 'FLUSH'
+            score = 75 + max(numbers)
+            print(f'this hand is a {handtype}: with score: {score}')
+
+    #Evaluate other hands in decending ranking
+    elif 4 in repeat_number:
+        handtype = 'FOUR OF A KIND'
+        score = score_four_of_a_kind(numbers)
+        print(f'this hand is a {handtype}: with score: {score}')
+    elif sorted(repeat_number) == [2,2,3,3,3]:
+        handtype = 'FULL HOUSE'
+        score = score_full_house(numbers)
+        print(f'this hand is a {handtype}: with score: {score}')
+    elif dif == 4 and max(repeat_number) == 1:
+        handtype = 'STRAIGHT'
+        score = 60 + max(numbers)
+        print(f'this hand is a {handtype}: with score: {score}')
+    elif 3 in repeat_number:
+        handtype = 'TRIPS'
+        score = score_three_of_a_kind(numbers)
+        print(f'this hand is a {handtype}: with score: {score}')
+    elif repeat_number.count(2) == 4:
+        handtype = 'TWO PAIR'
+        score = score_two_pair(numbers)
+        print(f'this hand is a {handtype}: with score: {score}')
+    elif repeat_number.count(2) == 2:
+        handtype = 'PAIR'
+        score = score_pair(numbers)
+        print(f'this hand is a {handtype}: with score: {score}')
+    else:
+        handtype= 'HIGH CARD'
+        num = sorted(numbers,reverse=True)
+        score = num[0] + num[1]/100 + num[2]/1000 + num[3]/10000 + num[4]/100000
+        print(f'this hand is a {handtype}: with score: {score}')
+    return score, handtype
+
+
+def calculate_payout(input_score: int, input_credits: int) -> int:
+    '''Takes a score and number of paid credits, returns payout
+    
+    input_score = Accepts a number between 5 and 135.
+    input_credits = Accepts a number between 0 and 4.
+    '''
+    score_dict = {
+        'royal_flush': {'payout': [250,500,750,1000,4000]},
+        'straight_flush': {'payout': [50,100,150,200,250]},
+        'quad_aces_234_kicker': {'payout': [400,800,1200,1600,2000]},
+        'quad_aces_jackqueenking_kicker': {'payout': [320,640,960,1280,1600]},
+        'quad_234_ace_kicker': {'payout': [160,320,480,640,800]},
+        'quad_jackqueenking_face_kicker': {'payout': [160,320,480,640,800]},
+        'quad_aces': {'payout': [160,320,480,640,800]},
+        'quad_234': {'payout': [80,160,240,320,400]},
+        'quad_5toking': {'payout': [50,100,150,200,250]},
+        'full_house': {'payout': [7,14,21,28,35]},
+        'flush': {'payout': [5,10,15,25,25]},
+        'straight': {'payout': [4,8,12,16,20]},
+        'trips': {'payout': [3,6,9,12,15]},
+        'two_pair': {'payout': [1,2,3,4,5]},
+        'pair_jacks_better': {'payout': [1,2,3,4,5]}
+    }
+
+    if input_score == 135:
+        return score_dict['royal_flush']['payout'][input_credits]
+
+    elif input_score > 120:
+        return score_dict['straight_flush']['payout'][input_credits]
+
+    elif input_score > 119.10:
+        return score_dict['quad_aces_jackqueenking_kicker']['payout'][input_credits]
+
+    elif input_score > 119.4:
+        return score_dict['quad_aces']['payout'][input_credits]
+
+    elif input_score > 119.0:
+        return score_dict['quad_jackqueenking_face_kicker']['payout'][input_credits]
+
+    elif input_score > 110.0:
+        return score_dict['quad_5toking']['payout'][input_credits]
+    
+    elif input_score == 106.14 or input_score == 107.14 or input_score == 108.14:
+        return score_dict['quad_234_ace_kicker']['payout'][input_credits]
+
+    elif input_score > 107.0:
+        return score_dict['quad_234']['payout'][input_credits]
+
+    elif input_score > 90:
+        return score_dict['full_house']['payout'][input_credits]
+
+    elif input_score > 89.00:
+        return score_dict['flush']['payout'][input_credits]
+
+    elif input_score > 70.00:
+        return score_dict['straight']['payout'][input_credits]
+
+    elif input_score > 51:
+        return score_dict['trips']['payout'][input_credits]
+
+    elif input_score > 30:
+        return score_dict['two_pair']['payout'][input_credits]
+
+    elif input_score > 26:
+        return score_dict['pair_jacks_better']['payout'][input_credits]
+
+    else:
+        #Hand does not meet minimum payout
+        return 0
+
+
+def load_player_balance(bank_file_location = os.path.dirname(os.path.realpath(__file__))) -> int:
+    '''Load the player balance from bank.txt'''
+    bank_store_path = os.path.join(bank_file_location, 'fcd_bank.txt' )
+    bank_store = open(bank_store_path, 'r', encoding = 'utf-8')
+    return int(bank_store.read())
```

### Comparing `five_card_draw-1.0.8/five_card_draw/fcd_pagegui.py` & `five_card_draw-1.1.0/five_card_draw/fcd_pagegui.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,367 +1,367 @@
-'''Module ran to start the program, Poker: 5 Card Redraw'''
-import sys
-import os.path
-import tkinter as tk
-from five_card_draw import poker_start, fcd_functions
-
-local_file_directory = os.path.dirname(os.path.realpath(__file__))
-asset_file_directory = os.path.join(local_file_directory + '\data')
-
-def vp_start_gui():
-    '''Starting point when module is the main routine.'''
-    global root
-    global prog_location
-    prog_call = sys.argv[0]
-    prog_location = os.path.split(prog_call)[0]
-    root = tk.Tk()
-    top = Credits (root)
-    poker_start.init(root, top)
-    root.mainloop()
-
-
-class Credits:
-    '''Class containing the GUI interface.'''
-    def __init__(self, top=None):
-        '''This class configures and populates the toplevel window.
-        top is the toplevel containing window.
-        All other window objects are initialized and defined here.
-        '''
-        #Initializing runtime values
-        self.bet_amount = 0
-        self.status_deal_button = True #Start state as "new hand"
-        self.card_hold_status = [False, False, False, False, False] #cards start unheld.
-        self.player_hand = []
-        self.deck = []
-        self.player_money = fcd_functions.load_player_balance()
-
-        _bgcolor = '#d9d9d9'
-        _fgcolor = '#000000'
-
-        #This Section controls the game window name and color
-        top.geometry("1920x1080")
-        top.minsize(1800, 1080)
-        top.maxsize(1800, 1080)
-        top.resizable(1,  1)
-        top.title("5 Card Draw")
-        top.configure(
-            background="#00008b",
-            highlightbackground="#d9d9d9",
-            highlightcolor="black"
-        )
-
-        #global card image
-        default_card_back_file = os.path.join(asset_file_directory + '\cardBack.png')
-        default_card_back_file = tk.PhotoImage(file=default_card_back_file)
-
-        #Initialize the bottom center display the number of winnings
-        self.player_winnings_display = tk.Message(top)
-        self.player_winnings_display.place(relx=0.000, rely=0.905, relheight=0.093, relwidth=0.178)
-        self.player_winnings_display.config(font=("Courier Bold", 55))
-        self.player_winnings_display.configure(
-            background="#00008b",
-            foreground="#cc3300",
-            highlightbackground="#d9d9d9",
-            highlightcolor="black",
-            text='''Winnings''',
-            width=342
-        )
-
-        #Initialize display for current credits
-        self.player_credits = tk.Message(top)
-        self.player_credits.place(relx=0.742, rely=0.920, relheight=0.050, relwidth=0.250)
-        self.player_credits.config(font=("Courier", 44))
-        self.player_credits.configure(background="#00008b",
-            foreground="#cc3300",
-            highlightbackground="#d9d9d9",
-            highlightcolor="black",
-            text='CREDITS',
-            width=550
-        )
-
-        #Initialize the banner image at the top
-        self.banner = tk.Button(top)
-        self.banner.place(relx=0.000, rely=0.000, height=400, width=1800)
-        banner_image = os.path.join(asset_file_directory + '\ScoringImage.png')
-        banner_image = tk.PhotoImage(file=banner_image)
-        self.banner.configure(
-            activebackground="#ececec",
-            activeforeground="#000000",
-            background="#d9d9d9",
-            disabledforeground="#a3a3a3",
-            foreground="#000000",
-            highlightbackground="#d9d9d9",
-            highlightcolor="black",
-            image=banner_image,
-            pady="0",
-            text='''Button'''
-        )
-        self.banner.image = banner_image
-
-        self.menubar = tk.Menu(top,font="TkMenuFont",bg=_bgcolor,fg=_fgcolor)
-        top.configure(menu = self.menubar)
-
-        #Initialize the 1 through 5 "hold" toggle displays
-        self.hold_button_1 = tk.Message(top)
-        self.hold_button_1.place(relx=0.112, rely=0.410, relheight=0.024, relwidth=0.026)
-        self.hold_button_2 = tk.Message(top)
-        self.hold_button_2.place(relx=0.292, rely=0.410, relheight=0.025, relwidth=0.026)
-        self.hold_button_3 = tk.Message(top)
-        self.hold_button_3.place(relx=0.480, rely=0.410, relheight=0.025, relwidth=0.026)
-        self.hold_button_4 = tk.Message(top)
-        self.hold_button_4.place(relx=0.667, rely=0.410, relheight=0.025, relwidth=0.026)
-        self.hold_button_5 = tk.Message(top)
-        self.hold_button_5.place(relx=0.865, rely=0.410, relheight=0.025, relwidth=0.026)
-
-        hold_objects = [self.hold_button_1, self.hold_button_2, self.hold_button_3, self.hold_button_4, self.hold_button_5]
-        for index, hold_object in enumerate(hold_objects):
-            hold_object.configure(
-                background="#00008b",
-                foreground="#000000",
-                highlightbackground="#d9d9d9",
-                highlightcolor="black",
-                text=''' ''',
-            )
-            hold_object.Image = default_card_back_file
-
-        #Intialize card 1 through 5, left to right
-        self.card_one = tk.Button(top)
-        self.card_one.place(relx=0.014, rely=0.430, height=508, width=350)
-        self.card_two = tk.Button(top)
-        self.card_two.place(relx=0.209, rely=0.430, height=508, width=350)
-        self.card_three = tk.Button(top)
-        self.card_three.place(relx=0.404, rely=0.430, height=508, width=350)
-        self.card_four = tk.Button(top)
-        self.card_four.place(relx=0.599, rely=0.430, height=508, width=350)
-        self.card_five = tk.Button(top)
-        self.card_five.place(relx=0.794, rely=0.430, height=508, width=350)
-
-        card_objects = [self.card_one, self.card_two, self.card_three, self.card_four, self.card_five]
-        for index, card_object in enumerate(card_objects):
-            card_object.configure(
-            activebackground="#ececec",
-            activeforeground="#000000",
-            background="#00008b",
-            disabledforeground="#a3a3a3",
-            foreground="#000000",
-            highlightbackground="#d9d9d9",
-            highlightcolor="black",
-            image=default_card_back_file,
-            pady="0",
-            command=lambda card_count = index + 1: self.toggle_card_hold(card_count),
-            text='''Button'''
-        )
-            card_object.Image = default_card_back_file
-
-        #Initialize the bet_one button
-        self.bet_one_button = tk.Button(top)
-        self.bet_one_button.place(relx=0.180, rely=0.905, height=90, width=230)
-        self.bet_one_button.config(font=("Courier Bold", 38))
-        self.bet_one_button.configure(
-            activebackground="#ececec",
-            activeforeground="#000000",
-            background="#E7E72B",
-            disabledforeground="#a3a3a3",
-            foreground="#000000",
-            highlightbackground="#d9d9d9",
-            highlightcolor="black",
-            pady="0",
-            text='''BET ONE''',
-            command=self.bet_one_command
-        )
-
-        #Initialize the bet_max button
-        self.bet_max_button = tk.Button(top)
-        self.bet_max_button.place(relx=0.310, rely=0.905, height=90, width=230)
-        self.bet_max_button.config(font=("Courier Bold", 38))
-        self.bet_max_button.configure(
-            activebackground="#ececec",
-            activeforeground="#000000",
-            background="#E7E72B",
-            disabledforeground="#a3a3a3",
-            foreground="#000000",
-            highlightbackground="#d9d9d9",
-            highlightcolor="black",
-            pady="0",
-            text='''BET MAX''',
-            command=self.bet_max_command
-        )
-
-        #Initialize the current bet display
-        self.current_bet = tk.Message(top)
-        self.current_bet.place(relx=0.450, rely=0.905, relheight=0.09, relwidth=0.100)
-        self.current_bet.config(font=("Courier Bold", 100))
-        self.current_bet.configure(
-            background="#00008b",
-            foreground="#cc3300",
-            highlightbackground="#d9d9d9",
-            highlightcolor="black",
-            text='''1''',
-            width=342
-        )
-
-        #initialize the deal and redraw button
-        self.deal_button = tk.Button(top)
-        self.deal_button.place(relx=0.615, rely=0.905, height=90, width=250)
-        self.deal_button.config(font=("Courier Bold", 40))
-        self.deal_button.configure(
-            activebackground="#ececec",
-            activeforeground="#000000",
-            background="#E7E72B",
-            disabledforeground="#a3a3a3",
-            foreground="#000000",
-            highlightbackground="#d9d9d9",
-            highlightcolor="black",
-            pady="0",
-            text='''DEAL''',
-            command=self.deal_command
-        )
-
-        #Initialize winning Hand banner in top center
-        self.winning_hand = tk.Message(top)
-        self.winning_hand.place(relx=0.350, rely=0.370, relheight=0.045, relwidth=0.300)
-        self.winning_hand.config(font=("Courier Bold", 44))
-        self.winning_hand.configure(
-            background="#E7E72B",
-            foreground="#000000", #000000 #cc3300"
-            text='''Hand Rank''',
-            width=600
-        )
-
-        #Intial update of images into client
-        root.update_idletasks()
-
-
-    def deal_command(self):
-        '''Function progressing state of the hand.
-        Alternates between redrawing cards or starting a new hand, and starting scoring.'''
-        print(f' Player Hand: {self.player_hand}')
-
-        #This list is used to update the card images for both redrawing and starting new hands.
-        card_list = [self.card_one, self.card_two, self.card_three, self.card_four, self.card_five]
-
-        if self.status_deal_button:
-            print("Starting New Hand")
-            #Creating player hand and clearing previous winning hand rank and winnings.
-            self.player_hand, self.deck = fcd_functions.create_hand(self.deck)
-            self.winning_hand.configure(text='', background="#00008b")
-            self.player_winnings_display.configure(text='')
-
-            #Subract Bet Amount
-            self.player_money = self.player_money - (self.bet_amount + 1)
-            self.player_credits.configure(text=f'{self.player_money} CREDITS')
-
-            #Updating the image of all cards in hand
-            for index, card in enumerate(self.player_hand):
-                new_card_file = (os.path.join(asset_file_directory, card)) + '.png'
-                new_card_image = tk.PhotoImage(file = new_card_file)
-                card_list[index].configure(image = new_card_image)
-                card_list[index].image = new_card_image
-
-            #change the redraw / new hand button to redraw
-            self.status_deal_button = False
-            self.deal_button.configure(text='''REDRAW''')
-            root.update_idletasks()
-
-        else:
-            #This phase redraws cards and immediately scores the redrawn cards.
-            print("Redrawing unheld cards")
-
-            #Drawing new cards for each held card and updating their images.
-            for index, card_hold_status in enumerate(self.card_hold_status):
-                if card_hold_status is False:
-                    new_card, self.deck = fcd_functions.draw_cards(self.deck, 1)
-                    new_card = ''.join(new_card)
-                    self.player_hand[index] = new_card
-                    new_card_file = os.path.join(asset_file_directory, new_card) + '.png'
-                    new_card_file = tk.PhotoImage(file=new_card_file)
-                    card_list[index].configure(image=new_card_file)
-                    card_list[index].Image = new_card_file
-                    root.update_idletasks()
-
-            #Display the hand ranking and associated score
-            hand_score, hand_type = fcd_functions.score_hand(self.player_hand)
-            self.winning_hand.configure(text=hand_type, background="#E7E72B")
-
-            #Calculate and Display Winnings
-            hand_winnings = fcd_functions.calculate_payout(hand_score, self.bet_amount)
-            self.player_winnings_display.configure(text=f"WIN   {hand_winnings}")
-            print(f'Player won ${hand_winnings}')
-
-            #Provide playout to player balance and update player credit balance
-            self.player_money = self.player_money + hand_winnings
-            self.player_credits.configure(text=f'{self.player_money} CREDITS')
-
-            #Update state to start new hand.
-            self.deal_button.configure(text='''DEAL''')
-            self.status_deal_button = True
-
-            #Resetting Holds displays and back end values
-            hold_buttons = [self.hold_button_1, self.hold_button_2, self.hold_button_3, self.hold_button_4, self.hold_button_5]
-            for hold_button in hold_buttons:
-                hold_button.configure(
-                    background="#00008b",
-                    foreground="#000000",
-                    highlightbackground="#d9d9d9",
-                    highlightcolor="black",
-                    text=''' '''
-                )
-            self.card_hold_status = [False,False,False,False,False]
-
-
-    def toggle_card_hold(self, card: int) -> None:
-        '''Toggles the hold or redrawing of a card in hand.'''
-        hold_buttons = [self.hold_button_1, self.hold_button_2, self.hold_button_3, self.hold_button_4, self.hold_button_5]
-
-        #If card is held, then toggle to false or vice versa. Update UI visual to match.
-        if self.status_deal_button is not True:
-            if self.card_hold_status[card-1]:
-                self.card_hold_status[card-1] = False
-                hold_buttons[card-1].configure(
-                    background="#00008b",
-                    foreground="#000000",
-                    highlightbackground="#d9d9d9",
-                    highlightcolor="black",
-                    text=''' '''
-                )
-
-            else:
-                self.card_hold_status[card-1] = True
-                hold_buttons[card-1].configure(
-                    background="#ff0000",
-                    foreground="#000000",
-                    highlightbackground="#d9d9d9",
-                    highlightcolor="black",
-                    text='''Held'''
-                )
-        root.update_idletasks()
-
-
-    def bet_max_command(self):
-        '''Sets the bet to the maximum. Bet amount is 4 since we start at 0.'''
-        print("Bet Max Button")
-
-        #Disallow changing bet mid hand by checking status_deal_button
-        if self.status_deal_button:
-            self.bet_amount = 4
-            self.current_bet.configure(text='''5''')
-        root.update_idletasks()
-
-
-    def bet_one_command(self):
-        '''Increments bet by one, starting at 0. Bet amount resets to 0 if incremented beyond 4.'''
-        print("Bet One Button")
-
-        #Disallow changing bet mid hand by checking status_deal_button
-        if self.status_deal_button:
-            if self.bet_amount == 4:
-                self.bet_amount = 0
-                self.current_bet.configure(text='''1''')
-            else:
-                self.bet_amount += 1
-                self.current_bet.configure(text=self.bet_amount + 1)
-        root.update_idletasks()
-
-
-if __name__ == '__main__':
-    '''Starts the GUI and begin the program.'''
-    vp_start_gui()
+'''Module ran to start the program, Poker: 5 Card Redraw'''
+import sys
+import os.path
+import tkinter as tk
+from five_card_draw import poker_start, fcd_functions
+
+local_file_directory = os.path.dirname(os.path.realpath(__file__))
+asset_file_directory = os.path.join(local_file_directory + '\data')
+
+def vp_start_gui():
+    '''Starting point when module is the main routine.'''
+    global root
+    global prog_location
+    prog_call = sys.argv[0]
+    prog_location = os.path.split(prog_call)[0]
+    root = tk.Tk()
+    top = Credits (root)
+    poker_start.init(root, top)
+    root.mainloop()
+
+
+class Credits:
+    '''Class containing the GUI interface.'''
+    def __init__(self, top=None):
+        '''This class configures and populates the toplevel window.
+        top is the toplevel containing window.
+        All other window objects are initialized and defined here.
+        '''
+        #Initializing runtime values
+        self.bet_amount = 0
+        self.status_deal_button = True #Start state as "new hand"
+        self.card_hold_status = [False, False, False, False, False] #cards start unheld.
+        self.player_hand = []
+        self.deck = []
+        self.player_money = fcd_functions.load_player_balance()
+
+        _bgcolor = '#d9d9d9'
+        _fgcolor = '#000000'
+
+        #This Section controls the game window name and color
+        top.geometry("1920x1080")
+        top.minsize(1800, 1080)
+        top.maxsize(1800, 1080)
+        top.resizable(1,  1)
+        top.title("5 Card Draw")
+        top.configure(
+            background="#00008b",
+            highlightbackground="#d9d9d9",
+            highlightcolor="black"
+        )
+
+        #global card image
+        default_card_back_file = os.path.join(asset_file_directory + '\cardBack.png')
+        default_card_back_file = tk.PhotoImage(file=default_card_back_file)
+
+        #Initialize the bottom center display the number of winnings
+        self.player_winnings_display = tk.Message(top)
+        self.player_winnings_display.place(relx=0.000, rely=0.905, relheight=0.093, relwidth=0.178)
+        self.player_winnings_display.config(font=("Courier Bold", 55))
+        self.player_winnings_display.configure(
+            background="#00008b",
+            foreground="#cc3300",
+            highlightbackground="#d9d9d9",
+            highlightcolor="black",
+            text='''Winnings''',
+            width=342
+        )
+
+        #Initialize display for current credits
+        self.player_credits = tk.Message(top)
+        self.player_credits.place(relx=0.742, rely=0.920, relheight=0.050, relwidth=0.250)
+        self.player_credits.config(font=("Courier", 44))
+        self.player_credits.configure(background="#00008b",
+            foreground="#cc3300",
+            highlightbackground="#d9d9d9",
+            highlightcolor="black",
+            text='CREDITS',
+            width=550
+        )
+
+        #Initialize the banner image at the top
+        self.banner = tk.Button(top)
+        self.banner.place(relx=0.000, rely=0.000, height=400, width=1800)
+        banner_image = os.path.join(asset_file_directory + '\ScoringImage.png')
+        banner_image = tk.PhotoImage(file=banner_image)
+        self.banner.configure(
+            activebackground="#ececec",
+            activeforeground="#000000",
+            background="#d9d9d9",
+            disabledforeground="#a3a3a3",
+            foreground="#000000",
+            highlightbackground="#d9d9d9",
+            highlightcolor="black",
+            image=banner_image,
+            pady="0",
+            text='''Button'''
+        )
+        self.banner.image = banner_image
+
+        self.menubar = tk.Menu(top,font="TkMenuFont",bg=_bgcolor,fg=_fgcolor)
+        top.configure(menu = self.menubar)
+
+        #Initialize the 1 through 5 "hold" toggle displays
+        self.hold_button_1 = tk.Message(top)
+        self.hold_button_1.place(relx=0.112, rely=0.410, relheight=0.024, relwidth=0.026)
+        self.hold_button_2 = tk.Message(top)
+        self.hold_button_2.place(relx=0.292, rely=0.410, relheight=0.025, relwidth=0.026)
+        self.hold_button_3 = tk.Message(top)
+        self.hold_button_3.place(relx=0.480, rely=0.410, relheight=0.025, relwidth=0.026)
+        self.hold_button_4 = tk.Message(top)
+        self.hold_button_4.place(relx=0.667, rely=0.410, relheight=0.025, relwidth=0.026)
+        self.hold_button_5 = tk.Message(top)
+        self.hold_button_5.place(relx=0.865, rely=0.410, relheight=0.025, relwidth=0.026)
+
+        hold_objects = [self.hold_button_1, self.hold_button_2, self.hold_button_3, self.hold_button_4, self.hold_button_5]
+        for index, hold_object in enumerate(hold_objects):
+            hold_object.configure(
+                background="#00008b",
+                foreground="#000000",
+                highlightbackground="#d9d9d9",
+                highlightcolor="black",
+                text=''' ''',
+            )
+            hold_object.Image = default_card_back_file
+
+        #Intialize card 1 through 5, left to right
+        self.card_one = tk.Button(top)
+        self.card_one.place(relx=0.014, rely=0.430, height=508, width=350)
+        self.card_two = tk.Button(top)
+        self.card_two.place(relx=0.209, rely=0.430, height=508, width=350)
+        self.card_three = tk.Button(top)
+        self.card_three.place(relx=0.404, rely=0.430, height=508, width=350)
+        self.card_four = tk.Button(top)
+        self.card_four.place(relx=0.599, rely=0.430, height=508, width=350)
+        self.card_five = tk.Button(top)
+        self.card_five.place(relx=0.794, rely=0.430, height=508, width=350)
+
+        card_objects = [self.card_one, self.card_two, self.card_three, self.card_four, self.card_five]
+        for index, card_object in enumerate(card_objects):
+            card_object.configure(
+            activebackground="#ececec",
+            activeforeground="#000000",
+            background="#00008b",
+            disabledforeground="#a3a3a3",
+            foreground="#000000",
+            highlightbackground="#d9d9d9",
+            highlightcolor="black",
+            image=default_card_back_file,
+            pady="0",
+            command=lambda card_count = index + 1: self.toggle_card_hold(card_count),
+            text='''Button'''
+        )
+            card_object.Image = default_card_back_file
+
+        #Initialize the bet_one button
+        self.bet_one_button = tk.Button(top)
+        self.bet_one_button.place(relx=0.180, rely=0.905, height=90, width=230)
+        self.bet_one_button.config(font=("Courier Bold", 38))
+        self.bet_one_button.configure(
+            activebackground="#ececec",
+            activeforeground="#000000",
+            background="#E7E72B",
+            disabledforeground="#a3a3a3",
+            foreground="#000000",
+            highlightbackground="#d9d9d9",
+            highlightcolor="black",
+            pady="0",
+            text='''BET ONE''',
+            command=self.bet_one_command
+        )
+
+        #Initialize the bet_max button
+        self.bet_max_button = tk.Button(top)
+        self.bet_max_button.place(relx=0.310, rely=0.905, height=90, width=230)
+        self.bet_max_button.config(font=("Courier Bold", 38))
+        self.bet_max_button.configure(
+            activebackground="#ececec",
+            activeforeground="#000000",
+            background="#E7E72B",
+            disabledforeground="#a3a3a3",
+            foreground="#000000",
+            highlightbackground="#d9d9d9",
+            highlightcolor="black",
+            pady="0",
+            text='''BET MAX''',
+            command=self.bet_max_command
+        )
+
+        #Initialize the current bet display
+        self.current_bet = tk.Message(top)
+        self.current_bet.place(relx=0.450, rely=0.905, relheight=0.09, relwidth=0.100)
+        self.current_bet.config(font=("Courier Bold", 100))
+        self.current_bet.configure(
+            background="#00008b",
+            foreground="#cc3300",
+            highlightbackground="#d9d9d9",
+            highlightcolor="black",
+            text='''1''',
+            width=342
+        )
+
+        #initialize the deal and redraw button
+        self.deal_button = tk.Button(top)
+        self.deal_button.place(relx=0.615, rely=0.905, height=90, width=250)
+        self.deal_button.config(font=("Courier Bold", 40))
+        self.deal_button.configure(
+            activebackground="#ececec",
+            activeforeground="#000000",
+            background="#E7E72B",
+            disabledforeground="#a3a3a3",
+            foreground="#000000",
+            highlightbackground="#d9d9d9",
+            highlightcolor="black",
+            pady="0",
+            text='''DEAL''',
+            command=self.deal_command
+        )
+
+        #Initialize winning Hand banner in top center
+        self.winning_hand = tk.Message(top)
+        self.winning_hand.place(relx=0.350, rely=0.370, relheight=0.045, relwidth=0.300)
+        self.winning_hand.config(font=("Courier Bold", 44))
+        self.winning_hand.configure(
+            background="#E7E72B",
+            foreground="#000000", #000000 #cc3300"
+            text='''Hand Rank''',
+            width=600
+        )
+
+        #Intial update of images into client
+        root.update_idletasks()
+
+
+    def deal_command(self):
+        '''Function progressing state of the hand.
+        Alternates between redrawing cards or starting a new hand, and starting scoring.'''
+        print(f' Player Hand: {self.player_hand}')
+
+        #This list is used to update the card images for both redrawing and starting new hands.
+        card_list = [self.card_one, self.card_two, self.card_three, self.card_four, self.card_five]
+
+        if self.status_deal_button:
+            print("Starting New Hand")
+            #Creating player hand and clearing previous winning hand rank and winnings.
+            self.player_hand, self.deck = fcd_functions.create_hand(self.deck)
+            self.winning_hand.configure(text='', background="#00008b")
+            self.player_winnings_display.configure(text='')
+
+            #Subract Bet Amount
+            self.player_money = self.player_money - (self.bet_amount + 1)
+            self.player_credits.configure(text=f'{self.player_money} CREDITS')
+
+            #Updating the image of all cards in hand
+            for index, card in enumerate(self.player_hand):
+                new_card_file = (os.path.join(asset_file_directory, card)) + '.png'
+                new_card_image = tk.PhotoImage(file = new_card_file)
+                card_list[index].configure(image = new_card_image)
+                card_list[index].image = new_card_image
+
+            #change the redraw / new hand button to redraw
+            self.status_deal_button = False
+            self.deal_button.configure(text='''REDRAW''')
+            root.update_idletasks()
+
+        else:
+            #This phase redraws cards and immediately scores the redrawn cards.
+            print("Redrawing unheld cards")
+
+            #Drawing new cards for each held card and updating their images.
+            for index, card_hold_status in enumerate(self.card_hold_status):
+                if card_hold_status is False:
+                    new_card, self.deck = fcd_functions.draw_cards(self.deck, 1)
+                    new_card = ''.join(new_card)
+                    self.player_hand[index] = new_card
+                    new_card_file = os.path.join(asset_file_directory, new_card) + '.png'
+                    new_card_file = tk.PhotoImage(file=new_card_file)
+                    card_list[index].configure(image=new_card_file)
+                    card_list[index].Image = new_card_file
+                    root.update_idletasks()
+
+            #Display the hand ranking and associated score
+            hand_score, hand_type = fcd_functions.score_hand(self.player_hand)
+            self.winning_hand.configure(text=hand_type, background="#E7E72B")
+
+            #Calculate and Display Winnings
+            hand_winnings = fcd_functions.calculate_payout(hand_score, self.bet_amount)
+            self.player_winnings_display.configure(text=f"WIN   {hand_winnings}")
+            print(f'Player won ${hand_winnings}')
+
+            #Provide playout to player balance and update player credit balance
+            self.player_money = self.player_money + hand_winnings
+            self.player_credits.configure(text=f'{self.player_money} CREDITS')
+
+            #Update state to start new hand.
+            self.deal_button.configure(text='''DEAL''')
+            self.status_deal_button = True
+
+            #Resetting Holds displays and back end values
+            hold_buttons = [self.hold_button_1, self.hold_button_2, self.hold_button_3, self.hold_button_4, self.hold_button_5]
+            for hold_button in hold_buttons:
+                hold_button.configure(
+                    background="#00008b",
+                    foreground="#000000",
+                    highlightbackground="#d9d9d9",
+                    highlightcolor="black",
+                    text=''' '''
+                )
+            self.card_hold_status = [False,False,False,False,False]
+
+
+    def toggle_card_hold(self, card: int) -> None:
+        '''Toggles the hold or redrawing of a card in hand.'''
+        hold_buttons = [self.hold_button_1, self.hold_button_2, self.hold_button_3, self.hold_button_4, self.hold_button_5]
+
+        #If card is held, then toggle to false or vice versa. Update UI visual to match.
+        if self.status_deal_button is not True:
+            if self.card_hold_status[card-1]:
+                self.card_hold_status[card-1] = False
+                hold_buttons[card-1].configure(
+                    background="#00008b",
+                    foreground="#000000",
+                    highlightbackground="#d9d9d9",
+                    highlightcolor="black",
+                    text=''' '''
+                )
+
+            else:
+                self.card_hold_status[card-1] = True
+                hold_buttons[card-1].configure(
+                    background="#ff0000",
+                    foreground="#000000",
+                    highlightbackground="#d9d9d9",
+                    highlightcolor="black",
+                    text='''Held'''
+                )
+        root.update_idletasks()
+
+
+    def bet_max_command(self):
+        '''Sets the bet to the maximum. Bet amount is 4 since we start at 0.'''
+        print("Bet Max Button")
+
+        #Disallow changing bet mid hand by checking status_deal_button
+        if self.status_deal_button:
+            self.bet_amount = 4
+            self.current_bet.configure(text='''5''')
+        root.update_idletasks()
+
+
+    def bet_one_command(self):
+        '''Increments bet by one, starting at 0. Bet amount resets to 0 if incremented beyond 4.'''
+        print("Bet One Button")
+
+        #Disallow changing bet mid hand by checking status_deal_button
+        if self.status_deal_button:
+            if self.bet_amount == 4:
+                self.bet_amount = 0
+                self.current_bet.configure(text='''1''')
+            else:
+                self.bet_amount += 1
+                self.current_bet.configure(text=self.bet_amount + 1)
+        root.update_idletasks()
+
+
+if __name__ == '__main__':
+    '''Starts the GUI and begin the program.'''
+    vp_start_gui()
```

### Comparing `five_card_draw-1.0.8/five_card_draw.egg-info/PKG-INFO` & `five_card_draw-1.1.0/five_card_draw.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-Metadata-Version: 2.1
-Name: five-card-draw
-Version: 1.0.8
-Summary: 5 Card Draw Video Poker application
-Home-page: https://github.com/ralbee1/5_card_draw
-Author: Richard Albee
-Author-email: Ralbee1@iwu.edu
-License: LICENSE.txt
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-<a name="readme-top"></a>
-
-<!-- VideoPoker-5CardRedraw -->
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-[![LinkedIn][linkedin-shield]][linkedin-url]
-
-
-<!-- PROJECT LOGO -->
-<br />
-<div align="center">
-  <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw">
-    <img src="documentation/logo.png" alt="Logo" width="80" height="80">
-  </a>
-
-<h3 align="center">VideoPoker-5CardRedraw</h3>
-
-  <p align="center">
-    A pythonic creation of a 5 card redraw video poker.
-    <br />
-    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
-    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw">View Demo</a>
-    ·
-    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw/issues">Report Bug</a>
-    ·
-    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw/issues">Request Feature</a>
-  </p>
-</div>
-
-
-
-<!-- TABLE OF CONTENTS -->
-<details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li>
-      <a href="#about-the-project">About The Project</a>
-      <ul>
-        <li><a href="#built-with">Built With</a></li>
-        <li><a href="#Features">Features</a></li>
-      </ul>
-    </li>
-    <li>
-      <a href="#getting-started">Getting Started</a>
-      <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
-        <li><a href="#installation">Installation</a></li>
-      </ul>
-    </li>
-    <li><a href="#usage">Usage</a></li>
-    <li><a href="#contact">Contact</a></li>
-    <li><a href="#acknowledgments">Acknowledgments</a></li>
-  </ol>
-</details>
-
-
-<!-- ABOUT THE PROJECT -->
-## About The Project
-<!-- 
-[![Product Name Screen Shot][product-screenshot]](https://example.com)
--->
-5 Card Draw is a playable Python 5 card draw poker application. This project served as a hands-on Python learning experience in 2021. On my journey, I learned about creating graphical user interfaces in python, pythonic best practices, CI/CD workflows, PyPi deployments, and much more. The beautiful learning opportunity provided this project was balancing desired learning opportunities and refining 5 Card Draw into a polished application. This project is currently archived with the last remaining features involved further polishing the UI/UX experience, adding sound, and cashing out player credits. If I were to start over, I'd rank poker hands with a symantic system over a integer score.
- 
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-### Features
-
-- [ ] **5 Card Redraw**
-  - [ ] Modular Hand Ranking and Scoring
-  - [ ] Player Hand and Deck creation
-  - [ ] Playable GUI interface
-  - [ ] Bank text file
-- [ ] **PyPi Installs**
-- [ ] **Pep 8 Standards**
-- [ ] **GitHub CI/CD Pipelines**
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-<!-- GETTING STARTED -->
-## Getting Started
-
-The following is an guide for running 5 card redraw poker locally.
-
-### Prerequisites
-
-1. [Python 3.10.8 or Newer](https://www.python.org/downloads/release/python-3108/)
-
-
-### Installation
-
-Local Repo Install:
-<br/>
-Summary: The developer install is for those who want to contribute to or clone VideoPoker-5CardRedraw.
-1. Clone the repo (or use Github Desktop)
-   ```sh
-   git clone https://github.com/ralbee1/5_card_draw.git
-   ```
-2. Open the CLI and navigate the current working directory to where you cloned VideoPoker-5CardDraw
-3. Install the Pip Package from the CLI, copy and run this command:
-   ```sh
-   py -m pip install -e .
-   ```
-<br/>
-<br/>
-User Install
-<br/>
-1. Automatic User Install from the Command line via PyPi.
-   ```sh
-   pip install five-card-draw
-   ```
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-<!-- USAGE EXAMPLES -->
-## Usage / How to Play
-If your python files open with Python by default then from the commmand line run:
-
-  ```js
-  poker_start.py;
-  ```
-
-Troubleshooting:
-1. "'poker_start.py' is not recognized as an internal or external command, operable program or batch file."
-  Your terminal needs to be able to find the file. For windows, you need to ensure your python "script" folder is in your path variable
-  For example: C:\Users\{username}\AppData\Roaming\Python\{pythonversion}\Scripts
-  You may also navigate to where the pip was installed and run poker_start.py with python manually.
-
-The game is played by aiming to make the best poker hand possible. The top of the interface shows the hand ranking and the payouts sorted by how many credits you bet per round, 1 thru 5. To begin, click DEAL. You hold cards with the intent of keeping them and drawing new cards to try to improve your hand ranking. After drawing new cards, your hand is automatically scored and profits are payed out. You may then click "DEAL" and start over.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-<!-- CONTACT -->
-## Contact
-
-* []()Email - ralbee1@iwu.edu
-* []()Project Link: [https://github.com/ralbee1/VideoPoker-5CardRedraw](https://github.com/ralbee1/VideoPoker-5CardRedraw)
-
-
-
-<!-- ACKNOWLEDGMENTS -->
-## Acknowledgments
-
-* []() This variant of poker was inspired by Super Double Double as found in Las Vegas Casinos.
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[contributors-shield]: https://img.shields.io/github/contributors/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[contributors-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[forks-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/network/members
-[stars-shield]: https://img.shields.io/github/stars/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[stars-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/stargazers
-[issues-shield]: https://img.shields.io/github/issues/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[issues-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/issues
-[license-shield]: https://img.shields.io/github/license/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
-[license-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/blob/master/LICENSE.txt
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
-[linkedin-url]: https://linkedin.com/in/Richard-Albee
-[product-screenshot]: images/screenshot.png
-[python.org]: https://www.python.org/static/img/python-logo.png
-[python-url]: https://www.python.org/
-[pypi.org]: https://pypi.org/static/images/logo-small.2a411bc6.svg
-[pypi-url]: https://pypi.org/project/pip/
+Metadata-Version: 2.1
+Name: five-card-draw
+Version: 1.1.0
+Summary: 5 Card Draw Video Poker application
+Home-page: https://github.com/ralbee1/5_card_draw
+Author: Richard Albee
+Author-email: Ralbee1@iwu.edu
+License: LICENSE.txt
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+<a name="readme-top"></a>
+
+<!-- VideoPoker-5CardRedraw -->
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+[![LinkedIn][linkedin-shield]][linkedin-url]
+
+
+<!-- PROJECT LOGO -->
+<br />
+<div align="center">
+  <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw">
+    <img src="documentation/logo.png" alt="Logo" width="80" height="80">
+  </a>
+
+<h3 align="center">VideoPoker-5CardRedraw</h3>
+
+  <p align="center">
+    A pythonic creation of a 5 card redraw video poker.
+    <br />
+    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw"><strong>Explore the docs »</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw">View Demo</a>
+    ·
+    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw/issues">Report Bug</a>
+    ·
+    <a href="https://github.com/ralbee1/VideoPoker-5CardRedraw/issues">Request Feature</a>
+  </p>
+</div>
+
+
+
+<!-- TABLE OF CONTENTS -->
+<details>
+  <summary>Table of Contents</summary>
+  <ol>
+    <li>
+      <a href="#about-the-project">About The Project</a>
+      <ul>
+        <li><a href="#built-with">Built With</a></li>
+        <li><a href="#Features">Features</a></li>
+      </ul>
+    </li>
+    <li>
+      <a href="#getting-started">Getting Started</a>
+      <ul>
+        <li><a href="#prerequisites">Prerequisites</a></li>
+        <li><a href="#installation">Installation</a></li>
+      </ul>
+    </li>
+    <li><a href="#usage">Usage</a></li>
+    <li><a href="#contact">Contact</a></li>
+    <li><a href="#acknowledgments">Acknowledgments</a></li>
+  </ol>
+</details>
+
+
+<!-- ABOUT THE PROJECT -->
+## About The Project
+<!-- 
+[![Product Name Screen Shot][product-screenshot]](https://example.com)
+-->
+5 Card Draw is a playable Python 5-card draw poker application. This project served as a hands-on Python learning experience in 2021. On my journey, I learned about creating graphical user interfaces in Python, pythonic best practices, CI/CD workflows, PyPi deployments, and much more. The beautiful learning opportunity this project provided was balancing desired learning opportunities and refining 5 Card Draw into a polished application. This project archived with the last remaining features involved in further polishing the UI/UX experience, adding sound, and cashing out player credits. If I were to start over, I'd rank poker hands with a semantic system over an integer score.
+ 
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+### Features
+
+- [ ] **5 Card Redraw**
+  - [ ] Modular Hand Ranking and Scoring
+  - [ ] Player Hand and Deck creation
+  - [ ] Playable GUI interface
+  - [ ] Bank text file
+- [ ] **PyPi Installs**
+- [ ] **Pep 8 Standards**
+- [ ] **GitHub CI/CD Pipelines**
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- GETTING STARTED -->
+## Getting Started
+
+The following is an guide for running 5 card redraw poker locally.
+
+### Prerequisites
+
+1. [Python 3.10.8 or Newer](https://www.python.org/downloads/release/python-3108/)
+
+
+### Installation
+
+Local Repo Install:
+<br/>
+Summary: The developer install is for those who want to contribute to or clone VideoPoker-5CardRedraw.
+1. Clone the repo (or use Github Desktop)
+   ```sh
+   git clone https://github.com/ralbee1/5_card_draw.git
+   ```
+2. Open the CLI and navigate the current working directory to where you cloned VideoPoker-5CardDraw
+3. Install the Pip Package from the CLI, copy and run this command:
+   ```sh
+   py -m pip install -e .
+   ```
+<br/>
+<br/>
+User Install
+<br/>
+1. Automatic User Install from the Command line via PyPi.
+   ```sh
+   pip install five-card-draw
+   ```
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+<!-- USAGE EXAMPLES -->
+## Usage / How to Play
+If your python files open with Python by default then from the commmand line run:
+
+  ```js
+  poker_start.py;
+  ```
+
+Troubleshooting:
+1. "'poker_start.py' is not recognized as an internal or external command, operable program or batch file."
+  Your terminal needs to be able to find the file. For windows, you need to ensure your python "script" folder is in your path variable
+  For example: C:\Users\{username}\AppData\Roaming\Python\{pythonversion}\Scripts
+  You may also navigate to where the pip was installed and run poker_start.py with python manually.
+
+The game is played by aiming to make the best poker hand possible. The top of the interface shows the hand ranking and the payouts sorted by how many credits you bet per round, 1 thru 5. To begin, click DEAL. You hold cards with the intent of keeping them and drawing new cards to try to improve your hand ranking. After drawing new cards, your hand is automatically scored and profits paid out. You may then click "DEAL" and start over.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+<!-- CONTACT -->
+## Contact
+
+* []()Email - ralbee1@iwu.edu
+* []()Project Link: [https://github.com/ralbee1/VideoPoker-5CardRedraw](https://github.com/ralbee1/VideoPoker-5CardRedraw)
+
+
+
+<!-- ACKNOWLEDGMENTS -->
+## Acknowledgments
+
+* []() This variant of poker was inspired by Super Double Double as found in Las Vegas Casinos.
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[contributors-shield]: https://img.shields.io/github/contributors/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[contributors-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[forks-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/network/members
+[stars-shield]: https://img.shields.io/github/stars/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[stars-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/stargazers
+[issues-shield]: https://img.shields.io/github/issues/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[issues-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/issues
+[license-shield]: https://img.shields.io/github/license/ralbee1/VideoPoker-5CardRedraw.svg?style=for-the-badge
+[license-url]: https://github.com/ralbee1/VideoPoker-5CardRedraw/blob/master/LICENSE.txt
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+[linkedin-url]: https://linkedin.com/in/Richard-Albee
+[product-screenshot]: images/screenshot.png
+[python.org]: https://www.python.org/static/img/python-logo.png
+[python-url]: https://www.python.org/
+[pypi.org]: https://pypi.org/static/images/logo-small.2a411bc6.svg
+[pypi-url]: https://pypi.org/project/pip/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: five-card-draw Version: 1.0.8 Summary: 5 Card Draw
+Metadata-Version: 2.1 Name: five-card-draw Version: 1.1.0 Summary: 5 Card Draw
 Video Poker application Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee Author-email: Ralbee1@iwu.edu License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENSE.txt   [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
 [linkedin-shield]][linkedin-url]
@@ -18,24 +18,24 @@
           o Features
    2. Getting_Started
           o Prerequisites
           o Installation
    3. Usage
    4. Contact
    5. Acknowledgments
-  ## About The Project  5 Card Draw is a playable Python 5 card draw poker
+  ## About The Project  5 Card Draw is a playable Python 5-card draw poker
 application. This project served as a hands-on Python learning experience in
 2021. On my journey, I learned about creating graphical user interfaces in
-python, pythonic best practices, CI/CD workflows, PyPi deployments, and much
-more. The beautiful learning opportunity provided this project was balancing
+Python, pythonic best practices, CI/CD workflows, PyPi deployments, and much
+more. The beautiful learning opportunity this project provided was balancing
 desired learning opportunities and refining 5 Card Draw into a polished
-application. This project is currently archived with the last remaining
-features involved further polishing the UI/UX experience, adding sound, and
-cashing out player credits. If I were to start over, I'd rank poker hands with
-a symantic system over a integer score.
+application. This project archived with the last remaining features involved in
+further polishing the UI/UX experience, adding sound, and cashing out player
+credits. If I were to start over, I'd rank poker hands with a semantic system
+over an integer score.
                                                                   (back_to_top)
 ### Features - [ ] **5 Card Redraw** - [ ] Modular Hand Ranking and Scoring -
 [ ] Player Hand and Deck creation - [ ] Playable GUI interface - [ ] Bank text
 file - [ ] **PyPi Installs** - [ ] **Pep 8 Standards** - [ ] **GitHub CI/CD
 Pipelines**
                                                                   (back_to_top)
  ## Getting Started The following is an guide for running 5 card redraw poker
@@ -60,15 +60,15 @@
 path variable For example: C:\Users\{username}\AppData\Roaming\Python\
 {pythonversion}\Scripts You may also navigate to where the pip was installed
 and run poker_start.py with python manually. The game is played by aiming to
 make the best poker hand possible. The top of the interface shows the hand
 ranking and the payouts sorted by how many credits you bet per round, 1 thru 5.
 To begin, click DEAL. You hold cards with the intent of keeping them and
 drawing new cards to try to improve your hand ranking. After drawing new cards,
-your hand is automatically scored and profits are payed out. You may then click
+your hand is automatically scored and profits paid out. You may then click
 "DEAL" and start over.
                                                                   (back_to_top)
  ## Contact * []()Email - ralbee1@iwu.edu * []()Project Link: [https://
 github.com/ralbee1/VideoPoker-5CardRedraw](https://github.com/ralbee1/
 VideoPoker-5CardRedraw)  ## Acknowledgments * []() This variant of poker was
 inspired by Super Double Double as found in Las Vegas Casinos.
                                                                   (back_to_top)
```

### Comparing `five_card_draw-1.0.8/five_card_draw.egg-info/SOURCES.txt` & `five_card_draw-1.1.0/five_card_draw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.8/setup.py` & `five_card_draw-1.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-'''Setup file for building a pip for a module.
-
-Local Install Process:
-
-Build Pip Distributable: py -m build --wheel from the /PythonTools/ directory with this setup.py in it. Then install from the .whl file.
-INSTRUCTIONS FOR BUILDING A PIP https://pip.pypa.io/en/stable/cli/pip_wheel/
-OR
-Developer Install: "py -m pip install -e ." from this folder.
-
-Publish a Pip Version to PyPi:
-0. Create an account https://pypi.org/account/register/
-1. Install Prequisites: py -m pip install --upgrade pip setuptools wheel twine build
-2. py setup.py sdist bdist_wheel
-3. py -m twine upload dist/*
-
-
-setuptools reference guide: https://docs.python.org/3/distutils/setupscript.html#installing-package-data
-'''
-import os
-from pathlib import Path
-from distutils.core import setup
-
-required_dependencies = [
-    'tk',
-    'pathlib'
-]
-scripts = [
-    str(Path('five_card_draw','poker_start.py'))
-]
-
-#Using distutils.core over setuptools since package data was not specified correctly, needing the manifest.in file
-setup(
-    name = 'five_card_draw',
-    version = os.getenv('PACKAGE_VERSION', '1.0.8'),
-    author = 'Richard Albee',
-    author_email='Ralbee1@iwu.edu',
-    packages=['five_card_draw','five_card_draw.data'],
-    package_dir={'five_card_draw': 'five_card_draw'},
-    package_data={'five_card_draw': ['data/*.png','*.txt']},
-    scripts=scripts,
-    url = "https://github.com/ralbee1/5_card_draw",
-    license='LICENSE.txt',
-    description='5 Card Draw Video Poker application',
-    long_description_content_type = 'text/markdown',
-    long_description=open('README.md', encoding='utf-8').read(),
-    install_requires=required_dependencies
-)
+'''Setup file for building a pip for a module.
+
+Local Install Process:
+
+Build Pip Distributable: py -m build --wheel from the /PythonTools/ directory with this setup.py in it. Then install from the .whl file.
+INSTRUCTIONS FOR BUILDING A PIP https://pip.pypa.io/en/stable/cli/pip_wheel/
+OR
+Developer Install: "py -m pip install -e ." from this folder.
+
+Publish a Pip Version to PyPi:
+0. Create an account https://pypi.org/account/register/
+1. Install Prequisites: py -m pip install --upgrade pip setuptools wheel twine build
+2. py setup.py sdist bdist_wheel
+3. py -m twine upload dist/*
+
+
+setuptools reference guide: https://docs.python.org/3/distutils/setupscript.html#installing-package-data
+'''
+import os
+from pathlib import Path
+from distutils.core import setup
+
+required_dependencies = [
+    'tk',
+    'pathlib'
+]
+scripts = [
+    str(Path('five_card_draw','poker_start.py'))
+]
+
+#Using distutils.core over setuptools since package data was not specified correctly, needing the manifest.in file
+setup(
+    name = 'five_card_draw',
+    version = os.getenv('PACKAGE_VERSION', '1.1.0'),
+    author = 'Richard Albee',
+    author_email='Ralbee1@iwu.edu',
+    packages=['five_card_draw','five_card_draw.data'],
+    package_dir={'five_card_draw': 'five_card_draw'},
+    package_data={'five_card_draw': ['data/*.png','*.txt']},
+    scripts=scripts,
+    url = "https://github.com/ralbee1/5_card_draw",
+    license='LICENSE.txt',
+    description='5 Card Draw Video Poker application',
+    long_description_content_type = 'text/markdown',
+    long_description=open('README.md', encoding='utf-8').read(),
+    install_requires=required_dependencies
+)
```

