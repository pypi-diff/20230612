# Comparing `tmp/five_card_draw-1.0.6.tar.gz` & `tmp/five_card_draw-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five_card_draw-1.0.6.tar", last modified: Mon Jun 12 15:32:03 2023, max compression
+gzip compressed data, was "five_card_draw-1.0.7.tar", last modified: Mon Jun 12 15:46:01 2023, max compression
```

## Comparing `five_card_draw-1.0.6.tar` & `five_card_draw-1.0.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 15:32:03.887418 five_card_draw-1.0.6/
--rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       55 2023-06-12 13:48:00.000000 five_card_draw-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     6850 2023-06-12 15:32:03.886420 five_card_draw-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     6546 2023-06-12 15:13:40.000000 five_card_draw-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 15:32:03.809086 five_card_draw-1.0.6/five_card_draw.egg-info/
--rw-rw-rw-   0        0        0     6850 2023-06-12 15:32:03.000000 five_card_draw-1.0.6/five_card_draw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2155 2023-06-12 15:32:03.000000 five_card_draw-1.0.6/five_card_draw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 15:32:03.000000 five_card_draw-1.0.6/five_card_draw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 15:32:03.000000 five_card_draw-1.0.6/five_card_draw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-12 15:32:03.000000 five_card_draw-1.0.6/five_card_draw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 15:32:03.887418 five_card_draw-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1695 2023-06-12 15:31:35.000000 five_card_draw-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:32:03.793511 five_card_draw-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 15:32:03.819278 five_card_draw-1.0.6/src/five_card_draw/
-drwxrwxrwx   0        0        0        0 2023-06-12 15:32:03.885423 five_card_draw-1.0.6/src/five_card_draw/data/
--rw-rw-rw-   0        0        0    56484 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/C10.png
--rw-rw-rw-   0        0        0   187958 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/C11.png
--rw-rw-rw-   0        0        0   205820 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/C12.png
--rw-rw-rw-   0        0        0   189382 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C13.png
--rw-rw-rw-   0        0        0    37544 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C14.png
--rw-rw-rw-   0        0        0    23382 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C2.png
--rw-rw-rw-   0        0        0    29340 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C3.png
--rw-rw-rw-   0        0        0    29132 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C4.png
--rw-rw-rw-   0        0        0    35845 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C5.png
--rw-rw-rw-   0        0        0    40916 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C6.png
--rw-rw-rw-   0        0        0    41816 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C7.png
--rw-rw-rw-   0        0        0    48567 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C8.png
--rw-rw-rw-   0        0        0    52318 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/C9.png
--rw-rw-rw-   0        0        0   432659 2021-11-02 01:23:17.000000 five_card_draw-1.0.6/src/five_card_draw/data/CardBack.png
--rw-rw-rw-   0        0        0    46699 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/D10.png
--rw-rw-rw-   0        0        0   197802 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/D11.png
--rw-rw-rw-   0        0        0   180712 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/D12.png
--rw-rw-rw-   0        0        0   198565 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/D13.png
--rw-rw-rw-   0        0        0    30901 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/D14.png
--rw-rw-rw-   0        0        0    19170 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/D2.png
--rw-rw-rw-   0        0        0    23815 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/D3.png
--rw-rw-rw-   0        0        0    24296 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/D4.png
--rw-rw-rw-   0        0        0    29806 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/D5.png
--rw-rw-rw-   0        0        0    33800 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/D6.png
--rw-rw-rw-   0        0        0    34176 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/D7.png
--rw-rw-rw-   0        0        0    40724 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/D8.png
--rw-rw-rw-   0        0        0    43365 2021-10-31 00:37:13.000000 five_card_draw-1.0.6/src/five_card_draw/data/D9.png
--rw-rw-rw-   0        0        0    49317 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/H10.png
--rw-rw-rw-   0        0        0   203728 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/H11.png
--rw-rw-rw-   0        0        0   197792 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/H12.png
--rw-rw-rw-   0        0        0   207052 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/H13.png
--rw-rw-rw-   0        0        0    36444 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/H14.png
--rw-rw-rw-   0        0        0    20058 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/H2.png
--rw-rw-rw-   0        0        0    24919 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/H3.png
--rw-rw-rw-   0        0        0    25320 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/H4.png
--rw-rw-rw-   0        0        0    31082 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/H5.png
--rw-rw-rw-   0        0        0    35239 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/H6.png
--rw-rw-rw-   0        0        0    35904 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/H7.png
--rw-rw-rw-   0        0        0    42890 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/H8.png
--rw-rw-rw-   0        0        0    45669 2021-10-31 00:37:13.000000 five_card_draw-1.0.6/src/five_card_draw/data/H9.png
--rw-rw-rw-   0        0        0    50853 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/S10.png
--rw-rw-rw-   0        0        0   190953 2021-10-31 00:37:11.000000 five_card_draw-1.0.6/src/five_card_draw/data/S11.png
--rw-rw-rw-   0        0        0   186480 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S12.png
--rw-rw-rw-   0        0        0   183329 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S13.png
--rw-rw-rw-   0        0        0    56051 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S14.png
--rw-rw-rw-   0        0        0    21104 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S2.png
--rw-rw-rw-   0        0        0    26211 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S3.png
--rw-rw-rw-   0        0        0    26311 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S4.png
--rw-rw-rw-   0        0        0    32110 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S5.png
--rw-rw-rw-   0        0        0    36726 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S6.png
--rw-rw-rw-   0        0        0    37510 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S7.png
--rw-rw-rw-   0        0        0    43823 2021-10-31 00:37:12.000000 five_card_draw-1.0.6/src/five_card_draw/data/S8.png
--rw-rw-rw-   0        0        0    46996 2021-10-31 00:37:13.000000 five_card_draw-1.0.6/src/five_card_draw/data/S9.png
--rw-rw-rw-   0        0        0   560393 2023-06-08 17:03:00.000000 five_card_draw-1.0.6/src/five_card_draw/data/ScoringImage.png
--rw-rw-rw-   0        0        0    43719 2021-10-31 00:37:13.000000 five_card_draw-1.0.6/src/five_card_draw/data/black_joker.png
--rw-rw-rw-   0        0        0    44079 2021-10-31 00:37:13.000000 five_card_draw-1.0.6/src/five_card_draw/data/red_joker.png
--rw-rw-rw-   0        0        0        4 2023-06-09 00:26:49.000000 five_card_draw-1.0.6/src/five_card_draw/fcd_bank.txt
--rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.6/src/five_card_draw/fcd_functions.py
--rw-rw-rw-   0        0        0    15556 2023-06-12 15:31:36.000000 five_card_draw-1.0.6/src/five_card_draw/fcd_pagegui.py
--rw-rw-rw-   0        0        0      486 2023-06-12 15:31:35.000000 five_card_draw-1.0.6/src/five_card_draw/poker_start.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.862863 five_card_draw-1.0.7/
+-rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       55 2023-06-12 13:48:00.000000 five_card_draw-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     7300 2023-06-12 15:46:01.862863 five_card_draw-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6996 2023-06-12 15:44:46.000000 five_card_draw-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.805585 five_card_draw-1.0.7/five_card_draw.egg-info/
+-rw-rw-rw-   0        0        0     7300 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2155 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 15:46:01.862863 five_card_draw-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1695 2023-06-12 15:45:43.000000 five_card_draw-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.789629 five_card_draw-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.809574 five_card_draw-1.0.7/src/five_card_draw/
+drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.861863 five_card_draw-1.0.7/src/five_card_draw/data/
+-rw-rw-rw-   0        0        0    56484 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/C10.png
+-rw-rw-rw-   0        0        0   187958 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/C11.png
+-rw-rw-rw-   0        0        0   205820 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/C12.png
+-rw-rw-rw-   0        0        0   189382 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C13.png
+-rw-rw-rw-   0        0        0    37544 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C14.png
+-rw-rw-rw-   0        0        0    23382 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C2.png
+-rw-rw-rw-   0        0        0    29340 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C3.png
+-rw-rw-rw-   0        0        0    29132 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C4.png
+-rw-rw-rw-   0        0        0    35845 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C5.png
+-rw-rw-rw-   0        0        0    40916 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C6.png
+-rw-rw-rw-   0        0        0    41816 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C7.png
+-rw-rw-rw-   0        0        0    48567 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C8.png
+-rw-rw-rw-   0        0        0    52318 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C9.png
+-rw-rw-rw-   0        0        0   432659 2021-11-02 01:23:17.000000 five_card_draw-1.0.7/src/five_card_draw/data/CardBack.png
+-rw-rw-rw-   0        0        0    46699 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/D10.png
+-rw-rw-rw-   0        0        0   197802 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/D11.png
+-rw-rw-rw-   0        0        0   180712 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/D12.png
+-rw-rw-rw-   0        0        0   198565 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D13.png
+-rw-rw-rw-   0        0        0    30901 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D14.png
+-rw-rw-rw-   0        0        0    19170 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D2.png
+-rw-rw-rw-   0        0        0    23815 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D3.png
+-rw-rw-rw-   0        0        0    24296 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D4.png
+-rw-rw-rw-   0        0        0    29806 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D5.png
+-rw-rw-rw-   0        0        0    33800 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D6.png
+-rw-rw-rw-   0        0        0    34176 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D7.png
+-rw-rw-rw-   0        0        0    40724 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D8.png
+-rw-rw-rw-   0        0        0    43365 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/D9.png
+-rw-rw-rw-   0        0        0    49317 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/H10.png
+-rw-rw-rw-   0        0        0   203728 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/H11.png
+-rw-rw-rw-   0        0        0   197792 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/H12.png
+-rw-rw-rw-   0        0        0   207052 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H13.png
+-rw-rw-rw-   0        0        0    36444 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H14.png
+-rw-rw-rw-   0        0        0    20058 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H2.png
+-rw-rw-rw-   0        0        0    24919 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H3.png
+-rw-rw-rw-   0        0        0    25320 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H4.png
+-rw-rw-rw-   0        0        0    31082 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H5.png
+-rw-rw-rw-   0        0        0    35239 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H6.png
+-rw-rw-rw-   0        0        0    35904 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H7.png
+-rw-rw-rw-   0        0        0    42890 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H8.png
+-rw-rw-rw-   0        0        0    45669 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/H9.png
+-rw-rw-rw-   0        0        0    50853 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/S10.png
+-rw-rw-rw-   0        0        0   190953 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/S11.png
+-rw-rw-rw-   0        0        0   186480 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S12.png
+-rw-rw-rw-   0        0        0   183329 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S13.png
+-rw-rw-rw-   0        0        0    56051 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S14.png
+-rw-rw-rw-   0        0        0    21104 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S2.png
+-rw-rw-rw-   0        0        0    26211 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S3.png
+-rw-rw-rw-   0        0        0    26311 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S4.png
+-rw-rw-rw-   0        0        0    32110 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S5.png
+-rw-rw-rw-   0        0        0    36726 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S6.png
+-rw-rw-rw-   0        0        0    37510 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S7.png
+-rw-rw-rw-   0        0        0    43823 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S8.png
+-rw-rw-rw-   0        0        0    46996 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/S9.png
+-rw-rw-rw-   0        0        0   560393 2023-06-08 17:03:00.000000 five_card_draw-1.0.7/src/five_card_draw/data/ScoringImage.png
+-rw-rw-rw-   0        0        0    43719 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/black_joker.png
+-rw-rw-rw-   0        0        0    44079 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/red_joker.png
+-rw-rw-rw-   0        0        0        4 2023-06-09 00:26:49.000000 five_card_draw-1.0.7/src/five_card_draw/fcd_bank.txt
+-rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.7/src/five_card_draw/fcd_functions.py
+-rw-rw-rw-   0        0        0    15556 2023-06-12 15:31:36.000000 five_card_draw-1.0.7/src/five_card_draw/fcd_pagegui.py
+-rw-rw-rw-   0        0        0      486 2023-06-12 15:31:35.000000 five_card_draw-1.0.7/src/five_card_draw/poker_start.py
```

### Comparing `five_card_draw-1.0.6/LICENSE.txt` & `five_card_draw-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/PKG-INFO` & `five_card_draw-1.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: five_card_draw
-Version: 1.0.6
-Summary: 5 Card Draw Video Poker application
-Home-page: https://github.com/ralbee1/5_card_draw
-Author: Richard Albee
-Author-email: Ralbee1@iwu.edu
-License: LICENSE.txt
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <a name="readme-top"></a>
 
 <!-- VideoPoker-5CardRedraw -->
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
@@ -131,17 +120,23 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- USAGE EXAMPLES -->
 ## Usage / How to Play
 If your python files open with Python by default then from the commmand line run:
 
   ```js
-  5_card_draw.py;
+  poker_start.py;
   ```
 
+Troubleshooting:
+1. "'poker_start.py' is not recognized as an internal or external command, operable program or batch file."
+  Your terminal needs to be able to find the file. For windows, you need to ensure your python "script" folder is in your path variable
+  For example: C:\Users\{username}\AppData\Roaming\Python\{pythonversion}\Scripts
+  You may also navigate to where the pip was installed and run poker_start.py with python manually.
+
 The game is played by aiming to make the best poker hand possible. The top of the interface shows the hand ranking and the payouts sorted by how many credits you bet per round, 1 thru 5. To begin, click DEAL. You hold cards with the intent of keeping them and drawing new cards to try to improve your hand ranking. After drawing new cards, your hand is automatically scored and profits are payed out. You may then click "DEAL" and start over.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- CONTACT -->
 ## Contact
```

#### html2text {}

```diff
@@ -1,14 +1,10 @@
-Metadata-Version: 2.1 Name: five_card_draw Version: 1.0.6 Summary: 5 Card Draw
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
@@ -49,21 +45,27 @@
 m pip install -e . ```
 
 User Install
 1. Automatic User Install from the Command line via PyPi. ```sh pip install
 five-card-draw ```
                                                                   (back_to_top)
  ## Usage / How to Play If your python files open with Python by default then
-from the commmand line run: ```js 5_card_draw.py; ``` The game is played by
-aiming to make the best poker hand possible. The top of the interface shows the
-hand ranking and the payouts sorted by how many credits you bet per round, 1
-thru 5. To begin, click DEAL. You hold cards with the intent of keeping them
-and drawing new cards to try to improve your hand ranking. After drawing new
-cards, your hand is automatically scored and profits are payed out. You may
-then click "DEAL" and start over.
+from the commmand line run: ```js poker_start.py; ``` Troubleshooting: 1.
+"'poker_start.py' is not recognized as an internal or external command,
+operable program or batch file." Your terminal needs to be able to find the
+file. For windows, you need to ensure your python "script" folder is in your
+path variable For example: C:\Users\{username}\AppData\Roaming\Python\
+{pythonversion}\Scripts You may also navigate to where the pip was installed
+and run poker_start.py with python manually. The game is played by aiming to
+make the best poker hand possible. The top of the interface shows the hand
+ranking and the payouts sorted by how many credits you bet per round, 1 thru 5.
+To begin, click DEAL. You hold cards with the intent of keeping them and
+drawing new cards to try to improve your hand ranking. After drawing new cards,
+your hand is automatically scored and profits are payed out. You may then click
+"DEAL" and start over.
                                                                   (back_to_top)
  ## Contact * []()Email - ralbee1@iwu.edu * []()Project Link: [https://
 github.com/ralbee1/VideoPoker-5CardRedraw](https://github.com/ralbee1/
 VideoPoker-5CardRedraw)  ## Acknowledgments * []() This variant of poker was
 inspired by Super Double Double as found in Las Vegas Casinos.
                                                                   (back_to_top)
   [contributors-shield]: https://img.shields.io/github/contributors/ralbee1/
```

### Comparing `five_card_draw-1.0.6/README.md` & `five_card_draw-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: five_card_draw
+Version: 1.0.7
+Summary: 5 Card Draw Video Poker application
+Home-page: https://github.com/ralbee1/5_card_draw
+Author: Richard Albee
+Author-email: Ralbee1@iwu.edu
+License: LICENSE.txt
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <a name="readme-top"></a>
 
 <!-- VideoPoker-5CardRedraw -->
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
@@ -120,17 +131,23 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- USAGE EXAMPLES -->
 ## Usage / How to Play
 If your python files open with Python by default then from the commmand line run:
 
   ```js
-  5_card_draw.py;
+  poker_start.py;
   ```
 
+Troubleshooting:
+1. "'poker_start.py' is not recognized as an internal or external command, operable program or batch file."
+  Your terminal needs to be able to find the file. For windows, you need to ensure your python "script" folder is in your path variable
+  For example: C:\Users\{username}\AppData\Roaming\Python\{pythonversion}\Scripts
+  You may also navigate to where the pip was installed and run poker_start.py with python manually.
+
 The game is played by aiming to make the best poker hand possible. The top of the interface shows the hand ranking and the payouts sorted by how many credits you bet per round, 1 thru 5. To begin, click DEAL. You hold cards with the intent of keeping them and drawing new cards to try to improve your hand ranking. After drawing new cards, your hand is automatically scored and profits are payed out. You may then click "DEAL" and start over.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- CONTACT -->
 ## Contact
```

#### html2text {}

```diff
@@ -1,10 +1,14 @@
-  [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
+Metadata-Version: 2.1 Name: five_card_draw Version: 1.0.7 Summary: 5 Card Draw
+Video Poker application Home-page: https://github.com/ralbee1/5_card_draw
+Author: Richard Albee Author-email: Ralbee1@iwu.edu License: LICENSE.txt
+Description-Content-Type: text/markdown License-File: LICENSE.txt   [!
+[Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
+[forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
+[issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
 [linkedin-shield]][linkedin-url]
                                     [Logo]
                        **** VideoPoker-5CardRedraw ****
              A pythonic creation of a 5 card redraw video poker.
                              Explore_the_docs_Â»
 
                   View_Demo Â· Report_Bug Â· Request_Feature
@@ -45,21 +49,27 @@
 m pip install -e . ```
 
 User Install
 1. Automatic User Install from the Command line via PyPi. ```sh pip install
 five-card-draw ```
                                                                   (back_to_top)
  ## Usage / How to Play If your python files open with Python by default then
-from the commmand line run: ```js 5_card_draw.py; ``` The game is played by
-aiming to make the best poker hand possible. The top of the interface shows the
-hand ranking and the payouts sorted by how many credits you bet per round, 1
-thru 5. To begin, click DEAL. You hold cards with the intent of keeping them
-and drawing new cards to try to improve your hand ranking. After drawing new
-cards, your hand is automatically scored and profits are payed out. You may
-then click "DEAL" and start over.
+from the commmand line run: ```js poker_start.py; ``` Troubleshooting: 1.
+"'poker_start.py' is not recognized as an internal or external command,
+operable program or batch file." Your terminal needs to be able to find the
+file. For windows, you need to ensure your python "script" folder is in your
+path variable For example: C:\Users\{username}\AppData\Roaming\Python\
+{pythonversion}\Scripts You may also navigate to where the pip was installed
+and run poker_start.py with python manually. The game is played by aiming to
+make the best poker hand possible. The top of the interface shows the hand
+ranking and the payouts sorted by how many credits you bet per round, 1 thru 5.
+To begin, click DEAL. You hold cards with the intent of keeping them and
+drawing new cards to try to improve your hand ranking. After drawing new cards,
+your hand is automatically scored and profits are payed out. You may then click
+"DEAL" and start over.
                                                                   (back_to_top)
  ## Contact * []()Email - ralbee1@iwu.edu * []()Project Link: [https://
 github.com/ralbee1/VideoPoker-5CardRedraw](https://github.com/ralbee1/
 VideoPoker-5CardRedraw)  ## Acknowledgments * []() This variant of poker was
 inspired by Super Double Double as found in Las Vegas Casinos.
                                                                   (back_to_top)
   [contributors-shield]: https://img.shields.io/github/contributors/ralbee1/
```

### Comparing `five_card_draw-1.0.6/five_card_draw.egg-info/PKG-INFO` & `five_card_draw-1.0.7/five_card_draw.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: five-card-draw
-Version: 1.0.6
+Version: 1.0.7
 Summary: 5 Card Draw Video Poker application
 Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -131,17 +131,23 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- USAGE EXAMPLES -->
 ## Usage / How to Play
 If your python files open with Python by default then from the commmand line run:
 
   ```js
-  5_card_draw.py;
+  poker_start.py;
   ```
 
+Troubleshooting:
+1. "'poker_start.py' is not recognized as an internal or external command, operable program or batch file."
+  Your terminal needs to be able to find the file. For windows, you need to ensure your python "script" folder is in your path variable
+  For example: C:\Users\{username}\AppData\Roaming\Python\{pythonversion}\Scripts
+  You may also navigate to where the pip was installed and run poker_start.py with python manually.
+
 The game is played by aiming to make the best poker hand possible. The top of the interface shows the hand ranking and the payouts sorted by how many credits you bet per round, 1 thru 5. To begin, click DEAL. You hold cards with the intent of keeping them and drawing new cards to try to improve your hand ranking. After drawing new cards, your hand is automatically scored and profits are payed out. You may then click "DEAL" and start over.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- CONTACT -->
 ## Contact
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: five-card-draw Version: 1.0.6 Summary: 5 Card Draw
+Metadata-Version: 2.1 Name: five-card-draw Version: 1.0.7 Summary: 5 Card Draw
 Video Poker application Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee Author-email: Ralbee1@iwu.edu License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENSE.txt   [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
 [linkedin-shield]][linkedin-url]
@@ -49,21 +49,27 @@
 m pip install -e . ```
 
 User Install
 1. Automatic User Install from the Command line via PyPi. ```sh pip install
 five-card-draw ```
                                                                   (back_to_top)
  ## Usage / How to Play If your python files open with Python by default then
-from the commmand line run: ```js 5_card_draw.py; ``` The game is played by
-aiming to make the best poker hand possible. The top of the interface shows the
-hand ranking and the payouts sorted by how many credits you bet per round, 1
-thru 5. To begin, click DEAL. You hold cards with the intent of keeping them
-and drawing new cards to try to improve your hand ranking. After drawing new
-cards, your hand is automatically scored and profits are payed out. You may
-then click "DEAL" and start over.
+from the commmand line run: ```js poker_start.py; ``` Troubleshooting: 1.
+"'poker_start.py' is not recognized as an internal or external command,
+operable program or batch file." Your terminal needs to be able to find the
+file. For windows, you need to ensure your python "script" folder is in your
+path variable For example: C:\Users\{username}\AppData\Roaming\Python\
+{pythonversion}\Scripts You may also navigate to where the pip was installed
+and run poker_start.py with python manually. The game is played by aiming to
+make the best poker hand possible. The top of the interface shows the hand
+ranking and the payouts sorted by how many credits you bet per round, 1 thru 5.
+To begin, click DEAL. You hold cards with the intent of keeping them and
+drawing new cards to try to improve your hand ranking. After drawing new cards,
+your hand is automatically scored and profits are payed out. You may then click
+"DEAL" and start over.
                                                                   (back_to_top)
  ## Contact * []()Email - ralbee1@iwu.edu * []()Project Link: [https://
 github.com/ralbee1/VideoPoker-5CardRedraw](https://github.com/ralbee1/
 VideoPoker-5CardRedraw)  ## Acknowledgments * []() This variant of poker was
 inspired by Super Double Double as found in Las Vegas Casinos.
                                                                   (back_to_top)
   [contributors-shield]: https://img.shields.io/github/contributors/ralbee1/
```

### Comparing `five_card_draw-1.0.6/five_card_draw.egg-info/SOURCES.txt` & `five_card_draw-1.0.7/five_card_draw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/setup.py` & `five_card_draw-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 scripts = [
     str(Path('src/five_card_draw','poker_start.py'))
 ]
 
 #Using distutils.core over setuptools since package data was not specified correctly, needing the manifest.in file
 setup(
     name = 'five_card_draw',
-    version = os.getenv('PACKAGE_VERSION', '1.0.6'),
+    version = os.getenv('PACKAGE_VERSION', '1.0.7'),
     author = 'Richard Albee',
     author_email='Ralbee1@iwu.edu',
     packages=['five_card_draw','five_card_draw.data'],
     package_dir={'five_card_draw': 'src/five_card_draw'},
     package_data={'five_card_draw': ['data/*.png','*.txt']},
     scripts=scripts,
     url = "https://github.com/ralbee1/5_card_draw",
```

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C10.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C11.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C12.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C13.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C14.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C2.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C3.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C4.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C5.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C6.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C7.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C8.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/C9.png` & `five_card_draw-1.0.7/src/five_card_draw/data/C9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/CardBack.png` & `five_card_draw-1.0.7/src/five_card_draw/data/CardBack.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D10.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D11.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D12.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D13.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D14.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D2.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D3.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D4.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D5.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D6.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D7.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D8.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/D9.png` & `five_card_draw-1.0.7/src/five_card_draw/data/D9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H10.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H11.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H12.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H13.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H14.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H2.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H3.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H4.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H5.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H6.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H7.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H8.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/H9.png` & `five_card_draw-1.0.7/src/five_card_draw/data/H9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S10.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S11.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S12.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S13.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S14.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S2.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S3.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S4.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S5.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S6.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S7.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S8.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/S9.png` & `five_card_draw-1.0.7/src/five_card_draw/data/S9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/ScoringImage.png` & `five_card_draw-1.0.7/src/five_card_draw/data/ScoringImage.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/black_joker.png` & `five_card_draw-1.0.7/src/five_card_draw/data/black_joker.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/data/red_joker.png` & `five_card_draw-1.0.7/src/five_card_draw/data/red_joker.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/fcd_functions.py` & `five_card_draw-1.0.7/src/five_card_draw/fcd_functions.py`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.6/src/five_card_draw/fcd_pagegui.py` & `five_card_draw-1.0.7/src/five_card_draw/fcd_pagegui.py`

 * *Files identical despite different names*

