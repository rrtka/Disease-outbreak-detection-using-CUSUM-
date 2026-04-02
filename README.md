Disease Outbreak Detection (CUSUM)

Overview

This project detects disease outbreaks using CUSUM control charts on weekly flu (ILI) data. It identifies abnormal increases in cases for early warning.

Features

Time-series analysis of flu data
CUSUM-based anomaly detection
Visualization of outbreak signals

Tech Stack

Python
Pandas
Matplotlib

Method

Compute mean (μ) and standard deviation (σ)

Apply CUSUM

CUSUM[i] = max(0, CUSUM[i-1] + (x[i] - μ - k))
Trigger outbreak if CUSUM > threshold

Output

Flu trend graph
Highlighted outbreak points
Total detected signals

Run
pip install pandas matplotlib
jupyter notebook

Summary
CUSUM helps detect early outbreak patterns from flu data, useful for public health monitoring.
