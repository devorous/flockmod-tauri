## Flockmod app with Tauri
This application uses Tauri to wrap Flockmod.com/draw/ in a minimal native shell.

Tauri leverages the builtin Webview2 browser on Windows which allows for a small executable size as well as great performance.

### Changes
There are two files I've changed to allow this app to open and run the flockmod website - 
- src-tauri/tauri.conf.json - The main settings file that defines the URL connection as well as window properties.
- src-tauri/capabilities/default.json - The permissions settings for the application.

### Issues 
Currently, there is no way to drag/drop images onto the application - they must be manually selected from the files directory.
I believe this is an issue with redirecting the app to a new URL, and if this were built from source code it would not be a problem.

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
