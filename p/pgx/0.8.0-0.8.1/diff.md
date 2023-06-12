# Comparing `tmp/pgx-0.8.0.tar.gz` & `tmp/pgx-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.8.0.tar", last modified: Fri May 26 04:16:33 2023, max compression
+gzip compressed data, was "pgx-0.8.1.tar", last modified: Mon Jun 12 09:53:37 2023, max compression
```

## Comparing `pgx-0.8.0.tar` & `pgx-0.8.1.tar`

### file list

```diff
@@ -1,148 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.569276 pgx-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 04:16:21.000000 pgx-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-26 04:16:33.569276 pgx-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14221 2023-05-26 04:16:21.000000 pgx-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.533276 pgx-0.8.0/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.537276 pgx-0.8.0/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_meld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_shanten.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/_yaku.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.537276 pgx-0.8.0/pgx/_mahjong/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_mahjong/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.541276 pgx-0.8.0/pgx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/api_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.545276 pgx-0.8.0/pgx/_src/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/assets/between.npy
--rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/assets/can_move.npy
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.549276 pgx-0.8.0/pgx/_src/dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/gardner_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.549276 pgx-0.8.0/pgx/_src/dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.553276 pgx-0.8.0/pgx/_src/dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.557276 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/dwg/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/gardner_chess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/_src/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    38512 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/connect_four.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.557276 pgx-0.8.0/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-26 04:16:21.000000 pgx-0.8.0/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/gardner_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.561276 pgx-0.8.0/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25161 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-05-26 04:16:22.000000 pgx-0.8.0/pgx/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.537276 pgx-0.8.0/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 04:16:33.000000 pgx-0.8.0/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-26 04:16:22.000000 pgx-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 04:16:33.569276 pgx-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-26 04:16:22.000000 pgx-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:33.565276 pgx-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    74697 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    39798 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    34016 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_gardner_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-26 04:16:22.000000 pgx-0.8.0/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.369275 pgx-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 09:53:24.000000 pgx-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-12 09:53:37.369275 pgx-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-06-12 09:53:24.000000 pgx-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.345275 pgx-0.8.1/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.349275 pgx-0.8.1/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_shanten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_yaku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.349275 pgx-0.8.1/pgx/_mahjong/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.349275 pgx-0.8.1/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.353275 pgx-0.8.1/pgx/_src/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/assets/between.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/assets/can_move.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.357275 pgx-0.8.1/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.357275 pgx-0.8.1/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.357275 pgx-0.8.1/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.361275 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/gardner_chess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38409 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.361275 pgx-0.8.1/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.365275 pgx-0.8.1/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25161 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.345275 pgx-0.8.1/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-12 09:53:24.000000 pgx-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:53:37.369275 pgx-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 09:53:24.000000 pgx-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.369275 pgx-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75241 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46618 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.8.0/LICENSE` & `pgx-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/PKG-INFO` & `pgx-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.8.0
+Version: 0.8.1
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -63,14 +63,20 @@
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
 while not (state.terminated | state.truncated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
+Pgx is a library that focuses on faster implementations rather than just the API itself. 
+However, the API itself is also sufficiently general. For example, all environments in Pgx can be converted to the AEC API of [PettingZoo](https://github.com/Farama-Foundation/PettingZoo), and you can run Pgx environments through the PettingZoo API.
+You can see the demonstration in Google Colab:
+
+<a href="https://colab.research.google.com/github/sotetsuk/pgx/blob/main/colab/pgx2pettingzoo.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+
 <!---
 ### Limitations (for the simplicity)
 * Does **NOT** support agent death and creation, which dynmically changes the array size. It does not well suit to GPU-accelerated computation.
 * Does **NOT** support Chance player (Nature player) with action selection.
 * Does **NOT** support OpenAI Gym API.
     * OpenAI Gym is for single-agent environment. Most of Pgx environments are multi-player games. Just defining opponents is not enough for converting multi-agent environemnts to OpenAI Gym environment. E.g., in the game of go, the next state s' is defined as the state just after placing a stone in AlhaGo paper. However, s' becomes the state after the opponents' play. This changes the definition of V(s').
 * Does **NOT** support PettingZoo API.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.8.0 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.8.1 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
@@ -30,31 +30,37 @@
 native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
 # vectorized states while not (state.terminated | state.truncated).all():
 action = model(state.current_player, state.observation,
 state.legal_action_mask) state = step(state, action) # state.reward (2,) ```
-## Supported games | Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:
-| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only]|[https:/
-/raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-
-dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+Pgx is a library that focuses on faster implementations rather than just the
+API itself. However, the API itself is also sufficiently general. For example,
+all environments in Pgx can be converted to the AEC API of [PettingZoo](https:/
+/github.com/Farama-Foundation/PettingZoo), and you can run Pgx environments
+through the PettingZoo API. You can see the demonstration in Google Colab:
+[Open_In_Colab]  ## Supported games | Backgammon | Chess | Shogi | Go | |:---:
+|:---:|:---:|:---:| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/backgammon_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
 light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
-`pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available
-games. Given an ``, you can create the environment via ```py >>> env = pgx.make
-() ``` You can check the current version of each environment by ```py >>>
-env.version ``` | Game/EnvId | Visualization | Version | Five-word description
-| |:---:|:---:|:---:|:---:| |2048
+assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
+> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
+can create the environment via ```py >>> env = pgx.make() ``` You can check the
+current version of each environment by ```py >>> env.version ``` | Game/EnvId |
+Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
+| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/animal_shogi_light.gif]| `v0` | *Animal-themed child-friendly
 shogi.* | |Backgammon
```

### Comparing `pgx-0.8.0/README.md` & `pgx-0.8.1/pgx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pgx
+Version: 0.8.1
+Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
+Home-page: https://github.com/sotetsuk/pgx
+Author: Sotetsu KOYAMADA
+Author-email: sotetsu.koyamada@gmail.com
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/logo.svg" width="40%">
 </div>
 
 A collection of GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
@@ -50,14 +63,20 @@
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
 while not (state.terminated | state.truncated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
+Pgx is a library that focuses on faster implementations rather than just the API itself. 
+However, the API itself is also sufficiently general. For example, all environments in Pgx can be converted to the AEC API of [PettingZoo](https://github.com/Farama-Foundation/PettingZoo), and you can run Pgx environments through the PettingZoo API.
+You can see the demonstration in Google Colab:
+
+<a href="https://colab.research.google.com/github/sotetsuk/pgx/blob/main/colab/pgx2pettingzoo.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+
 <!---
 ### Limitations (for the simplicity)
 * Does **NOT** support agent death and creation, which dynmically changes the array size. It does not well suit to GPU-accelerated computation.
 * Does **NOT** support Chance player (Nature player) with action selection.
 * Does **NOT** support OpenAI Gym API.
     * OpenAI Gym is for single-agent environment. Most of Pgx environments are multi-player games. Just defining opponents is not enough for converting multi-agent environemnts to OpenAI Gym environment. E.g., in the game of go, the next state s' is defined as the state just after placing a stone in AlhaGo paper. However, s' becomes the state after the opponents' play. This changes the definition of V(s').
 * Does **NOT** support PettingZoo API.
```

#### html2text {}

```diff
@@ -1,9 +1,15 @@
-[![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/badge.svg)]
-(https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
+Metadata-Version: 2.1 Name: pgx Version: 0.8.1 Summary: GPU/TPU-accelerated
+parallel game simulators for reinforcement learning (RL) Home-page: https://
+github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
+sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
+File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
+badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
   [https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/logo.svg]
 A collection of GPU/TPU-accelerated parallel game simulators for reinforcement
 learning (RL)
        [https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 go_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/
            main/docs/assets/go_dark.gif#gh-dark-mode-only][https://
  raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go_dark.gif#gh-dark-
@@ -24,31 +30,37 @@
 native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
 # vectorized states while not (state.terminated | state.truncated).all():
 action = model(state.current_player, state.observation,
 state.legal_action_mask) state = step(state, action) # state.reward (2,) ```
-## Supported games | Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:
-| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only]|[https:/
-/raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-
-dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+Pgx is a library that focuses on faster implementations rather than just the
+API itself. However, the API itself is also sufficiently general. For example,
+all environments in Pgx can be converted to the AEC API of [PettingZoo](https:/
+/github.com/Farama-Foundation/PettingZoo), and you can run Pgx environments
+through the PettingZoo API. You can see the demonstration in Google Colab:
+[Open_In_Colab]  ## Supported games | Backgammon | Chess | Shogi | Go | |:---:
+|:---:|:---:|:---:| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/backgammon_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
 light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
-`pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available
-games. Given an ``, you can create the environment via ```py >>> env = pgx.make
-() ``` You can check the current version of each environment by ```py >>>
-env.version ``` | Game/EnvId | Visualization | Version | Five-word description
-| |:---:|:---:|:---:|:---:| |2048
+assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
+> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
+can create the environment via ```py >>> env = pgx.make() ``` You can check the
+current version of each environment by ```py >>> env.version ``` | Game/EnvId |
+Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
+| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/animal_shogi_light.gif]| `v0` | *Animal-themed child-friendly
 shogi.* | |Backgammon
```

### Comparing `pgx-0.8.0/pgx/_mahjong/_hand.py` & `pgx-0.8.1/pgx/_mahjong/_hand.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,25 +31,22 @@
                         ),
                         hand[j],
                     )
                 )
         for j in range(4):
             hand = hand.at[j].set(Hand.add(hand[j], deck[-(16 * 3 + j + 1)]))  # type: ignore
 
-        last_draw = deck[-(16 * 3 + 4 + 1)].astype(int)
-        hand = hand.at[0].set(Hand.add(hand[0], last_draw))  # type: ignore
-
         return hand
 
     @staticmethod
-    def cache(code: int):
+    def cache(code):
         return (Hand.CACHE[code >> 5] >> (code & 0b11111)) & 1
 
     @staticmethod
-    def can_ron(hand: jnp.ndarray, tile: int):
+    def can_ron(hand: jnp.ndarray, tile):
         return Hand.can_tsumo(Hand.add(hand, tile))
 
     @staticmethod
     def can_riichi(hand: jnp.ndarray):
         """手牌は14枚"""
         return jax.vmap(
             lambda i: (hand[i] != 0) & Hand.is_tenpai(Hand.sub(hand, i))
@@ -117,31 +114,31 @@
             ),
             (heads, valid),
         )
 
         return ((valid & (heads == 1)) | thirteen_orphan | seven_pairs) == 1
 
     @staticmethod
-    def can_pon(hand: jnp.ndarray, tile: int) -> bool:
+    def can_pon(hand: jnp.ndarray, tile) -> bool:
         return hand[tile] >= 2  # type: ignore
 
     @staticmethod
-    def can_minkan(hand: jnp.ndarray, tile: int) -> bool:
+    def can_minkan(hand: jnp.ndarray, tile) -> bool:
         return hand[tile] == 3  # type: ignore
 
     @staticmethod
-    def can_kakan(hand: jnp.ndarray, tile: int) -> bool:
+    def can_kakan(hand: jnp.ndarray, tile) -> bool:
         return hand[tile] == 1  # type: ignore
 
     @staticmethod
-    def can_ankan(hand: jnp.ndarray, tile: int) -> bool:
+    def can_ankan(hand: jnp.ndarray, tile) -> bool:
         return hand[tile] == 4  # type: ignore
 
     @staticmethod
-    def can_chi(hand: jnp.ndarray, tile: int, action: int) -> bool:
+    def can_chi(hand: jnp.ndarray, tile, action) -> bool:
         return jax.lax.cond(
             (tile >= 27) | (action < Action.CHI_L) | (Action.CHI_R < action),
             lambda: False,
             lambda: jax.lax.switch(
                 action - Action.CHI_L,
                 [
                     lambda: (tile % 9 < 7)
@@ -157,39 +154,39 @@
                     & (hand[tile - 2] > 0)
                     & (hand[tile - 1] > 0),
                 ],
             ),
         )
 
     @staticmethod
-    def add(hand: jnp.ndarray, tile: int, x: int = 1) -> jnp.ndarray:
+    def add(hand: jnp.ndarray, tile, x=1) -> jnp.ndarray:
         return hand.at[tile].set(hand[tile] + x)
 
     @staticmethod
-    def sub(hand: jnp.ndarray, tile: int, x: int = 1) -> jnp.ndarray:
+    def sub(hand: jnp.ndarray, tile, x=1) -> jnp.ndarray:
         return Hand.add(hand, tile, -x)
 
     @staticmethod
-    def pon(hand: jnp.ndarray, tile: int) -> jnp.ndarray:
+    def pon(hand: jnp.ndarray, tile) -> jnp.ndarray:
         return Hand.sub(hand, tile, 2)
 
     @staticmethod
-    def minkan(hand: jnp.ndarray, tile: int) -> jnp.ndarray:
+    def minkan(hand: jnp.ndarray, tile) -> jnp.ndarray:
         return Hand.sub(hand, tile, 3)
 
     @staticmethod
-    def kakan(hand: jnp.ndarray, tile: int) -> jnp.ndarray:
+    def kakan(hand: jnp.ndarray, tile) -> jnp.ndarray:
         return Hand.sub(hand, tile)
 
     @staticmethod
-    def ankan(hand: jnp.ndarray, tile: int) -> jnp.ndarray:
+    def ankan(hand: jnp.ndarray, tile) -> jnp.ndarray:
         return Hand.sub(hand, tile, 4)
 
     @staticmethod
-    def chi(hand: jnp.ndarray, tile: int, action: int) -> jnp.ndarray:
+    def chi(hand: jnp.ndarray, tile, action) -> jnp.ndarray:
         return jax.lax.switch(
             action - Action.CHI_L,
             [
                 lambda: Hand.sub(Hand.sub(hand, tile + 1), tile + 2),
                 lambda: Hand.sub(Hand.sub(hand, tile - 1), tile + 1),
                 lambda: Hand.sub(Hand.sub(hand, tile - 2), tile - 1),
             ],
```

### Comparing `pgx-0.8.0/pgx/_mahjong/_meld.py` & `pgx-0.8.1/pgx/_mahjong/_meld.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_mahjong/_shanten.py` & `pgx-0.8.1/pgx/_mahjong/_shanten.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_mahjong/_yaku.py` & `pgx-0.8.1/pgx/_mahjong/_yaku.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/api_test.py` & `pgx-0.8.1/pgx/_src/api_test.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/assets/between.npy` & `pgx-0.8.1/pgx/_src/assets/between.npy`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/assets/can_move.npy` & `pgx-0.8.1/pgx/_src/assets/can_move.npy`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/chess_utils.py` & `pgx-0.8.1/pgx/_src/chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/animalshogi.py` & `pgx-0.8.1/pgx/_src/dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/backgammon.py` & `pgx-0.8.1/pgx/_src/dwg/backgammon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pgx.backgammon import State as BackgammonState
 from pgx.backgammon import _get_abs_board
 
 
-def _make_backgammon_dwg(dwg, state: BackgammonState, config):
+def _make_backgammon_dwg(dwg, state: BackgammonState, config):  # noqa: C901
     board = _get_abs_board(state)
     BOARD_WIDTH = config["BOARD_WIDTH"]
     BOARD_HEIGHT = config["BOARD_HEIGHT"]
     GRID_SIZE = config["GRID_SIZE"]
     color_set = config["COLOR_SET"]
     # background
     dwg.add(
@@ -100,35 +100,42 @@
                     r=0.5 * GRID_SIZE,
                     stroke=color_set.grid_color,
                     fill=fill_color,
                 )
             )
 
     # bar
-    for i, piece in enumerate(board[24:26]):  # 24:黒, 25:白
-        fill_color = color_set.p2_color
-        delta = 1
-        offset = 0.5
-        if i == 1:
-            piece = -piece
-            fill_color = color_set.p1_color
-            delta = -1
-            offset = -0.5
-        for n in range(piece):
-            board_g.add(
-                dwg.circle(
-                    center=(
-                        6.5 * GRID_SIZE,
-                        (7 + offset + n * delta) * GRID_SIZE,
-                    ),
-                    r=0.5 * GRID_SIZE,
-                    stroke=color_set.grid_color,
-                    fill=fill_color,
-                )
+    # 24:黒
+    piece = board[24]
+    for n in range(piece):
+        board_g.add(
+            dwg.circle(
+                center=(
+                    6.5 * GRID_SIZE,
+                    (7.5 + n) * GRID_SIZE,
+                ),
+                r=0.5 * GRID_SIZE,
+                stroke=color_set.grid_color,
+                fill=color_set.p2_color,
+            )
+        )
+    # 25:白
+    piece = -board[25]
+    for n in range(piece):
+        board_g.add(
+            dwg.circle(
+                center=(
+                    6.5 * GRID_SIZE,
+                    (6.5 - n) * GRID_SIZE,
+                ),
+                r=0.5 * GRID_SIZE,
+                stroke=color_set.grid_color,
+                fill=color_set.p1_color,
             )
+        )
 
     # off
     board_g.add(
         dwg.rect(
             (13 * GRID_SIZE, 0),
             (
                 4 * GRID_SIZE,
@@ -187,8 +194,52 @@
             ),
             fill=color_set.grid_color,
             font_size="34px",
             font_family="serif",
         )
     )
 
+    # dice
+    def _add_dice():
+        DICE = "⚀⚁⚂⚃⚄⚅"
+        if state._playable_dice[2] != -1:
+            for xy in range(4):
+                x = xy // 2
+                y = xy % 2
+
+                if state._playable_dice[y + 2 * x] == -1:
+                    continue
+
+                board_g.add(
+                    dwg.text(
+                        text=f"{DICE[state._playable_dice[y+2*x]]}",
+                        insert=(
+                            (13.5 + x * 1.3) * GRID_SIZE,
+                            (7.0 + y * 1.3) * GRID_SIZE,
+                        ),
+                        fill=color_set.grid_color,
+                        font_size="44px",
+                        font_family="sans serif",
+                    )
+                )
+        else:
+            x = 0
+            for dice in state._playable_dice:
+                if dice == -1:
+                    continue
+                board_g.add(
+                    dwg.text(
+                        text=f"{DICE[dice]}",
+                        insert=(
+                            (13.5 + x * 1.3) * GRID_SIZE,
+                            7.5 * GRID_SIZE,
+                        ),
+                        fill=color_set.grid_color,
+                        font_size="44px",
+                        font_family="sans serif",
+                    )
+                )
+                x += 1
+        return board_g
+
+    board_g = _add_dice()
     return board_g
```

### Comparing `pgx-0.8.0/pgx/_src/dwg/bridge_bidding.py` & `pgx-0.8.1/pgx/_src/dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/chess.py` & `pgx-0.8.1/pgx/_src/dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/connect_four.py` & `pgx-0.8.1/pgx/_src/dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/gardner_chess.py` & `pgx-0.8.1/pgx/_src/dwg/gardner_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/go.py` & `pgx-0.8.1/pgx/_src/dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/hex.py` & `pgx-0.8.1/pgx/_src/dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/LICENSE` & `pgx-0.8.1/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/bBishop.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/bKing.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/bKnight.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/bPawn.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/bQueen.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/bRook.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/wBishop.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/wKing.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/wKnight.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/wPawn.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/wQueen.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/chess/wRook.svg` & `pgx-0.8.1/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/kuhn_poker.py` & `pgx-0.8.1/pgx/_src/dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/leduc_holdem.py` & `pgx-0.8.1/pgx/_src/dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/othello.py` & `pgx-0.8.1/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/play2048.py` & `pgx-0.8.1/pgx/_src/dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/shogi.py` & `pgx-0.8.1/pgx/_src/dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/sparrow_mahjong.py` & `pgx-0.8.1/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/dwg/tictactoe.py` & `pgx-0.8.1/pgx/_src/dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/gardner_chess_utils.py` & `pgx-0.8.1/pgx/_src/gardner_chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/shogi_utils.py` & `pgx-0.8.1/pgx/_src/shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/struct.py` & `pgx-0.8.1/pgx/_src/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/_src/visualizer.py` & `pgx-0.8.1/pgx/_src/visualizer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -426,16 +426,16 @@
                 )
             self._make_dwg_group = _make_hex_dwg  # type:ignore
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
-                    "black",
                     "darkgray",
+                    "black",
                     "white",
                     "white",
                     "#1e1e1e",
                     "gray",
                     "#333333",
                 )
             else:
```

### Comparing `pgx-0.8.0/pgx/animal_shogi.py` & `pgx-0.8.1/pgx/animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/backgammon.py` & `pgx-0.8.1/pgx/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/bridge_bidding.py` & `pgx-0.8.1/pgx/bridge_bidding.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             print("2. Give the path of the dds hash table as an argument")
             sys.exit(1)
 
     def _init(self, key: jax.random.KeyArray) -> State:
         key1, key2, key3 = jax.random.split(key, num=3)
         return _init_by_key(jax.random.choice(key2, self.hash_keys), key3)
 
-    def _step(self, state: v1.State, action: jnp.ndarray) -> State:
+    def _step(self, state: v1.State, action: int) -> State:
         assert isinstance(state, State)
         return _step(state, action, self.hash_keys, self.hash_values)
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
         return _observe(state, player_id)
 
@@ -138,15 +138,14 @@
         return 4
 
     @property
     def _illegal_action_penalty(self) -> float:
         return -7600.0
 
 
-@jax.jit
 def init(rng: jax.random.KeyArray) -> State:
     rng1, rng2, rng3, rng4, rng5, rng6 = jax.random.split(rng, num=6)
     hand = jnp.arange(0, 52)
     hand = jax.random.permutation(rng2, hand)
     vul_NS = jax.random.choice(rng3, jnp.bool_([False, True]))
     vul_EW = jax.random.choice(rng4, jnp.bool_([False, True]))
     dealer = jax.random.randint(rng5, (1,), 0, 4, dtype=jnp.int8)[0]
@@ -165,15 +164,14 @@
         _vul_NS=vul_NS,
         _vul_EW=vul_EW,
         legal_action_mask=legal_actions,
     )
     return state
 
 
-@jax.jit
 def _init_by_key(key: jnp.ndarray, rng: jax.random.KeyArray) -> State:
     """Make init state from key"""
     rng1, rng2, rng3, rng4, rng5 = jax.random.split(rng, num=5)
     hand = _key_to_hand(key)
     vul_NS = jax.random.choice(rng2, jnp.bool_([False, True]))
     vul_EW = jax.random.choice(rng3, jnp.bool_([False, True]))
     dealer = jax.random.randint(rng4, (1,), 0, 4, dtype=jnp.int8)[0]
@@ -192,15 +190,14 @@
         _vul_NS=vul_NS,
         _vul_EW=vul_EW,
         legal_action_mask=legal_actions,
     )
     return state
 
 
-@jax.jit
 def _shuffle_players(rng: jax.random.KeyArray) -> jnp.ndarray:
     """Randomly arranges player IDs in a list in NESW order.
 
     Returns:
         jnp.ndarray: A list of 4 player IDs randomly arranged in NESW order.
 
     Example:
@@ -237,26 +234,24 @@
                 team_b_players[1],
                 team_a_players[1],
             ]
         ),
     )
 
 
-@jax.jit
 def _player_position(player: jnp.ndarray, state: State) -> jnp.ndarray:
     return jax.lax.cond(
         player != -1,
         lambda: jnp.int8(
             jnp.argmax(state._shuffled_players == player)
         ),  # playerと同じ要素のstate.shuffle_playersのindexを返す
         lambda: jnp.int8(-1),
     )
 
 
-@jax.jit
 def _step(
     state: State,
     action: int,
     hash_keys: jnp.ndarray,
     hash_values: jnp.ndarray,
 ) -> State:
     # fmt: off
@@ -278,15 +273,14 @@
                 lambda: _continue_step(_state_XX(state)),
             ],
         ),
         lambda: _continue_step(_state_bid(state, action)),
     )
 
 
-@jax.jit
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
     """Returns the observation of a given player"""
     # make vul of observation
     is_player_vul, is_non_player_vul = jax.lax.cond(
         (_player_position(state.current_player, state) == 0)
         | (_player_position(state.current_player, state) == 2),
         lambda: (state._vul_NS, state._vul_EW),
@@ -317,15 +311,14 @@
         state._turn.astype(jnp.int32),
         _make_obs_history,
         (state, player_id, last_bid, obs_history),
     )
     return jnp.concatenate((vul, obs_history, hand))
 
 
-@jax.jit
 def _make_obs_history(turn, vuls):
     state, player_id, last_bid, obs_history = vuls
     action = state._bidding_history[turn]
     relative_bidder = (
         (turn + state._dealer.astype(jnp.int32)) % 4
         + (4 - _player_position(player_id, state).astype(jnp.int32))
     ) % 4
@@ -368,27 +361,25 @@
                 4 + (action - BID_OFFSET_NUM) * 4 * 3 + relative_bidder
             ].set(True),
         ),
     )
     return state, player_id, last_bid, obs_history
 
 
-@jax.jit
-def _convert_card_pgx_to_openspiel(card: int) -> jnp.ndarray:
+def _convert_card_pgx_to_openspiel(card: jnp.ndarray) -> jnp.ndarray:
     """Convert numerical representation of cards from pgx to openspiel"""
     OPEN_SPIEL_SUIT_NUM = jnp.array([3, 2, 1, 0], dtype=jnp.int32)
     OPEN_SPIEL_RANK_NUM = jnp.array(
         [12, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], dtype=jnp.int32
     )
     suit = OPEN_SPIEL_SUIT_NUM[card // 13]
     rank = OPEN_SPIEL_RANK_NUM[card % 13]
     return suit + rank * 4
 
 
-@jax.jit
 def duplicate(
     init_state: State,
 ) -> State:
     """Make duplicated state where NSplayer and EWplayer are swapped"""
     duplicated_state = copy.deepcopy(init_state)
     ix = jnp.array([1, 0, 3, 2])
     # fmt: off
@@ -396,29 +387,27 @@
         _shuffled_players=duplicated_state._shuffled_players[ix],
         current_player=duplicated_state._shuffled_players[ix][duplicated_state._dealer]
     )
     # fmt: on
     return duplicated_state
 
 
-@jax.jit
 def _terminated_step(
     state: State,
     hash_keys: jnp.ndarray,
     hash_values: jnp.ndarray,
 ) -> State:
     """Return state if the game is successfully completed"""
     terminated = jnp.bool_(True)
     reward = _reward(state, hash_keys, hash_values)
     # fmt: off
     return state.replace(terminated=terminated, rewards=reward)  # type: ignore
     # fmt: on
 
 
-@jax.jit
 def _continue_step(
     state: State,
 ) -> State:
     """Return state when the game continues"""
     # fmt: off
     # 次ターンのプレイヤー、ターン数
     state = state.replace(  # type: ignore
@@ -430,28 +419,26 @@
     return state.replace(  # type: ignore
         legal_action_mask=state.legal_action_mask.at[PASS_ACTION_NUM].set(True).at[DOUBLE_ACTION_NUM].set(x_mask).at[REDOUBLE_ACTION_NUM].set(xx_mask),
         rewards=jnp.zeros(4, dtype=jnp.float32)
     )
     # fmt: on
 
 
-@jax.jit
 def _is_terminated(state: State) -> bool:
     """Check if the game is finished
     Four consecutive passes if not bid (pass out), otherwise three consecutive passes
     """
     return jax.lax.cond(
         ((state._last_bid == -1) & (state._pass_num == 4))
         | ((state._last_bid != -1) & (state._pass_num == 3)),
         lambda: True,
         lambda: False,
     )
 
 
-@jax.jit
 def _reward(
     state: State,
     hash_keys: jnp.ndarray,
     hash_values: jnp.ndarray,
 ) -> jnp.ndarray:
     """Return reward
     If pass out, 0 reward for everyone; if bid, calculate and return reward
@@ -461,15 +448,14 @@
         lambda: jnp.zeros(4, dtype=jnp.float32),  # pass out
         lambda: _make_reward(  # caluculate reward
             state, hash_keys, hash_values
         ),
     )
 
 
-@jax.jit
 def _make_reward(
     state: State,
     hash_keys: jnp.ndarray,
     hash_values: jnp.ndarray,
 ) -> jnp.ndarray:
     """Calculate rewards for each player by dds results
 
@@ -498,15 +484,14 @@
     partners = jax.vmap(lambda pos: _is_partner(pos, declare_position))(
         player_positions
     )
 
     return jnp.where(partners, score, -score)
 
 
-@jax.jit
 def _calc_score(
     denomination: jnp.ndarray,
     level: jnp.ndarray,
     vul: jnp.ndarray,
     call_x: jnp.ndarray,
     call_xx: jnp.ndarray,
     trick: jnp.ndarray,
@@ -518,15 +503,14 @@
     return jax.lax.cond(
         level + 6 > trick,
         lambda: _down_score(level, vul, call_x, call_xx, trick),
         lambda: _make_score(denomination, level, vul, call_x, call_xx, trick),
     )
 
 
-@jax.jit
 def _down_score(
     level: jnp.ndarray,
     vul: jnp.ndarray,
     call_x: jnp.ndarray,
     call_xx: jnp.ndarray,
     trick: jnp.ndarray,
 ) -> jnp.ndarray:
@@ -561,15 +545,14 @@
     return jax.lax.cond(
         call_xx,
         lambda: down_xx,
         lambda: jax.lax.cond(call_x, lambda: down_x, lambda: down),
     )
 
 
-@jax.jit
 def _make_score(
     denomination: jnp.ndarray,
     level: jnp.ndarray,
     vul: jnp.ndarray,
     call_x: jnp.ndarray,
     call_xx: jnp.ndarray,
     trick: jnp.ndarray,
@@ -666,15 +649,14 @@
             lambda: (score + _MAKE_X, overtrick_x),
         ),
         lambda: (score, over_trick_score_per_trick),
     )
     return score + over_trick_score_per_trick * over_trick
 
 
-@jax.jit
 def _contract(
     state: State,
 ) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray, jnp.ndarray]:
     """Return Contract which has position of declare ,denomination, level"""
     denomination = state._last_bid % 5
     level = state._last_bid // 5 + 1
     declare_position, vul = jax.lax.cond(
@@ -691,35 +673,31 @@
             ),
             state._vul_EW,
         ),
     )
     return declare_position, denomination, level, vul
 
 
-@jax.jit
 def _state_pass(
     state: State,
 ) -> State:
     """Change state if pass is taken"""
     return state.replace(_pass_num=state._pass_num + 1)  # type: ignore
 
 
-@jax.jit
 def _state_X(state: State) -> State:
     """Change state if double(X) is taken"""
     return state.replace(_call_x=jnp.bool_(True), _pass_num=jnp.int32(0))  # type: ignore
 
 
-@jax.jit
 def _state_XX(state: State) -> State:
     """Change state if double(XX) is taken"""
     return state.replace(_call_xx=jnp.bool_(True), _pass_num=jnp.int32(0))  # type: ignore
 
 
-@jax.jit
 def _state_bid(state: State, action: int) -> State:
     """Change state if bid is taken"""
     # 最後のbidとそのプレイヤーを保存
     bid = action - BID_OFFSET_NUM
     # fmt: off
     state = state.replace(_last_bid=bid, _last_bidder=state.current_player)  # type: ignore
     # fmt: on
@@ -744,41 +722,37 @@
         ),
         _call_x=jnp.bool_(False),
         _call_xx=jnp.bool_(False),
         _pass_num=jnp.int32(0),
     )
 
 
-@jax.jit
 def _bid_to_denomination(bid: int) -> int:
     """Calcularete denomination of bid"""
     return bid % 5
 
 
-@jax.jit
 def _position_to_team(position: jnp.ndarray) -> jnp.ndarray:
     """Determine which team from the position
     0: NS team, 1: EW team
     """
     return position % 2
 
 
-@jax.jit
 def _update_legal_action_X_XX(
     state: State,
 ) -> Tuple[bool, bool]:
     """Determine if X or XX is a legal move for the next player"""
     return jax.lax.cond(
         state._last_bidder != -1,
         lambda: (_is_legal_X(state), _is_legal_XX(state)),
         lambda: (False, False),
     )
 
 
-@jax.jit
 def _is_legal_X(state: State) -> bool:
     return jax.lax.cond(
         (state._call_x == 0)
         & (state._call_xx == 0)
         & (
             _is_partner(
                 _player_position(state._last_bidder, state),
@@ -787,15 +761,14 @@
             == 0
         ),
         lambda: True,
         lambda: False,
     )
 
 
-@jax.jit
 def _is_legal_XX(state: State) -> bool:
     return jax.lax.cond(
         state._call_x
         & (state._call_xx == 0)
         & (
             _is_partner(
                 _player_position(state._last_bidder, state),
@@ -803,15 +776,14 @@
             )
         ),
         lambda: True,
         lambda: False,
     )
 
 
-@jax.jit
 def _is_partner(position1: jnp.ndarray, position2: jnp.ndarray) -> jnp.ndarray:
     """Determine if positon1 and position2 belong to the same team"""
     return (abs(position1 - position2) + 1) % 2
 
 
 def _state_to_pbn(state: State) -> str:
     """Convert state to pbn format"""
@@ -829,21 +801,19 @@
                 if i != 3:
                     pbn += " "
             else:
                 pbn += "."
     return pbn
 
 
-@jax.jit
 def _state_to_key(state: State) -> jnp.ndarray:
     """Convert state to key of dds table"""
     hand = state._hand
-    key = jnp.zeros(52, dtype=jnp.int8)
-    for i in range(52):  # N: 0, E: 1, S: 2, W: 3
-        key = key.at[hand[i]].set(i // 13)
+    key = jnp.zeros(52, dtype=jnp.int32)
+    key = key.at[hand].set(jnp.arange(52, dtype=jnp.int32) // 13)
     key = key.reshape(4, 13)
     return _to_binary(key)
 
 
 def _pbn_to_key(pbn: str) -> jnp.ndarray:
     """Convert pbn to key of dds table"""
     key = jnp.zeros(52, dtype=jnp.int8)
@@ -853,17 +823,17 @@
             for card in cards:  # for each card
                 card_num = _card_str_to_int(card) + suit * 13
                 key[card_num] = player
     key = key.reshape(4, 13)
     return _to_binary(key)
 
 
-@jax.jit
 def _to_binary(x: jnp.ndarray) -> jnp.ndarray:
-    bases = jnp.array([4**i for i in range(13)], dtype=jnp.int32)[::-1]
+    # bases = jnp.array([4**i for i in range(13)], dtype=jnp.int32)[::-1]
+    bases = (4 ** jnp.arange(13))[::-1]
     return (x * bases).sum(axis=1)  # shape = (4, )
 
 
 def _card_str_to_int(card: str) -> int:
     if card == "K":
         return 12
     elif card == "Q":
@@ -874,37 +844,42 @@
         return 9
     elif card == "A":
         return 0
     else:
         return int(card) - 1
 
 
-@jax.jit
 def _key_to_hand(key: jnp.ndarray) -> jnp.ndarray:
     """Convert key to hand"""
 
     def _convert_quat(j):
         shifts = jnp.arange(24, -1, step=-2)
         quat_digits = (j >> shifts) & 0b11
         return quat_digits
 
     cards = jax.vmap(_convert_quat)(key).flatten()
     hand = jnp.zeros((4, 13), dtype=jnp.int32)
-    for i in range(4):
-        count = 0
-        for j in range(52):
-            hand, count = jax.lax.cond(
-                cards[j] == i,
-                lambda: (hand.at[i, count].set(j), count + 1),
-                lambda: (hand, count),
-            )
+
+    def loop_j(j, val):
+        i, count, (hand, card) = val
+        hand, count = jax.lax.cond(
+            cards[j] == i,
+            lambda: (hand.at[i, count].set(j), count + 1),
+            lambda: (hand, count),
+        )
+        return i, count, (hand, card)
+
+    def loop_i(i, val):
+        i, count, val = jax.lax.fori_loop(0, 52, loop_j, (i, 0, val))
+        return val
+
+    hand, _ = jax.lax.fori_loop(0, 4, loop_i, (hand, cards))
     return hand.flatten()
 
 
-@jax.jit
 def _value_to_dds_tricks(value: jnp.ndarray) -> jnp.ndarray:
     """Convert values to dds tricks
     >>> value = jnp.array([4160, 904605, 4160, 904605])
     >>> _value_to_dds_tricks(value)
     Array([ 0,  1,  0,  4,  0, 13, 12, 13,  9, 13,  0,  1,  0,  4,  0, 13, 12,
            13,  9, 13], dtype=int32)
     """
@@ -914,27 +889,25 @@
         hex_digits = (j >> shifts) & 0xF
         return hex_digits
 
     hex_digits = jax.vmap(_convert_hex)(value).flatten()
     return jnp.array(hex_digits, dtype=jnp.int32)
 
 
-@jax.jit
 def _calculate_dds_tricks(
     state: State,
     hash_keys: jnp.ndarray,
     hash_values: jnp.ndarray,
 ) -> jnp.ndarray:
     key = _state_to_key(state)
     return _value_to_dds_tricks(
         _find_value_from_key(key, hash_keys, hash_values)
     )
 
 
-@jax.jit
 def _find_value_from_key(
     key: jnp.ndarray, hash_keys: jnp.ndarray, hash_values: jnp.ndarray
 ):
     """Find a value matching key without batch processing
     >>> VALUES = jnp.arange(20).reshape(5, 4)
     >>> KEYS = jnp.arange(20).reshape(5, 4)
     >>> key = jnp.arange(4, 8)
```

### Comparing `pgx-0.8.0/pgx/chess.py` & `pgx-0.8.1/pgx/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/connect_four.py` & `pgx-0.8.1/pgx/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/experimental/bridge_bidding.py` & `pgx-0.8.1/pgx/experimental/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/experimental/gym.py` & `pgx-0.8.1/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/experimental/visualize.py` & `pgx-0.8.1/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/gardner_chess.py` & `pgx-0.8.1/pgx/gardner_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/go.py` & `pgx-0.8.1/pgx/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/hex.py` & `pgx-0.8.1/pgx/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/kuhn_poker.py` & `pgx-0.8.1/pgx/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/leduc_holdem.py` & `pgx-0.8.1/pgx/leduc_holdem.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,26 +143,28 @@
         _round=state._round + jnp.int8(round_over),
         _chips=chips,
         _raise_count=raise_count,
     )
 
 
 def _check_round_over(state, action):
-    round_over = (action == FOLD) | (
-        (state._last_action != INVALID_ACTION) & (action == CALL)
-    )
-    terminated = round_over & (state._round == 1)
+    fold = action == FOLD
+    call = (state._last_action != INVALID_ACTION) & (action == CALL)
+    _continue = (state._round == 0) & call
+
+    round_over = fold | call
+    terminated = round_over & (~_continue)
 
     reward = jax.lax.select(
-        terminated & (action == FOLD),
+        fold,
         jnp.float32([-1, -1]).at[1 - state.current_player].set(1),
         jnp.float32([0, 0]),
     )
     reward = jax.lax.select(
-        terminated & (action != FOLD),
+        terminated & call,
         _get_unit_reward(state),
         reward,
     )
     return round_over, terminated, reward
 
 
 def _get_unit_reward(state: State):
```

### Comparing `pgx-0.8.0/pgx/minatar/asterix.py` & `pgx-0.8.1/pgx/minatar/asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/minatar/breakout.py` & `pgx-0.8.1/pgx/minatar/breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/minatar/freeway.py` & `pgx-0.8.1/pgx/minatar/freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/minatar/seaquest.py` & `pgx-0.8.1/pgx/minatar/seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/minatar/space_invaders.py` & `pgx-0.8.1/pgx/minatar/space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/minatar/utils.py` & `pgx-0.8.1/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/othello.py` & `pgx-0.8.1/pgx/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/play2048.py` & `pgx-0.8.1/pgx/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/shogi.py` & `pgx-0.8.1/pgx/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/sparrow_mahjong.py` & `pgx-0.8.1/pgx/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/tic_tac_toe.py` & `pgx-0.8.1/pgx/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx/v1.py` & `pgx-0.8.1/pgx/v1.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/pgx.egg-info/PKG-INFO` & `pgx-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pgx
-Version: 0.8.0
-Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
-Home-page: https://github.com/sotetsuk/pgx
-Author: Sotetsu KOYAMADA
-Author-email: sotetsu.koyamada@gmail.com
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/logo.svg" width="40%">
 </div>
 
 A collection of GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
@@ -63,14 +50,20 @@
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
 while not (state.terminated | state.truncated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
+Pgx is a library that focuses on faster implementations rather than just the API itself. 
+However, the API itself is also sufficiently general. For example, all environments in Pgx can be converted to the AEC API of [PettingZoo](https://github.com/Farama-Foundation/PettingZoo), and you can run Pgx environments through the PettingZoo API.
+You can see the demonstration in Google Colab:
+
+<a href="https://colab.research.google.com/github/sotetsuk/pgx/blob/main/colab/pgx2pettingzoo.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+
 <!---
 ### Limitations (for the simplicity)
 * Does **NOT** support agent death and creation, which dynmically changes the array size. It does not well suit to GPU-accelerated computation.
 * Does **NOT** support Chance player (Nature player) with action selection.
 * Does **NOT** support OpenAI Gym API.
     * OpenAI Gym is for single-agent environment. Most of Pgx environments are multi-player games. Just defining opponents is not enough for converting multi-agent environemnts to OpenAI Gym environment. E.g., in the game of go, the next state s' is defined as the state just after placing a stone in AlhaGo paper. However, s' becomes the state after the opponents' play. This changes the definition of V(s').
 * Does **NOT** support PettingZoo API.
```

#### html2text {}

```diff
@@ -1,15 +1,9 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.8.0 Summary: GPU/TPU-accelerated
-parallel game simulators for reinforcement learning (RL) Home-page: https://
-github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
-sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
-File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
-badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
+[![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/badge.svg)]
+(https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
   [https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/logo.svg]
 A collection of GPU/TPU-accelerated parallel game simulators for reinforcement
 learning (RL)
        [https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 go_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/
            main/docs/assets/go_dark.gif#gh-dark-mode-only][https://
  raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go_dark.gif#gh-dark-
@@ -30,31 +24,37 @@
 native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
 # vectorized states while not (state.terminated | state.truncated).all():
 action = model(state.current_player, state.observation,
 state.legal_action_mask) state = step(state, action) # state.reward (2,) ```
-## Supported games | Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:
-| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only]|[https:/
-/raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-
-dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+Pgx is a library that focuses on faster implementations rather than just the
+API itself. However, the API itself is also sufficiently general. For example,
+all environments in Pgx can be converted to the AEC API of [PettingZoo](https:/
+/github.com/Farama-Foundation/PettingZoo), and you can run Pgx environments
+through the PettingZoo API. You can see the demonstration in Google Colab:
+[Open_In_Colab]  ## Supported games | Backgammon | Chess | Shogi | Go | |:---:
+|:---:|:---:|:---:| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/backgammon_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
 light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
-`pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available
-games. Given an ``, you can create the environment via ```py >>> env = pgx.make
-() ``` You can check the current version of each environment by ```py >>>
-env.version ``` | Game/EnvId | Visualization | Version | Five-word description
-| |:---:|:---:|:---:|:---:| |2048
+assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
+> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
+can create the environment via ```py >>> env = pgx.make() ``` You can check the
+current version of each environment by ```py >>> env.version ``` | Game/EnvId |
+Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
+| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/animal_shogi_light.gif]| `v0` | *Animal-themed child-friendly
 shogi.* | |Backgammon
```

### Comparing `pgx-0.8.0/pgx.egg-info/SOURCES.txt` & `pgx-0.8.1/pgx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 pgx/__init__.py
 pgx/animal_shogi.py
 pgx/backgammon.py
+pgx/baseline.py
 pgx/bridge_bidding.py
 pgx/chess.py
 pgx/connect_four.py
 pgx/gardner_chess.py
 pgx/go.py
 pgx/hex.py
 pgx/kuhn_poker.py
@@ -23,24 +24,26 @@
 pgx.egg-info/SOURCES.txt
 pgx.egg-info/dependency_links.txt
 pgx.egg-info/requires.txt
 pgx.egg-info/top_level.txt
 pgx/_mahjong/__init__.py
 pgx/_mahjong/_action.py
 pgx/_mahjong/_hand.py
+pgx/_mahjong/_mahjong.py
 pgx/_mahjong/_meld.py
 pgx/_mahjong/_shanten.py
 pgx/_mahjong/_yaku.py
 pgx/_mahjong/cache/__init__.py
 pgx/_src/__init__.py
 pgx/_src/api_test.py
 pgx/_src/chess_utils.py
 pgx/_src/gardner_chess_utils.py
 pgx/_src/shogi_utils.py
 pgx/_src/struct.py
+pgx/_src/utils.py
 pgx/_src/visualizer.py
 pgx/_src/assets/between.npy
 pgx/_src/assets/can_move.npy
 pgx/_src/dwg/__init__.py
 pgx/_src/dwg/animalshogi.py
 pgx/_src/dwg/backgammon.py
 pgx/_src/dwg/bridge_bidding.py
@@ -93,29 +96,29 @@
 pgx/_src/dwg/images/sparrow_mahjong/b.svg
 pgx/_src/dwg/images/sparrow_mahjong/gd.svg
 pgx/_src/dwg/images/sparrow_mahjong/oya.svg
 pgx/_src/dwg/images/sparrow_mahjong/rd.svg
 pgx/experimental/__init__.py
 pgx/experimental/bridge_bidding.py
 pgx/experimental/gym.py
-pgx/experimental/pettingzoo.py
 pgx/experimental/utils.py
 pgx/experimental/visualize.py
 pgx/minatar/__init__.py
 pgx/minatar/asterix.py
 pgx/minatar/breakout.py
 pgx/minatar/freeway.py
 pgx/minatar/seaquest.py
 pgx/minatar/space_invaders.py
 pgx/minatar/utils.py
 tests/__init__.py
 tests/minatar_utils.py
 tests/test_animal_shogi.py
 tests/test_asterix.py
 tests/test_backgammon.py
+tests/test_baseline.py
 tests/test_breakout.py
 tests/test_bridge_bidding.py
 tests/test_chess.py
 tests/test_connect_four.py
 tests/test_freeway.py
 tests/test_gardner_chess.py
 tests/test_go.py
```

### Comparing `pgx-0.8.0/pyproject.toml` & `pgx-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/setup.py` & `pgx-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/minatar_utils.py` & `pgx-0.8.1/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_animal_shogi.py` & `pgx-0.8.1/tests/test_animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_asterix.py` & `pgx-0.8.1/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_backgammon.py` & `pgx-0.8.1/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_breakout.py` & `pgx-0.8.1/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_bridge_bidding.py` & `pgx-0.8.1/tests/test_bridge_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,28 @@
     os.path.dirname(__file__), "assets/dds_hash_table.npy"
 )
 env = BridgeBidding(dds_hash_table_path=DDS_HASH_TABLE_PATH)
 
 init_by_key = jax.jit(env.init)
 step = jax.jit(env.step)
 observe = jax.jit(env.observe)
+_calc_score = jax.jit(_calc_score)
+_calculate_dds_tricks = jax.jit(_calculate_dds_tricks)
+_contract = jax.jit(_contract)
+_init_by_key = jax.jit(_init_by_key)
+_key_to_hand = jax.jit(_key_to_hand)
+_load_sample_hash = jax.jit(_load_sample_hash)
+_pbn_to_key = jax.jit(_pbn_to_key)
+_player_position = jax.jit(_player_position)
+_shuffle_players = jax.jit(_shuffle_players)
+_state_to_key = jax.jit(_state_to_key)
+_to_binary = jax.jit(_to_binary)
+_value_to_dds_tricks = jax.jit(_value_to_dds_tricks)
+duplicate = jax.jit(duplicate)
+init = jax.jit(init)
 
 
 def test_shuffle_players():
     key = jax.random.PRNGKey(0)
     for i in range(100):
         key, subkey = jax.random.split(key)
         shuffled_players = _shuffle_players(subkey)
```

### Comparing `pgx-0.8.0/tests/test_chess.py` & `pgx-0.8.1/tests/test_chess.py`

 * *Files 8% similar despite different names*

```diff
@@ -951,12 +951,133 @@
     state.save_svg("tests/assets/chess/observe_032.svg")
     assert (state.observation[:, :, 118] == 0).all()
     # pawn move
     state = step(state, jnp.int32(90))
     state.save_svg("tests/assets/chess/observe_032.svg")
     assert (state.observation[:, :, 118] == 0).all()
 
+    # repetition observation
+    # normal
+    state = State._from_fen("r3k2r/8/8/8/8/8/8/R3K2R w - - 0 1")
+    state.save_svg("tests/assets/chess/observe_033.svg")
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/observe_034.svg")
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/observe_035.svg")
+    state = step(state, jnp.int32(613))
+    state.save_svg("tests/assets/chess/observe_036.svg")
+    state = step(state, jnp.int32(613))
+    state.save_svg("tests/assets/chess/observe_037.svg")
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    state = step(state, jnp.int32(30))
+    # "tests/assets/chess/observe_034.svg"
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 13] == 1.).all()  # rep
+    state = step(state, jnp.int32(30))
+    # "tests/assets/chess/observe_035.svg"
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 13] == 1.).all()  # rep
+    state = step(state, jnp.int32(613))
+    # "tests/assets/chess/observe_036.svg"
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 3 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 3 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 7 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 7 + 13] == 1.).all()  # rep
+
+    # with castling rights
+    state = State._from_fen("r3k2r/8/8/8/8/8/8/R3K2R w KQkq - 0 1")
+    # "tests/assets/chess/observe_033.svg"
+    state = step(state, jnp.int32(30))
+    # "tests/assets/chess/observe_034.svg"
+    state = step(state, jnp.int32(30))
+    # "tests/assets/chess/observe_035.svg"
+    state = step(state, jnp.int32(613))
+    # "tests/assets/chess/observe_036.svg"
+    state = step(state, jnp.int32(613))
+    # "tests/assets/chess/observe_037.svg"
+    assert (state.observation[:, :, 14 * 0 + 12] == 1).all()
+    assert (state.observation[:, :, 14 * 0 + 13] == 0).all()
+    assert (state.observation[:, :, 14 * 4 + 12] == 1).all()
+    assert (state.observation[:, :, 14 * 4 + 13] == 0).all()
+    state = step(state, jnp.int32(30))
+    # "tests/assets/chess/observe_034.svg"
+    assert (state.observation[:, :, 14 * 0 + 12] == 1).all()
+    assert (state.observation[:, :, 14 * 0 + 13] == 0).all()
+    assert (state.observation[:, :, 14 * 4 + 12] == 1).all()
+    assert (state.observation[:, :, 14 * 4 + 13] == 0).all()
+    state = step(state, jnp.int32(30))
+    # "tests/assets/chess/observe_035.svg"
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    state = step(state, jnp.int32(613))
+    # "tests/assets/chess/observe_036.svg"
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 13] == 1.).all()  # rep
+
+    # with en-passant
+    state = State._from_fen("r3k2r/8/8/8/8/8/P7/R3K2R w - - 0 1")
+    state.save_svg("tests/assets/chess/observe_038.svg")
+    state = step(state, jnp.int32(90))
+    state.save_svg("tests/assets/chess/observe_039.svg")
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/observe_040.svg")
+    state = step(state, jnp.int32(30))
+    state.save_svg("tests/assets/chess/observe_041.svg")
+    state = step(state, jnp.int32(613))
+    state.save_svg("tests/assets/chess/observe_042.svg")
+    state = step(state, jnp.int32(613))
+    state.save_svg("tests/assets/chess/observe_043.svg")
+    assert (state.observation[:, :, 14 * 0 + 12] == 1).all()
+    assert (state.observation[:, :, 14 * 0 + 13] == 0).all()
+    assert (state.observation[:, :, 14 * 4 + 12] == 1).all()
+    assert (state.observation[:, :, 14 * 4 + 13] == 0).all()
+    state = step(state, jnp.int32(30))
+    # "tests/assets/chess/observe_039.svg"
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+
 
 def test_api():
     import pgx
     env = pgx.make("chess")
     pgx.v1_api_test(env, 5)
```

### Comparing `pgx-0.8.0/tests/test_connect_four.py` & `pgx-0.8.1/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_freeway.py` & `pgx-0.8.1/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_gardner_chess.py` & `pgx-0.8.1/tests/test_gardner_chess.py`

 * *Files 16% similar despite different names*

```diff
@@ -340,14 +340,135 @@
     assert (state.observation[:, :, 0] == expected_wpawn1).all()
     assert (state.observation[:, :, 112] == 1).all()
     state = step(state, 1042)
     state.save_svg("tests/assets/gardner_chess/observe_019.svg")
     assert (state.observation[:, :, 0] == expected_wpawn2).all()
     assert (state.observation[:, :, 112] == 0).all()
 
+    # check repetition observation
+    state = init(jax.random.PRNGKey(0))
+    state = step(state, jnp.int32(293))
+    state.save_svg("tests/assets/gardner_chess/observe_020.svg")
+    state = step(state, jnp.int32(289))
+    state.save_svg("tests/assets/gardner_chess/observe_021.svg")
+    state = step(state, jnp.int32(631))
+    state.save_svg("tests/assets/gardner_chess/observe_022.svg")
+    state = step(state, jnp.int32(145))
+    state.save_svg("tests/assets/gardner_chess/observe_023.svg")
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 1 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 2 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 2 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 3 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 3 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    state = step(state, jnp.int32(293))
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 2 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 3 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 3 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 13] == 1.).all()  # rep
+    state = step(state, jnp.int32(289))
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 3 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 3 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 13] == 1.).all()  # rep
+    state = step(state, jnp.int32(631))
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 3 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 3 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 7 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 7 + 13] == 1.).all()  # rep
+    state = step(state, jnp.int32(307))
+    state.save_svg("tests/assets/gardner_chess/observe_024.svg")
+    assert (state.observation[:, :, 14 * 0 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 0 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 1 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 3 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 3 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 6 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 7 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 7 + 13] == 1.).all()  # rep
+
+    state = init(jax.random.PRNGKey(0))
+    state = step(state, jnp.int32(293))
+    # "tests/assets/gardner_chess/observe_020.svg"
+    state = step(state, jnp.int32(289))
+    # "tests/assets/gardner_chess/observe_021.svg"
+    state = step(state, jnp.int32(631))
+    # "tests/assets/gardner_chess/observe_022.svg"
+    state = step(state, jnp.int32(21))
+    state.save_svg("tests/assets/gardner_chess/observe_025.svg")
+    state = step(state, jnp.int32(293))
+    state.save_svg("tests/assets/gardner_chess/observe_026.svg")
+    state = step(state, jnp.int32(265))
+    state.save_svg("tests/assets/gardner_chess/observe_027.svg")
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 1 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 2 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 2 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 3 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 3 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    state = step(state, jnp.int32(631))
+    state.save_svg("tests/assets/gardner_chess/observe_028.svg")
+    assert (state.observation[:, :, 14 * 0 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 0 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 1 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 2 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 2 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 3 + 12] == 1.).all()
+    assert (state.observation[:, :, 14 * 3 + 13] == 0.).all()
+    assert (state.observation[:, :, 14 * 4 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 4 + 13] == 1.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 12] == 0.).all()  # rep
+    assert (state.observation[:, :, 14 * 5 + 13] == 1.).all()  # rep
 
 def test_step():
     # normal step
     # queen
     state = State._from_fen("k4/5/5/1Q3/4K w - - 0 1")
     state.save_svg("tests/assets/gardner_chess/step_001.svg")
     assert state._board[p("b1")] == EMPTY
```

### Comparing `pgx-0.8.0/tests/test_go.py` & `pgx-0.8.1/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_hex.py` & `pgx-0.8.1/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_kuhn_poker.py` & `pgx-0.8.1/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_leduc_holdem.py` & `pgx-0.8.1/tests/test_leduc_holdem.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,54 @@
     assert state.current_player == 0
     assert (state.legal_action_mask == jnp.bool_([1, 1, 0])).all()
 
 
 def test_step():
     key = jax.random.PRNGKey(1)
 
+    # =================
+    state = init(key)
+    assert state.current_player == 1
+    # cards = [1 0]
+    # player 1 is the first
+
+    # first round
+    state = step(state, RAISE)
+    state = step(state, FOLD)
+    assert state.terminated
+    assert (state.rewards == jnp.float32([-1, 1])).all()
+
+    # =================
+    state = init(key)
+    assert state.current_player == 1
+    # cards = [1 0]
+    # player 1 is the first
+
+    # first round
+    state = step(state, RAISE)  # +2(3)
+    state = step(state, RAISE)  # +2(5)
+    state = step(state, FOLD)
+    assert state.terminated
+    assert (state.rewards == jnp.float32([3, -3])).all()
+
+    # =================
+    state = init(key)
+    assert state.current_player == 1
+    # cards = [1 0]
+    # player 1 is the first
+
+    # first round
+    state = step(state, CALL)
+    state = step(state, RAISE)  # +2(3)
+    state = step(state, RAISE)  # +2(5)
+    state = step(state, FOLD)
+    assert state.terminated
+    assert (state.rewards == jnp.float32([-3, 3])).all()
+
+    # =================
     state = init(key)
     assert state.current_player == 1
     # cards = [1 0]
     # player 1 is the first
 
     # first round
     state = step(state, CALL)
@@ -34,14 +74,15 @@
     state = step(state, RAISE)  # +4(7)
     state = step(state, RAISE)  # +4(11)
     assert not state.terminated
     state = step(state, CALL)
     assert state.terminated
     assert (state.rewards == jnp.float32([11, -11])).all()
 
+    # =================
     state = init(key)
     assert state.current_player == 1
     # cards = [1 0]
     # player 1 is the first
 
     # first round
     state = step(state, CALL)
```

### Comparing `pgx-0.8.0/tests/test_othello.py` & `pgx-0.8.1/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_play2048.py` & `pgx-0.8.1/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_seaquest.py` & `pgx-0.8.1/tests/test_seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_shogi.py` & `pgx-0.8.1/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_space_invaders.py` & `pgx-0.8.1/tests/test_space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_sparrow_mahjong.py` & `pgx-0.8.1/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.0/tests/test_tic_tac_toe.py` & `pgx-0.8.1/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

