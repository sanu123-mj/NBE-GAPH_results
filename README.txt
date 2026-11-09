
NBE-GAPH Illustrative Validation Results
========================================

This folder contains the complete output of a controlled synthetic
simulation that illustrates the logical behaviour of the four design
variables of the NBE-GAPH governance architecture.

IMPORTANT DISCLAIMER
--------------------
These results are NOT empirical findings from real schools, students,
or deployed platforms. They are a transparent numerical illustration
of the design logic under controlled assumptions. The paper remains
architectural; real-world pilot validation is future work.

What was simulated
------------------
- Synthetic population of 2000 students with heterogeneity in
  neurodiversity, SES, present bias, cognitive-load sensitivity, and
  baseline trust.
- 12 discrete timesteps.
- Five configurations:
  1. Full NBE-GAPH (all four variables active)
  2–5. Ablations (one variable set to zero at a time)
- Three independent random seeds: [42, 123, 2025]

Metrics
-------
- Mean engagement rate
- Sustained engagement (≥ 6/12 timesteps)
- Trust calibration error
- Equity gaps (Neurotypical–Neurodiverse and Higher-SES–Low-SES)

Statistical tests performed
---------------------------
- One-way ANOVA on engagement
- Tukey HSD pairwise comparisons
- Cohen's d effect sizes (Full vs each ablation)

Files
-----
tables/
  summary_all_seeds.csv          – raw summary per seed × config
  summary_mean_std.csv           – mean ± SD across seeds
  per_student_seed42_Full.csv – detailed student-level data (one seed)

figures/
  engagement_boxplot.png
  equity_gaps.png
  trust_error.png
  ablation_impact.png

logs/
  statistics.txt                 – full statistical report

How to cite / describe in the paper
-----------------------------------
"To illustrate the logical contribution of each design variable we
conducted a controlled synthetic simulation (N = 2000 agents,
3 random seeds). The full NBE-GAPH configuration was compared with
four ablations. Results (see Supplementary Material) show that
removing any single variable produces statistically significant
degradations in engagement and/or equity under the model assumptions.
This exercise is purely illustrative and does not constitute empirical
validation."

Generated with the NBE-GAPH Illustrative Validation Suite.
