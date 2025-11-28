# EnviroTech Dynamics – NumPy Temperature Analysis
A fast, vectorized data-analysis project built using NumPy to process 1 million+ temperature readings and detect anomalies without loops.


## 🚀 Project Summary
This project replaces slow, loop-based inspection with fast, vectorized NumPy operations. It analyzes environmental temperature data, identifies critical anomalies, and cleans faulty sensor readings using statistical techniques.

## 📁 Dataset Structure
- Temperature readings: 1,000,000 values
- Status codes (system health):
0 → Normal

1 → Warning

2 → Critical

3 → Sensor Error

## 🧠 Key Features
- Fast statistical analysis (mean, median, std, percentiles).
- Boolean masking for instant anomaly detection.
- Vectorization & broadcasting for complex operations.
- Faulty data replacement using median imputation.
- Matplotlib visualizations for insights.
- Performance checked with %timeit.

## ⚠️ Critical Findings
- 34 critical temperature spikes found.
- Values ranged 81°C–86°C, far above normal levels.
- Only 0.0034% of all readings, but high-risk. 

## 🧼 Data Cleaning Results
- 20,102 faulty records (status = 3) replaced with median (~45°C).
- Median remained unchanged (44.99°C) after cleaning.
- Dataset quality remained stable and reliable.

## 📊 Visual Outputs
- Plot of temperature distribution.
- Highlighted anomaly visualization.

## 🏁 Final Insights
- NumPy reduced analysis time from minutes to milliseconds.
- Loop-free vectorization made the system scalable. 
- Data cleaning improved reliability without changing distribution.
- The pipeline is now optimized, efficient, and ready for real deployment
