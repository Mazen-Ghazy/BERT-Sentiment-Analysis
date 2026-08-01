# 🎬 IMDb Sentiment Analysis using BERT

A Natural Language Processing (NLP) project that performs sentiment analysis on IMDb movie reviews using a fine-tuned BERT model.

---

# 📌 Project Overview

This project explores different approaches for sentiment analysis on the IMDb movie reviews dataset.

As a baseline, traditional Machine Learning models were trained using **TF-IDF** feature extraction. Several classifiers were evaluated, including:

- Logistic Regression
- Support Vector Machine (SVM)
- Multinomial Naive Bayes
- Random Forest

The best traditional Machine Learning approach achieved an accuracy of approximately **63%**.

To significantly improve performance, **BERT (bert-base-uncased)** was fine-tuned using Hugging Face Transformers, achieving an accuracy of **91.7%** on the test dataset.

The model classifies movie reviews into two classes:

- 😊 Positive
- 😞 Negative

---

# 📈 Model Comparison

| Model | Accuracy |
|-------------------------------|----------|
| TF-IDF + Logistic Regression | ~61% |
| TF-IDF + SVM | ~58% |
| TF-IDF + Multinomial Naive Bayes | ~62% |
| TF-IDF + Random Forest | ~63% |
| **Fine-Tuned BERT** | **91.7%** |

---

# 📊 Final Results

| Metric | Score |
|---------|-------|
| Accuracy | **91.7%** |
| Precision | **92%** |
| Recall | **92%** |
| F1-Score | **92%** |

---

# 🛠️ Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

---

# 📂 Project Structure

```text
Sentiment-Analysis-BERT/
│
├── train.ipynb
├── predict.py
├── requirements.txt
├── README.md
├── .gitignore
├── screenshots/
└── saved_model/      (Not included in GitHub)
```

---

# 🚀 Getting Started

## 1. Clone the repository

```bash
git clone https://github.com/your-username/Sentiment-Analysis-BERT.git

cd Sentiment-Analysis-BERT
```

---

## 2. Install the required libraries

```bash
pip install -r requirements.txt
```

---

## 3. Download the Fine-Tuned Model

The trained BERT model is hosted on **Hugging Face**.

Download the model from:

**(Hugging Face link will be added after uploading the model.)**

After downloading, create a folder named:

```text
saved_model
```

Place the downloaded files inside it.

The project should look like this:

```text
Sentiment-Analysis-BERT/
│
├── train.ipynb
├── predict.py
├── requirements.txt
├── README.md
├── .gitignore
├── screenshots/
└── saved_model/
    ├── config.json
    ├── model.safetensors
    ├── tokenizer.json
    ├── tokenizer_config.json
    ├── special_tokens_map.json
    └── vocab.txt
```

---

## 4. Run the Prediction Script

```bash
python predict.py
```

---

## 5. Enter Your Review

Example:

```text
Enter your review:

This movie was absolutely amazing!
```

Output:

```text
==================================================
Prediction : Positive
Confidence : 99.84%
==================================================
```

---

# 📷 Project Outputs

The repository includes:

- Confusion Matrix
- Classification Report
- Sample Predictions

*(Screenshots will be added.)*

---

# 🤖 Fine-Tuned Model

The fine-tuned model will be available on Hugging Face.

**Model Link:** *(Coming Soon)*

---

# 📚 Dataset

- IMDb Movie Reviews Dataset
- Binary Sentiment Classification
- Positive / Negative Reviews

---

# 💡 Future Improvements

- Deploy the model using Streamlit.
- Build a web application for real-time sentiment prediction.
- Compare additional Transformer models such as RoBERTa and DistilBERT.
- Optimize inference speed for deployment.

---

# 👨‍💻 Author

Developed as an educational NLP & Deep Learning project to compare traditional Machine Learning techniques with Transformer-based models for sentiment analysis.

This project demonstrates the complete workflow, including:

- Data preprocessing
- TF-IDF feature extraction
- Traditional Machine Learning models
- BERT fine-tuning
- Model evaluation
- Sentiment prediction (Inference)