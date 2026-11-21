# Keep a snapshot of the published notebook

This optional flow starts when Scott asks for an archive. Its purpose is to make one known revision available as a file for offline use or later reference. The archive covers the public GitHub repository at the specified revision. Private recipe drafts and unpublished assessments stay separate.

```mermaid
flowchart TD
    A["Scott requests a snapshot"] --> B["Resolve GitHub main to a commit SHA"]
    B --> C{"Matching snapshot already in Library?"}
    C -->|Yes| D["Check the saved revision and return its link"]
    C -->|No| E["Export the files at that exact commit"]
    E --> F["Open the ZIP and check its contents against the revision"]
    F --> G["Save the dated ZIP in ChatGPT Library"]
    G --> H["Return the file link and commit SHA"]
    H -->|Offline use| I["Scott downloads a local copy"]
```

Use a name such as `recipe-notebook-YYYY-MM-DD-<short-sha>.zip` and record the full commit SHA. A ZIP captures the files at one revision. For local work that needs branches and commit history, use a Git clone. Read live `main` before making later publication decisions because the snapshot may be older.
