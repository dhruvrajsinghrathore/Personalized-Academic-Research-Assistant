# Personalized-Academic-Research-Assistant

Description: Develop an academic research assistant that retrieves papers from an academic database, ranks them using BERT, and summarizes findings using an LLM like Ollama3.2.
Skills Demonstrated: RAG, academic document retrieval, summarization, ranking, and LangChain orchestration.

Key Features
Academic Paper Retrieval: Fetch relevant papers based on a research query using embeddings and FAISS.
BERT Ranking: Rank the retrieved papers using a fine-tuned BERT model trained on scientific datasets (e.g., SciBERT).
Summary Generation: Use Ollama3.2 to generate concise summaries for each retrieved paper.
Advanced Queries: Handle multi-turn dialogues for follow-up questions using LangChain.
Code Workflow
Data Preparation:
Use a dataset like arXiv Academic Papers or research PDFs.
Document Embeddings:
Generate embeddings using sentence-transformers/scibert.
Store embeddings in FAISS for retrieval.
Pipeline:
Combine retrieval, ranking, and summarization into a pipeline using LangChain.
