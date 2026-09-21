# FinAI Agent - Financial AI Assistant 🚀

FinAI is a backend AI agent designed to explain complex financial concepts in a clear and accessible way. Built with **FastAPI** and integrated with **Google Gemini AI**, it provides an intelligent, high-performance API for financial queries and assistant workflows.

---

## 📌 Features

* **AI-Powered Financial Insights:** Leverages Google Gemini AI to analyze and simplify financial terminology.
* **Asynchronous API Architecture:** High-performance RESTful endpoints using FastAPI and Uvicorn.
* **Lightweight Data Persistence:** Built-in SQLite integration for simple data management without extra database overhead.
* **Secure Environment Management:** Sensitive keys and service credentials managed safely via environment variables.

---

## 🎯 Motivation

I built **FinAI Agent** to demonstrate core backend development practices, including RESTful API design, third-party AI integration, and secure environment configuration. SQLite was selected for efficient local data storage, and environment variable isolation ensures production-ready credential management.

---

## 🛠️ Tech Stack

| Component | Technology | Version |
| :--- | :--- | :--- |
| **Language** | Python | `3.14.2` |
| **Framework** | FastAPI | `0.141.1` |
| **ASGI Server** | Uvicorn | `0.53.0` |
| **AI Provider** | Google Generative AI | `0.8.6` |
| **Data Validation** | Pydantic | `2.13.5` |
| **Environment Vars** | python-dotenv | `1.2.3` |
| **Database** | SQLite | Built-in |

---

## ⚙️ Local Setup & Installation

Follow these steps to run the project locally.

### 1. Prerequisites

Ensure you have **Python 3.14.2** installed on your system.

### 2. Clone the Repository

```bash
git clone [https://github.com/JepsXR/FinAI-MVP.git](https://github.com/JepsXR/FinAI-MVP.git)
cd FinAI-MVP

### 3. Create & Activate Virtual Environment

Windows PowerShell: 

python -m venv venv
.\venv\Scripts\Activate.ps1

Linux / macOS

python3 -m venv venv
source venv/bin/activate

### 4. Install dependences
Once your virtual environment is active, install all required packages:

pip install -r requirements.txt

### 5. Environment variables configuration
Create a .env file in the root directory based on the expected configuration:

Code Snippet: 
API_KEY=your_google_gemini_api_key_here

(Never commit your .env file to version control. Keep .env listed in .gitignore at all times).

## 🚀 Running the server
Start the local development server using Uvicorn:

uvicorn main:app --reload

Once running, access the interactive API documentation at:

Swagger UI: http://127.0.0.1:8000/docs

ReDoc: http://127.0.0.1:8000/redoc
