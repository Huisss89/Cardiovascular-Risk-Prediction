# Cardiovascular-Risk-Prediction
A machine learning project that predicts an individual's cardiovascular risk level (Low, Medium, or High) based on demographic information, dietary habits, lifestyle choices, and family history.

The project explores and compares three classification algorithms: Decision Tree, Random Forest, and Logistic Regression to evaluate their effectiveness in cardiovascular risk prediction.

**Google Colab Notebook:** https://colab.research.google.com/drive/1k3s-jQzL6OY8N_ykqzwMM4NLApHBoRqe?usp=sharing

<img width="1764" height="580" alt="image" src="https://github.com/user-attachments/assets/4fc41c60-2519-412a-b563-d097c50b2b3e" />

## Dataset
The project uses a dataset named `dataset.csv`, containing **2,100 records** and 17 input features.

The dataset includes:
- **Demographic Information:** Age, gender, height, weight, and income.
- **Dietary Habits:** Vegetable intake, water intake, junk food, snacks, and alcohol consumption.
- **Lifestyle Factors:** Smoking habits, exercise frequency, transportation, and television viewing habits.
- **Family History:** History of cardiovascular disease within the family.

**Target Variable:** Cardiovascular risk level (Low, Medium, or High).

## Technologies Used
- **Python:** Model implementation and data processing
- **Pandas:** Dataset loading, manipulation, and analysis
- **NumPy:** Numerical operations and data manipulation
- **Scikit-learn:** Machine learning models, preprocessing, hyperparameter tuning, and evaluation
- **Matplotlib:** Data visualization and plotting

## Requirements
- Python 3.x
- Jupyter Notebook or Google Colab

## Project Workflow
### 1. Data Exploration and Visualization
- Explore dataset dimensions, data types, and statistical summaries.
- Analyze categorical and numerical features.
- Visualize data distributions and relationships using histograms, pie charts, bar charts, scatter plots, heatmaps, and boxplots.

### 2. Data Preprocessing
- Check for duplicate records and missing values.
- Detect and remove outliers using the Interquartile Range (IQR) method.
- Perform feature selection using Random Forest feature importance.
- Remove irrelevant features.
- Standardize numerical features using StandardScaler.
- Apply one-hot encoding to categorical features.
- Split the dataset into training (80%) and testing (20%) sets.

After preprocessing, the dataset was reduced from 2,100 to **1,352 records**, with 22 encoded features.

### 3. Model Selection and Training
Implement and train three classification algorithms:

- **Decision Tree:** Predicts cardiovascular risk through a tree-like structure of decision rules.
- **Random Forest:** Combines multiple decision trees to improve classification performance.
- **Logistic Regression:** Predicts the probability of an individual belonging to each cardiovascular risk category.

### 4. Model Validation and Hyperparameter Tuning
- Apply 5-fold cross-validation to evaluate model performance.
- Use GridSearchCV to identify suitable hyperparameters.
- Train and evaluate the optimized models.

### 5. Model Evaluation
Evaluate model performance using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC curves and Area Under the Curve (AUC)
- Confusion matrices
- Matthews Correlation Coefficient (MCC)
- Cohen's Kappa
- Balanced Accuracy
- Jaccard Index
- Hamming Loss
- Learning curves

### 6. Feature Importance Analysis
Analyze the importance of individual features using:
- Decision Tree feature importance
- Random Forest feature importance
- Logistic Regression feature coefficients

## Results and Model Comparison

The models achieved the following test accuracies:

| Classification Model | Test Accuracy |
|---|---:|
| Logistic Regression | **99.26%** |
| Decision Tree | 98.89% |
| Random Forest | 95.90% |

**Key Findings:**
- Logistic Regression achieved the highest test accuracy and the best overall balance of classification performance.
- Decision Tree also demonstrated strong classification performance and offered better interpretability through its decision rules.
- Random Forest achieved good test accuracy but showed a larger gap between training and testing performance, suggesting potential overfitting.

## Visualizations and Analysis

The project includes various visualizations to analyze model performance and understand the relationships between dataset features and cardiovascular risk.

These include:
- Data distribution and correlation heatmaps.
- Confusion matrices and classification reports.
- ROC and Precision-Recall curves.
- Learning curves and model performance comparisons.
- Feature importance charts.
- Training and testing performance analysis.

## Conclusion

This project demonstrates the application of traditional machine learning algorithms to cardiovascular risk prediction using demographic, dietary, and lifestyle-related factors.

Among the three models, Logistic Regression achieved the best overall performance, followed by Decision Tree and Random Forest. The project also highlights the importance of data preprocessing, feature selection, cross-validation, and hyperparameter tuning in developing effective classification models.
