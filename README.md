# Reducing Stockouts and Order Hold Losses through Sales Analysis for a Fashion Jewellery Retailer

**BDM Capstone Project — IIT Madras BS Degree Programme**
Author: Ritoma Nandi (23F3001843)
Duration: March – May 2026 | Business: Zane Lifestyle (brand: **Vanki**)

---

## Overview

This project analyzes 3 months of sales and order data from **Vanki**, a small anti-tarnish fashion jewellery retailer operating through a physical shop and informal WhatsApp/Facebook order-taking, with no prior digital sales system or inventory tracking.

The analysis addresses two business problems:
1. **Sales & Inventory Performance** — which products/categories drive revenue, how demand varies, and what role pricing plays.
2. **Unconfirmed Order Holds ("Ghosting")** — quantifying revenue lost when customers put items on hold via WhatsApp and never follow through, and designing a data-backed hold policy to fix it.

---

## Key Findings

**Sales & Inventory**
- Bracelets and Earrings together account for **78% of total revenue** (₹21,850 + ₹20,343)
- Revenue grew **137%** from March to May (₹11,106 → ₹26,282)
- No strong 80/20 (Pareto) pattern — **37 of 75 SKUs** were needed to reach 70% of revenue
- Rings are the most volatile category (CV 74.2%), Earrings the most stable (CV 33.4%)
- Price explains only **7.5%** of demand variation (R² = 0.075) — product design/appeal matters more than pricing

**Order Holds**
- Of 36 valid hold incidents, **7 were ghosted (19.4% ghost rate)**
- Ghosted holds cost **₹3,518.44 (~6.5% of revenue)** — ₹2,320 in lost sales + ₹1,198.44 in bargaining-related margin loss
- Ghosted orders sit on hold **~20x longer** than converted ones (median 85.9 hrs vs 4.6 hrs)
- **72.2%** of all holds involved price bargaining, averaging a 9% discount request
- A proposed **24-hour auto-release policy** would have recovered all 7 ghosted incidents, vs. only 5 of 7 under a 48-hour rule

---

## Repository Contents

| File | Description |
|---|---|
| `23f3001843_Capstone_Project_Proposal.docx` | Initial project proposal |
| `23f3001843_Capstone_Project_Mid_Term.docx` | Mid-term submission |
| `23f3001843_Capstone_Project_Final_Submission.docx` | Final report with full methodology, analysis, and results |
| `23f3001843_Capstone_Project_PPT.pptx` | Viva voce presentation deck |
| `Jewelry_Orders.xlsx` | Cleaned dataset (Invoices, Daily Sales, Product Summary, Hold Tracker) |

---

## Methodology

- **Descriptive statistics** (mean, median, SD, CV) on order values and category-level demand
- **ABC / Pareto classification** of 75 SKUs by cumulative revenue contribution
- **Sales velocity analysis** (units sold per week, by product and category)
- **Pearson correlation** between unit price and quantity sold
- **Hold/ghosting analysis** — ghost rate, stock-hours blocked, bargaining impact, and a 24h vs. 48h auto-release policy simulation

Data was manually compiled from the owner's WhatsApp/Facebook order logs and physical sales register, then cleaned (standardized dates, unified category naming, currency parsing, duplicate/incomplete record handling) before analysis. All analysis was performed in Microsoft Excel.

---

## Recommendations

1. Use a combined **ABC + velocity + CV stocking priority matrix** rather than revenue-share alone
2. Set **category-specific reorder cycles** — monthly for Earrings/Bracelets, weekly review for Rings
3. Introduce a **24-hour hold policy** for WhatsApp/Facebook orders, with a 12-hour reminder for high-ghost-rate categories
4. Cap discretionary discounts at **5–10%** to limit bargaining-driven margin loss
5. Re-run this analysis **monthly** to track KPIs as a live monitoring practice

---

## Limitations

This analysis is based on 3 months of data (March–May 2026) from a single small retailer. Findings on seasonality, long-term demand patterns, and category trends should be treated as preliminary and revisited with more data over time.

---

## Author

Ritoma Nandi

---

*This project was completed as part of the Business Data Management (BDM) Capstone Project under the IIT Madras BS Degree Programme.*
