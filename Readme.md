Retrieval Augmented Generation (RAG) — Foundations & Practice

This repository contains concept-focused notes and hands-on notebooks covering the core ideas of Retrieval Augmented Generation (RAG), aimed at a DSAI student with an AI-first focus.

Contents
Conceptual Notes (PDFs)

RAG-1.pdf — Why RAG exists, core architecture, retrieval → augmentation → generation

RAG-2.pdf — Chunking, embeddings, vector databases, cosine similarity

RAG-3.pdf — Query-time retrieval, prompt augmentation, grounded generation

Hands-on Notebooks

rag.ipynb — Text preprocessing, vectorization, embedding intuition

rag2.ipynb — End-to-end RAG-style flow with retrieval + generation logic

What This Repository Covers Well

Motivation for RAG and its limitations vs plain LLMs

Offline ingestion vs online query-time pipeline

Chunking basics and overlap intuition

Embeddings and embedding matrix understanding

Cosine similarity and Top-K retrieval

Prompt augmentation for grounded generation

Clear separation of transformer embeddings vs RAG embeddings

What Is Intentionally Out of Scope (Next Level)

Vector database internals (FAISS, HNSW, IVF)

Chunking strategy optimization and semantic chunking

Retrieval evaluation metrics (precision@k, recall@k, MRR)

RAG failure modes and mitigation

Re-ranking and hybrid retrieval (BM25 + dense retrievers)

These are planned as advanced extensions, not fundamentals.

Learning Goal

This repository focuses on building correct mental models first, followed by lightweight hands-on practice, without premature optimization or low-level training code.

It is designed to be:

Conceptually strong

Exam and interview friendly

Ready to extend into production-grade RAG later