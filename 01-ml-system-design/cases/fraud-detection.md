# Design: Fraud Detection System

> Prompt: "Design a fraud detection system for a bank processing 50M transactions/day."

**Status:** In Progress
**Date:** 2026-09
**Related diagrams:** `../../diagrams/fraud-detection.png` _(not yet created)_
**Related solutions:** [`solutions/aws/fraud-detection-solution.md`](../solutions/aws/fraud-detection-solution.md)

---

## 1. Requirements
**Functional:**
- Score every transaction in real time (approve / decline / flag for review)
- Support rule-based overrides alongside ML scoring
- Provide explainability for flagged transactions (regulatory requirement)
- Allow human analysts to review and label flagged cases (feedback loop)

**Non-functional:**
- Latency: <100–300ms per decision (transaction can't hang)
- Availability: 99.99%+ (system going down blocks all payments)
- Throughput: 50M/day ≈ ~580 TPS average (Transactions Per Second); design for 5–10x peak (Black Friday, lunch hour)
- Consistency: eventual consistency fine for model updates; the transaction decision itself must be strongly consistent (no double-approval)

## 2. Constraints
- Class imbalance: fraud is ~0.1–0.5% of transactions — accuracy is a useless metric
- Cost asymmetry: false negative (missed fraud) vs. false positive (blocked legit purchase) have very different business costs
- Adversarial environment: fraudsters adapt to the model, so it decays faster than typical ML systems
- Regulatory: decisions often need to be explainable, not just a model score

## 3. Capacity Estimation
_(in progress — working through feature-store read/sec estimation and storage implications)_

## 4. High-Level Architecture
_(TODO)_

### Architecture Diagram
_(TODO)_

## 5. Data Flow
_(TODO)_

## 6. API / Interfaces
_(TODO)_

## 7. Storage
_(TODO)_

## 8. Scaling
_(TODO)_

## 9. Reliability
_(TODO)_

## 10. Security
_(TODO)_

## 11. Observability
_(TODO)_

## 12. Cost
_(TODO)_

## 13. Trade-offs
_(TODO)_

## 14. Failure Scenarios
_(TODO)_

## 15. Evolution / Future Improvements
_(TODO)_
