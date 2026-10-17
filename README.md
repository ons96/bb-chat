# BB Chat

A feature-rich, single-file HTML/JS browser chat client supporting OpenRouter, Groq, and Gemini LLM providers, with integrated DuckDuckGo and Brave web search capabilities and local persistent storage.

## Features
- Multi-provider support (OpenRouter free models, Groq fast inference, Google Gemini)
- Integrated Web Search (DuckDuckGo instant answers without API keys, Brave Search)
- Client-side storage via localStorage
- Responsive single-file design (`index.html`)

## Usage

Open `index.html` in a browser, or serve the directory with a local static HTTP
server:

```bash
python3 -m http.server 8080
```

Then visit `http://127.0.0.1:8080/`.

## Security and privacy

The client stores provider settings, API keys, and conversation history in the
browser's `localStorage` so the single-file app can reload them. Use it only on
a trusted device and clear the site's storage when finished. Never commit keys
or paste them into issue comments. Provider requests go directly from the
browser to the configured provider; a provider may require CORS support.
