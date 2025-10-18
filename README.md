# PlaygroundSeriesKaggle-S5E10

## Without Outlier Removal | XGBoost | RMSE 0.05628

- **Model**: XGBoost with `n_estimators=200`, `learning_rate=0.1`, `max_depth=6`, `min_child_weight=5`.
- **Feature Engineering**: Added interaction terms (`curvature_speed_limit`, `curvature_lighting_night`, `speed_limit_foggy`).
- **Preprocessing**: Applied one-hot encoding (`road_type`, `lighting`, `weather`, `time_of_day`) and StandardScaler on numerical features (`num_lanes`, `curvature`, `speed_limit`, etc.).
- **Performance**:
  - Test RMSE: 0.05628
  - R²: 0.885
  - CV RMSE: 0.05613
- **Submission**: Predictions rounded to three decimal places (`accident_risk`). Includes `id` and `accident_risk` columns.
- **Notes**: No outlier removal applied.
