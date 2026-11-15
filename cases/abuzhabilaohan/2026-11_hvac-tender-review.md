---
title: "Reading HVAC tenders: equipment list and first bid assessment"
authors: ["Abuzhabilaohan"]
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
title_zh: "读暖通招标文件：设备清单和初步投标评估"
summary_zh: "图纸和技术规范变成一份和图纸位置关联的设备清单，并给出自家产品的推荐和初步评估。图纸识别已在客户那里使用；选型和评估是已完成的演示。"
industry_zh: "建筑设备 / 暖通空调"
title_de: "HLK-Ausschreibungen lesen: Geräteliste und erste Angebotsbewertung"
summary_de: "Aus Zeichnungen und Leistungsverzeichnis entsteht eine mit der Zeichnung verknüpfte Geräteliste, mit Vorschlägen aus dem eigenen Sortiment und einer ersten Bewertung. Die Zeichnungserkennung läuft beim Kunden; Auswahl und Bewertung sind eine fertige Demo."
industry_de: "Gebäudetechnik / HLK"
title_fr: "Lire des appels d'offres CVC : liste d'équipements et première évaluation"
summary_fr: "Plans et cahier des charges deviennent une liste d'équipements reliée au plan, avec des suggestions tirées de la gamme de l'entreprise et une première évaluation. La reconnaissance des plans est en service chez le client ; sélection et évaluation sont une démo terminée."
industry_fr: "génie climatique / CVC"
title_it: "Leggere gare HVAC: elenco apparecchi e prima valutazione dell'offerta"
summary_it: "Disegni e capitolato diventano un elenco di apparecchi collegato al disegno, con proposte dalla gamma aziendale e una prima valutazione. Il riconoscimento dei disegni è in uso presso il cliente; selezione e valutazione sono una demo completata."
industry_it: "impianti / HVAC"
title_es: "Leer licitaciones de climatización: lista de equipos y primera evaluación"
summary_es: "Planos y pliego se convierten en una lista de equipos vinculada al plano, con propuestas de la gama propia y una primera evaluación. El reconocimiento de planos ya se usa en el cliente; la selección y la evaluación son una demo terminada."
industry_es: "instalaciones / climatización"
review: "pending: awaiting review by a second maintainer"
---

# Reading HVAC tenders: equipment list and first bid assessment

> **Disclosure:** written by Abuzhabilaohan, a Deploy@EU management team member, about a project delivered by DATONG AI, the team he works with. The community does not endorse any company. Based on the public case page linked below, published with the client's consent. **Review by a second maintainer: pending.**

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
