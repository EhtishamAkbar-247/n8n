# 🚀 AI-Powered Automation Workflows (n8n)

A collection of production-ready, automated AI agents and workflows built using **n8n**, **Google Gemini**, and **Pinecone vector stores** to optimize daily communication, content processing, and information retrieval.

---

## 📬 Project 1: AI Gmail Auto-Responder

An intelligent, self-hosted email management agent that acts as an automated copywriter assistant. It analyzes incoming emails, categorizes them, and draft contextually accurate responses automatically.

### 🌟 Key Features
* **Automated Triage:** Instantly monitors incoming messages via an n8n Gmail webhook trigger.
* **Context-Aware Replies:** Utilizes advanced LLMs to draft tailored, human-like responses based on the email's intent.
* **Review-Ready Drafts:** Saves the generated response directly to your Gmail drafts folder so you can review and click send.

### 🛠️ Tech Stack
* **Workflow Engine:** n8n
* **AI Model:** Google Gemini
* **Integrations:** Gmail API

---

## 📝 Project 2: Smart Gmail Summarizer & RAG Pipeline

A robust Retrieval-Augmented Generation (RAG) pipeline designed to extract, split, embed, and store massive documents (such as PDFs and email attachments) into a vector database for instant knowledge retrieval.

### 🌟 Key Features
* **Automated Document Ingestion:** Listens for new file creation events via a Google Drive Trigger.
* **Advanced Content Chunking:** Uses a **Recursive Character Text Splitter** nested within a Default Data Loader to cleanly slice large, multi-page PDFs (tested up to 125+ pages) into highly accurate semantic chunks.
* **Vector Embeddings:** Generates high-dimensional vector embeddings using the **Google Gemini Embeddings** model.
* **Vector Storage:** Streams and indexes processed chunks into a **Pinecone Vector Store** under dedicated namespaces (e.g., `FAQ`) for lightning-fast semantic search.

### 🛠️ Tech Stack
* **Workflow Engine:** n8n (Modern LangChain Nodes)
* **Embedding Model:** Google Gemini Embeddings
* **Vector Database:** Pinecone
* **Storage & Extraction:** Google Drive, PDF Extract

---

## 🚀 Getting Started

### Prerequisites
* A self-hosted or cloud instance of **n8n**
* Google AI Studio API Key (for Gemini embeddings)
* Pinecone API Key and an active Index
* Google Cloud Console OAuth credentials (for Gmail & Google Drive triggers)

