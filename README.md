# Fake-news-Detection
This project compares four classical machine learning algorithms—Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting—for detecting fake news. Using a balanced dataset and TF-IDF vectorization, we benchmark each model on accuracy, overfitting resistance, and generalization using various optimization techniques like regularization, feature selection, and pruning.

### 📊 Dataset:

We combined two publicly available datasets containing labeled real and fake news articles, resulting in **44,000** articles with a 50:50 class distribution.
Preprocessing steps included:
- Lowercasing
- Stopword removal
- Lemmatization
- TF-IDF vectorization (with unigrams + bigrams)

### 🔧 Models & Optimization
The following models were tested:

| Model               | Key Optimization  | Test Accuracy | Overfitting Gap |
| ------------------- | ----------------- | ------------- | --------------- |
| Logistic Regression | L2 Regularization | 97.5%         | 0.37%           |
| Decision Tree       | Feature Selection | 99.4%         | 0.05%           |
| Random Forest       | Feature Selection | 96.7%         | 0.24%           |
| Gradient Boosting   | Feature Selection | **99.44%**    | **0.13%**       |

### 📈 Results
- Gradient Boosting achieved perfect recall (0 false negatives) and the highest test accuracy.

+ Logistic Regression with L2 regularization had the smallest overfitting gap, showing good generalization.

+ Feature selection significantly improved model performance by eliminating noisy n-grams.

### 🧰 Dependencies

- Python 3.7+
- Scikit-learn
- Pandas
- NumPy
- NLTK
- Matplotlib (for plotting results)

### 🚀 Future Work
Integrate temporal and source metadata

Add incremental learning to adapt to evolving misinformation

Combine interpretability (Logistic Regression) with accuracy (Boosting) in hybrid models

Add explainability using SHAP or LIME

Extend to multilingual fake news detection
