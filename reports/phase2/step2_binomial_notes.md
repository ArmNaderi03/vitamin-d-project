# Phase 2 / Step 2 — Discrete count and binomial approximation

**Empirical NHANES August 2021–August 2023 file, inherited from Phase 1**

- Participants with valid D measurement and positive phlebotomy weight: N=5,824.
- Participants below D<50 nmol/L: K=1,177.
- Raw empirical probability: p_raw=0.202095; survey-weighted probability: p_w=0.208383.
- Equal-sized simple random subsamples **without replacement**: n=30, repeated 5,000 times (seed 1405).
- Mean event count of the simulation: 6.1310; simulated variance: 4.9966.
- Binomial approximation with **raw** p: E(X)=6.0628, Var(X)=4.8376.
- Exact finite-sample hypergeometric variance: 4.8135; finite population correction factor: 0.995020.
- Maximum pointwise absolute PMF difference (hypergeometric vs raw-p binomial): 0.000460.
- Weighted p in a **hypothetical independent** Bernoulli model gives E(X)=6.2515.

## Scientific interpretation

With a fixed set of N observed people and K observed events, repeated size-n SRS **without replacement** produces a hypergeometric count exactly, not a binomial count. Since n/N=0.515% is small, the binomial model using p_raw=K/N is a close approximation here. The original stratified and clustered NHANES probability sample does **not** meet independent-identically-distributed trial assumptions by default, and this teaching simulation does not reproduce its design. Weighted p changes the marginal population-oriented rate; Binomial(n,p_w) is a separate hypothetical scenario, not an NHANES sampling variance model.

No formal hypothesis test or confidence interval is reported in Phase 2 Step 2. Individual records must not be pushed to GitHub.
