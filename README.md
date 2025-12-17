### Predicting Human Cognitive Performance

**Author: Michael Viet Nguyen**

#### Executive summary
This project uses the Random Forest Regressor to analyze factors predicting an individual's Cognitive Score. Initial Exploratory Data Analysis (EDA) confirms strong predictive signals in the data:
• Reaction Time showed the strongest correlation with Cognitive Score (-0.818470), indicating that slower reaction times strongly correlate with lower scores.
• Memory Test Score (0.363894) was confirmed as a moderate positive predictor.
• Among categorical factors, Exercise Frequency showed the most variation in mean score, with high frequency groups achieving a considerably higher mean score than low-frequency groups.
• The data quality is confirmed to be high, as the outlier analysis showed the numeric features were highly uniform, requiring minimal treatment.

#### Rationale
Understanding which factors most reliably influence cognitive performance is critical for employers, educators, and public health officials who design wellness and development programs. Identifying reliable predictors—such as sleep duration or exercise frequency—allows organizations to make smarter decisions about how to optimize scheduling, target resources, or implement intervention strategies. For instance, if stress levels are confirmed as a dominant negative predictor, a company can focus efforts on employee stress reduction programs rather than expensive, generalized training. This analysis aims to provide actionable, data-driven intelligence to maximize human performance in work and educational settings.

#### Research Question
Which measurable lifestyle and demographic factors most strongly predict an individual's calculated Cognitive Score?


#### Data Sources
I will be using Kaggle’s “Human Cognitive Performance Analysis: Lifestyle & AI Predictions” dataset, which includes 80,000 samples detailing lifestyle factors, demographic attributes, and computed cognitive performance scores.

#### Methodology
This project utilizes a Supervised Learning approach, specifically implementing a regression model.
1. Data Cleaning and EDA: The dataset must be cleaned, including the removal of missing and duplicate values. This phase includes Outliers analysis to identify anomalies in the dataset.
2. Feature Engineering and Preprocessing: I will perform feature engineering to extraction and transformation of variables from raw data. This involves scaling numeric features (like sleep duration and stress levels) and implementing one-hot encoding for categorical variables (such as diet type and demographic attributes).
3. Modeling: I will develop an appropriate regression ML model to utilize as baseline for your analysis. I will implement the Random Forest Regressor to build the predictive model for the Cognitive Score.
4. Evaluation and Interpretation: The analysis requires a Clear identification of an evaluation metric and a Clear rationale for use of the given evaluation metric. The core research goal is Feature Importance Analysis to quantify which input variables contribute most significantly to predicting cognitive performance scores.

#### Results
The EDA confirms the presence of strong predictive features, setting the foundation for the modeling phase:
• Strongest Predictors: The most significant linear relationship was a strong negative correlation between Reaction Time and Cognitive Score (-0.818470). Memory Test Score showed a moderate positive correlation (0.363894).
• Negative Correlates: Variables like Stress Level (-0.227639), Daily Screen Time (-0.198515), and Caffeine Intake (-0.122862) showed negative correlations, aligning with the expectation that these factors negatively affect performance.
• Categorical Impact: Exercise Frequency demonstrated the greatest predictive influence among categorical features, with groups reporting high exercise frequency showing a considerably higher mean Cognitive Score than groups with low exercise frequency.
• Anticipated Performance: The Random Forest Regressor is anticipated to perform best because it handles nonlinear relationships and provides the necessary interpretable feature importance rankings, allowing us to rank these lifestyle factors precisely.

#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information