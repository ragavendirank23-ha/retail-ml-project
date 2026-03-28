# ML Workflow Assignment

## Task 1: Identification of Label and Data Leakage
- **Label:** `repeat_purchase_flag`. 
  - *Justification:* This is the target variable representing the specific outcome (repeat purchase within 30 days) that the model is being trained to predict.
- **Data Leakage:** `discount_used_on_repeat_order`.
  - *Justification:* This feature provides information about the repeat purchase event after it has occurred, meaning it wouldn't be available in a real-world scenario where we are trying to predict a future event.

## Task 2: Recommended ML Workflow Steps
1. **Exploratory Data Analysis (EDA):** Before modeling, it is crucial to visualize distributions and check for missing values or outliers to ensure the data is clean and representative.
2. **Feature Engineering & Scaling:** Gradient boosting models can be sensitive to data quality; transforming features or handling numerical scales (like converting INR values) ensures the model interprets the importance of each feature correctly.