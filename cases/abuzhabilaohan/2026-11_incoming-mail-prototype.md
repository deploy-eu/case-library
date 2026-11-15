---
title: "Assigning incoming letters to tenant companies: a prototype"
authors: ["Abuzhabilaohan"]
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
title_zh: "把来信分给入驻公司：一个原型"
summary_zh: "一家商务中心替几百家入驻公司收信。原型读取扫描后的信件并推荐收件公司，每一次分配都由人确认。用客户的真实样信测过，已交给客户的 IT 继续开发。"
industry_zh: "商务中心 / 办公服务"
title_de: "Eingehende Briefe Mieterfirmen zuordnen: ein Prototyp"
summary_de: "Ein Business Center nimmt Post für mehrere hundert Mieterfirmen an. Ein Prototyp liest gescannte Briefe und schlägt die Firma vor; jede Zuordnung bestätigt ein Mensch. Mit echten Beispielbriefen getestet und an die IT des Kunden übergeben."
industry_de: "Business Center / Bürodienstleistungen"
title_fr: "Attribuer le courrier entrant aux entreprises locataires : un prototype"
summary_fr: "Un centre d'affaires reçoit le courrier de plusieurs centaines d'entreprises. Un prototype lit les lettres numérisées et propose le destinataire ; chaque attribution est confirmée par une personne. Testé avec de vraies lettres et remis à l'informatique du client."
industry_fr: "centre d'affaires / services de bureau"
title_it: "Assegnare la posta in arrivo alle aziende ospitate: un prototipo"
summary_it: "Un business center riceve la posta di diverse centinaia di aziende. Un prototipo legge le lettere scansionate e propone il destinatario; ogni assegnazione è confermata da una persona. Testato con lettere reali e consegnato all'IT del cliente."
industry_it: "business center / servizi d'ufficio"
title_es: "Asignar el correo entrante a las empresas inquilinas: un prototipo"
summary_es: "Un centro de negocios recibe el correo de varios cientos de empresas. Un prototipo lee las cartas escaneadas y propone la empresa destinataria; cada asignación la confirma una persona. Probado con cartas reales y entregado al departamento de TI del cliente."
industry_es: "centro de negocios / servicios de oficina"
review: "pending: awaiting review by a second maintainer"
---

# Assigning incoming letters to tenant companies: a prototype

> **Disclosure:** written by Abuzhabilaohan, a Deploy@EU management team member, about a project delivered by DATONG AI, the team he works with. The community does not endorse any company. Based on the public case page linked below, published with the client's consent. **Review by a second maintainer: pending.**

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
