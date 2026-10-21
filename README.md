# 📄 DocuMind AI — Chat with Your PDF 🤖

💡 **An AI-powered PDF question-answering application** that lets users upload PDF documents and ask questions about their content using natural language.

## 🌟 Overview

DocuMind AI uses **Retrieval-Augmented Generation (RAG)** to retrieve relevant information from uploaded PDFs and generate context-grounded answers using a locally running Large Language Model (LLM).

## ✨ Features

- 📤 **PDF Upload** — Upload a PDF document for analysis.
- 💬 **Natural Language Q&A** — Ask questions about your document in plain English.
- ✂️ **Text Chunking** — Split extracted text into smaller chunks for efficient retrieval.
- 🧠 **Text Embeddings** — Convert document chunks into vector representations.
- 🔎 **Semantic Search** — Find relevant passages using FAISS.
- 🎯 **MMR Retrieval** — Retrieve relevant and diverse text chunks.
- 🤖 **AI-Powered Answers** — Generate responses using Llama 3.2.
- 📚 **Source References** — View retrieved passages and page numbers when available.
- 🖥️ **Interactive Interface** — Chat with your PDF through Streamlit.
- 🔒 **Local Model Inference** — Run the language model locally through Ollama.

## 🛠️ Tech Stack

| 🧰 Technology | 🎯 Purpose |
|---|---|
| 🐍 Python | Application logic |
| 🎨 Streamlit | Interactive web interface |
| 🔗 LangChain | LLM integration and retrieval pipeline |
| 🦙 Ollama | Run language models locally |
| 🤖 Llama 3.2 | Answer generation |
| 🧠 Nomic Embed Text | Generate text embeddings |
| 🔍 FAISS | Vector similarity search |

## ⚙️ How It Works

1. 📤 **Upload:** Select a PDF document.
2. 📖 **Extract:** Read the text from the PDF.
3. ✂️ **Chunk:** Divide the extracted text into smaller sections.
4. 🧠 **Embed:** Generate vector embeddings using Nomic Embed Text.
5. 🗄️ **Index:** Store the vectors in a FAISS vector store.
6. 🔄 **Rewrite:** Normalize selected question terms using predefined substitutions.
7. 🎯 **Retrieve:** Find relevant chunks using Maximal Marginal Relevance (MMR).
8. 🤖 **Generate:** Pass the retrieved context to Llama 3.2.
9. 📚 **Display:** Show the answer and relevant source passages.

## 📂 Project Structure

```text
📁 documind-ai-rag/
├── 🚀 app.py
├── 🤖 chatbot.py
├── 🧠 embeddings.py
├── 📖 pdf_reader.py
├── 🔄 query_rewriter.py
├── ✂️ text_splitter.py
├── 🔍 vector_store.py
├── 📦 requirements.txt
├── 📘 README.md
└── 🖼️ assets/
```

## 📋 Prerequisites

- 🐍 Python 3.10 or a compatible version supported by the dependencies
- 🦙 Ollama installed
- 🔧 Git

## 🚀 Installation and Setup

### 1️⃣ Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd documind-ai-rag
```

### 2️⃣ Create a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Download the AI models

```bash
ollama pull llama3.2
ollama pull nomic-embed-text
```

### 5️⃣ ▶️ Run the application

Make sure Ollama is running, then execute:

```bash
streamlit run app.py
```

🌐 Open the local URL displayed in your terminal, upload a PDF, and start chatting with your document!

## 🔮 Future Improvements

- 📚 Support multiple PDFs in a single session.
- 🎯 Implement hybrid search and reranking.
- 📥 Add downloadable chat transcripts.
- 💾 Add persistent conversation history.
- 📈 Improve retrieval accuracy and source citations.
- ☁️ Deploy the application through an API or cloud platform.

## 🎓 Learning Outcomes

- 🧩 Understanding Retrieval-Augmented Generation (RAG).
- 🔍 Working with text embeddings and vector similarity search.
- 🤖 Integrating local LLMs using Ollama.
- 🔗 Building retrieval pipelines with LangChain.
- 🎨 Developing interactive AI applications using Streamlit.

---

⭐ **If you find this project useful, consider giving the repository a star!**

