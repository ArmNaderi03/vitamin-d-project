# PROJECT_CARD — Route A: NHANES 2021–2023

**Title:** Vitamin D and selected demographic and health variables in adults 18+.

**Question:** How does the descriptive distribution of serum vitamin D vary
across demographic and health characteristics in the NHANES adult population?

**Unit:** One adult participant; unique key `SEQN`.
**Population:** Adults aged 18 years and over represented by NHANES,
subject to laboratory measurement eligibility and missingness.

**Primary quantitative response:** `LBXVIDMS` (nmol/L).
**Explanatory / grouping variables:** `RIAGENDR`, `RIDAGEYR`, `BMXBMI`,
`Mean_Systolic_BP`, `Mean_Diastolic_BP`, `Cigarettes_30Day_Total`,
`PHQ9_Total`, `PHQ9_Severity`, `Weighted_PA_Weekly`, `INDFMPIR`.

**Sampling design:** `WTPH2YR`, `WTPH2YR_clean`, `SDMVSTRA`, `SDMVPSU`.

**Phase 2 pre-defined events:**
- A: `LBXVIDMS < 50` nmol/L.
- B: `RIAGENDR == 2` (female, as recorded).
- D: serum vitamin D, continuous quantitative random variable.

**Analytical sample:** adult, valid vitamin D and sex code,
positive `WTPH2YR_clean` (5,824 rows).

**Planned Phase 2 approach:** weighted and unweighted empirical probability,
conditional/joint probability, descriptive independence checks, Bayes,
binomial counting comparison, normal approximation and distribution shape,
expectation, variance and covariance. Formal hypothesis testing reserved
for later phases.

**Reproducibility:** All Phase 2 computations read the prepared output of Phase 1.
