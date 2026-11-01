# Evidence Standards & Data Freshness Policy

A defining characteristic of the **App Idea Validation Protocol** is its strict evidentiary discipline. This document outlines the standards used to classify claims, verify external data, handle missing or contradictory metrics, and prevent confirmation bias.

---

## 1. The Tripartite Evidence Classification

Every factual statement, metric, or strategic conclusion in a validation dossier must be explicitly labeled using one of three categories:

### 1. `مشاهَد` (Observed Fact)
- **Definition:** Directly documented data points extracted from credible, publicly identifiable sources, official store listings, or first-party analytics.
- **Requirements:** Must cite the author/source, publication title, direct URL or methodology, and the specific date or observation window.
- **Example:** `"Sensor Tower reports global mobile consumer spending reached $167B in 2025 (State of Mobile 2026 report, published Jan 2026)."`

### 2. `استنتاج` (Inference)
- **Definition:** A logical or mathematical deduction derived directly from one or more observed facts.
- **Requirements:** Must state the explicit logical premise connecting the observation to the deduction. Cannot add unproven assumptions.
- **Example:** `"Because consumer spending grew +10.6% while downloads grew only +0.8%, market growth is driven by increased user monetization efficiency rather than net new user acquisition."`

### 3. `فرضية` (Hypothesis)
- **Definition:** An unverified assumption, strategic conjecture, or behavioral prediction that has not yet been proven in the target market.
- **Requirements:** Must be treated as unproven risk until tested by customer review mining, landing page conversion, or behavioral telemetry. Never treat absence of refutation as positive proof.
- **Example:** `"Solo remote workers will pay $4.99/month for an alarm app requiring a webcam photo verification."`

---

## 2. Source Quality Hierarchy

When researching markets, competitors, and benchmarks, prioritize sources using the following hierarchy:

| Tier | Source Category | Description & Typical Examples | Reliability |
|---|---|---|---|
| **Tier 1** | **Direct Platform & Regulatory Filings** | Apple Developer, Google Play Console policies, SEC filings, official store developer agreements. | Authoritative for policy, fees, and rules. |
| **Tier 2** | **First-Party Aggregate Benchmarks** | Anonymized data across tens of thousands of active apps (e.g., RevenueCat State of Subscription Apps, Adjust, AppsFlyer). | Highest empirical reliability for conversion and retention medians. |
| **Tier 3** | **Established Market Intelligence** | Sensor Tower, Appfigures, Data.ai, Business of Apps, TechCrunch research. | Excellent for macroeconomic trends, store rankings, and directional revenue estimates. |
| **Tier 4** | **Direct Voice-of-Customer Data** | Public 1–2 star app reviews on iOS App Store & Google Play, Reddit community threads, user interviews. | Ground truth for specific user grievances, usability hurdles, and feature requests. |
| **Tier 5** | **General Tech Blogs & Uncited Posts** | Medium articles, marketing blogs, AI-generated summaries without original citations. | **Unacceptable** as evidence without tracing to primary source. |

---

## 3. Publication Date vs. Measurement Window

Always differentiate between:
- **Publication Date:** The calendar date on which a report or article was released (e.g., February 2026).
- **Measurement Window:** The actual historical period during which data was collected (e.g., calendar year 2025, or Q1–Q3 2025).

A report published in 2026 frequently analyzes data from 2025. Conflating the two distorts growth velocity calculations.

---

## 4. Handling Missing Data

When researching a niche, key figures (e.g., exact revenue for a private bootstrapped competitor) may be inaccessible:
- **Never Invent Numbers:** Prohibit guessing or presenting speculative approximations as factual numbers.
- **Document "Data Unavailable":** Explicitly note `غير متوفر في المصادر المتاحة` (Not available in accessible sources).
- **Construct Measurable Proxies:** Substitute an observable proxy metric:
  - If monthly revenue is unknown, record total review count velocity (new reviews per month) combined with store category ranking history.
  - If churn is unknown, use industry benchmark ranges from RevenueCat for the corresponding category.

---

## 5. Resolving Conflicting Sources

When two reputable sources provide divergent figures (e.g., Sensor Tower estimating $50k/mo revenue while Appfigures estimates $30k/mo):
1. **Document Both Figures:** State the range and disclose the methodology difference.
2. **Adopt Conservative Values:** For revenue and conversion calculations, use the conservative (lower) figure.
3. **For Cost Estimates:** Use the higher figure to ensure unit economics withstand worst-case pressure.

---

## 6. Communicating Confidence & Uncertainty

A validation dossier must never project false certainty. Recommendations should always communicate:
- The sample size of competitor reviews mined.
- The age and geography of benchmark reports used.
- The boundary conditions under which conclusions remain valid.
