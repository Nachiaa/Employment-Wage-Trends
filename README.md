**Employment and Wage Trends Analysis in New York State**
**Overview**
This project analyzes employment and wage trends in New York State using data from the Quarterly Census of Employment and Wages (QCEW). The analysis examines how total wages evolve over time, the impact of the number of establishments on wages, classifies ownership types (government vs. private), and identifies natural groupings among establishments based on characteristics. We used predictive models and clustering to uncover patterns and provide actionable insights for understanding employment and wage dynamics in New York State.

**Business Questions**
**1.** How do total wages change over the years?
Goal: Analyze wage trends and identify patterns over time.
Method: Gradient Boosting Regressor for wage prediction by year.

**2.** H ow do the number of establishments and the year influence total wages?
Goal: Assess how establishments and time jointly impact wages.
Method: Random Forest Regressor for multi-factor wage prediction.

**3.** Can we classify ownership type (government or private) based on the number of establishments and total wages?
Goal: Distinguish ownership types through observed characteristics.
Method: Decision Tree Classifier for classification of ownership type.

**4.** What are the distinct clusters of establishments based on their characteristics?
Goal: Identify natural groupings of establishments by features.
Method: K-Means Clustering for pattern identification.

**Data Overview**
The data is sourced from the QCEW program and contains approximately 2.12 million records covering employment and wage statistics for New York State. We focused on data from 2015 to 2023, analyzing employment, wage trends, and ownership types by industry.

**Methodology**
**Data Preprocessing and EDA:**
Filtered data from 2015 onwards for New York State.
Standardized and cleaned data, removing outliers to improve model quality.
Conducted exploratory data analysis (EDA) to examine distribution and characteristics of key varia bles.

**Predictive Models:**
1.Gradient Boosting Regressor: Modeled wage trends by year but showed limitations in predictive performance, with a high Mean Squared Error (MSE).
2.Random Forest Regressor: Successfully predicted total wages by establishments and year, showing high R-squared accuracy (0.9039).
3.Decision Tree Classifier: Classified ownership types but performed moderately, with 49.79% accuracy, indicating room for model refinement.

**Clustering Analysis:**
K-Means Clustering: Identified three distinct establishment clusters based on characteristics, validated with a strong Silhouette Score (0.856).

**Insights**
Wage Trends: Total wages vary significantly over time, though the Gradient Boosting model struggled with accurate prediction.
Establishment and Wage Relationship: The number of establishments and the year strongly influence total wages, captured effectively by the Random Forest model.
Ownership Classification: Establishments could be classified into government or private ownership, though improvements in feature engineering may enhance accuracy.
Establishment Clusters: Three clusters of establishments were identified, potentially reflecting variations by industry, size, or location.

**Recommendations**
1. Improve Predictive Models:
Further tuning of the Gradient Boosting model and exploring additional features may enhance wage trend predictions.
Use larger datasets with the Random Forest model while exploring ensemble methods for further accuracy.

2. Refine Ownership Classification:
Include more features, such as industry type and location, to increase classification accuracy for ownership types.

3.Utilize Establishment Clusters for Strategy:
Investigate cluster characteristics to guide market segmentation, resource allocation, and strategic decisions.

**Conclusion**
This project provides a foundational analysis of employment and wage trends in New York State. While model accuracy varied, the insights gained help understand the dynamics between wages, establishments, and ownership types. Future work will focus on refining models, addressing data quality, and expanding feature engineering to draw more precise insights.

