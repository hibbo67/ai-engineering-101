# AI Engineering 101 — RAG Pipeline

This repository contains my implementation of a Retrieval-Augmented Generation (RAG) pipeline, built as part of a 45-day AI engineering curriculum. 

## 🚀 The Core Project: `day21_first_rag.ipynb`
Instead of just theory, this repo focuses on the working code. `day21_first_rag.ipynb` is a fully functional customer support bot that:
- Ingests documents into a vector database (ChromaDB)
- Embeds text using Google's `gemini-embedding-2`
- Retrieves relevant context based on semantic similarity
- Uses a distance threshold (guardrail) to prevent hallucinations
- Generates answers with Gemini 3.6 Flash, complete with source citations

## 📈 Evaluation
`day23_llm_judge.ipynb` builds on the RAG pipeline by adding an automated evaluation system. It uses an LLM as a judge to score the bot's answers on **Faithfulness** (no hallucinations) and **Helpfulness**, ensuring the system is reliable before deployment.

## 🛠️ Stack
- **LLM:** Google Gemini 3.6 Flash
- **Vector DB:** ChromaDB
- **Embeddings:** `gemini-embedding-2`
- **Environment:** Google Colab
