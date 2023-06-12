# Comparing `tmp/discord.py-2.2.3.tar.gz` & `tmp/discord.py-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord.py-2.2.3.tar", last modified: Mon May  1 22:22:20 2023, max compression
+gzip compressed data, was "discord.py-2.3.0.tar", last modified: Mon Jun 12 17:42:22 2023, max compression
```

## Comparing `discord.py-2.2.3.tar` & `discord.py-2.3.0.tar`

### file list

```diff
@@ -1,144 +1,143 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.584710 discord.py-2.2.3/
--rw-rw-rw-   0        0        0     1081 2021-02-02 07:58:56.000000 discord.py-2.2.3/LICENSE
--rw-rw-rw-   0        0        0      111 2021-08-22 06:25:27.000000 discord.py-2.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4212 2023-05-01 22:22:20.584710 discord.py-2.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2023-02-11 23:42:40.000000 discord.py-2.2.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.459598 discord.py-2.2.3/discord/
--rw-rw-rw-   0        0        0     1886 2023-05-01 22:14:33.000000 discord.py-2.2.3/discord/__init__.py
--rw-rw-rw-   0        0        0    11051 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/__main__.py
--rw-rw-rw-   0        0        0     1410 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/_types.py
--rw-rw-rw-   0        0        0    65763 2023-02-25 10:27:47.000000 discord.py-2.2.3/discord/abc.py
--rw-rw-rw-   0        0        0    26864 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/activity.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.472610 discord.py-2.2.3/discord/app_commands/
--rw-rw-rw-   0        0        0      424 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/__init__.py
--rw-rw-rw-   0        0        0    18077 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/checks.py
--rw-rw-rw-   0        0        0    95614 2023-02-25 10:27:47.000000 discord.py-2.2.3/discord/app_commands/commands.py
--rw-rw-rw-   0        0        0    19006 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/errors.py
--rw-rw-rw-   0        0        0    38500 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/app_commands/models.py
--rw-rw-rw-   0        0        0    13123 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/namespace.py
--rw-rw-rw-   0        0        0    32499 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/transformers.py
--rw-rw-rw-   0        0        0    10686 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/app_commands/translator.py
--rw-rw-rw-   0        0        0    47965 2023-02-25 10:27:47.000000 discord.py-2.2.3/discord/app_commands/tree.py
--rw-rw-rw-   0        0        0    10921 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/appinfo.py
--rw-rw-rw-   0        0        0    15837 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/asset.py
--rw-rw-rw-   0        0        0    34880 2023-05-01 22:00:03.000000 discord.py-2.2.3/discord/audit_logs.py
--rw-rw-rw-   0        0        0    23488 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/automod.py
--rw-rw-rw-   0        0        0     3751 2022-02-22 03:41:08.000000 discord.py-2.2.3/discord/backoff.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.513646 discord.py-2.2.3/discord/bin/
--rw-rw-rw-   0        0        0   441856 2021-02-02 07:58:56.000000 discord.py-2.2.3/discord/bin/libopus-0.x64.dll
--rw-rw-rw-   0        0        0   366080 2021-02-02 07:58:56.000000 discord.py-2.2.3/discord/bin/libopus-0.x86.dll
--rw-rw-rw-   0        0        0   114410 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/channel.py
--rw-rw-rw-   0        0        0    84965 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/client.py
--rw-rw-rw-   0        0        0    14168 2023-02-28 14:02:42.000000 discord.py-2.2.3/discord/colour.py
--rw-rw-rw-   0        0        0    16836 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/components.py
--rw-rw-rw-   0        0        0     3032 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/context_managers.py
--rw-rw-rw-   0        0        0    22722 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/embeds.py
--rw-rw-rw-   0        0        0     8574 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/emoji.py
--rw-rw-rw-   0        0        0    22131 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/enums.py
--rw-rw-rw-   0        0        0     8952 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.392538 discord.py-2.2.3/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.534666 discord.py-2.2.3/discord/ext/commands/
--rw-rw-rw-   0        0        0      437 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     2638 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/_types.py
--rw-rw-rw-   0        0        0    51719 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/bot.py
--rw-rw-rw-   0        0        0    30163 2023-02-28 07:20:21.000000 discord.py-2.2.3/discord/ext/commands/cog.py
--rw-rw-rw-   0        0        0    34547 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/ext/commands/context.py
--rw-rw-rw-   0        0        0    45392 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/ext/commands/converter.py
--rw-rw-rw-   0        0        0     9716 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    89352 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/ext/commands/core.py
--rw-rw-rw-   0        0        0    36151 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/ext/commands/errors.py
--rw-rw-rw-   0        0        0    22966 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/flags.py
--rw-rw-rw-   0        0        0    57705 2023-02-25 10:27:47.000000 discord.py-2.2.3/discord/ext/commands/help.py
--rw-rw-rw-   0        0        0    36595 2023-03-02 03:47:33.000000 discord.py-2.2.3/discord/ext/commands/hybrid.py
--rw-rw-rw-   0        0        0     8361 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/parameters.py
--rw-rw-rw-   0        0        0     6247 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.535666 discord.py-2.2.3/discord/ext/tasks/
--rw-rw-rw-   0        0        0    29180 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0     5378 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/file.py
--rw-rw-rw-   0        0        0    52208 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/flags.py
--rw-rw-rw-   0        0        0    34937 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/gateway.py
--rw-rw-rw-   0        0        0   140799 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/guild.py
--rw-rw-rw-   0        0        0    89365 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/http.py
--rw-rw-rw-   0        0        0    13334 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/integrations.py
--rw-rw-rw-   0        0        0    44412 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/interactions.py
--rw-rw-rw-   0        0        0    20595 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/invite.py
--rw-rw-rw-   0        0        0    40760 2023-02-25 08:13:35.000000 discord.py-2.2.3/discord/member.py
--rw-rw-rw-   0        0        0     5592 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/mentions.py
--rw-rw-rw-   0        0        0    82150 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/message.py
--rw-rw-rw-   0        0        0     1485 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/mixins.py
--rw-rw-rw-   0        0        0     3702 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/object.py
--rw-rw-rw-   0        0        0     3646 2022-02-20 10:26:28.000000 discord.py-2.2.3/discord/oggparse.py
--rw-rw-rw-   0        0        0    15065 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/opus.py
--rw-rw-rw-   0        0        0     7950 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/partial_emoji.py
--rw-rw-rw-   0        0        0    28320 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/permissions.py
--rw-rw-rw-   0        0        0    26456 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/player.py
--rw-rw-rw-   0        0        0        0 2021-08-22 06:25:27.000000 discord.py-2.2.3/discord/py.typed
--rw-rw-rw-   0        0        0    16826 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/raw_models.py
--rw-rw-rw-   0        0        0     8229 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/reaction.py
--rw-rw-rw-   0        0        0    17906 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/role.py
--rw-rw-rw-   0        0        0    23655 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/scheduled_event.py
--rw-rw-rw-   0        0        0    20129 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/shard.py
--rw-rw-rw-   0        0        0     6498 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/stage_instance.py
--rw-rw-rw-   0        0        0    73314 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/state.py
--rw-rw-rw-   0        0        0    16039 2023-05-01 21:59:43.000000 discord.py-2.2.3/discord/sticker.py
--rw-rw-rw-   0        0        0     4607 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/team.py
--rw-rw-rw-   0        0        0     9574 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/template.py
--rw-rw-rw-   0        0        0    32449 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/threads.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.572699 discord.py-2.2.3/discord/types/
--rw-rw-rw-   0        0        0      149 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/__init__.py
--rw-rw-rw-   0        0        0     2707 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/activity.py
--rw-rw-rw-   0        0        0     2386 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/types/appinfo.py
--rw-rw-rw-   0        0        0     8192 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/audit_log.py
--rw-rw-rw-   0        0        0     4009 2023-02-27 01:22:42.000000 discord.py-2.2.3/discord/types/automod.py
--rw-rw-rw-   0        0        0     4557 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/types/channel.py
--rw-rw-rw-   0        0        0     6266 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/command.py
--rw-rw-rw-   0        0        0     3057 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/components.py
--rw-rw-rw-   0        0        0     2329 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/embed.py
--rw-rw-rw-   0        0        0     1528 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/emoji.py
--rw-rw-rw-   0        0        0     8453 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/gateway.py
--rw-rw-rw-   0        0        0     5197 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/types/guild.py
--rw-rw-rw-   0        0        0     2288 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/integration.py
--rw-rw-rw-   0        0        0     6923 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/interactions.py
--rw-rw-rw-   0        0        0     2704 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/invite.py
--rw-rw-rw-   0        0        0     1898 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/member.py
--rw-rw-rw-   0        0        0     4182 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/types/message.py
--rw-rw-rw-   0        0        0     1746 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/role.py
--rw-rw-rw-   0        0        0     3294 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/scheduled_event.py
--rw-rw-rw-   0        0        0     1182 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/snowflake.py
--rw-rw-rw-   0        0        0     2257 2023-05-01 21:59:43.000000 discord.py-2.2.3/discord/types/sticker.py
--rw-rw-rw-   0        0        0     1499 2022-02-20 10:26:29.000000 discord.py-2.2.3/discord/types/team.py
--rw-rw-rw-   0        0        0     1609 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/template.py
--rw-rw-rw-   0        0        0     2454 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/threads.py
--rw-rw-rw-   0        0        0     1540 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/user.py
--rw-rw-rw-   0        0        0     2268 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/voice.py
--rw-rw-rw-   0        0        0     1978 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/webhook.py
--rw-rw-rw-   0        0        0     1460 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1883 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/types/widget.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.580706 discord.py-2.2.3/discord/ui/
--rw-rw-rw-   0        0        0      285 2022-02-20 10:13:32.000000 discord.py-2.2.3/discord/ui/__init__.py
--rw-rw-rw-   0        0        0    10620 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ui/button.py
--rw-rw-rw-   0        0        0     5899 2023-02-28 07:04:17.000000 discord.py-2.2.3/discord/ui/dynamic.py
--rw-rw-rw-   0        0        0     4372 2023-03-02 00:44:50.000000 discord.py-2.2.3/discord/ui/item.py
--rw-rw-rw-   0        0        0     7012 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ui/modal.py
--rw-rw-rw-   0        0        0    34049 2023-03-02 00:44:50.000000 discord.py-2.2.3/discord/ui/select.py
--rw-rw-rw-   0        0        0     8058 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/ui/text_input.py
--rw-rw-rw-   0        0        0    22878 2023-02-14 04:54:29.000000 discord.py-2.2.3/discord/ui/view.py
--rw-rw-rw-   0        0        0    15390 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/user.py
--rw-rw-rw-   0        0        0    41360 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/utils.py
--rw-rw-rw-   0        0        0    24974 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.583709 discord.py-2.2.3/discord/webhook/
--rw-rw-rw-   0        0        0      182 2021-08-15 18:01:53.000000 discord.py-2.2.3/discord/webhook/__init__.py
--rw-rw-rw-   0        0        0    69567 2023-05-01 22:00:19.000000 discord.py-2.2.3/discord/webhook/async_.py
--rw-rw-rw-   0        0        0    42520 2023-05-01 22:00:19.000000 discord.py-2.2.3/discord/webhook/sync.py
--rw-rw-rw-   0        0        0     7539 2023-02-11 23:42:40.000000 discord.py-2.2.3/discord/welcome_screen.py
--rw-rw-rw-   0        0        0    10162 2023-05-01 21:58:58.000000 discord.py-2.2.3/discord/widget.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:22:20.463602 discord.py-2.2.3/discord.py.egg-info/
--rw-rw-rw-   0        0        0     4212 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3092 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      330 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 22:22:19.000000 discord.py-2.2.3/discord.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      869 2023-02-11 23:42:40.000000 discord.py-2.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       18 2023-02-11 23:42:40.000000 discord.py-2.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 22:22:20.584710 discord.py-2.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2946 2023-02-11 23:42:40.000000 discord.py-2.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.709865 discord.py-2.3.0/
+-rw-rw-rw-   0        0        0     1081 2021-02-02 07:58:56.000000 discord.py-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0      111 2021-08-22 06:25:27.000000 discord.py-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4212 2023-06-12 17:42:22.708865 discord.py-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2945 2023-02-11 23:42:40.000000 discord.py-2.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.573744 discord.py-2.3.0/discord/
+-rw-rw-rw-   0        0        0     1886 2023-06-12 17:40:31.000000 discord.py-2.3.0/discord/__init__.py
+-rw-rw-rw-   0        0        0    11051 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/__main__.py
+-rw-rw-rw-   0        0        0     1410 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/_types.py
+-rw-rw-rw-   0        0        0    65844 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/abc.py
+-rw-rw-rw-   0        0        0    26864 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/activity.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.610777 discord.py-2.3.0/discord/app_commands/
+-rw-rw-rw-   0        0        0      424 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/__init__.py
+-rw-rw-rw-   0        0        0    18077 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/checks.py
+-rw-rw-rw-   0        0        0    94536 2023-05-03 00:13:10.000000 discord.py-2.3.0/discord/app_commands/commands.py
+-rw-rw-rw-   0        0        0    19006 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/errors.py
+-rw-rw-rw-   0        0        0    38502 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/app_commands/models.py
+-rw-rw-rw-   0        0        0    13123 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/namespace.py
+-rw-rw-rw-   0        0        0    32512 2023-06-04 11:51:52.000000 discord.py-2.3.0/discord/app_commands/transformers.py
+-rw-rw-rw-   0        0        0    10686 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/translator.py
+-rw-rw-rw-   0        0        0    47965 2023-02-25 10:27:47.000000 discord.py-2.3.0/discord/app_commands/tree.py
+-rw-rw-rw-   0        0        0    12713 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/appinfo.py
+-rw-rw-rw-   0        0        0    15837 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/asset.py
+-rw-rw-rw-   0        0        0    35367 2023-05-04 02:39:48.000000 discord.py-2.3.0/discord/audit_logs.py
+-rw-rw-rw-   0        0        0    23833 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/automod.py
+-rw-rw-rw-   0        0        0     3751 2022-02-22 03:41:08.000000 discord.py-2.3.0/discord/backoff.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.655817 discord.py-2.3.0/discord/bin/
+-rw-rw-rw-   0        0        0   441856 2021-02-02 07:58:56.000000 discord.py-2.3.0/discord/bin/libopus-0.x64.dll
+-rw-rw-rw-   0        0        0   366080 2021-02-02 07:58:56.000000 discord.py-2.3.0/discord/bin/libopus-0.x86.dll
+-rw-rw-rw-   0        0        0   116803 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/channel.py
+-rw-rw-rw-   0        0        0    85400 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/client.py
+-rw-rw-rw-   0        0        0    14403 2023-06-08 02:11:50.000000 discord.py-2.3.0/discord/colour.py
+-rw-rw-rw-   0        0        0    16836 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/components.py
+-rw-rw-rw-   0        0        0     3032 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/context_managers.py
+-rw-rw-rw-   0        0        0    22722 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/embeds.py
+-rw-rw-rw-   0        0        0     8574 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/emoji.py
+-rw-rw-rw-   0        0        0    22242 2023-06-08 02:11:39.000000 discord.py-2.3.0/discord/enums.py
+-rw-rw-rw-   0        0        0     8952 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.493673 discord.py-2.3.0/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.670831 discord.py-2.3.0/discord/ext/commands/
+-rw-rw-rw-   0        0        0      437 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     2638 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    51719 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    30245 2023-06-04 11:51:24.000000 discord.py-2.3.0/discord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    40048 2023-05-20 01:12:09.000000 discord.py-2.3.0/discord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    45846 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0     9716 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    89619 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    36450 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    22966 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    57732 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/ext/commands/help.py
+-rw-rw-rw-   0        0        0    36595 2023-03-02 03:47:33.000000 discord.py-2.3.0/discord/ext/commands/hybrid.py
+-rw-rw-rw-   0        0        0     9157 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/ext/commands/parameters.py
+-rw-rw-rw-   0        0        0     6247 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.671832 discord.py-2.3.0/discord/ext/tasks/
+-rw-rw-rw-   0        0        0    29180 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5378 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/file.py
+-rw-rw-rw-   0        0        0    54264 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/flags.py
+-rw-rw-rw-   0        0        0    35191 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/gateway.py
+-rw-rw-rw-   0        0        0   150174 2023-06-11 17:58:37.000000 discord.py-2.3.0/discord/guild.py
+-rw-rw-rw-   0        0        0    90056 2023-06-08 01:54:09.000000 discord.py-2.3.0/discord/http.py
+-rw-rw-rw-   0        0        0    13334 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/integrations.py
+-rw-rw-rw-   0        0        0    45093 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/interactions.py
+-rw-rw-rw-   0        0        0    20595 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/invite.py
+-rw-rw-rw-   0        0        0    41018 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/member.py
+-rw-rw-rw-   0        0        0     5592 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/mentions.py
+-rw-rw-rw-   0        0        0    85375 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/message.py
+-rw-rw-rw-   0        0        0     1485 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/mixins.py
+-rw-rw-rw-   0        0        0     3702 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/object.py
+-rw-rw-rw-   0        0        0     3646 2022-02-20 10:26:28.000000 discord.py-2.3.0/discord/oggparse.py
+-rw-rw-rw-   0        0        0    15233 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/opus.py
+-rw-rw-rw-   0        0        0     7950 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0    30153 2023-06-11 17:51:43.000000 discord.py-2.3.0/discord/permissions.py
+-rw-rw-rw-   0        0        0    26498 2023-06-04 11:51:24.000000 discord.py-2.3.0/discord/player.py
+-rw-rw-rw-   0        0        0        0 2021-08-22 06:25:27.000000 discord.py-2.3.0/discord/py.typed
+-rw-rw-rw-   0        0        0    16826 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/raw_models.py
+-rw-rw-rw-   0        0        0     8207 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/reaction.py
+-rw-rw-rw-   0        0        0    17906 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/role.py
+-rw-rw-rw-   0        0        0    23629 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/scheduled_event.py
+-rw-rw-rw-   0        0        0    20129 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/shard.py
+-rw-rw-rw-   0        0        0     6498 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/stage_instance.py
+-rw-rw-rw-   0        0        0    73376 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/state.py
+-rw-rw-rw-   0        0        0    16039 2023-05-01 21:59:43.000000 discord.py-2.3.0/discord/sticker.py
+-rw-rw-rw-   0        0        0     4792 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/team.py
+-rw-rw-rw-   0        0        0     9574 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/template.py
+-rw-rw-rw-   0        0        0    32456 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/threads.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.698855 discord.py-2.3.0/discord/types/
+-rw-rw-rw-   0        0        0      149 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     2707 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/activity.py
+-rw-rw-rw-   0        0        0     2487 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/types/appinfo.py
+-rw-rw-rw-   0        0        0     8192 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4009 2023-02-27 01:22:42.000000 discord.py-2.3.0/discord/types/automod.py
+-rw-rw-rw-   0        0        0     4804 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/types/channel.py
+-rw-rw-rw-   0        0        0     6266 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/command.py
+-rw-rw-rw-   0        0        0     3057 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/components.py
+-rw-rw-rw-   0        0        0     2329 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1528 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     8453 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     5279 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/types/guild.py
+-rw-rw-rw-   0        0        0     2288 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/integration.py
+-rw-rw-rw-   0        0        0     7046 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     2704 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1898 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/member.py
+-rw-rw-rw-   0        0        0     4251 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/types/message.py
+-rw-rw-rw-   0        0        0     1746 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/role.py
+-rw-rw-rw-   0        0        0     3294 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1182 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2257 2023-05-01 21:59:43.000000 discord.py-2.3.0/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     1499 2022-02-20 10:26:29.000000 discord.py-2.3.0/discord/types/team.py
+-rw-rw-rw-   0        0        0     1609 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/template.py
+-rw-rw-rw-   0        0        0     2454 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/threads.py
+-rw-rw-rw-   0        0        0     1572 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/types/user.py
+-rw-rw-rw-   0        0        0     2268 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/voice.py
+-rw-rw-rw-   0        0        0     1978 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1460 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1883 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/widget.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.704861 discord.py-2.3.0/discord/ui/
+-rw-rw-rw-   0        0        0      285 2022-02-20 10:13:32.000000 discord.py-2.3.0/discord/ui/__init__.py
+-rw-rw-rw-   0        0        0    10620 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ui/button.py
+-rw-rw-rw-   0        0        0     4372 2023-03-02 00:44:50.000000 discord.py-2.3.0/discord/ui/item.py
+-rw-rw-rw-   0        0        0     7035 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/ui/modal.py
+-rw-rw-rw-   0        0        0    34030 2023-06-04 11:51:24.000000 discord.py-2.3.0/discord/ui/select.py
+-rw-rw-rw-   0        0        0     8092 2023-06-04 11:53:08.000000 discord.py-2.3.0/discord/ui/text_input.py
+-rw-rw-rw-   0        0        0    22878 2023-02-14 04:54:29.000000 discord.py-2.3.0/discord/ui/view.py
+-rw-rw-rw-   0        0        0    16504 2023-06-08 02:12:29.000000 discord.py-2.3.0/discord/user.py
+-rw-rw-rw-   0        0        0    41506 2023-05-20 01:21:20.000000 discord.py-2.3.0/discord/utils.py
+-rw-rw-rw-   0        0        0    24974 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.707863 discord.py-2.3.0/discord/webhook/
+-rw-rw-rw-   0        0        0      182 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    69729 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0    42586 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7539 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10426 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/widget.py
+drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.599767 discord.py-2.3.0/discord.py.egg-info/
+-rw-rw-rw-   0        0        0     4212 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3070 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      330 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      869 2023-02-11 23:42:40.000000 discord.py-2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       18 2023-02-11 23:42:40.000000 discord.py-2.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 17:42:22.709865 discord.py-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2946 2023-02-11 23:42:40.000000 discord.py-2.3.0/setup.py
```

### Comparing `discord.py-2.2.3/LICENSE` & `discord.py-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/PKG-INFO` & `discord.py-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord.py
-Version: 2.2.3
+Version: 2.3.0
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/Rapptz/discord.py
 Author: Rapptz
 License: MIT
 Project-URL: Documentation, https://discordpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Rapptz/discord.py/issues
 Platform: UNKNOWN
```

### Comparing `discord.py-2.2.3/README.rst` & `discord.py-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/__init__.py` & `discord.py-2.3.0/discord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 """
 
 __title__ = 'discord'
 __author__ = 'Rapptz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2015-present Rapptz'
-__version__ = '2.2.3'
+__version__ = '2.3.0'
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
 import logging
 from typing import NamedTuple, Literal
 
 from .client import *
@@ -74,12 +74,12 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=2, minor=2, micro=3, releaselevel='final', serial=0)
+version_info: VersionInfo = VersionInfo(major=2, minor=3, micro=0, releaselevel='final', serial=0)
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 del logging, NamedTuple, Literal, VersionInfo
```

### Comparing `discord.py-2.2.3/discord/__main__.py` & `discord.py-2.3.0/discord/__main__.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/_types.py` & `discord.py-2.3.0/discord/_types.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/abc.py` & `discord.py-2.3.0/discord/abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,23 +215,26 @@
     This ABC must also implement :class:`~discord.abc.Snowflake`.
 
     Attributes
     -----------
     name: :class:`str`
         The user's username.
     discriminator: :class:`str`
-        The user's discriminator.
+        The user's discriminator. This is a legacy concept that is no longer used.
+    global_name: Optional[:class:`str`]
+        The user's global nickname.
     bot: :class:`bool`
         If the user is a bot account.
     system: :class:`bool`
         If the user is a system account.
     """
 
     name: str
     discriminator: str
+    global_name: Optional[str]
     bot: bool
     system: bool
 
     @property
     def display_name(self) -> str:
         """:class:`str`: Returns the user's display name."""
         raise NotImplementedError
@@ -244,15 +247,15 @@
     @property
     def avatar(self) -> Optional[Asset]:
         """Optional[:class:`~discord.Asset`]: Returns an Asset that represents the user's avatar, if present."""
         raise NotImplementedError
 
     @property
     def default_avatar(self) -> Asset:
-        """:class:`~discord.Asset`: Returns the default avatar for a given user. This is calculated by the user's discriminator."""
+        """:class:`~discord.Asset`: Returns the default avatar for a given user."""
         raise NotImplementedError
 
     @property
     def display_avatar(self) -> Asset:
         """:class:`~discord.Asset`: Returns the user's display avatar.
 
         For regular users this is just their default avatar or uploaded avatar.
@@ -939,16 +942,14 @@
                 overwrite = PermissionOverwrite(**permissions)
             except (ValueError, TypeError):
                 raise TypeError('Invalid permissions given to keyword arguments.')
         else:
             if len(permissions) > 0:
                 raise TypeError('Cannot mix overwrite and keyword arguments.')
 
-        # TODO: wait for event
-
         if overwrite is None:
             await http.delete_channel_permissions(self.id, target.id, reason=reason)
         elif isinstance(overwrite, PermissionOverwrite):
             (allow, deny) = overwrite.pair()
             await http.edit_channel_permissions(
                 self.id, target.id, str(allow.value), str(deny.value), perm_type, reason=reason
             )
@@ -1718,20 +1719,20 @@
         -------
         :class:`~discord.Message`
             The message with the message data parsed.
         """
 
         async def _around_strategy(retrieve: int, around: Optional[Snowflake], limit: Optional[int]):
             if not around:
-                return []
+                return [], None, 0
 
             around_id = around.id if around else None
             data = await self._state.http.logs_from(channel.id, retrieve, around=around_id)
 
-            return data, None, limit
+            return data, None, 0
 
         async def _after_strategy(retrieve: int, after: Optional[Snowflake], limit: Optional[int]):
             after_id = after.id if after else None
             data = await self._state.http.logs_from(channel.id, retrieve, after=after_id)
 
             if data:
                 if limit is not None:
```

### Comparing `discord.py-2.2.3/discord/activity.py` & `discord.py-2.3.0/discord/activity.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/app_commands/checks.py` & `discord.py-2.3.0/discord/app_commands/checks.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/app_commands/commands.py` & `discord.py-2.3.0/discord/app_commands/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     Type,
     TypeVar,
     Union,
     overload,
 )
 
 import re
+from copy import copy as shallow_copy
 
 from ..enums import AppCommandOptionType, AppCommandType, ChannelType, Locale
 from .models import Choice
 from .transformers import annotation_to_parameter, CommandParameter, NoneType
 from .errors import AppCommandError, CheckFailure, CommandInvokeError, CommandSignatureMismatch, CommandAlreadyRegistered
 from .translator import TranslationContextLocation, TranslationContext, Translator, locale_str
 from ..message import Message
@@ -703,33 +704,18 @@
         parent: Optional[Group],
         binding: GroupT,
         bindings: MutableMapping[GroupT, GroupT] = MISSING,
         set_on_binding: bool = True,
     ) -> Command:
         bindings = {} if bindings is MISSING else bindings
 
-        cls = self.__class__
-        copy = cls.__new__(cls)
-        copy.name = self.name
-        copy._locale_name = self._locale_name
-        copy._guild_ids = self._guild_ids
-        copy.checks = self.checks
-        copy.description = self.description
-        copy._locale_description = self._locale_description
-        copy.default_permissions = self.default_permissions
-        copy.guild_only = self.guild_only
-        copy.nsfw = self.nsfw
-        copy._attr = self._attr
-        copy._callback = self._callback
-        copy.on_error = self.on_error
+        copy = shallow_copy(self)
         copy._params = self._params.copy()
-        copy.module = self.module
         copy.parent = parent
         copy.binding = bindings.get(self.binding) if self.binding is not None else binding
-        copy.extras = self.extras
 
         if copy._attr and set_on_binding:
             setattr(copy.binding, copy._attr, copy)
 
         return copy
 
     async def get_translated_payload(self, translator: Translator) -> Dict[str, Any]:
@@ -1618,30 +1604,17 @@
         parent: Optional[Group],
         binding: Binding,
         bindings: MutableMapping[Group, Group] = MISSING,
         set_on_binding: bool = True,
     ) -> Group:
         bindings = {} if bindings is MISSING else bindings
 
-        cls = self.__class__
-        copy = cls.__new__(cls)
-        copy.name = self.name
-        copy._locale_name = self._locale_name
-        copy._guild_ids = self._guild_ids
-        copy.description = self.description
-        copy._locale_description = self._locale_description
+        copy = shallow_copy(self)
         copy.parent = parent
-        copy.module = self.module
-        copy.default_permissions = self.default_permissions
-        copy.guild_only = self.guild_only
-        copy.nsfw = self.nsfw
-        copy._attr = self._attr
-        copy._owner_cls = self._owner_cls
         copy._children = {}
-        copy.extras = self.extras
 
         bindings[self] = copy
 
         for child in self._children.values():
             child_copy = child._copy_with(parent=copy, binding=binding, bindings=bindings)
             child_copy.parent = copy
             copy._children[child_copy.name] = child_copy
```

### Comparing `discord.py-2.2.3/discord/app_commands/errors.py` & `discord.py-2.3.0/discord/app_commands/errors.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/app_commands/models.py` & `discord.py-2.3.0/discord/app_commands/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,15 +669,15 @@
         Whether the thread is locked.
     invitable: :class:`bool`
         Whether non-moderators can add other non-moderators to this thread.
         This is always ``True`` for public threads.
     archiver_id: Optional[:class:`int`]
         The user's ID that archived this thread.
     auto_archive_duration: :class:`int`
-        The duration in minutes until the thread is automatically archived due to inactivity.
+        The duration in minutes until the thread is automatically hidden from the channel list.
         Usually a value of 60, 1440, 4320 and 10080.
     archive_timestamp: :class:`datetime.datetime`
         An aware timestamp of when the thread's archived status was last updated in UTC.
     """
 
     __slots__ = (
         'id',
```

### Comparing `discord.py-2.2.3/discord/app_commands/namespace.py` & `discord.py-2.3.0/discord/app_commands/namespace.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/app_commands/transformers.py` & `discord.py-2.3.0/discord/app_commands/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -746,15 +746,15 @@
 
     This differs from the built in mapping by supporting a few more things.
     Likewise, this returns a "transformed" annotation that is ready to use with CommandParameter.transform.
     """
 
     try:
         return (_mapping[annotation], MISSING, True)
-    except KeyError:
+    except (KeyError, TypeError):
         pass
 
     if isinstance(annotation, Transformer):
         return (annotation, MISSING, False)
 
     if inspect.isclass(annotation):
         if issubclass(annotation, Transformer):
```

### Comparing `discord.py-2.2.3/discord/app_commands/translator.py` & `discord.py-2.3.0/discord/app_commands/translator.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/app_commands/tree.py` & `discord.py-2.3.0/discord/app_commands/tree.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/appinfo.py` & `discord.py-2.3.0/discord/appinfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         from .team import Team
 
         self._state: ConnectionState = state
         self.id: int = int(data['id'])
         self.name: str = data['name']
         self.description: str = data['description']
         self._icon: Optional[str] = data['icon']
-        self.rpc_origins: List[str] = data['rpc_origins']
+        self.rpc_origins: Optional[List[str]] = data.get('rpc_origins')
         self.bot_public: bool = data['bot_public']
         self.bot_require_code_grant: bool = data['bot_require_code_grant']
         self.owner: User = state.create_user(data['owner'])
 
         team: Optional[TeamPayload] = data.get('team')
         self.team: Optional[Team] = Team(state, team) if team else None
 
@@ -251,52 +251,92 @@
     verify_key: :class:`str`
         The hex encoded key for verification in interactions and the
         GameSDK's :ddocs:`GetTicket <game-sdk/applications#getticket>`.
     terms_of_service_url: Optional[:class:`str`]
         The application's terms of service URL, if set.
     privacy_policy_url: Optional[:class:`str`]
         The application's privacy policy URL, if set.
+    approximate_guild_count: :class:`int`
+        The approximate count of the guilds the bot was added to.
+
+        .. versionadded:: 2.3
+    redirect_uris: List[:class:`str`]
+        A list of authentication redirect URIs.
+
+        .. versionadded:: 2.3
+    interactions_endpoint_url: Optional[:class:`str`]
+        The interactions endpoint url of the application to receive interactions over this endpoint rather than
+        over the gateway, if configured.
+
+        .. versionadded:: 2.3
+    role_connections_verification_url: Optional[:class:`str`]
+        The application's connection verification URL which will render the application as
+        a verification method in the guild's role verification configuration.
+
+        .. versionadded:: 2.3
     """
 
     __slots__ = (
         '_state',
         'id',
         'name',
         'description',
         'rpc_origins',
         'verify_key',
         'terms_of_service_url',
         'privacy_policy_url',
         '_icon',
         '_flags',
+        '_cover_image',
+        'approximate_guild_count',
+        'redirect_uris',
+        'interactions_endpoint_url',
+        'role_connections_verification_url',
     )
 
     def __init__(self, *, state: ConnectionState, data: PartialAppInfoPayload):
         self._state: ConnectionState = state
         self.id: int = int(data['id'])
         self.name: str = data['name']
         self._icon: Optional[str] = data.get('icon')
         self._flags: int = data.get('flags', 0)
+        self._cover_image: Optional[str] = data.get('cover_image')
         self.description: str = data['description']
         self.rpc_origins: Optional[List[str]] = data.get('rpc_origins')
         self.verify_key: str = data['verify_key']
         self.terms_of_service_url: Optional[str] = data.get('terms_of_service_url')
         self.privacy_policy_url: Optional[str] = data.get('privacy_policy_url')
+        self.approximate_guild_count: int = data.get('approximate_guild_count', 0)
+        self.redirect_uris: List[str] = data.get('redirect_uris', [])
+        self.interactions_endpoint_url: Optional[str] = data.get('interactions_endpoint_url')
+        self.role_connections_verification_url: Optional[str] = data.get('role_connections_verification_url')
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__} id={self.id} name={self.name!r} description={self.description!r}>'
 
     @property
     def icon(self) -> Optional[Asset]:
         """Optional[:class:`.Asset`]: Retrieves the application's icon asset, if any."""
         if self._icon is None:
             return None
         return Asset._from_icon(self._state, self.id, self._icon, path='app')
 
     @property
+    def cover_image(self) -> Optional[Asset]:
+        """Optional[:class:`.Asset`]: Retrieves the cover image of the application's default rich presence.
+
+        This is only available if the application is a game sold on Discord.
+
+        .. versionadded:: 2.3
+        """
+        if self._cover_image is None:
+            return None
+        return Asset._from_cover_image(self._state, self.id, self._cover_image)
+
+    @property
     def flags(self) -> ApplicationFlags:
         """:class:`ApplicationFlags`: The application's flags.
 
         .. versionadded:: 2.0
         """
         return ApplicationFlags._from_value(self._flags)
```

### Comparing `discord.py-2.2.3/discord/asset.py` & `discord.py-2.3.0/discord/asset.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/audit_logs.py` & `discord.py-2.3.0/discord/audit_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     from .types.invite import Invite as InvitePayload
     from .types.role import Role as RolePayload
     from .types.snowflake import Snowflake
     from .types.command import ApplicationCommandPermissions
     from .types.automod import AutoModerationTriggerMetadata, AutoModerationAction
     from .user import User
     from .app_commands import AppCommand
+    from .webhook import Webhook
 
     TargetType = Union[
         Guild,
         abc.GuildChannel,
         Member,
         User,
         Role,
@@ -85,14 +86,17 @@
         Emoji,
         StageInstance,
         GuildSticker,
         Thread,
         Object,
         PartialIntegration,
         AutoModRule,
+        ScheduledEvent,
+        Webhook,
+        AppCommand,
         None,
     ]
 
 
 def _transform_timestamp(entry: AuditLogEntry, data: Optional[str]) -> Optional[datetime.datetime]:
     return utils.parse_time(data)
 
@@ -576,23 +580,25 @@
     def __init__(
         self,
         *,
         users: Mapping[int, User],
         integrations: Mapping[int, PartialIntegration],
         app_commands: Mapping[int, AppCommand],
         automod_rules: Mapping[int, AutoModRule],
+        webhooks: Mapping[int, Webhook],
         data: AuditLogEntryPayload,
         guild: Guild,
     ):
         self._state: ConnectionState = guild._state
         self.guild: Guild = guild
         self._users: Mapping[int, User] = users
         self._integrations: Mapping[int, PartialIntegration] = integrations
         self._app_commands: Mapping[int, AppCommand] = app_commands
         self._automod_rules: Mapping[int, AutoModRule] = automod_rules
+        self._webhooks: Mapping[int, Webhook] = webhooks
         self._from_data(data)
 
     def _from_data(self, data: AuditLogEntryPayload) -> None:
         self.action: enums.AuditLogAction = enums.try_enum(enums.AuditLogAction, data['action_type'])
         self.id: int = int(data['id'])
 
         # this key is technically not usually present
@@ -642,15 +648,17 @@
             elif (
                 self.action is enums.AuditLogAction.automod_block_message
                 or self.action is enums.AuditLogAction.automod_flag_message
                 or self.action is enums.AuditLogAction.automod_timeout_member
             ):
                 channel_id = utils._get_as_snowflake(extra, 'channel_id')
                 channel = None
-                if channel_id is not None:
+
+                # May be an empty string instead of None due to a Discord issue
+                if channel_id:
                     channel = self.guild.get_channel_or_thread(channel_id) or Object(id=channel_id)
 
                 self.extra = _AuditLogProxyAutoModAction(
                     automod_rule_name=extra['auto_moderation_rule_name'],
                     automod_rule_trigger_type=enums.try_enum(
                         enums.AutoModRuleTriggerType, extra['auto_moderation_rule_trigger_type']
                     ),
@@ -845,7 +853,13 @@
             else:
                 return Object(target_id, type=type)
 
         return target
 
     def _convert_target_auto_moderation(self, target_id: int) -> Union[AutoModRule, Object]:
         return self._automod_rules.get(target_id) or Object(target_id, type=AutoModRule)
+
+    def _convert_target_webhook(self, target_id: int) -> Union[Webhook, Object]:
+        # circular import
+        from .webhook import Webhook
+
+        return self._webhooks.get(target_id) or Object(target_id, type=Webhook)
```

### Comparing `discord.py-2.2.3/discord/automod.py` & `discord.py-2.3.0/discord/automod.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 import datetime
 
-from typing import TYPE_CHECKING, Any, Dict, Optional, List, Sequence, Set, Union, Sequence
+from typing import TYPE_CHECKING, Any, Dict, Optional, List, Set, Union, Sequence, overload
 
 from .enums import AutoModRuleTriggerType, AutoModRuleActionType, AutoModRuleEventType, try_enum
 from .flags import AutoModPresets
 from . import utils
 from .utils import MISSING, cached_slot_property
 
 if TYPE_CHECKING:
@@ -54,14 +54,17 @@
     'AutoModAction',
 )
 
 
 class AutoModRuleAction:
     """Represents an auto moderation's rule action.
 
+    .. note::
+        Only one of ``channel_id``, ``duration``, or ``custom_message`` can be used.
+
     .. versionadded:: 2.0
 
     Attributes
     -----------
     type: :class:`AutoModRuleActionType`
         The type of action to take.
         Defaults to :attr:`~AutoModRuleActionType.block_message`.
@@ -77,41 +80,51 @@
         Passing this sets :attr:`type` to :attr:`~AutoModRuleActionType.block_message`.
 
         .. versionadded:: 2.2
     """
 
     __slots__ = ('type', 'channel_id', 'duration', 'custom_message')
 
+    @overload
+    def __init__(self, *, channel_id: Optional[int] = ...) -> None:
+        ...
+
+    @overload
+    def __init__(self, *, duration: Optional[datetime.timedelta] = ...) -> None:
+        ...
+
+    @overload
+    def __init__(self, *, custom_message: Optional[str] = ...) -> None:
+        ...
+
     def __init__(
         self,
         *,
         channel_id: Optional[int] = None,
         duration: Optional[datetime.timedelta] = None,
         custom_message: Optional[str] = None,
     ) -> None:
         self.channel_id: Optional[int] = channel_id
         self.duration: Optional[datetime.timedelta] = duration
         self.custom_message: Optional[str] = custom_message
 
         if sum(v is None for v in (channel_id, duration, custom_message)) < 2:
             raise ValueError('Only one of channel_id, duration, or custom_message can be passed.')
 
+        self.type: AutoModRuleActionType = AutoModRuleActionType.block_message
         if channel_id:
             self.type = AutoModRuleActionType.send_alert_message
         elif duration:
             self.type = AutoModRuleActionType.timeout
-        else:
-            self.type = AutoModRuleActionType.block_message
 
     def __repr__(self) -> str:
         return f'<AutoModRuleAction type={self.type.value} channel={self.channel_id} duration={self.duration}>'
 
     @classmethod
     def from_data(cls, data: AutoModerationActionPayload) -> Self:
-        type_ = try_enum(AutoModRuleActionType, data['type'])
         if data['type'] == AutoModRuleActionType.timeout.value:
             duration_seconds = data['metadata']['duration_seconds']
             return cls(duration=datetime.timedelta(seconds=duration_seconds))
         elif data['type'] == AutoModRuleActionType.send_alert_message.value:
             channel_id = int(data['metadata']['channel_id'])
             return cls(channel_id=channel_id)
         return cls(custom_message=data.get('metadata', {}).get('custom_message'))
```

### Comparing `discord.py-2.2.3/discord/backoff.py` & `discord.py-2.3.0/discord/backoff.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/bin/libopus-0.x64.dll` & `discord.py-2.3.0/discord/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/bin/libopus-0.x86.dll` & `discord.py-2.3.0/discord/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/channel.py` & `discord.py-2.3.0/discord/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     overload,
 )
 import datetime
 
 import discord.abc
 from .scheduled_event import ScheduledEvent
 from .permissions import PermissionOverwrite, Permissions
-from .enums import ChannelType, ForumLayoutType, PrivacyLevel, try_enum, VideoQualityMode, EntityType
+from .enums import ChannelType, ForumLayoutType, ForumOrderType, PrivacyLevel, try_enum, VideoQualityMode, EntityType
 from .mixins import Hashable
 from . import utils
 from .utils import MISSING
 from .asset import Asset
 from .errors import ClientException
 from .stage_instance import StageInstance
 from .threads import Thread
@@ -156,14 +156,18 @@
         :attr:`~Permissions.manage_messages` bypass slowmode.
     nsfw: :class:`bool`
         If the channel is marked as "not safe for work" or "age restricted".
     default_auto_archive_duration: :class:`int`
         The default auto archive duration in minutes for threads created in this channel.
 
         .. versionadded:: 2.0
+    default_thread_slowmode_delay: :class:`int`
+        The default slowmode delay in seconds for threads created in this channel.
+
+        .. versionadded:: 2.3
     """
 
     __slots__ = (
         'name',
         'id',
         'guild',
         'topic',
@@ -172,14 +176,15 @@
         'category_id',
         'position',
         'slowmode_delay',
         '_overwrites',
         '_type',
         'last_message_id',
         'default_auto_archive_duration',
+        'default_thread_slowmode_delay',
     )
 
     def __init__(self, *, state: ConnectionState, guild: Guild, data: Union[TextChannelPayload, NewsChannelPayload]):
         self._state: ConnectionState = state
         self.id: int = int(data['id'])
         self._type: Literal[0, 5] = data['type']
         self._update(guild, data)
@@ -202,14 +207,15 @@
         self.category_id: Optional[int] = utils._get_as_snowflake(data, 'parent_id')
         self.topic: Optional[str] = data.get('topic')
         self.position: int = data['position']
         self.nsfw: bool = data.get('nsfw', False)
         # Does this need coercion into `int`? No idea yet.
         self.slowmode_delay: int = data.get('rate_limit_per_user', 0)
         self.default_auto_archive_duration: ThreadArchiveDuration = data.get('default_auto_archive_duration', 1440)
+        self.default_thread_slowmode_delay: int = data.get('default_thread_rate_limit_per_user', 0)
         self._type: Literal[0, 5] = data.get('type', self._type)
         self.last_message_id: Optional[int] = utils._get_as_snowflake(data, 'last_message_id')
         self._fill_overwrites(data)
 
     async def _get_channel(self) -> Self:
         return self
 
@@ -297,14 +303,15 @@
         topic: str = ...,
         position: int = ...,
         nsfw: bool = ...,
         sync_permissions: bool = ...,
         category: Optional[CategoryChannel] = ...,
         slowmode_delay: int = ...,
         default_auto_archive_duration: ThreadArchiveDuration = ...,
+        default_thread_slowmode_delay: int = ...,
         type: ChannelType = ...,
         overwrites: Mapping[OverwriteKeyT, PermissionOverwrite] = ...,
     ) -> TextChannel:
         ...
 
     async def edit(self, *, reason: Optional[str] = None, **options: Any) -> Optional[TextChannel]:
         """|coro|
@@ -355,15 +362,18 @@
             A :class:`Mapping` of target (either a role or a member) to
             :class:`PermissionOverwrite` to apply to the channel.
         default_auto_archive_duration: :class:`int`
             The new default auto archive duration in minutes for threads created in this channel.
             Must be one of ``60``, ``1440``, ``4320``, or ``10080``.
 
             .. versionadded:: 2.0
+        default_thread_slowmode_delay: :class:`int`
+            The new default slowmode delay in seconds for threads created in this channel.
 
+            .. versionadded:: 2.3
         Raises
         ------
         ValueError
             The new ``position`` is less than 0 or greater than the number of channels.
         TypeError
             The permission overwrite information is not in proper form.
         Forbidden
@@ -723,15 +733,15 @@
         name: :class:`str`
             The name of the thread.
         message: Optional[:class:`abc.Snowflake`]
             A snowflake representing the message to create the thread with.
             If ``None`` is passed then a private thread is created.
             Defaults to ``None``.
         auto_archive_duration: :class:`int`
-            The duration in minutes before a thread is automatically archived for inactivity.
+            The duration in minutes before a thread is automatically hidden from the channel list.
             If not provided, the channel's default auto archive duration is used.
 
             Must be one of ``60``, ``1440``, ``4320``, or ``10080``, if provided.
         type: Optional[:class:`ChannelType`]
             The type of thread to create. If a ``message`` is passed then this parameter
             is ignored, as a thread created with a message is always a public thread.
             By default this creates a private thread if this is ``None``.
@@ -1580,15 +1590,20 @@
         """Optional[:class:`StageInstance`]: The running stage instance of the stage channel.
 
         .. versionadded:: 2.0
         """
         return utils.get(self.guild.stage_instances, channel_id=self.id)
 
     async def create_instance(
-        self, *, topic: str, privacy_level: PrivacyLevel = MISSING, reason: Optional[str] = None
+        self,
+        *,
+        topic: str,
+        privacy_level: PrivacyLevel = MISSING,
+        send_start_notification: bool = False,
+        reason: Optional[str] = None,
     ) -> StageInstance:
         """|coro|
 
         Create a stage instance.
 
         You must have :attr:`~Permissions.manage_channels` to do this.
 
@@ -1596,14 +1611,19 @@
 
         Parameters
         -----------
         topic: :class:`str`
             The stage instance's topic.
         privacy_level: :class:`PrivacyLevel`
             The stage instance's privacy level. Defaults to :attr:`PrivacyLevel.guild_only`.
+        send_start_notification: :class:`bool`
+            Whether to send a start notification. This sends a push notification to @everyone if ``True``. Defaults to ``False``.
+            You must have :attr:`~Permissions.mention_everyone` to do this.
+
+            .. versionadded:: 2.3
         reason: :class:`str`
             The reason the stage instance was created. Shows up on the audit log.
 
         Raises
         ------
         TypeError
             If the ``privacy_level`` parameter is not the proper type.
@@ -1622,14 +1642,16 @@
 
         if privacy_level is not MISSING:
             if not isinstance(privacy_level, PrivacyLevel):
                 raise TypeError('privacy_level field must be of type PrivacyLevel')
 
             payload['privacy_level'] = privacy_level.value
 
+        payload['send_start_notification'] = send_start_notification
+
         data = await self._state.http.create_stage_instance(**payload, reason=reason)
         return StageInstance(guild=self.guild, state=self._state, data=data)
 
     async def fetch_instance(self) -> StageInstance:
         """|coro|
 
         Gets the running :class:`StageInstance`.
@@ -1661,14 +1683,15 @@
 
     @overload
     async def edit(
         self,
         *,
         name: str = ...,
         nsfw: bool = ...,
+        user_limit: int = ...,
         position: int = ...,
         sync_permissions: int = ...,
         category: Optional[CategoryChannel] = ...,
         overwrites: Mapping[OverwriteKeyT, PermissionOverwrite] = ...,
         rtc_region: Optional[str] = ...,
         video_quality_mode: VideoQualityMode = ...,
         slowmode_delay: int = ...,
@@ -1700,14 +1723,16 @@
         ----------
         name: :class:`str`
             The new channel's name.
         position: :class:`int`
             The new channel's position.
         nsfw: :class:`bool`
             To mark the channel as NSFW or not.
+        user_limit: :class:`int`
+            The new channel's user limit.
         sync_permissions: :class:`bool`
             Whether to sync permissions with the channel's new or pre-existing
             category. Defaults to ``False``.
         category: Optional[:class:`CategoryChannel`]
             The new category for this channel. Can be ``None`` to remove the
             category.
         slowmode_delay: :class:`int`
@@ -2150,14 +2175,18 @@
 
         .. versionadded:: 2.1
     default_layout: :class:`ForumLayoutType`
         The default layout for posts in this forum channel.
         Defaults to :attr:`ForumLayoutType.not_set`.
 
         .. versionadded:: 2.2
+    default_sort_order: Optional[:class:`ForumOrderType`]
+        The default sort order for posts in this forum channel.
+
+        .. versionadded:: 2.3
     """
 
     __slots__ = (
         'name',
         'id',
         'guild',
         'topic',
@@ -2169,14 +2198,15 @@
         'slowmode_delay',
         '_overwrites',
         'last_message_id',
         'default_auto_archive_duration',
         'default_thread_slowmode_delay',
         'default_reaction_emoji',
         'default_layout',
+        'default_sort_order',
         '_available_tags',
         '_flags',
     )
 
     def __init__(self, *, state: ConnectionState, guild: Guild, data: ForumChannelPayload):
         self._state: ConnectionState = state
         self.id: int = int(data['id'])
@@ -2214,14 +2244,19 @@
         if default_reaction_emoji:
             self.default_reaction_emoji = PartialEmoji.with_state(
                 state=self._state,
                 id=utils._get_as_snowflake(default_reaction_emoji, 'emoji_id') or None,  # Coerce 0 -> None
                 name=default_reaction_emoji.get('emoji_name') or '',
             )
 
+        self.default_sort_order: Optional[ForumOrderType] = None
+        default_sort_order = data.get('default_sort_order')
+        if default_sort_order is not None:
+            self.default_sort_order = try_enum(ForumOrderType, default_sort_order)
+
         self._flags: int = data.get('flags', 0)
         self._fill_overwrites(data)
 
     @property
     def type(self) -> Literal[ChannelType.forum]:
         """:class:`ChannelType`: The channel's Discord type."""
         return ChannelType.forum
@@ -2340,14 +2375,15 @@
         default_auto_archive_duration: ThreadArchiveDuration = ...,
         type: ChannelType = ...,
         overwrites: Mapping[OverwriteKeyT, PermissionOverwrite] = ...,
         available_tags: Sequence[ForumTag] = ...,
         default_thread_slowmode_delay: int = ...,
         default_reaction_emoji: Optional[EmojiInputType] = ...,
         default_layout: ForumLayoutType = ...,
+        default_sort_order: ForumOrderType = ...,
         require_tag: bool = ...,
     ) -> ForumChannel:
         ...
 
     async def edit(self, *, reason: Optional[str] = None, **options: Any) -> Optional[ForumChannel]:
         """|coro|
 
@@ -2398,14 +2434,18 @@
             The new default reaction emoji for threads in this channel.
 
             .. versionadded:: 2.1
         default_layout: :class:`ForumLayoutType`
             The new default layout for posts in this forum.
 
             .. versionadded:: 2.2
+        default_sort_order: Optional[:class:`ForumOrderType`]
+            The new default sort order for posts in this forum.
+
+            .. versionadded:: 2.3
         require_tag: :class:`bool`
             Whether to require a tag for threads in this channel or not.
 
             .. versionadded:: 2.1
 
         Raises
         ------
@@ -2460,14 +2500,29 @@
             pass
         else:
             if not isinstance(layout, ForumLayoutType):
                 raise TypeError(f'default_layout parameter must be a ForumLayoutType not {layout.__class__.__name__}')
 
             options['default_forum_layout'] = layout.value
 
+        try:
+            sort_order = options.pop('default_sort_order')
+        except KeyError:
+            pass
+        else:
+            if sort_order is None:
+                options['default_sort_order'] = None
+            else:
+                if not isinstance(sort_order, ForumOrderType):
+                    raise TypeError(
+                        f'default_sort_order parameter must be a ForumOrderType not {sort_order.__class__.__name__}'
+                    )
+
+                options['default_sort_order'] = sort_order.value
+
         payload = await self._edit(options, reason=reason)
         if payload is not None:
             # the payload will always be the proper channel payload
             return self.__class__(state=self._state, guild=self.guild, data=payload)  # type: ignore
 
     async def create_tag(
         self,
@@ -2551,15 +2606,15 @@
         or ``view`` to create a thread in a forum, since forum channels must have a starter message.
 
         Parameters
         -----------
         name: :class:`str`
             The name of the thread.
         auto_archive_duration: :class:`int`
-            The duration in minutes before a thread is automatically archived for inactivity.
+            The duration in minutes before a thread is automatically hidden from the channel list.
             If not provided, the channel's default auto archive duration is used.
 
             Must be one of ``60``, ``1440``, ``4320``, or ``10080``, if provided.
         slowmode_delay: Optional[:class:`int`]
             Specifies the slowmode rate limit for user in this channel, in seconds.
             The maximum value possible is ``21600``. By default no slowmode rate limit
             if this is ``None``.
@@ -2831,15 +2886,20 @@
         The direct message channel ID.
     """
 
     __slots__ = ('id', 'recipient', 'me', '_state')
 
     def __init__(self, *, me: ClientUser, state: ConnectionState, data: DMChannelPayload):
         self._state: ConnectionState = state
-        self.recipient: Optional[User] = state.store_user(data['recipients'][0])
+        self.recipient: Optional[User] = None
+
+        recipients = data.get('recipients')
+        if recipients is not None:
+            self.recipient = state.store_user(recipients[0])
+
         self.me: ClientUser = me
         self.id: int = int(data['id'])
 
     async def _get_channel(self) -> Self:
         return self
 
     def __str__(self) -> str:
```

### Comparing `discord.py-2.2.3/discord/client.py` & `discord.py-2.3.0/discord/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2055,21 +2055,23 @@
 
     async def fetch_guilds(
         self,
         *,
         limit: Optional[int] = 200,
         before: Optional[SnowflakeTime] = None,
         after: Optional[SnowflakeTime] = None,
+        with_counts: bool = True,
     ) -> AsyncIterator[Guild]:
         """Retrieves an :term:`asynchronous iterator` that enables receiving your guilds.
 
         .. note::
 
             Using this, you will only receive :attr:`.Guild.owner`, :attr:`.Guild.icon`,
-            :attr:`.Guild.id`, and :attr:`.Guild.name` per :class:`.Guild`.
+            :attr:`.Guild.id`, :attr:`.Guild.name`, :attr:`.Guild.approximate_member_count`,
+            and :attr:`.Guild.approximate_presence_count` per :class:`.Guild`.
 
         .. note::
 
             This method is an API call. For general usage, consider :attr:`guilds` instead.
 
         Examples
         ---------
@@ -2102,41 +2104,47 @@
             Retrieves guilds before this date or object.
             If a datetime is provided, it is recommended to use a UTC aware datetime.
             If the datetime is naive, it is assumed to be local time.
         after: Union[:class:`.abc.Snowflake`, :class:`datetime.datetime`]
             Retrieve guilds after this date or object.
             If a datetime is provided, it is recommended to use a UTC aware datetime.
             If the datetime is naive, it is assumed to be local time.
+        with_counts: :class:`bool`
+            Whether to include count information in the guilds. This fills the
+            :attr:`.Guild.approximate_member_count` and :attr:`.Guild.approximate_presence_count`
+            attributes without needing any privileged intents. Defaults to ``True``.
+
+            .. versionadded:: 2.3
 
         Raises
         ------
         HTTPException
             Getting the guilds failed.
 
         Yields
         --------
         :class:`.Guild`
             The guild with the guild data parsed.
         """
 
         async def _before_strategy(retrieve: int, before: Optional[Snowflake], limit: Optional[int]):
             before_id = before.id if before else None
-            data = await self.http.get_guilds(retrieve, before=before_id)
+            data = await self.http.get_guilds(retrieve, before=before_id, with_counts=with_counts)
 
             if data:
                 if limit is not None:
                     limit -= len(data)
 
                 before = Object(id=int(data[0]['id']))
 
             return data, before, limit
 
         async def _after_strategy(retrieve: int, after: Optional[Snowflake], limit: Optional[int]):
             after_id = after.id if after else None
-            data = await self.http.get_guilds(retrieve, after=after_id)
+            data = await self.http.get_guilds(retrieve, after=after_id, with_counts=with_counts)
 
             if data:
                 if limit is not None:
                     limit -= len(data)
 
                 after = Object(id=int(data[-1]['id']))
 
@@ -2482,16 +2490,14 @@
 
         Returns
         --------
         :class:`.AppInfo`
             The bot's application information.
         """
         data = await self.http.application_info()
-        if 'rpc_origins' not in data:
-            data['rpc_origins'] = None
         return AppInfo(self._connection, data)
 
     async def fetch_user(self, user_id: int, /) -> User:
         """|coro|
 
         Retrieves a :class:`~discord.User` based on their ID.
         You do not have to share any guilds with the user to get this information,
```

### Comparing `discord.py-2.2.3/discord/colour.py` & `discord.py-2.3.0/discord/colour.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,9 +505,19 @@
 
         .. colour:: #EEEFF1
 
         .. versionadded:: 2.2
         """
         return cls(0xEEEFF1)
 
+    @classmethod
+    def pink(cls) -> Self:
+        """A factory method that returns a :class:`Colour` with a value of ``0xEB459F``.
+
+        .. colour:: #EB459F
+
+        .. versionadded:: 2.3
+        """
+        return cls(0xEB459F)
+
 
 Color = Colour
```

### Comparing `discord.py-2.2.3/discord/components.py` & `discord.py-2.3.0/discord/components.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/context_managers.py` & `discord.py-2.3.0/discord/context_managers.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/embeds.py` & `discord.py-2.3.0/discord/embeds.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/emoji.py` & `discord.py-2.3.0/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/enums.py` & `discord.py-2.3.0/discord/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     'AppCommandType',
     'AppCommandOptionType',
     'AppCommandPermissionType',
     'AutoModRuleTriggerType',
     'AutoModRuleEventType',
     'AutoModRuleActionType',
     'ForumLayoutType',
+    'ForumOrderType',
 )
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 
 def _create_value_cls(name: str, comparable: bool):
@@ -290,14 +291,15 @@
 class DefaultAvatar(Enum):
     blurple = 0
     grey = 1
     gray = 1
     green = 2
     orange = 3
     red = 4
+    pink = 5
 
     def __str__(self) -> str:
         return self.name
 
 
 class NotificationLevel(Enum, comparable=True):
     all_messages = 0
@@ -747,14 +749,19 @@
 
 class ForumLayoutType(Enum):
     not_set = 0
     list_view = 1
     gallery_view = 2
 
 
+class ForumOrderType(Enum):
+    latest_activity = 0
+    creation_date = 1
+
+
 def create_unknown_value(cls: Type[E], val: Any) -> E:
     value_cls = cls._enum_value_cls_  # type: ignore # This is narrowed below
     name = f'unknown_{val}'
     return value_cls(name=name, value=val)
 
 
 def try_enum(cls: Type[E], val: Any) -> E:
```

### Comparing `discord.py-2.2.3/discord/errors.py` & `discord.py-2.3.0/discord/errors.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ext/commands/_types.py` & `discord.py-2.3.0/discord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ext/commands/bot.py` & `discord.py-2.3.0/discord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ext/commands/cog.py` & `discord.py-2.3.0/discord/ext/commands/cog.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,14 +546,16 @@
     async def cog_unload(self) -> None:
         """|maybecoro|
 
         A special method that is called when the cog gets removed.
 
         Subclasses must replace this if they want special unloading behaviour.
 
+        Exceptions raised in this method are ignored during extension unloading.
+
         .. versionchanged:: 2.0
 
             This method can now be a :term:`coroutine`.
         """
         pass
 
     @_cog_special_method
```

### Comparing `discord.py-2.2.3/discord/ext/commands/context.py` & `discord.py-2.3.0/discord/ext/commands/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 from __future__ import annotations
 
 import re
-from typing import TYPE_CHECKING, Any, Dict, Generator, Generic, List, Optional, TypeVar, Union, Sequence, Type
+from typing import TYPE_CHECKING, Any, Dict, Generator, Generic, List, Optional, TypeVar, Union, Sequence, Type, overload
 
 import discord.abc
 import discord.utils
 from discord import Interaction, Message, Attachment, MessageType, User, PartialMessageable, Permissions, ChannelType, Thread
 from discord.context_managers import Typing
 from .view import StringView
 
@@ -426,14 +426,22 @@
     def cog(self) -> Optional[Cog]:
         """Optional[:class:`.Cog`]: Returns the cog associated with this context's command. None if it does not exist."""
 
         if self.command is None:
             return None
         return self.command.cog
 
+    @property
+    def filesize_limit(self) -> int:
+        """:class:`int`: Returns the maximum number of bytes files can have when uploaded to this guild or DM channel associated with this context.
+
+        .. versionadded:: 2.3
+        """
+        return self.guild.filesize_limit if self.guild is not None else discord.utils.DEFAULT_FILE_SIZE_LIMIT_BYTES
+
     @discord.utils.cached_property
     def guild(self) -> Optional[Guild]:
         """Optional[:class:`.Guild`]: Returns the guild associated with this context's command. None if not available."""
         return self.message.guild
 
     @discord.utils.cached_property
     def channel(self) -> MessageableChannel:
@@ -611,14 +619,98 @@
                 injected = wrap_callback(cmd.send_command_help)
                 return await injected(entity)
             else:
                 return None
         except CommandError as e:
             await cmd.on_help_command_error(self, e)
 
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embed: Embed = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        ephemeral: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embed: Embed = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        ephemeral: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embeds: Sequence[Embed] = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        ephemeral: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embeds: Sequence[Embed] = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        ephemeral: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
     async def reply(self, content: Optional[str] = None, **kwargs: Any) -> Message:
         """|coro|
 
         A shortcut method to :meth:`send` to reply to the
         :class:`~discord.Message` referenced by this context.
 
         For interaction based contexts, this is the same as :meth:`send`.
@@ -712,14 +804,98 @@
         InteractionResponded
             This interaction has already been responded to before.
         """
 
         if self.interaction:
             await self.interaction.response.defer(ephemeral=ephemeral)
 
+    @overload
+    async def send(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embed: Embed = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        ephemeral: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def send(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embed: Embed = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        ephemeral: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def send(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embeds: Sequence[Embed] = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        ephemeral: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def send(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embeds: Sequence[Embed] = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        ephemeral: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
     async def send(
         self,
         content: Optional[str] = None,
         *,
         tts: bool = False,
         embed: Optional[Embed] = None,
         embeds: Optional[Sequence[Embed]] = None,
```

### Comparing `discord.py-2.2.3/discord/ext/commands/converter.py` & `discord.py-2.3.0/discord/ext/commands/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,35 +182,44 @@
     All lookups are via the local guild. If in a DM context, then the lookup
     is done by the global cache.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by mention.
-    3. Lookup by name#discrim
-    4. Lookup by name
-    5. Lookup by nickname
+    3. Lookup by username#discriminator (deprecated).
+    4. Lookup by username#0 (deprecated, only gets users that migrated from their discriminator).
+    5. Lookup by guild nickname.
+    6. Lookup by global name.
+    7. Lookup by user name.
 
     .. versionchanged:: 1.5
          Raise :exc:`.MemberNotFound` instead of generic :exc:`.BadArgument`
 
     .. versionchanged:: 1.5.1
         This converter now lazily fetches members from the gateway and HTTP APIs,
         optionally caching the result if :attr:`.MemberCacheFlags.joined` is enabled.
+
+    .. deprecated:: 2.3
+        Looking up users by discriminator will be removed in a future version due to
+        the removal of discriminators in an API change.
     """
 
     async def query_member_named(self, guild: discord.Guild, argument: str) -> Optional[discord.Member]:
         cache = guild._state.member_cache_flags.joined
-        if len(argument) > 5 and argument[-5] == '#':
-            username, _, discriminator = argument.rpartition('#')
-            members = await guild.query_members(username, limit=100, cache=cache)
-            return discord.utils.get(members, name=username, discriminator=discriminator)
+        username, _, discriminator = argument.rpartition('#')
+        if discriminator == '0' or (len(discriminator) == 4 and discriminator.isdigit()):
+            lookup = username
+            predicate = lambda m: m.name == username and m.discriminator == discriminator
         else:
-            members = await guild.query_members(argument, limit=100, cache=cache)
-            return discord.utils.find(lambda m: m.name == argument or m.nick == argument, members)
+            lookup = argument
+            predicate = lambda m: m.nick == argument or m.global_name == argument or m.name == argument
+
+        members = await guild.query_members(lookup, limit=100, cache=cache)
+        return discord.utils.find(predicate, members)
 
     async def query_member_by_id(self, bot: _Bot, guild: discord.Guild, user_id: int) -> Optional[discord.Member]:
         ws = bot._get_websocket(shard_id=guild.shard_id)
         cache = guild._state.member_cache_flags.joined
         if ws.is_ratelimited():
             # If we're being rate limited on the WS, then fall back to using the HTTP API
             # So we don't have to wait ~60 seconds for the query to finish
@@ -269,23 +278,29 @@
 
     All lookups are via the global user cache.
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by mention.
-    3. Lookup by name#discrim
-    4. Lookup by name
+    3. Lookup by username#discriminator (deprecated).
+    4. Lookup by username#0 (deprecated, only gets users that migrated from their discriminator).
+    5. Lookup by global name.
+    6. Lookup by user name.
 
     .. versionchanged:: 1.5
          Raise :exc:`.UserNotFound` instead of generic :exc:`.BadArgument`
 
     .. versionchanged:: 1.6
         This converter now lazily fetches users from the HTTP APIs if an ID is passed
         and it's not available in cache.
+
+    .. deprecated:: 2.3
+        Looking up users by discriminator will be removed in a future version due to
+        the removal of discriminators in an API change.
     """
 
     async def convert(self, ctx: Context[BotT], argument: str) -> discord.User:
         match = self._get_id_match(argument) or re.match(r'<@!?([0-9]{15,20})>$', argument)
         result = None
         state = ctx._state
 
@@ -296,33 +311,21 @@
                 try:
                     result = await ctx.bot.fetch_user(user_id)
                 except discord.HTTPException:
                     raise UserNotFound(argument) from None
 
             return result  # type: ignore
 
-        arg = argument
-
-        # Remove the '@' character if this is the first character from the argument
-        if arg[0] == '@':
-            # Remove first character
-            arg = arg[1:]
-
-        # check for discriminator if it exists,
-        if len(arg) > 5 and arg[-5] == '#':
-            discrim = arg[-4:]
-            name = arg[:-5]
-            predicate = lambda u: u.name == name and u.discriminator == discrim
-            result = discord.utils.find(predicate, state._users.values())
-            if result is not None:
-                return result
+        username, _, discriminator = argument.rpartition('#')
+        if discriminator == '0' or (len(discriminator) == 4 and discriminator.isdigit()):
+            predicate = lambda u: u.name == username and u.discriminator == discriminator
+        else:
+            predicate = lambda u: u.global_name == argument or u.name == argument
 
-        predicate = lambda u: u.name == arg
         result = discord.utils.find(predicate, state._users.values())
-
         if result is None:
             raise UserNotFound(argument)
 
         return result
 
 
 class PartialMessageConverter(Converter[discord.PartialMessage]):
@@ -1326,15 +1329,15 @@
                 else:
                     conversions[literal_type] = value
 
             if value == literal:
                 return value
 
         # if we're here, then we failed to match all the literals
-        raise BadLiteralArgument(param, literal_args, errors)
+        raise BadLiteralArgument(param, literal_args, errors, argument)
 
     # This must be the last if-clause in the chain of origin checking
     # Nearly every type is a generic type within the typing library
     # So care must be taken to make sure a more specialised origin handle
     # isn't overwritten by the widest if clause
     if origin is not None and is_generic_type(converter):
         converter = origin
```

### Comparing `discord.py-2.2.3/discord/ext/commands/cooldowns.py` & `discord.py-2.3.0/discord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ext/commands/core.py` & `discord.py-2.3.0/discord/ext/commands/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
                         parameter._annotation = default.annotation
                 else:
                     parameter._annotation = default.annotation
 
             parameter._default = default.default
             parameter._description = default._description
             parameter._displayed_default = default._displayed_default
+            parameter._displayed_name = default._displayed_name
 
         annotation = parameter.annotation
 
         if annotation is None:
             params[name] = parameter.replace(annotation=type(None))
             continue
 
@@ -190,16 +191,21 @@
     divide = PARAMETER_HEADING_REGEX.split(docstring, 1)
     if len(divide) == 1:
         return docstring
 
     description, param_docstring = divide
     for match in NUMPY_DOCSTRING_ARG_REGEX.finditer(param_docstring):
         name = match.group('name')
+
         if name not in params:
-            continue
+            is_display_name = discord.utils.get(params.values(), displayed_name=name)
+            if is_display_name:
+                name = is_display_name.name
+            else:
+                continue
 
         param = params[name]
         if param.description is None:
             param._description = _fold_text(match.group('description'))
 
     return _fold_text(description.strip())
 
@@ -1165,15 +1171,17 @@
             return self.usage
 
         params = self.clean_params
         if not params:
             return ''
 
         result = []
-        for name, param in params.items():
+        for param in params.values():
+            name = param.displayed_name or param.name
+
             greedy = isinstance(param.converter, Greedy)
             optional = False  # postpone evaluation of if it's an optional argument
 
             annotation: Any = param.converter.converter if greedy else param.converter
             origin = getattr(annotation, '__origin__', None)
             if not greedy and origin is Union:
                 none_cls = type(None)
@@ -2032,15 +2040,15 @@
 
     def predicate(ctx: Context[BotT]) -> bool:
         if ctx.guild is None:
             raise NoPrivateMessage()
 
         # ctx.guild is None doesn't narrow ctx.author to Member
         if isinstance(item, int):
-            role = discord.utils.get(ctx.author.roles, id=item)  # type: ignore
+            role = ctx.author.get_role(item)  # type: ignore
         else:
             role = discord.utils.get(ctx.author.roles, name=item)  # type: ignore
         if role is None:
             raise MissingRole(item)
         return True
 
     return check(predicate)
@@ -2079,16 +2087,20 @@
     """
 
     def predicate(ctx):
         if ctx.guild is None:
             raise NoPrivateMessage()
 
         # ctx.guild is None doesn't narrow ctx.author to Member
-        getter = functools.partial(discord.utils.get, ctx.author.roles)
-        if any(getter(id=item) is not None if isinstance(item, int) else getter(name=item) is not None for item in items):
+        if any(
+            ctx.author.get_role(item) is not None
+            if isinstance(item, int)
+            else discord.utils.get(ctx.author.roles, name=item) is not None
+            for item in items
+        ):
             return True
         raise MissingAnyRole(list(items))
 
     return check(predicate)
 
 
 def bot_has_role(item: int, /) -> Callable[[T], T]:
@@ -2109,19 +2121,18 @@
         ``item`` parameter is now positional-only.
     """
 
     def predicate(ctx):
         if ctx.guild is None:
             raise NoPrivateMessage()
 
-        me = ctx.me
         if isinstance(item, int):
-            role = discord.utils.get(me.roles, id=item)
+            role = ctx.me.get_role(item)
         else:
-            role = discord.utils.get(me.roles, name=item)
+            role = discord.utils.get(ctx.me.roles, name=item)
         if role is None:
             raise BotMissingRole(item)
         return True
 
     return check(predicate)
 
 
@@ -2140,16 +2151,18 @@
     """
 
     def predicate(ctx):
         if ctx.guild is None:
             raise NoPrivateMessage()
 
         me = ctx.me
-        getter = functools.partial(discord.utils.get, me.roles)
-        if any(getter(id=item) is not None if isinstance(item, int) else getter(name=item) is not None for item in items):
+        if any(
+            me.get_role(item) is not None if isinstance(item, int) else discord.utils.get(me.roles, name=item) is not None
+            for item in items
+        ):
             return True
         raise BotMissingAnyRole(list(items))
 
     return check(predicate)
 
 
 def has_permissions(**perms: bool) -> Check[Any]:
```

### Comparing `discord.py-2.2.3/discord/ext/commands/errors.py` & `discord.py-2.3.0/discord/ext/commands/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     -----------
     param: :class:`Parameter`
         The argument that is missing.
     """
 
     def __init__(self, param: Parameter) -> None:
         self.param: Parameter = param
-        super().__init__(f'{param.name} is a required argument that is missing.')
+        super().__init__(f'{param.displayed_name or param.name} is a required argument that is missing.')
 
 
 class MissingRequiredAttachment(UserInputError):
     """Exception raised when parsing a command and a parameter
     that requires an attachment is not given.
 
     This inherits from :exc:`UserInputError`
@@ -197,15 +197,15 @@
     -----------
     param: :class:`Parameter`
         The argument that is missing an attachment.
     """
 
     def __init__(self, param: Parameter) -> None:
         self.param: Parameter = param
-        super().__init__(f'{param.name} is a required argument that is missing an attachment.')
+        super().__init__(f'{param.displayed_name or param.name} is a required argument that is missing an attachment.')
 
 
 class TooManyArguments(UserInputError):
     """Exception raised when the command was passed too many arguments and its
     :attr:`.Command.ignore_extra` attribute was not set to ``True``.
 
     This inherits from :exc:`UserInputError`
@@ -897,15 +897,15 @@
 
         to_string = [_get_name(x) for x in converters]
         if len(to_string) > 2:
             fmt = '{}, or {}'.format(', '.join(to_string[:-1]), to_string[-1])
         else:
             fmt = ' or '.join(to_string)
 
-        super().__init__(f'Could not convert "{param.name}" into {fmt}.')
+        super().__init__(f'Could not convert "{param.displayed_name or param.name}" into {fmt}.')
 
 
 class BadLiteralArgument(UserInputError):
     """Exception raised when a :data:`typing.Literal` converter fails for all
     its associated values.
 
     This inherits from :exc:`UserInputError`
@@ -916,28 +916,33 @@
     -----------
     param: :class:`inspect.Parameter`
         The parameter that failed being converted.
     literals: Tuple[Any, ``...``]
         A tuple of values compared against in conversion, in order of failure.
     errors: List[:class:`CommandError`]
         A list of errors that were caught from failing the conversion.
+    argument: :class:`str`
+        The argument's value that failed to be converted. Defaults to an empty string.
+
+        .. versionadded:: 2.3
     """
 
-    def __init__(self, param: Parameter, literals: Tuple[Any, ...], errors: List[CommandError]) -> None:
+    def __init__(self, param: Parameter, literals: Tuple[Any, ...], errors: List[CommandError], argument: str = "") -> None:
         self.param: Parameter = param
         self.literals: Tuple[Any, ...] = literals
         self.errors: List[CommandError] = errors
+        self.argument: str = argument
 
         to_string = [repr(l) for l in literals]
         if len(to_string) > 2:
             fmt = '{}, or {}'.format(', '.join(to_string[:-1]), to_string[-1])
         else:
             fmt = ' or '.join(to_string)
 
-        super().__init__(f'Could not convert "{param.name}" into the literal {fmt}.')
+        super().__init__(f'Could not convert "{param.displayed_name or param.name}" into the literal {fmt}.')
 
 
 class ArgumentParsingError(UserInputError):
     """An exception raised when the parser fails to parse a user's input.
 
     This inherits from :exc:`UserInputError`.
```

### Comparing `discord.py-2.2.3/discord/ext/commands/flags.py` & `discord.py-2.3.0/discord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ext/commands/help.py` & `discord.py-2.3.0/discord/ext/commands/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -1162,15 +1162,15 @@
             return
 
         self.paginator.add_line(self.arguments_heading)
         max_size = self.get_max_size(arguments)  # type: ignore # not a command
 
         get_width = discord.utils._string_width
         for argument in arguments:
-            name = argument.name
+            name = argument.displayed_name or argument.name
             width = max_size - (get_width(name) - len(name))
             entry = f'{self.indent * " "}{name:<{width}} {argument.description or self.default_argument_description}'
             # we do not want to shorten the default value, if any.
             entry = self.shorten_text(entry)
             if argument.displayed_default is not None:
                 entry += f' (default: {argument.displayed_default})'
```

### Comparing `discord.py-2.2.3/discord/ext/commands/hybrid.py` & `discord.py-2.3.0/discord/ext/commands/hybrid.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ext/commands/parameters.py` & `discord.py-2.3.0/discord/ext/commands/parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,64 +83,70 @@
     r"""A class that stores information on a :class:`Command`\'s parameter.
 
     This is a subclass of :class:`inspect.Parameter`.
 
     .. versionadded:: 2.0
     """
 
-    __slots__ = ('_displayed_default', '_description', '_fallback')
+    __slots__ = ('_displayed_default', '_description', '_fallback', '_displayed_name')
 
     def __init__(
         self,
         name: str,
         kind: ParamKinds,
         default: Any = empty,
         annotation: Any = empty,
         description: str = empty,
         displayed_default: str = empty,
+        displayed_name: str = empty,
     ) -> None:
         super().__init__(name=name, kind=kind, default=default, annotation=annotation)
         self._name = name
         self._kind = kind
         self._description = description
         self._default = default
         self._annotation = annotation
         self._displayed_default = displayed_default
         self._fallback = False
+        self._displayed_name = displayed_name
 
     def replace(
         self,
         *,
         name: str = MISSING,  # MISSING here cause empty is valid
         kind: ParamKinds = MISSING,
         default: Any = MISSING,
         annotation: Any = MISSING,
         description: str = MISSING,
         displayed_default: Any = MISSING,
+        displayed_name: Any = MISSING,
     ) -> Self:
         if name is MISSING:
             name = self._name
         if kind is MISSING:
             kind = self._kind  # type: ignore  # this assignment is actually safe
         if default is MISSING:
             default = self._default
         if annotation is MISSING:
             annotation = self._annotation
         if description is MISSING:
             description = self._description
         if displayed_default is MISSING:
             displayed_default = self._displayed_default
+        if displayed_name is MISSING:
+            displayed_name = self._displayed_name
 
         return self.__class__(
             name=name,
             kind=kind,
             default=default,
             annotation=annotation,
             description=description,
             displayed_default=displayed_default,
+            displayed_name=displayed_name,
         )
 
     if not TYPE_CHECKING:  # this is to prevent anything breaking if inspect internals change
         name = _gen_property('name')
         kind = _gen_property('kind')
         default = _gen_property('default')
         annotation = _gen_property('annotation')
@@ -167,14 +173,22 @@
     def displayed_default(self) -> Optional[str]:
         """Optional[:class:`str`]: The displayed default in :class:`Command.signature`."""
         if self._displayed_default is not empty:
             return self._displayed_default
 
         return None if self.required else str(self.default)
 
+    @property
+    def displayed_name(self) -> Optional[str]:
+        """Optional[:class:`str`]: The name that is displayed to the user.
+
+        .. versionadded:: 2.3
+        """
+        return self._displayed_name if self._displayed_name is not empty else None
+
     async def get_default(self, ctx: Context[Any]) -> Any:
         """|coro|
 
         Gets this parameter's default value.
 
         Parameters
         ----------
@@ -189,16 +203,17 @@
 
 def parameter(
     *,
     converter: Any = empty,
     default: Any = empty,
     description: str = empty,
     displayed_default: str = empty,
+    displayed_name: str = empty,
 ) -> Any:
-    r"""parameter(\*, converter=..., default=..., description=..., displayed_default=...)
+    r"""parameter(\*, converter=..., default=..., description=..., displayed_default=..., displayed_name=...)
 
     A way to assign custom metadata for a :class:`Command`\'s parameter.
 
     .. versionadded:: 2.0
 
     Examples
     --------
@@ -217,39 +232,45 @@
     default: Any
         The default value for the parameter, if this is a :term:`callable` or a |coroutine_link|_ it is called with a
         positional :class:`Context` argument.
     description: :class:`str`
         The description of this parameter.
     displayed_default: :class:`str`
         The displayed default in :attr:`Command.signature`.
+    displayed_name: :class:`str`
+        The name that is displayed to the user.
+
+        .. versionadded:: 2.3
     """
     return Parameter(
         name='empty',
         kind=inspect.Parameter.POSITIONAL_OR_KEYWORD,
         annotation=converter,
         default=default,
         description=description,
         displayed_default=displayed_default,
+        displayed_name=displayed_name,
     )
 
 
 class ParameterAlias(Protocol):
     def __call__(
         self,
         *,
         converter: Any = empty,
         default: Any = empty,
         description: str = empty,
         displayed_default: str = empty,
+        displayed_name: str = empty,
     ) -> Any:
         ...
 
 
 param: ParameterAlias = parameter
-r"""param(\*, converter=..., default=..., description=..., displayed_default=...)
+r"""param(\*, converter=..., default=..., description=..., displayed_default=..., displayed_name=...)
 
 An alias for :func:`parameter`.
 
 .. versionadded:: 2.0
 """
 
 # some handy defaults
```

### Comparing `discord.py-2.2.3/discord/ext/commands/view.py` & `discord.py-2.3.0/discord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ext/tasks/__init__.py` & `discord.py-2.3.0/discord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/file.py` & `discord.py-2.3.0/discord/file.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/flags.py` & `discord.py-2.3.0/discord/flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 from functools import reduce
+from operator import or_
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, Iterator, List, Optional, Tuple, Type, TypeVar, overload
 
 from .enums import UserFlags
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
@@ -234,14 +235,20 @@
                Return the flag's hash.
 
         .. describe:: iter(x)
 
                Returns an iterator of ``(name, value)`` pairs. This allows it
                to be, for example, constructed as a dict or a list of pairs.
 
+        .. describe:: bool(b)
+
+            Returns whether any flag is set to ``True``.
+
+            .. versionadded:: 2.0
+
     Attributes
     -----------
     value: :class:`int`
         The raw value. This value is a bit array field of a 53-bit integer
         representing the currently available flags. You should query
         flags via the properties rather than using this raw value.
     """
@@ -356,14 +363,20 @@
 
                Return the flag's hash.
         .. describe:: iter(x)
 
                Returns an iterator of ``(name, value)`` pairs. This allows it
                to be, for example, constructed as a dict or a list of pairs.
 
+        .. describe:: bool(b)
+
+            Returns whether any flag is set to ``True``.
+
+            .. versionadded:: 2.0
+
     .. versionadded:: 1.3
 
     Attributes
     -----------
     value: :class:`int`
         The raw value. This value is a bit array field of a 53-bit integer
         representing the currently available flags. You should query
@@ -446,14 +459,22 @@
     def silent(self):
         """:class:`bool`: Alias for :attr:`suppress_notifications`.
 
         .. versionadded:: 2.2
         """
         return 4096
 
+    @flag_value
+    def voice(self):
+        """:class:`bool`: Returns ``True`` if the message is a voice message.
+
+        .. versionadded:: 2.3
+        """
+        return 8192
+
 
 @fill_with_flags()
 class PublicUserFlags(BaseFlags):
     r"""Wraps up the Discord User Public flags.
 
     .. container:: operations
 
@@ -496,14 +517,20 @@
             Return the flag's hash.
         .. describe:: iter(x)
 
             Returns an iterator of ``(name, value)`` pairs. This allows it
             to be, for example, constructed as a dict or a list of pairs.
             Note that aliases are not shown.
 
+        .. describe:: bool(b)
+
+            Returns whether any flag is set to ``True``.
+
+            .. versionadded:: 2.0
+
     .. versionadded:: 1.4
 
     Attributes
     -----------
     value: :class:`int`
         The raw value. This value is a bit array field of a 53-bit integer
         representing the currently available flags. You should query
@@ -680,14 +707,20 @@
 
                Return the flag's hash.
         .. describe:: iter(x)
 
                Returns an iterator of ``(name, value)`` pairs. This allows it
                to be, for example, constructed as a dict or a list of pairs.
 
+        .. describe:: bool(b)
+
+            Returns whether any intent is enabled.
+
+            .. versionadded:: 2.0
+
     Attributes
     -----------
     value: :class:`int`
         The raw value. You should query flags via the properties
         rather than using this raw value.
     """
 
@@ -779,14 +812,15 @@
         - :attr:`Guild.members`
         - :attr:`Member.roles`
         - :attr:`Member.nick`
         - :attr:`Member.premium_since`
         - :attr:`User.name`
         - :attr:`User.avatar`
         - :attr:`User.discriminator`
+        - :attr:`User.global_name`
 
         For more information go to the :ref:`member intent documentation <need_members_intent>`.
 
         .. note::
 
             Currently, this requires opting in explicitly via the developer portal as well.
             Bots in over 100 guilds will need to apply to Discord for verification.
@@ -1265,14 +1299,20 @@
 
                Return the flag's hash.
         .. describe:: iter(x)
 
                Returns an iterator of ``(name, value)`` pairs. This allows it
                to be, for example, constructed as a dict or a list of pairs.
 
+        .. describe:: bool(b)
+
+            Returns whether any flag is set to ``True``.
+
+            .. versionadded:: 2.0
+
     Attributes
     -----------
     value: :class:`int`
         The raw value. You should query flags via the properties
         rather than using this raw value.
     """
 
@@ -1408,24 +1448,37 @@
             Return the flag's hash.
         .. describe:: iter(x)
 
             Returns an iterator of ``(name, value)`` pairs. This allows it
             to be, for example, constructed as a dict or a list of pairs.
             Note that aliases are not shown.
 
+        .. describe:: bool(b)
+
+            Returns whether any flag is set to ``True``.
+
     .. versionadded:: 2.0
 
     Attributes
     -----------
     value: :class:`int`
         The raw value. You should query flags via the properties
         rather than using this raw value.
     """
 
     @flag_value
+    def auto_mod_badge(self):
+        """:class:`bool`: Returns ``True`` if the application uses at least 100 automod rules across all guilds.
+        This shows up as a badge in the official client.
+
+        .. versionadded:: 2.3
+        """
+        return 1 << 6
+
+    @flag_value
     def gateway_presence(self):
         """:class:`bool`: Returns ``True`` if the application is verified and is allowed to
         receive presence information over the gateway.
         """
         return 1 << 12
 
     @flag_value
@@ -1534,14 +1587,18 @@
             Return the flag's hash.
         .. describe:: iter(x)
 
             Returns an iterator of ``(name, value)`` pairs. This allows it
             to be, for example, constructed as a dict or a list of pairs.
             Note that aliases are not shown.
 
+        .. describe:: bool(b)
+
+            Returns whether any flag is set to ``True``.
+
     .. versionadded:: 2.0
 
     Attributes
     -----------
     value: :class:`int`
         The raw value. You should query flags via the properties
         rather than using this raw value.
@@ -1562,15 +1619,23 @@
         return 1 << 4
 
 
 class ArrayFlags(BaseFlags):
     @classmethod
     def _from_value(cls: Type[Self], value: List[int]) -> Self:
         self = cls.__new__(cls)
-        self.value = reduce(lambda a, b: a | (1 << b - 1), value, 0)
+        # This is a micro-optimization given the frequency this object can be created.
+        # (1).__lshift__ is used in place of lambda x: 1 << x
+        # prebinding to a method of a constant rather than define a lambda.
+        # Pairing this with map, is essentially equivalent to (1 << x for x in value)
+        # reduction using operator.or_ instead of defining a lambda each call
+        # Discord sends these starting with a value of 1
+        # Rather than subtract 1 from each element prior to left shift,
+        # we shift right by 1 once at the end.
+        self.value = reduce(or_, map((1).__lshift__, value), 0) >> 1
         return self
 
     def to_array(self) -> List[int]:
         return [i + 1 for i in range(self.value.bit_length()) if self.value & (1 << i)]
 
 
 @fill_with_flags()
@@ -1622,14 +1687,18 @@
             Return the flag's hash.
         .. describe:: iter(x)
 
             Returns an iterator of ``(name, value)`` pairs. This allows it
             to be, for example, constructed as a dict or a list of pairs.
             Note that aliases are not shown.
 
+        .. describe:: bool(b)
+
+            Returns whether any flag is set to ``True``.
+
     Attributes
     -----------
     value: :class:`int`
         The raw value. You should query flags via the properties
         rather than using this raw value.
     """
 
@@ -1706,14 +1775,18 @@
 
         .. describe:: iter(x)
 
             Returns an iterator of ``(name, value)`` pairs. This allows it
             to be, for example, constructed as a dict or a list of pairs.
             Note that aliases are not shown.
 
+        .. describe:: bool(b)
+
+            Returns whether any flag is set to ``True``.
+
 
     Attributes
     -----------
     value: :class:`int`
         The raw value. You should query flags via the properties
         rather than using this raw value.
     """
```

### Comparing `discord.py-2.2.3/discord/gateway.py` & `discord.py-2.3.0/discord/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -911,14 +911,15 @@
 
     async def speak(self, state: SpeakingState = SpeakingState.voice) -> None:
         payload = {
             'op': self.SPEAKING,
             'd': {
                 'speaking': int(state),
                 'delay': 0,
+                'ssrc': self._connection.ssrc,
             },
         }
 
         await self.send_as_json(payload)
 
     async def received_message(self, msg: Dict[str, Any]) -> None:
         _log.debug('Voice websocket frame received: %s', msg)
@@ -986,15 +987,19 @@
             return float('inf')
 
         return sum(heartbeat.recent_ack_latencies) / len(heartbeat.recent_ack_latencies)
 
     async def load_secret_key(self, data: Dict[str, Any]) -> None:
         _log.debug('received secret key for voice connection')
         self.secret_key = self._connection.secret_key = data['secret_key']
-        await self.speak()
+
+        # Send a speak command with the "not speaking" state.
+        # This also tells Discord our SSRC value, which Discord requires
+        # before sending any voice data (and is the real reason why we
+        # call this here).
         await self.speak(SpeakingState.none)
 
     async def poll_event(self) -> None:
         # This exception is handled up the chain
         msg = await asyncio.wait_for(self.ws.receive(), timeout=30.0)
         if msg.type is aiohttp.WSMsgType.TEXT:
             await self.received_message(utils._from_json(msg.data))
```

### Comparing `discord.py-2.2.3/discord/guild.py` & `discord.py-2.3.0/discord/guild.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     VerificationLevel,
     ContentFilter,
     NotificationLevel,
     NSFWLevel,
     MFALevel,
     Locale,
     AutoModRuleEventType,
+    ForumOrderType,
+    ForumLayoutType,
 )
 from .mixins import Hashable
 from .user import User
 from .invite import Invite
 from .widget import Widget
 from .asset import Asset
 from .flags import SystemChannelFlags
@@ -86,14 +88,15 @@
 from .threads import Thread, ThreadMember
 from .sticker import GuildSticker
 from .file import File
 from .audit_logs import AuditLogEntry
 from .object import OLDEST_OBJECT, Object
 from .welcome_screen import WelcomeScreen, WelcomeChannel
 from .automod import AutoModRule, AutoModTrigger, AutoModRuleAction
+from .partial_emoji import _EmojiTag, PartialEmoji
 
 
 __all__ = (
     'Guild',
     'BanEntry',
 )
 
@@ -125,14 +128,15 @@
         CategoryChannel as CategoryChannelPayload,
         StageChannel as StageChannelPayload,
         ForumChannel as ForumChannelPayload,
     )
     from .types.integration import IntegrationType
     from .types.snowflake import SnowflakeList
     from .types.widget import EditWidgetSettings
+    from .message import EmojiInputType
 
     VocalGuildChannel = Union[VoiceChannel, StageChannel]
     GuildChannel = Union[VocalGuildChannel, ForumChannel, TextChannel, CategoryChannel]
     ByCategoryItem = Tuple[Optional[CategoryChannel], List[GuildChannel]]
 
 
 class BanEntry(NamedTuple):
@@ -178,16 +182,14 @@
         All emojis that the guild owns.
     stickers: Tuple[:class:`GuildSticker`, ...]
         All stickers that the guild owns.
 
         .. versionadded:: 2.0
     afk_timeout: :class:`int`
         The number of seconds until someone is moved to the AFK channel.
-    afk_channel: Optional[:class:`VoiceChannel`]
-        The channel that denotes the AFK channel. ``None`` if it doesn't exist.
     id: :class:`int`
         The guild's ID.
     owner_id: :class:`int`
         The guild owner's ID. Use :attr:`Guild.owner` instead.
     unavailable: :class:`bool`
         Indicates if the guild is unavailable. If this is ``True`` then the
         reliability of other attributes outside of :attr:`Guild.id` is slim and they might
@@ -242,36 +244,39 @@
         The guild's Multi-Factor Authentication requirement level.
 
         .. versionchanged:: 2.0
             This field is now an enum instead of an :class:`int`.
 
     approximate_member_count: Optional[:class:`int`]
         The approximate number of members in the guild. This is ``None`` unless the guild is obtained
-        using :meth:`Client.fetch_guild` with ``with_counts=True``.
+        using :meth:`Client.fetch_guild` or :meth:`Client.fetch_guilds` with ``with_counts=True``.
 
         .. versionadded:: 2.0
     approximate_presence_count: Optional[:class:`int`]
         The approximate number of members currently active in the guild.
         Offline members are excluded. This is ``None`` unless the guild is obtained using
-        :meth:`Client.fetch_guild` with ``with_counts=True``.
+        :meth:`Client.fetch_guild` or :meth:`Client.fetch_guilds` with ``with_counts=True``.
 
         .. versionchanged:: 2.0
     premium_progress_bar_enabled: :class:`bool`
         Indicates if the guild has premium AKA server boost level progress bar enabled.
 
         .. versionadded:: 2.0
     widget_enabled: :class:`bool`
         Indicates if the guild has widget enabled.
 
         .. versionadded:: 2.0
+    max_stage_video_users: Optional[:class:`int`]
+        The maximum amount of users in a stage video channel.
+
+        .. versionadded:: 2.3
     """
 
     __slots__ = (
         'afk_timeout',
-        'afk_channel',
         'name',
         'id',
         'unavailable',
         'owner_id',
         'emojis',
         'stickers',
         'features',
@@ -285,14 +290,16 @@
         'premium_tier',
         'premium_subscription_count',
         'preferred_locale',
         'nsfw_level',
         'mfa_level',
         'vanity_url_code',
         'widget_enabled',
+        '_widget_channel_id',
+        '_afk_channel_id',
         '_members',
         '_channels',
         '_icon',
         '_banner',
         '_state',
         '_roles',
         '_member_count',
@@ -306,20 +313,22 @@
         '_public_updates_channel_id',
         '_stage_instances',
         '_scheduled_events',
         '_threads',
         'approximate_member_count',
         'approximate_presence_count',
         'premium_progress_bar_enabled',
+        '_safety_alerts_channel_id',
+        'max_stage_video_users',
     )
 
     _PREMIUM_GUILD_LIMITS: ClassVar[Dict[Optional[int], _GuildLimit]] = {
-        None: _GuildLimit(emoji=50, stickers=5, bitrate=96e3, filesize=8388608),
-        0: _GuildLimit(emoji=50, stickers=5, bitrate=96e3, filesize=8388608),
-        1: _GuildLimit(emoji=100, stickers=15, bitrate=128e3, filesize=8388608),
+        None: _GuildLimit(emoji=50, stickers=5, bitrate=96e3, filesize=utils.DEFAULT_FILE_SIZE_LIMIT_BYTES),
+        0: _GuildLimit(emoji=50, stickers=5, bitrate=96e3, filesize=utils.DEFAULT_FILE_SIZE_LIMIT_BYTES),
+        1: _GuildLimit(emoji=100, stickers=15, bitrate=128e3, filesize=utils.DEFAULT_FILE_SIZE_LIMIT_BYTES),
         2: _GuildLimit(emoji=150, stickers=30, bitrate=256e3, filesize=52428800),
         3: _GuildLimit(emoji=250, stickers=60, bitrate=384e3, filesize=104857600),
     }
 
     def __init__(self, *, data: GuildPayload, state: ConnectionState) -> None:
         self._channels: Dict[int, GuildChannel] = {}
         self._members: Dict[int, Member] = {}
@@ -469,79 +478,72 @@
         self.features: List[GuildFeature] = guild.get('features', [])
         self._splash: Optional[str] = guild.get('splash')
         self._system_channel_id: Optional[int] = utils._get_as_snowflake(guild, 'system_channel_id')
         self.description: Optional[str] = guild.get('description')
         self.max_presences: Optional[int] = guild.get('max_presences')
         self.max_members: Optional[int] = guild.get('max_members')
         self.max_video_channel_users: Optional[int] = guild.get('max_video_channel_users')
+        self.max_stage_video_users: Optional[int] = guild.get('max_stage_video_channel_users')
         self.premium_tier: int = guild.get('premium_tier', 0)
         self.premium_subscription_count: int = guild.get('premium_subscription_count') or 0
         self.vanity_url_code: Optional[str] = guild.get('vanity_url_code')
         self.widget_enabled: bool = guild.get('widget_enabled', False)
+        self._widget_channel_id: Optional[int] = utils._get_as_snowflake(guild, 'widget_channel_id')
         self._system_channel_flags: int = guild.get('system_channel_flags', 0)
         self.preferred_locale: Locale = try_enum(Locale, guild.get('preferred_locale', 'en-US'))
         self._discovery_splash: Optional[str] = guild.get('discovery_splash')
         self._rules_channel_id: Optional[int] = utils._get_as_snowflake(guild, 'rules_channel_id')
         self._public_updates_channel_id: Optional[int] = utils._get_as_snowflake(guild, 'public_updates_channel_id')
+        self._safety_alerts_channel_id: Optional[int] = utils._get_as_snowflake(guild, 'safety_alerts_channel_id')
         self.nsfw_level: NSFWLevel = try_enum(NSFWLevel, guild.get('nsfw_level', 0))
         self.mfa_level: MFALevel = try_enum(MFALevel, guild.get('mfa_level', 0))
         self.approximate_presence_count: Optional[int] = guild.get('approximate_presence_count')
         self.approximate_member_count: Optional[int] = guild.get('approximate_member_count')
         self.premium_progress_bar_enabled: bool = guild.get('premium_progress_bar_enabled', False)
         self.owner_id: Optional[int] = utils._get_as_snowflake(guild, 'owner_id')
-
-        self._sync(guild)
         self._large: Optional[bool] = None if self._member_count is None else self._member_count >= 250
+        self._afk_channel_id: Optional[int] = utils._get_as_snowflake(guild, 'afk_channel_id')
 
-        self.afk_channel: Optional[VocalGuildChannel] = self.get_channel(utils._get_as_snowflake(guild, 'afk_channel_id'))  # type: ignore
-
-    # TODO: refactor/remove?
-    def _sync(self, data: GuildPayload) -> None:
-        try:
-            self._large = data['large']
-        except KeyError:
-            pass
-
-        if 'channels' in data:
-            channels = data['channels']
+        if 'channels' in guild:
+            channels = guild['channels']
             for c in channels:
                 factory, ch_type = _guild_channel_factory(c['type'])
                 if factory:
                     self._add_channel(factory(guild=self, data=c, state=self._state))  # type: ignore
 
-        for obj in data.get('voice_states', []):
+        for obj in guild.get('voice_states', []):
             self._update_voice_state(obj, int(obj['channel_id']))
 
         cache_joined = self._state.member_cache_flags.joined
         cache_voice = self._state.member_cache_flags.voice
         self_id = self._state.self_id
-        for mdata in data.get('members', []):
+        for mdata in guild.get('members', []):
             member = Member(data=mdata, guild=self, state=self._state)  # type: ignore # Members will have the 'user' key in this scenario
             if cache_joined or member.id == self_id or (cache_voice and member.id in self._voice_states):
                 self._add_member(member)
 
         empty_tuple = ()
-        for presence in data.get('presences', []):
+        for presence in guild.get('presences', []):
             user_id = int(presence['user']['id'])
             member = self.get_member(user_id)
             if member is not None:
                 member._presence_update(presence, empty_tuple)  # type: ignore
 
-        if 'threads' in data:
-            threads = data['threads']
+        if 'threads' in guild:
+            threads = guild['threads']
             for thread in threads:
                 self._add_thread(Thread(guild=self, state=self._state, data=thread))
 
-        if 'stage_instances' in data:
-            for s in data['stage_instances']:
+        if 'stage_instances' in guild:
+            for s in guild['stage_instances']:
                 stage_instance = StageInstance(guild=self, data=s, state=self._state)
                 self._stage_instances[stage_instance.id] = stage_instance
 
-        if 'guild_scheduled_events' in data:
-            for s in data['guild_scheduled_events']:
+        if 'guild_scheduled_events' in guild:
+            for s in guild['guild_scheduled_events']:
                 scheduled_event = ScheduledEvent(data=s, state=self._state)
                 self._scheduled_events[scheduled_event.id] = scheduled_event
 
     @property
     def channels(self) -> Sequence[GuildChannel]:
         """Sequence[:class:`abc.GuildChannel`]: A list of channels that belongs to this guild."""
         return utils.SequenceProxy(self._channels.values())
@@ -732,14 +734,42 @@
         Returns
         --------
         Optional[:class:`Thread`]
             The returned thread or ``None`` if not found.
         """
         return self._threads.get(thread_id)
 
+    def get_emoji(self, emoji_id: int, /) -> Optional[Emoji]:
+        """Returns an emoji with the given ID.
+
+        .. versionadded:: 2.3
+
+        Parameters
+        ----------
+        emoji_id: int
+            The ID to search for.
+
+        Returns
+        --------
+        Optional[:class:`Emoji`]
+            The returned Emoji or ``None`` if not found.
+        """
+        emoji = self._state.get_emoji(emoji_id)
+        if emoji and emoji.guild == self:
+            return emoji
+        return None
+
+    @property
+    def afk_channel(self) -> Optional[VocalGuildChannel]:
+        """Optional[Union[:class:`VoiceChannel`, :class:`StageChannel`]]: The channel that denotes the AFK channel.
+
+        If no channel is set, then this returns ``None``.
+        """
+        return self.get_channel(self._afk_channel_id)  # type: ignore
+
     @property
     def system_channel(self) -> Optional[TextChannel]:
         """Optional[:class:`TextChannel`]: Returns the guild's channel used for system messages.
 
         If no channel is set, then this returns ``None``.
         """
         channel_id = self._system_channel_id
@@ -772,14 +802,37 @@
 
         .. versionadded:: 1.4
         """
         channel_id = self._public_updates_channel_id
         return channel_id and self._channels.get(channel_id)  # type: ignore
 
     @property
+    def safety_alerts_channel(self) -> Optional[TextChannel]:
+        """Optional[:class:`TextChannel`]: Return's the guild's channel used for safety alerts, if set.
+
+        For example, this is used for the raid protection setting. The guild must have the ``COMMUNITY`` feature.
+
+        .. versionadded:: 2.3
+        """
+        channel_id = self._safety_alerts_channel_id
+        return channel_id and self._channels.get(channel_id)  # type: ignore
+
+    @property
+    def widget_channel(self) -> Optional[Union[TextChannel, ForumChannel, VoiceChannel, StageChannel]]:
+        """Optional[Union[:class:`TextChannel`, :class:`ForumChannel`, :class:`VoiceChannel`, :class:`StageChannel`]]: Returns
+        the widget channel of the guild.
+
+        If no channel is set, then this returns ``None``.
+
+        .. versionadded:: 2.3
+        """
+        channel_id = self._widget_channel_id
+        return channel_id and self._channels.get(channel_id)  # type: ignore
+
+    @property
     def emoji_limit(self) -> int:
         """:class:`int`: The maximum number of emoji slots this guild has."""
         more_emoji = 200 if 'MORE_EMOJI' in self.features else 50
         return max(more_emoji, self._PREMIUM_GUILD_LIMITS[self.premium_tier].emoji)
 
     @property
     def sticker_limit(self) -> int:
@@ -1014,58 +1067,52 @@
     def created_at(self) -> datetime.datetime:
         """:class:`datetime.datetime`: Returns the guild's creation time in UTC."""
         return utils.snowflake_time(self.id)
 
     def get_member_named(self, name: str, /) -> Optional[Member]:
         """Returns the first member found that matches the name provided.
 
-        The name can have an optional discriminator argument, e.g. "Jake#0001"
-        or "Jake" will both do the lookup. However the former will give a more
-        precise result. Note that the discriminator must have all 4 digits
-        for this to work.
-
-        If a nickname is passed, then it is looked up via the nickname. Note
-        however, that a nickname + discriminator combo will not lookup the nickname
-        but rather the username + discriminator combo due to nickname + discriminator
-        not being unique.
+        The name is looked up in the following order:
+
+        - Username#Discriminator (deprecated)
+        - Username#0 (deprecated, only gets users that migrated from their discriminator)
+        - Nickname
+        - Global name
+        - Username
 
         If no member is found, ``None`` is returned.
 
         .. versionchanged:: 2.0
 
             ``name`` parameter is now positional-only.
 
+        .. deprecated:: 2.3
+
+            Looking up users via discriminator due to Discord API change.
+
         Parameters
         -----------
         name: :class:`str`
-            The name of the member to lookup with an optional discriminator.
+            The name of the member to lookup.
 
         Returns
         --------
         Optional[:class:`Member`]
             The member in this guild with the associated name. If not found
             then ``None`` is returned.
         """
 
-        result = None
         members = self.members
-        if len(name) > 5 and name[-5] == '#':
-            # The 5 length is checking to see if #0000 is in the string,
-            # as a#0000 has a length of 6, the minimum for a potential
-            # discriminator lookup.
-            potential_discriminator = name[-4:]
-
-            # do the actual lookup and return if found
-            # if it isn't found then we'll do a full name lookup below.
-            result = utils.get(members, name=name[:-5], discriminator=potential_discriminator)
-            if result is not None:
-                return result
+
+        username, _, discriminator = name.rpartition('#')
+        if discriminator == '0' or (len(discriminator) == 4 and discriminator.isdigit()):
+            return utils.find(lambda m: m.name == username and m.discriminator == discriminator, members)
 
         def pred(m: Member) -> bool:
-            return m.nick == name or m.name == name
+            return m.nick == name or m.global_name == name or m.name == name
 
         return utils.find(pred, members)
 
     @overload
     def _create_channel(
         self,
         name: str,
@@ -1195,14 +1242,15 @@
         news: bool = False,
         position: int = MISSING,
         topic: str = MISSING,
         slowmode_delay: int = MISSING,
         nsfw: bool = MISSING,
         overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = MISSING,
         default_auto_archive_duration: int = MISSING,
+        default_thread_slowmode_delay: int = MISSING,
     ) -> TextChannel:
         """|coro|
 
         Creates a :class:`TextChannel` for the guild.
 
         Note that you must have :attr:`~Permissions.manage_channels` to create the channel.
 
@@ -1260,22 +1308,26 @@
             The new channel's topic.
         slowmode_delay: :class:`int`
             Specifies the slowmode rate limit for user in this channel, in seconds.
             The maximum value possible is ``21600``.
         nsfw: :class:`bool`
             To mark the channel as NSFW or not.
         news: :class:`bool`
-             Whether to create the text channel as a news channel.
+            Whether to create the text channel as a news channel.
 
             .. versionadded:: 2.0
         default_auto_archive_duration: :class:`int`
             The default auto archive duration for threads created in the text channel (in minutes).
             Must be one of ``60``, ``1440``, ``4320``, or ``10080``.
 
             .. versionadded:: 2.0
+        default_thread_slowmode_delay: :class:`int`
+            The default slowmode delay in seconds for threads created in the text channel.
+
+            .. versionadded:: 2.3
         reason: Optional[:class:`str`]
             The reason for creating this channel. Shows up on the audit log.
 
         Raises
         -------
         Forbidden
             You do not have the proper permissions to create this channel.
@@ -1300,15 +1352,18 @@
         if slowmode_delay is not MISSING:
             options['rate_limit_per_user'] = slowmode_delay
 
         if nsfw is not MISSING:
             options['nsfw'] = nsfw
 
         if default_auto_archive_duration is not MISSING:
-            options["default_auto_archive_duration"] = default_auto_archive_duration
+            options['default_auto_archive_duration'] = default_auto_archive_duration
+
+        if default_thread_slowmode_delay is not MISSING:
+            options['default_thread_rate_limit_per_user'] = default_thread_slowmode_delay
 
         data = await self._create_channel(
             name,
             overwrites=overwrites,
             channel_type=ChannelType.news if news else ChannelType.text,
             category=category,
             reason=reason,
@@ -1572,14 +1627,17 @@
         category: Optional[CategoryChannel] = None,
         slowmode_delay: int = MISSING,
         nsfw: bool = MISSING,
         overwrites: Mapping[Union[Role, Member], PermissionOverwrite] = MISSING,
         reason: Optional[str] = None,
         default_auto_archive_duration: int = MISSING,
         default_thread_slowmode_delay: int = MISSING,
+        default_sort_order: ForumOrderType = MISSING,
+        default_reaction_emoji: EmojiInputType = MISSING,
+        default_layout: ForumLayoutType = MISSING,
         available_tags: Sequence[ForumTag] = MISSING,
     ) -> ForumChannel:
         """|coro|
 
         Similar to :meth:`create_text_channel` except makes a :class:`ForumChannel` instead.
 
         The ``overwrites`` parameter can be used to create a 'secret'
@@ -1616,14 +1674,27 @@
         default_auto_archive_duration: :class:`int`
             The default auto archive duration for threads created in the forum channel (in minutes).
             Must be one of ``60``, ``1440``, ``4320``, or ``10080``.
         default_thread_slowmode_delay: :class:`int`
             The default slowmode delay in seconds for threads created in this forum.
 
             .. versionadded:: 2.1
+        default_sort_order: :class:`ForumOrderType`
+            The default sort order for posts in this forum channel.
+
+            .. versionadded:: 2.3
+        default_reaction_emoji: Union[:class:`Emoji`, :class:`PartialEmoji`, :class:`str`]
+            The default reaction emoji for threads created in this forum to show in the
+            add reaction button.
+
+            .. versionadded:: 2.3
+        default_layout: :class:`ForumLayoutType`
+            The default layout for posts in this forum.
+
+            .. versionadded:: 2.3
         available_tags: Sequence[:class:`ForumTag`]
             The available tags for this forum channel.
 
             .. versionadded:: 2.1
 
         Raises
         -------
@@ -1655,14 +1726,38 @@
 
         if default_auto_archive_duration is not MISSING:
             options['default_auto_archive_duration'] = default_auto_archive_duration
 
         if default_thread_slowmode_delay is not MISSING:
             options['default_thread_rate_limit_per_user'] = default_thread_slowmode_delay
 
+        if default_sort_order is not MISSING:
+            if not isinstance(default_sort_order, ForumOrderType):
+                raise TypeError(
+                    f'default_sort_order parameter must be a ForumOrderType not {default_sort_order.__class__.__name__}'
+                )
+
+            options['default_sort_order'] = default_sort_order.value
+
+        if default_reaction_emoji is not MISSING:
+            if isinstance(default_reaction_emoji, _EmojiTag):
+                options['default_reaction_emoji'] = default_reaction_emoji._to_partial()._to_forum_tag_payload()
+            elif isinstance(default_reaction_emoji, str):
+                options['default_reaction_emoji'] = PartialEmoji.from_str(default_reaction_emoji)._to_forum_tag_payload()
+            else:
+                raise ValueError(f'default_reaction_emoji parameter must be either Emoji, PartialEmoji, or str')
+
+        if default_layout is not MISSING:
+            if not isinstance(default_layout, ForumLayoutType):
+                raise TypeError(
+                    f'default_layout parameter must be a ForumLayoutType not {default_layout.__class__.__name__}'
+                )
+
+            options['default_forum_layout'] = default_layout.value
+
         if available_tags is not MISSING:
             options['available_tags'] = [t.to_dict() for t in available_tags]
 
         data = await self._create_channel(
             name=name, overwrites=overwrites, channel_type=ChannelType.forum, category=category, reason=reason, **options
         )
 
@@ -1727,46 +1822,36 @@
         system_channel_flags: SystemChannelFlags = MISSING,
         preferred_locale: Locale = MISSING,
         rules_channel: Optional[TextChannel] = MISSING,
         public_updates_channel: Optional[TextChannel] = MISSING,
         premium_progress_bar_enabled: bool = MISSING,
         discoverable: bool = MISSING,
         invites_disabled: bool = MISSING,
+        widget_enabled: bool = MISSING,
+        widget_channel: Optional[Snowflake] = MISSING,
+        mfa_level: MFALevel = MISSING,
+        raid_alerts_disabled: bool = MISSING,
+        safety_alerts_channel: TextChannel = MISSING,
     ) -> Guild:
         r"""|coro|
 
         Edits the guild.
 
         You must have :attr:`~Permissions.manage_guild` to edit the guild.
 
-        .. versionchanged:: 1.4
-            The ``rules_channel`` and ``public_updates_channel`` keyword parameters were added.
-
-        .. versionchanged:: 2.0
-            The ``discovery_splash`` and ``community`` keyword parameters were added.
-
         .. versionchanged:: 2.0
             The newly updated guild is returned.
 
         .. versionchanged:: 2.0
             The ``region`` keyword parameter has been removed.
 
         .. versionchanged:: 2.0
             This function will now raise :exc:`TypeError` or
             :exc:`ValueError` instead of ``InvalidArgument``.
 
-        .. versionchanged:: 2.0
-            The ``preferred_locale`` keyword parameter now accepts an enum instead of :class:`str`.
-
-        .. versionchanged:: 2.0
-            The ``premium_progress_bar_enabled`` keyword parameter was added.
-
-        .. versionchanged:: 2.1
-            The ``discoverable`` and ``invites_disabled`` keyword parameters were added.
-
         Parameters
         ----------
         name: :class:`str`
             The new name of the guild.
         description: Optional[:class:`str`]
             The new description of the guild. Could be ``None`` for no description.
             This is only available to guilds that contain ``COMMUNITY`` in :attr:`Guild.features`.
@@ -1784,17 +1869,21 @@
             splash. This is only available to guilds that contain ``INVITE_SPLASH``
             in :attr:`Guild.features`.
         discovery_splash: :class:`bytes`
             A :term:`py:bytes-like object` representing the discovery splash.
             Only PNG/JPEG supported. Could be ``None`` to denote removing the
             splash. This is only available to guilds that contain ``DISCOVERABLE``
             in :attr:`Guild.features`.
+
+            .. versionadded:: 2.0
         community: :class:`bool`
             Whether the guild should be a Community guild. If set to ``True``\, both ``rules_channel``
             and ``public_updates_channel`` parameters are required.
+
+            .. versionadded:: 2.0
         afk_channel: Optional[:class:`VoiceChannel`]
             The new channel that is the AFK channel. Could be ``None`` for no AFK channel.
         afk_timeout: :class:`int`
             The number of seconds until someone is moved to the AFK channel.
         owner: :class:`Member`
             The new owner of the guild to transfer ownership to. Note that you must
             be owner of the guild to do this.
@@ -1808,45 +1897,84 @@
             The new vanity code for the guild.
         system_channel: Optional[:class:`TextChannel`]
             The new channel that is used for the system channel. Could be ``None`` for no system channel.
         system_channel_flags: :class:`SystemChannelFlags`
             The new system channel settings to use with the new system channel.
         preferred_locale: :class:`Locale`
             The new preferred locale for the guild. Used as the primary language in the guild.
+
+            .. versionchanged:: 2.0
+
+                Now accepts an enum instead of :class:`str`.
         rules_channel: Optional[:class:`TextChannel`]
             The new channel that is used for rules. This is only available to
             guilds that contain ``COMMUNITY`` in :attr:`Guild.features`. Could be ``None`` for no rules
             channel.
+
+            .. versionadded:: 1.4
         public_updates_channel: Optional[:class:`TextChannel`]
             The new channel that is used for public updates from Discord. This is only available to
             guilds that contain ``COMMUNITY`` in :attr:`Guild.features`. Could be ``None`` for no
             public updates channel.
+
+            .. versionadded:: 1.4
         premium_progress_bar_enabled: :class:`bool`
             Whether the premium AKA server boost level progress bar should be enabled for the guild.
+
+            .. versionadded:: 2.0
         discoverable: :class:`bool`
             Whether server discovery is enabled for this guild.
+
+            .. versionadded:: 2.1
         invites_disabled: :class:`bool`
             Whether joining via invites should be disabled for the guild.
+
+            .. versionadded:: 2.1
+        widget_enabled: :class:`bool`
+            Whether to enable the widget for the guild.
+
+            .. versionadded:: 2.3
+        widget_channel: Optional[:class:`abc.Snowflake`]
+             The new widget channel. ``None`` removes the widget channel.
+
+            .. versionadded:: 2.3
+        mfa_level: :class:`MFALevel`
+            The new guild's Multi-Factor Authentication requirement level.
+            Note that you must be owner of the guild to do this.
+
+            .. versionadded:: 2.3
         reason: Optional[:class:`str`]
             The reason for editing this guild. Shows up on the audit log.
 
+        raid_alerts_disabled: :class:`bool`
+            Whether the alerts for raid protection should be disabled for the guild.
+
+            .. versionadded:: 2.3
+
+        safety_alerts_channel: Optional[:class:`TextChannel`]
+            The new channel that is used for safety alerts. This is only available to
+            guilds that contain ``COMMUNITY`` in :attr:`Guild.features`. Could be ``None`` for no
+            safety alerts channel.
+
+            .. versionadded:: 2.3
+
         Raises
         -------
         Forbidden
             You do not have permissions to edit the guild.
         HTTPException
             Editing the guild failed.
         ValueError
             The image format passed in to ``icon`` is invalid. It must be
             PNG or JPG. This is also raised if you are not the owner of the
             guild and request an ownership transfer.
         TypeError
-            The type passed to the ``default_notifications``, ``verification_level``,
-            ``explicit_content_filter``, or ``system_channel_flags`` parameter was
-            of the incorrect type.
+            The type passed to the ``default_notifications``, ``rules_channel``, ``public_updates_channel``,
+            ``safety_alerts_channel`` ``verification_level``, ``explicit_content_filter``,
+            ``system_channel_flags``, or ``mfa_level`` parameter was of the incorrect type.
 
         Returns
         --------
         :class:`Guild`
             The newly updated guild. Note that this has the same limitations as
             mentioned in :meth:`Client.fetch_guild` and may not have full data.
         """
@@ -1910,22 +2038,41 @@
             else:
                 fields['system_channel_id'] = system_channel.id
 
         if rules_channel is not MISSING:
             if rules_channel is None:
                 fields['rules_channel_id'] = rules_channel
             else:
+                if not isinstance(rules_channel, TextChannel):
+                    raise TypeError(f'rules_channel must be of type TextChannel not {rules_channel.__class__.__name__}')
+
                 fields['rules_channel_id'] = rules_channel.id
 
         if public_updates_channel is not MISSING:
             if public_updates_channel is None:
                 fields['public_updates_channel_id'] = public_updates_channel
             else:
+                if not isinstance(public_updates_channel, TextChannel):
+                    raise TypeError(
+                        f'public_updates_channel must be of type TextChannel not {public_updates_channel.__class__.__name__}'
+                    )
+
                 fields['public_updates_channel_id'] = public_updates_channel.id
 
+        if safety_alerts_channel is not MISSING:
+            if safety_alerts_channel is None:
+                fields['safety_alerts_channel_id'] = safety_alerts_channel
+            else:
+                if not isinstance(safety_alerts_channel, TextChannel):
+                    raise TypeError(
+                        f'safety_alerts_channel must be of type TextChannel not {safety_alerts_channel.__class__.__name__}'
+                    )
+
+            fields['safety_alerts_channel_id'] = safety_alerts_channel.id
+
         if owner is not MISSING:
             if self.owner_id != self._state.self_id:
                 raise ValueError('To transfer ownership you must be the owner of the guild.')
 
             fields['owner_id'] = owner.id
 
         if verification_level is not MISSING:
@@ -1942,15 +2089,15 @@
 
         if system_channel_flags is not MISSING:
             if not isinstance(system_channel_flags, SystemChannelFlags):
                 raise TypeError('system_channel_flags field must be of type SystemChannelFlags')
 
             fields['system_channel_flags'] = system_channel_flags.value
 
-        if any(feat is not MISSING for feat in (community, discoverable, invites_disabled)):
+        if any(feat is not MISSING for feat in (community, discoverable, invites_disabled, raid_alerts_disabled)):
             features = set(self.features)
 
             if community is not MISSING:
                 if community:
                     if 'rules_channel_id' in fields and 'public_updates_channel_id' in fields:
                         features.add('COMMUNITY')
                     else:
@@ -1968,19 +2115,40 @@
 
             if invites_disabled is not MISSING:
                 if invites_disabled:
                     features.add('INVITES_DISABLED')
                 else:
                     features.discard('INVITES_DISABLED')
 
+            if raid_alerts_disabled is not MISSING:
+                if raid_alerts_disabled:
+                    features.add('RAID_ALERTS_DISABLED')
+                else:
+                    features.discard('RAID_ALERTS_DISABLED')
+
             fields['features'] = list(features)
 
         if premium_progress_bar_enabled is not MISSING:
             fields['premium_progress_bar_enabled'] = premium_progress_bar_enabled
 
+        widget_payload: EditWidgetSettings = {}
+        if widget_channel is not MISSING:
+            widget_payload['channel_id'] = None if widget_channel is None else widget_channel.id
+        if widget_enabled is not MISSING:
+            widget_payload['enabled'] = widget_enabled
+
+        if widget_payload:
+            await self._state.http.edit_widget(self.id, payload=widget_payload, reason=reason)
+
+        if mfa_level is not MISSING:
+            if not isinstance(mfa_level, MFALevel):
+                raise TypeError(f'mfa_level must be of type MFALevel not {mfa_level.__class__.__name__}')
+
+            await http.edit_guild_mfa_level(self.id, mfa_level=mfa_level.value)
+
         data = await http.edit_guild(self.id, reason=reason, **fields)
         return Guild(data=data, state=self._state)
 
     async def fetch_channels(self) -> Sequence[GuildChannel]:
         """|coro|
 
         Retrieves all :class:`abc.GuildChannel` that the guild has.
@@ -2803,14 +2971,76 @@
         --------
         :class:`ScheduledEvent`
             The scheduled event.
         """
         data = await self._state.http.get_scheduled_event(self.id, scheduled_event_id, with_counts)
         return ScheduledEvent(state=self._state, data=data)
 
+    @overload
+    async def create_scheduled_event(
+        self,
+        *,
+        name: str,
+        start_time: datetime.datetime,
+        entity_type: Literal[EntityType.external] = ...,
+        privacy_level: PrivacyLevel = ...,
+        location: str = ...,
+        end_time: datetime.datetime = ...,
+        description: str = ...,
+        image: bytes = ...,
+        reason: Optional[str] = ...,
+    ) -> ScheduledEvent:
+        ...
+
+    @overload
+    async def create_scheduled_event(
+        self,
+        *,
+        name: str,
+        start_time: datetime.datetime,
+        entity_type: Literal[EntityType.stage_instance, EntityType.voice] = ...,
+        privacy_level: PrivacyLevel = ...,
+        channel: Snowflake = ...,
+        end_time: datetime.datetime = ...,
+        description: str = ...,
+        image: bytes = ...,
+        reason: Optional[str] = ...,
+    ) -> ScheduledEvent:
+        ...
+
+    @overload
+    async def create_scheduled_event(
+        self,
+        *,
+        name: str,
+        start_time: datetime.datetime,
+        privacy_level: PrivacyLevel = ...,
+        location: str = ...,
+        end_time: datetime.datetime = ...,
+        description: str = ...,
+        image: bytes = ...,
+        reason: Optional[str] = ...,
+    ) -> ScheduledEvent:
+        ...
+
+    @overload
+    async def create_scheduled_event(
+        self,
+        *,
+        name: str,
+        start_time: datetime.datetime,
+        privacy_level: PrivacyLevel = ...,
+        channel: Union[VoiceChannel, StageChannel] = ...,
+        end_time: datetime.datetime = ...,
+        description: str = ...,
+        image: bytes = ...,
+        reason: Optional[str] = ...,
+    ) -> ScheduledEvent:
+        ...
+
     async def create_scheduled_event(
         self,
         *,
         name: str,
         start_time: datetime.datetime,
         entity_type: EntityType = MISSING,
         privacy_level: PrivacyLevel = MISSING,
@@ -2895,45 +3125,50 @@
         if start_time is not MISSING:
             if start_time.tzinfo is None:
                 raise ValueError(
                     'start_time must be an aware datetime. Consider using discord.utils.utcnow() or datetime.datetime.now().astimezone() for local time.'
                 )
             payload['scheduled_start_time'] = start_time.isoformat()
 
+        entity_type = entity_type or getattr(channel, '_scheduled_event_entity_type', MISSING)
         if entity_type is MISSING:
-            if channel is MISSING:
+            if channel and isinstance(channel, Object):
+                if channel.type is VoiceChannel:
+                    entity_type = EntityType.voice
+                elif channel.type is StageChannel:
+                    entity_type = EntityType.stage_instance
+
+            elif location not in (MISSING, None):
                 entity_type = EntityType.external
-            else:
-                _entity_type = getattr(channel, '_scheduled_event_entity_type', MISSING)
-                if _entity_type is None:
-                    raise TypeError(
-                        'invalid GuildChannel type passed, must be VoiceChannel or StageChannel '
-                        f'not {channel.__class__.__name__}'
-                    )
-                if _entity_type is MISSING:
-                    raise TypeError('entity_type must be passed in when passing an ambiguous channel type')
+        else:
+            if not isinstance(entity_type, EntityType):
+                raise TypeError('entity_type must be of type EntityType')
 
-                entity_type = _entity_type
+            payload['entity_type'] = entity_type.value
 
-        if not isinstance(entity_type, EntityType):
-            raise TypeError('entity_type must be of type EntityType')
+        if entity_type is None:
+            raise TypeError(
+                'invalid GuildChannel type passed, must be VoiceChannel or StageChannel ' f'not {channel.__class__.__name__}'
+            )
 
-        payload['entity_type'] = entity_type.value
+        if privacy_level is not MISSING:
+            if not isinstance(privacy_level, PrivacyLevel):
+                raise TypeError('privacy_level must be of type PrivacyLevel.')
 
-        payload['privacy_level'] = PrivacyLevel.guild_only.value
+            payload['privacy_level'] = privacy_level.value
 
         if description is not MISSING:
             payload['description'] = description
 
         if image is not MISSING:
             image_as_str: str = utils._bytes_to_base64_data(image)
             payload['image'] = image_as_str
 
         if entity_type in (EntityType.stage_instance, EntityType.voice):
-            if channel is MISSING or channel is None:
+            if channel in (MISSING, None):
                 raise TypeError('channel must be set when entity_type is voice or stage_instance')
 
             payload['channel_id'] = channel.id
 
             if location is not MISSING:
                 raise TypeError('location cannot be set when entity_type is voice or stage_instance')
         else:
@@ -2941,20 +3176,23 @@
                 raise TypeError('channel cannot be set when entity_type is external')
 
             if location is MISSING or location is None:
                 raise TypeError('location must be set when entity_type is external')
 
             metadata['location'] = location
 
-            if end_time is not MISSING:
-                if end_time.tzinfo is None:
-                    raise ValueError(
-                        'end_time must be an aware datetime. Consider using discord.utils.utcnow() or datetime.datetime.now().astimezone() for local time.'
-                    )
-                payload['scheduled_end_time'] = end_time.isoformat()
+            if end_time in (MISSING, None):
+                raise TypeError('end_time must be set when entity_type is external')
+
+        if end_time not in (MISSING, None):
+            if end_time.tzinfo is None:
+                raise ValueError(
+                    'end_time must be an aware datetime. Consider using discord.utils.utcnow() or datetime.datetime.now().astimezone() for local time.'
+                )
+            payload['scheduled_end_time'] = end_time.isoformat()
 
         if metadata:
             payload['entity_metadata'] = metadata
 
         data = await self._state.http.create_guild_scheduled_event(self.id, **payload, reason=reason)
         return ScheduledEvent(state=self._state, data=data)
 
@@ -3238,15 +3476,14 @@
 
         if name is not MISSING:
             fields['name'] = name
 
         data = await self._state.http.create_role(self.id, reason=reason, **fields)
         role = Role(guild=self, data=data, state=self._state)
 
-        # TODO: add to cache
         return role
 
     async def edit_role_positions(self, positions: Mapping[Snowflake, int], *, reason: Optional[str] = None) -> List[Role]:
         """|coro|
 
         Bulk edits a list of :class:`Role` in the guild.
 
@@ -3666,14 +3903,15 @@
         else:
             strategy, state = _before_strategy, before
             if after:
                 predicate = lambda m: int(m['id']) > after.id
 
         # avoid circular import
         from .app_commands import AppCommand
+        from .webhook import Webhook
 
         while True:
             retrieve = 100 if limit is None else min(limit, 100)
             if retrieve < 1:
                 return
 
             data, raw_entries, state, limit = await strategy(retrieve, state, limit)
@@ -3692,27 +3930,31 @@
 
             automod_rules = (
                 AutoModRule(data=raw_rule, guild=self, state=self._state)
                 for raw_rule in data.get('auto_moderation_rules', [])
             )
             automod_rule_map = {rule.id: rule for rule in automod_rules}
 
+            webhooks = (Webhook.from_state(data=raw_webhook, state=self._state) for raw_webhook in data.get('webhooks', []))
+            webhook_map = {webhook.id: webhook for webhook in webhooks}
+
             count = 0
 
             for count, raw_entry in enumerate(raw_entries, 1):
                 # Weird Discord quirk
                 if raw_entry['action_type'] is None:
                     continue
 
                 yield AuditLogEntry(
                     data=raw_entry,
                     users=user_map,
                     integrations=integration_map,
                     app_commands=app_command_map,
                     automod_rules=automod_rule_map,
+                    webhooks=webhook_map,
                     guild=self,
                 )
 
             if count < 100:
                 # There's no data left after this
                 break
 
@@ -3746,15 +3988,15 @@
         *,
         enabled: bool = MISSING,
         channel: Optional[Snowflake] = MISSING,
         reason: Optional[str] = None,
     ) -> None:
         """|coro|
 
-        Edits the widget of the guild.
+        Edits the widget of the guild. This can also be done with :attr:`~Guild.edit`.
 
         You must have :attr:`~Permissions.manage_guild` to do this.
 
         .. versionadded:: 2.0
 
         Parameters
         -----------
@@ -3774,15 +4016,16 @@
         """
         payload: EditWidgetSettings = {}
         if channel is not MISSING:
             payload['channel_id'] = None if channel is None else channel.id
         if enabled is not MISSING:
             payload['enabled'] = enabled
 
-        await self._state.http.edit_widget(self.id, payload=payload, reason=reason)
+        if payload:
+            await self._state.http.edit_widget(self.id, payload=payload, reason=reason)
 
     async def chunk(self, *, cache: bool = True) -> List[Member]:
         """|coro|
 
         Requests all members that belong to this guild. In order to use this,
         :meth:`Intents.members` must be enabled.
 
@@ -3966,15 +4209,15 @@
     async def create_automod_rule(
         self,
         *,
         name: str,
         event_type: AutoModRuleEventType,
         trigger: AutoModTrigger,
         actions: List[AutoModRuleAction],
-        enabled: bool = MISSING,
+        enabled: bool = False,
         exempt_roles: Sequence[Snowflake] = MISSING,
         exempt_channels: Sequence[Snowflake] = MISSING,
         reason: str = MISSING,
     ) -> AutoModRule:
         """|coro|
 
         Create an automod rule.
@@ -3991,15 +4234,15 @@
             The type of event that the automod rule will trigger on.
         trigger: :class:`AutoModTrigger`
             The trigger that will trigger the automod rule.
         actions: List[:class:`AutoModRuleAction`]
             The actions that will be taken when the automod rule is triggered.
         enabled: :class:`bool`
             Whether the automod rule is enabled.
-            Discord will default to ``False``.
+            Defaults to ``False``.
         exempt_roles: Sequence[:class:`abc.Snowflake`]
             A list of roles that will be exempt from the automod rule.
         exempt_channels: Sequence[:class:`abc.Snowflake`]
             A list of channels that will be exempt from the automod rule.
         reason: :class:`str`
             The reason for creating this automod rule. Shows up on the audit log.
```

### Comparing `discord.py-2.2.3/discord/http.py` & `discord.py-2.3.0/discord/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     Type,
     TypeVar,
     Union,
 )
 from urllib.parse import quote as _uriquote
 from collections import deque
 import datetime
+import socket
 
 import aiohttp
 
 from .errors import HTTPException, RateLimited, Forbidden, NotFound, LoginFailure, DiscordServerError, GatewayNotFound
 from .gateway import DiscordClientWebSocketResponse
 from .file import File
 from .mentions import AllowedMentions
@@ -780,15 +781,16 @@
             await self.__session.close()
 
     # login management
 
     async def static_login(self, token: str) -> user.User:
         # Necessary to get aiohttp to stop complaining about session creation
         if self.connector is MISSING:
-            self.connector = aiohttp.TCPConnector(limit=0)
+            # discord does not support ipv6
+            self.connector = aiohttp.TCPConnector(limit=0, family=socket.AF_INET)
 
         self.__session = aiohttp.ClientSession(
             connector=self.connector,
             ws_response_class=DiscordClientWebSocketResponse,
             trace_configs=None if self.http_trace is None else [self.http_trace],
         )
         self._global_over = asyncio.Event()
@@ -1144,14 +1146,15 @@
             'default_auto_archive_duration',
             'flags',
             'default_thread_rate_limit_per_user',
             'default_reaction_emoji',
             'available_tags',
             'applied_tags',
             'default_forum_layout',
+            'default_sort_order',
         )
 
         payload = {k: v for k, v in options.items() if k in valid_keys}
         return self.request(r, reason=reason, json=payload)
 
     def bulk_channel_update(
         self,
@@ -1185,14 +1188,17 @@
             'position',
             'permission_overwrites',
             'rate_limit_per_user',
             'rtc_region',
             'video_quality_mode',
             'default_auto_archive_duration',
             'default_thread_rate_limit_per_user',
+            'default_sort_order',
+            'default_reaction_emoji',
+            'default_forum_layout',
             'available_tags',
         )
         payload.update({k: v for k, v in options.items() if k in valid_keys and v is not None})
 
         return self.request(Route('POST', '/guilds/{guild_id}/channels', guild_id=guild_id), json=payload, reason=reason)
 
     def delete_channel(
@@ -1365,17 +1371,19 @@
     # Guild management
 
     def get_guilds(
         self,
         limit: int,
         before: Optional[Snowflake] = None,
         after: Optional[Snowflake] = None,
+        with_counts: bool = True,
     ) -> Response[List[guild.Guild]]:
         params: Dict[str, Any] = {
             'limit': limit,
+            'with_counts': int(with_counts),
         }
 
         if before:
             params['before'] = before
         if after:
             params['after'] = after
 
@@ -1418,20 +1426,27 @@
             'explicit_content_filter',
             'banner',
             'system_channel_flags',
             'rules_channel_id',
             'public_updates_channel_id',
             'preferred_locale',
             'premium_progress_bar_enabled',
+            'safety_alerts_channel_id',
         )
 
         payload = {k: v for k, v in fields.items() if k in valid_keys}
 
         return self.request(Route('PATCH', '/guilds/{guild_id}', guild_id=guild_id), json=payload, reason=reason)
 
+    def edit_guild_mfa_level(
+        self, guild_id: Snowflake, *, mfa_level: int, reason: Optional[str] = None
+    ) -> Response[guild.GuildMFALevel]:
+        payload = {'level': mfa_level}
+        return self.request(Route('POST', '/guilds/{guild_id}/mfa', guild_id=guild_id), json=payload, reason=reason)
+
     def get_template(self, code: str) -> Response[template.Template]:
         return self.request(Route('GET', '/guilds/templates/{code}', code=code))
 
     def guild_templates(self, guild_id: Snowflake) -> Response[List[template.Template]]:
         return self.request(Route('GET', '/guilds/{guild_id}/templates', guild_id=guild_id))
 
     def create_template(self, guild_id: Snowflake, payload: Dict[str, Any]) -> Response[template.Template]:
@@ -1899,14 +1914,15 @@
         return self.request(Route('GET', '/stage-instances/{channel_id}', channel_id=channel_id))
 
     def create_stage_instance(self, *, reason: Optional[str], **payload: Any) -> Response[channel.StageInstance]:
         valid_keys = (
             'channel_id',
             'topic',
             'privacy_level',
+            'send_start_notification',
         )
         payload = {k: v for k, v in payload.items() if k in valid_keys}
 
         return self.request(Route('POST', '/stage-instances'), json=payload, reason=reason)
 
     def edit_stage_instance(self, channel_id: Snowflake, *, reason: Optional[str] = None, **payload: Any) -> Response[None]:
         valid_keys = (
```

### Comparing `discord.py-2.2.3/discord/integrations.py` & `discord.py-2.3.0/discord/integrations.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/interactions.py` & `discord.py-2.3.0/discord/interactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,33 +21,36 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
+
+import logging
 from typing import Any, Dict, Optional, Generic, TYPE_CHECKING, Sequence, Tuple, Union
 import asyncio
 import datetime
 
 from . import utils
 from .enums import try_enum, Locale, InteractionType, InteractionResponseType
 from .errors import InteractionResponded, HTTPException, ClientException, DiscordException
 from .flags import MessageFlags
-from .channel import PartialMessageable, ChannelType
+from .channel import ChannelType
 from ._types import ClientT
 
 from .user import User
 from .member import Member
 from .message import Message, Attachment
 from .permissions import Permissions
 from .http import handle_message_parameters
 from .webhook.async_ import async_context, Webhook, interaction_response_params, interaction_message_response_params
 from .app_commands.namespace import Namespace
 from .app_commands.translator import locale_str, TranslationContext, TranslationContextLocation
+from .channel import _threaded_channel_factory
 
 __all__ = (
     'Interaction',
     'InteractionMessage',
     'InteractionResponse',
 )
 
@@ -65,20 +68,27 @@
     from .file import File
     from .mentions import AllowedMentions
     from aiohttp import ClientSession
     from .embeds import Embed
     from .ui.view import View
     from .app_commands.models import Choice, ChoiceT
     from .ui.modal import Modal
-    from .channel import VoiceChannel, StageChannel, TextChannel, ForumChannel, CategoryChannel
+    from .channel import VoiceChannel, StageChannel, TextChannel, ForumChannel, CategoryChannel, DMChannel, GroupChannel
     from .threads import Thread
     from .app_commands.commands import Command, ContextMenu
 
     InteractionChannel = Union[
-        VoiceChannel, StageChannel, TextChannel, ForumChannel, CategoryChannel, Thread, PartialMessageable
+        VoiceChannel,
+        StageChannel,
+        TextChannel,
+        ForumChannel,
+        CategoryChannel,
+        Thread,
+        DMChannel,
+        GroupChannel,
     ]
 
 MISSING: Any = utils.MISSING
 
 
 class Interaction(Generic[ClientT]):
     """Represents a Discord interaction.
@@ -92,16 +102,18 @@
     -----------
     id: :class:`int`
         The interaction's ID.
     type: :class:`InteractionType`
         The interaction type.
     guild_id: Optional[:class:`int`]
         The guild ID the interaction was sent from.
-    channel_id: Optional[:class:`int`]
-        The channel ID the interaction was sent from.
+    channel: Optional[Union[:class:`abc.GuildChannel`, :class:`abc.PrivateChannel`, :class:`Thread`]]
+        The channel the interaction was sent from.
+
+        Note that due to a Discord limitation, if sent from a DM channel :attr:`~DMChannel.recipient` is ``None``.
     application_id: :class:`int`
         The application ID that the interaction was for.
     user: Union[:class:`User`, :class:`Member`]
         The user or member that sent the interaction.
     message: Optional[:class:`Message`]
         The message that sent this interaction.
 
@@ -124,15 +136,14 @@
         This includes checks and execution.
     """
 
     __slots__: Tuple[str, ...] = (
         'id',
         'type',
         'guild_id',
-        'channel_id',
         'data',
         'application_id',
         'message',
         'user',
         'token',
         'version',
         'locale',
@@ -144,15 +155,15 @@
         '_state',
         '_client',
         '_session',
         '_baton',
         '_original_response',
         '_cs_response',
         '_cs_followup',
-        '_cs_channel',
+        'channel',
         '_cs_namespace',
         '_cs_command',
     )
 
     def __init__(self, *, data: InteractionPayload, state: ConnectionState[ClientT]):
         self._state: ConnectionState[ClientT] = state
         self._client: ClientT = state._get_client()
@@ -167,16 +178,32 @@
 
     def _from_data(self, data: InteractionPayload):
         self.id: int = int(data['id'])
         self.type: InteractionType = try_enum(InteractionType, data['type'])
         self.data: Optional[InteractionData] = data.get('data')
         self.token: str = data['token']
         self.version: int = data['version']
-        self.channel_id: Optional[int] = utils._get_as_snowflake(data, 'channel_id')
         self.guild_id: Optional[int] = utils._get_as_snowflake(data, 'guild_id')
+        self.channel: Optional[InteractionChannel] = None
+
+        raw_channel = data.get('channel', {})
+        raw_ch_type = raw_channel.get('type')
+        if raw_ch_type is not None:
+            factory, ch_type = _threaded_channel_factory(raw_ch_type)  # type is never None
+            if factory is None:
+                logging.info('Unknown channel type {type} for channel ID {id}.'.format_map(raw_channel))
+            else:
+                if ch_type in (ChannelType.group, ChannelType.private):
+                    channel = factory(me=self._client.user, data=raw_channel, state=self._state)  # type: ignore
+                else:
+                    guild = self._state._get_or_create_unavailable_guild(self.guild_id)  # type: ignore
+                    channel = factory(guild=guild, state=self._state, data=raw_channel)  # type: ignore
+
+                self.channel = channel
+
         self.application_id: int = int(data['application_id'])
 
         self.locale: Locale = try_enum(Locale, data.get('locale', 'en-US'))
         self.guild_locale: Optional[Locale]
         try:
             self.guild_locale = try_enum(Locale, data['guild_locale'])
         except KeyError:
@@ -191,14 +218,19 @@
 
         self.user: Union[User, Member] = MISSING
         self._permissions: int = 0
         self._app_permissions: int = int(data.get('app_permissions', 0))
 
         if self.guild_id:
             guild = self._state._get_or_create_unavailable_guild(self.guild_id)
+
+            # Upgrade Message.guild in case it's missing with partial guild data
+            if self.message is not None and self.message.guild is None:
+                self.message.guild = guild
+
             try:
                 member = data['member']  # type: ignore # The key is optional and handled
             except KeyError:
                 pass
             else:
                 self.user = Member(state=self._state, guild=guild, data=member)
                 self._permissions = self.user._permissions or 0
@@ -218,29 +250,18 @@
         return self._client
 
     @property
     def guild(self) -> Optional[Guild]:
         """Optional[:class:`Guild`]: The guild the interaction was sent from."""
         return self._state and self._state._get_guild(self.guild_id)
 
-    @utils.cached_slot_property('_cs_channel')
-    def channel(self) -> Optional[InteractionChannel]:
-        """Optional[Union[:class:`abc.GuildChannel`, :class:`PartialMessageable`, :class:`Thread`]]: The channel the interaction was sent from.
-
-        Note that due to a Discord limitation, DM channels are not resolved since there is
-        no data to complete them. These are :class:`PartialMessageable` instead.
-        """
-        guild = self.guild
-        channel = guild and guild._resolve_channel(self.channel_id)
-        if channel is None:
-            if self.channel_id is not None:
-                type = ChannelType.text if self.guild_id is not None else ChannelType.private
-                return PartialMessageable(state=self._state, guild_id=self.guild_id, id=self.channel_id, type=type)
-            return None
-        return channel
+    @property
+    def channel_id(self) -> Optional[int]:
+        """Optional[:class:`int`]: The ID of the channel the interaction was sent from."""
+        return self.channel.id if self.channel is not None else None
 
     @property
     def permissions(self) -> Permissions:
         """:class:`Permissions`: The resolved permissions of the member in the channel, including overwrites.
 
         In a non-guild context where this doesn't apply, an empty permissions object is returned.
         """
@@ -1016,16 +1037,16 @@
     def __init__(self, interaction: Interaction, parent: ConnectionState):
         self._interaction: Interaction = interaction
         self._parent: ConnectionState = parent
 
     def _get_guild(self, guild_id):
         return self._parent._get_guild(guild_id)
 
-    def store_user(self, data):
-        return self._parent.store_user(data)
+    def store_user(self, data, *, cache: bool = True):
+        return self._parent.store_user(data, cache=cache)
 
     def create_user(self, data):
         return self._parent.create_user(data)
 
     @property
     def http(self):
         return self._parent.http
```

### Comparing `discord.py-2.2.3/discord/invite.py` & `discord.py-2.3.0/discord/invite.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/member.py` & `discord.py-2.3.0/discord/member.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
 
         .. describe:: hash(x)
 
             Returns the member's hash.
 
         .. describe:: str(x)
 
-            Returns the member's name with the discriminator.
+            Returns the member's handle (e.g. ``name`` or ``name#discriminator``).
 
     Attributes
     ----------
     joined_at: Optional[:class:`datetime.datetime`]
         An aware datetime object that specifies the date and time in UTC that the member joined the guild.
         If the member left and rejoined the guild, this will be the latest date. In certain cases, this can be ``None``.
     activities: Tuple[Union[:class:`BaseActivity`, :class:`Spotify`]]
@@ -289,15 +289,15 @@
             Due to a Discord API limitation, a user's Spotify activity may not appear
             if they are listening to a song with a title longer
             than 128 characters. See :issue:`1738` for more information.
 
     guild: :class:`Guild`
         The guild that the member belongs to.
     nick: Optional[:class:`str`]
-        The guild specific nickname of the user.
+        The guild specific nickname of the user. Takes precedence over the global name.
     pending: :class:`bool`
         Whether the member is pending member verification.
 
         .. versionadded:: 1.6
     premium_since: Optional[:class:`datetime.datetime`]
         An aware datetime object that specifies the date and time in UTC when the member used their
         "Nitro boost" on the guild, if available. This could be ``None``.
@@ -325,14 +325,15 @@
         '_flags',
     )
 
     if TYPE_CHECKING:
         name: str
         id: int
         discriminator: str
+        global_name: Optional[str]
         bot: bool
         system: bool
         created_at: datetime.datetime
         default_avatar: Asset
         avatar: Optional[Asset]
         dm_channel: Optional[DMChannel]
         create_dm: Callable[[], Awaitable[DMChannel]]
@@ -364,15 +365,15 @@
         self.timed_out_until: Optional[datetime.datetime] = utils.parse_time(data.get('communication_disabled_until'))
 
     def __str__(self) -> str:
         return str(self._user)
 
     def __repr__(self) -> str:
         return (
-            f'<Member id={self._user.id} name={self._user.name!r} discriminator={self._user.discriminator!r}'
+            f'<Member id={self._user.id} name={self._user.name!r} global_name={self._user.global_name!r}'
             f' bot={self._user.bot} nick={self.nick!r} guild={self.guild!r}>'
         )
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, _UserTag) and other.id == self.id
 
     def __ne__(self, other: object) -> bool:
@@ -459,20 +460,26 @@
 
         if len(user) > 1:
             return self._update_inner_user(user)
         return None
 
     def _update_inner_user(self, user: UserPayload) -> Optional[Tuple[User, User]]:
         u = self._user
-        original = (u.name, u._avatar, u.discriminator, u._public_flags)
+        original = (u.name, u.discriminator, u._avatar, u.global_name, u._public_flags)
         # These keys seem to always be available
-        modified = (user['username'], user['avatar'], user['discriminator'], user.get('public_flags', 0))
+        modified = (
+            user['username'],
+            user['discriminator'],
+            user['avatar'],
+            user.get('global_name'),
+            user.get('public_flags', 0),
+        )
         if original != modified:
             to_return = User._copy(self._user)
-            u.name, u._avatar, u.discriminator, u._public_flags = modified
+            u.name, u.discriminator, u._avatar, u.global_name, u._public_flags = modified
             # Signal to dispatch on_user_update
             return to_return, u
 
     @property
     def status(self) -> Status:
         """:class:`Status`: The member's overall status. If the value is unknown, then it will be a :class:`str` instead."""
         return try_enum(Status, self._client_status._status)
@@ -577,19 +584,19 @@
         """:class:`str`: Returns a string that allows you to mention the member."""
         return f'<@{self._user.id}>'
 
     @property
     def display_name(self) -> str:
         """:class:`str`: Returns the user's display name.
 
-        For regular users this is just their username, but
-        if they have a guild specific nickname then that
+        For regular users this is just their global name or their username,
+        but if they have a guild specific nickname then that
         is returned instead.
         """
-        return self.nick or self.name
+        return self.nick or self.global_name or self.name
 
     @property
     def display_avatar(self) -> Asset:
         """:class:`Asset`: Returns the member's display avatar.
 
         For regular members this is just their avatar, but
         if they have a guild specific avatar then that
```

### Comparing `discord.py-2.2.3/discord/mentions.py` & `discord.py-2.3.0/discord/mentions.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/message.py` & `discord.py-2.3.0/discord/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from .member import Member
 from .flags import MessageFlags
 from .file import File
 from .utils import escape_mentions, MISSING
 from .http import handle_message_parameters
 from .guild import Guild
 from .mixins import Hashable
-from .sticker import StickerItem
+from .sticker import StickerItem, GuildSticker
 from .threads import Thread
 from .channel import PartialMessageable
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
     from .types.message import (
@@ -179,47 +179,65 @@
         The attachment's description. Only applicable to images.
 
         .. versionadded:: 2.0
     ephemeral: :class:`bool`
         Whether the attachment is ephemeral.
 
         .. versionadded:: 2.0
+    duration: Optional[:class:`float`]
+        The duration of the audio file in seconds. Returns ``None`` if it's not a voice message.
+
+        .. versionadded:: 2.3
+    waveform: Optional[:class:`bytes`]
+        The waveform (amplitudes) of the audio in bytes. Returns ``None`` if it's not a voice message.
+
+        .. versionadded:: 2.3
     """
 
     __slots__ = (
         'id',
         'size',
         'height',
         'width',
         'filename',
         'url',
         'proxy_url',
         '_http',
         'content_type',
         'description',
         'ephemeral',
+        'duration',
+        'waveform',
     )
 
     def __init__(self, *, data: AttachmentPayload, state: ConnectionState):
         self.id: int = int(data['id'])
         self.size: int = data['size']
         self.height: Optional[int] = data.get('height')
         self.width: Optional[int] = data.get('width')
         self.filename: str = data['filename']
         self.url: str = data['url']
         self.proxy_url: str = data['proxy_url']
         self._http = state.http
         self.content_type: Optional[str] = data.get('content_type')
         self.description: Optional[str] = data.get('description')
         self.ephemeral: bool = data.get('ephemeral', False)
+        self.duration: Optional[float] = data.get('duration_secs')
+
+        waveform = data.get('waveform')
+        self.waveform: Optional[bytes] = utils._base64_to_bytes(waveform) if waveform is not None else None
 
     def is_spoiler(self) -> bool:
         """:class:`bool`: Whether this attachment contains a spoiler."""
         return self.filename.startswith('SPOILER_')
 
+    def is_voice_message(self) -> bool:
+        """:class:`bool`: Whether this attachment is a voice message."""
+        return self.duration is not None and 'voice-message' in self.url
+
     def __repr__(self) -> str:
         return f'<Attachment id={self.id} filename={self.filename!r} url={self.url!r}>'
 
     def __str__(self) -> str:
         return self.url or ''
 
     async def save(
@@ -1211,15 +1229,15 @@
         .. versionadded:: 2.0
 
         Parameters
         -----------
         name: :class:`str`
             The name of the thread.
         auto_archive_duration: :class:`int`
-            The duration in minutes before a thread is automatically archived for inactivity.
+            The duration in minutes before a thread is automatically hidden from the channel list.
             If not provided, the channel's default auto archive duration is used.
 
             Must be one of ``60``, ``1440``, ``4320``, or ``10080``, if provided.
         slowmode_delay: Optional[:class:`int`]
             Specifies the slowmode rate limit for user in this channel, in seconds.
             The maximum value possible is ``21600``. By default no slowmode rate limit
             if this is ``None``.
@@ -1250,14 +1268,94 @@
             name=name,
             auto_archive_duration=auto_archive_duration or default_auto_archive_duration,
             rate_limit_per_user=slowmode_delay,
             reason=reason,
         )
         return Thread(guild=self.guild, state=self._state, data=data)
 
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embed: Embed = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embed: Embed = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embeds: Sequence[Embed] = ...,
+        file: File = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
+    @overload
+    async def reply(
+        self,
+        content: Optional[str] = ...,
+        *,
+        tts: bool = ...,
+        embeds: Sequence[Embed] = ...,
+        files: Sequence[File] = ...,
+        stickers: Sequence[Union[GuildSticker, StickerItem]] = ...,
+        delete_after: float = ...,
+        nonce: Union[str, int] = ...,
+        allowed_mentions: AllowedMentions = ...,
+        reference: Union[Message, MessageReference, PartialMessage] = ...,
+        mention_author: bool = ...,
+        view: View = ...,
+        suppress_embeds: bool = ...,
+        silent: bool = ...,
+    ) -> Message:
+        ...
+
     async def reply(self, content: Optional[str] = None, **kwargs: Any) -> Message:
         """|coro|
 
         A shortcut method to :meth:`.abc.Messageable.send` to reply to the
         :class:`.Message`.
 
         .. versionadded:: 1.6
@@ -1706,15 +1804,15 @@
     def _handle_embeds(self, value: List[EmbedPayload]) -> None:
         self.embeds = [Embed.from_dict(data) for data in value]
 
     def _handle_nonce(self, value: Union[str, int]) -> None:
         self.nonce = value
 
     def _handle_author(self, author: UserPayload) -> None:
-        self.author = self._state.store_user(author)
+        self.author = self._state.store_user(author, cache=self.webhook_id is None)
         if isinstance(self.guild, Guild):
             found = self.guild.get_member(self.author.id)
             if found is not None:
                 self.author = found
 
     def _handle_member(self, member: MemberPayload) -> None:
         # The gateway now gives us full Member objects sometimes with the following keys
@@ -1725,15 +1823,14 @@
         # ourselves to a more "partial" member object.
         author = self.author
         try:
             # Update member reference
             author._update_from_message(member)  # type: ignore
         except AttributeError:
             # It's a user here
-            # TODO: consider adding to cache here
             self.author = Member._from_message(message=self, data=member)
 
     def _handle_mentions(self, mentions: List[UserWithMemberPayload]) -> None:
         self.mentions = r = []
         guild = self.guild
         state = self._state
         if not isinstance(guild, Guild):
@@ -1921,15 +2018,15 @@
         if self.type is MessageType.channel_name_change:
             if getattr(self.channel, 'parent', self.channel).type is ChannelType.forum:
                 return f'{self.author.name} changed the post title: **{self.content}**'
             else:
                 return f'{self.author.name} changed the channel name: **{self.content}**'
 
         if self.type is MessageType.channel_icon_change:
-            return f'{self.author.name} changed the channel icon.'
+            return f'{self.author.name} changed the group icon.'
 
         if self.type is MessageType.pins_add:
             return f'{self.author.name} pinned a message to this channel.'
 
         if self.type is MessageType.new_member:
             formats = [
                 "{0} joined the party.",
```

### Comparing `discord.py-2.2.3/discord/mixins.py` & `discord.py-2.3.0/discord/mixins.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/object.py` & `discord.py-2.3.0/discord/object.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/oggparse.py` & `discord.py-2.3.0/discord/oggparse.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/opus.py` & `discord.py-2.3.0/discord/opus.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,15 +450,17 @@
             raise TypeError("Invalid arguments: FEC cannot be used with null data")
 
         if data is None:
             frame_size = self._get_last_packet_duration() or self.SAMPLES_PER_FRAME
             channel_count = self.CHANNELS
         else:
             frames = self.packet_get_nb_frames(data)
-            channel_count = self.packet_get_nb_channels(data)
+            # Discord silent frames erroneously present themselves as 1 channel instead of 2
+            # Therefore we need to hardcode the number instead of using packet_get_nb_channels
+            channel_count = self.CHANNELS
             samples_per_frame = self.packet_get_samples_per_frame(data)
             frame_size = frames * samples_per_frame
 
         pcm = (ctypes.c_int16 * (frame_size * channel_count))()
         pcm_ptr = ctypes.cast(pcm, c_int16_ptr)
 
         ret = _lib.opus_decode(self._state, data, len(data) if data else 0, pcm_ptr, frame_size, fec)
```

### Comparing `discord.py-2.2.3/discord/partial_emoji.py` & `discord.py-2.3.0/discord/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/permissions.py` & `discord.py-2.3.0/discord/permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,20 @@
                Return the permission's hash.
         .. describe:: iter(x)
 
                Returns an iterator of ``(perm, value)`` pairs. This allows it
                to be, for example, constructed as a dict or a list of pairs.
                Note that aliases are not shown.
 
+        .. describe:: bool(b)
+
+            Returns whether the permissions object has any permissions set to ``True``.
+
+            .. versionadded:: 2.0
+
     Attributes
     -----------
     value: :class:`int`
         The raw value. This value is a bit array field of a 53-bit integer
         representing the currently available permissions. You should query
         permissions via the properties rather than using this raw value.
     """
@@ -173,15 +179,15 @@
         return cls(0)
 
     @classmethod
     def all(cls) -> Self:
         """A factory method that creates a :class:`Permissions` with all
         permissions set to ``True``.
         """
-        return cls(0b11111111111111111111111111111111111111111)
+        return cls(0b11111111111111111111111111111111111111111111111)
 
     @classmethod
     def _timeout_mask(cls) -> int:
         p = cls.all()
         p.view_channel = False
         p.read_message_history = False
         return ~p.value
@@ -200,46 +206,53 @@
 
     @classmethod
     def all_channel(cls) -> Self:
         """A :class:`Permissions` with all channel-specific permissions set to
         ``True`` and the guild-specific ones set to ``False``. The guild-specific
         permissions are currently:
 
-        - :attr:`manage_emojis`
+        - :attr:`manage_expressions`
         - :attr:`view_audit_log`
         - :attr:`view_guild_insights`
         - :attr:`manage_guild`
         - :attr:`change_nickname`
         - :attr:`manage_nicknames`
         - :attr:`kick_members`
         - :attr:`ban_members`
         - :attr:`administrator`
+        - :attr:`create_expressions`
 
         .. versionchanged:: 1.7
            Added :attr:`stream`, :attr:`priority_speaker` and :attr:`use_application_commands` permissions.
 
         .. versionchanged:: 2.0
            Added :attr:`create_public_threads`, :attr:`create_private_threads`, :attr:`manage_threads`,
            :attr:`use_external_stickers`, :attr:`send_messages_in_threads` and
            :attr:`request_to_speak` permissions.
+
+        .. versionchanged:: 2.3
+           Added :attr:`use_soundboard`, :attr:`create_expressions` permissions.
         """
-        return cls(0b111110110110011111101111111111101010001)
+        return cls(0b01000111110110110011111101111111111101010001)
 
     @classmethod
     def general(cls) -> Self:
         """A factory method that creates a :class:`Permissions` with all
         "General" permissions from the official Discord UI set to ``True``.
 
         .. versionchanged:: 1.7
            Permission :attr:`read_messages` is now included in the general permissions, but
            permissions :attr:`administrator`, :attr:`create_instant_invite`, :attr:`kick_members`,
            :attr:`ban_members`, :attr:`change_nickname` and :attr:`manage_nicknames` are
            no longer part of the general permissions.
+
+        .. versionchanged:: 2.3
+            Added :attr:`create_expressions` permission.
         """
-        return cls(0b01110000000010000000010010110000)
+        return cls(0b10000000000001110000000010000000010010110000)
 
     @classmethod
     def membership(cls) -> Self:
         """A factory method that creates a :class:`Permissions` with all
         "Membership" permissions from the official Discord UI set to ``True``.
 
         .. versionadded:: 1.7
@@ -254,22 +267,25 @@
         .. versionchanged:: 1.7
            Permission :attr:`read_messages` is no longer part of the text permissions.
            Added :attr:`use_application_commands` permission.
 
         .. versionchanged:: 2.0
            Added :attr:`create_public_threads`, :attr:`create_private_threads`, :attr:`manage_threads`,
            :attr:`send_messages_in_threads` and :attr:`use_external_stickers` permissions.
+
+        .. versionchanged:: 2.3
+            Added :attr:`send_voice_messages` permission.
         """
-        return cls(0b111110010000000000001111111100001000000)
+        return cls(0b10000000111110010000000000001111111100001000000)
 
     @classmethod
     def voice(cls) -> Self:
         """A factory method that creates a :class:`Permissions` with all
         "Voice" permissions from the official Discord UI set to ``True``."""
-        return cls(0b1000000000000011111100000000001100000000)
+        return cls(0b1001001000000000000011111100000000001100000000)
 
     @classmethod
     def stage(cls) -> Self:
         """A factory method that creates a :class:`Permissions` with all
         "Stage Channel" permissions from the official Discord UI set to ``True``.
 
         .. versionadded:: 1.7
@@ -301,15 +317,15 @@
         - :attr:`ban_members`
         - :attr:`administrator`
         - :attr:`manage_channels`
         - :attr:`manage_guild`
         - :attr:`manage_messages`
         - :attr:`manage_roles`
         - :attr:`manage_webhooks`
-        - :attr:`manage_emojis_and_stickers`
+        - :attr:`manage_expressions`
         - :attr:`manage_threads`
         - :attr:`moderate_members`
 
         .. versionadded:: 2.0
         """
         return cls(0b10000010001110000000000000010000000111110)
 
@@ -540,21 +556,29 @@
 
     @flag_value
     def manage_webhooks(self) -> int:
         """:class:`bool`: Returns ``True`` if a user can create, edit, or delete webhooks."""
         return 1 << 29
 
     @flag_value
+    def manage_expressions(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can edit or delete emojis, stickers, and soundboard sounds.
+
+        .. versionadded:: 2.3
+        """
+        return 1 << 30
+
+    @make_permission_alias('manage_expressions')
     def manage_emojis(self) -> int:
-        """:class:`bool`: Returns ``True`` if a user can create, edit, or delete emojis."""
+        """:class:`bool`: An alias for :attr:`manage_expressions`."""
         return 1 << 30
 
-    @make_permission_alias('manage_emojis')
+    @make_permission_alias('manage_expressions')
     def manage_emojis_and_stickers(self) -> int:
-        """:class:`bool`: An alias for :attr:`manage_emojis`.
+        """:class:`bool`: An alias for :attr:`manage_expressions`.
 
         .. versionadded:: 2.0
         """
         return 1 << 30
 
     @flag_value
     def use_application_commands(self) -> int:
@@ -640,14 +664,46 @@
     def moderate_members(self) -> int:
         """:class:`bool`: Returns ``True`` if a user can time out other members.
 
         .. versionadded:: 2.0
         """
         return 1 << 40
 
+    @flag_value
+    def use_soundboard(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can use the soundboard.
+
+        .. versionadded:: 2.3
+        """
+        return 1 << 42
+
+    @flag_value
+    def create_expressions(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can create emojis, stickers, and soundboard sounds.
+
+        .. versionadded:: 2.3
+        """
+        return 1 << 43
+
+    @flag_value
+    def use_external_sounds(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can use sounds from other guilds.
+
+        .. versionadded:: 2.3
+        """
+        return 1 << 45
+
+    @flag_value
+    def send_voice_messages(self) -> int:
+        """:class:`bool`: Returns ``True`` if a user can send voice messages.
+
+        .. versionadded:: 2.3
+        """
+        return 1 << 46
+
 
 def _augment_from_permissions(cls):
     cls.VALID_NAMES = set(Permissions.VALID_FLAGS)
     aliases = set()
 
     # make descriptors for all the valid names and aliases
     for name, value in Permissions.__dict__.items():
@@ -741,27 +797,32 @@
         move_members: Optional[bool]
         use_voice_activation: Optional[bool]
         change_nickname: Optional[bool]
         manage_nicknames: Optional[bool]
         manage_roles: Optional[bool]
         manage_permissions: Optional[bool]
         manage_webhooks: Optional[bool]
+        manage_expressions: Optional[bool]
         manage_emojis: Optional[bool]
         manage_emojis_and_stickers: Optional[bool]
         use_application_commands: Optional[bool]
         request_to_speak: Optional[bool]
         manage_events: Optional[bool]
         manage_threads: Optional[bool]
         create_public_threads: Optional[bool]
         create_private_threads: Optional[bool]
         send_messages_in_threads: Optional[bool]
         external_stickers: Optional[bool]
         use_external_stickers: Optional[bool]
         use_embedded_activities: Optional[bool]
         moderate_members: Optional[bool]
+        use_soundboard: Optional[bool]
+        use_external_sounds: Optional[bool]
+        send_voice_messages: Optional[bool]
+        create_expressions: Optional[bool]
 
     def __init__(self, **kwargs: Optional[bool]):
         self._values: Dict[str, Optional[bool]] = {}
 
         for key, value in kwargs.items():
             if key not in self.VALID_NAMES:
                 raise ValueError(f'no permission called {key}.')
```

### Comparing `discord.py-2.2.3/discord/player.py` & `discord.py-2.3.0/discord/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,16 @@
             _log.info('ffmpeg process %s successfully terminated with return code of %s.', proc.pid, proc.returncode)
 
     def _pipe_writer(self, source: io.BufferedIOBase) -> None:
         while self._process:
             # arbitrarily large read size
             data = source.read(8192)
             if not data:
-                self._process.terminate()
+                if self._stdin is not None:
+                    self._stdin.close()
                 return
             try:
                 if self._stdin is not None:
                     self._stdin.write(data)
             except Exception:
                 _log.debug('Write error for %s, this is probably not a problem', self, exc_info=True)
                 # at this point the source data is either exhausted or the process is fubar
```

### Comparing `discord.py-2.2.3/discord/raw_models.py` & `discord.py-2.3.0/discord/raw_models.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/reaction.py` & `discord.py-2.3.0/discord/reaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 
     def __init__(self, *, message: Message, data: ReactionPayload, emoji: Optional[Union[PartialEmoji, Emoji, str]] = None):
         self.message: Message = message
         self.emoji: Union[PartialEmoji, Emoji, str] = emoji or message._state.get_reaction_emoji(data['emoji'])
         self.count: int = data.get('count', 1)
         self.me: bool = data['me']
 
-    # TODO: typeguard
     def is_custom_emoji(self) -> bool:
         """:class:`bool`: If this is a custom emoji."""
         return not isinstance(self.emoji, str)
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, self.__class__) and other.emoji == self.emoji
```

### Comparing `discord.py-2.2.3/discord/role.py` & `discord.py-2.3.0/discord/role.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/scheduled_event.py` & `discord.py-2.3.0/discord/scheduled_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,26 +499,25 @@
             if channel and isinstance(channel, Object):
                 if channel.type is VoiceChannel:
                     entity_type = EntityType.voice
                 elif channel.type is StageChannel:
                     entity_type = EntityType.stage_instance
             elif location not in (MISSING, None):
                 entity_type = EntityType.external
+        else:
+            if not isinstance(entity_type, EntityType):
+                raise TypeError('entity_type must be of type EntityType')
+
+            payload['entity_type'] = entity_type.value
 
         if entity_type is None:
             raise TypeError(
                 f'invalid GuildChannel type passed, must be VoiceChannel or StageChannel not {channel.__class__.__name__}'
             )
 
-        if entity_type is not MISSING:
-            if not isinstance(entity_type, EntityType):
-                raise TypeError('entity_type must be of type EntityType')
-
-            payload['entity_type'] = entity_type.value
-
         _entity_type = entity_type or self.entity_type
         _entity_type_changed = _entity_type is not self.entity_type
 
         if _entity_type in (EntityType.stage_instance, EntityType.voice):
             if channel is MISSING or channel is None:
                 if _entity_type_changed:
                     raise TypeError('channel must be set when entity_type is voice or stage_instance')
```

### Comparing `discord.py-2.2.3/discord/shard.py` & `discord.py-2.3.0/discord/shard.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/stage_instance.py` & `discord.py-2.3.0/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/state.py` & `discord.py-2.3.0/discord/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,26 +345,26 @@
     def _remove_voice_client(self, guild_id: int) -> None:
         self._voice_clients.pop(guild_id, None)
 
     def _update_references(self, ws: DiscordWebSocket) -> None:
         for vc in self.voice_clients:
             vc.main_ws = ws  # type: ignore # Silencing the unknown attribute (ok at runtime).
 
-    def store_user(self, data: Union[UserPayload, PartialUserPayload]) -> User:
+    def store_user(self, data: Union[UserPayload, PartialUserPayload], *, cache: bool = True) -> User:
         # this way is 300% faster than `dict.setdefault`.
         user_id = int(data['id'])
         try:
             return self._users[user_id]
         except KeyError:
             user = User(state=self, data=data)
-            if user.discriminator != '0000':
+            if cache:
                 self._users[user_id] = user
             return user
 
-    def store_user_no_intents(self, data: Union[UserPayload, PartialUserPayload]) -> User:
+    def store_user_no_intents(self, data: Union[UserPayload, PartialUserPayload], *, cache: bool = True) -> User:
         return User(state=self, data=data)
 
     def create_user(self, data: Union[UserPayload, PartialUserPayload]) -> User:
         return User(state=self, data=data)
 
     def get_user(self, id: int) -> Optional[User]:
         return self._users.get(id)
@@ -610,15 +610,15 @@
         channel, _ = self._get_guild_channel(data)
         # channel would be the correct type here
         message = Message(channel=channel, data=data, state=self)  # type: ignore
         self.dispatch('message', message)
         if self._messages is not None:
             self._messages.append(message)
         # we ensure that the channel is either a TextChannel, VoiceChannel, or Thread
-        if channel and channel.__class__ in (TextChannel, VoiceChannel, Thread):
+        if channel and channel.__class__ in (TextChannel, VoiceChannel, Thread, StageChannel):
             channel.last_message_id = message.id  # type: ignore
 
     def parse_message_delete(self, data: gw.MessageDeleteEvent) -> None:
         raw = RawMessageDeleteEvent(data)
         found = self._get_message(raw.message_id)
         raw.cached_message = found
         self.dispatch('raw_message_delete', raw)
@@ -1104,14 +1104,15 @@
             return
 
         entry = AuditLogEntry(
             users=self._users,
             integrations={},
             app_commands={},
             automod_rules={},
+            webhooks={},
             data=data,
             guild=guild,
         )
 
         self.dispatch('audit_log_entry_create', entry)
 
     def parse_auto_moderation_rule_create(self, data: AutoModerationRule) -> None:
```

### Comparing `discord.py-2.2.3/discord/sticker.py` & `discord.py-2.3.0/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/team.py` & `discord.py-2.3.0/discord/team.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,26 +104,30 @@
 
         .. describe:: hash(x)
 
             Return the team member's hash.
 
         .. describe:: str(x)
 
-            Returns the team member's name with discriminator.
+            Returns the team member's handle (e.g. ``name`` or ``name#discriminator``).
 
     .. versionadded:: 1.3
 
     Attributes
     -------------
     name: :class:`str`
         The team member's username.
     id: :class:`int`
         The team member's unique ID.
     discriminator: :class:`str`
-        The team member's discriminator. This is given when the username has conflicts.
+        The team member's discriminator. This is a legacy concept that is no longer used.
+    global_name: Optional[:class:`str`]
+        The team member's global nickname, taking precedence over the username in display.
+
+        .. versionadded:: 2.3
     bot: :class:`bool`
         Specifies if the user is a bot account.
     team: :class:`Team`
         The team that the member is from.
     membership_state: :class:`TeamMembershipState`
         The membership state of the member (e.g. invited or accepted)
     """
@@ -135,9 +139,9 @@
         self.membership_state: TeamMembershipState = try_enum(TeamMembershipState, data['membership_state'])
         self.permissions: List[str] = data['permissions']
         super().__init__(state=state, data=data['user'])
 
     def __repr__(self) -> str:
         return (
             f'<{self.__class__.__name__} id={self.id} name={self.name!r} '
-            f'discriminator={self.discriminator!r} membership_state={self.membership_state!r}>'
+            f'global_name={self.global_name!r} membership_state={self.membership_state!r}>'
         )
```

### Comparing `discord.py-2.2.3/discord/template.py` & `discord.py-2.3.0/discord/template.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/threads.py` & `discord.py-2.3.0/discord/threads.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         Whether the thread is locked.
     invitable: :class:`bool`
         Whether non-moderators can add other non-moderators to this thread.
         This is always ``True`` for public threads.
     archiver_id: Optional[:class:`int`]
         The user's ID that archived this thread.
     auto_archive_duration: :class:`int`
-        The duration in minutes until the thread is automatically archived due to inactivity.
+        The duration in minutes until the thread is automatically hidden from the channel list.
         Usually a value of 60, 1440, 4320 and 10080.
     archive_timestamp: :class:`datetime.datetime`
         An aware timestamp of when the thread's archived status was last updated in UTC.
     """
 
     __slots__ = (
         'name',
@@ -604,15 +604,15 @@
             Whether to lock the thread or not.
         pinned: :class:`bool`
             Whether to pin the thread or not. This only works if the thread is part of a forum.
         invitable: :class:`bool`
             Whether non-moderators can add other non-moderators to this thread.
             Only available for private threads.
         auto_archive_duration: :class:`int`
-            The new duration in minutes before a thread is automatically archived for inactivity.
+            The new duration in minutes before a thread is automatically hidden from the channel list.
             Must be one of ``60``, ``1440``, ``4320``, or ``10080``.
         slowmode_delay: :class:`int`
             Specifies the slowmode rate limit for user in this thread, in seconds.
             A value of ``0`` disables slowmode. The maximum value possible is ``21600``.
         applied_tags: Sequence[:class:`ForumTag`]
             The new tags to apply to the thread. There can only be up to 5 tags applied to a thread.
```

### Comparing `discord.py-2.2.3/discord/types/activity.py` & `discord.py-2.3.0/discord/types/activity.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/appinfo.py` & `discord.py-2.3.0/discord/types/appinfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,41 +40,42 @@
 class BaseAppInfo(TypedDict):
     id: Snowflake
     name: str
     verify_key: str
     icon: Optional[str]
     summary: str
     description: str
+    flags: int
+    cover_image: NotRequired[str]
+    terms_of_service_url: NotRequired[str]
+    privacy_policy_url: NotRequired[str]
+    rpc_origins: NotRequired[List[str]]
 
 
 class AppInfo(BaseAppInfo):
-    rpc_origins: List[str]
     owner: User
     bot_public: bool
     bot_require_code_grant: bool
     team: NotRequired[Team]
     guild_id: NotRequired[Snowflake]
     primary_sku_id: NotRequired[Snowflake]
     slug: NotRequired[str]
-    terms_of_service_url: NotRequired[str]
-    privacy_policy_url: NotRequired[str]
     hook: NotRequired[bool]
     max_participants: NotRequired[int]
     tags: NotRequired[List[str]]
     install_params: NotRequired[InstallParams]
     custom_install_url: NotRequired[str]
     role_connections_verification_url: NotRequired[str]
 
 
 class PartialAppInfo(BaseAppInfo, total=False):
-    rpc_origins: List[str]
-    cover_image: str
     hook: bool
-    terms_of_service_url: str
-    privacy_policy_url: str
     max_participants: int
-    flags: int
+    approximate_guild_count: int
+    redirect_uris: List[str]
+    interactions_endpoint_url: Optional[str]
+    role_connections_verification_url: Optional[str]
 
 
 class GatewayAppInfo(TypedDict):
     id: Snowflake
     flags: int
```

### Comparing `discord.py-2.2.3/discord/types/audit_log.py` & `discord.py-2.3.0/discord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/automod.py` & `discord.py-2.3.0/discord/types/automod.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/channel.py` & `discord.py-2.3.0/discord/types/channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,38 +130,48 @@
     id: Snowflake
     name: str
     moderated: bool
     emoji_id: Optional[Snowflake]
     emoji_name: Optional[str]
 
 
+ForumOrderType = Literal[0, 1]
 ForumLayoutType = Literal[0, 1, 2]
 
 
 class ForumChannel(_BaseTextChannel):
     type: Literal[15]
     available_tags: List[ForumTag]
     default_reaction_emoji: Optional[DefaultReaction]
+    default_sort_order: Optional[ForumOrderType]
     default_forum_layout: NotRequired[ForumLayoutType]
     flags: NotRequired[int]
 
 
 GuildChannel = Union[TextChannel, NewsChannel, VoiceChannel, CategoryChannel, StageChannel, ThreadChannel, ForumChannel]
 
 
-class DMChannel(_BaseChannel):
+class _BaseDMChannel(_BaseChannel):
     type: Literal[1]
     last_message_id: Optional[Snowflake]
+
+
+class DMChannel(_BaseDMChannel):
     recipients: List[PartialUser]
 
 
+class InteractionDMChannel(_BaseDMChannel):
+    recipients: NotRequired[List[PartialUser]]
+
+
 class GroupDMChannel(_BaseChannel):
     type: Literal[3]
     icon: Optional[str]
     owner_id: Snowflake
+    recipients: List[PartialUser]
 
 
 Channel = Union[GuildChannel, DMChannel, GroupDMChannel]
 
 PrivacyLevel = Literal[2]
```

### Comparing `discord.py-2.2.3/discord/types/command.py` & `discord.py-2.3.0/discord/types/command.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/components.py` & `discord.py-2.3.0/discord/types/components.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/embed.py` & `discord.py-2.3.0/discord/types/embed.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/emoji.py` & `discord.py-2.3.0/discord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/gateway.py` & `discord.py-2.3.0/discord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/guild.py` & `discord.py-2.3.0/discord/types/guild.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     'ROLE_SUBSCRIPTIONS_AVAILABLE_FOR_PURCHASE',
     'ROLE_SUBSCRIPTIONS_ENABLED',
     'TICKETED_EVENTS_ENABLED',
     'VANITY_URL',
     'VERIFIED',
     'VIP_REGIONS',
     'WELCOME_SCREEN_ENABLED',
+    'RAID_ALERTS_DISABLED',
 ]
 
 
 class _BaseGuildPreview(UnavailableGuild):
     name: str
     icon: Optional[str]
     splash: Optional[str]
@@ -157,14 +158,18 @@
     ...
 
 
 class GuildPrune(TypedDict):
     pruned: Optional[int]
 
 
+class GuildMFALevel(TypedDict):
+    level: MFALevel
+
+
 class ChannelPositionUpdate(TypedDict):
     id: Snowflake
     position: Optional[int]
     lock_permissions: Optional[bool]
     parent_id: Optional[Snowflake]
```

### Comparing `discord.py-2.2.3/discord/types/integration.py` & `discord.py-2.3.0/discord/types/integration.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/interactions.py` & `discord.py-2.3.0/discord/types/interactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, List, Literal, TypedDict, Union
 from typing_extensions import NotRequired
 
-from .channel import ChannelTypeWithoutThread, ThreadMetadata
+from .channel import ChannelTypeWithoutThread, ThreadMetadata, GuildChannel, InteractionDMChannel, GroupDMChannel
 from .threads import ThreadType
 from .member import Member
 from .message import Attachment
 from .role import Role
 from .snowflake import Snowflake
 from .user import User
 
@@ -200,14 +200,15 @@
 class _BaseInteraction(TypedDict):
     id: Snowflake
     application_id: Snowflake
     token: str
     version: Literal[1]
     guild_id: NotRequired[Snowflake]
     channel_id: NotRequired[Snowflake]
+    channel: Union[GuildChannel, InteractionDMChannel, GroupDMChannel]
     app_permissions: NotRequired[str]
     locale: NotRequired[str]
     guild_locale: NotRequired[str]
 
 
 class PingInteraction(_BaseInteraction):
     type: Literal[1]
```

### Comparing `discord.py-2.2.3/discord/types/invite.py` & `discord.py-2.3.0/discord/types/invite.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/member.py` & `discord.py-2.3.0/discord/types/member.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/message.py` & `discord.py-2.3.0/discord/types/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     proxy_url: str
     height: NotRequired[Optional[int]]
     width: NotRequired[Optional[int]]
     description: NotRequired[str]
     content_type: NotRequired[str]
     spoiler: NotRequired[bool]
     ephemeral: NotRequired[bool]
+    duration_secs: NotRequired[float]
+    waveform: NotRequired[str]
 
 
 MessageActivityType = Literal[1, 2, 3, 5]
 
 
 class MessageActivity(TypedDict):
     type: MessageActivityType
```

### Comparing `discord.py-2.2.3/discord/types/role.py` & `discord.py-2.3.0/discord/types/role.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/scheduled_event.py` & `discord.py-2.3.0/discord/types/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/snowflake.py` & `discord.py-2.3.0/discord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/sticker.py` & `discord.py-2.3.0/discord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/team.py` & `discord.py-2.3.0/discord/types/team.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/template.py` & `discord.py-2.3.0/discord/types/template.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/threads.py` & `discord.py-2.3.0/discord/types/threads.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/user.py` & `discord.py-2.3.0/discord/types/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,23 @@
 
 
 class PartialUser(TypedDict):
     id: Snowflake
     username: str
     discriminator: str
     avatar: Optional[str]
+    global_name: Optional[str]
 
 
 PremiumType = Literal[0, 1, 2]
 
 
 class User(PartialUser, total=False):
     bot: bool
     system: bool
     mfa_enabled: bool
-    local: str
+    locale: str
     verified: bool
     email: Optional[str]
     flags: int
     premium_type: PremiumType
     public_flags: int
```

### Comparing `discord.py-2.2.3/discord/types/voice.py` & `discord.py-2.3.0/discord/types/voice.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/webhook.py` & `discord.py-2.3.0/discord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/welcome_screen.py` & `discord.py-2.3.0/discord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/types/widget.py` & `discord.py-2.3.0/discord/types/widget.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ui/button.py` & `discord.py-2.3.0/discord/ui/button.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ui/item.py` & `discord.py-2.3.0/discord/ui/item.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/ui/modal.py` & `discord.py-2.3.0/discord/ui/modal.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     .. versionadded:: 2.0
 
     Examples
     ----------
 
     .. code-block:: python3
 
+        import discord
         from discord import ui
 
         class Questionnaire(ui.Modal, title='Questionnaire Response'):
             name = ui.TextInput(label='Name')
             answer = ui.TextInput(label='Answer', style=discord.TextStyle.paragraph)
 
             async def on_submit(self, interaction: discord.Interaction):
```

### Comparing `discord.py-2.2.3/discord/ui/select.py` & `discord.py-2.3.0/discord/ui/select.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,18 +158,18 @@
     def custom_id(self) -> str:
         """:class:`str`: The ID of the select menu that gets received during an interaction."""
         return self._underlying.custom_id
 
     @custom_id.setter
     def custom_id(self, value: str) -> None:
         if not isinstance(value, str):
-            raise TypeError('custom_id must be None or str')
+            raise TypeError('custom_id must be a str')
 
         self._underlying.custom_id = value
-        self._provided_custom_id = value is not None
+        self._provided_custom_id = True
 
     @property
     def placeholder(self) -> Optional[str]:
         """Optional[:class:`str`]: The placeholder text that is shown if nothing is selected, if any."""
         return self._underlying.placeholder
 
     @placeholder.setter
```

### Comparing `discord.py-2.2.3/discord/ui/text_input.py` & `discord.py-2.3.0/discord/ui/text_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,17 +133,18 @@
     def custom_id(self) -> str:
         """:class:`str`: The ID of the text input that gets received during an interaction."""
         return self._underlying.custom_id
 
     @custom_id.setter
     def custom_id(self, value: str) -> None:
         if not isinstance(value, str):
-            raise TypeError('custom_id must be None or str')
+            raise TypeError('custom_id must be a str')
 
         self._underlying.custom_id = value
+        self._provided_custom_id = True
 
     @property
     def width(self) -> int:
         return 5
 
     @property
     def value(self) -> str:
```

### Comparing `discord.py-2.2.3/discord/ui/view.py` & `discord.py-2.3.0/discord/ui/view.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/user.py` & `discord.py-2.3.0/discord/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,46 +61,50 @@
 
 
 class BaseUser(_UserTag):
     __slots__ = (
         'name',
         'id',
         'discriminator',
+        'global_name',
         '_avatar',
         '_banner',
         '_accent_colour',
         'bot',
         'system',
         '_public_flags',
         '_state',
     )
 
     if TYPE_CHECKING:
         name: str
         id: int
         discriminator: str
+        global_name: Optional[str]
         bot: bool
         system: bool
         _state: ConnectionState
         _avatar: Optional[str]
         _banner: Optional[str]
         _accent_colour: Optional[int]
         _public_flags: int
 
     def __init__(self, *, state: ConnectionState, data: Union[UserPayload, PartialUserPayload]) -> None:
         self._state = state
         self._update(data)
 
     def __repr__(self) -> str:
         return (
-            f"<BaseUser id={self.id} name={self.name!r} discriminator={self.discriminator!r}"
+            f"<BaseUser id={self.id} name={self.name!r} global_name={self.global_name!r}"
             f" bot={self.bot} system={self.system}>"
         )
 
     def __str__(self) -> str:
+        if self.discriminator == '0':
+            return self.name
         return f'{self.name}#{self.discriminator}'
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, _UserTag) and other.id == self.id
 
     def __ne__(self, other: object) -> bool:
         return not self.__eq__(other)
@@ -108,28 +112,30 @@
     def __hash__(self) -> int:
         return self.id >> 22
 
     def _update(self, data: Union[UserPayload, PartialUserPayload]) -> None:
         self.name = data['username']
         self.id = int(data['id'])
         self.discriminator = data['discriminator']
+        self.global_name = data.get('global_name')
         self._avatar = data['avatar']
         self._banner = data.get('banner', None)
         self._accent_colour = data.get('accent_color', None)
         self._public_flags = data.get('public_flags', 0)
         self.bot = data.get('bot', False)
         self.system = data.get('system', False)
 
     @classmethod
     def _copy(cls, user: Self) -> Self:
         self = cls.__new__(cls)  # bypass __init__
 
         self.name = user.name
         self.id = user.id
         self.discriminator = user.discriminator
+        self.global_name = user.global_name
         self._avatar = user._avatar
         self._banner = user._banner
         self._accent_colour = user._accent_colour
         self.bot = user.bot
         self._state = user._state
         self._public_flags = user._public_flags
 
@@ -137,14 +143,15 @@
 
     def _to_minimal_user_json(self) -> Dict[str, Any]:
         return {
             'username': self.name,
             'id': self.id,
             'avatar': self._avatar,
             'discriminator': self.discriminator,
+            'global_name': self.global_name,
             'bot': self.bot,
         }
 
     @property
     def public_flags(self) -> PublicUserFlags:
         """:class:`PublicUserFlags`: The publicly available flags the user has."""
         return PublicUserFlags._from_value(self._public_flags)
@@ -158,16 +165,21 @@
         """
         if self._avatar is not None:
             return Asset._from_avatar(self._state, self.id, self._avatar)
         return None
 
     @property
     def default_avatar(self) -> Asset:
-        """:class:`Asset`: Returns the default avatar for a given user. This is calculated by the user's discriminator."""
-        return Asset._from_default_avatar(self._state, int(self.discriminator) % len(DefaultAvatar))
+        """:class:`Asset`: Returns the default avatar for a given user."""
+        if self.discriminator == '0':
+            avatar_id = (self.id >> 22) % len(DefaultAvatar)
+        else:
+            avatar_id = int(self.discriminator) % 5
+
+        return Asset._from_default_avatar(self._state, avatar_id)
 
     @property
     def display_avatar(self) -> Asset:
         """:class:`Asset`: Returns the user's display avatar.
 
         For regular users this is just their default avatar or uploaded avatar.
 
@@ -256,18 +268,20 @@
         """
         return snowflake_time(self.id)
 
     @property
     def display_name(self) -> str:
         """:class:`str`: Returns the user's display name.
 
-        For regular users this is just their username, but
-        if they have a guild specific nickname then that
+        For regular users this is just their global name or their username,
+        but if they have a guild specific nickname then that
         is returned instead.
         """
+        if self.global_name:
+            return self.global_name
         return self.name
 
     def mentioned_in(self, message: Message) -> bool:
         """Checks if the user is mentioned in the specified message.
 
         Parameters
         -----------
@@ -301,24 +315,28 @@
 
         .. describe:: hash(x)
 
             Return the user's hash.
 
         .. describe:: str(x)
 
-            Returns the user's name with discriminator.
+            Returns the user's handle (e.g. ``name`` or ``name#discriminator``).
 
     Attributes
     -----------
     name: :class:`str`
         The user's username.
     id: :class:`int`
         The user's unique ID.
     discriminator: :class:`str`
-        The user's discriminator. This is given when the username has conflicts.
+        The user's discriminator. This is a legacy concept that is no longer used.
+    global_name: Optional[:class:`str`]
+        The user's global nickname, taking precedence over the username in display.
+
+        .. versionadded:: 2.3
     bot: :class:`bool`
         Specifies if the user is a bot account.
     system: :class:`bool`
         Specifies if the user is a system user (i.e. represents Discord officially).
 
         .. versionadded:: 1.3
 
@@ -339,15 +357,15 @@
         _flags: int
 
     def __init__(self, *, state: ConnectionState, data: UserPayload) -> None:
         super().__init__(state=state, data=data)
 
     def __repr__(self) -> str:
         return (
-            f'<ClientUser id={self.id} name={self.name!r} discriminator={self.discriminator!r}'
+            f'<ClientUser id={self.id} name={self.name!r} global_name={self.global_name!r}'
             f' bot={self.bot} verified={self.verified} mfa_enabled={self.mfa_enabled}>'
         )
 
     def _update(self, data: UserPayload) -> None:
         super()._update(data)
         # There's actually an Optional[str] phone field as well but I won't use it
         self.verified = data.get('verified', False)
@@ -405,14 +423,26 @@
                 payload['avatar'] = _bytes_to_base64_data(avatar)
             else:
                 payload['avatar'] = None
 
         data: UserPayload = await self._state.http.edit_profile(payload)
         return ClientUser(state=self._state, data=data)
 
+    @property
+    def mutual_guilds(self) -> List[Guild]:
+        """List[:class:`Guild`]: The guilds that the user shares with the client.
+
+        .. note::
+
+            This will only return mutual guilds within the client's internal cache.
+
+        .. versionadded:: 1.7
+        """
+        return list(self._state.guilds)
+
 
 class User(BaseUser, discord.abc.Messageable):
     """Represents a Discord user.
 
     .. container:: operations
 
         .. describe:: x == y
@@ -425,34 +455,38 @@
 
         .. describe:: hash(x)
 
             Return the user's hash.
 
         .. describe:: str(x)
 
-            Returns the user's name with discriminator.
+            Returns the user's handle (e.g. ``name`` or ``name#discriminator``).
 
     Attributes
     -----------
     name: :class:`str`
         The user's username.
     id: :class:`int`
         The user's unique ID.
     discriminator: :class:`str`
-        The user's discriminator. This is given when the username has conflicts.
+        The user's discriminator. This is a legacy concept that is no longer used.
+    global_name: Optional[:class:`str`]
+        The user's global nickname, taking precedence over the username in display.
+
+        .. versionadded:: 2.3
     bot: :class:`bool`
         Specifies if the user is a bot account.
     system: :class:`bool`
         Specifies if the user is a system user (i.e. represents Discord officially).
     """
 
     __slots__ = ('__weakref__',)
 
     def __repr__(self) -> str:
-        return f'<User id={self.id} name={self.name!r} discriminator={self.discriminator!r} bot={self.bot}>'
+        return f'<User id={self.id} name={self.name!r} global_name={self.global_name!r} bot={self.bot}>'
 
     async def _get_channel(self) -> DMChannel:
         ch = await self.create_dm()
         return ch
 
     @property
     def dm_channel(self) -> Optional[DMChannel]:
```

### Comparing `discord.py-2.2.3/discord/utils.py` & `discord.py-2.3.0/discord/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     Type,
     TypeVar,
     Union,
     overload,
     TYPE_CHECKING,
 )
 import unicodedata
-from base64 import b64encode
+from base64 import b64encode, b64decode
 from bisect import bisect_left
 import datetime
 import functools
 from inspect import isawaitable as _isawaitable, signature as _signature
 from operator import attrgetter
 from urllib.parse import urlencode
 import json
@@ -96,14 +96,15 @@
     'as_chunks',
     'format_dt',
     'MISSING',
     'setup_logging',
 )
 
 DISCORD_EPOCH = 1420070400000
+DEFAULT_FILE_SIZE_LIMIT_BYTES = 26214400
 
 
 class _MissingSentinel:
     __slots__ = ()
 
     def __eq__(self, other) -> bool:
         return False
@@ -624,14 +625,18 @@
 def _bytes_to_base64_data(data: bytes) -> str:
     fmt = 'data:{mime};base64,{data}'
     mime = _get_mime_type_for_image(data)
     b64 = b64encode(data).decode('ascii')
     return fmt.format(mime=mime, data=b64)
 
 
+def _base64_to_bytes(data: str) -> bytes:
+    return b64decode(data.encode('ascii'))
+
+
 def _is_submodule(parent: str, child: str) -> bool:
     return parent == child or child.startswith(parent + '.')
 
 
 if HAS_ORJSON:
 
     def _to_json(obj: Any) -> str:
@@ -896,15 +901,15 @@
 
 _MARKDOWN_ESCAPE_COMMON = r'^>(?:>>)?\s|\[.+\]\(.+\)'
 
 _MARKDOWN_ESCAPE_REGEX = re.compile(fr'(?P<markdown>{_MARKDOWN_ESCAPE_SUBREGEX}|{_MARKDOWN_ESCAPE_COMMON})', re.MULTILINE)
 
 _URL_REGEX = r'(?P<url><[^: >]+:\/[^ >]+>|(?:https?|steam):\/\/[^\s<]+[^<.,:;\"\'\]\s])'
 
-_MARKDOWN_STOCK_REGEX = fr'(?P<markdown>[_\\~|\*`]|{_MARKDOWN_ESCAPE_COMMON})'
+_MARKDOWN_STOCK_REGEX = fr'(?P<markdown>[_\\~|\*`#-]|{_MARKDOWN_ESCAPE_COMMON})'
 
 
 def remove_markdown(text: str, *, ignore_links: bool = True) -> str:
     """A helper function that removes markdown characters.
 
     .. versionadded:: 1.7
 
@@ -1235,19 +1240,20 @@
 
 def is_docker() -> bool:
     path = '/proc/self/cgroup'
     return os.path.exists('/.dockerenv') or (os.path.isfile(path) and any('docker' in line for line in open(path)))
 
 
 def stream_supports_colour(stream: Any) -> bool:
+    is_a_tty = hasattr(stream, 'isatty') and stream.isatty()
+
     # Pycharm and Vscode support colour in their inbuilt editors
     if 'PYCHARM_HOSTED' in os.environ or os.environ.get('TERM_PROGRAM') == 'vscode':
-        return True
+        return is_a_tty
 
-    is_a_tty = hasattr(stream, 'isatty') and stream.isatty()
     if sys.platform != 'win32':
         # Docker does not consistently have a tty attached to it
         return is_a_tty or is_docker()
 
     # ANSICON checks for things like ConEmu
     # WT_SESSION checks if this is Windows Terminal
     return is_a_tty and ('ANSICON' in os.environ or 'WT_SESSION' in os.environ)
```

### Comparing `discord.py-2.2.3/discord/voice_client.py` & `discord.py-2.3.0/discord/voice_client.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/webhook/async_.py` & `discord.py-2.3.0/discord/webhook/async_.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,17 +711,17 @@
         self._thread: Snowflake = thread
 
     def _get_guild(self, guild_id: Optional[int]) -> Optional[Guild]:
         if self._parent is not None:
             return self._parent._get_guild(guild_id)
         return None
 
-    def store_user(self, data: Union[UserPayload, PartialUserPayload]) -> BaseUser:
+    def store_user(self, data: Union[UserPayload, PartialUserPayload], *, cache: bool = True) -> BaseUser:
         if self._parent is not None:
-            return self._parent.store_user(data)
+            return self._parent.store_user(data, cache=cache)
         # state parameter is artificial
         return BaseUser(state=self, data=data)  # type: ignore
 
     def create_user(self, data: Union[UserPayload, PartialUserPayload]) -> BaseUser:
         # state parameter is artificial
         return BaseUser(state=self, data=data)  # type: ignore
 
@@ -1271,15 +1271,15 @@
 
         Returns
         --------
         :class:`Webhook`
             A partial :class:`Webhook`.
             A partial webhook is just a webhook object with an ID and a token.
         """
-        m = re.search(r'discord(?:app)?\.com/api/webhooks/(?P<id>[0-9]{17,20})/(?P<token>[A-Za-z0-9\.\-\_]{60,68})', url)
+        m = re.search(r'discord(?:app)?\.com/api/webhooks/(?P<id>[0-9]{17,20})/(?P<token>[A-Za-z0-9\.\-\_]{60,})', url)
         if m is None:
             raise ValueError('Invalid webhook URL given.')
 
         state = None
         if client is not MISSING:
             state = client._connection
             if session is MISSING:
@@ -1297,15 +1297,21 @@
         name = f"{channel.guild} #{channel}"
         feed: WebhookPayload = {
             'id': data['webhook_id'],
             'type': 2,
             'name': name,
             'channel_id': channel.id,
             'guild_id': channel.guild.id,
-            'user': {'username': user.name, 'discriminator': user.discriminator, 'id': user.id, 'avatar': user._avatar},
+            'user': {
+                'username': user.name,
+                'discriminator': user.discriminator,
+                'global_name': user.global_name,
+                'id': user.id,
+                'avatar': user._avatar,
+            },
         }
 
         state = channel._state
         http = state.http
         session = http._HTTPClient__session
         proxy_auth = http.proxy_auth
         proxy = http.proxy
```

### Comparing `discord.py-2.2.3/discord/webhook/sync.py` & `discord.py-2.3.0/discord/webhook/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -632,17 +632,17 @@
             auto session creation functions are used instead.
         bot_token: Optional[:class:`str`]
             The bot authentication token for authenticated requests
             involving the webhook.
 
         Returns
         --------
-        :class:`Webhook`
-            A partial :class:`Webhook`.
-            A partial webhook is just a webhook object with an ID and a token.
+        :class:`SyncWebhook`
+            A partial :class:`SyncWebhook`.
+            A partial :class:`SyncWebhook` is just a :class:`SyncWebhook` object with an ID and a token.
         """
         data: WebhookPayload = {
             'id': id,
             'type': 1,
             'token': token,
         }
         import requests
@@ -674,19 +674,19 @@
         Raises
         -------
         ValueError
             The URL is invalid.
 
         Returns
         --------
-        :class:`Webhook`
-            A partial :class:`Webhook`.
-            A partial webhook is just a webhook object with an ID and a token.
+        :class:`SyncWebhook`
+            A partial :class:`SyncWebhook`.
+            A partial :class:`SyncWebhook` is just a :class:`SyncWebhook` object with an ID and a token.
         """
-        m = re.search(r'discord(?:app)?\.com/api/webhooks/(?P<id>[0-9]{17,20})/(?P<token>[A-Za-z0-9\.\-\_]{60,68})', url)
+        m = re.search(r'discord(?:app)?\.com/api/webhooks/(?P<id>[0-9]{17,20})/(?P<token>[A-Za-z0-9\.\-\_]{60,})', url)
         if m is None:
             raise ValueError('Invalid webhook URL given.')
 
         data: Dict[str, Any] = m.groupdict()
         data['type'] = 1
         import requests
```

### Comparing `discord.py-2.2.3/discord/welcome_screen.py` & `discord.py-2.3.0/discord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/discord/widget.py` & `discord.py-2.3.0/discord/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,30 +117,34 @@
 
         .. describe:: hash(x)
 
             Return the widget member's hash.
 
         .. describe:: str(x)
 
-            Returns the widget member's ``name#discriminator``.
+            Returns the widget member's handle (e.g. ``name`` or ``name#discriminator``).
 
     Attributes
     -----------
     id: :class:`int`
         The member's ID.
     name: :class:`str`
         The member's username.
     discriminator: :class:`str`
-        The member's discriminator.
+        The member's discriminator. This is a legacy concept that is no longer used.
+    global_name: Optional[:class:`str`]
+        The member's global nickname, taking precedence over the username in display.
+
+        .. versionadded:: 2.3
     bot: :class:`bool`
         Whether the member is a bot.
     status: :class:`Status`
         The member's status.
     nick: Optional[:class:`str`]
-        The member's nickname.
+        The member's guild-specific nickname. Takes precedence over the global name.
     avatar: Optional[:class:`str`]
         The member's avatar hash.
     activity: Optional[Union[:class:`BaseActivity`, :class:`Spotify`]]
         The member's activity.
     deafened: Optional[:class:`bool`]
         Whether the member is currently deafened.
     muted: Optional[:class:`bool`]
@@ -187,17 +191,15 @@
             activity = create_activity(game, state)
 
         self.activity: Optional[Union[BaseActivity, Spotify]] = activity
 
         self.connected_channel: Optional[WidgetChannel] = connected_channel
 
     def __repr__(self) -> str:
-        return (
-            f"<WidgetMember name={self.name!r} discriminator={self.discriminator!r}" f" bot={self.bot} nick={self.nick!r}>"
-        )
+        return f"<WidgetMember name={self.name!r} global_name={self.global_name!r}" f" bot={self.bot} nick={self.nick!r}>"
 
     @property
     def display_name(self) -> str:
         """:class:`str`: Returns the member's display name."""
         return self.nick or self.name
 
 
@@ -222,15 +224,15 @@
     -----------
     id: :class:`int`
         The guild's ID.
     name: :class:`str`
         The guild's name.
     channels: List[:class:`WidgetChannel`]
         The accessible voice channels in the guild.
-    members: List[:class:`Member`]
+    members: List[:class:`WidgetMember`]
         The online members in the guild. Offline members
         do not appear in the widget.
 
         .. note::
 
             Due to a Discord limitation, if this data is available
             the users will be "anonymized" with linear IDs and discriminator
```

### Comparing `discord.py-2.2.3/discord.py.egg-info/PKG-INFO` & `discord.py-2.3.0/discord.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord.py
-Version: 2.2.3
+Version: 2.3.0
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/Rapptz/discord.py
 Author: Rapptz
 License: MIT
 Project-URL: Documentation, https://discordpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Rapptz/discord.py/issues
 Platform: UNKNOWN
```

### Comparing `discord.py-2.2.3/discord.py.egg-info/SOURCES.txt` & `discord.py-2.3.0/discord.py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 discord/types/user.py
 discord/types/voice.py
 discord/types/webhook.py
 discord/types/welcome_screen.py
 discord/types/widget.py
 discord/ui/__init__.py
 discord/ui/button.py
-discord/ui/dynamic.py
 discord/ui/item.py
 discord/ui/modal.py
 discord/ui/select.py
 discord/ui/text_input.py
 discord/ui/view.py
 discord/webhook/__init__.py
 discord/webhook/async_.py
```

### Comparing `discord.py-2.2.3/pyproject.toml` & `discord.py-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `discord.py-2.2.3/setup.py` & `discord.py-2.3.0/setup.py`

 * *Files identical despite different names*

