---
title: "A key account manager's AI setup with a second-agent check"
authors: ["Abuzhabilaohan"]
date: "not disclosed"
status: "live"
country: "not disclosed"
industry: "manufacturing / B2B sales"
company_size: "not disclosed"
existing_systems: ["mailbox", "chat", "calendar", "spreadsheets", "CRM"]
ai_and_tools: ["AI assistant with scheduled tasks", "checking agents", "scripts"]
walls: ["reliability", "data-quality"]
effort: "not disclosed"
anonymised: "yes"
consent: "client agreed to publication of the anonymised case"
title_zh: "大客户经理的 AI 搭档：每份草稿都有第二个 agent 把关"
summary_zh: "一位大客户经理用 AI 助手管理客户档案、邮件草稿、报告和 CRM 准备。每份草稿在他看到之前都先经过第二个 agent 检查；发送、保存和定价都由他自己做。"
industry_zh: "制造业 / B2B 销售"
title_de: "KI-Setup eines Key Account Managers mit Zweitprüfung durch einen zweiten Agenten"
summary_de: "Ein Key Account Manager führt Kundenakten, E-Mail-Entwürfe, Berichte und CRM-Vorbereitung über einen KI-Assistenten. Ein zweiter Agent prüft jeden Entwurf, bevor er ihn sieht; senden, speichern und Preise setzen macht er selbst."
industry_de: "Industrie / B2B-Vertrieb"
title_fr: "Le dispositif IA d'un key account manager, avec contrôle par un second agent"
summary_fr: "Un key account manager gère fiches clients, brouillons d'e-mails, rapports et préparation du CRM avec un assistant IA. Un second agent vérifie chaque brouillon avant qu'il ne le voie ; envoyer, enregistrer et fixer les prix restent à lui."
industry_fr: "industrie / vente B2B"
title_it: "Il setup IA di un key account manager, con il controllo di un secondo agente"
summary_it: "Un key account manager gestisce schede clienti, bozze di e-mail, report e preparazione del CRM con un assistente IA. Un secondo agente controlla ogni bozza prima che lui la veda; inviare, salvare e fissare i prezzi resta a lui."
industry_it: "manifattura / vendite B2B"
title_es: "El sistema de IA de un key account manager, con revisión de un segundo agente"
summary_es: "Un key account manager lleva fichas de clientes, borradores de correo, informes y preparación del CRM con un asistente de IA. Un segundo agente revisa cada borrador antes de que él lo vea; enviar, guardar y fijar precios lo hace él."
industry_es: "industria / ventas B2B"
review: "pending: awaiting review by a second maintainer"
---

# A key account manager's AI setup with a second-agent check

> **Disclosure:** written by Abuzhabilaohan, a Deploy@EU management team member, about a project delivered by DATONG AI, the team he works with. The community does not endorse any company. Published with the client's consent. **Review by a second maintainer: pending.**

> **Summary:** One key account manager runs customer files, email drafts, reports and CRM preparation through an AI assistant. A second agent checks every draft before he sees it; he sends, saves and sets prices himself.

## 1. The business problem
Contacts, history, commitments and next steps for each business customer were spread over emails and the CRM, so follow-ups slipped. Emails in two languages could each carry a wrong fact, a wrong tone or an unwarranted promise. On top came a weekly report, a stock and price list for one customer, and CRM upkeep.

## 2. What was already there
Mailbox, chat, calendar, spreadsheets and a CRM. Saving to the CRM stays a manual click.

## 3. What was built
```
06:12 follow-up drafts for unanswered first contacts (max 8 a day) → 06:52 morning report to himself
→ during the day: AI sorts new mail and chat into "act / info / ignore"
→ draft reply in the original thread, with translation → second agent checks facts against sources and tone
→ he edits and says "send" → CRM fields prepared by AI, he clicks save, AI reads back what was saved
→ every two days: stock and price list rebuilt by written rules and read back
```
- **13 tasks:** 4 run on a schedule, 8 are prepared by the AI, 1 stays entirely with the person.
- **Only two things run fully automatically:** the morning report (to himself) and the price list (prices by fixed rules).
- Customer files have version history and are backed up before every change.
- A dashboard brings together tasks, commitments with deadlines, meetings and new messages.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| Problems caught by the second check before sending, about three weeks |  | about 95 | counted from the change log, ±5 |
| Of these: facts or sources / tone / commitments not in the source |  | about 60% / 30% / 10% | estimated |
| Time saved |  |  | not measured |

## 5. Where it got stuck
- **Rules in the prompt did not hold.** Each correction was logged and added to the assistant's rules. Three kinds of error stopped; others came back despite a rule until they were turned into a fixed handbook.
- **Mechanical checks moved out of the model.** Whether a commitment exists, a source is cited or an email was really sent is now checked by a script.
- **A near miss:** a customer deadline was overwritten with a "check next time" note and almost passed. Commitments got their own column with a mandatory deadline the same day.
- The weekly report brief needed seven versions.

## 6. What we would do differently
Put everything that can be checked mechanically into scripts from the start, and give commitments a mandatory deadline before the first near miss.

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
