💳 Credit Card Fraud Detection System

 🌟 Project Overview

This project implements a Machine Learning solution to accurately detect fraudulent transactions within a highly imbalanced credit card dataset. The core challenge was training a robust model on data where legitimate transactions vastly outnumber fraud cases (severe class imbalance).

The solution focuses on **maximizing the model's ability to catch true fraudulent transactions (High Recall)**, which is critical for minimizing financial losses in a real-world setting.

---

 🔬 Key Techniques & Methodology

* **Imbalanced Data Handling (SMOTE):** Employed the **Synthetic Minority Oversampling Technique (SMOTE)** to effectively balance the dataset. This generated synthetic data points for the minority (fraud) class, preventing the model from becoming biased towards the majority (normal) transactions.
* **Model Optimization:** Used **GridSearchCV** with Cross-Validation for extensive hyperparameter tuning across ensemble models (e.g., Random Forest, Decision Tree). This process ensured the model was optimally configured to maximize the target metric.
* **Target Metric Prioritization:** The entire pipeline was optimized around maximizing the **Recall Score**—the most crucial metric for a fraud detection system, as minimizing **False Negatives** (missed fraud) is the priority.
* **Model Persistence:** The final, optimized model is saved using the `pickle` library for rapid loading and inference in a production environment.

---

 💻 Technical Stack

* **Language:** Python
* **Analysis & Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Imbalance Handling:** `imblearn` (SMOTE)
* **Visualization:** Matplotlib, Seaborn
* **Deployment Utility:** `pickle`

---

 📊 Results Summary

The final, tuned classification model achieved strong performance on the held-out test set:

| Metric | Score | Note |
| :--- | :--- | :--- |
| **Recall Score** | **[Your Recall Score, e.g., 0.86]** | **Successfully minimizes missed fraud cases (False Negatives).** |
| Precision Score | [Your Precision Score, e.g., 0.92] | Measures the accuracy of positive predictions. |
| F1 Score | [Your F1 Score, e.g., 0.89] | Balanced metric for evaluation. |

---

 ⚙️ Installation and Setup

 1. Data Source

The dataset used is based on anonymized credit card transactions. Due to the file size, the raw data is not hosted directly on GitHub.

**Please download the `creditcard.csv` file from the link below and place it in the root directory of this project.**

DATA DOWNLOAD LINK: https://drive.google.com/drive/folders/1LqNXIOCHvEQYrYXe2MRsKwqvuDCYhLii?usp=drive_link

### 2. Prerequisites

Ensure you have Python 3.x installed.

### 3. Clone the Repository

```bash
git clone [https://github.com/Dhwanit5656/your-repo-name.git](https://github.com/Dhwanit5656/your-repo-name.git)
cd your-repo-name
