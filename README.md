<div align="center">

# 👋 Hey, I'm Neerav Jha

### Backend Engineer crafting AI & automation systems

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=3FD0FF&center=true&vCenter=true&width=650&lines=Backend+%26+Systems+Engineer;I+build+things%2C+then+break+them+with+load+tests;Creator+of+env-doctor+%26+llm-gateway;Currently%3A+chasing+milliseconds" alt="Typing SVG" />

<br>

[![Portfolio](https://img.shields.io/badge/🌐_Portfolio-0F2027?style=for-the-badge)](https://neerav-portfolio-nine.vercel.app)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@neeravjha444)
[![Resume](https://img.shields.io/badge/Resume-2C5364?style=for-the-badge)](https://drive.google.com/file/d/1h-w5dZftKcPxryhzdudBlT-FsQ2AFgkQ/view?usp=drivesdk)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/neerav-jha)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:neeravjha444@gmail.com)

</div>

<br>

<img align="right" alt="coding" width="340"
src="https://user-images.githubusercontent.com/74038190/229223263-cf2e4b07-2615-4f87-9c38-e37600f8381a.gif">

## 🚀 About Me

- 🔭 Building **AI-powered backend systems** & voice assistants
- 🛠️ Shipped **env-doctor** — the ESLint of environment variables (CLI + VS Code extension + GitHub Action)
- ⚡ Shipped **llm-gateway** — a multi-provider LLM routing gateway with semantic caching, failover & cost tracking
- 🐛 Recently found (and fixed) an **8× latency bug** in my own production system — [read the postmortem →](https://medium.com/@neeravjha444/i-built-a-free-llm-gateway-then-my-own-load-test-exposed-an-8-latency-bug-f5fd25ce5863)
- 🌱 Focused on backend engineering, system design & data workflows
- ⚽ Fun fact: I debug code like I dribble — fast but controlled

<br clear="right">

---

## 📝 Latest Write-Up

### [I Built a Free LLM Gateway — Then My Own Load Test Exposed an 8× Latency Bug](https://medium.com/@neeravjha444/i-built-a-free-llm-gateway-then-my-own-load-test-exposed-an-8-latency-bug-f5fd25ce5863)

A production debugging story: a cache-hit endpoint that should never touch an LLM was clocking **p50 = 3,802ms**. The culprit — a fresh `httpx.AsyncClient()` (and a fresh TLS handshake) spun up on *every single Redis call*. One connection-pooling fix later:

| Metric | Before | After | Change |
|:---|:---:|:---:|:---:|
| **p50 Latency** | 3,802 ms | 473 ms | 🔻 **~8× faster** |
| **Throughput** | baseline | 5×+ | 🔺 **5×+ increase** |
| **Infra upgrade** | — | none | 💸 **$0 spent** |

📖 [Read the full breakdown on Medium](https://medium.com/@neeravjha444/i-built-a-free-llm-gateway-then-my-own-load-test-exposed-an-8-latency-bug-f5fd25ce5863) · ✍️ [More posts on Medium](https://medium.com/@neeravjha444)

---

## 📌 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🩺 [env-doctor](https://github.com/neerav34/env-doctor)

**The ESLint of environment variables.** Catches missing/undocumented env vars before they hit production.

- 📦 Ships as CLI, [VS Code extension](https://github.com/neerav34/env-doctor-vscode), and [GitHub Action](https://github.com/neerav34/env-doctor-action)
- 🔍 Inline warnings + automated PR checks

🔗 [Live landing page](https://env-doctor-web.vercel.app) · 📦 [npm package](https://www.npmjs.com/package/@neerav34/env-doctor)

</td>
<td width="50%" valign="top">

### ⚡ [llm-gateway](https://github.com/neerav34/llm-gateway)

**Multi-provider LLM routing gateway.** The real plumbing behind a production GenAI backend.

- 🔀 Automatic provider failover (Groq → OpenRouter)
- 🧠 Two-layer caching: exact-match + semantic (vector similarity)
- 🚦 Per-key rate limiting, cost tracking, and true SSE streaming

🔗 [Live gateway](https://llm-gateway-rb0k.onrender.com) · 🎥 [90-sec demo](https://www.youtube.com/watch?v=9BZbCSWbZqM) · 💻 [Source](https://github.com/neerav34/llm-gateway)

</td>
</tr>
</table>

---

## 💻 Tech Stack

**Languages:** Python · JavaScript · TypeScript · Java · SQL

**Backend & APIs:** Flask · Node.js · FastAPI · Django · GraphQL

**AI / ML / LLM Tooling:** PyTorch · TensorFlow · LangChain · OpenAI API · Hugging Face · Pandas · NumPy

**Databases:** MongoDB · MySQL · PostgreSQL · Redis

**DevOps & Infra:** Docker · Kubernetes · Terraform · AWS · GitHub Actions · Linux · Git

<details>
<summary>🎨 Show as badges</summary>
<br>

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![TypeScript](https://img.shields.io/badge/typescript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-025E8C?style=for-the-badge&logo=postgresql&logoColor=white)

![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)
![Node.js](https://img.shields.io/badge/node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)

![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![HuggingFace](https://img.shields.io/badge/🤗_HuggingFace-FFD21E?style=for-the-badge)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)

![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

</details>

---

## 📊 GitHub Stats

<p align="center">
  <img height="165em" src="https://github-readme-stats.vercel.app/api?username=neerav34&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" />
  <img height="165em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=neerav34&layout=compact&theme=tokyonight&hide_border=true" />
</p>
<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=neerav34&theme=tokyonight&hide_border=true" alt="streak stats" />
</p>

---

## 🔗 Find Me Elsewhere

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://neerav-portfolio-nine.vercel.app)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/neerav34)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/neerav-jha)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=white)](https://leetcode.com/u/neerav34/)
[![Medium](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@neeravjha444)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/neerav_jha)
