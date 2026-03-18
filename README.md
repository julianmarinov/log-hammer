# 🔨 Log Hammer

**A free, open-source QSO journal for amateur radio operators.**
No installation. No server. No account. Just open the HTML file and start logging.

> Built for everyday use — not for contests, but for the conversations that matter.

![Log Hammer Screenshot](https://lz1bex.eu/wp-content/uploads/2026/03/screenshot-2026-03-18-at-21.49.51-scaled.png)
<!-- Replace with actual screenshot path after upload -->

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Made for HAM Radio](https://img.shields.io/badge/Made%20for-HAM%20Radio-blue.svg)]()
[![Single File App](https://img.shields.io/badge/App-Single%20HTML%20File-orange.svg)]()

---

## What is Log Hammer?

Log Hammer is a browser-based QSO logging application that runs entirely on your local machine. All data is stored as plain `.md` (Markdown) files in a folder of your choice — readable in any text editor, fully yours, never uploaded anywhere.

It is **not** a contest logger. It is designed for structured, note-rich everyday logging:
- Who did you talk to, when, and what was it about?
- Notes, impressions, hashtags for quick retrieval
- Full history per callsign, searchable at any time

---

## Features

- 📋 **Chronological QSO log** — entries grouped by date, newest first
- ⏱ **Live / Manual time** — auto-inserts current time (local + UTC), with manual override and two-way sync between local and UTC fields
- 💾 **Local file storage** — saves to `.md` files via the File System Access API; auto-saves every 5 seconds
- 📁 **Monthly or yearly log files** — configured in Settings; notifies you when a new period begins
- 🔍 **Full-text search** — highlights matches inline, with prev/next navigation
- 📡 **Callsign filter** — see all QSOs with a specific station, with autocomplete
- 🏷 **Hashtags** — type `#tag` in any note; tags appear automatically in the sidebar; case-insensitive
- ✏️ **Inline editing** — click any entry to edit callsign, notes, date and time
- 🌍 **Cyrillic / Bulgarian support** — full Unicode support in all fields
- 🌙 **Dark / light theme** — toggle with one click
- ⚙️ **Settings** — callsign, file mode, language (English / Bulgarian); saved as JSON in the working folder
- 📄 **Human-readable file format** — `.md` files are plain text, editable in any editor

---

## Getting Started

### Requirements

| Browser | Support |
|---|---|
| Google Chrome 86+ | ✅ Full |
| Microsoft Edge 86+ | ✅ Full |
| Firefox | ⚠️ Partial (no direct file write) |
| Safari | ❌ Not supported |
| Mobile browsers | ❌ Not supported |

Works on **Windows**, **macOS**, and **Linux**.

### Usage

1. **Download** `Log-Hammer.html` from the [Releases](../../releases) page
2. **Open** it in Google Chrome or Microsoft Edge — no installation needed
3. Click **📂 Working Folder** and select a folder on your computer
4. If the folder is empty, you'll be prompted to create your first log file
5. Start logging — type a callsign, press **Tab**, add notes, press **Enter**

That's it.

---

## File Format

Log files are stored as standard Markdown:

```markdown
# March 2026 QSO Log

Station: LZ1BEX
Period: 2026-03-01 - 2026-03-31 | Log entries: 42

## 2026-03-18

- [09:55 UTC] - LZ1VIM Great signal on 20m, discussed antenna projects #yagi
- [07:37 UTC] - LZ3MTH Talked about the weather and 40m propagation #40m

## 2026-03-17

- [18:22 UTC] - LZ5AE First contact after long time, will try 17m next #interesting
```

Files are fully portable — copy them to any computer, open them in any text editor, or version-control them with Git.

---

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl+F` | Focus search bar |
| `Ctrl+S` | Manual save |
| `Tab` / `Enter` in callsign field | Move to notes |
| `Enter` in notes | Save entry |
| `Shift+Enter` in notes | New line in notes |
| `Escape` | Cancel / clear |
| `Enter` in search | Next match |

---

## Settings

Click **⚙** in the top-right corner to configure:

- **Station callsign** — your own callsign, shown in the log header
- **File organization** — monthly (`2026-03.md`) or yearly (`2026.md`)
- **Language** — English or Български (Bulgarian)

Settings are saved as `loghammer-settings.json` in your working folder and loaded automatically on next launch.

---

## Project Structure

```
Log-Hammer.html      ← The entire application (HTML + CSS + JS, single file)
README.md            ← This file
LICENSE              ← MIT License
screenshot.png       ← Application screenshot
```

There are no dependencies, no build steps, and no package manager. The entire application is a single self-contained `.html` file.

---

## Contributing

Contributions are welcome. If you have an idea, found a bug, or want to improve something:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-idea`)
3. Commit your changes
4. Open a Pull Request

For questions or ideas you can also reach out directly:
📬 **qso@lz1bex.eu**

---

## Roadmap

- [ ] Export to ADIF
- [ ] PDF export of log
- [ ] PWA / mobile-friendly version with IndexedDB storage
- [ ] English documentation

---

## License

```
MIT License

Copyright (c) 2026 LZ1BEX

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## About

Built with ❤️ by **LZ1BEX** — a Bulgarian amateur radio operator who wanted a better way to keep notes from the shack.

🌐 [lz1bex.eu](https://lz1bex.eu) &nbsp;·&nbsp; 📬 [qso@lz1bex.eu](mailto:qso@lz1bex.eu)

*73 de LZ1BEX*
