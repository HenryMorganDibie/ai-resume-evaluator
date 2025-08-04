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
C:\Users\Henry Morgan\henry-analytics-core\ai-resume-evaluator\screenshots\screenshots\home_view.png

### 📥 Resume Upload
C:\Users\Henry Morgan\henry-analytics-core\ai-resume-evaluator\screenshots\screenshots\upload_screen.png

### 📊 Match Score Breakdown
C:\Users\Henry Morgan\henry-analytics-core\ai-resume-evaluator\screenshots\screenshots\score_breakdown.png

---

## 🧠 Scoring Logic

Each resume is evaluated based on:
- **TF-IDF Text Similarity** (60%)
- **Keyword Match Score** (40%)
- **Matched Skills** (Python, SQL, Power BI, Excel, etc.)

The logic is customizable in `scorer.py` and `matcher.py`

---

## 📁 Project Structure
<pre lang="markdown">
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
</pre>


---

## 🛠️ Installation

```bash
# Clone the repo
git clone https://github.com/HenryMorganDibie/ai-resume-evaluator.git
cd ai-resume-evaluator

# Create virtual environment
python -m venv venv
venv\Scripts\activate      # On Windows
# source venv/bin/activate  # On macOS/Linux

# Install required packages
pip install -r requirements.txt
```

## ▶️ Run the App
```
streamlit run app.py
```

## 📥 Sample Data
Test the app using files in the sample_data/ folder or upload your own:

- sample_resume.pdf

- sample_jd.txt

## 🌐 Deployment Options
- Deploy your app on:

- Streamlit Cloud

- Render

- Heroku

Instructions can be added in a future deployment section.

## 👨‍💻 Built By
Henry C. Dibie
Data Scientist | Analytics & Automation | NLP & AI Products
📎 LinkedIn
📰 Medium