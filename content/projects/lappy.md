### LAPPY — AI Data Analysis Bot
**Western Formula Racing | Python / LangGraph / Slack / Gemini / Cohere**

AI-powered data analysis agent for the WFR telemetry team. Engineers ask questions in plain English via Slack; Lappy generates Python code in a sandboxed environment, queries TimescaleDB, and returns plots and insights directly to the channel.

### Architecture
- Custom Python package (`Slicks`) for secure TimescaleDB access
- LangGraph self-directed feedback loops for iterative code correction
- Two RAG systems: sensor/run context RAG (resolves ambiguous references like "front left temp from last Thursday") and feedback-loop RAG (stores approved queries for future reuse)
- Gemini + Cohere APIs for code generation and embedding

### Impact
- First time non-coding engineers on the team did analysis beyond Excel
- Continuously improving hit rate through engineer-validated query memory
- Core part of the first fully validated DAQ system WFR has had
