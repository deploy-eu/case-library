---
title: "Assigning incoming letters to tenant companies: a prototype"
authors: ["DATONG AI"]
date: "not disclosed"
status: "pilot"
country: "Germany"
industry: "business centre / office services"
company_size: "not disclosed"
existing_systems: ["paper mail", "scanner", "tenant list"]
ai_and_tools: ["OCR", "document classification", "entity matching", "review page"]
walls: ["data-quality"]
effort: "not disclosed"
anonymised: "yes"
consent: "client agreed to publication of the anonymised case (as on the public page linked below)"
review: "pending: awaiting review by a second maintainer"
---

# Assigning incoming letters to tenant companies: a prototype

> **Disclosure:** written by DATONG AI, the company of a Deploy@EU management team member. The community does not endorse any company. Based on the public case page linked below, published with the client's consent. **Review by a second maintainer: pending.**

> **Summary:** A business centre receives mail for several hundred tenant companies. A prototype reads scanned letters and suggests the tenant; a person confirms every assignment. It was tested with real sample letters and handed to the client's IT.

## 1. The business problem
All tenant mail arrives in one place. Each letter must be looked at, assigned to the right company and passed on. Several hundred companies have similar names, and a wrong assignment is embarrassing for the centre.

## 2. What was already there
Paper mail, a scanner and the list of tenant companies.

## 3. What was built
```
person scans the letter → sender, recipient and letter type recognised (AI)
→ tenant company suggested by entity matching (auto) → person confirms or corrects on a review page
```
- An evaluation with letters whose correct answer was known counts how often the suggestion is right.
- The prototype is not in production. The client's IT is developing it further.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| Assignment accuracy |  | evaluated, figure not published | measured, not disclosed |
| Time saved |  |  | none: not in live operation |

## 5. Where it got stuck
- **Similar company names.** Among several hundred tenants many names differ only slightly, which is the core difficulty of the matching.
- **The decision needed evidence.** The client wanted to know whether sorting can be automated reliably before funding a full system, so the work stopped at a measured prototype.
- **Hand-over instead of roll-out:** the client's own IT continues the build, so the prototype had to be documented for someone else.

## 6. What we would do differently
Publish the accuracy figure with the client's agreement; a prototype case is much more useful with its number.

## 7. Links
- Public case page: https://datongai.de/en/projects/incoming-mail/

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
