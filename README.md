# PRODIGY_DS_02.ipynb
Titanic EDA – Passenger Survival Analysis 🚢

Overview
This repository contains a clean and concise exploratory data analysis (EDA) on the classic Titanic dataset. The goal is to explore relationships between passenger attributes (like sex, age, class, embarkation point) and survival outcomes, identify key patterns, and summarize actionable insights.


Dataset

Source: Kaggle’s “Titanic: Machine Learning from Disaster”
File: train.csv
Contains 891 passenger records with features including:
- Survived (binary: 0 = No, 1 = Yes)
- Pclass (1st, 2nd, 3rd class)
- Name, Sex, Age, SibSp, Parch
- Ticket, Fare, Cabin, Embarked

Data Cleaning

- Age imputation: Replaced missing Age values with the median.
- Dropping low-value columns: Removed Cabin (significant missing data).
- Handling missing categories: Dropped rows lacking Embarked entries.

These steps were essential to ensure clean inputs for accurate plotting and correlation analysis.

Exploratory Analysis & Visualizations

- Survival vs. Sex: Bar charts highlight a clear gender disparity.
- Survival vs. Pclass: Visuals show 1st class passengers had higher survival rates.
- Survival vs. Embarked: Analysis suggests minor but interpretable differences by embarkation point.
- Age distribution: Kernel density plots and boxplots expose how survival probabilities varied across age groups.
- Correlation heatmap: Numeric variables—like Fare, SibSp, and Parch—were assessed for links to survival likelihood.

Key Findings

Gender Advantage

- Females had a notably higher survival rate (~74%) compared to males (~19%).

Class Matters

- 1st class passengers saw around a 63% survival rate, vs. ~24% for 3rd class.

Age Trends

- Children (under 16) survived at higher rates than adults.

- Elderly passengers had noticeably lower survival rates.

Embarkation Impact

- Passengers boarding at Cherbourg (C) showed slightly higher survival (≈55%) than from Southampton (S) or Queenstown (Q).

Insights & Interpretation

Social Priority: The “women and children first” policy was strongly operative.
Economic Disparity: Higher-class passengers had better access to lifeboats.
Network Effects: Traveling in small family groups (captured by SibSp/Parch) slightly improved survival odds—possibly due to family prioritization in rescue.

Limitations

- No advanced feature engineering (e.g., extracting titles from names).
- Imputation of missing ages is rudimentary—regression-based or group medians could improve accuracy.
- The dataset lacks details like ticket position or deck level, limiting deeper insights.

Only simple stat plots were used; multivariate models (e.g., logistic regression) could reveal stronger patterns.

Conclusion

From my analysis, I found that gender, class, and age played a big role in who survived. Women and first-class passengers were more likely to survive. Younger people also had better chances. Where a person got on the ship and whether they were with family seemed to have a smaller effect. This analysis helped me understand how these factors connect to survival on the Titanic.

