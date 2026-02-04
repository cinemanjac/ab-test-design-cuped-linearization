# A/B Test Design for Revenue Metrics with Linearization and CUPED

This project demonstrates how to design and validate an A/B experiment
for a ratio-based business metric (revenue per user).

The focus is on **experiment design**, rather than post-experiment analysis:
metric construction, variance reduction, sample size estimation,
and statistical validation via simulations.


## Experiment Design

The experiment design includes:

- **Metric Linearization**  
  The revenue-based ratio metric is transformed into a linear metric
  to enable valid statistical testing.

- **CUPED**  
  A pre-experimental covariate is used to reduce variance.
  The optimal pre-period window is selected based on correlation.

- **Sample Size Calculation**  
  Business MDE (percentage uplift) is translated into
  a statistical MDE for the linearized metric.

- **Validation**  
  AA simulations verify Type I error control,  
  AB simulations confirm statistical power,  


## Results

- **Sample Size Reduction:**  
  Applying CUPED reduced the required sample size by approximately **2.2x**.

- **Experiment Efficiency:**  
  The expected experiment duration was reduced by **~10 weeks**


## Tech Stack

- **Programming:** Python (Pandas, NumPy, SciPy, Matplotlib, Seaborn, Tqdm)
- **Statistical Methods:**  Metric Linearization, CUPED, Monte Carlo Simulations, Correlation Analysis

&nbsp;

This project focuses on experiment design and validation before launch.
Post-experiment analysis is intentionally out of scope.
