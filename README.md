# Fake-news-Detection
This project compares four classical machine learning algorithms—Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting—for detecting fake news. Using a balanced dataset and TF-IDF vectorization, we benchmark each model on accuracy, overfitting resistance, and generalization using various optimization techniques like regularization, feature selection, and pruning.

📊 ### Dataset:

We combined two publicly available datasets containing labeled real and fake news articles, resulting in **44,000** articles with a 50:50 class distribution.
Preprocessing steps included:
- Lowercasing
- Stopword removal
- Lemmatization
- TF-IDF vectorization (with unigrams + bigrams)

🧰 ### Dependencies

- Python 3.7+
- Scikit-learn
- Pandas
- NumPy
- NLTK
- Matplotlib (for plotting results)
