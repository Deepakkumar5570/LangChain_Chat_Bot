# 📚 Multi-Document RAG Chatbot with Gemini  

An AI-powered chatbot that leverages **Retrieval-Augmented Generation (RAG)** to answer queries from multiple PDF and text documents. Built with **LangChain**, **Google Gemini API**, and **ChromaDB** for embeddings and retrieval.  

This project allows you to upload a collection of documents (research papers, books, notes, etc.) and interact with them conversationally through an intelligent assistant.  

---

## ✨ Features  

- 🔍 **Multi-document support** (PDFs & text files)  
- ⚡ **RAG-based retrieval** for precise, context-aware answers  
- 🤖 Powered by **Gemini API** for natural responses  
- 💾 Persistent **ChromaDB vector storage** for embeddings  
- 📑 Preprocessing with **chunking** for better semantic search  
- 🖥️ **Streamlit UI** with chat-style interface  
- 🔄 Easy **rebuild script** to refresh embeddings when adding new documents  

---

## 📂 Project Structure  

```bash
rag-multidoc-chatbot/
│── data/
│   ├── pdfs/           # place your PDF documents here
│   ├── txts/           # place your TXT documents here
│── chroma_db/          # auto-generated vector database
│── src/
│   ├── __init__.py
│   ├── config.py       # API keys, model configs
│   ├── data_loader.py  # load PDFs & TXTs
│   ├── preprocess.py   # split & clean documents
│   ├── embed_store.py  # create/load vectorstore
│   ├── chatbot.py      # LangChain + Gemini pipeline
│   ├── app.py          # Streamlit app
│── rebuild_db.py       # script to rebuild embeddings
│── requirements.txt    # dependencies
│── .env                # environment variables (API keys, etc.)

```

## How To Use 

- Clone the repository
-     git clone https://github.com/Deepakkumar5570/rag-multidoc-chatbot.git
      cd rag-multidoc-chatbot
  
 ##  Create & activate a virtual environment
       python -m venv venv
       source venv/bin/activate   # Mac/Linux
       venv\Scripts\activate      # Windows
## Install dependencies
       pip install -r requirements.txt

 ## Set up environment variables
 Create a .env file in the root directory:
 
      GEMINI_API_KEY=your_gemini_api_key_here
## Usage
start the chatbot 

        streamlit run src/app.py
## Rebuild the database (after adding new documents)
        python rebuild_db.py
##  📘 Dataset Used

Currently trained on:

  - 30+ Project Gutenberg books

  - 50+ Research papers

  - 15+ Miscellaneous text documents

You can extend by dropping more PDFs or TXTs into:

   - data/pdfs/

  -  data/txts/

##  Roadmap
  -  Add support for DOCX & HTML documents
  -  Advanced metadata filtering (author, year, category)

  - UI for uploading documents directly

  - Evaluation pipeline for RAG performance

       



---

⚡ Pro Tip: If you add **screenshots or demo GIFs** in a `docs/` folder and reference them in the README, your repo will look extra professional.  

Do you want me to also create a **Demo section** in this README with placeholders for screenshots/GIFs?





