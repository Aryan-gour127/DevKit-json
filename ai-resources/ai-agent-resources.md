# AI agent resources

An agent system combines a model with instructions, tools, and a control loop. Tool calls can have real-world effects; validate inputs, restrict permissions, and require confirmation for consequential actions.

| Resource | Useful for | Pricing |
| --- | --- | --- |
| [LangGraph](https://langchain-ai.github.io/langgraph/) | Stateful agent and workflow orchestration | Open-source framework; model/provider usage may cost |
| [Microsoft Agent Framework](https://learn.microsoft.com/en-us/agent-framework/overview/) | Building agentic applications in Microsoft ecosystem | Documentation free; hosted services may incur charges |
| [Model Context Protocol](https://modelcontextprotocol.io/) | Standard patterns for connecting models to tools and context | Open specification; implementations have separate terms |
| [LlamaIndex](https://docs.llamaindex.ai/) | Data-connected LLM applications and retrieval | Open-source library; hosted offerings and model usage may cost |
| [OpenAI Agents SDK](https://openai.github.io/openai-agents-python/) | Agent handoffs, tools, and traces in Python | SDK open source; API model use is separately billed |

## Design checklist

- Define narrow tool schemas and validate all arguments.
- Apply least privilege and isolate untrusted content.
- Treat retrieved documents and model output as untrusted input.
- Bound retries, steps, time, and spending.
- Keep logs free of secrets; evaluate failures and unsafe actions.
- Require human review for external messages, financial operations, or destructive changes.

## Retrieval-augmented generation (RAG)

RAG retrieves source passages and supplies them to a model to ground answers. It is not a guarantee of correctness: evaluate retrieval quality, access controls, freshness, citations, and prompt-injection risks.
