---
title: "Price and availability from 15 online stores in one table"
authors: ["Abuzhabilaohan"]
date: "not disclosed"
status: "live"
country: "not disclosed"
industry: "retail / e-commerce"
company_size: "not disclosed"
existing_systems: ["product lists", "public store pages"]
ai_and_tools: ["product matching by name, barcode and image", "CSV export"]
walls: ["data-quality"]
effort: "not disclosed"
anonymised: "yes"
consent: "client agreed to publication of the anonymised case"
title_zh: "15 家网店的价格和库存，放进一张表"
summary_zh: "上传一份商品清单，系统在 15 家网店里查找。可能匹配的商品、价格和是否有货汇总到一张表里；团队确认款式确实一致后再导出。"
industry_zh: "零售 / 电商"
title_de: "Preise und Verfügbarkeit aus 15 Onlineshops in einer Tabelle"
summary_de: "Eine hochgeladene Produktliste wird in 15 Onlineshops gesucht. Mögliche Treffer, Preise und Verfügbarkeit landen in einer Tabelle; das Team prüft, ob die Varianten wirklich passen, und exportiert dann."
industry_de: "Einzelhandel / E-Commerce"
title_fr: "Prix et disponibilité de 15 boutiques en ligne dans un seul tableau"
summary_fr: "Une liste de produits est recherchée dans 15 boutiques en ligne. Correspondances possibles, prix et disponibilité arrivent dans un tableau ; l'équipe vérifie que les variantes concordent avant d'exporter."
industry_fr: "commerce / e-commerce"
title_it: "Prezzi e disponibilità da 15 negozi online in un'unica tabella"
summary_it: "Un elenco di prodotti viene cercato in 15 negozi online. Possibili corrispondenze, prezzi e disponibilità finiscono in una tabella; il team verifica che le varianti coincidano prima di esportare."
industry_it: "retail / e-commerce"
title_es: "Precios y disponibilidad de 15 tiendas online en una sola tabla"
summary_es: "Una lista de productos se busca en 15 tiendas online. Posibles coincidencias, precios y disponibilidad llegan a una tabla; el equipo comprueba que las variantes coinciden antes de exportar."
industry_es: "comercio / comercio electrónico"
review: "pending: awaiting review by a second maintainer"
---

# Price and availability from 15 online stores in one table

> **Disclosure:** written by Abuzhabilaohan, a Deploy@EU management team member, about a project delivered by DATONG AI, the team he works with. The community does not endorse any company. Published with the client's consent. **Review by a second maintainer: pending.**

> **Summary:** An uploaded product list is searched across 15 online stores. Possible matches, prices and availability land in one table; the team confirms that variants really match before exporting.

## 1. The business problem
Every store names products differently and shows variants differently. Searching by hand, copying prices and moving them into a spreadsheet took time, and it was easy to compare a different variant of the same product.

## 2. What was already there
Product lists in spreadsheets and the publicly visible pages of the stores.

## 3. What was built
```
person uploads a list, enters a product or pastes links
→ each store searched; possible matches by name, barcode and image (auto)
→ price, currency and availability per store in one table (auto)
→ person checks that variants match, exports CSV
```
- Store and variant stay visible in every row so the team can check them.
- Whether two listings are the same product, and all assortment and price decisions, stay with people.

## 4. Results
| What | Before | After | Measured or estimated? |
|---|---|---|---|
| Research for one product | about 1 hour | about 2 minutes | reported by the project team; number of products measured not recorded |

## 5. Where it got stuck
- **Variants.** Different sizes, colours or models of one product ended up in the same row unless the variant was checked before comparing prices.
- **Inconsistent names and links** across stores made matching by name alone unreliable; barcode and image had to be added.
- **Trust in the table** came only when source and result sat side by side in the same row.

## 6. What we would do differently
Record how many products were measured, so the time figure has a sample behind it.

---
<sub>By submitting, the authors confirm that the case contains no personal data, no confidential client information, and that publishing it was agreed with whoever needed to agree. Licensed under CC BY 4.0.</sub>
