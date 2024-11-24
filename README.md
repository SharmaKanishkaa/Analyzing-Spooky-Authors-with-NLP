# Spooky NLP and Topic Modelling Tutorial 👻📚
---

## 📝 **Project Overview**
The main objective of this project is to apply topic modelling techniques to a dataset and extract meaningful insights. The **Spooky Author dataset** contains stories written by different authors, and our goal is to uncover the main topics present across all the stories.

---

## 🔍 **Outline of the Notebook**

### 1. **Exploratory Data Analysis (EDA) & Wordclouds**
   - We begin by analyzing the dataset to get a sense of the data structure and distribution.
   - We'll calculate **word frequencies** across different authors and visualize these using **word clouds** (including creative image masks).
   - This section helps us understand the most common terms and identify potential topics visually.

### 2. **Natural Language Processing (NLP) with NLTK**
   - **Tokenization**: Breaking the raw text into individual words or tokens.
   - **Stopword Removal**: Removing common words (like "and", "the", etc.) that don't contribute meaningful information.
   - **Stemming**: Reducing words to their root form (e.g., "running" to "run").
   - **Vectorization**: Converting text into numerical form using:
     - **Term Frequency (TF)**: The frequency of a word in a document.
     - **Inverse Document Frequency (TF-IDF)**: The importance of a word within the entire corpus, helping reduce the weight of common words.

### 3. **Topic Modelling with LDA and NMF**
   - **Latent Dirichlet Allocation (LDA)**: LDA is a popular algorithm for topic modelling, where it assumes each document is a mixture of topics, and each topic is a mixture of words. We'll use LDA to extract topics and their associated words.
   - **Non-negative Matrix Factorization (NMF)**: Another technique used for topic extraction. It factorizes the document-term matrix into two lower-dimensional matrices to discover latent topics within the text.

---

## 📊 **Key Steps in the Project**

### **Data Loading & Preprocessing**
- Load the dataset and clean the text by removing punctuation, special characters, and unnecessary spaces.
- Apply **tokenization**, remove **stopwords**, and **stem** the words to prepare them for modelling.

### **Wordcloud Generation**
- Generate word clouds for each author and the entire corpus to visually capture the most frequent words and the nature of the topics.

### **Topic Modelling with LDA & NMF**
- **LDA**:
  - We will use the LDA model to identify the most common topics in the dataset.
  - Visualize topics by showing the most frequent words associated with each topic.
  
- **NMF**:
  - Similarly, NMF will be applied to extract topics and visualize the words associated with each topic.
  
### **Evaluation**
- Evaluate and compare the results from both models (LDA vs NMF) to see which one provides more coherent and interpretable topics.

---

## 💡 **Key Concepts**
- **Topic Modelling**: A way of automatically identifying topics in large datasets of text.
- **NLP**: A branch of AI focused on enabling computers to understand and process human languages.
- **LDA**: A probabilistic model used to find topics in a set of documents.
- **NMF**: A matrix factorization method that works well for topic modelling.

---

## 📈 **Visualizations**
- **Wordclouds**: Represent word frequency visually, with larger words indicating higher frequency.
- **Topic Distribution**: Visualize the most common words for each extracted topic.

---

## 🚀 **Future Improvements**
- **Hyperparameter Tuning**: Experiment with different hyperparameters for LDA and NMF to improve topic coherence.
- **Advanced NLP Techniques**: Implement more advanced NLP methods such as **word embeddings** (e.g., Word2Vec) for deeper text understanding.
- **Deep Learning**: Explore deep learning-based topic modelling techniques like **BERT** for more accurate topic extraction.

---

## 🛠️ **Technologies Used**
- **Python**: Main programming language for data manipulation, analysis, and modelling.
- **NLTK**: Natural Language Toolkit for text preprocessing tasks.
- **scikit-learn**: For vectorization (TF-IDF) and implementing the NMF algorithm.
- **gensim**: For implementing the LDA model.
- **matplotlib & wordcloud**: For visualizations and wordcloud generation.
