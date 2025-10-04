# 🧰 Usage and Installation Guide  
### *Principles of Building AI Agents (Second Edition)*

This guide explains how to **set up, explore, and extend** this repository — the practical companion to Sam Bhagwat’s *Principles of Building AI Agents (2nd Edition)*.  
Use it to install dependencies, run examples, and understand how the repository is organized.

---

## ⚙️ 1. Prerequisites

Before you start, make sure your environment meets these requirements:

| Tool | Description |
|------|--------------|
| [Node.js](https://nodejs.org/) v18+ | Runtime environment for JavaScript-based examples |
| npm or [Yarn](https://yarnpkg.com/) | Package manager |
| [Git](https://git-scm.com/) | Version control system |
| [VS Code](https://code.visualstudio.com/) | Recommended text editor |

Optional (for advanced experiments):
- Access to model APIs (OpenAI, Anthropic, etc.)  
- Python 3.10+ (if exploring hybrid or RAG-based examples)  
- [Docker](https://www.docker.com/) (for containerized agent demos)

---

## 🧩 2. Clone the Repository

```bash
git clone https://github.com/<your-username>/principles-of-building-ai-agents.git
cd principles-of-building-ai-agents
```

---

## 📦 3. Install Dependencies

Install all required packages to run or extend the code examples:

```bash
npm install
# or
yarn install
```

If you’re only exploring documentation or markdown summaries, installation isn’t required.

---

## 🔑 4. Environment Variables

Some examples may require API keys for model access.  
Use the provided `.env.example` file as a template:

```bash
cp .env.example .env
```

Then edit your `.env` file with valid keys:

```
OPENAI_API_KEY=your-openai-key
ANTHROPIC_API_KEY=your-anthropic-key
```

> ⚠️ **Important:** Your `.env` file is ignored by Git and should never be committed.

---

## 🚀 5. Explore the Repository

### Structure Overview

| Folder | Purpose |
|--------|----------|
| `summaries/` | Chapter-by-chapter summaries and conceptual notes |
| `exercises/` | Practical examples for each book section |
| `scripts/` *(optional)* | Shared logic or utilities for demos |
| `BOOK_SUMMARY.md` | Complete conceptual overview of all nine parts |
| `README.md` | Project overview and purpose |
| `USAGE_AND_INSTALL.md` | This setup and usage guide |

---

## 🧠 6. Running Examples

Once dependencies are installed, run examples directly from the terminal:

```bash
npm run start
# or run a specific example
node ./exercises/part-01-basic-agent/index.js
```

Each exercise demonstrates one or more concepts from the book such as:
- Prompting and structured outputs  
- Tool invocation and error handling  
- Memory and RAG  
- Multi-agent collaboration  

---

## 🧭 7. Learning Path

Follow this order to align with the book’s chapters:

| Book Part | Folder | Concept |
|------------|---------|----------|
| I | `/exercises/part-01-basic-agent` | Agent fundamentals & prompting |
| II | `/exercises/part-02-agent-design` | Reasoning loops & planning |
| III | `/exercises/part-03-tools` | Tool use & interface design |
| IV | `/exercises/part-04-workflows` | Control flow & orchestration |
| V | `/exercises/part-05-rag` | Retrieval-Augmented Generation |
| VI | `/exercises/part-06-multi-agent` | Multi-agent collaboration |
| VII | `/exercises/part-07-evals` | Evaluation & benchmarking |
| VIII | `/exercises/part-08-deployment` | Deployment & scaling |
| IX | `/exercises/part-09-future` | Multimodality & next-gen concepts |

---

## 🔧 8. Testing and Validation (Optional)

If you plan to add automated tests (e.g., with Jest):

```bash
npm test
# or
npx jest
```

Use this to validate your agent logic, outputs, or API integrations.

---

## 🧱 9. Extending the Project

To create your own experiments:

1. Duplicate one of the `exercises/` folders.  
2. Modify the logic or configuration for your use case.  
3. Add explanations or comments linking it back to book concepts.  
4. (Optional) Document your example in `/summaries/` for future reference.

---

## 🤝 10. Contributing

Contributions are welcome!  
You can propose new examples, expand documentation, or fix issues.

Steps:
```bash
# 1. Fork the repository
# 2. Create a branch for your contribution
git checkout -b feature/new-example

# 3. Commit your changes
git commit -m "Add new example: agent planning loop"

# 4. Push and open a PR
git push origin feature/new-example
```

---

## 🧩 11. Troubleshooting

| Problem | Possible Solution |
|----------|-------------------|
| `Error: Cannot find module` | Run `npm install` again |
| API call failing | Check your `.env` configuration |
| Node version mismatch | Use `nvm use 18` or higher |
| Permission denied | Run `chmod +x` on scripts if needed |

---

## 🪶 12. License and Attribution

This repository is **educational and non-commercial**, inspired by  
**Sam Bhagwat — _Principles of Building AI Agents (2nd Edition)_**

See [LICENSE](./LICENSE) for usage terms.

---

## 💬 13. Feedback and Support

If you find issues or have ideas for improvement:
- Open a [GitHub Issue](../../issues)  
- Suggest new exercises or topics  
- Share feedback through discussions  

---

© 2025 — Educational repository inspired by *Principles of Building AI Agents (2nd Edition)* by Sam Bhagwat.
