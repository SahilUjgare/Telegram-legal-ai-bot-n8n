# 🤖 Telegram Legal AI Bot (n8n + OpenAI + Pinecone)

A Telegram-based AI chatbot built using **n8n**, **OpenAI**, and **Pinecone Vector Store**.  
The bot answers **Indian Penal Code (IPC)** and legal-related questions using a **Retrieval-Augmented Generation (RAG)** approach.

---

## 🚀 Features

- 📩 Telegram chatbot integration using n8n
- 🧠 AI Agent powered by OpenAI Chat Models
- 📚 Context-aware responses via Pinecone Vector Store
- ☁️ Automatic document ingestion from Google Drive
- 💾 Conversation memory for better responses
- 🔄 Fully automated no-code workflows

---

## 🏗️ Architecture

### Telegram Bot Workflow
Telegram messages are processed by an AI Agent which retrieves relevant legal context from Pinecone before responding.

![Telegram AI Bot Workflow](assets/telegram-ai-bot-workflow.png)

Telegram Trigger
↓
AI Agent (OpenAI)
↓
Pinecone Vector Store
↓
Telegram Send Message


---

### Data Ingestion Workflow
Legal documents uploaded to Google Drive are automatically embedded and stored in Pinecone.

![Data Ingestion Workflow](assets/data-ingestion-pinecone-workflow.png)

Google Drive Trigger
↓
Download File
↓
Default Data Loader
↓
Recursive Text Splitter
↓
OpenAI Embeddings
↓
Pinecone Vector Store


---

## 💬 Telegram Bot Demo

Live example of the bot answering IPC-related queries on Telegram.

![Telegram Bot Chat Demo](assets/telegram-bot-chat-demo.png)

---

