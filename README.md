# A/B Test Design with CUPED for Revenue Metric

This project demonstrates how to design and validate an A/B test for a revenue-based metric.

The focus is on **experiment design**, rather than post-experiment analysis:
metric construction, variance reduction, sample size estimation,
and statistical validation via simulations.


## Experiment Design

The experiment design includes:

- **CUPED**  
  A pre-experimental covariate is used to reduce variance.

- **Sample Size Calculation**  
  Business MDE (percentage uplift) is translated into an absolute effect
  and used to estimate required sample size.

- **Duration Estimation**
  Sample size is converted into experiment duration using historical traffic.

- **Validation**  
  AA simulations verify Type I error control,  
  AB simulations validate statistical power and compare CUPED vs raw metric


## Results

- **Variance reduction** leads to a significant decrease in required sample size  
- **CUPED improves statistical power** under the same traffic constraints  
- **Simulation confirms correctness of the experimental design**


## Tech Stack

- **Programming:** Python (Pandas, NumPy, SciPy, Matplotlib, Seaborn, Tqdm)
- **Statistical Methods:** Pearson Correlation, CUPED, Monte Carlo Simulations, T-test

&nbsp;

This project focuses on experiment design and validation before launch.
Post-experiment analysis is intentionally out of scope.
