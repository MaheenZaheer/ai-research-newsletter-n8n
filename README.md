# Autonomous AI Research Newsletter Aggregator (n8n & Groq)

An automated backend pipeline that fetches real-time research papers from the arXiv API, uses an Advanced AI Agent (Groq / Llama 3) to summarize them, and dispatches a clean daily newsletter via Gmail.

## How It Works
1. **Schedule Trigger:** Runs automatically at scheduled intervals.
2. **HTTP Request:** Ingests live XML data from the official arXiv API.
3. **AI Agent (Groq):** Parses raw XML, filters top papers, and creates concise 2-sentence impactful summaries.
4. **Gmail Node:** Dynamically formats the AI output and sends the newsletter to the inbox.

## Tech Stack
- **Automation Platform:** n8n
- **LLM Provider:** Groq (Llama 3)
- **API Integration:** arXiv API
- **Delivery System:** Gmail Integration

## How to Use This Workflow
1. Download the `workflow.json` file from this repository.
2. Open your n8n instance, create a new workflow, and click on **Import from File** (or simply press `Ctrl + V` on the canvas).
3. Configure your credentials for **Groq API** and **Gmail Sign-in**.
4. Click **Publish** to activate the automation!
