# QnA-ChatBot
# Question Answering with RAG-Fusion and Groq LLM from a pdf

This repository demonstrates a **Retrieval-Augmented Generation (RAG)** pipeline for question answering on a PDF document about Economics, combining **Groq LLM** for query generation and final answers with **Cohere Reranker** for improved document ranking. The pipeline is evaluated using **RAGAS metrics**.

---

## Features

- Load and process PDF documents using `PyPDFLoader`.
- Chunk documents for efficient retrieval.
- Generate multiple search queries per user query using **Groq LLM**.
- Retrieve documents using **FAISS vector store**.
- Re-rank retrieved documents using **Cohere Reranker**.
- Perform final QA using **Groq-powered RetrievalQA**.
- Evaluate pipeline performance using **context precision** and **context recall** metrics from **RAGAS**.

---

## Requirements

- Python 3.10+
- `langchain`, `ragas`, `datasets`, `faiss`, `huggingface_hub`, `langchain_groq`, `langchain_cohere`
- API keys:
  - **Cohere API Key** (used for reranking)
- Optional: GPU for faster LLM inference

---

## 📝 Installation

```bash
pip install datasets ragas langchain langchain_groq langchain_cohere langchain_community faiss-cpu
