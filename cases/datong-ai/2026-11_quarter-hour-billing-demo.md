---
title: "Quarter-hour billing for shared solar power: a rules-only demo"
authors: ["DATONG AI"]
date: "not disclosed"
status: "pilot"
country: "Germany"
industry: "energy / utilities"
company_size: "not applicable (demo, no client)"
existing_systems: ["15-minute meter readings (simulated)", "the utility's billing system (CSV import)"]
ai_and_tools: ["web application", "EU-hosted database", "AI assistants for code and article drafts"]
walls: ["reliability"]
effort: "not disclosed"
anonymised: "yes"
consent: "client agreed to publication of the anonymised case (as on the public page linked below)"
review: "pending: awaiting review by a second maintainer"
---

# Quarter-hour billing for shared solar power: a rules-only demo

> **Disclosure:** written by DATONG AI, the company of a Deploy@EU management team member. The community does not endorse any company. Based on the public case page linked below, published with the client's consent. **Review by a second maintainer: pending.**

> **Summary:** A demo for utilities: solar power shared among the sites of one legal entity is allocated and balanced for every quarter hour of a month. The calculation uses fixed rules only. It runs on simulated data; no utility has used it in operation.

## 1. The business problem
A customer with several sites, some generating solar power and some consuming it, wants the power shared among its own sites and billed per quarter hour. Many utilities have no ready process for this, so requests are declined or left open.

## 2. What was already there
Nothing at a client. The demo assumes 15-minute readings per site and a billing system that can import a CSV file.

## 3. What was built
```
readings for all sites (simulated from weather and load profiles) → person chooses one of three allocation rules
→ distribution between sites per quarter hour, 96 values a day (rules)
→ balance check: generation = self-consumption + sharing + grid feed-in (auto)
→ monthly figures → billing table as CSV → person checks and passes it on
```
- **No AI in the calculation.** The same readings and rule must give the same bill every time, and an auditor must be able to trace each amount.
- Only the billing sub-ledger is covered. Money flows, the supplier role, market communication and the customer relationship stay with the utility.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| Balance difference over a full month (96 × 31 quarter hours) |  | 0 | measured on simulated data |
| Allocation rules running end to end |  | 3 of 3 | demo test |
| Errors found by sentence-by-sentence checking in one AI-drafted technical article |  | 22 | counted |

## 5. Where it got stuck
- **A regulatory change made the first legal model unworkable.** The demo had to be repositioned: it now targets utilities and covers only the sub-ledger, with no money flowing through it.
- **AI-drafted text contained plausible errors.** In the fourth technical article a person found 22, and only by checking every sentence.
- **Simulation proves the arithmetic, not the usefulness.** Without real meter readings from a utility, nobody knows whether it holds up in daily work.
- Database access rights had to be reviewed and tightened before the demo was shown.

## 6. What we would do differently
Find a utility willing to provide one month of real readings before building the second version.

## 7. Links
- Public case page: https://datongai.de/en/projects/utility-billing-demo/

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
