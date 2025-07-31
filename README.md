# Inventory Insight Agent

**Industry:** Retail

**Repository:** [tekvo-ai-hub/retail-inventory-llm](https://github.com/tekvo-ai-hub/retail-inventory-llm)

## Description
Query-based inventory insights using local models and PO logs.

## Requirements
### Functional
- Ingest product and order logs.
- Visualize low-stock items.
- Respond to queries.
### Non-Functional
- Private edge deployment.
- Real-time performance.
- Support CSV input.
## Solution Design
**LLM:** Mistral Instruct v0.2
**Vector DB:** LanceDB

### Components
- CSV Uploader
- Time-Series Visualizer
- RAG Agent
- LLM Query Bot
### Data Flow
$ CSV → Process → Embed → Index → Query → LLM → Output

### Tech Stack
- **Frontend:** Svelte
- **Backend:** Python (FastAPI)
- **Storage:** DuckDB
- **Deployment:** Docker Compose
