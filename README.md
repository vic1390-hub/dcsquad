DC Squad — Desmond Choo's AI Communications Team
A private AI-powered communications tool built for the office of Mr Desmond Choo, Member of Parliament for Tampines Changkat SMC, Minister of State for the Ministry of Defence, and Deputy Secretary-General of NTUC.
---
What this is
DC Squad is a browser-based app with five specialised AI agents, each trained on Mr Choo's public roles, key messages, and communications context.
Agent	Role
Iris	Sentiment & Research — monitors public opinion, media coverage, and narrative gaps
Cleo	Content Calendar Planner — builds weekly/monthly social media plans, synced to Google Calendar
Wren	Social Copywriter — drafts Facebook and Instagram posts in Mr Choo's voice
Arlo	Communications Strategist — positioning, message frameworks, crisis response
Nova	Newsletter Designer — writes the resident newsletter for Tampines Changkat
---
Access
🔗 Live app: `https://vic1390-hub.github.io/dc-squad`
To use the app you need:
An Anthropic API key — get one at console.anthropic.com
(Optional) A Google OAuth Client ID — to connect Cleo to Mr Choo's Google Calendar
Both are entered on the setup screen when you first open the app. They stay in your browser only — nothing is stored on any server.
---
Setup
Anthropic API key
Go to console.anthropic.com → API Keys → Create key
Paste it into the setup screen when you open the app
Google Calendar (for Cleo)
Go to console.cloud.google.com → create a project called `DC Squad`
Enable the Google Calendar API
Go to APIs & Services → Credentials → Create Credentials → OAuth client ID → Web application
Add `https://vic1390-hub.github.io` as an Authorised JavaScript origin
Copy the Client ID and paste it into the setup screen
---
Updating the app
Edit `index.html` directly on GitHub (click the file → pencil icon)
Commit changes — the app redeploys automatically within ~1 minute
---
Security notes
API keys are entered at runtime and stored only in browser memory — they are cleared when the tab is closed
No data is logged or stored on GitHub or any third-party server
All AI calls go directly from your browser to Anthropic's API
Calendar access is read-only and session-based (re-authorised each session)
This repository should remain private if sensitive communications are discussed in agent chats
---
Built with
Anthropic Claude API — claude-sonnet-4-20250514
Google Calendar API — read-only calendar access
Vanilla HTML/CSS/JS — no frameworks, no build step, runs entirely in the browser
---
For issues or updates, edit `index.html` directly or contact the team that set this up.
