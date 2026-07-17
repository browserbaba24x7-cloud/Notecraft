Notecraft — Smart Notes
A beautiful, fast, and fully offline note-taking Progressive Web App. Organize your thoughts with rich text editing, color-coded notes, folders, and instant search — all saved locally in your browser.

Notecraft

Features
Writing
Rich Text Editor — Bold, Italic, Underline, Strikethrough
Headings — H1, H2, H3 for structured notes
Lists — Bullet lists and numbered lists
Checkboxes — Interactive task items with check/uncheck
Code Blocks — Inline code and code blocks with monospace font
Blockquotes — Highlight important quotes
Dividers — Horizontal rules to separate sections
Tab Indentation — Press Tab to indent inside the editor
Organization
Folders — Create, rename, and delete custom folders
Color Coding — 10 colors to visually tag each note
Pin Notes — Pin important notes to the top of the list
Duplicate Notes — One-click clone of any note
Instant Search — Search across all notes by title or content
"All Notes" View — See every note across all folders
Data & Storage
Auto-Save — Notes save automatically as you type (600ms debounce)
Local Storage — All data stays in your browser, nothing sent to any server
Storage Monitor — Live storage usage bar in the status bar
Quota Handling — Graceful error handling when storage is full
Export — Download all notes as a .txt file
Clear Data — One-click reset to start fresh
HTML Cleanup — Automatically strips bloated contenteditable junk to save space
PWA & Install
Install as App — Works on Android, iOS, Desktop (Chrome, Edge, Safari)
Standalone Mode — No browser UI when installed
Custom Icons — Favicon, Apple Touch Icon, PWA manifest icons (192px & 512px)
Install Banner — Auto-appears when browser supports installation
Theme Color — Amber accent color in browser chrome
Design
Dark Theme — Easy on the eyes with warm amber accents
Animated Background — Subtle floating glow effects
Smooth Transitions — Every interaction has polish
Responsive — Full mobile support with slide-out sidebar
Keyboard Shortcuts — Power user friendly
Word & Character Count — Live counter below each note
Keyboard Shortcuts
Shortcut	Action
Ctrl + N	Create new note
Ctrl + B	Bold
Ctrl + I	Italic
Ctrl + U	Underline
Ctrl + Shift + F	Focus search
Tab	Indent in editor
Escape	Close modals / sidebar
File Structure
notecraft/
│
├── index.html # Main application (single file)
├── README.md # This file
│
├── favicon.svg # Browser tab icon (SVG, modern browsers)
├── favicon.ico # Browser tab icon (ICO, legacy support)
├── favicon-96x96.png # Browser tab icon (PNG fallback)
│
├── apple-touch-icon-n.png # iOS home screen icon (180x180+)
│
├── web-app-manifest-192x192.png # PWA icon — small (Android, Chrome)
├── web-app-manifest-512x512.png # PWA icon — large (Android, Chrome)
│
└── site.webmanifest # PWA manifest configuration


---

## Setup

### Quick Start (No Server Needed)

1. Download or clone all files into one folder
2. Open `index.html` directly in your browser
3. Start taking notes — everything works immediately

### With a Local Server (Recommended for PWA)

```bash
# Using Python
python -m http.server 8080

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8080

Why a server? The PWA install feature and service workers require serving over HTTP/HTTPS. Opening the HTML file directly (file://) works for everything except the install prompt.

Installing as an App
Android (Chrome)
Open the page in Chrome
Tap the "Install" banner at the bottom (or tap ⋮ menu → "Install app")
Notecraft appears on your home screen with the feather icon
iOS (Safari)
Open the page in Safari
Tap the Share button (square with arrow)
Scroll down and tap "Add to Home Screen"
The feather icon appears on your home screen
Desktop (Chrome / Edge)
Open the page in Chrome or Edge
Click the install icon in the address bar (⊕ or ↓)
Or click ⋮ menu → "Install Notecraft"
App opens in its own window with the icon in your taskbar/dock
How Data Works
All notes and folders are stored in localStorage under the key notecraft_data
Data persists across browser sessions — closing the tab does NOT delete your notes
Clearing browser data / cache WILL delete your notes
Use Export before clearing data if you want a backup
Storage limit is typically 5MB per origin (varies by browser)
The status bar shows live storage usage with a color-coded bar:
🟢 Green — under 50%
🟡 Yellow — 50-80%
🔴 Red — over 80%
Browser Support
Browser
Notes
PWA Install
Chrome 80+	Full support	Yes
Edge 80+	Full support	Yes
Firefox 80+	Full support	No (not supported by Firefox)
Safari 15+	Full support	Yes (via Add to Home Screen)
Mobile Chrome	Full support	Yes
Mobile Safari	Full support	Yes
Samsung Internet	Full support	Yes

Technology
HTML5 — Semantic markup
CSS3 — Custom properties, flexbox, animations, backdrop-filter
Vanilla JavaScript — Zero dependencies, no framework
ContentEditable API — Rich text editing
LocalStorage API — Persistent data storage
Web App Manifest — PWA configuration
Before Install Prompt API — Install banner
Google Fonts — Space Grotesk + JetBrains Mono
Font Awesome 6 — Icon library
Generating Icons
Icons were generated using RealFaviconGenerator:


have a miner update
