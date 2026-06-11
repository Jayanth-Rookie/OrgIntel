# 🏢 OrgIntel

**OrgIntel** is an internal AI-powered platform designed for organizations to securely manage, analyze, and query enterprise data. By leveraging **Retrieval-Augmented Generation (RAG)** and the **Model Context Protocol (MCP)**, OrgIntel enables smart, context-aware insights across departments while maintaining strict data governance.

---

## ✨ Key Features

- **🧠 Advanced RAG Architecture**: Interact with your organization's unstructured data (PDFs, docs) naturally through AI.
- **📊 MCP Integration**: Seamlessly handle and analyze large structured datasets (like Excel spreadsheets) to generate contextual insights.
- **🔐 Role-Based Access Control (RBAC)**: Strict differentiation between senior and junior employee access levels, ensuring sensitive/confidential data remains restricted to authorized personnel.
- **⚡ Real-time Communication**: Integrated WebSocket support for live updates and interactions.

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: React 19 (via Vite)
- **Styling**: Tailwind CSS 4
- **State Management**: Redux Toolkit & Redux Persist
- **Routing**: React Router v7
- **UI & Icons**: Lucide React, Sonner (for toasts)
- **PDF Handling**: React-PDF / PDF.js

### Backend
- **Server**: Node.js & Express.js
- **Database**: MongoDB (via Mongoose)
- **Vector Database**: ChromaDB
- **AI & LLMs**: Google Generative AI (Gemini), LangChain
- **Authentication**: JWT & bcrypt
- **Real-time**: Socket.io
- **File Processing**: Multer, PDF-Parse

---

## 📂 Project Structure

- `/Frontend` - React-based user interface.
- `/Backend` - Node.js server handling APIs, authentication, and database connections.
- `/MCP` - Scripts and configurations for the Model Context Protocol integrations.

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- MongoDB instance (local or Atlas)
- ChromaDB instance
- Google Gemini API Key

### 1. Clone the repository
```bash
git clone https://github.com/Jayanth-Rookie/OrgIntel.git
cd OrgIntel
```

### 2. Backend Setup
```bash
cd Backend
npm install
```
Create a `.env` file in the `/Backend` directory with the required variables:
- `PORT`
- `MONGO_URI`
- `JWT_SECRET`
- `GEMINI_API_KEY`
*(Include any other ChromaDB or specific environment variables required)*
```bash
npm run dev
```

### 3. Frontend Setup
```bash
cd ../Frontend
npm install
npm run dev
```

### 4. Access the App
Open your browser and navigate to `http://localhost:5173`.

---

## 📄 License
This project is for internal organizational use.
