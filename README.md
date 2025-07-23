# ML-pro-2
##########################################################################
# 🤖 AskMyDocs – Retrieval-Augmented Generation (RAG) PDF Chatbot

AskMyDocs is an intelligent chatbot that uses **Retrieval-Augmented Generation (RAG)** to answer questions based on the content of uploaded PDF files. It combines vector search and large language models to create a powerful document-based Q&A system.

---

## 🧠 What is RAG?

**Retrieval-Augmented Generation (RAG)** enhances language models with external knowledge. Instead of relying solely on model memory, it retrieves relevant chunks of information from a document and then generates a response based on both the prompt and the retrieved content.

---

## 🔥 Features

- 📄 Upload any PDF and ask questions about its content
- 🔍 Retrieves relevant information using semantic similarity (vector search)
- 🤖 Uses a language model (e.g., OpenAI GPT) for generating accurate answers
- 🧠 Handles large documents with smart chunking
- 🖥️ Optional Streamlit UI for interactive chatbot interface

---

## 🛠️ Tech Stack

| Tool       | Purpose                            |
|------------|------------------------------------|
| Python     | Core programming language          |
| LangChain  | RAG orchestration & chunking       |
| FAISS      | Vector store for document chunks   |
| OpenAI     | Language model for answering       |
| PyMuPDF    | PDF parsing and reading            |
| Streamlit  | (Optional) Frontend UI             |

---


---

## 🧠 How It Works

1. **Upload PDF** – Reads the full text using `PyMuPDF`.
2. **Chunking** – Splits document into overlapping chunks (to preserve context).
3. **Embedding** – Converts text chunks into dense vector embeddings.
4. **Vector Store** – Saves embeddings into FAISS index.
5. **Querying** – Takes user question and retrieves top-k relevant chunks.
6. **Answer Generation** – Sends the chunks + question to OpenAI GPT to generate a response.

---

## ✅ Requirements

- OpenAI API Key 🔑  
- Python 3.x  
- `langchain`, `openai`, `faiss-cpu`, `pymupdf`, `tiktoken`, `python-dotenv`

Install all dependencies:

```bash
pip install -q langchain openai faiss-cpu pymupdf tiktoken python-dotenv

