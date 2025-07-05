# CYBERSECURITY-Suspicious-Web-Threat-Interactions

This project analyzes suspicious web server traffic using Machine Learning and Deep Learning techniques to detect potential threats in real-time cloud environments. It demonstrates an end-to-end pipeline — from data cleaning and EDA to anomaly detection and classification — using Python, ML, and neural networks.

---

## 📌 **Project Overview**

- **Domain:** Cybersecurity  
- **Tools Used:** Python, Pandas, Seaborn, Matplotlib, Scikit-learn, TensorFlow, NetworkX, Jupyter Notebook, Google Colab, VS Code  
- **Difficulty Level:** Advanced  
- **Role:** Data Analyst  

---

## ⚡ **Dataset**

- **Source:** Web traffic records collected using AWS CloudWatch.
- **Content:** Each record represents a traffic stream to a web server, labeled with detection rules identifying suspicious or anomalous activities.

**Key Columns:**
- `bytes_in`, `bytes_out` — Traffic volume.
- `creation_time`, `end_time`, `time` — Timestamps.
- `src_ip`, `dst_ip` — IP addresses.
- `src_ip_country_code` — Source country.
- `protocol`, `dst_port`, `response.code` — Protocol details.
- `rule_names`, `observation_name`, `detection_types` — Suspicious activity labels.

---

## 🔍 **Project Steps**

1. **Data Import & Cleaning**
   - Load CSV data using `pandas`.
   - Remove duplicates.
   - Convert timestamps to datetime.
   - Standardize country codes.

2. **Data Transformation**
   - Feature engineering: session duration, scaling numeric features.
   - One-hot encoding for country codes.

3. **Exploratory Data Analysis**
   - Descriptive stats.
   - Correlation matrix.
   - Time-series analysis.
   - Detection type frequency by country.
   - Network graph: source IPs vs destination IPs.

4. **Machine Learning**
   - **Random Forest Classifier:** Classify suspicious vs normal traffic.
   - Metrics: Accuracy, Classification Report.

5. **Deep Learning**
   - Build a Neural Network (Sequential API, Dense layers).
   - Optionally test with CNN 1D for sequence pattern learning.
   - Visualize training & validation accuracy and loss.

6. **Visualizations**
   - Distribution plots.
   - Scatter plots with anomalies.
   - Heatmaps.
   - Network interaction graph.
