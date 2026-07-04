# AB Testing Conversion Analytics

A statistical inference pipeline designed to evaluate and validate A/B test experiments for marketing campaign conversion rates across user groups.

## Key Features

The pipeline processes user data through a strict statistical verification flow:

- Hypothesis Definition: Framework designed to test the Null Hypothesis ($H_0: p_A = p_B$) against the Alternative Hypothesis ($H_1: p_A \neq p_B$) at a 0.05 significance level ($\alpha$).
- Parametric Assumption Validation: Runs the Shapiro-Wilk test to evaluate normal distribution behaviors, proving the conversion datasets deviate from standard normality. It applies the Levene test to verify variance homogeneity between control and variant groups.
- Statistical Inference Testing: Runs a parametric Independent Student's t-test alongside a manual mathematical verification step to isolate means differences.
- Non-Parametric Validation: Executes a Mann-Whitney U test (Wilcoxon rank-sum) as the final mathematical criterion since the distribution properties break standard parametric requirements.
- Evaluation: Analyzes probability density functions and cumulative distributions to mathematically demonstrate that the geographical marketing variable yields no significant impact on final user conversion benchmarks.

## Quick Start
```bash
   pip install pandas numpy scipy seaborn matplotlib
```

---