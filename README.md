# 🏠 RentFreeze-Impact-Classifier-for-Makkah-Region

##  Project Overview
This project is a predictive analysis tool designed to assess the potential impact of a **Rent Freeze Policy** in the **Makkah Al-Mukarramah Region**. Inspired by the recent regulatory decisions regarding rent freezing in the Riyadh Region, this model predicts which cities and property types in Makkah would be most affected if similar regulations were implemented.

---

##  Tech Stack
*   **Language:** Python
*   **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
*   **Model:** Logistic Regression (Classification)
*   **Environment:** Google Colab 

---

##  Project Workflow

### 1. Data Engineering & Preprocessing
*   **Data Cleaning:** Cleaned column names and removed constant features (e.g., 'Region') to improve model focus.
*   **Target Labeling:** Created a dynamic "Impact Level" (`مستوى_التأثر`) based on whether the average rent exceeds the region's mean.
*   **Categorical Encoding:** Utilized `LabelEncoder` to transform cities and property types into numerical formats.
*   **Feature Scaling:** Applied `StandardScaler` to ensure all features contribute equally to the Logistic Regression model.

### 2. Model Training & Evaluation
*   **Algorithm:** Logistic Regression for binary classification.
*   **Metric Analysis:** Evaluated performance using a **Confusion Matrix** and a detailed **Classification Report** (Precision, Recall, F1-Score).
*   **Probability Prediction:** Beyond simple classification, the model calculates the specific **Probability of Impact** (`احتمالية_التأثر`) for every entry.

### 3. Key Insights (Top Cities)
The project identifies the top 5 cities most likely to be affected by analyzing the mean predicted probability of impact across different municipal areas.

---

##  Results Visualization
The model provides:
*   A **Confusion Matrix Heatmap** to visualize prediction accuracy.
*   A **Styled Ranking Table** showing the cities most vulnerable to rent freezing.
*   Probability distributions for different property types.

---


