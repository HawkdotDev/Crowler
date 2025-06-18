# Crowler

**Crowler** is a modern, open-source desktop application for full-stack SEO audits — like Screaming Frog meets Yoast, built with **Electron** & **Bun**.

It provides deep technical SEO analysis, keyword audits, performance scoring, link mapping, accessibility checks, and AI-assisted recommendations — all in a sleek, cross-platform desktop app.

---

## ✨ Features

- 🔍 Full-site crawling with JavaScript rendering (via Playwright)
- 🧠 Metadata & keyword analysis (titles, descriptions, density)
- 🏷️ Heading structure mapping (H1–H6 validation with hierarchy check)
- 🔗 Internal link graph with orphan page detection
- 🖼️ Image SEO (missing alt, decorative detection, format suggestions)
- 📦 Asset optimization & lazy loading audit
- 🔧 Schema.org, canonical tag, and robots.txt validation
- ⚡ Core Web Vitals via Lighthouse integration
- ♿ Accessibility compliance checks (WCAG 2.1 via axe-core)
- 📊 Google Search Console & GA4 API integration
- 📁 Export reports as PDF, CSV, or JSON
- 📈 Timeline-based scoring & improvement tracking
- ✅ Smart to-do list with severity and fix suggestions

---

## 🛠️ Tech Stack

| Layer           | Technology                                |
|----------------|--------------------------------------------|
| UI              | Electron, React, Tailwind CSS              |
| Runtime         | **Bun** (instead of Node.js)               |
| Crawler Engine  | Playwright, Cheerio                        |
| Auditors        | Lighthouse, axe-core, custom logic         |
| Storage         | SQLite (via `better-sqlite3`)              |
| Exporting       | jsPDF, csv-writer                          |
| APIs            | Google Search Console, Google Analytics    |

---

## 🚀 Getting Started (Bun)

```bash
# Clone the repo
git clone https://github.com/your-username/crowler.git
cd crowler

# Install dependencies
bun install

# Start development
bun run dev
````

> ⚠️ Playwright will install browser binaries if not already installed. You may need to run:
> `bunx playwright install`

---

## 📦 Build for Distribution

```bash
bun run build
```

> Uses `electron-builder` under the hood for Mac, Windows, and Linux packaging.

---

## 📚 Scripts (via Bun)

```bash
bun run dev        # Start Electron + Vite/React in dev mode
bun run lint       # Lint code
bun run format     # Format code with Prettier
bun run build      # Build the app for production
```

---

## 📂 Project Structure

```
crowler/
├── bunfig.toml
├── electron/
│   └── main.ts       # Main Electron process
├── src/
│   ├── App.tsx       # React UI
│   ├── components/   # UI components
│   ├── engine/       # Crawling & auditing logic
│   ├── db/           # SQLite integration
│   └── utils/        # Utilities (export, analysis, etc.)
└── public/
```

---

## 🤝 Contributing

Crowler is open-source and welcomes contributions!

* Fork the repo
* Create a new branch
* Submit a PR with clear description
* Discuss major ideas in an issue first!

```bash
bun run lint
```

> See [CONTRIBUTING.md](CONTRIBUTING.md) for more.

---

## 📄 License

MIT © 2025 Dwaipayan Dutta

---

## 🧠 Philosophy

Crowler is built to empower developers, marketers, and analysts with the **freedom** and **depth** of a Screaming Frog-style engine — but in an open, extensible, and beautifully visualized format.

---

### 🐾 Crawl. Audit. Improve. With **Crowler**

```
