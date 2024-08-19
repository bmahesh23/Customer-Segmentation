# Customer-Segmentation
#Customer Segmentation using Machine Learning

Project Overview:
This project aims to segment customers using various machine learning techniques, including both supervised and unsupervised approaches. The goal is to identify distinct customer groups based on demographic and behavioral data.

Data and Preprocessing:
- Dataset: 8068 customer records with 11 features
- Features include: ID, Gender, Ever_Married, Age, Graduated, Profession, Work_Experience, Spending_Score, Family_Size, Var_1, Segmentation
- Data cleaning: Removed 1403 rows with null values, resulting in 6665 clean records
- Encoding: One-hot encoding for categorical variables, Label encoding for target variable (Segmentation)

Tools and Libraries:
1. Python 3.x
2. pandas: Data manipulation and analysis
3. numpy: Numerical computing
4. matplotlib and seaborn: Data visualization
5. scikit-learn: Machine learning algorithms and preprocessing

Exploratory Data Analysis (EDA):
- Age distribution: Mean = 43.47 years, Standard deviation = 16.71 years
- Work Experience: Mean = 2.64 years, Standard deviation = 3.41 years
- Family Size: Mean = 2.85, Standard deviation = 1.53
- Gender distribution: 45.5% Female, 54.5% Male
- Spending Score distribution: Low (60%), Average (25%), High (15%)

Machine Learning Approaches:

1. Supervised Learning:
   a) Decision Tree Classifier
      - Accuracy: 44.71%
   b) Random Forest Classifier
      - Number of estimators: 1000
      - Accuracy: 48.16%

2. Unsupervised Learning:
   K-Means Clustering
   - Features used: Age and Family Size
   - Optimal number of clusters: 5 (determined using elbow method)
   - Visualization: 2D scatter plot of Age vs Family Size, color-coded by cluster

Key Findings:
1. The supervised models (Decision Tree and Random Forest) achieved moderate accuracy, suggesting that customer segmentation is a complex task with potential overlap between segments.
2. Random Forest outperformed Decision Tree, indicating that ensemble methods may be more suitable for this dataset.
3. K-Means clustering revealed 5 distinct customer segments based on Age and Family Size, providing a visual representation of customer groups.

Future Improvements:
1. Feature engineering to create more informative variables
2. Experiment with other algorithms (e.g., Gradient Boosting, Neural Networks)
3. Hyperparameter tuning to optimize model performance
4. Incorporate more features in the unsupervised learning approach

Conclusion:
This project demonstrates the application of both supervised and unsupervised machine learning techniques for customer segmentation. While the supervised models showed moderate performance, the unsupervised K-Means clustering provided valuable insights into customer groupings based on age and family size. These results can be used to tailor marketing strategies and improve customer targeting.]
