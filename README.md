# Q&A RAG System - Notebook Overview

This repository contains a Jupyter notebook that demonstrates the steps involved in setting up a Retrieval-Augmented Generation (RAG) system using vector embeddings and a Faiss vector database.

## Overview

The notebook guides you through the following key steps:

1. **Environment Setup**:
    - Installation of essential Python libraries such as `faiss-gpu`, `sentence-transformers`, `gradio`, and `langchain` components.
    - These libraries are crucial for creating embeddings, handling vectors, and interacting with the RAG system.

2. **Reading and Preparing Data**:
    - The data is read as a list of lists, which is the format required for generating embeddings.
    - This section ensures that your data is structured correctly for subsequent processing.

3. **Generating Embeddings**:
    - Embeddings are generated using the `paraphrase-multilingual-mpnet-base-v2` model from the `sentence-transformers` library.
    - These embeddings capture the semantic meaning of the input text, allowing for effective retrieval of similar content.

4. **Preprocessing for Faiss**:
    - Before indexing the data in the Faiss vector database, necessary preprocessing steps are carried out.
    - This step may include normalization, vectorization, or other transformations to optimize the data for indexing.

5. **Indexing in Faiss**:
    - The embeddings are stored in a Faiss vector database, which allows for fast and efficient retrieval.
    - The index is saved for future use, enabling quick loading without the need to regenerate embeddings.

6. **Loading the Index**:
    - The notebook provides steps to load the saved index, facilitating retrieval operations.
    - This feature is particularly useful for deploying the system in production environments where quick access to the index is essential.



## Dependencies

- `faiss-gpu`
- `sentence-transformers`
- `gradio`
- `langchain_google_genai`
- `langchain`
- `langchain_community`
- `langchain_anthropic`


