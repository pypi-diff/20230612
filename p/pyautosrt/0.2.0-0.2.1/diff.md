# Comparing `tmp/pyautosrt-0.2.0.tar.gz` & `tmp/pyautosrt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautosrt-0.2.0.tar", last modified: Sun Jun 11 03:32:43 2023, max compression
+gzip compressed data, was "pyautosrt-0.2.1.tar", last modified: Mon Jun 12 04:42:11 2023, max compression
```

## Comparing `pyautosrt-0.2.0.tar` & `pyautosrt-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 03:32:43.507923 pyautosrt-0.2.0/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2055 2023-06-11 03:32:43.507923 pyautosrt-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 03:32:43.482449 pyautosrt-0.2.0/pyautosrt/
--rw-rw-rw-   0        0        0   196913 2023-06-11 03:32:32.000000 pyautosrt-0.2.0/pyautosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 03:32:43.502680 pyautosrt-0.2.0/pyautosrt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-06-11 03:32:43.000000 pyautosrt-0.2.0/pyautosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-11 03:32:43.000000 pyautosrt-0.2.0/pyautosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 03:32:43.000000 pyautosrt-0.2.0/pyautosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-11 03:32:43.000000 pyautosrt-0.2.0/pyautosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-11 03:32:43.000000 pyautosrt-0.2.0/pyautosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-11 03:32:43.000000 pyautosrt-0.2.0/pyautosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-11 03:32:43.510920 pyautosrt-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1850 2023-06-11 02:57:09.000000 pyautosrt-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 03:32:43.505675 pyautosrt-0.2.0/test/
--rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.0/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:42:11.062891 pyautosrt-0.2.1/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2055 2023-06-12 04:42:11.063642 pyautosrt-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 04:42:11.011197 pyautosrt-0.2.1/pyautosrt/
+-rw-rw-rw-   0        0        0   213024 2023-06-12 04:41:04.000000 pyautosrt-0.2.1/pyautosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:42:11.046412 pyautosrt-0.2.1/pyautosrt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-12 04:42:10.000000 pyautosrt-0.2.1/pyautosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-12 04:42:11.066639 pyautosrt-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1850 2023-06-11 02:57:09.000000 pyautosrt-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 04:42:11.061396 pyautosrt-0.2.1/test/
+-rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.1/test/__init__.py
```

### Comparing `pyautosrt-0.2.0/LICENSE` & `pyautosrt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.0/PKG-INFO` & `pyautosrt-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.0
+Version: 0.2.1
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.0/README.md` & `pyautosrt-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.0/pyautosrt/__init__.py` & `pyautosrt-0.2.1/pyautosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import shlex
 
 #import warnings
 #warnings.filterwarnings("ignore", category=DeprecationWarning)
 #warnings.filterwarnings("ignore", category=RuntimeWarning)
 #sys.tracebacklimit = 0
 
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 
 
 #======================================================== ffmpeg_progress_yield ========================================================#
 
 
 import re
 #import subprocess
@@ -1669,15 +1669,14 @@
             media_filepath = media_filepath.replace("\\", "/")
         subtitle_streams = self.get_subtitle_streams(media_filepath)
         subtitle_streams_data = []
         if subtitle_streams:
             for subtitle_stream in subtitle_streams:
                 subtitle_stream_index = subtitle_stream['index']
                 subtitle_stream_language = subtitle_stream['language']
-                #print(f"Stream Index: {subtitle_stream_index}, Language: {subtitle_stream_language}")
                 subtitle_streams_data.append((subtitle_stream_index, subtitle_stream_language))
 
         subtitle_data = []
         subtitle_contents = []
 
         for subtitle_stream_index in range(len(subtitle_streams)):
             index, language = subtitle_streams_data[subtitle_stream_index]
@@ -1745,20 +1744,18 @@
                         '-f', 'srt',
                         '-'
                      ]
 
         try:
             result = subprocess.run(ffmpeg_cmd, capture_output=True, text=True)
             output = result.stdout
-			#print(output)
 
             timed_subtitles = []
             subtitle_data = []
             lines = output.strip().split('\n')
-            #print(lines)
             subtitles = []
             subtitle = None
             subtitle_blocks = []
             block = []
             for line in lines:
                 if line.strip() == '':
                     subtitle_blocks.append(block)
@@ -2091,14 +2088,139 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
+class MediaSubtitleRemover:
+    @staticmethod
+    def which(program):
+        def is_exe(media_filepath):
+            return os.path.isfile(media_filepath) and os.access(media_filepath, os.X_OK)
+        fpath, _ = os.path.split(program)
+        if fpath:
+            if is_exe(program):
+                return program
+        else:
+            for path in os.environ["PATH"].split(os.pathsep):
+                path = path.strip('"')
+                exe_file = os.path.join(path, program)
+                if is_exe(exe_file):
+                    return exe_file
+        return None
+
+    @staticmethod
+    def ffmpeg_check():
+        if MediaSubtitleRemover.which("ffmpeg"):
+            return "ffmpeg"
+        if MediaSubtitleRemover.which("ffmpeg.exe"):
+            return "ffmpeg.exe"
+        return None
+
+    def __init__(self, output_path=None, progress_callback=None, error_messages_callback=None):
+        self.output_path = output_path
+        self.progress_callback = progress_callback
+        self.error_messages_callback = error_messages_callback
+
+    def __call__(self, media_filepath):
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
+        if "\\" in self.output_path:
+            self.output_path = self.output_path.replace("\\", "/")
+
+        if not os.path.isfile(media_filepath):
+            if self.error_messages_callback:
+                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+            else:
+                print("The given file does not exist: {0}".format(media_filepath))
+                raise Exception("Invalid file: {0}".format(media_filepath))
+        if not self.ffmpeg_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("ffmpeg: Executable not found on machine.")
+            else:
+                print("ffmpeg: Executable not found on machine.")
+                raise Exception("Dependency not found: ffmpeg")
+
+        try:
+            ffmpeg_command = [
+                                'ffmpeg',
+                                '-y',
+                                '-i', media_filepath,
+                                '-c', 'copy',
+                                '-sn',
+                                self.output_path
+                             ]
+
+            info = "Removing subtitle streams from file"
+            start_time = time.time()
+
+            # USING ffmpeg_progress_yield MODULE
+            ff = FfmpegProgress(ffmpeg_command)
+            percentage = 0
+            for progress in ff.run_command_with_progress():
+                percentage = progress
+                if self.progress_callback:
+                    self.progress_callback(info, media_filepath, percentage, start_time)
+
+            '''
+            # WITHOUT USING ffmpeg_progress_yield MODULE
+            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+            else:
+                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+
+            if sys.platform == "win32":
+                process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+            else:
+                process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+
+            info = "Removing subtitle streams from file"
+            for line in process.stdout:
+                if "time=" in line:
+                    #print(line)
+                    time_str = line.split("time=")[1].split()[0]
+                    #print("time_str = %s" %time_str)
+                    current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+                    #print("current_duration = %s" %current_duration)
+                    if current_duration>0:
+                        percentage = int(current_duration*100/total_duration)
+                        if self.progress_callback:
+                            self.progress_callback(info, media_filepath, percentage)
+            '''
+
+            if os.path.isfile(self.output_path):
+                return self.output_path
+            else:
+                return None
+
+            if os.path.isfile(self.output_path):
+                return self.output_path
+            else:
+                return None
+
+        except KeyboardInterrupt:
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
+            return
+
+        except Exception as e:
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
+            return
+
+
 #=======================================================================================================================================#
 
 #----------------------------------------------------------- MISC FUNCTIONS -----------------------------------------------------------#
 
 
 '''
 from autosrt import Language, WavConverter,  SpeechRegionFinder, FLACConverter, SpeechRecognizer, SentenceTranslator, \
@@ -2206,15 +2328,15 @@
             super().run()
         except Exception as e:
             self.queue.put(('error', str(e)))
         else:
             self.queue.put(('done', None))
 
 
-def is_streaming_url(url):
+def is_streaming_url(url, error_messages_callback=None):
 
     streamlink = Streamlink()
 
     if is_valid_url(url):
         #print("is_valid_url(url) = {}".format(is_valid_url(url)))
         try:
             os.environ['STREAMLINK_DIR'] = './streamlink/'
@@ -2227,159 +2349,201 @@
                 return True
             else:
                 #print("is_streams = {}".format(False))
                 return False
 
         except OSError:
             #print("is_streams = OSError")
+            if error_messages_callback:
+                error_messages_callback("OSError")
             return False
         except ValueError:
             #print("is_streams = ValueError")
+            if error_messages_callback:
+                error_messages_callback("ValueError")
             return False
         except KeyError:
             #print("is_streams = KeyError")
+            if error_messages_callback:
+                error_messages_callback("KeyError")
             return False
         except RuntimeError:
             #print("is_streams = RuntimeError")
+            if error_messages_callback:
+                error_messages_callback("RuntimeError")
             return False
         except NoPluginError:
             #print("is_streams = NoPluginError")
+            if error_messages_callback:
+                error_messages_callback("NoPluginError")
             return False
         except StreamlinkError:
             return False
             #print("is_streams = StreamlinkError")
+            if error_messages_callback:
+                error_messages_callback("StreamlinkError")
         except StreamError:
             return False
             #print("is_streams = StreamlinkError")
+            if error_messages_callback:
+                error_messages_callback("StreamError")
         except NotImplementedError:
             #print("is_streams = NotImplementedError")
+            if error_messages_callback:
+                error_messages_callback("NotImplementedError")
             return False
         except Exception as e:
             #print("is_streams = {}".format(e))
+            if error_messages_callback:
+                error_messages_callback(e)
             return False
     else:
         #print("is_valid_url(url) = {}".format(is_valid_url(url)))
         return False
 
 
-def is_valid_url(url):
+def is_valid_url(url, error_messages_callback=None):
     try:
         response = httpx.head(url)
         response.raise_for_status()
         return True
-    except (httpx.HTTPError, ValueError):
+    except (httpx.HTTPError, ValueError) as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return False
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
         return False
 
 
-def record_streaming_windows(hls_url, media_filepath):
+def record_streaming_windows(hls_url, media_filepath, error_messages_callback=None):
     global not_recording, main_window
 
-    ffmpeg_cmd = ['ffmpeg', '-y', '-i', hls_url,  '-movflags', '+frag_keyframe+separate_moof+omit_tfhd_offset+empty_moov', '-fflags', 'nobuffer', media_filepath]
-    process = subprocess.Popen(ffmpeg_cmd, stderr=subprocess.PIPE, creationflags=subprocess.CREATE_NO_WINDOW)
-    msg = "RECORDING"
-    main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
-
-    while not not_recording:
-        if not_recording:
-            break
-
-        for line in iter(process.stderr.readline, b''):
-            line = line.decode('utf-8').rstrip()
-
-            if 'time=' in line:
-                time_str = line.split('time=')[1].split()[0]
-                streaming_duration_recorded = datetime.strptime(time_str, "%H:%M:%S.%f") - datetime(1900, 1, 1)
-                main_window.write_event_value('-EVENT-STREAMING-DURATION-RECORDED-', streaming_duration_recorded)
+    try:
+        ffmpeg_cmd = ['ffmpeg', '-y', '-i', hls_url,  '-movflags', '+frag_keyframe+separate_moof+omit_tfhd_offset+empty_moov', '-fflags', 'nobuffer', media_filepath]
+        process = subprocess.Popen(ffmpeg_cmd, stderr=subprocess.PIPE, creationflags=subprocess.CREATE_NO_WINDOW)
+        msg = "RECORDING"
+        main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
+
+        while not not_recording:
+            if not_recording:
+                break
+
+            for line in iter(process.stderr.readline, b''):
+                line = line.decode('utf-8').rstrip()
+
+                if 'time=' in line:
+                    time_str = line.split('time=')[1].split()[0]
+                    streaming_duration_recorded = datetime.strptime(time_str, "%H:%M:%S.%f") - datetime(1900, 1, 1)
+                    main_window.write_event_value('-EVENT-STREAMING-DURATION-RECORDED-', streaming_duration_recorded)
 
-    process.wait()
+        process.wait()
+
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
 
 
 # subprocess.Popen(ffmpeg_cmd) THREAD BEHAVIOR IS DIFFERENT IN LINUX
-def record_streaming_linux(url, output_file):
+def record_streaming_linux(url, output_file, error_messages_callback=None):
     global recognizing, ffmpeg_start_run_time, first_streaming_duration_recorded, main_window
 
     #ffmpeg_cmd = ['ffmpeg', '-y', '-i', url, '-c', 'copy', '-bsf:a', 'aac_adtstoasc', '-f', 'mp4', output_file]
     ffmpeg_cmd = ['ffmpeg', '-y', '-i', f'{url}',  '-movflags', '+frag_keyframe+separate_moof+omit_tfhd_offset+empty_moov', '-fflags', 'nobuffer', f'{output_file}']
 
     ffmpeg_start_run_time = datetime.now()
 
     # Define a function to run the ffmpeg process in a separate thread
     def run_ffmpeg():
-        i = 0
-        line = None
+        try:
+            i = 0
+            line = None
 
-        process = subprocess.Popen(ffmpeg_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
+            process = subprocess.Popen(ffmpeg_cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
 
-        msg = "RECORDING"
-        main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
+            msg = "RECORDING"
+            main_window.write_event_value('-EVENT-THREAD-RECORD-STREAMING-STATUS-', msg)
 
-        # Set up a timer to periodically check for new output
-        timeout = 1.0
-        timer = Timer(timeout, lambda: None)
-        timer.start()
+            # Set up a timer to periodically check for new output
+            timeout = 1.0
+            timer = Timer(timeout, lambda: None)
+            timer.start()
 
-        # Read output from ffmpeg process
-        while not not_recording:
-            # Check if the process has finished
-            if process.poll() is not None:
-                break
+            # Read output from ffmpeg process
+            while not not_recording:
+                # Check if the process has finished
+                if process.poll() is not None:
+                    break
 
-            # Check if there is new output to read, special for linux
-            rlist, _, _ = select.select([process.stderr], [], [], timeout)
-            if not rlist:
-                continue
+                # Check if there is new output to read, special for linux
+                rlist, _, _ = select.select([process.stderr], [], [], timeout)
+                if not rlist:
+                    continue
 
-            # Read the new output and print it
-            line = rlist[0].readline().strip()
-            #print(line)
-
-            # Search for the time information in the output and print it
-            time_str = re.search(r'time=(\d+:\d+:\d+\.\d+)', line)
-
-            if time_str:
-                time_value = time_str.group(1)
-                #print(f"Time: {time_value}")
-
-                if i == 0:
-                    ffmpeg_start_write_time = datetime.now()
-                    #print("ffmpeg_start_write_time = {}".format(ffmpeg_start_write_time))
-
-                    first_streaming_duration_recorded = datetime.strptime(str(time_value), "%H:%M:%S.%f") - datetime(1900, 1, 1)
-                    #print("first_streaming_duration_recorded = {}".format(first_streaming_duration_recorded))
-
-                    # MAKE SURE THAT first_streaming_duration_recorded EXECUTED ONLY ONCE
-                    i += 1
-
-                    #print("writing time_value")
-                    time_value_filename = "time_value"
-                    time_value_filepath = os.path.join(tempfile.gettempdir(), time_value_filename)
-                    time_value_file = open(time_value_filepath, "w")
-                    time_value_file.write(str(time_value))
-                    time_value_file.close()
-                    #print("time_value = {}".format(time_value))
-
-                streaming_duration_recorded = datetime.strptime(str(time_value), "%H:%M:%S.%f") - datetime(1900, 1, 1)
-                #print("streaming_duration_recorded = {}".format(streaming_duration_recorded))
-                main_window.write_event_value('-EVENT-STREAMING-DURATION-RECORDED-', streaming_duration_recorded)
+                # Read the new output and print it
+                line = rlist[0].readline().strip()
+                #print(line)
+
+                # Search for the time information in the output and print it
+                time_str = re.search(r'time=(\d+:\d+:\d+\.\d+)', line)
+
+                if time_str:
+                    time_value = time_str.group(1)
+                    #print(f"Time: {time_value}")
+
+                    if i == 0:
+                        ffmpeg_start_write_time = datetime.now()
+                        #print("ffmpeg_start_write_time = {}".format(ffmpeg_start_write_time))
+
+                        first_streaming_duration_recorded = datetime.strptime(str(time_value), "%H:%M:%S.%f") - datetime(1900, 1, 1)
+                        #print("first_streaming_duration_recorded = {}".format(first_streaming_duration_recorded))
+
+                        # MAKE SURE THAT first_streaming_duration_recorded EXECUTED ONLY ONCE
+                        i += 1
+
+                        #print("writing time_value")
+                        time_value_filename = "time_value"
+                        time_value_filepath = os.path.join(tempfile.gettempdir(), time_value_filename)
+                        time_value_file = open(time_value_filepath, "w")
+                        time_value_file.write(str(time_value))
+                        time_value_file.close()
+                        #print("time_value = {}".format(time_value))
+
+                    streaming_duration_recorded = datetime.strptime(str(time_value), "%H:%M:%S.%f") - datetime(1900, 1, 1)
+                    #print("streaming_duration_recorded = {}".format(streaming_duration_recorded))
+                    main_window.write_event_value('-EVENT-STREAMING-DURATION-RECORDED-', streaming_duration_recorded)
+
+                # Restart the timer to check for new output
+                timer.cancel()
+                timer = Timer(timeout, lambda: None)
+                if not not_recording: timer.start()
+
+            # Close the ffmpeg process and print the return code
+            process.stdout.close()
+            process.stderr.close()
 
-            # Restart the timer to check for new output
-            timer.cancel()
-            timer = Timer(timeout, lambda: None)
-            if not not_recording: timer.start()
+        except Exception as e:
+            if error_messages_callback:
+                error_messages_callback(e)
+            else:
+                print(e)
 
-        # Close the ffmpeg process and print the return code
-        process.stdout.close()
-        process.stderr.close()
-
-    # Start the thread to run ffmpeg
-    thread = Thread(target=run_ffmpeg)
-    if not not_recording: thread.start()
+        # Start the thread to run ffmpeg
+        thread = Thread(target=run_ffmpeg)
+        if not not_recording: thread.start()
 
-    # Return the thread object so that the caller can join it if needed
-    return thread
+        # Return the thread object so that the caller can join it if needed
+        return thread
 
 
 def stop_record_streaming_windows():
     global main_window, thread_record_streaming
 
     if thread_record_streaming and thread_record_streaming.is_alive():
         # Use ctypes to call the TerminateThread() function from the Windows API
@@ -2463,790 +2627,745 @@
 
 def show_error_messages(messages):
     global main_window, not_transcribing
     not_transcribing = True
     main_window.write_event_value("-EXCEPTION-", messages)
 
 
-def check_subtitle_stream(src, dst, media_filepath, media_type, subtitle_format, check_subtitle_streams_threading_event, transcribe_threading_event, n_media_filepaths, embed_src, embed_dst, force_recognize):
-    global language, thread_check_subtitle_stream, thread_transcribe_starter, not_transcribing, pool, main_window, \
-        removed_media_filepaths, completed_tasks, start_time
+def transcribe(src, dst, media_filepath, media_type, subtitle_format, embed_src, embed_dst, force_recognize):
+    global main_window, language, thread_transcribe, thread_transcribe_starter, not_transcribing, pool, \
+            removed_media_filepaths, completed_tasks, start_time  #, transcribe_completion_events
+
+    # CHECKING SUBTITLE STREAMS
+    if force_recognize == False:
+
+        file_display_name = os.path.basename(media_filepath).split('/')[-1]
+        src_subtitle_filepath = None
+        dst_subtitle_filepath = None
+        src_embedded_media_filepath = None
+        dst_embedded_media_filepath = None
+        ffmpeg_src_language_code = None
+        ffmpeg_dst_language_code = None
+        results = []
 
-    if not_transcribing: return
+        # CHECKING ffmpeg_src_language_code SUBTITLE STREAM ONLY, IF EXISTS WE PRINT IT AND EXTRACT IT
+        if is_same_language(src, dst, error_messages_callback=show_error_messages):
 
-    file_display_name = os.path.basename(media_filepath).split('/')[-1]
-    src_subtitle_filepath = None
-    dst_subtitle_filepath = None
-    src_embedded_media_filepath = None
-    dst_embedded_media_filepath = None
-    ffmpeg_src_language_code = None
-    ffmpeg_dst_language_code = None
-    results = []
-
-    # CHECKING ffmpeg_src_language_code SUBTITLE STREAM ONLY, IF EXISTS WE PRINT IT AND EXTRACT IT
-    if is_same_language(src, dst, error_messages_callback=show_error_messages):
-
-        if not_transcribing: return
-
-        ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
-
-        window_key = '-PROGRESS-LOG-'
-        msg = f"Checking {media_filepath}\n"
-        append_flag = True
-        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
-
-        subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
-        subtitle_streams_data = subtitle_stream_parser(media_filepath)
-
-        if not_transcribing: return
-
-        if subtitle_streams_data and subtitle_streams_data != []:
-
-            src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
+            if not_transcribing: return
 
-            if ffmpeg_src_language_code in subtitle_stream_parser.languages():
+            ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
 
-                if not_transcribing: return
+            window_key = '-PROGRESS-LOG-'
+            msg = f"Checking {file_display_name}\n"
+            append_flag = True
+            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                window_key = '-PROGRESS-LOG-'
-                msg = "Is '%s' subtitle stream exist : Yes\n" %(ffmpeg_src_language_code.center(3))
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+            subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
+            subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
-                subtitle_stream_regions = []
-                subtitle_stream_transcripts = []
-                for entry in src_subtitle_stream_timed_subtitles:
-                    subtitle_stream_regions.append(entry[0])
-                    subtitle_stream_transcripts.append(entry[1])
-                base, ext = os.path.splitext(media_filepath)
-                src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
-                writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+            if not_transcribing: return
 
-                if not_transcribing: return
+            if subtitle_streams_data and subtitle_streams_data != []:
 
-                window_key = '-PROGRESS-LOG-'
-                msg = f"Extracting '{ffmpeg_src_language_code}'subtitle stream as :\n  {src_subtitle_filepath}\n"
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
-                writer.write(src_subtitle_filepath)
-                if force_recognize == False:
-                    removed_media_filepaths.append(media_filepath)
+                if ffmpeg_src_language_code in subtitle_stream_parser.languages():
 
-                if not_transcribing: return
+                    if not_transcribing: return
 
-                if src_subtitle_filepath and os.path.isfile(src_subtitle_filepath):
-                    window_key = '-RESULTS-'
-                    msg = "Results for {} :\n".format(file_display_name)
+                    window_key = '-PROGRESS-LOG-'
+                    msg = "Is %s has '%s' subtitle stream : Yes\n" %(file_display_name, ffmpeg_src_language_code.center(3))
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    window_key = '-RESULTS-'
-                    msg = "{}\n".format(src_subtitle_filepath)
-                    append_flag = True
-                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                    subtitle_stream_regions = []
+                    subtitle_stream_transcripts = []
+                    for entry in src_subtitle_stream_timed_subtitles:
+                        subtitle_stream_regions.append(entry[0])
+                        subtitle_stream_transcripts.append(entry[1])
+                    base, ext = os.path.splitext(media_filepath)
+                    src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
+                    writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
 
-                    window_key = '-RESULTS-'
-                    msg = "\n"
+                    if not_transcribing: return
+
+                    window_key = '-PROGRESS-LOG-'
+                    msg = f"Extracting {file_display_name} '{ffmpeg_src_language_code}' subtitle stream as :\n  {src_subtitle_filepath}\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            else:
-                window_key = '-PROGRESS-LOG-'
-                msg = "Is '%s' subtitle stream exist : No\n" %(ffmpeg_src_language_code.center(3))
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
-
-                if not_transcribing: return
+                    writer.write(src_subtitle_filepath)
+                    if force_recognize == False:
+                        if media_filepath not in removed_media_filepaths:
+                            removed_media_filepaths.append(media_filepath)
 
-        if not_transcribing: return
+                    if not_transcribing: return
 
+                    if src_subtitle_filepath and os.path.isfile(src_subtitle_filepath):
+                        window_key = '-RESULTS-'
+                        msg = f"Results for {file_display_name} :\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-    # CHECKING ffmpeg_src_language_code AND ffmpeg_dst_language_code SUBTITLE STREAMS, IF EXISTS WE PRINT IT AND EXTRACT IT
-    # IF ONE OF THEM (ffmpeg_src_language_code OR ffmpeg_dst_language_code) NOT EXIST, WE TRANSLATE IT,
-    # AND IF BOOLEAN VALUE FOR EMBED (FOR SRC OR DST LANGUAGE) IS TRUE THEN WE EMBED IT
-    elif not is_same_language(src, dst, error_messages_callback=show_error_messages):
+                        window_key = '-RESULTS-'
+                        msg = "{}\n".format(src_subtitle_filepath)
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-        if not_transcribing: return
+                        window_key = '-RESULTS-'
+                        msg = "\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-        ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
-        ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
+                        completed_tasks += 1
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
+                        if force_recognize == False:
+                            if media_filepath not in removed_media_filepaths:
+                                removed_media_filepaths.append(media_filepath)
 
-        subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
-        subtitle_streams_data = subtitle_stream_parser(media_filepath)
+                    if embed_src == True:
+                        window_key = '-PROGRESS-LOG-'
+                        msg = f"Cannot embed '{src_subtitle_filepath}' into {file_display_name} because '{ffmpeg_src_language_code}' subtitle stream already existed\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-        if not_transcribing: return
 
-        window_key = '-PROGRESS-LOG-'
-        msg = f"Checking {media_filepath}\n"
-        append_flag = True
-        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                else:
+                    window_key = '-PROGRESS-LOG-'
+                    msg = "Is %s has '%s' subtitle stream : No\n" %(file_display_name, ffmpeg_src_language_code.center(3))
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-        if subtitle_streams_data and subtitle_streams_data != []:
+                    if not_transcribing: return
 
+                
             if not_transcribing: return
 
-            src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
-            dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
+        # CHECKING ffmpeg_src_language_code AND ffmpeg_dst_language_code SUBTITLE STREAMS, IF EXISTS WE PRINT IT AND EXTRACT IT
+        # IF ONE OF THEM (ffmpeg_src_language_code OR ffmpeg_dst_language_code) NOT EXIST, WE TRANSLATE IT,
+        # AND IF BOOLEAN VALUE FOR EMBED (FOR SRC OR DST LANGUAGE) IS TRUE THEN WE EMBED IT
+        elif not is_same_language(src, dst, error_messages_callback=show_error_messages):
 
-            # ffmpeg_src_language_code subtitle stream exist, we print it and extract it
-            if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-
-                if not_transcribing: return
-
-                window_key = '-PROGRESS-LOG-'
-                msg = "Is '%s' subtitle stream exist : Yes\n" %(ffmpeg_src_language_code.center(3))
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+            if not_transcribing: return
 
-                subtitle_stream_regions = []
-                subtitle_stream_transcripts = []
-                for entry in src_subtitle_stream_timed_subtitles:
-                    subtitle_stream_regions.append(entry[0])
-                    subtitle_stream_transcripts.append(entry[1])
-                    if not_transcribing: return
-                base, ext = os.path.splitext(media_filepath)
-                src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
-                writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+            ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
+            ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
 
-                if not_transcribing: return
+            subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
+            subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
-                window_key = '-PROGRESS-LOG-'
-                msg = f"Extracting '{ffmpeg_src_language_code}'subtitle stream as :\n  {src_subtitle_filepath}\n"
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
-
-                writer.write(src_subtitle_filepath)
-
-                results.append(src_subtitle_filepath)
+            if not_transcribing: return
 
-                if not_transcribing: return
+            window_key = '-PROGRESS-LOG-'
+            msg = f"Checking {file_display_name}\n"
+            append_flag = True
+            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            # ffmpeg_src_language_code subtitle stream not exist, just print it
-            else:
-                window_key = '-PROGRESS-LOG-'
-                msg = "Is '%s' subtitle stream exist : No\n" %(ffmpeg_src_language_code.center(3))
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+            if subtitle_streams_data and subtitle_streams_data != []:
 
                 if not_transcribing: return
 
+                src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
+                dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
 
-            # ffmpeg_dst_language_code subtitle stream exist, so we print it and extract it
-            if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
+                # ffmpeg_src_language_code subtitle stream exist, we print it and extract it
+                if ffmpeg_src_language_code in subtitle_stream_parser.languages():
 
-                if not_transcribing: return
+                    if not_transcribing: return
 
-                window_key = '-PROGRESS-LOG-'
-                msg = "Is '%s' subtitle stream exist : Yes\n" %(ffmpeg_dst_language_code.center(3))
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                    window_key = '-PROGRESS-LOG-'
+                    msg = "Is %s has '%s' subtitle stream : Yes\n" %(file_display_name, ffmpeg_src_language_code.center(3))
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                if not_transcribing: return
+                    subtitle_stream_regions = []
+                    subtitle_stream_transcripts = []
+                    for entry in src_subtitle_stream_timed_subtitles:
+                        subtitle_stream_regions.append(entry[0])
+                        subtitle_stream_transcripts.append(entry[1])
+                        if not_transcribing: return
+                    base, ext = os.path.splitext(media_filepath)
+                    src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
+                    writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
 
-                subtitle_stream_regions = []
-                subtitle_stream_transcripts = []
-                for entry in dst_subtitle_stream_timed_subtitles:
-                    subtitle_stream_regions.append(entry[0])
-                    subtitle_stream_transcripts.append(entry[1])
                     if not_transcribing: return
-                base, ext = os.path.splitext(media_filepath)
-                dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
-                writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
 
-                if not_transcribing: return
+                    window_key = '-PROGRESS-LOG-'
+                    msg = f"Extracting {file_display_name} '{ffmpeg_src_language_code}' subtitle stream as :\n  {src_subtitle_filepath}\n"
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                window_key = '-PROGRESS-LOG-'
-                msg = f"Extracting '{ffmpeg_dst_language_code}'subtitle stream as :\n  {dst_subtitle_filepath}\n"
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                    writer.write(src_subtitle_filepath)
 
-                writer.write(dst_subtitle_filepath)
+                    results.append(src_subtitle_filepath)
 
-                results.append(dst_subtitle_filepath)
+                    if not_transcribing: return
 
-                if not_transcribing: return
+                    if embed_src == True:
+                        window_key = '-PROGRESS-LOG-'
+                        msg = f"Cannot embed '{src_subtitle_filepath}' into {file_display_name} because '{ffmpeg_src_language_code}' subtitle stream already existed\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            # ffmpeg_dst_language_code subtitle stream not exist, just print it
-            else:
-                window_key = '-PROGRESS-LOG-'
-                msg = "Is '%s' subtitle stream exist : No\n" %(ffmpeg_dst_language_code.center(3))
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                if not_transcribing: return
+                # ffmpeg_src_language_code subtitle stream not exist, just print it
+                else:
+                    window_key = '-PROGRESS-LOG-'
+                    msg = "Is %s has '%s' subtitle stream : No\n" %(file_display_name, ffmpeg_src_language_code.center(3))
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            # ffmpeg_src_language_code subtitle stream = not exist,
-            # ffmpeg_dst_language_code subtitle stream = exist
-            # so we translate it from 'dst' to 'src'
-            if ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code not in subtitle_stream_parser.languages():
+                    if not_transcribing: return
 
-                if dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                # ffmpeg_dst_language_code subtitle stream exist, so we print it and extract it
+                if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
 
                     if not_transcribing: return
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = 'Translating {} subtitles from {} ({}) to {} ({})...\n' .format(file_display_name, language.name_of_code[dst], dst, language.name_of_code[src], src)
+                    msg = "Is %s has '%s' subtitle stream : Yes\n" %(file_display_name, ffmpeg_dst_language_code.center(3))
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    info = 'Translating subtitles from %s (%s) to %s (%s)' %(language.name_of_code[dst], dst, language.name_of_code[src], src)
-                    total = 100
-                    start_time = time.time()
-
-                    transcript_translator = SentenceTranslator(src=dst, dst=src, error_messages_callback=show_error_messages)
-
                     if not_transcribing: return
 
-                    translated_subtitle_stream_transcripts = []
-
-                    for i, translated_subtitle_stream_transcript in enumerate(pool[media_filepath].imap(transcript_translator, subtitle_stream_transcripts)):
-
-                        if not_transcribing:
-                            if pool[media_filepath]:
-                                pool[media_filepath].terminate()
-                                pool[media_filepath].close()
-                                pool[media_filepath].join()
-                                pool[media_filepath] = None
-                            return
-
-                        translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
-
+                    subtitle_stream_regions = []
+                    subtitle_stream_transcripts = []
+                    for entry in dst_subtitle_stream_timed_subtitles:
+                        subtitle_stream_regions.append(entry[0])
+                        subtitle_stream_transcripts.append(entry[1])
                         if not_transcribing: return
+                    base, ext = os.path.splitext(media_filepath)
+                    dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
+                    writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
 
-                        progress = int(i*100/len(dst_subtitle_stream_timed_subtitles))
-                        percentage = f'{progress}%'
-
-                        if progress > 0:
-                            elapsed_time = time.time() - start_time
-                            eta_seconds = (elapsed_time / progress) * (total - progress)
-                        else:
-                            eta_seconds = 0
-                        eta_time = timedelta(seconds=int(eta_seconds))
-                        eta_str = str(eta_time)
-                        hour, minute, second = eta_str.split(":")
-                        main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, percentage, progress, hour.zfill(2), minute, second))
-
-                    elapsed_time = time.time() - start_time
-                    elapsed_time_seconds = timedelta(seconds=int(elapsed_time))
-                    elapsed_time_str = str(elapsed_time_seconds)
-                    hour, minute, second = elapsed_time_str.split(":")
-                    main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, "100%", total, hour.zfill(2), minute, second))
-
-                    if not_transcribing:
-                        if pool[media_filepath]:
-                            pool[media_filepath].terminate()
-                            pool[media_filepath].close()
-                            pool[media_filepath].join()
-                            pool[media_filepath] = None
-                        return
+                    if not_transcribing: return
 
                     window_key = '-PROGRESS-LOG-'
-                    msg = "Writing translated subtitle file for {}\n".format(file_display_name)
+                    msg = f"Extracting {file_display_name} '{ffmpeg_dst_language_code}' subtitle stream as :\n  {dst_subtitle_filepath}\n"
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    base, ext = os.path.splitext(media_filepath)
-                    dst_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
-                    translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                    translation_writer.write(dst_subtitle_filepath)
+                    writer.write(dst_subtitle_filepath)
 
                     results.append(dst_subtitle_filepath)
 
-                    if not_transcribing:
-                        if pool[media_filepath]:
-                            pool[media_filepath].terminate()
-                            pool[media_filepath].close()
-                            pool[media_filepath].join()
-                            pool[media_filepath] = None
-                        return
+                    if not_transcribing: return
+
+                    if embed_dst == True:
+                        window_key = '-PROGRESS-LOG-'
+                        msg = f"Cannot embed '{dst_subtitle_filepath}' into {file_display_name} because '{ffmpeg_dst_language_code}' subtitle stream already existed\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
+                # ffmpeg_dst_language_code subtitle stream not exist, just print it
+                else:
                     window_key = '-PROGRESS-LOG-'
-                    msg = f"Translated subtitles file saved as :\n  {dst_subtitle_filepath}\n"
+                    msg = "Is %s has '%s' subtitle stream : No\n" %(file_display_name, ffmpeg_dst_language_code.center(3))
                     append_flag = True
                     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    if force_recognize == False:
-                        removed_media_filepaths.append(media_filepath)
+                    if not_transcribing: return
 
-                    # if embed_dst is True then we embed that translated srt into media_filepath
-                    if embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                # ffmpeg_src_language_code subtitle stream = not exist,
+                # ffmpeg_dst_language_code subtitle stream = exist
+                # so we translate it from 'dst' to 'src'
+                if ffmpeg_src_language_code not in subtitle_stream_parser.languages() and ffmpeg_dst_language_code in subtitle_stream_parser.languages():
 
-                        if not_transcribing: return
+                    if dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
 
-                        base, ext = os.path.splitext(media_filepath)
-                        tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                        ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
-                        dst_embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                        if not_transcribing: return
 
                         window_key = '-PROGRESS-LOG-'
-                        msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {file_display_name}"
+                        msg = f'Translating {file_display_name} subtitles from {language.name_of_code[dst]} ({dst}) to {language.name_of_code[src]} ({src})...\n'
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                        if not_transcribing: return
+                        info = 'Translating subtitles from %s (%s) to %s (%s)' %(language.name_of_code[dst], dst, language.name_of_code[src], src)
+                        total = 100
+                        start_time = time.time()
 
-                        try:
-                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                            result = subtitle_embedder(media_filepath)
-                        except Exception as e:
-                            not_transcribing = True
-                            main_window.write_event_value("-EXCEPTION-", e)
-                            return
+                        transcript_translator = SentenceTranslator(src=dst, dst=src, error_messages_callback=show_error_messages)
 
                         if not_transcribing: return
 
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
-                            shutil.copy(tmp_embedded_media_filepath_1, dst_embedded_media_filepath)
-                            os.remove(tmp_embedded_media_filepath_1)
+                        translated_subtitle_stream_transcripts = []
 
-                            results.append(dst_embedded_media_filepath)
+                        for i, translated_subtitle_stream_transcript in enumerate(pool[media_filepath].imap(transcript_translator, subtitle_stream_transcripts)):
 
-                        if os.path.isfile(dst_embedded_media_filepath):
-                            window_key = '-PROGRESS-LOG-'
-                            msg = f"Subtitle embedded {media_type} file saved as :\n  {dst_embedded_media_filepath}\n"
-                            append_flag = True
-                            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
-
-                        if not_transcribing: return
+                            if not_transcribing:
+                                if pool[media_filepath]:
+                                    pool[media_filepath].terminate()
+                                    pool[media_filepath].close()
+                                    pool[media_filepath].join()
+                                    pool[media_filepath] = None
+                                return
 
+                            translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
 
-            # ffmpeg_src_language_code subtitle stream = exist,
-            # ffmpeg_dst_language_code subtitle stream = not exist
-            # so we translate it from 'src' to 'dst'
-            elif ffmpeg_dst_language_code not in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
+                            if not_transcribing: return
 
-                if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                            progress = int(i*100/len(dst_subtitle_stream_timed_subtitles))
+                            percentage = f'{progress}%'
 
-                    if not_transcribing: return
+                            if progress > 0:
+                                elapsed_time = time.time() - start_time
+                                eta_seconds = (elapsed_time / progress) * (total - progress)
+                            else:
+                                eta_seconds = 0
+                            eta_time = timedelta(seconds=int(eta_seconds))
+                            eta_str = str(eta_time)
+                            hour, minute, second = eta_str.split(":")
+                            main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, percentage, progress, hour.zfill(2), minute, second))
 
-                    window_key = '-PROGRESS-LOG-'
-                    msg = 'Translating {} subtitles from {} ({}) to {} ({})...\n' .format(file_display_name, language.name_of_code[src], src, language.name_of_code[dst], dst)
-                    append_flag = True
-                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                        elapsed_time = time.time() - start_time
+                        elapsed_time_seconds = timedelta(seconds=int(elapsed_time))
+                        elapsed_time_str = str(elapsed_time_seconds)
+                        hour, minute, second = elapsed_time_str.split(":")
+                        main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, "100%", total, hour.zfill(2), minute, second))
 
-                    info = 'Translating subtitles from %s (%s) to %s (%s)' %(language.name_of_code[src], src, language.name_of_code[dst], dst)
-                    total = 100
-                    start_time = time.time()
+                        if not_transcribing:
+                            if pool[media_filepath]:
+                                pool[media_filepath].terminate()
+                                pool[media_filepath].close()
+                                pool[media_filepath].join()
+                                pool[media_filepath] = None
+                            return
 
-                    transcript_translator = SentenceTranslator(src=src, dst=dst, error_messages_callback=show_error_messages)
+                        window_key = '-PROGRESS-LOG-'
+                        msg = f"Writing {file_display_name} translated subtitle file...\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    if not_transcribing: return
+                        base, ext = os.path.splitext(media_filepath)
+                        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
+                        translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                        translation_writer.write(src_subtitle_filepath)
 
-                    translated_subtitle_stream_transcripts = []
-                    for i, translated_subtitle_stream_transcript in enumerate(pool[media_filepath].imap(transcript_translator, subtitle_stream_transcripts)):
+                        results.append(src_subtitle_filepath)
 
                         if not_transcribing:
                             if pool[media_filepath]:
                                 pool[media_filepath].terminate()
                                 pool[media_filepath].close()
                                 pool[media_filepath].join()
                                 pool[media_filepath] = None
                             return
 
-                        translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
+                        window_key = '-PROGRESS-LOG-'
+                        msg = f"{file_display_name} translated subtitles file saved as :\n  {src_subtitle_filepath}\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                        progress = int(i*100/len(src_subtitle_stream_timed_subtitles))
-                        
-                        percentage = f'{progress}%'
+                        # if embed_src is True then we embed that translated srt (from dst to src) above into media_filepath
+                        if embed_src == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
 
-                        if progress > 0:
-                            elapsed_time = time.time() - start_time
-                            eta_seconds = (elapsed_time / progress) * (total - progress)
-                        else:
-                            eta_seconds = 0
-                        eta_time = timedelta(seconds=int(eta_seconds))
-                        eta_str = str(eta_time)
-                        hour, minute, second = eta_str.split(":")
-                        main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, percentage, progress, hour.zfill(2), minute, second))
+                            if not_transcribing: return
 
-                    elapsed_time = time.time() - start_time
-                    elapsed_time_seconds = timedelta(seconds=int(elapsed_time))
-                    elapsed_time_str = str(elapsed_time_seconds)
-                    hour, minute, second = elapsed_time_str.split(":")
-                    main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, "100%", total, hour.zfill(2), minute, second))
+                            base, ext = os.path.splitext(media_filepath)
+                            tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
+                            ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
+                            src_embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
 
-                    if not_transcribing:
-                        if pool[media_filepath]:
-                            pool[media_filepath].terminate()
-                            pool[media_filepath].close()
-                            pool[media_filepath].join()
-                            pool[media_filepath] = None
-                        return
+                            window_key = '-PROGRESS-LOG-'
+                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {file_display_name}"
+                            append_flag = True
+                            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    window_key = '-PROGRESS-LOG-'
-                    msg = "Writing translated subtitle file for {}\n".format(file_display_name)
-                    append_flag = True
-                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                            if not_transcribing: return
 
-                    base, ext = os.path.splitext(media_filepath)
-                    dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
-                    translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                    translation_writer.write(dst_subtitle_filepath)
+                            try:
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                result = subtitle_embedder(media_filepath)
+                            except Exception as e:
+                                not_transcribing = True
+                                main_window.write_event_value("-EXCEPTION-", e)
+                                return
+
+                            if not_transcribing: return
+
+                            if os.path.isfile(tmp_embedded_media_filepath_1):
+                                shutil.copy(tmp_embedded_media_filepath_1, src_embedded_media_filepath)
+                                os.remove(tmp_embedded_media_filepath_1)
+
+                                results.append(src_embedded_media_filepath)
+
+                            if os.path.isfile(src_embedded_media_filepath):
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"{file_display_name} subtitle embedded {media_type} file saved as :\n  {src_embedded_media_filepath}\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                            else:
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"Cannot embed '{src_subtitle_filepath}' into {file_display_name} because '{ffmpeg_src_language_code}' subtitle stream already existed\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    results.append(dst_subtitle_filepath)
+                            if not_transcribing: return
 
-                    window_key = '-PROGRESS-LOG-'
-                    msg = f"Translated subtitles file saved as :\n  {dst_subtitle_filepath}\n"
-                    append_flag = True
-                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                        if force_recognize == False:
+                            if media_filepath not in removed_media_filepaths:
+                                removed_media_filepaths.append(media_filepath)
 
-                    if force_recognize == False:
-                        removed_media_filepaths.append(media_filepath)
 
-                    # if embed_src is True we embed_src that translated srt into media_filepath
-                    if embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                # ffmpeg_src_language_code subtitle stream = exist,
+                # ffmpeg_dst_language_code subtitle stream = not exist
+                # so we translate it from 'src' to 'dst'
+                elif ffmpeg_src_language_code in subtitle_stream_parser.languages() and ffmpeg_dst_language_code not in subtitle_stream_parser.languages():
 
-                        if not_transcribing: return
+                    if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
 
-                        base, ext = os.path.splitext(media_filepath)
-                        tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                        ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
-                        src_embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                        if not_transcribing: return
 
                         window_key = '-PROGRESS-LOG-'
-                        msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}"
+                        msg = f'Translating {file_display_name} subtitles from {language.name_of_code[src]} ({src}) to {language.name_of_code[dst]} ({dst})...\n'
                         append_flag = True
                         main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                        if not_transcribing: return
+                        info = 'Translating subtitles from %s (%s) to %s (%s)' %(language.name_of_code[src], src, language.name_of_code[dst], dst)
+                        total = 100
+                        start_time = time.time()
 
-                        try:
-                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                            result = subtitle_embedder(media_filepath)
-                        except Exception as e:
-                            not_transcribing = True
-                            main_window.write_event_value("-EXCEPTION-", e)
-                            return
+                        transcript_translator = SentenceTranslator(src=src, dst=dst, error_messages_callback=show_error_messages)
 
                         if not_transcribing: return
 
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
-                            shutil.copy(tmp_embedded_media_filepath_1, src_embedded_media_filepath)
-                            os.remove(tmp_embedded_media_filepath_1)
+                        translated_subtitle_stream_transcripts = []
+                        for i, translated_subtitle_stream_transcript in enumerate(pool[media_filepath].imap(transcript_translator, subtitle_stream_transcripts)):
 
-                            results.append(src_embedded_media_filepath)
-
-                        if os.path.isfile(src_embedded_media_filepath):
-                            window_key = '-PROGRESS-LOG-'
-                            msg = f"Subtitle embedded {media_type} file saved as :\n  {src_embedded_media_filepath}\n"
-                            append_flag = True
-                            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                            if not_transcribing:
+                                if pool[media_filepath]:
+                                    pool[media_filepath].terminate()
+                                    pool[media_filepath].close()
+                                    pool[media_filepath].join()
+                                    pool[media_filepath] = None
+                                return
 
+                            translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
 
-            # ffmpeg_dst_language_code subtitle stream = exist
-            # ffmpeg_src_language_code subtitle stream = exist
-            # remove media_filepath from proceed list
-            elif ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                if force_recognize == False:
-                    removed_media_filepaths.append(media_filepath)
+                            progress = int(i*100/len(src_subtitle_stream_timed_subtitles))
+                        
+                            percentage = f'{progress}%'
 
-            if not_transcribing: return
+                            if progress > 0:
+                                elapsed_time = time.time() - start_time
+                                eta_seconds = (elapsed_time / progress) * (total - progress)
+                            else:
+                                eta_seconds = 0
+                            eta_time = timedelta(seconds=int(eta_seconds))
+                            eta_str = str(eta_time)
+                            hour, minute, second = eta_str.split(":")
+                            main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, percentage, progress, hour.zfill(2), minute, second))
 
-            if (src_subtitle_filepath and os.path.isfile(src_subtitle_filepath)) or (dst_subtitle_filepath and os.path.isfile(dst_subtitle_filepath)):
-                window_key = '-RESULTS-'
-                msg = "Results for {} :\n".format(file_display_name)
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                        elapsed_time = time.time() - start_time
+                        elapsed_time_seconds = timedelta(seconds=int(elapsed_time))
+                        elapsed_time_str = str(elapsed_time_seconds)
+                        hour, minute, second = elapsed_time_str.split(":")
+                        main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, "100%", total, hour.zfill(2), minute, second))
 
-                for result in results:
-                    window_key = '-RESULTS-'
-                    msg = "{}\n".format(result)
-                    append_flag = True
-                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
-                
-            if (src_subtitle_filepath and os.path.isfile(src_subtitle_filepath)) or (dst_subtitle_filepath and os.path.isfile(dst_subtitle_filepath)):
-                window_key = '-RESULTS-'
-                msg = "\n"
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                        if not_transcribing:
+                            if pool[media_filepath]:
+                                pool[media_filepath].terminate()
+                                pool[media_filepath].close()
+                                pool[media_filepath].join()
+                                pool[media_filepath] = None
+                            return
 
-        if not_transcribing: return
+                        window_key = '-PROGRESS-LOG-'
+                        msg = f"Writing {file_display_name} translated subtitle file...\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-        window_key = '-PROGRESS-LOG-'
-        msg = "\n"
-        append_flag = True
-        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                        base, ext = os.path.splitext(media_filepath)
+                        dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
+                        translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                        translation_writer.write(dst_subtitle_filepath)
 
-    check_subtitle_streams_threading_event.set()
+                        results.append(dst_subtitle_filepath)
 
+                        window_key = '-PROGRESS-LOG-'
+                        msg = f"{file_display_name} translated subtitles file saved as :\n  {dst_subtitle_filepath}\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-# RUN A THREAD FOR EACH MEDIA FILE IN PARALEL
-def transcribe(src, dst, media_filepath, media_type, subtitle_format, check_subtitle_streams_threading_event, transcribe_threading_event, n_media_filepaths, embed_src, embed_dst, force_recognize):
-    global language, thread_transcribe, thread_transcribe_starter, not_transcribing, pool, main_window, \
-        removed_media_filepaths, completed_tasks, start_time
+                        if force_recognize == False:
+                            if media_filepath not in removed_media_filepaths:
+                                removed_media_filepaths.append(media_filepath)
+
+                        # if embed_src is True we embed_src that translated srt into media_filepath
+                        if embed_dst == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+
+                            if not_transcribing: return
+
+                            base, ext = os.path.splitext(media_filepath)
+                            tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
+                            ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
+                            dst_embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
 
-    if not_transcribing: return
+                            window_key = '-PROGRESS-LOG-'
+                            msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles file into {file_display_name}"
+                            append_flag = True
+                            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-    check_subtitle_streams_threading_event.wait()
+                            if not_transcribing: return
 
-    if not_transcribing: return
+                            try:
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                result = subtitle_embedder(media_filepath)
+                            except Exception as e:
+                                not_transcribing = True
+                                main_window.write_event_value("-EXCEPTION-", e)
+                                return
+
+                            if not_transcribing: return
+
+                            if os.path.isfile(tmp_embedded_media_filepath_1):
+                                shutil.copy(tmp_embedded_media_filepath_1, dst_embedded_media_filepath)
+                                os.remove(tmp_embedded_media_filepath_1)
+
+                                results.append(dst_embedded_media_filepath)
+
+                            if os.path.isfile(dst_embedded_media_filepath):
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"{file_display_name} subtitle embedded {media_type} file saved as :\n  {dst_embedded_media_filepath}\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                            else:
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"Cannot embed '{dst_subtitle_filepath}' into {file_display_name} file because '{ffmpeg_dst_language_code}' subtitle stream already existed\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+
+                # ffmpeg_dst_language_code subtitle stream = exist
+                # ffmpeg_src_language_code subtitle stream = exist
+                # remove media_filepath from proceed list
+                elif ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
 
-    language = Language()
-    wav_filepath = None
-    sample_rate = None
+                    if embed_src == True:
+                        window_key = '-PROGRESS-LOG-'
+                        msg = f"Cannot embed '{src_subtitle_filepath}' into {file_display_name} file because '{ffmpeg_src_language_code}' subtitle stream already existed\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-    base, ext = os.path.splitext(media_filepath)
-    src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
-    if os.path.isfile(src_subtitle_filepath): os.remove(src_subtitle_filepath)
+                    if embed_dst == True:
+                        window_key = '-PROGRESS-LOG-'
+                        msg = f"Cannot embed '{dst_subtitle_filepath}' into {file_display_name} file because '{ffmpeg_dst_language_code}' subtitle stream already existed\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-    if not is_same_language(src, dst, error_messages_callback=show_error_messages):
-        base, ext = os.path.splitext(media_filepath)
-        dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
-        if os.path.isfile(dst_subtitle_filepath): os.remove(dst_subtitle_filepath)
+                if not_transcribing: return
 
-    regions = None
-    file_display_name = os.path.basename(media_filepath).split('/')[-1]
-    short_file_display_name = None
-    w = 0
-    file_display_name_width = len(file_display_name)
-    if file_display_name_width >= 64:
-        w = 64
-        short_file_display_name = file_display_name[0:w] + ".." + ext
-    else:
-        w = file_display_name_width
-        short_file_display_name = file_display_name
+                if (src_subtitle_filepath and os.path.isfile(src_subtitle_filepath)) or (dst_subtitle_filepath and os.path.isfile(dst_subtitle_filepath)):
+                    window_key = '-RESULTS-'
+                    msg = f"Results for {file_display_name} :\n"
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-    window_key = '-PROGRESS-LOG-'
-    msg = "Processing {} :\n".format(file_display_name)
-    append_flag = True
-    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                    for result in results:
+                        window_key = '-RESULTS-'
+                        msg = f"{result}\n"
+                        append_flag = True
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                
+                    window_key = '-RESULTS-'
+                    msg = "\n"
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-    window_key = '-PROGRESS-LOG-'
-    msg = "Converting {} to a temporary WAV file...\n".format(file_display_name)
-    append_flag = True
-    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                    if force_recognize == False:
+                        if media_filepath not in removed_media_filepaths:
+                            removed_media_filepaths.append(media_filepath)
+                        completed_tasks += 1
+                        main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
-    start_time = time.time()
+            if not_transcribing: return
 
-    try:
-        wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
-        wav_filepath, sample_rate = wav_converter(media_filepath)
-    except Exception as e:
-        not_transcribing = True
-        main_window.write_event_value("-EXCEPTION-", e)
-        return
+            window_key = '-PROGRESS-LOG-'
+            msg = "\n"
+            append_flag = True
+            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-    if not_transcribing: return
+            #completed_tasks += 1
+            #main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
-    window_key = '-PROGRESS-LOG-'
-    msg = "{} converted WAV file is : {}\n".format(file_display_name, wav_filepath)
-    append_flag = True
-    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-    window_key = '-PROGRESS-LOG-'
-    msg = "Finding speech regions of {} WAV file...\n".format(file_display_name)
-    append_flag = True
-    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+    # TRANSCRIBE PART
 
-    try:
-        region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
-        regions = region_finder(wav_filepath)
-        num = len(regions)
-    except Exception as e:
-        not_transcribing = True
-        main_window.write_event_value("-EXCEPTION-", e)
-        return
+    #print(f"removed_media_filepaths = {removed_media_filepaths}")
+    #print(f"media_filepath not in removed_media_filepaths = {media_filepath not in removed_media_filepaths }")
 
-    window_key = '-PROGRESS-LOG-'
-    msg = "{} speech regions found = {}\n".format(file_display_name, len(regions))
-    append_flag = True
-    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+    if media_filepath not in removed_media_filepaths:
 
-    try:
-        converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
-        recognizer = SpeechRecognizer(language=src, rate=sample_rate, error_messages_callback=show_error_messages)
-    except Exception as e:
-        not_transcribing = True
-        main_window.write_event_value("-EXCEPTION-", e)
-        return
+        if not_transcribing: return
 
-    transcriptions = []
-    translated_transcriptions = []
+        language = Language()
+        wav_filepath = None
+        sample_rate = None
 
-    if not_transcribing: return
+        base, ext = os.path.splitext(media_filepath)
+        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src, format=subtitle_format)
+        if os.path.isfile(src_subtitle_filepath): os.remove(src_subtitle_filepath)
 
-    if regions:
-        try:
-            window_key = '-PROGRESS-LOG-'
-            msg = 'Converting {} speech regions to FLAC files...\n'.format(file_display_name)
-            append_flag = True
-            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+        if not is_same_language(src, dst, error_messages_callback=show_error_messages):
+            base, ext = os.path.splitext(media_filepath)
+            dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
+            if os.path.isfile(dst_subtitle_filepath): os.remove(dst_subtitle_filepath)
+
+        regions = None
+        file_display_name = os.path.basename(media_filepath).split('/')[-1]
+        short_file_display_name = None
+        w = 0
+        file_display_name_width = len(file_display_name)
+        if file_display_name_width >= 64:
+            w = 64
+            short_file_display_name = file_display_name[0:w] + ".." + ext
+        else:
+            w = file_display_name_width
+            short_file_display_name = file_display_name
 
-            file_display_name = os.path.basename(media_filepath).split('/')[-1]
+        window_key = '-PROGRESS-LOG-'
+        msg = f"Processing {file_display_name} :\n"
+        append_flag = True
+        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            info = 'Converting speech regions to FLAC files'
-            total = 100
+        window_key = '-PROGRESS-LOG-'
+        msg = f"Converting {file_display_name} to a temporary WAV file...\n"
+        append_flag = True
+        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            start_time = time.time()
+        start_time = time.time()
 
-            extracted_regions = []
+        try:
+            wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
+            wav_filepath, sample_rate = wav_converter(media_filepath)
+        except Exception as e:
+            not_transcribing = True
+            main_window.write_event_value("-EXCEPTION-", e)
+            return
 
-            for i, extracted_region in enumerate(pool[media_filepath].imap(converter, regions)):
+        if not_transcribing: return
 
-                if not_transcribing:
-                    if pool[media_filepath]:
-                        pool[media_filepath].terminate()
-                        pool[media_filepath].close()
-                        pool[media_filepath].join()
-                        pool[media_filepath] = None
-                    return
+        window_key = '-PROGRESS-LOG-'
+        msg = f"{file_display_name} converted WAV file is :\n  {wav_filepath}\n"
+        append_flag = True
+        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                extracted_regions.append(extracted_region)
+        window_key = '-PROGRESS-LOG-'
+        msg = f"Finding speech regions of {file_display_name} WAV file...\n"
+        append_flag = True
+        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                progress = int(i*100/len(regions))
-                percentage = f'{progress}%'
+        try:
+            region_finder = SpeechRegionFinder(frame_width=4096, min_region_size=0.5, max_region_size=6, error_messages_callback=show_error_messages)
+            regions = region_finder(wav_filepath)
+            num = len(regions)
+        except Exception as e:
+            not_transcribing = True
+            main_window.write_event_value("-EXCEPTION-", e)
+            return
 
-                if progress > 0:
-                    elapsed_time = time.time() - start_time
-                    eta_seconds = (elapsed_time / progress) * (total - progress)
-                else:
-                    eta_seconds = 0
-                eta_time = timedelta(seconds=int(eta_seconds))
-                eta_str = str(eta_time)
-                hour, minute, second = eta_str.split(":")
-                main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, percentage, progress, hour.zfill(2), minute, second))
-
-            elapsed_time = time.time() - start_time
-            elapsed_time_seconds = timedelta(seconds=int(elapsed_time))
-            elapsed_time_str = str(elapsed_time_seconds)
-            hour, minute, second = elapsed_time_str.split(":")
-            main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, "100%", total, hour.zfill(2), minute, second))
-
-            if not_transcribing:
-                if pool[media_filepath]:
-                    pool[media_filepath].terminate()
-                    pool[media_filepath].close()
-                    pool[media_filepath].join()
-                    pool[media_filepath] = None
-                return
+        window_key = '-PROGRESS-LOG-'
+        msg = f"{file_display_name} speech regions found = {len(regions)}\n"
+        append_flag = True
 
-            window_key = '-PROGRESS-LOG-'
-            msg = 'Creating {} transcriptions...\n'.format(file_display_name)
-            append_flag = True
-            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            file_display_name = os.path.basename(media_filepath).split('/')[-1]
+        try:
+            converter = FLACConverter(wav_filepath=wav_filepath, error_messages_callback=show_error_messages)
+            recognizer = SpeechRecognizer(language=src, rate=sample_rate, error_messages_callback=show_error_messages)
+        except Exception as e:
+            not_transcribing = True
+            main_window.write_event_value("-EXCEPTION-", e)
+            return
 
-            info = 'Creating transcriptions'
-            total = 100
+        transcriptions = []
+        translated_transcriptions = []
 
-            start_time = time.time()
+        if not_transcribing: return
 
-            for i, transcription in enumerate(pool[media_filepath].imap(recognizer, extracted_regions)):
+        if regions:
+            try:
+                window_key = '-PROGRESS-LOG-'
+                msg = f'Converting {file_display_name} speech regions to FLAC files...\n'
+                append_flag = True
+                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                if not_transcribing:
-                    if pool[media_filepath]:
-                        pool[media_filepath].terminate()
-                        pool[media_filepath].close()
-                        pool[media_filepath].join()
-                        pool[media_filepath] = None
-                    return
+                file_display_name = os.path.basename(media_filepath).split('/')[-1]
 
-                transcriptions.append(transcription)
+                info = 'Converting speech regions to FLAC files'
+                total = 100
 
-                progress = int(i*100/len(regions))
-                percentage = f'{progress}%'
+                start_time = time.time()
 
-                if progress > 0:
-                    elapsed_time = time.time() - start_time
-                    eta_seconds = (elapsed_time / progress) * (total - progress)
-                else:
-                    eta_seconds = 0
-                eta_time = timedelta(seconds=int(eta_seconds))
-                eta_str = str(eta_time)
-                hour, minute, second = eta_str.split(":")
-                main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, percentage, progress, hour.zfill(2), minute, second))
-
-            elapsed_time = time.time() - start_time
-            elapsed_time_seconds = timedelta(seconds=int(elapsed_time))
-            elapsed_time_str = str(elapsed_time_seconds)
-            hour, minute, second = elapsed_time_str.split(":")
-            main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, "100%", total, hour.zfill(2), minute, second))
-
-            if not_transcribing:
-                if pool[media_filepath]:
-                    pool[media_filepath].terminate()
-                    pool[media_filepath].close()
-                    pool[media_filepath].join()
-                    pool[media_filepath] = None
-                return
+                extracted_regions = []
 
-            window_key = '-PROGRESS-LOG-'
-            msg = "Writing subtitle file for {}\n".format(file_display_name)
-            append_flag = True
-            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                for i, extracted_region in enumerate(pool[media_filepath].imap(converter, regions)):
 
-            writer = SubtitleWriter(regions, transcriptions, subtitle_format, error_messages_callback=show_error_messages)
-            writer.write(src_subtitle_filepath)
+                    if not_transcribing:
+                        if pool[media_filepath]:
+                            pool[media_filepath].terminate()
+                            pool[media_filepath].close()
+                            pool[media_filepath].join()
+                            pool[media_filepath] = None
+                        return
 
-            if not_transcribing:
-                if pool[media_filepath]:
-                    pool[media_filepath].terminate()
-                    pool[media_filepath].close()
-                    pool[media_filepath].join()
-                    pool[media_filepath] = None
-                return
+                    extracted_regions.append(extracted_region)
 
-            if not is_same_language(src, dst, error_messages_callback=show_error_messages):
-                base, ext = os.path.splitext(media_filepath)
-                dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
-                
-                if not_transcribing:
-                    if pool[media_filepath]:
-                        pool[media_filepath].terminate()
-                        pool[media_filepath].close()
-                        pool[media_filepath].join()
-                        pool[media_filepath] = None
-                    return
+                    progress = int(i*100/len(regions))
+                    percentage = f'{progress}%'
 
-                timed_subtitles = writer.timed_subtitles
+                    if progress > 0:
+                        elapsed_time = time.time() - start_time
+                        eta_seconds = (elapsed_time / progress) * (total - progress)
+                    else:
+                        eta_seconds = 0
+                    eta_time = timedelta(seconds=int(eta_seconds))
+                    eta_str = str(eta_time)
+                    hour, minute, second = eta_str.split(":")
+                    main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, percentage, progress, hour.zfill(2), minute, second))
 
-                created_regions = []
-                created_transcripts = []
-                for entry in timed_subtitles:
-                    created_regions.append(entry[0])
-                    created_transcripts.append(entry[1])
+                elapsed_time = time.time() - start_time
+                elapsed_time_seconds = timedelta(seconds=int(elapsed_time))
+                elapsed_time_str = str(elapsed_time_seconds)
+                hour, minute, second = elapsed_time_str.split(":")
+                main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, "100%", total, hour.zfill(2), minute, second))
 
                 if not_transcribing:
                     if pool[media_filepath]:
                         pool[media_filepath].terminate()
                         pool[media_filepath].close()
                         pool[media_filepath].join()
                         pool[media_filepath] = None
                     return
 
                 window_key = '-PROGRESS-LOG-'
-                msg = 'Translating {} subtitles from {} ({}) to {} ({})...\n' .format(file_display_name, language.name_of_code[src], src, language.name_of_code[dst], dst)
+                msg = f"Creating {file_display_name} transcriptions...\n"
                 append_flag = True
                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                 file_display_name = os.path.basename(media_filepath).split('/')[-1]
 
-                info = 'Translating subtitles from %s (%s) to %s (%s)' %(language.name_of_code[src], src, language.name_of_code[dst], dst)
+                info = 'Creating transcriptions'
                 total = 100
 
                 start_time = time.time()
 
-                transcript_translator = SentenceTranslator(src=src, dst=dst, error_messages_callback=show_error_messages)
-                translated_transcriptions = []
-
-                for i, translated_transcription in enumerate(pool[media_filepath].imap(transcript_translator, created_transcripts)):
+                for i, transcription in enumerate(pool[media_filepath].imap(recognizer, extracted_regions)):
 
                     if not_transcribing:
                         if pool[media_filepath]:
                             pool[media_filepath].terminate()
                             pool[media_filepath].close()
                             pool[media_filepath].join()
                             pool[media_filepath] = None
                         return
 
-                    translated_transcriptions.append(translated_transcription)
+                    transcriptions.append(transcription)
 
-                    progress = int(i*100/len(timed_subtitles))
+                    progress = int(i*100/len(regions))
                     percentage = f'{progress}%'
 
                     if progress > 0:
                         elapsed_time = time.time() - start_time
                         eta_seconds = (elapsed_time / progress) * (total - progress)
                     else:
                         eta_seconds = 0
@@ -3266,299 +3385,437 @@
                         pool[media_filepath].terminate()
                         pool[media_filepath].close()
                         pool[media_filepath].join()
                         pool[media_filepath] = None
                     return
 
                 window_key = '-PROGRESS-LOG-'
-                msg = "Writing translated subtitle file for {}\n".format(file_display_name)
+                msg = f"Writing {file_display_name} subtitle file...\n"
                 append_flag = True
                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                translation_writer = SubtitleWriter(created_regions, translated_transcriptions, subtitle_format, error_messages_callback=show_error_messages)
-                translation_writer.write(dst_subtitle_filepath)
+                writer = SubtitleWriter(regions, transcriptions, subtitle_format, error_messages_callback=show_error_messages)
+                writer.write(src_subtitle_filepath)
 
                 if not_transcribing:
                     if pool[media_filepath]:
                         pool[media_filepath].terminate()
                         pool[media_filepath].close()
                         pool[media_filepath].join()
                         pool[media_filepath] = None
                     return
 
-            window_key = '-PROGRESS-LOG-'
-            msg = "{} subtitles file saved as :\n  {}\n".format(file_display_name, src_subtitle_filepath)
-            append_flag = True
-            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                if not is_same_language(src, dst, error_messages_callback=show_error_messages):
+                    base, ext = os.path.splitext(media_filepath)
+                    dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst, format=subtitle_format)
+                
+                    if not_transcribing:
+                        if pool[media_filepath]:
+                            pool[media_filepath].terminate()
+                            pool[media_filepath].close()
+                            pool[media_filepath].join()
+                            pool[media_filepath] = None
+                        return
 
-            window_key = '-RESULTS-'
-            msg = "Results for {} :\n".format(file_display_name)
-            append_flag = True
-            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                    timed_subtitles = writer.timed_subtitles
 
-            window_key = '-RESULTS-'
-            msg = "{}\n".format(src_subtitle_filepath)
-            append_flag = True
-            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                    created_regions = []
+                    created_transcripts = []
+                    for entry in timed_subtitles:
+                        created_regions.append(entry[0])
+                        created_transcripts.append(entry[1])
+
+                    if not_transcribing:
+                        if pool[media_filepath]:
+                            pool[media_filepath].terminate()
+                            pool[media_filepath].close()
+                            pool[media_filepath].join()
+                            pool[media_filepath] = None
+                        return
+
+                    window_key = '-PROGRESS-LOG-'
+                    msg = f'Translating {file_display_name} subtitles from {language.name_of_code[src]} ({src}) to {language.name_of_code[dst]} ({dst})...\n'
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+
+                    file_display_name = os.path.basename(media_filepath).split('/')[-1]
+
+                    info = 'Translating subtitles from %s (%s) to %s (%s)' %(language.name_of_code[src], src, language.name_of_code[dst], dst)
+                    total = 100
+
+                    start_time = time.time()
+
+                    transcript_translator = SentenceTranslator(src=src, dst=dst, error_messages_callback=show_error_messages)
+                    translated_transcriptions = []
+
+                    for i, translated_transcription in enumerate(pool[media_filepath].imap(transcript_translator, created_transcripts)):
+
+                        if not_transcribing:
+                            if pool[media_filepath]:
+                                pool[media_filepath].terminate()
+                                pool[media_filepath].close()
+                                pool[media_filepath].join()
+                                pool[media_filepath] = None
+                            return
+
+                        translated_transcriptions.append(translated_transcription)
+
+                        progress = int(i*100/len(timed_subtitles))
+                        percentage = f'{progress}%'
+
+                        if progress > 0:
+                            elapsed_time = time.time() - start_time
+                            eta_seconds = (elapsed_time / progress) * (total - progress)
+                        else:
+                            eta_seconds = 0
+                        eta_time = timedelta(seconds=int(eta_seconds))
+                        eta_str = str(eta_time)
+                        hour, minute, second = eta_str.split(":")
+                        main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, percentage, progress, hour.zfill(2), minute, second))
+
+                    elapsed_time = time.time() - start_time
+                    elapsed_time_seconds = timedelta(seconds=int(elapsed_time))
+                    elapsed_time_str = str(elapsed_time_seconds)
+                    hour, minute, second = elapsed_time_str.split(":")
+                    main_window.write_event_value('-EVENT-UPDATE-PROGRESS-BAR-', (file_display_name, info, total, "100%", total, hour.zfill(2), minute, second))
+
+                    if not_transcribing:
+                        if pool[media_filepath]:
+                            pool[media_filepath].terminate()
+                            pool[media_filepath].close()
+                            pool[media_filepath].join()
+                            pool[media_filepath] = None
+                        return
+
+                    window_key = '-PROGRESS-LOG-'
+                    msg = f"Writing {file_display_name} translated subtitle file...\n"
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+
+                    translation_writer = SubtitleWriter(created_regions, translated_transcriptions, subtitle_format, error_messages_callback=show_error_messages)
+                    translation_writer.write(dst_subtitle_filepath)
+
+                    if not_transcribing:
+                        if pool[media_filepath]:
+                            pool[media_filepath].terminate()
+                            pool[media_filepath].close()
+                            pool[media_filepath].join()
+                            pool[media_filepath] = None
+                        return
 
-            if not is_same_language(src, dst, error_messages_callback=show_error_messages):
                 window_key = '-PROGRESS-LOG-'
-                msg = "{} translated subtitles file saved as :\n  {}\n" .format(file_display_name, dst_subtitle_filepath)
+                msg = f"{file_display_name} subtitles file saved as :\n  {src_subtitle_filepath}\n"
                 append_flag = True
                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
                 window_key = '-RESULTS-'
-                msg = "{}\n" .format(dst_subtitle_filepath)
+                msg = f"Results for {file_display_name} :\n"
                 append_flag = True
                 main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
+                window_key = '-RESULTS-'
+                msg = "{}\n".format(src_subtitle_filepath)
+                append_flag = True
+                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            # EMBEDDING SUBTITLE FILE
-            embedded_media_filepath = None
-            if is_same_language(src, dst, error_messages_callback=show_error_messages):
+                if is_same_language(src, dst, error_messages_callback=show_error_messages) and embed_src == False:
+                    completed_tasks += 1
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
-                if embed_src == True:
+                if not is_same_language(src, dst, error_messages_callback=show_error_messages):
+                    window_key = '-PROGRESS-LOG-'
+                    msg = f"{file_display_name} translated subtitles file saved as :\n  {dst_subtitle_filepath}\n"
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    base, ext = os.path.splitext(media_filepath)
-                    tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                    ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
+                    window_key = '-RESULTS-'
+                    msg = "{}\n" .format(dst_subtitle_filepath)
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                if not is_same_language(src, dst, error_messages_callback=show_error_messages) and embed_src == False and embed_dst == False:
+                    completed_tasks += 1
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
-                    try:
-                        window_key = '-PROGRESS-LOG-'
-                        msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} ...\n"
-                        append_flag = True
-                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                # EMBEDDING SUBTITLE FILE
+                embedded_media_filepath = None
+                if is_same_language(src, dst, error_messages_callback=show_error_messages):
 
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(media_filepath)
+                    if embed_src == True:
 
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
-                            shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                            os.remove(tmp_embedded_media_filepath_1)
+                        base, ext = os.path.splitext(media_filepath)
+                        tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
+                        ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
 
-                    except Exception as e:
-                        not_transcribing = True
-                        main_window.write_event_value("-EXCEPTION-", e)
-                        return
+                        embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
 
-            elif not is_same_language(src, dst, error_messages_callback=show_error_messages):
+                        try:
+                            window_key = '-PROGRESS-LOG-'
+                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}...\n"
+                            append_flag = True
+                            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                if embed_src == True and embed_dst == True:
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            result = subtitle_embedder(media_filepath)
 
-                    base, ext = os.path.splitext(media_filepath)
-                    tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                    tmp_embedded_media_filepath_2 = "{base}.embedded2.{format}".format(base=base, format=ext[1:])
-                    ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
-                    ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
+                            if os.path.isfile(tmp_embedded_media_filepath_1):
+                                shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
+                                os.remove(tmp_embedded_media_filepath_1)
+                            else:
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"Cannot embed '{src_subtitle_filepath}' into {file_display_name} because '{ffmpeg_src_language_code}' subtitle stream already existed\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    embedded_media_filepath = "{base}.{src}.{dst}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
+                        except Exception as e:
+                            not_transcribing = True
+                            main_window.write_event_value("-EXCEPTION-", e)
+                            return
 
-                    try:
-                        window_key = '-PROGRESS-LOG-'
-                        msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} ...\n"
-                        append_flag = True
-                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                elif not is_same_language(src, dst, error_messages_callback=show_error_messages):
 
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(media_filepath)
+                    if embed_src == True and embed_dst == True:
 
-                        if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
-                            window_key = '-PROGRESS-LOG-'
-                            msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} ...\n"
-                            append_flag = True
-                            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                        base, ext = os.path.splitext(media_filepath)
+                        tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
+                        tmp_embedded_media_filepath_2 = "{base}.embedded2.{format}".format(base=base, format=ext[1:])
+                        ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
+                        ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
 
-                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                            result = subtitle_embedder(tmp_embedded_media_filepath_1)
+                        embedded_media_filepath = "{base}.{src}.{dst}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
 
-                        elif (not os.path.isfile(tmp_embedded_media_filepath_1)) and os.path.isfile(dst_subtitle_filepath):
+                        try:
                             window_key = '-PROGRESS-LOG-'
-                            msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} ...\n"
+                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {file_display_name}...\n"
                             append_flag = True
                             main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
                             result = subtitle_embedder(media_filepath)
 
-                        if os.path.isfile(tmp_embedded_media_filepath_2):
-                            shutil.copy(tmp_embedded_media_filepath_2, embedded_media_filepath)
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
-                            os.remove(tmp_embedded_media_filepath_1)
-                        if os.path.isfile(tmp_embedded_media_filepath_2):
-                            os.remove(tmp_embedded_media_filepath_2)
+                            if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {file_display_name}...\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                result = subtitle_embedder(tmp_embedded_media_filepath_1)
+
+                            elif (not os.path.isfile(tmp_embedded_media_filepath_1)) and os.path.isfile(dst_subtitle_filepath):
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {file_display_name}...\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                result = subtitle_embedder(media_filepath)
+
+                            if os.path.isfile(tmp_embedded_media_filepath_2):
+                                shutil.copy(tmp_embedded_media_filepath_2, embedded_media_filepath)
+                                if os.path.isfile(tmp_embedded_media_filepath_1):
+                                    os.remove(tmp_embedded_media_filepath_1)
+                                if os.path.isfile(tmp_embedded_media_filepath_2):
+                                    os.remove(tmp_embedded_media_filepath_2)
+                            else:
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"Cannot embed '{src_subtitle_filepath}' and {src_subtitle_filepath} into {file_display_name} because '{ffmpeg_src_language_code}' and '{ffmpeg_dst_language_code}' subtitle stream already existed\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                    except Exception as e:
-                        not_transcribing = True
-                        main_window.write_event_value("-EXCEPTION-", e)
-                        return
 
-                    if not_transcribing: return
+                        except Exception as e:
+                            not_transcribing = True
+                            main_window.write_event_value("-EXCEPTION-", e)
+                            return
 
-                elif embed_src == True and embed_dst == False:
+                        if not_transcribing: return
 
-                    base, ext = os.path.splitext(media_filepath)
-                    tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                    ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
+                    elif embed_src == True and embed_dst == False:
 
-                    embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                        base, ext = os.path.splitext(media_filepath)
+                        tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
+                        ffmpeg_src_language_code = language.ffmpeg_code_of_code[src]
 
-                    try:
-                        window_key = '-PROGRESS-LOG-'
-                        msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} ...\n"
-                        append_flag = True
-                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                        embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
 
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(media_filepath)
+                        try:
+                            window_key = '-PROGRESS-LOG-'
+                            msg = f"Embedding '{ffmpeg_src_language_code}' subtitles into {file_display_name}...\n"
+                            append_flag = True
+                            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
-                            shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                            os.remove(tmp_embedded_media_filepath_1)
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            result = subtitle_embedder(media_filepath)
 
-                    except Exception as e:
-                        not_transcribing = True
-                        main_window.write_event_value("-EXCEPTION-", e)
-                        return
+                            if os.path.isfile(tmp_embedded_media_filepath_1):
+                                shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
+                                os.remove(tmp_embedded_media_filepath_1)
+                            else:
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"Cannot embed '{src_subtitle_filepath}' into {file_display_name} because '{ffmpeg_src_language_code}' subtitle stream already existed\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                        if not_transcribing: return
+                        except Exception as e:
+                            not_transcribing = True
+                            main_window.write_event_value("-EXCEPTION-", e)
+                            return
 
-                elif embed_src == False and embed_dst == True:
+                            if not_transcribing: return
 
-                    base, ext = os.path.splitext(media_filepath)
-                    tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                    ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
+                    elif embed_src == False and embed_dst == True:
 
-                    embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                        base, ext = os.path.splitext(media_filepath)
+                        tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
+                        ffmpeg_dst_language_code = language.ffmpeg_code_of_code[dst]
 
-                    try:
-                        window_key = '-PROGRESS-LOG-'
-                        msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} ...\n"
-                        append_flag = True
-                        main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                        embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
 
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(media_filepath)
+                        try:
+                            window_key = '-PROGRESS-LOG-'
+                            msg = f"Embedding '{ffmpeg_dst_language_code}' subtitles into {file_display_name}...\n"
+                            append_flag = True
+                            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
-                            shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                            os.remove(tmp_embedded_media_filepath_1)
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            result = subtitle_embedder(media_filepath)
 
-                    except Exception as e:
-                        not_transcribing = True
-                        main_window.write_event_value("-EXCEPTION-", e)
-                        return
+                            if os.path.isfile(tmp_embedded_media_filepath_1):
+                                shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
+                                os.remove(tmp_embedded_media_filepath_1)
+                            else:
+                                window_key = '-PROGRESS-LOG-'
+                                msg = f"Cannot embed '{dst_subtitle_filepath}' into {file_display_name} because '{ffmpeg_dst_language_code}' subtitle stream already existed\n"
+                                append_flag = True
+                                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-                        if not_transcribing: return
+                        except Exception as e:
+                            not_transcribing = True
+                            main_window.write_event_value("-EXCEPTION-", e)
+                            return
 
-            if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
-                window_key = '-PROGRESS-LOG-'
-                msg = f"Subtitle embedded {media_type} file saved as :\n  {embedded_media_filepath}\n"
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                            if not_transcribing: return
 
-                window_key = '-RESULTS-'
-                msg = f"{embedded_media_filepath}\n"
-                append_flag = True
-                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+                    window_key = '-PROGRESS-LOG-'
+                    msg = f"{file_display_name} subtitle embedded {media_type} file saved as :\n  {embedded_media_filepath}\n"
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            window_key = '-RESULTS-'
-            msg = "\n"
-            append_flag = True
-            main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                    window_key = '-RESULTS-'
+                    msg = f"{embedded_media_filepath}\n"
+                    append_flag = True
+                    main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-            if is_same_language(src, dst, error_messages_callback=show_error_messages):
-                if embed_src == True:
-                    if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
-                        transcribe_threading_event.set()
-                        completed_tasks += 1
-                        main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
-                else:
-                    transcribe_threading_event.set()
                     completed_tasks += 1
                     main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
 
-            elif not is_same_language(src, dst, error_messages_callback=show_error_messages):
-                if embed_src == True or embed_dst == True:
-                    if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
-                        transcribe_threading_event.set()
-                        completed_tasks += 1
-                        main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
-                else:
-                    transcribe_threading_event.set()
-                    completed_tasks += 1
-                    main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
+                window_key = '-RESULTS-'
+                msg = "\n"
+                append_flag = True
+                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-        except Exception as e:
-            not_transcribing = True
-            main_window.write_event_value("-EXCEPTION-", e)
-            return
 
-    if pool[media_filepath]:
-        pool[media_filepath].close()
-        pool[media_filepath].join()
-        pool[media_filepath] = None
+            except Exception as e:
+                not_transcribing = True
+                main_window.write_event_value("-EXCEPTION-", e)
+                return
+
+        if pool[media_filepath]:
+            pool[media_filepath].close()
+            pool[media_filepath].join()
+            pool[media_filepath] = None
 
 
 def start_transcription(media_filepaths, src, dst, subtitle_format, embed_src, embed_dst, force_recognize):
-    global language, pool, thread_check_subtitle_stream, thread_transcribe, thread_transcribe_starter, removed_media_filepaths, completed_tasks, main_window
+    global main_window, language, pool, thread_check_subtitle_stream, thread_transcribe, thread_transcribe_starter, \
+            removed_media_filepaths, completed_tasks  #, transcribe_completion_events
 
     window_key = '-PROGRESS-LOG-'
     msg = ''
     append_flag = False
     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
     window_key = '-RESULTS-'
     msg = ''
     append_flag = False
     main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
 
-    n_media_filepaths = len(media_filepaths)
-    transcribe_completion_events = {}  # Dictionary to store completion events
-    check_subtitle_stream_completion_events = {}  # Dictionary to store completion events
-    pool = {media_filepath: multiprocessing.Pool(16, initializer=NoConsoleProcess) for media_filepath in media_filepaths}
-    media_types = {}
+    media_types = {media_filepath: check_file_type(media_filepath, error_messages_callback=show_error_messages) for media_filepath in media_filepaths}
+    #transcribe_completion_events = {media_filepath: threading.Event() for media_filepath in media_filepaths}
+    #pool = {media_filepath: multiprocessing.Pool(16, initializer=NoConsoleProcess) for media_filepath in media_filepaths}
+
     removed_media_filepaths = []
+    proceed_list = []
 
     for media_filepath in media_filepaths:
-        transcribe_completion_events[media_filepath] = threading.Event()
-        check_subtitle_stream_completion_events[media_filepath] = threading.Event()
-        media_types[media_filepath] = check_file_type(media_filepath, error_messages_callback=show_error_messages)
-        thread_check_subtitle_stream = Thread(target=check_subtitle_stream, args=(src, dst, media_filepath, media_types[media_filepath], subtitle_format, check_subtitle_stream_completion_events[media_filepath], transcribe_completion_events[media_filepath], n_media_filepaths, embed_src, embed_dst, force_recognize), daemon=True)
-        thread_check_subtitle_stream.start()
-        check_subtitle_stream_completion_events[media_filepath].wait()
 
-    #print(f"removed_media_filepaths = {removed_media_filepaths}")
-    if removed_media_filepaths:
-        for removed_media_filepath in removed_media_filepaths:
-            if removed_media_filepath in media_filepaths:
-                media_filepaths.remove(removed_media_filepath)
-                #main_window.write_event_value('-REMOVE-FILE-FROM-LIST-', removed_media_filepath)
-                main_window['-LIST-'].update(media_filepaths)
-                check_subtitle_stream_completion_events[media_filepath].set()
-                transcribe_completion_events[media_filepath].set()
-                completed_tasks += 1
-                main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
-
-    if media_filepaths:
-        for media_filepath in media_filepaths:
-            thread_transcribe = Thread(target=transcribe, args=(src, dst, media_filepath, media_types[media_filepath], subtitle_format, check_subtitle_stream_completion_events[media_filepath], transcribe_completion_events[media_filepath], n_media_filepaths, embed_src, embed_dst, force_recognize), daemon=True)
-            thread_transcribe.start()
-            transcribe_completion_events[media_filepath].wait()
-
-    #else:
-    #    for removed_media_filepath in removed_media_filepaths:
-    #        transcribe_completion_events[media_filepath].set()
-    #        completed_tasks += 1
-    #        main_window.write_event_value('-EVENT-TRANSCRIBE-TASKS-COMPLETED-', completed_tasks)
-
-    # Wait for all threads to complete
-    #for completion_event in transcribe_completion_events.values():
-    #    completion_event.wait()
+        if force_recognize == True:
+
+            media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+
+            base, ext = os.path.splitext(media_filepath)
+            tmp_subtitle_removed_media_filepath_1 = "{base}.removed1.{format}".format(base=base, format=ext[1:])
+            subtitle_removed_media_filepath = "{base}.force_recognize.{format}".format(base=base, format=ext[1:])
+
+            subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
+            tmp_output = subtitle_remover(media_filepath)
+
+            if os.path.isfile(tmp_output):
+                shutil.copy(tmp_output, subtitle_removed_media_filepath)
+                os.remove(tmp_output)
+
+                proceed_list.append(subtitle_removed_media_filepath)
+
+                window_key = '-PROGRESS-LOG-'
+                msg = f"Removing subtitle streams from {media_type} file...\n"
+                append_flag = False
+                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+
+                window_key = '-PROGRESS-LOG-'
+                msg = f"Subtitle removed {media_type} file saved as :\n  {subtitle_removed_media_filepath}\n"
+                append_flag = False
+                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+
+                '''
+                window_key = '-PROGRESS-LOG-'
+                msg = "\n"
+                append_flag = False
+                main_window.write_event_value('-EVENT-TRANSCRIBE-MESSAGES-', (window_key, msg, append_flag))
+                '''
+
+                #transcribe_completion_events[media_filepath] = threading.Event()
+
+        else:
+
+            proceed_list = media_filepaths
+
+
+    if proceed_list:
+
+        media_types = {media_filepath: check_file_type(media_filepath, error_messages_callback=show_error_messages) for media_filepath in proceed_list}
+        pool = {}
+        pool = {media_filepath: multiprocessing.Pool(16, initializer=NoConsoleProcess) for media_filepath in proceed_list}
+        #transcribe_completion_events = {}
+
+        #for e in check_subtitle_stream_completion_events:
+        #    print(f"e = {e}")
+
+        for media_filepath in proceed_list:
+            if os.path.isfile(media_filepath):
+                media_type = check_file_type(media_filepath, error_messages_callback=show_error_messages)
+
+                #print(f"check_subtitle_stream_completion_events[{media_filepath}].is_set() = {check_subtitle_stream_completion_events[media_filepath].is_set()}")
+                #transcribe_completion_events[media_filepath] = threading.Event()
+
+                thread_transcribe = Thread(target=transcribe, args=(src, dst, media_filepath, media_type, subtitle_format, embed_src, embed_dst, force_recognize), daemon=True)
+                thread_transcribe.start()
+                #transcribe_completion_events[media_filepath].wait()
+
 
 
 #------------------------------------------------------------ MAIN FUNCTION ------------------------------------------------------------#
 
 
 def main():
     global language, not_transcribing, thread_transcribe, thread_transcribe_starter, pool, removed_media_filepaths, \
@@ -3646,14 +3903,15 @@
     sg_listbox_values = []
     invalid_media_filepaths = []
     not_exist_filepaths = []
     argpath = None
 
     media_type = None
     embed_src = False
+    embed_dst = False
     force_recognize = False
     src_subtitle_filepath = None
     dst_subtitle_filepath = None
     ffmpeg_src_language_code = None
     ffmpeg_dst_language_code = None
     embedded_media_filepath = None
     subtitle_format = args.format
@@ -3818,14 +4076,15 @@
                     sg.Text('Translation language', size=(18,1)),
                     sg.Combo(list(language.code_of_name), default_value=sg_combo_dst_values, enable_events=True, key='-DST-'),
                     sg.Checkbox("Embed translated subtitles file into media file", default=embed_dst, key='-EMBED-DST-SUBTITLE-')
                 ],
                 [
                     sg.Text('Subtitle format', size=(18,1)),
                     sg.Combo(list(SubtitleFormatter.supported_formats), default_value=sg_combo_subtitle_format_values, enable_events=True, key='-SUBTITLE-FORMAT-'),
+                    sg.Checkbox("Force recognize", default=embed_dst, key='-FORCE-RECOGNIZE-')
                 ],
                 [
                     sg.Text('URL', size=(18,1)),
                     sg.Input(size=(58, 1), expand_x=True, expand_y=True, key='-URL-', enable_events=True, right_click_menu=['&Edit', ['&Copy','&Paste',]]),
                     sg.Button("Start Record Streaming", size=(22,1), key='-RECORD-STREAMING-')
                 ],
                 [
@@ -4124,18 +4383,16 @@
                 filepaths = []
                 invalid_media_filepaths = []
                 not_exist_filepaths = []
 
 
         elif event == '-REMOVE-FILE-FROM-LIST-':
 
-            listbox_selection = values['-LIST-']
-            if listbox_selection:
-                for index in listbox_selection[::-1]:
-                    sg_listbox_values.remove(index)
+            removed_file_list = values[event]
+            if removed_file_list:
                 main_window['-LIST-'].update(sg_listbox_values)
 
 
         elif event == '-REMOVE-':
 
             listbox_selection = values['-LIST-']
             if listbox_selection:
@@ -4185,14 +4442,15 @@
 
                 if not not_transcribing:
                     completed_tasks = 0
                     pool = None
                     main_window['-START-'].update(('Cancel','Start')[not_transcribing], button_color=(('white', ('red', '#283b5b')[not_transcribing])))
                     embed_src = main_window['-EMBED-SRC-SUBTITLE-'].get()
                     embed_dst = main_window['-EMBED-DST-SUBTITLE-'].get()
+                    force_recognize = main_window['-FORCE-RECOGNIZE-'].get()
                     thread_transcribe_starter = Thread(target=start_transcription, args=(sg_listbox_values, src, dst, subtitle_format, embed_src, embed_dst, force_recognize), daemon=True)
                     thread_transcribe_starter.start()
 
                 else:
                     not_transcribing = not not_transcribing
                     answer = popup_yes_no('Are you sure?', title='Confirm')
                     if 'Yes' in answer:
@@ -4245,15 +4503,18 @@
                 main_window['-ETA-'].update(time_str)
 
 
         elif event == '-EVENT-TRANSCRIBE-TASKS-COMPLETED-':
 
             completed_tasks = values[event]
 
-            if completed_tasks-len(removed_media_filepaths) == len(sg_listbox_values):
+            #print(f"completed_tasks = {completed_tasks}")
+            #print(f"len(sg_listbox_values) = {len(sg_listbox_values)}")
+
+            if completed_tasks == len(sg_listbox_values):
                 not_transcribing = True
                 main_window['-START-'].update(('Cancel','Start')[not_transcribing], button_color=(('white', ('red', '#283b5b')[not_transcribing])))
                 transcribe_end_time = time.time()
                 transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
                 transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
                 transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
                 hour, minute, second = transcribe_elapsed_time_str.split(":")
@@ -4297,15 +4558,15 @@
                 main_window['-RECORD-STREAMING-STATUS-'].update(text_color='black', background_color='green1')
                 main_window['-STREAMING-DURATION-RECORDED-'].update(text_color='black', background_color='green1')
 
 
         elif event == '-RECORD-STREAMING-':
 
             if not_recording == True:
-                is_valid_url_streaming = is_streaming_url(str(values['-URL-']).strip())
+                is_valid_url_streaming = is_streaming_url(str(values['-URL-']).strip(), error_messages_callback=show_error_messages)
 
             if not is_valid_url_streaming:
                 msg = "Invalid URL, please enter a valid URL"
                 sg.Popup(msg, title="Info", line_width=50, any_key_closes=True)
                 main_window['-URL-'].update('')
 
             else:
```

### Comparing `pyautosrt-0.2.0/pyautosrt.egg-info/PKG-INFO` & `pyautosrt-0.2.1/pyautosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.0
+Version: 0.2.1
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.0/setup.py` & `pyautosrt-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.0/test/__init__.py` & `pyautosrt-0.2.1/test/__init__.py`

 * *Files identical despite different names*

