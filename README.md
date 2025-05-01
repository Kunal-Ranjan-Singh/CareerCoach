
AI Career Coach is a Flask-based web application that leverages OpenAI's GPT models and FAISS vector search to provide intelligent resume evaluations and interactive career guidance. Users can upload their resumes and receive a summarized analysis, then interact with the system to ask career-related questions.

Features:-
Resume Analysis
Upload your PDF resume and receive a structured summary including:-

Career Objective

Skills and Expertise

Professional Experience

Educational Background

Notable Achievements

Question Answering System
Ask career-related questions directly based on your resume content and get smart, contextual responses.

Vector Search Integration
Uses FAISS for efficient document retrieval from embedded resume data.

🛠️ Tech Stack
Backend: Python, Flask

Frontend: HTML, Tailwind CSS, Framer Motion

AI Models: OpenAI GPT-4, ADA Embeddings

Vector DB: FAISS

PDF Processing: PyPDF2

LangChain: For prompt chaining and document QA

Project Structure
bash
Copy
Edit
├── app.py                  # Main Flask application
├── templates/              # HTML templates (Jinja2)
│   ├── index.html          # Resume upload page
│   ├── results.html        # Resume analysis results
│   ├── ask.html            # QA input page
│   ├── qa_results.html     # QA output page
│   └── query_results.html  # [Optional] extra query display
├── uploads/                # Directory to store uploaded PDFs
├── index.faiss             # FAISS index file
├── index.pkl               # FAISS metadata file
🔧 Setup Instructions
Clone the Repository



bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
Install Dependencies

bash
Copy
Edit
pip install -r requirements.txt
Set OpenAI API Key

Replace the api_key fields in app.py with your own key or manage via environment variables.

Run the App

bash
Copy
Edit
python app.py
Visit http://localhost:5000 in your browser.

Notes
The app uses LangChain for both summarization and retrieval-based QA.

Ensure your API key usage complies with OpenAI's terms.

Uploaded resumes must be in PDF format.

FAISS index is recreated on each new upload.

Demo
Coming soon...

Author:
Kunal – Made with ❤️
