### Predicting Human Cognitive Performance

**Author: Michael Viet Nguyen**

#### Executive summary
	This project aims to identify which measurable lifestyle factors most strongly predict an individual’s calculated Cognitive Score. The findings from EDA revealed that lifestyle factors vary widely in their predictive utility. 

	To preface, Reaction_Time and Memory_Test_Score were excluded from the numerical feature analysis. These values were measured and use to compute the Cognitive Score target feature.

	Analysis of numeric features indicated that Stress_Level had the highest linear correlation value with Cognitive Score, exhibiting a negative correlation of -0.227639. 

	Exercise Frequency was identified as the most impactful categorical predictor, accounting for a significant 14.21 point difference in mean Cognitive Score between high and low frequency groups. Comparatively, factors like Diet_Type and Gender showed negligible predictive power (0.34 points difference in mean). 

	The modeling phase will now proceed using Linear Regression as a baseline model and Random Forest Regressor to quantify the exact feature importance ranking of the remaining lifestyle variables.

#### Rationale
	Understanding which factors most reliably influence cognitive performance is critical for employers, educators, and public health officials who design wellness and development programs. Identifying reliable predictors allows organizations to make smarter decisions about how to optimize scheduling, target resources, or implement intervention strategies. For instance, if stress levels are confirmed as a dominant negative predictor, a company can focus efforts on employee stress reduction programs rather than expensive, generalized training. This analysis aims to provide actionable, data driven intelligence to maximize human performance in work and educational settings.


#### Research Question
	Which measurable lifestyle factors most strongly predict an individual's calculated Cognitive Score?


#### Data Sources
	I will be using Samharison’s “Human Cognitive Performance Analysis: Lifestyle & AI Predictions” dataset from Kaggle, which includes 80,000 samples detailing lifestyle factors, demographic attributes, and computed cognitive performance scores.


#### Methodology

	1. Data Preprocessing and Cleaning: 

		- This stage involved handling missing and duplicate values, conducting outliers analysis, and performing critical data integrity checks
    	- Numeric features (such as stress levels and sleep duration) were prepared using scaling methods to standardize their range, addressing minor skewness
    	- Categorical variables (such as diet type and demographic attributes) were prepared using one hot encoding.

	2. Supervised Learning: 

		- The Random Forest Regressor will be implemented to build the predictive model for the Cognitive Score
		- This model handles non linear relationships and will provide the best interpretable feature importance rankings

	3. Feature Importance Analysis: 

		- This technique will quantify the contribution of the input variables, providing a direct rank order answer to the research question


#### Results
	Categorical Feature Findings:

		- Exercise Frequency: Showed a massive difference of 14.21 points in mean `Cognitive_Score` between the highest and lowest frequency groups
		- Gender and Diet Type: Both showed a maximum difference of only 0.34 points in mean `Cognitive_Score` between their respective highest and lowest groups

	Numeric Feature Findings:
		- Excluding the 'Reaction_Time' and 'Memory_Test_Score', the correlation matrix showed that 'Stress_Level' is the strongest linear correlate among the remaining numeric predictors, exhibiting a negative correlation of -0.227639 with the Cognitive Score.

	This EDA indicates that both ExerciseFrequency and Stress Level are highly valuable predictors.


#### Next steps
	The next steps involve implementation and training of our Random Forest Regressor, applying the Feature Importance Analysis to rank all predictors, and interpreting the final evaluation metric.


#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information