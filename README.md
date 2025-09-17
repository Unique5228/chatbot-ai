# 🏦 Chatbot-AI  

An AI-powered chatbot designed to analyze and answer questions from **banking quarterly/annual reports**.  
Built with **LangChain**, **Vector Databases (FAISS)**, and **Large Language Models (LLMs)**, this chatbot enables financial insights through conversational AI.

---

## 🚀 Features  
- 📄 Extracts and processes financial reports (PDF/CSV)  
- 🔎 Retrieval-Augmented Generation (RAG) for accurate answers  
- 🧠 Integrates with LLMs (OpenAI / HuggingFace)  
- 📊 Summarizes key financial highlights  
- ⚡ Extendable with tools like financial ratio calculators  
- 🌐 Deployable via FastAPI / Streamlit  

---

## 📂 Project Structure  
```
chatbot-ai/
│-- app.py               # Main entry point  
│-- requirements.txt     # Python dependencies  
│-- .env.example         # Example environment variables  
│-- data/                # Place quarterly/annual reports here  
│-- modules/             # Chatbot logic & utility functions  
│-- README.md            # Project documentation  
...
...
...
...

```

---

## 🛠 Setup Instructions  

### 1. Clone the Repository  
```bash
git clone git@github.com:Unique5228/chatbot-ai.git
cd chatbot-ai
```

### 2. Setup Environment Variables  
Copy the example `.env` file and update with your API keys (e.g., `OPENAI_API_KEY`):  
```bash
cp .env.example .env
```

### 3. (Optional) Create a Virtual Environment  
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

### 4. Install Dependencies  
```bash
pip install -r requirements.txt
```

---

## ▶️ Usage  

Run the chatbot:  
```bash
python app.py
```

- If using **Streamlit**:  
```bash
streamlit run app.py
```

- If using **FastAPI**:  
```bash
uvicorn app:app --reload
```

---

## ⚙️ Example Interaction  

```text
User: "What was the net income in Q2 2024?"  
Bot:  "According to the Q2 2024 report, the net income was $1.2B, reflecting a 10% YoY increase."
```

---

## 🔧 Tech Stack  
- [LangChain](https://www.langchain.com/) – framework for LLM applications  
- [FAISS](https://github.com/facebookresearch/faiss) – vector similarity search  
- [OpenAI API](https://platform.openai.com/) or HuggingFace models  
- [PyPDF](https://pypi.org/project/pypdf/) – PDF parsing  
- [Streamlit](https://streamlit.io/) / [FastAPI](https://fastapi.tiangolo.com/) – deployment  

---

## 🔮 Roadmap  
- [ ] Add financial ratio calculator (EPS, P/E, growth rates)  
- [ ] Support multiple vector DBs (Pinecone, Weaviate)  
- [ ] Integrate advanced financial summarization  
- [ ] Dockerize for production deployment  

---

## 🤝 Contributing  
Contributions, issues, and feature requests are welcome!  
Please open a pull request or start a discussion for improvements.  

---

## 📜 License  
This project is licensed under the **MIT License**.  
