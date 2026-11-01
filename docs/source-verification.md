# Source Verification Guide

This guide details how to verify external data points, audit competitor figures, and confirm platform policies when running the validation protocol. It also provides an audit of the baseline figures referenced in the original protocol.

---

## 1. Verification Procedures by Domain

### 1.1 App Store & Platform Policies
Platform developer rules change frequently and must be audited directly at official developer portals:
- **Apple Developer Program:**
  - Annual Enrollment Fee: \$99/year.
  - Small Business Program: 15% commission tier for developers earning under \$1,000,000 annually (requires separate enrollment application).
  - Official Verification URL: [developer.apple.com/programs](https://developer.apple.com/programs/)
- **Google Play Console:**
  - One-time Registration Fee: \$25.
  - Personal Account Testing Policy: For personal developer accounts created after November 13, 2023, Google mandates that apps must run a closed test with **at least 12 testers opted in for at least 14 days continuously** before applying for production access. (Note: Organization accounts are exempt from this specific requirement).
  - Official Verification URL: [support.google.com/googleplay/android-developer](https://support.google.com/googleplay/android-developer/)

### 1.2 Subscription & Conversion Benchmarks
Do not use generic blog posts for conversion rates. Benchmark against industry-wide aggregate datasets:
- **RevenueCat State of Subscription Apps:** Examines millions of subscriptions across tens of thousands of real applications.
  - Key metrics to verify: Day 1 / Day 7 / Day 30 retention rates, paywall conversion rates (freemium vs. hard paywall), free trial conversion rates (7-day vs. 14-day), and monthly churn medians.
  - Verification: Access the latest annual report at [revenuecat.com/state-of-subscription-apps](https://www.revenuecat.com/state-of-subscription-apps/).
- **Adjust / AppsFlyer Mobile Benchmarks:** Essential for cross-category retention curves and regional acquisition costs.

### 1.3 Competitor Revenue & Download Estimates
Public store listings display install bands (Google Play) and review counts, but not gross revenue. To estimate financial performance:
- **Third-Party Intelligence Tools:** Use Sensor Tower, Appfigures, Peekly, or Data.ai.
- **Verification Rule:** Treat all third-party revenue figures as **directional estimates**, not audited financial statements.
- **Triangulation Formula:** Cross-check the estimated revenue against total store review volume and category rank history. A consistent Top 50 category rank in major markets confirms significant volume.

### 1.4 Competitor Complaint Mining Verification
When mining 1–2 star reviews:
- Filter reviews by "Most Recent" rather than "Most Helpful" to capture current technical flaws and regression bugs.
- Look across multiple regions (e.g., US, UK, GCC/MENA) to distinguish localized localization failures from universal product defects.
- Cross-reference store reviews with dedicated Reddit communities (`r/apps`, `r/productivity`, or niche-specific subreddits) and platforms such as JustUseApp.

---

## 2. Audit of Protocol Baseline Reference Figures

The original protocol (`references/KHALIL_COLDSTART_PROTOCOL.md`) contains a set of reference data points compiled as a concrete benchmark snapshot (November 2026 baseline). When using the protocol, distinguish between these historical reference baselines and verified real-time numbers:

| Metric in Baseline Snapshot | Protocol Baseline Value | Source & Context | Verification Status / Rule for Agents |
|---|---|---|---|
| **Global Mobile Consumer Spend (2025)** | ~\$167B (+10.6% YoY) | Sensor Tower State of Mobile (2025/2026) | *Reference snapshot.* Must be refreshed with the latest calendar year report upon live analysis. |
| **Non-Game App Spend vs Games** | Non-game \$85.6B vs Games \$81.8B | Sensor Tower milestone reporting non-games surpassing games | *Directional market shift.* Verifiable trend indicating high utility app willingness-to-pay. |
| **iOS Subscription Dominance** | ~73% of subscription revenue on iOS | RevenueCat / Industry consensus | *Benchmark.* Confirms iOS-first prioritization for consumer subscription apps. |
| **New App \$1k/mo Threshold** | ~17–20% reach \$1,000/mo in 2 years | RevenueCat State of Subscription Apps | *Empirical distribution median.* Used to calibrate realistic expectations. |
| **New App \$10k/mo Threshold** | ~4.6–5.0% reach \$10,000/mo | RevenueCat State of Subscription Apps | *Empirical filter.* Illustrates revenue concentration. |
| **Top 1% Publisher Concentration** | Top 1% capture 92% of IAP revenue | Industry market reports | *Structural reality.* Emphasizes building in focused niches rather than broad categories. |
| **GCC / MENA IAP Growth** | +41% Q1 2024 to Q1 2026 | Regional reports (Bidease / InvestGame) | *Regional trend.* Arabic localization provides defensible organic moat. |
| **Google Play Closed Testing Policy** | 12 testers for 14 continuous days | Google Play Console developer policy (personal accounts) | *Policy check.* Confirm current Google Play Console developer requirements before planning launch timeline. |
| **Apple Small Business Program Fee** | 15% under \$1M revenue, \$99/yr membership | Apple Developer Agreement | *Current standard.* Verify active developer account status. |

---

## 3. Policy for AI Agents Using This Framework

When an AI assistant (such as Claude) executes this protocol:
1. It must explicitly declare whether figures are drawn from the **reference baseline** or from an **active live query**.
2. If real-time search or API lookup is unavailable, it must state: *"Based on the protocol's November 2026 baseline data; verify current numbers before committing capital."*
3. Agents are strictly forbidden from extrapolating speculative numbers without an identified methodology.
