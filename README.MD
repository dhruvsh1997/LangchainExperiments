# 🧠 LangChain Experiments & Tutorials

![LangChain](https://img.shields.io/badge/LangChain-Framework-green)
![Notebooks](https://img.shields.io/badge/Format-Colab_Notebooks-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Python](https://img.shields.io/badge/Python-3.8+-blue)

A comprehensive collection of **hands-on Colab-style notebooks** for practical implementation and benchmarking of core LangChain components. Master the entire LLM application stack—from document processing to embeddings, vector stores, retrievers, and complete RAG pipelines through structured, modular learning.

## 🎯 What You'll Learn

This repository provides a systematic journey through the LangChain ecosystem, with each component carefully isolated to enable, Segmented Ratio Might be neede, Ragaas can be performed:

- **🎓 Focused Learning** - Master individual components without complexity
- **⚡ Performance Benchmarking** - Compare implementations with real metrics
- **🔧 Production-Ready Solutions** - Plug-and-play components for your applications
- **📊 Visual Analytics** - Interactive metrics and performance comparisons

## 📁 Repository Structures

```
LangChain-Playlist/
├── 📄 Loaders and Splitters/
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
├── 🔧 Output Parsers/
│   ├── OutputParser_StrOutputParser.ipynb
│   ├── OutputParser_JSONOutputParser.ipynb
│   ├── OutputParser_XMLOutputParser.ipynb
│   ├── OutputParser_PydanticOutputParser.ipynb
│   └── OutputParser_StructuredOutputParser.ipynb
│
├── 🔍 Retrievers/
│   ├── VectorStoreRetrieverMMR-InsideRAG.ipynb
│   ├── ParentDocumentRetriever-InsideRAG.ipynb
│   └── MultiVectorRetriever-InsideRAG.ipynb
│
├── 🧠 Memory (Langchain 0.1)/
│   ├── CombinedMemoryExample.ipynb
│   ├── ConversationBufferMemoryExample.ipynb
│   ├── MessagesPlaceholderWithMemoryExample.ipynb
│   ├── ConversationSummaryMemoryExample.ipynb
│   ├── VectorStoreRetrieverMemoryExample.ipynb
│   └── SimpleMemory_with_RunnableWithMessageHistory.ipynb
│
├── 🔗 Runnable (0.3)/
│   ├── Runnable-Based-RAG-Pipeline.ipynb
│   └── Runnable_for_LLM_PipelineWithMessageHistory.ipynb
│
├── 🔗 Chains/
│   └── QAChain.ipynb
│
├── 🛠️ Tools/
│   ├── Tavily_Search_Extract_Tool.ipynb
│   ├── JSON_AgentToolkit_Tool.ipynb
│   ├── YahooFinanceNews_Stock_Tools.ipynb
│   ├── QuipDocumentGenerator_Tool.ipynb
│   ├── NutritionAI_CustomNutritionAI_Tool.ipynb
│   └── CustomEmailOperations_Tool.ipynb
│
├── 🔎 QueryBuilder/
│   ├── Chainable Query Builders.ipynb
│   ├── Static Query Builder.ipynb
│   ├── Dynamic Query Builders.ipynb
│   └── Metadata-based Query Builders.ipynb
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

**Performance Metrics for Embedding Models**:

| **Metric** | **Purpose** | **Calculation Formula** |
|------------|-------------|-------------------------|
| **MRR (Mean Reciprocal Rank)** | Measures ranking quality by prioritizing the first relevant result | `MRR = (1/Q) * Σ(1/rank_i)`, where `Q` is number of queries, `rank_i` is position of first relevant result for query `i` |
| **MAP (Mean Average Precision)** | Evaluates precision across all relevant results | `MAP = (1/Q) * Σ(AP_q)`, where `AP_q = Σ(Precision@k * rel(k)) / # relevant docs`, `rel(k)` is 1 if item at rank `k` is relevant, else 0 |
| **NDCG (Normalized Discounted Cumulative Gain)** | Assesses ranking quality with graded relevance, emphasizing higher ranks | `NDCG = DCG / IDCG`, where `DCG = Σ((2^rel_i - 1) / log2(i+1))`, `IDCG` is ideal DCG |
| **Top-1 Accuracy** | Measures if the top result is relevant | `Accuracy = (# correct top-1 predictions) / (# queries)` |
| **Average Spearman** | Evaluates correlation between predicted and true rankings | `Spearman = 1 - (6 * Σd_i^2) / (n * (n^2 - 1))`, where `d_i` is difference in ranks, `n` is number of items |

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

### 📝 Prompt Templates

Master prompt engineering with comprehensive templating solutions, now evaluated with performance metrics for effectiveness.

| **Template Type** | **Purpose** | **Key Features** |
|-------------------|-------------|------------------|
| **PromptTemplate** | Basic text prompts | Variable substitution, input validation |
| **ChatPromptTemplate** | Conversation handling | Multi-turn context, role management |
| **ChatMessagePromptTemplate** | Individual messages | Role-based formatting, dynamic composition |
| **🆕 ImagePromptTemplate** | Vision model prompts | Image + text prompting, multimodal workflows |
| **🆕 PipelinePromptTemplate** | Complex prompt chains | Multi-stage processing, prompt composition |

**Performance Metrics for Prompt Templates**:

| **Metric** | **Purpose** | **Calculation Formula** |
|------------|-------------|-------------------------|
| **Exact Match (EM)** | Measures if the model's answer exactly matches the ground truth (case-insensitive) | `EM = 1` if prediction equals ground truth, else `0` |
| **F1 (Token Overlap)** | Evaluates precision and recall of shared tokens between prediction and ground truth | `F1 = 2 * (Precision * Recall) / (Precision + Recall)`, where `Precision = |P ∩ G| / |P|`, `Recall = |P ∩ G| / |G|` |
| **Accuracy (Overlay-based)** | Checks for any token overlap between prediction and ground truth | `Accuracy = 1` if `|P ∩ G| > 0`, else `0` |
| **Pass@k** | Indicates if at least one of k generated answers matches ground truth | `Pass@k = 1` if any of top `k` predictions match, else `0` |
| **METEOR** | Assesses semantic similarity, considering synonyms, word order, and stemming | Uses METEOR algorithm: aligns prediction and ground truth, computes weighted harmonic mean of precision and recall |

### 🔧 Output Parsers

Transform raw LLM outputs into structured, usable formats with comprehensive parsing strategies designed for production reliability and type safety.

#### 🎯 Why Output Parsers Matter

Raw LLM outputs are often unstructured strings that need transformation into specific formats for downstream applications. Output parsers bridge this gap by providing:

- **🔒 Type Safety** - Guaranteed output formats with validation
- **📊 Structured Data** - Convert text to JSON, XML, or custom formats
- **🛡️ Error Handling** - Robust parsing with fallback mechanisms
- **🔄 Consistency** - Standardized output formats across different LLMs
- **⚡ Performance** - Optimized parsing for production workflows

#### 🎨 Parser Architecture Flow

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                           OUTPUT PARSER PIPELINE                           │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  Raw LLM Output ──► [Parser] ──► [Validation] ──► [Transformation] ──► Result│
│         │              │            │                  │                    │
│         │              ▼            ▼                  ▼                    │
│         │         [Format       [Schema            [Type                   │
│         │          Detection]    Validation]       Casting]                │
│         │              │            │                  │                    │
│         │              ▼            ▼                  ▼                    │
│         │              └────────► [Error Recovery & Retry Logic] ◄────┘    │
│                                                                             │
├─────────────────────────────────────────────────────────────────────────────┤
│                        PARSER TYPES & USE CASES                            │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│ 📝 STRING PARSER    │ 🔧 JSON PARSER     │ 📋 XML PARSER                   │
│ Clean & format text │ Structured data    │ Hierarchical data               │
│ Remove artifacts    │ API responses      │ Configuration files             │
│ Standardize output  │ Database records   │ Markup processing               │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

#### 🔧 Available Parser Implementations

| **Parser Type** | **Implementation** | **Key Features** | **Best For** |
|-----------------|-------------------|------------------|--------------|
| **StrOutputParser** | String processing & cleanup | • Text normalization<br>• Whitespace handling<br>• Encoding standardization<br>• Content filtering | • Simple text responses<br>• Content summarization<br>• Text classification tasks<br>• Basic Q&A systems |
| **JSONOutputParser** | JSON structure parsing | • Schema validation<br>• Type enforcement<br>• Nested object handling<br>• Error recovery | • API integrations<br>• Structured data extraction<br>• Database operations<br>• Complex data workflows |
| **XMLOutputParser** | XML document parsing | • Hierarchical data extraction<br>• Namespace support<br>• Attribute parsing<br>• Document validation | • Configuration management<br>• Markup processing<br>• Legacy system integration<br>• Structured document workflows |
| **PydanticOutputParser** | Pydantic-based parsing | • Type-safe data models<br>• Automatic validation<br>• Error handling<br>• Structured output enforcement | • Type-safe applications<br>• Complex data validation<br>• API integrations<br>• Production workflows |
| **StructuredOutputParser** | Structured data parsing | • Flexible schema definition<br>• Custom format parsing<br>• Error recovery<br>• Dynamic output structuring | • Dynamic data extraction<br>• Custom format parsing<br>• Structured data workflows<br>• Integration with varied LLMs |

#### 🎯 Parser Use Cases & Examples

**📝 String Parser Applications**
```
┌─────────────────────────────────────────────────────────────────────────────┐
│                         STRING PARSER SCENARIOS                            │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│ 💬 CHAT RESPONSES     │ 📄 CONTENT GENERATION │ 🎯 CLASSIFICATION           │
│ Clean conversational │ Article & blog writing │ Sentiment analysis          │
│ text for display     │ Social media content   │ Category assignment         │
│                      │                        │                             │
│ 🔍 SEARCH QUERIES     │ 📊 REPORT GENERATION   │ 🌐 TRANSLATION              │
│ Query preprocessing  │ Executive summaries    │ Language conversion         │
│ Intent extraction    │ Technical documentation│ Localization workflows      │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

**🔧 JSON Parser Applications**
```
┌─────────────────────────────────────────────────────────────────────────────┐
│                          JSON PARSER SCENARIOS                             │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│ 🌐 API RESPONSES      │ 📊 DATA EXTRACTION     │ 🔗 INTEGRATION              │
│ REST API integration │ Entity recognition     │ Webhook processing          │
│ Service orchestration│ Structured information │ Multi-system workflows      │
│                      │                        │                             │
│ 📋 FORM PROCESSING    │ 🎯 DECISION TREES      │ 📈 ANALYTICS                │
│ User input validation│ Logic flow execution   │ Metrics collection          │
│ Dynamic form creation│ Conditional processing │ Performance tracking        │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

**📋 XML Parser Applications**
```
┌─────────────────────────────────────────────────────────────────────────────┐
│                          XML PARSER SCENARIOS                              │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│ ⚙️ CONFIGURATION      │ 📄 DOCUMENT PROCESSING │ 🔄 DATA TRANSFORMATION     │
│ Settings management  │ Rich text formatting   │ Format conversion           │
│ Environment configs  │ Markup preservation    │ Legacy system migration     │
│                      │                        │                             │
│ 🌐 WEB SCRAPING       │ 📊 REPORT GENERATION   │ 🗂️ METADATA EXTRACTION      │
│ HTML content parsing │ Structured reporting   │ Document properties         │
│ Data extraction      │ Template processing    │ Content cataloging          │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

### 🔍 Retrievers

Advanced retrieval strategies for sophisticated RAG implementations with comprehensive end-to-end examples, now evaluated with performance metrics.

| **Retriever Type** | **Implementation** | **Key Features** | **Best For** |
|-------------------|-------------------|------------------|--------------|
| **VectorStoreRetrieverMMR** | Maximum Marginal Relevance in RAG | • Diversity optimization<br>• Relevance-diversity balance<br>• Complete RAG pipeline integration | Avoiding redundant results, diverse content retrieval |
| **ParentDocumentRetriever** | Hierarchical document retrieval in RAG | • Parent-child document relationships<br>• Context preservation<br>• Full RAG workflow demonstration | Long documents, maintaining context while chunking |
| **MultiVectorRetriever** | Multiple vector representation in RAG | • Multiple embedding strategies<br>• Enhanced retrieval accuracy<br>• End-to-end RAG implementation | Complex documents, multi-aspect retrieval |

**Performance Metrics for Retrievers**:

| **Metric** | **Purpose** | **Calculation Formula** |
|------------|-------------|-------------------------|
| **Precision@10** | Measures proportion of top 10 retrieved documents that are relevant | `Precision@10 = (# relevant docs in top 10) / 10` |
| **Recall@10** | Measures proportion of all relevant documents retrieved in top 10 | `Recall@10 = (# relevant docs in top 10) / (# total relevant docs)` |
| **F1 Score** | Balances precision and recall | `F1 = 2 * (Precision * Recall) / (Precision + Recall)` |
| **MRR (Mean Reciprocal Rank)** | Prioritizes ranking of first relevant document | `MRR = (1/Q) * Σ(1/rank_i)`, where `rank_i` is position of first relevant result |
| **Hit@5** | Indicates if at least one relevant document is in top 5 | `Hit@5 = 1` if top 5 contains a relevant doc, else `0` |
| **Faithfulness** | Evaluates if retrieved content aligns with ground truth | `Faithfulness = (# retrieved docs consistent with ground truth) / (# retrieved docs)` |

Each retriever notebook includes:
- **🔄 Complete RAG Pipeline** - From document loading to final answer generation
- **📊 Performance Metrics** - Retrieval quality and response evaluation
- **⚙️ Configurable Parameters** - Fine-tune retrieval strategies
- **🎯 Real-world Examples** - Practical use cases and implementations
- **📈 Comparative Analysis** - Benchmarking against baseline retrievers

### 🔎 Query Builders

Construct precise and efficient queries for vector stores and databases with flexible query-building strategies.

| **Query Builder Type** | **Implementation** | **Key Features** | **Best For** |
|------------------------|--------------------|------------------|--------------|
| **Chainable Query Builders** | Chained query construction | • Modular query composition<br>• Fluent API design<br>• Reusable query patterns | Complex, multi-step queries |
| **Static Query Builder** | Predefined query structures | • Simplified query creation<br>• Fixed query templates<br>• High performance | Simple, repetitive queries |
| **Dynamic Query Builders** | Runtime query generation | • Adaptive query logic<br>• Context-aware construction<br>• Parameterized queries | Dynamic, user-driven searches |
| **Metadata-based Query Builders** | Metadata-driven query construction | • Metadata filtering<br>• Schema-aware queries<br>• Advanced filtering logic | Metadata-rich environments, precise retrieval |

**Performance Metrics for Query Builders**:

| **Metric** | **Purpose** | **Calculation Formula** |
|------------|-------------|-------------------------|
| **Query Execution Time** | Measures time taken to execute a query | `Time = End_time - Start_time` |
| **Precision@10** | Measures proportion of top 10 retrieved results that are relevant | `Precision@10 = (# relevant results in top 10) / 10` |
| **Recall@10** | Measures proportion of all relevant results retrieved in top 10 | `Recall@10 = (# relevant results in top 10) / (# total relevant results)` |
| **F1 Score** | Balances precision and recall | `F1 = 2 * (Precision * Recall) / (Precision + Recall)` |
| **Query Complexity** | Evaluates computational complexity of query construction | Qualitative assessment based on number of operations and conditions |

Each query builder notebook includes:
- **🔧 Query Construction Examples** - Step-by-step query building
- **📊 Performance Metrics** - Query efficiency and retrieval quality
- **⚙️ Configurable Parameters** - Customize query logic and filters
- **🎯 Real-world Use Cases** - Practical applications in search and retrieval
- **📈 Comparative Analysis** - Benchmarking against baseline query methods

### 🧠 Memory Systems (LangChain 0.1)

Implement sophisticated conversation memory and context management for stateful LLM applications with comprehensive memory strategies:

#### Core Memory Types

| **Memory Type** | **Implementation** | **Key Features** | **Best For** |
|-----------------|-------------------|------------------|--------------|
| **ConversationBufferMemory** | Basic conversation history storage | • Simple message buffering<br>• Automatic conversation tracking<br>• Memory size management | Chatbots, basic conversational AI |
| **ConversationSummaryMemory** | Intelligent conversation summarization | • Automatic conversation summarization<br>• Token-efficient storage<br>• Context compression | Long conversations, token optimization |
| **CombinedMemory** | Multiple memory types integration | • Multi-modal memory combination<br>• Flexible memory strategies<br>• Advanced context preservation | Complex applications, multi-context scenarios |

#### Advanced Memory Integration

| **Memory Type** | **Implementation** | **Key Features** | **Best For** |
|-----------------|-------------------|------------------|--------------|
| **VectorStoreRetrieverMemory** | Vector-based memory retrieval | • Semantic memory search<br>• Long-term context storage<br>• Similarity-based recall | Knowledge-intensive applications, semantic search |
| **MessagesPlaceholderWithMemory** | Template-based memory integration | • Prompt template integration<br>• Dynamic message insertion<br>• Structured conversation flow | Structured dialogues, guided conversations |
| **SimpleMemory with RunnableWithMessageHistory** | Modern LangChain memory patterns | • Runnable-based architecture<br>• Session management<br>• Streamlined memory handling | Production applications, modern LangChain workflows |

**Comprehensive Memory Features:**
- **💬 Conversation Continuity** - Maintain context across multiple interactions with various retention strategies
- **🔄 State Management** - Persistent conversation state handling with session support
- **⚙️ Configurable Retention** - Control memory size, summarization, and retention policies
- **📝 Message Formatting** - Structured conversation history management and template integration
- **🎯 Semantic Recall** - Vector-based memory search for intelligent context retrieval
- **📊 Memory Optimization** - Token-efficient storage through summarization and compression
- **🔗 Modern Integration** - Compatible with latest LangChain patterns and runnable architectures

**Memory Strategy Comparison:**
- **Buffer Memory**: Best for short conversations requiring full history
- **Summary Memory**: Ideal for long conversations needing context compression
- **Vector Memory**: Perfect for knowledge-intensive apps requiring semantic search
- **Combined Memory**: Optimal for complex scenarios requiring multiple memory types
- **Runnable Memory**: Recommended for modern production applications

*Note: These implementations use LangChain 0.1 memory patterns for backward compatibility and established workflows, with examples ranging from basic buffer storage to advanced vector-based semantic memory.*

### 🔗 Runnable Architecture (LangChain 0.3)

Master the modern **Runnable** paradigm - LangChain's revolutionary approach to building composable, type-safe, and highly performant LLM applications through functional programming principles.

#### 🎯 What are Runnables?

**Runnables** represent LangChain's next-generation architecture that treats every component as a composable, functional unit. Think of them as intelligent building blocks that can be seamlessly connected, parallelized, and orchestrated to create sophisticated AI workflows.

#### 🏗️ Runnable Architecture Flow

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                           RUNNABLE ECOSYSTEM                                │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  Input Data ──► [Runnable A] ──► [Runnable B] ──► [Runnable C] ──► Output   │
│       │              │              │              │                       │
│       │              ▼              ▼              ▼                       │
│       │         [Parallel      [Conditional   [Memory                     │
│       │          Execution]     Routing]      Integration]                 │
│       │              │              │              │                       │
│       │              ▼              ▼              ▼                       │
│       │              └────────► [Error Handling & Monitoring] ◄───┘        │
│                                                                             │
├─────────────────────────────────────────────────────────────────────────────┤
│                        CORE RUNNABLE FEATURES                              │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│ 🔄 COMPOSABILITY    │ 🚀 ASYNC SUPPORT   │ 🎯 TYPE SAFETY                  │
│ Chain components    │ Non-blocking ops   │ Runtime validation              │
│ seamlessly          │ & parallel exec    │ & error prevention              │
│                     │                    │                                 │
│ 📊 STREAMING        │ 🔍 OBSERVABILITY   │ ⚡ PERFORMANCE                  │
│ Real-time output    │ Built-in logging   │ Optimized execution             │
│ & progressive resp  │ & monitoring       │ & resource mgmt                 │
│                                                                             │
└─────────────────────────────────────────────────────────────────────────────┘
```

#### 🚀 Runnable Pipeline Patterns

```
📋 SEQUENTIAL PIPELINE (Linear Execution)
┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
│ Document │──► │ Embedder │──► │ Retriever│──► │   LLM    │
│ Loader   │    │          │    │          │    │ Response │
└──────────┘    └──────────┘    └──────────┘    └──────────┘

🔀 PARALLEL PIPELINE (Concurrent Execution)
┌──────────┐    ┌──────────┐
│ Vector   │──► │          │
│ Search   │    │ Response │
└──────────┘ ┌─►│ Merger   │──► Final Output
┌──────────┐ │  │          │
│ Keyword  │─┘  │          │
│ Search   │    └──────────┘
└──────────┘

🧠 MEMORY-ENHANCED PIPELINE (Stateful Execution)
┌──────────┐    ┌──────────┐    ┌──────────┐    ┌──────────┐
│   User   │──► │ Message  │──► │   LLM    │──► │ Response │
│  Input   │    │ History  │    │Pipeline  │    │+ Memory  │
└──────────┘    └──────────┘    └──────────┘    └──────────┘
                      ▲                              │
                      └──────────────────────────────┘
                           Memory Update Loop
```

#### 🎛️ Available Runnable Implementations

| **Runnable Type** | **Implementation** | **Key Features** | **Architecture Benefits** |
|-------------------|-------------------|------------------|---------------------------|
| **Runnable-Based RAG Pipeline** | Complete RAG workflow using Runnable architecture | • Modular component design<br>• Type-safe data flow<br>• Async/streaming support<br>• Error handling & monitoring | • Composable components<br>• Easy testing & debugging<br>• Performance optimization<br>• Scalable architecture |
| **Runnable LLM Pipeline with MessageHistory** | Conversational LLM with persistent memory | • Stateful conversation management<br>• Message history integration<br>• Session-based memory<br>• Streaming responses | • Memory state isolation<br>• Concurrent session handling<br>• Efficient context management<br>• Production-ready patterns |

#### 🔧 Runnable Core Concepts

**🎯 Composability**
```python
# Traditional Approach (Complex & Rigid)
chain = LLMChain(llm=llm, prompt=prompt)
result = chain.run(input_data)

# Runnable Approach (Simple & Flexible)
pipeline = prompt | llm | output_parser
result = pipeline.invoke(input_data)
```

**⚡ Streaming & Async**
```python
# Real-time streaming responses
async for chunk in pipeline.astream(input_data):
    print(chunk, end="")

# Batch processing with parallelization
results = await pipeline.abatch([input1, input2, input3])
```

**🔄 Error Handling & Retry**
```python
# Built-in error handling with fallbacks
pipeline_with_fallback = primary_pipeline.with_fallbacks([
    fallback_pipeline_1,
    fallback_pipeline_2
])
```

#### 📊 Runnable Advantages Over Traditional Chains

| **Aspect** | **Traditional Chains** | **Runnable Architecture** |
|------------|------------------------|---------------------------|
| **Composition** | Complex inheritance patterns | Simple pipe operators (`|`) |
| **Type Safety** | Runtime errors common | Compile-time validation |
| **Performance** | Sequential execution | Parallel & async support |
| **Debugging** | Black box behavior | Transparent data flow |
| **Testing** | Difficult to unit test | Easy component isolation |
| **Streaming** | Limited support | Native streaming capabilities |
| **Memory Management** | Manual state handling | Built-in session management |
| **Error Handling** | Custom implementations | Standardized patterns |

#### 🎓 Learning Path for Runnables

1. **Start with Runnable-Based RAG Pipeline** - Understand core concepts and composition patterns
2. **Explore MessageHistory Integration** - Learn stateful applications and memory management
3. **Practice Async & Streaming** - Master performance optimization techniques
4. **Build Custom Runnables** - Create your own composable components

**🔮 Why Runnables Matter:**
- **Future-Proof Architecture** - Built for LangChain's long-term vision
- **Industry Standards** - Following functional programming best practices
- **Production Ready** - Designed for enterprise-scale applications
- **Developer Experience** - Simplified debugging and maintenance

*Note: Runnable architecture represents LangChain 0.3+ paradigms and is the recommended approach for new applications, offering superior performance, maintainability, and developer experience.*

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
   - Master `PromptsTemplates/` for prompt engineering
   - **NEW: Explore `Output Parsers/` for structured output handling**
   - Explore `Retrievers/` for advanced retrieval strategies
   - Learn `Memory (Langchain 0.1)/` for conversation state management
   - Master `Runnable (0.3)/` for modern LangChain architecture patterns
   - **NEW: Dive into `QueryBuilder/` for efficient query construction**

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
