# Source: https://docs.flora.ai/editor/toolbar.md

\> For the complete documentation index, see \[llms.txt\](https://docs.flora.ai/llms.txt). Markdown versions of documentation pages are available by appending \`.md\` to page URLs; this page is available as \[Markdown\](https://docs.flora.ai/editor/toolbar.md). # Toolbar ## Summary The toolbar is where you can find the main editor tools.

![](https://docs.flora.ai/files/Nvs1Wo7Nya55cWIlNzKi)

\## Spawning Nodes By clicking the + button on the toolbar you can spawn different types of nodes: Text, Image, Video, and Audio. The add-node menu also includes a \*\*Technique\*\* entry — select it or press \*\*Shift+T\*\* to open a technique picker panel where you can browse, search, and add techniques directly to your canvas.

![](https://docs.flora.ai/files/ypDVEAJffpJv8ny86w6c)

\## Assets By clicking on the Assets button, you can browse all the visual assets you uploaded to the canvas.

![](https://docs.flora.ai/files/ExUn3sQ1ccylYCmZP0RW)

\## Generation History The Generation History button stores all the generated assets from your account, making it seamless for you to transport assets between projects.

![](https://docs.flora.ai/files/xw126y4tABWp9GmHn4Ja)

\## Flows Flows allow you to explore our pre-made workflows for various creative use cases. By \*\*hovering\*\* over the Flows button, you can view recent workflows along with the number of nodes deployed. \*\*Clicking\*\* on the Flows button lets you browse curated categories to find workflows that inspire your creative process.

![](https://docs.flora.ai/files/vaFmGOpwkIo9E3hcSkhF)

\## Split Into Layers The \*\*Split Into Layers\*\* tool lets you decompose an image into separate layer components. Select an image node and click the Split Into Layers button in the toolbar to open a visual cascade picker. Choose how many layers to split into (2–5) from the overlay, and FLORA automatically separates the image into distinct layers that you can edit independently. ## Comment The Comment Button is where you activate the comment cursor. Click on anywhere to start a text bubble and leave a comment for your collaborators.

![](https://docs.flora.ai/files/AbtW7jgnqeWWSWQtkoPB)

\--- # Agent Instructions This documentation is published with GitBook. GitBook is the documentation platform designed so that both humans and AI agents can read, navigate, and reason over technical content effectively. Learn more at gitbook.com. ## Querying This Documentation If you need additional information that is not directly available in this page, you can query the documentation dynamically by asking a question. Perform an HTTP GET request on the current page URL with the \`ask\` query parameter, and the optional \`goal\` query parameter: \`\`\` GET https://docs.flora.ai/editor/toolbar.md?ask=&goal= \`\`\` \`ask\` is the immediate question: it should be specific, self-contained, and written in natural language. \`goal\` is optional and describes the broader end goal you are ultimately trying to accomplish on behalf of the user. GitBook uses it to tailor the answer towards what is most useful for that goal. The response will contain a direct answer to the question and relevant excerpts and sources from the documentation. Use this mechanism when the answer is not explicitly present in the current page, you need clarification or additional context, or you want to retrieve related documentation sections.