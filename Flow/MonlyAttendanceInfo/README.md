English | MonlyattendanceInfo Flow
📌 Flow Type
Scheduled Cloud Flow — Runs on the 3rd day of every month

📋 Description
This Power Automate Flow automatically collects and aggregates employee attendance data from multiple SharePoint lists, then compiles a monthly summary sheet used by HR and payroll for salary calculations.

📊 Output Fields
Name (名前)

Total Working Hours (総工時)

Weekend Overtime (週末残業)

Commuter Pass Cost (定期券費用)

Commuter Route Info (定期区間)

Leave Type (休暇種別)

Leave Days (休暇日数)

⚙️ Main Features
🗂️ Automatically extracts data from multiple SharePoint lists

📆 Compiles employee working hours by converting from daily records to total hours

🌴 Introduces leave type classification, converting hours to leave days

📤 Generates a monthly output file or list used by HR

⚠️ Challenges
⏱️ Converting daily records to total hours — Workdays must be accurately converted, especially part-time cases

📉 Leave type processing — The system must:

Identify which type of leave (e.g. vacation, sick, personal)

Convert hours to days (rounding rules: e.g. 4 hours → 0.5 days)

Avoid rounding errors for partial leaves

🗃️ Multi-source integration — Merging multiple SharePoint lists with different structures

🔐 Access Control — Ensuring flow permissions cover all SharePoint sources

🚀 How to Use
Import the Flow zip file: MonlyattendanceInfo_*.zip

Reconnect your SharePoint lists as data sources

Schedule the flow to run monthly on the 3rd

Output can be saved to Excel Online, Dataverse, or a SharePoint report list

--------------------------------------------------------------------------------

中文 | MonlyattendanceInfo 出勤整合流程
📌 流程类型
定时云流 — 每月 3 日自动执行

📋 功能说明
该流程从多个 SharePoint 列表中提取员工出勤数据，计算整合后，生成用于 HR 发薪参考的 月度总表。

📊 输出字段
员工姓名

总工时

周末加班时数

定期券费用

定期通勤区间

休假种类

休假日数

⚙️ 功能亮点
自动抓取多个 SharePoint 表格的数据

将每天的打卡或工时数据转换为整月总工时

新增休假种类字段，根据休假类型转换小时为休假“日数”

输出一份 HR 可直接使用的月度考勤表

⚠️ 实现难点
⏱️ 总工时换算 — 需要将“出勤天数”或“打卡时间”换算成小时，处理早退、迟到等异常情况

🌴 休假种类解析：

需要区分各种类型的休假（如带薪休假、病假、特休等）

每种休假记录以小时为单位，需要换算为天（按规则四舍五入，如 4 小时 = 0.5 天）

🗃️ 多个数据源整合 — 各个 SharePoint 表字段命名、结构不同，需统一合并

🔐 权限处理 — 需要流程对多个 SharePoint 列表有读取权限

🚀 使用方式
导入 MonlyattendanceInfo_*.zip 文件

重新连接你的 SharePoint 数据源

设定每月 3 日运行

输出可为 Excel Online 文件、Dataverse 表，或 SharePoint 目标列表

--------------------------------------------------------------------------------

日本語 | MonlyattendanceInfo 勤怠集計フロー
📌 フロータイプ
スケジュール型クラウドフロー — 毎月 3日 に実行

📋 説明
この Power Automate フローは、複数の SharePoint リスト から従業員の出勤データを自動収集し、HR・給与計算向けの月次勤怠サマリーを作成します。

📊 出力項目
名前

総工時

週末残業時間

定期券費用

定期区間情報

休暇種別

休暇日数

⚙️ 主な機能
SharePoint リストから自動取得・集計

毎日の勤務データを 時間単位で換算

休暇の種類を明確化し、時間 → 日数の換算（例：4時間→0.5日）

HR 向けにレポートとして出力

⚠️ 課題点
⏱️ 工時換算の精度 — 勤務日数・時間を正確に合算（早退・遅刻も考慮）

🌴 休暇の処理：

休暇の種類を判別（有給、病欠、特別休暇など）

時間を日数に変換（0.5日の四捨五入処理を含む）

🗃️ 複数リスト統合 — 異なるリストの構造・項目名の統一

🔐 アクセス設定 — すべてのリストにアクセスする権限が必要

🚀 利用手順
Flow の zip ファイル（MonlyattendanceInfo_*.zip）をインポート

データソース（SharePoint）を再接続

スケジュールを毎月3日に設定

出力ファイルは Excel、Dataverse、または SharePoint リストに保存可能

