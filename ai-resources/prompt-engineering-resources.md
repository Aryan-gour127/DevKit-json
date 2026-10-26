# Prompt engineering resources

Prompting is iterative product work, not a replacement for validation, security controls, or evaluation.

| Resource | Useful for | Pricing |
| --- | --- | --- |
| [OpenAI prompt engineering guide](https://platform.openai.com/docs/guides/prompt-engineering) | Instructions, examples, and model-specific prompting | Free documentation; API use billed separately |
| [Anthropic prompt engineering overview](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview) | Prompt structure and Claude-specific techniques | Free documentation; service terms vary |
| [Google prompt design strategies](https://ai.google.dev/gemini-api/docs/prompting-strategies) | Prompting practices for Gemini models | Free documentation; API usage terms apply |
| [Promptfoo](https://www.promptfoo.dev/) | Comparing prompts and running evaluations | Open-source features available; hosted plans may cost |
| [Microsoft prompt engineering](https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/prompt-engineering) | Structured prompts and deployment considerations | Free documentation; Azure usage billed separately |

## Practical workflow

1. State the task, audience, constraints, and output format explicitly.
2. Provide only relevant context and representative examples.
3. Test normal, ambiguous, adversarial, and out-of-scope inputs.
4. Compare outputs with a repeatable evaluation set.
5. Validate structured output in code and reject unsafe actions.

Avoid placing confidential information in prompts unless the service is approved for that data and configured appropriately.
