# Comparing `tmp/five_card_draw-1.0.7.tar.gz` & `tmp/five_card_draw-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "five_card_draw-1.0.7.tar", last modified: Mon Jun 12 15:46:01 2023, max compression
+gzip compressed data, was "five_card_draw-1.0.8.tar", last modified: Mon Jun 12 16:35:51 2023, max compression
```

## Comparing `five_card_draw-1.0.7.tar` & `five_card_draw-1.0.8.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.862863 five_card_draw-1.0.7/
--rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       55 2023-06-12 13:48:00.000000 five_card_draw-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     7300 2023-06-12 15:46:01.862863 five_card_draw-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6996 2023-06-12 15:44:46.000000 five_card_draw-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.805585 five_card_draw-1.0.7/five_card_draw.egg-info/
--rw-rw-rw-   0        0        0     7300 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2155 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-12 15:46:01.000000 five_card_draw-1.0.7/five_card_draw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 15:46:01.862863 five_card_draw-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1695 2023-06-12 15:45:43.000000 five_card_draw-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.789629 five_card_draw-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.809574 five_card_draw-1.0.7/src/five_card_draw/
-drwxrwxrwx   0        0        0        0 2023-06-12 15:46:01.861863 five_card_draw-1.0.7/src/five_card_draw/data/
--rw-rw-rw-   0        0        0    56484 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/C10.png
--rw-rw-rw-   0        0        0   187958 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/C11.png
--rw-rw-rw-   0        0        0   205820 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/C12.png
--rw-rw-rw-   0        0        0   189382 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C13.png
--rw-rw-rw-   0        0        0    37544 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C14.png
--rw-rw-rw-   0        0        0    23382 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C2.png
--rw-rw-rw-   0        0        0    29340 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C3.png
--rw-rw-rw-   0        0        0    29132 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C4.png
--rw-rw-rw-   0        0        0    35845 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C5.png
--rw-rw-rw-   0        0        0    40916 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C6.png
--rw-rw-rw-   0        0        0    41816 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C7.png
--rw-rw-rw-   0        0        0    48567 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C8.png
--rw-rw-rw-   0        0        0    52318 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/C9.png
--rw-rw-rw-   0        0        0   432659 2021-11-02 01:23:17.000000 five_card_draw-1.0.7/src/five_card_draw/data/CardBack.png
--rw-rw-rw-   0        0        0    46699 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/D10.png
--rw-rw-rw-   0        0        0   197802 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/D11.png
--rw-rw-rw-   0        0        0   180712 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/D12.png
--rw-rw-rw-   0        0        0   198565 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D13.png
--rw-rw-rw-   0        0        0    30901 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D14.png
--rw-rw-rw-   0        0        0    19170 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D2.png
--rw-rw-rw-   0        0        0    23815 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D3.png
--rw-rw-rw-   0        0        0    24296 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D4.png
--rw-rw-rw-   0        0        0    29806 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D5.png
--rw-rw-rw-   0        0        0    33800 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D6.png
--rw-rw-rw-   0        0        0    34176 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D7.png
--rw-rw-rw-   0        0        0    40724 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/D8.png
--rw-rw-rw-   0        0        0    43365 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/D9.png
--rw-rw-rw-   0        0        0    49317 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/H10.png
--rw-rw-rw-   0        0        0   203728 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/H11.png
--rw-rw-rw-   0        0        0   197792 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/H12.png
--rw-rw-rw-   0        0        0   207052 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H13.png
--rw-rw-rw-   0        0        0    36444 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H14.png
--rw-rw-rw-   0        0        0    20058 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H2.png
--rw-rw-rw-   0        0        0    24919 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H3.png
--rw-rw-rw-   0        0        0    25320 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H4.png
--rw-rw-rw-   0        0        0    31082 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H5.png
--rw-rw-rw-   0        0        0    35239 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H6.png
--rw-rw-rw-   0        0        0    35904 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H7.png
--rw-rw-rw-   0        0        0    42890 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/H8.png
--rw-rw-rw-   0        0        0    45669 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/H9.png
--rw-rw-rw-   0        0        0    50853 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/S10.png
--rw-rw-rw-   0        0        0   190953 2021-10-31 00:37:11.000000 five_card_draw-1.0.7/src/five_card_draw/data/S11.png
--rw-rw-rw-   0        0        0   186480 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S12.png
--rw-rw-rw-   0        0        0   183329 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S13.png
--rw-rw-rw-   0        0        0    56051 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S14.png
--rw-rw-rw-   0        0        0    21104 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S2.png
--rw-rw-rw-   0        0        0    26211 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S3.png
--rw-rw-rw-   0        0        0    26311 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S4.png
--rw-rw-rw-   0        0        0    32110 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S5.png
--rw-rw-rw-   0        0        0    36726 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S6.png
--rw-rw-rw-   0        0        0    37510 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S7.png
--rw-rw-rw-   0        0        0    43823 2021-10-31 00:37:12.000000 five_card_draw-1.0.7/src/five_card_draw/data/S8.png
--rw-rw-rw-   0        0        0    46996 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/S9.png
--rw-rw-rw-   0        0        0   560393 2023-06-08 17:03:00.000000 five_card_draw-1.0.7/src/five_card_draw/data/ScoringImage.png
--rw-rw-rw-   0        0        0    43719 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/black_joker.png
--rw-rw-rw-   0        0        0    44079 2021-10-31 00:37:13.000000 five_card_draw-1.0.7/src/five_card_draw/data/red_joker.png
--rw-rw-rw-   0        0        0        4 2023-06-09 00:26:49.000000 five_card_draw-1.0.7/src/five_card_draw/fcd_bank.txt
--rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.7/src/five_card_draw/fcd_functions.py
--rw-rw-rw-   0        0        0    15556 2023-06-12 15:31:36.000000 five_card_draw-1.0.7/src/five_card_draw/fcd_pagegui.py
--rw-rw-rw-   0        0        0      486 2023-06-12 15:31:35.000000 five_card_draw-1.0.7/src/five_card_draw/poker_start.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:35:51.155023 five_card_draw-1.0.8/
+-rw-rw-rw-   0        0        0     1085 2023-05-07 02:37:12.000000 five_card_draw-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       55 2023-06-12 13:48:00.000000 five_card_draw-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     7300 2023-06-12 16:35:51.155023 five_card_draw-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6996 2023-06-12 15:44:46.000000 five_card_draw-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 16:35:50.930230 five_card_draw-1.0.8/five_card_draw/
+drwxrwxrwx   0        0        0        0 2023-06-12 16:35:51.154026 five_card_draw-1.0.8/five_card_draw/data/
+-rw-rw-rw-   0        0        0    56484 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/C10.png
+-rw-rw-rw-   0        0        0   187958 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/C11.png
+-rw-rw-rw-   0        0        0   205820 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/C12.png
+-rw-rw-rw-   0        0        0   189382 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C13.png
+-rw-rw-rw-   0        0        0    37544 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C14.png
+-rw-rw-rw-   0        0        0    23382 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C2.png
+-rw-rw-rw-   0        0        0    29340 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C3.png
+-rw-rw-rw-   0        0        0    29132 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C4.png
+-rw-rw-rw-   0        0        0    35845 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C5.png
+-rw-rw-rw-   0        0        0    40916 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C6.png
+-rw-rw-rw-   0        0        0    41816 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C7.png
+-rw-rw-rw-   0        0        0    48567 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C8.png
+-rw-rw-rw-   0        0        0    52318 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/C9.png
+-rw-rw-rw-   0        0        0   432659 2021-11-02 01:23:17.000000 five_card_draw-1.0.8/five_card_draw/data/CardBack.png
+-rw-rw-rw-   0        0        0    46699 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/D10.png
+-rw-rw-rw-   0        0        0   197802 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/D11.png
+-rw-rw-rw-   0        0        0   180712 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/D12.png
+-rw-rw-rw-   0        0        0   198565 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D13.png
+-rw-rw-rw-   0        0        0    30901 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D14.png
+-rw-rw-rw-   0        0        0    19170 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D2.png
+-rw-rw-rw-   0        0        0    23815 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D3.png
+-rw-rw-rw-   0        0        0    24296 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D4.png
+-rw-rw-rw-   0        0        0    29806 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D5.png
+-rw-rw-rw-   0        0        0    33800 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D6.png
+-rw-rw-rw-   0        0        0    34176 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D7.png
+-rw-rw-rw-   0        0        0    40724 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/D8.png
+-rw-rw-rw-   0        0        0    43365 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/D9.png
+-rw-rw-rw-   0        0        0    49317 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/H10.png
+-rw-rw-rw-   0        0        0   203728 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/H11.png
+-rw-rw-rw-   0        0        0   197792 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/H12.png
+-rw-rw-rw-   0        0        0   207052 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H13.png
+-rw-rw-rw-   0        0        0    36444 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H14.png
+-rw-rw-rw-   0        0        0    20058 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H2.png
+-rw-rw-rw-   0        0        0    24919 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H3.png
+-rw-rw-rw-   0        0        0    25320 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H4.png
+-rw-rw-rw-   0        0        0    31082 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H5.png
+-rw-rw-rw-   0        0        0    35239 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H6.png
+-rw-rw-rw-   0        0        0    35904 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H7.png
+-rw-rw-rw-   0        0        0    42890 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/H8.png
+-rw-rw-rw-   0        0        0    45669 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/H9.png
+-rw-rw-rw-   0        0        0    50853 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/S10.png
+-rw-rw-rw-   0        0        0   190953 2021-10-31 00:37:11.000000 five_card_draw-1.0.8/five_card_draw/data/S11.png
+-rw-rw-rw-   0        0        0   186480 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S12.png
+-rw-rw-rw-   0        0        0   183329 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S13.png
+-rw-rw-rw-   0        0        0    56051 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S14.png
+-rw-rw-rw-   0        0        0    21104 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S2.png
+-rw-rw-rw-   0        0        0    26211 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S3.png
+-rw-rw-rw-   0        0        0    26311 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S4.png
+-rw-rw-rw-   0        0        0    32110 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S5.png
+-rw-rw-rw-   0        0        0    36726 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S6.png
+-rw-rw-rw-   0        0        0    37510 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S7.png
+-rw-rw-rw-   0        0        0    43823 2021-10-31 00:37:12.000000 five_card_draw-1.0.8/five_card_draw/data/S8.png
+-rw-rw-rw-   0        0        0    46996 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/S9.png
+-rw-rw-rw-   0        0        0   560393 2023-06-08 17:03:00.000000 five_card_draw-1.0.8/five_card_draw/data/ScoringImage.png
+-rw-rw-rw-   0        0        0    43719 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/black_joker.png
+-rw-rw-rw-   0        0        0    44079 2021-10-31 00:37:13.000000 five_card_draw-1.0.8/five_card_draw/data/red_joker.png
+-rw-rw-rw-   0        0        0        4 2023-06-09 00:26:49.000000 five_card_draw-1.0.8/five_card_draw/fcd_bank.txt
+-rw-rw-rw-   0        0        0     9460 2023-06-09 00:26:20.000000 five_card_draw-1.0.8/five_card_draw/fcd_functions.py
+-rw-rw-rw-   0        0        0    15557 2023-06-12 16:33:46.000000 five_card_draw-1.0.8/five_card_draw/fcd_pagegui.py
+-rw-rw-rw-   0        0        0      486 2023-06-12 15:31:35.000000 five_card_draw-1.0.8/five_card_draw/poker_start.py
+drwxrwxrwx   0        0        0        0 2023-06-12 16:35:50.944480 five_card_draw-1.0.8/five_card_draw.egg-info/
+-rw-rw-rw-   0        0        0     7300 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1915 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 16:35:50.000000 five_card_draw-1.0.8/five_card_draw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 16:35:51.155023 five_card_draw-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1687 2023-06-12 16:35:28.000000 five_card_draw-1.0.8/setup.py
```

### Comparing `five_card_draw-1.0.7/LICENSE.txt` & `five_card_draw-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/PKG-INFO` & `five_card_draw-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: five_card_draw
-Version: 1.0.7
+Version: 1.0.8
 Summary: 5 Card Draw Video Poker application
 Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: five_card_draw Version: 1.0.7 Summary: 5 Card Draw
+Metadata-Version: 2.1 Name: five_card_draw Version: 1.0.8 Summary: 5 Card Draw
 Video Poker application Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee Author-email: Ralbee1@iwu.edu License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENSE.txt   [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
 [linkedin-shield]][linkedin-url]
```

### Comparing `five_card_draw-1.0.7/README.md` & `five_card_draw-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/five_card_draw.egg-info/PKG-INFO` & `five_card_draw-1.0.8/five_card_draw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: five-card-draw
-Version: 1.0.7
+Version: 1.0.8
 Summary: 5 Card Draw Video Poker application
 Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee
 Author-email: Ralbee1@iwu.edu
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: five-card-draw Version: 1.0.7 Summary: 5 Card Draw
+Metadata-Version: 2.1 Name: five-card-draw Version: 1.0.8 Summary: 5 Card Draw
 Video Poker application Home-page: https://github.com/ralbee1/5_card_draw
 Author: Richard Albee Author-email: Ralbee1@iwu.edu License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENSE.txt   [!
 [Contributors][contributors-shield]][contributors-url] [![Forks][forks-shield]]
 [forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
 [linkedin-shield]][linkedin-url]
```

### Comparing `five_card_draw-1.0.7/five_card_draw.egg-info/SOURCES.txt` & `five_card_draw-1.0.8/five_card_draw.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
+five_card_draw/fcd_bank.txt
+five_card_draw/fcd_functions.py
+five_card_draw/fcd_pagegui.py
+five_card_draw/poker_start.py
 five_card_draw.egg-info/PKG-INFO
 five_card_draw.egg-info/SOURCES.txt
 five_card_draw.egg-info/dependency_links.txt
 five_card_draw.egg-info/requires.txt
 five_card_draw.egg-info/top_level.txt
-src/five_card_draw/fcd_bank.txt
-src/five_card_draw/fcd_functions.py
-src/five_card_draw/fcd_pagegui.py
-src/five_card_draw/poker_start.py
-src/five_card_draw/data/C10.png
-src/five_card_draw/data/C11.png
-src/five_card_draw/data/C12.png
-src/five_card_draw/data/C13.png
-src/five_card_draw/data/C14.png
-src/five_card_draw/data/C2.png
-src/five_card_draw/data/C3.png
-src/five_card_draw/data/C4.png
-src/five_card_draw/data/C5.png
-src/five_card_draw/data/C6.png
-src/five_card_draw/data/C7.png
-src/five_card_draw/data/C8.png
-src/five_card_draw/data/C9.png
-src/five_card_draw/data/CardBack.png
-src/five_card_draw/data/D10.png
-src/five_card_draw/data/D11.png
-src/five_card_draw/data/D12.png
-src/five_card_draw/data/D13.png
-src/five_card_draw/data/D14.png
-src/five_card_draw/data/D2.png
-src/five_card_draw/data/D3.png
-src/five_card_draw/data/D4.png
-src/five_card_draw/data/D5.png
-src/five_card_draw/data/D6.png
-src/five_card_draw/data/D7.png
-src/five_card_draw/data/D8.png
-src/five_card_draw/data/D9.png
-src/five_card_draw/data/H10.png
-src/five_card_draw/data/H11.png
-src/five_card_draw/data/H12.png
-src/five_card_draw/data/H13.png
-src/five_card_draw/data/H14.png
-src/five_card_draw/data/H2.png
-src/five_card_draw/data/H3.png
-src/five_card_draw/data/H4.png
-src/five_card_draw/data/H5.png
-src/five_card_draw/data/H6.png
-src/five_card_draw/data/H7.png
-src/five_card_draw/data/H8.png
-src/five_card_draw/data/H9.png
-src/five_card_draw/data/S10.png
-src/five_card_draw/data/S11.png
-src/five_card_draw/data/S12.png
-src/five_card_draw/data/S13.png
-src/five_card_draw/data/S14.png
-src/five_card_draw/data/S2.png
-src/five_card_draw/data/S3.png
-src/five_card_draw/data/S4.png
-src/five_card_draw/data/S5.png
-src/five_card_draw/data/S6.png
-src/five_card_draw/data/S7.png
-src/five_card_draw/data/S8.png
-src/five_card_draw/data/S9.png
-src/five_card_draw/data/ScoringImage.png
-src/five_card_draw/data/black_joker.png
-src/five_card_draw/data/red_joker.png
+five_card_draw/data/C10.png
+five_card_draw/data/C11.png
+five_card_draw/data/C12.png
+five_card_draw/data/C13.png
+five_card_draw/data/C14.png
+five_card_draw/data/C2.png
+five_card_draw/data/C3.png
+five_card_draw/data/C4.png
+five_card_draw/data/C5.png
+five_card_draw/data/C6.png
+five_card_draw/data/C7.png
+five_card_draw/data/C8.png
+five_card_draw/data/C9.png
+five_card_draw/data/CardBack.png
+five_card_draw/data/D10.png
+five_card_draw/data/D11.png
+five_card_draw/data/D12.png
+five_card_draw/data/D13.png
+five_card_draw/data/D14.png
+five_card_draw/data/D2.png
+five_card_draw/data/D3.png
+five_card_draw/data/D4.png
+five_card_draw/data/D5.png
+five_card_draw/data/D6.png
+five_card_draw/data/D7.png
+five_card_draw/data/D8.png
+five_card_draw/data/D9.png
+five_card_draw/data/H10.png
+five_card_draw/data/H11.png
+five_card_draw/data/H12.png
+five_card_draw/data/H13.png
+five_card_draw/data/H14.png
+five_card_draw/data/H2.png
+five_card_draw/data/H3.png
+five_card_draw/data/H4.png
+five_card_draw/data/H5.png
+five_card_draw/data/H6.png
+five_card_draw/data/H7.png
+five_card_draw/data/H8.png
+five_card_draw/data/H9.png
+five_card_draw/data/S10.png
+five_card_draw/data/S11.png
+five_card_draw/data/S12.png
+five_card_draw/data/S13.png
+five_card_draw/data/S14.png
+five_card_draw/data/S2.png
+five_card_draw/data/S3.png
+five_card_draw/data/S4.png
+five_card_draw/data/S5.png
+five_card_draw/data/S6.png
+five_card_draw/data/S7.png
+five_card_draw/data/S8.png
+five_card_draw/data/S9.png
+five_card_draw/data/ScoringImage.png
+five_card_draw/data/black_joker.png
+five_card_draw/data/red_joker.png
```

### Comparing `five_card_draw-1.0.7/setup.py` & `five_card_draw-1.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,25 +21,25 @@
 from distutils.core import setup
 
 required_dependencies = [
     'tk',
     'pathlib'
 ]
 scripts = [
-    str(Path('src/five_card_draw','poker_start.py'))
+    str(Path('five_card_draw','poker_start.py'))
 ]
 
 #Using distutils.core over setuptools since package data was not specified correctly, needing the manifest.in file
 setup(
     name = 'five_card_draw',
-    version = os.getenv('PACKAGE_VERSION', '1.0.7'),
+    version = os.getenv('PACKAGE_VERSION', '1.0.8'),
     author = 'Richard Albee',
     author_email='Ralbee1@iwu.edu',
     packages=['five_card_draw','five_card_draw.data'],
-    package_dir={'five_card_draw': 'src/five_card_draw'},
+    package_dir={'five_card_draw': 'five_card_draw'},
     package_data={'five_card_draw': ['data/*.png','*.txt']},
     scripts=scripts,
     url = "https://github.com/ralbee1/5_card_draw",
     license='LICENSE.txt',
     description='5 Card Draw Video Poker application',
     long_description_content_type = 'text/markdown',
     long_description=open('README.md', encoding='utf-8').read(),
```

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C10.png` & `five_card_draw-1.0.8/five_card_draw/data/C10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C11.png` & `five_card_draw-1.0.8/five_card_draw/data/C11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C12.png` & `five_card_draw-1.0.8/five_card_draw/data/C12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C13.png` & `five_card_draw-1.0.8/five_card_draw/data/C13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C14.png` & `five_card_draw-1.0.8/five_card_draw/data/C14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C2.png` & `five_card_draw-1.0.8/five_card_draw/data/C2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C3.png` & `five_card_draw-1.0.8/five_card_draw/data/C3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C4.png` & `five_card_draw-1.0.8/five_card_draw/data/C4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C5.png` & `five_card_draw-1.0.8/five_card_draw/data/C5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C6.png` & `five_card_draw-1.0.8/five_card_draw/data/C6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C7.png` & `five_card_draw-1.0.8/five_card_draw/data/C7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C8.png` & `five_card_draw-1.0.8/five_card_draw/data/C8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/C9.png` & `five_card_draw-1.0.8/five_card_draw/data/C9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/CardBack.png` & `five_card_draw-1.0.8/five_card_draw/data/CardBack.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D10.png` & `five_card_draw-1.0.8/five_card_draw/data/D10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D11.png` & `five_card_draw-1.0.8/five_card_draw/data/D11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D12.png` & `five_card_draw-1.0.8/five_card_draw/data/D12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D13.png` & `five_card_draw-1.0.8/five_card_draw/data/D13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D14.png` & `five_card_draw-1.0.8/five_card_draw/data/D14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D2.png` & `five_card_draw-1.0.8/five_card_draw/data/D2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D3.png` & `five_card_draw-1.0.8/five_card_draw/data/D3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D4.png` & `five_card_draw-1.0.8/five_card_draw/data/D4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D5.png` & `five_card_draw-1.0.8/five_card_draw/data/D5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D6.png` & `five_card_draw-1.0.8/five_card_draw/data/D6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D7.png` & `five_card_draw-1.0.8/five_card_draw/data/D7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D8.png` & `five_card_draw-1.0.8/five_card_draw/data/D8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/D9.png` & `five_card_draw-1.0.8/five_card_draw/data/D9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H10.png` & `five_card_draw-1.0.8/five_card_draw/data/H10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H11.png` & `five_card_draw-1.0.8/five_card_draw/data/H11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H12.png` & `five_card_draw-1.0.8/five_card_draw/data/H12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H13.png` & `five_card_draw-1.0.8/five_card_draw/data/H13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H14.png` & `five_card_draw-1.0.8/five_card_draw/data/H14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H2.png` & `five_card_draw-1.0.8/five_card_draw/data/H2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H3.png` & `five_card_draw-1.0.8/five_card_draw/data/H3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H4.png` & `five_card_draw-1.0.8/five_card_draw/data/H4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H5.png` & `five_card_draw-1.0.8/five_card_draw/data/H5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H6.png` & `five_card_draw-1.0.8/five_card_draw/data/H6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H7.png` & `five_card_draw-1.0.8/five_card_draw/data/H7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H8.png` & `five_card_draw-1.0.8/five_card_draw/data/H8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/H9.png` & `five_card_draw-1.0.8/five_card_draw/data/H9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S10.png` & `five_card_draw-1.0.8/five_card_draw/data/S10.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S11.png` & `five_card_draw-1.0.8/five_card_draw/data/S11.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S12.png` & `five_card_draw-1.0.8/five_card_draw/data/S12.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S13.png` & `five_card_draw-1.0.8/five_card_draw/data/S13.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S14.png` & `five_card_draw-1.0.8/five_card_draw/data/S14.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S2.png` & `five_card_draw-1.0.8/five_card_draw/data/S2.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S3.png` & `five_card_draw-1.0.8/five_card_draw/data/S3.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S4.png` & `five_card_draw-1.0.8/five_card_draw/data/S4.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S5.png` & `five_card_draw-1.0.8/five_card_draw/data/S5.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S6.png` & `five_card_draw-1.0.8/five_card_draw/data/S6.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S7.png` & `five_card_draw-1.0.8/five_card_draw/data/S7.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S8.png` & `five_card_draw-1.0.8/five_card_draw/data/S8.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/S9.png` & `five_card_draw-1.0.8/five_card_draw/data/S9.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/ScoringImage.png` & `five_card_draw-1.0.8/five_card_draw/data/ScoringImage.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/black_joker.png` & `five_card_draw-1.0.8/five_card_draw/data/black_joker.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/data/red_joker.png` & `five_card_draw-1.0.8/five_card_draw/data/red_joker.png`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/fcd_functions.py` & `five_card_draw-1.0.8/five_card_draw/fcd_functions.py`

 * *Files identical despite different names*

### Comparing `five_card_draw-1.0.7/src/five_card_draw/fcd_pagegui.py` & `five_card_draw-1.0.8/five_card_draw/fcd_pagegui.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,31 +35,31 @@
         self.player_money = fcd_functions.load_player_balance()
 
         _bgcolor = '#d9d9d9'
         _fgcolor = '#000000'
 
         #This Section controls the game window name and color
         top.geometry("1920x1080")
-        top.minsize(1920, 1080)
-        top.maxsize(1920, 1080)
+        top.minsize(1800, 1080)
+        top.maxsize(1800, 1080)
         top.resizable(1,  1)
         top.title("5 Card Draw")
         top.configure(
             background="#00008b",
             highlightbackground="#d9d9d9",
             highlightcolor="black"
         )
 
         #global card image
         default_card_back_file = os.path.join(asset_file_directory + '\cardBack.png')
         default_card_back_file = tk.PhotoImage(file=default_card_back_file)
 
         #Initialize the bottom center display the number of winnings
         self.player_winnings_display = tk.Message(top)
-        self.player_winnings_display.place(relx=0.009, rely=0.905, relheight=0.093, relwidth=0.178)
+        self.player_winnings_display.place(relx=0.000, rely=0.905, relheight=0.093, relwidth=0.178)
         self.player_winnings_display.config(font=("Courier Bold", 55))
         self.player_winnings_display.configure(
             background="#00008b",
             foreground="#cc3300",
             highlightbackground="#d9d9d9",
             highlightcolor="black",
             text='''Winnings''',
@@ -76,15 +76,15 @@
             highlightcolor="black",
             text='CREDITS',
             width=550
         )
 
         #Initialize the banner image at the top
         self.banner = tk.Button(top)
-        self.banner.place(relx=0.030, rely=0.000, height=400, width=1800)
+        self.banner.place(relx=0.000, rely=0.000, height=400, width=1800)
         banner_image = os.path.join(asset_file_directory + '\ScoringImage.png')
         banner_image = tk.PhotoImage(file=banner_image)
         self.banner.configure(
             activebackground="#ececec",
             activeforeground="#000000",
             background="#d9d9d9",
             disabledforeground="#a3a3a3",
@@ -115,29 +115,29 @@
         hold_objects = [self.hold_button_1, self.hold_button_2, self.hold_button_3, self.hold_button_4, self.hold_button_5]
         for index, hold_object in enumerate(hold_objects):
             hold_object.configure(
                 background="#00008b",
                 foreground="#000000",
                 highlightbackground="#d9d9d9",
                 highlightcolor="black",
-                text=''' '''
+                text=''' ''',
             )
             hold_object.Image = default_card_back_file
 
         #Intialize card 1 through 5, left to right
         self.card_one = tk.Button(top)
-        self.card_one.place(relx=0.032, rely=0.430, height=508, width=350)
+        self.card_one.place(relx=0.014, rely=0.430, height=508, width=350)
         self.card_two = tk.Button(top)
-        self.card_two.place(relx=0.219, rely=0.430, height=508, width=350)
+        self.card_two.place(relx=0.209, rely=0.430, height=508, width=350)
         self.card_three = tk.Button(top)
-        self.card_three.place(relx=0.407, rely=0.430, height=508, width=350)
+        self.card_three.place(relx=0.404, rely=0.430, height=508, width=350)
         self.card_four = tk.Button(top)
-        self.card_four.place(relx=0.594, rely=0.430, height=508, width=350)
+        self.card_four.place(relx=0.599, rely=0.430, height=508, width=350)
         self.card_five = tk.Button(top)
-        self.card_five.place(relx=0.782, rely=0.430, height=508, width=350)
+        self.card_five.place(relx=0.794, rely=0.430, height=508, width=350)
 
         card_objects = [self.card_one, self.card_two, self.card_three, self.card_four, self.card_five]
         for index, card_object in enumerate(card_objects):
             card_object.configure(
             activebackground="#ececec",
             activeforeground="#000000",
             background="#00008b",
@@ -150,15 +150,15 @@
             command=lambda card_count = index + 1: self.toggle_card_hold(card_count),
             text='''Button'''
         )
             card_object.Image = default_card_back_file
 
         #Initialize the bet_one button
         self.bet_one_button = tk.Button(top)
-        self.bet_one_button.place(relx=0.185, rely=0.905, height=90, width=230)
+        self.bet_one_button.place(relx=0.180, rely=0.905, height=90, width=230)
         self.bet_one_button.config(font=("Courier Bold", 38))
         self.bet_one_button.configure(
             activebackground="#ececec",
             activeforeground="#000000",
             background="#E7E72B",
             disabledforeground="#a3a3a3",
             foreground="#000000",
@@ -197,15 +197,15 @@
             highlightcolor="black",
             text='''1''',
             width=342
         )
 
         #initialize the deal and redraw button
         self.deal_button = tk.Button(top)
-        self.deal_button.place(relx=0.625, rely=0.905, height=90, width=250)
+        self.deal_button.place(relx=0.615, rely=0.905, height=90, width=250)
         self.deal_button.config(font=("Courier Bold", 40))
         self.deal_button.configure(
             activebackground="#ececec",
             activeforeground="#000000",
             background="#E7E72B",
             disabledforeground="#a3a3a3",
             foreground="#000000",
@@ -214,15 +214,15 @@
             pady="0",
             text='''DEAL''',
             command=self.deal_command
         )
 
         #Initialize winning Hand banner in top center
         self.winning_hand = tk.Message(top)
-        self.winning_hand.place(relx=0.350, rely=0.365, relheight=0.045, relwidth=0.300)
+        self.winning_hand.place(relx=0.350, rely=0.370, relheight=0.045, relwidth=0.300)
         self.winning_hand.config(font=("Courier Bold", 44))
         self.winning_hand.configure(
             background="#E7E72B",
             foreground="#000000", #000000 #cc3300"
             text='''Hand Rank''',
             width=600
         )
```

