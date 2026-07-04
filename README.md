# Customer Analytics & Mortgage Risk Dashboard for Retail Banking

## Overview

This project explores customer behavior, mortgage exposure, and repayment risk within a fictional Australian retail bank, HarbourLine Bank Australia (HBA).

Using Tableau, I developed an executive dashboard designed to help decision-makers better understand customer tenure, mortgage portfolio exposure, repayment stress indicators, and retention opportunities. The dashboard combines customer demographics, lending data, credit health metrics, liquidity measures, and behavioral indicators to support proactive portfolio management.

## Key Results

- $9.88B mortgage portfolio analyzed
- 17.55% of mortgage customers identified as showing elevated repayment stress indicators
- 5.71% identified as highly stable retention candidates
- Customer retention appears to weaken beyond the 6-7 year tenure mark

**Interactive Dashboard:**

https://public.tableau.com/app/profile/fred.rinaldo/viz/MIS771A3_17699162989440/Dashboard1

![Dashboard Overview](Images/Dashboard_Overview.png)

---

## Business Problem

Like many Australian lenders, HBA operates in an environment shaped by rising living costs, interest rate sensitivity, and changing employment conditions.

While mortgage lending remains a major source of revenue, it also represents a significant source of risk. HBA's leadership wanted to better understand:

- How customer relationships evolve over time
- Where mortgage exposure is concentrated
- Which customer segments display early indicators of repayment stress
- Which customers represent long-term strategic value
- How to balance portfolio risk management with customer retention

The objective was to transform customer and lending data into actionable insights that support executive decision-making.

---

## Dataset

The analysis was performed using a synthetic retail banking dataset containing customer demographic, financial, lending, engagement, and risk-related information.

The dataset includes:

- Customer demographics
- Relationship tenure
- Product ownership
- Home loan balances
- Credit scores
- Deposit balances
- Industry risk classifications
- Delinquency indicators
- Digital engagement metrics
- Loyalty and rewards information

To keep the repository lightweight, a representative sample dataset and complete data dictionary are included.

---

## Analytical Approach

The dashboard was designed around a progression from customer understanding to portfolio prioritization.

Key analytical dimensions included:

- Customer tenure and relationship maturity
- Mortgage exposure
- Credit score health
- Financial leverage
- Liquidity buffers
- Industry risk
- Delinquency indicators

The analysis focuses on identifying leading indicators of repayment stress rather than relying solely on historical defaults.

### Highlights

| Metric | Value |
|----------|----------|
| Mortgage Customers | 13,997 |
| Total Mortgage Exposure | $9.88 Billion |
| Current Delinquency Rate | 1.3% |
| Customers Showing Elevated Repayment Stress | 17.55% |
| Highly Stable Mortgage Customers | 5.71% |

---

# Key Findings

## 1. Customer Retention Appears to Weaken Beyond 6-7 Years

![Customer Tenure Analysis](Images/Tenure_By_Age_Groups.png)

Customer relationships generally strengthen over time, with older customer groups more frequently represented within longer-tenure categories.

However, customer counts decline noticeably after the 6-7 year tenure band. Even among older customers, the 8-9 year tenure category never surpasses earlier tenure groups.

This suggests a potential retention bottleneck and highlights an opportunity to proactively engage customers before relationship maturity begins to decline.

---

## 2. Mortgage Exposure Is Concentrated Within Structurally Vulnerable Segments

![Mortgage Exposure & Leverage](Images/Mortgage_Exposure_Leverage.png)

Customers with poor credit score health and liquidity buffers of only one to six months account for approximately **15.22% of total mortgage balances**.

While many of these customers are not currently delinquent, the concentration of exposure within this segment suggests heightened vulnerability to adverse economic conditions.

This finding highlights the importance of evaluating both exposure size and customer risk characteristics when prioritizing portfolio oversight.

---

## 3. Repayment Stress Is Concentrated in Common Customer Segments

![Mortgage Repayment Stress Indicators](Images/Repayment_Stress_Indicators.png)

Approximately **17.55% of mortgage customers** exhibit characteristics associated with elevated repayment stress.

Analysis of relative delinquency indicators revealed that repayment stress is not limited to extreme outlier groups. Instead, many mid-range customer segments display elevated risk while representing meaningful portions of the mortgage portfolio.

Customers employed within higher-risk industries consistently showed higher relative delinquency rates, particularly when combined with weaker liquidity positions.

---

## 4. Liquidity Buffers Strongly Influence Risk Outcomes

![Concentration of Mortgage Risk and Liquidity](Images/Mortgage_Risk_Concentration.png)

Liquidity emerged as one of the strongest differentiators of repayment resilience.

Customers with stronger liquidity positions consistently demonstrated lower repayment stress indicators, while customers with limited cash reserves appeared disproportionately represented among higher-risk segments.

The findings suggest that liquidity plays a critical role in absorbing short-term financial shocks, even when customers possess similar credit profiles.

---

## 5. The Greatest Portfolio Risk Exists Where Exposure and Stress Intersect

![High-Risk Mortgage Segments](Images/High-Risk_Segments_1.png)

Portfolio risk is not evenly distributed across the mortgage book.

While some segments exhibit very high relative delinquency rates, they often represent relatively small customer populations and limited financial exposure.

More strategically important are the mid-risk, high-exposure segments that combine:

- Elevated repayment stress indicators
- Significant customer populations
- Large outstanding mortgage balances

These groups represent the greatest potential downside to portfolio performance and therefore warrant the highest monitoring priority.

---

## 6. Stable Customers Represent a Valuable Retention Opportunity

![Distribution of Stable Mortgage Customers](Images/Stable_Customers.png)

The analysis identified a distinct segment of financially stable mortgage customers characterized by:

- High or very high credit score health
- At least three months of liquidity buffer
- No observed delinquency
- Meaningful lending relationships

Geographic analysis showed that Western Australia consistently demonstrated the highest concentration of stable customers, while Tasmania and the Australian Capital Territory displayed comparatively lower shares.

These customers represent attractive targets for relationship-building, retention initiatives, and additional product adoption.

---

# Recommendations

## Recommendation 1: Introduce Tenure-Based Mortgage Review Programs

Develop structured relationship reviews beginning at four years of tenure and increasing at subsequent milestones.

Potential initiatives include:

- Mortgage pricing reviews
- Offset account fee waivers
- Redraw fee waivers
- Loyalty-based retention incentives

This approach targets customers before the observed decline in retention beyond the 6-7 year tenure range.

---

## Recommendation 2: Implement Proactive Early-Intervention Support

Identify customers exhibiting:

- Liquidity buffers of three months or less
- Medium to poor credit score health
- Higher leverage ratios
- Employment within higher-risk industries

Provide supportive outreach before repayment difficulties materialize through financial wellbeing reviews, repayment flexibility options, and hardship support pathways.

---

## Recommendation 3: Prioritize Mid-Risk, High-Exposure Segments

Focus monitoring resources on segments that combine elevated repayment stress indicators with significant mortgage balances.

These customers present a greater strategic risk than many extreme outlier groups due to the scale of their potential impact on portfolio performance.

---

## Recommendation 4: Enhance Future Risk Detection Capabilities

A preliminary logistic regression model was explored but delivered limited predictive value due to the highly imbalanced nature of the dataset, with delinquent customers representing only approximately 1.4% of mortgage holders.

Future iterations could investigate:

- Class-weighted logistic regression
- Decision tree models
- Ensemble methods
- Other approaches designed for imbalanced datasets

This would support a transition from descriptive analysis toward predictive risk management.

---

## Business Impact

This dashboard provides a framework for balancing two critical objectives:

1. Protecting the mortgage portfolio through proactive identification of emerging repayment stress.
2. Retaining profitable, long-term customers through targeted engagement and loyalty initiatives.

By combining customer tenure, mortgage exposure, liquidity position, leverage, credit health, and delinquency indicators into a single analytical view, decision-makers can prioritize intervention efforts where both risk and financial impact are greatest.

---

## Tools & Techniques

**Tools**

- Tableau

**Analytics Techniques**

- Customer Segmentation
- Mortgage Portfolio Analysis
- Credit Risk Assessment
- Customer Retention Analysis
- Financial Risk Profiling
- KPI Development
- Data Storytelling
- Executive Dashboard Design

---

## Repository Structure

```text
Data
├── Data Dictionary.csv
└── Sample Dataset.csv

Images
├── Dashboard_Overview.png
├── High-Risk_Segments_1.png
├── High-Risk_Segments_2.png
├── High-Risk_Segments_2.png
├── Mortgage_Exposure_Leverage.png
├── Mortgage_Risk_Concentration.png
├── Repayment_Stress_Indicators.png
├── Stable_Customers.png
└── Tenure_By_Age_Groups.png

README.md
```

---

## Disclaimer

This project was completed as part of postgraduate Business Analytics coursework and uses a fictional banking scenario with synthetic customer data for educational purposes.
