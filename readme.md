# 🧠 Toxic Comment Classification System

## 📌 Project Overview

This project is a **Machine Learning-based Toxic Comment Classification System** that classifies user comments into multiple toxicity categories such as:

* Toxic
* Severe Toxic
* Obscene
* Threat
* Insult
* Identity Hate

It uses **Natural Language Processing (NLP)** techniques and **Machine Learning models** to detect harmful content in text.

---

## 🚀 Features

* Text preprocessing (cleaning, stopwords removal, stemming)
* Multi-label classification
* TF-IDF vectorization
* Models used:

  * Logistic Regression
  * Naive Bayes
* Performance evaluation:

  * Accuracy
  * ROC-AUC Score
  * Classification Report
* Data visualization using Seaborn & Matplotlib

---

## 🗂️ Project Structure

```
├── train.csv
├── main.py
├── README.md
├── requirements.txt
```

---

## ⚙️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Kabirr2005/toxic-comment-classification.git
cd toxic-comment-classification
```

### 2️⃣ Create virtual environment (recommended)

```bash
python -m venv venv
venv\Scripts\activate   # Windows
source venv/bin/activate   # Mac/Linux
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Download NLTK data

```python
import nltk
nltk.download('stopwords')
```

---

## ▶️ How to Run

1. Place your dataset file:

```
train.csv
```

2. Update file path in code (if needed):

```python
df = pd.read_csv("path_to_your/train.csv")
```

3. Run the script:

```bash
python main.py
```

---

## 🔄 Workflow

### 1. Data Loading

* Load dataset using Pandas

### 2. Data Exploration

* Check null values
* Label distribution
* Visualizations

### 3. Text Preprocessing

* Lowercasing
* Removing special characters
* Stopword removal
* Stemming

### 4. Feature Extraction

* TF-IDF Vectorization

### 5. Model Training

* Naive Bayes
* Logistic Regression (OneVsRestClassifier)

### 6. Evaluation

* Accuracy Score
* ROC-AUC Score
* Classification Report

### 7. Prediction

* Test custom sentences for toxicity

---

## 📊 Output Example

```
roc_auc: 0.97
accuracy: 0.92
```

---

## 🧪 Example Predictions

### Input:

```
hello wikipedia
```

### Output:

```
toxic           0
severe_toxic    0
obscene         0
threat          0
insult          0
identity_hate   0
```

---

## 📈 Visualization

* Label distribution graph
* Labels per comment
* ROC Curve for model performance

---

## 🛠️ Technologies Used

* Python
* Pandas, NumPy
* NLTK
* Scikit-learn
* Matplotlib & Seaborn

---

## ⚠️ Notes

* Ensure dataset contains required columns:

  ```
  id, comment_text, toxic, severe_toxic, obscene, threat, insult, identity_hate
  ```
* Dataset should not contain missing values in text column.

---

## 🤝 Contributing

Feel free to fork this repo and improve the model or UI.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 👨‍💻 Author

Kabir Dang
