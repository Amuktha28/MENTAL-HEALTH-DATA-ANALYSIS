# gst
This project involves building a predictive model using GST (Goods and Services Tax) data to predict the target variable based on input features. The dataset provided is preprocessed to handle missing values, categorical variables, and scaling. The model used is a Random Forest Classifier.

# Key Methodology
# 1. Handling Imbalanced Data 
The model does not specifically mention handling imbalanced data. However, further techniques like over-sampling or under-sampling could be applied depending on the distribution of classes in the target data (observed from classification reports).

# 2.Model Selection: RandomForestClassifier

The RandomForestClassifier was chosen because it can handle both linear and non-linear data patterns and is effective in reducing overfitting through the ensemble of decision trees.
n_estimators=100: 100 trees are used to create a diverse and strong model.

# 3.Preprocessing and Data Transformation

A preprocessing pipeline was created to handle missing values, scale numeric features, and encode categorical variables (though none were present here).
StandardScaler ensures that all features contribute equally to the model, which is important for certain algorithms, such as neural networks.
# 4. Training and Validation

The model was trained on a clean, preprocessed dataset. The data pipeline helped automate preprocessing, ensuring the test data undergoes the same transformation.
No additional hyperparameter tuning was mentioned, though RandomForest hyperparameters can be fine-tuned to improve performance.

# 5.Evaluation Metrics

Accuracy: The model achieved an accuracy of 97.69%, indicating strong performance overall.
Classification Report: This shows high precision and recall for class 0, while class 1 has slightly lower precision but high recall (suggesting fewer false negatives).
AUC-ROC: 0.994: This near-perfect AUC-ROC score indicates the model is excellent at distinguishing between the two classes.

# 6.Confusion Matrix

A confusion matrix was plotted to provide insight into the number of true/false positives and negatives.
Class 0 dominates, but the model performs well across both classes, balancing false positives and false negatives effectively.
