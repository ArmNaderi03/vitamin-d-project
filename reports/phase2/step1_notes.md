# Phase 2 — Step 1 (empirical probability)

Analysis source: Phase 1 integrated adult dataset.
6,337 adults; 5,824 eligible with valid vitamin D and positive cleaned weight.

A = serum vitamin D < 50 nmol/L. B = recorded female sex.
- Weighted P(A) = 0.20838 (20.84%)
- Weighted P(B) = 0.51225 (51.23%)
- Weighted P(A ∩ B) = 0.09798
- Weighted P(A | B) = 0.19126 (19.13%)
- Weighted P(A | not B) = 0.22636 (22.64%)
- Weighted P(B | A) = 0.47017 (47.02%)
- Weighted P(A∩B) - P(A)P(B) = -0.00877.

The male minus female contrast is
3.51 percentage points.

Interpret these as descriptive weighted proportions, not formal design-based
inference. No independence test, confidence interval, or causal conclusion
is provided. See the reproducible notebook and CSV tables.
