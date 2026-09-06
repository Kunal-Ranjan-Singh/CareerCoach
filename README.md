# 🚀 AI Career Assistant

**AI Career Coach** is a Flask-based web application that leverages OpenAI's GPT models and FAISS vector search to provide intelligent resume evaluations and interactive career guidance. Users can upload their resumes to receive a structured analysis and interact with an AI to ask specific career-related questions based on their profile.

---

## ✨ Features

*   📄 **Resume Analysis:** Upload your PDF resume and instantly receive a comprehensive, structured summary including:
    *   Career Objective
    *   Skills and Expertise
    *   Professional Experience
    *   Educational Background
    *   Notable Achievements
*   💬 **Interactive Q&A System:** Ask career-related questions directly based on your resume's content and get smart, contextual responses.
*   🔍 **Vector Search Integration:** Utilizes FAISS for lightning-fast, efficient document retrieval from embedded resume data.

---

## 🛠️ Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Backend** | Python, Flask |
| **Frontend** | HTML, Tailwind CSS, Framer Motion |
| **AI & NLP** | OpenAI GPT-4, OpenAI ADA Embeddings, LangChain |
| **Data Processing** | PyPDF2 (PDF parsing), FAISS (Vector Database) |

---

## 📂 Project Structure

```text
├── app.py                # Main Flask application logic
├── requirements.txt      # Project dependencies (assumed)
├── index.faiss           # FAISS index file (generated dynamically)
├── index.pkl             # FAISS metadata file (generated dynamically)
├── uploads/              # Directory to store uploaded user PDFs
└── templates/            # HTML templates (Jinja2)
    ├── index.html        # Resume upload page
    ├── results.html      # Resume analysis results display
    ├── ask.html          # QA input interface
    ├── qa_results.html   # QA output display
    └── query_results.html# [Optional] Extra query display
```

## 🔧 Setup Instructions

Follow these steps to get the project running on your local machine.

### 1. Clone the Repository
```bash
git clone [https://github.com/yourusername/ai-career-coach.git](https://github.com/yourusername/ai-career-coach.git)
cd ai-career-coach
```
### 2. Create and activate Virtual Environment
# On macOS/Linux:
```
python -m venv venv
source venv/bin/activate
```

# On Windows:
```
python -m venv venv
venv\Scripts\activate
```
### 3. Install dependencies
```
pip install -r requirements.txt
```

### 4. Run the application
```
python app.py
```
Once the server starts, open your web browser and navigate to: http://localhost:5000

Demo
Coming soon...
