🦍 BongoOS 11

BongoOS 11 is a fast, lightweight, browser-based desktop operating system inspired by modern glassmorphic UI design—complete with a floating AI purple gorilla desktop assistant (Bongo), a tabbed live web browser (BongoChrome), a simulated Wi-Fi Manager connected to real internet APIs, and a full suite of built-in apps.

Built as a single-file, zero-dependency web app (index.html), BongoOS 11 can be hosted anywhere for free (GitHub Pages, Vercel, Netlify, or itch.io).

✨ Key Features

🦍 Bongo AI Desktop Assistant:

Draggable floating character with mouse-tracking eyes, animations (backflips, dancing, singing), and a speech bubble.

Powered by the Gemini API with real-time web grounding and OS voice/text commands (e.g., "open browser", "search space news", "turn off wifi").

🌐 BongoChrome Web Browser:

Multi-tabbed interface with back/forward history, omnibox search, bookmarks bar, and a DevTools network inspector.

Browse live embeddable sites (Wikipedia, OpenStreetMap) or run real-time AI-grounded web searches.

Offline Mini-Game: Disconnect Wi-Fi in the system tray to unlock the playable Banana Runner arcade game!

📶 Interactive Wi-Fi & System Tray:

Toggle Wi-Fi power, switch networks, test real internet latency, check live weather widgets, and toggle Light/Dark Mica themes.

🪟 Full Window Management:

Draggable, resizable, minimizable, and maximizable glassmorphic windows with dynamic z-index stacking and a centered taskbar.

🧰 Built-in App Suite:

Files & Trash Bin: Persistent virtual file system saved automatically to localStorage.

BongoPad: Rich plain-text editor with live word/character counters and file saving.

BongoShell: Interactive terminal supporting ls, cd, cat, touch, ping, neofetch, and bongo.

Paint Studio: Drawing canvas that saves PNG artwork directly into your virtual Pictures folder.

Banana Sweeper: Classic 8×8 Minesweeper puzzle game.

BongoBeats: Web Audio API chiptune & synth music player.

Calculator, Task Manager & Settings: Live system stats, wallpaper switcher, and power controls.

🚀 Quick Start & Hosting on GitHub Pages

Because BongoOS 11 is self-contained in a single HTML file, deploying it takes less than a minute:

Rename your HTML file to index.html and upload it alongside this README.md and LICENSE to a new GitHub repository.

Go to your repository Settings → Pages.

Under Build and deployment, select Deploy from a branch, choose main (or master) and / (root), and click Save.

Your live OS will be online at https://<your-username>.github.io/<your-repo-name>/!

Enabling Bongo AI on Your Own Site (Optional)

If you want the Gemini-powered AI chat and web overview features to work on your own public deployment:

Get a free API key from Google AI Studio.

In index.html, locate const apiKey = ""; inside callGeminiAPI() and insert your key (note: for public sites, restrict your API key to your GitHub Pages domain in Google Cloud Console).

🛠️ Tech Stack

HTML5 & Vanilla JavaScript (ES6+)

Tailwind CSS (via CDN)

Web Audio API (synthesized UI sound effects and music)

Open-Meteo & Wikipedia Public APIs (live weather and encyclopedia browsing)

Google Gemini API (conversational assistant & search grounding)

📄 License

This project is licensed under the MIT License — see the LICENSE file for details.
