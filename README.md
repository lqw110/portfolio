# portfolio

# 👋 Hi, I'm Iris

Senior Data Consultant @ EY | Machine Learning Engineer | CPA  

I build production-grade AI systems, including machine learning models, computer vision applications, and LLM-based solutions.

---

## 🔥 Highlights
- Experience building AI/ML systems in both academic and enterprise settings  
- Strong foundation in machine learning, computer vision, and data pipelines  
- Focus on practical, real-world problem solving  

---

## 🚀 Featured Projects

### ✈️ 1. Travel Social Agent
🔗 https://github.com/lqw110/travel-social-agent

An agentic AI app that turns a travel story and a folder of photos into a ready-to-publish Facebook post — with a human approving every step before anything goes live.

- Multimodal pipeline: an LLM analyzes the story, then a vision model scores every photo for relevance and writes a plain-language reason for each pick
- Human-in-the-loop by design — nothing is ever auto-posted; publishing requires an explicit approval click, with a dry-run mode on by default
- Five-step guided workflow (Story → Photos → Recommendations → Caption → Publish) built with Streamlit, with an editable AI-generated caption, live Facebook post preview, and one-click revisions
- Integrates the Meta Graph API for real publishing, and explores LangGraph for workflow orchestration

**Tech:** Python, OpenAI GPT-4o (text + vision), Streamlit, LangGraph, Meta Graph API

---

### 🗄️ 2. Text-to-SQL Agent
🔗 https://github.com/lqw110/text2sql_agent

An interactive terminal agent that converts natural-language questions into validated SQL, executes it against any SQLite database, and holds context across follow-up questions — with the guardrails and self-validation a real BI tool needs, not just a demo query generator.

- Per-question table selection before generation: one model call picks the relevant tables from the schema, so only what's needed enters the prompt — the piece that lets this scale past a schema too large to fit in context whole
- Guarded repair loop: `EXPLAIN`-validates generated SQL before ever executing it, and on failure feeds the real database error back to the model for self-correction, rather than guessing blind twice
- Two independent safety layers — a static read-only check for fast, readable errors, backed by a hard read-only SQLite connection as the actual guarantee against writes
- Execution-result scoring, not string-matching: compares result sets with column-order and tie-order tolerance, plus an LLM-as-judge fallback for questions with only a prose answer, cross-checked against the strict scorer so it's never trusted blind — all covered by 46 unit tests
- Also answers general SQL syntax/concept questions directly in plain language when that's what's actually being asked, instead of forcing a query

**Tech:** Python, OpenAI API (GPT-5 family), SQLite, structured outputs, pytest

---

### 📊 3. Machine Learning Capstone (Springboard)
🔗 https://github.com/lqw110/Springboardminiprojects

- End-to-end machine learning project covering data cleaning, feature engineering, and modeling  
- Applied traditional ML techniques to solve real-world prediction problems  
- Performed model evaluation and performance tuning  

**Tech:** Python, Pandas, Scikit-learn, Data Analysis  

---

### 👁️ 4. Computer Vision Project (MCIT - CIS 5810)
🔗 https://github.com/lqw110/CIS5810_final_project *(Private Repository)*

- Developed a computer vision system as part of graduate coursework  
- Implemented image processing and/or deep learning techniques  
- Focused on visual recognition and model performance  

⚠️ *This repository is private — happy to grant access upon request.*

**Tech:** Python, OpenCV, Deep Learning  

---

## 📫 Contact
- LinkedIn: https://linkedin.com/in/qiweilu
