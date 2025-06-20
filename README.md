# 🤖 Chat with PDF using Gemini Flash 2.0 + LlamaIndex + ChromaDB

Build an intelligent, privacy-friendly AI assistant that can read and answer questions from any PDF using a local RAG (Retrieval-Augmented Generation) pipeline.

No OpenAI or paid APIs — fully powered by **Gemini Flash 2.0**, **LlamaIndex**, and **ChromaDB**.

---

## 🚀 Features

- 📄 Upload any PDF document
- 🔍 Embed and search document context locally using **ChromaDB**
- 💡 Ask questions and get instant, smart answers via **Gemini Flash 2.0**
- ⚡ FastAPI backend + Streamlit front-end
- 🔐 Your PDF never gets sent to Gemini — only the relevant chunks do

---

## 🧠 How It Works

1. You upload a PDF via the Streamlit interface.
2. The text is extracted and split into small chunks.
3. Each chunk is converted into vector embeddings and stored in ChromaDB.
4. When you ask a question:
   - It’s converted into an embedding.
   - The top matching chunks are retrieved locally.
   - These chunks + your question are sent to **Gemini Flash 2.0**.
5. Gemini responds with an answer based only on the selected context.

---

## 🛠️ Tech Stack

- **Python**
- **Gemini Flash 2.0 API** (`google-generativeai`)
- **LlamaIndex**
- **ChromaDB**
- **FastAPI**
- **Streamlit**
- **PyMuPDF / PyPDF2**

---

## 📦 Installation

```bash
git clone https://github.com/your-username/chat-with-pdf-gemini.git
cd chat-with-pdf-gemini
pip install -r requirements.txt
