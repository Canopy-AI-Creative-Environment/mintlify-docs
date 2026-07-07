# Source: https://docs.flora.ai/nodes/video-node/text-to-video.md

\> For the complete documentation index, see \[llms.txt\](https://docs.flora.ai/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://docs.flora.ai/nodes/video-node/text-to-video.md). # Text to Video ## Summary Text-to-Video models generate videos by taking a text prompt as input, using the prompt to guide scene composition, motion, and style, resulting in dynamic video content that matches the described narrative or visual concept.

![](https://docs.flora.ai/files/IITGotwFud1qz4YICgN2)

\### Parameters These are parameters that are applicable to all our base models.

| Parameter | Type | Effect on Output |
| --- | --- | --- |
| Prompt | Text | The text prompt is processed through the selected model. |
| Aspect Ratio | 
_Landscape_ - _16:9 (576x1024)_,

_Portrait_ - _9:16 (1024x576), Square - 1:1._

 | This changes the output size of the node with a couple of options. |
| Seed | Seed | The seed is a deterministic number that indexes generations from the model. It's typically randomized, but you can set a seed if there's a particular output you're looking for! Keep in mind that all parameters must be the same in order for a given seed's output to persist. |

\### How to use Prompting is everything for Text to Video. Refer to the \[Text to Text\](/nodes/text-node/text-to-text.md) card to explore more workflow combinations, or browse example workflows on the \[Community page\](https://app.flora.ai/community). --- # Agent Instructions This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com. ## Querying This Documentation If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question. Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter: \`\`\` GET https://docs.flora.ai/nodes/video-node/text-to-video.md?ask=&goal= \`\`\` \`ask\` is the immediate question: it should be specific, self-contained, and written in natural language. \`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal. The response will contain a direct answer to the question and relevant excerpts and sources from the documentation. Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.