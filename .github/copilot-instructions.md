## Context and Objectives
You are an AI engineer at a mid-sized SaaS company that handles customer
inquiries across multiple departments (HR, IT Support, Finance, Legal).
The support team is overwhelmed with tickets being misrouted—HR
questions end up with IT, financial queries reach the legal team, etc.
Leadership has asked you to build an intelligent routing system that
automatically classifies incoming questions by department and routes
them to specialized AI agents that can provide accurate, context-aware
answers using the company's internal documentation.

The system must handle real customer queries, maintain full
observability for debugging misrouted questions, and automatically
evaluate response quality to catch errors before they reach customers.

### Objectives

- Build a multi-agent orchestration system with an orchestrator that
  classifies user intent and conditionally routes queries to specialized
  RAG agents. This solves the real-world problem of handling diverse
  queries with domain-specific knowledge.

- Implement the entire workflow using LangChain to leverage
  production-grade components (chains, retrievers, agents) rather than
  fragile custom code. This ensures maintainability and follows industry
  standards.

- Instrument complete workflow tracing with Langfuse so engineers can
  debug misclassifications, failed retrievals, and incorrect answers by
  inspecting the full execution path. This enables production monitoring
  and incident response.

- Create specialized RAG agents (minimum 3) with domain-specific
  document collections that ground answers in company documentation.
  This prevents hallucinations and ensures answers reflect actual
  company policies.

- Document your technical decisions explaining why you chose specific
  LangChain components, routing strategies, and RAG configurations. This
  demonstrates engineering judgment beyond just "making it work."

- **(Bonus)** Deploy an automated evaluator agent within Langfuse that
  scores each response on quality dimensions (relevance, completeness,
  accuracy). This catches low-quality answers before customers see them
  and provides continuous quality metrics.

**Why this matters:** Multi-agent systems with proper orchestration,
framework usage, and observability are the foundation of production LLM
applications. This project simulates real enterprise requirements:
handling diverse queries, using existing tools properly (LangChain),
debugging complex workflows (Langfuse), and maintaining quality
standards (evaluation). These skills directly transfer to building
customer-facing AI products.

## Assignment

Develop a Multi-Agent System where an Orchestrator Agent classifies the
user's query intent (e.g., HR or Tech). This classification triggers a
conditional route that delegates the retrieval task to the correct,
specialized RAG Agent for a contextually grounded answer. The entire
dynamic workflow must be implemented using LangChain and fully traced
with Langfuse.

**Bonus:** Deploy an Evaluator Agent within Langfuse to automatically
assign a 1-10 quality score to each RAG response based on the original
query and the final answer.

## Project Deliverables and Submission Requirements
Submit via a public Git repository link of the repository. Ensure the repository is self-contained and runnable.

## Expected repository structure
| **Deliverable**         | **Filename / Format**                                                                                                                                                            | **Minimum Content**                                                                                                                                                                                                                                                |
|-------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Main notebook           | multi_agent_system.ipynb or multiple files: src/multi_agent_system.py, src/agents/orchestrator.py, src/agents/hr_agent.py, src/agents/tech_agent.py, src/agents/finance_agent.py | All implementation in organized notebook sections: <br>(1) Setup & imports, <br>(2) Document loading & vector stores, <br>(3) Agent definitions, <br>(4) Orchestrator & routing, <br>(5) Testing & examples, <br>(6) Langfuse integration. Clear markdown headers separating each section. |
| Document collections    | data/hr_docs/, data/tech_docs/, data/finance_docs/                                                                                                                               | Minimum 50 chunks per domain. Documents in .txt, .pdf, .md, or .csv format. Each folder represents knowledge base for one specialized agent.                                                                                                                       |
| Test queries            | test_queries.json OR defined in notebook                                                                                                                                         | Minimum 10 test queries with expected intent categories. Can be JSON file or dictionary in notebook cell. Cover all agent types and edge cases.                                                                                                                    |
| README                  | README.md                                                                                                                                                                        | Project description, setup instructions (install requirements, set API keys), how to run notebook (cell execution order), usage examples (which cells to run), configuration notes, known limitations.                                                             |
| Dependencies            | requirements.txt                                                                                                                                                                 | langchain, langchain-openai, langfuse, openai, vector store library, tiktoken, python-dotenv, jupyter, ipykernel. Minimum 9 packages.                                                                                                                              |
| Environment template    | .env.example                                                                                                                                                                     | Template showing: <br>OPENAI_API_KEY=your-key-here, LANGFUSE_PUBLIC_KEY=pk-lf-xxx, LANGFUSE_SECRET_KEY=sk-lf-xxx, LANGFUSE_HOST=https://cloud.langfuse.com.                                                                                                        |
| Evaluator agent (BONUS) | In notebook section OR evaluator.py                                                                                                                                              | Evaluator implementation with Langfuse score API. Can be in dedicated notebook section with markdown explanation OR separate.py file imported into notebook.                                                                                                       |

