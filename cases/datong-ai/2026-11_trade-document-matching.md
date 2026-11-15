---
title: "Four-way document matching for commodity orders"
authors: ["DATONG AI"]
date: "not disclosed"
status: "live"
country: "not disclosed"
industry: "wholesale / trade"
company_size: "not disclosed"
existing_systems: ["messenger", "spreadsheets", "trading system"]
ai_and_tools: ["document recognition", "rule-based matching", "status overview"]
walls: ["data-quality"]
effort: "not disclosed"
anonymised: "yes"
consent: "client agreed to publication of the anonymised case (as on the public page linked below)"
review: "pending: awaiting review by a second maintainer"
---

# Four-way document matching for commodity orders

> **Disclosure:** written by DATONG AI, the company of a Deploy@EU management team member. The community does not endorse any company. Based on the public case page linked below, published with the client's consent. **Review by a second maintainer: pending.**

> **Summary:** Contracts, invoices, shipping documents and payment records arrive through different channels. They are now collected, read and matched per order by fixed rules; staff resolve the flagged mismatches.

## 1. The business problem
Each deal has four document types. Staff typed them by hand into several spreadsheets and compared them item by item. Fields went missing, company names did not match, and the only way to learn an order's status was often to ask someone.

## 2. What was already there
A messenger, several spreadsheets and the existing trading system. Documents arrive through different channels.

## 3. What was built
```
documents collected from all channels (auto) → key fields recognised (AI)
→ contract, invoice, shipping documents and payment linked by order and contracting party (rules)
→ mismatches and missing steps flagged → documentation staff open the original and resolve
```
- Results, mismatch alerts and open tasks are on one page; staff and management see them by role.
- Financing decisions, such as discounting a bill of exchange early, stay with management.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| Time spent entering documents | 100% | about 10% | estimated by the client; method unknown to us |

## 5. Where it got stuck
- **Unclear definitions.** Before matching could be automated, the team had to settle what an order number is, who counts as the contracting party, and how document fields relate.
- **Company names did not match** between documents, and fields were missing.
- **A mismatch alert alone was useless.** It only helped once each alert led straight to the original document, so staff could decide immediately.

## 6. What we would do differently
Agree the definitions of order and contracting party in writing before building any recognition.

## 7. Links
- Public case page: https://datongai.de/en/projects/trade-document-matching/

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
