# Decision Gates & Evaluation Criteria

Every stage of the **App Idea Validation Protocol** concludes with an explicit **Decision Gate**. A decision gate prevents premature progression, halts confirmation bias, and mandates a documented choice: **Continue (Pass)**, **Pivot**, or **Kill (Halt)**.

---

## 1. The Three Gate Outcomes

1. **Continue (Pass / استمرار):** The candidate idea satisfies all mandatory criteria, evidence thresholds, and minimum benchmarks for the current stage. The team advances to the immediate next stage.
2. **Pivot (تعديل المسار):** The underlying problem or market exhibits genuine demand, but the specific angle, audience segment, distribution channel, pricing model, or feature hypothesis failed verification. The core premise is adjusted and re-tested without re-inventing the foundational research.
3. **Kill (إيقاف الفكرة):** The candidate idea violates a non-negotiable constraint, faces insurmountable structural hurdles (e.g., heavily regulated legal/medical domains without capital), or shows zero empirical demand across multiple test angles. The idea is retired with zero financial loss and documented lessons.

---

## 2. Taxonomy of Criteria & Thresholds

To prevent dogmatic rigidity, this protocol classifies decision metrics into four distinct categories:

| Category | Definition | Example from Protocol | Rigidity |
|---|---|---|---|
| **Mandatory Constraints** | Non-negotiable physical, financial, legal, or skill boundaries defined at project inception. | Zero budget for paid cloud servers; builder cannot write native Swift. | **Absolute.** If violated, kill or discard immediately. |
| **Evidence Thresholds** | Observable empirical data points required from credible independent sources. | Competitor generating verified >\$10k/mo revenue; new entrant (<12 mo) demonstrating monetization. | **High.** Cannot be waived without documented empirical substitute. |
| **Heuristic Thresholds** | Practical operational rules of thumb used to make rapid triage decisions under uncertainty. | 300+ waitlist signups in 14 days; >100k views on problem videos; 17–20% 2-year \$1k/mo threshold. | **Contextual.** Directional guidelines that can be calibrated to niche size and audience. |
| **Hypotheses Requiring Experiments** | Unproven assumptions regarding customer psychology, switching behavior, or willingness to pay. | "Users will switch from the default clock app if an alarm requires a physical photo check." | **Tentative.** Must be marked `Hypothesis` until proven by review mining or landing tests. |

---

## 3. Stage-by-Stage Decision Gate Reference

### Stage 0: Constraints Gate
- **Check:** Does the candidate idea stay within recorded capital limits, existing technical proficiencies, available daily hours, and acceptable regulatory risks?
- **Kill Trigger:** Requires external seed capital, unmastered low-level platform code, or enters restricted financial/health sectors.

### Stage 1 & 2: Macro Market & Distribution Realities Gate
- **Check:** Is consumer spending in the category growing faster than download growth (indicating willingness to pay rather than a vanity volume trap)? Are subscription benchmarks realistic?
- **Kill Trigger:** Category monetization is entirely advertising-dependent or dominated by zero-margin commoditized offerings.

### Stage 3: The 10 Idea Elimination Filters Gate
- **Check:** Does the idea pass all 10 filters?
  1. Zero fixed infrastructure cost (on-device processing or per-user API coverage).
  2. Solo buildable within 4–8 weeks.
  3. Proven niche with statistical backing.
  4. Organic \$0 distribution channel viability (viral short-form or ASO intent).
  5. Decisive subscription or upfront monetization (no "we'll add ads later").
  6. Free from complex regulatory or licensing burdens.
  7. iOS-first viability (or demonstrated regional equivalent where spending is concentrated).
  8. Frequent recurring problem (at least weekly cadence to prevent 30%+ higher churn).
  9. Clean-room development (zero cloning of proprietary code, assets, or trademarks).
  10. Proven recent willingness to pay within the niche over the past 12 months.
- **Decision:** Failing even a single filter requires an explicit pivot or immediate elimination.

### Stage 4: Three-Proof Shortlist Gate
- **Check:** Can the candidate supply three independent proofs in the exact same direction?
  1. Incumbent giants actively monetizing now.
  2. Recent entrant (<12 months old) proving the door remains open today.
  3. Statistically defensible niche gap (few focused apps, high new-entrant revenue share).
- **Decision:** 3 proofs = Top candidate. 2 proofs = Defer. 0–1 proofs = Kill.

### Stage 5 & 6: Problem Definition & Complaint Mining Gate
- **Check:** Are hypothesized switching reasons verified by 1–2 star customer reviews of top competitors?
- **Decision:** If negative reviews contradict the hypothesis or show users do not care about the proposed differentiation, revise the angle (`Pivot`) before designing any screens.

### Stage 7: The 14-Day \$0 Pre-Validation Gate
- **Check:** Perform a 14-day zero-budget validation sprint using problem-focused short-form video and a simple landing page waitlist.
  - **Pass Threshold (Guideline):** ≥300 qualified waitlist signups or ≥1 video surpassing 100k views with high comment intent. Proceed to MVP scoping.
  - **Fail / Pivot Threshold:** <100 waitlist signups and <10k total reach. Pivot the angle or messaging without having spent capital.
- *Calibration Note:* For ultra-vertical B2B or niche professional tools, absolute signup volume may be lower (e.g., 25–50 verified target professionals) provided high intent is verified.

### Stage 8: MVP Scope Boundary Gate
- **Check:** Strictly 3–5 core capabilities focused on the primary switching reason. Every nice-to-have feature is relegated to the explicit anti-feature / deferred list.
- **Kill Trigger:** Inability to launch a monetizable build within 4–8 weeks due to runaway feature creep.

### Stage 9: Conservative Economics Gate
- **Check:** Do conservative scenarios (using industry median conversion of 2–5% freemium, 5–12% paywall, 45% trial-to-paid, and 8–10% monthly churn) yield acceptable unit economics covering ongoing variable costs?
- **Decision:** If positive unit economics require unrealistic assumptions (e.g., 25% conversion or zero churn), re-structure pricing or kill.

### Stage 10: Post-Launch Kill & Pivot Rules Gate
- **Check:** Post-launch telemetry tracking Day 1, Day 7, Day 30 retention and paywall conversion.
- **Rule:** If D1 < 25% or D30 < 5% or payment conversion < 2% after two documented, disciplined product iterations, execute an immediate pivot to an alternative angle within the same domain.
