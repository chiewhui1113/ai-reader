<div align="center">

# 📖 AI Reader · Ask While You Read

**A free, single-file PDF reader with a built-in AI tutor. Select any text and get an explanation right where you are — no copy-paste, no switching apps.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![No build](https://img.shields.io/badge/build-none-brightgreen)
![Single file](https://img.shields.io/badge/single--file-HTML-orange)
![100% client-side](https://img.shields.io/badge/100%25-client--side-success)
![PRs welcome](https://img.shields.io/badge/PRs-welcome-ff69b4)

English · [中文](README.zh.md)

</div>

---

> Reading a dense book or paper and hit a paragraph you don't get? Instead of breaking your flow to open ChatGPT and paste it, just **highlight it** — the AI explains, translates, or summarizes it in a side panel, in plain language with examples.

## ✨ Features

- **🖱️ Select-to-ask** — highlight any text → **Explain · Translate · Summarize · Highlight · Ask**
- **📚 Bookshelf** — import multiple PDFs with covers and reading progress
- **🔖 Resume & bookmarks** — auto-remembers where you left off; one-tap bookmarks
- **🖍️ Highlights + notes** — mark passages, attach notes, manage them in one place
- **🔎 AI page finder** — describe what you're looking for in plain words; AI points you to the right page
- **🎯 Three ask scopes** — selected text / current page / **the whole book**
- **💬 Per-book chat history** — conversations are saved separately for each book
- **🌗 Light / Sepia / Dark** reading themes
- **🌐 Bilingual UI** — switch between English and 中文 in one click
- **📱 Works everywhere** — phone and desktop, just a URL

## 🔒 Private & free by design

There is **no server**. Your books, progress, highlights and chats live in **your own browser** (IndexedDB) and never leave your device. AI runs on **your own free [Google Gemini](https://aistudio.google.com/app/apikey) key** and quota. That means: deploy once, and any number of people can use it — each with their own storage and quota, at **zero cost to the host**.

## 🚀 Deploy in 3 steps (GitHub Pages)

1. Create a repo (e.g. `ai-reader`) and upload `index.html`, `LICENSE`, `.nojekyll`.
2. **Settings → Pages → Source** → `Deploy from a branch` → `main` + `/ (root)`, save.
3. Wait a minute, get `https://<username>.github.io/ai-reader/`, share the link.

Your friends don't touch GitHub at all — they just open the link. The only one-time step for each person: paste their own free Gemini key in **⚙ Settings**.

## 🔑 First run

Open **⚙ Settings** → grab a free key at [aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey) → paste it. The key is stored only in your browser. Recommended model: `gemini-2.5-flash-lite` (highest free quota).

> Prefer not to deploy? You can also just open `index.html` locally — but Chrome blocks storage for `file://` pages, so use Firefox or run `python -m http.server` for full memory.

## 🛠️ Tech

One static HTML file: vanilla JS + [PDF.js](https://mozilla.github.io/pdf.js/) (CDN) + IndexedDB + Google Gemini API. No build, no dependencies, no tracking.

## 🤝 Contributing

Issues and PRs are welcome. If this saved you a few hundred copy-pastes, a ⭐ helps others find it!

## 📄 License

[MIT](LICENSE)
