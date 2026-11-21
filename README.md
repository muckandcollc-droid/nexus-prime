# NEXUS-PRIME | Solo Encrypted Financial Command Center (All-in-One Release)

A zero-knowledge, blank-slate personal bill and debt payoff PWA engineered for private/public GitHub Pages hosting and Android tablet installation.

## Key Capabilities
- **Zero Hardcoded Data**: Ships as a clean `$0.00` template in source control with no hardcoded credentials, account balances, or API keys.
- **AES-256-GCM Local Vault Encryption**: Optional PIN lock derives a non-extractable key via `PBKDF2-SHA256` (310,000 iterations) with a fresh 96-bit IV on every write and 10-minute idle auto-lock.
- **Password-Gated Developer Mode**: Boots cleanly into **User Mode** (`Dashboard`, `Bills & Credit`, `Statement OCR`, `Security & Backup`, plus **Export CSV**). Entering your salted `PBKDF2-SHA256` Developer Password unlocks **Gemini Copilot**, **AI Bot Farm** (Three.js 3D cyber-city), **Live xAI Console**, and **Test Operations**.
- **Local Statement OCR & Quick CSV Export**: Scan statements locally via `Tesseract.js`, export `.csv` ledgers anytime, and back up/restore encrypted `.nexusvault` snapshots.
- **PWA Ready**: Includes `192x192` and `512x512` PNG icons and `manifest.json` for Chrome home-screen installation on Android.
