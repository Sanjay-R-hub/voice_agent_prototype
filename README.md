# voice_agent_prototype
voice agent that helps people learn vocabulary
# Say It — Voice Vocabulary Tutor

A browser-based voice vocabulary tutor. Speaks a word aloud, listens to your
spoken (or typed) answer via the Web Speech API, and gives instant feedback.

No build step, no dependencies, no backend — it's a single static HTML file.

## Deploy on GitHub + Vercel

1. **Create a new GitHub repo**
   - Go to github.com → New repository → name it e.g. `voice-vocab-tutor`
   - Keep it Public (Vercel's free tier needs this, or a connected private repo)

2. **Upload this file**
   - On the new repo page, click "uploading an existing file"
   - Drag in `index.html` from this folder
   - Commit directly to the `main` branch

3. **Deploy on Vercel**
   - Go to vercel.com → sign in with your GitHub account
   - Click "Add New" → "Project"
   - Select the `voice-vocab-tutor` repo → click "Import"
   - Leave all settings as default (Vercel auto-detects static HTML — no
     framework, no build command needed)
   - Click "Deploy"

4. Vercel gives you a live URL like `voice-vocab-tutor.vercel.app` within
   about 30 seconds. That's your public, no-login-required link — test it
   in an incognito window before submitting anywhere.

## Notes

- Needs Chrome or Edge for the voice input (Web Speech API support is weak
  in Safari/Firefox) — text input works everywhere as a fallback.
- Needs microphone permission — the browser will prompt for it on first use.
- All logic runs client-side in the browser; nothing is sent to a server.
