# Sentiment Analysis on Product Reviews

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> NLP-based sentiment classifier achieving 87% accuracy on Amazon product reviews

[Live Demo](https://your-demo.streamlit.app) | [Documentation](#) | [Report Bug](#)

---

## 📊 Quick Overview

This project implements a **text classification pipeline** to analyze customer sentiment from product reviews. Built as part of the Microsoft AI Foundations Program (Edunet Foundation, May 2025).

### Key Features
- ✅ Preprocesses 2,000+ product reviews using NLTK
- ✅ Compares Naive Bayes vs. Logistic Regression models
- ✅ Achieves **87% accuracy** with Logistic Regression (F1-score: 0.84)
- ✅ Interactive visualization of sentiment distribution

---

## 🚀 Quick Start
```bash
# Clone repository
git clone https://github.com/saisurya2003/Sentiment-Analyzer-AI.git
cd Sentiment-Analyzer-AI

# Install dependencies
pip install -r requirements.txt

# Run analysis
python main.py
```

---

## 📁 Project Structure
```
Sentiment-Analyzer-AI/
├── data/
│   ├── reviews.csv              # Raw product reviews dataset
│   └── processed_reviews.csv    # Cleaned and tokenized data
├── notebooks/
│   └── Correct_Sentiment_Analyzer_AI_Project.ipynb
├── src/
│   ├── preprocess.py            # Text cleaning and tokenization
│   ├── train.py                 # Model training scripts
│   └── evaluate.py              # Performance metrics
├── models/
│   └── logistic_regression.pkl  # Trained model
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🧠 Methodology

### 1. Data Preprocessing
- Lowercasing and punctuation removal
- Stop word removal using NLTK
- Lemmatization with WordNetLemmatizer
- TF-IDF vectorization (max features: 5000)

### 2. Model Training
Compared two classification algorithms:

| Model                | Accuracy | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| Naive Bayes         | 82%      | 0.81      | 0.83   | 0.82     |
| **Logistic Regression** | **87%**  | **0.86**  | **0.88** | **0.84** |

### 3. Evaluation
- Confusion matrix analysis
- ROC-AUC curve visualization
- Cross-validation (5-fold)

---

## 📈 Results

### Confusion Matrix (Logistic Regression)
![Confusion Matrix](screenshots/confusion_matrix.png)

### Sentiment Distribution
![Distribution](screenshots/sentiment_distribution.png)

---

## 🛠️ Tech Stack

- **Language:** Python 3.8+
- **NLP Libraries:** NLTK, TextBlob
- **ML Framework:** Scikit-learn
- **Visualization:** Matplotlib, Seaborn
- **Notebook:** Jupyter

---

## 📚 Dataset

- **Source:** [Amazon Product Reviews Dataset](https://www.kaggle.com/datasets/...)
- **Size:** 2,000 reviews
- **Classes:** Positive, Negative, Neutral
- **Distribution:** 60% positive, 30% negative, 10% neutral

---

## 🔮 Future Improvements

- [ ] Deploy interactive Streamlit app
- [ ] Test BERT/RoBERTa transformers for comparison
- [ ] Add real-time sentiment analysis API
- [ ] Expand dataset to 50,000+ reviews
- [ ] Implement aspect-based sentiment analysis

---

## 📄 License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Sai Surya Nandivada**
- GitHub: [@saisurya2003](https://github.com/saisurya2003)
- LinkedIn: [saisuryanandivada](https://www.linkedin.com/in/saisuryanandivada)
- Email: saisuryanandivada@gmail.com

---

## 🙏 Acknowledgments

- Microsoft AI Foundations Program (via Edunet Foundation)
- NLTK and Scikit-learn communities
- [Dataset source credits]
