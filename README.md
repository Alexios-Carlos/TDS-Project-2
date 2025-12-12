# TDS Project 2: LLM Analysis - Autonomous Quiz Solver

An autonomous AI agent built for the **Tools in Data Science (TDS)** course. This application automatically solves multi-step data science quizzes by navigating websites, writing Python code, and analyzing data using **Google Gemini**.

## 🚀 Key Features
* **Autonomous Navigation:** Uses Playwright to browse web pages and extract tasks.
* **Intelligent Reasoning:** Uses LangGraph and Google Gemini 2.5 Flash to decide the next best step.
* **Code Execution:** Automatically generates and runs Python scripts to process CSVs, images, and logs.
* **Audio Processing:** Transcribes audio passphrases using `ffmpeg`.
* **Resilient:** Handles API rate limits and retries automatically.

## 🛠️ Tech Stack
* **Language:** Python 3.12
* **Web Framework:** FastAPI
* **LLM Orchestration:** LangChain & LangGraph
* **Browser Automation:** Playwright
* **Deployment:** Docker & Hugging Face Spaces

## ⚙️ API Usage
This project is deployed and running on Hugging Face Spaces.

**Endpoint:** `POST /solve`

**Sample Request:**
```json
{
  "email": "23f3001344@ds.study.iitm.ac.in",
  "secret": "YOUR_SECRET_KEY",
  "url": "[https://tds-llm-analysis.s-anand.net/project2](https://tds-llm-analysis.s-anand.net/project2)"
}
