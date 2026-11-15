---
title: "Monthly payroll checks for client companies"
authors: ["Abuzhabilaohan"]
date: "not disclosed"
status: "live"
country: "Germany"
industry: "business services / payroll"
company_size: "not disclosed"
existing_systems: ["shared mailbox", "project board", "cloud storage", "payslips as PDF from the tax advisor"]
ai_and_tools: ["automation platform", "text extraction on servers in Germany", "LLM for drafts only"]
walls: ["no-api", "gdpr", "data-quality", "change-management"]
effort: "not disclosed"
anonymised: "yes"
consent: "client agreed to publication of the anonymised case"
title_zh: "核薪：每月为客户公司核对工资单"
summary_zh: "一家服务商每月为客户公司做工资核算。围绕税务师工资单的整条链路（提醒、归档、双向核对、成本明细、付款指令草稿）现在都自动跑；员工每家客户只需审批两份草稿。"
industry_zh: "企业服务 / 薪资核算"
title_de: "Monatliche Lohnprüfung für Kundenunternehmen"
summary_de: "Ein Dienstleister erledigt jeden Monat die Lohnabrechnung für Kundenunternehmen. Die Kette rund um die Lohnzettel des Steuerberaters (Erinnerungen, Ablage, beidseitiger Abgleich, Kostenaufstellung, Entwurf der Zahlungsanweisung) läuft jetzt automatisch; das Team gibt pro Kunde zwei Entwürfe frei."
industry_de: "Unternehmensdienstleistungen / Lohnabrechnung"
title_fr: "Contrôle mensuel de la paie pour des entreprises clientes"
summary_fr: "Un prestataire gère chaque mois la paie d'entreprises clientes. Toute la chaîne autour des bulletins du conseiller fiscal (relances, classement, rapprochement dans les deux sens, récapitulatif des coûts, projet d'ordre de paiement) tourne désormais automatiquement ; l'équipe valide deux brouillons par client."
industry_fr: "services aux entreprises / paie"
title_it: "Controllo mensile delle buste paga per aziende clienti"
summary_it: "Un fornitore gestisce ogni mese le buste paga di aziende clienti. Tutta la catena attorno ai cedolini del consulente fiscale (promemoria, archiviazione, verifica incrociata, riepilogo dei costi, bozza dell'ordine di pagamento) ora gira in automatico; il team approva due bozze per cliente."
industry_it: "servizi alle imprese / buste paga"
title_es: "Control mensual de nóminas para empresas clientes"
summary_es: "Un proveedor gestiona cada mes las nóminas de empresas clientes. Toda la cadena en torno a las nóminas del asesor fiscal (recordatorios, archivo, conciliación en ambos sentidos, desglose de costes, borrador de orden de pago) funciona ahora automáticamente; el equipo aprueba dos borradores por cliente."
industry_es: "servicios a empresas / nóminas"
review: "pending: awaiting review by a second maintainer"
---

# Monthly payroll checks for client companies

> **Disclosure:** written by Abuzhabilaohan, a Deploy@EU management team member, about a project delivered by DATONG AI, the team he works with. The community does not endorse any company. Published with the client's consent. **Review by a second maintainer: pending.**

> **Summary:** A service provider runs monthly payroll for client companies. The chain around the tax advisor's payslips (reminders, filing, two-way reconciliation, cost breakdown, draft payment instruction) now runs automatically; staff approve two drafts per client.

## 1. The business problem
For every client company and month the payroll team reminded HR, collected changes, forwarded them to the tax advisor, waited for payslips, checked them, and wrote a cost breakdown and payment instruction. Whether every reported change had been applied depended on individual attention, and each new client added the same amount of work.

## 2. What was already there
A shared mailbox, a project board, cloud storage. Payslips arrive from the tax advisor as PDF files; there is no interface to the payroll software.

## 3. What was built
```
reminder to HR (auto, from the 10th, in the client's language) → replies read and filed (auto)
→ email to tax advisor (AI draft, person edits and sends) → late-payslip reminder (auto)
→ payslips recognised, matched to client and month (auto)
→ two-way reconciliation by fixed rules (auto) → cost breakdown (auto)
→ payment instruction (draft, person checks 3 points and approves)
```
- **Rules, not a model, do the numbers.** No language model reads the payslips: they are converted to text on servers in Germany and checked by fixed rules. Reported changes must appear on the payslip, and payslip changes must have been reported.
- **Anything unclear** (wrong month, unknown sender, unreadable file) goes to a separate folder with the reason. The system does not guess.
- **Draft versus sent** versions of every outgoing email are stored and compared, so the team sees how often drafts were used unchanged.
- Everything runs in the client's own accounts. An NDA and a data processing agreement are signed; employees' bank details appear in no automated step.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| Tasks done by hand per client company per month | 9 | 2 | counted |
| Team time per employee per month | about 40 min | about 16–20 min | estimated |
| Client companies served | 5 at launch | more than 10 | counted |
| Time saved overall |  |  | not measured yet |

## 5. Where it got stuck
- **No interface to the payroll software.** Payslips only exist as PDFs from the tax advisor, so the whole check works on extracted text.
- **Real writing varies.** HR departments answer in their own words and formats. Prescribing exact wording to people only moved the problem; the system had to cope with how people actually write.
- **Fixing mid-run unsettled the team.** Small problems during the first live month were collected and fixed together afterwards.
- **A mailbox migration** during operation: the process was rebuilt as a copy, tested fully, then switched over in about 15 minutes.
- **Scope was limited on purpose:** the target was the roughly 70% standard cases; special cases stay with people.

## 6. What we would do differently
Collect a list of the real reply formats from HR before building, and agree from day one that fixes come in batches after each monthly run.

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
