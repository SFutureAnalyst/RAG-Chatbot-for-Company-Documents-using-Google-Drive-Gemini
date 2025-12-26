# RAG-Chatbot-for-Company-Documents-using-Google-Drive-Gemini

A fully automated Retrieval-Augmented Generation (RAG) chatbot built using n8n, Google Drive, Gemini Embeddings, and Pinecone Vector Database to provide accurate, context-aware answers from company documents.
![rag](https://github.com/user-attachments/assets/c8c6180f-1178-4aeb-9a2d-b44a371961af)


## 🚀 Project Overview
This project implements an intelligent RAG-based chatbot that retrieves information from company documents stored in Google Drive. The system automatically ingests documents, generates embeddings, stores them in Pinecone, and uses AI models to answer user queries based on relevant retrieved context.

The entire workflow is orchestrated using n8n, enabling a no-code/low-code automation approach suitable for enterprise knowledge management.

## 🎯 Key Features

📂 Automatic document ingestion from Google Drive <br>
✂️ Text extraction and chunking<br>
🧠 Semantic embeddings using Google Gemini<br>
⚡ Fast similarity search with Pinecone<br>
💬 Conversational chatbot interface<br>
🔄 Real-time updates when documents change<br>
🧩 Fully modular n8n workflow<br>

## 🏗 System Architecture

Google Drive
     ↓
Text Loader → Text Splitter → Gemini Embeddings
     ↓
Pinecone Vector Database
     ↓
Query Embedding → Semantic Retrieval
     ↓
AI Agent (LLM)
     ↓
Final Answer to User

## 🧩 Workflow Modules

1. Google Drive Trigger – Detects new file uploads
2. File Download – Downloads uploaded documents
3. Text Extraction Module – Loads document content
4. Text Splitter – Splits content into chunks
5. Gemini Embedding Module – Converts text to vectors
6. Pinecone Vector Store (Insert) – Stores embeddings
7. Chat Trigger – Receives user queries
8. Pinecone Retrieval Tool – Finds relevant chunks
9. AI Agent + LLM – Generates final response

## 🔧 Requirements
## Software <br>
n8n (Self-hosted or Cloud)<br>
Docker Desktop (Recommended)<br>
Web Browser (Chrome / Edge)<br>
APIs & Services<br>
Google Drive API<br>
Google Gemini API<br>
Pinecone API<br>
OpenRouter API (optional)<br>
