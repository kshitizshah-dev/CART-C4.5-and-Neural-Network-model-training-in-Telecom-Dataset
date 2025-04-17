ML Model Training for Classification Value Prediction
This project focuses on developing and analyzing machine learning models for predicting classification values, with a focus on customer turnover and churn.  It involves data preprocessing, normalization, model training, and evaluation.

📁 Dataset
The dataset used contains 7,043 entries with features related to customer behavior.

After preprocessing, irrelevant or incomplete data entries were removed for better accuracy.


🔍 Data Preprocessing
Three approaches for handling missing values were considered:

Dropping rows with empty cells (human bias introduced).

Filling missing values with statistical measures (mean/median/mode).

Predicting missing values using ML (more accurate, but complex).

--- I used option 1 — dropped rows with missing values — since the dataset was large enough and this method was simpler and effective.

📊 Visualization
Data visualization helped identify trends and distributions within the dataset before feeding into ML models. These included:

Categorical value distributions

Churn ratio visualization

Feature relationships

---- Data Normalization
StandardScaler was used to normalize the features.

Ensures fair contribution of each feature to the model training process.

🧠 Models Implemented
The following models were trained and compared:

1. CART (Classification and Regression Tree)
Criterion: gini

With and without class_weight adjustments

2. C4.5 (simulated using entropy criterion)
Criterion: entropy

With and without class_weight

3. AdaBoost Classifier
Boosting technique

Basic implementation with default settings

4. Neural Network
A simple feedforward neural network

Accuracy tested after normalization

✅ Evaluation Metrics
Each model was evaluated based on:

Accuracy Score

Confusion Matrix

Weighted vs Non-weighted comparison
