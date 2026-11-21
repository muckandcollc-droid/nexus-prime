# NEXUS-PRIME | Solo Encrypted Financial Command Center

A zero-knowledge, blank-slate personal bill and debt payoff dashboard engineered for private GitHub Pages hosting and Android tablet PWA installation.

## Security Architecture
- **Zero Hardcoded Data:** `index.html` ships as a 100% blank `$0.00` template—no account numbers, balances, or API keys exist in source control.
- **Client-Side AES-256-GCM Encryption:** Enabling **Set PIN Lock** derives a non-extractable key via `PBKDF2-SHA256` (310,000 iterations) and encrypts all local state at rest with a fresh 96-bit IV on every write.
- **Portable `.nexusvault` Backups:** Export encrypted backup files to your device's Downloads folder (excluded from Git via `.gitignore`).
- **Backend Relay for xAI:** Keep `XAI_API_KEY` strictly in a local `.env` file behind a server proxy—never in frontend HTML.

## Quick GitHub Pages Setup
1. Create a **Private** repository on GitHub and upload `index.html`, `.gitignore`, `manifest.json`, and `README.md`.
2. Go to **Settings > Pages**, set **Source** to `Deploy from a branch` (`main` / `root`), and save.
3. Open your live Pages URL in Chrome on your Android tablet, tap **Add to Home screen**, and tap **Set PIN Lock** inside the app.
