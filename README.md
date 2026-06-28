# A/B Testing Analysis — Product Page Experiment

> Statistical hypothesis testing to determine whether a redesigned e-commerce product page significantly improves conversion rate, revenue, and engagement.

---

## Conversion Rate: Control vs Variant

![Conversion Rate](chart1_conversion_rate.png)

Variant B converts at **4.94% vs Control's 3.50%** — a **+41.1% relative lift**, confirmed statistically significant.

---

## Statistical Significance (Chi-Square Test)

![Chi-Square Test](chart2_chi_square.png)

χ² = 12.47 | **p-value = 0.0004** | well below α = 0.05 threshold. The result is not due to chance.

---

## Revenue Projection

![Revenue Projection](chart3_revenue_projection.png)

Shipping Variant B projects **+$970,144 additional revenue per year** at 50,000 monthly visitors.

---

## Performance Across All Devices

![Device Breakdown](chart4_device_breakdown.png)

Variant B outperforms Control on Desktop (5.0% vs 3.4%), Mobile (4.9% vs 3.8%), and Tablet (2.3% vs 1.8%).

---

## Statistical Test Results

| Metric | Control (A) | Variant (B) | Lift | Test | p-value | Significant? |
|--------|-------------|-------------|------|------|---------|--------------|
| Conversion Rate | 3.50% | 4.94% | +41.1% | Chi-Square | 0.0004 | ✅ Yes |
| Avg Order Value | $75.14 | $85.97 | +14.4% | T-Test | 0.0422 | ✅ Yes |
| Time on Page | 45s | 61s | +35.6% | Mann-Whitney U | <0.0001 | ✅ Yes |

---

## ✅ Decision: SHIP VARIANT B

All three primary metrics show statistically significant improvement. The new design (image carousel + social proof + urgency elements) is conclusively better. Projected annual revenue uplift: **~$970K**.

---

## Files

| File | Description |
|------|-------------|
| `AB_Testing_Analysis.ipynb` | Full analysis notebook with all charts and statistical tests |
| `AB_Testing_Dashboard.html` | Interactive standalone dashboard (open in browser) |

## Tech Stack

**Python** (pandas, numpy, scipy.stats) · **Plotly** · **Matplotlib** · **Jupyter Notebook**

Statistical tests used: Chi-Square, Independent T-Test, Mann-Whitney U, Wilson Confidence Intervals

## How to Run

```bash
git clone https://github.com/darshitjayswal1/ab-testing-analysis
jupyter notebook AB_Testing_Analysis.ipynb
```

---
*Scenario: Fashion e-commerce brand | 10,000 users | 4-week experiment*
