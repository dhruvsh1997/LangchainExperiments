# 🧠 LangChain Tutorial Code Repository

Welcome to the official code repository for my **LangChain Playlist Series**!

This repository contains hands-on, modular notebooks designed to explore and demonstrate key components of the LangChain framework — from document loaders and splitters to embedding models, vector databases, and retrieval-augmented generation (RAG) workflows.

> 🔬 **This is a living repository** — content will continuously grow and evolve as we explore deeper concepts.

## 📁 Repository Structure

The repository is organized into the following folders:

| Folder Name | Description |
|-------------|-------------|
| `Loader and Splitters` | Notebooks demonstrating different document loaders and text splitters |
| `Embedding Models` | Guides and experiments using various embedding models (OpenAI, BGE, etc) |
| `VectorDBs` | Examples of working with FAISS, Chroma, Pinecone, and other vector stores |
| `RetrieverChains` | Implementing retrievers and chains for question answering and RAG |
| `Tools and LLMs` | Working with LangChain tools, agents, and large language models (LLMs) |

## 📘 Current Focus: `Loader and Splitters`

### ✅ Implemented:

This folder currently includes notebooks demonstrating and benchmarking the following loader + splitter combinations:

1. **PyPDFLoader + SemanticChunker**
   - Focused on semantic-aware chunking using sentence transformers
   - Performance metrics include token count, semantic flow, chunk variability, and structural preservation

2. **UnstructuredPDFLoader + RecursiveCharacterTextSplitter**
   - Heuristic-based PDF extraction with rule-based recursive text splitting
   - Benchmarked for content quality, chunk consistency, memory usage, and processing time

Each notebook includes:
- Full pipeline: Loading → Splitting → Metrics Evaluation
- Interpretive, Colab-ready structure
- Comments and explanations for educational clarity
- Loader & splitter performance comparisons

## 📺 YouTube Playlist

👉 [LangChain Playlist on YouTube](#) *(update this with your actual link)*

Follow along the series and clone this repo to run code alongside the tutorials.

## 💡 Contribution & Roadmap

While this repository is part of a tutorial series, I welcome:
- Suggestions on advanced loader/splitter pairings
- Requests for new model demos
- Pull requests once the structure matures

### 📅 Coming Soon:
- Embedding Model Comparisons
- FAISS & Chroma Indexing
- Retrieval Chains + Custom Prompting
- Agent Toolchains
- LangGraph workflows

## 🛠️ Setup Instructions

Ensure you have the right environment for running the notebooks:

```bash
pip install langchain langchain-community langchain-text-splitters sentence-transformers transformers unstructured psutil
```