# Housing Price Prediction (Philadelphia)
### Project Overview

This project explores predicting residential housing sale prices using machine learning techniques. The primary objective is to analyze how location-based and assessed-value features relate to property sale prices and to evaluate the limitations of a model trained with a restricted feature set.

The model uses XGBoost Regression and emphasizes model evaluation, feature analysis, and understanding why real-world prediction models can underperform when important information is missing.

This project is inspired by and based on the following repository:
**https://github.com/MYoussef885/House_Price_Prediction**

That project provided structural and conceptual guidance, while this implementation adapts the approach to a different dataset and focuses more heavily on diagnostic analysis and model shortcomings.

## Dataset

The dataset contains real estate transaction and assessment data for Philadelphia properties.

Key fields used:
- Longitude (lng)
-  Latitude (lat)
-  ZIP Code
-  Ward
-  Adjusted Fair Market Value
-  Total Consideration (sale price – target variable)

Preprocessing steps:
-  Removed invalid and low-value transactions
-  Filtered missing or malformed records
-  Converted date columns to datetime format
-  Selected relevant numerical features for modeling

The dataset is split into training and testing sets using an 80/20 split
## Results of the first project

- **R² Score (Training):** ~0.95  
- **Mean Absolute Error (MAE):** High relative to sale prices  

Although the R² score appears strong, the MAE indicates large absolute prediction errors, suggesting the model struggles with accurate price estimation.

## Next Steps 
Remake the model using a more comprehensive dataset that includes additional property-level features to improve housing price predictions in Philadelphia.
Future improvements to this project include incorporating additional property level features such as square footage and property age, improving the handling of categorical variables, tuning model hyperparameters using cross validation, and comparing the performance of the current model against simpler baseline models to better understand its strengths and limitations.


