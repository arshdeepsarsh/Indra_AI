# 🤖 Indra AI — RAG Chatbot using Streamlit, Qdrant & OpenAI

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-UI-red?logo=streamlit)
![RAG](https://img.shields.io/badge/RAG-Retrieval%20Augmented%20Generation-purple)
![OpenAI](https://img.shields.io/badge/OpenAI-Embeddings-green)
![Vector DB](https://img.shields.io/badge/VectorDB-Qdrant-blue)
![FAISS](https://img.shields.io/badge/VectorSearch-FAISS-orange)
![LLM](https://img.shields.io/badge/LLM-Powered-brightgreen)
![Status](https://img.shields.io/badge/Project-Active-success)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen)


Indra AI is a Retrieval-Augmented Generation (RAG) chatbot that allows users to:

- Ask natural language questions  
- Upload PDF/Text files for context  
- Retrieve Wikipedia summaries  
- Get accurate answers using OpenAI embeddings + vector search  

Built with Streamlit UI, Qdrant Vector DB, and OpenAI embeddings.

---

## 🚀 Features

- RAG-based question answering  
- PDF/Text document support  
- Wikipedia knowledge fetching  
- Vector search using Qdrant/FAISS  
- Clean Streamlit interface  
- Secure `.env` API key handling  

---

## 📁 Project Structure

```
Indra_AI/
│── rag_backend/
│   ├── app.py
│   ├── main.py
│   ├── embedder.py
│   ├── generator.py
│   ├── evaluation.py
│   ├── pdf_loader.py
│   ├── vector.py
│   ├── wikipedia_loader.py
│   ├── requirements.txt
│
├── .env.example
├── .gitignore
├── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/arshdeepsarsh/Indra_AI.git
cd Indra_AI
```

---

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate:

**Windows**
```bash
venv\Scripts\activate
```

**Mac/Linux**
```bash
source venv/bin/activate
```

---

### 3. Install dependencies
```bash
pip install -r rag_backend/requirements.txt
```

---

### 4. Add your API key

Create a `.env` file:

```
OPENAI_API_KEY=your_api_key_here
```

(Or copy from `.env.example`)

---

## ▶️ Run the Application

### Streamlit UI
```bash
streamlit run rag_backend/app.py
```

### CLI Mode
```bash
python rag_backend/main.py
```

---

## 🧠 How It Works (RAG Pipeline)

```
User Query / Document Upload
          ↓
Text Chunking
          ↓
Embedding Generation (OpenAI)
          ↓
Vector Storage (Qdrant / FAISS)
          ↓
Similarity Search
          ↓
Response Generation
```

---

## 🛣️ Roadmap

- Chat history  
- Qwen/Gemini model support  
- Voice input  
- Deployment on Streamlit Cloud  
- Multi-document support  

---

## 🤝 Contributing

Pull requests are welcome.  
Please open an issue to discuss new features or improvements.

---

## License

MIT License

---

## ⭐ Support

If you find this project useful, consider giving it a ⭐ on GitHub!
