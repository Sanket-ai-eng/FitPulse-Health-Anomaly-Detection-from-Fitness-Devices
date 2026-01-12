# Health Anomaly Detection Dashboard – Report Summary

## 1. Objective

The primary objective of this project is to design and implement an **interactive health anomaly detection dashboard** that enables users to upload fitness data and automatically identify abnormal patterns in key health metrics such as **heart rate, sleep duration, and step count**. The dashboard aims to provide actionable insights through visual analytics and downloadable reports, supporting early detection of unusual health behaviors.

---

## 2. Dashboard Workflow

The dashboard follows a clear and modular workflow:

1. **Data Upload**
   Users upload fitness data files in **CSV or JSON** format through the Streamlit interface executed in **Google Colaboratory**.

2. **Data Preprocessing**

   * Timestamp conversion and sorting
   * Handling missing values using mean imputation
   * Selection of relevant numerical health metrics

3. **Feature Integration & Modeling**

   * Key features: heart rate, sleep hours, and step count
   * Anomaly detection using the **Isolation Forest** machine learning algorithm

4. **Interactive Analysis**

   * Metric-wise and date-wise filtering
   * Dynamic execution of anomaly detection based on selected filters

5. **Visualization & Reporting**

   * Interactive trend graphs with anomaly markers
   * Generation and download of anomaly summary reports in CSV format

---

## 3. Tools & Libraries Used

* **Programming Language:** Python
* **Dashboard Framework:** Streamlit
* **Notebook Environment:** Google Colaboratory
* **Machine Learning:** Scikit-learn (Isolation Forest)
* **Data Processing:** Pandas, NumPy
* **Visualization:** Plotly
* **Deployment/Tunneling:** Ngrok

---

## 4. Key Insights from the Dashboard

* Sudden spikes or drops in **heart rate** are effectively identified as anomalies, helping detect potential stress or health irregularities.
* **Sleep duration anomalies** reveal inconsistent sleep patterns, indicating possible fatigue or lifestyle imbalance.
* Abnormal **step count behavior** highlights unusually sedentary or overly active days.
* Combined metric analysis allows better contextual understanding of health anomalies rather than isolated observations.
* The downloadable report enables further offline analysis and documentation.

---

## 5. Screenshot References

* **Figure 1:** Dashboard Home Page with Data Upload Option
* **Figure 2:** Heart Rate Trend with Anomaly Markers
* **Figure 3:** Sleep Duration Analysis with Detected Anomalies
* **Figure 4:** Step Count Behavior Visualization
* **Figure 5:** Anomaly Summary Report Download Section

(*Screenshots to be captured from the Streamlit dashboard execution in Google Colab*)

---

**End of Report**
