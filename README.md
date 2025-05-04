# 🦁 Lannister Financial Analysis Console 🦁

A Streamlit application for interactive machine learning analysis on financial datasets, fit for the Lords of Casterly Rock.

**Course Name:** AF3005 – Programming for Finance
**Instructor:** Dr. Usama Arshad

---

## 📊 Console Overview
*"A Lannister always pays his debts... and analyzes his returns."*

This console provides a step-by-step interface for executing financial strategies using machine learning, ensuring your coffers remain full:

* **Load Treasury Data:** Upload CSV ledgers or scry the live markets using the Yahoo Finance (`yfinance`) API.
* **Choose Strategy:** Select your analytical approach - Predict Value (Linear Regression), Predict Outcome (Logistic Regression), or Group Assets (K-Means Clustering).
* **Refine Data:** Cleanse the ledgers by handling missing entries (imputation) and encoding non-numeric factors.
* **Select Factors of Influence:** Interactively choose input factors (X) and the target outcome (y - for supervised strategies).
* **Prepare the Battlefield / Standardize Measures:** Divide forces into training/testing sets for supervised strategies and apply standard scaling to numeric factors.
* **Execute Strategy:** Train the chosen ML model on the prepared data with configurable parameters.
* **Assess the Outcome:** Evaluate strategy performance using relevant metrics (MSE, R2, Accuracy, Confusion Matrix, Silhouette Score, Inertia).
* **Visualize & Claim Spoils:** Visualize results using interactive Plotly charts (Actual vs. Predicted Wealth, Factor Influence, House Clusters) and download the spoils of your analysis.

![image](https://github.com/user-attachments/assets/57b41ea0-e5ac-4f03-864d-53efc3af944e)



---

## ⚙️ Installation Guide
**Prerequisites:**
* Python 3.8+
* pip package manager

**Steps:**
1.  **Clone the Repository:** (Replace with your actual repository link)
    ```bash
    git clone [Link to your GitHub Repo Here]
    cd [your-repo-directory-name]
    ```
2.  **Install Dependencies:** Ensure you have a `requirements.txt` file with the following content (or create one):
    ```text
    streamlit
    pandas
    numpy
    scikit-learn
    plotly
    yfinance
    joblib
    matplotlib
    statsmodels
    ```
    Then install using pip:
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the Console:** (Update the python script name if necessary)
    ```bash
    streamlit run lannister_finance_app.py
    ```
4.  **Access:** Open your web browser and navigate to `http://localhost:8501` (or the URL provided by Streamlit).

---

## 🌐 Deployment (Optional)
*Replace with your deployment link if applicable*

**Live Console:**
https://lannister-strategies.streamlit.app/

---

## 🛠️ Features
**Core Functionality:**

* **📜 Data Input:**
    * Upload CSV Ledgers.
    * Scry Market Data via Yahoo Finance API (Tickers, Period, Interval).
* **🧠 Strategy Selection:**
    * Predict Value (Linear Regression).
    * Predict Outcome (Logistic Regression - Binary).
    * Group Assets (K-Means Clustering).
* **✨ Data Refinement:**
    * Missing Value Imputation (Mean/Mode).
    * Categorical Factor Encoding (Label Encoding).
* **🎯 Factor/Outcome Selection:**
    * Multi-select Input Factors (X).
    * Select Target Outcome (y) for supervised strategies.
* **⚔️ Preparation & Standardization:**
    * Train/Test split for supervised strategies.
    * StandardScaler for numeric factors.
* **📈 Strategy Execution:**
    * Train selected model with configurable parameters (K, C, etc.).
* **⚖️ Outcome Assessment:**
    * **Regression:** MSE, MAE, R-squared.
    * **Classification:** Accuracy, Confusion Matrix.
    * **Clustering:** Silhouette Score, Inertia (WCSS).
* **📊 Visualization (Interactive Plotly):**
    * Division of Forces Pie Chart.
    * Actual vs. Predicted Wealth Scatter Plot.
    * Factor Influence Bar Chart.
    * Confusion Matrix Heatmap.
    * 2D House Cluster Scatter Plot (user selects axes).
* **💰 Claim Spoils (Downloads):**
    * Download Strategy Bundle (`.joblib` - model, scaler, features).
    * Download Test Predictions (CSV).
    * Download Clustered Data (CSV).

---

## 📸 Demo / Screenshots



https://github.com/user-attachments/assets/9cd5e1b9-dec2-40d2-8c0a-92e1e52eba66


**Console Screenshots:**
![image](https://github.com/user-attachments/assets/244a940a-687f-4ed3-93d4-256d909610e1)
![image](https://github.com/user-attachments/assets/481d3a83-d60d-447a-929f-ad8f54ede801)
![image](https://github.com/user-attachments/assets/ce1272d2-da4b-4333-8889-4ade90913d50)
![image](https://github.com/user-attachments/assets/2b8c826b-619b-4b0c-a86c-66630c53f5f1)


---

## 📚 Technologies Used
**Armory:**

* **Console Framework:** Streamlit
* **Ledger Management:** Pandas, NumPy
* **Strategic Intelligence:** Scikit-learn (`sklearn`)
* **Market Scrying:** yfinance
* **Visual Reports:** Plotly, Matplotlib
* **Strategy Persistence:** Joblib
