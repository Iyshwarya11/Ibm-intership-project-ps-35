# 🚧 Intelligent Classification of Rural Infrastructure Projects (PMGSY)

> A machine learning project built using IBM Watsonx.ai & AutoAI to classify infrastructure projects under the correct PMGSY scheme.

---

## 📌 Problem Statement

The **Pradhan Mantri Gram Sadak Yojana (PMGSY)** is a rural development program by the Indian government aimed at providing all-weather road connectivity to unconnected habitations.

Manual classification of projects into schemes like **PMGSY-I**, **PMGSY-II**, **RCPLWEA**, etc. is time-consuming, error-prone, and non-scalable.

### ✅ Objective

To build an **intelligent ML model** that can automatically classify a project into the correct scheme based on **financial and physical parameters**.

---

## 💡 Proposed Solution

- Used **IBM Watsonx.ai AutoAI** to train multiple ML models automatically.
- Data was cleaned and preprocessed using built-in tools.
- The best model (based on accuracy) was **XGBoost Classifier**.
- Model was deployed as a **REST API** using IBM Cloud.

---

## 🔧 Technologies Used

| Component        | Tech Stack                        |
|------------------|-----------------------------------|
| Data Source      | AI Kosh - PMGSY Dataset           |
| Platform         | IBM Watsonx.ai (Cloud-based)      |
| ML Pipeline      | IBM AutoAI                        |
| ML Libraries     | `scikit-learn`, `autoai-libs`, `ibm-watsonx-ai`, `pandas` |
| Deployment       | IBM Cloud - Watsonx Online API    |

---

## 🧪 Algorithm & Deployment

- AutoAI tried several classification models like:
  - Logistic Regression
  - Decision Trees
  - XGBoost (selected for best accuracy)
- Inputs:
  - `STATE_NAME`, `DISTRICT_NAME`, `LENGTH_OF_ROAD_WORK_SANCTIONED`, `COST_OF_WORKS_SANCTIONED`, etc.
- AutoAI handled:
  - Feature engineering
  - Model selection
  - Hyperparameter tuning
  - Evaluation
- Final model deployed as a **RESTful service** (Web API).

---

## 📊 Results

The model achieved high accuracy in correctly classifying the project schemes. IBM AutoAI generated the pipeline and deployment automatically. Below is an example of the deployed prediction:

