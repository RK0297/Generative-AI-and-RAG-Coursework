# Generative AI and RAG Fundamentals

Last Updated: June 8, 2026

Comprehensive coursework covering Generative AI, Retrieval-Augmented Generation (RAG) systems, and production-grade pipelines. This repository contains concept-focused notes, hands-on notebooks, and resources for building correct mental models before extending into enterprise AI applications.

**Tags:** `generative-ai`, `rag`, `llm`, `nlp`, `vector-search`, `chromadb`, `bert`, `langchain`, `ai-engineering`, `machine-learning`, `peft`, `lora`, `qlora`, `fine-tuning`

## Learning Path

```
00 Docker Fundamentals ─────────── Containerization for reproducible environments
        │
01 BERT & NLP Foundations ──────── NLP mental models with transformers
        │
02 RAG & LLM Fundamentals ─────── Retrieval-augmented generation concepts
        │
03 Vector Search & Retrieval ───── Efficient semantic search with ChromaDB
        │
04 Advanced RAG & Fine-Tuning ──── LangChain orchestration, evaluation,
        │                           guardrails, LoRA/QLoRA fine-tuning
        │
05 Data Engineering ────────────── Scalable data pipelines with Kafka & Spark
```

## Directory Structure

### 00-Docker-Fundamentals
Container infrastructure and deployment basics.
| File | Description |
|------|-------------|
| Docker_Basics.pdf | Introduction to Docker, containerization concepts, and image management |
| Docker_Networks_and_Composition.pdf | Docker networking, multi-container orchestration, and Compose workflows |

### 01-BERT-NLP-Foundations
Foundational NLP models and transformer architecture.
| File | Description |
|------|-------------|
| bert_fundamentals.ipynb | Tokenization, loading BERT, extracting hidden states, NER, custom PyTorch structures |
| bert_flashcards.html | Visual explanation of BERT encoder blocks, MLM, and NSP |

### 02-RAG-LLM-Fundamentals
Core concepts for prompting, generation, embeddings, and basic similarity matching.
| File | Description |
|------|-------------|
| llm_generation_embeddings.ipynb | Embeddings via APIs (OpenAI/OpenRouter), text generation with GPT-2 |
| rag_scratch_implementation.ipynb | Complete RAG loop with pure math (cosine similarity, dot products) |
| hugging_face_ecosystem_walkthrough.ipynb | Walkthrough of the Hugging Face ecosystem |
| Hugging_Face.pptx | Presentation on Hugging Face libraries and models |
| rag_01_foundations_and_architecture.pdf | Why RAG exists, core architecture, retrieval-generation flow |
| rag_03_query_time_retrieval.pdf | Query-time retrieval, prompt augmentation, grounded generation |

### 03-Vector-Search-and-Retrieval
Vector search algorithms, ChromaDB implementations, and similarity-based retrieval.
| File | Description |
|------|-------------|
| chromadb_walkthrough.ipynb | Vector search using ChromaDB |
| Vector_Search_Fundamentals.pptx | Vector search concepts and applications |
| Chunking_Hybrid_RAG_Evaluation.pdf | Chunking strategies, hybrid RAG, retrieval evaluation metrics |

### 04-Advanced-RAG-LangChain
LangChain orchestrations, retrieval evaluations, guardrails, and parameter-efficient fine-tuning.

**Notebooks:**
| # | File | Description |
|---|------|-------------|
| 01 | rag_knowledge_graph_neo4j.ipynb | Graph-based RAG using Neo4j and LangChain |
| 02 | advanced_rag_self_query.ipynb | Self-querying retrieval with metadata filtering |
| 03 | rag_evaluation.ipynb | RAG evaluation using RAGAS metrics (faithfulness, relevancy, context precision) |
| 04 | chatbot_evaluation.ipynb | Evaluating conversational AI with automated metrics |
| 05 | llm_guardrails.ipynb | Safety guardrails for LLM applications (input/output validation, content filtering) |
| 06 | lora_qlora_peft_finetuning.ipynb | LoRA, QLoRA, PEFT fine-tuning with OPT-350M on WikiText-2 — architecture diagrams, weight freezing, gradient checkpointing, adapter management |

**Reference Materials:**
| File | Description |
|------|-------------|
| KV_and_Graph_DB_Notes.pdf | Key-value stores, graph databases, structured data retrieval |
| AWS_EC2.pdf | EC2 instance types, configuration, and deployment for AI workloads |
| Pinecone__Vector_Database.pdf | Pinecone vector database architecture, indexing, production deployment |

> **Note:** `Neo4jVector` import has moved. Use:
> ```python
> from langchain_neo4j.vectorstores import Neo4jVector  # pip install langchain-neo4j
> ```

### 05-Data-Engineering-and-Streaming
Real-time data processing and complementary big data technologies.
| File | Description |
|------|-------------|
| kafka_pyspark_streaming_walkthrough.ipynb | Real-time pipelines with Apache Kafka and PySpark Streaming (Windows setup) |
| Big_Data_Technologies.pdf | Big data platforms, distributed computing, data processing frameworks |
| Time_Series_Fundamentals.pdf | Time series analysis, forecasting, temporal data patterns |
| Database_Management_Fundamentals.pdf | Database concepts, ACID properties, query optimization |

## Learning Goal

This repository focuses on building correct mental models first, followed by lightweight hands-on practice, extending natively into production-grade AI pipelines and enterprise applications.