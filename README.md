# 📰 News RAG Project

This project implements a **Retrieval-Augmented Generation (RAG)** system on news articles.
It retrieves relevant news content using vector embeddings and a vector database, then generates answers using a large language model.
A **Gradio web interface** is used to provide an interactive frontend for querying the system.

---

## 📌 Project Overview

The pipeline follows these main steps:

1. Collect news articles from the NewsAPI.
2. Clean and preprocess the text data.
3. Split articles into chunks for efficient retrieval.
4. Generate embeddings and store them in a Pinecone vector database.
5. Use a RAG pipeline to retrieve relevant documents and generate responses.
6. Provide a user-friendly interface using **Gradio**.

---

## 🛠️ Technologies Used

* **Python**
* **LangChain**
* **Hugging Face Transformers**
* **Meta LLaMA 3.2 (3B Instruct)**
* **Pinecone** (Vector Database)
* **NewsAPI** (Data Source)
* **Gradio** (Frontend Interface)

---

## 🔐 Environment Variables

The following environment variables are required:

* `NEWS_API_KEY` – NewsAPI key
* `PINECONE_API_KEY` – Pinecone API key
* `HF_TOKEN` – Hugging Face token (required for gated LLaMA models)

Make sure these are set before running the notebook.

---

## 🤖 Model

The project uses the following language model:

* **meta-llama/Llama-3.2-3B-Instruct**

Authentication is required because this is a **gated Hugging Face model**.

---

## 🌐 Frontend (Gradio)

A **Gradio interface** is used to allow users to:

* Enter natural language questions
* Query the RAG system
* Receive generated answers in real time

This makes the project easy to interact with without directly running code cells.

---

## ▶️ How to Run

1. Install dependencies
2. Set required environment variables
3. Run the notebook cells in order
4. Launch the Gradio interface
5. Ask questions related to the ingested news articles

---

## ✅ Results

The system successfully retrieves relevant news documents and generates coherent answers based on the retrieved context.
It demonstrates the effectiveness of combining vector search with large language models.

---

## Future Improvements

* Add metadata filtering (date, source, category)
* Improve chunking strategy
* Experiment with different embedding models
* Deploy the Gradio app online

---

## 📌 Conclusion

This project demonstrates a complete end-to-end RAG pipeline applied to real-world news data, enhanced with an interactive frontend for improved usability.
