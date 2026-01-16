# Steel Plate Fault Detection & Economic Impact Analysis

### 📋 Project Overview
An end-to-end Machine Learning pipeline for multi-class steel plate fault detection, integrated with a **Cost-Sensitive Learning strategy** to minimize operational financial risk rather than just maximizing raw accuracy.

### 💰 Business Value (Cost-Benefit Analysis)
Traditional ML models treat all errors equally, but in a steel mill, a **missed defect (False Negative)** causes massive liability compared to a **false alarm (False Positive)**.
* **Scenario Simulation:** Defined a Cost Matrix where a missed fault costs **$1,000** (client claim) and a false alarm costs **$50** (re-inspection).
* **Optimization:** By shifting the optimization target from "Accuracy" to "Risk Minimization", the model adjusts decision thresholds dynamically.
* **Impact:** Achieved a **~40% reduction in total estimated cost** compared to the baseline strategy, prioritizing defect capture to protect brand reputation.

### 🛠️ Methodology
```mermaid
graph LR
A[UCI Raw Data] --> B(Data Cleaning & Feature Engineering)
B --> C{Ensemble Model<br/>LGBM + RF + LR}
C --> D[Risk Minimization<br/>via Cost Matrix]
C --> E[Root Cause Analysis<br/>via SHAP Values]
### 📊 Results
