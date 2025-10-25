
---

## 1. Data Exploration
- Conducted **Exploratory Data Analysis (EDA)** to identify trends, correlations, and feature relationships.  
- Found key predictors such as `coolingRate` and `smallDefects`.  
- Proposed hypotheses based on observed non-linear patterns and multicollinearity.

---

## 2. Regression Models
- Implemented:
  - **Support Vector Regression (RBF Kernel)**  
  - **Gradient Boosting Regressor (GBR)**  
- Tuned using **GridSearchCV (5-fold cross-validation)**.  
- **GBR outperformed SVR**, achieving:
  - **Lower RMSE (~115 hrs)**  
  - **Higher R² (~0.91)**  
- Recommended for precise numerical lifespan prediction.

---

## 3. Classification Models
- Created **multi-class target labels** using **K-Means clustering** (`k=3`: Low, Medium, High).  
- Trained:
  - **Random Forest Classifier**
  - **Multinomial Logistic Regression**
- Evaluated using **weighted F1-score** (handles class imbalance).  
- **Random Forest achieved ~0.92 F1-score**, offering high interpretability and real-world usability.  
- Recommended for deployment due to its clear and actionable output.

---

## 4. Key Insights
- Regression delivers **precision**, but classification delivers **practicality**.  
- The **multi-class model** aligns better with manufacturing decisions — enabling quick categorization of parts as *Low*, *Medium*, or *High* quality.

---

## 5. How to Run

```bash
# Create and activate environment
conda env create -f environment.yml
conda activate ml-coursework

# Launch Jupyter Notebook
jupyter notebook Machine_Learning_Coursework.ipynb
