# Personal Agentic AI Chatbot

A powerful, customizable AI chatbot with web search capabilities, built using LangGraph, LangChain, and multiple LLM providers.

## Overview

This project implements an agentic AI chatbot that can:

- Use different language models from Groq and OpenAI
- Perform web searches to provide up-to-date information
- Be customized with different system prompts
- Run as a web application with a Streamlit frontend and FastAPI backend

## Features

- **Multiple LLM Support**: Choose between Groq models (llama-3.3-70b-versatile, mixtral-8x7b-32768) and OpenAI models (gpt-4o-mini)
- **Web Search Integration**: Enable web search capabilities using Tavily Search
- **Customizable System Prompts**: Define your AI agent's personality and capabilities
- **Modern Web Interface**: Easy-to-use Streamlit frontend
- **Robust Backend**: FastAPI server with Pydantic validation

## Architecture

The project consists of three main components:

1. **AI Agent (ai_agent.py)**: Implements the LangGraph agent with LLM integration and search tools
2. **Frontend (frontend.py)**: Streamlit-based user interface for interacting with the AI agent
3. **Backend (backend.py)**: FastAPI server that processes requests from the frontend and communicates with the AI agent

## Installation

1. Clone the repository:

```
git clone https://github.com/MdTanwer/Personal-Agentic-AI-Chatbot.git
cd Personal-Agentic-AI-Chatbot
```

2. Install dependencies:

```
pip install -r requirements.txt
```

3. Set up environment variables:
   Create a `.env` file with your API keys:

```
GROQ_API_KEY=your_groq_api_key
TAVILY_API_KEY=your_tavily_api_key
OPENAI_API_KEY=your_openai_api_key
```

## Usage

1. Start the backend server:

```
python backend.py
```

2. In a separate terminal, start the frontend:

```
streamlit run frontend.py
```

3. Open your browser and navigate to http://localhost:8501

4. Configure your AI agent:
   - Select a model provider (Groq or OpenAI)
   - Choose a specific model
   - Define a system prompt
   - Enable/disable web search
   - Enter your query and click "Ask Agent!"

## Requirements

See `requirements.txt` for a complete list of dependencies. Key requirements include:

- langchain
- langgraph
- streamlit
- fastapi
- openai
- groq

## License

This project is licensed under the terms included in the LICENSE file.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
