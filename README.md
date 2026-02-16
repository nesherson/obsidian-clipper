# Obsidian Clipper

A Firefox/Zen browser extension that captures selected text, mathematical formulas,
and images from Math Academy directly into an Obsidian note.

## Setup

### 1. Install the Obsidian Local REST API plugin

In Obsidian: **Settings → Community plugins → Browse → "Local REST API"**

After installing, note the **API key** from the plugin settings page.
The plugin runs on port `27123` by default.

### 2. Load the extension in Zen / Firefox

1. Open `about:debugging` in Zen browser
2. Click **"This Firefox"** in the sidebar
3. Click **"Load Temporary Add-on…"**
4. Select the `manifest.json` file inside this folder

### 3. Configure the extension

Click the extension icon in the toolbar. Enter:

- **Target note path** — e.g. `Math Academy/Captured Notes.md` (relative to your vault)
- **API port** — `27123` unless you changed it
- **API key** — from the Local REST API plugin settings

Click **Test connection** to verify, then **Save**.

## Usage

1. Open any Math Academy lecture
2. Select text or a formula on the page
3. Press **Ctrl+Alt+C** (or your custom shortcut)
4. A green toast notification confirms the capture

The captured content is appended to your target note;
