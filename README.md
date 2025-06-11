This project applies **feature selection** techniques and trains a **Random Forest Classifier** to predict breast cancer diagnoses with high accuracy (above 90%).

## 📂 Dataset

- Source: [Kaggle - Breast Cancer Dataset](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset)
- Target: `diagnosis` column (`M` = Malignant, `B` = Benign)

## 📊 Workflow

1. **Data Preprocessing**
   - Dropped unnecessary columns (e.g., `id`)
   - Converted target labels (`M`, `B`) to binary values (1, 0)

2. **Feature Selection**
   - Used `SelectKBest` with Chi-Square test to select the top 10 relevant features

3. **Model Training**
   - Split data into train/test sets (80/20)
   - Applied `StandardScaler` for normalization
   - Trained a `RandomForestClassifier`

4. **Model Evaluation**
   - Achieved over 90% accuracy on the test set
   - Evaluated using accuracy score and classification report