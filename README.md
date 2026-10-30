# TryPad

A lightweight, offline **Notion-style notes app** that runs entirely in the browser (single HTML file).

Notes are saved as **Markdown (`.md`) files** on your local disk. Page hierarchy is mirrored with folders.

## Features

- Hierarchical pages & sub-pages (collapsible tree)
- Sidebar sorted **A–Z** by page title
- Rich text: bold, italic, underline, strikethrough, headings
- Code blocks, hyperlinks, images (resize remembered), tables
- Notion-style typing shortcuts
- Search across all pages and sub-pages
- Resizable left sidebar
- Dark mode (🌙 / ☀️ toggle; preference remembered)
- Local folder storage via File System Access API (Chrome / Edge)
- Remembers last folder (one-click reconnect)

## Requirements

- **Chrome** or **Edge** (File System Access API)
- Not fully supported in Firefox / Safari for local folder saving

## Usage

1. Open **`trypad.html`** in Chrome or Edge
2. Click **Select Folder…** and choose a folder for your notes
3. Create pages, write, insert images / tables / code blocks
4. Use the **moon/sun button** (top-left) to switch light / dark mode
5. Next time you open the app, click **Reconnect** (or it may auto-connect if permission is still granted)

### Suggested layout

```text
TryPad/
  trypad.html         ← this app (single file)
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
| Enter on empty list item | Exit list |
| Enter on empty quote line | Exit quote |
| Tab / Shift+Tab | Indent / outdent (or next table cell) |
| Ctrl/Cmd + N | New page |
| Ctrl/Cmd + S | Save |
| Ctrl/Cmd + K | Focus search |

## Privacy

- Everything stays on your computer
- No server, no account, no cloud sync
- Data = plain Markdown files you can open with any editor

## License

MIT
