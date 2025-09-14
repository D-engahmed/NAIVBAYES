# Naive Bayes Classifiers: A Comparative Study

This project provides an in-depth comparison of three Naive Bayes classifier variants (GaussianNB, MultinomialNB, and BernoulliNB) using real-world datasets from Kaggle. The project includes comprehensive visualizations, performance metrics, and interactive components to understand when and how to use each classifier type.

## 📊 Project Overview

The notebook demonstrates:
- Theoretical foundations of different Naive Bayes classifiers
- Practical implementation on real datasets
- Interactive visualizations and performance comparisons
- Detailed analysis of each classifier's strengths and weaknesses

## 🧮 Classifiers Compared

| Classifier | Best For | Data Type | Example Use Case |
|------------|----------|-----------|------------------|
| GaussianNB | Continuous features | Real-valued | Medical diagnosis, sensor readings |
| MultinomialNB | Discrete counts | Positive integers | Text classification (word counts) |
| BernoulliNB | Binary features | 0/1 values | Spam detection, yes/no features |

## 📁 Datasets Used

1. **Wine Quality Dataset** (GaussianNB)
   - Continuous features: chemical properties of wine
   - Target: wine quality classification (Low/Medium/High)

2. **SMS Spam Collection** (MultinomialNB)
   - Text data converted to word counts
   - Target: spam/ham classification

3. **Titanic Dataset** (BernoulliNB)
   - Binary/categorical features: sex, class, alone, etc.
   - Target: survival prediction

## 🚀 Installation & Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd naive-bayes-comparison
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Download the datasets from Kaggle:
   - [Wine Quality Dataset](https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009)
   - [SMS Spam Collection](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
   - [Titanic Dataset](https://www.kaggle.com/competitions/titanic/data)

4. Place the datasets in the project directory with these filenames:
   - `winequality-red.csv`
   - `spam.csv`
   - `titanic.csv`

## 💻 Usage

Run the Jupyter notebook:
```bash
jupyter notebook explane.ipynb
```

The notebook includes:
- Detailed explanations of each Naive Bayes variant
- Code implementations with visualizations
- Interactive tabs for exploring different classifiers
- Performance comparisons across datasets

## 📈 Results Summary

| Classifier | Dataset | Accuracy | Key Strengths |
|------------|---------|----------|---------------|
| GaussianNB | Wine Quality | 71.88% | Handles continuous data well |
| MultinomialNB | SMS Spam | 98.39% | Excellent for text classification |
| BernoulliNB | Titanic | 73.43% | Effective with binary features |

## 🎨 Visualizations

The project includes multiple interactive visualizations:
- Confusion matrices for each classifier
- Feature importance charts
- PCA projections with decision boundaries
- Performance comparison charts
- Interactive tabs for exploring different datasets

## 🧠 Key Insights

1. **GaussianNB** works best with normally distributed continuous data
2. **MultinomialNB** excels at text classification with count-based features
3. **BernoulliNB** is ideal for binary/categorical data
4. Each classifier makes different assumptions about feature distributions
5. Choice of classifier should be based on data characteristics rather than performance alone

## 📚 Theoretical Background

All Naive Bayes classifiers are based on **Bayes' Theorem**:

$$P(C \mid X) = \frac{P(X \mid C)P(C)}{P(X)}$$

The difference lies in how they calculate $P(X \mid C)$:
- **GaussianNB**: Assumes features follow normal distribution
- **MultinomialNB**: Uses multinomial distribution for count data
- **BernoulliNB**: Uses Bernoulli distribution for binary features

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
