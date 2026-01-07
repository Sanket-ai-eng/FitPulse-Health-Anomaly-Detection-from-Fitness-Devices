# Milestone 3: Anomaly Detection and Visualization

## 📌 Objective

The objective of this milestone is to:

* Detect abnormal patterns in wearable sensor data
* Apply multiple anomaly detection techniques
* Visualize anomalies clearly for interpretation

---

## Dataset

**File used:** `FitPulse_cleaned.csv`

### Important Columns

* `time_stamp` – Timestamp of recorded data
* `heart_rate` – Heart rate readings
* `sleep_tracking` – Sleep state information

The dataset is sorted chronologically before analysis.

---

## Tools & Technologies

* **Python 3**
* **Pandas** – Data handling
* **NumPy** – Numerical computations
* **Matplotlib** – Visualization
* **Scikit-learn** – KMeans clustering, data scaling
* **Prophet** – Time-series forecasting and residual analysis

---

## Methodology

### 1️⃣ Rule-Based Anomaly Detection

* Calculates mean and standard deviation
* Uses the 3-sigma rule (mean ± 3×std)
* Flags extreme values as anomalies

### 2️⃣ Clustering-Based Outlier Detection (KMeans)

* Data is standardized using `StandardScaler`
* KMeans clustering (k = 3) is applied
* Points farthest from cluster centers (top 5%) are flagged as anomalies

### 3️⃣ Prophet Residual-Based Anomaly Detection

* Prophet models expected time-series behavior
* Residuals (actual − predicted) are calculated
* Large residual deviations are marked as anomalies

### 4️⃣ Final Anomaly Decision

A data point is considered anomalous if **any one** of the above methods detects it.

---

## Visualizations

Generated plots are saved in the `visualizations/` folder:

* `heart_rate_anomalies.png` – Heart rate anomalies over time
* `sleep_anomalies.png` – Sleep pattern anomalies over time

Each plot shows:

* Line chart → entire dataset
* Scatter points → detected anomalies

---

## ▶️ How to Run

1. Install required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn prophet
```

2. Ensure the dataset path is correct:

```
../FitPulse_cleaned.csv
```

3. Open and run the notebook:

```bash
anomaly_detection.ipynb
```

## 🧠 Learning Outcomes

* Applied multiple anomaly detection strategies
* Worked with time-series wearable data
* Visualized and interpreted anomalous behavior

---

## 📝 Report Statement

> "Anomalies in heart rate and sleep patterns were detected using statistical thresholds, KMeans clustering, and Prophet residual analysis, and visualized using time-series plots."

---

## 👤 Author

**Sanket**

