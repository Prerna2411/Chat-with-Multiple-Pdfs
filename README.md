# 🗂️ Chat with Multiple PDFs – Cohere + LangChain

This project allows you to **chat with one or more PDF documents** using **Cohere embeddings** and **LangChain**, enabling intelligent document understanding and Q&A.

---

## 🚀 Features

- 📚 Upload multiple PDFs  
- 🤖 Ask natural-language questions  
- 🧠 Uses Cohere’s `embed-english-v3.0` model for semantic understanding  
- 🔗 Built using LangChain, Cohere, and optionally Streamlit for UI  

---

## 🛠️ Tech Stack

- Python 3.8+  
- [LangChain](https://www.langchain.com/)  
- [Cohere](https://cohere.com/)  
- [python-dotenv](https://pypi.org/project/python-dotenv/)  
- [Streamlit](https://streamlit.io/) (optional for frontend)  
- [FAISS](https://github.com/facebookresearch/faiss) (or any other vector store)

---

## 📁 Folder Structure

chat-with-multiple-pdfs/
│
├── app.py # Main app logic
├── requirements.txt # Dependencies
├── .env # API key storage (ignored by git)
└── README.md # Project documentation


---

## 🧠 How It Works

1. **PDF Loading**  
   PDFs are loaded and split into smaller chunks using LangChain's `TextSplitter`.

2. **Embedding with Cohere**  
   Each chunk is embedded using `CohereEmbeddings` with the model `embed-english-v3.0`.

3. **Storing in Vector DB**  
   The resulting embeddings are stored in a vector store like FAISS.

4. **Question Answering**  
   When a question is asked, the system retrieves the most relevant chunks and generates an answer using an LLM.

---
