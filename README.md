# 🕋 Hajj & Umrah RAG Chatbot
*An AI guide for the holiest journeys.*


<p align="center">
  <b>✨ Intelligent • Authentic • Reverent ✨</b><br>
  Guided by Islamic knowledge. Powered by modern AI.
</p>

---

## What is this project?

An elegant, retrieval-augmented AI assistant that answers questions related to **Hajj and Umrah**, grounded in a curated Islamic knowledge base.  
Combining **Node.js**, **OpenAI**, and a **React + Tailwind UI**, this project delivers *faithful, contextual, and safe answers* for pilgrims and students alike.

---

# Features

### Retrieval-Augmented Generation (RAG)
The chatbot retrieves relevant Hajj/Umrah knowledge before answering, ensuring accuracy and clarity.

### Faithful Islamic Answers
Responses are grounded strictly in the provided `knowledge.json`.

### Lightweight Retriever
Simple bag-of-words + similarity scoring for fast retrieval.

### Modern Elegant UI
- Black & gold theme  
- Smooth chat UI  
- Loading animations  
- Suggested quick questions  

---

# 📦 Project Structure

```
hajj-rag-system/
│
├── backend/                 # RAG engine + API
│   ├── server.js
│   ├── ragEngine.js
│   ├── retriever.js
│   ├── data/
│   │   └── knowledge.json
│   └── .env
│
└── hajj-ui/                 # React + Tailwind UI
    ├── App.jsx
    ├── HajjUmrahChat.jsx
    ├── main.jsx
    └── index.css
```

---

# 🔧 Backend Setup (Node.js + Express + OpenAI)

### Install dependencies
```bash
cd backend
npm install
```

### Environment variables
Create `backend/.env`:
```
OPENAI_API_KEY=sk-proj-xxxx
PORT=3001
```

### Start backend
```bash
npm start
```

---

# 🎨 Frontend Setup (React + Vite + Tailwind)

### Install dependencies
```bash
cd hajj-ui
npm install
```

### Vite proxy
```js
server: {
  proxy: {
    "/api": "http://localhost:3001"
  }
}
```

### Run frontend
```bash
npm run dev
```

---

# How the RAG Pipeline Works

1. User sends a question  
2. Backend retrieves relevant context  
3. Prompt is built with Islamic references  
4. LLM generates grounded response  
5. UI displays the answer  

---

# Test Questions

- What are the pillars of Hajj?  
- What happens on the Day of Arafat?  
- What is Ihram?  
- What is Tawaf al-Wida’?  

---

# 🌟 Future Enhancements

- Arabic mode  
- Embedding-based retrieval  
- Cloud deployment  
- Chat history  

---

**🤍 May this project benefit every pilgrim, learner, and seeker. 🤍**
