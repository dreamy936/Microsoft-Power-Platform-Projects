-----English Introduction-------
📌 Flow Name: MonlyAttendanceInfo
📋 Project Overview
This is a Microsoft Power Automate Flow designed to automatically notify employees of their monthly attendance summary via email. It helps streamline HR communication and improve transparency in attendance management.

This project serves as a practical showcase of Power Platform automation capabilities, especially suitable for HR tools or attendance notification systems.

✅ Key Features
⏰ Scheduled monthly execution (e.g., every 1st day of the month at 9:00 AM)

📤 Sends automated emails to employees

📎 Email content includes dynamic attendance data such as total workdays, late arrivals, and absences

🔗 Can connect to data sources such as SharePoint, Excel Online, Dataverse, etc.

🧩 Modular and easy to reuse in other environments

🧑‍💻 How to Use
1. Import the Flow into Power Automate
Go to Power Automate

On the left menu, click My Flows → Import

Upload the file MonlyAttendanceInfo_20250731060314.zip

Reconfigure the required connections (e.g., Outlook, SharePoint, Excel)

Set the recipient field to pull dynamically from employee email data

2. Configure the Recurrence Trigger
Recommended: Run on the 1st of every month at 9:00 AM

You can modify the frequency based on your business needs (e.g., biweekly or end-of-month)

3. Example Email Output
yaml
Copy
Edit
Subject: Your Attendance Report for This Month

Dear John,

Here is your attendance summary for July 2024:
- Days Present: 20
- Times Late: 2
- Days Absent: 1

Please contact HR if you have any questions.
🌐 Tech Stack
Technology	Purpose
Power Automate	Flow automation
Outlook Connector	Send emails
SharePoint / Excel / Dataverse	Data source

📁 Repository Structure
python
Copy
Edit
Flow/
├── MonlyAttendanceInfo_20250731060314.zip   # Exported Power Automate Flow
└── README.md                                # Project description (this file)
📈 Highlights
Built entirely via low-code, visual logic

Automates a real-world HR task with practical business value

Easy to import/export and reuse across environments

🧠 Reflections & Future Improvements
Current version uses a static email body; future upgrades could dynamically generate personalized PDF reports

Can be integrated with Power Apps to allow employees to apply for leave or view their attendance in real time





------中文简介-------
📌 Flow 名称：MonlyAttendanceInfo
📋 项目简介
本 Flow 为 Microsoft Power Automate 上开发的自动化流程，旨在每月自动向员工发送个人出勤记录通知，帮助员工及时了解自己的出勤情况，提高人事沟通效率。

本项目适合作为展示 Microsoft Power Platform 自动化技能的实际案例，适用于 HR 系统、考勤提醒系统等。

✅ 主要功能功能点
⏰ 每月定时触发（如每月 1 日上午 9:00）

📤 自动发送邮件通知给员工

📎 邮件正文中包含其当月的考勤摘要（例如：出勤天数、迟到次数、缺勤天数等）

📊 数据来源可以连接 SharePoint、Excel Online、Dataverse 或其他系统（视情况配置）

🧩 模块化设计，便于迁移或复用

🧑‍💻 使用说明
1. 导入此 Flow 到你的环境
打开 Power Automate 官网：https://flow.microsoft.com

点击左侧栏的 “My flows” → “Import”

上传 MonlyattendanceInfo_20250731060314.zip

绑定你的数据源（如 SharePoint、Outlook、Excel 文件等）

配置邮件收件人字段为动态员工邮箱

2. 配置计划触发器
建议设置为：每月1日早上9:00自动运行

可根据需要自定义频率（如：双周一次、每月最后一个工作日等）

3. 预览邮件格式（示例）：
diff
Copy
Edit
主题：您本月的出勤情况

亲爱的张三，您好！

以下是您2024年7月的出勤概况：
- 出勤天数：20天
- 迟到次数：2次
- 缺勤天数：1天

如有疑问请联系HR部门。
🌐 技术栈与平台
技术	用途
Power Automate	流程自动化
Outlook 连接器	发送邮件
SharePoint / Excel / Dataverse	考勤数据来源（可配置）

📦 文件结构说明
python
Copy
Edit
Flow/
├── MonlyattendanceInfo_20250731060314.zip   # Flow 导出文件
└── README.md                                # 项目说明文档（本文件）
📈 项目亮点
无需编码，基于图形化操作构建

实现定时邮件通知，自动化 HR 流程

易于迁移至其他环境（导出/导入即可）

🧠 项目反思（可选，用于加分）
目前是静态邮件模板，后续可接入 Power Apps 表单实现自定义请假/补签等操作

可扩展支持生成 PDF 附件发送给员工作为记录
