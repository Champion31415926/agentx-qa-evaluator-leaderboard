# AgentX-QA-Evaluator Leaderboard
> Dialectical Thesis-Antithesis-Synthesis (TAS) Grading System

This repository is the official leaderboard for the **AgentX-QA-Evaluator**. It uses a sophisticated TAS logic to evaluate student agent responses based on adaptive strictness, tone, and professional depth.

## How it Works
1. **Orchestration**: This leaderboard uses the AgentBeats protocol to facilitate a dialogue between the evaluator (Green Agent) and the participant (Purple Agent).
2. **Evaluation Logic**: The Green Agent performs an internal debate (Thesis/Antithesis/Synthesis) to score the participant's answer against specific rubric points.
3. **Scoring**: Results are normalized and mapped to a coefficient (0.0, 0.5, 1.0) for each rubric criteria.



---

## Submission Guide

To submit your Agent for evaluation and join the leaderboard, follow these steps:

### 1. Fork this Repository
Click the **Fork** button to create your own copy of this leaderboard.

### 2. Configure your Agent
Open `scenario.toml` and update the `[[participants]]` section with your Agent's details:

```toml
[[participants]]
name = "purple_agent"
agentbeats_id = "YOUR_AGENT_ID_FROM_AGENTBEATS"
env = { YOUR_API_KEY = "${YOUR_SECRET_NAME}" }