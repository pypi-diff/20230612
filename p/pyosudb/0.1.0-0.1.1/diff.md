# Comparing `tmp/pyosudb-0.1.0.tar.gz` & `tmp/pyosudb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyosudb-0.1.0.tar", last modified: Mon Jun 12 11:30:36 2023, max compression
+gzip compressed data, was "pyosudb-0.1.1.tar", last modified: Mon Jun 12 16:41:49 2023, max compression
```

## Comparing `pyosudb-0.1.0.tar` & `pyosudb-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 11:30:36.489756 pyosudb-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-06-06 21:12:18.000000 pyosudb-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      522 2023-06-12 11:30:36.488757 pyosudb-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-07 20:16:57.000000 pyosudb-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 11:30:36.470755 pyosudb-0.1.0/pyosudb/
--rw-rw-rw-   0        0        0      231 2023-06-12 06:33:29.000000 pyosudb-0.1.0/pyosudb/__init__.py
--rw-rw-rw-   0        0        0     1646 2023-06-12 11:23:36.000000 pyosudb-0.1.0/pyosudb/collectiondb.py
--rw-rw-rw-   0        0        0    12597 2023-06-12 05:22:09.000000 pyosudb-0.1.0/pyosudb/datatypes.py
--rw-rw-rw-   0        0        0    10008 2023-06-12 11:20:02.000000 pyosudb-0.1.0/pyosudb/osudb.py
--rw-rw-rw-   0        0        0      882 2023-06-12 11:26:42.000000 pyosudb-0.1.0/pyosudb/presencedb.py
--rw-rw-rw-   0        0        0     1586 2023-06-12 11:25:25.000000 pyosudb-0.1.0/pyosudb/scoresdb.py
--rw-rw-rw-   0        0        0     1830 2023-06-12 10:36:37.000000 pyosudb-0.1.0/pyosudb/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 11:30:36.484755 pyosudb-0.1.0/pyosudb.egg-info/
--rw-rw-rw-   0        0        0      522 2023-06-12 11:30:36.000000 pyosudb-0.1.0/pyosudb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-06-12 11:30:36.000000 pyosudb-0.1.0/pyosudb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 11:30:36.000000 pyosudb-0.1.0/pyosudb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 11:30:36.000000 pyosudb-0.1.0/pyosudb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      679 2023-06-12 10:28:10.000000 pyosudb-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 11:30:36.489756 pyosudb-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 11:30:36.487756 pyosudb-0.1.0/tests/
--rw-rw-rw-   0        0        0     1105 2023-06-12 10:23:08.000000 pyosudb-0.1.0/tests/test_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:49.340594 pyosudb-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-12 16:41:36.000000 pyosudb-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 16:41:49.336594 pyosudb-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:36.000000 pyosudb-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:49.336594 pyosudb-0.1.1/pyosudb/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-12 16:41:36.000000 pyosudb-0.1.1/pyosudb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-12 16:41:36.000000 pyosudb-0.1.1/pyosudb/collectiondb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-06-12 16:41:36.000000 pyosudb-0.1.1/pyosudb/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-06-12 16:41:36.000000 pyosudb-0.1.1/pyosudb/osudb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-12 16:41:36.000000 pyosudb-0.1.1/pyosudb/presencedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-12 16:41:36.000000 pyosudb-0.1.1/pyosudb/scoresdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-12 16:41:36.000000 pyosudb-0.1.1/pyosudb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:49.336594 pyosudb-0.1.1/pyosudb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-12 16:41:49.000000 pyosudb-0.1.1/pyosudb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-12 16:41:49.000000 pyosudb-0.1.1/pyosudb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:41:49.000000 pyosudb-0.1.1/pyosudb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 16:41:49.000000 pyosudb-0.1.1/pyosudb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-12 16:41:36.000000 pyosudb-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:41:49.340594 pyosudb-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:41:49.336594 pyosudb-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-12 16:41:37.000000 pyosudb-0.1.1/tests/test_parsing.py
```

### Comparing `pyosudb-0.1.0/pyosudb/collectiondb.py` & `pyosudb-0.1.1/pyosudb/collectiondb.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from dataclasses import dataclass
-from typing import List, Union
-import os
-import io
-
-from pyosudb import utils
-from pyosudb.datatypes import Collection
-
-
-@dataclass
-class Collectiondb:
-    """
-    Class representing collection.db file
-
-    Attributes
-    ----
-    version: int
-        osu! version when this file created
-
-    count_collections: int
-        Amount of collections in .db file
-
-    collections: List[Collection]
-        List of collections represented by "Collection" class
-    """
-    version: int
-    count_collections: int
-    collections: List[Collection]
-
-
-class _Parser:
-    def __init__(self, collectiondb_file) -> None:
-        self.collectiondb_file = collectiondb_file
-        self.offset = 0
-
-    def parse(self) -> Collectiondb:
-        version = utils.read_uint(self.collectiondb_file)
-        count_collections = utils.read_uint(self.collectiondb_file)
-        collections = []
-        for _ in range(count_collections):
-            collections.append(Collection.parse(self.collectiondb_file, version))
-
-        return Collectiondb(version, count_collections, collections)
-
-
-def parse_collectiondb(collectiondb_file: Union[str, os.PathLike, io.BytesIO]) -> Collectiondb:
-    """
-    Parse collection.db file
-
-    Args
-    ----
-    collectiondb_file: str | os.PathLike | io.BytesIO
-        Path or opened file
-
-    Returns
-    ----
-    Collectiondb
-        instance of Collectiondb class
-    """
-    if not isinstance(collectiondb_file, io.BytesIO):
-        collectiondb_file = open(collectiondb_file, "rb")
-
-    return _Parser(collectiondb_file).parse()
+from dataclasses import dataclass
+from typing import List, Union
+import os
+import io
+
+from pyosudb import utils
+from pyosudb.datatypes import Collection
+
+
+@dataclass
+class Collectiondb:
+    """
+    Class representing collection.db file
+
+    Attributes
+    ----
+    version: int
+        osu! version when this file created
+
+    count_collections: int
+        Amount of collections in .db file
+
+    collections: List[Collection]
+        List of collections represented by "Collection" class
+    """
+    version: int
+    count_collections: int
+    collections: List[Collection]
+
+
+class _Parser:
+    def __init__(self, collectiondb_file) -> None:
+        self.collectiondb_file = collectiondb_file
+        self.offset = 0
+
+    def parse(self) -> Collectiondb:
+        version = utils.read_uint(self.collectiondb_file)
+        count_collections = utils.read_uint(self.collectiondb_file)
+        collections = []
+        for _ in range(count_collections):
+            collections.append(Collection.parse(self.collectiondb_file, version))
+
+        return Collectiondb(version, count_collections, collections)
+
+
+def parse_collectiondb(collectiondb_file: Union[str, os.PathLike, io.BytesIO]) -> Collectiondb:
+    """
+    Parse collection.db file
+
+    Args
+    ----
+    collectiondb_file: str | os.PathLike | io.BytesIO
+        Path or opened file
+
+    Returns
+    ----
+    Collectiondb
+        instance of Collectiondb class
+    """
+    if not isinstance(collectiondb_file, io.BytesIO):
+        collectiondb_file = open(collectiondb_file, "rb")
+
+    return _Parser(collectiondb_file).parse()
```

### Comparing `pyosudb-0.1.0/pyosudb/datatypes.py` & `pyosudb-0.1.1/pyosudb/datatypes.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,470 +1,470 @@
-from enum import Enum, IntFlag
-from dataclasses import dataclass
-from typing import Optional, List
-import io
-import datetime
-import pickle
-
-from pyosudb import utils
-
-
-class GameMode(Enum):
-    """
-    osu! gamemodes
-    """
-    STD = 0
-    TAIKO = 1
-    CTB = 2
-    MANIA = 3
-
-
-class Mod(IntFlag):
-    """
-    osu! mods or their combination
-    """
-    NM = 0
-    NF = 1 << 0
-    EZ = 1 << 1
-    TD = 1 << 2
-    HD = 1 << 3
-    HR = 1 << 4
-    SD = 1 << 5
-    DT = 1 << 6
-    RX = 1 << 7
-    HT = 1 << 8
-    NC = 1 << 9
-    FL = 1 << 10
-    AT = 1 << 11
-    SO = 1 << 12
-    AP = 1 << 13
-    PF = 1 << 14
-    K4 = 1 << 15
-    K5 = 1 << 16
-    K6 = 1 << 17
-    K7 = 1 << 18
-    K8 = 1 << 19
-    FD = 1 << 20
-    RD = 1 << 21
-    CN = 1 << 22
-    TP = 1 << 23
-    K9 = 1 << 24
-    CO = 1 << 25
-    K1 = 1 << 26
-    K3 = 1 << 27
-    K2 = 1 << 28
-    V2 = 1 << 29
-    MR = 1 << 30
-
-
-class Grade(Enum):
-    """
-    osu! grades on scores
-    """
-    SS_silver = 0
-    S_silver = 1
-    SS = 2
-    S = 3
-    A = 4
-    B = 5
-    C = 6
-    D = 7
-    Unplayed = 9
-
-
-class RankedStatus(Enum):
-    """
-    osu! beatmap statuses
-    """
-    UNKNOWN = 0
-    UNSUBMITTED = 1
-    PENDING = 2  # also wip and graveyard
-    UNUSED = 3  # ???
-    RANKED = 4
-    APPROVED = 5
-    QUALIFIED = 6
-    LOVED = 7
-
-
-class UserPermissions(IntFlag):
-    """
-    osu! user permission in chat
-    """
-    UNKNOWN = 0
-    NORMAL = 1
-    MODERATOR = 1 << 1
-    SUPPORTER = 1 << 2
-    FRIEND = 1 << 3
-    PEPPY = 1 << 4
-    WORLD_CUP_STAFF = 1 << 5
-
-
-@dataclass
-class TimingPoint:
-    """
-    Timing point in osu! beatmap
-    """
-    bpm: float
-    offset: float
-    inherited: bool
-
-
-@dataclass
-class ModStarRatingPair:
-    """
-    Pairs for beatmaps with mods combination and their star rating with those mods
-    """
-    mod: Mod
-    star_rating: float
-
-
-@dataclass
-class Beatmap:
-    """
-    osu! beatmap
-    """
-    size: Optional[int]  # only present if osu! version is less than 20191106
-    artist: str
-    artist_unicode: str
-    title: str
-    title_unicode: str
-    mapper: str
-    difficulty: str
-    audio_file: str
-    md5_hash: str
-    osu_file: str
-
-    ranked_status: RankedStatus
-    count_hitcircles: int
-    count_sliders: int
-    count_spinners: int
-    last_modification: datetime.datetime
-
-    ar: int
-    cs: int
-    hp: int
-    od: int
-    slider_velocity: float
-
-    std_pairs: List[ModStarRatingPair]
-    taiko_pairs: List[ModStarRatingPair]
-    ctb_pairs: List[ModStarRatingPair]
-    mania_pairs: List[ModStarRatingPair]
-
-    drain_time: int
-    total_time: int
-    preview_time: int
-
-    timing_points: List[TimingPoint]
-
-    difficulty_id: int
-    beatmap_id: int
-    thread_id: int
-
-    std_grade: int
-    taiko_grade: int
-    ctb_grade: int
-    mania_grade: int
-
-    local_offset: int
-    stack_leniency: int
-
-    gameplay_mode: GameMode
-
-    song_source: str
-    song_tags: str
-
-    online_offset: int
-
-    title_font: str
-
-    unplayed: bool
-    last_played: datetime.datetime
-
-    is_osz2: bool
-    folder_name: str
-    last_checked: datetime.datetime
-
-    ignore_sound: bool
-    ignore_skin: bool
-    disable_storyboard: bool
-    disable_video: bool
-
-    visual_override: bool
-
-    unknown: Optional[int]  # osu! wiki page literally says it's unknown and present if game version less than 20140609
-
-    last_modification2: datetime.datetime  # ?
-
-    mania_scroll_speed: int
-
-    @staticmethod
-    def parse(buffer: io.BytesIO, game_ver: int = 0):
-        """
-        Parse beatmap from file
-
-        Args
-        ----
-        buffer: io.BytesIO
-            Opened file
-        game_ver: int
-            Version of game
-
-        Returns
-        ----
-        Beatmap
-            Parsed beatmap
-        """
-        size = None
-        if game_ver < 20191106:
-            size = utils.read_uint(buffer)
-        artist = utils.read_string(buffer)
-        artist_unicode = utils.read_string(buffer)
-        title = utils.read_string(buffer)
-
-        title_unicode = utils.read_string(buffer)
-        creator = utils.read_string(buffer)
-        difficulty = utils.read_string(buffer)
-        audio_file = utils.read_string(buffer)
-        md5_hash = utils.read_string(buffer)
-        osu_file = utils.read_string(buffer)
-
-        ranked_status = RankedStatus(utils.read_ubyte(buffer))
-        count_hitcircles = utils.read_ushort(buffer)
-        count_sliders = utils.read_ushort(buffer)
-        count_spiners = utils.read_ushort(buffer)
-
-        last_modification = utils.read_datetime(buffer)
-
-        if game_ver < 20140609:
-            ar = utils.read_ubyte(buffer)
-            cs = utils.read_ubyte(buffer)
-            hp = utils.read_ubyte(buffer)
-            od = utils.read_ubyte(buffer)
-        else:
-            ar = utils.read_float(buffer)
-            cs = utils.read_float(buffer)
-            hp = utils.read_float(buffer)
-            od = utils.read_float(buffer)
-
-        slider_velocity = utils.read_double(buffer)
-
-        std_pairs = []
-        taiko_pairs = []
-        ctb_pairs = []
-        mania_pairs = []
-        if game_ver >= 20140609:
-            for _ in range(utils.read_uint(buffer)):
-                tmp = utils.read_int_double(buffer)
-                std_pairs.append(ModStarRatingPair(Mod(tmp[0]), tmp[1]))
-
-            for _ in range(utils.read_uint(buffer)):
-                tmp = utils.read_int_double(buffer)
-                taiko_pairs.append(ModStarRatingPair(Mod(tmp[0]), tmp[1]))
-
-            for _ in range(utils.read_uint(buffer)):
-                tmp = utils.read_int_double(buffer)
-                ctb_pairs.append(ModStarRatingPair(Mod(tmp[0]), tmp[1]))
-
-            for _ in range(utils.read_uint(buffer)):
-                tmp = utils.read_int_double(buffer)
-                mania_pairs.append(ModStarRatingPair(Mod(tmp[0]), tmp[1]))
-
-        drain_time = utils.read_uint(buffer)
-        total_time = utils.read_uint(buffer)
-        preview_time = utils.read_uint(buffer)
-
-        timing_points = []
-        for _ in range(utils.read_uint(buffer)):
-            timing_points.append(TimingPoint(*utils.read_timing_point(buffer)))
-
-        difficulty_id = utils.read_uint(buffer)
-        beatmap_id = utils.read_uint(buffer)
-        thread_id = utils.read_uint(buffer)
-
-        std_grade = utils.read_ubyte(buffer)
-        taiko_grade = utils.read_ubyte(buffer)
-        ctb_grade = utils.read_ubyte(buffer)
-        mania_grade = utils.read_ubyte(buffer)
-
-        local_offset = utils.read_ushort(buffer)
-        stack_laniency = utils.read_float(buffer)
-
-        gameplay_mode = GameMode(utils.read_ubyte(buffer))
-
-        song_source = utils.read_string(buffer)
-        song_tags = utils.read_string(buffer)
-
-        online_offset = utils.read_ushort(buffer)
-
-        title_font = utils.read_string(buffer)
-
-        unplayed = utils.read_bool(buffer)
-        last_played = utils.read_datetime(buffer)
-
-        is_osz2 = utils.read_bool(buffer)
-        folder_name = utils.read_string(buffer)
-        last_checked = utils.read_datetime(buffer)
-
-        ignore_sound = utils.read_bool(buffer)
-        ignore_skin = utils.read_bool(buffer)
-        disable_storyboard = utils.read_bool(buffer)
-        disable_video = utils.read_bool(buffer)
-
-        visual_override = utils.read_bool(buffer)
-
-        unknown = None
-        if game_ver < 20140609:
-            unknown = utils.read_uint(buffer)  # osu! wiki page literally says it's unknown and present if game version less than 20140609
-
-        last_modification_time = utils.read_uint(buffer)
-
-        mania_scroll_speed = utils.read_ubyte(buffer)
-
-        return Beatmap(size, artist, artist_unicode, title, title_unicode, creator, difficulty, audio_file, md5_hash, osu_file, ranked_status, count_hitcircles, count_sliders,
-                       count_spiners, last_modification, ar, cs, hp, od, slider_velocity, std_pairs, taiko_pairs, ctb_pairs, mania_pairs, drain_time, total_time, preview_time,
-                       timing_points, difficulty_id, beatmap_id, thread_id, std_grade, taiko_grade, ctb_grade, mania_grade, local_offset, stack_laniency, gameplay_mode, song_source,
-                       song_tags, online_offset, title_font, unplayed, last_played, is_osz2, folder_name, last_checked, ignore_sound, ignore_skin, disable_storyboard, disable_video,
-                       visual_override, unknown, last_modification_time, mania_scroll_speed)
-
-    @staticmethod
-    def from_sql(*args):
-        # TODO: rewrite func cuz this one is kinda unsave
-        """
-        Get beatmap from sql row
-
-        Returns
-        ----
-        Beatmap
-            osu! beatmap
-        """
-        new_args = []
-        for arg in args:
-            if arg is None:
-                new_args.append(arg)
-                continue
-
-            if type(arg) == str and (arg[:2] == "b\'" or arg[:2] == "b\""):
-                new_args.append(pickle.loads(bytearray(eval(arg))))
-                continue
-            new_args.append(arg)
-
-        return Beatmap(*new_args)
-
-
-@dataclass
-class Score:
-    """
-    osu! score
-    """
-    gamemode: GameMode
-    score_version: int
-    beatmap_hash: str
-    username: str
-    replay_hash: str
-
-    count_300: int
-    count_100: int
-    count_50: int
-    count_geki: int
-    count_katu: int
-    count_miss: int
-
-    total_score: int
-    max_combo: int
-    perfect_combo: bool
-
-    mods: Mod
-
-    timestamp: datetime.datetime
-    online_score_id: int
-    additional_info: Optional[float] = 0
-
-    def parse(buffer: io.BytesIO, game_ver: int = 0):
-        """
-        Parse score from file
-
-        Args
-        ----
-        buffer: io.BytesIO
-            Opened file
-        game_ver: int
-            Version of game
-
-        Returns
-        ----
-        Beatmap
-            Parsed score
-        """
-        gamemode = GameMode(utils.read_ubyte(buffer))
-        score_version = utils.read_uint(buffer)
-        beatmap_hash = utils.read_string(buffer)
-        username = utils.read_string(buffer)
-        replay_hash = utils.read_string(buffer)
-
-        count_300 = utils.read_ushort(buffer)
-        count_100 = utils.read_ushort(buffer)
-        count_50 = utils.read_ushort(buffer)
-        count_geki = utils.read_ushort(buffer)
-        count_katu = utils.read_ushort(buffer)
-        count_miss = utils.read_ushort(buffer)
-
-        total_score = utils.read_uint(buffer)
-        max_combo = utils.read_ushort(buffer)
-        perfect_combo = utils.read_bool(buffer)
-
-        mods = Mod(utils.read_uint(buffer))
-
-        utils.read_string(buffer)  # this one always should be empty for some reason, skip it
-        timestamp = utils.read_datetime(buffer)
-        utils.read_uint(buffer)  # always should be -1, skip it
-        online_score_id = utils.read_ulong(buffer)
-
-        additional_info = None
-        # if target practice in mods
-        if Mod(1 << 23) in mods:
-            additional_info = utils.read_double(buffer)
-
-        return Score(gamemode, score_version, beatmap_hash, username, replay_hash,
-                     count_300, count_100, count_50, count_geki, count_katu, count_miss,
-                     total_score, max_combo, perfect_combo, timestamp, online_score_id, additional_info)
-
-
-@dataclass
-class BeatmapScores:
-    """
-    List of scores on beatmap
-    """
-    beatmap_hash: str
-    count_scores: int
-    scores: List[Score]
-
-    @staticmethod
-    def parse(buffer: io.BytesIO, game_ver: int = 0):
-        beatmap_hash = utils.read_string(buffer)
-        count_scores = utils.read_uint(buffer)
-        scores = []
-        for _ in range(count_scores):
-            scores.append(Score.parse(buffer, game_ver))
-
-        return BeatmapScores(beatmap_hash, count_scores, scores)
-
-
-@dataclass
-class Collection:
-    """
-    osu! collection with beatmaps
-    """
-    name: str
-    count_beatmaps: int
-    beatmaps_hash: List[str]
-
-    @staticmethod
-    def parse(buffer: io.BytesIO, game_ver: int = 0):
-        name = utils.read_string(buffer)
-        count_beatmaps = utils.read_uint(buffer)
-        beatmaps_hash = []
-
-        for _ in range(count_beatmaps):
-            beatmaps_hash.append(utils.read_string(buffer))
-
-        return Collection(name, count_beatmaps, beatmaps_hash)
+from enum import Enum, IntFlag
+from dataclasses import dataclass
+from typing import Optional, List
+import io
+import datetime
+import pickle
+
+from pyosudb import utils
+
+
+class GameMode(Enum):
+    """
+    osu! gamemodes
+    """
+    STD = 0
+    TAIKO = 1
+    CTB = 2
+    MANIA = 3
+
+
+class Mod(IntFlag):
+    """
+    osu! mods or their combination
+    """
+    NM = 0
+    NF = 1 << 0
+    EZ = 1 << 1
+    TD = 1 << 2
+    HD = 1 << 3
+    HR = 1 << 4
+    SD = 1 << 5
+    DT = 1 << 6
+    RX = 1 << 7
+    HT = 1 << 8
+    NC = 1 << 9
+    FL = 1 << 10
+    AT = 1 << 11
+    SO = 1 << 12
+    AP = 1 << 13
+    PF = 1 << 14
+    K4 = 1 << 15
+    K5 = 1 << 16
+    K6 = 1 << 17
+    K7 = 1 << 18
+    K8 = 1 << 19
+    FD = 1 << 20
+    RD = 1 << 21
+    CN = 1 << 22
+    TP = 1 << 23
+    K9 = 1 << 24
+    CO = 1 << 25
+    K1 = 1 << 26
+    K3 = 1 << 27
+    K2 = 1 << 28
+    V2 = 1 << 29
+    MR = 1 << 30
+
+
+class Grade(Enum):
+    """
+    osu! grades on scores
+    """
+    SS_silver = 0
+    S_silver = 1
+    SS = 2
+    S = 3
+    A = 4
+    B = 5
+    C = 6
+    D = 7
+    Unplayed = 9
+
+
+class RankedStatus(Enum):
+    """
+    osu! beatmap statuses
+    """
+    UNKNOWN = 0
+    UNSUBMITTED = 1
+    PENDING = 2  # also wip and graveyard
+    UNUSED = 3  # ???
+    RANKED = 4
+    APPROVED = 5
+    QUALIFIED = 6
+    LOVED = 7
+
+
+class UserPermissions(IntFlag):
+    """
+    osu! user permission in chat
+    """
+    UNKNOWN = 0
+    NORMAL = 1
+    MODERATOR = 1 << 1
+    SUPPORTER = 1 << 2
+    FRIEND = 1 << 3
+    PEPPY = 1 << 4
+    WORLD_CUP_STAFF = 1 << 5
+
+
+@dataclass
+class TimingPoint:
+    """
+    Timing point in osu! beatmap
+    """
+    bpm: float
+    offset: float
+    inherited: bool
+
+
+@dataclass
+class ModStarRatingPair:
+    """
+    Pairs for beatmaps with mods combination and their star rating with those mods
+    """
+    mod: Mod
+    star_rating: float
+
+
+@dataclass
+class Beatmap:
+    """
+    osu! beatmap
+    """
+    size: Optional[int]  # only present if osu! version is less than 20191106
+    artist: str
+    artist_unicode: str
+    title: str
+    title_unicode: str
+    mapper: str
+    difficulty: str
+    audio_file: str
+    md5_hash: str
+    osu_file: str
+
+    ranked_status: RankedStatus
+    count_hitcircles: int
+    count_sliders: int
+    count_spinners: int
+    last_modification: datetime.datetime
+
+    ar: int
+    cs: int
+    hp: int
+    od: int
+    slider_velocity: float
+
+    std_pairs: List[ModStarRatingPair]
+    taiko_pairs: List[ModStarRatingPair]
+    ctb_pairs: List[ModStarRatingPair]
+    mania_pairs: List[ModStarRatingPair]
+
+    drain_time: int
+    total_time: int
+    preview_time: int
+
+    timing_points: List[TimingPoint]
+
+    difficulty_id: int
+    beatmap_id: int
+    thread_id: int
+
+    std_grade: int
+    taiko_grade: int
+    ctb_grade: int
+    mania_grade: int
+
+    local_offset: int
+    stack_leniency: int
+
+    gameplay_mode: GameMode
+
+    song_source: str
+    song_tags: str
+
+    online_offset: int
+
+    title_font: str
+
+    unplayed: bool
+    last_played: datetime.datetime
+
+    is_osz2: bool
+    folder_name: str
+    last_checked: datetime.datetime
+
+    ignore_sound: bool
+    ignore_skin: bool
+    disable_storyboard: bool
+    disable_video: bool
+
+    visual_override: bool
+
+    unknown: Optional[int]  # osu! wiki page literally says it's unknown and present if game version less than 20140609
+
+    last_modification2: datetime.datetime  # ?
+
+    mania_scroll_speed: int
+
+    @staticmethod
+    def parse(buffer: io.BytesIO, game_ver: int = 0):
+        """
+        Parse beatmap from file
+
+        Args
+        ----
+        buffer: io.BytesIO
+            Opened file
+        game_ver: int
+            Version of game
+
+        Returns
+        ----
+        Beatmap
+            Parsed beatmap
+        """
+        size = None
+        if game_ver < 20191106:
+            size = utils.read_uint(buffer)
+        artist = utils.read_string(buffer)
+        artist_unicode = utils.read_string(buffer)
+        title = utils.read_string(buffer)
+
+        title_unicode = utils.read_string(buffer)
+        creator = utils.read_string(buffer)
+        difficulty = utils.read_string(buffer)
+        audio_file = utils.read_string(buffer)
+        md5_hash = utils.read_string(buffer)
+        osu_file = utils.read_string(buffer)
+
+        ranked_status = RankedStatus(utils.read_ubyte(buffer))
+        count_hitcircles = utils.read_ushort(buffer)
+        count_sliders = utils.read_ushort(buffer)
+        count_spiners = utils.read_ushort(buffer)
+
+        last_modification = utils.read_datetime(buffer)
+
+        if game_ver < 20140609:
+            ar = utils.read_ubyte(buffer)
+            cs = utils.read_ubyte(buffer)
+            hp = utils.read_ubyte(buffer)
+            od = utils.read_ubyte(buffer)
+        else:
+            ar = utils.read_float(buffer)
+            cs = utils.read_float(buffer)
+            hp = utils.read_float(buffer)
+            od = utils.read_float(buffer)
+
+        slider_velocity = utils.read_double(buffer)
+
+        std_pairs = []
+        taiko_pairs = []
+        ctb_pairs = []
+        mania_pairs = []
+        if game_ver >= 20140609:
+            for _ in range(utils.read_uint(buffer)):
+                tmp = utils.read_int_double(buffer)
+                std_pairs.append(ModStarRatingPair(Mod(tmp[0]), tmp[1]))
+
+            for _ in range(utils.read_uint(buffer)):
+                tmp = utils.read_int_double(buffer)
+                taiko_pairs.append(ModStarRatingPair(Mod(tmp[0]), tmp[1]))
+
+            for _ in range(utils.read_uint(buffer)):
+                tmp = utils.read_int_double(buffer)
+                ctb_pairs.append(ModStarRatingPair(Mod(tmp[0]), tmp[1]))
+
+            for _ in range(utils.read_uint(buffer)):
+                tmp = utils.read_int_double(buffer)
+                mania_pairs.append(ModStarRatingPair(Mod(tmp[0]), tmp[1]))
+
+        drain_time = utils.read_uint(buffer)
+        total_time = utils.read_uint(buffer)
+        preview_time = utils.read_uint(buffer)
+
+        timing_points = []
+        for _ in range(utils.read_uint(buffer)):
+            timing_points.append(TimingPoint(*utils.read_timing_point(buffer)))
+
+        difficulty_id = utils.read_uint(buffer)
+        beatmap_id = utils.read_uint(buffer)
+        thread_id = utils.read_uint(buffer)
+
+        std_grade = utils.read_ubyte(buffer)
+        taiko_grade = utils.read_ubyte(buffer)
+        ctb_grade = utils.read_ubyte(buffer)
+        mania_grade = utils.read_ubyte(buffer)
+
+        local_offset = utils.read_ushort(buffer)
+        stack_laniency = utils.read_float(buffer)
+
+        gameplay_mode = GameMode(utils.read_ubyte(buffer))
+
+        song_source = utils.read_string(buffer)
+        song_tags = utils.read_string(buffer)
+
+        online_offset = utils.read_ushort(buffer)
+
+        title_font = utils.read_string(buffer)
+
+        unplayed = utils.read_bool(buffer)
+        last_played = utils.read_datetime(buffer)
+
+        is_osz2 = utils.read_bool(buffer)
+        folder_name = utils.read_string(buffer)
+        last_checked = utils.read_datetime(buffer)
+
+        ignore_sound = utils.read_bool(buffer)
+        ignore_skin = utils.read_bool(buffer)
+        disable_storyboard = utils.read_bool(buffer)
+        disable_video = utils.read_bool(buffer)
+
+        visual_override = utils.read_bool(buffer)
+
+        unknown = None
+        if game_ver < 20140609:
+            unknown = utils.read_uint(buffer)  # osu! wiki page literally says it's unknown and present if game version less than 20140609
+
+        last_modification_time = utils.read_uint(buffer)
+
+        mania_scroll_speed = utils.read_ubyte(buffer)
+
+        return Beatmap(size, artist, artist_unicode, title, title_unicode, creator, difficulty, audio_file, md5_hash, osu_file, ranked_status, count_hitcircles, count_sliders,
+                       count_spiners, last_modification, ar, cs, hp, od, slider_velocity, std_pairs, taiko_pairs, ctb_pairs, mania_pairs, drain_time, total_time, preview_time,
+                       timing_points, difficulty_id, beatmap_id, thread_id, std_grade, taiko_grade, ctb_grade, mania_grade, local_offset, stack_laniency, gameplay_mode, song_source,
+                       song_tags, online_offset, title_font, unplayed, last_played, is_osz2, folder_name, last_checked, ignore_sound, ignore_skin, disable_storyboard, disable_video,
+                       visual_override, unknown, last_modification_time, mania_scroll_speed)
+
+    @staticmethod
+    def from_sql(*args):
+        # TODO: rewrite func cuz this one is kinda unsave
+        """
+        Get beatmap from sql row
+
+        Returns
+        ----
+        Beatmap
+            osu! beatmap
+        """
+        new_args = []
+        for arg in args:
+            if arg is None:
+                new_args.append(arg)
+                continue
+
+            if type(arg) == str and (arg[:2] == "b\'" or arg[:2] == "b\""):
+                new_args.append(pickle.loads(bytearray(eval(arg))))
+                continue
+            new_args.append(arg)
+
+        return Beatmap(*new_args)
+
+
+@dataclass
+class Score:
+    """
+    osu! score
+    """
+    gamemode: GameMode
+    score_version: int
+    beatmap_hash: str
+    username: str
+    replay_hash: str
+
+    count_300: int
+    count_100: int
+    count_50: int
+    count_geki: int
+    count_katu: int
+    count_miss: int
+
+    total_score: int
+    max_combo: int
+    perfect_combo: bool
+
+    mods: Mod
+
+    timestamp: datetime.datetime
+    online_score_id: int
+    additional_info: Optional[float] = 0
+
+    def parse(buffer: io.BytesIO, game_ver: int = 0):
+        """
+        Parse score from file
+
+        Args
+        ----
+        buffer: io.BytesIO
+            Opened file
+        game_ver: int
+            Version of game
+
+        Returns
+        ----
+        Beatmap
+            Parsed score
+        """
+        gamemode = GameMode(utils.read_ubyte(buffer))
+        score_version = utils.read_uint(buffer)
+        beatmap_hash = utils.read_string(buffer)
+        username = utils.read_string(buffer)
+        replay_hash = utils.read_string(buffer)
+
+        count_300 = utils.read_ushort(buffer)
+        count_100 = utils.read_ushort(buffer)
+        count_50 = utils.read_ushort(buffer)
+        count_geki = utils.read_ushort(buffer)
+        count_katu = utils.read_ushort(buffer)
+        count_miss = utils.read_ushort(buffer)
+
+        total_score = utils.read_uint(buffer)
+        max_combo = utils.read_ushort(buffer)
+        perfect_combo = utils.read_bool(buffer)
+
+        mods = Mod(utils.read_uint(buffer))
+
+        utils.read_string(buffer)  # this one always should be empty for some reason, skip it
+        timestamp = utils.read_datetime(buffer)
+        utils.read_uint(buffer)  # always should be -1, skip it
+        online_score_id = utils.read_ulong(buffer)
+
+        additional_info = None
+        # if target practice in mods
+        if Mod(1 << 23) in mods:
+            additional_info = utils.read_double(buffer)
+
+        return Score(gamemode, score_version, beatmap_hash, username, replay_hash,
+                     count_300, count_100, count_50, count_geki, count_katu, count_miss,
+                     total_score, max_combo, perfect_combo, timestamp, online_score_id, additional_info)
+
+
+@dataclass
+class BeatmapScores:
+    """
+    List of scores on beatmap
+    """
+    beatmap_hash: str
+    count_scores: int
+    scores: List[Score]
+
+    @staticmethod
+    def parse(buffer: io.BytesIO, game_ver: int = 0):
+        beatmap_hash = utils.read_string(buffer)
+        count_scores = utils.read_uint(buffer)
+        scores = []
+        for _ in range(count_scores):
+            scores.append(Score.parse(buffer, game_ver))
+
+        return BeatmapScores(beatmap_hash, count_scores, scores)
+
+
+@dataclass
+class Collection:
+    """
+    osu! collection with beatmaps
+    """
+    name: str
+    count_beatmaps: int
+    beatmaps_hash: List[str]
+
+    @staticmethod
+    def parse(buffer: io.BytesIO, game_ver: int = 0):
+        name = utils.read_string(buffer)
+        count_beatmaps = utils.read_uint(buffer)
+        beatmaps_hash = []
+
+        for _ in range(count_beatmaps):
+            beatmaps_hash.append(utils.read_string(buffer))
+
+        return Collection(name, count_beatmaps, beatmaps_hash)
```

### Comparing `pyosudb-0.1.0/pyosudb/osudb.py` & `pyosudb-0.1.1/pyosudb/osudb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-from dataclasses import dataclass
-from typing import Union, Any, List
-import datetime
-import tempfile
-import sqlite3
-import pickle
-import io
-import os
-
-from pyosudb import utils
-from pyosudb.datatypes import Beatmap, UserPermissions
-
-
-@dataclass
-class Osudb:
-    """
-    Class representing osu!.db file
-
-    Attributes
-    ----
-    game_version: int
-        osu! version when this file created
-
-    folder_count: int
-        Amount of folders in "songs" folder
-
-    account_unlocked: bool
-        Is account banned. False if banned, True otherwise
-
-    unlock_datetime: datetime.datetime
-        Time until account will be unbanned. Always 0 if account is not banned (account_unlocked=True)
-
-    username: str
-        Player username
-
-    sql_beatmaps_db: sqlite3.Connection
-        Connection to sqllite3 database. It must not be set by the user
-
-    user_permissions: UserPermissions
-        User permissions in chat. Check UserPermissions class for more info
-    """
-    game_version: int
-    folder_count: int
-    account_unlocked: bool  # false if account banned/locked
-    unlock_datetime: datetime.datetime
-    username: str
-    count_beatmaps: int
-
-    sql_beatmaps_db: sqlite3.Connection
-
-    user_permissions: UserPermissions
-
-    # can't be saved because osu.db can be big and we don't need 20k objects with maps in our ram
-    def beatmaps(self) -> List[Beatmap]:
-        """
-        List of beatmaps
-
-        Returns
-        ----
-        List[Beatmaps]
-            List of Beatmaps instances
-        """
-        cursor = self.sql_beatmaps_db.cursor()
-        return [Beatmap.from_sql(*beatmap) for beatmap in cursor.execute("SELECT * FROM 'beatmaps' ")]
-
-    def get_beatmap_from_hash(self, hash: str) -> Beatmap:
-        """
-        Get beatmap from sql table using hash
-
-        Args
-        ----
-        hash: str
-            beatmap hash
-
-        Returns
-        ----
-        Beatmap
-            instance of Beatmap
-        """
-        cursor = self.sql_beatmaps_db.cursor()
-        return Beatmap.from_sql(cursor.execute(f"SELECT * FROM 'beatmaps' WHERE md5_hash='{hash}'")[0])
-
-    def beatmaps_execute_sql(self, command) -> Any:
-        """
-        Executes sql command in table with beatmaps
-        """
-        cursor = self.sql_beatmaps_db.cursor()
-        return cursor.execute(command)
-
-
-class _Parser:
-    def __init__(self, osu_db_file) -> None:
-        self.osu_db_file = osu_db_file
-        self.offset = 0
-
-    def generate_sql_db(self) -> None:
-        """
-        Generates sql table for file
-        """
-        cursor = self.beatmaps_db.cursor()
-        cursor.execute("SELECT count(name) FROM sqlite_master WHERE type='table' AND name='beatmaps'")
-        if cursor.fetchone()[0] == 1:
-            self.beatmaps_db.execute("DROP TABLE beatmaps")
-        self.beatmaps_db.execute("""CREATE TABLE beatmaps (
-                            size INTEGER,
-                            artist TEXT,
-                            artist_unicode TEXT,
-                            title TEXT,
-                            title_unicode TEXT,
-                            mapper TEXT,
-                            difficulty TEXT,
-                            audio_file TEXT,
-                            md5_hash TEXT,
-                            osu_file TEXT,
-                            ranked_status TEXT,
-                            count_hitcircles INTEGER,
-                            count_sliders INTEGER,
-                            count_spinners INTEGER,
-                            last_modification TEXT,
-                            ar NUMERIC,
-                            cs NUMERIC,
-                            hp NUMERIC,
-                            od NUMERIC,
-                            slider_velocity NUMERIC,
-                            std_pairs TEXT,
-                            taiko_pairs TEXT,
-                            ctb_pairs TEXT,
-                            mania_pairs TEXT,
-                            drain_time INTEGER,
-                            total_time INTEGER,
-                            preview_time INTEGER,
-                            timing_points TEXT,
-                            difficulty_id INTEGER,
-                            beatmap_id INTEGER,
-                            thread_id INTEGER,
-                            std_grade TEXT,
-                            taiko_grade TEXT,
-                            ctb_grade TEXT,
-                            mania_grade TEXT,
-                            local_offset INTEGER,
-                            stack_leniency NUMERIC,
-                            gameplay_mode TEXT,
-                            song_source TEXT,
-                            song_tags TEXT,
-                            online_offset INTEGER,
-                            title_font TEXT,
-                            unplayed INTEGER,
-                            last_played INTEGER,
-                            is_osz2 INTEGER,
-                            folder_name TEXT,
-                            last_checked TEXT,
-                            ignore_sound INTEGER,
-                            ignore_skin INTEGER,
-                            disable_storyboard INTEGER,
-                            disable_video INTEGER,
-                            visual_override INTEGER,
-                            unknown INTEGER,
-                            last_modification2 TEXT,
-                            mania_scroll_speed INTEGER
-                        );""")
-
-    def add_beatmap_to_db(self, beatmap: Beatmap) -> None:
-        """
-        Adds beatmap to sql table
-        """
-        self.beatmaps_db.execute("INSERT INTO beatmaps VALUES (?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)",
-                                 (beatmap.size, beatmap.artist, beatmap.artist_unicode, beatmap.title, beatmap.title_unicode,
-                                  beatmap.mapper, beatmap.difficulty, beatmap.audio_file, beatmap.md5_hash, beatmap.osu_file,
-                                  str(pickle.dumps(beatmap.ranked_status)), beatmap.count_hitcircles, beatmap.count_sliders, beatmap.count_spinners, str(pickle.dumps(beatmap.last_modification)),
-                                  beatmap.ar, beatmap.cs, beatmap.hp, beatmap.od, beatmap.slider_velocity,
-                                  str(pickle.dumps(beatmap.std_pairs)), str(pickle.dumps(beatmap.taiko_pairs)), str(pickle.dumps(beatmap.ctb_pairs)), str(pickle.dumps(beatmap.mania_pairs)),
-                                  beatmap.drain_time, beatmap.total_time, beatmap.preview_time, str(pickle.dumps(beatmap.timing_points)), beatmap.difficulty_id, beatmap.beatmap_id,
-                                  beatmap.thread_id, str(pickle.dumps(beatmap.std_grade)), str(pickle.dumps(beatmap.taiko_grade)), str(pickle.dumps(beatmap.ctb_grade)), str(pickle.dumps(beatmap.mania_grade)),
-                                  beatmap.local_offset, beatmap.stack_leniency, str(pickle.dumps(beatmap.gameplay_mode)), beatmap.song_source, beatmap.song_tags,
-                                  beatmap.online_offset, beatmap.title_font, beatmap.unplayed, str(pickle.dumps(beatmap.last_played)), beatmap.is_osz2,
-                                  beatmap.folder_name, str(pickle.dumps(beatmap.last_checked)), beatmap.ignore_sound, beatmap.ignore_skin, beatmap.disable_storyboard,
-                                  beatmap.disable_video, beatmap.visual_override, beatmap.unknown, beatmap.last_modification2, beatmap.mania_scroll_speed))
-
-    def parse(self, connection: sqlite3.Connection = None, skip_beatmaps: bool = False) -> Osudb:
-        game_version = utils.read_uint(self.osu_db_file)
-        folder_count = utils.read_uint(self.osu_db_file)
-        account_unlocked = utils.read_bool(self.osu_db_file)
-        unlock_datetime = utils.read_datetime(self.osu_db_file)
-        username = utils.read_string(self.osu_db_file)
-        count_beatmaps = utils.read_uint(self.osu_db_file)
-
-        self.beatmaps_db = connection
-        if skip_beatmaps:
-            for _ in range(count_beatmaps):
-                Beatmap.parse(self.osu_db_file, game_version)
-        else:
-            self.generate_sql_db()
-            for _ in range(count_beatmaps):
-                self.add_beatmap_to_db(Beatmap.parse(self.osu_db_file, game_version))
-
-            self.beatmaps_db.commit()
-
-        user_permissions = UserPermissions(utils.read_uint(self.osu_db_file))
-
-        return Osudb(game_version, folder_count, account_unlocked, unlock_datetime, username, count_beatmaps, self.beatmaps_db, user_permissions)
-
-
-def parse_osudb(osudb_file: Union[str, os.PathLike, io.BytesIO], beatmaps_db: Union[str, os.PathLike] = None, skip_beatmaps: bool = False) -> Osudb:
-    """
-    Parse osu!.db file
-
-    Args
-    ----
-    osudb_file: str | os.PathLike | io.BytesIO
-        Path or opened file
-
-    beatmaps_db: str | os.PathLike = None
-        Path to sql database with beatmaps. \n
-        If None - creates temp file in system temp directory  \n
-        If non existing file, creates new one in that path  \n
-        If existing file, opens it  \n
-
-    skip_beatmaps: bool = False
-        Skip beatmap parsing. \n
-        Can decrease time for parsing, but beatmaps will be not available to use \n
-        (except if beatmaps_db is profided with existing file)
-
-    Returns
-    ----
-    Osudb
-        instance of Osudb class
-    """
-    if not isinstance(osudb_file, io.BytesIO):
-        osudb_file = open(osudb_file, "rb")
-
-    db_connection = None
-
-    if beatmaps_db is None:
-        db_connection = sqlite3.connect(tempfile.gettempdir() + "pyosudb_tmp.sql")
-    else:
-        db_connection = sqlite3.connect(beatmaps_db)
-
-    return _Parser(osudb_file).parse(db_connection, skip_beatmaps)
+from dataclasses import dataclass
+from typing import Union, Any, List
+import datetime
+import tempfile
+import sqlite3
+import pickle
+import io
+import os
+
+from pyosudb import utils
+from pyosudb.datatypes import Beatmap, UserPermissions
+
+
+@dataclass
+class Osudb:
+    """
+    Class representing osu!.db file
+
+    Attributes
+    ----
+    game_version: int
+        osu! version when this file created
+
+    folder_count: int
+        Amount of folders in "songs" folder
+
+    account_unlocked: bool
+        Is account banned. False if banned, True otherwise
+
+    unlock_datetime: datetime.datetime
+        Time until account will be unbanned. Always 0 if account is not banned (account_unlocked=True)
+
+    username: str
+        Player username
+
+    sql_beatmaps_db: sqlite3.Connection
+        Connection to sqllite3 database. It must not be set by the user
+
+    user_permissions: UserPermissions
+        User permissions in chat. Check UserPermissions class for more info
+    """
+    game_version: int
+    folder_count: int
+    account_unlocked: bool  # false if account banned/locked
+    unlock_datetime: datetime.datetime
+    username: str
+    count_beatmaps: int
+
+    sql_beatmaps_db: sqlite3.Connection
+
+    user_permissions: UserPermissions
+
+    # can't be saved because osu.db can be big and we don't need 20k objects with maps in our ram
+    def beatmaps(self) -> List[Beatmap]:
+        """
+        List of beatmaps
+
+        Returns
+        ----
+        List[Beatmaps]
+            List of Beatmaps instances
+        """
+        cursor = self.sql_beatmaps_db.cursor()
+        return [Beatmap.from_sql(*beatmap) for beatmap in cursor.execute("SELECT * FROM 'beatmaps' ").fetchall()]
+
+    def get_beatmap_from_hash(self, hash: str) -> Beatmap:
+        """
+        Get beatmap from sql table using hash
+
+        Args
+        ----
+        hash: str
+            beatmap hash
+
+        Returns
+        ----
+        Beatmap
+            instance of Beatmap
+        """
+        cursor = self.sql_beatmaps_db.cursor()
+        return Beatmap.from_sql(*cursor.execute(f"SELECT * FROM 'beatmaps' WHERE md5_hash='{hash}'").fetchone())
+
+    def beatmaps_execute_sql(self, command) -> Any:
+        """
+        Executes sql command in table with beatmaps
+        """
+        cursor = self.sql_beatmaps_db.cursor()
+        return cursor.execute(command).fetchall()
+
+
+class _Parser:
+    def __init__(self, osu_db_file) -> None:
+        self.osu_db_file = osu_db_file
+        self.offset = 0
+
+    def generate_sql_db(self) -> None:
+        """
+        Generates sql table for file
+        """
+        cursor = self.beatmaps_db.cursor()
+        cursor.execute("SELECT count(name) FROM sqlite_master WHERE type='table' AND name='beatmaps'")
+        if cursor.fetchone()[0] == 1:
+            self.beatmaps_db.execute("DROP TABLE beatmaps")
+        self.beatmaps_db.execute("""CREATE TABLE beatmaps (
+                            size INTEGER,
+                            artist TEXT,
+                            artist_unicode TEXT,
+                            title TEXT,
+                            title_unicode TEXT,
+                            mapper TEXT,
+                            difficulty TEXT,
+                            audio_file TEXT,
+                            md5_hash TEXT,
+                            osu_file TEXT,
+                            ranked_status TEXT,
+                            count_hitcircles INTEGER,
+                            count_sliders INTEGER,
+                            count_spinners INTEGER,
+                            last_modification TEXT,
+                            ar NUMERIC,
+                            cs NUMERIC,
+                            hp NUMERIC,
+                            od NUMERIC,
+                            slider_velocity NUMERIC,
+                            std_pairs TEXT,
+                            taiko_pairs TEXT,
+                            ctb_pairs TEXT,
+                            mania_pairs TEXT,
+                            drain_time INTEGER,
+                            total_time INTEGER,
+                            preview_time INTEGER,
+                            timing_points TEXT,
+                            difficulty_id INTEGER,
+                            beatmap_id INTEGER,
+                            thread_id INTEGER,
+                            std_grade TEXT,
+                            taiko_grade TEXT,
+                            ctb_grade TEXT,
+                            mania_grade TEXT,
+                            local_offset INTEGER,
+                            stack_leniency NUMERIC,
+                            gameplay_mode TEXT,
+                            song_source TEXT,
+                            song_tags TEXT,
+                            online_offset INTEGER,
+                            title_font TEXT,
+                            unplayed INTEGER,
+                            last_played INTEGER,
+                            is_osz2 INTEGER,
+                            folder_name TEXT,
+                            last_checked TEXT,
+                            ignore_sound INTEGER,
+                            ignore_skin INTEGER,
+                            disable_storyboard INTEGER,
+                            disable_video INTEGER,
+                            visual_override INTEGER,
+                            unknown INTEGER,
+                            last_modification2 TEXT,
+                            mania_scroll_speed INTEGER
+                        );""")
+
+    def add_beatmap_to_db(self, beatmap: Beatmap) -> None:
+        """
+        Adds beatmap to sql table
+        """
+        self.beatmaps_db.execute("INSERT INTO beatmaps VALUES (?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)",
+                                 (beatmap.size, beatmap.artist, beatmap.artist_unicode, beatmap.title, beatmap.title_unicode,
+                                  beatmap.mapper, beatmap.difficulty, beatmap.audio_file, beatmap.md5_hash, beatmap.osu_file,
+                                  str(pickle.dumps(beatmap.ranked_status)), beatmap.count_hitcircles, beatmap.count_sliders, beatmap.count_spinners, str(pickle.dumps(beatmap.last_modification)),
+                                  beatmap.ar, beatmap.cs, beatmap.hp, beatmap.od, beatmap.slider_velocity,
+                                  str(pickle.dumps(beatmap.std_pairs)), str(pickle.dumps(beatmap.taiko_pairs)), str(pickle.dumps(beatmap.ctb_pairs)), str(pickle.dumps(beatmap.mania_pairs)),
+                                  beatmap.drain_time, beatmap.total_time, beatmap.preview_time, str(pickle.dumps(beatmap.timing_points)), beatmap.difficulty_id, beatmap.beatmap_id,
+                                  beatmap.thread_id, str(pickle.dumps(beatmap.std_grade)), str(pickle.dumps(beatmap.taiko_grade)), str(pickle.dumps(beatmap.ctb_grade)), str(pickle.dumps(beatmap.mania_grade)),
+                                  beatmap.local_offset, beatmap.stack_leniency, str(pickle.dumps(beatmap.gameplay_mode)), beatmap.song_source, beatmap.song_tags,
+                                  beatmap.online_offset, beatmap.title_font, beatmap.unplayed, str(pickle.dumps(beatmap.last_played)), beatmap.is_osz2,
+                                  beatmap.folder_name, str(pickle.dumps(beatmap.last_checked)), beatmap.ignore_sound, beatmap.ignore_skin, beatmap.disable_storyboard,
+                                  beatmap.disable_video, beatmap.visual_override, beatmap.unknown, beatmap.last_modification2, beatmap.mania_scroll_speed))
+
+    def parse(self, connection: sqlite3.Connection = None, skip_beatmaps: bool = False) -> Osudb:
+        game_version = utils.read_uint(self.osu_db_file)
+        folder_count = utils.read_uint(self.osu_db_file)
+        account_unlocked = utils.read_bool(self.osu_db_file)
+        unlock_datetime = utils.read_datetime(self.osu_db_file)
+        username = utils.read_string(self.osu_db_file)
+        count_beatmaps = utils.read_uint(self.osu_db_file)
+
+        self.beatmaps_db = connection
+        if skip_beatmaps:
+            for _ in range(count_beatmaps):
+                Beatmap.parse(self.osu_db_file, game_version)
+        else:
+            self.generate_sql_db()
+            for _ in range(count_beatmaps):
+                self.add_beatmap_to_db(Beatmap.parse(self.osu_db_file, game_version))
+
+            self.beatmaps_db.commit()
+
+        user_permissions = UserPermissions(utils.read_uint(self.osu_db_file))
+
+        return Osudb(game_version, folder_count, account_unlocked, unlock_datetime, username, count_beatmaps, self.beatmaps_db, user_permissions)
+
+
+def parse_osudb(osudb_file: Union[str, os.PathLike, io.BytesIO], beatmaps_db: Union[str, os.PathLike] = None, skip_beatmaps: bool = False) -> Osudb:
+    """
+    Parse osu!.db file
+
+    Args
+    ----
+    osudb_file: str | os.PathLike | io.BytesIO
+        Path or opened file
+
+    beatmaps_db: str | os.PathLike = None
+        Path to sql database with beatmaps. \n
+        If None - creates temp file in system temp directory  \n
+        If non existing file, creates new one in that path  \n
+        If existing file, opens it  \n
+
+    skip_beatmaps: bool = False
+        Skip beatmap parsing. \n
+        Can decrease time for parsing, but beatmaps will be not available to use \n
+        (except if beatmaps_db is profided with existing file)
+
+    Returns
+    ----
+    Osudb
+        instance of Osudb class
+    """
+    if not isinstance(osudb_file, io.BytesIO):
+        osudb_file = open(osudb_file, "rb")
+
+    db_connection = None
+
+    if beatmaps_db is None:
+        db_connection = sqlite3.connect(tempfile.gettempdir() + "pyosudb_tmp.sql")
+    else:
+        db_connection = sqlite3.connect(beatmaps_db)
+
+    return _Parser(osudb_file).parse(db_connection, skip_beatmaps)
```

### Comparing `pyosudb-0.1.0/pyosudb/presencedb.py` & `pyosudb-0.1.1/pyosudb/presencedb.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from dataclasses import dataclass
-from typing import List
-
-from pyosudb import utils
-
-
-class _PresencedbParser:
-    def __init__(self, osu_db_file) -> None:
-        self.osu_db_file = osu_db_file
-        self.offset = 0
-
-    def parse(self):
-        version = utils.read_uint(self.osu_db_file)
-        count = utils.read_uint(self.osu_db_file)
-        # 2 ?
-        gamemode = utils.read_ubyte(self.osu_db_file)  # ?
-        # ?
-        rank = utils.read_uint(self.osu_db_file)
-        # return Presencedb(version, count)
-
-
-@dataclass
-class Presencedb:
-    """
-    DO NOT USE IT FOR NOW!
-
-    I'm currentry searching info about presence.db file, so this nit works.
-    """
-    version: int
-    count: int
-    values: List
-
-
-if __name__ == "__main__":
-    a = _PresencedbParser(open(r"C:\Users\olegrakov\Desktop\presence.db", "rb"))
-    a.parse()
+from dataclasses import dataclass
+from typing import List
+
+from pyosudb import utils
+
+
+class _PresencedbParser:
+    def __init__(self, osu_db_file) -> None:
+        self.osu_db_file = osu_db_file
+        self.offset = 0
+
+    def parse(self):
+        version = utils.read_uint(self.osu_db_file)
+        count = utils.read_uint(self.osu_db_file)
+        # 2 ?
+        gamemode = utils.read_ubyte(self.osu_db_file)  # ?
+        # ?
+        rank = utils.read_uint(self.osu_db_file)
+        # return Presencedb(version, count)
+
+
+@dataclass
+class Presencedb:
+    """
+    DO NOT USE IT FOR NOW!
+
+    I'm currentry searching info about presence.db file, so this nit works.
+    """
+    version: int
+    count: int
+    values: List
+
+
+if __name__ == "__main__":
+    a = _PresencedbParser(open(r"C:\Users\olegrakov\Desktop\presence.db", "rb"))
+    a.parse()
```

### Comparing `pyosudb-0.1.0/pyosudb/scoresdb.py` & `pyosudb-0.1.1/pyosudb/scoresdb.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from dataclasses import dataclass
-from typing import List, Union
-import os
-import io
-
-from pyosudb import utils
-from pyosudb.datatypes import BeatmapScores
-
-
-@dataclass
-class Scoresdb:
-    """
-    Class representing scores.db file
-
-    Attributes
-    ----
-    version: int
-        osu! version when this file created
-
-    count_beatmaps_scores: int
-        Amount of beatmaps scores in .db file
-
-    beatmaps_scores: List[BeatmapScores]
-        List of scores on beatmaps represented by "BeatmapScores" class
-    """
-    version: int
-    count_beatmaps_scores: int
-    beatmaps_scores: List[BeatmapScores]
-
-
-class _Parser:
-    def __init__(self, score_db_file) -> None:
-        self.score_db_file = score_db_file
-        self.offset = 0
-
-    def parse(self) -> Scoresdb:
-        version = utils.read_uint(self.score_db_file)
-        count_beatmaps = utils.read_uint(self.score_db_file)
-        beatmaps = []
-        for _ in range(count_beatmaps):
-            beatmaps.append(BeatmapScores.parse(self.score_db_file, version))
-
-        return Scoresdb(version, count_beatmaps, beatmaps)
-
-
-def parse_scoresdb(scoresdb_file: Union[str, os.PathLike, io.BytesIO]) -> Scoresdb:
-    """
-    Parse scores.db file
-
-    Args
-    ----
-    scoresdb_file: str | os.PathLike | io.BytesIO
-        Path or opened file
-
-    Returns
-    ----
-    scoresdb
-        instance of scoresdb class
-    """
-    if not isinstance(scoresdb_file, io.BytesIO):
-        scoresdb_file = open(scoresdb_file, "rb")
-
-    return _Parser(scoresdb_file).parse()
+from dataclasses import dataclass
+from typing import List, Union
+import os
+import io
+
+from pyosudb import utils
+from pyosudb.datatypes import BeatmapScores
+
+
+@dataclass
+class Scoresdb:
+    """
+    Class representing scores.db file
+
+    Attributes
+    ----
+    version: int
+        osu! version when this file created
+
+    count_beatmaps_scores: int
+        Amount of beatmaps scores in .db file
+
+    beatmaps_scores: List[BeatmapScores]
+        List of scores on beatmaps represented by "BeatmapScores" class
+    """
+    version: int
+    count_beatmaps_scores: int
+    beatmaps_scores: List[BeatmapScores]
+
+
+class _Parser:
+    def __init__(self, score_db_file) -> None:
+        self.score_db_file = score_db_file
+        self.offset = 0
+
+    def parse(self) -> Scoresdb:
+        version = utils.read_uint(self.score_db_file)
+        count_beatmaps = utils.read_uint(self.score_db_file)
+        beatmaps = []
+        for _ in range(count_beatmaps):
+            beatmaps.append(BeatmapScores.parse(self.score_db_file, version))
+
+        return Scoresdb(version, count_beatmaps, beatmaps)
+
+
+def parse_scoresdb(scoresdb_file: Union[str, os.PathLike, io.BytesIO]) -> Scoresdb:
+    """
+    Parse scores.db file
+
+    Args
+    ----
+    scoresdb_file: str | os.PathLike | io.BytesIO
+        Path or opened file
+
+    Returns
+    ----
+    scoresdb
+        instance of scoresdb class
+    """
+    if not isinstance(scoresdb_file, io.BytesIO):
+        scoresdb_file = open(scoresdb_file, "rb")
+
+    return _Parser(scoresdb_file).parse()
```

### Comparing `pyosudb-0.1.0/pyosudb/utils.py` & `pyosudb-0.1.1/pyosudb/utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import struct
-import datetime
-
-
-# PART OF CODE COPIED FROM https://github.com/jaasonw/osu-db-tools
-def read_bool(buffer) -> bool:
-    return struct.unpack("<?", buffer.read(1))[0]
-
-
-def read_ubyte(buffer) -> int:
-    return struct.unpack("<B", buffer.read(1))[0]
-
-
-def read_ushort(buffer) -> int:
-    return struct.unpack("<H", buffer.read(2))[0]
-
-
-def read_uint(buffer) -> int:
-    return struct.unpack("<I", buffer.read(4))[0]
-
-
-def read_float(buffer) -> float:
-    return struct.unpack("<f", buffer.read(4))[0]
-
-
-def read_double(buffer) -> float:
-    return struct.unpack("<d", buffer.read(8))[0]
-
-
-def read_ulong(buffer) -> int:
-    return struct.unpack("<Q", buffer.read(8))[0]
-
-
-# osu specific
-def read_int_double(buffer):
-    read_ubyte(buffer)
-    integer = read_uint(buffer)
-    read_ubyte(buffer)
-    double = read_double(buffer)
-    return (integer, double)
-
-
-def read_timing_point(buffer):
-    bpm = read_double(buffer)
-    offset = read_double(buffer)
-    inherited = read_bool(buffer)
-    return (bpm, offset, inherited)
-
-
-def read_string(buffer, encoding: str = "utf-8") -> str:
-    strlen = 0
-    strflag = read_ubyte(buffer)
-    if (strflag == 0x0b):
-        strlen = 0
-        shift = 0
-        # uleb128
-        # https://en.wikipedia.org/wiki/LEB128
-        while True:
-            byte = read_ubyte(buffer)
-            strlen |= ((byte & 0x7F) << shift)
-            if (byte & (1 << 7)) == 0:
-                break
-            shift += 7
-    return (struct.unpack("<" + str(strlen) + "s", buffer.read(strlen))[0]).decode(encoding)
-# PART OF CODE COPIED FROM https://github.com/jaasonw/osu-db-tools
-
-
-def read_datetime(buffer) -> datetime.datetime:
-    return datetime.datetime.min + datetime.timedelta(microseconds=read_ulong(buffer) / 10)
+import struct
+import datetime
+
+
+# PART OF CODE COPIED FROM https://github.com/jaasonw/osu-db-tools
+def read_bool(buffer) -> bool:
+    return struct.unpack("<?", buffer.read(1))[0]
+
+
+def read_ubyte(buffer) -> int:
+    return struct.unpack("<B", buffer.read(1))[0]
+
+
+def read_ushort(buffer) -> int:
+    return struct.unpack("<H", buffer.read(2))[0]
+
+
+def read_uint(buffer) -> int:
+    return struct.unpack("<I", buffer.read(4))[0]
+
+
+def read_float(buffer) -> float:
+    return struct.unpack("<f", buffer.read(4))[0]
+
+
+def read_double(buffer) -> float:
+    return struct.unpack("<d", buffer.read(8))[0]
+
+
+def read_ulong(buffer) -> int:
+    return struct.unpack("<Q", buffer.read(8))[0]
+
+
+# osu specific
+def read_int_double(buffer):
+    read_ubyte(buffer)
+    integer = read_uint(buffer)
+    read_ubyte(buffer)
+    double = read_double(buffer)
+    return (integer, double)
+
+
+def read_timing_point(buffer):
+    bpm = read_double(buffer)
+    offset = read_double(buffer)
+    inherited = read_bool(buffer)
+    return (bpm, offset, inherited)
+
+
+def read_string(buffer, encoding: str = "utf-8") -> str:
+    strlen = 0
+    strflag = read_ubyte(buffer)
+    if (strflag == 0x0b):
+        strlen = 0
+        shift = 0
+        # uleb128
+        # https://en.wikipedia.org/wiki/LEB128
+        while True:
+            byte = read_ubyte(buffer)
+            strlen |= ((byte & 0x7F) << shift)
+            if (byte & (1 << 7)) == 0:
+                break
+            shift += 7
+    return (struct.unpack("<" + str(strlen) + "s", buffer.read(strlen))[0]).decode(encoding)
+# PART OF CODE COPIED FROM https://github.com/jaasonw/osu-db-tools
+
+
+def read_datetime(buffer) -> datetime.datetime:
+    return datetime.datetime.min + datetime.timedelta(microseconds=read_ulong(buffer) / 10)
```

### Comparing `pyosudb-0.1.0/tests/test_parsing.py` & `pyosudb-0.1.1/tests/test_parsing.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from pathlib import Path
-from datetime import datetime
-
-import pyosudb
-from pyosudb.datatypes import UserPermissions
-
-RES = Path(__file__).parent / "resources"
-
-
-def test_parsing_osudb():
-    db = pyosudb.parse_osudb(RES / "osu!.db", RES / "tmp_osudb.sql")
-    assert db.game_version == 20230319
-    assert db.folder_count == 2736
-    assert db.account_unlocked is True
-    assert db.unlock_datetime == datetime.min
-    assert db.username == "OlegSuperBro"
-    assert db.count_beatmaps == 12020
-    assert len(db.beatmaps()) == db.count_beatmaps
-    assert db.user_permissions == UserPermissions.NORMAL
-
-
-def test_parsing_osudb_with_sql():
-    db = pyosudb.parse_osudb(RES / "osu!.db", RES / "beatmaps.sql", skip_beatmaps=True)
-    assert db.game_version == 20230319
-    assert db.folder_count == 2736
-    assert db.account_unlocked is True
-    assert db.unlock_datetime == datetime.min
-    assert db.username == "OlegSuperBro"
-    assert db.count_beatmaps == 12020
-    assert len(db.beatmaps()) == db.count_beatmaps
-    assert db.user_permissions == UserPermissions.NORMAL
+from pathlib import Path
+from datetime import datetime
+
+import pyosudb
+from pyosudb.datatypes import UserPermissions
+
+RES = Path(__file__).parent / "resources"
+
+
+def test_parsing_osudb():
+    db = pyosudb.parse_osudb(RES / "osu!.db", RES / "tmp_osudb.sql")
+    assert db.game_version == 20230319
+    assert db.folder_count == 2736
+    assert db.account_unlocked is True
+    assert db.unlock_datetime == datetime.min
+    assert db.username == "OlegSuperBro"
+    assert db.count_beatmaps == 12020
+    assert len(db.beatmaps()) == db.count_beatmaps
+    assert db.user_permissions == UserPermissions.NORMAL
+
+
+def test_parsing_osudb_with_sql():
+    db = pyosudb.parse_osudb(RES / "osu!.db", RES / "beatmaps.sql", skip_beatmaps=True)
+    assert db.game_version == 20230319
+    assert db.folder_count == 2736
+    assert db.account_unlocked is True
+    assert db.unlock_datetime == datetime.min
+    assert db.username == "OlegSuperBro"
+    assert db.count_beatmaps == 12020
+    assert len(db.beatmaps()) == db.count_beatmaps
+    assert db.user_permissions == UserPermissions.NORMAL
```

