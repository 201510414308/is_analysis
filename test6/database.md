
## <center>Student_form</center>
| 字段  | 类型 | 主键、外键 | 可以为空 |默认值| 约束 | 说明 |
|  :---:  | :---:  |  :---:   |  :-----------:   | :---:  | :---: | :---: |
|Stu_Number|NUMBER(16,0) |主键|否|无|无|学生学号|
|Stu_Name|varchar(20byte)|无|否|无|无|学生姓名|
|User_Id|varchar(20byte)|外键|否|无|无|学生的用户ID|
|Class|VARCHAR(8,0)|无|否|无|无|班级号|
|Github_Username|VARCHAR(20 BYTE)|无|否|无|无|Github用户名|
|Password|varchar(20byte)|无|否|无|无|密码|
|Disable|varchar(10byte)|无|否|无|无|是否禁用|
## <center>Teacher_form</center>
| 字段  | 类型 | 主键、外键 | 可以为空 |默认值| 约束 | 说明 |
| :---:  | :---:  |  :---:     |   :---------:   | :---: | :---: |:---: |
|Tea_Number|NUMBER(16,0)|主键|否|无|无|教师编号|
|User_Id|NUMBER(26,0)|外键|否|无|无|教师的用户ID|
|Tea_Name|varchar(24byte)|无|否|无|无|教师姓名|
|department  |varchar(32byte)|无|否|无|无|教师所在部门|


## <center>Grade_form</center>
| 字段  | 类型 | 主键、外键 | 可以为空 |默认值| 约束 | 说明 |
|:---:    | :---:  |    :---:     |   :---------:   | :---:   | :---: | :---: |
|Stu_Number|NUMBER(16,0)|主键、Student_form外键|否|无|无|学生学号|
|Test_Id|varchar(32byte)|无|否|无|无|实验编号|
|result | float|无|否|无|无|成绩分数|
|memo   |varchar(400byte)|无|否|无|无|评价|
|update_date|Date|无|否|无|无|成绩修改时间|

## <center>Course_form</center>
| 字段  | 类型 | 主键、外键 | 可以为空 |默认值| 约束 | 说明 |
|:---:    | :---:  |    :---:     |   :---------:   | :---:   | :---: | :---: |
|Cou_Id|NUMBER(8,0)|主键|否|无|无|课程编号|
|Stu_Number/NUMBER(16,0)|外键|否|无|无|学生编号|
|Tea_Number/NUMBER(16,0)|外键|否|无|无|教师编号|
|Cou_Name|varchar(20,0)|外键|否|无|无|课程名称|




## <center>Terms_form</center>
| 字段  | 类型 | 主键、外键 | 可以为空 |默认值| 约束 | 说明 |
|:---:    | :---:  |    :---:     |   :---------:   | :---:   | :---: | :---: |
|Term_Id|NUMBER(16,0)|主键|否|无|无|学期编号|
|Stu_Number/NUMBER(16,0)|外键|否|无|无|学生编号|
|Tea_Number/NUMBER(16,0)|外键|否|无|无|教师编号|
