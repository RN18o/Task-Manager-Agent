# Task-Manager-Agent

Task-Manager-Agent is an AI-powered engineering project planner that transforms user requirements into fully structured implementation plans and generates complete projects. It leverages LangGraph for agentic workflows and Google's Generative AI to intelligently decompose complex projects into manageable tasks.

## 🏗️ Architecture

- **Planner Agent** – Analyzes your request and generates a detailed project plan.
- **Architect Agent** – Breaks down the plan into specific engineering tasks with explicit context for each file.
- **Coder Agent** – Implements each task, writes directly into files, and uses available tools like a real developer.

<div style="text-align: center;">
    <img src="image.png" alt="Coder Agent Architecture" width="90%"/>
</div>

## Features

- **AI-Powered Planning**: Uses Google's Gemini 2.5 Flash to understand project requirements and generate structured plans
- **Multi-Agent Workflow**: Implements a sophisticated agent-based system with specialized roles:
  - **Planner Agent**: Converts user prompts into comprehensive project plans
  - **Architect Agent**: Transforms plans into detailed task-based implementation steps
  - **Coder Agent**: Executes implementation tasks using available tools
- **Structured Output**: Uses Pydantic models for type-safe data structures throughout the pipeline


## Requirements

- Python >= 3.13
- Required dependencies (see `pyproject.toml`):
  - langchain >= 1.0.8
  - langgraph >= 1.0.3
  - langchain-google-genai >= 3.1.0
  - openai >= 2.8.1
  - pydantic >= 2.12.4
  - python-dotenv >= 0.9.9

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Task-Manager-Agent
```

2. Install dependencies:
```bash
pip install -r requirements.txt
# or using poetry
poetry install
```

3. Set up environment variables:
Create a `.env` file in the root directory with your API keys:
```
GOOGLE_API_KEY=your_google_api_key
OPENAI_API_KEY=your_openai_api_key (optional)
```

## Usage

Run the project planner from the command line:

```bash
python main.py

```

### 🧪 Example Prompts
- Create a to-do list application using html, css, and javascript.
- Create a simple calculator web application.
- Create a simple blog API in FastAPI with a SQLite database.

Thanks 🙏


