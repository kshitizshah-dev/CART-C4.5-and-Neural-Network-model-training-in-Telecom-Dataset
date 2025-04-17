
# ML Model Training for Classification Value Prediction

This project focuses on developing and analyzing machine learning models for predicting classification values, with a focus on customer turnover and churn.  It involves data preprocessing, normalization, model training, and evaluation.


## Dataset
The dataset used contains 7,043 entries with features related to customer behavior.

After preprocessing, irrelevant or incomplete data entries were removed for better accuracy.

## 🔍 Data Preprocessing
Three approaches for handling missing values were considered:

Dropping rows with empty cells (human bias introduced).

Filling missing values with statistical measures (mean/median/mode).

Predicting missing values using ML (more accurate, but complex).

--- I droped rows with missing values as this dataset was large enough and a large portion of the data were missing in some columns. 

##  📊 Visualization
Data visualization helped identify trends and distributions within the dataset before feeding into ML models. These included:

- Categorical value distributions

- Churn ratio visualization

- Feature relationships
## Data Normalization

StandardScaler was used to normalize the features.
## 🧠 Models Implemented
The following models were trained and compared:

- CART (Classification and Regression Tree)
    Criterion: gini
    With and without class_weight adjustments

-  C4.5 (simulated using entropy criterion)
    Criterion: entropy

    With and without class_weight

- AdaBoost Classifier

- Neural Network
## ✅ Evaluation Metrics
Each model was evaluated based on:

- Accuracy Score
- Confusion Matrix
