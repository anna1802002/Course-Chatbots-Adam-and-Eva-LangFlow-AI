# 🎮 Eva – The Gamified Learning AI

**Eva** is a gamified learning assistant that transforms traditional study materials into **interactive challenges, quests, and rewards**.  
Built with **LangFlow** and **RAG**, Eva redefines how students learn by turning each topic into a motivating game-like experience.

---

## 🌟 Key Features
- **Gamified Learning** – Converts lessons into interactive quests, puzzles, and levels.  
- **Personalized Progression** – Adapts difficulty and feedback based on user performance.  
- **Reward & Badge System** – Motivates learners with XP, badges, and leaderboards.  
- **Community Challenges** – Enables collaborative and competitive learning events.  
- **Contextual Generation** – Retrieves accurate course material using **ChromaDB** and **OpenAI Embeddings**.

---

## 🧩 Tech Stack & Architecture
| Component | Description |
|------------|-------------|
| **Framework** | [LangFlow](https://github.com/logspace-ai/langflow) |
| **RAG Engine** | ChromaDB + OpenAI text-embedding-3-small |
| **Model** | Groq `llama-3.1-8b-instant` |
| **Temperature** | 0.5 (balanced creativity) |
| **Pipeline** | Study Material Loader → Split → Embed → Retrieve → Prompt → Generate → Output |

---

## 🧱 Pipeline Breakdown
1. **File Loader** – Imports PDFs or notes for gamified content generation.  
2. **Text Splitter** – Breaks down long documents (1000-char chunks, 200 overlap).  
3. **Embedding Generator** – Converts text into semantic vectors.  
4. **ChromaDB Storage** – Stores embeddings persistently for quick retrieval.  
5. **Retriever Flow** – Fetches relevant chunks when a topic is requested.  
6. **Prompt Template** – Generates personalized learning quests with rewards.  
7. **LLM Processing** – Uses Groq’s `llama-3.1-8b-instant` to create game-like challenges.  
8. **Chat Output** – Displays the interactive quest in LangFlow’s chat UI.


---

## ⚙️ How to Run
1. Launch [LangFlow](https://github.com/logspace-ai/langflow)
2. Import the `Eva.json` flow
3. Add your OpenAI API key under the Embeddings node
4. Upload your study content (text/PDF)
5. Ask Eva: *“Create a quest on linear regression”* or *“Make a gamified challenge for world history”*

---

## 📂 Repository Files
- `Eva.json` — LangFlow pipeline export  
- `Eva.pdf` — Full documentation of the RAG + Gamification pipeline  
- `README.md` — This guide  

---

## 👩‍💻 Author
**Ananya Mahesh Shetty**  
*Humanitarians AI x Stellis Labs| Northeastern University*  
📧 shetty.ana@northeastern.edu  
🌐 [LinkedIn](https://www.linkedin.com/in/ananya-mahesh-shetty)

---

