---
title: "Drafting replies to price inquiries for a small importer (FICTIONAL EXAMPLE)"
authors: ["Deploy@EU maintainers"]
date: "2026-01"
status: "pilot"
country: "Germany"
industry: "wholesale / trade"
company_size: "10–49 employees"
existing_systems: ["Outlook", "Excel price list", "on-premise ERP without API"]
ai_and_tools: ["Claude", "Python"]
walls: ["legacy-desktop", "no-api", "data-quality"]
anonymised: "yes"
consent: "n/a — fictional"
---

# Drafting replies to price inquiries for a small importer

> ⚠️ **This is a fictional example** written to show how a case looks. The company, numbers and details are invented. It is not a real deployment.

> **Summary:** A fictional kitchen-appliance importer received ~40 price inquiries a week by email. An AI assistant now reads each inquiry, checks stock in an Excel export of the ERP, and drafts a reply with a quote for the salesperson to check and send.

## 1. The business problem
Two salespeople spent much of their mornings copying article numbers from emails into the ERP, checking stock, and writing quotes. Answers often took a day.

## 2. What was already there
Outlook; an Excel price list maintained by hand; an on-premise ERP with **no API** — only a nightly CSV stock export.

## 3. What was built
```
inquiry email → AI extracts articles & quantities → looks up price list + stock CSV
→ drafts quote and reply in Outlook → salesperson checks → sends
```
The AI never sends anything and never sets prices: prices come from the price list; anything outside it is flagged for the salesperson.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| Time to first reply | (fictional) | (fictional) | — |

In a real case, this table holds your measured numbers.

## 5. Where it got stuck
- The ERP had no API, so the nightly CSV was the only source; stock could be up to a day old.
- Article names differed between the price list, the ERP and customer emails ("same product, three names").

## 6. What we would do differently
Clean up article names first; it would have saved most of the debugging.
