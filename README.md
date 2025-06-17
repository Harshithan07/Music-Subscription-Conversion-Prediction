# Music Subscription Conversion Prediction – Freemium-to-Premium Modeling

## ABOUT THE PROJECT:
This project focused on developing a predictive model for XYZ, a music-listening social platform, to identify users most likely to convert from free to premium subscriptions following a promotional campaign. As an individual contributor in a team setting, I led the data preprocessing, oversampling strategy, feature selection, and classification modeling using Python and scikit-learn. The goal was to support better targeting strategies in future campaigns by using data science to rank conversion likelihoods.


## USE CASE EXPLANATION:
In the freemium business model, predicting upgrade potential is critical for increasing revenue while minimizing promotional waste. This project falls under subscription analytics, predictive modeling, and customer behavior mining. Our goal was to support marketing operations by:

- Prioritizing likely converters

- Reducing customer acquisition costs

- Improving personalization in campaigns
The dataset was highly imbalanced (~3.7% converters), making it a real-world challenge requiring robust evaluation and sampling strategies.


## HOW IT IS BUILT AND FULL WORKING:

1. Data Preprocessing:

- Cleaned and normalized a dataset of 41,540 users (1,540 adopters, 40,000 non-adopters).

- Removed irrelevant ID columns and engineered delta features for user activity trends.

- Handled imbalance using Random Oversampling on the minority class (positive converters).

2. Modeling Techniques Explored:

- Trained baseline Decision Tree and tuned Random Forest Classifier for best performance.

- Performed GridSearchCV for hyperparameter optimization (max depth, estimators, min split).

- Applied feature importance ranking to interpret the drivers of adoption.

3. Evaluation & Metric Justification:

- Chose AUC-ROC as the primary metric to handle imbalance while measuring discriminatory power.

- AUC was prioritized over accuracy or F1 due to business need to prioritize top-ranked high-likelihood adopters.

4. Key Features Identified:

- subscriber_friend_cnt, delta_friend_cnt, delta_songsListened, and friend_country_cnt were among the most influential predictors.


## OUTPUT AND RESULTS OR BENCHMARKS:

- Final Random Forest model achieved AUC ≈ 0.77, demonstrating effective separation of converters vs. non-converters.

- Identified top behavioral signals indicating subscription likelihood, enabling marketing segmentation.

- Presented actionable managerial insights with visuals for non-technical stakeholders (e.g., top predictive behaviors, targeting strategies).


## SKILLS, TOOLS:
Python, Scikit-learn, Random Forest, Decision Tree, Oversampling, ROC-AUC, GridSearchCV, Feature Importance, Classification, Data Cleaning, Model Evaluation, Business Communication

## KEYWORDS:
Freemium model, subscription analytics, imbalanced classification, customer prediction, random forest, oversampling, AUC optimization, data-driven marketing, churn prevention, music tech analytics

