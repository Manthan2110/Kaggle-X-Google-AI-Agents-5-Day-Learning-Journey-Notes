<p align="center">
  <img src="https://img.shields.io/badge/Kaggle%20×%20Google-AI%20Agents%20Intensive-blue?style=for-the-badge">
</p>

<h1 align="center">🤖 Kaggle × Google — 5-Day AI Agents Intensive</h1>
<p align="center">My complete learning journey, structured notes, hands-on codelabs, and capstone project documenting all 5 days of the workshop.</p>

---

## 📌 Table of Contents
- [🚀 About the Program](#-about-the-program)
- [📊 Badges](#-badges)
- [🗂️ Repository Structure](#️-repository-structure)
- [📅 Day-Wise Breakdown](#-day-wise-breakdown)
- [🧩 Capstone Project (Detailed)](#-capstone-project-detailed)
- [📚 Resources](#-resources)
- [🧾 Proof of Participation](#-proof-of-participation)
- [👨‍💻 About Me](#-about-me)
- [⭐ How to Use This Repo](#-how-to-use-this-repo)
- [📩 Connect With Me](#-connect-with-me)

---

## 🚀 About the Program
The **5-Day AI Agents Intensive** by Kaggle & Google is a hands-on workshop focused on building **agentic AI systems** using modern LLM workflows.

Over the span of 5 days, participants learn:
- Agent architecture & cognitive workflow design  
- Tool calling, APIs, and decision loops  
- Memory systems & planning  
- Agent evaluation & debugging  
- Building a complete end-to-end AI agent  

This repository documents everything I learned, practiced, and built during the program.

---

## 📊 Badges
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Days](https://img.shields.io/badge/Days-5-blue)
![Agents](https://img.shields.io/badge/Agentic-AI-orange)
![Google](https://img.shields.io/badge/Google-Workshop-red)
![Kaggle](https://img.shields.io/badge/Kaggle-Learning-blue)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 🗂️ Repository Structure
```bash
📁 kaggle-google-5-day-ai-agents/
│
├── 📁 certificate/
│   └── kaggle_google_ai_agents_certificate.pdf
│   └── README.md
│
├── 📁 Day-1-Introduction-to-Agentic-AI/
│   └── README.md
│   └── day-1a-from-prompt-to-action.ipynb
│   └── day-1b-agent-architectures.ipynb
│
├── 📁 Day-2-Tools-and-Actions/
│   └── README.md
│   └── day-2a-agent-tools.ipynb
│   └── day-2b-agent-tools-best-practices.ipynb
│
├── 📁 Day-3 Context Engineering: Sessions & Memory/
│   └── README.md
│   └── day-3a-agent-sessions.ipynb
│   └── day-3b-agent-memory.ipynb
│
├── 📁 Day-4 : Agent Observability & Agent Evaluation/
│   └── README.md
│   └── day-4a-agent-observability.ipynb
│   └── day-4b-agent-evaluation.ipynb
│
├── 📁 Day-5 : Agent2Agent Communication & Agent Deployment directory/
│   ├── README.md
│   └── day-5a-agent2agent-communication.ipynb
│   └── day-5b-agent-deployment.ipynb
│
├── 📁 resources
│   ├── slides/
│   └── screenshots/
│
├── LICENSE
├── .gitignore
└── README.md
```

---

## 📅 Day-Wise Breakdown

### **Day 1 – Introduction to Agentic AI**
- Understanding what AI Agents are & how they differ from traditional LLM apps
- Agent loops: perception → reasoning → action → feedback
- Building your first agent using ADK + Gemini
- Mini Task: Create a basic single-agent reasoning workflow

---

### **Day 2 – Tools, Actions & Multi-Agent Basics**
- Using tools: Google Search, custom APIs, structured tool schemas
- Developing tool-aware autonomous agents
- Introduction to multi-agent architectures (roles, communication, routing)
- Mini Task: Build a tool-enabled agent + simple multi-agent team

---

### **Day 3 – Memory & Planning**
- Short-term, long-term, episodic, and vector-based memory systems
- Planning: subgoals, multi-step reasoning, execution loops
- Improving agent consistency & adaptability using memory
- Mini Task: Build an agent with memory + a planning-driven workflow

---

### **Day 4 – Observability & Evaluation**
- Logging, monitoring & tracing agent behavior (Agent Observability)
- Evaluating agent reliability using metrics & structured tests
- Safety, governance, and guardrails for agent actions & tool usage
- Mini Task: Evaluate an agent, find weak spots, and improve performance

---

### **Day 5 – Agent Communication & Deployment**

- Building agent-to-agent communication workflows for collaboration
- Designing role-based multi-agent systems (planner, researcher, evaluator, etc.)
- Deploying agents as production-ready services using ADK (REST APIs, configs, runtime)
- Mini Task: Create a communicating multi-agent system and deploy it as an API
_Add your architecture, flow, tools used, and results here._

---

## 🧩 Capstone Project (Detailed)
> This project builds InsightForge AI, a fully automated multi-agent data analyst capable of performing end-to-end data exploration in seconds. It integrates specialized agents for EDA, visualization, ML feature importance, clustering, and AI-powered insight generation using LLMs. The system produces interactive dashboards, intelligent summaries, and a structured analytical report from a single dataset upload. A natural-language chat interface allows users to query the dataset conversationally. The solution demonstrates the practical application of agentic AI architecture, turning raw data into actionable insights effortlessly.

### **1. 🧠 Problem Statement**

Traditional EDA is slow, repetitive, and requires coding skills that many beginners and business users lack. Analysts spend significant time cleaning data, generating charts, and interpreting patterns.  
**InsightForge AI** automates this entire workflow, making insights accessible instantly and eliminating the need for manual coding or complex data exploration.

---

### **2. 🏗 Architecture Diagram (Text Summary)**
```bash
User Upload
↓
Data Loader Agent
↓
EDA Agent
↓
Visualization Agent
↓
ML Agent (Feature Importance)
↓
Clustering Agent (PCA + KMeans)
↓
LLM Insights Agent
↓
Report Agent
↓
Streamlit Dashboard + Chat Interface
```


Each agent performs a specialized task and passes results through a shared context, forming a seamless **multi-agent analytics pipeline**.

---

### **3. 🔧 Tools & Memory Used**

- **LLMs:** Gemini / OpenAI (insight reasoning + chat interface)  
- **Libraries:** Pandas, NumPy, Scikit-learn, Plotly  
- **Framework:** Streamlit for interactive UI  
- **Memory:** Shared AgentContext storing dataset, stats, plots, reports & insights  
- **ML Models:** RandomForest (feature importance), PCA + KMeans (clustering)

---

### **4. 🚀 Final Workflow Summary**

Once a CSV is uploaded, **InsightForge AI** automatically:

1. Loads and validates the dataset  
2. Performs full EDA and computes statistics  
3. Generates interactive Plotly visualizations  
4. Produces rule-based + LLM-powered insights  
5. Computes ML feature importance  
6. Performs PCA-based clustering with explanations  
7. Generates a structured analytical report  
8. Enables natural-language chat with the dataset  

**All of this happens in just a few seconds.**

---

### **5. 📤 Output Examples**

- 📊 **Interactive Visualizations:** histograms, boxplots, heatmaps, violin plots, PCA cluster plots  
- 📈 **ML Outputs:** feature importance bar chart  
- 🧠 **AI Insights:** trend summaries, outliers, correlations, patterns  
- 📄 **Report Generation:** clean structured EDA report with tables & charts  
- 💬 **Chat Interface:** dataset-grounded natural-language answers  

GitHub Repo of Project : [Link](https://github.com/Manthan2110/MultiAgent-Analytics-Suite)

---

## 📚 Resources
- Kaggle Learn: AI Agents  
- Google Developers: Agentic AI Documentation  
- LLM safety & evaluation guides  
- Codelab notebooks  

---

## 🧾 Proof of Participation
This repository publicly documents all **5 days of the AI Agents Intensive**, including:
- Notes  
- Tasks  
- Code  
- Screenshots (optional)  
- Capstone project  

_This repo acts as open proof of attendance and completion._

---

## 👨‍💻 About Me
I am passionate about **AI/ML Engineering, LLMs, and Agentic AI systems**.  
This workshop strengthens my ability to design **end-to-end agent workflows** and apply agentic intelligence to real-world problems.

---

## ⭐ How to Use This Repo
- Explore each day's folder  
- Review code labs  
- Study architecture diagrams  
- Clone and modify the agent examples  
- Use this as a reference for building your own agents  

---

## 📩 Connect With Me
- **LinkedIn:** [My LinkedIn profile ](https://www.linkedin.com/in/manthanjadav/)
- **Kaggle:** [My Kaggle profile ](https://www.kaggle.com/manthan2110) 
- **GitHub:** [My GitHub profile](https://github.com/Manthan2110)  

---

### ⭐ If you find this helpful, consider giving the repo a star!

