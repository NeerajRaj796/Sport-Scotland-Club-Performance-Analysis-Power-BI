📊 **CASE STUDY**
**Scotland Membership/Club Performance Dashboard**


Author: Neeraj Raj Srinivasa Raju
Tool: Microsoft Power BI | DAX | Power Query
Data Source: sportscotland Public Club Dataset (2023–2025)

This case study follows the structured data lifecycle:

Ask → Prepare → Process → Analyze → Share → Act

**Dashboard Structure:**

![Club Members – Year-on-Year Performance](Club-Members-Page.png)

![Participants – Year-on-Year Performance](Participants-Page.png)

![Coaches, Capacity & Location – Year-on-Year Analysis](Coaches-Page.png)

**Scenario**


Sportscotland works in partnership with Scottish Governing Bodies to increase participation in sport across Scotland. To support this objective, annual data is collected on club membership, participants, and coaches across multiple local authorities.

The dataset analysed in this project covers three reporting years (2023–2025) and includes 81,000 registered members, 51,000 participants, and 889 active coaches across more than 200 clubs.

The purpose of this analysis was not simply to visualise totals, but to evaluate sustainability. Specifically, the goal was to determine whether growth in engagement is being supported by sufficient and appropriately distributed coaching capacity.

The central strategic question guiding the analysis was:

Is sport participation growing sustainably, and is coaching capacity aligned to support that growth across Scotland?

1️⃣**Ask**

To answer this overarching question, the analysis was structured around five operational objectives.

First, I needed to determine whether formal membership is growing year-on-year and whether that growth is significant.

Second, I assessed whether participation — which often acts as a pipeline into membership — is stable or volatile.

Third, I examined whether the coaching workforce is expanding at a rate that matches demand growth.

Fourth, I evaluated demographic balance, particularly gender representation across membership and coaching.

Finally, I assessed geographic distribution to identify regional disparities in engagement and workforce supply.

Each of these areas directly influences funding decisions, workforce planning, and long-term development strategy.

2️⃣**Prepare**

Before building the dashboard, I defined clear baseline performance indicators to anchor the analysis.

Total membership stands at 81,000, with a year-on-year growth rate of 13.93%. Adult members account for 51,000, while youth members account for 30,000 — representing 37% of the total membership base. Female members make up approximately 38,000, or 47% of total members.

Participation totals 51,000 individuals across the three-year period.

The coaching workforce consists of 889 coaches, with 53% qualified and 28% female representation. Coaching growth year-on-year is 1.91%.

When calculated as a capacity ratio, there is approximately one coach per 91 members.

Defining these metrics early ensured that every calculation later in the process was aligned to answering sustainability and workforce alignment questions.

3️⃣**Process**

The dataset required structural cleaning and validation before meaningful analysis could begin.

Duplicate headers were removed and data types were standardised. Membership splits were validated to ensure that adult plus youth totals reconciled with overall membership totals. Similarly, male and female totals were checked for consistency.

A star schema model was implemented to support scalable analysis. Separate fact tables were created for Members, Participants, and Coaches. These were connected through shared dimensions including Club, Local Authority, and Year.

Advanced DAX measures were developed using CALCULATE and FILTER to compute dynamic year-on-year comparisons. DIVIDE was used to ensure safe ratio calculations, and structured VAR/RETURN logic improved clarity and maintainability.

This modelling approach ensured that insights remained accurate even when filtered by region or year.

4️⃣**Analyze**


**Membership – Growth and Structural Stability**

Membership currently stands at 81,000 and is growing at 13.93% year-on-year. This indicates strong engagement growth across Scotland.

However, headline growth does not automatically imply sustainability. The composition of that growth is equally important.

Youth members account for 30,000 individuals, representing 37% of total membership. This indicates that growth is not limited to adult recreational engagement but includes a significant youth development pipeline.

Female membership stands at approximately 47%, suggesting near-balanced representation at the participation level.

When examining club-level performance, however, growth appears concentrated. For example, Club C19 shows approximately 4.9K growth, while several clubs remain below 3K. This suggests dependency on high-performing clubs.

From a strategic perspective, this means that while overall membership is increasing, resilience may be limited if mid-performing clubs do not improve.

Participation – Engagement Volatility and Future Risk

Participation totals 51,000 across the reporting period.

However, the trend analysis reveals instability. Participation fell from 22.8K in 2023 to 10.8K in 2024 — a decline of approximately 12,000 individuals — before partially recovering to 17.5K in 2025.

This volatility introduces risk. Participation often precedes membership. If engagement fluctuates significantly, long-term membership growth may become inconsistent.

Demographically, participation is balanced, with youth participation at 46% and female participation at 45%. This suggests that inclusion efforts at the participation level are effective.

Geographically, however, participation is concentrated in specific authorities. Edinburgh accounts for approximately 13K participants, and Glasgow accounts for around 9K. Several authorities report minimal engagement.

This indicates uneven regional access or programme reach.

From a strategic standpoint, stabilising participation and reducing regional inequality should be prioritised to protect long-term membership growth.

Coaching Capacity – Alignment and Structural Risk

The most significant finding emerges from the workforce analysis.

Total coaches number 889, with year-on-year growth of only 1.91%.

When compared to membership growth of 13.93%, a widening capacity gap becomes clear.

With 81,000 members supported by 889 coaches, the ratio equates to approximately 91 members per coach. If membership continues to grow at current rates without proportional coaching expansion, this ratio will increase further.

Only 53% of coaches are qualified. This suggests that nearly half of the workforce may require further development to ensure programme quality.

Gender representation presents another imbalance. Female members represent approximately 47% of total membership, yet female coaches represent only 28%. This 19 percentage point gap suggests potential barriers in coaching progression pathways.

Regionally, workforce distribution is uneven. Edinburgh has 197 coaches and Glasgow 183, while several authorities have fewer than 20. This imbalance may impact service quality and access in lower-capacity regions.

From a sustainability perspective, coaching capacity misalignment represents the most critical structural risk.

5️⃣ **Share**

The dashboard was intentionally structured across three focused pages.

The first page establishes demand through membership growth and demographic composition.

The second page evaluates engagement stability through participation trends and geographic variation.

The third page assesses supply through coaching capacity, qualification levels, and regional distribution.

This progression mirrors strategic decision-making logic: demand, pipeline, and supply.

Interactive slicers allow filtering by year and region to support scenario analysis and policy evaluation.

6️⃣**Act**

Based on the findings, several strategic actions are recommended.

First, coaching recruitment growth must increase toward 10–12% annually to align more closely with membership growth of 13.93%.

Second, the qualification rate should be improved from 53% toward at least 60% to strengthen workforce quality.

Third, female coaching development pathways should be prioritised to close the 19 percentage point gender gap.

Fourth, targeted funding should be directed toward underrepresented local authorities to rebalance workforce and participation distribution.

Finally, the 2023–2024 participation drop should be investigated to identify retention barriers and prevent future volatility.

**Final Strategic Position**

The data demonstrates that sport engagement across Scotland is expanding in scale and remains relatively inclusive at membership and participation levels.

However, coaching capacity is not growing at the same pace as demand, and regional and gender imbalances persist within the workforce.

Without intervention, workforce strain and inequality may undermine long-term sustainability.

This dashboard moves beyond descriptive reporting and provides a capacity-aligned sustainability model to support evidence-based decision-making.
