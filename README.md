# Multi-Agent Planner, Researcher, and Writer using CrewAI

## Overview

This project demonstrates a simple yet powerful multi-agent workflow using the **CrewAI** framework. The system uses specialized AI agents that collaborate to research, plan, write, and refine content on a given topic.

The workflow mimics a real-world content creation team where each agent has a dedicated responsibility and contributes to the final output through a structured sequence of tasks.

## Features

* Multi-agent collaboration using CrewAI
* Automated content planning and research
* AI-powered content generation
* Editorial review and quality assurance
* Structured task orchestration
* SEO-aware content creation
* Modular and extensible architecture

## Architecture

The solution consists of three specialized agents:

### 1. Content Planner

Responsible for:

* Researching the topic
* Identifying current trends and key developments
* Defining target audience
* Creating a detailed content outline
* Suggesting SEO keywords and references

### 2. Content Writer

Responsible for:

* Generating the article based on the planner's output
* Creating engaging and structured content
* Incorporating SEO recommendations
* Maintaining consistency and readability

### 3. Editor

Responsible for:

* Reviewing the generated article
* Correcting grammatical and stylistic issues
* Ensuring adherence to editorial standards
* Producing publication-ready content

## Workflow

```text
Topic Input
      │
      ▼
Content Planner
      │
      ▼
Content Writer
      │
      ▼
Editor
      │
      ▼
Final Article
```

## Technologies Used

* Python
* CrewAI
* CrewAI Tools
* LangChain Community
* OpenAI GPT Models

## Installation

Clone the repository:

```bash
git clone https://github.com/<your-username>/<repository-name>.git
cd <repository-name>
```

Install dependencies:

```bash
pip install crewai==0.28.8
pip install crewai_tools==0.1.6
pip install langchain_community==0.0.29
```

## Configuration

Set your OpenAI API key:

```python
import os

os.environ["OPENAI_API_KEY"] = "YOUR_API_KEY"
os.environ["OPENAI_MODEL_NAME"] = "gpt-3.5-turbo"
```

Alternatively:

```bash
export OPENAI_API_KEY=YOUR_API_KEY
```

## Running the Project

Launch the notebook:

```bash
jupyter notebook
```

Open:

```text
Multi_Agent_Planner,_Researcher_and_Writer_using_CREWAI.ipynb
```

Provide a topic and execute the notebook cells.

Example:

```python
inputs = {
    "topic": "Artificial Intelligence in Banking"
}
```

## Example Use Cases

* Blog generation
* Market research summaries
* Technical article creation
* Product documentation drafts
* Industry trend analysis
* Thought leadership content

## Future Enhancements

* Web search integration
* Retrieval-Augmented Generation (RAG)
* Human-in-the-loop review workflows
* Multi-language content generation
* Agent memory and context persistence
* Knowledge base integration
* Custom tools and MCP server support

## Learning Outcomes

This project demonstrates:

* Multi-agent orchestration patterns
* Agent specialization and delegation
* Sequential task execution
* Prompt engineering techniques
* AI-assisted content generation workflows
* Practical implementation of CrewAI

## License

This project is intended for educational and learning purposes. Feel free to fork, modify, and extend it for your own use cases.
