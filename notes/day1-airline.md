# Day 1 — Predicting Airline Satisfaction (Kaggle Playground S6E10)

## What I did
- Joined Kaggle Playground S6E10 competition
- Loaded train/test data using pandas in a Kaggle notebook
- Encoded the target with LabelEncoder, one-hot encoded features
  with pd.get_dummies()
- Handled missing values with fillna(0)
- Trained Logistic Regression (max_iter=5000)
- Public leaderboard score (ROC-AUC): 0.92216

## What I learned
- Kaggle input path format: /kaggle/input/competitions/<comp-slug>/train.csv
- predict_proba gives probabilities — needed for ROC-AUC scoring
- get_dummies on train and test separately can cause column mismatch;
  fix with reindex(columns=X.columns, fill_value=0)
- Validation split concept: hold out 20% to estimate performance locally

## Next steps
- Try Random Forest / XGBoost and compare scores
- Learn feature engineering + cross-validation
- Nov playground competition participation
