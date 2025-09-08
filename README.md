# Heart Disease Detection

**Dataset:** Kaggle Heart Failure Prediction Dataset

**Objective:** To classify whether a patient has heart disease using machine learning models.

**Steps Taken:**
**Step 1: Dataset Setup**
Installed Kaggle API, uploaded `kaggle.json`, downloaded the dataset, unzipped it, and loaded the CSV file into a Pandas DataFrame.

**Step 2: Data Cleaning**
Checked for missing values and duplicate rows. Removed any duplicates to ensure data integrity.

**Step 3: Encoding and Balancing**
Encoded categorical features using LabelEncoder. Addressed class imbalance using SMOTE to oversample the minority class, ensuring balanced data for model training.

**Step 4: Train-Test Split and Scaling**
Split the dataset into training and test sets (80-20 split). Standardized the features using StandardScaler to improve model performance.

**Step 5: Model Selection and Cross-Validation**
Implemented Decision Tree and K-Nearest Neighbors classifiers. Applied 5-fold stratified cross-validation to evaluate the initial performance of both models.

**Step 6: Hyperparameter Tuning**
Used GridSearchCV to find the best hyperparameters for Decision Tree (max depth and criterion) and KNN (number of neighbors and weights) to optimize model performance.

**Step 7: Model Evaluation**
Evaluated the tuned models on the test set using Accuracy, Precision, Recall, F1 Score, and Classification Report.

**Step 8: Visualization**
Plotted a bar chart comparing Accuracy, Precision, Recall, and F1 Score of Decision Tree and KNN for easy interpretation of results.

**Results:**
Decision Tree
Accuracy 0.8676
Precision 0.8641
Recall 0.8725
F1 Score 0.8683

KNN
Accuracy 0.8529
Precision 0.9000
Recall 0.7941
F1 Score 0.8438

The bar chart visualization confirms that the Decision Tree has slightly higher overall performance, while KNN achieves higher precision but lower recall.

<img width="567" height="435" alt="image" src="https://github.com/user-attachments/assets/ae152ed1-f2b4-4933-9f4c-c0352fee85bb" />


**Future Improvements:**
Consider using ensemble methods like Random Forest or XGBoost, applying AutoML for automated model optimization, and performing advanced feature engineering to enhance prediction accuracy.
