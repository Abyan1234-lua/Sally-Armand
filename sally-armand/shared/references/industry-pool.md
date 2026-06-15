# Industry Pool — Random Mode

Sally draws from this pool when generating random personas with no brief.

---

## Indonesia-Biased Pool (60% weight)

| Code | Industry | Sub-sector |
|------|----------|-----------|
| ID-01 | E-commerce / Retail | Tokopedia/Shopee seller, brand owner, logistics |
| ID-02 | Education | Private school teacher, tutoring center owner, edtech user |
| ID-03 | F&B | Small restaurant owner, cloud kitchen, food distributor |
| ID-04 | Healthcare | Clinic staff, pharmacist, health insurance agent |
| ID-05 | Finance | Bank officer, fintech user, insurance agent, independent trader |
| ID-06 | Logistics & Supply Chain | Warehouse manager, courier ops, distribution |
| ID-07 | Creative / Agency | Freelance designer, content creator, social media manager |
| ID-08 | Property | Agent, developer marketing, property investor |
| ID-09 | Manufacturing | SME factory owner, procurement manager |
| ID-10 | Government / NGO | Civil servant, program officer, foundation manager |
| ID-11 | Tech Startup | Early employee, product manager, founder |
| ID-12 | Retail (Offline) | Traditional market trader, minimarket franchise owner |

---

## Global Pool (40% weight)

| Code | Industry | Geography Bias |
|------|----------|---------------|
| GL-01 | SaaS / Software | USA, UK, Australia |
| GL-02 | Healthcare | USA, Europe |
| GL-03 | Marketing / Advertising | Global metro (NY, London, Singapore) |
| GL-04 | Education (Higher Ed) | USA, UK, India |
| GL-05 | Finance / Fintech | Singapore, London, NY |
| GL-06 | Creative / Design | Global remote |
| GL-07 | Retail / Fashion | Europe, USA |
| GL-08 | Real Estate | Australia, USA, UAE |
| GL-09 | Manufacturing | China, Germany, Japan |
| GL-10 | Non-profit / Social Impact | East Africa, Southeast Asia, USA |

---

## Randomization Rules

1. If user says "Indonesia" or geography implies local → draw from ID pool
2. If user says "global" or doesn't specify → 60% ID, 40% GL
3. If user says "surprise me" → roll random from full pool
4. Never put two personas from the same industry code in the same batch
