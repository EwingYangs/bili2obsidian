# BiliBili Sync for Obsidian

> Automatically sync your BiliBili **favorites** into your Obsidian vault, with optional AI summaries of video transcripts.

English · [简体中文](./README.md) · [Website bilibili.2obsidian.com](https://bilibili.2obsidian.com)

> ⚠️ **This is closed-source software.** It is distributed only as a compiled build (obfuscated `main.js`); the source code is not available. Redistribution, reverse engineering, and modified redistribution are prohibited. See [LICENSE](./LICENSE).

---

## Features

| Capability | Description |
|------------|-------------|
| 📁 Favorites sync | BiliBili favorites folders synced to local Markdown |
| 🖼 Cover download | Video covers saved locally |
| 📜 Transcripts | Video transcripts synced as searchable text |
| 🤖 AI summaries | Optional — summarize transcripts with any OpenAI-compatible model |
| ⏱ Scheduled sync | Background incremental sync on an interval |

## Preview

<!-- TODO: record GIFs into assets/ and replace the placeholders below -->
<!-- ![login](./assets/login.gif) -->
<!-- ![sync](./assets/sync.gif) -->

## Installation

### Option 1 — BRAT (recommended, auto-updates)

1. Install and enable **BRAT** (Beta Reviewer's Auto-update Tool) from Obsidian community plugins
2. Open BRAT and choose **Add Beta plugin**
3. Enter the repository URL:
   ```
   https://github.com/EwingYangs/bili2obsidian
   ```
4. Enable **BiliBili Sync** under **Settings → Community plugins**

> BRAT tracks GitHub Releases and updates to the latest version automatically.

### Option 2 — Manual

1. Download `main.js`, `manifest.json`, `styles.css` from the latest [Release](https://github.com/EwingYangs/bili2obsidian/releases)
2. Create a folder `bili2obsidian` under your vault's `.obsidian/plugins/` and drop the three files in:
   ```
   YourVault/.obsidian/plugins/bili2obsidian/
   ├── main.js
   ├── manifest.json
   └── styles.css
   ```
3. Restart Obsidian and enable the plugin under **Settings → Community plugins**

## Usage

After enabling, go to **Settings → BiliBili Sync**:

1. Click "Log in to BiliBili", scan/sign in inside the popup, then click "Extract Cookie"
2. Configure the root folder, sync interval, and which favorites folders to sync
3. Turn on "Scheduled auto-sync" for background incremental syncing
4. For transcript AI summaries, enable "AI summary" and fill in an OpenAI-compatible API Key / Base URL / model

See the [User Guide](./USER_GUIDE.md) for the full list of settings.

## Free quota & license code

- **100 videos** free trial — all features available, no signup required
- After 100 synced videos, enter a **license code** in settings to keep syncing
- License codes are available via the "Buy license" entry in settings or the [website](https://bilibili.2obsidian.com), bound per device

## Acceptable use

This plugin is intended solely for syncing content **you have the right to access on your own account** into your **personal Obsidian knowledge base**, for personal offline reading and organization.

- ❌ Do NOT use it for bulk crawling/scraping of other people's data or any unauthorized data collection
- ❌ Do NOT use the synced content commercially or redistribute it publicly; you must comply with BiliBili's terms of service and applicable laws
- ⚠️ You are responsible for your own use; you bear all consequences of any misuse

## Privacy & authorization

- Your BiliBili login **cookie is stored only in your local vault** — never uploaded
- Synced content is written only to your local Obsidian vault
- If AI summary is enabled, transcripts are sent to the AI service you configured yourself
- Only the license code and a device identifier are sent to the authorization service for validation (quota & license management)

## Feedback

Questions or suggestions? Open an [Issue](https://github.com/EwingYangs/bili2obsidian/issues) or visit the [website bilibili.2obsidian.com](https://bilibili.2obsidian.com).

## License

**Closed-source software.** Distributed only as a compiled build; the source code is not available. Redistribution, reverse engineering, and modified redistribution are prohibited. See [LICENSE](./LICENSE).
