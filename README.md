# 🤖 ChatWithDocs – AI-Powered Document Assistant

ChatWithDocs is an intelligent chatbot that allows users to converse with structured documents as if they were speaking to a human expert. Built using **LlamaIndex**, **Google Gemini Embeddings**, and **Gradio**, it enables multilingual support, contextual understanding, and real-time response generation.


![Built with LlamaIndex](https://img.shields.io/badge/Built%20with-LlamaIndex-blueviolet?style=for-the-badge)
![Powered by Gemini](https://img.shields.io/badge/Powered%20by-Google%20Gemini-ff6c37?style=for-the-badge)

## 📌 Features

- 🔍 **Document Search**: Ingests `.txt`, `.pdf`, and other files from the `/Docs` folder
- 🧠 **Semantic Understanding**: Uses Google’s `text-embedding-004` to embed content
- 💬 **Contextual Responses**: Generates accurate, relevant answers using Gemini LLM
- 🌍 **Multilingual**: Supports queries in multiple languages
- 🖥️ **Gradio UI**: Clean, minimal interface to interact with the chatbot


## 🛠️ Tech Stack

| Technology     | Purpose                                   |
|----------------|--------------------------------------------|
| Python (Jupyter) | Core development                         |
| LlamaIndex     | Chunking, indexing, querying documents     |
| GoogleGenAI (Gemini) | Embedding + LLM response generation |
| Gradio         | Frontend/chat interface                    |


## 📂 Folder Structure

```bash 
📁 ChatWithDocs/
┣ 📁 Docs/ → Place your input documents here
┣ 📁 Storage/ → Auto-generated vector index and metadata
┣ 📁 Code/ → Contains all notebook (chat + UI)
┣ 📄 .env → Stores your Gemini API key securely
┣ 📄 README.md
┗ 📄 requirements.txt
```

## ⚙️ Setup Instructions

> 📌 Prerequisites: Python 3.9+, Google Cloud API key (Gemini access), pip

1. **Clone the Repo**
```bash
git clone https://github.com/G-Pavithran-dev/ChatWithDocs.git
cd ChatWithDocs
```

2. **Create a Virtual Environment**

- Option A : Using `venv` (Recommended for Python Environment)
 ```bash
python -m venv venv
venv\Scripts\activate
```
- Option B : Using `Condo`
```bash
conda create --name chatwithdocs python=3.10 -y
conda activate chatwithdocs
```

3. **Install Requirements**
```bash
pip install -r requirements.txt
```

4. **Configure API Key**
Create a ```.env``` file in the root directory:
```ini
GOOGLE_GENAI_API_KEY=your_google_gemini_api_key_here
```

5. **Launch the Application**
- Run the notebook ```indexing.ipynb``` which reads files and creates index
- Then, Run the notebook ```chat_bot.ipynb``` which contains the actual chat_bot logics

## 🎓 Additional Use Case - Academic Productivity
Students can upload their course materials (notes, textbooks, guidelines) and ask questions directly. The chatbot responds with accurate, context-aware replies in their preferred language — making learning faster and more accessible.

## 📬 Connect with me
Made with ❤️ by ```Pavithran G``` 

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/g-pavithran)  

If you found this project helpful, ⭐ the repo!
