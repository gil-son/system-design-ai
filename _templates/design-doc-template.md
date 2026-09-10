# Design: [System Name]

> Prompt: "Design a production-grade [X] for [Y] users."

**Status:** Draft / Reviewed / Final
**Date:**
**Related diagrams:** `../../diagrams/[name].png`

---

## 1. Requirements
**Functional:**
-

**Non-functional:**
- Latency:
- Availability:
- Throughput:
- Consistency:

## 2. Constraints
-

## 3. Capacity Estimation
- Traffic (avg / peak):
- Storage:
- Bandwidth:
- Back-of-envelope math:

## 4. High-Level Architecture
_(diagram + one-paragraph description)_

## 5. Data Flow
_(step-by-step, request → response)_

## 6. API / Interfaces
```
POST /endpoint
{
  ...
}
```

## 7. Storage
- What's stored, where, why this choice over alternatives

## 8. Scaling
- Bottlenecks and how each is addressed

## 9. Reliability
- Failure modes, redundancy, retries, fallback behavior

## 10. Security
- AuthN/AuthZ, data protection, PII handling

## 11. Observability
- Metrics, logging, tracing, alerting

## 12. Cost
- Rough cost drivers and levers to reduce them

## 13. Trade-offs
- Key decisions and what was given up

## 14. Failure Scenarios
- What breaks first under load / partial outage, and the mitigation

## 15. Evolution / Future Improvements
- What v2 looks like
