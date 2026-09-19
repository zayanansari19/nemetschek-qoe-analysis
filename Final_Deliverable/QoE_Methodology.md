# Nemetschek SE — Quality of Earnings Analysis: Methodology Write-Up

**Prepared by:** Zayan Ansari  
**Date:** September 2026  
**Subject:** Nemetschek SE (XETRA: NEM)  
**Period:** FY2020 – FY2024

---

## 1. Framework Overview

This Quality of Earnings (QoE) analysis follows the methodology used by Big 4 Transaction Services (TS) teams during commercial due diligence engagements. The framework evaluates the **sustainability, predictability, and quality** of a target company's earnings across ten analytical dimensions, producing findings in the standard Observation → Implication → Management Question → Risk Rating format.

The analysis is adapted for a **software/SaaS company undergoing a business model transition** from perpetual licenses to subscription-based revenue, which creates specific analytical challenges around revenue recognition timing, deferred revenue interpretation, and margin trajectory during the transition period.

## 2. Data Sources & Extraction

All data is sourced from publicly available Nemetschek SE annual reports and filings:

| Source | Coverage | Key Data Points |
|--------|----------|----------------|
| Annual Report 2024 | FY2024 + FY2023 comparative | Consolidated P&L, BS, CF; Notes 1-26; Segment reporting; Management report |
| Annual Report 2023 | FY2023 + FY2022 comparative | Cross-verification; Key Figures 5-year table |
| Annual Report 2022 | FY2022 + FY2021 comparative | Historical data extension; Key Figures table |
| Annual Report 2021 | FY2021 + FY2020 comparative | Historical baseline |
| Annual Report 2020 | FY2020 + FY2019 comparative | Period start baseline |
| H1 2025 Report | H1 2025 interim | Forward indicators, latest trend |
| Company Presentation 2024 | Strategic context | Market positioning, strategy |

**Data extraction approach:**
- Primary financial data (revenue, EBITDA, net income, cash flow) extracted from audited Key Figures tables spanning 5 years, cross-verified across overlapping reports
- Detailed breakdowns (revenue by type, region, segment) extracted from Note [1] (Revenue Recognition) and Note [26] (Segment Reporting) of the AR 2024 consolidated financial statements
- Acquisition details from Business Combinations note (AR 2024 pp.172-175)
- Growth decomposition (organic vs inorganic, currency-adjusted) from Management Report (AR 2024 pp.111-125)
- Balance sheet and cash flow data from consolidated statements (AR 2024 pp.153-157)

**Data derivation:** Where absolute EUR figures were available only for FY2023-2024 (from AR 2024 notes), FY2020-2022 segment and regional revenue was estimated by applying reported percentage splits to total revenue. These derived figures are clearly marked in the workbook with source citations.

## 3. Analytical Dimensions

### 3.1 Revenue Quality
**Objective:** Assess the predictability and contractual nature of the revenue base.

**Metrics:**
- Recurring revenue as % of total (target: >80%)
- Subscription/SaaS as % of total and % of recurring
- Revenue stream CAGR (5-year)
- Revenue type YoY growth rates

**Why it matters:** Recurring revenue is contracted and predictable, supporting higher valuation multiples. The ratio of subscription to maintenance within recurring revenue indicates how far the transition has progressed — maintenance is recurring but less sticky than multi-year subscriptions.

### 3.2 ARR (Annual Recurring Revenue)
**Objective:** Measure the forward run-rate of contracted revenue.

**Metrics:**
- ARR absolute level and growth rate
- ARR / Revenue ratio (>1.0x = embedded forward growth)
- Organic ARR growth (excluding M&A)

**Interpretation:** ARR exceeding reported revenue (ratio >1.0x) means new subscriptions signed during the period contribute annualized run-rate beyond what was recognized — a strong quality signal indicating embedded near-term growth.

### 3.3 Organic vs Inorganic Growth
**Objective:** Decompose growth into sustainable organic performance vs M&A-driven expansion.

**Approach:**
- Total growth = Organic growth + M&A contribution + FX impact
- Organic growth calculated by excluding post-acquisition revenue from acquisitions closed in the period (GoCanvas: €27.5M in 6 months)
- Currency-adjusted figures use Nemetschek's reported constant-currency growth rates

**Why it matters:** Organic growth demonstrates the underlying business momentum and is generally valued more highly than M&A-driven growth, which carries integration risk.

### 3.4 Segment Profitability
**Objective:** Identify which business units drive group performance and where risks concentrate.

**Metrics per segment (Design, Build, Manage, Media):**
- Revenue contribution and growth
- EBITDA and EBITDA margin
- Margin trajectory (FY23 → FY24)
- Organic vs total growth decomposition

**Key insight:** The Build segment's margin decline (35.1% → 31.8%) is directly attributable to GoCanvas integration. Design's margin expansion (27.7% → 29.7%) reflects operating leverage from the subscription transition. Manage's revenue stagnation makes it the key risk segment.

### 3.5 Cash Conversion
**Objective:** Validate that accrual-based earnings are backed by actual cash generation.

**Metrics:**
- Cash Conversion Ratio = Operating Cash Flow / Net Income (target: >100%)
- FCF before M&A / Net Income
- Capex / Revenue (capital intensity)

**Interpretation:** A software business with annual upfront billing should consistently convert >100% of net income to cash. Nemetschek's 5-year average of ~156% exceeds this benchmark. The 1.4% capex/revenue ratio confirms an asset-light model.

### 3.6 Working Capital (DSO)
**Objective:** Monitor collection efficiency and identify potential revenue quality concerns.

**Metrics:**
- Days Sales Outstanding = Trade Receivables (net) / Revenue × 365
- Trade receivables growth vs revenue growth
- Bad debt allowance trend

**Red flag test:** When receivables grow materially faster than revenue (Nemetschek: +48% vs +16.9%), it may signal extended payment terms, collection difficulties, or integration effects from newly acquired entities.

### 3.7 Deferred Revenue
**Objective:** Assess forward revenue visibility from pre-paid customer commitments.

**Metrics:**
- Deferred revenue (contract liabilities) absolute and as % of revenue
- Split between short-term (current) and long-term (non-current)
- Recognition rate (how much of opening balance was recognized in the period)

**Interpretation:** Growing deferred revenue indicates increasing pre-paid commitments — a positive forward visibility signal. The 97.7% recognition rate (€265.1M of €271.2M opening balance recognized in FY24) confirms predictable revenue conversion.

### 3.8 Balance Sheet Assessment
**Objective:** Evaluate financial health and flexibility post-M&A.

**Metrics:**
- Net cash / (debt) position
- Equity ratio
- Goodwill / total assets
- Leverage ratios (debt / equity, debt / EBITDA)

**Context:** The GoCanvas acquisition fundamentally changed Nemetschek's balance sheet structure. The shift from net cash (€268M) to net debt (~€295M) is material but manageable given €307M operating cash flow. The 53% goodwill-to-assets ratio is typical for serial acquirers in software.

### 3.9 Geographic Diversification
**Objective:** Assess revenue concentration risk across regions.

**Metrics:**
- Revenue by region (absolute and %)
- Regional mix shift over 5 years
- Growth rate by region

**Trend:** The structural shift toward Americas (30.5% → 40.4%) is strategically positive, providing exposure to the world's largest AEC software market.

### 3.10 Customer Concentration
**Objective:** Evaluate key-client dependency risk.

**Assessment:** Based on management disclosures ("broad client structure, no concentration risk") and the inherently fragmented nature of AEC sector demand. No single customer represents >5% of revenue — a low-risk profile.

## 4. Findings Format

Each finding follows the Big 4 Transaction Services format:

| Element | Description |
|---------|-------------|
| **Observation** | Factual statement of what the data shows, with specific figures |
| **Implication** | What this means for the investment thesis or valuation |
| **Management Question** | What a buyer would ask management in a due diligence meeting |
| **Risk Rating** | LOW / MEDIUM / HIGH based on materiality and probability |

**Risk Rating Criteria:**
- **LOW:** Supports the thesis; no material concern; monitored as part of normal course
- **MEDIUM:** Requires active monitoring; potential for deterioration; may need management action
- **HIGH:** Material risk to the thesis; could affect valuation or deal structure; requires specific diligence

## 5. Deliverables

| Deliverable | Description |
|-------------|-------------|
| **Nemetschek_QoE_v1.xlsx** | 8-tab Excel workbook: Cover, Exec_Summary, Data_Raw, Revenue_Analysis, Recurring_Rev, Segment_DeepDive, Quality_Metrics, Findings |
| **Nemetschek_QoE_Dashboard.html** | Interactive HTML dashboard with Chart.js visualizations across 7 views (Overview, Revenue, Recurring, Segments, Quality, Findings, Methodology) |
| **QoE_Methodology.md** | This document — analysis framework and approach description |

## 6. Limitations

- Analysis based solely on **publicly available** annual report data — no access to management, internal metrics, or data room materials
- **Net revenue retention rate**, customer-level churn, and contract duration distribution are not publicly disclosed
- FY2020-2022 segment data in absolute EUR is **estimated** from reported percentage splits
- GoCanvas is assessed on only **6 months** of post-acquisition data; full-year integration effects are unknown
- Currency-adjusted figures use **company-reported** constant-currency growth rates, not independently calculated rates
- No access to **competitive benchmarking** data (peer multiples, market share)
- The analysis does not constitute investment advice or a recommendation

## 7. Skills Demonstrated

This project demonstrates proficiency in:

1. **Financial Data Extraction** — Parsing and cross-referencing multi-year annual reports (PDF), identifying the correct notes and page references
2. **Quality of Earnings Framework** — Applying Big 4 TS methodology to a real company with specific focus on software/SaaS metrics
3. **Revenue Decomposition** — Breaking down revenue by type, region, and segment; tracking subscription transition dynamics
4. **M&A Analysis** — Purchase price allocation, goodwill analysis, organic vs inorganic growth decomposition
5. **Excel Modeling** — Professional workbook construction with openpyxl (color-coded tabs, charts, source citations, consistent formatting)
6. **Data Visualization** — Interactive Chart.js dashboard with 15+ charts across multiple views
7. **Analytical Writing** — Clear, structured findings in professional TS format with actionable management questions
8. **Python/Automation** — Automated workbook generation from extracted data, ensuring consistency and reproducibility

---

*This analysis was prepared using publicly available data from Nemetschek SE annual reports for portfolio and interview demonstration purposes.*
