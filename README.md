# HR Attrition Dashboard

An interactive HR analytics dashboard built to visualize employee attrition patterns across age, job role, department, travel frequency, gender, and marital status using IBM's HR Analytics dataset.

---

## Overview

This project explores workforce attrition by converting raw pivot table counts into meaningful attrition rates — calculated as:

```
Attrition Rate (%) = Yes (leavers) ÷ (Yes + No) × 100
```

This ensures every metric is comparable across groups, regardless of group size.

---

## Dataset

**Source:** IBM HR Analytics Employee Attrition & Performance dataset  
**Records:** 1,470 employees  
**Attrition:** 237 employees left (16.1% overall rate)

The pivot data used covers:
- Age band breakdown (Yes / No / Grand Total)
- Job role breakdown (No / Yes / Grand Total)
- Gender × Marital Status (Yes counts per cell)
- Department × Business Travel (No / Yes / Grand Total)
- Education level (headcount only)

---

## Dashboard Sections

| Section | Metric shown |
|---|---|
| Age band | Attrition rate per age group |
| Job role | Attrition rate per role |
| Gender | Attrition rate — Male vs Female |
| Marital status | Attrition rate — Single / Married / Divorced |
| Gender × Marital | Share of leavers within each gender |
| Department | Attrition rate — Sales / HR / R&D |
| Travel frequency | Attrition rate per dept × travel band |

---

## Key Findings

- **Under-25 employees** have the highest attrition rate at **39.2%**
- **Sales Representatives** are the highest-risk role at **39.8%**
- **Sales department** leads by department at **20.6%**
- **Frequent travelers in HR** have a **36.4%** attrition rate
- **Single employees** leave at **25.5%** vs 12.5% for married and 10.1% for divorced
- **Male employees** leave slightly more (17.0%) than female (14.8%)

---

## Data Limitations

- **Education:** The dataset only provides headcount per education level — no Yes/No split — so attrition rate by education cannot be calculated.
- **Gender × Marital rate:** The pivot table provides Yes counts per cell but not No counts, making true cell-level rates impossible. The dashboard shows share of leavers within gender instead.

---




## How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/your-username/hr-attrition-dashboard.git
   ```
2. Open `dashboard/index.html` in any browser — no build step or dependencies required.

---

## License

MIT
