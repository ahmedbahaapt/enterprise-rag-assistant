# Enterprise Knowledge Web Assistant

[![Python 3.x](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![LangChain](https://img.shields.io/badge/Framework-LangChain-green.svg)](https://langchain.com/)
[![Ollama](https://img.shields.io/badge/LLM-Ollama-black.svg)](https://ollama.com/)

> **Zero Data Leakage** Retrieval-Augmented Generation (RAG) system designed for corporate environments.

## About the Project
This project is a secure, air-gapped web assistant that allows organizations to query internal technical documents (manuals, regulations, PDFs) using natural language. By leveraging **Local Large Language Models (LLMs)** via Ollama and a vector database, the system ensures that sensitive corporate data never leaves the internal network.

It solves two critical enterprise challenges:
1. **Data Leaks:** Completely eliminates reliance on public APIs.
2. **Hallucinations:** The LLM is strictly grounded to the retrieved context, providing exact document citations for human validation.

---

## Table of Contents
- [Architecture & Features](#-architecture--features)
- [Tech Stack](#-tech-stack)
- [Repository Structure](#-repository-structure)
- [Getting Started](#-getting-started)
- [Academic Context](#-academic-context)

---

## Architecture & Features
* **Frontend:** Clean web interface for technical chat and document upload management.
* **Backend/Orchestration:** Python API using **LangChain** to handle document ingestion, semantic chunking, and context retrieval.
* **Vector Database:** Local semantic search storage (e.g., ChromaDB / FAISS).
* **Inference Engine:** **Ollama** running a quantized model (e.g., Llama 3) entirely on local CPU/GPU resources.
* **Prompt Security:** Input sanitization to mitigate Prompt Injection vulnerabilities.

---

## Tech Stack
* **Core Language:** Python 3
* **AI Framework:** LangChain
* **Local Inference:** Ollama
* **Version Control:** Git & GitHub

---

## Repository Structure

```text
enterprise-rag-assistant/
├── assets/       # Images, UML diagrams, and UI mockups
├── docs/         # Software Engineering reports and architecture specs
├── notebooks/    # Jupyter notebooks for testing embeddings and RAG pipelines
├── src/          # Main application source code (API backend & Frontend)
└── tests/        # Unit and integration tests for document retrieval logic
