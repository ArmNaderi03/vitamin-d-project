# Data provenance and reconstruction

Official source: CDC/NCHS, NHANES August 2021–August 2023
https://wwwn.cdc.gov/nchs/nhanes/continuousnhanes/default.aspx?Cycle=2021-2023

Raw source files used in Phase 1:
`DEMO_L`, `VID_L`, `BMX_L`, `BPXO_L`, `SMQ_L`, `DPQ_L`, `PAQ_L`.
The participant-level merge uses `SEQN`. Derived variables include
BMI, mean blood pressures, estimated 30-day cigarettes, PHQ-9,
weighted physical activity and `WTPH2YR_clean`.

Local dataset: `data/final_data.csv`, generated at the end of Phase 1.
It has 6,337 rows and 20 columns; 5,824 rows have valid serum vitamin D
and a positive cleaned phlebotomy weight. The file is **not committed**.

**Actual download date:** Enter the real date from Phase 1 records or
download logs. No date is invented in this template.

Reproduce by running `notebooks/phase1.ipynb` in order and exporting
`final_data.to_csv("data/final_data.csv", index=False)` from repository root.
Then run `notebooks/phase2_step1.ipynb`.

Large/source datasets must not be included in GitHub or CW submissions,
except if the course team expressly instructs otherwise.
