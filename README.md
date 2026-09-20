📚 Advanced RAG Chatbot

An intelligent Retrieval-Augmented Generation (RAG) application that enables users to upload a PDF document, ask natural language questions, generate AI-powered document summaries, and explore document chunks through an interactive interface.

Built using Python, LangChain, FAISS, Sentence Transformers, Groq Llama-3, and Streamlit, this project demonstrates an end-to-end RAG pipeline with a clean user experience and modular architecture.

---

🚀 Features

📄 PDF Upload

- Upload a PDF document through an intuitive interface.
- Displays uploaded file name and file size.

⚡ Intelligent Processing Pipeline

The application processes every uploaded PDF using multiple stages:

- PDF Loading
- Text Chunking
- Embedding Generation
- FAISS Vector Store Creation
- Retrieval Initialization

A live progress indicator keeps users informed throughout the processing workflow.

---

📊 Document Statistics

Displays useful information immediately after processing:

- Total Pages
- Total Chunks
- Embedding Model
- Vector Database
- LLM Model
- Processing Time

---

💬 AI Chat with PDF

Ask questions in natural language.

The system:

- Retrieves relevant document chunks
- Builds contextual prompts
- Generates accurate answers using Groq Llama-3
- Maintains short-term conversation memory
- Displays document sources used for every answer

---

📄 AI Document Summary

Generate an AI-powered summary of the uploaded document.

The summary includes:

- Overview
- Key Points
- Important Information
- Conclusion

---

🧩 Chunk Explorer

Explore how the document is divided internally.

For every chunk, the application displays:

- Chunk NumberS
- Page Number
- Character Count
- Word Count
- Complete Chunk Content

This feature helps users understand the internal working of Retrieval-Augmented Generation.

---

📚 Source Citation

Every generated answer includes document source information to improve transparency.

---

💾 FAISS Index Caching

Previously processed documents automatically reuse stored FAISS indexes, reducing processing time significantly.

---

🧠 Conversation Memory

Maintains recent conversation history to improve follow-up questions without requiring a database.

---

🏗 Project Architecture

                User Uploads PDF
                        │
                        ▼
                 PDF Loader
                        │
                        ▼
            Recursive Text Splitter
                        │
                        ▼
         Sentence Transformer Embeddings
                        │
                        ▼
             FAISS Vector Database
                        │
                        ▼
        Similarity Retrieval (MMR Search)
                        │
                        ▼
      Groq Llama-3.3-70B Large Language Model
                        │
                        ▼
      AI Answer / Summary / Source Citation

---

🛠 Tech Stack

Programming Language

- Python

Framework

- Streamlit

LLM

- Groq API
- Llama-3.3-70B Versatile

RAG Framework

- LangChain

Embedding Model

- all-MiniLM-L6-v2

Vector Database

- FAISS

PDF Processing

- PyPDF Loader

Chunking

- Recursive Character Text Splitter

---

📂 Project Structure

Advanced-RAG-Chatbot/

│
├── app.py
│
├── services/
│   ├── pdf_loader.py
│   ├── text_splitter.py
│   ├── embeddings.py
│   ├── vector_store.py
│   ├── rag_pipeline.py
│   └── llm.py
│
├── uploads/
├── indexes/
│
├── requirements.txt
└── README.md

---

⚙ Workflow

1. Upload a PDF document.
2. Load and split the document into chunks.
3. Generate embeddings using Sentence Transformers.
4. Store embeddings in FAISS.
5. Retrieve relevant chunks using similarity search.
6. Generate answers with Groq Llama-3.
7. Display retrieved document sources.
8. Generate document summaries.
9. Explore document chunks.

---

✨ Key Highlights

- End-to-End Retrieval-Augmented Generation Pipeline
- Clean Modular Code Structure
- Interactive Streamlit Interface
- AI Document Summary
- Chunk Explorer
- Processing Progress Indicators
- Document Statistics Dashboard
- Source Citation
- Session-Based Conversation Memory
- Cached FAISS Indexing
- Efficient Similarity Retrieval
- Scalable Service-Based Architecture

---

💡 Future Improvements

- Multi-document Retrieval
- OCR Support for Scanned PDFs
- Hybrid Search (Dense + Keyword)
- Metadata Filtering
- Citation Highlighting
- Multi-language Document Support
- Export Chat History
- User Authentication

---

🎯 Learning Outcomes

This project demonstrates practical understanding of:

- Retrieval-Augmented Generation (RAG)
- LangChain Pipelines
- Vector Databases
- Embedding Models
- Semantic Search
- Prompt Engineering
- Large Language Models
- Streamlit Application Development
- Modular Python Architecture
- AI Application Deployment

---

📸 Screenshots

Add screenshots of:

- Home Page
- PDF Upload
- Processing Progress
- Document Statistics
- AI Chat
- AI Summary
- Chunk Explorer

---

🚀 Installation

git clone <repository-url>

cd Advanced-RAG-Chatbot

pip install -r requirements.txt

streamlit run app.py

---

👨‍💻 Author

Yuvaraj Kushwaha

B.Tech Computer Science Engineering

Passionate about Generative AI, Retrieval-Augmented Generation (RAG), Large Language Models, and AI Application Development.

---

⭐ If you found this project useful, consider giving it a Star on GitHub!