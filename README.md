# 📊 Submission Projects: Sentiment Analysis & Image Classification

This repository contains two submission projects from the **Fundamental Deep Learning** Course:

1. **Sentiment Analysis** of ChatGPT app reviews.  
2. **Image Classification** using the CIFAR-10 dataset with CNN.

## 🎓 About "Asah" Program

This submission projects was developed as part of the **Asah** Program led by **Dicoding** in association with **Accenture**, a learning initiative designed to help participants strengthen their skills through practical projects.  

---

## 🚀 Project 1: Sentiment Analysis

### 📂 Dataset
- Source: Scraped reviews from the ChatGPT app (Google Play Store).
- Format: CSV (`chatgpt_reviews.csv`).

### ⚙️ Preprocessing
- Remove duplicates & special characters.
- Case folding, tokenization.
- Stopword removal (NLTK).
- Stemming (Sastrawi).

### 🤖 Models & Accuracy
- **Scheme 1: SVM + TF-IDF (80/20 split)**
  - Training Accuracy: ~99.99%
  - Testing Accuracy: ~98.68%
- **Scheme 2: Random Forest + Word2Vec (70/30 split)**
  - Training Accuracy: ~99.53%
  - Testing Accuracy: ~85.76%
- **Scheme 3: Deep Learning LSTM (70/30 split)**
  - Training Accuracy: ~91.52%
  - Testing Accuracy: ~91.53%

### 📊 Evaluation
- Metrics: Accuracy, Precision, Recall, F1-score.
- Visualization: WordCloud, sentiment distribution.

---

## 🖼️ Project 2: Image Classification

### 📂 Dataset
- CIFAR-10 (60,000 images, 10 classes).
- Subset of 4 classes used: **airplane, automobile, bird, cat**.
- Split: Train, Validation, Test.

### ⚙️ Preprocessing
- Pixel normalization (0–255 → 0–1).
- **Data Augmentation**:
  - Rotation
  - Translation
  - Horizontal flip
  - Zoom

### 🤖 CNN Model
- Conv2D + MaxPooling
- Flatten
- Dense + ReLU
- Softmax output
- Optimizer: Adam  
- Loss: Categorical Crossentropy

### 📊 Results
- Accuracy: ~93%  
- Additional evaluation: Confusion Matrix & prediction visualization.

| Image | Predicted | True Label |
|-------|-----------|------------|
| 🐱 **cat** | cat | cat |
| ✈️ **airplane** | airplane | airplane |
| 🚗 **automobile** | automobile | automobile |
| 🐱 **cat** | cat | cat |
| 🚙 **automobile** | automobile | automobile |

---

## ⚡ How to Run

**1. Clone the repository**
```bash
git clone https://github.com/username/ml-projects.git
cd ml-projects
```
 
**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the notebooks**
- Sentiment Analysis: `notebook_model.ipynb`  
- Image Classification: `notebook.ipynb`
