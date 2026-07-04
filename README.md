# pdf_rag_chatbot

A Retrieval-Augmented Generation (RAG) chatbot that answers questions from uploaded PDF documents using Flask, LangChain, Hugging Face embeddings, Chroma vector database, and open-source LLMs.

The application is built with **Flask**, **LangChain**, **Chroma Vector Database**, **Hugging Face Embeddings**, and an **open-source Large Language Model (LLM)** running through IBM Watsonx.

---

## Features

- Upload PDF documents
- Extract and process document text
- Split documents into semantic chunks
- Generate vector embeddings using Sentence Transformers
- Store embeddings in Chroma Vector Database
- Retrieve the most relevant document sections
- Generate context-aware answers using an open-source LLM
- Interactive web interface
- Light/Dark mode
- Chat history support

---

## Architecture

```
User
   │
   ▼
Frontend (HTML/CSS/JavaScript)
   │
   ▼
Flask Backend
   │
   ▼
Document Processing
   │
   ├── PyPDFLoader
   ├── Text Splitter
   ├── HuggingFace Embeddings
   └── Chroma Vector Database
   │
   ▼
Retriever
   │
   ▼
Open Source LLM
   │
   ▼
Answer
```

---

## Tech Stack

- Python
- Flask
- LangChain
- Hugging Face Transformers
- Sentence Transformers
- ChromaDB
- IBM Watsonx
- HTML
- CSS
- JavaScript

---

## Project Structure

```
pdf-rag-chatbot/
│
├── server.py
├── worker.py
├── requirements.txt
├── templates/
│   └── index.html
├── static/
│   ├── script.js
│   └── style.css
└── README.md
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/your-username/pdf-rag-chatbot.git
```

Move into the project directory

```bash
cd pdf-rag-chatbot
```

Create a virtual environment

```bash
python -m venv my_env
```

Activate the environment

Linux/macOS

```bash
source my_env/bin/activate
```

Windows

```bash
my_env\Scripts\activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Run the Application

```bash
python server.py
```

Open your browser

```
http://127.0.0.1:8000
```

---

## How It Works

1. Upload a PDF document.
2. Extract text using **PyPDFLoader**.
3. Split the document into chunks.
4. Convert chunks into embeddings.
5. Store embeddings in Chroma.
6. Convert the user's question into an embedding.
7. Retrieve the most relevant document chunks.
8. Send the retrieved context to the LLM.
9. Return an accurate answer based on the document.

---

## RAG Pipeline

```
PDF
 │
 ▼
Text Extraction
 │
 ▼
Chunking
 │
 ▼
Embeddings
 │
 ▼
Vector Database
 │
 ▼
Retriever
 │
 ▼
LLM
 │
 ▼
Answer
```

---

## Future Improvements

- Multiple PDF support
- Persistent vector database
- Streaming responses
- Source citations
- Conversation memory
- Docker deployment
- Authentication
- GPU optimization
- REST API
- Support for additional document formats

---

## Learning Objectives

This project demonstrates practical implementation of:

- Retrieval-Augmented Generation (RAG)
- LangChain
- Flask Web Development
- Vector Databases
- Semantic Search
- Embedding Models
- Open-source Large Language Models
- PDF Question Answering

---

## License

This project is for educational and research purposes.