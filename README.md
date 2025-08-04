# 🤖 AI Resume Evaluator

An AI-powered Streamlit app that allows HR teams and recruiters to evaluate and score resumes based on job descriptions using natural language processing (NLP) and customizable scoring logic.

---

## 🚀 Features

- 🔍 **Resume Parsing** – Supports PDF and DOCX files.
- 📝 **Job Description Input** – Paste or upload job requirements.
- 📊 **Smart Resume Scoring** – Uses NLP (TF-IDF + keyword matching) to generate match scores.
- 📂 **Batch Upload** – Score multiple resumes in one go.
- 🧠 **Explainable Scoring** – View matched keywords and similarity breakdown.

---

## 📸 Demo Screenshots

### 🏠 Home View
ai-resume-evaluator\screenshots\screenshots\home_view.png

### 📥 Resume Upload
ai-resume-evaluator\screenshots\screenshots\upload_screen.png

### 📊 Match Score Breakdown
ai-resume-evaluator\screenshots\screenshots\score_breakdown.png

---

## 🧠 Scoring Logic

Each resume is evaluated based on:
- **TF-IDF Text Similarity** (60%)
- **Keyword Match Score** (40%)
- **Matched Skills** (Python, SQL, Power BI, Excel, etc.)

You can customize the skill list and weights in `scorer.py`.

---

## 📁 Project Structure

ai-resume-evaluator/
├── app.py # Main Streamlit app
├── utils/
│ ├── parser.py # Extract text from resumes and JDs
│ ├── scorer.py # Scoring logic
│ └── matcher.py # Keyword/fuzzy matching functions
├── sample_data/
│ ├── sample_resume.pdf
│ └── sample_jd.txt
├── screenshots/
│ ├── home_view.png
│ ├── upload_screen.png
│ └── score_breakdown.png
├── requirements.txt
├── README.md
└── .gitignore