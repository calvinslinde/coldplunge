# Cold Plunge Tracker

A small app for building cold-water tolerance: log each session, get a goal that scales itself (it adds fewer seconds as sessions get longer), and talk to a coach built on Google's Gemini. Installs as a home-screen app and works offline.

**Use it:** https://calvinslinde.github.io/coldplunge/

## What's here

- `index.html`, `app.js`, `style.css`: the whole app. No build step.
- `sw.js`, `manifest.json`: offline support and install-to-home-screen.

## The coach

The coach calls Gemini directly from the browser with a key you paste into Settings (a Google AI Studio key). The key stays in your browser's storage; nothing is sent anywhere but Google. Without a key, everything else still works.

## Run it locally

```
python3 -m http.server 8000
```

Then visit http://localhost:8000/.

Built with Claude.
