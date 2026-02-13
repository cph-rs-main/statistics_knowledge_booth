---
date: '2026-02-09T17:00:57-07:00'
title: "Choosing Interrater Reliability Methods"
author: "Sebastian Cheong"
output:
  blogdown::html_page:
    toc: true
    toc_float: true
    theme: "simpla"
---

# Choosing Interrater Reliability (IRR) Methods 

**Interrater reliability** Best practices and statisical methdologies for IRR

## Krippendorff's Alpha (KA)

- **Use Case**: Suitable for any number of raters, ordinal, interval, ratio, or nominal data.
- **Strengths**:
  - Handles missing data.
  - Works with small sample sizes.
  - Flexible for different data types (Geijer et al., 2025)
- **Limitations**:
  - **Sensitive to marginal distributions**: When raters agree on a prevalent category (e.g., 90% of ratings are "3"), KA assumes this is due to chance and penalizes the agreement.
  - This creates the "Kappa paradox" where high observed agreement yields low reliability scores when categories are skewed.
  - Tends to perform better with smaller sample sizes (Zhao et al., 2012)

## Gwet's AC2

- **Use Case**: Alternative to KA for ordinal data with multiple raters.
- **Strengths**:
  - **Robust to skewed distributions**: Does not assume independence between raters.
  - More stable when categories are unevenly distributed (Gwet, 2008)
  - Higher interpretability when raters show consistent central tendency
- **Limitations**:
  - Suffers from the same limitations as the KA
  - May overestimate reliability in certain edge cases

## Practical Example: High Agreement Scenario

When raters distribute responses evenly across categories (no category &gt;35%), both KA and AC2 agree on high reliability.

