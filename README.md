# PIMA Diabetes Prediction

A machine learning pipeline to predict the likelihood of diabetes in patients 
based on health attributes, built with an end-to-end MLOps workflow.

## Business Context
A healthcare clinic needs to identify high-risk diabetes patients early to enable 
timely intervention. This project uses the PIMA Indian Diabetes dataset to build 
a predictive model and deploy it as a real-time web application.

## Dataset Features
| Feature | Description |
|---|---|
| preg | Number of pregnancies |
| plas | Plasma glucose concentration |
| pres | Diastolic blood pressure (mm Hg) |
| skin | Triceps skinfold thickness (mm) |
| test | 2-hour serum insulin (mu U/ml) |
| mass | Body mass index (BMI) |
| pedi | Diabetes pedigree function |
| age | Age (years) |
| class | Outcome — 1: Diabetic, 0: Non-Diabetic |

## MLOps Pipeline (GitHub Actions)
push to main
│
▼
setup-environment → register-dataset → data-prep → train-model → deploy-hosting



## Tech Stack
- **Model:** Gradient Boosting Classifier (scikit-learn)
- **Data & Model Registry:** Hugging Face Hub
- **CI/CD:** GitHub Actions
- **Frontend:** Streamlit on Hugging Face Spaces
- **Serialization:** joblib

## Live Demo
[PIMA Diabetes Prediction App](https://huggingface.co/spaces/kcharoensri/PIMA-Diabetes-Prediction)
