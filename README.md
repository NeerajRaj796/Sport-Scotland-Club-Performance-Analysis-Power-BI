🏅 Sport Scotland Membership, Participation & Coaching Analysis
Power BI | Advanced DAX | Public Sector Performance Analytics
📌 Project Overview

This project was undertaken as a structured analytical challenge to evaluate how sport participation is evolving across Scotland using publicly available data from sportscotland. The dataset covers a three-year period (2023–2025) and includes over 200 clubs, 81K registered members, 51K annual participants, and 889 active coaches.

The objective was to determine whether growth in membership and participation is being supported by sufficient coaching capacity, and whether engagement is balanced across demographics and geography.

Rather than presenting isolated metrics, this project integrates membership, participation, and coaching data into a single scalable Power BI model to provide a complete performance view.

🎯 Business Question

Is sport engagement growing sustainably, and is coaching capacity aligned with that growth across Scotland?

To answer this, the analysis focused on:

Total Members & Members YoY %

Total Participants & Participants trends

Total Coaches & Coaches YoY %

Female % and Youth % representation

Qualified Coaches %

Coaches-to-Members ratio

Geographic distribution by local authority

🛠 Data Preparation & Modelling

The dataset was restructured using Power Query to remove duplicate headers, standardise formats, and validate totals across adult/youth and male/female splits.

A star schema model was implemented:

Fact Tables

Members

Participants

Coaches

Dimensions

Club

Local Authority

Year

DAX measures were built using:

CALCULATE and FILTER for dynamic YoY logic

DIVIDE for safe percentage and ratio calculations

Cross-table aggregation for capacity comparisons

This ensured the dashboard supports accurate time-based performance tracking.

📊 Findings by Analytical Area

📈 Membership – Scale & Growth

![Club Members – Year-on-Year Performance](Club-Members-Page.png)

Total Membership stands at 81K, split into:

51K Adult Members

30K Youth Members

38K Female Members

45K Male Members

YoY Growth: 13.93%

Youth members represent approximately 37% of total membership (30K of 81K), indicating a strong development pipeline. Female members account for roughly 47%, showing near-balanced representation at membership level.

However, growth is not evenly distributed across clubs. For example:

Club C19 shows 4.9K growth, significantly higher than several clubs below 3K.

Interpretation

Membership growth is strong at nearly 14%, but performance concentration suggests reliance on specific high-performing clubs.

Strategic Action

Replicate best practices from top-performing clubs (e.g., C19).

Monitor clubs with flat or declining YoY % for operational support.

Maintain gender balance near current 47–50% levels.

🏃 Participation – Engagement Pipeline

![Participants – Year-on-Year Performance](Participants-Page.png)

Total Participants: 51K

28K Adult Participants

23K Youth Participants

23K Female Participants

Youth Participation: 46%

Female Participation: 45%

Participation trend:

22.8K (2023)

10.8K (2024)

17.5K (2025)

This reflects a significant drop between 2023 and 2024, followed by recovery in 2025.

Geographically:

City of Edinburgh shows ~13K participation

Glasgow City shows ~9K

Several authorities show near-zero engagement

Interpretation

Participation remains strong overall but demonstrates volatility year-on-year. Since participants represent future members, instability here may affect long-term growth.

Strategic Action

Investigate drivers of the 12K drop from 2023 to 2024.

Improve participant-to-member conversion in high-volume authorities.

Target low-engagement regions with outreach programmes.

🧑‍🏫 Coaching – Workforce Capacity & Alignment

![Coaches, Capacity & Location – Year-on-Year Analysis](Coaches-Page.png)


Total Coaches: 889
Qualified Coaches: 469
Qualified Coaches %: 53%
Female Coaches %: 28%
Coaches YoY Growth: 1.91%

Coaches-to-Members ratio: 0.01
This equates to approximately 1 coach per 91 members (81K / 889).

Regional coaching distribution:

City of Edinburgh: 197 coaches

Glasgow City: 183 coaches

Some regions: fewer than 20 coaches

Interpretation

Membership is growing at 13.93%, while coaching capacity is growing at only 1.91%. This indicates workforce growth is not keeping pace with demand.

Female representation in membership is ~47%, while female coaching stands at 28%, creating a significant gender gap.

Strategic Action

Increase coaching recruitment growth toward 10–12% annually.

Launch female coach development initiatives to close the 19% gender gap.

Improve qualification rate from 53% toward 60%+.

Rebalance workforce allocation in underrepresented local authorities.

📊 Dashboard Pages
📈 Club Members – Year-on-Year Performance

This page analyses membership growth, demographic representation, and club-level variation to assess sustainability and performance concentration.

🏃 Participants – Year-on-Year Performance

This page evaluates participation trends and demographic composition to measure engagement stability and future membership pipeline strength.

🧑‍🏫 Coaches, Capacity & Location – Year-on-Year Analysis

This page assesses workforce scale, qualification levels, gender representation, and geographic distribution to evaluate alignment between supply and demand.

📌 Final Conclusion

The analysis shows:

Membership is growing strongly (13.93%).

Participation remains substantial (51K) but volatile.

Coaching capacity growth (1.91%) is significantly lower than membership growth.

Female representation is balanced at membership level (~47%) but underrepresented in coaching (28%).

Workforce distribution varies significantly by region.

This indicates that while engagement levels are healthy, sustainable growth requires:

Workforce expansion

Improved coach qualification rates

Increased female coach recruitment

Geographic balancing of resources

Stabilisation of participation retention

By integrating scale, growth, demographics, and workforce capacity into one analytical model, this dashboard enables evidence-based strategic planning rather than reactive reporting.
