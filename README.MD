# 🧠 LangChain Experiments & Tutorials

![LangChain](https://img.shields.io/badge/LangChain-Framework-green)
![Notebooks](https://img.shields.io/badge/Format-Colab_Notebooks-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

A comprehensive collections of **hands-on Colab-style notebooks** for practical implementations and benchmarking of core LangChain components. Step through the entire LLM application stack—from document processing to embeddings, vector stores, retrievers, and complete RAG pipelines.

## 🧩 Repository Overview

This repository provides a modular journey through the Langchain ecosystem, with each component carefully isolated to allow for:
- **Focused learning** of individual components
- **Comparative benchmarking** across implementation options
- **Plug-and-play solutions** for your LLM-powered applications

## 📁 Repository Structures

```
LangChain-Playlist/
├── Loader and Splitters/
│   ├── PDF Based/
│   │   ├── PyPDFLoader_with_SemanticChunker.ipynb
│   │   ├── UnstructuredPDFLoader_with_RecursiveCharacterTextSplitter.ipynb
│   │   └── PyMuPDFLoaderWithRecursiveCharacterTextSplitter.ipynb
│   ├── TextFile Based/
│   │   └── TextLoader_with_SemanticChunker.ipynb
│   ├── ExcelFile Based/
│   │   └── UnstructuredExcelLoader_with_CharacterTextSplitter.ipynb
│   ├── Document Based/
│   │   └── UnstructuredWordDocumentLoader_with_RecursiveCharacterTextSplitter.ipynb
│   ├── JSON Based/
│   │   └── JSONLoader_with_RecursiveJsonSplitter.ipynb
│   ├── HTML_URL Based/
│   │   ├── BSHTMLLoaderWithHTMLHeaderTextSplitter.ipynb
│   │   └── UnstructuredHTMLLoaderWithRecursiveCharacterTextSplitter.ipynb
│   └── Markdown_Based/
│       └── UnstructuredMarkdownLoader_with_MarkdownHeaderTextSplitter.ipynb
│
├── Embedding Models/
│   ├── BASE Embedding/
│   │   ├── all-MiniLM-L12-v2.ipynb
│   │   ├── all-MiniLM-L6-v2.ipynb
│   │   ├── gte-multilingual-base.ipynb
│   │   ├── OpenAIEmbedding-text_embedding_3_large.ipynb
│   │   ├── GIST-Embedding-v0.ipynb
│   │   ├── cohere_embed_english_v3_0.ipynb
│   │   ├── all-mpnet-base-v2.ipynb
│   │   ├── multi-qa-mpnet-base-dot-v1.ipynb
│   │   └── msmarco_distilbert_cos_v5.ipynb
│   └── ReRanking Embedding/
│       └── [Coming Soon]
│
├── VectorDB's/
│   ├── FAISS.ipynb
│   ├── ChromaDB.ipynb
│   ├── Weaviate.ipynb
│   ├── Qdrant.ipynb
│   ├── Pinecone.ipynb
│   └── Redis.ipynb
│
├── Chains/
│   └── [Coming Soon]
│
├── Tools/
│   └── [Coming Soon]
│
├── LLMs/
│   └── [Coming Soon]
```

## 🔍 Currently Available Components

### 📄 Document Loaders & Splitters

Organized by document types with specialized loaders and splitters:

#### PDF Based Documents

<table>
  <tr>
    <td width="33%">
      <b>PyPDFLoader + SemanticChunker</b><br>
      <ul>
        <li>Semantic flow scoring</li>
        <li>Chunk coherence metrics</li>
        <li>Token cost efficiency</li>
      </ul>
    </td>
    <td width="33%">
      <b>UnstructuredPDFLoader + RecursiveCharacterTextSplitter</b><br>
      <ul>
        <li>Rule-based chunking efficiency</li>
        <li>Memory utilization analysis</li>
        <li>Content structure preservation</li>
      </ul>
    </td>
    <td width="33%">
      <b>PyMuPDFLoader + RecursiveCharacterTextSplitter</b><br>
      <ul>
        <li>Enhanced PDF parsing</li>
        <li>Structure-aware chunking</li>
        <li>Performance benchmark comparison</li>
      </ul>
    </td>
  </tr>
</table>

#### TextFile Based Documents

<table>
  <tr>
    <td>
      <b>TextLoader + SemanticChunker</b><br>
      <ul>
        <li>Plain text document processing</li>
        <li>Semantic boundary detection</li>
        <li>Context-aware chunking for .txt files</li>
        <li>Optimized for narrative and unstructured text</li>
      </ul>
    </td>
  </tr>
</table>

#### ExcelFile Based Documents

<table>
  <tr>
    <td>
      <b>UnstructuredExcelLoader + CharacterTextSplitter</b><br>
      <ul>
        <li>Excel spreadsheet data extraction (.xlsx, .xls)</li>
        <li>Cell-based content processing</li>
        <li>Character-level text splitting for tabular data</li>
        <li>Handles multiple sheets and structured data formats</li>
      </ul>
    </td>
  </tr>
</table>

#### Document Based Documents

<table>
  <tr>
    <td>
      <b>UnstructuredWordDocumentLoader + RecursiveCharacterTextSplitter</b><br>
      <ul>
        <li>Microsoft Word document processing (.docx, .doc)</li>
        <li>Rich text formatting preservation</li>
        <li>Recursive chunking for complex document structures</li>
        <li>Handles headers, tables, and embedded content</li>
      </ul>
    </td>
  </tr>
</table>

#### JSON Based Documents

<table>
  <tr>
    <td>
      <b>JSONLoader + RecursiveJsonSplitter</b><br>
      <ul>
        <li>JSON data structure processing</li>
        <li>Nested object and array handling</li>
        <li>Schema-aware recursive splitting</li>
        <li>Preserves hierarchical relationships in data</li>
      </ul>
    </td>
  </tr>
</table>

#### HTML/URL Based Documents

<table>
  <tr>
    <td width="50%">
      <b>BSHTMLLoader + HTMLHeaderTextSplitter</b><br>
      <ul>
        <li>Web content extraction</li>
        <li>Header-based document structuring</li>
        <li>HTML-specific chunking strategies</li>
      </ul>
    </td>
    <td width="50%">
      <b>UnstructuredHTMLLoader + RecursiveCharacterTextSplitter</b><br>
      <ul>
        <li>Comprehensive HTML parsing</li>
        <li>Content-focused extraction</li>
        <li>Character-based recursive splitting</li>
      </ul>
    </td>
  </tr>
</table>

#### Markdown Based Documents

<table>
  <tr>
    <td>
      <b>UnstructuredMarkdownLoader + MarkdownHeaderTextSplitter</b><br>
      <ul>
        <li>Markdown document processing</li>
        <li>Header-based hierarchical splitting</li>
        <li>Structure-preserving chunking</li>
      </ul>
    </td>
  </tr>
</table>

### 🧬 Embedding Models

Base embedding model implementations with performance comparisons:

<table>
  <tr>
    <td><b>all-MiniLM-L6-v2</b></td>
    <td><b>all-MiniLM-L12-v2</b></td>
    <td><b>gte-multilingual-base</b></td>
  </tr>
  <tr>
    <td><b>OpenAI text-embedding-3-large</b></td>
    <td><b>GIST-Embedding-v0</b></td>
    <td><b>cohere_embed_english_v3_0</b></td>
  </tr>
  <tr>
    <td><b>all-mpnet-base-v2</b></td>
    <td><b>multi-qa-mpnet-base-dot-v1</b></td>
    <td><b>msmarco_distilbert_cos_v5</b></td>
  </tr>
</table>

### 🧲 Vector Databases

Practical integration examples across multiple vector stores:

<div align="center">
  <b>FAISS</b> • <b>ChromaDB</b> • <b>Weaviate</b> • <b>Qdrant</b> • <b>Pinecone</b> • <b>Redis</b>
</div>

## 🚧 Coming Soon

<table>
  <tr>
    <td><b>🔍 Retriever Chains</b><br>Multi-vector and hybrid retrievers</td>
    <td><b>⚙️ LangChain Tools</b><br>Calculator, SerpAPI, etc.</td>
  </tr>
  <tr>
    <td><b>🧠 LLMs</b><br>GPT-4, Claude, open-source LLMs</td>
    <td><b>🧪 RAG Pipelines</b><br>Complete retrieval-augmented generation workflows</td>
  </tr>
  <tr>
    <td colspan="2"><b>🧑‍🔬 Benchmarking Tools</b><br>Embedding effectiveness, latency, chunk impact analysis</td>
  </tr>
</table>

## 💻 How to Use

Each notebook follows a **Colab-friendly format** with:

1. **Clear explanations** of concepts and implementation details
2. **Interactive parameters** you can modify to test different configurations
3. **Visual metrics** and performance comparisons
4. **Self-contained examples** that work with minimal setup

> Perfect for researchers, engineers, and students exploring LLM applications with LangChain.

## 🤝 Contribute

Contributions are welcome in many forms:

- ⭐ Star this repo to show support
- 🐛 Open issues for bugs or clarifications
- 💡 Suggest improvements or new component
- 🧪 Submit PRs for new implementations

## 📜 License

This repository is licensed under the **MIT License**.

---

<div align="center">
  <i>Built with ❤️ for the LangChain community</i>
</div>