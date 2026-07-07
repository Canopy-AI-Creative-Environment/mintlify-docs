# Source: https://docs.flora.ai/models/audio-models.md

\> For the complete documentation index, see \[llms.txt\](https://docs.flora.ai/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://docs.flora.ai/models/audio-models.md). # Audio Models Here are all the audio models currently available in FLORA. ## Speech & Voice These models generate or transcribe speech.

| Model | Est. time (s) | Description | Best for |
| --- | --- | --- | --- |
| **ElevenLabs Multilingual v2** | 15 | Natural text-to-speech with multilingual voice synthesis. | Voiceovers, narration, multilingual content, accessible media. |
| **ElevenLabs Scribe v2** | 10 | Transcribe speech to text. | Transcription, subtitles, meeting notes, content indexing. |
| **Gemini 3.1 Flash TTS** | 10 | Text to speech with prompted expressiveness. | Expressive voiceovers, character dialog, and stylized narration. |

\## Sound Effects & Music These models generate sound effects and music from text prompts.

| Model | Est. time (s) | Description | Best for |
| --- | --- | --- | --- |
| **ElevenLabs Music v1** | 30 | Generate music using a text prompt. | Background tracks, musical stings, and prompt-driven composition. |
| **ElevenLabs Sound Effects** | 15 | Generate sound effects and Foley from text descriptions. | Foley, ambient soundscapes, UI sounds, game audio. |

\--- # Agent Instructions This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com. ## Querying This Documentation If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question. Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter: \`\`\` GET https://docs.flora.ai/models/audio-models.md?ask=&goal= \`\`\` \`ask\` is the immediate question: it should be specific, self-contained, and written in natural language. \`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal. The response will contain a direct answer to the question and relevant excerpts and sources from the documentation. Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.