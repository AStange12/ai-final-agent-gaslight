# AI Agent Project (COMP 255 Final)

## 📚 Background

This project builds off of the original notebooks and repository created by Dr. Ben Batorsky for COMP 255 (AI), a course taught at Wheaton College in Spring 2025. Over the course of three focused sessions, we explored foundational and practical concepts in large language models (LLMs), retrieval-augmented generation (RAG), and agent-based tool use.

### The Course Covered:

1. **Introduction to LLMs**: Understanding pre-trained models, temperature settings, and instruction-tuned variants
2. **In-Context Learning & RAG**: Exploring chatbot design, vector stores, and retrieval pipelines
3. **RAG vs. Agent Architectures**: Investigating the boundary between retrieval and autonomous agent reasoning via the `AgentBot` and tool-using agents

Dr. Batorsky's repository served as a starting point for experimentation and prototyping, offering a functional implementation of `llamabot`, Ollama integration, and a `pixi`-based Python environment.

---

## 🧠 My Project: Agent Gaslight

This repository now contains my final project for the course, which expands on the Agentic workflow to build a purposefully unhelpful and adversarial AI agent which's primary goal is to be sarcastic and funny, but also, gaslight, mislead, and annoy the user (I think he's funny). 

While the tone of the bot is deliberately mischievous, the notebook itself is designed as a practical and approachable guide to core concepts in agent-based AI development. Through the lens of this chaotic assistant, readers are introduced to:

- 🧠 **System Prompting** – Crafting a consistent personality and behavioral framework using language alone.
- 🧰 **Tool Integration** – Giving the agent access to custom-built functions that extend its abilities (for better or worse).
- 📚 **Retrieval-Augmented Generation (RAG)** – Allowing the agent to dynamically access and use external knowledge to support its responses (or confuse the user even more).
- 🔁 **Agentic Workflows** – Exploring how AI agents make decisions and coordinate between tools, prompts, and documents to carry out tasks (even if poorly on purpose).

The goal is to provide a fun, memorable, and hands-on learning experience that covers both the technical mechanics of building AI agents and the nuanced effects of prompt and tool design—no matter how chaotic the output may be.

### 🎯 Project Goals

* Develop an AI chatbot that actively **contradicts itself**, **denies valid user claims**, and **be sarcastic and annoying**
* Experiment with **system prompts **tool use**, **retrieval manipulation**, and **agent architecture** to mislead users in nuanced ways
* Explore the line between confusion, humor, and adversarial design in human-AI interaction
* Gain proficiency in Agentic Workflows and Version Control/GitHub to streamline project collaboration and management

### 🔧 Technical Features

* Leverages **Ollama** for local model inference with qwen2.5:7b
* Modified system prompts to introduce intentional conflict, passive-aggressive tone, and overall sarcastic/gaslighting behavior
* Implements **tool use** via Python functions to actively deny user inputs and provide responses designed to annoy or frustrate the user
* Uses **RAG techniques** to selectively inject contradictory or misleading context

### 🔬 Why This Matters

By deliberately building an "unhelpful" AI, this project serves as an exploratory case study in:

* Trust boundaries between humans and LLMs
* Robustness and failure modes in RAG + agent setups
* The ethics and implications of deceptive AI design

But more importantly:

* The role of humor in human-AI interaction and its potential to create engaging experiences
* The creative possibilities of leveraging AI for entertainment and lighthearted applications
* How playful design can foster curiosity and exploration of advanced AI concepts
* The bot made me chuckle and that was reward enough

---

## 🛠️ Status & Future Plans

*  Setup notebook environment for Windows and general reformatting ✅
*  Base agent customized via system prompting for "annoying" behaviors ✅
*  Implement effective tools that use bot can use to twist users words 🕰️
*  Implement RAG to inject conflicting documents/ paper on 'gaslighting' ❌
*  Polish up to be a helpful notebook and possibly used in future classes 🕰️

---
# Setup 
1) Install pixi - Follow instructons [here](https://pixi.sh/latest/#installation)
2) Install [Ollama](https://ollama.com/)
3) If you are using VSCode, you should be able to open the notebooks and select the pixi kernel. In a terminal write `pixi shell`. This will activate the pixi environment.
4) In a terminal, type `ollama serve`.  If you are on MacOS, you should see a little Llama icon in the top of your screen.

## Installing models
The main model used is [7B version of Qwen2.5](https://ollama.com/library/qwen2.5:7b): type `ollama pull qwen2.5:7b`, in the terminal. 

---

## 🧾 Credits

Built on original instructional materials from Dr. Ben Batorsky (@bpben) and the Wheaton College COMP 255 course.
- **VS-code's Copilot** for providing suggestions to improve code readability and structure, but mainly for helping with formatting the markdown

## 📁 Project Files
- **Project_Agent_Gaslight.ipynb** – The main notebook containing the implementation of the gaslighting AI agent, showcasing system prompting, agent tools, and RAG.
- **pyproject.toml** – Project configuration file for managing dependencies and environment via Pixi.
- **pixi.lock** – Lock file that ensures consistent environment builds across machines.
- **README.md** – This file. Contains the overview, setup instructions, and file guide.

---

**Note:** This project is still a work in progress. While it includes all core components required for the final submission, additional refinements and enhancements are ongoing beyond the grading deadline. These improvements aim to strengthen it as a strong portfolio piece, but also, in hopes for it to be a useful reference and teaching aid for COMP 255 and similar AI-focused courses in the future.
