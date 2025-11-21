🌟 Indra AI — Intelligent RAG Chatbot (Streamlit + Qdrant + OpenAI)

Indra AI is a powerful, Retrieval-Augmented Generation (RAG) chatbot that combines:

Streamlit UI

OpenAI embeddings + GPT responses

Qdrant vector database

Wikipedia search

PDF, TXT, DOCX document ingestion

Ask questions, upload documents, and get context-aware answers instantly.

✨ Features
🤖 Smart Chat Interface

A modern Streamlit UI with chat bubbles, animation, and memory.

📄 Document Upload & RAG

Upload:

PDF

TXT

DOCX

Indra AI stores chunks in Qdrant Vector DB and retrieves the most relevant context using embeddings.

🌐 Wikipedia Retrieval

Automatically fetches summary from Wikipedia when no documents are uploaded.

🔍 Accurate Similarity Matching

Uses:

sentence-transformers

FAISS / Qdrant similarity search

📦 No Code Changes Needed

Runs “as is” — just install and run.

📁 Project Structure
Indra_AI/
│── rag_backend/
│   ├── app.py               # Main Streamlit App
│   ├── main.py              # Legacy CLI Version (kept for reference)
│   ├── embedder.py
│   ├── generator.py
│   ├── evaluation.py
│   ├── vector.py
│   ├── pdf_loader.py
│   ├── wikipedia_loader.py
│   ├── requirements.txt
│
│── .env.example
│── .gitignore
│── README.md
│── assets/                 # (Create this folder manually)
│    ├── screenshot.png
│    └── demo.gif

🛠️ Installation
Step 1 — Clone the Repository
git clone https://github.com/yourusername/Indra_AI
cd Indra_AI

Step 2 — Create Virtual Environment
python -m venv venv

Step 3 — Activate venv
venv\Scripts\activate     # Windows

Step 4 — Install Dependencies
pip install -r rag_backend/requirements.txt

Step 5 — Configure Environment

Create .env file:

OPENAI_API_KEY=your_real_key_here


Or copy template:

copy .env.example .env


Add your key inside it.

🚀 Run the App
streamlit run rag_backend/app.py


The app opens automatically at:

👉 http://localhost:8501

📸 Screenshots

(Add screenshots in your assets/ folder)

![IndraAI UI](assets/screenshot.png)

🧩 How It Works: RAG Architecture
User Query
    ↓
Wikipedia Fetch (optional)
    ↓
Embedding (OpenAI)
    ↓
Vector Search (Qdrant)
    ↓
Ranked Context
    ↓
GPT-based Answer Generation

🗺️ Roadmap

 Add chat history persistence

 Add support for multiple PDFs

 Support Gemini / Qwen local mode

 Improve UI animations

🧑‍💻 Author

Arshdeep Singh
AI & Machine Learning Engineer
India