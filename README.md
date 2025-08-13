# llm-rag-demo
A demonstration project showing how to build a Retrieval-Augmented Generation (RAG) system using a Large Language Model (LLM) with PDF documents. This project uses LangChain, HuggingFace embeddings, and Qdrant to create a vector database for context-aware question answering.
## Overview
This project demonstrates the difference between using a **plain LLM** and a **Retrieval-Augmented Generation (RAG) pipeline** with a vector database. The use case is answering questions about the FIFA Club World Cup 2025 using PDF documents as the knowledge source.  

The workflow:
1. Load PDF documents containing tournament information.
2. Split documents into chunks.
3. Generate embeddings for each chunk.
4. Store embeddings in a Qdrant vector database.
5. Retrieve the most relevant chunks for a user question.
6. Use an LLM to answer the question using retrieved context.

---

## Features
- Compare plain LLM answers vs RAG-enhanced answers.
- Uses HuggingFace embeddings for vector representation.
- Uses Qdrant Cloud as the vector database.
- Supports multiple PDF files as the knowledge base.
- Interactive in Google Colab.

---

## Requirements
- Python 3.8+
- Google Colab (recommended)
- Packages:
  ```bash
  !pip install -U langchain langchain-openai langchain-community qdrant-client pypdf openai
