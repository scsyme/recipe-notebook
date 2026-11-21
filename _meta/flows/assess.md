# Assess a recipe after cooking

Scott can report a cook in ordinary language. ChatGPT drafts a dated note recording what changed, what happened and what to try next time. For example, “I spread the second tray thinner and it crisped up better” is useful evidence for the next cook. Keep personal and family details out of the public note unless Scott explicitly asks to include them.

```mermaid
flowchart TD
    A["Scott reports a cook"] --> B["ChatGPT drafts a dated kitchen note"]
    B --> C{"Where should the note go?"}
    C -->|Discuss| D["Review or refine in chat"]
    D --> B
    C -->|Keep privately| E["Save with the Library draft or as a linked note"]
    C -->|Publish| F{"Recipe already on GitHub?"}
    F -->|Yes| G["Append under My kitchen notes"]
    F -->|No| H["Confirm whether to publish the recipe too"]
    H -->|Recipe and note requested| I["Publish recipe with its first cook note"]
    H -->|Keep recipe private| E
    G --> J["Update Tried status and verify recipe and index"]
    I --> J
```

Use the cook date if known. If only the report date is known, label it as such. Preserve the creator's method alongside Scott's observations. A confirmed cook supports a **Tried** update even if the dish turned out poorly.
