# Latest Resume & Tech Stack Study Material

My living repo for two things:

1. **Resume** — the current version of my resume (editable `.docx` + `.pdf`), updated whenever I ship something new.
2. **Study Material** — a single interactive study guide (`.html`) covering target job roles, every tool in my tech stack, system design, AI system design, DSA, networking, software-engineering concepts, and where to stay updated.

## Latest versions

| What | File | Updated |
|---|---|---|
| Resume (Word) | [`Resume/Thejas M - Resume (2026-11-26).docx`](Resume/) | 2026-11-26 |
| Resume (PDF) | [`Resume/Thejas M - Resume (2026-11-26).pdf`](Resume/) | 2026-11-26 |
| Study guide | [`Study Material/Tech Career Playbook (2026-11-25).html`](Study%20Material/) | 2026-11-25 |
| Applications log | [`Applications/applications on 2026-11-26.html`](Applications/) | 2026-11-26 |

> Keep this table pointing at the newest files every time you update.

## ⚠️ Naming rule — always put the day's date in the file name

Every resume and study-material file **must** carry the date it was updated, in `YYYY-MM-DD` format (sorts correctly by name):

```
Resume/Thejas M - Resume (YYYY-MM-DD).docx
Resume/Thejas M - Resume (YYYY-MM-DD).pdf
Study Material/Tech Career Playbook (YYYY-MM-DD).html
Study Material/<Topic name> (YYYY-MM-DD).html        ← for any new study material
```

- A new update = a **new file with that day's date**. Don't overwrite an old dated file.
- Move superseded versions into `Resume/archive/` or `Study Material/archive/` so the top level only shows the latest.
- Update the **Latest versions** table above in the same commit.
- Commit message format: `resume: <what changed> (YYYY-MM-DD)` or `material: <what changed> (YYYY-MM-DD)`.

## Applications log

One HTML page per day of job applications, named `applications on YYYY-MM-DD.html` (made by LevelUpCorp `scripts/daily_summary.py`). Download and open in a browser.

## How to use the study guide

Download `Study Material/Tech Career Playbook (<date>).html` and open it in any browser (GitHub shows HTML as source code, so it must be opened locally).

- 🌓 dark / light mode toggle, sidebar contents, search (press `/`)
- Every topic: **plain-words intro → depth → real-work example → comparison & trade-offs → interview Q&A → links**
- Tick **learned** on a topic to track progress (saved in your browser)

### What's inside

| Chapter | Covers |
|---|---|
| Start Here | How to use the guide, study method |
| Your Resume: Interview Prep | Every resume bullet → likely questions + model answers |
| Job Roles & Career Map | Data/Product/Marketing Analyst, Analytics Eng, Growth Eng, FDE, AI/LLM Eng, AI Automation, Solutions Eng, DS, MLE/MLOps, Data Eng, DevOps/SRE, AI PM; salaries (indicative), interviews, recommended path |
| AI, LLM & ML Tech Stack | LLM internals, MoE, prompting, tool calling, agents, MCP, LangChain/LangGraph, embeddings, vector DBs, RAG, model routing, OpenClaw, Claude Code, evals, fine-tuning, classic ML |
| Languages & Data / Marketing Analytics / Automation & APIs / DevOps & Cloud / Extras | Python, SQL, pandas, stats, BI, warehouses, GA4, GSC, SEO, REST/OAuth, scraping, Selenium/Playwright, Git, Docker, Kubernetes, Azure, Linux, HTML/CSS, blockchain… |
| System Design, AI System Design, Classic Case Studies | Caching, load balancing, databases, queues, rate limiting, reliability, model routing & fallback, RAG at scale, worked designs |
| SE Fundamentals & Networking | OOP, SOLID, patterns, concurrency, testing; DNS, TCP/UDP, HTTP, TLS, "what happens when you type a URL" |
| DSA | Roadmap from zero, Big-O, every major pattern with Python templates + LeetCode links, SQL interview problems |
| Staying Updated | News, newsletters, YouTube, podcasts, engineering blogs, communities to join |

## Updating the repo (Windows, PowerShell)

```powershell
cd "C:\Users\Thejas\Desktop\Thejas\Personal\Latest-Resume-TechStack-Material"
git pull
# add the new dated files, move old ones to archive/, update the table above
git add -A
git commit -m "resume: added <new project> (YYYY-MM-DD)"
git push
```

## Privacy

The resume contains my phone number and email — **keep this repository private**, or publish a copy without contact details if it ever needs to be public. Never commit API keys, `token.json`, `client_secret*.json` or `.env` files.
