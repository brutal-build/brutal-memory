<h1 align="center">Brutal Memory</h1>

> <p align="center">A brutalist web app for browsing and exporting conversations from Hermes Agent's <code>state.db</code>. Zero backend, zero uploads — everything runs in your browser.</p>

<p align="center">Built with <strong>Vite 6</strong> + <strong>React 19</strong> + <strong>TypeScript</strong> + <strong>Tailwind CSS v4</strong>. Drop your SQLite database file and browse all your AI conversations locally.</p>

---

## Features

- **Drop & Browse** — drag your `state.db` file into the browser
- **Session List** — all conversations sorted by date
- **Search** — filter sessions by title with debounced input
- **Filters** — source (tui, telegram, cron, discord…), archived status, sort order
- **Chat View** — read conversations with proper formatting
- **Session Details** — model, source, duration, token counts, tool calls
- **Export** — single session as `.md`, all sessions as `.json` or `.zip` of `.md` files

---

## Quick Start

### Prerequisites

- **Node.js 20+**

### 1. Clone and install

```bash
git clone https://github.com/brutal-build/brutal-memory
cd brutal-memory
npm install
```

### 2. Run

```bash
npm run dev
```

Opens at `http://localhost:5173`.

### 3. Build for production

```bash
npm run build
```

Or visit the live demo: **[brutal-memory.vercel.app](https://brutal-memory.vercel.app)**

---

## Usage

1. Open the app
2. Click `[ SELECT FILE ]` or drag your `state.db` file onto the page
3. Browse your sessions

> Your database stays in your browser. Nothing is uploaded.

---

## Where is state.db?

| Platform | Location |
|----------|----------|
| Windows | `%LOCALAPPDATA%/hermes/profiles/<profile>/state.db` |
| macOS | `~/Library/Application Support/hermes/profiles/<profile>/state.db` |
| Linux | `~/.local/share/hermes/profiles/<profile>/state.db` |

---

## Tech Stack

| Layer | Tech |
|-------|------|
| Framework | React 19 |
| Bundler | Vite 6 |
| Language | TypeScript |
| Styling | Tailwind CSS v4 |
| Database | sql.js (SQLite → WebAssembly) |
| State | zustand |
| Export | JSZip |
| Hosting | Vercel |

---

## License

MIT — [brutal-build](https://github.com/brutal-build)
