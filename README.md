# awesome-n8n-ai-agents

> A curated collection of production-ready **n8n + LLM automation workflows** — real AI agents for job search, content creation, analytics, and more.

![n8n](https://img.shields.io/badge/n8n-EA4B71?logo=n8n&logoColor=white&style=flat-square)
![Claude](https://img.shields.io/badge/Claude-CC785C?logo=anthropic&logoColor=white&style=flat-square)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?logo=openai&logoColor=white&style=flat-square)
![Gemini](https://img.shields.io/badge/Gemini-4285F4?logo=google&logoColor=white&style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)

Each workflow in this collection is **fully documented**, **importable into n8n**, and built around a real use case — not toy examples.

---

## Workflows

### Job & Career Automation

| Project | Stack | What it does |
|---------|-------|-------------|
| [JobPilot — AI Job Search Agent](https://github.com/chintalaanvesh/jobpilot-ai-agent) | n8n · Claude · Next.js · Supabase | Scrapes LinkedIn jobs, scores each against your resume (0–100), generates personalized cover letters and outreach emails. Full dashboard UI with live demo. |

---

### Content & Social Media Automation

| Project | Stack | What it does |
|---------|-------|-------------|
| [Instagram Content Agent](https://github.com/chintalaanvesh/instagram-content-agent) | n8n · GPT-4o · Gemini Imagen 4.0 · Cloudinary | RSS feeds → relevance scoring → caption + hashtag generation → AI image generation → Cloudinary post-processing → Google Sheets content calendar. Fully automated, daily. |

---

### Analytics & Data Pipelines

| Project | Stack | What it does |
|---------|-------|-------------|
| [Gig Surge Analytics](https://github.com/chintalaanvesh/gig-surge-analytics) | n8n · GPT-4o Vision · PostgreSQL · Google Sheets | Turns delivery platform surge screenshots into a queryable PostgreSQL database. Conversational AI agent answers earnings questions in plain English using SQL tool calls. |
| [Zomato Spend Analyzer](https://github.com/chintalaanvesh/zomato-spend-analyzer) | n8n · OpenAI · Telegram | Extracts Zomato invoices, analyzes spending patterns, sends reports and budget alerts via Telegram. |

---

### Multimodal & Vision Pipelines

| Project | Stack | What it does |
|---------|-------|-------------|
| [Ad Variable Extraction](https://github.com/chintalaanvesh/ad-variable-extraction) | n8n · Claude Vision · Cloudinary · Google Sheets | Pulls video frames from Cloudinary, runs Claude Vision + Claude Text to extract 10 creative performance variables per ad, writes structured output back to Google Sheets. |

---

### Chatbots & Support

| Project | Stack | What it does |
|---------|-------|-------------|
| [Credit Support Chatbot](https://github.com/chintalaanvesh/credit-support-chatbot) | JavaScript · HTML · LLM | AI-powered customer support chatbot for credit-related queries. |

---

## How to Use Any Workflow

Every project repo contains:
- A **detailed README** with architecture diagram, workflow breakdown, and setup steps
- The **n8n workflow JSON** (importable via n8n → Import Workflow)
- Environment variable templates

**General setup pattern:**

```bash
# 1. Clone the individual project repo
git clone https://github.com/chintalaanvesh/<project-name>.git

# 2. Follow the README setup steps

# 3. Import the workflow JSON into your n8n instance
#    n8n → Workflows → Import from file → select workflow.json

# 4. Add your API credentials in n8n (OpenAI / Claude / Gemini key)

# 5. Update webhook URLs if required, then activate
```

---

## Tech Stack Across the Collection

| Category | Tools |
|----------|-------|
| Orchestration | n8n (self-hosted or cloud) |
| LLMs | Claude (Anthropic), GPT-4o (OpenAI), Gemini (Google) |
| Vision / Multimodal | Claude Vision, GPT-4o Vision, Gemini Imagen 4.0 |
| Databases | PostgreSQL, Supabase |
| Storage / Media | Cloudinary, Google Drive |
| Frontend | Next.js, TypeScript |
| Notifications | Telegram |
| Spreadsheets | Google Sheets |

---

## Contributing

Found a bug, want to add a workflow, or have an improvement? Contributions are welcome.

1. Fork this repo
2. Add your workflow to the relevant category in the table above
3. Make sure your project repo has: a clear README, a workflow JSON file, and documented env variables
4. Open a PR with a short description of what your workflow does

If you want to suggest a use case for a new workflow, open an [issue](https://github.com/chintalaanvesh/awesome-n8n-ai-agents/issues) with the label `workflow-idea`.

---

## About

Built by [Chintala Anvesh](https://github.com/chintalaanvesh) — building AI agents and automation workflows with n8n, Claude, GPT-4o, and Gemini.

Connect on [LinkedIn](https://www.linkedin.com/in/chintalaanvesh) · Star this repo if it's useful ⭐
