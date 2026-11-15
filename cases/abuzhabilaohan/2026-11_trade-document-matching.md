---
title: "Four-way document matching for commodity orders"
authors: ["Abuzhabilaohan"]
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
consent: "client agreed to publication of the anonymised case"
title_zh: "大宗贸易订单的四单匹配"
summary_zh: "合同、发票、运输单据和付款记录从不同渠道进来。现在按订单自动收集、识别，并用固定规则匹配；员工只处理被标出的不一致。"
industry_zh: "批发 / 贸易"
title_de: "Vierfach-Abgleich von Dokumenten für Rohstoffaufträge"
summary_de: "Verträge, Rechnungen, Versanddokumente und Zahlungen kommen über verschiedene Kanäle. Jetzt werden sie gesammelt, gelesen und pro Auftrag nach festen Regeln abgeglichen; das Team klärt die markierten Abweichungen."
industry_de: "Großhandel / Handel"
title_fr: "Rapprochement à quatre documents pour des commandes de matières premières"
summary_fr: "Contrats, factures, documents d'expédition et paiements arrivent par différents canaux. Ils sont désormais collectés, lus et rapprochés par commande selon des règles fixes ; l'équipe traite les écarts signalés."
industry_fr: "commerce de gros / négoce"
title_it: "Abbinamento a quattro documenti per ordini di materie prime"
summary_it: "Contratti, fatture, documenti di spedizione e pagamenti arrivano da canali diversi. Ora vengono raccolti, letti e abbinati per ordine con regole fisse; il team risolve le discrepanze segnalate."
industry_it: "commercio all'ingrosso"
title_es: "Conciliación de cuatro documentos para pedidos de materias primas"
summary_es: "Contratos, facturas, documentos de envío y pagos llegan por canales distintos. Ahora se recogen, se leen y se concilian por pedido con reglas fijas; el equipo resuelve las discrepancias marcadas."
industry_es: "comercio mayorista"
review: "pending: awaiting review by a second maintainer"
---

# Four-way document matching for commodity orders

> **Disclosure:** written by Abuzhabilaohan, a Deploy@EU management team member, about a project delivered by DATONG AI, the team he works with. The community does not endorse any company. Published with the client's consent. **Review by a second maintainer: pending.**

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

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
