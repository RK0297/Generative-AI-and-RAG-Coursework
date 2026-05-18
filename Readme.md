# Generative AI and RAG Coursework

Last Updated: May 18, 2026

This repository contains concept-focused notes and hands-on notebooks covering the core ideas of Generative AI, Retrieval-Augmented Generation (RAG), and advanced agentic workflows.

## Directory Structure

### 01-BERT
Foundational NLP models and architecture.
- bert_fundamentals.ipynb: Tokenization, loading BERT, extracting hidden states, identifying NER, custom PyTorch structures.
- bert_flashcards.html: Visual explanation of BERT encoder blocks, MLM, and NSP.

### 02-Basic-RAG-and-LLMs
Core concepts for Prompting, generation, and basic similarity matching.
- llm_generation_embeddings.ipynb: Exploring embeddings via APIs (OpenAI/OpenRouter) and generating text via local transformers like GPT-2.
- rag_scratch_implementation.ipynb: Complete RAG loop implementation with pure math (cosine similarity, dot products) and basic API ingestion.

### 03-Vector-Search
(Coming Soon) Vector search algorithms, ChromaDB implementations, and FAISS.

### 04-Advanced-RAG
(Coming Soon) LangChain, LangGraph orchestrations, retrieval evaluations, hybrid search, and production GenAI pipelines.

### 05-Miscellaneous
Support scripts and testing directories.

### Lectures
Concept notes physically written and typed for learning.
- rag_01_foundations_and_architecture.pdf: Why RAG exists, core architecture, and the retrieval-generation flow.
- rag_03_query_time_retrieval.pdf: Query-time retrieval, prompt augmentation, and grounded generation.

## Learning Goal

This repository focuses on building correct mental models first, followed by lightweight hands-on practice, extending natively into production-grade pipelines.