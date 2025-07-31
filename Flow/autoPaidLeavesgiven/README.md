English | AutoPaidLeavesGiven
📌 Flow Type
Scheduled Cloud Flow — Executes on the 1st day of every month

📋 Description
This Power Automate Flow automatically calculates and allocates paid leave (年休) to employees based on their entry date (start date). The logic is as follows:

🧮 Paid Leave Rules
Years of Service	Allocated Days
0.5 years	10 days
1.5 years	11 days
2.5 years	12 days
3.5 years	14 days
4.5 years	16 days
5.5 years	18 days
6.5 years or more	20 days (max)

🔧 Key Features
📆 Automatically runs every month

🧑‍💼 Processes all employees with valid start dates

🔄 Updates their available paid leave based on tenure

✅ Ensures compliance with HR policy rules

⚠️ Challenges
🔍 Precision in tenure calculation — Must account for exact 0.5-year marks (e.g., 6 months = 183 days in leap years)

🗓️ Leap year & month variations — February, leap years, etc., affect day counts

🔁 Avoid duplicate updates — Ensures the same leave isn’t added repeatedly each month

🔗 Integration with external sources — Such as SharePoint lists, Dataverse, or Excel Online

📊 Logging or audit trail — (optional) Adds logging for HR to track what leave was granted and when

🔗 How to Use
Import the Flow from autopaidleavesgiven_*.zip

Configure the data source: should include at least Name, Start Date, and Leave Balance

Schedule it to run monthly on the 1st

Test with a few dummy employee records to validate logic

----------------------------------------------------

中文 | 自动带薪年假发放流程
📌 流程类型
定时云流 — 每月 1 日自动执行

📋 功能说明
该 Power Automate 流程会根据员工的 入职日期 自动计算工龄，并按照 HR 规则 发放对应的年假天数。

🧮 发放逻辑如下：
工龄（年）	年假天数
满 0.5 年	10 天
满 1.5 年	11 天
满 2.5 年	12 天
满 3.5 年	14 天
满 4.5 年	16 天
满 5.5 年	18 天
满 6.5 年以上	20 天（封顶）

🔧 主要功能
每月定时自动运行

读取员工入职时间字段，计算当前工龄

满半年后开始发放年假

更新到现有年假字段中

⚠️ 实现难点
🔍 半年门槛判断 — 必须精确到 183 天，处理闰年及不同月份天数

⏱️ 避免重复添加 — 每月运行一次，需判断是否已发放

🗂️ 与不同数据源集成 — SharePoint 列表、Excel Online、Dataverse

🧾 权限设置 — 要有对年假字段的写入权限

📊 日志可视化（可选） — 输出日志供 HR 审核

🚀 使用方式
导入本压缩包 autopaidleavesgiven_*.zip

设置正确的数据连接（包含姓名、入职日期、年假字段）

建议设定每月 1 日自动执行

可通过测试员工记录验证功能逻辑

----------------------------------------------------
日本語 | 自動有給付与フロー
📌 フローの種類
スケジュール型クラウドフロー — 毎月 1日 に実行されます

📋 説明
この Power Automate フローは、従業員の 入社日 をもとに有給日数を自動計算し、年次有給を付与するものです。

🧮 有給日数のルール：
勤続年数	付与される有給
0.5 年	10 日
1.5 年	11 日
2.5 年	12 日
3.5 年	14 日
4.5 年	16 日
5.5 年	18 日
6.5 年以上	20 日（上限）

🔧 主な機能
毎月自動実行（定期スケジュール）

入社日をもとに勤務年数を計算

条件を満たした従業員に有給日数を付与

外部ソースとの連携も可能（SharePoint / Excel 等）

⚠️ 実装上の課題
📆 0.5年の判定精度 — 183日を正確に計算（うるう年や月ごとの変動あり）

🔁 重複更新の防止 — 同じ社員に何度も付与しないよう制御

🔗 接続の再構成が必要 — 環境ごとにデータソースや接続の再設定が必要

🔐 アクセス権限 — 有給項目を更新できる権限が必要

📝 監査ログ — HR 向けに記録を残す機能（オプション）

🧪 使用方法
Flow をインポート（zip ファイル）

「名前」「入社日」「有給日数」などのカラムを含むデータソースを接続

スケジュール設定（例：毎月1日 午前9時）

テスト用従業員で動作確認を推奨
