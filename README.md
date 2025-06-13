🗂️ Chat with Multiple PDFs – Cohere + LangChain
This project allows you to chat with one or more PDF documents using Cohere embeddings and LangChain, enabling intelligent document understanding and Q&A.

🚀 Features
📚 Upload multiple PDFs

🤖 Ask natural-language questions

🧠 Uses Cohere’s embed-english-v3.0 model for semantic understanding

🔗 Built using LangChain, Cohere, and optionally Streamlit for UI

🛠️ Tech Stack
Python 3.8+

LangChain

Cohere

Python-dotenv

Streamlit (optional for frontend)

FAISS (or other vector store)

📁 Folder Structure
chat-with-multiple-pdfs/
│
├── app.py                  # Main app logic
├── requirements.txt        # Dependencies
├── .env                    # API key storage (ignored by git)
└── README.md               # Project documentation

🧠 How It Works
1.PDFs are loaded and split into smaller chunks using LangChain's TextSplitter.

2.Each chunk is embedded using CohereEmbeddings with model embed-english-v3.0.

3.Embeddings are stored in a vector store like FAISS.

4.When you ask a question, it retrieves the most relevant chunks and returns an AI-generated answer.
