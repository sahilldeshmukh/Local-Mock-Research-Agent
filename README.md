# 🤖 Local Mock Research Agent: Edge AI Simulation with LangChain & FAISS

This project showcases a fully offline research assistant framework using LangChain with simulated components. It demonstrates how a research agent and answer-generating agent can collaborate on structured knowledge retrieval—without requiring any external API keys or internet access.

---

## 🔍 Project Summary

This prototype simulates how AI agents collaborate to perform research on technical domains—specifically Edge AI—using mock documents and LangChain's `FakeLLM` and `FakeEmbeddings`. The system performs a mini pipeline of ingesting knowledge, indexing, and answering user questions as if it were backed by a real LLM and vector store.

It’s ideal for:
- Teaching LangChain workflows
- Debugging RAG pipelines
- Demonstrating retrieval-based AI agents without cost or API limits

---

## 🧠 Features

- ✨ Modular Research Agent & Answer Drafter
- 🧪 FAISS Vector Store with Fake Embeddings
- 🧱 Chunking via RecursiveCharacterTextSplitter
- 🎭 Uses LangChain’s FakeListLLM to simulate generated answers
- 🔌 No API keys, no external dependencies

---

## 📂 Project Structure


---

## 🚦 How It Works

### 🧩 Step 1: Research Agent

Pulls mock documents related to Edge AI topics like:
- Federated Learning
- TinyML
- AI + 5G integration
These are split into chunks and embedded using fake embeddings.

### 🧠 Step 2: Answer Drafter

Runs a LangChain `RetrievalQA` over the FAISS index, simulating question answering using `FakeListLLM`.

---

## 🚀 Quick Start

1. Clone the repo  
   ```bash
   git clone https://github.com/your-username/mock-edge-ai-agent.git
   cd mock-edge-ai-agent
