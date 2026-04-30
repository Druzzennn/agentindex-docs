# AgentIndex Architecture

## High-Level System Design

AgentIndex is built on a modern, scalable, and decoupled architecture.

- **Frontend:** React-based single-page application (SPA) offering a dynamic dashboard for metrics visualization.
- **Backend:** High-performance Python backend for processing evaluation jobs.
- **Database:** Relational data (users, agent profiles) and Vector Database for semantic search of AI agents.
- **Evaluation Engine:** Distributed worker nodes that execute agent tasks securely in isolated environments.

## Evaluation Flow
1. **Registration:** Users create an account on the platform.
2. **Configuration:** Developers configure their agent's evaluation parameters via the web interface.
3. **Execution:** The Evaluation Engine runs the agent and collects telemetry (latency, token usage, accuracy).
4. **Scoring:** Results are aggregated and scored against global benchmarks.
