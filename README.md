# 📄 PDF RAG Chatbot using Gemini, LangChain & FAISS

A Retrieval-Augmented Generation (RAG) chatbot that answers questions from PDF documents using **Google Gemini 2.5 Flash**, **LangChain**, **Hugging Face Embeddings**, and **FAISS**.

---

## 🚀 Overview

This project demonstrates a simple Retrieval-Augmented Generation (RAG) pipeline for question answering over PDF documents.

Instead of sending the entire document to the language model, the application retrieves only the most relevant text chunks using semantic search and provides them as context to Gemini, resulting in more accurate and context-aware responses.

---

## ✨ Features

- 📄 Supports multiple PDF documents
- ✂️ Automatic document chunking
- 🧠 Hugging Face sentence embeddings
- ⚡ Fast semantic search using FAISS
- 🤖 Answer generation using Gemini 2.5 Flash
- 📚 Displays source PDF names and page numbers
- 💻 Easy to run in Google Colab

---

## 🛠️ Technologies Used

- Python
- Google Colab
- LangChain
- FAISS
- Hugging Face Embeddings
- Google Gemini 2.5 Flash
- PyPDF

---

## 📂 Project Structure

```
PDF-RAG-Chatbot-using-Gemini-LangChain-FAISS/

│── PDF_RAG_Chatbot_Gemini.ipynb
│── README.md
```

---

## 🔄 Workflow

```
                PDF Documents
                      │
                      ▼
              Load PDF Documents
                      │
                      ▼
             Split into Text Chunks
                      │
                      ▼
         Generate Hugging Face Embeddings
                      │
                      ▼
            Store Vectors in FAISS
                      │
                      ▼
                User Question
                      │
                      ▼
         Retrieve Relevant Chunks
                      │
                      ▼
             Gemini 2.5 Flash
                      │
                      ▼
        Answer with Source Citations
```

---

## 🚀 Installation

Install the required libraries:

```bash
pip install langchain
pip install langchain-community
pip install langchain-google-genai
pip install langchain-huggingface
pip install langchain-text-splitters
pip install faiss-cpu
pip install sentence-transformers
pip install pypdf
```

---

## 🔑 Gemini API Key

Get a free Gemini API key from **Google AI Studio**.

https://aistudio.google.com/app/apikey

Run the following code:

```python
import os
from getpass import getpass

os.environ["GOOGLE_API_KEY"] = getpass("Enter your Gemini API Key: ")
```

---

## ▶️ How to Run

1. Clone this repository.
2. Open the notebook in Google Colab.
3. Install the required dependencies.
4. Enter your Gemini API key.
5. Upload your own PDF documents.
6. Run all notebook cells.
7. Ask questions about the uploaded PDFs.

---

## 💬 Example Questions

- What is Retrieval-Augmented Generation?
- Explain self-attention.
- Summarize the uploaded document.
- What are the advantages of RAG?
- What are the limitations discussed in the paper?
- Compare the ideas presented in the uploaded PDFs.

---

## 📷 Sample Output

```
Question:
What are the advantages of RAG?

Answer:
RAG improves factual accuracy by retrieving relevant
information from external documents before generating
responses.

Sources:
paper1.pdf | Page 8
paper2.pdf | Page 10
```

---

## 📚 Learning Outcomes

This project helped me understand:

- Retrieval-Augmented Generation (RAG)
- PDF document loading and processing
- Text chunking
- Sentence embeddings
- Vector databases with FAISS
- Semantic similarity search
- Prompt engineering
- Integrating LangChain with Google Gemini

---

## 🔮 Future Improvements

- Conversation memory
- Persistent vector databases
- Streamlit or Gradio web interface
- Hybrid search (vector + keyword search)
- Support for more document formats
- Metadata-based filtering
- Multi-document comparison

---

## 📄 Note

This repository does **not** include PDF documents.

You can upload your own PDFs or use publicly available research papers (for example, from arXiv) to test the chatbot.

---

## 👩‍💻 Author

**Geethika**

This project was built as part of my learning journey in **Generative AI, Large Language Models (LLMs), Retrieval-Augmented Generation (RAG), and LangChain**.

---
⭐ If you found this project useful, consider giving it a star!
