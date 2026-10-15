# brain

Personal knowledge base. One repo for everything I learn and collect.

```
brain/
├── claude/
│   ├── conversations/   # exported chats, summaries, memory notes
│   └── projects/        # project instructions, prompts, artifacts
├── obsidian/
│   └── vault/           # copy of the Obsidian vault (markdown)
├── notebooklm/
│   ├── notebooks/       # one folder per notebook (sources + notes)
│   └── exports/         # raw exports (notes, summaries, audio overviews, etc.)
└── inbox/               # drop anything here; sort later
```

## Getting things in

**Claude** – Settings > Privacy > Export data (emailed zip), or paste/save chats as `.md` into `claude/conversations/`.

**Obsidian** – Copy your vault folder into `obsidian/vault/` (or point Obsidian at this folder, or use the Obsidian Git plugin).

**NotebookLM** – There is no direct GitHub sync. For each notebook: copy/save notes (Studio panel > note > "Convert to source"/copy), download sources (PDF, docs), and save Markdown into `notebooklm/notebooks/<notebook-name>/`. Anything you can't sort yet goes in `inbox/`.

Then: `git add -A && git commit -m "add <what>" && git push`.

> Keep this repo **private**. Don't commit passwords, API keys, or other people's private data.
