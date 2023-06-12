# Comparing `tmp/robotframework-6.1b1.zip` & `tmp/robotframework-6.1rc1.zip`

## zipinfo {}

```diff
@@ -1,307 +1,308 @@
-Zip file size: 719096 bytes, number of entries: 305
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/
--rw-rw-r--  2.0 unx    11358 b- defN 23-Jan-08 21:34 robotframework-6.1b1/LICENSE.txt
--rw-rw-r--  2.0 unx     6176 b- defN 23-Mar-10 21:51 robotframework-6.1b1/tasks.py
--rw-rw-r--  2.0 unx     9280 b- defN 23-Mar-28 14:56 robotframework-6.1b1/BUILD.rst
--rw-rw-r--  2.0 unx      607 b- defN 23-Jan-08 21:34 robotframework-6.1b1/COPYRIGHT.txt
--rw-rw-r--  2.0 unx    12212 b- defN 23-Mar-28 14:56 robotframework-6.1b1/INSTALL.rst
--rwxrwxr-x  2.0 unx     3359 b- defN 23-May-05 21:12 robotframework-6.1b1/setup.py
--rw-rw-r--  2.0 unx     5444 b- defN 23-Mar-28 14:56 robotframework-6.1b1/README.rst
--rw-rw-r--  2.0 unx    11985 b- defN 23-Mar-10 21:51 robotframework-6.1b1/CONTRIBUTING.rst
--rw-rw-r--  2.0 unx      228 b- defN 23-Jan-08 21:34 robotframework-6.1b1/MANIFEST.in
--rw-rw-r--  2.0 unx     6417 b- defN 23-Jan-08 21:34 robotframework-6.1b1/AUTHORS.rst
--rw-rw-r--  2.0 unx     8685 b- defN 23-May-05 21:54 robotframework-6.1b1/PKG-INFO
--rw-rw-r--  2.0 unx       38 b- defN 23-May-05 21:54 robotframework-6.1b1/setup.cfg
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/result/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/output/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/conf/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/variables/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/libdocpkg/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/reporting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/running/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/utils/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/parsing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/libraries/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/api/
--rw-rw-r--  2.0 unx     1353 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/pythonpathsetter.py
--rwxrwxr-x  2.0 unx    22432 b- defN 23-Apr-12 21:16 robotframework-6.1b1/src/robot/rebot.py
--rwxrwxr-x  2.0 unx    12523 b- defN 23-Apr-12 21:16 robotframework-6.1b1/src/robot/libdoc.py
--rw-rw-r--  2.0 unx    10709 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/errors.py
--rwxrwxr-x  2.0 unx    11316 b- defN 23-Apr-12 21:16 robotframework-6.1b1/src/robot/testdoc.py
--rw-rw-r--  2.0 unx     2121 b- defN 23-Mar-30 02:33 robotframework-6.1b1/src/robot/__init__.py
--rw-rw-r--  2.0 unx     1405 b- defN 23-May-05 21:12 robotframework-6.1b1/src/robot/version.py
--rwxrwxr-x  2.0 unx      803 b- defN 23-Apr-12 21:14 robotframework-6.1b1/src/robot/__main__.py
--rwxrwxr-x  2.0 unx    31972 b- defN 23-Apr-26 10:51 robotframework-6.1b1/src/robot/run.py
--rw-rw-r--  2.0 unx    13316 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/result/xmlelementhandlers.py
--rw-rw-r--  2.0 unx     5760 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/result/executionresult.py
--rw-rw-r--  2.0 unx     1165 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/result/messagefilter.py
--rw-rw-r--  2.0 unx     2306 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/result/suiteteardownfailed.py
--rw-rw-r--  2.0 unx     2645 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/result/flattenkeywordmatcher.py
--rw-rw-r--  2.0 unx     5032 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/result/merger.py
--rw-rw-r--  2.0 unx     8276 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/result/resultbuilder.py
--rw-rw-r--  2.0 unx     1797 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/result/executionerrors.py
--rw-rw-r--  2.0 unx     1457 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/result/modeldeprecation.py
--rw-rw-r--  2.0 unx     2084 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/result/__init__.py
--rw-rw-r--  2.0 unx     5614 b- defN 23-Apr-04 23:22 robotframework-6.1b1/src/robot/result/keywordremover.py
--rw-rw-r--  2.0 unx     3926 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/result/visitor.py
--rw-rw-r--  2.0 unx    25861 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/result/model.py
--rw-rw-r--  2.0 unx     2561 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/result/configurer.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/output/console/
--rw-rw-r--  2.0 unx     6772 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/output/listeners.py
--rw-rw-r--  2.0 unx     3368 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/output/output.py
--rw-rw-r--  2.0 unx     3797 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/output/listenermethods.py
--rw-rw-r--  2.0 unx     2678 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/output/pyloggingconf.py
--rw-rw-r--  2.0 unx     1899 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/output/filelogger.py
--rw-rw-r--  2.0 unx     5159 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/output/loggerhelper.py
--rw-rw-r--  2.0 unx     2257 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/output/stdoutlogsplitter.py
--rw-rw-r--  2.0 unx    10129 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/output/logger.py
--rw-rw-r--  2.0 unx     2098 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/output/librarylogger.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/output/__init__.py
--rw-rw-r--  2.0 unx     3507 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/output/debugfile.py
--rw-rw-r--  2.0 unx    10611 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/output/xmllogger.py
--rw-rw-r--  2.0 unx     6060 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/output/listenerarguments.py
--rw-rw-r--  2.0 unx     1005 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/output/console/quiet.py
--rw-rw-r--  2.0 unx     6034 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/output/console/verbose.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/output/console/__init__.py
--rw-rw-r--  2.0 unx     3434 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/output/console/dotted.py
--rw-rw-r--  2.0 unx     6807 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/output/console/highlighting.py
--rw-rw-r--  2.0 unx     2540 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/model/message.py
--rw-rw-r--  2.0 unx     5611 b- defN 23-Apr-04 23:06 robotframework-6.1b1/src/robot/model/stats.py
--rw-rw-r--  2.0 unx     7197 b- defN 23-Apr-06 17:11 robotframework-6.1b1/src/robot/model/testcase.py
--rw-rw-r--  2.0 unx     6968 b- defN 23-Apr-25 18:26 robotframework-6.1b1/src/robot/model/tags.py
--rw-rw-r--  2.0 unx     1312 b- defN 23-Apr-04 23:37 robotframework-6.1b1/src/robot/model/fixture.py
--rw-rw-r--  2.0 unx     8818 b- defN 23-Apr-06 20:10 robotframework-6.1b1/src/robot/model/body.py
--rw-rw-r--  2.0 unx     7742 b- defN 23-Apr-05 17:01 robotframework-6.1b1/src/robot/model/itemlist.py
--rw-rw-r--  2.0 unx    12228 b- defN 23-Apr-28 16:14 robotframework-6.1b1/src/robot/model/testsuite.py
--rw-rw-r--  2.0 unx    11299 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/model/control.py
--rw-rw-r--  2.0 unx     1112 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/model/metadata.py
--rw-rw-r--  2.0 unx     2218 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/model/suitestatistics.py
--rw-rw-r--  2.0 unx     2115 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/model/modifier.py
--rw-rw-r--  2.0 unx     4933 b- defN 23-Apr-06 17:11 robotframework-6.1b1/src/robot/model/keyword.py
--rw-rw-r--  2.0 unx     1682 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/model/namepatterns.py
--rw-rw-r--  2.0 unx     1360 b- defN 23-Apr-04 19:08 robotframework-6.1b1/src/robot/model/tagsetter.py
--rw-rw-r--  2.0 unx     1829 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/model/__init__.py
--rw-rw-r--  2.0 unx    21366 b- defN 23-May-05 21:05 robotframework-6.1b1/src/robot/model/visitor.py
--rw-rw-r--  2.0 unx     2615 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/model/totalstatistics.py
--rw-rw-r--  2.0 unx     4060 b- defN 23-Apr-05 00:37 robotframework-6.1b1/src/robot/model/filter.py
--rw-rw-r--  2.0 unx     7512 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/model/modelobject.py
--rw-rw-r--  2.0 unx     3400 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/model/configurer.py
--rw-rw-r--  2.0 unx     2632 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/model/statistics.py
--rw-rw-r--  2.0 unx     4992 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/model/tagstatistics.py
--rw-rw-r--  2.0 unx    26226 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/conf/settings.py
--rw-rw-r--  2.0 unx     1255 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/conf/__init__.py
--rw-rw-r--  2.0 unx    47767 b- defN 23-May-03 17:44 robotframework-6.1b1/src/robot/conf/languages.py
--rw-rw-r--  2.0 unx     2555 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/conf/gatherfailed.py
--rw-rw-r--  2.0 unx     2823 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/variables.py
--rw-rw-r--  2.0 unx     9222 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/variables/scopes.py
--rw-rw-r--  2.0 unx     4421 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/variables/store.py
--rw-rw-r--  2.0 unx     8339 b- defN 23-Apr-05 21:52 robotframework-6.1b1/src/robot/variables/search.py
--rw-rw-r--  2.0 unx     8968 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/replacer.py
--rw-rw-r--  2.0 unx     8602 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/assigner.py
--rw-rw-r--  2.0 unx     1729 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/variables/notfound.py
--rw-rw-r--  2.0 unx     4747 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/finders.py
--rw-rw-r--  2.0 unx     1380 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/variables/__init__.py
--rw-rw-r--  2.0 unx     6798 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/variables/filesetter.py
--rw-rw-r--  2.0 unx     5683 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/variables/evaluation.py
--rw-rw-r--  2.0 unx     5348 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/variables/tablesetter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/variables/resolvable.py
--rw-rw-r--  2.0 unx     1172 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libdocpkg/writer.py
--rw-rw-r--  2.0 unx     4620 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libdocpkg/builder.py
--rw-rw-r--  2.0 unx     5673 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/libdocpkg/jsonbuilder.py
--rw-rw-r--  2.0 unx     1397 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libdocpkg/htmlwriter.py
--rw-rw-r--  2.0 unx     1767 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libdocpkg/output.py
--rw-rw-r--  2.0 unx      841 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/libdocpkg/jsonwriter.py
--rw-rw-r--  2.0 unx     6943 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libdocpkg/xmlwriter.py
--rw-rw-r--  2.0 unx     7609 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libdocpkg/standardtypes.py
--rw-rw-r--  2.0 unx     7130 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/libdocpkg/robotbuilder.py
--rwxrwxr-x  2.0 unx     3586 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/libdocpkg/consoleviewer.py
--rw-rw-r--  2.0 unx     4311 b- defN 23-Mar-10 21:54 robotframework-6.1b1/src/robot/libdocpkg/datatypes.py
--rw-rw-r--  2.0 unx      835 b- defN 23-Mar-14 09:13 robotframework-6.1b1/src/robot/libdocpkg/__init__.py
--rw-rw-r--  2.0 unx     5293 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libdocpkg/htmlutils.py
--rw-rw-r--  2.0 unx     7993 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libdocpkg/model.py
--rw-rw-r--  2.0 unx     7082 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/libdocpkg/xmlbuilder.py
--rw-rw-r--  2.0 unx     3409 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/reporting/xunitwriter.py
--rw-rw-r--  2.0 unx     8029 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/reporting/jsmodelbuilders.py
--rw-rw-r--  2.0 unx     3984 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/reporting/jsbuildingcontext.py
--rw-rw-r--  2.0 unx     4022 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/reporting/jswriter.py
--rw-rw-r--  2.0 unx     1671 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/reporting/stringcache.py
--rw-rw-r--  2.0 unx     1192 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/reporting/__init__.py
--rw-rw-r--  2.0 unx     5674 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/reporting/resultwriter.py
--rw-rw-r--  2.0 unx     2482 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/reporting/logreportwriters.py
--rw-rw-r--  2.0 unx     3525 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/reporting/jsexecutionresult.py
--rw-rw-r--  2.0 unx     1044 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/reporting/outputwriter.py
--rw-rw-r--  2.0 unx     1498 b- defN 23-May-04 19:41 robotframework-6.1b1/src/robot/reporting/expandkeywordmatcher.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/running/timeouts/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/running/builder/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/running/arguments/
--rw-rw-r--  2.0 unx     8505 b- defN 23-Apr-05 21:52 robotframework-6.1b1/src/robot/running/context.py
--rw-rw-r--  2.0 unx     9604 b- defN 23-Apr-05 17:43 robotframework-6.1b1/src/robot/running/librarykeywordrunner.py
--rw-rw-r--  2.0 unx    11770 b- defN 23-Apr-24 20:14 robotframework-6.1b1/src/robot/running/handlers.py
--rw-rw-r--  2.0 unx     1159 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/modelcombiner.py
--rw-rw-r--  2.0 unx     2602 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/libraryscopes.py
--rw-rw-r--  2.0 unx     3072 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/signalhandler.py
--rw-rw-r--  2.0 unx    10918 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/userkeywordrunner.py
--rw-rw-r--  2.0 unx    28966 b- defN 23-May-05 16:04 robotframework-6.1b1/src/robot/running/bodyrunner.py
--rw-rw-r--  2.0 unx     2647 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/usererrorhandler.py
--rw-rw-r--  2.0 unx    11206 b- defN 23-Apr-25 17:25 robotframework-6.1b1/src/robot/running/suiterunner.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Mar-15 16:57 robotframework-6.1b1/src/robot/running/status.py
--rw-rw-r--  2.0 unx     3720 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/runkwregister.py
--rw-rw-r--  2.0 unx    15721 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/running/testlibraries.py
--rw-rw-r--  2.0 unx     3334 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/outputcapture.py
--rw-rw-r--  2.0 unx     3966 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/userkeyword.py
--rw-rw-r--  2.0 unx     4803 b- defN 23-May-05 20:41 robotframework-6.1b1/src/robot/running/__init__.py
--rw-rw-r--  2.0 unx     1772 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/randomizer.py
--rw-rw-r--  2.0 unx    22162 b- defN 23-Apr-24 20:15 robotframework-6.1b1/src/robot/running/namespace.py
--rw-rw-r--  2.0 unx     3399 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/statusreporter.py
--rw-rw-r--  2.0 unx     2366 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/running/handlerstore.py
--rw-rw-r--  2.0 unx     4787 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/dynamicmethods.py
--rw-rw-r--  2.0 unx    29220 b- defN 23-May-02 15:52 robotframework-6.1b1/src/robot/running/model.py
--rw-rw-r--  2.0 unx     5816 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/importer.py
--rw-rw-r--  2.0 unx     1240 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/timeouts/posix.py
--rw-rw-r--  2.0 unx     4015 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/timeouts/__init__.py
--rw-rw-r--  2.0 unx     2320 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/timeouts/windows.py
--rw-rw-r--  2.0 unx     6444 b- defN 23-Apr-28 15:47 robotframework-6.1b1/src/robot/running/builder/parsers.py
--rw-rw-r--  2.0 unx    22451 b- defN 23-May-03 02:14 robotframework-6.1b1/src/robot/running/builder/transformers.py
--rw-rw-r--  2.0 unx     6737 b- defN 23-May-05 20:30 robotframework-6.1b1/src/robot/running/builder/settings.py
--rw-rw-r--  2.0 unx    12795 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/running/builder/builders.py
--rw-rw-r--  2.0 unx      772 b- defN 23-Apr-25 21:50 robotframework-6.1b1/src/robot/running/builder/__init__.py
--rw-rw-r--  2.0 unx     2975 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/arguments/argumentmapper.py
--rw-rw-r--  2.0 unx     3475 b- defN 23-Mar-10 21:54 robotframework-6.1b1/src/robot/running/arguments/argumentconverter.py
--rw-rw-r--  2.0 unx     4980 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/running/arguments/argumentresolver.py
--rw-rw-r--  2.0 unx     5939 b- defN 23-Mar-14 09:13 robotframework-6.1b1/src/robot/running/arguments/embedded.py
--rw-rw-r--  2.0 unx     4291 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/running/arguments/customconverters.py
--rw-rw-r--  2.0 unx    26053 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/running/arguments/typeconverters.py
--rw-rw-r--  2.0 unx     2331 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/running/arguments/typevalidator.py
--rw-rw-r--  2.0 unx     8547 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/running/arguments/argumentspec.py
--rw-rw-r--  2.0 unx     8520 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/running/arguments/argumentparser.py
--rw-rw-r--  2.0 unx     4349 b- defN 23-Apr-25 17:26 robotframework-6.1b1/src/robot/running/arguments/argumentvalidator.py
--rw-rw-r--  2.0 unx     1010 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/running/arguments/__init__.py
--rw-rw-r--  2.0 unx     2052 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/robotio.py
--rw-rw-r--  2.0 unx     3542 b- defN 23-Apr-21 15:51 robotframework-6.1b1/src/robot/utils/filereader.py
--rw-rw-r--  2.0 unx     1586 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/sortable.py
--rw-rw-r--  2.0 unx     4102 b- defN 23-Mar-15 02:28 robotframework-6.1b1/src/robot/utils/escaping.py
--rw-rw-r--  2.0 unx     2956 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/restreader.py
--rw-rw-r--  2.0 unx     1955 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/frange.py
--rw-rw-r--  2.0 unx     6131 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/connectioncache.py
--rw-rw-r--  2.0 unx     4314 b- defN 23-Apr-28 17:01 robotframework-6.1b1/src/robot/utils/normalizing.py
--rw-rw-r--  2.0 unx     3956 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/utils/markupwriters.py
--rw-rw-r--  2.0 unx     3202 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/utils/setter.py
--rw-rw-r--  2.0 unx      809 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/compress.py
--rw-rw-r--  2.0 unx     5373 b- defN 23-Apr-28 17:15 robotframework-6.1b1/src/robot/utils/misc.py
--rw-rw-r--  2.0 unx     2254 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/dotdict.py
--rw-rw-r--  2.0 unx     3721 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/recommendations.py
--rw-rw-r--  2.0 unx     5436 b- defN 23-Apr-27 02:29 robotframework-6.1b1/src/robot/utils/text.py
--rw-rw-r--  2.0 unx     2149 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/unic.py
--rw-rw-r--  2.0 unx     1664 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/markuputils.py
--rw-rw-r--  2.0 unx     5391 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/utils/robotpath.py
--rw-rw-r--  2.0 unx    16133 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/utils/robottime.py
--rw-rw-r--  2.0 unx     3221 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/utils/encoding.py
--rw-rw-r--  2.0 unx     3262 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/encodingsniffer.py
--rw-rw-r--  2.0 unx    15942 b- defN 23-Apr-24 23:28 robotframework-6.1b1/src/robot/utils/argumentparser.py
--rw-rw-r--  2.0 unx     8776 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/asserts.py
--rw-rw-r--  2.0 unx     4569 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/utils/__init__.py
--rw-rw-r--  2.0 unx     4300 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/application.py
--rw-rw-r--  2.0 unx     2635 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/etreewrapper.py
--rw-rw-r--  2.0 unx     3042 b- defN 23-Apr-21 14:40 robotframework-6.1b1/src/robot/utils/match.py
--rw-rw-r--  2.0 unx     4673 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/error.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/utils/robotenv.py
--rw-rw-r--  2.0 unx     9851 b- defN 23-Mar-27 20:53 robotframework-6.1b1/src/robot/utils/htmlformatters.py
--rw-rw-r--  2.0 unx     7487 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/charwidth.py
--rw-rw-r--  2.0 unx     1389 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/utils/platform.py
--rw-rw-r--  2.0 unx    13504 b- defN 23-Mar-31 19:19 robotframework-6.1b1/src/robot/utils/importer.py
--rw-rw-r--  2.0 unx      902 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/utils/robotinspect.py
--rw-rw-r--  2.0 unx     5565 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/utils/robottypes.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/libdoc/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/rebot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/lib/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/testdoc/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/htmldata/common/
--rw-rw-r--  2.0 unx     4127 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/htmldata/jsonwriter.py
--rw-rw-r--  2.0 unx     3476 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/htmlfilewriter.py
--rw-rw-r--  2.0 unx     2535 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/template.py
--rw-rw-r--  2.0 unx      983 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/__init__.py
--rw-rw-r--  2.0 unx      138 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/libdoc/print.css
--rw-rw-r--  2.0 unx    14346 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.css
--rw-rw-r--  2.0 unx    28636 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.html
--rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/libdoc/__init__.py
--rw-rw-r--  2.0 unx     8894 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/libdoc/pygments.css
--rw-rw-r--  2.0 unx     1341 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/libdoc/doc_formatting.css
--rw-rw-r--  2.0 unx     4646 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/common.css
--rw-rw-r--  2.0 unx     3413 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/report.css
--rw-rw-r--  2.0 unx     6955 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/htmldata/rebot/log.js
--rw-rw-r--  2.0 unx      699 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/print.css
--rw-rw-r--  2.0 unx     6510 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/view.js
--rw-rw-r--  2.0 unx    30836 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/report.html
--rw-rw-r--  2.0 unx    10023 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/htmldata/rebot/testdata.js
--rw-rw-r--  2.0 unx     7155 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/util.js
--rw-rw-r--  2.0 unx    11525 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/htmldata/rebot/model.js
--rw-rw-r--  2.0 unx    15416 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/htmldata/rebot/log.html
--rw-rw-r--  2.0 unx     1487 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/fileloading.js
--rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/rebot/__init__.py
--rw-rw-r--  2.0 unx      903 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/rebot/doc_formatting.css
--rw-rw-r--  2.0 unx     7390 b- defN 23-Feb-28 18:30 robotframework-6.1b1/src/robot/htmldata/rebot/log.css
--rw-rw-r--  2.0 unx    13667 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jsxcompressor.min.js
--rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/lib/__init__.py
--rw-rw-r--  2.0 unx    43881 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jquery.tablesorter.min.js
--rw-rw-r--  2.0 unx     1524 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jquery.highlight.min.js
--rw-rw-r--  2.0 unx    89476 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jquery.min.js
--rw-rw-r--  2.0 unx     6141 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/lib/jquery.tmpl.min.js
--rw-rw-r--  2.0 unx      153 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.css
--rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/testdoc/__init__.py
--rw-rw-r--  2.0 unx     9765 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.html
--rw-rw-r--  2.0 unx      872 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/common/storage.js
--rw-rw-r--  2.0 unx      373 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/htmldata/common/js_disabled.css
--rw-rw-r--  2.0 unx      643 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/htmldata/common/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/parsing/model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/parsing/parser/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-05 21:54 robotframework-6.1b1/src/robot/parsing/lexer/
--rw-rw-r--  2.0 unx     6451 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/parsing/suitestructure.py
--rw-rw-r--  2.0 unx     1311 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/parsing/__init__.py
--rw-rw-r--  2.0 unx    14745 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/model/blocks.py
--rw-rw-r--  2.0 unx     1035 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/model/__init__.py
--rw-rw-r--  2.0 unx     2355 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/parsing/model/visitor.py
--rw-rw-r--  2.0 unx    44561 b- defN 23-May-05 17:04 robotframework-6.1b1/src/robot/parsing/model/statements.py
--rw-rw-r--  2.0 unx     3778 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/parser/blockparsers.py
--rw-rw-r--  2.0 unx     5321 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/parser/parser.py
--rw-rw-r--  2.0 unx      710 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/parsing/parser/__init__.py
--rw-rw-r--  2.0 unx     4036 b- defN 23-May-03 16:09 robotframework-6.1b1/src/robot/parsing/parser/fileparser.py
--rw-rw-r--  2.0 unx     7778 b- defN 23-May-03 20:51 robotframework-6.1b1/src/robot/parsing/lexer/lexer.py
--rw-rw-r--  2.0 unx    11601 b- defN 23-May-03 20:46 robotframework-6.1b1/src/robot/parsing/lexer/blocklexers.py
--rw-rw-r--  2.0 unx     5380 b- defN 23-May-03 20:52 robotframework-6.1b1/src/robot/parsing/lexer/context.py
--rw-rw-r--  2.0 unx     8487 b- defN 23-May-03 21:02 robotframework-6.1b1/src/robot/parsing/lexer/settings.py
--rw-rw-r--  2.0 unx     9113 b- defN 23-May-03 20:45 robotframework-6.1b1/src/robot/parsing/lexer/tokens.py
--rw-rw-r--  2.0 unx    10328 b- defN 23-May-03 20:45 robotframework-6.1b1/src/robot/parsing/lexer/statementlexers.py
--rw-rw-r--  2.0 unx      755 b- defN 23-May-03 20:47 robotframework-6.1b1/src/robot/parsing/lexer/__init__.py
--rw-rw-r--  2.0 unx     5565 b- defN 23-May-03 01:27 robotframework-6.1b1/src/robot/parsing/lexer/tokenizer.py
--rw-rw-r--  2.0 unx    71458 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/libraries/XML.py
--rw-rw-r--  2.0 unx    14289 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Screenshot.py
--rw-rw-r--  2.0 unx     1104 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/libraries/Easter.py
--rw-rw-r--  2.0 unx     5960 b- defN 23-Mar-28 14:56 robotframework-6.1b1/src/robot/libraries/dialogs_py.py
--rw-rw-r--  2.0 unx    36128 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/String.py
--rw-rw-r--  2.0 unx    54972 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Telnet.py
--rw-rw-r--  2.0 unx    28349 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/DateTime.py
--rw-rw-r--  2.0 unx    10309 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Remote.py
--rw-rw-r--  2.0 unx    64676 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/OperatingSystem.py
--rw-rw-r--  2.0 unx    43712 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Collections.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/libraries/__init__.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Reserved.py
--rw-rw-r--  2.0 unx     4567 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/libraries/Dialogs.py
--rw-rw-r--  2.0 unx   187410 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/libraries/BuiltIn.py
--rw-rw-r--  2.0 unx    44928 b- defN 23-Apr-24 23:30 robotframework-6.1b1/src/robot/libraries/Process.py
--rw-rw-r--  2.0 unx    22854 b- defN 23-May-05 20:01 robotframework-6.1b1/src/robot/api/interfaces.py
--rw-rw-r--  2.0 unx    21210 b- defN 23-Apr-04 15:38 robotframework-6.1b1/src/robot/api/parsing.py
--rw-rw-r--  2.0 unx     5157 b- defN 23-Mar-10 21:51 robotframework-6.1b1/src/robot/api/deco.py
--rw-rw-r--  2.0 unx     4918 b- defN 23-Apr-04 12:26 robotframework-6.1b1/src/robot/api/logger.py
--rw-rw-r--  2.0 unx     4009 b- defN 23-Apr-25 23:34 robotframework-6.1b1/src/robot/api/__init__.py
--rw-rw-r--  2.0 unx     3140 b- defN 23-Jan-08 21:34 robotframework-6.1b1/src/robot/api/exceptions.py
--rw-rw-r--  2.0 unx     8930 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx      108 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/entry_points.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     8685 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 23-May-05 21:54 robotframework-6.1b1/src/robotframework.egg-info/top_level.txt
-305 files, 2338076 bytes uncompressed, 664580 bytes compressed:  71.6%
+Zip file size: 729166 bytes, number of entries: 306
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/
+-rw-rw-r--  2.0 unx    11358 b- defN 23-Jan-08 21:34 robotframework-6.1rc1/LICENSE.txt
+-rw-rw-r--  2.0 unx     6176 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/tasks.py
+-rw-rw-r--  2.0 unx     9280 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/BUILD.rst
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jun-01 01:14 robotframework-6.1rc1/COPYRIGHT.txt
+-rw-rw-r--  2.0 unx    12212 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/INSTALL.rst
+-rwxrwxr-x  2.0 unx     3399 b- defN 23-Jun-05 17:47 robotframework-6.1rc1/setup.py
+-rw-rw-r--  2.0 unx     5444 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/README.rst
+-rw-rw-r--  2.0 unx    11985 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/CONTRIBUTING.rst
+-rw-rw-r--  2.0 unx      228 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/MANIFEST.in
+-rw-rw-r--  2.0 unx     6417 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/AUTHORS.rst
+-rw-rw-r--  2.0 unx     8738 b- defN 23-Jun-05 17:48 robotframework-6.1rc1/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jun-05 17:48 robotframework-6.1rc1/setup.cfg
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robotframework.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/result/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/output/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/conf/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/variables/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/libdocpkg/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/reporting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/running/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/utils/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/htmldata/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/parsing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/libraries/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/api/
+-rw-rw-r--  2.0 unx     1353 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/pythonpathsetter.py
+-rwxrwxr-x  2.0 unx    22432 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/rebot.py
+-rwxrwxr-x  2.0 unx    12583 b- defN 23-Jun-02 11:10 robotframework-6.1rc1/src/robot/libdoc.py
+-rw-rw-r--  2.0 unx    10709 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/errors.py
+-rwxrwxr-x  2.0 unx    11316 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/testdoc.py
+-rw-rw-r--  2.0 unx     2121 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/__init__.py
+-rw-rw-r--  2.0 unx     1406 b- defN 23-Jun-05 17:47 robotframework-6.1rc1/src/robot/version.py
+-rwxrwxr-x  2.0 unx      803 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/__main__.py
+-rwxrwxr-x  2.0 unx    32434 b- defN 23-Jun-01 23:10 robotframework-6.1rc1/src/robot/run.py
+-rw-rw-r--  2.0 unx    13254 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/xmlelementhandlers.py
+-rw-rw-r--  2.0 unx     5760 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/executionresult.py
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/messagefilter.py
+-rw-rw-r--  2.0 unx     2306 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/suiteteardownfailed.py
+-rw-rw-r--  2.0 unx     2645 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/flattenkeywordmatcher.py
+-rw-rw-r--  2.0 unx     5032 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/merger.py
+-rw-rw-r--  2.0 unx     8276 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/resultbuilder.py
+-rw-rw-r--  2.0 unx     1797 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/executionerrors.py
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/modeldeprecation.py
+-rw-rw-r--  2.0 unx     2084 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/__init__.py
+-rw-rw-r--  2.0 unx     5614 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/keywordremover.py
+-rw-rw-r--  2.0 unx     3926 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/visitor.py
+-rw-rw-r--  2.0 unx    33275 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/model.py
+-rw-rw-r--  2.0 unx     2561 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/result/configurer.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/output/console/
+-rw-rw-r--  2.0 unx     6772 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/listeners.py
+-rw-rw-r--  2.0 unx     3368 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/output.py
+-rw-rw-r--  2.0 unx     3797 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/listenermethods.py
+-rw-rw-r--  2.0 unx     2678 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/pyloggingconf.py
+-rw-rw-r--  2.0 unx     1899 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/filelogger.py
+-rw-rw-r--  2.0 unx     5159 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/loggerhelper.py
+-rw-rw-r--  2.0 unx     2257 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/stdoutlogsplitter.py
+-rw-rw-r--  2.0 unx    10129 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/logger.py
+-rw-rw-r--  2.0 unx     2098 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/librarylogger.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-01 01:14 robotframework-6.1rc1/src/robot/output/__init__.py
+-rw-rw-r--  2.0 unx     3507 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/debugfile.py
+-rw-rw-r--  2.0 unx    10611 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/xmllogger.py
+-rw-rw-r--  2.0 unx     6060 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/listenerarguments.py
+-rw-rw-r--  2.0 unx     1005 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/console/quiet.py
+-rw-rw-r--  2.0 unx     6034 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/console/verbose.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-01 01:14 robotframework-6.1rc1/src/robot/output/console/__init__.py
+-rw-rw-r--  2.0 unx     3434 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/console/dotted.py
+-rw-rw-r--  2.0 unx     6807 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/output/console/highlighting.py
+-rw-rw-r--  2.0 unx     2540 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/message.py
+-rw-rw-r--  2.0 unx     5611 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/stats.py
+-rw-rw-r--  2.0 unx     7556 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/testcase.py
+-rw-rw-r--  2.0 unx     7704 b- defN 23-Jun-02 00:15 robotframework-6.1rc1/src/robot/model/tags.py
+-rw-rw-r--  2.0 unx     1777 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/fixture.py
+-rw-rw-r--  2.0 unx    12239 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/body.py
+-rw-rw-r--  2.0 unx     7958 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/itemlist.py
+-rw-rw-r--  2.0 unx    16534 b- defN 23-Jun-05 13:39 robotframework-6.1rc1/src/robot/model/testsuite.py
+-rw-rw-r--  2.0 unx    13418 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/control.py
+-rw-rw-r--  2.0 unx     1355 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/metadata.py
+-rw-rw-r--  2.0 unx     2218 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/suitestatistics.py
+-rw-rw-r--  2.0 unx     2115 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/modifier.py
+-rw-rw-r--  2.0 unx     5135 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/keyword.py
+-rw-rw-r--  2.0 unx     1769 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/namepatterns.py
+-rw-rw-r--  2.0 unx     1360 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/tagsetter.py
+-rw-rw-r--  2.0 unx     1883 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/__init__.py
+-rw-rw-r--  2.0 unx    21366 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/visitor.py
+-rw-rw-r--  2.0 unx     2721 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/totalstatistics.py
+-rw-rw-r--  2.0 unx     4060 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/filter.py
+-rw-rw-r--  2.0 unx     9306 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/modelobject.py
+-rw-rw-r--  2.0 unx     3400 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/configurer.py
+-rw-rw-r--  2.0 unx     2632 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/statistics.py
+-rw-rw-r--  2.0 unx     4992 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/model/tagstatistics.py
+-rw-rw-r--  2.0 unx    26418 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/conf/settings.py
+-rw-rw-r--  2.0 unx     1255 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/conf/__init__.py
+-rw-rw-r--  2.0 unx    48030 b- defN 23-Jun-02 16:20 robotframework-6.1rc1/src/robot/conf/languages.py
+-rw-rw-r--  2.0 unx     2555 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/conf/gatherfailed.py
+-rw-rw-r--  2.0 unx     2823 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/variables.py
+-rw-rw-r--  2.0 unx     9222 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/scopes.py
+-rw-rw-r--  2.0 unx     4421 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/store.py
+-rw-rw-r--  2.0 unx     8556 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/search.py
+-rw-rw-r--  2.0 unx     8968 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/replacer.py
+-rw-rw-r--  2.0 unx    11286 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/assigner.py
+-rw-rw-r--  2.0 unx     1729 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/notfound.py
+-rw-rw-r--  2.0 unx     4747 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/finders.py
+-rw-rw-r--  2.0 unx     1380 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/__init__.py
+-rw-rw-r--  2.0 unx     6798 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/filesetter.py
+-rw-rw-r--  2.0 unx     5701 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/evaluation.py
+-rw-rw-r--  2.0 unx     5348 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/tablesetter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/variables/resolvable.py
+-rw-rw-r--  2.0 unx     1172 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/writer.py
+-rw-rw-r--  2.0 unx     4620 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/builder.py
+-rw-rw-r--  2.0 unx     5673 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/jsonbuilder.py
+-rw-rw-r--  2.0 unx     1397 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/htmlwriter.py
+-rw-rw-r--  2.0 unx     1767 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/output.py
+-rw-rw-r--  2.0 unx      841 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/jsonwriter.py
+-rw-rw-r--  2.0 unx     6943 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/xmlwriter.py
+-rw-rw-r--  2.0 unx     7609 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/standardtypes.py
+-rw-rw-r--  2.0 unx     7130 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/robotbuilder.py
+-rwxrwxr-x  2.0 unx     3586 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/consoleviewer.py
+-rw-rw-r--  2.0 unx     4321 b- defN 23-Jun-02 11:10 robotframework-6.1rc1/src/robot/libdocpkg/datatypes.py
+-rw-rw-r--  2.0 unx      835 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/__init__.py
+-rw-rw-r--  2.0 unx     5293 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/htmlutils.py
+-rw-rw-r--  2.0 unx     7993 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/model.py
+-rw-rw-r--  2.0 unx     7082 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libdocpkg/xmlbuilder.py
+-rw-rw-r--  2.0 unx     3409 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/xunitwriter.py
+-rw-rw-r--  2.0 unx     8029 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/jsmodelbuilders.py
+-rw-rw-r--  2.0 unx     3984 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/jsbuildingcontext.py
+-rw-rw-r--  2.0 unx     4022 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/jswriter.py
+-rw-rw-r--  2.0 unx     1671 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/stringcache.py
+-rw-rw-r--  2.0 unx     1192 b- defN 23-Jun-01 01:14 robotframework-6.1rc1/src/robot/reporting/__init__.py
+-rw-rw-r--  2.0 unx     5674 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/resultwriter.py
+-rw-rw-r--  2.0 unx     2482 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/logreportwriters.py
+-rw-rw-r--  2.0 unx     3525 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/jsexecutionresult.py
+-rw-rw-r--  2.0 unx     1044 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/outputwriter.py
+-rw-rw-r--  2.0 unx     1498 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/reporting/expandkeywordmatcher.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/running/timeouts/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/running/builder/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/running/arguments/
+-rw-rw-r--  2.0 unx     8505 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/context.py
+-rw-rw-r--  2.0 unx     9604 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/librarykeywordrunner.py
+-rw-rw-r--  2.0 unx    11770 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/handlers.py
+-rw-rw-r--  2.0 unx     1159 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/modelcombiner.py
+-rw-rw-r--  2.0 unx     2602 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/libraryscopes.py
+-rw-rw-r--  2.0 unx     3072 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/signalhandler.py
+-rw-rw-r--  2.0 unx    10918 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/userkeywordrunner.py
+-rw-rw-r--  2.0 unx    28966 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/bodyrunner.py
+-rw-rw-r--  2.0 unx     2647 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/usererrorhandler.py
+-rw-rw-r--  2.0 unx    11206 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/suiterunner.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/status.py
+-rw-rw-r--  2.0 unx     3720 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/runkwregister.py
+-rw-rw-r--  2.0 unx    15721 b- defN 23-Jun-01 17:06 robotframework-6.1rc1/src/robot/running/testlibraries.py
+-rw-rw-r--  2.0 unx     3334 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/outputcapture.py
+-rw-rw-r--  2.0 unx     3966 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/userkeyword.py
+-rw-rw-r--  2.0 unx     4803 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/__init__.py
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/randomizer.py
+-rw-rw-r--  2.0 unx    22162 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/namespace.py
+-rw-rw-r--  2.0 unx     3399 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/statusreporter.py
+-rw-rw-r--  2.0 unx     2366 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/handlerstore.py
+-rw-rw-r--  2.0 unx     4787 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/dynamicmethods.py
+-rw-rw-r--  2.0 unx    32761 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/model.py
+-rw-rw-r--  2.0 unx     5837 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/importer.py
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/timeouts/posix.py
+-rw-rw-r--  2.0 unx     4015 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/timeouts/__init__.py
+-rw-rw-r--  2.0 unx     2320 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/timeouts/windows.py
+-rw-rw-r--  2.0 unx     6626 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/builder/parsers.py
+-rw-rw-r--  2.0 unx    22451 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/builder/transformers.py
+-rw-rw-r--  2.0 unx     6792 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/builder/settings.py
+-rw-rw-r--  2.0 unx    13969 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/builder/builders.py
+-rw-rw-r--  2.0 unx      772 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/builder/__init__.py
+-rw-rw-r--  2.0 unx     2975 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/argumentmapper.py
+-rw-rw-r--  2.0 unx     3475 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/argumentconverter.py
+-rw-rw-r--  2.0 unx     4980 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/argumentresolver.py
+-rw-rw-r--  2.0 unx     5939 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/embedded.py
+-rw-rw-r--  2.0 unx     4291 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/customconverters.py
+-rw-rw-r--  2.0 unx    26053 b- defN 23-Jun-02 10:45 robotframework-6.1rc1/src/robot/running/arguments/typeconverters.py
+-rw-rw-r--  2.0 unx     2331 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/typevalidator.py
+-rw-rw-r--  2.0 unx     8547 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/argumentspec.py
+-rw-rw-r--  2.0 unx     8520 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/argumentparser.py
+-rw-rw-r--  2.0 unx     4349 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/argumentvalidator.py
+-rw-rw-r--  2.0 unx     1010 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/running/arguments/__init__.py
+-rw-rw-r--  2.0 unx     2052 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/robotio.py
+-rw-rw-r--  2.0 unx     3542 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/filereader.py
+-rw-rw-r--  2.0 unx     1586 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/sortable.py
+-rw-rw-r--  2.0 unx     4102 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/escaping.py
+-rw-rw-r--  2.0 unx     2956 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/restreader.py
+-rw-rw-r--  2.0 unx     1955 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/frange.py
+-rw-rw-r--  2.0 unx     6131 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/connectioncache.py
+-rw-rw-r--  2.0 unx     4628 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/normalizing.py
+-rw-rw-r--  2.0 unx     3956 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/markupwriters.py
+-rw-rw-r--  2.0 unx     3309 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/setter.py
+-rw-rw-r--  2.0 unx      809 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/compress.py
+-rw-rw-r--  2.0 unx     5373 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/misc.py
+-rw-rw-r--  2.0 unx     2254 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/dotdict.py
+-rw-rw-r--  2.0 unx     3721 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/recommendations.py
+-rw-rw-r--  2.0 unx     5537 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/text.py
+-rw-rw-r--  2.0 unx     2149 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/unic.py
+-rw-rw-r--  2.0 unx     1664 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/markuputils.py
+-rw-rw-r--  2.0 unx     5391 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/robotpath.py
+-rw-rw-r--  2.0 unx    16133 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/robottime.py
+-rw-rw-r--  2.0 unx     3221 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/encoding.py
+-rw-rw-r--  2.0 unx     3262 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/encodingsniffer.py
+-rw-rw-r--  2.0 unx    15942 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/argumentparser.py
+-rw-rw-r--  2.0 unx     8776 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/asserts.py
+-rw-rw-r--  2.0 unx     4623 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/__init__.py
+-rw-rw-r--  2.0 unx     4300 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/application.py
+-rw-rw-r--  2.0 unx     2635 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/etreewrapper.py
+-rw-rw-r--  2.0 unx     3060 b- defN 23-Jun-02 00:15 robotframework-6.1rc1/src/robot/utils/match.py
+-rw-rw-r--  2.0 unx     4673 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/error.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-01 01:14 robotframework-6.1rc1/src/robot/utils/robotenv.py
+-rw-rw-r--  2.0 unx     9851 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/htmlformatters.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/typehints.py
+-rw-rw-r--  2.0 unx     7487 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/charwidth.py
+-rw-rw-r--  2.0 unx     1389 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/platform.py
+-rw-rw-r--  2.0 unx    13504 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/importer.py
+-rw-rw-r--  2.0 unx      902 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/robotinspect.py
+-rw-rw-r--  2.0 unx     5565 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/utils/robottypes.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/htmldata/libdoc/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/htmldata/rebot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/htmldata/lib/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/htmldata/testdoc/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/htmldata/common/
+-rw-rw-r--  2.0 unx     4127 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/jsonwriter.py
+-rw-rw-r--  2.0 unx     3476 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/htmlfilewriter.py
+-rw-rw-r--  2.0 unx     2535 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/template.py
+-rw-rw-r--  2.0 unx      983 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/__init__.py
+-rw-rw-r--  2.0 unx      138 b- defN 23-Jan-08 21:34 robotframework-6.1rc1/src/robot/htmldata/libdoc/print.css
+-rw-rw-r--  2.0 unx    14346 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/libdoc/libdoc.css
+-rw-rw-r--  2.0 unx    28643 b- defN 23-Jun-02 11:08 robotframework-6.1rc1/src/robot/htmldata/libdoc/libdoc.html
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/libdoc/__init__.py
+-rw-rw-r--  2.0 unx     8894 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/libdoc/pygments.css
+-rw-rw-r--  2.0 unx     1341 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/libdoc/doc_formatting.css
+-rw-rw-r--  2.0 unx     4646 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/common.css
+-rw-rw-r--  2.0 unx     3413 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/report.css
+-rw-rw-r--  2.0 unx     7146 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/log.js
+-rw-rw-r--  2.0 unx      699 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/print.css
+-rw-rw-r--  2.0 unx     6510 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/view.js
+-rw-rw-r--  2.0 unx    30877 b- defN 23-Jun-02 11:08 robotframework-6.1rc1/src/robot/htmldata/rebot/report.html
+-rw-rw-r--  2.0 unx    10023 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/testdata.js
+-rw-rw-r--  2.0 unx     7155 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/util.js
+-rw-rw-r--  2.0 unx    11525 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/model.js
+-rw-rw-r--  2.0 unx    15435 b- defN 23-Jun-02 11:08 robotframework-6.1rc1/src/robot/htmldata/rebot/log.html
+-rw-rw-r--  2.0 unx     1487 b- defN 23-Jan-08 21:34 robotframework-6.1rc1/src/robot/htmldata/rebot/fileloading.js
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/__init__.py
+-rw-rw-r--  2.0 unx      903 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/doc_formatting.css
+-rw-rw-r--  2.0 unx     7390 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/rebot/log.css
+-rw-rw-r--  2.0 unx    13667 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/lib/jsxcompressor.min.js
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/lib/__init__.py
+-rw-rw-r--  2.0 unx    43881 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/lib/jquery.tablesorter.min.js
+-rw-rw-r--  2.0 unx     1524 b- defN 23-Jan-08 21:34 robotframework-6.1rc1/src/robot/htmldata/lib/jquery.highlight.min.js
+-rw-rw-r--  2.0 unx    89476 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/lib/jquery.min.js
+-rw-rw-r--  2.0 unx     6141 b- defN 23-Jan-08 21:34 robotframework-6.1rc1/src/robot/htmldata/lib/jquery.tmpl.min.js
+-rw-rw-r--  2.0 unx      153 b- defN 23-Jan-08 21:34 robotframework-6.1rc1/src/robot/htmldata/testdoc/testdoc.css
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/testdoc/__init__.py
+-rw-rw-r--  2.0 unx     9765 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/testdoc/testdoc.html
+-rw-rw-r--  2.0 unx      872 b- defN 23-Jun-01 01:14 robotframework-6.1rc1/src/robot/htmldata/common/storage.js
+-rw-rw-r--  2.0 unx      373 b- defN 23-Jan-08 21:34 robotframework-6.1rc1/src/robot/htmldata/common/js_disabled.css
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/htmldata/common/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/parsing/model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/parsing/parser/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jun-05 17:48 robotframework-6.1rc1/src/robot/parsing/lexer/
+-rw-rw-r--  2.0 unx     8637 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/suitestructure.py
+-rw-rw-r--  2.0 unx     1311 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/__init__.py
+-rw-rw-r--  2.0 unx    14731 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/model/blocks.py
+-rw-rw-r--  2.0 unx     1035 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/model/__init__.py
+-rw-rw-r--  2.0 unx     2355 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/model/visitor.py
+-rw-rw-r--  2.0 unx    44561 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/model/statements.py
+-rw-rw-r--  2.0 unx     3778 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/parser/blockparsers.py
+-rw-rw-r--  2.0 unx     5321 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/parser/parser.py
+-rw-rw-r--  2.0 unx      710 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/parser/__init__.py
+-rw-rw-r--  2.0 unx     4036 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/parser/fileparser.py
+-rw-rw-r--  2.0 unx     7778 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/lexer/lexer.py
+-rw-rw-r--  2.0 unx    11601 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/lexer/blocklexers.py
+-rw-rw-r--  2.0 unx     5380 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/lexer/context.py
+-rw-rw-r--  2.0 unx     8487 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/lexer/settings.py
+-rw-rw-r--  2.0 unx     9113 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/lexer/tokens.py
+-rw-rw-r--  2.0 unx    10364 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/lexer/statementlexers.py
+-rw-rw-r--  2.0 unx      755 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/lexer/__init__.py
+-rw-rw-r--  2.0 unx     5565 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/parsing/lexer/tokenizer.py
+-rw-rw-r--  2.0 unx    71458 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/XML.py
+-rw-rw-r--  2.0 unx    14289 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/Screenshot.py
+-rw-rw-r--  2.0 unx     1104 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/Easter.py
+-rw-rw-r--  2.0 unx     5960 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/dialogs_py.py
+-rw-rw-r--  2.0 unx    36128 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/String.py
+-rw-rw-r--  2.0 unx    54972 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/Telnet.py
+-rw-rw-r--  2.0 unx    28349 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/DateTime.py
+-rw-rw-r--  2.0 unx    10309 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/Remote.py
+-rw-rw-r--  2.0 unx    64676 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/OperatingSystem.py
+-rw-rw-r--  2.0 unx    45482 b- defN 23-Jun-02 12:54 robotframework-6.1rc1/src/robot/libraries/Collections.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-01 01:14 robotframework-6.1rc1/src/robot/libraries/__init__.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/Reserved.py
+-rw-rw-r--  2.0 unx     4567 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/Dialogs.py
+-rw-rw-r--  2.0 unx   187436 b- defN 23-Jun-02 11:10 robotframework-6.1rc1/src/robot/libraries/BuiltIn.py
+-rw-rw-r--  2.0 unx    44928 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/libraries/Process.py
+-rw-rw-r--  2.0 unx    22854 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/api/interfaces.py
+-rw-rw-r--  2.0 unx    21210 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/api/parsing.py
+-rw-rw-r--  2.0 unx     5157 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/api/deco.py
+-rw-rw-r--  2.0 unx     4918 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/api/logger.py
+-rw-rw-r--  2.0 unx     4009 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/api/__init__.py
+-rw-rw-r--  2.0 unx     3140 b- defN 23-Jun-01 01:15 robotframework-6.1rc1/src/robot/api/exceptions.py
+-rw-rw-r--  2.0 unx     8959 b- defN 23-Jun-05 17:48 robotframework-6.1rc1/src/robotframework.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx      108 b- defN 23-Jun-05 17:48 robotframework-6.1rc1/src/robotframework.egg-info/entry_points.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-05 17:48 robotframework-6.1rc1/src/robotframework.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     8738 b- defN 23-Jun-05 17:48 robotframework-6.1rc1/src/robotframework.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jun-05 17:48 robotframework-6.1rc1/src/robotframework.egg-info/top_level.txt
+306 files, 2374690 bytes uncompressed, 673864 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,916 +1,919 @@
-Filename: robotframework-6.1b1/
+Filename: robotframework-6.1rc1/
 Comment: 
 
-Filename: robotframework-6.1b1/src/
+Filename: robotframework-6.1rc1/src/
 Comment: 
 
-Filename: robotframework-6.1b1/LICENSE.txt
+Filename: robotframework-6.1rc1/LICENSE.txt
 Comment: 
 
-Filename: robotframework-6.1b1/tasks.py
+Filename: robotframework-6.1rc1/tasks.py
 Comment: 
 
-Filename: robotframework-6.1b1/BUILD.rst
+Filename: robotframework-6.1rc1/BUILD.rst
 Comment: 
 
-Filename: robotframework-6.1b1/COPYRIGHT.txt
+Filename: robotframework-6.1rc1/COPYRIGHT.txt
 Comment: 
 
-Filename: robotframework-6.1b1/INSTALL.rst
+Filename: robotframework-6.1rc1/INSTALL.rst
 Comment: 
 
-Filename: robotframework-6.1b1/setup.py
+Filename: robotframework-6.1rc1/setup.py
 Comment: 
 
-Filename: robotframework-6.1b1/README.rst
+Filename: robotframework-6.1rc1/README.rst
 Comment: 
 
-Filename: robotframework-6.1b1/CONTRIBUTING.rst
+Filename: robotframework-6.1rc1/CONTRIBUTING.rst
 Comment: 
 
-Filename: robotframework-6.1b1/MANIFEST.in
+Filename: robotframework-6.1rc1/MANIFEST.in
 Comment: 
 
-Filename: robotframework-6.1b1/AUTHORS.rst
+Filename: robotframework-6.1rc1/AUTHORS.rst
 Comment: 
 
-Filename: robotframework-6.1b1/PKG-INFO
+Filename: robotframework-6.1rc1/PKG-INFO
 Comment: 
 
-Filename: robotframework-6.1b1/setup.cfg
+Filename: robotframework-6.1rc1/setup.cfg
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/
+Filename: robotframework-6.1rc1/src/robot/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robotframework.egg-info/
+Filename: robotframework-6.1rc1/src/robotframework.egg-info/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/
+Filename: robotframework-6.1rc1/src/robot/result/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/
+Filename: robotframework-6.1rc1/src/robot/output/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/
+Filename: robotframework-6.1rc1/src/robot/model/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/conf/
+Filename: robotframework-6.1rc1/src/robot/conf/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/
+Filename: robotframework-6.1rc1/src/robot/variables/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/
+Filename: robotframework-6.1rc1/src/robot/reporting/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/
+Filename: robotframework-6.1rc1/src/robot/running/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/
+Filename: robotframework-6.1rc1/src/robot/utils/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/
+Filename: robotframework-6.1rc1/src/robot/htmldata/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/
+Filename: robotframework-6.1rc1/src/robot/parsing/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/
+Filename: robotframework-6.1rc1/src/robot/libraries/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/api/
+Filename: robotframework-6.1rc1/src/robot/api/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/pythonpathsetter.py
+Filename: robotframework-6.1rc1/src/robot/pythonpathsetter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/rebot.py
+Filename: robotframework-6.1rc1/src/robot/rebot.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdoc.py
+Filename: robotframework-6.1rc1/src/robot/libdoc.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/errors.py
+Filename: robotframework-6.1rc1/src/robot/errors.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/testdoc.py
+Filename: robotframework-6.1rc1/src/robot/testdoc.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/__init__.py
+Filename: robotframework-6.1rc1/src/robot/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/version.py
+Filename: robotframework-6.1rc1/src/robot/version.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/__main__.py
+Filename: robotframework-6.1rc1/src/robot/__main__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/run.py
+Filename: robotframework-6.1rc1/src/robot/run.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/xmlelementhandlers.py
+Filename: robotframework-6.1rc1/src/robot/result/xmlelementhandlers.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/executionresult.py
+Filename: robotframework-6.1rc1/src/robot/result/executionresult.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/messagefilter.py
+Filename: robotframework-6.1rc1/src/robot/result/messagefilter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/suiteteardownfailed.py
+Filename: robotframework-6.1rc1/src/robot/result/suiteteardownfailed.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/flattenkeywordmatcher.py
+Filename: robotframework-6.1rc1/src/robot/result/flattenkeywordmatcher.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/merger.py
+Filename: robotframework-6.1rc1/src/robot/result/merger.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/resultbuilder.py
+Filename: robotframework-6.1rc1/src/robot/result/resultbuilder.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/executionerrors.py
+Filename: robotframework-6.1rc1/src/robot/result/executionerrors.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/modeldeprecation.py
+Filename: robotframework-6.1rc1/src/robot/result/modeldeprecation.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/__init__.py
+Filename: robotframework-6.1rc1/src/robot/result/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/keywordremover.py
+Filename: robotframework-6.1rc1/src/robot/result/keywordremover.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/visitor.py
+Filename: robotframework-6.1rc1/src/robot/result/visitor.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/model.py
+Filename: robotframework-6.1rc1/src/robot/result/model.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/result/configurer.py
+Filename: robotframework-6.1rc1/src/robot/result/configurer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/console/
+Filename: robotframework-6.1rc1/src/robot/output/console/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/listeners.py
+Filename: robotframework-6.1rc1/src/robot/output/listeners.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/output.py
+Filename: robotframework-6.1rc1/src/robot/output/output.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/listenermethods.py
+Filename: robotframework-6.1rc1/src/robot/output/listenermethods.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/pyloggingconf.py
+Filename: robotframework-6.1rc1/src/robot/output/pyloggingconf.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/filelogger.py
+Filename: robotframework-6.1rc1/src/robot/output/filelogger.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/loggerhelper.py
+Filename: robotframework-6.1rc1/src/robot/output/loggerhelper.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/stdoutlogsplitter.py
+Filename: robotframework-6.1rc1/src/robot/output/stdoutlogsplitter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/logger.py
+Filename: robotframework-6.1rc1/src/robot/output/logger.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/librarylogger.py
+Filename: robotframework-6.1rc1/src/robot/output/librarylogger.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/__init__.py
+Filename: robotframework-6.1rc1/src/robot/output/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/debugfile.py
+Filename: robotframework-6.1rc1/src/robot/output/debugfile.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/xmllogger.py
+Filename: robotframework-6.1rc1/src/robot/output/xmllogger.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/listenerarguments.py
+Filename: robotframework-6.1rc1/src/robot/output/listenerarguments.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/console/quiet.py
+Filename: robotframework-6.1rc1/src/robot/output/console/quiet.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/console/verbose.py
+Filename: robotframework-6.1rc1/src/robot/output/console/verbose.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/console/__init__.py
+Filename: robotframework-6.1rc1/src/robot/output/console/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/console/dotted.py
+Filename: robotframework-6.1rc1/src/robot/output/console/dotted.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/output/console/highlighting.py
+Filename: robotframework-6.1rc1/src/robot/output/console/highlighting.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/message.py
+Filename: robotframework-6.1rc1/src/robot/model/message.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/stats.py
+Filename: robotframework-6.1rc1/src/robot/model/stats.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/testcase.py
+Filename: robotframework-6.1rc1/src/robot/model/testcase.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/tags.py
+Filename: robotframework-6.1rc1/src/robot/model/tags.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/fixture.py
+Filename: robotframework-6.1rc1/src/robot/model/fixture.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/body.py
+Filename: robotframework-6.1rc1/src/robot/model/body.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/itemlist.py
+Filename: robotframework-6.1rc1/src/robot/model/itemlist.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/testsuite.py
+Filename: robotframework-6.1rc1/src/robot/model/testsuite.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/control.py
+Filename: robotframework-6.1rc1/src/robot/model/control.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/metadata.py
+Filename: robotframework-6.1rc1/src/robot/model/metadata.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/suitestatistics.py
+Filename: robotframework-6.1rc1/src/robot/model/suitestatistics.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/modifier.py
+Filename: robotframework-6.1rc1/src/robot/model/modifier.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/keyword.py
+Filename: robotframework-6.1rc1/src/robot/model/keyword.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/namepatterns.py
+Filename: robotframework-6.1rc1/src/robot/model/namepatterns.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/tagsetter.py
+Filename: robotframework-6.1rc1/src/robot/model/tagsetter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/__init__.py
+Filename: robotframework-6.1rc1/src/robot/model/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/visitor.py
+Filename: robotframework-6.1rc1/src/robot/model/visitor.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/totalstatistics.py
+Filename: robotframework-6.1rc1/src/robot/model/totalstatistics.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/filter.py
+Filename: robotframework-6.1rc1/src/robot/model/filter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/modelobject.py
+Filename: robotframework-6.1rc1/src/robot/model/modelobject.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/configurer.py
+Filename: robotframework-6.1rc1/src/robot/model/configurer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/statistics.py
+Filename: robotframework-6.1rc1/src/robot/model/statistics.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/model/tagstatistics.py
+Filename: robotframework-6.1rc1/src/robot/model/tagstatistics.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/conf/settings.py
+Filename: robotframework-6.1rc1/src/robot/conf/settings.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/conf/__init__.py
+Filename: robotframework-6.1rc1/src/robot/conf/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/conf/languages.py
+Filename: robotframework-6.1rc1/src/robot/conf/languages.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/conf/gatherfailed.py
+Filename: robotframework-6.1rc1/src/robot/conf/gatherfailed.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/variables.py
+Filename: robotframework-6.1rc1/src/robot/variables/variables.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/scopes.py
+Filename: robotframework-6.1rc1/src/robot/variables/scopes.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/store.py
+Filename: robotframework-6.1rc1/src/robot/variables/store.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/search.py
+Filename: robotframework-6.1rc1/src/robot/variables/search.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/replacer.py
+Filename: robotframework-6.1rc1/src/robot/variables/replacer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/assigner.py
+Filename: robotframework-6.1rc1/src/robot/variables/assigner.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/notfound.py
+Filename: robotframework-6.1rc1/src/robot/variables/notfound.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/finders.py
+Filename: robotframework-6.1rc1/src/robot/variables/finders.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/__init__.py
+Filename: robotframework-6.1rc1/src/robot/variables/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/filesetter.py
+Filename: robotframework-6.1rc1/src/robot/variables/filesetter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/evaluation.py
+Filename: robotframework-6.1rc1/src/robot/variables/evaluation.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/tablesetter.py
+Filename: robotframework-6.1rc1/src/robot/variables/tablesetter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/variables/resolvable.py
+Filename: robotframework-6.1rc1/src/robot/variables/resolvable.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/writer.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/writer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/builder.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/builder.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/jsonbuilder.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/jsonbuilder.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/htmlwriter.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/htmlwriter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/output.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/output.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/jsonwriter.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/jsonwriter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/xmlwriter.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/xmlwriter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/standardtypes.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/standardtypes.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/robotbuilder.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/robotbuilder.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/consoleviewer.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/consoleviewer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/datatypes.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/datatypes.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/__init__.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/htmlutils.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/htmlutils.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/model.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/model.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libdocpkg/xmlbuilder.py
+Filename: robotframework-6.1rc1/src/robot/libdocpkg/xmlbuilder.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/xunitwriter.py
+Filename: robotframework-6.1rc1/src/robot/reporting/xunitwriter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/jsmodelbuilders.py
+Filename: robotframework-6.1rc1/src/robot/reporting/jsmodelbuilders.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/jsbuildingcontext.py
+Filename: robotframework-6.1rc1/src/robot/reporting/jsbuildingcontext.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/jswriter.py
+Filename: robotframework-6.1rc1/src/robot/reporting/jswriter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/stringcache.py
+Filename: robotframework-6.1rc1/src/robot/reporting/stringcache.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/__init__.py
+Filename: robotframework-6.1rc1/src/robot/reporting/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/resultwriter.py
+Filename: robotframework-6.1rc1/src/robot/reporting/resultwriter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/logreportwriters.py
+Filename: robotframework-6.1rc1/src/robot/reporting/logreportwriters.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/jsexecutionresult.py
+Filename: robotframework-6.1rc1/src/robot/reporting/jsexecutionresult.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/outputwriter.py
+Filename: robotframework-6.1rc1/src/robot/reporting/outputwriter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/reporting/expandkeywordmatcher.py
+Filename: robotframework-6.1rc1/src/robot/reporting/expandkeywordmatcher.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/timeouts/
+Filename: robotframework-6.1rc1/src/robot/running/timeouts/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/builder/
+Filename: robotframework-6.1rc1/src/robot/running/builder/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/
+Filename: robotframework-6.1rc1/src/robot/running/arguments/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/context.py
+Filename: robotframework-6.1rc1/src/robot/running/context.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/librarykeywordrunner.py
+Filename: robotframework-6.1rc1/src/robot/running/librarykeywordrunner.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/handlers.py
+Filename: robotframework-6.1rc1/src/robot/running/handlers.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/modelcombiner.py
+Filename: robotframework-6.1rc1/src/robot/running/modelcombiner.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/libraryscopes.py
+Filename: robotframework-6.1rc1/src/robot/running/libraryscopes.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/signalhandler.py
+Filename: robotframework-6.1rc1/src/robot/running/signalhandler.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/userkeywordrunner.py
+Filename: robotframework-6.1rc1/src/robot/running/userkeywordrunner.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/bodyrunner.py
+Filename: robotframework-6.1rc1/src/robot/running/bodyrunner.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/usererrorhandler.py
+Filename: robotframework-6.1rc1/src/robot/running/usererrorhandler.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/suiterunner.py
+Filename: robotframework-6.1rc1/src/robot/running/suiterunner.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/status.py
+Filename: robotframework-6.1rc1/src/robot/running/status.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/runkwregister.py
+Filename: robotframework-6.1rc1/src/robot/running/runkwregister.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/testlibraries.py
+Filename: robotframework-6.1rc1/src/robot/running/testlibraries.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/outputcapture.py
+Filename: robotframework-6.1rc1/src/robot/running/outputcapture.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/userkeyword.py
+Filename: robotframework-6.1rc1/src/robot/running/userkeyword.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/__init__.py
+Filename: robotframework-6.1rc1/src/robot/running/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/randomizer.py
+Filename: robotframework-6.1rc1/src/robot/running/randomizer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/namespace.py
+Filename: robotframework-6.1rc1/src/robot/running/namespace.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/statusreporter.py
+Filename: robotframework-6.1rc1/src/robot/running/statusreporter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/handlerstore.py
+Filename: robotframework-6.1rc1/src/robot/running/handlerstore.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/dynamicmethods.py
+Filename: robotframework-6.1rc1/src/robot/running/dynamicmethods.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/model.py
+Filename: robotframework-6.1rc1/src/robot/running/model.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/importer.py
+Filename: robotframework-6.1rc1/src/robot/running/importer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/timeouts/posix.py
+Filename: robotframework-6.1rc1/src/robot/running/timeouts/posix.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/timeouts/__init__.py
+Filename: robotframework-6.1rc1/src/robot/running/timeouts/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/timeouts/windows.py
+Filename: robotframework-6.1rc1/src/robot/running/timeouts/windows.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/builder/parsers.py
+Filename: robotframework-6.1rc1/src/robot/running/builder/parsers.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/builder/transformers.py
+Filename: robotframework-6.1rc1/src/robot/running/builder/transformers.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/builder/settings.py
+Filename: robotframework-6.1rc1/src/robot/running/builder/settings.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/builder/builders.py
+Filename: robotframework-6.1rc1/src/robot/running/builder/builders.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/builder/__init__.py
+Filename: robotframework-6.1rc1/src/robot/running/builder/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/argumentmapper.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/argumentmapper.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/argumentconverter.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/argumentconverter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/argumentresolver.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/argumentresolver.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/embedded.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/embedded.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/customconverters.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/customconverters.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/typeconverters.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/typeconverters.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/typevalidator.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/typevalidator.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/argumentspec.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/argumentspec.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/argumentparser.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/argumentparser.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/argumentvalidator.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/argumentvalidator.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/running/arguments/__init__.py
+Filename: robotframework-6.1rc1/src/robot/running/arguments/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/robotio.py
+Filename: robotframework-6.1rc1/src/robot/utils/robotio.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/filereader.py
+Filename: robotframework-6.1rc1/src/robot/utils/filereader.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/sortable.py
+Filename: robotframework-6.1rc1/src/robot/utils/sortable.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/escaping.py
+Filename: robotframework-6.1rc1/src/robot/utils/escaping.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/restreader.py
+Filename: robotframework-6.1rc1/src/robot/utils/restreader.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/frange.py
+Filename: robotframework-6.1rc1/src/robot/utils/frange.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/connectioncache.py
+Filename: robotframework-6.1rc1/src/robot/utils/connectioncache.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/normalizing.py
+Filename: robotframework-6.1rc1/src/robot/utils/normalizing.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/markupwriters.py
+Filename: robotframework-6.1rc1/src/robot/utils/markupwriters.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/setter.py
+Filename: robotframework-6.1rc1/src/robot/utils/setter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/compress.py
+Filename: robotframework-6.1rc1/src/robot/utils/compress.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/misc.py
+Filename: robotframework-6.1rc1/src/robot/utils/misc.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/dotdict.py
+Filename: robotframework-6.1rc1/src/robot/utils/dotdict.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/recommendations.py
+Filename: robotframework-6.1rc1/src/robot/utils/recommendations.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/text.py
+Filename: robotframework-6.1rc1/src/robot/utils/text.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/unic.py
+Filename: robotframework-6.1rc1/src/robot/utils/unic.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/markuputils.py
+Filename: robotframework-6.1rc1/src/robot/utils/markuputils.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/robotpath.py
+Filename: robotframework-6.1rc1/src/robot/utils/robotpath.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/robottime.py
+Filename: robotframework-6.1rc1/src/robot/utils/robottime.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/encoding.py
+Filename: robotframework-6.1rc1/src/robot/utils/encoding.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/encodingsniffer.py
+Filename: robotframework-6.1rc1/src/robot/utils/encodingsniffer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/argumentparser.py
+Filename: robotframework-6.1rc1/src/robot/utils/argumentparser.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/asserts.py
+Filename: robotframework-6.1rc1/src/robot/utils/asserts.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/__init__.py
+Filename: robotframework-6.1rc1/src/robot/utils/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/application.py
+Filename: robotframework-6.1rc1/src/robot/utils/application.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/etreewrapper.py
+Filename: robotframework-6.1rc1/src/robot/utils/etreewrapper.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/match.py
+Filename: robotframework-6.1rc1/src/robot/utils/match.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/error.py
+Filename: robotframework-6.1rc1/src/robot/utils/error.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/robotenv.py
+Filename: robotframework-6.1rc1/src/robot/utils/robotenv.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/htmlformatters.py
+Filename: robotframework-6.1rc1/src/robot/utils/htmlformatters.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/charwidth.py
+Filename: robotframework-6.1rc1/src/robot/utils/typehints.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/platform.py
+Filename: robotframework-6.1rc1/src/robot/utils/charwidth.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/importer.py
+Filename: robotframework-6.1rc1/src/robot/utils/platform.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/robotinspect.py
+Filename: robotframework-6.1rc1/src/robot/utils/importer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/utils/robottypes.py
+Filename: robotframework-6.1rc1/src/robot/utils/robotinspect.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/
+Filename: robotframework-6.1rc1/src/robot/utils/robottypes.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/
+Filename: robotframework-6.1rc1/src/robot/htmldata/libdoc/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/lib/
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/testdoc/
+Filename: robotframework-6.1rc1/src/robot/htmldata/lib/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/common/
+Filename: robotframework-6.1rc1/src/robot/htmldata/testdoc/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/jsonwriter.py
+Filename: robotframework-6.1rc1/src/robot/htmldata/common/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/htmlfilewriter.py
+Filename: robotframework-6.1rc1/src/robot/htmldata/jsonwriter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/template.py
+Filename: robotframework-6.1rc1/src/robot/htmldata/htmlfilewriter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/__init__.py
+Filename: robotframework-6.1rc1/src/robot/htmldata/template.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/print.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/libdoc/print.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.html
+Filename: robotframework-6.1rc1/src/robot/htmldata/libdoc/libdoc.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/__init__.py
+Filename: robotframework-6.1rc1/src/robot/htmldata/libdoc/libdoc.html
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/pygments.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/libdoc/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/libdoc/doc_formatting.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/libdoc/pygments.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/common.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/libdoc/doc_formatting.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/report.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/common.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/log.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/report.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/print.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/log.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/view.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/print.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/report.html
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/view.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/testdata.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/report.html
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/util.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/testdata.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/model.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/util.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/log.html
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/model.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/fileloading.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/log.html
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/__init__.py
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/fileloading.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/doc_formatting.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/rebot/log.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/doc_formatting.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/lib/jsxcompressor.min.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/rebot/log.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/lib/__init__.py
+Filename: robotframework-6.1rc1/src/robot/htmldata/lib/jsxcompressor.min.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/lib/jquery.tablesorter.min.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/lib/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/lib/jquery.highlight.min.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/lib/jquery.tablesorter.min.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/lib/jquery.min.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/lib/jquery.highlight.min.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/lib/jquery.tmpl.min.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/lib/jquery.min.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/lib/jquery.tmpl.min.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/testdoc/__init__.py
+Filename: robotframework-6.1rc1/src/robot/htmldata/testdoc/testdoc.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.html
+Filename: robotframework-6.1rc1/src/robot/htmldata/testdoc/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/common/storage.js
+Filename: robotframework-6.1rc1/src/robot/htmldata/testdoc/testdoc.html
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/common/js_disabled.css
+Filename: robotframework-6.1rc1/src/robot/htmldata/common/storage.js
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/htmldata/common/__init__.py
+Filename: robotframework-6.1rc1/src/robot/htmldata/common/js_disabled.css
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/model/
+Filename: robotframework-6.1rc1/src/robot/htmldata/common/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/parser/
+Filename: robotframework-6.1rc1/src/robot/parsing/model/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/lexer/
+Filename: robotframework-6.1rc1/src/robot/parsing/parser/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/suitestructure.py
+Filename: robotframework-6.1rc1/src/robot/parsing/lexer/
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/__init__.py
+Filename: robotframework-6.1rc1/src/robot/parsing/suitestructure.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/model/blocks.py
+Filename: robotframework-6.1rc1/src/robot/parsing/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/model/__init__.py
+Filename: robotframework-6.1rc1/src/robot/parsing/model/blocks.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/model/visitor.py
+Filename: robotframework-6.1rc1/src/robot/parsing/model/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/model/statements.py
+Filename: robotframework-6.1rc1/src/robot/parsing/model/visitor.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/parser/blockparsers.py
+Filename: robotframework-6.1rc1/src/robot/parsing/model/statements.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/parser/parser.py
+Filename: robotframework-6.1rc1/src/robot/parsing/parser/blockparsers.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/parser/__init__.py
+Filename: robotframework-6.1rc1/src/robot/parsing/parser/parser.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/parser/fileparser.py
+Filename: robotframework-6.1rc1/src/robot/parsing/parser/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/lexer/lexer.py
+Filename: robotframework-6.1rc1/src/robot/parsing/parser/fileparser.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/lexer/blocklexers.py
+Filename: robotframework-6.1rc1/src/robot/parsing/lexer/lexer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/lexer/context.py
+Filename: robotframework-6.1rc1/src/robot/parsing/lexer/blocklexers.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/lexer/settings.py
+Filename: robotframework-6.1rc1/src/robot/parsing/lexer/context.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/lexer/tokens.py
+Filename: robotframework-6.1rc1/src/robot/parsing/lexer/settings.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/lexer/statementlexers.py
+Filename: robotframework-6.1rc1/src/robot/parsing/lexer/tokens.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/lexer/__init__.py
+Filename: robotframework-6.1rc1/src/robot/parsing/lexer/statementlexers.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/parsing/lexer/tokenizer.py
+Filename: robotframework-6.1rc1/src/robot/parsing/lexer/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/XML.py
+Filename: robotframework-6.1rc1/src/robot/parsing/lexer/tokenizer.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/Screenshot.py
+Filename: robotframework-6.1rc1/src/robot/libraries/XML.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/Easter.py
+Filename: robotframework-6.1rc1/src/robot/libraries/Screenshot.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/dialogs_py.py
+Filename: robotframework-6.1rc1/src/robot/libraries/Easter.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/String.py
+Filename: robotframework-6.1rc1/src/robot/libraries/dialogs_py.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/Telnet.py
+Filename: robotframework-6.1rc1/src/robot/libraries/String.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/DateTime.py
+Filename: robotframework-6.1rc1/src/robot/libraries/Telnet.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/Remote.py
+Filename: robotframework-6.1rc1/src/robot/libraries/DateTime.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/OperatingSystem.py
+Filename: robotframework-6.1rc1/src/robot/libraries/Remote.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/Collections.py
+Filename: robotframework-6.1rc1/src/robot/libraries/OperatingSystem.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/__init__.py
+Filename: robotframework-6.1rc1/src/robot/libraries/Collections.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/Reserved.py
+Filename: robotframework-6.1rc1/src/robot/libraries/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/Dialogs.py
+Filename: robotframework-6.1rc1/src/robot/libraries/Reserved.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/BuiltIn.py
+Filename: robotframework-6.1rc1/src/robot/libraries/Dialogs.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/libraries/Process.py
+Filename: robotframework-6.1rc1/src/robot/libraries/BuiltIn.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/api/interfaces.py
+Filename: robotframework-6.1rc1/src/robot/libraries/Process.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/api/parsing.py
+Filename: robotframework-6.1rc1/src/robot/api/interfaces.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/api/deco.py
+Filename: robotframework-6.1rc1/src/robot/api/parsing.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/api/logger.py
+Filename: robotframework-6.1rc1/src/robot/api/deco.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/api/__init__.py
+Filename: robotframework-6.1rc1/src/robot/api/logger.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robot/api/exceptions.py
+Filename: robotframework-6.1rc1/src/robot/api/__init__.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robotframework.egg-info/SOURCES.txt
+Filename: robotframework-6.1rc1/src/robot/api/exceptions.py
 Comment: 
 
-Filename: robotframework-6.1b1/src/robotframework.egg-info/entry_points.txt
+Filename: robotframework-6.1rc1/src/robotframework.egg-info/SOURCES.txt
 Comment: 
 
-Filename: robotframework-6.1b1/src/robotframework.egg-info/dependency_links.txt
+Filename: robotframework-6.1rc1/src/robotframework.egg-info/entry_points.txt
 Comment: 
 
-Filename: robotframework-6.1b1/src/robotframework.egg-info/PKG-INFO
+Filename: robotframework-6.1rc1/src/robotframework.egg-info/dependency_links.txt
 Comment: 
 
-Filename: robotframework-6.1b1/src/robotframework.egg-info/top_level.txt
+Filename: robotframework-6.1rc1/src/robotframework.egg-info/PKG-INFO
+Comment: 
+
+Filename: robotframework-6.1rc1/src/robotframework.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `robotframework-6.1b1/LICENSE.txt` & `robotframework-6.1rc1/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/tasks.py` & `robotframework-6.1rc1/tasks.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/BUILD.rst` & `robotframework-6.1rc1/BUILD.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/COPYRIGHT.txt` & `robotframework-6.1rc1/COPYRIGHT.txt`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/INSTALL.rst` & `robotframework-6.1rc1/INSTALL.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/setup.py` & `robotframework-6.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from os.path import abspath, join, dirname
 from setuptools import find_packages, setup
 
 
 # Version number typically updated by running `invoke set-version <version>`.
 # Run `invoke --help set-version` or see tasks.py for details.
-VERSION = '6.1b1'
+VERSION = '6.1rc1'
 with open(join(dirname(abspath(__file__)), 'README.rst')) as f:
     LONG_DESCRIPTION = f.read()
     base_url = 'https://github.com/robotframework/robotframework/blob/master'
     for text in ('INSTALL', 'CONTRIBUTING'):
         search = '`<{0}.rst>`__'.format(text)
         replace = '`{0}.rst <{1}/{0}.rst>`__'.format(text, base_url)
         if search not in LONG_DESCRIPTION:
@@ -24,14 +24,15 @@
 Programming Language :: Python :: 3 :: Only
 Programming Language :: Python :: 3.6
 Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
 Programming Language :: Python :: 3.9
 Programming Language :: Python :: 3.10
 Programming Language :: Python :: 3.11
+Programming Language :: Python :: 3.12
 Programming Language :: Python :: Implementation :: CPython
 Programming Language :: Python :: Implementation :: PyPy
 Topic :: Software Development :: Testing
 Topic :: Software Development :: Testing :: Acceptance
 Topic :: Software Development :: Testing :: BDD
 Framework :: Robot Framework
 """.strip().splitlines()
```

## Comparing `robotframework-6.1b1/README.rst` & `robotframework-6.1rc1/README.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/CONTRIBUTING.rst` & `robotframework-6.1rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/AUTHORS.rst` & `robotframework-6.1rc1/AUTHORS.rst`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/PKG-INFO` & `robotframework-6.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: robotframework
-Version: 6.1b1
+Version: 6.1rc1
 Summary: Generic automation framework for acceptance testing and robotic process automation (RPA)
 Home-page: https://robotframework.org
 Author: Pekka Klärck
 Author-email: peke@eliga.fi
 License: Apache License 2.0
 Download-URL: https://pypi.org/project/robotframework
 Project-URL: Source, https://github.com/robotframework/robotframework
 Project-URL: Issue Tracker, https://github.com/robotframework/robotframework/issues
 Project-URL: Documentation, https://robotframework.org/robotframework
-Project-URL: Release Notes, https://github.com/robotframework/robotframework/blob/master/doc/releasenotes/rf-6.1b1.rst
+Project-URL: Release Notes, https://github.com/robotframework/robotframework/blob/master/doc/releasenotes/rf-6.1rc1.rst
 Project-URL: Slack, http://slack.robotframework.org
 Project-URL: Twitter, https://twitter.com/robotframework
 Description: Robot Framework
         ===============
         
         .. contents::
            :local:
@@ -173,14 +173,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Classifier: Topic :: Software Development :: Testing :: BDD
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.6
```

## Comparing `robotframework-6.1b1/src/robot/pythonpathsetter.py` & `robotframework-6.1rc1/src/robot/pythonpathsetter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/rebot.py` & `robotframework-6.1rc1/src/robot/rebot.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdoc.py` & `robotframework-6.1rc1/src/robot/libdoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,25 +200,26 @@
 
     def _get_docformat(self, docformat):
         return self._validate('Doc format', docformat, 'ROBOT', 'TEXT', 'HTML', 'REST')
 
     def _get_format_and_specdocformat(self, format, specdocformat, output):
         extension = Path(output).suffix[1:]
         format = self._validate('Format', format or extension,
-                                'HTML', 'XML', 'JSON', 'LIBSPEC')
+                                'HTML', 'XML', 'JSON', 'LIBSPEC', allow_none=False)
         specdocformat = self._validate('Spec doc format', specdocformat, 'RAW', 'HTML')
         if format == 'HTML' and specdocformat:
             raise DataError("The --specdocformat option is not applicable with "
                             "HTML outputs.")
         return format, specdocformat
 
-    def _validate(self, kind, value, *valid):
-        if not value:
+    def _validate(self, kind, value, *valid, allow_none=True):
+        if value:
+            value = value.upper()
+        elif allow_none:
             return None
-        value = value.upper()
         if value not in valid:
             raise DataError(f"{kind} must be {seq2str(valid, lastsep=' or ')}, "
                             f"got '{value}'.")
         return value
 
     def _validate_theme(self, theme, format):
         theme = self._validate('Theme', theme, 'DARK', 'LIGHT', 'NONE')
```

## Comparing `robotframework-6.1b1/src/robot/errors.py` & `robotframework-6.1rc1/src/robot/errors.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/testdoc.py` & `robotframework-6.1rc1/src/robot/testdoc.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/__init__.py` & `robotframework-6.1rc1/src/robot/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/version.py` & `robotframework-6.1rc1/src/robot/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  limitations under the License.
 
 import re
 import sys
 
 # Version number typically updated by running `invoke set-version <version>`.
 # Run `invoke --help set-version` or see tasks.py for details.
-VERSION = '6.1b1'
+VERSION = '6.1rc1'
 
 
 def get_version(naked=False):
     if naked:
         return re.split('(a|b|rc|.dev)', VERSION)[0]
     return VERSION
```

## Comparing `robotframework-6.1b1/src/robot/__main__.py` & `robotframework-6.1rc1/src/robot/__main__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/run.py` & `robotframework-6.1rc1/src/robot/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,20 @@
                           a custom language file.
  -F --extension value     Parse only files with this extension when executing
                           a directory. Has no effect when running individual
                           files or when using resource files. If more than one
                           extension is needed, separate them with a colon.
                           Examples: `--extension txt`, `--extension robot:txt`
                           Only `*.robot` files are parsed by default.
+ -I --parseinclude pattern *  Parse only files matching `pattern`. It can be:
+                          - a file name or pattern like `example.robot` or
+                            `*.robot` to parse all files matching that name,
+                          - a file path like `path/to/example.robot`, or
+                          - a directory path like `path/to/example` to parse
+                            all files in that directory, recursively.
  -N --name name           Set the name of the top level suite. By default the
                           name is created based on the executed file or
                           directory.
  -D --doc documentation   Set the documentation of the top level suite.
                           Simple formatting is supported (e.g. *bold*). If the
                           documentation contains spaces, it must be quoted.
                           If the value is path to an existing file, actual
@@ -147,17 +153,17 @@
     --skiponfailure tag *  Tests having given tag will be skipped if they fail.
                           Tag can be a pattern
  -v --variable name:value *  Set variables in the test data. Only scalar
                           variables with string value are supported and name is
                           given without `${}`. See --variablefile for a more
                           powerful variable setting mechanism.
                           Examples:
-                          --variable str:Hello       =>  ${str} = `Hello`
-                          -v hi:Hi_World -E space:_  =>  ${hi} = `Hi World`
-                          -v x: -v y:42              =>  ${x} = ``, ${y} = `42`
+                          --variable name:Robot  =>  ${name} = `Robot`
+                          -v "hello:Hello world" =>  ${hello} = `Hello world`
+                          -v x: -v y:42          =>  ${x} = ``, ${y} = `42`
  -V --variablefile path *  Python or YAML file file to read variables from.
                           Possible arguments to the variable file can be given
                           after the path using colon or semicolon as separator.
                           Examples: --variablefile path/vars.yaml
                                     --variablefile environment.py:testing
  -d --outputdir dir       Where to create output files. The default is the
                           directory where tests are run from and the given path
@@ -427,16 +433,16 @@
             LOGGER.register_console_logger(stdout=options.get('stdout'),
                                            stderr=options.get('stderr'))
             raise
         LOGGER.register_console_logger(**settings.console_output_config)
         LOGGER.info(f'Settings:\n{settings}')
         if settings.pythonpath:
             sys.path = settings.pythonpath + sys.path
-        builder = TestSuiteBuilder(settings.suite_names,
-                                   included_extensions=settings.extension,
+        builder = TestSuiteBuilder(included_extensions=settings.extension,
+                                   included_files=settings.parse_include,
                                    custom_parsers=settings.parsers,
                                    rpa=settings.rpa,
                                    lang=settings.languages,
                                    allow_empty_suite=settings.run_empty_suite)
         suite = builder.build(*datasources)
         settings.rpa = suite.rpa
         if settings.pre_run_modifiers:
```

## Comparing `robotframework-6.1b1/src/robot/result/xmlelementhandlers.py` & `robotframework-6.1rc1/src/robot/result/xmlelementhandlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,16 @@
     def register(cls, handler):
         cls.element_handlers[handler.tag] = handler()
         return handler
 
     def get_child_handler(self, tag):
         if tag not in self.children:
             if not self.tag:
-                raise DataError("Incompatible root element '%s'." % tag)
-            raise DataError("Incompatible child element '%s' for '%s'."
-                            % (tag, self.tag))
+                raise DataError(f"Incompatible root element '{tag}'.")
+            raise DataError(f"Incompatible child element '{tag}' for '{self.tag}'.")
         return self.element_handlers[tag]
 
     def start(self, elem, result):
         return result
 
     def end(self, elem, result):
         pass
@@ -125,15 +124,15 @@
                           'while', 'return', 'break', 'continue', 'error'))
 
     def start(self, elem, result):
         elem_type = elem.get('type')
         if not elem_type:
             creator = self._create_keyword
         else:
-            creator = getattr(self, '_create_%s' % elem_type.lower().replace(' ', '_'))
+            creator = getattr(self, '_create_' + elem_type.lower())
         return creator(elem, result)
 
     def _create_keyword(self, elem, result):
         try:
             body = result.body
         except AttributeError:
             body = self._get_body_for_suite_level_keyword(result)
@@ -146,15 +145,15 @@
         # Add the keyword into a suite setup or teardown, depending on have we already
         # seen tests or not. Create an implicit setup/teardown if needed. Possible real
         # setup/teardown parsed later will reset the implicit one otherwise, but leaves
         # the added keyword into its body.
         kw_type = 'teardown' if result.tests or result.suites else 'setup'
         keyword = getattr(result, kw_type)
         if not keyword:
-            keyword.config(kwname='Implicit %s' % kw_type, status=keyword.PASS)
+            keyword.config(kwname=f'Implicit {kw_type}', status=keyword.PASS)
         return keyword.body
 
     def _create_setup(self, elem, result):
         return result.setup.config(kwname=elem.get('name', ''),
                                    libname=elem.get('library'))
 
     def _create_teardown(self, elem, result):
@@ -376,15 +375,15 @@
         if result.type == result.KEYWORD:
             result.assign += (value,)
         elif result.type == result.FOR:
             result.variables += (value,)
         elif result.type == result.ITERATION:
             result.variables[elem.get('name')] = value
         else:
-            raise DataError("Invalid element '%s' for result '%r'." % (elem, result))
+            raise DataError(f"Invalid element '{elem}' for result '{result!r}'.")
 
 
 @ElementHandler.register
 class ArgumentsHandler(ElementHandler):    # RF < 4 compatibility.
     tag = 'arguments'
     children = frozenset(('arg',))
```

## Comparing `robotframework-6.1b1/src/robot/result/executionresult.py` & `robotframework-6.1rc1/src/robot/result/executionresult.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/messagefilter.py` & `robotframework-6.1rc1/src/robot/result/messagefilter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/suiteteardownfailed.py` & `robotframework-6.1rc1/src/robot/result/suiteteardownfailed.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/flattenkeywordmatcher.py` & `robotframework-6.1rc1/src/robot/result/flattenkeywordmatcher.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/merger.py` & `robotframework-6.1rc1/src/robot/result/merger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/resultbuilder.py` & `robotframework-6.1rc1/src/robot/result/resultbuilder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/executionerrors.py` & `robotframework-6.1rc1/src/robot/result/executionerrors.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/modeldeprecation.py` & `robotframework-6.1rc1/src/robot/result/modeldeprecation.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/__init__.py` & `robotframework-6.1rc1/src/robot/result/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/keywordremover.py` & `robotframework-6.1rc1/src/robot/result/keywordremover.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/visitor.py` & `robotframework-6.1rc1/src/robot/result/visitor.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/result/model.py` & `robotframework-6.1rc1/src/robot/result/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,167 +31,259 @@
 be imported via the :mod:`robot.running` module.
 
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#listener-interface
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#programmatic-modification-of-results
 
 """
 
+import sys
+import warnings
 from collections import OrderedDict
+from datetime import datetime, timedelta
 from itertools import chain
-import warnings
+from pathlib import Path
+from typing import Generic, Mapping, Sequence, Type, Union, TypeVar
+
+if sys.version_info >= (3, 8):
+    from typing import Literal
 
 from robot import model
-from robot.model import BodyItem, create_fixture, Keywords, Tags, TotalStatisticsBuilder
-from robot.utils import get_elapsed_time, setter
+from robot.model import (BodyItem, create_fixture, DataDict, Keywords, Tags,
+                         SuiteVisitor, TotalStatistics, TotalStatisticsBuilder,
+                         TestCases, TestSuites)
+from robot.utils import copy_signature, get_elapsed_time, KnownAtRuntime, setter
 
 from .configurer import SuiteConfigurer
 from .messagefilter import MessageFilter
 from .modeldeprecation import deprecated, DeprecatedAttributesMixin
 from .keywordremover import KeywordRemover
 from .suiteteardownfailed import SuiteTeardownFailed, SuiteTeardownFailureHandler
 
+IT = TypeVar('IT', bound='IfBranch|TryBranch')
+FW = TypeVar('FW', bound='ForIteration|WhileIteration')
+
+BodyItemParent = Union['TestSuite', 'TestCase', 'For', 'ForIteration', 'If', 'IfBranch',
+                       'Try', 'TryBranch', 'While', 'WhileIteration', None]
+
 
-class Body(model.Body):
+class Body(model.BaseBody['Keyword', 'For', 'While', 'If', 'Try', 'Return', 'Continue',
+                          'Break', 'Message', 'Error']):
     __slots__ = []
 
 
-class Branches(model.Branches):
+class Branches(model.BaseBranches['Keyword', 'For', 'While', 'If', 'Try', 'Return',
+                                  'Continue', 'Break', 'Message', 'Error', IT]):
     __slots__ = []
 
 
-class Iterations(model.BaseBody):
+class IterationType(Generic[FW]):
+    """Class that wrapps `Generic` as python doesn't allow multple generic inheritance"""
+    pass
+
+
+class Iterations(model.BaseBody['Keyword', 'For', 'While', 'If', 'Try', 'Return',
+                                'Continue', 'Break', 'Message', 'Error'], IterationType[FW]):
     __slots__ = ['iteration_class']
+    iteration_type: Type[FW] = KnownAtRuntime
 
-    def __init__(self, iteration_class, parent=None, items=None):
+    def __init__(self, iteration_class: Type[FW],
+                 parent: BodyItemParent = None,
+                 items: 'Sequence[FW|DataDict]' = ()):
         self.iteration_class = iteration_class
         super().__init__(parent, items)
 
-    def create_iteration(self, *args, **kwargs):
-        return self.append(self.iteration_class(*args, **kwargs))
+    @copy_signature(iteration_type)
+    def create_iteration(self, *args, **kwargs) -> FW:
+        return self._create(self.iteration_class, 'iteration_class', args, kwargs)
 
 
 @Body.register
 @Branches.register
 @Iterations.register
 class Message(model.Message):
-    __slots__ = []
+    __slots__ = ()
 
 
 class StatusMixin:
-    __slots__ = []
     PASS = 'PASS'
     FAIL = 'FAIL'
     SKIP = 'SKIP'
     NOT_RUN = 'NOT RUN'
     NOT_SET = 'NOT SET'
+    starttime: 'str|None'
+    endtime: 'str|None'
+    __slots__ = ()
 
     @property
-    def elapsedtime(self):
-        """Total execution time in milliseconds."""
+    def elapsedtime(self) -> int:
+        """Total execution time in milliseconds.
+
+        This attribute will be replaced by :attr:`elapsed_time` in the future.
+        """
         return get_elapsed_time(self.starttime, self.endtime)
 
     @property
-    def passed(self):
+    def elapsed_time(self) -> timedelta:
+        """Total execution time as a ``timedelta``.
+
+        This attribute will replace :attr:`elapsedtime` in the future.
+
+        New in Robot Framework 6.1.
+        """
+        return timedelta(milliseconds=self.elapsedtime)
+
+    @property
+    def start_time(self) -> 'datetime|None':
+        """Execution start time as a ``datetime`` or as ``None`` if not set.
+
+        This attribute will replace :attr:`starttime` in the future.
+
+        New in Robot Framework 6.1.
+        """
+        return self._timestr_to_datetime(self.starttime) if self.starttime else None
+
+    @start_time.setter
+    def start_time(self, start_time: 'datetime|None'):
+        self.starttime = self._datetime_to_timestr(start_time) if start_time else None
+
+    @property
+    def end_time(self) -> 'datetime|None':
+        """Execution end time as a ``datetime`` or as ``None`` if not set.
+
+        This attribute will replace :attr:`endtime` in the future.
+
+        New in Robot Framework 6.1.
+        """
+        return self._timestr_to_datetime(self.endtime) if self.endtime else None
+
+    @end_time.setter
+    def end_time(self, end_time: 'datetime|None'):
+        self.endtime = self._datetime_to_timestr(end_time) if end_time else None
+
+    def _timestr_to_datetime(self, ts: str) -> datetime:
+        micro = int(ts[18:]) * 1000
+        return datetime(int(ts[:4]), int(ts[4:6]), int(ts[6:8]),
+                        int(ts[9:11]), int(ts[12:14]), int(ts[15:17]), micro)
+
+    def _datetime_to_timestr(self, dt: datetime) -> str:
+        millis = int(round(dt.microsecond, -3) / 1000)
+        return (f'{dt.year}{dt.month:02}{dt.day:02} '
+                f'{dt.hour:02}:{dt.minute:02}.{dt.second:02}.{millis}')
+
+    @property
+    def passed(self) -> bool:
         """``True`` when :attr:`status` is 'PASS', ``False`` otherwise."""
         return self.status == self.PASS
 
     @passed.setter
-    def passed(self, passed):
+    def passed(self, passed: bool):
         self.status = self.PASS if passed else self.FAIL
 
     @property
-    def failed(self):
+    def failed(self) -> bool:
         """``True`` when :attr:`status` is 'FAIL', ``False`` otherwise."""
         return self.status == self.FAIL
 
     @failed.setter
-    def failed(self, failed):
+    def failed(self, failed: bool):
         self.status = self.FAIL if failed else self.PASS
 
     @property
-    def skipped(self):
+    def skipped(self) -> bool:
         """``True`` when :attr:`status` is 'SKIP', ``False`` otherwise.
 
         Setting to ``False`` value is ambiguous and raises an exception.
         """
         return self.status == self.SKIP
 
     @skipped.setter
-    def skipped(self, skipped):
+    def skipped(self, skipped: 'Literal[True]'):
         if not skipped:
-            raise ValueError("`skipped` value must be truthy, got '%s'." % skipped)
+            raise ValueError(f"`skipped` value must be truthy, got '{skipped}'.")
         self.status = self.SKIP
 
     @property
-    def not_run(self):
+    def not_run(self) -> bool:
         """``True`` when :attr:`status` is 'NOT RUN', ``False`` otherwise.
 
         Setting to ``False`` value is ambiguous and raises an exception.
         """
         return self.status == self.NOT_RUN
 
     @not_run.setter
-    def not_run(self, not_run):
+    def not_run(self, not_run: 'Literal[True]'):
         if not not_run:
-            raise ValueError("`not_run` value must be truthy, got '%s'." % not_run)
+            raise ValueError(f"`not_run` value must be truthy, got '{not_run}'.")
         self.status = self.NOT_RUN
 
 
 class ForIteration(BodyItem, StatusMixin, DeprecatedAttributesMixin):
     """Represents one FOR loop iteration."""
     type = BodyItem.ITERATION
     body_class = Body
     repr_args = ('variables',)
     __slots__ = ['variables', 'status', 'starttime', 'endtime', 'doc']
 
-    def __init__(self, variables=None, status='FAIL', starttime=None, endtime=None,
-                 doc='', parent=None):
-        self.variables = variables or OrderedDict()
+    def __init__(self, variables: 'Mapping[str, str]|None' = None,
+                 status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 doc: str = '',
+                 parent: BodyItemParent = None):
+        self.variables = OrderedDict(variables or ())
         self.parent = parent
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
         self.doc = doc
-        self.body = None
+        self.body = []
 
     @setter
-    def body(self, body):
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
         return self.body_class(self, body)
 
-    def visit(self, visitor):
+    def visit(self, visitor: SuiteVisitor):
         visitor.visit_for_iteration(self)
 
     @property
     @deprecated
-    def name(self):
+    def name(self) -> str:
         return ', '.join('%s = %s' % item for item in self.variables.items())
 
 
 @Body.register
 class For(model.For, StatusMixin, DeprecatedAttributesMixin):
-    iterations_class = Iterations
     iteration_class = ForIteration
+    iterations_class = Iterations[iteration_class]
     __slots__ = ['status', 'starttime', 'endtime', 'doc']
 
-    def __init__(self, variables=(),  flavor='IN', values=(), start=None, mode=None,
-                 fill=None, status='FAIL', starttime=None, endtime=None, doc='',
-                 parent=None):
+    def __init__(self, variables: Sequence[str] = (),
+                 flavor: "Literal['IN', 'IN RANGE', 'IN ENUMERATE', 'IN ZIP']" = 'IN',
+                 values: Sequence[str] = (),
+                 start: 'str|None' = None,
+                 mode: 'str|None' = None,
+                 fill: 'str|None' = None,
+                 status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 doc: str = '',
+                 parent: BodyItemParent = None):
         super().__init__(variables, flavor, values, start, mode, fill, parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
         self.doc = doc
 
     @setter
-    def body(self, iterations):
+    def body(self, iterations: 'Sequence[ForIteration|DataDict]') -> iterations_class:
         return self.iterations_class(self.iteration_class, self, iterations)
 
     @property
     @deprecated
-    def name(self):
+    def name(self) -> str:
         variables = ' | '.join(self.variables)
         values = ' | '.join(self.values)
         for name, value in [('start', self.start),
                             ('mode', self.mode),
                             ('fill', self.fill)]:
             if value is not None:
                 values += f' | {name}={value}'
@@ -200,58 +292,67 @@
 
 class WhileIteration(BodyItem, StatusMixin, DeprecatedAttributesMixin):
     """Represents one WHILE loop iteration."""
     type = BodyItem.ITERATION
     body_class = Body
     __slots__ = ['status', 'starttime', 'endtime', 'doc']
 
-    def __init__(self, status='FAIL', starttime=None, endtime=None,
-                 doc='', parent=None):
+    def __init__(self, status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 doc: str = '',
+                 parent: BodyItemParent = None):
         self.parent = parent
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
         self.doc = doc
-        self.body = None
+        self.body = ()
 
     @setter
-    def body(self, body):
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
         return self.body_class(self, body)
 
-    def visit(self, visitor):
+    def visit(self, visitor: SuiteVisitor):
         visitor.visit_while_iteration(self)
 
     @property
     @deprecated
-    def name(self):
+    def name(self) -> str:
         return ''
 
 
 @Body.register
 class While(model.While, StatusMixin, DeprecatedAttributesMixin):
-    iterations_class = Iterations
     iteration_class = WhileIteration
+    iterations_class = Iterations[iteration_class]
     __slots__ = ['status', 'starttime', 'endtime', 'doc']
 
-    def __init__(self, condition=None, limit=None, on_limit=None,
-                 on_limit_message=None, parent=None, status='FAIL',
-                 starttime=None, endtime=None, doc=''):
+    def __init__(self, condition: 'str|None' = None,
+                 limit: 'str|None' = None,
+                 on_limit: 'str|None' = None,
+                 on_limit_message: 'str|None' = None,
+                 status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 doc: str = '',
+                 parent: BodyItemParent = None):
         super().__init__(condition, limit, on_limit, on_limit_message, parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
         self.doc = doc
 
     @setter
-    def body(self, iterations):
+    def body(self, iterations: 'Sequence[WhileIteration|DataDict]') -> iterations_class:
         return self.iterations_class(self.iteration_class, self, iterations)
 
     @property
     @deprecated
-    def name(self):
+    def name(self) -> str:
         parts = []
         if self.condition:
             parts.append(self.condition)
         if self.limit:
             parts.append(f'limit={self.limit}')
         if self.on_limit:
             parts.append(f'on_limit={self.on_limit}')
@@ -260,229 +361,273 @@
         return ' | '.join(parts)
 
 
 class IfBranch(model.IfBranch, StatusMixin, DeprecatedAttributesMixin):
     body_class = Body
     __slots__ = ['status', 'starttime', 'endtime', 'doc']
 
-    def __init__(self, type=BodyItem.IF, condition=None, status='FAIL',
-                 starttime=None, endtime=None, doc='', parent=None):
+    def __init__(self, type: str = BodyItem.IF,
+                 condition: 'str|None' = None,
+                 status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 doc: str = '',
+                 parent: BodyItemParent = None):
         super().__init__(type, condition, parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
         self.doc = doc
 
     @property
     @deprecated
-    def name(self):
-        return self.condition
+    def name(self) -> str:
+        return self.condition or ''
 
 
 @Body.register
 class If(model.If, StatusMixin, DeprecatedAttributesMixin):
     branch_class = IfBranch
-    branches_class = Branches
+    branches_class = Branches[branch_class]
     __slots__ = ['status', 'starttime', 'endtime', 'doc']
 
-    def __init__(self, status='FAIL', starttime=None, endtime=None, doc='', parent=None):
+    def __init__(self, status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 doc: str = '',
+                 parent: BodyItemParent = None):
         super().__init__(parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
         self.doc = doc
 
 
 class TryBranch(model.TryBranch, StatusMixin, DeprecatedAttributesMixin):
     body_class = Body
     __slots__ = ['status', 'starttime', 'endtime', 'doc']
 
-    def __init__(self, type=BodyItem.TRY, patterns=(), pattern_type=None, variable=None,
-                 status='FAIL', starttime=None, endtime=None, doc='', parent=None):
+    def __init__(self, type: str = BodyItem.TRY,
+                 patterns: Sequence[str] = (),
+                 pattern_type: 'str|None' = None,
+                 variable: 'str|None' = None,
+                 status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 doc: str = '',
+                 parent: BodyItemParent = None):
         super().__init__(type, patterns, pattern_type, variable, parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
         self.doc = doc
 
     @property
     @deprecated
-    def name(self):
+    def name(self) -> str:
         patterns = list(self.patterns)
         if self.pattern_type:
             patterns.append(f'type={self.pattern_type}')
         parts = []
         if patterns:
             parts.append(' | '.join(patterns))
         if self.variable:
             parts.append(f'AS {self.variable}')
         return ' '.join(parts)
 
 
 @Body.register
 class Try(model.Try, StatusMixin, DeprecatedAttributesMixin):
     branch_class = TryBranch
-    branches_class = Branches
+    branches_class = Branches[branch_class]
     __slots__ = ['status', 'starttime', 'endtime', 'doc']
 
-    def __init__(self, status='FAIL', starttime=None, endtime=None, doc='', parent=None):
+    def __init__(self, status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 doc: str = '',
+                 parent: BodyItemParent = None):
         super().__init__(parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
         self.doc = doc
 
 
 @Body.register
 class Return(model.Return, StatusMixin, DeprecatedAttributesMixin):
     __slots__ = ['status', 'starttime', 'endtime']
     body_class = Body
 
-    def __init__(self, values=(), status='FAIL', starttime=None, endtime=None, parent=None):
+    def __init__(self, values: Sequence[str] = (),
+                 status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 parent: BodyItemParent = None):
         super().__init__(values, parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
-        self.body = None
+        self.body = ()
 
     @setter
-    def body(self, body):
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
         """Child keywords and messages as a :class:`~.Body` object.
 
         Typically empty. Only contains something if running RETURN has failed
         due to a syntax error or listeners have logged messages or executed
         keywords.
         """
         return self.body_class(self, body)
 
     @property
     @deprecated
-    def args(self):
+    def args(self) -> 'tuple[str, ...]':
         return self.values
 
     @property
     @deprecated
-    def doc(self):
+    def doc(self) -> str:
         return ''
 
 
 @Body.register
 class Continue(model.Continue, StatusMixin, DeprecatedAttributesMixin):
     __slots__ = ['status', 'starttime', 'endtime']
     body_class = Body
 
-    def __init__(self, status='FAIL', starttime=None, endtime=None, parent=None):
+    def __init__(self, status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 parent: BodyItemParent = None):
         super().__init__(parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
-        self.body = None
+        self.body = ()
 
     @setter
-    def body(self, body):
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
         """Child keywords and messages as a :class:`~.Body` object.
 
         Typically empty. Only contains something if running CONTINUE has failed
         due to a syntax error or listeners have logged messages or executed
         keywords.
         """
         return self.body_class(self, body)
 
     @property
     @deprecated
-    def args(self):
+    def args(self) -> 'tuple[str, ...]':
         return ()
 
     @property
     @deprecated
-    def doc(self):
+    def doc(self) -> str:
         return ''
 
 
 @Body.register
 class Break(model.Break, StatusMixin, DeprecatedAttributesMixin):
     __slots__ = ['status', 'starttime', 'endtime']
     body_class = Body
 
-    def __init__(self, status='FAIL', starttime=None, endtime=None, parent=None):
+    def __init__(self, status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 parent: BodyItemParent = None):
         super().__init__(parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
-        self.body = None
+        self.body = ()
 
     @setter
-    def body(self, body):
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
         """Child keywords and messages as a :class:`~.Body` object.
 
         Typically empty. Only contains something if running BREAK has failed
         due to a syntax error or listeners have logged messages or executed
         keywords.
         """
         return self.body_class(self, body)
 
     @property
     @deprecated
-    def args(self):
+    def args(self) -> 'tuple[str, ...]':
         return ()
 
     @property
     @deprecated
-    def doc(self):
+    def doc(self) -> str:
         return ''
 
 
 @Body.register
 class Error(model.Error, StatusMixin, DeprecatedAttributesMixin):
     __slots__ = ['status', 'starttime', 'endtime']
     body_class = Body
 
-    def __init__(self, values=(), status='FAIL', starttime=None, endtime=None, parent=None):
+    def __init__(self, values: Sequence[str] = (),
+                 status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 parent: BodyItemParent = None):
         super().__init__(values, parent)
         self.status = status
         self.starttime = starttime
         self.endtime = endtime
-        self.body = None
+        self.body = ()
 
     @setter
-    def body(self, body):
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
         """Messages as a :class:`~.Body` object.
 
         Typically contains the message that caused the error.
         """
         return self.body_class(self, body)
 
     @property
     @deprecated
-    def kwname(self):
+    def kwname(self) -> str:
         return self.values[0]
 
     @property
     @deprecated
-    def args(self):
+    def args(self) -> 'tuple[str, ...]':
         return self.values[1:]
 
     @property
     @deprecated
-    def doc(self):
+    def doc(self) -> 'str':
         return ''
 
 
 @Body.register
 @Branches.register
 @Iterations.register
 class Keyword(model.Keyword, StatusMixin):
     """Represents an executed library or user keyword."""
     body_class = Body
     __slots__ = ['kwname', 'libname', 'doc', 'timeout', 'status', '_teardown',
                  'starttime', 'endtime', 'message', 'sourcename']
 
-    def __init__(self, kwname='', libname='', doc='', args=(), assign=(), tags=(),
-                 timeout=None, type=BodyItem.KEYWORD, status='FAIL', starttime=None,
-                 endtime=None, parent=None, sourcename=None):
+    def __init__(self, kwname: str = '',
+                 libname: str = '',
+                 doc: str = '',
+                 args: Sequence[str] = (),
+                 assign: Sequence[str] = (),
+                 tags: Sequence[str] = (),
+                 timeout: 'str|None' = None,
+                 type: str = BodyItem.KEYWORD,
+                 status: str = 'FAIL',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 sourcename: 'str|None' = None,
+                 parent: BodyItemParent = None):
         super().__init__(None, args, assign, type, parent)
         #: Name of the keyword without library or resource name.
         self.kwname = kwname
         #: Name of the library or resource containing this keyword.
         self.libname = libname
         self.doc = doc
         self.tags = tags
@@ -491,83 +636,83 @@
         self.starttime = starttime
         self.endtime = endtime
         #: Keyword status message. Used only if suite teardowns fails.
         self.message = ''
         #: Original name of keyword with embedded arguments.
         self.sourcename = sourcename
         self._teardown = None
-        self.body = None
+        self.body = ()
 
     @setter
-    def body(self, body):
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
         """Possible keyword body as a :class:`~.Body` object.
 
         Body can consist of child keywords, messages, and control structures
         such as IF/ELSE. Library keywords typically have an empty body.
         """
         return self.body_class(self, body)
 
     @property
-    def keywords(self):
+    def keywords(self) -> Keywords:
         """Deprecated since Robot Framework 4.0.
 
         Use :attr:`body` or :attr:`teardown` instead.
         """
         keywords = self.body.filter(messages=False)
         if self.teardown:
             keywords.append(self.teardown)
         return Keywords(self, keywords)
 
     @keywords.setter
     def keywords(self, keywords):
         Keywords.raise_deprecation_error()
 
     @property
-    def messages(self):
+    def messages(self) -> 'list[Message]':
         """Keyword's messages.
 
         Starting from Robot Framework 4.0 this is a list generated from messages
         in :attr:`body`.
         """
-        return self.body.filter(messages=True)
+        return self.body.filter(messages=True)    # type: ignore
 
     @property
-    def children(self):
+    def children(self) -> 'list[BodyItem]':
         """List of child keywords and messages in creation order.
 
         Deprecated since Robot Framework 4.0. Use :attr:`body` instead.
         """
         warnings.warn("'Keyword.children' is deprecated. Use 'Keyword.body' instead.")
         return list(self.body)
 
     @property
-    def name(self):
+    def name(self) -> 'str|None':
         """Keyword name in format ``libname.kwname``.
 
         Just ``kwname`` if :attr:`libname` is empty. In practice that is the
         case only with user keywords in the same file as the executed test case
         or test suite.
 
         Cannot be set directly. Set :attr:`libname` and :attr:`kwname`
         separately instead.
         """
         if not self.libname:
             return self.kwname
-        return '%s.%s' % (self.libname, self.kwname)
+        return f'{self.libname}.{self.kwname}'
 
     @name.setter
     def name(self, name):
         if name is not None:
             raise AttributeError("Cannot set 'name' attribute directly. "
                                  "Set 'kwname' and 'libname' separately instead.")
         self.kwname = None
         self.libname = None
 
     @property    # Cannot use @setter because it would create teardowns recursively.
-    def teardown(self):
+    def teardown(self) -> 'Keyword':
         """Keyword teardown as a :class:`Keyword` object.
 
         Teardown can be modified by setting attributes directly::
 
             keyword.teardown.name = 'Example'
             keyword.teardown.args = ('First', 'Second')
 
@@ -587,115 +732,134 @@
         attribute avoids creating the ``Keyword`` object and is thus more memory
         efficient.
 
         New in Robot Framework 4.0. Earlier teardown was accessed like
         ``keyword.keywords.teardown``. :attr:`has_teardown` is new in Robot
         Framework 4.1.2.
         """
-        if self._teardown is None and self:
-            self._teardown = create_fixture(None, self, self.TEARDOWN)
+        if self._teardown is None:
+            self._teardown = create_fixture(self.__class__, None, self, self.TEARDOWN)
         return self._teardown
 
     @teardown.setter
-    def teardown(self, teardown):
-        self._teardown = create_fixture(teardown, self, self.TEARDOWN)
+    def teardown(self, teardown: 'Keyword|DataDict|None'):
+        self._teardown = create_fixture(self.__class__, teardown, self, self.TEARDOWN)
 
     @property
-    def has_teardown(self):
+    def has_teardown(self) -> bool:
         """Check does a keyword have a teardown without creating a teardown object.
 
         A difference between using ``if kw.has_teardown:`` and ``if kw.teardown:``
         is that accessing the :attr:`teardown` attribute creates a :class:`Keyword`
         object representing a teardown even when the keyword actually does not
         have one. This typically does not matter, but with bigger suite structures
         having lots of keywords it can have a considerable effect on memory usage.
 
         New in Robot Framework 4.1.2.
         """
         return bool(self._teardown)
 
     @setter
-    def tags(self, tags):
+    def tags(self, tags: Sequence[str]) -> model.Tags:
         """Keyword tags as a :class:`~.model.tags.Tags` object."""
         return Tags(tags)
 
 
-class TestCase(model.TestCase, StatusMixin):
+class TestCase(model.TestCase[Keyword], StatusMixin):
     """Represents results of a single test case.
 
     See the base class for documentation of attributes not documented here.
     """
     __slots__ = ['status', 'message', 'starttime', 'endtime']
     body_class = Body
     fixture_class = Keyword
 
-    def __init__(self, name='', doc='', tags=None, timeout=None, lineno=None,
-                 status='FAIL', message='', starttime=None, endtime=None,
-                 parent=None):
+    def __init__(self, name: str = '',
+                 doc: str = '',
+                 tags: Sequence[str] = (),
+                 timeout: 'str|None' = None,
+                 lineno: 'int|None' = None,
+                 status: str = 'FAIL',
+                 message: str = '',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 parent: 'TestSuite|None' = None):
         super().__init__(name, doc, tags, timeout, lineno, parent)
         #: Status as a string ``PASS`` or ``FAIL``. See also :attr:`passed`.
         self.status = status
         #: Test message. Typically a failure message but can be set also when
         #: test passes.
         self.message = message
         #: Test case execution start time in format ``%Y%m%d %H:%M:%S.%f``.
         self.starttime = starttime
         #: Test case execution end time in format ``%Y%m%d %H:%M:%S.%f``.
         self.endtime = endtime
 
     @property
-    def not_run(self):
+    def not_run(self) -> bool:
         return False
 
     @property
-    def critical(self):
+    def critical(self) -> bool:
         warnings.warn("'TestCase.critical' is deprecated and always returns 'True'.")
         return True
 
+    @setter
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
+        """Test body as a :class:`~robot.result.Body` object."""
+        return self.body_class(self, body)
+
 
-class TestSuite(model.TestSuite, StatusMixin):
+class TestSuite(model.TestSuite[Keyword, TestCase], StatusMixin):
     """Represents results of a single test suite.
 
     See the base class for documentation of attributes not documented here.
     """
     __slots__ = ['message', 'starttime', 'endtime']
     test_class = TestCase
     fixture_class = Keyword
 
-    def __init__(self, name='', doc='', metadata=None, source=None, message='',
-                 starttime=None, endtime=None, rpa=False, parent=None):
+    def __init__(self, name: str = '',
+                 doc: str = '',
+                 metadata: 'Mapping[str, str]|None' = None,
+                 source: 'Path|str|None' = None,
+                 rpa: bool = False,
+                 message: str = '',
+                 starttime: 'str|None' = None,
+                 endtime: 'str|None' = None,
+                 parent: 'TestSuite|None' = None):
         super().__init__(name, doc, metadata, source, rpa, parent)
         #: Possible suite setup or teardown error message.
         self.message = message
         #: Suite execution start time in format ``%Y%m%d %H:%M:%S.%f``.
         self.starttime = starttime
         #: Suite execution end time in format ``%Y%m%d %H:%M:%S.%f``.
         self.endtime = endtime
 
     @property
-    def passed(self):
+    def passed(self) -> bool:
         """``True`` if no test has failed but some have passed, ``False`` otherwise."""
         return self.status == self.PASS
 
     @property
-    def failed(self):
+    def failed(self) -> bool:
         """``True`` if any test has failed, ``False`` otherwise."""
         return self.status == self.FAIL
 
     @property
-    def skipped(self):
+    def skipped(self) -> bool:
         """``True`` if there are no passed or failed tests, ``False`` otherwise."""
         return self.status == self.SKIP
 
     @property
-    def not_run(self):
+    def not_run(self) -> bool:
         return False
 
     @property
-    def status(self):
+    def status(self) -> "Literal['PASS', 'SKIP', 'FAIL']":
         """'PASS', 'FAIL' or 'SKIP' depending on test statuses.
 
         - If any test has failed, status is 'FAIL'.
         - If no test has failed but at least some test has passed, status is 'PASS'.
         - If there are no failed or passed tests, status is 'SKIP'. This covers both
           the case when all tests have been skipped and when there are no tests.
         """
@@ -703,59 +867,63 @@
         if stats.failed:
             return self.FAIL
         if stats.passed:
             return self.PASS
         return self.SKIP
 
     @property
-    def statistics(self):
+    def statistics(self) -> TotalStatistics:
         """Suite statistics as a :class:`~robot.model.totalstatistics.TotalStatistics` object.
 
         Recreated every time this property is accessed, so saving the results
         to a variable and inspecting it is often a good idea::
 
             stats = suite.statistics
             print(stats.failed)
             print(stats.total)
             print(stats.message)
         """
-        return TotalStatisticsBuilder(self, self.rpa).stats
+        return TotalStatisticsBuilder(self, bool(self.rpa)).stats
 
     @property
-    def full_message(self):
+    def full_message(self) -> str:
         """Combination of :attr:`message` and :attr:`stat_message`."""
         if not self.message:
             return self.stat_message
-        return '%s\n\n%s' % (self.message, self.stat_message)
+        return f'{self.message}\n\n{self.stat_message}'
 
     @property
-    def stat_message(self):
+    def stat_message(self) -> str:
         """String representation of the :attr:`statistics`."""
         return self.statistics.message
 
     @property
-    def elapsedtime(self):
+    def elapsedtime(self) -> int:
         """Total execution time in milliseconds."""
         if self.starttime and self.endtime:
             return get_elapsed_time(self.starttime, self.endtime)
         return sum(child.elapsedtime for child in
                    chain(self.suites, self.tests, (self.setup, self.teardown)))
 
-    def remove_keywords(self, how):
+    @setter
+    def suites(self, suites: 'Sequence[TestSuite|DataDict]') -> TestSuites['TestSuite']:
+        return TestSuites['TestSuite'](self.__class__, self, suites)
+
+    def remove_keywords(self, how: str):
         """Remove keywords based on the given condition.
 
         :param how: What approach to use when removing keywords. Either
             ``ALL``, ``PASSED``, ``FOR``, ``WUKS``, or ``NAME:<pattern>``.
 
         For more information about the possible values see the documentation
         of the ``--removekeywords`` command line option.
         """
         self.visit(KeywordRemover(how))
 
-    def filter_messages(self, log_level='TRACE'):
+    def filter_messages(self, log_level: str = 'TRACE'):
         """Remove log messages below the specified ``log_level``."""
         self.visit(MessageFilter(log_level))
 
     def configure(self, **options):
         """A shortcut to configure a suite using one method call.
 
         Can only be used with the root test suite.
@@ -769,21 +937,21 @@
             suite.configure(remove_keywords='PASSED',
                             doc='Smoke test results.')
 
         Not to be confused with :meth:`config` method that suites, tests,
         and keywords have to make it possible to set multiple attributes in
         one call.
         """
-        model.TestSuite.configure(self)    # Parent validates call is allowed.
+        super().configure()    # Parent validates is call allowed.
         self.visit(SuiteConfigurer(**options))
 
     def handle_suite_teardown_failures(self):
         """Internal usage only."""
         self.visit(SuiteTeardownFailureHandler())
 
-    def suite_teardown_failed(self, error):
+    def suite_teardown_failed(self, message: str):
         """Internal usage only."""
-        self.visit(SuiteTeardownFailed(error))
+        self.visit(SuiteTeardownFailed(message))
 
-    def suite_teardown_skipped(self, message):
+    def suite_teardown_skipped(self, message: str):
         """Internal usage only."""
         self.visit(SuiteTeardownFailed(message, skipped=True))
```

## Comparing `robotframework-6.1b1/src/robot/result/configurer.py` & `robotframework-6.1rc1/src/robot/result/configurer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/listeners.py` & `robotframework-6.1rc1/src/robot/output/listeners.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/output.py` & `robotframework-6.1rc1/src/robot/output/output.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/listenermethods.py` & `robotframework-6.1rc1/src/robot/output/listenermethods.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/pyloggingconf.py` & `robotframework-6.1rc1/src/robot/output/pyloggingconf.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/filelogger.py` & `robotframework-6.1rc1/src/robot/output/filelogger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/loggerhelper.py` & `robotframework-6.1rc1/src/robot/output/loggerhelper.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/stdoutlogsplitter.py` & `robotframework-6.1rc1/src/robot/output/stdoutlogsplitter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/logger.py` & `robotframework-6.1rc1/src/robot/output/logger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/librarylogger.py` & `robotframework-6.1rc1/src/robot/output/librarylogger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/__init__.py` & `robotframework-6.1rc1/src/robot/output/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/debugfile.py` & `robotframework-6.1rc1/src/robot/output/debugfile.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/xmllogger.py` & `robotframework-6.1rc1/src/robot/output/xmllogger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/listenerarguments.py` & `robotframework-6.1rc1/src/robot/output/listenerarguments.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/console/quiet.py` & `robotframework-6.1rc1/src/robot/output/console/quiet.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/console/verbose.py` & `robotframework-6.1rc1/src/robot/output/console/verbose.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/console/__init__.py` & `robotframework-6.1rc1/src/robot/output/console/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/console/dotted.py` & `robotframework-6.1rc1/src/robot/output/console/dotted.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/output/console/highlighting.py` & `robotframework-6.1rc1/src/robot/output/console/highlighting.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/message.py` & `robotframework-6.1rc1/src/robot/model/message.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/stats.py` & `robotframework-6.1rc1/src/robot/model/stats.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/testcase.py` & `robotframework-6.1rc1/src/robot/model/testcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,67 +9,76 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import sys
 from pathlib import Path
-from typing import Any, Iterable, Mapping, Sequence, Type, TYPE_CHECKING
+from typing import Any, Generic, Sequence, Type, TYPE_CHECKING, TypeVar
 
 from robot.utils import setter
 
-from .body import Body
+from .body import Body, BodyItem
 from .fixture import create_fixture
 from .itemlist import ItemList
 from .keyword import Keyword, Keywords
-from .modelobject import ModelObject
+from .modelobject import DataDict, ModelObject
 from .tags import Tags
 
 if TYPE_CHECKING:
     from .testsuite import TestSuite
     from .visitor import SuiteVisitor
 
 
-class TestCase(ModelObject):
+TC = TypeVar('TC', bound='TestCase')
+KW = TypeVar('KW', bound='Keyword', covariant=True)
+
+
+class TestCase(ModelObject, Generic[KW] if sys.version_info >= (3, 7) else object):
     """Base model for a single test case.
 
     Extended by :class:`robot.running.model.TestCase` and
     :class:`robot.result.model.TestCase`.
     """
     body_class = Body
-    fixture_class = Keyword
+    # See model.TestSuite on removing the type ignore directive
+    fixture_class: Type[KW] = Keyword # type: ignore
     repr_args = ('name',)
     __slots__ = ['parent', 'name', 'doc', 'timeout', 'lineno', '_setup', '_teardown']
 
-    def __init__(self, name: str = '', doc: str = '', tags: Sequence[str] = (),
-                 timeout: 'str|None' = None, lineno: 'int|None' = None,
+    def __init__(self, name: str = '',
+                 doc: str = '',
+                 tags: Sequence[str] = (),
+                 timeout: 'str|None' = None,
+                 lineno: 'int|None' = None,
                  parent: 'TestSuite|None' = None):
         self.name = name
         self.doc = doc
         self.tags = tags
         self.timeout = timeout
         self.lineno = lineno
         self.parent = parent
         self.body = []
-        self._setup: 'Keyword|None' = None
-        self._teardown: 'Keyword|None' = None
+        self._setup: 'KW|None' = None
+        self._teardown: 'KW|None' = None
 
     @setter
-    def body(self, body: 'Iterable[Keyword|Mapping]') -> Body:
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
         """Test body as a :class:`~robot.model.body.Body` object."""
         return self.body_class(self, body)
 
     @setter
     def tags(self, tags: Sequence[str]) -> Tags:
         """Test tags as a :class:`~.model.tags.Tags` object."""
         return Tags(tags)
 
     @property
-    def setup(self) -> Keyword:
+    def setup(self) -> KW:
         """Test setup as a :class:`~.model.keyword.Keyword` object.
 
         This attribute is a ``Keyword`` object also when a test has no setup
         but in that case its truth value is ``False``.
 
         Setup can be modified by setting attributes directly::
 
@@ -86,20 +95,20 @@
 
             test.setup = None
 
         New in Robot Framework 4.0. Earlier setup was accessed like
         ``test.keywords.setup``.
         """
         if self._setup is None:
-            self._setup = create_fixture(None, self, Keyword.SETUP)
+            self._setup = create_fixture(self.fixture_class, None, self, Keyword.SETUP)
         return self._setup
 
     @setup.setter
-    def setup(self, setup: 'Keyword|Mapping|None'):
-        self._setup = create_fixture(setup, self, Keyword.SETUP)
+    def setup(self, setup: 'KW|DataDict|None'):
+        self._setup = create_fixture(self.fixture_class, setup, self, Keyword.SETUP)
 
     @property
     def has_setup(self) -> bool:
         """Check does a suite have a setup without creating a setup object.
 
         A difference between using ``if test.has_setup:`` and ``if test.setup:``
         is that accessing the :attr:`setup` attribute creates a :class:`Keyword`
@@ -114,20 +123,20 @@
     @property
     def teardown(self) -> Keyword:
         """Test teardown as a :class:`~.model.keyword.Keyword` object.
 
         See :attr:`setup` for more information.
         """
         if self._teardown is None:
-            self._teardown = create_fixture(None, self, Keyword.TEARDOWN)
+            self._teardown = create_fixture(self.fixture_class, None, self, Keyword.TEARDOWN)
         return self._teardown
 
     @teardown.setter
-    def teardown(self, teardown: 'Keyword|Mapping|None'):
-        self._teardown = create_fixture(teardown, self, Keyword.TEARDOWN)
+    def teardown(self, teardown: 'KW|DataDict|None'):
+        self._teardown = create_fixture(self.fixture_class, teardown, self, Keyword.TEARDOWN)
 
     @property
     def has_teardown(self) -> bool:
         """Check does a test have a teardown without creating a teardown object.
 
         See :attr:`has_setup` for more information.
 
@@ -180,33 +189,33 @@
         return self.name
 
     def to_dict(self) -> 'dict[str, Any]':
         data: 'dict[str, Any]' = {'name': self.name}
         if self.doc:
             data['doc'] = self.doc
         if self.tags:
-            data['tags'] = list(self.tags)
+            data['tags'] = tuple(self.tags)
         if self.timeout:
             data['timeout'] = self.timeout
         if self.lineno:
             data['lineno'] = self.lineno
         if self.has_setup:
             data['setup'] = self.setup.to_dict()
         if self.has_teardown:
             data['teardown'] = self.teardown.to_dict()
         data['body'] = self.body.to_dicts()
         return data
 
 
-class TestCases(ItemList[TestCase]):
+class TestCases(ItemList[TC]):
     __slots__ = []
 
-    def __init__(self, test_class: Type[TestCase] = TestCase,
+    def __init__(self, test_class: Type[TC] = TestCase,
                  parent: 'TestSuite|None' = None,
-                 tests: 'Sequence[TestCase|Mapping]' = ()):
+                 tests: 'Sequence[TC|DataDict]' = ()):
         super().__init__(test_class, {'parent': parent}, tests)
 
     def _check_type_and_set_attrs(self, test):
         test = super()._check_type_and_set_attrs(test)
         if test.parent:
             for visitor in test.parent._visitors:
                 test.visit(visitor)
```

## Comparing `robotframework-6.1b1/src/robot/model/tags.py` & `robotframework-6.1rc1/src/robot/model/tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from abc import ABC, abstractmethod
-from typing import Iterator, overload, Sequence
+from typing import Any, Iterable, Iterator, overload, Sequence
 
-from robot.utils import is_string, normalize, NormalizedDict, Matcher
+from robot.utils import normalize, NormalizedDict, Matcher
 
 
 class Tags(Sequence[str]):
     __slots__ = ['_tags', '_reserved']
 
-    def __init__(self, tags: Sequence[str] = ()):
+    def __init__(self, tags: Iterable[str] = ()):
         if isinstance(tags, Tags):
             self._tags, self._reserved = tags._tags, tags._reserved
         else:
             self._tags, self._reserved = self._init_tags(tags)
 
     def robot(self, name: str) -> bool:
         """Check do tags contain a reserved tag in format `robot:<name>`.
@@ -34,38 +34,38 @@
         This is same as `'robot:<name>' in tags` but considerably faster.
         """
         return name in self._reserved
 
     def _init_tags(self, tags) -> 'tuple[tuple[str, ...], tuple[str, ...]]':
         if not tags:
             return (), ()
-        if is_string(tags):
+        if isinstance(tags, str):
             tags = (tags,)
         return self._normalize(tags)
 
     def _normalize(self, tags):
         nd = NormalizedDict([(str(t), None) for t in tags], ignore='_')
         if '' in nd:
             del nd['']
         if 'NONE' in nd:
             del nd['NONE']
         reserved = tuple(tag[6:] for tag in nd.normalized_keys if tag[:6] == 'robot:')
         return tuple(nd), reserved
 
-    def add(self, tags: Sequence[str]):
+    def add(self, tags: Iterable[str]):
         self.__init__(tuple(self) + tuple(Tags(tags)))
 
-    def remove(self, tags: Sequence[str]):
+    def remove(self, tags: Iterable[str]):
         match = TagPatterns(tags).match
         self.__init__([t for t in self if not match(t)])
 
-    def match(self, tags: Sequence[str]) -> bool:
+    def match(self, tags: Iterable[str]) -> bool:
         return TagPatterns(tags).match(self)
 
-    def __contains__(self, tags) -> bool:
+    def __contains__(self, tags: Iterable[str]) -> bool:
         return self.match(tags)
 
     def __len__(self) -> int:
         return len(self._tags)
 
     def __iter__(self) -> Iterator[str]:
         return iter(self._tags)
@@ -73,15 +73,17 @@
     def __str__(self) -> str:
         tags = ', '.join(self)
         return f'[{tags}]'
 
     def __repr__(self) -> str:
         return repr(list(self))
 
-    def __eq__(self, other) -> bool:
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, Iterable):
+            return False
         if not isinstance(other, Tags):
             other = Tags(other)
         self_normalized = [normalize(tag, ignore='_') for tag in self]
         other_normalized = [normalize(tag, ignore='_') for tag in other]
         return sorted(self_normalized) == sorted(other_normalized)
 
     @overload
@@ -93,27 +95,27 @@
         ...
 
     def __getitem__(self, index: 'int|slice') -> 'str|Tags':
         if isinstance(index, slice):
             return Tags(self._tags[index])
         return self._tags[index]
 
-    def __add__(self, other: Sequence[str]) -> 'Tags':
+    def __add__(self, other: Iterable[str]) -> 'Tags':
         return Tags(tuple(self) + tuple(Tags(other)))
 
 
 class TagPatterns(Sequence['TagPattern']):
 
-    def __init__(self, patterns: Sequence[str]):
+    def __init__(self, patterns: Iterable[str]):
         self._patterns = tuple(TagPattern.from_string(p) for p in Tags(patterns))
 
-    def match(self, tags: Sequence[str]) -> bool:
+    def match(self, tags: Iterable[str]) -> bool:
         if not self._patterns:
             return False
-        tags = tags if isinstance(tags, Tags) else Tags(tags)
+        tags = normalize_tags(tags)
         return any(p.match(tags) for p in self._patterns)
 
     def __contains__(self, tag: str) -> bool:
         return self.match(tag)
 
     def __len__(self) -> int:
         return len(self._patterns)
@@ -140,84 +142,103 @@
         if 'OR' in pattern:
             return OrTagPattern(pattern.split('OR'))
         if 'AND' in pattern or '&' in pattern:
             return AndTagPattern(pattern.replace('&', 'AND').split('AND'))
         return SingleTagPattern(pattern)
 
     @abstractmethod
-    def match(self, tags: Sequence[str]) -> bool:
+    def match(self, tags: Iterable[str]) -> bool:
         raise NotImplementedError
 
     @abstractmethod
     def __iter__(self) -> Iterator['TagPattern']:
         raise NotImplementedError
 
     @abstractmethod
     def __str__(self) -> str:
         raise NotImplementedError
 
 
 class SingleTagPattern(TagPattern):
 
     def __init__(self, pattern: str):
-        self._matcher = Matcher(pattern, ignore='_')
+        # Normalization is handled here, not in Matcher, for performance reasons.
+        # This way we can normalize tags only once.
+        self._matcher = Matcher(normalize(pattern, ignore='_'),
+                                caseless=False, spaceless=False)
 
-    def match(self, tags: Sequence[str]) -> bool:
+    def match(self, tags: Iterable[str]) -> bool:
+        tags = normalize_tags(tags)
         return self._matcher.match_any(tags)
 
     def __iter__(self) -> Iterator['TagPattern']:
         yield self
 
     def __str__(self) -> str:
         return self._matcher.pattern
 
     def __bool__(self) -> bool:
         return bool(self._matcher)
 
 
 class AndTagPattern(TagPattern):
 
-    def __init__(self, patterns: Sequence[str]):
+    def __init__(self, patterns: Iterable[str]):
         self._patterns = tuple(TagPattern.from_string(p) for p in patterns)
 
-    def match(self, tags: Sequence[str]) -> bool:
+    def match(self, tags: Iterable[str]) -> bool:
+        tags = normalize_tags(tags)
         return all(p.match(tags) for p in self._patterns)
 
     def __iter__(self) -> Iterator['TagPattern']:
         return iter(self._patterns)
 
     def __str__(self) -> str:
         return ' AND '.join(str(pattern) for pattern in self)
 
 
 class OrTagPattern(TagPattern):
 
-    def __init__(self, patterns: Sequence[str]):
+    def __init__(self, patterns: Iterable[str]):
         self._patterns = tuple(TagPattern.from_string(p) for p in patterns)
 
-    def match(self, tags: Sequence[str]) -> bool:
+    def match(self, tags: Iterable[str]) -> bool:
+        tags = normalize_tags(tags)
         return any(p.match(tags) for p in self._patterns)
 
     def __iter__(self) -> Iterator['TagPattern']:
         return iter(self._patterns)
 
     def __str__(self) -> str:
         return ' OR '.join(str(pattern) for pattern in self)
 
 
 class NotTagPattern(TagPattern):
 
-    def __init__(self, must_match: str, must_not_match: Sequence[str]):
+    def __init__(self, must_match: str, must_not_match: Iterable[str]):
         self._first = TagPattern.from_string(must_match)
         self._rest = OrTagPattern(must_not_match)
 
-    def match(self, tags: Sequence[str]) -> bool:
-        if not self._first:
-            return not self._rest.match(tags)
-        return self._first.match(tags) and not self._rest.match(tags)
+    def match(self, tags: Iterable[str]) -> bool:
+        tags = normalize_tags(tags)
+        return ((self._first.match(tags) or not self._first)
+                and not self._rest.match(tags))
 
     def __iter__(self) -> Iterator['TagPattern']:
         yield self._first
         yield from self._rest
 
     def __str__(self) -> str:
         return ' NOT '.join(str(pattern) for pattern in self).lstrip()
+
+
+def normalize_tags(tags: Iterable[str]) -> Iterable[str]:
+    """Performance optimization to normalize tags only once."""
+    if isinstance(tags, NormalizedTags):
+        return tags
+    if isinstance(tags, str):
+        tags = [tags]
+    return NormalizedTags([normalize(t, ignore='_') for t in tags])
+
+
+class NormalizedTags(list):
+    pass
```

## Comparing `robotframework-6.1b1/src/robot/model/itemlist.py` & `robotframework-6.1rc1/src/robot/model/itemlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from functools import total_ordering
-from collections.abc import Mapping
-from typing import (Iterable, Iterator, MutableSequence, overload, TYPE_CHECKING,
+from typing import (Any, Iterable, Iterator, MutableSequence, overload, TYPE_CHECKING,
                     Type, TypeVar)
 
-from robot.utils import type_name
+from robot.utils import copy_signature, KnownAtRuntime, type_name
+
+from .modelobject import DataDict
 
 if TYPE_CHECKING:
     from .visitor import SuiteVisitor
 
 
 T = TypeVar('T')
 Self = TypeVar('Self', bound='ItemList')
@@ -40,54 +41,57 @@
     Starting from Robot Framework 6.1, items can be added as dictionaries and
     actual items are generated based on them automatically. If the type has
     a ``from_dict`` class method, it is used, and otherwise dictionary data is
     passed to the type as keyword arguments.
     """
 
     __slots__ = ['_item_class', '_common_attrs', '_items']
+    # TypeVar T needs to be applied to a variable to be compatible with @copy_signature
+    item_type: Type[T] = KnownAtRuntime
 
     def __init__(self, item_class: Type[T],
-                 common_attrs: 'Mapping|None' = None,
-                 items: 'Iterable[T|Mapping]' = ()):
+                 common_attrs: 'dict[str, Any]|None' = None,
+                 items: 'Iterable[T|DataDict]' = ()):
         self._item_class = item_class
         self._common_attrs = common_attrs
         self._items: 'list[T]' = []
         if items:
             self.extend(items)
 
+    @copy_signature(item_type)
     def create(self, *args, **kwargs) -> T:
         """Create a new item using the provided arguments."""
         return self.append(self._item_class(*args, **kwargs))
 
-    def append(self, item: 'T|Mapping'):
+    def append(self, item: 'T|DataDict') -> T:
         item = self._check_type_and_set_attrs(item)
         self._items.append(item)
         return item
 
-    def _check_type_and_set_attrs(self, item: 'T|Mapping') -> T:
+    def _check_type_and_set_attrs(self, item: 'T|DataDict') -> T:
         if not isinstance(item, self._item_class):
-            if isinstance(item, Mapping):
+            if isinstance(item, dict):
                 item = self._item_from_dict(item)
             else:
                 raise TypeError(f'Only {type_name(self._item_class)} objects '
                                 f'accepted, got {type_name(item)}.')
         if self._common_attrs:
             for attr, value in self._common_attrs.items():
                 setattr(item, attr, value)
         return item
 
-    def _item_from_dict(self, data: Mapping) -> T:
+    def _item_from_dict(self, data: DataDict) -> T:
         if hasattr(self._item_class, 'from_dict'):
             return self._item_class.from_dict(data)    # type: ignore
         return self._item_class(**data)
 
-    def extend(self, items: 'Iterable[T|Mapping]'):
+    def extend(self, items: 'Iterable[T|DataDict]'):
         self._items.extend(self._check_type_and_set_attrs(i) for i in items)
 
-    def insert(self, index: int, item: 'T|Mapping'):
+    def insert(self, index: int, item: 'T|DataDict'):
         item = self._check_type_and_set_attrs(item)
         self._items.insert(index, item)
 
     def index(self, item: T, *start_and_end) -> int:
         return self._items.index(item, *start_and_end)
 
     def clear(self):
@@ -121,19 +125,19 @@
         # subclasses don't have compatible __init__.
         new = type(self)(self._item_class)
         new._common_attrs = self._common_attrs
         new.extend(items)
         return new
 
     @overload
-    def __setitem__(self, index: int, item: 'T|Mapping'):
+    def __setitem__(self, index: int, item: 'T|DataDict'):
         ...
 
     @overload
-    def __setitem__(self, index: slice, item: 'Iterable[T|Mapping]'):
+    def __setitem__(self, index: slice, item: 'Iterable[T|DataDict]'):
         ...
 
     def __setitem__(self, index, item):
         if isinstance(index, slice):
             self._items[index] = [self._check_type_and_set_attrs(i) for i in item]
         else:
             self._items[index] = self._check_type_and_set_attrs(item)
@@ -205,15 +209,15 @@
     def __imul__(self: Self, count: int) -> Self:
         self._items *= count
         return self
 
     def __rmul__(self: Self, count: int) -> Self:
         return self * count
 
-    def to_dicts(self) -> 'list[dict]':
+    def to_dicts(self) -> 'list[DataDict]':
         """Return list of items converted to dictionaries.
 
         Items are converted to dictionaries using the ``to_dict`` method, if
         they have it, or the built-in ``vars()``.
 
         New in Robot Framework 6.1.
         """
```

## Comparing `robotframework-6.1b1/src/robot/model/testsuite.py` & `robotframework-6.1rc1/src/robot/running/builder/builders.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,329 +9,303 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from collections.abc import Mapping
+import warnings
+from itertools import chain
+from os.path import normpath
 from pathlib import Path
-from typing import Any, Iterator, Sequence, Type
+from typing import cast, Sequence
 
-from robot.utils import setter
-
-from .configurer import SuiteConfigurer
-from .filter import Filter, EmptySuiteRemover
-from .fixture import create_fixture
-from .itemlist import ItemList
-from .keyword import Keyword, Keywords
-from .metadata import Metadata
-from .modelobject import ModelObject
-from .tagsetter import TagSetter
-from .testcase import TestCase, TestCases
-from .visitor import SuiteVisitor
-
-
-class TestSuite(ModelObject):
-    """Base model for single suite.
-
-    Extended by :class:`robot.running.model.TestSuite` and
-    :class:`robot.result.model.TestSuite`.
+from robot.conf import LanguagesLike
+from robot.errors import DataError
+from robot.output import LOGGER
+from robot.parsing import (SuiteFile, SuiteDirectory, SuiteStructure,
+                           SuiteStructureBuilder, SuiteStructureVisitor)
+from robot.utils import Importer, seq2str, split_args_from_name_or_path, type_name
+
+from ..model import ResourceFile, TestSuite
+from .parsers import (CustomParser, JsonParser, NoInitFileDirectoryParser, Parser,
+                      RestParser, RobotParser)
+from .settings import TestDefaults
+
+
+class TestSuiteBuilder:
+    """Builder to construct ``TestSuite`` objects based on data on the disk.
+
+    The :meth:`build` method constructs executable
+    :class:`~robot.running.model.TestSuite` objects based on test data files
+    or directories. There are two main use cases for this API:
+
+    - Execute the created suite by using its
+      :meth:`~robot.running.model.TestSuite.run` method. The suite can be
+      modified before execution if needed.
+
+    - Inspect the suite to see, for example, what tests it has or what tags
+      tests have. This can be more convenient than using the lower level
+      :mod:`~robot.parsing` APIs.
+
+    Both modifying the suite and inspecting what data it contains are easiest
+    done by using the :mod:`~robot.model.visitor` interface.
+
+    This class is part of the public API and should be imported via the
+    :mod:`robot.api` package. An alternative is using the
+    :meth:`TestSuite.from_file_system <robot.running.model.TestSuite.from_file_system>`
+    classmethod that uses this class internally.
     """
-    test_class = TestCase    #: Internal usage only.
-    fixture_class = Keyword  #: Internal usage only.
-    repr_args = ('name',)
-    __slots__ = ['parent', '_name', 'doc', '_setup', '_teardown', 'rpa', '_my_visitors']
-
-    def __init__(self, name: str = '', doc: str = '', metadata: 'Mapping|None' = None,
-                 source: 'Path|str|None' = None, rpa: 'bool|None' = None,
-                 parent: 'TestSuite|None' = None):
-        self._name = name
-        self.doc = doc
-        self.metadata = metadata
-        self.source = source
-        self.parent = parent
+
+    def __init__(self, included_suites: str = 'DEPRECATED',
+                 included_extensions: Sequence[str] = ('.robot', '.rbt', '.robot.rst'),
+                 included_files: Sequence[str] = (),
+                 custom_parsers: Sequence[str] = (),
+                 defaults: 'TestDefaults|None' = None,
+                 rpa: 'bool|None' = None,
+                 lang: LanguagesLike = None,
+                 allow_empty_suite: bool = False,
+                 process_curdir: bool = True):
+        """
+        :param included_suites:
+            This argument used to be used for limiting what suite file to parse.
+            It is deprecated and has no effect starting from RF 6.1. Use the
+            new ``included_files`` argument or filter the created suite after
+            parsing instead.
+        :param included_extensions:
+            List of extensions of files to parse. Same as ``--extension``.
+        :param included_files:
+            List of names, paths or directory paths of files to parse. All files
+            are parsed by default. Same as `--parse-include`. New in RF 6.1.
+        :param custom_parsers:
+            Custom parsers as names or paths (same as ``--parser``) or as
+            parser objects. New in RF 6.1.
+        :param defaults:
+            Possible test specific defaults from suite initialization files.
+            New in RF 6.1.
+        :param rpa:
+            Explicit execution mode. ``True`` for RPA and ``False`` for test
+            automation. By default, mode is got from data file headers and possible
+            conflicting headers cause an error. Same as ``--rpa`` or ``--norpa``.
+        :param lang:
+            Additional languages to be supported during parsing.
+            Can be a string matching any of the supported language codes or names,
+            an initialized :class:`~robot.conf.languages.Language` subclass,
+            a list containing such strings or instances, or a
+            :class:`~robot.conf.languages.Languages` instance.
+        :param allow_empty_suite:
+            Specify is it an error if the built suite contains no tests.
+            Same as ``--runemptysuite``.
+        :param process_curdir:
+            Control processing the special ``${CURDIR}`` variable. It is
+            resolved already at parsing time by default, but that can be
+            changed by giving this argument ``False`` value.
+        """
+        self.standard_parsers = self._get_standard_parsers(lang, process_curdir)
+        self.custom_parsers = self._get_custom_parsers(custom_parsers)
+        self.defaults = defaults
+        self.included_extensions = tuple(included_extensions or ())
+        self.included_files = tuple(included_files or ())
         self.rpa = rpa
-        self.suites = []
-        self.tests = []
-        self._setup: 'Keyword|None' = None
-        self._teardown: 'Keyword|None' = None
-        self._my_visitors: 'list[SuiteVisitor]' = []
-
-    @staticmethod
-    def name_from_source(source: 'Path|str|None') -> str:
-        if not source:
-            return ''
+        self.allow_empty_suite = allow_empty_suite
+        # TODO: Remove in RF 7.
+        if included_suites != 'DEPRECATED':
+            warnings.warn("'TestSuiteBuilder' argument 'included_suites' is deprecated "
+                          "and has no effect. Use the new 'included_files' argument "
+                          "or filter the parsed suite instead.")
+
+    def _get_standard_parsers(self, lang: LanguagesLike,
+                              process_curdir: bool) -> 'dict[str, Parser]':
+        robot_parser = RobotParser(lang, process_curdir)
+        rest_parser = RestParser(lang, process_curdir)
+        json_parser = JsonParser()
+        return {
+            'robot': robot_parser,
+            'rst': rest_parser,
+            'rest': rest_parser,
+            'robot.rst': rest_parser,
+            'rbt': json_parser,
+            'json': json_parser
+        }
+
+    def _get_custom_parsers(self, parsers: Sequence[str]) -> 'dict[str, CustomParser]':
+        custom_parsers = {}
+        importer = Importer('parser', LOGGER)
+        for parser in parsers:
+            if isinstance(parser, (str, Path)):
+                name, args = split_args_from_name_or_path(parser)
+                parser = importer.import_class_or_module(name, args)
+            else:
+                name = type_name(parser)
+            try:
+                custom_parser = CustomParser(parser)
+            except TypeError as err:
+                raise DataError(f"Importing parser '{name}' failed: {err}")
+            for ext in custom_parser.extensions:
+                custom_parsers[ext] = custom_parser
+        return custom_parsers
+
+    def build(self, *paths: 'Path|str') -> TestSuite:
+        """
+        :param paths: Paths to test data files or directories.
+        :return: :class:`~robot.running.model.TestSuite` instance.
+        """
+        paths = self._normalize_paths(paths)
+        extensions = self.included_extensions + tuple(self.custom_parsers)
+        structure = SuiteStructureBuilder(extensions,
+                                          self.included_files).build(*paths)
+        suite = SuiteStructureParser(self._get_parsers(paths), self.defaults,
+                                     self.rpa).parse(structure)
+        if not self.allow_empty_suite:
+            self._validate_not_empty(suite, multi_source=len(paths) > 1)
+        suite.remove_empty_suites(preserve_direct_children=len(paths) > 1)
+        return suite
+
+    def _normalize_paths(self, paths: 'Sequence[Path|str]') -> 'tuple[Path, ...]':
+        if not paths:
+            raise DataError('One or more source paths required.')
+        # Cannot use `Path.resolve()` here because it resolves all symlinks which
+        # isn't desired. `Path` doesn't have any methods for normalizing paths
+        # so need to use `os.path.normpath()`. Also that _may_ resolve symlinks,
+        # but we need to do it for backwards compatibility.
+        paths = [Path(normpath(p)).absolute() for p in paths]
+        non_existing = [p for p in paths if not p.exists()]
+        if non_existing:
+            raise DataError(f"Parsing {seq2str(non_existing)} failed: "
+                            f"File or directory to execute does not exist.")
+        return tuple(paths)
+
+    def _get_parsers(self, paths: 'Sequence[Path]') -> 'dict[str|None, Parser]':
+        parsers = {None: NoInitFileDirectoryParser(), **self.custom_parsers}
+        robot_parser = self.standard_parsers['robot']
+        for ext in chain(self.included_extensions,
+                         [self._get_ext(pattern) for pattern in self.included_files],
+                         [self._get_ext(pth) for pth in paths if pth.is_file()]):
+            ext = ext.lstrip('.').lower()
+            if ext not in parsers and ext.replace('.', '').isalnum():
+                parsers[ext] = self.standard_parsers.get(ext, robot_parser)
+        return parsers
+
+    def _get_ext(self, path: 'str|Path') -> str:
+        if not isinstance(path, Path):
+            path = Path(path)
+        return ''.join(path.suffixes)
+
+    def _validate_not_empty(self, suite: TestSuite, multi_source: bool = False):
+        if multi_source:
+            for child in suite.suites:
+                self._validate_not_empty(child)
+        elif not suite.has_tests:
+            raise DataError(f"Suite '{suite.name}' contains no tests or tasks.")
+
+
+class SuiteStructureParser(SuiteStructureVisitor):
+
+    def __init__(self, parsers: 'dict[str|None, Parser]',
+                 defaults: 'TestDefaults|None' = None, rpa: 'bool|None' = None):
+        self.parsers = parsers
+        self.rpa = rpa
+        self.defaults = defaults
+        self._rpa_given = rpa is not None
+        self.suite: 'TestSuite|None' = None
+        self._stack: 'list[tuple[TestSuite, TestDefaults]]' = []
+
+    @property
+    def parent_defaults(self) -> 'TestDefaults|None':
+        return self._stack[-1][-1] if self._stack else self.defaults
+
+    def parse(self, structure: SuiteStructure) -> TestSuite:
+        structure.visit(self)
+        suite = cast(TestSuite, self.suite)
+        suite.rpa = self.rpa
+        return suite
+
+    def visit_file(self, structure: SuiteFile):
+        LOGGER.info(f"Parsing file '{structure.source}'.")
+        suite = self._build_suite_file(structure)
+        if self.suite is None:
+            self.suite = suite
+        else:
+            self._stack[-1][0].suites.append(suite)
+
+    def start_directory(self, structure: SuiteDirectory):
+        if structure.source:
+            LOGGER.info(f"Parsing directory '{structure.source}'.")
+        suite, defaults = self._build_suite_directory(structure)
+        if self.suite is None:
+            self.suite = suite
+        else:
+            self._stack[-1][0].suites.append(suite)
+        self._stack.append((suite, defaults))
+
+    def end_directory(self, structure: SuiteDirectory):
+        suite, _ = self._stack.pop()
+        if suite.rpa is None and suite.suites:
+            suite.rpa = suite.suites[0].rpa
+
+    def _build_suite_file(self, structure: SuiteFile):
+        source = cast(Path, structure.source)
+        defaults = self.parent_defaults or TestDefaults()
+        parser = self.parsers[structure.extension]
+        try:
+            suite = parser.parse_suite_file(source, defaults)
+            if not suite.tests:
+                LOGGER.info(f"Data source '{source}' has no tests or tasks.")
+            self._validate_execution_mode(suite)
+        except DataError as err:
+            raise DataError(f"Parsing '{source}' failed: {err.message}")
+        return suite
+
+    def _build_suite_directory(self, structure: SuiteDirectory):
+        source = cast(Path, structure.init_file or structure.source)
+        defaults = TestDefaults(self.parent_defaults)
+        parser = self.parsers[structure.extension]
+        try:
+            suite = parser.parse_init_file(source, defaults)
+            if structure.is_multi_source:
+                suite.config(name='', source=None)
+        except DataError as err:
+            raise DataError(f"Parsing '{source}' failed: {err.message}")
+        return suite, defaults
+
+    def _validate_execution_mode(self, suite: TestSuite):
+        if self._rpa_given:
+            suite.rpa = self.rpa
+        elif suite.rpa is None:
+            pass
+        elif self.rpa is None:
+            self.rpa = suite.rpa
+        elif self.rpa is not suite.rpa:
+            this, that = ('tasks', 'tests') if suite.rpa else ('tests', 'tasks')
+            raise DataError(f"Conflicting execution modes. File has {this} "
+                            f"but files parsed earlier have {that}. Fix headers "
+                            f"or use '--rpa' or '--norpa' options to set the "
+                            f"execution mode explicitly.")
+
+
+class ResourceFileBuilder:
+
+    def __init__(self, lang: LanguagesLike = None, process_curdir: bool = True):
+        self.lang = lang
+        self.process_curdir = process_curdir
+
+    def build(self, source: Path) -> ResourceFile:
         if not isinstance(source, Path):
             source = Path(source)
-        name = source.name if source.is_dir() else source.stem
-        if '__' in name:
-            name = name.split('__', 1)[1] or name
-        name = name.replace('_', ' ').strip()
-        return name.title() if name.islower() else name
-
-    @property
-    def _visitors(self) -> 'list[SuiteVisitor]':
-        parent_visitors = self.parent._visitors if self.parent else []
-        return self._my_visitors + parent_visitors
-
-    @property
-    def name(self) -> str:
-        """Suite name.
-
-        If name is not set, it is constructed from source. If source is not set,
-        name is constructed from child suite names by concatenating them with
-        `` & ``. If there are no child suites, name is an empty string.
-        """
-        return (self._name
-                or self.name_from_source(self.source)
-                or ' & '.join(s.name for s in self.suites))
-
-    @name.setter
-    def name(self, name: str):
-        self._name = name
-
-    @setter
-    def source(self, source: 'Path|str|None') -> 'Path|None':
-        return source if isinstance(source, (Path, type(None))) else Path(source)
-
-    @property
-    def longname(self) -> str:
-        """Suite name prefixed with the long name of the parent suite."""
-        if not self.parent:
-            return self.name
-        return f'{self.parent.longname}.{self.name}'
-
-    @setter
-    def metadata(self, metadata: 'Mapping|None') -> Metadata:
-        """Free suite metadata as dictionary-like ``Metadata`` object."""
-        return Metadata(metadata)
-
-    @setter
-    def suites(self, suites: 'Sequence[TestSuite|Mapping]') -> 'TestSuites':
-        return TestSuites(self.__class__, self, suites)
-
-    @setter
-    def tests(self, tests: 'Sequence[TestCase|Mapping]') -> TestCases:
-        return TestCases(self.test_class, self, tests)
-
-    @property
-    def setup(self) -> Keyword:
-        """Suite setup.
-
-        This attribute is a ``Keyword`` object also when a suite has no setup
-        but in that case its truth value is ``False``. The preferred way to
-        check does a suite have a setup is using :attr:`has_setup`.
-
-        Setup can be modified by setting attributes directly::
-
-            suite.setup.name = 'Example'
-            suite.setup.args = ('First', 'Second')
-
-        Alternatively the :meth:`config` method can be used to set multiple
-        attributes in one call::
-
-            suite.setup.config(name='Example', args=('First', 'Second'))
-
-        The easiest way to reset the whole setup is setting it to ``None``.
-        It will automatically recreate the underlying ``Keyword`` object::
-
-            suite.setup = None
-
-        New in Robot Framework 4.0. Earlier setup was accessed like
-        ``suite.keywords.setup``.
-        """
-        if self._setup is None:
-            self._setup = create_fixture(None, self, Keyword.SETUP)
-        return self._setup
-
-    @setup.setter
-    def setup(self, setup: 'Keyword|Mapping|None'):
-        self._setup = create_fixture(setup, self, Keyword.SETUP)
-
-    @property
-    def has_setup(self) -> bool:
-        """Check does a suite have a setup without creating a setup object.
-
-        A difference between using ``if suite.has_setup:`` and ``if suite.setup:``
-        is that accessing the :attr:`setup` attribute creates a :class:`Keyword`
-        object representing the setup even when the suite actually does not have
-        one. This typically does not matter, but with bigger suite structures
-        it can have some effect on memory usage.
-
-        New in Robot Framework 5.0.
-        """
-        return bool(self._setup)
-
-    @property
-    def teardown(self) -> Keyword:
-        """Suite teardown.
-
-        See :attr:`setup` for more information.
-        """
-        if self._teardown is None:
-            self._teardown = create_fixture(None, self, Keyword.TEARDOWN)
-        return self._teardown
-
-    @teardown.setter
-    def teardown(self, teardown: 'Keyword|Mapping|None'):
-        self._teardown = create_fixture(teardown, self, Keyword.TEARDOWN)
-
-    @property
-    def has_teardown(self) -> bool:
-        """Check does a suite have a teardown without creating a teardown object.
-
-        See :attr:`has_setup` for more information.
-
-        New in Robot Framework 5.0.
-        """
-        return bool(self._teardown)
-
-    @property
-    def keywords(self) -> Keywords:
-        """Deprecated since Robot Framework 4.0.
-
-        Use :attr:`setup` or :attr:`teardown` instead.
-        """
-        keywords = [self.setup, self.teardown]
-        return Keywords(self, [kw for kw in keywords if kw])
-
-    @keywords.setter
-    def keywords(self, keywords):
-        Keywords.raise_deprecation_error()
-
-    @property
-    def id(self) -> str:
-        """An automatically generated unique id.
-
-        The root suite has id ``s1``, its child suites have ids ``s1-s1``,
-        ``s1-s2``, ..., their child suites get ids ``s1-s1-s1``, ``s1-s1-s2``,
-        ..., ``s1-s2-s1``, ..., and so on.
-
-        The first test in a suite has an id like ``s1-t1``, the second has an
-        id ``s1-t2``, and so on. Similarly, keywords in suites (setup/teardown)
-        and in tests get ids like ``s1-k1``, ``s1-t1-k1``, and ``s1-s4-t2-k5``.
-        """
-        if not self.parent:
-            return 's1'
-        suites = self.parent.suites
-        index = suites.index(self) if self in suites else len(suites)
-        return f'{self.parent.id}-s{index + 1}'
-
-    @property
-    def all_tests(self) -> Iterator[TestCase]:
-        """Yields all tests this suite and its child suites contain.
-
-        New in Robot Framework 6.1.
-        """
-        yield from self.tests
-        for suite in self.suites:
-            yield from suite.all_tests
-
-    @property
-    def test_count(self) -> int:
-        """Total number of the tests in this suite and in its child suites."""
-        # This is considerably faster than `return len(list(self.all_tests))`.
-        return len(self.tests) + sum(suite.test_count for suite in self.suites)
-
-    @property
-    def has_tests(self) -> bool:
-        if self.tests:
-            return True
-        return any(s.has_tests for s in self.suites)
-
-    def set_tags(self, add: Sequence[str] = (), remove: Sequence[str] = (),
-                 persist: bool = False):
-        """Add and/or remove specified tags to the tests in this suite.
-
-        :param add: Tags to add as a list or, if adding only one,
-            as a single string.
-        :param remove: Tags to remove as a list or as a single string.
-            Can be given as patterns where ``*`` and ``?`` work as wildcards.
-        :param persist: Add/remove specified tags also to new tests added
-            to this suite in the future.
-        """
-        setter = TagSetter(add, remove)
-        self.visit(setter)
-        if persist:
-            self._my_visitors.append(setter)
-
-    def filter(self, included_suites: 'Sequence[str]|None' = None,
-               included_tests: 'Sequence[str]|None' = None,
-               included_tags: 'Sequence[str]|None' = None,
-               excluded_tags: 'Sequence[str]|None' = None):
-        """Select test cases and remove others from this suite.
-
-        Parameters have the same semantics as ``--suite``, ``--test``,
-        ``--include``, and ``--exclude`` command line options. All of them
-        can be given as a list of strings, or when selecting only one, as
-        a single string.
-
-        Child suites that contain no tests after filtering are automatically
-        removed.
-
-        Example::
-
-            suite.filter(included_tests=['Test 1', '* Example'],
-                         included_tags='priority-1')
-        """
-        self.visit(Filter(included_suites, included_tests,
-                          included_tags, excluded_tags))
-
-    def configure(self, **options):
-        """A shortcut to configure a suite using one method call.
-
-        Can only be used with the root test suite.
-
-        :param options: Passed to
-            :class:`~robot.model.configurer.SuiteConfigurer` that will then
-            set suite attributes, call :meth:`filter`, etc. as needed.
-
-        Not to be confused with :meth:`config` method that suites, tests,
-        and keywords have to make it possible to set multiple attributes in
-        one call.
-        """
-        if self.parent is not None:
-            raise ValueError("'TestSuite.configure()' can only be used with "
-                             "the root test suite.")
-        if options:
-            self.visit(SuiteConfigurer(**options))
-
-    def remove_empty_suites(self, preserve_direct_children: bool = False):
-        """Removes all child suites not containing any tests, recursively."""
-        self.visit(EmptySuiteRemover(preserve_direct_children))
-
-    def visit(self, visitor: SuiteVisitor):
-        """:mod:`Visitor interface <robot.model.visitor>` entry-point."""
-        visitor.visit_suite(self)
-
-    def __str__(self) -> str:
-        return self.name
-
-    def to_dict(self) -> 'dict[str, Any]':
-        data: 'dict[str, Any]' = {'name': self.name}
-        if self.doc:
-            data['doc'] = self.doc
-        if self.metadata:
-            data['metadata'] = dict(self.metadata)
-        if self.source:
-            data['source'] = str(self.source)
-        if self.rpa:
-            data['rpa'] = self.rpa
-        if self.has_setup:
-            data['setup'] = self.setup.to_dict()
-        if self.has_teardown:
-            data['teardown'] = self.teardown.to_dict()
-        if self.tests:
-            data['tests'] = self.tests.to_dicts()
-        if self.suites:
-            data['suites'] = self.suites.to_dicts()
-        return data
-
-
-class TestSuites(ItemList[TestSuite]):
-    __slots__ = []
-
-    def __init__(self, suite_class: Type[TestSuite] = TestSuite,
-                 parent: 'TestSuite|None' = None,
-                 suites: 'Sequence[TestSuite|Mapping]' = ()):
-        super().__init__(suite_class, {'parent': parent}, suites)
+        LOGGER.info(f"Parsing resource file '{source}'.")
+        resource = self._parse(source)
+        if resource.imports or resource.variables or resource.keywords:
+            LOGGER.info(f"Imported resource file '{source}' ({len(resource.keywords)} "
+                        f"keywords).")
+        else:
+            LOGGER.warn(f"Imported resource file '{source}' is empty.")
+        return resource
+
+    def _parse(self, source: Path) -> ResourceFile:
+        suffix = source.suffix.lower()
+        if suffix in ('.rst', '.rest'):
+            parser = RestParser(self.lang, self.process_curdir)
+        elif suffix in ('.json', '.rsrc'):
+            parser = JsonParser()
+        else:
+            parser = RobotParser(self.lang, self.process_curdir)
+        return parser.parse_resource_file(source)
```

## Comparing `robotframework-6.1b1/src/robot/model/metadata.py` & `robotframework-6.1rc1/src/robot/reporting/outputwriter.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from robot.utils import is_string, NormalizedDict
+from robot.output.xmllogger import XmlLogger
 
 
-class Metadata(NormalizedDict):
+class OutputWriter(XmlLogger):
 
-    def __init__(self, initial=None):
-        super().__init__(initial, ignore='_')
+    def __init__(self, output, rpa=False):
+        XmlLogger.__init__(self, output, rpa=rpa, generator='Rebot')
 
-    def __setitem__(self, key, value):
-        if not is_string(key):
-            key = str(key)
-        if not is_string(value):
-            value = str(value)
-        super().__setitem__(key, value)
+    def start_message(self, msg):
+        self._write_message(msg)
 
-    def __str__(self):
-        return '{%s}' % ', '.join('%s: %s' % (k, self[k]) for k in self)
+    def close(self):
+        self._writer.end('robot')
+        self._writer.close()
+
+    def end_result(self, result):
+        self.close()
```

## Comparing `robotframework-6.1b1/src/robot/model/suitestatistics.py` & `robotframework-6.1rc1/src/robot/model/suitestatistics.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/modifier.py` & `robotframework-6.1rc1/src/robot/model/modifier.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/keyword.py` & `robotframework-6.1rc1/src/robot/model/keyword.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,121 +9,133 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Any, Sequence, Type, TYPE_CHECKING
+from typing import cast, Sequence, Type, TYPE_CHECKING
 import warnings
 
-from .body import Body, BodyItem
+from .body import Body, BodyItem, BodyItemParent
 from .itemlist import ItemList
+from .modelobject import DataDict
 
 if TYPE_CHECKING:
-    from .testcase import TestCase
-    from .testsuite import TestSuite
     from .visitor import SuiteVisitor
 
 
 @Body.register
 class Keyword(BodyItem):
     """Base model for a single keyword.
 
     Extended by :class:`robot.running.model.Keyword` and
     :class:`robot.result.model.Keyword`.
     """
     repr_args = ('name', 'args', 'assign')
     __slots__ = ['_name', 'args', 'assign', 'type']
 
-    def __init__(self, name: str = '', args: Sequence[str] = (),
-                 assign: Sequence[str] = (), type: str = BodyItem.KEYWORD,
-                 parent: 'TestSuite|TestCase|BodyItem|None' = None):
-        self._name = name
+    def __init__(self, name: 'str|None' = '',
+                 args: Sequence[str] = (),
+                 assign: Sequence[str] = (),
+                 type: str = BodyItem.KEYWORD,
+                 parent: BodyItemParent = None):
+        self.name = name
         self.args = args
         self.assign = assign
         self.type = type
         self.parent = parent
 
     @property
-    def name(self) -> str:
+    def name(self) -> 'str|None':
         return self._name
 
     @name.setter
-    def name(self, name: str):
+    def name(self, name: 'str|None'):
         self._name = name
 
+    @property
+    def id(self) -> 'str|None':
+        if not self:
+            return None
+        return super().id
+
     def visit(self, visitor: 'SuiteVisitor'):
         """:mod:`Visitor interface <robot.model.visitor>` entry-point."""
         if self:
             visitor.visit_keyword(self)
 
     def __bool__(self) -> bool:
         return self.name is not None
 
     def __str__(self) -> str:
         parts = list(self.assign) + [self.name] + list(self.args)
         return '    '.join(str(p) for p in parts)
 
-    def to_dict(self) -> 'dict[str, Any]':
-        data: 'dict[str, Any]' = {'name': self.name}
+    def to_dict(self) -> DataDict:
+        data: DataDict = {'name': self.name}
         if self.args:
             data['args'] = list(self.args)
         if self.assign:
             data['assign'] = list(self.assign)
         return data
 
 
-class Keywords(ItemList[Keyword]):
+# FIXME: Remote in RF 7.
+class Keywords(ItemList[BodyItem]):
     """A list-like object representing keywords in a suite, a test or a keyword.
 
     Read-only and deprecated since Robot Framework 4.0.
     """
     __slots__ = []
     deprecation_message = (
         "'keywords' attribute is read-only and deprecated since Robot Framework 4.0. "
         "Use 'body', 'setup' or 'teardown' instead."
     )
 
-    def __init__(self, parent: 'TestSuite|None' = None,
-                 keywords: 'Sequence[Keyword]|Keywords' = ()):
+    def __init__(self, parent: BodyItemParent = None,
+                 keywords: Sequence[BodyItem] = ()):
         warnings.warn(self.deprecation_message, UserWarning)
         ItemList.__init__(self, object, {'parent': parent})
         if keywords:
             ItemList.extend(self, keywords)
 
     @property
     def setup(self) -> 'Keyword|None':
-        return self[0] if (self and self[0].type == 'SETUP') else None
+        if self and self[0].type == 'SETUP':
+            return cast(Keyword, self[0])
+        return None
 
     @setup.setter
     def setup(self, kw):
         self.raise_deprecation_error()
 
     def create_setup(self, *args, **kwargs):
         self.raise_deprecation_error()
 
     @property
     def teardown(self) -> 'Keyword|None':
-        return self[-1] if (self and self[-1].type == 'TEARDOWN') else None
+        if self and self[-1].type == 'TEARDOWN':
+            return cast(Keyword, self[-1])
+        return None
 
     @teardown.setter
     def teardown(self, kw: Keyword):
         self.raise_deprecation_error()
 
     def create_teardown(self, *args, **kwargs):
         self.raise_deprecation_error()
 
     @property
     def all(self) -> 'Keywords':
         """Iterates over all keywords, including setup and teardown."""
         return self
 
     @property
-    def normal(self) -> 'list[Keyword]':
+    def normal(self) -> 'list[BodyItem]':
         """Iterates over normal keywords, omitting setup and teardown."""
         return [kw for kw in self if kw.type not in ('SETUP', 'TEARDOWN')]
 
     def __setitem__(self, index: int, item: Keyword):
         self.raise_deprecation_error()
 
     def create(self, *args, **kwargs):
```

## Comparing `robotframework-6.1b1/src/robot/model/namepatterns.py` & `robotframework-6.1rc1/src/robot/model/namepatterns.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,31 +9,32 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Iterable, Iterator
+from typing import Iterable, Iterator, Sequence
 
 from robot.utils import MultiMatcher
 
 
 class NamePatterns(Iterable[str]):
 
-    def __init__(self, patterns: Iterator[str] = ()):
-        self.matcher = MultiMatcher(patterns, ignore='_')
+    def __init__(self, patterns: Sequence[str] = (), ignore: Sequence[str] = '_'):
+        self.matcher = MultiMatcher(patterns, ignore)
 
     def match(self, name: str, longname: 'str|None' = None) -> bool:
-        return self._match(name) or longname and self._match_longname(longname)
+        return bool(self._match(name) or
+                    longname and self._match_longname(longname))
 
-    def _match(self, name):
+    def _match(self, name: str) -> bool:
         return self.matcher.match(name)
 
-    def _match_longname(self, name):
+    def _match_longname(self, name: str) -> bool:
         raise NotImplementedError
 
     def __bool__(self) -> bool:
         return bool(self.matcher)
 
     def __iter__(self) -> Iterator[str]:
         for matcher in self.matcher:
```

## Comparing `robotframework-6.1b1/src/robot/model/tagsetter.py` & `robotframework-6.1rc1/src/robot/model/tagsetter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/__init__.py` & `robotframework-6.1rc1/src/robot/model/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 These classes are extended both by :mod:`execution <robot.running.model>`
 and :mod:`result <robot.result.model>` related model objects and used also
 elsewhere.
 
 This package is considered stable.
 """
 
-from .body import BaseBody, Body, BodyItem, Branches
+from .body import BaseBody, Body, BodyItem, BaseBranches
 from .configurer import SuiteConfigurer
 from .control import Break, Continue, Error, For, If, IfBranch, Return, Try, TryBranch, While
 from .fixture import create_fixture
 from .itemlist import ItemList
 from .keyword import Keyword, Keywords
 from .message import Message, Messages
-from .modelobject import ModelObject
+from .modelobject import DataDict, ModelObject
 from .modifier import ModelModifier
 from .namepatterns import SuiteNamePatterns, TestNamePatterns
 from .statistics import Statistics
 from .tags import Tags, TagPattern, TagPatterns
-from .testcase import TestCase
-from .testsuite import TestSuite
-from .totalstatistics import TotalStatisticsBuilder
+from .testcase import TestCase, TestCases
+from .testsuite import TestSuite, TestSuites
+from .totalstatistics import TotalStatistics, TotalStatisticsBuilder
 from .visitor import SuiteVisitor
```

## Comparing `robotframework-6.1b1/src/robot/model/visitor.py` & `robotframework-6.1rc1/src/robot/model/visitor.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/totalstatistics.py` & `robotframework-6.1rc1/src/robot/model/totalstatistics.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,55 +9,57 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+from collections.abc import Iterator
+
 from robot.utils import test_or_task
 
 from .stats import TotalStat
 from .visitor import SuiteVisitor
 
 
 class TotalStatistics:
     """Container for total statistics."""
 
-    def __init__(self, rpa=False):
+    def __init__(self, rpa: bool = False):
         #: Instance of :class:`~robot.model.stats.TotalStat` for all the tests.
         self._stat = TotalStat(test_or_task('All {Test}s', rpa))
         self._rpa = rpa
 
     def visit(self, visitor):
         visitor.visit_total_statistics(self._stat)
 
-    def __iter__(self):
+    def __iter__(self) -> 'Iterator[TotalStat]':
         yield self._stat
 
     @property
-    def total(self):
+    def total(self) -> int:
         return self._stat.total
 
     @property
-    def passed(self):
+    def passed(self) -> int:
         return self._stat.passed
 
     @property
-    def skipped(self):
+    def skipped(self) -> int:
         return self._stat.skipped
 
     @property
-    def failed(self):
+    def failed(self) -> int:
         return self._stat.failed
 
     def add_test(self, test):
         self._stat.add_test(test)
 
     @property
-    def message(self):
+    def message(self) -> str:
         """String representation of the statistics.
 
         For example::
             2 tests, 1 passed, 1 failed
         """
         # TODO: should this message be highlighted in console
         test_or_task = 'test' if not self._rpa else 'task'
```

## Comparing `robotframework-6.1b1/src/robot/model/filter.py` & `robotframework-6.1rc1/src/robot/model/filter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/modelobject.py` & `robotframework-6.1rc1/src/robot/model/modelobject.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,111 +11,138 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import copy
 import json
-import os
-import pathlib
+from pathlib import Path
+from typing import Any, Dict, overload, TextIO, Type, TypeVar
 
-from robot.utils import SetterAwareType, type_name
+from robot.errors import DataError
+from robot.utils import get_error_message, SetterAwareType, type_name
+
+
+T = TypeVar('T', bound='ModelObject')
+DataDict = Dict[str, Any]
 
 
 class ModelObject(metaclass=SetterAwareType):
     repr_args = ()
     __slots__ = []
 
     @classmethod
-    def from_dict(cls, data):
+    def from_dict(cls: Type[T], data: DataDict) -> T:
         """Create this object based on data in a dictionary.
 
         Data can be got from the :meth:`to_dict` method or created externally.
         """
         try:
             return cls().config(**data)
-        except AttributeError as err:
-            raise ValueError(f"Creating '{full_name(cls)}' object from dictionary "
-                             f"failed: {err}")
+        except (AttributeError, TypeError) as err:
+            raise DataError(f"Creating '{full_name(cls)}' object from dictionary "
+                            f"failed: {err}")
 
     @classmethod
-    def from_json(cls, source):
+    def from_json(cls: Type[T], source: 'str|bytes|TextIO|Path') -> T:
         """Create this object based on JSON data.
 
         The data is given as the ``source`` parameter. It can be:
 
         - a string (or bytes) containing the data directly,
         - an open file object where to read the data, or
-        - a path (string or `pathlib.Path`__) to a UTF-8 encoded file to read.
-
-        __ https://docs.python.org/3/library/pathlib.html
+        - a path (``pathlib.Path`` or string) to a UTF-8 encoded file to read.
 
         The JSON data is first converted to a Python dictionary and the object
         created using the :meth:`from_dict` method.
 
         Notice that the ``source`` is considered to be JSON data if it is
         a string and contains ``{``. If you need to use ``{`` in a file system
         path, pass it in as a ``pathlib.Path`` instance.
         """
         try:
             data = JsonLoader().load(source)
-        except ValueError as err:
-            raise ValueError(f'Loading JSON data failed: {err}')
+        except (TypeError, ValueError) as err:
+            raise DataError(f'Loading JSON data failed: {err}')
         return cls.from_dict(data)
 
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         """Serialize this object into a dictionary.
 
         The object can be later restored by using the :meth:`from_dict` method.
         """
         raise NotImplementedError
 
-    def to_json(self, file=None, *, ensure_ascii=False, indent=0,
-                separators=(',', ':')):
+    @overload
+    def to_json(self, file: None = None, *, ensure_ascii: bool = False,
+                indent: int = 0, separators: 'tuple[str, str]' = (',', ':')) -> str:
+        ...
+
+    @overload
+    def to_json(self, file: 'TextIO|Path|str', *, ensure_ascii: bool = False,
+                indent: int = 0, separators: 'tuple[str, str]' = (',', ':')) -> None:
+        ...
+
+    def to_json(self, file: 'None|TextIO|Path|str' = None, *,
+                ensure_ascii: bool = False, indent: int = 0,
+                separators: 'tuple[str, str]' = (',', ':')) -> 'None|str':
         """Serialize this object into JSON.
 
         The object is first converted to a Python dictionary using the
         :meth:`to_dict` method and then the dictionary is converted to JSON.
 
         The ``file`` parameter controls what to do with the resulting JSON data.
         It can be:
 
         - ``None`` (default) to return the data as a string,
         - an open file object where to write the data, or
-        - a path to a file where to write the data using UTF-8 encoding.
+        - a path (``pathlib.Path`` or string) to a file where to write
+          the data using UTF-8 encoding.
 
         JSON formatting can be configured using optional parameters that
         are passed directly to the underlying json__ module. Notice that
         the defaults differ from what ``json`` uses.
 
         __ https://docs.python.org/3/library/json.html
         """
         return JsonDumper(ensure_ascii=ensure_ascii, indent=indent,
                           separators=separators).dump(self.to_dict(), file)
 
-    def config(self, **attributes):
+    def config(self: T, **attributes) -> T:
         """Configure model object with given attributes.
 
         ``obj.config(name='Example', doc='Something')`` is equivalent to setting
         ``obj.name = 'Example'`` and ``obj.doc = 'Something'``.
 
         New in Robot Framework 4.0.
         """
-        for name in attributes:
+        for name, value in attributes.items():
             try:
-                setattr(self, name, attributes[name])
+                orig = getattr(self, name)
+            except AttributeError:
+                raise AttributeError(f"'{full_name(self)}' object does not have "
+                                     f"attribute '{name}'")
+            # Preserve tuples. Main motivation is converting lists with `from_json`.
+            if isinstance(orig, tuple) and not isinstance(value, tuple):
+                try:
+                    value = tuple(value)
+                except TypeError:
+                    raise TypeError(f"'{full_name(self)}' object attribute '{name}' "
+                                    f"is 'tuple', got '{type_name(value)}'.")
+            try:
+                setattr(self, name, value)
             except AttributeError as err:
                 # Ignore error setting attribute if the object already has it.
-                # Avoids problems with `to/from_dict` roundtrip with body items
-                # having un-settable `type` attribute that is needed in dict data.
-                if getattr(self, name, object()) != attributes[name]:
+                # Avoids problems with `from_dict` with body items having
+                # un-settable `type` attribute that is needed in dict data.
+                if value != orig:
                     raise AttributeError(f"Setting attribute '{name}' failed: {err}")
         return self
 
-    def copy(self, **attributes):
+    def copy(self: T, **attributes) -> T:
         """Return a shallow copy of this object.
 
         :param attributes: Attributes to be set to the returned copy.
             For example, ``obj.copy(name='New name')``.
 
         See also :meth:`deepcopy`. The difference between ``copy`` and
         ``deepcopy`` is the same as with the methods having same names in
@@ -124,15 +151,15 @@
         __ https://docs.python.org/3/library/copy.html
         """
         copied = copy.copy(self)
         for name in attributes:
             setattr(copied, name, attributes[name])
         return copied
 
-    def deepcopy(self, **attributes):
+    def deepcopy(self: T, **attributes) -> T:
         """Return a deep copy of this object.
 
         :param attributes: Attributes to be set to the returned copy.
             For example, ``obj.deepcopy(name='New name')``.
 
         See also :meth:`copy`. The difference between ``deepcopy`` and
         ``copy`` is the same as with the methods having same names in
@@ -141,68 +168,79 @@
         __ https://docs.python.org/3/library/copy.html
         """
         copied = copy.deepcopy(self)
         for name in attributes:
             setattr(copied, name, attributes[name])
         return copied
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         arguments = [(name, getattr(self, name)) for name in self.repr_args]
         args_repr = ', '.join(f'{name}={value!r}' for name, value in arguments
                               if self._include_in_repr(name, value))
         return f"{full_name(self)}({args_repr})"
 
-    def _include_in_repr(self, name, value):
+    def _include_in_repr(self, name: str, value: Any) -> bool:
         return True
 
 
-def full_name(obj):
-    typ = type(obj) if not isinstance(obj, type) else obj
-    parts = typ.__module__.split('.') + [typ.__name__]
+def full_name(obj_or_cls):
+    cls = type(obj_or_cls) if not isinstance(obj_or_cls, type) else obj_or_cls
+    parts = cls.__module__.split('.') + [cls.__name__]
     if len(parts) > 1 and parts[0] == 'robot':
         parts[2:-1] = []
     return '.'.join(parts)
 
 
 class JsonLoader:
 
-    def load(self, source):
+    def load(self, source: 'str|bytes|TextIO|Path') -> DataDict:
         try:
             data = self._load(source)
-        except (json.JSONDecodeError, TypeError) as err:
-            raise ValueError(f'Invalid JSON data: {err}')
+        except (json.JSONDecodeError, TypeError):
+            raise ValueError(f'Invalid JSON data: {get_error_message()}')
         if not isinstance(data, dict):
-            raise ValueError(f"Expected dictionary, got {type_name(data)}.")
+            raise TypeError(f"Expected dictionary, got {type_name(data)}.")
         return data
 
     def _load(self, source):
         if self._is_path(source):
             with open(source, encoding='UTF-8') as file:
                 return json.load(file)
         if hasattr(source, 'read'):
             return json.load(source)
         return json.loads(source)
 
     def _is_path(self, source):
-        if isinstance(source, os.PathLike):
+        if isinstance(source, Path):
             return True
         if not isinstance(source, str) or '{' in source:
             return False
-        return os.path.isfile(source)
+        try:
+            return Path(source).is_file()
+        except OSError:    # Can happen on Windows w/ Python < 3.10.
+            return False
 
 
 class JsonDumper:
 
     def __init__(self, **config):
         self.config = config
 
-    def dump(self, data, output=None):
+    @overload
+    def dump(self, data: DataDict, output: None = None) -> str:
+        ...
+
+    @overload
+    def dump(self, data: DataDict, output: 'TextIO|Path|str') -> None:
+        ...
+
+    def dump(self, data: DataDict, output: 'None|TextIO|Path|str' = None) -> 'None|str':
         if not output:
             return json.dumps(data, **self.config)
-        elif isinstance(output, (str, pathlib.Path)):
+        elif isinstance(output, (str, Path)):
             with open(output, 'w', encoding='UTF-8') as file:
                 json.dump(data, file, **self.config)
         elif hasattr(output, 'write'):
             json.dump(data, output, **self.config)
         else:
-            raise TypeError(f"Output should be None, open file or path, "
+            raise TypeError(f"Output should be None, path or open file, "
                             f"got {type_name(output)}.")
```

## Comparing `robotframework-6.1b1/src/robot/model/configurer.py` & `robotframework-6.1rc1/src/robot/model/configurer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/statistics.py` & `robotframework-6.1rc1/src/robot/model/statistics.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/model/tagstatistics.py` & `robotframework-6.1rc1/src/robot/model/tagstatistics.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/conf/settings.py` & `robotframework-6.1rc1/src/robot/conf/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     _cli_opts = {'RPA'              : ('rpa', None),
                  'Name'             : ('name', None),
                  'Doc'              : ('doc', None),
                  'Metadata'         : ('metadata', []),
                  'TestNames'        : ('test', []),
                  'TaskNames'        : ('task', []),
                  'SuiteNames'       : ('suite', []),
+                 'ParseInclude'     : ('parseinclude', []),
                  'SetTag'           : ('settag', []),
                  'Include'          : ('include', []),
                  'Exclude'          : ('exclude', []),
                  'OutputDir'        : ('outputdir', abspath('.')),
                  'Log'              : ('log', 'log.html'),
                  'Report'           : ('report', 'report.html'),
                  'XUnit'            : ('xunit', None),
@@ -404,14 +405,18 @@
         return self._filter_empty(self['Include'])
 
     @property
     def exclude(self):
         return self._filter_empty(self['Exclude'])
 
     @property
+    def parse_include(self):
+        return self['ParseInclude']
+
+    @property
     def pythonpath(self):
         return self['PythonPath']
 
     @property
     def status_rc(self):
         return self['StatusRC']
 
@@ -448,15 +453,15 @@
 
     @rpa.setter
     def rpa(self, value):
         self['RPA'] = value
 
 
 class RobotSettings(_BaseSettings):
-    _extra_cli_opts = {'Extension'          : ('extension', ('.robot', '.rbt')),
+    _extra_cli_opts = {'Extension'          : ('extension', ('.robot', '.rbt', '.robot.rst')),
                        'Output'             : ('output', 'output.xml'),
                        'LogLevel'           : ('loglevel', 'INFO'),
                        'MaxErrorLines'      : ('maxerrorlines', 40),
                        'MaxAssignLength'    : ('maxassignlength', 200),
                        'DryRun'             : ('dryrun', False),
                        'ExitOnFailure'      : ('exitonfailure', False),
                        'ExitOnError'        : ('exitonerror', False),
@@ -480,16 +485,17 @@
                        'DebugFile'          : ('debugfile', None),
                        'Language'           : ('language', [])}
     _languages = None
 
     def get_rebot_settings(self):
         settings = RebotSettings()
         settings.start_timestamp = self.start_timestamp
-        not_copied = {'Include', 'Exclude', 'TestNames', 'SuiteNames', 'Name', 'Doc',
-                      'Metadata', 'SetTag', 'Output', 'LogLevel', 'TimestampOutputs'}
+        not_copied = {'Include', 'Exclude', 'TestNames', 'SuiteNames', 'ParseInclude',
+                      'Name', 'Doc', 'Metadata', 'SetTag', 'Output', 'LogLevel',
+                      'TimestampOutputs'}
         for opt in settings._opts:
             if opt in self and opt not in not_copied:
                 settings._opts[opt] = self[opt]
         settings._opts['ProcessEmptySuite'] = self['RunEmptySuite']
         return settings
 
     def _output_disabled(self):
```

## Comparing `robotframework-6.1b1/src/robot/conf/__init__.py` & `robotframework-6.1rc1/src/robot/conf/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/conf/languages.py` & `robotframework-6.1rc1/src/robot/conf/languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,14 +363,15 @@
     test_cases_header = 'Testovací případy'
     tasks_header = 'Úlohy'
     keywords_header = 'Klíčová slova'
     comments_header = 'Komentáře'
     library_setting = 'Knihovna'
     resource_setting = 'Zdroj'
     variables_setting = 'Proměnná'
+    name_setting = 'Název'
     documentation_setting = 'Dokumentace'
     metadata_setting = 'Metadata'
     suite_setup_setting = 'Příprava sady'
     suite_teardown_setting = 'Ukončení sady'
     test_setup_setting = 'Příprava testu'
     test_teardown_setting = 'Ukončení testu'
     test_template_setting = 'Šablona testu'
@@ -404,14 +405,15 @@
     test_cases_header = 'Testgevallen'
     tasks_header = 'Taken'
     keywords_header = 'Sleutelwoorden'
     comments_header = 'Opmerkingen'
     library_setting = 'Bibliotheek'
     resource_setting = 'Resource'
     variables_setting = 'Variabele'
+    name_setting = 'Naam'
     documentation_setting = 'Documentatie'
     metadata_setting = 'Metadata'
     suite_setup_setting = 'Suite Preconditie'
     suite_teardown_setting = 'Suite Postconditie'
     test_setup_setting = 'Test Preconditie'
     test_teardown_setting = 'Test Postconditie'
     test_template_setting = 'Test Sjabloon'
@@ -526,14 +528,15 @@
     test_cases_header = 'Unités de test'
     tasks_header = 'Tâches'
     keywords_header = 'Mots-clés'
     comments_header = 'Commentaires'
     library_setting = 'Bibliothèque'
     resource_setting = 'Ressource'
     variables_setting = 'Variable'
+    name_setting = 'Nom'
     documentation_setting = 'Documentation'
     metadata_setting = 'Méta-donnée'
     suite_setup_setting = 'Mise en place de suite'
     suite_teardown_setting = 'Démontage de suite'
     test_setup_setting = 'Mise en place de test'
     test_teardown_setting = 'Démontage de test'
     test_template_setting = 'Modèle de test'
@@ -567,14 +570,15 @@
     test_cases_header = 'Testfälle'
     tasks_header = 'Aufgaben'
     keywords_header = 'Schlüsselwörter'
     comments_header = 'Kommentare'
     library_setting = 'Bibliothek'
     resource_setting = 'Ressource'
     variables_setting = 'Variablen'
+    name_setting = 'Name'
     documentation_setting = 'Dokumentation'
     metadata_setting = 'Metadaten'
     suite_setup_setting = 'Suitevorbereitung'
     suite_teardown_setting = 'Suitenachbereitung'
     test_setup_setting = 'Testvorbereitung'
     test_teardown_setting = 'Testnachbereitung'
     test_template_setting = 'Testvorlage'
@@ -608,14 +612,15 @@
     test_cases_header = 'Casos de Teste'
     tasks_header = 'Tarefas'
     keywords_header = 'Palavras-Chave'
     comments_header = 'Comentários'
     library_setting = 'Biblioteca'
     resource_setting = 'Recurso'
     variables_setting = 'Variável'
+    name_setting = 'Nome'
     documentation_setting = 'Documentação'
     metadata_setting = 'Metadados'
     suite_setup_setting = 'Configuração da Suíte'
     suite_teardown_setting = 'Finalização de Suíte'
     test_setup_setting = 'Inicialização de Teste'
     test_teardown_setting = 'Finalização de Teste'
     test_template_setting = 'Modelo de Teste'
@@ -649,14 +654,15 @@
     test_cases_header = 'Casos de Teste'
     tasks_header = 'Tarefas'
     keywords_header = 'Palavras-Chave'
     comments_header = 'Comentários'
     library_setting = 'Biblioteca'
     resource_setting = 'Recurso'
     variables_setting = 'Variável'
+    name_setting = 'Nome'
     documentation_setting = 'Documentação'
     metadata_setting = 'Metadados'
     suite_setup_setting = 'Inicialização de Suíte'
     suite_teardown_setting = 'Finalização de Suíte'
     test_setup_setting = 'Inicialização de Teste'
     test_teardown_setting = 'Finalização de Teste'
     test_template_setting = 'Modelo de Teste'
@@ -729,15 +735,15 @@
     test_cases_header = 'Przypadki testowe'
     tasks_header = 'Zadania'
     keywords_header = 'Słowa kluczowe'
     comments_header = 'Komentarze'
     library_setting = 'Biblioteka'
     resource_setting = 'Zasób'
     variables_setting = 'Zmienne'
-    name_setting = "Nazwa"
+    name_setting = 'Nazwa'
     documentation_setting = 'Dokumentacja'
     metadata_setting = 'Metadane'
     suite_setup_setting = 'Inicjalizacja zestawu'
     suite_teardown_setting = 'Ukończenie zestawu'
     test_setup_setting = 'Inicjalizacja testu'
     test_teardown_setting = 'Ukończenie testu'
     test_template_setting = 'Szablon testu'
@@ -810,14 +816,15 @@
     test_cases_header = 'Casos de prueba'
     tasks_header = 'Tareas'
     keywords_header = 'Palabras clave'
     comments_header = 'Comentarios'
     library_setting = 'Biblioteca'
     resource_setting = 'Recursos'
     variables_setting = 'Variable'
+    name_setting = 'Nombre'
     documentation_setting = 'Documentación'
     metadata_setting = 'Metadatos'
     suite_setup_setting = 'Configuración de la Suite'
     suite_teardown_setting = 'Desmontaje de la Suite'
     test_setup_setting = 'Configuración de prueba'
     test_teardown_setting = 'Desmontaje de la prueba'
     test_template_setting = 'Plantilla de prueba'
@@ -1013,14 +1020,15 @@
     test_cases_header = 'Testfall'
     tasks_header = 'Taskar'
     keywords_header = 'Nyckelord'
     comments_header = 'Kommentarer'
     library_setting = 'Bibliotek'
     resource_setting = 'Resurs'
     variables_setting = 'Variabel'
+    name_setting = 'Namn'
     documentation_setting = 'Dokumentation'
     metadata_setting = 'Metadata'
     suite_setup_setting = 'Svit konfigurering'
     suite_teardown_setting = 'Svit nedrivning'
     test_setup_setting = 'Test konfigurering'
     test_teardown_setting = 'Test nedrivning'
     test_template_setting = 'Test mall'
@@ -1095,14 +1103,15 @@
     test_cases_header = 'Cazuri De Test'
     tasks_header = 'Sarcini'
     keywords_header = 'Cuvinte Cheie'
     comments_header = 'Comentarii'
     library_setting = 'Librarie'
     resource_setting = 'Resursa'
     variables_setting = 'Variabila'
+    name_setting = 'Nume'
     documentation_setting = 'Documentatie'
     metadata_setting = 'Metadate'
     suite_setup_setting = 'Configurare De Suita'
     suite_teardown_setting = 'Configurare De Intrerupere'
     test_setup_setting = 'Setare De Test'
     test_teardown_setting = 'Inrerupere De Test'
     test_template_setting = 'Sablon De Test'
@@ -1136,14 +1145,15 @@
     test_cases_header = 'Casi Di Test'
     tasks_header = 'Attività'
     keywords_header = 'Parole Chiave'
     comments_header = 'Commenti'
     library_setting = 'Libreria'
     resource_setting = 'Risorsa'
     variables_setting = 'Variabile'
+    name_setting = 'Nome'
     documentation_setting = 'Documentazione'
     metadata_setting = 'Metadati'
     suite_setup_setting = 'Configurazione Suite'
     suite_teardown_setting = 'Distruzione Suite'
     test_setup_setting = 'Configurazione Test'
     test_teardown_setting = 'Distruzione Test'
     test_template_setting = 'Modello Test'
```

## Comparing `robotframework-6.1b1/src/robot/conf/gatherfailed.py` & `robotframework-6.1rc1/src/robot/conf/gatherfailed.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/variables.py` & `robotframework-6.1rc1/src/robot/variables/variables.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/scopes.py` & `robotframework-6.1rc1/src/robot/variables/scopes.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/store.py` & `robotframework-6.1rc1/src/robot/variables/store.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/search.py` & `robotframework-6.1rc1/src/robot/variables/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,29 +43,29 @@
     return is_variable(string, '@')
 
 
 def is_dict_variable(string):
     return is_variable(string, '&')
 
 
-def is_assign(string, identifiers='$@&', allow_assign_mark=False):
+def is_assign(string, identifiers='$@&', allow_assign_mark=False, allow_items=False):
     match = search_variable(string, identifiers, ignore_errors=True)
-    return match.is_assign(allow_assign_mark)
+    return match.is_assign(allow_assign_mark, allow_items=allow_items)
 
 
-def is_scalar_assign(string, allow_assign_mark=False):
-    return is_assign(string, '$', allow_assign_mark)
+def is_scalar_assign(string, allow_assign_mark=False, allow_items=False):
+    return is_assign(string, '$', allow_assign_mark, allow_items)
 
 
-def is_list_assign(string, allow_assign_mark=False):
-    return is_assign(string, '@', allow_assign_mark)
+def is_list_assign(string, allow_assign_mark=False, allow_items=False):
+    return is_assign(string, '@', allow_assign_mark, allow_items)
 
 
-def is_dict_assign(string, allow_assign_mark=False):
-    return is_assign(string, '&', allow_assign_mark)
+def is_dict_assign(string, allow_assign_mark=False, allow_items=False):
+    return is_assign(string, '&', allow_assign_mark, allow_items)
 
 
 class VariableMatch:
 
     def __init__(self, string, identifier=None, base=None, items=(), start=-1, end=-1):
         self.string = string
         self.identifier = identifier
@@ -110,21 +110,22 @@
 
     def is_list_variable(self):
         return self.identifier == '@' and self.is_variable()
 
     def is_dict_variable(self):
         return self.identifier == '&' and self.is_variable()
 
-    def is_assign(self, allow_assign_mark=False, allow_nested=False):
+    def is_assign(self,
+                  allow_assign_mark=False, allow_nested=False, allow_items=False):
         if allow_assign_mark and self.string.endswith('='):
             match = search_variable(self.string[:-1].rstrip(), ignore_errors=True)
-            return match.is_assign()
+            return match.is_assign(allow_items=allow_items)
         return (self.is_variable()
                 and self.identifier in '$@&'
-                and not self.items
+                and (allow_items or not self.items)
                 and (allow_nested or not search_variable(self.base)))
 
     def is_scalar_assign(self, allow_assign_mark=False, allow_nested=False):
         return self.identifier == '$' and self.is_assign(allow_assign_mark, allow_nested)
 
     def is_list_assign(self, allow_assign_mark=False, allow_nested=False):
         return self.identifier == '@' and self.is_assign(allow_assign_mark, allow_nested)
```

## Comparing `robotframework-6.1b1/src/robot/variables/replacer.py` & `robotframework-6.1rc1/src/robot/variables/replacer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/notfound.py` & `robotframework-6.1rc1/src/robot/variables/notfound.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/finders.py` & `robotframework-6.1rc1/src/robot/variables/finders.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/__init__.py` & `robotframework-6.1rc1/src/robot/variables/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/filesetter.py` & `robotframework-6.1rc1/src/robot/variables/filesetter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/evaluation.py` & `robotframework-6.1rc1/src/robot/variables/evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,28 +67,30 @@
     return eval(expression, namespace, local_ns)
 
 
 def _decorate_variables(expression, variable_store):
     variable_started = False
     variable_found = False
     tokens = []
+    prev_toknum = None
     for toknum, tokval, _, _, _ in generate_tokens(StringIO(expression).readline):
         if variable_started:
             if toknum == token.NAME:
                 if tokval not in variable_store:
-                    variable_not_found('$%s' % tokval,
+                    variable_not_found(f'${tokval}',
                                        variable_store.as_dict(decoration=False),
                                        deco_braces=False)
                 tokval = 'RF_VAR_' + tokval
                 variable_found = True
             else:
-                tokens.append((token.ERRORTOKEN, '$'))
+                tokens.append((prev_toknum, '$'))
             variable_started = False
-        if toknum == token.ERRORTOKEN and tokval == '$':
+        if tokval == '$':
             variable_started = True
+            prev_toknum = toknum
         else:
             tokens.append((toknum, tokval))
     return untokenize(tokens).strip() if variable_found else expression
 
 
 def _import_modules(module_names):
     modules = {}
```

## Comparing `robotframework-6.1b1/src/robot/variables/tablesetter.py` & `robotframework-6.1rc1/src/robot/variables/tablesetter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/variables/resolvable.py` & `robotframework-6.1rc1/src/robot/variables/resolvable.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/writer.py` & `robotframework-6.1rc1/src/robot/libdocpkg/writer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/builder.py` & `robotframework-6.1rc1/src/robot/libdocpkg/builder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/jsonbuilder.py` & `robotframework-6.1rc1/src/robot/libdocpkg/jsonbuilder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/htmlwriter.py` & `robotframework-6.1rc1/src/robot/libdocpkg/htmlwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/output.py` & `robotframework-6.1rc1/src/robot/libdocpkg/output.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/jsonwriter.py` & `robotframework-6.1rc1/src/robot/libdocpkg/jsonwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/xmlwriter.py` & `robotframework-6.1rc1/src/robot/libdocpkg/xmlwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/standardtypes.py` & `robotframework-6.1rc1/src/robot/libdocpkg/standardtypes.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/robotbuilder.py` & `robotframework-6.1rc1/src/robot/libdocpkg/robotbuilder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/consoleviewer.py` & `robotframework-6.1rc1/src/robot/libdocpkg/consoleviewer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/datatypes.py` & `robotframework-6.1rc1/src/robot/libdocpkg/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         required_keys = list(getattr(typed_dict, '__required_keys__', []))
         optional_keys = list(getattr(typed_dict, '__optional_keys__', []))
         for key, value in typed_dict.__annotations__.items():
             typ = value.__name__ if isclass(value) else str(value)
             required = key in required_keys if required_keys or optional_keys else None
             items.append(TypedDictItem(key, typ, required))
         return cls(cls.TYPED_DICT, typed_dict.__name__, getdoc(typed_dict),
-                   accepts=(str,), items=items)
+                   accepts=(str, 'Mapping'), items=items)
 
     def to_dictionary(self, legacy=False):
         data = {
             'type': self.type,
             'name': self.name,
             'doc': self.doc,
         }
```

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/__init__.py` & `robotframework-6.1rc1/src/robot/libdocpkg/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/htmlutils.py` & `robotframework-6.1rc1/src/robot/libdocpkg/htmlutils.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/model.py` & `robotframework-6.1rc1/src/robot/libdocpkg/model.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libdocpkg/xmlbuilder.py` & `robotframework-6.1rc1/src/robot/libdocpkg/xmlbuilder.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/xunitwriter.py` & `robotframework-6.1rc1/src/robot/reporting/xunitwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/jsmodelbuilders.py` & `robotframework-6.1rc1/src/robot/reporting/jsmodelbuilders.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/jsbuildingcontext.py` & `robotframework-6.1rc1/src/robot/reporting/jsbuildingcontext.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/jswriter.py` & `robotframework-6.1rc1/src/robot/reporting/jswriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/stringcache.py` & `robotframework-6.1rc1/src/robot/reporting/stringcache.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/__init__.py` & `robotframework-6.1rc1/src/robot/reporting/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/resultwriter.py` & `robotframework-6.1rc1/src/robot/reporting/resultwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/logreportwriters.py` & `robotframework-6.1rc1/src/robot/reporting/logreportwriters.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/jsexecutionresult.py` & `robotframework-6.1rc1/src/robot/reporting/jsexecutionresult.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/reporting/outputwriter.py` & `robotframework-6.1rc1/src/robot/running/timeouts/posix.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,24 +9,32 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from robot.output.xmllogger import XmlLogger
+from signal import setitimer, signal, SIGALRM, ITIMER_REAL
 
 
-class OutputWriter(XmlLogger):
+class Timeout:
 
-    def __init__(self, output, rpa=False):
-        XmlLogger.__init__(self, output, rpa=rpa, generator='Rebot')
+    def __init__(self, timeout, error):
+        self._timeout = timeout
+        self._error = error
 
-    def start_message(self, msg):
-        self._write_message(msg)
+    def execute(self, runnable):
+        self._start_timer()
+        try:
+            return runnable()
+        finally:
+            self._stop_timer()
 
-    def close(self):
-        self._writer.end('robot')
-        self._writer.close()
+    def _start_timer(self):
+        signal(SIGALRM, self._raise_timeout_error)
+        setitimer(ITIMER_REAL, self._timeout)
 
-    def end_result(self, result):
-        self.close()
+    def _raise_timeout_error(self, signum, frame):
+        raise self._error
+
+    def _stop_timer(self):
+        setitimer(ITIMER_REAL, 0)
```

## Comparing `robotframework-6.1b1/src/robot/reporting/expandkeywordmatcher.py` & `robotframework-6.1rc1/src/robot/reporting/expandkeywordmatcher.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/context.py` & `robotframework-6.1rc1/src/robot/running/context.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/librarykeywordrunner.py` & `robotframework-6.1rc1/src/robot/running/librarykeywordrunner.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/handlers.py` & `robotframework-6.1rc1/src/robot/running/handlers.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/modelcombiner.py` & `robotframework-6.1rc1/src/robot/running/modelcombiner.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/libraryscopes.py` & `robotframework-6.1rc1/src/robot/running/libraryscopes.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/signalhandler.py` & `robotframework-6.1rc1/src/robot/running/signalhandler.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/userkeywordrunner.py` & `robotframework-6.1rc1/src/robot/running/userkeywordrunner.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/bodyrunner.py` & `robotframework-6.1rc1/src/robot/running/bodyrunner.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/usererrorhandler.py` & `robotframework-6.1rc1/src/robot/running/usererrorhandler.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/suiterunner.py` & `robotframework-6.1rc1/src/robot/running/suiterunner.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/status.py` & `robotframework-6.1rc1/src/robot/running/status.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/runkwregister.py` & `robotframework-6.1rc1/src/robot/running/runkwregister.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/testlibraries.py` & `robotframework-6.1rc1/src/robot/running/testlibraries.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/outputcapture.py` & `robotframework-6.1rc1/src/robot/running/outputcapture.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/userkeyword.py` & `robotframework-6.1rc1/src/robot/running/userkeyword.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/__init__.py` & `robotframework-6.1rc1/src/robot/running/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/randomizer.py` & `robotframework-6.1rc1/src/robot/running/randomizer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/namespace.py` & `robotframework-6.1rc1/src/robot/running/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,33 +366,33 @@
 
     def _get_runner_from_resource_files(self, name):
         handlers = [handler for res in self.resources.values()
                     for handler in res.handlers_for(name)]
         if not handlers:
             return None
         if len(handlers) > 1:
-            handlers = self._prioritize_same_file_or_public(handlers)
+            handlers = self._filter_based_on_search_order(handlers)
             if len(handlers) > 1:
-                handlers = self._select_best_matches(handlers)
+                handlers = self._prioritize_same_file_or_public(handlers)
                 if len(handlers) > 1:
-                    handlers = self._filter_based_on_search_order(handlers)
+                    handlers = self._select_best_matches(handlers)
                     if len(handlers) > 1:
                         self._raise_multiple_keywords_found(handlers, name)
         return handlers[0].create_runner(name, self.languages)
 
     def _get_runner_from_libraries(self, name):
         handlers = [handler for lib in self.libraries.values()
                     for handler in lib.handlers_for(name)]
         if not handlers:
             return None
         pre_run_message = None
         if len(handlers) > 1:
-            handlers = self._select_best_matches(handlers)
+            handlers = self._filter_based_on_search_order(handlers)
             if len(handlers) > 1:
-                handlers = self._filter_based_on_search_order(handlers)
+                handlers = self._select_best_matches(handlers)
                 if len(handlers) > 1:
                     handlers, pre_run_message = self._filter_stdlib_handler(handlers)
                     if len(handlers) > 1:
                         self._raise_multiple_keywords_found(handlers, name)
         runner = handlers[0].create_runner(name, self.languages)
         if pre_run_message:
             runner.pre_run_messages += (pre_run_message,)
```

## Comparing `robotframework-6.1b1/src/robot/running/statusreporter.py` & `robotframework-6.1rc1/src/robot/running/statusreporter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/handlerstore.py` & `robotframework-6.1rc1/src/robot/running/handlerstore.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/dynamicmethods.py` & `robotframework-6.1rc1/src/robot/running/dynamicmethods.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/model.py` & `robotframework-6.1rc1/src/robot/running/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,377 +30,400 @@
 The :class:`TestSuite` class is exposed via the :mod:`robot.api` package. If other
 classes are needed, they can be imported from :mod:`robot.running`.
 
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#programmatic-modification-of-results
 __ http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#listener-interface
 """
 
+import sys
 import warnings
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import Any, Mapping, Sequence, TYPE_CHECKING, Union
+if sys.version_info >= (3, 8):
+    from typing import Literal
 
 from robot import model
 from robot.conf import RobotSettings
 from robot.errors import BreakLoop, ContinueLoop, DataError, ReturnFromKeyword
-from robot.model import BodyItem, create_fixture, Keywords, ModelObject
+from robot.model import (BodyItem, create_fixture, DataDict, Keywords, ModelObject,
+                         TestCases, TestSuites)
 from robot.output import LOGGER, Output, pyloggingconf
 from robot.result import (Break as BreakResult, Continue as ContinueResult,
                           Error as ErrorResult, Return as ReturnResult)
 from robot.utils import setter
 
 from .bodyrunner import ForRunner, IfRunner, KeywordRunner, TryRunner, WhileRunner
 from .randomizer import Randomizer
 from .statusreporter import StatusReporter
 
 if TYPE_CHECKING:
     from robot.parsing import File
     from .builder import TestDefaults
 
 
-class Body(model.Body):
+BodyItemParent = Union['TestSuite', 'TestCase', 'UserKeyword', 'For', 'If', 'IfBranch',
+                       'Try', 'TryBranch', 'While', None]
+
+
+class Body(model.BaseBody['Keyword', 'For', 'While', 'If', 'Try', 'Return', 'Continue',
+                          'Break', 'model.Message', 'Error']):
     __slots__ = []
 
 
+class WithSource:
+    __slots__ = ()
+    parent: BodyItemParent
+
+    @property
+    def source(self) -> 'Path|None':
+        return self.parent.source if self.parent is not None else None
+
+
 @Body.register
-class Keyword(model.Keyword):
+class Keyword(model.Keyword, WithSource):
     """Represents an executable keyword call.
 
     A keyword call consists only of a keyword name, arguments and possible
     assignment in the data::
 
         Keyword    arg
         ${result} =    Another Keyword    arg1    arg2
 
     The actual keyword that is executed depends on the context where this model
     is executed.
     """
     __slots__ = ['lineno']
 
-    def __init__(self, name='', args=(), assign=(), type=BodyItem.KEYWORD, parent=None,
-                 lineno=None):
+    def __init__(self, name: str = '',
+                 args: Sequence[str] = (),
+                 assign: Sequence[str] = (),
+                 type: str = BodyItem.KEYWORD,
+                 parent: BodyItemParent = None,
+                 lineno: 'int|None' = None):
         super().__init__(name, args, assign, type, parent)
         self.lineno = lineno
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         return data
 
     def run(self, context, run=True, templated=None):
         return KeywordRunner(context, run).run(self)
 
 
 @Body.register
-class For(model.For):
+class For(model.For, WithSource):
     __slots__ = ['lineno', 'error']
     body_class = Body
 
-    def __init__(self, variables=(), flavor='IN', values=(), start=None, mode=None,
-                 fill=None, parent=None, lineno=None, error=None):
+    def __init__(self, variables: Sequence[str] = (),
+                 flavor: "Literal['IN', 'IN RANGE', 'IN ENUMERATE', 'IN ZIP']" = 'IN',
+                 values: Sequence[str] = (),
+                 start: 'str|None' = None,
+                 mode: 'str|None' = None,
+                 fill: 'str|None' = None,
+                 parent: BodyItemParent = None,
+                 lineno: 'int|None' = None,
+                 error: 'str|None' = None):
         super().__init__(variables, flavor, values, start, mode, fill, parent)
         self.lineno = lineno
         self.error = error
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         if self.error:
             data['error'] = self.error
         return data
 
     def run(self, context, run=True, templated=False):
         return ForRunner(context, self.flavor, run, templated).run(self)
 
 
 @Body.register
-class While(model.While):
+class While(model.While, WithSource):
     __slots__ = ['lineno', 'error']
     body_class = Body
 
-    def __init__(self, condition=None, limit=None, on_limit_message=None,
-                 parent=None, lineno=None, error=None):
-        super().__init__(condition, limit, on_limit_message, parent)
+    def __init__(self, condition: 'str|None' = None,
+                 limit: 'str|None' = None,
+                 on_limit: 'str|None' = None,
+                 on_limit_message: 'str|None' = None,
+                 parent: BodyItemParent = None,
+                 lineno: 'int|None' = None,
+                 error: 'str|None' = None):
+        super().__init__(condition, limit, on_limit, on_limit_message, parent)
         self.lineno = lineno
         self.error = error
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         if self.error:
             data['error'] = self.error
         return data
 
     def run(self, context, run=True, templated=False):
         return WhileRunner(context, run, templated).run(self)
 
 
-class IfBranch(model.IfBranch):
+class IfBranch(model.IfBranch, WithSource):
     __slots__ = ['lineno']
     body_class = Body
 
-    def __init__(self, type=BodyItem.IF, condition=None, parent=None, lineno=None):
+    def __init__(self, type: str = BodyItem.IF,
+                 condition: 'str|None' = None,
+                 parent: BodyItemParent = None,
+                 lineno: 'int|None' = None):
         super().__init__(type, condition, parent)
         self.lineno = lineno
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         return data
 
 
 @Body.register
-class If(model.If):
+class If(model.If, WithSource):
     __slots__ = ['lineno', 'error']
     branch_class = IfBranch
 
-    def __init__(self, parent=None, lineno=None, error=None):
+    def __init__(self, parent: BodyItemParent = None,
+                 lineno: 'int|None' = None,
+                 error: 'str|None' = None):
         super().__init__(parent)
         self.lineno = lineno
         self.error = error
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
     def run(self, context, run=True, templated=False):
         return IfRunner(context, run, templated).run(self)
 
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         if self.error:
             data['error'] = self.error
         return data
 
 
-class TryBranch(model.TryBranch):
+class TryBranch(model.TryBranch, WithSource):
     __slots__ = ['lineno']
     body_class = Body
 
-    def __init__(self, type=BodyItem.TRY, patterns=(), pattern_type=None,
-                 variable=None, parent=None, lineno=None):
+    def __init__(self, type: str = BodyItem.TRY,
+                 patterns: Sequence[str] = (),
+                 pattern_type: 'str|None' = None,
+                 variable: 'str|None' = None,
+                 parent: BodyItemParent = None,
+                 lineno: 'int|None' = None):
         super().__init__(type, patterns, pattern_type, variable, parent)
         self.lineno = lineno
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         return data
 
 
 @Body.register
-class Try(model.Try):
+class Try(model.Try, WithSource):
     __slots__ = ['lineno', 'error']
     branch_class = TryBranch
 
-    def __init__(self, parent=None, lineno=None, error=None):
+    def __init__(self, parent: BodyItemParent = None,
+                 lineno: 'int|None' = None,
+                 error: 'str|None' = None):
         super().__init__(parent)
         self.lineno = lineno
         self.error = error
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
     def run(self, context, run=True, templated=False):
         return TryRunner(context, run, templated).run(self)
 
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         if self.error:
             data['error'] = self.error
         return data
 
 
 @Body.register
-class Return(model.Return):
+class Return(model.Return, WithSource):
     __slots__ = ['lineno', 'error']
 
-    def __init__(self, values=(), parent=None, lineno=None, error=None):
+    def __init__(self, values: Sequence[str] = (),
+                 parent: BodyItemParent = None,
+                 lineno: 'int|None' = None,
+                 error: 'str|None' = None):
         super().__init__(values, parent)
         self.lineno = lineno
         self.error = error
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
     def run(self, context, run=True, templated=False):
         with StatusReporter(self, ReturnResult(self.values), context, run):
             if run:
                 if self.error:
                     raise DataError(self.error, syntax=True)
                 if not context.dry_run:
                     raise ReturnFromKeyword(self.values)
 
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         if self.error:
             data['error'] = self.error
         return data
 
 
 @Body.register
-class Continue(model.Continue):
+class Continue(model.Continue, WithSource):
     __slots__ = ['lineno', 'error']
 
-    def __init__(self, parent=None, lineno=None, error=None):
+    def __init__(self, parent: BodyItemParent = None,
+                 lineno: 'int|None' = None,
+                 error: 'str|None' = None):
         super().__init__(parent)
         self.lineno = lineno
         self.error = error
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
     def run(self, context, run=True, templated=False):
         with StatusReporter(self, ContinueResult(), context, run):
             if run:
                 if self.error:
                     raise DataError(self.error, syntax=True)
                 if not context.dry_run:
                     raise ContinueLoop()
 
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         if self.error:
             data['error'] = self.error
         return data
 
 
 @Body.register
-class Break(model.Break):
+class Break(model.Break, WithSource):
     __slots__ = ['lineno', 'error']
 
-    def __init__(self, parent=None, lineno=None, error=None):
+    def __init__(self, parent: BodyItemParent = None,
+                 lineno: 'int|None' = None,
+                 error: 'str|None' = None):
         super().__init__(parent)
         self.lineno = lineno
         self.error = error
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
     def run(self, context, run=True, templated=False):
         with StatusReporter(self, BreakResult(), context, run):
             if run:
                 if self.error:
                     raise DataError(self.error, syntax=True)
                 if not context.dry_run:
                     raise BreakLoop()
 
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         if self.error:
             data['error'] = self.error
         return data
 
 
 @Body.register
-class Error(model.Error):
+class Error(model.Error, WithSource):
     __slots__ = ['lineno', 'error']
 
-    def __init__(self, values=(), parent=None, lineno=None, error=None):
+    def __init__(self, values: Sequence[str] = (),
+                 parent: BodyItemParent = None,
+                 lineno: 'int|None' = None,
+                 error: str = ''):
         super().__init__(values, parent)
         self.lineno = lineno
         self.error = error
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
     def run(self, context, run=True, templated=False):
         with StatusReporter(self, ErrorResult(self.values), context, run):
             if run:
                 raise DataError(self.error)
 
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.lineno:
             data['lineno'] = self.lineno
         if self.error:
             data['error'] = self.error
         return data
 
 
-class TestCase(model.TestCase):
+class TestCase(model.TestCase[Keyword]):
     """Represents a single executable test case.
 
     See the base class for documentation of attributes not documented here.
     """
     __slots__ = ['template', 'error']
     body_class = Body        #: Internal usage only.
     fixture_class = Keyword  #: Internal usage only.
 
-    def __init__(self, name='', doc='', tags=None, timeout=None, template=None,
-                 lineno=None, error=None):
-        super().__init__(name, doc, tags, timeout, lineno)
+    def __init__(self, name: str = '',
+                 doc: str = '',
+                 tags: Sequence[str] = (),
+                 timeout: 'str|None' = None,
+                 lineno: 'int|None' = None,
+                 parent: 'TestSuite|None' = None,
+                 template: 'str|None' = None,
+                 error: 'str|None' = None):
+        super().__init__(name, doc, tags, timeout, lineno, parent)
         #: Name of the keyword that has been used as a template when building the test.
         # ``None`` if template is not used.
         self.template = template
         self.error = error
 
-    @property
-    def source(self):
-        return self.parent.source if self.parent is not None else None
-
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         if self.template:
             data['template'] = self.template
         if self.error:
             data['error'] = self.error
         return data
 
+    @setter
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
+        """Test body as a :class:`~robot.running.Body` object."""
+        return self.body_class(self, body)
+
 
-class TestSuite(model.TestSuite):
+class TestSuite(model.TestSuite[Keyword, TestCase]):
     """Represents a single executable test suite.
 
     See the base class for documentation of attributes not documented here.
     """
     __slots__ = []
     test_class = TestCase    #: Internal usage only.
     fixture_class = Keyword  #: Internal usage only.
 
-    def __init__(self,  name='', doc='', metadata=None, source=None, rpa=None):
-        super().__init__(name, doc, metadata, source, rpa)
+    def __init__(self, name: str = '',
+                 doc: str = '',
+                 metadata: 'Mapping[str, str]|None' = None,
+                 source: 'Path|str|None' = None,
+                 rpa: 'bool|None' = None,
+                 parent: 'TestSuite|None' = None):
+        super().__init__(name, doc, metadata, source, rpa, parent)
         #: :class:`ResourceFile` instance containing imports, variables and
         #: keywords the suite owns. When data is parsed from the file system,
         #: this data comes from the same test case file that creates the suite.
         self.resource = ResourceFile(parent=self)
 
     @setter
     def resource(self, resource: 'ResourceFile|dict') -> 'ResourceFile':
@@ -472,16 +495,16 @@
         New in Robot Framework 6.1. See also :meth:`from_model` and
         :meth:`from_file_system`.
         """
         from robot.parsing import get_model
         model = get_model(string, data_only=True, **config)
         return cls.from_model(model, defaults=defaults)
 
-    def configure(self, randomize_suites=False, randomize_tests=False,
-                  randomize_seed=None, **options):
+    def configure(self, randomize_suites: bool = False, randomize_tests: bool = False,
+                  randomize_seed: 'int|None' = None, **options):
         """A shortcut to configure a suite using one method call.
 
         Can only be used with the root test suite.
 
         :param randomize_xxx: Passed to :meth:`randomize`.
         :param options: Passed to
             :class:`~robot.model.configurer.SuiteConfigurer` that will then
@@ -492,27 +515,32 @@
             suite.configure(included_tags=['smoke'],
                             doc='Smoke test results.')
 
         Not to be confused with :meth:`config` method that suites, tests,
         and keywords have to make it possible to set multiple attributes in
         one call.
         """
-        model.TestSuite.configure(self, **options)
+        super().configure(**options)
         self.randomize(randomize_suites, randomize_tests, randomize_seed)
 
-    def randomize(self, suites=True, tests=True, seed=None):
+    def randomize(self, suites: bool = True, tests: bool = True,
+                  seed: 'int|None' = None):
         """Randomizes the order of suites and/or tests, recursively.
 
         :param suites: Boolean controlling should suites be randomized.
         :param tests: Boolean controlling should tests be randomized.
         :param seed: Random seed. Can be given if previous random order needs
             to be re-created. Seed value is always shown in logs and reports.
         """
         self.visit(Randomizer(suites, tests, seed))
 
+    @setter
+    def suites(self, suites: 'Sequence[TestSuite|DataDict]') -> TestSuites['TestSuite']:
+        return TestSuites['TestSuite'](self.__class__, self, suites)
+
     def run(self, settings=None, **options):
         """Executes the suite based on the given ``settings`` or ``options``.
 
         :param settings: :class:`~robot.conf.settings.RobotSettings` object
             to configure test execution.
         :param options: Used to construct new
             :class:`~robot.conf.settings.RobotSettings` object if ``settings``
@@ -576,95 +604,97 @@
                     IMPORTER.reset()
                     output = Output(settings)
                     runner = SuiteRunner(output, settings)
                     self.visit(runner)
                 output.close(runner.result)
         return runner.result
 
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = super().to_dict()
         data['resource'] = self.resource.to_dict()
         return data
 
 
 class Variable(ModelObject):
     repr_args = ('name', 'value')
 
-    def __init__(self, name, value=(), parent=None, lineno=None, error=None):
+    def __init__(self, name: str = '',
+                 value: Sequence[str] = (),
+                 parent: 'ResourceFile|None' = None,
+                 lineno: 'int|None' = None,
+                 error: 'str|None' = None):
         self.name = name
-        self.value = value
+        self.value = tuple(value)
         self.parent = parent
         self.lineno = lineno
         self.error = error
 
     @property
-    def source(self):
+    def source(self) -> 'Path|None':
         return self.parent.source if self.parent is not None else None
 
-    def report_invalid_syntax(self, message, level='ERROR'):
+    def report_invalid_syntax(self, message: str, level: str = 'ERROR'):
         source = self.source or '<unknown>'
         line = f' on line {self.lineno}' if self.lineno else ''
         LOGGER.write(f"Error in file '{source}'{line}: "
                      f"Setting variable '{self.name}' failed: {message}", level)
 
-    @classmethod
-    def from_dict(cls, data):
-        return cls(**data)
-
-    def to_dict(self):
-        data = {'name': self.name, 'value': list(self.value)}
+    def to_dict(self) -> DataDict:
+        data = {'name': self.name, 'value': self.value}
         if self.lineno:
             data['lineno'] = self.lineno
         if self.error:
             data['error'] = self.error
         return data
 
 
 class ResourceFile(ModelObject):
     repr_args = ('source',)
     __slots__ = ('_source', 'parent', 'doc')
 
-    def __init__(self, source=None, parent=None, doc=''):
-        self._source = source
+    def __init__(self, source: 'Path|str|None' = None,
+                 parent: 'TestSuite|None' = None,
+                 doc: str = ''):
+        self.source = source
         self.parent = parent
         self.doc = doc
         self.imports = []
         self.variables = []
         self.keywords = []
 
     @property
-    def source(self):
+    def source(self) -> 'Path|None':
         if self._source:
             return self._source
         if self.parent:
             return self.parent.source
         return None
 
     @source.setter
-    def source(self, source):
-        if not isinstance(source, (Path, type(None))):
+    def source(self, source: 'Path|str|None'):
+        if isinstance(source, str):
             source = Path(source)
         self._source = source
 
     @setter
-    def imports(self, imports):
+    def imports(self, imports: Sequence['Import']) -> 'Imports':
         return Imports(self, imports)
 
     @setter
-    def variables(self, variables):
-        return model.ItemList(Variable, {'parent': self}, items=variables)
+    def variables(self, variables: Sequence['Variable']) -> 'Variables':
+        return Variables(self, variables)
 
     @setter
-    def keywords(self, keywords):
-        return model.ItemList(UserKeyword, {'parent': self}, items=keywords)
+    def keywords(self, keywords: Sequence['UserKeyword']) -> 'UserKeywords':
+        return UserKeywords(self, keywords)
 
-    def to_dict(self):
+    def to_dict(self) -> DataDict:
         data = {}
         if self._source:
-            data['source'] = str(self.source)
+            data['source'] = str(self._source)
         if self.doc:
             data['doc'] = self.doc
         if self.imports:
             data['imports'] = self.imports.to_dicts()
         if self.variables:
             data['variables'] = self.variables.to_dicts()
         if self.keywords:
@@ -674,181 +704,201 @@
 
 class UserKeyword(ModelObject):
     repr_args = ('name', 'args')
     fixture_class = Keyword
     __slots__ = ['name', 'args', 'doc', 'return_', 'timeout', 'lineno', 'parent',
                  'error', '_teardown']
 
-    def __init__(self, name='', args=(), doc='', tags=(), return_=None,
-                 timeout=None, lineno=None, parent=None, error=None):
+    def __init__(self, name: str = '',
+                 args: Sequence[str] = (),
+                 doc: str = '',
+                 tags: Sequence[str] = (),
+                 return_: Sequence[str] = (),
+                 timeout: 'str|None' = None,
+                 lineno: 'int|None' = None,
+                 parent: 'ResourceFile|None' = None,
+                 error: 'str|None' = None):
         self.name = name
-        self.args = args
+        self.args = tuple(args)
         self.doc = doc
         self.tags = tags
-        self.return_ = return_ or ()
+        self.return_ = tuple(return_)
         self.timeout = timeout
         self.lineno = lineno
         self.parent = parent
         self.error = error
-        self.body = None
+        self.body = []
         self._teardown = None
 
     @setter
-    def body(self, body):
-        """Child keywords as a :class:`~.Body` object."""
+    def body(self, body: 'Sequence[BodyItem|DataDict]') -> Body:
         return Body(self, body)
 
     @property
-    def keywords(self):
+    def keywords(self) -> Keywords:
         """Deprecated since Robot Framework 4.0.
 
         Use :attr:`body` or :attr:`teardown` instead.
         """
         kws = list(self.body)
         if self.teardown:
             kws.append(self.teardown)
         return Keywords(self, kws)
 
     @keywords.setter
     def keywords(self, keywords):
         Keywords.raise_deprecation_error()
 
     @property
-    def teardown(self):
+    def teardown(self) -> Keyword:
         if self._teardown is None:
-            self._teardown = create_fixture(None, self, Keyword.TEARDOWN)
+            self._teardown = create_fixture(self.fixture_class, None, self, Keyword.TEARDOWN)
         return self._teardown
 
     @teardown.setter
-    def teardown(self, teardown):
-        self._teardown = create_fixture(teardown, self, Keyword.TEARDOWN)
+    def teardown(self, teardown: 'Keyword|DataDict|None'):
+        self._teardown = create_fixture(self.fixture_class, teardown, self, Keyword.TEARDOWN)
 
     @property
-    def has_teardown(self):
+    def has_teardown(self) -> bool:
         """Check does a keyword have a teardown without creating a teardown object.
 
         A difference between using ``if uk.has_teardown:`` and ``if uk.teardown:``
         is that accessing the :attr:`teardown` attribute creates a :class:`Keyword`
         object representing the teardown even when the user keyword actually does
         not have one. This can have an effect on memory usage.
 
         New in Robot Framework 6.1.
         """
         return bool(self._teardown)
 
     @setter
-    def tags(self, tags):
+    def tags(self, tags: Sequence[str]) -> model.Tags:
         return model.Tags(tags)
 
     @property
-    def source(self):
+    def source(self) -> 'Path|None':
         return self.parent.source if self.parent is not None else None
 
-    def to_dict(self):
-        data = {'name': self.name}
-        if self.args:
-            data['args'] = list(self.args)
-        if self.doc:
-            data['doc'] = self.doc
-        if self.tags:
-            data['tags'] = list(self.tags)
-        if self.return_:
-            data['return_'] = self.return_
-        if self.timeout:
-            data['timeout'] = self.timeout
-        if self.lineno:
-            data['lineno'] = self.lineno
-        if self.error:
-            data['error'] = self.error
+    def to_dict(self) -> DataDict:
+        data: DataDict = {'name': self.name}
+        for name, value in [('args', self.args),
+                            ('doc', self.doc),
+                            ('tags', tuple(self.tags)),
+                            ('return_', self.return_),
+                            ('timeout', self.timeout),
+                            ('lineno', self.lineno),
+                            ('error', self.error)]:
+            if value:
+                data[name] = value
         data['body'] = self.body.to_dicts()
         if self.has_teardown:
             data['teardown'] = self.teardown.to_dict()
         return data
 
 
 class Import(ModelObject):
     repr_args = ('type', 'name', 'args', 'alias')
     LIBRARY = 'LIBRARY'
     RESOURCE = 'RESOURCE'
     VARIABLES = 'VARIABLES'
 
-    def __init__(self, type, name, args=(), alias=None, parent=None, lineno=None):
+    def __init__(self, type: "Literal['LIBRARY', 'RESOURCE', 'VARIABLES']",
+                 name: str,
+                 args: Sequence[str] = (),
+                 alias: 'str|None' = None,
+                 parent: 'ResourceFile|None' = None,
+                 lineno: 'int|None' = None):
         if type not in (self.LIBRARY, self.RESOURCE, self.VARIABLES):
             raise ValueError(f"Invalid import type: Expected '{self.LIBRARY}', "
                              f"'{self.RESOURCE}' or '{self.VARIABLES}', got '{type}'.")
         self.type = type
         self.name = name
-        self.args = args
+        self.args = tuple(args)
         self.alias = alias
         self.parent = parent
         self.lineno = lineno
 
     @property
-    def source(self) -> Path:
+    def source(self) -> 'Path|None':
         return self.parent.source if self.parent is not None else None
 
     @property
-    def directory(self) -> Path:
+    def directory(self) -> 'Path|None':
         source = self.source
         return source.parent if source and not source.is_dir() else source
 
     @property
-    def setting_name(self):
+    def setting_name(self) -> str:
         return self.type.title()
 
-    def select(self, library, resource, variables):
+    def select(self, library: Any, resource: Any, variables: Any) -> Any:
         return {self.LIBRARY: library,
                 self.RESOURCE: resource,
                 self.VARIABLES: variables}[self.type]
 
-    def report_invalid_syntax(self, message, level='ERROR'):
+    def report_invalid_syntax(self, message: str, level: str = 'ERROR'):
         source = self.source or '<unknown>'
         line = f' on line {self.lineno}' if self.lineno else ''
         LOGGER.write(f"Error in file '{source}'{line}: {message}", level)
 
     @classmethod
-    def from_dict(cls, data):
+    def from_dict(cls, data) -> 'Import':
         return cls(**data)
 
-    def to_dict(self):
-        data = {'type': self.type, 'name': self.name}
+    def to_dict(self) -> DataDict:
+        data: DataDict = {'type': self.type, 'name': self.name}
         if self.args:
-            data['args'] = list(self.args)
+            data['args'] = self.args
         if self.alias:
             data['alias'] = self.alias
         if self.lineno:
             data['lineno'] = self.lineno
         return data
 
-    def _include_in_repr(self, name, value):
+    def _include_in_repr(self, name: str, value: Any) -> bool:
         return name in ('type', 'name') or value
 
 
 class Imports(model.ItemList):
 
-    def __init__(self, parent, imports=None):
+    def __init__(self, parent: ResourceFile, imports: Sequence[Import] = ()):
         super().__init__(Import, {'parent': parent}, items=imports)
 
-    def library(self, name, args=(), alias=None, lineno=None):
+    def library(self, name: str, args: Sequence[str] = (), alias: 'str|None' = None,
+                lineno: 'int|None' = None) -> Import:
         """Create library import."""
-        self.create(Import.LIBRARY, name, args, alias, lineno=lineno)
+        return self.create(Import.LIBRARY, name, args, alias, lineno=lineno)
 
-    def resource(self, name, lineno=None):
+    def resource(self, name: str, lineno: 'int|None' = None) -> Import:
         """Create resource import."""
-        self.create(Import.RESOURCE, name, lineno=lineno)
+        return self.create(Import.RESOURCE, name, lineno=lineno)
 
-    def variables(self, name, args=(), lineno=None):
+    def variables(self, name: str, args: Sequence[str] = (),
+                  lineno: 'int|None' = None) -> Import:
         """Create variables import."""
-        self.create(Import.VARIABLES, name, args, lineno=lineno)
+        return self.create(Import.VARIABLES, name, args, lineno=lineno)
 
-    def create(self, *args, **kwargs):
+    def create(self, *args, **kwargs) -> Import:
         """Generic method for creating imports.
 
         Import type specific methods :meth:`library`, :meth:`resource` and
         :meth:`variables` are recommended over this method.
         """
         # RF 6.1 changed types to upper case. Code below adds backwards compatibility.
         if args:
             args = (args[0].upper(),) + args[1:]
         elif 'type' in kwargs:
             kwargs['type'] = kwargs['type'].upper()
         return super().create(*args, **kwargs)
+
+
+class Variables(model.ItemList[Variable]):
+
+    def __init__(self, parent: ResourceFile, variables: Sequence[Variable] = ()):
+        super().__init__(Variable, {'parent': parent}, items=variables)
+
+
+class UserKeywords(model.ItemList[UserKeyword]):
+
+    def __init__(self, parent: ResourceFile, keywords: Sequence[UserKeyword] = ()):
+        super().__init__(UserKeyword, {'parent': parent}, items=keywords)
```

## Comparing `robotframework-6.1b1/src/robot/running/importer.py` & `robotframework-6.1rc1/src/robot/running/importer.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from robot.utils import normpath, seq2str, seq2str2, is_string
 
 from .builder import ResourceFileBuilder
 from .handlerstore import HandlerStore
 from .testlibraries import TestLibrary
 
 
-RESOURCE_EXTENSIONS = ('.resource', '.robot', '.txt', '.tsv', '.rst', '.rest')
+RESOURCE_EXTENSIONS = {'.resource', '.robot', '.txt', '.tsv', '.rst', '.rest',
+                       '.json', '.rsrc'}
 
 
 class Importer:
 
     def __init__(self):
         self._library_cache = ImportCache()
         self._resource_cache = ImportCache()
@@ -45,54 +46,53 @@
     def import_library(self, name, args, alias, variables):
         lib = TestLibrary(name, args, variables, create_handlers=False)
         positional, named = lib.positional_args, lib.named_args
         lib = self._import_library(name, positional, named, lib)
         if alias:
             alias = variables.replace_scalar(alias)
             lib = self._copy_library(lib, alias)
-            LOGGER.info("Imported library '%s' with name '%s'" % (name, alias))
+            LOGGER.info(f"Imported library '{name}' with name '{alias}'.")
         return lib
 
     def import_resource(self, path, lang=None):
         self._validate_resource_extension(path)
         if path in self._resource_cache:
-            LOGGER.info("Found resource file '%s' from cache" % path)
+            LOGGER.info(f"Found resource file '{path}' from cache.")
         else:
             resource = ResourceFileBuilder(lang=lang).build(path)
             self._resource_cache[path] = resource
         return self._resource_cache[path]
 
     def _validate_resource_extension(self, path):
         extension = os.path.splitext(path)[1]
         if extension.lower() not in RESOURCE_EXTENSIONS:
-            raise DataError("Invalid resource file extension '%s'. "
-                            "Supported extensions are %s."
-                            % (extension, seq2str(RESOURCE_EXTENSIONS)))
+            extensions = seq2str(sorted(RESOURCE_EXTENSIONS))
+            raise DataError(f"Invalid resource file extension '{extension}'. "
+                            f"Supported extensions are {extensions}.")
 
     def _import_library(self, name, positional, named, lib):
-        args = positional + ['%s=%s' % arg for arg in named]
+        args = positional + [f'{name}={value}' for name, value in named]
         key = (name, positional, named)
         if key in self._library_cache:
-            LOGGER.info("Found library '%s' with arguments %s from cache."
-                        % (name, seq2str2(args)))
+            LOGGER.info(f"Found library '{name}' with arguments {seq2str2(args)} "
+                        f"from cache.")
             return self._library_cache[key]
         lib.create_handlers()
         self._library_cache[key] = lib
         self._log_imported_library(name, args, lib)
         return lib
 
     def _log_imported_library(self, name, args, lib):
         type = lib.__class__.__name__.replace('Library', '').lower()[1:]
         listener = ', with listener' if lib.has_listener else ''
-        LOGGER.info("Imported library '%s' with arguments %s "
-                    "(version %s, %s type, %s scope, %d keywords%s)"
-                    % (name, seq2str2(args), lib.version or '<unknown>',
-                       type, lib.scope, len(lib), listener))
+        LOGGER.info(f"Imported library '{name}' with arguments {seq2str2(args)} "
+                    f"(version {lib.version or '<unknown>'}, {type} type, "
+                    f"{lib.scope} scope, {len(lib)} keywords{listener}).")
         if not lib:
-            LOGGER.warn("Imported library '%s' contains no keywords." % name)
+            LOGGER.warn(f"Imported library '{name}' contains no keywords.")
 
     def _copy_library(self, orig, name):
         # This is pretty ugly. Hopefully we can remove cache and copying
         # altogether in 3.0 and always just re-import libraries:
         # https://github.com/robotframework/robotframework/issues/2106
         lib = copy.copy(orig)
         lib.name = name
```

## Comparing `robotframework-6.1b1/src/robot/running/timeouts/__init__.py` & `robotframework-6.1rc1/src/robot/running/timeouts/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/timeouts/windows.py` & `robotframework-6.1rc1/src/robot/running/timeouts/windows.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/builder/parsers.py` & `robotframework-6.1rc1/src/robot/running/builder/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,25 @@
         raise DataError(f"'{self.name}' does not support parsing initialization files.")
 
     def parse_resource_file(self, source: Path) -> ResourceFile:
         raise DataError(f"'{self.name}' does not support parsing resource files.")
 
 
 class RobotParser(Parser):
+    extensions = ()
 
     def __init__(self, lang: LanguagesLike = None, process_curdir: bool = True):
         self.lang = lang
         self.process_curdir = process_curdir
 
     def parse_suite_file(self, source: Path, defaults: TestDefaults) -> TestSuite:
         model = get_model(self._get_source(source), data_only=True,
                           curdir=self._get_curdir(source), lang=self.lang)
-        suite = TestSuite(name=TestSuite.name_from_source(source), source=source)
+        suite = TestSuite(name=TestSuite.name_from_source(source, self.extensions),
+                          source=source)
         SuiteBuilder(suite, FileSettings(defaults)).build(model)
         return suite
 
     def parse_init_file(self, source: Path, defaults: TestDefaults) -> TestSuite:
         model = get_init_model(self._get_source(source), data_only=True,
                                curdir=self._get_curdir(source), lang=self.lang)
         directory = source.parent
@@ -81,31 +83,34 @@
                                    curdir=self._get_curdir(source), lang=self.lang)
         resource = ResourceFile(source=source)
         ResourceBuilder(resource).build(model)
         return resource
 
 
 class RestParser(RobotParser):
+    extensions = ('.robot.rst', '.rst', '.rest')
 
     def _get_source(self, source: Path) -> str:
         with FileReader(source) as reader:
             return read_rest_data(reader)
 
 
 class JsonParser(Parser):
 
     def parse_suite_file(self, source: Path, defaults: TestDefaults) -> TestSuite:
         return TestSuite.from_json(source)
 
     def parse_init_file(self, source: Path, defaults: TestDefaults) -> TestSuite:
         return TestSuite.from_json(source)
 
-    # FIXME: Resource imports don't otherwise support JSON yet!
     def parse_resource_file(self, source: Path) -> ResourceFile:
-        return ResourceFile.from_json(source)
+        try:
+            return ResourceFile.from_json(source)
+        except DataError as err:
+            raise DataError(f"Parsing JSON resource file '{source}' failed: {err}")
 
 
 class NoInitFileDirectoryParser(Parser):
 
     def parse_init_file(self, source: Path, defaults: TestDefaults) -> TestSuite:
         return TestSuite(name=TestSuite.name_from_source(source), source=source)
```

## Comparing `robotframework-6.1b1/src/robot/running/builder/transformers.py` & `robotframework-6.1rc1/src/robot/running/builder/transformers.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/builder/settings.py` & `robotframework-6.1rc1/src/robot/running/builder/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,25 @@
 from ..model import TestCase
 
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 
 
-    class FixtureDict(TypedDict):
+    class OptionalItems(TypedDict, total=False):
+        args: 'Sequence[str]'
+        lineno: int
+
+
+    class FixtureDict(OptionalItems):
         """Dictionary containing setup or teardown info.
 
         :attr:`args` and :attr:`lineno` are optional.
         """
         name: str
-        args: 'Sequence[str]'
-        lineno: int
 
 else:
     class FixtureDict(dict):
         pass
 
 
 class TestDefaults:
```

## Comparing `robotframework-6.1b1/src/robot/running/builder/__init__.py` & `robotframework-6.1rc1/src/robot/running/builder/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/argumentmapper.py` & `robotframework-6.1rc1/src/robot/running/arguments/argumentmapper.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/argumentconverter.py` & `robotframework-6.1rc1/src/robot/running/arguments/argumentconverter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/argumentresolver.py` & `robotframework-6.1rc1/src/robot/running/arguments/argumentresolver.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/embedded.py` & `robotframework-6.1rc1/src/robot/running/arguments/embedded.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/customconverters.py` & `robotframework-6.1rc1/src/robot/running/arguments/customconverters.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/typeconverters.py` & `robotframework-6.1rc1/src/robot/running/arguments/typeconverters.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/typevalidator.py` & `robotframework-6.1rc1/src/robot/running/arguments/typevalidator.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/argumentspec.py` & `robotframework-6.1rc1/src/robot/running/arguments/argumentspec.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/argumentparser.py` & `robotframework-6.1rc1/src/robot/running/arguments/argumentparser.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/argumentvalidator.py` & `robotframework-6.1rc1/src/robot/running/arguments/argumentvalidator.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/running/arguments/__init__.py` & `robotframework-6.1rc1/src/robot/running/arguments/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/robotio.py` & `robotframework-6.1rc1/src/robot/utils/robotio.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/filereader.py` & `robotframework-6.1rc1/src/robot/utils/filereader.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from collections.abc import Iterator
-from io import IOBase, StringIO
+from io import StringIO
 from pathlib import Path
-from typing import Union
+from typing import TextIO, Union
 
 from .robottypes import is_bytes, is_pathlike, is_string
 
 
-Source = Union[Path, str, IOBase]
+Source = Union[Path, str, TextIO]
 
 
 class FileReader:  # FIXME: Rename to SourceReader
     """Utility to ease reading different kind of source files.
 
     Supports different sources where to read the data:
 
@@ -42,15 +42,15 @@
     In all cases bytes are automatically decoded to Unicode and possible
     BOM removed.
     """
 
     def __init__(self, source: Source, accept_text: bool = False):
         self.file, self._opened = self._get_file(source, accept_text)
 
-    def _get_file(self, source: Source, accept_text: bool) -> 'tuple[IOBase, bool]':
+    def _get_file(self, source: Source, accept_text: bool) -> 'tuple[TextIO, bool]':
         path = self._get_path(source, accept_text)
         if path:
             file = open(path, 'rb')
             opened = True
         elif is_string(source):
             file = StringIO(source)
             opened = True
```

## Comparing `robotframework-6.1b1/src/robot/utils/sortable.py` & `robotframework-6.1rc1/src/robot/utils/sortable.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/escaping.py` & `robotframework-6.1rc1/src/robot/utils/escaping.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/restreader.py` & `robotframework-6.1rc1/src/robot/utils/restreader.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/frange.py` & `robotframework-6.1rc1/src/robot/utils/frange.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/connectioncache.py` & `robotframework-6.1rc1/src/robot/utils/connectioncache.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/normalizing.py` & `robotframework-6.1rc1/src/robot/utils/normalizing.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,32 +10,39 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import re
-from collections.abc import Mapping, MutableMapping, Sequence
-from typing import overload
+from collections.abc import Iterable, Iterator, Mapping, Sequence
+from typing import Any, MutableMapping, overload, TypeVar
+
+
+V = TypeVar('V')
+Self = TypeVar('Self', bound='NormalizedDict')
 
 
 @overload
 def normalize(string: str, ignore: 'Sequence[str]' = (), caseless: bool = True,
               spaceless: bool = True) -> str:
     ...
 
+
 @overload
 def normalize(string: bytes, ignore: 'Sequence[bytes]' = (), caseless: bool = True,
               spaceless: bool = True) -> bytes:
     ...
 
+
+# TODO: Remove bytes support in RF 7.0. There shouldn't be needs for that with Python 3.
 def normalize(string, ignore=(), caseless=True, spaceless=True):
-    """Normalizes given string according to given spec.
+    """Normalize the ``string`` according to the given spec.
 
-    By default string is turned to lower case and all whitespace is removed.
+    By default, string is turned to lower case and all whitespace is removed.
     Additional characters can be removed by giving them in ``ignore`` list.
     """
     empty = '' if isinstance(string, str) else b''
     if isinstance(ignore, bytes):
         # Iterating bytes in Python3 yields integers.
         ignore = [bytes([i]) for i in ignore]
     if spaceless:
@@ -51,81 +58,81 @@
     return string
 
 
 def normalize_whitespace(string):
     return re.sub(r'\s', ' ', string, flags=re.UNICODE)
 
 
-class NormalizedDict(MutableMapping):
+class NormalizedDict(MutableMapping[str, V]):
     """Custom dictionary implementation automatically normalizing keys."""
 
-    def __init__(self, initial=None, ignore=(), caseless=True, spaceless=True):
+    def __init__(self, initial: 'Mapping[str, V]|Iterable[tuple[str, V]]|None' = None,
+                 ignore: 'Sequence[str]' = (), caseless: bool = True,
+                 spaceless: bool = True):
         """Initialized with possible initial value and normalizing spec.
 
         Initial values can be either a dictionary or an iterable of name/value
-        pairs. In the latter case items are added in the given order.
+        pairs.
 
         Normalizing spec has exact same semantics as with the :func:`normalize`
         function.
         """
-        self._data = {}
-        self._keys = {}
+        self._data: 'dict[str, V]' = {}
+        self._keys: 'dict[str, str]' = {}
         self._normalize = lambda s: normalize(s, ignore, caseless, spaceless)
         if initial:
-            items = initial.items() if hasattr(initial, 'items') else initial
-            for key, value in items:
-                self[key] = value
+            self.update(initial)
 
     @property
-    def normalized_keys(self):
-        return self._keys
+    def normalized_keys(self) -> 'tuple[str, ...]':
+        return tuple(self._keys)
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> V:
         return self._data[self._normalize(key)]
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: str, value: V):
         norm_key = self._normalize(key)
         self._data[norm_key] = value
         self._keys.setdefault(norm_key, key)
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: str):
         norm_key = self._normalize(key)
         del self._data[norm_key]
         del self._keys[norm_key]
 
-    def __iter__(self):
+    def __iter__(self) -> 'Iterator[str]':
         return (self._keys[norm_key] for norm_key in sorted(self._keys))
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._data)
 
-    def __str__(self):
+    def __str__(self) -> str:
         items = ', '.join(f'{key!r}: {self[key]!r}' for key in self)
         return f'{{{items}}}'
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         name = type(self).__name__
         params = str(self) if self else ''
         return f'{name}({params})'
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if not isinstance(other, Mapping):
             return False
         if not isinstance(other, NormalizedDict):
             other = NormalizedDict(other)
         return self._data == other._data
 
-    def copy(self):
-        copy = NormalizedDict()
+    def copy(self: Self) -> Self:
+        copy = type(self)()
         copy._data = self._data.copy()
         copy._keys = self._keys.copy()
         copy._normalize = self._normalize
         return copy
 
     # Speed-ups. Following methods are faster than default implementations.
 
-    def __contains__(self, key):
+    def __contains__(self, key: str) -> bool:
         return self._normalize(key) in self._data
 
     def clear(self):
         self._data.clear()
         self._keys.clear()
```

## Comparing `robotframework-6.1b1/src/robot/utils/markupwriters.py` & `robotframework-6.1rc1/src/robot/utils/markupwriters.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/setter.py` & `robotframework-6.1rc1/src/robot/utils/setter.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import sys
 from typing import Callable, Generic, overload, TypeVar, Type, Union
 
 
 T = TypeVar('T')
 V = TypeVar('V')
 A = TypeVar('A')
 
@@ -88,7 +89,11 @@
         if '__slots__' in dct:
             slots = list(dct['__slots__'])
             for item in dct.values():
                 if isinstance(item, setter):
                     slots.append(item.attr_name)
             dct['__slots__'] = slots
         return type.__new__(cls, name, bases, dct)
+
+    if sys.version_info < (3, 7):
+        def __getitem__(self, item):
+            return self
```

## Comparing `robotframework-6.1b1/src/robot/utils/compress.py` & `robotframework-6.1rc1/src/robot/utils/compress.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/misc.py` & `robotframework-6.1rc1/src/robot/utils/misc.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/dotdict.py` & `robotframework-6.1rc1/src/robot/utils/dotdict.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/recommendations.py` & `robotframework-6.1rc1/src/robot/utils/recommendations.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/text.py` & `robotframework-6.1rc1/src/robot/utils/text.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,20 +76,21 @@
 def _count_virtual_line_length(line):
     if not line:
         return 1
     lines, remainder = divmod(len(line), _MAX_ERROR_LINE_LENGTH)
     return lines if not remainder else lines + 1
 
 
-def format_assign_message(variable, value, cut_long=True):
+def format_assign_message(variable, value, items=None, cut_long=True):
     formatter = {'$': safe_str, '@': seq2str2, '&': _dict_to_str}[variable[0]]
     value = formatter(value)
     if cut_long:
         value = cut_assign_value(value)
-    return '%s = %s' % (variable, value)
+    decorated_items = ''.join(f'[{item}]' for item in items) if items else ''
+    return f'{variable}{decorated_items} = {value}'
 
 def _dict_to_str(d):
     if not d:
         return '{ }'
     return '{ %s }' % ' | '.join('%s=%s' % (safe_str(k), safe_str(d[k])) for k in d)
```

## Comparing `robotframework-6.1b1/src/robot/utils/unic.py` & `robotframework-6.1rc1/src/robot/utils/unic.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/markuputils.py` & `robotframework-6.1rc1/src/robot/utils/markuputils.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/robotpath.py` & `robotframework-6.1rc1/src/robot/utils/robotpath.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/robottime.py` & `robotframework-6.1rc1/src/robot/utils/robottime.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/encoding.py` & `robotframework-6.1rc1/src/robot/utils/encoding.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/encodingsniffer.py` & `robotframework-6.1rc1/src/robot/utils/encodingsniffer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/argumentparser.py` & `robotframework-6.1rc1/src/robot/utils/argumentparser.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/asserts.py` & `robotframework-6.1rc1/src/robot/utils/asserts.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/__init__.py` & `robotframework-6.1rc1/src/robot/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
                          is_list_like, is_number, is_pathlike, is_string, is_truthy,
                          is_union, type_name, type_repr, typeddict_types)
 from .setter import setter, SetterAwareType
 from .sortable import Sortable
 from .text import (cut_assign_value, cut_long_message, format_assign_message,
                    get_console_length, getdoc, getshortdoc, pad_console_length,
                    split_tags_from_doc, split_args_from_name_or_path)
+from .typehints import copy_signature, KnownAtRuntime
 from .unic import prepr, safe_str
 
 
 def read_rest_data(rstfile):
     from .restreader import read_rest_data
     return read_rest_data(rstfile)
```

## Comparing `robotframework-6.1b1/src/robot/utils/application.py` & `robotframework-6.1rc1/src/robot/utils/application.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/etreewrapper.py` & `robotframework-6.1rc1/src/robot/utils/etreewrapper.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/match.py` & `robotframework-6.1rc1/src/robot/utils/match.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import re
 import fnmatch
-from functools import partial
 from typing import Iterable, Iterator, Sequence
 
 from .normalizing import normalize
 from .robottypes import is_string
 
 
 def eq(str1: str, str2: str, ignore: Sequence[str] = (), caseless: bool = True,
@@ -30,27 +29,29 @@
 
 
 class Matcher:
 
     def __init__(self, pattern: str, ignore: Sequence[str] = (), caseless: bool = True,
                  spaceless: bool = True, regexp: bool = False):
         self.pattern = pattern
-        self._normalize = partial(normalize, ignore=ignore, caseless=caseless,
-                                  spaceless=spaceless)
+        if caseless or spaceless or ignore:
+            self._normalize = lambda s: normalize(s, ignore, caseless, spaceless)
+        else:
+            self._normalize = lambda s: s
         self._regexp = self._compile(self._normalize(pattern), regexp=regexp)
 
     def _compile(self, pattern, regexp=False):
         if not regexp:
             pattern = fnmatch.translate(pattern)
         return re.compile(pattern, re.DOTALL)
 
     def match(self, string: str) -> bool:
         return self._regexp.match(self._normalize(string)) is not None
 
-    def match_any(self, strings: Sequence[str]) -> bool:
+    def match_any(self, strings: Iterable[str]) -> bool:
         return any(self.match(s) for s in strings)
 
     def __bool__(self) -> bool:
         return bool(self._normalize(self.pattern))
 
 
 class MultiMatcher(Iterable[Matcher]):
@@ -70,15 +71,15 @@
         return patterns
 
     def match(self, string: str) -> bool:
         if self.matchers:
             return any(m.match(string) for m in self.matchers)
         return self.match_if_no_patterns
 
-    def match_any(self, strings: Sequence[str]) -> bool:
+    def match_any(self, strings: Iterable[str]) -> bool:
         return any(self.match(s) for s in strings)
 
     def __len__(self) -> int:
         return len(self.matchers)
 
     def __iter__(self) -> Iterator[Matcher]:
         return iter(self.matchers)
```

## Comparing `robotframework-6.1b1/src/robot/utils/error.py` & `robotframework-6.1rc1/src/robot/utils/error.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/robotenv.py` & `robotframework-6.1rc1/src/robot/utils/robotenv.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/htmlformatters.py` & `robotframework-6.1rc1/src/robot/utils/htmlformatters.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/charwidth.py` & `robotframework-6.1rc1/src/robot/utils/charwidth.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/platform.py` & `robotframework-6.1rc1/src/robot/utils/platform.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/importer.py` & `robotframework-6.1rc1/src/robot/utils/importer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/robotinspect.py` & `robotframework-6.1rc1/src/robot/utils/robotinspect.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/utils/robottypes.py` & `robotframework-6.1rc1/src/robot/utils/robottypes.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/jsonwriter.py` & `robotframework-6.1rc1/src/robot/htmldata/jsonwriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/htmlfilewriter.py` & `robotframework-6.1rc1/src/robot/htmldata/htmlfilewriter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/template.py` & `robotframework-6.1rc1/src/robot/htmldata/template.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/__init__.py` & `robotframework-6.1rc1/src/robot/htmldata/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.css` & `robotframework-6.1rc1/src/robot/htmldata/libdoc/libdoc.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/libdoc/libdoc.html` & `robotframework-6.1rc1/src/robot/htmldata/libdoc/libdoc.html`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,17 @@
           arguments.search = false;
       }
       $.tmpl(name + '-template', arguments).appendTo(container);
     }
 
     function scrollToHash() {
         if (window.location.hash) {
-            var hash = window.location.hash.substring(1).replace('+', ' ');
-            window.location.hash = '';
-            window.location.hash = hash;
+            var hash = window.location.hash.substring(1);
+            var id = decodeURIComponent(hash);
+            document.getElementById(id).scrollIntoView();
         }
     }
 
     function tagSearch(tag, hash) {
       document.getElementsByClassName('search-input')[0].value = '';
       const include = {tags: true, tagsExact: true};
       const url = window.location.pathname + "?tag=" + tag + (hash || "");
```

## Comparing `robotframework-6.1b1/src/robot/htmldata/libdoc/__init__.py` & `robotframework-6.1rc1/src/robot/htmldata/libdoc/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/libdoc/pygments.css` & `robotframework-6.1rc1/src/robot/htmldata/libdoc/pygments.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/libdoc/doc_formatting.css` & `robotframework-6.1rc1/src/robot/htmldata/libdoc/doc_formatting.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/common.css` & `robotframework-6.1rc1/src/robot/htmldata/rebot/common.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/report.css` & `robotframework-6.1rc1/src/robot/htmldata/rebot/report.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/log.js` & `robotframework-6.1rc1/src/robot/htmldata/rebot/log.js`

 * *Files 2% similar despite different names*

### js-beautify {}

```diff
@@ -9,14 +9,17 @@
 
 function toggleSuite(suiteId) {
     toggleElement(suiteId, ['keyword', 'suite', 'test']);
 }
 
 function toggleTest(testId) {
     toggleElement(testId, ['keyword']);
+    var test = window.testdata.findLoaded(testId);
+    if (test.status == "FAIL" || test.status == "SKIP")
+        expandFailed(test);
 }
 
 function toggleKeyword(kwId) {
     toggleElement(kwId, ['keyword']);
 }
 
 function toggleElement(elementId, childrenNames) {
@@ -86,15 +89,15 @@
 function loadAndExpandElementIds(ids) {
     for (var i in ids) {
         window.testdata.ensureLoaded(ids[i], expandElementsWithIds);
     }
 }
 
 function expandFailed(element) {
-    if (element.status == "FAIL") {
+    if (element.status == "FAIL" || (element.type == "test" && element.status == "SKIP")) {
         window.elementsToExpand = [element];
         window.expandDecider = function(e) {
             return e.status == "FAIL";
         };
         expandRecursively();
     }
 }
```

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/print.css` & `robotframework-6.1rc1/src/robot/htmldata/rebot/print.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/view.js` & `robotframework-6.1rc1/src/robot/htmldata/rebot/view.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/report.html` & `robotframework-6.1rc1/src/robot/htmldata/rebot/report.html`

 * *Files 0% similar despite different names*

```diff
@@ -261,16 +261,16 @@
         return !(excludePattern && test.matchesTagPattern(excludePattern));
     });
 }
 
 function scrollToSelector(base, query) {
     $('#test-details-container').css('min-height', $(window).height());
     var anchor = query ? base + '?' + encodeURIComponent(query) : base;
-    window.location.hash = '';
     window.location.hash = window.prevLocationHash = anchor;
+    document.getElementById('test-details-container').scrollIntoView();
 }
 
 function renderSelector(args, template, stats) {
     window.elementsToRender = [];
     var container = $('#test-details-container');
     container.empty();
     $.tmpl('detailsHeaderTemplate', args).appendTo(container);
```

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/testdata.js` & `robotframework-6.1rc1/src/robot/htmldata/rebot/testdata.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/util.js` & `robotframework-6.1rc1/src/robot/htmldata/rebot/util.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/model.js` & `robotframework-6.1rc1/src/robot/htmldata/rebot/model.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/log.html` & `robotframework-6.1rc1/src/robot/htmldata/rebot/log.html`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,16 @@
 }
 
 function makeElementVisible(id) {
     window.testdata.ensureLoaded(id, function (ids) {
         util.map(ids, expandElementWithId);
         if (ids.length) {
             expandFailed(window.testdata.findLoaded(util.last(ids)));
-            window.location.hash = '';
             window.location.hash = id;
+            document.getElementById(id).scrollIntoView();
             highlightLinkTarget();
         }
     });
 }
 
 function addExecutionLog(main) {
     $('body').append($(testOrTask('<h2>{Test} Execution Log</h2>')),
```

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/fileloading.js` & `robotframework-6.1rc1/src/robot/htmldata/rebot/fileloading.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/__init__.py` & `robotframework-6.1rc1/src/robot/htmldata/rebot/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/doc_formatting.css` & `robotframework-6.1rc1/src/robot/htmldata/rebot/doc_formatting.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/rebot/log.css` & `robotframework-6.1rc1/src/robot/htmldata/rebot/log.css`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/lib/jsxcompressor.min.js` & `robotframework-6.1rc1/src/robot/htmldata/lib/jsxcompressor.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/lib/__init__.py` & `robotframework-6.1rc1/src/robot/htmldata/lib/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/lib/jquery.tablesorter.min.js` & `robotframework-6.1rc1/src/robot/htmldata/lib/jquery.tablesorter.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/lib/jquery.highlight.min.js` & `robotframework-6.1rc1/src/robot/htmldata/lib/jquery.highlight.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/lib/jquery.min.js` & `robotframework-6.1rc1/src/robot/htmldata/lib/jquery.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/lib/jquery.tmpl.min.js` & `robotframework-6.1rc1/src/robot/htmldata/lib/jquery.tmpl.min.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/testdoc/__init__.py` & `robotframework-6.1rc1/src/robot/htmldata/testdoc/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/testdoc/testdoc.html` & `robotframework-6.1rc1/src/robot/htmldata/testdoc/testdoc.html`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/common/storage.js` & `robotframework-6.1rc1/src/robot/htmldata/common/storage.js`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/htmldata/common/__init__.py` & `robotframework-6.1rc1/src/robot/htmldata/common/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/__init__.py` & `robotframework-6.1rc1/src/robot/parsing/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/model/blocks.py` & `robotframework-6.1rc1/src/robot/parsing/model/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from abc import ABC
 from contextlib import contextmanager
-from io import IOBase
 from pathlib import Path
-from typing import cast, Iterator, Sequence, Union
+from typing import cast, Iterator, Sequence, TextIO, Union
 
 from robot.utils import file_writer, test_or_task
 
 from .statements import (Break, Continue, ElseHeader, ElseIfHeader, End, ExceptHeader,
                          Error, FinallyHeader, ForHeader, IfHeader, KeywordCall,
                          KeywordName, Node, ReturnSetting, ReturnStatement,
                          SectionHeader, Statement, TemplateArguments, TestCaseName,
@@ -70,15 +69,15 @@
     def __init__(self, sections: 'Sequence[Section]' = (), source: 'Path|None' = None,
                  languages: Sequence[str] = ()):
         super().__init__()
         self.sections = list(sections)
         self.source = source
         self.languages = list(languages)
 
-    def save(self, output: 'Path|str|IOBase|None' = None):
+    def save(self, output: 'Path|str|TextIO|None' = None):
         """Save model to the given ``output`` or to the original source file.
 
         The ``output`` can be a path to a file or an already opened file
         object. If ``output`` is not given, the original source file will
         be overwritten.
         """
         output = output or self.source
@@ -383,15 +382,15 @@
             self.errors += ('WHILE loop cannot be empty.',)
         if not self.end:
             self.errors += ('WHILE loop must have closing END.',)
 
 
 class ModelWriter(ModelVisitor):
 
-    def __init__(self, output: 'Path|str|IOBase'):
+    def __init__(self, output: 'Path|str|TextIO'):
         if isinstance(output, (Path, str)):
             self.writer = file_writer(output)
             self.close_writer = True
         else:
             self.writer = output
             self.close_writer = False
```

## Comparing `robotframework-6.1b1/src/robot/parsing/model/__init__.py` & `robotframework-6.1rc1/src/robot/parsing/model/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/model/visitor.py` & `robotframework-6.1rc1/src/robot/parsing/model/visitor.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/model/statements.py` & `robotframework-6.1rc1/src/robot/parsing/model/statements.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/parser/blockparsers.py` & `robotframework-6.1rc1/src/robot/parsing/parser/blockparsers.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/parser/parser.py` & `robotframework-6.1rc1/src/robot/parsing/parser/parser.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/parser/__init__.py` & `robotframework-6.1rc1/src/robot/parsing/parser/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/parser/fileparser.py` & `robotframework-6.1rc1/src/robot/parsing/parser/fileparser.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/lexer/lexer.py` & `robotframework-6.1rc1/src/robot/parsing/lexer/lexer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/lexer/blocklexers.py` & `robotframework-6.1rc1/src/robot/parsing/lexer/blocklexers.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/lexer/context.py` & `robotframework-6.1rc1/src/robot/parsing/lexer/context.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/lexer/settings.py` & `robotframework-6.1rc1/src/robot/parsing/lexer/settings.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/lexer/tokens.py` & `robotframework-6.1rc1/src/robot/parsing/lexer/tokens.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/lexer/statementlexers.py` & `robotframework-6.1rc1/src/robot/parsing/lexer/statementlexers.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             token.type = Token.ARGUMENT
 
     def _lex_as_keyword_call(self):
         keyword_seen = False
         for token in self.statement:
             if keyword_seen:
                 token.type = Token.ARGUMENT
-            elif is_assign(token.value, allow_assign_mark=True):
+            elif is_assign(token.value, allow_assign_mark=True, allow_items=True):
                 token.type = Token.ASSIGN
             else:
                 token.type = Token.KEYWORD
                 keyword_seen = True
 
 
 class ForHeaderLexer(StatementLexer):
@@ -240,15 +240,15 @@
 class InlineIfHeaderLexer(StatementLexer):
     token_type = Token.INLINE_IF
 
     def handles(self, statement: StatementTokens) -> bool:
         for token in statement:
             if token.value == 'IF':
                 return True
-            if not is_assign(token.value, allow_assign_mark=True):
+            if not is_assign(token.value, allow_assign_mark=True, allow_items=True):
                 return False
         return False
 
     def lex(self):
         if_seen = False
         for token in self.statement:
             if if_seen:
```

## Comparing `robotframework-6.1b1/src/robot/parsing/lexer/__init__.py` & `robotframework-6.1rc1/src/robot/parsing/lexer/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/parsing/lexer/tokenizer.py` & `robotframework-6.1rc1/src/robot/parsing/lexer/tokenizer.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/XML.py` & `robotframework-6.1rc1/src/robot/libraries/XML.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/Screenshot.py` & `robotframework-6.1rc1/src/robot/libraries/Screenshot.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/Easter.py` & `robotframework-6.1rc1/src/robot/libraries/Easter.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/dialogs_py.py` & `robotframework-6.1rc1/src/robot/libraries/dialogs_py.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/String.py` & `robotframework-6.1rc1/src/robot/libraries/String.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/Telnet.py` & `robotframework-6.1rc1/src/robot/libraries/Telnet.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/DateTime.py` & `robotframework-6.1rc1/src/robot/libraries/DateTime.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/Remote.py` & `robotframework-6.1rc1/src/robot/libraries/Remote.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/OperatingSystem.py` & `robotframework-6.1rc1/src/robot/libraries/OperatingSystem.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/Collections.py` & `robotframework-6.1rc1/src/robot/libraries/Collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import copy
+from ast import literal_eval
 
 from robot.api import logger
-from robot.utils import (is_dict_like, is_list_like, is_string, is_truthy, Matcher,
-                         plural_or_not as s, seq2str, seq2str2, type_name)
+from robot.utils import (get_error_message, is_dict_like, is_list_like, is_truthy,
+                         Matcher, plural_or_not as s, seq2str, seq2str2, type_name)
 from robot.utils.asserts import assert_equal
 from robot.version import get_version
 
 
 class NotSet:
     def __repr__(self):
         return ""
@@ -107,14 +108,19 @@
         an integer.
 
         Example:
         | Set List Value | ${L3} | 1  | xxx |
         | Set List Value | ${L3} | -1 | yyy |
         =>
         | ${L3} = ['a', 'xxx', 'yyy']
+
+        Starting from Robot Framework 6.1, it is also possible to use the native
+        item assignment syntax. This is equivalent to the above:
+        | ${L3}[1] =  | Set Variable | xxx |
+        | ${L3}[-1] = | Set Variable | yyy |
         """
         self._validate_list(list_)
         try:
             list_[self._index_to_int(index)] = value
         except IndexError:
             self._index_error(list_, index)
 
@@ -491,29 +497,33 @@
 
         Use `Create Dictionary` from the BuiltIn library for constructing new
         dictionaries.
         """
         return dict(item)
 
     def set_to_dictionary(self, dictionary, *key_value_pairs, **items):
-        """Adds the given ``key_value_pairs`` and ``items`` to the ``dictionary``.
+        """Adds the given ``key_value_pairs`` and/or ``items`` to the ``dictionary``.
 
-        Giving items as ``key_value_pairs`` means giving keys and values
-        as separate arguments:
+        If given items already exist in the dictionary, their values are updated.
 
-        | Set To Dictionary | ${D1} | key | value | second | ${2} |
+        It is easiest to specify items using the ``name=value`` syntax:
+        | Set To Dictionary | ${D1} | key=value | second=${2} |
         =>
         | ${D1} = {'a': 1, 'key': 'value', 'second': 2}
 
-        | Set To Dictionary | ${D1} | key=value | second=${2} |
-
-        The latter syntax is typically more convenient to use, but it has
-        a limitation that keys must be strings.
+        A limitation of the above syntax is that keys must be strings.
+        That can be avoided by passing keys and values as separate arguments:
+        | Set To Dictionary | ${D1} | key | value | ${2} | value 2 |
+        =>
+        | ${D1} = {'a': 1, 'key': 'value', 2: 'value 2'}
 
-        If given keys already exist in the dictionary, their values are updated.
+        Starting from Robot Framework 6.1, it is also possible to use the native
+        item assignment syntax. This is equivalent to the above:
+        | ${D1}[key] =  | Set Variable | value |
+        | ${D1}[${2}] = | Set Variable | value 2 |
         """
         self._validate_dictionary(dictionary)
         if len(key_value_pairs) % 2 != 0:
             raise ValueError("Adding data to a dictionary failed. There "
                              "should be even number of key-value-pairs.")
         for i in range(0, len(key_value_pairs), 2):
             dictionary[key_value_pairs[i]] = key_value_pairs[i+1]
@@ -747,27 +757,49 @@
         Use the ``msg`` argument to override the default error message.
         """
         self._validate_dictionary(dictionary)
         _verify_condition(value not in dictionary.values(),
                           f"Dictionary contains value '{value}'.",
                           msg)
 
-    def dictionaries_should_be_equal(self, dict1, dict2, msg=None, values=True):
+    def dictionaries_should_be_equal(self, dict1, dict2, msg=None, values=True,
+                                     ignore_keys=None):
         """Fails if the given dictionaries are not equal.
 
         First the equality of dictionaries' keys is checked and after that all
         the key value pairs. If there are differences between the values, those
         are listed in the error message. The types of the dictionaries do not
         need to be same.
 
+        ``ignore_keys`` can be used to provide a list of keys to ignore in the
+        comparison. It can be an actual list or a Python list literal. This
+        option is new in Robot Framework 6.1.
+
+        Examples:
+        | Dictionaries Should Be Equal | ${dict} | ${expected} |
+        | Dictionaries Should Be Equal | ${dict} | ${expected} | ignore_keys=${ignored} |
+        | Dictionaries Should Be Equal | ${dict} | ${expected} | ignore_keys=['key1', 'key2'] |
+
         See `Lists Should Be Equal` for more information about configuring
         the error message with ``msg`` and ``values`` arguments.
         """
         self._validate_dictionary(dict1)
         self._validate_dictionary(dict2, 2)
+        if ignore_keys:
+            if isinstance(ignore_keys, str):
+                try:
+                    ignore_keys = literal_eval(ignore_keys)
+                except Exception:
+                    raise ValueError("Converting 'ignore_keys' to a list failed: "
+                                     + get_error_message())
+            if not is_list_like(ignore_keys):
+                raise ValueError(f"'ignore_keys' must be list-like, "
+                                 f"got {type_name(ignore_keys)}.")
+            dict1 = {k: v for k, v in dict1.items() if k not in ignore_keys}
+            dict2 = {k: v for k, v in dict2.items() if k not in ignore_keys}
         keys = self._keys_should_be_equal(dict1, dict2, msg, values)
         self._key_values_should_be_equal(keys, dict1, dict2, msg, values)
 
     def dictionary_should_contain_sub_dictionary(self, dict1, dict2, msg=None,
                                                  values=True):
         """Fails unless all items in ``dict2`` are found from ``dict1``.
 
@@ -1017,21 +1049,20 @@
     elif is_truthy(values) and str(values).upper() != 'NO VALUES':
         msg += '\n' + default_msg
     raise AssertionError(msg)
 
 
 def _get_matches_in_iterable(iterable, pattern, case_insensitive=False,
                              whitespace_insensitive=False):
-    if not is_string(pattern):
+    if not isinstance(pattern, str):
         raise TypeError(f"Pattern must be string, got '{type_name(pattern)}'.")
     regexp = False
     if pattern.startswith('regexp='):
         pattern = pattern[7:]
         regexp = True
     elif pattern.startswith('glob='):
         pattern = pattern[5:]
     matcher = Matcher(pattern,
                       caseless=is_truthy(case_insensitive),
                       spaceless=is_truthy(whitespace_insensitive),
                       regexp=regexp)
-    return [string for string in iterable
-            if is_string(string) and matcher.match(string)]
+    return [item for item in iterable if isinstance(item, str) and matcher.match(item)]
```

## Comparing `robotframework-6.1b1/src/robot/libraries/__init__.py` & `robotframework-6.1rc1/src/robot/libraries/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/Reserved.py` & `robotframework-6.1rc1/src/robot/libraries/Reserved.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/Dialogs.py` & `robotframework-6.1rc1/src/robot/libraries/Dialogs.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/libraries/BuiltIn.py` & `robotframework-6.1rc1/src/robot/libraries/BuiltIn.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
             except RuntimeError:
                 raise RuntimeError("'%s' cannot be converted to a floating "
                                    "point number: %s" % (item, error))
 
     def convert_to_string(self, item):
         """Converts the given item to a Unicode string.
 
-        Strings are also [http://www.macchiato.com/unicode/nfc-faq|
+        Strings are also [https://en.wikipedia.org/wiki/Unicode_equivalence|
         NFC normalized].
 
         Use `Encode String To Bytes` and `Decode Bytes To String` keywords
         in ``String`` library if you need to convert between Unicode and byte
         strings using different encodings. Use `Convert To Bytes` if you just
         want to create byte strings.
         """
@@ -831,15 +831,15 @@
         ``LEADING`` or ``TRAILING`` (case-insensitive), the comparison is done
         without leading or trailing spaces, respectively.
 
         If ``collapse_spaces`` is given a true value (see `Boolean arguments`) and both
         arguments are strings, the comparison is done with all white spaces replaced by
         a single space character.
 
-        Strings are always [http://www.macchiato.com/unicode/nfc-faq|
+        Strings are always [https://en.wikipedia.org/wiki/Unicode_equivalence|
         NFC normalized].
 
         ``strip_spaces`` is new in Robot Framework 4.0 and ``collapse_spaces`` is new
         in Robot Framework 4.1.
         """
         self._log_types_at_info_if_different(first, second)
         first = safe_str(first)
@@ -873,15 +873,15 @@
         ``LEADING`` or ``TRAILING`` (case-insensitive), the comparison is done
         without leading or trailing spaces, respectively.
 
         If ``collapse_spaces`` is given a true value (see `Boolean arguments`) and both
         arguments are strings, the comparison is done with all white spaces replaced by
         a single space character.
 
-        Strings are always [http://www.macchiato.com/unicode/nfc-faq| NFC normalized].
+        Strings are always [https://en.wikipedia.org/wiki/Unicode_equivalence|NFC normalized].
 
         ``strip_spaces`` is new in Robot Framework 4.0
         and ``collapse_spaces`` is new in Robot Framework 4.1.
         """
         self._log_types_at_info_if_different(first, second)
         first = safe_str(first)
         second = safe_str(second)
```

## Comparing `robotframework-6.1b1/src/robot/libraries/Process.py` & `robotframework-6.1rc1/src/robot/libraries/Process.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/api/interfaces.py` & `robotframework-6.1rc1/src/robot/api/interfaces.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/api/parsing.py` & `robotframework-6.1rc1/src/robot/api/parsing.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/api/deco.py` & `robotframework-6.1rc1/src/robot/api/deco.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/api/logger.py` & `robotframework-6.1rc1/src/robot/api/logger.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/api/__init__.py` & `robotframework-6.1rc1/src/robot/api/__init__.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robot/api/exceptions.py` & `robotframework-6.1rc1/src/robot/api/exceptions.py`

 * *Files identical despite different names*

## Comparing `robotframework-6.1b1/src/robotframework.egg-info/SOURCES.txt` & `robotframework-6.1rc1/src/robotframework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -249,14 +249,15 @@
 src/robot/utils/robotio.py
 src/robot/utils/robotpath.py
 src/robot/utils/robottime.py
 src/robot/utils/robottypes.py
 src/robot/utils/setter.py
 src/robot/utils/sortable.py
 src/robot/utils/text.py
+src/robot/utils/typehints.py
 src/robot/utils/unic.py
 src/robot/variables/__init__.py
 src/robot/variables/assigner.py
 src/robot/variables/evaluation.py
 src/robot/variables/filesetter.py
 src/robot/variables/finders.py
 src/robot/variables/notfound.py
```

## Comparing `robotframework-6.1b1/src/robotframework.egg-info/PKG-INFO` & `robotframework-6.1rc1/src/robotframework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: robotframework
-Version: 6.1b1
+Version: 6.1rc1
 Summary: Generic automation framework for acceptance testing and robotic process automation (RPA)
 Home-page: https://robotframework.org
 Author: Pekka Klärck
 Author-email: peke@eliga.fi
 License: Apache License 2.0
 Download-URL: https://pypi.org/project/robotframework
 Project-URL: Source, https://github.com/robotframework/robotframework
 Project-URL: Issue Tracker, https://github.com/robotframework/robotframework/issues
 Project-URL: Documentation, https://robotframework.org/robotframework
-Project-URL: Release Notes, https://github.com/robotframework/robotframework/blob/master/doc/releasenotes/rf-6.1b1.rst
+Project-URL: Release Notes, https://github.com/robotframework/robotframework/blob/master/doc/releasenotes/rf-6.1rc1.rst
 Project-URL: Slack, http://slack.robotframework.org
 Project-URL: Twitter, https://twitter.com/robotframework
 Description: Robot Framework
         ===============
         
         .. contents::
            :local:
@@ -173,14 +173,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Classifier: Topic :: Software Development :: Testing :: BDD
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.6
```

