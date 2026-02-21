📊 CASE STUDY: Sport Scotland Membership, Participation & Coaching Dashboard

Author: Neeraj Raj Srinivasa Raju
Tool: Microsoft Power BI, DAX, Power Query, Excel
Data Source: sportscotland Public Club Dataset (2023–2025)

The case study follows the six-step data analysis lifecycle:

❓ Ask
💻 Prepare
🛠 Process
📊 Analyze
📋 Share
🎯 Act

Scenario

sportscotland collects annual data from Scottish Governing Bodies to monitor:

Club membership

Participation levels

Coaching workforce

Regional distribution

The dataset covers over:

200+ clubs

81K members

51K participants

889 coaches

The objective of this analysis was to transform raw structured datasets into an integrated Business Intelligence dashboard that identifies:

Year-on-Year membership growth

Participation stability and conversion potential

Coaching capacity alignment

Gender representation

Regional disparities

The goal was to support sustainable sport development planning across Scotland.

1️⃣ Ask

💡 Business Task:

Analyze sportscotland membership, participation, and coaching data to determine whether engagement growth is sustainable and workforce capacity is aligned.

Primary stakeholders:
Sport development planners and workforce strategy teams

Secondary stakeholders:
Regional officers and inclusion programme leads

Key Questions:

Is membership growing year-on-year?

Is participation stable or volatile?

Is coaching capacity keeping pace with membership growth?

Are there gender gaps in membership vs coaching?

Which local authorities outperform or underperform?

2️⃣ Prepare

📂 Data Source: sportscotland public reporting dataset

Time period used:
2023, 2024, 2025

Key Metrics Defined:

Total Members: 81K

YoY Membership Growth: 13.93%

Adult Members: 51K

Youth Members: 30K

Female Members: 38K (~47%)

Total Participants: 51K

Female Participants: 23K (~45%)

Total Coaches: 889

Qualified Coaches: 469 (53%)

Female Coaches: 28%

Coaches YoY Growth: 1.91%

Coaches-to-Members Ratio: ~1:91

Data Reliability Considerations:

Structured aggregated reporting

No personal identifiers

Multi-year consistency

Separate tables for Members, Participants, Coaches

Limitations:

Three-year comparison only

Aggregated club-level data

No individual tracking

3️⃣ Process
Data Cleaning Steps:

Removed duplicate headers

Standardised club names

Verified totals across adult/youth splits

Validated gender totals

Checked club-year uniqueness

Reconciled totals using Excel cross-validation

Data Model Implemented:

Star Schema:

Fact Tables:

Fact_Members

Fact_Participants

Fact_Coaches

Dimension Tables:

Dim_Club

Dim_LocalAuthority

Dim_Year

Relationships configured as one-to-many for clean filtering.

Key DAX Used:

CALCULATE()

FILTER()

DIVIDE()

SUMX()

ALL()

VAR / RETURN

This enabled dynamic YoY KPIs, demographic percentages, and capacity ratios.

4️⃣ Analyze
📌 Club Members – Year-on-Year Performance

![Club Members – Year-on-Year Performance](Club-Members-Page.png)

Membership stands at 81K, with 13.93% YoY growth.

Breakdown:

Adult: 51K

Youth: 30K (37%)

Female: 38K (~47%)

Insight:

Youth representation is strong, indicating long-term sustainability.
Female membership is near balanced.

However, growth is concentrated:

C19 shows 4.9K growth

Several clubs remain below 3K

This indicates uneven growth distribution.

📌 Participants – Engagement & Pipeline

![Participants – Year-on-Year Performance](Participants-Page.png)

Total Participants: 51K

Trend:

22.8K (2023)

10.8K (2024)

17.5K (2025)

This reflects volatility between 2023 and 2024 with partial recovery.

Demographics:

Youth Participation: 46%

Female Participation: 45%

Regional insight:

Edinburgh ~13K

Glasgow ~9K

Several areas near zero

Participation remains high overall but is unstable year-on-year.

📌 Coaches – Capacity & Alignment

![Coaches, Capacity & Location – Year-on-Year Analysis](Coaches-Page.png)


Total Coaches: 889
Coaches YoY Growth: 1.91%
Qualified Coaches: 53%
Female Coaches: 28%

Capacity Ratio:

81K Members / 889 Coaches ≈ 1 coach per 91 members

Key Observations:

Membership growth (13.93%) significantly exceeds coaching growth (1.91%).

Female membership (~47%) vs Female coaches (28%) shows a 19% representation gap.

Edinburgh (197 coaches) and Glasgow (183 coaches) dominate workforce distribution.

Several authorities have fewer than 20 coaches.

This indicates workforce imbalance and potential service pressure.

5️⃣ Share

The dashboard was structured into three core analytical pages:

Club Members – Growth & Demographics

Participants – Engagement & Regional Comparison

Coaches – Capacity & Workforce Distribution

Interactive slicers (Year, Local Authority) allow dynamic filtering.

The design prioritises clarity, KPI visibility, and benchmarking rather than decorative visuals.

Each page progresses from:

High-level KPIs → Trend → Regional breakdown → Club-level comparison

6️⃣ Act
Conclusions Based on Analysis:

📈 Membership is growing strongly (13.93%).
🏃 Participation remains substantial (51K) but volatile.
🧑‍🏫 Coaching growth (1.91%) is not keeping pace with membership growth.
👩 Female membership (~47%) significantly exceeds female coaching (28%).
🗺 Workforce and participation distribution are uneven geographically.

Strategic Recommendations:

🔹 Increase coaching recruitment growth toward 10–12% annually to match membership growth.
🔹 Develop female coaching development pathways to close the 19% gender gap.
🔹 Improve coach qualification rate from 53% toward 60%+.
🔹 Target low-engagement local authorities with outreach funding.
🔹 Investigate participation drop between 2023–2024 to improve retention.
🔹 Replicate success factors from high-growth clubs (e.g., C19).

📌 What This Demonstrates

✔ Structured BI lifecycle
✔ Clean star-schema modelling
✔ Advanced DAX implementation
✔ Capacity-based analysis (not just totals)
✔ Quantified, action-driven insights
✔ Public sector strategic alignment

📬 Contact

Neeraj Raj Srinivasa Raju
📧 neerajrajsrinivasaraju@gmail.com
