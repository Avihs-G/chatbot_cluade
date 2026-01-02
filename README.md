# chatbot_cluade

This repository contains a small demo that uses the `puter` client-side JavaScript SDK to talk to the Claude model and present a streaming chat interface.

Files
- `index.php` — a tiny example that calls `puter.ai.chat()` (from the vendor script) and prints a response.
- `chat_bot.html` — a simple chat UI that streams AI responses and supports code blocks (copyable) for generated page files.

Usage
1. Open `chat_bot.html` in your browser (for a local dev server you can run `python -m http.server` or use any static server).
2. Type a website requirement into the input (press Enter to send). Examples:
   - "Build a single-page product landing page with a hero, features, and signup form."
   - "Create a 3-page portfolio with home, projects, and contact pages; minimal responsive design."
   - "Generate an index and post page for a blog in plain HTML/CSS/JS."
3. The AI (model: `claude-sonnet-4.5`) will stream a response into the chat; code blocks are displayed in a copyable box.

Notes
- This is a demo for prototyping and learning how to build conversational UIs; secure keys and production integration are not included.
- The UI uses `https://js.puter.com/v2/` as in `index.php` to reach the AI model.


Feel free to open `chat_bot.html` and try example prompts — the assistant will return page code and short explanations.