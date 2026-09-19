# Nemetschek QoE Project — Interview Study Guide

**Purpose:** Everything you need to understand and confidently explain every concept in your QoE dashboard project during a job interview at Nemetschek, Siemens, or any consulting/finance role.

**How to use this:** Read it section by section. Each concept has: what it means → why it matters → how it shows up in YOUR project → likely interview questions with answers. The methodology doc (`QoE_Methodology.md`) is your reference for the *structure* of the analysis; this guide is your reference for the *concepts* behind it.

**Your background:** Basic corporate finance + financial/cost accounting. This guide fills the gaps without repeating what you already know.

---

## PART 1: THE FRAMEWORK — "What is a QoE and Why Did You Do One?"

### 1.1 Quality of Earnings (QoE) Analysis

**What it is:** A QoE is the core financial analysis done during M&A due diligence. When a company is being acquired, the buyer hires a Big 4 firm (Deloitte, PwC, EY, KPMG) to answer one question: *"Are the earnings real, sustainable, and likely to continue?"*

**Why it exists:** Reported earnings under IFRS/GAAP can include one-off items, aggressive accounting, or unsustainable trends. A QoE strips those away to find the "normalized" or "underlying" earnings a buyer can rely on.

**The three pillars of quality:**
1. **Sustainability** — Will this revenue/profit continue next year? (Recurring revenue is more sustainable than one-off project fees)
2. **Predictability** — How confident can we be in the forecast? (Contracted ARR is more predictable than pipeline)
3. **Cash-backing** — Are earnings converting to actual cash? (A company can show profit on paper but not generate cash if receivables pile up)

**How it shows up in your project:** Your entire analysis is structured around these three pillars. The Revenue Analysis and Recurring Rev tabs assess sustainability. The ARR and deferred revenue analysis assesses predictability. The Quality Metrics tab (cash conversion, DSO) assesses cash-backing.

> **Interview Q:** *"Why did you choose a QoE framework for this project?"*
> **Your answer:** "Because Nemetschek is a software company in the middle of a subscription transition — exactly the kind of company that would be a due diligence target. A QoE lets me evaluate whether the 17% revenue growth is real and sustainable, or whether it's inflated by one-off license sales and acquisitions. It's the framework any buyer would use, so it shows I can think like a Transaction Services analyst."

> **Interview Q:** *"What's the difference between a QoE and just reading the annual report?"*
> **Your answer:** "The annual report tells you what happened. A QoE asks whether it will keep happening. For example, Nemetschek reports 16.9% revenue growth — but my analysis decomposes that into 13.7% organic and 3.2% from the GoCanvas acquisition. A buyer pays a different multiple for organic growth than for acquired growth, so that distinction matters for valuation."

### 1.2 Big 4 Transaction Services (TS) Format

**What it is:** The standard format used by Big 4 due diligence teams to present findings to clients (the buyer, usually a PE firm or corporate acquirer).

**The format:**
- **Observation:** Pure fact. What the data shows, with specific numbers. No opinion.
- **Implication:** What this means for the deal. How does it affect risk, valuation, or the investment thesis?
- **Management Question:** What you'd ask the target company's management team in a due diligence session. This shows you're thinking like a buyer.
- **Risk Rating:** LOW / MEDIUM / HIGH based on how material the issue is.

**Why this format matters:** It shows you can communicate financial analysis in a structured, professional way — the same way a Deloitte or PwC analyst would present to a client.

> **Interview Q:** *"Walk me through one of your findings."*
> **Your answer (Finding #3 — GoCanvas):** "The observation is that Nemetschek acquired GoCanvas for €665 million in July 2024, with goodwill representing 80% of the purchase price. In six months post-acquisition, GoCanvas generated €27.5 million revenue but only €5.5 million EBITDA — a 20% margin, versus the group's 30%. The implication is that this is a high-risk integration bet that materially changed the balance sheet — they took on €500 million in debt. The management question I'd ask is: what are the synergy targets, what's the path to 30%+ margins, and how does GoCanvas integrate with Bluebeam? I rated this HIGH risk because of the size, the low initial margins, and the leverage change."

---

## PART 2: FINANCIAL STATEMENTS — "Where Did the Numbers Come From?"

### 2.1 The Three Financial Statements (Quick Refresh)

You know these from accounting, but here's how they connect in the QoE:

**Income Statement (P&L)** → "How much did they earn?"
- Revenue → broken down by type (subscription, license, maintenance) and by segment
- EBITDA = Earnings Before Interest, Tax, Depreciation & Amortization → the standard profitability metric for software companies because it strips out non-cash charges and capital structure effects
- Net Income → bottom line, but less useful in software because D&A (especially from acquisitions) can distort it

**Balance Sheet** → "What do they own and owe?"
- Trade receivables → used to calculate DSO (collection speed)
- Deferred revenue (contract liabilities) → pre-paid customer commitments = forward visibility
- Goodwill → the premium paid over net assets in acquisitions
- Debt vs equity → capital structure health

**Cash Flow Statement** → "Is the profit real cash?"
- Operating Cash Flow (OCF) → cash generated by the business
- Capex → capital expenditure (very low for software = asset-light)
- Free Cash Flow (FCF) = OCF - Capex → cash available to shareholders/debt repayment
- FCF before M&A → strips out acquisition spending to show underlying cash generation

**In your project:** The Data_Raw tab has all three statements' key figures with source page references. The methodology doc Section 2 explains exactly which pages and notes each number came from.

### 2.2 EBITDA vs EBIT vs Net Income — Why EBITDA?

**Why software companies use EBITDA:**
- **EBIT** includes D&A. In software, a big chunk of D&A is "PPA amortization" — amortizing intangible assets acquired through M&A. Nemetschek had €36.7M of PPA amortization in FY24. This is a non-cash accounting charge that doesn't reflect operational performance.
- **EBITDA** removes all D&A, giving a cleaner view of operational profitability.
- **Net Income** includes interest (capital structure choice) and tax (jurisdiction-dependent). Neither reflects how well the business actually runs.

**In your project:** EBITDA margin is the primary profitability metric throughout. Nemetschek's 30.2% is the headline number. The organic EBITDA margin (31.1%, excluding GoCanvas) shows the underlying business performs even better.

> **Interview Q:** *"Why did you use EBITDA instead of net income as the profitability metric?"*
> **Your answer:** "EBITDA is standard for software company analysis because it strips out non-cash D&A — especially PPA amortization from acquisitions, which was €36.7 million for Nemetschek in FY24 — as well as capital structure and tax effects. It gives a cleaner picture of operational profitability. Net income is still important for cash conversion analysis, which I cover in the Quality Metrics tab."

### 2.3 Revenue Recognition & IFRS 15 (Just Enough)

**The core idea:** Under IFRS 15, you recognize revenue when you deliver the service, not when you get paid.

**How this plays out at Nemetschek:**
- **Perpetual license:** Customer pays once, gets the software forever. Revenue recognized mostly upfront at delivery. This is why license revenue is "lumpier" — it's a one-time event.
- **Subscription/SaaS:** Customer pays monthly/annually for access. Revenue recognized evenly over the subscription period. If someone pays €120 for a 12-month subscription in July, you recognize €10/month — only €60 in that year, the other €60 is "deferred revenue" (a liability on the balance sheet because you still owe them 6 months of service).
- **Maintenance:** Annual support contracts, recognized evenly over the period. Similar to subscription but without the software access.

**Why this matters for QoE:** Subscription revenue is recognized over time, so it's inherently smoother and more predictable. This is why the transition from licenses to subscriptions is the central theme of your analysis — it fundamentally changes the quality of Nemetschek's earnings.

**Deferred revenue connection:** When a customer pre-pays and you haven't delivered yet, the cash sits on your balance sheet as "deferred revenue" (also called "contract liabilities" under IFRS 15). It's essentially a backlog of guaranteed future revenue. Growing deferred revenue = growing forward visibility = higher quality earnings.

> **Interview Q:** *"What's deferred revenue and why is it a positive signal?"*
> **Your answer:** "Deferred revenue represents cash customers have already paid for services Nemetschek hasn't yet delivered. It's a liability on the balance sheet because they still owe the service. For a QoE analysis, growing deferred revenue is a strong positive signal — it's essentially guaranteed future revenue. Nemetschek's deferred revenue grew 42% to €386 million, and 97.7% of the prior year's opening balance was recognized as revenue, confirming very predictable conversion."

---

## PART 3: SaaS & SUBSCRIPTION METRICS — "The Heart of the Analysis"

### 3.1 The Subscription Transition — Why It's the Biggest Story

**What's happening:** Nemetschek is shifting from selling perpetual software licenses (pay once, own forever) to subscription/SaaS (pay annually, access as long as you subscribe).

**Why companies do this:**
- **Predictable revenue:** Instead of lumpy one-time sales, you get contracted annual payments
- **Higher lifetime value:** A customer paying €100/year for 10 years = €1,000 vs a one-time €500 license
- **Better valuation multiples:** Public markets value recurring revenue at 8-15x vs 2-4x for perpetual license businesses
- **Stickier customers:** Harder to leave when your workflows depend on the subscription

**The "valley of transition":** When you stop selling licenses and start selling subscriptions, near-term revenue actually *drops* because you're recognizing subscription revenue over time instead of upfront. This creates a temporary dip — the "valley" — before the recurring base builds up and starts growing faster than the lost license revenue.

**In your project:** This is the entire story of the Recurring_Rev tab. In FY20, only 15.1% of revenue was subscription/SaaS. By FY24, it's 57.0%. Meanwhile, license revenue dropped from €210M to €101M. The valley appears to be mostly crossed — license decline is decelerating while subscription growth is accelerating.

### 3.2 ARR (Annual Recurring Revenue)

**What it is:** The annualized value of all active recurring contracts at a point in time. If you have 1,000 customers each paying €1,000/year, your ARR is €1M — regardless of when they signed or when the revenue gets recognized in the P&L.

**ARR vs Revenue:** Revenue is what you *recognized* in the P&L during the period (backward-looking). ARR is the *run-rate* of what you'd recognize over the next 12 months if nothing changed (forward-looking).

**Why ARR > Revenue is a quality signal:** If ARR (€1,020M) exceeds recognized revenue (€996M), it means new contracts signed during the year added enough run-rate to push the forward number above the backward number. This is "embedded growth" — even without signing a single new customer, next year's revenue should be higher than this year's.

**Organic ARR growth:** Nemetschek's total ARR grew 41.9%, but 34.6% was organic (excluding GoCanvas). The difference shows how much of the growth is from M&A vs the existing business.

> **Interview Q:** *"What does ARR tell you that revenue doesn't?"*
> **Your answer:** "Revenue is backward-looking — what was recognized this year. ARR is forward-looking — the current run-rate of contracted recurring revenue. Nemetschek's ARR of €1.02 billion exceeds their FY24 revenue of €996 million, giving a ratio of 1.02x. That means even with zero new sales, next year's revenue has a higher starting point. It's one of the strongest quality signals in the analysis."

### 3.3 Recurring Revenue Types

**Subscription/SaaS:** Customer pays for access to software, usually monthly or annually. Can be cloud-hosted (SaaS) or on-premise with a subscription key. Highest quality — contracted, predictable, growing.

**Maintenance:** Customer bought a perpetual license and pays an annual maintenance fee (typically 15-20% of the license price) for updates and support. It's recurring, but it's tied to the legacy license base — as customers migrate to subscriptions, maintenance eventually goes away.

**Why the split matters:** Both are "recurring," but they have very different futures. Subscription is growing at 88% and represents the future. Maintenance is the legacy base that will eventually convert. Your analysis tracks both within the recurring bucket to show this progression.

**In your project:** Sub/SaaS as % of recurring went from 25.2% (FY20) to 65.9% (FY24). The "crossover" — when subscription exceeded maintenance — happened around FY23. This is a key milestone in the transition.

### 3.4 Metrics You Mentioned But Couldn't Calculate (Know These Anyway)

**Net Revenue Retention (NRR):** Measures how much revenue from *existing* customers grew or shrank over 12 months, including upsells, downgrades, and churn. >100% means existing customers are spending more. Best-in-class SaaS is 120%+. Nemetschek doesn't disclose this publicly — it's a limitation you should be ready to discuss.

**Gross Revenue Retention (GRR):** Same but excluding upsells — pure churn measure. Typical good SaaS: >90%.

**Customer Lifetime Value (LTV) / Customer Acquisition Cost (CAC):** How much a customer is worth over their lifetime vs how much it cost to acquire them. LTV/CAC > 3x is the benchmark. Again, not disclosed by Nemetschek.

> **Interview Q:** *"What metric would you most want to add to this analysis if you had access to management data?"*
> **Your answer:** "Net revenue retention. It's the single most important SaaS metric I couldn't calculate from public data. It tells you whether existing customers are expanding their spend, which is the cheapest growth a company can get. For a company in subscription transition, NRR above 110% would confirm that the new model is generating upsell, not just replacement of license revenue."

---

## PART 4: GROWTH ANALYSIS — "Is the Growth Real?"

### 4.1 Organic vs Inorganic Growth

**Organic growth:** Revenue increase from the existing business — same entities, same products, no acquisitions. This is the "real" underlying growth rate.

**Inorganic growth:** Revenue added by acquiring other companies. GoCanvas was acquired July 1, 2024, and contributed €27.5M in revenue over 6 months.

**Why buyers care:** Organic growth commands a higher valuation multiple because it's repeatable and doesn't require capital outlay. Inorganic growth carries integration risk — you might pay €665M for a company and then fail to integrate it.

**The calculation for Nemetschek FY24:**
- Total revenue growth: 16.9%
- Organic (excluding GoCanvas): 13.7%
- GoCanvas contribution: ~3.2 percentage points
- This means ~81% of growth was organic — a strong signal

> **Interview Q:** *"Why is organic growth valued more highly than acquisition-driven growth?"*
> **Your answer:** "Three reasons. First, organic growth is repeatable — it comes from product-market fit and sales execution, not from spending capital. Second, it carries no integration risk. Third, it's a signal of competitive strength — customers are choosing your product. In my analysis, 81% of Nemetschek's FY24 growth was organic, which is strong. The 19% from GoCanvas still needs to prove itself — that acquisition is my highest-risk finding."

### 4.2 Currency-Adjusted (Constant Currency) Growth

**What it means:** Calculating growth as if exchange rates hadn't changed. With 40% of revenue from the Americas (mostly USD), EUR/USD movements can significantly affect reported growth.

**Example:** If the USD weakened against EUR, Nemetschek's Americas revenue would be worth fewer euros — making growth look lower than the underlying business actually grew. Currency-adjusted growth removes this distortion.

**In your project:** Nemetschek's revenue grew 16.9% nominal and 17.2% currency-adjusted. The small difference means FX had a slight negative impact in FY24. For ARR, the difference is also small (41.9% vs 41.6%). This is good — it means the growth story isn't FX-dependent.

### 4.3 CAGR (Compound Annual Growth Rate)

**Formula:** CAGR = (End Value / Start Value)^(1/n) - 1

You've probably seen this in finance class. In your project, the 5-year revenue CAGR is 13.6% (from €596.9M in FY20 to €995.6M in FY24, over 4 years).

**Why CAGR vs simple average growth:** CAGR smooths out year-to-year volatility and accounts for compounding. The simple average of yearly growth rates can be misleading if growth was uneven.

---

## PART 5: M&A CONCEPTS — "The GoCanvas Story"

### 5.1 Goodwill & Purchase Price Allocation (PPA)

**What goodwill is:** When you buy a company for more than its net assets (assets minus liabilities) are worth, the difference is goodwill. It represents intangible value — brand, customer relationships, technology, market position.

**GoCanvas example:**
- Purchase price: €665M
- Net assets acquired: €131M (the tangible "stuff" — cash, receivables, minus liabilities)
- Goodwill: €535M (the 80% premium above net assets)
- Identified intangible assets: €253M (customer relationships, technology — separately valued from goodwill)

**Why 80% goodwill is notable:** It means Nemetschek is paying mostly for future potential, not for existing assets. If the integration fails and GoCanvas doesn't grow as expected, that goodwill may need to be written down (impairment), which hits the P&L as a large one-off loss.

**Goodwill impairment risk:** Under IFRS, goodwill isn't amortized — it sits on the balance sheet and gets tested annually for impairment. If the acquired business underperforms, the goodwill gets written down. Nemetschek's total goodwill jumped from €552M to €1,135M (53% of total assets). That's a lot of "future potential" to live up to.

> **Interview Q:** *"Is the goodwill-to-assets ratio of 53% a concern?"*
> **Your answer:** "It's elevated but not unusual for serial acquirers in software. Companies like SAP and Dassault have similar ratios. The concern is concentration — €535M of that goodwill is from a single acquisition, GoCanvas, which has only been integrated for six months and has margins well below group average. If GoCanvas underperforms, that's a large impairment risk. But with €307M in operating cash flow, the business generates enough cash to service the debt that funded the acquisition."

### 5.2 PPA Amortization

**What it is:** The intangible assets identified in an acquisition (customer relationships, technology — the €253M for GoCanvas) get amortized over their useful life, typically 5-15 years. This shows up in D&A on the income statement.

**Why it matters for EBITDA vs net income:** PPA amortization was €36.7M in FY24 (out of total D&A of €66.8M). It's a real economic cost of the acquisition but it's non-cash, which is why EBITDA (which excludes it) is the preferred metric. It also explains why EBITDA margin (30.2%) looks so much better than net income margin (18.0%).

---

## PART 6: QUALITY METRICS — "Proving the Earnings Are Real"

### 6.1 Cash Conversion Ratio

**Formula:** OCF / Net Income

**What it tells you:** If a company reports €100 in net income but only generates €80 in cash, something is off — maybe revenue was recognized aggressively, or receivables are piling up. A ratio above 100% means the company generates *more* cash than it reports in profit. For software companies with upfront annual billing, this is typical and expected.

**Nemetschek:** 172% in FY24 (€307M OCF / €179M net income). This is excellent. The 5-year average of ~156% confirms this isn't a one-year fluke.

**Why it's above 100%:** Mainly because of D&A (non-cash charges reduce net income but not cash flow) and growing deferred revenue (customers paying upfront for subscriptions that haven't been recognized yet — cash in, no revenue yet).

### 6.2 Free Cash Flow (FCF) — Two Versions

**FCF (reported):** OCF minus ALL investing activities. In FY24, this was *negative* €400M because of the €681M spent on GoCanvas. This looks scary but is misleading for underlying performance.

**FCF before M&A:** OCF minus capex only (excluding acquisitions). This was €294M in FY24 (+22% YoY). This shows the underlying business generates strong cash regardless of M&A activity.

**Why your project tracks both:** To show that the negative reported FCF is entirely an M&A timing effect, not a deterioration in business quality. A buyer needs to see through that.

### 6.3 DSO (Days Sales Outstanding)

**Formula:** (Trade Receivables / Revenue) × 365

**What it measures:** On average, how many days it takes to collect payment from customers.

**Why the DSO increase is a flag:** Nemetschek's DSO went from 42.7 days (FY23) to 54.0 days (FY24). Trade receivables grew 48% while revenue grew only 16.9%. Three possible explanations:
1. GoCanvas brought in receivables with longer collection terms
2. Nemetschek is offering longer payment terms to win competitive deals
3. Some customers are struggling to pay

The bad debt allowance also doubled (€3.9M → €8.6M), which adds to the concern. This is why it's a MEDIUM risk finding — not alarming on its own, but worth monitoring.

> **Interview Q:** *"One of your metrics showed deterioration. Which one and what would you do about it?"*
> **Your answer:** "DSO increased from 42.7 to 54.0 days — trade receivables grew three times faster than revenue. If I had access to management, I'd ask three things: how much of the increase is from GoCanvas receivables, what's the aging profile of receivables over 90 days, and whether they're extending payment terms to win deals. The doubling of the bad debt allowance is also worth investigating. It's not alarming yet — 54 days is still reasonable for B2B software — but the trajectory needs monitoring."

### 6.4 Deferred Revenue as a Quality Signal

**What it is:** Cash collected from customers for services not yet delivered. It's a liability on the balance sheet (you owe the service) but it's *the best kind of liability* because it represents guaranteed future revenue.

**Nemetschek FY24:** €386M total deferred revenue (39% of revenue). Of the FY23 opening balance of €271M, 97.7% was recognized as revenue in FY24. This means the "conversion rate" from backlog to revenue is almost perfect.

**Short-term vs long-term split:**
- Short-term (€355M): Expected to be recognized within 12 months
- Long-term (€31M): Multi-year contracts recognized beyond 12 months — this quintupled from €6.2M, suggesting Nemetschek is signing longer-duration contracts (positive for predictability)

---

## PART 7: BALANCE SHEET & CAPITAL STRUCTURE

### 7.1 Net Cash vs Net Debt

**Net cash/debt** = Cash - Total Borrowings

**Nemetschek pre-GoCanvas (FY23):** €268M cash - ~€0 debt = **net cash of €268M** (very conservative, zero leverage)

**Nemetschek post-GoCanvas (FY24):** €206M cash - €500M LT borrowings = **net debt of ~€295M**

**Why this matters:** The balance sheet fundamentally changed in one year. The company went from having zero financial risk to having meaningful leverage. This reduces financial flexibility for future M&A and increases interest cost.

**Is it manageable?** Yes — net debt / EBITDA is about 1.0x (€295M / €301M), which is low by any standard. Investment-grade companies routinely operate at 2-3x. But it's a *change* that needs to be flagged.

### 7.2 Equity Ratio

**Formula:** Total Equity / Total Assets

**Nemetschek:** Dropped from 61.4% to 44.2%. This reflects both the new debt and the increase in assets (mostly goodwill from GoCanvas). A 44% equity ratio is still healthy — it just looks dramatic compared to the prior year.

---

## PART 8: SEGMENT ANALYSIS — "Which Parts of the Business Are Good?"

Nemetschek has four segments, each with different brands:

| Segment | Key Brands | What They Do | FY24 Share |
|---------|-----------|-------------|-----------|
| **Design** | Allplan, Vectorworks, Graphisoft | Architectural design software (BIM) | 49% |
| **Build** | Bluebeam, GoCanvas | Construction execution & documentation | 34% |
| **Manage** | Spacewell | Building management & operations | 5% |
| **Media** | Maxon (Cinema 4D, Redshift) | 3D rendering & visual effects | 12% |

**Key insights to know:**
- **Design** is the largest and most stable. Margin expanding (27.7% → 29.7%) = subscription transition working
- **Build** grew fastest (+28.4%) but includes GoCanvas. Organic growth was 18.0%. Margin declined (35.1% → 31.8%) because GoCanvas drags it down
- **Manage** is the problem child. Revenue declined 1.1% with only 10.2% EBITDA margin. Your MEDIUM risk finding
- **Media** has the best margins (36.5%) but organic growth was flat (-0.1%). Maxon is a mature business

> **Interview Q:** *"If you were advising a buyer, which segment would concern you most?"*
> **Your answer:** "Manage, which is Spacewell. It's the only segment with declining revenue, and even though its margin improved from 3.6% to 10.2%, it's still far below the group average of 30%. It's only 5% of revenue, so it's not material to the group, but strategically it raises the question of whether Nemetschek has the right product-market fit in building management. In a due diligence, I'd ask management whether they're considering divesting it or doubling down with investment."

---

## PART 9: INDUSTRY CONTEXT — "Why Nemetschek, Why AEC Software?"

### 9.1 AEC = Architecture, Engineering, Construction

Nemetschek operates in AEC software — tools used to design, build, and manage buildings and infrastructure. This market is undergoing digitization (moving from paper/manual processes to software), which is a massive tailwind.

### 9.2 BIM = Building Information Modeling

The key technology trend. BIM creates a digital 3D model of a building that contains all the data — materials, costs, timelines, structural properties. Governments increasingly mandate BIM for public projects (UK, Germany, Nordics). This drives adoption of Nemetschek's Design segment products.

### 9.3 Why the Americas Growth Matters

The US is the largest construction market globally but has been slower to adopt BIM software compared to Europe. Nemetschek's Americas share growing from 30.5% to 40.4% means they're capturing this under-penetrated market. GoCanvas (US-based, construction field operations) is part of this strategy.

### 9.4 The Rule of 40

**What it is:** A SaaS benchmark that says Revenue Growth % + EBITDA Margin % should exceed 40%.

**Nemetschek FY24:** 16.9% growth + 30.2% margin = **47.1%** → passes comfortably.

This is a quick one-liner that shows you know SaaS benchmarks. Interviewers at tech or consulting firms often know it.

---

## PART 10: LIKELY INTERVIEW QUESTIONS (RAPID FIRE)

**Q: Walk me through the project in 60 seconds.**
> "I built a Quality of Earnings analysis for Nemetschek, the German AEC software company, using their actual annual report data from 2020 to 2024. I extracted financial data from five years of annual reports, analyzed it across ten dimensions — revenue quality, ARR, organic vs inorganic growth, segment profitability, cash conversion, working capital, and more — and presented findings in the Big 4 Transaction Services format. The key story is a company successfully transitioning from perpetual licenses to subscriptions — recurring revenue went from 60% to 87% of total. The main risk is the €665 million GoCanvas acquisition, which changed the balance sheet from net cash to net debt."

**Q: What's the single most important number in your analysis?**
> "Recurring revenue reaching 86.5% of total, up from 60.2% five years ago. It means the vast majority of Nemetschek's revenue is now contracted and predictable. Combined with an ARR of €1.02 billion exceeding reported revenue, it tells me the earnings are high quality and the growth is sustainable."

**Q: What surprised you most?**
> "How dramatically the balance sheet changed in one year. Going from essentially zero debt to €500 million in long-term borrowings for a single acquisition is a bold move. The business can service it — debt-to-EBITDA is only 1x — but it shows a strategic shift from conservative European capital management to a more aggressive US-style growth-through-acquisition approach."

**Q: What would you do differently?**
> "Two things. First, I'd want net revenue retention data — it's the single most important SaaS metric I couldn't calculate from public filings. Second, I'd add a peer comparison — benchmarking Nemetschek's margins and growth against Autodesk, Trimble, and RIB Software to contextualize whether these numbers are good relative to peers, not just in absolute terms."

**Q: How did you build the Excel workbook?**
> "I used Python with openpyxl to programmatically generate all eight tabs. This wasn't just formatting — I extracted data from annual report PDFs, cross-verified numbers across overlapping reports, calculated derived metrics like DSO and cash conversion ratios, and built the workbook with consistent formatting, embedded charts, and source citations on every data point. The automation means I can regenerate the entire workbook if new data comes in."

**Q: Why not use Power BI or Tableau for the dashboard?**
> "For a portfolio project that needs to be self-contained and shareable without requiring software licenses, a single HTML file with Chart.js is more practical. It runs in any browser with no dependencies. In a real work setting, I'd absolutely use Power BI — it offers better interactivity, data refresh, and collaboration. The HTML dashboard shows I understand visualization principles; Power BI would be the production tool."

---

## PART 11: WHAT TO READ NEXT (2-3 Hours Total)

**Priority 1 (1 hour) — SaaS Metrics:**
- Search: "SaaS metrics guide for investors" (Bessemer Venture Partners publishes a great free one)
- Key terms to lock in: ARR, MRR, NRR (net revenue retention), GRR (gross revenue retention), CAC, LTV, Rule of 40
- You need this because SaaS metrics are the vocabulary of the analysis

**Priority 2 (30 min) — QoE Basics:**
- Search: "quality of earnings analysis due diligence" + any Big 4 blog
- Look for Deloitte or PwC articles explaining vendor due diligence
- You need this because it frames *why* the analysis exists

**Priority 3 (30 min) — Goodwill & PPA:**
- Review your accounting textbook chapter on business combinations
- Key: goodwill creation, PPA intangible assets, impairment testing
- You need this because GoCanvas is your highest-risk finding

**Priority 4 (30 min) — Nemetschek's Business:**
- Read the Company Presentation 2024 PDF (it's in your Reports folder — it's the short, visual overview)
- Know the four segments, the key brands, and the AEC market context
- You need this because interviewers will ask "tell me about the company"

**Optional — Peer Context:**
- Look up Autodesk's recent earnings (they completed a similar subscription transition 2-3 years ago)
- Knowing that "Autodesk's transition caused a temporary revenue dip before accelerating" lets you contextualize Nemetschek's journey

---

*Study this guide → re-read the methodology doc → flip through the Excel tabs → you're ready to present it.*
