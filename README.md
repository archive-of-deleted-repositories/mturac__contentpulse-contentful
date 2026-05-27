<!-- ContentPulse Contentful — Semantic Decay & Freshness Engine -->

<p align="center">
  <a href="https://github.com/mturac/contentpulse-contentful">
    <img src="https://img.shields.io/badge/🚀_ContentPulse-Contentful_App-2478CC?style=for-the-badge&logo=contentful&logoColor=white" alt="ContentPulse Contentful" />
  </a>
</p>

<h1 align="center">
  <img src="https://raw.githubusercontent.com/simple-icons/simple-icons/develop/icons/contentful.svg" width="48" alt="Contentful" />
  <br/>
  ContentPulse for Contentful
</h1>

<p align="center">
  <strong>🔍 Detect outdated content before your readers do.</strong>
</p>

<p align="center">
  <em>A Contentful App that automatically detects semantic decay in your content — stale dates, outdated version references, and aging information.</em>
</p>

<p align="center">
  <a href="#-quick-start">Quick Start</a> · <a href="#-features">Features</a> · <a href="https://github.com/mturac/contentpulse-contentful/stargazers">⭐ Star</a>
</p>

---

<p align="center">
  <img src="https://img.shields.io/github/stars/mturac/contentpulse-contentful?style=social" alt="GitHub stars" />
  <img src="https://img.shields.io/github/forks/mturac/contentpulse-contentful?style=social" alt="GitHub forks" />
  <img src="https://img.shields.io/github/issues/mturac/contentpulse-contentful?style=social" alt="GitHub issues" />
</p>

---

## 📊 Badges

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue?style=flat-square" alt="Version 1.0.0" />
  <img src="https://img.shields.io/badge/license-MIT-green?style=flat-square" alt="License MIT" />
  <img src="https://img.shields.io/badge/Contentful-App-2478CC?style=flat-square&logo=contentful&logoColor=white" alt="Contentful App" />
  <img src="https://img.shields.io/badge/TypeScript-5.6-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=white" alt="React" />
  <img src="https://img.shields.io/badge/PRs-Welcome-brightgreen?style=flat-square" alt="PRs Welcome" />
</p>

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🕐 **Date Decay Detection** | Finds stale dates using `chrono-node` natural language parsing |
| 🔖 **Version Decay Detection** | Catches outdated version strings (`v2.0.0`, `2023 edition`) |
| 📊 **Freshness Score** | 0-100 score based on content age and decay severity |
| 🖥️ **Sidebar Widget** | Forma 36 design system sidebar widget |
| 🎯 **Per-Entry Analysis** | Analyzes content on every entry save |
| 🔒 **Privacy-First** | All analysis runs client-side — no external API calls |

---

## 🚀 Quick Start

### 1. Install Dependencies

```bash
npm install
```

### 2. Create Contentful App

1. Go to your Contentful space
2. Navigate to **Apps** → **Create App**
3. Upload the built app or use the Contentful CLI

### 3. Add to Content Type

1. Go to your content model
2. Add the ContentPulse sidebar widget
3. Save the content type

### 4. Done

Create or edit any entry. The freshness score and warnings appear in the sidebar.

---

## ⚙️ Configuration

The app works out of the box with sensible defaults:

| Option | Default | Description |
|--------|---------|-------------|
| `maxAgeDays` | `365` | Days after which a date is considered stale |

---

## 📊 Warning Types & Severity

| Type | Trigger | Severity |
|------|---------|----------|
| `date_decay` | Date exceeds `maxAgeDays` | 🟡-🔴 |
| `version_decay` | Version references old year | 🟡-🔴 |

| Severity | Score Penalty | When |
|----------|---------------|------|
| 🟢 `low` | -5 | Mildly stale |
| 🟡 `medium` | -10 | Moderately stale |
| 🟠 `high` | -15 | Very stale |
| 🔴 `critical` | -25 | Extremely stale |

---

## 🔒 Privacy

- ✅ **Client-Side Only** — All analysis runs in the browser
- ✅ **No External APIs** — Content never leaves the client
- ✅ **No Data Collection** — No analytics or telemetry
- ✅ **Open Source** — Full transparency

---

## 🤝 Contributing

Contributions welcome! Please read our Contributing Guide before submitting PRs.

---

## 📄 License

MIT © [Mehmet Turac](https://github.com/mturac)

---

<p align="center">
  <strong>Made with ❤️ for the Contentful community</strong>
</p>

<p align="center">
  <a href="https://github.com/mturac/contentpulse-contentful/stargazers">
    <img src="https://img.shields.io/badge/⭐_Star_on_GitHub-2478CC?style=for-the-badge&logo=github&logoColor=white" alt="Star on GitHub" />
  </a>
</p>
