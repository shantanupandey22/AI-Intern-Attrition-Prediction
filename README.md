# AI-Powered Attrition Prediction System

## Overview
This project predicts whether an employee is likely to leave the company (**attrition**) using the **IBM HR Analytics Employee Attrition & Performance** dataset.  
It was developed as part of a technical assessment for the AI Intern role at **ABOSS Technologies**.

The solution includes:
- Data exploration and preprocessing
- Machine learning model training
- Model evaluation and visualizations
- Research brief on a recent AI trend (RAG)

---

## Project Structure
<img width="550" height="259" alt="image" src="https://github.com/user-attachments/assets/730a9bbc-e7b2-4371-aa70-4c5fbb9c4deb" />


---

## Dataset
Source: [IBM HR Analytics Employee Attrition & Performance](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)  

Place the CSV file `WA_Fn-UseC_-HR-Employee-Attrition.csv` in the `data/` folder before running the notebook.

---

## Steps Performed

### 1. Data Understanding & Preprocessing
- Loaded dataset and explored structure
- Checked for missing values (none found)
- Encoded categorical variables with **OneHotEncoder**
- Scaled numerical features with **StandardScaler**
- Removed extreme outliers using IQR clipping

### 2. Model Building
- Algorithm: **Random Forest Classifier**
- Hyperparameter tuning with **GridSearchCV**
- Evaluation metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC
- Visualizations: Attrition count, Age vs Monthly Income, Department-wise attrition rate, Confusion Matrix, ROC Curve
- **Feature Importance** chart to understand key factors influencing attrition

### 3. Predictions
- Generated predictions for test set employees (Stay / Leave)
- Created results table with actual vs predicted labels

### 4. Research Brief
- Topic: **Retrieval-Augmented Generation (RAG)**
- Covers what it is, why it matters, use case, and challenges

---

## Results
| Metric     | Score   |
|------------|---------|
| Accuracy   | ~89%    |
| Precision  | ~84%    |
| Recall     | ~82%    |
| F1 Score   | ~83%    |
| ROC-AUC    | ~91%    |

---

## How to Run
1. Clone the repository:
   git clone https://github.com/<your-username>/AI-Intern-Attrition-Prediction.git
   cd AI-Intern-Attrition-Prediction
2. Install dependencies:
   pip install -r requirements.txt
3. Download the dataset from Kaggle and place it in data/ folder:
   data/WA_Fn-UseC_-HR-Employee-Attrition.csv
4. Run the Jupyter Notebook:
   jupyter notebook notebooks/attrition_prediction.ipynb
   
## Research Brief
See report/research_brief.md for the AI trend research on Retrieval-Augmented Generation (RAG).

## License
This project is for educational purposes only.

If you paste this into your `README.md` file in GitHub, all **headings**, **bold text**, **tables**, and **code formatting** will display exactly as intended.  

Do you want me to now also give you a **ready-made `requirements.txt`** so reviewers can run it instantly? That’s usually a plus in internship submissions.
