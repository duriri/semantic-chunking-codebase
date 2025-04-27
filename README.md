# Duriri - Semantic Chunking in RAG

This repository demonstrates the use of **semantic chunking** in the context of **Retrieval-Augmented Generation (RAG)**. The goal is to improve the quality of retrieval and generation tasks by chunking information based on **meaning** and **context** rather than arbitrary sizes. This enhances the relevance and coherence of the information retrieved, especially in tasks like question-answering, summarization, and document retrieval.

## 🔍 What is Semantic Chunking?

**Semantic chunking** involves dividing content into meaningful units (chunks) based on their semantic or contextual relevance, rather than simply splitting them by size (like token count). In the RAG pipeline, this improves:

- More accurate retrieval of context-relevant documents
- Better performance in question-answering and summarization tasks
- Easier debugging, readability, and module reuse

## 🧠 Why Use Semantic Chunking in RAG?

Traditional RAG systems often split documents into equal-sized chunks, which can result in lost context (e.g., breaking up a paragraph or idea into smaller chunks). By using **semantic chunking**, the context is preserved, leading to:

- **Long document Q&A:** Ensuring full context is available for accurate answers.
- **Context-aware generation:** Retaining relevant context during generation tasks.
- **Legal, technical, or educational content retrieval:** Maintaining critical meaning in specialized content.

## 🧩 Key Components of This Repository

- **`cluster_semantic_chunker.py`**: Implementation of semantic chunking using clustering techniques to divide documents into meaningful chunks.
- **`kamradt_modified_chunker.py`**: A modified chunker for more specific use cases, adjusting semantic chunking techniques.
- **`semantic_chunking_clustring_HDBSCAN.ipynb`**: A Jupyter notebook demonstrating semantic chunking using **HDBSCAN** (Hierarchical Density-Based Spatial Clustering of Applications with Noise).
- **`semantic_chunking_clustring_kmeans.ipynb`**: A Jupyter notebook demonstrating semantic chunking using **KMeans clustering**.
- **`SemanticSplitGenerator`**: Embedding-based dynamic chunking using cosine similarity and adaptive breakpoints. Ideal for:- Sentence-level semantic boundaries- Configurable length/similarity thresholds - Built-in summarization support.
  
