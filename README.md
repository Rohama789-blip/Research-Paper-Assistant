# 📚 Research Paper Assistant

<div align="center">

# 🤖 Research Paper Assistant

### RAG-powered AI assistant for research papers

**FastAPI • LangChain • LangGraph • LangSmith • Groq • PyPDF • PDFPlumber**

</div>

---

## 🎬 Demo

> Add your application screen-recording GIF here.

![Research Paper Assistant Demo](demo.gif)

---

## ✨ Overview

Research Paper Assistant is a Retrieval-Augmented Generation (RAG) application that allows users to upload one or multiple research papers in PDF format and ask questions about them.

The assistant retrieves relevant information from the uploaded documents before generating an answer.

The application is designed to answer **only from the uploaded research papers**.

If the required information is not found, it responds:

> The answer is not available in the uploaded documents.

---

## 🚀 Features

- 📄 Upload one or multiple research papers
- 🔍 Retrieve relevant document chunks
- 🤖 AI-generated answers using Groq
- 🧠 Retrieval-Augmented Generation
- 🔗 LangChain integration
- 🕸️ LangGraph workflow
- 📊 Optional LangSmith tracing
- 📑 Document-level source information
- 📃 Page number references
- ⚠️ Unsupported file validation
- 💬 Interactive chat interface
- 🧹 Clear uploaded documents
- 📱 Responsive UI
- ✨ Animated modern interface

---

# 🏗️ Architecture

```text
                 ┌─────────────────────┐
                 │    PDF Upload       │
                 └──────────┬──────────┘
                            │
                            ▼
                ┌──────────────────────┐
                │ PyPDF / PDFPlumber   │
                │   Text Extraction    │
                └──────────┬───────────┘
                           │
                           ▼
                ┌──────────────────────┐
                │ LangChain Text       │
                │      Splitter        │
                └──────────┬───────────┘
                           │
                           ▼
                ┌──────────────────────┐
                │   TF-IDF Retrieval   │
                │ Cosine Similarity    │
                └──────────┬───────────┘
                           │
                    User Question
                           │
                           ▼
                ┌──────────────────────┐
                │ Relevant PDF Chunks  │
                └──────────┬───────────┘
                           │
                           ▼
                ┌──────────────────────┐
                │      LangGraph       │
                │   Generate Node      │
                └──────────┬───────────┘
                           │
                           ▼
                ┌──────────────────────┐
                │      Groq LLM        │
                └──────────┬───────────┘
                           │
                           ▼
              ┌─────────────────────────┐
              │ Answer + Source Pages  │
              └─────────────────────────┘