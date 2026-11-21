# Extract a recipe and keep a draft

A bare recipe link starts an extraction. The same flow works for a recording, screenshot or recipe page. ChatGPT checks the current [recipe guidance](../recipe-guidance.md), gathers the available evidence and shows a cookable recipe or a clearly labelled partial extraction.

```mermaid
flowchart TD
    A["Scott shares a recipe source"] --> B["ChatGPT checks the source and alternatives"]
    B --> C{"Enough detail to cook?"}
    C -->|Yes| D["Show the recipe in chat"]
    C -->|Gaps remain| E["Show verified details and name the gaps"]
    E -->|Scott supplies more evidence| B
    D --> F{"What does Scott want next?"}
    E --> F
    F -->|Review later| G["Leave the extraction in chat"]
    F -->|Keep a private draft| H["Save Markdown in ChatGPT Library"]
    F -->|Publish| I["Start the GitHub publication flow"]
```

“Keep this as a private draft” gives the recipe a durable file before publication. Use one Markdown file per draft with the source link, the extraction and any open questions. Return the file link so Scott can resume from it later. A plain “save this” follows the project's existing [publication flow](publish.md).
