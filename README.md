# 🤖 DocuMind AI

## AI-Powered Document Assistant & Resume Analyzer

**Understand documents. Discover skills. Prepare for opportunities.**

DocuMind AI is a full-stack application that extracts text from PDF and TXT documents, analyzes resumes, compares skills with job descriptions, and answers questions about document content.

### ✨ Features

* 📄 PDF and TXT document text extraction
* 🤖 AI-powered document question answering
* 🧑‍💼 Resume skill detection
* 🎯 Job description and skill matching
* 📊 Resume skill-match percentage
* 💡 Resume improvement suggestions
* 🗂️ Analysis history using SQLite
* 🎨 Responsive React dashboard
* 🔌 REST API with FastAPI
* 🔐 Optional OpenAI API integration

### 🧰 Tech Stack

* **Frontend:** React.js, Vite, CSS
* **Backend:** Python, FastAPI
* **PDF Processing:** PyMuPDF
* **Database:** SQLite
* **AI Integration:** OpenAI API (optional)
* **Icons:** Lucide React

### 🏗️ Project Architecture

React Frontend → FastAPI Backend → Document Processing and Resume Analysis → SQLite Database

Optional AI integration provides AI-generated document answers.

### 📂 Project Structure

```text
ai-document-assistant-resume-analyzer/
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   └── .env.example
├── frontend/
│   ├── index.html
│   ├── package.json
│   └── src/
│       ├── main.jsx
│       └── style.css
└── README.md
```

### ⚙️ Installation

**Prerequisites:** Python 3.10+, Node.js 18+, npm, and VS Code.

**1. Clone the repository**

```bash
git clone https://github.com/abinaya-345/ai-document-assistant-resume-analyzer.git
cd ai-document-assistant-resume-analyzer
```

**2. Start the backend**

```bash
cd backend
python -m venv .venv
```

Windows:

```powershell
.venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
uvicorn main:app --reload
```

**3. Start the frontend**

Open a second terminal:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL shown by Vite, normally `http://localhost:5173`.

### 🔌 API Endpoints

| Method | Endpoint       | Purpose                |
| ------ | -------------- | ---------------------- |
| GET    | `/`            | API welcome message    |
| GET    | `/api/health`  | Health check           |
| POST   | `/api/extract` | Extract document text  |
| POST   | `/api/analyze` | Analyze resume         |
| POST   | `/api/ask`     | Ask document questions |
| GET    | `/api/history` | View analysis history  |

API documentation: `http://127.0.0.1:8000/docs`

### 📚 Learning Resources

* 🐍 Python: https://docs.python.org/3/tutorial/
* ⚡ FastAPI: https://fastapi.tiangolo.com/tutorial/
* ⚛️ React: https://react.dev/learn
* 🚀 Vite: https://vite.dev/guide/
* 📄 PyMuPDF: https://pymupdf.readthedocs.io/en/latest/
* 🗄️ SQLite: https://www.sqlite.org/docs.html
* 🤖 OpenAI API: https://platform.openai.com/docs/
* 🐙 GitHub: https://docs.github.com/en

### 🛡️ Security and Limitations

* Never publish API keys or private documents.
* The skill-match percentage is a basic keyword-based indicator, not a real ATS score.
* Local document question answering may miss context.
* Scanned PDFs require OCR, which is not included.
* Production deployment requires additional authentication, security, privacy controls, and validation.

### 🚀 Future Enhancements

* [ ] User authentication
* [ ] OCR for scanned PDFs
* [ ] Semantic search and RAG
* [ ] Downloadable resume reports
* [ ] Automated testing
* [ ] Docker deployment
* [ ] Multilingual support

### 👩‍🏫 Internship Guide

**Guide Name:** Vaishali

### 👩‍💻 Developer

**Name:** ABINAYA N

**LinkedIn:** https://www.linkedin.com/in/abinaya-n-b06954375

**GitHub:** https://github.com/abinaya-345

---

⭐ Built with Python, React, and AI for learning and portfolio development.

