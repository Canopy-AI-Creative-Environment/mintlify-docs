# Source: https://docs.flora.ai/models/text-models.md

\> For the complete documentation index, see \[llms.txt\](https://docs.flora.ai/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://docs.flora.ai/models/text-models.md). # Text Models Here are all the text models currently available in FLORA.

| Model | Est. time (s) | Description | Best for |
| --- | --- | --- | --- |
| **Claude Opus 4.5** | 25 | Combines maximum capability with practical performance. | In-depth domain expertise, nuanced dialogue, legal or policy analysis, and strategic decision support. |
| **Claude Opus 4.6** | 8 | Anthropic's frontier model, supports adaptive thinking. | Anthropic's frontier model, supports adaptive thinking. |
| **Claude Opus 4.7** | 25 | Flagship model by Anthropic that handles complex, long-running tasks. | Most advanced Anthropic reasoning, complex analysis, and highest-fidelity outputs. |
| **Claude Opus 4.8** | 25 | Anthropic's most capable model for complex reasoning. | Anthropic's most capable model for complex reasoning. |
| **Claude Sonnet 4.5** | 25 | Balanced speed and intelligence. | Balanced performance, creative writing, code generation, and versatile task handling. |
| **Claude Sonnet 4.6** | 8 | State-of-the-art results at fast speeds. | Balanced performance, creative writing, code generation, and versatile task handling. |
| **Claude Sonnet 5** | 35 | State-of-the-art results at fast speeds. | State-of-the-art results at fast speeds. |
| **Gemini 2.5 Pro** | 30 | Google's best for complex reasoning. | Enterprise-scale analytics, multimodal Q&A, detailed data synthesis, and robust safety-critical tasks. |
| **Gemini 3 Flash** | 25 | Transcribe audio files with reasoning. | Instant summarization, real-time assistance, mobile-first interactions, and search tasks. |
| **Gemini 3.1 Pro** | 45 | Google's latest and most capable reasoning model. | Advanced reasoning, complex analysis, and Google's most capable language model. |
| **GPT 4o Mini** | 20 | Fast and affordable for simple tasks. | Quick drafts, instant summarization, lightweight chatbots, and real-time user feedback loops. |
| **GPT-5** | 40 | Advanced reasoning with deep thinking. | Advanced reasoning, long-context analysis, high-precision code generation, and complex multi-step problem-solving. |
| **GPT-5.1** | 30 | OpenAI's advanced reasoning model. | Enhanced reasoning, complex analysis, and multi-step problem-solving with improved accuracy. |
| **GPT-5.2** | 35 | OpenAI’s model marking significant improvements in general intelligence. | Cutting-edge reasoning, highest accuracy, and most capable OpenAI model. |
| **GPT-5.4** | 35 | Versatile text model with advances in reasoning. | State-of-the-art reasoning, maximum accuracy, and OpenAI's flagship model. |
| **GPT-5.5** | 24 | Frontier model suitable for complex professional work. | Frontier model suitable for complex professional work. |
| **o3 Deep Research** | 600 | Use multi-step analysis with web search support. | In-depth research, comprehensive analysis, multi-source synthesis, and complex investigation tasks. |

\--- # Agent Instructions This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com. ## Querying This Documentation If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question. Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter: \`\`\` GET https://docs.flora.ai/models/text-models.md?ask=&goal= \`\`\` \`ask\` is the immediate question: it should be specific, self-contained, and written in natural language. \`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal. The response will contain a direct answer to the question and relevant excerpts and sources from the documentation. Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.