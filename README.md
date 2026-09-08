# Cookie Cats A/B Test Analysis

## TL;DR
Analyzed a mobile game A/B test (90k+ users) comparing two gate placements 
(level 30 vs level 40). Found no significant difference in Day-1 retention, 
but a statistically significant drop in Day-7 retention for the gate_40 
group (p = 0.0016). Recommended against moving the gate.

## Tools
Python, Pandas, SciPy, Statsmodels, Matplotlib

## Method
Chi-square test of independence and two-proportion z-test on retention_1 
and retention_7 across two experiment groups.

## Key Finding
Day-7 retention: gate_30 = 19.0% vs gate_40 = 18.2% (statistically significant, 
p = 0.0016). Day-1 retention showed no significant difference (p = 0.0755).

## Files
- `cookie_cats_ab_test.ipynb` — full analysis
- `cookie_cats.csv` — dataset
