# 🧠 LangChain Experiments & Tutorials

![LangChain](https://img.shields.io/badge/LangChain-Framework-green)
![Notebooks](https://img.shields.io/badge/Format-Colab_Notebooks-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Python](https://img.shields.io/badge/Python-3.8+-blue)

A comprehensive collection of **hands-on Colab-style notebooks** for practical implementations and benchmarking of core LangChain components. Master the entire LLM application stack—from document processing to embeddings, vector stores, retrievers, and complete RAG pipelines through structured, modular learning.

## 🎯 What You'll Learn

This repository provides a systematic journey through the LangChain ecosystem, with each component carefully isolated to enable:

- **🎓 Focused Learning** - Master individual components without complexity
- **⚡ Performance Benchmarking** - Compare implementations with real metrics
- **🔧 Production-Ready Solutions** - Plug-and-play components for your applications
- **📊 Visual Analytics** - Interactive metrics and performance comparisons

## 📁 Repository Structure

```
LangChain-Playlist/
├── 📄 Loader and Splitters/
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
│   ├── PPT Based/
│   │   └── UnstructuredPowerPointLoader_with_CharacterTextSplitter.ipynb
│   ├── JSON Based/
│   │   └── JSONLoader_with_RecursiveJsonSplitter.ipynb
│   ├── HTML_URL Based/
│   │   ├── BSHTMLLoaderWithHTMLHeaderTextSplitter.ipynb
│   │   └── UnstructuredHTMLLoaderWithRecursiveCharacterTextSplitter.ipynb
│   └── Markdown_Based/
│       └── UnstructuredMarkdownLoader_with_MarkdownHeaderTextSplitter.ipynb
│
├── 🧬 Embedding Models/
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
│   └── RERANKER Models/
│       ├── ms-marco-MiniLM-L-6-v2.ipynb
│       ├── ms-marco-MiniLM-L-12-v2.ipynb
│       ├── tomaarsen-ModernBERT-base-gooaq-bce.ipynb
│       ├── quora-distilroberta-base.ipynb
│       ├── stsb-roberta-large.ipynb
│       └── qnli-electra-base.ipynb
│
├── 🧲 VectorDB's/
│   ├── FAISS.ipynb
│   ├── ChromaDB.ipynb
│   ├── Weaviate.ipynb
│   ├── Qdrant.ipynb
│   ├── Pinecone.ipynb
│   └── Redis.ipynb
│
├── 📝 PromptsTemplates/
│   ├── PromptTemplateExample.ipynb
│   ├── ChatPromptTemplateExample.ipynb
│   ├── ChatMessagePromptTemplateExample.ipynb
│   ├── ImagePromptTemplateExample.ipynb
│   └── PipelinePromptTemplateExample.ipynb
│
├── 🔍 Retrievers/
│   ├── VectorStoreRetrieverMMR-InsideRAG.ipynb
│   ├── ParentDocumentRetriever-InsideRAG.ipynb
│   └── MultiVectorRetriever-InsideRAG.ipynb
│
├── 🔗 Chains/
│   └── [Coming Soon]
│
├── 🛠️ Tools/
│   ├── Tavily_Search_Extract_Tool.ipynb
│   ├── JSON_AgentToolkit_Tool.ipynb
│   ├── YahooFinanceNews_Stock_Tools.ipynb
│   ├── QuipDocumentGenerator_Tool.ipynb
│   ├── NutritionAI_CustomNutritionAI_Tool.ipynb
│   └── CustomEmailOperations_Tool.ipynb
│
└── 🤖 LLMs/
    └── [Coming Soon]
```

## 🔍 Available Components

### 📄 Document Loaders & Text Splitters

Transform diverse document formats into LLM-ready chunks with specialized loaders and intelligent splitting strategies.

#### PDF Processing Pipeline

| **Loader + Splitter** | **Key Features** | **Best For** |
|------------------------|------------------|--------------|
| **PyPDFLoader + SemanticChunker** | • Semantic coherence scoring<br>• Context-aware boundaries<br>• Token optimization | Research papers, long-form content |
| **UnstructuredPDFLoader + RecursiveCharacterTextSplitter** | • Advanced structure detection<br>• Memory-efficient processing<br>• Content preservation | Complex layouts, mixed content |
| **PyMuPDFLoader + RecursiveCharacterTextSplitter** | • Enhanced PDF parsing<br>• Metadata extraction<br>• Performance benchmarks | High-volume PDF processing |

#### Specialized Document Formats

| **Document Type** | **Implementation** | **Capabilities** |
|-------------------|-------------------|------------------|
| **📄 Text Files** | TextLoader + SemanticChunker | Plain text processing, narrative boundaries |
| **📊 Excel Files** | UnstructuredExcelLoader + CharacterTextSplitter | Multi-sheet processing, tabular data extraction |
| **📝 Word Documents** | UnstructuredWordDocumentLoader + RecursiveCharacterTextSplitter | Rich formatting, embedded content handling |
| **🎯 PowerPoint** | UnstructuredPowerPointLoader + CharacterTextSplitter | Slide extraction, speaker notes processing |
| **🔧 JSON Data** | JSONLoader + RecursiveJsonSplitter | Schema-aware splitting, hierarchical preservation |
| **🌐 HTML/Web** | BSHTMLLoader / UnstructuredHTMLLoader | Web scraping, content-focused extraction |
| **📋 Markdown** | UnstructuredMarkdownLoader + MarkdownHeaderTextSplitter | Structure-preserving, header-based chunking |

### 🧬 Embedding Models

**Base Embedding Models** - Comprehensive performance analysis across leading embedding architectures:

| **Model Family** | **Variants** | **Strengths** |
|------------------|--------------|---------------|
| **MiniLM** | L6-v2, L12-v2 | Fast inference, balanced performance |
| **MPNet** | all-mpnet-base-v2, multi-qa-mpnet-base-dot-v1 | Superior semantic understanding |
| **Multilingual** | gte-multilingual-base | Cross-language retrieval |
| **Commercial** | OpenAI text-embedding-3-large, Cohere v3.0 | State-of-the-art accuracy |
| **Specialized** | GIST-Embedding-v0, msmarco-distilbert-cos-v5 | Domain-specific optimization |

**Reranker Models** - Boost retrieval precision with advanced reranking:

| **Model** | **Architecture** | **Use Case** |
|-----------|------------------|--------------|
| **ms-marco-MiniLM-L-6-v2** | Lightweight transformer | Production environments, speed-critical |
| **ms-marco-MiniLM-L-12-v2** | Enhanced transformer | Balanced accuracy-speed tradeoff |
| **ModernBERT-base-gooaq-bce** | Modern BERT + BCE | Maximum accuracy, research applications |
| **🆕 quora-distilroberta-base** | DistilRoBERTa architecture | Question similarity, community Q&A |
| **🆕 stsb-roberta-large** | Large RoBERTa model | Semantic textual similarity tasks |
| **🆕 qnli-electra-base** | ELECTRA-based model | Natural language inference, Q&A |

### 🧲 Vector Databases

Production-ready integrations with leading vector storage solutions:

<div align="center">

| **FAISS** | **ChromaDB** | **Weaviate** |
|-----------|--------------|--------------|
| **Meta's similarity search** | **Local-first vector DB** | **Production vector DB** |
| High-performance indexing | Simple setup & deployment | GraphQL API, cloud-ready |

| **Qdrant** | **Pinecone** | **Redis** |
|------------|--------------|-----------|
| **Open-source vector DB** | **Managed vector service** | **In-memory vector search** |
| Self-hosted flexibility | Serverless scaling | Ultra-low latency |

</div>

### 🔍 Retrievers

Advanced retrieval strategies for sophisticated RAG implementations with comprehensive end-to-end examples:

| **Retriever Type** | **Implementation** | **Key Features** | **Best For** |
|-------------------|-------------------|------------------|--------------|
| **VectorStoreRetrieverMMR** | Maximum Marginal Relevance in RAG | • Diversity optimization<br>• Relevance-diversity balance<br>• Complete RAG pipeline integration | Avoiding redundant results, diverse content retrieval |
| **ParentDocumentRetriever** | Hierarchical document retrieval in RAG | • Parent-child document relationships<br>• Context preservation<br>• Full RAG workflow demonstration | Long documents, maintaining context while chunking |
| **MultiVectorRetriever** | Multiple vector representation in RAG | • Multiple embedding strategies<br>• Enhanced retrieval accuracy<br>• End-to-end RAG implementation | Complex documents, multi-aspect retrieval |

Each retriever notebook includes:
- **🔄 Complete RAG Pipeline** - From document loading to final answer generation
- **📊 Performance Metrics** - Retrieval quality and response evaluation
- **⚙️ Configurable Parameters** - Fine-tune retrieval strategies
- **🎯 Real-world Examples** - Practical use cases and implementations
- **📈 Comparative Analysis** - Benchmarking against baseline retrievers

### 📝 Prompt Templates

Master prompt engineering with comprehensive templating solutions:

| **Template Type** | **Purpose** | **Key Features** |
|-------------------|-------------|------------------|
| **PromptTemplate** | Basic text prompts | Variable substitution, input validation |
| **ChatPromptTemplate** | Conversation handling | Multi-turn context, role management |
| **ChatMessagePromptTemplate** | Individual messages | Role-based formatting, dynamic composition |
| **🆕 ImagePromptTemplate** | Vision model prompts | Image + text prompting, multimodal workflows |
| **🆕 PipelinePromptTemplate** | Complex prompt chains | Multi-stage processing, prompt composition |

### 🛠️ LangChain Tools

Extend LLM capabilities with powerful external integrations:

#### Search & Information Tools
| **Tool** | **Functionality** | **Use Cases** |
|----------|-------------------|---------------|
| **Tavily Search & Extract** | Real-time web search + content extraction | Research automation, fact-checking |

#### Data Processing Tools
| **Tool** | **Functionality** | **Use Cases** |
|----------|-------------------|---------------|
| **JSON AgentToolkit** | JSON manipulation & querying | API integration, data transformation |
| **🆕 QuipDocumentGenerator** | Automated document creation | Report generation, content workflows |

#### Financial & Market Tools
| **Tool** | **Functionality** | **Use Cases** |
|----------|-------------------|---------------|
| **Yahoo Finance News & Stock** | Market data & financial news | Investment research, market analysis |

#### Specialized AI Tools
| **Tool** | **Functionality** | **Use Cases** |
|----------|-------------------|---------------|
| **🆕 NutritionAI & CustomNutritionAI** | Nutritional analysis & recommendations | Health apps, dietary planning |
| **🆕 CustomEmailOperations** | Email automation & processing | Communication workflows, CRM integration |

## 🚀 Getting Started

### Prerequisites
```bash
pip install langchain langchain-community langchain-openai
pip install faiss-cpu chromadb sentence-transformers
```

### Quick Start
1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/LangChain-Playlist.git
   cd LangChain-Playlist
   ```

2. **Open any notebook in Google Colab**
   - Each notebook contains installation commands
   - All examples are self-contained
   - Interactive parameters for experimentation

3. **Start with the basics**
   - Begin with `Loader and Splitters/` for document processing
   - Move to `Embedding Models/` for vector representations
   - Progress to `VectorDB's/` for storage solutions
   - Explore `Retrievers/` for advanced retrieval strategies

## 📊 Notebook Features

Each notebook includes:

- **🎯 Clear Learning Objectives** - What you'll accomplish
- **📚 Concept Explanations** - Theory behind implementations  
- **⚙️ Interactive Parameters** - Modify and experiment easily
- **📈 Performance Metrics** - Visual comparisons and benchmarks
- **🔍 Troubleshooting Guides** - Common issues and solutions
- **💡 Best Practices** - Production deployment tips

## 🔄 Upcoming Features

| **Category** | **Components** | **ETA** |
|--------------|----------------|---------|
| **🤖 LLM Integration** | GPT-4, Claude, Llama, Gemini implementations | Q2 2024 |
| **🧪 Advanced RAG Pipelines** | Multi-agent RAG, conditional retrieval, hybrid approaches | Q3 2024 |
| **📊 Benchmarking Suite** | Automated performance testing & comparison | Q3 2024 |
| **🔧 Agent Frameworks** | Multi-agent systems, tool routing | Q4 2024 |

## 🤝 Contributing

We welcome contributions from the community!

### Ways to Contribute
- **⭐ Star this repository** to show support
- **🐛 Report bugs** or request clarifications
- **💡 Suggest new components** or improvements
- **📝 Submit pull requests** with new implementations
- **📚 Improve documentation** and examples

### Contribution Guidelines
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Follow the existing notebook structure and naming conventions
4. Include comprehensive documentation and examples
5. Test your implementation thoroughly
6. Submit a pull request with detailed description

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **LangChain Team** for the incredible framework
- **Open Source Community** for embedding models and vector databases
- **Contributors** who help improve this resource

## 📞 Support

- **📖 Documentation**: Check individual notebook READMEs
- **💬 Discussions**: Use GitHub Discussions for questions
- **🐛 Issues**: Report bugs via GitHub Issues
- **📧 Contact**: Open an issue for direct communication

---

<div align="center">
  
**⚡ Ready to master LangChain? Start with any notebook and build your LLM expertise step by step! ⚡**

*Built with ❤️ for the LangChain community*

[![GitHub stars](https://img.shields.io/github/stars/dhruvsh1997/LangchainExperiments?style=social)](https://github.com/dhruvsh1997/LangchainExperiments)
[![GitHub forks](https://img.shields.io/github/forks/dhruvsh1997/LangchainExperiments?style=social)](https://github.com/dhruvsh1997/LangchainExperiments)

</div>