# 🚀 Next Word Prediction using BiLSTM (Teluglish NLP)

## 📌 Overview

This project focuses on building a deep learning–based **Next Word Prediction system** using a Bidirectional LSTM (BiLSTM) model.
The model is trained on a **Teluglish dataset** (a mix of Telugu and English written in Roman script), representing real-life conversational text.

The goal is to create a system that can understand sentence patterns and **predict the most probable next word** in a sequence.

---

## 🎯 Goals of the Project

* Develop an end-to-end NLP pipeline
* Train a sequence model for next-word prediction
* Handle mixed-language conversational data
* Generate meaningful and context-aware predictions
* Build a reusable prediction system

---

## 🧠 Highlights

* Custom text preprocessing pipeline
* Tokenization with vocabulary mapping
* N-gram sequence generation
* Sequence padding for uniform input
* Bidirectional LSTM architecture
* Probabilistic word prediction (Top-K sampling)
* Supports real-time inference

---

## ⚙️ Technologies Used

* **Python**
* **TensorFlow / Keras**
* **NumPy**
* Streamlit for deployment*(Optional)*

---

## 🔄 Project Pipeline

### 1️⃣ Data Preparation

* Loaded raw text dataset
* Cleaned and structured sentences
* Removed noise and invalid entries
* Preserved conversational flow

---

### 2️⃣ Tokenization

* Converted words into integer sequences
* Built a vocabulary from dataset
* Handled unknown words using tokenization

---

### 3️⃣ Sequence Creation

* Generated progressive sequences for training

Example:

```
Sentence: nenu coding chestunnanu

Sequences:
[nenu]
[nenu coding]
[nenu coding chestunnanu]
```

---

### 4️⃣ Padding

* Applied **pre-padding** to ensure equal input length
* Maintains sequence alignment for LSTM

---

### 5️⃣ Model Architecture

```
Embedding → BiLSTM → Dropout → BiLSTM → Dropout → Dense
```

* **Embedding Layer**: Converts words into dence vectors
* **BiLSTM Layers**: Captures forward & backward context
* **Dropout**: Reduces overfitting
* **Dense Layer**: Predicts next word probability

---

## 🧠 Model Configuration

* Embedding Size: 100
* LSTM Units: 100 & 80
* Dropout Rate: 0.3
* Loss Function: Categorical Crossentropy
* Optimizer: Adam
* Metric: Accuracy

---

## 📊 Performance

* Training Accuracy: ~60–66%
* Validation Accuracy: ~60–66%

The model learns sentence structure effectively despite limited and repetitive data.

---

## 🧪 Example Predictions

```
Input: nenu coding
Output: nenu coding chestunnanu fast ga complete cheyali

Input: team meeting
Output: team meeting important ga undi report prepare chestunnanu

Input: nenu coffee
Output: nenu coffee tagutunnanu relax avvali ani anukuntunnanu
```

---

## ⚠️ Challenges

* Limited dataset diversity
* Repetitive sentence patterns
* Occasional unnatural word combinations

---

## 🚀 Future Enhancements

* Improve dataset quality and size
* Implement Attention Mechanism
* Experiment with GRU / Transformer models
* Build a web-based interface using Streamlit
* Improve grammatical correctness

---

## 🏁 Conclusion

This project demonstrates how deep learning models like BiLSTM can be used to understand and generate human-like text.
It provides a strong foundation in NLP concepts such as tokenization, sequence modeling, and text generation.

---

## 👨‍💻 Author

**Sanjay Kumar**

---

⭐*If you like this project, consider giving it a star on GitHub!*
