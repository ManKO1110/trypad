# TryPad

A lightweight, offline **Notion-style notes app** that runs entirely in the browser (HTML + CSS + JS only).

Notes are saved as **Markdown (`.md`) files** on your local disk, with a folder structure that mirrors page hierarchy.

## Features

- Hierarchical pages & sub-pages (collapsible tree)
- Rich text editing (bold, italic, headings, lists, quotes)
- Notion-style typing shortcuts (`-` + space → bullet, `#` + space → heading, …)
- Image upload + free resize (size remembered after save)
- Tables with add/remove row & column, **Tab** to move between cells
- Search across all pages and sub-pages
- Resizable left sidebar
- Local folder storage via File System Access API (Chrome / Edge)
- Remembers last folder (one-click reconnect)

## Requirements

- **Chrome** or **Edge** (File System Access API)
- Not fully supported in Firefox / Safari for local folder saving

## Usage

1. Open `index.html` in Chrome or Edge
2. Click **Select Folder…** and choose a folder for your notes
3. Create pages, write, insert images/tables
4. Next time you open the app, click **Reconnect** (or it may auto-connect if permission is still granted)

### Suggested layout

```text
TryPad/
  index.html          ← this app
  Notes/              ← select this folder in the app
    Welcome.md
    Projects.md
    Projects/
      Alpha.md
```

## Shortcuts

| Shortcut | Action |
|----------|--------|
| `-` / `*` + Space | Bullet list |
| `1.` + Space | Numbered list |
| `#` / `##` / `###` + Space | Heading |
| `>` + Space | Quote |
| Ctrl/Cmd + N | New page |
| Ctrl/Cmd + S | Save |
| Ctrl/Cmd + K | Focus search |
| Tab / Shift+Tab | Next / previous table cell |

## Privacy

- Everything stays on your computer
- No server, no account, no cloud sync
- Data = plain Markdown files you can open with any editor

## License

MIT
