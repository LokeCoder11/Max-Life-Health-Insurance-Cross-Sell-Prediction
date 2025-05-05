# Max-Life-Health-Insurance-Cross-Sell-Prediction
Max Life Health Insurance Cross Sell Prediction - Classification

Health Insurance Cross-Sell Prediction: A Systematic Analytical Investigation
Research Objective:
This investigation aims to develop and validate a sophisticated classification framework for predicting customer receptivity toward supplementary vehicular insurance products. The implementation of this predictive architecture will facilitate enhanced identification of high-probability conversion candidates, thereby optimizing marketing resource allocation and customer engagement strategies.
Dataset Characterization:
The analytical dataset comprises 12 distinct predictor variables encompassing customer demographic attributes, vehicular specifications, and insurance history metrics. Principal variables include Age, Gender, Region_Code, Previously_insured, Vehicle_age, Vehicle_damage, Annual_premium, PolicySalesChannel, and Vintage. The dependent variable, Response, represents a binary classification of customer interest in supplementary insurance coverage (1: Affirmative, 0: Negative).
Exploratory Data Analysis (EDA):
The exploratory phase employed systematic statistical techniques to elucidate underlying patterns and correlative relationships that informed subsequent model development.
Data Preprocessing and Normalization:

Variable Type Transformation: Categorical predictor variables including Region_Code and PolicySalesChannel underwent conversion from numerical to string formats to facilitate appropriate encoding methodologies.
Missing Value Analysis: The dataset was subjected to comprehensive examination for incomplete observations, with identified anomalies addressed to maintain data integrity.
Outlier Detection and Treatment: The Annual_premium distribution underwent scrutiny utilizing the Interquartile Range (IQR) methodology, resulting in the exclusion of 2.71% of observations that exhibited values beyond statistically acceptable thresholds.

Feature Engineering and Transformation:

Age Stratification: The continuous Age variable was discretized into three categorical strata: 'Young' (< 30 years), 'Middle Age' (30-50 years), and 'Old' (> 50 years), enabling the identification of age-associated response patterns.
Categorical Variable Encoding: One-Hot Encoding methodology was applied to nominal variables such as Gender, Vehicle_age, and Vehicle_damage, while Binary Encoding was implemented for high-cardinality features including Region_Code and PolicySalesChannel to mitigate dimensionality expansion.

Univariate and Bivariate Statistical Analysis:

Univariate Distribution Assessment: Frequency distributions and boxplots were employed to analyze the statistical properties of continuous variables including Age, Annual_premium, and Vintage.
Bivariate Relationship Examination: Bar charts and comparative boxplots facilitated the investigation of associative relationships between Response and categorical predictors such as Previously_insured, Vehicle_age, and Vehicle_damage. The analysis revealed statistically significant associations between prior insurance status, documented vehicle damage, and heightened receptivity to supplementary insurance offerings.

Correlation Analysis:

Annual_premium and Vintage were subjected to detailed correlation analysis to quantify their associative relationship with the target variable.

Predictive Model Development:
The dataset underwent stratified partitioning into training (80%) and validation (20%) subsets. Multiple classification algorithms were implemented, including Logistic Regression, Random Forest, and XGBoost. Hyperparameter optimization was conducted through cross-validation, with precision designated as the primary evaluation criterion due to its relevance in minimizing false positive classifications.
Model Performance Evaluation:

The predictive frameworks were assessed using a multidimensional evaluation approach incorporating Precision, Recall, F1-Score, and Accuracy metrics. The Random Forest algorithm demonstrated superior predictive performance with elevated precision metrics, establishing it as the optimal classification framework.
The confusion matrix and Receiver Operating Characteristic (ROC) curve with calculated Area Under Curve (AUC) provided additional validation of the model's discriminative capacity between positive and negative response categories.

Feature Importance Analysis:

The finalized model identified Previously_insured, Vehicle_damage, and Annual_premium as variables with maximum predictive influence. These findings suggest that customers with established insurance history, documented vehicle damage incidents, and higher premium payment structures exhibit significantly increased propensity for positive response to supplementary insurance offerings.

Conclusion and Implementation Implications:
The optimized predictive framework effectively differentiates between receptive and non-receptive customers with high precision metrics. This model is suitable for deployment within marketing operational contexts to optimize customer targeting strategies, ensuring resource allocation toward high-probability conversion candidates. The insights derived from feature importance analysis provide strategic guidance for future marketing initiatives and product development strategies within the insurance sector.
