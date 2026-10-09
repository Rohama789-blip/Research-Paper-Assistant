# 📚 Research Paper Assistant

An AI-powered Research Paper Assistant that helps users upload PDF research papers, extract their content, and ask questions based on the uploaded documents using Retrieval-Augmented Generation (RAG).

## 🚀 Features

- 📄 Upload research papers in PDF format.
- 📝 Extract text from PDF documents.
- ✂️ Split extracted text into manageable chunks.
- 🔍 Retrieve relevant information from uploaded documents.
- 🤖 Ask questions and get context-based answers.
- 📊 View document processing statistics.
- 🌐 Simple web interface powered by FastAPI.

## 🛠️ Tech Stack

- **Python** — Core programming language
- **FastAPI** — Backend API framework
- **HTML, CSS, JavaScript** — Frontend
- **RAG (Retrieval-Augmented Generation)** — Document-based question answering
- **PDF Processing** — Text extraction from research papers

## 📁 Project Structure

```text
Research-Paper-Assistant/
├── backend/
│   ├── pdf_processor.py
│   └── rag.py
├── static/
│   ├── style.css
│   └── script.js
├── templates/
│   └── index.html
├── main.py
├── requirements.txt
├── .gitignore
└── README.md
```

*Note: The structure may vary depending on your implementation.*

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Rohama789-blip/Research-Paper-Assistant.git
```

### 2. Navigate to the Project Directory

```bash
cd Research-Paper-Assistant
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the Application

```bash
uvicorn main:app --reload
```

### 6. Open in Your Browser

Visit:

http://127.0.0.1:8000

## 💡 How It Works

1. Upload a research paper in PDF format.
2. The application extracts text from the document.
3. The extracted text is divided into chunks.
4. The RAG pipeline retrieves relevant content for a question.
5. The application returns an answer based on the retrieved content.

## 🎯 Project Objective

The goal of this project is to make research papers easier to understand and explore by enabling users to ask questions directly from their uploaded documents.

## 🔮 Future Improvements

- Support for multiple document formats.
- Improved semantic search using vector embeddings.
- Source citations with page numbers.
- Conversation history.
- Enhanced answer generation using an LLM.
- Improved document management.


## 📄 License

This project is available for educational and research purposes. Add a specific open-source license if you intend to distribute it under one.
