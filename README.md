# AUTOCLIP — Deploy Instructions (Free, No Server Cost)

This turns your phone-only file into a real website with a proper `https://` link — the
same fix that made your other GitHub + Render project actually work. Once it's on
GitHub Pages, the mic and file picker will work correctly (they're blocked on a plain
local file, which is exactly what broke last time).

## Steps (do this on your phone, using GitHub's mobile site or app)

1. Go to github.com and log into your existing account (the one you used for the other project).
2. Tap **+ → New repository**.
3. Name it anything, e.g. `autoclip`. Set it to **Public**. Create it.
4. Inside the new repo, tap **Add file → Upload files**.
5. Upload the `index.html` file from this folder.
6. Commit the upload (straight to the `main` branch).
7. Go to the repo's **Settings** tab → **Pages** (left sidebar).
8. Under "Build and deployment", set **Source: Deploy from a branch**, **Branch: main**, folder: `/ (root)`. Save.
9. Wait about a minute, then refresh — GitHub will show your live link:
   `https://<your-username>.github.io/autoclip/`
10. Open that link on your phone in Chrome. Upload a video, tap Start — mic and file
    picker will now work properly since it's a real HTTPS site.

## What's next once this is live

Right now captions are transcribed by playing your video's audio into your phone's
mic — that's the only 100%-free method with no server. If accuracy isn't good enough
for real use once you test it, the next upgrade is wiring in a proper speech-to-text
API (free tier available on services like AssemblyAI or Deepgram) — that needs a
small backend to hide the API key, which is the same kind of setup you already did
on Render. Tell me when you're ready and I'll build that version too.
