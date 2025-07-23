# 🧠 Advanced Sentiment Analysis — GloVe & BERT

This project is an advanced version of sentiment analysis, building upon version 1, where we used TF-IDF (Term Frequency–Inverse Document Frequency) for classifying text based on word occurrence. While effective to a degree, TF-IDF lacks semantic understanding.

In this version, we incorporate **word embeddings** and **transformer-based sentence embeddings** to better capture the meaning of text.

---

## 🚀 What's Inside

### 1. **Word Vectorization with GloVe**
We use the `"glove-twitter-200"` pretrained word embeddings to create dense vector representations of each word. These vectors are averaged across a sentence to classify sentiment more meaningfully than TF-IDF.

### 2. **Sentence Vectorization with BERT**
We leverage BERT (Bidirectional Encoder Representations from Transformers) using the `bert-base-uncased` model to extract sentence-level context. This allows for more nuanced understanding of syntax and semantics.

---

## 📂 Dataset Used

- **Sentiment140**: A large-scale dataset containing 1.6 million tweets labeled as positive or negative. This dataset was used to train and evaluate both models.

---

## 🛠️ Technologies Used

- Python
- Scikit-learn
- PyTorch
- HuggingFace Transformers
- GloVe word embeddings (`glove-twitter-200`)
- BERT (`bert-base-uncased`)

---

## 📊 Model Comparison

| Model             | Vectorization | Approach          | Result |
|------------------|---------------|-------------------|--------|
| TF-IDF (v1)       | Word-based    | Statistical count | ✅ Basic |
| GloVe (v2)        | Word-based    | Semantic embedding| ✅ Better |
| BERT (v3)         | Sentence-based| Transformer-based | ✅✅ Best |
