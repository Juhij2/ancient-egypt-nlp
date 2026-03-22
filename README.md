# NLP on Ancient Egyptian Texts

This project applies modern Natural Language Processing (NLP) techniques to English translations of ancient Egyptian texts. The goal is to explore thematic structure within funerary texts and compare funerary writing with mythic narrative texts.

## Project Overview

The project is divided into four main parts:

### 1. Topic Modeling (LDA)
- Applied TF-IDF and Latent Dirichlet Allocation (LDA)
- Identified recurring themes in *Book of the Dead* chapters:
  - Solar praise and hymnic language
  - Judgment and the weighing of the heart
  - Underworld passages and Osirian material

### 2. Embedding-Based Analysis
- Used sentence-transformer embeddings (MiniLM)
- Compared chapters using cosine similarity
- Performed clustering (KMeans)
- Visualized structure using PCA and UMAP
- Built a semantic search system

### 3. Genre Classification (Funerary vs Mythic)
- Combined funerary and mythic Egyptian texts
- Generated embeddings for all documents
- Trained classifiers:
  - Logistic Regression
  - Linear SVM
- Achieved **93.75% cross-validation accuracy**

### 4. Neural Network Classifier
- Built a small feed-forward neural network (PyTorch)
- Trained using backpropagation
- Achieved strong performance on a held-out test set
- Compared performance with linear models

## Key Findings

- Topic modeling reveals meaningful thematic structure in funerary texts
- Sentence embeddings capture semantic relationships between chapters
- Funerary and mythic texts separate clearly in embedding space
- Simple linear models perform very well on genre classification
- Neural networks can learn the distinction, but small dataset limits conclusions

## Limitations

- The analysis is performed on English translations, not original ancient Egyptian language
- The dataset is small (16 documents), so results should be interpreted cautiously

## Technologies Used

- Python
- pandas, numpy
- scikit-learn
- nltk
- sentence-transformers
- PyTorch
- matplotlib
- umap-learn
