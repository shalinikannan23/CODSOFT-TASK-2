# CODSOFT-TASK-2
# Spam Detection Using Naive Bayes

# Overview
This code demonstrates the implementation of a spam detection model using the Naive Bayes algorithm. The dataset used for training and testing the model is named "spam.csv." The code involves data preprocessing, model training, evaluation, and comparison of two text vectorization techniques: Count Vectorizer and TF-IDF Vectorizer.

# Step 1: Importing Libraries
The necessary libraries are imported, including numpy, pandas, seaborn, matplotlib.pyplot, and chardet for encoding detection and data visualization. Additionally, sklearn modules for model building, evaluation, and text feature extraction are imported.

# Step 2: Reading the Dataset
The dataset "spam.csv" is read into a Pandas DataFrame (df). The encoding of the file is detected using the chardet library to ensure correct reading of the text data.

# Step 3: Data Cleaning
The code cleans the dataset by:

Dropping unnecessary columns.
Renaming columns for better clarity.
Mapping the target labels: 'ham' (non-spam) as 0 and 'spam' as 1.

# Step 4: Data Visualization
A pie chart is created to visualize the distribution of spam and ham messages in the dataset.

# Step 5: Data Splitting
The dataset is split into features (X) and target labels (y). The data is then divided into training and testing sets using an 80-20 split.

# Step 6: Model Training and Testing (Count Vectorizer + Naive Bayes)
A Pipeline is constructed with:

CountVectorizer to convert the text data into a matrix of token counts.
MultinomialNB as the Naive Bayes classifier.
The model is trained on the training set (X_train, y_train) and predictions are made on the test set (X_test).

# Step 7: Model Evaluation (Count Vectorizer + Naive Bayes)
The model's performance is evaluated using:

Accuracy Score to measure the overall correctness of predictions.
Classification Report to display precision, recall, F1-score, and support for each class.
Confusion Matrix visualized using a heatmap to show the true vs. predicted labels.
# Step 8: Model Training and Testing (TF-IDF Vectorizer + Naive Bayes)
A second Pipeline is constructed with:

TfidfVectorizer to convert the text data into TF-IDF features.
MultinomialNB as the Naive Bayes classifier.
The model is again trained on the training set and predictions are made on the test set.

# Step 9: Model Evaluation (TF-IDF Vectorizer + Naive Bayes)
Similar to the previous step, the model's performance with TF-IDF features is evaluated using:

# Accuracy Score for overall correctness.
Classification Report for detailed metrics.
Confusion Matrix visualized using a heatmap.
