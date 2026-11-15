---
title: "Reading HVAC tenders: equipment list and first bid assessment"
authors: ["DATONG AI"]
date: "not disclosed"
status: "pilot"
country: "not disclosed"
industry: "building services / HVAC"
company_size: "not disclosed"
existing_systems: ["drawings", "specifications", "product range", "territory rules", "technical documents"]
ai_and_tools: ["drawing recognition", "company knowledge base", "report generation"]
walls: ["data-quality"]
effort: "not disclosed"
anonymised: "yes"
consent: "client agreed to publication of the anonymised case (as on the public page linked below)"
review: "pending: awaiting review by a second maintainer"
---

# Reading HVAC tenders: equipment list and first bid assessment

> **Disclosure:** written by DATONG AI, the company of a Deploy@EU management team member. The community does not endorse any company. Based on the public case page linked below, published with the client's consent. **Review by a second maintainer: pending.**

> **Summary:** Drawings and specifications become an equipment list linked to the drawing, with suggestions from the company's own range and a first assessment. Drawing recognition is in use at the client; selection and assessment are a finished demo.

## 1. The business problem
Engineers and sales engineers read every drawing, marked and counted equipment by hand, and compared it with the specification and their own range. A missed unit led to a wrong bid.

## 2. What was already there
Tender drawings and specifications from many design offices, the company's product range, territory rules and technical documents.

## 3. What was built
```
person uploads drawings and specification, confirms document types
→ AI reads equipment type, tag, quantity, technical values; keeps drawing location and page
→ AI suggests equipment from the range, with sources, and lists open questions
→ short report with a score (auto) → engineers confirm quantities and selection
→ project team decides on bidding and price
```
- Every statement can be traced to paragraph, table, value and page.
- The score only helps decide how much more time to invest. Costing and bid writing are still being developed.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| First assessment of a tender | 3–5 days (client's estimate) | about 20 min plus engineer review | reported in a project presentation; not measured under the same conditions |
| Equipment correctly recognised on drawings | about 70% | over 90% | reported; sample and test standard not documented |

## 5. Where it got stuck
- **Every design office draws differently.** The same equipment appears with different symbols and labels.
- **A list without locations could not be corrected.** Each line had to link back to its place on the drawing before engineers could check it.
- **Technically suitable was not enough.** A unit must also be in the company's range and sales territory.
- **Two different times were mixed up:** time to a first assessment and time to a finished bid, which also includes review, costing and approval.

## 6. What we would do differently
Record the two times separately from the first day, and define the test sample for recognition accuracy so the figures can be compared.

## 7. Links
- Public case page: https://datongai.de/en/projects/hvac-tender-review/

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
