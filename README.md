# Data Drift Metrics Comparison

## Introduction
This code aims to compare different metrics for measuring data drift in continuous distributions. The experimentation involves simulating two types of drift in a continuous distribution at different sample sizes. The metrics considered for comparison include statistical tests such as the Two-sample mean z-test, Kolmogorov-Smirnov test, K-Sample Anderson-Darling test, and other measures like KL Divergence, JS Distance, and Population Stability Index (PSI).

## Code Overview

### Dependencies
- `numpy`: For numerical operations and random number generation.
- `pandas`: For data manipulation and analysis.
- `matplotlib.pyplot`: For plotting visualizations.
- `scipy.stats`: For statistical functions.
- `seaborn`: For statistical data visualization.
- `sklearn.metrics`: For pairwise metrics.
- `matplotlib.animation.FuncAnimation`: For creating animations.

### Functions
1. **generate_distribution**: Generates a numeric distribution with multiple components.
2. **introduce_drift**: Simulates dynamic shifts in means of normal distributions to introduce drift.
3. **probabilty_distribtion_from_samples**: Generates probability distributions from given samples.
4. **calculate_psi**: Calculates the Population Stability Index (PSI) for a variable.
5. **compute_metrics**: Computes various metrics for comparing two distributions.

### Experimentation
The code performs the following steps:
1. Generates a reference distribution.
2. Introduces drift into the reference distribution to create variant distributions with small and drastic drift magnitudes.
3. Computes various metrics for comparing the reference distribution with variant distributions.
4. Stores metric values in a DataFrame.
5. Groups, averages, and sorts metric values.
6. Saves metric values to a CSV file for further analysis.

