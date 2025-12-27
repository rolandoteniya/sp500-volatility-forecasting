# Optimizing S&P 500 Volatility Forecasts with Deep Learning
> **MSc Data Science & AI Dissertation | University of Liverpool**
> **Grade: 78% (Distinction)**

## 📈 Project Overview
This research investigates the predictive power of the **CBOE Volatility Index (VIX)** when integrated into Deep Learning architectures for forecasting S&P 500 volatility. I conducted a systematic "bake-off" of nine different models, ranging from traditional econometric benchmarks (ARCH/GARCH) to complex hybrid architectures.

### **The Result:**
My final **VIX-enhanced LSTM** achieved a **61.5% improvement** in forecast accuracy over the baseline ARCH model on out-of-sample test data.

---

### **📄 [View Full Dissertation Report (PDF)](./Roland%20Oteniya%20MSc%20Dissertation.pdf)**
---

## 🛠️ Tech Stack
* **Languages:** Python (Pandas, NumPy, Scikit-learn)
* **Deep Learning:** TensorFlow, Keras (LSTM, Hybrid Architectures)
* **Econometrics:** Arch (ARCH, GARCH, EGARCH, APARCH models)
* **Interpretability:** SHAP (Shapley Additive Explanations)
* **Visualization:** Matplotlib, Seaborn 

## 🧪 Methodology & Innovation
Unlike standard time-series projects, this research proved that **feature engineering** is often more critical than architectural complexity:

* **Systematic Comparison:** Benchmarked 9 models across three categories: Econometric, Deep Learning, and Hybrid.
* **Feature Dominance:** Demonstrated that a simple two-feature VIX-LSTM outperformed a complex APARCH-VIX-LSTM hybrid by **14.6%**, proving that architectural complexity does not always equate to predictive power.
* **Statistical Rigor:** Validated all results using the **Diebold-Mariano test** to ensure improvements were statistically significant.
* **Explainable AI (XAI):** Deployed **SHAP** to interpret the 'black-box' mechanics, confirming the VIX’s overwhelming importance as the dominant predictive driver.



## 📊 Key Findings

| Model Category | Top Performing Model | Accuracy vs. Baseline (ARCH) |
| :--- | :--- | :--- |
| **Econometric** | ARCH (Baseline) | -- |
| **Hybrid** | APARCH-VIX-LSTM | +46.9% |
| **Deep Learning** | **VIX-LSTM** | **+61.5%** |

### **Performance Metric Calculation**
The improvement was calculated using the Root Mean Square Error ($RMSE$) reduction:
$$\% \text{ Improvement} = \frac{RMSE_{\text{baseline}} - RMSE_{\text{optimized}}}{RMSE_{\text{baseline}}} \times 100$$

## ⚙️ Professional Reflection & Growth
* **On Optimization:** While initial hyperparameter tuning for this research was conducted through systematic manual sensitivity analysis to observe model behavior, I have since implemented automated optimization frameworks like **Optuna** in subsequent projects.
* **On MLOps:** To ensure full reproducibility, I now utilize **MLflow** or **Weights & Biases** for experiment tracking and model versioning.
* **Deployment:** Future iterations of this project will focus on containerization using **Docker** and deployment via **FastAPI** to serve real-time volatility forecasts.

## 📂 Repository Structure
* `S&P500_Volatility_LSTM.ipynb`: The full refactored data science pipeline.
* `Roland_Oteniya_MSc_Dissertation.pdf`: The complete distinction-grade report.

## 🤝 Acknowledgements
This research was submitted as part of the MSc in Data Science & AI at the University of Liverpool. Generative AI was utilized as a technical assistant to debug neural network architectures and optimize code structure for professional documentation.
