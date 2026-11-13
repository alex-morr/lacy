# Lacy — a free local-first iPhone web app

This is a static progressive web app (PWA). It has no server, subscriptions, API keys, or automatic access to your private accounts.

## Features
- Home dashboard with counts, upcoming events, and quick actions
- Create/edit/complete/delete tasks; priority, due date, and search
- Create/edit/delete scheduled events and import `.ics` calendar events (one-time import; not sync)
- Draft, edit, copy, and delete message replies (never sends texts)
- Safe shortcut links to ChatGPT, Gmail, Google Calendar, and an optional secure OpenClaw URL
- Local browser storage and JSON backup/restore
- Offline functionality after a successful visit on HTTPS

## Install on your iPhone (free)
1. Upload **all files** in this folder to a static HTTPS host you trust (such as GitHub Pages). The repository can be public, but **do not upload personal drafts or backups**; this folder only contains app code.
2. Open the resulting HTTPS URL in Safari on your iPhone.
3. Tap the Share button → **Add to Home Screen** → Add.
4. Open **Lacy** from the home screen.

GitHub Pages example: make a repository named `lacy-app`, upload these files, open Settings → Pages → Deploy from branch, then select `main` and `/ (root)`. The URL usually becomes `https://YOUR-USERNAME.github.io/lacy-app/`.

**Privacy:** tasks, event entries and drafts are stored in localStorage on each browser/device, not encrypted in a database or synchronized across devices. Other apps, anyone who can access your unlocked device, or malicious browser extensions could potentially access stored content. Avoid entering sensitive messages; export backups only to trusted locations. Clearing browser data can delete entries. If you host on GitHub Pages, the source code is public but **your entered data is not uploaded to GitHub** by this app.

**Limitations:** This is a functional local planner and message-draft manager, not a production backend assistant. It does not have access to ChatGPT tools or automatically read Gmail, Calendar, iMessage, or OpenClaw. The optional OpenClaw link only opens your existing Gateway; never enter a token in a saved URL. For live integrations, a secure backend and relevant authorizations would need to be designed and implemented separately.
