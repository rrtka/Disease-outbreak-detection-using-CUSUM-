Overview


Detects early disease outbreak signals using weekly flu (ILI) data

Uses CUSUM (Cumulative Sum Control Chart) for anomaly detection


Tech Stack


Python

Pandas

Matplotlib


Approach


Calculate mean (μ) and standard deviation (σ)

Apply CUSUM algorithm:

CUSUM[i] = max(0, CUSUM[i-1] + (x[i] - μ - k))

Identify outbreak when CUSUM exceeds threshold


Results


Visualized flu trends over time

Highlighted potential outbreak points

Computed total outbreak signals


How to Run


Install dependencies

pip install pandas matplotlib

Run the notebook

jupyter notebook
Summary
Provides a simple method for early outbreak detection
Useful for public health monitoring and analysis
