# Comparing `tmp/yunxiao-0.2.1.tar.gz` & `tmp/yunxiao-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.2.1.tar", last modified: Sat Jun 10 13:47:08 2023, max compression
+gzip compressed data, was "yunxiao-0.2.2.tar", last modified: Mon Jun 12 14:34:20 2023, max compression
```

## Comparing `yunxiao-0.2.1.tar` & `yunxiao-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 13:47:08.407558 yunxiao-0.2.1/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    14308 2023-06-10 13:47:08.392860 yunxiao-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.2.1/README.md
--rw-rw-rw-   0        0        0      943 2023-06-10 13:46:34.000000 yunxiao-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 13:47:08.407558 yunxiao-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 13:47:08.386794 yunxiao-0.2.1/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.1/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    21418 2023-06-10 04:23:34.000000 yunxiao-0.2.1/yunxiao/app.py
--rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.1/yunxiao/web.py
--rw-rw-rw-   0        0        0     5237 2023-06-10 06:16:21.000000 yunxiao-0.2.1/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:47:08.391850 yunxiao-0.2.1/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    14308 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 14:34:20.460454 yunxiao-0.2.2/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    14308 2023-06-12 14:34:20.460454 yunxiao-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.2.2/README.md
+-rw-rw-rw-   0        0        0     1031 2023-06-12 14:34:05.000000 yunxiao-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 14:34:20.460454 yunxiao-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 14:34:20.453903 yunxiao-0.2.2/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.2/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.2/yunxiao/app.py
+-rw-rw-rw-   0        0        0    16714 2023-06-12 14:10:01.000000 yunxiao-0.2.2/yunxiao/v2.py
+-rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.2/yunxiao/web.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.2/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-12 14:34:20.458434 yunxiao-0.2.2/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    14308 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.2.1/LICENSE` & `yunxiao-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.1/PKG-INFO` & `yunxiao-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.1
+Version: 0.2.2
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.2.1/README.md` & `yunxiao-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.1/pyproject.toml` & `yunxiao-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.2.1"
+version = "0.2.2"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,10 +22,11 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.2.2" = "新增 v2, 更清晰的函数命名，简洁快速的拉取全部数据。"
 "0.2.1" = "web 端请求 BUG 修复"
 "0.2.0" = "BUG修复"
 "0.1.9" = "更改鉴权方式，保存鉴权到系统环境变量。当因鉴权失效导致请求失败时，自动更新鉴权并重新发起请求。意图减少更新鉴权的次数。"
```

### Comparing `yunxiao-0.2.1/yunxiao/app.py` & `yunxiao-0.2.2/yunxiao/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class App(YunXiao):
     def __init__(self, configfile: str = "yunxiao_config.ini", campus: list = None):
         """
         初始化，输入用户账号密码，以及要操作的校区。
         :param campus: 校区
+        :param configfile: 配置文件路径
         """
         super().__init__(configfile)
         if campus is None:
             self.campus = []
         else:
             self.campus = campus
 
@@ -42,51 +43,62 @@
                 json=kwargs.get("json"),
                 params=kwargs.get("params"),
                 headers={"x3-authentication": self.token}
             )
 
         return response.json()
 
+    # 列出校区
+    def list_campus(self):
+        return self.request(
+            method="get",
+            url="https://yunxiao.xiaogj.com/api/cs-crm/campus/list?type=2"
+        )
+
+    # [数据/当前数据] 总剩余学费，总欠缴费用，总欠缴物品费用，在读学员。
     def find_now_data_report(self):
         """
         [数据/当前数据]
         总剩余学费，总欠缴费用，总欠缴物品费用，在读学员。
         """
         return self.request(
             method="post",
             url=self.reportpath + "findNowDataReport",
             json={"campusIds": self.campus, "_t_": UsedTime.stamp}
         )
 
+    # 课消数据
     def find_course_money(self, date: str = UsedTime.yymm, datetype: int = 1):
         """
         课消数据。
         :param date: 月份，格式示例： 2023-02
         :param datetype:
         :return:
         """
         return self.request(
             method="post",
             url=self.reportpath + "findCourseMoney",
             json={"campusIds": self.campus, "date": date, "dateType": datetype, "_t_": UsedTime.stamp}
         )
 
+    # 学费收入数据
     def find_tuition(self, date: str = UsedTime.yymm, datetype: int = 1):
         """
         学费收入数据。
         :param date: 月份，格式示例： 2023-02
         :param datetype:
         :return:
         """
         return self.request(
             method="post",
             url=self.reportpath + "findTuition",
             json={"campusIds": self.campus, "date": date, "dateType": datetype, "_t_": UsedTime.stamp}
         )
 
+    # 学费退费数据
     def find_refund_money(self, date: str = UsedTime.yymm, datetype: int = 1):
         """
         学费退费数据
         :param date: 月份，格式示例： 2023-02
         :param datetype:
         :return:
         """
@@ -105,21 +117,17 @@
         """
         return self.request(
             method="post",
             url=self.reportpath + "findDataReport",
             json={"campusIds": self.campus, "date": date, "_t_": UsedTime.stamp}
         )
 
-    # [数据][报表][校区数据]
-    def find_data_report_list(
-            self,
-            startdate: str = UsedTime.yymm01,
-            enddate: str = UsedTime.today,
-            orderbycampus: int = 1
-    ):
+    # [数据][报表][校区数据] 某日到某日数据
+    def find_data_report_list(self, startdate: str = UsedTime.yymm01, enddate: str = UsedTime.today,
+                              orderbycampus: int = 1):
         """
         某日到某日数据。
         :param startdate: 起始日期
         :param enddate: 截至日期
         :param orderbycampus:
         :return:
         """
@@ -131,14 +139,15 @@
                 "startDate": startdate,
                 "endDate": enddate,
                 "orderByCampus": orderbycampus,
                 "_t_": UsedTime.stamp
             }
         )
 
+    # 学生数据 - 费用报表。
     def find_student_course_fee(
             self,
             curriculumids: list = None,
             status: list = None,
             studentname: str = None
     ):
         """
@@ -156,14 +165,15 @@
                 "curriculumIds": curriculumids,
                 "status": status,
                 "studentName": studentname,
                 "_t_": UsedTime.stamp
             }
         )
 
+    # 学生数据 - 课时报表。
     def find_student_course_amount(
             self,
             curriculumids: list = None,
             status: list = None,
             studentname: str = None
     ):
         """
@@ -181,32 +191,26 @@
                 "curriculumIds": curriculumids,
                 "status": status,
                 "studentName": studentname,
                 "_t_": UsedTime.stamp
             }
         )
 
-    def order(
-            self,
-            ordertype: int = 0,
-            searchname: str = "",
-            orderstatuslist: list = None,
-            starttime: str = UsedTime.yymm01,
-            endtime: str = UsedTime.today,
-            pagesize: int = 1
-    ):
+    # [收银管理/订单管理] 查看收费订单。
+    def order(self, ordertype: int = 0, searchname: str = "", orderstatuslist: list = None,
+              starttime: str = UsedTime.yymm01, endtime: str = UsedTime.today, pagesize: int = 1):
         """
         [收银管理/订单管理]
         查看收费订单。
-        :param ordertype:
-        :param searchname:
+        :param ordertype: 订单类型
+        :param searchname: 查询姓名
         :param orderstatuslist:
-        :param starttime:
-        :param endtime:
-        :param pagesize:
+        :param starttime: 起始时间
+        :param endtime: 截至时间
+        :param pagesize: 每页数量
         :return:
         """
         return self.request(
             method="post",
             url=self.orderpath + "Info/pageAdbOrder",
             json={
                 "_t_": UsedTime.stamp,
@@ -223,14 +227,15 @@
                 "page": {
                     "pageNum": 1,
                     "pageSize": pagesize
                 }
             }
         )
 
+    # [收银管理/订单管理/订单详情] 查询订单详情。
     def order_info(self, orderinfoid: int = 0):
         """
         [收银管理/订单管理/订单详情]
         查询订单详情。
         :param orderinfoid:
         :return:
         """
@@ -239,29 +244,24 @@
             url=self.orderpath + "Info/get",
             params={
                 "_t_": UsedTime.stamp,
                 "orderInfoId": orderinfoid,
             }
         )
 
-    # [工作台][订单管理][退费]
-    def refund_order(
-            self,
-            searchname: str = "",
-            starttime: str = UsedTime.yymm01,
-            endtime: str = UsedTime.today,
-            pagesize: int = 1
-    ):
+    # [工作台][订单管理][退费] 查询退费订单
+    def refund_order(self, searchname: str = "", starttime: str = UsedTime.yymm01,
+                     endtime: str = UsedTime.today, pagesize: int = 1):
         """
         [收银管理/订单管理/退费]
         查询退费订单。
-        :param searchname:
-        :param starttime:
-        :param endtime:
-        :param pagesize:
+        :param searchname: 查询姓名
+        :param starttime: 起始时间
+        :param endtime: 结束时间
+        :param pagesize: 项目数
         :return:
         """
         return self.request(
             method="post",
             url=self.orderpath + "Refund/adbRefundOrderInfoPage",
             json={
                 "_t_": UsedTime.stamp,
@@ -274,20 +274,16 @@
                 "page": {
                     "pageNum": 1,
                     "pageSize": pagesize
                 }
             }
         )
 
-    def course_absent(
-            self,
-            starttime: str = UsedTime.yymm01,
-            endtime: str = UsedTime.today,
-            pagesize: int = 1
-    ):
+    # [教务管理 / 缺勤管理]
+    def course_absent(self, starttime: str = UsedTime.yymm01, endtime: str = UsedTime.today, pagesize: int = 1):
         """
         [教务管理/缺勤管理]
         :param starttime: 起始时间
         :param endtime: 结束时间
         :param pagesize: 单页项目数量
         :return:
         """
@@ -306,20 +302,16 @@
                 "page": {
                     "pageNum": 1,
                     "pageSize": pagesize
                 }
             }
         )
 
-    def company_course(
-            self,
-            date: str = UsedTime.today,
-            teacherids: list = None,
-            pagesize: int = 1
-    ):
+    # [教务管理/课表点名/全部课表]
+    def company_course(self, date: str = UsedTime.today, teacherids: list = None, pagesize: int = 1):
         """
         [教务管理/课表点名/全部课表]
         :param date:
         :param teacherids:
         :param pagesize:
         :return:
         """
@@ -336,18 +328,15 @@
                     "pageNum": 1,
                     "pageSize": pagesize
                 }
             }
         )
 
     # [工作台][学员][学员卡包]
-    def student_card(
-            self,
-            studentid=None
-    ):
+    def student_card(self, studentid=None):
         """
         查看学员的课程卡包
         :param studentid: 学生ID
         :return: json数据
         """
         return self.request(
             method="post",
@@ -359,39 +348,31 @@
                     "pageNum": 1,
                     "pageSize": 999
                 }
             }
         )
 
     # [工作台][学员][就读课程]
-    def student_attend_course(
-            self,
-            studentid: str = None
-    ):
+    def student_attend_course(self, studentid: str = None):
         return self.request(
             method="post",
             url=self.edupath + "courseStudent/findStudentAttendCourse",
             json={
                 "_t_": UsedTime.stamp,
                 "studentId": studentid,
                 "page": {
                     "pageNum": 1,
                     "pageSize": 999
                 }
             }
         )
 
     # [工作台][学员][就读课程][出入班记录]
-    def operation_record_list(
-            self,
-            studentid: int = None,
-            curriculum_id: int = None,
-            campus_ids_index: int = None,
-            campus_id: int = None
-    ):
+    def operation_record_list(self, studentid: int = None, curriculum_id: int = None, campus_ids_index: int = None,
+                              campus_id: int = None):
         """
         [工作台][学员][就读课程][出入班记录]
         :param campus_id:
         :param campus_ids_index: 实例中选择的校区列表索引，必须从中列表中选择一个。
         :param studentid:
         :param curriculum_id:
         :return:
@@ -407,34 +388,30 @@
                 "campusId": campus_id,
                 "studentId": str(studentid),
                 "curriculumId": curriculum_id
             }
         )
 
     # [工作台][班级]
-    def class_info_page(
-            self,
-            classstatus=0,
-            curriculumids: list = None,
-            teacherids: list = None
-    ):
+    def class_info_page(self, classstatus=0, curriculumids: list = None, teacherids: list = None):
         return self.request(
             method="post",
             url=self.edupath + "classInfo/page",
             json={
                 "_t_": UsedTime.stamp,
                 "orgTag": 1,
                 "campusIds": self.campus,
                 "classStatus": classstatus,
                 "curriculumIds": curriculumids,
                 "teacherIds": teacherids,
                 "page": {"pageNum": 1, "pageSize": 500}
             }
         )
 
+    # 查询指定班级信息
     def class_info(self, classid: int = None):
         """
         查询指定班级信息
         :param classid: 班级id
         :return:
         """
         return self.request(
@@ -442,14 +419,15 @@
             url=self.edupath + "classInfo/getClassInfoVo",
             params={
                 "_t_": UsedTime.stamp,
                 "classId": classid
             }
         )
 
+    # 查询指定班级的学员
     def class_student(self, classid: int = None, inout: int = 1):
         """
         查询指定班级的学员
         :param classid:     班级id
         :param inout:       [1]当前在班学员 [2]历史学员
         :return:
         """
@@ -459,14 +437,15 @@
             params={
                 "_t_": UsedTime.stamp,
                 "classId": classid,
                 "inout": inout
             }
         )
 
+    # 查询指定班级排课
     def class_arrange(self, classid: int = None):
         """
         查询指定班级排课。
         :param classid: 班级id
         :return:
         """
         return self.request(
@@ -476,21 +455,16 @@
                 "_t_": UsedTime.stamp,
                 "classId": classid,
                 "isDesc": False,
                 "status": None
             }
         )
 
-    def arrange(
-            self,
-            starttime: str = None,
-            endtime: str = None,
-            page_num: int = 1,
-            page_size: int = 99999
-    ):
+    # 排课管理
+    def arrange(self, starttime: str = None, endtime: str = None, page_num: int = 1, page_size: int = 99999):
         """
         排课管理。
         :param page_num:
         :param page_size:
         :param starttime: 查询起始时间
         :param endtime: 查询截止时间
         :return:
@@ -506,19 +480,15 @@
                 "courseStatusList": [0, 1],
                 "displayCompletedClass": False,
                 "page": {"pageNum": page_num, "pageSize": page_size}
             }
         )
 
     # 查询所有在开的课程
-    def curriculum(
-            self,
-            searchname: str = None,
-            haltsalelist: list = None
-    ):
+    def curriculum(self, searchname: str = None, haltsalelist: list = None):
         """
         查询所有在开的课程
         :param searchname: 查找关键字。
         :param haltsalelist: 是否在售。0>在售 1>停售
         :return:
         """
         return self.request(
@@ -532,24 +502,22 @@
                 "page": {
                     "pageNum": 1,
                     "pageSize": 999
                 }
             }
         )
 
-    # 查询所有在开的课程
+    # 编辑课程
     def update_curriculum_price_item(
             self,
             searchname: str = None,
             haltsalelist: list = None
     ):
         """
-        查询所有在开的课程
-        :param searchname: 查找关键字。
-        :param haltsalelist: 是否在售。0>在售 1>停售
+        ⚠ 编辑课程，谨慎使用
         :return:
         """
         return self.request(
             method="post",
             url=self.edupath + "curriculum/updateCurriculumPriceItem",
             json={
                 "_t_": UsedTime.stamp,
@@ -560,38 +528,31 @@
                     "pageNum": 1,
                     "pageSize": 500
                 }
             }
         )
 
     # 设为曾就读学生。
-    def become_history(
-            self,
-            studentlist: list
-    ):
+    def become_history(self, studentlist: list):
         """
         设为曾就读学生。
         :param studentlist: 学生ID
         :return:
         """
         return self.request(
             method="post",
             url=self.edupath + "student/becomeHistory",
             json={
                 "_t_": UsedTime.stamp, "studentIds": studentlist
             }
         )
 
     # 设学生为停课状态。
-    def student_suspend_course(
-            self,
-            student_id: str,
-            suspend_course_date: str = UsedTime.today,
-            remove_class: int = True
-    ):
+    def student_suspend_course(self, student_id: str, suspend_course_date: str = UsedTime.today,
+                               remove_class: int = True):
         """
         设为停课状态。
         :param student_id: 学生ID
         :param suspend_course_date: 停课时间。0000-00-00
         :param remove_class: 是否从班级中移除
         :return:
         """
@@ -606,22 +567,16 @@
                 "studentId": student_id,
                 "suspendCourseDate": suspend_course_date,
                 "type": 0
             }
         )
 
     # [教务管理 / 学员] 列出学生
-    def student_list(
-            self,
-            curriculumids: list = None,
-            classids: list = None,
-            name: str = "",
-            status: list = None,
-            class_student_status: int = 0
-    ):
+    def student_list(self, curriculumids: list = None, classids: list = None, name: str = "",
+                     status: list = None, class_student_status: int = 0):
         """
         [教务管理/学员]
         列出学生
         :param curriculumids: 课程筛选
         :param classids: 班级筛选
         :param name: 姓名查询关键字
         :param status: 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员
@@ -644,35 +599,29 @@
                 "classStudentStatus": class_student_status,
                 "orgTag": 1,
                 "page": {"pageNum": 1, "pageSize": 1000000}
             }
         )
 
     # [教务管理 / 学员 / 学员详情] 查询学员详细信息。
-    def student_info(
-            self,
-            studentid: int = None
-    ):
+    def student_info(self, studentid: int = None):
         """
         [教务管理/学员/学员详情]
         查询学员详细信息。
         :param studentid: 学生ID
         :return:
         """
         return self.request(
             method="get",
             url=self.crmpath + "student/getContainFace",
             params={"_t_": UsedTime.stamp, "id": studentid, "companyId": 658811}
         )
 
     # 查询老师
-    def get_teacher_list(
-            self,
-            querykey: str = None
-    ):
+    def get_teacher_list(self, querykey: str = None):
         """
         查询老师
         :param querykey: 关键词检索
         :return:
         """
         return self.request(
             method="post",
@@ -686,8 +635,8 @@
             }
         )
 
 
 if __name__ == "__main__":
     logging.basicConfig(level="INFO")
     app = App("18050019727", "jm123456", [])
-    app.find_student_course_fee(status=[1]).get("data").get("cardCourseTradedList")
+    app.find_student_course_fee(status=[1]).get("data").get("cardCourseTradedList")
```

### Comparing `yunxiao-0.2.1/yunxiao/web.py` & `yunxiao-0.2.2/yunxiao/web.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.1/yunxiao/yunxiao.py` & `yunxiao-0.2.2/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.1/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.2.2/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.1
+Version: 0.2.2
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

