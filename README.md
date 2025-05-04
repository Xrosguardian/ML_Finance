# Interactive Financial Machine Learning Pipeline

A Streamlit application for interactive machine learning analysis on financial datasets.

---

## 📊 App Overview
This application provides a step-by-step interface for performing machine learning tasks on financial data:
-   **Data Loading:** Upload CSV datasets (e.g., from Kragle) or fetch live stock data using the Yahoo Finance (`yfinance`) API.
-   **Model Selection:** Choose between Linear Regression, Logistic Regression, or K-Means Clustering.
-   **Preprocessing:** Handle missing values (imputation) and encode categorical features.
-   **Feature Selection:** Interactively select features (X) and target variable (y - for supervised models).
-   **Train/Test Split & Scaling:** Split data for supervised learning and apply standard scaling to numeric features.
-   **Model Training:** Train the selected ML model on the prepared data.
-   **Evaluation:** Evaluate model performance using relevant metrics (MSE, R2, Accuracy, Confusion Matrix, Silhouette Score, Inertia).
-   **Visualization:** Visualize results using interactive Plotly charts (Actual vs. Predicted, Feature Importance, Cluster Plots).
-   **Downloads:** Download the trained model (including scaler and feature names) and prediction/clustering results.
  
![image](https://github.com/user-attachments/assets/4b50d827-2b66-4a94-9ffb-703d1ac0d897)

---

## ⚙️ Installation Guide
**Prerequisites:**
-   Python 3.8+
-   pip package manager

**Steps:**
1.  **Clone Repository:** (Replace with your actual repository link)
    ```bash
    git clone [https://github.com/yourusername/financial-ml-pipeline.git](https://github.com/yourusername/financial-ml-pipeline.git)
    cd financial-ml-pipeline
    ```
2.  **Install Dependencies:** Create a `requirements.txt` file (provided in a previous step) with the following content:
    ```text
    streamlit
    pandas
    numpy
    scikit-learn
    plotly
    yfinance
    joblib
    matplotlib
    ```
    Then install using pip:
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the App:** (Make sure your Python script is named `finance_ml_app.py` or update the command accordingly)
    ```bash
    streamlit run finance_ml_app.py
    ```
4.  **Access:** Open your web browser and navigate to `http://localhost:8501` (or the URL provided by Streamlit).

---

## 🌐 Deployment (Optional)

**Live Demo:**
https://mlfinance-gtmnrninhlaxnaffzwb969.streamlit.app/
---

## 🛠️ Features
**Core Functionality:**

* **💾 Data Input:**
    * Upload CSV files.
    * Fetch stock data via Yahoo Finance API (Tickers, Period, Interval).
* **🤖 Model Selection:**
    * Linear Regression (for regression tasks).
    * Logistic Regression (for binary classification tasks).
    * K-Means Clustering (for unsupervised grouping).
* **✨ Preprocessing:**
    * Missing Value Imputation (Mean for numeric, Mode for categorical).
    * Basic Categorical Feature Encoding (Label Encoding).
* **🎯 Feature/Target Selection:**
    * Multi-select features (X).
    * Select target variable (y) for supervised models.
* **✂️ Data Splitting & Scaling:**
    * Train/Test split for supervised models.
    * StandardScaler for numeric features.
* **🧠 Model Training:**
    * Train selected model with configurable parameters (e.g., K for K-Means, C for Logistic Regression).
* **📈 Evaluation:**
    * **Regression:** MSE, MAE, R-squared.
    * **Classification:** Accuracy, Confusion Matrix (visualized).
    * **Clustering:** Silhouette Score, Inertia (WCSS).
* **📊 Visualization (Interactive Plotly):**
    * Train/Test Split Pie Chart.
    * Actual vs. Predicted Scatter Plot (Linear Regression).
    * Feature Importance Bar Chart (Linear/Logistic Regression).
    * Confusion Matrix Heatmap (Logistic Regression).
    * 2D Cluster Scatter Plot (K-Means - user selects axes).
* **📥 Downloads:**
    * Download trained model bundle (`.joblib` containing model, scaler, feature names).
    * Download test set predictions (CSV for supervised).
    * Download data with cluster assignments (CSV for K-Means).

---

## 📸 Demo / Screenshots


**Video Demo:**


https://github.com/user-attachments/assets/dd76e379-2f35-467b-a484-6d31f4678699


**Application Screenshots:**
![image](https://github.com/user-attachments/assets/42c5b4d4-539c-4b6a-b2b5-32a8fc601f92)
![image](https://github.com/user-attachments/assets/2d0d21cb-b8a5-4991-9349-acb3232a533a)
![image](https://github.com/user-attachments/assets/ce0b77fc-338a-4c2d-a897-1e2b7989ce79)
![image](https://github.com/user-attachments/assets/5e8e7848-b8e4-431e-bc0c-bd806561e6b4)
![image](https://github.com/user-attachments/assets/f12112ae-c77c-406e-84a3-f31f5acd9410)


---

## 📚 Technologies Used
**Stack Components:**

* **Frontend/Framework:** Streamlit
* **Data Handling:** Pandas, NumPy
* **Machine Learning:** Scikit-learn (`sklearn`)
* **Data Fetching:** yfinance
* **Visualization:** Plotly, Matplotlib (implicitly used by other libraries)
* **Model Persistence:** Joblib
