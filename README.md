# CTSE_ChatBot

📘 CTSE Chatbot – Lecture Notes Question Answering System
This project is an intelligent chatbot designed to answer questions based on the content of a given lecture PDF (e.g., CTSE.pdf). It uses LangChain, Hugging Face Transformers, and FAISS to process the document, generate embeddings, retrieve relevant content, and generate accurate answers.

✨ Key Features
📄 PDF Loader – Parses lecture notes using PyPDFLoader.

✂️ Text Chunking – Splits content into manageable chunks for better processing.

🧠 Embeddings with MiniLM – Uses all-MiniLM-L6-v2 for semantic search.

🔍 FAISS Vector Store – Efficient document retrieval with similarity search.

💬 Flan-T5 Based LLM – Answers are generated with the lightweight google/flan-t5-small model.

❌ Hallucination Prevention – Skips answers when relevant content is missing.

🛠️ Error Handling & Logging – Logs weak or unanswered queries to incorrect_answers.log.

🧪 How It Works
Loads and parses the lecture PDF.

Splits the text into overlapping chunks.

Converts chunks into embeddings and stores them in FAISS.

Accepts user queries via a command-line interface.

Retrieves relevant content and generates an answer.

If no relevant content is found, the bot politely declines to answer.

🚀 Technologies Used
Python

LangChain

HuggingFace Transformers

FAISS

PyPDFLoader

Flan-T5 Small (via transformers.pipeline)
