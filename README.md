# **NLP Basics and Text Vectorization Techniques**

This repository provides a comprehensive overview of **Natural Language Processing (NLP)** basics, including text preprocessing, vectorization techniques, and foundational terminology. It also outlines key differences between Stemming and Lemmatization and discusses advanced concepts like semantic representations and the progression of NLP techniques.

---

## **Contents**

### **1. Text Preprocessing**
Text preprocessing is the foundation of NLP tasks, helping convert raw text into a format suitable for analysis and modeling.

- **Tokenization**: Splitting text into smaller units like words or sentences.
- **Stop Words Removal**: Removing common words that add little meaning, such as "is," "the," "and."
- **Stemming**: Reducing words to their base or root form (e.g., "running" → "run").
  - **Advantages**:
    - Faster and computationally efficient.
    - Useful for filtering and quick tasks.
  - **Disadvantages**:
    - Does not produce meaningful words (e.g., "caring" → "car").
- **Lemmatization**: Reducing words to their dictionary form (e.g., "running" → "run").
  - **Advantages**:
    - Retains the meaning of words.
    - Suitable for tasks like chatbots, language translation, and summarization.
  - **Disadvantages**:
    - Computationally expensive compared to stemming.

---

### **2. Vectorization Techniques**
Text vectorization converts text data into numerical representations for machine learning models. Below are the primary methods:

#### **One Hot Encoding (OHE)**
- Represents text data as binary vectors based on unique words.
- **Example**:  
  Sentences:  
  - "A man eats food."  
  - "Cat eats food."  
  Vocabulary: `[a, man, eats, food, cat]`  
  OHE for "A man eats food":  
  `[1, 1, 1, 1, 0]`

- **Advantages**:
  - Simple and intuitive.
  - Easy to implement.
- **Disadvantages**:
  - Creates sparse matrices.
  - Out-of-Vocabulary (OOV) issues.
  - Fails to capture semantic meaning or word order.

---

#### **Bag of Words (BoW)**
- Represents documents as word frequency vectors.
- **Steps**:
  1. Remove stopwords.
  2. Count word frequencies.
  3. Create a matrix for word occurrences across documents.

- **Example**:  
  Sentences:  
  - D1: "Good boy."  
  - D2: "Good girl."  
  Vocabulary: `[good, boy, girl]`
### Matrix Representation

| Document | Good | Boy | Girl |
|----------|------|-----|------|
| D1       | 1    | 1   | 0    |
| D2       | 1    | 0   | 1    |

- **Advantages**:
- Simple and effective for small datasets.
- **Disadvantages**:
- Sparse matrices.
- Ignores word order and semantic meaning.

---

#### **TF-IDF (Term Frequency-Inverse Document Frequency)**
- Evaluates the importance of words in a document relative to the corpus.
- **Use Cases**: Text classification, sentiment analysis, and information retrieval.
- **Advantages**:
- Captures important words effectively.
- **Disadvantages**:
- Computationally expensive for large datasets.

---

### **3. Advanced Techniques**
#### **Word Embeddings**
- Techniques like Word2Vec, GloVe, and FastText capture semantic meanings and relationships between words.
- **Example**:  
Relationships like "king" → "queen" and "man" → "woman."

#### **N-Grams**
- Captures sequences of words (e.g., bigram: "good boy," trigram: "good boy eats").
- Helps retain word order and local context.

---

### **4. NLP Terminology**
- **Corpus**: A collection of text data (e.g., paragraphs, documents).
- **Documents**: Individual text entries in a corpus (e.g., sentences).
- **Vocabulary**: Unique words across the corpus.
- **Word**: Basic units of text processing.

---

### **5. Semantic Representation**
The progression of NLP techniques:

            Semantic Meaning
              (Advanced Models)
      ----------------------------------
      Word Embeddings (e.g., Word2Vec)
      ----------------------------------
      TF-IDF / Bag of Words
      ----------------------------------
      One Hot Encoding
      ----------------------------------
      Text Preprocessing

---

## **How to Use**
1. Clone the repository.
2. Use the notes for reference or as a learning guide.
3. Explore techniques in **Google Colab** or Jupyter Notebooks to apply these concepts.

---

## **Contributions**
We welcome contributions to enhance this repository:
1. Fork the repository.
2. Add new examples, explanations, or advanced techniques.
3. Submit a pull request for review.

---

## **Author**
👤 **Nevil Dhinoja**  
Interested in **NLP**, **Generative AI**, **Machine Learning**, and **Deep Learning**. Passionate about exploring the intersection of language and technology.  

---

Feel free to explore, share, and contribute! 🚀



