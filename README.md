# Medical-Assistant-Chatbot
🩺 Medical Assistant Chatbot (RAG-based)  The Medical Assistant Chatbot is an AI-powered healthcare support system designed to provide reliable, quick, and context-aware medical information. It uses Retrieval-Augmented Generation (RAG) to combine Large Language Models (LLMs) with a curated medical knowledge base.

An AI-powered **medical assistant chatbot** built with **LangChain, Groq LLMs, Pinecone, and HuggingFace embeddings**.  
The chatbot can process **medical PDFs**, generate embeddings, store them in a vector database, and perform **retrieval-augmented generation (RAG)** for accurate question answering.  

---

## 📌 Features  
- 📄 **PDF ingestion** using `PyPDFLoader` / `DirectoryLoader`  
- ✂️ **Text chunking** with `RecursiveCharacterTextSplitter`  
- 🔎 **Vector search** powered by **Pinecone**  
- 🧠 **Embeddings** with HuggingFace models  
- ⚡ **LLM inference** using **Groq**  
- 🔗 **Retrieval chain** via LangChain  
- 🌐 **Flask API** for deployment  

---

## 📂 Project Structure 
Medical-Assistant-Chatbot/
│── research/ # Jupyter notebooks for experimentation
│ └── trials.ipynb
│── app/ # Flask application (if separated)
│── .env # Environment variables (not tracked in Git)
│── requirements.txt # Python dependencies
│── .gitignore # Ignored files
│── README.md # Project documentation


---

## ⚙️ Installation  

### 1️⃣ Clone the repository  
```bash
git clone https://github.com/akshay-aiml/Medical-Assistant-Chatbot.git
cd Medical-Assistant-Chatbot

2️⃣ Setup virtual environment
python -m venv .venv
source .venv/bin/activate   # On Linux/Mac
.venv\Scripts\activate      # On Windows

3️⃣ Install dependencies
pip install -r requirements.txt

🔑 Environment Variables

Create a .env file in the project root with:
PINECONE_API_KEY=your_pinecone_api_key
GROQ_API_KEY=your_groq_api_key

(Keep .env private and never commit it to GitHub)

🚀 Usage
Run Jupyter Notebook
jupyter notebook research/trials.ipynb

🛠️ Tech Stack

LangChain → Document processing & RAG
HuggingFace → Sentence embeddings
Pinecone → Vector database
Groq → LLM for inference

📖 Example Workflow

Upload and parse medical PDFs
Split text into chunks
Embed chunks using HuggingFace models
Store vectors in Pinecone
Query chatbot → Retrieve relevant chunks → Generate AI-powered response

