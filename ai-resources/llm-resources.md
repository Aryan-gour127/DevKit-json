# LLM resources

Provider capabilities, model names, quotas, and prices change frequently. Treat vendor comparison pages as snapshots and confirm details in current API documentation.

| Resource | Useful for | Pricing and limits |
| --- | --- | --- |
| [OpenAI API docs](https://platform.openai.com/docs/) | Models, API usage, structured outputs, and tool calling | API usage is billed by current pricing; check eligibility and rates |
| [Anthropic API docs](https://docs.anthropic.com/) | Claude models, messages API, and tool use | Usage and plan terms vary; consult current pricing |
| [Google Gemini API docs](https://ai.google.dev/gemini-api/docs) | Gemini API, structured output, and function calling | Free quotas and paid usage may apply; verify current limits |
| [Hugging Face model hub](https://huggingface.co/models) | Discovering model cards and associated artifacts | Public models may be free to access; gated downloads and hosted inference can have limits or costs |
| [OpenRouter](https://openrouter.ai/) | Accessing models through a unified API | Provider/model pricing varies; review routing and data terms |

## Concepts to compare

- **Context window:** Maximum input/output context supported for a model or request.
- **Structured output:** Constraining generated responses to a declared format; validate results regardless.
- **Tool/function calling:** Model-proposed structured calls that application code must validate and authorize.
- **Evaluation:** Measure quality against representative test cases, not anecdotes alone.
- **Data handling:** Check retention, training use, residency, and deletion policies for each provider.

Do not infer model quality or privacy from a name, benchmark, or free quota alone.
