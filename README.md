# **Personalized Academic Research Assistant**

### **Project Overview**
The **Personalized Academic Research Assistant** is an intelligent tool designed to streamline academic research. It retrieves relevant academic papers, ranks them based on contextual relevance, and generates concise summaries, providing researchers with key insights efficiently.

---

### **Key Features**
1. **Academic Paper Retrieval**  
   - Fetches relevant papers from academic databases like arXiv using embeddings and **FAISS** for efficient search.  
   - Supports custom research queries to narrow down results.  

2. **BERT Ranking**  
   - Ranks retrieved papers using a fine-tuned **BERT model** (e.g., SciBERT) trained on scientific datasets.  
   - Ensures the most contextually relevant papers are prioritized.

3. **Summary Generation**  
   - Leverages **Ollama3.2**, a cutting-edge large language model, to generate concise summaries for each paper.  
   - Offers quick insights into complex research topics.

4. **Advanced Query Handling**  
   - Supports multi-turn dialogues to refine search results and answer follow-up questions using **LangChain**.  
   - Enhances user experience by enabling conversational interactions.

---

### **Skills Demonstrated**
- **RAG (Retrieval-Augmented Generation)**: Combines retrieval and LLM-based generation for accurate and context-aware results.  
- **Document Retrieval**: Efficiently retrieves relevant papers using **FAISS** and embeddings.  
- **Summarization**: Generates human-readable summaries for dense academic content using LLMs.  
- **Ranking**: Implements fine-tuned **BERT models** to rank papers based on relevance.  
- **LangChain Orchestration**: Integrates retrieval, ranking, and summarization into a seamless pipeline.

---

### **Code Workflow**

#### **1. Data Preparation**
- Utilize datasets like arXiv Academic Papers or research PDFs.
- Clean and preprocess text data, extracting titles, abstracts, and other metadata.

#### **2. Document Embeddings**
- Generate embeddings for paper abstracts using **sentence-transformers/scibert**.  
- Store these embeddings in **FAISS**, a high-performance similarity search library, for fast retrieval.

#### **3. Pipeline Integration**
- Combine the following components into a unified workflow using **LangChain**:
  1. **Retrieval**: Search the FAISS index for relevant papers based on a user query.  
  2. **Ranking**: Score and rank results using a fine-tuned **BERT model** to prioritize contextual relevance.  
  3. **Summarization**: Pass top-ranked papers to **Ollama3.2** for concise summary generation.

#### **4. Advanced Query Support**
- Enable follow-up questions and multi-turn dialogue handling through LangChain’s conversational capabilities.

---

### **Future Enhancements**
- Expand support for additional datasets like PubMed and IEEE Xplore.
- Integrate PDF parsing for offline research papers.
- Incorporate fine-tuning capabilities for domain-specific queries.

---

### **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
