📝 NoteCraft
A beautiful, fast, and fully responsive note-taking web app built with pure HTML, CSS, and Vanilla JavaScript. NoteCraft allows you to organize your thoughts using nested folders, rich text formatting, and local storage persistence—all without needing a backend or database.

NoteCraft License Made with

✨ Features
📁 Nested Organization: Create colorful folders to group related notes together.
✍️ Rich Text Editor: Format your notes with headings, bold/italic/underline text, lists, quotes, code blocks, and custom text colors.
🖱️ Drag & Drop: Easily move notes between different folders.
🔒 Passcode Locking: Secure individual notes or entire folders with a passcode to prevent unauthorized viewing.
📌 Pin Notes: Keep your most important notes pinned to the top of the folder.
🔍 Instant Search: Quickly filter notes by title or content directly from the sidebar.
🗑️ Trash Bin: Safely delete notes or folders. Restore them easily or permanently delete them.
🎨 Customizable UI: Choose from 10 vibrant colors for your folders. Includes a sleek, dark-themed interface with ambient background glows.
💾 Auto-Save: All data is automatically saved to your browser's localStorage. No account or internet connection required.
⌨️ Keyboard Shortcuts: Fast navigation and note creation.
📱 PWA Ready: Meta tags configured for installation on mobile and desktop home screens.
🛠️ Tech Stack
HTML5: Semantic structure and PWA configuration.
CSS3: Custom properties (variables), Flexbox, smooth transitions, and animations. Fully responsive layout.
Vanilla JavaScript (ES5/ES6): DOM manipulation, state management, and localStorage integration.
Font Awesome 6: For crisp, scalable icons.
Google Fonts: Space Grotesk for headings and DM Sans for body text.
🚀 Getting Started
Because NoteCraft is built entirely with front-end technologies, getting it running is incredibly simple.

Prerequisites
You just need a modern web browser (Chrome, Firefox, Edge, Safari).

Installation & Running
Download/Clone the repository:
bash

git clone https://github.com/your-username/notecraft.git
Navigate to the project folder:
bash

cd notecraft
Add Icons (Optional but recommended):
Ensure you have a ./favicon/ folder containing the following files (as referenced in the HTML):
favicon.svg
favicon-96x96.png
favicon.ico
apple-touch-icon.png
Run the app:
Simply open the index.html file in your web browser.
bash

# If you are using VS Code, you can use Live Server
# Or just double-click the index.html file
⌨️ Keyboard Shortcuts
Shortcut
Action
Ctrl + N	Create a new note
Esc	Close sidebar, modals, or context menus

📂 Project Structure
text

.
├── index.html          # Main HTML file containing structure, styles, and scripts
├── favicon/            # Folder containing app icons
│   ├── favicon.svg
│   ├── favicon-96x96.png
│   ├── favicon.ico
│   └── apple-touch-icon.png
└── README.md           # This file
🧠 How It Works
State Management: The app maintains a global folders and trash array. Every time a change is made (create, edit, delete, drag), the state is updated and saveData() writes the JSON stringified state to localStorage.
Rendering: The render() function dynamically rebuilds the sidebar folder tree and note list based on the current state, applying active states, colors, and pinned items.
ContentEditable: The main editor uses a contenteditable div. The toolbar utilizes document.execCommand to apply rich text formatting (bold, italic, lists, etc.).
🛡️ Data Privacy
NoteCraft stores all data locally in your browser's Local Storage.

No data is ever sent to a server.
Clearing your browser's cache/site data will permanently delete your notes. (Consider exporting your notes manually if you clear your browser frequently).

Made with ❤️ and Vanilla JS.