---
title: "Quarter-hour billing for shared solar power: a rules-only demo"
authors: ["Abuzhabilaohan"]
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
title_zh: "共享光伏电的刻钟结算：只用规则的演示"
summary_zh: "给电力公司的演示：一家法人多个站点之间共享的光伏电，按月里每一刻钟分配并平衡。计算只用固定规则。目前跑在模拟数据上，还没有电力公司实际使用。"
industry_zh: "能源 / 公用事业"
title_de: "Viertelstundengenaue Abrechnung von geteiltem Solarstrom: eine Demo nur mit Regeln"
summary_de: "Eine Demo für Stadtwerke: Solarstrom, der zwischen den Standorten einer Gesellschaft geteilt wird, wird für jede Viertelstunde eines Monats verteilt und bilanziert. Gerechnet wird nur mit festen Regeln. Läuft auf simulierten Daten; noch kein Versorger nutzt sie im Betrieb."
industry_de: "Energie / Stadtwerke"
title_fr: "Facturation au quart d'heure de l'énergie solaire partagée : une démo à base de règles"
summary_fr: "Une démo pour les fournisseurs d'énergie : l'électricité solaire partagée entre les sites d'une même entité est répartie et équilibrée pour chaque quart d'heure du mois. Le calcul n'utilise que des règles fixes. Elle tourne sur des données simulées ; aucun fournisseur ne l'utilise encore."
industry_fr: "énergie / services publics"
title_it: "Fatturazione al quarto d'ora dell'energia solare condivisa: una demo solo a regole"
summary_it: "Una demo per le utility: l'energia solare condivisa tra le sedi di un'unica società viene ripartita e bilanciata per ogni quarto d'ora del mese. Il calcolo usa solo regole fisse. Gira su dati simulati; nessuna utility la usa ancora."
industry_it: "energia / multiutility"
title_es: "Facturación por cuartos de hora de energía solar compartida: una demo solo con reglas"
summary_es: "Una demo para comercializadoras: la energía solar compartida entre las sedes de una misma entidad se reparte y cuadra para cada cuarto de hora del mes. El cálculo usa solo reglas fijas. Funciona con datos simulados; ninguna comercializadora la usa todavía."
industry_es: "energía / suministros"
review: "pending: awaiting review by a second maintainer"
---

# Quarter-hour billing for shared solar power: a rules-only demo

> **Disclosure:** written by Abuzhabilaohan, a Deploy@EU management team member, about a project delivered by DATONG AI, the team he works with. The community does not endorse any company. Based on the public case page linked below, published with the client's consent. **Review by a second maintainer: pending.**

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
