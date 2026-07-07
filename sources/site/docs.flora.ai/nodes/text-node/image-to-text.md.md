# Source: https://docs.flora.ai/nodes/text-node/image-to-text.md

\> For the complete documentation index, see \[llms.txt\](https://docs.flora.ai/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://docs.flora.ai/nodes/text-node/image-to-text.md). # Image to Text ## Summary By connecting an image node to a text node, you can extract information from visual content, style, and composition. You can also get creative in your ask to abstract the visual information from the image node.

![](https://docs.flora.ai/files/qnMHuVd97kkR9UUtxD5Y)

"Give me a visual analysis on the visual style and composition of this image"

![](https://docs.flora.ai/files/sHFMoKrS0Pi127i6aqoX)

"Capture the mood of this image in a haiku"

\## Prompt \* "Describe this image in a few sentences", \* "What hidden rhythm flows through this scene?", \* "Give me a visual analysis of the composition of this image", \* "Conjure a visual poem for this". \*\*\* --- # Agent Instructions This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com. ## Querying This Documentation If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question. Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter: \`\`\` GET https://docs.flora.ai/nodes/text-node/image-to-text.md?ask=&goal= \`\`\` \`ask\` is the immediate question: it should be specific, self-contained, and written in natural language. \`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal. The response will contain a direct answer to the question and relevant excerpts and sources from the documentation. Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.