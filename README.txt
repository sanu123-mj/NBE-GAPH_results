


- Synthetic population of 2000 students with heterogeneity in
  neurodiversity, SES, present bias, cognitive-load sensitivity, and
  baseline trust.
- 12 discrete timesteps.
- Five configurations:
  1. Full NBE-GAPH (all four variables active)
  2–5. Ablations (one variable set to zero at a time)
- Three independent random seeds: [42, 123, 2025]

- Mean engagement rate
- Sustained engagement (≥ 6/12 timesteps)
- Trust calibration error
- Equity gaps (Neurotypical–Neurodiverse and Higher-SES–Low-SES)

- One-way ANOVA on engagement
- Tukey HSD pairwise comparisons
- Cohen's d effect sizes (Full vs each ablation)


tables/
  summary_all_seeds.csv          – raw summary per seed × config
  summary_mean_std.csv           – mean ± SD across seeds
  per_student_seed42_Full.csv – detailed student-level data (one seed)

figures/
  engagement_boxplot.png
  equity_gaps.png
  trust_error.png
  ablation_impact.png




