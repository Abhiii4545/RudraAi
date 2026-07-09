# Rudra AI 🚀

**Rudra AI** is a powerful, self-hosted developer control center for coding agents and automations. It connects your coding agents directly to your workspace, allowing you to run agents like Claude Code, Gemini, OpenAI, or any ACP (Agent-Client Protocol) compatible agent across local, remote, and cloud environments.

With **Rudra AI**, you can convert complex tasks into automated steps, deploy agents inside isolated sandboxes, and integrate them with tools like Slack, GitHub, and Jira.

---

## Key Features

- 🛠️ **Self-Host Anywhere**: Run Rudra AI locally on your machine, in Docker containers, or on private virtual machines.
- ⚡ **Multi-Agent & Multi-Backend**: Switch seamlessly between local runtimes and remote cloud environments.
- 🔄 **Automations**: Create schedules and webhooks to trigger tasks (like compiling reports or running test suites) automatically.
- 🤖 **Bring Your Own Model (BYOM)**: Support for OpenAI, Anthropic, Gemini, local LLMs (via Ollama/LiteLLM), and more.
- 🔒 **Secure Sandboxing**: Keep your host system safe by running agent code inside Docker containers.

---

## Getting Started

### Prerequisites

To run Rudra AI locally from source, you will need:
- **Node.js** 22.12.x or later
- **Python** 3.12 or 3.13
- **Poetry** (Python package manager)
- **Docker** (optional, but highly recommended for sandboxed execution)

---

### Step-by-Step Installation

#### 1. Clone the Repository
```bash
git clone https://github.com/Rudra-AI/Rudra-AI.git
cd Rudra-AI
```

#### 2. Install Dependencies
Build the backend and frontend environments:
```bash
make build
```

#### 3. Run the Servers

##### Run Both Frontend & Backend Together:
```bash
make run
```

##### Run Separately:
- **Backend Only** (port 3000):
  ```bash
  make start-backend
  ```
- **Frontend Only** (port 3001):
  ```bash
  make start-frontend
  ```

---

## Architecture Overview

Rudra AI consists of a Python FastAPI backend and a React (Vite/React Router) frontend:

1. **Rudra AI Backend**: Exposes a REST API to manage agent instances, coordinate communications, and sandbox operations.
2. **Rudra AI Canvas Frontend**: A sleek visual interface that lets you chat with agents, view their workspace, edit files, and check execution logs in real-time.

---

## License

This project is licensed under the MIT License.
