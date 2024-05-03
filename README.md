**Lab Report: Rule-Based NLP and Regex for Bill Generation**

**Objective:**
The main aim of this lab was to gain proficiency in Rule-Based Natural Language Processing (NLP) and Regular Expressions (Regex), fundamental techniques in the field of Natural Language Processing. The lab also provided an introduction to Word Embeddings, another essential concept in NLP.

**Work Done:**

**Part 1: Rule-Based NLP and Regex:**
In this section of the lab, we focused on implementing a Python program using Regex to generate a bill from a given text input provided by the user. The objective was to extract relevant information such as product names, quantities, and prices from the input text using Regex patterns.

**Use Case:**
For the practical exercise, we were given a sample text input: "I bought three Samsung smartphones 150 $ each, four kilos of fresh banana for 1,2 dollar a kilogram, and one Hamburger with 4,5 dollar." Our task was to develop a Python script that could parse this text and generate a bill with the following details:

**Generated Bill:**
- Product             Quantity    UnitPrice    TotalPrice
- Samsung smartphones   3           150          450
- banana                4           1.2          4.8
- Hamburger             1           4.5          4.5

**Challenges Faced:**
- Identifying and constructing appropriate Regex patterns to accurately extract product information from the text.
- Handling variations in numeric representations (e.g., numbers written out as words or containing commas for thousands separators).
- Ensuring robustness of the script to handle different formats and structures of input text.

**Part 2: Word Embedding**

#### Work Completed:
1. **Data Preparation:**
    - Retrieved text data from a MongoDB collection named 'NLP'.
    - Preprocessed the text data by tokenizing it into words.

2. **Encoding and Vectorization:**
    - Applied the following techniques on the tokenized data:
        - One-hot encoding
        - Bag of words
        - TF-IDF
    - Used libraries such as Scikit-learn for encoding and vectorization.

3. **Word Embedding Models:**
    - Implemented Word2Vec models (Skip Gram and CBOW) using Gensim.
    - Utilized GloVe and FastText models for word embedding.
    - Trained the models on the tokenized data to generate word vectors.

4. **Vector Visualization:**
    - Applied the t-SNE algorithm to reduce the dimensionality of the vectors.
    - Plotted the encoded/vectorized vectors in 3D space for visualization.

#### Results and Conclusion:
- **One-Hot Encoding, Bag of Words, and TF-IDF:**
    - These traditional techniques are effective for representing text data but may result in high-dimensional sparse vectors.

- **Word2Vec (Skip Gram and CBOW):**
    - Word2Vec models capture semantic relationships between words and generate dense word embeddings.
    - Skip Gram and CBOW models have their respective strengths, with Skip Gram being better suited for larger datasets.

- **GloVe and FastText:**
    - GloVe and FastText models offer alternative approaches to word embedding, incorporating additional contextual information.
    - GloVe focuses on global word co-occurrence statistics, while FastText utilizes subword information.

- **Vector Visualization:**
    - The t-SNE plots provide insights into the distribution of word vectors in a lower-dimensional space.
    - Different encoding/vectorization techniques and word embedding models result in distinct clustering patterns.

**Conclusion:**
The lab provided valuable hands-on experience in applying Rule-Based NLP techniques and Regex for information extraction tasks. By completing this exercise, we gained a deeper understanding of how to leverage Regex patterns to parse and extract structured data from unstructured text, a skill that is essential in many NLP applications, not only that  . Overall, the lab successfully achieved its objective of familiarizing us with Rule-Based NLP and Regex concepts in a practical context.

**Skills Learned:**: RegEx , Word Embedding , Skip Gram , One Hot Encoding , Word2Vec , TF-IDF  , FastText , ... etc.
