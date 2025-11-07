# 🧠 Adam – The Quiz Maker

**Adam** is an AI-powered quiz generator built entirely in **LangFlow**, designed to make learning more interactive and personalized.  
Leveraging **Retrieval-Augmented Generation (RAG)** and **semantic search**, Adam dynamically creates quizzes based on uploaded course content, tracks learning progress, and provides instant feedback — acting like a smart tutor.

---

## 🚀 Key Features
- **Adaptive Quiz Generation** – Creates quizzes from uploaded study materials using LangFlow + RAG.
- **Multiple Question Types** – Supports multiple-choice, short answer, and true/false formats.
- **Smart Retrieval System** – Uses **ChromaDB** and **OpenAI Embeddings** for precise, context-aware question generation.
- **Instant Feedback Loop** – Provides explanations and hints after each question.
- **Dynamic Difficulty** – Adjusts question complexity based on user performance.

---

## 🧩 Tech Stack & Architecture
| Component | Description |
|------------|-------------|
| **Framework** | [LangFlow](https://github.com/logspace-ai/langflow) |
| **RAG System** | OpenAI Embeddings + ChromaDB |
| **Model** | Groq `llama-3.1-8b-instant` |
| **Temperature** | 0.4 for accuracy & creativity balance |
| **Pipeline** | Data Loader → Embed → Retrieve → Prompt → Generate → Output |

---

## 🧱 Pipeline Breakdown
1. **Data Loader** – Ingests PDF or text materials into the RAG system.  
2. **Text Splitter** – Chunks data into manageable text blocks (1000 chars, 200 overlap).  
3. **Embedding Generator** – Converts text into vector embeddings for semantic search.  
4. **ChromaDB Storage** – Stores embeddings for persistent retrieval.  
5. **Retriever Flow** – Finds relevant context from stored materials.  
6. **Prompt Template** – Generates structured quiz prompts from retrieved content.  
7. **LLM Processing** – Uses `llama-3.1-8b-instant` (Groq API) to generate the quiz.  
8. **Chat Output** – Displays quiz interactively within LangFlow.


---

## ⚙️ How to Run
1. Open [LangFlow](https://github.com/logspace-ai/langflow)
2. Import the `Adam.json` file into a new flow
3. Add your OpenAI API key under the Embeddings node
4. Upload course content (PDFs, notes, etc.)
5. Chat with Adam — ask *“Generate a quiz on World War II”* or *“Test me on supply chain management basics”*

---

## 📂 Repository Files
- `Adam.json` — Full LangFlow pipeline export  
- `Adam The Quiz Maker Documentation.pdf` — Detailed architecture, pipeline, and prompt flow  
- `README.md` — You’re reading it!  

---

## 🧑‍💻 Author
**Ananya Mahesh Shetty**  
*Humanitarians AI x Stellis Labs | Northeastern University*  
📧 shetty.ana@northeastern.edu  
🌐 [LinkedIn](https://www.linkedin.com/in/ananya-mahesh-shetty)

---
