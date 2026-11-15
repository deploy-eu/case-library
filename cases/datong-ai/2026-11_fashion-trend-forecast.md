---
title: "Trend forecast for style elements with short, gappy data"
authors: ["DATONG AI"]
date: "not disclosed"
status: "live"
country: "not disclosed"
industry: "retail / fashion"
company_size: "not disclosed"
existing_systems: ["online buzz data", "search volume data"]
ai_and_tools: ["forecasting models", "dashboard"]
walls: ["data-quality"]
effort: "not disclosed"
anonymised: "yes"
consent: "client agreed to publication of the anonymised case (as on the public page linked below)"
review: "pending: awaiting review by a second maintainer"
---

# Trend forecast for style elements with short, gappy data

> **Disclosure:** written by DATONG AI, the company of a Deploy@EU management team member. The community does not endorse any company. Based on the public case page linked below, published with the client's consent. **Review by a second maintainer: pending.**

> **Summary:** A fashion retailer forecasts how style elements develop from online buzz and search volume. The model borrows information from related elements; specialists decide what enters range planning. Accepted by the client.

## 1. The business problem
Many style elements, but only monthly values for each. Search data had gaps and sudden jumps, so one element's history alone said little about its direction, and similar styles were hard to compare.

## 2. What was already there
Monthly online buzz and search volume series. No data about individual customers.

## 3. What was built
```
buzz and search data prepared by the same rules, gaps marked (auto)
→ model estimates the trend, drawing on related elements (AI)
→ forecasts for elements and style groups in a dashboard (auto)
→ specialists review against business context and decide (person)
```
- Several forecasting models were compared for short, medium and long horizons.
- The client received a retrainable model, the tested model set and the dashboard.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| Direction of a trend called correctly | 60% | 85% | reported in project documents; sample and method not documented |

## 5. Where it got stuck
- **Too few data points per series.** With monthly values and gaps, single-series forecasting did not work; the missing information had to come from related series.
- **Definitions first:** what counts as an element, which period matters, how gaps are handled.
- **Quality depends on the horizon.** It had to be measured for exactly the period the planning decisions are made for.

## 6. What we would do differently
Document the evaluation sample and method alongside the result, so the accuracy figures can be checked later.

## 7. Links
- Public case page: https://datongai.de/en/projects/fashion-trend-forecast/

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
