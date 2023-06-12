# Comparing `tmp/dimples-0.1.7.tar.gz` & `tmp/dimples-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimples-0.1.7.tar", last modified: Fri Jun  9 17:20:51 2023, max compression
+gzip compressed data, was "dist/dimples-0.1.8.tar", last modified: Mon Jun 12 15:42:23 2023, max compression
```

## Comparing `dimples-0.1.7.tar` & `dimples-0.1.8.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-09 17:20:51.000000 dimples-0.1.7/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.1.7/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/
--rw-r--r--   0 moky       (501) staff       (20)     7071 2023-06-03 12:10:17.000000 dimples-0.1.7/dimples/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/client/
--rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.1.7/dimples/client/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/client/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     2191 2023-06-09 16:37:34.000000 dimples-0.1.7/dimples/client/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.1.7/dimples/client/cpu/grp_expel.py
--rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.1.7/dimples/client/cpu/grp_invite.py
--rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.1.7/dimples/client/cpu/grp_query.py
--rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.1.7/dimples/client/cpu/grp_quit.py
--rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.1.7/dimples/client/cpu/grp_reset.py
--rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.1.7/dimples/client/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/client/cpu/history.py
--rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/client/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/client/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.1.7/dimples/client/cpu/text.py
--rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.1.7/dimples/client/group.py
--rw-r--r--   0 moky       (501) staff       (20)     7713 2023-06-06 16:33:40.000000 dimples-0.1.7/dimples/client/messenger.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/client/network/
--rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.1.7/dimples/client/network/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.1.7/dimples/client/network/session.py
--rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.1.7/dimples/client/network/state.py
--rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/client/network/transition.py
--rw-r--r--   0 moky       (501) staff       (20)     6560 2023-06-06 16:21:36.000000 dimples-0.1.7/dimples/client/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     7190 2023-06-09 16:42:29.000000 dimples-0.1.7/dimples/client/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.1.7/dimples/client/terminal.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/common/
--rw-r--r--   0 moky       (501) staff       (20)     2209 2023-06-06 13:30:28.000000 dimples-0.1.7/dimples/common/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4322 2023-06-02 08:44:29.000000 dimples-0.1.7/dimples/common/ans.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/common/dbi/
--rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.1.7/dimples/common/dbi/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.1.7/dimples/common/dbi/account.py
--rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.1.7/dimples/common/dbi/message.py
--rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.1.7/dimples/common/dbi/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.1.7/dimples/common/facebook.py
--rw-r--r--   0 moky       (501) staff       (20)     7945 2023-06-09 16:13:09.000000 dimples-0.1.7/dimples/common/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     7918 2023-06-06 16:22:19.000000 dimples-0.1.7/dimples/common/packer.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/common/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2536 2023-02-23 09:20:27.000000 dimples-0.1.7/dimples/common/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.1.7/dimples/common/protocol/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.1.7/dimples/common/protocol/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.1.7/dimples/common/protocol/login.py
--rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.1.7/dimples/common/protocol/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.1.7/dimples/common/protocol/report.py
--rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.1.7/dimples/common/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.1.7/dimples/config.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/conn/
--rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.1.7/dimples/conn/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.1.7/dimples/conn/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/conn/gatekeeper.py
--rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.1.7/dimples/conn/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.1.7/dimples/conn/mtp.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/conn/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/conn/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/conn/protocol/mars.py
--rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/conn/protocol/ws.py
--rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.1.7/dimples/conn/queue.py
--rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.1.7/dimples/conn/seeker.py
--rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.1.7/dimples/conn/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.1.7/dimples/conn/ws.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/database/
--rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.1.7/dimples/database/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.1.7/dimples/database/account.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/database/dos/
--rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.1.7/dimples/database/dos/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.1.7/dimples/database/dos/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/database/dos/document.py
--rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.1.7/dimples/database/dos/group.py
--rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.1.7/dimples/database/dos/login.py
--rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.1.7/dimples/database/dos/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.1.7/dimples/database/dos/private.py
--rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.1.7/dimples/database/dos/station.py
--rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.1.7/dimples/database/dos/user.py
--rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.1.7/dimples/database/message.py
--rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.1.7/dimples/database/session.py
--rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/database/t_cipherkey.py
--rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.1.7/dimples/database/t_document.py
--rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.1.7/dimples/database/t_group.py
--rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.1.7/dimples/database/t_login.py
--rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.1.7/dimples/database/t_message.py
--rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.1.7/dimples/database/t_meta.py
--rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.1.7/dimples/database/t_private.py
--rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.1.7/dimples/database/t_station.py
--rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.1.7/dimples/database/t_user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples/edge/
--rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/edge/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    13562 2023-06-09 14:59:48.000000 dimples-0.1.7/dimples/edge/octopus.py
--rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.1.7/dimples/edge/shared.py
--rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.1.7/dimples/edge/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/register/
--rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/register/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.1.7/dimples/register/generate.py
--rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.1.7/dimples/register/modify.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/register/run.py
--rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/register/shared.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/server/
--rw-r--r--   0 moky       (501) staff       (20)     2561 2023-06-07 12:19:50.000000 dimples-0.1.7/dimples/server/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/server/cpu/
--rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.1.7/dimples/server/cpu/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2640 2023-02-23 10:54:44.000000 dimples-0.1.7/dimples/server/cpu/ans.py
--rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.1.7/dimples/server/cpu/document.py
--rw-r--r--   0 moky       (501) staff       (20)     3341 2023-04-14 16:24:15.000000 dimples-0.1.7/dimples/server/cpu/handshake.py
--rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.1.7/dimples/server/cpu/login.py
--rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/server/cpu/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.1.7/dimples/server/cpu/report.py
--rw-r--r--   0 moky       (501) staff       (20)    13057 2023-06-09 13:06:31.000000 dimples-0.1.7/dimples/server/dispatcher.py
--rw-r--r--   0 moky       (501) staff       (20)    12628 2023-06-09 17:18:59.000000 dimples-0.1.7/dimples/server/messenger.py
--rw-r--r--   0 moky       (501) staff       (20)     6659 2023-06-09 08:36:13.000000 dimples-0.1.7/dimples/server/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.1.7/dimples/server/processor.py
--rw-r--r--   0 moky       (501) staff       (20)     6443 2023-06-09 13:36:28.000000 dimples-0.1.7/dimples/server/push_info.py
--rw-r--r--   0 moky       (501) staff       (20)     6719 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/server/push_service.py
--rw-r--r--   0 moky       (501) staff       (20)     5877 2023-06-07 13:18:30.000000 dimples-0.1.7/dimples/server/pusher.py
--rw-r--r--   0 moky       (501) staff       (20)     7986 2023-01-14 12:19:38.000000 dimples-0.1.7/dimples/server/session.py
--rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/server/session_center.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/station/
--rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.1.7/dimples/station/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.1.7/dimples/station/handler.py
--rw-r--r--   0 moky       (501) staff       (20)     7087 2023-06-07 11:52:56.000000 dimples-0.1.7/dimples/station/shared.py
--rwxr-xr-x   0 moky       (501) staff       (20)     3782 2023-06-04 10:23:09.000000 dimples-0.1.7/dimples/station/start.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:51.000000 dimples-0.1.7/dimples/utils/
--rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.1.7/dimples/utils/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 12:24:04.000000 dimples-0.1.7/dimples/utils/cache.py
--rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.1.7/dimples/utils/checker.py
--rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/utils/dos.py
--rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.1.7/dimples/utils/log.py
--rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.1.7/dimples/utils/singleton.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     3274 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/entry_points.txt
--rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-09 17:20:50.000000 dimples-0.1.7/dimples.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-09 17:20:51.000000 dimples-0.1.7/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-09 16:14:04.000000 dimples-0.1.7/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-12 15:42:23.000000 dimples-0.1.8/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      568 2022-12-11 05:07:49.000000 dimples-0.1.8/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/
+-rw-r--r--   0 moky       (501) staff       (20)     7204 2023-06-10 12:29:39.000000 dimples-0.1.8/dimples/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/client/
+-rw-r--r--   0 moky       (501) staff       (20)     1997 2023-06-03 11:38:39.000000 dimples-0.1.8/dimples/client/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/client/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     2191 2023-06-09 16:37:34.000000 dimples-0.1.8/dimples/client/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4011 2023-06-02 18:30:20.000000 dimples-0.1.8/dimples/client/cpu/grp_expel.py
+-rw-r--r--   0 moky       (501) staff       (20)     4116 2023-06-02 18:31:07.000000 dimples-0.1.8/dimples/client/cpu/grp_invite.py
+-rw-r--r--   0 moky       (501) staff       (20)     3554 2023-02-23 11:18:06.000000 dimples-0.1.8/dimples/client/cpu/grp_query.py
+-rw-r--r--   0 moky       (501) staff       (20)     3558 2023-06-02 18:31:36.000000 dimples-0.1.8/dimples/client/cpu/grp_quit.py
+-rw-r--r--   0 moky       (501) staff       (20)     6498 2023-06-02 18:32:15.000000 dimples-0.1.8/dimples/client/cpu/grp_reset.py
+-rw-r--r--   0 moky       (501) staff       (20)     5150 2023-02-23 14:17:47.000000 dimples-0.1.8/dimples/client/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     2948 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/client/cpu/history.py
+-rw-r--r--   0 moky       (501) staff       (20)     1869 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/client/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/client/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     1895 2023-06-09 16:41:36.000000 dimples-0.1.8/dimples/client/cpu/text.py
+-rw-r--r--   0 moky       (501) staff       (20)    16324 2023-06-02 17:03:56.000000 dimples-0.1.8/dimples/client/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     9951 2023-06-12 14:16:50.000000 dimples-0.1.8/dimples/client/messenger.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/client/network/
+-rw-r--r--   0 moky       (501) staff       (20)     3246 2023-02-23 14:19:20.000000 dimples-0.1.8/dimples/client/network/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6258 2023-02-23 14:14:03.000000 dimples-0.1.8/dimples/client/network/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     8302 2023-06-03 11:39:42.000000 dimples-0.1.8/dimples/client/network/state.py
+-rw-r--r--   0 moky       (501) staff       (20)     9531 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/client/network/transition.py
+-rw-r--r--   0 moky       (501) staff       (20)     6619 2023-06-12 13:22:46.000000 dimples-0.1.8/dimples/client/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     7190 2023-06-09 16:42:29.000000 dimples-0.1.8/dimples/client/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     5521 2023-02-23 14:13:41.000000 dimples-0.1.8/dimples/client/terminal.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/common/
+-rw-r--r--   0 moky       (501) staff       (20)     2209 2023-06-06 13:30:28.000000 dimples-0.1.8/dimples/common/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4322 2023-06-02 08:44:29.000000 dimples-0.1.8/dimples/common/ans.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/common/dbi/
+-rw-r--r--   0 moky       (501) staff       (20)     2324 2023-06-09 14:20:27.000000 dimples-0.1.8/dimples/common/dbi/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6396 2023-06-02 10:33:41.000000 dimples-0.1.8/dimples/common/dbi/account.py
+-rw-r--r--   0 moky       (501) staff       (20)     2465 2023-06-02 07:39:55.000000 dimples-0.1.8/dimples/common/dbi/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     7877 2023-06-09 15:01:59.000000 dimples-0.1.8/dimples/common/dbi/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6739 2023-06-02 09:05:19.000000 dimples-0.1.8/dimples/common/facebook.py
+-rw-r--r--   0 moky       (501) staff       (20)     7827 2023-06-12 14:51:01.000000 dimples-0.1.8/dimples/common/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     7710 2023-06-12 13:20:42.000000 dimples-0.1.8/dimples/common/packer.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/common/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2536 2023-02-23 09:20:27.000000 dimples-0.1.8/dimples/common/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3321 2023-06-09 16:01:10.000000 dimples-0.1.8/dimples/common/protocol/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     5004 2022-12-23 07:24:37.000000 dimples-0.1.8/dimples/common/protocol/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     4523 2023-06-02 08:11:42.000000 dimples-0.1.8/dimples/common/protocol/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     6085 2023-06-02 08:40:15.000000 dimples-0.1.8/dimples/common/protocol/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     2521 2023-06-02 08:42:45.000000 dimples-0.1.8/dimples/common/protocol/report.py
+-rw-r--r--   0 moky       (501) staff       (20)     4486 2023-06-04 16:41:38.000000 dimples-0.1.8/dimples/common/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6211 2023-06-03 12:24:47.000000 dimples-0.1.8/dimples/config.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/conn/
+-rw-r--r--   0 moky       (501) staff       (20)     4449 2023-01-14 13:47:09.000000 dimples-0.1.8/dimples/conn/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    10335 2023-06-07 13:23:28.000000 dimples-0.1.8/dimples/conn/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     9892 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/conn/gatekeeper.py
+-rw-r--r--   0 moky       (501) staff       (20)    10305 2023-01-14 13:25:42.000000 dimples-0.1.8/dimples/conn/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     7851 2023-02-23 09:10:59.000000 dimples-0.1.8/dimples/conn/mtp.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/conn/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     1842 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/conn/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8711 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/conn/protocol/mars.py
+-rw-r--r--   0 moky       (501) staff       (20)     8254 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/conn/protocol/ws.py
+-rw-r--r--   0 moky       (501) staff       (20)     5411 2023-02-23 09:10:59.000000 dimples-0.1.8/dimples/conn/queue.py
+-rw-r--r--   0 moky       (501) staff       (20)     7738 2022-12-14 05:44:44.000000 dimples-0.1.8/dimples/conn/seeker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5726 2023-06-02 09:57:33.000000 dimples-0.1.8/dimples/conn/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6991 2023-01-14 12:47:37.000000 dimples-0.1.8/dimples/conn/ws.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/database/
+-rw-r--r--   0 moky       (501) staff       (20)     2560 2023-06-04 16:46:57.000000 dimples-0.1.8/dimples/database/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7000 2023-06-02 12:26:57.000000 dimples-0.1.8/dimples/database/account.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/database/dos/
+-rw-r--r--   0 moky       (501) staff       (20)     1808 2023-06-05 05:13:02.000000 dimples-0.1.8/dimples/database/dos/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4071 2022-12-22 17:59:17.000000 dimples-0.1.8/dimples/database/dos/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     3769 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/database/dos/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     4232 2023-06-02 10:30:44.000000 dimples-0.1.8/dimples/database/dos/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3141 2023-06-02 11:02:33.000000 dimples-0.1.8/dimples/database/dos/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     2680 2022-12-22 17:58:13.000000 dimples-0.1.8/dimples/database/dos/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5630 2023-06-02 11:04:20.000000 dimples-0.1.8/dimples/database/dos/private.py
+-rw-r--r--   0 moky       (501) staff       (20)     8033 2023-06-09 14:40:24.000000 dimples-0.1.8/dimples/database/dos/station.py
+-rw-r--r--   0 moky       (501) staff       (20)     5625 2023-06-02 11:01:02.000000 dimples-0.1.8/dimples/database/dos/user.py
+-rw-r--r--   0 moky       (501) staff       (20)     3097 2022-12-13 10:56:52.000000 dimples-0.1.8/dimples/database/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     4229 2023-06-04 17:05:32.000000 dimples-0.1.8/dimples/database/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     2972 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/database/t_cipherkey.py
+-rw-r--r--   0 moky       (501) staff       (20)     3710 2023-06-09 14:19:20.000000 dimples-0.1.8/dimples/database/t_document.py
+-rw-r--r--   0 moky       (501) staff       (20)     7715 2023-06-05 05:41:56.000000 dimples-0.1.8/dimples/database/t_group.py
+-rw-r--r--   0 moky       (501) staff       (20)     3718 2023-06-09 14:19:56.000000 dimples-0.1.8/dimples/database/t_login.py
+-rw-r--r--   0 moky       (501) staff       (20)     5144 2022-12-22 18:03:37.000000 dimples-0.1.8/dimples/database/t_message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3513 2023-06-05 05:36:10.000000 dimples-0.1.8/dimples/database/t_meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     5589 2023-06-05 05:38:08.000000 dimples-0.1.8/dimples/database/t_private.py
+-rw-r--r--   0 moky       (501) staff       (20)     6647 2023-06-05 05:31:39.000000 dimples-0.1.8/dimples/database/t_station.py
+-rw-r--r--   0 moky       (501) staff       (20)     6455 2023-06-05 05:39:18.000000 dimples-0.1.8/dimples/database/t_user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/edge/
+-rw-r--r--   0 moky       (501) staff       (20)     2127 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/edge/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    13567 2023-06-12 14:07:59.000000 dimples-0.1.8/dimples/edge/octopus.py
+-rw-r--r--   0 moky       (501) staff       (20)     5594 2023-06-05 05:51:39.000000 dimples-0.1.8/dimples/edge/shared.py
+-rw-r--r--   0 moky       (501) staff       (20)     2726 2023-06-04 10:23:09.000000 dimples-0.1.8/dimples/edge/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/register/
+-rw-r--r--   0 moky       (501) staff       (20)     1441 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/register/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9516 2023-06-02 10:01:29.000000 dimples-0.1.8/dimples/register/generate.py
+-rw-r--r--   0 moky       (501) staff       (20)     7045 2023-06-02 10:02:10.000000 dimples-0.1.8/dimples/register/modify.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3880 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/register/run.py
+-rw-r--r--   0 moky       (501) staff       (20)     1971 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/register/shared.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/server/
+-rw-r--r--   0 moky       (501) staff       (20)     2561 2023-06-07 12:19:50.000000 dimples-0.1.8/dimples/server/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/server/cpu/
+-rw-r--r--   0 moky       (501) staff       (20)     1855 2023-02-23 09:37:38.000000 dimples-0.1.8/dimples/server/cpu/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2640 2023-02-23 10:54:44.000000 dimples-0.1.8/dimples/server/cpu/ans.py
+-rw-r--r--   0 moky       (501) staff       (20)     4781 2023-06-03 12:02:30.000000 dimples-0.1.8/dimples/server/cpu/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     3464 2023-06-12 12:55:43.000000 dimples-0.1.8/dimples/server/cpu/handshake.py
+-rw-r--r--   0 moky       (501) staff       (20)     3853 2023-06-03 12:02:46.000000 dimples-0.1.8/dimples/server/cpu/login.py
+-rw-r--r--   0 moky       (501) staff       (20)     1847 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/server/cpu/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     3089 2023-01-31 05:28:07.000000 dimples-0.1.8/dimples/server/cpu/report.py
+-rw-r--r--   0 moky       (501) staff       (20)    13580 2023-06-12 12:40:57.000000 dimples-0.1.8/dimples/server/dispatcher.py
+-rw-r--r--   0 moky       (501) staff       (20)    14053 2023-06-12 15:03:48.000000 dimples-0.1.8/dimples/server/messenger.py
+-rw-r--r--   0 moky       (501) staff       (20)     6659 2023-06-09 08:36:13.000000 dimples-0.1.8/dimples/server/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     5791 2023-02-23 11:39:56.000000 dimples-0.1.8/dimples/server/processor.py
+-rw-r--r--   0 moky       (501) staff       (20)     6443 2023-06-09 13:36:28.000000 dimples-0.1.8/dimples/server/push_info.py
+-rw-r--r--   0 moky       (501) staff       (20)     6719 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/server/push_service.py
+-rw-r--r--   0 moky       (501) staff       (20)     5877 2023-06-07 13:18:30.000000 dimples-0.1.8/dimples/server/pusher.py
+-rw-r--r--   0 moky       (501) staff       (20)     7986 2023-01-14 12:19:38.000000 dimples-0.1.8/dimples/server/session.py
+-rw-r--r--   0 moky       (501) staff       (20)     6997 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/server/session_center.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/station/
+-rw-r--r--   0 moky       (501) staff       (20)     1549 2023-02-23 13:34:51.000000 dimples-0.1.8/dimples/station/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4624 2023-06-07 12:21:10.000000 dimples-0.1.8/dimples/station/handler.py
+-rw-r--r--   0 moky       (501) staff       (20)     7087 2023-06-07 11:52:56.000000 dimples-0.1.8/dimples/station/shared.py
+-rwxr-xr-x   0 moky       (501) staff       (20)     3782 2023-06-04 10:23:09.000000 dimples-0.1.8/dimples/station/start.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples/utils/
+-rw-r--r--   0 moky       (501) staff       (20)     2568 2023-02-23 13:38:40.000000 dimples-0.1.8/dimples/utils/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6447 2022-12-22 12:24:04.000000 dimples-0.1.8/dimples/utils/cache.py
+-rw-r--r--   0 moky       (501) staff       (20)     4016 2023-06-02 18:00:31.000000 dimples-0.1.8/dimples/utils/checker.py
+-rw-r--r--   0 moky       (501) staff       (20)     5978 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/utils/dos.py
+-rw-r--r--   0 moky       (501) staff       (20)     2805 2022-12-28 05:23:15.000000 dimples-0.1.8/dimples/utils/log.py
+-rw-r--r--   0 moky       (501) staff       (20)     1735 2022-12-11 05:07:49.000000 dimples-0.1.8/dimples/utils/singleton.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1061 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     3274 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)      118 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/entry_points.txt
+-rw-r--r--   0 moky       (501) staff       (20)      108 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        8 2023-06-12 15:42:23.000000 dimples-0.1.8/dimples.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2023-06-12 15:42:23.000000 dimples-0.1.8/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1675 2023-06-12 09:37:23.000000 dimples-0.1.8/setup.py
```

### Comparing `dimples-0.1.7/PKG-INFO` & `dimples-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.7
+Version: 0.1.8
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.7/README.md` & `dimples-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/__init__.py` & `dimples-0.1.8/dimples/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,28 +214,32 @@
     #
     #   Common Protocol
     #
     'HandshakeCommand', 'HandshakeState',
     'ReceiptCommand',
     'LoginCommand',
     'ReportCommand',
+    'AnsCommand',
 
     #
     #   Database Interfaces
     #
-    'PrivateKeyDBI', 'MetaDBI', 'DocumentDBI', 'UserDBI', 'GroupDBI',
+    'PrivateKeyDBI', 'MetaDBI', 'DocumentDBI', 'UserDBI', 'ContactDBI', 'GroupDBI',
     'AccountDBI',
     'ReliableMessageDBI', 'CipherKeyDBI',
     'MessageDBI',
-    'LoginDBI', 'ProviderDBI',
+    'LoginDBI', 'ProviderDBI', 'StationDBI',
     'SessionDBI',
+    'ProviderInfo', 'StationInfo',
 
     #
     #   Common Extends
     #
+    'AddressNameServer',
     'CommonFacebook',
     'CommonMessenger',
+    'CommonMessagePacker',
     'Transmitter',
     'Session',
 
     'Config',
 ]
```

### Comparing `dimples-0.1.7/dimples/client/__init__.py` & `dimples-0.1.8/dimples/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/__init__.py` & `dimples-0.1.8/dimples/client/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/grp_expel.py` & `dimples-0.1.8/dimples/client/cpu/grp_expel.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/grp_invite.py` & `dimples-0.1.8/dimples/client/cpu/grp_invite.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/grp_query.py` & `dimples-0.1.8/dimples/client/cpu/grp_query.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/grp_quit.py` & `dimples-0.1.8/dimples/client/cpu/grp_quit.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/grp_reset.py` & `dimples-0.1.8/dimples/client/cpu/grp_reset.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/handshake.py` & `dimples-0.1.8/dimples/client/cpu/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/history.py` & `dimples-0.1.8/dimples/client/cpu/history.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/login.py` & `dimples-0.1.8/dimples/client/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/receipt.py` & `dimples-0.1.8/dimples/client/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/cpu/text.py` & `dimples-0.1.8/dimples/client/cpu/text.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/group.py` & `dimples-0.1.8/dimples/client/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/messenger.py` & `dimples-0.1.8/dimples/client/messenger.py`

 * *Files 27% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 """
     Messenger for client
     ~~~~~~~~~~~~~~~~~~~~
 
     Transform and send message
 """
 
-from typing import Optional
+from typing import Optional, List, Dict
 
 from dimples import EntityType, ID, EVERYONE
 from dimples import Station
-from dimples import Envelope, InstantMessage
-from dimples import MetaCommand, DocumentCommand
+from dimples import Envelope, InstantMessage, ReliableMessage
+from dimples import ContentType, MetaCommand, DocumentCommand, ReceiptCommand
 
 from ..utils import QueryFrequencyChecker
 from ..common import HandshakeCommand, ReportCommand, LoginCommand
 from ..common import CommonMessenger
 
 from .network import ClientSession
 
@@ -74,19 +74,29 @@
             i_msg['visa'] = user.visa.dictionary
             self.send_instant_message(msg=i_msg, priority=-1)
         else:
             # handshake again
             cmd = HandshakeCommand.restart(session=session_key)
             self.send_content(sender=None, receiver=srv_id, content=cmd, priority=-1)
 
+    # Override
     def handshake_success(self):
-        """ callback for handshake success """
         # broadcast current documents after handshake success
         self.broadcast_document()
 
+    # Override
+    def suspend_reliable_message(self, msg: ReliableMessage, error: Dict):
+        self.warning(msg='suspend message: %s -> %s, %s' % (msg.sender, msg.receiver, error))
+        msg['error'] = error
+
+    # Override
+    def suspend_instant_message(self, msg: InstantMessage, error: Dict):
+        self.warning(msg='suspend message: %s -> %s, %s' % (msg.sender, msg.receiver, error))
+        msg['error'] = error
+
     def broadcast_login(self, sender: ID, user_agent: str):
         """ send login command to keep roaming """
         # get current station
         station = self.session.station
         assert sender.type != EntityType.STATION, 'station (%s) cannot login: %s' % (sender, station)
         # create login command
         command = LoginCommand(identifier=sender)
@@ -169,7 +179,44 @@
             self.error(msg='group assistants not found: %s' % identifier)
             return False
         # querying members from bot
         command = DocumentCommand.query(identifier=identifier)
         for bot in assistants:
             self.send_content(sender=None, receiver=bot, content=command, priority=1)
         return True
+
+    # Override
+    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+        # call super
+        responses = super().process_reliable_message(msg=msg)
+        if len(responses) == 0 and self._needs_receipt(msg=msg):
+            current_user = self.facebook.current_user
+            res = ReceiptCommand.create(text='Message received', msg=msg)
+            env = Envelope.create(sender=current_user.identifier, receiver=msg.sender)
+            i_msg = InstantMessage.create(head=env, body=res)
+            s_msg = self.encrypt_message(msg=i_msg)
+            assert s_msg is not None, 'failed to encrypt message: %s -> %s' % (current_user, msg.sender)
+            r_msg = self.sign_message(msg=s_msg)
+            assert r_msg is not None, 'failed to sign message: %s -> %s' % (current_user, msg.sender)
+            responses = [r_msg]
+        return responses
+
+    # noinspection PyMethodMayBeStatic
+    def _needs_receipt(self, msg: ReliableMessage) -> bool:
+        if msg.type == ContentType.COMMAND:
+            # filter for looping message (receipt for receipt)
+            return False
+        sender = msg.sender
+        # receiver = msg.receiver
+        # if sender.type == EntityType.STATION or sender.type == EntityType.BOT:
+        #     if receiver.type == EntityType.STATION or receiver.type == EntityType.BOT:
+        #         # message between bots
+        #         return False
+        if sender.type != EntityType.USER:  # and receiver.type != EntityType.USER:
+            # message between bots
+            return False
+        # current_user = self.facebook.current_user
+        # if receiver != current_user.identifier:
+        #     # forward message
+        #     return True
+        # TODO: other condition?
+        return True
```

### Comparing `dimples-0.1.7/dimples/client/network/__init__.py` & `dimples-0.1.8/dimples/client/network/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/network/session.py` & `dimples-0.1.8/dimples/client/network/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/network/state.py` & `dimples-0.1.8/dimples/client/network/state.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/network/transition.py` & `dimples-0.1.8/dimples/client/network/transition.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/packer.py` & `dimples-0.1.8/dimples/client/packer.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,23 +44,24 @@
     # Override
     def _check_instant_message_receiver(self, msg: InstantMessage) -> bool:
         receiver = msg.receiver
         if receiver.is_broadcast:
             # broadcast message
             return True
         elif receiver.is_group:
+            messenger = get_messenger(packer=self)
             # check group's meta & members
             members = self._members(group=receiver)
             if members is None:
                 # group not ready, suspend message for waiting meta/members
                 error = {
                     'message': 'group not ready',
                     'group': str(receiver),
                 }
-                self._suspend_instant_message(msg=msg, error=error)
+                messenger.suspend_instant_message(msg=msg, error=error)
                 return False
             waiting = []
             for item in members:
                 if self._visa_key(user=item) is not None:
                     # member is OK
                     continue
                 # meta not ready
@@ -68,15 +69,15 @@
             if len(waiting) > 0:
                 # member(s) not ready, suspend message for waiting document
                 error = {
                     'message': 'encrypt keys not found',
                     'group': str(receiver),
                     'members': ID.revert(array=waiting),
                 }
-                self._suspend_instant_message(msg=msg, error=error)
+                messenger.suspend_instant_message(msg=msg, error=error)
                 return False
             # receiver is OK
             return True
         # check user's meta & document
         return super()._check_instant_message_receiver(msg=msg)
 
     # Override
```

### Comparing `dimples-0.1.7/dimples/client/processor.py` & `dimples-0.1.8/dimples/client/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/client/terminal.py` & `dimples-0.1.8/dimples/client/terminal.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/__init__.py` & `dimples-0.1.8/dimples/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/ans.py` & `dimples-0.1.8/dimples/common/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/dbi/__init__.py` & `dimples-0.1.8/dimples/common/dbi/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/dbi/account.py` & `dimples-0.1.8/dimples/common/dbi/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/dbi/message.py` & `dimples-0.1.8/dimples/common/dbi/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/dbi/session.py` & `dimples-0.1.8/dimples/common/dbi/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/facebook.py` & `dimples-0.1.8/dimples/common/facebook.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/messenger.py` & `dimples-0.1.8/dimples/common/messenger.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,25 +26,25 @@
 """
     Common extensions for Messenger
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Transform and send message
 """
 
+import threading
 from abc import ABC, abstractmethod
-from typing import Optional, Tuple, List
+from typing import Optional, Tuple, List, Dict
 
-from dimsdk import EntityType, ID
-from dimsdk import ContentType, Content, Envelope
+from dimsdk import ID
+from dimsdk import Content, Envelope
 from dimsdk import InstantMessage, ReliableMessage
 from dimsdk import EntityDelegate, CipherKeyDelegate
 from dimsdk import Messenger, Packer, Processor
 
 from ..utils import Logging
-from ..common import ReceiptCommand
 
 from .dbi import MessageDBI
 
 from .facebook import CommonFacebook
 from .session import Transmitter, Session
 
 
@@ -53,14 +53,18 @@
     def __init__(self, session: Session, facebook: CommonFacebook, database: MessageDBI):
         super().__init__()
         self.__session = session
         self.__facebook = facebook
         self.__database = database
         self.__packer: Optional[Packer] = None
         self.__processor: Optional[Processor] = None
+        # suspended messages
+        self.__suspend_lock = threading.Lock()
+        self.__incoming_messages: List[ReliableMessage] = []
+        self.__outgoing_messages: List[InstantMessage] = []
 
     @property  # Override
     def packer(self) -> Packer:
         return self.__packer
 
     @packer.setter
     def packer(self, delegate: Packer):
@@ -90,14 +94,19 @@
     def facebook(self) -> CommonFacebook:
         return self.__facebook
 
     @property
     def session(self) -> Session:
         return self.__session
 
+    @abstractmethod
+    def handshake_success(self):
+        """ callback for handshake success """
+        raise NotImplemented
+
     @abstractmethod  # protected
     def query_meta(self, identifier: ID) -> bool:
         """ request for meta with entity ID """
         raise NotImplemented
 
     @abstractmethod  # protected
     def query_document(self, identifier: ID) -> bool:
@@ -105,14 +114,48 @@
         raise NotImplemented
 
     @abstractmethod  # protected
     def query_members(self, identifier: ID) -> bool:
         """ request for group members with group ID """
         raise NotImplemented
 
+    #
+    #   Suspend messages
+    #
+
+    def suspend_reliable_message(self, msg: ReliableMessage, error: Dict):
+        """ Add income message in a queue for waiting sender's visa """
+        self.warning(msg='suspend message: %s -> %s, %s' % (msg.sender, msg.receiver, error))
+        msg['error'] = error
+        with self.__suspend_lock:
+            if len(self.__incoming_messages) > 32:
+                self.__incoming_messages.pop(0)
+            self.__incoming_messages.append(msg)
+
+    def _resume_reliable_messages(self) -> List[ReliableMessage]:
+        with self.__suspend_lock:
+            messages = self.__incoming_messages
+            self.__incoming_messages = []
+            return messages
+
+    def suspend_instant_message(self, msg: InstantMessage, error: Dict):
+        """ Add outgo message in a queue for waiting receiver's visa """
+        self.warning(msg='suspend message: %s -> %s, %s' % (msg.sender, msg.receiver, error))
+        msg['error'] = error
+        with self.__suspend_lock:
+            if len(self.__outgoing_messages) > 32:
+                self.__outgoing_messages.pop(0)
+            self.__outgoing_messages.append(msg)
+
+    def _resume_instant_messages(self) -> List[InstantMessage]:
+        with self.__suspend_lock:
+            messages = self.__outgoing_messages
+            self.__outgoing_messages = []
+            return messages
+
     # # Override
     # def serialize_key(self, key: Union[dict, SymmetricKey], msg: InstantMessage) -> Optional[bytes]:
     #     # try to reuse message key
     #     reused = key.get('reused')
     #     if reused is not None:
     #         if msg.receiver.is_group:
     #             # reuse key for grouped message
@@ -121,51 +164,14 @@
     #         key.pop('reused', None)
     #     data = super().serialize_key(key=key, msg=msg)
     #     if reused is not None:
     #         # put it back
     #         key['reused'] = reused
     #     return data
 
-    # Override
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
-        # call super
-        responses = super().process_reliable_message(msg=msg)
-        if len(responses) == 0 and self._needs_receipt(msg=msg):
-            current_user = self.facebook.current_user
-            res = ReceiptCommand.create(text='Message received', msg=msg)
-            env = Envelope.create(sender=current_user.identifier, receiver=msg.sender)
-            i_msg = InstantMessage.create(head=env, body=res)
-            s_msg = self.encrypt_message(msg=i_msg)
-            assert s_msg is not None, 'failed to encrypt message: %s -> %s' % (current_user, msg.sender)
-            r_msg = self.sign_message(msg=s_msg)
-            assert r_msg is not None, 'failed to sign message: %s -> %s' % (current_user, msg.sender)
-            responses = [r_msg]
-        return responses
-
-    # noinspection PyMethodMayBeStatic
-    def _needs_receipt(self, msg: ReliableMessage) -> bool:
-        if msg.type == ContentType.COMMAND:
-            # filter for looping message (receipt for receipt)
-            return False
-        sender = msg.sender
-        # receiver = msg.receiver
-        # if sender.type == EntityType.STATION or sender.type == EntityType.BOT:
-        #     if receiver.type == EntityType.STATION or receiver.type == EntityType.BOT:
-        #         # message between bots
-        #         return False
-        if sender.type != EntityType.USER:  # and receiver.type != EntityType.USER:
-            # message between bots
-            return False
-        # current_user = self.facebook.current_user
-        # if receiver != current_user.identifier:
-        #     # forward message
-        #     return True
-        # TODO: other condition?
-        return True
-
     #
     #   Interfaces for Transmitting Message
     #
 
     # Override
     def send_content(self, sender: Optional[ID], receiver: ID, content: Content,
                      priority: int = 0) -> Tuple[InstantMessage, Optional[ReliableMessage]]:
```

### Comparing `dimples-0.1.7/dimples/common/packer.py` & `dimples-0.1.8/dimples/common/packer.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,37 +20,27 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from abc import ABC
-from typing import Optional, Dict, List
+from typing import Optional, List
 
 from dimsdk import EncryptKey
 from dimsdk import ID
 from dimsdk import InstantMessage, SecureMessage, ReliableMessage
 from dimsdk import MessagePacker
 
 from ..utils import Logging
 
 
 class CommonMessagePacker(MessagePacker, Logging, ABC):
 
     # protected
-    def _suspend_reliable_message(self, msg: ReliableMessage, error: Dict):
-        """ Add income message in a queue for waiting sender's visa """
-        pass
-
-    # protected
-    def _suspend_instant_message(self, msg: InstantMessage, error: Dict):
-        """ Add outgo message in a queue for waiting receiver's visa """
-        pass
-
-    # protected
     def _visa_key(self, user: ID) -> Optional[EncryptKey]:
         """ for checking whether user's ready """
         facebook = get_facebook(packer=self)
         key = facebook.public_key_for_encryption(identifier=user)
         if key is not None:
             # user is ready
             return key
@@ -96,15 +86,16 @@
             # sender is OK
             return True
         # sender not ready, suspend message for waiting document
         error = {
             'message': 'verify key not found',
             'user': str(sender),
         }
-        self._suspend_reliable_message(msg=msg, error=error)  # msg['error'] = error
+        messenger = get_messenger(packer=self)
+        messenger.suspend_reliable_message(msg=msg, error=error)  # msg['error'] = error
         return False
 
     # protected
     def _check_reliable_message_receiver(self, msg: ReliableMessage) -> bool:
         receiver = msg.receiver
         if receiver.is_broadcast:
             # broadcast message
@@ -118,15 +109,16 @@
         if members is not None:
             return True
         # group not ready, suspend message for waiting members
         error = {
             'message': 'group not ready',
             'group': str(receiver),
         }
-        self._suspend_reliable_message(msg=msg, error=error)  # msg['error'] = error
+        messenger = get_messenger(packer=self)
+        messenger.suspend_reliable_message(msg=msg, error=error)  # msg['error'] = error
         return False
 
     # protected
     def _check_instant_message_receiver(self, msg: InstantMessage) -> bool:
         """ Check receiver before encrypting message """
         receiver = msg.receiver
         if receiver.is_broadcast:
@@ -143,15 +135,16 @@
             # receiver is OK
             return True
         # receiver not ready, suspend message for waiting document
         error = {
             'message': 'encrypt key not found',
             'user': str(receiver),
         }
-        self._suspend_instant_message(msg=msg, error=error)  # msg['error'] = error
+        messenger = get_messenger(packer=self)
+        messenger.suspend_instant_message(msg=msg, error=error)  # msg['error'] = error
         return False
 
     # Override
     def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
         if not self._check_instant_message_receiver(msg=msg):
             # receiver not ready
             self.warning(msg='receiver not ready: %s' % msg.receiver)
```

### Comparing `dimples-0.1.7/dimples/common/protocol/__init__.py` & `dimples-0.1.8/dimples/common/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/protocol/ans.py` & `dimples-0.1.8/dimples/common/protocol/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/protocol/handshake.py` & `dimples-0.1.8/dimples/common/protocol/handshake.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/protocol/login.py` & `dimples-0.1.8/dimples/common/protocol/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/protocol/receipt.py` & `dimples-0.1.8/dimples/common/protocol/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/protocol/report.py` & `dimples-0.1.8/dimples/common/protocol/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/common/session.py` & `dimples-0.1.8/dimples/common/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/config.py` & `dimples-0.1.8/dimples/config.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/__init__.py` & `dimples-0.1.8/dimples/conn/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/gate.py` & `dimples-0.1.8/dimples/conn/gate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/gatekeeper.py` & `dimples-0.1.8/dimples/conn/gatekeeper.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/mars.py` & `dimples-0.1.8/dimples/conn/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/mtp.py` & `dimples-0.1.8/dimples/conn/mtp.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/protocol/__init__.py` & `dimples-0.1.8/dimples/conn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/protocol/mars.py` & `dimples-0.1.8/dimples/conn/protocol/mars.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/protocol/ws.py` & `dimples-0.1.8/dimples/conn/protocol/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/queue.py` & `dimples-0.1.8/dimples/conn/queue.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/seeker.py` & `dimples-0.1.8/dimples/conn/seeker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/session.py` & `dimples-0.1.8/dimples/conn/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/conn/ws.py` & `dimples-0.1.8/dimples/conn/ws.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/__init__.py` & `dimples-0.1.8/dimples/database/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/account.py` & `dimples-0.1.8/dimples/database/account.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/dos/__init__.py` & `dimples-0.1.8/dimples/database/dos/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/dos/base.py` & `dimples-0.1.8/dimples/database/dos/base.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/dos/document.py` & `dimples-0.1.8/dimples/database/dos/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/dos/group.py` & `dimples-0.1.8/dimples/database/dos/group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/dos/login.py` & `dimples-0.1.8/dimples/database/dos/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/dos/meta.py` & `dimples-0.1.8/dimples/database/dos/meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/dos/private.py` & `dimples-0.1.8/dimples/database/dos/private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/dos/station.py` & `dimples-0.1.8/dimples/database/dos/station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/dos/user.py` & `dimples-0.1.8/dimples/database/dos/user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/message.py` & `dimples-0.1.8/dimples/database/message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/session.py` & `dimples-0.1.8/dimples/database/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/t_cipherkey.py` & `dimples-0.1.8/dimples/database/t_cipherkey.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/t_document.py` & `dimples-0.1.8/dimples/database/t_document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/t_group.py` & `dimples-0.1.8/dimples/database/t_group.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/t_login.py` & `dimples-0.1.8/dimples/database/t_login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/t_message.py` & `dimples-0.1.8/dimples/database/t_message.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/t_meta.py` & `dimples-0.1.8/dimples/database/t_meta.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/t_private.py` & `dimples-0.1.8/dimples/database/t_private.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/t_station.py` & `dimples-0.1.8/dimples/database/t_station.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/database/t_user.py` & `dimples-0.1.8/dimples/database/t_user.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/edge/__init__.py` & `dimples-0.1.8/dimples/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/edge/octopus.py` & `dimples-0.1.8/dimples/edge/octopus.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
         self.info(msg='redirect msg(type=%d, sig=%s): %s -> %s | from %s, traces: %s'
                   % (msg.type, sig, msg.sender, msg.receiver, get_remote_station(messenger=self), msg.get('traces')))
         return self._deliver_message(msg=msg)
 
     @abstractmethod
     def _deliver_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         """ call octopus to redirect message """
-        pass
+        return []
 
 
 def get_remote_station(messenger: ClientMessenger) -> ID:
     session = messenger.session
     station = session.station
     return station.identifier
```

### Comparing `dimples-0.1.7/dimples/edge/shared.py` & `dimples-0.1.8/dimples/edge/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/edge/start.py` & `dimples-0.1.8/dimples/edge/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/register/__init__.py` & `dimples-0.1.8/dimples/register/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/register/generate.py` & `dimples-0.1.8/dimples/register/generate.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/register/modify.py` & `dimples-0.1.8/dimples/register/modify.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/register/run.py` & `dimples-0.1.8/dimples/register/run.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/register/shared.py` & `dimples-0.1.8/dimples/register/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/__init__.py` & `dimples-0.1.8/dimples/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/cpu/__init__.py` & `dimples-0.1.8/dimples/server/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/cpu/ans.py` & `dimples-0.1.8/dimples/server/cpu/ans.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/cpu/document.py` & `dimples-0.1.8/dimples/server/cpu/document.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/cpu/handshake.py` & `dimples-0.1.8/dimples/server/cpu/handshake.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,58 +28,58 @@
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     Handshake Protocol
 """
 
 from typing import List
 
-from dimp import ID
-from dimp import ReliableMessage
-from dimp import Content
-
+from dimsdk import ID, Content, ReliableMessage
 from dimsdk.cpu import BaseCommandProcessor
 
 from ...utils import Log
 from ...common import HandshakeCommand
 from ...common import CommonMessenger, Session
 
 
 class HandshakeCommandProcessor(BaseCommandProcessor):
 
     @property
-    def session(self) -> Session:
-        messenger = self.messenger
-        assert isinstance(messenger, CommonMessenger), 'messenger error: %s' % messenger
-        return messenger.session
+    def messenger(self) -> CommonMessenger:
+        transceiver = super().messenger
+        assert isinstance(transceiver, CommonMessenger), 'messenger error: %s' % transceiver
+        return transceiver
 
     # Override
     def process(self, content: Content, msg: ReliableMessage) -> List[Content]:
         assert isinstance(content, HandshakeCommand), 'handshake command error: %s' % content
         title = content.title
         if title in ['DIM?', 'DIM!']:
             # S -> C
             text = 'Handshake command error: %s' % title
             return self._respond_text(text=text)
         # C -> S: Hello world!
         assert 'Hello world!' == title, 'Handshake command error: %s' % content
         # set/update session in session server with new session key
-        session = self.session
+        messenger = self.messenger
+        session = messenger.session
         if session.key == content.session:
             # session key match
             Log.info(msg='handshake accepted: %s, session: %s' % (msg.sender, session.key))
             # verified success
-            handshake_accepted(identifier=msg.sender, session=session)
+            handshake_accepted(identifier=msg.sender, session=session, messenger=messenger)
             res = HandshakeCommand.success(session=session.key)
         else:
             # session key not match
             # ask client to sign it with the new session key
             res = HandshakeCommand.again(session=session.key)
         return [res]
 
 
-def handshake_accepted(identifier: ID, session: Session):
-    # 1. update session ID
+def handshake_accepted(identifier: ID, session: Session, messenger: CommonMessenger):
     from ..session_center import SessionCenter
     center = SessionCenter()
+    # 1. update session ID
     center.update_session(session=session, identifier=identifier)
     # 2. update session flag
     session.set_active(active=True)
+    # 3. callback
+    messenger.handshake_success()
```

### Comparing `dimples-0.1.7/dimples/server/cpu/login.py` & `dimples-0.1.8/dimples/server/cpu/login.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/cpu/receipt.py` & `dimples-0.1.8/dimples/server/cpu/receipt.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/cpu/report.py` & `dimples-0.1.8/dimples/server/cpu/report.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/dispatcher.py` & `dimples-0.1.8/dimples/server/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,27 @@
                 # push notification for the receiver
                 pusher = self.__pusher
                 if pusher is None:
                     self.warning(msg='pusher not set yet, drop notification for: %s' % receiver)
                 else:
                     pusher.push_notification(msg=msg)
         # OK
-        return [] if responses is None else responses
+        if responses is None:
+            # user not online, and not roaming to other station
+            text = 'Message cached'
+            res = ReceiptCommand.create(text=text, msg=msg)
+            return [res]
+        elif len(responses) == 0:
+            # user roamed to other station, but bridge not found
+            text = 'Message received'
+            res = ReceiptCommand.create(text=text, msg=msg)
+            return [res]
+        else:
+            # message delivered
+            return responses
 
     def __save_reliable_message(self, msg: ReliableMessage, receiver: ID) -> bool:
         if receiver.type == EntityType.STATION or msg.sender.type == EntityType.STATION:
             # no need to save station message
             return False
         db = self.__mdb
         return db.cache_reliable_message(msg=msg, receiver=receiver)
@@ -282,16 +294,17 @@
         :param receiver: actual receiver
         :return: responses
         """
         assert receiver.is_user, 'receiver ID error: %s' % receiver
         assert receiver.type != EntityType.STATION, 'should not push message for station: %s' % receiver
         # 1. try to push message directly
         if session_push(msg=msg, receiver=receiver) > 0:
-            text = 'Message pushed'
+            text = 'Message delivered for recipient'
             cmd = ReceiptCommand.create(text=text, msg=msg)
+            cmd['recipient'] = str(receiver)
             return [cmd]
         # 2. get roaming station
         roaming = get_roaming_station(receiver=receiver, database=self.database)
         if roaming is None:
             # login command not found
             # return None to tell the pusher to push notification for it.
             return None
@@ -339,15 +352,15 @@
     # NOTE: the messenger will serialize this message immediately, so
     #       we don't need to clone this dictionary to avoid 'neighbor'
     #       be changed to another value before pushing to the bridge.
     # clone = msg.copy_dictionary()
     # msg = ReliableMessage.parse(msg=clone)
     msg['neighbor'] = str(neighbor)
     if session_push(msg=msg, receiver=bridge) > 0:
-        text = 'Message pushing to neighbor station via the bridge'
+        text = 'Message redirected to neighbor station via the bridge'
         cmd = ReceiptCommand.create(text=text, msg=msg)
         cmd['neighbor'] = str(neighbor)
         return [cmd]
     else:
         # station bridge not found
         # return an empty array to avoid calling pusher
         return []
```

### Comparing `dimples-0.1.7/dimples/server/messenger.py` & `dimples-0.1.8/dimples/server/messenger.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,14 +48,31 @@
 from .packer import FilterManager
 from .dispatcher import Dispatcher
 from .session_center import SessionCenter
 
 
 class ServerMessenger(CommonMessenger):
 
+    # Override
+    def handshake_success(self):
+        session = self.session
+        identifier = session.identifier
+        remote_address = session.remote_address
+        self.warning(msg='user login: %s, socket: %s' % (identifier, remote_address))
+        # process suspended messages
+        messages = self._resume_reliable_messages()
+        for msg in messages:
+            self.info(msg='processing suspended message: %s -> %s' % (msg.sender, msg.receiver))
+            try:
+                responses = self.process_reliable_message(msg=msg)
+                for res in responses:
+                    self.send_reliable_message(msg=res, priority=1)
+            except Exception as error:
+                self.error(msg='failed to process incoming message: %s' % error)
+
     def __broadcast_reliable_message(self, msg: ReliableMessage, station: ID):
         receiver = msg.receiver
         db = self.session.database
         # get other recipients
         recipients = get_recipients(msg=msg, receiver=receiver, db=db)
         if len(recipients) == 0:
             self.warning('other recipients not found: %s' % receiver)
@@ -131,15 +148,36 @@
         if self.is_blocked(msg=msg):
             self.warning(msg='user is blocked: %s -> %s (group: %s)' % (msg.sender, msg.receiver, msg.group))
             return None
         sender = msg.sender
         receiver = msg.receiver
         current = self.facebook.current_user
         sid = current.identifier
-        # 1. verify message
+        # 1. check receiver
+        if receiver != sid and receiver != Station.ANY:  # and receiver != Station.EVERY:
+            # message not for this station, check session for delivering
+            session = self.session
+            if session.identifier is None or not session.active:
+                # not login?
+                # 1.1. suspend this message for waiting handshake
+                error = {
+                    'message': 'user not login',
+                }
+                self.suspend_reliable_message(msg=msg, error=error)
+                # 1.2. ask client to handshake again (with session key)
+                # this message won't be delivered before handshake accepted
+                cmd = HandshakeCommand.ask(session=session.key)
+                self.send_content(sender=sid, receiver=sender, content=cmd)
+                return None
+            # session is active and user login success
+            # if sender == session.ID,
+            #   we can trust this message an no need to verify it;
+            # else if sender is a neighbor station,
+            #   we can trust it too;
+        # 2. verify message
         s_msg = super().verify_message(msg=msg)
         if receiver == sid:
             # message to this station
             # maybe a meta command, document command, etc ...
             return s_msg
         elif receiver.is_broadcast:
             # if receiver == 'station@anywhere':
@@ -156,30 +194,21 @@
                 # forward to search bot
                 self.__broadcast_reliable_message(msg=msg, station=sid)
                 return None
             return s_msg
         elif receiver.is_group:
             self.error(msg='group message should not send to station: %s -> %s' % (sender, receiver))
             return None
-
-        # 2. check session for delivering
-        session = self.session
-        if session.identifier is None or not session.active:
-            # not login? ask client to handshake again (with session key)
-            # this message won't be delivered before handshake accepted
-            cmd = HandshakeCommand.ask(session=session.key)
-            self.send_content(sender=sid, receiver=sender, content=cmd)
-            # DISCUSS: suspend this message for waiting handshake accepted
-            #          or let the client to send it again?
-            return None
-        # session is active, so this message is not for current station,
+        # 3. this message is not for current station,
         # deliver to the real receiver and respond to sender
         dispatcher = Dispatcher()
-        dispatcher.deliver_message(msg=msg, receiver=receiver)
-        # TODO: send responses to the sender?
+        responses = dispatcher.deliver_message(msg=msg, receiver=receiver)
+        assert len(responses) > 0, 'should not happen'
+        for res in responses:
+            self.send_content(sender=sid, receiver=sender, content=res)
 
     # Override
     def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         # call super
         responses = super().process_reliable_message(msg=msg)
         current = self.facebook.current_user
         sid = current.identifier
```

### Comparing `dimples-0.1.7/dimples/server/packer.py` & `dimples-0.1.8/dimples/server/packer.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/processor.py` & `dimples-0.1.8/dimples/server/processor.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/push_info.py` & `dimples-0.1.8/dimples/server/push_info.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/push_service.py` & `dimples-0.1.8/dimples/server/push_service.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/pusher.py` & `dimples-0.1.8/dimples/server/pusher.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/session.py` & `dimples-0.1.8/dimples/server/session.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/server/session_center.py` & `dimples-0.1.8/dimples/server/session_center.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/station/__init__.py` & `dimples-0.1.8/dimples/station/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/station/handler.py` & `dimples-0.1.8/dimples/station/handler.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/station/shared.py` & `dimples-0.1.8/dimples/station/shared.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/station/start.py` & `dimples-0.1.8/dimples/station/start.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/utils/__init__.py` & `dimples-0.1.8/dimples/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/utils/cache.py` & `dimples-0.1.8/dimples/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/utils/checker.py` & `dimples-0.1.8/dimples/utils/checker.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/utils/dos.py` & `dimples-0.1.8/dimples/utils/dos.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/utils/log.py` & `dimples-0.1.8/dimples/utils/log.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples/utils/singleton.py` & `dimples-0.1.8/dimples/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/dimples.egg-info/PKG-INFO` & `dimples-0.1.8/dimples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimples
-Version: 0.1.7
+Version: 0.1.8
 Summary: DIMP Library for Edges and Stations
 Home-page: https://github.com/dimchat/demo-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # DIMP Library for Edges and Stations (Python version)
```

### Comparing `dimples-0.1.7/dimples.egg-info/SOURCES.txt` & `dimples-0.1.8/dimples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimples-0.1.7/setup.py` & `dimples-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '0.1.7'
+__version__ = '0.1.8'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
```

