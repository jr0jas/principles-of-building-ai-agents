# 🧩 General Glossary

### *Principles of Building AI Agents (Second Edition)*

A conceptual index of foundational terms used throughout the book.  
Each definition is concise, context-aware, and aligned with the book’s technical framing.

---

## ⚙️ Core Concepts

### **AI (Artificial Intelligence)**

The science and engineering of building machines capable of performing tasks that require human-like intelligence — including perception, reasoning, learning, and decision-making.  
In the book’s context, **AI** is not limited to static models or chatbots but refers to **systems that think, act, and adapt** based on goals and data.

---

### **LLM (Large Language Model)**

A neural network trained on massive text corpora to understand and generate human-like language.  
LLMs such as GPT or Claude act as the **“cognitive core”** of agents, providing reasoning, planning, and communication abilities.  
They interpret prompts, generate structured responses, and interface with memory and tools through protocols like MCP.

---

### **AI Agent**

A structured system that **reasons, plans, remembers, and acts** toward a goal.  
An agent = **Model (LLM) + Tools + Memory + Workflow**.  
It can use external APIs, recall past experiences, and adapt its behavior dynamically.  
Agents differ from chatbots by having autonomy and compositional intelligence — they can self-reflect, retrieve facts, and collaborate with other agents.

---

## 🧠 Agent Architecture

### **Model**

The cognitive engine or “brain” of the agent (usually an LLM).  
It interprets prompts, generates reasoning steps, and decides which tools to call.

### **Tool**

Any external capability the agent can use — an API, function, or service.  
Tools extend the agent’s reach beyond language, enabling it to access data, perform computations, or take actions in the world.

### **Memory**

The system that stores context and knowledge across time.  
It can include:

* **Working memory:** short-term reasoning buffer.  
* **Session memory:** persistent during interaction.  
* **Long-term memory:** knowledge database or vector store.  
* **Hierarchical memory:** structured across layers for context relevance.

### **Workflow**

The control logic or “operating system” of the agent.  
It defines how reasoning steps, tool calls, and reflections are sequenced — often visualized as directed graphs (DAGs) or flowcharts.

---

## 🔁 Reasoning Patterns

### **Prompting**

The art of instructing an LLM to achieve a desired behavior or output.  
The book treats prompting as a **form of programming**, where inputs are structured (e.g., JSON schemas) to ensure predictability and composability.

### **Reflection**

The process of an agent evaluating its own reasoning or output.  
Reflection enables self-correction, iterative improvement, and meta-cognition.

### **Plan–Act–Observe–Reflect Loop**

The fundamental reasoning cycle.  
An agent plans a task, acts (calls tools or generates outputs), observes the results, and reflects to refine its future behavior.

---

## 📚 Knowledge and Retrieval

### **RAG (Retrieval-Augmented Generation)**

A method where an agent retrieves relevant documents or data before responding.  
It grounds the model’s outputs in factual context, improving accuracy and reducing hallucination.

### **Embeddings**

Numerical vector representations of text that capture meaning.  
Used to compare and retrieve semantically similar information from large knowledge stores.

### **Vector Store**

A database that indexes embeddings, enabling fast similarity search for RAG pipelines.

---

## 🔌 Ecosystem and Protocols

### **MCP (Model Context Protocol)**

A standard communication layer that allows LLMs and tools to interact consistently.  
It defines how tools describe capabilities, handle inputs/outputs, and log actions — creating an **interoperable and auditable agent ecosystem**.

### **A2A (Agent-to-Agent Communication)**

The protocol or framework enabling multiple agents to exchange structured messages, collaborate, and delegate tasks.

---

## 🧩 Multi-Agent Systems

### **Supervisor/Worker Pattern**

A coordination model where one agent oversees others, distributing subtasks and aggregating results.

### **Agent-as-Tool**

When an agent exposes its capabilities as an API so other agents can call it — promoting modularity and reuse.

---

## 🧾 Evaluation and Observability

### **Eval**

An automated framework for testing agent behavior.  
Evals measure correctness, consistency, tone, and reasoning quality, transforming subjective performance into measurable engineering data.

### **Observability**

The practice of tracing and visualizing an agent’s reasoning process.  
It allows debugging, performance optimization, and auditability.

---

## 🚀 Deployment and Scaling

### **Containerization**

Packaging agents into isolated runtime environments (e.g., Docker, Cloud Run) for predictable deployment and scaling.

### **Canary Deployment**

Rolling out new versions of an agent incrementally to monitor safety and performance before full release.

### **Feature Flags**

Toggle mechanisms that control which features or tools are active per environment or user group.

---

## 🌌 Advanced Topics

### **Multimodal Agent**

An AI agent capable of understanding and generating multiple data types (text, image, audio, code).

### **Self-Improvement**

When an agent learns from its traces, reflections, or user feedback to autonomously optimize future behavior.

### **Governance**

Frameworks ensuring agents behave ethically, safely, and in compliance with regulations.  
Includes traceability, accountability, and human-in-the-loop mechanisms.

---

### 💡 Summary Insight

> The glossary reinforces the book’s thesis:  
> **Modern AI agents = cognitive systems engineered for autonomy, collaboration, and reliability — not just language generation.**
