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

This repository now contains my final project for the course, which expands on the AgentBot framework to build a purposefully unhelpful and adversarial AI agent which's primary goal is to gaslight, mislead, and annoy the user. The goal of the project is to:

### 🎯 Project Goals

* Develop an AI chatbot that actively **contradicts itself**, **denies valid user claims**, and **be a pain to use**
* Experiment with **system prompts**, **retrieval manipulation**, and **agent architecture** to mislead users in nuanced ways
* Explore the line between confusion, humor, and adversarial design in human-AI interaction
* Gain proficiency in version control and GitHub to streamline project collaboration and management

### 🔧 Technical Features

* Leverages **Ollama** for local model inference with Qwen2.5 and LLaMA 3
* Uses **RAG techniques** to selectively inject contradictory or misleading context
* Modified system prompts to introduce intentional conflict, passive-aggressive tone, and overall sarcastic/gaslighting behavior

### 🔬 Why This Matters

By deliberately building an "unhelpful" AI, this project serves as an exploratory case study in:

* Trust boundaries between humans and LLMs
* Robustness and failure modes in RAG + agent setups
* The ethics and implications of deceptive AI design
* Gain hands-on experience in designing and implementing AI agents with specific behaviors

---

## 🛠️ Status & Future Plans

*  Setup notebook environment for Windows and general reformatting
*  Base agent customized via system prompting for "annoying" behaviors
*  RAG backend being tuned to inject conflicting documents
*  Test, Adjust, Repeat

---
# Setup - needs to be configiured for my project

## Setup with Codespaces
1) Select "use as template" in the top right of [the main page of the repo](https://github.com/bpben/wheaton_llm_class)
2) Click on "Open in a Codespace, which will start a [Github Codespace](https://github.com/features/codespaces)
NOTE: This will take some time on the first run, and it's not clear when the environment is finished building. Leave it for some time before following the directions under "installing models".

## Setup locally
1) Install pixi - Follow instructons [here](https://pixi.sh/latest/#installation)
2) Install [Ollama](https://ollama.com/)
3) If you are using VSCode, you should be able to open the notebooks and select the pixi kernel.  If not, you can use Jupyter Lab installed as part of the pixi environment.  In a terminal write `pixi shell`.  This will activate the pixi environment.  Then write `jupyter lab` and Jupyter Lab will open, allowing you to navigate to the notebooks and run the exercises.
4) In a terminal, type `ollama serve`.  If you are on MacOS, you should see a little Llama icon in the top of your screen.

## Installing models
The main model used is [qwen2.5:1.5b](https://ollama.com/library/qwen2.5:1.5b).  To pull this model run `ollama pull qwen2.5:1.5b`.

To run the first few cells of the first notebook, you will need the [pretrained version of llama 3.2](https://ollama.com/library/llama3.2:1b-text-q5_K_S): `ollama pull llama3.2:1b-text-q5_K_S`.

The agent workflow will likely fail unless you use the [7B version of Qwen2.5](https://ollama.com/library/qwen2.5:7b): `ollama pull qwen2.5:7b`.  Note - this can be used in place of the 1.5b parameter model, but you will need to change the `sft_model` parameter in the notebooks.

To run ALL notebooks:
```
ollama pull qwen2.5:1.5b
ollama pull qwen2.5:7b
ollama pull llama3.2:1b-text-q5_K_S
```

---

## 🧾 Credits

Built on original instructional materials from Dr. Ben Batorsky (@bpben) and the Wheaton College COMP 255 course.