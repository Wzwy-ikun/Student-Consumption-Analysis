🌟 高校学生消费行为分析项目（Python + Excel + Tableau）

A Student Consumption Analytics Dashboard Project

📌 项目简介（Project Overview）

本项目基于模拟的高校学生信息与消费流水数据，构建一个完整的数据分析流程，包括：

数据生成与预处理（Python）

数据清洗与结构化（Excel）

关系构建与可视化分析（Tableau）

交互式仪表板（Dashboard）

关键洞察总结

通过分析不同年级、不同专业与不同消费类型的行为模式，本项目试图探索校园内的主要消费趋势，辅助管理者、商家与研究人员理解学生消费习惯。
## 📁 项目结构（Repository Structure）

```text
Student-Consumption-Analysis/
│── README.md                 # 项目说明文件（当前文件）
│── Data/
│     ├── students_clean.csv       # 学生基础信息
│     └── transactions_clean.csv   # 消费流水明细
│── Code/
│     └── generate_data.py         # Python 数据生成脚本
│── Visualizations/
│     ├── dashboard.png            # Tableau 仪表板截图
│     └── cover.png                # 项目封面图
│── Report/
│     └── 高校学生消费行为分析报告.docx  # 完整版项目报告
│── Supplement/
      └── vlookup_notes.txt        # Excel 字段补全说明

##🧵 数据说明（Data Description）
1. Students（学生表）
字段	含义
student_id	学号
gender	性别
age	年龄
grade	年级（1~4 对应大一~大四）
major	专业名称
family_income	家庭收入（区间随机）

共 300 条记录

2. Transactions（消费流水表）
字段	含义
trans_id	交易编号
student_id	学号（外键）
amount	金额
category	消费类别（饮料/超市/餐饮等）
pay_method	支付方式（微信/支付宝）
time	时间（含日期与具体时间）
location	地点

共 37,644 条交易记录

🛠️ 使用到的工具（Tech Stack）
数据生成与预处理

Python（Pandas、Numpy、Datetime）

数据清洗

Microsoft Excel
（缺失值检查、字段分列、VLOOKUP 字段补全、格式标准化）

可视化

Tableau Public
（关系模型构建、饼图、柱状图、筛选器、仪表板设计）

📊 仪表板展示（Dashboard Preview）
🎨 项目封面图（Cover）
<img src="Visualizations/cover.png" width="600"/>
📈 Tableau 仪表板（Dashboard）
<img src="Visualizations/dashboard.png" width="900"/>

👉 如果你有 Tableau Public 链接，可以贴在这里：

Tableau Dashboard Online View:
https://public.tableau.com/xxxxxxxxxxx

🔍 分析结论（Key Insights）
1. 消费结构较为均衡

饮料、餐饮、生活服务、文具等类别占比接近，说明学生消费结构相对稳定。

2. 年级消费差异明显

大四学生消费金额最高

大二学生较为节制
推测与社团活动、课程材料与生活习惯有关。

3. 不同专业差异存在

金融、电子信息、工商管理消费更高

计算机类学生支出相对较低

可能与课程性质、学习模式、组织活动相关。

🧭 项目流程（Workflow）
1️⃣ 数据生成

使用 Python 生成模拟学生信息和相应消费记录。

2️⃣ 数据清洗

Excel 检查缺失值、字段格式、异常值处理，补充字段（Month、Weekday、Date）。

3️⃣ 关联建模

Tableau 建立学生表与消费表的多对一关系。

4️⃣ 可视化

创建如下图表：

消费类别占比饼图

按年级消费金额柱状图

按专业消费金额柱状图

并加入筛选器形成交互分析仪表板。

5️⃣ 洞察总结

输出项目报告（docx）。

📝 项目报告（Report）

完整报告文档：
👉 Report/高校学生消费行为分析报告.docx

内容包括：

项目背景

数据获取

数据清洗

可视化结果

分析结论

建议与扩展方向
🚀 如何复现项目（How to Reproduce）
git clone https://github.com/
Wzwy-ikun/Student-Consumption-Analysis
cd Student-Consumption-Analysis
1. 生成数据（可选）
python Code/generate_data.py
2. 打开 Excel 查看清洗流程

打开 Data 文件夹查看 CSV 文件。

3. 打开 Tableau

导入 Data 文件夹的两个 CSV
按照 README 的截图即可复现仪表板。

🎯 适用场景（Use Cases）

数据分析作品集

数据分析师面试展示

数据可视化课程作业

BI 工具学习实践

论文/课题数据示例

👤 作者（Author）

王智帏杨
Data Analyst | Python | SQL | Excel | Tableau
欢迎交流！

⭐ 如果你觉得这个项目不错，可以点个 Star 支持一下！
