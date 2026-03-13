# 🤖 Generative-Agents: Autonomous LLM Orchestration Framework

[![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://opensource.org/licenses/MIT)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-orange.svg)](https://openai.com/)

**Generative-Agents** is a research-inspired framework for building autonomous agents capable of complex reasoning, long-term memory management, and recursive self-reflection. It provides the building blocks for creating "Smallville"-style simulations or goal-oriented autonomous workers.

## 🌟 Key Features
- **Long-Term Memory:** Vector-database backed memory stream for storing and retrieving past experiences based on relevance, recency, and importance.
- **Reflection Engine:** Periodic self-reflection to generate higher-level insights from raw observations.
- **Hierarchical Planning:** Recursive decomposition of high-level goals into actionable sub-tasks.
- **Tool-Use (Function Calling):** Seamless integration with external APIs and computational tools.

## 🛠️ System Architecture
`	ext
[ Observation ] -> [ Memory Stream ] -> [ Retrieval ]
                        |                   |
                [ Reflection Engine ] <-----|
                        |
                [ Planning Engine ] -> [ Action / Tool Use ]
`

## 📦 Installation
`ash
git clone https://github.com/NavneetPrabhat2/Generative-Agents.git
cd Generative-Agents
pip install -r requirements.txt
`

## 🚀 Usage Example
### Initializing a Generative Agent
`python
from generative_agents import Agent

# Create an agent with a specific personality and goal
agent = Agent(
    name="ResearchBot",
    persona="A meticulous data scientist specializing in quantum computing.",
    memory_config={"vector_db": "chroma"}
)

# Assign a task
agent.observe("User asked to summarize recent breakthroughs in topological qubits.")
plan = agent.plan()
action = agent.act()
`

## 🔬 Research Context
This framework is based on the architecture described in *"Generative Agents: Interactive Simulacra of Human Behavior"* (Park et al., 2023). It extends the concept to include structured tool-use and multi-agent coordination.

---
Developed by **Navneet Prabhat**