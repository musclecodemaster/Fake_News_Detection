# Fake_News_Detection

Fake News Detection – Assignment Summary
📌 Objective
Build a semantic classification model to distinguish between true and fake news using Word2Vec-based vectorization and supervised learning.

💼 Business Context
With the rising spread of misinformation, the goal is to create a model that automatically classifies news articles as true or fake, leveraging semantic relationships in text rather than relying only on syntax.

📂 Dataset Details
True.csv – 21,417 rows of true news

Fake.csv – 23,502 rows of fake news

Columns: title, text, date

🔧 Key Tasks and Pipeline
1. Data Preparation 
Combine true and fake datasets

Add a news_label column: 1 for true, 0 for fake

Handle null values

Merge title and text into news_text, drop other columns

2. Text Preprocessing 
Clean text: lowercase, remove brackets, punctuation, numbers

POS tagging & lemmatization (retain only NN/NNS)

Create new columns: cleaned_text, lemmatized_nouns

3. Train/Validation Split 
70% training, 30% validation split using train_test_split

4. Exploratory Data Analysis (EDA) 
Compare character lengths (cleaned vs. lemmatized)

WordCloud for top 40 words (true & fake news)

N-gram analysis (unigrams, bigrams, trigrams for both)

5. Optional EDA on Validation Data
6. Feature Extraction 
Word embedding using:

Use average word vectors for each news item

7. Model Training & Evaluation 
Train and evaluate three models:

Logistic Regression

Accuracy: ~91.2%

Decision Tree

Accuracy: ~86.9%

Random Forest

Accuracy: ~92.6% (best performance)

Metrics:

Accuracy, Precision, Recall, F1-score

Classification Reports provided
