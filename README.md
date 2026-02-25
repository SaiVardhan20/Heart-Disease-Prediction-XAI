📘 Heart Disease Prediction using Explainable AI (XAI)

This repository contains the research paper, dataset, and implementation code for the project:

“Evaluating Explanation Consistency of Explainable Machine Learning Models for Heart Disease Risk Prediction.”

The project focuses on clinical risk prediction, explainable AI, and explanation reliability analysis using SHAP and LIME across multiple machine learning models.

🔍 1. Project Overview

Cardiovascular disease is one of the leading causes of mortality worldwide. Machine learning models can predict heart disease risk from clinical attributes, but their adoption in healthcare is limited due to lack of interpretability and trust.

Explainable AI (XAI) methods such as SHAP and LIME help interpret model predictions. However, different explainability methods may provide inconsistent explanations for the same patient.

This project investigates:

Predictive performance of ML models for heart disease

Reliability of SHAP vs LIME explanations

Quantitative explanation consistency

Case-based interpretability aligned with clinical reasoning

🧠 2. Key Objectives

Predict heart disease using machine learning

Compare interpretable vs black-box models

Generate global and local explanations

Quantify SHAP–LIME explanation agreement

Evaluate explanation stability in healthcare AI

Improve interpretability via case-based reasoning

🗂 3. Project Structure
Heart-Disease-Prediction-XAI/
│
├── data/
│   └── heart.csv
│
├── paper/
│   └── Evaluating Explanation Consistency of Explainable Machine Learning Models for Heart Disease Risk Prediction.pdf
│
├── heart_disease_xai.ipynb
├── README.md
📊 4. Dataset

The project uses the UCI Heart Disease (Cleveland) dataset containing structured clinical attributes.

Feature	Description
age	Age
sex	Sex
cp	Chest pain type
trestbps	Resting blood pressure
chol	Cholesterol
fbs	Fasting blood sugar
restecg	ECG results
thalach	Max heart rate
exang	Exercise angina
oldpeak	ST depression
slope	ST slope
ca	Number of vessels
thal	Thalassemia
target	Heart disease

Location: data/heart.csv

🛠 5. Methodology (What the Notebook Does)

The notebook follows an end-to-end explainable ML pipeline.

Step 1 – Data Loading & Inspection

Load UCI heart dataset

Check class distribution

Verify feature types and ranges

Step 2 – Preprocessing

Train/test split (stratified)

Feature scaling for LR & MLP

Raw features for Random Forest

Handling clinical feature encoding

Step 3 – Model Training

Models trained:

Logistic Regression

Random Forest

Multi-Layer Perceptron

Training uses:

Binary cross-entropy loss

Class weighting

Cross-validation

Step 4 – Model Evaluation

Metrics computed:

Accuracy

Precision

Recall (Sensitivity)

Specificity

F1-score

ROC-AUC

Calibration assessed using:

Calibration curves

Brier score

Step 5 – Explainable AI
🔹 SHAP

Global feature importance

Local patient explanations

Beeswarm plots

Force plots

🔹 LIME

Local surrogate explanations

Feature contribution visualization

Step 6 – Explanation Consistency Analysis

For each patient:

Extract top-k SHAP features

Extract top-k LIME features

Compute feature overlap score

This quantifies agreement between explainability methods.

Step 7 – Case-Based Explanation

Predictions are compared with similar patients using:

Nearest-neighbor similarity

Outcome statistics

Feature attribution

This improves clinical interpretability.

📈 6. Results (Summary)

Random Forest achieved highest ROC-AUC and recall

Logistic Regression provided strong interpretability

SHAP and LIME showed moderate agreement

Explanation variability observed across patients

Case-based explanations improved trust

🚀 7. How to Run the Project
1️⃣ Install Dependencies
pip install numpy pandas scikit-learn matplotlib shap lime
2️⃣ Open Notebook
jupyter notebook heart_disease_xai.ipynb
3️⃣ Run All Cells

The notebook will:

Train models

Evaluate performance

Generate SHAP & LIME explanations

Compute consistency metrics

🧪 8. Technologies Used

Python

NumPy

Pandas

scikit-learn

Matplotlib

SHAP

LIME

Jupyter Notebook

📄 9. Research Paper

The paper/ folder contains:

Full methodology

Experimental results

Equations

Workflow diagrams

Literature review

🙌 10. Authors

Kari Sai Vardhan (Lead Author)

Maram Ramakrishna Reddy

Kore Akhil

Modugula Pavan Kumar Reddy

Aaskaran Bishnoi

⭐ 11. Citation

If you use this work:

Kari Sai Vardhan et al.,
“Evaluating Explanation Consistency of Explainable Machine Learning Models for Heart Disease Risk Prediction”
ICTIS Conference, 2026
