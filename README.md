#  ResumeAgent-CrewAI

**A CrewAI-based multi-agent system for intelligent resume evaluation**

---

## 📌 Overview

**ResumeAgent-CrewAI** is an intelligent multi-agent framework built using [CrewAI](https://github.com/joaomdmoura/crewAI). It uses powerful LLM agents to evaluate candidate resumes for AI/ML job roles and generate appropriate responses—either an acceptance or a polite rejection message.

This project demonstrates how CrewAI and Google Gemini models can streamline resume screening and HR communication using autonomous agents.

---

## 🧪 How It Works

### 👨‍💼 Agents
- **Resume Evaluator Agent**: Determines if a resume fits an AI/ML job role and returns a YES/NO with a brief reason.
- **Reply Writer Agent**: Crafts a clear, professional message to the candidate based on the evaluator’s output.

### 🧾 Workflow
1. Resume text is provided.
2. The **Evaluator Agent** checks job relevance.
3. The **Reply Agent** composes a message based on the result.
4. The Crew executes all tasks sequentially using LLMs.

---

## 🛠️ Tech Stack

| Component      | Description                                 |
|----------------|---------------------------------------------|
| `CrewAI`       | Multi-agent task orchestration              |
| `LangChain`    | LLM tooling and memory/context management   |
| `Google Gemini`| LLM model used via `langchain_google_genai` |
| `Python 3.10+` | Programming language                        |

---

## 📦 Installation

```bash

# Install dependencies
pip install crewai langgraph langchain_community langchain_google_genai
