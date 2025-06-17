# Music Subscription Conversion Prediction – Freemium-to-Premium Modeling

## ABOUT THE PROJECT:
This project focused on building a predictive model for XYZ, a music-listening social network, to identify users most likely to convert from free to premium subscriptions after a campaign. Implemented entirely in R, the solution handled imbalanced class distribution, evaluated multiple classifiers, and provided interpretable metrics for targeting optimization. I led the model development, feature evaluation, and presentation of managerial insights.


## USE CASE EXPLANATION:
In freemium business models, predicting high-likelihood converters is essential to increase ROI on campaigns. This case addressed subscription analytics, where identifying responsive users helps improve personalization and reduce marketing spend. The project is relevant for marketing analysts, data scientists, and growth strategists in digital platforms or subscription-based services.


## HOW IT IS BUILT AND FULL WORKING:

1. Data Preparation:

- Dataset: 41,540 users (1,540 adopters, 40,000 non-adopters) with 25 behavioral attributes.

- Removed identifiers, engineered delta-based behavior change features.

- Performed Smote oversampling to address 1:26 imbalance.

2. Modeling:

- Trained Decision Tree and Random Forest models using rpart, randomForest, and ROCR libraries.

- Conducted 5-fold cross-validation.

- Evaluated using AUC, F1 Score, and Cumulative Response Curves.

3. Model Insights:

- Random Forest outperformed others with AUC = 0.77 and strong lift in top deciles.

- Top predictors: subscriber_friend_cnt, delta_songsListened, delta_friend_cnt, and avg_friend_male.

4. Presentation:

- Translated technical metrics (TPR, Precision, ROC) into business KPIs.

- Delivered a managerial summary with targeting strategies for high-response segment


## OUTPUT AND RESULTS OR BENCHMARKS:

- Final Random Forest model achieved AUC ≈ 0.77, demonstrating effective separation of converters vs. non-converters.

- Top 3 deciles captured 60–70% of all converters, guiding priority targets.

- Visualized adoption potential via cumulative response and lift charts for campaign ROI.


## SKILLS, TOOLS:
R, rpart, randomForest, ROCR, caret, dplyr, data visualization, oversampling, ROC curve, F1 score, cumulative gains, segmentation modeling

## KEYWORDS:
Freemium analytics, music tech, R machine learning, subscription prediction, class imbalance, random forest in R, ROC-AUC, campaign targeting, lift chart, marketing analytics

