---
title: "AI back office for a small pearl jewellery brand"
authors: ["Abuzhabilaohan"]
date: "not disclosed"
status: "live"
country: "not disclosed"
industry: "jewellery / direct sales via social media"
company_size: "1–9 employees"
existing_systems: ["chat apps", "screenshots", "several spreadsheets (one shared with a partner)", "online shop"]
ai_and_tools: ["AI assistant", "spreadsheets"]
walls: ["data-quality", "change-management"]
effort: "not disclosed"
anonymised: "yes"
consent: "client agreed to publication of the anonymised case"
title_zh: "小珍珠品牌的 AI 后台"
summary_zh: "老板在直播和聊天里卖货。现在每卖一单她转发一张截图，助手就记下订单、付款、发货和库存；金额不清楚时会先问她。"
industry_zh: "珠宝 / 社交媒体直销"
title_de: "KI-Backoffice für eine kleine Perlenschmuckmarke"
summary_de: "Die Inhaberin verkauft in Livestreams und Chats. Nach jedem Verkauf leitet sie einen Screenshot weiter; ein Assistent erfasst Bestellung, Zahlung, Versand und Bestand und fragt nach, wenn ein Betrag unklar ist."
industry_de: "Schmuck / Direktvertrieb über Social Media"
title_fr: "Back-office IA pour une petite marque de bijoux en perles"
summary_fr: "La fondatrice vend en live et par messagerie. Après chaque vente, elle transfère une capture d'écran ; un assistant enregistre commande, paiement, expédition et stock, et pose la question dès qu'un montant est flou."
industry_fr: "bijoux / vente directe sur les réseaux sociaux"
title_it: "Back office con IA per un piccolo marchio di gioielli di perle"
summary_it: "La titolare vende in live e in chat. Dopo ogni vendita inoltra uno screenshot; un assistente registra ordine, pagamento, spedizione e magazzino, e chiede quando un importo non è chiaro."
industry_it: "gioielli / vendita diretta sui social"
title_es: "Back office con IA para una pequeña marca de joyas de perlas"
summary_es: "La dueña vende en directos y chats. Tras cada venta reenvía una captura; un asistente registra pedido, pago, envío y stock, y pregunta cuando un importe no está claro."
industry_es: "joyería / venta directa en redes sociales"
review: "pending: awaiting review by a second maintainer"
---

# AI back office for a small pearl jewellery brand

> **Disclosure:** written by Abuzhabilaohan, a Deploy@EU management team member, about a project delivered by DATONG AI, the team he works with. The community does not endorse any company. Published with the client's consent. **Review by a second maintainer: pending.**

> **Summary:** The owner sells in live streams and chats. She now forwards a screenshot after each sale; an assistant records order, payment, shipping and stock, and asks whenever an amount is unclear.

## 1. The business problem
Every sale depended on the owner: typing the order from the chat, finding the payment, passing on the address, updating stock, informing the customer. Information was spread over chats, screenshots and several spreadsheets, and she often checked the same thing twice.

## 2. What was already there
Chats, screenshots, several spreadsheets (one shared with a business partner) and an online shop. The owner did not want to learn a new program or fill in forms.

## 3. What was built
```
sale → owner forwards chat screenshot → AI creates customer, order, items; prices by her rules; deducts stock
→ payment arrives → AI matches it; if unclear it asks and enters nothing
→ AI drafts the customer message from her templates → she reads and sends it herself
→ every morning 07:30: list of what ships today, what is open, what is nearly sold out; nightly backup
```
- **Money:** the assistant never guesses. Unclear amounts are queried.
- **Item recognition:** each item has one number; the owner's, supplier's and customers' names are attached as aliases. New names are matched to similar entries and confirmed once.
- **Add-ons:** highlight clips from live streams (AI finds 30–60 second passages, a person reviews and publishes), a monthly analysis of public posts in the industry, and shop images set to one uniform background.
- Rules and prices change only on her instruction, and every change is logged. The sheet shared with the partner syncs only after she confirms.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| Steps the owner does by hand, whole process | 33 | 16 | estimated (owner's own count) |
| Errors in amounts, final test round |  | 0 | measured |
| Background colour difference, first 10 shop images | visibly different | at most 1 on a 0–255 scale | measured |

## 5. Where it got stuck
- **Same item, three names.** The owner, the supplier and customers each named the same pearl differently, so orders could not be matched to stock until every item got one number with aliases.
- **A form would not have been used.** The first idea, rebuilding the spreadsheets digitally, was dropped; the input had to stay screenshots and voice messages.
- **Three test rounds** with real screenshots and special cases were needed before amounts were error-free.
- **Background brightness was a judgement call.** Near-white backgrounds, common for jewellery, made white pearls lose their outline; a slightly darker grey was chosen.

## 6. What we would do differently
Start from the result the owner needs, not from her existing spreadsheets. That decision came after the first design, and it would have saved a round.

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
