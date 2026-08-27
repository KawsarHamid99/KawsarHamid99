<h1 align="center">Kawsar Hamid</h1>

<p align="center">
  <b>AI / ML Engineer — Agentic Systems, LLM Applications & RAG</b><br>
  MS in Artificial Intelligence (in progress) · University of the Cumberlands, USA<br>
  New York, USA
</p>

<p align="center">
  <a href="https://linkedin.com/in/YOUR-LINKEDIN"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:kawsarhamid7225@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://careerfitai.onrender.com"><img src="https://img.shields.io/badge/Live_Demo-CareerFitAI-16A34A?style=flat-square" alt="Live demo"></a>
  <a href="https://github.com/KawsarHamid99"><img src="https://img.shields.io/github/followers/KawsarHamid99?label=Follow&style=flat-square&logo=github" alt="Follow"></a>
</p>

---

## About

I build **LLM-powered applications and multi-agent systems** — retrieval pipelines, tool-using agents, and the backends that make them deployable.

I came to AI from backend engineering, and that shapes how I build. My agents run on typed state graphs with durable checkpointing, my retrieval systems are built to be measured rather than demoed, and my projects ship with tests, CI, and a public URL. The interesting problems in this field aren't in the model call — they're in retrieval quality, state management, token budgets, and failure handling.

- 🎓 **MS in Artificial Intelligence**, University of the Cumberlands (USA) — in progress
- 🤖 Building with **LangGraph, LangChain, MCP, and RAG** — multi-agent orchestration and tool integration
- 🚀 Shipped **[CareerFitAI](https://careerfitai.onrender.com)** — a deployed resume/job-match analyzer with a test suite and CI
- 🧠 Deep learning background in **NLP (RNN sentiment models)** and **computer vision (medical imaging)**
- 🏗️ Prior **Python / Django REST** backend engineering — API design, PostgreSQL, Docker
- 📫 **kawsarhamid7225@gmail.com** · open to **AI Engineer / ML Engineer / LLM Engineer** roles

---

## 🤖 Agentic AI & LLM Systems

| Project | What it does | Stack |
| --- | --- | --- |
| **[CareerFitAI](https://github.com/KawsarHamid99/CareerFitAI)** · [🌐 live demo](https://careerfitai.onrender.com) | Analyzes how well a resume matches a job description — alignment score, matched vs. missing skills, and improvement suggestions with generated charts. **Scoring is deterministic Python; the LLM is deliberately confined to interpreting computed results**, so output stays reproducible and explainable. Ships with a pytest suite, GitHub Actions CI, and a Render Blueprint deploy. | FastAPI, OpenAI API, pdfplumber, python-docx, matplotlib, pytest |
| **[MCP Travel Assistant](https://github.com/KawsarHamid99/mcp-travel-assistant)** | Multi-agent planner where every agent reaches its tools over the **Model Context Protocol** — a weather MCP server I wrote with FastMCP, Tavily's hosted MCP over streamable HTTP, and a third-party aviation MCP server over stdio, unified behind one `MultiServerMCPClient`. State is checkpointed to Postgres so runs resume by thread ID; tool output is trimmed to stay inside provider token limits. | LangGraph, MCP, FastMCP, Groq, PostgreSQL |
| **[LangGraph Travel Planner](https://github.com/KawsarHamid99/langgraph-travel-planner)** | A four-node LangGraph pipeline — flight → hotel → itinerary → response — over typed shared state with reducer-based message accumulation and Postgres checkpointing. The direct-tool precursor to the MCP version above. | LangGraph, LangChain, Groq, Tavily, Streamlit |
| **[Conversational RAG over PDFs](https://github.com/KawsarHamid99/conversational-rag-pdf)** | Upload PDFs and ask follow-up questions that resolve against earlier turns: a history-aware retriever rewrites each question into a standalone query before retrieval, with chat history isolated per session ID. | LangChain, ChromaDB, Sentence-Transformers, Groq, Streamlit |
| **[Natural-Language SQL Agent](https://github.com/KawsarHamid99/nl-sql-agent)** | Ask questions in plain English against SQLite or a live MySQL connection — the agent inspects the schema, writes and runs the query, and streams its intermediate reasoning to the UI. | LangChain SQL Agent, SQLAlchemy, Groq, Streamlit |

## 🧠 Applied ML & Deep Learning

| Project | What it does | Stack |
| --- | --- | --- |
| **[Movie Review Sentiment](https://github.com/KawsarHamid99/movieReviewPrediction)** | Sentiment classifier over the IMDB corpus built on a recurrent network, packaged with the trained model for direct inference. | TensorFlow/Keras, RNN, NLP |
| **[Pneumonia Detection](https://github.com/KawsarHamid99/PneumoniaDetection)** | Chest X-ray classifier for pneumonia detection, with a browser-based interface for uploading and scoring images. | Deep Learning, Computer Vision, Medical Imaging |
| **[ML-Powered Django App](https://github.com/KawsarHamid99/ML_based_Django_application)** | Serves a trained ML model behind a Django web application — an early end-to-end take on getting a model into production. | Django, scikit-learn |

---

## Tech Stack

**LLM & Agent Engineering**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square&logo=groq&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)

`Multi-Agent Orchestration` · `Model Context Protocol` · `Tool / Function Calling` · `Agent State & Checkpointing` · `Prompt Engineering` · `Token Budgeting`

**RAG & Vector Retrieval**

![HuggingFace](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Chroma](https://img.shields.io/badge/ChromaDB-FF6B6B?style=flat-square&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat-square&logo=meta&logoColor=white)

`Sentence-Transformers` · `Recursive Chunking` · `History-Aware Retrievers` · `Document Loaders (PDF / Web / Arxiv)`

**ML & Deep Learning**

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

**Engineering & Deployment**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)

---

## Currently Working On

- **Agentic design patterns** — supervisor/worker topologies, planning, reflection, and multi-agent handoff in LangGraph
- **Model Context Protocol** — authoring custom MCP servers and connecting agents across stdio and streamable-HTTP transports
- **Production LLM concerns** — durable state, evaluation harnesses, tracing, token budgeting under rate limits, and cost control
- **Graduate coursework** in deep learning and AI systems at the University of the Cumberlands

---

<p align="center">
  <i>Open to AI/ML engineering roles — on-site, hybrid, or remote.</i><br>
  <a href="mailto:kawsarhamid7225@gmail.com">kawsarhamid7225@gmail.com</a>
</p>
