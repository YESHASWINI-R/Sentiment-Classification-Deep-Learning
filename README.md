# 🎬 Sentiment Analysis using Deep Learning

### Simple Neural Network | CNN | LSTM

This project performs **movie review sentiment analysis** using Deep Learning techniques.
The model predicts whether a review is **positive** or **negative** based on the review text.

Three different deep learning architectures were implemented and compared:

* Simple Neural Network (ANN)
* Convolutional Neural Network (CNN)
* Long Short-Term Memory Network (LSTM)

The project was developed using **TensorFlow/Keras** in Google Colab with the IMDB Movie Reviews Dataset.

---

## 📌 Project Objective

The main goal of this project is to classify movie reviews into:

* Positive Sentiment
* Negative Sentiment

using Natural Language Processing (NLP) and Deep Learning models.

---

## 🛠️ Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

---

## 📂 Dataset Information

Dataset used:

[IMDB 50K Movie Reviews Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews?utm_source=chatgpt.com)

### Dataset Details

* 50,000 movie reviews
* Binary sentiment classification
* Balanced dataset
* Text reviews with sentiment labels

### Labels

| Sentiment | Value |
| --------- | ----- |
| Positive  | 1     |
| Negative  | 0     |

---

## 📊 Exploratory Data Analysis

Performed:

* Dataset inspection
* Class distribution visualization
* Sentiment balance checking
* Data preprocessing and encoding

The dataset contains an equal number of positive and negative reviews.

---

## ⚙️ Data Preprocessing

The following NLP preprocessing techniques were applied:

* Sentiment label encoding
* Train-Test Split
* Tokenization
* Sequence conversion
* Padding sequences using `pad_sequences`

### Configuration

```python id="e0j7b3"
MAX_WORDS = 10000
MAX_LEN = 200
```

---

# 🤖 Deep Learning Models

## 1️⃣ Simple Neural Network (ANN)

Architecture:

* Embedding Layer
* Flatten Layer
* Dense Layers

### Accuracy

✅ **86.91%**

The ANN model provided a good baseline for sentiment classification.

---

## 2️⃣ Convolutional Neural Network (CNN)

Architecture:

* Embedding Layer
* Conv1D Layer
* Global Max Pooling
* Dense + Dropout Layers

### Accuracy

✅ **88.85%**

The CNN model achieved the best performance among all models.

---

## 3️⃣ Long Short-Term Memory Network (LSTM)

Architecture:

* Embedding Layer
* LSTM Layer
* Dropout Layers
* Dense Layers

### Accuracy

✅ **87.88%**

The LSTM model captured sequential text information effectively but required higher training time.

---

## 📈 Model Comparison

| Model                 | Test Accuracy |
| --------------------- | ------------- |
| Simple Neural Network | 86.91%        |
| CNN                   | 88.85%        |
| LSTM                  | 87.88%        |

### 🏆 Best Performing Model

**CNN achieved the highest accuracy.**

---

## 🧪 Sentiment Prediction Examples

### Positive Review

```python id="ndn33k"
"I absolutely loved this movie! It was fantastic."
```

Output:

```python id="k9x1cf"
Positive
```

---

### Negative Review

```python id="v8g3ad"
"This movie was boring and a complete waste of time."
```

Output:

```python id="b7u2qa"
Negative
```

---

## ▶️ How to Run the Project

### 1️⃣ Install Required Libraries

```bash id="8sdvkl"
pip install tensorflow pandas numpy matplotlib seaborn scikit-learn kaggle
```

### 2️⃣ Upload Kaggle API File

Upload your `kaggle.json` file to access the dataset.

### 3️⃣ Run the Notebook

Execute all notebook cells step by step in Google Colab.

---

## 🔄 Project Workflow

```text id="gx8pzm"
Dataset Collection
        ↓
Text Preprocessing
        ↓
Tokenization & Padding
        ↓
Model Training
        ↓
Model Evaluation
        ↓
Sentiment Prediction
```

---

## 🚀 Future Improvements

* Add GRU and Bidirectional LSTM models
* Deploy as a web application
* Use pretrained embeddings like Word2Vec or GloVe
* Build real-time sentiment analysis system
* Add support for multilingual reviews

---

## 👩‍💻 Developed By

**Yeshaswini R**


---

## ⭐ GitHub

If you found this project useful, consider giving the repository a star ⭐
