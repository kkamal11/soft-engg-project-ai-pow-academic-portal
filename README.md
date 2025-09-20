# 🎓 AI-Powered Academic Portal  



An academic platform built as part of a **Software Engineering Project (Team 26)**.  

This system provides an end-to-end solution for students, faculty, and administrators, integrating **AI features**, **learning management tools**, and **performance analytics**.  



---



## 🚀 Overview  



The project is divided into two major components:  



- **Frontend** → A modern web client built with Vue.js 3, Tailwind CSS, and Pinia for state management.  

- **Backend API** → A FastAPI-based backend with PostgreSQL, JWT authentication, file storage, plagiarism detection, and vector store retrieval for AI-driven features.  



---



## ✨ Key Features  



### Frontend  

- 🎓 Course Management & Enrollment  

- 📊 Analytics Dashboard  

- 👥 User Management System  

- 🎥 Video Lecture Platform  

- 📚 Content & FAQ Management  

- 🔐 Role-based Access Control  



### Backend  

- 🔑 JWT Authentication + Google OAuth  

- 📂 File Uploads (Local & S3-compatible storage)  

- 📝 Assignment & Grading System  

- 🔍 Plagiarism Detection  

- 📖 Vector Store for Course Material Retrieval (AI-powered Q&A)  

- 🛠 Monitoring & Health Checks  



---



## 🛠️ Technology Stack  



### Frontend  

- **Framework:** Vue.js 3 (Composition API)  

- **State Management:** Pinia  

- **Styling:** Tailwind CSS  

- **Routing:** Vue Router  

- **Build Tool:** Vite  

- **Code Quality:** ESLint  

- **Package Manager:** npm  



### Backend  

- **Framework:** FastAPI (Python 3.9+)  

- **Database:** PostgreSQL (with `pgvector` extension)  

- **Storage:** Local & S3-compatible (Cloudflare R2, AWS S3)  

- **Authentication:** JWT + Google OAuth  

- **Caching/Optional:** Redis  

- **LLM/AI:** Google `text-embedding-004`, LangChain PGVector  



---



## 📦 Project Structure  



```

project-root/

├── frontend/           # Vue.js 3 + Tailwind CSS client

│   └── src/            # Components, views, stores, services

└── backend/            # FastAPI backend

         ├── main.py         # Entry point

         ├── services/       # Core services (auth, courses, grading)

         ├── uploads/        # Local file storage (dev mode)

         └── pdfs/           # Course PDFs for vector store

```  



---



## ⚡ Setup & Installation  



### Prerequisites  

- Node.js v16+ & npm v7+  

- Python 3.9+  

- PostgreSQL  

- Git  



---



### 🔹 Frontend Setup  



```bash

# Clone repo and go to frontend

git clone [repository-url]

cd project-root/frontend



# Install dependencies

npm install



# Set up environment

cp .env.example .env



# Start dev server

npm run dev

```



The app runs at **http://localhost:5173**  



---



### 🔹 Backend Setup  



```bash

# Go to backend

cd project-root/backend



# Install dependencies

pip install -r requirements.txt



# Setup environment

cp .env.example .env   # update with DB, JWT, S3 credentials



# Run backend server

uvicorn main:app --reload

```



Backend runs at **http://localhost:8000**  

- Swagger Docs → `http://localhost:8000/docs`  

- ReDoc → `http://localhost:8000/redoc`  



---



## 🧪 Testing  



### Frontend  

```bash

npm run test:unit     # Unit tests

npm run test:e2e      # End-to-end tests

```



### Backend  

```bash

pytest

```  



---



## 🚀 Deployment  



### Frontend  

- Netlify, Vercel, or static web server (Nginx/Apache).  

- Run `npm run build` → deploy `dist/` folder.  



### Backend  

- Local / Docker / Vercel serverless functions.  

- Ensure S3 storage is configured for file uploads.  

- Example: Vercel deployment uses `backend/` as root with optimized build script.  



---



## 📖 Coding Standards  



- Vue 3 **Composition API** with `<script setup>`  

- Pinia for state management  

- TypeScript where possible  

- ESLint rules enforced  

- Backend follows **PEP8** & FastAPI best practices  

- Secure handling of JWT & API tokens  



---



## 🔒 Security & Best Practices  



- Input validation & sanitization  

- HTTPS for all API calls  

- Lazy loading & caching for performance  

- Proper error handling & logging  

- Role-based access control  



---



## 🤝 Contributing  



1. Fork & create a feature branch  

2. Commit changes with clear messages  

3. Add/update tests  

4. Update documentation if needed  

5. Submit a pull request  



---



## 📄 License  

&nbsp;



---



**Last Updated:** February 2025  

**Version:** 1.0.0  



