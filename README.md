# PlaygroundSeriesKaggle-S5E10

## Without Outlier Removal | XGB | RMSE 0.06160

XGBoost model with n_estimators=200, learning_rate=0.1, max_depth=6, min_child_weight=5. 
Preprocessed data with one-hot encoding (road_type, lighting, weather, time_of_day), 
StandardScaler on numerical features (num_lanes, curvature, speed_limit, etc.), 
and added interaction terms (curvature_speed_limit, curvature_lighting_night, speed_limit_foggy). 
Test RMSE: 0.05628, R²: 0.885, CV RMSE: 0.05613. 
Predictions rounded to three decimal places as per competition format. 
