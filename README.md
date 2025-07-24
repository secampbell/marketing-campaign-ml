# 🎯 Campaign Success Predictor

A machine learning project built in **Azure ML Studio** that predicts whether a marketing campaign will be successful based on key campaign attributes.

This project was created as part of an AI portfolio initiative using synthetic marketing data for robotics company, **Neuverra**.

---

## 📦 What’s Inside

| File / Notebook                  | Purpose |
|----------------------------------|---------|
| `eda_marketing_campaigns.ipynb` | Cleaned and restructured a chaotic dataset into meaningful campaign logic |
| `campaign_prediction_pipeline.ipynb` | Trains a classification model using AutoML & prepares it for deployment |
| `feature_importance_chart.png`  | Visual showing which features matter most |
| `sample_prediction_output.png`  | Shows an example predicted `success_flag` of 1.00 |

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
