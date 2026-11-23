🔍 SEO Keyword Research AI Agent

This project is a Python-based AI Agent that takes a seed keyword and returns 50 optimized, rankable keyword suggestions based on:

High search volume

Low SEO competition

Trending relevance

It uses Gemini, Google Trends, and SerpAPI to intelligently generate and filter SEO keyword candidates.

🚀 Features

✅ Generate 100+ keyword suggestions using Gemini Pro (LLM)

📈 Score keyword popularity via Google Trends

📊 Fetch real-time SEO metrics via SerpAPI

🧠 Evaluate keyword rankability using Gemini reasoning

🔎 Filter & sort by: volume, competition, and trends

💡 Return Top 50 keywords that are SEO-optimized

🔁 (Optional) Automate entire flow with n8n

🧠 How It Works

Input: User enters a seed keyword (e.g., "remote internship")

Gemini: Generates long-tail, low-competition keyword ideas

Google Trends: Gets 12-month average trend score for each keyword

SerpAPI: Returns search volume + competition proxy

Gemini (again): Checks if keyword is rankable

Filter + Sort: By volume > 10K, comp < 10, rankable

Output: 50 best keywords printed or exported

🛠️ Tech Stack

Tool

Purpose

Gemini (Google Generative AI)

LLM-powered keyword generation + reasoning

Google Trends (pytrends)

Trend score over 12 months

SerpAPI

Search volume + competition data

Python 3.10+

Scripting & orchestration

(Optional) n8n

Full workflow automation

📦 Installation

pip install google-generativeai pytrends requests

🔧 Configuration

Set your API keys at the top of the script:

GEMINI_API_KEY = "your_gemini_key"
SERPAPI_KEY = "your_serpapi_key"

▶️ Running the Agent

python seo_agent.py

You’ll be prompted to enter a seed keyword. The agent will print the top 50 keyword recommendations with volume, competition, and trend scores.

📊 Sample Output

01) remote internship 2025 | Volume: 80000 | Comp: 6 | Trend: 72
02) best paid internships abroad | Volume: 72000 | Comp: 4 | Trend: 67
...

📤 Optional Automation (n8n)

Use n8n to:

Trigger the script via webhook or UI

Run and parse keyword results

Push to Google Sheets, Notion, or Email


📜 License


MIT License — Free to use and extend.
