# 🎯 Campaign Success Predictor

A machine learning project built in **Azure ML Studio** that predicts whether a marketing campaign will be successful based on key campaign attributes.

This project was created as part of an AI portfolio initiative using synthetic marketing data for robotics company, **Neuverra**.

---

## 📦 What’s Inside

| File / Notebook                  | Purpose |
|----------------------------------|---------|
| `1-workspace.png` | Workspace setup showing notebooks and pipeline files. |
| `2-autoML_run.png` | AutoML project overview with dataset and job configuration. |
| `3-autoML_model_metrics.png` | Model metrics dashboard showing accuracy, precision-recall, ROC, and other. |
| `4-EDA_stats.png` | EDA summary stats |
| `5-correlation_matrix.png` | Correlation heatmap |
| `6-success_distribution.png` | Distribution of success_flag |
| `7-success_per_campaign.png` | Success by campaign objective boxplot |
| `8-feature_importance.png` | Feature importance chart |
| `9-predictive_analysis_email_campaign.png` | Sample prediction output of success for a future email campaign. |

---

## 🧠 Model Summary

We used Azure's **AutoML** to train a classifier to predict a binary `success_flag` outcome based on a variety of features like:

- Channel (`Email`, `Direct Sales`, etc.)
- Objective (`Promote New Product`, `Customer Retention`, etc.)
- Target Audience (`Retail`, `SMB`, etc.)
- Metrics (Impressions, Conversions, Click-Through Rate, etc.)
- Pipeline Value Generated
- AI Score (custom Neuverra metric)

The final model was deployed for live testing and returned accurate results using new data.

---

## 🛠️ Tech Stack

- **Azure Machine Learning Studio**
- Python 3.10
- Pandas / Matplotlib / Sklearn
- Azure AutoML

---

## 🗂️ Dataset Notes

The original dataset was, let’s say, “enthusiastically random.” Early work involved extensive **data prep and reshaping** to make the structure meaningful before applying any ML logic. While this didn’t necessarily improve predictive accuracy, it gave the data a cleaner backbone to work with.

---

## 🔍 Feature Importance

The most impactful features in predicting campaign success were:

- `click_through_rate`
- `conversion_rate` 
- `AI_score` and `pipeline_value_generated` made minor contributions.
