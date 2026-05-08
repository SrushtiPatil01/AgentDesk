# AgentDesk

An agentic customer support platform that coordinates specialized AI agents to handle refunds, order tracking, and inventory workflows autonomously.

## Overview

AgentDesk replaces brittle rule-based support flows with a multi-agent system. Each agent specializes in a domain (refunds, orders, inventory) and communicates through the Model Context Protocol (MCP), with Redis maintaining conversational state across turns. The platform is built for low-latency, high-concurrency support workloads.

## Features

- 🤖 **Multi-agent orchestration** — Specialized agents for refunds, order tracking, and inventory queries
- 🔌 **MCP-based tool use** — Agents invoke external systems through a standardized protocol
- 🧠 **Stateful conversations** — Redis-backed memory persists context across user turns
- ⚡ **Sub-3s p95 latency** — Achieved through parallel external API calls and async agent execution
- 🔄 **Task orchestration** — API-driven workflow routing across agents
- 📦 **Container-ready** — Dockerized and deployable on AWS ECS

## Tech Stack

- **Language:** Python
- **Framework:** FastAPI
- **LLM:** OpenAI API
- **Protocol:** Model Context Protocol (MCP)
- **Database:** PostgreSQL
- **Cache / State:** Redis
- **Deployment:** Docker, AWS ECS
