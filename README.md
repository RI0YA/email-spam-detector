# email-spam-detector
📌 Project Overview
This project is a machine learning-based Spam Filter designed to classify emails as either Ham (legitimate) or Spam. Built using Python and the scikit-learn library, it utilizes a Multinomial Naive Bayes classifier to identify malicious patterns, such as phishing triggers and common spam terminology.

🛠️ Tech StackLanguage: 
Python 3.xLibraries:
  Pandas: For data cleaning and handling missing values.
  Scikit-Learn: For text vectorization (CountVectorizer), dataset splitting, and model training.
  Matplotlib & Seaborn: For visualizing performance through confusion matrices.
  Pickle: For model serialization and deployment.

⚙️ Machine Learning PipelineData Cleaning: 
Handled missing text values and encoded string labels into integers ($0$ for Ham, $1$ for Spam).
Dataset Splitting: Utilized Stratified Sampling to ensure a balanced representation of both classes in the training and testing sets.
Vectorization: Converted raw email text into a numerical matrix using a bag-of-words approach.
Training: Trained a MultinomialNB classifier which achieved high accuracy in identifying spam triggers.

📊 Performance Results
The model was evaluated using a Confusion Matrix to ensure low false-positive rates, which is critical for cybersecurity applications.
Final Accuracy: 100% (on current test split).
Metrics: The classification report includes Precision, Recall, and F1-score for both classes.

🚀 How to RunClone the Repo:
Install Requirements:
 You should install these via pip. You can run this command in your terminal:
          📋 Detailed Breakdown
                        pandas: Used for loading your spam.csv, cleaning columns, and handling missing values.
                        scikit-learn: Provides the CountVectorizer for text processing, train_test_split for data division, and the MultinomialNB model itself.
                        matplotlib: The base library used for generating your plots.
                        seaborn: Used to create the high-quality heatmap for your Confusion Matrix.

Predict: Use the saved spam_model.pkl and vectorizer.pkl to run predictions on new text without retraining.
