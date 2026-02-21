📊 CASE STUDY
Sport Scotland Membership, Participation & Coaching Sustainability Analysis

Author: Neeraj Raj Srinivasa Raju
Tool: Microsoft Power BI | DAX | Power Query
Data Source: sportscotland Public Club Dataset (2023–2025)

This analysis follows the structured data lifecycle:

❓ Ask → 💻 Prepare → 🛠 Process → 📊 Analyze → 📋 Share → 🎯 Act

Scenario

sportscotland’s core objective is to increase participation in sport across Scotland while ensuring that growth is inclusive, sustainable, and regionally balanced.

To support this objective, data is collected annually from Scottish Governing Bodies covering:

• Club Membership
• Participants (non-members engaging in sport)
• Coaching Workforce
• Local Authority distribution

The dataset analysed includes:

81,000 formal club members

51,000 participants

889 coaches

200+ clubs

Multiple Scottish local authorities

Three reporting years (2023–2025)

The critical strategic concern was not simply whether participation exists — but whether growth in engagement is supported by sufficient workforce capacity and balanced geographically and demographically.

1️⃣ ASK — Defining the Strategic Question

The analysis was guided by one central question:

Is participation growth sustainable, and is coaching capacity aligned to support it?

This expands into five operational sub-questions:

Is membership growing year-on-year?

Is participation stable enough to sustain that growth?

Is coaching capacity expanding at a similar rate?

Is inclusion balanced across gender and age?

Are resources evenly distributed across Scotland?

These directly inform funding allocation, workforce strategy, inclusion initiatives, and regional investment.

2️⃣ PREPARE — Establishing the Baseline

Before modelling, I defined performance benchmarks to ensure every calculation would tie back to decision-making.

Core Performance Snapshot
Metric	Value
Total Members	81,000
Membership YoY Growth	13.93%
Adult Members	51,000
Youth Members	30,000 (37%)
Female Members	38,000 (~47%)
Total Participants	51,000
Total Coaches	889
Coaches YoY Growth	1.91%
Qualified Coaches	469 (53%)
Female Coaches	28%
Coaches-to-Members Ratio	1 : 91

This immediately establishes the key tension:

Membership growth = 13.93%
Coaching growth = 1.91%

That disparity drives the rest of the analysis.

3️⃣ PROCESS — Ensuring Data Integrity

The dataset required validation before insights could be trusted.

I:

• Removed duplicate headers
• Verified that adult + youth totals reconciled to total membership
• Validated male + female splits
• Ensured club-year combinations were unique
• Standardised local authority naming
• Implemented a star schema for clean modelling

The final model included:

Fact Tables:

Members

Participants

Coaches

Dimension Tables:

Club

Local Authority

Year

DAX calculations were built using:

CALCULATE() for context transitions

FILTER() for year-over-year comparisons

DIVIDE() for safe ratio calculations

VAR/RETURN for structured logic

ALL() for benchmarking

This ensured accurate, dynamic, and filter-aware KPIs.

4️⃣ ANALYZE — Connecting the Dots

Now we move from numbers to meaning.

📈 PAGE 1 — Membership Growth & Sustainability

![Club Members – Year-on-Year Performance](Club-Members-Page.png)


Membership currently stands at 81,000, growing at 13.93% year-on-year.

At face value, this is strong growth.

However, sustainability depends on composition and distribution.

Demographic Composition

Youth Members: 30,000 (37%)

Adult Members: 51,000 (63%)

Female Members: 38,000 (~47%)

The youth proportion of 37% suggests a healthy development pipeline. Growth is not concentrated purely in adult recreational participation.

Female representation at 47% indicates near parity at membership level, suggesting inclusion initiatives are reaching their target demographic.

Distribution Risk

Growth is uneven:

Club C19: +4.9K

Multiple clubs below 3K

This suggests dependency on high-performing clubs.

If top clubs plateau, aggregate growth may slow dramatically.

Strategic Interpretation

Membership is expanding.
Inclusion at membership level is balanced.
However, resilience depends on broader club performance.

Without lifting mid-tier and lower-tier clubs, growth may not be structurally stable.

🏃 PAGE 2 — Participation & Pipeline Stability

![Participants – Year-on-Year Performance](Participants-Page.png)

Total Participants: 51,000

Trend:

Year	Participants
2023	22.8K
2024	10.8K
2025	17.5K

The 12K drop between 2023 and 2024 represents a 52% decline.

Although 2025 shows recovery, participation remains below 2023 levels.

Participation often precedes membership. Therefore:

If participation is volatile → future membership growth becomes uncertain.

Demographics

Youth Participation: 46%

Female Participation: 45%

Participation inclusion mirrors membership inclusion, which indicates demographic reach is consistent.

Geographic Variation

Edinburgh ≈ 13K

Glasgow ≈ 9K

Several authorities near zero

This indicates participation is regionally concentrated.

Strategic Interpretation

Participation is strong in scale but unstable in trend.

If volatility persists, membership growth may flatten within 1–2 reporting cycles.

Regional inequality suggests uneven access or engagement.

🧑‍🏫 PAGE 3 — Coaching Capacity & Workforce Alignment

![Coaches, Capacity & Location – Year-on-Year Analysis](Coaches-Page.png)

Total Coaches: 889

Growth: 1.91%

Membership growth: 13.93%

This creates a widening capacity gap.

Capacity Ratio

81,000 Members ÷ 889 Coaches ≈ 91 Members per Coach

If membership continues to grow at 13.93% annually and coaching grows at 1.91%, the ratio will worsen significantly over the next 2–3 years.

Qualification Quality

Qualified Coaches: 53%

Nearly half the workforce is unqualified.

This raises concerns around programme quality and development pathways.

Gender Representation

Female Members: 47%

Female Coaches: 28%

Gap: 19 percentage points

This indicates potential barriers in coaching progression for women.

Regional Imbalance

Edinburgh: 197 Coaches

Glasgow: 183 Coaches

Some regions: <20

Workforce concentration increases inequality in service access.

Strategic Interpretation

The coaching workforce is not scaling with demand.

If unaddressed:

Programme quality may decline

Retention may drop

Inclusion objectives may stall

This is the most significant strategic risk identified.

5️⃣ SHARE — Communicating to Stakeholders

The dashboard was intentionally structured as:

Growth (Members)

Stability (Participants)

Capacity (Coaches)

This narrative mirrors decision logic:

Demand → Pipeline → Supply

Interactive slicers allow scenario-based filtering by year and region.

The design prioritises KPI visibility and benchmarking to support executive decision-making.

6️⃣ ACT — Strategic Direction
1. Workforce Expansion

Coaching growth must increase from 1.91% to at least 10–12% annually to align with membership growth.

2. Qualification Improvement

Raise qualified coach rate from 53% to 60%+ to improve service quality.

3. Gender Pathway Development

Close 19% coaching gender gap through targeted mentoring and certification subsidies.

4. Regional Rebalancing

Allocate workforce grants to underrepresented authorities.

5. Participation Stabilisation

Investigate root cause of 12K drop between 2023–2024.

Final Strategic Position

The data clearly shows that:

• Engagement is growing
• Inclusion at participation level is strong
• Workforce capacity is lagging
• Regional inequality persists

The primary strategic risk is capacity misalignment.

Without accelerating coaching expansion and improving qualification rates, continued membership growth may strain service delivery.

This dashboard transforms isolated metrics into a connected sustainability model — linking growth, inclusion, geography, and workforce into one strategic view.

If you’d like, I can now turn this into:

• A spoken 10-minute presentation script
• Or a senior-executive summary version (5 minutes, sharper and more strategic)

dont write everything in one line. keep it in paragraphs

Perfect — thank you for clarifying.
Now I’ll rewrite this properly in clear, structured paragraphs, like you are presenting to senior stakeholders — not rushed, not compressed, and not written in single-line fragments.

This will read like a real strategic presentation narrative.

📊 CASE STUDY
Sport Scotland Membership, Participation & Coaching Sustainability Analysis

Author: Neeraj Raj Srinivasa Raju
Tool: Microsoft Power BI | DAX | Power Query
Data Source: sportscotland Public Club Dataset (2023–2025)

This case study follows the structured data lifecycle:

Ask → Prepare → Process → Analyze → Share → Act

Scenario

sportscotland works in partnership with Scottish Governing Bodies to increase participation in sport across Scotland. To support this objective, annual data is collected on club membership, participants, and coaches across multiple local authorities.

The dataset analysed in this project covers three reporting years (2023–2025) and includes 81,000 registered members, 51,000 participants, and 889 active coaches across more than 200 clubs.

The purpose of this analysis was not simply to visualise totals, but to evaluate sustainability. Specifically, the goal was to determine whether growth in engagement is being supported by sufficient and appropriately distributed coaching capacity.

The central strategic question guiding the analysis was:

Is sport participation growing sustainably, and is coaching capacity aligned to support that growth across Scotland?

1️⃣ Ask

To answer this overarching question, the analysis was structured around five operational objectives.

First, I needed to determine whether formal membership is growing year-on-year and whether that growth is significant.

Second, I assessed whether participation — which often acts as a pipeline into membership — is stable or volatile.

Third, I examined whether the coaching workforce is expanding at a rate that matches demand growth.

Fourth, I evaluated demographic balance, particularly gender representation across membership and coaching.

Finally, I assessed geographic distribution to identify regional disparities in engagement and workforce supply.

Each of these areas directly influences funding decisions, workforce planning, and long-term development strategy.

2️⃣ Prepare

Before building the dashboard, I defined clear baseline performance indicators to anchor the analysis.

Total membership stands at 81,000, with a year-on-year growth rate of 13.93%. Adult members account for 51,000, while youth members account for 30,000 — representing 37% of the total membership base. Female members make up approximately 38,000, or 47% of total members.

Participation totals 51,000 individuals across the three-year period.

The coaching workforce consists of 889 coaches, with 53% qualified and 28% female representation. Coaching growth year-on-year is 1.91%.

When calculated as a capacity ratio, there is approximately one coach per 91 members.

Defining these metrics early ensured that every calculation later in the process was aligned to answering sustainability and workforce alignment questions.

3️⃣ Process

The dataset required structural cleaning and validation before meaningful analysis could begin.

Duplicate headers were removed and data types were standardised. Membership splits were validated to ensure that adult plus youth totals reconciled with overall membership totals. Similarly, male and female totals were checked for consistency.

A star schema model was implemented to support scalable analysis. Separate fact tables were created for Members, Participants, and Coaches. These were connected through shared dimensions including Club, Local Authority, and Year.

Advanced DAX measures were developed using CALCULATE and FILTER to compute dynamic year-on-year comparisons. DIVIDE was used to ensure safe ratio calculations, and structured VAR/RETURN logic improved clarity and maintainability.

This modelling approach ensured that insights remained accurate even when filtered by region or year.

4️⃣ Analyze
Membership – Growth and Structural Stability

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

5️⃣ Share

The dashboard was intentionally structured across three focused pages.

The first page establishes demand through membership growth and demographic composition.

The second page evaluates engagement stability through participation trends and geographic variation.

The third page assesses supply through coaching capacity, qualification levels, and regional distribution.

This progression mirrors strategic decision-making logic: demand, pipeline, and supply.

Interactive slicers allow filtering by year and region to support scenario analysis and policy evaluation.

6️⃣ Act

Based on the findings, several strategic actions are recommended.

First, coaching recruitment growth must increase toward 10–12% annually to align more closely with membership growth of 13.93%.

Second, the qualification rate should be improved from 53% toward at least 60% to strengthen workforce quality.

Third, female coaching development pathways should be prioritised to close the 19 percentage point gender gap.

Fourth, targeted funding should be directed toward underrepresented local authorities to rebalance workforce and participation distribution.

Finally, the 2023–2024 participation drop should be investigated to identify retention barriers and prevent future volatility.

Final Strategic Position

The data demonstrates that sport engagement across Scotland is expanding in scale and remains relatively inclusive at membership and participation levels.

However, coaching capacity is not growing at the same pace as demand, and regional and gender imbalances persist within the workforce.

Without intervention, workforce strain and inequality may undermine long-term sustainability.

This dashboard moves beyond descriptive reporting and provides a capacity-aligned sustainability model to support evidence-based decision-making.
