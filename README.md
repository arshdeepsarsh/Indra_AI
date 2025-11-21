🌟 Indra AI — Intelligent RAG Chatbot (Streamlit + Qdrant + OpenAI)

Your all-in-one intelligent assistant powered by Retrieval-Augmented Generation (RAG).
Ask questions, upload documents, fetch Wikipedia context — Indra AI understands and answers with precision.

<div align="left">












</div>
🚀 Overview

Indra_AI is a Retrieval-Augmented AI Chatbot that allows users to:

✔ Ask natural questions
✔ Upload PDF/TXT/DOCX files
✔ Retrieve intelligent context using Qdrant Vector Search
✔ Automatically fetch Wikipedia summaries
✔ Generate accurate answers using OpenAI embeddings

This project demonstrates full-stack AI engineering with embeddings, vector databases, and LLM-based reasoning — built entirely in Python.

🎯 Features
🤖 Smart Conversational Chat

Elegant Streamlit UI with natural conversation flow.

📚 RAG Document Question-Answering

Upload documents → They are chunked, embedded & indexed in Qdrant.

🌐 Wikipedia Summaries

When no documents are available, Indra AI fetches context automatically.

⚡ Fast Vector Search

Powered by:

sentence-transformers

Qdrant-client

FAISS CPU

🔐 Secure API Usage

.env file supported (key not exposed in repo).
.env.example template provided.

📦 Zero-Code Setup

Clone → Install → Run.

🗂️ Project Structure
Indra_AI/
│── rag_backend/
│   ├── app.py               # Streamlit main app
│   ├── main.py              # Legacy CLI version
│   ├── embedder.py
│   ├── generator.py
│   ├── evaluation.py
│   ├── vector.py
│   ├── wikipedia_loader.py
│   ├── pdf_loader.py
│   ├── requirements.txt
│
│── .env.example
│── .gitignore
│── README.md
│── venv/
│── assets/  (optional)
│    ├── screenshot.png
│    └── demo.gif

🔧 Installation
1️⃣ Clone the Repository
git clone https://github.com/arshdeepsarsh/Indra_AI.git
cd Indra_AI

2️⃣ Create Virtual Environment
python -m venv venv

3️⃣ Activate

Windows:

venv\Scripts\activate

4️⃣ Install Dependencies
pip install -r rag_backend/requirements.txt

5️⃣ Add API Key

Create .env:

OPENAI_API_KEY=your_key_here

▶️ Run the App
streamlit run rag_backend/app.py


The chatbot will open at:

👉 http://localhost:8501

📸 Screenshots

(Upload your screenshot into /assets/screenshot.png and update below)

![IndraAI UI](assets/screenshot.png)

🔬 How It Works (RAG Pipeline)
User Query/Document
         ↓
Embedding Generation (OpenAI)
         ↓
Vector Indexing (Qdrant)
         ↓
Context Retrieval (FAISS Similarity)
         ↓
LLM Answer Generation (ChatCompletion)


This hybrid approach ensures:

✔ High accuracy
✔ Context-aware responses
✔ Faster answer generation

📌 Roadmap

 Add multi-document support

 Add conversational memory

 Add Gemini/Qwen local support

 Add history saving

 Deploy online (Streamlit Cloud / HuggingFace Spaces)

🤝 Contributing

Pull requests welcome!
Please open an issue for feature requests.

🧑‍💻 Author

Arshdeep Singh
AI & Software Engineering Enthusiast

📜 License

This project is under the MIT License.

🌟 If you like this project → Give it a STAR ⭐ on GitHub!
