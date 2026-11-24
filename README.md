# Design Tools

A shared home for the HTML design tools our team has built.

**Live site:** `https://<your-org>.github.io/design-tools/` (update once Pages is on)

## How it's organised

```
design-tools/
├── index.html        ← landing page (lists every tool automatically)
├── tools.json        ← the list of tools — add yours here
├── README.md
└── tools/
    ├── colour-contrast/
    │   └── index.html
    └── spacing-scale/
        ├── index.html
        └── styles.css
```

Each tool lives in its own folder under `tools/`, and its main file must be called `index.html`.

## Adding a tool (no Git needed)

1. **Upload your files.** On your computer, put your tool in a folder named in lowercase with hyphens, e.g. `type-scale-generator`, with the main file called `index.html`. On the repo page, open the `tools` folder, click **Add file → Upload files**, and drag the whole folder in. GitHub keeps the folder structure.
2. **List it on the landing page.** Open `tools.json`, click the ✏️ pencil, and add an entry:
   ```json
   {
     "name": "Type Scale Generator",
     "folder": "type-scale-generator",
     "description": "One sentence on what it does.",
     "author": "Your Name",
     "tags": ["typography"]
   }
   ```
   Put a comma between entries and none after the last one.
3. **Commit.** The site updates in a minute or two.

## Ground rules

- **Self-contained.** Links to files inside your own folder are fine; avoid absolute paths like `/styles.css`, which will break.
- **No secrets.** This repo and site are public — no API keys, client names or confidential work.
- **Edit only your own tool** unless you've agreed otherwise with its author.
- **Use tags** from the existing list where you can (e.g. `colour`, `typography`, `layout`, `accessibility`, `export`).
