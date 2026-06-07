# Generative AI and RAG Fundamentals

Last Updated: June 7, 2026

Comprehensive coursework covering Generative AI, Retrieval-Augmented Generation (RAG) systems, and production-grade pipelines. This repository contains concept-focused notes, hands-on notebooks, and resources for building correct mental models before extending into enterprise AI applications.

**Tags:** `generative-ai`, `rag`, `llm`, `nlp`, `vector-search`, `chromadb`, `bert`, `langchain`, `ai-engineering`, `machine-learning`, `peft`, `lora`, `qlora`, `fine-tuning`

## Directory Structure

### 00-Docker-Fundamentals
Container infrastructure and deployment basics.
- Docker_Basics.pdf: Introduction to Docker, containerization concepts, and image management.
- Docker_Networks_and_Composition.pdf: Docker networking, multi-container orchestration, and Compose workflows.

### 01-BERT-NLP-Foundations
Foundational NLP models and transformer architecture.
- bert_fundamentals.ipynb: Tokenization, loading BERT, extracting hidden states, identifying NER, custom PyTorch structures.
- bert_flashcards.html: Visual explanation of BERT encoder blocks, MLM, and NSP.

### 02-RAG-LLM-Fundamentals
Core concepts for prompting, generation, embeddings, and basic similarity matching.
- llm_generation_embeddings.ipynb: Exploring embeddings via APIs (OpenAI/OpenRouter) and generating text via local transformers like GPT-2.
- rag_scratch_implementation.ipynb: Complete RAG loop implementation with pure math (cosine similarity, dot products) and basic API ingestion.
- hugging_face_ecosystem_walkthrough.ipynb: Walkthrough of the Hugging Face ecosystem.
- Hugging_Face.pptx: Presentation on Hugging Face libraries and models.
- rag_01_foundations_and_architecture.pdf: Why RAG exists, core architecture, and the retrieval-generation flow.
- rag_03_query_time_retrieval.pdf: Query-time retrieval, prompt augmentation, and grounded generation.

### 03-Vector-Search-and-Retrieval
Vector search algorithms, ChromaDB implementations, and similarity-based retrieval.
- chromadb_walkthrough.ipynb: Walkthrough of vector search using ChromaDB.
- Vector_Search_Fundamentals.pptx: Presentation on vector search concepts and applications.
- Chunking_Hybrid_RAG_Evaluation.pdf: Advanced chunking strategies, hybrid RAG approaches, and retrieval evaluation metrics.

### 04-Advanced-RAG-LangChain
LangChain orchestrations, retrieval evaluations, guardrails, and parameter-efficient fine-tuning.
- 01_rag_knowledge_graph_neo4j.ipynb: Graph-based RAG using Neo4j and LangChain for knowledge graph retrieval.
- 02_advanced_rag_self_query.ipynb: Self-querying retrieval with metadata filtering and dynamic prompt construction.
- 03_rag_evaluation.ipynb: RAG pipeline evaluation using RAGAS metrics (faithfulness, relevancy, context precision).
- 04_chatbot_evaluation.ipynb: Evaluating conversational AI systems with automated metrics.
- 05_llm_guardrails.ipynb: Implementing safety guardrails for LLM applications (input/output validation, content filtering).
- 06_lora_qlora_peft_finetuning.ipynb: Complete LoRA, QLoRA, and PEFT fine-tuning pipeline with OPT-350M on WikiText-2. Includes architecture diagrams, weight freezing, gradient checkpointing, and adapter management.
- KV_and_Graph_DB_Notes.pdf: Key-value stores, graph databases, and structured data retrieval patterns.

**Note:** `Neo4jVector` import has moved. Use one of these approaches:
```python
# Option 1 (LangChain community)
from langchain_community.vectorstores.neo4j_vector import Neo4jVector

# Option 2 (Recommended - requires langchain-neo4j)
from langchain_neo4j.vectorstores import Neo4jVector
pip install langchain-neo4j
```

### 05-Data-Engineering-and-Streaming
Support scripts, real-time data processing, and complementary big data technologies.
- kafka_pyspark_streaming_walkthrough.ipynb: Real-time data pipelines using Apache Kafka and PySpark Streaming (Windows setup guide included).
- Big_Data_Technologies.pdf: Overview of big data platforms, distributed computing, and data processing frameworks.
- Time_Series_Fundamentals.pdf: Time series analysis, forecasting, and temporal data patterns.
- Database_Management_Fundamentals.pdf: Database concepts, ACID properties, and query optimization.

## Learning Path

1. **Docker Fundamentals** → Understand containerization for reproducible environments
2. **BERT & NLP Foundations** → Build NLP mental models with transformers
3. **RAG & LLM Fundamentals** → Master retrieval-augmented generation concepts
4. **Vector Search & Retrieval** → Implement efficient semantic search
5. **Advanced RAG & Fine-Tuning** → Production-grade orchestration, evaluation, guardrails, and LoRA/QLoRA fine-tuning
6. **Data Engineering** → Build scalable data pipelines

## Learning Goal

This repository focuses on building correct mental models first, followed by lightweight hands-on practice, extending natively into production-grade AI pipelines and enterprise applications.