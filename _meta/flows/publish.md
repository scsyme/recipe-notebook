# Publish a recipe to GitHub

Start here when Scott asks to add, save or publish a recipe to the notebook. A chat extraction and a private Markdown draft are equally valid starting points.

```mermaid
flowchart TD
    A["Scott requests publication"] --> B["Read the chat recipe or Library draft"]
    B --> C["Check current main by source link and dish"]
    C --> D{"Matching recipe?"}
    D -->|Yes| E["Compare with the existing recipe and cook notes"]
    D -->|No| F["Prepare a new recipe file and index entry"]
    E --> G{"Anything to update?"}
    G -->|No| J["Return the existing GitHub link"]
    G -->|Yes| H["Update the recipe and index as needed"]
    F --> I["Commit and verify on GitHub"]
    H --> I
    I --> J
```

Keep source attribution and meaningful uncertainties. Check for useful [kitchen pairings](../recipe-guidance.md#kitchen-pairings). After a write, read back the recipe and check its README link on `main`. GitHub holds the published version. If an earlier Library draft turns up later, compare it with the live recipe before using it.
