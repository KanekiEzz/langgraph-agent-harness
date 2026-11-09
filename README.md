# LangGraph Agent Harness Demo

A minimal Python example demonstrating **Harness Engineering** concepts built on top of **LangGraph** and **LangChain** using a local Ollama model (`qwen3`).

##  Concepts Covered
- **State Management**: Using `AgentState` to track messages and step counts.
- **Execution Limits**: Preventing infinite loops with `MAX_STEPS`.
- **Tool Permissions**: Enforcing authorized tool usage via standard Harness controls (`ALLOWED_TOOLS`).
- **Observability**: Intercepting and logging execution states.

##  Quickstart

```bash
# 1. Install dependencies
pip install -U langchain langchain-ollama langgraph

# 2. Pull local LLM
ollama pull qwen3:8b

# 3. Run the harness demo
python main.py