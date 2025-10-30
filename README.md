# ChatBot-Using-Langchain
This project is a LangChain-powered chatbot that allows users to ask questions about a PDF document and receive intelligent, context-aware answers. It uses Ollama LLMs (like LLaMA2 or Mistral), FAISS vector search, and custom prompt engineering to deliver concise responses based on retrieved document chunks.

---

## 🧠 Features

- 📄 PDF ingestion using `PyPDFLoader`
- ✂️ Text chunking with `RecursiveCharacterTextSplitter`
- 🧠 Embeddings via `OllamaEmbeddings` (supports local LLMs)
- 🔍 Semantic search using FAISS vector store
- 🗣️ Response generation using `Ollama` or `OpenAI`
- 🧾 Custom prompt template for concise answers
- 🧪 LangChain Tracing enabled for debugging

---

## 🛠️ Tech Stack

| Component        | Tool/Library                  |
|------------------|-------------------------------|
| LLM              | Ollama (LLaMA2 / Mistral)     |
| Framework        | LangChain                     |
| Embeddings       | OllamaEmbeddings              |
| Vector Store     | FAISS                         |
| PDF Loader       | PyPDFLoader                   |
| Prompt Template  | ChatPromptTemplate            |
| Environment      | Python + `.env` config        |

---

## 📁 Project Structure

├── main.py # Entry point for chatbot
├── Job Description.pdf # Sample document to query
├── .env # API keys and config 
├── requirements.txt # Dependencies


---

## 🚀 Getting Started

1. Clone the repository**
git clone https://github.com/your-username/langchain-pdf-chatbot.git

cd langchain-pdf-chatbot

2. Install dependencies
pip install -r requirements.txt

3. Configure environment variables
Create a .env file in the root directory and add:
LANGCHAIN_API_KEY=your_langchain_api_key

4.Run the chatbot
python main.py


🧪 Sample Usage
query = "How many total items are there?"
answer = ask_question(query)
print(answer)

