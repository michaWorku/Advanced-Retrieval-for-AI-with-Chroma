# **Advanced Retrieval for AI with Chroma**  

## **Course Overview**  
[Advanced Retrieval for AI with Chroma](https://www.deeplearning.ai/short-courses/advanced-retrieval-for-ai/) explores **advanced retrieval techniques** to enhance **information retrieval** for **Retrieval-Augmented Generation (RAG) and AI applications**. Led by **Anton Troynikov**, this course focuses on **improving query relevance**, **embedding fine-tuning**, and **re-ranking search results** using Chroma DB.  

### **What You’ll Learn**  
- Identify and fix poor query results.  
- Use **LLMs** to enhance queries.  
- Fine-tune **embeddings** using user feedback.  

### **Key Topics**  
- **Query Expansion** – Augment queries with generated answers or multiple queries for improved retrieval.  
- **Cross-encoder Re-ranking** – Improve search accuracy by prioritizing relevant documents.  
- **Embedding Adapters** – Customize embeddings to emphasize application-specific features.  

By the end of this course, you’ll be able to **optimize AI retrieval pipelines** and improve search accuracy, making your **RAG systems more effective and reliable**. 🚀  
 

## **Course Contents**  

### [**1. Embeddings-Based Retrieval**]()  
- Introduction to **Retrieval-Augmented Generation (RAG)**.  
- **Data Processing:**  
  - Load and filter PDF data.  
  - Use text splitters (character-based & token-based).  
- **Chroma DB Implementation:**  
  - Store embeddings in Chroma collections.  
  - Retrieve relevant documents using queries.  
- **Building a RAG Pipeline:**  
  - Combine retrieval with an **LLM-based response generator**.  

📌 [*Notebook: `L1-Embeddings_based_retrival.ipynb`*]()  

### [**2. Pitfalls of Retrieval – When Simple Vector Search Fails** ] 
- **Understanding Retrieval Issues:**  
  - When queries return **semantically similar but irrelevant** results.  
  - Distractions in retrieved documents.  
- **Visualization with UMAP:**  
  - Project query and document embeddings.  
  - Identify **relevance vs. distraction** in retrieval.  

📌 [*Notebook: `L2-Pitfalls_of_retrieval.ipynb`*]()  

### [**3. Query Expansion**]()  
- **Expansion with Generated Answers:**  
  - Use **LLMs** to suggest possible answers, which are included in the query.  
  - Retrieve documents with additional context.  
- **Expansion with Multiple Queries:**  
  - Generate multiple reformulations of a query.  
  - Retrieve results for **all variations** and merge responses.  
- **Visualization:**  
  - Project original & expanded query embeddings to analyze impact.  

📌 [*Notebook: `L3-Query_expansion.ipynb`*]()  

### [**4. Cross-Encoder Re-ranking**]()  
- **Improving Retrieval with Re-ranking:**  
  - Retrieve more documents initially and then **rank** them based on relevance.  
- **Comparison of Bi-encoder vs. Cross-encoder:**  
  - **Bi-encoder:** Independent embeddings for query & document.  
  - **Cross-encoder:** Processes both together for **better contextual understanding**.  
- **Applications:**  
  - Re-rank retrieved results to **prioritize the most relevant ones**.  
  - Combine **query expansion & re-ranking** for improved retrieval.  

📌 [*Notebook: `L4-Cross_encoder_reranking.ipynb`*]()  

### [**5. Embedding Adapters**]()  
- **Enhancing Embeddings for Better Retrieval:**  
  - Generate and retrieve **training data**.  
  - Fine-tune embeddings using an **adapter layer**.  
- **Training a Custom Adapter Model:**  
  - Build a model to **adjust embeddings** for domain-specific needs.  
  - Train using **MSE loss** to optimize retrieval quality.  
- **Visualization of Adapted Embeddings:**  
  - Compare standard vs. adapted embeddings to measure improvements.  

📌 [*Notebook: `L5-Embedding_addaptors.ipynb`*]()  

### **6. Other Advanced Techniques**  
- **Fine-tuning Embedding Models** – Train custom embeddings for better domain adaptation.  
- **Fine-tuning LLMs for Retrieval** – Improve AI models for **query understanding**.  
- **Deep Relevance Modeling** – Enhance retrieval with neural relevance models.  
- **Deep Chunking** – Optimize document splitting for retrieval performance.  

📌 *References:*  
- [RA-DIT: Retrieval-Augmented Dual Instruction Tuning](https://arxiv.org/abs/2310.01352)  
- [InstructRetro: Retrieval-Augmented Pretraining](https://arxiv.org/abs/2310.07713)  


## **Notebooks & Resources**  

| Topic | Notebook |  
|-----------------------------|----------------------------------|  
| **Embeddings-Based Retrieval** | [`L1-Embeddings_based_retrival.ipynb`]() |  
| **Pitfalls of Retrieval** | [`L2-Pitfalls_of_retrieval.ipynb`]() |  
| **Query Expansion** | [`L3-Query_expansion.ipynb`]() |  
| **Cross-Encoder Re-ranking** | [`L4-Cross_encoder_reranking.ipynb`]() |  
| **Embedding Adapters** | [`L5-Embedding_addaptors.ipynb`]() |  
| **Example Dataset** | [`microsoft_annual_report_2022.pdf`]() |  
  

## **Getting Started**  
1. Install required dependencies:  
   ```bash
   pip install chromadb transformers torch umap-learn
   ```
2. Load and preprocess your dataset.  
3. Run the notebooks in order to **implement advanced retrieval techniques**.  

## **References**  
- [Course Link](https://www.deeplearning.ai/short-courses/advanced-retrieval-for-ai/)  

This course equips you with **state-of-the-art retrieval techniques** to **boost AI-powered search systems**! 🚀