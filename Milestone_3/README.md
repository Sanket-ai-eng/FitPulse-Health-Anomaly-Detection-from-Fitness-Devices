# Module 3: Anomaly Detection and Visualization

## Project Overview

This project implements **Module 3: Anomaly Detection and Visualization** using a real-world wearable/Fitbit activity dataset (`dailyActivity_merged.csv`). The goal is to identify unusual activity patterns (anomalies) in time-series data and visualize them clearly.

The solution combines:

* **Rule-based anomaly detection (thresholds)**
* **Clustering-based outlier detection (KMeans)**
* **Model-based anomaly detection (Prophet residuals)**

All detected anomalies are visualized on time-series plots.

---

##  Dataset

**File:** `dailyActivity_merged.csv`

**Key Columns Used:**

* `ActivityDate` – Date of activity
* `TotalSteps` – Total number of steps per day

The dataset is first sorted chronologically to ensure correct time-series analysis.

---

## Technologies & Libraries

* Python 3
* Pandas – Data manipulation
* NumPy – Numerical computations
* Matplotlib – Data visualization
* Scikit-learn – KMeans clustering, scaling
* Prophet – Time-series forecasting and residual analysis

---

## Methodology

### 1️⃣ Rule-Based Anomaly Detection (Thresholds)

* Computes **mean** and **standard deviation** of daily steps
* Uses the **3-sigma rule (mean ± 3×std)**
* Values outside this range are marked as anomalies

### 2️⃣ Clustering-Based Outlier Detection (KMeans)

* Step counts are **standardized** using `StandardScaler`
* KMeans clustering is applied (k = 3)
* Distance of each point from its cluster center is calculated
* Top **5% farthest points** are marked as anomalies

### 3️⃣ Prophet Residual-Based Anomaly Detection

* Prophet models the expected step trend over time
* **Residuals = Actual − Predicted values**
* Large residuals (beyond 3× standard deviation) are flagged as anomalies

### 4️⃣ Final Anomaly Decision

A data point is considered an anomaly if **any one** of the above methods flags it.

---

##  Visualization

* **Line plot** represents the **entire dataset** (all datapoints)
* **Scatter points** highlight anomalous observations
* An additional **time-window plot** zooms into a specific date range for detailed analysis

---

##  Key Learning Outcomes

* Understanding different anomaly detection approaches
* Applying clustering and forecasting models on time-series data
* Visualizing anomalies for interpretability

---

## 👤 Author

**Sanket**
