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
<img width="956" height="628" alt="home_view" src="https://github.com/user-attachments/assets/84f933d5-4700-4c59-b96b-157b793348e1" />


### 📥 Resume Upload
<img width="1059" height="297" alt="upload _screen" src="https://github.com/user-attachments/assets/97fa2254-69ec-4e40-956c-b901c9a285a2" />


### 📊 Match Score Breakdown
<img width="849" height="205" alt="score_breakdown" src="https://github.com/user-attachments/assets/5aa7162b-9928-4e8d-873b-307d83db5c50" />


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
