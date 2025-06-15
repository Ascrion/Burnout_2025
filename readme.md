# Burnout 2025: Predicting MotoGP Lap Times

This project was built as part of the Burnout 2025 Datathon, where the challenge was to predict the lap time of a MotoGP rider using historical data, rider stats, bike specs, and race conditions. The dataset was huge — over 2 million rows with a mix of numerical, categorical, and engineered features — making both performance and speed crucial.

## What This Project Does:

### Makes sense of complex race data:
By creating meaningful features like Lap_Duration_per_km, Speed_vs_Avg, and Finish_Rate, we tried to capture how the rider, track, and bike all interact.

### Uses AutoML for smart tuning 
FLAML helped find the best model (ExtraTreesRegressor) with optimal parameters — saving time and boosting performance.

### Tests reliability with K-Fold validation
A 5-fold cross-validation setup ensured the model didn’t just perform well by luck. It consistently hit an RMSE around **14.3234**, which is solid given the dataset scale.

### Avoids overcomplicating the pipeline
We kept things clean — avoiding target leakage, skipping unnecessary encodings, and making sure the same logic applied to both train and test sets.
