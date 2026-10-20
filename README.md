# AI Engineering 101 — RAG & Agentic Pipeline

This repository contains my implementation of a Retrieval-Augmented Generation (RAG) pipeline and autonomous agents, built as part of a 45-day AI engineering curriculum. 

## 🚀 Core Projects

### 1. The RAG Pipeline: `day21_first_rag.ipynb`
A fully functional customer support bot that:
- Ingests documents into a vector database (ChromaDB)
- Embeds text using Google's `gemini-embedding-2`
- Retrieves relevant context based on semantic similarity
- Uses a distance threshold (guardrail) to prevent hallucinations
- Generates answers with Gemini 3.6 Flash, complete with source citations

### 2. Automated Evaluation: `day23_llm_judge.ipynb`
An automated testing system that uses an LLM as a judge to score the RAG bot's answers on **Faithfulness** (no hallucinations) and **Helpfulness**.

### 3. Autonomous Loop Agent: `day26_loop_agent.ipynb`
A multi-step AI agent that evaluates its own progress. It uses a stateful loop to call multiple tools in sequence (like a calculator and a string reverser) until a complex goal is completed, with a built-in circuit breaker to prevent infinite loops.

## 🛠️ Stack
- **LLM:** Google Gemini 3.6 Flash
- **Vector DB:** ChromaDB
- **Embeddings:** `gemini-embedding-2`
- **Environment:** Google Colab
