## Flockmod app with Tauri
This application uses Tauri to wrap Flockmod.com/draw/ in a minimal native shell.

Tauri leverages the builtin Webview2 browser on Windows which allows for a small executable size as well as great performance.

## Building from Source

**Prerequisites:**
- [Rust](https://www.rust-lang.org/)
- [Node.js](https://nodejs.org/)

**Steps:**
```bash
git clone https://github.com/devorous/flockmod-tauri.git
cd flockmod-tauri
npm install

# Development
npm run tauri dev

# Production build
npm run tauri build
```

---
