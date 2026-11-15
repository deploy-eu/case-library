---
title: "AI back office for a small pearl jewellery brand"
authors: ["DATONG AI"]
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
consent: "client agreed to publication of the anonymised case (as on the public page linked below)"
review: "pending: awaiting review by a second maintainer"
---

# AI back office for a small pearl jewellery brand

> **Disclosure:** written by DATONG AI, the company of a Deploy@EU management team member. The community does not endorse any company. Based on the public case page linked below, published with the client's consent. **Review by a second maintainer: pending.**

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

## 7. Links
- Public case page: https://datongai.de/en/projects/jewellery-back-office/

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
