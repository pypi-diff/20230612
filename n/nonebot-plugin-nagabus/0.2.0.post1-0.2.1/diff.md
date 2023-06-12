# Comparing `tmp/nonebot_plugin_nagabus-0.2.0.post1.tar.gz` & `tmp/nonebot_plugin_nagabus-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.2.0.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.2.1.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.2.0.post1.tar` & `nonebot_plugin_nagabus-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.0.post1/LICENSE
--rw-r--r--   0        0        0     1237 2023-06-01 03:26:14.711563 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-06-01 02:59:37.618752 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
--rw-r--r--   0        0        0     2873 2023-06-01 03:15:37.986641 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
--rw-r--r--   0        0        0     4828 2023-06-01 03:15:38.024057 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2420 2023-06-01 03:34:15.583151 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0     3089 2023-05-29 12:30:46.127834 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    20455 2023-05-30 02:38:14.130387 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0     1003 2023-06-01 06:53:39.708977 nonebot_plugin_nagabus-0.2.0.post1/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.0.post1/README.md
--rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.0.post1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1237 2023-06-01 03:26:14.711563 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-06-09 05:28:00.065113 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
+-rw-r--r--   0        0        0     2872 2023-06-09 05:28:24.454277 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
+-rw-r--r--   0        0        0     4650 2023-06-09 06:01:06.071925 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2420 2023-06-01 06:58:40.633672 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1617 2023-06-09 05:51:28.775960 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/70ff5fb4923e_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     3709 2023-06-09 06:12:20.123461 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0      436 2023-06-09 05:28:00.075631 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/errors.py
+-rw-r--r--   0        0        0     3415 2023-06-09 15:01:04.190237 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1248 2023-06-09 15:00:22.460735 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    21192 2023-06-09 14:41:10.459561 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0      347 2023-06-09 05:53:37.650409 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      997 2023-06-09 06:08:29.587244 nonebot_plugin_nagabus-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.2.1/README.md
+-rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/LICENSE` & `nonebot_plugin_nagabus-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/naga.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     __tablename__ = 'nonebot_plugin_nagabus_order'
     __table_args__ = {"extend_existing": True}
 
     haihu_id: Mapped[str] = mapped_column(primary_key=True)
     customer_id: Mapped[int]
     cost_np: Mapped[int]
     source: Mapped[NagaOrderSource]
-    model_type: Mapped[int]
+    model_type: Mapped[str]
     status: Mapped[NagaOrderStatus]
     naga_report: Mapped[Optional[str]]  # json of NagaReport
     create_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
     update_time: Mapped[datetime] = mapped_column(UTCDateTime)
 
 
 class MajsoulOrderOrm(SqlModel):
@@ -35,13 +35,13 @@
     __table_args__ = {"extend_existing": True}
 
     naga_haihu_id: Mapped[str] = mapped_column(ForeignKey("nonebot_plugin_nagabus_order.haihu_id", ondelete="cascade"),
                                                primary_key=True)
     paipu_uuid: Mapped[str] = mapped_column(index=True)
     kyoku: Mapped[int]
     honba: Mapped[int]
-    model_type: Mapped[int]
+    model_type: Mapped[str]
 
     order: Mapped[NagaOrderOrm] = relationship(foreign_keys="MajsoulOrderOrm.naga_haihu_id",
                                                cascade="save-update, delete",
                                                passive_deletes=True,
                                                lazy="joined")
```

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nonebot import logger
 from nonebot.exception import MatcherException, ActionFailed
 from nonebot.internal.matcher import current_matcher
 from nonebot_plugin_access_control.errors import RateLimitedError
 from nonebot_plugin_saa import MessageFactory
 
 from ..errors import BadRequestError
-from ...naga.service import OrderError, InvalidGameError, UnsupportedGameError
+from ...naga.errors import OrderError, InvalidGameError, UnsupportedGameError
 
 
 def handle_error(silently: bool = False):
     def decorator(func):
         @wraps(func)
         async def wrapped_func(*args, **kwargs):
             matcher = current_matcher.get()
```

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 
 from nonebot import on_command
 from nonebot.internal.matcher import Matcher
 from nonebot.internal.params import Depends
 from nonebot.params import CommandArg
 from nonebot_plugin_saa import MessageFactory
 from nonebot_plugin_session import extract_session, Session
-from nonebot_plugin_session.model import get_or_add_session_model
 
 from .errors import BadRequestError
 from .interceptors.handle_error import handle_error
 from ..ac import ac
 from ..naga import naga
-from ..naga.service import InvalidKyokuHonbaError
+from ..naga.errors import InvalidKyokuHonbaError
 from ..utils.integer import decode_integer
 from ..utils.nonebot import default_cmd_start
 
 analyze_srv = ac.create_subservice("analyze")
 
 
-async def analyze_majsoul(matcher: Matcher, customer_id: int, uuid: str, kyoku: int, honba: int):
+async def analyze_majsoul(matcher: Matcher, session: Session, uuid: str, kyoku: int, honba: int):
     try:
-        report, cost_np = await naga.analyze_majsoul(uuid, kyoku, honba, customer_id)
+        report, cost_np = await naga.analyze_majsoul(uuid, kyoku, honba, session)
         await MessageFactory(f"https://naga.dmv.nico/htmls/{report.report_id}.html?tw=0").send(reply=True)
 
         if cost_np == 0:
             token = matcher.state["ac_token"]
             await token.retire()
             await MessageFactory("由于此前已解析过该局，本次解析消耗0NP").send(reply=True)
         else:
@@ -40,82 +39,78 @@
                 kyoku_honba.append(f"南{kyoku - 3}局{honba}本场")
             else:
                 kyoku_honba.append(f"西{kyoku - 7}局{honba}本场")
 
         raise BadRequestError(f"请输入正确的场次与本场（{'、'.join(kyoku_honba)}）") from e
 
 
-async def analyze_tenhou(matcher: Matcher, customer_id: int, haihu_id: str, seat: int):
-    report, cost_np = await naga.analyze_tenhou(haihu_id, seat, customer_id)
+async def analyze_tenhou(matcher: Matcher, session: Session, haihu_id: str, seat: int):
+    report, cost_np = await naga.analyze_tenhou(haihu_id, seat, session)
     await MessageFactory(f"https://naga.dmv.nico/htmls/{report.report_id}.html?tw={seat}").send(reply=True)
 
     if cost_np == 0:
         token = matcher.state["ac_token"]
         await token.retire()
         await MessageFactory("由于此前已解析过该局，本次解析消耗0NP").send(reply=True)
     else:
         await MessageFactory(f"本次解析消耗{cost_np}NP").send(reply=True)
 
 
 naga_analyze_matcher = on_command("naga", priority=10)
 
 uuid_reg = re.compile(r"\d{6}-[\da-fA-F]{8}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{12}")
 
-kyoku_honba_reg = re.compile(r"([东南西])([一二三四1234])局([0123456789零一两二三四五六七八九十百千万亿]+)本场")
+kyoku_honba_reg = re.compile(r"([东南西])([一二三四1234])局(([0123456789零一两二三四五六七八九十百千万亿]+)本场)?")
 
 
 @naga_analyze_matcher.handle()
 @handle_error()
 @analyze_srv.patch_handler(retire_on_throw=True)
 async def naga_analyze(matcher: Matcher, cmd_args=CommandArg(),
                        session: Session = Depends(extract_session)):
-    model = await get_or_add_session_model(session)
-
     args = cmd_args.extract_plain_text().split(' ')
     if "maj-soul" in args[0]:
         mat = uuid_reg.search(args[0])
         if not mat:
             raise BadRequestError("不正确的雀魂牌谱")
 
         uuid = mat.group(0)
 
-        kyoku = None
-        honba = None
+        kyoku = -1
+        honba = -1
 
         if len(args) >= 2:
             mat = kyoku_honba_reg.search(args[1])
             if mat:
-                raw_wind, raw_kyoku, raw_honba = mat.groups()
+                raw_wind, raw_kyoku, _, raw_honba = mat.groups()
 
                 try:
                     kyoku = decode_integer(raw_kyoku) - 1
                     if raw_wind == '南':
                         kyoku += 4
                     elif raw_wind == '西':
                         kyoku += 8
 
-                    honba = decode_integer(raw_honba)
+                    if raw_honba is not None:
+                        honba = decode_integer(raw_honba)
                 except ValueError:
                     pass
 
-        if kyoku is None or honba is None:
-            await analyze_majsoul(matcher, model.id, uuid, -1, -1)  # 让其发送该局的场次本场信息
-        else:
-            await analyze_majsoul(matcher, model.id, uuid, kyoku, honba)
+        await analyze_majsoul(matcher, session, uuid, kyoku, honba)  # 如果未指定场次本场，则让其发送该局的场次本场信息
     elif "tenhou" in args[0]:
         tenhou_url = args[0].strip()
 
         _, _, _, _, tenhou_query, _ = urlparse(tenhou_url)
         tenhou_query = parse_qs(tenhou_query)
 
         haihu_id = tenhou_query["log"][0]
         seat = 0
         if "tw" in tenhou_query and len(tenhou_query["tw"]) > 0:
             seat = int(tenhou_query["tw"][0])
 
-        await analyze_tenhou(matcher, model.id, haihu_id, seat)
+        await analyze_tenhou(matcher, session, haihu_id, seat)
     else:
         await MessageFactory(
             "用法：\n"
             f"{default_cmd_start}naga <雀魂牌谱链接> <东/南x局x本场>：消耗10NP解析雀魂小局\n"
             f"{default_cmd_start}naga <天凤牌谱链接>：消耗50NP解析天凤半庄"
         ).send(reply=True)
```

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Sequence
 
 from httpx import AsyncClient
 from nonebot import logger
 from pydantic import BaseModel
 
 from .model import NagaReport, NagaOrder, NagaHanchanModelType, NagaTonpuuModelType, NagaGameRule
+from .utils import model_type_to_str
 
 
 class OrderReportList(BaseModel):
     report: List[NagaReport]
     order: List[NagaOrder]
 
 
@@ -53,20 +54,22 @@
                 "Referer": "https://naga.dmv.nico/naga_report/order_report_list/"
             },
             params={"year": year, "month": month}
         )
         return OrderReportList.parse_obj(resp.json())
 
     async def analyze_tenhou(self, haihu_id: str, seat: int,
-                             model_type: NagaHanchanModelType = NagaHanchanModelType.nishiki) -> AnalyzeTenhou:
+                             rule: NagaGameRule,
+                             model_type: Union[Sequence[NagaHanchanModelType],
+                                               Sequence[NagaHanchanModelType]]) -> AnalyzeTenhou:
         data = {
             "haihu_id": haihu_id,
             "seat": seat,
             "reanalysis": 0,
-            "player_type": model_type.value,
+            "player_types": model_type_to_str(model_type),
             "csrfmiddlewaretoken": self.client.cookies["csrftoken"]
         }
 
         resp = await self.client.post(
             "/url_analyze/",
             headers={
                 "Referer": "https://naga.dmv.nico/naga_report/order_form/"
@@ -75,31 +78,26 @@
         )
 
         if len(resp.content) > 0:
             return AnalyzeTenhou.parse_obj(resp.json())
         else:
             return AnalyzeTenhou(status=200, msg="")
 
-    async def analyze_custom(self, data: Union[list, str], seat: int = 0,
-                             rule: NagaGameRule = NagaGameRule.hanchan,
-                             model_type: Union[
-                                 NagaHanchanModelType, NagaTonpuuModelType] = NagaHanchanModelType.nishiki):
+    async def analyze_custom(self, data: Union[list, str], seat: int,
+                             rule: NagaGameRule,
+                             model_type: Union[Sequence[NagaHanchanModelType],
+                                               Sequence[NagaTonpuuModelType]]):
         if not isinstance(data, str):
             data = json.dumps(data, ensure_ascii=False)
 
-        if rule == NagaGameRule.hanchan:
-            assert isinstance(model_type, NagaHanchanModelType)
-        elif rule == NagaGameRule.tonpuu:
-            assert isinstance(model_type, NagaTonpuuModelType)
-
         res_data = {
             "json_data": data,
             "seat": seat,
             "game_type": rule.value,
-            "player_type": model_type.value,
+            "player_types": model_type_to_str(model_type),
             "csrfmiddlewaretoken": self.client.cookies["csrftoken"]
         }
 
         await self.client.post(
             "/custom_haihu_analyze/",
             headers={
                 "Referer": "https://naga.dmv.nico/naga_report/order_form/"
```

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 import asyncio
 import random
 from asyncio import create_task
 from datetime import datetime
-from typing import Union
+from typing import Union, Sequence
 from uuid import uuid4
 
 from nonebot import logger
 
 from nonebot_plugin_nagabus.naga.api import OrderReportList, AnalyzeTenhou
-from nonebot_plugin_nagabus.naga.model import NagaGameRule, NagaHanchanModelType, NagaTonpuuModelType, NagaOrder, \
-    NagaModel, NagaReport, NagaReportPlayer, NagaOrderStatus
+from nonebot_plugin_nagabus.naga.model import NagaGameRule, NagaHanchanModelType, NagaOrder, \
+    NagaReport, NagaReportPlayer, NagaOrderStatus, NagaModel
+from nonebot_plugin_nagabus.naga.utils import model_type_to_str
 from nonebot_plugin_nagabus.utils.tz import TZ_TOKYO
 
 
 class FakeNagaApi:
     def __init__(self):
         self.report = []
         self.order = []
 
     async def close(self):
         ...
 
     async def order_report_list(self, year: int, month: int) -> OrderReportList:
         return OrderReportList(report=self.report, order=self.order)
 
+    @logger.catch
     async def _produce_order(self, order: NagaOrder):
         await asyncio.sleep(1)
 
         self.order.insert(0, order)
         logger.debug(f"Insert order (haihu_id: {order.haihu_id})")
 
+    @logger.catch
     async def _produce_report(self, report: NagaReport):
         await asyncio.sleep(20)
 
         self.report.insert(0, report)
         logger.debug(f"Insert report (haihu_id: {report.haihu_id}, report_id: {report.report_id})")
 
-    async def analyze_custom(self, data: Union[dict, str], seat: int = 0,
-                             rule: NagaGameRule = NagaGameRule.hanchan,
-                             model_type: Union[
-                                 NagaHanchanModelType, NagaTonpuuModelType] = NagaHanchanModelType.nishiki):
+    async def analyze_custom(self, data: Union[dict, str], seat: int,
+                             rule: NagaGameRule,
+                             model_type: Union[Sequence[NagaHanchanModelType],
+                                               Sequence[NagaHanchanModelType]]):
         time = datetime.now(tz=TZ_TOKYO).replace(tzinfo=None).isoformat(timespec='seconds')
         feat = ''.join(str(random.randint(1, 9)) for _ in range(16))
         haihu_id = f"custom_haihu_{time}_{feat}"
-        order = NagaOrder(haihu_id=haihu_id, status=NagaOrderStatus.ok, model=NagaModel(2, 0, model_type), rule=rule)
+        order = NagaOrder(haihu_id=haihu_id, status=NagaOrderStatus.ok,
+                          model=NagaModel(2, 2, 0, model_type_to_str(model_type)), rule=rule)
         create_task(self._produce_order(order))
 
         report_id = str(uuid4())
         report = NagaReport(haihu_id=haihu_id, players=[NagaReportPlayer("AI", 0)] * 4, report_id=report_id, seat=0,
-                            model=NagaModel(2, 0, model_type), rule=rule)
+                            model=NagaModel(2, 2, 0, model_type_to_str(model_type)), rule=rule)
         create_task(self._produce_report(report))
 
     async def analyze_tenhou(self, haihu_id: str, seat: int,
-                             model_type: NagaHanchanModelType = NagaHanchanModelType.nishiki) -> AnalyzeTenhou:
+                             rule: NagaGameRule,
+                             model_type: Union[Sequence[NagaHanchanModelType],
+                                               Sequence[NagaHanchanModelType]]) -> AnalyzeTenhou:
         for o in self.order:
             if o.haihu_id == haihu_id:
                 return AnalyzeTenhou(status=400, msg="すでに解析済みの牌譜です")
 
-        order = NagaOrder(haihu_id=haihu_id, status=NagaOrderStatus.ok, model=NagaModel(2, 0, model_type),
+        order = NagaOrder(haihu_id=haihu_id, status=NagaOrderStatus.ok,
+                          model=NagaModel(2, 2, 0, model_type_to_str(model_type)),
                           rule=NagaGameRule.hanchan)
         create_task(self._produce_order(order))
 
         report_id = str(uuid4())
         report = NagaReport(haihu_id=haihu_id, players=[NagaReportPlayer("AI", 0)] * 4, report_id=report_id, seat=seat,
-                            model=NagaModel(2, 0, model_type), rule=NagaGameRule.hanchan)
+                            model=NagaModel(2, 2, 0, model_type_to_str(model_type)), rule=NagaGameRule.hanchan)
         create_task(self._produce_report(report))
 
         return AnalyzeTenhou(status=200, msg="")
```

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import IntEnum
-from typing import List, NamedTuple
+from typing import List, NamedTuple, Any
 
 
 class NagaGameRule(IntEnum):
     hanchan = 0
     tonpuu = 1
 
 
@@ -24,15 +24,16 @@
     nickname: str
     pt: int
 
 
 class NagaModel(NamedTuple):
     major: int
     minor: int
-    type: int
+    old_type: int  # 新版本恒为0，旧版本为NagaHanchanModelType/NagaTonpuuModelType的枚举值
+    type: str  # NagaHanchanModelType/NagaTonpuuModelType的枚举值，逗号分隔
 
 
 class NagaReport(NamedTuple):
     haihu_id: str
     players: List[NagaReportPlayer]
     report_id: str
     seat: int
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/naga/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import asyncio
 import json
 import re
 from asyncio import Lock
 from datetime import datetime, timezone
 from inspect import isawaitable
-from typing import Dict, Union, Optional, List, Tuple
+from typing import Dict, Union, Optional, List, Sequence
 
 from monthdelta import monthdelta
 from nonebot import logger
+from nonebot_plugin_session import Session
+from nonebot_plugin_session.model import get_or_add_session_model
 from sqlalchemy import select, update
 from tensoul.downloader import MajsoulDownloadError
 
 from .api import NagaApi, OrderReportList
+from .errors import InvalidGameError, UnsupportedGameError, OrderError, InvalidKyokuHonbaError
 from .fake_api import FakeNagaApi
 from .model import NagaGameRule, NagaHanchanModelType, NagaTonpuuModelType, NagaOrder, NagaReport, NagaOrderStatus, \
     NagaServiceOrder, NagaServiceUserStatistic
+from .utils import model_type_to_str
 from ..config import conf
 from ..data.naga import MajsoulOrderOrm, NagaOrderOrm, NagaOrderSource
 from ..data.session import get_session
 from ..mjs import get_majsoul_paipu
 from ..utils.tz import TZ_TOKYO
 
 DURATION = 2
@@ -27,66 +31,51 @@
 class ObservableOrderReport:
     def __init__(self, api: NagaApi):
         self.api = api
         self.value = None
         self._observers = []
         self._refresh_worker = None
 
-    async def _refresh(self):
-        while True:
-            observers = self._observers
-            self._observers = []
-
-            if len(observers) != 0:
-                logger.trace("refreshing naga orders and reports...")
-
-                current = datetime.now(tz=TZ_TOKYO)
-                prev_month = current - monthdelta(months=1)
+    @logger.catch
+    async def _refresh_once(self):
+        current = datetime.now(tz=TZ_TOKYO)
+        prev_month = current - monthdelta(months=1)
 
-                list_this_month = await self.api.order_report_list(current.year, current.month)
-                list_prev_month = await self.api.order_report_list(prev_month.year, prev_month.month)
+        list_this_month = await self.api.order_report_list(current.year, current.month)
+        list_prev_month = await self.api.order_report_list(prev_month.year, prev_month.month)
 
-                self.value = OrderReportList(report=[*list_this_month.report, *list_prev_month.report],
-                                             order=[*list_this_month.order, *list_prev_month.order])
+        self.value = OrderReportList(report=[*list_this_month.report, *list_prev_month.report],
+                                     order=[*list_this_month.order, *list_prev_month.order])
 
-                for ob in observers:
-                    x = ob(self.value)
-                    if isawaitable(x):
-                        await x
+    async def _refresh(self):
+        while True:
+            try:
+                if len(self._observers) != 0:
+                    logger.trace("refreshing naga orders and reports...")
+
+                    await self._refresh_once()
+
+                    observers = self._observers
+                    self._observers = []
+
+                    for ob in observers:
+                        x = ob(self.value)
+                        if isawaitable(x):
+                            await x
+            except BaseException as e:
+                logger.exception(e)
 
             await asyncio.sleep(DURATION)
 
     def observe_once(self, callback):
         self._observers.append(callback)
         if self._refresh_worker is None:
             self._refresh_worker = asyncio.create_task(self._refresh())
 
 
-class NagaError(BaseException):
-    ...
-
-
-class OrderError(NagaError):
-    ...
-
-
-class InvalidGameError(NagaError):
-    ...
-
-
-class UnsupportedGameError(NagaError):
-    ...
-
-
-class InvalidKyokuHonbaError(NagaError):
-    def __init__(self, available_kyoku_honba: List[Tuple[int, int]]):
-        super().__init__()
-        self.available_kyoku_honba = available_kyoku_honba
-
-
 class NagaService:
     _tenhou_haihu_id_reg = re.compile(r"^20\d{8}gm-[a-f\d]{4}-[a-z\d]{4,5}-[a-zA-Z\d]{8}$")
 
     def __init__(self, cookies: Dict[str, str], timeout: float = 90.0):
         if conf.naga_fake_api:
             self.api = FakeNagaApi()
             logger.warning("using fake naga api")
@@ -131,16 +120,16 @@
             else:
                 return await report
         finally:
             cancel_flag = True
 
     async def _order_custom(self, data: Union[list, str],
                             rule: NagaGameRule,
-                            model_type: Union[NagaHanchanModelType,
-                                              NagaTonpuuModelType]) -> NagaOrder:
+                            model_type: Union[None, Sequence[NagaHanchanModelType],
+                                              Sequence[NagaTonpuuModelType]] = None) -> NagaOrder:
         current = datetime.now(tz=TZ_TOKYO)
         await self.api.analyze_custom(data, 0, rule, model_type)
 
         order_fut = asyncio.get_running_loop().create_future()
         retry = 0  # 下单完马上获取order的话，有时候order刷新不出来，可以多试几次
 
         def _make_callback():
@@ -174,19 +163,37 @@
 
             return callback
 
         self._order_report.observe_once(_make_callback())
 
         return await order_fut
 
-    async def analyze_majsoul(self, majsoul_uuid: str, kyoku: int, honba: int,
-                              customer_id: int,
-                              *,
-                              model_type: Union[NagaHanchanModelType,
-                                                NagaTonpuuModelType, None] = None) -> NagaServiceOrder:
+    @staticmethod
+    def _handle_model_type(rule: NagaGameRule,
+                           model_type: Union[None, Sequence[NagaHanchanModelType],
+                                             Sequence[NagaHanchanModelType]]) -> Union[Sequence[NagaHanchanModelType],
+                                                                                       Sequence[NagaHanchanModelType]]:
+        if rule == NagaGameRule.hanchan:
+            if model_type is None:
+                model_type = [NagaHanchanModelType.nishiki, NagaHanchanModelType.kagashi]
+            assert isinstance(model_type, list) or isinstance(model_type, tuple)
+            for t in model_type:
+                assert isinstance(t, NagaHanchanModelType)
+        elif rule == NagaGameRule.tonpuu:
+            if model_type is None:
+                model_type = [NagaTonpuuModelType.nu, NagaTonpuuModelType.sigma]
+            assert isinstance(model_type, list) or isinstance(model_type, tuple)
+            for t in model_type:
+                assert isinstance(t, NagaTonpuuModelType)
+
+        return model_type
+
+    async def analyze_majsoul(self, majsoul_uuid: str, kyoku: int, honba: int, session: Session,
+                              *, model_type: Union[None, Sequence[NagaHanchanModelType],
+                                                   Sequence[NagaTonpuuModelType]] = None) -> NagaServiceOrder:
         sess = get_session()
 
         try:
             data = await get_majsoul_paipu(majsoul_uuid)
         except MajsoulDownloadError as e:
             logger.opt(colors=True).warning(f"Failed to download paipu <y>{majsoul_uuid}</y>, code: {e.code}")
             if e.code == 1203:
@@ -198,148 +205,151 @@
             raise UnsupportedGameError("only yonma game is supported")
 
         if "東" in data["rule"]["disp"]:
             rule = NagaGameRule.tonpuu
         else:
             rule = NagaGameRule.hanchan
 
-        if model_type is None:
-            if rule == NagaGameRule.hanchan:
-                model_type = NagaHanchanModelType.nishiki
-            else:
-                model_type = NagaTonpuuModelType.sigma
+        log = None
+        for i, l in enumerate(data["log"]):
+            if l[0][0] == kyoku:
+                if honba == -1:
+                    # 未指定本场
+                    if (i == 0 or data["log"][i - 1][0][0] != kyoku) \
+                            and (i == len(data["log"]) - 1 or data["log"][i + 1][0][0] != kyoku):
+                        # 该场次只存在一个本场
+                        honba = l[0][1]
+                        log = l
+                    break
+                elif l[0][1] == honba:
+                    log = l
+                    break
+
+        if log is None:
+            available_kyoku_honba = [(l[0][0], l[0][1]) for l in data["log"]]
+            raise InvalidKyokuHonbaError(available_kyoku_honba)
+
+        model_type = self._handle_model_type(rule, model_type)
+        model_type_str = model_type_to_str(model_type)
 
         haihu_id = ""
         new_order = False
 
         async def _get_local_order() -> Optional[NagaOrderOrm]:
             stmt = select(MajsoulOrderOrm).where(MajsoulOrderOrm.paipu_uuid == majsoul_uuid,
                                                  MajsoulOrderOrm.kyoku == kyoku,
                                                  MajsoulOrderOrm.honba == honba,
-                                                 MajsoulOrderOrm.model_type == model_type.value)
+                                                 MajsoulOrderOrm.model_type == model_type_str)
 
             order_orm: Optional[MajsoulOrderOrm] = (await sess.execute(stmt)).scalar_one_or_none()
             if order_orm is not None:
                 if order_orm.order.status == NagaOrderStatus.ok or \
                         datetime.now(tz=timezone.utc).timestamp() - order_orm.order.update_time.timestamp() < 90:
                     return order_orm.order
                 else:  # 超过90s仍未分析完成则删除重来
                     logger.opt(colors=True).info(f"Delete majsoul paipu <y>{majsoul_uuid} "
-                                                 f"(kyoku: {kyoku}, honba: {honba}, "
-                                                 f"model_type: {model_type.name})</y> analyze order: {order_orm.naga_haihu_id}, "
+                                                 f"(kyoku: {kyoku}, honba: {honba})</y> "
+                                                 f"analyze order: {order_orm.naga_haihu_id}, "
                                                  f"because it takes over 90 seconds and still not done")
                     await sess.delete(order_orm.order)
                     await sess.delete(order_orm)
                     await sess.commit()
                     return None
 
         # 加锁防止重复下单
         local_order = await _get_local_order()
         if local_order is None:
             async with self._majsoul_order_mutex:
                 local_order = await _get_local_order()
                 if local_order is None:
                     # 不存在记录，安排解析
                     logger.opt(colors=True).info(f"Ordering majsoul paipu <y>{majsoul_uuid} "
-                                                 f"(kyoku: {kyoku}, honba: {honba}, "
-                                                 f"model_type: {model_type.name})</y> analyze...")
-
-                    log = None
-                    for l in data["log"]:
-                        if l[0][0] == kyoku and l[0][1] == honba:
-                            log = l
-                            break
-
-                    if log is None:
-                        available_kyoku_honba = [(l[0][0], l[0][1]) for l in data["log"]]
-                        raise InvalidKyokuHonbaError(available_kyoku_honba)
+                                                 f"(kyoku: {kyoku}, honba: {honba})</y> analyze...")
 
                     # data["log"] = log
                     data = {
                         "title": data["title"],
                         "name": data["name"],
                         "rule": data["rule"],
                         "log": [log]
                     }
 
                     order = await self._order_custom([data], rule, model_type)
                     haihu_id = order.haihu_id
 
                     new_order = True
 
+                    session_model = await get_or_add_session_model(session, sess)
                     order_orm = NagaOrderOrm(haihu_id=haihu_id,
-                                             customer_id=customer_id,
+                                             customer_id=session_model.id,
                                              cost_np=10,
                                              source=NagaOrderSource.majsoul,
-                                             model_type=model_type.value,
+                                             model_type=model_type_str,
                                              status=NagaOrderStatus.analyzing,
                                              create_time=datetime.now(tz=timezone.utc),
                                              update_time=datetime.now(tz=timezone.utc))
 
                     majsoul_order_orm = MajsoulOrderOrm(naga_haihu_id=haihu_id,
                                                         paipu_uuid=majsoul_uuid,
                                                         kyoku=kyoku,
                                                         honba=honba,
-                                                        model_type=model_type.value,
+                                                        model_type=model_type_str,
                                                         order=order_orm)
 
                     sess.add(order_orm)
                     sess.add(majsoul_order_orm)
                     await sess.commit()
 
         if local_order is not None:
             # 存在记录
             if local_order.status == NagaOrderStatus.ok:
                 logger.opt(colors=True).info(f"Found a existing majsoul paipu <y>{majsoul_uuid} "
-                                             f"(kyoku: {kyoku}, honba: {honba}, "
-                                             f"model_type: {model_type.name})</y> "
+                                             f"(kyoku: {kyoku}, honba: {honba})</y> "
                                              f"analyze report: {local_order.haihu_id}")
                 report = NagaReport(*json.loads(local_order.naga_report))
                 return NagaServiceOrder(report, 0)
 
             haihu_id = local_order.naga_haihu_id
             logger.opt(colors=True).info(f"Found a processing majsoul paipu <y>{majsoul_uuid} "
-                                         f"(kyoku: {kyoku}, honba: {honba}, "
-                                         f"model_type: {model_type.name})</y> "
+                                         f"(kyoku: {kyoku}, honba: {honba})</y> "
                                          f"analyze order: {haihu_id}")
 
         assert haihu_id != ""
 
         logger.opt(colors=True).info(f"Waiting for majsoul paipu <y>{majsoul_uuid} "
-                                     f"(kyoku: {kyoku}, honba: {honba}, "
-                                     f"model_type: {model_type.name})</y> "
+                                     f"(kyoku: {kyoku}, honba: {honba})</y> "
                                      f"analyze report: {haihu_id} ...")
         report = await self._get_report(haihu_id)
 
         if new_order:
             # 需要更新之前创建的NagaOrderOrm
             logger.opt(colors=True).debug(f"Updating majsoul paipu <y>{majsoul_uuid} "
-                                          f"(kyoku: {kyoku}, honba: {honba}, "
-                                          f"model_type: {model_type.name})</y> "
+                                          f"(kyoku: {kyoku}, honba: {honba})</y> "
                                           f"analyze report: {haihu_id}...")
             stmt = update(NagaOrderOrm).where(NagaOrderOrm.haihu_id == haihu_id).values(
                 status=NagaOrderStatus.ok, naga_report=json.dumps(report), update_time=datetime.now(timezone.utc)
             )
             await sess.execute(stmt)
             await sess.commit()
 
             return NagaServiceOrder(report, 10)
         else:
             return NagaServiceOrder(report, 0)
 
-    async def _order_tenhou(self, haihu_id: str, seat: int, model_type: NagaHanchanModelType):
-        res = await self.api.analyze_tenhou(haihu_id, seat, model_type)
+    async def _order_tenhou(self, haihu_id: str, seat: int, rule: NagaGameRule,
+                            model_type: Union[None, Sequence[NagaHanchanModelType],
+                                              Sequence[NagaHanchanModelType]] = None):
+        res = await self.api.analyze_tenhou(haihu_id, seat, rule, model_type)
         if res.status != 200:
             raise OrderError(res.msg)
 
     # needs test
-    async def analyze_tenhou(self, haihu_id: str, seat: int, customer_id: int,
-                             *,
-                             model_type: Union[NagaHanchanModelType,
-                                               NagaTonpuuModelType, None] = None) -> NagaServiceOrder:
+    async def analyze_tenhou(self, haihu_id: str, seat: int, session: Session,
+                             *, model_type: Union[None, Sequence[NagaHanchanModelType],
+                                                  Sequence[NagaHanchanModelType]] = None) -> NagaServiceOrder:
         sess = get_session()
 
         if not self._tenhou_haihu_id_reg.match(haihu_id):
             raise InvalidGameError(f"invalid haihu_id: {haihu_id}")
 
         haihu_element = haihu_id.split('-')
         if len(haihu_element) != 4:
@@ -352,87 +362,80 @@
         is_online = bool(haihu_rule & 1)
 
         if is_yonma and is_kuitan and is_online:
             rule = NagaGameRule.hanchan if is_hanchan else NagaGameRule.tonpuu
         else:
             raise UnsupportedGameError("only online kuitan yonma game is supported")
 
-        if model_type is None:
-            if rule == NagaGameRule.hanchan:
-                model_type = NagaHanchanModelType.nishiki
-            else:
-                model_type = NagaTonpuuModelType.sigma
+        model_type = self._handle_model_type(rule, model_type)
+        model_type_str = model_type_to_str(model_type)
 
         new_order = False
 
         async def _get_local_order() -> Optional[NagaOrderOrm]:
             stmt = select(NagaOrderOrm).where(NagaOrderOrm.haihu_id == haihu_id,
-                                              NagaOrderOrm.model_type == model_type.value)
+                                              NagaOrderOrm.model_type == model_type_str)
 
             order_orm: Optional[NagaOrderOrm] = (await sess.execute(stmt)).scalar_one_or_none()
             if order_orm is not None:
                 if order_orm.status == NagaOrderStatus.ok or \
                         datetime.now(tz=timezone.utc).timestamp() - order_orm.update_time.timestamp() < 300:
                     return order_orm
                 else:  # 超过90s仍未分析完成则删除重来
-                    logger.opt(colors=True).info(f"Delete tenhou paipu <y>{haihu_id} "
-                                                 f"(model_type: {model_type.name})</y> analyze order "
+                    logger.opt(colors=True).info(f"Delete tenhou paipu <y>{haihu_id}</y> analyze order "
                                                  f"because it takes over 90 seconds and still not done")
                     await sess.delete(order_orm)
                     await sess.commit()
                     return None
 
         # 加锁防止重复下单
         local_order = await _get_local_order()
         if local_order is None:
             async with self._tenhou_order_mutex:
                 local_order = await _get_local_order()
                 if local_order is None:
                     # 不存在记录，安排解析
-                    logger.opt(colors=True).info(f"Ordering tenhou paipu <y>{haihu_id} "
-                                                 f"(model_type: {model_type.name})</y> analyze...")
+                    logger.opt(colors=True).info(f"Ordering tenhou paipu <y>{haihu_id}</y> analyze...")
 
-                    await self._order_tenhou(haihu_id, seat, model_type)
+                    await self._order_tenhou(haihu_id, seat, rule, model_type)
 
                     new_order = True
 
+                    session_model = await get_or_add_session_model(session, sess)
+
                     order_orm = NagaOrderOrm(haihu_id=haihu_id,
-                                             customer_id=customer_id,
+                                             customer_id=session_model.id,
                                              cost_np=50 if rule == NagaGameRule.hanchan else 30,
                                              source=NagaOrderSource.tenhou,
-                                             model_type=model_type.value,
+                                             model_type=model_type_str,
                                              status=NagaOrderStatus.analyzing,
                                              create_time=datetime.now(tz=timezone.utc),
                                              update_time=datetime.now(tz=timezone.utc))
 
                     sess.add(order_orm)
                     await sess.commit()
 
         if local_order is not None:
             # 存在记录
             if local_order.status == NagaOrderStatus.ok:
-                logger.opt(colors=True).info(f"Found a existing tenhou paipu <y>{haihu_id} "
-                                             f"(model_type: {model_type.name})</y> "
+                logger.opt(colors=True).info(f"Found a existing tenhou paipu <y>{haihu_id})</y> "
                                              "analyze report")
                 report = NagaReport(*json.loads(local_order.naga_report))
                 return NagaServiceOrder(report, 0)
 
-            logger.opt(colors=True).info(f"Found a processing tenhou paipu <y>{haihu_id} "
-                                         f"(model_type: {model_type.name})</y> "
+            logger.opt(colors=True).info(f"Found a processing tenhou paipu <y>{haihu_id})</y> "
                                          "analyze order")
 
-        logger.opt(colors=True).info(f"Waiting for tenhou paipu <y>{haihu_id} "
-                                     f"(model_type: {model_type.name})</y> "
+        logger.opt(colors=True).info(f"Waiting for tenhou paipu <y>{haihu_id})</y> "
                                      f"analyze report...")
         report = await self._get_report(haihu_id)
 
         if new_order:
             # 需要更新之前创建的NagaOrderOrm
-            logger.opt(colors=True).debug(f"Updating tenhou paipu <y>{haihu_id} "
-                                          f"(model_type: {model_type.name})</y> "
+            logger.opt(colors=True).debug(f"Updating tenhou paipu <y>{haihu_id})</y> "
                                           "analyze report...")
             stmt = update(NagaOrderOrm).where(NagaOrderOrm.haihu_id == haihu_id).values(
                 status=NagaOrderStatus.ok, naga_report=json.dumps(report), update_time=datetime.now(timezone.utc)
             )
             await sess.execute(stmt)
             await sess.commit()
```

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.2.1/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/pyproject.toml` & `nonebot_plugin_nagabus-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.2.0.post1"
+version = "0.2.1"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/README.md` & `nonebot_plugin_nagabus-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.2.0.post1/PKG-INFO` & `nonebot_plugin_nagabus-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.2.0.post1
+Version: 0.2.1
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

