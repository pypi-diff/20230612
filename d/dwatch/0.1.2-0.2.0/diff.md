# Comparing `tmp/dwatch-0.1.2.tar.gz` & `tmp/dwatch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwatch-0.1.2.tar", last modified: Tue Oct 25 09:52:21 2022, max compression
+gzip compressed data, was "dwatch-0.2.0.tar", last modified: Mon Jun 12 11:05:22 2023, max compression
```

## Comparing `dwatch-0.1.2.tar` & `dwatch-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 09:52:21.414404 dwatch-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2022-10-25 09:52:14.000000 dwatch-0.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      117 2022-10-25 09:52:14.000000 dwatch-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7064 2022-10-25 09:52:21.414404 dwatch-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5790 2022-10-25 09:52:14.000000 dwatch-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 09:52:21.414404 dwatch-0.1.2/dwatch/
--rw-rw-rw-   0 root         (0) root         (0)      330 2022-10-25 09:52:14.000000 dwatch-0.1.2/dwatch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-10-25 09:52:14.000000 dwatch-0.1.2/dwatch/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7497 2022-10-25 09:52:14.000000 dwatch-0.1.2/dwatch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5008 2022-10-25 09:52:14.000000 dwatch-0.1.2/dwatch/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3308 2022-10-25 09:52:14.000000 dwatch-0.1.2/dwatch/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3261 2022-10-25 09:52:14.000000 dwatch-0.1.2/dwatch/monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     2153 2022-10-25 09:52:14.000000 dwatch-0.1.2/dwatch/render.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2022-10-25 09:52:14.000000 dwatch-0.1.2/dwatch/report_template.jinja.html
--rw-rw-rw-   0 root         (0) root         (0)      218 2022-10-25 09:52:14.000000 dwatch-0.1.2/dwatch/report_template.jinja.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-25 09:52:21.414404 dwatch-0.1.2/dwatch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7064 2022-10-25 09:52:21.000000 dwatch-0.1.2/dwatch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      406 2022-10-25 09:52:21.000000 dwatch-0.1.2/dwatch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-25 09:52:21.000000 dwatch-0.1.2/dwatch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2022-10-25 09:52:21.000000 dwatch-0.1.2/dwatch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2022-10-25 09:52:21.000000 dwatch-0.1.2/dwatch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-10-25 09:52:21.000000 dwatch-0.1.2/dwatch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-25 09:52:21.414404 dwatch-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3973 2022-10-25 09:52:14.000000 dwatch-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:05:22.100421 dwatch-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-12 11:05:13.000000 dwatch-0.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-12 11:05:13.000000 dwatch-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7437 2023-06-12 11:05:22.100421 dwatch-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6163 2023-06-12 11:05:13.000000 dwatch-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:05:22.100421 dwatch-0.2.0/dwatch/
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-06-12 11:05:13.000000 dwatch-0.2.0/dwatch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-12 11:05:13.000000 dwatch-0.2.0/dwatch/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7770 2023-06-12 11:05:13.000000 dwatch-0.2.0/dwatch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5008 2023-06-12 11:05:13.000000 dwatch-0.2.0/dwatch/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3645 2023-06-12 11:05:13.000000 dwatch-0.2.0/dwatch/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3261 2023-06-12 11:05:13.000000 dwatch-0.2.0/dwatch/monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-06-12 11:05:13.000000 dwatch-0.2.0/dwatch/render.py
+-rw-rw-rw-   0 root         (0) root         (0)     2198 2023-06-12 11:05:13.000000 dwatch-0.2.0/dwatch/report_template.jinja.html
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-06-12 11:05:13.000000 dwatch-0.2.0/dwatch/report_template.jinja.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:05:22.100421 dwatch-0.2.0/dwatch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7437 2023-06-12 11:05:22.000000 dwatch-0.2.0/dwatch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      406 2023-06-12 11:05:22.000000 dwatch-0.2.0/dwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 11:05:22.000000 dwatch-0.2.0/dwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-12 11:05:22.000000 dwatch-0.2.0/dwatch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-12 11:05:22.000000 dwatch-0.2.0/dwatch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-12 11:05:22.000000 dwatch-0.2.0/dwatch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 11:05:22.100421 dwatch-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3965 2023-06-12 11:05:13.000000 dwatch-0.2.0/setup.py
```

### Comparing `dwatch-0.1.2/LICENSE` & `dwatch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dwatch-0.1.2/PKG-INFO` & `dwatch-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwatch
-Version: 0.1.2
+Version: 0.2.0
 Summary: A tool to watch command output for differences and send notifications.
 Home-page: https://github.com/IngoMeyer441/dwatch
 Author: Ingo Meyer
 Author-email: i.meyer@fz-juelich.de
 License: MIT
 Keywords: administration,monitoring
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,14 +76,17 @@
 
 Without `--stdout` the diff output is sent as an HTML email. By default, dwatch uses the `sendmail` tool for this, which
 is available if a local email server like Postfix or Exim is installed or if a simple mail forwarder like
 [ssmtp](https://packages.debian.org/stable/ssmtp) is present. As an alternative, dwatch supports direct communication
 with a mail server with Python's builtin [smtplib](https://docs.python.org/3/library/smtplib.html). This can be used if
 no email server is installed locally. In either case, run
 
+Use the `--description` option with a text argument to add a description to the diff report and the subject field of
+emails. This can be useful to distinguish different commands.
+
 ```bash
 dwatch --write-default-config
 ```
 
 to create a default configuration file at `~/.dwatchrc`. Open the file with a text editor and configure a sender
 `from_address` and receiver `to_address` in the `[mail]` section:
 
@@ -131,30 +134,33 @@
     cron jobs.
   - `shell`: Run the given command in a subshell. This is useful to allow shell patterns in a command like pipes (for
     example `command | grep pattern`).
 
 ## Command line options
 
 ```text
-usage: dwatch [-h] [-i INTERVAL] [-o | -O] [-s | -S] [--stdout] [-V] [-w]
-              [-q | --error | --warn | -v | --debug]
+usage: dwatch [-h] [-d DESCRIPTION] [-i INTERVAL] [-o | -O] [-s | -S]
+              [--stdout] [-V] [-w] [-q | --error | --warn | -v | --debug]
               [command]
 
 dwatch is a tool for watching command output for changes and notifiying the
 user. Default values for command line options are taken from the config file
 at "~/.dwatchrc"
 
 positional arguments:
   command               the command to watch
 
 options:
   -h, --help            show this help message and exit
+  -d DESCRIPTION, --description DESCRIPTION
+                        add a description which is added to the diff output
+                        and used in the e-mail subject
   -i INTERVAL, --interval INTERVAL
                         set the interval for the watched command (default:
-                        "2.0")
+                        "60.0")
   -o, --run-once        run the given command once and exit (default: "False")
   -O, --no-run-once     don't run the given command once and exit (default:
                         "True")
   -s, --shell           run the given command in a shell subprocess (default:
                         "False")
   -S, --no-shell        don't run the given command in a shell subprocess
                         (default: "True")
```

### Comparing `dwatch-0.1.2/README.md` & `dwatch-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 
 Without `--stdout` the diff output is sent as an HTML email. By default, dwatch uses the `sendmail` tool for this, which
 is available if a local email server like Postfix or Exim is installed or if a simple mail forwarder like
 [ssmtp](https://packages.debian.org/stable/ssmtp) is present. As an alternative, dwatch supports direct communication
 with a mail server with Python's builtin [smtplib](https://docs.python.org/3/library/smtplib.html). This can be used if
 no email server is installed locally. In either case, run
 
+Use the `--description` option with a text argument to add a description to the diff report and the subject field of
+emails. This can be useful to distinguish different commands.
+
 ```bash
 dwatch --write-default-config
 ```
 
 to create a default configuration file at `~/.dwatchrc`. Open the file with a text editor and configure a sender
 `from_address` and receiver `to_address` in the `[mail]` section:
 
@@ -99,30 +102,33 @@
     cron jobs.
   - `shell`: Run the given command in a subshell. This is useful to allow shell patterns in a command like pipes (for
     example `command | grep pattern`).
 
 ## Command line options
 
 ```text
-usage: dwatch [-h] [-i INTERVAL] [-o | -O] [-s | -S] [--stdout] [-V] [-w]
-              [-q | --error | --warn | -v | --debug]
+usage: dwatch [-h] [-d DESCRIPTION] [-i INTERVAL] [-o | -O] [-s | -S]
+              [--stdout] [-V] [-w] [-q | --error | --warn | -v | --debug]
               [command]
 
 dwatch is a tool for watching command output for changes and notifiying the
 user. Default values for command line options are taken from the config file
 at "~/.dwatchrc"
 
 positional arguments:
   command               the command to watch
 
 options:
   -h, --help            show this help message and exit
+  -d DESCRIPTION, --description DESCRIPTION
+                        add a description which is added to the diff output
+                        and used in the e-mail subject
   -i INTERVAL, --interval INTERVAL
                         set the interval for the watched command (default:
-                        "2.0")
+                        "60.0")
   -o, --run-once        run the given command once and exit (default: "False")
   -O, --no-run-once     don't run the given command once and exit (default:
                         "True")
   -s, --shell           run the given command in a shell subprocess (default:
                         "False")
   -S, --no-shell        don't run the given command in a shell subprocess
                         (default: "True")
```

### Comparing `dwatch-0.1.2/dwatch/cli.py` & `dwatch-0.2.0/dwatch/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,21 @@
 %(prog)s is a tool for watching command output for changes and notifiying the user.
 Default values for command line options are taken from the config file at "{}"
 """.format(
             CONFIG_FILEPATH
         ),
     )
     parser.add_argument(
+        "-d",
+        "--description",
+        action="store",
+        dest="description",
+        help="add a description which is added to the diff output and used in the e-mail subject",
+    )
+    parser.add_argument(
         "-i",
         "--interval",
         action="store",
         default=config.interval,
         type=float,
         dest="interval",
         help='set the interval for the watched command (default: "%(default)s")',
@@ -175,15 +182,15 @@
         command = [args.command]
     else:
         command = shlex.split(args.command)
     for original_command_output, compare_command_output in watch(command, args.shell, args.run_once, args.interval):
         if args.print_on_stdout:
             logger.info("Write command diff to stdout:")
             report_plain = render_template(
-                TemplateType.PLAIN, args.command, original_command_output, compare_command_output
+                TemplateType.PLAIN, args.command, original_command_output, compare_command_output, args.description
             )
             print(report_plain)
             print()
         else:
             logger.info("Generate an HTML diff and send a mail")
             send_mail(
                 args.command,
@@ -192,14 +199,15 @@
                 config.mail_backend,
                 config.mail_from_address,
                 config.mail_to_addresses,
                 config.mail_server,
                 config.mail_encryption,
                 config.mail_login_user,
                 config.mail_login_password,
+                args.description,
             )
 
 
 def main() -> None:
     expected_exceptions = (MailError,)
     try:
         args = parse_arguments()
```

### Comparing `dwatch-0.1.2/dwatch/config.py` & `dwatch-0.2.0/dwatch/config.py`

 * *Files identical despite different names*

### Comparing `dwatch-0.1.2/dwatch/mail.py` & `dwatch-0.2.0/dwatch/mail.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from email.mime.text import MIMEText
 from enum import Enum, auto
 from typing import Iterable, Optional, Type
 
 from .monitor import CommandOutput
 from .render import TemplateType, render_template
 
-MAIL_SUBJECT = "Change detected on watched command output"
+MAIL_SUBJECT_WITH_DESCRIPTION = "{description:s}: change detected"
+MAIL_SUBJECT_WITHOUT_DESCRIPTION = "Change detected on watched command output"
 
 logger = logging.getLogger(__name__)
 
 
 class MailBackend(Enum):
     SENDMAIL = auto()
     SMTPLIB = auto()
@@ -42,26 +43,27 @@
     mail_backend: MailBackend,
     from_address: str,
     to_addresses: Iterable[str],
     mail_server_url: str,
     encryption: MailEncryption,
     login_user: Optional[str] = None,
     login_password: Optional[str] = None,
+    command_description: Optional[str] = None,
 ) -> None:
     def use_sendmail(message: MIMEMultipart) -> None:
         logging.debug("Send mail with sendmail")
         try:
             subprocess.run(["/usr/sbin/sendmail", "-t", "-oi"], input=message.as_bytes(), check=True)
         except subprocess.CalledProcessError as e:
             raise MailError("Could not send mail.") from e
 
     def use_smtplib(message: MIMEMultipart) -> None:
         logging.debug('Send mail with Python\'s builtin smtplib, encryption: "%s"', encryption.name)
         if encryption is MailEncryption.SSL:
-            smtp_class = smtplib.SMTP_SSL  # type: Type[smtplib.SMTP]
+            smtp_class: Type[smtplib.SMTP] = smtplib.SMTP_SSL
             port = MailPorts.SSL
         elif encryption is MailEncryption.STARTTLS:
             smtp_class = smtplib.SMTP
             port = MailPorts.STARTTLS
         else:
             smtp_class = smtplib.SMTP
             port = MailPorts.PLAIN
@@ -86,16 +88,19 @@
         MailBackend.SENDMAIL: use_sendmail,
         MailBackend.SMTPLIB: use_smtplib,
     }
 
     message = MIMEMultipart("alternative")
     message["From"] = from_address
     message["To"] = ", ".join(to_addresses)
-    message["Subject"] = MAIL_SUBJECT
-    content_plain = render_template(TemplateType.PLAIN, command, original_text, compare_text)
-    content_html = render_template(TemplateType.HTML, command, original_text, compare_text)
+    if command_description is None:
+        message["Subject"] = MAIL_SUBJECT_WITHOUT_DESCRIPTION
+    else:
+        message["Subject"] = MAIL_SUBJECT_WITH_DESCRIPTION.format(description=command_description)
+    content_plain = render_template(TemplateType.PLAIN, command, original_text, compare_text, command_description)
+    content_html = render_template(TemplateType.HTML, command, original_text, compare_text, command_description)
     message_part_plain = MIMEText(content_plain, "plain", _charset="utf-8")
     message_part_html = MIMEText(content_html, "html", _charset="utf-8")
     message.attach(message_part_plain)
     message.attach(message_part_html)
 
     backend_to_func[mail_backend](message)
```

### Comparing `dwatch-0.1.2/dwatch/monitor.py` & `dwatch-0.2.0/dwatch/monitor.py`

 * *Files identical despite different names*

### Comparing `dwatch-0.1.2/dwatch/render.py` & `dwatch-0.2.0/dwatch/render.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 from difflib import HtmlDiff, unified_diff
 from enum import Enum, auto
+from typing import Optional
 
 import jinja2
 
 from .monitor import CommandOutput
 
 NUM_CONTEXT_LINES = 3
 HTML_TABSIZE = 4
@@ -23,22 +24,24 @@
 
 
 def render_template(
     template_type: TemplateType,
     command: str,
     original_command_output: CommandOutput,
     compare_command_output: CommandOutput,
+    description: Optional[str] = None,
 ) -> str:
     template = jinja2.Environment(loader=jinja2.FileSystemLoader(os.path.dirname(__file__))).get_template(
         HTML_TEMPLATE_FILENAME if template_type is TemplateType.HTML else PLAIN_TEMPLATE_FILENAME
     )
     jinja_data = {
         "command": command.strip(),
         "original_text": original_command_output.output.rstrip(),
         "compare_text": compare_command_output.output.rstrip(),
+        "description": description,
     }
     if template_type is TemplateType.HTML:
         logging.debug("Render HTML diff")
         html_diff = HtmlDiff(tabsize=HTML_TABSIZE, wrapcolumn=HTML_WRAPCOLUMN)
         html_table = html_diff.make_table(
             original_command_output.output.splitlines(keepends=True),
             compare_command_output.output.splitlines(keepends=True),
```

### Comparing `dwatch-0.1.2/dwatch/report_template.jinja.html` & `dwatch-0.2.0/dwatch/report_template.jinja.html`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,18 @@
       white-space: pre;
     }
   </style>
 </head>
 
 <body>
   <h1>Diff report</h1>
+  {% if description is not none -%}
+  <h2>Description</h2>
+  <p>{{ description }}</p>
+  {% endif -%}
   <h2>Command</h2>
   <pre>
 {%- for line in command.splitlines() -%}
 <span class="line-number"></span><code>{{- line -}}</code>
 {% endfor -%}
 </pre>
   <h2>Command output differences</h2>
```

#### html2text {}

```diff
@@ -1,8 +1,12 @@
 ****** Diff report ******
+{% if description is not none -%}
+***** Description *****
+{{ description }}
+{% endif -%}
 ***** Command *****
 {%- for line in command.splitlines() -%}
 {{- line -}}
 {% endfor -%}
 ***** Command output differences *****
 {{ diff_table }}
 ***** Full previous command output *****
```

### Comparing `dwatch-0.1.2/dwatch.egg-info/PKG-INFO` & `dwatch-0.2.0/dwatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwatch
-Version: 0.1.2
+Version: 0.2.0
 Summary: A tool to watch command output for differences and send notifications.
 Home-page: https://github.com/IngoMeyer441/dwatch
 Author: Ingo Meyer
 Author-email: i.meyer@fz-juelich.de
 License: MIT
 Keywords: administration,monitoring
 Classifier: Development Status :: 5 - Production/Stable
@@ -76,14 +76,17 @@
 
 Without `--stdout` the diff output is sent as an HTML email. By default, dwatch uses the `sendmail` tool for this, which
 is available if a local email server like Postfix or Exim is installed or if a simple mail forwarder like
 [ssmtp](https://packages.debian.org/stable/ssmtp) is present. As an alternative, dwatch supports direct communication
 with a mail server with Python's builtin [smtplib](https://docs.python.org/3/library/smtplib.html). This can be used if
 no email server is installed locally. In either case, run
 
+Use the `--description` option with a text argument to add a description to the diff report and the subject field of
+emails. This can be useful to distinguish different commands.
+
 ```bash
 dwatch --write-default-config
 ```
 
 to create a default configuration file at `~/.dwatchrc`. Open the file with a text editor and configure a sender
 `from_address` and receiver `to_address` in the `[mail]` section:
 
@@ -131,30 +134,33 @@
     cron jobs.
   - `shell`: Run the given command in a subshell. This is useful to allow shell patterns in a command like pipes (for
     example `command | grep pattern`).
 
 ## Command line options
 
 ```text
-usage: dwatch [-h] [-i INTERVAL] [-o | -O] [-s | -S] [--stdout] [-V] [-w]
-              [-q | --error | --warn | -v | --debug]
+usage: dwatch [-h] [-d DESCRIPTION] [-i INTERVAL] [-o | -O] [-s | -S]
+              [--stdout] [-V] [-w] [-q | --error | --warn | -v | --debug]
               [command]
 
 dwatch is a tool for watching command output for changes and notifiying the
 user. Default values for command line options are taken from the config file
 at "~/.dwatchrc"
 
 positional arguments:
   command               the command to watch
 
 options:
   -h, --help            show this help message and exit
+  -d DESCRIPTION, --description DESCRIPTION
+                        add a description which is added to the diff output
+                        and used in the e-mail subject
   -i INTERVAL, --interval INTERVAL
                         set the interval for the watched command (default:
-                        "2.0")
+                        "60.0")
   -o, --run-once        run the given command once and exit (default: "False")
   -O, --no-run-once     don't run the given command once and exit (default:
                         "True")
   -s, --shell           run the given command in a shell subprocess (default:
                         "False")
   -S, --no-shell        don't run the given command in a shell subprocess
                         (default: "True")
```

### Comparing `dwatch-0.1.2/setup.py` & `dwatch-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List, Optional, Tuple, cast
 
 from setuptools import find_packages, setup
 
 
 class PyinstallerCommand(Command):
     description = "create a self-contained executable with PyInstaller"
-    user_options = []  # type: List[Tuple[str, Optional[str], str]]
+    user_options: List[Tuple[str, Optional[str], str]] = []
 
     def initialize_options(self) -> None:
         pass
 
     def finalize_options(self) -> None:
         pass
```

