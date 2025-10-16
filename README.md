 AI LinkedIn Job Match Recommender (n8n No-Code Workflow)

A no-code **AI workflow built using n8n** that fetches job listings from LinkedIn (via Apify API), analyzes them using **OpenAI GPT models**, and automatically matches them to a candidate’s resume stored in Google Drive.  
The results including job details, required experience, keywords, and ATS-optimized resume suggestions are stored in **Google Sheets** for easy tracking.

---

## 🚀 Features
- 🔄 Automated job fetching from LinkedIn using **Apify API**
- 🧠 Job classification using **OpenAI GPT-4-mini**
- 💡 Extraction of **keywords, skills, tools, and experience** from job descriptions
- 🧾 **Resume analysis and matching** using embeddings
- 🧹 **Duplicate job removal** to ensure unique entries
- 📊 Data logging into **Google Sheets** for review and tracking
- ⚙️ 100% built with **drag-and-drop automation in n8n**

---

## 🛠️ Tools Used
| Tool | Purpose |
| **n8n** | Workflow orchestration |
| **OpenAI API (GPT-4-mini)** | Job analysis, resume tailoring |
| **Apify (LinkedIn Job Scraper)** | Job listings |
| **Google Drive API** | Resume download |
| **Google Sheets API** | Output logging |
| **Vector Store (LangChain)** | Resume embeddings for matching |

---

## 🧩 Workflow Overview
![Workflow Screenshot](workflow_screenshot.png)

### Flow Summary
1. **Trigger:** Manual or scheduled execution  
2. **Fetch Jobs:** via Apify LinkedIn job dataset API  
3. **AI Agent (OpenAI):** Analyzes and classifies each job  
4. **Remove Duplicates:** Skips previously processed jobs  
5. **Download Resume:** Fetches candidate’s resume from Google Drive  
6. **Vector Store & Embeddings:** Creates embeddings for semantic matching  
7. **AI Resume Edit Agent:** Aligns the resume with each job posting  
8. **Append to Google Sheets:** Logs results (title, company, skills, match score, etc.)

---

## 🧾 Setup & Reuse Instructions
1. Install or open [n8n](https://n8n.io/) (Cloud or local).  
2. Import the workflow file: ** Job Fetch.json **.  
3. Configure credentials:
   - **Apify API Token** (for LinkedIn jobs)
   - **Google Drive OAuth**
   - **Google Sheets OAuth**
   - **OpenAI API Key**
4. Update the **Google Sheet ID** and **resume file ID** in the workflow.
5. Click **“Execute Workflow”** or schedule it via cron.

---

## ✨ Author
**Koushik Tippani**  
_Data Engineer | AI & Automation Enthusiast_  
[LinkedIn](https://www.linkedin.com/in/koushik-tippani-b4290820b/)
