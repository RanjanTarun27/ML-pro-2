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

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/askmydocs-rag-chatbot.git
cd askmydocs-rag-chatbot
