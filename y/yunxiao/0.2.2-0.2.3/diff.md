# Comparing `tmp/yunxiao-0.2.2.tar.gz` & `tmp/yunxiao-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.2.2.tar", last modified: Mon Jun 12 14:34:20 2023, max compression
+gzip compressed data, was "yunxiao-0.2.3.tar", last modified: Mon Jun 12 20:59:39 2023, max compression
```

## Comparing `yunxiao-0.2.2.tar` & `yunxiao-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 14:34:20.460454 yunxiao-0.2.2/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    14308 2023-06-12 14:34:20.460454 yunxiao-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.2.2/README.md
--rw-rw-rw-   0        0        0     1031 2023-06-12 14:34:05.000000 yunxiao-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 14:34:20.460454 yunxiao-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 14:34:20.453903 yunxiao-0.2.2/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.2/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.2/yunxiao/app.py
--rw-rw-rw-   0        0        0    16714 2023-06-12 14:10:01.000000 yunxiao-0.2.2/yunxiao/v2.py
--rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.2/yunxiao/web.py
--rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.2/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-12 14:34:20.458434 yunxiao-0.2.2/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    14308 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 14:34:20.000000 yunxiao-0.2.2/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 20:59:39.390273 yunxiao-0.2.3/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0    12954 2023-06-12 20:59:39.389265 yunxiao-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12463 2023-06-12 14:40:15.000000 yunxiao-0.2.3/README.md
+-rw-rw-rw-   0        0        0     1031 2023-06-12 20:59:24.000000 yunxiao-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 20:59:39.390273 yunxiao-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 20:59:39.377084 yunxiao-0.2.3/test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:59:04.000000 yunxiao-0.2.3/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:59:39.382154 yunxiao-0.2.3/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.3/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    21527 2023-06-12 09:49:14.000000 yunxiao-0.2.3/yunxiao/app.py
+-rw-rw-rw-   0        0        0    17304 2023-06-12 20:58:35.000000 yunxiao-0.2.3/yunxiao/v2.py
+-rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.3/yunxiao/web.py
+-rw-rw-rw-   0        0        0     5237 2023-06-12 10:27:58.000000 yunxiao-0.2.3/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:59:39.388258 yunxiao-0.2.3/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    12954 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 20:59:39.000000 yunxiao-0.2.3/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.2.2/LICENSE` & `yunxiao-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.2/PKG-INFO` & `yunxiao-0.2.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.2
+Version: 0.2.3
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # YunXiao API
 An API tool for YunXiao Education Institution Management System.
 
 
 # Copyright Statement
 YunXiao software is owned by XiaoGuanJia. This project is for learning purposes only. If there is any infringement, please contact me to delete.
 
 
 # Contact
 admin@sqkkyzx.com
 
 
 # API Endpoint
+
 ## App
 
 - ### arrange
 
 ` 排课管理。 ` 
 
 | Parameter | Description |
@@ -191,14 +193,22 @@
 ` 查询老师 ` 
 
 | Parameter | Description |
 |-----------|-------------|
 | querykey | 关键词检索 |
 
 
+- ### list_campus
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
 - ### operation_record_list
 
 ` [工作台][学员][就读课程][出入班记录] ` 
 
 | Parameter | Description |
 |-----------|-------------|
 | campus_ids_index | 实例中选择的校区列表索引，必须从中列表中选择一个。 |
@@ -206,14 +216,19 @@
 
 - ### order
 
 ` [收银管理/订单管理] ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| ordertype | 订单类型 |
+| searchname | 查询姓名 |
+| starttime | 起始时间 |
+| endtime | 截至时间 |
+| pagesize | 每页数量 |
 
 
 - ### order_info
 
 ` [收银管理/订单管理/订单详情] ` 
 
 | Parameter | Description |
@@ -222,14 +237,42 @@
 
 - ### refund_order
 
 ` [收银管理/订单管理/退费] ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| searchname | 查询姓名 |
+| starttime | 起始时间 |
+| endtime | 结束时间 |
+| pagesize | 项目数 |
+
+
+- ### renew_cookie
+
+` 刷新 cookie.tmp 配置中存储的 cookie ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### renew_token
+
+` 刷新 token.tmp 配置中存储的 token ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### request
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
 
 
 - ### student_attend_course
 
 `  ` 
 
 | Parameter | Description |
@@ -274,14 +317,22 @@
 | Parameter | Description |
 |-----------|-------------|
 | student_id | 学生ID |
 | suspend_course_date | 停课时间。0000-00-00 |
 | remove_class | 是否从班级中移除 |
 
 
+- ### update_curriculum_price_item
+
+` ⚠ 编辑课程，谨慎使用 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
 ## Web
 
 - ### find_course_sign_charge
 
 ` 查询课消记录 ` 
 
 | Parameter | Description |
@@ -296,429 +347,337 @@
 | Parameter | Description |
 |-----------|-------------|
 | starttime | 起始时间 |
 | endtime | 结束时间 |
 | orderstatus | 订单状态。 |
 
 
-- ### find_student_course_amount
+- ### find_payment_list
 
-` 取得所有学员的课时统计数据。 ` 
+` 收入明细报表。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
+| group_no | 收据编号 |
+| pay_start_date | 支付起始时间 |
+| pay_end_date | 支付结束时间 |
+| order_status | 订单状态 1>已付款 4>已作废 |
+| page_num | 页数 |
+| page_size | 每页项目数 |
 
 
-- ### find_student_course_fee
+- ### find_receipt
 
-` 取得所有学员的课时统计数据。 ` 
+` 收据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| student_name | 学员姓名。 |
-| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
-| display_history | 是否显示曾就读。<True:显示><False:不显示> |
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
 
 
-- ### student_course_card
+- ### find_student_course_amount
 
-` 取得所有学员的课程卡片。 ` 
+` 取得所有学员的课时统计数据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
 | page_num | 页数。 |
 | page_size | 每页记录数。 |
 
 
-- ### teacher_arrange
+- ### find_student_course_fee
 
-` 取得指定老师的课表。 ` 
+` 取得所有学员的课时统计数据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| teacher_id | 查询的老师ID |
-| start_date | 起始日期，默认为本周一 |
-| end_date | 结束日期，默认为本周日 |
+| student_name | 学员姓名。 |
+| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
+| display_history | 是否显示曾就读。<True:显示><False:不显示> |
 | page_num | 页数。 |
 | page_size | 每页记录数。 |
 
 
-## App
-
-- ### arrange
-
-` 排课管理。 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| starttime | 查询起始时间 |
-| endtime | 查询截止时间 |
-
-
-- ### become_history
+- ### receipt
 
-` 设为曾就读学生。 ` 
+` 收据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| studentlist | 学生ID |
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
 
 
-- ### class_arrange
+- ### renew_cookie
 
-` 查询指定班级排课。 ` 
+` 刷新 cookie.tmp 配置中存储的 cookie ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| classid | 班级id |
 
 
-- ### class_info
+- ### renew_token
 
-` 查询指定班级信息 ` 
+` 刷新 token.tmp 配置中存储的 token ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| classid | 班级id |
 
 
-- ### class_info_page
+- ### request
 
 `  ` 
 
 | Parameter | Description |
 |-----------|-------------|
 
 
-- ### class_student
-
-` 查询指定班级的学员 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| classid |     班级id |
-| inout |       [1]当前在班学员 [2]历史学员 |
-
-
-- ### company_course
-
-` [教务管理/课表点名/全部课表] ` 
-
-| Parameter | Description |
-|-----------|-------------|
-
-
-- ### course_absent
-
-` [教务管理/缺勤管理] ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| starttime | 起始时间 |
-| endtime | 结束时间 |
-| pagesize | 单页项目数量 |
-
-
-- ### curriculum
-
-` 查询所有在开的课程 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| searchname | 查找关键字。 |
-| haltsalelist | 是否在售。0>在售 1>停售 |
-
-
-- ### find_course_money
+- ### snap_info_by_payment_group_id
 
-` 课消数据。 ` 
+` 收据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 月份，格式示例： 2023-02 |
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
 
 
-- ### find_data_report
+- ### student_course_card
 
-` 每日简报。 ` 
+` 取得所有学员的课程卡片。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 日期，格式示例 2023-02-01 |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
 
 
-- ### find_data_report_list
+- ### teacher_arrange
 
-` 某日到某日数据。 ` 
+` 取得指定老师的课表。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| startdate | 起始日期 |
-| enddate | 截至日期 |
-
-
-- ### find_now_data_report
-
-` [数据/当前数据] ` 
+| teacher_id | 查询的老师ID |
+| start_date | 起始日期，默认为本周一 |
+| end_date | 结束日期，默认为本周日 |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
 
-| Parameter | Description |
-|-----------|-------------|
 
+## V2
 
-- ### find_refund_money
+- ### arrange_list_date
 
-` 学费退费数据 ` 
+` 列出日期范围全部排课[最大9999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 月份，格式示例： 2023-02 |
 
 
-- ### find_student_course_amount
+- ### arrange_list_daterange
 
-` 学生数据 - 课时报表。 ` 
+` 列出全部排课[最大99999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| curriculumids | 课程ID列表 |
-| status | 学生状态列表 |
-| studentname | 按学生姓名检索 |
 
 
-- ### find_student_course_fee
+- ### arrange_queery_date
 
-` 学生数据 - 费用报表。 ` 
+` ⚠ 未完成，无法使用 查询指定日期排课 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| curriculumids | 课程ID列表 |
-| status | 学生状态列表 |
-| studentname | 按学生姓名检索 |
 
 
-- ### find_tuition
+- ### arrange_query_daterange
 
-` 学费收入数据。 ` 
+` 排课管理。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 月份，格式示例： 2023-02 |
+| displayCompletedClass | 显示已结班排课 |
+| starttime | 查询起始时间 |
+| endtime | 查询截止时间 |
 
 
-- ### get_teacher_list
+- ### campus_list_all
 
-` 查询老师 ` 
+`  ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| querykey | 关键词检索 |
 
 
-- ### operation_record_list
+- ### campus_todaymoney_list_all
 
-` [工作台][学员][就读课程][出入班记录] ` 
+` 分校区列出指定日期的费用数据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| campus_ids_index | 实例中选择的校区列表索引，必须从中列表中选择一个。 |
+| date | 日期 |
 
 
-- ### order
+- ### card_list_all
 
-` [收银管理/订单管理] ` 
+` 列出所有课程卡 ` 
 
 | Parameter | Description |
 |-----------|-------------|
 
 
-- ### order_info
+- ### charge_detail_list_daterange
 
-` [收银管理/订单管理/订单详情] ` 
+` :param startdate: YY-MM-DD ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| enddate | YY-MM-DD |
 
 
-- ### refund_order
+- ### charge_record_list_daterange
 
-` [收银管理/订单管理/退费] ` 
+` :param startdate: YY-MM-DD ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| enddate | YY-MM-DD |
 
 
-- ### student_attend_course
+- ### class_list_all
 
 `  ` 
 
 | Parameter | Description |
 |-----------|-------------|
 
 
-- ### student_card
-
-` 查看学员的课程卡包 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| studentid | 学生ID |
-
-
-- ### student_info
+- ### curriculum_list_all
 
-` [教务管理/学员/学员详情] ` 
+` 列出全部课程[最大9999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| studentid | 学生ID |
 
 
-- ### student_list
+- ### curriculum_query
 
-` [教务管理/学员] ` 
+` 查询所有在开的课程 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| curriculumids | 课程筛选 |
-| classids | 班级筛选 |
-| name | 姓名查询关键字 |
-| status | 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员 |
-| class_student_status | 0>不筛选 1>未入班 2>已入班 |
+| searchname | 查找关键字。 |
+| haltsalelist | 是否在售。0>在售 1>停售 |
 
 
-- ### student_suspend_course
+- ### money_list_month
 
-` 设为停课状态。 ` 
+` :param yy_mm: 月份，格式示例： 2023-02 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| student_id | 学生ID |
-| suspend_course_date | 停课时间。0000-00-00 |
-| remove_class | 是否从班级中移除 |
 
 
-- ### update_curriculum_price_item
+- ### order_item_list_all
 
-` 查询所有在开的课程 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| searchname | 查找关键字。 |
-| haltsalelist | 是否在售。0>在售 1>停售 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-## Web
+- ### payment_item_list_all
 
-- ### find_course_sign_charge
-
-` 查询课消记录 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| sort_field | 时间筛选模式。 <operationTime> - 操作时间 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-- ### find_order_item_all
+- ### payment_record_list_all
 
-` 查询订单明细。 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| starttime | 起始时间 |
-| endtime | 结束时间 |
-| orderstatus | 订单状态。 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-- ### find_payment_list
+- ### payment_refund_list_all
 
-` 收入明细报表。 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| group_no | 收据编号 |
-| pay_start_date | 支付起始时间 |
-| pay_end_date | 支付结束时间 |
-| order_status | 订单状态 1>已付款 4>已作废 |
-| page_num | 页数 |
-| page_size | 每页项目数 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-- ### find_receipt
+- ### renew_cookie
 
-` 收据。 ` 
+` 刷新 cookie.tmp 配置中存储的 cookie ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| order_id | 订单 ID |
-| payment_group_id | 支付 ID |
 
 
-- ### find_student_course_amount
+- ### renew_token
 
-` 取得所有学员的课时统计数据。 ` 
+` 刷新 token.tmp 配置中存储的 token ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
 
 
-- ### find_student_course_fee
+- ### request
 
-` 取得所有学员的课时统计数据。 ` 
+`  ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| student_name | 学员姓名。 |
-| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
-| display_history | 是否显示曾就读。<True:显示><False:不显示> |
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
 
 
-- ### receipt
+- ### student_listall
 
-` 收据。 ` 
+` 列出全部学生[最大99999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| order_id | 订单 ID |
-| payment_group_id | 支付 ID |
 
 
-- ### snap_info_by_payment_group_id
+- ### student_query
 
-` 收据。 ` 
+` [教务管理/学员] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| order_id | 订单 ID |
-| payment_group_id | 支付 ID |
+| size | 项目数量 |
+| curriculumids | 课程筛选 |
+| classids | 班级筛选 |
+| name | 姓名查询关键字 |
+| status | 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员 |
+| class_student_status | 0>不筛选 1>未入班 2>已入班 |
 
 
-- ### student_course_card
+- ### teacher_list_all
 
-` 取得所有学员的课程卡片。 ` 
+` 列出全部老师<MAX-9999> ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
 
 
-- ### teacher_arrange
+- ### teacher_query
 
-` 取得指定老师的课表。 ` 
+` :return: ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| teacher_id | 查询的老师ID |
-| start_date | 起始日期，默认为本周一 |
-| end_date | 结束日期，默认为本周日 |
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
```

### Comparing `yunxiao-0.2.2/README.md` & `yunxiao-0.2.3/yunxiao.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,35 @@
+Metadata-Version: 2.1
+Name: yunxiao
+Version: 0.2.3
+Summary: An API SDK tool for Cloud School Education Institution Management System.
+Author-email: YiZixuan <admin@sqkkyzx.com>
+License: GPL-3.0-only
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # YunXiao API
 An API tool for YunXiao Education Institution Management System.
 
 
 # Copyright Statement
 YunXiao software is owned by XiaoGuanJia. This project is for learning purposes only. If there is any infringement, please contact me to delete.
 
 
 # Contact
 admin@sqkkyzx.com
 
 
 # API Endpoint
+
 ## App
 
 - ### arrange
 
 ` 排课管理。 ` 
 
 | Parameter | Description |
@@ -178,14 +193,22 @@
 ` 查询老师 ` 
 
 | Parameter | Description |
 |-----------|-------------|
 | querykey | 关键词检索 |
 
 
+- ### list_campus
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
 - ### operation_record_list
 
 ` [工作台][学员][就读课程][出入班记录] ` 
 
 | Parameter | Description |
 |-----------|-------------|
 | campus_ids_index | 实例中选择的校区列表索引，必须从中列表中选择一个。 |
@@ -193,14 +216,19 @@
 
 - ### order
 
 ` [收银管理/订单管理] ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| ordertype | 订单类型 |
+| searchname | 查询姓名 |
+| starttime | 起始时间 |
+| endtime | 截至时间 |
+| pagesize | 每页数量 |
 
 
 - ### order_info
 
 ` [收银管理/订单管理/订单详情] ` 
 
 | Parameter | Description |
@@ -209,14 +237,42 @@
 
 - ### refund_order
 
 ` [收银管理/订单管理/退费] ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| searchname | 查询姓名 |
+| starttime | 起始时间 |
+| endtime | 结束时间 |
+| pagesize | 项目数 |
+
+
+- ### renew_cookie
+
+` 刷新 cookie.tmp 配置中存储的 cookie ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### renew_token
+
+` 刷新 token.tmp 配置中存储的 token ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### request
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
 
 
 - ### student_attend_course
 
 `  ` 
 
 | Parameter | Description |
@@ -261,14 +317,22 @@
 | Parameter | Description |
 |-----------|-------------|
 | student_id | 学生ID |
 | suspend_course_date | 停课时间。0000-00-00 |
 | remove_class | 是否从班级中移除 |
 
 
+- ### update_curriculum_price_item
+
+` ⚠ 编辑课程，谨慎使用 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
 ## Web
 
 - ### find_course_sign_charge
 
 ` 查询课消记录 ` 
 
 | Parameter | Description |
@@ -283,429 +347,337 @@
 | Parameter | Description |
 |-----------|-------------|
 | starttime | 起始时间 |
 | endtime | 结束时间 |
 | orderstatus | 订单状态。 |
 
 
-- ### find_student_course_amount
+- ### find_payment_list
 
-` 取得所有学员的课时统计数据。 ` 
+` 收入明细报表。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
+| group_no | 收据编号 |
+| pay_start_date | 支付起始时间 |
+| pay_end_date | 支付结束时间 |
+| order_status | 订单状态 1>已付款 4>已作废 |
+| page_num | 页数 |
+| page_size | 每页项目数 |
 
 
-- ### find_student_course_fee
+- ### find_receipt
 
-` 取得所有学员的课时统计数据。 ` 
+` 收据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| student_name | 学员姓名。 |
-| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
-| display_history | 是否显示曾就读。<True:显示><False:不显示> |
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
 
 
-- ### student_course_card
+- ### find_student_course_amount
 
-` 取得所有学员的课程卡片。 ` 
+` 取得所有学员的课时统计数据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
 | page_num | 页数。 |
 | page_size | 每页记录数。 |
 
 
-- ### teacher_arrange
+- ### find_student_course_fee
 
-` 取得指定老师的课表。 ` 
+` 取得所有学员的课时统计数据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| teacher_id | 查询的老师ID |
-| start_date | 起始日期，默认为本周一 |
-| end_date | 结束日期，默认为本周日 |
+| student_name | 学员姓名。 |
+| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
+| display_history | 是否显示曾就读。<True:显示><False:不显示> |
 | page_num | 页数。 |
 | page_size | 每页记录数。 |
 
 
-## App
-
-- ### arrange
-
-` 排课管理。 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| starttime | 查询起始时间 |
-| endtime | 查询截止时间 |
-
-
-- ### become_history
+- ### receipt
 
-` 设为曾就读学生。 ` 
+` 收据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| studentlist | 学生ID |
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
 
 
-- ### class_arrange
+- ### renew_cookie
 
-` 查询指定班级排课。 ` 
+` 刷新 cookie.tmp 配置中存储的 cookie ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| classid | 班级id |
 
 
-- ### class_info
+- ### renew_token
 
-` 查询指定班级信息 ` 
+` 刷新 token.tmp 配置中存储的 token ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| classid | 班级id |
 
 
-- ### class_info_page
+- ### request
 
 `  ` 
 
 | Parameter | Description |
 |-----------|-------------|
 
 
-- ### class_student
-
-` 查询指定班级的学员 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| classid |     班级id |
-| inout |       [1]当前在班学员 [2]历史学员 |
-
-
-- ### company_course
-
-` [教务管理/课表点名/全部课表] ` 
-
-| Parameter | Description |
-|-----------|-------------|
-
-
-- ### course_absent
-
-` [教务管理/缺勤管理] ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| starttime | 起始时间 |
-| endtime | 结束时间 |
-| pagesize | 单页项目数量 |
-
-
-- ### curriculum
-
-` 查询所有在开的课程 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| searchname | 查找关键字。 |
-| haltsalelist | 是否在售。0>在售 1>停售 |
-
-
-- ### find_course_money
+- ### snap_info_by_payment_group_id
 
-` 课消数据。 ` 
+` 收据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 月份，格式示例： 2023-02 |
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
 
 
-- ### find_data_report
+- ### student_course_card
 
-` 每日简报。 ` 
+` 取得所有学员的课程卡片。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 日期，格式示例 2023-02-01 |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
 
 
-- ### find_data_report_list
+- ### teacher_arrange
 
-` 某日到某日数据。 ` 
+` 取得指定老师的课表。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| startdate | 起始日期 |
-| enddate | 截至日期 |
-
-
-- ### find_now_data_report
-
-` [数据/当前数据] ` 
+| teacher_id | 查询的老师ID |
+| start_date | 起始日期，默认为本周一 |
+| end_date | 结束日期，默认为本周日 |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
 
-| Parameter | Description |
-|-----------|-------------|
 
+## V2
 
-- ### find_refund_money
+- ### arrange_list_date
 
-` 学费退费数据 ` 
+` 列出日期范围全部排课[最大9999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 月份，格式示例： 2023-02 |
 
 
-- ### find_student_course_amount
+- ### arrange_list_daterange
 
-` 学生数据 - 课时报表。 ` 
+` 列出全部排课[最大99999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| curriculumids | 课程ID列表 |
-| status | 学生状态列表 |
-| studentname | 按学生姓名检索 |
 
 
-- ### find_student_course_fee
+- ### arrange_queery_date
 
-` 学生数据 - 费用报表。 ` 
+` ⚠ 未完成，无法使用 查询指定日期排课 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| curriculumids | 课程ID列表 |
-| status | 学生状态列表 |
-| studentname | 按学生姓名检索 |
 
 
-- ### find_tuition
+- ### arrange_query_daterange
 
-` 学费收入数据。 ` 
+` 排课管理。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 月份，格式示例： 2023-02 |
+| displayCompletedClass | 显示已结班排课 |
+| starttime | 查询起始时间 |
+| endtime | 查询截止时间 |
 
 
-- ### get_teacher_list
+- ### campus_list_all
 
-` 查询老师 ` 
+`  ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| querykey | 关键词检索 |
 
 
-- ### operation_record_list
+- ### campus_todaymoney_list_all
 
-` [工作台][学员][就读课程][出入班记录] ` 
+` 分校区列出指定日期的费用数据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| campus_ids_index | 实例中选择的校区列表索引，必须从中列表中选择一个。 |
+| date | 日期 |
 
 
-- ### order
+- ### card_list_all
 
-` [收银管理/订单管理] ` 
+` 列出所有课程卡 ` 
 
 | Parameter | Description |
 |-----------|-------------|
 
 
-- ### order_info
+- ### charge_detail_list_daterange
 
-` [收银管理/订单管理/订单详情] ` 
+` :param startdate: YY-MM-DD ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| enddate | YY-MM-DD |
 
 
-- ### refund_order
+- ### charge_record_list_daterange
 
-` [收银管理/订单管理/退费] ` 
+` :param startdate: YY-MM-DD ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| enddate | YY-MM-DD |
 
 
-- ### student_attend_course
+- ### class_list_all
 
 `  ` 
 
 | Parameter | Description |
 |-----------|-------------|
 
 
-- ### student_card
-
-` 查看学员的课程卡包 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| studentid | 学生ID |
-
-
-- ### student_info
+- ### curriculum_list_all
 
-` [教务管理/学员/学员详情] ` 
+` 列出全部课程[最大9999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| studentid | 学生ID |
 
 
-- ### student_list
+- ### curriculum_query
 
-` [教务管理/学员] ` 
+` 查询所有在开的课程 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| curriculumids | 课程筛选 |
-| classids | 班级筛选 |
-| name | 姓名查询关键字 |
-| status | 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员 |
-| class_student_status | 0>不筛选 1>未入班 2>已入班 |
+| searchname | 查找关键字。 |
+| haltsalelist | 是否在售。0>在售 1>停售 |
 
 
-- ### student_suspend_course
+- ### money_list_month
 
-` 设为停课状态。 ` 
+` :param yy_mm: 月份，格式示例： 2023-02 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| student_id | 学生ID |
-| suspend_course_date | 停课时间。0000-00-00 |
-| remove_class | 是否从班级中移除 |
 
 
-- ### update_curriculum_price_item
+- ### order_item_list_all
 
-` 查询所有在开的课程 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| searchname | 查找关键字。 |
-| haltsalelist | 是否在售。0>在售 1>停售 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-## Web
-
-- ### find_course_sign_charge
+- ### payment_item_list_all
 
-` 查询课消记录 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| sort_field | 时间筛选模式。 <operationTime> - 操作时间 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-- ### find_order_item_all
+- ### payment_record_list_all
 
-` 查询订单明细。 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| starttime | 起始时间 |
-| endtime | 结束时间 |
-| orderstatus | 订单状态。 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-- ### find_payment_list
+- ### payment_refund_list_all
 
-` 收入明细报表。 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| group_no | 收据编号 |
-| pay_start_date | 支付起始时间 |
-| pay_end_date | 支付结束时间 |
-| order_status | 订单状态 1>已付款 4>已作废 |
-| page_num | 页数 |
-| page_size | 每页项目数 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-- ### find_receipt
+- ### renew_cookie
 
-` 收据。 ` 
+` 刷新 cookie.tmp 配置中存储的 cookie ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| order_id | 订单 ID |
-| payment_group_id | 支付 ID |
 
 
-- ### find_student_course_amount
+- ### renew_token
 
-` 取得所有学员的课时统计数据。 ` 
+` 刷新 token.tmp 配置中存储的 token ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
 
 
-- ### find_student_course_fee
+- ### request
 
-` 取得所有学员的课时统计数据。 ` 
+`  ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| student_name | 学员姓名。 |
-| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
-| display_history | 是否显示曾就读。<True:显示><False:不显示> |
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
 
 
-- ### receipt
+- ### student_listall
 
-` 收据。 ` 
+` 列出全部学生[最大99999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| order_id | 订单 ID |
-| payment_group_id | 支付 ID |
 
 
-- ### snap_info_by_payment_group_id
+- ### student_query
 
-` 收据。 ` 
+` [教务管理/学员] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| order_id | 订单 ID |
-| payment_group_id | 支付 ID |
+| size | 项目数量 |
+| curriculumids | 课程筛选 |
+| classids | 班级筛选 |
+| name | 姓名查询关键字 |
+| status | 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员 |
+| class_student_status | 0>不筛选 1>未入班 2>已入班 |
 
 
-- ### student_course_card
+- ### teacher_list_all
 
-` 取得所有学员的课程卡片。 ` 
+` 列出全部老师<MAX-9999> ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
 
 
-- ### teacher_arrange
+- ### teacher_query
 
-` 取得指定老师的课表。 ` 
+` :return: ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| teacher_id | 查询的老师ID |
-| start_date | 起始日期，默认为本周一 |
-| end_date | 结束日期，默认为本周日 |
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
```

### Comparing `yunxiao-0.2.2/pyproject.toml` & `yunxiao-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.2.2"
+version = "0.2.3"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
```

### Comparing `yunxiao-0.2.2/yunxiao/app.py` & `yunxiao-0.2.3/yunxiao/app.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.2/yunxiao/v2.py` & `yunxiao-0.2.3/yunxiao/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -462,10 +462,22 @@
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": 1, "pageSize": 100000},
                 "campusIds": self.campus,
                 "displayHistory": True
             }
         )["data"]
 
+    # 列出所有招生来源选项
+    def student_comefrom_select_item_list(self):
+        return self.request(
+            method="get",
+            url=f"https://yunxiao.xiaogj.com/api/cs-crm/customField/get",
+            params={"_t_": UsedTime.stamp, "customFieldId": "26118419"}
+        )["data"]["selectItemList"]
 
-if __name__ == "__main__":
-    logging.basicConfig(level="INFO")
+    # 列出所有公立年级选项
+    def student_grade_select_item_list(self):
+        return self.request(
+            method="get",
+            url=f"https://yunxiao.xiaogj.com/api/cs-crm/customField/get",
+            params={"_t_": UsedTime.stamp, "customFieldId": "26118418"}
+        )["data"]["selectItemList"]
```

### Comparing `yunxiao-0.2.2/yunxiao/web.py` & `yunxiao-0.2.3/yunxiao/web.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.2/yunxiao/yunxiao.py` & `yunxiao-0.2.3/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.2/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.2.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-Metadata-Version: 2.1
-Name: yunxiao
-Version: 0.2.2
-Summary: An API SDK tool for Cloud School Education Institution Management System.
-Author-email: YiZixuan <admin@sqkkyzx.com>
-License: GPL-3.0-only
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # YunXiao API
 An API tool for YunXiao Education Institution Management System.
 
 
 # Copyright Statement
 YunXiao software is owned by XiaoGuanJia. This project is for learning purposes only. If there is any infringement, please contact me to delete.
 
 
 # Contact
 admin@sqkkyzx.com
 
 
 # API Endpoint
+
 ## App
 
 - ### arrange
 
 ` 排课管理。 ` 
 
 | Parameter | Description |
@@ -191,14 +180,22 @@
 ` 查询老师 ` 
 
 | Parameter | Description |
 |-----------|-------------|
 | querykey | 关键词检索 |
 
 
+- ### list_campus
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
 - ### operation_record_list
 
 ` [工作台][学员][就读课程][出入班记录] ` 
 
 | Parameter | Description |
 |-----------|-------------|
 | campus_ids_index | 实例中选择的校区列表索引，必须从中列表中选择一个。 |
@@ -206,14 +203,19 @@
 
 - ### order
 
 ` [收银管理/订单管理] ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| ordertype | 订单类型 |
+| searchname | 查询姓名 |
+| starttime | 起始时间 |
+| endtime | 截至时间 |
+| pagesize | 每页数量 |
 
 
 - ### order_info
 
 ` [收银管理/订单管理/订单详情] ` 
 
 | Parameter | Description |
@@ -222,14 +224,42 @@
 
 - ### refund_order
 
 ` [收银管理/订单管理/退费] ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| searchname | 查询姓名 |
+| starttime | 起始时间 |
+| endtime | 结束时间 |
+| pagesize | 项目数 |
+
+
+- ### renew_cookie
+
+` 刷新 cookie.tmp 配置中存储的 cookie ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### renew_token
+
+` 刷新 token.tmp 配置中存储的 token ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
+- ### request
+
+`  ` 
+
+| Parameter | Description |
+|-----------|-------------|
 
 
 - ### student_attend_course
 
 `  ` 
 
 | Parameter | Description |
@@ -274,14 +304,22 @@
 | Parameter | Description |
 |-----------|-------------|
 | student_id | 学生ID |
 | suspend_course_date | 停课时间。0000-00-00 |
 | remove_class | 是否从班级中移除 |
 
 
+- ### update_curriculum_price_item
+
+` ⚠ 编辑课程，谨慎使用 ` 
+
+| Parameter | Description |
+|-----------|-------------|
+
+
 ## Web
 
 - ### find_course_sign_charge
 
 ` 查询课消记录 ` 
 
 | Parameter | Description |
@@ -296,429 +334,337 @@
 | Parameter | Description |
 |-----------|-------------|
 | starttime | 起始时间 |
 | endtime | 结束时间 |
 | orderstatus | 订单状态。 |
 
 
-- ### find_student_course_amount
+- ### find_payment_list
 
-` 取得所有学员的课时统计数据。 ` 
+` 收入明细报表。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
+| group_no | 收据编号 |
+| pay_start_date | 支付起始时间 |
+| pay_end_date | 支付结束时间 |
+| order_status | 订单状态 1>已付款 4>已作废 |
+| page_num | 页数 |
+| page_size | 每页项目数 |
 
 
-- ### find_student_course_fee
+- ### find_receipt
 
-` 取得所有学员的课时统计数据。 ` 
+` 收据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| student_name | 学员姓名。 |
-| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
-| display_history | 是否显示曾就读。<True:显示><False:不显示> |
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
 
 
-- ### student_course_card
+- ### find_student_course_amount
 
-` 取得所有学员的课程卡片。 ` 
+` 取得所有学员的课时统计数据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
 | page_num | 页数。 |
 | page_size | 每页记录数。 |
 
 
-- ### teacher_arrange
+- ### find_student_course_fee
 
-` 取得指定老师的课表。 ` 
+` 取得所有学员的课时统计数据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| teacher_id | 查询的老师ID |
-| start_date | 起始日期，默认为本周一 |
-| end_date | 结束日期，默认为本周日 |
+| student_name | 学员姓名。 |
+| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
+| display_history | 是否显示曾就读。<True:显示><False:不显示> |
 | page_num | 页数。 |
 | page_size | 每页记录数。 |
 
 
-## App
-
-- ### arrange
+- ### receipt
 
-` 排课管理。 ` 
+` 收据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| starttime | 查询起始时间 |
-| endtime | 查询截止时间 |
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
 
 
-- ### become_history
+- ### renew_cookie
 
-` 设为曾就读学生。 ` 
+` 刷新 cookie.tmp 配置中存储的 cookie ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| studentlist | 学生ID |
 
 
-- ### class_arrange
+- ### renew_token
 
-` 查询指定班级排课。 ` 
+` 刷新 token.tmp 配置中存储的 token ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| classid | 班级id |
-
 
-- ### class_info
 
-` 查询指定班级信息 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| classid | 班级id |
-
-
-- ### class_info_page
+- ### request
 
 `  ` 
 
 | Parameter | Description |
 |-----------|-------------|
 
 
-- ### class_student
-
-` 查询指定班级的学员 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| classid |     班级id |
-| inout |       [1]当前在班学员 [2]历史学员 |
-
-
-- ### company_course
-
-` [教务管理/课表点名/全部课表] ` 
-
-| Parameter | Description |
-|-----------|-------------|
-
-
-- ### course_absent
-
-` [教务管理/缺勤管理] ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| starttime | 起始时间 |
-| endtime | 结束时间 |
-| pagesize | 单页项目数量 |
-
-
-- ### curriculum
-
-` 查询所有在开的课程 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| searchname | 查找关键字。 |
-| haltsalelist | 是否在售。0>在售 1>停售 |
-
-
-- ### find_course_money
+- ### snap_info_by_payment_group_id
 
-` 课消数据。 ` 
+` 收据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 月份，格式示例： 2023-02 |
+| order_id | 订单 ID |
+| payment_group_id | 支付 ID |
 
 
-- ### find_data_report
+- ### student_course_card
 
-` 每日简报。 ` 
+` 取得所有学员的课程卡片。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 日期，格式示例 2023-02-01 |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
 
 
-- ### find_data_report_list
+- ### teacher_arrange
 
-` 某日到某日数据。 ` 
+` 取得指定老师的课表。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| startdate | 起始日期 |
-| enddate | 截至日期 |
-
-
-- ### find_now_data_report
-
-` [数据/当前数据] ` 
+| teacher_id | 查询的老师ID |
+| start_date | 起始日期，默认为本周一 |
+| end_date | 结束日期，默认为本周日 |
+| page_num | 页数。 |
+| page_size | 每页记录数。 |
 
-| Parameter | Description |
-|-----------|-------------|
 
+## V2
 
-- ### find_refund_money
+- ### arrange_list_date
 
-` 学费退费数据 ` 
+` 列出日期范围全部排课[最大9999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 月份，格式示例： 2023-02 |
 
 
-- ### find_student_course_amount
+- ### arrange_list_daterange
 
-` 学生数据 - 课时报表。 ` 
+` 列出全部排课[最大99999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| curriculumids | 课程ID列表 |
-| status | 学生状态列表 |
-| studentname | 按学生姓名检索 |
 
 
-- ### find_student_course_fee
+- ### arrange_queery_date
 
-` 学生数据 - 费用报表。 ` 
+` ⚠ 未完成，无法使用 查询指定日期排课 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| curriculumids | 课程ID列表 |
-| status | 学生状态列表 |
-| studentname | 按学生姓名检索 |
 
 
-- ### find_tuition
+- ### arrange_query_daterange
 
-` 学费收入数据。 ` 
+` 排课管理。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| date | 月份，格式示例： 2023-02 |
+| displayCompletedClass | 显示已结班排课 |
+| starttime | 查询起始时间 |
+| endtime | 查询截止时间 |
 
 
-- ### get_teacher_list
+- ### campus_list_all
 
-` 查询老师 ` 
+`  ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| querykey | 关键词检索 |
 
 
-- ### operation_record_list
+- ### campus_todaymoney_list_all
 
-` [工作台][学员][就读课程][出入班记录] ` 
+` 分校区列出指定日期的费用数据。 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| campus_ids_index | 实例中选择的校区列表索引，必须从中列表中选择一个。 |
+| date | 日期 |
 
 
-- ### order
+- ### card_list_all
 
-` [收银管理/订单管理] ` 
+` 列出所有课程卡 ` 
 
 | Parameter | Description |
 |-----------|-------------|
 
 
-- ### order_info
+- ### charge_detail_list_daterange
 
-` [收银管理/订单管理/订单详情] ` 
+` :param startdate: YY-MM-DD ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| enddate | YY-MM-DD |
 
 
-- ### refund_order
+- ### charge_record_list_daterange
 
-` [收银管理/订单管理/退费] ` 
+` :param startdate: YY-MM-DD ` 
 
 | Parameter | Description |
 |-----------|-------------|
+| enddate | YY-MM-DD |
 
 
-- ### student_attend_course
+- ### class_list_all
 
 `  ` 
 
 | Parameter | Description |
 |-----------|-------------|
 
 
-- ### student_card
-
-` 查看学员的课程卡包 ` 
-
-| Parameter | Description |
-|-----------|-------------|
-| studentid | 学生ID |
-
-
-- ### student_info
+- ### curriculum_list_all
 
-` [教务管理/学员/学员详情] ` 
+` 列出全部课程[最大9999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| studentid | 学生ID |
 
 
-- ### student_list
+- ### curriculum_query
 
-` [教务管理/学员] ` 
+` 查询所有在开的课程 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| curriculumids | 课程筛选 |
-| classids | 班级筛选 |
-| name | 姓名查询关键字 |
-| status | 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员 |
-| class_student_status | 0>不筛选 1>未入班 2>已入班 |
+| searchname | 查找关键字。 |
+| haltsalelist | 是否在售。0>在售 1>停售 |
 
 
-- ### student_suspend_course
+- ### money_list_month
 
-` 设为停课状态。 ` 
+` :param yy_mm: 月份，格式示例： 2023-02 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| student_id | 学生ID |
-| suspend_course_date | 停课时间。0000-00-00 |
-| remove_class | 是否从班级中移除 |
 
 
-- ### update_curriculum_price_item
+- ### order_item_list_all
 
-` 查询所有在开的课程 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| searchname | 查找关键字。 |
-| haltsalelist | 是否在售。0>在售 1>停售 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-## Web
+- ### payment_item_list_all
 
-- ### find_course_sign_charge
-
-` 查询课消记录 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| sort_field | 时间筛选模式。 <operationTime> - 操作时间 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-- ### find_order_item_all
+- ### payment_record_list_all
 
-` 查询订单明细。 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| starttime | 起始时间 |
-| endtime | 结束时间 |
-| orderstatus | 订单状态。 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-- ### find_payment_list
+- ### payment_refund_list_all
 
-` 收入明细报表。 ` 
+` 列出指定操作日期范围的所有订单记录 ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| group_no | 收据编号 |
-| pay_start_date | 支付起始时间 |
-| pay_end_date | 支付结束时间 |
-| order_status | 订单状态 1>已付款 4>已作废 |
-| page_num | 页数 |
-| page_size | 每页项目数 |
+| enddate | YY-MM-DD |
+| startdate | YY-MM-DD |
 
 
-- ### find_receipt
+- ### renew_cookie
 
-` 收据。 ` 
+` 刷新 cookie.tmp 配置中存储的 cookie ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| order_id | 订单 ID |
-| payment_group_id | 支付 ID |
 
 
-- ### find_student_course_amount
+- ### renew_token
 
-` 取得所有学员的课时统计数据。 ` 
+` 刷新 token.tmp 配置中存储的 token ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
 
 
-- ### find_student_course_fee
+- ### request
 
-` 取得所有学员的课时统计数据。 ` 
+`  ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| student_name | 学员姓名。 |
-| status | 学员状态。[0:"未收费"][1:"在读"][7:"停课"] |
-| display_history | 是否显示曾就读。<True:显示><False:不显示> |
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
 
 
-- ### receipt
+- ### student_listall
 
-` 收据。 ` 
+` 列出全部学生[最大99999条] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| order_id | 订单 ID |
-| payment_group_id | 支付 ID |
 
 
-- ### snap_info_by_payment_group_id
+- ### student_query
 
-` 收据。 ` 
+` [教务管理/学员] ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| order_id | 订单 ID |
-| payment_group_id | 支付 ID |
+| size | 项目数量 |
+| curriculumids | 课程筛选 |
+| classids | 班级筛选 |
+| name | 姓名查询关键字 |
+| status | 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员 |
+| class_student_status | 0>不筛选 1>未入班 2>已入班 |
 
 
-- ### student_course_card
+- ### teacher_list_all
 
-` 取得所有学员的课程卡片。 ` 
+` 列出全部老师<MAX-9999> ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
 
 
-- ### teacher_arrange
+- ### teacher_query
 
-` 取得指定老师的课表。 ` 
+` :return: ` 
 
 | Parameter | Description |
 |-----------|-------------|
-| teacher_id | 查询的老师ID |
-| start_date | 起始日期，默认为本周一 |
-| end_date | 结束日期，默认为本周日 |
-| page_num | 页数。 |
-| page_size | 每页记录数。 |
```

